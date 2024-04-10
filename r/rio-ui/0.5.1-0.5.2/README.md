# Comparing `tmp/rio_ui-0.5.1.tar.gz` & `tmp/rio_ui-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio_ui-0.5.1.tar", max compression
+gzip compressed data, was "rio_ui-0.5.2.tar", max compression
```

## Comparing `rio_ui-0.5.1.tar` & `rio_ui-0.5.2.tar`

### file list

```diff
@@ -1,198 +1,207 @@
--rw-r--r--   0        0        0    35149 2024-04-06 18:09:28.058340 rio_ui-0.5.1/LICENSE.txt
--rw-r--r--   0        0        0     2251 2024-04-08 17:33:45.089793 rio_ui-0.5.1/README.md
--rw-r--r--   0        0        0     2441 2024-04-08 18:47:07.327845 rio_ui-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      676 2024-04-08 18:37:44.149116 rio_ui-0.5.1/rio/__init__.py
--rw-r--r--   0        0        0       91 2024-04-06 18:09:28.078340 rio_ui-0.5.1/rio/__main__.py
--rw-r--r--   0        0        0    19306 2024-04-08 18:37:44.149116 rio_ui-0.5.1/rio/app.py
--rw-r--r--   0        0        0    31728 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/app_server.py
--rw-r--r--   0        0        0      233 2024-04-06 18:09:28.081673 rio_ui-0.5.1/rio/assets/hosted/README.md
--rw-r--r--   0        0        0   557380 2024-04-06 18:09:28.088340 rio_ui-0.5.1/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf
--rw-r--r--   0        0        0   401608 2024-04-06 18:09:28.091673 rio_ui-0.5.1/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf
--rw-r--r--   0        0        0   403724 2024-04-06 18:09:28.095007 rio_ui-0.5.1/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf
--rw-r--r--   0        0        0   556216 2024-04-06 18:09:28.098340 rio_ui-0.5.1/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf
--rw-r--r--   0        0        0     4449 2024-04-06 18:09:28.098340 rio_ui-0.5.1/rio/assets/hosted/fonts/Noto Sans/OFL.txt
--rw-r--r--   0        0        0    11560 2024-04-06 18:09:28.101673 rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   167336 2024-04-06 18:09:28.101673 rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2024-04-06 18:09:28.105007 rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2024-04-06 18:09:28.105007 rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   168260 2024-04-06 18:09:28.105007 rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0    11560 2024-04-06 18:09:28.098340 rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt
--rw-r--r--   0        0        0    87392 2024-04-06 18:09:28.098340 rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf
--rw-r--r--   0        0        0    94636 2024-04-06 18:09:28.101673 rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
--rw-r--r--   0        0        0    94372 2024-04-06 18:09:28.101673 rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf
--rw-r--r--   0        0        0    87236 2024-04-06 18:09:28.101673 rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf
--rw-r--r--   0        0        0    54189 2024-04-08 17:00:05.405088 rio_ui-0.5.1/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
--rw-r--r--   0        0        0    31665 2024-04-06 18:09:28.105007 rio_ui-0.5.1/rio/assets/hosted/rio-logos/rio-logo-square.png
--rw-r--r--   0        0        0  1081400 2024-04-07 20:27:02.369218 rio_ui-0.5.1/rio/assets/icon-sets/material.tar.xz
--rw-r--r--   0        0        0    15424 2024-04-07 21:06:13.848440 rio_ui-0.5.1/rio/assets/icon-sets/rio.tar.xz
--rw-r--r--   0        0        0     1096 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/assets/icon-sets/styling.tar.xz
--rw-r--r--   0        0        0     8798 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/assets.py
--rw-r--r--   0        0        0     3316 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/byte_serving.py
--rw-r--r--   0        0        0     7300 2024-04-07 08:57:25.471514 rio_ui-0.5.1/rio/cli/__init__.py
--rw-r--r--   0        0        0     2392 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/cli/cli_instance.py
--rw-r--r--   0        0        0     6642 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/cli/nice_traceback.py
--rw-r--r--   0        0        0    12019 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/cli/project.py
--rw-r--r--   0        0        0    11944 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/cli/project_setup.py
--rw-r--r--   0        0        0     4172 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/cli/rio_api.py
--rw-r--r--   0        0        0     2278 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/cli/rioignore.py
--rw-r--r--   0        0        0      107 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/cli/run_project/__init__.py
--rw-r--r--   0        0        0     5404 2024-04-08 16:50:31.798904 rio_ui-0.5.1/rio/cli/run_project/app_loading.py
--rw-r--r--   0        0        0    20827 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/cli/run_project/arbiter.py
--rw-r--r--   0        0        0     1656 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/cli/run_project/file_watcher_worker.py
--rw-r--r--   0        0        0      423 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/cli/run_project/run_models.py
--rw-r--r--   0        0        0      476 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/cli/run_project/run_utils.py
--rw-r--r--   0        0        0     3779 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/cli/run_project/uvicorn_worker.py
--rw-r--r--   0        0        0     2229 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/cli/run_project/webview_worker.py
--rw-r--r--   0        0        0     3982 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/cli/tomlconfig.py
--rw-r--r--   0        0        0    19597 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/color.py
--rw-r--r--   0        0        0     7924 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/common.py
--rw-r--r--   0        0        0     1641 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/components/__init__.py
--rw-r--r--   0        0        0     4459 2024-04-07 11:52:48.918024 rio_ui-0.5.1/rio/components/app_root.py
--rw-r--r--   0        0        0     4055 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/components/auto_form.py
--rw-r--r--   0        0        0     4744 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/components/banner.py
--rw-r--r--   0        0        0      889 2024-04-07 08:57:25.524848 rio_ui-0.5.1/rio/components/build_failed.py
--rw-r--r--   0        0        0    13342 2024-04-07 11:49:35.305610 rio_ui-0.5.1/rio/components/button.py
--rw-r--r--   0        0        0     5057 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/components/card.py
--rw-r--r--   0        0        0     1025 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/components/class_container.py
--rw-r--r--   0        0        0      352 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/components/code_explorer.py
--rw-r--r--   0        0        0     3724 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/components/color_picker.py
--rw-r--r--   0        0        0    25919 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/components/component.py
--rw-r--r--   0        0        0     1029 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/components/component_tree.py
--rw-r--r--   0        0        0     1218 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/components/container.py
--rw-r--r--   0        0        0      215 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/components/debugger_connector.py
--rw-r--r--   0        0        0     4067 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/components/devel_component.py
--rw-r--r--   0        0        0     3868 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/components/drawer.py
--rw-r--r--   0        0        0     6649 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/components/dropdown.py
--rw-r--r--   0        0        0     2707 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/components/flow_container.py
--rw-r--r--   0        0        0     5853 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/components/fundamental_component.py
--rw-r--r--   0        0        0     7053 2024-04-06 18:09:28.108340 rio_ui-0.5.1/rio/components/grid.py
--rw-r--r--   0        0        0      568 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/html.py
--rw-r--r--   0        0        0     7768 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/components/icon.py
--rw-r--r--   0        0        0     3662 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/image.py
--rw-r--r--   0        0        0    13092 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/key_event_listener.py
--rw-r--r--   0        0        0     2735 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/labeled_column.py
--rw-r--r--   0        0        0     8750 2024-04-07 11:33:00.334931 rio_ui-0.5.1/rio/components/linear_containers.py
--rw-r--r--   0        0        0     4464 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/link.py
--rw-r--r--   0        0        0    10146 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/components/list_items.py
--rw-r--r--   0        0        0     3312 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/list_view.py
--rw-r--r--   0        0        0     1357 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/components/markdown.py
--rw-r--r--   0        0        0     4903 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/media_player.py
--rw-r--r--   0        0        0     6842 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/mouse_event_listener.py
--rw-r--r--   0        0        0     5137 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/multi_line_text_input.py
--rw-r--r--   0        0        0     1415 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/node_input.py
--rw-r--r--   0        0        0     1419 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/node_output.py
--rw-r--r--   0        0        0     8457 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/number_input.py
--rw-r--r--   0        0        0     2183 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/overlay.py
--rw-r--r--   0        0        0     5053 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/components/page_view.py
--rw-r--r--   0        0        0     4945 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/plot.py
--rw-r--r--   0        0        0     3259 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/popup.py
--rw-r--r--   0        0        0      942 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/progress_bar.py
--rw-r--r--   0        0        0     3546 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/progress_circle.py
--rw-r--r--   0        0        0     4074 2024-04-07 08:57:25.541514 rio_ui-0.5.1/rio/components/rectangle.py
--rw-r--r--   0        0        0     3667 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/revealer.py
--rw-r--r--   0        0        0     1857 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/root_components.py
--rw-r--r--   0        0        0     1875 2024-04-07 11:33:12.028273 rio_ui-0.5.1/rio/components/scroll_container.py
--rw-r--r--   0        0        0     1180 2024-04-07 11:33:14.818276 rio_ui-0.5.1/rio/components/scroll_target.py
--rw-r--r--   0        0        0     1107 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/components/separator.py
--rw-r--r--   0        0        0     6099 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/slider.py
--rw-r--r--   0        0        0     3635 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/slideshow.py
--rw-r--r--   0        0        0     1435 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/spacer.py
--rw-r--r--   0        0        0     2547 2024-04-07 11:33:20.541614 rio_ui-0.5.1/rio/components/stack.py
--rw-r--r--   0        0        0     3140 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/switch.py
--rw-r--r--   0        0        0      846 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/switcher.py
--rw-r--r--   0        0        0     9216 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/switcher_bar.py
--rw-r--r--   0        0        0     2297 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/table.py
--rw-r--r--   0        0        0     2011 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/components/text.py
--rw-r--r--   0        0        0     5352 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/text_input.py
--rw-r--r--   0        0        0     1224 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/theme_context_switcher.py
--rw-r--r--   0        0        0     2847 2024-04-07 11:33:30.271622 rio_ui-0.5.1/rio/components/tooltip.py
--rw-r--r--   0        0        0      637 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/components/website.py
--rw-r--r--   0        0        0      123 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/cursor_style.py
--rw-r--r--   0        0        0     5840 2024-04-08 18:37:44.152450 rio_ui-0.5.1/rio/dataclass.py
--rw-r--r--   0        0        0       53 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/debug/__init__.py
--rw-r--r--   0        0        0       41 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/debug/client_side_debugger/__init__.py
--rw-r--r--   0        0        0    10077 2024-04-07 11:33:35.984959 rio_ui-0.5.1/rio/debug/client_side_debugger/component_details.py
--rw-r--r--   0        0        0     3566 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/debug/client_side_debugger/debugger.py
--rw-r--r--   0        0        0      790 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/debug/client_side_debugger/deploy_page.py
--rw-r--r--   0        0        0      777 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/debug/client_side_debugger/docs_page.py
--rw-r--r--   0        0        0    12239 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/debug/client_side_debugger/icons_page.py
--rw-r--r--   0        0        0     2369 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/debug/client_side_debugger/project_page.py
--rw-r--r--   0        0        0     2265 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/debug/client_side_debugger/sample_icons_grid.py
--rw-r--r--   0        0        0    16567 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/debug/client_side_debugger/theme_picker_page.py
--rw-r--r--   0        0        0     1058 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/debug/client_side_debugger/tree_page.py
--rw-r--r--   0        0        0     7224 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/debug/monkeypatches.py
--rw-r--r--   0        0        0        0 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/debug/stress_client/__init__.py
--rw-r--r--   0        0        0      666 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/debug/stress_client/stress_client.py
--rw-r--r--   0        0        0      567 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/debug/typing_utils.py
--rw-r--r--   0        0        0    14210 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/debug/validator.py
--rw-r--r--   0        0        0       52 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/docs/__init__.py
--rw-r--r--   0        0        0     4867 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/docs/custom.py
--rw-r--r--   0        0        0     1124 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/docs/models.py
--rw-r--r--   0        0        0    14587 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/docs/parsers.py
--rw-r--r--   0        0        0      960 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/errors.py
--rw-r--r--   0        0        0     3173 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/event.py
--rw-r--r--   0        0        0     6732 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/fills.py
--rw-r--r--   0        0        0   529182 2024-04-08 18:46:46.851183 rio_ui-0.5.1/rio/generated/index.html
--rw-r--r--   0        0        0      897 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/global_state.py
--rw-r--r--   0        0        0     9940 2024-04-07 11:32:34.208243 rio_ui-0.5.1/rio/icon_registry.py
--rw-r--r--   0        0        0     3500 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/inspection.py
--rw-r--r--   0        0        0     3625 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/maybes.py
--rw-r--r--   0        0        0     1531 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/patches_for_3rd_party_stuff.py
--rw-r--r--   0        0        0     7348 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/routing.py
--rw-r--r--   0        0        0      417 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/self_serializing.py
--rw-r--r--   0        0        0     8463 2024-04-06 18:09:28.111674 rio_ui-0.5.1/rio/serialization.py
--rw-r--r--   0        0        0    76894 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/session.py
--rw-r--r--   0        0        0     1395 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/README.md
--rw-r--r--   0        0        0    12292 2024-04-08 13:26:45.976064 rio_ui-0.5.1/rio/snippets/__init__.py
--rw-r--r--   0        0        0      167 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/__init__.py
--rw-r--r--   0        0        0   157984 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/assets/jane-doe.jpg
--rw-r--r--   0        0        0   181111 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/assets/john-doe.jpg
--rw-r--r--   0        0        0      153 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/components/__init__.py
--rw-r--r--   0        0        0     1042 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/components/about_me.py
--rw-r--r--   0        0        0     1225 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/components/contact.py
--rw-r--r--   0        0        0     3649 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/components/history.py
--rw-r--r--   0        0        0     2042 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/components/projects.py
--rw-r--r--   0        0        0      642 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/components/skill_bars.py
--rw-r--r--   0        0        0       42 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/pages/__init__.py
--rw-r--r--   0        0        0     4373 2024-04-07 11:49:46.858457 rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/pages/biography_page.py
--rw-r--r--   0        0        0      192 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/pages/biography_page_after_tutorial_4.py
--rw-r--r--   0        0        0     1318 2024-04-07 11:52:22.599157 rio_ui-0.5.1/rio/snippets/snippet-files/other-examples/simple_counter_app.py
--rw-r--r--   0        0        0      684 2024-04-06 18:08:52.814883 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
--rw-r--r--   0        0        0      863 2024-04-07 08:57:25.584848 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/__init__.py
--rw-r--r--   0        0        0      223 2024-04-07 08:57:25.591515 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
--rw-r--r--   0        0        0     1833 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
--rw-r--r--   0        0        0     1196 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
--rw-r--r--   0        0        0     3728 2024-04-08 18:37:44.155783 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
--rw-r--r--   0        0        0      517 2024-04-08 18:37:44.159116 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
--rw-r--r--   0        0        0     2227 2024-04-07 09:24:53.378316 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
--rw-r--r--   0        0        0      184 2024-04-07 18:38:03.958535 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
--rw-r--r--   0        0        0       32 2024-04-06 18:08:52.818216 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
--rw-r--r--   0        0        0     5823 2024-04-08 18:37:44.159116 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
--rw-r--r--   0        0        0     3344 2024-04-06 18:08:52.814883 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
--rw-r--r--   0        0        0        0 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Empty/README.md
--rw-r--r--   0        0        0        0 2024-04-07 08:44:19.156096 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Empty/__init__.py
--rw-r--r--   0        0        0       46 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Empty/components/__init__.py
--rw-r--r--   0        0        0      769 2024-04-07 09:08:53.709464 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Empty/components/sample_component.py
--rw-r--r--   0        0        0       98 2024-04-07 08:04:03.043617 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Empty/meta.json
--rw-r--r--   0        0        0        0 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
--rw-r--r--   0        0        0      495 2024-04-08 18:37:44.159116 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
--rw-r--r--   0        0        0     3344 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
--rw-r--r--   0        0        0        4 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Simple Dashboard/README.md
--rw-r--r--   0        0        0        0 2024-04-07 08:44:22.292774 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Simple Dashboard/__init__.py
--rw-r--r--   0        0        0   139537 2024-04-07 11:11:59.577096 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Simple Dashboard/assets/smartphone-sales-clean.csv
--rw-r--r--   0        0        0      123 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Simple Dashboard/meta.json
--rw-r--r--   0        0        0     3649 2024-04-07 11:48:59.185121 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Simple Dashboard/pages/interactive_plot.py
--rw-r--r--   0        0        0     3586 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Simple Dashboard/thumbnail.svg
--rw-r--r--   0        0        0      490 2024-04-08 13:25:22.132597 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
--rw-r--r--   0        0        0        0 2024-04-08 13:21:28.592126 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 12:55:14.311995 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
--rw-r--r--   0        0        0       92 2024-04-08 13:26:20.426025 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
--rw-r--r--   0        0        0       44 2024-04-08 15:32:19.997165 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
--rw-r--r--   0        0        0     5570 2024-04-08 18:37:44.159116 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0     3344 2024-04-08 13:24:10.679136 rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
--rw-r--r--   0        0        0     8134 2024-04-08 18:37:44.159116 rio_ui-0.5.1/rio/state_properties.py
--rw-r--r--   0        0        0     3077 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/text_style.py
--rw-r--r--   0        0        0    19418 2024-04-07 12:44:53.024638 rio_ui-0.5.1/rio/theme.py
--rw-r--r--   0        0        0     5167 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/user_settings_module.py
--rw-r--r--   0        0        0     3890 2024-04-06 18:09:28.115007 rio_ui-0.5.1/rio/world_units.py
--rw-r--r--   0        0        0     4762 1970-01-01 00:00:00.000000 rio_ui-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-06 18:09:28.058340 rio_ui-0.5.2/LICENSE.txt
+-rw-r--r--   0        0        0     5088 2024-04-10 18:36:10.559283 rio_ui-0.5.2/README.md
+-rw-r--r--   0        0        0     2441 2024-04-10 16:51:11.474556 rio_ui-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      676 2024-04-08 18:37:44.149116 rio_ui-0.5.2/rio/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-06 18:09:28.078340 rio_ui-0.5.2/rio/__main__.py
+-rw-r--r--   0        0        0    19313 2024-04-09 19:38:54.555684 rio_ui-0.5.2/rio/app.py
+-rw-r--r--   0        0        0    32013 2024-04-09 19:38:54.585684 rio_ui-0.5.2/rio/app_server.py
+-rw-r--r--   0        0        0      233 2024-04-06 18:09:28.081673 rio_ui-0.5.2/rio/assets/hosted/README.md
+-rw-r--r--   0        0        0   557380 2024-04-06 18:09:28.088340 rio_ui-0.5.2/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf
+-rw-r--r--   0        0        0   401608 2024-04-06 18:09:28.091673 rio_ui-0.5.2/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf
+-rw-r--r--   0        0        0   403724 2024-04-06 18:09:28.095007 rio_ui-0.5.2/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf
+-rw-r--r--   0        0        0   556216 2024-04-06 18:09:28.098340 rio_ui-0.5.2/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf
+-rw-r--r--   0        0        0     4449 2024-04-06 18:09:28.098340 rio_ui-0.5.2/rio/assets/hosted/fonts/Noto Sans/OFL.txt
+-rw-r--r--   0        0        0    11560 2024-04-06 18:09:28.101673 rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   167336 2024-04-06 18:09:28.101673 rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2024-04-06 18:09:28.105007 rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2024-04-06 18:09:28.105007 rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   168260 2024-04-06 18:09:28.105007 rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0    11560 2024-04-06 18:09:28.098340 rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt
+-rw-r--r--   0        0        0    87392 2024-04-06 18:09:28.098340 rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf
+-rw-r--r--   0        0        0    94636 2024-04-06 18:09:28.101673 rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
+-rw-r--r--   0        0        0    94372 2024-04-06 18:09:28.101673 rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf
+-rw-r--r--   0        0        0    87236 2024-04-06 18:09:28.101673 rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf
+-rw-r--r--   0        0        0    54189 2024-04-08 17:00:05.405088 rio_ui-0.5.2/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
+-rw-r--r--   0        0        0    31665 2024-04-06 18:09:28.105007 rio_ui-0.5.2/rio/assets/hosted/rio-logos/rio-logo-square.png
+-rw-r--r--   0        0        0  1081400 2024-04-07 20:27:02.369218 rio_ui-0.5.2/rio/assets/icon-sets/material.tar.xz
+-rw-r--r--   0        0        0    15424 2024-04-07 21:06:13.848440 rio_ui-0.5.2/rio/assets/icon-sets/rio.tar.xz
+-rw-r--r--   0        0        0     1096 2024-04-06 18:09:28.108340 rio_ui-0.5.2/rio/assets/icon-sets/styling.tar.xz
+-rw-r--r--   0        0        0     8798 2024-04-08 18:37:44.152450 rio_ui-0.5.2/rio/assets.py
+-rw-r--r--   0        0        0     3316 2024-04-06 18:09:28.108340 rio_ui-0.5.2/rio/byte_serving.py
+-rw-r--r--   0        0        0     7300 2024-04-07 08:57:25.471514 rio_ui-0.5.2/rio/cli/__init__.py
+-rw-r--r--   0        0        0     2392 2024-04-08 18:37:44.152450 rio_ui-0.5.2/rio/cli/cli_instance.py
+-rw-r--r--   0        0        0     6642 2024-04-06 18:09:28.108340 rio_ui-0.5.2/rio/cli/nice_traceback.py
+-rw-r--r--   0        0        0    12019 2024-04-06 18:09:28.108340 rio_ui-0.5.2/rio/cli/project.py
+-rw-r--r--   0        0        0    11944 2024-04-08 18:37:44.152450 rio_ui-0.5.2/rio/cli/project_setup.py
+-rw-r--r--   0        0        0     4172 2024-04-08 18:37:44.152450 rio_ui-0.5.2/rio/cli/rio_api.py
+-rw-r--r--   0        0        0     2278 2024-04-08 18:37:44.152450 rio_ui-0.5.2/rio/cli/rioignore.py
+-rw-r--r--   0        0        0      107 2024-04-06 18:09:28.108340 rio_ui-0.5.2/rio/cli/run_project/__init__.py
+-rw-r--r--   0        0        0     5404 2024-04-08 16:50:31.798904 rio_ui-0.5.2/rio/cli/run_project/app_loading.py
+-rw-r--r--   0        0        0    20827 2024-04-08 18:37:44.152450 rio_ui-0.5.2/rio/cli/run_project/arbiter.py
+-rw-r--r--   0        0        0     1656 2024-04-06 18:09:28.108340 rio_ui-0.5.2/rio/cli/run_project/file_watcher_worker.py
+-rw-r--r--   0        0        0      423 2024-04-06 18:09:28.108340 rio_ui-0.5.2/rio/cli/run_project/run_models.py
+-rw-r--r--   0        0        0      476 2024-04-08 18:37:44.152450 rio_ui-0.5.2/rio/cli/run_project/run_utils.py
+-rw-r--r--   0        0        0     3779 2024-04-06 18:09:28.108340 rio_ui-0.5.2/rio/cli/run_project/uvicorn_worker.py
+-rw-r--r--   0        0        0     2229 2024-04-06 18:09:28.108340 rio_ui-0.5.2/rio/cli/run_project/webview_worker.py
+-rw-r--r--   0        0        0     3982 2024-04-08 18:37:44.152450 rio_ui-0.5.2/rio/cli/tomlconfig.py
+-rw-r--r--   0        0        0    19604 2024-04-09 19:38:54.559018 rio_ui-0.5.2/rio/color.py
+-rw-r--r--   0        0        0     7924 2024-04-08 18:37:44.152450 rio_ui-0.5.2/rio/common.py
+-rw-r--r--   0        0        0     1552 2024-04-10 18:34:30.899371 rio_ui-0.5.2/rio/components/__init__.py
+-rw-r--r--   0        0        0     4469 2024-04-10 16:49:08.291150 rio_ui-0.5.2/rio/components/app_root.py
+-rw-r--r--   0        0        0     4055 2024-04-08 18:37:44.152450 rio_ui-0.5.2/rio/components/auto_form.py
+-rw-r--r--   0        0        0     4751 2024-04-09 19:38:54.559018 rio_ui-0.5.2/rio/components/banner.py
+-rw-r--r--   0        0        0      889 2024-04-07 08:57:25.524848 rio_ui-0.5.2/rio/components/build_failed.py
+-rw-r--r--   0        0        0    13356 2024-04-09 19:38:54.559018 rio_ui-0.5.2/rio/components/button.py
+-rw-r--r--   0        0        0     5064 2024-04-09 19:38:54.559018 rio_ui-0.5.2/rio/components/card.py
+-rw-r--r--   0        0        0     1025 2024-04-06 18:09:28.108340 rio_ui-0.5.2/rio/components/class_container.py
+-rw-r--r--   0        0        0      352 2024-04-06 18:09:28.108340 rio_ui-0.5.2/rio/components/code_explorer.py
+-rw-r--r--   0        0        0     3745 2024-04-09 19:38:54.559018 rio_ui-0.5.2/rio/components/color_picker.py
+-rw-r--r--   0        0        0    26039 2024-04-10 17:00:38.844482 rio_ui-0.5.2/rio/components/component.py
+-rw-r--r--   0        0        0     1029 2024-04-06 18:09:28.108340 rio_ui-0.5.2/rio/components/component_tree.py
+-rw-r--r--   0        0        0     1225 2024-04-09 19:38:54.562351 rio_ui-0.5.2/rio/components/container.py
+-rw-r--r--   0        0        0      215 2024-04-06 18:09:28.108340 rio_ui-0.5.2/rio/components/debugger_connector.py
+-rw-r--r--   0        0        0     4067 2024-04-06 18:09:28.108340 rio_ui-0.5.2/rio/components/devel_component.py
+-rw-r--r--   0        0        0     3889 2024-04-09 19:38:54.562351 rio_ui-0.5.2/rio/components/drawer.py
+-rw-r--r--   0        0        0     6670 2024-04-09 19:38:54.562351 rio_ui-0.5.2/rio/components/dropdown.py
+-rw-r--r--   0        0        0     2922 2024-04-09 19:38:54.562351 rio_ui-0.5.2/rio/components/flow_container.py
+-rw-r--r--   0        0        0     5867 2024-04-10 17:00:38.844482 rio_ui-0.5.2/rio/components/fundamental_component.py
+-rw-r--r--   0        0        0     7057 2024-04-09 19:38:54.562351 rio_ui-0.5.2/rio/components/grid.py
+-rw-r--r--   0        0        0      604 2024-04-09 19:38:54.562351 rio_ui-0.5.2/rio/components/html.py
+-rw-r--r--   0        0        0     7782 2024-04-09 19:38:54.562351 rio_ui-0.5.2/rio/components/icon.py
+-rw-r--r--   0        0        0     3676 2024-04-09 19:38:54.562351 rio_ui-0.5.2/rio/components/image.py
+-rw-r--r--   0        0        0    13127 2024-04-09 19:38:54.565684 rio_ui-0.5.2/rio/components/key_event_listener.py
+-rw-r--r--   0        0        0     2981 2024-04-10 16:49:08.291150 rio_ui-0.5.2/rio/components/labeled_column.py
+-rw-r--r--   0        0        0     8968 2024-04-09 19:38:54.585684 rio_ui-0.5.2/rio/components/linear_containers.py
+-rw-r--r--   0        0        0     4478 2024-04-09 19:38:54.565684 rio_ui-0.5.2/rio/components/link.py
+-rw-r--r--   0        0        0    10196 2024-04-10 16:49:08.291150 rio_ui-0.5.2/rio/components/list_items.py
+-rw-r--r--   0        0        0     3527 2024-04-09 19:38:54.565684 rio_ui-0.5.2/rio/components/list_view.py
+-rw-r--r--   0        0        0     1389 2024-04-09 19:38:54.565684 rio_ui-0.5.2/rio/components/markdown.py
+-rw-r--r--   0        0        0     4917 2024-04-09 19:38:54.565684 rio_ui-0.5.2/rio/components/media_player.py
+-rw-r--r--   0        0        0     6919 2024-04-09 19:38:54.565684 rio_ui-0.5.2/rio/components/mouse_event_listener.py
+-rw-r--r--   0        0        0     5165 2024-04-09 19:38:54.569018 rio_ui-0.5.2/rio/components/multi_line_text_input.py
+-rw-r--r--   0        0        0     1422 2024-04-09 19:38:54.569018 rio_ui-0.5.2/rio/components/node_input.py
+-rw-r--r--   0        0        0     1426 2024-04-09 19:38:54.569018 rio_ui-0.5.2/rio/components/node_output.py
+-rw-r--r--   0        0        0     8478 2024-04-09 19:38:54.569018 rio_ui-0.5.2/rio/components/number_input.py
+-rw-r--r--   0        0        0     2190 2024-04-09 19:38:54.569018 rio_ui-0.5.2/rio/components/overlay.py
+-rw-r--r--   0        0        0     5060 2024-04-09 19:38:54.569018 rio_ui-0.5.2/rio/components/page_view.py
+-rw-r--r--   0        0        0     4959 2024-04-09 19:38:54.569018 rio_ui-0.5.2/rio/components/plot.py
+-rw-r--r--   0        0        0     3280 2024-04-09 19:38:54.569018 rio_ui-0.5.2/rio/components/popup.py
+-rw-r--r--   0        0        0      975 2024-04-09 19:38:54.569018 rio_ui-0.5.2/rio/components/progress_bar.py
+-rw-r--r--   0        0        0     3560 2024-04-09 19:38:54.569018 rio_ui-0.5.2/rio/components/progress_circle.py
+-rw-r--r--   0        0        0     4106 2024-04-09 19:38:54.569018 rio_ui-0.5.2/rio/components/rectangle.py
+-rw-r--r--   0        0        0     3688 2024-04-09 19:38:54.572351 rio_ui-0.5.2/rio/components/revealer.py
+-rw-r--r--   0        0        0     1857 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/components/root_components.py
+-rw-r--r--   0        0        0     1889 2024-04-09 19:38:54.572351 rio_ui-0.5.2/rio/components/scroll_container.py
+-rw-r--r--   0        0        0     1213 2024-04-09 19:38:54.572351 rio_ui-0.5.2/rio/components/scroll_target.py
+-rw-r--r--   0        0        0     1114 2024-04-09 19:38:54.572351 rio_ui-0.5.2/rio/components/separator.py
+-rw-r--r--   0        0        0     6120 2024-04-09 19:38:54.572351 rio_ui-0.5.2/rio/components/slider.py
+-rw-r--r--   0        0        0     3649 2024-04-09 19:38:54.572351 rio_ui-0.5.2/rio/components/slideshow.py
+-rw-r--r--   0        0        0     1442 2024-04-09 19:38:54.572351 rio_ui-0.5.2/rio/components/spacer.py
+-rw-r--r--   0        0        0     2762 2024-04-09 19:38:54.572351 rio_ui-0.5.2/rio/components/stack.py
+-rw-r--r--   0        0        0     3154 2024-04-09 19:38:54.572351 rio_ui-0.5.2/rio/components/switch.py
+-rw-r--r--   0        0        0      879 2024-04-09 19:38:54.572351 rio_ui-0.5.2/rio/components/switcher.py
+-rw-r--r--   0        0        0     9237 2024-04-09 19:38:54.572351 rio_ui-0.5.2/rio/components/switcher_bar.py
+-rw-r--r--   0        0        0     2305 2024-04-09 19:38:54.572351 rio_ui-0.5.2/rio/components/table.py
+-rw-r--r--   0        0        0     2018 2024-04-09 19:38:54.575684 rio_ui-0.5.2/rio/components/text.py
+-rw-r--r--   0        0        0     5380 2024-04-09 19:38:54.575684 rio_ui-0.5.2/rio/components/text_input.py
+-rw-r--r--   0        0        0     1231 2024-04-09 19:38:54.575684 rio_ui-0.5.2/rio/components/theme_context_switcher.py
+-rw-r--r--   0        0        0     2861 2024-04-09 19:38:54.575684 rio_ui-0.5.2/rio/components/tooltip.py
+-rw-r--r--   0        0        0      633 2024-04-09 19:38:54.575684 rio_ui-0.5.2/rio/components/website.py
+-rw-r--r--   0        0        0      123 2024-04-08 18:37:44.152450 rio_ui-0.5.2/rio/cursor_style.py
+-rw-r--r--   0        0        0     5840 2024-04-08 18:37:44.152450 rio_ui-0.5.2/rio/dataclass.py
+-rw-r--r--   0        0        0       53 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/debug/__init__.py
+-rw-r--r--   0        0        0       41 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/debug/client_side_debugger/__init__.py
+-rw-r--r--   0        0        0    10121 2024-04-10 16:49:08.291150 rio_ui-0.5.2/rio/debug/client_side_debugger/component_details.py
+-rw-r--r--   0        0        0     3634 2024-04-10 18:34:30.899371 rio_ui-0.5.2/rio/debug/client_side_debugger/debugger.py
+-rw-r--r--   0        0        0      795 2024-04-10 16:49:08.291150 rio_ui-0.5.2/rio/debug/client_side_debugger/deploy_page.py
+-rw-r--r--   0        0        0      782 2024-04-10 16:49:08.291150 rio_ui-0.5.2/rio/debug/client_side_debugger/docs_page.py
+-rw-r--r--   0        0        0    12334 2024-04-10 16:49:08.291150 rio_ui-0.5.2/rio/debug/client_side_debugger/icons_page.py
+-rw-r--r--   0        0        0     2379 2024-04-10 16:49:08.291150 rio_ui-0.5.2/rio/debug/client_side_debugger/project_page.py
+-rw-r--r--   0        0        0     2265 2024-04-08 18:37:44.155783 rio_ui-0.5.2/rio/debug/client_side_debugger/sample_icons_grid.py
+-rw-r--r--   0        0        0    16573 2024-04-10 16:49:08.291150 rio_ui-0.5.2/rio/debug/client_side_debugger/theme_picker_page.py
+-rw-r--r--   0        0        0     1089 2024-04-10 18:34:30.899371 rio_ui-0.5.2/rio/debug/client_side_debugger/tree_page.py
+-rw-r--r--   0        0        0     7224 2024-04-08 18:37:44.155783 rio_ui-0.5.2/rio/debug/monkeypatches.py
+-rw-r--r--   0        0        0        0 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/debug/stress_client/__init__.py
+-rw-r--r--   0        0        0      666 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/debug/stress_client/stress_client.py
+-rw-r--r--   0        0        0      567 2024-04-08 18:37:44.155783 rio_ui-0.5.2/rio/debug/typing_utils.py
+-rw-r--r--   0        0        0    14210 2024-04-08 18:37:44.155783 rio_ui-0.5.2/rio/debug/validator.py
+-rw-r--r--   0        0        0       52 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/docs/__init__.py
+-rw-r--r--   0        0        0     4867 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/docs/custom.py
+-rw-r--r--   0        0        0     1124 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/docs/models.py
+-rw-r--r--   0        0        0    14587 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/docs/parsers.py
+-rw-r--r--   0        0        0      960 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/errors.py
+-rw-r--r--   0        0        0     3173 2024-04-08 18:37:44.155783 rio_ui-0.5.2/rio/event.py
+-rw-r--r--   0        0        0     6732 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/fills.py
+-rw-r--r--   0        0        0   942587 2024-04-10 14:20:32.873198 rio_ui-0.5.2/rio/generated/index.html
+-rw-r--r--   0        0        0      897 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/global_state.py
+-rw-r--r--   0        0        0     9940 2024-04-07 11:32:34.208243 rio_ui-0.5.2/rio/icon_registry.py
+-rw-r--r--   0        0        0     3500 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/inspection.py
+-rw-r--r--   0        0        0     3625 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/maybes.py
+-rw-r--r--   0        0        0     1531 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/patches_for_3rd_party_stuff.py
+-rw-r--r--   0        0        0     7380 2024-04-09 19:38:54.575684 rio_ui-0.5.2/rio/routing.py
+-rw-r--r--   0        0        0      417 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/self_serializing.py
+-rw-r--r--   0        0        0     8463 2024-04-06 18:09:28.111674 rio_ui-0.5.2/rio/serialization.py
+-rw-r--r--   0        0        0    76894 2024-04-08 18:37:44.155783 rio_ui-0.5.2/rio/session.py
+-rw-r--r--   0        0        0     1395 2024-04-06 18:09:28.115007 rio_ui-0.5.2/rio/snippets/README.md
+-rw-r--r--   0        0        0    12292 2024-04-08 13:26:45.976064 rio_ui-0.5.2/rio/snippets/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-06 18:09:28.115007 rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/__init__.py
+-rw-r--r--   0        0        0   157984 2024-04-06 18:09:28.115007 rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/assets/jane-doe.jpg
+-rw-r--r--   0        0        0   181111 2024-04-06 18:09:28.115007 rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/assets/john-doe.jpg
+-rw-r--r--   0        0        0      153 2024-04-06 18:09:28.115007 rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/components/__init__.py
+-rw-r--r--   0        0        0     1062 2024-04-10 16:49:08.291150 rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/components/about_me.py
+-rw-r--r--   0        0        0     1234 2024-04-10 16:49:08.291150 rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/components/contact.py
+-rw-r--r--   0        0        0     3648 2024-04-10 16:49:08.291150 rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/components/history.py
+-rw-r--r--   0        0        0     2042 2024-04-08 18:37:44.155783 rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/components/projects.py
+-rw-r--r--   0        0        0      643 2024-04-10 16:49:08.291150 rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/components/skill_bars.py
+-rw-r--r--   0        0        0       42 2024-04-06 18:09:28.115007 rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/pages/__init__.py
+-rw-r--r--   0        0        0     4373 2024-04-07 11:49:46.858457 rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/pages/biography_page.py
+-rw-r--r--   0        0        0      192 2024-04-06 18:09:28.115007 rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/pages/biography_page_after_tutorial_4.py
+-rw-r--r--   0        0        0     1318 2024-04-09 16:47:56.822558 rio_ui-0.5.2/rio/snippets/snippet-files/other-examples/simple_counter_app.py
+-rw-r--r--   0        0        0      684 2024-04-06 18:08:52.814883 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
+-rw-r--r--   0        0        0      851 2024-04-10 17:01:52.454442 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/__init__.py
+-rw-r--r--   0        0        0      223 2024-04-07 08:57:25.591515 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
+-rw-r--r--   0        0        0     1833 2024-04-08 18:37:44.155783 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
+-rw-r--r--   0        0        0     1196 2024-04-08 18:37:44.155783 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
+-rw-r--r--   0        0        0     3728 2024-04-08 18:37:44.155783 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
+-rw-r--r--   0        0        0      517 2024-04-08 18:37:44.159116 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
+-rw-r--r--   0        0        0     2227 2024-04-07 09:24:53.378316 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
+-rw-r--r--   0        0        0      184 2024-04-07 18:38:03.958535 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
+-rw-r--r--   0        0        0       32 2024-04-06 18:08:52.818216 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
+-rw-r--r--   0        0        0     5823 2024-04-10 17:01:52.457775 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
+-rw-r--r--   0        0        0     3344 2024-04-06 18:08:52.814883 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
+-rw-r--r--   0        0        0        0 2024-04-06 18:09:28.115007 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Empty/README.md
+-rw-r--r--   0        0        0        0 2024-04-07 08:44:19.156096 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Empty/__init__.py
+-rw-r--r--   0        0        0       46 2024-04-06 18:09:28.115007 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Empty/components/__init__.py
+-rw-r--r--   0        0        0      769 2024-04-07 09:08:53.709464 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Empty/components/sample_component.py
+-rw-r--r--   0        0        0       98 2024-04-07 08:04:03.043617 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Empty/meta.json
+-rw-r--r--   0        0        0        0 2024-04-06 18:09:28.115007 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-08 18:37:44.159116 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
+-rw-r--r--   0        0        0     3344 2024-04-06 18:09:28.115007 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
+-rw-r--r--   0        0        0        4 2024-04-10 16:49:08.284483 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 16:49:08.284483 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple CRUD/__init__.py
+-rw-r--r--   0        0        0       68 2024-04-10 16:49:08.284483 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
+-rw-r--r--   0        0        0     4805 2024-04-10 16:49:08.284483 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
+-rw-r--r--   0        0        0     4118 2024-04-10 16:49:08.284483 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
+-rw-r--r--   0        0        0     1685 2024-04-10 16:49:08.284483 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple CRUD/models.py
+-rw-r--r--   0        0        0       32 2024-04-10 16:49:08.284483 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
+-rw-r--r--   0        0        0     6589 2024-04-10 16:49:08.284483 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
+-rw-r--r--   0        0        0     3586 2024-04-10 16:49:08.284483 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
+-rw-r--r--   0        0        0        4 2024-04-06 18:09:28.115007 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple Dashboard/README.md
+-rw-r--r--   0        0        0        0 2024-04-07 08:44:22.292774 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple Dashboard/__init__.py
+-rw-r--r--   0        0        0   139537 2024-04-07 11:11:59.577096 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple Dashboard/assets/smartphones.csv
+-rw-r--r--   0        0        0      210 2024-04-09 20:00:32.337025 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple Dashboard/meta.json
+-rw-r--r--   0        0        0     4112 2024-04-09 20:06:22.094075 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple Dashboard/pages/interactive_plot.py
+-rw-r--r--   0        0        0     3586 2024-04-06 18:09:28.115007 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple Dashboard/thumbnail.svg
+-rw-r--r--   0        0        0      490 2024-04-08 13:25:22.132597 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 13:21:28.592126 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:55:14.311995 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-08 13:26:20.426025 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
+-rw-r--r--   0        0        0       44 2024-04-08 15:32:19.997165 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
+-rw-r--r--   0        0        0     5570 2024-04-10 17:01:52.457775 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0     3344 2024-04-08 13:24:10.679136 rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
+-rw-r--r--   0        0        0     8134 2024-04-08 18:37:44.159116 rio_ui-0.5.2/rio/state_properties.py
+-rw-r--r--   0        0        0     3077 2024-04-06 18:09:28.115007 rio_ui-0.5.2/rio/text_style.py
+-rw-r--r--   0        0        0    19432 2024-04-09 19:38:54.575684 rio_ui-0.5.2/rio/theme.py
+-rw-r--r--   0        0        0     5167 2024-04-06 18:09:28.115007 rio_ui-0.5.2/rio/user_settings_module.py
+-rw-r--r--   0        0        0     3890 2024-04-06 18:09:28.115007 rio_ui-0.5.2/rio/world_units.py
+-rw-r--r--   0        0        0     7599 1970-01-01 00:00:00.000000 rio_ui-0.5.2/PKG-INFO
```

### Comparing `rio_ui-0.5.1/LICENSE.txt` & `rio_ui-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/pyproject.toml` & `rio_ui-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 license = "LGPL-3.0" # TODO
 name = "rio-ui"
