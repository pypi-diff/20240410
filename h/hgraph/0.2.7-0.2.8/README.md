# Comparing `tmp/hgraph-0.2.7.tar.gz` & `tmp/hgraph-0.2.8.tar.gz`

## Comparing `hgraph-0.2.7.tar` & `hgraph-0.2.8.tar`

### file list

```diff
@@ -1,276 +1,291 @@
--rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 hgraph-0.2.7/CHANGELOG.md
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 hgraph-0.2.7/ROADMAP.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 hgraph-0.2.7/.github/dependabot.yml
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 hgraph-0.2.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 hgraph-0.2.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 hgraph-0.2.7/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/index.md
--rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/evaluation_clock_uml.png
--rw-r--r--   0        0        0    15820 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/evaluation_engine_api.png
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/forward_propagation_graph.md
--rw-r--r--   0        0        0     8774 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/graph_executor_uml.png
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/graph_runtime.md
--rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/graph_uml.png
--rw-r--r--   0        0        0    10793 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/node_uml.png
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/run_mode_uml.png
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/services.md
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/src_cmpt_snk_diagram.png
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/python/component_signature.md
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/python/hg_types.md
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/python/node_signature.md
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/python/program_anatomy.md
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/python/schema_based_types.md
--rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/python/what_is_1_1.png
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/exception_handling.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/exception_handling.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/feedback.md
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/feedback.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/generics.md
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/generics.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/graphs_and_nodes.md
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/graphs_and_nodes.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/hello_world.md
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/hello_world.py
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/injectable_attributes.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/injectable_attributes.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/life_cycle.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/life_cycle.py
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/map_reduce_switch.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/map_reduce_switch.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/node_testing.md
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/node_testing.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/push_source_node.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/push_source_node.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/quick_start.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/examples/monitoring/__init__.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 hgraph-0.2.7/examples/monitoring/monitoring.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/examples/monitoring/phase_1/__init__.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 hgraph-0.2.7/examples/monitoring/phase_1/monitoring_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/examples/web_api/__init__.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 hgraph-0.2.7/examples/web_api/web_api.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/__about__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_builder/__init__.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_builder/_builder.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_builder/_graph_builder.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_builder/_input_builder.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_builder/_node_builder.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_builder/_output_builder.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_builder/_scalar_builder.py
--rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_builder/_ts_builder.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/__init__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_impl_configuration.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/graph_construction.md
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/__init__.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_graph_builder.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_map_builder.py
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_node_builder.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_node_impl_builder.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_reduce_builder.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_service_impl_builder.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_switch_builder.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_try_except_builder.py
--rw-r--r--   0        0        0    13563 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_ts_builder.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_common.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_data_writer.py
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_evaluation_clock.py
--rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_evaluation_engine.py
--rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_graph.py
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_graph_executor.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_graph_recorder.py
--rw-r--r--   0        0        0     7503 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_map_node.py
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_nested_evaluation_engine.py
--rw-r--r--   0        0        0    18657 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_node.py
--rw-r--r--   0        0        0    11241 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_reduce_node.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_service_node_impl.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_switch_node.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_try_except_node.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_feature_extension.py
--rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_input.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_output.py
--rw-r--r--   0        0        0     8823 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_ref.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_scalar_value.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_signal.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_ts.py
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_tsb.py
--rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_tsd.py
--rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_tsl.py
--rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_tss.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_constants.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_data_writer.py
--rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_evaluation_clock.py
--rw-r--r--   0        0        0    13773 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_evaluation_engine.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_feedback.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_global_state.py
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_graph.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_graph_executor.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_graph_recorder.py
--rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_graph_runner.py
--rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_lifecycle.py
--rw-r--r--   0        0        0    13113 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_node.py
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_operators.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/__init__.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_error_type.py
--rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_frame_scalar_type_meta_data.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_ref_meta_data.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_ref_type.py
--rw-r--r--   0        0        0    35935 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_scalar_type_meta_data.py
--rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_scalar_types.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_scalar_value.py
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_schema_type.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_time_series_meta_data.py
--rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_time_series_types.py
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_ts_meta_data.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_ts_signal_meta_data.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_ts_type.py
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_ts_type_var_meta_data.py
--rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_tsb_meta_data.py
--rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_tsb_type.py
--rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_tsd_meta_data.py
--rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_tsd_type.py
--rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_tsl_meta_data.py
--rw-r--r--   0        0        0     7690 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_tsl_type.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_tss_meta_data.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_tss_type.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_type_meta_data.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_typing_utils.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/__init__.py
--rw-r--r--   0        0        0    19268 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_decorators.py
--rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_dispatch.py
--rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_exception_handling.py
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_graph_builder.py
--rw-r--r--   0        0        0    28010 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_map.py
--rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_reduce.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_source_code_details.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_stub_wiring_node.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_switch.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_context.py
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_errors.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_instance.py
--rw-r--r--   0        0        0    16810 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_signature.py
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_port.py
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_utils.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/__init__.py
--rw-r--r--   0        0        0    12168 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_graph_wiring_node_class.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_map_wiring_node.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_node_impl_wiring_node_class.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_pull_source_node_class.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_python_wiring_node_classes.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_reduce_wiring_node.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_reference_service_node_class.py
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_req_repl_service_node_service.py
--rw-r--r--   0        0        0    15633 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_service_impl_node_class.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_service_interface_node_class.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_stub_wiring_node_class.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_subscription_service_node_service.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_switch_wiring_node.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_try_except_wiring_node.py
--rw-r--r--   0        0        0    26970 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_wiring_node_class.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/__init__.py
--rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_analytical.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_compound_scalar_operators.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_conditional.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_const.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_data_source_polars.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_datetime_operators.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_drop_dups.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_format.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_frame_operators.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_graph.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_logical.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_math.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_null_sink.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_numpy.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_operators.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_pass_through.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_print.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_record.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_replay.py
--rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_service_utils.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_set_operators.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_stream_operators.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_tsb_operators.py
--rw-r--r--   0        0        0    14011 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_tsd_operators.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_tsl_operators.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_tss_operators.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_tuple_operators.py
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_window_operators.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/test/__init__.py
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/test/_node_printer.py
--rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/test/_node_unit_tester.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/test/testing.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/__init__.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/test_wiring.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_impl/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_impl/_builder/__init__.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_impl/_builder/test_graph_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_impl/_runtime/__init__.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_impl/_runtime/test_graph_runner.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_impl/_runtime/test_node_impl.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_impl/_runtime/test_record_replay.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_runtime/__init__.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_runtime/test_feedback.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_runtime/test_scheduler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_types/__init__.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_types/test_complex_types.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_types/test_operator_rank.py
--rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_types/test_type_meta_data.py
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_types/test_type_meta_resolve.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/__init__.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_auto_const.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_auto_resolve.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_de_dupping_of_nodes.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_decorators.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_dispatch.py
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_error_handling.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_generic_graphs.py
--rw-r--r--   0        0        0    14626 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_map.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_overloads.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_ref.py
--rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_service.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_switch.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_ts_wiring.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_tsb_wiring.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_tsd_wiring.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_tsl_wiring.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_tss.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_wiring_node_signature.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/__init__.py
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_analytical.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_compound_scalar_operators.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_conditional.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_const.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_data_source_polars.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_drop_dups.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_format.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_frame.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_logical.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_math.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_numpy.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_operators.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_print.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_push_queue.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_recorder.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_replay.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_stream_operators.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_tsb_operators.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_tsd_operators.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_tsl_operators.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_tss_operators.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_window_operators.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_wp_operators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/test/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/test/test_eval_node.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/test/test_node_printer.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 hgraph-0.2.7/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hgraph-0.2.7/LICENSE
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 hgraph-0.2.7/README.md
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 hgraph-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 hgraph-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     8113 2020-02-02 00:00:00.000000 hgraph-0.2.8/CHANGELOG.md
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 hgraph-0.2.8/ROADMAP.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 hgraph-0.2.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 hgraph-0.2.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 hgraph-0.2.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 hgraph-0.2.8/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/index.md
+-rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/evaluation_clock_uml.png
+-rw-r--r--   0        0        0    15820 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/evaluation_engine_api.png
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/forward_propagation_graph.md
+-rw-r--r--   0        0        0     8774 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/graph_executor_uml.png
+-rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/graph_runtime.md
+-rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/graph_uml.png
+-rw-r--r--   0        0        0    10793 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/node_uml.png
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/run_mode_uml.png
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/services.md
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/src_cmpt_snk_diagram.png
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/python/component_signature.md
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/python/hg_types.md
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/python/node_signature.md
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/python/program_anatomy.md
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/python/schema_based_types.md
+-rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/python/what_is_1_1.png
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/exception_handling.md
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/exception_handling.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/feedback.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/feedback.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/generics.md
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/generics.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/graphs_and_nodes.md
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/graphs_and_nodes.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/hello_world.md
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/hello_world.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/injectable_attributes.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/injectable_attributes.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/life_cycle.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/life_cycle.py
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/map_reduce_switch.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/map_reduce_switch.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/node_testing.md
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/node_testing.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/push_source_node.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/push_source_node.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/quick_start.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/monitoring/__init__.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/monitoring/monitoring.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/monitoring/phase_1/__init__.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/monitoring/phase_1/monitoring_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/notebook/__init__.py
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/notebook/example_book.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/web_api/__init__.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/web_api/web_api.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/web_ui/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/web_ui/__init__.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/web_ui/web_ui.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/__about__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_builder/__init__.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_builder/_builder.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_builder/_graph_builder.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_builder/_input_builder.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_builder/_node_builder.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_builder/_output_builder.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_builder/_scalar_builder.py
+-rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_builder/_ts_builder.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/__init__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_impl_configuration.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/graph_construction.md
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/__init__.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_graph_builder.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_map_builder.py
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_node_builder.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_node_impl_builder.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_reduce_builder.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_service_impl_builder.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_switch_builder.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_try_except_builder.py
+-rw-r--r--   0        0        0    13563 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_ts_builder.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_common.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_data_writer.py
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_evaluation_clock.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_evaluation_engine.py
+-rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_graph.py
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_graph_executor.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_graph_recorder.py
+-rw-r--r--   0        0        0     7503 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_map_node.py
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_nested_evaluation_engine.py
+-rw-r--r--   0        0        0    18657 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_node.py
+-rw-r--r--   0        0        0    11241 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_reduce_node.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_service_node_impl.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_switch_node.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_try_except_node.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_feature_extension.py
+-rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_input.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_output.py
+-rw-r--r--   0        0        0     8823 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_ref.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_scalar_value.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_signal.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_ts.py
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_tsb.py
+-rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_tsd.py
+-rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_tsl.py
+-rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_tss.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_constants.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_data_writer.py
+-rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_evaluation_clock.py
+-rw-r--r--   0        0        0    13773 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_evaluation_engine.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_feedback.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_global_state.py
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_graph.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_graph_executor.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_graph_recorder.py
+-rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_graph_runner.py
+-rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_lifecycle.py
+-rw-r--r--   0        0        0    13113 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_node.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_operators.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/__init__.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_error_type.py
+-rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_frame_scalar_type_meta_data.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_ref_meta_data.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_ref_type.py
+-rw-r--r--   0        0        0    35974 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_scalar_type_meta_data.py
+-rw-r--r--   0        0        0     8786 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_scalar_types.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_scalar_value.py
+-rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_schema_type.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_time_series_meta_data.py
+-rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_time_series_types.py
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_ts_meta_data.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_ts_signal_meta_data.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_ts_type.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_ts_type_var_meta_data.py
+-rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_tsb_meta_data.py
+-rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_tsb_type.py
+-rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_tsd_meta_data.py
+-rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_tsd_type.py
+-rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_tsl_meta_data.py
+-rw-r--r--   0        0        0     7690 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_tsl_type.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_tss_meta_data.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_tss_type.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_type_meta_data.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_typing_utils.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/__init__.py
+-rw-r--r--   0        0        0    20255 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_decorators.py
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_dispatch.py
+-rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_exception_handling.py
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_graph_builder.py
+-rw-r--r--   0        0        0    28010 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_map.py
+-rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_reduce.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_source_code_details.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_stub_wiring_node.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_switch.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_context.py
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_errors.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_instance.py
+-rw-r--r--   0        0        0    20628 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_signature.py
+-rw-r--r--   0        0        0    11410 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_port.py
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_utils.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/__init__.py
+-rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_graph_wiring_node_class.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_map_wiring_node.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_node_impl_wiring_node_class.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_pull_source_node_class.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_python_wiring_node_classes.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_reduce_wiring_node.py
+-rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_reference_service_node_class.py
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_req_repl_service_node_service.py
+-rw-r--r--   0        0        0    16410 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_service_impl_node_class.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_service_interface_node_class.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_stub_wiring_node_class.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_subscription_service_node_service.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_switch_wiring_node.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_try_except_wiring_node.py
+-rw-r--r--   0        0        0    24577 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_wiring_node_class.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/adaptors/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/adaptors/perspective/__init__.py
+-rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/adaptors/perspective/_perspective.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/adaptors/perspective/_perspetive_publish.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/adaptors/perspective/index_template.html
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/adaptors/perspective/table_template.html
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/adaptors/perspective/workspace_template.html
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/__init__.py
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_analytical.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_compound_scalar_operators.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_conditional.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_const.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_data_source_polars.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_datetime_operators.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_drop_dups.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_format.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_frame_operators.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_graph.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_logical.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_math.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_null_sink.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_numpy.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_operators.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_pass_through.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_print.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_record.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_replay.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_service_utils.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_set_operators.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_stream_operators.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_tsb_operators.py
+-rw-r--r--   0        0        0    14011 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_tsd_operators.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_tsl_operators.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_tss_operators.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_tuple_operators.py
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_window_operators.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/notebook/NoteBook.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/notebook/__init__.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/notebook/_notebook_graph.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/test/__init__.py
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/test/_node_printer.py
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/test/_node_unit_tester.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/test/testing.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/__init__.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/test_wiring.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_impl/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_impl/_builder/__init__.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_impl/_builder/test_graph_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_impl/_runtime/__init__.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_impl/_runtime/test_graph_runner.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_impl/_runtime/test_node_impl.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_impl/_runtime/test_record_replay.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_runtime/__init__.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_runtime/test_feedback.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_runtime/test_scheduler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_types/__init__.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_types/test_complex_types.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_types/test_operator_rank.py
+-rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_types/test_type_meta_data.py
+-rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_types/test_type_meta_resolve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/__init__.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_auto_const.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_auto_resolve.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_de_dupping_of_nodes.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_decorators.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_dispatch.py
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_error_handling.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_generic_graphs.py
+-rw-r--r--   0        0        0    14626 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_map.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_overloads.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_ref.py
+-rw-r--r--   0        0        0    11845 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_service.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_switch.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_ts_wiring.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_tsb_wiring.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_tsd_wiring.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_tsl_wiring.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_tss.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_wiring_node_signature.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/__init__.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_analytical.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_compound_scalar_operators.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_conditional.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_const.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_data_source_polars.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_drop_dups.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_format.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_frame.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_logical.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_math.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_numpy.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_operators.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_print.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_push_queue.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_recorder.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_replay.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_stream_operators.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_tsb_operators.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_tsd_operators.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_tsl_operators.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_tss_operators.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_window_operators.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_wp_operators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/test/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/test/test_eval_node.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/test/test_node_printer.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 hgraph-0.2.8/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hgraph-0.2.8/LICENSE
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 hgraph-0.2.8/README.md
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 hgraph-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 hgraph-0.2.8/PKG-INFO
```

