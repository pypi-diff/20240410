# Comparing `tmp/digsim-logic-simulator-0.3.0.tar.gz` & `tmp/digsim-logic-simulator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digsim-logic-simulator-0.3.0.tar", last modified: Sat Dec 16 17:13:57 2023, max compression
+gzip compressed data, was "digsim-logic-simulator-0.4.0.tar", last modified: Wed Apr 10 15:52:14 2024, max compression
```

## Comparing `digsim-logic-simulator-0.3.0.tar` & `digsim-logic-simulator-0.4.0.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.480605 digsim-logic-simulator-0.3.0/
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1688 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/LICENSE.md
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      107 2023-12-05 20:35:09.000000 digsim-logic-simulator-0.3.0/MANIFEST.in
--rw-r--r--   0 fredrik   (1000) fredrik   (1000)     6332 2023-12-16 17:13:57.480605 digsim-logic-simulator-0.3.0/PKG-INFO
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3401 2023-12-16 13:57:42.000000 digsim-logic-simulator-0.3.0/README.md
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1708 2023-12-16 17:13:03.000000 digsim-logic-simulator-0.3.0/pyproject.toml
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)       38 2023-12-16 17:13:57.480605 digsim-logic-simulator-0.3.0/setup.cfg
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.460605 digsim-logic-simulator-0.3.0/src/
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.460605 digsim-logic-simulator-0.3.0/src/digsim/
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      151 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/__init__.py
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.460605 digsim-logic-simulator-0.3.0/src/digsim/app/
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1370 2023-12-09 11:00:01.000000 digsim-logic-simulator-0.3.0/src/digsim/app/__main__.py
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.464604 digsim-logic-simulator-0.3.0/src/digsim/app/gui/
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      167 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui/__init__.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    16482 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui/_circuit_area.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     6425 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui/_component_selection.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     5312 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui/_main_window.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    13150 2023-12-09 10:09:56.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui/_top_bar.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      660 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui/_utils.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1533 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui/_warning_dialog.py
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.464604 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      266 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/__init__.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3095 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_bus_bit_object.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3354 2023-12-16 16:54:43.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_buzzer_object.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2818 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_component_context_menu.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    13236 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_component_object.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2091 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_component_port_item.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3612 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_dip_switch_object.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2606 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_gui_note_object.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2467 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_gui_object_factory.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1928 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_hexdigit_object.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     7588 2023-12-09 10:12:50.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_image_objects.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3572 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_label_object.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2674 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_logic_analyzer_object.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     4262 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_seven_segment_object.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2763 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_shortcut_objects.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      955 2023-12-09 11:31:36.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_yosys_object.py
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.468605 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    12062 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/AND.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1591 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/Analyzer.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    12819 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/BUF.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     5856 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/Buzzer.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3117 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/Clock.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     9038 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/DFF.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    16899 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/DIP_SWITCH.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     4452 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/FlipFlop.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     5493 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/IC.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     7075 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/LED_OFF.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     9389 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/LED_ON.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1912 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/MUX.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    11718 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/NAND.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    15091 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/NOR.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    12593 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/NOT.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1212 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/ONE.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    14870 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/OR.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     8468 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/PB.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     4752 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/Switch_OFF.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     4819 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/Switch_ON.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    14610 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/XNOR.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    16118 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/XOR.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3117 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/YOSYS.png
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3459 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/ZERO.png
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.468605 digsim-logic-simulator-0.3.0/src/digsim/app/images/
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    16041 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/images/app_icon.png
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.472605 digsim-logic-simulator-0.3.0/src/digsim/app/model/
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      161 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/model/__init__.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     6551 2023-12-09 10:34:43.000000 digsim-logic-simulator-0.3.0/src/digsim/app/model/_model.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     6500 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/model/_model_components.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1810 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/model/_model_new_wire.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     5078 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/model/_model_objects.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1141 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/model/_model_settings.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2511 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/model/_model_shortcuts.py
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.472605 digsim-logic-simulator-0.3.0/src/digsim/app/settings/
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      310 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/settings/__init__.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    16311 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/settings/_component_settings.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2801 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/settings/_gui_settings.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1561 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/app/settings/_shortcut_dialog.py
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.472605 digsim-logic-simulator-0.3.0/src/digsim/circuit/
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      218 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/__init__.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    11823 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/_circuit.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1710 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/_waves_writer.py
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.476605 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1269 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/__init__.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1912 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_bus_bits.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1030 2023-12-09 12:10:40.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_button.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1125 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_buzzer.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1487 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_clock.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1807 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_dip_switch.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2942 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_flip_flops.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     7192 2023-12-09 11:51:54.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_gates.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2257 2023-12-07 20:16:08.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_hexdigit.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      916 2023-12-09 10:14:05.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_ic.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     5112 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_label_wire.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      454 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_led.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1809 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_logic_analyzer.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1482 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_mem64kbyte.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1255 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_memstdout.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      602 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_note.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1202 2023-12-09 12:10:40.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_on_off_switch.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      798 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_seven_segment.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      679 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_static_level.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1236 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_static_value.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    37737 2023-12-07 20:15:45.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_yosys_atoms.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     8888 2023-12-16 13:57:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_yosys_component.py
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.476605 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/atoms/
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      485 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/atoms/__init__.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     9865 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/atoms/_component.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      173 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/atoms/_digsim_exception.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    12159 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/atoms/_port.py
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.476605 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/ic/
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    26632 2023-12-13 16:33:58.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/ic/74162.json
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    21211 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/circuit/components/ic/7448.json
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.476605 digsim-logic-simulator-0.3.0/src/digsim/synth/
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      182 2023-12-09 10:47:03.000000 digsim-logic-simulator-0.3.0/src/digsim/synth/__init__.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2175 2023-12-16 13:57:42.000000 digsim-logic-simulator-0.3.0/src/digsim/synth/__main__.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     4047 2023-12-16 17:04:39.000000 digsim-logic-simulator-0.3.0/src/digsim/synth/_synthesis.py
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.476605 digsim-logic-simulator-0.3.0/src/digsim/utils/
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      169 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/utils/__init__.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     8562 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/src/digsim/utils/_yosys_netlist.py
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.480605 digsim-logic-simulator-0.3.0/src/digsim_logic_simulator.egg-info/
--rw-r--r--   0 fredrik   (1000) fredrik   (1000)     6332 2023-12-16 17:13:57.000000 digsim-logic-simulator-0.3.0/src/digsim_logic_simulator.egg-info/PKG-INFO
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     4624 2023-12-16 17:13:57.000000 digsim-logic-simulator-0.3.0/src/digsim_logic_simulator.egg-info/SOURCES.txt
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)        1 2023-12-16 17:13:57.000000 digsim-logic-simulator-0.3.0/src/digsim_logic_simulator.egg-info/dependency_links.txt
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)       84 2023-12-16 17:13:57.000000 digsim-logic-simulator-0.3.0/src/digsim_logic_simulator.egg-info/requires.txt
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)        7 2023-12-16 17:13:57.000000 digsim-logic-simulator-0.3.0/src/digsim_logic_simulator.egg-info/top_level.txt
-drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2023-12-16 17:13:57.480605 digsim-logic-simulator-0.3.0/tests/
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     7367 2023-12-16 17:06:49.000000 digsim-logic-simulator-0.3.0/tests/test_gates.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3605 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/tests/test_yosys_aldff.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     5292 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/tests/test_yosys_dff.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2547 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/tests/test_yosys_dlatch.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    18075 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/tests/test_yosys_gates.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2547 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/tests/test_yosys_latch.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     6036 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/tests/test_yosys_netlist.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     6619 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/tests/test_yosys_sdff.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     7615 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.3.0/tests/test_yosys_sr.py
--rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2833 2023-12-16 16:52:00.000000 digsim-logic-simulator-0.3.0/tests/test_yosys_synth.py
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.862140 digsim-logic-simulator-0.4.0/
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1688 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/LICENSE.md
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      107 2023-12-05 20:35:09.000000 digsim-logic-simulator-0.4.0/MANIFEST.in
+-rw-r--r--   0 fredrik   (1000) fredrik   (1000)     6332 2024-04-10 15:52:14.862140 digsim-logic-simulator-0.4.0/PKG-INFO
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3401 2023-12-16 13:57:42.000000 digsim-logic-simulator-0.4.0/README.md
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1989 2024-04-10 15:50:19.000000 digsim-logic-simulator-0.4.0/pyproject.toml
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)       38 2024-04-10 15:52:14.862140 digsim-logic-simulator-0.4.0/setup.cfg
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.850142 digsim-logic-simulator-0.4.0/src/
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.850142 digsim-logic-simulator-0.4.0/src/digsim/
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      149 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/__init__.py
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.854141 digsim-logic-simulator-0.4.0/src/digsim/app/
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1368 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/__main__.py
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.854141 digsim-logic-simulator-0.4.0/src/digsim/app/gui/
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      165 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui/__init__.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    16366 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui/_circuit_area.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     6388 2024-02-01 19:51:04.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui/_component_selection.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     5275 2024-02-01 19:51:07.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui/_main_window.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    13066 2024-02-01 19:51:10.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui/_top_bar.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      660 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui/_utils.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1496 2024-02-01 19:51:13.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui/_warning_dialog.py
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.854141 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      264 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/__init__.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3059 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_bus_bit_object.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3352 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_buzzer_object.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2821 2024-04-10 15:50:15.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_component_context_menu.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    13078 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_component_object.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2089 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_component_port_item.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3576 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_dip_switch_object.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2604 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_gui_note_object.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2465 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_gui_object_factory.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1926 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_hexdigit_object.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     7553 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_image_objects.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3570 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_label_object.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2671 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_logic_analyzer_object.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     4227 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_seven_segment_object.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2724 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_shortcut_objects.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      953 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_yosys_object.py
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.858141 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    12062 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/AND.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1591 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/Analyzer.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    12819 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/BUF.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     5856 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/Buzzer.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3117 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/Clock.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     9038 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/DFF.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    16899 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/DIP_SWITCH.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     4452 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/FlipFlop.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     5493 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/IC.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     7075 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/LED_OFF.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     9389 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/LED_ON.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1912 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/MUX.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    11718 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/NAND.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    15091 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/NOR.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    12593 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/NOT.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1212 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/ONE.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    14870 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/OR.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     8468 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/PB.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     4752 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/Switch_OFF.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     4819 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/Switch_ON.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    14610 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/XNOR.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    16118 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/XOR.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3117 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/YOSYS.png
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3459 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/ZERO.png
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.858141 digsim-logic-simulator-0.4.0/src/digsim/app/images/
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    16041 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/images/app_icon.png
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.858141 digsim-logic-simulator-0.4.0/src/digsim/app/model/
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      159 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/model/__init__.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     6506 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/model/_model.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     6500 2024-01-31 19:43:13.000000 digsim-logic-simulator-0.4.0/src/digsim/app/model/_model_components.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1810 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/model/_model_new_wire.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     5040 2024-02-01 19:51:40.000000 digsim-logic-simulator-0.4.0/src/digsim/app/model/_model_objects.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1141 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/app/model/_model_settings.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2511 2024-01-31 19:43:13.000000 digsim-logic-simulator-0.4.0/src/digsim/app/model/_model_shortcuts.py
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.858141 digsim-logic-simulator-0.4.0/src/digsim/app/settings/
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      308 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/app/settings/__init__.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    16279 2024-02-01 19:51:43.000000 digsim-logic-simulator-0.4.0/src/digsim/app/settings/_component_settings.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2764 2024-02-01 19:51:45.000000 digsim-logic-simulator-0.4.0/src/digsim/app/settings/_gui_settings.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1524 2024-02-01 19:51:48.000000 digsim-logic-simulator-0.4.0/src/digsim/app/settings/_shortcut_dialog.py
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.858141 digsim-logic-simulator-0.4.0/src/digsim/circuit/
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      216 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/__init__.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    11748 2024-02-01 19:51:51.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/_circuit.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1645 2024-02-01 19:51:54.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/_waves_writer.py
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.858141 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1267 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/__init__.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1912 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_bus_bits.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1028 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_button.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1123 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_buzzer.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1485 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_clock.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1805 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_dip_switch.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2942 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_flip_flops.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     7157 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_gates.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2255 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_hexdigit.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      917 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_ic.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     5110 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_label_wire.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      452 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_led.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1807 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_logic_analyzer.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1482 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_mem64kbyte.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1255 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_memstdout.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      602 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_note.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1200 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_on_off_switch.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      797 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_seven_segment.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      677 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_static_level.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     1234 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_static_value.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    37599 2024-02-01 19:52:00.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_yosys_atoms.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     8810 2024-02-01 19:52:03.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_yosys_component.py
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.858141 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/atoms/
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      483 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/atoms/__init__.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     9824 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/atoms/_component.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      173 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/atoms/_digsim_exception.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    12119 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/atoms/_port.py
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.858141 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/ic/
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    26632 2023-12-13 16:33:58.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/ic/74162.json
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    21211 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/circuit/components/ic/7448.json
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.862140 digsim-logic-simulator-0.4.0/src/digsim/synth/
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      180 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/synth/__init__.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2173 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/synth/__main__.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     4271 2024-02-01 18:57:59.000000 digsim-logic-simulator-0.4.0/src/digsim/synth/_synthesis.py
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.862140 digsim-logic-simulator-0.4.0/src/digsim/utils/
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)      167 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/src/digsim/utils/__init__.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     8562 2023-12-05 20:22:42.000000 digsim-logic-simulator-0.4.0/src/digsim/utils/_yosys_netlist.py
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.862140 digsim-logic-simulator-0.4.0/src/digsim_logic_simulator.egg-info/
+-rw-r--r--   0 fredrik   (1000) fredrik   (1000)     6332 2024-04-10 15:52:14.000000 digsim-logic-simulator-0.4.0/src/digsim_logic_simulator.egg-info/PKG-INFO
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     4624 2024-04-10 15:52:14.000000 digsim-logic-simulator-0.4.0/src/digsim_logic_simulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)        1 2024-04-10 15:52:14.000000 digsim-logic-simulator-0.4.0/src/digsim_logic_simulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)       84 2024-04-10 15:52:14.000000 digsim-logic-simulator-0.4.0/src/digsim_logic_simulator.egg-info/requires.txt
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)        7 2024-04-10 15:52:14.000000 digsim-logic-simulator-0.4.0/src/digsim_logic_simulator.egg-info/top_level.txt
+drwxrwxr-x   0 fredrik   (1000) fredrik   (1000)        0 2024-04-10 15:52:14.862140 digsim-logic-simulator-0.4.0/tests/
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     7366 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/tests/test_gates.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     3603 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/tests/test_yosys_aldff.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     5290 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/tests/test_yosys_dff.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2545 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/tests/test_yosys_dlatch.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)    18073 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/tests/test_yosys_gates.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2545 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/tests/test_yosys_latch.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     6035 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/tests/test_yosys_netlist.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     6617 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/tests/test_yosys_sdff.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     7579 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/tests/test_yosys_sr.py
+-rw-rw-r--   0 fredrik   (1000) fredrik   (1000)     2904 2024-03-20 18:39:14.000000 digsim-logic-simulator-0.4.0/tests/test_yosys_synth.py
```

### Comparing `digsim-logic-simulator-0.3.0/LICENSE.md` & `digsim-logic-simulator-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/PKG-INFO` & `digsim-logic-simulator-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digsim-logic-simulator
-Version: 0.3.0
+Version: 0.4.0
 Summary: Interactive Digital Logic Simulator
 Author-email: Fredrik Andersson <freand@gmail.com>
 Maintainer-email: Fredrik Andersson <freand@gmail.com>
 License: The Clear BSD License
         
         Copyright (c) 2023, Fredrik Andersson
         All rights reserved.