-version = "0.5.1"
+version = "0.5.2"
 description = "Build modern Websites and Apps just with Python"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>", "Paul Pinterits"]
 readme = "README.md"
 packages = [{ include = "rio" }]
 include = ["rio/generated/index.html"]
 keywords = [
     "web-development",
@@ -46,15 +46,15 @@
 [tool.poetry.dependencies]
 aiofiles = "^23.2.1"
 cefpython3 = { version = "^66.1", platform = "windows", optional = true }
 fastapi = "^0.109.1"
 fuzzywuzzy = "^0.18.0"
 gitignore-parser = "^0.1.9"
 httpx = "^0.25.1"
-imy = "^0.2.1"
+imy = "^0.2.2"
 introspection = "^1.7.13"
 keyring = "^24.3.0"
 pillow = "^10.2.0"
 platformdirs = { version = "^3.11.0", optional = true }
 pygobject = { version = "^3.44.1", platform = "linux", optional = true }
 pytest = "^7.3.1"
 python = "^3.10"
```

### Comparing `rio_ui-0.5.1/rio/__init__.py` & `rio_ui-0.5.2/rio/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/app.py` & `rio_ui-0.5.2/rio/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
                 align_x=0.5,
                 align_y=0.0,
             )
 
     return DefaultConnectionLostComponent()
 
 