### Comparing `hgraph-0.2.7/CHANGELOG.md` & `hgraph-0.2.8/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -277,7 +277,14 @@
 --------------------------
 
 * Add support for multi-service implementations
 * Support multiple inputs in a request-reply service
 * nested tsd merge
 * constraint type wiring improvements
 
+Version 0.2.8 (10-04-2024)
+--------------------------
+
+* Add initial notebook support
+* Add perspective adaptor
+* Add support for generic services
+
```

### Comparing `hgraph-0.2.7/ROADMAP.md` & `hgraph-0.2.8/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/.github/ISSUE_TEMPLATE/bug_report.md` & `hgraph-0.2.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/.github/ISSUE_TEMPLATE/feature_request.md` & `hgraph-0.2.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/index.md` & `hgraph-0.2.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/concepts/evaluation_clock_uml.png` & `hgraph-0.2.8/docs/concepts/evaluation_clock_uml.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/concepts/evaluation_engine_api.png` & `hgraph-0.2.8/docs/concepts/evaluation_engine_api.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/concepts/forward_propagation_graph.md` & `hgraph-0.2.8/docs/concepts/forward_propagation_graph.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/concepts/graph_executor_uml.png` & `hgraph-0.2.8/docs/concepts/graph_executor_uml.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/concepts/graph_runtime.md` & `hgraph-0.2.8/docs/concepts/graph_runtime.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/concepts/graph_uml.png` & `hgraph-0.2.8/docs/concepts/graph_uml.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/concepts/node_uml.png` & `hgraph-0.2.8/docs/concepts/node_uml.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/concepts/run_mode_uml.png` & `hgraph-0.2.8/docs/concepts/run_mode_uml.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/concepts/services.md` & `hgraph-0.2.8/docs/concepts/services.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/concepts/src_cmpt_snk_diagram.png` & `hgraph-0.2.8/docs/concepts/src_cmpt_snk_diagram.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/python/component_signature.md` & `hgraph-0.2.8/docs/python/component_signature.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/python/hg_types.md` & `hgraph-0.2.8/docs/python/hg_types.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/python/node_signature.md` & `hgraph-0.2.8/docs/python/node_signature.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/python/program_anatomy.md` & `hgraph-0.2.8/docs/python/program_anatomy.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/python/schema_based_types.md` & `hgraph-0.2.8/docs/python/schema_based_types.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/python/what_is_1_1.png` & `hgraph-0.2.8/docs/python/what_is_1_1.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/exception_handling.md` & `hgraph-0.2.8/docs/quick_start/exception_handling.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/exception_handling.py` & `hgraph-0.2.8/docs/quick_start/exception_handling.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/feedback.md` & `hgraph-0.2.8/docs/quick_start/feedback.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/generics.md` & `hgraph-0.2.8/docs/quick_start/generics.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/generics.py` & `hgraph-0.2.8/docs/quick_start/generics.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/graphs_and_nodes.md` & `hgraph-0.2.8/docs/quick_start/graphs_and_nodes.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/graphs_and_nodes.py` & `hgraph-0.2.8/docs/quick_start/graphs_and_nodes.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/hello_world.md` & `hgraph-0.2.8/docs/quick_start/hello_world.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/injectable_attributes.md` & `hgraph-0.2.8/docs/quick_start/injectable_attributes.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/injectable_attributes.py` & `hgraph-0.2.8/docs/quick_start/injectable_attributes.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/life_cycle.md` & `hgraph-0.2.8/docs/quick_start/life_cycle.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/map_reduce_switch.md` & `hgraph-0.2.8/docs/quick_start/map_reduce_switch.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/map_reduce_switch.py` & `hgraph-0.2.8/docs/quick_start/map_reduce_switch.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/node_testing.md` & `hgraph-0.2.8/docs/quick_start/node_testing.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/push_source_node.md` & `hgraph-0.2.8/docs/quick_start/push_source_node.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/push_source_node.py` & `hgraph-0.2.8/docs/quick_start/push_source_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/docs/quick_start/quick_start.md` & `hgraph-0.2.8/docs/quick_start/quick_start.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/examples/monitoring/monitoring.md` & `hgraph-0.2.8/examples/monitoring/monitoring.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/examples/monitoring/phase_1/monitoring_api.py` & `hgraph-0.2.8/examples/monitoring/phase_1/monitoring_api.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/examples/web_api/web_api.py` & `hgraph-0.2.8/examples/web_api/web_api.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_builder/_builder.py` & `hgraph-0.2.8/src/hgraph/_builder/_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_builder/_graph_builder.py` & `hgraph-0.2.8/src/hgraph/_builder/_graph_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_builder/_input_builder.py` & `hgraph-0.2.8/src/hgraph/_builder/_input_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_builder/_node_builder.py` & `hgraph-0.2.8/src/hgraph/_builder/_node_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_builder/_output_builder.py` & `hgraph-0.2.8/src/hgraph/_builder/_output_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_builder/_ts_builder.py` & `hgraph-0.2.8/src/hgraph/_builder/_ts_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/graph_construction.md` & `hgraph-0.2.8/src/hgraph/_impl/graph_construction.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_builder/_graph_builder.py` & `hgraph-0.2.8/src/hgraph/_impl/_builder/_graph_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_builder/_map_builder.py` & `hgraph-0.2.8/src/hgraph/_impl/_builder/_map_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_builder/_node_builder.py` & `hgraph-0.2.8/src/hgraph/_impl/_builder/_node_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_builder/_node_impl_builder.py` & `hgraph-0.2.8/src/hgraph/_impl/_builder/_node_impl_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_builder/_reduce_builder.py` & `hgraph-0.2.8/src/hgraph/_impl/_builder/_reduce_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_builder/_service_impl_builder.py` & `hgraph-0.2.8/src/hgraph/_impl/_builder/_service_impl_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_builder/_switch_builder.py` & `hgraph-0.2.8/src/hgraph/_impl/_builder/_switch_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_builder/_try_except_builder.py` & `hgraph-0.2.8/src/hgraph/_impl/_builder/_try_except_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_builder/_ts_builder.py` & `hgraph-0.2.8/src/hgraph/_impl/_builder/_ts_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_runtime/__init__.py` & `hgraph-0.2.8/src/hgraph/_impl/_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_runtime/_common.py` & `hgraph-0.2.8/src/hgraph/_impl/_runtime/_common.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_runtime/_data_writer.py` & `hgraph-0.2.8/src/hgraph/_impl/_runtime/_data_writer.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_runtime/_evaluation_clock.py` & `hgraph-0.2.8/src/hgraph/_impl/_runtime/_evaluation_clock.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_runtime/_evaluation_engine.py` & `hgraph-0.2.8/src/hgraph/_impl/_runtime/_evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_runtime/_graph.py` & `hgraph-0.2.8/src/hgraph/_impl/_runtime/_graph.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_runtime/_graph_executor.py` & `hgraph-0.2.8/src/hgraph/_impl/_runtime/_graph_executor.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_runtime/_graph_recorder.py` & `hgraph-0.2.8/src/hgraph/_impl/_runtime/_graph_recorder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_runtime/_map_node.py` & `hgraph-0.2.8/src/hgraph/_impl/_runtime/_map_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_runtime/_nested_evaluation_engine.py` & `hgraph-0.2.8/src/hgraph/_impl/_runtime/_nested_evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_runtime/_node.py` & `hgraph-0.2.8/src/hgraph/_impl/_runtime/_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_runtime/_reduce_node.py` & `hgraph-0.2.8/src/hgraph/_impl/_runtime/_reduce_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_runtime/_service_node_impl.py` & `hgraph-0.2.8/src/hgraph/_impl/_runtime/_service_node_impl.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_runtime/_switch_node.py` & `hgraph-0.2.8/src/hgraph/_impl/_runtime/_switch_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_runtime/_try_except_node.py` & `hgraph-0.2.8/src/hgraph/_impl/_runtime/_try_except_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_types/_feature_extension.py` & `hgraph-0.2.8/src/hgraph/_impl/_types/_feature_extension.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_types/_input.py` & `hgraph-0.2.8/src/hgraph/_impl/_types/_input.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_types/_output.py` & `hgraph-0.2.8/src/hgraph/_impl/_types/_output.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_types/_ref.py` & `hgraph-0.2.8/src/hgraph/_impl/_types/_ref.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_types/_scalar_value.py` & `hgraph-0.2.8/src/hgraph/_impl/_types/_scalar_value.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_types/_signal.py` & `hgraph-0.2.8/src/hgraph/_impl/_types/_signal.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_types/_ts.py` & `hgraph-0.2.8/src/hgraph/_impl/_types/_ts.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_types/_tsb.py` & `hgraph-0.2.8/src/hgraph/_impl/_types/_tsb.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_types/_tsd.py` & `hgraph-0.2.8/src/hgraph/_impl/_types/_tsd.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_types/_tsl.py` & `hgraph-0.2.8/src/hgraph/_impl/_types/_tsl.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_impl/_types/_tss.py` & `hgraph-0.2.8/src/hgraph/_impl/_types/_tss.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_runtime/__init__.py` & `hgraph-0.2.8/src/hgraph/_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_runtime/_data_writer.py` & `hgraph-0.2.8/src/hgraph/_runtime/_data_writer.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_runtime/_evaluation_clock.py` & `hgraph-0.2.8/src/hgraph/_runtime/_evaluation_clock.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_runtime/_evaluation_engine.py` & `hgraph-0.2.8/src/hgraph/_runtime/_evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_runtime/_feedback.py` & `hgraph-0.2.8/src/hgraph/_runtime/_feedback.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_runtime/_global_state.py` & `hgraph-0.2.8/src/hgraph/_runtime/_global_state.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_runtime/_graph.py` & `hgraph-0.2.8/src/hgraph/_runtime/_graph.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_runtime/_graph_executor.py` & `hgraph-0.2.8/src/hgraph/_runtime/_graph_executor.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_runtime/_graph_recorder.py` & `hgraph-0.2.8/src/hgraph/_runtime/_graph_recorder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_runtime/_graph_runner.py` & `hgraph-0.2.8/src/hgraph/_runtime/_graph_runner.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_runtime/_lifecycle.py` & `hgraph-0.2.8/src/hgraph/_runtime/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_runtime/_node.py` & `hgraph-0.2.8/src/hgraph/_runtime/_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_runtime/_operators.py` & `hgraph-0.2.8/src/hgraph/_runtime/_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/__init__.py` & `hgraph-0.2.8/src/hgraph/_types/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_error_type.py` & `hgraph-0.2.8/src/hgraph/_types/_error_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_frame_scalar_type_meta_data.py` & `hgraph-0.2.8/src/hgraph/_types/_frame_scalar_type_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_ref_meta_data.py` & `hgraph-0.2.8/src/hgraph/_types/_ref_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_ref_type.py` & `hgraph-0.2.8/src/hgraph/_types/_ref_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_scalar_type_meta_data.py` & `hgraph-0.2.8/src/hgraph/_types/_scalar_type_meta_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,21 +124,21 @@
             return tp
         elif not weak:
             raise ParseError(f"No resolution available for '{str(self)}'")
         else:
             return self
 
     def do_build_resolution_dict(self, resolution_dict: dict[TypeVar, "HgTypeMetaData"], wired_type: "HgTypeMetaData"):
-        if not wired_type.is_scalar:
+        if wired_type and not wired_type.is_scalar:
             raise ParseError(f"Scalar TypeVar '{str(self)}' does not match non-scalar type: '{str(wired_type)}'")
         type_var: TypeVar = cast(TypeVar, self.py_type)
         if self == wired_type:
             return  # No additional information can be gleaned!
         if type_var in resolution_dict:
-            if resolution_dict[type_var] != wired_type:
+            if wired_type and resolution_dict[type_var] != wired_type:
                 from hgraph._wiring._wiring_errors import TemplateTypeIncompatibleResolution
                 raise TemplateTypeIncompatibleResolution(self, resolution_dict[type_var], wired_type)
         else:
             resolution_dict[type_var] = wired_type
 
     @classmethod
     def parse_type(cls, value_tp) -> Optional["HgTypeMetaData"]:
@@ -171,15 +171,15 @@
         self.py_type = py_type
         self.convertable_types = convertable_types
 
     def __eq__(self, o: object) -> bool:
         return type(o) is HgAtomicType and self.py_type is o.py_type
 
     def __str__(self) -> str:
-        return f'{self.py_type}'
+        return f'{self.py_type.__name__}'
 
     def __repr__(self) -> str:
         return f'HgAtomicType({repr(self.py_type)})'
 
     def __hash__(self) -> int:
         return hash(self.py_type)
```

### Comparing `hgraph-0.2.7/src/hgraph/_types/_scalar_types.py` & `hgraph-0.2.8/src/hgraph/_types/_scalar_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,17 +212,29 @@
 
 def is_keyable_scalar(value) -> bool:
     """
     Is this value a supported scalar type. Not all python types are valid scalar types.
     This is a first pass estimate, and does not do a deep parse on container classes.
     This is not a substitute for HgScalarType.parse.
     """