```

### Comparing `digsim-logic-simulator-0.3.0/README.md` & `digsim-logic-simulator-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/__main__.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" The main class module of the digsim.app namespace """
+"""The main class module of the digsim.app namespace"""
 
 import argparse
 import sys
 from pathlib import Path
 
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QIcon, QPainter, QPixmap
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui/_circuit_area.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui/_circuit_area.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
 """The circuit area and component widget"""
 
-# pylint: disable=unused-argument
-# pylint: disable=useless-parent-delegation
-# pylint: disable=too-few-public-methods
-
 from functools import partial
 
 from PySide6.QtCore import QPoint, QPointF, QRect, QRectF, Qt, QTimer
 from PySide6.QtGui import QBrush, QPainterPath, QPen
 from PySide6.QtWidgets import (
     QGraphicsItem,
     QGraphicsPathItem,
@@ -19,15 +15,14 @@
     QGraphicsView,
 )
 
 from digsim.app.settings import ComponentSettingsDialog
 
 
 class WirePartGraphicsItem(QGraphicsRectItem):
-
     """A part of a wire graphcis item"""
 
     CLOSE_TO_WIRE_MARGIN = 10
 
     def __init__(self, app_model, src_port, parent, point_pair):
         src, dst = point_pair
         x_low, x_high = (src.x(), dst.x()) if src.x() < dst.x() else (dst.x(), src.x())
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui/_component_selection.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui/_component_selection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
 """Module for the component selection classes"""
 