+@final
 class App:
     """
     Contains all the information needed to run a Rio app.
 
     Apps group all the information needed for Rio to run your application, such
     as its name, icon and, and the pages it contains. Apps also expose several
     lifetime events that you can use to perform tasks such as initialization and
```

### Comparing `rio_ui-0.5.1/rio/app_server.py` & `rio_ui-0.5.2/rio/app_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,23 @@
         self,
         app_: app.App,
         debug_mode: bool,
         running_in_window: bool,
         validator_factory: Callable[[rio.Session], debug.Validator] | None,
         internal_on_app_start: Callable[[], None] | None,
     ):
-        super().__init__(lifespan=__class__._lifespan)
+        super().__init__(
+            title=app_.name,
+            # summary=...,
+            # description=...,
+            openapi_url="/openapi.json" if debug_mode else None,
+            docs_url="/docs" if debug_mode else None,
+            redoc_url="/redoc" if debug_mode else None,
+            lifespan=__class__._lifespan,
+        )
 
         self.app = app_
         self.debug_mode = debug_mode
         self.running_in_window = running_in_window
         self.validator_factory = validator_factory
         self.internal_on_app_start = internal_on_app_start
```

### Comparing `rio_ui-0.5.1/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf` & `rio_ui-0.5.2/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf` & `rio_ui-0.5.2/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf` & `rio_ui-0.5.2/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf` & `rio_ui-0.5.2/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/hosted/fonts/Noto Sans/OFL.txt` & `rio_ui-0.5.2/rio/assets/hosted/fonts/Noto Sans/OFL.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto/LICENSE.txt` & `rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf` & `rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf` & `rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf` & `rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf` & `rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt` & `rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf` & `rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf` & `rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf` & `rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf` & `rio_ui-0.5.2/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png` & `rio_ui-0.5.2/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/hosted/rio-logos/rio-logo-square.png` & `rio_ui-0.5.2/rio/assets/hosted/rio-logos/rio-logo-square.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/icon-sets/material.tar.xz` & `rio_ui-0.5.2/rio/assets/icon-sets/material.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/icon-sets/rio.tar.xz` & `rio_ui-0.5.2/rio/assets/icon-sets/rio.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets/icon-sets/styling.tar.xz` & `rio_ui-0.5.2/rio/assets/icon-sets/styling.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/assets.py` & `rio_ui-0.5.2/rio/assets.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/byte_serving.py` & `rio_ui-0.5.2/rio/byte_serving.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/cli/__init__.py` & `rio_ui-0.5.2/rio/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/cli/cli_instance.py` & `rio_ui-0.5.2/rio/cli/cli_instance.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/cli/nice_traceback.py` & `rio_ui-0.5.2/rio/cli/nice_traceback.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/cli/project.py` & `rio_ui-0.5.2/rio/cli/project.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/cli/project_setup.py` & `rio_ui-0.5.2/rio/cli/project_setup.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/cli/rio_api.py` & `rio_ui-0.5.2/rio/cli/rio_api.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/cli/rioignore.py` & `rio_ui-0.5.2/rio/cli/rioignore.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/cli/run_project/app_loading.py` & `rio_ui-0.5.2/rio/cli/run_project/app_loading.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/cli/run_project/arbiter.py` & `rio_ui-0.5.2/rio/cli/run_project/arbiter.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/cli/run_project/file_watcher_worker.py` & `rio_ui-0.5.2/rio/cli/run_project/file_watcher_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/cli/run_project/uvicorn_worker.py` & `rio_ui-0.5.2/rio/cli/run_project/uvicorn_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/cli/run_project/webview_worker.py` & `rio_ui-0.5.2/rio/cli/run_project/webview_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/cli/tomlconfig.py` & `rio_ui-0.5.2/rio/cli/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/color.py` & `rio_ui-0.5.2/rio/color.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 __all__ = [
     "Color",
     "ColorSet",
 ]
 
 
+@final
 class Color(SelfSerializing):
     """
     A color, optionally with an opacity.
 
     The `Color` class does exactly what it says on the tin: It represents a
     single color. They're used throughout Rio to specify the color of text,
     fills, and more.