-    return isinstance(value, (bool, int, float, date, datetime, time, timedelta, str, tuple, frozenset, frozendict,
-                              CompoundScalar, Size, Enum)) or (
-            isinstance(value, type) and (value in (bool, int, float, date, datetime, time, timedelta, str) or
-                                         issubclass(value, (tuple, frozenset, frozendict, CompoundScalar, Size, Enum)))
+    return (
+            isinstance(value, (bool, int, float, date, datetime, time, timedelta, str, tuple, frozenset, frozendict,
+                              CompoundScalar, Size, Enum))
+            or
+            (isinstance(value, type) and (
+                    value in (bool, int, float, date, datetime, time, timedelta, str)
+                    or
+                    issubclass(value, (tuple, frozenset, frozendict, CompoundScalar, Size, Enum))))
+            or
+            (isinstance(value, TypeVar) and (
+                        value.__bound__ in (Hashable, bool, int, float, date, datetime, time, timedelta, str)
+                        or
+                        issubclass(value.__bound__, (tuple, frozenset, frozendict, CompoundScalar, Size, Enum))
+                        or
+                        all(is_keyable_scalar(v) for v in value.__constraints__)
+                        ))
     )
 
 
 def is_compound_scalar(value) -> bool:
     """Is the value an instance of CompoundScalar or is a type which is a subclass of CompoundScalar"""
     return isinstance(value, CompoundScalar) or (isinstance(value, type) and issubclass(value, CompoundScalar))
```

### Comparing `hgraph-0.2.7/src/hgraph/_types/_scalar_value.py` & `hgraph-0.2.8/src/hgraph/_types/_scalar_value.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_schema_type.py` & `hgraph-0.2.8/src/hgraph/_types/_schema_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_time_series_meta_data.py` & `hgraph-0.2.8/src/hgraph/_types/_time_series_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_time_series_types.py` & `hgraph-0.2.8/src/hgraph/_types/_time_series_types.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_ts_meta_data.py` & `hgraph-0.2.8/src/hgraph/_types/_ts_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_ts_signal_meta_data.py` & `hgraph-0.2.8/src/hgraph/_types/_ts_signal_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_ts_type.py` & `hgraph-0.2.8/src/hgraph/_types/_ts_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_ts_type_var_meta_data.py` & `hgraph-0.2.8/src/hgraph/_types/_ts_type_var_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_tsb_meta_data.py` & `hgraph-0.2.8/src/hgraph/_types/_tsb_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_tsb_type.py` & `hgraph-0.2.8/src/hgraph/_types/_tsb_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_tsd_meta_data.py` & `hgraph-0.2.8/src/hgraph/_types/_tsd_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_tsd_type.py` & `hgraph-0.2.8/src/hgraph/_types/_tsd_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_tsl_meta_data.py` & `hgraph-0.2.8/src/hgraph/_types/_tsl_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_tsl_type.py` & `hgraph-0.2.8/src/hgraph/_types/_tsl_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_tss_meta_data.py` & `hgraph-0.2.8/src/hgraph/_types/_tss_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_tss_type.py` & `hgraph-0.2.8/src/hgraph/_types/_tss_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_types/_type_meta_data.py` & `hgraph-0.2.8/src/hgraph/_types/_type_meta_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         The outputs are fully reliant on types to be resolved using the wired_types on the inputs to resolve the output
         types.
         """
         if self.is_resolved:
             return
 
         if self != wired_type:
-            self.do_build_resolution_dict(resolution_dict, wired_type.dereference())
+            self.do_build_resolution_dict(resolution_dict, wired_type.dereference() if wired_type else None)
 
     def do_build_resolution_dict(self, resolution_dict: dict[TypeVar, "HgTypeMetaData"], wired_type: "HgTypeMetaData"):
         """
         Implementation method for build_resolution_dict - to be overriden by the derived classes
         """
         if wired_type is not None and type(self) != type(wired_type):
             from hgraph._wiring._wiring_errors import IncorrectTypeBinding
```

### Comparing `hgraph-0.2.7/src/hgraph/_types/_typing_utils.py` & `hgraph-0.2.8/src/hgraph/_types/_typing_utils.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/__init__.py` & `hgraph-0.2.8/src/hgraph/_wiring/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 from hgraph._wiring._dispatch import *
 from hgraph._wiring._wiring_node_class._switch_wiring_node import *
 from hgraph._wiring._wiring_node_class._try_except_wiring_node import *
 from hgraph._wiring._wiring_node_class import *
 from hgraph._wiring._wiring_context import *
 from hgraph._wiring._wiring_errors import *
 from hgraph._wiring._wiring_node_signature import *
+from hgraph._wiring._wiring_port import *
 from hgraph._wiring._wiring_utils import *
```

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_decorators.py` & `hgraph-0.2.8/src/hgraph/_wiring/_decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,22 +84,24 @@
     :param overloads: If this node overloads an operator, this is the operator it is designed to overload.
     """
     from hgraph._wiring._wiring_node_signature import WiringNodeType
     return _node_decorator(WiringNodeType.SINK_NODE, fn, node_impl, active, valid, all_valid, overloads=overloads,
                            resolvers=resolvers)
 
 
-def graph(fn: GRAPH_SIGNATURE = None, overloads: "WiringNodeClass" | GRAPH_SIGNATURE = None) -> GRAPH_SIGNATURE:
+def graph(fn: GRAPH_SIGNATURE = None,
+          overloads: "WiringNodeClass" | GRAPH_SIGNATURE = None,
+          resolvers: Mapping[TypeVar, Callable] = None) -> GRAPH_SIGNATURE:
     """
     Wraps a wiring function. The function can take the form of a function that looks like a compute_node,
     sink_node, souce_node, or a graph with no inputs or outputs. There is generally at least one graph in
     any application. The main graph.
     """
     from hgraph._wiring._wiring_node_signature import WiringNodeType
-    return _node_decorator(WiringNodeType.GRAPH, fn, overloads=overloads)
+    return _node_decorator(WiringNodeType.GRAPH, fn, overloads=overloads, resolvers=resolvers)
 
 
 def generator(fn: SOURCE_NODE_SIGNATURE = None,
               overloads: "WiringNodeClass" | GRAPH_SIGNATURE = None,
               resolvers: Mapping[TypeVar, Callable] = None) -> SOURCE_NODE_SIGNATURE:
     """
     Creates a pull source node that supports generating a sequence of ticks that will be fed into the
@@ -174,15 +176,16 @@
 
 
 SERVICE_DEFINITION = TypeVar('SERVICE_DEFINITION', bound=Callable)
 
 default_path = None
 
 
-def subscription_service(fn: SERVICE_DEFINITION) -> SERVICE_DEFINITION:
+def subscription_service(fn: SERVICE_DEFINITION = None,
+                         resolvers: Mapping[TypeVar, Callable] = None) -> SERVICE_DEFINITION:
     """
     A subscription service is a service where the input receives a subscription key and then
     streams back results. This looks like:
 
         default=None
 
         @subscription_service
@@ -196,18 +199,19 @@
         @graph
         def my_code():
             register_service(default, my_subscription_svc, my_subscription_svc_impl)
             ...
             out = my_subscription_svc(default, ts1="mkt_data.mcu_3m")
     """
     from hgraph._wiring._wiring_node_signature import WiringNodeType
-    return _node_decorator(WiringNodeType.SUBS_SVC, fn)
+    return _node_decorator(WiringNodeType.SUBS_SVC, fn, resolvers=resolvers)
 
 
-def reference_service(fn: SERVICE_DEFINITION) -> SERVICE_DEFINITION:
+def reference_service(fn: SERVICE_DEFINITION = None,
+                      resolvers: Mapping[TypeVar, Callable] = None) -> SERVICE_DEFINITION:
     """
     A reference service is a service that only produces a value that does not vary by request.
     The pattern for a reference services is the same as a source node.
 
     for example:
 
         @reference_service
@@ -218,18 +222,19 @@
     and that bound instance will be to the path 'ref_svc://<module>.<svc_name>' for example:
     'ref_svc://a.b.c.my_reference_service'
 
     The implementation needs to be registered by the outer wiring node, if not registered, it will look for a remote
     instance of the service to bind to.
     """
     from hgraph._wiring._wiring_node_signature import WiringNodeType
-    return _node_decorator(WiringNodeType.REF_SVC, fn)
+    return _node_decorator(WiringNodeType.REF_SVC, fn, resolvers=resolvers)
 
 
-def request_reply_service(fn: SERVICE_DEFINITION) -> SERVICE_DEFINITION:
+def request_reply_service(fn: SERVICE_DEFINITION = None,
+                          resolvers: Mapping[TypeVar, Callable] = None) -> SERVICE_DEFINITION:
     """
     A request-reply service takes a request and returns a response, error or time-out.
     for example:
 
         class RequestReplyService(Generic[TIME_SERIES_TYPE_1]):
             result: TIME_SERIES_TYPE_1
             time_out: TS[bool]
@@ -237,42 +242,55 @@
 
         @request_reply_service
         def my_request_replay(path: str | None, request: TIME_SERIES_TYPE) -> TSB[ReqRepResponse[TIME_SERIES_TYPE_1]]:
             ...
 
     """
     from hgraph._wiring._wiring_node_signature import WiringNodeType
-    return _node_decorator(WiringNodeType.REQ_REP_SVC, fn)
+    return _node_decorator(WiringNodeType.REQ_REP_SVC, fn, resolvers=resolvers)
 
 
-def service_impl(*, interfaces: Sequence[SERVICE_DEFINITION] | SERVICE_DEFINITION = None):
+def service_impl(*, interfaces: Sequence[SERVICE_DEFINITION] | SERVICE_DEFINITION = None,
+                 resolvers: Mapping[TypeVar, Callable] = None):
     """
     Wraps a service implementation. The service is defined to implement the declared interface.
     """
     from hgraph._wiring._wiring_node_signature import WiringNodeType
-    return _node_decorator(WiringNodeType.SVC_IMPL, None, interfaces=interfaces)
+    return _node_decorator(WiringNodeType.SVC_IMPL, None, interfaces=interfaces, resolvers=resolvers)
 
 
-def register_service(path: str, implementation, **kwargs):
+def register_service(path: str, implementation, resolution_dict=None, **kwargs):
     """
     Binds the implementation of the interface to the path provided. The additional kwargs
     are passed to the implementation. These should be defined on the implementation and are independent of the
     attributes defined in the service.
     :param path:
     :param implementation:
+    :param resolution_dict:
     :param kwargs:
     :return:
     """
+    from hgraph._wiring._wiring_node_class._wiring_node_class import PreResolvedWiringNodeWrapper, WiringNodeClass
     from hgraph._wiring._wiring_node_class._service_impl_node_class import ServiceImplNodeClass
+
+    if isinstance(implementation, PreResolvedWiringNodeWrapper):
+        implementation = implementation.underlying_node
+        resolution_dict = implementation.resolved_types or {}
+    else:
+        resolution_dict = WiringNodeClass._convert_item(resolution_dict) if resolution_dict else {}
+
     if not isinstance(implementation, ServiceImplNodeClass):
         raise CustomMessageWiringError("The provided implementation is not a 'service_impl' wrapped function.")
 
     from hgraph import WiringGraphContext
+
     for i in implementation.interfaces:
-        WiringGraphContext.instance().register_service_impl(i, i.full_path(path), implementation, kwargs)
+        WiringGraphContext.instance().register_service_impl(
+            i, i.full_path(path) if path else None, implementation, kwargs,
+            resolution_dict)
 
 
 def service_adaptor(interface):
     """
     @service
     def my_interface(ts1: TIME_SERIES, ...) -> OUT_TIME_SERIES:
         pass
```

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_dispatch.py` & `hgraph-0.2.8/src/hgraph/_wiring/_dispatch.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_exception_handling.py` & `hgraph-0.2.8/src/hgraph/_wiring/_exception_handling.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_graph_builder.py` & `hgraph-0.2.8/src/hgraph/_wiring/_graph_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_map.py` & `hgraph-0.2.8/src/hgraph/_wiring/_map.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_reduce.py` & `hgraph-0.2.8/src/hgraph/_wiring/_reduce.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_stub_wiring_node.py` & `hgraph-0.2.8/src/hgraph/_wiring/_stub_wiring_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_switch.py` & `hgraph-0.2.8/src/hgraph/_wiring/_switch.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_context.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_context.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_errors.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_errors.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_instance.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_instance.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_signature.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_signature.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     HgTypeOfTypeMetaData
 from hgraph._types._time_series_meta_data import HgTimeSeriesTypeMetaData
 from hgraph._types._type_meta_data import HgTypeMetaData, AUTO_RESOLVE
 from hgraph._types._type_meta_data import ParseError
 from hgraph._types._tsb_meta_data import HgTimeSeriesSchemaTypeMetaData, HgTSBTypeMetaData
 from hgraph._wiring._source_code_details import SourceCodeDetails
 from hgraph._wiring._wiring_context import WiringContext
-from hgraph._wiring._wiring_errors import IncorrectTypeBinding
+from hgraph._wiring._wiring_errors import IncorrectTypeBinding, CustomMessageWiringError
 
 __all__ = ("extract_signature", "WiringNodeType", "WiringNodeSignature", "extract_hg_type",
            "extract_hg_time_series_type", "extract_scalar_type", "extract_injectable_inputs")
 
 
 class WiringNodeType(Enum):
     PUSH_SOURCE_NODE = 0
@@ -141,14 +141,76 @@
         """Split out scalar inputs from time-series inputs """
         return frozendict({k: v for k, v in self.input_types.items() if v.is_scalar})
 
     @property
     def time_series_inputs(self) -> Mapping[str, HgTimeSeriesTypeMetaData]:
         return frozendict({k: v for k, v in self.input_types.items() if not v.is_scalar})
 
+    def convert_kwargs_to_types(self, _ensure_match=True, **kwargs) -> dict[str, HgTypeMetaData]:
+        """Attempt to convert input types to better support type resolution"""
+        # We only need to extract un-resolved values
+        kwarg_types = {}
+        for k, v in self.input_types.items():
+            with WiringContext(current_arg=k):
+                arg = kwargs.get(k, self.defaults.get(k))
+                if arg is None:
+                    if v.is_injectable:
+                        # For injectables we expect the value to be None, and the type must already be resolved.
+                        kwarg_types[k] = v
+                    else:
+                        # We should wire in a null source
+                        if k in self.defaults:
+                            kwarg_types[k] = v
+                        elif _ensure_match:
+                            raise CustomMessageWiringError(
+                                f"Argument '{k}' is not marked as optional, but no value was supplied")
+                if k in filter(lambda k_: k_ in self.time_series_args, self.args):
+                    # This should then get a wiring node, and we would like to extract the output type,
+                    # But this is optional, so we should ensure that the type is present
+                    if arg is None:
+                        continue  # We will wire in a null source later
+                    from hgraph import WiringPort
+                    if not isinstance(arg, WiringPort):
+                        tp = HgScalarTypeMetaData.parse_value(arg)
+                        kwarg_types[k] = tp
+                    elif arg.output_type:
+                        kwarg_types[k] = arg.output_type
+                    elif _ensure_match:
+                        raise ParseError(
+                            f'{k}: {v} = {arg}, argument supplied is not a valid source or compute_node output')
+                elif type(v) is HgTypeOfTypeMetaData:
+                    if not isinstance(arg, (type, GenericAlias, _GenericAlias, TypeVar)) and arg is not AUTO_RESOLVE:
+                        # This is not a type of something (Have seen this as being an instance of HgTypeMetaData)
+                        raise IncorrectTypeBinding(v, arg)
+                    v = HgTypeMetaData.parse_type(arg) if arg is not AUTO_RESOLVE else v.value_tp
+                    kwarg_types[k] = HgTypeOfTypeMetaData(v)
+                else:
+                    if arg is None:
+                        kwarg_types[k] = v
+                    else:
+                        tp = HgScalarTypeMetaData.parse_value(arg)
+                        kwarg_types[k] = tp
+                        if tp is None:
+                            if k in self.unresolved_args:
+                                if _ensure_match:
+                                    raise ParseError(f"In {self.name}, {k}: {v} = {arg}; arg is not parsable, "
+                                                     f"but we require type resolution")
+                            else:
+                                # If the signature was not unresolved, then we can use the signature, but the input value
+                                # May yet be incorrectly typed.
+                                kwarg_types[k] = v
+        return kwarg_types
+
+    def try_build_resolution_dict(self, pre_resolved_types: dict[TypeVar, HgTypeMetaData | Callable]):
+        from hgraph._wiring._wiring_node_class import extract_kwargs
+        pre_resolved_types = pre_resolved_types or {}
+        kwargs = extract_kwargs(self, _ensure_match=False)
+        kwarg_types = self.convert_kwargs_to_types(**kwargs, _ensure_match=False)
+        return self.build_resolution_dict(pre_resolved_types, kwarg_types, kwargs)
+
     def build_resolution_dict(self, pre_resolved_types: dict[TypeVar, HgTypeMetaData | Callable],
                               kwarg_types, kwargs) -> dict[TypeVar, HgTypeMetaData]:
         """Expect kwargs to be a dict of arg to type mapping / value mapping"""
         resolution_dict: dict[TypeVar, HgTypeMetaData] = {k: v for k, v in pre_resolved_types.items() if
                                                           isinstance(v, HgTypeMetaData)} if pre_resolved_types else {}
         resolvers_dict: dict[TypeVar, Callable] = {k: v for k, v in pre_resolved_types.items() if
                                                           isfunction(v)} if pre_resolved_types else {}
@@ -160,16 +222,17 @@
                     meta_data.build_resolution_dict_from_scalar(resolution_dict, kwt, kwargs[arg])
                 else:
                     meta_data.build_resolution_dict(resolution_dict, kwarg_types.get(arg))
         # now ensures all "resolved" items are actually resolved
         out_dict = {}
         all_resolved = True
         for k, v in resolution_dict.items():
-            out_dict[k] = v if v.is_resolved else v.resolve(resolution_dict)
-            all_resolved &= out_dict[k].is_resolved
+            if v is not None:
+                out_dict[k] = v if v.is_resolved else v.resolve(resolution_dict)
+                all_resolved &= out_dict[k].is_resolved
 
         if resolvers_dict:
             scalars = {k: v for k, v in kwargs.items() if (kwt := kwarg_types.get(k)) and kwt.is_scalar}
             for k, v in pre_resolved_types.items():
                 if isfunction(v) and k not in out_dict:
                     resolved = v(resolution_dict, scalars)
                     if isinstance(resolved, (type, GenericAlias, _GenericAlias, TypeVar)):
```

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_port.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_port.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import typing
 from dataclasses import dataclass
 from functools import cached_property
 from typing import Mapping, Generic
 
-from hgraph._types._typing_utils import nth
-
+from hgraph._types._ref_meta_data import HgREFTypeMetaData
+from hgraph._types._scalar_types import SCALAR
 from hgraph._types._time_series_meta_data import HgTimeSeriesTypeMetaData
+from hgraph._types._time_series_types import TIME_SERIES_TYPE
 from hgraph._types._tsb_meta_data import HgTSBTypeMetaData
+from hgraph._types._tsb_type import TimeSeriesSchema
 from hgraph._types._tsd_meta_data import HgTSDTypeMetaData
+from hgraph._types._tsd_type import KEY_SET_ID
 from hgraph._types._tsl_meta_data import HgTSLTypeMetaData
-from hgraph._types._ref_meta_data import HgREFTypeMetaData
-from hgraph._types._type_meta_data import HgTypeMetaData
-from hgraph._types._ref_type import REF
-from hgraph._types._ref_meta_data import HgREFTypeMetaData
 from hgraph._types._tss_type import TSS
-from hgraph._types._tsd_type import KEY_SET_ID
-from hgraph._types._tsb_type import TimeSeriesSchema
-from hgraph._wiring._wiring_errors import CustomMessageWiringError
-from hgraph._types._scalar_types import SCALAR
-from hgraph._types._time_series_types import TIME_SERIES_TYPE
+from hgraph._types._type_meta_data import HgTypeMetaData
+from hgraph._types._typing_utils import nth
 from hgraph._wiring._wiring_context import WIRING_CONTEXT
+from hgraph._wiring._wiring_errors import CustomMessageWiringError
 
 if typing.TYPE_CHECKING:
     from hgraph import WiringNodeInstance
 
 
+__all__ = ("WiringPort", "ErrorWiringPort", "TSDWiringPort", "TSDREFWiringPort",
+           "TSBWiringPort", "TSBREFWiringPort", "TSLWiringPort", "TSLREFWiringPort")
+
+
 def _wiring_port_for(tp: HgTypeMetaData, node_instance: "WiringNodeInstance", path: [int, ...]) -> "WiringPort":
     return {
         HgTSDTypeMetaData: lambda: TSDWiringPort(node_instance, path),
         HgTSBTypeMetaData: lambda: TSBWiringPort(node_instance, path),
         HgTSLTypeMetaData: lambda: TSLWiringPort(node_instance, path),
         HgREFTypeMetaData: lambda: {
                    HgTSDTypeMetaData: lambda: TSDREFWiringPort(node_instance, path),
```

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_utils.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_utils.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/__init__.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_graph_wiring_node_class.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_graph_wiring_node_class.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import sys
-from collections import defaultdict
 from copy import copy
 from graphlib import TopologicalSorter
-from itertools import chain
 from typing import Optional, TypeVar, Callable, Tuple, Dict
 
-from hgraph._wiring._wiring_node_signature import WiringNodeSignature
+from frozendict import frozendict
+
 from hgraph._types._ts_type_var_meta_data import HgTsTypeVarTypeMetaData
 from hgraph._types._type_meta_data import HgTypeMetaData
 from hgraph._wiring._source_code_details import SourceCodeDetails
 from hgraph._wiring._wiring_context import WiringContext
-from hgraph._wiring._wiring_node_class._wiring_node_class import BaseWiringNodeClass
-from hgraph._wiring._wiring_port import WiringPort
 from hgraph._wiring._wiring_errors import WiringError, CustomMessageWiringError
+from hgraph._wiring._wiring_node_class._service_interface_node_class import ServiceInterfaceNodeClass
+from hgraph._wiring._wiring_node_class._wiring_node_class import BaseWiringNodeClass, PreResolvedWiringNodeWrapper
+from hgraph._wiring._wiring_node_signature import WiringNodeSignature, WiringNodeType
+from hgraph._wiring._wiring_port import WiringPort
 
 __all__ = ('WiringGraphContext', "GraphWiringNodeClass")
 
 
 class WiringGraphContext:
     """
     Used to track the call stack and to track sink nodes for the graph.
@@ -57,29 +58,29 @@
         return [graph.wiring_node_signature.src_location for graph in reversed(cls.__stack__[1:])
                 if graph.wiring_node_signature]
 
     @classmethod
     def wiring_path_name(cls) -> str:
         """Return a graph call stack in names of graphs"""
         return '.'.join(graph.wiring_node_signature.name for graph in cls.__stack__[1:]
-                if graph.wiring_node_signature)
+                        if graph.wiring_node_signature)
 
     @classmethod
     def instance(cls) -> "WiringGraphContext":
         return WiringGraphContext.__stack__[-1] if WiringGraphContext.__stack__ else None
 
     def __init__(self, node_signature: Optional[WiringNodeSignature]):
         """
         If we are wiring the root graph, then there is no wiring node. In this case None is
         passed in.
         """
         self._wiring_node_signature: WiringNodeSignature = node_signature
         self._sink_nodes: ["WiringNodeInstance"] = []
         self._other_nodes: [Tuple["WiringPort", dict]] = []
-        self._service_clients: [Tuple["WiringNodeClass", str]] = []
+        self._service_clients: [Tuple["WiringNodeClass", str, dict[TypeVar, HgTypeMetaData]]] = []
         self._service_implementations: Dict[str, Tuple["WiringNodeClass", "ServiceImplNodeClass", dict]] = {}
         self._built_services = {}
 
         self._current_frame = sys._getframe(1)
 
     @property
     def sink_nodes(self) -> tuple["WiringNodeInstance", ...]:
@@ -119,85 +120,123 @@
         Label the nodes in the graph with the variable name if the output was assigned to a local variable
         """
         for port, locals in self._other_nodes:
             varname = next((k for k, v in locals.items() if v is port), None)
             if varname and port.path == ():
                 port.node_instance.set_label(varname)
 
-    def register_service_client(self, service: "ServiceInterfaceNodeClass", path: str):
+    def register_service_client(self, service: "ServiceInterfaceNodeClass", path: str, type_map: dict = None):
         """
         Register a service client with the graph context
         """
-        self._service_clients.append((service, path))
+        self._service_clients.append((service, path, frozendict(type_map) if type_map else frozendict()))
 
-    def register_service_impl(self, service: "ServiceInterfaceNodeClass", path: str, impl: "ServiceImplNodeClass", kwargs):
+    def register_service_impl(self, service: "ServiceInterfaceNodeClass", path: str, impl: "ServiceImplNodeClass",
+                              kwargs, resolution_dict=None):
         """
         Register a service client with the graph context
         """
+        if path is None:
+            path = service.signature.name
+
+        if resolution_dict:
+            path = f"{path}[{ServiceInterfaceNodeClass._resolution_dict_to_str(resolution_dict)}]"
+
         if prev_impl := self._service_implementations.get(path):
             CustomMessageWiringError(f"Service implementation already registered for service at path: {path}: "
                                      f"{prev_impl[0].signature.signature} with {prev_impl[1]}")
 
         self._service_implementations[path] = (service, impl, kwargs)
 
-    def find_service_impl(self, path):
-        for c in WiringGraphContext.__stack__:
-            if item := c._service_implementations.get(path):
-                return item
-
-        raise CustomMessageWiringError(f"No service implementation found for path: {path}")
+    def find_service_impl(self, path, resolution_dict=None, quiet=False):
+        if path.endswith(']'):
+            typed_path = path
+            path = path.split('[', 1)[0]
+        elif resolution_dict:
+            typed_path = f"{path}[{ServiceInterfaceNodeClass._resolution_dict_to_str(resolution_dict)}]"
+        else:
+            typed_path = None
+
+        def find_impl(path):
+            for c in WiringGraphContext.__stack__:
+                if item := c._service_implementations.get(path):
+                    return item
+
+        if typed_path and (item := find_impl(typed_path)):
+            return item
+        elif item := find_impl(path):
+            return item
+        elif item := find_impl(path.split('/')[-1]):
+            return item
+        else:
+            if not quiet:
+                raise CustomMessageWiringError(f"No service implementation found for path: {typed_path}")
 
     def add_built_service_impl(self, path, node):
         if node:
             self.add_sink_node(node)
 
         self._built_services[path] = node
 
     def built_services(self):
         return self._built_services
 
+    def is_service_built(self, path, resolution_dict=None):
+        if resolution_dict:
+            path = f"{path}[{ServiceInterfaceNodeClass._resolution_dict_to_str(resolution_dict)}]"
+
+        return self._built_services.get(path)
+
     def build_services(self):
         """
         Build the service implementations for the graph
         """
         service_clients = copy(self._service_clients)
         dependencies = {}
         while True:
-            services_to_build = set()
-            for service, path in set(service_clients):
-                if item := self._service_implementations.get(path):
+            services_to_build = dict()
+            for service, path, type_map in set(service_clients):
+                typed_path = service.typed_full_path(path, type_map)
+
+                if item := self.find_service_impl(path, type_map):
                     interface, impl, kwargs = item
-                    if interface != service:
-                        raise CustomMessageWiringError(f"service implementation for path {path} implements "
-                                                       f"{interface.signature.signature} which does not match the client "
-                                                       f"expecting {service.signature.signature}")
-                    services_to_build.add(path)
                 else:
-                    raise CustomMessageWiringError(f'No implementation found for service: {service.signature.name} at path: {path}')
+                    raise CustomMessageWiringError(
+                        f'No implementation found for service: {service.signature.name} at path: {path}')
+
+                if isinstance(interface, PreResolvedWiringNodeWrapper):
+                    interface = interface.underlying_node
 
-            for path in services_to_build:
-                if path not in self._built_services:
+                if interface != service:
+                    raise CustomMessageWiringError(f"service implementation for path {path} implements "
+                                                   f"{interface.signature.signature} which does not match the client "
+                                                   f"expecting {service.signature.signature}")
+
+                services_to_build[typed_path] = (service, path, impl, kwargs, type_map)
+
+            for typed_path in services_to_build:
+                if typed_path not in self._built_services:
                     clients_before = len(self._service_clients)
 
-                    service, impl, kwargs = self._service_implementations[path]
-                    impl(path=path, __interface__=service, **kwargs)
+                    service, path, impl, kwargs, type_map = services_to_build[typed_path]
+                    impl(path=path, __interface__=service, __pre_resolved_types__=type_map, **kwargs)
 
                     new_clients = self._service_clients[clients_before:]
-                    dependencies.update({path: set(p for _, p in new_clients if p != path)})
+                    dependencies.update({typed_path: set(s.typed_full_path(p, t) for s, p, t in new_clients
+                                                         if s.signature.node_type != WiringNodeType.REQ_REP_SVC)})
 
             if self._service_clients == service_clients:
                 break
             else:
                 service_clients = copy(self._service_clients)
 
         ordered = list(TopologicalSorter(dependencies).static_order())
         for i, path in enumerate(ordered):
             object.__setattr__(self._built_services[path], 'rank', i + 2)
 
-
     def __enter__(self):
         WiringGraphContext.__stack__.append(self)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         WiringGraphContext.__stack__.pop()
         if WiringGraphContext.__stack__:
@@ -219,45 +258,48 @@
         if found_overload:
             return r
 
         # We don't want graph and node signatures to operate under different rules as this would make
         # moving between node and graph implementations problematic, so resolution rules of the signature
         # hold
         with WiringContext(current_wiring_node=self, current_signature=self.signature):
-            kwargs_, resolved_signature = self._validate_and_resolve_signature(*args,
-                                                                               __pre_resolved_types__=__pre_resolved_types__,
-                                                                               __enforce_output_type__=False,
-                                                                               **kwargs)
+            kwargs_, resolved_signature, _ = self._validate_and_resolve_signature(*args,
+                                                                                  __pre_resolved_types__=__pre_resolved_types__,
+                                                                                  __enforce_output_type__=False,
+                                                                                  **kwargs)
 
             # But graph nodes are evaluated at wiring time, so this is the graph expansion happening here!
             with WiringGraphContext(self.signature) as g:
                 out: WiringPort = self.fn(**kwargs_)
                 WiringGraphContext.instance().label_nodes()
                 if output_type := resolved_signature.output_type:
                     from hgraph import HgTSBTypeMetaData
                     if not isinstance(out, WiringPort):
                         if isinstance(out, dict) and isinstance(output_type, HgTSBTypeMetaData):
                             out = output_type.py_type.from_ts(**out)
                         elif isinstance(out, dict) and isinstance(output_type, HgTsTypeVarTypeMetaData):
                             for c in output_type.constraints:
                                 if isinstance(c, HgTSBTypeMetaData) and \
-                                        all((t:= c.bundle_schema_tp.meta_data_schema.get(k)) and t.matches(v.output_type.dereference()) for k, v in out.items()):
+                                        all((t := c.bundle_schema_tp.meta_data_schema.get(k)) and t.matches(
+                                            v.output_type.dereference()) for k, v in out.items()):
                                     out = c.py_type.from_ts(**out)
                                     break
                             else:
-                                raise WiringError(f"Expected a time series of type '{str(output_type)}' but got a dict of "
-                                                  f"{{{', '.join(f'{k}:{str(v.output_type)}' for k, v in out.items())}}}")
+                                raise WiringError(
+                                    f"Expected a time series of type '{str(output_type)}' but got a dict of "
+                                    f"{{{', '.join(f'{k}:{str(v.output_type)}' for k, v in out.items())}}}")
                         else:
                             try:
                                 # use build resolution dict from scalar as a proxy for "is this scalar a valid const value for this time series"
                                 output_type.build_resolution_dict_from_scalar({}, HgTypeMetaData.parse_value(out), out)
                                 from hgraph.nodes import const
                                 out = const(out, tp=output_type.py_type)
                             except Exception as e:
-                                raise WiringError(f"Expected a time series of type '{str(output_type)}' but got '{str(out)}'") from e
+                                raise WiringError(
+                                    f"Expected a time series of type '{str(output_type)}' but got '{str(out)}'") from e
 
                     if not output_type.dereference().matches(out.output_type.dereference()):
                         raise WiringError(f"'{self.signature.name}' declares it's output as '{str(output_type)}' but "
                                           f"'{str(out.output_type)}' was returned from the graph")
                 elif WiringGraphContext.is_strict() and not g.has_sink_nodes():
                     raise WiringError(f"'{self.signature.name}' does not seem to do anything")
                 return out
```

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_map_wiring_node.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_map_wiring_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_node_impl_wiring_node_class.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_node_impl_wiring_node_class.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_pull_source_node_class.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_pull_source_node_class.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_python_wiring_node_classes.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_python_wiring_node_classes.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_reduce_wiring_node.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_reduce_wiring_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_reference_service_node_class.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_reference_service_node_class.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,16 +28,14 @@
         if type(output_type) is not HgREFTypeMetaData:
             node_signature = node_signature.copy_with(time_series_output=HgREFTypeMetaData(output_type))
 
         from hgraph._impl._builder import PythonNodeImplNodeBuilder
         input_builder, output_builder, error_builder = create_input_output_builders(node_signature,
                                                                                     self.error_output_type)
 
-        scalars = frozendict({"path": self.full_path(scalars.get("path"))})
-
         from hgraph._impl._runtime._node import BaseNodeImpl
 
         class _PythonReferenceServiceStubSourceNode(BaseNodeImpl):
 
             def do_eval(self):
                 """The service must be available by now, so we can retrieve the output reference."""
                 from hgraph._runtime._global_state import GlobalState
@@ -62,26 +60,31 @@
             error_builder=error_builder,
             node_impl=_PythonReferenceServiceStubSourceNode
         )
 
     def __call__(self, *args, __pre_resolved_types__: dict[TypeVar, HgTypeMetaData] = None,
                  **kwargs) -> "WiringPort":
         with WiringContext(current_wiring_node=self, current_signature=self.signature):
-            kwargs_, resolved_signature = self._validate_and_resolve_signature(*args,
+            kwargs_, resolved_signature, resolution_dict = self._validate_and_resolve_signature(*args,
                                                                                __pre_resolved_types__=__pre_resolved_types__,
                                                                                **kwargs)
 
-            port = super().__call__(*args, __pre_resolved_types__=__pre_resolved_types__, **kwargs)
+            typed_full_path = self.typed_full_path(kwargs_.get("path"), resolution_dict)
+            port = super().__call__(__pre_resolved_types__=__pre_resolved_types__, **(kwargs_ | {'path': typed_full_path}))
 
             from hgraph import WiringGraphContext
-            WiringGraphContext.instance().register_service_client(self, self.full_path(kwargs_.get("path")))
+            WiringGraphContext.instance().register_service_client(self, self.full_path(kwargs_.get("path")), resolution_dict or None)
 
             return port
 
-    def wire_impl_out_stub(self, path, out):
+    def wire_impl_out_stub(self, path, out, __pre_resolved_types__=None):
         from hgraph.nodes import capture_output_to_global_state
         from hgraph import WiringGraphContext
 
-        full_path = self.full_path(path)
-        capture_output_to_global_state(full_path, out)
+        typed_full_path = self.typed_full_path(path, self.signature.try_build_resolution_dict(__pre_resolved_types__))
+        capture_output_to_global_state(typed_full_path, out)
+
+        WiringGraphContext.instance().add_built_service_impl(typed_full_path, None)
 
-        WiringGraphContext.instance().add_built_service_impl(full_path, None)
+    def register_impl(self, path: str, impl: "NodeBuilder", __pre_resolved_types__: dict[TypeVar, HgTypeMetaData] = None):
+        from hgraph import register_service
+        register_service(path, impl, self.signature.try_build_resolution_dict(__pre_resolved_types__))
```

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_req_repl_service_node_service.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_req_repl_service_node_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,58 +20,61 @@
         if user_path is None:
             user_path = f"{self.fn.__module__}"
         return f"reqrepl_svc://{user_path}/{self.fn.__name__}"
 
     def __call__(self, *args, __pre_resolved_types__: dict[TypeVar, HgTypeMetaData | Callable] = None, **kwargs) -> "WiringPort":
 
         with WiringContext(current_wiring_node=self, current_signature=self.signature):
-            kwargs_, resolved_signature = self._validate_and_resolve_signature(*args,
-                                                                               __pre_resolved_types__=__pre_resolved_types__,
-                                                                               **kwargs)
+            kwargs_, resolved_signature, resolution_dict = self._validate_and_resolve_signature(
+                *args,
+                __pre_resolved_types__=__pre_resolved_types__,
+                **kwargs)
 
             # But graph nodes are evaluated at wiring time, so this is the graph expansion happening here!
             with WiringGraphContext(self.signature) as g:
+                typed_full_path = self.typed_full_path(kwargs_.get("path"), resolution_dict)
                 full_path = self.full_path(kwargs_.get("path"))
-                g.register_service_client(self, full_path)
+                g.register_service_client(self, full_path, resolution_dict or None)
 
                 from hgraph.nodes._service_utils import _request_service
                 from hgraph.nodes._service_utils import _request_reply_service
                 from hgraph import TIME_SERIES_TYPE_1
 
                 ts_kwargs = {k: v for k, v in kwargs_.items() if k in resolved_signature.time_series_args}
                 if resolved_signature.output_type is not None:
                     return _request_reply_service[TIME_SERIES_TYPE_1: resolved_signature.output_type](
-                        path=full_path,
+                        path=typed_full_path,
                         request=TSB[ts_schema(**resolved_signature.time_series_inputs)].from_ts(**ts_kwargs))
                 else:
                     return _request_service(
-                        path=full_path,
+                        path=typed_full_path,
                         request=TSB[ts_schema(**resolved_signature.time_series_inputs)].from_ts(**ts_kwargs))
 
-    def wire_impl_inputs_stub(self, path):
+    def wire_impl_inputs_stub(self, path, __pre_resolved_types__: dict[TypeVar, HgTypeMetaData | Callable] = None):
         from hgraph.nodes import get_shared_reference_output
 
-        full_path = self.full_path(path)
+        typed_full_path = self.typed_full_path(path, self.signature.try_build_resolution_dict(__pre_resolved_types__))
 
         request_tps = {}
         requests = {}
         for arg in self.signature.time_series_args:
-            interface_tp = self.signature.input_types[arg]
+            interface_tp = self.signature.input_types[arg].resolve(resolution_dict=__pre_resolved_types__)
             request_tps[arg] = TSD[int, interface_tp.py_type]
-            requests[arg] = get_shared_reference_output[TIME_SERIES_TYPE: request_tps[arg]](f"{full_path}_request_{arg}_out")
+            requests[arg] = get_shared_reference_output[TIME_SERIES_TYPE: request_tps[arg]](f"{typed_full_path}/request_{arg}_out")
 
-        WiringGraphContext.instance().add_built_service_impl(full_path, None)
+        WiringGraphContext.instance().add_built_service_impl(typed_full_path, None)
 
         return TSB[ts_schema(**request_tps)].from_ts(**requests)
 
-    def wire_impl_out_stub(self, path, out):
+    def wire_impl_out_stub(self, path, out, __pre_resolved_types__=None):
         from hgraph.nodes import write_service_replies
-        write_service_replies(self.full_path(path), out)
+        write_service_replies(self.typed_full_path(path, self.signature.try_build_resolution_dict(__pre_resolved_types__)), out)
 
-    @cached_property
-    def impl_signature(self):
+    def impl_signature(self, __pre_resolved_types__: dict[TypeVar, HgTypeMetaData | Callable] = None):
+        resolution_dict = self.signature.try_build_resolution_dict(__pre_resolved_types__)
         return self.signature.copy_with(
             input_types=frozendict(
-                {k: HgTypeMetaData.parse_type(TSD[int, v]) for k, v in self.signature.time_series_inputs.items()}
+                {k: HgTypeMetaData.parse_type(TSD[int, v.resolve(resolution_dict)]) for k, v in self.signature.time_series_inputs.items()}
                 | self.signature.scalar_inputs),
-            output_type=HgTypeMetaData.parse_type(TSD[int, self.signature.output_type.py_type]) if self.signature.output_type else None
+            output_type=HgTypeMetaData.parse_type(
+                TSD[int, self.signature.output_type.resolve(resolution_dict).py_type]) if self.signature.output_type else None
         )
```

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_service_impl_node_class.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_service_impl_node_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Mapping, Any, Sequence, TypeVar, Dict
 
 from frozendict import frozendict
 
-from hgraph import TIME_SERIES_TYPE
+from hgraph import TIME_SERIES_TYPE, graph
 from hgraph._builder._graph_builder import GraphBuilder
 from hgraph._runtime._global_state import GlobalState
 from hgraph._types._scalar_type_meta_data import HgAtomicType, HgObjectType
 from hgraph._types._tss_meta_data import HgTSSTypeMetaData
 from hgraph._types._type_meta_data import HgTypeMetaData
 from hgraph._wiring._graph_builder import create_graph_builder
 from hgraph._wiring._wiring_context import WiringContext
@@ -46,23 +46,18 @@
         if not isinstance(interfaces, (tuple, list, set)):
             interfaces = (interfaces,)
         self.interfaces = tuple(interfaces)
 
         # Ensure the service impl signature is valid given the signature definitions of the interfaces.
         validate_signature_vs_interfaces(signature, fn, interfaces)
 
-    def _validate_service_not_already_bound(self, path: str | None):
-        paths = [interface.full_path(path) for interface in self.interfaces]
-        gs = GlobalState.instance()
-        if any(p in gs for p in paths):
+    def _validate_service_not_already_bound(self, path: str | None, __pre_resolved_types__: dict[TypeVar, HgTypeMetaData | Callable] = None):
+        if WiringGraphContext.instance().is_service_built(path, __pre_resolved_types__):
             raise CustomMessageWiringError(
                 f"This path: '{path}' has already been registered for this service implementation")
-        # Reserve the paths now
-        for p in paths:
-            gs[p] = self  # use this as a placeholder until we have built the node
 
     def __call__(self, *args, __pre_resolved_types__: dict[TypeVar, HgTypeMetaData | Callable] = None,
                  __interface__: WiringNodeSignature = None,
                  **kwargs) -> "WiringPort":
 
         with WiringContext(current_wiring_node=self, current_signature=self._original_signature):
             path = kwargs.get("path")
@@ -72,30 +67,30 @@
 
             if not __interface__.is_full_path(path):
                 full_path = __interface__.full_path(path)
             else:
                 full_path = path
                 path = __interface__.path_from_full_path(full_path)
 
-            self._validate_service_not_already_bound(full_path)
+            self._validate_service_not_already_bound(full_path, __pre_resolved_types__)
             kwargs["path"] = path
 
             # TODO: This is only going to resolve scalars or output values, we need to
             # take a look at resolving the actual signature if there are pre-resolved-types.
-            kwargs_, resolved_signature = self._validate_and_resolve_signature(
+            kwargs_, resolved_signature, resolution_dict = self._validate_and_resolve_signature(
                 *args,
                 __pre_resolved_types__=__pre_resolved_types__,
                 **kwargs)
 
             resolved_signature = resolved_signature.copy_with(input_types=frozendict({
                         **resolved_signature.input_types,
                         'inner_graph': HgObjectType.parse_type(object)}))
 
             with WiringContext(current_wiring_node=self, current_signature=self.signature):
-                inner_graph, paths = create_inner_graph(self._original_signature, self.fn, kwargs_, self.interfaces)
+                inner_graph, paths = create_inner_graph(self._original_signature, self.fn, kwargs_, self.interfaces, resolution_dict)
                 kwargs_['inner_graph'] = inner_graph
 
             # We pass in rank of -1 because service implementations are ranked at the end of the graph build
             wiring_node_instance = create_wiring_node_instance(self, resolved_signature,
                                                                frozendict(kwargs_), rank=-1)
 
             for p in paths:
@@ -168,130 +163,132 @@
             case _:
                 raise CustomMessageWiringError(f"Unknown service type: {interface_sig.node_type}")
     else:
         pass # multiservice implementations use the interface stub APIs to wire up the service so checking happens there
 
 
 def create_inner_graph(wiring_signature: WiringNodeSignature, fn: Callable, scalars: Mapping[str, Any],
-                       interfaces: list[WiringNodeSignature]) -> (GraphBuilder, [str]):
+                       interfaces: list[WiringNodeSignature], resolution_dict: dict[TypeVar, HgTypeMetaData] = None) -> (GraphBuilder, [str]):
     if len(interfaces) == 1:
         s: WiringNodeSignature = interfaces[0].signature
         match s.node_type:
             case WiringNodeType.REF_SVC:
-                return wire_reference_data_service(wiring_signature, fn, scalars, interfaces[0])
+                return wire_reference_data_service(wiring_signature, fn, scalars, interfaces[0], resolution_dict)
             case WiringNodeType.SUBS_SVC:
-                return wire_subscription_service(wiring_signature, fn, scalars, interfaces[0])
+                return wire_subscription_service(wiring_signature, fn, scalars, interfaces[0], resolution_dict)
             case WiringNodeType.REQ_REP_SVC:
-                return wire_request_reply_service(wiring_signature, fn, scalars, interfaces[0])
+                return wire_request_reply_service(wiring_signature, fn, scalars, interfaces[0], resolution_dict)
             case _:
                 raise CustomMessageWiringError(f"Unknown service type: {s.node_type}")
     else:
         with WiringGraphContext(None) as context:
-            graph = wire_multi_service(fn, scalars)
+            graph, final_resolution_dict = wire_multi_service(fn, scalars)
             for path, node in context.built_services().items():
                 if node:
                     raise CustomMessageWiringError(f"Mitliservice implementations should not be registering service nodes")
 
                 s: WiringNodeClass = context.find_service_impl(path)[0]
                 match s.signature.node_type:
                     case WiringNodeType.REF_SVC: # reference service does not require external stubs
                         pass
                     case WiringNodeType.SUBS_SVC: # subscription service does not require external stubs
                         pass
                     case WiringNodeType.REQ_REP_SVC:
-                        wire_request_reply_service_stubs(s.impl_signature, path, s)
+                        wire_request_reply_service_stubs(s[final_resolution_dict].impl_signature(), path, s, final_resolution_dict)
                     case _:
                         raise CustomMessageWiringError(f"Unknown service type: {s.signature.node_type}")
 
             return graph, list(context.built_services().keys())
 
 
-def wire_multi_service(fn: Callable, scalars: Mapping[str, Any]):
+def wire_multi_service(fn: Callable, scalars: Mapping[str, Any], resolution_dict: dict[TypeVar, HgTypeMetaData] = None):
     with WiringNodeInstanceContext(), WiringGraphContext(None) as context:
-        fn(**scalars)
+        g = graph(fn)
+        _, _, final_resolution_dict = g._validate_and_resolve_signature(__pre_resolved_types__=resolution_dict, **scalars)
+        g[resolution_dict](**scalars)
         sink_nodes = context.pop_sink_nodes()
-        return create_graph_builder(sink_nodes, False)
+        return create_graph_builder(sink_nodes, False), final_resolution_dict
 
 
 def wire_subscription_service(wiring_signature: WiringNodeSignature, fn: Callable, scalars: Mapping[str, Any],
-                              interface):
+                              interface, resolution_dict=None) -> (GraphBuilder, [str]):
     path = (scalars := dict(scalars)).pop("path")
-    full_path = interface.full_path(path)
+    typed_full_path = interface.typed_full_path(path, resolution_dict)
 
     from hgraph._wiring._decorators import graph
-    from hgraph.nodes._service_utils import capture_output_to_global_state, capture_output_node_to_global_state
 
     @graph
     def subscription_service():
-        subscriptions = interface.wire_impl_inputs_stub(path)
+        subscriptions = interface[resolution_dict].wire_impl_inputs_stub(path)
         # Call the implementation graph with the scalars provided
-        out = fn(**(subscriptions.as_dict() | scalars))
-        interface.wire_impl_out_stub(path, out)
+        out = graph(fn)[resolution_dict](**(subscriptions.as_dict() | scalars))
+        interface[resolution_dict].wire_impl_out_stub(path, out)
 
     with WiringNodeInstanceContext(), WiringGraphContext(wiring_signature) as context:
         subscription_service()
         sink_nodes = context.pop_sink_nodes()
-        return create_graph_builder(sink_nodes, False), [full_path]
+        return create_graph_builder(sink_nodes, False), [typed_full_path]
 
 
-def wire_request_reply_service_stubs(wiring_signature: WiringNodeSignature, path, interface):
+def wire_request_reply_service_stubs(wiring_signature: WiringNodeSignature, typed_full_path, interface, resolution_dict=None):
     from hgraph.nodes._service_utils import capture_output_node_to_global_state, capture_output_to_global_state
 
     for arg in wiring_signature.time_series_args:
         tp = wiring_signature.input_types[arg]
-        request_node = last_value_source_node(f"{path}_request_{arg}", tp)
+        request_node = last_value_source_node(f"{typed_full_path}/request_{arg}", tp.resolve(resolution_dict))
         request = _wiring_port_for(tp, request_node, tuple())
-        capture_output_node_to_global_state(f"{path}_request_{arg}", request)
-        capture_output_to_global_state(f"{path}_request_{arg}_out", request)
+        capture_output_node_to_global_state(f"{typed_full_path}/request_{arg}", request)
+        capture_output_to_global_state(f"{typed_full_path}/request_{arg}_out", request)
 
     if wiring_signature.output_type is not None:
-        replies_node = last_value_source_node(f"{path}_replies_fb", wiring_signature.output_type)
-        replies = _wiring_port_for(tp, replies_node, tuple())
-        capture_output_node_to_global_state(f"{path}_replies_fb", replies)
-        capture_output_to_global_state(f"{path}_replies", replies)
+        replies_node = last_value_source_node(f"{typed_full_path}/replies_fb", wiring_signature.output_type.resolve(resolution_dict))
+        replies = _wiring_port_for(wiring_signature.output_type, replies_node, tuple())
+        capture_output_node_to_global_state(f"{typed_full_path}/replies_fb", replies)
+        capture_output_to_global_state(f"{typed_full_path}/replies", replies)
 
 
 def wire_request_reply_service(wiring_signature: WiringNodeSignature, fn: Callable, scalars: Mapping[str, Any],
-                              interface) -> (GraphBuilder, [str]):
+                              interface, resolution_dict) -> (GraphBuilder, [str]):
     path = (scalars := dict(scalars)).pop("path")
-    full_path = interface.full_path(path)
+    typed_full_path = interface.typed_full_path(path, resolution_dict)
 
-    wire_request_reply_service_stubs(wiring_signature, full_path, interface)
+    wire_request_reply_service_stubs(wiring_signature, typed_full_path, interface, resolution_dict)
 
     from hgraph._wiring._decorators import graph
 
     @graph
     def request_reply_service():
-        requests = interface.wire_impl_inputs_stub(path)
+        requests = interface[resolution_dict].wire_impl_inputs_stub(path)
         # Call the implementation graph with the scalars provided
-        out = fn(**(requests.as_dict() | scalars))
-        interface.wire_impl_out_stub(path, out)
+        out = graph(fn)[resolution_dict](**(requests.as_dict() | scalars))
+        interface[resolution_dict].wire_impl_out_stub(path, out)
 
     with WiringNodeInstanceContext(), WiringGraphContext(wiring_signature) as context:
         request_reply_service()
         sink_nodes = context.pop_sink_nodes()
-        return create_graph_builder(sink_nodes, False), [full_path]
+        return create_graph_builder(sink_nodes, False), [typed_full_path]
 
 
 def wire_reference_data_service(
         wiring_signature: WiringNodeSignature,
         fn: Callable,
         scalars: Mapping[str, Any],
-        interface) -> (GraphBuilder, [str]):
+        interface,
+        resolution_dict) -> (GraphBuilder, [str]):
     # The path was added to the scalars when initially wired to create the wiring node instance,
     # now we pop it off so that we can make use of both the scalars and the path.
     path = (scalars := dict(scalars)).pop("path")