-# pylint: disable=too-few-public-methods
-
 from functools import partial
 
 from PySide6.QtCore import QMimeData, QSize, Qt, QTimer
 from PySide6.QtGui import QDrag, QPainter, QPixmap
 from PySide6.QtWidgets import QFrame, QLabel, QPushButton, QVBoxLayout, QWidget
 
 import digsim.app.gui_objects
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui/_main_window.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui/_main_window.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
 """The main window and widgets of the digsim gui application"""
 
-# pylint: disable=too-few-public-methods
-
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QKeySequence, QShortcut
 from PySide6.QtWidgets import (
     QHBoxLayout,
     QMainWindow,
     QMessageBox,
     QScrollArea,
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui/_top_bar.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui/_top_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
 """The top bar of the main window/gui application"""
 
-# pylint: disable=too-few-public-methods
-# pylint: disable=too-many-instance-attributes
-
 from pathlib import Path
 
 import qtawesome as qta
 
 from PySide6.QtCore import Qt, QTimer
 from PySide6.QtWidgets import (
     QCheckBox,
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui/_utils.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui/_utils.py`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui/_warning_dialog.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui/_warning_dialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
 """A warning dialog"""
 
-# pylint: disable=too-few-public-methods
-
 from PySide6.QtCore import QSize, Qt
 from PySide6.QtWidgets import (
     QDialog,
     QDialogButtonBox,
     QFrame,
     QHBoxLayout,
     QLabel,
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_bus_bit_object.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_bus_bit_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
-""" A hexdigit component placed in the GUI """
+"""A hexdigit component placed in the GUI"""
 
 from PySide6.QtCore import QPoint, QSize, Qt
 from PySide6.QtGui import QPen
 
 from ._component_object import ComponentObject
 
 
-# pylint: disable=too-many-arguments
-
-
 class BusBitsObject(ComponentObject):
     """The class for a bus/bit component placed in the GUI"""
 
     WIRE_LENGTH_COMPONENT = 5
     WIRE_LENGTH_SELECTABLE = 15
     PORT_DISTANCE = 10
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_buzzer_object.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_buzzer_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" A buzzer component object """
+"""A buzzer component object"""
 
 from math import pi, sin
 from struct import pack
 
 from PySide6.QtCore import QByteArray, QIODevice
 from PySide6.QtMultimedia import QAudioFormat, QAudioSink, QMediaDevices
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_component_context_menu.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_component_context_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" A component context menu """
+"""A component context menu"""
 
 from PySide6.QtGui import QAction
 from PySide6.QtWidgets import QMenu
 
 from digsim.app.settings import ComponentSettingsDialog
 
 
@@ -54,15 +54,15 @@
         self._menu_action = self.exec_(position)
 
     def get_action(self):
         """Get context menu action"""
         return self._menu_action.text() if self._menu_action is not None else ""
 
     def _delete(self):
-        self._component_object.select(True)
+        self._component_object.setSelected(True)
         self._app_model.objects.delete_selected()
 
     def _raise(self):
         self._app_model.objects.components.bring_to_front(self._component_object)
 
     def _lower(self):
         self._app_model.objects.components.send_to_back(self._component_object)
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_component_object.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_component_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
-""" A component placed in the GUI """
-
-# pylint: disable=unused-argument
-# pylint: disable=too-many-public-methods
-# pylint: disable=too-many-instance-attributes
-# pylint: disable=too-many-arguments
+"""A component placed in the GUI"""
 
 import abc
 
 from PySide6.QtCore import QPoint, QRect, QSize, Qt
 from PySide6.QtGui import QFont, QFontMetrics, QPen
 from PySide6.QtWidgets import QGraphicsItem, QGraphicsRectItem
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_component_port_item.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_component_port_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" A component port graphics item """
+"""A component port graphics item"""
 
 from PySide6.QtCore import QRect, Qt
 from PySide6.QtGui import QBrush, QPen
 from PySide6.QtWidgets import QGraphicsRectItem
 
 from digsim.circuit.components.atoms import PortConnectionError
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_dip_switch_object.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_dip_switch_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
-""" A hexdigit component placed in the GUI """
+"""A hexdigit component placed in the GUI"""
 
 from PySide6.QtCore import QPoint, QRect, Qt
 from PySide6.QtGui import QFont, QPen
 
 from ._image_objects import ImageObject
 
 
-# pylint: disable=too-many-arguments
-
-
 class DipSwitchObject(ImageObject):
     """The class for a bus/bit component placed in the GUI"""
 
     IMAGE_FILENAME = "images/DIP_SWITCH.png"
     DIP_SWITCH_WIDTH = 20
     DIP_SWITCH_HEIGHT = 10
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_gui_note_object.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_gui_note_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" A GUI note object """
+"""A GUI note object"""
 
 from PySide6.QtCore import QPoint, QRect, Qt
 from PySide6.QtGui import QFont, QFontMetrics, QPen
 
 from ._component_object import ComponentObject
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_gui_object_factory.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_gui_object_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" A GUI component object factory module """
+"""A GUI component object factory module"""
 
 from digsim.circuit.components.atoms import DigsimException
 
 from ._bus_bit_object import BitsBusObject, BusBitsObject
 from ._buzzer_object import BuzzerObject
 from ._dip_switch_object import DipSwitchObject
 from ._gui_note_object import GuiNoteObject
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_hexdigit_object.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_hexdigit_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" A hexdigit component placed in the GUI """
+"""A hexdigit component placed in the GUI"""
 
 from ._component_object import ComponentObject
 from ._seven_segment_object import SevenSegmentObject
 
 
 class HexDigitObject(SevenSegmentObject):
     """The class for a hexdigit component placed in the GUI"""
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_image_objects.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_image_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
-""" A component with an image as symbol the GUI """
-
-# pylint: disable=too-many-arguments
+"""A component with an image as symbol the GUI"""
 
 from pathlib import Path
 
 from PySide6.QtCore import QPoint, Qt
 from PySide6.QtGui import QFont, QPen, QPixmap
 
 from ._component_object import ComponentObject
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_label_object.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_label_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" A label component placed in the GUI """
+"""A label component placed in the GUI"""
 
 from PySide6.QtCore import QPoint, QRect, Qt
 from PySide6.QtGui import QPen, QPolygon
 
 from ._component_object import ComponentObject
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_logic_analyzer_object.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_logic_analyzer_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" A Logic Analyzer component placed in the GUI """
+"""A Logic Analyzer component placed in the GUI"""
 
 from PySide6.QtCore import QPoint, QRect, Qt
 from PySide6.QtGui import QPainterPath, QPen
 
 from ._image_objects import ImageObject
 
 
@@ -19,15 +19,14 @@
 
     def __init__(self, app_model, component, xpos, ypos):
         super().__init__(app_model, component, xpos, ypos)
         self.width = self.SIGNAL_NAME_WIDTH + self.ANALYZER_DISPLAY_WIDTH + 2 * self.RECT_TO_BORDER
         self.update_ports()
 
     def paint_component(self, painter):
-
         self.paint_component_base(painter)
         painter.setBrush(Qt.SolidPattern)
         painter.setBrush(Qt.black)
         painter.drawRoundedRect(
             QRect(
                 self.object_pos.x() + self.SIGNAL_NAME_WIDTH,
                 self.object_pos.y() + 2 * self.RECT_TO_BORDER,
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_seven_segment_object.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_seven_segment_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
-""" A 7-segment component placed in the GUI """
-
-# pylint: disable=too-many-arguments
+"""A 7-segment component placed in the GUI"""
 
 from PySide6.QtCore import QPoint, Qt
 from PySide6.QtGui import QPainterPath
 
 from ._component_object import ComponentObject
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_shortcut_objects.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_shortcut_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
-""" A button component with an image as symbol the GUI """
-
-# pylint: disable=too-few-public-methods
+"""A button component with an image as symbol the GUI"""
 
 from functools import partial
 
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QAction, QPen
 
 from digsim.app.settings import ShortcutDialog
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/_yosys_object.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/_yosys_object.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" A yosys component with an image as symbol the GUI """
+"""A yosys component with an image as symbol the GUI"""
 
 from PySide6.QtGui import QAction
 
 from digsim.circuit.components.atoms import DigsimException
 
 from ._image_objects import ImageObject
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/AND.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/AND.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/Analyzer.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/Analyzer.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/BUF.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/BUF.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/Buzzer.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/Buzzer.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/Clock.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/Clock.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/DFF.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/DFF.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/DIP_SWITCH.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/DIP_SWITCH.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/FlipFlop.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/FlipFlop.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/IC.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/IC.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/LED_OFF.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/LED_OFF.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/LED_ON.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/LED_ON.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/MUX.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/MUX.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/NAND.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/NAND.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/NOR.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/NOR.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/NOT.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/NOT.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/ONE.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/ONE.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/OR.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/OR.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/PB.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/PB.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/Switch_OFF.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/Switch_OFF.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/Switch_ON.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/Switch_ON.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/XNOR.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/XNOR.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/XOR.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/XOR.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/YOSYS.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/YOSYS.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/gui_objects/images/ZERO.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/gui_objects/images/ZERO.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/images/app_icon.png` & `digsim-logic-simulator-0.4.0/src/digsim/app/images/app_icon.png`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/model/_model.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/model/_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
-""" An application model for a GUI simulated circuit """
-
-# pylint: disable=too-many-instance-attributes
+"""An application model for a GUI simulated circuit"""
 
 import json
 import queue
 import time
 from pathlib import Path
 
 from PySide6.QtCore import QThread, Signal
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/model/_model_components.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/model/_model_components.py`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/model/_model_new_wire.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/model/_model_new_wire.py`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/model/_model_objects.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/model/_model_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
 """Handle objects in the model"""
 
-# pylint: disable=too-many-public-methods
-
 from digsim.circuit import Circuit
 from digsim.circuit.components.atoms import DigsimException
 
 from ._model_components import ModelComponents
 from ._model_new_wire import NewWire
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/model/_model_settings.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/model/_model_settings.py`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/model/_model_shortcuts.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/model/_model_shortcuts.py`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/settings/_component_settings.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/settings/_component_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
 """The component settings dialog(s)"""
 
-# pylint: disable=too-many-branches
-
 import pathlib
 
 from PySide6.QtCore import Qt, Signal
 from PySide6.QtWidgets import (
     QCheckBox,
     QComboBox,
     QDialog,
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/settings/_gui_settings.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/settings/_gui_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
 """The GUI settings dialog"""
 
-# pylint: disable=too-few-public-methods
-
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QCheckBox, QComboBox, QDialog, QDialogButtonBox, QGridLayout, QLabel
 
 
 class GuiSettingsDialog(QDialog):
     """GUI Settings Dialog"""
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/app/settings/_shortcut_dialog.py` & `digsim-logic-simulator-0.4.0/src/digsim/app/settings/_shortcut_dialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
 """The shurtcut dialog"""
 
-# pylint: disable=too-few-public-methods
-
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QComboBox, QDialog, QDialogButtonBox, QLabel, QVBoxLayout
 
 
 class ShortcutDialog(QDialog):
     """Shortcut Dialog"""
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/_circuit.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/_circuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
 """
 Module that handles the circuit simulation of components
 """
 
-# pylint: disable=too-many-public-methods
-# pylint: disable=too-many-arguments
-
 import json
 import os
 
 from ._waves_writer import WavesWriter
 from .components.atoms import Component, DigsimException
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/_waves_writer.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/_waves_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
 """
 Module that handles the creation of vcd files
 """
 
-# pylint: disable=consider-using-with
-# pylint: disable=import-error
-
 from vcd import VCDWriter
 
 
 class WavesWriter:
     """Class that handles the creation of vcd files"""
 
     def __init__(self, filename):
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/__init__.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" All classes within digsim.circuit.components namespace """
+"""All classes within digsim.circuit.components namespace"""
 
 from ._bus_bits import Bus2Wires, Wires2Bus  # noqa: F401
 from ._button import PushButton  # noqa: F401
 from ._buzzer import Buzzer  # noqa: F401
 from ._clock import Clock  # noqa: F401
 from ._dip_switch import DipSwitch  # noqa: F401
 from ._flip_flops import SRFF, ClockedJKFF, ClockedSRFF, ClockedTFF, FlipFlop  # noqa: F401
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_bus_bits.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_bus_bits.py`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_button.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_button.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" A PushButton component """
+"""A PushButton component"""
 
 import logging
 
 from .atoms import CallbackComponent, PortOutImmediate
 
 
 class PushButton(CallbackComponent):
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_buzzer.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_buzzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" Module with the Buzzer component """
+"""Module with the Buzzer component"""
 
 from .atoms import CallbackComponent, PortIn
 
 
 class Buzzer(CallbackComponent):
     """Buzzer component class"""
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_clock.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_clock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" Clock component module """
+"""Clock component module"""
 
 from .atoms import CallbackComponent, PortOutDelta, PortOutImmediate
 
 
 class Clock(CallbackComponent):
     """Clock component class"""
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_dip_switch.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_dip_switch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" A Dip-switch component """
+"""A Dip-switch component"""
 
 from .atoms import CallbackComponent, PortOutImmediate
 
 
 class DipSwitch(CallbackComponent):
     """On/Off Switch  component class"""
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_flip_flops.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_flip_flops.py`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_gates.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_gates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
-""" Module with the basic logic gates """
-
-# pylint: disable=too-many-arguments
+"""Module with the basic logic gates"""
 
 import math
 
 from .atoms import Component, ComponentException, MultiComponent, PortIn, PortOutDelta, PortWire
 
 
 class NOT(Component):
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_hexdigit.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_hexdigit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" HexDigit component module """
+"""HexDigit component module"""
 
 from .atoms import CallbackComponent, PortIn
 
 
 class HexDigit(CallbackComponent):
     """HexDigit component class"""
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_ic.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_ic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
 """
 Module for creating a yosys component in the ic folder
 """
+
 from pathlib import Path
 
 from ._yosys_component import YosysComponent
 
 
 class IntegratedCircuit(YosysComponent):
     """IC component class (predefined yosys module)"""
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_label_wire.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_label_wire.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" Label Wire components module """
+"""Label Wire components module"""
 
 from .atoms import Component, DigsimException, PortWire
 
 
 class _LabelWireStorage:
     """Singleton class with label wires"""
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_logic_analyzer.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_logic_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" Module with Logic Analyzer component """
+"""Module with Logic Analyzer component"""
 
 from .atoms import CallbackComponent, PortOutDelta, PortWire
 
 
 class LogicAnalyzer(CallbackComponent):
     """Logic Analyzer component class"""
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_mem64kbyte.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_mem64kbyte.py`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_memstdout.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_memstdout.py`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_note.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_note.py`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_on_off_switch.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_on_off_switch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" An On/Off Switch  component """
+"""An On/Off Switch  component"""
 
 import logging
 
 from .atoms import CallbackComponent, PortOutDelta
 
 
 class OnOffSwitch(CallbackComponent):
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_seven_segment.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_seven_segment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" Module with 7-segment LED component """
+"""Module with 7-segment LED component"""
+
 from .atoms import CallbackComponent, PortIn
 
 
 class SevenSegment(CallbackComponent):
     """7-segment LED component class"""
 
     PORTLIST = ["A", "B", "C", "D", "E", "F", "G", "dot"]
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_static_level.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_static_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" Module with the Static Logic components """
+"""Module with the Static Logic components"""
 
 from .atoms import Component, PortOutDelta
 
 
 class VDD(Component):
     """VDD / Logic1 component class"""
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_static_value.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_static_value.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" Module with the Static Leve component """
+"""Module with the Static Leve component"""
 
 from .atoms import Component, PortOutImmediate
 
 
 class StaticValue(Component):
     """Static value component class"""
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_yosys_atoms.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_yosys_atoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
 """
 Module with yosys atom component classes
 
 All components are implemented from the specification in:
 https://github.com/YosysHQ/yosys/blob/master/techlibs/common/simcells.v
 """
 
-# pylint: disable=too-many-arguments
-# pylint: disable=consider-using-in
-# pylint: disable=too-many-lines
-# pylint: disable=too-many-branches
-
 from .atoms import Component, DigsimException, PortIn, PortOutDelta, PortWire
 
 
 class YosysNotImplementedException(DigsimException):
     """Exception for not implemented components"""
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/_yosys_component.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/_yosys_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
 """
 Module with classes to create a yosys component
 from a yosys json netlist.
 """
 
-# pylint: disable=protected-access
-# pylint: disable=too-many-instance-attributes
-
 import json
 
 import digsim.circuit.components._yosys_atoms
 from digsim.synth import Synthesis
 from digsim.utils import YosysNetlist
 
 from .atoms import Component, DigsimException, MultiComponent, PortMultiBitWire
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/atoms/_component.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/atoms/_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
-""" This module contains the base classes for all component types """
-
-
-# pylint: disable=too-many-public-methods
+"""This module contains the base classes for all component types"""
 
 import abc
 import copy
 import importlib
 
 from ._digsim_exception import DigsimException
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/atoms/_port.py` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/atoms/_port.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
-""" This module contains the classes for all component ports """
-
-# pylint: disable=too-many-public-methods
+"""This module contains the classes for all component ports"""
 
 import abc
 
 from ._digsim_exception import DigsimException
 
 
 class PortConnectionError(DigsimException):
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/ic/74162.json` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/ic/74162.json`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/circuit/components/ic/7448.json` & `digsim-logic-simulator-0.4.0/src/digsim/circuit/components/ic/7448.json`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/synth/__main__.py` & `digsim-logic-simulator-0.4.0/src/digsim/synth/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" The main class module of the digsim.synth namespace """
+"""The main class module of the digsim.synth namespace"""
 
 import argparse
 import sys
 import time
 
 from . import Synthesis, SynthesisException
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/synth/_synthesis.py` & `digsim-logic-simulator-0.4.0/src/digsim/synth/_synthesis.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import json
 import shutil
 import sys
 
 import pexpect
 import pexpect.popen_spawn
+
 from digsim.circuit.components.atoms import DigsimException
 
 
 class SynthesisException(DigsimException):
     """Exception class for yosys synthesis"""
 
 
@@ -29,19 +30,26 @@
             # Unexpected EOF means ERROR
             errorline = "ERROR"
             for line in before_lines:
                 if "ERROR" in line:
                     errorline = line
                     break
             raise SynthesisException(errorline)
-        return before_lines
+
+        # Remove escape sequence in output
+        out_lines = []
+        for line in before_lines:
+            if line.startswith("\x1b"):
+                continue
+            out_lines.append(line)
+        return out_lines
 
     @classmethod
     def _pexpect_spawn_yosys(cls):
-        yosys_exe = shutil.which("yowasp-yosys")
+        yosys_exe = shutil.which("yosys") or shutil.which("yowasp-yosys")
 
         if yosys_exe is None:
             raise SynthesisException("Yosys executable not found")
 
         if sys.platform == "win32":
             return pexpect.popen_spawn.PopenSpawn(yosys_exe)
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim/utils/_yosys_netlist.py` & `digsim-logic-simulator-0.4.0/src/digsim/utils/_yosys_netlist.py`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/src/digsim_logic_simulator.egg-info/PKG-INFO` & `digsim-logic-simulator-0.4.0/src/digsim_logic_simulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digsim-logic-simulator
-Version: 0.3.0
+Version: 0.4.0
 Summary: Interactive Digital Logic Simulator
 Author-email: Fredrik Andersson <freand@gmail.com>
 Maintainer-email: Fredrik Andersson <freand@gmail.com>
 License: The Clear BSD License
         
         Copyright (c) 2023, Fredrik Andersson
         All rights reserved.
```

### Comparing `digsim-logic-simulator-0.3.0/src/digsim_logic_simulator.egg-info/SOURCES.txt` & `digsim-logic-simulator-0.4.0/src/digsim_logic_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digsim-logic-simulator-0.3.0/tests/test_gates.py` & `digsim-logic-simulator-0.4.0/tests/test_gates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" Pystest module to test functionality of gates """
+"""Pystest module to test functionality of gates"""
 
 import pytest
+
 from digsim.circuit import Circuit
 from digsim.circuit.components import AND, DFF, MUX, NAND, NOR, NOT, OR, SR, XOR
 
 
 @pytest.mark.parametrize(
     "in_a,in_b,out_y",
     [
```

### Comparing `digsim-logic-simulator-0.3.0/tests/test_yosys_aldff.py` & `digsim-logic-simulator-0.4.0/tests/test_yosys_aldff.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" Pystest module to test functionality of yosys asynchronous load dff """
+"""Pystest module to test functionality of yosys asynchronous load dff"""
 
+import pytest
 from utilities import _H, _L, inv
 
-import pytest
 from digsim.circuit import Circuit
 from digsim.circuit.components._yosys_atoms import (
     _ALDFF_NN_,
     _ALDFF_NP_,
     _ALDFF_PN_,
     _ALDFF_PP_,
     _ALDFFE_NNN_,
```

### Comparing `digsim-logic-simulator-0.3.0/tests/test_yosys_dff.py` & `digsim-logic-simulator-0.4.0/tests/test_yosys_dff.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" Pystest module to test functionality of yosys dff """
+"""Pystest module to test functionality of yosys dff"""
 
+import pytest
 from utilities import _H, _L, inv
 
-import pytest
 from digsim.circuit import Circuit
 from digsim.circuit.components._yosys_atoms import (
     _DFF_N_,
     _DFF_NN0_,
     _DFF_NN1_,
     _DFF_NP0_,
     _DFF_NP1_,
```

### Comparing `digsim-logic-simulator-0.3.0/tests/test_yosys_dlatch.py` & `digsim-logic-simulator-0.4.0/tests/test_yosys_dlatch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" Pystest module to test functionality of yosys latches """
+"""Pystest module to test functionality of yosys latches"""
 
+import pytest
 from utilities import _H, _L, inv
 
-import pytest
 from digsim.circuit import Circuit
 from digsim.circuit.components._yosys_atoms import (
     _DLATCH_N_,
     _DLATCH_NN0_,
     _DLATCH_NN1_,
     _DLATCH_NP0_,
     _DLATCH_NP1_,
```

### Comparing `digsim-logic-simulator-0.3.0/tests/test_yosys_gates.py` & `digsim-logic-simulator-0.4.0/tests/test_yosys_gates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" Pystest module to test functionality of yosys gates """
+"""Pystest module to test functionality of yosys gates"""
 
+import pytest
 from utilities import _H, _L, _X
 
-import pytest
 from digsim.circuit import Circuit
 from digsim.circuit.components._yosys_atoms import (
     _AND_,
     _ANDNOT_,
     _AOI3_,
     _AOI4_,
     _BUF_,
```

### Comparing `digsim-logic-simulator-0.3.0/tests/test_yosys_latch.py` & `digsim-logic-simulator-0.4.0/tests/test_yosys_latch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" Pystest module to test functionality of yosys latches """
+"""Pystest module to test functionality of yosys latches"""
 
+import pytest
 from utilities import _H, _L, inv
 
-import pytest
 from digsim.circuit import Circuit
 from digsim.circuit.components._yosys_atoms import (
     _DLATCH_N_,
     _DLATCH_NN0_,
     _DLATCH_NN1_,
     _DLATCH_NP0_,
     _DLATCH_NP1_,
```

### Comparing `digsim-logic-simulator-0.3.0/tests/test_yosys_netlist.py` & `digsim-logic-simulator-0.4.0/tests/test_yosys_netlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" Pystest module to test functionality of yosys component """
+"""Pystest module to test functionality of yosys component"""
 
 import pytest
+
 from digsim.circuit import Circuit
 from digsim.circuit.components import YosysComponent, YosysComponentException
 from digsim.utils import YosysNetlist
 
 
 netlist_dict_if_one = {
     "modules": {
```

### Comparing `digsim-logic-simulator-0.3.0/tests/test_yosys_sdff.py` & `digsim-logic-simulator-0.4.0/tests/test_yosys_sdff.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Fredrik Andersson, 2023
 # All rights reserved
 
-""" Pystest module to test functionality of yosys synrhonous reset dff """
+"""Pystest module to test functionality of yosys synrhonous reset dff"""
 
+import pytest
 from utilities import _H, _L, inv
 
-import pytest
 from digsim.circuit import Circuit
 from digsim.circuit.components._yosys_atoms import (
     _SDFF_NN0_,
     _SDFF_NN1_,
     _SDFF_NP0_,
     _SDFF_NP1_,
     _SDFF_PN0_,
```

### Comparing `digsim-logic-simulator-0.3.0/tests/test_yosys_sr.py` & `digsim-logic-simulator-0.4.0/tests/test_yosys_sr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
-""" Pystest module to test functionality of yosys sr """
-
-# pylint: disable=too-many-statements
+"""Pystest module to test functionality of yosys sr"""
 
+import pytest
 from utilities import _H, _L, inv
 
-import pytest
 from digsim.circuit import Circuit
 from digsim.circuit.components._yosys_atoms import (
     _DFFSR_NNN_,
     _DFFSR_NNP_,
     _DFFSR_NPN_,
     _DFFSR_NPP_,
     _DFFSR_PNN_,
```

### Comparing `digsim-logic-simulator-0.3.0/tests/test_yosys_synth.py` & `digsim-logic-simulator-0.4.0/tests/test_yosys_synth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-# Copyright (c) Fredrik Andersson, 2023
+# Copyright (c) Fredrik Andersson, 2023-2024
 # All rights reserved
 
-""" Pystest module to test functionality of yosys synthesis """
-
-# pylint: disable=redefined-outer-name
+"""Pystest module to test functionality of yosys synthesis"""
 
+import os
 from pathlib import Path
 
 import pytest
+
 from digsim.synth import Synthesis, SynthesisException
 
 
 @pytest.fixture
 def verilog_path():
     """Fixture: get path to verilog modules"""
-    return Path(__file__).parent.relative_to(Path.cwd()) / "verilog"
+    # Get the relative path to example folder
+    test_path = os.path.relpath(os.path.abspath(__file__), os.getcwd())
+    return Path(test_path).parent / "verilog"
 
 
 def test_yosys_list_modules_single_files(verilog_path):
     """test list modules in single file (with single module)"""
     modules = Synthesis.list_modules(str(verilog_path / "one_module.v"))
     assert len(modules) == 1
     assert "module_one" in modules
@@ -45,15 +47,15 @@
     assert "multi_module_three" in modules
 
 
 def test_yosys_list_module_with_error(verilog_path):
     """test list modules in single file (with multiple modules)"""
 
     with pytest.raises(SynthesisException):
-        Synthesis.list_modules([str(verilog_path / "moule_with_error.v")])
+        Synthesis.list_modules([str(verilog_path / "module_with_error.v")])
 
 
 def test_yosys_synth_single_file_single_module(verilog_path):
     """test synth single file (with single module)"""
     synthesis = Synthesis(str(verilog_path / "one_module.v"), "module_one")
     netlist_dict = synthesis.synth_to_dict()
     assert "modules" in netlist_dict
@@ -72,11 +74,11 @@
     assert "modules" in netlist_dict
     assert "multi_module_two" in netlist_dict["modules"]
 
 
 def test_yosys_synth_module_with_error(verilog_path):
     """test list modules in single file (with multiple modules)"""
 
-    synthesis = Synthesis(str(verilog_path / "moule_with_error.v"), "error_module")
+    synthesis = Synthesis(str(verilog_path / "module_with_error.v"), "error_module")
 
     with pytest.raises(SynthesisException):
         synthesis.synth_to_dict()
```