```

### Comparing `rio_ui-0.5.1/rio/common.py` & `rio_ui-0.5.2/rio/common.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/components/__init__.py` & `rio_ui-0.5.2/rio/components/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-import typing
-
-from . import component_tree, debugger_connector
-from .app_root import *
 from .auto_form import *
 from .banner import *
 from .button import *
 from .card import *
 from .code_explorer import *
 from .color_picker import *
 from .component import *
@@ -53,9 +49,9 @@
 from .text import *
 from .text_input import *
 from .theme_context_switcher import *
 from .tooltip import *
 from .website import *
 
 assert (
-    Container is not typing.Container
+    Container.__module__ != "typing"
 ), "Looks like somebody imported `typing.Container`, thus accidentally overwriting `rio.Container`. Are you missing an `__all__` in some component?"
```

### Comparing `rio_ui-0.5.1/rio/components/app_root.py` & `rio_ui-0.5.2/rio/components/app_root.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,20 +66,20 @@
                     size=3,
                     on_press=self.on_press_close,
                 ),
                 rio.Column(
                     rio.Text(
                         self.session.app.name,
                         style="heading2",
-                        align_x=0,
+                        justify='left',
                     ),
                     rio.Text(
                         "TODO: Subtext",
                         style="dim",
-                        align_x=0,
+                        justify='left',
                     ),
                     align_y=0,
                 ),
                 spacing=1,
                 margin_x=1,
                 margin_y=1,
                 align_x=0,
```

### Comparing `rio_ui-0.5.1/rio/components/auto_form.py` & `rio_ui-0.5.2/rio/components/auto_form.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/components/banner.py` & `rio_ui-0.5.2/rio/components/banner.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from . import component
 
 __all__ = [
     "Banner",
 ]
 
 
+@final
 class Banner(component.Component):
     r"""
     # Banner
 
     Displays a short message to the user.
 
     Banners can either show a short text message to the users, or disappear
```

### Comparing `rio_ui-0.5.1/rio/components/build_failed.py` & `rio_ui-0.5.2/rio/components/build_failed.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/components/button.py` & `rio_ui-0.5.2/rio/components/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 
 CHILD_MARGIN_X = 1.0
 CHILD_MARGIN_Y = 0.3
 INITIALLY_DISABLED_FOR = 0.25
 
 
+@final
 class Button(Component):
     """
     # Button
 
     A clickable button.
 
     The `Button` component allows the user to trigger an action by clicking on
@@ -218,14 +219,15 @@
             content = f"text:{self.content!r}"
         else:
             content = f"content:{self.content._id}"
 
         return f"<Button id:{self._id} {content}>"
 
 
+@final
 class IconButton(Component):
     """
     # IconButton
 
     A round, clickable button with an icon.
 
     The `IconButton` component allows the user to trigger an action by clicking
```

### Comparing `rio_ui-0.5.1/rio/components/card.py` & `rio_ui-0.5.2/rio/components/card.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "Card",
 ]
 
 
+@final
 class Card(FundamentalComponent):
     """
     # Card
 
     A container that visually encompasses its child components.
 
     Cards are used to group related components together, and to visually
```

### Comparing `rio_ui-0.5.1/rio/components/class_container.py` & `rio_ui-0.5.2/rio/components/class_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/components/color_picker.py` & `rio_ui-0.5.2/rio/components/color_picker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY, dataclass
-from typing import Any
+from typing import Any, final
 
 from uniserde import JsonDoc
 
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "ColorPicker",
     "ColorChangeEvent",
 ]
 
 
+@final
 @dataclass
 class ColorChangeEvent:
     color: rio.Color
 
 