-    full_path = interface.full_path(path)
+    typed_full_path = interface.typed_full_path(path, resolution_dict)
 
     from hgraph._wiring._decorators import graph
     from hgraph.nodes._service_utils import capture_output_to_global_state
 
     @graph
     def ref_svc_inner_graph():
         # Call the implementation graph with the scalars provided
-        out = fn(**scalars)
-        capture_output_to_global_state(full_path, out)
+        out = graph(fn)[resolution_dict](**scalars)
+        capture_output_to_global_state(typed_full_path, out)
 
     with WiringNodeInstanceContext(), WiringGraphContext(wiring_signature) as context:
         ref_svc_inner_graph()
         sink_nodes = context.pop_sink_nodes()
-        return create_graph_builder(sink_nodes, False), [full_path]
+        return create_graph_builder(sink_nodes, False), [typed_full_path]
```

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_stub_wiring_node_class.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_stub_wiring_node_class.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_subscription_service_node_service.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_subscription_service_node_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,51 +20,59 @@
         if not signature.defaults.get("path"):
             signature = signature.copy_with(defaults=frozendict(signature.defaults | {"path": None}))
         super().__init__(signature, fn)
         if (l := len(signature.time_series_args)) != 1:
             raise CustomMessageWiringError(f"Expected 1 time-series argument, got {l}")
         ts_type = signature.input_types[next(iter(signature.time_series_args))]
         if type(ts_type) is not HgTSTypeMetaData or not is_keyable_scalar(ts_type.value_scalar_tp.py_type):
-            raise CustomMessageWiringError("The subscription property must be a TS[KEYABLE_SCALAR]")
+            raise CustomMessageWiringError(f"The subscription property must be a TS[KEYABLE_SCALAR], {ts_type} is not")
 
     def full_path(self, user_path: str | None) -> str:
         if user_path is None:
             user_path = f"{self.fn.__module__}"
         return f"subs_svc://{user_path}/{self.fn.__name__}"
 
     def __call__(self, *args, __pre_resolved_types__: dict[TypeVar, HgTypeMetaData | Callable] = None, **kwargs) -> "WiringPort":
 
         with WiringContext(current_wiring_node=self, current_signature=self.signature):
-            kwargs_, resolved_signature = self._validate_and_resolve_signature(*args,
+            kwargs_, resolved_signature, resolution_dict = self._validate_and_resolve_signature(*args,
                                                                                __pre_resolved_types__=__pre_resolved_types__,
                                                                                **kwargs)
 
             # But graph nodes are evaluated at wiring time, so this is the graph expansion happening here!
             with WiringGraphContext(self.signature) as g:
+                typed_full_path = self.typed_full_path(kwargs_.get("path"), resolution_dict)
                 full_path = self.full_path(kwargs_.get("path"))
-                g.register_service_client(self, full_path)
+                g.register_service_client(self, full_path, resolution_dict)
 
                 from hgraph.nodes._service_utils import _subscribe
                 from hgraph import TIME_SERIES_TYPE
                 return _subscribe[TIME_SERIES_TYPE: resolved_signature.output_type](
-                    path=full_path,
+                    path=typed_full_path,
                     key=kwargs_[next(iter(resolved_signature.time_series_args))])
 
-    def wire_impl_inputs_stub(self, path):
+    def wire_impl_inputs_stub(self, path, __pre_resolved_types__: dict[TypeVar, HgTypeMetaData | Callable] = None):
         from hgraph.nodes import capture_output_node_to_global_state
         from hgraph import last_value_source_node, ts_schema
 
-        full_path = self.full_path(path)
+        resolution_dict = self.signature.try_build_resolution_dict(__pre_resolved_types__)
+        typed_path = self.typed_full_path(path, resolution_dict)
 
         arg = next(iter(self.signature.time_series_args))
         subscriptions = last_value_source_node(f"{self.signature.name}_{arg}",
-                                               (tp := TSS[self.signature.input_types[arg].scalar_type().py_type]))
+                                               (tp := TSS[self.signature.input_types[arg].resolve(resolution_dict).scalar_type().py_type]))
+        subscriptions.set_label(f"{typed_path}/inputs/{arg}")
         subscriptions = _wiring_port_for(tp, subscriptions, tuple())
-        capture_output_node_to_global_state(f"{full_path}_subs", subscriptions)
+        capture_output_node_to_global_state(f"{typed_path}/subs", subscriptions)
 
-        WiringGraphContext.instance().add_built_service_impl(full_path, None)
+        WiringGraphContext.instance().add_built_service_impl(typed_path, None)
 
         return TSB[ts_schema(**{arg: HgTypeMetaData.parse_type(tp)})].from_ts(**{arg: subscriptions})
 
-    def wire_impl_out_stub(self, path, out):
+    def wire_impl_out_stub(self, path, out, __pre_resolved_types__=None):
         from hgraph.nodes import capture_output_to_global_state
-        capture_output_to_global_state(f"{self.full_path(path)}_out", out)
+        capture_output_to_global_state(
+            f"{self.typed_full_path(path, self.signature.try_build_resolution_dict(__pre_resolved_types__))}/out", out)
+
+    def register_impl(self, path: str, impl: "NodeBuilder", __pre_resolved_types__: dict[TypeVar, HgTypeMetaData] = None):
+        from hgraph import register_service
+        register_service(path, impl, self.signature.try_build_resolution_dict(__pre_resolved_types__))
```

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_switch_wiring_node.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_switch_wiring_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_try_except_wiring_node.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_try_except_wiring_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_wiring_node_class.py` & `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_wiring_node_class.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,18 @@
     def __init__(self, signature: WiringNodeSignature, fn: Callable):
         self.signature: WiringNodeSignature = signature
         self.fn: Callable = fn
 
     def __call__(self, *args, **kwargs) -> "WiringNodeInstance":
         raise NotImplementedError()
 
