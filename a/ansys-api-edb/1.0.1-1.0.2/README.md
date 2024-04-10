# Comparing `tmp/ansys-api-edb-1.0.1.tar.gz` & `tmp/ansys-api-edb-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-edb-1.0.1.tar", last modified: Thu Mar 28 20:24:39 2024, max compression
+gzip compressed data, was "ansys-api-edb-1.0.2.tar", last modified: Wed Apr 10 15:42:19 2024, max compression
```

## Comparing `ansys-api-edb-1.0.1.tar` & `ansys-api-edb-1.0.2.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:24:39.609306 ansys-api-edb-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-28 20:24:39.609306 ansys-api-edb-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:24:39.589306 ansys-api-edb-1.0.1/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:24:39.589306 ansys-api-edb-1.0.1/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:24:39.589306 ansys-api-edb-1.0.1/ansys/api/edb/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:24:39.609306 ansys-api-edb-1.0.1/ansys/api/edb/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/arc_data.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/board_bend_def.proto
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/bondwire.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/bondwire_def.proto
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/bundle_term.proto
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/cell.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/cell_instance.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/circle.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/component_def.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/component_group.proto
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/component_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/component_pin.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/component_property.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/connectable.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/database.proto
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/dataset_def.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/debye_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/definition_obj.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/die_property.proto
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/dielectric_material_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/differential_pair.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/djordjecvic_sarkar_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/edb_defs.proto
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/edb_messages.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/edge_term.proto
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/extended_net.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/group.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/hfss_simulation_settings.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/hfss_simulation_setup.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/hierarchy_obj.proto
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/ic_component_property.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/inst_array.proto
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/io_component_property.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/layer.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/layer_collection.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/layer_map.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/layout.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/layout_instance.proto
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/layout_instance_context.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/layout_obj.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/layout_obj_instance.proto
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/layout_obj_instance_2d_geometry.proto
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/layout_obj_instance_3d_geometry.proto
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/layout_obj_instance_geometry.proto
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/material_def.proto
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/material_property_thermal_modifier.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/mcad_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/model.proto
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/multipole_debye_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/net.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/netclass.proto
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/netlist_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/package_def.proto
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/padstack_def.proto
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/padstack_def_data.proto
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/padstack_inst_term.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/padstack_instance.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/path.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/pin_group.proto
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/pin_group_term.proto
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/pin_pair_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/point_3d_data.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/point_data.proto
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/point_term.proto
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/polygon.proto
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/polygon_data.proto
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/port_post_processing_prop.proto
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/port_property.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/primitive.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/r_tree.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/raptor_x_simulation_settings.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/rectangle.proto
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/refs.proto
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/rlc.proto
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/rlc_component_property.proto
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/simulation_settings.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/simulation_setup.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/siwave_dcir_simulation_settings.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8850 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/siwave_simulation_settings.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/solder_ball_property.proto
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/sparameter_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/spice_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/stackup_layer.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/structure3d.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/term.proto
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/term_inst.proto
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/term_inst_term.proto
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/text.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/transform.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/transform3d.proto
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/value.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/variable_server.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/via_group.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/via_layer.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/ansys/api/edb/v1/voltage_regulator.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:24:39.609306 ansys-api-edb-1.0.1/ansys_api_edb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-28 20:24:39.000000 ansys-api-edb-1.0.1/ansys_api_edb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-03-28 20:24:39.000000 ansys-api-edb-1.0.1/ansys_api_edb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 20:24:39.000000 ansys-api-edb-1.0.1/ansys_api_edb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-28 20:24:39.000000 ansys-api-edb-1.0.1/ansys_api_edb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-28 20:24:39.000000 ansys-api-edb-1.0.1/ansys_api_edb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 20:24:39.000000 ansys-api-edb-1.0.1/ansys_api_edb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 20:24:39.609306 ansys-api-edb-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-03-28 20:24:30.000000 ansys-api-edb-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:42:19.131120 ansys-api-edb-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-10 15:42:19.131120 ansys-api-edb-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:42:19.111120 ansys-api-edb-1.0.2/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:42:19.111120 ansys-api-edb-1.0.2/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:42:19.111120 ansys-api-edb-1.0.2/ansys/api/edb/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:42:19.127120 ansys-api-edb-1.0.2/ansys/api/edb/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/arc_data.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/board_bend_def.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/bondwire.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/bondwire_def.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/bundle_term.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/cell.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/cell_instance.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/circle.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/component_def.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/component_group.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/component_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/component_pin.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/component_property.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/connectable.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/database.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/dataset_def.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/debye_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/definition_obj.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/die_property.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/dielectric_material_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/differential_pair.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/djordjecvic_sarkar_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/edb_defs.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/edb_messages.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/edge_term.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/extended_net.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/group.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/hfss_simulation_settings.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/hfss_simulation_setup.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/hierarchy_obj.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/ic_component_property.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/inst_array.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/io_component_property.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/layer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/layer_collection.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/layer_map.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/layout.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/layout_instance.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/layout_instance_context.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/layout_obj.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/layout_obj_instance.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/layout_obj_instance_2d_geometry.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/layout_obj_instance_3d_geometry.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/layout_obj_instance_geometry.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/material_def.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/material_property_thermal_modifier.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/mcad_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/multipole_debye_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/net.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/netclass.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/netlist_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/package_def.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/padstack_def.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/padstack_def_data.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/padstack_inst_term.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/padstack_instance.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/path.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/pin_group.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/pin_group_term.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/pin_pair_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/point_3d_data.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/point_data.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/point_term.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/polygon.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/polygon_data.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/port_post_processing_prop.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/port_property.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/primitive.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/r_tree.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/raptor_x_simulation_settings.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/rectangle.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/refs.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/rlc.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/rlc_component_property.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/simulation_settings.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/simulation_setup.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/siwave_dcir_simulation_settings.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8850 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/siwave_simulation_settings.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/solder_ball_property.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/sparameter_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/spice_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/stackup_layer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/structure3d.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/term.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/term_inst.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/term_inst_term.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/text.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/transform.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/transform3d.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/value.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/variable_server.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/via_group.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/via_layer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/ansys/api/edb/v1/voltage_regulator.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:42:19.127120 ansys-api-edb-1.0.2/ansys_api_edb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-10 15:42:19.000000 ansys-api-edb-1.0.2/ansys_api_edb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-10 15:42:19.000000 ansys-api-edb-1.0.2/ansys_api_edb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 15:42:19.000000 ansys-api-edb-1.0.2/ansys_api_edb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-10 15:42:19.000000 ansys-api-edb-1.0.2/ansys_api_edb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 15:42:19.000000 ansys-api-edb-1.0.2/ansys_api_edb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 15:42:19.000000 ansys-api-edb-1.0.2/ansys_api_edb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 15:42:19.131120 ansys-api-edb-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-10 15:42:10.000000 ansys-api-edb-1.0.2/setup.py
```

### Comparing `ansys-api-edb-1.0.1/LICENCE` & `ansys-api-edb-1.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/PKG-INFO` & `ansys-api-edb-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-edb
-Version: 1.0.1
-Summary: Autogenerated Python gRPC interface package for ansys-api-edb, built on 20:24:39 on 28 March 2024
+Version: 1.0.2
+Summary: Autogenerated Python gRPC interface package for ansys-api-edb, built on 15:42:19 on 10 April 2024
 Home-page: https://github.com/ansys/ansys-api-edb
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Project-URL: Documentation, https://github.com/ansys/ansys-api-edb/#readme
```

### Comparing `ansys-api-edb-1.0.1/README.md` & `ansys-api-edb-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/arc_data.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/arc_data.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/board_bend_def.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/board_bend_def.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/bondwire.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/bondwire.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/bondwire_def.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/bondwire_def.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/cell.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/cell.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/cell_instance.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/cell_instance.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/circle.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/circle.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/component_def.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/component_def.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/component_group.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/component_group.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/component_model.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/component_model.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/component_pin.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/component_pin.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/component_property.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/component_property.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/connectable.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/connectable.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/database.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/database.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/dataset_def.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/dataset_def.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/debye_model.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/debye_model.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/die_property.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/die_property.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/differential_pair.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/differential_pair.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/djordjecvic_sarkar_model.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/djordjecvic_sarkar_model.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/edb_defs.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/edb_defs.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/edb_messages.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/edb_messages.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/edge_term.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/edge_term.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/extended_net.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/extended_net.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/group.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/group.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/hfss_simulation_settings.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/hfss_simulation_settings.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/hfss_simulation_setup.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/hfss_simulation_setup.proto`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
   bool refine_inside = 3;
   string mesh_region = 4;
   repeated MeshOpNetLayerInfoMessage net_layer_info = 5;
   oneof mesh_operation_sub_type {
     SkinDepthMeshOperationMessage skin_depth_mesh_op = 6;
     LengthMeshOperationMessage length_mesh_op = 7;
   }
+  bool solve_inside = 8;
 }
 
 message MeshOperationsMessage {
   repeated MeshOperationMessage mesh_ops = 1;
 }
 
 message MeshOperationsPropertyMessage {
```

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/hierarchy_obj.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/hierarchy_obj.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/ic_component_property.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/ic_component_property.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/inst_array.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/inst_array.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/io_component_property.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/io_component_property.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/layer.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/layer.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/layer_collection.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/layer_collection.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/layer_map.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/layer_map.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/layout.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/layout.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/layout_instance.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/layout_instance.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/layout_instance_context.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/layout_instance_context.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/layout_obj.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/layout_obj.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/layout_obj_instance.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/layout_obj_instance.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/layout_obj_instance_2d_geometry.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/layout_obj_instance_2d_geometry.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/layout_obj_instance_3d_geometry.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/layout_obj_instance_3d_geometry.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/layout_obj_instance_geometry.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/layout_obj_instance_geometry.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/material_def.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/material_def.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/material_property_thermal_modifier.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/material_property_thermal_modifier.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/mcad_model.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/mcad_model.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/multipole_debye_model.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/multipole_debye_model.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/net.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/net.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/netclass.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/netclass.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/package_def.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/package_def.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/padstack_def.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/padstack_def.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/padstack_def_data.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/padstack_def_data.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/padstack_inst_term.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/padstack_inst_term.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/padstack_instance.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/padstack_instance.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/path.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/path.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/pin_group.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/pin_group.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/pin_group_term.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/pin_group_term.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/pin_pair_model.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/pin_pair_model.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/point_3d_data.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/point_3d_data.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/point_data.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/point_data.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/point_term.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/point_term.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/polygon.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/polygon.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/polygon_data.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/polygon_data.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/port_property.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/port_property.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/primitive.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/primitive.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/r_tree.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/r_tree.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/raptor_x_simulation_settings.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/raptor_x_simulation_settings.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/rectangle.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/rectangle.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/refs.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/refs.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/rlc_component_property.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/rlc_component_property.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/simulation_settings.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/simulation_settings.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/simulation_setup.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/simulation_setup.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/siwave_dcir_simulation_settings.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/siwave_dcir_simulation_settings.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/siwave_simulation_settings.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/siwave_simulation_settings.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/solder_ball_property.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/solder_ball_property.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/sparameter_model.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/sparameter_model.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/spice_model.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/spice_model.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/stackup_layer.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/stackup_layer.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/structure3d.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/structure3d.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/term.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/term.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/term_inst.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/term_inst.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/term_inst_term.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/term_inst_term.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/text.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/text.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/transform.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/transform.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/transform3d.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/transform3d.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/variable_server.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/variable_server.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/via_group.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/via_group.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/via_layer.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/via_layer.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys/api/edb/v1/voltage_regulator.proto` & `ansys-api-edb-1.0.2/ansys/api/edb/v1/voltage_regulator.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/ansys_api_edb.egg-info/PKG-INFO` & `ansys-api-edb-1.0.2/ansys_api_edb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-edb
-Version: 1.0.1
-Summary: Autogenerated Python gRPC interface package for ansys-api-edb, built on 20:24:39 on 28 March 2024
+Version: 1.0.2
+Summary: Autogenerated Python gRPC interface package for ansys-api-edb, built on 15:42:19 on 10 April 2024
 Home-page: https://github.com/ansys/ansys-api-edb
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Project-URL: Documentation, https://github.com/ansys/ansys-api-edb/#readme
```

### Comparing `ansys-api-edb-1.0.1/ansys_api_edb.egg-info/SOURCES.txt` & `ansys-api-edb-1.0.2/ansys_api_edb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansys-api-edb-1.0.1/setup.py` & `ansys-api-edb-1.0.2/setup.py`

 * *Files identical despite different names*
