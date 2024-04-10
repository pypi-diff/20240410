# Comparing `tmp/mct-nightly-2.0.0.20240408.430.tar.gz` & `tmp/mct-nightly-2.0.0.20240409.404.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-nightly-2.0.0.20240408.430.tar", last modified: Mon Apr  8 00:04:31 2024, max compression
+gzip compressed data, was "mct-nightly-2.0.0.20240409.404.tar", last modified: Tue Apr  9 00:04:07 2024, max compression
```

## Comparing `mct-nightly-2.0.0.20240408.430.tar` & `mct-nightly-2.0.0.20240409.404.tar`

### file list

```diff
@@ -1,591 +1,591 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.325041 mct-nightly-2.0.0.20240408.430/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-08 00:03:53.000000 mct-nightly-2.0.0.20240408.430/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-04-08 00:04:31.325041 mct-nightly-2.0.0.20240408.430/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17988 2024-04-08 00:03:53.000000 mct-nightly-2.0.0.20240408.430/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.261041 mct-nightly-2.0.0.20240408.430/mct_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-04-08 00:04:31.000000 mct-nightly-2.0.0.20240408.430/mct_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    36229 2024-04-08 00:04:31.000000 mct-nightly-2.0.0.20240408.430/mct_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 00:04:31.000000 mct-nightly-2.0.0.20240408.430/mct_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-08 00:04:31.000000 mct-nightly-2.0.0.20240408.430/mct_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 00:04:31.000000 mct-nightly-2.0.0.20240408.430/mct_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.261041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-08 00:04:30.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.265041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.265041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.265041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/back2framework/base_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/base_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.265041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/collectors/base_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/collectors/histogram_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/collectors/mean_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/collectors/statistics_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.265041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/fusion/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/fusion/layer_fusing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.269041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38178 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/base_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    28492 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/base_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/functional_node.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4744 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/graph_matchers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/graph_searches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.269041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/memory_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/memory_graph/cut.py
--rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.269041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/hessian/hessian_info_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/hessian/hessian_info_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/hessian/trace_hessian_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.269041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/matchers/
--rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/matchers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3091 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/matchers/base_graph_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2210 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/matchers/base_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3706 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/matchers/edge_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1773 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/matchers/function.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2745 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/matchers/node_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/matchers/walk_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/memory_computation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.273041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)    37578 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.273041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.273041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/search_methods/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
--rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/model_builder_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/model_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/model_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.273041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/network_editors/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/network_editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/network_editors/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/network_editors/edit_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/network_editors/node_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.273041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/channels_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.277041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/importance_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.277041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/mask/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    19523 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/memory_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/prune_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/pruner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/pruning_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/pruning_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/pruning_section.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.277041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/core_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/debug_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
--rw-r--r--   0 runner    (1001) docker     (127)    26737 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.277041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18165 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)    41524 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantize_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.281041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/similarity_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.281041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.281041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29865 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.281041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/visualization/nn_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21951 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/graph_prep_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.285041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.285041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15567 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/custom_layer_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.285041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.289041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.289041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    29027 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/keras_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/keras_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.289041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.289041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.289041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.289041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/connectivity_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.289041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/nested_model/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/node_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/resource_utilization_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.289041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/tf_tensor_numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.289041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.293041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.293041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.293041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.293041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.297041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    38459 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.297041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.297041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.297041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/pytorch_device_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    26868 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.297041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.297041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/reader/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12626 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/reader/graph_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/reader/node_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.297041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/quantization_prep_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.297041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.301041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/data_generation_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/model_info_exctractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/optimization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.301041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    21539 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/keras_data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/model_info_exctractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.301041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/optimization_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/optimization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.301041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.301041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/optimization_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19085 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/optimization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20937 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/defaultdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.301041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.301041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.305041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.305041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.305041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.305041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.305041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.305041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.305041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/keras/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.305041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.305041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.309041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.309041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/common/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/common/gptq_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/common/gptq_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/common/gptq_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    17705 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/common/gptq_training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.309041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    18438 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13913 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.309041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.309041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.309041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.309041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15808 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    12430 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.313041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.313041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.313041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.313041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/pruning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.313041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/pruning/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/pruning/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/pruning/keras/pruning_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.313041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/pruning/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/pruning/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/pruning/pytorch/pruning_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.313041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/ptq/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/ptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.313041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/ptq/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/ptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/ptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.313041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/ptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/ptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/ptq/pytorch/quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/ptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.313041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.313041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/common/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/common/qat_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.313041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.317041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.317041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/lsq/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.317041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.317041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.317041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.317041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/lsq/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.317041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.317041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/immutable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.317041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.321041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.321041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.321041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.321041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.321041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.321041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.321041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.321041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.321041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.321041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.325041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.325041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.325041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.325041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.325041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.325041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:04:31.325041 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-08 00:03:54.000000 mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-08 00:04:31.325041 mct-nightly-2.0.0.20240408.430/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-08 00:04:30.000000 mct-nightly-2.0.0.20240408.430/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.408983 mct-nightly-2.0.0.20240409.404/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-04-09 00:04:07.408983 mct-nightly-2.0.0.20240409.404/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17988 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.340982 mct-nightly-2.0.0.20240409.404/mct_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-04-09 00:04:06.000000 mct-nightly-2.0.0.20240409.404/mct_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    36229 2024-04-09 00:04:07.000000 mct-nightly-2.0.0.20240409.404/mct_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:04:06.000000 mct-nightly-2.0.0.20240409.404/mct_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-09 00:04:06.000000 mct-nightly-2.0.0.20240409.404/mct_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-09 00:04:06.000000 mct-nightly-2.0.0.20240409.404/mct_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.340982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-09 00:04:04.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.340982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.340982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.340982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/back2framework/base_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/base_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.344982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/collectors/base_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/collectors/histogram_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/collectors/mean_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/collectors/statistics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.344982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/fusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/fusion/layer_fusing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.344982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38178 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28492 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/functional_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4744 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/graph_matchers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/graph_searches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.344982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/memory_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/memory_graph/cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.344982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/hessian/hessian_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/hessian/hessian_info_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/hessian/trace_hessian_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.348982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/matchers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/matchers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3091 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/matchers/base_graph_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2210 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/matchers/base_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3706 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/matchers/edge_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1773 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/matchers/function.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2745 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/matchers/node_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/matchers/walk_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/memory_computation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.348982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37578 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.348982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.348982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/search_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/model_builder_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/model_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/model_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.352982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/network_editors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/network_editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/network_editors/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/network_editors/edit_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/network_editors/node_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.352982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/channels_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.352982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/importance_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.352982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19523 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/memory_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/prune_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/pruner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/pruning_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/pruning_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/pruning_section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.356983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/core_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/debug_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26947 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.356983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18165 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41524 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantize_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.356983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/similarity_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.360983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.360983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29865 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.360983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/visualization/nn_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21951 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/graph_prep_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.364982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.364982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15567 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/custom_layer_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.364982 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.368983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.368983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29027 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/keras_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/keras_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.368983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.368983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.368983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.368983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/connectivity_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.372983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/nested_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/resource_utilization_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.372983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/tf_tensor_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.372983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.372983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.372983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.372983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.372983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.376983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38459 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.376983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.376983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.376983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/pytorch_device_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26868 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.380983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.380983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12626 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/reader/graph_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/reader/node_holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/reader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.380983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/quantization_prep_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.380983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.380983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/data_generation_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/model_info_exctractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/optimization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.380983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21539 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/keras_data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/model_info_exctractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.384983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/optimization_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/optimization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.384983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.384983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/optimization_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19085 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/optimization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20937 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/defaultdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.384983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.384983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.384983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.388983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.388983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.388983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.388983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.388983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.388983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/keras/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.388983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.388983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.388983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.392983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/common/gptq_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/common/gptq_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/common/gptq_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17705 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/common/gptq_training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.392983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18875 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14299 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.392983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.392983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.392983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.392983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16245 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.396983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.396983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.396983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.396983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/pruning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.396983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/pruning/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/pruning/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/pruning/keras/pruning_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.396983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/pruning/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/pruning/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/pruning/pytorch/pruning_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.396983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/ptq/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/ptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.396983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/ptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/ptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/ptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.396983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/ptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/ptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/ptq/pytorch/quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/ptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.396983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.396983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/common/qat_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.396983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.400983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.400983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/lsq/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.400983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.400983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.400983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.400983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/lsq/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.400983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.400983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/immutable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.400983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.404983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.404983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.404983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.404983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.404983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.404983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.404983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.404983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.404983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.408983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.408983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.408983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.408983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.408983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.408983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.408983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:04:07.408983 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-09 00:03:27.000000 mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 00:04:07.412983 mct-nightly-2.0.0.20240409.404/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-09 00:04:04.000000 mct-nightly-2.0.0.20240409.404/setup.py
```

### Comparing `mct-nightly-2.0.0.20240408.430/LICENSE.md` & `mct-nightly-2.0.0.20240409.404/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/PKG-INFO` & `mct-nightly-2.0.0.20240409.404/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 2.0.0.20240408.430
+Version: 2.0.0.20240409.404
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
```

### Comparing `mct-nightly-2.0.0.20240408.430/README.md` & `mct-nightly-2.0.0.20240409.404/README.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/mct_nightly.egg-info/PKG-INFO` & `mct-nightly-2.0.0.20240409.404/mct_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 2.0.0.20240408.430
+Version: 2.0.0.20240409.404
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
```

### Comparing `mct-nightly-2.0.0.20240408.430/mct_nightly.egg-info/SOURCES.txt` & `mct-nightly-2.0.0.20240409.404/mct_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 from model_compression_toolkit import qat
 from model_compression_toolkit import exporter
 from model_compression_toolkit import gptq
 from model_compression_toolkit import data_generation
 from model_compression_toolkit import pruning
 from model_compression_toolkit.trainable_infrastructure.keras.load_model import keras_load_quantized_model
 