+@final
 class ColorPicker(FundamentalComponent):
     """
     # ColorPicker
 
     Allows the user to pick an RGB(A) color.
 
     `ColorPicker` is a component that allows the user to pick a color. It
```

### Comparing `rio_ui-0.5.1/rio/components/component.py` & `rio_ui-0.5.2/rio/components/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from uniserde import Jsonable, JsonDoc
 
 import rio
 
 from .. import event, global_state, inspection
 from ..dataclass import RioDataclassMeta, class_local_fields, internal_field
 from ..state_properties import StateBindingMaker, StateProperty
-from . import fundamental_component
 
 __all__ = ["Component"]
 
 
 T = TypeVar("T")
 
 
@@ -510,14 +509,16 @@
 
     def _iter_direct_and_indirect_child_containing_attributes(
         self,
         *,
         include_self: bool,
         recurse_into_high_level_components: bool,
     ) -> Iterable[Component]:
+        from . import fundamental_component  # Avoid circular import problem
+
         # Special case the component itself to handle `include_self`
         if include_self:
             yield self
 
         if not recurse_into_high_level_components and not isinstance(
             self, fundamental_component.FundamentalComponent
         ):
@@ -534,14 +535,16 @@
             ):
                 to_do.extend(cur._iter_direct_children())
 
     def _iter_component_tree(self) -> Iterable[Component]:
         """
         Iterate over all components in the component tree, with this component as the root.
         """
+        from . import fundamental_component  # Avoid circular import problem
+
         yield self
 
         if isinstance(self, fundamental_component.FundamentalComponent):
             for child in self._iter_direct_children():
                 yield from child._iter_component_tree()
         else:
             build_result = self.session._weak_component_data_by_component[
```

### Comparing `rio_ui-0.5.1/rio/components/component_tree.py` & `rio_ui-0.5.2/rio/components/component_tree.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/components/container.py` & `rio_ui-0.5.2/rio/components/container.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .component import Component
 
 __all__ = [
     "Container",
 ]
 
 
+@final
 class Container(Component):
     """
     # Container
 
     A component holding a single child.
 
     `Container` is a simple container which holds a single child component. It
```

### Comparing `rio_ui-0.5.1/rio/components/devel_component.py` & `rio_ui-0.5.2/rio/components/devel_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/components/drawer.py` & `rio_ui-0.5.2/rio/components/drawer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY, dataclass
-from typing import Literal
+from typing import Literal, final
 
 from uniserde import JsonDoc
 
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "Drawer",
     "DrawerOpenOrCloseEvent",
 ]
 
 
+@final
 @dataclass
 class DrawerOpenOrCloseEvent:
     is_open: bool
 
 
+@final
 class Drawer(FundamentalComponent):
     """
     # Drawer
 
     A container which slides in from the edge of the screen.
 
     Drawers are containers which can either be completely hidden from view, or
```

### Comparing `rio_ui-0.5.1/rio/components/dropdown.py` & `rio_ui-0.5.2/rio/components/dropdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from collections.abc import Mapping, Sequence
 from dataclasses import KW_ONLY, dataclass
-from typing import Any, Generic, Literal, TypeVar
+from typing import Any, Generic, Literal, TypeVar, final
 
 from uniserde import JsonDoc
 
 import rio
 
 from .fundamental_component import FundamentalComponent
 
@@ -14,19 +14,21 @@
     "Dropdown",
     "DropdownChangeEvent",
 ]
 
 T = TypeVar("T")
 
 
+@final
 @dataclass
 class DropdownChangeEvent(Generic[T]):
     value: T
 
 
+@final
 class Dropdown(FundamentalComponent, Generic[T]):
     """
     # Dropdown
 
     A dropdown menu allowing the user to select one of several options.
 
     Dropdowns present the user with a list of options, allowing them to select
```

### Comparing `rio_ui-0.5.1/rio/components/flow_container.py` & `rio_ui-0.5.2/rio/components/flow_container.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY
-from typing import Literal
+from typing import Literal, final
+
+from typing_extensions import Self
 
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = ["FlowContainer"]
 
 
+@final
 class FlowContainer(FundamentalComponent):
     """
     # FlowContainer
 
     A container that lays out its children in a horizontal or vertical flow.
 
     `FlowContainer` is a container that lays out its children in a horizontal or
@@ -89,9 +92,16 @@
         )
 
         self.children = list(children)
         self.column_spacing = column_spacing
         self.row_spacing = row_spacing
         self.justify = justify
 
+    def add(self, child: rio.Component) -> Self:
+        """
+        Appends a child component.
+        """
+        self.children.append(child)
+        return self
+
 
 FlowContainer._unique_id = "FlowContainer-builtin"
```

### Comparing `rio_ui-0.5.1/rio/components/fundamental_component.py` & `rio_ui-0.5.2/rio/components/fundamental_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 from uniserde import Jsonable, JsonDoc
 
 import rio
 
 from .. import common, inspection
 from .component import Component
 
-__all__ = ["FundamentalComponent", "KeyboardFocusableFundamentalComponent"]
+__all__ = [
+    "FundamentalComponent",
+    "KeyboardFocusableFundamentalComponent",
+]
 
 
 JAVASCRIPT_SOURCE_TEMPLATE = """
 // Run the code in a function to avoid name clashes with globals
 (function () {
 
     %(js_source)s
```

### Comparing `rio_ui-0.5.1/rio/components/grid.py` & `rio_ui-0.5.2/rio/components/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from __future__ import annotations
 
 import math
 from collections.abc import Iterable
 from dataclasses import KW_ONLY, dataclass
-from typing import Literal
+from typing import Literal, final
 
+from typing_extensions import Self
 from uniserde import JsonDoc
 
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = ["Grid"]
 
 
+@final
 @dataclass
 class GridChildPosition:
     row: int
     column: int
     width: int = 1
     height: int = 1
 
 
+@final
 class Grid(FundamentalComponent):
     """
     # Grid
 
     A container which arranges its children in a table-like grid.
 
     Grids arrange their children in a table-like grid. Each child is placed in
@@ -127,17 +130,14 @@
 
         # JS can only work with lists of Components, so we'll store the
         # components and their positions separately
         self._children, self._child_positions = self._add_initial_children(rows)
 
         self._properties_set_by_creator_.update(["_children", "_child_positions"])
 
-    def __repr__(self) -> str:
-        return "foo"
-
     def _add_initial_children(
         self,
         children: Iterable[rio.Component | Iterable[rio.Component]],
     ) -> tuple[list[rio.Component], list[GridChildPosition]]:
         """
         Adds the children added in the constructor to the component. This is
         fairly complex and thus has its own function so not to pollute the
@@ -185,27 +185,27 @@
         self,
         child: rio.Component,
         row: int,
         column: int,
         *,
         width: int = 1,
         height: int = 1,
-    ) -> Grid:
+    ) -> Self:
         assert isinstance(child, rio.Component), child
         """
         Add a child to the grid at a specified position.
 
         Args:
             child: The child component to add to the grid.
 
             row: The row in which to place the child.
 
             column: The column in which to place the child.
 
-            width The number of columns the child should take up.
+            width: The number of columns the child should take up.
 
             height: The number of rows the child should take up.
 
 
         Example:
             ```python
             grid = rio.Grid(row_spacing=1, column_spacing=1)
```

### Comparing `rio_ui-0.5.1/rio/components/icon.py` & `rio_ui-0.5.2/rio/components/icon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY
 from pathlib import Path
-from typing import Literal
+from typing import Literal, final
 
 from uniserde import JsonDoc
 
 import rio
 
 from .. import color, fills, icon_registry
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "Icon",
 ]
 
 
+@final
 class Icon(FundamentalComponent):
     """
     # Icon
 
     Displays one of many pre-bundled icons.
 
     Icons are a great way to add polish to your app. A good icon can help your
```

### Comparing `rio_ui-0.5.1/rio/components/image.py` & `rio_ui-0.5.2/rio/components/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY
-from typing import Literal
+from typing import Literal, final
 
 from uniserde import JsonDoc
 
 from .. import assets
 from ..common import EventHandler, ImageLike
 from .fundamental_component import FundamentalComponent
 
 __all__ = ["Image"]
 
 
+@final
 class Image(FundamentalComponent):
     """
     # Image
 
     Displays an image file.
 
     `Image` does just what you'd expect: it displays a single image. The image
```

### Comparing `rio_ui-0.5.1/rio/components/key_event_listener.py` & `rio_ui-0.5.2/rio/components/key_event_listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY, dataclass
-from typing import Any, Literal
+from typing import Any, Literal, final
 
 from uniserde import Jsonable
 
 import rio
 
 from .fundamental_component import KeyboardFocusableFundamentalComponent
 
@@ -586,26 +586,30 @@
     def __str__(self) -> str:
         keys = [key for key in _MODIFIERS if key in self.modifiers]
         keys.append(self.software_key)
 
         return " + ".join(keys)
 
 
+@final
 class KeyDownEvent(_KeyUpDownEvent):
     pass
 
 
+@final
 class KeyUpEvent(_KeyUpDownEvent):
     pass
 
 
+@final
 class KeyPressEvent(_KeyUpDownEvent):
     pass
 
 
+@final
 class KeyEventListener(KeyboardFocusableFundamentalComponent):
     """
     Calls an event handler when a key is pressed or released.
 
     `KeyEventListener` is a container for a single child component. It listens
     for keyboard events and calls corresponding event handlers when they occur.
```

### Comparing `rio_ui-0.5.1/rio/components/labeled_column.py` & `rio_ui-0.5.2/rio/components/labeled_column.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
 from collections.abc import Mapping
 from dataclasses import field
-from typing import Literal
+from typing import Literal, final
+
+from typing_extensions import Self
 
 import rio
 
 from .component import Component
 
 __all__ = ["LabeledColumn"]
 
 
+@final
 class LabeledColumn(Component):
     """
     # LabeledColumn
 
     A container that lays out its children in a column, with labels for each child.
 
     `LabeledColumn` is a container that lays out its children in a column, with
@@ -80,22 +83,29 @@
 
     @property
     def content(self) -> Mapping[str, Component]:
         return self._content
 
     @content.setter
     def content(self, children: Mapping[str, Component]) -> None:
-        self._content = children
+        self._content = dict(children)
         self._child_list = list(children.values())
 
-    def build(self) -> Component:
-        rows = []
+    def add(self, label: str, child: rio.Component) -> Self:
+        """
+        Appends a child component.
+        """
+        self._content[label] = child
+        self._child_list.append(child)
 
-        for label, child in self.content.items():
-            rows.append(
-                [
-                    rio.Text(label, align_x=1),
-                    child,
-                ]
-            )
+        return self
+
+    def build(self) -> Component:
+        rows = [
+            [
+                rio.Text(label, justify='right'),
+                child,
+            ]
+            for label, child in self.content.items()
+        ]
 
         return rio.Grid(*rows, row_spacing=0.1, column_spacing=0.2)
```

### Comparing `rio_ui-0.5.1/rio/components/linear_containers.py` & `rio_ui-0.5.2/rio/components/linear_containers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from collections.abc import Sequence
-from typing import Literal
+from typing import Literal, final
 
+from typing_extensions import Self
 from uniserde import JsonDoc
 
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
@@ -20,33 +21,40 @@
     spacing: float = 0.0
     proportions: Literal["homogeneous"] | Sequence[float] | None = None
 
     # Don't let @dataclass generate a constructor
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
+    def add(self, child: rio.Component) -> Self:
+        """
+        Appends a child component.
+        """
+        self.children.append(child)
+        return self
+
     def _custom_serialize(self) -> JsonDoc:
         return {"proportions": self.proportions}  # type: ignore[variance]
 
 
+@final
 class Row(_LinearContainer):
     """
     # Row
 
     A container that lays out its children horizontally.
 
     `Row`s are one of the most common components in Rio. They take any number of
     children and lay them out horizontally, with the first one on the left, the
     second one to its right, and so on. All components in `Row`s occupy the full
     height of their parent.
 
     The `Row`'s horizontal counterpart is the `Column`. A similar component, but
     stacking its children in the Z direction, is the `Stack`.
 
-
     ## Undefined Space
 
     Like most containers in `rio`, `Row`s always attempt to allocate all
     available space to their children. In the context of a `Row` though, this
     could easily lead to unexpected results. If more space is available than
     needed, should all children grow? Only the first? Should they grow by equal
     amounts, or proportionally?
@@ -57,28 +65,26 @@
     unmistakable animated sprites.
 
     Getting rid of undefined space is easy: Depending on what look you're going
     for, either add a `Spacer` somewhere into your `Row`, assign one of the
     components a `"grow"` value as its height, or set the `Row`'s vertical
     alignment.
 
-
     ## Attributes:
 
     `children`: The components to place in this `Row`.
 
     `spacing`: How much empty space to leave between two adjacent children. No
             spacing is added before the first child or after the last child.
 
     `proportions`: If set, the children will grow according to these proportions.
         - `homogeneous`: All children will grow equally.
         - A list of floats: Each child will grow according to its proportion.
         - `None`: Allows all child components to expand as much as they need.
 