-    def _convert_item(self, item) -> dict[TypeVar, HgTypeMetaData | Callable]:
+    @staticmethod
+    def _convert_item(item) -> dict[TypeVar, HgTypeMetaData | Callable]:
+        if isinstance(item, dict):
+            item = tuple(slice(k, v) for k, v in item.items())
         if isinstance(item, slice):
             item = (item,)  # Normalise all items into a tuple
         out = {}
         for s in item:
             assert s.step is None, f"Signature of type resolution is incorrect, expect TypeVar: Type, ... got {s}"
             assert s.start is not None, f"Signature of type resolution is incorrect, expect TypeVar: Type, ... got {s}"
             assert s.stop is not None, "signature of type resolution is incorrect, None is not a valid type"
@@ -118,15 +121,15 @@
                     k not in kwargs_}
     if _ensure_match and any(arg not in kwargs_ for arg in signature.args):
         raise SyntaxError(f"[{signature.signature}] Has incorrect kwargs names "
                           f"{[arg for arg in kwargs_ if arg not in signature.args]} "
                           f"expected: {[arg for arg in signature.args if arg not in kwargs_]}")
     # Filter kwargs to ensure only valid keys are present, this will also align the order of kwargs with args.
     kwargs_ = {k: kwargs_[k] for k in signature.args if k in kwargs_}