-__version__ = "2.0.0.20240408.000430"
+__version__ = "2.0.0.20240409.000404"
```

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/constants.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/analyzer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/analyzer.py`

 * *Files 23% similar despite different names*

```diff
@@ -26,38 +26,48 @@
 
 from model_compression_toolkit.core.common.visualization.tensorboard_writer import TensorboardWriter
 from model_compression_toolkit.logger import Logger
 
 
 def analyzer_model_quantization(representative_data_gen: Callable,
                                 tb_w: TensorboardWriter,
-                                tg: Graph,
+                                float_graph: Graph,
+                                quantized_graph: Graph,
                                 fw_impl: FrameworkImplementation,
                                 fw_info: FrameworkInfo):
     """
     Plot the cosine similarity of different points on the graph between the float and quantized
     graphs. Add them to the passed TensorboardWriter object and close all tensorboard writer open
     files.
 
     Args:
         representative_data_gen: Dataset used for calibration.
         tb_w: TensorBoardWriter object to log events.
-        tg: Graph of quantized model.
+        float_graph: Graph of float model.
+        quantized_graph: Graph of quantized model.
         fw_impl: FrameworkImplementation object with a specific framework methods implementation.
         fw_info: Information needed for quantization about the specific framework.
 
     """
     if tb_w is not None:
-        visual = NNVisualizer(tg,
+        visual = NNVisualizer(float_graph,
+                              quantized_graph,
                               fw_impl=fw_impl,
                               fw_info=fw_info)
-
-        for i, _data in enumerate(representative_data_gen()):
-            if i >= NUM_SAMPLES_DISTANCE_TENSORBOARD:
-                break
-            figure = visual.plot_distance_graph(_data,
-                                                distance_fn=compute_cs,
-                                                convert_to_range=lambda a: 1 - 2 * a)
-            tb_w.add_figure(figure, f'similarity_distance_sample_{i}')
+        if not visual.has_compare_points():
+            Logger.error(f'No comparing points were found to plot analyze similarity.')
         else:
-            Logger.warning(f'Not enough batches in representative dataset to generate {NUM_SAMPLES_DISTANCE_TENSORBOARD} figures')
+            visualized_samples = 0
+            for _data in representative_data_gen():
+                batch_size = _data[0].shape[0]
+                for sample_index in range(batch_size):
+                    if visualized_samples >= NUM_SAMPLES_DISTANCE_TENSORBOARD:
+                        break
+                    figure = visual.plot_distance_graph(_data,
+                                                        sample_index=sample_index,
+                                                        distance_fn=compute_cs,
+                                                        convert_to_range=lambda a: 1 - 2 * a)
+                    tb_w.add_figure(figure, f'similarity_distance_sample_{visualized_samples}')
+                    visualized_samples += 1
+            if visualized_samples < NUM_SAMPLES_DISTANCE_TENSORBOARD:
+                Logger.error(f'Not enough batches in representative dataset to generate {NUM_SAMPLES_DISTANCE_TENSORBOARD} figures')
         tb_w.close()
```

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/back2framework/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/back2framework/base_model_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/back2framework/base_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/base_substitutions.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/base_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/collectors/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/collectors/base_collector.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/collectors/base_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/collectors/histogram_collector.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/collectors/histogram_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/collectors/mean_collector.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/collectors/mean_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/collectors/statistics_collector.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/collectors/statistics_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/framework_implementation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/framework_info.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/fusion/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/fusion/layer_fusing.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/fusion/layer_fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/base_graph.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/base_node.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/base_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/edge.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/edge.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/functional_node.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/functional_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/graph_matchers.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/graph_matchers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/graph_searches.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/graph_searches.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/memory_graph/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/memory_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/memory_graph/cut.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/memory_graph/cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/hessian/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/hessian/hessian_info_service.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/hessian/hessian_info_service.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/hessian/hessian_info_utils.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/hessian/hessian_info_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/hessian/trace_hessian_request.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/hessian/trace_hessian_request.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/matchers/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/matchers/base_graph_filter.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/matchers/base_graph_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/matchers/base_matcher.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/matchers/base_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/matchers/edge_matcher.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/matchers/edge_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/matchers/function.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/matchers/function.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/matchers/node_matcher.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/matchers/node_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/matchers/walk_matcher.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/matchers/walk_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/memory_computation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/memory_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/model_builder_mode.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/model_builder_mode.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/model_collector.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/model_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/model_validation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/network_editors/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/network_editors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/network_editors/actions.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/network_editors/actions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/network_editors/edit_network.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/network_editors/edit_network.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/network_editors/node_filters.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/network_editors/node_filters.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/node_prior_info.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/channels_grouping.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/channels_grouping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/mask/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/memory_calculator.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/memory_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/prune_graph.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/prune_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/pruner.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/pruner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/pruning_config.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/pruning_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/pruning_info.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/pruning_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/pruning/pruning_section.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/pruning/pruning_section.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/core_config.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/core_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/debug_config.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/debug_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/node_quantization_config.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/node_quantization_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,32 +37,32 @@
 
 
 class BaseNodeQuantizationConfig(object):
     """
     Base class for node quantization configuration
     """
 