-
     ## Example:
 
     This minimal example will display a `Row` with two text components:
 
     ```python
     rio.Row(rio.Text("Hello"), rio.Text("World!"))
     ```
@@ -140,14 +146,15 @@
         self.spacing = spacing
         self.proportions = proportions
 
 
 Row._unique_id = "Row-builtin"
 
 
+@final
 class Column(_LinearContainer):
     """
     # Column
 
     A container that lays out its children vertically.
 
     `Column`s are one of the most common components in Rio. They take any number
```

### Comparing `rio_ui-0.5.1/rio/components/link.py` & `rio_ui-0.5.2/rio/components/link.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
 import webbrowser
-from typing import Any, Literal
+from typing import Any, Literal, final
 
 from uniserde import JsonDoc
 
 import rio
 
 from .. import common
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "Link",
 ]
 
 
+@final
 class Link(FundamentalComponent):
     """
     # Link
 
     Navigates to a page or URL when clicked.
 
     `Link`s display a short text, or arbitrary component, and navigate to a page
```

### Comparing `rio_ui-0.5.1/rio/components/list_items.py` & `rio_ui-0.5.2/rio/components/list_items.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "HeadingListItem",
     "SeparatorListItem",
     "SimpleListItem",
     "CustomListItem",
 ]
 
 
+@final
 class HeadingListItem(FundamentalComponent):
     """
     # HeadingListItem
 
     A simple list item with only a header.
 
     `HeadingListItem`s are the easiest way to create list items, which can take
@@ -69,21 +70,23 @@
 
     text: str
 
 
 HeadingListItem._unique_id = "HeadingListItem-builtin"
 
 
+@final
 class SeparatorListItem(FundamentalComponent):
     pass
 
 
 SeparatorListItem._unique_id = "SeparatorListItem-builtin"
 
 
+@final
 class SimpleListItem(Component):
     """
     # SimpleListItem
 
     A simple list item with a header and optional secondary text and children.
 
     `SimpleListItem`s are a convenient way to create list items, which can
@@ -188,25 +191,25 @@
         if self.left_child is not None:
             children.append(self.left_child)
 
         # Main content (text)
         text_children = [
             rio.Text(
                 self.text,
-                align_x=0,
+                        justify='left',
             )
         ]
 
         if self.secondary_text:
             text_children.append(
                 rio.Text(
                     self.secondary_text,
                     wrap=True,
                     style="dim",
-                    align_x=0,
+                        justify='left',
                 )
             )
 
         children.append(
             rio.Column(
                 *text_children,
                 spacing=0.5,
@@ -227,14 +230,15 @@
                 width="grow",
             ),
             on_press=self.on_press,
             key="",
         )
 
 
+@final
 class CustomListItem(FundamentalComponent):
     """
     # CustomListItem
 
     A list item with custom content.
 
     Most of the time the `SimpleListItem` will do the job. With
```

### Comparing `rio_ui-0.5.1/rio/components/list_view.py` & `rio_ui-0.5.2/rio/components/list_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
-from typing import Literal
+from typing import Literal, final
+
+from typing_extensions import Self
 
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = ["ListView"]
 
 
+@final
 class ListView(FundamentalComponent):
     """
     # ListView
 
     Vertically arranges and styles its children.
 
     A container which arranges its children in a vertical list. It is similar to `Column`,
@@ -104,9 +107,16 @@
             height=height,
             align_x=align_x,
             align_y=align_y,
         )
 
         self.children = list(children)
 
+    def add(self, child: rio.Component) -> Self:
+        """
+        Appends a child component.
+        """
+        self.children.append(child)
+        return self
+
 
 ListView._unique_id = "ListView-builtin"
```

### Comparing `rio_ui-0.5.1/rio/components/markdown.py` & `rio_ui-0.5.2/rio/components/markdown.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from dataclasses import KW_ONLY
+from typing import final
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "Markdown",
 ]
 
 
+@final
 class Markdown(FundamentalComponent):
     """
     # Markdown
 
     Displays Markdown-formatted text.
 
     `Markdown` displays text formatted using markdown. Markdown is a
```

### Comparing `rio_ui-0.5.1/rio/components/media_player.py` & `rio_ui-0.5.2/rio/components/media_player.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
 import pathlib
-from typing import Literal
+from typing import Literal, final
 
 from uniserde import JsonDoc
 
 import rio
 
 from .. import assets, color
 from ..common import EventHandler
 from .fundamental_component import KeyboardFocusableFundamentalComponent
 
 __all__ = ["MediaPlayer"]
 
 
+@final
 class MediaPlayer(KeyboardFocusableFundamentalComponent):
     """
     # MediaPlayer
 
     Plays audio and video.
 
     `MediaPlayer` plays back audio and video files. It can play local files and
```

### Comparing `rio_ui-0.5.1/rio/components/mouse_event_listener.py` & `rio_ui-0.5.2/rio/components/mouse_event_listener.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,77 +21,88 @@
     "MouseLeaveEvent",
     "DragStartEvent",
     "DragMoveEvent",
     "DragEndEvent",
 ]
 
 
+@final
 class MouseButton(enum.Enum):
     LEFT = "left"
     MIDDLE = "middle"
     RIGHT = "right"
 
 
 @dataclass
 class _MouseUpDownEvent:
     button: MouseButton
     x: float
     y: float
 
 
+@final
 class PressEvent(_MouseUpDownEvent):
     pass
 
 
+@final
 class MouseDownEvent(_MouseUpDownEvent):
     pass
 
 
+@final
 class MouseUpEvent(_MouseUpDownEvent):
     pass
 
 
 @dataclass
 class _MousePositionedEvent:
     x: float
     y: float
 
 
+@final
 class MouseMoveEvent(_MousePositionedEvent):
     pass
 
 
+@final
 class MouseEnterEvent(_MousePositionedEvent):
     pass
 
 
+@final
 class MouseLeaveEvent(_MousePositionedEvent):
     pass
 
 
 @dataclass
 class _DragEvent:
     button: MouseButton
     x: float
     y: float
     component: rio.Component
 
 
+@final
 class DragStartEvent(_DragEvent):
     pass
 
 
+@final
 class DragMoveEvent(_DragEvent):
     pass
 
 
+@final
 class DragEndEvent(_DragEvent):
     pass
 
 
+@final
 class MouseEventListener(FundamentalComponent):
     """
     Allows you to listen for mouse events on a component.
 
     `MouseEventListeners` take a single child component and display it. They
     then listen for any mouse activity on the child component and report it
     through their event handlers.
```

### Comparing `rio_ui-0.5.1/rio/components/multi_line_text_input.py` & `rio_ui-0.5.2/rio/components/multi_line_text_input.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY, dataclass
-from typing import Any
+from typing import Any, final
 
 from uniserde import JsonDoc
 
 import rio
 
 from .fundamental_component import KeyboardFocusableFundamentalComponent
 
 __all__ = [
     "MultiLineTextInput",
     "MultiLineTextInputChangeEvent",
     "MultiLineTextInputConfirmEvent",
 ]
 
 
+@final
 @dataclass
 class MultiLineTextInputChangeEvent:
     text: str
 
 
+@final
 @dataclass
 class MultiLineTextInputConfirmEvent:
     text: str
 
 
+@final
 class MultiLineTextInput(KeyboardFocusableFundamentalComponent):
     """
     # MultiLineTextInput
 
     A user-editable text field.
 
     It's similar to `TextInput`, but it allows the user to enter multiple lines of text.
```

### Comparing `rio_ui-0.5.1/rio/components/node_input.py` & `rio_ui-0.5.2/rio/components/node_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "NodeInput",
 ]
 
 
+@final
 class NodeInput(FundamentalComponent):
     name: str
     color: rio.Color
 
     def __init__(
         self,
         name: str,
```

### Comparing `rio_ui-0.5.1/rio/components/node_output.py` & `rio_ui-0.5.2/rio/components/node_output.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "NodeOutput",
 ]
 
 
+@final
 class NodeOutput(FundamentalComponent):
     name: str
     color: rio.Color
 
     def __init__(
         self,
         name: str,
```

### Comparing `rio_ui-0.5.1/rio/components/number_input.py` & `rio_ui-0.5.2/rio/components/number_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,24 +19,27 @@
 # float
 _multiplier_suffixes: Mapping[str, int] = {
     "k": 1_000,
     "m": 1_000_000,
 }
 
 
+@final
 @dataclass
 class NumberInputChangeEvent:
     value: float
 
 
+@final
 @dataclass
 class NumberInputConfirmEvent:
     value: float
 
 
+@final
 class NumberInput(Component):
     """
     # NumberInput
 
     Like `TextInput`, but specifically for inputting numbers.
 
     `NumberInput` allows the user to enter a number. This is similar to the
```

### Comparing `rio_ui-0.5.1/rio/components/overlay.py` & `rio_ui-0.5.2/rio/components/overlay.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "Overlay",
 ]
 
 
+@final
 class Overlay(FundamentalComponent):
     """
     # Overlay
 
     Displays its child above all other components.
 
     The overlay component takes a single child component, and displays it above
```

### Comparing `rio_ui-0.5.1/rio/components/page_view.py` & `rio_ui-0.5.2/rio/components/page_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         spacing=3,
         width=20,
         align_x=0.5,
         align_y=0.35,
     )
 
 
+@final
 class PageView(Component):
     """
     # PageView
 
     Placeholders for pages.
 
     Rio apps can consist of many pages. You might have a welcome page, a
```

### Comparing `rio_ui-0.5.1/rio/components/plot.py` & `rio_ui-0.5.2/rio/components/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import copy
 import io
-from typing import TYPE_CHECKING, Literal, cast
+from typing import TYPE_CHECKING, Literal, cast, final
 
 from uniserde import JsonDoc
 
 import rio
 
 from .. import maybes
 from .fundamental_component import FundamentalComponent
@@ -16,14 +16,15 @@
     import matplotlib.figure  # type: ignore
     import plotly.graph_objects  # type: ignore
 
 
 __all__ = ["Plot"]
 
 
+@final
 class Plot(FundamentalComponent):
     """
     # Plot
 
     Displays a matplotlib, seaborn or plotly plot.
```

### Comparing `rio_ui-0.5.1/rio/components/popup.py` & `rio_ui-0.5.2/rio/components/popup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY, dataclass
-from typing import Literal
+from typing import Literal, final
 
 from uniserde import JsonDoc
 
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "Popup",
     "PopupOpenOrCloseEvent",
 ]
 
 
+@final
 @dataclass
 class PopupOpenOrCloseEvent:
     is_open: bool
 
 
+@final
 class Popup(FundamentalComponent):
     """
     # Popup
 
     A container which floats above other components.
 
     Popups are containers which float above the page when open. This allows you
```

### Comparing `rio_ui-0.5.1/rio/components/progress_bar.py` & `rio_ui-0.5.2/rio/components/progress_bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from typing import final
+
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "ProgressBar",
 ]
 
 
+@final
 class ProgressBar(FundamentalComponent):
     """
     # ProgressBar
 
     A progress indicator in the shape of a horizontal bar.
 
     `ProgressBar` conveys to the user that activity is ongoing. It can either
```

### Comparing `rio_ui-0.5.1/rio/components/progress_circle.py` & `rio_ui-0.5.2/rio/components/progress_circle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
-from typing import Literal
+from typing import Literal, final
 
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "ProgressCircle",
 ]
 
 
+@final
 class ProgressCircle(FundamentalComponent):
     """
     # ProgressCircle
 
     A progress indicator in the shape of a circle.
 
     `ProgressCircle` conveys to the user that activity is ongoing. It can either
```

### Comparing `rio_ui-0.5.1/rio/components/rectangle.py` & `rio_ui-0.5.2/rio/components/rectangle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY
+from typing import final
 
 from uniserde import JsonDoc
 
 import rio
 
 from .. import cursor_style
 from ..color import Color
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "Rectangle",
 ]
 
 
+@final
 class Rectangle(FundamentalComponent):
     """
     # Rectangle
 
     A customizable rectangle shape.
 
     Rectangles are versatile components that can be used to build up more
```

### Comparing `rio_ui-0.5.1/rio/components/revealer.py` & `rio_ui-0.5.2/rio/components/revealer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY, dataclass
-from typing import Literal, TypeVar
+from typing import Literal, TypeVar, final
 
 from uniserde import JsonDoc
 
 import rio
 
 from .fundamental_component import FundamentalComponent
 
@@ -13,19 +13,21 @@
     "Revealer",
     "RevealerChangeEvent",
 ]
 
 T = TypeVar("T")
 
 
+@final
 @dataclass
 class RevealerChangeEvent:
     is_open: bool
 
 