-    if len(kwargs_) < len(signature.args) - _args_offset:
+    if _ensure_match and len(kwargs_) < len(signature.args) - _args_offset:
         raise MissingInputsError(kwargs_)
     return kwargs_
 
 
 def prepare_kwargs(signature: WiringNodeSignature, *args, _ignore_defaults: bool = False, **kwargs) -> dict[str, Any]:
     """
     Extract the args and kwargs, apply defaults and validate the input shape as correct.
@@ -149,114 +152,64 @@
     def overload(self, other: "WiringNodeClass"):
         if getattr(self, "overload_list", None) is None:
             self.overload_list = OverloadedWiringNodeHelper(self)
 
         self.overload_list.overload(other)
 
     def __getitem__(self, item) -> WiringNodeClass:
-        return PreResolvedWiringNodeWrapper(signature=self.signature, fn=self.fn,
-                                            underlying_node=self, resolved_types=self._convert_item(item))
+        if item:
+            return PreResolvedWiringNodeWrapper(signature=self.signature, fn=self.fn,
+                                                underlying_node=self, resolved_types=self._convert_item(item))
+        else:
+            return self
 
     def _prepare_kwargs(self, *args, **kwargs) -> dict[str, Any]:
         """
         Extract the args and kwargs, apply defaults and validate the input shape as correct.
         This does not validate the types, just that all args are provided.
         """
         kwargs_ = prepare_kwargs(self.signature, *args, **kwargs)
         return kwargs_
 
-    def _convert_kwargs_to_types(self, **kwargs) -> dict[str, HgTypeMetaData]:
-        """Attempt to convert input types to better support type resolution"""
-        # We only need to extract un-resolved values
-        kwarg_types = {}
-        for k, v in self.signature.input_types.items():
-            with WiringContext(current_arg=k):
-                arg = kwargs.get(k, self.signature.defaults.get(k))
-                if arg is None:
-                    if v.is_injectable:
-                        # For injectables we expect the value to be None, and the type must already be resolved.
-                        kwarg_types[k] = v
-                    else:
-                        # We should wire in a null source
-                        if k in self.signature.defaults:
-                            kwarg_types[k] = v
-                        else:
-                            raise CustomMessageWiringError(
-                                f"Argument '{k}' is not marked as optional, but no value was supplied")
-                if k in filter(lambda k_: k_ in self.signature.time_series_args, self.signature.args):
-                    # This should then get a wiring node, and we would like to extract the output type,
-                    # But this is optional, so we should ensure that the type is present
-                    if arg is None:
-                        continue  # We will wire in a null source later
-                    if not isinstance(arg, WiringPort):
-                        tp = HgScalarTypeMetaData.parse_value(arg)
-                        kwarg_types[k] = tp
-                    elif arg.output_type:
-                        kwarg_types[k] = arg.output_type
-                    else:
-                        raise ParseError(
-                            f'{k}: {v} = {arg}, argument supplied is not a valid source or compute_node output')
-                elif type(v) is HgTypeOfTypeMetaData:
-                    if not isinstance(arg, (type, GenericAlias, _GenericAlias, TypeVar)) and arg is not AUTO_RESOLVE:
-                        # This is not a type of something (Have seen this as being an instance of HgTypeMetaData)
-                        raise IncorrectTypeBinding(v, arg)
-                    v = HgTypeMetaData.parse_type(arg) if arg is not AUTO_RESOLVE else v.value_tp
-                    kwarg_types[k] = HgTypeOfTypeMetaData(v)
-                else:
-                    if arg is None:
-                        kwarg_types[k] = v
-                    else:
-                        tp = HgScalarTypeMetaData.parse_value(arg)
-                        kwarg_types[k] = tp
-                        if tp is None:
-                            if k in self.signature.unresolved_args:
-                                raise ParseError(f"In {self.signature.name}, {k}: {v} = {arg}; arg is not parsable, "
-                                                 f"but we require type resolution")
-                            else:
-                                # If the signature was not unresolved, then we can use the signature, but the input value
-                                # May yet be incorrectly typed.
-                                kwarg_types[k] = v
-        return kwarg_types
-
     def resolve_signature(self, *args, __pre_resolved_types__: dict[TypeVar, HgTypeMetaData | Callable] = None,
                           **kwargs) -> "WiringNodeSignature":
-        _, resolved_signature = self._validate_and_resolve_signature(*args,
+        _, resolved_signature, _ = self._validate_and_resolve_signature(*args,
                                                                      __pre_resolved_types__=__pre_resolved_types__,
                                                                      **kwargs)
         return resolved_signature
 
     def _validate_and_resolve_signature(self, *args,
                                         __pre_resolved_types__: dict[TypeVar, HgTypeMetaData | Callable],
                                         __enforce_output_type__: bool = True,
                                         **kwargs) \
-            -> tuple[dict[str, Any], WiringNodeSignature]:
+            -> tuple[dict[str, Any], WiringNodeSignature, dict[TypeVar, HgTypeMetaData]]:
         """
         Insure the inputs wired in match the signature of this node and resolve any missing types.
         """
         # Validate that all inputs have been received and apply the defaults.
         record_replay_id = kwargs.pop("__record_id__", None)
         kwargs = self._prepare_kwargs(*args, **kwargs)
         WiringContext.current_kwargs = kwargs
         try:
             # Extract any additional required type resolution information from inputs
-            kwarg_types = self._convert_kwargs_to_types(**kwargs)
+            kwarg_types = self.signature.convert_kwargs_to_types(**kwargs)
             # Do the resolve to ensure types match as well as actually resolve the types.
             resolution_dict = self.signature.build_resolution_dict(__pre_resolved_types__, kwarg_types, kwargs)
             resolved_inputs = self.signature.resolve_inputs(resolution_dict)
             resolved_output = self.signature.resolve_output(resolution_dict, weak=not __enforce_output_type__)
             valid_inputs = self.signature.resolve_valid_inputs(**kwargs)
             all_valid_inputs = self.signature.resolve_all_valid_inputs(**kwargs)
             resolved_inputs = self.signature.resolve_auto_resolve_kwargs(resolution_dict, kwarg_types, kwargs,
                                                                          resolved_inputs)
 
             if self.signature.is_resolved:
                 self.signature.resolve_auto_const_and_type_kwargs(kwarg_types, kwargs)
                 self.signature.validate_resolved_types(kwarg_types, kwargs)
                 return kwargs, self.signature if record_replay_id is None else self.signature.copy_with(
-                    record_and_replay_id=record_replay_id)
+                    record_and_replay_id=record_replay_id), resolution_dict
             else:
                 # Only need to re-create if we actually resolved the signature.
                 resolve_signature = WiringNodeSignature(
                     node_type=self.signature.node_type,
                     name=self.signature.name,
                     args=self.signature.args,
                     defaults=self.signature.defaults,
@@ -271,15 +224,15 @@
                     injectable_inputs=self.signature.injectable_inputs,  # This should not differ based on resolution
                     label=self.signature.label,
                     record_and_replay_id=record_replay_id
                 )
                 if resolve_signature.is_resolved and __enforce_output_type__ or resolve_signature.is_weakly_resolved:
                     resolve_signature.resolve_auto_const_and_type_kwargs(kwarg_types, kwargs)
                     self.signature.validate_resolved_types(kwarg_types, kwargs)
-                    return kwargs, resolve_signature
+                    return kwargs, resolve_signature, resolution_dict
                 else:
                     raise WiringError(f"{resolve_signature.name} was not able to resolve itself")
         except Exception as e:
             if isinstance(e, WiringError):
                 raise e
             from hgraph._wiring._wiring_node_class._graph_wiring_node_class import WiringGraphContext
             path = '\n'.join(str(p) for p in WiringGraphContext.wiring_path())
@@ -302,15 +255,15 @@
         found_overload, r = self._check_overloads(*args, **kwargs, __pre_resolved_types__=__pre_resolved_types__)
         if found_overload:
             return r
 
         # TODO: Capture the call site information (line number / file etc.) for better error reporting.
         with WiringContext(current_wiring_node=self, current_signature=self.signature):
             # Now validate types and resolve any un-resolved types and provide an updated signature.
-            kwargs_, resolved_signature = self._validate_and_resolve_signature(*args,
+            kwargs_, resolved_signature, _ = self._validate_and_resolve_signature(*args,
                                                                                __pre_resolved_types__=__pre_resolved_types__,
                                                                                **kwargs)
 
             # TODO: This mechanism to work out rank may fail when using a delayed binding?
             match resolved_signature.node_type:
                 case WiringNodeType.PUSH_SOURCE_NODE:
                     rank = 0
@@ -405,17 +358,29 @@
     def __call__(self, *args, **kwargs) -> "WiringPort":
         more_resolved_types = kwargs.pop('__pre_resolved_types__', None) or {}
         return self.underlying_node(*args,
                                     __pre_resolved_types__={**self.resolved_types, **more_resolved_types},
                                     **kwargs)
 
     def __getitem__(self, item):
-        return PreResolvedWiringNodeWrapper(signature=self.underlying_node.signature, fn=self.fn,
-                                            underlying_node=self.underlying_node,
-                                            resolved_types={**self.resolved_types, **self._convert_item(item)})
+        if item:
+            return PreResolvedWiringNodeWrapper(signature=self.underlying_node.signature, fn=self.fn,
+                                                underlying_node=self.underlying_node,
+                                                resolved_types={**self.resolved_types, **self._convert_item(item)})
+        else:
+            return self
+
+    def __getattr__(self, item):
+        if (fn := getattr(self.underlying_node, item)) is not None and inspect.ismethod(fn):
+            if '__pre_resolved_types__' in inspect.signature(fn).parameters:
+                return lambda *args, **kwargs: fn(*args, **kwargs, __pre_resolved_types__=self.resolved_types)
+            else:
+                return lambda *args, **kwargs: fn(*args, **kwargs)
+
+        raise AttributeError(f"Attribute {item} not found on {self.underlying_node}")
 
 
 class OverloadedWiringNodeHelper:
     """
     This meta wiring node class deals with graph/node declaration overloads, for example when we have an implementation
     of a node that is generic
