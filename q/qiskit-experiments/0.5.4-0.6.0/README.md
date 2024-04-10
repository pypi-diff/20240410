# Comparing `tmp/qiskit-experiments-0.5.4.tar.gz` & `tmp/qiskit-experiments-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-experiments-0.5.4.tar", last modified: Wed Nov  1 16:20:37 2023, max compression
+gzip compressed data, was "qiskit-experiments-0.6.0.tar", last modified: Thu Feb  8 04:51:42 2024, max compression
```

## Comparing `qiskit-experiments-0.5.4.tar` & `qiskit-experiments-0.6.0.tar`

### file list

```diff
@@ -1,209 +1,230 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.981836 qiskit-experiments-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2023-11-01 16:20:37.981836 qiskit-experiments-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.965836 qiskit-experiments-0.5.4/qiskit_experiments/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.969836 qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15765 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/base_calibration_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/basis_gate_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/calibration_key_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/calibration_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    70996 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/calibrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/control_channel_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     7115 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/update_library.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.969836 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17468 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/base_curve_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15107 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/composite_curve_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    19613 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/curve_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    22146 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/curve_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12185 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/curve_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6292 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/fit_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    11532 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/guess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.969836 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/standard_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/standard_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/standard_analysis/bloch_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/standard_analysis/decay.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/standard_analysis/error_amplification_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/standard_analysis/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     9615 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/standard_analysis/oscillation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/standard_analysis/resonance.py
--rw-r--r--   0 runner    (1001) docker     (127)    17350 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.969836 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12035 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/visualization/base_drawer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5949 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/visualization/curves.py
--rw-r--r--   0 runner    (1001) docker     (127)    16466 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/visualization/fit_result_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/visualization/mpl_drawer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/visualization/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.969836 qiskit-experiments-0.5.4/qiskit_experiments/data_processing/
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/data_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/data_processing/data_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    12779 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/data_processing/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/data_processing/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/data_processing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    42185 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/data_processing/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/data_processing/processor_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/data_processing/sklearn_discriminators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.969836 qiskit-experiments-0.5.4/qiskit_experiments/database_service/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/database_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/database_service/device_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/database_service/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/database_service/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.973836 qiskit-experiments-0.5.4/qiskit_experiments/framework/
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17743 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/analysis_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/analysis_result_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/backend_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15017 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/backend_timing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10332 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/base_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    16475 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/base_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.973836 qiskit-experiments-0.5.4/qiskit_experiments/framework/composite/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/composite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7898 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/composite/batch_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)    16334 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/composite/composite_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     8034 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/composite/composite_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8030 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/composite/parallel_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    84134 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/experiment_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    23184 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/restless_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/framework/store_init_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.973836 qiskit-experiments-0.5.4/qiskit_experiments/library/
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.973836 qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/fine_amplitude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8728 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/fine_drag_cal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/fine_frequency_cal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/frequency_cal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/half_angle_cal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11663 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/rough_amplitude_cal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/rough_drag_cal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/rough_frequency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.973836 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.977836 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/correlated_readout_error_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/cr_hamiltonian_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10058 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/drag_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/fine_amplitude_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/local_readout_error_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/multi_state_discrimination_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7944 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/ramsey_xy_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/readout_angle_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/resonator_spectroscopy_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/t1_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/t2hahn_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/t2ramsey_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/tphi_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/zz_ramsey_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/correlated_readout_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    24596 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/cr_hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/drag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/ef_spectroscopy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18587 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/fine_amplitude.py
--rw-r--r--   0 runner    (1001) docker     (127)    12418 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/fine_drag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/fine_frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/half_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/local_readout_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     5401 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/multi_state_discrimination.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/qubit_spectroscopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8286 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/rabi.py
--rw-r--r--   0 runner    (1001) docker     (127)     9236 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/ramsey_xy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/readout_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/resonator_spectroscopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/spectroscopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/t1.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/t2hahn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/t2ramsey.py
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/tphi.py
--rw-r--r--   0 runner    (1001) docker     (127)    15761 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/zz_ramsey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.977836 qiskit-experiments-0.5.4/qiskit_experiments/library/quantum_volume/
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/quantum_volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10721 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/quantum_volume/qv_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/quantum_volume/qv_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.977836 qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20032 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/clifford_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.977836 qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/data/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/data/clifford_compose_1q.npz
--rw-r--r--   0 runner    (1001) docker     (127)   434028 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/data/clifford_compose_2q_sparse.npz
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/data/clifford_inverse_1q.npz
--rw-r--r--   0 runner    (1001) docker     (127)    19116 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/data/clifford_inverse_2q.npz
--rw-r--r--   0 runner    (1001) docker     (127)     7463 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/interleaved_rb_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12946 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/interleaved_rb_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)    14888 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/rb_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/rb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19643 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/standard_rb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.977836 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.977836 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/basis/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/basis/base_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/basis/cache_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    29737 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/basis/local_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     8716 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/basis/pauli_basis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.981836 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20672 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/cvxpy_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (127)    10343 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/cvxpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/fitter_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13316 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/lininv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12083 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/lstsq_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/postprocess_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)    10719 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/scipy_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/mit_qpt_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/mit_qst_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/mit_tomography_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6949 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/qpt_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     8445 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/qpt_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/qst_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/qst_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)    19670 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/tomography_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13606 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/tomography_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.981836 qiskit-experiments-0.5.4/qiskit_experiments/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/test/fake_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    20066 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/test/fake_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    31398 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/test/mock_iq_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    37323 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/test/mock_iq_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/test/noisy_delay_aer_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    23891 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/test/pulse_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7189 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/test/t2hahn_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.981836 qiskit-experiments-0.5.4/qiskit_experiments/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.981836 qiskit-experiments-0.5.4/qiskit_experiments/visualization/drawers/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/visualization/drawers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23669 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/visualization/drawers/base_drawer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/visualization/drawers/legacy_curve_compat_drawer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23317 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/visualization/drawers/mpl_drawer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.981836 qiskit-experiments-0.5.4/qiskit_experiments/visualization/plotters/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/visualization/plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25866 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/visualization/plotters/base_plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/visualization/plotters/curve_plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16098 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/visualization/plotters/iq_plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/visualization/style.py
--rw-r--r--   0 runner    (1001) docker     (127)    10622 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8900 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/qiskit_experiments/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:20:37.965836 qiskit-experiments-0.5.4/qiskit_experiments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2023-11-01 16:20:37.000000 qiskit-experiments-0.5.4/qiskit_experiments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10175 2023-11-01 16:20:37.000000 qiskit-experiments-0.5.4/qiskit_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 16:20:37.000000 qiskit-experiments-0.5.4/qiskit_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 16:20:37.000000 qiskit-experiments-0.5.4/qiskit_experiments.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-11-01 16:20:37.000000 qiskit-experiments-0.5.4/qiskit_experiments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-01 16:20:37.000000 qiskit-experiments-0.5.4/qiskit_experiments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-01 16:20:37.981836 qiskit-experiments-0.5.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2591 2023-11-01 16:20:35.000000 qiskit-experiments-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.149839 qiskit-experiments-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-02-08 04:51:42.149839 qiskit-experiments-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.121839 qiskit-experiments-0.6.0/qiskit_experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.125839 qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15765 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/base_calibration_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18383 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/basis_gate_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/calibration_key_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/calibration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74018 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/calibrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/control_channel_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10181 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/save_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/update_library.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.125839 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15826 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/base_curve_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/composite_curve_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/curve_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22832 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/curve_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/curve_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/fit_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/guess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15986 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/scatter_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.125839 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/standard_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/standard_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/standard_analysis/bloch_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/standard_analysis/decay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/standard_analysis/error_amplification_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/standard_analysis/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/standard_analysis/oscillation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/standard_analysis/resonance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20644 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.125839 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/visualization/base_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/visualization/curves.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17079 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/visualization/fit_result_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/visualization/mpl_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/visualization/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.129839 qiskit-experiments-0.6.0/qiskit_experiments/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/data_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/data_processing/data_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/data_processing/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/data_processing/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/data_processing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42599 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/data_processing/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/data_processing/processor_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/data_processing/sklearn_discriminators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.129839 qiskit-experiments-0.6.0/qiskit_experiments/database_service/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/database_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/database_service/device_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/database_service/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/database_service/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.129839 qiskit-experiments-0.6.0/qiskit_experiments/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17750 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/analysis_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/analysis_result_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/analysis_result_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/backend_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/backend_timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/base_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18584 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/base_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.133839 qiskit-experiments-0.6.0/qiskit_experiments/framework/composite/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/composite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/composite/batch_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/composite/composite_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/composite/composite_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/composite/parallel_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.133839 qiskit-experiments-0.6.0/qiskit_experiments/framework/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/containers/artifact_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/containers/figure_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109489 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/experiment_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22084 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/package_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9549 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/restless_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/framework/store_init_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.133839 qiskit-experiments-0.6.0/qiskit_experiments/library/
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.133839 qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/fine_amplitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/fine_drag_cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/fine_frequency_cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/frequency_cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/half_angle_cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/rough_amplitude_cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/rough_drag_cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/rough_frequency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.137839 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.137839 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/correlated_readout_error_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/cr_hamiltonian_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9924 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/drag_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/fine_amplitude_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/local_readout_error_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/multi_state_discrimination_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/ramsey_xy_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/readout_angle_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/resonator_spectroscopy_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/t1_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/t2hahn_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/t2ramsey_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/tphi_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/zz_ramsey_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/correlated_readout_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22910 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/cr_hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/drag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/ef_spectroscopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18070 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/fine_amplitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/fine_drag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/fine_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/half_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/local_readout_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/multi_state_discrimination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/qubit_spectroscopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/rabi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/ramsey_xy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/readout_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11874 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/resonator_spectroscopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/spectroscopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/t1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/t2hahn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/t2ramsey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/tphi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15529 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/zz_ramsey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.141839 qiskit-experiments-0.6.0/qiskit_experiments/library/driven_freq_tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/driven_freq_tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/driven_freq_tuning/coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/driven_freq_tuning/p1_spect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/driven_freq_tuning/p1_spect_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15864 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/driven_freq_tuning/ramsey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13818 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/driven_freq_tuning/ramsey_amp_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17014 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/driven_freq_tuning/ramsey_amp_scan_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.141839 qiskit-experiments-0.6.0/qiskit_experiments/library/quantum_volume/
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/quantum_volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12468 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/quantum_volume/qv_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/quantum_volume/qv_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.141839 qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/clifford_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25209 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/clifford_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.141839 qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/data/clifford_compose_1q.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   341802 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/data/clifford_compose_2q_dense_selected.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/data/clifford_inverse_1q.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    17677 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/data/clifford_inverse_2q.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/interleaved_rb_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/interleaved_rb_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14890 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/rb_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/rb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20218 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/standard_rb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.145839 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.145839 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/basis/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/basis/base_basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/basis/cache_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29739 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/basis/local_basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8716 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/basis/pauli_basis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.145839 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/fitters/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/fitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20666 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/fitters/cvxpy_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/fitters/cvxpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/fitters/fitter_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/fitters/lininv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/fitters/lstsq_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/fitters/postprocess_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/mit_qpt_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/mit_qst_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/mit_tomography_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/qpt_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/qpt_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/qst_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/qst_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19168 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/tomography_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/tomography_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.149839 qiskit-experiments-0.6.0/qiskit_experiments/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/test/fake_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19488 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/test/fake_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31466 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/test/mock_iq_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34931 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/test/mock_iq_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/test/noisy_delay_aer_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24608 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/test/pulse_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/test/t2hahn_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.149839 qiskit-experiments-0.6.0/qiskit_experiments/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.149839 qiskit-experiments-0.6.0/qiskit_experiments/visualization/drawers/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/visualization/drawers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26080 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/visualization/drawers/base_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/visualization/drawers/legacy_curve_compat_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26039 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/visualization/drawers/mpl_drawer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.149839 qiskit-experiments-0.6.0/qiskit_experiments/visualization/plotters/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/visualization/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27337 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/visualization/plotters/base_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/visualization/plotters/curve_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16098 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/visualization/plotters/iq_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/visualization/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/qiskit_experiments/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.121839 qiskit-experiments-0.6.0/qiskit_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-02-08 04:51:41.000000 qiskit-experiments-0.6.0/qiskit_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-02-08 04:51:42.000000 qiskit-experiments-0.6.0/qiskit_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 04:51:41.000000 qiskit-experiments-0.6.0/qiskit_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-08 04:51:41.000000 qiskit-experiments-0.6.0/qiskit_experiments.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 04:51:41.000000 qiskit-experiments-0.6.0/qiskit_experiments.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-08 04:51:41.000000 qiskit-experiments-0.6.0/qiskit_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-08 04:51:41.000000 qiskit-experiments-0.6.0/qiskit_experiments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/requirements-extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 04:51:42.149839 qiskit-experiments-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:51:42.149839 qiskit-experiments-0.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-02-08 04:51:36.000000 qiskit-experiments-0.6.0/test/test_base.py
```

### Comparing `qiskit-experiments-0.5.4/LICENSE.txt` & `qiskit-experiments-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/PKG-INFO` & `qiskit-experiments-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 Metadata-Version: 2.1
 Name: qiskit-experiments
-Version: 0.5.4
+Version: 0.6.0
 Summary: Software for developing quantum computing programs
-Home-page: https://github.com/Qiskit/qiskit-experiments
+Home-page: https://github.com/Qiskit-Extensions/qiskit-experiments
 Author: Qiskit Development Team
-Author-email: hello@qiskit.org
+Author-email: qiskit@us.ibm.com
 License: Apache 2.0
-Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-experiments/issues
-Project-URL: Documentation, https://qiskit.org/documentation/
-Project-URL: Source Code, https://github.com/Qiskit/qiskit-experiments
+Project-URL: Bug Tracker, https://github.com/Qiskit-Extensions/qiskit-experiments/issues
+Project-URL: Documentation, https://qiskit-extensions.github.io/qiskit-experiments
+Project-URL: Source Code, https://github.com/Qiskit-Extensions/qiskit-experiments
 Description: # Qiskit Experiments
         
-        [![License](https://img.shields.io/github/license/Qiskit/qiskit-experiments.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)
+        [![License](https://img.shields.io/github/license/Qiskit-Extensions/qiskit-experiments.svg)](https://opensource.org/licenses/Apache-2.0)
+        [![Release](https://img.shields.io/github/release/Qiskit-Extensions/qiskit-experiments.svg)](https://github.com/Qiskit-Extensions/qiskit-experiments/releases)
+        ![Python](https://img.shields.io/pypi/pyversions/qiskit-experiments.svg)
+        [![DOI](https://joss.theoj.org/papers/10.21105/joss.05329/status.svg)](https://doi.org/10.21105/joss.05329)
         
         **Qiskit Experiments** is a repository that builds tools for building, running,
         and analyzing experiments on noisy quantum computers using Qiskit.
         
         To learn more about the package, you can see the 
-        [most up-to-date documentation](https://qiskit.org/documentation/experiments/dev/) 
+        [most up-to-date documentation](https://qiskit-extensions.github.io/qiskit-experiments/dev)
         corresponding to the main branch of this repository or the 
-        [documentation for the latest stable release](https://qiskit.org/documentation/experiments).
+        [documentation for the latest stable release](https://qiskit-extensions.github.io/qiskit-experiments).
         
         ## Contribution Guidelines
         
         If you'd like to contribute to Qiskit Experiments, please take a look at our
         [contribution guidelines](CONTRIBUTING.md). This project adheres to Qiskit's
         [code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to
         uphold this code.
         
-        We use [GitHub issues](https://github.com/Qiskit/qiskit-experiments/issues) for
+        We use [GitHub issues](https://github.com/Qiskit-Extensions/qiskit-experiments/issues) for
         tracking requests and bugs. Please
         [join the Qiskit Slack community](https://qisk.it/join-slack)
         and use the [#experiments](https://qiskit.slack.com/archives/CGZDF48EN) channel for discussion and
         simple questions.
         For questions that are more suited for a forum we use the Qiskit tag in 
         [Stack Exchange](https://quantumcomputing.stackexchange.com/questions/tagged/qiskit).
         
         ## Authors and Citation
         
-        Qiskit Experiments is the work of [many people](https://github.com/Qiskit/qiskit-experiments/graphs/contributors) who contribute
-        to the project at different levels. If you use Qiskit Experiments, please cite
-        the following references:
-        
-        - Qiskit, as per the [BibTeX file](https://github.com/Qiskit/qiskit-metapackage/blob/master/Qiskit.bib).
-        - Qiskit Experiments, as per the [DOI](https://doi.org/10.5281/zenodo.7737483).
+        Qiskit Experiments is the work of [many people](https://github.com/Qiskit-Extensions/qiskit-experiments/graphs/contributors) who contribute
+        to the project at different levels. If you use Qiskit Experiments, please cite our
+        [paper](https://doi.org/10.21105/joss.05329) as per the included [citation file](CITATION.cff).
         
         ## License
         
         [Apache License 2.0](LICENSE.txt)
         
         
 Keywords: qiskit sdk quantum
@@ -56,15 +56,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: extras
```

### Comparing `qiskit-experiments-0.5.4/README.md` & `qiskit-experiments-0.6.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # Qiskit Experiments
 
-[![License](https://img.shields.io/github/license/Qiskit/qiskit-experiments.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)
+[![License](https://img.shields.io/github/license/Qiskit-Extensions/qiskit-experiments.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Release](https://img.shields.io/github/release/Qiskit-Extensions/qiskit-experiments.svg)](https://github.com/Qiskit-Extensions/qiskit-experiments/releases)
+![Python](https://img.shields.io/pypi/pyversions/qiskit-experiments.svg)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05329/status.svg)](https://doi.org/10.21105/joss.05329)
 
 **Qiskit Experiments** is a repository that builds tools for building, running,
 and analyzing experiments on noisy quantum computers using Qiskit.
 
 To learn more about the package, you can see the 
-[most up-to-date documentation](https://qiskit.org/documentation/experiments/dev/) 
+[most up-to-date documentation](https://qiskit-extensions.github.io/qiskit-experiments/dev)
 corresponding to the main branch of this repository or the 
-[documentation for the latest stable release](https://qiskit.org/documentation/experiments).
+[documentation for the latest stable release](https://qiskit-extensions.github.io/qiskit-experiments).
 
 ## Contribution Guidelines
 
 If you'd like to contribute to Qiskit Experiments, please take a look at our
 [contribution guidelines](CONTRIBUTING.md). This project adheres to Qiskit's
 [code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to
 uphold this code.
 
-We use [GitHub issues](https://github.com/Qiskit/qiskit-experiments/issues) for
+We use [GitHub issues](https://github.com/Qiskit-Extensions/qiskit-experiments/issues) for
 tracking requests and bugs. Please
 [join the Qiskit Slack community](https://qisk.it/join-slack)
 and use the [#experiments](https://qiskit.slack.com/archives/CGZDF48EN) channel for discussion and
 simple questions.
 For questions that are more suited for a forum we use the Qiskit tag in 
 [Stack Exchange](https://quantumcomputing.stackexchange.com/questions/tagged/qiskit).
 
 ## Authors and Citation
 
-Qiskit Experiments is the work of [many people](https://github.com/Qiskit/qiskit-experiments/graphs/contributors) who contribute
-to the project at different levels. If you use Qiskit Experiments, please cite
-the following references:
-
-- Qiskit, as per the [BibTeX file](https://github.com/Qiskit/qiskit-metapackage/blob/master/Qiskit.bib).
-- Qiskit Experiments, as per the [DOI](https://doi.org/10.5281/zenodo.7737483).
+Qiskit Experiments is the work of [many people](https://github.com/Qiskit-Extensions/qiskit-experiments/graphs/contributors) who contribute
+to the project at different levels. If you use Qiskit Experiments, please cite our
+[paper](https://doi.org/10.21105/joss.05329) as per the included [citation file](CITATION.cff).
 
 ## License
 
 [Apache License 2.0](LICENSE.txt)
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
       - Classes for creating figures from experiment results.
 
 Certain experiments also have additional utilities contained which can be
 accessed by importing the following modules.
 
 - :mod:`qiskit_experiments.library.calibration`
 - :mod:`qiskit_experiments.library.characterization`
+- :mod:`qiskit_experiments.library.driven_freq_tuning`
 - :mod:`qiskit_experiments.library.randomized_benchmarking`
 - :mod:`qiskit_experiments.library.tomography`
 """
 
 from .version import __version__
 
 # Modules
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 .. warning::
     The calibrations interface is still in active development. It may have
     breaking API changes without deprecation warnings in future releases until
     otherwise indicated.
 
 Calibrating qubit setups is the task of finding the pulse shapes and parameter
-values that maximizes the fidelity of the resulting quantum operations. This
+values that maximize the fidelity of the resulting quantum operations. This
 therefore requires experiments which are analyzed to extract parameter values.
 Furthermore, the resulting parameter values and schedules must be managed. The
 calibration management module in Qiskit experiments allows users to manage
 the resulting schedules and parameter values from obtained when running
 calibration experiments from the :mod:`~qiskit_experiments.library`.
 
 Classes
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/base_calibration_experiment.py` & `qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/base_calibration_experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
     @property
     def analysis(self) -> Union[BaseAnalysis, None]:
         """Return the analysis instance for the experiment.
 
         .. note::
             Analysis instance set to calibration experiment is implicitly patched to run
-            calibration updator to update the parameters in the calibration table.
+            calibration updater to update the parameters in the calibration table.
         """
         return self._analysis
 
     @analysis.setter
     def analysis(self, analysis: Union[BaseAnalysis, None]) -> None:
         """Set the analysis instance for the experiment"""
         if analysis is None:
@@ -174,18 +174,18 @@
             experiment_data = analysis_run(*args, **kwargs)
             if self.auto_update:
                 experiment_data.add_analysis_callback(self.update_calibrations)
             return experiment_data
 
         # Monkey patch run method.
         # This calls update_calibrations immediately after standard analysis.
-        # This mechanism allows a composite experiment to invoke updator.
+        # This mechanism allows a composite experiment to invoke updater.
         # Note that the composite experiment only takes circuits from individual experiment
         # and the composite analysis calls analysis.run of each experiment.
-        # This is only place the updator function can be called from the composite experiment.
+        # This is only place the updater function can be called from the composite experiment.
         analysis.run = _wrap_run_analysis
         BaseExperiment.analysis.fset(self, analysis)
 
     @classmethod
     def _default_experiment_options(cls) -> Options:
         """Default values for a calibration experiment.
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/basis_gate_library.py` & `qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/basis_gate_library.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 Note that the set of available libraries will be extended in future releases.
 """
 
 from abc import ABC, abstractmethod
 from collections.abc import Mapping
 from typing import Any, Dict, List, Optional, Set
 from warnings import warn
+import numpy as np
 
 from qiskit.circuit import Parameter
 from qiskit import pulse
 from qiskit.pulse import ScheduleBlock
 
 from qiskit_experiments.calibration_management.calibration_key_types import DefaultCalValue
 from qiskit_experiments.exceptions import CalibrationError
@@ -31,14 +32,17 @@
 
 class BasisGateLibrary(ABC, Mapping):
     """A base class for libraries of basis gates to make it easier to setup Calibrations."""
 
     # Location where default parameter values are stored. These may be updated at construction.
     __default_values__ = {}
 
+    # Parameters that do not belong to a schedule, a set of names
+    __parameters_without_schedule__ = set()
+
     def __init__(
         self,
         basis_gates: Optional[List[str]] = None,
         default_values: Optional[Dict] = None,
         **extra_kwargs,
     ):
         """Setup the library.
@@ -190,26 +194,34 @@
         - y: :math:`\pi` pulse around the y-axis.
         - sy: :math:`\pi/2` pulse around the y-axis.
 
     Pulse parameters:
         - duration: Duration of the pulses Default value: 160 samples.
         - σ: Standard deviation of the pulses Default value: ``duration / 4``.
         - β: DRAG parameter of the pulses Default value: 0.
-        - amp: Amplitude of the pulses. If the parameters are linked then ``x`` and ``y``
+        - amp: Magnitude of the complex amplitude of the pulses. If the parameters are
+          linked then ``x`` and ``y``
           share the same parameter and ``sx`` and ``sy`` share the same parameter.
           Default value: 50% of the maximum output for ``x`` and ``y`` and 25% of the
           maximum output for ``sx`` and ``sy``. Note that the user provided default amplitude
           in the ``__init__`` method sets the default amplitude of the ``x`` and ``y`` pulses.
           The amplitude of the ``sx`` and ``sy`` pulses is half the provided value.
+        - angle: The phase of the complex amplitude of the pulses.
+
+    Parameters without schedule:
+        - meas_freq: frequency of the measurement drives.
+        - drive_freq: frequency of the qubit drives.
 
     Note that the β and amp parameters may be linked between the x and y as well as between
     the sx and sy pulses. All pulses share the same duration and σ parameters.
     """
 
-    __default_values__ = {"duration": 160, "amp": 0.5, "β": 0.0}
+    __default_values__ = {"duration": 160, "amp": 0.5, "β": 0.0, "angle": 0.0}
+
+    __parameters_without_schedule__ = {"meas_freq", "drive_freq"}
 
     def __init__(
         self,
         basis_gates: Optional[List[str]] = None,
         default_values: Optional[Dict] = None,
         link_parameters: bool = True,
     ):
@@ -236,33 +248,33 @@
         return {"x": 1, "y": 1, "sx": 1, "sy": 1}
 
     def _build_schedules(self, basis_gates: Set[str]) -> Dict[str, ScheduleBlock]:
         """Build the schedule of the class."""
         dur = Parameter("duration")
         sigma = Parameter("σ")
 
-        x_amp, x_beta = Parameter("amp"), Parameter("β")
+        x_amp, x_beta, x_angle = Parameter("amp"), Parameter("β"), Parameter("angle")
 
         if self._link_parameters:
-            y_amp, y_beta = 1.0j * x_amp, x_beta
+            y_amp, y_beta, y_angle = x_amp, x_beta, x_angle + np.pi / 2
         else:
-            y_amp, y_beta = Parameter("amp"), Parameter("β")
+            y_amp, y_beta, y_angle = Parameter("amp"), Parameter("β"), Parameter("angle")
 
-        sx_amp, sx_beta = Parameter("amp"), Parameter("β")
+        sx_amp, sx_beta, sx_angle = Parameter("amp"), Parameter("β"), Parameter("angle")
 
         if self._link_parameters:
-            sy_amp, sy_beta = 1.0j * sx_amp, sx_beta
+            sy_amp, sy_beta, sy_angle = sx_amp, sx_beta, sx_angle + np.pi / 2
         else:
-            sy_amp, sy_beta = Parameter("amp"), Parameter("β")
+            sy_amp, sy_beta, sy_angle = Parameter("amp"), Parameter("β"), Parameter("angle")
 
         # Create the schedules for the gates
-        sched_x = self._single_qubit_schedule("x", dur, x_amp, sigma, x_beta)
-        sched_y = self._single_qubit_schedule("y", dur, y_amp, sigma, y_beta)
-        sched_sx = self._single_qubit_schedule("sx", dur, sx_amp, sigma, sx_beta)
-        sched_sy = self._single_qubit_schedule("sy", dur, sy_amp, sigma, sy_beta)
+        sched_x = self._single_qubit_schedule("x", dur, x_amp, sigma, x_beta, x_angle)
+        sched_y = self._single_qubit_schedule("y", dur, y_amp, sigma, y_beta, y_angle)
+        sched_sx = self._single_qubit_schedule("sx", dur, sx_amp, sigma, sx_beta, sx_angle)
+        sched_sy = self._single_qubit_schedule("sy", dur, sy_amp, sigma, sy_beta, sy_angle)
 
         schedules = {}
         for sched in [sched_x, sched_y, sched_sx, sched_sy]:
             if sched.name in basis_gates:
                 schedules[sched.name] = sched
 
         return schedules
@@ -270,21 +282,22 @@
     @staticmethod
     def _single_qubit_schedule(
         name: str,
         dur: Parameter,
         amp: Parameter,
         sigma: Parameter,
         beta: Parameter,
+        angle: Parameter,
     ) -> ScheduleBlock:
         """Build a single qubit pulse."""
 
         chan = pulse.DriveChannel(Parameter("ch0"))
 
         with pulse.build(name=name) as sched:
-            pulse.play(pulse.Drag(duration=dur, amp=amp, sigma=sigma, beta=beta), chan)
+            pulse.play(pulse.Drag(duration=dur, amp=amp, sigma=sigma, beta=beta, angle=angle), chan)
 
         return sched
 
     def default_values(self) -> List[DefaultCalValue]:
         """Return the default values for the parameters.
 
         Returns
@@ -303,16 +316,16 @@
                         value = self._default_values["duration"] / 4
                     else:
                         value = self._default_values[param.name]
 
                     if name in {"sx", "sy"} and param.name == "amp":
                         value /= 2.0
 
-                    if "y" in name and param.name == "amp":
-                        value *= 1.0j
+                    if "y" in name and param.name == "angle":
+                        value += np.pi / 2
 
                     defaults.append(DefaultCalValue(value, param.name, tuple(), name))
 
         return defaults
 
 
 class EchoedCrossResonance(BasisGateLibrary):
@@ -334,15 +347,23 @@
         - tgt_amp: The amplitude of the pulse applied to the target qubit. Default value: 0.
         - σ: The standard deviation of the flanks. Default value: 64 samples.
         - amp: The amplitude of the pulses applied to the control qubit. Default value: 50%.
         - duration: The duration of the cr45p and cr45m pulses. Default value: 1168 samples.
         - risefall: The number of σ's in the flanks of the pulses. Default value: 2.
     """
 
-    __default_values__ = {"tgt_amp": 0.0, "amp": 0.5, "σ": 64, "risefall": 2, "duration": 1168}
+    __default_values__ = {
+        "tgt_amp": 0.0,
+        "tgt_angle": 0.0,
+        "amp": 0.5,
+        "angle": 0.0,
+        "σ": 64,
+        "risefall": 2,
+        "duration": 1168,
+    }
 
     def __init__(
         self,
         basis_gates: Optional[List[str]] = None,
         default_values: Optional[Dict] = None,
         target_pulses: bool = True,
     ):
@@ -375,51 +396,69 @@
 
     def _build_schedules(self, basis_gates: Set[str]) -> Dict[str, ScheduleBlock]:
         """Build the schedules of the CR library."""
 
         schedules = {}
 
         tgt_amp = Parameter("tgt_amp")
+        tgt_angle = Parameter("tgt_angle")
         sigma = Parameter("σ")
         cr_amp = Parameter("amp")
+        cr_angle = Parameter("angle")
         cr_dur = Parameter("duration")
         cr_rf = Parameter("risefall")
         t_chan_idx = Parameter("ch1")
         u_chan_idx = Parameter("ch0.1")
         t_chan = pulse.DriveChannel(t_chan_idx)
         u_chan = pulse.ControlChannel(u_chan_idx)
 
         if "cr45p" in basis_gates:
             with pulse.build(name="cr45p") as cr45p:
                 pulse.play(
-                    pulse.GaussianSquare(cr_dur, cr_amp, risefall_sigma_ratio=cr_rf, sigma=sigma),
+                    pulse.GaussianSquare(
+                        cr_dur, cr_amp, angle=cr_angle, risefall_sigma_ratio=cr_rf, sigma=sigma
+                    ),
                     u_chan,
                 )
 
                 if self._target_pulses:
                     pulse.play(
                         pulse.GaussianSquare(
-                            cr_dur, tgt_amp, risefall_sigma_ratio=cr_rf, sigma=sigma
+                            cr_dur,
+                            tgt_amp,
+                            angle=tgt_angle,
+                            risefall_sigma_ratio=cr_rf,
+                            sigma=sigma,
                         ),
                         t_chan,
                     )
 
             schedules["cr45p"] = cr45p
 
         if "cr45m" in basis_gates:
             with pulse.build(name="cr45m") as cr45m:
                 pulse.play(
-                    pulse.GaussianSquare(cr_dur, -cr_amp, risefall_sigma_ratio=cr_rf, sigma=sigma),
+                    pulse.GaussianSquare(
+                        cr_dur,
+                        cr_amp,
+                        angle=cr_angle + np.pi,
+                        risefall_sigma_ratio=cr_rf,
+                        sigma=sigma,
+                    ),
                     u_chan,
                 )
 
                 if self._target_pulses:
                     pulse.play(
                         pulse.GaussianSquare(
-                            cr_dur, -tgt_amp, risefall_sigma_ratio=cr_rf, sigma=sigma
+                            cr_dur,
+                            tgt_amp,
+                            angle=tgt_angle + np.pi,
+                            risefall_sigma_ratio=cr_rf,
+                            sigma=sigma,
                         ),
                         t_chan,
                     )
 
             schedules["cr45m"] = cr45m
 
         # Echoed Cross-Resonance gate
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/calibration_key_types.py` & `qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/calibration_key_types.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/calibration_utils.py` & `qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/calibration_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/calibrations.py` & `qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/calibrations.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Class to store and manage the results of calibration experiments."""
 
+import warnings
 import os
-from collections import defaultdict
+from collections import defaultdict, Counter
 from datetime import datetime, timezone
 from typing import Any, Dict, Set, Tuple, Union, List, Optional
 import csv
 import dataclasses
 import json
-import warnings
 import rustworkx as rx
 
 from qiskit.pulse import (
     ScheduleBlock,
     DriveChannel,
     ControlChannel,
     MeasureChannel,
@@ -31,14 +31,15 @@
     RegisterSlot,
     MemorySlot,
     InstructionScheduleMap,
 )
 from qiskit.pulse.channels import PulseChannel
 from qiskit.circuit import Parameter, ParameterExpression
 from qiskit.providers.backend import Backend
+from qiskit.utils.deprecation import deprecate_func, deprecate_arg
 
 from qiskit_experiments.exceptions import CalibrationError
 from qiskit_experiments.calibration_management.basis_gate_library import BasisGateLibrary
 from qiskit_experiments.calibration_management.parameter_value import ParameterValue
 from qiskit_experiments.calibration_management.control_channel_map import ControlChannelMap
 from qiskit_experiments.calibration_management.calibration_utils import (
     used_in_references,
@@ -47,31 +48,25 @@
     update_schedule_dependency,
 )
 from qiskit_experiments.calibration_management.calibration_key_types import (
     ParameterKey,
     ParameterValueType,
     ScheduleKey,
 )
-from qiskit_experiments.framework import BackendData
+from qiskit_experiments.framework import BackendData, ExperimentEncoder, ExperimentDecoder
 
 
 class Calibrations:
     """
     A class to manage schedules with calibrated parameter values. Schedules are
     intended to be fully parameterized, including the index of the channels. See
     the module-level documentation for extra details. Note that only instances of
     ScheduleBlock are supported.
     """
 
-    # The name of the parameter under which the qubit frequencies are registered.
-    __drive_freq_parameter__ = "drive_freq"
-
-    # The name of the parameter under which the readout frequencies are registered.
-    __readout_freq_parameter__ = "meas_freq"
-
     def __init__(
         self,
         coupling_map: Optional[List[List[int]]] = None,
         control_channel_map: Optional[Dict[Tuple[int, ...], List[ControlChannel]]] = None,
         libraries: Optional[List[BasisGateLibrary]] = None,
         add_parameter_defaults: bool = True,
         backend_name: Optional[str] = None,
@@ -148,48 +143,67 @@
 
         self._libraries = libraries
         if libraries is not None:
             if not isinstance(libraries, list):
                 libraries = [libraries]
 
             for lib in libraries:
-
                 # Add the basis gates
                 for gate in lib.basis_gates:
                     self.add_schedule(lib[gate], num_qubits=lib.num_qubits(gate))
 
                 # Add the default values
                 if add_parameter_defaults:
                     for param_conf in lib.default_values():
                         self.add_parameter_value(*param_conf, update_inst_map=False)
 
+                # Add the parameters that do not belong to a schedule.
+                for param_name in lib.__parameters_without_schedule__:
+                    self._register_parameter(Parameter(param_name), tuple())
+
         # This internal parameter is False so that if a schedule is added after the
         # init it will be set to True and serialization will raise an error.
         self._has_manually_added_schedule = False
 
         # Instruction schedule map variables and support variables.
         self._inst_map = InstructionScheduleMap()
 
-        # Use the same naming convention as in backend.defaults()
-        self.drive_freq = Parameter(self.__drive_freq_parameter__)
-        self.meas_freq = Parameter(self.__readout_freq_parameter__)
-        self._register_parameter(self.drive_freq, ())
-        self._register_parameter(self.meas_freq, ())
-
         # Backends with a single qubit may not have a coupling map.
         self._coupling_map = coupling_map if coupling_map is not None else []
 
         # A dict extension of the coupling map where the key is the number of qubits and
         # the values are a list of qubits coupled.
         self._operated_qubits = self._get_operated_qubits()
         self._check_consistency()
 
         # Push the schedules to the instruction schedule map.
         self.update_inst_map()
 
+    @property
+    @deprecate_func(
+        is_property=True,
+        since="0.6",
+        package_name="qiskit-experiments",
+        additional_msg="The drive_freq is moved to FixedFrequencyTransmon basis gate library.",
+    )
+    def drive_freq(self):
+        """Parameter object for qubit drive frequency."""
+        return self._parameter_map.get(("drive_freq", (), None), None)
+
+    @property
+    @deprecate_func(
+        is_property=True,
+        since="0.6",
+        package_name="qiskit-experiments",
+        additional_msg="The meas_freq is moved to FixedFrequencyTransmon basis gate library.",
+    )
+    def meas_freq(self):
+        """Parameter object for qubit measure frequency."""
+        return self._parameter_map.get(("meas_freq", (), None), None)
+
     def _check_consistency(self):
         """Check that the attributes defined in self are consistent.
 
         Raises:
             CalibrationError: If there is a control channel map but no coupling map.
             CalibrationError: If a qubit in the control channel map is not in the
                 coupling map.
@@ -232,15 +246,15 @@
         Args:
             backend: A backend instance from which to extract the qubit and readout frequencies
                 (which will be added as first guesses for the corresponding parameters) as well
                 as the coupling map.
             libraries: A list of libraries from which to get template schedules to register as
                 well as default parameter values.
             add_parameter_defaults: A boolean to indicate whether the default parameter values of
-                the given library should be used to populate the calibrations. By default this
+                the given library should be used to populate the calibrations. By default, this
                 value is ``True``.
 
         Returns:
             An instance of Calibrations instantiated from a backend.
         """
         backend_data = BackendData(backend)
 
@@ -255,19 +269,21 @@
             libraries,
             add_parameter_defaults,
             backend_data.name,
             backend_data.version,
         )
 
         if add_parameter_defaults:
-            for qubit, freq in enumerate(backend_data.drive_freqs):
-                cals.add_parameter_value(freq, cals.drive_freq, qubit, update_inst_map=False)
-
-            for meas, freq in enumerate(backend_data.meas_freqs):
-                cals.add_parameter_value(freq, cals.meas_freq, meas, update_inst_map=False)
+            if ("drive_freq", (), None) in cals._parameter_map:
+                for qubit, freq in enumerate(backend_data.drive_freqs):
+                    cals.add_parameter_value(freq, "drive_freq", qubit, update_inst_map=False)
+
+            if ("meas_freq", (), None) in cals._parameter_map:
+                for meas, freq in enumerate(backend_data.meas_freqs):
+                    cals.add_parameter_value(freq, "meas_freq", meas, update_inst_map=False)
 
         # Update the instruction schedule map after adding all parameter values.
         cals.update_inst_map()
 
         return cals
 
     @property
@@ -444,15 +460,14 @@
 
         Returns:
             A list of tuples. Each tuple is the set of qubits for which there is a schedule
             named ``schedule_name`` and ``partial_qubits`` is a sub-set of said qubits.
         """
         for key, circuit_inst_num_qubits in self._schedules_qubits.items():
             if key.schedule == schedule_name:
-
                 if len(partial_qubits) == circuit_inst_num_qubits:
                     return [partial_qubits]
 
                 else:
                     candidates = self._operated_qubits[circuit_inst_num_qubits]
                     qubits_for_update = []
                     for candidate_qubits in candidates:
@@ -883,15 +898,14 @@
                 if len(qubits) <= index:
                     raise CalibrationError(f"Not enough qubits given for channel {chan}.")
 
                 return qubits[index]
 
             # Control channels name example ch1.0$1
             if isinstance(chan, ControlChannel):
-
                 channel_index_parts = chan.index.name[2:].split("$")
                 qubit_channels = channel_index_parts[0]
 
                 indices = [int(sub_channel) for sub_channel in qubit_channels.split(".")]
                 ch_qubits = tuple(qubits[index] for index in indices)
                 chs_ = self._control_channel_map.get(ch_qubits, [])
 
@@ -1252,20 +1266,20 @@
 
     def schedules(self) -> List[Dict[str, Any]]:
         """Return the managed schedules in a list of dictionaries.
 
         Returns:
             data: A list of dictionaries with all the schedules in it. The key-value pairs are
 
-                * 'qubits': the qubits to which this schedule applies. This may be an empty
-                  tuple () if the schedule is the default for all qubits.
-                * 'schedule': The schedule.
-                * 'parameters': The parameters in the schedule exposed for convenience.
+            * ``qubits``: the qubits to which this schedule applies. This may be an empty
+                tuple () if the schedule is the default for all qubits.
+            * ``schedule``: The schedule.
+            * ``parameters``: The parameters in the schedule exposed for convenience.
 
-                This list of dictionaries can easily be converted to a data frame.
+            This list of dictionaries can easily be converted to a data frame.
         """
         data = []
         for key, sched in self._schedules.items():
             data.append({"qubits": key.qubits, "schedule": sched, "parameters": sched.parameters})
 
         return data
 
@@ -1348,87 +1362,101 @@
         value_dict = dataclasses.asdict(value)
         value_dict["qubits"] = key.qubits
         value_dict["parameter"] = key.parameter
         value_dict["schedule"] = key.schedule
         value_dict["date_time"] = value_dict["date_time"].strftime("%Y-%m-%d %H:%M:%S.%f%z")
         data.append(value_dict)
 
+    @deprecate_arg(
+        name="file_type",
+        since="0.6",
+        additional_msg="Full calibration saving is now supported in json format. csv is deprecated.",
+        package_name="qiskit-experiments",
+        predicate=lambda file_type: file_type == "csv",
+    )
     def save(
         self,
-        file_type: str = "csv",
+        file_type: str = "json",
         folder: str = None,
         overwrite: bool = False,
         file_prefix: str = "",
         most_recent_only: bool = False,
     ):
         """Save the parameterized schedules and parameter value.
 
-        The schedules and parameter values can be stored in csv files. This method creates
-        three files:
+        .. note::
 
-        * parameter_config.csv: This file stores a table of parameters which indicates
-          which parameters appear in which schedules.
-        * parameter_values.csv: This file stores the values of the calibrated parameters.
-        * schedules.csv: This file stores the parameterized schedules.
-
-        Warning:
-            Schedule blocks will only be saved in string format and can therefore not be
-            reloaded and must instead be rebuilt.
+            Full round-trip serialization of a :class:`.Calibrations` instance
+            is only supported in JSON format.
+            This may be extended to other file formats in future version.
 
         Args:
-            file_type: The type of file to which to save. By default this is a csv.
+            file_type: The type of file to which to save. By default, this is a json.
                 Other file types may be supported in the future.
             folder: The folder in which to save the calibrations.
             overwrite: If the files already exist then they will not be overwritten
                 unless overwrite is set to True.
             file_prefix: A prefix to add to the name of the files such as a date tag or a
                 UUID.
             most_recent_only: Save only the most recent value. This is set to False by
                 default so that when saving to csv all values will be saved.
 
         Raises:
             CalibrationError: If the files exist and overwrite is not set to True.
         """
-        warnings.warn("Schedules are only saved in text format. They cannot be re-loaded.")
-
         cwd = os.getcwd()
         if folder:
             os.chdir(folder)
 
-        parameter_config_file = file_prefix + "parameter_config.csv"
-        parameter_value_file = file_prefix + "parameter_values.csv"
-        schedule_file = file_prefix + "schedules.csv"
+        if file_type == "json":
+            from .save_utils import calibrations_to_dict
 
-        if os.path.isfile(parameter_config_file) and not overwrite:
-            raise CalibrationError(
-                f"{parameter_config_file} already exists. Set overwrite to True."
-            )
+            file_path = file_prefix + ".json"
+            if os.path.isfile(file_path) and not overwrite:
+                raise CalibrationError(f"{file_path} already exists. Set overwrite to True.")
 
-        if os.path.isfile(parameter_value_file) and not overwrite:
-            raise CalibrationError(f"{parameter_value_file} already exists. Set overwrite to True.")
+            canonical_data = calibrations_to_dict(self, most_recent_only=most_recent_only)
+            with open(file_path, "w", encoding="utf-8") as file:
+                json.dump(canonical_data, file, cls=ExperimentEncoder)
 
-        if os.path.isfile(schedule_file) and not overwrite:
-            raise CalibrationError(f"{schedule_file} already exists. Set overwrite to True.")
+        elif file_type == "csv":
+            warnings.warn("Schedules are only saved in text format. They cannot be re-loaded.")
 
-        # Write the parameter configuration.
-        header_keys = ["parameter.name", "parameter unique id", "schedule", "qubits"]
-        body = []
+            parameter_config_file = file_prefix + "parameter_config.csv"
+            parameter_value_file = file_prefix + "parameter_values.csv"
+            schedule_file = file_prefix + "schedules.csv"
 
-        for parameter, keys in self.parameters.items():
-            for key in keys:
-                body.append(
-                    {
-                        "parameter.name": parameter.name,
-                        "parameter unique id": self._hash_to_counter_map[parameter],
-                        "schedule": key.schedule,
-                        "qubits": key.qubits,
-                    }
+            if os.path.isfile(parameter_config_file) and not overwrite:
+                raise CalibrationError(
+                    f"{parameter_config_file} already exists. Set overwrite to True."
                 )
 
-        if file_type == "csv":
+            if os.path.isfile(parameter_value_file) and not overwrite:
+                raise CalibrationError(
+                    f"{parameter_value_file} already exists. Set overwrite to True."
+                )
+
+            if os.path.isfile(schedule_file) and not overwrite:
+                raise CalibrationError(f"{schedule_file} already exists. Set overwrite to True.")
+
+            # Write the parameter configuration.
+            header_keys = ["parameter.name", "parameter unique id", "schedule", "qubits"]
+            body = []
+
+            for parameter, keys in self.parameters.items():
+                for key in keys:
+                    body.append(
+                        {
+                            "parameter.name": parameter.name,
+                            "parameter unique id": self._hash_to_counter_map[parameter],
+                            "schedule": key.schedule,
+                            "qubits": key.qubits,
+                        }
+                    )
+
             with open(parameter_config_file, "w", newline="", encoding="utf-8") as output_file:
                 dict_writer = csv.DictWriter(output_file, header_keys)
                 dict_writer.writeheader()
                 dict_writer.writerows(body)
 
             # Write the values of the parameters.
             values = self.parameters_table(most_recent_only=most_recent_only)["data"]
@@ -1449,14 +1477,22 @@
                 dict_writer.writerows(schedules)
 
         else:
             raise CalibrationError(f"Saving to .{file_type} is not yet supported.")
 
         os.chdir(cwd)
 
+    @deprecate_func(
+        since="0.6",
+        additional_msg=(
+            "Saving calibration in csv format is deprecate "
+            "as well as functions that support this functionality."
+        ),
+        package_name="qiskit-experiments",
+    )
     def schedule_information(self) -> Tuple[List[str], List[Dict]]:
         """Get the information on the schedules stored in the calibrations.
 
         This function serializes the schedule by simply printing them.
 
         Returns:
             A tuple, the first element is the header row while the second is a dictionary
@@ -1467,14 +1503,19 @@
         # Serialize the schedules. For now we just print them.
         schedules = []
         for key, sched in self._schedules.items():
             schedules.append({"name": key.schedule, "qubits": key.qubits, "schedule": str(sched)})
 
         return ["name", "qubits", "schedule"], schedules
 
+    @deprecate_func(
+        since="0.6",
+        additional_msg="Loading and saving calibrations in CSV format is deprecated.",
+        package_name="qiskit-experiments",
+    )
     def load_parameter_values(self, file_name: str = "parameter_values.csv"):
         """
         Load parameter values from a given file into self._params.
 
         Args:
             file_name: The name of the file that stores the parameters. Will default to
                 parameter_values.csv.
@@ -1510,31 +1551,53 @@
             exp_id: The id of the experiment that created the parameter value.
             group: The calibration group to which the parameter belongs.
             schedule: The schedule to which the parameter belongs. The empty string
                 "" is converted to None.
             parameter: The name of the parameter.
             qubits: The qubits on which the parameter acts.
         """
+        # TODO remove this after load_parameter_values method is removed.
+
         param_val = ParameterValue(value, date_time, valid, exp_id, group)
 
         if schedule == "":
             schedule_name = None
         else:
             schedule_name = schedule
 
         key = ParameterKey(parameter, self._to_tuple(qubits), schedule_name)
         self.add_parameter_value(param_val, *key, update_inst_map=False)
 
     @classmethod
-    def load(cls, files: List[str]) -> "Calibrations":
+    @deprecate_arg(
+        name="files",
+        new_alias="file_path",
+        since="0.6",
+        package_name="qiskit-experiments",
+    )
+    def load(cls, file_path: str) -> "Calibrations":
         """
         Retrieves the parameterized schedules and pulse parameters from the
         given location.
+
+        Args:
+            file_path: Path to file location.
+
+        Returns:
+            Calibration instance restored from the file.
         """
-        raise CalibrationError("Full calibration loading is not implemented yet.")
+        from .save_utils import calibrations_from_dict
+
+        with open(file_path, "r", encoding="utf-8") as file:
+            # Do we really need branching for data types?
+            # Parsing data format and dispatching the loader seems an overkill,
+            # but save method intend to support multiple formats.
+            cal_data = json.load(file, cls=ExperimentDecoder)
+
+        return calibrations_from_dict(cal_data)
 
     @staticmethod
     def _to_tuple(qubits: Union[str, int, Tuple[int, ...]]) -> Tuple[int, ...]:
         """Ensure that qubits is a tuple of ints.
 
         Args:
             qubits: An int, a tuple of ints, or a string representing a tuple of ints.
@@ -1591,22 +1654,30 @@
             if repr(schedule) != repr(other._schedules.get(key, None)):
                 return False
 
         # Check the keys.
         if self._schedules.keys() != other._schedules.keys():
             return False
 
-        def _hash(data: dict):
-            return hash(json.dumps(data))
-
-        sorted_params_a = sorted(self.parameters_table()["data"], key=_hash)
-        sorted_params_b = sorted(other.parameters_table()["data"], key=_hash)
-
-        return sorted_params_a == sorted_params_b
+        def _counting(table):
+            return Counter(map(lambda d: tuple(d.items()), table["data"]))
 
+        # Use counting sort algorithm to compare unordered sequences
+        # https://en.wikipedia.org/wiki/Counting_sort
+        return _counting(self.parameters_table()) == _counting(other.parameters_table())
+
+    @deprecate_func(
+        since="0.6",
+        additional_msg=(
+            "Configuration data for Calibrations instance is deprecate. "
+            "Please use ExperimentEncoder and ExperimentDecoder to "
+            "serialize and deserialize this instance with JSON format."
+        ),
+        package_name="qiskit-experiments",
+    )
     def config(self) -> Dict[str, Any]:
         """Return the settings used to initialize the calibrations.
 
         Returns:
             The config dictionary of the calibrations instance.
 
         Raises:
@@ -1631,27 +1702,37 @@
         return {
             "class": self.__class__.__name__,
             "kwargs": kwargs,
             "parameters": self.parameters_table()["data"],
         }
 
     @classmethod
+    @deprecate_func(
+        since="0.6",
+        additional_msg="This method will be removed and no alternative will be provided.",
+        package_name="qiskit-experiments",
+    )
     def from_config(cls, config: Dict) -> "Calibrations":
-        """Deserialize the calibrations given the input dictionary"""
-
-        config["kwargs"]["control_channel_map"] = config["kwargs"]["control_channel_map"].chan_map
+        """Restore Calibration from config data.
 
-        calibrations = cls(**config["kwargs"])
+        Args:
+            config: Configuration data.
 
-        for param_config in config["parameters"]:
-            calibrations._add_parameter_value_from_conf(**param_config)
+        Returns:
+            Calibration instance restored from configuration data.
+        """
+        from .save_utils import calibrations_from_dict
 
-        return calibrations
+        return calibrations_from_dict(config)
 
     def __json_encode__(self):
         """Convert to format that can be JSON serialized."""
-        return self.config()
+        from .save_utils import calibrations_to_dict
+
+        return calibrations_to_dict(self, most_recent_only=False)
 
     @classmethod
     def __json_decode__(cls, value: Dict[str, Any]) -> "Calibrations":
         """Load from JSON compatible format."""
-        return cls.from_config(value)
+        from .save_utils import calibrations_from_dict
+
+        return calibrations_from_dict(value)
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/control_channel_map.py` & `qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/control_channel_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/parameter_value.py` & `qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/parameter_value.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # that they have been altered from the originals.
 
 """Data class for parameter values."""
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Union
+import warnings
 
 from qiskit_experiments.exceptions import CalibrationError
 
 
 @dataclass
 class ParameterValue:
     """A data class to store parameter values."""
@@ -67,14 +68,25 @@
                 formats = list(base_fmt + zone for zone in zone_fmts)
                 raise CalibrationError(
                     f"Cannot parse {self.date_time} in either of {formats} formats."
                 )
 
         self.date_time = self.date_time.astimezone()
 
+        if isinstance(self.value, complex):
+            warnings.warn(
+                "Support of complex parameters is now pending deprecation, following the"
+                "same transition in Qiskit's Pulse module."
+                "The main use of complex parameters was the complex amplitude in SymbolicPulse"
+                "instances. This use could be removed by converting the pulses to the"
+                "ScalableSymbolicPulse class which uses two floats (amp,angle) for the"
+                "complex amplitude.",
+                PendingDeprecationWarning,
+            )
+
         if not isinstance(self.value, (int, float, complex)):
             raise CalibrationError(f"Values {self.value} must be int, float or complex.")
 
         if not isinstance(self.date_time, datetime):
             raise CalibrationError(f"Datetime {self.date_time} must be a datetime.")
 
         if not isinstance(self.valid, bool):
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/calibration_management/update_library.py` & `qiskit-experiments-0.6.0/qiskit_experiments/calibration_management/update_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,38 +145,35 @@
     # pylint: disable=arguments-differ,unused-argument
     @classmethod
     def update(
         cls,
         calibrations: Calibrations,
         exp_data: ExperimentData,
         result_index: Optional[int] = None,
-        parameter: str = None,
+        parameter: str = "drive_freq",
         group: str = "default",
         fit_parameter: Optional[str] = None,
         **options,
     ):
         """Update a qubit frequency from, e.g., QubitSpectroscopy
 
         The value of the amplitude must be derived from the fit so the base method cannot be used.
 
         Args:
             calibrations: The calibrations to update.
             exp_data: The experiment data from which to update.
             result_index: The result index to use which defaults to -1.
             parameter: The name of the parameter to update. If None is given this will default
-                to :code:`calibrations.__qubit_freq_parameter__`.
+                to `drive_freq`.
             group: The calibrations group to update. Defaults to "default."
             options: Trailing options.
             fit_parameter: The name of the fit parameter in the analysis result. This will default
                 to the class variable :code:`__fit_parameter__` if not given.
 
         """
-        if parameter is None:
-            parameter = calibrations.__drive_freq_parameter__
-
         super().update(
             calibrations=calibrations,
             exp_data=exp_data,
             parameter=parameter,
             schedule=None,
             result_index=result_index,
             group=group,
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 Data Classes
 ============
 
 .. autosummary::
     :toctree: ../stubs/
 
+    ScatterTable
     SeriesDef
     CurveData
     CurveFitResult
     ParameterRepr
     FitOptions
 
 Visualization
@@ -77,17 +78,14 @@
     fit_function.cos
     fit_function.cos_decay
     fit_function.exponential_decay
     fit_function.gaussian
     fit_function.sqrt_lorentzian
     fit_function.sin
     fit_function.sin_decay
-    fit_function.bloch_oscillation_x
-    fit_function.bloch_oscillation_y
-    fit_function.bloch_oscillation_z
 
 Initial Guess Estimators
 ========================
 .. autosummary::
     :toctree: ../stubs/
 
     guess.constant_sinusoidal_offset
@@ -116,25 +114,24 @@
     utils.level2_probability
     utils.probability
 
 """
 from .base_curve_analysis import BaseCurveAnalysis
 from .curve_analysis import CurveAnalysis
 from .composite_curve_analysis import CompositeCurveAnalysis
+from .scatter_table import ScatterTable
 from .curve_data import (
     CurveData,
     CurveFitResult,
     FitData,
     FitOptions,
     ParameterRepr,
     SeriesDef,
 )
 from .curve_fit import (
-    curve_fit,
-    multi_curve_fit,
     process_curve_data,
     process_multi_curve_data,
 )
 from .visualization import BaseCurveDrawer, MplCurveDrawer
 from . import guess
 from . import fit_function
 from . import utils
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/base_curve_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/base_curve_analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 import warnings
 from abc import ABC, abstractmethod
 from typing import Dict, List, Union
 
 import lmfit
 
+from qiskit.utils.deprecation import deprecate_func
+
 from qiskit_experiments.data_processing import DataProcessor
 from qiskit_experiments.data_processing.processor_library import get_processor
 from qiskit_experiments.framework import (
     AnalysisResultData,
     BaseAnalysis,
     ExperimentData,
     Options,
@@ -31,17 +33,17 @@
 from qiskit_experiments.visualization import (
     BaseDrawer,
     BasePlotter,
     CurvePlotter,
     LegacyCurveCompatDrawer,
     MplDrawer,
 )
-from qiskit_experiments.warnings import deprecated_function
 
-from .curve_data import CurveData, CurveFitResult, ParameterRepr
+from .curve_data import CurveFitResult, ParameterRepr
+from .scatter_table import ScatterTable
 
 PARAMS_ENTRY_PREFIX = "@Parameters_"
 DATA_ENTRY_PREFIX = "@Data_"
 
 
 class BaseCurveAnalysis(BaseAnalysis, ABC):
     """Abstract superclass of curve analysis base classes.
@@ -92,20 +94,18 @@
     that creates fit result object from the formatted dataset.
 
     .. rubric:: _create_analysis_results
 
     This method creates analysis results for important fit parameters
     that might be defined by analysis options ``result_parameters``.
 
-    .. rubric:: _create_curve_data
+    .. rubric:: _create_figures
 
-    This method to creates analysis results for the formatted dataset, i.e. data used for the fitting.
-    Entries are created when the analysis option ``return_data_points`` is ``True``.
-    If analysis consists of multiple series, analysis result is created for
-    each curve data in the series definitions.
+    This method creates figures by consuming the scatter table data.
+    Figures are created when the analysis option ``plot`` is ``True``.
 
     .. rubric:: _initialize
 
     This method initializes analysis options against input experiment data.
     Usually this method is called before other methods are called.
 
     """
@@ -127,17 +127,19 @@
 
     @property
     def plotter(self) -> BasePlotter:
         """A short-cut to the curve plotter instance."""
         return self._options.plotter
 
     @property
-    @deprecated_function(
-        last_version="0.6",
-        msg="Replaced by `plotter` from the new visualization submodule.",
+    @deprecate_func(
+        since="0.5",
+        additional_msg="Use `plotter` from the new visualization module.",
+        removal_timeline="after 0.6",
+        package_name="qiskit-experiments",
     )
     def drawer(self) -> BaseDrawer:
         """A short-cut for curve drawer instance, if set. ``None`` otherwise."""
         if isinstance(self.plotter.drawer, LegacyCurveCompatDrawer):
             return self.plotter.drawer._curve_drawer
         else:
             return None
@@ -147,41 +149,43 @@
         """Return default analysis options.
 
         Analysis Options:
             plotter (BasePlotter): A curve plotter instance to visualize
                 the analysis result.
             plot_raw_data (bool): Set ``True`` to draw processed data points,
                 dataset without formatting, on canvas. This is ``False`` by default.
-            plot (bool): Set ``True`` to create figure for fit result.
-                This is ``True`` by default.
-            return_fit_parameters (bool): Set ``True`` to return all fit model parameters
-                with details of the fit outcome. Default to ``True``.
-            return_data_points (bool): Set ``True`` to include in the analysis result
+            plot (bool): Set ``True`` to create figure for fit result or ``False`` to
+                not create a figure. This overrides the behavior of ``generate_figures``.
+            return_fit_parameters (bool): (Deprecated) Set ``True`` to return all fit model parameters
+                with details of the fit outcome. Default to ``False``.
+            return_data_points (bool): (Deprecated) Set ``True`` to include in the analysis result
                 the formatted data points given to the fitter. Default to ``False``.
             data_processor (Callable): A callback function to format experiment data.
                 This can be a :class:`.DataProcessor`
                 instance that defines the `self.__call__` method.
             normalization (bool): Set ``True`` to normalize y values within range [-1, 1].
                 Default to ``False``.
-            average_method (str): Method to average the y values when the same x values
-                appear multiple times. One of "sample", "iwv" (i.e. inverse weighted variance),
-                "shots_weighted". See :func:`.mean_xy_data` for details. Default to
-                "shots_weighted".
+            average_method (Literal["sample", "iwv", "shots_weighted"]): Method
+                to average the y values when the same x values
+                appear multiple times. One of "sample", "iwv" (i.e. inverse
+                weighted variance), "shots_weighted". See :func:`.mean_xy_data`
+                for details. Default to "shots_weighted".
             p0 (Dict[str, float]): Initial guesses for the fit parameters.
                 The dictionary is keyed on the fit parameter names.
             bounds (Dict[str, Tuple[float, float]]): Boundary of fit parameters.
                 The dictionary is keyed on the fit parameter names and
                 values are the tuples of (min, max) of each parameter.
             fit_method (str): Fit method that LMFIT minimizer uses.
                 Default to ``least_squares`` method which implements the
                 Trust Region Reflective algorithm to solve the minimization problem.
                 See LMFIT documentation for available options.
             lmfit_options (Dict[str, Any]): Options that are passed to the
                 LMFIT minimizer. Acceptable options depend on fit_method.
             x_key (str): Circuit metadata key representing a scanned value.
+            fit_category (str): Name of dataset in the scatter table to fit.
             result_parameters (List[Union[str, ParameterRepr]): Parameters reported in the
                 database as a dedicated entry. This is a list of parameter representation
                 which is either string or ParameterRepr object. If you provide more
                 information other than name, you can specify
                 ``[ParameterRepr("alpha", "\u03B1", "a.u.")]`` for example.
                 The parameter name should be defined in the series definition.
                 Representation should be printable in standard output, i.e. no latex syntax.
@@ -199,21 +203,21 @@
                 and the value is a sorting key-value pair that filters the experiment results,
                 and the filtering is done based on the circuit metadata.
         """
         options = super()._default_options()
 
         options.plotter = CurvePlotter(MplDrawer())
         options.plot_raw_data = False
-        options.plot = True
         options.return_fit_parameters = True
         options.return_data_points = False
         options.data_processor = None
         options.normalization = False
         options.average_method = "shots_weighted"
         options.x_key = "xval"
+        options.fit_category = "formatted"
         options.result_parameters = []
         options.extra = {}
         options.fit_method = "least_squares"
         options.lmfit_options = {}
         options.p0 = {}
         options.bounds = {}
         options.fixed_parameters = {}
@@ -222,105 +226,55 @@
 
         # Set automatic validator for particular option values
         options.set_validator(field="data_processor", validator_value=DataProcessor)
         options.set_validator(field="plotter", validator_value=BasePlotter)
 
         return options
 
-    def set_options(self, **fields):
-        """Set the analysis options for :meth:`run` method.
-
-        Args:
-            fields: The fields to update the options
-
-        Raises:
-            KeyError: When removed option ``curve_fitter`` is set.
-        """
-        # TODO remove this in Qiskit Experiments v0.5
-
-        if "curve_fitter_options" in fields:
-            warnings.warn(
-                "The option 'curve_fitter_options' is replaced with 'lmfit_options.' "
-                "This option will be removed in Qiskit Experiments 0.5.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-            fields["lmfit_options"] = fields.pop("curve_fitter_options")
-
-        # TODO remove this in Qiskit Experiments 0.6
-        if "curve_drawer" in fields:
-            warnings.warn(
-                "The option 'curve_drawer' is replaced with 'plotter'. "
-                "This option will be removed in Qiskit Experiments 0.6.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-            # Set the plotter drawer to `curve_drawer`. If `curve_drawer` is the right type, set it
-            # directly. If not, wrap it in a compatibility drawer.
-            if isinstance(fields["curve_drawer"], BaseDrawer):
-                plotter = self.options.plotter
-                plotter.drawer = fields.pop("curve_drawer")
-                fields["plotter"] = plotter
-            else:
-                drawer = fields["curve_drawer"]
-                compat_drawer = LegacyCurveCompatDrawer(drawer)
-                plotter = self.options.plotter
-                plotter.drawer = compat_drawer
-                fields["plotter"] = plotter
-
-        super().set_options(**fields)
-
     @abstractmethod
     def _run_data_processing(
         self,
         raw_data: List[Dict],
-        models: List[lmfit.Model],
-    ) -> CurveData:
+        category: str = "raw",
+    ) -> ScatterTable:
         """Perform data processing from the experiment result payload.
 
         Args:
             raw_data: Payload in the experiment data.
-            models: A list of LMFIT models that provide the model name and
-                optionally data sorting keys.
+            category: Category string of the output dataset.
 
         Returns:
             Processed data that will be sent to the formatter method.
-
-        Raises:
-            DataProcessorError: When model is multi-objective function but
-                data sorting option is not provided.
-            DataProcessorError: When key for x values is not found in the metadata.
         """
 
     @abstractmethod
     def _format_data(
         self,
-        curve_data: CurveData,
-    ) -> CurveData:
-        """Postprocessing for the processed dataset.
+        curve_data: ScatterTable,
+        category: str = "formatted",
+    ) -> ScatterTable:
+        """Postprocessing for preparing the fitting data.
 
         Args:
             curve_data: Processed dataset created from experiment results.
+            category: Category string of the output dataset.
 
         Returns:
-            Formatted data.
+            New scatter table instance including fit data.
         """
 
     @abstractmethod
     def _run_curve_fit(
         self,
-        curve_data: CurveData,
-        models: List[lmfit.Model],
+        curve_data: ScatterTable,
     ) -> CurveFitResult:
         """Perform curve fitting on given data collection and fit models.
 
         Args:
             curve_data: Formatted data to fit.
-            models: A list of LMFIT models that are used to build a cost function
-                for the LMFIT minimizer.
 
         Returns:
             The best fitting outcome with minimum reduced chi-squared value.
         """
 
     def _evaluate_quality(
         self,
@@ -330,15 +284,15 @@
 
         Args:
             fit_data: Fit outcome.
 
         Returns:
             String that represents fit result quality. Usually "good" or "bad".
         """
-        if fit_data.reduced_chisq < 3.0:
+        if 0 < fit_data.reduced_chisq < 3.0:
             return "good"
         return "bad"
 
     def _create_analysis_results(
         self,
         fit_data: CurveFitResult,
         quality: str,
@@ -379,50 +333,61 @@
                 quality=quality,
                 extra=par_metadata,
             )
             outcomes.append(outcome)
 
         return outcomes
 
+    # pylint: disable=unused-argument
     def _create_curve_data(
         self,
-        curve_data: CurveData,
-        models: List[lmfit.Model],
+        curve_data: ScatterTable,
         **metadata,
     ) -> List[AnalysisResultData]:
         """Create analysis results for raw curve data.
 
         Args:
             curve_data: Formatted data that is used for the fitting.
-            models: A list of LMFIT models that provides model names
-                to extract subsets of experiment data.
 
         Returns:
             List of analysis result data.
         """
         samples = []
 
-        for model in models:
-            sub_data = curve_data.get_subset_of(model._name)
+        for model_name, sub_data in list(curve_data.groupby("model_name")):
             raw_datum = AnalysisResultData(
                 name=DATA_ENTRY_PREFIX + self.__class__.__name__,
                 value={
-                    "xdata": sub_data.x,
-                    "ydata": sub_data.y,
-                    "sigma": sub_data.y_err,
+                    "xdata": sub_data.xval.to_numpy(),
+                    "ydata": sub_data.yval.to_numpy(),
+                    "sigma": sub_data.yerr.to_numpy(),
                 },
                 extra={
-                    "name": model._name,
+                    "name": model_name,
                     **metadata,
                 },
             )
             samples.append(raw_datum)
 
         return samples
 
+    def _create_figures(
+        self,
+        curve_data: ScatterTable,
+    ) -> List["matplotlib.figure.Figure"]:
+        """Create a list of figures from the curve data.
+
+        Args:
+            curve_data: Scatter data table containing all data points.
+
+        Returns:
+            A list of figures.
+        """
+        return []
+
     def _initialize(
         self,
         experiment_data: ExperimentData,
     ):
         """Initialize curve analysis with experiment data.
 
         This method is called ahead of other processing.
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/composite_curve_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/composite_curve_analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,33 +15,37 @@
 """
 # pylint: disable=invalid-name
 import warnings
 from typing import Dict, List, Optional, Tuple, Union
 
 import lmfit
 import numpy as np
+import pandas as pd
 from uncertainties import unumpy as unp
 
+from qiskit.utils.deprecation import deprecate_func
+
 from qiskit_experiments.framework import (
     AnalysisResultData,
     BaseAnalysis,
     ExperimentData,
     Options,
 )
 from qiskit_experiments.visualization import (
     BaseDrawer,
     BasePlotter,
     CurvePlotter,
     LegacyCurveCompatDrawer,
     MplDrawer,
 )
-from qiskit_experiments.warnings import deprecated_function
 
-from .base_curve_analysis import PARAMS_ENTRY_PREFIX, BaseCurveAnalysis
+from qiskit_experiments.framework.containers import FigureType, ArtifactData
+from .base_curve_analysis import DATA_ENTRY_PREFIX, BaseCurveAnalysis, PARAMS_ENTRY_PREFIX
 from .curve_data import CurveFitResult
+from .scatter_table import ScatterTable
 from .utils import eval_with_uncertainties
 
 
 class CompositeCurveAnalysis(BaseAnalysis):
     r"""Composite Curve Analysis.
 
     The :class:`.CompositeCurveAnalysis` takes multiple curve analysis instances
@@ -79,16 +83,14 @@
             analysis = CompositeCurveAnalysis(analyses=analyses)
 
         This ``analysis`` will return two analysis result data for the fit parameter "freq"
         for experiments with the initial state :math:`|0\rangle` and :math:`|1\rangle`.
         The experimental circuits starting with different initial states must be
         distinguished by the circuit metadata ``{"init_state": 0}`` or ``{"init_state": 1}``,
         along with the "xval" in the same dictionary.
-        If you want to compute another quantity using two fitting outcomes, you can
-        override :meth:`CompositeCurveAnalysis._create_curve_data` in subclass.
 
     :class:`.CompositeCurveAnalysis` subclass may override following methods.
 
     .. rubric:: _evaluate_quality
 
     This method evaluates the quality of the composite fit based on
     the all analysis outcomes.
@@ -96,14 +98,19 @@
     otherwise it returns "bad".
 
     .. rubric:: _create_analysis_results
 
     This method is passed all the group fit outcomes and can return a list of
     new values to be stored in the analysis results.
 
+    .. rubric:: _create_figures
+
+    This method creates figures by consuming the scatter table data.
+    Figures are created when the analysis option ``plot`` is ``True``.
+
     """
 
     def __init__(
         self,
         analyses: List[BaseCurveAnalysis],
         name: Optional[str] = None,
     ):
@@ -138,17 +145,19 @@
 
     @property
     def plotter(self) -> BasePlotter:
         """A short-cut to the plotter instance."""
         return self._options.plotter
 
     @property
-    @deprecated_function(
-        last_version="0.6",
-        msg="Replaced by `plotter` from the new visualization submodule.",
+    @deprecate_func(
+        since="0.5",
+        additional_msg="Use `plotter` from the new visualization module instead.",
+        removal_timeline="after 0.6",
+        package_name="qiskit-experiments",
     )
     def drawer(self) -> BaseDrawer:
         """A short-cut for curve drawer instance, if set. ``None`` otherwise."""
         if hasattr(self._options, "curve_drawer"):
             return self._options.curve_drawer
         else:
             return None
@@ -203,35 +212,82 @@
             quality: Quality of fit outcome.
 
         Returns:
             List of analysis result data.
         """
         return []
 
+    def _create_figures(
+        self,
+        curve_data: ScatterTable,
+    ) -> List["matplotlib.figure.Figure"]:
+        """Create a list of figures from the curve data.
+
+        Args:
+            curve_data: Scatter data table containing all data points.
+
+        Returns:
+            A list of figures.
+        """
+        for analysis in self.analyses():
+            group_data = curve_data.filter(analysis=analysis.name)
+            model_names = analysis.model_names()
+            for series_id, sub_data in group_data.iter_by_series_id():
+                full_name = f"{model_names[series_id]}_{analysis.name}"
+                # Plot raw data scatters
+                if analysis.options.plot_raw_data:
+                    raw_data = sub_data.filter(category="raw")
+                    self.plotter.set_series_data(
+                        series_name=full_name,
+                        x=raw_data.x,
+                        y=raw_data.y,
+                    )
+                # Plot formatted data scatters
+                formatted_data = sub_data.filter(category=analysis.options.fit_category)
+                self.plotter.set_series_data(
+                    series_name=full_name,
+                    x_formatted=formatted_data.x,
+                    y_formatted=formatted_data.y,
+                    y_formatted_err=formatted_data.y_err,
+                )
+                # Plot fit lines
+                line_data = sub_data.filter(category="fitted")
+                if len(line_data) == 0:
+                    continue
+                fit_stdev = line_data.y_err
+                self.plotter.set_series_data(
+                    series_name=full_name,
+                    x_interp=line_data.x,
+                    y_interp=line_data.y,
+                    y_interp_err=fit_stdev if np.isfinite(fit_stdev).all() else None,
+                )
+
+        return [self.plotter.figure()]
+
     @classmethod
     def _default_options(cls) -> Options:
         """Default analysis options.
 
         Analysis Options:
             plotter (BasePlotter): A plotter instance to visualize
                 the analysis result.
             plot (bool): Set ``True`` to create figure for fit result.
                 This is ``True`` by default.
-            return_fit_parameters (bool): Set ``True`` to return all fit model parameters
-                with details of the fit outcome. Default to ``True``.
-            return_data_points (bool): Set ``True`` to include in the analysis result
+            return_fit_parameters (bool): (Deprecated) Set ``True`` to return all fit model parameters
+                with details of the fit outcome. Default to ``False``.
+            return_data_points (bool): (Deprecated) Set ``True`` to include in the analysis result
                 the formatted data points given to the fitter. Default to ``False``.
             extra (Dict[str, Any]): A dictionary that is appended to all database entries
                 as extra information.
         """
         options = super()._default_options()
         options.update_options(
             plotter=CurvePlotter(MplDrawer()),
             plot=True,
-            return_fit_parameters=True,
+            return_fit_parameters=False,
             return_data_points=False,
             extra={},
         )
 
         # Set automatic validator for particular option values
         options.set_validator(field="plotter", validator_value=BasePlotter)
 
@@ -270,129 +326,143 @@
                     UserWarning,
                 )
         super().set_options(**fields)
 
     def _run_analysis(
         self,
         experiment_data: ExperimentData,
-    ) -> Tuple[List[AnalysisResultData], List["matplotlib.figure.Figure"]]:
-
-        analysis_results = []
+    ) -> Tuple[List[Union[AnalysisResultData, ArtifactData]], List[FigureType]]:
+        result_data: List[Union[AnalysisResultData, ArtifactData]] = []
+        figures: List[FigureType] = []
+        artifacts: list[ArtifactData] = []
+
+        # Flag for plotting can be "always", "never", or "selective"
+        # the analysis option overrides self._generate_figures if set
+        if self.options.get("plot", None):
+            plot = "always"
+        elif self.options.get("plot", None) is False:
+            plot = "never"
+        else:
+            plot = getattr(self, "_generate_figures", "always")
 
         fit_dataset = {}
-        red_chi = {}
+        curve_data_set = []
         for analysis in self._analyses:
             analysis._initialize(experiment_data)
+            analysis.set_options(plot=False)
 
             metadata = analysis.options.extra.copy()
             metadata["group"] = analysis.name
 
-            processed_data = analysis._run_data_processing(
-                raw_data=experiment_data.data(),
-                models=analysis.models,
-            )
-
-            if self.options.plot and analysis.options.plot_raw_data:
-                for model in analysis.models:
-                    sub_data = processed_data.get_subset_of(model._name)
-                    self.plotter.set_series_data(
-                        model._name + f"_{analysis.name}",
-                        x=sub_data.x,
-                        y=sub_data.y,
-                    )
-
-            # Format data
-            formatted_data = analysis._format_data(processed_data)
-            if self.options.plot:
-                for model in analysis.models:
-                    sub_data = formatted_data.get_subset_of(model._name)
-                    self.plotter.set_series_data(
-                        model._name + f"_{analysis.name}",
-                        x_formatted=sub_data.x,
-                        y_formatted=sub_data.y,
-                        y_formatted_err=sub_data.y_err,
-                    )
-
-            # Run fitting
-            fit_data = analysis._run_curve_fit(
-                curve_data=formatted_data,
-                models=analysis.models,
-            )
+            table = analysis._format_data(analysis._run_data_processing(experiment_data.data()))
+            formatted_subset = table.filter(category=analysis.options.fit_category)
+            fit_data = analysis._run_curve_fit(formatted_subset)
+            fit_dataset[analysis.name] = fit_data
 
             if fit_data.success:
                 quality = analysis._evaluate_quality(fit_data)
-                red_chi[analysis.name] = fit_data.reduced_chisq
             else:
                 quality = "bad"
 
             if self.options.return_fit_parameters:
+                # Store fit status overview entry regardless of success.
+                # This is sometime useful when debugging the fitting code.
                 overview = AnalysisResultData(
                     name=PARAMS_ENTRY_PREFIX + analysis.name,
                     value=fit_data,
                     quality=quality,
                     extra=metadata,
                 )
-                analysis_results.append(overview)
+                result_data.append(overview)
 
             if fit_data.success:
-                # Add extra analysis results
-                analysis_results.extend(
+                # Add fit data to curve data table
+                model_names = analysis.model_names()
+                for series_id, sub_data in formatted_subset.iter_by_series_id():
+                    xval = sub_data.x
+                    if len(xval) == 0:
+                        # If data is empty, skip drawing this model.
+                        # This is the case when fit model exist but no data to fit is provided.
+                        continue
+                    # Compute X, Y values with fit parameters.
+                    xval_arr_fit = np.linspace(np.min(xval), np.max(xval), num=100, dtype=float)
+                    uval_arr_fit = eval_with_uncertainties(
+                        x=xval_arr_fit,
+                        model=analysis.models[series_id],
+                        params=fit_data.ufloat_params,
+                    )
+                    yval_arr_fit = unp.nominal_values(uval_arr_fit)
+                    if fit_data.covar is not None:
+                        yerr_arr_fit = unp.std_devs(uval_arr_fit)
+                    else:
+                        yerr_arr_fit = np.zeros_like(xval_arr_fit)
+                    for xval, yval, yerr in zip(xval_arr_fit, yval_arr_fit, yerr_arr_fit):
+                        table.add_row(
+                            xval=xval,
+                            yval=yval,
+                            yerr=yerr,
+                            series_name=model_names[series_id],
+                            series_id=series_id,
+                            category="fitted",
+                            analysis=analysis.name,
+                        )
+                result_data.extend(
                     analysis._create_analysis_results(
-                        fit_data=fit_data, quality=quality, **metadata.copy()
+                        fit_data=fit_data,
+                        quality=quality,
+                        **metadata.copy(),
                     )
                 )
 
-                # Draw fit result
-                if self.options.plot:
-                    x_interp = np.linspace(
-                        np.min(formatted_data.x), np.max(formatted_data.x), num=100
-                    )
-                    for model in analysis.models:
-                        y_data_with_uncertainty = eval_with_uncertainties(
-                            x=x_interp,
-                            model=model,
-                            params=fit_data.ufloat_params,
-                        )
-                        y_interp = unp.nominal_values(y_data_with_uncertainty)
-                        # Add fit line data
-                        self.plotter.set_series_data(
-                            model._name + f"_{analysis.name}",
-                            x_interp=x_interp,
-                            y_interp=y_interp,
-                        )
-                        if fit_data.covar is not None:
-                            # Add confidence interval data
-                            y_interp_err = unp.std_devs(y_data_with_uncertainty)
-                            if np.isfinite(y_interp_err).all():
-                                self.plotter.set_series_data(
-                                    model._name + f"_{analysis.name}",
-                                    y_interp_err=y_interp_err,
-                                )
-
-            # Add raw data points
             if self.options.return_data_points:
-                analysis_results.extend(
-                    analysis._create_curve_data(
-                        curve_data=formatted_data,
-                        models=analysis.models,
-                        **metadata,
-                    )
+                # Add raw data points
+                warnings.warn(
+                    f"{DATA_ENTRY_PREFIX + self.name} has been moved to experiment data artifacts. "
+                    "Saving this result with 'return_data_points'=True will be disabled in "
+                    "Qiskit Experiments 0.7.",
+                    DeprecationWarning,
+                )
+                result_data.extend(
+                    analysis._create_curve_data(curve_data=formatted_subset, **metadata)
                 )
 
-            fit_dataset[analysis.name] = fit_data
+            curve_data_set.append(table)
 
+        combined_curve_data = ScatterTable.from_dataframe(
+            pd.concat([d.dataframe for d in curve_data_set])
+        )
         total_quality = self._evaluate_quality(fit_dataset)
-        if red_chi:
-            self.plotter.set_supplementary_data(fit_red_chi=red_chi)
+
+        # After the quality is determined, plot can become a boolean flag for whether
+        # to generate the figure
+        plot_bool = plot == "always" or (plot == "selective" and total_quality == "bad")
 
         # Create analysis results by combining all fit data
         if all(fit_data.success for fit_data in fit_dataset.values()):
-            primary_results = self._create_analysis_results(
+            composite_results = self._create_analysis_results(
                 fit_data=fit_dataset, quality=total_quality, **self.options.extra.copy()
             )
-            analysis_results.extend(primary_results)
-            self.plotter.set_supplementary_data(primary_results=primary_results)
+            result_data.extend(composite_results)
+        else:
+            composite_results = []
 
-        if self.options.plot:
-            return analysis_results, [self.plotter.figure()]
+        artifacts.append(
+            ArtifactData(
+                name="curve_data",
+                data=combined_curve_data,
+            )
+        )
+        artifacts.append(
+            ArtifactData(
+                name="fit_summary",
+                data=fit_dataset,
+            )
+        )
+
+        if plot_bool:
+            self.plotter.set_supplementary_data(
+                fit_red_chi={k: v.reduced_chisq for k, v in fit_dataset.items() if v.success},
+                primary_results=composite_results,
+            )
+            figures.extend(self._create_figures(curve_data=combined_curve_data))
 
-        return analysis_results, []
+        return result_data + artifacts, figures
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/curve_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/curve_analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,28 +9,43 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
 Analysis class for curve fitting.
 """
+import warnings
+
 # pylint: disable=invalid-name
 
 from typing import Dict, List, Tuple, Union, Optional
+from functools import partial
 
 import lmfit
 import numpy as np
+import pandas as pd
 from uncertainties import unumpy as unp
 
-from qiskit_experiments.framework import ExperimentData, AnalysisResultData
+from qiskit_experiments.framework import (
+    ExperimentData,
+    AnalysisResultData,
+)
+from qiskit_experiments.framework.containers import FigureType, ArtifactData
 from qiskit_experiments.data_processing.exceptions import DataProcessorError
 
-from .base_curve_analysis import BaseCurveAnalysis, PARAMS_ENTRY_PREFIX
-from .curve_data import CurveData, FitOptions, CurveFitResult
-from .utils import eval_with_uncertainties, convert_lmfit_result, multi_mean_xy_data, data_sort
+from .base_curve_analysis import BaseCurveAnalysis, DATA_ENTRY_PREFIX, PARAMS_ENTRY_PREFIX
+from .curve_data import FitOptions, CurveFitResult
+from .scatter_table import ScatterTable
+from .utils import (
+    eval_with_uncertainties,
+    convert_lmfit_result,
+    shot_weighted_average,
+    inverse_weighted_variance,
+    sample_average,
+)
 
 
 class CurveAnalysis(BaseCurveAnalysis):
     """Base class for curve analysis with single curve group.
 
     The fit parameters from the series defined under the analysis class are all shared
     and the analysis performs a single multi-objective function optimization.
@@ -72,21 +87,18 @@
     Usually it returns string "good" or "bad" according to the evaluation.
 
     .. rubric:: _create_analysis_results
 
     This method creates analysis results for important fit parameters
     that might be defined by analysis options ``result_parameters``.
 
-    .. rubric:: _create_curve_data
+    .. rubric:: _create_figures
 
-    This method creates analysis results containing the formatted dataset,
-    i.e. data used for the fitting.
-    Entries are created when the analysis option ``return_data_points`` is ``True``.
-    If analysis consists of multiple series, an analysis result is created for
-    each series definition.
+    This method creates figures by consuming the scatter table data.
+    Figures are created when the analysis option ``plot`` is ``True``.
 
     .. rubric:: _initialize
 
     This method initializes analysis options against input experiment data.
     Usually this method is called before other methods are called.
 
     """
@@ -128,162 +140,170 @@
         return unite_params
 
     @property
     def models(self) -> List[lmfit.Model]:
         """Return fit models."""
         return self._models
 
+    def model_names(self) -> List[str]:
+        """Return model names."""
+        return [getattr(m, "_name", f"model-{i}") for i, m in enumerate(self._models)]
+
     def _run_data_processing(
         self,
         raw_data: List[Dict],
-        models: List[lmfit.Model],
-    ) -> CurveData:
+        category: str = "raw",
+    ) -> ScatterTable:
         """Perform data processing from the experiment result payload.
 
         Args:
             raw_data: Payload in the experiment data.
-            models: A list of LMFIT models that provide the model name and
-                optionally data sorting keys.
+            category: Category string of the output dataset.
 
         Returns:
             Processed data that will be sent to the formatter method.
 
         Raises:
-            DataProcessorError: When model is a multi-objective function but
-                data sorting option is not provided.
             DataProcessorError: When key for x values is not found in the metadata.
+            ValueError: When data processor is not provided.
         """
+        opt = self.options
 
-        def _matched(metadata, **filters):
-            try:
-                return all(metadata[key] == val for key, val in filters.items())
-            except KeyError:
-                return False
-
-        if not self.options.filter_data:
-            analyzed_data = raw_data
+        # Create table
+        if opt.filter_data:
+            to_process = [d for d in raw_data if opt.filter_data.items() <= d["metadata"].items()]
         else:
-            analyzed_data = [
-                d for d in raw_data if _matched(d["metadata"], **self.options.filter_data)
-            ]
-
-        x_key = self.options.x_key
-
-        try:
-            xdata = np.asarray([datum["metadata"][x_key] for datum in analyzed_data], dtype=float)
-        except KeyError as ex:
-            raise DataProcessorError(
-                f"X value key {x_key} is not defined in circuit metadata."
-            ) from ex
-
-        ydata = self.options.data_processor(analyzed_data)
-        shots = np.asarray([datum.get("shots", np.nan) for datum in analyzed_data])
-
-        if len(models) == 1:
-            # all data belongs to the single model
-            data_allocation = np.full(xdata.size, 0, dtype=int)
+            to_process = raw_data
+
+        # Compute y value
+        if not self.options.data_processor:
+            raise ValueError(
+                f"Data processor is not set for the {self.__class__.__name__} instance. "
+                "Initialize the instance with the experiment data, or set the "
+                "data_processor analysis options."
+            )
+        processed = self.options.data_processor(to_process)
+        yvals = unp.nominal_values(processed).flatten()
+        with np.errstate(invalid="ignore"):
+            # For averaged data, the processed std dev will be NaN.
+            # Setting std_devs to NaN will trigger floating point exceptions
+            # which we can ignore. See https://stackoverflow.com/q/75656026
+            yerrs = unp.std_devs(processed).flatten()
+
+        # Prepare circuit metadata to data class mapper from data_subfit_map value.
+        if len(self._models) == 1:
+            classifier = {self.model_names()[0]: {}}
         else:
-            data_allocation = np.full(xdata.size, -1, dtype=int)
-            for idx, sub_model in enumerate(models):
-                try:
-                    tags = self.options.data_subfit_map[sub_model._name]
-                except KeyError as ex:
-                    raise DataProcessorError(
-                        f"Data sort options for model {sub_model._name} is not defined. "
-                        "Please provide the 'data_subfit_map' analysis option for this model."
-                    ) from ex
-                if tags is None:
-                    continue
-                matched_inds = np.asarray(
-                    [_matched(d["metadata"], **tags) for d in analyzed_data], dtype=bool
-                )
-                data_allocation[matched_inds] = idx
+            classifier = self.options.data_subfit_map
 
-        return CurveData(
-            x=xdata,
-            y=unp.nominal_values(ydata),
-            y_err=unp.std_devs(ydata),
-            shots=shots,
-            data_allocation=data_allocation,
-            labels=[sub_model._name for sub_model in models],
-        )
+        table = ScatterTable()
+        for datum, yval, yerr in zip(to_process, yvals, yerrs):
+            metadata = datum["metadata"]
+            try:
+                xval = metadata[opt.x_key]
+            except KeyError as ex:
+                raise DataProcessorError(
+                    f"X value key {opt.x_key} is not defined in the circuit metadata."
+                ) from ex
+
+            # Assign series name and series id
+            for series_id, (series_name, spec) in enumerate(classifier.items()):
+                if spec.items() <= metadata.items():
+                    break
+            else:
+                # This is unclassified data.
+                series_name = pd.NA
+                series_id = pd.NA
+            table.add_row(
+                xval=xval,
+                yval=yval,
+                yerr=yerr,
+                series_name=series_name,
+                series_id=series_id,
+                category=category,
+                shots=datum.get("shots", pd.NA),
+                analysis=self.name,
+            )
+        return table
 
     def _format_data(
         self,
-        curve_data: CurveData,
-    ) -> CurveData:
-        """Postprocessing for the processed dataset.
+        curve_data: ScatterTable,
+        category: str = "formatted",
+    ) -> ScatterTable:
+        """Postprocessing for preparing the fitting data.
 
         Args:
             curve_data: Processed dataset created from experiment results.
+            category: Category string of the output dataset.
 
         Returns:
-            Formatted data.
+            New scatter table instance including data to fit.
         """
-        # take average over the same x value by keeping sigma
-        data_allocation, xdata, ydata, sigma, shots = multi_mean_xy_data(
-            series=curve_data.data_allocation,
-            xdata=curve_data.x,
-            ydata=curve_data.y,
-            sigma=curve_data.y_err,
-            shots=curve_data.shots,
-            method=self.options.average_method,
-        )
-
-        # sort by x value in ascending order
-        data_allocation, xdata, ydata, sigma, shots = data_sort(
-            series=data_allocation,
-            xdata=xdata,
-            ydata=ydata,
-            sigma=sigma,
-            shots=shots,
-        )
+        averaging_methods = {
+            "shots_weighted": shot_weighted_average,
+            "iwv": inverse_weighted_variance,
+            "sample": sample_average,
+        }
+        average = averaging_methods[self.options.average_method]
+        model_names = self.model_names()
+
+        for (series_name, xval), sub_data in curve_data.iter_groups("series_name", "xval"):
+            avg_yval, avg_yerr, shots = average(
+                sub_data.y,
+                sub_data.y_err,
+                sub_data.shots,
+            )
+            try:
+                series_id = model_names.index(series_name)
+            except ValueError:
+                series_id = pd.NA
+            curve_data.add_row(
+                xval=xval,
+                yval=avg_yval,
+                yerr=avg_yerr,
+                series_name=series_name,
+                series_id=series_id,
+                category=category,
+                shots=shots,
+                analysis=self.name,
+            )
 
-        return CurveData(
-            x=xdata,
-            y=ydata,
-            y_err=sigma,
-            shots=shots,
-            data_allocation=data_allocation,
-            labels=curve_data.labels,
-        )
+        return curve_data
 
     def _generate_fit_guesses(
         self,
         user_opt: FitOptions,
-        curve_data: CurveData,  # pylint: disable=unused-argument
+        curve_data: ScatterTable,  # pylint: disable=unused-argument
     ) -> Union[FitOptions, List[FitOptions]]:
         """Create algorithmic initial fit guess from analysis options and curve data.
 
         Args:
             user_opt: Fit options filled with user provided guess and bounds.
             curve_data: Formatted data collection to fit.
 
         Returns:
             List of fit options that are passed to the fitter function.
         """
         return user_opt
 
     def _run_curve_fit(
         self,
-        curve_data: CurveData,
-        models: List[lmfit.Model],
+        curve_data: ScatterTable,
     ) -> CurveFitResult:
         """Perform curve fitting on given data collection and fit models.
 
         Args:
             curve_data: Formatted data to fit.
-            models: A list of LMFIT models that are used to build a cost function
-                for the LMFIT minimizer.
 
         Returns:
             The best fitting outcome with minimum reduced chi-squared value.
         """
         unite_parameter_names = []
-        for model in models:
+        for model in self._models:
             # Seems like this is not efficient looping, but using set operation sometimes
             # yields bad fit. Not sure if this is an edge case, but
             # `TestRamseyXY` unittest failed due to the significant chisq value
             # in which the least_square fitter terminates with `xtol` rather than `ftol`
             # condition, i.e. `ftol` condition indicates termination by cost function.
             # This code respects the ordering of parameters so that it matches with
             # the signature of fit function and it is backward compatible.
@@ -310,44 +330,40 @@
             fixed_parameters = {}
 
         fit_options = self._generate_fit_guesses(default_fit_opt, curve_data)
 
         if isinstance(fit_options, FitOptions):
             fit_options = [fit_options]
 
+        # Create convenient function to compute residual of the models.
+        partial_residuals = []
         valid_uncertainty = np.all(np.isfinite(curve_data.y_err))
-
-        model_weights = {}
-        if valid_uncertainty:
-            for model in models:
-                sub_yerr = curve_data.get_subset_of(model._name).y_err
-                if len(sub_yerr) == 0:
-                    continue
-                nonzero_yerr = np.where(np.isclose(sub_yerr, 0.0), np.finfo(float).eps, sub_yerr)
+        for idx, sub_data in curve_data.iter_by_series_id():
+            if valid_uncertainty:
+                nonzero_yerr = np.where(
+                    np.isclose(sub_data.y_err, 0.0),
+                    np.finfo(float).eps,
+                    sub_data.y_err,
+                )
                 raw_weights = 1 / nonzero_yerr
                 # Remove outlier. When all sample values are the same with sample average,
                 # or sampling error is zero with shot-weighted average,
                 # some yerr values might be very close to zero, yielding significant weights.
                 # With such outlier, the fit doesn't sense residual of other data points.
                 maximum_weight = np.percentile(raw_weights, 90)
-                model_weights[model._name] = np.clip(raw_weights, 0.0, maximum_weight)
-
-        # Objective function for minimize. This computes composite residuals of sub models.
-        def _objective(_params):
-            ys = []
-            for model in models:
-                sub_data = curve_data.get_subset_of(model._name)
-                yi = model._residual(
-                    params=_params,
-                    data=sub_data.y,
-                    weights=model_weights.get(model._name, None),
-                    x=sub_data.x,
-                )
-                ys.append(yi)
-            return np.concatenate(ys)
+                weights = np.clip(raw_weights, 0.0, maximum_weight)
+            else:
+                weights = None
+            model_residual = partial(
+                self._models[idx]._residual,
+                data=sub_data.y,
+                weights=weights,
+                x=sub_data.x,
+            )
+            partial_residuals.append(model_residual)
 
         # Run fit for each configuration
         res = None
         for fit_option in fit_options:
             # Setup parameter configuration, i.e. init value, bounds
             guess_params = lmfit.Parameters()
             for name in unite_parameter_names:
@@ -359,15 +375,15 @@
                     max=bounds[1],
                     vary=name not in fixed_parameters,
                 )
 
             try:
                 with np.errstate(all="ignore"):
                     new = lmfit.minimize(
-                        fcn=_objective,
+                        fcn=lambda x: np.concatenate([p(x) for p in partial_residuals]),
                         params=guess_params,
                         method=self.options.fit_method,
                         scale_covar=not valid_uncertainty,
                         nan_policy="omit",
                         **fit_option.fitter_opts,
                     )
             except Exception:  # pylint: disable=broad-except
@@ -376,127 +392,184 @@
             if res is None or not res.success:
                 res = new
                 continue
 
             if new.success and res.redchi > new.redchi:
                 res = new
 
-        return convert_lmfit_result(res, models, curve_data.x, curve_data.y)
-
-    def _run_analysis(
-        self, experiment_data: ExperimentData
-    ) -> Tuple[List[AnalysisResultData], List["pyplot.Figure"]]:
-
-        # Prepare for fitting
-        self._initialize(experiment_data)
+        return convert_lmfit_result(
+            res,
+            self._models,
+            curve_data.x,
+            curve_data.y,
+        )
 
-        analysis_results = []
+    def _create_figures(
+        self,
+        curve_data: ScatterTable,
+    ) -> List["matplotlib.figure.Figure"]:
+        """Create a list of figures from the curve data.
 
-        # Run data processing
-        processed_data = self._run_data_processing(
-            raw_data=experiment_data.data(),
-            models=self._models,
-        )
+        Args:
+            curve_data: Scatter data table containing all data points.
 
-        if self.options.plot and self.options.plot_raw_data:
-            for model in self._models:
-                sub_data = processed_data.get_subset_of(model._name)
+        Returns:
+            A list of figures.
+        """
+        for series_id, sub_data in curve_data.iter_by_series_id():
+            model_name = self.model_names()[series_id]
+            # Plot raw data scatters
+            if self.options.plot_raw_data:
+                raw_data = sub_data.filter(category="raw")
                 self.plotter.set_series_data(
-                    model._name,
-                    x=sub_data.x,
-                    y=sub_data.y,
+                    series_name=model_name,
+                    x=raw_data.x,
+                    y=raw_data.y,
                 )
-
-        # Format data
-        formatted_data = self._format_data(processed_data)
-        if self.options.plot:
-            for model in self._models:
-                sub_data = formatted_data.get_subset_of(model._name)
+            # Plot formatted data scatters
+            formatted_data = sub_data.filter(category=self.options.fit_category)
+            self.plotter.set_series_data(
+                series_name=model_name,
+                x_formatted=formatted_data.x,
+                y_formatted=formatted_data.y,
+                y_formatted_err=formatted_data.y_err,
+            )
+            # Plot fit lines
+            line_data = sub_data.filter(category="fitted")
+            if len(line_data) == 0:
+                continue
+            self.plotter.set_series_data(
+                series_name=model_name,
+                x_interp=line_data.x,
+                y_interp=line_data.y,
+            )
+            fit_stdev = line_data.y_err
+            if np.isfinite(fit_stdev).all():
                 self.plotter.set_series_data(
-                    model._name,
-                    x_formatted=sub_data.x,
-                    y_formatted=sub_data.y,
-                    y_formatted_err=sub_data.y_err,
+                    series_name=model_name,
+                    y_interp_err=fit_stdev,
                 )
 
-        # Run fitting
-        fit_data = self._run_curve_fit(
-            curve_data=formatted_data,
-            models=self._models,
-        )
+        return [self.plotter.figure()]
+
+    def _run_analysis(
+        self,
+        experiment_data: ExperimentData,
+    ) -> Tuple[List[Union[AnalysisResultData, ArtifactData]], List[FigureType]]:
+        figures: List[FigureType] = []
+        result_data: List[Union[AnalysisResultData, ArtifactData]] = []
+        artifacts: list[ArtifactData] = []
+
+        # Flag for plotting can be "always", "never", or "selective"
+        # the analysis option overrides self._generate_figures if set
+        if self.options.get("plot", None):
+            plot = "always"
+        elif self.options.get("plot", None) is False:
+            plot = "never"
+        else:
+            plot = getattr(self, "_generate_figures", "always")
+
+        # Prepare for fitting
+        self._initialize(experiment_data)
+
+        table = self._format_data(self._run_data_processing(experiment_data.data()))
+        formatted_subset = table.filter(category=self.options.fit_category)
+        fit_data = self._run_curve_fit(formatted_subset)
 
         if fit_data.success:
             quality = self._evaluate_quality(fit_data)
-            self.plotter.set_supplementary_data(fit_red_chi=fit_data.reduced_chisq)
         else:
             quality = "bad"
 
+        # After the quality is determined, plot can become a boolean flag for whether
+        # to generate the figure
+        plot_bool = plot == "always" or (plot == "selective" and quality == "bad")
+
         if self.options.return_fit_parameters:
             # Store fit status overview entry regardless of success.
             # This is sometime useful when debugging the fitting code.
             overview = AnalysisResultData(
                 name=PARAMS_ENTRY_PREFIX + self.name,
                 value=fit_data,
                 quality=quality,
                 extra=self.options.extra,
             )
-            analysis_results.append(overview)
+            result_data.append(overview)
 
-        # Create figure and result data
         if fit_data.success:
-            # Create analysis results
-            primary_results = self._create_analysis_results(
-                fit_data=fit_data, quality=quality, **self.options.extra.copy()
-            )
-            analysis_results.extend(primary_results)
-            self.plotter.set_supplementary_data(primary_results=primary_results)
-
-            # Draw fit curves and report
-            if self.options.plot:
-                for model in self._models:
-                    sub_data = formatted_data.get_subset_of(model._name)
-                    if sub_data.x.size == 0:
-                        # If data is empty, skip drawing this model.
-                        # This is the case when fit model exist but no data to fit is provided.
-                        # For example, experiment may omit experimenting with some setting.
-                        continue
-                    x_interp = np.linspace(np.min(sub_data.x), np.max(sub_data.x), num=100)
-
-                    y_data_with_uncertainty = eval_with_uncertainties(
-                        x=x_interp,
-                        model=model,
-                        params=fit_data.ufloat_params,
-                    )
-                    y_interp = unp.nominal_values(y_data_with_uncertainty)
-                    # Add fit line data
-                    self.plotter.set_series_data(
-                        model._name,
-                        x_interp=x_interp,
-                        y_interp=y_interp,
+            # Add fit data to curve data table
+            model_names = self.model_names()
+            for series_id, sub_data in formatted_subset.iter_by_series_id():
+                xval = sub_data.x
+                if len(xval) == 0:
+                    # If data is empty, skip drawing this model.
+                    # This is the case when fit model exist but no data to fit is provided.
+                    continue
+                # Compute X, Y values with fit parameters.
+                xval_arr_fit = np.linspace(np.min(xval), np.max(xval), num=100, dtype=float)
+                uval_arr_fit = eval_with_uncertainties(
+                    x=xval_arr_fit,
+                    model=self._models[series_id],
+                    params=fit_data.ufloat_params,
+                )
+                yval_arr_fit = unp.nominal_values(uval_arr_fit)
+                if fit_data.covar is not None:
+                    yerr_arr_fit = unp.std_devs(uval_arr_fit)
+                else:
+                    yerr_arr_fit = np.zeros_like(xval_arr_fit)
+                for xval, yval, yerr in zip(xval_arr_fit, yval_arr_fit, yerr_arr_fit):
+                    table.add_row(
+                        xval=xval,
+                        yval=yval,
+                        yerr=yerr,
+                        series_name=model_names[series_id],
+                        series_id=series_id,
+                        category="fitted",
+                        analysis=self.name,
                     )
-                    if fit_data.covar is not None:
-                        # Add confidence interval data
-                        y_interp_err = unp.std_devs(y_data_with_uncertainty)
-                        if np.isfinite(y_interp_err).all():
-                            self.plotter.set_series_data(
-                                model._name,
-                                y_interp_err=y_interp_err,
-                            )
+            result_data.extend(
+                self._create_analysis_results(
+                    fit_data=fit_data,
+                    quality=quality,
+                    **self.options.extra.copy(),
+                )
+            )
 
-        # Add raw data points
         if self.options.return_data_points:
-            analysis_results.extend(
-                self._create_curve_data(curve_data=formatted_data, models=self._models)
+            # Add raw data points
+            warnings.warn(
+                f"{DATA_ENTRY_PREFIX + self.name} has been moved to experiment data artifacts. "
+                "Saving this result with 'return_data_points'=True will be disabled in "
+                "Qiskit Experiments 0.7.",
+                DeprecationWarning,
             )
+            result_data.extend(self._create_curve_data(curve_data=formatted_subset))
 
-        # Finalize plot
-        if self.options.plot:
-            return analysis_results, [self.plotter.figure()]
+        artifacts.append(
+            ArtifactData(
+                name="curve_data",
+                data=table,
+            )
+        )
+        artifacts.append(
+            ArtifactData(
+                name="fit_summary",
+                data=fit_data,
+            )
+        )
+
+        if plot_bool:
+            if fit_data.success:
+                self.plotter.set_supplementary_data(
+                    fit_red_chi=fit_data.reduced_chisq,
+                    primary_results=[r for r in result_data if not r.name.startswith("@")],
+                )
+            figures.extend(self._create_figures(curve_data=table))
 
-        return analysis_results, []
+        return result_data + artifacts, figures
 
     def __getstate__(self):
         state = self.__dict__.copy()
         # Convert models into JSON str.
         # This object includes local function and cannot be pickled.
         source = [m.dumps() for m in state["_models"]]
         state["_models"] = source
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/curve_data.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/curve_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 import itertools
 import inspect
 from typing import Any, Dict, Union, List, Tuple, Optional, Iterable, Callable
 
 import numpy as np
 import uncertainties
 from uncertainties.unumpy import uarray
+
+from qiskit.utils.deprecation import deprecate_func
+
 from qiskit_experiments.exceptions import AnalysisError
-from qiskit_experiments.warnings import deprecated_function, deprecated_class
 
 
-@deprecated_class("0.5", msg="SeriesDef is now replaced with LMFIT Model.")
 @dataclasses.dataclass(frozen=True)
 class SeriesDef:
     """A dataclass to describe the definition of the curve.
 
     Attributes:
         fit_func: A callable that defines the fit model of this curve. The argument names
             in the callable are parsed to create the fit parameter list, which will appear
@@ -58,14 +59,24 @@
     name: str = "Series-0"
     plot_color: str = "black"
     plot_symbol: str = "o"
     canvas: Optional[int] = None
     model_description: Optional[str] = None
     signature: Tuple[str, ...] = dataclasses.field(init=False)
 
+    @deprecate_func(
+        since="0.5",
+        additional_msg="SeriesDef has been replaced by the LMFIT module.",
+        removal_timeline="after 0.6",
+        package_name="qiskit-experiments",
+    )
+    def __init__(self, *args, **kwargs):
+        self.args = args
+        self.kwargs = kwargs
+
     def __post_init__(self):
         """Parse the fit function signature to extract the names of the variables.
         Fit functions take arguments F(x, p0, p1, p2, ...) thus the first value should be excluded.
         """
         signature = list(inspect.signature(self.fit_func).parameters.keys())
         fitparams = tuple(signature[1:])
 
@@ -97,14 +108,23 @@
     x: np.ndarray
     y: np.ndarray
     y_err: np.ndarray
     shots: np.ndarray
     data_allocation: np.ndarray
     labels: List[str]
 
+    @deprecate_func(
+        since="0.6",
+        additional_msg="CurveData is replaced by `ScatterTable`'s DataFrame representation.",
+        removal_timeline="after 0.7",
+        package_name="qiskit-experiments",
+    )
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
     def get_subset_of(self, index: Union[str, int]) -> "CurveData":
         """Filter data by series name or index.
 
         Args:
             index: Series index of name.
 
         Returns:
@@ -211,18 +231,21 @@
                 ufloat_fitvals = uncertainties.correlated_values(
                     nom_values=[self.params[name] for name in self.var_names],
                     covariance_mat=self.covar,
                     tags=self.var_names,
                 )
             else:
                 # Invalid covariance matrix. Std dev is set to nan, i.e. not computed.
-                ufloat_fitvals = uarray(
-                    nominal_values=[self.params[name] for name in self.var_names],
-                    std_devs=np.full(len(self.var_names), np.nan),
-                )
+                with np.errstate(invalid="ignore"):
+                    # Setting std_devs to NaN will trigger floating point exceptions
+                    # which we can ignore. See https://stackoverflow.com/q/75656026
+                    ufloat_fitvals = uarray(
+                        nominal_values=[self.params[name] for name in self.var_names],
+                        std_devs=np.full(len(self.var_names), np.nan),
+                    )
             # Combine fixed params and fitting variables into a single dictionary
             # Fixed parameter has zero std_dev
             ufloat_params = {}
             for name in self.params.keys():
                 try:
                     uind = self.var_names.index(name)
                     ufloat_params[name] = ufloat_fitvals[uind]
@@ -245,19 +268,14 @@
             correl = self.covar / stdevs / stdevs[:, np.newaxis]
         else:
             correl = None
 
         setattr(self, "_correl", correl)
         return correl
 
-    @deprecated_function("0.5", "Use '.ufloat_params' which returns a dictionary instead.")
-    def fitval(self, key: str) -> uncertainties.UFloat:
-        """Deprecated. Return UFloat parameter specified by the key."""
-        return self.ufloat_params[key]
-
     def __str__(self):
         ret = "CurveFitResult:"
         ret += f"\n - fitting method: {self.method}"
         ret += f"\n - number of sub-models: {len(self.model_repr)}"
         for model_name, model_expr in self.model_repr.items():
             if len(model_expr) > 60:
                 model_expr = f"{model_expr[:60]}..."
@@ -324,17 +342,14 @@
         }
 
     @classmethod
     def __json_decode__(cls, value):
         return cls(**value)
 
 
-@deprecated_class(
-    "0.5", msg="Fit data is replaced with 'CurveFitResult' based on LMFIT minimizer result."
-)
 @dataclasses.dataclass(frozen=True)
 class FitData:
     """A dataclass to store the outcome of the fitting.
 
     Attributes:
         popt: List of optimal parameter values with uncertainties if available.
         popt_keys: List of parameter names being fit.
@@ -349,14 +364,23 @@
     popt_keys: List[str]
     pcov: np.ndarray
     reduced_chisq: float
     dof: int
     x_data: np.ndarray
     y_data: np.ndarray
 
+    @deprecate_func(
+        since="0.5",
+        additional_msg="Fit data is replaced with 'CurveFitResult' based on LMFIT minimizer result.",
+        removal_timeline="after 0.6",
+        package_name="qiskit-experiments",
+    )
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
     @property
     def x_range(self) -> Tuple[float, float]:
         """Range of x values."""
         return np.min(self.x_data), np.max(self.x_data)
 
     @property
     def y_range(self) -> Tuple[float, float]:
@@ -466,15 +490,15 @@
             if self.get(key) is None:
                 self[key] = value
 
     @staticmethod
     def format(value: Any) -> Any:
         """Format dictionary value.
 
-        Subcasses may override this method to provide their own validation.
+        Subclasses may override this method to provide their own validation.
 
         Args:
             value: New value to assign.
 
         Returns:
             Formatted value.
         """
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/guess.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/guess.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,15 +394,17 @@
     """
     valid_inds = y > b
 
     # Remove y values below b
     y = y[valid_inds]
     x = x[valid_inds]
 
-    if len(x) < 2:
+    if len(x) == 0:
+        return 0
+    if len(x) == 1:
         # If number of element is 1, assume y(0) = 1.0 and directly compute alpha.
         a = 1.0 - b
         return ((y[0] - b) / a) ** (1 / x[0])
 
     ry = (y[1:] - b) / (y[:-1] - b)
     dx = np.diff(x)
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/standard_analysis/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/standard_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/standard_analysis/bloch_trajectory.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/standard_analysis/bloch_trajectory.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         }
 
         return default_options
 
     def _generate_fit_guesses(
         self,
         user_opt: curve.FitOptions,
-        curve_data: curve.CurveData,
+        curve_data: curve.ScatterTable,
     ) -> Union[curve.FitOptions, List[curve.FitOptions]]:
         """Create algorithmic initial fit guess from analysis options and curve data.
 
         Args:
             user_opt: Fit options filled with user provided guess and bounds.
             curve_data: Formatted data collection to fit.
 
@@ -166,17 +166,17 @@
             List of fit options that are passed to the fitter function.
         """
         fit_options = []
 
         user_opt.bounds.set_if_empty(t_off=(0, np.inf), b=(-1, 1))
         user_opt.p0.set_if_empty(b=1e-9)
 
-        x_data = curve_data.get_subset_of("x")
-        y_data = curve_data.get_subset_of("y")
-        z_data = curve_data.get_subset_of("z")
+        x_data = curve_data.filter(series="x")
+        y_data = curve_data.filter(series="y")
+        z_data = curve_data.filter(series="z")
 
         omega_xyz = []
         for data in (x_data, y_data, z_data):
             ymin, ymax = np.percentile(data.y, [10, 90])
             if ymax - ymin < 0.2:
                 # oscillation amplitude might be almost zero,
                 # then exclude from average because of lower SNR
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/standard_analysis/decay.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/standard_analysis/decay.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             ],
             name=name,
         )
 
     def _generate_fit_guesses(
         self,
         user_opt: curve.FitOptions,
-        curve_data: curve.CurveData,
+        curve_data: curve.ScatterTable,
     ) -> Union[curve.FitOptions, List[curve.FitOptions]]:
         """Create algorithmic initial fit guess from analysis options and curve data.
 
         Args:
             user_opt: Fit options filled with user provided guess and bounds.
             curve_data: Formatted data collection to fit.
 
@@ -94,21 +94,21 @@
             )
         return user_opt
 
     def _evaluate_quality(self, fit_data: curve.CurveFitResult) -> Union[str, None]:
         """Algorithmic criteria for whether the fit is good or bad.
 
         A good fit has:
-            - a reduced chi-squared lower than three
+            - a reduced chi-squared lower than three and greater than zero
             - tau error is less than its value
         """
         tau = fit_data.ufloat_params["tau"]
 
         criteria = [
-            fit_data.reduced_chisq < 3,
+            0 < fit_data.reduced_chisq < 3,
             curve.utils.is_error_not_significant(tau),
         ]
 
         if all(criteria):
             return "good"
 
         return "bad"
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/standard_analysis/error_amplification_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/standard_analysis/error_amplification_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         default_options.max_good_angle_error = np.pi / 2
 
         return default_options
 
     def _generate_fit_guesses(
         self,
         user_opt: curve.FitOptions,
-        curve_data: curve.CurveData,
+        curve_data: curve.ScatterTable,
     ) -> Union[curve.FitOptions, List[curve.FitOptions]]:
         """Create algorithmic initial fit guess from analysis options and curve data.
 
         Args:
             user_opt: Fit options filled with user provided guess and bounds.
             curve_data: Formatted data collection to fit.
 
@@ -181,22 +181,22 @@
 
         return options
 
     def _evaluate_quality(self, fit_data: curve.CurveFitResult) -> Union[str, None]:
         """Algorithmic criteria for whether the fit is good or bad.
 
         A good fit has:
-            - a reduced chi-squared lower than three,
+            - a reduced chi-squared lower than three and greater than zero,
             - a measured angle error that is smaller than the allowed maximum good angle error.
               This quantity is set in the analysis options.
         """
         fit_d_theta = fit_data.ufloat_params["d_theta"]
 
         criteria = [
-            fit_data.reduced_chisq < 3,
+            0 < fit_data.reduced_chisq < 3,
             abs(fit_d_theta.nominal_value) < abs(self.options.max_good_angle_error),
         ]
 
         if all(criteria):
             return "good"
 
         return "bad"
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/standard_analysis/gaussian.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/standard_analysis/gaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         options.result_parameters = [curve.ParameterRepr("freq", "f01", "Hz")]
         options.normalization = True
         return options
 
     def _generate_fit_guesses(
         self,
         user_opt: curve.FitOptions,
-        curve_data: curve.CurveData,
+        curve_data: curve.ScatterTable,
     ) -> Union[curve.FitOptions, List[curve.FitOptions]]:
         """Create algorithmic initial fit guess from analysis options and curve data.
 
         Args:
             user_opt: Fit options filled with user provided guess and bounds.
             curve_data: Formatted data collection to fit.
 
@@ -122,15 +122,15 @@
 
         return user_opt
 
     def _evaluate_quality(self, fit_data: curve.CurveFitResult) -> Union[str, None]:
         """Algorithmic criteria for whether the fit is good or bad.
 
         A good fit has:
-            - a reduced chi-squared less than 3,
+            - a reduced chi-squared less than 3 and greater than zero,
             - a peak within the scanned frequency range,
             - a standard deviation that is not larger than the scanned frequency range,
             - a standard deviation that is wider than the smallest frequency increment,
             - a signal-to-noise ratio, defined as the amplitude of the peak divided by the
               square root of the median y-value less the fit offset, greater than a
               threshold of two, and
             - a standard error on the sigma of the Gaussian that is smaller than the sigma.
@@ -145,15 +145,15 @@
         snr = abs(fit_a.n) / np.sqrt(abs(np.median(fit_data.y_data) - fit_b.n))
         fit_width_ratio = fit_sigma.n / np.ptp(fit_data.x_data)
 
         criteria = [
             fit_data.x_range[0] <= fit_freq.n <= fit_data.x_range[1],
             1.5 * freq_increment < fit_sigma.n,
             fit_width_ratio < 0.25,
-            fit_data.reduced_chisq < 3,
+            0 < fit_data.reduced_chisq < 3,
             curve.utils.is_error_not_significant(fit_sigma),
             snr > 2,
         ]
 
         if all(criteria):
             return "good"
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/standard_analysis/oscillation.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/standard_analysis/oscillation.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 from typing import List, Union, Optional
 
 import lmfit
 import numpy as np
 
 import qiskit_experiments.curve_analysis as curve
-from qiskit_experiments.warnings import deprecated_class
 
 
 class OscillationAnalysis(curve.CurveAnalysis):
     r"""Oscillation analysis class based on a fit of the data to a cosine function.
 
     # section: fit_model
 
@@ -69,15 +68,15 @@
             ],
             name=name,
         )
 
     def _generate_fit_guesses(
         self,
         user_opt: curve.FitOptions,
-        curve_data: curve.CurveData,
+        curve_data: curve.ScatterTable,
     ) -> Union[curve.FitOptions, List[curve.FitOptions]]:
         """Create algorithmic initial fit guess from analysis options and curve data.
 
         Args:
             user_opt: Fit options filled with user provided guess and bounds.
             curve_data: Formatted data collection to fit.
 
@@ -108,23 +107,23 @@
 
         return options
 
     def _evaluate_quality(self, fit_data: curve.CurveFitResult) -> Union[str, None]:
         """Algorithmic criteria for whether the fit is good or bad.
 
         A good fit has:
-            - a reduced chi-squared lower than three,
+            - a reduced chi-squared lower than three and greater than zero,
             - more than a quarter of a full period,
             - less than 10 full periods, and
             - an error on the fit frequency lower than the fit frequency.
         """
         fit_freq = fit_data.ufloat_params["freq"]
 
         criteria = [
-            fit_data.reduced_chisq < 3,
+            0 < fit_data.reduced_chisq < 3,
             1.0 / 4.0 < fit_freq.nominal_value < 10.0,
             curve.utils.is_error_not_significant(fit_freq),
         ]
 
         if all(criteria):
             return "good"
 
@@ -186,15 +185,15 @@
             ],
             name=name,
         )
 
     def _generate_fit_guesses(
         self,
         user_opt: curve.FitOptions,
-        curve_data: curve.CurveData,
+        curve_data: curve.ScatterTable,
     ) -> Union[curve.FitOptions, List[curve.FitOptions]]:
         """Create algorithmic initial fit guess from analysis options and curve data.
 
         Args:
             user_opt: Fit options filled with user provided guess and bounds.
             curve_data: Formatted data collection to fit.
 
@@ -257,31 +256,24 @@
 
         return options
 
     def _evaluate_quality(self, fit_data: curve.CurveFitResult) -> Union[str, None]:
         """Algorithmic criteria for whether the fit is good or bad.
 
         A good fit has:
-            - a reduced chi-squared lower than three
+            - a reduced chi-squared lower than three and greater than zero
             - relative error of tau is less than its value
             - relative error of freq is less than its value
         """
         tau = fit_data.ufloat_params["tau"]
         freq = fit_data.ufloat_params["freq"]
 
         criteria = [
-            fit_data.reduced_chisq < 3,
+            0 < fit_data.reduced_chisq < 3,
             curve.utils.is_error_not_significant(tau),
             curve.utils.is_error_not_significant(freq),
         ]
 
         if all(criteria):
             return "good"
 
         return "bad"
-
-
-@deprecated_class("0.5", new_cls=DampedOscillationAnalysis)
-class DumpedOscillationAnalysis:
-    """Deprecated."""
-
-    pass
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/standard_analysis/resonance.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/standard_analysis/resonance.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         options.result_parameters = [curve.ParameterRepr("freq", "f01", "Hz")]
         options.normalization = True
         return options
 
     def _generate_fit_guesses(
         self,
         user_opt: curve.FitOptions,
-        curve_data: curve.CurveData,
+        curve_data: curve.ScatterTable,
     ) -> Union[curve.FitOptions, List[curve.FitOptions]]:
         """Create algorithmic initial fit guess from analysis options and curve data.
 
         Args:
             user_opt: Fit options filled with user provided guess and bounds.
             curve_data: Formatted data collection to fit.
 
@@ -122,15 +122,15 @@
 
         return user_opt
 
     def _evaluate_quality(self, fit_data: curve.CurveFitResult) -> Union[str, None]:
         """Algorithmic criteria for whether the fit is good or bad.
 
         A good fit has:
-            - a reduced chi-squared less than 3,
+            - a reduced chi-squared less than 3 and greater than zero,
             - a peak within the scanned frequency range,
             - a standard deviation that is not larger than the scanned frequency range,
             - a standard deviation that is wider than the smallest frequency increment,
             - a signal-to-noise ratio, defined as the amplitude of the peak divided by the
               square root of the median y-value less the fit offset, greater than a
               threshold of two, and
             - a standard error on the kappa of the Lorentzian that is smaller than the kappa.
@@ -145,15 +145,15 @@
         snr = abs(fit_a.n) / np.sqrt(abs(np.median(fit_data.y_data) - fit_b.n))
         fit_width_ratio = fit_kappa.n / np.ptp(fit_data.x_data)
 
         criteria = [
             fit_data.x_range[0] <= fit_freq.n <= fit_data.x_range[1],
             1.5 * freq_increment < fit_kappa.n,
             fit_width_ratio < 0.25,
-            fit_data.reduced_chisq < 3,
+            0 < fit_data.reduced_chisq < 3,
             curve.utils.is_error_not_significant(fit_kappa),
             snr > 2,
         ]
 
         if all(criteria):
             return "good"
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/utils.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 from typing import Union, Optional, List, Dict, Tuple, Callable
 import time
 
 import asteval
 import lmfit
 import numpy as np
+import pandas as pd
+from qiskit.utils.deprecation import deprecate_func
 from qiskit.utils import detach_prefix
 from uncertainties import UFloat, wrap as wrap_function
 from uncertainties import unumpy
 
 from qiskit_experiments.curve_analysis.curve_data import CurveFitResult
 from qiskit_experiments.exceptions import AnalysisError, QiskitError
 from qiskit_experiments.framework import AnalysisResultData
@@ -218,14 +220,112 @@
             # This falls into normal derivative computation.
             pass
 
     wrapfunc = np.vectorize(wrap_function(model.func))
     return wrapfunc(x=x, **sub_params)
 
 
+def shot_weighted_average(
+    yvals: np.ndarray,
+    yerrs: np.ndarray,
+    shots: np.ndarray,
+) -> Tuple[float, float, float]:
+    """Compute shot based variance and weighted average of the categorized data frame.
+
+    Sample is weighted by the shot number.
+
+    Args:
+        yvals: Y values to average.
+        yerrs: Y errors to average.
+        shots: Number of shots used to obtain Y value and error.
+
+    Returns:
+        Averaged Y value, Y error, and total shots.
+    """
+    if len(yvals) == 1:
+        return yvals[0], yerrs[0], shots[0]
+
+    if any(s is pd.NA for s in shots):
+        # Shot number is unknown
+        return np.mean(yvals), np.nan, pd.NA
+
+    total_shots = np.sum(shots)
+    weights = shots / total_shots
+
+    avg_yval = np.sum(weights * yvals)
+    avg_yerr = np.sqrt(np.sum(weights**2 * yerrs**2))
+
+    return avg_yval, avg_yerr, total_shots
+
+
+def inverse_weighted_variance(
+    yvals: np.ndarray,
+    yerrs: np.ndarray,
+    shots: np.ndarray,
+) -> Tuple[float, float, int]:
+    """Compute inverse weighted variance and weighted average of the categorized data frame.
+
+    Sample is weighted by the inverse of the data variance.
+
+    Args:
+        yvals: Y values to average.
+        yerrs: Y errors to average.
+        shots: Number of shots used to obtain Y value and error.
+
+    Returns:
+        Averaged Y value, Y error, and total shots.
+    """
+    if len(yvals) == 1:
+        return yvals[0], yerrs[0], shots[0]
+
+    total_shots = np.sum(shots)
+    weights = 1 / yerrs**2
+    yvar = 1 / np.sum(weights)
+
+    avg_yval = yvar * np.sum(weights * yvals)
+    avg_yerr = np.sqrt(yvar)
+
+    return avg_yval, avg_yerr, total_shots
+
+
+# pylint: disable=unused-argument
+def sample_average(
+    yvals: np.ndarray,
+    yerrs: np.ndarray,
+    shots: np.ndarray,
+) -> Tuple[float, float, int]:
+    """Compute sample based variance and average of the categorized data frame.
+
+    Original variance of the data is ignored and variance is computed with the y values.
+
+    Args:
+        yvals: Y values to average.
+        yerrs: Y errors to average (ignored).
+        shots: Number of shots used to obtain Y value and error.
+
+    Returns:
+        Averaged Y value, Y error, and total shots.
+    """
+    if len(yvals) == 1:
+        return yvals[0], 0.0, shots[0]
+
+    total_shots = np.sum(shots)
+
+    avg_yval = np.mean(yvals)
+    avg_yerr = np.sqrt(np.mean((avg_yval - yvals) ** 2) / len(yvals))
+
+    return avg_yval, avg_yerr, total_shots
+
+
+@deprecate_func(
+    since="0.6",
+    additional_msg="The curve data representation has been replaced by the `DataFrame` format.",
+    package_name="qiskit-experiments",
+    pending=True,
+)
 def filter_data(data: List[Dict[str, any]], **filters) -> List[Dict[str, any]]:
     """Return the list of filtered data
 
     Args:
         data: list of data dicts.
         filters: kwargs for filtering based on metadata
                  values.
@@ -245,14 +345,20 @@
                 include = False
                 break
         if include:
             filtered_data.append(datum)
     return filtered_data
 
 
+@deprecate_func(
+    since="0.6",
+    additional_msg="The curve data representation has been replaced by the `DataFrame` format.",
+    package_name="qiskit-experiments",
+    pending=True,
+)
 def mean_xy_data(
     xdata: np.ndarray,
     ydata: np.ndarray,
     sigma: Optional[np.ndarray] = None,
     shots: Optional[np.ndarray] = None,
     method: str = "sample",
 ) -> Tuple[np.ndarray, ...]:
@@ -365,14 +471,20 @@
 
         return x_means, y_means, y_sigmas, y_shots
 
     # Invalid method
     raise QiskitError(f"Unsupported method {method}")
 
 
+@deprecate_func(
+    since="0.6",
+    additional_msg="The curve data representation has been replaced by the `DataFrame` format.",
+    package_name="qiskit-experiments",
+    pending=True,
+)
 def multi_mean_xy_data(
     series: np.ndarray,
     xdata: np.ndarray,
     ydata: np.ndarray,
     sigma: Optional[np.ndarray] = None,
     shots: Optional[np.ndarray] = None,
     method: str = "sample",
@@ -423,14 +535,20 @@
         np.concatenate(xdata_means),
         np.concatenate(ydata_means),
         np.concatenate(sigma_means),
         np.concatenate(shots_sums),
     )
 
 
+@deprecate_func(
+    since="0.6",
+    additional_msg="The curve data representation has been replaced by the `DataFrame` format.",
+    package_name="qiskit-experiments",
+    pending=True,
+)
 def data_sort(
     series: np.ndarray,
     xdata: np.ndarray,
     ydata: np.ndarray,
     sigma: Optional[np.ndarray] = None,
     shots: Optional[np.ndarray] = None,
 ) -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/visualization/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/visualization/base_drawer.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/visualization/base_drawer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,19 @@
 # that they have been altered from the originals.
 
 """Curve drawer abstract class."""
 
 from abc import ABC, abstractmethod
 from typing import Dict, Optional, Sequence
 
+from qiskit.utils.deprecation import deprecate_func
+
 from qiskit_experiments.framework import Options
-from qiskit_experiments.warnings import deprecated_class
 
 
-@deprecated_class(
-    "0.6",
-    msg="Plotting and drawing of analysis figures has been moved to the new "
-    "`qiskit_experiments.visualization` module.",
-)
 class BaseCurveDrawer(ABC):
     """Abstract class for the serializable Qiskit Experiments curve drawer.
 
     A curve drawer may be implemented by different drawing backends such as matplotlib
     or plotly. Sub-classes that wrap these backends by subclassing `BaseCurveDrawer` must
     implement the following abstract methods.
 
@@ -80,14 +76,21 @@
 
         This method is called after fitting is completed and when there is valid fit outcome.
         This method is called with the list of analysis results and the reduced chi-squared values.
         The fit report should be generated to show this information on the canvas.
 
     """
 
+    @deprecate_func(
+        since="0.5",
+        additional_msg="Plotting and drawing functionality has been moved to the new "
+        "`qiskit_experiments.visualization` module.",
+        removal_timeline="after 0.6",
+        package_name="qiskit-experiments",
+    )
     def __init__(self):
         self._options = self._default_options()
         self._set_options = set()
         self._axis = None
         self._curves = []
 
     @property
@@ -244,15 +247,15 @@
         self,
         x_data: Sequence[float],
         y_ub: Sequence[float],
         y_lb: Sequence[float],
         name: Optional[str] = None,
         **options,
     ):
-        """Draw cofidence interval.
+        """Draw confidence interval.
 
         Args:
             x_data: X values.
             y_ub: The upper boundary of Y values.
             y_lb: The lower boundary of Y values.
             name: Name of this curve.
             options: Valid options for the drawer backend API.
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/visualization/curves.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/visualization/curves.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,23 +13,26 @@
 Plotting functions for experiment analysis
 """
 from typing import Callable, List, Optional, Tuple
 
 import numpy as np
 from uncertainties import unumpy as unp
 
+from qiskit.utils.deprecation import deprecate_func
+
 from qiskit_experiments.curve_analysis.curve_data import FitData
 from qiskit_experiments.framework.matplotlib import get_non_gui_ax
-from qiskit_experiments.warnings import deprecated_function
 
 
-@deprecated_function(
-    "0.6",
-    msg="Plotting and drawing functionality has been moved to the new "
+@deprecate_func(
+    since="0.5",
+    additional_msg="Plotting and drawing functionality has been moved to the new "
     "`qiskit_experiments.visualization` module.",
+    removal_timeline="after 0.6",
+    package_name="qiskit-experiments",
 )
 def plot_curve_fit(
     func: Callable,
     result: FitData,
     ax=None,
     num_fit_points: int = 100,
     labelsize: int = 14,
@@ -97,18 +100,20 @@
 
     # Formatting
     ax.tick_params(labelsize=labelsize)
     ax.grid(grid)
     return ax
 
 
-@deprecated_function(
-    "0.6",
-    msg="Plotting and drawing functionality has been moved to the new "
+@deprecate_func(
+    since="0.5",
+    additional_msg="Plotting and drawing functionality has been moved to the new "
     "`qiskit_experiments.visualization` module.",
+    removal_timeline="after 0.6",
+    package_name="qiskit-experiments",
 )
 def plot_scatter(
     xdata: np.ndarray,
     ydata: np.ndarray,
     ax=None,
     labelsize: int = 14,
     grid: bool = True,
@@ -146,18 +151,20 @@
 
     # Formatting
     ax.tick_params(labelsize=labelsize)
     ax.grid(grid)
     return ax
 
 
-@deprecated_function(
-    "0.6",
-    msg="Plotting and drawing functionality has been moved to the new "
+@deprecate_func(
+    since="0.5",
+    additional_msg="Plotting and drawing functionality has been moved to the new "
     "`qiskit_experiments.visualization` module.",
+    removal_timeline="after 0.6",
+    package_name="qiskit-experiments",
 )
 def plot_errorbar(
     xdata: np.ndarray,
     ydata: np.ndarray,
     sigma: Optional[np.ndarray] = None,
     ax=None,
     labelsize: int = 14,
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/visualization/fit_result_plotters.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/visualization/fit_result_plotters.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,32 +25,37 @@
 from enum import Enum
 from typing import Dict, List, Optional
 
 import numpy as np
 import uncertainties
 from matplotlib.ticker import FuncFormatter
 from qiskit.utils import detach_prefix
+from qiskit.utils.deprecation import deprecate_func
 
 from qiskit_experiments.curve_analysis.curve_data import CurveData, FitData, SeriesDef
 from qiskit_experiments.framework import AnalysisResultData
 from qiskit_experiments.framework.matplotlib import get_non_gui_ax
-from qiskit_experiments.warnings import deprecated_class, deprecated_function
 
 from .curves import plot_curve_fit, plot_errorbar, plot_scatter
 from .style import PlotterStyle
 
 
-@deprecated_class(
-    "0.6",
-    msg="Plotting and drawing of analysis figures has been moved to the new "
-    "`qiskit_experiments.visualization` module.",
-)
 class MplDrawSingleCanvas:
     """A plotter to draw a single canvas figure for fit result."""
 
+    @deprecate_func(
+        since="0.5",
+        additional_msg="Plotting and drawing of analysis figures has been moved to the new "
+        "`qiskit_experiments.visualization` module.",
+        removal_timeline="after 0.6",
+        package_name="qiskit-experiments",
+    )
+    def __init__(self):
+        super().__init__()
+
     @classmethod
     def draw(
         cls,
         series_defs: List[SeriesDef],
         raw_samples: List[CurveData],
         fit_samples: List[CurveData],
         tick_labels: Dict[str, str],
@@ -146,22 +151,27 @@
 
         axis.tick_params(labelsize=style.tick_label_size)
         axis.grid(True)
 
         return figure
 
 
-@deprecated_class(
-    "0.6",
-    msg="Plotting and drawing of analysis figures has been replaced with the new"
-    "`qiskit_experiments.visualization` module.",
-)
 class MplDrawMultiCanvasVstack:
     """A plotter to draw a vertically stacked multi canvas figure for fit result."""
 
+    @deprecate_func(
+        since="0.5",
+        additional_msg="Plotting and drawing of analysis figures has been moved to the new "
+        "`qiskit_experiments.visualization` module.",
+        removal_timeline="after 0.6",
+        package_name="qiskit-experiments",
+    )
+    def __init__(self):
+        pass
+
     @classmethod
     def draw(
         cls,
         series_defs: List[SeriesDef],
         raw_samples: List[CurveData],
         fit_samples: List[CurveData],
         tick_labels: Dict[str, str],
@@ -309,18 +319,20 @@
 
         axis.tick_params(labelsize=style.tick_label_size)
         axis.grid(True)
 
         return figure
 
 
-@deprecated_function(
-    "0.6",
-    msg="Plotting and drawing of analysis figures has been replaced with the new"
+@deprecate_func(
+    since="0.5",
+    additional_msg="Plotting and drawing of analysis figures has been moved to the new "
     "`qiskit_experiments.visualization` module.",
+    removal_timeline="after 0.6",
+    package_name="qiskit-experiments",
 )
 def draw_single_curve_mpl(
     axis: "matplotlib.axes.Axes",
     series_def: SeriesDef,
     raw_sample: CurveData,
     fit_sample: CurveData,
     fit_data: FitData,
@@ -367,18 +379,20 @@
             ax=axis,
             color=series_def.plot_color,
             zorder=2,
             fit_uncertainty=style.plot_sigma,
         )
 
 
-@deprecated_function(
-    "0.6",
-    msg="Plotting and drawing of analysis figures has been replaced with the new"
+@deprecate_func(
+    since="0.5",
+    additional_msg="Plotting and drawing of analysis figures has been moved to the new "
     "`qiskit_experiments.visualization` module.",
+    removal_timeline="after 0.6",
+    package_name="qiskit-experiments",
 )
 def write_fit_report(result_entries: List[AnalysisResultData]) -> str:
     """A function that generates fit reports documentation from list of data.
 
     Args:
         result_entries: List of data entries.
 
@@ -435,17 +449,22 @@
 
             analysis_description += f"{res.name} = {value_repr}\n"
 
     return analysis_description
 
 
 # pylint: disable=invalid-name
-@deprecated_class(
-    "0.6",
-    msg="Plotting and drawing of analysis figures has been moved to the new "
-    "`qiskit_experiments.visualization` module.",
-)
 class FitResultPlotters(Enum):
     """Map the plotter name to the plotters."""
 
     mpl_single_canvas = MplDrawSingleCanvas
     mpl_multiv_canvas = MplDrawMultiCanvasVstack
+
+    @deprecate_func(
+        since="0.5",
+        additional_msg="Plotting and drawing of analysis figures has been moved to the new "
+        "`qiskit_experiments.visualization` module.",
+        removal_timeline="after 0.6",
+        package_name="qiskit-experiments",
+    )
+    def __post_init__(self):
+        pass
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/curve_analysis/visualization/mpl_drawer.py` & `qiskit-experiments-0.6.0/qiskit_experiments/curve_analysis/visualization/mpl_drawer.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,32 +17,37 @@
 import numpy as np
 from matplotlib.axes import Axes
 from matplotlib.cm import tab10
 from matplotlib.figure import Figure
 from matplotlib.markers import MarkerStyle
 from matplotlib.ticker import Formatter, ScalarFormatter
 from qiskit.utils import detach_prefix
+from qiskit.utils.deprecation import deprecate_func
 
 from qiskit_experiments.framework.matplotlib import get_non_gui_ax
-from qiskit_experiments.warnings import deprecated_class
 
 from .base_drawer import BaseCurveDrawer
 
 
-@deprecated_class(
-    "0.6",
-    msg="Plotting and drawing of analysis figures has been replaced with the new"
-    "`qiskit_experiments.visualization` module.",
-)
 class MplCurveDrawer(BaseCurveDrawer):
     """Curve drawer for MatplotLib backend."""
 
     DefaultMarkers = MarkerStyle.filled_markers
     DefaultColors = tab10.colors
 
+    @deprecate_func(
+        since="0.5",
+        additional_msg="Plotting and drawing of analysis figures has been moved to the new "
+        "`qiskit_experiments.visualization` module.",
+        removal_timeline="after 0.6",
+        package_name="qiskit-experiments",
+    )
+    def __init__(self):
+        super().__init__()
+
     class PrefixFormatter(Formatter):
         """Matplotlib axis formatter to detach prefix.
 
         If a value is, e.g., x=1000.0 and the factor is 1000, then it will be shown
         as 1.0 in the ticks and its unit will be shown with the prefactor 'k'
         in the axis label.
         """
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/data_processing/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/data_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/data_processing/data_action.py` & `qiskit-experiments-0.6.0/qiskit_experiments/data_processing/data_action.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/data_processing/data_processor.py` & `qiskit-experiments-0.6.0/qiskit_experiments/data_processing/data_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,22 +44,22 @@
 
 
 class DataProcessor:
     """
     A DataProcessor defines a sequence of operations to perform on experimental data.
     Calling an instance of DataProcessor applies this sequence on the input argument.
     A DataProcessor is created with a list of DataAction instances. Each DataAction
-    applies its _process method on the data and returns the processed data. The nodes
+    applies its ``_process`` method on the data and returns the processed data. The nodes
     in the DataProcessor may also perform data validation and some minor formatting.
     The output of one data action serves as input for the next data action.
-    DataProcessor.__call__(datum) usually takes in an entry from the data property of
+    ``DataProcessor.__call__(datum)`` usually takes in an entry from the data property of
     an ExperimentData object (i.e. a dict containing metadata and memory keys and
     possibly counts, like the Result.data property) and produces the formatted data.
-    DataProcessor.__call__(datum) extracts the data from the given datum under
-    DataProcessor._input_key (which is specified at initialization) of the given datum.
+    ``DataProcessor.__call__(datum)`` extracts the data from the given datum under
+    ``DataProcessor._input_key`` (which is specified at initialization) of the given datum.
     """
 
     def __init__(
         self,
         input_key: str,
         data_actions: List[DataAction] = None,
     ):
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/data_processing/discriminator.py` & `qiskit-experiments-0.6.0/qiskit_experiments/data_processing/discriminator.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/data_processing/exceptions.py` & `qiskit-experiments-0.6.0/qiskit_experiments/data_processing/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/data_processing/nodes.py` & `qiskit-experiments-0.6.0/qiskit_experiments/data_processing/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,18 @@
         Returns:
              Arrays with one less dimension than the given data.
         """
         ax = self._axis
 
         reduced_array = np.mean(data, axis=ax)
         nominals = unp.nominal_values(reduced_array)
-        errors = unp.std_devs(reduced_array)
+        with np.errstate(invalid="ignore"):
+            # Setting std_devs to NaN will trigger floating point exceptions
+            # which we can ignore. See https://stackoverflow.com/q/75656026
+            errors = unp.std_devs(reduced_array)
 
         if np.any(np.isnan(errors)):
             # replace empty elements with SEM
             sem = np.std(unp.nominal_values(data), axis=ax) / np.sqrt(data.shape[ax])
             errors = np.where(np.isnan(errors), sem, errors)
 
         return unp.uarray(nominals, errors)
@@ -733,17 +736,17 @@
         alpha_prior: Union[float, Sequence[float]] = 0.5,
         validate: bool = True,
     ):
         """Initialize a counts to probability data conversion.
 
         Args:
             outcome: The bitstring for which to return the probability and variance.
-            alpha_prior: A prior Beta distribution parameter ``[`alpha0, alpha1]``.
+            alpha_prior: A prior Beta distribution parameter ``[alpha0, alpha1]``.
                          If specified as float this will use the same value for
-                         ``alpha0`` and``alpha1`` (Default: 0.5).
+                         ``alpha0`` and ``alpha1`` (Default: 0.5).
             validate: If set to False the DataAction will not validate its input.
 
         Raises:
             DataProcessorError: When the dimension of the prior and expected parameter vector
                 do not match.
         """
         self._outcome = outcome
@@ -777,15 +780,18 @@
             freq = counts_dict.get(self._outcome, 0)
             alpha_posterior = [freq + self._alpha_prior[0], shots - freq + self._alpha_prior[1]]
             alpha_sum = sum(alpha_posterior)
 
             p_mean = alpha_posterior[0] / alpha_sum
             p_var = p_mean * (1 - p_mean) / (alpha_sum + 1)
 
-            probabilities[idx] = ufloat(nominal_value=p_mean, std_dev=np.sqrt(p_var))
+            with np.errstate(invalid="ignore"):
+                # Setting std_devs to NaN will trigger floating point exceptions
+                # which we can ignore. See https://stackoverflow.com/q/75656026
+                probabilities[idx] = ufloat(nominal_value=p_mean, std_dev=np.sqrt(p_var))
 
         return probabilities
 
     def __repr__(self):
         """String representation of the node."""
         options_str = ", ".join(
             [
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/data_processing/processor_library.py` & `qiskit-experiments-0.6.0/qiskit_experiments/data_processing/processor_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,16 +113,16 @@
         job_meta = metadata.pop("job_metadata")
         run_options = job_meta[-1].get("run_options", {})
         for opt in ["meas_level", "meas_return"]:
             if opt in run_options:
                 metadata[opt] = run_options[opt]
         warnings.warn(
             "The analyzed ExperimentData contains deprecated data processor "
-            " job_metadata which has been been updated to current metadat format. "
-            "If this data was loaded from a database servide you should re-save it "
+            " job_metadata which has been been updated to current metadata format. "
+            "If this data was loaded from a database service you should re-save it "
             "to update the metadata in the database.",
             DeprecationWarning,
         )
 
     meas_level = metadata.get("meas_level", MeasLevel.CLASSIFIED)
     meas_return = metadata.get("meas_return", MeasReturnType.AVERAGE)
     normalize = analysis_options.get("normalization", True)
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/data_processing/sklearn_discriminators.py` & `qiskit-experiments-0.6.0/qiskit_experiments/data_processing/sklearn_discriminators.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/database_service/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/database_service/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,20 +16,32 @@
 =============================================================
 
 .. currentmodule:: qiskit_experiments.database_service
 
 This subpackage provides database-specific utility functions and exceptions which
 are used with the :class:`.ExperimentData` and :class:`.AnalysisResult` classes.
 
+Device Components
+=================
+
+.. autosummary::
+   :toctree: ../stubs/
+
+   DeviceComponent
+   Qubit
+   Resonator
+   UnknownComponent
+   to_component
 
 Exceptions
 ==========
 
 .. autosummary::
    :toctree: ../stubs/
 
    ExperimentDataError
    ExperimentEntryExists
    ExperimentEntryNotFound
 """
 
 from .exceptions import ExperimentDataError, ExperimentEntryExists, ExperimentEntryNotFound
+from .device_component import DeviceComponent, Qubit, Resonator, UnknownComponent, to_component
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/database_service/device_component.py` & `qiskit-experiments-0.6.0/qiskit_experiments/database_service/device_component.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
 """Device component classes."""
 
 from abc import ABC, abstractmethod
 
 
 class DeviceComponent(ABC):
-    """Class representing a device component."""
+    """Abstract class representing a device component. Custom components should be subclassed from
+    this class."""
 
     @abstractmethod
     def __str__(self):
         pass
 
     def __repr__(self):
         return f"<{self.__class__.__name__}({str(self)})>"
@@ -29,60 +30,61 @@
         return str(self) == str(value)
 
 
 class Qubit(DeviceComponent):
     """Class representing a qubit device component."""
 
     def __init__(self, index: int):
-        self._index = index
+        self.index = index
 
     def __str__(self):
-        return f"Q{self._index}"
+        return f"Q{self.index}"
 
     def __json_encode__(self):
-        return {"index": self._index}
+        return {"index": self.index}
 
 
 class Resonator(DeviceComponent):
     """Class representing a resonator device component."""
 
     def __init__(self, index: int):
-        self._index = index
+        self.index = index
 
     def __str__(self):
-        return f"R{self._index}"
+        return f"R{self.index}"
 
     def __json_encode__(self):
-        return {"index": self._index}
+        return {"index": self.index}
 
 
 class UnknownComponent(DeviceComponent):
-    """Class representing unknown device component."""
+    """Class representing an unknown device component."""
 
     def __init__(self, component: str):
-        self._component = component
+        self.component = component
 
     def __str__(self):
-        return self._component
+        return self.component
 
     def __json_encode__(self):
-        return {"component": self._component}
+        return {"component": self.component}
 
 
 def to_component(string: str) -> DeviceComponent:
-    """Convert the input string to a ``DeviceComponent`` instance.
+    """Convert the input string to a :class:`.DeviceComponent` instance.
 
     Args:
         string: String to be converted.
 
     Returns:
-        A ``DeviceComponent`` instance.
+        A :class:`.DeviceComponent` instance.
 
     Raises:
         ValueError: If input string is not a valid device component.
     """
+    if isinstance(string, DeviceComponent):
+        return string
     if string.startswith("Q"):
         return Qubit(int(string[1:]))
-    elif string.startswith("R"):
+    if string.startswith("R"):
         return Resonator(int(string[1:]))
-    else:
-        return UnknownComponent(string)
+    return UnknownComponent(string)
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/database_service/exceptions.py` & `qiskit-experiments-0.6.0/qiskit_experiments/database_service/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,7 +27,13 @@
     pass
 
 
 class ExperimentEntryExists(ExperimentDataError):
     """Errors raised when an experiment entry already exists."""
 
     pass
+
+
+class ExperimentDataSaveFailed(ExperimentDataError):
+    """Errors raised when an experiment save fails."""
+
+    pass
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/database_service/utils.py` & `qiskit-experiments-0.6.0/qiskit_experiments/database_service/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,46 +8,42 @@
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Experiment utility functions."""
 
+import importlib.metadata
 import io
+import zipfile
 import logging
 import threading
 import traceback
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from datetime import datetime, timezone
-from typing import Callable, Tuple, Dict, Any, Union, Type, Optional
+from typing import Callable, Tuple, Dict, Any, Union, Type, Optional, List, Iterator
 import json
 
 import dateutil.parser
-import pkg_resources
 from dateutil import tz
-from qiskit.version import __version__ as terra_version
 
 from qiskit_ibm_experiment import (
     IBMExperimentEntryExists,
     IBMExperimentEntryNotFound,
 )
 
 from .exceptions import ExperimentEntryNotFound, ExperimentEntryExists, ExperimentDataError
-from ..version import __version__ as experiments_version
 
 LOG = logging.getLogger(__name__)
 
 
 def qiskit_version():
     """Return the Qiskit version."""
-    try:
-        return pkg_resources.get_distribution("qiskit").version
-    except Exception:  # pylint: disable=broad-except
-        return {"qiskit-terra": terra_version, "qiskit-experiments": experiments_version}
+    return {p: importlib.metadata.distribution(p).version for p in ("qiskit", "qiskit-experiments")}
 
 
 def parse_timestamp(utc_dt: Union[datetime, str]) -> datetime:
     """Parse a UTC ``datetime`` object or string.
 
     Args:
         utc_dt: Input UTC `datetime` or string.
@@ -75,14 +71,60 @@
     Returns:
         A ``datetime`` with the local timezone.
     """
     local_dt = utc_dt.astimezone(tz.tzlocal())
     return local_dt
 
 
+def objs_to_zip(
+    filenames: List[str], objects: List[any], json_encoder: Optional[json.JSONEncoder] = None
+) -> bytes:
+    """Serialize a list of objects to JSON and pack into a zipped file buffer.
+
+    Args:
+        filenames: List of names for each serialized object inside the buffer. Names will have the
+        ``.json`` extension added.
+        objects: List of objects to be JSON serialized then zipped.
+        json_encoder: The JSON encoder to use.
+
+    Returns:
+        A bytes object containing the zipped files.
+    """
+    zip_buffer = io.BytesIO()
+
+    with zipfile.ZipFile(zip_buffer, "w", zipfile.ZIP_DEFLATED, False) as zip_file:
+        for filename, data in zip(filenames, objects):
+            zip_file.writestr(f"{filename}.json", json.dumps(data, cls=json_encoder))
+
+    zip_buffer.seek(0)
+    return zip_buffer
+
+
+def zip_to_objs(zip_bytes: bytes, json_decoder: Optional[json.JSONDecoder] = None) -> Iterator[any]:
+    """Extract objects by deserializing JSON files in a zipped buffer.
+
+    Args:
+        zip_bytes: Bytes object representing the zipped file.
+        json_decoder: The JSON decoder to use.
+
+    Returns:
+        A list of objects extracted from the zip file buffer.
+    """
+    if len(zip_bytes) == 0:  # artifact has been deleted
+        yield iter(())
+
+    zip_buffer = io.BytesIO(zip_bytes)
+
+    with zipfile.ZipFile(zip_buffer, "r") as zip_file:
+        for file_name in zip_file.namelist():
+            with zip_file.open(file_name) as file:
+                json_data = file.read().decode("utf-8")
+                yield json.loads(json_data, cls=json_decoder)
+
+
 def plot_to_svg_bytes(figure: "pyplot.Figure") -> bytes:
     """Convert a pyplot Figure to SVG in bytes.
 
     Args:
         figure: Figure to be converted
 
     Returns:
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/exceptions.py` & `qiskit-experiments-0.6.0/qiskit_experiments/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,18 +20,17 @@
 Overview
 ========
 
 The experiment framework broadly defines an experiment as the execution of one or more
 circuits on a device, and analysis of the resulting measurement data
 to return one or more derived results.
 
-The interface for running an experiment is through the *Experiment* classes,
-such as those contained in the :mod:`~qiskit_experiments.library`.
-The following pseudo-code illustrates the typical workflow in Qiskit Experiments
-for
+The interface for running an experiment is through the ``Experiment`` classes subclassed from
+:class:`.BaseExperiment`, such as those contained in the :mod:`~qiskit_experiments.library`. The
+following pseudo-code illustrates the typical workflow in Qiskit Experiments for
 
 - Initializing a new experiment
 - Running the experiment on a backend
 - Saving result to an online database (for compatible providers)
 - Viewing analysis results
 
 .. code-block:: python
@@ -83,28 +82,31 @@
     :toctree: ../stubs/
 
     ExperimentData
     ExperimentStatus
     AnalysisStatus
     AnalysisResult
     AnalysisResultData
+    AnalysisResultTable
     ExperimentConfig
     AnalysisConfig
     ExperimentEncoder
     ExperimentDecoder
+    ArtifactData
     FigureData
 
 .. _composite-experiment:
 
 Composite Experiment Classes
 ****************************
 
 .. autosummary::
     :toctree: ../stubs/
 
+    CompositeExperiment
     ParallelExperiment
     BatchExperiment
     CompositeAnalysis
 
 Base Classes
 ************
 
@@ -124,25 +126,33 @@
     BackendTiming
     RestlessMixin
 
 """
 from qiskit.providers.options import Options
 from qiskit_experiments.framework.backend_data import BackendData
 from qiskit_experiments.framework.analysis_result import AnalysisResult
-from qiskit_experiments.framework.experiment_data import (
+from qiskit_experiments.framework.status import (
     ExperimentStatus,
     AnalysisStatus,
+    AnalysisCallback,
+)
+from qiskit_experiments.framework.containers import (
+    ArtifactData,
     FigureData,
+    FigureType,
 )
 from .base_analysis import BaseAnalysis
 from .base_experiment import BaseExperiment
 from .backend_timing import BackendTiming
 from .configs import ExperimentConfig, AnalysisConfig
 from .analysis_result_data import AnalysisResultData
+from .analysis_result_table import AnalysisResultTable
 from .experiment_data import ExperimentData
 from .composite import (
     ParallelExperiment,
     BatchExperiment,
+    CompositeExperiment,
     CompositeAnalysis,
 )
 from .json import ExperimentEncoder, ExperimentDecoder
 from .restless_mixin import RestlessMixin
+from .package_deps import numpy_version
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/analysis_result.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/analysis_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,20 +205,21 @@
         result.set_data(data)
         result._created_in_db = True
         result.service = service
         return result
 
     def save(self, suppress_errors: bool = True) -> None:
         """Save this analysis result in the database.
+
         Args:
             suppress_errors: should the method catch exceptions (true) or
-            pass them on, potentially aborting the experiemnt (false)
+                pass them on, potentially aborting the experiment (false).
         Raises:
             ExperimentDataError: If the analysis result contains invalid data.
-            QiskitError: If the save to the database failed
+            QiskitError: If the save to the database failed.
         """
         if not self.service:
             LOG.warning(
                 "Analysis result cannot be saved because no experiment service is available."
             )
             return
         try:
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/analysis_result_data.py` & `qiskit-experiments-0.6.0/qiskit_experiments/test/noisy_delay_aer_simulator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,75 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2021.
+# (C) Copyright IBM 2022.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
+"""
+Temporary backend to be used to apply T2 and T1 noise.
+"""
+from typing import List
+
+from qiskit import QuantumCircuit
+from qiskit.circuit import Delay
+
+from qiskit_aer import AerSimulator
+from qiskit_aer.jobs.aerjob import AerJob
+from qiskit_aer.noise.passes import RelaxationNoisePass
+
+from qiskit_experiments.framework import BackendData
+
+
+class NoisyDelayAerBackend(AerSimulator):
+    """Backend for T1 and T2Ramsey experiments."""
+
+    def __init__(
+        self,
+        t1: List[float] = None,
+        t2: List[float] = None,
+        dt: float = None,
+        backend=None,
+        **backend_options,
+    ):
+        """configure backend noise"""
+
+        super().__init__(**backend_options)
+        self._t2 = t2 or [1e-4]
+        self._t1 = t1 or [2e-4]
+        if backend:
+            dt = BackendData(backend).dt
+        if dt is not None:
+            self._dt_unit = True
+            self._dt_factor = dt
+        else:
+            self._dt_unit = False
+            self._dt_factor = dt or 1e-9
+
+        self._op_types = [Delay]
+
+    # pylint: disable=arguments-differ
+    def run(self, run_input: List[QuantumCircuit], **run_options) -> AerJob:
+        """
+        Add noise pass to all circuits and then run the circuits.
+
+        Args:
+            run_input: List of circuit to run.
+            run_options (kwargs): additional run time backend options.
+
+        Returns:
+            AerJob: A job that contains the simulated data.
+
+        """
+        relax_pass = RelaxationNoisePass(
+            self._t1, self._t2, dt=self._dt_factor, op_types=self._op_types
+        )
+
+        noisy_circuits = []
+        for circ in run_input:
+            noisy_circuits.append(relax_pass(circ))
 
-"""Helper dataclass for constructing analysis results."""
-
-import dataclasses
-import logging
-from typing import Optional, Dict, Any, List
-
-LOG = logging.getLogger(__name__)
-
-
-@dataclasses.dataclass
-class AnalysisResultData:
-    """Dataclass for experiment analysis results"""
-
-    # TODO: move stderr and unit into custom value class
-    name: str
-    value: Any
-    chisq: Optional[float] = None
-    quality: Optional[str] = None
-    extra: Dict[str, Any] = dataclasses.field(default_factory=dict, hash=False, compare=False)
-    device_components: List = dataclasses.field(default_factory=list)
-
-    def __str__(self):
-        out = f"{self.name}:"
-        out += f"\n- value:{self.value}"
-        if self.chisq is not None:
-            out += f"\n- chisq: {self.chisq}"
-        if self.quality is not None:
-            out += f"\n- quality: {self.quality}"
-        if self.extra:
-            out += f"\n- extra: <{len(self.extra)} items>"
-        if self.device_components:
-            out += f"\n- device_components: {[str(i) for i in self.device_components]}"
-        return out
-
-    def __iter__(self):
-        """Return iterator of data fields (attr, value)"""
-        return iter((field.name, getattr(self, field.name)) for field in dataclasses.fields(self))
+        return super().run(noisy_circuits, **run_options)
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/backend_data.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/backend_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,33 +13,67 @@
 Backend data access helper class
 
 Since `BackendV1` and `BackendV2` do not share the same interface, this
 class unifies data access for various data fields.
 """
 from qiskit.providers.models import PulseBackendConfiguration
 from qiskit.providers import BackendV1, BackendV2
-from qiskit.providers.fake_provider import fake_backend, FakeBackendV2, FakeBackend
+from qiskit.providers.fake_provider import FakeBackend
+from qiskit.providers.fake_provider.fake_backend import FakeBackendV2
+from qiskit.utils.deprecation import deprecate_func
+
+try:
+    # Removed in Qiskit 1.0. Different from the other FakeBackendV2's
+    from qiskit.providers.fake_provider import QiskitFakeBackendV2
+except ImportError:
+
+    class QiskitFakeBackendV2:
+        """Dummy class for when FakeBackendV2 import fails
+
+        This class is only used in isinstance checks. If the import fails, then
+        there won't be an instance of the class either so any dummy class is
+        fine.
+        """
+
+        pass
+
+
+try:
+    # A copy of qiskit.providers.fake_provider.fake_backend.FakeBackendV2, at
+    # least as of qiskit-ibm-runtime 0.18.0 and Qiskit 1.0
+    from qiskit_ibm_runtime.fake_provider.fake_backend import FakeBackendV2 as RuntimeFakeBackendV2
+except ImportError:
+
+    class RuntimeFakeBackendV2:
+        """Dummy class for when FakeBackendV2 import fails
+
+        This class is only used in isinstance checks. If the import fails, then
+        there won't be an instance of the class either so any dummy class is
+        fine.
+        """
+
+        pass
 
 
 class BackendData:
     """Class for providing joint interface for accessing backend data"""
 
     def __init__(self, backend):
         """Inits the backend and verifies version"""
         self._backend = backend
         self._v1 = isinstance(backend, BackendV1)
         self._v2 = isinstance(backend, BackendV2)
         if self._v2:
             self._parse_additional_data()
 
     def _parse_additional_data(self):
-        # data specific parsing not done yet in qiskit-terra
+        # data specific parsing not done yet in upstream qiskit
         if hasattr(self._backend, "_conf_dict") and self._backend._conf_dict["open_pulse"]:
             if "u_channel_lo" not in self._backend._conf_dict:
-                self._backend._conf_dict["u_channel_lo"] = []  # to avoid terra bug
+                self._backend._conf_dict["u_channel_lo"] = []  # to avoid qiskit bug
             self._pulse_conf = PulseBackendConfiguration.from_dict(self._backend._conf_dict)
 
     @property
     def name(self):
         """Returns the backend name"""
         if self._v1:
             return self._backend.name()
@@ -142,18 +176,15 @@
     @property
     def acquire_alignment(self):
         """Returns the backend's time constraint acquire alignment"""
         try:
             if self._v1:
                 return self._backend.configuration().timing_constraints.get("acquire_alignment", 1)
             elif self._v2:
-                # currently has a typo in terra
-                if hasattr(self._backend.target, "acquire_alignment"):
-                    return self._backend.target.acquire_alignment
-                return self._backend.target.aquire_alignment
+                return self._backend.target.acquire_alignment
         except AttributeError:
             return 1
         return 1
 
     @property
     def dt(self):
         """Returns the backend's input time resolution"""
@@ -221,15 +252,15 @@
 
     @property
     def meas_freqs(self):
         """Returns the backend's measurement stimulus frequencies.
 
         .. note::
 
-            The qiskit-terra base classes do not provide this information as a
+            The qiskit base classes do not provide this information as a
             standard backend property, but it is available from some providers
             in the data returned by the ``Backend.defaults()`` method.
         """
         if not hasattr(self._backend, "defaults"):
             return []
         return getattr(self._backend.defaults(), "meas_freq_est", [])
 
@@ -240,29 +271,41 @@
             return self._backend.configuration().num_qubits
         elif self._v2:
             # meas_freq_est is currently not part of the BackendV2
             return self._backend.num_qubits
         return None
 
     @property
+    @deprecate_func(
+        is_property=True,
+        since="0.6",
+        additional_msg=(
+            "is_simulator is deprecated because BackendV2 does not provide a "
+            "standard way for checking this property. Calling code must "
+            "determine if a backend uses a simulator from context."
+        ),
+        package_name="qiskit-experiments",
+    )  # Note: remove all FakeBackend imports when removing this code
     def is_simulator(self):
         """Returns True given an indication the backend is a simulator
 
         .. note::
 
             For `BackendV2` we sometimes cannot be sure, because it lacks
             a `simulator` field, as was present in `BackendV1`'s configuration.
             We still check whether the backend inherits `FakeBackendV2`, for
-            either of its existing implementations in Terra.
+            either of its existing implementations in Qiskit.
         """
         if self._v1:
             if self._backend.configuration().simulator or isinstance(self._backend, FakeBackend):
                 return True
         if self._v2:
-            if isinstance(self._backend, (FakeBackendV2, fake_backend.FakeBackendV2)):
+            if isinstance(
+                self._backend, (FakeBackendV2, QiskitFakeBackendV2, RuntimeFakeBackendV2)
+            ):
                 return True
 
         return False
 
     def qubit_t1(self, qubit: int) -> float:
         """Return the T1 value for a qubit from the backend properties
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/backend_timing.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/backend_timing.py`

 * *Files 6% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
         from qiskit import pulse
         from qiskit.circuit import Gate, Parameter
 
 
         def circuits(self):
             chan = pulse.DriveChannel(0)
-            dur = Paramater("duration")
+            dur = Parameter("duration")
 
             with pulse.build() as sched:
                 pulse.play(pulse.Gaussian(duration=dur, amp=1, sigma=dur / 4), chan)
 
             gate = Gate("Rabi", num_qubits=1, params=[dur])
 
             template_circ = QuantumCircuit(1, 1)
@@ -176,29 +176,54 @@
                 # Track corresponding duration for the pulse in seconds
                 circ.metadata = {
                     "xval": timing.pulse_time(time=duration),
                     "unit": "s",
                 }
     """
 
-    def __init__(self, backend: Backend):
+    def __init__(
+        self,
+        backend: Backend,
+        *,
+        acquire_alignment: Optional[int] = None,
+        granularity: Optional[int] = None,
+        min_length: Optional[int] = None,
+        pulse_alignment: Optional[int] = None,
+        dt: Optional[float] = None,
+    ):
         """Initialize backend timing object
 
+        .. note::
+            Backend may not accept user defined constraint value.
+            One may want to provide these values when the constraints data is missing in the backend,
+            or in some situation you can intentionally ignore the constraints.
+            Invalid constraint values may break experiment circuits, resulting in the
+            failure in or unexpected results from the execution.
+
         Args:
-            experiment: the experiment to provide timing help for
+            backend: the backend to provide timing help for.
+            acquire_alignment: Optional. Constraint for the acquisition instruction alignment
+                in units of dt. Default to the backend value.
+            granularity: Optional. Constraint for the pulse samples granularity
+                in units of dt. Defaults to the backend value.
+            min_length: Optional. Constraint for the minimum pulse samples
+                in units of dt. Defaults to the backend value.
+            pulse_alignment: Optional. Constraint for the pulse play instruction alignment
+                in units of dt. Default to the backend value.
+            dt: Optional. Time interval of pulse samples. Default to the backend value.
         """
         backend_data = BackendData(backend)
 
         # Pull all the timing data from the backend
-        self._acquire_alignment = backend_data.acquire_alignment
-        self._granularity = backend_data.granularity
-        self._min_length = backend_data.min_length
-        self._pulse_alignment = backend_data.pulse_alignment
+        self._acquire_alignment = acquire_alignment or backend_data.acquire_alignment
+        self._granularity = granularity or backend_data.granularity
+        self._min_length = min_length or backend_data.min_length
+        self._pulse_alignment = pulse_alignment or backend_data.pulse_alignment
         #: The backend's ``dt`` value, copied to :class:`.BackendTiming` for convenience
-        self.dt = backend_data.dt
+        self.dt = dt or backend_data.dt
 
     @property
     def delay_unit(self) -> str:
         """The delay unit for the current backend
 
         "dt" is used if dt is present in the backend configuration. Otherwise
         "s" is used.
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/base_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/base_analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,23 +11,28 @@
 # that they have been altered from the originals.
 """
 Base analysis class.
 """
 from abc import ABC, abstractmethod
 import copy
 from collections import OrderedDict
+from datetime import datetime
 from typing import List, Tuple, Union, Dict
+import warnings
+
+from dateutil import tz
 
 from qiskit_experiments.database_service.device_component import Qubit
 from qiskit_experiments.framework import Options
+from qiskit_experiments.framework.containers.artifact_data import ArtifactData
 from qiskit_experiments.framework.store_init_args import StoreInitArgs
 from qiskit_experiments.framework.experiment_data import ExperimentData
+from qiskit_experiments.framework.containers import FigureData, FigureType
 from qiskit_experiments.framework.configs import AnalysisConfig
-from qiskit_experiments.framework.analysis_result_data import AnalysisResultData
-from qiskit_experiments.framework.analysis_result import AnalysisResult
+from qiskit_experiments.framework.analysis_result_data import AnalysisResultData, as_table_element
 
 
 class BaseAnalysis(ABC, StoreInitArgs):
     """Abstract base class for analyzing Experiment data.
 
     The data produced by experiments (i.e. subclasses of BaseExperiment)
     are analyzed with subclasses of BaseAnalysis. The analysis is
@@ -119,70 +124,114 @@
         replace_results: bool = False,
         **options,
     ) -> ExperimentData:
         """Run analysis and update ExperimentData with analysis result.
 
         Args:
             experiment_data: the experiment data to analyze.
-            replace_results: If True clear any existing analysis results and
-                             figures in the experiment data and replace with
+            replace_results: If True clear any existing analysis results, figures,
+                             and artifacts in the experiment data and replace with
                              new results. See note for additional information.
             options: additional analysis options. See class documentation for
                      supported options.
 
         Returns:
-            An experiment data object containing the analysis results and figures.
+            An experiment data object containing analysis results, figures, and artifacts.
 
         Raises:
             QiskitError: If experiment_data container is not valid for analysis.
 
         .. note::
             **Updating Results**
 
-            If analysis is run with ``replace_results=True`` then any analysis results
-            and figures in the experiment data will be cleared and replaced with the
+            If analysis is run with ``replace_results=True`` then any analysis results,
+            figures, and artifacts in the experiment data will be cleared and replaced with the
             new analysis results. Saving this experiment data will replace any
             previously saved data in a database service using the same experiment ID.
 
             If analysis is run with ``replace_results=False`` and the experiment data
             being analyzed has already been saved to a database service, or already
             contains analysis results or figures, a copy with a unique experiment ID
             will be returned containing only the new analysis results and figures.
             This data can then be saved as its own experiment to a database service.
         """
         # Make a new copy of experiment data if not updating results
         if not replace_results and _requires_copy(experiment_data):
             experiment_data = experiment_data.copy()
 
-        experiment_components = self._get_experiment_components(experiment_data)
-
         # Set Analysis options
         if not options:
             analysis = self
         else:
             analysis = self.copy()
             analysis.set_options(**options)
 
-        def run_analysis(expdata):
+        def run_analysis(expdata: ExperimentData):
             # Clearing previous analysis data
             experiment_data._clear_results()
-            # making new analysis
+
+            if not expdata.data():
+                warnings.warn("ExperimentData object data is empty.\n")
+
+            # Making new analysis
             results, figures = analysis._run_analysis(expdata)
-            # Add components
-            analysis_results = [
-                analysis._format_analysis_result(
-                    result, expdata.experiment_id, experiment_components
-                )
-                for result in results
-            ]
-            # Update experiment data with analysis results
-            if analysis_results:
-                expdata.add_analysis_results(analysis_results)
+
+            if results:
+                for result in results:
+                    if isinstance(result, AnalysisResultData):
+                        # Populate missing data fields
+                        if not result.experiment_id:
+                            result.experiment_id = expdata.experiment_id
+                        if not result.experiment:
+                            result.experiment = expdata.experiment_type
+                        if not result.device_components:
+                            result.device_components = self._get_experiment_components(expdata)
+                        if not result.backend:
+                            result.backend = expdata.backend_name
+                        if not result.created_time:
+                            result.created_time = datetime.now(tz.tzlocal())
+                        if not result.run_time:
+                            result.run_time = expdata.running_time
+
+                        # To canonical kwargs to add to the analysis table.
+                        table_format = as_table_element(result)
+
+                        # Remove result_id to make sure the id is unique in the scope of the container.
+                        # This will let the container generate a unique id.
+                        del table_format["result_id"]
+
+                        expdata.add_analysis_results(**table_format)
+                    elif isinstance(result, ArtifactData):
+                        if not result.experiment_id:
+                            result.experiment_id = expdata.experiment_id
+                        if not result.device_components:
+                            result.device_components = self._get_experiment_components(expdata)
+                        if not result.experiment:
+                            result.experiment = expdata.experiment_type
+                        expdata.add_artifacts(result)
+                    else:
+                        raise TypeError(
+                            f"Invalid object type {result.__class__.__name__} for analysis results. "
+                            "This data cannot be stored in the experiment data."
+                        )
+
             if figures:
-                expdata.add_figures(figures, figure_names=self.options.figure_names)
+                figure_to_add = []
+                for figure in figures:
+                    if not isinstance(figure, FigureData):
+                        qubits_repr = "_".join(
+                            map(str, expdata.metadata.get("device_components", [])[:5])
+                        )
+                        short_id = expdata.experiment_id[:8]
+                        figure = FigureData(
+                            figure=figure,
+                            name=f"{expdata.experiment_type}_{qubits_repr}_{short_id}.svg",
+                        )
+                    figure_to_add.append(figure)
+                expdata.add_figures(figure_to_add, figure_names=self.options.figure_names)
 
         experiment_data.add_analysis_callback(run_analysis)
 
         return experiment_data
 
     def _get_experiment_components(self, experiment_data: ExperimentData):
         """Subclasses may override this method to specify the experiment components."""
@@ -191,43 +240,19 @@
                 Qubit(qubit) for qubit in experiment_data.metadata["physical_qubits"]
             ]
         else:
             experiment_components = []
 
         return experiment_components
 
-    def _format_analysis_result(self, data, experiment_id, experiment_components=None):
-        """Format run analysis result to DbAnalysisResult"""
-        device_components = []
-        if data.device_components:
-            device_components = data.device_components
-        elif experiment_components:
-            device_components = experiment_components
-
-        if isinstance(data, AnalysisResult):
-            # Update device components and experiment id
-            data.device_components = device_components
-            data.experiment_id = experiment_id
-            return data
-
-        return AnalysisResult(
-            name=data.name,
-            value=data.value,
-            device_components=device_components,
-            experiment_id=experiment_id,
-            chisq=data.chisq,
-            quality=data.quality,
-            extra=data.extra,
-        )
-
     @abstractmethod
     def _run_analysis(
         self,
         experiment_data: ExperimentData,
-    ) -> Tuple[List[AnalysisResultData], List["matplotlib.figure.Figure"]]:
+    ) -> Tuple[List[Union[AnalysisResultData, ArtifactData]], List[FigureType]]:
         """Run analysis on circuit data.
 
         Args:
             experiment_data: the experiment data to analyze.
 
         Returns:
             A pair ``(analysis_results, figures)`` where ``analysis_results``
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/base_experiment.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/base_experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,21 +24,20 @@
 from qiskit.qobj.utils import MeasLevel
 from qiskit.providers.options import Options
 from qiskit_experiments.framework import BackendData
 from qiskit_experiments.framework.store_init_args import StoreInitArgs
 from qiskit_experiments.framework.base_analysis import BaseAnalysis
 from qiskit_experiments.framework.experiment_data import ExperimentData
 from qiskit_experiments.framework.configs import ExperimentConfig
-from qiskit_experiments.warnings import deprecate_arguments
+from qiskit_experiments.database_service import Qubit
 
 
 class BaseExperiment(ABC, StoreInitArgs):
     """Abstract base class for experiments."""
 
-    @deprecate_arguments({"qubits": "physical_qubits"}, "0.5")
     def __init__(
         self,
         physical_qubits: Sequence[int],
         analysis: Optional[BaseAnalysis] = None,
         backend: Optional[Backend] = None,
         experiment_type: Optional[str] = None,
     ):
@@ -50,15 +49,15 @@
             backend: Optional, the backend to run the experiment on.
             experiment_type: Optional, the experiment type string.
 
         Raises:
             QiskitError: If qubits contains duplicates.
         """
         # Experiment identification metadata
-        self._type = experiment_type if experiment_type else type(self).__name__
+        self.experiment_type = experiment_type
 
         # Circuit parameters
         self._num_qubits = len(physical_qubits)
         self._physical_qubits = tuple(physical_qubits)
         if self._num_qubits != len(set(self._physical_qubits)):
             raise QiskitError("Duplicate qubits in physical qubits list.")
 
@@ -87,14 +86,22 @@
             self._set_backend(backend)
 
     @property
     def experiment_type(self) -> str:
         """Return experiment type."""
         return self._type
 
+    @experiment_type.setter
+    def experiment_type(self, exp_type: str) -> None:
+        """Set the type for the experiment."""
+        if exp_type is None:
+            self._type = type(self).__name__
+        else:
+            self._type = exp_type
+
     @property
     def physical_qubits(self) -> Tuple[int, ...]:
         """Return the device qubits for the experiment."""
         return self._physical_qubits
 
     @property
     def num_qubits(self) -> int:
@@ -262,28 +269,80 @@
 
         Subclasses can override this method to set any final option
         values derived from other options or attributes of the
         experiment before `_run` is called.
         """
         pass
 
-    def _run_jobs(self, circuits: List[QuantumCircuit], **run_options) -> List[Job]:
-        """Run circuits on backend as 1 or more jobs."""
+    def _max_circuits(self, backend: Backend = None):
+        """
+        Calculate the maximum number of circuits per job for the experiment.
+        """
+
+        # set backend
+        if backend is None:
+            if self.backend is None:
+                raise QiskitError("A backend must be provided.")
+            backend = self.backend
         # Get max circuits for job splitting
         max_circuits_option = getattr(self.experiment_options, "max_circuits", None)
-        max_circuits_backend = self._backend_data.max_circuits
+        max_circuits_backend = BackendData(backend).max_circuits
+
         if max_circuits_option and max_circuits_backend:
-            max_circuits = min(max_circuits_option, max_circuits_backend)
+            return min(max_circuits_option, max_circuits_backend)
         elif max_circuits_option:
-            max_circuits = max_circuits_option
+            return max_circuits_option
+        else:
+            return max_circuits_backend
+
+    def job_info(self, backend: Backend = None):
+        """
+        Get information about job distribution for the experiment on a specific
+        backend.
+
+        Args:
+            backend: Optional, the backend for which to get job distribution
+                information. If not specified, the experiment must already have a
+                set backend.
+
+        Returns:
+            dict: A dictionary containing information about job distribution.
+
+                - "Total number of circuits in the experiment": Total number of
+                  circuits in the experiment.
+
+                - "Maximum number of circuits per job": Maximum number of
+                  circuits in one job based on backend and experiment settings.
+
+                - "Total number of jobs": Number of jobs needed to run this
+                  experiment on the currently set backend.
+
+        Raises:
+            QiskitError: if backend is not specified.
+
+        """
+        max_circuits = self._max_circuits(backend)
+        total_circuits = len(self.circuits())
+
+        if max_circuits is None:
+            num_jobs = 1
         else:
-            max_circuits = max_circuits_backend
+            num_jobs = (total_circuits + max_circuits - 1) // max_circuits
+        return {
+            "Total number of circuits in the experiment": total_circuits,
+            "Maximum number of circuits per job": max_circuits,
+            "Total number of jobs": num_jobs,
+        }
+
+    def _run_jobs(self, circuits: List[QuantumCircuit], **run_options) -> List[Job]:
+        """Run circuits on backend as 1 or more jobs."""
+        max_circuits = self._max_circuits(self.backend)
 
         # Run experiment jobs
-        if max_circuits and len(circuits) > max_circuits:
+        if max_circuits and (len(circuits) > max_circuits):
             # Split jobs for backends that have a maximum job size
             job_circuits = [
                 circuits[i : i + max_circuits] for i in range(0, len(circuits), max_circuits)
             ]
         else:
             # Run as single job
             job_circuits = [circuits]
@@ -409,18 +468,21 @@
         """
         self._run_options.update_options(**fields)
         self._set_run_options = self._set_run_options.union(fields)
 
     def _metadata(self) -> Dict[str, any]:
         """Return experiment metadata for ExperimentData.
 
-        Subclasses can override this method to add custom experiment
-        metadata to the returned experiment result data.
+        By default, this assumes the experiment is running on qubits only. Subclasses can override
+        this method to add custom experiment metadata to the returned experiment result data.
         """
-        metadata = {"physical_qubits": list(self.physical_qubits)}
+        metadata = {
+            "physical_qubits": list(self.physical_qubits),
+            "device_components": list(map(Qubit, self.physical_qubits)),
+        }
         return metadata
 
     def __json_encode__(self):
         """Convert to format that can be JSON serialized"""
         return self.config()
 
     @classmethod
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/composite/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/composite/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Composite Experiments"""
 
 # Base classes
+from .composite_experiment import CompositeExperiment
 from .composite_analysis import CompositeAnalysis
 
 # Composite experiment classes
 from .parallel_experiment import ParallelExperiment
 from .batch_experiment import BatchExperiment
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/composite/batch_experiment.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/composite/batch_experiment.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # that they have been altered from the originals.
 """
 Batch Experiment class.
 """
 
 from typing import List, Optional, Dict
 from collections import OrderedDict, defaultdict
+import warnings
 
 from qiskit import QuantumCircuit
 from qiskit.providers import Job, Backend, Options
 
 from .composite_experiment import CompositeExperiment, BaseExperiment
 from .composite_analysis import CompositeAnalysis
 
@@ -42,16 +43,17 @@
     documentation for additional information.
     """
 
     def __init__(
         self,
         experiments: List[BaseExperiment],
         backend: Optional[Backend] = None,
-        flatten_results: bool = False,
+        flatten_results: bool = None,
         analysis: Optional[CompositeAnalysis] = None,
+        experiment_type: Optional[str] = None,
     ):
         """Initialize a batch experiment.
 
         Args:
             experiments: a list of experiments.
             backend: Optional, the backend to run the experiment on.
             flatten_results: If True flatten all component experiment results
@@ -60,26 +62,41 @@
                              component experiment results as a separate child
                              ExperimentData container. This kwarg is ignored
                              if the analysis kwarg is used.
             analysis: Optional, the composite analysis class to use. If not
                       provided this will be initialized automatically from the
                       supplied experiments.
         """
+        if flatten_results is None:
+            # Backward compatibility for 0.6
+            # This if-clause will be removed in 0.7 and flatten_result=True is set in arguments.
+            warnings.warn(
+                "Default value of flatten_results will be turned to True in Qiskit Experiments 0.7. "
+                "If you want child experiment data for each subset experiment, "
+                "set 'flatten_results=False' explicitly.",
+                DeprecationWarning,
+            )
+            flatten_results = False
 
         # Generate qubit map
         self._qubit_map = OrderedDict()
         logical_qubit = 0
         for expr in experiments:
             for physical_qubit in expr.physical_qubits:
                 if physical_qubit not in self._qubit_map:
                     self._qubit_map[physical_qubit] = logical_qubit
                     logical_qubit += 1
         qubits = tuple(self._qubit_map.keys())
         super().__init__(
-            experiments, qubits, backend=backend, analysis=analysis, flatten_results=flatten_results
+            experiments,
+            qubits,
+            backend=backend,
+            analysis=analysis,
+            flatten_results=flatten_results,
+            experiment_type=experiment_type,
         )
 
     def circuits(self):
         return self._batch_circuits(to_transpile=False)
 
     def _transpiled_circuits(self):
         return self._batch_circuits(to_transpile=True)
@@ -92,15 +109,15 @@
             if self.physical_qubits == expr.physical_qubits or to_transpile:
                 qubit_mapping = None
             else:
                 qubit_mapping = [self._qubit_map[qubit] for qubit in expr.physical_qubits]
 
             if isinstance(expr, BatchExperiment):
                 # Batch experiments don't contain their own native circuits.
-                # If to_trasnpile is True then the circuits will be transpiled at the non-batch
+                # If to_transpile is True then the circuits will be transpiled at the non-batch
                 # experiments.
                 # Fetch the circuits from the sub-experiments.
                 expr_circuits = expr._batch_circuits(to_transpile)
             elif to_transpile:
                 expr_circuits = expr._transpiled_circuits()
             else:
                 expr_circuits = expr.circuits()
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/composite/composite_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/composite/composite_analysis.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 """
 Composite Experiment Analysis class.
 """
 
 from typing import List, Dict, Union, Optional, Tuple
+import warnings
 import numpy as np
 from qiskit.result import marginal_distribution
 from qiskit.result.postprocess import format_counts_memory
 from qiskit_experiments.framework import BaseAnalysis, ExperimentData
 from qiskit_experiments.framework.analysis_result_data import AnalysisResultData
 from qiskit_experiments.framework.base_analysis import _requires_copy
 from qiskit_experiments.exceptions import AnalysisError
@@ -30,15 +31,15 @@
     run together in a single execution, the results of which are returned
     as a single list of circuit result data in the :class:`ExperimentData`
     container.
 
     Analysis of this composite circuit data involves constructing
     a list of experiment data containers for each component experiment containing
     the marginalized circuit result data for that experiment. These are saved as
-    :meth:.~ExperimentData.child_data` in the main :class:`.ExperimentData` container.
+    :meth:`~.ExperimentData.child_data` in the main :class:`.ExperimentData` container.
     Each component experiment data is then analyzed using the analysis class from
     the corresponding component experiment.
 
     .. note::
 
         If the composite :class:`ExperimentData` does not already contain child
         experiment data containers for the component experiments they will be
@@ -47,31 +48,51 @@
 
         When calling :meth:`~.CompositeAnalysis.run` on experiment data already
         containing initialized component experiment data, any previously stored circuit
         data will be cleared and replaced with the marginalized data from the composite
         experiment data.
     """
 
-    def __init__(self, analyses: List[BaseAnalysis], flatten_results: bool = False):
+    def __init__(
+        self,
+        analyses: List[BaseAnalysis],
+        flatten_results: bool = None,
+        generate_figures: Optional[str] = "always",
+    ):
         """Initialize a composite analysis class.
 
         Args:
             analyses: a list of component experiment analysis objects.
             flatten_results: If True flatten all component experiment results
                              into a single ExperimentData container, including
                              nested composite experiments. If False save each
                              component experiment results as a separate child
                              ExperimentData container.
+            generate_figures: Optional flag to set the figure generation behavior.
+                If ``always``, figures are always generated. If ``never``, figures are never generated.
+                If ``selective``, figures are generated if the analysis ``quality`` is ``bad``.
         """
+        if flatten_results is None:
+            # Backward compatibility for 0.6
+            # This if-clause will be removed in 0.7 and flatten_result=True is set in arguments.
+            warnings.warn(
+                "Default value of flatten_results will be turned to True in Qiskit Experiments 0.7. "
+                "If you want child experiment data for each subset experiment, "
+                "set 'flatten_results=False' explicitly.",
+                DeprecationWarning,
+            )
+            flatten_results = False
         super().__init__()
         self._analyses = analyses
         self._flatten_results = False
         if flatten_results:
             self._set_flatten_results()
 
+        self._set_generate_figures(generate_figures)
+
     def component_analysis(
         self, index: Optional[int] = None
     ) -> Union[BaseAnalysis, List[BaseAnalysis]]:
         """Return the component experiment Analysis instance.
 
         Args:
             index: Optional, the component index to return analysis for.
@@ -81,14 +102,22 @@
             The analysis instance for the specified index, or a list of all
             analysis instances if index is None.
         """
         if index is None:
             return self._analyses
         return self._analyses[index]
 
+    def set_options(self, **fields):
+        """Set the analysis options for the experiment. If the `broadcast` argument set to `True`, the
+        analysis options will cascade to the child experiments."""
+        super().set_options(**fields)
+        if fields.get("broadcast", None):
+            for sub_analysis in self._analyses:
+                sub_analysis.set_options(**fields)
+
     def copy(self):
         ret = super().copy()
         # Recursively copy analysis
         ret._analyses = [analysis.copy() for analysis in ret._analyses]
         return ret
 
     def run(
@@ -98,15 +127,15 @@
         **options,
     ) -> ExperimentData:
         # Make a new copy of experiment data if not updating results
         if not replace_results and _requires_copy(experiment_data):
             experiment_data = experiment_data.copy()
 
         if not self._flatten_results:
-            # Initialize child components if they are not initalized
+            # Initialize child components if they are not initialized
             # This only needs to be done if results are not being flattened
             self._add_child_data(experiment_data)
 
         # Run analysis with replace_results = True since we have already
         # created the copy if it was required
         return super().run(experiment_data, replace_results=True, **options)
 
@@ -125,23 +154,26 @@
         # for all component analysis to finish before returning
         # the parent experiment analysis results
         for sub_expdata in component_expdata:
             sub_expdata.block_for_results()
         # Optionally flatten results from all component experiments
         # for adding to the main experiment data container
         if self._flatten_results:
-            return self._combine_results(component_expdata)
-
+            analysis_results, figures = self._combine_results(component_expdata)
+            for res in analysis_results:
+                # Override experiment  ID because entries are flattened
+                res.experiment_id = experiment_data.experiment_id
+            return analysis_results, figures
         return [], []
 
     def _component_experiment_data(self, experiment_data: ExperimentData) -> List[ExperimentData]:
         """Return a list of marginalized experiment data for component experiments.
 
         Args:
-            experiment_data: a composite experiment experiment data container.
+            experiment_data: a composite experiment data container.
 
         Returns:
             The list of analysis-ready marginalized experiment data for each
             component experiment.
 
         Raises:
             AnalysisError: If the component experiment data cannot be extracted.
@@ -199,24 +231,24 @@
             # Pre-process the memory if any to avoid redundant calls to format_counts_memory
             f_memory = self._format_memory(datum, composite_clbits)
 
             for i, index in enumerate(metadata["composite_index"]):
                 if index not in marginalized_data:
                     # Initialize data list for marginalized
                     marginalized_data[index] = []
-                sub_data = {"metadata": metadata["composite_metadata"][i]}
+                sub_data = {
+                    k: v for k, v in datum.items() if k not in ("metadata", "counts", "memory")
+                }
+                sub_data["metadata"] = metadata["composite_metadata"][i]
                 if "counts" in datum:
                     if composite_clbits is not None:
-                        # `marginal_distribution() doesn't support int64 values
-                        # so detect and cast to an int. This can be removed
-                        # when Qiskit/qiskit-terra#9976 is released
-                        counts = datum["counts"]
-                        if any(isinstance(x, np.integer) for x in counts.values()):
-                            counts = {k: int(v) for k, v in counts.items()}
-                        sub_data["counts"] = marginal_distribution(counts, composite_clbits[i])
+                        sub_data["counts"] = marginal_distribution(
+                            counts=datum["counts"],
+                            indices=composite_clbits[i],
+                        )
                     else:
                         sub_data["counts"] = datum["counts"]
                 if "memory" in datum:
                     if composite_clbits is not None:
                         # level 2
                         if f_memory is not None:
                             idx = slice(
@@ -327,35 +359,54 @@
     def _set_flatten_results(self):
         """Recursively set flatten_results to True for all composite components."""
         self._flatten_results = True
         for analysis in self._analyses:
             if isinstance(analysis, CompositeAnalysis):
                 analysis._set_flatten_results()
 
+    def _set_generate_figures(self, generate_figures):
+        """Recursively propagate ``generate_figures`` to all child experiments."""
+        self._generate_figures = generate_figures
+        for analysis in self._analyses:
+            if isinstance(analysis, CompositeAnalysis):
+                analysis._set_generate_figures(generate_figures)
+            else:
+                analysis._generate_figures = generate_figures
+
     def _combine_results(
-        self, component_experiment_data: List[ExperimentData]
+        self,
+        component_experiment_data: List[ExperimentData],
     ) -> Tuple[List[AnalysisResultData], List["matplotlib.figure.Figure"]]:
         """Combine analysis results from component experiment data.
 
         Args:
             component_experiment_data: list of experiment data containers containing the
                                        analysis results for each component experiment.
 
         Returns:
             A pair of the combined list of all analysis results from each of the
             component experiments, and a list of all figures from each component
             experiment.
         """
         analysis_results = []
         figures = []
-        for i, sub_expdata in enumerate(component_experiment_data):
+        for sub_expdata in component_experiment_data:
             figures += sub_expdata._figures.values()
-            for result in sub_expdata.analysis_results():
-                # Add metadata to distinguish the component experiment
-                # the result was generated from
-                result.extra["component_experiment"] = {
-                    "experiment_type": sub_expdata.experiment_type,
-                    "component_index": i,
-                }
-                analysis_results.append(result)
+
+            # Convert Dataframe Series back into AnalysisResultData
+            # This is due to limitation that _run_analysis must return List[AnalysisResultData],
+            # and some composite analysis such as TphiAnalysis overrides this method to
+            # return extra quantity computed from sub analysis results.
+            # This produces unnecessary data conversion.
+            # The _run_analysis mechanism seems just complicating the entire logic.
+            # Since it's impossible to deprecate the usage of this protected method,
+            # we should implement new CompositeAnalysis class with much more efficient
+            # internal logic. Note that the child data structure is no longer necessary
+            # because dataframe offers more efficient data filtering mechanisms.
+            analysis_table = sub_expdata.analysis_results(columns="all", dataframe=True)
+            for _, series in analysis_table.iterrows():
+                data = AnalysisResultData.from_table_element(**series.to_dict())
+                analysis_results.append(data)
+            for artifact in sub_expdata.artifacts():
+                analysis_results.append(artifact)
 
         return analysis_results, figures
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/composite/composite_experiment.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/composite/composite_experiment.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,31 +13,29 @@
 Composite Experiment abstract base class.
 """
 
 from typing import List, Sequence, Optional, Union
 from abc import abstractmethod
 import warnings
 from qiskit.providers.backend import Backend
-from qiskit_experiments.warnings import deprecate_arguments
 from qiskit_experiments.exceptions import QiskitError
 from qiskit_experiments.framework import BaseExperiment
 from .composite_analysis import CompositeAnalysis
 
 
 class CompositeExperiment(BaseExperiment):
     """Composite Experiment base class"""
 
-    @deprecate_arguments({"qubits": "physical_qubits"}, "0.5")
     def __init__(
         self,
         experiments: List[BaseExperiment],
         physical_qubits: Sequence[int],
         backend: Optional[Backend] = None,
         experiment_type: Optional[str] = None,
-        flatten_results: bool = False,
+        flatten_results: bool = None,
         analysis: Optional[CompositeAnalysis] = None,
     ):
         """Initialize the composite experiment object.
 
         Args:
             experiments: a list of experiment objects.
             physical_qubits: list of physical qubits for the experiment.
@@ -53,14 +51,25 @@
                       provided this will be initialized automatically from the
                       supplied experiments.
 
         Raises:
             QiskitError: If the provided analysis class is not a CompositeAnalysis
                          instance.
         """
+        if flatten_results is None:
+            # Backward compatibility for 0.6
+            # This if-clause will be removed in 0.7 and flatten_result=True is set in arguments.
+            warnings.warn(
+                "Default value of flatten_results will be turned to True in Qiskit Experiments 0.7. "
+                "If you want child experiment data for each subset experiment, "
+                "set 'flatten_results=False' explicitly.",
+                DeprecationWarning,
+            )
+            flatten_results = False
+
         self._experiments = experiments
         self._num_experiments = len(experiments)
         if analysis is None:
             analysis = CompositeAnalysis(
                 [exp.analysis for exp in self._experiments], flatten_results=flatten_results
             )
         super().__init__(
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/composite/parallel_experiment.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/composite/parallel_experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 """
 Parallel Experiment class.
 """
 from typing import List, Optional
+import warnings
 import numpy as np
 
 from qiskit import QuantumCircuit, ClassicalRegister
 from qiskit.circuit import Clbit
 from qiskit.providers.backend import Backend
 from qiskit_experiments.exceptions import QiskitError
 from .composite_experiment import CompositeExperiment, BaseExperiment
@@ -42,16 +43,17 @@
     documentation for additional information.
     """
 
     def __init__(
         self,
         experiments: List[BaseExperiment],
         backend: Optional[Backend] = None,
-        flatten_results: bool = False,
+        flatten_results: bool = None,
         analysis: Optional[CompositeAnalysis] = None,
+        experiment_type: Optional[str] = None,
     ):
         """Initialize the analysis object.
 
         Args:
             experiments: a list of experiments.
             backend: Optional, the backend to run the experiment on.
             flatten_results: If True flatten all component experiment results
@@ -60,19 +62,34 @@
                              component experiment results as a separate child
                              ExperimentData container. This kwarg is ignored
                              if the analysis kwarg is used.
             analysis: Optional, the composite analysis class to use. If not
                       provided this will be initialized automatically from the
                       supplied experiments.
         """
+        if flatten_results is None:
+            # Backward compatibility for 0.6
+            # This if-clause will be removed in 0.7 and flatten_result=True is set in arguments.
+            warnings.warn(
+                "Default value of flatten_results will be turned to True in Qiskit Experiments 0.7. "
+                "If you want child experiment data for each subset experiment, "
+                "set 'flatten_results=False' explicitly.",
+                DeprecationWarning,
+            )
+            flatten_results = False
         qubits = []
         for exp in experiments:
             qubits += exp.physical_qubits
         super().__init__(
-            experiments, qubits, backend=backend, analysis=analysis, flatten_results=flatten_results
+            experiments,
+            qubits,
+            backend=backend,
+            analysis=analysis,
+            flatten_results=flatten_results,
+            experiment_type=experiment_type,
         )
 
     def circuits(self):
         return self._combined_circuits(device_layout=False)
 
     def _transpiled_circuits(self):
         return self._combined_circuits(device_layout=True)
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/configs.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/configs.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,23 +18,20 @@
 
 from qiskit.exceptions import QiskitError
 from qiskit_experiments.version import __version__
 
 
 @dataclasses.dataclass(frozen=True)
 class ExperimentConfig:
-    """Store configuration settings for an Experiment
+    """Store configuration settings for an Experiment class.
 
-    This stores the current configuration of a
-    :class:~qiskit_experiments.framework.BaseExperiment` and
-    can be used to reconstruct the experiment using either the
-    :meth:`experiment` property if the experiment class type is
-    currently stored, or the
-    :meth:~qiskit_experiments.framework.BaseExperiment.from_config`
-    class method of the appropriate experiment.
+    This stores the current configuration of a :class:`.BaseExperiment` and can be used to
+    reconstruct the experiment using either the :meth:`experiment` property if the experiment class
+    type is currently stored, or the :meth:`~.BaseExperiment.from_config` class method of the
+    appropriate experiment.
     """
 
     cls: type = None
     args: Tuple[Any] = dataclasses.field(default_factory=tuple)
     kwargs: Dict[str, Any] = dataclasses.field(default_factory=dict)
     experiment_options: Dict[str, Any] = dataclasses.field(default_factory=dict)
     transpile_options: Dict[str, Any] = dataclasses.field(default_factory=dict)
@@ -71,23 +68,20 @@
                     " installing a compatible qiskit-experiments version."
                 )
             raise QiskitError(f"{msg}\nError Message:\n{str(ex)}") from ex
 
 
 @dataclasses.dataclass(frozen=True)
 class AnalysisConfig:
-    """Store configuration settings for Analysis
+    """Store configuration settings for an Analysis class.
 
-    This stores the current configuration of a
-    :class:~qiskit_experiments.framework.BaseAnalysis` and
-    can be used to reconstruct the analysis class using either the
-    :meth:`analysis` property if the analysis class type is
-    currently stored, or the
-    :meth:~qiskit_experiments.framework.BaseAnalysis.from_config`
-    class method of the appropriate experiment.
+    This stores the current configuration of a :class:`.BaseAnalysis` and can be used to reconstruct
+    the analysis class using either the :meth:`analysis` property if the analysis class type is
+    currently stored, or the :meth:`~.BaseAnalysis.from_config` class method of the appropriate
+    experiment.
     """
 
     cls: type = None
     args: Tuple[Any] = dataclasses.field(default_factory=tuple)
     kwargs: Dict[str, Any] = dataclasses.field(default_factory=dict)
     options: Dict[str, Any] = dataclasses.field(default_factory=dict)
     version: str = __version__
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/experiment_data.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/experiment_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,53 +11,66 @@
 # that they have been altered from the originals.
 """
 Experiment Data class
 """
 
 from __future__ import annotations
 import logging
-import dataclasses
+import re
 from typing import Dict, Optional, List, Union, Any, Callable, Tuple, TYPE_CHECKING
-from datetime import datetime
+from datetime import datetime, timezone
 from concurrent import futures
-from threading import Event
 from functools import wraps
-from collections import deque
+from collections import deque, defaultdict
 import contextlib
 import copy
 import uuid
-import enum
 import time
-import io
 import sys
+import json
 import traceback
+import warnings
 import numpy as np
+import pandas as pd
+from dateutil import tz
 from matplotlib import pyplot
-from matplotlib.figure import Figure as MatplotlibFigure
 from qiskit.result import Result
 from qiskit.providers.jobstatus import JobStatus, JOB_FINAL_STATES
 from qiskit.exceptions import QiskitError
 from qiskit.providers import Job, Backend, Provider
+from qiskit.utils.deprecation import deprecate_arg
 
-from qiskit_ibm_experiment import IBMExperimentService
-from qiskit_ibm_experiment import ExperimentData as ExperimentDataclass
+from qiskit_ibm_experiment import (
+    IBMExperimentService,
+    ExperimentData as ExperimentDataclass,
+    AnalysisResultData as AnalysisResultDataclass,
+    ResultQuality,
+)
 from qiskit_experiments.framework.json import ExperimentEncoder, ExperimentDecoder
 from qiskit_experiments.database_service.utils import (
     qiskit_version,
     plot_to_svg_bytes,
     ThreadSafeOrderedDict,
     ThreadSafeList,
 )
+from qiskit_experiments.database_service.device_component import to_component, DeviceComponent
 from qiskit_experiments.framework.analysis_result import AnalysisResult
+from qiskit_experiments.framework.analysis_result_data import AnalysisResultData
+from qiskit_experiments.framework.analysis_result_table import AnalysisResultTable
 from qiskit_experiments.framework import BackendData
+from qiskit_experiments.framework.containers import ArtifactData
+from qiskit_experiments.framework import ExperimentStatus, AnalysisStatus, AnalysisCallback
 from qiskit_experiments.database_service.exceptions import (
     ExperimentDataError,
     ExperimentEntryNotFound,
-    ExperimentEntryExists,
+    ExperimentDataSaveFailed,
 )
+from qiskit_experiments.database_service.utils import objs_to_zip, zip_to_objs
+
+from .containers.figure_data import FigureData, FigureType
 
 if TYPE_CHECKING:
     # There is a cyclical dependency here, but the name needs to exist for
     # Sphinx on Python 3.9+ to link type hints correctly.  The gating on
     # `TYPE_CHECKING` means that the import will never be resolved by an actual
     # interpreter, only static analysis.
     from . import BaseExperiment
@@ -74,90 +87,70 @@
         if self.auto_save:
             self.save_metadata()
         return return_val
 
     return _wrapped
 
 
-class FigureData:
-    """Wrapper class for figures and figure metadata. The raw figure can be accessed with
-    the ``figure`` attribute."""
-
-    def __init__(self, figure, name=None, metadata=None):
-        """Creates a new figure data object.
-
-        Args:
-            figure: the raw figure itself. Can be SVG or matplotlib.Figure.
-            name: Optional, the name of the figure.
-            metadata: Optional, any metadata to be stored with the figure."""
-        self.figure = figure
-        self._name = name
-        self.metadata = metadata or {}
-
-    # name is read only
-    @property
-    def name(self) -> str:
-        """The name of the figure"""
-        return self._name
-
-    @property
-    def metadata(self) -> dict:
-        """The metadata dictionary stored with the figure"""
-        return self._metadata
-
-    @metadata.setter
-    def metadata(self, new_metadata: dict):
-        """Set the metadata to new value; must be a dictionary"""
-        if not isinstance(new_metadata, dict):
-            raise ValueError("figure metadata must be a dictionary")
-        self._metadata = new_metadata
-
-    def copy(self, new_name: Optional[str] = None):
-        """Creates a copy of the figure data"""
-        name = new_name or self.name
-        return FigureData(figure=self.figure, name=name, metadata=copy.deepcopy(self.metadata))
-
-    def __json_encode__(self) -> Dict[str, Any]:
-        """Return the json representation of the figure data"""
-        return {"figure": self.figure, "name": self.name, "metadata": self.metadata}
+def utc_to_local(utc_dt: datetime) -> datetime:
+    """Convert input UTC timestamp to local timezone.
 
-    @classmethod
-    def __json_decode__(cls, args: Dict[str, Any]) -> "FigureData":
-        """Initialize a figure data from the json representation"""
-        return cls(**args)
-
-    def _repr_png_(self):
-        if isinstance(self.figure, MatplotlibFigure):
-            b = io.BytesIO()
-            self.figure.savefig(b, format="png", bbox_inches="tight")
-            png = b.getvalue()
-            return png
-        else:
-            return None
+    Args:
+        utc_dt: Input UTC timestamp.
+
+    Returns:
+        A ``datetime`` with the local timezone.
+    """
+    if utc_dt is None:
+        return None
+    local_dt = utc_dt.astimezone(tz.tzlocal())
+    return local_dt
+
+
+def local_to_utc(local_dt: datetime) -> datetime:
+    """Convert input local timezone timestamp to UTC timezone.
+
+    Args:
+        local_dt: Input local timestamp.
 
-    def _repr_svg_(self):
-        if isinstance(self.figure, str):
-            return self.figure
-        if isinstance(self.figure, bytes):
-            return str(self.figure)
+    Returns:
+        A ``datetime`` with the UTC timezone.
+    """
+    if local_dt is None:
         return None
+    utc_dt = local_dt.astimezone(tz.UTC)
+    return utc_dt
+
+
+def parse_utc_datetime(dt_str: str) -> datetime:
+    """Parses UTC datetime from a string"""
+    if dt_str is None:
+        return None
+
+    db_datetime_format = "%Y-%m-%dT%H:%M:%S.%fZ"
+    dt_utc = datetime.strptime(dt_str, db_datetime_format)
+    dt_utc = dt_utc.replace(tzinfo=timezone.utc)
+    return dt_utc
 
 
 class ExperimentData:
     """Experiment data container class.
 
+    .. note::
+        Saving experiment data to the cloud database is currently a limited access feature. You can
+        check whether you have access by logging into the IBM Quantum interface
+        and seeing if you can see the `database <https://quantum.ibm.com/experiments>`__.
+
     This class handles the following:
 
     1. Storing the data related to an experiment: raw data, metadata, analysis results,
        and figures
     2. Managing jobs and adding data from jobs automatically
     3. Saving and loading data from the database service
 
-    |
-
     The field ``db_data`` is a dataclass (``ExperimentDataclass``) containing
     all the data that can be stored in the database and loaded from it, and
     as such is subject to strict conventions.
 
     Other data fields can be added and used freely, but they won't be saved
     to the database.
 
@@ -166,47 +159,64 @@
     _metadata_version = 1
     _job_executor = futures.ThreadPoolExecutor()
 
     _json_encoder = ExperimentEncoder
     _json_decoder = ExperimentDecoder
 
     _metadata_filename = "metadata.json"
+    _max_workers_cap = 10
 
     def __init__(
         self,
         experiment: Optional["BaseExperiment"] = None,
         backend: Optional[Backend] = None,
         service: Optional[IBMExperimentService] = None,
+        provider: Optional[Provider] = None,
         parent_id: Optional[str] = None,
         job_ids: Optional[List[str]] = None,
         child_data: Optional[List[ExperimentData]] = None,
         verbose: Optional[bool] = True,
         db_data: Optional[ExperimentDataclass] = None,
+        start_datetime: Optional[datetime] = None,
         **kwargs,
     ):
         """Initialize experiment data.
 
         Args:
             experiment: Experiment object that generated the data.
             backend: Backend the experiment runs on. This overrides the
                 backend in the experiment object.
             service: The service that stores the experiment results to the database
+            provider: The provider used for the experiments
+                (can be used to automatically obtain the service)
             parent_id: ID of the parent experiment data
                 in the setting of a composite experiment
             job_ids: IDs of jobs submitted for the experiment.
             child_data: List of child experiment data.
             verbose: Whether to print messages.
             db_data: A prepared ExperimentDataclass of the experiment info.
                 This overrides other db parameters.
+            start_datetime: The time when the experiment started running.
+                If none, defaults to the current time.
+
+        Additional info:
+            In order to save the experiment data to the cloud service, the class
+            needs access to the experiment service provider. It can be obtained
+            via three different methods, given here by priority:
+
+            1. Passing it directly via the ``service`` parameter.
+            2. Implicitly obtaining it from the ``provider`` parameter.
+            3. Implicitly obtaining it from the ``backend`` parameter, using that backend's provider.
         """
         if experiment is not None:
             backend = backend or experiment.backend
             experiment_type = experiment.experiment_type
         else:
-            experiment_type = None
+            # Don't use None since the resultDB won't accept that
+            experiment_type = ""
         if job_ids is None:
             job_ids = []
 
         self._experiment = experiment
 
         # data stored in the database
         metadata = {}
@@ -228,52 +238,63 @@
                 experiment_type=experiment_type,
                 parent_id=parent_id,
                 job_ids=job_ids,
                 metadata=metadata,
             )
         else:
             self._db_data = db_data
-
+        if self.start_datetime is None:
+            if start_datetime is None:
+                start_datetime = datetime.now()
+            self.start_datetime = start_datetime
         for key, value in kwargs.items():
             if hasattr(self._db_data, key):
                 setattr(self._db_data, key, value)
             else:
                 LOG.warning("Key '%s' not stored in the database", key)
 
         # general data related
         self._backend = None
         if backend is not None:
             self._set_backend(backend, recursive=False)
+        self.provider = provider
+        if provider is None and backend is not None:
+            self.provider = backend.provider
         self._service = service
-        if self._service is None and self.backend is not None:
+        if self._service is None and self.provider is not None:
+            self._service = self.get_service_from_provider(self.provider)
+        if self._service is None and self.provider is None and self.backend is not None:
             self._service = self.get_service_from_backend(self.backend)
         self._auto_save = False
         self._created_in_db = False
         self._extra_data = kwargs
         self.verbose = verbose
 
         # job handling related
         self._jobs = ThreadSafeOrderedDict(job_ids)
         self._job_futures = ThreadSafeOrderedDict()
+        self._running_time = None
         self._analysis_callbacks = ThreadSafeOrderedDict()
         self._analysis_futures = ThreadSafeOrderedDict()
         # Set 2 workers for analysis executor so there can be 1 actively running
         # future and one waiting "running" future. This is to allow the second
         # future to be cancelled without waiting for the actively running future
         # to finish first.
         self._analysis_executor = futures.ThreadPoolExecutor(max_workers=2)
         self._monitor_executor = futures.ThreadPoolExecutor()
 
         # data storage
         self._result_data = ThreadSafeList()
         self._figures = ThreadSafeOrderedDict(self._db_data.figure_names)
-        self._analysis_results = ThreadSafeOrderedDict()
+        self._analysis_results = AnalysisResultTable()
+        self._artifacts = ThreadSafeOrderedDict()
 
         self._deleted_figures = deque()
         self._deleted_analysis_results = deque()
+        self._deleted_artifacts = set()  # for holding unique artifact names to be deleted
 
         # Child related
         # Add component data and set parent ID to current container
         self._child_data = ThreadSafeOrderedDict()
         if child_data is not None:
             self._set_child_data(child_data)
 
@@ -323,53 +344,77 @@
 
         Returns:
             Experiment metadata.
         """
         return self._db_data.metadata
 
     @property
-    def creation_datetime(self) -> "datetime":
+    def creation_datetime(self) -> datetime:
         """Return the creation datetime of this experiment data.
 
         Returns:
-            The creation datetime of this experiment data.
+            The timestamp when this experiment data was saved to the cloud service
+            in the local timezone.
 
         """
         return self._db_data.creation_datetime
 
     @property
-    def start_datetime(self) -> "datetime":
+    def start_datetime(self) -> datetime:
         """Return the start datetime of this experiment data.
 
         Returns:
-            The start datetime of this experiment data.
+            The timestamp when this experiment began running in the local timezone.
 
         """
         return self._db_data.start_datetime
 
+    @start_datetime.setter
+    def start_datetime(self, new_start_datetime: datetime) -> None:
+        self._db_data.start_datetime = new_start_datetime
+
     @property
-    def updated_datetime(self) -> "datetime":
+    def updated_datetime(self) -> datetime:
         """Return the update datetime of this experiment data.
 
         Returns:
-            The update datetime of this experiment data.
+            The timestamp when this experiment data was last updated in the service
+            in the local timezone.
 
         """
         return self._db_data.updated_datetime
 
     @property
-    def end_datetime(self) -> "datetime":
+    def running_time(self) -> datetime:
+        """Return the running time of this experiment data.
+
+        The running time is the time the latest successful job started running on
+        the remote quantum machine. This can change as more jobs finish.
+
+        """
+        return self._running_time
+
+    @property
+    def end_datetime(self) -> datetime:
         """Return the end datetime of this experiment data.
 
+        The end datetime is the time the latest job data was
+        added without errors; this can change as more jobs finish.
+
         Returns:
-            The end datetime of this experiment data.
+            The timestamp when the last job of this experiment finished
+            in the local timezone.
 
         """
         return self._db_data.end_datetime
 
+    @end_datetime.setter
+    def end_datetime(self, new_end_datetime: datetime) -> None:
+        self._db_data.end_datetime = new_end_datetime
+
     @property
     def hub(self) -> str:
         """Return the hub of this experiment data.
 
         Returns:
             The hub of this experiment data.
 
@@ -393,25 +438,14 @@
         Returns:
             The project of this experiment data.
 
         """
         return self._db_data.project
 
     @property
-    def _provider(self) -> Optional[Provider]:
-        """Return the provider.
-
-        Returns:
-            Provider used for the experiment, or ``None`` if unknown.
-        """
-        if self._backend is None:
-            return None
-        return self._backend.provider()
-
-    @property
     def experiment_id(self) -> str:
         """Return experiment ID
 
         Returns:
             Experiment ID.
         """
 
@@ -548,48 +582,58 @@
         self._backend_data = BackendData(new_backend)
         self._db_data.backend = self._backend_data.name
         if self._db_data.backend is None:
             self._db_data.backend = str(new_backend)
         provider = self._backend_data.provider
         if provider is not None:
             self._set_hgp_from_provider(provider)
+        # qiskit-ibm-runtime style
+        elif hasattr(self._backend, "_instance"):
+            self.hgp = self._backend._instance
         if recursive:
             for data in self.child_data():
                 data._set_backend(new_backend)
 
     def _set_hgp_from_provider(self, provider):
         try:
-            hub = None
-            group = None
-            project = None
-            # qiskit-ibmq-provider style
-            if hasattr(provider, "credentials"):
-                creds = provider.credentials
-                hub = creds.hub
-                group = creds.group
-                project = creds.project
             # qiskit-ibm-provider style
             if hasattr(provider, "_hgps"):
-                hub, group, project = list(self.backend.provider._hgps.keys())[0].split("/")
-            self._db_data.hub = self._db_data.hub or hub
-            self._db_data.group = self._db_data.group or group
-            self._db_data.project = self._db_data.project or project
-        except (AttributeError, IndexError):
+                for hgp_string, hgp in provider._hgps.items():
+                    if self.backend.name in hgp.backends:
+                        self.hgp = hgp_string
+                        break
+        except (AttributeError, IndexError, QiskitError):
             return
 
+    @property
+    def hgp(self) -> str:
+        """Returns Hub/Group/Project data as a formatted string"""
+        return f"{self.hub}/{self.group}/{self.project}"
+
+    @hgp.setter
+    def hgp(self, new_hgp: str) -> None:
+        """Sets the Hub/Group/Project data from a formatted string"""
+        if re.match(r"[^/]*/[^/]*/[^/]*$", new_hgp) is None:
+            raise QiskitError("hgp can be only given in a <hub>/<group>/<project> format")
+        self._db_data.hub, self._db_data.group, self._db_data.project = new_hgp.split("/")
+
     def _clear_results(self):
         """Delete all currently stored analysis results and figures"""
         # Schedule existing analysis results for deletion next save call
-        for key in self._analysis_results.keys():
-            self._deleted_analysis_results.append(key)
-        self._analysis_results = ThreadSafeOrderedDict()
+        self._deleted_analysis_results.extend(list(self._analysis_results.result_ids))
+        self._analysis_results.clear()
         # Schedule existing figures for deletion next save call
+        # TODO: Fully delete artifacts from the service
+        # Current implementation uploads empty files instead
+        for artifact in self._artifacts.values():
+            self._deleted_artifacts.add(artifact.name)
         for key in self._figures.keys():
             self._deleted_figures.append(key)
         self._figures = ThreadSafeOrderedDict()
+        self._artifacts = ThreadSafeOrderedDict()
 
     @property
     def service(self) -> Optional[IBMExperimentService]:
         """Return the database service.
 
         Returns:
             Service that can be used to access this experiment in a database.
@@ -605,14 +649,32 @@
 
         Raises:
             ExperimentDataError: If an experiment service is already being used.
         """
         self._set_service(service)
 
     @property
+    def provider(self) -> Optional[Provider]:
+        """Return the backend provider.
+
+        Returns:
+            Provider that is used to obtain backends and job data.
+        """
+        return self._provider
+
+    @provider.setter
+    def provider(self, provider: Provider) -> None:
+        """Set the provider to be used for obtaining job data
+
+        Args:
+            provider: Provider to be used.
+        """
+        self._provider = provider
+
+    @property
     def auto_save(self) -> bool:
         """Return current auto-save option.
 
         Returns:
             Whether changes will be automatically saved.
         """
         return self._auto_save
@@ -620,46 +682,41 @@
     @auto_save.setter
     def auto_save(self, save_val: bool) -> None:
         """Set auto save preference.
 
         Args:
             save_val: Whether to do auto-save.
         """
-        if save_val is True and not self._auto_save:
-            self.save()
+        # children will be saved once we set auto_save for them
+        if save_val is True:
+            self.save(save_children=False)
         self._auto_save = save_val
-        for res in self._analysis_results.values():
-            # Setting private variable directly to avoid duplicate save. This
-            # can be removed when we start tracking changes.
-            res._auto_save = save_val
         for data in self.child_data():
             data.auto_save = save_val
 
     @property
     def source(self) -> Dict:
         """Return the class name and version."""
         return self._db_data.metadata["_source"]
 
     # Data addition and deletion
 
     def add_data(
         self,
-        data: Union[Result, List[Result], Job, List[Job], Dict, List[Dict]],
+        data: Union[Result, List[Result], Dict, List[Dict]],
     ) -> None:
         """Add experiment data.
 
         Args:
             data: Experiment data to add. Several types are accepted for convenience:
 
                 * Result: Add data from this ``Result`` object.
                 * List[Result]: Add data from the ``Result`` objects.
                 * Dict: Add this data.
                 * List[Dict]: Add this list of data.
-                * Job: (Deprecated) Add data from the job result.
-                * List[Job]: (Deprecated) Add data from the job results.
 
         Raises:
             TypeError: If the input data type is invalid.
         """
         if any(not future.done() for future in self._analysis_futures.values()):
             LOG.warning(
                 "Not all analysis has finished running. Adding new data may "
@@ -783,31 +840,37 @@
         Args:
             job: the Job to wait for and add data from.
 
         Returns:
             A tuple (str, bool) of the job id and bool of if the job data was added.
 
         Raises:
-            Exception: If an error occured when adding job data.
+            Exception: If an error occurred when adding job data.
         """
         jid = job.job_id()
         try:
             job_result = job.result()
-            self._add_result_data(job_result)
+            try:
+                self._running_time = job.time_per_step().get("running", None)
+            except AttributeError:
+                pass
+            self._add_result_data(job_result, jid)
             LOG.debug("Job data added [Job ID: %s]", jid)
+            # sets the endtime to be the time the last successful job was added
+            self.end_datetime = datetime.now()
             return jid, True
         except Exception as ex:  # pylint: disable=broad-except
             # Handle cancelled jobs
             status = job.status()
             if status == JobStatus.CANCELLED:
                 LOG.warning("Job was cancelled before completion [Job ID: %s]", jid)
                 return jid, False
             if status == JobStatus.ERROR:
                 LOG.error(
-                    "Job data not added for errorred job [Job ID: %s]\nError message: %s",
+                    "Job data not added for errored job [Job ID: %s]\nError message: %s",
                     jid,
                     job.error_message(),
                 )
                 return jid, False
             LOG.warning("Adding data from job failed [Job ID: %s]", job.job_id())
             raise ex
 
@@ -821,15 +884,15 @@
         added.
 
         Args:
             callback: Callback function invoked when job finishes successfully.
                       The callback function will be called as
                       ``callback(expdata, **kwargs)`` where `expdata` is this
                       ``DbExperimentData`` object, and `kwargs` are any additional
-                      keywork arguments passed to this method.
+                      keyword arguments passed to this method.
             **kwargs: Keyword arguments to be passed to the callback function.
         """
         with self._job_futures.lock and self._analysis_futures.lock:
             # Create callback dataclass
             cid = uuid.uuid4().hex
             self._analysis_callbacks[cid] = AnalysisCallback(
                 name=callback.__name__,
@@ -909,58 +972,84 @@
                 f"Analysis callback failed [Experiment ID: {self.experiment_id}]"
                 f"[Analysis Callback ID: {callback_id}]:\n{tb_text}"
             )
             self._analysis_callbacks[callback_id].error_msg = error_msg
             LOG.warning(error_msg)
             return callback_id, False
 
-    def _add_result_data(self, result: Result) -> None:
+    def _add_result_data(self, result: Result, job_id: Optional[str] = None) -> None:
         """Add data from a Result object
 
         Args:
             result: Result object containing data to be added.
+            job_id: The id of the job the result came from. If `None`, the
+            job id in `result` is used.
         """
-        if result.job_id not in self._jobs:
-            self._jobs[result.job_id] = None
-            self.job_ids.append(result.job_id)
+        if job_id is None:
+            job_id = result.job_id
+        if job_id not in self._jobs:
+            self._jobs[job_id] = None
+            self.job_ids.append(job_id)
         with self._result_data.lock:
             # Lock data while adding all result data
             for i, _ in enumerate(result.results):
                 data = result.data(i)
-                data["job_id"] = result.job_id
+                data["job_id"] = job_id
                 if "counts" in data:
                     # Format to Counts object rather than hex dict
                     data["counts"] = result.get_counts(i)
                 expr_result = result.results[i]
                 if hasattr(expr_result, "header") and hasattr(expr_result.header, "metadata"):
                     data["metadata"] = expr_result.header.metadata
                 data["shots"] = expr_result.shots
                 data["meas_level"] = expr_result.meas_level
                 if hasattr(expr_result, "meas_return"):
                     data["meas_return"] = expr_result.meas_return
                 self._result_data.append(data)
 
     def _retrieve_data(self):
         """Retrieve job data if missing experiment data."""
-        if self._result_data or not self._backend:
+        # Get job results if missing in experiment data.
+        if self.provider is None:
+            # 'self._result_data' could be locked, so I check a copy of it.
+            if not self._result_data.copy():
+                # Adding warning so the user will have indication why the analysis may fail.
+                LOG.warning(
+                    "Provider for ExperimentData object doesn't exist, resulting in a failed attempt to"
+                    " retrieve data from the server; no stored result data exists"
+                )
             return
-        # Get job results if missing experiment data.
         retrieved_jobs = {}
-        for jid, job in self._jobs.items():
-            if job is None:
+        jobs_to_retrieve = []  # the list of all jobs to retrieve from the server
+
+        # first find which jobs are listed in the `job_ids` field of the experiment data
+        if self.job_ids is not None:
+            for jid in self.job_ids:
+                if jid not in self._jobs or self._jobs[jid] is None:
+                    jobs_to_retrieve.append(jid)
+
+        for jid in jobs_to_retrieve:
+            LOG.debug("Retrieving job [Job ID: %s]", jid)
+            try:  # qiskit-ibm-runtime syntax
+                job = self.provider.job(jid)
+                retrieved_jobs[jid] = job
+            except AttributeError:  # TODO: remove this path for qiskit-ibm-provider
                 try:
-                    LOG.debug("Retrieving job from backend %s [Job ID: %s]", self._backend, jid)
-                    job = self._backend.retrieve_job(jid)
+                    job = self.provider.retrieve_job(jid)
                     retrieved_jobs[jid] = job
                 except Exception:  # pylint: disable=broad-except
                     LOG.warning(
-                        "Unable to retrieve data from job on backend %s [Job ID: %s]",
-                        self._backend,
+                        "Unable to retrieve data from job [Job ID: %s]: %s",
                         jid,
+                        traceback.format_exc(),
                     )
+            except Exception:  # pylint: disable=broad-except
+                LOG.warning(
+                    "Unable to retrieve data from job [Job ID: %s]: %s", jid, traceback.format_exc()
+                )
         # Add retrieved job objects to stored jobs and extract data
         for jid, job in retrieved_jobs.items():
             self._jobs[jid] = job
             if job.status() in JOB_FINAL_STATES:
                 # Add job results synchronously
                 self._add_job_data(job)
             else:
@@ -996,39 +1085,40 @@
         if isinstance(index, str):
             return [data for data in self._result_data if data.get("job_id") == index]
         raise TypeError(f"Invalid index type {type(index)}.")
 
     @do_auto_save
     def add_figures(
         self,
-        figures,
-        figure_names=None,
-        overwrite=False,
-        save_figure=None,
+        figures: Union[FigureType, List[FigureType]],
+        figure_names: Optional[Union[str, List[str]]] = None,
+        overwrite: bool = False,
+        save_figure: Optional[bool] = None,
     ) -> Union[str, List[str]]:
         """Add the experiment figure.
 
         Args:
-            figures (str or bytes or pyplot.Figure or list): Paths of the figure
-                files or figure data.
-            figure_names (str or list): Names of the figures. If ``None``, use the figure file
-                names, if given, or a generated name. If `figures` is a list, then
-                `figure_names` must also be a list of the same length or ``None``.
-            overwrite (bool): Whether to overwrite the figure if one already exists with
-                the same name.
-            save_figure (bool): Whether to save the figure in the database. If ``None``,
+            figures: Paths of the figure files or figure data.
+            figure_names: Names of the figures. If ``None``, use the figure file
+                names, if given, or a generated name of the format ``experiment_type``, figure
+                index, first 5 elements of ``device_components``, and first 8 digits of the
+                experiment ID connected by underscores, such as ``T1_Q0_0123abcd.svg``. If `figures`
+                is a list, then `figure_names` must also be a list of the same length or ``None``.
+            overwrite: Whether to overwrite the figure if one already exists with
+                the same name. By default, overwrite is ``False`` and the figure will be renamed
+                with an incrementing numerical suffix. For example, trying to save ``figure.svg`` when
+                ``figure.svg`` already exists will save it as ``figure-1.svg``, and trying to save
+                ``figure-1.svg`` when ``figure-1.svg`` already exists will save it as ``figure-2.svg``.
+            save_figure: Whether to save the figure in the database. If ``None``,
                 the ``auto-save`` attribute is used.
 
         Returns:
-            str or list:
-                Figure names.
+            Figure names in SVG format.
 
         Raises:
-            ExperimentEntryExists: If the figure with the same name already exists,
-                and `overwrite=True` is not specified.
             ValueError: If an input parameter has an invalid value.
         """
         if figure_names is not None and not isinstance(figure_names, list):
             figure_names = [figure_names]
         if not isinstance(figures, list):
             figures = [figures]
         if figure_names is not None and len(figures) != len(figure_names):
@@ -1037,46 +1127,75 @@
                 "the same size as the parameter figures."
             )
 
         added_figs = []
         for idx, figure in enumerate(figures):
             if figure_names is None:
                 if isinstance(figure, str):
+                    # figure is a filename, so we use it as the name
                     fig_name = figure
-                else:
+                elif not isinstance(figure, FigureData):
+                    # Generate a name in the form StandardRB_Q0_Q1_Q2_b4f1d8ad-1.svg
                     fig_name = (
                         f"{self.experiment_type}_"
-                        f"Fig-{len(self._figures)}_"
-                        f"Exp-{self.experiment_id[:8]}.svg"
+                        f'{"_".join(str(i) for i in self.metadata.get("device_components", [])[:5])}_'
+                        f"{self.experiment_id[:8]}.svg"
                     )
+                else:
+                    # Keep the existing figure name if there is one
+                    fig_name = figure.name
             else:
                 fig_name = figure_names[idx]
-
             if not fig_name.endswith(".svg"):
                 LOG.info("File name %s does not have an SVG extension. A '.svg' is added.")
                 fig_name += ".svg"
 
             existing_figure = fig_name in self._figures
             if existing_figure and not overwrite:
-                raise ExperimentEntryExists(
-                    f"A figure with the name {fig_name} for this experiment "
-                    f"already exists. Specify overwrite=True if you "
-                    f"want to overwrite it."
-                )
+                # Remove any existing suffixes then generate new figure name
+                # StandardRB_Q0_Q1_Q2_b4f1d8ad.svg becomes StandardRB_Q0_Q1_Q2_b4f1d8ad
+                fig_name_chunked = fig_name.rsplit("-", 1)
+                if len(fig_name_chunked) != 1:  # Figure name already has a suffix
+                    # This extracts StandardRB_Q0_Q1_Q2_b4f1d8ad as the prefix from
+                    # StandardRB_Q0_Q1_Q2_b4f1d8ad-1.svg
+                    fig_name_prefix = fig_name_chunked[0]
+                    try:
+                        fig_name_suffix = int(fig_name_chunked[1].rsplit(".", 1)[0])
+                    except ValueError:  # the suffix is not an int, add our own suffix
+                        # my-custom-figure-name will be the prefix of my-custom-figure-name.svg
+                        fig_name_prefix = fig_name.rsplit(".", 1)[0]
+                        fig_name_suffix = 0
+                else:
+                    # StandardRB_Q0_Q1_Q2_b4f1d8ad.svg has no hyphens so
+                    # StandardRB_Q0_Q1_Q2_b4f1d8ad would be its prefix
+                    fig_name_prefix = fig_name.rsplit(".", 1)[0]
+                    fig_name_suffix = 0
+                fig_name = f"{fig_name_prefix}-{fig_name_suffix + 1}.svg"
+                while fig_name in self._figures:  # Increment suffix until the name isn't taken
+                    # If StandardRB_Q0_Q1_Q2_b4f1d8ad-1.svg already exists,
+                    # StandardRB_Q0_Q1_Q2_b4f1d8ad-2.svg will be the name of this figure
+                    fig_name_suffix += 1
+                    fig_name = f"{fig_name_prefix}-{fig_name_suffix + 1}.svg"
+
             # figure_data = None
             if isinstance(figure, str):
                 with open(figure, "rb") as file:
                     figure = file.read()
 
             # check whether the figure is already wrapped, meaning it came from a sub-experiment
             if isinstance(figure, FigureData):
                 figure_data = figure.copy(new_name=fig_name)
+                figure = figure_data.figure
 
             else:
-                figure_metadata = {"qubits": self.metadata.get("physical_qubits")}
+                figure_metadata = {
+                    "qubits": self.metadata.get("physical_qubits"),
+                    "device_components": self.metadata.get("device_components"),
+                    "experiment_type": self.experiment_type,
+                }
                 figure_data = FigureData(figure=figure, name=fig_name, metadata=figure_metadata)
 
             self._figures[fig_name] = figure_data
             self._db_data.figure_names.append(fig_name)
 
             save = save_figure if save_figure is not None else self.auto_save
             if save and self._service:
@@ -1104,29 +1223,46 @@
 
         Returns:
             Figure name.
 
         Raises:
             ExperimentEntryNotFound: If the figure is not found.
         """
-        if isinstance(figure_key, int):
-            figure_key = self._figures.keys()[figure_key]
-        elif figure_key not in self._figures:
-            raise ExperimentEntryNotFound(f"Figure {figure_key} not found.")
+        figure_key = self._find_figure_key(figure_key)
 
         del self._figures[figure_key]
         self._deleted_figures.append(figure_key)
 
         if self._service and self.auto_save:
             with service_exception_to_warning():
                 self.service.delete_figure(experiment_id=self.experiment_id, figure_name=figure_key)
             self._deleted_figures.remove(figure_key)
 
         return figure_key
 
+    def _find_figure_key(
+        self,
+        figure_key: int | str,
+    ) -> str:
+        """A helper method to find figure key."""
+        if isinstance(figure_key, int):
+            if figure_key < 0 or figure_key >= len(self._figures):
+                raise ExperimentEntryNotFound(f"Figure index {figure_key} out of range.")
+            return self._figures.keys()[figure_key]
+
+        # All figures must have '.svg' in their names when added, as the extension is added to the key
+        # name in the `add_figures()` method of this class.
+        if isinstance(figure_key, str):
+            if not figure_key.endswith(".svg"):
+                figure_key += ".svg"
+
+        if figure_key not in self._figures:
+            raise ExperimentEntryNotFound(f"Figure key {figure_key} not found.")
+        return figure_key
+
     def figure(
         self,
         figure_key: Union[str, int],
         file_name: Optional[str] = None,
     ) -> Union[int, FigureData]:
         """Retrieve the specified experiment figure.
 
@@ -1138,18 +1274,15 @@
         Returns:
             The size of the figure if `file_name` is specified. Otherwise the
             content of the figure as a `FigureData` object.
 
         Raises:
             ExperimentEntryNotFound: If the figure cannot be found.
         """
-        if isinstance(figure_key, int):
-            if figure_key < 0 or figure_key >= len(self._figures.keys()):
-                raise ExperimentEntryNotFound(f"Figure {figure_key} not found.")
-            figure_key = self._figures.keys()[figure_key]
+        figure_key = self._find_figure_key(figure_key)
 
         figure_data = self._figures.get(figure_key, None)
         if figure_data is None and self.service:
             figure = self.service.figure(experiment_id=self.experiment_id, figure_name=figure_key)
             figure_data = FigureData(figure=figure, name=figure_key)
             self._figures[figure_key] = figure_data
 
@@ -1158,181 +1291,318 @@
 
         if file_name:
             with open(file_name, "wb") as output:
                 num_bytes = output.write(figure_data.figure)
                 return num_bytes
         return figure_data
 
+    @deprecate_arg(
+        name="results",
+        since="0.6",
+        additional_msg="Use keyword arguments rather than creating an AnalysisResult object.",
+        package_name="qiskit-experiments",
+        pending=True,
+    )
     @do_auto_save
     def add_analysis_results(
         self,
-        results: Union[AnalysisResult, List[AnalysisResult]],
+        results: Optional[Union[AnalysisResult, List[AnalysisResult]]] = None,
+        *,
+        name: Optional[str] = None,
+        value: Optional[Any] = None,
+        quality: Optional[str] = None,
+        components: Optional[List[DeviceComponent]] = None,
+        experiment: Optional[str] = None,
+        experiment_id: Optional[str] = None,
+        result_id: Optional[str] = None,
+        tags: Optional[List[str]] = None,
+        backend: Optional[str] = None,
+        run_time: Optional[datetime] = None,
+        created_time: Optional[datetime] = None,
+        **extra_values,
     ) -> None:
         """Save the analysis result.
 
         Args:
             results: Analysis results to be saved.
-        """
-        if not isinstance(results, list):
-            results = [results]
-
-        for result in results:
-            self._analysis_results[result.result_id] = result
-
-            with contextlib.suppress(ExperimentDataError):
-                result.service = self.service
-                result.auto_save = self.auto_save
-
-            if self.auto_save and self._service:
-                result.save()
+            name: Name of the result entry.
+            value: Analyzed quantity.
+            quality: Quality of the data.
+            components: Associated device components.
+            experiment: String identifier of the associated experiment.
+            experiment_id: ID of the associated experiment.
+            result_id: ID of this analysis entry. If not set a random UUID is generated.
+            tags: List of arbitrary tags.
+            backend: Name of associated backend.
+            run_time: The date time when the experiment started to run on the device.
+            created_time: The date time when this analysis is performed.
+            extra_values: Arbitrary keyword arguments for supplementary information.
+                New dataframe columns are created in the analysis result table with added keys.
+        """
+        if results is not None:
+            # TODO deprecate this path
+            if not isinstance(results, list):
+                results = [results]
+            for result in results:
+                extra_values = result.extra.copy()
+                if result.chisq is not None:
+                    # Move chisq to extra.
+                    # This is not global outcome, e.g. QPT doesn't provide chisq.
+                    extra_values["chisq"] = result.chisq
+                experiment = extra_values.pop("experiment", self.experiment_type)
+                backend = extra_values.pop("backend", self.backend_name)
+                run_time = extra_values.pop("run_time", self.running_time)
+                created_time = extra_values.pop("created_time", None)
+                self._analysis_results.add_data(
+                    name=result.name,
+                    value=result.value,
+                    quality=result.quality,
+                    components=result.device_components,
+                    experiment=experiment,
+                    experiment_id=result.experiment_id,
+                    result_id=result.result_id,
+                    tags=result.tags,
+                    backend=backend,
+                    run_time=run_time,
+                    created_time=created_time,
+                    **extra_values,
+                )
+                if self.auto_save:
+                    result.save()
+        else:
+            experiment = experiment or self.experiment_type
+            experiment_id = experiment_id or self.experiment_id
+            tags = tags or []
+            backend = backend or self.backend_name
+
+            uid = self._analysis_results.add_data(
+                result_id=result_id,
+                name=name,
+                value=value,
+                quality=quality,
+                components=components,
+                experiment=experiment,
+                experiment_id=experiment_id,
+                tags=tags or [],
+                backend=backend,
+                run_time=run_time,
+                created_time=created_time,
+                **extra_values,
+            )
+            if self.auto_save:
+                service_result = _series_to_service_result(
+                    series=self._analysis_results.get_data(uid, columns="all").iloc[0],
+                    service=self._service,
+                    auto_save=False,
+                )
+                service_result.save()
 
     @do_auto_save
     def delete_analysis_result(
         self,
         result_key: Union[int, str],
-    ) -> str:
+    ) -> list[str]:
         """Delete the analysis result.
 
         Args:
             result_key: ID or index of the analysis result to be deleted.
 
         Returns:
-            Analysis result ID.
+            Deleted analysis result IDs.
 
         Raises:
-            ExperimentEntryNotFound: If analysis result not found.
+            ExperimentEntryNotFound: If analysis result not found or multiple entries are found.
         """
-
-        if isinstance(result_key, int):
-            result_key = self._analysis_results.keys()[result_key]
-        else:
-            # Retrieve from DB if needed.
-            result_key = self.analysis_results(result_key, block=False).result_id
-
-        del self._analysis_results[result_key]
-        self._deleted_analysis_results.append(result_key)
+        uids = self._analysis_results.del_data(result_key)
 
         if self._service and self.auto_save:
             with service_exception_to_warning():
-                self.service.delete_analysis_result(result_id=result_key)
-            self._deleted_analysis_results.remove(result_key)
+                for uid in uids:
+                    self.service.delete_analysis_result(result_id=uid)
+        else:
+            self._deleted_analysis_results.extend(uids)
 
-        return result_key
+        return uids
 
     def _retrieve_analysis_results(self, refresh: bool = False):
         """Retrieve service analysis results.
 
         Args:
             refresh: Retrieve the latest analysis results from the server, if
                 an experiment service is available.
         """
         # Get job results if missing experiment data.
-        if self.service and (not self._analysis_results or refresh):
+        if self.service and (len(self._analysis_results) == 0 or refresh):
             retrieved_results = self.service.analysis_results(
                 experiment_id=self.experiment_id, limit=None, json_decoder=self._json_decoder
             )
             for result in retrieved_results:
-                result_id = result.result_id
-
-                self._analysis_results[result_id] = AnalysisResult(service=self.service)
-                self._analysis_results[result_id].set_data(result)
-                self._analysis_results[result_id]._created_in_db = True
+                # Canonicalize IBM specific data structure.
+                # TODO define proper data schema on frontend and delegate this to service.
+                cano_quality = AnalysisResult.RESULT_QUALITY_TO_TEXT.get(result.quality, "unknown")
+                cano_components = [to_component(c) for c in result.device_components]
+                extra = result.result_data["_extra"]
+                if result.chisq is not None:
+                    extra["chisq"] = result.chisq
+                self._analysis_results.add_data(
+                    name=result.result_type,
+                    value=result.result_data["_value"],
+                    quality=cano_quality,
+                    components=cano_components,
+                    experiment_id=result.experiment_id,
+                    result_id=result.result_id,
+                    tags=result.tags,
+                    backend=result.backend_name,
+                    created_time=result.creation_datetime,
+                    **extra,
+                )
 
+    @deprecate_arg(
+        name="dataframe",
+        deprecation_description="Setting ``dataframe`` to False in analysis_results",
+        since="0.6",
+        package_name="qiskit-experiments",
+        pending=True,
+        predicate=lambda dataframe: not dataframe,
+    )
     def analysis_results(
         self,
-        index: Optional[Union[int, slice, str]] = None,
+        index: int | slice | str | None = None,
         refresh: bool = False,
         block: bool = True,
-        timeout: Optional[float] = None,
-    ) -> Union[AnalysisResult, List[AnalysisResult]]:
+        timeout: float | None = None,
+        columns: str | list[str] = "default",
+        dataframe: bool = False,
+    ) -> AnalysisResult | list[AnalysisResult] | pd.DataFrame:
         """Return analysis results associated with this experiment.
 
+        When this method is called with ``dataframe=True`` you will receive
+        matched result entries with the ``index`` condition in the dataframe format.
+        You can access a certain entry value by specifying its row index by either
+        row number or short index string. For example,
+
+        .. jupyter-input::
+
+            results = exp_data.analysis_results("res1", dataframe=True)
+
+            print(results)
+
+        .. jupyter-output::
+
+                      name  experiment  components  value  quality  backend          run_time
+            7dd286f4  res1       MyExp    [Q0, Q1]      1     good    test1  2024-02-06 13:46
+            f62042a7  res1       MyExp    [Q2, Q3]      2     good    test1  2024-02-06 13:46
+
+        Getting the first result value with a row number (``iloc``).
+
+        .. code-block:: python
+
+            value = results.iloc[0].value
+
+        Getting the first result value with a short index (``loc``).
+
+        .. code-block:: python
+
+            value = results.loc["7dd286f4"]
+
+        See the pandas `DataFrame`_ documentation for the tips about data handling.
+
+        .. _DataFrame: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html
+
         Args:
             index: Index of the analysis result to be returned.
                 Several types are accepted for convenience:
 
-                    * None: Return all analysis results.
-                    * int: Specific index of the analysis results.
-                    * slice: A list slice of indexes.
-                    * str: ID or name of the analysis result.
+                * None: Return all analysis results.
+                * int: Specific index of the analysis results.
+                * slice: A list slice of indexes.
+                * str: ID or name of the analysis result.
+
             refresh: Retrieve the latest analysis results from the server, if
                 an experiment service is available.
-            block: If True block for any analysis callbacks to finish running.
+            block: If ``True``, block for any analysis callbacks to finish running.
             timeout: max time in seconds to wait for analysis callbacks to finish running.
+            columns: Specifying a set of columns to return. You can pass a list of each
+                column name to return, otherwise builtin column groups are available:
+
+                * ``all``: Return all columns, including metadata to communicate
+                  with the experiment service, such as entry IDs.
+                * ``default``: Return columns including analysis result with supplementary
+                  information about experiment.
+                * ``minimal``: Return only analysis subroutine returns.
+
+            dataframe: Set to ``True`` to return analysis results in the dataframe format.
 
         Returns:
-            Analysis results for this experiment.
+            A copy of analysis results data. Updating the returned object doesn't
+            mutate the original dataset.
 
         Raises:
-            TypeError: If the input `index` has an invalid type.
             ExperimentEntryNotFound: If the entry cannot be found.
         """
         if block:
             self._wait_for_futures(
                 self._analysis_futures.values(), name="analysis", timeout=timeout
             )
         self._retrieve_analysis_results(refresh=refresh)
-        if index is None:
-            return self._analysis_results.values()
 
-        def _make_not_found_message(index: Union[int, slice, str]) -> str:
-            """Helper to make error message for index not found"""
-            msg = [f"Analysis result {index} not found."]
-            errors = self.errors()
-            if errors:
-                msg.append(f"Errors: {errors}")
-            return "\n".join(msg)
-
-        if isinstance(index, int):
-            if index >= len(self._analysis_results.values()):
-                raise ExperimentEntryNotFound(_make_not_found_message(index))
-            return self._analysis_results.values()[index]
-        if isinstance(index, slice):
-            results = self._analysis_results.values()[index]
-            if not results:
-                raise ExperimentEntryNotFound(_make_not_found_message(index))
-            return results
-        if isinstance(index, str):
-            # Check by result ID
-            if index in self._analysis_results:
-                return self._analysis_results[index]
-            # Check by name
-            filtered = [
-                result for result in self._analysis_results.values() if result.name == index
-            ]
-            if not filtered:
-                raise ExperimentEntryNotFound(_make_not_found_message(index))
-            if len(filtered) == 1:
-                return filtered[0]
-            else:
-                return filtered
+        if dataframe:
+            return self._analysis_results.get_data(index, columns=columns)
 
-        raise TypeError(f"Invalid index type {type(index)}.")
+        # Convert back into List[AnalysisResult] which is payload for IBM experiment service.
+        # This will be removed in future version.
+        tmp_df = self._analysis_results.get_data(index, columns="all")
+        service_results = []
+        for _, series in tmp_df.iterrows():
+            service_results.append(
+                _series_to_service_result(
+                    series=series,
+                    service=self._service,
+                    auto_save=self._auto_save,
+                )
+            )
+        if index == 0 and tmp_df.iloc[0]["name"].startswith("@"):
+            warnings.warn(
+                "Curve fit results have moved to experiment artifacts and will be removed "
+                "from analysis results in a future release. Use "
+                'expdata.artifacts("fit_summary").data to access curve fit results.',
+                DeprecationWarning,
+            )
+        elif isinstance(index, (int, slice)):
+            warnings.warn(
+                "Accessing analysis results via a numerical index is deprecated and will be "
+                "removed in a future release. Use the ID or name of the analysis result "
+                "instead.",
+                DeprecationWarning,
+            )
+        if len(service_results) == 1 and index is not None:
+            return service_results[0]
+        return service_results
 
     # Save and load from the database
 
     def save_metadata(self) -> None:
         """Save this experiments metadata to a database service.
 
         .. note::
-            This method does not save analysis results nor figures.
+            This method does not save analysis results, figures, or artifacts.
             Use :meth:`save` for general saving of all experiment data.
 
             See :meth:`qiskit.providers.experiment.IBMExperimentService.create_experiment`
             for fields that are saved.
         """
         self._save_experiment_metadata()
         for data in self.child_data():
             data.save_metadata()
 
     def _save_experiment_metadata(self, suppress_errors: bool = True) -> None:
         """Save this experiments metadata to a database service.
         Args:
             suppress_errors: should the method catch exceptions (true) or
-            pass them on, potentially aborting the experiemnt (false)
+            pass them on, potentially aborting the experiment (false)
         Raises:
             QiskitError: If the save to the database failed
         .. note::
             This method does not save analysis results nor figures.
             Use :meth:`save` for general saving of all experiment data.
 
             See :meth:`qiskit.providers.experiment.IBMExperimentService.create_experiment`
@@ -1347,42 +1617,70 @@
             return
         try:
             handle_metadata_separately = self._metadata_too_large()
             if handle_metadata_separately:
                 metadata = self._db_data.metadata
                 self._db_data.metadata = {}
 
-            self.service.create_or_update_experiment(
+            result = self.service.create_or_update_experiment(
                 self._db_data, json_encoder=self._json_encoder, create=not self._created_in_db
             )
+            if isinstance(result, dict):
+                created_datetime = result.get("created_at", None)
+                updated_datetime = result.get("updated_at", None)
+                self._db_data.creation_datetime = parse_utc_datetime(created_datetime)
+                self._db_data.updated_datetime = parse_utc_datetime(updated_datetime)
+
             self._created_in_db = True
 
             if handle_metadata_separately:
                 self.service.file_upload(
-                    self._db_data.experiment_id, self._metadata_filename, metadata
+                    self._db_data.experiment_id,
+                    self._metadata_filename,
+                    metadata,
+                    json_encoder=self._json_encoder,
                 )
                 self._db_data.metadata = metadata
 
         except Exception as ex:  # pylint: disable=broad-except
             # Don't automatically fail the experiment just because its data cannot be saved.
             LOG.error("Unable to save the experiment data: %s", traceback.format_exc())
             if not suppress_errors:
                 raise QiskitError(f"Experiment data save failed\nError Message:\n{str(ex)}") from ex
 
     def _metadata_too_large(self):
         """Determines whether the metadata should be stored in a separate file"""
         # currently the entire POST JSON request body is limited by default to 100kb
-        return sys.getsizeof(self.metadata) > 10000
+        total_metadata_size = sys.getsizeof(json.dumps(self.metadata, cls=self._json_encoder))
+        return total_metadata_size > 10000
 
-    def save(self, suppress_errors: bool = True) -> None:
+    # Save and load from the database
+
+    def save(
+        self,
+        suppress_errors: bool = True,
+        max_workers: int = 3,
+        save_figures: bool = True,
+        save_artifacts: bool = True,
+        save_children: bool = True,
+    ) -> None:
         """Save the experiment data to a database service.
 
         Args:
             suppress_errors: should the method catch exceptions (true) or
-            pass them on, potentially aborting the experiemnt (false)
+                pass them on, potentially aborting the experiment (false)
+            max_workers: Maximum number of concurrent worker threads (default 3, maximum 10)
+            save_figures: Whether to save figures in the database or not
+            save_artifacts: Whether to save artifacts in the database
+            save_children: For composite experiments, whether to save children as well
+
+        Raises:
+            ExperimentDataSaveFailed: If no experiment database service
+            was found, or the experiment service failed to save
+
         .. note::
             This saves the experiment metadata, all analysis results, and all
             figures. Depending on the number of figures and analysis results this
             operation could take a while.
 
             To only update a previously saved experiments metadata (eg for
             additional tags or notes) use :meth:`save_metadata`.
@@ -1390,65 +1688,157 @@
         # TODO - track changes
         if not self._service:
             LOG.warning(
                 "Experiment cannot be saved because no experiment service is available. "
                 "An experiment service is available, for example, "
                 "when using an IBM Quantum backend."
             )
-            return
+            if suppress_errors:
+                return
+            else:
+                raise ExperimentDataSaveFailed("No service found")
+        if max_workers > self._max_workers_cap:
+            LOG.warning(
+                "max_workers cannot be larger than %s. Setting max_workers = %s now.",
+                self._max_workers_cap,
+                self._max_workers_cap,
+            )
+            max_workers = self._max_workers_cap
+
+        if save_artifacts:
+            # populate the metadata entry for artifact file names
+            self.metadata["artifact_files"] = {
+                f"{artifact.name}.zip" for artifact in self._artifacts.values()
+            }
 
         self._save_experiment_metadata(suppress_errors=suppress_errors)
+
         if not self._created_in_db:
             LOG.warning("Could not save experiment metadata to DB, aborting experiment save")
             return
 
-        for result in self._analysis_results.values():
-            result.save(suppress_errors=suppress_errors)
+        analysis_results_to_create = []
+        for _, series in self._analysis_results.dataframe.iterrows():
+            # TODO We should support saving entire dataframe
+            #  Calling API per entry takes huge amount of time.
+            legacy_result = _series_to_service_result(
+                series=series,
+                service=self._service,
+                auto_save=False,
+            )
+            analysis_results_to_create.append(legacy_result._db_data)
+        try:
+            self.service.create_analysis_results(
+                data=analysis_results_to_create,
+                blocking=True,
+                json_encoder=self._json_encoder,
+                max_workers=max_workers,
+            )
+        except Exception as ex:  # pylint: disable=broad-except
+            # Don't automatically fail the experiment just because its data cannot be saved.
+            LOG.error("Unable to save the experiment data: %s", traceback.format_exc())
+            if not suppress_errors:
+                raise ExperimentDataSaveFailed(
+                    f"Analysis result save failed\nError Message:\n{str(ex)}"
+                ) from ex
 
         for result in self._deleted_analysis_results.copy():
             with service_exception_to_warning():
                 self._service.delete_analysis_result(result_id=result)
             self._deleted_analysis_results.remove(result)
 
-        with self._figures.lock:
-            for name, figure in self._figures.items():
-                if figure is None:
-                    continue
-                # currently only the figure and its name are stored in the database
-                if isinstance(figure, FigureData):
-                    figure = figure.figure
-                    LOG.debug("Figure metadata is currently not saved to the database")
-                if isinstance(figure, pyplot.Figure):
-                    figure = plot_to_svg_bytes(figure)
-                self._service.create_or_update_figure(
-                    experiment_id=self.experiment_id, figure=figure, figure_name=name
+        if save_figures:
+            with self._figures.lock:
+                figures_to_create = []
+                for name, figure in self._figures.items():
+                    if figure is None:
+                        continue
+                    # currently only the figure and its name are stored in the database
+                    if isinstance(figure, FigureData):
+                        figure = figure.figure
+                        LOG.debug("Figure metadata is currently not saved to the database")
+                    if isinstance(figure, pyplot.Figure):
+                        figure = plot_to_svg_bytes(figure)
+                    figures_to_create.append((figure, name))
+                self.service.create_figures(
+                    experiment_id=self.experiment_id,
+                    figure_list=figures_to_create,
+                    blocking=True,
+                    max_workers=max_workers,
                 )
 
         for name in self._deleted_figures.copy():
             with service_exception_to_warning():
                 self._service.delete_figure(experiment_id=self.experiment_id, figure_name=name)
             self._deleted_figures.remove(name)
 
+        # save artifacts
+        if save_artifacts:
+            with self._artifacts.lock:
+                # make dictionary {artifact name: [artifact ids]}
+                artifact_list = defaultdict(list)
+                for artifact in self._artifacts.values():
+                    artifact_list[artifact.name].append(artifact.artifact_id)
+                try:
+                    for artifact_name, artifact_ids in artifact_list.items():
+                        file_zipped = objs_to_zip(
+                            artifact_ids,
+                            [self._artifacts[artifact_id] for artifact_id in artifact_ids],
+                            json_encoder=self._json_encoder,
+                        )
+                        self.service.file_upload(
+                            experiment_id=self.experiment_id,
+                            file_name=f"{artifact_name}.zip",
+                            file_data=file_zipped,
+                        )
+                except Exception:  # pylint: disable=broad-except:
+                    LOG.error("Unable to save artifacts: %s", traceback.format_exc())
+
+            # Upload a blank file if the whole file should be deleted
+            # TODO: replace with direct artifact deletion when available
+            for artifact_name in self._deleted_artifacts.copy():
+                try:  # Don't overwrite with a blank file if there's still artifacts with this name
+                    self.artifacts(artifact_name)
+                except Exception:  # pylint: disable=broad-except:
+                    with service_exception_to_warning():
+                        self.service.file_upload(
+                            experiment_id=self.experiment_id,
+                            file_name=f"{artifact_name}.zip",
+                            file_data=None,
+                        )
+                # Even if we didn't overwrite an artifact file, we don't need to keep this because
+                # an existing artifact(s) needs to be deleted to delete the artifact file in the future
+                self._deleted_artifacts.remove(artifact_name)
+
         if not self.service.local and self.verbose:
             print(
                 "You can view the experiment online at "
-                f"https://quantum-computing.ibm.com/experiments/{self.experiment_id}"
+                f"https://quantum.ibm.com/experiments/{self.experiment_id}"
             )
         # handle children, but without additional prints
-        for data in self._child_data.values():
-            original_verbose = data.verbose
-            data.verbose = False
-            data.save()
-            data.verbose = original_verbose
+        if save_children:
+            for data in self._child_data.values():
+                original_verbose = data.verbose
+                data.verbose = False
+                data.save(
+                    suppress_errors=suppress_errors,
+                    max_workers=max_workers,
+                    save_figures=save_figures,
+                    save_artifacts=save_artifacts,
+                )
+                data.verbose = original_verbose
 
     def jobs(self) -> List[Job]:
         """Return a list of jobs for the experiment"""
         return self._jobs.values()
 
-    def cancel_jobs(self, ids: Optional[Union[str, List[str]]] = None) -> bool:
+    def cancel_jobs(
+        self,
+        ids: str | list[str] | None = None,
+    ) -> bool:
         """Cancel any running jobs.
 
         Args:
             ids: Job(s) to cancel. If None all non-finished jobs will be cancelled.
 
         Returns:
             True if the specified jobs were successfully cancelled
@@ -1474,15 +1864,18 @@
 
                 # Remove done or cancelled job futures
                 if jid in self._job_futures:
                     del self._job_futures[jid]
 
         return all_cancelled
 
-    def cancel_analysis(self, ids: Optional[Union[str, List[str]]] = None) -> bool:
+    def cancel_analysis(
+        self,
+        ids: str | list[str] | None = None,
+    ) -> bool:
         """Cancel any queued analysis callbacks.
 
         .. note::
             A currently running analysis callback cannot be cancelled.
 
         Args:
             ids: Analysis callback(s) to cancel. If None all non-finished
@@ -1562,15 +1955,14 @@
             job_ids = self._job_futures.keys()
             job_futs = self._job_futures.values()
             analysis_ids = self._analysis_futures.keys()
             analysis_futs = self._analysis_futures.values()
 
         # Wait for futures
         self._wait_for_futures(job_futs + analysis_futs, name="jobs and analysis", timeout=timeout)
-
         # Clean up done job futures
         num_jobs = len(job_ids)
         for jid, fut in zip(job_ids, job_futs):
             if (fut.done() and not fut.exception()) or fut.cancelled():
                 if jid in self._job_futures:
                     del self._job_futures[jid]
                     num_jobs -= 1
@@ -1617,15 +2009,15 @@
             LOG.info(
                 "Waiting for %s timed out before completion [Experiment ID: %s].",
                 name,
                 self.experiment_id,
             )
             value = False
 
-        # Check for futures that were cancelled or errorred
+        # Check for futures that were cancelled or errored
         excepts = ""
         for fut in waited.done:
             ex = fut.exception()
             if ex:
                 excepts += "\n".join(traceback.format_exception(type(ex), ex, ex.__traceback__))
                 value = False
             elif fut.cancelled():
@@ -1727,15 +2119,14 @@
             :meth:`cancel_jobs` to terminate these remaining jobs.
 
         Returns:
             The job execution status.
         """
         statuses = set()
         with self._jobs.lock:
-
             # No jobs present
             if not self._jobs:
                 return JobStatus.DONE
 
             statuses = set()
             for job in self._jobs.values():
                 if job:
@@ -1864,50 +2255,85 @@
         if isinstance(index, (int, slice)):
             return self._child_data.values()[index]
         if isinstance(index, str):
             return self._child_data[index]
         raise QiskitError(f"Invalid index type {type(index)}.")
 
     @classmethod
-    def load(cls, experiment_id: str, service: IBMExperimentService) -> "ExperimentData":
+    def load(
+        cls,
+        experiment_id: str,
+        service: Optional[IBMExperimentService] = None,
+        provider: Optional[Provider] = None,
+    ) -> "ExperimentData":
         """Load a saved experiment data from a database service.
 
         Args:
             experiment_id: Experiment ID.
             service: the database service.
+            provider: an IBMProvider required for loading job data and
+                can be used to initialize the service. When using
+                :external+qiskit_ibm_runtime:doc:`qiskit-ibm-runtime <index>`,
+                this is the :class:`~qiskit_ibm_runtime.QiskitRuntimeService` and should
+                not be confused with the experiment database service
+                :meth:`qiskit_ibm_experiment.IBMExperimentService`.
 
         Returns:
             The loaded experiment data.
+        Raises:
+            ExperimentDataError: If not service nor provider were given.
         """
+        if service is None:
+            if provider is None:
+                raise ExperimentDataError(
+                    "Loading an experiment requires a valid Qiskit provider or experiment service."
+                )
+            service = cls.get_service_from_provider(provider)
         data = service.experiment(experiment_id, json_decoder=cls._json_decoder)
         if service.experiment_has_file(experiment_id, cls._metadata_filename):
-            metadata = service.file_download(experiment_id, cls._metadata_filename)
+            metadata = service.file_download(
+                experiment_id, cls._metadata_filename, json_decoder=cls._json_decoder
+            )
             data.metadata.update(metadata)
-        expdata = cls(service=service, db_data=data)
+
+        expdata = cls(service=service, db_data=data, provider=provider)
 
         # Retrieve data and analysis results
         # Maybe this isn't necessary but the repr of the class should
         # be updated to show correct number of results including remote ones
         expdata._retrieve_data()
         expdata._retrieve_analysis_results()
 
+        # Recreate artifacts
+        try:
+            if "artifact_files" in expdata.metadata:
+                for filename in expdata.metadata["artifact_files"]:
+                    if service.experiment_has_file(experiment_id, filename):
+                        artifact_file = service.file_download(experiment_id, filename)
+                        for artifact in zip_to_objs(artifact_file, json_decoder=cls._json_decoder):
+                            expdata.add_artifacts(artifact)
+        except Exception:  # pylint: disable=broad-except:
+            LOG.error("Unable to load artifacts: %s", traceback.format_exc())
+
         # mark it as existing in the DB
         expdata._created_in_db = True
 
         child_data_ids = expdata.metadata.pop("child_data_ids", [])
-        child_data = [ExperimentData.load(child_id, service) for child_id in child_data_ids]
+        child_data = [
+            ExperimentData.load(child_id, service, provider) for child_id in child_data_ids
+        ]
         expdata._set_child_data(child_data)
 
         return expdata
 
     def copy(self, copy_results: bool = True) -> "ExperimentData":
         """Make a copy of the experiment data with a new experiment ID.
 
         Args:
-            copy_results: If True copy the analysis results and figures
+            copy_results: If True copy the analysis results, figures, and artifacts
                           into the returned container, along with the
                           experiment data and metadata. If False only copy
                           the experiment data and metadata.
 
         Returns:
             A copy of the experiment data object with the same data
             but different IDs.
@@ -1918,20 +2344,23 @@
 
             This method can not be called from an analysis callback. It waits
             for analysis callbacks to complete before copying analysis results.
         """
         new_instance = ExperimentData(
             backend=self.backend,
             service=self.service,
+            provider=self.provider,
             parent_id=self.parent_id,
             job_ids=self.job_ids,
             child_data=list(self._child_data.values()),
             verbose=self.verbose,
         )
         new_instance._db_data = self._db_data.copy()
+        # Figure names shouldn't be copied over
+        new_instance._db_data.figure_names = []
         new_instance._db_data.experiment_id = str(
             uuid.uuid4()
         )  # different id for copied experiment
         if self.experiment is None:
             new_instance._experiment = None
         else:
             new_instance._experiment = self.experiment.copy()
@@ -1958,21 +2387,23 @@
         # If not copying results return the object
         if not copy_results:
             return new_instance
 
         # Copy results and figures.
         # This requires analysis callbacks to finish
         self._wait_for_futures(self._analysis_futures.values(), name="analysis")
-        with self._analysis_results.lock:
-            new_instance._analysis_results = ThreadSafeOrderedDict()
-            new_instance.add_analysis_results([result.copy() for result in self.analysis_results()])
+        new_instance._analysis_results = self._analysis_results.copy()
         with self._figures.lock:
             new_instance._figures = ThreadSafeOrderedDict()
             new_instance.add_figures(self._figures.values())
 
+        with self._artifacts.lock:
+            new_instance._artifacts = ThreadSafeOrderedDict()
+            new_instance.add_artifacts(self._artifacts.values())
+
         # Recursively copy child data
         child_data = [data.copy(copy_results=copy_results) for data in self.child_data()]
         new_instance._set_child_data(child_data)
         return new_instance
 
     def _set_child_data(self, child_data: List[ExperimentData]):
         """Set child experiment data for the current experiment."""
@@ -1992,16 +2423,14 @@
 
         Raises:
             ExperimentDataError: If an experiment service is already being used and `replace==False`.
         """
         if self._service and not replace:
             raise ExperimentDataError("An experiment service is already being used.")
         self._service = service
-        for result in self._analysis_results.values():
-            result.service = service
         with contextlib.suppress(Exception):
             self.auto_save = self._service.options.get("auto_save", False)
         for data in self.child_data():
             data._set_service(service)
 
     def add_tags_recursive(self, tags2add: List[str]) -> None:
         """Add tags to this experiment itself and its descendants
@@ -2019,15 +2448,15 @@
         Args:
             tags2remove - the tags that will be removed from the existing tags
         """
         self.tags = [x for x in self.tags if x not in tags2remove]
         for data in self._child_data.values():
             data.remove_tags_recursive(tags2remove)
 
-    # represetnation and serialization
+    # representation and serialization
 
     def __repr__(self):
         out = f"{type(self).__name__}({self.experiment_type}"
         out += f", {self.experiment_id}"
         if self.parent_id:
             out += f", parent_id={self.parent_id}"
         if self.tags:
@@ -2096,16 +2525,18 @@
             "_deleted_figures": self._deleted_figures,
             "_deleted_analysis_results": self._deleted_analysis_results,
             "_result_data": self._result_data,
             "_extra_data": self._extra_data,
             "_created_in_db": self._created_in_db,
             "_figures": self._safe_serialize_figures(),  # Convert figures to SVG
             "_jobs": self._safe_serialize_jobs(),  # Handle non-serializable objects
+            "_artifacts": self._artifacts,
             "_experiment": self._experiment,
             "_child_data": self._child_data,
+            "_running_time": self._running_time,
         }
         # the attribute self._service in charge of the connection and communication with the
         #  experiment db. It doesn't have meaning in the json format so there is no need to serialize
         #  it.
         for att in ["_service", "_backend"]:
             json_value[att] = None
             value = getattr(self, att)
@@ -2145,35 +2576,50 @@
         # Handle partially pickleable attributes
         state["_jobs"] = self._safe_serialize_jobs()
 
         return state
 
     @staticmethod
     def get_service_from_backend(backend):
-        """Initializes the server from the backend data"""
-        db_url = "https://auth.quantum-computing.ibm.com/api"
+        """Initializes the service from the backend data"""
+        # qiskit-ibm-runtime style
+        try:
+            if hasattr(backend, "service"):
+                token = backend.service._account.token
+                return IBMExperimentService(token=token, url=backend.service._account.url)
+            return ExperimentData.get_service_from_provider(backend.provider)
+        except Exception:  # pylint: disable=broad-except
+            return None
+
+    @staticmethod
+    def get_service_from_provider(provider):
+        """Initializes the service from the provider data"""
         try:
-            provider = backend._provider
-            # qiskit-ibmq-provider style
-            if hasattr(provider, "credentials"):
-                token = provider.credentials.token
             # qiskit-ibm-provider style
             if hasattr(provider, "_account"):
-                token = provider._account.token
-            service = IBMExperimentService(token=token, url=db_url)
-            return service
+                warnings.warn(
+                    "qiskit-ibm-provider has been deprecated in favor of qiskit-ibm-runtime. Support"
+                    "for qiskit-ibm-provider backends will be removed in Qiskit Experiments 0.7.",
+                    DeprecationWarning,
+                    stacklevel=2,
+                )
+                return IBMExperimentService(
+                    token=provider._account.token, url=provider._account.url
+                )
+            return None
         except Exception:  # pylint: disable=broad-except
             return None
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         # Initialize non-pickled attributes
         self._job_futures = ThreadSafeOrderedDict()
         self._analysis_futures = ThreadSafeOrderedDict()
         self._analysis_executor = futures.ThreadPoolExecutor(max_workers=1)
+        self._monitor_executor = futures.ThreadPoolExecutor()
 
     def __str__(self):
         line = 51 * "-"
         n_res = len(self._analysis_results)
         status = self.status()
         ret = line
         ret += f"\nExperiment: {self.experiment_type}"
@@ -2189,76 +2635,177 @@
         if self.backend:
             ret += f"\nBackend: {self.backend}"
         if self.tags:
             ret += f"\nTags: {self.tags}"
         ret += f"\nData: {len(self._result_data)}"
         ret += f"\nAnalysis Results: {n_res}"
         ret += f"\nFigures: {len(self._figures)}"
+        ret += f"\nArtifacts: {len(self._artifacts)}"
         return ret
 
+    def add_artifacts(self, artifacts: ArtifactData | list[ArtifactData], overwrite: bool = False):
+        """Add artifacts to experiment. The artifact ID must be unique.
 
-@contextlib.contextmanager
-def service_exception_to_warning():
-    """Convert an exception raised by experiment service to a warning."""
-    try:
-        yield
-    except Exception:  # pylint: disable=broad-except
-        LOG.warning("Experiment service operation failed: %s", traceback.format_exc())
+        Args:
+            artifacts: Artifact or list of artifacts to be added.
+            overwrite: Whether to overwrite the existing artifact.
+        """
+        if isinstance(artifacts, ArtifactData):
+            artifacts = [artifacts]
+
+        for artifact in artifacts:
+            if artifact.artifact_id in self._artifacts and not overwrite:
+                raise ValueError(
+                    "An artifact with id {artifact.id} already exists."
+                    "Set overwrite to True if you want to overwrite the existing"
+                    "artifact."
+                )
+            self._artifacts[artifact.artifact_id] = artifact
 
+    def delete_artifact(
+        self,
+        artifact_key: int | str,
+    ) -> str | list[str]:
+        """Delete specified artifact data.
 
-class ExperimentStatus(enum.Enum):
-    """Class for experiment status enumerated type."""
+        Args:
+            artifact_key: UID, name or index of the figure.
 
-    EMPTY = "experiment data is empty"
-    INITIALIZING = "experiment jobs are being initialized"
-    VALIDATING = "experiment jobs are validating"
-    QUEUED = "experiment jobs are queued"
-    RUNNING = "experiment jobs is actively running"
-    CANCELLED = "experiment jobs or analysis has been cancelled"
-    POST_PROCESSING = "experiment analysis is actively running"
-    DONE = "experiment jobs and analysis have successfully run"
-    ERROR = "experiment jobs or analysis incurred an error"
+        Returns:
+            Deleted artifact ids.
+        """
+        artifact_keys = self._find_artifact_keys(artifact_key)
 
-    def __json_encode__(self):
-        return self.name
+        for key in artifact_keys:
+            self._deleted_artifacts.add(self._artifacts[key].name)
+            del self._artifacts[key]
 
-    @classmethod
-    def __json_decode__(cls, value):
-        return cls.__members__[value]  # pylint: disable=unsubscriptable-object
+        if len(artifact_keys) == 1:
+            return artifact_keys[0]
+        return artifact_keys
+
+    def artifacts(
+        self,
+        artifact_key: int | str = None,
+    ) -> ArtifactData | list[ArtifactData]:
+        """Return specified artifact data.
 
+        Args:
+            artifact_key: UID, name or index of the figure.
 
-class AnalysisStatus(enum.Enum):
-    """Class for analysis callback status enumerated type."""
+        Returns:
+            A list of specified artifact data.
+        """
+        if artifact_key is None:
+            return self._artifacts.values()
 
-    QUEUED = "analysis callback is queued"
-    RUNNING = "analysis callback is actively running"
-    CANCELLED = "analysis callback has been cancelled"
-    DONE = "analysis callback has successfully run"
-    ERROR = "analysis callback incurred an error"
+        artifact_keys = self._find_artifact_keys(artifact_key)
 
-    def __json_encode__(self):
-        return self.name
+        out = []
+        for key in artifact_keys:
+            artifact_data = self._artifacts[key]
+            out.append(artifact_data)
 
-    @classmethod
-    def __json_decode__(cls, value):
-        return cls.__members__[value]  # pylint: disable=unsubscriptable-object
+        if len(out) == 1:
+            return out[0]
+        return out
 
+    def _find_artifact_keys(
+        self,
+        artifact_key: int | str,
+    ) -> list[str]:
+        """A helper method to find artifact key."""
+        if isinstance(artifact_key, int):
+            if artifact_key < 0 or artifact_key >= len(self._artifacts):
+                raise ExperimentEntryNotFound(f"Artifact index {artifact_key} out of range.")
+            return [self._artifacts.keys()[artifact_key]]
+
+        if artifact_key not in self._artifacts:
+            name_matched = [k for k, d in self._artifacts.items() if d.name == artifact_key]
+            if len(name_matched) == 0:
+                raise ExperimentEntryNotFound(f"Artifact key {artifact_key} not found.")
+            return name_matched
+        return [artifact_key]
 
-@dataclasses.dataclass
-class AnalysisCallback:
-    """Dataclass for analysis callback status"""
-
-    name: str = ""
-    callback_id: str = ""
-    status: AnalysisStatus = AnalysisStatus.QUEUED
-    error_msg: Optional[str] = None
-    event: Event = dataclasses.field(default_factory=Event)
 
-    def __getstate__(self):
-        # We need to remove the Event object from state when pickling
-        # since events are not pickleable
-        state = self.__dict__
-        state["event"] = None
-        return state
+@contextlib.contextmanager
+def service_exception_to_warning():
+    """Convert an exception raised by experiment service to a warning."""
+    try:
+        yield
+    except Exception:  # pylint: disable=broad-except
+        LOG.warning("Experiment service operation failed: %s", traceback.format_exc())
 
-    def __json_encode__(self):
-        return self.__getstate__()
+
+def _series_to_service_result(
+    series: pd.Series,
+    service: IBMExperimentService,
+    auto_save: bool,
+    source: Optional[Dict[str, Any]] = None,
+) -> AnalysisResult:
+    """Helper function to convert dataframe to AnalysisResult payload for IBM experiment service.
+
+    .. note::
+
+        Now :class:`.AnalysisResult` is only used to save data in the experiment service.
+        All local operations must be done with :class:`.AnalysisResultTable` dataframe.
+        ExperimentData._analysis_results are totally decoupled from
+        the model of IBM experiment service until this function is implicitly called.
+
+    Args:
+        series: Pandas dataframe Series (a row of dataframe).
+        service: Experiment service.
+        auto_save: Do auto save when entry value changes.
+
+    Returns:
+        Legacy AnalysisResult payload.
+    """
+    # TODO This must be done on experiment service rather than by client.
+    qe_result = AnalysisResultData.from_table_element(**series.replace({np.nan: None}).to_dict())
+
+    result_data = AnalysisResult.format_result_data(
+        value=qe_result.value,
+        extra=qe_result.extra,
+        chisq=qe_result.chisq,
+        source=source,
+    )
+
+    # Overwrite formatted result data dictionary with original objects.
+    # The format_result_data method implicitly deep copies input value and extra field,
+    # but it means the dictionary stores input objects with different object id.
+    # This affects computation of error propagation with ufloats, because it
+    # recognizes the value correlation with object id.
+    # See test.curve_analysis.test_baseclass.TestCurveAnalysis.test_end_to_end_compute_new_entry.
+    result_data["_value"] = qe_result.value
+    result_data["_extra"] = qe_result.extra
+
+    # IBM Experiment Service doesn't have data field for experiment and run time.
+    # These are added to extra field so that these data can be saved.
+    result_data["_extra"]["experiment"] = qe_result.experiment
+    result_data["_extra"]["run_time"] = qe_result.run_time
+
+    try:
+        quality = ResultQuality(str(qe_result.quality).upper())
+    except ValueError:
+        quality = "unknown"
+
+    experiment_service_payload = AnalysisResultDataclass(
+        result_id=qe_result.result_id,
+        experiment_id=qe_result.experiment_id,
+        result_type=qe_result.name,
+        result_data=result_data,
+        device_components=list(map(to_component, qe_result.device_components)),
+        quality=quality,
+        tags=qe_result.tags,
+        backend_name=qe_result.backend,
+        creation_datetime=qe_result.created_time,
+        chisq=qe_result.chisq,
+    )
+
+    service_result = AnalysisResult()
+    service_result.set_data(experiment_service_payload)
+
+    with contextlib.suppress(ExperimentDataError):
+        service_result.service = service
+        service_result.auto_save = auto_save
+
+    return service_result
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/json.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,28 +19,26 @@
 import inspect
 import io
 import json
 import math
 import traceback
 import warnings
 import zlib
+from datetime import datetime
 from functools import lru_cache
 from types import FunctionType, MethodType
 from typing import Any, Dict, Type, Optional, Union, Callable
 
 import lmfit
 import numpy as np
 import scipy.sparse as sps
 import uncertainties
 from qiskit import qpy
 from qiskit.circuit import ParameterExpression, QuantumCircuit, Instruction
-from qiskit.circuit.library import BlueprintCircuit
-from qiskit.quantum_info import DensityMatrix
-from qiskit.quantum_info.operators.channel.quantum_channel import QuantumChannel
-from qiskit.result import LocalReadoutMitigator, CorrelatedReadoutMitigator
+from qiskit.pulse import ScheduleBlock
 from qiskit_experiments.version import __version__
 
 
 @lru_cache()
 def get_module_version(mod_name: str) -> str:
     """Return the __version__ of a module if defined.
 
@@ -456,14 +454,16 @@
             value = _serialize_and_encode(obj, np.save, allow_pickle=False)
             return {"__type__": "ndarray", "__value__": value}
         if isinstance(obj, sps.spmatrix):
             value = _serialize_and_encode(obj, sps.save_npz, compress=False)
             return {"__type__": "spmatrix", "__value__": value}
         if isinstance(obj, bytes):
             return _serialize_bytes(obj)
+        if isinstance(obj, datetime):
+            return {"__type__": "datetime", "__value__": obj.isoformat()}
         if isinstance(obj, np.number):
             return obj.item()
         if dataclasses.is_dataclass(obj):
             # Note that dataclass.asdict recursively convert nested dataclass into dictionary.
             # Thus inter dataclass is unintentionally decoded as dictionary.
             # obj.__dict__ doesn't convert inter dataclass thus serialization
             # is offloaded to usual json serialization mechanism.
@@ -500,53 +500,30 @@
             circuit = QuantumCircuit(obj.num_qubits, obj.num_clbits)
             circuit.append(obj, range(obj.num_qubits), range(obj.num_clbits))
             value = _serialize_and_encode(
                 data=circuit, serializer=lambda buff, data: qpy.dump(data, buff)
             )
             return {"__type__": "Instruction", "__value__": value}
         if isinstance(obj, QuantumCircuit):
-            # TODO Remove the decompose when terra 6713 is released.
-            if isinstance(obj, BlueprintCircuit):
-                obj = obj.decompose()
             value = _serialize_and_encode(
                 data=obj, serializer=lambda buff, data: qpy.dump(data, buff)
             )
             return {"__type__": "QuantumCircuit", "__value__": value}
+        if isinstance(obj, ScheduleBlock):
+            value = _serialize_and_encode(
+                data=obj, serializer=lambda buff, data: qpy.dump(data, buff)
+            )
+            return {"__type__": "ScheduleBlock", "__value__": value}
         if isinstance(obj, ParameterExpression):
             value = _serialize_and_encode(
                 data=obj,
                 serializer=qpy._write_parameter_expression,
                 compress=False,
             )
             return {"__type__": "ParameterExpression", "__value__": value}
-        if isinstance(obj, QuantumChannel):
-            # Temporary fix for incorrect settings in qiskit-terra
-            # See https://github.com/Qiskit/qiskit-terra/pull/7194
-            settings = {
-                "data": obj.data,
-                "input_dims": obj.input_dims(),
-                "output_dims": obj.output_dims(),
-            }
-            return _serialize_object(obj, settings=settings)
-        if isinstance(obj, LocalReadoutMitigator):
-            # Temporary handling until serialization is added to terra stable release
-            settings = {"assignment_matrices": obj._assignment_mats, "qubits": obj.qubits}
-            return _serialize_object(obj, settings=settings)
-        if isinstance(obj, CorrelatedReadoutMitigator):
-            # Temporary handling until serialization is added to terra stable release
-            settings = {"assignment_matrix": obj._assignment_mat, "qubits": obj.qubits}
-            return _serialize_object(obj, settings=settings)
-        if isinstance(obj, DensityMatrix):
-            # Temporary fix for incorrect settings in qiskit-terra
-            # See https://github.com/Qiskit/qiskit-terra/pull/7194
-            settings = {
-                "data": obj.data,
-                "dims": obj.dims(),
-            }
-            return _serialize_object(obj, settings=settings)
         if istype(obj):
             return _serialize_type(obj)
         try:
             return super().default(obj)
         except TypeError:
             return _serialize_object(obj)
 
@@ -577,23 +554,27 @@
                 return _decode_and_deserialize(obj_val, np.load, name=obj_type)
             if obj_type == "spmatrix":
                 return _decode_and_deserialize(obj_val, sps.load_npz, name=obj_type)
             if obj_type == "b64encoded":
                 return _deserialize_bytes(obj_val)
             if obj_type == "set":
                 return set(obj_val)
+            if obj_type == "datetime":
+                return datetime.fromisoformat(obj_val)
             if obj_type == "LMFIT.Model":
                 tmp = lmfit.Model(func=None)
                 load_obj = tmp.loads(s=obj_val)
                 return load_obj
             if obj_type == "Instruction":
                 circuit = _decode_and_deserialize(obj_val, qpy.load, name="QuantumCircuit")[0]
                 return circuit.data[0][0]
             if obj_type == "QuantumCircuit":
                 return _decode_and_deserialize(obj_val, qpy.load, name=obj_type)[0]
+            if obj_type == "ScheduleBlock":
+                return _decode_and_deserialize(obj_val, qpy.load, name=obj_type)[0]
             if obj_type == "ParameterExpression":
                 return _decode_and_deserialize(
                     obj_val, qpy._read_parameter_expression, name=obj_type
                 )
             if obj_type == "safe_float":
                 return self._NaNs.get(obj_val, obj_val)
             if obj_type == "object":
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/matplotlib.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/matplotlib.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/restless_mixin.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/restless_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,18 @@
     This class makes it possible for users to enter a restless run mode without having
     to manually set all the required run options and the data processor. The required options
     are ``rep_delay``, ``init_qubits``, ``memory``, and ``meas_level``. Furthermore,
     subclasses can override the :meth:`_get_restless_processor` method if they require more
     complex restless data processing such as two-qubit calibrations. In addition, this
     class makes it easy to determine if restless measurements are supported for a given
     experiment.
+
+    User Manual
+        :doc:`/manuals/measurement/restless_measurements`
+
     """
 
     analysis: BaseAnalysis
     _default_run_options: Options()
     set_run_options: Callable
     _backend: Backend
     _physical_qubits: Sequence[int]
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/framework/store_init_args.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/store_init_args.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 """
 ======================================================
 Experiment Library (:mod:`qiskit_experiments.library`)
 ======================================================
 
 .. currentmodule:: qiskit_experiments.library
 
-A library of of quantum characterization, calibration and verification
+A library of quantum characterization, calibration and verification
 experiments for calibrating and benchmarking quantum devices. See
-:mod:`qiskit_experiments.framework` for general information the framework
+:mod:`qiskit_experiments.framework` for general information on the framework
 for running experiments.
 
 
 .. _verification:
 
 Verification Experiments
 ========================
@@ -72,14 +72,17 @@
     ~characterization.ReadoutAngle
     ~characterization.ResonatorSpectroscopy
     ~characterization.RoughDrag
     ~characterization.FineDrag
     ~characterization.FineXDrag
     ~characterization.FineSXDrag
     ~characterization.MultiStateDiscrimination
+    ~driven_freq_tuning.StarkRamseyXY
+    ~driven_freq_tuning.StarkRamseyXYAmpScan
+    ~driven_freq_tuning.StarkP1Spectroscopy
 
 .. _characterization two qubits:
 
 Characterization Experiments: Two Qubits
 ========================================
 
 Experiments for characterization of properties of two qubit interactions.
@@ -190,14 +193,19 @@
     TomographyExperiment,
     StateTomography,
     ProcessTomography,
     MitigatedStateTomography,
     MitigatedProcessTomography,
 )
 from .quantum_volume import QuantumVolume
+from .driven_freq_tuning import (
+    StarkRamseyXY,
+    StarkRamseyXYAmpScan,
+    StarkP1Spectroscopy,
+)
 
 # Experiment Sub-modules
 from . import calibration
 from . import characterization
 from . import randomized_benchmarking
 from . import tomography
 from . import quantum_volume
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/fine_amplitude.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/fine_amplitude.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,27 @@
 from qiskit_experiments.calibration_management import (
     BaseCalibrationExperiment,
     Calibrations,
 )
 from qiskit_experiments.library.characterization import FineAmplitude
 from qiskit_experiments.framework import ExperimentData, Options
 from qiskit_experiments.calibration_management.update_library import BaseUpdater
-from qiskit_experiments.warnings import qubit_deprecate
 
 
 class FineAmplitudeCal(BaseCalibrationExperiment, FineAmplitude):
     r"""A calibration version of the :class:`.FineAmplitude` experiment.
 
     # section: overview
 
         :class:`FineAmplitudeCal` is a subclass of :class:`.FineAmplitude`. In the calibration
         experiment the circuits that are run have a custom gate with the pulse schedule attached
         to it through the calibrations.
 
     """
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         calibrations: Calibrations,
         schedule_name: str,
         backend: Optional[Backend] = None,
         cal_parameter_name: Optional[str] = "amp",
@@ -156,15 +154,14 @@
             group,
         )
 
 
 class FineXAmplitudeCal(FineAmplitudeCal):
     """A calibration experiment to calibrate the amplitude of the X schedule."""
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         calibrations: Calibrations,
         schedule_name: str,
         backend: Optional[Backend] = None,
         cal_parameter_name: Optional[str] = "amp",
@@ -205,15 +202,14 @@
         circuit.sx(0)
         return circuit
 
 
 class FineSXAmplitudeCal(FineAmplitudeCal):
     """A calibration experiment to calibrate the amplitude of the SX schedule."""
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         calibrations: Calibrations,
         schedule_name: str,
         backend: Optional[Backend] = None,
         cal_parameter_name: Optional[str] = "amp",
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/fine_drag_cal.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/fine_drag_cal.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,31 +23,29 @@
 from qiskit_experiments.framework import ExperimentData, Options
 from qiskit_experiments.calibration_management import (
     BaseCalibrationExperiment,
     Calibrations,
 )
 from qiskit_experiments.calibration_management.update_library import BaseUpdater
 from qiskit_experiments.library.characterization.fine_drag import FineDrag
-from qiskit_experiments.warnings import qubit_deprecate
 
 
 class FineDragCal(BaseCalibrationExperiment, FineDrag):
-    """A calibration version of the fine drag experiment."""
+    """A calibration version of the fine DRAG experiment."""
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         calibrations: Calibrations,
         schedule_name: str,
         backend: Optional[Backend] = None,
         cal_parameter_name: Optional[str] = "β",
         auto_update: bool = True,
     ):
-        r"""See class :class:`FineDrag` for details.
+        r"""See class :class:`.FineDrag` for details.
 
         Note that this class implicitly assumes that the target angle of the gate
         is :math:`\pi` as seen from the default experiment options.
 
         Args:
             physical_qubits: Sequence containing the qubit for which to run the
                 fine drag calibration.
@@ -64,16 +62,14 @@
             Gate(name=schedule_name, num_qubits=1, params=[]),
             schedule_name=schedule_name,
             backend=backend,
             cal_parameter_name=cal_parameter_name,
             auto_update=auto_update,
         )
 
-        self.set_transpile_options(basis_gates=["sx", schedule_name, "rz"])
-
     @classmethod
     def _default_experiment_options(cls) -> Options:
         """Default experiment options.
 
         Experiment Options:
             target_angle (float): The target rotation angle of the gate being calibrated.
                 This value is needed for the update rule.
@@ -146,26 +142,25 @@
 
         BaseUpdater.add_parameter_value(
             self._cals, experiment_data, new_beta, self._param_name, schedule, group
         )
 
 
 class FineXDragCal(FineDragCal):
-    """Fine drag calibration of X gate."""
+    """Fine DRAG calibration of X gate."""
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         calibrations: Calibrations,
         backend: Optional[Backend] = None,
         cal_parameter_name: Optional[str] = "β",
         auto_update: bool = True,
     ):
-        r"""see class :class:`FineDrag` for details.
+        r"""see class :class:`.FineDrag` for details.
 
         Args:
             physical_qubits: Sequence containing the qubit for which to run the
                 fine drag calibration.
             calibrations: The calibrations instance with the schedules.
             backend: Optional, the backend to run the experiment on.
             cal_parameter_name: The name of the parameter in the schedule to update.
@@ -179,26 +174,25 @@
             backend=backend,
             cal_parameter_name=cal_parameter_name,
             auto_update=auto_update,
         )
 
 
 class FineSXDragCal(FineDragCal):
-    """Fine drag calibration of X gate."""
+    """Fine DRAG calibration of X gate."""
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         calibrations: Calibrations,
         backend: Optional[Backend] = None,
         cal_parameter_name: Optional[str] = "β",
         auto_update: bool = True,
     ):
-        r"""see class :class:`FineDrag` for details.
+        r"""see class :class:`.FineDrag` for details.
 
         Args:
             physical_qubits: Sequence containing the qubit for which to run the
                 fine drag calibration.
             calibrations: The calibrations instance with the schedules.
             backend: Optional, the backend to run the experiment on.
             cal_parameter_name: The name of the parameter in the schedule to update.
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/fine_frequency_cal.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/fine_frequency_cal.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,25 @@
 from qiskit_experiments.framework import ExperimentData
 from qiskit_experiments.calibration_management.update_library import BaseUpdater
 from qiskit_experiments.calibration_management import (
     BaseCalibrationExperiment,
     Calibrations,
 )
 from qiskit_experiments.library.characterization.fine_frequency import FineFrequency
-from qiskit_experiments.warnings import qubit_deprecate
 
 
 class FineFrequencyCal(BaseCalibrationExperiment, FineFrequency):
     """A calibration version of the fine frequency experiment."""
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         calibrations: Calibrations,
         backend: Optional[Backend] = None,
+        cal_parameter_name: Optional[str] = "drive_freq",
         delay_duration: Optional[int] = None,
         repetitions: List[int] = None,
         auto_update: bool = True,
         gate_name: str = "sx",
     ):
         r"""See class :class:`.FineFrequency` for details.
 
@@ -50,33 +49,35 @@
         error attributed to a frequency offset in the qubit.
 
         Args:
             physical_qubits: Sequence containing the qubit for which to run the
                 fine frequency calibration.
             calibrations: The calibrations instance with the schedules.
             backend: Optional, the backend to run the experiment on.
+            cal_parameter_name: The name of the parameter to update in the calibrations.
+                This defaults to `drive_freq`.
             delay_duration: The duration of the delay at :math:`n=1`. If this value is
                 not given then the duration of the gate named ``gate_name`` in the
                 calibrations will be used.
-            auto_update: Whether or not to automatically update the calibrations. By
-                default this variable is set to True.
+            auto_update: Whether to automatically update the calibrations or not. By
+                default, this variable is set to True.
             gate_name: This argument is only needed if ``delay_duration`` is None. This
                 should be the name of a valid schedule in the calibrations.
         """
         if delay_duration is None:
             delay_duration = calibrations.get_schedule(gate_name, physical_qubits[0]).duration
 
         super().__init__(
             calibrations,
             physical_qubits,
             delay_duration=delay_duration,
             schedule_name=None,
             repetitions=repetitions,
             backend=backend,
-            cal_parameter_name=calibrations.__drive_freq_parameter__,
+            cal_parameter_name=cal_parameter_name,
             auto_update=auto_update,
         )
 
         if self.backend is not None:
             self.set_experiment_options(dt=self._backend_data.dt)
 
     @classmethod
@@ -118,15 +119,15 @@
         circuit.add_calibration("sx", self.physical_qubits, schedule)
 
     def update_calibrations(self, experiment_data: ExperimentData):
         r"""Update the qubit frequency based on the measured angle deviation.
 
         The frequency of the qubit is updated according to
 
-        ..math::
+        .. math::
 
             f \to f - \frac{{\rm d}\theta}{2\pi\tau{\rm d}t}
 
         Here, :math:`{\rm d}\theta` is the measured angle error from the fit. The duration of
         the single qubit-gate is :math:`\tau` in samples and :math:`{\rm d}t` is the duration
         of a sample. This is also the duration of the time unit ``dt`` of the delay.
         """
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/frequency_cal.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/frequency_cal.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,49 +20,50 @@
 from qiskit_experiments.framework import ExperimentData
 from qiskit_experiments.library.characterization.ramsey_xy import RamseyXY
 from qiskit_experiments.calibration_management.calibrations import Calibrations
 from qiskit_experiments.calibration_management.update_library import BaseUpdater
 from qiskit_experiments.calibration_management.base_calibration_experiment import (
     BaseCalibrationExperiment,
 )
-from qiskit_experiments.warnings import qubit_deprecate
 
 
 class FrequencyCal(BaseCalibrationExperiment, RamseyXY):
     """A qubit frequency calibration experiment based on the Ramsey XY experiment."""
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         calibrations: Calibrations,
         backend: Optional[Backend] = None,
+        cal_parameter_name: Optional[str] = "drive_freq",
         delays: Optional[List] = None,
         osc_freq: float = 2e6,
         auto_update: bool = True,
     ):
         """
         Args:
             physical_qubits: Sequence containing the qubit on which to run the
                 frequency calibration.
             calibrations: The calibrations instance with the schedules.
             backend: Optional, the backend to run the experiment on.
+            cal_parameter_name: The name of the parameter to update in the calibrations.
+                This defaults to `drive_freq`.
             delays: The list of delays that will be scanned in the experiment, in seconds.
             osc_freq: A frequency shift in Hz that will be applied by means of
                 a virtual Z rotation to increase the frequency of the measured oscillation.
             auto_update: If set to True, which is the default, then the experiment will
                 automatically update the frequency in the calibrations.
         """
         super().__init__(
             calibrations,
             physical_qubits,
             backend=backend,
             delays=delays,
             osc_freq=osc_freq,
-            cal_parameter_name=calibrations.__drive_freq_parameter__,
+            cal_parameter_name=cal_parameter_name,
             auto_update=auto_update,
         )
 
     def _metadata(self) -> Dict[str, any]:
         """Add the oscillation frequency of the experiment to the metadata."""
         metadata = super()._metadata()
         metadata["osc_freq"] = self.experiment_options.osc_freq
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/half_angle_cal.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/rough_drag_cal.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,122 +6,114 @@
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-"""Half angle calibration."""
+"""Rough drag calibration experiment."""
 
-from typing import Dict, Optional, Sequence
-import numpy as np
+from typing import Dict, Iterable, Optional, Sequence
 
-from qiskit.circuit import QuantumCircuit
+from qiskit.circuit import Parameter, QuantumCircuit
 from qiskit.providers.backend import Backend
 
 from qiskit_experiments.framework import ExperimentData
 from qiskit_experiments.calibration_management import (
     BaseCalibrationExperiment,
     Calibrations,
 )
-from qiskit_experiments.library.characterization import HalfAngle
 from qiskit_experiments.calibration_management.update_library import BaseUpdater
-from qiskit_experiments.warnings import qubit_deprecate
+from qiskit_experiments.library.characterization.drag import RoughDrag
 
 
-class HalfAngleCal(BaseCalibrationExperiment, HalfAngle):
-    """Calibration version of the half-angle experiment."""
+class RoughDragCal(BaseCalibrationExperiment, RoughDrag):
+    """A calibration version of the :class:`.RoughDrag` experiment.
+
+    # section: manual
+        :ref:`DRAG Calibration`
+
+    """
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         calibrations: Calibrations,
         backend: Optional[Backend] = None,
-        schedule_name: str = "sx",
-        cal_parameter_name: Optional[str] = "amp",
+        schedule_name: str = "x",
+        betas: Iterable[float] = None,
+        cal_parameter_name: Optional[str] = "β",
         auto_update: bool = True,
+        group: str = "default",
     ):
-        """see class :class:`HalfAngle` for details.
+        r"""see class :class:`.RoughDrag` for details.
 
         Args:
             physical_qubits: Sequence containing the qubit for which to run the
-                half-angle calibration.
+                rough DRAG calibration.
             calibrations: The calibrations instance with the schedules.
             backend: Optional, the backend to run the experiment on.
-            schedule_name: The name of the schedule to calibrate which defaults to sx.
-            cal_parameter_name: The name of the parameter in the schedule to update. This will
-                default to amp since the complex amplitude contains the phase of the pulse.
-            auto_update:  Whether or not to automatically update the calibrations. By
+            schedule_name: The name of the schedule to calibrate. Defaults to "x".
+            betas: A list of DRAG parameter values to scan. If None is given 51 betas ranging
+                from -5 to 5 will be scanned.
+            cal_parameter_name: The name of the parameter in the schedule to update.
+                Defaults to "β".
+            auto_update: Whether or not to automatically update the calibrations. By
                 default this variable is set to True.
+            group: The group of calibration parameters to use. The default value is "default".
         """
+        qubit = physical_qubits[0]
+        schedule = calibrations.get_schedule(
+            schedule_name, qubit, assign_params={cal_parameter_name: Parameter("β")}, group=group
+        )
+
+        self._validate_channels(schedule, [qubit])
+        self._validate_parameters(schedule, 1)
+
         super().__init__(
             calibrations,
             physical_qubits,
+            schedule=schedule,
+            betas=betas,
             backend=backend,
             schedule_name=schedule_name,
             cal_parameter_name=cal_parameter_name,
             auto_update=auto_update,
         )
 
     def _metadata(self) -> Dict[str, any]:
         """Add metadata to the experiment data making it more self contained.
 
-        The following keys are added to the experiment's metadata:
-            cal_param_value: The value of the pulse amplitude. This value together with
-                the fit result will be used to find the new value of the pulse amplitude.
+        The following keys are added to each experiment's metadata:
+            cal_param_value: The value of the previous calibrated beta.
             cal_param_name: The name of the parameter in the calibrations.
             cal_schedule: The name of the schedule in the calibrations.
             cal_group: The calibration group to which the parameter belongs.
         """
         metadata = super()._metadata()
         metadata["cal_param_value"] = self._cals.get_parameter_value(
-            self._param_name,
-            self._physical_qubits,
-            self._sched_name,
-            group=self.experiment_options.group,
+            self._param_name, self.physical_qubits, self._sched_name, self.experiment_options.group
         )
-
         return metadata
 
     def _attach_calibrations(self, circuit: QuantumCircuit):
-        """Adds the calibrations to the transpiled circuits."""
-        for gate in ["y", "sx"]:
-            schedule = self._cals.get_schedule(gate, self.physical_qubits)
-            circuit.add_calibration(gate, self.physical_qubits, schedule)
+        """RoughDrag already has the schedules attached in the program circuits."""
+        pass
 
     def update_calibrations(self, experiment_data: ExperimentData):
-        r"""Update the value of the parameter in the calibrations.
+        """Update the beta using the value directly reported from the fit.
 
-        The parameter that is updated is the phase of the sx pulse. This phase is contained
-        in the complex amplitude of the pulse. The update rule for the half angle calibration is
-        therefore:
-
-        ..math::
-
-            A \to A \cdot e^{-i{\rm d}\theta_\text{hac}/2}
-
-        where :math:`A` is the complex amplitude of the sx pulse which has an angle which might be
-        different from the angle of the x pulse due to the non-linearity in the mixer's skew. The
-        angle :math:`{\rm d}\theta_\text{hac}` is the angle deviation measured through the error
-        amplifying pulse sequence.
-
-        Args:
-            experiment_data: The experiment data from which to extract the measured over/under
-                rotation used to adjust the amplitude.
+        See :class:`.DragCalAnalysis` for details on the fit.
         """
 
-        result_index = self.experiment_options.result_index
-        group = experiment_data.metadata["cal_group"]
-        prev_amp = experiment_data.metadata["cal_param_value"]
-
-        d_theta = BaseUpdater.get_value(experiment_data, "d_hac", result_index)
-        new_amp = prev_amp * np.exp(-1.0j * d_theta / 2)
+        new_beta = BaseUpdater.get_value(
+            experiment_data, "beta", self.experiment_options.result_index
+        )
 
         BaseUpdater.add_parameter_value(
             self._cals,
             experiment_data,
-            new_amp,
+            new_beta,
             self._param_name,
             self._sched_name,
-            group,
+            self.experiment_options.group,
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/rough_amplitude_cal.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/rough_amplitude_cal.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,25 +20,23 @@
 from qiskit.circuit import Parameter
 from qiskit.providers.backend import Backend
 
 from qiskit_experiments.framework import ExperimentData
 from qiskit_experiments.calibration_management import BaseCalibrationExperiment, Calibrations
 from qiskit_experiments.library.characterization import Rabi
 from qiskit_experiments.calibration_management.update_library import BaseUpdater
-from qiskit_experiments.warnings import qubit_deprecate
 
 AnglesSchedules = namedtuple(
     "AnglesSchedules", ["target_angle", "parameter", "schedule", "previous_value"]
 )
 
 
 class RoughAmplitudeCal(BaseCalibrationExperiment, Rabi):
     """A calibration version of the Rabi experiment."""
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         calibrations: Calibrations,
         schedule_name: str = "x",
         amplitudes: Iterable[float] = None,
         cal_parameter_name: Optional[str] = "amp",
@@ -178,25 +176,25 @@
         result_index = self.experiment_options.result_index
         group = experiment_data.metadata["cal_group"]
 
         rate = 2 * np.pi * BaseUpdater.get_value(experiment_data, self.__outcome__, result_index)
 
         for angle, param, schedule, prev_amp in experiment_data.metadata["angles_schedules"]:
 
-            value = np.round(angle / rate, decimals=8) * np.exp(1.0j * np.angle(prev_amp))
+            # This implementation conserves the type, while working for both real and complex prev_amp
+            value = np.round(angle / rate, decimals=8) * prev_amp / np.abs(prev_amp)
 
             BaseUpdater.add_parameter_value(
                 self._cals, experiment_data, value, param, schedule, group
             )
 
 
 class RoughXSXAmplitudeCal(RoughAmplitudeCal):
     """A rough amplitude calibration of x and sx gates."""
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         calibrations: Calibrations,
         amplitudes: Iterable[float] = None,
         backend: Optional[Backend] = None,
     ):
@@ -222,15 +220,14 @@
 class EFRoughXSXAmplitudeCal(RoughAmplitudeCal):
     r"""A rough amplitude calibration of :math:`X` and :math:`SX` gates on the
     :math:`|1\rangle` <-> :math:`|2\rangle` transition.
     """
 
     __outcome__ = "rabi_rate_12"
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         calibrations: Calibrations,
         amplitudes: Iterable[float] = None,
         backend: Optional[Backend] = None,
         ef_pulse_label: str = "12",
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/rough_drag_cal.py` & `qiskit-experiments-0.6.0/qiskit_experiments/framework/analysis_result_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,116 +6,135 @@
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-"""Rough drag calibration experiment."""
+"""Helper dataclass for constructing analysis results."""
 
-from typing import Dict, Iterable, Optional, Sequence
-
-from qiskit.circuit import Parameter, QuantumCircuit
-from qiskit.providers.backend import Backend
-
-from qiskit_experiments.framework import ExperimentData
-from qiskit_experiments.calibration_management import (
-    BaseCalibrationExperiment,
-    Calibrations,
-)
-from qiskit_experiments.calibration_management.update_library import BaseUpdater
-from qiskit_experiments.library.characterization.drag import RoughDrag
-from qiskit_experiments.warnings import qubit_deprecate
-
-
-class RoughDragCal(BaseCalibrationExperiment, RoughDrag):
-    """A calibration version of the :class:`.RoughDrag` experiment.
-
-    # section: manual
-        :ref:`DRAG Calibration`
-
-    """
-
-    @qubit_deprecate()
-    def __init__(
-        self,
-        physical_qubits: Sequence[int],
-        calibrations: Calibrations,
-        backend: Optional[Backend] = None,
-        schedule_name: str = "x",
-        betas: Iterable[float] = None,
-        cal_parameter_name: Optional[str] = "β",
-        auto_update: bool = True,
-        group: str = "default",
+import dataclasses
+import logging
+from typing import Optional, Dict, Any, List
+
+from qiskit_experiments.database_service.device_component import DeviceComponent
+
+
+LOG = logging.getLogger(__name__)
+
+
+@dataclasses.dataclass
+class AnalysisResultData:
+    """Dataclass for experiment analysis results"""
+
+    name: str
+    value: Any
+    experiment: str = None
+    chisq: Optional[float] = None
+    quality: Optional[str] = None
+    experiment_id: Optional[str] = None
+    result_id: Optional[str] = None
+    tags: List = dataclasses.field(default_factory=list)
+    backend: Optional[str] = None
+    run_time: Optional[str] = None
+    created_time: Optional[str] = None
+    extra: Dict[str, Any] = dataclasses.field(default_factory=dict, hash=False, compare=False)
+    device_components: List = dataclasses.field(default_factory=list)
+
+    @classmethod
+    def from_table_element(
+        cls,
+        name: str,
+        value: Any,
+        experiment: Optional[str] = None,
+        components: Optional[List[DeviceComponent]] = None,
+        quality: Optional[str] = None,
+        experiment_id: Optional[str] = None,
+        result_id: Optional[str] = None,
+        tags: Optional[List[str]] = None,
+        backend: Optional[str] = None,
+        run_time: Optional[str] = None,
+        created_time: Optional[str] = None,
+        **extra,
     ):
-        r"""see class :class:`.RoughDrag` for details.
+        """A factory method of AnalysisResultData from a single element in AnalysisResultTable.
 
         Args:
-            physical_qubits: Sequence containing the qubit for which to run the
-                rough DRAG calibration.
-            calibrations: The calibrations instance with the schedules.
-            backend: Optional, the backend to run the experiment on.
-            schedule_name: The name of the schedule to calibrate. Defaults to "x".
-            betas: A list of DRAG parameter values to scan. If None is given 51 betas ranging
-                from -5 to 5 will be scanned.
-            cal_parameter_name: The name of the parameter in the schedule to update.
-                Defaults to "β".
-            auto_update: Whether or not to automatically update the calibrations. By
-                default this variable is set to True.
-            group: The group of calibration parameters to use. The default value is "default".
+            name: Name of this entity.
+            value: Result value.
+            experiment: Type of experiment.
+            components: Device component that the experiment was run on.
+            quality: Quality of this result.
+            experiment_id: ID of associated experiment.
+            result_id: Unique ID of this data entry in the storage.
+            tags: List of tags.
+            backend: Device name that the experiment was run on.
+            run_time: A time at the experiment was run.
+            created_time: A time at this value was computed.
+            **extra: Extra information.
         """
-        qubit = physical_qubits[0]
-        schedule = calibrations.get_schedule(
-            schedule_name, qubit, assign_params={cal_parameter_name: Parameter("β")}, group=group
-        )
-
-        self._validate_channels(schedule, [qubit])
-        self._validate_parameters(schedule, 1)
+        chisq = extra.pop("chisq", None)
 
-        super().__init__(
-            calibrations,
-            physical_qubits,
-            schedule=schedule,
-            betas=betas,
+        return AnalysisResultData(
+            name=name,
+            value=value,
+            experiment=experiment,
+            chisq=chisq,
+            quality=quality,
+            experiment_id=experiment_id,
+            result_id=result_id,
+            tags=tags,
             backend=backend,
-            schedule_name=schedule_name,
-            cal_parameter_name=cal_parameter_name,
-            auto_update=auto_update,
+            run_time=run_time,
+            created_time=created_time,
+            device_components=components,
+            extra=extra,
         )
 
-    def _metadata(self) -> Dict[str, any]:
-        """Add metadata to the experiment data making it more self contained.
+    def __str__(self):
+        out = f"{self.name}:"
+        out += f"\n- value:{self.value}"
+        if self.chisq is not None:
+            out += f"\n- chisq: {self.chisq}"
+        if self.quality is not None:
+            out += f"\n- quality: {self.quality}"
+        if self.extra:
+            out += f"\n- extra: <{len(self.extra)} items>"
+        if self.device_components:
+            out += f"\n- device_components: {[str(i) for i in self.device_components]}"
+        return out
+
+    def __iter__(self):
+        """Return iterator of data fields (attr, value)"""
+        return iter((field.name, getattr(self, field.name)) for field in dataclasses.fields(self))
+
+
+def as_table_element(
+    result_data: AnalysisResultData,
+) -> Dict[str, Any]:
+    """Python dataclass as_dict-like function to return
+    canonical data for analysis AnalysisResultTable.
 
-        The following keys are added to each experiment's metadata:
-            cal_param_value: The value of the previous calibrated beta.
-            cal_param_name: The name of the parameter in the calibrations.
-            cal_schedule: The name of the schedule in the calibrations.
-            cal_group: The calibration group to which the parameter belongs.
-        """
-        metadata = super()._metadata()
-        metadata["cal_param_value"] = self._cals.get_parameter_value(
-            self._param_name, self.physical_qubits, self._sched_name, self.experiment_options.group
-        )
-        return metadata
-
-    def _attach_calibrations(self, circuit: QuantumCircuit):
-        """RoughDrag already has the schedules attached in the program circuits."""
-        pass
+    Args:
+        result_data: AnalysisResultData dataclass to format.
 
-    def update_calibrations(self, experiment_data: ExperimentData):
-        """Update the beta using the value directly reported from the fit.
-
-        See :class:`DragCalAnalysis` for details on the fit.
-        """
-
-        new_beta = BaseUpdater.get_value(
-            experiment_data, "beta", self.experiment_options.result_index
-        )
+    Returns:
+        Formatted data representation in dictionary format.
+    """
+    out = {
+        "name": result_data.name,
+        "experiment": result_data.experiment,
+        "components": result_data.device_components,
+        "value": result_data.value,
+        "quality": result_data.quality,
+        "experiment_id": result_data.experiment_id,
+        "result_id": result_data.result_id,
+        "tags": result_data.tags,
+        "backend": result_data.backend,
+        "run_time": result_data.run_time,
+        "created_time": result_data.created_time,
+    }
+    if result_data.chisq is not None:
+        out["chisq"] = result_data.chisq
+    out.update(result_data.extra)
 
-        BaseUpdater.add_parameter_value(
-            self._cals,
-            experiment_data,
-            new_beta,
-            self._param_name,
-            self._sched_name,
-            self.experiment_options.group,
-        )
+    return out
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/calibration/rough_frequency.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/calibration/rough_frequency.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,56 +20,58 @@
 from qiskit_experiments.library.characterization.qubit_spectroscopy import QubitSpectroscopy
 from qiskit_experiments.library.characterization.ef_spectroscopy import EFSpectroscopy
 from qiskit_experiments.calibration_management.update_library import Frequency
 from qiskit_experiments.calibration_management.calibrations import Calibrations
 from qiskit_experiments.calibration_management.base_calibration_experiment import (
     BaseCalibrationExperiment,
 )
-from qiskit_experiments.warnings import qubit_deprecate
 
 
 class RoughFrequencyCal(BaseCalibrationExperiment, QubitSpectroscopy):
     """A calibration experiment that runs :class:`.QubitSpectroscopy` to calibrate the qubit
     transition frequency."""
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         calibrations: Calibrations,
         frequencies: Iterable[float],
         backend: Optional[Backend] = None,
         auto_update: bool = True,
         absolute: bool = True,
+        cal_parameter_name: Optional[str] = "drive_freq",
     ):
         """See :class:`.QubitSpectroscopy` for detailed documentation.
 
         Args:
             physical_qubits: List with the qubit on which to run spectroscopy.
             calibrations: If calibrations is given then running the experiment may update the values
                 of the frequencies stored in calibrations.
             frequencies: The frequencies to scan in the experiment, in Hz.
             backend: Optional, the backend to run the experiment on.
             auto_update: If set to True, which is the default, then the experiment will
                 automatically update the frequency in the calibrations.
             absolute: Boolean to specify if the frequencies are absolute or relative to the
                 qubit frequency in the backend.
+            cal_parameter_name: The name of the parameter to update in the calibrations.
+                This defaults to `drive_freq`.
 
         Raises:
             QiskitError: If there are less than three frequency shifts.
 
         """
         super().__init__(
             calibrations,
             physical_qubits,
             frequencies,
             backend=backend,
             absolute=absolute,
             updater=Frequency,
             auto_update=auto_update,
+            cal_parameter_name=cal_parameter_name,
         )
 
     def _attach_calibrations(self, circuit: QuantumCircuit):
         """QubitSpectroscopy already has the schedules attached in the program circuits."""
         pass
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 """Analysis Classes"""
 
 from .drag_analysis import DragCalAnalysis
 from .fine_amplitude_analysis import FineAmplitudeAnalysis
 from .ramsey_xy_analysis import RamseyXYAnalysis
 from .t2ramsey_analysis import T2RamseyAnalysis
 from .t2hahn_analysis import T2HahnAnalysis
-from .t1_analysis import T1Analysis
-from .t1_analysis import T1KerneledAnalysis
+from .t1_analysis import T1Analysis, T1KerneledAnalysis
 from .tphi_analysis import TphiAnalysis
 from .cr_hamiltonian_analysis import CrossResonanceHamiltonianAnalysis
 from .readout_angle_analysis import ReadoutAngleAnalysis
 from .local_readout_error_analysis import LocalReadoutErrorAnalysis
 from .correlated_readout_error_analysis import CorrelatedReadoutErrorAnalysis
 from .resonator_spectroscopy_analysis import ResonatorSpectroscopyAnalysis
 from .zz_ramsey_analysis import ZZRamseyAnalysis
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/correlated_readout_error_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/correlated_readout_error_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         This class generates the full assignment matrix :math:`A` characterizing the
         readout error for the given qubits from the experiment results
         and returns the resulting :class:`~qiskit.result.CorrelatedReadoutMitigator`
 
         :math:`A` is a :math:`2^n\times 2^n` matrix :math:`A` such that :math:`A_{y,x}`
         is the probability to observe :math:`y` given the true outcome should be :math:`x`.
 
-        In the experiment, for each :math:`x`a circuit is constructed whose expected
+        In the experiment, for each :math:`x` a circuit is constructed whose expected
         outcome is :math:`x`. From the observed results on the circuit, the probability for
         each :math:`y` is determined, and :math:`A_{y,x}` is set accordingly.
 
         Analysis Results:
            * "Local Readout Mitigator": The :class:`~qiskit.result.LocalReadoutMitigator`.
 
         Analysis Figures:
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/cr_hamiltonian_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/cr_hamiltonian_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/drag_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/drag_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,29 +100,29 @@
             )
             del fields["reps"]
         super().set_options(**fields)
 
     def _generate_fit_guesses(
         self,
         user_opt: curve.FitOptions,
-        curve_data: curve.CurveData,
+        curve_data: curve.ScatterTable,
     ) -> Union[curve.FitOptions, List[curve.FitOptions]]:
         """Create algorithmic initial fit guess from analysis options and curve data.
 
         Args:
             user_opt: Fit options filled with user provided guess and bounds.
             curve_data: Formatted data collection to fit.
 
         Returns:
             List of fit options that are passed to the fitter function.
         """
         # Use the highest-frequency curve to estimate the oscillation frequency.
-        max_rep_model_name = self._models[-1]._name
+        max_rep_model_name = self.model_names()[-1]
         max_rep = self.options.data_subfit_map[max_rep_model_name]["nrep"]
-        curve_data = curve_data.get_subset_of(max_rep_model_name)
+        curve_data = curve_data.filter(series=max_rep_model_name)
 
         x_data = curve_data.x
         min_beta, max_beta = min(x_data), max(x_data)
 
         freqs_guess = curve.guess.frequency(curve_data.x, curve_data.y) / max_rep
         user_opt.p0.set_if_empty(freq=freqs_guess)
 
@@ -152,16 +152,15 @@
                 new_opt.p0.set_if_empty(amp=ptp_y * amp_factor, beta=beta_guess)
                 options.append(new_opt)
 
         return options
 
     def _run_curve_fit(
         self,
-        curve_data: curve.CurveData,
-        models: List[lmfit.Model],
+        curve_data: curve.ScatterTable,
     ) -> curve.CurveFitResult:
         r"""Perform curve fitting on given data collection and fit models.
 
         .. note::
 
             This class post-processes the fit result from a Drag analysis.
 
@@ -183,43 +182,41 @@
 
             .. math::
 
                 \beta = \beta_\text{fit} + n_\text{min} / {\rm freq}.
 
         Args:
             curve_data: Formatted data to fit.
-            models: A list of LMFIT models that are used to build a cost function
-                for the LMFIT minimizer.
 
         Returns:
             The best fitting outcome with minimum reduced chi-squared value.
         """
-        fit_result = super()._run_curve_fit(curve_data, models)
+        fit_result = super()._run_curve_fit(curve_data)
 
         if fit_result and fit_result.params is not None:
             beta = fit_result.params["beta"]
             freq = fit_result.params["freq"]
             min_beta = ((beta + 1 / freq / 2) % (1 / freq)) - 1 / freq / 2
             fit_result.params["beta"] = min_beta
 
         return fit_result
 
     def _evaluate_quality(self, fit_data: curve.CurveFitResult) -> Union[str, None]:
         """Algorithmic criteria for whether the fit is good or bad.
 
         A good fit has:
-            - a reduced chi-squared lower than three,
+            - a reduced chi-squared lower than three and greater than zero,
             - a DRAG parameter value within the first period of the lowest number of repetitions,
             - an error on the drag beta smaller than the beta.
         """
         fit_beta = fit_data.ufloat_params["beta"]
         fit_freq = fit_data.ufloat_params["freq"]
 
         criteria = [
-            fit_data.reduced_chisq < 3,
+            0 < fit_data.reduced_chisq < 3,
             abs(fit_beta.nominal_value) < 1 / fit_freq.nominal_value / 2,
             curve.utils.is_error_not_significant(fit_beta),
         ]
 
         if all(criteria):
             return "good"
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/fine_amplitude_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/fine_amplitude_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/local_readout_error_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/local_readout_error_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/multi_state_discrimination_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/multi_state_discrimination_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/ramsey_xy_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/ramsey_xy_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,27 +98,27 @@
         default_options.result_parameters = ["freq"]
 
         return default_options
 
     def _generate_fit_guesses(
         self,
         user_opt: curve.FitOptions,
-        curve_data: curve.CurveData,
+        curve_data: curve.ScatterTable,
     ) -> Union[curve.FitOptions, List[curve.FitOptions]]:
         """Create algorithmic initial fit guess from analysis options and curve data.
 
         Args:
             user_opt: Fit options filled with user provided guess and bounds.
             curve_data: Formatted data collection to fit.
 
         Returns:
             List of fit options that are passed to the fitter function.
         """
-        ramx_data = curve_data.get_subset_of("X")
-        ramy_data = curve_data.get_subset_of("Y")
+        ramx_data = curve_data.filter(series="X")
+        ramy_data = curve_data.filter(series="Y")
 
         # At very low frequency, y value of X (Y) curve stay at P=1.0 (0.5) for all x values.
         # Computing y peak-to-peak with combined data gives fake amplitude of 0.25.
         # Same for base, i.e. P=0.75 is often estimated in this case.
         full_y_ptp = np.ptp(curve_data.y)
         avg_y_ptp = 0.5 * (np.ptp(ramx_data.y) + np.ptp(ramy_data.y))
         max_y = np.max(curve_data.y)
@@ -188,21 +188,21 @@
 
         return opts
 
     def _evaluate_quality(self, fit_data: curve.CurveFitResult) -> Union[str, None]:
         """Algorithmic criteria for whether the fit is good or bad.
 
         A good fit has:
-            - a reduced chi-squared lower than three,
+            - a reduced chi-squared lower than three and greater than zero,
             - an error on the frequency smaller than the frequency.
         """
         fit_freq = fit_data.ufloat_params["freq"]
 
         criteria = [
-            fit_data.reduced_chisq < 3,
+            0 < fit_data.reduced_chisq < 3,
             curve.utils.is_error_not_significant(fit_freq),
         ]
 
         if all(criteria):
             return "good"
 
         return "bad"
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/readout_angle_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/readout_angle_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/resonator_spectroscopy_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/resonator_spectroscopy_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/t1_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/t1_analysis.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,19 +11,17 @@
 # that they have been altered from the originals.
 """
 T1 Analysis class.
 """
 from typing import Union
 
 import numpy as np
-from uncertainties import unumpy as unp
 
 import qiskit_experiments.curve_analysis as curve
 from qiskit_experiments.framework import Options
-from qiskit_experiments.curve_analysis.curve_data import CurveData
 
 
 class T1Analysis(curve.DecayAnalysis):
     """A class to analyze T1 experiments."""
 
     @classmethod
     def _default_options(cls) -> Options:
@@ -38,27 +36,27 @@
 
         return options
 
     def _evaluate_quality(self, fit_data: curve.CurveFitResult) -> Union[str, None]:
         """Algorithmic criteria for whether the fit is good or bad.
 
         A good fit has:
-            - a reduced chi-squared lower than three
+            - a reduced chi-squared lower than three and greater than zero
             - absolute amp is within [0.9, 1.1]
             - base is less than 0.1
             - amp error is less than 0.1
             - tau error is less than its value
             - base error is less than 0.1
         """
         amp = fit_data.ufloat_params["amp"]
         tau = fit_data.ufloat_params["tau"]
         base = fit_data.ufloat_params["base"]
 
         criteria = [
-            fit_data.reduced_chisq < 3,
+            0 < fit_data.reduced_chisq < 3,
             abs(amp.nominal_value - 1.0) < 0.1,
             abs(base.nominal_value) < 0.1,
             curve.utils.is_error_not_significant(amp, absolute=0.1),
             curve.utils.is_error_not_significant(tau),
             curve.utils.is_error_not_significant(base, absolute=0.1),
         ]
 
@@ -85,60 +83,52 @@
 
         return options
 
     def _evaluate_quality(self, fit_data: curve.CurveFitResult) -> Union[str, None]:
         """Algorithmic criteria for whether the fit is good or bad.
 
         A good fit has:
-            - a reduced chi-squared lower than three
+            - a reduced chi-squared lower than three and greater than zero
             - absolute amp is within [0.9, 1.1]
             - base is less than 0.1
             - amp error is less than 0.1
             - tau error is less than its value
             - base error is less than 0.1
         """
         amp = fit_data.ufloat_params["amp"]
         tau = fit_data.ufloat_params["tau"]
         base = fit_data.ufloat_params["base"]
 
         criteria = [
-            fit_data.reduced_chisq < 3,
+            0 < fit_data.reduced_chisq < 3,
             abs(amp.nominal_value - 1.0) < 0.1,
             abs(base.nominal_value) < 0.1,
             curve.utils.is_error_not_significant(amp, absolute=0.1),
             curve.utils.is_error_not_significant(tau),
             curve.utils.is_error_not_significant(base, absolute=0.1),
         ]
 
         if all(criteria):
             return "good"
 
         return "bad"
 
     def _format_data(
         self,
-        curve_data: curve.CurveData,
-    ) -> curve.CurveData:
-        """Postprocessing for the processed dataset.
+        curve_data: curve.ScatterTable,
+        category: str = "formatted",
+    ) -> curve.ScatterTable:
+        """Postprocessing for preparing the fitting data.
 
         Args:
             curve_data: Processed dataset created from experiment results.
+            category: Category string of the output dataset.
 
         Returns:
-            Formatted data.
+            New scatter table instance including fit data.
         """
         # check if the SVD decomposition categorized 0 as 1 by calculating the average slope
-        diff_y = np.diff(unp.nominal_values(curve_data.y), axis=0)
+        diff_y = np.diff(curve_data.y)
         avg_slope = sum(diff_y) / len(diff_y)
-        if avg_slope[0] > 0:
-            new_y_data = 1 - curve_data.y
-            new_curve_data = CurveData(
-                x=curve_data.x,
-                y=new_y_data,
-                y_err=curve_data.y_err,
-                shots=curve_data.shots,
-                data_allocation=curve_data.data_allocation,
-                labels=curve_data.labels,
-            )
-
-            return super()._format_data(new_curve_data)
+        if avg_slope > 0:
+            curve_data.y = 1 - curve_data.y
         return super()._format_data(curve_data)
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/t2hahn_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/t2hahn_analysis.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,27 +46,27 @@
 
         return options
 
     def _evaluate_quality(self, fit_data: curve.CurveFitResult) -> Union[str, None]:
         """Algorithmic criteria for whether the fit is good or bad.
 
         A good fit has:
-            - a reduced chi-squared lower than three
+            - a reduced chi-squared lower than three and greater than zero
             - absolute amp is within [0.4, 0.6]
             - base is less is within [0.4, 0.6]
             - amp error is less than 0.1
             - tau error is less than its value
             - base error is less than 0.1
         """
         amp = fit_data.ufloat_params["amp"]
         tau = fit_data.ufloat_params["tau"]
         base = fit_data.ufloat_params["base"]
 
         criteria = [
-            fit_data.reduced_chisq < 3,
+            0 < fit_data.reduced_chisq < 3,
             abs(amp.nominal_value - 0.5) < 0.1,
             abs(base.nominal_value - 0.5) < 0.1,
             curve.utils.is_error_not_significant(amp, absolute=0.1),
             curve.utils.is_error_not_significant(tau),
             curve.utils.is_error_not_significant(base, absolute=0.1),
         ]
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/t2ramsey_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/t2ramsey_analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,25 +37,25 @@
 
         return options
 
     def _evaluate_quality(self, fit_data: curve.CurveFitResult) -> Union[str, None]:
         """Algorithmic criteria for whether the fit is good or bad.
 
         A good fit has:
-            - a reduced chi-squared lower than three
+            - a reduced chi-squared lower than three and greater than zero
             - relative error of amp is less than 10 percent
             - relative error of tau is less than 10 percent
             - relative error of freq is less than 10 percent
         """
         amp = fit_data.ufloat_params["amp"]
         tau = fit_data.ufloat_params["tau"]
         freq = fit_data.ufloat_params["freq"]
 
         criteria = [
-            fit_data.reduced_chisq < 3,
+            0 < fit_data.reduced_chisq < 3,
             curve.utils.is_error_not_significant(amp, fraction=0.1),
             curve.utils.is_error_not_significant(tau, fraction=0.1),
             curve.utils.is_error_not_significant(freq, fraction=0.1),
         ]
 
         if all(criteria):
             return "good"
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/tphi_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/tphi_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/analysis/zz_ramsey_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/analysis/zz_ramsey_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,20 @@
 
 import lmfit
 import numpy as np
 
 from qiskit.providers.options import Options
 
 import qiskit_experiments.curve_analysis as curve
-from qiskit_experiments.curve_analysis import CurveAnalysis, CurveData, CurveFitResult, FitOptions
+from qiskit_experiments.curve_analysis import (
+    CurveAnalysis,
+    ScatterTable,
+    CurveFitResult,
+    FitOptions,
+)
 from qiskit_experiments.curve_analysis.utils import is_error_not_significant
 
 
 class ZZRamseyAnalysis(CurveAnalysis):
     # Disable long line check because we can't break the long math lines
     # pylint: disable=line-too-long
     r"""A class to analyze a :math:`ZZ` Ramsey experiment.
@@ -117,15 +122,15 @@
         }
 
         return default_options
 
     def _generate_fit_guesses(
         self,
         user_opt: FitOptions,
-        curve_data: CurveData,
+        curve_data: ScatterTable,
     ) -> Union[FitOptions, List[FitOptions]]:
         """Compute the initial guesses.
 
         Args:
             user_opt: Fit options filled with user provided guess and bounds.
             curve_data: Preprocessed data to be fit.
 
@@ -133,16 +138,16 @@
             List of fit options that are passed to the fitter function.
         """
         y_max = np.max(curve_data.y)
         y_min = np.min(curve_data.y)
         y_ptp = y_max - y_min
         x_max = np.max(curve_data.x)
 
-        data_0 = curve_data.get_subset_of("0")
-        data_1 = curve_data.get_subset_of("1")
+        data_0 = curve_data.filter(series="0")
+        data_1 = curve_data.filter(series="1")
 
         def typical_step(arr):
             """Find the typical step size of an array"""
             steps = np.diff(np.sort(arr))
             # If points are not unique, there will be 0's that don't count as
             # steps
             steps = steps[steps != 0]
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/correlated_readout_error.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/correlated_readout_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 """
 Correlated readout error calibration experiment class.
 """
 from typing import Iterable, List, Optional
 from qiskit import QuantumCircuit
 from qiskit.providers.backend import BackendV2, Backend
 from qiskit.exceptions import QiskitError
-from qiskit_experiments.warnings import deprecate_arguments
 from qiskit_experiments.framework import BaseExperiment
 from qiskit_experiments.library.characterization.analysis.correlated_readout_error_analysis import (
     CorrelatedReadoutErrorAnalysis,
 )
 
 
 def calibration_circuit(num_qubits: int, state_label: str) -> QuantumCircuit:
@@ -70,19 +69,21 @@
 
         See :class:`CorrelatedReadoutErrorAnalysis`
         documentation for additional information on correlated readout error experiment analysis.
 
     # section: analysis_ref
         :class:`CorrelatedReadoutErrorAnalysis`
 
+    # section: manual
+        :doc:`/manuals/measurement/readout_mitigation`
+
     # section: reference
         .. ref_arxiv:: 1 2006.14044
     """
 
-    @deprecate_arguments({"qubits": "physical_qubits"}, "0.5")
     def __init__(
         self,
         physical_qubits: Optional[Iterable[int]] = None,
         backend: Optional[Backend] = None,
     ):
         """Initialize a correlated readout error characterization experiment.
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/cr_hamiltonian.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/cr_hamiltonian.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,21 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 """
 Cross resonance Hamiltonian tomography.
 """
 
-from typing import List, Tuple, Sequence, Iterable, Optional, Type
+from typing import List, Tuple, Sequence, Optional, Type
 
-import warnings
 import numpy as np
 from qiskit import pulse, circuit, QuantumCircuit
 from qiskit.circuit.parameterexpression import ParameterValueType
 from qiskit.exceptions import QiskitError
 from qiskit.providers import Backend
-from qiskit_experiments.warnings import deprecate_arguments
 from qiskit_experiments.framework import (
     BaseExperiment,
     BackendTiming,
     Options,
 )
 from qiskit_experiments.library.characterization.analysis import CrossResonanceHamiltonianAnalysis
 
@@ -120,45 +118,39 @@
         :class:`CrossResonanceHamiltonianAnalysis`
 
     # section: reference
         .. ref_arxiv:: 1 1603.04821
 
     # section: manual
         .. ref_website:: Qiskit Textbook 6.7,
-            https://qiskit.org/textbook/ch-quantum-hardware/hamiltonian-tomography.html
+            https://github.com/Qiskit/textbook/blob/main/notebooks/quantum-hardware-pulses/hamiltonian-tomography.ipynb
     """
 
     # Number of CR pulses. The flat top duration per pulse is divided by this number.
     num_pulses = 1
 
     class CRPulseGate(circuit.Gate):
         """A pulse gate of cross resonance. Definition should be provided via calibration."""
 
         def __init__(self, width: ParameterValueType):
             super().__init__("cr_gate", 2, [width])
 
-    @deprecate_arguments({"qubits": "physical_qubits"}, "0.5")
     def __init__(
         self,
         physical_qubits: Tuple[int, int],
-        flat_top_widths: Optional[Iterable[float]] = None,
         backend: Optional[Backend] = None,
         cr_gate: Optional[Type[circuit.Gate]] = None,
         durations: Optional[Sequence[int]] = None,
         **kwargs,
     ):
         """Create a new experiment.
 
         Args:
             physical_qubits: Two-value tuple of qubit indices on which to run tomography.
                 The first index stands for the control qubit.
-            flat_top_widths: Deprecated. The total duration of the square part of
-                cross resonance pulse(s) to scan, in units of dt.
-                The total pulse duration including Gaussian rising and falling edges is
-                implicitly computed with experiment parameters ``sigma`` and ``risefall``.
             backend: Optional, the backend to run the experiment on.
             cr_gate: Optional, circuit gate class representing the cross resonance pulse.
                 Providing this object allows us to run this experiment with circuit simulator,
                 and this object might be used for testing, development of analysis protocol,
                 and educational purpose without needing to wait for hardware queueing.
                 Note that this instance must provide matrix representation, such as
                 unitary gate or Hamiltonian gate, and the class is expected to be instantiated
@@ -185,61 +177,43 @@
         self._backend_timing = None
 
         super().__init__(
             physical_qubits, analysis=CrossResonanceHamiltonianAnalysis(), backend=backend
         )
         self.set_experiment_options(durations=durations, **kwargs)
 
-        if flat_top_widths is not None:
-            # TODO remove this in Qiskit Experiments 0.6
-            self.set_experiment_options(flat_top_widths=flat_top_widths)
-
     @classmethod
     def _default_experiment_options(cls) -> Options:
         """Default experiment options.
 
         Experiment Options:
-            flat_top_widths (np.ndarray): Deprecated. Length of Gaussian flat top to scan.
             durations (np.ndarray): The total duration of the cross resonance pulse(s) to scan,
                 in units of sec. Values should be longer than pulse ramps.
             min_durations (int): The minimum default pulse duration in samples.
             max_durations (int): The maximum default pulse duration in samples.
             num_durations (int): The number of measured durations. The experiment automatically
                 creates durations of linear increment along with ``min_durations`` and
                 ``max_durations`` when user doesn't explicitly provide ``durations``.
             amp (complex): Amplitude of the cross resonance tone.
             amp_t (complex): Amplitude of the cancellation or rotary drive on target qubit.
             sigma (float): Sigma of Gaussian rise and fall edges, in units of dt.
             risefall (float): Ratio of edge durations to sigma.
         """
         options = super()._default_experiment_options()
-        options.flat_top_widths = None  # to be removed in Qiskit Experiments 0.6
         options.durations = None
         options.min_durations = 60e-9
         options.max_durations = 1200e-9
         options.num_durations = 48
         options.amp = 0.5
         options.amp_t = 0.0
         options.sigma = 64
         options.risefall = 2
 
         return options
 
-    def set_experiment_options(self, **fields):
-        if "flat_top_widths" in fields:
-            # TODO remove this in Qiskit Experiments 0.6
-            warnings.warn(
-                "'flat_top_widths' argument has been deprecated and will be removed. "
-                "Use 'durations' instead. New variable includes pulse ramps, "
-                "and it cannot include zero in the sequence. "
-                "This argument will be dropped with this warning in Qiskit Experiments 0.6.",
-                DeprecationWarning,
-            )
-        super().set_experiment_options(**fields)
-
     def _set_backend(self, backend: Backend):
         """Set the backend for the experiment with timing analysis."""
         super()._set_backend(backend)
         self._backend_timing = BackendTiming(backend)
 
     def _get_dt(self) -> float:
         """A helper function to get finite dt.
@@ -265,19 +239,14 @@
 
         return duration - 2 * sigma_sec * self.experiment_options.risefall
 
     def _get_durations(self) -> np.ndarray:
         """Return cross resonance pulse durations in units of sec."""
         opt = self.experiment_options
 
-        if opt.flat_top_widths is not None:
-            # TODO Remove this in Qiskit Experiments 0.6
-            widths = np.asarray(opt.flat_top_widths, dtype=float)
-            return self._get_dt() * (widths + 2 * opt.sigma * opt.risefall)
-
         if opt.durations is None:
             return np.linspace(opt.min_durations, opt.max_durations, opt.num_durations)
 
         return np.asarray(opt.durations, dtype=float)
 
     def _build_cr_circuit(self, pulse_gate: circuit.Gate) -> QuantumCircuit:
         """Single tone cross resonance.
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/drag.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/drag.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from qiskit.exceptions import QiskitError
 from qiskit.providers.backend import Backend
 from qiskit.pulse import ScheduleBlock
 
 from qiskit_experiments.framework import BaseExperiment, Options
 from qiskit_experiments.framework.restless_mixin import RestlessMixin
 from qiskit_experiments.library.characterization.analysis import DragCalAnalysis
-from qiskit_experiments.warnings import qubit_deprecate
 
 
 class RoughDrag(BaseExperiment, RestlessMixin):
     r"""An experiment that scans the DRAG parameter to find the optimal value.
 
     # section: overview
 
@@ -89,15 +88,14 @@
         options = super()._default_experiment_options()
         options.schedule = None
         options.reps = [1, 3, 5]
         options.betas = np.linspace(-5, 5, 51)
 
         return options
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         schedule: ScheduleBlock,
         betas: Optional[Iterable[float]] = None,
         backend: Optional[Backend] = None,
     ):
@@ -164,21 +162,19 @@
             circuit.measure_active()
 
             circuit.add_calibration(
                 "Drag(" + schedule.name + ")", self.physical_qubits, schedule, params=[beta]
             )
 
             for beta_val in self.experiment_options.betas:
-                beta_val = np.round(beta_val, decimals=6)
+                beta_val = float(np.round(beta_val, decimals=6))
 
                 assigned_circuit = circuit.assign_parameters({beta: beta_val}, inplace=False)
 
                 assigned_circuit.metadata = {
-                    "experiment_type": self._type,
-                    "qubits": self.physical_qubits,
                     "xval": beta_val,
                     "nrep": rep,
                 }
 
                 circuits.append(assigned_circuit)
 
         return circuits
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/ef_spectroscopy.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/ef_spectroscopy.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from typing import Iterable, Optional, Sequence
 from qiskit import QuantumCircuit
 from qiskit.providers import Backend
 from qiskit.circuit import Gate
 
 from qiskit_experiments.curve_analysis import ParameterRepr
 from qiskit_experiments.library.characterization.qubit_spectroscopy import QubitSpectroscopy
-from qiskit_experiments.warnings import qubit_deprecate
 
 
 class EFSpectroscopy(QubitSpectroscopy):
     """A spectroscopy experiment to obtain a frequency sweep of the qubit's e-f transition.
 
     # section: overview
         The circuits produced by spectroscopy, i.e.
@@ -34,15 +33,14 @@
                   q_0: ┤ X ├┤ Spec(freq) ├─░─┤M├
                        └───┘└────────────┘ ░ └╥┘
             measure: 1/═══════════════════════╩═
                                               0
 
     """
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         frequencies: Iterable[float],
         backend: Optional[Backend] = None,
         absolute: bool = True,
     ):
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/fine_amplitude.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/fine_amplitude.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from qiskit.circuit import Gate
 from qiskit.circuit.library import XGate, SXGate
 from qiskit.providers.backend import Backend
 from qiskit_experiments.data_processing import DataProcessor, nodes
 from qiskit_experiments.framework import BaseExperiment, Options
 from qiskit_experiments.framework.restless_mixin import RestlessMixin
 from qiskit_experiments.library.characterization.analysis import FineAmplitudeAnalysis
-from qiskit_experiments.warnings import deprecate_arguments, qubit_deprecate
 
 
 class FineAmplitude(BaseExperiment, RestlessMixin):
     r"""An experiment to determine the optimal pulse amplitude by amplifying gate errors.
 
     # section: overview
 
@@ -109,15 +108,14 @@
         options.repetitions = list(range(1, 15))
         options.gate = None
         options.normalization = True
         options.add_cal_circuits = True
 
         return options
 
-    @deprecate_arguments({"qubits": "physical_qubits"}, "0.5")
     def __init__(
         self,
         physical_qubits: Sequence[int],
         gate: Gate,
         backend: Optional[Backend] = None,
         measurement_qubits: Sequence[int] = None,
     ):
@@ -160,18 +158,15 @@
             if add_x:
                 qubits = meas_circuit.get_instructions("measure")[0][1]
                 circ.x(qubits)
 
             circ.compose(meas_circuit, inplace=True)
 
             circ.metadata = {
-                "experiment_type": self._type,
-                "qubits": self.physical_qubits,
                 "xval": add_x,
-                "unit": "gate number",
                 "series": "spam-cal",
             }
 
             cal_circuits.append(circ)
 
         return cal_circuits
 
@@ -227,18 +222,15 @@
             for _ in range(repetition):
                 circuit.append(self.experiment_options.gate, qubits)
 
             # Add the measurement part of the circuit
             circuit.compose(meas_circ, qubits, range(meas_circ.num_clbits), inplace=True)
 
             circuit.metadata = {
-                "experiment_type": self._type,
-                "qubits": self.physical_qubits,
                 "xval": repetition,
-                "unit": "gate number",
                 "series": 1,
             }
 
             circuits.append(circuit)
 
         return circuits
 
@@ -257,15 +249,14 @@
 
     # section: overview
 
         :class:`FineXAmplitude` is a subclass of :class:`FineAmplitude` and is used to set
         the appropriate values for the default options.
     """
 
-    @qubit_deprecate()
     def __init__(self, physical_qubits: Sequence[int], backend: Optional[Backend] = None):
         """Initialize the experiment."""
         super().__init__(physical_qubits, XGate(), backend=backend)
         # Set default analysis options
         self.analysis.set_options(
             fixed_parameters={
                 "angle_per_gate": np.pi,
@@ -296,15 +287,14 @@
 
     # section: overview
 
         :class:`FineSXAmplitude` is a subclass of :class:`FineAmplitude` and is used to set
         the appropriate values for the default options.
     """
 
-    @qubit_deprecate()
     def __init__(self, physical_qubits: Sequence[int], backend: Optional[Backend] = None):
         """Initialize the experiment."""
         super().__init__(physical_qubits, SXGate(), backend=backend)
         # Set default analysis options
         self.analysis.set_options(
             fixed_parameters={
                 "angle_per_gate": np.pi / 2,
@@ -357,15 +347,14 @@
             fine_amp = FineZXAmplitude(qubits, backend)
             fine_amp.set_transpile_options(inst_map=inst_map)
 
         Here, :code:`my_schedule` is the pulse schedule that will implement the
         :code:`RZXGate(np.pi / 2)` rotation.
     """
 
-    @deprecate_arguments({"qubits": "physical_qubits"}, "0.5")
     def __init__(self, physical_qubits: Sequence[int], backend: Optional[Backend] = None):
         """Initialize the experiment."""
 
         # We cannot use RZXGate since it has a parameter so we redefine the gate.
         # Failing to do so causes issues with QuantumCircuit.calibrations.
         gate = Gate("szx", 2, [])
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/fine_drag.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/fine_drag.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,23 +18,22 @@
 from qiskit import QuantumCircuit
 from qiskit.circuit import Gate
 from qiskit.circuit.library import XGate, SXGate
 from qiskit.providers.backend import Backend
 from qiskit_experiments.framework import BaseExperiment, Options
 from qiskit_experiments.framework.restless_mixin import RestlessMixin
 from qiskit_experiments.curve_analysis.standard_analysis import ErrorAmplificationAnalysis
-from qiskit_experiments.warnings import qubit_deprecate
 
 
 class FineDrag(BaseExperiment, RestlessMixin):
     r"""An experiment that performs fine characterizations of DRAG pulse coefficients.
 
     # section: overview
 
-        :class:`FineDrag` runs fine DRAG characterization experiments (see :class:`.DragCal`
+        :class:`FineDrag` runs fine DRAG characterization experiments (see :class:`.RoughDrag`
         for the definition of DRAG pulses). Fine DRAG proceeds by iterating the gate sequence
         Rp - Rm where Rp is a rotation around an axis and Rm is the same rotation but in the
         opposite direction and is implemented by the gates Rz - Rp - Rz where the Rz gates
         are virtual Z-rotations, see Ref. [1]. The executed circuits are of the form
 
         .. parsed-literal::
 
@@ -146,15 +145,14 @@
         options = super()._default_experiment_options()
         options.repetitions = list(range(20))
         options.schedule = None
         options.gate = None
 
         return options
 
-    @qubit_deprecate()
     def __init__(
         self, physical_qubits: Sequence[int], gate: Gate, backend: Optional[Backend] = None
     ):
         """Setup a fine amplitude experiment on the given qubit.
 
         Args:
             physical_qubits: List containing the qubit on which to run the fine
@@ -216,20 +214,15 @@
                 circuit.add_calibration(
                     self.experiment_options.gate.name,
                     self.physical_qubits,
                     schedule,
                     params=[],
                 )
 
-            circuit.metadata = {
-                "experiment_type": self._type,
-                "qubits": self.physical_qubits,
-                "xval": repetition,
-                "unit": "gate number",
-            }
+            circuit.metadata = {"xval": repetition}
 
             circuits.append(circuit)
 
         return circuits
 
     def _metadata(self):
         metadata = super()._metadata()
@@ -240,15 +233,14 @@
                 metadata[run_opt] = getattr(self.run_options, run_opt)
         return metadata
 
 
 class FineXDrag(FineDrag):
     """Class to fine characterize the DRAG parameter of an X gate."""
 
-    @qubit_deprecate()
     def __init__(self, physical_qubits: Sequence[int], backend: Optional[Backend] = None):
         """Initialize the experiment."""
         super().__init__(physical_qubits, XGate(), backend=backend)
 
     @classmethod
     def _default_experiment_options(cls) -> Options:
         r"""Default values for the FineXDrag experiment.
@@ -266,15 +258,14 @@
         """Return the quantum circuit done before the Rp - Rz - Rp - Rz gates."""
         return QuantumCircuit(1)
 
 
 class FineSXDrag(FineDrag):
     """Class to fine characterize the DRAG parameter of an :math:`SX` gate."""
 
-    @qubit_deprecate()
     def __init__(self, physical_qubits: Sequence[int], backend: Optional[Backend] = None):
         """Initialize the experiment."""
         super().__init__(physical_qubits, SXGate(), backend=backend)
 
     @classmethod
     def _default_experiment_options(cls) -> Options:
         r"""Default values for the FineSXDrag experiment.
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/fine_frequency.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/fine_frequency.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import numpy as np
 
 from qiskit import QuantumCircuit
 from qiskit.providers.backend import Backend
 
 from qiskit_experiments.framework import BaseExperiment, Options
 from qiskit_experiments.curve_analysis.standard_analysis import ErrorAmplificationAnalysis
-from qiskit_experiments.warnings import qubit_deprecate
 
 
 class FineFrequency(BaseExperiment):
     r"""An experiment to make a fine measurement of the qubit frequency.
 
     # section: overview
 
@@ -47,15 +46,14 @@
                     └────┘└────────────────┘└──────────┘└────┘ ░ └╥┘
             meas: 1/══════════════════════════════════════════════╩═
                                                                   0
     # section: analysis_ref
         :class:`~qiskit_experiments.curve_analysis.ErrorAmplificationAnalysis`
     """
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         delay_duration: int,
         backend: Optional[Backend] = None,
         repetitions: Optional[List[int]] = None,
     ):
@@ -125,20 +123,15 @@
 
             circuit.delay(duration=self.experiment_options.delay_duration * repetition, unit="dt")
 
             circuit.rz(np.pi * repetition / 2, 0)
             circuit.sx(0)
             circuit.measure_all()
 
-            circuit.metadata = {
-                "experiment_type": self._type,
-                "qubits": self.physical_qubits,
-                "xval": repetition,
-                "unit": "Number of delays",
-            }
+            circuit.metadata = {"xval": repetition}
 
             circuits.append(circuit)
 
         return circuits
 
     def _metadata(self):
         metadata = super()._metadata()
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/half_angle.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/t2hahn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,150 +1,179 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2021.
+# (C) Copyright IBM 2022.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
+"""
+T2Hahn Echo Experiment class.
+"""
 
-"""Half angle characterization."""
-
-from typing import List, Optional, Sequence
+from typing import List, Optional, Union, Sequence
 import numpy as np
 
-from qiskit import QuantumCircuit
-from qiskit.providers import Backend
+from qiskit import QuantumCircuit, QiskitError
+from qiskit.circuit import Parameter
+from qiskit.providers.backend import Backend
 
-from qiskit_experiments.framework import BaseExperiment, Options
-from qiskit_experiments.curve_analysis.standard_analysis import ErrorAmplificationAnalysis
-from qiskit_experiments.curve_analysis import ParameterRepr
-from qiskit_experiments.warnings import qubit_deprecate
+from qiskit_experiments.framework import BackendTiming, BaseExperiment, Options
+from qiskit_experiments.library.characterization.analysis.t2hahn_analysis import T2HahnAnalysis
 
 
-class HalfAngle(BaseExperiment):
-    r"""An experiment class to measure the amount by which sx and x are not parallel.
+class T2Hahn(BaseExperiment):
+    r"""An experiment to measure the dephasing time insensitive to inhomogeneous
+    broadening using Hahn echos.
 
     # section: overview
 
-        This experiment runs circuits that repeat blocks of :code:`sx - sx - y` gates
-        inserted in a Ramsey type experiment, i.e. the full gate sequence is thus
-        :code:`Ry(π/2) - [sx - sx - y] ^ n - sx` where :code:`n` is varied.
+        This experiment is used to estimate the :math:`T_2` time of a single qubit.
+        :math:`T_2` is the dephasing time or the transverse relaxation time of the qubit
+        on the Bloch sphere as a result of both energy relaxation and pure dephasing in
+        the transverse plane. Unlike :math:`T_2^*`, which is measured by
+        :class:`.T2Ramsey`, :math:`T_2` is insensitive to inhomogenous broadening.
+
+        This experiment consists of a series of circuits of the form
+
 
         .. parsed-literal::
 
-                    ┌─────────┐┌────┐┌────┐┌───┐   ┌────┐┌────┐┌───┐┌────┐ ░ ┌─┐
-               q_0: ┤ Ry(π/2) ├┤ sx ├┤ sx ├┤ y ├...┤ sx ├┤ sx ├┤ y ├┤ sx ├─░─┤M├
-                    └─────────┘└────┘└────┘└───┘   └────┘└────┘└───┘└────┘ ░ └╥┘
-            meas: 1/════════════════════════════...═══════════════════════════╩═
-                                                                              0
-
-        This sequence measures angle errors where the axis of the :code:`sx` and :code:`x`
-        rotation are not parallel. A similar experiment is described in Ref.~[1] where the
-        gate sequence :code:`x - y` is repeated to amplify errors caused by non-orthogonal
-        :code:`x` and :code:`y` rotation axes. Such errors can occur due to phase errors.
-        For example, the non-linearities in the mixer's skew for :math:`\pi/2` pulses may
-        be different from the :math:`\pi` pulse.
+                 ┌─────────┐┌──────────┐┌───────┐┌──────────┐┌─────────┐┌─┐
+            q_0: ┤ Rx(π/2) ├┤ DELAY(t) ├┤ RX(π) ├┤ DELAY(t) ├┤ RX(π/2) ├┤M├
+                 └─────────┘└──────────┘└───────┘└──────────┘└─────────┘└╥┘
+            c: 1/════════════════════════════════════════════════════════╩═
+                                                                         0
+
+        for each *t* from the specified delay times
+        and the delays are specified by the user.
+        The delays that are specified are delay for each delay gate while
+        the delay in the metadata is the total delay which is delay * (num_echoes +1)
+        The circuits are run on the device or on a simulator backend.
+
+    # section: manual
+        :doc:`/manuals/characterization/t2hahn`
 
     # section: analysis_ref
-        :class:`.ErrorAmplificationAnalysis`
+        :class:`T2HahnAnalysis`
 
     # section: reference
-        .. ref_arxiv:: 1 1504.06597
+        .. ref_arxiv:: 1 1904.06560
     """
 
     @classmethod
     def _default_experiment_options(cls) -> Options:
-        r"""Default values for the half angle experiment.
+        """Default experiment options.
 
         Experiment Options:
-            repetitions (List[int]): A list of the number of times that the gate
-                sequence :code:`[sx sx y]` is repeated.
+            delays (Iterable[float]): Delay times of the experiments.
+            num_echoes (int): The number of echoes to preform.
         """
         options = super()._default_experiment_options()
-        options.repetitions = list(range(15))
-        return options
 
-    @classmethod
-    def _default_transpile_options(cls) -> Options:
-        """Default transpile options.
-
-        The basis gates option should not be changed since it will affect the gates and
-        the pulses that are run on the hardware.
-        """
-        options = super()._default_transpile_options()
-        options.basis_gates = ["sx", "rz", "y"]
-        options.inst_map = None
+        options.delays = None
+        options.num_echoes = 1
         return options
 
-    @qubit_deprecate()
-    def __init__(self, physical_qubits: Sequence[int], backend: Optional[Backend] = None):
-        """Setup a half angle experiment on the given qubit.
+    def __init__(
+        self,
+        physical_qubits: Sequence[int],
+        delays: Union[List[float], np.array],
+        num_echoes: int = 1,
+        backend: Optional[Backend] = None,
+    ):
+        """
+        Initialize the T2 - Hahn Echo class.
 
         Args:
-            physical_qubits: List containing the qubits on which to run the
-                fine amplitude calibration experiment.
+            physical_qubits: a single-element sequence containing the qubit whose T2 is to be
+                estimated.
+            delays: Total delay times of the experiments.
+            backend: Optional, the backend to run the experiment on.
+            num_echoes: The number of echoes to preform.
             backend: Optional, the backend to run the experiment on.
+
+        Raises:
+            QiskitError : Error for invalid input.
         """
-        analysis = ErrorAmplificationAnalysis()
+        # Initialize base experiment
+        super().__init__(physical_qubits, analysis=T2HahnAnalysis(), backend=backend)
 
-        default_bounds = analysis.options.bounds
-        default_bounds.update({"d_theta": (-np.pi / 2, np.pi / 2)})
+        # Set experiment options
+        self.set_experiment_options(delays=delays, num_echoes=num_echoes)
+        self._verify_parameters()
 
-        analysis.set_options(
-            fixed_parameters={
-                "angle_per_gate": np.pi,
-                "phase_offset": -np.pi / 2,
-                "amp": 1.0,
-            },
-            result_parameters=[ParameterRepr("d_theta", "d_hac", "rad")],
-            normalization=True,
-            bounds=default_bounds,
-        )
-
-        super().__init__(physical_qubits, analysis=analysis, backend=backend)
-
-    @staticmethod
-    def _pre_circuit() -> QuantumCircuit:
-        """Return the preparation circuit for the experiment."""
-        return QuantumCircuit(1)
+    def _verify_parameters(self):
+        """
+        Verify input correctness, raise QiskitError if needed.
+
+        Raises:
+            QiskitError : Error for invalid input.
+        """
+        if any(delay < 0 for delay in self.experiment_options.delays):
+            raise QiskitError(
+                f"The lengths list {self.experiment_options.delays} should only contain "
+                "non-negative elements."
+            )
 
     def circuits(self) -> List[QuantumCircuit]:
-        """Create the circuits for the half angle calibration experiment."""
+        """
+        Return a list of experiment circuits.
 
-        circuits = []
+        Each circuit consists of RX(π/2) followed by a sequence of delay gate,
+        RX(π) for echo and delay gate again.
+        The sequence repeats for the number of echoes and terminates with RX(±π/2).
+
+        Returns:
+            The experiment circuits.
+        """
+        timing = BackendTiming(self.backend)
 
-        for repetition in self.experiment_options.repetitions:
-            circuit = self._pre_circuit()
+        delay_param = Parameter("delay")
 
-            # First ry gate
-            circuit.rz(np.pi / 2, 0)
-            circuit.sx(0)
-            circuit.rz(-np.pi / 2, 0)
-
-            # Error amplifying sequence
-            for _ in range(repetition):
-                circuit.sx(0)
-                circuit.sx(0)
-                circuit.y(0)
-
-            circuit.sx(0)
-            circuit.measure_all()
-
-            circuit.metadata = {
-                "experiment_type": self._type,
-                "qubits": self.physical_qubits,
-                "xval": repetition,
-                "unit": "repetition number",
-            }
+        num_echoes = self.experiment_options.num_echoes
 
-            circuits.append(circuit)
+        # First X rotation in 90 degrees
+        template = QuantumCircuit(1, 1)
+        template.rx(np.pi / 2, 0)  # Brings the qubit to the X Axis
+        if num_echoes == 0:
+            # if number of echoes is 0 then just apply the delay gate
+            template.delay(delay_param, 0, timing.delay_unit)
+        else:
+            for _ in range(num_echoes):
+                template.delay(delay_param, 0, timing.delay_unit)
+                template.rx(np.pi, 0)
+                template.delay(delay_param, 0, timing.delay_unit)
+
+        if num_echoes % 2 == 1:
+            template.rx(np.pi / 2, 0)  # X90 again since the num of echoes is odd
+        else:
+            template.rx(-np.pi / 2, 0)  # X(-90) again since the num of echoes is even
+        template.measure(0, 0)  # measure
+
+        circuits = []
+        for delay in self.experiment_options.delays:
+            if num_echoes == 0:
+                single_delay = timing.delay_time(time=delay)
+                total_delay = single_delay
+            else:
+                # Equal delay is put before and after each echo, so each echo gets
+                # two delay gates. When there are multiple echoes, the total delay
+                # between echoes is 2 * single_delay, made up of two delay gates.
+                single_delay = timing.delay_time(time=delay / num_echoes / 2)
+                total_delay = single_delay * num_echoes * 2
+
+            assigned = template.assign_parameters(
+                {delay_param: timing.round_delay(time=single_delay)}, inplace=False
+            )
+            assigned.metadata = {"xval": total_delay}
+            circuits.append(assigned)
 
         return circuits
 
     def _metadata(self):
         metadata = super()._metadata()
         # Store measurement level and meas return if they have been
         # set for the experiment
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/local_readout_error.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/local_readout_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 """
 Local readout error calibration experiment class.
 """
 from typing import Iterable, List, Optional
 from qiskit import QuantumCircuit
 from qiskit.providers.backend import BackendV2, Backend
 from qiskit.exceptions import QiskitError
-from qiskit_experiments.warnings import deprecate_arguments
 from qiskit_experiments.framework import BaseExperiment
 from qiskit_experiments.library.characterization.analysis.local_readout_error_analysis import (
     LocalReadoutErrorAnalysis,
 )
 from .correlated_readout_error import calibration_circuit
 
 
@@ -59,19 +58,21 @@
 
         See :class:`LocalReadoutErrorAnalysis`
         documentation for additional information on local readout error experiment analysis.
 
     # section: analysis_ref
         :class:`LocalReadoutErrorAnalysis`
 
+    # section: manual
+        :doc:`/manuals/measurement/readout_mitigation`
+
     # section: reference
         .. ref_arxiv:: 1 2006.14044
     """
 
-    @deprecate_arguments({"qubits": "physical_qubits"}, "0.5")
     def __init__(
         self,
         physical_qubits: Optional[Iterable[int]] = None,
         backend: Optional[Backend] = None,
     ):
         """Initialize a local readout error characterization experiment.
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/multi_state_discrimination.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/multi_state_discrimination.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from qiskit import QuantumCircuit
 from qiskit.circuit import Gate
 from qiskit.providers import Backend
 from qiskit.providers.options import Options
 from qiskit.pulse import ScheduleBlock
 from qiskit.qobj.utils import MeasLevel, MeasReturnType
 from qiskit_experiments.framework import BaseExperiment
-from qiskit_experiments.warnings import qubit_deprecate
 from qiskit_experiments.library.characterization import MultiStateDiscriminationAnalysis
 
 
 class MultiStateDiscrimination(BaseExperiment):
     r"""An experiment that discriminates between the first :math:`n` energy states.
 
     # section: overview
@@ -52,15 +51,15 @@
                 meas: ═══════════════════════╩═
 
     # section: analysis_ref
         :class:`MultiStateDiscriminationAnalysis`
 
     # section: reference
         `Qiskit Textbook\
-        <https://qiskit.org/textbook/ch-quantum-hardware/accessing_higher_energy_states.html>`_
+        <https://github.com/Qiskit/textbook/blob/main/notebooks/quantum-hardware-pulses/accessing_higher_energy_states.ipynb>`_
 
     """
 
     @classmethod
     def _default_run_options(cls) -> Options:
         """Default option values for the experiment :meth:`run` method."""
         options = super()._default_run_options()
@@ -83,15 +82,14 @@
         """
         options = super()._default_experiment_options()
         options.n_states = 2
         options.schedules = None
 
         return options
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         backend: Optional[Backend] = None,
         n_states: Optional[int] = None,
         schedules: Optional[Dict[str, ScheduleBlock]] = None,
     ):
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/qubit_spectroscopy.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/qubit_spectroscopy.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,12 +119,12 @@
         # Create the circuits to run
         circs = []
         for freq in self._frequencies:
             freq_shift = freq - self._backend_center_frequency if self._absolute else freq
             freq_shift = np.round(freq_shift, decimals=3)
 
             assigned_circ = circuit.assign_parameters({freq_param: freq_shift}, inplace=False)
-            self._add_metadata(assigned_circ, freq, sched)
+            self._add_metadata(assigned_circ, freq)
 
             circs.append(assigned_circ)
 
         return circs
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/rabi.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/rabi.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from qiskit.providers import Backend
 from qiskit.pulse import ScheduleBlock
 from qiskit.exceptions import QiskitError
 
 from qiskit_experiments.framework import BaseExperiment, Options
 from qiskit_experiments.framework.restless_mixin import RestlessMixin
 from qiskit_experiments.curve_analysis import ParameterRepr, OscillationAnalysis
-from qiskit_experiments.warnings import qubit_deprecate
 
 
 class Rabi(BaseExperiment, RestlessMixin):
     r"""An experiment that scans a pulse amplitude to calibrate rotations on the :math:`|0\rangle`
     <-> :math:`|1\rangle` transition.
 
     # section: overview
@@ -47,16 +46,16 @@
 
         The user provides his own schedule for the Rabi at initialization which must have one
         free parameter, i.e. the amplitude to scan and a drive channel which matches the qubit.
 
     # section: manual
         :ref:`Rabi Calibration`
 
-        See also `Qiskit Textbook <https://qiskit.org/textbook/ch-quantum-hardware/\
-        calibrating-qubits-pulse.html>`_
+        See also the `Qiskit Textbook
+        <https://github.com/Qiskit/textbook/blob/main/notebooks/quantum-hardware-pulses/calibrating-qubits-pulse.ipynb>`_
         for the pulse level programming of a Rabi experiment.
 
     # section: analysis_ref
         :class:`~qiskit_experiments.curve_analysis.OscillationAnalysis`
     """
 
     __gate_name__ = "Rabi"
@@ -85,15 +84,14 @@
         options = super()._default_experiment_options()
 
         options.amplitudes = np.linspace(-0.95, 0.95, 51)
         options.schedule = None
 
         return options
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         schedule: ScheduleBlock,
         amplitudes: Optional[Iterable[float]] = None,
         backend: Optional[Backend] = None,
     ):
@@ -157,23 +155,19 @@
 
         # Create template circuit
         circuit, param = self._template_circuit()
 
         # Create the circuits to run
         circs = []
         for amp in self.experiment_options.amplitudes:
-            amp = np.round(amp, decimals=6)
+            # casting is needed because for amplitude '0', np.round method return datatype of int32
+            # which isn't serializable in the metadata.
+            amp = float(np.round(amp, decimals=6))
             assigned_circ = circuit.assign_parameters({param: amp}, inplace=False)
-            assigned_circ.metadata = {
-                "experiment_type": self._type,
-                "qubits": self.physical_qubits,
-                "xval": amp,
-                "unit": "arb. unit",
-                "amplitude": amp,
-            }
+            assigned_circ.metadata = {"xval": amp}
 
             circs.append(assigned_circ)
 
         return circs
 
     def _metadata(self):
         metadata = super()._metadata()
@@ -183,15 +177,15 @@
             if hasattr(self.run_options, run_opt):
                 metadata[run_opt] = getattr(self.run_options, run_opt)
         return metadata
 
 
 class EFRabi(Rabi):
     r"""An experiment that scans the amplitude of a pulse inducing rotations on the
-     :math:`|1\rangle` <-> :math:`|2\rangle` transition.
+    :math:`|1\rangle` <-> :math:`|2\rangle` transition.
 
     # section: overview
 
         This experiment is a subclass of the :class:`Rabi` experiment but takes place between
         the first and second excited state. An initial X gate populates the first excited state.
         The Rabi pulse is applied on the :math:`|1\rangle` <-> :math:`|2\rangle` transition
         (sometimes also labeled the e <-> f transition). The necessary frequency shift (typically
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/ramsey_xy.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/ramsey_xy.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,27 +7,24 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Ramsey XY frequency characterization experiment."""
-
 from typing import List, Optional, Sequence
-import numpy as np
 
-from qiskit import QuantumCircuit
-from qiskit.circuit import Parameter
+import numpy as np
+from qiskit.circuit import QuantumCircuit, Parameter
 from qiskit.providers.backend import Backend
 from qiskit.qobj.utils import MeasLevel
 
-from qiskit_experiments.framework import BackendTiming, BaseExperiment
+from qiskit_experiments.framework import BaseExperiment, Options, BackendTiming
 from qiskit_experiments.framework.restless_mixin import RestlessMixin
 from qiskit_experiments.library.characterization.analysis import RamseyXYAnalysis
-from qiskit_experiments.warnings import qubit_deprecate
 
 
 class RamseyXY(BaseExperiment, RestlessMixin):
     r"""A sign-sensitive experiment to measure the frequency of a qubit.
 
     # section: overview
 
@@ -82,29 +79,28 @@
         circuit above it appears as the delay-dependent angle θ(τ).
 
     # section: analysis_ref
         :class:`RamseyXYAnalysis`
     """
 
     @classmethod
-    def _default_experiment_options(cls):
+    def _default_experiment_options(cls) -> Options:
         """Default values for the Ramsey XY experiment.
 
         Experiment Options:
             delays (list): The list of delays that will be scanned in the experiment, in seconds.
             osc_freq (float): A frequency shift in Hz that will be applied by means of
                 a virtual Z rotation to increase the frequency of the measured oscillation.
         """
         options = super()._default_experiment_options()
         options.delays = np.linspace(0, 1.0e-6, 51)
         options.osc_freq = 2e6
 
         return options
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         backend: Optional[Backend] = None,
         delays: Optional[List] = None,
         osc_freq: float = 2e6,
     ):
@@ -144,50 +140,43 @@
 
         rotation_angle = 2 * np.pi * self.experiment_options.osc_freq * p_delay
 
         if timing.delay_unit == "dt":
             rotation_angle = rotation_angle * timing.dt
 
         # Create the X and Y circuits.
-        metadata = {
-            "experiment_type": self._type,
-            "qubits": self.physical_qubits,
-            "osc_freq": self.experiment_options.osc_freq,
-            "unit": "s",
-        }
-
         ram_x = self._pre_circuit()
         ram_x.sx(0)
         ram_x.delay(p_delay, 0, timing.delay_unit)
         ram_x.rz(rotation_angle, 0)
         ram_x.sx(0)
         ram_x.measure_active()
-        ram_x.metadata = metadata.copy()
 
         ram_y = self._pre_circuit()
         ram_y.sx(0)
         ram_y.delay(p_delay, 0, timing.delay_unit)
         ram_y.rz(rotation_angle - np.pi / 2, 0)
         ram_y.sx(0)
         ram_y.measure_active()
-        ram_y.metadata = metadata.copy()
 
         circs = []
         for delay in self.experiment_options.delays:
-            assigned_x = ram_x.assign_parameters(
-                {p_delay: timing.round_delay(time=delay)}, inplace=False
-            )
-            assigned_x.metadata["series"] = "X"
-            assigned_x.metadata["xval"] = timing.delay_time(time=delay)
-
-            assigned_y = ram_y.assign_parameters(
-                {p_delay: timing.round_delay(time=delay)}, inplace=False
-            )
-            assigned_y.metadata["series"] = "Y"
-            assigned_y.metadata["xval"] = timing.delay_time(time=delay)
+            delay_dt = timing.round_delay(time=delay)
+            delay_sec = timing.delay_time(time=delay)
+
+            assigned_x = ram_x.assign_parameters({p_delay: delay_dt}, inplace=False)
+            assigned_x.metadata = {
+                "series": "X",
+                "xval": delay_sec,
+            }
+            assigned_y = ram_y.assign_parameters({p_delay: delay_dt}, inplace=False)
+            assigned_y.metadata = {
+                "series": "Y",
+                "xval": delay_sec,
+            }
 
             circs.extend([assigned_x, assigned_y])
 
         return circs
 
     def _finalize(self):
         # Set initial guess for sinusoidal offset when meas level is 2.
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/readout_angle.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/readout_angle.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from typing import List, Optional, Sequence
 
 from qiskit.circuit import QuantumCircuit
 from qiskit.qobj.utils import MeasLevel
 from qiskit.providers.backend import Backend
 
 from qiskit_experiments.framework import BaseExperiment, Options
-from qiskit_experiments.warnings import qubit_deprecate
 from qiskit_experiments.library.characterization.analysis.readout_angle_analysis import (
     ReadoutAngleAnalysis,
 )
 
 
 class ReadoutAngle(BaseExperiment):
     r"""
@@ -43,31 +42,28 @@
            in the ground state, the second circuit sets the qubit in the excited state
            and measures it. Measurements are in level 1 (kerneled).
         2. Backend execution: actually running the circuits on the device
            (or a simulator that supports level 1 measurements). The backend returns
            the cluster centers of the ground and excited states.
         3. Analysis of results: return the average of the angles of the two centers.
 
-        |
-
     # section: analysis_ref
         :class:`ReadoutAngleAnalysis`
     """
 
     @classmethod
     def _default_run_options(cls) -> Options:
         """Default run options."""
         options = super()._default_run_options()
 
         options.meas_level = MeasLevel.KERNELED
         options.meas_return = "avg"
 
         return options
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         backend: Optional[Backend] = None,
     ):
         """
         Initialize the readout angle experiment class
@@ -85,20 +81,15 @@
         Return a list of experiment circuits
 
         Returns:
             The experiment circuits
         """
         circ0 = QuantumCircuit(1, 1)
         circ0.measure(0, 0)
+        circ0.metadata = {"xval": 0}
 
         circ1 = QuantumCircuit(1, 1)
         circ1.x(0)
         circ1.measure(0, 0)
-
-        for i, circ in enumerate([circ0, circ1]):
-            circ.metadata = {
-                "experiment_type": self._type,
-                "qubit": self.physical_qubits[0],
-                "xval": i,
-            }
+        circ1.metadata = {"xval": 1}
 
         return [circ0, circ1]
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/resonator_spectroscopy.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/resonator_spectroscopy.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from qiskit import pulse
 from qiskit.circuit import Parameter
 from qiskit.exceptions import QiskitError
 from qiskit.providers import Backend
 
 from qiskit_experiments.framework import BackendData, BackendTiming, Options
 from qiskit_experiments.library.characterization.spectroscopy import Spectroscopy
-from qiskit_experiments.warnings import qubit_deprecate
+from qiskit_experiments.database_service import Resonator
 from .analysis.resonator_spectroscopy_analysis import ResonatorSpectroscopyAnalysis
 
 
 class ResonatorSpectroscopy(Spectroscopy):
     """An experiment to perform frequency spectroscopy of the readout resonator.
 
     # section: overview
@@ -142,15 +142,14 @@
                 raise QiskitError(
                     "Initial circuit must be for exactly one qubit and zero classical bits. Got "
                     f"{initial_circuit.num_qubits} qubits and {initial_circuit.num_clbits} "
                     "classical bits instead."
                 )
         return super().set_experiment_options(**fields)
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         backend: Optional[Backend] = None,
         frequencies: Optional[Iterable[float]] = None,
         absolute: bool = True,
         **experiment_options,
@@ -158,15 +157,15 @@
         """Initialize a resonator spectroscopy experiment.
 
         A spectroscopy experiment run by setting the frequency of the readout drive.
         The parameters of the GaussianSquare spectroscopy pulse can be specified at run-time
         through the experiment options.
 
         Args:
-            physical_qubits: List containing the qubit on which to run readout
+            physical_qubits: List containing the resonator on which to run readout
                 spectroscopy.
             backend: Optional, the backend to run the experiment on.
             frequencies: The frequencies to scan in the experiment, in Hz. The default values
                 range from -20 MHz to 20 MHz in 51 steps. If the ``absolute`` variable is
                 set to True then a center frequency obtained from the backend's defaults is
                 added to each value of this range.
             absolute: Boolean to specify if the frequencies are absolute or relative to the
@@ -254,14 +253,20 @@
                 ),
                 pulse.MeasureChannel(qubit),
             )
             pulse.acquire(duration, qubit, pulse.MemorySlot(self.experiment_options.memory_slot))
 
         return schedule, freq_param
 
+    def _metadata(self):
+        """Update metadata with the resonator components."""
+        metadata = super()._metadata()
+        metadata["device_components"] = list(map(Resonator, self.physical_qubits))
+        return metadata
+
     def circuits(self):
         """Create the circuit for the spectroscopy experiment.
 
         The circuits are based on a GaussianSquare pulse and a frequency_shift instruction
         encapsulated in a measurement instruction.
 
         Returns:
@@ -274,12 +279,12 @@
             freq_shift = freq - self._backend_center_frequency if self._absolute else freq
             freq_shift = np.round(freq_shift, decimals=3)
 
             sched_ = sched.assign_parameters({freq_param: freq_shift}, inplace=False)
 
             circuit = self._template_circuit()
             circuit.add_calibration("measure", self.physical_qubits, sched_)
-            self._add_metadata(circuit, freq, sched)
+            self._add_metadata(circuit, freq)
 
             circs.append(circuit)
 
         return circs
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/spectroscopy.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/spectroscopy.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,20 @@
 """Abstract spectroscopy experiment base class."""
 
 from abc import ABC, abstractmethod
 from typing import Iterable, Optional, Sequence
 
 import numpy as np
 from qiskit import QuantumCircuit
-from qiskit import pulse
 from qiskit.exceptions import QiskitError
 from qiskit.providers import Backend
 from qiskit.qobj.utils import MeasLevel
 
 from qiskit_experiments.framework import BaseAnalysis, BaseExperiment, Options
 from qiskit_experiments.curve_analysis import ResonanceAnalysis
-from qiskit_experiments.warnings import qubit_deprecate
 
 
 class Spectroscopy(BaseExperiment, ABC):
     """An abstract class for spectroscopy experiments."""
 
     @classmethod
     def _default_experiment_options(cls) -> Options:
@@ -58,15 +56,14 @@
         options = super()._default_run_options()
 
         options.meas_level = MeasLevel.KERNELED
         options.meas_return = "avg"
 
         return options
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         frequencies: Iterable[float],
         backend: Optional[Backend] = None,
         absolute: bool = True,
         analysis: Optional[BaseAnalysis] = None,
@@ -107,27 +104,21 @@
         This frequency is used to calculate the appropriate frequency shifts to apply to the
         spectroscopy pulse as its frequency is scanned in the experiment. Spectroscopy experiments
         should implement schedules using frequency shifts. Therefore, if an absolute frequency
         range is given the frequency shifts need to be corrected by the backend default frequency
         which depends on the nature of the spectroscopy experiment.
         """
 
-    def _add_metadata(self, circuit: QuantumCircuit, freq: float, sched: pulse.ScheduleBlock):
+    def _add_metadata(self, circuit: QuantumCircuit, freq: float):
         """Helper method to add the metadata to avoid code duplication with subclasses."""
 
         if not self._absolute:
             freq += self._backend_center_frequency
 
-        circuit.metadata = {
-            "experiment_type": self._type,
-            "qubits": self.physical_qubits,
-            "xval": np.round(freq, decimals=3),
-            "unit": "Hz",
-            "schedule": str(sched),
-        }
+        circuit.metadata = {"xval": np.round(freq, decimals=3)}
 
     def _metadata(self):
         metadata = super()._metadata()
         # Store measurement level and meas return if they have been
         # set for the experiment
         for run_opt in ["meas_level", "meas_return"]:
             if hasattr(self.run_options, run_opt):
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/t1.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/t1.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 """
 T1 Experiment class.
 """
 
 from typing import List, Optional, Union, Sequence
-import numpy as np
 
-from qiskit import QuantumCircuit
+import numpy as np
+from qiskit.circuit import QuantumCircuit
 from qiskit.providers.backend import Backend
+
 from qiskit_experiments.framework import BackendTiming, BaseExperiment, Options
-from qiskit_experiments.warnings import qubit_deprecate
 from qiskit_experiments.library.characterization.analysis.t1_analysis import T1Analysis
 
 
 class T1(BaseExperiment):
     r"""An experiment to measure the qubit relaxation time.
 
     # section: overview
@@ -49,15 +49,14 @@
         Experiment Options:
             delays (Iterable[float]): Delay times of the experiments in seconds.
         """
         options = super()._default_experiment_options()
         options.delays = None
         return options
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         delays: Union[List[float], np.array],
         backend: Optional[Backend] = None,
     ):
         """
@@ -92,20 +91,15 @@
             circ = QuantumCircuit(1, 1)
             circ.x(0)
             circ.barrier(0)
             circ.delay(timing.round_delay(time=delay), 0, timing.delay_unit)
             circ.barrier(0)
             circ.measure(0, 0)
 
-            circ.metadata = {
-                "experiment_type": self._type,
-                "qubit": self.physical_qubits[0],
-                "unit": "s",
-            }
-            circ.metadata["xval"] = timing.delay_time(time=delay)
+            circ.metadata = {"xval": timing.delay_time(time=delay)}
 
             circuits.append(circ)
 
         return circuits
 
     def _metadata(self):
         metadata = super()._metadata()
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/t2hahn.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/half_angle.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,187 +1,172 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2022.
+# (C) Copyright IBM 2021.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
-"""
-T2Hahn Echo Experiment class.
-"""
 
-from typing import List, Optional, Union, Sequence
-import numpy as np
+"""Half angle characterization."""
 
-from qiskit import QuantumCircuit, QiskitError
-from qiskit.circuit import Parameter
-from qiskit.providers.backend import Backend
-
-from qiskit_experiments.framework import BackendTiming, BaseExperiment, Options
-from qiskit_experiments.library.characterization.analysis.t2hahn_analysis import T2HahnAnalysis
-from qiskit_experiments.warnings import qubit_deprecate
+from typing import List, Optional, Sequence
+import numpy as np
 
+from qiskit import QuantumCircuit
+from qiskit.providers import Backend
 
-class T2Hahn(BaseExperiment):
-    r"""An experiment to measure the dephasing time insensitive to inhomogeneous
-    broadening using Hahn echos.
+from qiskit_experiments.framework import BaseExperiment, Options
+from qiskit_experiments.curve_analysis.standard_analysis import ErrorAmplificationAnalysis
+from qiskit_experiments.curve_analysis import ParameterRepr
 
-    # section: overview
 
-        This experiment is used to estimate the :math:`T_2` time of a single qubit.
-        :math:`T_2` is the dephasing time or the transverse relaxation time of the qubit
-        on the Bloch sphere as a result of both energy relaxation and pure dephasing in
-        the transverse plane. Unlike :math:`T_2^*`, which is measured by
-        :class:`.T2Ramsey`, :math:`T_2` is insensitive to inhomogenous broadening.
+class HalfAngle(BaseExperiment):
+    r"""An experiment class to measure the amount by which sx and x are not parallel.
 
-        This experiment consists of a series of circuits of the form
+    # section: overview
 
+        This experiment runs circuits that repeat blocks of :code:`sx - sx - y` gates
+        inserted in a Ramsey type experiment, i.e. the full gate sequence is thus
+        :code:`Ry(π/2) - [sx - sx - y] ^ n - sx` where :code:`n` is varied.
 
         .. parsed-literal::
 
-                 ┌─────────┐┌──────────┐┌───────┐┌──────────┐┌─────────┐┌─┐
-            q_0: ┤ Rx(π/2) ├┤ DELAY(t) ├┤ RX(π) ├┤ DELAY(t) ├┤ RX(π/2) ├┤M├
-                 └─────────┘└──────────┘└───────┘└──────────┘└─────────┘└╥┘
-            c: 1/════════════════════════════════════════════════════════╩═
-                                                                         0
-
-        for each *t* from the specified delay times
-        and the delays are specified by the user.
-        The delays that are specified are delay for each delay gate while
-        the delay in the metadata is the total delay which is delay * (num_echoes +1)
-        The circuits are run on the device or on a simulator backend.
-
-    # section: manual
-        :doc:`/manuals/characterization/t2hahn`
+                    ┌─────────┐┌────┐┌────┐┌───┐   ┌────┐┌────┐┌───┐┌────┐ ░ ┌─┐
+               q_0: ┤ Ry(π/2) ├┤ sx ├┤ sx ├┤ y ├...┤ sx ├┤ sx ├┤ y ├┤ sx ├─░─┤M├
+                    └─────────┘└────┘└────┘└───┘   └────┘└────┘└───┘└────┘ ░ └╥┘
+            meas: 1/════════════════════════════...═══════════════════════════╩═
+                                                                              0
+
+        This sequence measures angle errors where the axis of the :code:`sx` and :code:`x`
+        rotation are not parallel. A similar experiment is described in Ref.~[1] where the
+        gate sequence :code:`x - y` is repeated to amplify errors caused by non-orthogonal
+        :code:`x` and :code:`y` rotation axes.
+
+        One cause of such errors is non-linearity in the microwave mixer used
+        to produce the pulses for the ``x`` and ``sx`` gates. Typically, these
+        gates are calibrated to have the same duration and so have different
+        pulse amplitudes. Non-linearities in the mixer's skew can cause the
+        angle to differ for these different pulse amplitudes.
+
+        The way the experiment works is that the initial ``Ry(π/2)`` puts the
+        qubit close to the :math:`+X` state, with a deviation :math:`δθ`, due
+        to the misalignment between ``sx`` and ``x`` (``Ry(π/2)`` is
+        implemented with ``sx`` as described below). The first ``sx - sx`` do
+        nothing as they should be rotations about the axis the qubit is
+        pointing along. The first ``y`` then mirrors the qubit about the
+        :math:`y` axis in the :math:`xy` plane of the Bloch sphere, so the
+        :math:`δθ` deviation from :math:`+X` becomes a :math:`-δθ` from
+        :math:`-X`. The next ``sx - sx`` sequence rotates about the axis that
+        is :math:`+δθ` rotated in the :math:`xy` plane from :math:`+X`, which
+        takes the deviation from :math:`-X` from :math:`-δθ` to :math:`+3 δθ`.
+        Then the next ``y`` mirrors this across the :math:`y` axis, taking the
+        state to :math:`-3 δθ` from :math:`+X`. This pattern continues with
+        each iteration, with the angular deviation in units of :math:`δθ`
+        following the sequence 1, 3, 5, 7, 9, etc. from :math:`+X` and
+        :math:`-X`. The final ``sx`` rotation serves mainly to rotate these
+        deviations from :math:`+X` and :math:`-X` in the :math:`xy` plane into
+        deviations out of the :math:`xy` plane, so that they appear as a signal
+        in the :math:`Z` basis.  Because ``sx`` has a :math:`δθ` deviation from
+        ``x``, the final ``sx`` adds an extra :math:`δθ` to the deviations, so
+        the pattern ends up as 2, 4, 6, 8, etc., meaning that each iteration
+        adds :math:`2 δθ` to the deviation from the equator of the Bloch sphere
+        (with the sign alternating due to the ``y`` gates, so the deviations
+        are really -2, 4, -6, 8, etc.).
+
+        For the implementation of the circuits, the experiment uses ``Rz(π/2) -
+        sx - Rz(-π/2)`` to implement the ``Ry(π/2)`` and ``Rz(π/2) - x -
+        Rz(-π/2)`` to implement the ``y``. So the experiment makes use of only
+        ``sx``, ``x``, ``Rz(π/2)``, and ``Rz(-π/2)`` gates. For the
+        experiment's analysis to be valid, it is important that the ``sx`` and
+        ``x`` gates are not replaced (such as by a transpiler pass that
+        replaces ``x`` with ``sx - sx``), as it is the angle between them which
+        is being inferred. It is assumed that the angle between ``x`` and
+        ``Rz`` is exactly :math:`π/2`.
 
     # section: analysis_ref
-        :class:`T2HahnAnalysis`
+        :class:`.ErrorAmplificationAnalysis`
 
     # section: reference
-        .. ref_arxiv:: 1 1904.06560
+        .. ref_arxiv:: 1 1504.06597
     """
 
     @classmethod
     def _default_experiment_options(cls) -> Options:
-        """Default experiment options.
+        r"""Default values for the half angle experiment.
 
         Experiment Options:
-            delays (Iterable[float]): Delay times of the experiments.
-            num_echoes (int): The number of echoes to preform.
+            repetitions (List[int]): A list of the number of times that the gate
+                sequence :code:`[sx sx y]` is repeated.
         """
         options = super()._default_experiment_options()
-
-        options.delays = None
-        options.num_echoes = 1
+        options.repetitions = list(range(15))
         return options
 
-    @qubit_deprecate()
-    def __init__(
-        self,
-        physical_qubits: Sequence[int],
-        delays: Union[List[float], np.array],
-        num_echoes: int = 1,
-        backend: Optional[Backend] = None,
-    ):
-        """
-        Initialize the T2 - Hahn Echo class
+    def __init__(self, physical_qubits: Sequence[int], backend: Optional[Backend] = None):
+        """Setup a half angle experiment on the given qubit.
 
         Args:
-            physical_qubits: a single-element sequence containing the qubit whose T2 is to be
-                estimated
-            delays: Total delay times of the experiments.
+            physical_qubits: List containing the qubits on which to run the
+                fine amplitude calibration experiment.
             backend: Optional, the backend to run the experiment on.
-            num_echoes: The number of echoes to preform.
-            backend: Optional, the backend to run the experiment on.
-
-         Raises:
-             QiskitError : Error for invalid input.
         """
-        # Initialize base experiment
-        super().__init__(physical_qubits, analysis=T2HahnAnalysis(), backend=backend)
+        analysis = ErrorAmplificationAnalysis()
 
-        # Set experiment options
-        self.set_experiment_options(delays=delays, num_echoes=num_echoes)
-        self._verify_parameters()
+        default_bounds = analysis.options.bounds
+        default_bounds.update({"d_theta": (-np.pi / 2, np.pi / 2)})
 
-    def _verify_parameters(self):
-        """
-        Verify input correctness, raise QiskitError if needed.
-
-        Raises:
-            QiskitError : Error for invalid input.
-        """
-        if any(delay < 0 for delay in self.experiment_options.delays):
-            raise QiskitError(
-                f"The lengths list {self.experiment_options.delays} should only contain "
-                "non-negative elements."
-            )
+        analysis.set_options(
+            fixed_parameters={
+                "angle_per_gate": np.pi,
+                "phase_offset": -np.pi / 2,
+                "amp": 1.0,
+            },
+            result_parameters=[ParameterRepr("d_theta", "d_hac", "rad")],
+            normalization=True,
+            bounds=default_bounds,
+        )
+
+        super().__init__(physical_qubits, analysis=analysis, backend=backend)
+
+    @staticmethod
+    def _pre_circuit() -> QuantumCircuit:
+        """Return the preparation circuit for the experiment."""
+        return QuantumCircuit(1)
 
     def circuits(self) -> List[QuantumCircuit]:
-        """
-        Return a list of experiment circuits.
+        """Create the circuits for the half angle calibration experiment."""
 
-        Each circuit consists of RX(π/2) followed by a sequence of delay gate,
-        RX(π) for echo and delay gate again.
-        The sequence repeats for the number of echoes and terminates with RX(±π/2).
+        circuits = []
 
-        Returns:
-            The experiment circuits.
-        """
-        timing = BackendTiming(self.backend)
+        for repetition in self.experiment_options.repetitions:
+            circuit = self._pre_circuit()
 
-        template = QuantumCircuit(1, 1)
-        template.metadata = {
-            "experiment_type": self._type,
-            "qubit": self.physical_qubits[0],
-            "unit": "s",
-        }
-
-        delay_param = Parameter("delay")
-
-        num_echoes = self.experiment_options.num_echoes
-
-        # First X rotation in 90 degrees
-        template.rx(np.pi / 2, 0)  # Brings the qubit to the X Axis
-        if num_echoes == 0:
-            # if number of echoes is 0 then just apply the delay gate
-            template.delay(delay_param, 0, timing.delay_unit)
-        else:
-            for _ in range(num_echoes):
-                template.delay(delay_param, 0, timing.delay_unit)
-                template.rx(np.pi, 0)
-                template.delay(delay_param, 0, timing.delay_unit)
-
-        if num_echoes % 2 == 1:
-            template.rx(np.pi / 2, 0)  # X90 again since the num of echoes is odd
-        else:
-            template.rx(-np.pi / 2, 0)  # X(-90) again since the num of echoes is even
-        template.measure(0, 0)  # measure
+            # First ry gate
+            circuit.rz(np.pi / 2, 0)
+            circuit.sx(0)
+            circuit.rz(-np.pi / 2, 0)
+
+            # Error amplifying sequence
+            for _ in range(repetition):
+                circuit.sx(0)
+                circuit.sx(0)
+                circuit.rz(np.pi / 2, 0)
+                circuit.x(0)
+                circuit.rz(-np.pi / 2, 0)
 
-        circuits = []
-        for delay in self.experiment_options.delays:
-            if num_echoes == 0:
-                single_delay = timing.delay_time(time=delay)
-                total_delay = single_delay
-            else:
-                # Equal delay is put before and after each echo, so each echo gets
-                # two delay gates. When there are multiple echoes, the total delay
-                # between echoes is 2 * single_delay, made up of two delay gates.
-                single_delay = timing.delay_time(time=delay / num_echoes / 2)
-                total_delay = single_delay * num_echoes * 2
-
-            assigned = template.assign_parameters(
-                {delay_param: timing.round_delay(time=single_delay)}, inplace=False
-            )
-            assigned.metadata["xval"] = total_delay
-            circuits.append(assigned)
+            circuit.sx(0)
+            circuit.measure_all()
+
+            circuit.metadata = {"xval": repetition}
+
+            circuits.append(circuit)
 
         return circuits
 
     def _metadata(self):
         metadata = super()._metadata()
         # Store measurement level and meas return if they have been
         # set for the experiment
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/t2ramsey.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/t2ramsey.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 import qiskit
 from qiskit import QuantumCircuit
 from qiskit.providers.backend import Backend
 
 from qiskit_experiments.framework import BackendTiming, BaseExperiment, Options
 from qiskit_experiments.library.characterization.analysis.t2ramsey_analysis import T2RamseyAnalysis
-from qiskit_experiments.warnings import qubit_deprecate
 
 
 class T2Ramsey(BaseExperiment):
     r"""An experiment to measure the Ramsey frequency and the qubit dephasing time
     sensitive to inhomogeneous broadening.
 
     # section: overview
@@ -75,15 +74,14 @@
         options = super()._default_experiment_options()
 
         options.delays = None
         options.osc_freq = 0.0
 
         return options
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         delays: Union[List[float], np.array],
         backend: Optional[Backend] = None,
         osc_freq: float = 0.0,
     ):
@@ -123,27 +121,22 @@
             circ.delay(timing.round_delay(time=delay), 0, timing.delay_unit)
             circ.rz(rotation_angle, 0)
             circ.barrier(0)
             circ.sx(0)
             circ.barrier(0)
             circ.measure(0, 0)
 
-            circ.metadata = {
-                "experiment_type": self._type,
-                "qubit": self.physical_qubits[0],
-                "xval": timing.delay_time(time=delay),
-                "osc_freq": self.experiment_options.osc_freq,
-                "unit": "s",
-            }
+            circ.metadata = {"xval": timing.delay_time(time=delay)}
 
             circuits.append(circ)
 
         return circuits
 
     def _metadata(self):
         metadata = super()._metadata()
         # Store measurement level and meas return if they have been
         # set for the experiment
         for run_opt in ["meas_level", "meas_return"]:
             if hasattr(self.run_options, run_opt):
                 metadata[run_opt] = getattr(self.run_options, run_opt)
+        metadata["osc_freq"] = self.experiment_options.osc_freq
         return metadata
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/tphi.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/tphi.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 from typing import List, Optional, Union, Sequence
 import numpy as np
 
 from qiskit import QiskitError
 from qiskit.providers import Backend
 from qiskit_experiments.framework.composite.batch_experiment import BatchExperiment
-from qiskit_experiments.warnings import qubit_deprecate
 from qiskit_experiments.library.characterization import (
     T1,
     T2Ramsey,
     T2Hahn,
     TphiAnalysis,
 )
 
@@ -60,15 +59,14 @@
     # section: see_also
         * :py:class:`qiskit_experiments.library.characterization.T1`
         * :py:class:`qiskit_experiments.library.characterization.T2Ramsey`
         * :py:class:`qiskit_experiments.library.characterization.T2Hahn`
 
     """
 
-    @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         delays_t1: List[Union[List[float], np.array]],
         delays_t2: List[Union[List[float], np.array]],
         t2type: str = "hahn",
         osc_freq: float = 0.0,
@@ -116,15 +114,20 @@
             exp_options["num_echoes"] = num_echoes
         else:
             raise QiskitError(f"Invalid T2 experiment type {t2type} specified.")
 
         analysis = TphiAnalysis([exp_t1.analysis, exp_t2.analysis])
 
         # Create batch experiment
-        super().__init__([exp_t1, exp_t2], backend=backend, analysis=analysis)
+        super().__init__(
+            [exp_t1, exp_t2],
+            flatten_results=True,
+            backend=backend,
+            analysis=analysis,
+        )
         self.set_experiment_options(**exp_options)
 
     def set_experiment_options(self, **fields):
         """Set the experiment options.
         Args:
             fields: The fields defining the options.
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/characterization/zz_ramsey.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/characterization/zz_ramsey.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 import numpy as np
 
 from qiskit import QuantumCircuit
 from qiskit.providers.backend import Backend
 from qiskit.circuit import Parameter, ParameterExpression
 
-from qiskit_experiments.warnings import deprecate_arguments
 from qiskit_experiments.framework import BackendTiming, BaseExperiment, Options
 from .analysis.zz_ramsey_analysis import ZZRamseyAnalysis
 
 
 class ZZRamsey(BaseExperiment):
     r"""An experiment to characterize the static :math:`ZZ` interaction for a qubit pair.
 
@@ -123,15 +122,14 @@
             «                                      0
 
     # section: analysis_ref
 
         :class:`ZZRamseyAnalysis`
     """
 
-    @deprecate_arguments({"qubits": "physical_qubits"}, "0.5")
     def __init__(
         self,
         physical_qubits: Tuple[int, int],
         backend: Union[Backend, None] = None,
         **experiment_options,
     ):
         """Create new experiment.
@@ -219,18 +217,14 @@
             dt_value: the value of the backend ``dt`` value. Used to convert
                 delay values into units of seconds.
             delay_unit: the unit of circuit delay instructions.
 
         Returns:
             Circuits for series 0 and 1
         """
-        metadata = {
-            "unit": "s",
-        }
-
         delay = Parameter("delay")
 
         timing = BackendTiming(self.backend)
 
         frequency = frequency if frequency is not None else self.frequency()
         # frequency is always in units of Hz.  delay_freq has inverse units to
         # the units of `delay`.
@@ -242,15 +236,15 @@
         if timing.delay_unit != "s":
             delay_freq = timing.dt * frequency
         else:
             delay_freq = frequency
 
         # Template circuit for series 0
         # Control qubit starting in |0> state, flipping to |1> in middle
-        circ0 = QuantumCircuit(2, 1, metadata=metadata.copy())
+        circ0 = QuantumCircuit(2, 1)
         circ0.metadata["series"] = "0"
 
         circ0.sx(0)
 
         circ0.barrier()
         circ0.delay(delay, 0, timing.delay_unit)
         circ0.barrier()
@@ -269,15 +263,15 @@
         circ0.x(1)
 
         circ0.barrier()
         circ0.measure(0, 0)
 
         # Template circuit for series 1
         # Control qubit starting in |1> state, flipping to |0> in middle
-        circ1 = QuantumCircuit(2, 1, metadata=metadata.copy())
+        circ1 = QuantumCircuit(2, 1)
         circ1.metadata["series"] = "1"
 
         circ1.x(1)
         circ1.sx(0)
 
         circ1.barrier()
         circ1.delay(delay, 0, timing.delay_unit)
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/quantum_volume/qv_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/quantum_volume/qv_analysis.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,52 +11,167 @@
 # that they have been altered from the originals.
 """
 Quantum Volume analysis class.
 """
 
 import math
 import warnings
-from typing import Optional
+from typing import List
 
 import numpy as np
 import uncertainties
 from qiskit_experiments.exceptions import AnalysisError
-from qiskit_experiments.curve_analysis.visualization import plot_scatter, plot_errorbar
 from qiskit_experiments.framework import (
     BaseAnalysis,
     AnalysisResultData,
     Options,
 )
+from qiskit_experiments.visualization import BasePlotter, MplDrawer
+
+
+class QuantumVolumePlotter(BasePlotter):
+    """Plotter for QuantumVolumeAnalysis
+
+    .. note::
+
+        This plotter only supports one series, named ``hops``, which it expects
+        to have an ``individual`` data key containing the individual heavy
+        output probabilities for each circuit in the experiment. Additional
+        series will be ignored.
+    """
+
+    @classmethod
+    def expected_series_data_keys(cls) -> List[str]:
+        """Returns the expected series data keys supported by this plotter.
+
+        Data Keys:
+            individual: Heavy-output probability fraction for each individual circuit
+        """
+        return ["individual"]
+
+    @classmethod
+    def expected_supplementary_data_keys(cls) -> List[str]:
+        """Returns the expected figures data keys supported by this plotter.
+
+        Data Keys:
+            depth: The depth of the quantun volume circuits used in the experiment
+        """
+        return ["depth"]
+
+    def set_supplementary_data(self, **data_kwargs):
+        """Sets supplementary data for the plotter.
+
+        Args:
+            data_kwargs: See :meth:`expected_supplementary_data_keys` for the
+                expected supplementary data keys.
+        """
+        # Hook method to capture the depth for inclusion in the plot title
+        if "depth" in data_kwargs:
+            self.set_figure_options(
+                figure_title=(
+                    f"Quantum Volume experiment for depth {data_kwargs['depth']}"
+                    " - accumulative hop"
+                ),
+            )
+        super().set_supplementary_data(**data_kwargs)
+
+    @classmethod
+    def _default_figure_options(cls) -> Options:
+        options = super()._default_figure_options()
+        options.xlabel = "Number of Trials"
+        options.ylabel = "Heavy Output Probability"
+        options.figure_title = "Quantum Volume experiment - accumulative hop"
+        options.series_params = {
+            "hop": {"color": "gray", "symbol": "."},
+            "threshold": {"color": "black", "linestyle": "dashed", "linewidth": 1},
+            "hop_cumulative": {"color": "r"},
+            "hop_twosigma": {"color": "lightgray"},
+        }
+        return options
+
+    @classmethod
+    def _default_options(cls) -> Options:
+        options = super()._default_options()
+        options.style["figsize"] = (6.4, 4.8)
+        options.style["axis_label_size"] = 14
+        options.style["symbol_size"] = 2
+        return options
+
+    def _plot_figure(self):
+        (hops,) = self.data_for("hops", ["individual"])
+        trials = np.arange(1, 1 + len(hops))
+        hop_accumulative = np.cumsum(hops) / trials
+        hop_twosigma = 2 * (hop_accumulative * (1 - hop_accumulative) / trials) ** 0.5
+
+        self.drawer.line(
+            trials,
+            hop_accumulative,
+            name="hop_cumulative",
+            label="Cumulative HOP",
+            legend=True,
+        )
+        self.drawer.hline(
+            2 / 3,
+            name="threshold",
+            label="Threshold",
+            legend=True,
+        )
+        self.drawer.scatter(
+            trials,
+            hops,
+            name="hop",
+            label="Individual HOP",
+            legend=True,
+            linewidth=1.5,
+        )
+        self.drawer.filled_y_area(
+            trials,
+            hop_accumulative - hop_twosigma,
+            hop_accumulative + hop_twosigma,
+            alpha=0.5,
+            legend=True,
+            name="hop_twosigma",
+            label="2σ",
+        )
+
+        self.drawer.set_figure_options(
+            ylim=(
+                max(hop_accumulative[-1] - 4 * hop_twosigma[-1], 0),
+                min(hop_accumulative[-1] + 4 * hop_twosigma[-1], 1),
+            ),
+        )
 
 
 class QuantumVolumeAnalysis(BaseAnalysis):
     r"""A class to analyze quantum volume experiments.
 
     # section: overview
         Calculate the quantum volume of the analysed system.
         The quantum volume is determined by the largest successful circuit depth.
-        A depth is successful if it has 'mean heavy-output probability' > 2/3 with confidence
+        A depth is successful if it has `mean heavy-output probability` > 2/3 with confidence
         level > 0.977 (corresponding to z_value = 2), and at least 100 trials have been ran.
         we assume the error (standard deviation) of the heavy output probability is due to a
         binomial distribution. The standard deviation for binomial distribution is
         :math:`\sqrt{(np(1-p))}`, where :math:`n` is the number of trials and :math:`p`
         is the success probability.
     """
 
     @classmethod
     def _default_options(cls) -> Options:
         """Return default analysis options.
 
         Analysis Options:
             plot (bool): Set ``True`` to create figure for fit result.
             ax (AxesSubplot): Optional. A matplotlib axis object to draw.
+            plotter (BasePlotter): Plotter object to use for figure generation.
         """
         options = super()._default_options()
         options.plot = True
         options.ax = None
+        options.plotter = QuantumVolumePlotter(MplDrawer())
         return options
 
     def _run_analysis(self, experiment_data):
         data = experiment_data.data()
         num_trials = len(data)
         depth = None
         heavy_output_prob_exp = []
@@ -73,16 +188,17 @@
             heavy_output_prob_exp.append(
                 self._calc_exp_heavy_output_probability(data_trial, heavy_output)
             )
 
         hop_result, qv_result = self._calc_quantum_volume(heavy_output_prob_exp, depth, num_trials)
 
         if self.options.plot:
-            ax = self._format_plot(hop_result, ax=self.options.ax)
-            figures = [ax.get_figure()]
+            self.options.plotter.set_series_data("hops", individual=hop_result.extra["HOPs"])
+            self.options.plotter.set_supplementary_data(depth=hop_result.extra["depth"])
+            figures = [self.options.plotter.figure()]
         else:
             figures = None
         return [hop_result, qv_result], figures
 
     @staticmethod
     def _calc_ideal_heavy_output(probabilities_vector, depth):
         """
@@ -171,27 +287,27 @@
 
         return confidence_level
 
     def _calc_quantum_volume(self, heavy_output_prob_exp, depth, trials):
         """
         Calc the quantum volume of the analysed system.
         quantum volume is determined by the largest successful depth.
-        A depth is successful if it has 'mean heavy-output probability' > 2/3 with confidence
+        A depth is successful if it has `mean heavy-output probability` > 2/3 with confidence
         level > 0.977 (corresponding to z_value = 2), and at least 100 trials have been ran.
         we assume the error (standard deviation) of the heavy output probability is due to a
         binomial distribution. standard deviation for binomial distribution is sqrt(np(1-p)),
         where n is the number of trials and p is the success probability.
 
         Returns:
             dict: quantum volume calculations -
             the quantum volume,
             whether the results passed the threshold,
             the confidence of the result,
             the heavy output probability for each trial,
-            the mean heavy output probability,
+            the mean heavy-output probability,
             the error of the heavy output probability,
             the depth of the circuit,
             the number of trials ran
         """
         quantum_volume = 1
         success = False
 
@@ -234,77 +350,7 @@
                 "success": success,
                 "confidence": confidence_level,
                 "depth": depth,
                 "trials": trials,
             },
         )
         return hop_result, qv_result
-
-    @staticmethod
-    def _format_plot(
-        hop_result: AnalysisResultData, ax: Optional["matplotlib.pyplot.AxesSubplot"] = None
-    ):
-        """Format the QV plot
-
-        Args:
-            hop_result: the heavy output probability analysis result.
-            ax: matplotlib axis to add plot to.
-
-        Returns:
-            AxesSubPlot: the matplotlib axes containing the plot.
-        """
-        trials = hop_result.extra["trials"]
-        heavy_probs = hop_result.extra["HOPs"]
-        trial_list = np.arange(1, trials + 1)  # x data
-
-        hop_accumulative = np.cumsum(heavy_probs) / trial_list
-        two_sigma = 2 * (hop_accumulative * (1 - hop_accumulative) / trial_list) ** 0.5
-
-        # Plot individual HOP as scatter
-        ax = plot_scatter(
-            trial_list,
-            heavy_probs,
-            ax=ax,
-            s=3,
-            zorder=3,
-            label="Individual HOP",
-        )
-        # Plot accumulative HOP
-        ax.plot(trial_list, hop_accumulative, color="r", label="Cumulative HOP")
-
-        # Plot two-sigma shaded area
-        ax = plot_errorbar(
-            trial_list,
-            hop_accumulative,
-            two_sigma,
-            ax=ax,
-            fmt="none",
-            ecolor="lightgray",
-            elinewidth=20,
-            capsize=0,
-            alpha=0.5,
-            label="2$\\sigma$",
-        )
-        # Plot 2/3 success threshold
-        ax.axhline(2 / 3, color="k", linestyle="dashed", linewidth=1, label="Threshold")
-
-        ax.set_ylim(
-            max(hop_accumulative[-1] - 4 * two_sigma[-1], 0),
-            min(hop_accumulative[-1] + 4 * two_sigma[-1], 1),
-        )
-
-        ax.set_xlabel("Number of Trials", fontsize=14)
-        ax.set_ylabel("Heavy Output Probability", fontsize=14)
-
-        ax.set_title(
-            "Quantum Volume experiment for depth "
-            + str(hop_result.extra["depth"])
-            + " - accumulative hop",
-            fontsize=14,
-        )
-
-        # Re-arrange legend order
-        handles, labels = ax.get_legend_handles_labels()
-        handles = [handles[1], handles[2], handles[0], handles[3]]
-        labels = [labels[1], labels[2], labels[0], labels[3]]
-        ax.legend(handles, labels)
-        return ax
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/quantum_volume/qv_experiment.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/quantum_volume/qv_experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,26 +13,20 @@
 Quantum Volume Experiment class.
 """
 
 from typing import Union, Sequence, Optional, List
 from numpy.random import Generator, default_rng
 from numpy.random.bit_generator import BitGenerator, SeedSequence
 
-try:
-    from qiskit import Aer
-
-    HAS_SIMULATION_BACKEND = True
-except ImportError:
-    HAS_SIMULATION_BACKEND = False
+from qiskit.utils.optionals import HAS_AER
 
 from qiskit import QuantumCircuit
 from qiskit.circuit.library import QuantumVolume as QuantumVolumeCircuit
 from qiskit import transpile
 from qiskit.providers.backend import Backend
-from qiskit_experiments.warnings import deprecate_arguments
 from qiskit_experiments.framework import BaseExperiment, Options
 from .qv_analysis import QuantumVolumeAnalysis
 
 
 class QuantumVolume(BaseExperiment):
     """An experiment to measure the largest random square circuit that can be run on a processor.
 
@@ -42,40 +36,42 @@
         circuit of equal width and depth that the computer successfully implements.
         Quantum computing systems with high-fidelity operations, high connectivity,
         large calibrated gate sets, and circuit rewriting toolchains are expected to
         have higher quantum volumes.
 
         The Quantum Volume is determined by the largest circuit depth :math:`d_{max}`,
         and equals to :math:`2^{d_{max}}`.
-        See `Qiskit Textbook
-        <https://qiskit.org/textbook/ch-quantum-hardware/measuring-quantum-volume.html>`_
+        See the `Qiskit Textbook
+        <https://github.com/Qiskit/textbook/blob/main/notebooks/quantum-hardware/measuring-quantum-volume.ipynb>`_
         for an explanation on the QV protocol.
 
         In the QV experiment we generate :class:`~qiskit.circuit.library.QuantumVolume` circuits on
         :math:`d` qubits, which contain :math:`d` layers, where each layer consists of random 2-qubit
         unitary gates from :math:`SU(4)`, followed by a random permutation on the :math:`d` qubits.
         Then these circuits run on the quantum backend and on an ideal simulator (either
         :class:`~qiskit_aer.AerSimulator` or :class:`~qiskit.quantum_info.Statevector`).
 
-        A depth :math:`d` QV circuit is successful if it has 'mean heavy-output probability' > 2/3 with
+        A depth :math:`d` QV circuit is successful if it has `mean heavy-output probability` > 2/3 with
         confidence level > 0.977 (corresponding to z_value = 2), and at least 100 trials have been ran.
 
         See :class:`QuantumVolumeAnalysis` documentation for additional
         information on QV experiment analysis.
 
     # section: analysis_ref
         :class:`QuantumVolumeAnalysis`
 
+    # section: manual
+        :doc:`/manuals/verification/quantum_volume`
+
     # section: reference
         .. ref_arxiv:: 1 1811.12926
         .. ref_arxiv:: 2 2008.08571
 
     """
 
-    @deprecate_arguments({"qubits": "physical_qubits"}, "0.5")
     def __init__(
         self,
         physical_qubits: Sequence[int],
         backend: Optional[Backend] = None,
         trials: Optional[int] = 100,
         seed: Optional[Union[int, SeedSequence, BitGenerator, Generator]] = None,
         simulation_backend: Optional[Backend] = None,
@@ -84,62 +80,64 @@
 
         Args:
             physical_qubits: list of physical qubits for the experiment.
             backend: Optional, the backend to run the experiment on.
             trials: The number of trials to run the quantum volume circuit.
             seed: Optional, seed used to initialize ``numpy.random.default_rng``
                   when generating circuits. The ``default_rng`` will be initialized
-                  with this seed value everytime :meth:`circuits` is called.
+                  with this seed value every time :meth:`circuits` is called.
             simulation_backend: The simulator backend to use to generate
                 the expected results. the simulator must have a 'save_probabilities'
-                method. If None :class:`AerSimulator` simulator will be used
-                (in case :class:`AerSimulator` is not
-                installed :class:`qiskit.quantum_info.Statevector` will be used).
+                method. If None, the :class:`qiskit_aer.AerSimulator` simulator will be used
+                (in case :external+qiskit_aer:doc:`qiskit-aer <index>` is not
+                installed, :class:`qiskit.quantum_info.Statevector` will be used).
         """
         super().__init__(physical_qubits, analysis=QuantumVolumeAnalysis(), backend=backend)
 
         # Set configurable options
         self.set_experiment_options(trials=trials, seed=seed)
 
-        if not simulation_backend and HAS_SIMULATION_BACKEND:
+        if not simulation_backend and HAS_AER:
+            from qiskit_aer import Aer
+
             self._simulation_backend = Aer.get_backend("aer_simulator")
         else:
             self._simulation_backend = simulation_backend
 
     @classmethod
     def _default_experiment_options(cls) -> Options:
         """Default experiment options.
 
         Experiment Options:
             trials (int): Optional, number of times to generate new Quantum Volume
                 circuits and calculate their heavy output.
             seed (None or int or SeedSequence or BitGenerator or Generator): A seed
                 used to initialize ``numpy.random.default_rng`` when generating circuits.
-                The ``default_rng`` will be initialized with this seed value everytime
+                The ``default_rng`` will be initialized with this seed value every time
                 :meth:`circuits` is called.
         """
         options = super()._default_experiment_options()
 
         options.trials = 100
         options.seed = None
 
         return options
 
     def _get_ideal_data(self, circuit: QuantumCircuit, **run_options) -> List[float]:
         """Return ideal measurement probabilities.
 
-        In case the user does not have Aer installed use Terra to calculate
-        the ideal state.
+        In case the user does not have Aer installed, use Qiskit's quantum info module
+        to calculate the ideal state.
 
         Args:
             circuit: the circuit to extract the ideal data from
             run_options: backend run options.
 
         Returns:
-            list: list of the probabilities for each state in the circuit (as Numpy array)
+            list: list of the probabilities for each state in the circuit.
         """
         ideal_circuit = circuit.remove_final_measurements(inplace=False)
         if self._simulation_backend:
             ideal_circuit.save_probabilities()
             # always transpile with optimization_level 0, even if the non ideal circuits will run
             # with different optimization level, because we need to compare the results to the
             # exact generated probabilities
@@ -148,15 +146,15 @@
             ideal_result = self._simulation_backend.run(ideal_circuit, **run_options).result()
             probabilities = ideal_result.data().get("probabilities")
         else:
             from qiskit.quantum_info import Statevector
 
             state_vector = Statevector(ideal_circuit)
             probabilities = state_vector.probabilities()
-        return probabilities
+        return list(probabilities)
 
     def circuits(self) -> List[QuantumCircuit]:
         """Return a list of Quantum Volume circuits.
 
         Returns:
             A list of :class:`QuantumCircuit`.
         """
@@ -165,15 +163,13 @@
         depth = self._num_qubits
 
         # Note: the trials numbering in the metadata is starting from 1 for each new experiment run
         for trial in range(1, self.experiment_options.trials + 1):
             qv_circ = QuantumVolumeCircuit(depth, depth, seed=rng)
             qv_circ.measure_active()
             qv_circ.metadata = {
-                "experiment_type": self._type,
                 "depth": depth,
                 "trial": trial,
-                "qubits": self.physical_qubits,
                 "ideal_probabilities": self._get_ideal_data(qv_circ),
             }
             circuits.append(qv_circ)
         return circuits
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -33,14 +33,22 @@
 .. autosummary::
     :toctree: ../stubs/
     :template: autosummary/analysis.rst
 
     RBAnalysis
     InterleavedRBAnalysis
 
+Synthesis
+=========
+
+.. autosummary::
+    :toctree: ../stubs/
+
+    RBDefaultCliffordSynthesis
+
 Utilities
 =========
 
 .. autosummary::
     :toctree: ../stubs/
 
     RBUtils
@@ -48,7 +56,8 @@
 """
 from .standard_rb import StandardRB
 from .interleaved_rb_experiment import InterleavedRB
 from .rb_analysis import RBAnalysis
 from .interleaved_rb_analysis import InterleavedRBAnalysis
 from .clifford_utils import CliffordUtils
 from .rb_utils import RBUtils
+from .clifford_synthesis import RBDefaultCliffordSynthesis
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/clifford_utils.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/clifford_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,37 +13,43 @@
 Utilities for using the Clifford group in randomized benchmarking.
 """
 
 import itertools
 import os
 from functools import lru_cache
 from numbers import Integral
-from typing import Optional, Union, Tuple, Sequence
+from typing import Optional, Union, Tuple, Sequence, Iterable
 
 import numpy as np
-import scipy.sparse
 from numpy.random import Generator, default_rng
 
 from qiskit.circuit import CircuitInstruction, Qubit
 from qiskit.circuit import Gate, Instruction
 from qiskit.circuit import QuantumCircuit, QuantumRegister
 from qiskit.circuit.library import SdgGate, HGate, SGate, XGate, YGate, ZGate
 from qiskit.compiler import transpile
 from qiskit.exceptions import QiskitError
 from qiskit.quantum_info import Clifford, random_clifford
-from qiskit_experiments.warnings import deprecated_function
+from qiskit.transpiler import CouplingMap, PassManager
+from qiskit.transpiler.passes.synthesis.high_level_synthesis import HLSConfig, HighLevelSynthesis
+from qiskit.utils.deprecation import deprecate_func
 
+DEFAULT_SYNTHESIS_METHOD = "rb_default"
 
 _DATA_FOLDER = os.path.join(os.path.dirname(__file__), "data")
 
 _CLIFFORD_COMPOSE_1Q = np.load(f"{_DATA_FOLDER}/clifford_compose_1q.npz")["table"]
 _CLIFFORD_INVERSE_1Q = np.load(f"{_DATA_FOLDER}/clifford_inverse_1q.npz")["table"]
-_CLIFFORD_COMPOSE_2Q = scipy.sparse.load_npz(f"{_DATA_FOLDER}/clifford_compose_2q_sparse.npz")
 _CLIFFORD_INVERSE_2Q = np.load(f"{_DATA_FOLDER}/clifford_inverse_2q.npz")["table"]
-
+_clifford_compose_2q_data = np.load(f"{_DATA_FOLDER}/clifford_compose_2q_dense_selected.npz")
+_CLIFFORD_COMPOSE_2Q_DENSE = _clifford_compose_2q_data["table"]
+# valid indices for the columns of the _CLIFFORD_COMPOSE_2Q_DENSE table
+_valid_sparse_indices = _clifford_compose_2q_data["valid_sparse_indices"]
+# map a clifford number to the index of _CLIFFORD_COMPOSE_2Q_DENSE
+_clifford_num_to_dense_index = {idx: ii for ii, idx in enumerate(_valid_sparse_indices)}
 
 # Transpilation utilities
 def _transpile_clifford_circuit(
     circuit: QuantumCircuit, physical_qubits: Sequence[int]
 ) -> QuantumCircuit:
     # Simplified transpile that only decomposes Clifford circuits and creates the layout.
     return _apply_qubit_layout(_decompose_clifford_ops(circuit), physical_qubits=physical_qubits)
@@ -104,45 +110,149 @@
                 clbits=instr.clbits,
             ),
         )
     self.global_phase += other.global_phase
     return self
 
 
-def _truncate_inactive_qubits(
-    circ: QuantumCircuit, active_qubits: Sequence[Qubit]
+def _synthesize_clifford(
+    clifford: Clifford,
+    basis_gates: Optional[Tuple[str]],
+    coupling_tuple: Optional[Tuple[Tuple[int, int]]] = None,
+    synthesis_method: str = DEFAULT_SYNTHESIS_METHOD,
 ) -> QuantumCircuit:
-    res = QuantumCircuit(active_qubits, name=circ.name, metadata=circ.metadata)
-    for inst in circ:
-        if all(q in active_qubits for q in inst.qubits):
-            res.append(inst)
-    res.calibrations = circ.calibrations
-    return res
+    """Synthesize a circuit of a Clifford element. The resulting circuit contains only
+    ``basis_gates`` and it complies with ``coupling_tuple``.
+
+    Args:
+        clifford: Clifford element to be converted
+        basis_gates: basis gates to use in the conversion
+        coupling_tuple: coupling map to use in the conversion in the form of tuple of edges
+        synthesis_method: conversion algorithm name
+
+    Returns:
+        Synthesized circuit
+    """
+    qc = QuantumCircuit(clifford.num_qubits, name=str(clifford))
+    qc.append(clifford, qc.qubits)
+    return _synthesize_clifford_circuit(
+        qc,
+        basis_gates=basis_gates,
+        coupling_tuple=coupling_tuple,
+        synthesis_method=synthesis_method,
+    )
 
 
 def _synthesize_clifford_circuit(
-    circuit: QuantumCircuit, basis_gates: Tuple[str]
+    circuit: QuantumCircuit,
+    basis_gates: Optional[Tuple[str]],
+    coupling_tuple: Optional[Tuple[Tuple[int, int]]] = None,
+    synthesis_method: str = DEFAULT_SYNTHESIS_METHOD,
 ) -> QuantumCircuit:
-    # synthesizes clifford circuits using given basis gates, for use during
-    # custom transpilation during RB circuit generation.
-    return transpile(circuit, basis_gates=list(basis_gates), optimization_level=1)
+    """Convert a Clifford circuit into one composed of ``basis_gates`` with
+    satisfying ``coupling_tuple`` using the specified synthesis method.
+
+    Args:
+        circuit: Clifford circuit to be converted
+        basis_gates: basis gates to use in the conversion
+        coupling_tuple: coupling map to use in the conversion in the form of tuple of edges
+        synthesis_method: name of Clifford synthesis algorithm to use
 
+    Returns:
+        Synthesized circuit
+    """
+    if basis_gates:
+        basis_gates = list(basis_gates)
+    coupling_map = CouplingMap(coupling_tuple) if coupling_tuple else None
+
+    # special handling for 1q or 2q case for speed
+    if circuit.num_qubits <= 2:
+        if synthesis_method == DEFAULT_SYNTHESIS_METHOD:
+            return transpile(
+                circuit,
+                basis_gates=basis_gates,
+                coupling_map=coupling_map,
+                optimization_level=1,
+            )
+        else:
+            # Provided custom synthesis method, re-synthesize Clifford circuit
+            # convert the circuit back to a Clifford object and then call the synthesis plugin
+            new_circuit = QuantumCircuit(circuit.num_qubits, name=circuit.name)
+            new_circuit.append(Clifford(circuit), new_circuit.qubits)
+            circuit = new_circuit
+
+    # for 3q+ or custom synthesis method, synthesizes clifford circuit
+    hls_config = HLSConfig(clifford=[(synthesis_method, {"basis_gates": basis_gates})])
+    pm = PassManager([HighLevelSynthesis(hls_config=hls_config, coupling_map=coupling_map)])
+    circuit = pm.run(circuit)
+    return circuit
 
-@lru_cache(maxsize=None)
+
+@lru_cache(maxsize=256)
 def _clifford_1q_int_to_instruction(
-    num: Integral, basis_gates: Optional[Tuple[str]]
+    num: Integral,
+    basis_gates: Optional[Tuple[str]],
+    synthesis_method: str = DEFAULT_SYNTHESIS_METHOD,
 ) -> Instruction:
-    return CliffordUtils.clifford_1_qubit_circuit(num, basis_gates).to_instruction()
+    return CliffordUtils.clifford_1_qubit_circuit(
+        num, basis_gates=basis_gates, synthesis_method=synthesis_method
+    ).to_instruction()
 
 
 @lru_cache(maxsize=11520)
 def _clifford_2q_int_to_instruction(
-    num: Integral, basis_gates: Optional[Tuple[str]]
+    num: Integral,
+    basis_gates: Optional[Tuple[str]],
+    coupling_tuple: Optional[Tuple[Tuple[int, int]]],
+    synthesis_method: str = DEFAULT_SYNTHESIS_METHOD,
+) -> Instruction:
+    return CliffordUtils.clifford_2_qubit_circuit(
+        num,
+        basis_gates=basis_gates,
+        coupling_tuple=coupling_tuple,
+        synthesis_method=synthesis_method,
+    ).to_instruction()
+
+
+def _hash_cliff(cliff):
+    return cliff.tableau.tobytes(), cliff.tableau.shape
+
+
+def _dehash_cliff(cliff_hash):
+    tableau = np.frombuffer(cliff_hash[0], dtype=bool).reshape(cliff_hash[1])
+    return Clifford(tableau)
+
+
+def _clifford_to_instruction(
+    clifford: Clifford,
+    basis_gates: Optional[Tuple[str]],
+    coupling_tuple: Optional[Tuple[Tuple[int, int]]],
+    synthesis_method: str = DEFAULT_SYNTHESIS_METHOD,
+) -> Instruction:
+    return _cached_clifford_to_instruction(
+        _hash_cliff(clifford),
+        basis_gates=basis_gates,
+        coupling_tuple=coupling_tuple,
+        synthesis_method=synthesis_method,
+    )
+
+
+@lru_cache(maxsize=256)
+def _cached_clifford_to_instruction(
+    cliff_hash: Tuple[str, Tuple[int, int]],
+    basis_gates: Optional[Tuple[str]],
+    coupling_tuple: Optional[Tuple[Tuple[int, int]]],
+    synthesis_method: str = DEFAULT_SYNTHESIS_METHOD,
 ) -> Instruction:
-    return CliffordUtils.clifford_2_qubit_circuit(num, basis_gates).to_instruction()
+    return _synthesize_clifford(
+        _dehash_cliff(cliff_hash),
+        basis_gates=basis_gates,
+        coupling_tuple=coupling_tuple,
+        synthesis_method=synthesis_method,
+    ).to_instruction()
 
 
 # The classes VGate and WGate are not actually used in the code - we leave them here to give
 # a better understanding of the composition of the layers for 2-qubit Cliffords.
 class VGate(Gate):
     """V Gate used in Clifford synthesis."""
 
@@ -199,15 +309,19 @@
     def clifford_2_qubit(cls, num):
         """Return the 2-qubit clifford element corresponding to ``num``,
         where ``num`` is between 0 and 11519.
         """
         return Clifford(cls.clifford_2_qubit_circuit(num), validate=False)
 
     @classmethod
-    @deprecated_function("0.6")
+    @deprecate_func(
+        since="0.5",
+        removal_timeline="after 0.6",
+        package_name="qiskit-experiments",
+    )
     def random_cliffords(
         cls, num_qubits: int, size: int = 1, rng: Optional[Union[int, Generator]] = None
     ):
         """Generate a list of random clifford elements"""
         if rng is None:
             rng = default_rng()
         elif isinstance(rng, int):
@@ -219,15 +333,19 @@
         if num_qubits == 2:
             samples = rng.integers(cls.NUM_CLIFFORD_2_QUBIT, size=size)
             return [Clifford(cls.clifford_2_qubit_circuit(i), validate=False) for i in samples]
 
         return [random_clifford(num_qubits, seed=rng) for _ in range(size)]
 
     @classmethod
-    @deprecated_function("0.6")
+    @deprecate_func(
+        since="0.5",
+        removal_timeline="after 0.6",
+        package_name="qiskit-experiments",
+    )
     def random_clifford_circuits(
         cls, num_qubits: int, size: int = 1, rng: Optional[Union[int, Generator]] = None
     ):
         """Generate a list of random clifford circuits"""
         if rng is None:
             rng = default_rng()
         elif isinstance(rng, int):
@@ -240,15 +358,20 @@
             samples = rng.integers(cls.NUM_CLIFFORD_2_QUBIT, size=size)
             return [cls.clifford_2_qubit_circuit(i) for i in samples]
 
         return [random_clifford(num_qubits, seed=rng).to_circuit() for _ in range(size)]
 
     @classmethod
     @lru_cache(maxsize=24)
-    def clifford_1_qubit_circuit(cls, num, basis_gates: Optional[Tuple[str, ...]] = None):
+    def clifford_1_qubit_circuit(
+        cls,
+        num,
+        basis_gates: Optional[Tuple[str, ...]] = None,
+        synthesis_method: str = DEFAULT_SYNTHESIS_METHOD,
+    ):
         """Return the 1-qubit clifford circuit corresponding to ``num``,
         where ``num`` is between 0 and 23.
         """
         unpacked = cls._unpack_num(num, cls.CLIFFORD_1_QUBIT_SIG)
         i, j, p = unpacked[0], unpacked[1], unpacked[2]
         qc = QuantumCircuit(1, name=f"Clifford-1Q({num})")
         if i == 1:
@@ -261,28 +384,36 @@
             qc.x(0)
         if p == 2:
             qc.y(0)
         if p == 3:
             qc.z(0)
 
         if basis_gates:
-            qc = _synthesize_clifford_circuit(qc, basis_gates)
+            qc = _synthesize_clifford_circuit(qc, basis_gates, synthesis_method=synthesis_method)
 
         return qc
 
     @classmethod
     @lru_cache(maxsize=11520)
-    def clifford_2_qubit_circuit(cls, num, basis_gates: Optional[Tuple[str, ...]] = None):
+    def clifford_2_qubit_circuit(
+        cls,
+        num,
+        basis_gates: Optional[Tuple[str, ...]] = None,
+        coupling_tuple: Optional[Tuple[Tuple[int, int]]] = None,
+        synthesis_method: str = DEFAULT_SYNTHESIS_METHOD,
+    ):
         """Return the 2-qubit clifford circuit corresponding to `num`
         where `num` is between 0 and 11519.
         """
         qc = QuantumCircuit(2, name=f"Clifford-2Q({num})")
         for layer, idx in enumerate(_layer_indices_from_num(num)):
             if basis_gates:
-                layer_circ = _transformed_clifford_layer(layer, idx, basis_gates)
+                layer_circ = _transformed_clifford_layer(
+                    layer, idx, basis_gates, coupling_tuple, synthesis_method=synthesis_method
+                )
             else:
                 layer_circ = _CLIFFORD_LAYER[layer][idx]
             _circuit_compose(qc, layer_circ, qubits=(0, 1))
 
         return qc
 
     @staticmethod
@@ -409,37 +540,30 @@
 
 ########
 # Functions for 2-qubit integer Clifford operations
 def compose_2q(lhs: Integral, rhs: Integral) -> Integral:
     """Return the composition of 2-qubit clifford integers."""
     num = lhs
     for layer, idx in enumerate(_layer_indices_from_num(rhs)):
-        circ = _CLIFFORD_LAYER[layer][idx]
-        num = _compose_num_with_circuit_2q(num, circ)
+        gate_numbers = _CLIFFORD_LAYER_NUMS[layer][idx]
+        for n in gate_numbers:
+            num = _CLIFFORD_COMPOSE_2Q_DENSE[num, _clifford_num_to_dense_index[n]]
     return num
 
 
 def inverse_2q(num: Integral) -> Integral:
     """Return the inverse of a 2-qubit clifford integer."""
     return _CLIFFORD_INVERSE_2Q[num]
 
 
 def num_from_2q_circuit(qc: QuantumCircuit) -> Integral:
     """Convert a given 2-qubit Clifford circuit to the corresponding integer."""
-    return _compose_num_with_circuit_2q(0, qc)
-
-
-def _compose_num_with_circuit_2q(num: Integral, qc: QuantumCircuit) -> Integral:
-    """Compose a number that represents a Clifford, with a Clifford circuit, and return the
-    number that represents the resulting Clifford."""
-    lhs = num
-    for inst in qc:
-        qubits = tuple(qc.find_bit(q).index for q in inst.qubits)
-        rhs = _num_from_2q_gate(op=inst.operation, qubits=qubits)
-        lhs = _CLIFFORD_COMPOSE_2Q[lhs, rhs]
+    lhs = 0
+    for rhs in _clifford_2q_nums_from_2q_circuit(qc):
+        lhs = _CLIFFORD_COMPOSE_2Q_DENSE[lhs, _clifford_num_to_dense_index[rhs]]
     return lhs
 
 
 def _num_from_2q_gate(
     op: Instruction, qubits: Optional[Union[Tuple[int, int], Tuple[int]]] = None
 ) -> int:
     """
@@ -553,26 +677,48 @@
 
 
 _CLIFFORD_LAYER = (
     _create_cliff_2q_layer_0(),
     _create_cliff_2q_layer_1(),
     _create_cliff_2q_layer_2(),
 )
-_NUM_LAYER_0 = 36
 _NUM_LAYER_1 = 20
 _NUM_LAYER_2 = 16
 
 
-@lru_cache(maxsize=None)
+def _clifford_2q_nums_from_2q_circuit(qc: QuantumCircuit) -> Iterable[Integral]:
+    """Yield Clifford numbers that represents the 2Q Clifford circuit."""
+    for inst in qc:
+        qubits = tuple(qc.find_bit(q).index for q in inst.qubits)
+        yield _num_from_2q_gate(op=inst.operation, qubits=qubits)
+
+
+# Construct mapping from Clifford layers to series of Clifford numbers
+_CLIFFORD_LAYER_NUMS = [
+    [tuple(_clifford_2q_nums_from_2q_circuit(qc)) for qc in _CLIFFORD_LAYER[layer]]
+    for layer in [0, 1, 2]
+]
+
+
+@lru_cache(maxsize=256)
 def _transformed_clifford_layer(
-    layer: int, index: Integral, basis_gates: Tuple[str, ...]
+    layer: int,
+    index: Integral,
+    basis_gates: Tuple[str, ...],
+    coupling_tuple: Optional[Tuple[Tuple[int, int]]],
+    synthesis_method: str = DEFAULT_SYNTHESIS_METHOD,
 ) -> QuantumCircuit:
     # Return the index-th quantum circuit of the layer translated with the basis_gates.
     # The result is cached for speed.
-    return _synthesize_clifford_circuit(_CLIFFORD_LAYER[layer][index], basis_gates)
+    return _synthesize_clifford_circuit(
+        _CLIFFORD_LAYER[layer][index],
+        basis_gates=basis_gates,
+        coupling_tuple=coupling_tuple,
+        synthesis_method=synthesis_method,
+    )
 
 
 def _num_from_layer_indices(triplet: Tuple[Integral, Integral, Integral]) -> Integral:
     """Return the clifford number corresponding to the input triplet."""
     num = triplet[0] * _NUM_LAYER_1 * _NUM_LAYER_2 + triplet[1] * _NUM_LAYER_2 + triplet[2]
     return num
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/interleaved_rb_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/interleaved_rb_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         default_options.result_parameters = ["alpha", "alpha_c"]
         default_options.average_method = "sample"
         return default_options
 
     def _generate_fit_guesses(
         self,
         user_opt: curve.FitOptions,
-        curve_data: curve.CurveData,
+        curve_data: curve.ScatterTable,
     ) -> Union[curve.FitOptions, List[curve.FitOptions]]:
         """Create algorithmic initial fit guess from analysis options and curve data.
 
         Args:
             user_opt: Fit options filled with user provided guess and bounds.
             curve_data: Formatted data collection to fit.
 
@@ -137,20 +137,20 @@
             alpha_c=(0, 1),
             b=(0, 1),
         )
 
         b_guess = 1 / 2**self._num_qubits
 
         # for standard RB curve
-        std_curve = curve_data.get_subset_of("standard")
+        std_curve = curve_data.filter(series="standard")
         alpha_std = curve.guess.rb_decay(std_curve.x, std_curve.y, b=b_guess)
         a_std = (std_curve.y[0] - b_guess) / (alpha_std ** std_curve.x[0])
 
         # for interleaved RB curve
-        int_curve = curve_data.get_subset_of("interleaved")
+        int_curve = curve_data.filter(series="interleaved")
         alpha_int = curve.guess.rb_decay(int_curve.x, int_curve.y, b=b_guess)
         a_int = (int_curve.y[0] - b_guess) / (alpha_int ** int_curve.x[0])
 
         alpha_c = min(alpha_int / alpha_std, 1.0)
 
         user_opt.p0.set_if_empty(
             b=b_guess,
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/interleaved_rb_experiment.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/interleaved_rb_experiment.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,29 +10,26 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 """
 Interleaved RB Experiment class.
 """
 import itertools
 import warnings
-from typing import Union, Iterable, Optional, List, Sequence, Tuple
+from typing import Union, Iterable, Optional, List, Sequence, Dict, Any
 
 from numpy.random import Generator
 from numpy.random.bit_generator import BitGenerator, SeedSequence
 
 from qiskit.circuit import QuantumCircuit, Instruction, Gate, Delay
-from qiskit.compiler import transpile
 from qiskit.exceptions import QiskitError
 from qiskit.providers.backend import Backend
 from qiskit.quantum_info import Clifford
-from qiskit.transpiler.exceptions import TranspilerError
-from qiskit_experiments.warnings import deprecate_arguments
 from qiskit_experiments.framework import Options
 from qiskit_experiments.framework.backend_timing import BackendTiming
-from .clifford_utils import _truncate_inactive_qubits
+from .clifford_utils import _synthesize_clifford
 from .clifford_utils import num_from_1q_circuit, num_from_2q_circuit
 from .interleaved_rb_analysis import InterleavedRBAnalysis
 from .standard_rb import StandardRB, SequenceElementType
 
 
 class InterleavedRB(StandardRB):
     """An experiment to characterize the error rate of a specific gate on a device.
@@ -46,20 +43,22 @@
         After running the two sequences on a backend, it calculates the probabilities to get back to
         the ground state, fits the two exponentially decaying curves, and estimates
         the interleaved gate error. See Ref. [1] for details.
 
     # section: analysis_ref
         :class:`InterleavedRBAnalysis`
 
+    # section: manual
+        :doc:`/manuals/verification/randomized_benchmarking`
+
     # section: reference
         .. ref_arxiv:: 1 1203.4550
 
     """
 
-    @deprecate_arguments({"qubits": "physical_qubits"}, "0.5")
     def __init__(
         self,
         interleaved_element: Union[QuantumCircuit, Gate, Delay, Clifford],
         physical_qubits: Sequence[int],
         lengths: Iterable[int],
         backend: Optional[Backend] = None,
         num_samples: int = 3,
@@ -68,28 +67,27 @@
         circuit_order: str = "RIRIRI",
     ):
         """Initialize an interleaved randomized benchmarking experiment.
 
         Args:
             interleaved_element: The element to interleave,
                     given either as a Clifford element, gate, delay or circuit.
-                    If the element contains any non-basis gates,
-                    it will be transpiled with ``transpiled_options`` of this experiment.
+                    All instructions in the element must be supported in the ``backend``(``target``).
                     If it is/contains a delay, its duration and unit must comply with
                     the timing constraints of the ``backend``
                     (:class:`~qiskit_experiments.framework.backend_timing.BackendTiming`
                     is useful to obtain valid delays).
                     Parameterized circuits/instructions are not allowed.
             physical_qubits: list of physical qubits for the experiment.
             lengths: A list of RB sequences lengths.
             backend: The backend to run the experiment on.
             num_samples: Number of samples to generate for each sequence length.
             seed: Optional, seed used to initialize ``numpy.random.default_rng``.
                   when generating circuits. The ``default_rng`` will be initialized
-                  with this seed value everytime :meth:`circuits` is called.
+                  with this seed value every time :meth:`circuits` is called.
             full_sampling: If True all Cliffords are independently sampled for
                            all lengths. If False for sample of lengths longer
                            sequences are constructed by appending additional
                            Clifford samples to shorter sequences.
             circuit_order: How to order the reference and the interleaved circuits.
                 ``"RIRIRI"`` (default) - Alternate a reference and an interleaved circuit. Or
                 ``"RRRIII"`` - Push all reference circuits first, then all interleaved ones.
@@ -181,28 +179,26 @@
     def circuits(self) -> List[QuantumCircuit]:
         """Return a list of RB circuits.
 
         Returns:
             A list of :class:`QuantumCircuit`.
 
         Raises:
-            QiskitError: If the ``interleaved_element`` provided to the constructor
-                cannot be transpiled.
+            QiskitError: If interleaved_element has non-supported instruction in the backend.
         """
         # Convert interleaved element to transpiled circuit operation and store it for speed
         self.__set_up_interleaved_op()
 
         # Build circuits of reference sequences
         reference_sequences = self._sample_sequences()
         reference_circuits = self._sequences_to_circuits(reference_sequences)
         for circ, seq in zip(reference_circuits, reference_sequences):
             circ.metadata = {
                 "xval": len(seq),
                 "group": "Clifford",
-                "physical_qubits": self.physical_qubits,
                 "interleaved": False,
             }
         # Build circuits of interleaved sequences
         interleaved_sequences = []
         for seq in reference_sequences:
             new_seq = []
             for elem in seq:
@@ -210,62 +206,58 @@
                 new_seq.append(self._interleaved_cliff)
             interleaved_sequences.append(new_seq)
         interleaved_circuits = self._sequences_to_circuits(interleaved_sequences)
         for circ, seq in zip(interleaved_circuits, reference_sequences):
             circ.metadata = {
                 "xval": len(seq),  # set length of the reference sequence
                 "group": "Clifford",
-                "physical_qubits": self.physical_qubits,
                 "interleaved": True,
             }
 
         if self.experiment_options.circuit_order == "RRRIII":
             return reference_circuits + interleaved_circuits
         # Default order: RIRIRI
         return list(itertools.chain.from_iterable(zip(reference_circuits, interleaved_circuits)))
 
     def _to_instruction(
-        self, elem: SequenceElementType, basis_gates: Optional[Tuple[str]] = None
+        self,
+        elem: SequenceElementType,
+        synthesis_options: Dict[str, Optional[Any]],
     ) -> Instruction:
         if elem is self._interleaved_cliff:
             return self._interleaved_op
 
-        return super()._to_instruction(elem, basis_gates)
+        return super()._to_instruction(elem, synthesis_options)
 
     def __set_up_interleaved_op(self) -> None:
         # Convert interleaved element to transpiled circuit operation and store it for speed
         self._interleaved_op = self._interleaved_element
-        basis_gates = self._get_basis_gates()
         # Convert interleaved element to circuit
         if isinstance(self._interleaved_op, Clifford):
-            self._interleaved_op = self._interleaved_op.to_circuit()
+            opts = self._get_synthesis_options()
+            self._interleaved_op = _synthesize_clifford(self._interleaved_op, **opts)
 
         if isinstance(self._interleaved_op, QuantumCircuit):
             interleaved_circ = self._interleaved_op
         elif isinstance(self._interleaved_op, Gate):
             interleaved_circ = QuantumCircuit(self.num_qubits, name=self._interleaved_op.name)
             interleaved_circ.append(self._interleaved_op, list(range(self.num_qubits)))
         else:  # Delay
             interleaved_circ = []
 
-        if basis_gates and any(i.operation.name not in basis_gates for i in interleaved_circ):
-            # Transpile circuit with non-basis gates and remove idling qubits
-            try:
-                interleaved_circ = transpile(
-                    interleaved_circ, self.backend, **vars(self.transpile_options)
+        # Validate if all instructions in the interleaved circuit are supported in the backend
+        if self.backend and hasattr(self.backend, "target"):
+            for inst in interleaved_circ:
+                qargs = tuple(
+                    self.physical_qubits[interleaved_circ.find_bit(q).index] for q in inst.qubits
                 )
-            except TranspilerError as err:
-                raise QiskitError("Failed to transpile interleaved_element.") from err
-            interleaved_circ = _truncate_inactive_qubits(
-                interleaved_circ, active_qubits=interleaved_circ.qubits[: self.num_qubits]
-            )
-            # Convert transpiled circuit to operation
-            if len(interleaved_circ) == 1:
-                self._interleaved_op = interleaved_circ.data[0].operation
-            else:
-                self._interleaved_op = interleaved_circ
+                if not self.backend.target.instruction_supported(inst.operation.name, qargs):
+                    raise QiskitError(
+                        f"{inst.operation.name} in interleaved element is not supported"
+                        f" on qubits {qargs} in the backend."
+                    )
 
         # Store interleaved operation as Instruction
         if isinstance(self._interleaved_op, QuantumCircuit):
             if not self._interleaved_op.name.startswith("Clifford"):
                 self._interleaved_op.name = f"Clifford-{self._interleaved_op.name}"
             self._interleaved_op = self._interleaved_op.to_instruction()
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/rb_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/rb_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         default_options.average_method = "sample"
 
         return default_options
 
     def _generate_fit_guesses(
         self,
         user_opt: curve.FitOptions,
-        curve_data: curve.CurveData,
+        curve_data: curve.ScatterTable,
     ) -> Union[curve.FitOptions, List[curve.FitOptions]]:
         """Create algorithmic initial fit guess from analysis options and curve data.
 
         Args:
             user_opt: Fit options filled with user provided guess and bounds.
             curve_data: Formatted data collection to fit.
 
@@ -396,15 +396,15 @@
     for analysis_data in extra_analyses:
         if (
             not analysis_data.name.startswith("EPG_")
             or len(analysis_data.device_components) > 1
             or not str(analysis_data.device_components[0]).startswith("Q")
         ):
             continue
-        qind = analysis_data.device_components[0]._index
+        qind = analysis_data.device_components[0].index
         gate = analysis_data.name[4:]
         formatted_key = (qind,), gate
         epg_1qs[formatted_key] = analysis_data.value
 
     if not epg_1qs:
         return epc
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/rb_utils.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/rb_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/randomized_benchmarking/standard_rb.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/randomized_benchmarking/standard_rb.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,45 +8,45 @@
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 """
 Standard RB Experiment class.
 """
-import logging
 import functools
+import logging
 from collections import defaultdict
 from numbers import Integral
-from typing import Union, Iterable, Optional, List, Sequence, Tuple
+from typing import Union, Iterable, Optional, List, Sequence, Dict, Any
 
 import numpy as np
+import rustworkx as rx
 from numpy.random import Generator, default_rng
 from numpy.random.bit_generator import BitGenerator, SeedSequence
 
-from qiskit.circuit import QuantumCircuit, Instruction, Barrier
+from qiskit.circuit import CircuitInstruction, QuantumCircuit, Instruction, Barrier, Gate
 from qiskit.exceptions import QiskitError
 from qiskit.providers import BackendV2Converter
 from qiskit.providers.backend import Backend, BackendV1, BackendV2
 from qiskit.pulse.instruction_schedule_map import CalibrationPublisher
 from qiskit.quantum_info import Clifford
 from qiskit.quantum_info.random import random_clifford
 from qiskit.transpiler import CouplingMap
-
-from qiskit_experiments.warnings import deprecate_arguments
 from qiskit_experiments.framework import BaseExperiment, Options
 from qiskit_experiments.framework.restless_mixin import RestlessMixin
-
 from .clifford_utils import (
     CliffordUtils,
+    DEFAULT_SYNTHESIS_METHOD,
     compose_1q,
     compose_2q,
     inverse_1q,
     inverse_2q,
     _clifford_1q_int_to_instruction,
     _clifford_2q_int_to_instruction,
+    _clifford_to_instruction,
     _transpile_clifford_circuit,
 )
 from .rb_analysis import RBAnalysis
 
 LOG = logging.getLogger(__name__)
 
 
@@ -57,15 +57,15 @@
     """An experiment to characterize the error rate of a gate set on a device.
 
     # section: overview
 
     Randomized Benchmarking (RB) is an efficient and robust method
     for estimating the average error rate of a set of quantum gate operations.
     See `Qiskit Textbook
-    <https://qiskit.org/textbook/ch-quantum-hardware/randomized-benchmarking.html>`_
+    <https://github.com/Qiskit/textbook/blob/main/notebooks/quantum-hardware/randomized-benchmarking.ipynb>`_
     for an explanation on the RB method.
 
     A standard RB experiment generates sequences of random Cliffords
     such that the unitary computed by the sequences is the identity.
     After running the sequences on a backend, it calculates the probabilities to get back to
     the ground state, fits an exponentially decaying curve, and estimates
     the Error Per Clifford (EPC), as described in Refs. [1, 2].
@@ -74,20 +74,22 @@
         In 0.5.0, the default value of ``optimization_level`` in ``transpile_options`` changed
         from ``0`` to ``1`` for RB experiments. That may result in shorter RB circuits
         hence slower decay curves than before.
 
     # section: analysis_ref
         :class:`RBAnalysis`
 
+    # section: manual
+        :doc:`/manuals/verification/randomized_benchmarking`
+
     # section: reference
         .. ref_arxiv:: 1 1009.3639
         .. ref_arxiv:: 2 1109.6887
     """
 
-    @deprecate_arguments({"qubits": "physical_qubits"}, "0.5")
     def __init__(
         self,
         physical_qubits: Sequence[int],
         lengths: Iterable[int],
         backend: Optional[Backend] = None,
         num_samples: int = 3,
         seed: Optional[Union[int, SeedSequence, BitGenerator, Generator]] = None,
@@ -98,15 +100,15 @@
         Args:
             physical_qubits: List of physical qubits for the experiment.
             lengths: A list of RB sequences lengths.
             backend: The backend to run the experiment on.
             num_samples: Number of samples to generate for each sequence length.
             seed: Optional, seed used to initialize ``numpy.random.default_rng``.
                   when generating circuits. The ``default_rng`` will be initialized
-                  with this seed value everytime :meth:`circuits` is called.
+                  with this seed value every time :meth:`circuits` is called.
             full_sampling: If True all Cliffords are independently sampled for all lengths.
                            If False for sample of lengths longer sequences are constructed
                            by appending additional samples to shorter sequences.
                            The default is False.
 
         Raises:
             QiskitError: If any invalid argument is supplied.
@@ -137,26 +139,29 @@
         """Default experiment options.
 
         Experiment Options:
             lengths (List[int]): A list of RB sequences lengths.
             num_samples (int): Number of samples to generate for each sequence length.
             seed (None or int or SeedSequence or BitGenerator or Generator): A seed
                 used to initialize ``numpy.random.default_rng`` when generating circuits.
-                The ``default_rng`` will be initialized with this seed value everytime
+                The ``default_rng`` will be initialized with this seed value every time
                 :meth:`circuits` is called.
             full_sampling (bool): If True all Cliffords are independently sampled for
                 all lengths. If False for sample of lengths longer sequences are constructed
                 by appending additional Clifford samples to shorter sequences.
+            clifford_synthesis_method (str): The name of the Clifford synthesis plugin to use
+                for building circuits of RB sequences.
         """
         options = super()._default_experiment_options()
         options.update_options(
             lengths=None,
             num_samples=None,
             seed=None,
             full_sampling=None,
+            clifford_synthesis_method=DEFAULT_SYNTHESIS_METHOD,
         )
 
         return options
 
     @classmethod
     def _default_transpile_options(cls) -> Options:
         """Default transpiler options for transpiling RB circuits."""
@@ -182,15 +187,14 @@
         # Convert each sequence into circuit and append the inverse to the end.
         circuits = self._sequences_to_circuits(sequences)
         # Add metadata for each circuit
         for circ, seq in zip(circuits, sequences):
             circ.metadata = {
                 "xval": len(seq),
                 "group": "Clifford",
-                "physical_qubits": self.physical_qubits,
             }
         return circuits
 
     def _sample_sequences(self) -> List[Sequence[SequenceElementType]]:
         """Sample RB sequences
 
         Returns:
@@ -206,195 +210,206 @@
             for _ in range(self.experiment_options.num_samples):
                 longest_seq = self.__sample_sequence(max(self.experiment_options.lengths), rng)
                 for length in self.experiment_options.lengths:
                     sequences.append(longest_seq[:length])
 
         return sequences
 
-    def _get_basis_gates(self) -> Optional[Tuple[str, ...]]:
-        """Get sorted basis gates to use in basis transformation during circuit generation.
+    def _get_synthesis_options(self) -> Dict[str, Optional[Any]]:
+        """Get options for Clifford synthesis from the backend information as a dictionary.
 
-        - Return None if this experiment is an RB with 3 or more qubits.
-        - Return None if no basis gates are supplied via ``backend`` or ``transpile_options``.
-        - Return None if all 2q-gates supported on the physical qubits of the backend are one-way
-        directed (e.g. cx(0, 1) is supported but cx(1, 0) is not supported).
-
-        In all those case when None are returned, basis transformation will be skipped in the
-        circuit generation step (i.e. :meth:`circuits`) and it will be done in the successive
-        transpilation step (i.e. :meth:`_transpiled_circuits`) that calls :func:`transpile`.
+        The options include:
+        - "basis_gates": Sorted basis gate names.
+            Return None if no basis gates are supplied via ``backend`` or ``transpile_options``.
+        - "coupling_tuple": Reduced coupling map in the form of tuple of edges in the coupling graph.
+            Return None if no coupling map are supplied via ``backend`` or ``transpile_options``.
 
         Returns:
-            Sorted basis gate names.
+            Synthesis options as a dictionary.
         """
-        # 3 or more qubits case: Return None (skip basis transformation in circuit generation)
-        if self.num_qubits > 2:
-            return None
-
-        # 1 qubit case: Return all basis gates (or None if no basis gates are supplied)
-        if self.num_qubits == 1:
-            basis_gates = self.transpile_options.get("basis_gates", None)
-            if not basis_gates and self.backend:
-                if isinstance(self.backend, BackendV2):
-                    basis_gates = self.backend.operation_names
-                elif isinstance(self.backend, BackendV1):
-                    basis_gates = self.backend.configuration().basis_gates
-            return tuple(sorted(basis_gates)) if basis_gates else None
-
-        def is_bidirectional(coupling_map):
-            if coupling_map is None:
-                # None for a coupling map implies all-to-all coupling
-                return True
-            return len(coupling_map.reduce(self.physical_qubits).get_edges()) == 2
-
-        # 2 qubits case: Return all basis gates except for one-way directed 2q-gates.
-        # Return None if there is no bidirectional 2q-gates in basis gates.
-        if self.num_qubits == 2:
-            basis_gates = self.transpile_options.get("basis_gates", [])
-            if not basis_gates and self.backend:
-                if isinstance(self.backend, BackendV2) and self.backend.target:
-                    has_bidirectional_2q_gates = False
-                    for op_name in self.backend.target:
-                        if self.backend.target.operation_from_name(op_name).num_qubits == 2:
-                            if is_bidirectional(self.backend.target.build_coupling_map(op_name)):
-                                has_bidirectional_2q_gates = True
-                            else:
-                                continue
-                        basis_gates.append(op_name)
-                    if not has_bidirectional_2q_gates:
-                        basis_gates = None
-                elif isinstance(self.backend, BackendV1):
-                    cmap = self.backend.configuration().coupling_map
-                    if cmap is None or is_bidirectional(CouplingMap(cmap)):
-                        basis_gates = self.backend.configuration().basis_gates
-            return tuple(sorted(basis_gates)) if basis_gates else None
-
-        return None
+        basis_gates = self.transpile_options.get("basis_gates", [])
+        coupling_map = self.transpile_options.get("coupling_map", None)
+        if coupling_map:
+            coupling_map = coupling_map.reduce(self.physical_qubits)
+        if not (basis_gates and coupling_map) and self.backend:
+            if isinstance(self.backend, BackendV2) and "simulator" in self.backend.name:
+                basis_gates = basis_gates if basis_gates else self.backend.target.operation_names
+                coupling_map = coupling_map if coupling_map else None
+            elif isinstance(self.backend, BackendV2):
+                gate_ops = [op for op in self.backend.target.operations if isinstance(op, Gate)]
+                backend_basis_gates = [op.name for op in gate_ops if op.num_qubits != 2]
+                backend_cmap = None
+                for op in gate_ops:
+                    if op.num_qubits != 2:
+                        continue
+                    cmap = self.backend.target.build_coupling_map(op.name)
+                    if cmap is None:
+                        backend_basis_gates.append(op.name)
+                    else:
+                        reduced = cmap.reduce(self.physical_qubits)
+                        if rx.is_weakly_connected(reduced.graph):
+                            backend_basis_gates.append(op.name)
+                            backend_cmap = reduced
+                            # take the first non-global 2q gate if backend has multiple 2q gates
+                            break
+                basis_gates = basis_gates if basis_gates else backend_basis_gates
+                coupling_map = coupling_map if coupling_map else backend_cmap
+            elif isinstance(self.backend, BackendV1):
+                backend_basis_gates = self.backend.configuration().basis_gates
+                backend_cmap = self.backend.configuration().coupling_map
+                if backend_cmap:
+                    backend_cmap = CouplingMap(backend_cmap).reduce(self.physical_qubits)
+                basis_gates = basis_gates if basis_gates else backend_basis_gates
+                coupling_map = coupling_map if coupling_map else backend_cmap
+
+        return {
+            "basis_gates": tuple(sorted(basis_gates)) if basis_gates else None,
+            "coupling_tuple": tuple(sorted(coupling_map.get_edges())) if coupling_map else None,
+            "synthesis_method": self.experiment_options["clifford_synthesis_method"],
+        }
 
     def _sequences_to_circuits(
         self, sequences: List[Sequence[SequenceElementType]]
     ) -> List[QuantumCircuit]:
         """Convert an RB sequence into circuit and append the inverse to the end.
 
         Returns:
             A list of RB circuits.
         """
-        basis_gates = self._get_basis_gates()
+        synthesis_opts = self._get_synthesis_options()
         # Circuit generation
         circuits = []
         for i, seq in enumerate(sequences):
             if (
                 self.experiment_options.full_sampling
                 or i % len(self.experiment_options.lengths) == 0
             ):
                 prev_elem, prev_seq = self.__identity_clifford(), []
 
             circ = QuantumCircuit(self.num_qubits)
             for elem in seq:
-                circ.append(self._to_instruction(elem, basis_gates), circ.qubits)
-                circ.append(Barrier(self.num_qubits), circ.qubits)
+                circ.append(self._to_instruction(elem, synthesis_opts), circ.qubits)
+                circ._append(CircuitInstruction(Barrier(self.num_qubits), circ.qubits))
 
             # Compute inverse, compute only the difference from the previous shorter sequence
             prev_elem = self.__compose_clifford_seq(prev_elem, seq[len(prev_seq) :])
             prev_seq = seq
             inv = self.__adjoint_clifford(prev_elem)
 
-            circ.append(self._to_instruction(inv, basis_gates), circ.qubits)
+            circ.append(self._to_instruction(inv, synthesis_opts), circ.qubits)
             circ.measure_all()  # includes insertion of the barrier before measurement
             circuits.append(circ)
         return circuits
 
     def __sample_sequence(self, length: int, rng: Generator) -> Sequence[SequenceElementType]:
         # Sample an RB sequence with the given length.
         # Return integer instead of Clifford object for 1 or 2 qubits case for speed
         if self.num_qubits == 1:
             return rng.integers(CliffordUtils.NUM_CLIFFORD_1_QUBIT, size=length)
         if self.num_qubits == 2:
             return rng.integers(CliffordUtils.NUM_CLIFFORD_2_QUBIT, size=length)
-        # Return circuit object instead of Clifford object for 3 or more qubits case for speed
-        return [random_clifford(self.num_qubits, rng).to_circuit() for _ in range(length)]
+        # Return Clifford object for 3 or more qubits case
+        return [random_clifford(self.num_qubits, rng) for _ in range(length)]
 
     def _to_instruction(
-        self, elem: SequenceElementType, basis_gates: Optional[Tuple[str, ...]] = None
+        self,
+        elem: SequenceElementType,
+        synthesis_options: Dict[str, Optional[Any]],
     ) -> Instruction:
+        """Return the instruction of a Clifford element.
+
+        The resulting instruction contains a circuit definition with ``basis_gates`` and
+        it complies with ``coupling_tuple``, which is specified in ``synthesis_options``.
+
+        Args:
+            elem: a Clifford element to be converted
+            synthesis_options: options for synthesizing the Clifford element
+
+        Returns:
+            Converted instruction
+        """
         # Switching for speed up
         if isinstance(elem, Integral):
             if self.num_qubits == 1:
-                return _clifford_1q_int_to_instruction(elem, basis_gates)
+                return _clifford_1q_int_to_instruction(
+                    elem,
+                    basis_gates=synthesis_options["basis_gates"],
+                    synthesis_method=synthesis_options["synthesis_method"],
+                )
             if self.num_qubits == 2:
-                return _clifford_2q_int_to_instruction(elem, basis_gates)
+                return _clifford_2q_int_to_instruction(elem, **synthesis_options)
 
-        return elem.to_instruction()
+        return _clifford_to_instruction(elem, **synthesis_options)
 
     def __identity_clifford(self) -> SequenceElementType:
         if self.num_qubits <= 2:
             return 0
         return Clifford(np.eye(2 * self.num_qubits))
 
     def __compose_clifford_seq(
         self, base_elem: SequenceElementType, elements: Sequence[SequenceElementType]
     ) -> SequenceElementType:
         if self.num_qubits <= 2:
             return functools.reduce(
                 compose_1q if self.num_qubits == 1 else compose_2q, elements, base_elem
             )
-        # 3 or more qubits: compose Clifford from circuits for speed
-        circ = QuantumCircuit(self.num_qubits)
+        # 3 or more qubits
+        res = base_elem
         for elem in elements:
-            circ.compose(elem, inplace=True)
-        return base_elem.compose(Clifford.from_circuit(circ))
+            res = res.compose(elem)
+        return res
 
     def __adjoint_clifford(self, op: SequenceElementType) -> SequenceElementType:
         if self.num_qubits == 1:
             return inverse_1q(op)
         if self.num_qubits == 2:
             return inverse_2q(op)
         if isinstance(op, QuantumCircuit):
             return Clifford.from_circuit(op).adjoint()
         return op.adjoint()
 
     def _transpiled_circuits(self) -> List[QuantumCircuit]:
         """Return a list of experiment circuits, transpiled."""
         has_custom_transpile_option = (
-            not set(vars(self.transpile_options)).issubset({"basis_gates", "optimization_level"})
+            not set(vars(self.transpile_options)).issubset(
+                {"basis_gates", "coupling_map", "optimization_level"}
+            )
             or self.transpile_options.get("optimization_level", 1) != 1
         )
-        has_no_undirected_2q_basis = self._get_basis_gates() is None
-        if self.num_qubits > 2 or has_custom_transpile_option or has_no_undirected_2q_basis:
+        if has_custom_transpile_option:
             transpiled = super()._transpiled_circuits()
         else:
             transpiled = [
                 _transpile_clifford_circuit(circ, physical_qubits=self.physical_qubits)
                 for circ in self.circuits()
             ]
-            # Set custom calibrations provided in backend
-            if isinstance(self.backend, BackendV2):
-                qargs_patterns = [self.physical_qubits]  # for self.num_qubits == 1
+            # Set custom calibrations provided in backend (excluding simulators)
+            if isinstance(self.backend, BackendV2) and "simulator" not in self.backend.name:
+                qargs_patterns = [self.physical_qubits]  # for 1q or 3q+ case
                 if self.num_qubits == 2:
                     qargs_patterns = [
                         (self.physical_qubits[0],),
                         (self.physical_qubits[1],),
                         self.physical_qubits,
                         (self.physical_qubits[1], self.physical_qubits[0]),
                     ]
 
+                qargs_supported = self.backend.target.qargs
                 instructions = []  # (op_name, qargs) for each element where qargs means qubit tuple
                 for qargs in qargs_patterns:
-                    for op_name in self.backend.target.operation_names_for_qargs(qargs):
-                        instructions.append((op_name, qargs))
+                    if qargs in qargs_supported:
+                        for op_name in self.backend.target.operation_names_for_qargs(qargs):
+                            instructions.append((op_name, qargs))
 
                 common_calibrations = defaultdict(dict)
                 for op_name, qargs in instructions:
                     inst_prop = self.backend.target[op_name].get(qargs, None)
                     if inst_prop is None:
                         continue
-                    try:
-                        schedule = inst_prop.calibration
-                    except AttributeError:
-                        # TODO remove after qiskit-terra/#9681 is in stable release.
-                        schedule = None
+                    schedule = inst_prop.calibration
                     if schedule is None:
                         continue
                     publisher = schedule.metadata.get("publisher", CalibrationPublisher.QISKIT)
                     if publisher != CalibrationPublisher.BACKEND_PROVIDER:
                         common_calibrations[op_name][(qargs, tuple())] = schedule
 
                 for circ in transpiled:
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,16 +48,14 @@
 
 Fitter functions for state reconstruction in tomography analysis
 
 .. autosummary::
     :toctree: ../stubs/
 
     fitters.linear_inversion
-    fitters.scipy_gaussian_lstsq
-    fitters.scipy_linear_lstsq
     fitters.cvxpy_gaussian_lstsq
     fitters.cvxpy_linear_lstsq
 
 
 Basis Classes
 =============
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/basis/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/basis/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/basis/base_basis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/basis/base_basis.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     * The :meth:`~.PreparationBasis.matrix_shape` method which returns the shape of subsystem
       dimensions of the density matrix state on the specified qubits.
     """
 
     @abstractmethod
     def matrix_shape(self, qubits: Sequence[int]) -> Tuple[int, ...]:
-        """Return the shape of subsystem dimensions of the state attr:`~matrix`.
+        """Return the shape of subsystem dimensions of the state :attr:`~matrix`.
 
         Args:
             qubits: the physical qubit subsystems.
 
         Returns:
             A tuple of subsystem dimensions for the specified qubits.
         """
@@ -166,15 +166,15 @@
 
         Returns:
             A tuple of the number of measurement outcomes for specified qubits.
         """
 
     @abstractmethod
     def matrix_shape(self, qubits: Sequence[int]) -> Tuple[int, ...]:
-        """Return the shape of subsystem dimensions of a POVM attr:`~matrix`.
+        """Return the shape of subsystem dimensions of a POVM :attr:`~matrix`.
 
         Args:
             qubits: the physical qubit subsystems.
 
         Returns:
             A tuple of subsystem dimensions for the specified qubits.
         """
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/basis/cache_method.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/basis/cache_method.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/basis/local_basis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/basis/local_basis.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
             # TODO: In the future we could add support for different orderings
             #       of qubits by permuting the returned POVMS
             states = self._qubit_states[qubits]
             if index in states:
                 return states[index]
 
             # Look up custom 0 init state for specified qubits
-            # TODO: Add support for noisy instuctions
+            # TODO: Add support for noisy instructions
             if not self._instructions:
                 raise NotImplementedError(
                     f"Basis {self.name} does not define circuits to construct POVMs from"
                 )
             key0 = num_qubits * (0,)
             if key0 in states:
                 circuit = _tensor_product_circuit(self._instructions, index, self._name)
@@ -485,15 +485,15 @@
             # TODO: In the future we could add support for different orderings
             #       of qubits by permuting the returned POVMS
             povms = self._qubit_povms[qubits]
             if index in povms:
                 return povms[index]
 
             # Look up custom Z-default POVM for specified qubits
-            # TODO: Add support for noisy instuctions
+            # TODO: Add support for noisy instructions
             if not self._instructions:
                 raise NotImplementedError(
                     f"Basis {self.name} does not define circuits to construct POVMs from"
                 )
             key0 = num_qubits * (0,)
             if key0 in povms:
                 circuit = _tensor_product_circuit(self._instructions, index, self._name)
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/basis/pauli_basis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/basis/pauli_basis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/fitters/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,9 +11,8 @@
 # that they have been altered from the originals.
 
 """Tomography fitter functions"""
 
 from .fitter_data import tomography_fitter_data
 from .postprocess_fit import postprocess_fitter
 from .lininv import linear_inversion
-from .scipy_lstsq import scipy_linear_lstsq, scipy_gaussian_lstsq
 from .cvxpy_lstsq import cvxpy_linear_lstsq, cvxpy_gaussian_lstsq
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/cvxpy_lstsq.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/fitters/cvxpy_lstsq.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,22 +97,22 @@
         of qubits try the
         :func:`~qiskit_experiments.library.tomography.fitters.linear_inversion`
         fitter function.
 
     Args:
         outcome_data: measurement outcome frequency data.
         shot_data: basis measurement total shot data.
-        measurement_data: measurement basis indice data.
-        preparation_data: preparation basis indice data.
+        measurement_data: measurement basis index data.
+        preparation_data: preparation basis index data.
         measurement_basis: Optional, measurement matrix basis.
         preparation_basis: Optional, preparation matrix basis.
         measurement_qubits: Optional, the physical qubits that were measured.
             If None they are assumed to be ``[0, ..., M-1]`` for M measured qubits.
         preparation_qubits: Optional, the physical qubits that were prepared.
-            If None they are assumed to be ``[0, ..., N-1]`` for N preparated qubits.
+            If None they are assumed to be ``[0, ..., N-1]`` for N prepared qubits.
         conditional_measurement_indices: Optional, conditional measurement data
             indices. If set this will return a list of fitted states conditioned
             on a fixed basis measurement of these qubits.
         conditional_preparation_indices: Optional, conditional preparation data
             indices. If set this will return a list of fitted states conditioned
             on a fixed basis preparation of these qubits.
         trace: trace constraint for the fitted matrix. If "auto" this will be set
@@ -214,15 +214,15 @@
                 preparation_qubits=preparation_qubits,
                 weights=cond_weights,
                 conditional_measurement_indices=conditional_measurement_indices,
                 conditional_preparation_indices=conditional_preparation_indices,
             )
 
             # Since CVXPY only works with real variables we must specify the real
-            # and imaginary parts of matrices seperately: rho = rho_r + 1j * rho_i
+            # and imaginary parts of matrices separately: rho = rho_r + 1j * rho_i
 
             num_circ_components, num_tomo_components, _ = probability_data.shape
             dim = int(np.sqrt(basis_matrix.shape[1]))
 
             # Generate list of conditional components for block diagonal matrix
             # rho = sum_k |k><k| \otimes rho(k)
             rhos_r = []
@@ -304,15 +304,15 @@
                         rhos_i[idx]
                     )
                     data = probability_data[i, j]
                     args.append(model - data)
                     idx += 1
 
             # Combine all variables and constraints into a joint optimization problem
-            # if tehre is a joint constraint
+            # if there is a joint constraint
             if joint_cons:
                 args = [cvxpy.hstack(args)]
                 for cons_i in cons:
                     joint_cons += cons_i
                 cons = [joint_cons]
 
             # Solve each component separately
@@ -387,15 +387,15 @@
             -\log\mathcal{L}(\rho)
                 &= |W(Ax -y) \|_2^2 \\
                 &= \sum_i \frac{1}{\sigma_i^2}(\mbox{Tr}[E_j\rho] - \hat{p}_i)^2
 
     Additional Details
         The Gaussian weights are estimated from the observed frequency and shot data
         via a Bayesian update of a Dirichlet distribution with observed outcome data
-        frequences :math:`f_i(s)`, and Dirichlet prior :math:`\alpha_i(s)` for
+        frequencies :math:`f_i(s)`, and Dirichlet prior :math:`\alpha_i(s)` for
         tomography basis index `i` and measurement outcome `s`.
 
         The mean posterior probabilities are computed as
 
         .. math:
             p_i(s) &= \frac{f_i(s) + \alpha_i(s)}{\bar{\alpha}_i + N_i} \\
             Var[p_i(s)] &= \frac{p_i(s)(1-p_i(s))}{\bar{\alpha}_i + N_i + 1}
@@ -403,36 +403,36 @@
 
         where :math:`N_i = \sum_s f_i(s)` is the total number of shots, and
         :math:`\bar{\alpha}_i = \sum_s \alpha_i(s)` is the norm of the prior.
 
     Args:
         outcome_data: measurement outcome frequency data.
         shot_data: basis measurement total shot data.
-        measurement_data: measurement basis indice data.
-        preparation_data: preparation basis indice data.
+        measurement_data: measurement basis index data.
+        preparation_data: preparation basis index data.
         measurement_basis: Optional, measurement matrix basis.
         preparation_basis: Optional, preparation matrix basis.
         measurement_qubits: Optional, the physical qubits that were measured.
             If None they are assumed to be ``[0, ..., M-1]`` for M measured qubits.
         preparation_qubits: Optional, the physical qubits that were prepared.
-            If None they are assumed to be ``[0, ..., N-1]`` for N preparated qubits.
+            If None they are assumed to be ``[0, ..., N-1]`` for N prepared qubits.
         conditional_measurement_indices: Optional, conditional measurement data
             indices. If set this will return a list of conditional fitted states
             conditioned on a fixed basis measurement of these qubits.
         trace: trace constraint for the fitted matrix. If "auto" this will be set
                to 1 for QST or the input dimension for QST (default: "auto").
         psd: If True rescale the eigenvalues of fitted matrix to be positive
              semidefinite (default: True)
         trace_preserving: Enforce the fitted matrix to be trace preserving when
                           fitting a Choi-matrix in quantum process
                           tomography. If "auto" this will be set to True for
                           QPT and False for QST (default: "auto").
         partial_trace: Enforce conditional fitted Choi matrices to partial
                        trace to POVM matrices.
-        outcome_prior: The Baysian prior :math:`\alpha` to use computing Gaussian
+        outcome_prior: The Bayesian prior :math:`\alpha` to use computing Gaussian
             weights. See additional information.
         max_weight: Set the maximum value allowed for weights vector computed from
             tomography data variance.
         kwargs: kwargs for cvxpy solver.
 
     Raises:
         QiskitError: If CVXPY is not installed on the current system.
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/cvxpy_utils.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/fitters/cvxpy_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,41 +60,44 @@
                 "You can install it with 'pip install cvxpy'."
             )
         return func(*args, **kwargs)
 
     return decorated_func
 
 
-def solve_iteratively(problem: Problem, initial_iters: int, scale: int = 2, **solve_kwargs) -> None:
+def solve_iteratively(
+    problem: Problem, initial_iters: int, scale: int = 2, solver: str = "SCS", **solve_kwargs
+) -> None:
     """Solve a CVXPY problem increasing iterations if solution is inaccurate.
 
     If the problem is not solved with the ``initial_iters`` value of
     iterations the number of iterations will be doubled up to the
     specified ``"max_iters"`` value in the solve_kwargs. If no max
     iters is specified this will be set to 4 times the initial iters
     values.
 
     Args:
         problem: A CVXPY Problem to solve
         initial_iters: The initial number of max iterations to use
                        when solving the problem
         scale: Scale factor for increasing the initial_iters up to
                max_iters at each step (Default: 2).
+        solver: The solver to use. Defaults to the Splitting Conic Solver.
         solve_kwargs: kwargs for problem.solve method.
 
     Raises:
         AnalysisError: If the CVXPY solve fails to return an optimal or
                        optimal_inaccurate solution.
     """
     current_max_iters = initial_iters
     final_max_iters = solve_kwargs.get("max_iters", 2 * scale * initial_iters)
     problem_solved = False
     while not problem_solved:
         solve_kwargs["max_iters"] = current_max_iters
-        problem.solve(**solve_kwargs)
+        problem.solve(solver=solver, **solve_kwargs)
         if problem.status in ["optimal_inaccurate", "optimal"]:
             problem_solved = True
         elif problem.status == "unbounded_inaccurate":
             if scale > 1 and current_max_iters < final_max_iters:
                 current_max_iters = int(scale * current_max_iters)
             else:
                 raise AnalysisError(
@@ -191,15 +194,15 @@
     else:
         raise TypeError("Input must be a cvxpy variable or list of variables")
     cons = [cvxpy.trace(arg_r) == np.real(trace)]
 
     if hermitian:
         return cons
 
-    # If not hermitian add imaginary trace constrant
+    # If not hermitian add imaginary trace constraint
     if isinstance(mat_i, (list, tuple)):
         arg_i = cvxpy.sum(mat_i)
     elif isinstance(mat_i, Variable):
         arg_i = mat_i
     else:
         raise TypeError("Input must be a cvxpy variable or list of variables")
     cons.append(cvxpy.trace(arg_i) == np.imag(trace))
@@ -272,15 +275,15 @@
 
     ptr = partial_trace_super(input_dim, output_dim)
     cons = [ptr @ cvxpy.vec(arg_r) == np.identity(input_dim).ravel()]
 
     if hermitian:
         return cons
 
-    # If not hermitian add imaginary partial trace constrant
+    # If not hermitian add imaginary partial trace constraint
     if isinstance(mat_i, (tuple, list)):
         arg_r = cvxpy.sum(mat_i)
     elif isinstance(mat_i, Variable):
         arg_i = mat_i
     else:
         raise TypeError("Input must be a cvxpy variable or list of variables")
     cons.append(ptr @ cvxpy.vec(arg_i) == np.zeros(input_dim**2))
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/fitter_data.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/fitters/fitter_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 
 
 def _basis_dimensions(
     basis: Optional[Union[MeasurementBasis, PreparationBasis]] = None,
     qubits: Optional[Sequence[int]] = None,
     conditional_indices: Optional[Sequence[int]] = None,
 ) -> Tuple[int, ...]:
-    """Caculate input and output dimensions for basis and qubits"""
+    """Calculate input and output dimensions for basis and qubits"""
     if not qubits:
         return (1,)
 
     # Get dimension of the preparation and measurement qubits subsystems
     if conditional_indices is None:
         full_qubits = qubits
     else:
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/lininv.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/fitters/lininv.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,16 +89,16 @@
         or :func:`~qiskit_experiments.library.tomography.fitters.cvxpy_linear_lstsq`
         function can be used to solve the same objective function via
         least-squares optimization.
 
     Args:
         outcome_data: basis outcome frequency data.
         shot_data: basis outcome total shot data.
-        measurement_data: measurement basis indice data.
-        preparation_data: preparation basis indice data.
+        measurement_data: measurement basis index data.
+        preparation_data: preparation basis index data.
         measurement_basis: the tomography measurement basis.
         preparation_basis: the tomography preparation basis.
         measurement_qubits: Optional, the physical qubits that were measured.
              If None they are assumed to be [0, ..., M-1] for M measured qubits.
         preparation_qubits: Optional, the physical qubits that were prepared.
             If None they are assumed to be [0, ..., N-1] forN prepared qubits.
         conditional_measurement_indices: Optional, conditional measurement data
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/lstsq_utils.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/fitters/lstsq_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 Common utility functions for tomography fitters.
 """
 
 from typing import Optional, Tuple, Callable, Sequence, Union
 import functools
 import numpy as np
-from qiskit.utils import deprecate_arguments
+from qiskit.utils.deprecation import deprecate_arg
 from qiskit_experiments.exceptions import AnalysisError
 from qiskit_experiments.library.tomography.basis import (
     MeasurementBasis,
     PreparationBasis,
 )
 
 
@@ -185,25 +185,30 @@
 
                 # Increase counter
                 cond_idxs[outcome_cond] += 1
 
     return basis_mat, probs, prob_weights
 
 
-@deprecate_arguments({"beta": "outcome_prior"})
+@deprecate_arg(
+    "beta",
+    new_alias="outcome_prior",
+    since="0.5",
+    package_name="qiskit-experiments",
+)
 def binomial_weights(
     outcome_data: np.ndarray,
     shot_data: Optional[Union[np.ndarray, int]] = None,
     outcome_prior: Union[np.ndarray, int] = 0.5,
     max_weight: float = 1e10,
 ) -> np.ndarray:
     r"""Compute weights from tomography data variance.
 
     This is computed via a Bayesian update of a Dirichlet distribution
-    with observed outcome data frequences :math:`f_i(s)`, and Dirichlet
+    with observed outcome data frequencies :math:`f_i(s)`, and Dirichlet
     prior :math:`\alpha_i(s)` for tomography basis index `i` and
     measurement outcome `s`.
 
     The mean posterior probabilities are computed as
 
     .. math:
         p_i(s) &= \frac{f_i(s) + \alpha_i(s)}{\bar{\alpha}_i + N_i} \\
@@ -227,30 +232,30 @@
     """
     # Compute variance
     _, variance = dirichlet_mean_and_var(
         outcome_data,
         shot_data=shot_data,
         outcome_prior=outcome_prior,
     )
-    # Use max weights to determin a min variance value and clip variance
+    # Use max weights to determine a min variance value and clip variance
     min_variance = 1 / (max_weight**2)
     variance = np.clip(variance, min_variance, None)
     weights = 1.0 / np.sqrt(variance)
     return weights
 
 
 def dirichlet_mean_and_var(
     outcome_data: np.ndarray,
     shot_data: Optional[Union[np.ndarray, int]] = None,
     outcome_prior: Union[np.ndarray, int] = 0.5,
 ) -> Tuple[np.ndarray, np.ndarray]:
     r"""Compute mean probabilities and variance from outcome data.
 
     This is computed via a Bayesian update of a Dirichlet distribution
-    with observed outcome data frequences :math:`f_i(s)`, and Dirichlet
+    with observed outcome data frequencies :math:`f_i(s)`, and Dirichlet
     prior :math:`\alpha_i(s)` for tomography basis index `i` and
     measurement outcome `s`.
 
     The mean posterior probabilities are computed as
 
     .. math:
         p_i(s) &= \frac{f_i(s) + \alpha_i(s)}{\bar{\alpha}_i + N_i} \\
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/postprocess_fit.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/fitters/postprocess_fit.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/fitters/scipy_lstsq.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/driven_freq_tuning/p1_spect.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,280 +1,269 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2021.
+# (C) Copyright IBM 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
-"""
-Linear least-square MLE tomography fitter.
-"""
+"""P1 experiment at various qubit frequencies."""
+
+from __future__ import annotations
+
+from collections.abc import Sequence
 
-from typing import Optional, Dict, Tuple, Union
-import time
 import numpy as np
-import scipy.linalg as la
-from qiskit.utils import deprecate_function
-from qiskit_experiments.exceptions import AnalysisError
-from qiskit_experiments.library.tomography.basis import (
-    MeasurementBasis,
-    PreparationBasis,
+from qiskit import pulse
+from qiskit.circuit import QuantumCircuit, Gate, Parameter, ParameterExpression
+from qiskit.providers.backend import Backend
+from qiskit.utils import optionals as _optional
+
+from qiskit_experiments.framework import BackendTiming, BaseExperiment, Options
+from .p1_spect_analysis import StarkP1SpectAnalysis
+
+from .coefficients import (
+    StarkCoefficients,
+    retrieve_coefficients_from_backend,
 )
-from . import lstsq_utils
-from .fitter_data import _basis_dimensions
 
-# Note this warning doesnt show up when run in analysis so we
-# also add a warning when setting the option value that calls this function
+if _optional.HAS_SYMENGINE:
+    import symengine as sym
+else:
+    import sympy as sym
 
-# pylint: disable = bad-docstring-quotes
-@deprecate_function(
-    "The scipy lstsq tomography fitters are deprecated as of 0.4 and will "
-    "be removed after the 0.5 release. Use the `linear_lstsq`, "
-    "`cvxpy_linear_lstsq`, or `cvxpy_gaussian_lstsq` fitters instead."
-)
-def scipy_linear_lstsq(
-    outcome_data: np.ndarray,
-    shot_data: np.ndarray,
-    measurement_data: np.ndarray,
-    preparation_data: np.ndarray,
-    measurement_basis: Optional[MeasurementBasis] = None,
-    preparation_basis: Optional[PreparationBasis] = None,
-    measurement_qubits: Optional[Tuple[int, ...]] = None,
-    preparation_qubits: Optional[Tuple[int, ...]] = None,
-    weights: Optional[np.ndarray] = None,
-    **kwargs,
-) -> Tuple[np.ndarray, Dict]:
-    r"""Weighted linear least-squares tomography fitter.
-
-    Overview
-        This fitter reconstructs the maximum-likelihood estimate by using
-        :func:`scipy.linalg.lstsq` to minimize the least-squares negative log
-        likelihood function
-
-        .. math::
-            \hat{\rho}
-                &= -\mbox{argmin }\log\mathcal{L}{\rho} \\
-                &= \mbox{argmin }\sum_i w_i^2(\mbox{Tr}[E_j\rho] - \hat{p}_i)^2 \\
-                &= \mbox{argmin }\|W(Ax - y) \|_2^2
-
-        where
-
-        - :math:`A = \sum_j |j \rangle\!\langle\!\langle E_j|` is the matrix of measured
-          basis elements.
-        - :math:`W = \sum_j w_j|j\rangle\!\langle j|` is an optional diagonal weights
-          matrix if an optional weights vector is supplied.
-        - :math:`y = \sum_j \hat{p}_j |j\langle` is the vector of estimated measurement
-          outcome probabilites for each basis element.
-        - :math:`x = |\rho\rangle\!\rangle` is the vectorized density matrix.
-
-    .. note::
-
-        Linear least-squares constructs the full basis matrix :math:`A` as a dense
-        numpy array so should not be used for than 5 or 6 qubits. For larger number
-        of qubits try the
-        :func:`~qiskit_experiments.library.tomography.fitters.linear_inversion`
-        fitter function.
-
-    Args:
-        outcome_data: measurement outcome frequency data.
-        shot_data: basis measurement total shot data.
-        measurement_data: measurement basis indice data.
-        preparation_data: preparation basis indice data.
-        measurement_basis: Optional, measurement matrix basis.
-        preparation_basis: Optional, preparation matrix basis.
-        measurement_qubits: Optional, the physical qubits that were measured.
-            If None they are assumed to be ``[0, ..., M-1]`` for M measured qubits.
-        preparation_qubits: Optional, the physical qubits that were prepared.
-            If None they are assumed to be ``[0, ..., N-1]`` for N preparated qubits.
-        weights: Optional array of weights for least squares objective.
-        kwargs: additional kwargs for :func:`scipy.linalg.lstsq`.
 
-    Raises:
-        AnalysisError: If the fitted vector is not a square matrix
+class StarkP1Spectroscopy(BaseExperiment):
+    """P1 spectroscopy experiment with Stark tone.
+
+    # section: overview
+
+        This experiment measures a probability of the excitation state of the qubit
+        with a certain delay after excitation.
+        A Stark tone is applied during this delay to move the
+        qubit frequency to conduct a spectroscopy of qubit relaxation quantity.
+
+        .. parsed-literal::
+
+                 ┌───┐┌──────────────────┐┌─┐
+              q: ┤ X ├┤ Stark(stark_amp) ├┤M├
+                 └───┘└──────────────────┘└╥┘
+            c: 1/══════════════════════════╩═
+                                           0
+
+        Since the qubit relaxation rate may depend on the qubit frequency due to the
+        coupling to nearby energy levels, this experiment is useful to find out
+        lossy operation frequency that might be harmful to the gate fidelity [1].
+
+    # section: analysis_ref
+        :class:`qiskit_experiments.library.driven_freq_tuning.StarkP1SpectAnalysis`
+
+    # section: reference
+        .. ref_arxiv:: 1 2105.15201
+
+    # section: see_also
+        :class:`qiskit_experiments.library.driven_freq_tuning.ramsey.StarkRamseyXY`
+        :class:`qiskit_experiments.library.driven_freq_tuning.ramsey_amp_scan.StarkRamseyXYAmpScan`
+
+    # section: manual
+        :doc:`/manuals/characterization/stark_experiment`
 
-    Returns:
-        The fitted matrix rho that maximizes the least-squares likelihood function.
     """
-    t_start = time.time()
 
-    if kwargs.pop("conditional_measurement_indices", None):
-        raise AnalysisError(
-            "scipy_linear_lstsq fitter does not support conditional_measurement_indices."
+    def __init__(
+        self,
+        physical_qubits: Sequence[int],
+        backend: Backend | None = None,
+        **experiment_options,
+    ):
+        """
+        Initialize new experiment class.
+
+        Args:
+            physical_qubits: Sequence with the index of the physical qubit.
+            backend: Optional, the backend to run the experiment on.
+            experiment_options: Experiment options. See the class documentation or
+                ``self._default_experiment_options`` for descriptions.
+        """
+        self._timing = None
+
+        super().__init__(
+            physical_qubits=physical_qubits,
+            analysis=StarkP1SpectAnalysis(),
+            backend=backend,
         )
-    if kwargs.pop("conditional_preparation_indices", None):
-        raise AnalysisError(
-            "scipy_linear_lstsq fitter does not support conditional_preparation_indices."
+        self.set_experiment_options(**experiment_options)
+
+    @classmethod
+    def _default_experiment_options(cls) -> Options:
+        """Default experiment options.
+
+        Experiment Options:
+            t1_delay (float): The T1 delay time after excitation pulse. The delay must be
+                sufficiently greater than the edge duration determined by the stark_sigma.
+            stark_channel (PulseChannel): Pulse channel to apply Stark tones.
+                If not provided, the same channel with the qubit drive is used.
+            stark_freq_offset (float): Offset of Stark tone frequency from the qubit frequency.
+                This must be greater than zero not to apply Rabi drive.
+            stark_sigma (float): Gaussian sigma of the rising and falling edges
+                of the Stark tone, in seconds.
+            stark_risefall (float): Ratio of sigma to the duration of
+                the rising and falling edges of the Stark tone.
+            min_xval (float): Minimum x value.
+            max_xval (float): Maximum x value.
+            num_xvals (int): Number of x-values to scan.
+            xval_type (str): Type of x-value. Either ``amplitude`` or ``frequency``.
+                Setting to frequency requires pre-calibration of Stark shift coefficients.
+            spacing (str): A policy for the spacing to create an amplitude list from
+                ``min_stark_amp`` to ``max_stark_amp``. Either ``linear`` or ``quadratic``
+                must be specified.
+            xvals (list[float]): The list of x-values that will be scanned in the experiment.
+                If not set, then ``num_xvals`` parameters spaced according to
+                the ``spacing`` policy between ``min_xval`` and ``max_xval`` are used.
+                If ``xvals`` is set, these parameters are ignored.
+            stark_coefficients (StarkCoefficients): Calibrated Stark shift coefficients.
+                This value is necessary when xval_type is "frequency".
+                When this value is None, a search for the "stark_coefficients" in the
+                result database is run. This requires having the experiment service
+                available in the backend set for the experiment.
+        """
+        options = super()._default_experiment_options()
+        options.update_options(
+            t1_delay=20e-6,
+            stark_channel=None,
+            stark_freq_offset=80e6,
+            stark_sigma=15e-9,
+            stark_risefall=2,
+            min_xval=-1.0,
+            max_xval=1.0,
+            num_xvals=201,
+            xval_type="amplitude",
+            spacing="quadratic",
+            xvals=None,
+            stark_coefficients=None,
         )
-    if measurement_basis and measurement_qubits is None:
-        measurement_qubits = tuple(range(measurement_data.shape[1]))
-    if preparation_basis and preparation_qubits is None:
-        preparation_qubits = tuple(range(preparation_data.shape[1]))
-
-    input_dims = _basis_dimensions(
-        basis=preparation_basis,
-        qubits=preparation_qubits,
-    )
-    output_dims = _basis_dimensions(
-        basis=measurement_basis,
-        qubits=measurement_qubits,
-    )
-
-    metadata = {
-        "fitter": "scipy_linear_lstsq",
-        "input_dims": input_dims,
-        "output_dims": output_dims,
-    }
-
-    basis_matrix, probability_data, probability_weights = lstsq_utils.lstsq_data(
-        outcome_data,
-        shot_data,
-        measurement_data,
-        preparation_data,
-        measurement_basis=measurement_basis,
-        preparation_basis=preparation_basis,
-        measurement_qubits=measurement_qubits,
-        preparation_qubits=preparation_qubits,
-        weights=weights,
-    )
-
-    # Perform least squares fit using Scipy.linalg lstsq function
-    lstsq_options = {"check_finite": False, "lapack_driver": "gelsy"}
-    for key, val in kwargs.items():
-        lstsq_options[key] = val
-
-    # Solve each conditional component independently
-    num_circ_components = probability_data.shape[0]
-
-    if probability_weights is not None:
-        probability_data = probability_weights * probability_data
-
-    fits = []
-    if num_circ_components > 1:
-        metadata["conditional_circuit_outcome"] = []
-    for i in range(num_circ_components):
-        if probability_weights is not None:
-            wt_basis_matrix = probability_weights[i, 0][:, None] * basis_matrix
+        options.set_validator("spacing", ["linear", "quadratic"])
+        options.set_validator("xval_type", ["amplitude", "frequency"])
+        options.set_validator("stark_freq_offset", (0, np.inf))
+        options.set_validator("stark_channel", pulse.channels.PulseChannel)
+        options.set_validator("stark_coefficients", StarkCoefficients)
+        return options
+
+    def _set_backend(self, backend: Backend):
+        super()._set_backend(backend)
+        self._timing = BackendTiming(backend)
+
+    def parameters(self) -> np.ndarray:
+        """Stark tone amplitudes to use in circuits.
+
+        Returns:
+            The list of amplitudes to use for the different circuits based on the
+            experiment options.
+
+        Raises:
+            ValueError: When invalid xval spacing is specified.
+        """
+        opt = self.experiment_options  # alias
+
+        if opt.xvals is None:
+            if opt.spacing == "linear":
+                params = np.linspace(opt.min_xval, opt.max_xval, opt.num_xvals)
+            elif opt.spacing == "quadratic":
+                min_sqrt = np.sign(opt.min_xval) * np.sqrt(np.abs(opt.min_xval))
+                max_sqrt = np.sign(opt.max_xval) * np.sqrt(np.abs(opt.max_xval))
+                lin_params = np.linspace(min_sqrt, max_sqrt, opt.num_xvals)
+                params = np.sign(lin_params) * lin_params**2
+            else:
+                raise ValueError(f"Spacing option {opt.spacing} is not valid.")
         else:
-            wt_basis_matrix = basis_matrix
-
-        sol, _, _, _ = la.lstsq(wt_basis_matrix, probability_data[i, 0], **lstsq_options)
+            params = np.asarray(opt.xvals, dtype=float)
 
-        # Reshape fit to a density matrix
-        size = len(sol)
-        dim = int(np.sqrt(size))
-        if dim * dim != size:
-            raise AnalysisError("Least-squares fitter: invalid result shape.")
-        fit = np.reshape(sol, (dim, dim), order="F")
-        fits.append(fit)
-        if num_circ_components > 1:
-            metadata["conditional_circuit_outcome"].append(i)
-
-    t_stop = time.time()
-    metadata["fitter_time"] = t_stop - t_start
-
-    if len(fits) == 1:
-        return fits[0], metadata
-    return fits, metadata
-
-
-def scipy_gaussian_lstsq(
-    outcome_data: np.ndarray,
-    shot_data: np.ndarray,
-    measurement_data: np.ndarray,
-    preparation_data: np.ndarray,
-    measurement_basis: Optional[MeasurementBasis] = None,
-    preparation_basis: Optional[PreparationBasis] = None,
-    measurement_qubits: Optional[Tuple[int, ...]] = None,
-    preparation_qubits: Optional[Tuple[int, ...]] = None,
-    outcome_prior: Union[np.ndarray, int] = 0.5,
-    max_weight: float = 1e10,
-    **kwargs,
-) -> Dict:
-    r"""Gaussian linear least-squares tomography fitter.
-
-    .. note::
-
-        This function calls :func:`scipy_linear_lstsq` with a Gaussian weights
-        vector. Refer to its documentation for additional details.
-
-    Overview
-        This fitter uses the :func:`scipy_linear_lstsq` fitter to reconstructs
-        the maximum-likelihood estimate of the Gaussian weighted least-squares
-        log-likelihood function
-
-        .. math::
-            \hat{rho} &= \mbox{argmin} -\log\mathcal{L}{\rho} \\
-            -\log\mathcal{L}(\rho)
-                &= \sum_i \frac{1}{\sigma_i^2}(\mbox{Tr}[E_j\rho] - \hat{p}_i)^2
-                = \|W(Ax -y) \|_2^2
-
-    Additional Details
-        The Gaussian weights are estimated from the observed frequency and shot data
-        via a Bayesian update of a Dirichlet distribution with observed outcome data
-        frequences :math:`f_i(s)`, and Dirichlet prior :math:`\alpha_i(s)` for
-        tomography basis index `i` and measurement outcome `s`.
-
-        The mean posterior probabilities are computed as
-
-        .. math:
-            p_i(s) &= \frac{f_i(s) + \alpha_i(s)}{\bar{\alpha}_i + N_i} \\
-            Var[p_i(s)] &= \frac{p_i(s)(1-p_i(s))}{\bar{\alpha}_i + N_i + 1}
-            w_i(s) = \sqrt{Var[p_i(s)]}^{-1}
-
-        where :math:`N_i = \sum_s f_i(s)` is the total number of shots, and
-        :math:`\bar{\alpha}_i = \sum_s \alpha_i(s)` is the norm of the prior.
-
-    Args:
-        outcome_data: measurement outcome frequency data.
-        shot_data: basis measurement total shot data.
-        measurement_data: measurement basis indice data.
-        preparation_data: preparation basis indice data.
-        measurement_basis: Optional, measurement matrix basis.
-        preparation_basis: Optional, preparation matrix basis.
-        measurement_qubits: Optional, the physical qubits that were measured.
-            If None they are assumed to be ``[0, ..., M-1]`` for M measured qubits.
-        preparation_qubits: Optional, the physical qubits that were prepared.
-            If None they are assumed to be ``[0, ..., N-1]`` for N preparated qubits.
-        outcome_prior: The Baysian prior :math:`\alpha` to use computing Gaussian
-            weights. See additional information.
-        max_weight: Set the maximum value allowed for weights vector computed from
-            tomography data variance.
-        kwargs: additional kwargs for :func:`scipy.linalg.lstsq`.
+        if opt.xval_type == "frequency":
+            coeffs = opt.stark_coefficients
+            if coeffs is None:
+                coeffs = retrieve_coefficients_from_backend(
+                    backend=self.backend,
+                    qubit=self.physical_qubits[0],
+                )
+            return coeffs.convert_freq_to_amp(freqs=params)
+        return params
+
+    def parameterized_circuits(self) -> tuple[QuantumCircuit, ...]:
+        """Create circuits with parameters for P1 experiment with Stark shift.
+
+        Returns:
+            Quantum template circuit for P1 experiment.
+        """
+        opt = self.experiment_options  # alias
+        param = Parameter("stark_amp")
+        sym_param = param._symbol_expr
+
+        # Pulse gates
+        stark = Gate("Stark", 1, [param])
+
+        # Note that Stark tone yields negative (positive) frequency shift
+        # when the Stark tone frequency is higher (lower) than qubit f01 frequency.
+        # This choice gives positive frequency shift with positive Stark amplitude.
+        qubit_f01 = self._backend_data.drive_freqs[self.physical_qubits[0]]
+        neg_sign_of_amp = ParameterExpression(
+            symbol_map={param: sym_param},
+            expr=-sym.sign(sym_param),
+        )
+        abs_of_amp = ParameterExpression(
+            symbol_map={param: sym_param},
+            expr=sym.Abs(sym_param),
+        )
+        stark_freq = qubit_f01 + neg_sign_of_amp * opt.stark_freq_offset
+        stark_channel = opt.stark_channel or pulse.DriveChannel(self.physical_qubits[0])
+        sigma_dt = opt.stark_sigma / self._backend_data.dt
+        delay_dt = self._timing.round_pulse(time=opt.t1_delay)
+
+        with pulse.build() as stark_schedule:
+            pulse.set_frequency(stark_freq, stark_channel)
+            pulse.play(
+                pulse.GaussianSquare(
+                    duration=delay_dt,
+                    amp=abs_of_amp,
+                    sigma=sigma_dt,
+                    risefall_sigma_ratio=opt.stark_risefall,
+                ),
+                stark_channel,
+            )
+
+        temp_t1 = QuantumCircuit(1, 1)
+        temp_t1.x(0)
+        temp_t1.append(stark, [0])
+        temp_t1.measure(0, 0)
+        temp_t1.add_calibration(
+            gate=stark,
+            qubits=self.physical_qubits,
+            schedule=stark_schedule,
+        )
 
-    Raises:
-        AnalysisError: If the fitted vector is not a square matrix
+        return (temp_t1,)
 
-    Returns:
-        The fitted matrix rho that maximizes the least-squares likelihood function.
-    """
-    t_start = time.time()
+    def circuits(self) -> list[QuantumCircuit]:
+        """Create circuits.
 
-    weights = lstsq_utils.binomial_weights(
-        outcome_data,
-        shot_data=shot_data,
-        outcome_prior=outcome_prior,
-        max_weight=max_weight,
-    )
-
-    fits, metadata = scipy_linear_lstsq(
-        outcome_data,
-        shot_data,
-        measurement_data,
-        preparation_data,
-        measurement_basis=measurement_basis,
-        preparation_basis=preparation_basis,
-        measurement_qubits=measurement_qubits,
-        preparation_qubits=preparation_qubits,
-        weights=weights,
-        **kwargs,
-    )
-    t_stop = time.time()
-
-    # Update metadata
-    metadata["fitter"] = "scipy_gaussian_lstsq"
-    metadata["fitter_time"] = t_stop - t_start
+        Returns:
+            A list of P1 circuits with a variable Stark tone amplitudes.
+        """
+        (t1_circ,) = self.parameterized_circuits()
+        param = next(iter(t1_circ.parameters))
+
+        circs = []
+        for amp in self.parameters():
+            t1_assigned = t1_circ.assign_parameters({param: amp}, inplace=False)
+            t1_assigned.metadata = {"xval": amp}
+            circs.append(t1_assigned)
+
+        return circs
+
+    def _metadata(self) -> dict[str, any]:
+        """Return experiment metadata for ExperimentData."""
+        metadata = super()._metadata()
+        metadata["stark_freq_offset"] = self.experiment_options.stark_freq_offset
 
-    return fits, metadata
+        return metadata
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/mit_qpt_experiment.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/mit_qpt_experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,22 +74,22 @@
             measurement_indices: Optional, the `physical_qubits` indices to be measured.
                 If None all circuit physical qubits will be measured.
             preparation_indices: Optional, the `physical_qubits` indices to be prepared.
                 If None all circuit physical qubits will be prepared.
             basis_indices: Optional, a list of basis indices for generating partial
                 tomography measurement data. Each item should be given as a pair of
                 lists of preparation and measurement basis configurations
-                ``([p[0], p[1], ..], m[0], m[1], ...])``, where ``p[i]`` is the
+                ``([p[0], p[1], ...], [m[0], m[1], ...])``, where ``p[i]`` is the
                 preparation basis index, and ``m[i]`` is the measurement basis index
                 for qubit-i. If not specified full tomography for all indices of the
                 preparation and measurement bases will be performed.
             conditional_circuit_clbits: Optional, the clbits in the source circuit to
                 be conditioned on when reconstructing the state. If True all circuit
                 clbits will be conditioned on. Enabling this will return a list of
-                reconstrated state components conditional on the values of these clbit
+                reconstructed state components conditional on the values of these clbit
                 values.
             analysis: Optional, a custom tomography analysis instance to use.
                 If ``"default"`` :class:`~.ProcessTomographyAnalysis` will be
                 used. If None no analysis instance will be set.
         """
         tomo_exp = ProcessTomography(
             circuit,
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/mit_qst_experiment.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/mit_qst_experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                 tomography measurement data. Each item should be given as a list of
                 measurement basis configurations ``[m[0], m[1], ...]`` where ``m[i]``
                 is the measurement basis index for qubit-i. If not specified full
                 tomography for all indices of the measurement basis will be performed.
             conditional_circuit_clbits: Optional, the clbits in the source circuit to
                 be conditioned on when reconstructing the state. If True all circuit
                 clbits will be conditioned on. Enabling this will return a list of
-                reconstrated state components conditional on the values of these clbit
+                reconstructed state components conditional on the values of these clbit
                 values.
             analysis: Optional, a custom tomography analysis instance to use.
                 If ``"default"`` :class:`~.ProcessTomographyAnalysis` will be
                 used. If None no analysis instance will be set.
         """
         tomo_exp = StateTomography(
             circuit,
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/mit_tomography_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/mit_tomography_analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,33 +95,35 @@
         roerror_analysis, tomo_analysis = self._analyses
         roerror_data, tomo_data = self._component_experiment_data(experiment_data)
 
         # Run readout error analysis
         roerror_analysis.run(roerror_data, replace_results=True).block_for_results()
 
         # Construct noisy measurement basis
-        mitigator = roerror_data.analysis_results(0).value
+        mitigator = roerror_data.analysis_results("Local Readout Mitigator").value
 
-        # Construct noisy measurement basis
-        measurement_basis = PauliMeasurementBasis(mitigator=mitigator)
-        tomo_analysis.set_options(measurement_basis=measurement_basis)
-
-        # Run mitigated tomography analysis
-        tomo_analysis.run(tomo_data, replace_results=True).block_for_results()
-        for res in tomo_data.analysis_results(block=False):
-            res.extra["mitigated"] = True
+        # Run mitigated tomography analysis with noisy mitigated basis
+        # Tomo analysis instance is internally copied by setting option with run.
+        tomo_analysis.run(
+            tomo_data,
+            replace_results=True,
+            measurement_basis=PauliMeasurementBasis(mitigator=mitigator),
+            extra={"mitigated": True},
+        ).block_for_results()
 
         # Combine results so that tomography results are ordered first
         combined_data = [tomo_data, roerror_data]
 
         # Run unmitigated tomography analysis
         if self.options.unmitigated_fit:
-            tomo_analysis.set_options(measurement_basis=PauliMeasurementBasis())
-            nomit_data = tomo_analysis.run(tomo_data, replace_results=False).block_for_results()
-            for res in nomit_data.analysis_results(block=False):
-                res.extra["mitigated"] = False
+            nomit_data = tomo_analysis.run(
+                tomo_data,
+                replace_results=False,
+                measurement_basis=PauliMeasurementBasis(),
+                extra={"mitigated": False},
+            ).block_for_results()
             combined_data.append(nomit_data)
 
         if self._flatten_results:
             return self._combine_results(combined_data)
 
         return [], []
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/qpt_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/qpt_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,20 +26,16 @@
 
         Built-in fitter functions may be selected using the following string
         labels, refer to the corresponding functions documentation for additional
         details on the fitters.
 
         * ``"linear_inversion"``:
           :func:`~qiskit_experiments.library.tomography.fitters.linear_inversion` (Default)
-        * ``"scipy_linear_lstsq"``:
-          :func:`~qiskit_experiments.library.tomography.fitters.scipy_linear_lstsq`
         * ``"cvxpy_linear_lstsq"``:
           :func:`~qiskit_experiments.library.tomography.fitters.cvxpy_linear_lstsq`
-        * ``"scipy_gaussian_lstsq"``:
-          :func:`~qiskit_experiments.library.tomography.fitters.scipy_gaussian_lstsq`
         * ``"cvxpy_gaussian_lstsq"``:
           :func:`~qiskit_experiments.library.tomography.fitters.cvxpy_gaussian_lstsq`
 
         PSD Rescaling
 
         For fitters that do not constrain the reconstructed state to be
         `positive-semidefinite` (PSD) we construct the maximum-likelihood
@@ -88,39 +84,40 @@
                 or trace dim for :class:`~qiskit.quantum_info.Choi` matrices (Default: True).
             measurement_qubits (Sequence[int]): Optional, the physical qubits with tomographic
                 measurements. If not specified will be set to ``[0, ..., N-1]`` for N-qubit
                 tomographic measurements.
             preparation_qubits (Sequence[int]): Optional, the physical qubits with tomographic
                 preparations. If not specified will be set to ``[0, ..., N-1]`` for N-qubit
                 tomographic preparations.
-                This can  be a string to select one of the built-in fitters, or a callable to
+            fitter (str or Callable): The fitter function to use for reconstruction.
+                This can be a string to select one of the built-in fitters, or a callable to
                 supply a custom fitter function. See the `Fitter Functions` section for
                 additional information.
             target (str or
                 :class:`~qiskit.quantum_info.operators.channel.quantum_channel.QuantumChannel`
                 or :class:`~qiskit.quantum_info.Operator`): Optional, Set a custom target quantum
                 channel for computing the :func:`~qiskit.quantum_info.process_fidelity` of the
                 fitted process against (Default: None).
             conditional_circuit_clbits (list[int]): Optional, the clbit indices in the
                 source circuit to be conditioned on when reconstructing the channel.
-                Enabling this will return a list of reconstrated channel components
+                Enabling this will return a list of reconstructed channel components
                 conditional on the values of these clbit values. The integer value of the
                 conditioning clbits is stored in state analysis result extra field
                 `"conditional_circuit_outcome"`.
             conditional_measurement_indices (list[int]): Optional, indices of tomography
                 measurement qubits to used for conditional state reconstruction. Enabling
-                this will return a list of reconstrated channel components conditioned on
+                this will return a list of reconstructed channel components conditioned on
                 the remaining tomographic bases conditional on the basis index, and outcome
                 value for these measurements. The conditional measurement basis index and
                 integer value of the measurement outcome is stored in state analysis result
                 extra fields `"conditional_measurement_index"` and
                 `"conditional_measurement_outcome"` respectively.
             conditional_preparation_indices (list[int]): Optional, indices of tomography
                 preparation qubits to used for conditional state reconstruction. Enabling
-                this will return a list of reconstrated channel components conditioned on
+                this will return a list of reconstructed channel components conditioned on
                 the remaining tomographic bases conditional on the basis index. The
                 conditional preparation basis index is stored in state analysis result
                 extra fields `"conditional_preparation_index"`.
         """
         options = super()._default_options()
         options.measurement_basis = PauliMeasurementBasis()
         options.preparation_basis = PauliPreparationBasis()
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/qpt_experiment.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/qpt_experiment.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from typing import Union, Optional, List, Tuple, Sequence
 import numpy as np
 from qiskit.circuit import QuantumCircuit, Instruction, Clbit
 from qiskit.providers.backend import Backend
 from qiskit.quantum_info.operators.base_operator import BaseOperator
 from qiskit.quantum_info import Choi, Operator, Statevector, DensityMatrix, partial_trace
 
-from qiskit_experiments.warnings import deprecate_arguments
 from qiskit_experiments.exceptions import QiskitError
 from .tomography_experiment import TomographyExperiment, TomographyAnalysis, BaseAnalysis
 from .qpt_analysis import ProcessTomographyAnalysis
 from . import basis
 
 
 class ProcessTomography(TomographyExperiment):
@@ -45,22 +44,14 @@
         preparation and measurement bases.
 
     # section: analysis_ref
         :class:`ProcessTomographyAnalysis`
 
     """
 
-    @deprecate_arguments(
-        {
-            "qubits": "physical_qubits",
-            "measurement_qubits": "measurement_indices",
-            "preparation_qubits": "preparation_indices",
-        },
-        "0.5",
-    )
     def __init__(
         self,
         circuit: Union[QuantumCircuit, Instruction, BaseOperator],
         backend: Optional[Backend] = None,
         physical_qubits: Optional[Sequence[int]] = None,
         measurement_basis: basis.MeasurementBasis = basis.PauliMeasurementBasis(),
         measurement_indices: Optional[Sequence[int]] = None,
@@ -86,22 +77,22 @@
             preparation_basis: Tomography basis for measurements. If not specified the
                 default basis is the :class:`~basis.PauliPreparationBasis`.
             preparation_indices: Optional, the `physical_qubits` indices to be prepared.
                 If None all circuit physical qubits will be prepared.
             basis_indices: Optional, a list of basis indices for generating partial
                 tomography measurement data. Each item should be given as a pair of
                 lists of preparation and measurement basis configurations
-                ``([p[0], p[1], ..], m[0], m[1], ...])``, where ``p[i]`` is the
+                ``([p[0], p[1], ...], [m[0], m[1], ...])``, where ``p[i]`` is the
                 preparation basis index, and ``m[i]`` is the measurement basis index
                 for qubit-i. If not specified full tomography for all indices of the
                 preparation and measurement bases will be performed.
             conditional_circuit_clbits: Optional, the clbits in the source circuit to
                 be conditioned on when reconstructing the channel. If True all circuit
                 clbits will be conditioned on. Enabling this will return a list of
-                reconstrated channel components conditional on the values of these clbit
+                reconstructed channel components conditional on the values of these clbit
                 values.
             analysis: Optional, a custom analysis instance to use. If ``"default"``
                 :class:`~.ProcessTomographyAnalysis` will be used. If None no analysis
                 instance will be set.
             target: Optional, a custom quantum state target for computing the
                 state fidelity of the fitted density matrix during analysis.
                 If "default" the state will be inferred from the input circuit
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/qst_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/qst_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,16 @@
 
         Built-in fitter functions may be selected using the following string
         labels, refer to the corresponding functions documentation for additional
         details on the fitters.
 
         * ``"linear_inversion"``:
           :func:`~qiskit_experiments.library.tomography.fitters.linear_inversion` (Default)
-        * ``"scipy_linear_lstsq"``:
-          :func:`~qiskit_experiments.library.tomography.fitters.scipy_linear_lstsq`
         * ``"cvxpy_linear_lstsq"``:
           :func:`~qiskit_experiments.library.tomography.fitters.cvxpy_linear_lstsq`
-        * ``"scipy_gaussian_lstsq"``:
-          :func:`~qiskit_experiments.library.tomography.fitters.scipy_gaussian_lstsq`
         * ``"cvxpy_gaussian_lstsq"``:
           :func:`~qiskit_experiments.library.tomography.fitters.cvxpy_gaussian_lstsq`
 
         PSD Rescaling
 
         For fitters that do not constrain the reconstructed state to be
         `positive-semidefinite` (PSD) we construct the maximum-likelihood
@@ -66,15 +62,15 @@
 
         Analysis Options:
             measurement_basis (:class:`~qiskit_experiments.library.tomography.basis.MeasurementBasis`):
                 The measurement
                 :class:`~qiskit_experiments.library.tomography.basis.MeasurementBasis`
                 to use for tomographic state reconstruction.
             fitter (str or Callable): The fitter function to use for reconstruction.
-                This can  be a string to select one of the built-in fitters, or a callable to
+                This can be a string to select one of the built-in fitters, or a callable to
                 supply a custom fitter function. See the `Fitter Functions` section for
                 additional information.
             fitter_options (dict): Any addition kwarg options to be supplied to the fitter
                 function. For documentation of available kwargs refer to the fitter function
                 documentation.
             rescale_positive (bool): If True rescale the state returned by the fitter
                 to be positive-semidefinite. See the `PSD Rescaling` section for
@@ -88,23 +84,23 @@
             target (str or :class:`~qiskit.quantum_info.DensityMatrix`
                 or :class:`~qiskit.quantum_info.Statevector`): Optional,
                 set a custom target quantum state for computing the
                 :func:`~qiskit.quantum_info.state_fidelity`
                 of the fitted state against (Default: None).
             conditional_circuit_clbits (list[int]): Optional, the clbit indices in the
                 source circuit to be conditioned on when reconstructing the state.
-                Enabling this will return a list of reconstrated state components
+                Enabling this will return a list of reconstructed state components
                 conditional on the values of these clbit values. The integer value of the
                 conditioning clbits is stored in state analysis result extra field
                 `"conditional_circuit_outcome"`.
             conditional_measurement_indices (list[int]): Optional, indices of tomography
                 measurement qubits to used for conditional state reconstruction. Enabling
-                this will return a list of reconstrated state components conditioned on
+                this will return a list of reconstructed state components conditioned on
                 the remaining tomographic bases conditional on the basis index, and outcome
-                value for these measurements. The conditionl measurement basis index and
+                value for these measurements. The conditional measurement basis index and
                 integer value of the measurement outcome is stored in state analysis result
                 extra fields `"conditional_measurement_index"` and
                 `"conditional_measurement_outcome"` respectively.
         """
         options = super()._default_options()
         options.measurement_basis = PauliMeasurementBasis()
         return options
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/qst_experiment.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/qst_experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 from typing import Union, Optional, List, Sequence
 from qiskit.providers.backend import Backend
 from qiskit.circuit import QuantumCircuit, Instruction, Clbit
 from qiskit.quantum_info.operators.base_operator import BaseOperator
 from qiskit.quantum_info import Statevector, DensityMatrix, partial_trace
 
-from qiskit_experiments.warnings import deprecate_arguments
 from qiskit_experiments.exceptions import QiskitError
 from .tomography_experiment import TomographyExperiment, TomographyAnalysis, BaseAnalysis
 from .qst_analysis import StateTomographyAnalysis
 from . import basis
 
 
 class StateTomography(TomographyExperiment):
@@ -41,19 +40,19 @@
         Performing full state tomography on an `N`-qubit state requires
         running :math:`3^N` measurement circuits when using the default
         measurement basis.
 
     # section: analysis_ref
         :class:`StateTomographyAnalysis`
 
+    # section: manual
+        :doc:`/manuals/verification/state_tomography`
+
     """
 
-    @deprecate_arguments(
-        {"qubits": "physical_qubits", "measurement_qubits": "measurement_indices"}, "0.5"
-    )
     def __init__(
         self,
         circuit: Union[QuantumCircuit, Instruction, BaseOperator, Statevector],
         backend: Optional[Backend] = None,
         physical_qubits: Optional[Sequence[int]] = None,
         measurement_basis: basis.MeasurementBasis = basis.PauliMeasurementBasis(),
         measurement_indices: Optional[Sequence[int]] = None,
@@ -78,15 +77,15 @@
                 tomography measurement data. Each item should be given as a list of
                 measurement basis configurations ``[m[0], m[1], ...]`` where ``m[i]``
                 is the measurement basis index for qubit-i. If not specified full
                 tomography for all indices of the measurement basis will be performed.
             conditional_circuit_clbits: Optional, the clbits in the source circuit to
                 be conditioned on when reconstructing the state. If True all circuit
                 clbits will be conditioned on. Enabling this will return a list of
-                reconstrated state components conditional on the values of these clbit
+                reconstructed state components conditional on the values of these clbit
                 values.
             analysis: Optional, a custom analysis instance to use. If ``"default"``
                 :class:`~.StateTomographyAnalysis` will be used. If None no analysis
                 instance will be set.
             target: Optional, a custom quantum state target for computing the
                 state fidelity of the fitted density matrix during analysis.
                 If "default" the state will be inferred from the input circuit
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/tomography_analysis.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/tomography_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,43 +12,38 @@
 """
 Quantum process tomography analysis
 """
 
 
 from typing import List, Union, Callable
 from collections import defaultdict
-import warnings
 import numpy as np
 import scipy.linalg as la
 from uncertainties import ufloat
 
 from qiskit.quantum_info import DensityMatrix, Choi, Operator
 from qiskit.quantum_info.operators.base_operator import BaseOperator
 from qiskit.quantum_info.operators.channel.quantum_channel import QuantumChannel
 
 from qiskit_experiments.exceptions import AnalysisError
-from qiskit_experiments.framework import BaseAnalysis, AnalysisResultData, Options
+from qiskit_experiments.framework import BaseAnalysis, AnalysisResultData, Options, numpy_version
 from .fitters import (
     tomography_fitter_data,
     postprocess_fitter,
     linear_inversion,
-    scipy_linear_lstsq,
-    scipy_gaussian_lstsq,
     cvxpy_linear_lstsq,
     cvxpy_gaussian_lstsq,
 )
 
 
 class TomographyAnalysis(BaseAnalysis):
     """Base analysis for state and process tomography experiments."""
 
     _builtin_fitters = {
         "linear_inversion": linear_inversion,
-        "scipy_linear_lstsq": scipy_linear_lstsq,
-        "scipy_gaussian_lstsq": scipy_gaussian_lstsq,
         "cvxpy_linear_lstsq": cvxpy_linear_lstsq,
         "cvxpy_gaussian_lstsq": cvxpy_gaussian_lstsq,
     }
     _cvxpy_fitters = (
         cvxpy_linear_lstsq,
         cvxpy_gaussian_lstsq,
     )
@@ -98,32 +93,33 @@
                 performed and the target fidelity will not include a standard error
                 (Default: 0).
             target_bootstrap_seed (int | None | Generator): Optional, RNG seed or
                 Generator to use for bootstrapping data for boostrapped fidelity
                 standard error calculation (Default: None).
             conditional_circuit_clbits (list[int]): Optional, the clbit indices in the
                 source circuit to be conditioned on when reconstructing the state.
-                Enabling this will return a list of reconstrated state components
+                Enabling this will return a list of reconstructed state components
                 conditional on the values of these clbit values. The integer value of the
                 conditioning clbits is stored in state analysis result extra field
                 `"conditional_circuit_outcome"`.
             conditional_measurement_indices (list[int]): Optional, indices of tomography
                 measurement qubits to used for conditional state reconstruction. Enabling
-                this will return a list of reconstrated state components conditioned on
+                this will return a list of reconstructed state components conditioned on
                 the remaining tomographic bases conditional on the basis index, and outcome
-                value for these measurements. The conditionl measurement basis index and
+                value for these measurements. The conditional measurement basis index and
                 integer value of the measurement outcome is stored in state analysis result
                 extra fields `"conditional_measurement_index"` and
                 `"conditional_measurement_outcome"` respectively.
             conditional_preparation_indices (list[int]): Optional, indices of tomography
                 preparation qubits to used for conditional state reconstruction. Enabling
-                this will return a list of reconstrated channel components conditioned on
+                this will return a list of reconstructed channel components conditioned on
                 the remaining tomographic bases conditional on the basis index. The
-                conditionl preparation basis index is stored in state analysis result
+                conditional preparation basis index is stored in state analysis result
                 extra fields `"conditional_preparation_index"`.
+            extra (Dict[str, Any]): Extra metadata dictionary attached to analysis results.
         """
         options = super()._default_options()
 
         options.measurement_basis = None
         options.preparation_basis = None
         options.fitter = "linear_inversion"
         options.fitter_options = {}
@@ -133,32 +129,17 @@
         options.preparation_qubits = None
         options.target = None
         options.target_bootstrap_samples = 0
         options.target_bootstrap_seed = None
         options.conditional_circuit_clbits = None
         options.conditional_measurement_indices = None
         options.conditional_preparation_indices = None
+        options.extra = {}
         return options
 
-    def set_options(self, **fields):
-        if fields.get("fitter", None) in [
-            "scipy_linear_lstsq",
-            "scipy_gaussian_lstsq",
-            scipy_linear_lstsq,
-            scipy_gaussian_lstsq,
-        ]:
-            warnings.warn(
-                "The scipy lstsq tomography fitters are deprecated as of 0.4 and will "
-                "be removed after the 0.5 release. Use the `linear_lstsq`, "
-                "`cvxpy_linear_lstsq`, or `cvxpy_gaussian_lstsq` fitter instead.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-        super().set_options(**fields)
-
     @classmethod
     def _get_fitter(cls, fitter: Union[str, Callable]) -> Callable:
         """Return fitter function for named builtin fitters"""
         if fitter is None:
             raise AnalysisError("No tomography fitter given")
         if not isinstance(fitter, str):
             return fitter
@@ -249,14 +230,17 @@
         # Finally format state result metadata to remove eigenvectors
         # which are no longer needed to reduce size
         for state_result in state_results:
             state_result.extra.pop("eigvecs")
 
         analysis_results = state_results + other_results
 
+        if self.options.extra:
+            for res in analysis_results:
+                res.extra.update(self.options.extra)
         return analysis_results, []
 
     def _fit_state_results(
         self,
         fitter: Callable,
         outcome_data: np.ndarray,
         shot_data: np.ndarray,
@@ -322,21 +306,22 @@
         if isinstance(seed, np.random.Generator):
             rng = seed
         else:
             rng = np.random.default_rng(seed)
         prob_data = outcome_data / shot_data[None, :, None]
         bs_fidelities = []
         for _ in range(self.options.target_bootstrap_samples):
-            # Once python 3.7 support is dropped and minimum NumPy
-            # version can be set to 1.22 this can be replaced with
-            # `sampled_data = rng.multinomial(shot_data, probs)`
-            sampled_data = np.zeros_like(outcome_data)
-            for i in range(prob_data.shape[0]):
-                for j in range(prob_data.shape[1]):
-                    sampled_data[i, j] = rng.multinomial(shot_data[j], prob_data[i, j])
+            # TODO: remove conditional once numpy is pinned at 1.22 and above
+            if numpy_version() >= (1, 22):
+                sampled_data = rng.multinomial(shot_data, prob_data)
+            else:
+                sampled_data = np.zeros_like(outcome_data)
+                for i in range(prob_data.shape[0]):
+                    for j in range(prob_data.shape[1]):
+                        sampled_data[i, j] = rng.multinomial(shot_data[j], prob_data[i, j])
 
             try:
                 state_results = self._fit_state_results(
                     fitter,
                     sampled_data,
                     shot_data,
                     measurement_data,
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/library/tomography/tomography_experiment.py` & `qiskit-experiments-0.6.0/qiskit_experiments/library/tomography/tomography_experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from typing import Union, Optional, Iterable, List, Tuple, Sequence
 from itertools import product
 from qiskit.circuit import QuantumCircuit, Instruction, ClassicalRegister, Clbit
 from qiskit.circuit.library import Permutation
 from qiskit.providers.backend import Backend
 from qiskit.quantum_info.operators.base_operator import BaseOperator
 
-from qiskit_experiments.warnings import deprecate_arguments
 from qiskit_experiments.exceptions import QiskitError
 from qiskit_experiments.framework import BaseExperiment, BaseAnalysis, Options
 from .basis import PreparationBasis, MeasurementBasis
 from .tomography_analysis import TomographyAnalysis
 
 
 class TomographyExperiment(BaseExperiment):
@@ -43,22 +42,14 @@
                 If None All basis elements will be measured.
 
         """
         options = super()._default_experiment_options()
         options.basis_indices = None
         return options
 
-    @deprecate_arguments(
-        {
-            "qubits": "physical_qubits",
-            "measurement_qubits": "measurement_indices",
-            "preparation_qubits": "preparation_indices",
-        },
-        "0.5",
-    )
     def __init__(
         self,
         circuit: Union[QuantumCircuit, Instruction, BaseOperator],
         backend: Optional[Backend] = None,
         physical_qubits: Optional[Sequence[int]] = None,
         measurement_basis: Optional[MeasurementBasis] = None,
         measurement_indices: Optional[Sequence[int]] = None,
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/test/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/test/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,16 +33,14 @@
 
     PulseBackend
     SingleTransmonTestBackend
     MockIQBackend
     MockIQParallelBackend
     T2HahnBackend
     NoisyDelayAerBackend
-    PulseBackend
-    SingleTransmonTestBackend
 
 Helpers
 =======
 
 Helper classes for supporting test functionality.
 
 .. autosummary::
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/test/fake_backend.py` & `qiskit-experiments-0.6.0/qiskit_experiments/test/fake_backend.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,30 +9,45 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Fake backend class for tests."""
 import uuid
 from qiskit.circuit.library import Measure
+from qiskit.providers import ProviderV1
 from qiskit.providers.backend import BackendV2
 from qiskit.providers.options import Options
 from qiskit.transpiler import Target
 
 from qiskit.result import Result
 
 from qiskit_experiments.test.utils import FakeJob
 
 
+class FakeProvider(ProviderV1):
+    """Fake provider with no backends for testing"""
+
+    def backends(self, name=None, **kwargs):
+        """List of available backends. Empty in this case"""
+        return []
+
+
 class FakeBackend(BackendV2):
     """
     Fake backend for test purposes only.
     """
 
-    def __init__(self, backend_name="fake_backend", num_qubits=1, max_experiments=100):
-        super().__init__(name=backend_name)
+    def __init__(
+        self,
+        provider=FakeProvider(),
+        backend_name="fake_backend",
+        num_qubits=1,
+        max_experiments=100,
+    ):
+        super().__init__(provider=provider, name=backend_name)
         self._target = Target(num_qubits=num_qubits)
         # Add a measure for each qubit so a simple measure circuit works
         self.target.add_instruction(Measure())
         self._max_circuits = max_experiments
 
     @property
     def max_circuits(self):
@@ -44,16 +59,29 @@
         return Options()
 
     @property
     def target(self) -> Target:
         return self._target
 
     def run(self, run_input, **options):
+        if not isinstance(run_input, list):
+            run_input = [run_input]
+        results = [
+            {
+                "data": {"0": 100},
+                "shots": 100,
+                "success": True,
+                "header": {"metadata": circ.metadata},
+                "meas_level": 2,
+            }
+            for circ in run_input
+        ]
+
         result = {
             "backend_name": "fake_backend",
             "backend_version": "0",
             "qobj_id": uuid.uuid4().hex,
             "job_id": uuid.uuid4().hex,
             "success": True,
-            "results": [],
+            "results": results,
         }
         return FakeJob(backend=self, result=Result.from_dict(result))
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/test/fake_service.py` & `qiskit-experiments-0.6.0/qiskit_experiments/test/fake_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,73 +8,38 @@
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Fake service class for tests."""
 
-from typing import Optional, List, Dict, Type, Any, Union, Tuple, Callable
-import functools
+from typing import Optional, List, Dict, Type, Any, Union, Tuple
 import json
 from datetime import datetime, timedelta
 import uuid
 
-from qiskit_experiments.test.fake_backend import FakeBackend
+import pandas as pd
+from qiskit_ibm_experiment import AnalysisResultData
 
+from qiskit_experiments.test.fake_backend import FakeBackend
 from qiskit_experiments.database_service.device_component import DeviceComponent
 from qiskit_experiments.database_service.exceptions import (
     ExperimentEntryExists,
     ExperimentEntryNotFound,
 )
 
 
-# Check if PANDAS package is installed
-try:
-    import pandas as pd
-
-    HAS_PANDAS = True
-except ImportError:
-    pd = None
-    HAS_PANDAS = False
-
-
-def requires_pandas(func: Callable) -> Callable:
-    """Function decorator for functions requiring Pandas.
-
-    Args:
-        func: a function requiring Pandas.
-
-    Returns:
-        The decorated function.
-
-    Raises:
-        QiskitError: If Pandas is not installed.
-    """
-
-    @functools.wraps(func)
-    def decorated_func(*args, **kwargs):
-        if not HAS_PANDAS:
-            raise ImportError(
-                f"The pandas python package is required for {func}."
-                "You can install it with 'pip install pandas'."
-            )
-        return func(*args, **kwargs)
-
-    return decorated_func
-
-
 class FakeService:
     """
     This extremely simple database is designated for testing and as a playground for developers.
     It does not support multi-threading.
     It is not guaranteed to perform well for a large amount of data.
     It implements most of the methods of `DatabaseService`.
     """
 
-    @requires_pandas
     def __init__(self):
         self.exps = pd.DataFrame(
             columns=[
                 "experiment_type",
                 "backend_name",
                 "metadata",
                 "experiment_id",
@@ -97,15 +62,14 @@
                 "device_components",
                 "tags",
                 "quality",
                 "verified",
                 "result_id",
                 "chisq",
                 "creation_datetime",
-                "service",
                 "backend_name",
             ]
         )
 
     def create_experiment(
         self,
         experiment_type: str,
@@ -143,41 +107,46 @@
         #    experiment, with the first experiment dated to midnight of January 1st, 2022, the
         #    second experiment an hour later, etc.
         # figure_names - the fake service currently does not support figures. The column
         #    (degenerated to []) is required to prevent a flaw in the work with DbExperimentData.
         # backend - the query methods `experiment` and `experiments` are supposed to return an
         #    an instantiated backend object, and not only the backend name. We assume that the fake
         #    service works with the fake backend (class FakeBackend).
-        self.exps = pd.concat(
+        row = pd.DataFrame(
             [
-                self.exps,
-                pd.DataFrame(
-                    [
-                        {
-                            "experiment_type": experiment_type,
-                            "experiment_id": experiment_id,
-                            "parent_id": parent_id,
-                            "backend_name": backend_name,
-                            "metadata": metadata,
-                            "job_ids": job_ids,
-                            "tags": tags,
-                            "notes": notes,
-                            "share_level": kwargs.get("share_level", None),
-                            "device_components": [],
-                            "start_datetime": datetime(2022, 1, 1)
-                            + timedelta(hours=len(self.exps)),
-                            "figure_names": [],
-                            "backend": FakeBackend(backend_name=backend_name),
-                        }
-                    ],
-                    columns=self.exps.columns,
-                ),
+                {
+                    "experiment_type": experiment_type,
+                    "experiment_id": experiment_id,
+                    "parent_id": parent_id,
+                    "backend_name": backend_name,
+                    "metadata": metadata,
+                    "job_ids": job_ids,
+                    "tags": tags,
+                    "notes": notes,
+                    "share_level": kwargs.get("share_level", None),
+                    "device_components": [],
+                    "start_datetime": datetime(2022, 1, 1) + timedelta(hours=len(self.exps)),
+                    "figure_names": [],
+                    "backend": FakeBackend(backend_name=backend_name),
+                }
             ],
-            ignore_index=True,
+            columns=self.exps.columns,
         )
+        if len(self.exps) > 0:
+            self.exps = pd.concat(
+                [
+                    self.exps,
+                    row,
+                ],
+                ignore_index=True,
+            )
+        else:
+            # Avoid the FutureWarning on concatenating empty DataFrames
+            # introduced in https://github.com/pandas-dev/pandas/pull/52532
+            self.exps = row
 
         return experiment_id
 
     def update_experiment(
         self,
         experiment_id: str,
         metadata: Optional[Dict] = None,
@@ -325,43 +294,47 @@
         # Clarifications about some of the columns:
         # backend_name - taken from the experiment.
         # creation_datetime - start_datetime - not a parameter of
         #    `DatabaseService.create_analysis_result` but a parameter of
         #    `IBMExperimentService.create_analysis_result`. Since `DbExperimentData` does not set it
         #    via kwargs (as it does with chisq), the user cannot control the time and the service
         #    alone decides about it. Here we've chosen to set the start date of the experiment.
-        self.results = pd.concat(
+        row = pd.DataFrame(
             [
-                self.results,
-                pd.DataFrame(
-                    [
-                        {
-                            "result_data": result_data,
-                            "result_id": result_id,
-                            "result_type": result_type,
-                            "device_components": device_components,
-                            "experiment_id": experiment_id,
-                            "quality": quality,
-                            "verified": verified,
-                            "tags": tags,
-                            "backend_name": self.exps.loc[self.exps.experiment_id == experiment_id]
-                            .iloc[0]
-                            .backend_name,
-                            "chisq": kwargs.get("chisq", None),
-                            "creation_datetime": self.exps.loc[
-                                self.exps.experiment_id == experiment_id
-                            ]
-                            .iloc[0]
-                            .start_datetime,
-                        }
-                    ]
-                ),
-            ],
-            ignore_index=True,
+                {
+                    "result_data": result_data,
+                    "result_id": result_id,
+                    "result_type": result_type,
+                    "device_components": device_components,
+                    "experiment_id": experiment_id,
+                    "quality": quality,
+                    "verified": verified,
+                    "tags": tags,
+                    "backend_name": self.exps.loc[self.exps.experiment_id == experiment_id]
+                    .iloc[0]
+                    .backend_name,
+                    "chisq": kwargs.get("chisq", None),
+                    "creation_datetime": self.exps.loc[self.exps.experiment_id == experiment_id]
+                    .iloc[0]
+                    .start_datetime,
+                }
+            ]
         )
+        if len(self.results) > 0:
+            self.results = pd.concat(
+                [
+                    self.results,
+                    row,
+                ],
+                ignore_index=True,
+            )
+        else:
+            # Avoid the FutureWarning on concatenating empty DataFrames
+            # introduced in https://github.com/pandas-dev/pandas/pull/52532
+            self.results = row
 
         # a helper method for updating the experiment's device components, see usage below
         def add_new_components(expcomps):
             for dc in device_components:
                 if dc not in expcomps:
                     expcomps.append(dc)
 
@@ -418,15 +391,15 @@
         result_type: Optional[str] = None,
         backend_name: Optional[str] = None,
         quality: Optional[str] = None,
         verified: Optional[bool] = None,
         tags: Optional[List[str]] = None,
         tags_operator: Optional[str] = "OR",
         **filters: Any,
-    ) -> List[Dict]:
+    ) -> List[AnalysisResultData]:
         """Returns a list of analysis results filtered by the given criteria"""
         # pylint: disable = unused-argument
         df = self.results
 
         # TODO: skipping device components for now until we consolidate more with the provider service
         # (in the qiskit-experiments service there is no operator for device components,
         # so the specification for filtering is not clearly defined)
@@ -475,15 +448,15 @@
             )
 
         df = df.sort_values(
             ["creation_datetime", "result_id"], ascending=[(sortby_split[1] == "asc"), True]
         )
 
         df = df.iloc[:limit]
-        return df.to_dict("records")
+        return [AnalysisResultData(**res) for res in df.to_dict("records")]
 
     def delete_analysis_result(self, result_id: str) -> None:
         """Deletes an analysis result"""
         if result_id not in self.results.result_id.values:
             return
 
         index = self.results[self.results.result_id == result_id].index
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/test/mock_iq_backend.py` & `qiskit-experiments-0.6.0/qiskit_experiments/test/mock_iq_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 from typing import Sequence, List, Tuple, Dict, Union, Any
 import numpy as np
 
 from qiskit import QuantumCircuit
 from qiskit.circuit.library import XGate, SXGate
 from qiskit.result import Result
 from qiskit.providers.fake_provider import FakeOpenPulse2Q
-from qiskit.providers.fake_provider.fake_backend import FakeBackendV2
-
 from qiskit.qobj.utils import MeasLevel
+from qiskit_ibm_runtime.fake_provider.fake_backend import FakeBackendV2
+
 from qiskit_experiments.exceptions import QiskitError
 from qiskit_experiments.framework import Options
 from qiskit_experiments.test.utils import FakeJob
 from qiskit_experiments.data_processing.exceptions import DataProcessorError
 from qiskit_experiments.test.mock_iq_helpers import (
     MockIQExperimentHelper,
     MockIQParallelExperimentHelper,
@@ -225,15 +225,16 @@
         rng_seed: int = 0,
     ):
         """
         Initialize the backend.
 
         Args:
             experiment_helper(MockIQExperimentHelper): Experiment helper class that contains
-                'compute_probabilities' function and 'iq_phase' function for the backend to execute.
+                :meth:`~MockIQExperimentHelper.compute_probabilities` and
+                :meth:`~MockIQExperimentHelper.iq_phase` methods for the backend to execute.
             rng_seed(int): The random seed value.
         """
 
         self._experiment_helper = experiment_helper
         self._rng = np.random.default_rng(rng_seed)
 
         super().__init__()
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/test/mock_iq_helpers.py` & `qiskit-experiments-0.6.0/qiskit_experiments/test/mock_iq_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,17 @@
         """Create a MockIQBackend helper object to define how the backend functions.
 
         :attr:`iq_cluster_centers` and :attr:`iq_cluster_width` define the base IQ
         cluster centers and standard deviations for each qubit in a
         :class:`MockIQBackend` instance. These are used by :meth:`iq_clusters` by
         default. Subclasses can override :meth:`iq_clusters` to return a modified
         version of :attr:`iq_cluster_centers` and :attr:`iq_cluster_width`.
-        `iq_cluster_centers` is a list of tuples. For a given qubit ``i_qbt`` and
+        :attr:`iq_cluster_centers` is a list of tuples. For a given qubit ``i_qbt`` and
         computational state ``i_state`` (either `0` or `1`), the centers of the IQ
-        clusters are found by indexing ``iq_cluster_centers`` as follows:
+        clusters are found by indexing :attr:`iq_cluster_centers` as follows:
 
         .. code-block:: python
 
             iq_center = helper.iq_cluster_centers[i_qbt][i_state]
             center_inphase = iq_center[0]
             center_quadrature = iq_center[1]
 
@@ -65,15 +65,15 @@
         properties are stored appropriately.
 
         Args:
             iq_cluster_centers: A list of tuples containing the clusters' centers in the IQ plane. There
                 are different centers for different logical values of the qubit. Defaults to a single
                 qubit with clusters in quadrants 1 and 3.
             iq_cluster_width: A list of standard deviation values for the sampling of each qubit.
-                Defaults to widths of 1.0 for each qubit in `iq_cluster_centers`.
+                Defaults to widths of 1.0 for each qubit in :attr:`iq_cluster_centers`.
 
         """
         self._iq_cluster_centers = (
             iq_cluster_centers if iq_cluster_centers is not None else [((-1.0, -1.0), (1.0, 1.0))]
         )
         self._iq_cluster_width = (
             iq_cluster_width
@@ -188,23 +188,23 @@
         circuits: List[QuantumCircuit],
     ) -> List[Tuple[List[Tuple[IQPoint, IQPoint]], List[float]]]:
         """Returns circuit-specific IQ cluster centers and widths in the IQ plane.
 
         Subclasses can override this function to modify the centers and widths of IQ clusters based on
         the circuits being simulated by a :class:`MockIQBackend`. The base centers and widths are
         stored internally within the helper object, and can be set in :meth:`__init__` or by modifying
-        attr:`iq_cluster_centers` and attr:`iq_cluster_width`. The default behaviour for
+        :attr:`iq_cluster_centers` and :attr:`iq_cluster_width`. The default behavior for
         :meth:`iq_clusters` is to return the centers and widths unmodified for each circuit in
-        `circuits`. Subclasses may return different centers and widths based on the circuits provided.
+        ``circuits``. Subclasses may return different centers and widths based on the circuits provided.
 
         The returned list contains a tuple per circuit. Each tuple contains the IQ centers and widths in
-        the same format as attr:`iq_cluster_centers` and attr:`iq_cluster_width`, passed as
+        the same format as :attr:`iq_cluster_centers` and :attr:`iq_cluster_width`, passed as
         arguments to :meth:`__init__`. The format of the centers and widths lists, in the argument
-        list and in the returned tuples, must match the format of `iq_cluster_centers` and
-        `iq_cluster_width` in :func:`qiskit_experiments.test.MockIQExperimentHelper.__init__`.
+        list and in the returned tuples, must match the format of :attr:`iq_cluster_centers` and
+        :attr:`iq_cluster_width` in :func:`qiskit_experiments.test.MockIQExperimentHelper.__init__`.
 
         Args:
             circuits: The quantum circuits for which the clusters should be modified.
 
         Returns:
             List: A list of tuples containing the circuit-specific IQ centers and widths for the
                 provided circuits.
@@ -220,16 +220,16 @@
         exp_list: List[BaseExperiment],
         exp_helper_list: List[MockIQExperimentHelper],
     ):
         """
         Parallel Experiment Helper initializer. The class assumes `exp_helper_list` is ordered to
         match the corresponding experiment in `exp_list`.
 
-        Note that :meth:`__init__` does not have `iq_cluster_centers` and `iq_cluster_width` as in
-        :func:`MockIQExperimentHelper.__init__`. This is because the centers and widths for
+        Note that :meth:`__init__` does not have :attr:`iq_cluster_centers` and :attr:`iq_cluster_width`
+        as in :func:`MockIQExperimentHelper.__init__`. This is because the centers and widths for
         :class:`MockIQParallelBackend` are stored in multiple experiment helpers in the list
         `exp_helper_list`.
 
         Args:
             exp_list(List): List of experiments.
             exp_helper_list(List): Ordered list of :class:`.MockIQExperimentHelper` corresponding to the
              experiments in `exp_list`. Nested parallel experiment aren't supported currently.
@@ -385,99 +385,55 @@
             that experiment.
 
         Raises:
             QiskitError: If an instruction is applied with qubits that don't belong to the same
             experiment.
             TypeError: The data type provided doesn't match the expected type (`tuple` or `int`).
         """
-        # exp_idx_map connects an experiment to its circuit in the output.
-        exp_idx_map = {exp: exp_idx for exp_idx, exp in enumerate(self.exp_list)}
-        qubit_exp_map = self._create_qubit_exp_map()
-
         exp_circuits_list = [[] for _ in self.exp_list]
+        qubits_expid_map = {exp.physical_qubits: i for i, exp in enumerate(self.exp_list)}
 
         for qc in qc_list:
-            # Quantum Register to qubit mapping
-            qubit_indices = {bit: idx for idx, bit in enumerate(qc.qubits)}
-
             # initialize quantum circuit for each experiment for this instance of circuit to fill
             # with instructions.
-            for exp_circuit in exp_circuits_list:
+            for i in range(len(self.exp_list)):
                 # we copy the circuit to ensure that the circuit properties (e.g. calibrations and qubit
                 # frequencies) are the same in the new circuit.
-                qcirc = qc.copy()
-                qcirc.data.clear()
-                qcirc.metadata.clear()
-                exp_circuit.append(qcirc)
+                empty_qc = qc.copy_empty_like()
+                empty_qc.metadata.clear()
+                exp_circuits_list[i].append(empty_qc)
 
             # fixing metadata
-            for exp_metadata in qc.metadata["composite_metadata"]:
-                # getting a qubit of one of the experiments that we ran in parallel. The key in the
-                # metadata is different for different experiments.
-                qubit_metadata = (
-                    exp_metadata.get("qubit")
-                    if exp_metadata.get("qubit") is not None
-                    else exp_metadata.get("qubits")
-                )
-                if isinstance(qubit_metadata, tuple):
-                    exp = qubit_exp_map[qubit_metadata[0]]
-                elif isinstance(qubit_metadata, int):
-                    exp = qubit_exp_map[qubit_metadata]
-                else:
-                    raise TypeError(
-                        f"The qubit information in the metadata is of type {type(qubit_metadata)}."
-                        f" Supported formats are `tuple` and `int`"
-                    )
-                # using the qubit to access the experiment. Then, we go to the last circuit in
-                # `exp_circuit` of the corresponding experiment, and we overwrite the metadata.
-                exp_circuits_list[exp_idx_map[exp]][-1].metadata = exp_metadata.copy()
+            for exp_idx, sub_metadata in zip(
+                qc.metadata["composite_index"],
+                qc.metadata["composite_metadata"],
+            ):
+                exp_circuits_list[exp_idx][-1].metadata = sub_metadata.copy()
+
             # sorting instructions by qubits indexes and inserting them into a circuit of the relevant
             # experiment
             for inst, qarg, carg in qc.data:
-                exp = qubit_exp_map[qubit_indices[qarg[0]]]
-                # making a list from the qubits the instruction affects
-                qubit_indexes = [qubit_indices[qr] for qr in qarg]
-                # check that the instruction is part of the experiment
-                if set(qubit_indexes).issubset(set(exp.physical_qubits)):
-                    # appending exp_circuits_list[experiment_index][last_circuit]
-                    exp_circuits_list[exp_idx_map[exp]][-1].append(inst, qarg, carg)
+                qubit_indices = set(qc.find_bit(qr).index for qr in qarg)
+                for qubits, exp_idx in qubits_expid_map.items():
+                    if qubit_indices.issubset(qubits):
+                        exp_circuits_list[exp_idx][-1].append(inst, qarg, carg)
+                        break
                 else:
                     raise QiskitError(
                         "A gate operates on two qubits that don't belong to the same experiment."
                     )
 
             # deleting empty circuits
             for exp_circuits in exp_circuits_list:
                 # 'exp_circuits' is a list of circuits of a specific experiment
                 if not exp_circuits[-1].data:
                     exp_circuits.pop()
 
         return exp_circuits_list
 
-    def _create_qubit_exp_map(self) -> Dict[int, BaseExperiment]:
-        """
-        Creating a dictionary that connect qubits to their respective experiments.
-        Returns:
-            Dict: A dictionary in the form {num: experiment} where num in experiment.physical_qubits
-
-        Raises:
-            QiskitError: If a qubit belong to two experiments.
-        """
-        qubit_experiment_mapping = {}
-        for exp in self.exp_list:
-            for qubit in exp.physical_qubits:
-                if qubit not in qubit_experiment_mapping:
-                    qubit_experiment_mapping[qubit] = exp
-                else:
-                    raise QiskitError(
-                        "There are duplications of qubits between parallel experiments"
-                    )
-
-        return qubit_experiment_mapping
-
 
 class MockIQDragHelper(MockIQExperimentHelper):
     """Functions needed for test_drag"""
 
     def __init__(
         self,
         gate_name: str = "Rp",
@@ -857,32 +813,29 @@
 
 
 class MockIQT1Helper(MockIQExperimentHelper):
     """Functions needed for T1 experiment on mock IQ backend"""
 
     def __init__(
         self,
-        t1: List[float] = None,
+        t1: float = None,
         iq_cluster_centers: Optional[List[Tuple[IQPoint, IQPoint]]] = None,
         iq_cluster_width: Optional[List[float]] = None,
     ):
         super().__init__(iq_cluster_centers, iq_cluster_width)
-        self._t1 = t1 or [90e-6]
+        self._t1 = t1 or 90e-6
 
     def compute_probabilities(self, circuits: List[QuantumCircuit]) -> List[Dict[str, float]]:
         """Return the probability of being in the excited state."""
         output_dict_list = []
         for circuit in circuits:
             probability_output_dict = {}
 
             # extracting information from the circuit.
-            qubit_idx = circuit.metadata["qubit"]
             delay = circuit.metadata["xval"]
 
             # creating a probability dict.
-            if qubit_idx >= len(self._t1):
-                raise QiskitError(f"There is no 'T1' value for qubit index {qubit_idx}.")
-            probability_output_dict["1"] = np.exp(-delay / self._t1[qubit_idx])
+            probability_output_dict["1"] = np.exp(-delay / self._t1)
             probability_output_dict["0"] = 1 - probability_output_dict["1"]
             output_dict_list.append(probability_output_dict)
 
         return output_dict_list
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/test/pulse_backend.py` & `qiskit-experiments-0.6.0/qiskit_experiments/test/pulse_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,33 +31,32 @@
 from qiskit.pulse.transforms import block_to_schedule
 from qiskit.qobj.pulse_qobj import PulseQobjInstruction
 from qiskit.qobj.utils import MeasLevel, MeasReturnType
 from qiskit.quantum_info.states import DensityMatrix, Statevector
 from qiskit.result import Result, Counts
 from qiskit.transpiler import InstructionProperties, Target
 
-from qiskit_dynamics import Solver
-from qiskit_dynamics.pulse import InstructionToSignals
-
+from qiskit_experiments.warnings import HAS_DYNAMICS
 from qiskit_experiments.data_processing.discriminator import BaseDiscriminator
 from qiskit_experiments.exceptions import QiskitError
 from qiskit_experiments.test.utils import FakeJob
 
 
+@HAS_DYNAMICS.require_in_instance
 class PulseBackend(BackendV2):
     r"""Abstract base class for pulse simulation backends in Qiskit Experiments.
 
     This backend is designed for the tests in Qiskit Experiments as well as for the
     tutorials in Qiskit Experiments. The backend has a Qiskit Dynamics pulse simulator
     which allows it to simulate pulse schedules that are included in the calibrations
     attached to quantum circuits. In addition, sub-classes should implement a set of default
     schedules so that circuits that do not provide calibrations can also run, much like
     the hardware backends. In addition, the backends are also capable of simulating level-
     one (IQ data) and level-two (counts) data. Subclasses of these backends can have an
-    optional disciminator so that they can produce counts based on sampled IQ data. If
+    optional discriminator so that they can produce counts based on sampled IQ data. If
     a discriminator is not provided then the counts will be produced from a statevector
     or density matrix.
 
     .. warning::
 
         Some of the functionality in this backend may move to Qiskit Dynamics and/or be
         refactored. These backends are not intended as a general pulse-simulator backend
@@ -69,33 +68,39 @@
         self,
         static_hamiltonian: np.ndarray,
         hamiltonian_operators: np.ndarray,
         static_dissipators: Optional[np.ndarray] = None,
         dt: float = 0.1 * 1e-9,
         solver_method="RK23",
         seed: int = 0,
+        atol: float = None,
+        rtol: float = None,
         **kwargs,
     ):
         """Initialize a backend with model information.
 
         Args:
             static_hamiltonian: Time-independent term in the Hamiltonian.
             hamiltonian_operators: List of time-dependent operators
             static_dissipators: Constant dissipation operators. Defaults to None.
             dt: Sample rate for simulating pulse schedules. Defaults to 0.1*1e-9.
             solver_method: Numerical solver method to use. Check qiskit_dynamics for available
                 methods. Defaults to "RK23".
             seed: An optional seed given to the random number generator. If this argument is not
                 set then the seed defaults to 0.
+            atol: Absolute tolerance during solving.
+            rtol: Relative tolerance during solving.
         """
+        from qiskit_dynamics import Solver
+
         super().__init__(
             None,
             name="PulseBackendV2",
             description="A PulseBackend simulator",
-            online_date=datetime.datetime.utcnow(),
+            online_date=datetime.datetime.now(datetime.timezone.utc),
             backend_version="0.0.1",
         )
 
         # subclasses must implements default pulse schedules
         self._defaults = None
 
         self._target = Target(dt=dt, granularity=16)
@@ -104,14 +109,20 @@
         self._rng = np.random.default_rng(seed)
 
         # The instance to convert pulse schedules to signals for Qiskit Dynamics.
         self.converter = None
 
         self.solver_method = solver_method
 
+        self.solve_kwargs = {}
+        if atol:
+            self.solve_kwargs["atol"] = atol
+        if rtol:
+            self.solve_kwargs["rtol"] = rtol
+
         self.static_hamiltonian = static_hamiltonian
         self.hamiltonian_operators = hamiltonian_operators
         self.static_dissipators = static_dissipators
         self.solver = Solver(
             static_hamiltonian=self.static_hamiltonian,
             hamiltonian_operators=self.hamiltonian_operators,
             static_dissipators=self.static_dissipators,
@@ -334,14 +345,15 @@
         time_f = schedule.duration * self.dt
         unitary = self.solver.solve(
             t_span=[0.0, time_f],
             y0=self.y_0,
             t_eval=[time_f],
             signals=signal,
             method=self.solver_method,
+            **self.solve_kwargs,
         ).y[0]
 
         return unitary
 
     def run(self, run_input: Union[QuantumCircuit, List[QuantumCircuit]], **run_options) -> FakeJob:
         """Run method takes circuits as input and returns FakeJob with IQ data or counts.
 
@@ -426,49 +438,56 @@
                 run_result["data"]["memory"] = measurement_data
 
             result["results"].append(run_result)
 
         return FakeJob(self, Result.from_dict(result))
 
 
+@HAS_DYNAMICS.require_in_instance
 class SingleTransmonTestBackend(PulseBackend):
     r"""A backend that corresponds to a three level anharmonic transmon qubit.
 
     The Hamiltonian of the system is
 
     .. math::
         H = \hbar \sum_{j=1,2} \left[\omega_j |j\rangle\langle j| +
                 \mathcal{E}(t) \lambda_j (\sigma_j^+ + \sigma_j^-)\right]
 
-    Here, :math:`\omega_j` is the transition frequency from level :math`0` to level
+    Here, :math:`\omega_j` is the transition frequency from level :math:`0` to level
     :math:`j`. :math:`\mathcal{E}(t)` is the drive field and :math:`\sigma_j^\pm` are
     the raising and lowering operators between levels :math:`j-1` and :math:`j`.
     """
 
     def __init__(
         self,
         qubit_frequency: float = 5e9,
         anharmonicity: float = -0.25e9,
         lambda_1: float = 1e9,
         lambda_2: float = 0.8e9,
         gamma_1: float = 1e4,
         noise: bool = True,
+        atol: float = None,
+        rtol: float = None,
         **kwargs,
     ):
         """Initialise backend with hamiltonian parameters
 
         Args:
             qubit_frequency: Frequency of the qubit (0-1). Defaults to 5e9.
             anharmonicity: Qubit anharmonicity $\\alpha$ = f12 - f01. Defaults to -0.25e9.
             lambda_1: Strength of 0-1 transition. Defaults to 1e9.
             lambda_2: Strength of 1-2 transition. Defaults to 0.8e9.
             gamma_1: Relaxation rate (1/T1) for 1-0. Defaults to 1e4.
             noise: Defaults to True. If True then T1 dissipation is included in the pulse-simulation.
                 The strength is given by ``gamma_1``.
+            atol: Absolute tolerance during solving.
+            rtol: Relative tolerance during solving.
         """
+        from qiskit_dynamics.pulse import InstructionToSignals
+
         qubit_frequency_02 = 2 * qubit_frequency + anharmonicity
         ket0 = np.array([[1, 0, 0]]).T
         ket1 = np.array([[0, 1, 0]]).T
         ket2 = np.array([[0, 0, 1]]).T
 
         sigma_m1 = ket0 @ ket1.T.conj()
         sigma_m2 = ket1 @ ket2.T.conj()
@@ -501,14 +520,16 @@
             static_hamiltonian=drift,
             hamiltonian_operators=control,
             static_dissipators=static_dissipators,
             rotating_frame=r_frame,
             rwa_cutoff_freq=1.9 * qubit_frequency,
             rwa_carrier_freqs=[qubit_frequency],
             evaluation_mode=evaluation_mode,
+            atol=atol,
+            rtol=rtol,
             **kwargs,
         )
 
         self._defaults = PulseDefaults.from_dict(
             {
                 "qubit_freq_est": [qubit_frequency / 1e9],
                 "meas_freq_est": [0],
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/test/t2hahn_backend.py` & `qiskit-experiments-0.6.0/qiskit_experiments/test/t2hahn_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/test/utils.py` & `qiskit-experiments-0.6.0/qiskit_experiments/test/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/version.py` & `qiskit-experiments-0.6.0/qiskit_experiments/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/visualization/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/visualization/drawers/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/visualization/drawers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/visualization/drawers/base_drawer.py` & `qiskit-experiments-0.6.0/qiskit_experiments/visualization/drawers/base_drawer.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,16 +107,14 @@
     2. Initialize the canvas.
     3. Call relevant drawing methods to create the figure. When calling the drawing
        method that creates the graphic you would like to use in the legend, set
        ``legend=True``. For example, ``drawer.scatter(...,legend=True)`` would use
        the scatter points as the legend graphics for the given series.
     4. Format the canvas and call :meth:`figure` to get the figure.
 
-    |
-
     .. rubric:: Options and Figure Options
 
     Drawers have both :attr:`options` and :attr:`figure_options` available to set
     parameters that define how to draw and what is drawn, respectively.
     :class:`BasePlotter` is similar in that it also has ``options`` and
     ``figure_options``. The former contains class-specific variables that define how an
     instance behaves. The latter contains figure-specific variables that typically
@@ -192,57 +190,78 @@
         """Return default figure options.
 
         Figure Options:
             xlabel (Union[str, List[str]]): X-axis label string of the output figure. If
                 there are multiple columns in the canvas, this could be a list of labels.
             ylabel (Union[str, List[str]]): Y-axis label string of the output figure. If
                 there are multiple rows in the canvas, this could be a list of labels.
-            xlim (Tuple[float, float]): Min and max value of the horizontal axis. If not
-                provided, it is automatically scaled based on the input data points.
-            ylim (Tuple[float, float]): Min and max value of the vertical axis. If not
-                provided, it is automatically scaled based on the input data points.
-            xval_unit (str): Unit of x values. No scaling prefix is needed here as this
-                is controlled by ``xval_unit_scale``.
-            yval_unit (str): Unit of y values. See ``xval_unit`` for details.
-            xval_unit_scale (bool): Whether to add an SI unit prefix to ``xval_unit`` if
-                needed. For example, when the x values represent time and
+            xlim (Union[Tuple[float, float], List[Tuple[float, float]]): Min and max value
+                of the horizontal axis. If not provided, it is automatically scaled based
+                on the input data points. If there are multiple columns in the canvas,
+                this could be a list of xlims.
+            ylim (Union[Tuple[float, float], List[Tuple[float, float]]): Min and max value
+                of the vertical axis. If not provided, it is automatically scaled based
+                on the input data points. If there are multiple rows in the canvas,
+                this could be a list of ylims.
+            xval_unit (Union[str, List[str]]): Unit of x values.
+                No scaling prefix is needed here as this is controlled by ``xval_unit_scale``.
+                If there are multiple columns in the canvas, this could be a list of xval_units.
+            yval_unit (Union[str, List[str]]): Unit of y values.
+                No scaling prefix is needed here as this is controlled by ``yval_unit_scale``.
+                If there are multiple rows in the canvas, this could be a list of yval_units.
+            xval_unit_scale (Union[bool, List[bool]]): Whether to add an SI unit prefix to
+                ``xval_unit`` if needed. For example, when the x values represent time and
                 ``xval_unit="s"``, ``xval_unit_scale=True`` adds an SI unit prefix to
                 ``"s"`` based on X values of plotted data. In the output figure, the
                 prefix is automatically selected based on the maximum value in this
                 axis. If your x values are in [1e-3, 1e-4], they are displayed as [1 ms,
                 10 ms]. By default, this option is set to ``True``. If ``False`` is
                 provided, the axis numbers will be displayed in the scientific notation.
-            yval_unit_scale (bool): Whether to add an SI unit prefix to ``yval_unit`` if
-                needed. See ``xval_unit_scale`` for details.
+                If there are multiple columns in the canvas, this could be a list of xval_unit_scale.
+            yval_unit_scale (Union[bool, List[bool]]): Whether to add an SI unit prefix to
+                ``yval_unit`` if needed. See ``xval_unit_scale`` for details.
+                If there are multiple rows in the canvas, this could be a list of yval_unit_scale.
+            xscale (str): The scaling of the x-axis, such as ``log`` or ``linear``.
+            yscale (str): The scaling of the y-axis, such as ``log`` or ``linear``.
             figure_title (str): Title of the figure. Defaults to None, i.e. nothing is
                 shown.
+            sharex (bool): Set True to share x-axis ticks among sub-plots.
+            sharey (bool): Set True to share y-axis ticks among sub-plots.
             series_params (Dict[str, Dict[str, Any]]): A dictionary of parameters for
                 each series. This is keyed on the name for each series. Sub-dictionary
                 is expected to have the following three configurations, "canvas",
                 "color", "symbol" and "label"; "canvas" is the integer index of axis
                 (when multi-canvas plot is set), "color" is the color of the drawn
                 graphics, "symbol" is the series marker style for scatter plots, and
                 "label" is a user provided series label that appears in the legend.
             custom_style (PlotStyle): The style definition to use when drawing. This
                 overwrites style parameters in ``default_style`` in :attr:`options`.
                 Defaults to an empty PlotStyle instance (i.e., ``PlotStyle()``).
         """
-        return Options(
+        options = Options(
             xlabel=None,
             ylabel=None,
             xlim=None,
             ylim=None,
             xval_unit=None,
             yval_unit=None,
             xval_unit_scale=True,
             yval_unit_scale=True,
+            xscale=None,
+            yscale=None,
+            sharex=True,
+            sharey=True,
             figure_title=None,
             series_params={},
             custom_style=PlotStyle(),
         )
+        options.set_validator("xscale", ["linear", "log", "symlog", "logit", "quadratic", None])
+        options.set_validator("yscale", ["linear", "log", "symlog", "logit", "quadratic", None])
+
+        return options
 
     def set_options(self, **fields):
         """Set the drawer options.
 
         Args:
             fields: The fields to update the options
 
@@ -376,14 +395,38 @@
             name: Name of this series.
             label: Optional legend label to override ``name`` and ``series_params``.
             legend: Whether the drawn area must have a legend entry. Defaults to False.
                 The series label in the legend will be ``label`` if it is not None. If
                 it is, then ``series_params`` is searched for a ``"label"`` entry for
                 the series identified by ``name``. If this is also ``None``, then
                 ``name`` is used as the fallback. If no ``name`` is provided, then no
+                legend entry is generated.
+            options: Valid options for the drawer backend API.
+        """
+
+    @abstractmethod
+    def hline(
+        self,
+        y_value: float,
+        name: Optional[SeriesName] = None,
+        label: Optional[str] = None,
+        legend: bool = False,
+        **options,
+    ):
+        """Draw a horizontal line.
+
+        Args:
+            y_value: Y value for line.
+            name: Name of this series.
+            label: Optional legend label to override ``name`` and ``series_params``.
+            legend: Whether the drawn area must have a legend entry. Defaults to False.
+                The series label in the legend will be ``label`` if it is not None. If
+                it is, then ``series_params`` is searched for a ``"label"`` entry for
+                the series identified by ``name``. If this is also ``None``, then
+                ``name`` is used as the fallback. If no ``name`` is provided, then no
                 legend entry is generated.
             options: Valid options for the drawer backend API.
         """
 
     @abstractmethod
     def filled_y_area(
         self,
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/visualization/drawers/legacy_curve_compat_drawer.py` & `qiskit-experiments-0.6.0/qiskit_experiments/visualization/drawers/legacy_curve_compat_drawer.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,29 +10,24 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Compatibility wrapper for legacy BaseCurveDrawer."""
 
 import warnings
 from typing import Any, Optional, Sequence, Tuple, Union
-
 import numpy as np
 
+from qiskit.utils.deprecation import deprecate_func
+
 from qiskit_experiments.curve_analysis.visualization import BaseCurveDrawer
-from qiskit_experiments.warnings import deprecated_class
 
 from ..utils import ExtentTuple
 from .base_drawer import BaseDrawer
 
 
-@deprecated_class(
-    "0.6",
-    msg="Legacy drawers from `.curve_analysis.visualization are deprecated. This compatibility wrapper "
-    "will be removed alongside the deprecated modules removal",
-)
 class LegacyCurveCompatDrawer(BaseDrawer):
     """A compatibility wrapper for the legacy and deprecated :class:`BaseCurveDrawer`.
 
     :mod:`qiskit_experiments.curve_analysis.visualization` is deprecated and will be
     replaced with the new :mod:`qiskit_experiments.visualization` module. Analysis
     classes instead use subclasses of :class:`BasePlotter` to generate figures. This
     class wraps the legacy :class:`BaseCurveDrawer` class so it can be used by analysis
@@ -40,14 +35,21 @@
 
     .. note::
         As :class:`BaseCurveDrawer` doesn't support customizing legend entries, the
         ``legend`` and ``label`` parameters in drawing methods (such as
         :meth:`scatter`) are unsupported and do nothing.
     """
 
+    @deprecate_func(
+        since="0.5",
+        additional_msg="Legacy drawers from ``curve_analysis.visualization`` are deprecated. "
+        "This compatibility wrapper will be removed alongside the deprecated modules removal",
+        removal_timeline="after 0.6",
+        package_name="qiskit-experiments",
+    )
     def __init__(self, curve_drawer: BaseCurveDrawer):
         """Create a LegacyCurveCompatDrawer instance.
 
         Args:
             curve_drawer: A legacy BaseCurveDrawer to wrap in the compatibility drawer.
         """
         super().__init__()
@@ -115,14 +117,45 @@
             legend: Unsupported as :class:`BaseCurveDrawer` doesn't support toggling
                 legend entries.
             options: Valid options for the drawer backend API.
         """
         self._curve_drawer.draw_fit_line(x_data, y_data, name, **options)
 
     # pylint: disable=unused-argument
+    def hline(
+        self,
+        y_value: float,
+        name: Optional[str] = None,
+        label: Optional[str] = None,
+        legend: bool = False,
+        **options,
+    ):
+        """Draw a horizontal line.
+
+        .. note::
+
+            This method was added to fulfill the
+            :class:`~qiskit_experiments.visualization.BaseDrawer` interface,
+            but it is not supported for this class since there was no
+            equivalent in
+            :class:`~qiskit_experiments.curve_analysis.visualization.BaseCurveDrawer`.
+
+        Args:
+            y_value: Y value for line.
+            name: Name of this series.
+            label: Unsupported label option
+            legend: Unsupported legend option
+            options: Additional options
+        """
+        warnings.warn(
+            "hline is not supported by the LegacyCurveCompatDrawer",
+            UserWarning,
+        )
+
+    # pylint: disable=unused-argument
     def filled_y_area(
         self,
         x_data: Sequence[float],
         y_ub: Sequence[float],
         y_lb: Sequence[float],
         name: Optional[str] = None,
         label: Optional[str] = None,
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/visualization/drawers/mpl_drawer.py` & `qiskit-experiments-0.6.0/qiskit_experiments/visualization/drawers/mpl_drawer.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Curve drawer for matplotlib backend."""
 
+import numbers
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 from matplotlib.axes import Axes
 from matplotlib.cm import tab10
 from matplotlib.colors import Colormap, LinearSegmentedColormap
 from matplotlib.figure import Figure
@@ -75,14 +76,17 @@
         if not self.options.axis:
             axis = get_non_gui_ax()
             figure = axis.get_figure()
             figure.set_size_inches(*self.style["figsize"])
         else:
             axis = self.options.axis
 
+        sharex = self.figure_options.sharex
+        sharey = self.figure_options.sharey
+
         n_rows, n_cols = self.options.subplots
         n_subplots = n_cols * n_rows
         if n_subplots > 1:
             # Add inset axis. User may provide a single axis object via the analysis option,
             # while this analysis tries to draw its result in multiple canvases,
             # especially when the analysis consists of multiple curves.
             # Inset axis is experimental implementation of matplotlib 3.0 so maybe unstable API.
@@ -95,28 +99,28 @@
                     bounds = [
                         inset_ax_w * j,
                         1 - inset_ax_h * (i + 1),
                         inset_ax_w,
                         inset_ax_h,
                     ]
                     sub_ax = axis.inset_axes(bounds, transform=axis.transAxes, zorder=1)
-                    if j != 0:
+                    if j != 0 and sharey:
                         # remove y axis except for most-left plot
-                        sub_ax.set_yticklabels([])
+                        sub_ax.yaxis.set_tick_params(labelleft=False)
                     else:
                         # this axis locates at left, write y-label
                         if self.figure_options.ylabel:
                             label = self.figure_options.ylabel
                             if isinstance(label, list):
                                 # Y label can be given as a list for each sub axis
                                 label = label[i]
                             sub_ax.set_ylabel(label, fontsize=self.style["axis_label_size"])
-                    if i != n_rows - 1:
+                    if i != n_rows - 1 and sharex:
                         # remove x axis except for most-bottom plot
-                        sub_ax.set_xticklabels([])
+                        sub_ax.xaxis.set_tick_params(labelleft=False)
                     else:
                         # this axis locates at bottom, write x-label
                         if self.figure_options.xlabel:
                             label = self.figure_options.xlabel
                             if isinstance(label, list):
                                 # X label can be given as a list for each sub axis
                                 label = label[j]
@@ -139,102 +143,143 @@
     def format_canvas(self):
         if self._axis.child_axes:
             # Multi canvas mode
             all_axes = self._axis.child_axes
         else:
             all_axes = [self._axis]
 
-        # Add data labels if there are multiple labels registered per sub_ax.
-        for sub_ax in all_axes:
-            _, labels = sub_ax.get_legend_handles_labels()
-            if len(labels) > 1:
-                sub_ax.legend(loc=self.style["legend_loc"])
+        # Set axes scale. This needs to be done before anything tries to work with
+        # the axis limits because if no limits or data are set explicitly the
+        # default limits depend on the scale method (for example, the minimum
+        # value is 0 for linear scaling but not for log scaling).
+        def signed_sqrt(x):
+            return np.sign(x) * np.sqrt(abs(x))
+
+        def signed_square(x):
+            return np.sign(x) * x**2
 
-        # Format x and y axis
         for ax_type in ("x", "y"):
-            # Get axis formatter from drawing options
-            if ax_type == "x":
-                lim = self.figure_options.xlim
-                unit = self.figure_options.xval_unit
-                unit_scale = self.figure_options.xval_unit_scale
-            else:
-                lim = self.figure_options.ylim
-                unit = self.figure_options.yval_unit
-                unit_scale = self.figure_options.yval_unit_scale
-
-            # Compute data range from auto scale
-            if not lim:
-                v0 = np.nan
-                v1 = np.nan
-                for sub_ax in all_axes:
-                    if ax_type == "x":
-                        this_v0, this_v1 = sub_ax.get_xlim()
-                    else:
-                        this_v0, this_v1 = sub_ax.get_ylim()
-                    v0 = np.nanmin([v0, this_v0])
-                    v1 = np.nanmax([v1, this_v1])
-                lim = (v0, v1)
-
-            # Format axis number notation
-            if unit and unit_scale:
-                # If value is specified, automatically scale axis magnitude
-                # and write prefix to axis label, i.e. 1e3 Hz -> 1 kHz
-                maxv = max(np.abs(lim[0]), np.abs(lim[1]))
-                try:
-                    scaled_maxv, prefix = detach_prefix(maxv, decimal=3)
-                    prefactor = scaled_maxv / maxv
-                except ValueError:
-                    prefix = ""
-                    prefactor = 1
-
-                formatter = MplDrawer.PrefixFormatter(prefactor)
-                units_str = f" [{prefix}{unit}]"
-            else:
-                # Use scientific notation with 3 digits, 1000 -> 1e3
-                formatter = ScalarFormatter()
-                formatter.set_scientific(True)
-                formatter.set_powerlimits((-3, 3))
+            for sub_ax in all_axes:
+                scale = self.figure_options.get(f"{ax_type}scale")
+                if ax_type == "x":
+                    mpl_setscale = sub_ax.set_xscale
+                else:
+                    mpl_setscale = sub_ax.set_yscale
 
-                units_str = f" [{unit}]" if unit else ""
+                # Apply non linear axis spacing
+                if scale is not None:
+                    if scale == "quadratic":
+                        mpl_setscale("function", functions=(signed_square, signed_sqrt))
+                    else:
+                        mpl_setscale(scale)
 
+        # Get axis formatter from drawing options
+        formatter_opts = {}
+        for ax_type in ("x", "y"):
+            limit = self.figure_options.get(f"{ax_type}lim")
+            unit = self.figure_options.get(f"{ax_type}val_unit")
+            unit_scale = self.figure_options.get(f"{ax_type}val_unit_scale")
+
+            # Format options to a list for each axis
+            if limit is None or isinstance(limit[0], numbers.Number):
+                limit = [limit] * len(all_axes)
+            if unit is None or isinstance(unit, str):
+                unit = [unit] * len(all_axes)
+            if isinstance(unit_scale, bool):
+                unit_scale = [unit_scale] * len(all_axes)
+
+            # Compute min-max value for auto scaling
+            min_vals = []
+            max_vals = []
             for sub_ax in all_axes:
                 if ax_type == "x":
-                    ax = getattr(sub_ax, "xaxis")
-                    tick_labels = sub_ax.get_xticklabels()
+                    min_v, max_v = sub_ax.get_xlim()
+                else:
+                    min_v, max_v = sub_ax.get_ylim()
+                min_vals.append(min_v)
+                max_vals.append(max_v)
+
+            formatter_opts[ax_type] = {
+                "limit": limit,
+                "unit": unit,
+                "unit_scale": unit_scale,
+                "min_ax_vals": min_vals,
+                "max_ax_vals": max_vals,
+            }
+
+        for i, sub_ax in enumerate(all_axes):
+            # Add data labels if there are multiple labels registered per sub_ax.
+            _, labels = sub_ax.get_legend_handles_labels()
+            if len(labels) > 1:
+                sub_ax.legend(loc=self.style["legend_loc"])
+
+            for ax_type in ("x", "y"):
+                limit = formatter_opts[ax_type]["limit"][i]
+                unit = formatter_opts[ax_type]["unit"][i]
+                unit_scale = formatter_opts[ax_type]["unit_scale"][i]
+                min_ax_vals = formatter_opts[ax_type]["min_ax_vals"]
+                max_ax_vals = formatter_opts[ax_type]["max_ax_vals"]
+                share_axis = self.figure_options.get(f"share{ax_type}")
+
+                if ax_type == "x":
+                    mpl_axis_obj = getattr(sub_ax, "xaxis")
+                    mpl_setlimit = sub_ax.set_xlim
+                    mpl_share = sub_ax.sharex
+                else:
+                    mpl_axis_obj = getattr(sub_ax, "yaxis")
+                    mpl_setlimit = sub_ax.set_ylim
+                    mpl_share = sub_ax.sharey
+
+                if limit is None:
+                    if share_axis:
+                        limit = min(min_ax_vals), max(max_ax_vals)
+                    else:
+                        limit = min_ax_vals[i], max_ax_vals[i]
+
+                # Create formatter for axis tick label notation
+                if unit and unit_scale:
+                    # If value is specified, automatically scale axis magnitude
+                    # and write prefix to axis label, i.e. 1e3 Hz -> 1 kHz
+                    maxv = max(np.abs(limit[0]), np.abs(limit[1]))
+                    try:
+                        scaled_maxv, prefix = detach_prefix(maxv, decimal=3)
+                        prefactor = scaled_maxv / maxv
+                    except ValueError:
+                        prefix = ""
+                        prefactor = 1
+                    formatter = MplDrawer.PrefixFormatter(prefactor)
+                    units_str = f" [{prefix}{unit}]"
                 else:
-                    ax = getattr(sub_ax, "yaxis")
-                    tick_labels = sub_ax.get_yticklabels()
+                    # Use scientific notation with 3 digits, 1000 -> 1e3
+                    formatter = ScalarFormatter()
+                    formatter.set_scientific(True)
+                    formatter.set_powerlimits((-3, 3))
+                    units_str = f" [{unit}]" if unit else ""
+                mpl_axis_obj.set_major_formatter(formatter)
 
-                if tick_labels:
-                    # Set formatter only when tick labels exist
-                    ax.set_major_formatter(formatter)
+                # Add units to axis label if both exist
                 if units_str:
-                    # Add units to label if both exist
-                    label_txt_obj = ax.get_label()
+                    label_txt_obj = mpl_axis_obj.get_label()
                     label_str = label_txt_obj.get_text()
                     if label_str:
                         label_txt_obj.set_text(label_str + units_str)
 
-            # Auto-scale all axes to the first sub axis
-            if ax_type == "x":
-                # get_shared_y_axes() is immutable from matplotlib>=3.6.0. Must use Axis.sharey()
-                # instead, but this can only be called once per axis. Here we call sharey  on all axes in
-                # a chain, which should have the same effect.
-                if len(all_axes) > 1:
-                    for ax1, ax2 in zip(all_axes[1:], all_axes[0:-1]):
-                        ax1.sharex(ax2)
-                all_axes[0].set_xlim(lim)
-            else:
-                # get_shared_y_axes() is immutable from matplotlib>=3.6.0. Must use Axis.sharey()
-                # instead, but this can only be called once per axis. Here we call sharey  on all axes in
-                # a chain, which should have the same effect.
-                if len(all_axes) > 1:
-                    for ax1, ax2 in zip(all_axes[1:], all_axes[0:-1]):
-                        ax1.sharey(ax2)
-                all_axes[0].set_ylim(lim)
+                # Consider axis sharing among subplots
+                if share_axis:
+                    if i == 0:
+                        # Limit is set to the first axis only.
+                        mpl_setlimit(limit)
+                    else:
+                        # get_shared_*_axes() is immutable from matplotlib>=3.6.0.
+                        # Must use Axis.share*() instead, but this can only be called once per axis.
+                        # Here we call share* on all axes in a chain, which should have the same effect.
+                        mpl_share(all_axes[i - 1])
+                else:
+                    mpl_setlimit(limit)
+
         # Add title
         if self.figure_options.figure_title is not None:
             self._axis.set_title(
                 label=self.figure_options.figure_title,
                 fontsize=self.style["axis_label_size"],
             )
 
@@ -387,21 +432,42 @@
     ):
         series_params = self.figure_options.series_params.get(name, {})
         axis = series_params.get("canvas", None)
         color = series_params.get("color", self._get_default_color(name))
 
         draw_ops = {
             "color": color,
-            "linestyle": "-",
-            "linewidth": 2,
+            "linestyle": series_params.get("linestyle", "-"),
+            "linewidth": series_params.get("linewidth", 2),
         }
         self._update_label_in_options(draw_ops, name, label, legend)
         draw_ops.update(**options)
         self._get_axis(axis).plot(x_data, y_data, **draw_ops)
 
+    def hline(
+        self,
+        y_value: float,
+        name: Optional[SeriesName] = None,
+        label: Optional[str] = None,
+        legend: bool = False,
+        **options,
+    ):
+        series_params = self.figure_options.series_params.get(name, {})
+        axis = series_params.get("canvas", None)
+        color = series_params.get("color", self._get_default_color(name))
+
+        draw_ops = {
+            "color": color,
+            "linestyle": series_params.get("linestyle", "-"),
+            "linewidth": series_params.get("linewidth", 2),
+        }
+        self._update_label_in_options(draw_ops, name, label, legend)
+        draw_ops.update(**options)
+        self._get_axis(axis).axhline(y_value, **draw_ops)
+
     def filled_y_area(
         self,
         x_data: Sequence[float],
         y_ub: Sequence[float],
         y_lb: Sequence[float],
         name: Optional[SeriesName] = None,
         label: Optional[str] = None,
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/visualization/plotters/__init__.py` & `qiskit-experiments-0.6.0/qiskit_experiments/visualization/plotters/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/visualization/plotters/base_plotter.py` & `qiskit-experiments-0.6.0/qiskit_experiments/visualization/plotters/base_plotter.py`

 * *Files 6% similar despite different names*

```diff
@@ -417,60 +417,78 @@
         )
 
     @classmethod
     def _default_figure_options(cls) -> Options:
         """Return default figure options.
 
         Figure Options:
-            xlabel (Union[str, List[str]]): X-axis label string of the output figure.
-                If there are multiple columns in the canvas, this could be a list of
-                labels.
-            ylabel (Union[str, List[str]]): Y-axis label string of the output figure.
-                If there are multiple rows in the canvas, this could be a list of
-                labels.
-            xlim (Tuple[float, float]): Min and max value of the horizontal axis.
-                If not provided, it is automatically scaled based on the input data
-                points.
-            ylim (Tuple[float, float]): Min and max value of the vertical axis.
-                If not provided, it is automatically scaled based on the input data
-                points.
-            xval_unit (str): Unit of x values. No scaling prefix is needed here as this
-                is controlled by ``xval_unit_scale``.
-            yval_unit (str): Unit of y values. See ``xval_unit`` for details.
-            xval_unit_scale (bool): Whether to add an SI unit prefix to ``xval_unit`` if
-                needed. For example, when the x values represent time and
+            xlabel (Union[str, List[str]]): X-axis label string of the output figure. If
+                there are multiple columns in the canvas, this could be a list of labels.
+            ylabel (Union[str, List[str]]): Y-axis label string of the output figure. If
+                there are multiple rows in the canvas, this could be a list of labels.
+            xlim (Union[Tuple[float, float], List[Tuple[float, float]]): Min and max value
+                of the horizontal axis. If not provided, it is automatically scaled based
+                on the input data points. If there are multiple columns in the canvas,
+                this could be a list of xlims.
+            ylim (Union[Tuple[float, float], List[Tuple[float, float]]): Min and max value
+                of the vertical axis. If not provided, it is automatically scaled based
+                on the input data points. If there are multiple rows in the canvas,
+                this could be a list of ylims.
+            xval_unit (Union[str, List[str]]): Unit of x values.
+                No scaling prefix is needed here as this is controlled by ``xval_unit_scale``.
+                If there are multiple columns in the canvas, this could be a list of xval_units.
+            yval_unit (Union[str, List[str]]): Unit of y values.
+                No scaling prefix is needed here as this is controlled by ``yval_unit_scale``.
+                If there are multiple rows in the canvas, this could be a list of yval_units.
+            xval_unit_scale (Union[bool, List[bool]]): Whether to add an SI unit prefix to
+                ``xval_unit`` if needed. For example, when the x values represent time and
                 ``xval_unit="s"``, ``xval_unit_scale=True`` adds an SI unit prefix to
                 ``"s"`` based on X values of plotted data. In the output figure, the
                 prefix is automatically selected based on the maximum value in this
                 axis. If your x values are in [1e-3, 1e-4], they are displayed as [1 ms,
                 10 ms]. By default, this option is set to ``True``. If ``False`` is
                 provided, the axis numbers will be displayed in the scientific notation.
-            yval_unit_scale (bool): Whether to add an SI unit prefix to ``yval_unit`` if
-                needed. See ``xval_unit_scale`` for details.
+                If there are multiple columns in the canvas, this could be a list of xval_unit_scale.
+            yval_unit_scale (Union[bool, List[bool]]): Whether to add an SI unit prefix to
+                ``yval_unit`` if needed. See ``xval_unit_scale`` for details.
+                If there are multiple rows in the canvas, this could be a list of yval_unit_scale.
+            xscale (str): The scaling of the x-axis, such as ``log`` or ``linear``.
+            yscale (str): The scaling of the y-axis, such as ``log`` or ``linear``.
             figure_title (str): Title of the figure. Defaults to None, i.e. nothing is
                 shown.
-            series_params (Dict[SeriesName, Dict[str, Any]]): A dictionary of plot
-                parameters for each series. This is keyed on the name for each series.
-                Sub-dictionary is expected to have following three configurations,
-                "canvas", "color", and "symbol"; "canvas" is the integer index of axis
-                (when multi-canvas plot is set), "color" is the color of the curve, and
-                "symbol" is the marker Style of the curve for scatter plots.
+            sharex (bool): Set True to share x-axis ticks among sub-plots.
+            sharey (bool): Set True to share y-axis ticks among sub-plots.
+            series_params (Dict[str, Dict[str, Any]]): A dictionary of parameters for
+                each series. This is keyed on the name for each series. Sub-dictionary
+                is expected to have the following three configurations, "canvas",
+                "color", "symbol" and "label"; "canvas" is the integer index of axis
+                (when multi-canvas plot is set), "color" is the color of the drawn
+                graphics, "symbol" is the series marker style for scatter plots, and
+                "label" is a user provided series label that appears in the legend.
         """
-        return Options(
+        options = Options(
             xlabel=None,
             ylabel=None,
             xlim=None,
             ylim=None,
             xval_unit=None,
             yval_unit=None,
             xval_unit_scale=True,
             yval_unit_scale=True,
+            xscale=None,
+            yscale=None,
+            sharex=True,
+            sharey=True,
             figure_title=None,
             series_params={},
         )
+        options.set_validator("xscale", ["linear", "log", "symlog", "logit", "quadratic", None])
+        options.set_validator("yscale", ["linear", "log", "symlog", "logit", "quadratic", None])
+
+        return options
 
     def set_options(self, **fields):
         """Set the plotter options.
 
         Args:
             fields: The fields to update in options.
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/visualization/plotters/curve_plotter.py` & `qiskit-experiments-0.6.0/qiskit_experiments/visualization/plotters/curve_plotter.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/visualization/plotters/iq_plotter.py` & `qiskit-experiments-0.6.0/qiskit_experiments/visualization/plotters/iq_plotter.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/visualization/style.py` & `qiskit-experiments-0.6.0/qiskit_experiments/visualization/style.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments/visualization/utils.py` & `qiskit-experiments-0.6.0/qiskit_experiments/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments.egg-info/PKG-INFO` & `qiskit-experiments-0.6.0/qiskit_experiments.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 Metadata-Version: 2.1
 Name: qiskit-experiments
-Version: 0.5.4
+Version: 0.6.0
 Summary: Software for developing quantum computing programs
-Home-page: https://github.com/Qiskit/qiskit-experiments
+Home-page: https://github.com/Qiskit-Extensions/qiskit-experiments
 Author: Qiskit Development Team
-Author-email: hello@qiskit.org
+Author-email: qiskit@us.ibm.com
 License: Apache 2.0
-Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-experiments/issues
-Project-URL: Documentation, https://qiskit.org/documentation/
-Project-URL: Source Code, https://github.com/Qiskit/qiskit-experiments
+Project-URL: Bug Tracker, https://github.com/Qiskit-Extensions/qiskit-experiments/issues
+Project-URL: Documentation, https://qiskit-extensions.github.io/qiskit-experiments
+Project-URL: Source Code, https://github.com/Qiskit-Extensions/qiskit-experiments
 Description: # Qiskit Experiments
         
-        [![License](https://img.shields.io/github/license/Qiskit/qiskit-experiments.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)
+        [![License](https://img.shields.io/github/license/Qiskit-Extensions/qiskit-experiments.svg)](https://opensource.org/licenses/Apache-2.0)
+        [![Release](https://img.shields.io/github/release/Qiskit-Extensions/qiskit-experiments.svg)](https://github.com/Qiskit-Extensions/qiskit-experiments/releases)
+        ![Python](https://img.shields.io/pypi/pyversions/qiskit-experiments.svg)
+        [![DOI](https://joss.theoj.org/papers/10.21105/joss.05329/status.svg)](https://doi.org/10.21105/joss.05329)
         
         **Qiskit Experiments** is a repository that builds tools for building, running,
         and analyzing experiments on noisy quantum computers using Qiskit.
         
         To learn more about the package, you can see the 
-        [most up-to-date documentation](https://qiskit.org/documentation/experiments/dev/) 
+        [most up-to-date documentation](https://qiskit-extensions.github.io/qiskit-experiments/dev)
         corresponding to the main branch of this repository or the 
-        [documentation for the latest stable release](https://qiskit.org/documentation/experiments).
+        [documentation for the latest stable release](https://qiskit-extensions.github.io/qiskit-experiments).
         
         ## Contribution Guidelines
         
         If you'd like to contribute to Qiskit Experiments, please take a look at our
         [contribution guidelines](CONTRIBUTING.md). This project adheres to Qiskit's
         [code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to
         uphold this code.
         
-        We use [GitHub issues](https://github.com/Qiskit/qiskit-experiments/issues) for
+        We use [GitHub issues](https://github.com/Qiskit-Extensions/qiskit-experiments/issues) for
         tracking requests and bugs. Please
         [join the Qiskit Slack community](https://qisk.it/join-slack)
         and use the [#experiments](https://qiskit.slack.com/archives/CGZDF48EN) channel for discussion and
         simple questions.
         For questions that are more suited for a forum we use the Qiskit tag in 
         [Stack Exchange](https://quantumcomputing.stackexchange.com/questions/tagged/qiskit).
         
         ## Authors and Citation
         
-        Qiskit Experiments is the work of [many people](https://github.com/Qiskit/qiskit-experiments/graphs/contributors) who contribute
-        to the project at different levels. If you use Qiskit Experiments, please cite
-        the following references:
-        
-        - Qiskit, as per the [BibTeX file](https://github.com/Qiskit/qiskit-metapackage/blob/master/Qiskit.bib).
-        - Qiskit Experiments, as per the [DOI](https://doi.org/10.5281/zenodo.7737483).
+        Qiskit Experiments is the work of [many people](https://github.com/Qiskit-Extensions/qiskit-experiments/graphs/contributors) who contribute
+        to the project at different levels. If you use Qiskit Experiments, please cite our
+        [paper](https://doi.org/10.21105/joss.05329) as per the included [citation file](CITATION.cff).
         
         ## License
         
         [Apache License 2.0](LICENSE.txt)
         
         
 Keywords: qiskit sdk quantum
@@ -56,15 +56,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: extras
```

### Comparing `qiskit-experiments-0.5.4/qiskit_experiments.egg-info/SOURCES.txt` & `qiskit-experiments-0.6.0/qiskit_experiments.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
+requirements-extras.txt
 requirements.txt
 setup.py
 qiskit_experiments/VERSION.txt
 qiskit_experiments/__init__.py
 qiskit_experiments/exceptions.py
 qiskit_experiments/version.py
 qiskit_experiments/warnings.py
 qiskit_experiments.egg-info/PKG-INFO
 qiskit_experiments.egg-info/SOURCES.txt
 qiskit_experiments.egg-info/dependency_links.txt
+qiskit_experiments.egg-info/entry_points.txt
 qiskit_experiments.egg-info/not-zip-safe
 qiskit_experiments.egg-info/requires.txt
 qiskit_experiments.egg-info/top_level.txt
 qiskit_experiments/calibration_management/__init__.py
 qiskit_experiments/calibration_management/base_calibration_experiment.py
 qiskit_experiments/calibration_management/basis_gate_library.py
 qiskit_experiments/calibration_management/calibration_key_types.py
 qiskit_experiments/calibration_management/calibration_utils.py
 qiskit_experiments/calibration_management/calibrations.py
 qiskit_experiments/calibration_management/control_channel_map.py
 qiskit_experiments/calibration_management/parameter_value.py
+qiskit_experiments/calibration_management/save_utils.py
 qiskit_experiments/calibration_management/update_library.py
 qiskit_experiments/curve_analysis/__init__.py
 qiskit_experiments/curve_analysis/base_curve_analysis.py
 qiskit_experiments/curve_analysis/composite_curve_analysis.py
 qiskit_experiments/curve_analysis/curve_analysis.py
 qiskit_experiments/curve_analysis/curve_data.py
 qiskit_experiments/curve_analysis/curve_fit.py
 qiskit_experiments/curve_analysis/fit_function.py
 qiskit_experiments/curve_analysis/guess.py
+qiskit_experiments/curve_analysis/scatter_table.py
 qiskit_experiments/curve_analysis/utils.py
 qiskit_experiments/curve_analysis/standard_analysis/__init__.py
 qiskit_experiments/curve_analysis/standard_analysis/bloch_trajectory.py
 qiskit_experiments/curve_analysis/standard_analysis/decay.py
 qiskit_experiments/curve_analysis/standard_analysis/error_amplification_analysis.py
 qiskit_experiments/curve_analysis/standard_analysis/gaussian.py
 qiskit_experiments/curve_analysis/standard_analysis/oscillation.py
@@ -57,29 +61,35 @@
 qiskit_experiments/database_service/__init__.py
 qiskit_experiments/database_service/device_component.py
 qiskit_experiments/database_service/exceptions.py
 qiskit_experiments/database_service/utils.py
 qiskit_experiments/framework/__init__.py
 qiskit_experiments/framework/analysis_result.py
 qiskit_experiments/framework/analysis_result_data.py
+qiskit_experiments/framework/analysis_result_table.py
 qiskit_experiments/framework/backend_data.py
 qiskit_experiments/framework/backend_timing.py
 qiskit_experiments/framework/base_analysis.py
 qiskit_experiments/framework/base_experiment.py
 qiskit_experiments/framework/configs.py
 qiskit_experiments/framework/experiment_data.py
 qiskit_experiments/framework/json.py
 qiskit_experiments/framework/matplotlib.py
+qiskit_experiments/framework/package_deps.py
 qiskit_experiments/framework/restless_mixin.py
+qiskit_experiments/framework/status.py
 qiskit_experiments/framework/store_init_args.py
 qiskit_experiments/framework/composite/__init__.py
 qiskit_experiments/framework/composite/batch_experiment.py
 qiskit_experiments/framework/composite/composite_analysis.py
 qiskit_experiments/framework/composite/composite_experiment.py
 qiskit_experiments/framework/composite/parallel_experiment.py
+qiskit_experiments/framework/containers/__init__.py
+qiskit_experiments/framework/containers/artifact_data.py
+qiskit_experiments/framework/containers/figure_data.py
 qiskit_experiments/library/__init__.py
 qiskit_experiments/library/calibration/__init__.py
 qiskit_experiments/library/calibration/fine_amplitude.py
 qiskit_experiments/library/calibration/fine_drag_cal.py
 qiskit_experiments/library/calibration/fine_frequency_cal.py
 qiskit_experiments/library/calibration/frequency_cal.py
 qiskit_experiments/library/calibration/half_angle_cal.py
@@ -119,26 +129,34 @@
 qiskit_experiments/library/characterization/analysis/readout_angle_analysis.py
 qiskit_experiments/library/characterization/analysis/resonator_spectroscopy_analysis.py
 qiskit_experiments/library/characterization/analysis/t1_analysis.py
 qiskit_experiments/library/characterization/analysis/t2hahn_analysis.py
 qiskit_experiments/library/characterization/analysis/t2ramsey_analysis.py
 qiskit_experiments/library/characterization/analysis/tphi_analysis.py
 qiskit_experiments/library/characterization/analysis/zz_ramsey_analysis.py
+qiskit_experiments/library/driven_freq_tuning/__init__.py
+qiskit_experiments/library/driven_freq_tuning/coefficients.py
+qiskit_experiments/library/driven_freq_tuning/p1_spect.py
+qiskit_experiments/library/driven_freq_tuning/p1_spect_analysis.py
+qiskit_experiments/library/driven_freq_tuning/ramsey.py
+qiskit_experiments/library/driven_freq_tuning/ramsey_amp_scan.py
+qiskit_experiments/library/driven_freq_tuning/ramsey_amp_scan_analysis.py
 qiskit_experiments/library/quantum_volume/__init__.py
 qiskit_experiments/library/quantum_volume/qv_analysis.py
 qiskit_experiments/library/quantum_volume/qv_experiment.py
 qiskit_experiments/library/randomized_benchmarking/__init__.py
+qiskit_experiments/library/randomized_benchmarking/clifford_synthesis.py
 qiskit_experiments/library/randomized_benchmarking/clifford_utils.py
 qiskit_experiments/library/randomized_benchmarking/interleaved_rb_analysis.py
 qiskit_experiments/library/randomized_benchmarking/interleaved_rb_experiment.py
 qiskit_experiments/library/randomized_benchmarking/rb_analysis.py
 qiskit_experiments/library/randomized_benchmarking/rb_utils.py
 qiskit_experiments/library/randomized_benchmarking/standard_rb.py
 qiskit_experiments/library/randomized_benchmarking/data/clifford_compose_1q.npz
-qiskit_experiments/library/randomized_benchmarking/data/clifford_compose_2q_sparse.npz
+qiskit_experiments/library/randomized_benchmarking/data/clifford_compose_2q_dense_selected.npz
 qiskit_experiments/library/randomized_benchmarking/data/clifford_inverse_1q.npz
 qiskit_experiments/library/randomized_benchmarking/data/clifford_inverse_2q.npz
 qiskit_experiments/library/tomography/__init__.py
 qiskit_experiments/library/tomography/mit_qpt_experiment.py
 qiskit_experiments/library/tomography/mit_qst_experiment.py
 qiskit_experiments/library/tomography/mit_tomography_analysis.py
 qiskit_experiments/library/tomography/qpt_analysis.py
@@ -155,15 +173,14 @@
 qiskit_experiments/library/tomography/fitters/__init__.py
 qiskit_experiments/library/tomography/fitters/cvxpy_lstsq.py
 qiskit_experiments/library/tomography/fitters/cvxpy_utils.py
 qiskit_experiments/library/tomography/fitters/fitter_data.py
 qiskit_experiments/library/tomography/fitters/lininv.py
 qiskit_experiments/library/tomography/fitters/lstsq_utils.py
 qiskit_experiments/library/tomography/fitters/postprocess_fit.py
-qiskit_experiments/library/tomography/fitters/scipy_lstsq.py
 qiskit_experiments/test/__init__.py
 qiskit_experiments/test/fake_backend.py
 qiskit_experiments/test/fake_service.py
 qiskit_experiments/test/mock_iq_backend.py
 qiskit_experiments/test/mock_iq_helpers.py
 qiskit_experiments/test/noisy_delay_aer_simulator.py
 qiskit_experiments/test/pulse_backend.py
@@ -175,8 +192,9 @@
 qiskit_experiments/visualization/drawers/__init__.py
 qiskit_experiments/visualization/drawers/base_drawer.py
 qiskit_experiments/visualization/drawers/legacy_curve_compat_drawer.py
 qiskit_experiments/visualization/drawers/mpl_drawer.py
 qiskit_experiments/visualization/plotters/__init__.py
 qiskit_experiments/visualization/plotters/base_plotter.py
 qiskit_experiments/visualization/plotters/curve_plotter.py
-qiskit_experiments/visualization/plotters/iq_plotter.py
+qiskit_experiments/visualization/plotters/iq_plotter.py
+test/test_base.py
```

### Comparing `qiskit-experiments-0.5.4/setup.py` & `qiskit-experiments-0.6.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 import os
 from setuptools import setup, find_packages
 
 with open("requirements.txt", encoding="utf-8") as f:
     REQUIREMENTS = f.read().splitlines()
 
+with open("requirements-extras.txt", encoding="utf-8") as f:
+    EXTRAS = f.read().splitlines()
 
 version_path = os.path.abspath(
     os.path.join(os.path.join(os.path.dirname(__file__), "qiskit_experiments"), "VERSION.txt")
 )
 with open(version_path, "r", encoding="utf-8") as fd:
     version = fd.read().rstrip()
 
@@ -32,39 +34,45 @@
 
 setup(
     name="qiskit-experiments",
     version=version,
     description="Software for developing quantum computing programs",
     long_description=README,
     long_description_content_type="text/markdown",
-    url="https://github.com/Qiskit/qiskit-experiments",
+    url="https://github.com/Qiskit-Extensions/qiskit-experiments",
     author="Qiskit Development Team",
-    author_email="hello@qiskit.org",
+    author_email="qiskit@us.ibm.com",
     license="Apache 2.0",
     classifiers=[
         "Environment :: Console",
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Scientific/Engineering",
     ],
     keywords="qiskit sdk quantum",
     packages=find_packages(exclude=["test*"]),
     install_requires=REQUIREMENTS,
+    extras_require={"extras": EXTRAS},
     include_package_data=True,
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
-        "Bug Tracker": "https://github.com/Qiskit/qiskit-experiments/issues",
-        "Documentation": "https://qiskit.org/documentation/",
-        "Source Code": "https://github.com/Qiskit/qiskit-experiments",
+        "Bug Tracker": "https://github.com/Qiskit-Extensions/qiskit-experiments/issues",
+        "Documentation": "https://qiskit-extensions.github.io/qiskit-experiments",
+        "Source Code": "https://github.com/Qiskit-Extensions/qiskit-experiments",
     },
     zip_safe=False,
+    entry_points={
+        "qiskit.synthesis": [
+            "clifford.rb_default = qiskit_experiments.library.randomized_benchmarking.clifford_synthesis:RBDefaultCliffordSynthesis",
+        ],
+    },
 )
```