+@final
 class Revealer(FundamentalComponent):
     """
     # Revealer
 
     A component that can be used to hide and reveal content.
 
     `Revealer` is a versatile component that can be used to hide and reveal
```

### Comparing `rio_ui-0.5.1/rio/components/root_components.py` & `rio_ui-0.5.2/rio/components/root_components.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/components/scroll_container.py` & `rio_ui-0.5.2/rio/components/scroll_container.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY
-from typing import Literal
+from typing import Literal, final
 
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = ["ScrollContainer"]
 
 
+@final
 class ScrollContainer(FundamentalComponent):
     """
     # ScrollContainer
 
     Displays a scroll bar if its child grows too large.
 
     `ScrollContainer` is a container which displays a scroll bar if its child
```

### Comparing `rio_ui-0.5.1/rio/components/scroll_target.py` & `rio_ui-0.5.2/rio/components/scroll_target.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
+from typing import final
+
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = ["ScrollTarget"]
 
 
+@final
 class ScrollTarget(FundamentalComponent):
     """
     # ScrollTarget
 
     Allows browsers to scroll to a specific component via URL fragment.
 
     `ScrollTarget` is a container which can be referenced by a URL fragment,
```

### Comparing `rio_ui-0.5.1/rio/components/separator.py` & `rio_ui-0.5.2/rio/components/separator.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "Separator",
 ]
 
 
+@final
 class Separator(FundamentalComponent):
     """
     # Separator
 
     A line to separate content.
 
     `Separator` is a horizontal or vertical line that can be used to separate content. It
```

### Comparing `rio_ui-0.5.1/rio/components/slider.py` & `rio_ui-0.5.2/rio/components/slider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Literal
+from typing import Literal, final
 
 from uniserde import JsonDoc
 
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "Slider",
     "SliderChangeEvent",
 ]
 
 
+@final
 @dataclass
 class SliderChangeEvent:
     value: float
 
 
+@final
 class Slider(FundamentalComponent):
     """
     # Slider
 
     A component for selecting a single value from a range.
 
     The `Slider` components allows the user to select a single real number value
```

### Comparing `rio_ui-0.5.1/rio/components/slideshow.py` & `rio_ui-0.5.2/rio/components/slideshow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY
 from datetime import timedelta
-from typing import Literal
+from typing import Literal, final
 
 from uniserde import JsonDoc
 
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "Slideshow",
 ]
 
 
+@final
 class Slideshow(FundamentalComponent):
     """
     # Slideshow
 
     Prominently switch between multiple components based on a timer.
 
     The `Slideshow` component is a container that can hold multiple components,
```

### Comparing `rio_ui-0.5.1/rio/components/spacer.py` & `rio_ui-0.5.2/rio/components/spacer.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from . import class_container
 
 __all__ = [
     "Spacer",
 ]
 
 
+@final
 class Spacer(class_container.ClassContainer):
     """
     # Spacer
 
     Adds empty space.
 
     Spacers are invisible components which add empty space between other
```

### Comparing `rio_ui-0.5.1/rio/components/stack.py` & `rio_ui-0.5.2/rio/components/stack.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
-from typing import Literal
+from typing import Literal, final
+
+from typing_extensions import Self
 
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = ["Stack"]
 
 
+@final
 class Stack(FundamentalComponent):
     """
     # Stack
 
     A container that stacks its children in the Z direction.
 
     `Stacks` are similar to rows and columns, but they stack their children in
@@ -89,9 +92,16 @@
             height=height,
             align_x=align_x,
             align_y=align_y,
         )
 
         self.children = list(children)
 
+    def add(self, child: rio.Component) -> Self:
+        """
+        Appends a child component.
+        """
+        self.children.append(child)
+        return self
+
 
 Stack._unique_id = "Stack-builtin"
```

### Comparing `rio_ui-0.5.1/rio/components/switch.py` & `rio_ui-0.5.2/rio/components/switch.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 
 __all__ = [
     "Switch",
     "SwitchChangeEvent",
 ]
 
 
+@final
 @dataclass
 class SwitchChangeEvent:
     is_on: bool
 
 
+@final
 class Switch(FundamentalComponent):
     """
     # Switch
 
     An input for `True` / `False` values.
 
     Switches allow the user to toggle between an "on" and an "off" state. They
```

### Comparing `rio_ui-0.5.1/rio/components/switcher.py` & `rio_ui-0.5.2/rio/components/switcher.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
+from typing import final
+
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "Switcher",
 ]
 
 
+@final
 class Switcher(FundamentalComponent):
     """
     # Switcher
 
     A container which can switch between different components.
 
     A `Switcher` is a container which can switch between different components.
```

### Comparing `rio_ui-0.5.1/rio/components/switcher_bar.py` & `rio_ui-0.5.2/rio/components/switcher_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from collections.abc import Sequence
 from dataclasses import dataclass
-from typing import Any, Generic, Literal, TypeVar
+from typing import Any, Generic, Literal, TypeVar, final
 
 from uniserde import JsonDoc
 
 import rio
 
 from .. import icon_registry
 from .fundamental_component import FundamentalComponent
@@ -15,19 +15,21 @@
     "SwitcherBarChangeEvent",
     "SwitcherBar",
 ]
 
 T = TypeVar("T")
 
 
+@final
 @dataclass
 class SwitcherBarChangeEvent(Generic[T]):
     value: T | None
 
 
+@final
 class SwitcherBar(FundamentalComponent, Generic[T]):
     """
     # SwitcherBar
 
     A bar of options which can be switched between.
 
     A `SwitcherBar` is a bar of options which can be switched between. It is
```

### Comparing `rio_ui-0.5.1/rio/components/table.py` & `rio_ui-0.5.2/rio/components/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 __all__ = ["Table"]
 
 
 TableValue = int | float | str
 
 
+@final
 class Table(FundamentalComponent):
     """
     # Table
 
     A table of data.
 
     Tables are a way to display data in a grid, with rows and columns. They are
```

### Comparing `rio_ui-0.5.1/rio/components/text.py` & `rio_ui-0.5.2/rio/components/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "Text",
 ]
 
 
+@final
 class Text(FundamentalComponent):
     """
     # Text
 
     Displays unformatted text.
 
     `Text` displays text without any formatting, making it one of the most
```

### Comparing `rio_ui-0.5.1/rio/components/text_input.py` & `rio_ui-0.5.2/rio/components/text_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY, dataclass
-from typing import Any
+from typing import Any, final
 
 from uniserde import JsonDoc
 
 import rio
 
 from .fundamental_component import KeyboardFocusableFundamentalComponent
 
 __all__ = [
     "TextInput",
     "TextInputChangeEvent",
     "TextInputConfirmEvent",
 ]
 
 
+@final
 @dataclass
 class TextInputChangeEvent:
     text: str
 
 
+@final
 @dataclass
 class TextInputConfirmEvent:
     text: str
 
 
+@final
 class TextInput(KeyboardFocusableFundamentalComponent):
     """
     # TextInput
 
     A user-editable text field.
 
     `TextInput` allows the user to enter a short text. The text can either be
```

### Comparing `rio_ui-0.5.1/rio/components/theme_context_switcher.py` & `rio_ui-0.5.2/rio/components/theme_context_switcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "ThemeContextSwitcher",
 ]
 
 
+@final
 class ThemeContextSwitcher(FundamentalComponent):
     """
     # ThemeContextSwitcher
 
     A container which can switch between different components.
 
     A `ThemeContextSwitcher` is a container which can switch between different
```

### Comparing `rio_ui-0.5.1/rio/components/tooltip.py` & `rio_ui-0.5.2/rio/components/tooltip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
-from typing import Literal
+from typing import Literal, final
 
 import rio
 
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "Tooltip",
 ]
 
 
+@final
 class Tooltip(FundamentalComponent):
     """
     # Tooltip
 
     A small pop-up window that appears when the user hovers over an element.
 
     `Tooltip` is a small pop-up window that appears when the user hovers over an
```

### Comparing `rio_ui-0.5.1/rio/components/website.py` & `rio_ui-0.5.2/rio/components/website.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from typing import *  # type: ignore
+from typing import final
 
 from ..common import URL
 from .fundamental_component import FundamentalComponent
 
 __all__ = [
     "Website",
 ]
 
 
+@final
 class Website(FundamentalComponent):
     """
     # Website
 
     Displays a website.
 
     `Website` takes a URL as input and displays that website in your app.
```

### Comparing `rio_ui-0.5.1/rio/dataclass.py` & `rio_ui-0.5.2/rio/dataclass.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/debug/client_side_debugger/component_details.py` & `rio_ui-0.5.2/rio/debug/client_side_debugger/component_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             *,
             width: int = 1,
         ) -> None:
             result.add(
                 rio.Text(
                     text,
                     style="dim" if is_label else "text",
-                    align_x=1 if is_label else 0,
+                    justify='right' if is_label else 'left',
                 ),
                 row_index,
                 column_index,
                 width=width,
             )
 
         # Any values which should be displayed right in the title
@@ -122,15 +122,15 @@
 
         if target.key is not None:
             header_accessories = [
                 rio.Icon("material/key", fill="dim"),
                 rio.Text(
                     target.key,
                     style="dim",
-                    align_x=0,
+                        justify='left',
                 ),
             ]
 
         # Title
         result.add(
             rio.Row(
                 rio.Text(
@@ -156,15 +156,15 @@
         except ValueError:
             pass
 
         result.add(
             rio.Text(
                 f"{file} line {line}",
                 style="dim",
-                align_x=0,
+                        justify='left',
             ),
             row_index,
             0,
             width=4,
         )
         row_index += 1
 
@@ -223,16 +223,16 @@
 
                 py_height_str = repr(py_height_str)
 
             # Spacing to separate the table from the rest
             row_index += 1
 
             # Header
-            result.add(rio.Text("width", style="dim", align_x=0), row_index, 1)
-            result.add(rio.Text("height", style="dim", align_x=0), row_index, 2)
+            result.add(rio.Text("width", style="dim",  justify='left'), row_index, 1)
+            result.add(rio.Text("height", style="dim", justify='left'), row_index, 2)
             row_index += 1
 
             # The size as specified in Python
             add_cell("python", 0, True)
             add_cell(py_width_str, 1, False)
             add_cell(py_height_str, 2, False)
             row_index += 1
```

### Comparing `rio_ui-0.5.1/rio/debug/client_side_debugger/debugger.py` & `rio_ui-0.5.2/rio/debug/client_side_debugger/debugger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import *  # type: ignore
 
-import rio
+import rio.components.class_container
+import rio.components.debugger_connector
 
 from . import (
     deploy_page,
     docs_page,
     icons_page,
     project_page,
     theme_picker_page,
```

### Comparing `rio_ui-0.5.1/rio/debug/client_side_debugger/deploy_page.py` & `rio_ui-0.5.2/rio/debug/client_side_debugger/deploy_page.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class DeployPage(rio.Component):
     def build(self) -> rio.Component:
         return rio.Column(
             rio.Text(
                 "Deploy",
                 style="heading2",
                 margin=1,
-                align_x=0,
+                justify='left',
             ),
             rio.Column(
                 rio.Icon(
                     "material/rocket-launch",
                     width=6,
                     height=6,
                     margin_bottom=3,
```

### Comparing `rio_ui-0.5.1/rio/debug/client_side_debugger/docs_page.py` & `rio_ui-0.5.2/rio/debug/client_side_debugger/docs_page.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class DocsPage(rio.Component):
     def build(self) -> rio.Component:
         return rio.Column(
             rio.Text(
                 "Documentation",
                 style="heading2",
                 margin=1,
-                align_x=0,
+                justify='left',
             ),
             rio.Column(
                 rio.Text(
                     "New here? The Rio tutorial can help you get started.",
                     wrap=True,
                 ),
                 rio.Button(
```

### Comparing `rio_ui-0.5.1/rio/debug/client_side_debugger/icons_page.py` & `rio_ui-0.5.2/rio/debug/client_side_debugger/icons_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,21 @@
         self.selected_variant = variant
 
     def build_details(self) -> rio.Component:
         assert self.selected_icon is not None
         children = []
 
         # Heading
-        children.append(rio.Text("Configure", style="heading3", align_x=0))
+        children.append(
+            rio.Text(
+                "Configure",
+                style="heading3",
+                justify='left',
+            )
+        )
 
         # Fill
         children.append(
             rio.Dropdown(
                 label="Fill",
                 options=[
                     "primary",
@@ -275,15 +281,15 @@
         python_source = f"rio.Icon(\n    {params_str},\n)"
 
         # Code sample
         children.append(
             rio.Text(
                 "Example Code",
                 style="heading3",
-                align_x=0,
+                justify='left',
                 margin_top=1,
             )
         )
 
         children.append(
             rio.Markdown(
                 f"""