-    def set_quant_config_attr(self, parameter_name: str, parameter_value: Any,
+    def set_quant_config_attr(self, config_parameter_name: str, config_parameter_value: Any,
                               *args: List[Any], **kwargs: Dict[str, Any]):
         """
         Changes a BaseNodeQuantizationConfig's parameter.
         Note that arg and kwargs are only to allow clean override in the child classes.
 
         Args:
-            parameter_name: parameter name to change.
-            parameter_value: parameter value to change.
+            config_parameter_name: parameter name to change.
+            config_parameter_value: parameter value to change.
             args: A list of additional arguments.
             kwargs: A dictionary with additional key arguments.
 
         """
 
-        if hasattr(self, parameter_name):
-            setattr(self, parameter_name, parameter_value)
+        if hasattr(self, config_parameter_name):
+            setattr(self, config_parameter_name, config_parameter_value)
         else:
-            Logger.warning(f"Parameter {parameter_name} could not be found in the node quantization config and "
+            Logger.warning(f"Parameter {config_parameter_name} could not be found in the node quantization config and "
                            f"was not updated!")
 
     def __repr__(self) -> str:
         """
         Returns: String to display a NodeQuantizationConfig object.
         """
         repr_str = ''
@@ -517,42 +517,43 @@
         """
         attrs_with_name = {k: v for k, v in self.attributes_config_mapping.items() if attr_name in k}
         if len(attrs_with_name) > 1:
             Logger.warning(f"Found multiple weight attributes containing the name {attr_name}: "
                            f"{list(attrs_with_name.keys())}.")
         return attrs_with_name
 
-    def set_quant_config_attr(self, parameter_name: str, parameter_value: Any, attr_name: str = None,
+    def set_quant_config_attr(self, config_parameter_name: str, config_parameter_value: Any, attr_name: str = None,
                               *args: List[Any], **kwargs: Dict[str, Any]):
         """
         This method overrides the parent class set_quant_config_attr to enable setting a specific weights
         attribute config parameter.
 
         Args:
             attr_name: attribute name to change.
-            parameter_name: parameter name to change.
-            parameter_value: parameter value to change.
+            config_parameter_name: parameter name to change.
+            config_parameter_value: parameter value to change.
             args: A list of additional arguments.
             kwargs: A dictionary with additional key arguments.
 
         """
 
         if attr_name is None:
-            super(NodeWeightsQuantizationConfig, self).set_quant_config_attr(parameter_name, parameter_value,
+            super(NodeWeightsQuantizationConfig, self).set_quant_config_attr(config_parameter_name,
+                                                                             config_parameter_value,
                                                                              *args, **kwargs)
         else:
             if self.has_attribute_config(attr_name):
                 attr_cfg = self.get_attr_config(attr_name)
-                if hasattr(attr_cfg, parameter_name):
-                    setattr(attr_cfg, parameter_name, parameter_value)
+                if hasattr(attr_cfg, config_parameter_name):
+                    setattr(attr_cfg, config_parameter_name, config_parameter_value)
                 else:
-                    Logger.warning(f"Parameter {parameter_name} could not be found in the node quantization config of "
+                    Logger.warning(f"Parameter {config_parameter_name} could not be found in the node quantization config of "
                                    f"weights attribute {attr_name} and was not updated!")
             else:
-                Logger.error(f"Weights attribute {attr_name} could not be found to set parameter {parameter_name}.")
+                Logger.error(f"Weights attribute {attr_name} could not be found to set parameter {config_parameter_name}.")
 
     def __eq__(self, other: Any) -> bool:
         """
         Compares the object to another object to find if they are equal.
 
         Args:
             other: An object to compare to.
```

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_config.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,36 +19,37 @@
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.quantization.quantize_node import get_quantized_weights_attr_by_qc
 from model_compression_toolkit.logger import Logger
 
 
-def quantize_graph_weights(graph: Graph) -> Graph:
+def quantize_graph_weights(graph_to_quantize: Graph) -> Graph:
     """
     Get a graph representing a model, and quantize its nodes' weights.
     Each node is quantized according to the passed framework info and quantization configuration.
     If weights bias correction is enabled in the quantization configuration, a bias correction term
     is calculated and subtracted from the original node's bias. The graph is quantized in-place.
 
     Args:
-        graph: Graph to quantize its nodes.
+        graph_to_quantize: Graph to quantize its nodes.
 
     """
+    _quantized_graph = copy.deepcopy(graph_to_quantize)
     # Iterate over nodes in the graph and quantize each node's weights and activations
     # (according to operators groups in framework info).
-    for n in graph.nodes():
+    for n in _quantized_graph.nodes():
         for attr in n.get_node_weights_attributes():
             if n.is_weights_quantization_enabled(attr):
                 quantized_attr, io_channels_axes = \
                     get_quantized_weights_attr_by_qc(attr,
                                                      n,
                                                      n.final_weights_quantization_cfg.get_attr_config(attr))
 
                 Logger.debug(
                     f'Weights attribute: {attr} of node name: {n.name} has the following quantization params: '
                     f'{str(n.final_weights_quantization_cfg.get_attr_config(attr).weights_quantization_params)}')
 
                 # Set the attribute to be the quantized attribute.
                 n.set_weights_by_keys(attr, quantized_attr)
 
-    return graph
+    return _quantized_graph
```

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantize_node.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantize_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantizers/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/similarity_analyzer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/similarity_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,18 @@
 
     error = np.abs(float_flat - fxp_flat).mean(axis=-1)
     if norm:
         error /= (np.abs(float_flat).mean(axis=-1) + norm_eps)
     return error
 
 
-def compute_cs(float_tensor: np.ndarray, fxp_tensor: np.ndarray, eps: float = 1e-8, batch: bool = False,
+def compute_cs(float_tensor: np.ndarray,
+               fxp_tensor: np.ndarray,
+               eps: float = 1e-8,
+               batch: bool = False,
                axis: int = None) -> float:
     """
     Compute the similarity between two tensor using cosine similarity.
     The returned values is between 0 to 1: the smaller returned value,
     the greater similarity there is between the two tensors.
 
     Args:
```

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/apply_substitutions.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/apply_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/user_info.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/user_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/visualization/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/visualization/final_config_visualizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/visualization/final_config_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/visualization/nn_visualizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/visualization/nn_visualizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+
 from typing import Tuple, List, Callable
 
 import numpy as np
 from matplotlib import pyplot as plt
 from matplotlib.figure import Figure
 
-from model_compression_toolkit.core.common.quantization.quantize_graph_weights import quantize_graph_weights
 from model_compression_toolkit.core.common import Graph
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 from model_compression_toolkit.core.common.model_builder_mode import ModelBuilderMode
 from model_compression_toolkit.core.common.similarity_analyzer import compute_cs
+from model_compression_toolkit.logger import Logger
 
 
 def _get_compare_points(input_graph: Graph) -> Tuple[List[BaseNode], List[str]]:
     """
     Create a list of nodes in a graph where we collect their output statistics, and a corresponding list
     of their names for tensors comparison purposes.
     Args:
@@ -53,81 +54,107 @@
     NNVisualizer can compare the two models outputs after each layer.
     The results can be displayed using plot_cs_graph by passing it an input image to use
     for inference of the models.
     """
 
     def __init__(self,
                  graph_float: Graph,
+                 graph_quantized: Graph,
                  fw_impl: FrameworkImplementation,
                  fw_info: FrameworkInfo):
         """
         Initialize a NNVisualizer object.
         Args:
             graph_float: Float version of the graph.
+            graph_quantized: Quantized version of the graph.
+            fw_impl: Framework implementation with framework-specific methods implementation.
+            fw_info: Framework info with framework-specific information.
 
         """
 
         self.graph_float = graph_float
-        self.graph_quantized = quantize_graph_weights(graph_float)
+        self.graph_quantized = graph_quantized
         self.fw_impl = fw_impl
         self.fw_info = fw_info
 
         # Get compare points of two graphs.
         self.compare_points, self.compare_points_name = _get_compare_points(self.graph_quantized)
         self.compare_points_float, self.compare_points_name_float = _get_compare_points(self.graph_float)
 
+        if len(self.compare_points) != len(self.compare_points_float):
+            Logger.critical(f"Number of compare points in float and quantized models must be equal but "
+                            f"num of quantized compare points: {len(self.compare_points)} and "
+                            f"num of float compare points: {len(self.compare_points_float)}")
+        if len(self.compare_points_name) != len(self.compare_points_name_float):
+            Logger.critical(f"Number of compare points in float and quantized models must be equal "
+                            f"but num of quantized compare points: {len(self.compare_points_name)}"
+                            f" and num of float compare points: "
+                            f"{len(self.compare_points_name_float)}")
+
         self.quantized_model, _ = self.fw_impl.model_builder(self.graph_quantized,
                                                              mode=ModelBuilderMode.QUANTIZED,
                                                              append2output=self.compare_points,
                                                              fw_info=self.fw_info)
 
         self.float_model, _ = self.fw_impl.model_builder(self.graph_float,
                                                          mode=ModelBuilderMode.FLOAT,
                                                          append2output=self.compare_points_float,
                                                          fw_info=self.fw_info)
 
+    def has_compare_points(self) -> bool:
+        """
+
+        Returns: Whether or not compare points were found.
+
+        """
+        return len(self.compare_points_float) > 0 and len(self.compare_points) > 0 and len(
+            self.compare_points_name_float) > 0 and len(self.compare_points_name) > 0
+
+
     def plot_distance_graph(self,
                             input_image: np.ndarray,
+                            sample_index: int,
                             distance_fn: Callable = compute_cs,
                             convert_to_range: Callable = lambda a: a) -> Figure:
         """
         Compare and plot the outputs of the quantized and the float versions
         of a neural network that KerasNNVisualizer has.
 
         Args:
             input_image: Image to use as input to the networks.
+            sample_index: The index of the sample from input_image to use for comparison.
             distance_fn: Distance function to calculate the distance between two tensors.
             convert_to_range: Optional function to move the distance values into a specific range, e.g., when using
                 cosine similarity for distance, use 'lambda a: 1 - 2 * a' to convert the distance values to the range
                 of [-1, 1].
 
         Returns:
             Figure of the distance per layer.
         """
 
         # To compare cosine similarity, we use a single image as input (per input),
         # to make the difference more noticeable when exists
         new_inputs = []
         for single_input in input_image:
-            img = single_input[0]
+            img = single_input[sample_index]
             new_inputs.append(np.expand_dims(img, axis=0))
 
         # Get outputs
         tensors_float = self.fw_impl.run_model_inference(self.float_model, new_inputs)
         tensors_fxp = self.fw_impl.run_model_inference(self.quantized_model, new_inputs)
 
         # Compute distance between couples of outputs.
         distance_array = np.asarray(
             [distance_fn(self.fw_impl.to_numpy(t_float), self.fw_impl.to_numpy(t_fxp)) for t_float, t_fxp in zip(tensors_float, tensors_fxp)])
 
         distance_array = convert_to_range(distance_array)
 
         # Display the result: distance at every layer's output.
         fig = plt.figure()
-        plt.plot(distance_array)
+        plt.plot(list(range(len(distance_array))), distance_array)
         eps = 0.5
         y_limits = (min(distance_array) - eps, max(distance_array) + eps)
         plt.ylim(y_limits)
         plt.grid()
         plt.xlabel('Layer')
         plt.ylabel('Distance')
         return fig
```

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/common/visualization/tensorboard_writer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/common/visualization/tensorboard_writer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/graph_prep_runner.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/graph_prep_runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/back2framework/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/back2framework/float_model_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/back2framework/instance_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/constants.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/custom_layer_validation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/custom_layer_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/default_framework_info.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/hessian/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/keras_implementation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/keras_model_validation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/keras_model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/keras_node_prior_info.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/keras_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/pruning/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/quantizer/base_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/quantizer/base_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/common.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/common.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/connectivity_handler.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/connectivity_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/nested_model/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/nested_model/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/node_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/node_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/reader/reader.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/resource_utilization_data_facade.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/resource_utilization_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/tf_tensor_numpy.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/tf_tensor_numpy.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/keras/visualization/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/keras/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/constants.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/default_framework_info.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/hessian/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/pruning/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/pytorch_device_config.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/pytorch_device_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/pytorch_implementation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/reader/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/reader/graph_builders.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/reader/graph_builders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/reader/node_holders.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/reader/node_holders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/reader/reader.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/pytorch/utils.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/quantization_prep_runner.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/quantization_prep_runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/core/runner.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/core/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/constants.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/data_generation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/data_generation_config.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/data_generation_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/enums.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/enums.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/image_pipeline.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/model_info_exctractors.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/common/optimization_utils.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/common/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/constants.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/image_pipeline.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/keras_data_generation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/keras_data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/model_info_exctractors.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/keras/optimization_utils.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/keras/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/constants.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/image_pipeline.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/optimization_utils.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/defaultdict.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/defaultdict.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/common/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/common/gptq_config.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/common/gptq_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/common/gptq_constants.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/common/gptq_constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/common/gptq_framework_implementation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/common/gptq_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/common/gptq_graph.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/common/gptq_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/common/gptq_training.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/common/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/gptq_loss.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/gptq_training.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/gptq_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,20 +333,24 @@
                     node = graph.find_node_by_name('_'.join(layer.layer.name.split('_')[3:]))
                 if len(node) != 1:
                     Logger.critical(f"Unable to update the GPTQ graph because the layer named '{layer.layer.name}' could not be found. "
                                     f"Verify that the layer names in the GPTQ model match those in the graph.")
                 node = node[0]
                 kernel_attribute = get_kernel_attribute_name_for_gptq(layer_type=node.type,
                                                                       fw_info=self.fw_info)
+                # TODO: only kernel attributes are currently trained in GPTQ, so only the kernel weights need to be updated.
+                #  To enable GPTQ for other attributes, this code needs to be modified.
                 weights, weight_quant_config, activation_quant_config = \
                     layer.weights_quantizers[kernel_attribute].update_layer_quantization_params(layer)
                 for weight_attr, weight in weights.items():
                     node.set_weights_by_keys(weight_attr, weight.numpy())
-                for config_attr, config_value in weight_quant_config.items():
-                    node.final_weights_quantization_cfg.set_quant_config_attr(config_attr, config_value)
+                for config_parameter_name, config_parameter_value in weight_quant_config.items():
+                    node.final_weights_quantization_cfg.set_quant_config_attr(config_parameter_name,
+                                                                              config_parameter_value,
+                                                                              attr_name=kernel_attribute)
                 for config_attr, config_value in activation_quant_config.items():
                     node.final_activation_quantization_cfg.set_quant_config_attr(config_attr, config_value)
                 if self.gptq_config.train_bias:
                     use_bias = layer.layer.get_config().get(USE_BIAS)
                     if use_bias is not None and use_bias:
                         new_bias = layer.layer.bias.numpy()
                         node.set_weights_by_keys(BIAS, new_bias)
```

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/graph_info.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantization_facade.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+import copy
 
 from typing import Callable, Tuple
 from packaging import version
 
+from model_compression_toolkit.core.common.quantization.quantize_graph_weights import quantize_graph_weights
 from model_compression_toolkit.core.common.visualization.tensorboard_writer import init_tensorboard_writer
 from model_compression_toolkit.gptq.common.gptq_constants import REG_DEFAULT
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import TENSORFLOW, FOUND_TF
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfig
 from model_compression_toolkit.core.common.mixed_precision.resource_utilization_tools.resource_utilization import ResourceUtilization
@@ -206,28 +208,35 @@
                                                                   core_config=core_config,
                                                                   fw_info=DEFAULT_KERAS_INFO,
                                                                   fw_impl=fw_impl,
                                                                   tpc=target_platform_capabilities,
                                                                   target_resource_utilization=target_resource_utilization,
                                                                   tb_w=tb_w)
 
+        float_graph = copy.deepcopy(tg)
+
         tg_gptq = gptq_runner(tg,
                               core_config,
                               gptq_config,
                               representative_data_gen,
                               gptq_representative_data_gen if gptq_representative_data_gen else representative_data_gen,
                               DEFAULT_KERAS_INFO,
                               fw_impl,
                               tb_w,
                               hessian_info_service=hessian_info_service)
 
         del hessian_info_service
 
         if core_config.debug_config.analyze_similarity:
-            analyzer_model_quantization(representative_data_gen, tb_w, tg_gptq, fw_impl, fw_info)
+            analyzer_model_quantization(representative_data_gen,
+                                        tb_w,
+                                        float_graph,
+                                        tg_gptq,
+                                        fw_impl,
+                                        DEFAULT_KERAS_INFO)
 
         return get_exportable_keras_model(tg_gptq)
 
 else:
     # If tensorflow is not installed,
     # we raise an exception when trying to use these functions.
     def get_keras_gptq_config(*args, **kwargs):
```

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/gptq_loss.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/gptq_training.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/gptq_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,20 +280,24 @@
                 node = self.graph_quant.find_node_by_name(name)
                 if len(node) != 1:
                     Logger.critical(f"Cannot update GPTQ graph: Layer with name '{name}' is missing or not unique. "
                                     f"Ensure each layer has a unique name and exists within the graph for updates.")
                 node = node[0]
                 kernel_attribute = get_kernel_attribute_name_for_gptq(layer_type=node.type,
                                                                       fw_info=self.fw_info)
+                # TODO: only kernel attributes are currently trained in GPTQ, so only the kernel weights need to be updated.
+                #  To enable GPTQ for other attributes, this code needs to be modified.
                 weights, weight_quant_config, activation_quant_config = \
                     layer.weights_quantizers[kernel_attribute].update_layer_quantization_params(layer)
                 for weight_attr, weight in weights.items():
                     node.set_weights_by_keys(weight_attr, self.fw_impl.to_numpy(weight))
-                for config_attr, config_value in weight_quant_config.items():
-                    node.final_weights_quantization_cfg.set_quant_config_attr(config_attr, config_value)
+                for config_parameter_name, config_parameter_value in weight_quant_config.items():
+                    node.final_weights_quantization_cfg.set_quant_config_attr(config_parameter_name,
+                                                                              config_parameter_value,
+                                                                              attr_name=kernel_attribute)
                 for config_attr, config_value in activation_quant_config.items():
                     node.final_activation_quantization_cfg.set_quant_config_attr(config_attr, config_value)
                 if self.gptq_config.train_bias and hasattr(layer.layer, BIAS):
                     node.set_weights_by_keys(BIAS, self.fw_impl.to_numpy(getattr(layer.layer, BIAS)))
 
         return graph_quant
```

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/graph_info.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantization_facade.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+import copy
+
 from typing import Callable
 from model_compression_toolkit.core import common
 from model_compression_toolkit.constants import FOUND_TORCH
 from model_compression_toolkit.core.common.visualization.tensorboard_writer import init_tensorboard_writer
 from model_compression_toolkit.gptq.common.gptq_constants import REG_DEFAULT
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import PYTORCH
@@ -173,14 +175,15 @@
                                                                      representative_data_gen=representative_data_gen,
                                                                      core_config=core_config,
                                                                      fw_info=DEFAULT_PYTORCH_INFO,
                                                                      fw_impl=fw_impl,
                                                                      tpc=target_platform_capabilities,
                                                                      target_resource_utilization=target_resource_utilization,
                                                                      tb_w=tb_w)
+        float_graph = copy.deepcopy(graph)
 
         # ---------------------- #
         # GPTQ Runner
         # ---------------------- #
         graph_gptq = gptq_runner(graph,
                                  core_config,
                                  gptq_config,
@@ -188,15 +191,20 @@
                                  gptq_representative_data_gen if gptq_representative_data_gen else representative_data_gen,
                                  DEFAULT_PYTORCH_INFO,
                                  fw_impl,
                                  tb_w,
                                  hessian_info_service=hessian_info_service)
 
         if core_config.debug_config.analyze_similarity:
-            analyzer_model_quantization(representative_data_gen, tb_w, graph_gptq, fw_impl, DEFAULT_PYTORCH_INFO)
+            analyzer_model_quantization(representative_data_gen,
+                                        tb_w,
+                                        float_graph,
+                                        graph_gptq,
+                                        fw_impl,
+                                        DEFAULT_PYTORCH_INFO)
 
         return get_exportable_pytorch_model(graph_gptq)
 
 
 else:
     # If torch is not installed,
     # we raise an exception when trying to use these functions.
```

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/gptq/runner.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/gptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/logger.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/logger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/pruning/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/pruning/keras/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/pruning/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/pruning/keras/pruning_facade.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/pruning/keras/pruning_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/pruning/pytorch/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/pruning/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/pruning/pytorch/pruning_facade.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/pruning/pytorch/pruning_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/ptq/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/ptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/ptq/keras/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/ptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/ptq/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/ptq/keras/quantization_facade.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+import copy
 
 from typing import Callable
 
 from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core.analyzer import analyzer_model_quantization
+from model_compression_toolkit.core.common.quantization.quantize_graph_weights import quantize_graph_weights
 from model_compression_toolkit.core.common.visualization.tensorboard_writer import init_tensorboard_writer
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import TENSORFLOW, FOUND_TF
 from model_compression_toolkit.core.common.mixed_precision.resource_utilization_tools.resource_utilization import ResourceUtilization
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfig
 from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import TargetPlatformCapabilities
@@ -118,16 +120,16 @@
 
         KerasModelValidation(model=in_model,
                              fw_info=fw_info).validate()
 
         if core_config.mixed_precision_enable:
             if not isinstance(core_config.mixed_precision_config, MixedPrecisionQuantizationConfig):
                 Logger.critical("Given quantization config to mixed-precision facade is not of type "
-                                    "MixedPrecisionQuantizationConfig. Please use keras_post_training_quantization "
-                                    "API, or pass a valid mixed precision configuration.")  # pragma: no cover
+                                "MixedPrecisionQuantizationConfig. Please use keras_post_training_quantization "
+                                "API, or pass a valid mixed precision configuration.")  # pragma: no cover
 
         tb_w = init_tensorboard_writer(fw_info)
 
         fw_impl = KerasImplementation()
 
         # Ignore returned hessian service as PTQ does not use it
         tg, bit_widths_config, _ = core_runner(in_model=in_model,
@@ -135,23 +137,38 @@
                                                core_config=core_config,
                                                fw_info=fw_info,
                                                fw_impl=fw_impl,
                                                tpc=target_platform_capabilities,
                                                target_resource_utilization=target_resource_utilization,
                                                tb_w=tb_w)
 
-        tg = ptq_runner(tg, representative_data_gen, core_config, fw_info, fw_impl, tb_w)
+        # At this point, tg is a graph that went through substitutions (such as BN folding) and is
+        # ready for quantization (namely, it holds quantization params, etc.) but the weights are
+        # not quantized yet. For this reason, we use it to create a graph that acts as a "float" graph
+        # for things like similarity analyzer (because the quantized and float graph should have the same
+        # architecture to find the appropriate compare points for similarity computation).
+        similarity_baseline_graph = copy.deepcopy(tg)
+
+        graph_with_stats_correction = ptq_runner(tg,
+                                                 representative_data_gen,
+                                                 core_config,
+                                                 fw_info,
+                                                 fw_impl,
+                                                 tb_w)
 
         if core_config.debug_config.analyze_similarity:
+            quantized_graph = quantize_graph_weights(graph_with_stats_correction)
             analyzer_model_quantization(representative_data_gen,
-                                        tb_w, tg,
+                                        tb_w,
+                                        similarity_baseline_graph,
+                                        quantized_graph,
                                         fw_impl,
                                         fw_info)
 
-        return get_exportable_keras_model(tg)
+        return get_exportable_keras_model(graph_with_stats_correction)
 
 
 
 else:
     # If tensorflow is not installed,
     # we raise an exception when trying to use these functions.
     def keras_post_training_quantization(*args, **kwargs):
```

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/ptq/pytorch/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/ptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/ptq/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/ptq/pytorch/quantization_facade.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,28 +8,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+import copy
+
 from typing import Callable
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.visualization.tensorboard_writer import init_tensorboard_writer
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import PYTORCH, FOUND_TORCH
 from model_compression_toolkit.target_platform_capabilities.target_platform import TargetPlatformCapabilities
 from model_compression_toolkit.core.common.mixed_precision.resource_utilization_tools.resource_utilization import ResourceUtilization
 from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfig
 from model_compression_toolkit.core.runner import core_runner
 from model_compression_toolkit.ptq.runner import ptq_runner
 from model_compression_toolkit.core.analyzer import analyzer_model_quantization
+from model_compression_toolkit.core.common.quantization.quantize_graph_weights import quantize_graph_weights
 
 
 if FOUND_TORCH:
     from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
     from model_compression_toolkit.core.pytorch.pytorch_implementation import PytorchImplementation
     from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
     from torch.nn import Module
@@ -86,45 +89,61 @@
             Set number of clibration iterations to 1:
 
             >>> import model_compression_toolkit as mct
             >>> quantized_module, quantization_info = mct.ptq.pytorch_post_training_quantization(module, repr_datagen)
 
         """
 
+        fw_info = DEFAULT_PYTORCH_INFO
+
         if core_config.mixed_precision_enable:
             if not isinstance(core_config.mixed_precision_config, MixedPrecisionQuantizationConfig):
                 Logger.critical("Given quantization config to mixed-precision facade is not of type "
-                             "MixedPrecisionQuantizationConfig. Please use "
-                             "pytorch_post_training_quantization API, or pass a valid mixed precision "
-                             "configuration.")  # pragma: no cover
+                                "MixedPrecisionQuantizationConfig. Please use "
+                                "pytorch_post_training_quantization API, or pass a valid mixed precision "
+                                "configuration.")  # pragma: no cover
 
-        tb_w = init_tensorboard_writer(DEFAULT_PYTORCH_INFO)
+        tb_w = init_tensorboard_writer(fw_info)
 
         fw_impl = PytorchImplementation()
 
         # Ignore hessian info service as it is not used here yet.
         tg, bit_widths_config, _ = core_runner(in_model=in_module,
                                                representative_data_gen=representative_data_gen,
                                                core_config=core_config,
-                                               fw_info=DEFAULT_PYTORCH_INFO,
+                                               fw_info=fw_info,
                                                fw_impl=fw_impl,
                                                tpc=target_platform_capabilities,
                                                target_resource_utilization=target_resource_utilization,
                                                tb_w=tb_w)
 
-        tg = ptq_runner(tg, representative_data_gen, core_config, DEFAULT_PYTORCH_INFO, fw_impl, tb_w)
+        # At this point, tg is a graph that went through substitutions (such as BN folding) and is
+        # ready for quantization (namely, it holds quantization params, etc.) but the weights are
+        # not quantized yet. For this reason, we use it to create a graph that acts as a "float" graph
+        # for things like similarity analyzer (because the quantized and float graph should have the same
+        # architecture to find the appropriate compare points for similarity computation).
+        similarity_baseline_graph = copy.deepcopy(tg)
+
+        graph_with_stats_correction = ptq_runner(tg,
+                                                 representative_data_gen,
+                                                 core_config,
+                                                 fw_info,
+                                                 fw_impl,
+                                                 tb_w)
 
         if core_config.debug_config.analyze_similarity:
+            quantized_graph = quantize_graph_weights(graph_with_stats_correction)
             analyzer_model_quantization(representative_data_gen,
                                         tb_w,
-                                        tg,
+                                        similarity_baseline_graph,
+                                        quantized_graph,
                                         fw_impl,
-                                        DEFAULT_PYTORCH_INFO)
+                                        fw_info)
 
-        return get_exportable_pytorch_model(tg)
+        return get_exportable_pytorch_model(graph_with_stats_correction)
 
 
 else:
     # If torch is not installed,
     # we raise an exception when trying to use these functions.
     def pytorch_post_training_quantization(*args, **kwargs):
         Logger.critical("PyTorch must be installed to use 'pytorch_post_training_quantization_experimental'. "
```

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/ptq/runner.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/ptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/common/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/common/qat_config.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/common/qat_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/constants.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/immutable.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/immutable.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/common/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/common/constants.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/keras/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/keras/load_model.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py` & `mct-nightly-2.0.0.20240409.404/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240408.430/setup.py` & `mct-nightly-2.0.0.20240409.404/setup.py`

 * *Files identical despite different names*

