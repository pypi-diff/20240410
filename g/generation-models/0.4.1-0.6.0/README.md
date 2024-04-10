# Comparing `tmp/generation_models-0.4.1.tar.gz` & `tmp/generation_models-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generation_models-0.4.1.tar", max compression
+gzip compressed data, was "generation_models-0.6.0.tar", max compression
```

## Comparing `generation_models-0.4.1.tar` & `generation_models-0.6.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       13 2023-07-24 17:41:49.366627 generation_models-0.4.1/generation_models/.gitignore
--rw-r--r--   0        0        0       47 2023-07-24 17:41:49.366782 generation_models-0.4.1/generation_models/__init__.py
--rw-r--r--   0        0        0   121753 2024-02-28 19:41:30.255860 generation_models-0.4.1/generation_models/generation_models.py
--rw-r--r--   0        0        0      640 2024-02-29 00:39:39.734150 generation_models-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 generation_models-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-10-12 04:36:37.827057 generation_models-0.6.0/generation_models/.gitignore
+-rw-r--r--   0        0        0       47 2024-04-05 22:18:23.392678 generation_models-0.6.0/generation_models/__init__.py
+-rw-r--r--   0        0        0   128989 2024-04-10 03:52:53.009565 generation_models-0.6.0/generation_models/generation_models.py
+-rw-r--r--   0        0        0      640 2024-04-10 03:52:53.010491 generation_models-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 generation_models-0.6.0/setup.py
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 generation_models-0.6.0/PKG-INFO
```

### Comparing `generation_models-0.4.1/generation_models/generation_models.py` & `generation_models-0.6.0/generation_models/generation_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -509,17 +509,21 @@
                 {
                     "dam prices": dam_prices,
                     "reserve market data": values["reserve_markets"],
                 }
             )
 
         if values["load_peak_reduction"]:
-            _check_lengths(
-                {"rtm prices": values["energy_prices"].rtm, "peak reduction data": values["load_peak_reduction"]}
-            )
+            if isinstance(values["energy_prices"], DARTPrices):
+                rtm = values["energy_prices"].rtm
+            elif isinstance(values["energy_prices"], DARTPriceScenarios):
+                rtm = values["energy_prices"].rtm[0]
+            else:
+                rtm = values["energy_prices"]
+            _check_lengths({"rtm prices": rtm, "peak reduction data": values["load_peak_reduction"]})
         return values
 
 
 class SolarResourceTimeSeries(BaseModel):
     r"""Irradiance and environmental time series data
 
     - The interval for all time series is assumed to match :attr:`PVGenerationModel.time_interval_mins`.
@@ -2546,14 +2550,19 @@
     r"""Specify the point at which the BESS and generation source are coupled"""
     pv_inputs: GenerationModel
     r"""Submodel for PV or external power generation"""
     enable_grid_charge_year: t.Optional[float]
     r"""Simulation year in which to allow grid charging. Currently, many hybrid systems are not allowed to charge from
     the grid, but are expected to be able to sometime in the future
     """
+    solar_revenue_adder: t.Optional[t.List[float]] = None
+    r"""list of prices to be assigned as additional revenue earned by solar in each time interval. Can be used to
+    model Renewable Energy Credit (REC) revenue or Production Tax Credit (PTC) Revenue. Prices correspond to the time
+    interval given by :attr:`time_interval_mins`. The list length must match the sum of all battery terms when given
+    in the chosen time interval."""
 
     @property
     def project_term(self) -> int:
         r"""Equivalent to ``project_term`` provided in :attr:`pv_inputs`"""
         return self.pv_inputs.project_term
 
     @property
@@ -2605,14 +2614,26 @@
 
     @validator("storage_inputs")
     def set_default_solver(cls, v: MultiStorageInputs):
         if v.solver_config.solver is None:
             v.solver_config.solver = Solver.GLPK_HiGHS
         return v
 
+    @root_validator(skip_on_failure=True)
+    def check_solar_adder_length(cls, values):
+        if values["solar_revenue_adder"]:
+            if isinstance(values["energy_prices"], DARTPrices):
+                rtm = values["energy_prices"].rtm
+            elif isinstance(values["energy_prices"], DARTPriceScenarios):
+                rtm = values["energy_prices"].rtm[0]
+            else:
+                rtm = values["energy_prices"]
+            _check_lengths({"rtm prices": rtm, "solar revenue adder": values["solar_revenue_adder"]})
+        return values
+
 
 class StandaloneStorageModel(ProjectTermMixin, ImportExportLimitMixin, MarketBase):
     r"""Simulation class for standalone storage simulations. The results schema is
     :class:`StandaloneStorageModelWithDownstreamResultsV0` if a downstream system is specified, otherwise the schema
     is :class:`StandaloneStorageModelSimpleResultsV0`"""
 
     project_type: t.Optional[t.Literal["storage"]] = "storage"
@@ -2725,20 +2746,28 @@
 
 
 JobModel = Annotated[
     t.Union[StandaloneStorageModel, PVStorageModel, GenerationModel], Field(discriminator="project_type")
 ]
 
 
+class ResultsFormat(str, Enum):
+    r""":meta private:"""
+    v0 = "v0"
+    v1 = "v1"
+    v2 = "v2"
+
+
 @optional_discriminators(["model"])
 class AsyncModelBase(BaseModel):
     r""":meta private:"""
 
     id: str
     model: JobModel
+    results_format: ResultsFormat = "v0"
     results_path: t.Optional[str]
 
 
 @optional_discriminators(["model"])
 class AsyncPVModel(AsyncModelBase):
     r""":meta private:"""
 
@@ -2759,17 +2788,14 @@
     id: str
     model: StandaloneStorageModel
 
 
 class SolarTimeSeriesV0(BaseModel):
     r"""-"""
 
-    class Config:
-        extra = "forbid"
-
     ideal_tracker_rotation: t.Optional[list]
     r"""-"""
     front_total_poa: t.Optional[list]
     r"""-"""
     rear_total_poa: t.Optional[list]
     r"""-"""
     effective_total_poa: t.Optional[list]
@@ -2835,17 +2861,14 @@
     sam_design_parameters: dict
     r"""-"""
 
 
 class SolarWaterfallVO(BaseModel):
     r"""-"""
 
-    class Config:
-        extra = "forbid"
-
     gh_ann: t.Optional[float]
     r"""-"""
     nominal_poa_ann: t.Optional[float]
     r"""-"""
     shading_lp: t.Optional[float]
     r"""-"""
     soiling_lp: t.Optional[float]
@@ -2907,17 +2930,14 @@
     annual_energy: float
     r"""-"""
 
 
 class SolarStorageTimeSeriesV0(BaseModel):
     r"""-"""
 
-    class Config:
-        extra = "forbid"
-
     battery_internal_energy: list
     r"""-"""
     battery_internal_energy_max: list
     r"""-"""
     battery_limit: t.Union[float, list]
     r"""-"""
     battery_output: list
@@ -2979,29 +2999,29 @@
     negative_solar_storage_poi: list
     r"""-"""
 
 
 class SolarStorageWaterfallV0(SolarWaterfallVO):
     r"""-"""
 
-    class Config:
-        extra = "forbid"
-
     battery_operation_lp: float
     r"""-"""
     excess_power_at_coupling_lp: float
     r"""-"""
     captured_excess_at_coupling_lp: float
     r"""-"""
 
 
 class OptimizerTimeSeriesV0(BaseModel):
     r"""-"""
 
-    # note here we don't forbid extras because of reserve markets and adversarial utilization
+    # note here we allow extras because of reserve markets and adversarial utilization
+    class Config:
+        extra = "allow"
+
     hvac_load: list
     r"""-"""
     nominal_hvac_load: list
     r"""-"""
     storage_discharge_max: list
     r"""-"""
     import_limit_at_coupling: t.Optional[list]
@@ -3089,15 +3109,18 @@
     net_load: t.Optional[list]
     r"""-"""
 
 
 class MarketAwardsTimeSeriesV0(BaseModel):
     r"""-"""
 
-    # note here we don't forbid extras because of reserve markets
+    # note here we allow extras because of reserve markets
+    class Config:
+        extra = "allow"
+
     charge: list
     r"""-"""
     discharge: list
     r"""-"""
     total_output: list
     r"""-"""
     rt_tare: list
@@ -3123,17 +3146,14 @@
     rtm_solar: t.Optional[list]
     r"""-"""
 
 
 class StandaloneStorageSystemTimeSeriesV0(BaseModel):
     r"""-"""
 
-    class Config:
-        extra = "forbid"
-
     dc_power: t.Optional[list]
     r"""-"""
     dc_voltage: t.Optional[list]
     r"""-"""
     inverter_clipping_loss: t.Optional[list]
     r"""-"""
     inverter_tare_loss: t.Optional[list]
@@ -3184,17 +3204,14 @@
     r"""-"""
 
 
 class GenerationModelResultsV0(SolarTimeSeriesV0):
     r"""Results schema returned when a :class:`PVGenerationModel`, :class:`ACExternalGenerationModel` or
     :class:`DCExternalGenerationModel` simulation is run"""
 
-    class Config:
-        extra = "forbid"
-
     tyba_api_loss_waterfall: SolarWaterfallVO
     r"""-"""
     warnings: t.List[str]
     r"""-"""
     coupling: None
     r"""-"""
 
@@ -3213,17 +3230,14 @@
             reformed_model_dict[(outer_key, inner_key)] = values
     return reformed_model_dict
 
 
 class PVStorageModelResultsV0(BaseModel):
     r"""Results schema returned when a :class:`PVStorageModel` simulation is run"""
 
-    class Config:
-        extra = "forbid"
-
     solar_only: SolarTimeSeriesV0
     r"""-"""
     solar_storage: SolarStorageTimeSeriesV0
     r"""-"""
     waterfall: SolarStorageWaterfallV0
     r"""-"""
     optimizer: OptimizerTimeSeriesV0
@@ -3247,17 +3261,14 @@
         return pd.DataFrame(_reform_for_multiindex_df(model_dict))
 
 
 class StandaloneStorageModelWithDownstreamResultsV0(BaseModel):
     r"""Results schema returned when a :class:`StandaloneStorageModel` simulation is run with a
     :attr:`downstream_system` specified"""
 
-    class Config:
-        extra = "forbid"
-
     system: StandaloneStorageSystemTimeSeriesV0
     r"""-"""
     optimizer_outputs: OptimizerTimeSeriesV0
     r"""-"""
     market_awards: t.Optional[MarketAwardsTimeSeriesV0]
     r"""-"""
 
@@ -3266,17 +3277,218 @@
         return pd.DataFrame(_reform_for_multiindex_df(model_dict))
 
 
 class StandaloneStorageModelSimpleResultsV0(OptimizerTimeSeriesV0):
     r"""Results schema returned when a :class:`StandaloneStorageModel` simulation is run without a
     :attr:`downstream_system` specified"""
 
-    # note we don't forbid extras because we inherit from OptimizerTimeSeriesV0
+    # note we allow extras because we inherit from OptimizerTimeSeriesV0
+    class Config:
+        extra = "allow"
+
     pre_hvac_output: list
     r"""-"""
     pre_hvac_battery_output: list
     r"""-"""
     pre_hvac_total_output: list
     r"""-"""
 
     def time_series_df(self):
         return pd.DataFrame(self.dict(exclude_unset=True))
+
+
+class PowerFlowTimeSeriesV2(BaseModel):
+    r""":meta private:"""
+
+    dc_bus_power_kW: t.Optional[t.List[float]]
+    r"""-"""
+    dc_bus_voltage_V: t.Optional[t.List[float]]
+    r"""-"""
+    inverter_clipping_loss_kW: t.Optional[t.List[float]]
+    r"""-"""
+    inverter_efficiency: t.Optional[t.List[float]]
+    r"""-"""
+    inverter_tare_loss_kW: t.Optional[t.List[float]]
+    r"""-"""
+    inverter_consumption_loss_kW: t.Optional[t.List[float]]
+    r"""-"""
+    lv_bus_power_kW: t.Optional[t.List[float]]
+    r"""-"""
+    mv_xfmr_total_loss_kW: t.Optional[t.List[float]]
+    r"""-"""
+    mv_xfmr_load_loss_kW: t.Optional[t.List[float]]
+    r"""-"""
+    mv_xfmr_no_load_loss_kW: t.Optional[t.List[float]]
+    r"""-"""
+    mv_bus_power_kW: t.Optional[t.List[float]]
+    r"""-"""
+    ac_wiring_loss_kW: t.Optional[t.List[float]]
+    r"""-"""
+    hv_xfmr_total_loss_kW: t.Optional[t.List[float]]
+    r"""-"""
+    hv_xfmr_load_loss_kW: t.Optional[t.List[float]]
+    r"""-"""
+    hv_xfmr_no_load_loss_kW: t.Optional[t.List[float]]
+    r"""-"""
+    export_bus_power_kW: t.List[float]
+    r"""-"""
+    transmission_loss_kW: t.List[float]
+    r"""-"""
+    poi_power_pre_clip_kW: t.List[float]
+    r"""-"""
+    poi_power_pre_adjustment_kW: t.List[float]
+    r"""-"""
+    poi_power_kW: t.List[float]
+    r"""-"""
+    poi_power_positive_kW: t.List[float]
+    r"""-"""
+    poi_power_negative_kW: t.List[float]
+    r"""-"""
+    _defaults: t.ClassVar[t.List[str]] = [
+        "dc_bus_power_kW",
+        "dc_bus_voltage_V",
+        "inverter_clipping_loss_kW",
+        "inverter_efficiency",
+        "inverter_tare_loss_kW",
+        "inverter_consumption_loss_kW",
+        "lv_bus_power_kW",
+        "mv_xfmr_total_loss_kW",
+        "mv_bus_power_kW",
+        "ac_wiring_loss_kW",
+        "hv_xfmr_total_loss_kW",
+        "export_bus_power_kW",
+        "transmission_loss_kW",
+        "poi_power_pre_clip_kW",
+        "poi_power_pre_adjustment_kW",
+        "poi_power_kW",
+        "poi_power_positive_kW",
+        "poi_power_negative_kW",
+    ]
+
+    @classmethod
+    def default_include(cls):
+        return {k: True for k in cls._defaults}
+
+
+class GenerationTimeSeriesV2(PowerFlowTimeSeriesV2):
+    r"""-"""
+
+    ghi_Wm2: t.Optional[t.List[float]]
+    r"""-"""
+    tracker_rotation_angle_deg: t.Optional[t.List[float]]
+    r"""-"""
+    front_poa_nominal_Wm2: t.Optional[t.List[float]]
+    r"""-"""
+    front_poa_shaded_Wm2: t.Optional[t.List[float]]
+    r"""-"""
+    front_poa_shaded_soiled_Wm2: t.Optional[t.List[float]]
+    r"""-"""
+    front_poa_Wm2: t.Optional[t.List[float]]
+    r"""-"""
+    rear_poa_Wm2: t.Optional[t.List[float]]
+    r"""-"""
+    poa_effective_Wm2: t.Optional[t.List[float]]
+    r"""-"""
+    poa_effective_power_kW: t.Optional[t.List[float]]
+    r"""-"""
+    cell_temperature_quasi_steady_C: t.Optional[t.List[float]]
+    r"""-"""
+    cell_temperature_C: t.Optional[t.List[float]]
+    r"""-"""
+    module_efficiency: t.Optional[t.List[float]]
+    r"""-"""
+    dc_shading_loss_kW: t.Optional[t.List[float]]
+    r"""-"""
+    dc_snow_loss_kW: t.Optional[t.List[float]]
+    r"""-"""
+    mppt_window_loss_kW: t.Optional[t.List[float]]
+    r"""-"""
+    pv_gross_dc_power_kW: t.Optional[t.List[float]]
+    r"""-"""
+    pv_dc_power_undegraded_kW: t.Optional[t.List[float]]
+    r"""-"""
+    _defaults: t.ClassVar[t.List[str]] = [
+        "ghi_Wm2",
+        "front_poa_Wm2",
+        "rear_poa_Wm2",
+        "poa_effective_Wm2",
+        "pv_gross_dc_power_kW",
+    ] + PowerFlowTimeSeriesV2._defaults
+
+
+class Year1WaterfallV2(BaseModel):
+    r""":meta private:"""
+
+    dc_bus_energy_kWh: t.Optional[float]
+    inverter_clipping: t.Optional[float]
+    inverter_consumption: t.Optional[float]
+    inverter_tare: t.Optional[float]
+    inverter_efficiency: t.Optional[float]
+    lv_bus_energy_kWh: t.Optional[float]
+    mv_transformer: t.Optional[float]
+    mv_bus_energy_kWh: t.Optional[float]
+    ac_wiring: t.Optional[float]
+    hv_transformer: t.Optional[float]
+    export_bus_energy_kWh: float
+    transmission: float
+    poi_clipping: float
+    poi_adjustment: float
+    poi_energy_kWh: float
+
+
+class GenerationYear1WaterfallV2(Year1WaterfallV2):
+    r"""-"""
+
+    ghi_Whm2: t.Optional[float]
+    front_transposition: t.Optional[float]
+    front_shading: t.Optional[float]
+    front_soiling: t.Optional[float]
+    front_iam: t.Optional[float]
+    rear_poa: t.Optional[float]
+    rear_bifaciality: t.Optional[float]
+    poa_effective_annual_Whm2: t.Optional[float]
+    array_area_m2: t.Optional[float]
+    poa_effective_energy_kWh: t.Optional[float]
+    stc_pv_module_effeciency: t.Optional[float]
+    pv_dc_nominal_energy_kWh: t.Optional[float]
+    non_stc_irradiance_temperature: t.Optional[float]
+    r"""this includes DC derate due to beam shading (electrical effect), will be broken out in the future"""
+    mppt_clip: t.Optional[float]
+    snow: t.Optional[float]
+    pv_dc_gross_energy_kWh: t.Optional[float]
+    nameplate: t.Optional[float]
+    lid: t.Optional[float]
+    mismatch: t.Optional[float]
+    diodes: t.Optional[float]
+    dc_optimizer: t.Optional[float]
+    tracking_error: t.Optional[float]
+    dc_wiring: t.Optional[float]
+    dc_adjustment: t.Optional[float]
+
+
+class GenerationModelResultsV2(BaseModel):
+    r"""Results schema returned when a :class:`PVGenerationModel`, :class:`ACExternalGenerationModel` or
+    :class:`DCExternalGenerationModel` simulation is run"""
+
+    time_series: GenerationTimeSeriesV2
+    r"""-"""
+    waterfall: GenerationYear1WaterfallV2
+    r"""-"""
+    sam_raw: t.Optional[dict]
+    r"""-"""
+    solar_resource: t.Optional[SolarResource]
+    r"""-"""
+    warnings: t.Optional[t.List[str]]
+    r"""-"""
+    _defaults: t.ClassVar[t.List[str]] = ["time_series", "waterfall", "warnings"]
+
+    def time_series_df(self):
+        return pd.DataFrame(
+            self.dict(
+                exclude_unset=True,
+            )
+        )
+
+    def default_dict(self):
+        inc = {k: True for k in self._defaults}
+        inc["time_series"] = self.time_series.default_include()
+        return self.dict(exclude_unset=True, include=inc)
```

### Comparing `generation_models-0.4.1/pyproject.toml` & `generation_models-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "generation-models"
-version = "0.4.1"
+version = "0.6.0"
 description = "generation API data model"
 authors = ["battery_al <allenlawrence94@gmail.com>"]
 packages = [{include = "generation_models"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.5.1"
```

### Comparing `generation_models-0.4.1/PKG-INFO` & `generation_models-0.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generation-models
-Version: 0.4.1
+Version: 0.6.0
 Summary: generation API data model
 Author: battery_al
 Author-email: allenlawrence94@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