```

### Comparing `rio_ui-0.5.1/rio/debug/client_side_debugger/project_page.py` & `rio_ui-0.5.2/rio/debug/client_side_debugger/project_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,21 +32,21 @@
         # ignored (except for the project name). Display the data and edit the
         # file if the user changes the values!
 
         return rio.Column(
             rio.Text(
                 project_name,
                 style="heading2",
-                align_x=0,
+                justify='left',
             ),
             rio.Text(
                 str(self.project.project_directory),
                 style="dim",
                 margin_bottom=2,
-                align_x=0,
+                justify='left',
             ),
             rio.Text(
                 "To launch your project, Rio needs to know the name of your python module and in which variable you've stored your app. You can configure those here.",
                 wrap=True,
             ),
             rio.TextInput(
                 label="Main Module",
```

### Comparing `rio_ui-0.5.1/rio/debug/client_side_debugger/sample_icons_grid.py` & `rio_ui-0.5.2/rio/debug/client_side_debugger/sample_icons_grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/debug/client_side_debugger/theme_picker_page.py` & `rio_ui-0.5.2/rio/debug/client_side_debugger/theme_picker_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,23 +197,23 @@
                         rio.Text(
                             self.palette_nicename,
                             style=rio.TextStyle(
                                 # font_size=self.session.theme.heading3_style.font_size,
                                 fill=palette.foreground,
                             ),
                             selectable=False,
-                            align_x=0,
+                justify='left',
                         ),
                         rio.Text(
                             f"#{palette.background.hex}",
                             style=rio.TextStyle(
                                 font_size=1,
                                 fill=palette.foreground.replace(opacity=0.5),
                             ),
-                            align_x=0,
+                justify='left',
                         ),
                         spacing=0.2,
                         margin_x=1,
                         margin_y=0.8,
                     ),
                     fill=palette.background,
                     corner_radius=(
@@ -342,15 +342,15 @@
         return rio.ScrollContainer(
             content=rio.Column(
                 # Main Colors
                 # rio.Text(
                 #     "Theme Colors",
                 #     style="heading3",
                 #     margin_bottom=1,
-                #     align_x=0,
+                #     justify='left',
                 # ),
                 PalettePicker(
                     shared_open_key=self.bind().shared_open_key,
                     palette_nicename="Primary",
                     palette_attribute_name="primary_palette",
                     is_colorful_palette=False,
                     round_top=True,
@@ -415,24 +415,24 @@
                 ),
                 # Corner radii
                 rio.Text(
                     "Corner Radii",
                     style="heading3",
                     margin_top=1,
                     margin_bottom=1,
-                    align_x=0,
+                    justify='left',
                 ),
                 radius_sliders,
                 # Theme Variants
                 rio.Text(
                     "Theme Variants",
                     style="heading3",
                     margin_top=1,
                     margin_bottom=1,
-                    align_x=0,
+                    justify='left',
                 ),
                 rio.Row(
                     rio.Spacer(),
                     rio.IconButton(
                         "material/light-mode",
                         style="minor" if self.create_light_theme else "plain",
                         on_press=self._toggle_create_light_theme,
@@ -447,15 +447,15 @@
                 ),
                 # Code Sample
                 rio.Text(
                     "Code Sample",
                     style="heading3",
                     margin_top=1,
                     # margin_bottom=1,  Not used for now, since markdown has an oddly large margin anyway
-                    align_x=0,
+                    justify='left',
                 ),
                 rio.Markdown(
                     f"""
 ```python
 {get_source_for_theme(self.session.theme, create_theme_pair=self.create_light_theme and self.create_dark_theme)}
 ```
                     """,
```

### Comparing `rio_ui-0.5.1/rio/debug/client_side_debugger/tree_page.py` & `rio_ui-0.5.2/rio/debug/client_side_debugger/tree_page.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import *  # type: ignore
 
-import rio
+import rio.components.component_tree
 
 from . import component_details
 
 
 class TreePage(rio.Component):
     _selected_component_id: int | None = None
 
@@ -15,15 +15,15 @@
         margin = 1
 
         children = [
             rio.Text(
                 "Component Tree",
                 style="heading2",
                 margin=margin,
-                align_x=0,
+                justify="left",
             ),
             rio.components.component_tree.ComponentTree(
                 width=10,
                 height="grow",
                 margin_left=margin,
                 on_select_component=self._on_select_component,
             ),
```

### Comparing `rio_ui-0.5.1/rio/debug/monkeypatches.py` & `rio_ui-0.5.2/rio/debug/monkeypatches.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/debug/stress_client/stress_client.py` & `rio_ui-0.5.2/rio/debug/stress_client/stress_client.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/debug/typing_utils.py` & `rio_ui-0.5.2/rio/debug/typing_utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/debug/validator.py` & `rio_ui-0.5.2/rio/debug/validator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/docs/custom.py` & `rio_ui-0.5.2/rio/docs/custom.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/docs/models.py` & `rio_ui-0.5.2/rio/docs/models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/docs/parsers.py` & `rio_ui-0.5.2/rio/docs/parsers.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/errors.py` & `rio_ui-0.5.2/rio/errors.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/event.py` & `rio_ui-0.5.2/rio/event.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/fills.py` & `rio_ui-0.5.2/rio/fills.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/global_state.py` & `rio_ui-0.5.2/rio/global_state.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/icon_registry.py` & `rio_ui-0.5.2/rio/icon_registry.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/inspection.py` & `rio_ui-0.5.2/rio/inspection.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/maybes.py` & `rio_ui-0.5.2/rio/maybes.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/patches_for_3rd_party_stuff.py` & `rio_ui-0.5.2/rio/patches_for_3rd_party_stuff.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/routing.py` & `rio_ui-0.5.2/rio/routing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
 import logging
 from collections.abc import Callable, Iterable
 from dataclasses import KW_ONLY, dataclass, field
+from typing import final
 
 import rio
 
 from . import common
 from .errors import NavigationFailed
 
 __all__ = ["Page"]
 
 
+@final
 @dataclass(frozen=True)
 class Page:
     """
     A routable page in a Rio app.
 
     Rio apps can consist of many pages. You might have a welcome page, a
     settings page, a login, and so on. `Page` components contain all information
```

### Comparing `rio_ui-0.5.1/rio/serialization.py` & `rio_ui-0.5.2/rio/serialization.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/session.py` & `rio_ui-0.5.2/rio/session.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/README.md` & `rio_ui-0.5.2/rio/snippets/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/__init__.py` & `rio_ui-0.5.2/rio/snippets/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/assets/jane-doe.jpg` & `rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/assets/jane-doe.jpg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/assets/john-doe.jpg` & `rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/assets/john-doe.jpg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/components/about_me.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/components/about_me.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,27 +15,27 @@
                 fill_mode="zoom",
                 margin_right=2,
             ),
             rio.Column(
                 rio.Text(
                     "Jane Doe",
                     style="heading1",
-                    align_x=0,
+                    justify='left',
                 ),
                 rio.Text(
                     "Data Analyst",
-                    align_x=0,
+                    justify='left',
                 ),
                 rio.Text(
                     "AI Researcher",
-                    align_x=0,
+                    justify='left',
                 ),
                 rio.Text(
                     "Python Developer",
-                    align_x=0,
+                    justify='left',
                 ),
                 spacing=0.5,
                 align_y=0,
                 width="grow",
             ),
             width="grow",
         )
```

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/components/contact.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/components/contact.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             )
 
         # Combine everything
         result = rio.Row(
             image,
             rio.Text(
                 self.text,
-                align_x=0,
+                    justify='left',
                 width="grow",
             ),
             width="grow",
             margin=0.2,
         )
 
         # If a link is provided, wrap the result in a link
```

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/components/history.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/components/history.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,28 +26,28 @@
                     margin_right=2,
                     align_x=0,
                     align_y=0,
                 ),
                 rio.Column(
                     rio.Text(
                         f"{self.from_string} - {self.to_string}",
-                        align_x=0,
+                    justify='left',
                         style=rio.TextStyle(fill=rio.Color.GREY),
                     ),
                     rio.Text(
                         f"{self.title} at {self.organization}",
                         style="heading3",
-                        align_x=0,
+                    justify='left',
                     ),
                     rio.Revealer(
                         None,
                         rio.Text(
                             self.details,
                             wrap=True,
-                            align_x=0,
+                    justify='left',
                         ),
                         is_open=self.is_open,
                     ),
                     spacing=0.3,
                     width="grow",
                     align_y=0,
                 ),
```

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/components/projects.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/components/projects.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/components/skill_bars.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/components/skill_bars.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         rows = []
 
         for name, level in self.skills.items():
             rows.append(
                 rio.Column(
                     rio.Text(
                         name,
-                        align_x=0,
+                    justify='left',
                     ),
                     rio.ProgressBar(
                         level / 10,
                     ),
                 )
             )
```

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/old-tutorial-biography/pages/biography_page.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/old-tutorial-biography/pages/biography_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/other-examples/simple_counter_app.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/other-examples/simple_counter_app.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/README.md` & `rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/__init__.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # <additional-imports>
 import openai
 
-import rio
-
 # </additional-imports>
 
 
 # <additional-code>
 OPENAI_API_KEY = "<placeholder>"  # Replace this with your OpenAI API key
```

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg` & `rio_ui-0.5.2/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Empty/components/sample_component.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Empty/components/sample_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg` & `rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Simple Dashboard/assets/smartphone-sales-clean.csv` & `rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple Dashboard/assets/smartphones.csv`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Simple Dashboard/pages/interactive_plot.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple Dashboard/pages/interactive_plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,58 @@
-import urllib.request
-from pathlib import Path
-
-import pandas as pd
-import plotly.graph_objs as go
+from dataclasses import field
 
 import rio
 
-# Load the dataset
-CSV_PATH = Path(__file__).parent / "smartphone-sales.csv"
-CSV_URL = "https://TODO-real-url.com"
-
-if not CSV_PATH.exists():
-    with urllib.request.urlopen(CSV_URL) as response:
-        CSV_PATH.write_bytes(response.read())
+# <additional-imports>
+import pandas as pd
+import plotly.graph_objs as go
 
-raw_df = pd.read_csv(CSV_PATH)
-raw_df = raw_df.head(1000)
+# </additional-imports>
 
 
 # <component>
 class InteractivePlot(rio.Component):
-    x_axis: str = raw_df.columns[0]
-    y_axis: str = raw_df.columns[1]
+    # The full dataset, containing all smartphone data. This will be loaded when
+    # the component is initialized. See the `load_data` method for details.
+    dataset: pd.DataFrame = field(default_factory=pd.DataFrame)
+
+    # The currently selected columns to display in the scatterplot. These values
+    # will be initializes when the dataset is loaded.
+    x_axis: str = ""
+    y_axis: str = ""
 
+    # If this is `True`, we'll take care to remove unlikely data by keeping only
+    # the tenth to ninetieth percentile of the dataset.
     remove_outliers: bool = False
 
+    @rio.event.on_populate
+    def load_data(self) -> None:
+        self.dataset = pd.read_csv(
+            self.session.assets / "smartphones.csv",
+        )
+        self.x_axis = self.dataset.columns[0]
+        self.y_axis = self.dataset.columns[1]
+
     async def on_download_csv(self) -> None:
         # Build a CSV file from the selected columns
-        selected_df = raw_df[[self.x_axis, self.y_axis]]
+        selected_df = self.dataset[[self.x_axis, self.y_axis]]
         csv = selected_df.to_csv(index=False)
 
         # Save the file
         await self.session.save_file(
             file_name="scatter.csv",
             file_contents=csv,
         )
 
     def filter_data(self) -> pd.DataFrame:
         """
         Remove outliers from the dataset, by keeping only the tenth to ninetieth
         percentile.
         """
-        result = raw_df
+        result = self.dataset
 
         # Remove outliers in the x-axis
         series = result[self.x_axis]
 
         if series.dtype in [int, float]:
             lower = series.quantile(0.10)
             upper = series.quantile(0.90)
@@ -64,15 +71,15 @@
         return result
 
     def build(self) -> rio.Component:
         # Fetch the data
         if self.remove_outliers:
             df = self.filter_data()
         else:
-            df = raw_df
+            df = self.dataset
 
         # Build the plot
         return rio.Row(
             rio.Plot(
                 go.Figure(
                     go.Scatter(
                         x=df[self.x_axis],
```

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Simple Dashboard/thumbnail.svg` & `rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py` & `rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg` & `rio_ui-0.5.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/state_properties.py` & `rio_ui-0.5.2/rio/state_properties.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/text_style.py` & `rio_ui-0.5.2/rio/text_style.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/theme.py` & `rio_ui-0.5.2/rio/theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         hue=hue,
         saturation=map_range(saturation, 0.5, 1, 1, 0),
         value=min(target_brightness * 2, 1),
         opacity=color.opacity,
     )
 
 
+@final
 @dataclass(frozen=True)
 class Palette:
     background: rio.Color
     background_variant: rio.Color
     background_active: rio.Color
 
     foreground: rio.Color
@@ -110,14 +111,15 @@
             background_active=common.first_non_null(
                 background_active, self.background_active
             ),
             foreground=common.first_non_null(foreground, self.foreground),
         )
 
 
+@final
 @dataclass(frozen=True)
 class Theme:
     """
     Defines the visual style of the application.
 
     The `Theme` contains all colors, text styles, and other visual properties
     that are used throughout the application. If you wish to change the
```

### Comparing `rio_ui-0.5.1/rio/user_settings_module.py` & `rio_ui-0.5.2/rio/user_settings_module.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.1/rio/world_units.py` & `rio_ui-0.5.2/rio/world_units.py`

 * *Files identical despite different names*