```

### Comparing `hgraph-0.2.7/src/hgraph/nodes/__init__.py` & `hgraph-0.2.8/src/hgraph/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_analytical.py` & `hgraph-0.2.8/src/hgraph/nodes/_analytical.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_compound_scalar_operators.py` & `hgraph-0.2.8/src/hgraph/nodes/_compound_scalar_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_conditional.py` & `hgraph-0.2.8/src/hgraph/nodes/_conditional.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_const.py` & `hgraph-0.2.8/src/hgraph/nodes/_const.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_data_source_polars.py` & `hgraph-0.2.8/src/hgraph/nodes/_data_source_polars.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_datetime_operators.py` & `hgraph-0.2.8/src/hgraph/nodes/_datetime_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_format.py` & `hgraph-0.2.8/src/hgraph/nodes/_format.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_frame_operators.py` & `hgraph-0.2.8/src/hgraph/nodes/_frame_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_math.py` & `hgraph-0.2.8/src/hgraph/nodes/_math.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_numpy.py` & `hgraph-0.2.8/src/hgraph/nodes/_numpy.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_operators.py` & `hgraph-0.2.8/src/hgraph/nodes/_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_print.py` & `hgraph-0.2.8/src/hgraph/nodes/_print.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_record.py` & `hgraph-0.2.8/src/hgraph/nodes/_record.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_replay.py` & `hgraph-0.2.8/src/hgraph/nodes/_replay.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_service_utils.py` & `hgraph-0.2.8/src/hgraph/nodes/_service_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 @sink_node
 def write_subscription_key(path: str, key: TS[SCALAR], _state: STATE = None):
     """
     Updates a TSS attached to the path with the key provided.
     This will also ensure use the associated tracker to ensure that we don't update unless required and performs
     the appropriate reference counting.
     """
-    svc_node_in = GlobalState.instance().get(f"{path}_subs")
+    svc_node_in = GlobalState.instance().get(f"{path}/subs")
     (s := _state.tracker[(v := key.value)]).add(_state.subscription_id)
     set_delta = set()
     if _state.previous_key:
         (s_old := _state.tracker[_state.previous_key]).remove(_state.subscription_id)
         if not s_old:
             set_delta.add(Removed(_state.previous_key))
     _state.previous_key = v
@@ -76,36 +76,36 @@
 
 @write_subscription_key.stop
 def write_subscription_key_stop(path: str, _state: STATE):
     if key := _state.previous_key:
         (s := _state.tracker[key]).remove(_state.subscription_id)
         if not s:
             del _state.tracker[key]
-            if subs_in := GlobalState.instance().get(f"{path}_subs"):
+            if subs_in := GlobalState.instance().get(f"{path}/subs"):
                 subs_in.apply_value(Removed(key))
 
 
 @graph
 def _subscribe(path: str, key: TS[SCALAR], _s_tp: type[SCALAR] = AUTO_RESOLVE,
                _ts_tp: type[TIME_SERIES_TYPE] = AUTO_RESOLVE) -> TIME_SERIES_TYPE:
     """Implement the stub for subscription"""
     write_subscription_key(path, key)
-    out = get_shared_reference_output[TIME_SERIES_TYPE: TSD[_s_tp, _ts_tp]](f"{path}_out")
+    out = get_shared_reference_output[TIME_SERIES_TYPE: TSD[_s_tp, _ts_tp]](f"{path}/out")
     return out[key]
 
 
 @compute_node
 def write_service_request(path: str, request: TIME_SERIES_TYPE, _output: TS_OUT[int] = None, _state: STATE = None) -> \
         TS[int]:
     """
     Updates TSDs attached to the path with the data provided.
     """
     for arg, ts in request.items():
         if ts.modified:
-            svc_node_in = GlobalState.instance().get(f"{path}_request_{arg}")
+            svc_node_in = GlobalState.instance().get(f"{path}/request_{arg}")
             svc_node_in.apply_value({id(_state.requestor_id): ts.delta_value})
 
     if not _output.valid:
         return id(_state.requestor_id)
 
 
 @write_service_request.start
@@ -114,38 +114,38 @@
 
 
 @write_service_request.stop
 def write_service_request_stop(request: TIME_SERIES_TYPE, path: str, _state: STATE):
     if request.valid:
         for arg, i in request.items():
             if i.valid:
-                if svc_node_in := GlobalState.instance().get(f"{path}_request_{arg}"):
+                if svc_node_in := GlobalState.instance().get(f"{path}/request_{arg}"):
                     svc_node_in.apply_value({id(_state.requestor_id): REMOVE_IF_EXISTS})
 
 
 @sink_node
 def write_service_replies(path: str, response: TIME_SERIES_TYPE):
     """
     Updates TSDs attached to the path with the data provided.
     """
-    svc_node_in = GlobalState.instance().get(f"{path}_replies_fb")
+    svc_node_in = GlobalState.instance().get(f"{path}/replies_fb")
     svc_node_in.apply_value(response.delta_value)
 
 
 @graph
 def _request_service(path: str, request: TIME_SERIES_TYPE):
     null_sink(write_service_request(path, request))
 
 
 @graph
 def _request_reply_service(path: str, request: TIME_SERIES_TYPE,
                      tp_out: Type[TIME_SERIES_TYPE_1] = AUTO_RESOLVE) -> TIME_SERIES_TYPE_1:
     requestor_id = write_service_request(path, request)
     if tp_out:
-        out = get_shared_reference_output[TIME_SERIES_TYPE: TSD[int, tp_out]](f"{path}_replies")
+        out = get_shared_reference_output[TIME_SERIES_TYPE: TSD[int, tp_out]](f"{path}/replies")
         return out[requestor_id]
 
 
 class SharedReferenceNodeClass(BaseWiringNodeClass):
 
     def create_node_builder_instance(self, node_signature: "NodeSignature",
                                      scalars: Mapping[str, Any]) -> "NodeBuilder":
```

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_set_operators.py` & `hgraph-0.2.8/src/hgraph/nodes/_set_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_stream_operators.py` & `hgraph-0.2.8/src/hgraph/nodes/_stream_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_tsb_operators.py` & `hgraph-0.2.8/src/hgraph/nodes/_tsb_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_tsd_operators.py` & `hgraph-0.2.8/src/hgraph/nodes/_tsd_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_tsl_operators.py` & `hgraph-0.2.8/src/hgraph/nodes/_tsl_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_tss_operators.py` & `hgraph-0.2.8/src/hgraph/nodes/_tss_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_tuple_operators.py` & `hgraph-0.2.8/src/hgraph/nodes/_tuple_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/nodes/_window_operators.py` & `hgraph-0.2.8/src/hgraph/nodes/_window_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/test/_node_printer.py` & `hgraph-0.2.8/src/hgraph/test/_node_printer.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/test/_node_unit_tester.py` & `hgraph-0.2.8/src/hgraph/test/_node_unit_tester.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/src/hgraph/test/testing.md` & `hgraph-0.2.8/src/hgraph/test/testing.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/test_wiring.py` & `hgraph-0.2.8/tests/python/unit/hgraph/test_wiring.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_impl/_builder/test_graph_builder.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_impl/_builder/test_graph_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_impl/_runtime/test_graph_runner.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_impl/_runtime/test_graph_runner.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_impl/_runtime/test_record_replay.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_impl/_runtime/test_record_replay.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_runtime/test_feedback.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_runtime/test_feedback.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_runtime/test_scheduler.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_runtime/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_types/test_complex_types.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_types/test_complex_types.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_types/test_operator_rank.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_types/test_operator_rank.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_types/test_type_meta_data.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_types/test_type_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_types/test_type_meta_resolve.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_types/test_type_meta_resolve.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_auto_const.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_auto_const.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_auto_resolve.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_auto_resolve.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_de_dupping_of_nodes.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_de_dupping_of_nodes.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_decorators.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_dispatch.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_error_handling.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_generic_graphs.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_generic_graphs.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_map.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_map.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_overloads.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_overloads.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_ref.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_ref.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_switch.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_switch.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_tsb_wiring.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_tsb_wiring.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_tsd_wiring.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_tsd_wiring.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_tsl_wiring.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_tsl_wiring.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_tss.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_tss.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_wiring_node_signature.py` & `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_wiring_node_signature.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_analytical.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_analytical.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_compound_scalar_operators.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_compound_scalar_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_conditional.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_conditional.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_const.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_const.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_data_source_polars.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_data_source_polars.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_format.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_format.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_frame.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_frame.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_math.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_math.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_numpy.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_numpy.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_operators.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_push_queue.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_push_queue.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_recorder.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_recorder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_tsb_operators.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_tsb_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_tsd_operators.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_tsd_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_tsl_operators.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_tsl_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_tss_operators.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_tss_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_window_operators.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_window_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_wp_operators.py` & `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_wp_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/tests/python/unit/hgraph/test/test_node_printer.py` & `hgraph-0.2.8/tests/python/unit/hgraph/test/test_node_printer.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     captured = capsys.readouterr()
     lines = captured.out.splitlines()
     expected = iter([
         "Starting Graph",
         "not_.+Started node",
         "Started Graph",
         "Eval Start",
-        "not_.+True\[IN\]",
-        "not_.+False\[OUT\]",
+        "not_.+True\\[IN\\]",
+        "not_.+False\\[OUT\\]",
         "Eval Done",
         "Graph Stopping",
         "not_.+Stopped node"
         "Graph Stopped"
     ])
     expected_next = re.compile(next(expected))
     for line in expected:
```

### Comparing `hgraph-0.2.7/LICENSE` & `hgraph-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/README.md` & `hgraph-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/pyproject.toml` & `hgraph-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.7/PKG-INFO` & `hgraph-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hgraph
-Version: 0.2.7
+Version: 0.2.8
 Summary: A functional reactive engine
 Project-URL: Homepage, https://github.com/hhenson/hgraph
 Project-URL: Repository, https://github.com/hhenson/hgraph.git
 Author-email: Howard Henson <howard@henson.me.uk>
 License: MIT License
         
         Copyright (c) 2023 Howard Henson
```

