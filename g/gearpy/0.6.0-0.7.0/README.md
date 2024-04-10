# Comparing `tmp/gearpy-0.6.0.tar.gz` & `tmp/gearpy-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gearpy-0.6.0.tar", last modified: Mon Mar 18 22:27:03 2024, max compression
+gzip compressed data, was "dist/gearpy-0.7.0.tar", last modified: Tue Apr  9 19:55:48 2024, max compression
```

## Comparing `gearpy-0.6.0.tar` & `gearpy-0.7.0.tar`

### file list

```diff
@@ -1,52 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:27:03.000000 gearpy-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-03-18 22:27:03.000000 gearpy-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-18 22:26:48.000000 gearpy-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:27:03.000000 gearpy-0.6.0/gearpy/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:27:03.000000 gearpy-0.6.0/gearpy/mechanical_objects/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/mechanical_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27002 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/mechanical_objects/dc_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/mechanical_objects/flywheel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:27:03.000000 gearpy-0.6.0/gearpy/mechanical_objects/gear_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/mechanical_objects/gear_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36614 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/mechanical_objects/helical_gear.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/mechanical_objects/mating_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    15230 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/mechanical_objects/mechanical_object_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    34832 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/mechanical_objects/spur_gear.py
--rw-r--r--   0 runner    (1001) docker     (127)    28254 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/mechanical_objects/worm_gear.py
--rw-r--r--   0 runner    (1001) docker     (127)    31306 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/mechanical_objects/worm_wheel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:27:03.000000 gearpy-0.6.0/gearpy/motor_control/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/motor_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/motor_control/motor_control_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/motor_control/pwm_control.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:27:03.000000 gearpy-0.6.0/gearpy/motor_control/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/motor_control/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/motor_control/rules/constant_pwm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/motor_control/rules/reach_angular_position.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/motor_control/rules/rules_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/motor_control/rules/start_limit_current.py
--rw-r--r--   0 runner    (1001) docker     (127)    12179 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/motor_control/rules/start_proportional_to_angular_position.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/motor_control/rules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    40521 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/powertrain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:27:03.000000 gearpy-0.6.0/gearpy/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/sensors/absolute_rotary_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/sensors/tachometer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/sensors/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12718 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:27:03.000000 gearpy-0.6.0/gearpy/units/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/units/unit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    82280 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/units/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:27:03.000000 gearpy-0.6.0/gearpy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16187 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/utils/animate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13434 2024-03-18 22:26:48.000000 gearpy-0.6.0/gearpy/utils/relations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:27:03.000000 gearpy-0.6.0/gearpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-03-18 22:27:03.000000 gearpy-0.6.0/gearpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-03-18 22:27:03.000000 gearpy-0.6.0/gearpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 22:27:03.000000 gearpy-0.6.0/gearpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-18 22:27:03.000000 gearpy-0.6.0/gearpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-18 22:27:03.000000 gearpy-0.6.0/gearpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 22:27:03.000000 gearpy-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-03-18 22:26:48.000000 gearpy-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-04-09 19:55:48.000000 gearpy-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-04-09 19:55:37.000000 gearpy-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/mechanical_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31110 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/dc_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/flywheel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/mechanical_objects/gear_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/gear_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44171 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/helical_gear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/mating_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17752 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/mechanical_object_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41309 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/spur_gear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34264 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/worm_gear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37362 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/worm_wheel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/motor_control/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/motor_control_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/pwm_control.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/motor_control/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/rules/constant_pwm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7711 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/rules/reach_angular_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/rules/rules_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/rules/start_limit_current.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/rules/start_proportional_to_angular_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/rules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55448 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/powertrain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/sensors/absolute_rotary_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/sensors/amperometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/sensors/sensor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/sensors/tachometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/sensors/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14582 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/units/unit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89909 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/units/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17524 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/utils/animate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20123 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/utils/relations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/utils/stop_condition/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/utils/stop_condition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/utils/stop_condition/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/utils/stop_condition/operator_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/utils/stop_condition/stop_condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-04-09 19:55:47.000000 gearpy-0.7.0/gearpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:55:47.000000 gearpy-0.7.0/gearpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-09 19:55:47.000000 gearpy-0.7.0/gearpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 19:55:47.000000 gearpy-0.7.0/gearpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:55:48.000000 gearpy-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-09 19:55:37.000000 gearpy-0.7.0/setup.py
```

### Comparing `gearpy-0.6.0/gearpy/mechanical_objects/dc_motor.py` & `gearpy-0.7.0/gearpy/mechanical_objects/dc_motor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,66 @@
 from gearpy.units import AngularPosition, AngularSpeed, AngularAcceleration, Current, InertiaMoment, Torque, UnitBase
 from .mechanical_object_base import RotatingObject, MotorBase
 from typing import Dict, List, Union, Optional
 
 
 class DCMotor(MotorBase):
-    r"""``gearpy.mechanical_objects.dc_motor.DCMotor`` object.
+    r""":py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>` object.
 
     Attributes
     ----------
-    :py:attr:`name` : str
+    :py:attr:`name` : :py:class:`str`
         Name of the DC motor.
-    :py:attr:`drives` : RotatingObject
-        Rotating object driven by DC motor, it can be a flywheel or a gear.
-    :py:attr:`angular_position` : AngularPosition
+    :py:attr:`drives` : :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
+        Rotating object driven by DC motor, it can be a
+        :py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` or a gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`).
+    :py:attr:`angular_position` : :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`
         Angular position of the DC motor.
-    :py:attr:`angular_speed` : AngularSpeed
+    :py:attr:`angular_speed` : :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`
         Angular speed of the DC motor.
-    :py:attr:`angular_acceleration` : AngularAcceleration
+    :py:attr:`angular_acceleration` : :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`
         Angular acceleration of the DC motor.
-    :py:attr:`no_load_speed` : AngularSpeed
+    :py:attr:`no_load_speed` : :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`
         No load angular speed of the DC motor.
-    :py:attr:`maximum_torque` : Torque
+    :py:attr:`maximum_torque` : :py:class:`Torque <gearpy.units.units.Torque>`
         Maximum torque developed by the DC motor.
-    :py:attr:`torque` : Torque
+    :py:attr:`torque` : :py:class:`Torque <gearpy.units.units.Torque>`
         Net torque applied on the DC motor.
-    :py:attr:`driving_torque` : Torque
+    :py:attr:`driving_torque` : :py:class:`Torque <gearpy.units.units.Torque>`
         Driving torque developed by the DC motor.
-    :py:attr:`load_torque` : Torque
+    :py:attr:`load_torque` : :py:class:`Torque <gearpy.units.units.Torque>`
         Load torque applied on the DC motor by its driven gear.
-    :py:attr:`inertia_moment` : InertiaMoment
+    :py:attr:`inertia_moment` : :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`
         Moment of inertia of the DC motor.
-    :py:attr:`no_load_electric_current` : Current
+    :py:attr:`no_load_electric_current` : :py:class:`Current <gearpy.units.units.Current>`
         No load electric current absorbed by the DC motor.
-    :py:attr:`maximum_electric_current` : Current
+    :py:attr:`maximum_electric_current` : :py:class:`Current <gearpy.units.units.Current>`
         Maximum electric current absorbed by the DC motor.
-    :py:attr:`electric_current_is_computable` : bool
-        Whether is possible to compute the electric current absorbed by the DC motor.
-    :py:attr:`electric_current` : Current
+    :py:attr:`electric_current_is_computable` : :py:class:`bool`
+        Whether is possible to compute the :py:attr:`electric_current` absorbed by the DC motor.
+    :py:attr:`electric_current` : :py:class:`Current <gearpy.units.units.Current>`
         Electric current absorbed by the DC motor.
-    :py:attr:`pwm` : float or int
+    :py:attr:`pwm` : :py:class:`float` or :py:class:`int`
         Pulse Width Modulation duty cycle of the supply voltage of the DC motor.
-    :py:attr:`time_variables` : dict
+    :py:attr:`time_variables` : :py:class:`dict`
         Time variables of the DC motor.
 
     Methods
     -------
     :py:meth:`compute_torque`
-        Computes the driving torque developed by the DC motor.
+        It computes the :py:attr:`driving_torque` developed by the DC motor.
     :py:meth:`compute_electric_current`
-        Computes the electric current absorbed by the DC motor.
+        It computes the :py:attr:`electric_current` absorbed by the DC motor.
     :py:meth:`update_time_variables`
-        Updates ``time_variables`` dictionary by appending the last value of each time variable to corresponding list.
+        It updates :py:attr:`time_variables` dictionary by appending the last value of each time variable to
+        corresponding list.
     """
 
     def __init__(self,
                  name: str,
                  inertia_moment: InertiaMoment,
                  no_load_speed: AngularSpeed,
                  maximum_torque: Torque,
@@ -101,322 +107,315 @@
 
         if self.electric_current_is_computable:
             self.__electric_current = None
             self.time_variables['electric current'] = []
 
     @property
     def name(self) -> str:
-        """Name of the DC motor. It must be a non-empty string. \n
+        """Name of the DC motor. It must be a non-empty :py:class:`str`. \n
         It must be a unique name, not shared by other elements in the powertrain elements. \n
         Once set at the DC motor instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        str
+        :py:class:`str`
             Name of the DC motor.
 
-        Raises
-        ------
-        TypeError
-            If ``name`` is not a string.
-        ValueError
-            If ``name`` is an empty string.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`name` is not a :py:class:`str`.
+           ``ValueError``
+               If :py:attr:`name` is an empty :py:class:`str`.
         """
         return super().name
 
     @property
     def drives(self) -> RotatingObject:
-        """Rotating object driven by DC motor, it can be a flywheel or a gear. It must be a ``RotatingObject``. \n
-        To set this property use :py:func:`gearpy.utils.relations.add_fixed_joint`.
+        """Rotating object driven by DC motor, it can be a
+        :py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` or a gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`). It must be an instance of
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`. \n
+        To set this property use :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
-        RotatingObject
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
             Rotating object driven by the DC motor.
 
-        Raises
-        ------
-        TypeError
-            If ``drives`` is not an instance of ``RotatingObject``.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`drives` is not an instance of
+               :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`.
         """
         return super().drives
 
     @drives.setter
     def drives(self, drives: RotatingObject):
         super(DCMotor, type(self)).drives.fset(self, drives)
 
     @property
     def angular_position(self) -> AngularPosition:
-        """Angular position of the DC motor. It must be an instance of ``AngularPosition``.
+        """Angular position of the DC motor. It must be an instance of
+        :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`.
 
         Returns
         -------
-        AngularPosition
+        :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`
             Angular position of the DC motor.
 
-        Raises
-        ------
-        TypeError
-            If ``angular_position`` is not an instance of ``AngularPosition``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularPosition`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`angular_position` is not an instance of
+               :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`.
         """
         return super().angular_position
 
     @angular_position.setter
     def angular_position(self, angular_position: AngularPosition):
         super(DCMotor, type(self)).angular_position.fset(self, angular_position)
 
     @property
     def angular_speed(self) -> AngularSpeed:
-        """Angular speed of the DC motor. It must be an instance of ``AngularSpeed``.
+        """Angular speed of the DC motor.
+        It must be an instance of :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`.
 
         Returns
         -------
-        AngularSpeed
+        :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`
             Angular speed of the DC motor.
 
-        Raises
-        ------
-        TypeError
-            If ``angular_speed`` is not an instance of ``AngularSpeed``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularSpeed`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`angular_speed` is not an instance of
+               :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`.
         """
         return super().angular_speed
 
     @angular_speed.setter
     def angular_speed(self, angular_speed: AngularSpeed):
         super(DCMotor, type(self)).angular_speed.fset(self, angular_speed)
 
     @property
     def angular_acceleration(self) -> AngularAcceleration:
-        """Angular acceleration of the DC motor. It must be an instance of ``AngularAcceleration``.
+        """Angular acceleration of the DC motor. It must be an instance of
+        :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`.
 
         Returns
         -------
-        AngularAcceleration
+        :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`
             Angular acceleration of the DC motor.
 
-        Raises
-        ------
-        TypeError
-            If ``angular_acceleration`` is not an instance of ``AngularAcceleration``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularAcceleration`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`angular_acceleration` is not an instance of
+               :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`.
         """
         return super().angular_acceleration
 
     @angular_acceleration.setter
     def angular_acceleration(self, angular_acceleration: AngularAcceleration):
         super(DCMotor, type(self)).angular_acceleration.fset(self, angular_acceleration)
 
     @property
     def no_load_speed(self) -> AngularSpeed:
-        """No load angular speed of the DC motor. It must be an instance of ``AngularSpeed``. Its value must be
-        positive. \n
+        """No load angular speed of the DC motor. It must be an instance of
+        :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`. Its value must be positive. \n
         It is the angular speed at which the DC motor rotates when no load is applied to its rotor. \n
         Once set at the DC motor instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        AngularSpeed
+        :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`
             No load angular speed of the DC motor.
 
-        Raises
-        ------
-        TypeError
-            If ``no_load_speed`` is not an instance of ``AngularSpeed``.
-        ValueError
-            If ``no_load_speed`` is negative or null.
+        .. admonition:: Raises
+           :class: warning
 
-        Se Also
-        -------
-        :py:class:`gearpy.units.units.AngularSpeed`
+           ``TypeError``
+               If :py:attr:`no_load_speed` is not an instance of
+               :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`.
+           ``ValueError``
+               If :py:attr:`no_load_speed` is negative or null.
         """
         return self.__no_load_speed
 
     @property
     def maximum_torque(self) -> Torque:
-        """Maximum torque developed by the DC motor. It must be an instance of ``Torque``. Its value must be
-        positive. \n
+        """Maximum torque developed by the DC motor. It must be an instance of
+        :py:class:`Torque <gearpy.units.units.Torque>`. Its value must be positive. \n
         It is the maximum torque the DC motor can develop when its rotor is kept still by the load. \n
         Once set at the DC motor instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Maximum torque developed by the DC motor.
 
-        Raises
-        ------
-        TypeError
-            If ``maximum_torque`` is not an instance of ``Torque``.
-        ValueError
-            If ``maximum_torque`` is negative or null.
+        .. admonition:: Raises
+           :class: warning
 
-        Se Also
-        -------
-        :py:class:`gearpy.units.units.Torque`
+           ``TypeError``
+               If :py:attr:`maximum_torque` is not an instance of :py:class:`Torque <gearpy.units.units.Torque>`.
+           ``ValueError``
+               If :py:attr:`maximum_torque` is negative or null.
         """
         return self.__maximum_torque
 
     @property
     def torque(self) -> Torque:
-        """Net torque applied on the DC motor. It must be an instance of ``Torque``. \n
-        It is computed as the difference between ``driving_torque`` and ``load_torque``.
+        """Net torque applied on the DC motor. It must be an instance of
+        :py:class:`Torque <gearpy.units.units.Torque>`. \n
+        It is computed as the difference between :py:attr:`driving_torque` and :py:attr:`load_torque`.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Net torque applied on the DC motor.
 
-        Raises
-        ------
-        TypeError
-            If ``torque`` is not an instance of ``Torque``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Torque`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`torque` is not an instance of :py:class:`Torque <gearpy.units.units.Torque>`.
         """
         return super().torque
 
     @torque.setter
     def torque(self, torque: Torque):
         super(DCMotor, type(self)).torque.fset(self, torque)
 
     @property
     def driving_torque(self) -> Torque:
-        """Driving torque developed by the DC motor. It must be an instance of ``Torque``.
+        """Driving torque developed by the DC motor. It must be an instance of
+        :py:class:`Torque <gearpy.units.units.Torque>`.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Driving torque developed by the DC motor.
 
-        Raises
-        ------
-        TypeError
-            If ``driving_torque`` is not an instance of ``Torque``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Torque`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`driving_torque` is not an instance of :py:class:`Torque <gearpy.units.units.Torque>`.
+
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`compute_torque`
         """
         return super().driving_torque
 
     @driving_torque.setter
     def driving_torque(self, driving_torque: Torque):
         super(DCMotor, type(self)).driving_torque.fset(self, driving_torque)
 
     @property
     def load_torque(self) -> Torque:
-        """Load torque applied on the DC motor by its driven gear. It must be an instance of ``Torque``.
+        """Load torque applied on the DC motor by its driven gear. It must be an instance of
+        :py:class:`Torque <gearpy.units.units.Torque>`.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Load torque applied on the DC motor by its driven gear.
 
-        Raises
-        ------
-        TypeError
-            If ``load_torque`` is not an instance of ``Torque``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Torque`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`load_torque` is not an instance of :py:class:`Torque <gearpy.units.units.Torque>`.
         """
         return super().load_torque
 
     @load_torque.setter
     def load_torque(self, load_torque: Torque):
         super(DCMotor, type(self)).load_torque.fset(self, load_torque)
 
     @property
     def inertia_moment(self) -> InertiaMoment:
-        """Moment of inertia of the DC motor's rotor. It must be an instance of ``InertiaMoment``. \n
+        """Moment of inertia of the DC motor's rotor. It must be an instance of
+        :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`. \n
         Once set at the DC motor instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        InertiaMoment
+        :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`
             Moment of inertia of the DC motor's rotor.
 
-        Raises
-        ------
-        TypeError
-            If ``inertia_moment`` is not an instance of ``InertiaMoment``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.InertiaMoment`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`inertia_moment` is not an instance of
+               :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`.
         """
         return super().inertia_moment
 
-    def compute_torque(self):
-        r"""Computes the driving torque developed by the DC motor. \n
-        The driving torque depends on the two constants ``no_load_speed`` and ``maximum_torque`` and the two variables
-        ``angular_speed`` and ``pwm`` of the DCMotor.
-        The computed torque has the same unit of ``maximum_torque``.
+    def compute_torque(self) -> None:
+        """It computes the :py:attr:`driving_torque` developed by the DC motor. \n
+        The driving torque depends on the two constants :py:attr:`no_load_speed` and :py:attr:`maximum_torque` and the
+        two variables :py:attr:`angular_speed` and :py:attr:`pwm` of the DCMotor. \n
+        The computed torque has the same unit of :py:attr:`maximum_torque`.
+        """\
+        r"""
+        .. admonition:: Notes
+           :class: tip
 
-        Notes
-        -----
-        The computation is based on the following relationship:
+           The computation is based on the following relationship:
 
-        .. math::
-            T \left( \dot{\theta} , T_{max}^D , \dot{\theta}_0^D \right) =
-            T_{max}^D \left( 1 - \frac{\dot{\theta}}{\dot{\theta}_0^D} \right)
+           .. math::
+               T \left( \dot{\theta} , T_{max}^D , \dot{\theta}_0^D \right) =
+               T_{max}^D \left( 1 - \frac{\dot{\theta}}{\dot{\theta}_0^D} \right)
 
-        where:
+           where:
 
-        - :math:`T` is the DC motor developed driving torque,
-        - :math:`\dot{\theta}` is the actual DC motor angular speed,
-        - :math:`T_{max}^D` is the DC motor maximum torque developed by the DC motor keeping into account ``pwm``,
-        - :math:`\dot{\theta}_0^D` is the DC motor no load angular speed keeping into account ``pwm``.
+           - :math:`T` is the DC motor developed driving torque :py:attr:`driving_torque`,
+           - :math:`\dot{\theta}` is the actual DC motor angular speed :py:attr:`angular_speed`,
+           - :math:`T_{max}^D` is the DC motor maximum torque developed by the DC motor **keeping into account**
+             :py:attr:`pwm`,
+           - :math:`\dot{\theta}_0^D` is the DC motor no load angular speed **keeping into account** :py:attr:`pwm`.
 
-        The maximum torque can be computed as:
+           The maximum torque can be computed as:
 
-        .. math::
-            T_{max}^D \left( D \right) = T_{max} \frac{D \, i_{max} - i_0}{i_{max} - i_0}
+           .. math::
+               T_{max}^D \left( D \right) = T_{max} \frac{D \, i_{max} - i_0}{i_{max} - i_0}
 
-        and the no load angular speed can be computed as:
+           and the no load angular speed can be computed as:
 
-        .. math::
-            \dot{\theta}_0^D \left( D \right) = D \, \dot{\theta}_0
+           .. math::
+               \dot{\theta}_0^D \left( D \right) = D \, \dot{\theta}_0
 
-        where:
+           where:
 
-        - :math:`D` is the DC motor supply voltage PWM duty cycle (``pwm``),
-        - :math:`T_{max}` is the DC motor maximum torque (``maximum_torque``),
-        - :math:`i_{max}` is the DC motor maximum electric current (``maximum_electric_current``),
-        - :math:`i_0` is the DC motor no load electric current (``no_load_electric_current``),
-        - :math:`\dot{\theta}_0` is the DC motor no load angular speed (``no_load_speed``).
+           - :math:`D` is the DC motor supply voltage PWM duty cycle (:py:attr:`pwm`),
+           - :math:`T_{max}` is the DC motor :py:attr:`maximum_torque`,
+           - :math:`i_{max}` is the DC motor :py:attr:`maximum_electric_current`,
+           - :math:`i_0` is the DC motor :py:attr:`no_load_electric_current`,
+           - :math:`\dot{\theta}_0` is the DC motor :py:attr:`no_load_speed`.
 
-        If the ``pwm`` is lower than a critical threshold, then the motor cannot develop any torque, so the
-        ``driving_torque`` will be null. The critical ``pwm`` value can be computed as:
+           If the :py:attr:`pwm` is lower than a critical threshold, then the motor cannot develop any torque, so the
+           :py:attr:`driving_torque` will be null. The critical :py:attr:`pwm` value can be computed as:
 
-        .. math::
-            D_{lim} = \frac{i_0}{i_{max}}
-
-        See Also
-        --------
-        :py:attr:`driving_torque`
-        :py:attr:`pwm`
+           .. math::
+               D_{lim} = \frac{i_0}{i_{max}}
         """
         if not self.electric_current_is_computable:
             self.driving_torque = Torque(value = (1 - self.angular_speed/self.no_load_speed)*self.maximum_torque.value,
                                          unit = self.maximum_torque.unit)
             return
 
         pwm_min = self.no_load_electric_current/self.maximum_electric_current \
@@ -436,119 +435,116 @@
             no_load_speed = self.pwm*self.no_load_speed
 
         self.driving_torque = Torque(value = (1 - self.angular_speed/no_load_speed)*maximum_torque.value,
                                      unit = self.maximum_torque.unit)
 
     @property
     def no_load_electric_current(self) -> Optional[Current]:
-        """No load electric current absorbed by the DC motor. It must be an instance of ``Current``. Its value must be
-        positive or null and lower than ``maximum_electric_current``. \n
+        """No load electric current absorbed by the DC motor. It must be an instance of
+        :py:class:`Current <gearpy.units.units.Current>`. Its value must be positive or null and lower than
+        :py:attr:`maximum_electric_current`. \n
         It is the electric current absorbed by the DC motor when no load is applied to its rotor. \n
         Once set at the DC motor instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        Current
+        :py:class:`Current <gearpy.units.units.Current>`
             No load electric current of the DC motor.
 
-        Raises
-        ------
-        TypeError
-            If ``no_load_electric_current`` is not an instance of ``Current``.
-        ValueError
-            - If ``no_load_electric_current`` is negative,
-            - if ``no_load_electric_current`` is higher than or equal to ``maximum_electric_current``.
+        .. admonition:: Raises
+           :class: warning
 
-        Se Also
-        -------
-        :py:class:`gearpy.units.units.Current`
+           ``TypeError``
+               If :py:attr:`no_load_electric_current` is not an instance of
+               :py:class:`Current <gearpy.units.units.Current>`.
+           ``ValueError``
+               - If :py:attr:`no_load_electric_current` is negative,
+               - if :py:attr:`no_load_electric_current` is higher than or equal to :py:attr:`maximum_electric_current`.
         """
         return self.__no_load_electric_current
 
     @property
     def maximum_electric_current(self) -> Optional[Current]:
-        """Maximum electric current absorbed by the DC motor. It must be an instance of ``Current``. Its value must be
-        positive and greater than ``no_load_electric_current``. \n
+        """Maximum electric current absorbed by the DC motor. It must be an instance of
+        :py:class:`Current <gearpy.units.units.Current>`. Its value must be positive and greater than
+        :py:attr:`no_load_electric_current`. \n
         It is the maximum electric current the DC motor can absorb when its rotor is kept still by the load. \n
         Once set at the DC motor instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        Current
+        :py:class:`Current <gearpy.units.units.Current>`
             Maximum electric current absorbed by the DC motor.
 
-        Raises
-        ------
-        TypeError
-            If ``maximum_electric_current`` is not an instance of ``Current``.
-        ValueError
-            - If ``maximum_electric_current`` is negative or null,
-            - if ``maximum_electric_current`` is lower than or equal to ``no_load_electric_current``.
+        .. admonition:: Raises
+           :class: warning
 
-        Se Also
-        -------
-        :py:class:`gearpy.units.units.Current`
+           ``TypeError``
+               If :py:attr:`maximum_electric_current` is not an instance of
+               :py:class:`Current <gearpy.units.units.Current>`.
+           ``ValueError``
+               - If :py:attr:`maximum_electric_current` is negative or null,
+               - if :py:attr:`maximum_electric_current` is lower than or equal to :py:attr:`no_load_electric_current`.
         """
         return self.__maximum_electric_current
 
-    def compute_electric_current(self):
-        r"""Computes the electric current absorbed by the DC motor. The absorbed electric current depends on the two
-        constants ``no_load_electric_current`` and ``maximum_electric_current`` and the two variables ``driving_torque``
-        and ``pwm`` of the DC motor.
-        The computed electric current has the same unit of ``maximum_electric_current``.
-
-        Notes
-        -----
-        The computation is based on the following relationship:
+    def compute_electric_current(self) -> None:
+        """It computes the :py:attr:`electric_current` absorbed by the DC motor. \n
+        The absorbed electric current depends on the two constants :py:attr:`no_load_electric_current` and 
+        :py:attr:`maximum_electric_current` and the two variables :py:attr:`driving_torque` and :py:attr:`pwm` of the DC 
+        motor. \n
+        The computed electric current has the same unit of :py:attr:`maximum_electric_current`.
+        """ \
+        r"""
+        .. admonition:: Notes
+           :class: tip
 
-        .. math::
-            i \left( T \right) = \left( i_{max}^D - i_0 \right) \frac{T}{T_{max}^D} + i_0
+           The computation is based on the following relationship:
 
-        where:
+           .. math::
+               i \left( T \right) = \left( i_{max}^D - i_0 \right) \frac{T}{T_{max}^D} + i_0
 
-        - :math:`i` is the electric current absorbed by the DC motor,
-        - :math:`T` is the DC motor developed driving torque,
-        - :math:`i_{max}^D` is the maximum electric current absorbed by the DC motor keeping into account ``pwm``,
-        - :math:`i_0` is the no load electric current absorbed by the DC motor (``no_load_electric_current``),
-        - :math:`T_{max}^D` is the DC motor maximum torque developed by the DC motor keeping into account ``pwm``.
+           where:
 
-        The maximum torque can be computed as:
+           - :math:`i` is the :py:attr:`electric_current` absorbed by the DC motor,
+           - :math:`T` is the DC motor developed :py:attr:`driving_torque`,
+           - :math:`i_{max}^D` is the maximum electric current absorbed by the DC motor **keeping into account**
+             :py:attr:`pwm`,
+           - :math:`i_0` is the :py:attr:`no_load_electric_current` absorbed by the DC motor,
+           - :math:`T_{max}^D` is the DC motor maximum torque developed by the DC motor **keeping into account**
+             :py:attr:`pwm`.
 
-        .. math::
-            T_{max}^D \left( D \right) = T_{max} \frac{D \, i_{max} - i_0}{i_{max} - i_0}
+           The maximum torque can be computed as:
 
-        and the maximum electric current can be computed as:
+           .. math::
+               T_{max}^D \left( D \right) = T_{max} \frac{D \, i_{max} - i_0}{i_{max} - i_0}
 
-        .. math::
-            i_{max}^D \left( D \right) = D \, i_{max}
+           and the maximum electric current can be computed as:
 
-        where:
+           .. math::
+               i_{max}^D \left( D \right) = D \, i_{max}
 
-        - :math:`D` is the DC motor supply voltage PWM duty cycle (``pwm``),
-        - :math:`T_{max}` is the DC motor maximum torque (``maximum_torque``),
-        - :math:`i_{max}` is the DC motor maximum electric current (``maximum_electric_current``),
-        - :math:`i_0` is the DC motor no load electric current (``no_load_electric_current``).
+           where:
 
-        If the ``pwm`` is lower than a critical threshold, then the motor cannot develop any torque, so the
-        ``electrical_current`` will depend only on ``pwm`` value. The critical ``pwm`` value can be computed as:
+           - :math:`D` is the DC motor supply voltage PWM duty cycle (:py:attr:`pwm`),
+           - :math:`T_{max}` is the DC motor :py:attr:`maximum_torque`,
+           - :math:`i_{max}` is the DC motor :py:attr:`maximum_electric_current`,
+           - :math:`i_0` is the DC motor :py:attr:`no_load_electric_current`.
 
-        .. math::
-            D_{lim} = \frac{i_0}{i_{max}}
+           If the :py:attr:`pwm` is lower than a critical threshold, then the motor cannot develop any torque, so the
+           :py:attr:`electric_current` will depend only on :py:attr:`pwm` value. The critical :py:attr:`pwm` value can 
+           be computed as:
 
-        and the relative electric current can be computed as:
+           .. math::
+               D_{lim} = \frac{i_0}{i_{max}}
 
-        .. math::
-            i_{lim} \left( D \right) = D \, i_{max}
+           and the relative electric current can be computed as:
 
-        See Also
-        --------
-        :py:attr:`no_load_electric_current`
-        :py:attr:`maximum_electric_current`
-        :py:attr:`electric_current`
-        :py:attr:`pwm`
+           .. math::
+               i_{lim} \left( D \right) = D \, i_{max}
         """
         maximum_electric_current = self.pwm*self.maximum_electric_current
         pwm_min = self.no_load_electric_current/self.maximum_electric_current
         if abs(self.pwm) <= pwm_min:
             if pwm_min == 0:
                 self.electric_current = Current(value = 0, unit = self.maximum_electric_current.unit)
             else:
@@ -569,49 +565,52 @@
         self.electric_current = Current(value = ((maximum_electric_current - no_load_electric_current)*
                                                    (self.driving_torque/maximum_torque) +
                                                    no_load_electric_current).value,
                                           unit = self.maximum_electric_current.unit)
 
     @property
     def electric_current_is_computable(self) -> bool:
-        """Whether is possible to compute the electric current absorbed by the DC motor. The electric current
-        computation depends on the value of ``no_load_electric_current`` and ``maximum_electric_current``, so if
-        these optional parameters have been set at DC motor instantiation, then it is possible to compute the absorbed
-        electric current and this property is ``True``, otherwise is ``False``.
+        """Whether is possible to compute the :py:attr:`electric_current` absorbed by the DC motor. \n
+        The electric current computation depends on the value of :py:attr:`no_load_electric_current` and
+        :py:attr:`maximum_electric_current`, so if these optional parameters have been set at DC motor instantiation,
+        then it is possible to compute the absorbed electric current and this property is ``True``, otherwise is
+        ``False``.
 
         Returns
         -------
-        bool
+        :py:class:`bool`
             Whether is possible to compute the electric current absorbed by the DC motor.
 
-        See Also
-        --------
-        :py:attr:`no_load_electric_current`
-        :py:attr:`maximum_electric_current`
-        :py:meth:`compute_electric_current`
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`compute_electric_current`
         """
         return (self.__no_load_electric_current is not None) and (self.__maximum_electric_current is not None)
 
     @property
     def electric_current(self) -> Optional[Current]:
-        """Electric current absorbed by the DC motor. It must be an instance of ``Current``.
+        """Electric current absorbed by the DC motor. It must be an instance of
+        :py:class:`Current <gearpy.units.units.Current>`.
 
         Returns
         -------
-        Current
+        :py:class:`Current <gearpy.units.units.Current>`
             Electric current absorbed by the DC motor.
 
-        Raises
-        ------
-        TypeError
-            If ``electric_current`` is not an instance of ``Current``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Current`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`electric_current` is not an instance of :py:class:`Current <gearpy.units.units.Current>`.
+
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`compute_electric_current`
         """
         return self.__electric_current
 
     @electric_current.setter
     def electric_current(self, electric_current: Current):
         if not isinstance(electric_current, Current):
             raise TypeError(f"Parameter 'electric_current' must be an instance of {Current.__name__!r}.")
@@ -619,86 +618,86 @@
         self.__electric_current = electric_current
 
     @property
     def time_variables(self) -> Dict[str, List[UnitBase]]:
         """Time variables of the DC motor. Each time variable is stored as a dictionary key-value pair. The available
         time variables are:
 
-        - ``angular position``,
-        - ``angular speed``,
-        - ``angular acceleration``,
-        - ``torque``,
-        - ``driving torque``,
-        - ``load torque``,
-        - ``electric current``,
-        - ``pwm``.
+        - :py:attr:`angular_position`: ``'angular position'``,
+        - :py:attr:`angular_speed`: ``'angular speed'``,
+        - :py:attr:`angular_acceleration`: ``'angular acceleration'``,
+        - :py:attr:`torque`: ``'torque'``,
+        - :py:attr:`driving_torque`: ``'driving torque'``,
+        - :py:attr:`load_torque`: ``'load torque'``,
+        - :py:attr:`electric_current`: ``'electric current'``,
+        - :py:attr:`pwm`: ``'pwm'``.
 
-        ``electric current`` is listed among time variables only if it is computable indeed, depending on which motor
-        parameters was set at DC motor instantiation. \n
+        ``'electric current'`` is listed among time variables only if it is computable indeed, depending on which motor
+        parameters was set at DC motor instantiation; see :py:attr:`electric_current_is_computable` for more details. \n
         Corresponding values of the dictionary are lists of the respective time variable values. \n
-        At each time iteration, the ``Solver`` appends every time variables' values to the relative list in the
-        dictionary.
+        At each time iteration, the :py:class:`Solver <gearpy.solver.Solver>` appends every time variables' values to
+        the relative list in the dictionary.
 
         Returns
         -------
-        dict
+        :py:class:`dict`
             Time variables of the DC motor.
 
-        See Also
-        --------
-        :py:meth:`update_time_variables`
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`update_time_variables`
         """
         return super().time_variables
 
     def update_time_variables(self) -> None:
-        """Updates ``time_variables`` dictionary by appending the last value of each time variable (key of the
+        """It updates :py:attr:`time_variables` dictionary by appending the last value of each time variable (key of the
         dictionary) to corresponding list (value of the dictionary).
-
-        See Also
-        --------
-        :py:attr:`time_variables`
         """
         super().update_time_variables()
         if self.electric_current_is_computable:
             self.time_variables['electric current'].append(self.electric_current)
         if 'pwm' not in self.time_variables.keys():
             self.time_variables['pwm'] = [self.pwm]
         else:
             self.time_variables['pwm'].append(self.pwm)
 
     @property
     def pwm(self) -> Union[float, int]:
         """Pulse Width Modulation duty cycle of the supply voltage of the DC motor. \n
-        It must be a float or an integer within ``-1`` and ``1``. \n
-        In general the duty cycle can be between ``0`` and ``1``, but ``pwm`` can be between ``-1`` and ``1``, in order
-        to take into account the voltage sign with respect to the direction of rotation:
+        It must be a :py:class:`float` or an :py:class:`int` within ``-1`` and ``1``. \n
+        In general the duty cycle can be between ``0`` and ``1``, but :py:attr:`pwm` can be between ``-1`` and ``1``, in
+        order to take into account the voltage sign with respect to the direction of rotation:
 
-        - if ``pwm`` is positive, then the supply voltage pushes the motor to rotate in the `positive` direction,
-        - if ``pwm`` is negative, then the supply voltage pushes the motor to rotate in the `negative` direction,
-        - if ``pwm`` is null, then the supply voltage is null to and the motor does not develop any driving torque.
+        - if :py:attr:`pwm` is positive, then the supply voltage pushes the motor to rotate in the `positive` direction,
+        - if :py:attr:`pwm` is negative, then the supply voltage pushes the motor to rotate in the `negative` direction,
+        - if :py:attr:`pwm` is null, then the supply voltage is null to and the motor does not develop any driving
+          torque.
 
-        The ``pwm`` value has an impact on the ``driving_torque`` developed and the ``electric_current`` absorbed by
-        the DC motor.
+        The :py:attr:`pwm` value has an impact on the :py:attr:`driving_torque` developed and the
+        :py:attr:`electric_current` absorbed by the DC motor.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Pulse Width Modulation duty cycle of the supply voltage of the DC motor.
 
-        Raises
-        ------
-        TypeError
-            If ``pwm`` is not a float or an integer.
-        ValueError
-            If ``pwm`` is not within ``-1`` and ``1``.
-
-        See Also
-        --------
-        :py:meth:`compute_torque`
-        :py:meth:`compute_electric_current`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`pwm` is not a :py:class:`float` or an :py:class:`int`.
+           ``ValueError``
+               If :py:attr:`pwm` is not within ``-1`` and ``1``.
+
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`compute_torque` \n
+           :py:meth:`compute_electric_current`
         """
         return self.__pwm
 
     @pwm.setter
     def pwm(self, pwm: Union[float, int]):
         if not isinstance(pwm, float) and not isinstance(pwm, int):
             raise TypeError("Parameter 'pwm' must be a float or an integer.")
```

### Comparing `gearpy-0.6.0/gearpy/mechanical_objects/flywheel.py` & `gearpy-0.7.0/gearpy/mechanical_objects/flywheel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,381 +1,380 @@
 from gearpy.units import AngularPosition, AngularSpeed, AngularAcceleration, InertiaMoment, Torque, UnitBase
 from .mechanical_object_base import RotatingObject
-from typing import Dict, List
+from typing import Dict, List, Union
 
 
 class Flywheel(RotatingObject):
-    r"""``gearpy.mechanical_objects.flywheel.Flywheel`` object.
+    r""":py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` object.
 
     Attributes
     ----------
-    :py:attr:`name` : str
+    :py:attr:`name` : :py:class:`str`
         Name of the flywheel.
-    :py:attr:`driven_by` : RotatingObject
-        Rotating object that drives the flywheel, for example a motor or a gear.
-    :py:attr:`drives` : RotatingObject
-        Rotating object driven by the flywheel, it can be a gear.
-    :py:attr:`master_gear_ratio` : float
+    :py:attr:`driven_by` : :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
+        Rotating object that drives the flywheel, for example a
+        :py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>` or a gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`).
+    :py:attr:`drives` : :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
+        Rotating object driven by the flywheel, it can be a gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`).
+    :py:attr:`master_gear_ratio` : :py:class:`float`
         Gear ratio of the fixed joint between the flywheel and its driving rotating object.
-    :py:attr:`master_gear_efficiency` : float or int
+    :py:attr:`master_gear_efficiency` : :py:class:`float` or :py:class:`int`
         Efficiency of the fixed joint between the flywheel and its driving rotating object.
-    :py:attr:`angular_position` : AngularPosition
+    :py:attr:`angular_position` : :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`
         Angular position of the flywheel.
-    :py:attr:`angular_speed` : AngularSpeed
+    :py:attr:`angular_speed` : :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`
         Angular speed of the flywheel.
-    :py:attr:`angular_acceleration` : AngularAcceleration
+    :py:attr:`angular_acceleration` : :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`
         Angular acceleration of the flywheel.
-    :py:attr:`torque` : Torque
+    :py:attr:`torque` : :py:class:`Torque <gearpy.units.units.Torque>`
         Net torque applied on the flywheel.
-    :py:attr:`driving_torque` : Torque
+    :py:attr:`driving_torque` : :py:class:`Torque <gearpy.units.units.Torque>`
         Driving torque applied on the flywheel by its driving rotating object.
-    :py:attr:`load_torque` : Torque
+    :py:attr:`load_torque` : :py:class:`Torque <gearpy.units.units.Torque>`
         Load torque applied on the flywheel by its driven rotating object.
-    :py:attr:`inertia_moment` : InertiaMoment
+    :py:attr:`inertia_moment` : :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`
         Moment of inertia of the flywheel.
-    :py:attr:`time_variables` : dict
+    :py:attr:`time_variables` : :py:class:`dict`
         Time variables of the flywheel.
 
     Methods
     -------
     :py:meth:`update_time_variables`
-        Updates ``time_variables`` dictionary by appending the last value of each time variable to corresponding list.
+        It updates :py:attr:`time_variables` dictionary by appending the last value of each time variable to
+        corresponding list.
     """
 
     def __init__(self, name: str, inertia_moment: InertiaMoment):
         super().__init__(name = name, inertia_moment = inertia_moment)
 
         self.__driven_by = None
         self.__drives = None
         self.__master_gear_ratio = None
         self.__master_gear_efficiency = 1
 
     @property
     def name(self) -> str:
-        """Name of the flywheel. It must be a non-empty string. \n
+        """Name of the flywheel. It must be a non-empty :py:class:`str`. \n
         It must be a unique name, not shared by other elements in the powertrain elements. \n
         Once set at the flywheel instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        str
+        :py:class:`str`
             Name of the flywheel.
 
-        Raises
-        ------
-        TypeError
-            If ``name`` is not a string.
-        ValueError
-            If ``name`` is an empty string.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`name` is not a :py:class:`str`.
+           ``ValueError``
+               If :py:attr:`name` is an empty :py:class:`str`.
         """
         return super().name
 
     @property
     def driven_by(self) -> RotatingObject:
-        """Rotating object that drives the flywheel, for example a motor or a gear. It must be a ``RotatingObject``. \n
-        To set this property use :py:func:`gearpy.utils.relations.add_fixed_joint`.
+        """Rotating object that drives the flywheel, for example a
+        :py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>` or a gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`). It must be a
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`. \n
+        To set this property use :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
-        RotatingObject
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
             Master rotating object that drives the flywheel.
 
-        Raises
-        ------
-        TypeError
-            If ``driven_by`` is not an instance of ``RotatingObject``.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`driven_by` is not an instance of
+               :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`.
         """
         return self.__driven_by
 
     @driven_by.setter
     def driven_by(self, driven_by: RotatingObject):
         if not isinstance(driven_by, RotatingObject):
             raise TypeError(f"Parameter 'driven_by' must be an instance of {RotatingObject.__name__!r}.")
 
         self.__driven_by = driven_by
 
     @property
     def drives(self) -> RotatingObject:
-        """Rotating object driven by the flywheel, it can be a gear. It must be a ``RotatingObject``. \n
-        To set this property use :py:func:`gearpy.utils.relations.add_fixed_joint`.
+        """Rotating object driven by the flywheel, it can be a gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`). It must be a
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`. \n
+        To set this property use :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
-        RotatingObject
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
             Rotating object driven by the flywheel.
 
-        Raises
-        ------
-        TypeError
-            If ``drives`` is not an instance of ``RotatingObject``.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`drives` is not an instance of
+               :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`.
         """
         return self.__drives
 
     @drives.setter
     def drives(self, drives: RotatingObject):
         if not isinstance(drives, RotatingObject):
             raise TypeError(f"Parameter 'drives' must be an instance of {RotatingObject.__name__!r}.")
 
         self.__drives = drives
 
     @property
     def angular_position(self) -> AngularPosition:
-        """Angular position of the flywheel. It must be an instance of ``AngularPosition``.
+        """Angular position of the flywheel. It must be an instance of
+        :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`.
 
         Returns
         -------
-        AngularPosition
+        :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`
             Angular position of the flywheel.
 
-        Raises
-        ------
-        TypeError
-            If ``angular_position`` is not an instance of ``AngularPosition``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularPosition`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`angular_position` is not an instance of
+               :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`.
         """
         return super().angular_position
 
     @angular_position.setter
     def angular_position(self, angular_position: AngularPosition):
         super(Flywheel, type(self)).angular_position.fset(self, angular_position)
 
     @property
     def angular_speed(self) -> AngularSpeed:
-        """Angular speed of the flywheel. It must be an instance of ``AngularSpeed``.
+        """Angular speed of the flywheel. It must be an instance of
+        :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`.
 
         Returns
         -------
-        AngularSpeed
+        :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`
             Angular speed of the flywheel.
 
-        Raises
-        ------
-        TypeError
-            If ``angular_speed`` is not an instance of ``AngularSpeed``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularSpeed`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`angular_speed` is not an instance of
+               :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`.
         """
         return super().angular_speed
 
     @angular_speed.setter
     def angular_speed(self, angular_speed: AngularSpeed):
         super(Flywheel, type(self)).angular_speed.fset(self, angular_speed)
 
     @property
     def angular_acceleration(self) -> AngularAcceleration:
-        """Angular acceleration of the flywheel. It must be an instance of ``AngularAcceleration``.
+        """Angular acceleration of the flywheel. It must be an instance of
+        :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`.
 
         Returns
         -------
-        AngularAcceleration
+        :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`
             Angular acceleration of the flywheel.
 
-        Raises
-        ------
-        TypeError
-            If ``angular_acceleration`` is not an instance of ``AngularAcceleration``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularAcceleration`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`angular_acceleration` is not an instance of
+               :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`.
         """
         return super().angular_acceleration
 
     @angular_acceleration.setter
     def angular_acceleration(self, angular_acceleration: AngularAcceleration):
         super(Flywheel, type(self)).angular_acceleration.fset(self, angular_acceleration)
 
     @property
     def torque(self) -> Torque:
-        """Net torque applied on the flywheel. It must be an instance of ``Torque``. \n
-        It is computed as the difference between ``driving_torque`` and ``load_torque``.
+        """Net torque applied on the flywheel. It must be an instance of
+        :py:class:`Torque <gearpy.units.units.Torque>`. \n
+        It is computed as the difference between :py:attr:`driving_torque` and :py:attr:`load_torque`.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Net torque applied on the flywheel.
 
-        Raises
-        ------
-        TypeError
-            If ``torque`` is not an instance of ``Torque``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Torque`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`torque` is not an instance of :py:class:`Torque <gearpy.units.units.Torque>`.
         """
         return super().torque
 
     @torque.setter
     def torque(self, torque: Torque):
         super(Flywheel, type(self)).torque.fset(self, torque)
 
     @property
     def driving_torque(self) -> Torque:
-        """Driving torque applied on the flywheel by its driving rotating object. It must be an instance of ``Torque``.
+        """Driving torque applied on the flywheel by its driving rotating object. It must be an instance of
+        :py:class:`Torque <gearpy.units.units.Torque>`.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Driving torque applied on the flywheel by its driving rotating object.
 
-        Raises
-        ------
-        TypeError
-            If ``driving_torque`` is not an instance of ``Torque``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Torque`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`driving_torque` is not an instance of :py:class:`Torque <gearpy.units.units.Torque>`.
         """
         return super().driving_torque
 
     @driving_torque.setter
     def driving_torque(self, driving_torque: Torque):
         super(Flywheel, type(self)).driving_torque.fset(self, driving_torque)
 
     @property
     def load_torque(self) -> Torque:
-        """Load torque applied on the flywheel by its driven rotating object. It must be an instance of ``Torque``.
+        """Load torque applied on the flywheel by its driven rotating object. It must be an instance of
+        :py:class:`Torque <gearpy.units.units.Torque>`.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Load torque applied on the flywheel by its driven rotating object.
 
-        Raises
-        ------
-        TypeError
-            If ``load_torque`` is not an instance of ``Torque``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Torque`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`load_torque` is not an instance of :py:class:`Torque <gearpy.units.units.Torque>`.
         """
         return super().load_torque
 
     @load_torque.setter
     def load_torque(self, load_torque: Torque):
         super(Flywheel, type(self)).load_torque.fset(self, load_torque)
 
     @property
     def master_gear_ratio(self) -> float:
         """Gear ratio of the fixed joint between the flywheel and its driving rotating object. It must be a positive a
         float. Since the relation between the flywheel and its neighbor elements in the powertrain elements is always a
-        fixed joint, the gear ratio will be set to ``1`` by :py:func:`gearpy.utils.relations.add_fixed_joint`. \n
-        To set this property use :py:func:`gearpy.utils.relations.add_fixed_joint`.
+        fixed joint, the gear ratio will be always set to ``1`` by
+        :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`. \n
+        To set this property use :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
-        float
+        :py:class:`float`
             Gear ratio of the fixed joint between the flywheel and its driving rotating object.
 
-        Raises
-        ------
-        TypeError
-            If ``master_gear_ratio`` is not a float.
-        ValueError
-            If ``master_gear_ratio`` is negative or null.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`master_gear_ratio` is not a :py:class:`float`.
+           ``ValueError``
+               If :py:attr:`master_gear_ratio` is negative or null.
         """
         return self.__master_gear_ratio
 
     @master_gear_ratio.setter
     def master_gear_ratio(self, master_gear_ratio: float):
         if not isinstance(master_gear_ratio, float):
             raise TypeError("Parameter 'master_gear_ratio' must be a float.")
 
         if master_gear_ratio <= 0:
             raise ValueError("Parameter 'master_gear_ratio' must be positive.")
 
         self.__master_gear_ratio = master_gear_ratio
 
     @property
-    def master_gear_efficiency(self) -> float:
+    def master_gear_efficiency(self) -> Union[float, int]:
         """Efficiency of the fixed joint between the flywheel and its driving rotating object. Since the relation
         between the flywheel and its neighbor elements in the powertrain elements is always a fixed joint, the
-        efficiency is always equal to ``1`` and cannot be overwritten.
+        efficiency is always equal to ``1`` and cannot be overwritten. \n
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Efficiency of the fixed joint between the flywheel and its driving rotating object.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
         """
         return self.__master_gear_efficiency
 
     @property
     def inertia_moment(self) -> InertiaMoment:
-        """Moment of inertia of the flywheel. It must be an instance of ``InertiaMoment``. \n
+        """Moment of inertia of the flywheel. It must be an instance of
+        :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`. \n
         Once set at the flywheel instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        InertiaMoment
+        :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`
             Moment of inertia of the flywheel.
 
-        Raises
-        ------
-        TypeError
-            If ``inertia_moment`` is not an instance of ``InertiaMoment``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.InertiaMoment`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`inertia_moment` is not an instance of
+               :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`.
         """
         return super().inertia_moment
 
     @property
     def time_variables(self) -> Dict[str, List[UnitBase]]:
         """Time variables of the flywheel. Each time variable is stored as a dictionary key-value pair. The available
         time variables are:
 
-        - ``angular_position``,
-        - ``angular_speed``,
-        - ``angular_acceleration``,
-        - ``torque``,
-        - ``driving_torque``,
-        - ``load_torque``.
+        - :py:attr:`angular_position`: ``'angular position'``,
+        - :py:attr:`angular_speed`: ``'angular speed'``,
+        - :py:attr:`angular_acceleration`: ``'angular acceleration'``,
+        - :py:attr:`torque`: ``'torque'``,
+        - :py:attr:`driving_torque`: ``'driving torque'``,
+        - :py:attr:`load_torque`: ``'load torque'``.
 
         Corresponding values of the dictionary are lists of the respective time variable values. \n
-        At each time iteration, the ``Solver`` appends every time variables' values to the relative list in the
-        dictionary.
+        At each time iteration, the :py:class:`Solver <gearpy.solver.Solver>` appends every time variables' values to
+        the relative list in the dictionary.
 
         Returns
         -------
-        dict
+        :py:class:`dict`
             Time variables of the flywheel.
 
-        See Also
-        --------
-        :py:meth:`update_time_variables`
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`update_time_variables`
         """
         return super().time_variables
 
     def update_time_variables(self) -> None:
-        """Updates ``time_variables`` dictionary by appending the last value of each time variable (key of the
+        """It updates :py:attr:`time_variables` dictionary by appending the last value of each time variable (key of the
         dictionary) to corresponding list (value of the dictionary).
-
-        See Also
-        --------
-        :py:attr:`time_variables`
         """
         super().update_time_variables()
```

### Comparing `gearpy-0.6.0/gearpy/mechanical_objects/helical_gear.py` & `gearpy-0.7.0/gearpy/mechanical_objects/spur_gear.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,816 +1,761 @@
 from gearpy.units import AngularPosition, AngularSpeed, AngularAcceleration, Angle, Force, InertiaMoment, Length, \
     Stress, Time, Torque, UnitBase
-from math import sin, cos, sqrt, atan, tan
-from .mechanical_object_base import RotatingObject, lewis_factor_function, Role
+from math import sqrt
+from .mechanical_object_base import RotatingObject, GearBase, lewis_factor_function, Role
 from .mating_roles import MatingMaster, MatingSlave
-from .spur_gear import SpurGear
 from typing import Callable, Dict, List, Union, Optional
 
 
-class HelicalGear(SpurGear):
-    r"""``gearpy.mechanical_objects.helical_gear.HelicalGear`` object.
+class SpurGear(GearBase):
+    r""":py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>` object.
 
     Attributes
     ----------
-    :py:attr:`name` : str
-        Name of the helical gear.
-    :py:attr:`n_teeth` : int
+    :py:attr:`name` : :py:class:`str`
+        Name of the spur gear.
+    :py:attr:`n_teeth` : :py:class:`int`
         Number of gear teeth.
-    :py:attr:`inertia_moment` : InertiaMoment
+    :py:attr:`inertia_moment` : :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`
         Moment of inertia of the gear.
-    :py:attr:`helix_angle` : Angle
-        Helix angle of the helical gear.
-    :py:attr:`module` : Length
+    :py:attr:`module` : :py:class:`Length <gearpy.units.units.Length>`
         Unit of the gear teeth size.
-    :py:attr:`reference_diameter` : Length
+    :py:attr:`reference_diameter` : :py:class:`Length <gearpy.units.units.Length>`
         Reference diameter of the gear.
-    :py:attr:`face_width` : Length
+    :py:attr:`face_width` : :py:class:`Length <gearpy.units.units.Length>`
         Face width of the gear.
-    :py:attr:`elastic_modulus` : Stress
+    :py:attr:`elastic_modulus` : :py:class:`Stress <gearpy.units.units.Stress>`
         Elastic modulus of the material of the gear.
-    :py:attr:`lewis_factor` : float
+    :py:attr:`lewis_factor` : :py:class:`float`
         Factor used to compute stresses on the gear tooth.
-    :py:attr:`driven_by` : RotatingObject
-        Rotating object that drives the gear, for example a motor, a flywheel or another gear.
-    :py:attr:`drives` : RotatingObject
-        Rotating object driven by the gear, it can be a flywheel or another gear.
-    :py:attr:`master_gear_ratio` : float
+    :py:attr:`driven_by` : :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
+        Rotating object that drives the gear, for example a
+        :py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>`, a
+        :py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` or another gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`).
+    :py:attr:`drives` : :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
+        Rotating object driven by the gear, it can be a
+        :py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` or another gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`).
+    :py:attr:`master_gear_ratio` : :py:class:`float`
         Gear ratio of the mating between the gear and its driving gear.
-    :py:attr:`master_gear_efficiency` : float or int
+    :py:attr:`master_gear_efficiency` : :py:class:`float` or :py:class:`int`
         Efficiency of the gear mating between the gear and its driving gear.
-    :py:attr:`mating_role`: Role
+    :py:attr:`mating_role`: :py:class:`Role <gearpy.mechanical_objects.mechanical_object_base.Role>`
         The role of the gear in the gear mating.
-    :py:attr:`angular_position` : AngularPosition
+    :py:attr:`angular_position` : :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`
         Angular position of the gear.
-    :py:attr:`angular_speed` : AngularSpeed
+    :py:attr:`angular_speed` : :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`
         Angular speed of the gear.
-    :py:attr:`angular_acceleration` : AngularAcceleration
+    :py:attr:`angular_acceleration` : :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`
         Angular acceleration of the gear.
-    :py:attr:`torque` : Torque
+    :py:attr:`torque` : :py:class:`Torque <gearpy.units.units.Torque>`
         Net torque applied on the gear.
-    :py:attr:`driving_torque` : Torque
+    :py:attr:`driving_torque` : :py:class:`Torque <gearpy.units.units.Torque>`
         Driving torque applied on the gear by its driving gear.
-    :py:attr:`load_torque` : Torque
+    :py:attr:`load_torque` : :py:class:`Torque <gearpy.units.units.Torque>`
         Load torque applied on the gear by its driven gear or an external load.
-    :py:attr:`tangential_force` : Force
+    :py:attr:`tangential_force` : :py:class:`Force <gearpy.units.units.Force>`
         Tangential force applied on the gear teeth by the mating gear.
-    :py:attr:`tangential_force_is_computable` : bool
-        Whether is possible to compute the tangential force on the gear teeth.
-    :py:attr:`bending_stress` : Stress
+    :py:attr:`tangential_force_is_computable` : :py:class:`bool`
+        Whether is possible to compute the :py:attr:`tangential_force` on the gear teeth.
+    :py:attr:`bending_stress` : :py:class:`Stress <gearpy.units.units.Stress>`
         Bending stress applied on the gear teeth by the mating gear.
-    :py:attr:`bending_stress_is_computable` : bool
-        Whether is possible to compute the bending stress on the gear teeth.
-    :py:attr:`contact_stress` : Stress
+    :py:attr:`bending_stress_is_computable` : :py:class:`bool`
+        Whether is possible to compute the :py:attr:`bending_stress` on the gear teeth.
+    :py:attr:`contact_stress` : :py:class:`Stress <gearpy.units.units.Stress>`
         The stress generated by the contact with mating gear teeth.
-    :py:attr:`contact_stress_is_computable` : bool
-        Whether is possible to compute the contact stress on the gear teeth.
-    :py:attr:`time_variables` : dict
+    :py:attr:`contact_stress_is_computable` : :py:class:`bool`
+        Whether is possible to compute the :py:attr:`contact_stress` on the gear teeth.
+    :py:attr:`time_variables` : :py:class:`dict`
         Time variables of the gear.
 
     Methods
     -------
     :py:meth:`compute_tangential_force`
-        Computes the tangential force applied on the gear teeth by the mating gear.
+        It computes the :py:attr:`tangential_force` applied on the gear teeth by the mating gear.
     :py:meth:`compute_bending_stress`
-        Computes the bending stress applied on the gear teeth by the mating gear.
+        It computes the :py:attr:`bending_stress` applied on the gear teeth by the mating gear.
     :py:meth:`compute_contact_stress`
-        Computes the contact stress generated by the contact with mating gear teeth.
+        It computes the :py:attr:`contact_stress` generated by the contact with mating gear teeth.
     :py:meth:`external_torque`
         Custom function to compute the external torque applied on the gear.
     :py:meth:`update_time_variables`
-        Updates ``time_variables`` dictionary by appending the last value of each time variable to corresponding list.
+        It updates :py:attr:`time_variables` dictionary by appending the last value of each time variable to
+        corresponding list.
     """
 
     def __init__(self,
                  name: str,
                  n_teeth: int,
                  inertia_moment: InertiaMoment,
-                 helix_angle: Angle,
                  module: Optional[Length] = None,
                  face_width: Optional[Length] = None,
                  elastic_modulus: Optional[Stress] = None):
         super().__init__(name = name,
                          n_teeth = n_teeth,
                          module = module,
                          face_width = face_width,
                          inertia_moment = inertia_moment,
                          elastic_modulus = elastic_modulus)
 
-        if not isinstance(helix_angle, Angle):
-            raise TypeError(f"Parameter 'helix_angle' must be an instance of {Angle.__name__!r}.")
-
-        if helix_angle >= Angle(90, 'deg'):
-            raise ValueError(f"Parameter 'helix_angle' cannot be greater than or equal to 90 degrees.")
-
-        self.__helix_angle = helix_angle
-
         if self.tangential_force_is_computable:
             self.time_variables['tangential force'] = []
 
             if self.bending_stress_is_computable:
                 self.time_variables['bending stress'] = []
-                PRESSURE_ANGLE = Angle(20, 'deg')
-                self.__TRANSVERSE_PRESSURE_ANGLE = Angle(value = atan(PRESSURE_ANGLE.tan()/helix_angle.cos()),
-                                                         unit = 'rad')
-                BASE_HELIX_ANGLE = Angle(value = atan(self.__TRANSVERSE_PRESSURE_ANGLE.cos()*self.__helix_angle.tan()),
-                                         unit = 'rad')
-                virtual_n_teeth = n_teeth/(BASE_HELIX_ANGLE.cos())**2/self.__helix_angle.cos()
-
-                self.__lewis_factor = lewis_factor_function(virtual_n_teeth).take(0)
+                self.__lewis_factor = lewis_factor_function(self.n_teeth).take(0)
 
                 if self.contact_stress_is_computable:
                     self.time_variables['contact stress'] = []
+                    self.__PRESSURE_ANGLE = Angle(20, 'deg')
 
     @property
     def name(self) -> str:
-        """Name of the helical gear. It must be a non-empty string. \n
+        """Name of the spur gear. It must be a non-empty :py:class:`str`. \n
         It must be a unique name, not shared by other elements in the powertrain elements. \n
-        Once set at the helical gear instantiation, it cannot be changed afterward.
+        Once set at the spur gear instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        str
-            Name of the helical gear.
+        :py:class:`str`
+            Name of the spur gear.
 
-        Raises
-        ------
-        TypeError
-            If ``name`` is not a string.
-        ValueError
-            If ``name`` is an empty string.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`name` is not a :py:class:`str`.
+           ``ValueError``
+               If :py:attr:`name` is an empty :py:class:`str`.
         """
         return super().name
 
     @property
     def n_teeth(self) -> int:
         """Number of gear teeth. It must be a positive integer. \n
-        Once set at the helical gear instantiation, it cannot be changed afterward.
+        Once set at the spur gear instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        int
+        :py:class:`int`
             Number of gear teeth.
 
-        Raises
-        ------
-        TypeError
-            If ``n_teeth`` is not an integer.
-        ValueError
-            If ``n_teeth`` is less than the minimum number of teeth, based on Lewis Factor table.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`n_teeth` is not an :py:class:`int`.
+           ``ValueError``
+               If :py:attr:`n_teeth` is less than the minimum number of teeth, based on Lewis Factor table.
         """
         return super().n_teeth
 
     @property
     def inertia_moment(self) -> InertiaMoment:
-        """Moment of inertia of the gear. It must be an instance of ``InertiaMoment``. \n
-        Once set at the helical gear instantiation, it cannot be changed afterward.
+        """Moment of inertia of the gear. It must be an instance of
+        :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`. \n
+        Once set at the spur gear instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        InertiaMoment
+        :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`
             Moment of inertia of the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``inertia_moment`` is not an instance of ``InertiaMoment``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.InertiaMoment`
-        """
-        return super().inertia_moment
-
-    @property
-    def helix_angle(self) -> Angle:
-        """Helix angle of the helical gear. It must be an instance of ``Angle`` lower than 90 degrees. \n
-        Once set at the helical gear instantiation, it cannot be changed afterward.
-
-        Returns
-        -------
-        Angle
-            The helix angle of the helical gear.
-
-        Raises
-        ------
-        TypeError
-            If ``helix_angle`` is not an instance of ``Angle``.
-        ValueError
-            If ``helix_angle`` is greater than or equal to 90 degrees.
+        .. admonition:: Raises
+           :class: warning
 
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Angle`
+           ``TypeError``
+               If :py:attr:`inertia_moment` is not an instance of
+               :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`.
         """
-        return self.__helix_angle
+        return super().inertia_moment
 
     @property
     def module(self) -> Optional[Length]:
-        """Unit of the gear teeth size. It must be an instance of ``Length``. \n
-        Once set at the helical gear instantiation, it cannot be changed afterward.
+        """Unit of the gear teeth size. It must be an instance of :py:class:`Length <gearpy.units.units.Length>`. \n
+        Once set at the spur gear instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        Length
+        :py:class:`Length <gearpy.units.units.Length>`
             Unit of the gear teeth size.
 
-        Raises
-        ------
-        TypeError
-            If ``module`` is not an instance of ``Length``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Length`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`module` is not an instance of :py:class:`Length <gearpy.units.units.Length>`.
         """
         return super().module
 
     @property
     def reference_diameter(self) -> Optional[Length]:
-        """Reference diameter of the gear. It must be an instance of ``Length``. \n
-        It is computed as the product of ``n_teeth`` times ``module`` at the helical gear instantiation and it cannot be
-        changed afterward.
+        """Reference diameter of the gear. It must be an instance of :py:class:`Length <gearpy.units.units.Length>`. \n
+        It is computed as the product of :py:attr:`n_teeth` times :py:attr:`module` at the spur gear instantiation and
+        it cannot be changed afterward.
 
         Returns
         -------
-        Length
+        :py:class:`Length <gearpy.units.units.Length>`
             Reference diameter of the gear.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Length`
         """
         return super().reference_diameter
 
     @property
     def face_width(self) -> Optional[Length]:
-        """Face width of the gear. It must be an instance of ``Length``.
+        """Face width of the gear. It must be an instance of :py:class:`Length <gearpy.units.units.Length>`.
 
         Returns
         -------
-        Length
+        :py:class:`Length <gearpy.units.units.Length>`
             Face width of the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``face_width`` is not an instance of ``Length``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Length`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`face_width` is not an instance of :py:class:`Length <gearpy.units.units.Length>`.
         """
         return super().face_width
 
     @property
     def elastic_modulus(self) -> Optional[Stress]:
-        """Elastic modulus of the material of the gear. It must be an instance of ``Stress``. It must be positive.
+        """Elastic modulus of the material of the gear. It must be an instance of
+        :py:class:`Stress <gearpy.units.units.Stress>`. It must be positive.
 
         Returns
         -------
-        Stress
+        :py:class:`Stress <gearpy.units.units.Stress>`
             Elastic modulus of the material of the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``elastic_modulus`` is not an instance of ``Stress``.
-        ValueError
-            If ``elastic_modulus`` value is negative or null.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Stress`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`elastic_modulus` is not an instance of :py:class:`Stress <gearpy.units.units.Stress>`.
+           ``ValueError``
+               If :py:attr:`elastic_modulus` value is negative or null.
         """
         return super().elastic_modulus
 
     @property
     def lewis_factor(self) -> Optional[float]:
         """Factor used to compute stresses on the gear tooth. \n
-        It is a tabular value that in general depends on the number of gear teeth, the pressure angle and the helix
-        angle. In this case, the considered pressure angle is always 20 degrees, so the Lewis factor depends only on the
-        number of gear teeth and the helix angle.
+        It is a tabular value that in general depends on the number of gear teeth and the pressure angle. In this
+        case, the considered pressure angle is always 20 degrees, so the Lewis factor depends only on the number of gear
+        teeth :py:attr:`n_teeth`.
 
         Returns
         -------
-        float
+        :py:class:`float`
             Factor used to compute stresses on the gear tooth.
         """
         return self.__lewis_factor
 
     @property
     def driven_by(self) -> RotatingObject:
-        """Rotating object that drives the gear, for example a motor, a flywheel or another gear. It must be a
-        ``RotatingObject``.
+        """Rotating object that drives the gear, for example a
+        :py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>`, a
+        :py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` or another gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`). It must be a
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`. \n
+        To set this property use :py:func:`add_gear_mating <gearpy.utils.relations.add_gear_mating>` or
+        :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
-        RotatingObject
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
             Master rotating object that drives the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``driven_by`` is not an instance of ``RotatingObject``.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_gear_mating`
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`driven_by` is not an instance of
+               :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`.
         """
         return super().driven_by
 
     @driven_by.setter
     def driven_by(self, driven_by: RotatingObject):
-        super(HelicalGear, type(self)).driven_by.fset(self, driven_by)
+        super(SpurGear, type(self)).driven_by.fset(self, driven_by)
 
     @property
     def drives(self) -> RotatingObject:
-        """Rotating object driven by the gear, it can be a flywheel or another gear. It must be a ``RotatingObject``.
+        """Rotating object driven by the gear, it can be a
+        :py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` or another gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`). It must be a
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`. \n
+        To set this property use :py:func:`add_gear_mating <gearpy.utils.relations.add_gear_mating>` or
+        :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
-        RotatingObject
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
             Rotating object driven by the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``drives`` is not an instance of ``RotatingObject``.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_gear_mating`
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`drives` is not an instance of
+               :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`.
         """
         return super().drives
 
     @drives.setter
     def drives(self, drives: RotatingObject):
-        super(HelicalGear, type(self)).drives.fset(self, drives)
+        super(SpurGear, type(self)).drives.fset(self, drives)
 
     @property
     def master_gear_ratio(self) -> float:
-        """Gear ratio of the mating between the gear and its driving gear. It must be a positive a float. \n
-        If the gear is fixed to another driving ``RotatingObject``, then the ratio is ``1``, otherwise it is defined as
-        the ratio between the gear number of teeth ``n_teeth`` and the same parameter of the master (driving) gear. \n
-        To set this property use :py:func:`gearpy.utils.relations.add_gear_mating` or
-        :py:func:`gearpy.utils.relations.add_fixed_joint`.
+        """Gear ratio of the mating between the gear and its driving gear. It must be a positive a :py:class:`float`. \n
+        If the gear is fixed to another driving
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`, then the ratio is
+        ``1``, otherwise it is defined as the ratio between the gear number of teeth :py:attr:`n_teeth` and the same
+        parameter of the master (driving) gear. \n
+        To set this property use :py:func:`add_gear_mating <gearpy.utils.relations.add_gear_mating>` or
+        :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
-        float
+        :py:class:`float`
             Gear ratio of the mating between the gear and its driving gear.
 
-        Raises
-        ------
-        TypeError
-            If ``master_gear_ratio`` is not a float.
-        ValueError
-            If ``master_gear_ratio`` is negative or null.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_gear_mating`
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`master_gear_ratio` is not a :py:class:`float`.
+           ``ValueError``
+               If :py:attr:`master_gear_ratio` is negative or null.
         """
         return super().master_gear_ratio
 
     @master_gear_ratio.setter
     def master_gear_ratio(self, master_gear_ratio: float):
-        super(HelicalGear, type(self)).master_gear_ratio.fset(self, master_gear_ratio)
+        super(SpurGear, type(self)).master_gear_ratio.fset(self, master_gear_ratio)
 
     @property
     def master_gear_efficiency(self) -> Union[float, int]:
-        """Efficiency of the gear mating between the gear and its driving gear. It must be a float or an integer within
-        ``0`` and ``1``. \n
-        To set this property use :py:func:`gearpy.utils.relations.add_gear_mating` or
-        :py:func:`gearpy.utils.relations.add_fixed_joint`.
+        """Efficiency of the gear mating between the gear and its driving gear. It must be a :py:class:`float` or an
+        :py:class:`int` within ``0`` and ``1``. \n
+        To set this property use :py:func:`add_gear_mating <gearpy.utils.relations.add_gear_mating>` or
+        :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Efficiency of the gear mating between the gear and its driving gear.
 
-        Raises
-        ------
-        TypeError
-            If ``master_gear_efficiency`` is not a float or an integer.
-        ValueError
-            If ``master_gear_efficiency`` is not within ``0`` and ``1``.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_gear_mating`
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`master_gear_efficiency` is not a :py:class:`float` or an :py:class:`int`.
+           ``ValueError``
+               If :py:attr:`master_gear_efficiency` is not within ``0`` and ``1``.
         """
         return super().master_gear_efficiency
 
     @master_gear_efficiency.setter
     def master_gear_efficiency(self, master_gear_efficiency: Union[float, int]):
-        super(HelicalGear, type(self)).master_gear_efficiency.fset(self, master_gear_efficiency)
+        super(SpurGear, type(self)).master_gear_efficiency.fset(self, master_gear_efficiency)
 
     @property
     def mating_role(self) -> Role:
-        """Role of the gear in the gear mating. To set this parameter use ``add_gear_mating``. \n
-        If the gear drives the mate one, then it is the "master" gear and its role is ``MatingMaster``, otherwise it is
-        the "slave" one and its role is ``MatingSlave``.
+        """Role of the gear in the gear mating. \n
+        If the gear drives the mate one, then it is the "master" gear and its role is
+        :py:class:`MatingMaster <gearpy.mechanical_objects.mating_roles.MatingMaster>`, otherwise it is the "slave" one
+        and its role is :py:class:`MatingSlave <gearpy.mechanical_objects.mating_roles.MatingSlave>`. \n
+        To set this parameter use :py:func:`add_gear_mating <gearpy.utils.relations.add_gear_mating>`.
 
         Returns
         -------
-        Role
+        :py:class:`Role <gearpy.mechanical_objects.mechanical_object_base.Role>`
             The role of the gear in the gear mating.
 
-        Raises
-        ------
-        ValueError
-            If ``mating_role`` is not a subclass of ``Role``.
+        .. admonition:: Raises
+           :class: warning
+
+           ``ValueError``
+               If :py:attr:`mating_role` is not a subclass of
+               :py:class:`Role <gearpy.mechanical_objects.mechanical_object_base.Role>`.
         """
         return super().mating_role
 
     @mating_role.setter
     def mating_role(self, mating_role: Role):
-        super(HelicalGear, type(self)).mating_role.fset(self, mating_role)
+        super(SpurGear, type(self)).mating_role.fset(self, mating_role)
 
     @property
     def angular_position(self) -> AngularPosition:
-        """Angular position of the gear. It must be an instance of ``AngularPosition``.
+        """Angular position of the gear. It must be an instance of
+        :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`.
 
         Returns
         -------
-        AngularPosition
+        :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`
             Angular position of the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``angular_position`` is not an instance of ``AngularPosition``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularPosition`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`angular_position` is not an instance of
+               :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`.
         """
         return super().angular_position
 
     @angular_position.setter
     def angular_position(self, angular_position: AngularPosition):
-        super(HelicalGear, type(self)).angular_position.fset(self, angular_position)
+        super(SpurGear, type(self)).angular_position.fset(self, angular_position)
 
     @property
     def angular_speed(self) -> AngularSpeed:
-        """Angular speed of the gear. It must be an instance of ``AngularSpeed``.
+        """Angular speed of the gear. It must be an instance of
+        :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`.
 
         Returns
         -------
-        AngularSpeed
+        :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`
             Angular speed of the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``angular_speed`` is not an instance of ``AngularSpeed``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularSpeed`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`angular_speed` is not an instance of
+               :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`.
         """
         return super().angular_speed
 
     @angular_speed.setter
     def angular_speed(self, angular_speed: AngularSpeed):
-        super(HelicalGear, type(self)).angular_speed.fset(self, angular_speed)
+        super(SpurGear, type(self)).angular_speed.fset(self, angular_speed)
 
     @property
     def angular_acceleration(self) -> AngularAcceleration:
-        """Angular acceleration of the gear. It must be an instance of ``AngularAcceleration``.
+        """Angular acceleration of the gear. It must be an instance of
+        :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`.
 
         Returns
         -------
-        AngularAcceleration
+        :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`
             Angular acceleration of the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``angular_acceleration`` is not an instance of ``AngularAcceleration``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularAcceleration`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`angular_acceleration` is not an instance of
+               :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`.
         """
         return super().angular_acceleration
 
     @angular_acceleration.setter
     def angular_acceleration(self, angular_acceleration: AngularAcceleration):
-        super(HelicalGear, type(self)).angular_acceleration.fset(self, angular_acceleration)
+        super(SpurGear, type(self)).angular_acceleration.fset(self, angular_acceleration)
 
     @property
     def torque(self) -> Torque:
-        """Net torque applied on the gear. It must be an instance of ``Torque``. \n
-        It is computed as the difference between ``driving_torque`` and ``load_torque``.
+        """Net torque applied on the gear. It must be an instance of :py:class:`Torque <gearpy.units.units.Torque>`. \n
+        It is computed as the difference between :py:attr:`driving_torque` and :py:attr:`load_torque`.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Net torque applied on the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``torque`` is not an instance of ``Torque``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Torque`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`torque` is not an instance of :py:class:`Torque <gearpy.units.units.Torque>`.
         """
         return super().torque
 
     @torque.setter
     def torque(self, torque: Torque):
-        super(HelicalGear, type(self)).torque.fset(self, torque)
+        super(SpurGear, type(self)).torque.fset(self, torque)
 
     @property
     def driving_torque(self) -> Torque:
-        """Driving torque applied on the gear by its driving gear. It must be an instance of ``Torque``.
+        """Driving torque applied on the gear by its driving gear. It must be an instance of
+        :py:class:`Torque <gearpy.units.units.Torque>`.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Driving torque applied on the gear by its driving gear.
 
-        Raises
-        ------
-        TypeError
-            If ``driving_torque`` is not an instance of ``Torque``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Torque`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`driving_torque` is not an instance of :py:class:`Torque <gearpy.units.units.Torque>`.
         """
         return super().driving_torque
 
     @driving_torque.setter
     def driving_torque(self, driving_torque: Torque):
-        super(HelicalGear, type(self)).driving_torque.fset(self, driving_torque)
+        super(SpurGear, type(self)).driving_torque.fset(self, driving_torque)
 
     @property
     def load_torque(self) -> Torque:
-        """Load torque applied on the gear by its driven gear or an external load. It must be an instance of ``Torque``.
+        """Load torque applied on the gear by its driven gear or an external load. It must be an instance of
+        :py:class:`Torque <gearpy.units.units.Torque>`.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Load torque applied on the gear by its driven gear or an external load.
 
-        Raises
-        ------
-        TypeError
-            If ``load_torque`` is not an instance of ``Torque``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Torque`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`load_torque` is not an instance of :py:class:`Torque <gearpy.units.units.Torque>`.
         """
         return super().load_torque
 
     @load_torque.setter
     def load_torque(self, load_torque: Torque):
-        super(HelicalGear, type(self)).load_torque.fset(self, load_torque)
+        super(SpurGear, type(self)).load_torque.fset(self, load_torque)
 
     @property
     def tangential_force(self) -> Force:
-        """Tangential force applied on the gear teeth by the mating gear. It must be an instance of ``Force``.
+        """Tangential force applied on the gear teeth by the mating gear. It must be an instance of
+        :py:class:`Force <gearpy.units.units.Force>`.
 
         Returns
         -------
-        Force
+        :py:class:`Force <gearpy.units.units.Force>`
             Tangential force applied on the gear teeth by the mating gear.
 
-        Raises
-        ------
-        TypeError
-            If ``tangential_force`` is not an instance of ``Force``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Force`
-        :py:meth:`compute_tangential_force`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`tangential_force` is not an instance of :py:class:`Force <gearpy.units.units.Force>`.
+
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`compute_tangential_force`
         """
         return super().tangential_force
 
     @tangential_force.setter
     def tangential_force(self, tangential_force: Force):
-        super(HelicalGear, type(self)).tangential_force.fset(self, tangential_force)
+        super(SpurGear, type(self)).tangential_force.fset(self, tangential_force)
 
-    def compute_tangential_force(self):
-        """Computes the tangential force applied on the gear teeth by the mating gear. \n
+    def compute_tangential_force(self) -> None:
+        """It computes the :py:attr:`tangential_force` applied on the gear teeth by the mating gear. \n
         Considering a gear mating:
 
-        - if the gear is the master one, then it takes into account the ``load_torque`` for the computation,
-        - if the gear is the slave one, then it take into account the ``driving_torque`` for the computation.
+        - if the gear is the master one, then it takes into account the :py:attr:`load_torque` for the computation,
+        - if the gear is the slave one, then it take into account the :py:attr:`driving_torque` for the computation.
 
         The tangential force is computed dividing the just described reference torque by the reference radius (half of
-        the reference diameter).
+        the :py:attr:`reference_diameter`).
 
-        Raises
-        ------
-        ValueError
-            If a gear mating between two gears has not been set.
-
-        See Also
-        --------
-        :py:attr:`tangential_force`
+        .. admonition:: Raises
+           :class: warning
+
+           ``ValueError``
+               If a gear mating between two gears has not been set.
         """
         if self.mating_role == MatingMaster:
             self.tangential_force = abs(self.load_torque)/(self.reference_diameter/2)
         elif self.mating_role == MatingSlave:
             self.tangential_force = abs(self.driving_torque)/(self.reference_diameter/2)
         else:
             raise ValueError("Gear mating not defined. "
                              "Use 'gearpy.utils.add_gear_mating' to set up a mating between two gears.")
 
     @property
     def tangential_force_is_computable(self) -> bool:
-        """Whether is possible to compute the tangential force on the gear teeth. The tangential force computation
-        depends on the value of ``module``, so if this optional parameter has been set at helical gear instantiation,
-        then it is possible to compute the tangential force and this property is ``True``, otherwise is ``False``.
+        """Whether is possible to compute the :py:attr:`tangential_force` on the gear teeth. \n
+        The tangential force computation depends on the value of :py:attr:`module`, so if this optional parameter has
+        been set at spur gear instantiation, then it is possible to compute the tangential force and this property is
+        ``True``, otherwise is ``False``.
 
         Returns
         -------
-        bool
+        :py:class:`bool`
             Whether is possible to compute the tangential force on the gear teeth.
 
-        See Also
-        --------
-        :py:attr:`module`
-        :py:attr:`tangential_force`
-        :py:meth:`compute_tangential_force`
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`compute_tangential_force`
         """
         return super().tangential_force_is_computable
 
     @property
     def bending_stress(self) -> Stress:
-        """Bending stress applied on the gear teeth by the mating gear. It must be an instance of ``Stress``.
+        """Bending stress applied on the gear teeth by the mating gear. It must be an instance of
+        :py:class:`Stress <gearpy.units.units.Stress>`.
 
         Returns
         -------
-        Stress
+        :py:class:`Stress <gearpy.units.units.Stress>`
             Bending stress applied on the gear teeth by the mating gear.
 
-        Raises
-        ------
-        TypeError
-            If ``bending_stress`` is not an instance of ``Stress``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Stress`
-        :py:meth:`compute_bending_stress`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`bending_stress` is not an instance of :py:class:`Stress <gearpy.units.units.Stress>`.
+
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`compute_bending_stress`
         """
         return super().bending_stress
 
     @bending_stress.setter
     def bending_stress(self, bending_stress: Stress):
-        super(HelicalGear, type(self)).bending_stress.fset(self, bending_stress)
+        super(SpurGear, type(self)).bending_stress.fset(self, bending_stress)
 
-    def compute_bending_stress(self):
-        r"""Computes the bending stress applied on the gear teeth by the mating gear.
+    def compute_bending_stress(self) -> None:
+        r"""It computes the :py:attr:`bending_stress` applied on the gear teeth by the mating gear.
 
-        Notes
-        -----
-        The bending stress computation is based on the following assumptions:
-
-        - the tooth is stressed by the overall force acting on the tip of the tooth itself,
-        - the most unfavorable situation is considered in the calculation, as if there is only one pair of teeth in
-          contact within the contact segment,
-        - the component of the overall force that determines the bending on the tooth is the only one considered and,
-          for simplicity, is taken as having a value equal to the tangential force on the reference diameter,
-        - the radial component of the overall force that causes a compressive stress on the tooth is neglected.
-
-        The bending stress is computed with the following formula:
-
-        .. math::
-            \sigma_b = \frac{F_t}{m \, b \, Y_{LW}}
-
-        where:
-
-        - :math:`F_t` is the tangential force applied on the tooth,
-        - :math:`m` is the gear module (``module``),
-        - :math:`b` is the gear tooth face width (``face_width``),
-        - :math:`Y_{LW}` is the gear Lewis factor (``lewis_factor``).
-
-        See Also
-        --------
-        :py:attr:`bending_stress`
-        :py:attr:`tangential_force`
-        :py:attr:`module`
-        :py:attr:`face_width`
-        :py:attr:`lewis_factor`
+        .. admonition:: Notes
+           :class: tip
+
+           The bending stress computation is based on the following assumptions:
+
+           - the tooth is stressed by the overall force acting on the tip of the tooth itself,
+           - the most unfavorable situation is considered in the calculation, as if there is only one pair of teeth in
+             contact within the contact segment,
+           - the component of the overall force that determines the bending on the tooth is the only one considered and,
+             for simplicity, is taken as having a value equal to the tangential force on the reference diameter,
+           - the radial component of the overall force that causes a compressive stress on the tooth is neglected.
+
+           The bending stress is computed with the following formula:
+
+           .. math::
+               \sigma_b = \frac{F_t}{m \, b \, Y_{LW}}
+
+           where:
+
+           - :math:`F_t` is the :py:attr:`tangential_force` applied on the tooth,
+           - :math:`m` is the gear :py:attr:`module`,
+           - :math:`b` is the gear tooth :py:attr:`face_width`,
+           - :math:`Y_{LW}` is the gear :py:attr:`lewis_factor`.
         """
         self.bending_stress = self.tangential_force/(self.module*self.face_width)/self.lewis_factor
 
     @property
     def bending_stress_is_computable(self) -> bool:
-        """Whether is possible to compute the bending stress on the gear teeth. The bending stress computation depends
-        on the value of ``module`` and ``face_width``, so if these optional parameters have been set at helical gear
-        instantiation, then it is possible to compute the bending stress and this property is ``True``, otherwise is
-        ``False``.
+        """Whether is possible to compute the :py:attr:`bending_stress` on the gear teeth. \n
+        The bending stress computation depends on the value of :py:attr:`module` and :py:attr:`face_width`, so if these
+        optional parameters have been set at spur gear instantiation, then it is possible to compute the bending stress
+        and this property is ``True``, otherwise is ``False``.
 
         Returns
         -------
-        bool
+        :py:class:`bool`
             Whether is possible to compute the bending stress on the gear teeth.
 
-        See Also
-        --------
-        :py:attr:`module`
-        :py:attr:`face_width`
-        :py:attr:`bending_stress`
-        :py:meth:`compute_bending_stress`
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`compute_bending_stress`
         """
         return super().bending_stress_is_computable
 
     @property
     def contact_stress(self) -> Stress:
-        """Stress generated by the contact with mating gear teeth. It must be an instance of ``Stress``.
+        """Stress generated by the contact with mating gear teeth. It must be an instance of
+        :py:class:`Stress <gearpy.units.units.Stress>`.
 
         Returns
         -------
-        Stress
+        :py:class:`Stress <gearpy.units.units.Stress>`
             The stress generated by the contact with mating gear teeth.
 
-        Raises
-        ------
-        TypeError
-            If ``contact_stress`` is not an instance of ``Stress``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Stress`
-        :py:meth:`compute_contact_stress`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`contact_stress` is not an instance of :py:class:`Stress <gearpy.units.units.Stress>`.
+
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`compute_contact_stress`
         """
         return super().contact_stress
 
     @contact_stress.setter
     def contact_stress(self, contact_stress: Stress):
-        super(HelicalGear, type(self)).contact_stress.fset(self, contact_stress)
+        super(SpurGear, type(self)).contact_stress.fset(self, contact_stress)
+
+    def compute_contact_stress(self) -> None:
+        r"""It computes the :py:attr:`contact_stress` generated by the contact with mating gear teeth.
 
-    def compute_contact_stress(self):
-        r"""Computes the contact stress generated by the contact with mating gear teeth.
+        .. admonition:: Raises
+           :class: warning
 
-        Raises
-        ------
-        ValueError
-            - If a gear mating between two gears has not been set,
-            - if gear role is ``MatingMaster`` and its slave gear misses ``module`` parameter,
-            - if gear role is ``MatingMaster`` and its slave gear misses ``elastic_modulus`` parameter,
-            - if gear role is ``MatingSlave`` and its master gear misses ``module`` parameter,
-            - if gear role is ``MatingSlave`` and its master gear misses ``elastic_modulus`` parameter.
-
-        Notes
-        -----
-        The contact stress computation is based on the following assumptions:
-
-        - perfect elasticity of the materials the two mating gear,
-        - absence of friction forces in the contact point,
-        - small size of the contact surface compared to the size of the bodies between which contact occurs.
-
-        The contact stress is computed with the following formula:
-
-        .. math::
-            \sigma_c = 0.262922 \, \sqrt{\frac{4 \, F_t \, \cos \beta}{b \, \cos \alpha_t \, \sin \alpha_t}
-            \left( \frac{1}{D_1} + \frac{1}{D_2} \right) \, \frac{E_1 \, E_2}{E_1 + E_2}}
-
-        where:
-
-        - :math:`F_t` is the tangential force applied on the tooth,
-        - :math:`\beta` is the gear helix angle (``helix_angle``),
-        - :math:`b` is the gear face width (``face_width``),
-        - :math:`\alpha_t` is the transverse pressure angle of the gear,
-        - :math:`D_1` is the gear reference diameter (``reference_diameter``),
-        - :math:`D_2` is the mating gear reference diameter,
-        - :math:`E_1` is the gear elastic modulus (``elastic_modulus``),
-        - :math:`E_2` is the mating gear elastic modulus.
-
-        The transverse pressure angle of the gear can be computed with the formula:
-
-        .. math::
-            \alpha_t = \tan^{-1} \frac{\tan \alpha}{\cos \beta}
-
-        where :math:`\alpha` is the pressure angle of the gear, always equal to 20 degrees.
-
-        See Also
-        --------
-        :py:attr:`contact_stress`
-        :py:attr:`tangential_force`
-        :py:attr:`elastic_modulus`
-        :py:attr:`face_width`
-        :py:attr:`reference_diameter`
-        :py:attr:`helix_angle`
+           ``ValueError``
+               - If a gear mating between two gears has not been set,
+               - if :py:attr:`mating_role` is 
+                 :py:class:`MatingMaster <gearpy.mechanical_objects.mating_roles.MatingMaster>` and its slave gear 
+                 misses :py:attr:`module` parameter,
+               - if :py:attr:`mating_role` is 
+                 :py:class:`MatingMaster <gearpy.mechanical_objects.mating_roles.MatingMaster>` and its slave gear 
+                 misses :py:attr:`elastic_modulus` parameter,
+               - if :py:attr:`mating_role` is 
+                 :py:class:`MatingSlave <gearpy.mechanical_objects.mating_roles.MatingSlave>` and its master gear misses 
+                 :py:attr:`module` parameter,
+               - if :py:attr:`mating_role` is 
+                 :py:class:`MatingSlave <gearpy.mechanical_objects.mating_roles.MatingSlave>` and its master gear misses 
+                 :py:attr:`elastic_modulus` parameter.
+
+        .. admonition:: Notes
+           :class: tip
+
+           The contact stress computation is based on the following assumptions:
+
+           - perfect elasticity of the materials the two mating gear,
+           - absence of friction forces in the contact point,
+           - small size of the contact surface compared to the size of the bodies between which contact occurs.
+
+           The contact stress is computed with the following formula:
+
+           .. math::
+               \sigma_c = 0.262922 \, \sqrt{\frac{4 \, F_t}{b \, \cos \alpha \, \sin \alpha}
+               \left( \frac{1}{D_1} + \frac{1}{D_2} \right) \, \frac{E_1 \, E_2}{E_1 + E_2}}
+
+           where:
+
+           - :math:`F_t` is the :py:attr:`tangential_force` tangential force applied on the tooth,
+           - :math:`b` is the gear :py:attr:`face_width`,
+           - :math:`\alpha` is the pressure angle of the gear, always equal to 20 degrees,
+           - :math:`D_1` is the gear :py:attr:`reference_diameter`,
+           - :math:`D_2` is the mating gear :py:attr:`reference_diameter`,
+           - :math:`E_1` is the gear :py:attr:`elastic_modulus`,
+           - :math:`E_2` is the mating gear :py:attr:`elastic_modulus`.
         """
         if self.mating_role == MatingMaster:
             if self.drives.module is not None:
                 mate_reference_diameter = self.drives.reference_diameter
             else:
                 raise ValueError(f"Impossible to compute contact stress for {self.__class__.__name__} {self.name!r} "
                                  f"because its mating {self.__class__.__name__} {self.drives.name!r} misses "
@@ -836,138 +781,144 @@
                                  f"'elastic_modulus' parameter.")
         else:
             raise ValueError("Gear mating not defined. "
                              "Use 'gearpy.utils.add_gear_mating' to set up a mating between two gears.")
 
         equivalent_elastic_modulus = 2*self.elastic_modulus* \
                                      (mate_elastic_modulus/(self.elastic_modulus + mate_elastic_modulus))
-        inverse_curvature_sum = self.__TRANSVERSE_PRESSURE_ANGLE.sin()/2*self.reference_diameter* \
+        inverse_curvature_sum = self.__PRESSURE_ANGLE.sin()/2*self.reference_diameter* \
                                 (mate_reference_diameter/(self.reference_diameter + mate_reference_diameter))
-        contact_pressure = self.tangential_force/self.__TRANSVERSE_PRESSURE_ANGLE.cos()/ \
-                                                 (self.face_width/self.__helix_angle.cos()*inverse_curvature_sum)
+        contact_pressure = self.tangential_force/self.__PRESSURE_ANGLE.cos()/(self.face_width*inverse_curvature_sum)
 
         self.contact_stress = Stress(value = 0.262922*sqrt(equivalent_elastic_modulus.to('Pa').value*
                                                            contact_pressure.to('Pa').value),
                                      unit = 'Pa')
 
     @property
     def contact_stress_is_computable(self) -> bool:
-        """Whether is possible to compute the contact stress force on the gear teeth. The contact stress computation
-        depends on the value of ``module``, ``face_width`` and ``elastic_modulus``, so if these optional parameters have
-        been set at helical gear instantiation, then it is possible to compute the contact stress and this property is
-        ``True``, otherwise is ``False``.
+        """Whether is possible to compute the :py:attr:`contact_stress` force on the gear teeth. \n
+        The contact stress computation depends on the value of :py:attr:`module`, :py:attr:`face_width` and
+        :py:attr:`elastic_modulus`, so if these optional parameters have been set at spur gear instantiation, then it is
+        possible to compute the contact stress and this property is ``True``, otherwise is ``False``.
 
         Returns
         -------
-        bool
+        :py:class:`bool`
             Whether is possible to compute the contact stress on the gear teeth.
 
-        See Also
-        --------
-        :py:attr:`module`
-        :py:attr:`face_width`
-        :py:attr:`elastic_modulus`
-        :py:attr:`contact_stress`
-        :py:meth:`compute_contact_stress`
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`compute_contact_stress`
         """
         return super().contact_stress_is_computable
 
     @property
     def external_torque(self) -> Callable[[AngularPosition, AngularSpeed, Time], Torque]:
         """Custom function to compute the external torque applied on the gear. It must be a function with parameters
-        ``angular_position``, ``angular_speed`` and ``time``. The function must return an instance of ``Torque``.
+        ``angular_position``, ``angular_speed`` and ``time``. The function must return an instance of
+        :py:class:`Torque <gearpy.units.units.Torque>`.
 
         Returns
         -------
-        Callable
+        :py:obj:`Callable <typing.Callable>`
             The function to compute the external torque applied on the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``external_torque`` is not callable.
-        KeyError
-            If ``external_torque`` misses parameters ``angular_position``, ``angular_speed`` or ``time``.
-
-        Examples
-        --------
-        Constant torque, not dependent on ``angular_position``, ``angular_speed`` or ``time``.
-
-        >>> from gearpy.mechanical_objects import HelicalGear
-        >>> from gearpy.units import InertiaMoment, Torque
-        >>> gear = HelicalGear(name = 'gear', n_teeth = 10, inertia_moment = InertiaMoment(1, 'kgm^2'))
-        >>> gear.external_torque = lambda angular_position, angular_speed, time: Torque(5, 'Nm')
-
-        Torque dependent on ``angular_position`` and ``time``. \n
-        In this case the gear gets a periodic load, dependent on time, and an extra load dependent on its angular
-        position. The dependence by angular position may be used to model cases where cams are involved.
-
-        >>> import numpy as np
-        >>> from gearpy.units import AngularPosition, AngularSpeed, Time
-        >>> def custom_external_torque(angular_position: AngularPosition,
-        ...                            angular_speed: AngularSpeed,
-        ...                            time: Time):
-        ...     return Torque(value = angular_position.sin() +
-        ...                           np.cos(time.to('sec').value),
-        ...                   unit = 'Nm')
-        >>> gear.external_torque = custom_external_torque
-
-        Torque dependent on ``angular_position``, ``angular_speed`` and ``time``. \n
-        With respect ot the previous case, the gear gets an extra load dependent on its angular speed. The dependence by
-        angular speed may be used to model cases where air friction is not negligible.
-
-        >>> def complex_external_torque(angular_position: AngularPosition,
-        ...                             angular_speed: AngularSpeed,
-        ...                             time: Time):
-        ...     return Torque(value = angular_position.sin() +
-        ...                           0.001*(angular_speed.to('rad/s').value)**2 +
-        ...                           np.cos(time.to('sec').value),
-        ...                   unit = 'Nm')
-        >>> gear.external_torque = complex_external_torque
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:meth:`external_torque` is not callable.
+           ``KeyError``
+               If :py:meth:`external_torque` misses parameters ``angular_position``, ``angular_speed`` or ``time``.
+
+        .. admonition:: Examples
+           :class: important
+
+           Constant torque, not dependent on ``angular_position``, ``angular_speed`` or ``time``.
+
+           >>> from gearpy.mechanical_objects import SpurGear
+           >>> from gearpy.units import InertiaMoment, Torque
+           >>> gear = SpurGear(name = 'gear', n_teeth = 10, inertia_moment = InertiaMoment(1, 'kgm^2'))
+           >>> gear.external_torque = lambda angular_position, angular_speed, time: Torque(5, 'Nm')
+
+           Torque dependent on ``angular_position`` and ``time``. \n
+           In this case the gear gets a periodic load, dependent on time, and an extra load dependent on its angular
+           position. The dependence by angular position may be used to model cases where cams are involved.
+
+           >>> import numpy as np
+           >>> from gearpy.units import AngularPosition, AngularSpeed, Time
+           >>> def custom_external_torque(angular_position: AngularPosition,
+           ...                            angular_speed: AngularSpeed,
+           ...                            time: Time):
+           ...     return Torque(value = angular_position.sin() +
+           ...                           np.cos(time.to('sec').value),
+           ...                   unit = 'Nm')
+           >>> gear.external_torque = custom_external_torque
+
+           Torque dependent on ``angular_position``, ``angular_speed`` and ``time``. \n
+           With respect ot the previous case, the gear gets an extra load dependent on its angular speed. The dependence
+           by angular speed may be used to model cases where air friction is not negligible.
+
+           >>> def complex_external_torque(angular_position: AngularPosition,
+           ...                             angular_speed: AngularSpeed,
+           ...                             time: Time):
+           ...     return Torque(value = angular_position.sin() +
+           ...                           0.001*(angular_speed.to('rad/s').value)**2 +
+           ...                           np.cos(time.to('sec').value),
+           ...                   unit = 'Nm')
+           >>> gear.external_torque = complex_external_torque
         """
         return super().external_torque
 
     @external_torque.setter
     def external_torque(self, external_torque: Callable[[AngularPosition, AngularSpeed, Time], Torque]):
-        super(HelicalGear, type(self)).external_torque.fset(self, external_torque)
+        super(SpurGear, type(self)).external_torque.fset(self, external_torque)
 
     @property
     def time_variables(self) -> Dict[str, List[UnitBase]]:
         """Time variables of the gear. Each time variable is stored as a dictionary key-value pair. The available time
         variables are:
 
-        - ``angular position``,
-        - ``angular speed``,
-        - ``angular acceleration``,
-        - ``torque``,
-        - ``driving torque``,
-        - ``load torque``,
-        - ``tangential force``,
-        - ``bending stress``,
-        - ``contact stress``.
-
-        ``tangential force``, ``bending stress`` and ``contact stress`` are listed among time variables only if they are
-        computable indeed, depending on which gear parameters are set at gear instantiation. \n
+        - :py:attr:`angular_position`: ``'angular position'``,
+        - :py:attr:`angular_speed`: ``'angular speed'``,
+        - :py:attr:`angular_acceleration`: ``'angular acceleration'``,
+        - :py:attr:`torque`: ``'torque'``,
+        - :py:attr:`driving_torque`: ``'driving torque'``,
+        - :py:attr:`load_torque`: ``'load torque'``,
+        - :py:attr:`tangential_force`: ``'tangential force'``,
+        - :py:attr:`bending_stress`: ``'bending stress'``,
+        - :py:attr:`contact_stress`: ``'contact stress'``.
+
+        ``'tangential force'``, ``'bending stress'`` and ``'contact stress'`` are listed among time variables only if
+        they are computable indeed, depending on which gear parameters are set at gear instantiation; see
+        :py:attr:`tangential_force_is_computable`, :py:attr:`bending_stress_is_computable` and
+        :py:attr:`contact_stress_is_computable` for more details. \n
         Corresponding values of the dictionary are lists of the respective time variable values. \n
-        At each time iteration, the ``Solver`` appends every time variables' values to the relative list in the
-        dictionary.
+        At each time iteration, the :py:class:`Solver <gearpy.solver.Solver>` appends every time variables' values to
+        the relative list in the dictionary.
 
         Returns
         -------
-        dict
+        :py:class:`dict`
             Time variables of the gear.
 
-        See Also
-        --------
-        :py:meth:`update_time_variables`
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`update_time_variables`
         """
         return super().time_variables
 
     def update_time_variables(self) -> None:
-        """Updates ``time_variables`` dictionary by appending the last value of each time variable (key of the
+        """It updates :py:attr:`time_variables` dictionary by appending the last value of each time variable (key of the
         dictionary) to corresponding list (value of the dictionary).
-
-        See Also
-        --------
-        :py:attr:`time_variables`
         """
         super().update_time_variables()
+        if self.tangential_force_is_computable:
+            self.time_variables['tangential force'].append(self.tangential_force)
+
+            if self.bending_stress_is_computable:
+                self.time_variables['bending stress'].append(self.bending_stress)
+
+                if self.contact_stress_is_computable:
+                    self.time_variables['contact stress'].append(self.contact_stress)
```

### Comparing `gearpy-0.6.0/gearpy/mechanical_objects/mechanical_object_base.py` & `gearpy-0.7.0/gearpy/mechanical_objects/mechanical_object_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,38 +7,51 @@
 import pandas as pd
 from scipy.interpolate import interp1d
 from typing import Callable, Dict, List, Union
 
 
 LEWIS_FACTOR_DATA_FILE = (imp_resources.files(gear_data) / 'lewis_factor_table.csv')
 LEWIS_FACTOR_DATA = pd.read_csv(LEWIS_FACTOR_DATA_FILE)
-MINIMUM_TEETH_NUMBER = LEWIS_FACTOR_DATA.loc[LEWIS_FACTOR_DATA.index[0], 'number of teeth']
-lewis_factor_function = interp1d(x = LEWIS_FACTOR_DATA['number of teeth'],
-                                 y = LEWIS_FACTOR_DATA['Lewis factor'],
-                                 fill_value = (LEWIS_FACTOR_DATA.loc[LEWIS_FACTOR_DATA.index[0], 'Lewis factor'],
-                                               LEWIS_FACTOR_DATA.loc[LEWIS_FACTOR_DATA.index[-1], 'Lewis factor']),
+MINIMUM_TEETH_NUMBER = LEWIS_FACTOR_DATA.loc[LEWIS_FACTOR_DATA.index[0], 'Number of teeth']
+lewis_factor_function = interp1d(x = LEWIS_FACTOR_DATA['Number of teeth'],
+                                 y = LEWIS_FACTOR_DATA['Lewis Factor'],
+                                 fill_value = (LEWIS_FACTOR_DATA.loc[LEWIS_FACTOR_DATA.index[0], 'Lewis Factor'],
+                                               LEWIS_FACTOR_DATA.loc[LEWIS_FACTOR_DATA.index[-1], 'Lewis Factor']),
                                  bounds_error = False)
 
 WORM_GEAR_AND_WHEEL_DATA_FILE = (imp_resources.files(gear_data) / 'worm_gear_and_wheel_data.csv')
 WORM_GEAR_AND_WHEEL_DATA = pd.read_csv(WORM_GEAR_AND_WHEEL_DATA_FILE)
 WORM_GEAR_AND_WHEEL_AVAILABLE_PRESSURE_ANGLES = [Angle(value, 'deg')
-                                                 for value in WORM_GEAR_AND_WHEEL_DATA['pressure angle']]
+                                                 for value in WORM_GEAR_AND_WHEEL_DATA['Pressure Angle']]
 
 
 def worm_gear_and_wheel_maximum_helix_angle_function(pressure_angle: Angle) -> Angle:
-    return Angle(value = float(WORM_GEAR_AND_WHEEL_DATA.set_index('pressure angle').
-                               loc[pressure_angle.to('deg').value, 'maximum helix angle']),
+    return Angle(value = float(WORM_GEAR_AND_WHEEL_DATA.set_index('Pressure Angle').
+                               loc[pressure_angle.to('deg').value, 'Maximum Helix Angle']),
                                 unit = 'deg')
 
 
 def worm_wheel_lewis_factor_function(pressure_angle: Angle) -> Angle:
-    return WORM_GEAR_AND_WHEEL_DATA.set_index('pressure angle').loc[pressure_angle.to('deg').value, 'Lewis factor']
+    return WORM_GEAR_AND_WHEEL_DATA.set_index('Pressure Angle').loc[pressure_angle.to('deg').value, 'Lewis Factor']
 
 
 class MechanicalObject(ABC):
+    """:py:class:`MechanicalObject <gearpy.mechanical_objects.mechanical_object_base.MechanicalObject>` object. \n
+    Abstract base class for creating mechanical objects.
+
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>` \n
+       :py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` \n
+       :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>` \n
+       :py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>` \n
+       :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>` \n
+       :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`
+    """
 
     @abstractmethod
     def __init__(self, name: str):
         if not isinstance(name, str):
             raise TypeError("Parameter 'name' must be a string.")
 
         if name == '':
@@ -49,14 +62,27 @@
     @property
     @abstractmethod
     def name(self) -> str:
         return self.__name
 
 
 class RotatingObject(MechanicalObject):
+    """:py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>` object. \n
+    Abstract base class for creating rotating objects.
+
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>` \n
+       :py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` \n
+       :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>` \n
+       :py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>` \n
+       :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>` \n
+       :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`
+    """
 
     @abstractmethod
     def __init__(self, name: str, inertia_moment: InertiaMoment):
         super().__init__(name = name)
 
         if not isinstance(inertia_moment, InertiaMoment):
             raise TypeError(f"Parameter 'inertia_moment' must be an instance of {InertiaMoment.__name__!r}.")
@@ -171,14 +197,22 @@
         self.__time_variables['angular acceleration'].append(self.__angular_acceleration)
         self.__time_variables['torque'].append(self.__torque)
         self.__time_variables['driving torque'].append(self.__driving_torque)
         self.__time_variables['load torque'].append(self.__load_torque)
 
 
 class MotorBase(RotatingObject):
+    """:py:class:`MotorBase <gearpy.mechanical_objects.mechanical_object_base.MotorBase>` object. \n
+    Abstract base class for creating motor objects.
+
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>`
+    """
 
     @abstractmethod
     def __init__(self, name: str, inertia_moment: InertiaMoment):
         super().__init__(name = name, inertia_moment = inertia_moment)
         self.__drives = None
 
     @property
@@ -195,14 +229,24 @@
         self.__drives = drives
 
     @abstractmethod
     def compute_torque(self, **kargs): ...
 
 
 class GearBase(RotatingObject):
+    """:py:class:`GearBase <gearpy.mechanical_objects.mechanical_object_base.GearBase>` object. \n
+    Abstract base class for creating gear objects.
+
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>` \n
+       :py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>` \n
+       :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`
+    """
 
     @abstractmethod
     def __init__(self,
                  name: str,
                  n_teeth: int,
                  module: Length,
                  face_width: Length,
@@ -225,15 +269,15 @@
                 raise TypeError(f"Parameter 'face_width' must be an instance of {Length.__name__!r}.")
 
         if elastic_modulus is not None:
             if not isinstance(elastic_modulus, Stress):
                 raise TypeError(f"Parameter 'elastic_modulus' must be an instance of {Stress.__name__!r}.")
 
             if elastic_modulus.value <= 0:
-                raise ValueError(f"Parameter 'elastic_modulus' must be positive.")
+                raise ValueError("Parameter 'elastic_modulus' must be positive.")
 
         self.__n_teeth = n_teeth
         self.__driven_by = None
         self.__drives = None
         self.__master_gear_ratio = None
         self.__master_gear_efficiency = 1
         self.__mating_role = None
@@ -433,8 +477,17 @@
         for parameter in ['angular_position', 'angular_speed', 'time']:
             if parameter not in sig.parameters.keys():
                 raise KeyError(f"Function 'external_torque' misses parameter {parameter!r}.")
 
         self.__external_torque = external_torque
 
 
-class Role(ABC): ...
+class Role(ABC):
+    """:py:class:`Role <gearpy.mechanical_objects.mechanical_object_base.Role>` object. \n
+    Abstract base class for creating role objects.
+
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:class:`MatingMaster <gearpy.mechanical_objects.mating_roles.MatingMaster>` \n
+       :py:class:`MatingSlave <gearpy.mechanical_objects.mating_roles.MatingSlave>`
+    """
```

### Comparing `gearpy-0.6.0/gearpy/mechanical_objects/spur_gear.py` & `gearpy-0.7.0/gearpy/mechanical_objects/worm_wheel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,930 +1,844 @@
 from gearpy.units import AngularPosition, AngularSpeed, AngularAcceleration, Angle, Force, InertiaMoment, Length, \
-    Stress, Time, Torque, UnitBase
-from math import sin, cos, sqrt
-from .mechanical_object_base import RotatingObject, GearBase, lewis_factor_function, Role
+                         Stress, Time, Torque, UnitBase
+from math import pi
+from .mechanical_object_base import RotatingObject, Role, WORM_GEAR_AND_WHEEL_AVAILABLE_PRESSURE_ANGLES, \
+                                    worm_gear_and_wheel_maximum_helix_angle_function, worm_wheel_lewis_factor_function
 from .mating_roles import MatingMaster, MatingSlave
+from .helical_gear import HelicalGear
 from typing import Callable, Dict, List, Union, Optional
 
 
-class SpurGear(GearBase):
-    r"""``gearpy.mechanical_objects.spur_gear.SpurGear`` object.
+class WormWheel(HelicalGear):
+    r""":py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>` object.
 
     Attributes
     ----------
-    :py:attr:`name` : str
-        Name of the spur gear.
-    :py:attr:`n_teeth` : int
+    :py:attr:`name` : :py:class:`str`
+        Name of the worm wheel.
+    :py:attr:`n_teeth` : :py:class:`int`
         Number of gear teeth.
-    :py:attr:`inertia_moment` : InertiaMoment
+    :py:attr:`inertia_moment` : :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`
         Moment of inertia of the gear.
-    :py:attr:`module` : Length
+    :py:attr:`helix_angle` : :py:class:`Angle <gearpy.units.units.Angle>`
+        Helix angle of the worm wheel.
+    :py:attr:`pressure_angle` : :py:class:`Angle <gearpy.units.units.Angle>`
+        Pressure angle of the worm wheel.
+    :py:attr:`module` : :py:class:`Length <gearpy.units.units.Length>`
         Unit of the gear teeth size.
-    :py:attr:`reference_diameter` : Length
+    :py:attr:`reference_diameter` : :py:class:`Length <gearpy.units.units.Length>`
         Reference diameter of the gear.
-    :py:attr:`face_width` : Length
+    :py:attr:`face_width` : :py:class:`Length <gearpy.units.units.Length>`
         Face width of the gear.
-    :py:attr:`elastic_modulus` : Stress
-        Elastic modulus of the material of the gear.
-    :py:attr:`lewis_factor` : float
+    :py:attr:`lewis_factor` : :py:attr:`float`
         Factor used to compute stresses on the gear tooth.
-    :py:attr:`driven_by` : RotatingObject
-        Rotating object that drives the gear, for example a motor, a flywheel or another gear.
-    :py:attr:`drives` : RotatingObject
-        Rotating object driven by the gear, it can be a flywheel or another gear.
-    :py:attr:`master_gear_ratio` : float
+    :py:attr:`driven_by` : :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
+        Rotating object that drives the gear, for example a
+        :py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>`, a
+        :py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` or another gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`).
+    :py:attr:`drives` : :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
+        Rotating object driven by the gear, it can be a
+        :py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` or another gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`).
+    :py:attr:`master_gear_ratio` : :py:class:`float`
         Gear ratio of the mating between the gear and its driving gear.
-    :py:attr:`master_gear_efficiency` : float or int
+    :py:attr:`master_gear_efficiency` : :py:class:`float` or :py:class:`int`
         Efficiency of the gear mating between the gear and its driving gear.
-    :py:attr:`mating_role`: Role
+    :py:attr:`mating_role`: :py:class:`Role <gearpy.mechanical_objects.mechanical_object_base.Role>`
         The role of the gear in the gear mating.
-    :py:attr:`angular_position` : AngularPosition
+    :py:attr:`angular_position` : :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`
         Angular position of the gear.
-    :py:attr:`angular_speed` : AngularSpeed
+    :py:attr:`angular_speed` : :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`
         Angular speed of the gear.
-    :py:attr:`angular_acceleration` : AngularAcceleration
+    :py:attr:`angular_acceleration` : :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`
         Angular acceleration of the gear.
-    :py:attr:`torque` : Torque
+    :py:attr:`torque` : :py:class:`Torque <gearpy.units.units.Torque>`
         Net torque applied on the gear.
-    :py:attr:`driving_torque` : Torque
+    :py:attr:`driving_torque` : :py:class:`Torque <gearpy.units.units.Torque>`
         Driving torque applied on the gear by its driving gear.
-    :py:attr:`load_torque` : Torque
+    :py:attr:`load_torque` : :py:class:`Torque <gearpy.units.units.Torque>`
         Load torque applied on the gear by its driven gear or an external load.
-    :py:attr:`tangential_force` : Force
+    :py:attr:`tangential_force` : :py:class:`Force <gearpy.units.units.Force>`
         Tangential force applied on the gear teeth by the mating gear.
-    :py:attr:`tangential_force_is_computable` : bool
-        Whether is possible to compute the tangential force on the gear teeth.
-    :py:attr:`bending_stress` : Stress
+    :py:attr:`tangential_force_is_computable` : :py:class:`bool`
+        Whether is possible to compute the :py:attr:`tangential_force` on the gear teeth.
+    :py:attr:`bending_stress` : :py:class:`Stress <gearpy.units.units.Stress>`
         Bending stress applied on the gear teeth by the mating gear.
-    :py:attr:`bending_stress_is_computable` : bool
-        Whether is possible to compute the bending stress on the gear teeth.
-    :py:attr:`contact_stress` : Stress
-        The stress generated by the contact with mating gear teeth.
-    :py:attr:`contact_stress_is_computable` : bool
-        Whether is possible to compute the contact stress on the gear teeth.
-    :py:attr:`time_variables` : dict
+    :py:attr:`bending_stress_is_computable` : :py:class:`bool`
+        Whether is possible to compute the :py:attr:`bending_stress` on the gear teeth.
+    :py:attr:`time_variables` : :py:class:`dict`
         Time variables of the gear.
 
     Methods
     -------
     :py:meth:`compute_tangential_force`
-        Computes the tangential force applied on the gear teeth by the mating gear.
+        It computes the :py:attr:`tangential_force` applied on the gear teeth by the mating gear.
     :py:meth:`compute_bending_stress`
-        Computes the bending stress applied on the gear teeth by the mating gear.
-    :py:meth:`compute_contact_stress`
-        Computes the contact stress generated by the contact with mating gear teeth.
+        It computes the :py:attr:`bending_stress` applied on the gear teeth by the mating gear.
     :py:meth:`external_torque`
         Custom function to compute the external torque applied on the gear.
     :py:meth:`update_time_variables`
-        Updates ``time_variables`` dictionary by appending the last value of each time variable to corresponding list.
+        It updates :py:attr:`time_variables` dictionary by appending the last value of each time variable to
+        corresponding list.
     """
 
     def __init__(self,
                  name: str,
                  n_teeth: int,
                  inertia_moment: InertiaMoment,
+                 helix_angle: Angle,
+                 pressure_angle: Angle,
                  module: Optional[Length] = None,
-                 face_width: Optional[Length] = None,
-                 elastic_modulus: Optional[Stress] = None):
+                 face_width: Optional[Length] = None):
         super().__init__(name = name,
                          n_teeth = n_teeth,
                          module = module,
                          face_width = face_width,
                          inertia_moment = inertia_moment,
-                         elastic_modulus = elastic_modulus)
+                         helix_angle = helix_angle,
+                         elastic_modulus = None)
+
+        if not isinstance(pressure_angle, Angle):
+            raise TypeError(f"Parameter 'pressure_angle' must be an instance of {Angle.__name__!r}.")
+
+        if pressure_angle not in WORM_GEAR_AND_WHEEL_AVAILABLE_PRESSURE_ANGLES:
+            raise ValueError(f"Value {pressure_angle!r} for parameter 'pressure_angle' not available. "
+                             f"Available pressure angles are: {WORM_GEAR_AND_WHEEL_AVAILABLE_PRESSURE_ANGLES}")
+
+        maximum_helix_angle = worm_gear_and_wheel_maximum_helix_angle_function(pressure_angle = pressure_angle)
+        if helix_angle > maximum_helix_angle:
+            raise ValueError(f"Parameter 'helix_angle' too high. For a {pressure_angle} 'pressure_angle', "
+                             f"the maximum 'helix_angle' is {maximum_helix_angle}.")
+
+        self.__helix_angle = helix_angle
+        self.__pressure_angle = pressure_angle
 
         if self.tangential_force_is_computable:
             self.time_variables['tangential force'] = []
 
             if self.bending_stress_is_computable:
                 self.time_variables['bending stress'] = []
-                self.__lewis_factor = lewis_factor_function(self.n_teeth).take(0)
-
-                if self.contact_stress_is_computable:
-                    self.time_variables['contact stress'] = []
-                    self.__PRESSURE_ANGLE = Angle(20, 'deg')
+                self.__lewis_factor = worm_wheel_lewis_factor_function(pressure_angle = pressure_angle)
 
     @property
     def name(self) -> str:
-        """Name of the spur gear. It must be a non-empty string. \n
+        """Name of the worm wheel. It must be a non-empty :py:class:`str`. \n
         It must be a unique name, not shared by other elements in the powertrain elements. \n
-        Once set at the spur gear instantiation, it cannot be changed afterward.
+        Once set at the worm wheel instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        str
-            Name of the spur gear.
+        :py:class:`str`
+            Name of the worm wheel.
+
+        .. admonition:: Raises
+           :class: warning
 
-        Raises
-        ------
-        TypeError
-            If ``name`` is not a string.
-        ValueError
-            If ``name`` is an empty string.
+           ``TypeError``
+               If :py:attr:`name` is not a :py:class:`str`.
+           ValueError
+               If :py:attr:`name` is an empty :py:class:`str`.
         """
         return super().name
 
     @property
     def n_teeth(self) -> int:
-        """Number of gear teeth. It must be a positive integer. \n
-        Once set at the spur gear instantiation, it cannot be changed afterward.
+        """Number of gear teeth. It must be a positive :py:class:`int`. \n
+        Once set at the worm wheel instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        int
+        :py:class:`int`
             Number of gear teeth.
 
-        Raises
-        ------
-        TypeError
-            If ``n_teeth`` is not an integer.
-        ValueError
-            If ``n_teeth`` is less than the minimum number of teeth, based on Lewis Factor table.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`n_teeth` is not an :py:class:`int`.
+           ``ValueError``
+               If :py:attr:`n_teeth` is less than the minimum number of teeth, based on Lewis Factor table.
         """
         return super().n_teeth
 
     @property
     def inertia_moment(self) -> InertiaMoment:
-        """Moment of inertia of the gear. It must be an instance of ``InertiaMoment``. \n
-        Once set at the spur gear instantiation, it cannot be changed afterward.
+        """Moment of inertia of the gear. It must be an instance of
+        :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`. \n
+        Once set at the worm wheel instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        InertiaMoment
+        :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`
             Moment of inertia of the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``inertia_moment`` is not an instance of ``InertiaMoment``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.InertiaMoment`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`inertia_moment` is not an instance of
+               :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`.
         """
         return super().inertia_moment
 
     @property
-    def module(self) -> Optional[Length]:
-        """Unit of the gear teeth size. It must be an instance of ``Length``. \n
-        Once set at the spur gear instantiation, it cannot be changed afterward.
+    def helix_angle(self) -> Angle:
+        """Helix angle of the worm wheel. It must be an instance of :py:class:`Angle <gearpy.units.units.Angle>`. \n
+        The maximum allowable value of helix angle depends on the :py:attr:`pressure_angle`. \n
+        Once set at the worm gear instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        Length
-            Unit of the gear teeth size.
+        :py:class:`Angle <gearpy.units.units.Angle>`
+            The helix angle of the worm wheel.
 
-        Raises
-        ------
-        TypeError
-            If ``module`` is not an instance of ``Length``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Length`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`helix_angle` is not an instance of :py:class:`Angle <gearpy.units.units.Angle>`.
+           ``ValueError``
+               If :py:attr:`helix_angle` is greater than the maximum allowable helix angle, depending on
+               :py:attr:`pressure_angle` value.
         """
-        return super().module
+        return self.__helix_angle
 
     @property
-    def reference_diameter(self) -> Optional[Length]:
-        """Reference diameter of the gear. It must be an instance of ``Length``. \n
-        It is computed as the product of ``n_teeth`` times ``module`` at the spur gear instantiation and it cannot be
-        changed afterward.
+    def pressure_angle(self) -> Angle:
+        """Pressure angle of the worm wheel. It must be an instance of :py:class:`Angle <gearpy.units.units.Angle>` and
+        its value must be one of: 14.5 deg, 20 deg, 25 deg or 30 deg. \n
+        Once set at the worm wheel instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        Length
-            Reference diameter of the gear.
+        :py:class:`Angle <gearpy.units.units.Angle>`
+            The pressure angle of the worm wheel.
+
+        .. admonition:: Raises
+           :class: warning
 
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Length`
+           ``TypeError``
+               If :py:attr:`pressure_angle` is not an instance of :py:class:`Angle <gearpy.units.units.Angle>`.
+           ``ValueError``
+               If :py:attr:`pressure_angle` value is not among available ones: 14.5 deg, 20 deg, 25 deg or 30 deg.
         """
-        return super().reference_diameter
+        return self.__pressure_angle
 
     @property
-    def face_width(self) -> Optional[Length]:
-        """Face width of the gear. It must be an instance of ``Length``.
+    def module(self) -> Optional[Length]:
+        """Unit of the gear teeth size. It must be an instance of :py:class:`Length <gearpy.units.units.Length>`. \n
+        Once set at the worm wheel instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        Length
-            Face width of the gear.
+        :py:class:`Length <gearpy.units.units.Length>`
+            Unit of the gear teeth size.
 
-        Raises
-        ------
-        TypeError
-            If ``face_width`` is not an instance of ``Length``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Length`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`module` is not an instance of :py:class:`Length <gearpy.units.units.Length>`.
         """
-        return super().face_width
+        return super().module
 
     @property
-    def elastic_modulus(self) -> Optional[Stress]:
-        """Elastic modulus of the material of the gear. It must be an instance of ``Stress``. It must be positive.
+    def reference_diameter(self) -> Optional[Length]:
+        """Reference diameter of the gear. It must be an instance of :py:class:`Length <gearpy.units.units.Length>`. \n
+        It is computed as the product of :py:attr:`n_teeth` times :py:attr:`module` at the worm wheel instantiation and
+        it cannot be changed afterward.
 
         Returns
         -------
-        Stress
-            Elastic modulus of the material of the gear.
+        :py:class:`Length <gearpy.units.units.Length>`
+            Reference diameter of the gear.
+        """
+        return super().reference_diameter
 
-        Raises
-        ------
-        TypeError
-            If ``elastic_modulus`` is not an instance of ``Stress``.
-        ValueError
-            If ``elastic_modulus`` value is negative or null.
+    @property
+    def face_width(self) -> Optional[Length]:
+        """Face width of the gear. It must be an instance of :py:class:`Length <gearpy.units.units.Length>`.
+
+        Returns
+        -------
+        :py:class:`Length <gearpy.units.units.Length>`
+            Face width of the gear.
 
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Stress`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`face_width` is not an instance of :py:class:`Length <gearpy.units.units.Length>`.
         """
-        return super().elastic_modulus
+        return super().face_width
 
     @property
     def lewis_factor(self) -> Optional[float]:
         """Factor used to compute stresses on the gear tooth. \n
-        It is a tabular value that in general depends on the number of gear teeth and the pressure angle. In this
-        case, the considered pressure angle is always 20 degrees, so the Lewis factor depends only on the number of gear
-        teeth.
+        It is a tabular value that depends on the :py:attr:`pressure_angle`.
 
         Returns
         -------
-        float
+        :py:attr:`float`
             Factor used to compute stresses on the gear tooth.
         """
         return self.__lewis_factor
 
     @property
     def driven_by(self) -> RotatingObject:
-        """Rotating object that drives the gear, for example a motor, a flywheel or another gear. It must be a
-        ``RotatingObject``.
+        """Rotating object that drives the gear, for example a
+        :py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>`, a
+        :py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` or another gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`). It must be a
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`. \n
+        To set this property use :py:func:`add_worm_gear_mating <gearpy.utils.relations.add_worm_gear_mating>` or
+        :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
-        RotatingObject
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
             Master rotating object that drives the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``driven_by`` is not an instance of ``RotatingObject``.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_gear_mating`
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`driven_by` is not an instance of
+               :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`.
         """
         return super().driven_by
 
     @driven_by.setter
     def driven_by(self, driven_by: RotatingObject):
-        super(SpurGear, type(self)).driven_by.fset(self, driven_by)
+        super(WormWheel, type(self)).driven_by.fset(self, driven_by)
 
     @property
     def drives(self) -> RotatingObject:
-        """Rotating object driven by the gear, it can be a flywheel or another gear. It must be a ``RotatingObject``.
+        """Rotating object driven by the gear, it can be a
+        :py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` or another gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`). It must be a
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`. \n
+        To set this property use :py:func:`add_worm_gear_mating <gearpy.utils.relations.add_worm_gear_mating>` or
+        :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
-        RotatingObject
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
             Rotating object driven by the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``drives`` is not an instance of ``RotatingObject``.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_gear_mating`
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`drives` is not an instance of
+               :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`.
         """
         return super().drives
 
     @drives.setter
     def drives(self, drives: RotatingObject):
-        super(SpurGear, type(self)).drives.fset(self, drives)
+        super(WormWheel, type(self)).drives.fset(self, drives)
 
     @property
     def master_gear_ratio(self) -> float:
-        """Gear ratio of the mating between the gear and its driving gear. It must be a positive a float. \n
-        If the gear is fixed to another driving ``RotatingObject``, then the ratio is ``1``, otherwise it is defined as
-        the ratio between the gear number of teeth ``n_teeth`` and the same parameter of the master (driving) gear. \n
-        To set this property use :py:func:`gearpy.utils.relations.add_gear_mating` or
-        :py:func:`gearpy.utils.relations.add_fixed_joint`.
+        """Gear ratio of the mating between the gear and its driving gear. It must be a positive a :py:class:`float`. \n
+        If the wheel gear is fixed to another driving
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`, then the ratio is
+        ``1``, otherwise it is defined as the ratio between the worm wheel number of teeth :py:attr:`n_teeth` and the
+        driving  worm gear number of starts
+        :py:attr:`WormGear.n_starts <gearpy.mechanical_objects.worm_gear.WormGear.n_starts>`. \n
+        To set this property use :py:func:`add_worm_gear_mating <gearpy.utils.relations.add_worm_gear_mating>` or
+        :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
-        float
+        :py:class:`float`
             Gear ratio of the mating between the gear and its driving gear.
 
-        Raises
-        ------
-        TypeError
-            If ``master_gear_ratio`` is not a float.
-        ValueError
-            If ``master_gear_ratio`` is negative or null.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_gear_mating`
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`master_gear_ratio` is not a :py:class:`float`.
+           ``ValueError``
+               If :py:attr:`master_gear_ratio` is negative or null.
         """
         return super().master_gear_ratio
 
     @master_gear_ratio.setter
     def master_gear_ratio(self, master_gear_ratio: float):
-        super(SpurGear, type(self)).master_gear_ratio.fset(self, master_gear_ratio)
+        super(WormWheel, type(self)).master_gear_ratio.fset(self, master_gear_ratio)
 
     @property
     def master_gear_efficiency(self) -> Union[float, int]:
-        """Efficiency of the gear mating between the gear and its driving gear. It must be a float or an integer within
-        ``0`` and ``1``. \n
-        To set this property use :py:func:`gearpy.utils.relations.add_gear_mating` or
-        :py:func:`gearpy.utils.relations.add_fixed_joint`.
+        """Efficiency of the gear mating between the gear and its driving gear. It must be a :py:class:`float`  or an
+        :py:class:`int` within ``0`` and ``1``. \n
+        To set this property use :py:func:`add_worm_gear_mating <gearpy.utils.relations.add_worm_gear_mating>` or
+        :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Efficiency of the gear mating between the gear and its driving gear.
 
-        Raises
-        ------
-        TypeError
-            If ``master_gear_efficiency`` is not a float or an integer.
-        ValueError
-            If ``master_gear_efficiency`` is not within ``0`` and ``1``.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_gear_mating`
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`master_gear_efficiency` is not a :py:class:`float` or an :py:class:`int`.
+           ``ValueError``
+               If :py:attr:`master_gear_efficiency` is not within ``0`` and ``1``.
         """
         return super().master_gear_efficiency
 
     @master_gear_efficiency.setter
     def master_gear_efficiency(self, master_gear_efficiency: Union[float, int]):
-        super(SpurGear, type(self)).master_gear_efficiency.fset(self, master_gear_efficiency)
+        super(WormWheel, type(self)).master_gear_efficiency.fset(self, master_gear_efficiency)
 
     @property
     def mating_role(self) -> Role:
-        """Role of the gear in the gear mating. To set this parameter use ``add_gear_mating``. \n
-        If the gear drives the mate one, then it is the "master" gear and its role is ``MatingMaster``, otherwise it is
-        the "slave" one and its role is ``MatingSlave``.
+        """Role of the gear in the gear mating. \n
+        If the gear drives the mate one, then it is the "master" gear and its role is
+        :py:class:`MatingMaster <gearpy.mechanical_objects.mating_roles.MatingMaster>`, otherwise it is
+        the "slave" one and its role is :py:class:`MatingSlave <gearpy.mechanical_objects.mating_roles.MatingSlave>`. \n
+        To set this parameter use :py:func:`add_worm_gear_mating <gearpy.utils.relations.add_worm_gear_mating>`.
 
         Returns
         -------
-        Role
+        :py:class:`Role <gearpy.mechanical_objects.mechanical_object_base.Role>`
             The role of the gear in the gear mating.
 
-        Raises
-        ------
-        ValueError
-            If ``mating_role`` is not a subclass of ``Role``.
+        .. admonition:: Raises
+           :class: warning
+
+           ``ValueError``
+               If :py:attr:`mating_role` is not a subclass of
+               :py:class:`Role <gearpy.mechanical_objects.mechanical_object_base.Role>`.
         """
         return super().mating_role
 
     @mating_role.setter
     def mating_role(self, mating_role: Role):
-        super(SpurGear, type(self)).mating_role.fset(self, mating_role)
+        super(WormWheel, type(self)).mating_role.fset(self, mating_role)
 
     @property
     def angular_position(self) -> AngularPosition:
-        """Angular position of the gear. It must be an instance of ``AngularPosition``.
+        """Angular position of the gear. It must be an instance of
+        :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`.
 
         Returns
         -------
-        AngularPosition
+        :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`
             Angular position of the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``angular_position`` is not an instance of ``AngularPosition``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularPosition`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`angular_position` is not an instance of
+               :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`.
         """
         return super().angular_position
 
     @angular_position.setter
     def angular_position(self, angular_position: AngularPosition):
-        super(SpurGear, type(self)).angular_position.fset(self, angular_position)
+        super(WormWheel, type(self)).angular_position.fset(self, angular_position)
 
     @property
     def angular_speed(self) -> AngularSpeed:
-        """Angular speed of the gear. It must be an instance of ``AngularSpeed``.
+        """Angular speed of the gear. It must be an instance of
+        :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`.
 
         Returns
         -------
-        AngularSpeed
+        :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`
             Angular speed of the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``angular_speed`` is not an instance of ``AngularSpeed``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularSpeed`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`angular_speed` is not an instance of
+               :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`.
         """
         return super().angular_speed
 
     @angular_speed.setter
     def angular_speed(self, angular_speed: AngularSpeed):
-        super(SpurGear, type(self)).angular_speed.fset(self, angular_speed)
+        super(WormWheel, type(self)).angular_speed.fset(self, angular_speed)
 
     @property
     def angular_acceleration(self) -> AngularAcceleration:
-        """Angular acceleration of the gear. It must be an instance of ``AngularAcceleration``.
+        """Angular acceleration of the gear. It must be an instance of
+        :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`.
 
         Returns
         -------
-        AngularAcceleration
+        :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`
             Angular acceleration of the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``angular_acceleration`` is not an instance of ``AngularAcceleration``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularAcceleration`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`angular_acceleration` is not an instance of
+               :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`.
         """
         return super().angular_acceleration
 
     @angular_acceleration.setter
     def angular_acceleration(self, angular_acceleration: AngularAcceleration):
-        super(SpurGear, type(self)).angular_acceleration.fset(self, angular_acceleration)
+        super(WormWheel, type(self)).angular_acceleration.fset(self, angular_acceleration)
 
     @property
     def torque(self) -> Torque:
-        """Net torque applied on the gear. It must be an instance of ``Torque``. \n
-        It is computed as the difference between ``driving_torque`` and ``load_torque``.
+        """Net torque applied on the gear. It must be an instance of :py:class:`Torque <gearpy.units.units.Torque>`. \n
+        It is computed as the difference between :py:attr:`driving_torque` and :py:attr:`load_torque`.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Net torque applied on the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``torque`` is not an instance of ``Torque``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Torque`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`torque` is not an instance of :py:class:`Torque <gearpy.units.units.Torque>`.
         """
         return super().torque
 
     @torque.setter
     def torque(self, torque: Torque):
-        super(SpurGear, type(self)).torque.fset(self, torque)
+        super(WormWheel, type(self)).torque.fset(self, torque)
 
     @property
     def driving_torque(self) -> Torque:
-        """Driving torque applied on the gear by its driving gear. It must be an instance of ``Torque``.
+        """Driving torque applied on the gear by its driving gear. It must be an instance of
+        :py:class:`Torque <gearpy.units.units.Torque>`.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Driving torque applied on the gear by its driving gear.
 
-        Raises
-        ------
-        TypeError
-            If ``driving_torque`` is not an instance of ``Torque``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Torque`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`driving_torque` is not an instance of :py:class:`Torque <gearpy.units.units.Torque>`.
         """
         return super().driving_torque
 
     @driving_torque.setter
     def driving_torque(self, driving_torque: Torque):
-        super(SpurGear, type(self)).driving_torque.fset(self, driving_torque)
+        super(WormWheel, type(self)).driving_torque.fset(self, driving_torque)
 
     @property
     def load_torque(self) -> Torque:
-        """Load torque applied on the gear by its driven gear or an external load. It must be an instance of ``Torque``.
+        """Load torque applied on the gear by its driven gear or an external load. It must be an instance of
+        :py:class:`Torque <gearpy.units.units.Torque>`.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Load torque applied on the gear by its driven gear or an external load.
 
-        Raises
-        ------
-        TypeError
-            If ``load_torque`` is not an instance of ``Torque``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Torque`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`load_torque` is not an instance of :py:class:`Torque <gearpy.units.units.Torque>`.
         """
         return super().load_torque
 
     @load_torque.setter
     def load_torque(self, load_torque: Torque):
-        super(SpurGear, type(self)).load_torque.fset(self, load_torque)
+        super(WormWheel, type(self)).load_torque.fset(self, load_torque)
 
     @property
     def tangential_force(self) -> Force:
-        """Tangential force applied on the gear teeth by the mating gear. It must be an instance of ``Force``.
+        """Tangential force applied on the gear teeth by the mating gear. It must be an instance of
+        :py:class:`Force <gearpy.units.units.Force>`.
 
         Returns
         -------
-        Force
+        :py:class:`Force <gearpy.units.units.Force>`
             Tangential force applied on the gear teeth by the mating gear.
 
-        Raises
-        ------
-        TypeError
-            If ``tangential_force`` is not an instance of ``Force``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Force`
-        :py:meth:`compute_tangential_force`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`tangential_force` is not an instance of :py:class:`Force <gearpy.units.units.Force>`.
+
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`compute_tangential_force`
         """
         return super().tangential_force
 
     @tangential_force.setter
     def tangential_force(self, tangential_force: Force):
-        super(SpurGear, type(self)).tangential_force.fset(self, tangential_force)
+        super(WormWheel, type(self)).tangential_force.fset(self, tangential_force)
 
-    def compute_tangential_force(self):
-        """Computes the tangential force applied on the gear teeth by the mating gear. \n
+    def compute_tangential_force(self) -> None:
+        """It computes the :py:attr:`tangential_force` applied on the gear teeth by the mating gear. \n
         Considering a gear mating:
 
-        - if the gear is the master one, then it takes into account the ``load_torque`` for the computation,
-        - if the gear is the slave one, then it take into account the ``driving_torque`` for the computation.
+        - if the gear is the master one, then it takes into account the :py:attr:`load_torque` for the computation,
+        - if the gear is the slave one, then it take into account the :py:attr:`driving_torque` for the computation.
 
         The tangential force is computed dividing the just described reference torque by the reference radius (half of
-        the reference diameter).
+        the :py:attr:`reference_diameter`).
 
-        Raises
-        ------
-        ValueError
-            If a gear mating between two gears has not been set.
-
-        See Also
-        --------
-        :py:attr:`tangential_force`
+        .. admonition:: Raises
+           :class: warning
+
+           ``ValueError``
+               If a gear mating between two gears has not been set.
         """
         if self.mating_role == MatingMaster:
             self.tangential_force = abs(self.load_torque)/(self.reference_diameter/2)
         elif self.mating_role == MatingSlave:
             self.tangential_force = abs(self.driving_torque)/(self.reference_diameter/2)
         else:
             raise ValueError("Gear mating not defined. "
-                             "Use 'gearpy.utils.add_gear_mating' to set up a mating between two gears.")
+                             "Use 'gearpy.utils.add_worm_gear_mating' to set up a mating between two gears.")
 
     @property
     def tangential_force_is_computable(self) -> bool:
-        """Whether is possible to compute the tangential force on the gear teeth. The tangential force computation
-        depends on the value of ``module``, so if this optional parameter has been set at spur gear instantiation, then
-        it is possible to compute the tangential force and this property is ``True``, otherwise is ``False``.
+        """Whether is possible to compute the :py:attr:`tangential_force` on the gear teeth. \n
+        The tangential force computation depends on the value of :py:attr:`module`, so if this optional parameter has
+        been set at worm wheel instantiation, then it is possible to compute the tangential force and this property is
+        ``True``, otherwise is ``False``.
 
         Returns
         -------
-        bool
+        :py:class:`bool`
             Whether is possible to compute the tangential force on the gear teeth.
 
-        See Also
-        --------
-        :py:attr:`module`
-        :py:attr:`tangential_force`
-        :py:meth:`compute_tangential_force`
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`compute_tangential_force`
         """
         return super().tangential_force_is_computable
 
     @property
     def bending_stress(self) -> Stress:
-        """Bending stress applied on the gear teeth by the mating gear. It must be an instance of ``Stress``.
+        """Bending stress applied on the gear teeth by the mating gear. It must be an instance of
+        :py:class:`Stress <gearpy.units.units.Stress>`.
 
         Returns
         -------
-        Stress
+        :py:class:`Stress <gearpy.units.units.Stress>`
             Bending stress applied on the gear teeth by the mating gear.
 
-        Raises
-        ------
-        TypeError
-            If ``bending_stress`` is not an instance of ``Stress``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Stress`
-        :py:meth:`compute_bending_stress`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`bending_stress` is not an instance of :py:class:`Stress <gearpy.units.units.Stress>`.
+
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`compute_bending_stress`
         """
         return super().bending_stress
 
     @bending_stress.setter
     def bending_stress(self, bending_stress: Stress):
-        super(SpurGear, type(self)).bending_stress.fset(self, bending_stress)
+        super(WormWheel, type(self)).bending_stress.fset(self, bending_stress)
 
-    def compute_bending_stress(self):
-        r"""Computes the bending stress applied on the gear teeth by the mating gear.
+    def compute_bending_stress(self) -> None:
+        r"""It computes the :py:attr:`bending_stress` applied on the gear teeth by the mating gear.
 
-        Notes
-        -----
-        The bending stress computation is based on the following assumptions:
-
-        - the tooth is stressed by the overall force acting on the tip of the tooth itself,
-        - the most unfavorable situation is considered in the calculation, as if there is only one pair of teeth in
-          contact within the contact segment,
-        - the component of the overall force that determines the bending on the tooth is the only one considered and,
-          for simplicity, is taken as having a value equal to the tangential force on the reference diameter,
-        - the radial component of the overall force that causes a compressive stress on the tooth is neglected.
-
-        The bending stress is computed with the following formula:
-
-        .. math::
-            \sigma_b = \frac{F_t}{m \, b \, Y_{LW}}
-
-        where:
-
-        - :math:`F_t` is the tangential force applied on the tooth,
-        - :math:`m` is the gear module (``module``),
-        - :math:`b` is the gear tooth face width (``face_width``),
-        - :math:`Y_{LW}` is the gear Lewis factor (``lewis_factor``).
-
-        See Also
-        --------
-        :py:attr:`bending_stress`
-        :py:attr:`tangential_force`
-        :py:attr:`module`
-        :py:attr:`face_width`
-        :py:attr:`lewis_factor`
-        """
-        self.bending_stress = self.tangential_force/(self.module*self.face_width)/self.lewis_factor
+        .. admonition:: Notes
+           :class: tip
 
-    @property
-    def bending_stress_is_computable(self) -> bool:
-        """Whether is possible to compute the bending stress on the gear teeth. The bending stress computation depends
-        on the value of ``module`` and ``face_width``, so if these optional parameters have been set at spur gear
-        instantiation, then it is possible to compute the bending stress and this property is ``True``, otherwise is
-        ``False``.
+           The bending stress computation is based on the following assumptions:
 
-        Returns
-        -------
-        bool
-            Whether is possible to compute the bending stress on the gear teeth.
+           - the tooth is stressed by the overall force acting on the tip of the tooth itself,
+           - the most unfavorable situation is considered in the calculation, as if there is only one pair of teeth in
+             contact within the contact segment,
+           - the component of the overall force that determines the bending on the tooth is the only one considered and,
+             for simplicity, is taken as having a value equal to the tangential force on the reference diameter,
+           - the radial component of the overall force that causes a compressive stress on the tooth is neglected.
+
+           The bending stress is computed with the following formula:
+
+           .. math::
+               \sigma_b = \frac{F_t}{p_n \, b_{eff} \, Y_{LW}}
+
+           where:
 
-        See Also
-        --------
-        :py:attr:`module`
-        :py:attr:`face_width`
-        :py:attr:`bending_stress`
-        :py:meth:`compute_bending_stress`
-        """
-        return super().bending_stress_is_computable
-
-    @property
-    def contact_stress(self) -> Stress:
-        """Stress generated by the contact with mating gear teeth. It must be an instance of ``Stress``.
-
-        Returns
-        -------
-        Stress
-            The stress generated by the contact with mating gear teeth.
-
-        Raises
-        ------
-        TypeError
-            If ``contact_stress`` is not an instance of ``Stress``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Stress`
-        :py:meth:`compute_contact_stress`
-        """
-        return super().contact_stress
-
-    @contact_stress.setter
-    def contact_stress(self, contact_stress: Stress):
-        super(SpurGear, type(self)).contact_stress.fset(self, contact_stress)
-
-    def compute_contact_stress(self):
-        r"""Computes the contact stress generated by the contact with mating gear teeth.
-
-        Raises
-        ------
-        ValueError
-            - If a gear mating between two gears has not been set,
-            - if gear role is ``MatingMaster`` and its slave gear misses ``module`` parameter,
-            - if gear role is ``MatingMaster`` and its slave gear misses ``elastic_modulus`` parameter,
-            - if gear role is ``MatingSlave`` and its master gear misses ``module`` parameter,
-            - if gear role is ``MatingSlave`` and its master gear misses ``elastic_modulus`` parameter.
-
-        Notes
-        -----
-        The contact stress computation is based on the following assumptions:
-
-        - perfect elasticity of the materials the two mating gear,
-        - absence of friction forces in the contact point,
-        - small size of the contact surface compared to the size of the bodies between which contact occurs.
-
-        The contact stress is computed with the following formula:
-
-        .. math::
-            \sigma_c = 0.262922 \, \sqrt{\frac{4 \, F_t}{b \, \cos \alpha \, \sin \alpha}
-            \left( \frac{1}{D_1} + \frac{1}{D_2} \right) \, \frac{E_1 \, E_2}{E_1 + E_2}}
-
-        where:
-
-        - :math:`F_t` is the tangential force applied on the tooth,
-        - :math:`b` is the gear face width (``face_width``),
-        - :math:`\alpha` is the pressure angle of the gear, always equal to 20 degrees,
-        - :math:`D_1` is the gear reference diameter (``reference_diameter``),
-        - :math:`D_2` is the mating gear reference diameter,
-        - :math:`E_1` is the gear elastic modulus (``elastic_modulus``),
-        - :math:`E_2` is the mating gear elastic modulus.
-
-        See Also
-        --------
-        :py:attr:`contact_stress`
-        :py:attr:`tangential_force`
-        :py:attr:`elastic_modulus`
-        :py:attr:`face_width`
-        :py:attr:`reference_diameter`
+           - :math:`F_t` is the :py:attr:`tangential_force` applied on the tooth,
+           - :math:`p_n` is the normal pitch,
+           - :math:`b_{eff}` is the effective tooth face width,
+           - :math:`Y_{LW}` is the gear Lewis factor :py:attr:`lewis_factor`.
+
+           The normal pitch can be computed with:
+
+           .. math::
+               p_n = \frac{\pi d_{wg} \sin \beta}{N}
+
+           where:
+
+           - :math:`d_{wg}` is the mating worm gear :py:attr:`reference_diameter`,
+           - :math:`\beta` is the mating worm gear :py:attr:`helix_angle`,
+           - :math:`N` is the worm wheel number of teeth :py:attr:`n_teeth`.
+
+           The effective tooth face width :math:`b_{eff}` is the minimum between the worm wheel face width 
+           :py:attr:`face_width` and the mating worm gear reference diameter multiplied by 0.67.
         """
         if self.mating_role == MatingMaster:
-            if self.drives.module is not None:
-                mate_reference_diameter = self.drives.reference_diameter
-            else:
-                raise ValueError(f"Impossible to compute contact stress for {self.__class__.__name__} {self.name!r} "
-                                 f"because its mating {self.__class__.__name__} {self.drives.name!r} misses "
-                                 f"'module' parameter.")
-            if self.drives.elastic_modulus is not None:
-                mate_elastic_modulus = self.drives.elastic_modulus
-            else:
-                raise ValueError(f"Impossible to compute contact stress for {self.__class__.__name__} {self.name!r} "
-                                 f"because its mating {self.__class__.__name__} {self.drives.name!r} misses "
-                                 f"'elastic_modulus' parameter.")
+            normal_pitch = pi*self.drives.reference_diameter*self.drives.helix_angle.sin()/self.n_teeth
+            effective_face_width = min(self.face_width, 0.67*self.drives.reference_diameter)
         elif self.mating_role == MatingSlave:
-            if self.driven_by.module is not None:
-                mate_reference_diameter = self.driven_by.reference_diameter
-            else:
-                raise ValueError(f"Impossible to compute contact stress for {self.__class__.__name__} {self.name!r} "
-                                 f"because its mating {self.__class__.__name__} {self.driven_by.name!r} misses "
-                                 f"'module' parameter.")
-            if self.driven_by.elastic_modulus is not None:
-                mate_elastic_modulus = self.driven_by.elastic_modulus
-            else:
-                raise ValueError(f"Impossible to compute contact stress for {self.__class__.__name__} {self.name!r} "
-                                 f"because its mating {self.__class__.__name__} {self.driven_by.name!r} misses "
-                                 f"'elastic_modulus' parameter.")
+            normal_pitch = pi*self.driven_by.reference_diameter*self.driven_by.helix_angle.sin()/self.n_teeth
+            effective_face_width = min(self.face_width, 0.67*self.driven_by.reference_diameter)
         else:
             raise ValueError("Gear mating not defined. "
-                             "Use 'gearpy.utils.add_gear_mating' to set up a mating between two gears.")
+                             "Use 'gearpy.utils.add_worm_gear_mating' to set up a mating between two gears.")
+        self.bending_stress = self.tangential_force/(normal_pitch*effective_face_width)/self.lewis_factor
 
-        equivalent_elastic_modulus = 2*self.elastic_modulus* \
-                                     (mate_elastic_modulus/(self.elastic_modulus + mate_elastic_modulus))
-        inverse_curvature_sum = self.__PRESSURE_ANGLE.sin()/2*self.reference_diameter* \
-                                (mate_reference_diameter/(self.reference_diameter + mate_reference_diameter))
-        contact_pressure = self.tangential_force/self.__PRESSURE_ANGLE.cos()/(self.face_width*inverse_curvature_sum)
-
-        self.contact_stress = Stress(value = 0.262922*sqrt(equivalent_elastic_modulus.to('Pa').value*
-                                                           contact_pressure.to('Pa').value),
-                                     unit = 'Pa')
-
-    @property
-    def contact_stress_is_computable(self) -> bool:
-        """Whether is possible to compute the contact stress force on the gear teeth. The contact stress computation
-        depends on the value of ``module``, ``face_width`` and ``elastic_modulus``, so if these optional parameters have
-        been set at spur gear instantiation, then it is possible to compute the contact stress and this property is
-        ``True``, otherwise is ``False``.
+    @property
+    def bending_stress_is_computable(self) -> bool:
+        """Whether is possible to compute the :py:attr:`bending_stress` on the gear teeth. \n
+        The bending stress computation depends on the value of :py:attr:`module` and :py:attr:`face_width` and the
+        ``reference_diameter`` of the mating :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`, so if
+        these optional parameters have been set at worm wheel and worm gear instantiations, then it is possible to
+        compute the bending stress and this property is ``True``, otherwise is ``False``.
 
         Returns
         -------
-        bool
-            Whether is possible to compute the contact stress on the gear teeth.
+        :py:class:`bool`
+            Whether is possible to compute the bending stress on the gear teeth.
+
+        .. admonition:: See Also
+           :class: seealso
 
-        See Also
-        --------
-        :py:attr:`module`
-        :py:attr:`face_width`
-        :py:attr:`elastic_modulus`
-        :py:attr:`contact_stress`
-        :py:meth:`compute_contact_stress`
+           :py:meth:`compute_bending_stress`
         """
-        return super().contact_stress_is_computable
+        if self.mating_role == MatingMaster:
+            return super().bending_stress_is_computable and (self.drives.reference_diameter is not None)
+        if self.mating_role == MatingSlave:
+            return super().bending_stress_is_computable and (self.driven_by.reference_diameter is not None)
+        else:
+            return super().bending_stress_is_computable
 
     @property
     def external_torque(self) -> Callable[[AngularPosition, AngularSpeed, Time], Torque]:
         """Custom function to compute the external torque applied on the gear. It must be a function with parameters
-        ``angular_position``, ``angular_speed`` and ``time``. The function must return an instance of ``Torque``.
+        ``angular_position``, ``angular_speed`` and ``time``. The function must return an instance of
+        :py:class:`Torque <gearpy.units.units.Torque>`.
 
         Returns
         -------
-        Callable
+        :py:obj:`Callable <typing.Callable>`
             The function to compute the external torque applied on the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``external_torque`` is not callable.
-        KeyError
-            If ``external_torque`` misses parameters ``angular_position``, ``angular_speed`` or ``time``.
-
-        Examples
-        --------
-        Constant torque, not dependent on ``angular_position``, ``angular_speed`` or ``time``.
-
-        >>> from gearpy.mechanical_objects import SpurGear
-        >>> from gearpy.units import InertiaMoment, Torque
-        >>> gear = SpurGear(name = 'gear', n_teeth = 10, inertia_moment = InertiaMoment(1, 'kgm^2'))
-        >>> gear.external_torque = lambda angular_position, angular_speed, time: Torque(5, 'Nm')
-
-        Torque dependent on ``angular_position`` and ``time``. \n
-        In this case the gear gets a periodic load, dependent on time, and an extra load dependent on its angular
-        position. The dependence by angular position may be used to model cases where cams are involved.
-
-        >>> import numpy as np
-        >>> from gearpy.units import AngularPosition, AngularSpeed, Time
-        >>> def custom_external_torque(angular_position: AngularPosition,
-        ...                            angular_speed: AngularSpeed,
-        ...                            time: Time):
-        ...     return Torque(value = angular_position.sin() +
-        ...                           np.cos(time.to('sec').value),
-        ...                   unit = 'Nm')
-        >>> gear.external_torque = custom_external_torque
-
-        Torque dependent on ``angular_position``, ``angular_speed`` and ``time``. \n
-        With respect ot the previous case, the gear gets an extra load dependent on its angular speed. The dependence by
-        angular speed may be used to model cases where air friction is not negligible.
-
-        >>> def complex_external_torque(angular_position: AngularPosition,
-        ...                             angular_speed: AngularSpeed,
-        ...                             time: Time):
-        ...     return Torque(value = angular_position.sin() +
-        ...                           0.001*(angular_speed.to('rad/s').value)**2 +
-        ...                           np.cos(time.to('sec').value),
-        ...                   unit = 'Nm')
-        >>> gear.external_torque = complex_external_torque
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`external_torque` is not callable.
+           ``KeyError``
+               If :py:attr:`external_torque` misses parameters ``angular_position``, ``angular_speed`` or ``time``.
+
+        .. admonition:: Examples
+           :class: important
+
+           Constant torque, not dependent on ``angular_position``, ``angular_speed`` or ``time``.
+
+           >>> from gearpy.mechanical_objects import WormWheel
+           >>> from gearpy.units import InertiaMoment, Torque
+           >>> gear = WormWheel(name = 'gear', n_teeth = 10, inertia_moment = InertiaMoment(1, 'kgm^2'))
+           >>> gear.external_torque = lambda angular_position, angular_speed, time: Torque(5, 'Nm')
+
+           Torque dependent on ``angular_position`` and ``time``. \n
+           In this case the gear gets a periodic load, dependent on time, and an extra load dependent on its angular
+           position. The dependence by angular position may be used to model cases where cams are involved.
+
+           >>> import numpy as np
+           >>> from gearpy.units import AngularPosition, AngularSpeed, Time
+           >>> def custom_external_torque(angular_position: AngularPosition,
+           ...                            angular_speed: AngularSpeed,
+           ...                            time: Time):
+           ...     return Torque(value = angular_position.sin() +
+           ...                           np.cos(time.to('sec').value),
+           ...                   unit = 'Nm')
+           >>> gear.external_torque = custom_external_torque
+
+           Torque dependent on ``angular_position``, ``angular_speed`` and ``time``. \n
+           With respect ot the previous case, the gear gets an extra load dependent on its angular speed. The dependence by
+           angular speed may be used to model cases where air friction is not negligible.
+
+           >>> def complex_external_torque(angular_position: AngularPosition,
+           ...                             angular_speed: AngularSpeed,
+           ...                             time: Time):
+           ...     return Torque(value = angular_position.sin() +
+           ...                           0.001*(angular_speed.to('rad/s').value)**2 +
+           ...                           np.cos(time.to('sec').value),
+           ...                   unit = 'Nm')
+           >>> gear.external_torque = complex_external_torque
         """
         return super().external_torque
 
     @external_torque.setter
     def external_torque(self, external_torque: Callable[[AngularPosition, AngularSpeed, Time], Torque]):
-        super(SpurGear, type(self)).external_torque.fset(self, external_torque)
+        super(WormWheel, type(self)).external_torque.fset(self, external_torque)
 
     @property
     def time_variables(self) -> Dict[str, List[UnitBase]]:
-        """Time variables of the gear. Each time variable is stored as a dictionary key-value pair. The available time
-        variables are:
+        """Time variables of the worm wheel. Each time variable is stored as a dictionary key-value pair. The available
+        time variables are:
 
-        - ``angular position``,
-        - ``angular speed``,
-        - ``angular acceleration``,
-        - ``torque``,
-        - ``driving torque``,
-        - ``load torque``,
-        - ``tangential force``,
-        - ``bending stress``,
-        - ``contact stress``.
-
-        ``tangential force``, ``bending stress`` and ``contact stress`` are listed among time variables only if they are
-        computable indeed, depending on which gear parameters are set at gear instantiation. \n
+        - :py:attr:`angular_position`: ``'angular position'``,
+        - :py:attr:`angular_speed`: ``'angular speed'``,
+        - :py:attr:`angular_acceleration`: ``'angular acceleration'``,
+        - :py:attr:`torque`: ``'torque'``,
+        - :py:attr:`driving_torque`: ``'driving torque'``,
+        - :py:attr:`load_torque`: ``'load torque'``,
+        - :py:attr:`tangential_force`: ``'tangential force'``,
+        - :py:attr:`bending_stress`: ``'bending stress'``.
+
+        ``'tangential force'`` and ``'bending stress'`` are listed among time variables only if they are computable
+        indeed, depending on which gear parameters are set at worm wheel instantiation; see
+        :py:attr:`tangential_force_is_computable` and :py:attr:`bending_stress_is_computable`. \n
         Corresponding values of the dictionary are lists of the respective time variable values. \n
-        At each time iteration, the ``Solver`` appends every time variables' values to the relative list in the
-        dictionary.
+        At each time iteration, the :py:class:`Solver <gearpy.solver.Solver>` appends every time variables' values to
+        the relative list in the dictionary.
 
         Returns
         -------
-        dict
-            Time variables of the gear.
+        :py:class:`dict`
+            Time variables of the worm wheel.
+
+        .. admonition:: See Also
+           :class: seealso
 
-        See Also
-        --------
-        :py:meth:`update_time_variables`
+           :py:meth:`update_time_variables`
         """
         return super().time_variables
 
     def update_time_variables(self) -> None:
-        """Updates ``time_variables`` dictionary by appending the last value of each time variable (key of the
+        """It updates :py:attr:`time_variables` dictionary by appending the last value of each time variable (key of the
         dictionary) to corresponding list (value of the dictionary).
-
-        See Also
-        --------
-        :py:attr:`time_variables`
         """
         super().update_time_variables()
-        if self.tangential_force_is_computable:
-            self.time_variables['tangential force'].append(self.tangential_force)
-
-            if self.bending_stress_is_computable:
-                self.time_variables['bending stress'].append(self.bending_stress)
-
-                if self.contact_stress_is_computable:
-                    self.time_variables['contact stress'].append(self.contact_stress)
```

### Comparing `gearpy-0.6.0/gearpy/mechanical_objects/worm_wheel.py` & `gearpy-0.7.0/gearpy/mechanical_objects/worm_gear.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,859 +1,763 @@
 from gearpy.units import AngularPosition, AngularSpeed, AngularAcceleration, Angle, Force, InertiaMoment, Length, \
-                         Stress, Time, Torque, UnitBase
-from math import pi
-from .mechanical_object_base import RotatingObject, Role, WORM_GEAR_AND_WHEEL_AVAILABLE_PRESSURE_ANGLES, \
-                                    worm_gear_and_wheel_maximum_helix_angle_function, worm_wheel_lewis_factor_function
+                         Time, Torque, UnitBase
+from inspect import signature
 from .mating_roles import MatingMaster, MatingSlave
-from .helical_gear import HelicalGear
+from .mechanical_object_base import RotatingObject, Role, WORM_GEAR_AND_WHEEL_AVAILABLE_PRESSURE_ANGLES, \
+                                    worm_gear_and_wheel_maximum_helix_angle_function
 from typing import Callable, Dict, List, Union, Optional
 
 
-class WormWheel(HelicalGear):
-    r"""``gearpy.mechanical_objects.worm_wheel.WormWheel`` object.
+class WormGear(RotatingObject):
+    r""":py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>` object.
 
     Attributes
     ----------
-    :py:attr:`name` : str
-        Name of the worm wheel.
-    :py:attr:`n_teeth` : int
-        Number of gear teeth.
-    :py:attr:`inertia_moment` : InertiaMoment
+    :py:attr:`name` : :py:class:`str`
+        Name of the worm gear.
+    :py:attr:`n_starts` : :py:class:`int`
+        Number of starts, which refers to the number of independent threads running around the length of the thread.
+    :py:attr:`inertia_moment` : :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`
         Moment of inertia of the gear.
-    :py:attr:`helix_angle` : Angle
-        Helix angle of the worm wheel.
-    :py:attr:`pressure_angle` : Angle
-        Pressure angle of the worm wheel.
-    :py:attr:`module` : Length
-        Unit of the gear teeth size.
-    :py:attr:`reference_diameter` : Length
+    :py:attr:`helix_angle` : :py:class:`Angle <gearpy.units.units.Angle>`
+        Helix angle of the worm gear.
+    :py:attr:`pressure_angle` : :py:class:`Angle <gearpy.units.units.Angle>`
+        Pressure angle of the worm gear.
+    :py:attr:`reference_diameter` : :py:class:`Length <gearpy.units.units.Length>`
         Reference diameter of the gear.
-    :py:attr:`face_width` : Length
-        Face width of the gear.
-    :py:attr:`lewis_factor` : float
-        Factor used to compute stresses on the gear tooth.
-    :py:attr:`driven_by` : RotatingObject
-        Rotating object that drives the gear, for example a motor, a flywheel or another gear.
-    :py:attr:`drives` : RotatingObject
-        Rotating object driven by the gear, it can be a flywheel or another gear.
-    :py:attr:`master_gear_ratio` : float
+    :py:attr:`self_locking` : :py:class:`bool`
+        Whether the :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>` cannot be moved by the mating
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`.
+    :py:attr:`driven_by` : :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
+        Rotating object that drives the gear, for example a
+        :py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>`, a
+        :py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` or another gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`).
+    :py:attr:`drives` : :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
+        Rotating object driven by the gear, it can be a
+        :py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` or another gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`).
+    :py:attr:`master_gear_ratio` : :py:class:`float`
         Gear ratio of the mating between the gear and its driving gear.
-    :py:attr:`master_gear_efficiency` : float or int
+    :py:attr:`master_gear_efficiency` : :py:class:`float` or :py:class:`int`
         Efficiency of the gear mating between the gear and its driving gear.
-    :py:attr:`mating_role`: Role
+    :py:attr:`mating_role`: :py:class:`Role <gearpy.mechanical_objects.mechanical_object_base.Role>`
         The role of the gear in the gear mating.
-    :py:attr:`angular_position` : AngularPosition
+    :py:attr:`angular_position` : :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`
         Angular position of the gear.
-    :py:attr:`angular_speed` : AngularSpeed
+    :py:attr:`angular_speed` : :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`
         Angular speed of the gear.
-    :py:attr:`angular_acceleration` : AngularAcceleration
+    :py:attr:`angular_acceleration` : :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`
         Angular acceleration of the gear.
-    :py:attr:`torque` : Torque
+    :py:attr:`torque` : :py:class:`Torque <gearpy.units.units.Torque>`
         Net torque applied on the gear.
-    :py:attr:`driving_torque` : Torque
+    :py:attr:`driving_torque` : :py:class:`Torque <gearpy.units.units.Torque>`
         Driving torque applied on the gear by its driving gear.
-    :py:attr:`load_torque` : Torque
+    :py:attr:`load_torque` : :py:class:`Torque <gearpy.units.units.Torque>`
         Load torque applied on the gear by its driven gear or an external load.
-    :py:attr:`tangential_force` : Force
-        Tangential force applied on the gear teeth by the mating gear.
-    :py:attr:`tangential_force_is_computable` : bool
-        Whether is possible to compute the tangential force on the gear teeth.
-    :py:attr:`bending_stress` : Stress
-        Bending stress applied on the gear teeth by the mating gear.
-    :py:attr:`bending_stress_is_computable` : bool
-        Whether is possible to compute the bending stress on the gear teeth.
-    :py:attr:`time_variables` : dict
+    :py:attr:`tangential_force` : :py:class:`Force <gearpy.units.units.Force>`
+        Tangential force applied on the gear threads by the mating gear.
+    :py:attr:`tangential_force_is_computable` : :py:class:`bool`
+        Whether is possible to compute the :py:attr:`tangential_force` on the gear threads.
+    :py:attr:`time_variables` : :py:class:`dict`
         Time variables of the gear.
 
     Methods
     -------
     :py:meth:`compute_tangential_force`
-        Computes the tangential force applied on the gear teeth by the mating gear.
-    :py:meth:`compute_bending_stress`
-        Computes the bending stress applied on the gear teeth by the mating gear.
+        It computes the :py:attr:`tangential_force` applied on the gear threads by the mating gear.
     :py:meth:`external_torque`
         Custom function to compute the external torque applied on the gear.
     :py:meth:`update_time_variables`
-        Updates ``time_variables`` dictionary by appending the last value of each time variable to corresponding list.
+        It updates :py:attr:`time_variables` dictionary by appending the last value of each time variable to
+        corresponding list.
     """
 
     def __init__(self,
                  name: str,
-                 n_teeth: int,
+                 n_starts: int,
                  inertia_moment: InertiaMoment,
                  helix_angle: Angle,
                  pressure_angle: Angle,
-                 module: Optional[Length] = None,
-                 face_width: Optional[Length] = None):
+                 reference_diameter: Optional[Length] = None):
         super().__init__(name = name,
-                         n_teeth = n_teeth,
-                         module = module,
-                         face_width = face_width,
-                         inertia_moment = inertia_moment,
-                         helix_angle = helix_angle,
-                         elastic_modulus = None)
+                         inertia_moment = inertia_moment)
+
+        if not isinstance(n_starts, int):
+            raise TypeError("Parameter 'n_starts' must be an integer.")
+
+        if n_starts < 1:
+            raise ValueError("Parameter 'n_starts' must be equal to or greater than one.")
+
+        if not isinstance(helix_angle, Angle):
+            raise TypeError(f"Parameter 'helix_angle' must be an instance of {Angle.__name__!r}.")
 
         if not isinstance(pressure_angle, Angle):
             raise TypeError(f"Parameter 'pressure_angle' must be an instance of {Angle.__name__!r}.")
 
         if pressure_angle not in WORM_GEAR_AND_WHEEL_AVAILABLE_PRESSURE_ANGLES:
             raise ValueError(f"Value {pressure_angle!r} for parameter 'pressure_angle' not available. "
                              f"Available pressure angles are: {WORM_GEAR_AND_WHEEL_AVAILABLE_PRESSURE_ANGLES}")
 
         maximum_helix_angle = worm_gear_and_wheel_maximum_helix_angle_function(pressure_angle = pressure_angle)
         if helix_angle > maximum_helix_angle:
             raise ValueError(f"Parameter 'helix_angle' too high. For a {pressure_angle} 'pressure_angle', "
                              f"the maximum 'helix_angle' is {maximum_helix_angle}.")
 
+        if reference_diameter is not None:
+            if not isinstance(reference_diameter, Length):
+                raise TypeError(f"Parameter 'reference_diameter' must be an instance of {Length.__name__!r}.")
+
+        self.__n_starts = n_starts
         self.__helix_angle = helix_angle
         self.__pressure_angle = pressure_angle
+        self.__reference_diameter = reference_diameter
+        self.__self_locking = None
+        self.__driven_by = None
+        self.__drives = None
+        self.__master_gear_ratio = None
+        self.__master_gear_efficiency = 1
+        self.__mating_role = None
+        self.__external_torque = None
 
         if self.tangential_force_is_computable:
+            self.__tangential_force = None
             self.time_variables['tangential force'] = []
 
-            if self.bending_stress_is_computable:
-                self.time_variables['bending stress'] = []
-                self.__lewis_factor = worm_wheel_lewis_factor_function(pressure_angle = pressure_angle)
-
     @property
     def name(self) -> str:
-        """Name of the worm wheel. It must be a non-empty string. \n
+        """Name of the worm gear. It must be a non-empty :py:class:`str`. \n
         It must be a unique name, not shared by other elements in the powertrain elements. \n
-        Once set at the worm wheel instantiation, it cannot be changed afterward.
+        Once set at the worm gear instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        str
-            Name of the worm wheel.
+        :py:class:`str`
+            Name of the worm gear.
+
+        .. admonition:: Raises
+           :class: warning
 
-        Raises
-        ------
-        TypeError
-            If ``name`` is not a string.
-        ValueError
-            If ``name`` is an empty string.
+           ``TypeError``
+               If :py:attr:`name` is not a :py:class:`str`.
+           ``ValueError``
+               If :py:attr:`name` is an empty :py:class:`str`.
         """
         return super().name
 
     @property
-    def n_teeth(self) -> int:
-        """Number of gear teeth. It must be a positive integer. \n
-        Once set at the worm wheel instantiation, it cannot be changed afterward.
+    def n_starts(self) -> int:
+        """Number of starts, which refers to the number of independent threads running around the length of the thread.
+        It must be a positive :py:class:`int` equal to or greater than ``1``. \n
+        Once set at the worm gear instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        int
-            Number of gear teeth.
+        :py:class:`int`
+            Number of starts, which refers to the number of independent threads running around the length of the thread.
 
-        Raises
-        ------
-        TypeError
-            If ``n_teeth`` is not an integer.
-        ValueError
-            If ``n_teeth`` is less than the minimum number of teeth, based on Lewis Factor table.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`n_starts` is not an :py:class:`int`.
+           ``ValueError``
+               If :py:attr:`n_starts` is lower than ``1``.
         """
-        return super().n_teeth
+        return self.__n_starts
 
     @property
     def inertia_moment(self) -> InertiaMoment:
-        """Moment of inertia of the gear. It must be an instance of ``InertiaMoment``. \n
-        Once set at the worm wheel instantiation, it cannot be changed afterward.
+        """Moment of inertia of the gear. It must be an instance of
+        :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`. \n
+        Once set at the worm gear instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        InertiaMoment
+        :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`
             Moment of inertia of the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``inertia_moment`` is not an instance of ``InertiaMoment``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.InertiaMoment`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`inertia_moment` is not an instance of
+               :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`.
         """
         return super().inertia_moment
 
     @property
     def helix_angle(self) -> Angle:
-        """Helix angle of the worm wheel. It must be an instance of ``Angle``. \n
-        The maximum allowable value of helix angle depends on the pressure angle. \n
+        """Helix angle of the worm gear. It must be an instance of :py:class:`Angle <gearpy.units.units.Angle>`. \n
+        The maximum allowable value of helix angle depends on the :py:attr:`pressure_angle`. \n
         Once set at the worm gear instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        Angle
-            The helix angle of the worm wheel.
+        :py:class:`Angle <gearpy.units.units.Angle>`
+            The helix angle of the worm gear.
 
-        Raises
-        ------
-        TypeError
-            If ``helix_angle`` is not an instance of ``Angle``.
-        ValueError
-            If ``helix_angle`` is greater than the maximum allowable helix angle, depending on ``pressure_angle`` value.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Angle`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`helix_angle` is not an instance of :py:class:`Angle <gearpy.units.units.Angle>`.
+           ``ValueError``
+               If :py:attr:`helix_angle` is greater than the maximum allowable helix angle, depending on
+               :py:attr:`pressure_angle` value.
         """
         return self.__helix_angle
 
     @property
     def pressure_angle(self) -> Angle:
-        """Pressure angle of the worm wheel. It must be an instance of ``Angle`` and its value must be one of: 14.5 deg,
-        20 deg, 25 deg or 30 deg. \n
-        Once set at the worm wheel instantiation, it cannot be changed afterward.
+        """Pressure angle of the worm gear. It must be an instance of :py:class:`Angle <gearpy.units.units.Angle>` and
+        its value must be one of: 14.5 deg, 20 deg, 25 deg or 30 deg. \n
+        Once set at the worm gear instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        Angle
-            The pressure angle of the worm wheel.
+        :py:class:`Angle <gearpy.units.units.Angle>`
+            The pressure angle of the worm gear.
 
-        Raises
-        ------
-        TypeError
-            If ``pressure_angle`` is not an instance of ``Angle``.
-        ValueError
-            If ``pressure_angle`` value is not among available ones: 14.5 deg, 20 deg, 25 deg or 30 deg.
+        .. admonition:: Raises
+           :class: warning
 
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Angle`
+           ``TypeError``
+               If :py:attr:`pressure_angle` is not an instance of :py:class:`Angle <gearpy.units.units.Angle>`.
+           ``ValueError``
+               If :py:attr:`pressure_angle` value is not among available ones: 14.5 deg, 20 deg, 25 deg or 30 deg.
         """
         return self.__pressure_angle
 
     @property
-    def module(self) -> Optional[Length]:
-        """Unit of the gear teeth size. It must be an instance of ``Length``. \n
-        Once set at the worm wheel instantiation, it cannot be changed afterward.
-
-        Returns
-        -------
-        Length
-            Unit of the gear teeth size.
-
-        Raises
-        ------
-        TypeError
-            If ``module`` is not an instance of ``Length``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Length`
-        """
-        return super().module
-
-    @property
     def reference_diameter(self) -> Optional[Length]:
-        """Reference diameter of the gear. It must be an instance of ``Length``. \n
-        It is computed as the product of ``n_teeth`` times ``module`` at the worm wheel instantiation and it cannot be
-        changed afterward.
+        """Reference diameter of the gear. It must be an instance of :py:class:`Length <gearpy.units.units.Length>`. \n
+        Once set at the worm gear instantiation, it cannot be changed afterward.
 
         Returns
         -------
-        Length
+        :py:class:`Length <gearpy.units.units.Length>`
             Reference diameter of the gear.
 
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Length`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`reference_diameter` is not an instance of :py:class:`Length <gearpy.units.units.Length>`.
         """
-        return super().reference_diameter
+        return self.__reference_diameter
 
     @property
-    def face_width(self) -> Optional[Length]:
-        """Face width of the gear. It must be an instance of ``Length``.
+    def self_locking(self) -> bool:
+        """Whether the :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>` cannot be moved by the mating
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`. \n
+        The gear mating can be self-locking if the amount of friction is high enough with respect to the gear pressure
+        and helix angles. \n
+        If the mating is self-locking, then the :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`
+        cannot be moved by the mating :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`. \n
+        To set this property use :py:func:`add_worm_gear_mating <gearpy.utils.relations.add_worm_gear_mating>`.
 
         Returns
         -------
-        Length
-            Face width of the gear.
-
-        Raises
-        ------
-        TypeError
-            If ``face_width`` is not an instance of ``Length``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Length`
+        :py:class:`bool`
+            Whether the :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>` cannot be moved by the
+            mating :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`.
         """
-        return super().face_width
-
-    @property
-    def lewis_factor(self) -> Optional[float]:
-        """Factor used to compute stresses on the gear tooth. \n
-        It is a tabular value that in general depends on the pressure angle.
+        return self.__self_locking
 
-        Returns
-        -------
-        float
-            Factor used to compute stresses on the gear tooth.
+    @self_locking.setter
+    def self_locking(self, self_locking: bool):
+        if not isinstance(self_locking, bool):
+            raise TypeError("Parameter 'self_locking' must be a boolean.")
 
-        See Also
-        --------
-        :py:attr:`pressure_angle`
-        """
-        return self.__lewis_factor
+        self.__self_locking = self_locking
 
     @property
     def driven_by(self) -> RotatingObject:
-        """Rotating object that drives the gear, for example a motor, a flywheel, another gear or a worm gear. It must
-        be a ``RotatingObject``.
+        """Rotating object that drives the gear, for example a
+        :py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>`, a
+        :py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` or another gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`). It must be a
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`. \n
+        To set this property use :py:func:`add_worm_gear_mating <gearpy.utils.relations.add_worm_gear_mating>` or
+        :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
-        RotatingObject
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
             Master rotating object that drives the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``driven_by`` is not an instance of ``RotatingObject``.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_worm_gear_mating`
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`driven_by` is not an instance of
+               :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`.
         """
-        return super().driven_by
+        return self.__driven_by
 
     @driven_by.setter
     def driven_by(self, driven_by: RotatingObject):
-        super(WormWheel, type(self)).driven_by.fset(self, driven_by)
+        if not isinstance(driven_by, RotatingObject):
+            raise TypeError(f"Parameter 'driven_by' must be an instance of {RotatingObject.__name__!r}.")
+
+        self.__driven_by = driven_by
 
     @property
     def drives(self) -> RotatingObject:
-        """Rotating object driven by the gear, it can be a flywheel, another gear or a worm gear. It must be a
-        ``RotatingObject``.
+        """Rotating object driven by the gear, it can be a
+        :py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` or another gear
+        (:py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>`,
+        :py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>`,
+        :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>`,
+        :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`). It must be a
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`. \n
+        To set this property use :py:func:`add_worm_gear_mating <gearpy.utils.relations.add_worm_gear_mating>` or
+        :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
-        RotatingObject
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
             Rotating object driven by the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``drives`` is not an instance of ``RotatingObject``.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_worm_gear_mating`
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`drives` is not an instance of
+               :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`.
         """
-        return super().drives
+        return self.__drives
 
     @drives.setter
     def drives(self, drives: RotatingObject):
-        super(WormWheel, type(self)).drives.fset(self, drives)
+        if not isinstance(drives, RotatingObject):
+            raise TypeError(f"Parameter 'drives' must be an instance of {RotatingObject.__name__!r}.")
+
+        self.__drives = drives
 
     @property
     def master_gear_ratio(self) -> float:
-        """Gear ratio of the mating between the gear and its driving gear. It must be a positive a float. \n
-        If the wheel gear is fixed to another driving ``RotatingObject``, then the ratio is ``1``, otherwise it is
-        defined as the ratio between the worm wheel number of teeth ``n_teeth`` and the driving worm gear number of
-        starts ``n_starts``. \n
-        To set this property use :py:func:`gearpy.utils.relations.add_worm_gear_mating` or
-        :py:func:`gearpy.utils.relations.add_fixed_joint`.
+        """Gear ratio of the mating between the gear and its driving gear. It must be a positive a :py:class:`float`. \n
+        If the worm gear is fixed to another driving
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`, then the ratio is
+        ``1``, otherwise it is defined as the ratio between the worm gear number of starts :py:attr:`n_starts` and the
+        driving wheel gear number of teeth
+        :py:attr:`WormWheel.n_teeth <gearpy.mechanical_objects.worm_wheel.WormWheel.n_teeth>`. \n
+        To set this property use :py:func:`add_worm_gear_mating <gearpy.utils.relations.add_worm_gear_mating>` or
+        :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
-        float
+        :py:class:`float`
             Gear ratio of the mating between the gear and its driving gear.
 
-        Raises
-        ------
-        TypeError
-            If ``master_gear_ratio`` is not a float.
-        ValueError
-            If ``master_gear_ratio`` is negative or null.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_worm_gear_mating`
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`master_gear_ratio` is not a :py:class:`float`.
+           ``ValueError``
+               If :py:attr:`master_gear_ratio` is negative or null.
         """
-        return super().master_gear_ratio
+        return self.__master_gear_ratio
 
     @master_gear_ratio.setter
     def master_gear_ratio(self, master_gear_ratio: float):
-        super(WormWheel, type(self)).master_gear_ratio.fset(self, master_gear_ratio)
+        if not isinstance(master_gear_ratio, float):
+            raise TypeError("Parameter 'master_gear_ratio' must be a float.")
+
+        if master_gear_ratio <= 0:
+            raise ValueError("Parameter 'master_gear_ratio' must be positive.")
+
+        self.__master_gear_ratio = master_gear_ratio
 
     @property
     def master_gear_efficiency(self) -> Union[float, int]:
-        """Efficiency of the gear mating between the gear and its driving gear. It must be a float or an integer within
-        ``0`` and ``1``. \n
-        To set this property use :py:func:`gearpy.utils.relations.add_worm_gear_mating` or
-        :py:func:`gearpy.utils.relations.add_fixed_joint`.
+        """Efficiency of the gear mating between the gear and its driving gear. It must be a :py:class:`float` or an
+        :py:class:`int` within ``0`` and ``1``. \n
+        To set this property use :py:func:`add_worm_gear_mating <gearpy.utils.relations.add_worm_gear_mating>` or
+        :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Efficiency of the gear mating between the gear and its driving gear.
 
-        Raises
-        ------
-        TypeError
-            If ``master_gear_efficiency`` is not a float or an integer.
-        ValueError
-            If ``master_gear_efficiency`` is not within ``0`` and ``1``.
-
-        See Also
-        --------
-        :py:func:`gearpy.utils.relations.add_worm_gear_mating`
-        :py:func:`gearpy.utils.relations.add_fixed_joint`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`master_gear_efficiency` is not a :py:class:`float` or an :py:class:`int`.
+           ``ValueError``
+               If :py:attr:`master_gear_efficiency` is not within ``0`` and ``1``.
         """
-        return super().master_gear_efficiency
+        return self.__master_gear_efficiency
 
     @master_gear_efficiency.setter
     def master_gear_efficiency(self, master_gear_efficiency: Union[float, int]):
-        super(WormWheel, type(self)).master_gear_efficiency.fset(self, master_gear_efficiency)
+        if not isinstance(master_gear_efficiency, float) and not isinstance(master_gear_efficiency, int):
+            raise TypeError("Parameter 'master_gear_efficiency' must be a float or an integer.")
+
+        if master_gear_efficiency > 1 or master_gear_efficiency < 0:
+            raise ValueError("Parameter 'master_gear_efficiency' must be within 0 and 1.")
+
+        self.__master_gear_efficiency = master_gear_efficiency
 
     @property
     def mating_role(self) -> Role:
-        """Role of the gear in the gear mating. To set this parameter use ``add_worm_gear_mating``. \n
-        If the gear drives the mate one, then it is the "master" gear and its role is ``MatingMaster``, otherwise it is
-        the "slave" one and its role is ``MatingSlave``.
+        """Role of the gear in the gear mating. \n
+        If the gear drives the mate one, then it is the "master" gear and its role is
+        :py:class:`MatingMaster <gearpy.mechanical_objects.mating_roles.MatingMaster>`, otherwise it is
+        the "slave" one and its role is :py:class:`MatingSlave <gearpy.mechanical_objects.mating_roles.MatingSlave>`. \n
+        To set this parameter use :py:func:`add_worm_gear_mating <gearpy.utils.relations.add_worm_gear_mating>`.
 
         Returns
         -------
-        Role
+        :py:class:`Role <gearpy.mechanical_objects.mechanical_object_base.Role>`
             The role of the gear in the gear mating.
 
-        Raises
-        ------
-        ValueError
-            If ``mating_role`` is not a subclass of ``Role``.
+        .. admonition:: Raises
+           :class: warning
+
+           ``ValueError``
+               If :py:attr:`mating_role` is not a subclass of
+               :py:class:`Role <gearpy.mechanical_objects.mechanical_object_base.Role>`.
         """
-        return super().mating_role
+        return self.__mating_role
 
     @mating_role.setter
     def mating_role(self, mating_role: Role):
-        super(WormWheel, type(self)).mating_role.fset(self, mating_role)
+        if hasattr(mating_role, '__name__'):
+            if not issubclass(mating_role, Role):
+                raise TypeError(f"Parameter 'mating_role' must be a subclass of {Role.__name__!r}.")
+        else:
+            raise TypeError(f"Parameter 'mating_role' must be a subclass of {Role.__name__!r}.")
+
+        self.__mating_role = mating_role
 
     @property
     def angular_position(self) -> AngularPosition:
-        """Angular position of the gear. It must be an instance of ``AngularPosition``.
+        """Angular position of the gear. It must be an instance of
+        :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`.
 
         Returns
         -------
-        AngularPosition
+        :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`
             Angular position of the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``angular_position`` is not an instance of ``AngularPosition``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularPosition`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`angular_position` is not an instance of
+               :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`.
         """
         return super().angular_position
 
     @angular_position.setter
     def angular_position(self, angular_position: AngularPosition):
-        super(WormWheel, type(self)).angular_position.fset(self, angular_position)
+        super(WormGear, type(self)).angular_position.fset(self, angular_position)
 
     @property
     def angular_speed(self) -> AngularSpeed:
-        """Angular speed of the gear. It must be an instance of ``AngularSpeed``.
+        """Angular speed of the gear. It must be an instance of
+        :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`.
 
         Returns
         -------
-        AngularSpeed
+        :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`
             Angular speed of the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``angular_speed`` is not an instance of ``AngularSpeed``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularSpeed`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`angular_speed` is not an instance of
+               :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`.
         """
         return super().angular_speed
 
     @angular_speed.setter
     def angular_speed(self, angular_speed: AngularSpeed):
-        super(WormWheel, type(self)).angular_speed.fset(self, angular_speed)
+        super(WormGear, type(self)).angular_speed.fset(self, angular_speed)
 
     @property
     def angular_acceleration(self) -> AngularAcceleration:
-        """Angular acceleration of the gear. It must be an instance of ``AngularAcceleration``.
+        """Angular acceleration of the gear. It must be an instance of
+        :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`.
 
         Returns
         -------
-        AngularAcceleration
+        :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`
             Angular acceleration of the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``angular_acceleration`` is not an instance of ``AngularAcceleration``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularAcceleration`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`angular_acceleration` is not an instance of
+               :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`.
         """
         return super().angular_acceleration
 
     @angular_acceleration.setter
     def angular_acceleration(self, angular_acceleration: AngularAcceleration):
-        super(WormWheel, type(self)).angular_acceleration.fset(self, angular_acceleration)
+        super(WormGear, type(self)).angular_acceleration.fset(self, angular_acceleration)
 
     @property
     def torque(self) -> Torque:
-        """Net torque applied on the gear. It must be an instance of ``Torque``. \n
-        It is computed as the difference between ``driving_torque`` and ``load_torque``.
+        """Net torque applied on the gear. It must be an instance of :py:class:`Torque <gearpy.units.units.Torque>`. \n
+        It is computed as the difference between :py:attr:`driving_torque` and :py:attr:`load_torque`.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Net torque applied on the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``torque`` is not an instance of ``Torque``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Torque`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`torque` is not an instance of :py:class:`Torque <gearpy.units.units.Torque>`.
         """
         return super().torque
 
     @torque.setter
     def torque(self, torque: Torque):
-        super(WormWheel, type(self)).torque.fset(self, torque)
+        super(WormGear, type(self)).torque.fset(self, torque)
 
     @property
     def driving_torque(self) -> Torque:
-        """Driving torque applied on the gear by its driving gear. It must be an instance of ``Torque``.
+        """Driving torque applied on the gear by its driving gear. It must be an instance of
+        :py:class:`Torque <gearpy.units.units.Torque>`.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Driving torque applied on the gear by its driving gear.
 
-        Raises
-        ------
-        TypeError
-            If ``driving_torque`` is not an instance of ``Torque``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Torque`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`driving_torque` is not an instance of :py:class:`Torque <gearpy.units.units.Torque>`.
         """
         return super().driving_torque
 
     @driving_torque.setter
     def driving_torque(self, driving_torque: Torque):
-        super(WormWheel, type(self)).driving_torque.fset(self, driving_torque)
+        super(WormGear, type(self)).driving_torque.fset(self, driving_torque)
 
     @property
     def load_torque(self) -> Torque:
-        """Load torque applied on the gear by its driven gear or an external load. It must be an instance of ``Torque``.
+        """Load torque applied on the gear by its driven gear or an external load. It must be an instance of
+        :py:class:`Torque <gearpy.units.units.Torque>`.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Load torque applied on the gear by its driven gear or an external load.
 
-        Raises
-        ------
-        TypeError
-            If ``load_torque`` is not an instance of ``Torque``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Torque`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`load_torque` is not an instance of :py:class:`Torque <gearpy.units.units.Torque>`.
         """
         return super().load_torque
 
     @load_torque.setter
     def load_torque(self, load_torque: Torque):
-        super(WormWheel, type(self)).load_torque.fset(self, load_torque)
+        super(WormGear, type(self)).load_torque.fset(self, load_torque)
 
     @property
     def tangential_force(self) -> Force:
-        """Tangential force applied on the gear teeth by the mating gear. It must be an instance of ``Force``.
+        """Tangential force applied on the gear threads by the mating gear. It must be an instance of
+        :py:class:`Force <gearpy.units.units.Force>`.
 
         Returns
         -------
-        Force
-            Tangential force applied on the gear teeth by the mating gear.
+        :py:class:`Force <gearpy.units.units.Force>`
+            Tangential force applied on the gear threads by the mating gear.
+
+        .. admonition:: Raises
+           :class: warning
 
-        Raises
-        ------
-        TypeError
-            If ``tangential_force`` is not an instance of ``Force``.
+           ``TypeError``
+               If :py:attr:`tangential_force` is not an instance of :py:class:`Force <gearpy.units.units.Force>`.
 
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Force`
-        :py:meth:`compute_tangential_force`
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`compute_tangential_force`
         """
-        return super().tangential_force
+        return self.__tangential_force
 
     @tangential_force.setter
     def tangential_force(self, tangential_force: Force):
-        super(WormWheel, type(self)).tangential_force.fset(self, tangential_force)
+        if not isinstance(tangential_force, Force):
+            raise TypeError(f"Parameter 'tangential_force' must be an instance of {Force.__name__!r}.")
+
+        self.__tangential_force = tangential_force
 
-    def compute_tangential_force(self):
-        """Computes the tangential force applied on the gear teeth by the mating gear. \n
+    def compute_tangential_force(self) -> None:
+        """It computes the :py:attr:`tangential_force` applied on the gear threads by the mating gear. \n
         Considering a gear mating:
 
-        - if the gear is the master one, then it takes into account the ``load_torque`` for the computation,
-        - if the gear is the slave one, then it take into account the ``driving_torque`` for the computation.
+        - if the gear is the master one, then it takes into account the :py:attr:`load_torque` for the computation,
+        - if the gear is the slave one, then it take into account the :py:attr:`driving_torque` for the computation.
 
         The tangential force is computed dividing the just described reference torque by the reference radius (half of
-        the reference diameter).
+        the :py:attr:`reference_diameter`).
+
+        .. admonition:: Raises
+           :class: warning
 
-        Raises
-        ------
-        ValueError
-            If a gear mating between two gears has not been set.
-
-        See Also
-        --------
-        :py:attr:`tangential_force`
+           ``ValueError``
+               If a gear mating between two gears has not been set.
         """
         if self.mating_role == MatingMaster:
-            self.tangential_force = abs(self.load_torque)/(self.reference_diameter/2)
+            self.tangential_force = abs(self.load_torque)/(self.reference_diameter/2)*self.helix_angle.tan()
         elif self.mating_role == MatingSlave:
-            self.tangential_force = abs(self.driving_torque)/(self.reference_diameter/2)
+            self.tangential_force = abs(self.driving_torque)/(self.reference_diameter/2)*self.helix_angle.tan()
         else:
             raise ValueError("Gear mating not defined. "
                              "Use 'gearpy.utils.add_worm_gear_mating' to set up a mating between two gears.")
 
     @property
     def tangential_force_is_computable(self) -> bool:
-        """Whether is possible to compute the tangential force on the gear teeth. The tangential force computation
-        depends on the value of ``module``, so if this optional parameter has been set at worm wheel instantiation,
-        then it is possible to compute the tangential force and this property is ``True``, otherwise is ``False``.
-
-        Returns
-        -------
-        bool
-            Whether is possible to compute the tangential force on the gear teeth.
-
-        See Also
-        --------
-        :py:attr:`module`
-        :py:attr:`tangential_force`
-        :py:meth:`compute_tangential_force`
-        """
-        return super().tangential_force_is_computable
-
-    @property
-    def bending_stress(self) -> Stress:
-        """Bending stress applied on the gear teeth by the mating gear. It must be an instance of ``Stress``.
+        """Whether is possible to compute the :py:attr:`tangential_force` on the gear threads. \n
+        The tangential force computation depends on the value of :py:attr:`reference_diameter`, so if this optional
+        parameter has been set at worm gear instantiation, then it is possible to compute the tangential force and this
+        property is ``True``, otherwise is ``False``.
 
         Returns
         -------
-        Stress
-            Bending stress applied on the gear teeth by the mating gear.
-
-        Raises
-        ------
-        TypeError
-            If ``bending_stress`` is not an instance of ``Stress``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Stress`
-        :py:meth:`compute_bending_stress`
-        """
-        return super().bending_stress
-
-    @bending_stress.setter
-    def bending_stress(self, bending_stress: Stress):
-        super(WormWheel, type(self)).bending_stress.fset(self, bending_stress)
-
-    def compute_bending_stress(self):
-        r"""Computes the bending stress applied on the gear teeth by the mating gear.
-
-        Notes
-        -----
-        The bending stress computation is based on the following assumptions:
-
-        - the tooth is stressed by the overall force acting on the tip of the tooth itself,
-        - the most unfavorable situation is considered in the calculation, as if there is only one pair of teeth in
-          contact within the contact segment,
-        - the component of the overall force that determines the bending on the tooth is the only one considered and,
-          for simplicity, is taken as having a value equal to the tangential force on the reference diameter,
-        - the radial component of the overall force that causes a compressive stress on the tooth is neglected.
-
-        The bending stress is computed with the following formula:
-
-        .. math::
-            \sigma_b = \frac{F_t}{p_n \, b_{eff} \, Y_{LW}}
-
-        where:
-
-        - :math:`F_t` is the tangential force applied on the tooth,
-        - :math:`p_n` is the normal pitch,
-        - :math:`b_{eff}` is the effective tooth face width,
-        - :math:`Y_{LW}` is the gear Lewis factor (``lewis_factor``).
+        :py:class:`bool`
+            Whether is possible to compute the tangential force on the gear threads.
 
-        The normal pitch can be computed with:
+        .. admonition:: See Also
+           :class: seealso
 
-        .. math::
-            p_n = \frac{\pi d_{wg} \sin \beta}{N}
-
-        where:
-
-        - :math:`d_{wg}` is the mating worm gear reference diameter,
-        - :math:`\beta` is the mating worm gear helix angle,
-        - :math:`N` is the worm wheel number of teeth (``n_teeth``).
-
-        The effective tooth face width `b_{eff}` is the minimum between the worm wheel face width (``face_width``) and
-        the mating worm gear reference diameter multiplied by 0.67.
-
-        See Also
-        --------
-        :py:attr:`bending_stress`
-        :py:attr:`tangential_force`
-        :py:attr:`module`
-        :py:attr:`face_width`
-        :py:attr:`lewis_factor`
-        """
-        if self.mating_role == MatingMaster:
-            normal_pitch = pi*self.drives.reference_diameter*self.drives.helix_angle.sin()/self.n_teeth
-            effective_face_width = min(self.face_width, 0.67*self.drives.reference_diameter)
-        elif self.mating_role == MatingSlave:
-            normal_pitch = pi*self.driven_by.reference_diameter*self.driven_by.helix_angle.sin()/self.n_teeth
-            effective_face_width = min(self.face_width, 0.67*self.driven_by.reference_diameter)
-        else:
-            raise ValueError("Gear mating not defined. "
-                             "Use 'gearpy.utils.add_worm_gear_mating' to set up a mating between two gears.")
-        self.bending_stress = self.tangential_force/(normal_pitch*effective_face_width)/self.lewis_factor
-
-    @property
-    def bending_stress_is_computable(self) -> bool:
-        """Whether is possible to compute the bending stress on the gear teeth. The bending stress computation depends
-        on the value of ``module`` and ``face_width`` and the ``reference_diameter`` of the mating ``WormGear``, so if
-        these optional parameters have been set at worm wheel and worm gear instantiations, then it is possible to
-        compute the bending stress and this property is ``True``, otherwise is ``False``.
-
-        Returns
-        -------
-        bool
-            Whether is possible to compute the bending stress on the gear teeth.
-
-        See Also
-        --------
-        :py:attr:`module`
-        :py:attr:`face_width`
-        :py:attr:`bending_stress`
-        :py:meth:`compute_bending_stress`
+           :py:meth:`compute_tangential_force`
         """
-        if self.mating_role == MatingMaster:
-            return super().bending_stress_is_computable and (self.drives.reference_diameter is not None)
-        if self.mating_role == MatingSlave:
-            return super().bending_stress_is_computable and (self.driven_by.reference_diameter is not None)
-        else:
-            return super().bending_stress_is_computable
+        return self.__reference_diameter is not None
 
     @property
     def external_torque(self) -> Callable[[AngularPosition, AngularSpeed, Time], Torque]:
         """Custom function to compute the external torque applied on the gear. It must be a function with parameters
-        ``angular_position``, ``angular_speed`` and ``time``. The function must return an instance of ``Torque``.
+        ``angular_position``, ``angular_speed`` and ``time``. The function must return an instance of
+        :py:class:`Torque <gearpy.units.units.Torque>`.
 
         Returns
         -------
-        Callable
+        :py:obj:`Callable <typing.Callable>`
             The function to compute the external torque applied on the gear.
 
-        Raises
-        ------
-        TypeError
-            If ``external_torque`` is not callable.
-        KeyError
-            If ``external_torque`` misses parameters ``angular_position``, ``angular_speed`` or ``time``.
-
-        Examples
-        --------
-        Constant torque, not dependent on ``angular_position``, ``angular_speed`` or ``time``.
-
-        >>> from gearpy.mechanical_objects import WormWheel
-        >>> from gearpy.units import InertiaMoment, Torque
-        >>> gear = WormWheel(name = 'gear', n_teeth = 10, inertia_moment = InertiaMoment(1, 'kgm^2'))
-        >>> gear.external_torque = lambda angular_position, angular_speed, time: Torque(5, 'Nm')
-
-        Torque dependent on ``angular_position`` and ``time``. \n
-        In this case the gear gets a periodic load, dependent on time, and an extra load dependent on its angular
-        position. The dependence by angular position may be used to model cases where cams are involved.
-
-        >>> import numpy as np
-        >>> from gearpy.units import AngularPosition, AngularSpeed, Time
-        >>> def custom_external_torque(angular_position: AngularPosition,
-        ...                            angular_speed: AngularSpeed,
-        ...                            time: Time):
-        ...     return Torque(value = angular_position.sin() +
-        ...                           np.cos(time.to('sec').value),
-        ...                   unit = 'Nm')
-        >>> gear.external_torque = custom_external_torque
-
-        Torque dependent on ``angular_position``, ``angular_speed`` and ``time``. \n
-        With respect ot the previous case, the gear gets an extra load dependent on its angular speed. The dependence by
-        angular speed may be used to model cases where air friction is not negligible.
-
-        >>> def complex_external_torque(angular_position: AngularPosition,
-        ...                             angular_speed: AngularSpeed,
-        ...                             time: Time):
-        ...     return Torque(value = angular_position.sin() +
-        ...                           0.001*(angular_speed.to('rad/s').value)**2 +
-        ...                           np.cos(time.to('sec').value),
-        ...                   unit = 'Nm')
-        >>> gear.external_torque = complex_external_torque
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:meth:`external_torque` is not callable.
+           ``KeyError``
+               If :py:meth:`external_torque` misses parameters ``angular_position``, ``angular_speed`` or ``time``.
+
+        .. admonition:: Examples
+           :class: important
+
+           Constant torque, not dependent on ``angular_position``, ``angular_speed`` or ``time``.
+
+           >>> from gearpy.mechanical_objects import WormGear
+           >>> from gearpy.units import InertiaMoment, Torque, Angle
+           >>> gear = WormGear(name = 'gear', n_starts = 1, inertia_moment = InertiaMoment(1, 'kgm^2'),
+           >>>                 pressure_angle = Angle(20, 'deg'), helix_angle = Angle(10, 'deg'))
+           >>> gear.external_torque = lambda angular_position, angular_speed, time: Torque(5, 'Nm')
+
+           Torque dependent on ``angular_position`` and ``time``. \n
+           In this case the gear gets a periodic load, dependent on time, and an extra load dependent on its angular
+           position. The dependence by angular position may be used to model cases where cams are involved.
+
+           >>> import numpy as np
+           >>> from gearpy.units import AngularPosition, AngularSpeed, Time
+           >>> def custom_external_torque(angular_position: AngularPosition,
+           ...                            angular_speed: AngularSpeed,
+           ...                            time: Time):
+           ...     return Torque(value = angular_position.sin() +
+           ...                           np.cos(time.to('sec').value),
+           ...                   unit = 'Nm')
+           >>> gear.external_torque = custom_external_torque
+
+           Torque dependent on ``angular_position``, ``angular_speed`` and ``time``. \n
+           With respect ot the previous case, the gear gets an extra load dependent on its angular speed. The dependence
+           by angular speed may be used to model cases where air friction is not negligible.
+
+           >>> def complex_external_torque(angular_position: AngularPosition,
+           ...                             angular_speed: AngularSpeed,
+           ...                             time: Time):
+           ...     return Torque(value = angular_position.sin() +
+           ...                           0.001*(angular_speed.to('rad/s').value)**2 +
+           ...                           np.cos(time.to('sec').value),
+           ...                   unit = 'Nm')
+           >>> gear.external_torque = complex_external_torque
         """
-        return super().external_torque
+        return self.__external_torque
 
     @external_torque.setter
     def external_torque(self, external_torque: Callable[[AngularPosition, AngularSpeed, Time], Torque]):
-        super(WormWheel, type(self)).external_torque.fset(self, external_torque)
+        if not isinstance(external_torque, Callable):
+            raise TypeError("Parameter 'external_torque' must be callable.")
+
+        sig = signature(external_torque)
+        for parameter in ['angular_position', 'angular_speed', 'time']:
+            if parameter not in sig.parameters.keys():
+                raise KeyError(f"Function 'external_torque' misses parameter {parameter!r}.")
+
+        self.__external_torque = external_torque
 
     @property
     def time_variables(self) -> Dict[str, List[UnitBase]]:
-        """Time variables of the worm wheel. Each time variable is stored as a dictionary key-value pair. The available
-        time variables are:
+        """Time variables of the gear. Each time variable is stored as a dictionary key-value pair. The available time
+        variables are:
 
-        - ``angular position``,
-        - ``angular speed``,
-        - ``angular acceleration``,
-        - ``torque``,
-        - ``driving torque``,
-        - ``load torque``,
-        - ``tangential force``,
-        - ``bending stress``.
+        - :py:attr:`angular_position`: ``'angular position'``,
+        - :py:attr:`angular_speed`: ``'angular speed'``,
+        - :py:attr:`angular_acceleration`: ``'angular acceleration'``,
+        - :py:attr:`torque`: ``'torque'``,
+        - :py:attr:`driving_torque`: ``'driving torque'``,
+        - :py:attr:`load_torque`: ``'load torque'``,
+        - :py:attr:`tangential_force`: ``'tangential force'``
 
-        ``tangential force`` and ``bending stress`` are listed among time variables only if they are computable indeed,
-        depending on which gear parameters are set at worm wheel instantiation. \n
+        ``'tangential force'`` is listed among time variables only if they are computable indeed, depending on which gear
+        parameters are set at gear instantiation; see :py:attr:`tangential_force_is_computable`. \n
         Corresponding values of the dictionary are lists of the respective time variable values. \n
-        At each time iteration, the ``Solver`` appends every time variables' values to the relative list in the
-        dictionary.
+        At each time iteration, the :py:class:`Solver <gearpy.solver.Solver>` appends every time variables' values to
+        the relative list in the dictionary.
 
         Returns
         -------
-        dict
-            Time variables of the worm wheel.
+        :py:class:`dict`
+            Time variables of the gear.
 
-        See Also
-        --------
-        :py:meth:`update_time_variables`
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:meth:`update_time_variables`
         """
         return super().time_variables
 
     def update_time_variables(self) -> None:
-        """Updates ``time_variables`` dictionary by appending the last value of each time variable (key of the
+        """It updates :py:attr:`time_variables` dictionary by appending the last value of each time variable (key of the
         dictionary) to corresponding list (value of the dictionary).
-
-        See Also
-        --------
-        :py:attr:`time_variables`
         """
         super().update_time_variables()
+        if self.tangential_force_is_computable:
+            self.time_variables['tangential force'].append(self.tangential_force)
```

### Comparing `gearpy-0.6.0/gearpy/motor_control/motor_control_base.py` & `gearpy-0.7.0/gearpy/motor_control/motor_control_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 from abc import ABC, abstractmethod
 from gearpy.mechanical_objects import MotorBase, RotatingObject
 from gearpy.powertrain import Powertrain
 from gearpy.motor_control.rules.rules_base import RuleBase
 
 
 class MotorControlBase(ABC):
+    """:py:class:`MotorControlBase <gearpy.motor_control.motor_control_base.MotorControlBase>` object. \n
+    Abstract base class for creating motor control objects.
+
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:class:`PWMControl <gearpy.motor_control.pwm_control.PWMControl>`
+    """
 
     @abstractmethod
     def __init__(self, powertrain: Powertrain):
         if not isinstance(powertrain, Powertrain):
             raise TypeError(f"Parameter 'powertrain' must be an instance of {Powertrain.__name__!r}.")
 
         if not powertrain.elements:
@@ -16,29 +24,18 @@
 
         if not isinstance(powertrain.elements[0], MotorBase):
             raise TypeError(f"First element in 'powertrain' must be an instance of {MotorBase.__name__!r}.")
 
         if not all([isinstance(item, RotatingObject) for item in powertrain.elements]):
             raise TypeError(f"All elements of 'powertrain' must be instances of {RotatingObject.__name__!r}.")
 
-        self.__powertrain = powertrain
-        self.__rules = []
-
     @property
     @abstractmethod
-    def powertrain(self) -> Powertrain:
-        return self.__powertrain
-
-    @property
-    @abstractmethod
-    def rules(self) -> list:
-        return self.__rules
+    def rules(self) -> list: ...
 
     @abstractmethod
     def add_rule(self, rule: RuleBase):
         if not isinstance(rule, RuleBase):
             raise TypeError(f"Parameter 'rule' must be an instance of {RuleBase.__name__!r}.")
 
-        self.__rules.append(rule)
-
     @abstractmethod
     def apply_rules(self): ...
```

### Comparing `gearpy-0.6.0/gearpy/motor_control/rules/reach_angular_position.py` & `gearpy-0.7.0/gearpy/motor_control/rules/reach_angular_position.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,51 +4,44 @@
 from gearpy.units import AngularPosition, Angle
 from gearpy.motor_control.rules.rules_base import RuleBase
 from typing import Union
 from .utils import _compute_static_error
 
 
 class ReachAngularPosition(RuleBase):
-    """gearpy.motor_control.rules.reach_angular_position.ReachAngularPosition object. \n
+    """:py:class:`ReachAngularPosition <gearpy.motor_control.rules.reach_angular_position.ReachAngularPosition>` object. \n
     It can be used to make the ``encoder``'s ``target`` reach a ``target_angular_position`` within a ``braking_angle``.
 
-    Attributes
-    ----------
-    :py:attr:`encoder` : AbsoluteRotaryEncoder
-        Sensor used to measure the ``angular_position`` of a ``RotatingObject``, which is compared to
-        ``target_angular_position``.
-    :py:attr:`powertrain` : Powertrain
-        Powertrain whose motor's ``pwm`` is controlled in order to reach a specific angular position.
-    :py:attr:`target_angular_position` : AngularPosition
-        Angular position to be reached by the ``encoder``'s target.
-    :py:attr:`braking_angle` : Angle
-        The angle within which the motor's ``pwm`` is controlled in order to brake and reach the
-        ``target_angular_position``.
-
     Methods
     -------
     :py:meth:`apply`
-        Computes the ``pwm`` to apply to the ``powertrain``'s motor in order to reach a ``target_angular_position`` by
-        the ``target`` rotating object of the ``encoder``, within a specific ``braking_angle``.
+        It computes the ``pwm`` to apply to the ``powertrain``'s motor in order to reach a ``target_angular_position``
+        by the ``target`` rotating object of the ``encoder``, within a specific ``braking_angle``.
+
+    .. admonition:: Raises
+       :class: warning
+
+       ``TypeError``
+           - If ``encoder`` is not an instance of
+             :py:class:`AbsoluteRotaryEncoder <gearpy.sensors.absolute_rotary_encoder.AbsoluteRotaryEncoder>`,
+           - if ``powertrain`` is not an instance of :py:class:`Powertrain <gearpy.powertrain.Powertrain>`,
+           - if the first element in ``powertrain`` is not an instance of
+             :py:class:`MotorBase <gearpy.mechanical_objects.mechanical_object_base.MotorBase>`,
+           - if an element of ``powertrain`` is not an instance of
+             :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`,
+           - if ``target_angular_position`` is not an instance of
+             :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`,
+           - if ``braking_angle`` is not an instance of :py:class:`Angle <gearpy.units.units.Angle>`.
+       ``ValueError``
+           If ``powertrain.elements`` is an empty :py:class:`tuple`.
 
-    Raises
-    ------
-    TypeError
-        - If ``encoder`` is not an instance of ``AbsoluteRotaryEncoder``,
-        - if ``powertrain`` is not an instance of ``Powertrain``,
-        - if the first element in ``powertrain`` is not an instance of ``MotorBase``,
-        - if an element of ``powertrain`` is not an instance of ``RotatingObject``,
-        - if ``target_angular_position`` is not an instance of ``AngularPosition``,
-        - if ``braking_angle`` is not an instance of ``Angle``.
-    ValueError
-        If ``powertrain.elements`` is an empty tuple.
-
-    See Also
-    --------
-    :py:attr:`gearpy.mechanical_objects.dc_motor.DCMotor.pwm`
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:attr:`DCMotor.pwm <gearpy.mechanical_objects.dc_motor.DCMotor.pwm>`
     """
 
     def __init__(self,
                  encoder: AbsoluteRotaryEncoder,
                  powertrain: Powertrain,
                  target_angular_position: AngularPosition,
                  braking_angle: Angle):
@@ -76,141 +69,82 @@
             raise TypeError(f"Parameter 'braking_angle' must be an instance of {Angle.__name__!r}.")
 
         self.__encoder = encoder
         self.__powertrain = powertrain
         self.__target_angular_position = target_angular_position
         self.__braking_angle = braking_angle
 
-    @property
-    def encoder(self) -> AbsoluteRotaryEncoder:
-        """Sensor used to measure the ``angular_position`` of a ``RotatingObject``, which is compared to
-        ``target_angular_position``.
-
-        Returns
-        -------
-        AbsoluteRotaryEncoder
-            Sensor used to measure the ``angular_position`` of a ``RotatingObject``, which is compared to
-            ``target_angular_position``.
-
-        Notes
-        -----
-        This parameter serves as a remainder for the user about the need to use an encoder in the mechanism, otherwise
-        this type of control cannot be applied.
-
-        See Also
-        --------
-        :py:class:`gearpy.sensors.AbsoluteRotaryEncoder`
-        """
-        return self.__encoder
-
-    @property
-    def powertrain(self) -> Powertrain:
-        """Powertrain whose motor's ``pwm`` is controlled in order to reach a specific angular position.
-
-        Returns
-        -------
-        Powertrain
-            Powertrain whose motor's ``pwm`` is controlled in order to reach a specific angular position.
-
-        See Also
-        --------
-        :py:class:`gearpy.powertrain.Powertrain`
-        """
-        return self.__powertrain
-
-    @property
-    def target_angular_position(self) -> AngularPosition:
-        """Angular position to be reached by the ``encoder``'s target. The rule is applied up until the ``encoder``'s
-        target's ``angular_position`` equals the ``target_angular_position``.
-
-        Returns
-        -------
-        AngularPosition
-            Angular position to be reached by the ``encoder``'s target.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularPosition`
-        """
-        return self.__target_angular_position
-
-    @property
-    def braking_angle(self) -> Angle:
-        """Angle within which the motor's ``pwm`` is controlled in order to brake and reach the
-        ``target_angular_position``. \n
-        The rule is applied only if the difference between ``target_angular_position`` and the ``encoder``'s target
-        ``angular_position`` is lower than or equal to the ``braking_angle``. \n
-        The lower the ``braking_angle`` the higher the deceleration of the system, thus the higher the vibrations
-        produced.
-
-        Returns
-        -------
-        Angle
-            The angle within which the motor's ``pwm`` is controlled in order to brake and reach the
-            ``target_angular_position``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Angle`
-        """
-        return self.__braking_angle
-
     def apply(self) -> Union[None, float, int]:
-        r"""Computes the ``pwm`` to apply to the ``powertrain``'s DC motor in order to reach a
+        """It computes the ``pwm`` to apply to the ``powertrain``'s DC motor in order to reach a 
         ``target_angular_position`` by the ``target`` rotating object of the ``encoder``, within a specific
         ``braking_angle``.
 
         Returns
         -------
-        float or int or None
+        :py:class:`float` or :py:class:`int` or :py:obj:`None`
             PWM value to apply to the motor in order to reach the target angular position.
 
-        Notes
-        -----
-        It computes the ``powertrain``'s *static error* according to the following formula:
-
-        .. math::
-            \theta_{err} \left( T_l \right) = \frac{T_l}{T_{max}} \, \frac{\theta_b}{\eta_t}
-
-        where:
-
-        - :math:`\theta_{err}` is the ``powertrain`` static error,
-        - :math:`T_l` is the load torque on the ``powertrain`` DC motor,
-        - :math:`T_{max}` is the maximum torque developed by the ``powertrain`` DC motor,
-        - :math:`\theta_b` is the ``braking_angle`` parameter,
-        - :math:`\eta_t` is the ``powertrain`` overall efficiency, computed as:
-
-        .. math::
-            \eta_t = \prod_{i = 1}^N \eta_i
-
-        where:
-
-        - :math:`\eta_i` is the mechanical mating efficiency of the mating between two gears,
-        - :math:`N` is the total number of gear matings in the ``powertrain``.
-
-        Then it checks the applicability condition, defined as:
-
-        .. math::
-            \theta \ge \theta_s = \theta_t - \theta_b + \theta_{err}
-
-        where:
+        .. admonition:: Notes
+           :class: tip
 
-        - :math:`\theta` is the ``encoder``'s ``target`` ``angular_position``,
-        - :math:`\theta_s` is the braking starting angle,
-        - :math:`\theta_t` is the ``target_angular_position`` parameter.
+           The braking angle is the angle within which the motor's ``pwm`` is controlled in order to brake and reach the
+           ``target_angular_position``. \n
+           The rule is applied only if the difference between ``target_angular_position`` and the ``encoder``'s target
+           ``angular_position`` is lower than or equal to the ``braking_angle``. \n
+           The lower the ``braking_angle`` the higher the deceleration of the system, thus the higher the vibrations
+           produced. \n
+           First of all, the rule computes the ``powertrain``'s *static error* according to the following formula:
+        """\
+        r"""
+           .. math::
+               \theta_{err} \left( T_l \right) = \frac{T_l}{T_{max}} \, \frac{\theta_b}{\eta_t}
+
+           where:
+
+           - :math:`\theta_{err}` is the ``powertrain`` static error,
+           - :math:`T_l` is the load torque on the ``powertrain`` DC motor 
+             (:py:attr:`DCMotor.load_torque <gearpy.mechanical_objects.dc_motor.DCMotor.load_torque>`),
+           - :math:`T_{max}` is the maximum torque developed by the ``powertrain`` DC motor
+             (:py:attr:`DCMotor.maximum_torque <gearpy.mechanical_objects.dc_motor.DCMotor.maximum_torque>`),
+           - :math:`\theta_b` is the ``braking_angle`` parameter,
+           - :math:`\eta_t` is the ``powertrain`` overall efficiency, computed as:
+
+           .. math::
+               \eta_t = \prod_{i = 1}^N \eta_i
+
+           where:
+
+           - :math:`\eta_i` is the mechanical mating efficiency of the mating between two gears 
+             (:py:attr:`SpurGear.master_gear_efficiency <gearpy.mechanical_objects.spur_gear.SpurGear.master_gear_efficiency>` or
+             :py:attr:`HelicalGear.master_gear_efficiency <gearpy.mechanical_objects.helical_gear.HelicalGear.master_gear_efficiency>` or
+             :py:attr:`WormGear.master_gear_efficiency <gearpy.mechanical_objects.worm_gear.WormGear.master_gear_efficiency>` or 
+             :py:attr:`WormWheel.master_gear_efficiency <gearpy.mechanical_objects.worm_wheel.WormWheel.master_gear_efficiency>`),
+           - :math:`N` is the total number of gear matings in the ``powertrain``.
+
+           Then it checks the applicability condition, defined as:
+
+           .. math::
+               \theta \ge \theta_s = \theta_t - \theta_b + \theta_{err}
+
+           where:
+
+           - :math:`\theta` is the ``encoder``'s ``target`` ``angular_position``,
+           - :math:`\theta_s` is the braking starting angle,
+           - :math:`\theta_t` is the ``target_angular_position`` parameter.
 
-        If the applicability condition is not met, then it returns ``None``, otherwise it computes the ``pwm`` as:
+           If the applicability condition is not met, then it returns :py:obj:`None`, otherwise it computes the ``pwm`` 
+           as:
 
-        .. math::
-            D \left( \theta \right) = 1 - \frac{\theta - \theta_s}{\theta_b}
+           .. math::
+               D \left( \theta \right) = 1 - \frac{\theta - \theta_s}{\theta_b}
 
-        where :math:`D` is the supply voltage PWM duty cycle (``pwm``) to apply to the DC motor in order to reach the
-        ``target_angular_position`` by the ``encoder``'s ``target`` rotating object.
+           where :math:`D` is the supply voltage PWM duty cycle ``pwm`` to apply to the DC motor in order to reach the
+           ``target_angular_position`` by the ``encoder``'s ``target`` rotating object.
         """
-        angular_position = self.encoder.get_value()
+        angular_position = self.__encoder.get_value()
 
-        regime_angular_position_error = _compute_static_error(braking_angle = self.braking_angle,
-                                                              powertrain = self.powertrain)
-        braking_starting_angle = self.target_angular_position - self.braking_angle + regime_angular_position_error
+        regime_angular_position_error = _compute_static_error(braking_angle = self.__braking_angle,
+                                                              powertrain = self.__powertrain)
+        braking_starting_angle = self.__target_angular_position - self.__braking_angle + regime_angular_position_error
 
         if angular_position >= braking_starting_angle:
-            return 1 - (angular_position - braking_starting_angle)/self.braking_angle
+            return 1 - (angular_position - braking_starting_angle)/self.__braking_angle
```

### Comparing `gearpy-0.6.0/gearpy/motor_control/rules/start_limit_current.py` & `gearpy-0.7.0/gearpy/motor_control/rules/start_limit_current.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,56 +3,47 @@
 from gearpy.units import AngularPosition, Current
 import numpy as np
 from gearpy.motor_control.rules.rules_base import RuleBase
 from typing import Union
 
 
 class StartLimitCurrent(RuleBase):
-    """gearpy.motor_control.rules.start_limit_current.StartLimitCurrent object. \n
+    """:py:class:`StartLimitCurrent <gearpy.motor_control.rules.start_limit_current.StartLimitCurrent>` object. \n
     It can be used to make a gradual start of the powertrain's motion and limit the ``motor`` absorbed electric
     current to be lower than or equal to a ``limit_electric_current`` value. It computes a ``pwm`` to apply to the
     ``motor`` up until the ``encoder``'s ``target``'s ``angular_position`` equals ``target_angular_position``. \n
     For an optimal ``pwm`` management, it is suggested to set the ``motor`` as the ``tachometer``'s ``target``.
 
-    Attributes
-    ----------
-    :py:attr:`encoder` : AbsoluteRotaryEncoder
-        Sensor used to measure the ``angular_position`` of a ``RotatingObject``, which is compared to
-        ``target_angular_position``.
-    :py:attr:`tachometer` : Tachometer
-        Sensor used to measure the ``angular_speed`` of a ``RotatingObject``.
-    :py:attr:`motor` : DCMotor
-        Motor that has to be controlled through ``pwm`` value.
-    :py:attr:`limit_electric_current` : Current
-        Maximum allowable electric current to be absorbed by the ``motor``.
-    :py:attr:`target_angular_position` : AngularPosition
-        Angular position to be reached by the ``encoder``'s target.
-
     Methods
     -------
     :py:meth:`apply`
-        Computes the ``pwm`` to apply to the ``motor`` in order to limit its absorbed electric current to be lower
+        It computes the ``pwm`` to apply to the ``motor`` in order to limit its absorbed electric current to be lower
         or equal to ``limit_electric_current``, until the ``encoder``'s ``target`` rotating object's
         ``angular_position`` equals the ``target_angular_position``.
 
-    Raises
-    ------
-    TypeError
-        - If ``encoder`` is not an instance of ``AbsoluteRotaryEncoder``,
-        - If ``tachometer`` is not an instance of ``Tachometer``,
-        - If ``motor`` is not an instance of ``DCMotor``,
-        - if ``target_angular_position`` is not an instance of ``AngularPosition``,
-        - if ``limit_electric_current`` is not an instance of ``Current``.
-    ValueError
-        - If the ``motor`` cannot compute ``electric_current`` property,
-        - if ``limit_electric_current`` is negative or null.
-
-    See Also
-    --------
-    :py:attr:`gearpy.mechanical_objects.dc_motor.DCMotor.pwm`
+    .. admonition:: Raises
+       :class: warning
+
+       ``TypeError``
+           - If ``encoder`` is not an instance of
+             :py:class:`AbsoluteRotaryEncoder <gearpy.sensors.absolute_rotary_encoder.AbsoluteRotaryEncoder>`,
+           - If ``tachometer`` is not an instance of :py:class:`Tachometer <gearpy.sensors.tachometer.Tachometer>`,
+           - If ``motor`` is not an instance of :py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>`,
+           - if ``target_angular_position`` is not an instance of
+             :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`,
+           - if ``limit_electric_current`` is not an instance of :py:class:`Current <gearpy.units.units.Current>`.
+       ``ValueError``
+           - If the ``motor`` cannot compute ``electric_current`` property
+             (:py:attr:`DCMotor.electric_current <gearpy.mechanical_objects.dc_motor.DCMotor.electric_current>`),
+           - if ``limit_electric_current`` is negative or null.
+
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:attr:`DCMotor.pwm <gearpy.mechanical_objects.dc_motor.DCMotor.pwm>`
     """
 
     def __init__(self,
                  encoder: AbsoluteRotaryEncoder,
                  tachometer: Tachometer,
                  motor: DCMotor,
                  target_angular_position: AngularPosition,
@@ -82,148 +73,64 @@
 
         self.__encoder = encoder
         self.__tachometer = tachometer
         self.__motor = motor
         self.__limit_electric_current = limit_electric_current
         self.__target_angular_position = target_angular_position
 
-    @property
-    def encoder(self) -> AbsoluteRotaryEncoder:
-        """Sensor used to measure the ``angular_position`` of a ``RotatingObject``, which is compared to
-        ``target_angular_position``.
-
-        Returns
-        -------
-        AbsoluteRotaryEncoder
-            Sensor used to measure the ``angular_position`` of a ``RotatingObject``, which is compared to
-            ``target_angular_position``.
-
-        Notes
-        -----
-        This parameter serves as a remainder for the user about the need to use an encoder in the mechanism, otherwise
-        this type of control cannot be applied.
-
-        See Also
-        --------
-        :py:class:`gearpy.sensors.AbsoluteRotaryEncoder`
-        """
-        return self.__encoder
-
-    @property
-    def tachometer(self) -> Tachometer:
-        """Sensor used to measure the ``angular_speed`` of a ``RotatingObject``.
-
-        Returns
-        -------
-        Tachometer
-            Sensor used to measure the ``angular_speed`` of a ``RotatingObject``.
-
-        Notes
-        -----
-        This parameter serves as a remainder for the user about the need to use a tachometer in the mechanism,
-        otherwise this type of control cannot be applied.
-
-        See Also
-        --------
-        :py:class:`gearpy.sensors.Tachometer`
-        """
-        return self.__tachometer
-
-    @property
-    def motor(self) -> DCMotor:
-        """Motor that has to be controlled through ``pwm`` value.
-
-        Returns
-        -------
-        DCMotor
-           Motor that has to be controlled through ``pwm`` value.
-
-        See Also
-        --------
-        :py:class:`gearpy.mechanical_objects.dc_motor.DCMotor`
-        """
-        return self.__motor
-
-    @property
-    def limit_electric_current(self) -> Current:
-        """Maximum allowable electric current to be absorbed by the ``motor``. While the rule is applied, the absorbed
-        electric current is equal to or lower than this value.
-
-        Returns
-        -------
-        Current
-            Maximum allowable electric current to be absorbed by the ``DCMotor``.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.Current`
-        """
-        return self.__limit_electric_current
-
-    @property
-    def target_angular_position(self) -> AngularPosition:
-        """Angular position to be reached by the ``encoder``'s target. The rule is applied up until the ``encoder``'s
-        target's ``angular_position`` equals the ``target_angular_position``.
-
-        Returns
-        -------
-        AngularPosition
-            Angular position to be reached by the ``encoder``'s target.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.AngularPosition`
-        """
-        return self.__target_angular_position
-
     def apply(self) -> Union[None, float, int]:
-        r"""Computes the ``pwm`` to apply to the ``motor`` in order to limit its absorbed electric current to be lower
-        or equal to ``limit_electric_current``, until the ``encoder``'s ``target`` rotating object's
+        r"""It computes the ``pwm`` to apply to the ``motor`` in order to limit its absorbed electric current to be
+        lower or equal to ``limit_electric_current``, until the ``encoder``'s ``target`` rotating object's
         ``angular_position`` equals the ``target_angular_position``.
 
         Returns
         -------
-        float or int or None
+        :py:class:`float` or :py:class:`int` or :py:obj:`None`
             PWM value to apply to the ``motor`` in order to limit its absorbed electric current to be lower or equal to
             ``limit_electric_current``
 
-        Notes
-        -----
-        It checks the applicability condition, defined as:
-
-        .. math::
-            \theta \le \theta_t
+        .. admonition:: Notes
+           :class: tip
 
-        where:
+           It checks the applicability condition, defined as:
 
-        - :math:`\theta` is the ``encoder``'s ``target`` ``angular_position``,
-        - :math:`\theta_t` is the ``target_angular_position``.
+           .. math::
+               \theta \le \theta_t
 
-        If the applicability condition is not met, then it returns ``None``, otherwise it computes the ``pwm`` as:
-
-        .. math::
-            D \left( \dot{\theta} \right) = \frac{1}{2} \, \left( \frac{\dot{\theta}}{\dot{\theta}_0} +
-            \frac{i_{lim}}{i_{max}} + \sqrt{ \left( \frac{\dot{\theta}}{\dot{\theta}_0} \right)^2 +
-            \left( \frac{i_{lim}}{i_{max}} \right)^2 +
-            2 \frac{\dot{\theta}}{\dot{\theta}_0} \frac{i_{lim} - 2 i_0}{i_{max}} } \right)
-
-        where:
-
-        - :math:`\dot{\theta}` is the ``tachometer``'s ``target``'s angular speed,
-        - :math:`\dot{\theta}_0` is the ``motor`` no load angular speed (``no_load_speed``),
-        - :math:`i_{lim}` is the ``limit_electric_current`` parameter,
-        - :math:`i_{max}` is the ``motor`` maximum electric current (``maximum_electric_current``),
-        - :math:`i_0` is the ``motor`` no load electric current (``no_load_electric_current``).
-        """
-        angular_position = self.encoder.get_value()
-        angular_speed = self.tachometer.get_value()
-        no_load_speed = self.motor.no_load_speed
-        maximum_electric_current = self.motor.maximum_electric_current
-        no_load_electric_current = self.motor.no_load_electric_current
+           where:
+
+           - :math:`\theta` is the ``encoder``'s ``target`` ``angular_position``,
+           - :math:`\theta_t` is the ``target_angular_position``.
+
+           If the applicability condition is not met, then it returns :py:obj:`None`, otherwise it computes the ``pwm``
+           as:
+
+           .. math::
+               D \left( \dot{\theta} \right) = \frac{1}{2} \, \left( \frac{\dot{\theta}}{\dot{\theta}_0} +
+               \frac{i_{lim}}{i_{max}} + \sqrt{ \left( \frac{\dot{\theta}}{\dot{\theta}_0} \right)^2 +
+               \left( \frac{i_{lim}}{i_{max}} \right)^2 +
+               2 \frac{\dot{\theta}}{\dot{\theta}_0} \frac{i_{lim} - 2 i_0}{i_{max}} } \right)
+
+           where:
+
+           - :math:`\dot{\theta}` is the ``tachometer``'s ``target``'s angular speed,
+           - :math:`\dot{\theta}_0` is the ``motor`` no load angular speed
+             (:py:attr:`DCMotor.no_load_speed <gearpy.mechanical_objects.dc_motor.DCMotor.no_load_speed>`),
+           - :math:`i_{lim}` is the ``limit_electric_current`` parameter,
+           - :math:`i_{max}` is the ``motor`` maximum electric current
+             (:py:attr:`DCMotor.maximum_electric_current <gearpy.mechanical_objects.dc_motor.DCMotor.maximum_electric_current>`),
+           - :math:`i_0` is the ``motor`` no load electric current
+             (:py:attr:`DCMotor.no_load_electric_current <gearpy.mechanical_objects.dc_motor.DCMotor.no_load_electric_current>`).
+        """
+        angular_position = self.__encoder.get_value()
+        angular_speed = self.__tachometer.get_value()
+        no_load_speed = self.__motor.no_load_speed
+        maximum_electric_current = self.__motor.maximum_electric_current
+        no_load_electric_current = self.__motor.no_load_electric_current
         speed_ratio = angular_speed/no_load_speed
-        electric_ratio = self.limit_electric_current/maximum_electric_current
+        electric_ratio = self.__limit_electric_current/maximum_electric_current
 
-        if angular_position <= self.target_angular_position:
+        if angular_position <= self.__target_angular_position:
             return 1/2*(speed_ratio + electric_ratio +
                         np.sqrt(speed_ratio**2 + electric_ratio**2 +
-                                2*speed_ratio*((self.limit_electric_current - 2*no_load_electric_current)/
+                                2*speed_ratio*((self.__limit_electric_current - 2*no_load_electric_current)/
                                                 maximum_electric_current)))
```

### Comparing `gearpy-0.6.0/gearpy/motor_control/rules/utils.py` & `gearpy-0.7.0/gearpy/motor_control/rules/utils.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.6.0/gearpy/sensors/absolute_rotary_encoder.py` & `gearpy-0.7.0/gearpy/sensors/absolute_rotary_encoder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 from gearpy.mechanical_objects import RotatingObject
 from gearpy.units import AngularPosition
+from .sensor_base import SensorBase
 from typing import Optional, Union
 
 
-class AbsoluteRotaryEncoder:
-    r"""``gearpy.sensors.absolute_rotary_encoder.AbsoluteRotaryEncoder`` object.
+class AbsoluteRotaryEncoder(SensorBase):
+    r""":py:class:`AbsoluteRotaryEncoder <gearpy.sensors.absolute_rotary_encoder.AbsoluteRotaryEncoder>` object.
 
     Attributes
     ----------
-    :py:attr:`target` : RotatingObject
+    :py:attr:`target` : :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
         Target rotating object whose angular position is probed by the sensor.
 
     Methods
     -------
     :py:meth:`get_value`
-        Gets the angular position of the ``target`` rotating object.
+        It gets the angular position of the :py:attr:`target` rotating object.
     """
 
     def __init__(self, target: RotatingObject):
         if not isinstance(target, RotatingObject):
             raise TypeError(f"Parameter 'target' must be an instance of {RotatingObject.__name__!r}.")
 
         self.__target = target
 
     @property
     def target(self) -> RotatingObject:
         """Target rotating object whose angular position is probed by the sensor.
 
         Returns
         -------
-        RotatingObject
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
             Target rotating object whose angular position is probed by the sensor.
 
-        Raises
-        ------
-        TypeError
-            If ``target`` is not an instance of ``RotatingObject``.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`target` is not an instance of
+               :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`.
         """
         return self.__target
 
     def get_value(self, unit: Optional[str] = None) -> Union[AngularPosition, float, int]:
-        """Gets the angular position of the ``target`` rotating object. \n
+        """It gets the angular position of the :py:attr:`target` rotating object. \n
         If a ``unit`` is set, then it converts the angular position to that unit and returns only the numerical value as
         float or integer.
 
         Parameters
         ----------
-        unit : str, optional
-            The unit to which convert the ``target`` angular position. If specified, it converts the angular position
-            and returns only the numerical value as float or integer, otherwise it returns an ``AngularPosition``.
-            Default is ``None``, so it returns an ``AngularPosition``.
+        ``unit`` : :py:class:`str`, optional
+            The unit to which convert the :py:attr:`target` angular position. If specified, it converts the angular
+            position and returns only the numerical value as float or integer, otherwise it returns an
+            :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`. Default is :py:obj:`None`, so it returns
+            an :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`.
 
         Returns
         -------
-        AngularPosition or float or int
-            Angular position of the ``target`` rotating object.
+        :py:class:`AngularPosition <gearpy.units.units.AngularPosition>` or :py:class:`float` or :py:class:`int`
+            Angular position of the :py:attr:`target` rotating object.
+
+        .. admonition:: Raises
+           :class: warning
 
-        Raises
-        ------
-        TypeError
-            If ``unit`` is not a string.
-
-        See Also
-        --------
-        :py:func:`gearpy.units.units.AngularPosition`
+           ``TypeError``
+               If ``unit`` is not a :py:class:`str`.
         """
         if not isinstance(unit, str) and unit is not None:
             raise TypeError("Parameter 'unit' must be a string.")
 
         if unit is None:
             return self.__target.angular_position
         else:
```

### Comparing `gearpy-0.6.0/gearpy/sensors/tachometer.py` & `gearpy-0.7.0/gearpy/sensors/tachometer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 from gearpy.mechanical_objects import RotatingObject
 from gearpy.units import AngularSpeed
+from .sensor_base import SensorBase
 from typing import Optional, Union
 
 
-class Tachometer:
-    r"""``gearpy.sensors.tachometer.Tachometer`` object.
+class Tachometer(SensorBase):
+    r""":py:class:`Tachometer <gearpy.sensors.tachometer.Tachometer>` object.
 
     Attributes
     ----------
-    :py:attr:`target` : RotatingObject
+    :py:attr:`target` : :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
         Target rotating object whose angular speed is probed by the sensor.
 
     Methods
     -------
     :py:meth:`get_value`
-        Gets the angular speed of the ``target`` rotating object.
+        It gets the angular speed of the :py:attr:`target` rotating object.
     """
 
     def __init__(self, target: RotatingObject):
         if not isinstance(target, RotatingObject):
             raise TypeError(f"Parameter 'target' must be an instance of {RotatingObject.__name__!r}.")
 
         self.__target = target
 
     @property
     def target(self) -> RotatingObject:
         """Target rotating object whose angular speed is probed by the sensor.
 
         Returns
         -------
-        RotatingObject
+        :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`
             Target rotating object whose angular speed is probed by the sensor.
 
-        Raises
-        ------
-        TypeError
-            If ``target`` is not an instance of ``RotatingObject``.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`target` is not an instance of
+               :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`.
         """
         return self.__target
 
     def get_value(self, unit: Optional[str] = None) -> Union[AngularSpeed, float, int]:
-        """Gets the angular speed of the ``target`` rotating object. \n
+        """It gets the angular speed of the :py:attr:`target` rotating object. \n
         If a ``unit`` is set, then it converts the angular speed to that unit and returns only the numerical value as
         float or integer.
 
         Parameters
         ----------
-        unit : str, optional
-            The unit to which convert the ``target`` angular speed. If specified, it converts the angular speed and
-            returns only the numerical value as float or integer, otherwise it returns an ``AngularSpeed``. Default is
-            ``None``, so it returns an ``AngularSpeed``.
+        ``unit`` : :py:class:`str`, optional
+            The unit to which convert the :py:attr:`target` angular speed. If specified, it converts the angular speed
+            and returns only the numerical value as float or integer, otherwise it returns an
+            :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`. Default is :py:obj:`None`, so it returns an
+            :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`.
 
         Returns
         -------
-        AngularSpeed or float or int
-            Angular speed of the ``target`` rotating object.
+        :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>` or :py:class:`float` or :py:class:`int`
+            Angular speed of the :py:attr:`target` rotating object.
+
+        .. admonition:: Raises
+           :class: warning
 
-        Raises
-        ------
-        TypeError
-            If ``unit`` is not a string.
-
-        See Also
-        --------
-        :py:func:`gearpy.units.units.AngularSpeed`
+           ``TypeError``
+               If ``unit`` is not a :py:class:`str`.
         """
         if not isinstance(unit, str) and unit is not None:
             raise TypeError("Parameter 'unit' must be a string.")
 
         if unit is None:
             return self.__target.angular_speed
         else:
```

### Comparing `gearpy-0.6.0/gearpy/sensors/timer.py` & `gearpy-0.7.0/gearpy/sensors/timer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from gearpy.units import Time, TimeInterval
 
 
 class Timer:
-    r"""``gearpy.sensors.timer.Timer`` object.
+    r""":py:class:`Timer <gearpy.sensors.timer.Timer>` object.
 
     Attributes
     ----------
-    :py:attr:`start_time` : Time
+    :py:attr:`start_time` : :py:class:`Time <gearpy.units.units.Time>`
         Start time after which the timer is active.
-    :py:attr:`duration` : TimeInterval
-        Time duration of the timer, starting from ``start_time``
+    :py:attr:`duration` : :py:class:`TimeInterval <gearpy.units.units.TimeInterval>`
+        Time duration of the timer, starting from :py:attr:`start_time`
 
     Methods
     -------
     :py:meth:`is_active`
-        Checks if the simulation ``current_time`` is greater than or equal to ``start_time`` but lower than or equal
-        to ``current_time`` + ``duration``.
+        It checks if the simulation ``current_time`` is greater than or equal to :py:attr:`start_time` but lower than or
+        equal to the sum of ``current_time`` and :py:attr:`duration`.
     """
 
     def __init__(self, start_time: Time, duration: TimeInterval):
         if not isinstance(start_time, Time):
             raise TypeError(f"Parameter 'start_time' must be an instance of {Time.__name__!r}.")
 
         if not isinstance(duration, TimeInterval):
@@ -30,57 +30,60 @@
 
     @property
     def start_time(self) -> Time:
         """Start time after which the timer is active.
 
         Returns
         -------
-        Time
+        :py:class:`Time <gearpy.units.units.Time>`
             Start time after which the timer is active.
 
-        Raises
-        ------
-        TypeError
-            If ``start_time`` is not an instance of ``Time``.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`start_time` is not an instance of :py:class:`Time <gearpy.units.units.Time>`.
         """
         return self.__start_time
 
     @property
     def duration(self) -> TimeInterval:
-        """Time duration of the timer, starting from ``start_time``.
+        """Time duration of the timer, starting from :py:attr:`start_time`.
 
         Returns
         -------
-        TimeInterval
-            Time duration of the timer, starting from ``start_time``
+        :py:class:`TimeInterval <gearpy.units.units.TimeInterval>`
+            Time duration of the timer, starting from :py:attr:`start_time`
+
+        .. admonition:: Raises
+           :class: warning
 
-        Raises
-        ------
-        TypeError
-            If ``duration`` is not an instance of ``TimeInterval``.
+           ``TypeError``
+               If :py:attr:`duration` is not an instance of :py:class:`TimeInterval <gearpy.units.units.TimeInterval>`.
         """
         return self.__duration
 
     def is_active(self, current_time: Time) -> bool:
-        """Checks if the simulation ``current_time`` is greater than or equal to ``start_time`` but lower than or equal
-        to ``current_time`` + ``duration``.
+        """It checks if the simulation ``current_time`` is greater than or equal to :py:attr:`start_time` but lower than
+        or equal to the sum of ``current_time`` and :py:attr:`duration`.
 
         Parameters
         ----------
-        current_time : Time
-            Current time of the simulation, to be compared with ``start_time`` and ``duration``.
+        ``current_time`` : :py:class:`Time <gearpy.units.units.Time>`
+            Current time of the simulation, to be compared with :py:attr:`start_time` and :py:attr:`duration`.
 
         Returns
         -------
-        bool
-            Whether ``current_time`` is greater than or equal to ``start_time`` but lower than or equal to
-            ``start_time`` + ``duration``.
-
-        Raises
-        ------
-        TypeError
-            If ``current_time`` is not an instance of ``Time``.
+        :py:class:`bool`
+            Whether ``current_time`` is greater than or equal to :py:attr:`start_time` but lower than or equal to the
+            sum of :py:attr:`start_time` and :py:attr:`duration`.
+
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If ``current_time`` is not an instance of :py:class:`Time <gearpy.units.units.Time>`.
         """
         if not isinstance(current_time, Time):
             raise TypeError(f"Parameter 'current_time' must be an instance of {Time.__name__!r}.")
 
         return (current_time >= self.start_time) and ((current_time - self.start_time) <= self.duration)
```

### Comparing `gearpy-0.6.0/gearpy/solver.py` & `gearpy-0.7.0/gearpy/solver.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,278 +1,290 @@
-from gearpy.mechanical_objects import RotatingObject, MotorBase, GearBase
+from gearpy.mechanical_objects import RotatingObject, MotorBase, GearBase, WormGear
 from gearpy.motor_control import MotorControlBase
 from gearpy.powertrain import Powertrain
 from gearpy.units import Time, TimeInterval, Torque, AngularSpeed, AngularAcceleration
+from gearpy.utils import StopCondition
 import numpy as np
 from typing import Optional
 
 
 NULL_ANGULAR_SPEED = AngularSpeed(0, 'rad/s')
 NULL_ANGULAR_ACCELERATION = AngularAcceleration(0, 'rad/s^2')
 NULL_TORQUE = Torque(0, 'Nm')
 
 
 class Solver:
-    r"""``gearpy.solver.Solver`` object.
-
-    Attributes
-    ----------
-    :py:attr:`powertrain` : Powertrain
-        Mechanical powertrain to be simulated.
+    r""":py:class:`Solver <gearpy.solver.Solver>` object.
 
     Methods
     -------
     :py:meth:`run`
-        Runs the powertrain simulation.
+        It runs the powertrain simulation.
+
+    .. admonition:: Raises
+       :class: warning
 
-    Raises
-    ------
-    TypeError
-        - If ``powertrain`` is not an instance of ``Powertrain``,
-        - if the first element in ``powertrain`` is not an instance of ``MotorBase``,
-        - if an element of ``powertrain`` is not an instance of ``RotatingObject``,
-        - if ``motor_control`` is not an instance of ``MotorControlBase``.
-    ValueError
-        If ``powertrain.elements`` is an empty tuple.
-
-    See Also
-    --------
-    :py:class:`gearpy.powertrain.Powertrain`
-    :py:class:`gearpy.motor_control.pwm_control.PWMControl`
+       ``TypeError``
+           - If ``powertrain`` is not an instance of :py:class:`Powertrain <gearpy.powertrain.Powertrain>`,
+           - if the first element in ``powertrain`` is not an instance of
+             :py:class:`MotorBase <gearpy.mechanical_objects.mechanical_object_base.MotorBase>`,
+           - if an element of ``powertrain`` is not an instance of
+             :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`.
+       ``ValueError``
+           If :py:attr:`Powertrain.elements <gearpy.powertrain.Powertrain.elements>` is an empty :py:class:`tuple`.
     """
 
-    def __init__(self, powertrain: Powertrain, motor_control: Optional[MotorControlBase] = None):
+    def __init__(self, powertrain: Powertrain):
         if not isinstance(powertrain, Powertrain):
             raise TypeError(f"Parameter 'powertrain' must be an instance of {Powertrain.__name__!r}.")
 
         if not powertrain.elements:
             raise ValueError("Parameter 'powertrain.elements' cannot be an empty tuple.")
 
         if not isinstance(powertrain.elements[0], MotorBase):
             raise TypeError(f"First element in 'powertrain' must be an instance of {MotorBase.__name__!r}.")
 
         if not all([isinstance(element, RotatingObject) for element in powertrain.elements]):
             raise TypeError(f"All elements of 'powertrain' must be instances of {RotatingObject.__name__!r}.")
 
-        if not isinstance(motor_control, MotorControlBase) and motor_control is not None:
-            raise TypeError(f"Parameter 'motor_control' must be an instance of {MotorControlBase.__name__!r}.")
-
-        self.powertrain = powertrain
-        self.motor_control = motor_control
+        self.__powertrain = powertrain
         self.__powertrain_is_locked = False
 
-    def run(self, time_discretization: TimeInterval, simulation_time: TimeInterval):
-        """Runs the powertrain simulation. \n
+    def run(self,
+            time_discretization: TimeInterval,
+            simulation_time: TimeInterval,
+            motor_control: Optional[MotorControlBase] = None,
+            stop_condition: Optional[StopCondition] = None) -> None:
+        """It runs the powertrain simulation. \n
         The simulation is performed in several steps:
 
         - it computes the whole powertrain equivalent moment of inertia with respect to the last
           gear, by multiplying each element's moment of inertia, starting from the motor, by it gear ratio with respect
-          to the following element in the powertrain elements and sum them up
+          to the following element in the powertrain elements and sum them up,
         - for each time step and for each powertrain element, it computes:
 
-          - the angular position and angular speed, from the last element in the powertrain elements to the first one
+          - the angular position and angular speed, from the last element in the powertrain elements to the first one,
           - the driving torque, load torque, net torque, electrical current for motors (if computable), tangential
-            force, bending stress and contact stress for gears (if computable)
-          - the angular acceleration of each powertrain element.
+            force, bending stress and contact stress for gears (if computable), motor control rules (if available),
+            simulation stopping condition (if available),
+          - the angular acceleration of each powertrain element,
 
         - for each time step it performs a time integration to compute angular position and speed of the last element in
           the powertrain elements.
 
         Parameters
         ----------
-        time_discretization : TimeInterval
+        ``time_discretization`` : :py:class:`TimeInterval <gearpy.units.units.TimeInterval>`
             Time discretization to be used for the simulation.
-        simulation_time : TimeInterval
+        ``simulation_time`` : :py:class:`TimeInterval <gearpy.units.units.TimeInterval>`
             Duration of the simulation.
-
-        Raises
-        ------
-        TypeError
-            - If ``time_discretization`` is not an instance of ``TimeInterval``,
-            - if ``simulation_time`` is not an instance of ``TimeInterval``,
-            - if function ``external_torque`` of one gear in the powertrain elements does not return an instance of
-              ``Torque``.
-        ValueError
-            - If ``time_discretization`` is greater or equal to ``simulation_time``,
-            - if function ``external_torque`` has not been defined for any gear of the powertrain.
-
-        Notes
-        -----
-        If ``powertrain.elements.time`` is an empty list, it performs the simulation starting the time from ``0 sec``;
-        otherwise it concatenates another simulation to existing values of time and time variables.
-
-        See Also
-        --------
-        :py:class:`gearpy.units.units.TimeInterval`
+        ``motor_control`` : :py:class:`MotorControlBase <gearpy.motor_control.motor_control_base.MotorControlBase>`, optional
+            Rules to control the powertrain motor.
+        ``stop_condition`` : :py:class:`StopCondition <gearpy.utils.stop_condition.stop_condition.StopCondition>`, optional
+            Simulation stopping condition.
+
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If ``time_discretization`` is not an instance of
+                 :py:class:`TimeInterval <gearpy.units.units.TimeInterval>`,
+               - if ``simulation_time`` is not an instance of
+                 :py:class:`TimeInterval <gearpy.units.units.TimeInterval>`,
+               - if ``motor_control`` is not an instance of
+                 :py:class:`MotorControlBase <gearpy.motor_control.motor_control_base.MotorControlBase>`,
+               - if ``stop_condition`` is not an instance of
+                 :py:class:`StopCondition <gearpy.utils.stop_condition.stop_condition.StopCondition>`,
+               - if function ``external_torque`` of one gear in the powertrain elements does not return an instance of
+                 :py:class:`Torque <gearpy.units.units.Torque>`,
+           ``ValueError``
+               - If ``time_discretization`` is greater or equal to ``simulation_time``,
+               - if function ``external_torque`` has not been defined for any gear of the powertrain.
+
+        .. admonition:: Notes
+           :class: tip
+
+           If :py:attr:`Powertrain.time <gearpy.powertrain.Powertrain.time>` is an empty :py:class:`list`, it performs
+           the simulation starting the time from ``0 sec``; otherwise it concatenates another simulation to existing
+           values of time and time variables.
         """
         if not isinstance(time_discretization, TimeInterval):
             raise TypeError(f"Parameter 'time_discretization' must be an instance of {TimeInterval.__name__!r}.")
 
         if not isinstance(simulation_time, TimeInterval):
             raise TypeError(f"Parameter 'simulation_time' must be an instance of {TimeInterval.__name__!r}.")
 
         if time_discretization >= simulation_time:
             raise ValueError("Parameter 'time_discretization' cannot be greater or equal to 'simulation_time'.")
 
         if not any([element.external_torque is not None
-                    for element in self.powertrain.elements if isinstance(element, GearBase)]):
+                    for element in self.__powertrain.elements if isinstance(element, GearBase)]):
             raise ValueError("The function 'external_torque' has not been defined for any gear of the powertrain. "
                              "Add this function to a powertrain gear.")
 
+        if not isinstance(motor_control, MotorControlBase) and motor_control is not None:
+            raise TypeError(f"Parameter 'motor_control' must be an instance of {MotorControlBase.__name__!r}.")
+
+        if not isinstance(stop_condition, StopCondition) and stop_condition is not None:
+            raise TypeError(f"Parameter 'stop_condition' must be an instance of {StopCondition.__name__!r}.")
+
         self._compute_powertrain_inertia()
-        if self.powertrain.time:
-            initial_time = self.powertrain.time[-1]
+        if self.__powertrain.time:
+            initial_time = self.__powertrain.time[-1]
             final_time = initial_time + simulation_time + time_discretization
         else:
             initial_time = Time(value = 0, unit = time_discretization.unit)
             final_time = initial_time + simulation_time + time_discretization
-            self.powertrain.update_time(initial_time)
-            self._compute_powertrain_variables()
+            self.__powertrain.update_time(initial_time)
+            self._compute_powertrain_variables(motor_control = motor_control)
 
         for k in np.arange(initial_time.value + time_discretization.value, final_time.value, time_discretization.value):
 
-            self.powertrain.update_time(Time(value = float(k), unit = time_discretization.unit))
+            self.__powertrain.update_time(Time(value = float(k), unit = time_discretization.unit))
             self._time_integration(time_discretization = time_discretization)
-            self._compute_powertrain_variables()
+            self._compute_powertrain_variables(motor_control = motor_control)
+            if stop_condition is not None:
+                if stop_condition.check_condition():
+                    break
 
     def _compute_powertrain_inertia(self):
 
-        self.powertrain_inertia_moment = self.powertrain.elements[0].inertia_moment
-        for element in self.powertrain.elements[1:]:
-            self.powertrain_inertia_moment *= element.master_gear_ratio
-            self.powertrain_inertia_moment += element.inertia_moment
+        self.__powertrain_inertia_moment = self.__powertrain.elements[0].inertia_moment
+        for element in self.__powertrain.elements[1:]:
+            self.__powertrain_inertia_moment *= element.master_gear_ratio
+            self.__powertrain_inertia_moment += element.inertia_moment
 
-    def _compute_powertrain_variables(self):
+    def _compute_powertrain_variables(self, motor_control: Optional[MotorControlBase]):
 
         self._compute_angular_position_and_speed()
         self._check_powertrain_is_locked()
         if self.__powertrain_is_locked:
             self._compute_locked_powertrain_angular_speed_and_acceleration()
         self._compute_load_torque()
-        self._compute_motor_control()
+        self._compute_motor_control(motor_control = motor_control)
         self._compute_driving_torque()
         self._compute_torque()
         if not self.__powertrain_is_locked:
             self._compute_angular_acceleration()
         self._compute_force()
         self._compute_stress()
         self._compute_electric_current()
         self._update_time_variables()
 
     def _compute_angular_position_and_speed(self):
 
-        for i in range(len(self.powertrain.elements) - 2, -1, -1):
-            gear_ratio = self.powertrain.elements[i + 1].master_gear_ratio
+        for i in range(len(self.__powertrain.elements) - 2, -1, -1):
+            gear_ratio = self.__powertrain.elements[i + 1].master_gear_ratio
             self._transmit_angular_position(gear_ratio = gear_ratio, i = i)
             self._transmit_angular_speed(gear_ratio = gear_ratio, i = i)
 
     def _transmit_angular_position(self, gear_ratio, i):
 
-        self.powertrain.elements[i].angular_position = gear_ratio*self.powertrain.elements[i + 1].angular_position
+        self.__powertrain.elements[i].angular_position = gear_ratio*self.__powertrain.elements[i + 1].angular_position
 
     def _transmit_angular_speed(self, gear_ratio, i):
 
-        self.powertrain.elements[i].angular_speed = gear_ratio*self.powertrain.elements[i + 1].angular_speed
+        self.__powertrain.elements[i].angular_speed = gear_ratio*self.__powertrain.elements[i + 1].angular_speed
 
     def _transmit_angular_acceleration(self, gear_ratio, i):
 
-        self.powertrain.elements[i].angular_acceleration = \
-                gear_ratio*self.powertrain.elements[i + 1].angular_acceleration
+        self.__powertrain.elements[i].angular_acceleration = \
+                gear_ratio*self.__powertrain.elements[i + 1].angular_acceleration
 
-    def _compute_motor_control(self):
+    def _compute_motor_control(self, motor_control: Optional[MotorControlBase]):
 
-        if self.motor_control is not None:
-            self.motor_control.apply_rules()
+        if motor_control is not None:
+            motor_control.apply_rules()
 
     def _compute_driving_torque(self):
 
-        self.powertrain.elements[0].compute_torque()
+        self.__powertrain.elements[0].compute_torque()
 
-        for i in range(1, len(self.powertrain.elements)):
-            self.powertrain.elements[i].driving_torque = self.powertrain.elements[i - 1].driving_torque* \
-                                                         self.powertrain.elements[i].master_gear_efficiency* \
-                                                         self.powertrain.elements[i].master_gear_ratio
+        for i in range(1, len(self.__powertrain.elements)):
+            self.__powertrain.elements[i].driving_torque = self.__powertrain.elements[i - 1].driving_torque* \
+                                                           self.__powertrain.elements[i].master_gear_efficiency* \
+                                                           self.__powertrain.elements[i].master_gear_ratio
 
     def _compute_load_torque(self):
 
-        for i in range(len(self.powertrain.elements) - 1, 0, -1):
-            if hasattr(self.powertrain.elements[i], 'external_torque'):
-                if self.powertrain.elements[i].external_torque is not None:
+        for i in range(len(self.__powertrain.elements) - 1, 0, -1):
+            if hasattr(self.__powertrain.elements[i], 'external_torque'):
+                if self.__powertrain.elements[i].external_torque is not None:
                     external_torque = \
-                        self.powertrain.elements[i].\
-                        external_torque(time = self.powertrain.time[-1],
-                                        angular_position = self.powertrain.elements[i].angular_position,
-                                        angular_speed = self.powertrain.elements[i].angular_speed)
+                        self.__powertrain.elements[i].\
+                        external_torque(time = self.__powertrain.time[-1],
+                                        angular_position = self.__powertrain.elements[i].angular_position,
+                                        angular_speed = self.__powertrain.elements[i].angular_speed)
                     if not isinstance(external_torque, Torque):
-                        raise TypeError(f"Function 'external_torque' of {self.powertrain.elements[i].name!r} "
+                        raise TypeError(f"Function 'external_torque' of {self.__powertrain.elements[i].name!r} "
                                         f"must return an instance of {Torque.__name__!r}.")
-                    self.powertrain.elements[i].load_torque = external_torque
+                    self.__powertrain.elements[i].load_torque = external_torque
 
-            self.powertrain.elements[i - 1].load_torque = self.powertrain.elements[i].load_torque/ \
-                                                          self.powertrain.elements[i].master_gear_efficiency/ \
-                                                          self.powertrain.elements[i].master_gear_ratio
+            self.__powertrain.elements[i - 1].load_torque = self.__powertrain.elements[i].load_torque/ \
+                                                            self.__powertrain.elements[i].master_gear_efficiency/ \
+                                                            self.__powertrain.elements[i].master_gear_ratio
 
     def _compute_torque(self):
 
-        for element in self.powertrain.elements:
+        for element in self.__powertrain.elements:
             element.torque = element.driving_torque - element.load_torque
 
     def _compute_force(self):
 
-        for element in self.powertrain.elements:
-            if isinstance(element, GearBase):
+        for element in self.__powertrain.elements:
+            if isinstance(element, GearBase) or isinstance(element, WormGear):
                 if element.tangential_force_is_computable:
                     element.compute_tangential_force()
 
     def _compute_stress(self):
 
-        for element in self.powertrain.elements:
+        for element in self.__powertrain.elements:
             if isinstance(element, GearBase):
                 if element.bending_stress_is_computable:
                     element.compute_bending_stress()
                     if element.contact_stress_is_computable:
                         element.compute_contact_stress()
 
     def _compute_electric_current(self):
 
-        if self.powertrain.elements[0].electric_current_is_computable:
-            self.powertrain.elements[0].compute_electric_current()
+        if self.__powertrain.elements[0].electric_current_is_computable:
+            self.__powertrain.elements[0].compute_electric_current()
 
     def _compute_angular_acceleration(self):
 
-        self.powertrain.elements[-1].angular_acceleration = self.powertrain.elements[-1].torque/\
-                                                            self.powertrain_inertia_moment
+        self.__powertrain.elements[-1].angular_acceleration = self.__powertrain.elements[-1].torque/ \
+                                                              self.__powertrain_inertia_moment
 
-        for i in range(len(self.powertrain.elements) - 2, -1, -1):
-            gear_ratio = self.powertrain.elements[i + 1].master_gear_ratio
+        for i in range(len(self.__powertrain.elements) - 2, -1, -1):
+            gear_ratio = self.__powertrain.elements[i + 1].master_gear_ratio
             self._transmit_angular_acceleration(gear_ratio = gear_ratio, i = i)
 
     def _update_time_variables(self):
 
-        for element in self.powertrain.elements:
+        for element in self.__powertrain.elements:
             element.update_time_variables()
 
     def _time_integration(self, time_discretization: TimeInterval):
 
-        self.powertrain.elements[-1].angular_speed += \
-            self.powertrain.elements[-1].angular_acceleration*time_discretization
-        self.powertrain.elements[-1].angular_position += \
-            self.powertrain.elements[-1].angular_speed*time_discretization
+        self.__powertrain.elements[-1].angular_speed += \
+            self.__powertrain.elements[-1].angular_acceleration*time_discretization
+        self.__powertrain.elements[-1].angular_position += \
+            self.__powertrain.elements[-1].angular_speed*time_discretization
 
     def _check_powertrain_is_locked(self):
 
-        motor = self.powertrain.elements[0]
-        if self.powertrain.self_locking and (motor.pwm == 0 or
-                                             (motor.pwm > 0 and motor.angular_speed < NULL_ANGULAR_SPEED) or
-                                             (motor.pwm < 0 and motor.angular_speed > NULL_ANGULAR_SPEED)):
+        motor = self.__powertrain.elements[0]
+        if self.__powertrain.self_locking and (motor.pwm == 0 or
+                                               (motor.pwm > 0 and motor.angular_speed < NULL_ANGULAR_SPEED) or
+                                               (motor.pwm < 0 and motor.angular_speed > NULL_ANGULAR_SPEED)):
             self.__powertrain_is_locked = True
             return
 
         if motor.torque is not None:
             if (motor.torque > NULL_TORQUE and motor.pwm > 0) or (motor.torque < NULL_TORQUE and motor.pwm < 0):
                 self.__powertrain_is_locked = False
 
     def _compute_locked_powertrain_angular_speed_and_acceleration(self):
 
-        for element in self.powertrain.elements:
+        for element in self.__powertrain.elements:
             element.angular_speed = NULL_ANGULAR_SPEED
             element.angular_acceleration = NULL_ANGULAR_ACCELERATION
```

### Comparing `gearpy-0.6.0/gearpy/units/unit_base.py` & `gearpy-0.7.0/gearpy/units/unit_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,34 @@
 from typing import Union
 
 
 COMPARISON_TOLERANCE = 1e-12
 
 
 class UnitBase(ABC):
+    """:py:class:`UnitBase <gearpy.units.unit_base.UnitBase>` object. \n
+    Abstract base class for creating unit objects.
+
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>` \n
+       :py:class:`Angle <gearpy.units.units.Angle>` \n
+       :py:class:`AngularPosition <gearpy.units.units.AngularPosition>` \n
+       :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>` \n
+       :py:class:`Current <gearpy.units.units.Current>` \n
+       :py:class:`Force <gearpy.units.units.Force>` \n
+       :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>` \n
+       :py:class:`Length <gearpy.units.units.Length>` \n
+       :py:class:`Stress <gearpy.units.units.Stress>` \n
+       :py:class:`Surface <gearpy.units.units.Surface>` \n
+       :py:class:`Time <gearpy.units.units.Time>` \n
+       :py:class:`TimeInterval <gearpy.units.units.TimeInterval>` \n
+       :py:class:`Torque <gearpy.units.units.Torque>`
+    """
 
     __UNITS = {}
 
     @abstractmethod
     def __init__(self, value: Union[float, int], unit: str):
         if not isinstance(value, float) and not isinstance(value, int):
             raise TypeError("Parameter 'value' must be a float or an integer.")
```

### Comparing `gearpy-0.6.0/gearpy/units/units.py` & `gearpy-0.7.0/gearpy/units/units.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from math import pi, sin, cos, tan
 from typing import Union, Optional
 from .unit_base import UnitBase
 
 
 class AngularPosition(UnitBase):
-    r"""``gearpy.units.units.AngularPosition`` object.
+    r""":py:class:`AngularPosition <gearpy.units.units.AngularPosition>` object.
 
     Attributes
     ----------
-    :py:attr:`unit` : str
+    :py:attr:`unit` : :py:class:`str`
         Symbol of the unit of measurement for angular position.
-    :py:attr:`value` : float or int
+    :py:attr:`value` : :py:class:`float` or :py:class:`int`
         Angular position numerical value.
 
     Methods
     -------
     :py:meth:`to`
-        Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
+        It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement.
     :py:meth:`sin`
-        Computes the sine of the angular position at a given frequency.
+        It computes the sine of the angular position at a given frequency.
     :py:meth:`cos`
-        Computes the cosine of the angular position at a given frequency.
+        It computes the cosine of the angular position at a given frequency.
     :py:meth:`tan`
-        Computes the tangent of the angular position at a given frequency.
+        It computes the tangent of the angular position at a given frequency.
     """
 
     __UNITS = {'rad': 1,
                'deg': pi/180,
                'arcmin': pi/180/60,
                'arcsec': pi/180/60/60,
                'rot': 2*pi}
@@ -69,101 +70,107 @@
         if isinstance(other, AngularPosition):
             return self.__value/other.to(self.__unit).value
         else:
             return AngularPosition(value = self.__value/other, unit = self.__unit)
 
     @property
     def value(self) -> Union[float, int]:
-        """Angular position numerical value. The relative unit is expressed by the ``unit`` property.
+        """Angular position numerical value. The relative unit is expressed by the :py:attr:`unit` property.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Angular position numerical value.
 
-        Raises
-        ------
-        TypeError
-            If ``value`` is not a float or an integer.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`value` is not a :py:class:`float` or an :py:class:`int`.
         """
         return self.__value
 
     @property
     def unit(self) -> str:
-        """Symbol of the unit of measurement for angular position. It must be a string.
+        """Symbol of the unit of measurement for angular position. It must be a :py:class:`str`.
         Available units are:
 
         - ``'rad'`` for radian,
         - ``'deg'`` for degree,
         - ``'arcmin'`` for minute of arc,
         - ``'arcsec'`` for second of arc,
         - ``'rot'`` for rotation.
 
         Returns
         -------
-        str
+        :py:class:`str`
             Symbol of the unit of measurement for angular position.
 
-        Raises
-        ------
-        TypeError
-            If ``unit`` is not a string.
-        KeyError
-            If the ``unit`` is not among available ones.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`unit` is not a :py:class:`str`.
+           ``KeyError``
+               If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
     def to(self, target_unit: str, inplace: bool = False) -> 'AngularPosition':
-        """Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
-        If ``inplace`` is ``True``, it overrides actual ``value`` and ``unit``, otherwise it returns a new instance with
-        the converted ``value`` and the ``target_unit`` as ``unit``.
+        """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement. \n
+        If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
+        instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
-        target_unit : str
+        ``target_unit`` : :py:class:`str`
             Target unit to which convert the current value.
-        inplace : bool, optional
+        ``inplace`` : :py:class:`bool`, optional
             Whether to override the current instance value. Default is ``False``, so it does not override the current
             value.
 
         Returns
         -------
-        AngularPosition
+        :py:class:`AngularPosition <gearpy.units.units.AngularPosition>`
             Converted angular position.
 
-        Raises
-        ------
-        TypeError
-            - If ``target_unit`` is not a string,
-            - if ``inplace`` is not a bool.
-        KeyError
-            If the ``target_unit`` is not among available ones.
-
-        Examples
-        --------
-        ``AngularPosition`` instantiation.
-
-        >>> from gearpy.units import AngularPosition
-        >>> p = AngularPosition(180, 'deg')
-        >>> p
-        ... 180 deg
-
-        Conversion from degree to radian with ``inplace = False`` by default, so it does not override the current value.
-
-        >>> p.to('rad')
-        ... 3.141592653589793 rad
-        >>> p
-        ... 180 deg
-
-        Conversion from degree to minute of arc with ``inplace = True``, in order to override the current value.
-
-        >>> p.to('arcmin', inplace = True)
-        ... 10800.0 arcmin
-        >>> p
-        ... 10800.0 arcmin
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If ``target_unit`` is not a :py:class:`str`,
+               - if ``inplace`` is not a :py:class:`bool`.
+           ``KeyError``
+               If the ``target_unit`` is not among available ones.
+
+        .. admonition:: Examples
+           :class: important
+
+           ``AngularPosition`` instantiation.
+
+           >>> from gearpy.units import AngularPosition
+           >>> p = AngularPosition(180, 'deg')
+           >>> p
+           ... 180 deg
+
+           Conversion from degree to radian with ``inplace = False`` by default, so it does not override the current
+           value.
+
+           >>> p.to('rad')
+           ... 3.141592653589793 rad
+           >>> p
+           ... 180 deg
+
+           Conversion from degree to minute of arc with ``inplace = True``, in order to override the current value.
+
+           >>> p.to('arcmin', inplace = True)
+           ... 10800.0 arcmin
+           >>> p
+           ... 10800.0 arcmin
         """
         super().to(target_unit = target_unit, inplace = inplace)
 
         if target_unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{target_unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
@@ -176,79 +183,80 @@
             self.__value = target_value
             self.__unit = target_unit
             return self
         else:
             return AngularPosition(value = target_value, unit = target_unit)
 
     def sin(self, frequency: Optional[Union[float, int]] = 1/2/pi) -> float:
-        """Computes the sine of the angular position at a given frequency.
+        r"""It computes the sine of the angular position at a given frequency.
 
         Parameters
         ----------
-        frequency : float or int, optional
-            Frequency to multiply by before computing the sine.
+        ``frequency`` : :py:class:`float` or :py:class:`int`, optional
+            Frequency to multiply by before computing the sine. Default is :math:`\frac{1}{2 \pi}`.
 
         Returns
         -------
-        float
+        :py:class:`float`
             Computed sine of the angular position.
         """
         return sin(2*pi*frequency*self.to('rad').value)
 
     def cos(self, frequency: Optional[Union[float, int]] = 1/2/pi) -> float:
-        """Computes the cosine of the angular position at a given frequency.
+        r"""It computes the cosine of the angular position at a given frequency.
 
         Parameters
         ----------
-        frequency : float or int, optional
-            Frequency to multiply by before computing the cosine.
+        ``frequency`` : :py:class:`float` or :py:class:`int`, optional
+            Frequency to multiply by before computing the cosine. Default is :math:`\frac{1}{2 \pi}`.
 
         Returns
         -------
-        float
+        :py:class:`float`
             Computed cosine of the angular position.
         """
         return cos(2*pi*frequency*self.to('rad').value)
 
     def tan(self, frequency: Optional[Union[float, int]] = 1/2/pi) -> float:
-        """Computes the tangent of the angular position at a given frequency.
+        r"""It computes the tangent of the angular position at a given frequency.
 
         Parameters
         ----------
-        frequency : float or int, optional
-            Frequency to multiply by before computing the tangent.
+        ``frequency`` : :py:class:`float` or :py:class:`int`, optional
+            Frequency to multiply by before computing the tangent. Default is :math:`\frac{1}{2 \pi}`.
 
         Returns
         -------
-        float
+        :py:class:`float`
             Computed tangent of the angular position.
         """
         return tan(2*pi*frequency*self.to('rad').value)
 
 
 class Angle(AngularPosition):
-    r"""``gearpy.units.units.Angle`` object.
+    r""":py:class:`Angle <gearpy.units.units.Angle>` object.
 
     Attributes
     ----------
-    :py:attr:`unit` : str
+    :py:attr:`unit` : :py:class:`str`
         Symbol of the unit of measurement for angle.
-    :py:attr:`value` : float or int
+    :py:attr:`value` : :py:class:`float` or :py:class:`int`
         Angle numerical value.
 
     Methods
     -------
     :py:meth:`to`
-        Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
+        It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement.
     :py:meth:`sin`
-        Computes the sine of the angle at a given frequency.
+        It computes the sine of the angle at a given frequency.
     :py:meth:`cos`
-        Computes the cosine of the angle at a given frequency.
+        It computes the cosine of the angle at a given frequency.
     :py:meth:`tan`
-        Computes the tangent of the angle at a given frequency.
+        It computes the tangent of the angle at a given frequency.
     """
 
     def __init__(self, value: Union[float, int], unit: str):
         super().__init__(value = value, unit = unit)
 
         if value < 0:
             raise ValueError("Parameter 'value' must be positive or null.")
@@ -294,173 +302,181 @@
         if isinstance(other, AngularPosition):
             return self.__value/other.to(self.__unit).value
         else:
             return Angle(value = self.__value/other, unit = self.__unit)
 
     @property
     def value(self) -> Union[float, int]:
-        """Angle numerical value. The relative unit is expressed by the ``unit`` property. It must be positive or null.
+        """Angle numerical value. The relative unit is expressed by the :py:attr:`unit` property. It must be positive or
+        null.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Angle numerical value.
 
-        Raises
-        ------
-        TypeError
-            If ``value`` is not a float or an integer.
-        ValueError
-            If ``value`` is negative.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`value` is not a :py:class:`float` or an :py:class:`int`.
+           ``ValueError``
+               If :py:attr:`value` is negative.
         """
         return super().value
 
     @property
     def unit(self) -> str:
-        """Symbol of the unit of measurement for angle. It must be a string.
+        """Symbol of the unit of measurement for angle. It must be a :py:class:`str`.
         Available units are:
 
         - ``'rad'`` for radian,
         - ``'deg'`` for degree,
         - ``'arcmin'`` for minute of arc,
         - ``'arcsec'`` for second of arc,
         - ``'rot'`` for rotation.
 
         Returns
         -------
-        str
+        :py:class:`str`
             Symbol of the unit of measurement for angle.
 
-        Raises
-        ------
-        TypeError
-            If ``unit`` is not a string.
-        KeyError
-            If the ``unit`` is not among available ones.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`unit` is not a :py:class:`str`.
+           ``KeyError``
+               If the :py:attr:`unit` is not among available ones.
         """
         return super().unit
 
     def to(self, target_unit: str, inplace: bool = False) -> 'Angle':
-        """Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
-        If ``inplace`` is ``True``, it overrides actual ``value`` and ``unit``, otherwise it returns a new instance with
-        the converted ``value`` and the ``target_unit`` as ``unit``.
+        """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement. \n
+        If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
+        instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
-        target_unit : str
+        ``target_unit`` : :py:class:`str`
             Target unit to which convert the current value.
-        inplace : bool, optional
+        ``inplace`` : :py:class:`bool`, optional
             Whether to override the current instance value. Default is ``False``, so it does not override the current
             value.
 
         Returns
         -------
-        Angle
+        :py:class:`Angle <gearpy.units.units.Angle>`
             Converted angle.
 
-        Raises
-        ------
-        TypeError
-            - If ``target_unit`` is not a string,
-            - if ``inplace`` is not a bool.
-        KeyError
-            If the ``target_unit`` is not among available ones.
-
-        Examples
-        --------
-        ``Angle`` instantiation.
-
-        >>> from gearpy.units import Angle
-        >>> a = Angle(180, 'deg')
-        >>> a
-        ... 180 deg
-
-        Conversion from degree to radian with ``inplace = False`` by default, so it does not override the current value.
-
-        >>> a.to('rad')
-        ... 3.141592653589793 rad
-        >>> a
-        ... 180 deg
-
-        Conversion from degree to minute of arc with ``inplace = True``, in order to override the current value.
-
-        >>> a.to('arcmin', inplace = True)
-        ... 10800.0 arcmin
-        >>> a
-        ... 10800.0 arcmin
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If ``target_unit`` is not a :py:class:`str`,
+               - if ``inplace`` is not a :py:class:`bool`.
+           ``KeyError``
+               If the ``target_unit`` is not among available ones.
+
+        .. admonition:: Examples
+           :class: important
+
+           ``Angle`` instantiation.
+
+           >>> from gearpy.units import Angle
+           >>> a = Angle(180, 'deg')
+           >>> a
+           ... 180 deg
+
+           Conversion from degree to radian with ``inplace = False`` by default, so it does not override the current
+           value.
+
+           >>> a.to('rad')
+           ... 3.141592653589793 rad
+           >>> a
+           ... 180 deg
+
+           Conversion from degree to minute of arc with ``inplace = True``, in order to override the current value.
+
+           >>> a.to('arcmin', inplace = True)
+           ... 10800.0 arcmin
+           >>> a
+           ... 10800.0 arcmin
         """
         converted = super().to(target_unit = target_unit, inplace = inplace)
 
         if inplace:
             self.__value = converted.value
             self.__unit = converted.unit
             return self
         else:
             return Angle(value = converted.value, unit = converted.unit)
 
     def sin(self, frequency: Optional[Union[float, int]] = 1/2/pi) -> float:
-        """Computes the sine of the angle at a given frequency.
+        r"""It computes the sine of the angle at a given frequency.
 
         Parameters
         ----------
-        frequency : float or int, optional
-            Frequency to multiply by before computing the sine.
+        ``frequency`` : :py:class:`float` or :py:class:`int`, optional
+            Frequency to multiply by before computing the sine. Default is :math:`\frac{1}{2 \pi}`.
 
         Returns
         -------
-        float
+        :py:class:`float`
             Computed sine of the angle.
         """
         return super().sin(frequency = frequency)
 
     def cos(self, frequency: Optional[Union[float, int]] = 1/2/pi) -> float:
-        """Computes the cosine of the angle at a given frequency.
+        r"""It computes the cosine of the angle at a given frequency.
 
         Parameters
         ----------
-        frequency : float or int, optional
-            Frequency to multiply by before computing the cosine.
+        ``frequency`` : :py:class:`float` or :py:class:`int`, optional
+            Frequency to multiply by before computing the cosine. Default is :math:`\frac{1}{2 \pi}`.
 
         Returns
         -------
-        float
+        :py:class:`float`
             Computed cosine of the angle.
         """
         return super().cos(frequency = frequency)
 
     def tan(self, frequency: Optional[Union[float, int]] = 1/2/pi) -> float:
-        """Computes the tangent of the angle at a given frequency.
+        r"""It computes the tangent of the angle at a given frequency.
 
         Parameters
         ----------
-        frequency : float or int, optional
-            Frequency to multiply by before computing the tangent.
+        ``frequency`` : :py:class:`float` or :py:class:`int`, optional
+            Frequency to multiply by before computing the tangent. Default is :math:`\frac{1}{2 \pi}`.
 
         Returns
         -------
-        float
+        :py:class:`float`
             Computed tangent of the angle.
         """
         return super().tan(frequency = frequency)
 
 
 class AngularSpeed(UnitBase):
-    r"""``gearpy.units.units.AngularSpeed`` object.
+    r""":py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>` object.
 
     Attributes
     ----------
-    :py:attr:`unit` : str
+    :py:attr:`unit` : :py:class:`str`
         Symbol of the unit of measurement for angular speed.
-    :py:attr:`value` : float or int
+    :py:attr:`value` : :py:class:`float` or :py:class:`int`
         Angular speed numerical value.
 
     Methods
     -------
     :py:meth:`to`
-        Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
+        It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement.
     """
 
     __UNITS = {'rad/s': 1,
                'rad/min': 1/60,
                'rad/h': 1/60/60,
                'deg/s': pi/180,
                'deg/min': pi/180/60,
@@ -512,107 +528,112 @@
         if isinstance(other, AngularSpeed):
             return self.__value/other.to(self.__unit).value
         else:
             return AngularSpeed(value = self.__value/other, unit = self.__unit)
 
     @property
     def value(self) -> Union[float, int]:
-        """Angular speed numerical value. The relative unit is expressed by the ``unit`` property.
+        """Angular speed numerical value. The relative unit is expressed by the :py:attr:`unit` property.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Angular speed numerical value.
 
-        Raises
-        ------
-        TypeError
-            If ``value`` is not a float or an integer.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`value` is not a :py:class:`float` or an :py:class:`int`.
         """
         return self.__value
 
     @property
     def unit(self) -> str:
-        """Symbol of the unit of measurement for angular speed. It must be a string.
+        """Symbol of the unit of measurement for angular speed. It must be a :py:class:`str`.
         Available units are:
 
         - ``'rad/s'`` for radian per second,
         - ``'rad/min'`` for radian per minute,
         - ``'rad/h'`` for radian per hour,
         - ``'deg/s'`` for degree per second,
         - ``'deg/min'`` for degree per minute,
         - ``'deg/h'`` for degree per hour,
         - ``'rps'`` for revolutions per second,
         - ``'rpm'`` for revolutions per minute,
         - ``'rph'`` for revolutions per hour.
 
         Returns
         -------
-        str
+        :py:class:`str`
             Symbol of the unit of measurement for angular speed.
 
-        Raises
-        ------
-        TypeError
-            If ``unit`` is not a string.
-        KeyError
-            If the ``unit`` is not among available ones.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`unit` is not a :py:class:`str`.
+           ``KeyError``
+               If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
     def to(self, target_unit: str, inplace: bool = False) -> 'AngularSpeed':
-        """Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
-        If ``inplace`` is ``True``, it overrides actual ``value`` and ``unit``, otherwise it returns a new instance with
-        the converted ``value`` and the ``target_unit`` as ``unit``.
+        """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement. \n
+        If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
+        instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
-        target_unit : str
+        ``target_unit`` : :py:class:`str`
             Target unit to which convert the current value.
-        inplace : bool, optional
+        ``inplace`` : :py:class:`bool`, optional
             Whether to override the current instance value. Default is ``False``, so it does not override the current
             value.
 
         Returns
         -------
-        AngularSpeed
+        :py:class:`AngularSpeed <gearpy.units.units.AngularSpeed>`
             Converted angular speed.
 
-        Raises
-        ------
-        TypeError
-            - If ``target_unit`` is not a string,
-            - if ``inplace`` is not a bool.
-        KeyError
-            If the ``target_unit`` is not among available ones.
-
-        Examples
-        --------
-        ``AngularSpeed`` instantiation.
-
-        >>> from gearpy.units import AngularSpeed
-        >>> s = AngularSpeed(1000, 'rpm')
-        >>> s
-        ... 1000 rpm
-
-        Conversion from revolutions per minute to radian per second with ``inplace = False`` by default, so it does not
-        override the current value.
-
-        >>> s.to('rad/s')
-        ... 104.71975511965977 rad/s
-        >>> s
-        ... 1000 rpm
-
-        Conversion from revolutions per minute to revolutions per second with ``inplace = True``, in order to override
-        the current value.
-
-        >>> s.to('rps', inplace = True)
-        ... 16.666666666666664 rps
-        >>> s
-        ... 16.666666666666664 rps
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If ``target_unit`` is not a :py:class:`str`,
+               - if ``inplace`` is not a :py:class:`bool`.
+           ``KeyError``
+               If the ``target_unit`` is not among available ones.
+
+        .. admonition:: Examples
+           :class: important
+
+           ``AngularSpeed`` instantiation.
+
+           >>> from gearpy.units import AngularSpeed
+           >>> s = AngularSpeed(1000, 'rpm')
+           >>> s
+           ... 1000 rpm
+
+           Conversion from revolutions per minute to radian per second with ``inplace = False`` by default, so it does
+           not override the current value.
+
+           >>> s.to('rad/s')
+           ... 104.71975511965977 rad/s
+           >>> s
+           ... 1000 rpm
+
+           Conversion from revolutions per minute to revolutions per second with ``inplace = True``, in order to
+           override the current value.
+
+           >>> s.to('rps', inplace = True)
+           ... 16.666666666666664 rps
+           >>> s
+           ... 16.666666666666664 rps
         """
         super().to(target_unit = target_unit, inplace = inplace)
 
         if target_unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{target_unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
@@ -626,27 +647,28 @@
             self.__unit = target_unit
             return self
         else:
             return AngularSpeed(value = target_value, unit = target_unit)
 
 
 class AngularAcceleration(UnitBase):
-    r"""``gearpy.units.units.AngularAcceleration`` object.
+    r""":py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>` object.
 
     Attributes
     ----------
-    :py:attr:`unit` : str
+    :py:attr:`unit` : :py:class:`str`
         Symbol of the unit of measurement for angular acceleration.
-    :py:attr:`value` : float or int
+    :py:attr:`value` : :py:class:`float` or :py:class:`int`
         Angular acceleration numerical value.
 
     Methods
     -------
     :py:meth:`to`
-        Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
+        It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement.
     """
 
     __UNITS = {'rad/s^2': 1,
                'deg/s^2': pi/180,
                'rot/s^2': 2*pi}
 
     def __init__(self, value: Union[float, int], unit: str):
@@ -693,101 +715,106 @@
         if isinstance(other, AngularAcceleration):
             return self.__value/other.to(self.__unit).value
         else:
             return AngularAcceleration(value = self.__value/other, unit = self.__unit)
 
     @property
     def value(self) -> Union[float, int]:
-        """Angular acceleration numerical value. The relative unit is expressed by the ``unit`` property.
+        """Angular acceleration numerical value. The relative unit is expressed by the :py:attr:`unit` property.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Angular acceleration numerical value.
 
-        Raises
-        ------
-        TypeError
-            If ``value`` is not a float or an integer.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`value` is not a :py:class:`float` or an :py:class:`int`.
         """
         return self.__value
 
     @property
     def unit(self) -> str:
-        """Symbol of the unit of measurement for angular acceleration. It must be a string.
+        """Symbol of the unit of measurement for angular acceleration. It must be a :py:class:`str`.
         Available units are:
 
         - ``'rad/s^2'`` for radian per second squared,
         - ``'deg/s^2'`` for degree per second squared,
         - ``'rot/s^2'`` for rotation per second squared.
 
         Returns
         -------
-        str
+        :py:class:`str`
             Symbol of the unit of measurement for angular acceleration.
 
-        Raises
-        ------
-        TypeError
-            If ``unit`` is not a string.
-        KeyError
-            If the ``unit`` is not among available ones.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`unit` is not a :py:class:`str`.
+           ``KeyError``
+               If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
     def to(self, target_unit: str, inplace: bool = False) -> 'AngularAcceleration':
-        """Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
-        If ``inplace`` is ``True``, it overrides actual ``value`` and ``unit``, otherwise it returns a new instance with
-        the converted ``value`` and the ``target_unit`` as ``unit``.
+        """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement. \n
+        If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
+        instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
-        target_unit : str
+        ``target_unit`` : :py:class:`str`
             Target unit to which convert the current value.
-        inplace : bool, optional
+        ``inplace`` : :py:class:`bool`, optional
             Whether to override the current instance value. Default is ``False``, so it does not override the current
             value.
 
         Returns
         -------
-        AngularAcceleration
+        :py:class:`AngularAcceleration <gearpy.units.units.AngularAcceleration>`
             Converted angular acceleration.
 
-        Raises
-        ------
-        TypeError
-            - If ``target_unit`` is not a string,
-            - if ``inplace`` is not a bool.
-        KeyError
-            If the ``target_unit`` is not among available ones.
-
-        Examples
-        --------
-        ``AngularAcceleration`` instantiation.
-
-        >>> from gearpy.units import AngularAcceleration
-        >>> a = AngularAcceleration(180, 'deg/s^2')
-        >>> a
-        ... 180 deg/s^2
-
-        Conversion from degree per second squared to radian per second squared with ``inplace = False`` by default, so
-        it does not override the current value.
-
-        >>> a.to('rad/s^2')
-        ... 3.141592653589793 rad/s^2
-        >>> a
-        ... 180 deg/s^2
-
-        Conversion from degree per second squared to radian per second squared with ``inplace = True``, in order to
-        override the current value.
-
-        >>> a.to('rad/s^2', inplace = True)
-        ... 3.141592653589793 rad/s^2
-        >>> a
-        ... 3.141592653589793 rad/s^2
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If ``target_unit`` is not a :py:class:`str`,
+               - if ``inplace`` is not a :py:class:`bool`.
+           ``KeyError``
+               If the ``target_unit`` is not among available ones.
+
+        .. admonition:: Examples
+           :class: important
+
+           ``AngularAcceleration`` instantiation.
+
+           >>> from gearpy.units import AngularAcceleration
+           >>> a = AngularAcceleration(180, 'deg/s^2')
+           >>> a
+           ... 180 deg/s^2
+
+           Conversion from degree per second squared to radian per second squared with ``inplace = False`` by default,
+           so it does not override the current value.
+
+           >>> a.to('rad/s^2')
+           ... 3.141592653589793 rad/s^2
+           >>> a
+           ... 180 deg/s^2
+
+           Conversion from degree per second squared to radian per second squared with ``inplace = True``, in order to
+           override the current value.
+
+           >>> a.to('rad/s^2', inplace = True)
+           ... 3.141592653589793 rad/s^2
+           >>> a
+           ... 3.141592653589793 rad/s^2
         """
         super().to(target_unit = target_unit, inplace = inplace)
 
         if target_unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{target_unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
@@ -801,27 +828,28 @@
             self.__unit = target_unit
             return self
         else:
             return AngularAcceleration(value = target_value, unit = target_unit)
 
 
 class InertiaMoment(UnitBase):
-    r"""``gearpy.units.units.InertiaMoment`` object.
+    r""":py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>` object.
 
     Attributes
     ----------
-    :py:attr:`unit` : str
+    :py:attr:`unit` : :py:class:`str`
         Symbol of the unit of measurement for moment of inertia.
-    :py:attr:`value` : float or int
+    :py:attr:`value` : :py:class:`float` or :py:class:`int`
         Moment of inertia numerical value.
 
     Methods
     -------
     :py:meth:`to`
-        Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
+        It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement.
     """
 
     __UNITS = {'kgm^2': 1,
                'kgdm^2': 1e-2,
                'kgcm^2': 1e-4,
                'kgmm^2': 1e-6,
                'gm^2': 1e-3,
@@ -876,109 +904,114 @@
         if isinstance(other, InertiaMoment):
             return self.__value/other.to(self.__unit).value
         else:
             return InertiaMoment(value = self.__value/other, unit = self.__unit)
 
     @property
     def value(self) -> Union[float, int]:
-        """Moment of inertia numerical value. The relative unit is expressed by the ``unit`` property. It must be
+        """Moment of inertia numerical value. The relative unit is expressed by the :py:attr:`unit` property. It must be
         positive.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Moment of inertia numerical value.
 
-        Raises
-        ------
-        TypeError
-            If ``value`` is not a float or an integer.
-        ValueError
-            If ``value`` is negative or null.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`value` is not a :py:class:`float` or an :py:class:`int`.
+           ``ValueError``
+               If :py:attr:`value` is negative or null.
         """
         return self.__value
 
     @property
     def unit(self) -> str:
-        """Symbol of the unit of measurement for moment of inertia. It must be a string.
+        """Symbol of the unit of measurement for moment of inertia. It must be a :py:class:`str`.
         Available units are:
 
         - ``'kgm^2'`` for kilogram-square meter,
         - ``'kgdm^2'`` for kilogram-square decimeter,
         - ``'kgcm^2'`` for kilogram-square centimeter,
         - ``'kgmm^2'`` for kilogram-square millimeter,
         - ``'gm^2'`` for gram-square meter,
         - ``'gdm^2'`` for gram-square decimeter,
         - ``'gcm^2'`` for gram-square centimeter,
         - ``'gmm^2'`` for gram-square millimeter.
 
         Returns
         -------
-        str
+        :py:class:`str`
             Symbol of the unit of measurement for moment of inertia.
 
-        Raises
-        ------
-        TypeError
-            If ``unit`` is not a string.
-        KeyError
-            If the ``unit`` is not among available ones.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`unit` is not a :py:class:`str`.
+           ``KeyError``
+               If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
     def to(self, target_unit: str, inplace: bool = False) -> 'InertiaMoment':
-        """Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
-        If ``inplace`` is ``True``, it overrides actual ``value`` and ``unit``, otherwise it returns a new instance with
-        the converted ``value`` and the ``target_unit`` as ``unit``.
+        """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement. \n
+        If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
+        instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
-        target_unit : str
+        ``target_unit`` : :py:class:`str`
             Target unit to which convert the current value.
-        inplace : bool, optional
+        ``inplace`` : :py:class:`bool`, optional
             Whether to override the current instance value. Default is ``False``, so it does not override the current
             value.
 
         Returns
         -------
-        InertiaMoment
+        :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`
             Converted moment of inertia.
 
-        Raises
-        ------
-        TypeError
-            - If ``target_unit`` is not a string,
-            - if ``inplace`` is not a bool.
-        KeyError
-            If the ``target_unit`` is not among available ones.
-
-        Examples
-        --------
-        ``InertiaMoment`` instantiation.
-
-        >>> from gearpy.units import InertiaMoment
-        >>> i = InertiaMoment(1, 'kgm^2')
-        >>> i
-        ... 1 kgm^2
-
-        Conversion from kilogram-square meter to gram-square meter with ``inplace = False`` by default, so it does not
-        override the current value.
-
-        >>> i.to('gm^2')
-        ... 1000.0 gm^2
-        >>> i
-        ... 1 kgm^2
-
-        Conversion from kilograms-square meter to gram-square meter with ``inplace = True``, in order to override the
-        current value.
-
-        >>> i.to('gm^2', inplace = True)
-        ... 1000.0 gm^2
-        >>> i
-        ... 1000.0 gm^2
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If ``target_unit`` is not a :py:class:`str`,
+               - if ``inplace`` is not a :py:class:`bool`.
+           ``KeyError``
+               If the ``target_unit`` is not among available ones.
+
+        .. admonition:: Examples
+           :class: important
+
+           ``InertiaMoment`` instantiation.
+
+           >>> from gearpy.units import InertiaMoment
+           >>> i = InertiaMoment(1, 'kgm^2')
+           >>> i
+           ... 1 kgm^2
+
+           Conversion from kilogram-square meter to gram-square meter with ``inplace = False`` by default, so it does
+           not override the current value.
+
+           >>> i.to('gm^2')
+           ... 1000.0 gm^2
+           >>> i
+           ... 1 kgm^2
+
+           Conversion from kilograms-square meter to gram-square meter with ``inplace = True``, in order to override the
+           current value.
+
+           >>> i.to('gm^2', inplace = True)
+           ... 1000.0 gm^2
+           >>> i
+           ... 1000.0 gm^2
         """
         super().to(target_unit = target_unit, inplace = inplace)
 
         if target_unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{target_unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
@@ -992,27 +1025,28 @@
             self.__unit = target_unit
             return self
         else:
             return InertiaMoment(value = target_value, unit = target_unit)
 
 
 class Torque(UnitBase):
-    r"""``gearpy.units.units.Torque`` object.
+    r""":py:class:`Torque <gearpy.units.units.Torque>` object.
 
     Attributes
     ----------
-    :py:attr:`unit` : str
+    :py:attr:`unit` : :py:class:`str`
         Symbol of the unit of measurement for torque.
-    :py:attr:`value` : float or int
+    :py:attr:`value` : :py:class:`float` or :py:class:`int`
         Torque numerical value.
 
     Methods
     -------
     :py:meth:`to`
-        Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
+        It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement.
     """
 
     __UNITS = {'Nm': 1,
                'mNm': 1e-3,
                'mNdm': 1e-4,
                'mNcm': 1e-5,
                'mNmm': 1e-6,
@@ -1072,31 +1106,32 @@
         elif isinstance(other, Torque):
             return self.__value/other.to(self.__unit).value
         else:
             return Torque(value = self.__value/other, unit = self.__unit)
 
     @property
     def value(self) -> Union[float, int]:
-        """Torque numerical value. The relative unit is expressed by the ``unit`` property.
+        """Torque numerical value. The relative unit is expressed by the :py:attr:`unit` property.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Torque numerical value.
 
-        Raises
-        ------
-        TypeError
-            If ``value`` is not a float or an integer.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`value` is not a :py:class:`float` or an :py:class:`int`.
         """
         return self.__value
 
     @property
     def unit(self) -> str:
-        """Symbol of the unit of measurement for Torque. It must be a string.
+        """Symbol of the unit of measurement for Torque. It must be a :py:class:`str`.
         Available units are:
 
         - ``'Nm'`` for newton-meter,
         - ``'mNm'`` for milli-newton-meter,
         - ``'mNdm'`` for milli-newton-decimeter,
         - ``'mNcm'`` for milli-newton-centimeter,
         - ``'mNmm'`` for milli-newton-millimeter,
@@ -1111,76 +1146,80 @@
         - ``'gfm'`` for gram force-meter,
         - ``'gfdm'`` for gram force-decimeter,
         - ``'gfcm'`` for gram force-centimeter,
         - ``'gfmm'`` for gram force-millimeter.
 
         Returns
         -------
-        str
+        :py:class:`str`
             Symbol of the unit of measurement for torque.
 
-        Raises
-        ------
-        TypeError
-            If ``unit`` is not a string.
-        KeyError
-            If the ``unit`` is not among available ones.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`unit` is not a :py:class:`str`.
+           ``KeyError``
+               If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
     def to(self, target_unit: str, inplace: bool = False) -> 'Torque':
-        """Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
-        If ``inplace`` is ``True``, it overrides actual ``value`` and ``unit``, otherwise it returns a new instance with
-        the converted ``value`` and the ``target_unit`` as ``unit``.
+        """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement. \n
+        If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
+        instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
-        target_unit : str
+        ``target_unit`` : :py:class:`str`
             Target unit to which convert the current value.
-        inplace : bool, optional
+        ``inplace`` : :py:class:`bool`, optional
             Whether to override the current instance value. Default is ``False``, so it does not override the current
             value.
 
         Returns
         -------
-        Torque
+        :py:class:`Torque <gearpy.units.units.Torque>`
             Converted torque.
 
-        Raises
-        ------
-        TypeError
-            - If ``target_unit`` is not a string,
-            - if ``inplace`` is not a bool.
-        KeyError
-            If the ``target_unit`` is not among available ones.
-
-        Examples
-        --------
-        ``Torque`` instantiation.
-
-        >>> from gearpy.units import Torque
-        >>> T = Torque(1, 'Nm')
-        >>> T
-        ... 1 Nm
-
-        Conversion from newton-meter to kilogram force-meter with ``inplace = False`` by default, so it does not
-        override the current value.
-
-        >>> T.to('kgfm')
-        ... 0.10197162129779283 kgfm
-        >>> T
-        ... 1 Nm
-
-        Conversion from newton-meter to kilogram force-meter with ``inplace = True``, in order to override the current
-        value.
-
-        >>> T.to('kgfm', inplace = True)
-        ... 0.10197162129779283 kgfm
-        >>> T
-        ... 0.10197162129779283 kgfm
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If ``target_unit`` is not a :py:class:`str`,
+               - if ``inplace`` is not a :py:class:`bool`.
+           ``KeyError``
+               If the ``target_unit`` is not among available ones.
+
+        .. admonition:: Examples
+           :class: important
+
+           ``Torque`` instantiation.
+
+           >>> from gearpy.units import Torque
+           >>> T = Torque(1, 'Nm')
+           >>> T
+           ... 1 Nm
+
+           Conversion from newton-meter to kilogram force-meter with ``inplace = False`` by default, so it does not
+           override the current value.
+
+           >>> T.to('kgfm')
+           ... 0.10197162129779283 kgfm
+           >>> T
+           ... 1 Nm
+
+           Conversion from newton-meter to kilogram force-meter with ``inplace = True``, in order to override the
+           current value.
+
+           >>> T.to('kgfm', inplace = True)
+           ... 0.10197162129779283 kgfm
+           >>> T
+           ... 0.10197162129779283 kgfm
         """
         super().to(target_unit = target_unit, inplace = inplace)
 
         if target_unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{target_unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
@@ -1194,27 +1233,28 @@
             self.__unit = target_unit
             return self
         else:
             return Torque(value = target_value, unit = target_unit)
 
 
 class Time(UnitBase):
-    r"""``gearpy.units.units.Time`` object.
+    r""":py:class:`Time <gearpy.units.units.Time>` object.
 
     Attributes
     ----------
-    :py:attr:`unit` : str
+    :py:attr:`unit` : :py:class:`str`
         Symbol of the unit of measurement for time.
-    :py:attr:`value` : float or int
+    :py:attr:`value` : :py:class:`float` or :py:class:`int`
         Time numerical value.
 
     Methods
     -------
     :py:meth:`to`
-        Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
+        It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement.
     """
 
     __UNITS = {'sec': 1,
                'min': 60,
                'hour': 60*60,
                'ms': 1e-3}
 
@@ -1269,100 +1309,106 @@
         if isinstance(other, Time):
             return self.__value/other.to(self.__unit).value
         else:
             return Time(value = self.__value/other, unit = self.__unit)
 
     @property
     def value(self) -> Union[float, int]:
-        """Time numerical value. The relative unit is expressed by the ``unit`` property.
+        """Time numerical value. The relative unit is expressed by the :py:attr:`unit` property.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Time numerical value.
 
-        Raises
-        ------
-        TypeError
-            If ``value`` is not a float or an integer.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`value` is not a :py:class:`float` or an :py:class:`int`.
         """
         return self.__value
 
     @property
     def unit(self) -> str:
-        """Symbol of the unit of measurement for time. It must be a string.
+        """Symbol of the unit of measurement for time. It must be a :py:class:`str`.
         Available units are:
 
         - ``'sec'`` for second,
         - ``'min'`` for minute,
         - ``'hour'`` for hour,
         - ``'ms'`` for millisecond.
 
         Returns
         -------
-        str
+        :py:class:`str`
             Symbol of the unit of measurement for time.
 
-        Raises
-        ------
-        TypeError
-            If ``unit`` is not a string.
-        KeyError
-            If the ``unit`` is not among available ones.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`unit` is not a :py:class:`str`.
+           ``KeyError``
+               If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
     def to(self, target_unit: str, inplace: bool = False) -> 'Time':
-        """Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
-        If ``inplace`` is ``True``, it overrides actual ``value`` and ``unit``, otherwise it returns a new instance with
-        the converted ``value`` and the ``target_unit`` as ``unit``.
+        """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement. \n
+        If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
+        instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
-        target_unit : str
+        ``target_unit`` : :py:class:`str`
             Target unit to which convert the current value.
-        inplace : bool, optional
+        ``inplace`` : :py:class:`bool`, optional
             Whether to override the current instance value. Default is ``False``, so it does not override the current
             value.
 
         Returns
         -------
-        Time
+        :py:class:`Time <gearpy.units.units.Time>`
             Converted time.
 
-        Raises
-        ------
-        TypeError
-            - If ``target_unit`` is not a string,
-            - if ``inplace`` is not a bool.
-        KeyError
-            If the ``target_unit`` is not among available ones.
-
-        Examples
-        --------
-        ``Time`` instantiation.
-
-        >>> from gearpy.units import Time
-        >>> t = Time(1, 'hour')
-        >>> t
-        ... 1 hour
-
-        Conversion from hour to second with ``inplace = False`` by default, so it does not override the current value.
-
-        >>> t.to('sec')
-        ... 3600.0 sec
-        >>> t
-        ... 1 hour
-
-        Conversion from hour to second with ``inplace = True``, in order to override the current value.
-
-        >>> t.to('sec', inplace = True)
-        ... 3600.0 sec
-        >>> t
-        ... 3600.0 sec
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If ``target_unit`` is not a :py:class:`str`,
+               - if ``inplace`` is not a :py:class:`bool`.
+           ``KeyError``
+               If the ``target_unit`` is not among available ones.
+
+        .. admonition:: Examples
+           :class: important
+
+           ``Time`` instantiation.
+
+           >>> from gearpy.units import Time
+           >>> t = Time(1, 'hour')
+           >>> t
+           ... 1 hour
+
+           Conversion from hour to second with ``inplace = False`` by default, so it does not override the current
+           value.
+
+           >>> t.to('sec')
+           ... 3600.0 sec
+           >>> t
+           ... 1 hour
+
+           Conversion from hour to second with ``inplace = True``, in order to override the current value.
+
+           >>> t.to('sec', inplace = True)
+           ... 3600.0 sec
+           >>> t
+           ... 3600.0 sec
         """
         super().to(target_unit = target_unit, inplace = inplace)
 
         if target_unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{target_unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
@@ -1376,27 +1422,28 @@
             self.__unit = target_unit
             return self
         else:
             return Time(value = target_value, unit = target_unit)
 
 
 class TimeInterval(Time):
-    r"""``gearpy.units.units.TimeInterval`` object.
+    r""":py:class:`TimeInterval <gearpy.units.units.TimeInterval>` object.
 
     Attributes
     ----------
-    :py:attr:`unit` : str
+    :py:attr:`unit` : :py:class:`str`
         Symbol of the unit of measurement for time interval.
-    :py:attr:`value` : float or int
+    :py:attr:`value` : :py:class:`float` or :py:class:`int`
         Time interval numerical value.
 
     Methods
     -------
     :py:meth:`to`
-        Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
+        It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement.
     """
 
     def __init__(self, value: Union[float, int], unit: str):
         super().__init__(value = value, unit = unit)
 
         if value <= 0:
             raise ValueError("Parameter 'value' must be positive.")
@@ -1442,127 +1489,135 @@
         if isinstance(other, Time):
             return self.__value/other.to(self.__unit).value
         else:
             return TimeInterval(value = self.__value/other, unit = self.__unit)
 
     @property
     def value(self) -> Union[float, int]:
-        """Time interval numerical value. The relative unit is expressed by the ``unit`` property. It must be positive.
+        """Time interval numerical value. The relative unit is expressed by the :py:attr:`unit` property. It must be
+        positive.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Time interval numerical value.
 
-        Raises
-        ------
-        TypeError
-            If ``value`` is not a float or an integer.
-        ValueError
-            If ``value`` is negative or null.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`value` is not a :py:class:`float` or an :py:class:`int`.
+           ``ValueError``
+               If :py:attr:`value` is negative or null.
         """
         return super().value
 
     @property
     def unit(self) -> str:
-        """Symbol of the unit of measurement for time interval. It must be a string.
+        """Symbol of the unit of measurement for time interval. It must be a :py:class:`str`.
         Available units are:
 
         - ``'sec'`` for second,
         - ``'min'`` for minute,
         - ``'hour'`` for hour,
         - ``'ms'`` for millisecond.
 
         Returns
         -------
-        str
+        :py:class:`str`
             Symbol of the unit of measurement for time interval.
 
-        Raises
-        ------
-        TypeError
-            If ``unit`` is not a string.
-        KeyError
-            If the ``unit`` is not among available ones.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`unit` is not a :py:class:`str`.
+           ``KeyError``
+               If the :py:attr:`unit` is not among available ones.
         """
         return super().unit
 
     def to(self, target_unit: str, inplace: bool = False) -> 'TimeInterval':
-        """Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
-        If ``inplace`` is ``True``, it overrides actual ``value`` and ``unit``, otherwise it returns a new instance with
-        the converted ``value`` and the ``target_unit`` as ``unit``.
+        """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement. \n
+        If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
+        instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
-        target_unit : str
+        ``target_unit`` : :py:class:`str`
             Target unit to which convert the current value.
-        inplace : bool, optional
+        ``inplace`` : :py:class:`bool`, optional
             Whether to override the current instance value. Default is ``False``, so it does not override the current
             value.
 
         Returns
         -------
-        TimeInterval
+        :py:class:`TimeInterval <gearpy.units.units.TimeInterval>`
             Converted time interval.
 
-        Raises
-        ------
-        TypeError
-            - If ``target_unit`` is not a string,
-            - if ``inplace`` is not a bool.
-        KeyError
-            If the ``target_unit`` is not among available ones.
-
-        Examples
-        --------
-        ``TimeInterval`` instantiation.
-
-        >>> from gearpy.units import TimeInterval
-        >>> dt = TimeInterval(1, 'hour')
-        >>> dt
-        ... 1 hour
-
-        Conversion from hour to second with ``inplace = False`` by default, so it does not override the current value.
-
-        >>> dt.to('sec')
-        ... 3600.0 sec
-        >>> dt
-        ... 1 hour
-
-        Conversion from hour to second with ``inplace = True``, in order to override the current value.
-
-        >>> dt.to('sec', inplace = True)
-        ... 3600.0 sec
-        >>> dt
-        ... 3600.0 sec
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If ``target_unit`` is not a :py:class:`str`,
+               - if ``inplace`` is not a :py:class:`bool`.
+           ``KeyError``
+               If the ``target_unit`` is not among available ones.
+
+        .. admonition:: Examples
+           :class: important
+
+           ``TimeInterval`` instantiation.
+
+           >>> from gearpy.units import TimeInterval
+           >>> dt = TimeInterval(1, 'hour')
+           >>> dt
+           ... 1 hour
+
+           Conversion from hour to second with ``inplace = False`` by default, so it does not override the current
+           value.
+
+           >>> dt.to('sec')
+           ... 3600.0 sec
+           >>> dt
+           ... 1 hour
+
+           Conversion from hour to second with ``inplace = True``, in order to override the current value.
+
+           >>> dt.to('sec', inplace = True)
+           ... 3600.0 sec
+           >>> dt
+           ... 3600.0 sec
         """
         converted = super().to(target_unit = target_unit, inplace = inplace)
 
         if inplace:
             self.__value = converted.value
             self.__unit = converted.unit
             return self
         else:
             return TimeInterval(value = converted.value, unit = converted.unit)
 
 
 class Length(UnitBase):
-    r"""``gearpy.units.units.Length`` object.
+    r""":py:class:`Length <gearpy.units.units.Length>` object.
 
     Attributes
     ----------
-    :py:attr:`unit` : str
+    :py:attr:`unit` : :py:class:`str`
         Symbol of the unit of measurement for length.
-    :py:attr:`value` : float or int
+    :py:attr:`value` : :py:class:`float` or :py:class:`int`
         Length numerical value.
 
     Methods
     -------
     :py:meth:`to`
-        Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
+        It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement.
     """
 
     __UNITS = {'m': 1,
                'dm': 1e-1,
                'cm': 1e-2,
                'mm': 1e-3}
 
@@ -1610,103 +1665,108 @@
         if isinstance(other, Length):
             return self.__value/other.to(self.__unit).value
         else:
             return Length(value = self.__value/other, unit = self.__unit)
 
     @property
     def value(self) -> Union[float, int]:
-        """Length numerical value. The relative unit is expressed by the ``unit`` property. It must be positive.
+        """Length numerical value. The relative unit is expressed by the :py:attr:`unit` property. It must be positive.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Length numerical value.
 
-        Raises
-        ------
-        TypeError
-            If ``value`` is not a float or an integer.
-        ValueError
-            If ``value`` is negative or null.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`value` is not a :py:class:`float` or an :py:class:`int`.
+           ``ValueError``
+               If :py:attr:`value` is negative or null.
         """
         return self.__value
 
     @property
     def unit(self) -> str:
-        """Symbol of the unit of measurement for length. It must be a string.
+        """Symbol of the unit of measurement for length. It must be a :py:class:`str`.
         Available units are:
 
         - ``'m'`` for meter,
         - ``'dm'`` for decimeter,
         - ``'cm'`` for centimeter,
         - ``'mm'`` for millimeter.
 
         Returns
         -------
-        str
+        :py:class:`str`
             Symbol of the unit of measurement for length.
 
-        Raises
-        ------
-        TypeError
-            If ``unit`` is not a string.
-        KeyError
-            If the ``unit`` is not among available ones.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`unit` is not a :py:class:`str`.
+           ``KeyError``
+               If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
     def to(self, target_unit: str, inplace: bool = False) -> 'Length':
-        """Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
-        If ``inplace`` is ``True``, it overrides actual ``value`` and ``unit``, otherwise it returns a new instance with
-        the converted ``value`` and the ``target_unit`` as ``unit``.
+        """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement. \n
+        If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
+        instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
-        target_unit : str
+        ``target_unit`` : :py:class:`str`
             Target unit to which convert the current value.
-        inplace : bool, optional
+        ``inplace`` : :py:class:`bool`, optional
             Whether to override the current instance value. Default is ``False``, so it does not override the current
             value.
 
         Returns
         -------
-        Length
+        :py:class:`Length <gearpy.units.units.Length>`
             Converted length.
 
-        Raises
-        ------
-        TypeError
-            - If ``target_unit`` is not a string,
-            - if ``inplace`` is not a bool.
-        KeyError
-            If the ``target_unit`` is not among available ones.
-
-        Examples
-        --------
-        ``Length`` instantiation.
-
-        >>> from gearpy.units import Length
-        >>> l = Length(1, 'm')
-        >>> l
-        ... 1 m
-
-        Conversion from meter to centimeter with ``inplace = False`` by default, so it does not override the current
-        value.
-
-        >>> l.to('cm')
-        ... 100.0 cm
-        >>> l
-        ... 1 m
-
-        Conversion from meter to centimeter with ``inplace = True``, in order to override the current value.
-
-        >>> l.to('cm', inplace = True)
-        ... 100.0 cm
-        >>> l
-        ... 100.0 cm
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If ``target_unit`` is not a :py:class:`str`,
+               - if ``inplace`` is not a :py:class:`bool`.
+           ``KeyError``
+               If the ``target_unit`` is not among available ones.
+
+        .. admonition:: Examples
+           :class: important
+
+           ``Length`` instantiation.
+
+           >>> from gearpy.units import Length
+           >>> l = Length(1, 'm')
+           >>> l
+           ... 1 m
+
+           Conversion from meter to centimeter with ``inplace = False`` by default, so it does not override the current
+           value.
+
+           >>> l.to('cm')
+           ... 100.0 cm
+           >>> l
+           ... 1 m
+
+           Conversion from meter to centimeter with ``inplace = True``, in order to override the current value.
+
+           >>> l.to('cm', inplace = True)
+           ... 100.0 cm
+           >>> l
+           ... 100.0 cm
         """
         super().to(target_unit = target_unit, inplace = inplace)
 
         if target_unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{target_unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
@@ -1720,27 +1780,28 @@
             self.__unit = target_unit
             return self
         else:
             return Length(value = target_value, unit = target_unit)
 
 
 class Surface(UnitBase):
-    r"""``gearpy.units.units.Surface`` object.
+    r""":py:class:`Surface <gearpy.units.units.Surface>` object.
 
     Attributes
     ----------
-    :py:attr:`unit` : str
+    :py:attr:`unit` : :py:class:`str`
         Symbol of the unit of measurement for surface.
-    :py:attr:`value` : float or int
+    :py:attr:`value` : :py:class:`float` or :py:class:`int`
         Surface numerical value.
 
     Methods
     -------
     :py:meth:`to`
-        Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
+        It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement.
     """
 
     __UNITS = {'m^2': 1,
                'dm^2': 1e-2,
                'cm^2': 1e-4,
                'mm^2': 1e-6}
 
@@ -1785,104 +1846,109 @@
         if isinstance(other, Surface):
             return self.__value/other.to(self.__unit).value
         else:
             return Surface(value = self.__value/other, unit = self.__unit)
 
     @property
     def value(self) -> Union[float, int]:
-        """Surface numerical value. The relative unit is expressed by the ``unit`` property. It must be positive.
+        """Surface numerical value. The relative unit is expressed by the :py:attr:`unit` property. It must be positive.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Surface numerical value.
 
-        Raises
-        ------
-        TypeError
-            If ``value`` is not a float or an integer.
-        ValueError
-            If ``value`` is negative or null.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`value` is not a :py:class:`float` or an :py:class:`int`.
+           ``ValueError``
+               If :py:attr:`value` is negative or null.
         """
         return self.__value
 
     @property
     def unit(self) -> str:
-        """Symbol of the unit of measurement for surface. It must be a string.
+        """Symbol of the unit of measurement for surface. It must be a :py:class:`str`.
         Available units are:
 
         - ``'m^2'`` for square meter,
         - ``'dm^2'`` for square decimeter,
         - ``'cm^2'`` for square centimeter,
         - ``'mm^2'`` for square millimeter.
 
         Returns
         -------
-        str
+        :py:class:`str`
             Symbol of the unit of measurement for surface.
 
-        Raises
-        ------
-        TypeError
-            If ``unit`` is not a string.
-        KeyError
-            If the ``unit`` is not among available ones.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`unit` is not a :py:class:`str`.
+           ``KeyError``
+               If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
     def to(self, target_unit: str, inplace: bool = False) -> 'Surface':
-        """Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
-        If ``inplace`` is ``True``, it overrides actual ``value`` and ``unit``, otherwise it returns a new instance with
-        the converted ``value`` and the ``target_unit`` as ``unit``.
+        """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement. \n
+        If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
+        instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
-        target_unit : str
+        ``target_unit`` : :py:class:`str`
             Target unit to which convert the current value.
-        inplace : bool, optional
+        ``inplace`` : :py:class:`bool`, optional
             Whether to override the current instance value. Default is ``False``, so it does not override the current
             value.
 
         Returns
         -------
-        Surface
+        :py:class:`Surface <gearpy.units.units.Surface>`
             Converted surface.
 
-        Raises
-        ------
-        TypeError
-            - If ``target_unit`` is not a string,
-            - if ``inplace`` is not a bool.
-        KeyError
-            If the ``target_unit`` is not among available ones.
-
-        Examples
-        --------
-        ``Surface`` instantiation.
-
-        >>> from gearpy.units import Surface
-        >>> s = Surface(1, 'm^2')
-        >>> s
-        ... 1 m^2
-
-        Conversion from square meter to square millimeter with ``inplace = False`` by default, so it does not override
-        the current value.
-
-        >>> s.to('mm^2')
-        ... 1000000.0 mm^2
-        >>> s
-        ... 1 m^2
-
-        Conversion from square meter to square millimeter with ``inplace = True``, in order to override the current
-        value.
-
-        >>> s.to('mm^2', inplace = True)
-        ... 1000000.0 mm^2
-        >>> s
-        ... 1000000.0 mm^2
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If ``target_unit`` is not a :py:class:`str`,
+               - if ``inplace`` is not a :py:class:`bool`.
+           ``KeyError``
+               If the ``target_unit`` is not among available ones.
+
+        .. admonition:: Examples
+           :class: important
+
+           ``Surface`` instantiation.
+
+           >>> from gearpy.units import Surface
+           >>> s = Surface(1, 'm^2')
+           >>> s
+           ... 1 m^2
+
+           Conversion from square meter to square millimeter with ``inplace = False`` by default, so it does not
+           override the current value.
+
+           >>> s.to('mm^2')
+           ... 1000000.0 mm^2
+           >>> s
+           ... 1 m^2
+
+           Conversion from square meter to square millimeter with ``inplace = True``, in order to override the current
+           value.
+
+           >>> s.to('mm^2', inplace = True)
+           ... 1000000.0 mm^2
+           >>> s
+           ... 1000000.0 mm^2
         """
         super().to(target_unit = target_unit, inplace = inplace)
 
         if target_unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{target_unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
@@ -1896,27 +1962,28 @@
             self.__unit = target_unit
             return self
         else:
             return Surface(value = target_value, unit = target_unit)
 
 
 class Force(UnitBase):
-    r"""``gearpy.units.units.Force`` object.
+    r""":py:class:`Force <gearpy.units.units.Force>` object.
 
     Attributes
     ----------
-    :py:attr:`unit` : str
+    :py:attr:`unit` : :py:class:`str`
         Symbol of the unit of measurement for force.
-    :py:attr:`value` : float or int
+    :py:attr:`value` : :py:class:`float` or :py:class:`int`
         Force numerical value.
 
     Methods
     -------
     :py:meth:`to`
-        Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
+        It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement.
     """
 
     __UNITS = {'N': 1,
                'mN': 1e-3,
                'kN': 1e3,
                'kgf': 9.80665,
                'gf': 9.80665e-3}
@@ -1962,102 +2029,107 @@
         elif isinstance(other, Surface):
             return Stress(value = self.to('N').value/other.to('m^2').value, unit = 'Pa')
         else:
             return Force(value = self.__value/other, unit = self.__unit)
 
     @property
     def value(self) -> Union[float, int]:
-        """Force numerical value. The relative unit is expressed by the ``unit`` property.
+        """Force numerical value. The relative unit is expressed by the :py:attr:`unit` property.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Force numerical value.
 
-        Raises
-        ------
-        TypeError
-            If ``value`` is not a float or an integer.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`value` is not a :py:class:`float` or an :py:class:`int`.
         """
         return self.__value
 
     @property
     def unit(self) -> str:
-        """Symbol of the unit of measurement for force. It must be a string.
+        """Symbol of the unit of measurement for force. It must be a :py:class:`str`.
         Available units are:
 
         - ``'N'`` for newton,
         - ``'mN'`` for milli-newton,
         - ``'kN'`` for kilo-newton,
         - ``'kgf'`` for kilogram force,
         - ``'gf'`` for gram force.
 
         Returns
         -------
-        str
+        :py:class:`str`
             Symbol of the unit of measurement for force.
 
-        Raises
-        ------
-        TypeError
-            If ``unit`` is not a string.
-        KeyError
-            If the ``unit`` is not among available ones.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`unit` is not a :py:class:`str`.
+           ``KeyError``
+               If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
     def to(self, target_unit: str, inplace: bool = False) -> 'Force':
-        """Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
-        If ``inplace`` is ``True``, it overrides actual ``value`` and ``unit``, otherwise it returns a new instance with
-        the converted ``value`` and the ``target_unit`` as ``unit``.
+        """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement. \n
+        If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
+        instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
-        target_unit : str
+        ``target_unit`` : :py:class:`str`
             Target unit to which convert the current value.
-        inplace : bool, optional
+        ``inplace`` : :py:class:`bool`, optional
             Whether to override the current instance value. Default is ``False``, so it does not override the current
             value.
 
         Returns
         -------
-        Force
+        :py:class:`Force <gearpy.units.units.Force>`
             Converted force.
 
-        Raises
-        ------
-        TypeError
-            - If ``target_unit`` is not a string,
-            - if ``inplace`` is not a bool.
-        KeyError
-            If the ``target_unit`` is not among available ones.
-
-        Examples
-        --------
-        ``Force`` instantiation.
-
-        >>> from gearpy.units import Force
-        >>> f = Force(1, 'N')
-        >>> f
-        ... 1 N
-
-        Conversion from newton to kilogram force with ``inplace = False`` by default, so it does not override the
-        current value.
-
-        >>> f.to('kgf')
-        ... 0.10197162129779283 kgf
-        >>> f
-        ... 1 N
-
-        Conversion from newton to kilogram force with ``inplace = True``, in order to override the current value.
-
-        >>> f.to('kgf', inplace = True)
-        ... 0.10197162129779283 kgf
-        >>> f
-        ... 0.10197162129779283 kgf
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If ``target_unit`` is not a :py:class:`str`,
+               - if ``inplace`` is not a :py:class:`bool`.
+           ``KeyError``
+               If the ``target_unit`` is not among available ones.
+
+        .. admonition:: Examples
+           :class: important
+
+           ``Force`` instantiation.
+
+           >>> from gearpy.units import Force
+           >>> f = Force(1, 'N')
+           >>> f
+           ... 1 N
+
+           Conversion from newton to kilogram force with ``inplace = False`` by default, so it does not override the
+           current value.
+
+           >>> f.to('kgf')
+           ... 0.10197162129779283 kgf
+           >>> f
+           ... 1 N
+
+           Conversion from newton to kilogram force with ``inplace = True``, in order to override the current value.
+
+           >>> f.to('kgf', inplace = True)
+           ... 0.10197162129779283 kgf
+           >>> f
+           ... 0.10197162129779283 kgf
         """
         super().to(target_unit = target_unit, inplace = inplace)
 
         if target_unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{target_unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
@@ -2071,27 +2143,28 @@
             self.__unit = target_unit
             return self
         else:
             return Force(value = target_value, unit = target_unit)
 
 
 class Stress(UnitBase):
-    r"""``gearpy.units.units.Stress`` object.
+    r""":py:class:`Stress <gearpy.units.units.Stress>` object.
 
     Attributes
     ----------
-    :py:attr:`unit` : str
+    :py:attr:`unit` : :py:class:`str`
         Symbol of the unit of measurement for stress.
-    :py:attr:`value` : float or int
+    :py:attr:`value` : :py:class:`float` or :py:class:`int`
         Stress numerical value.
 
     Methods
     -------
     :py:meth:`to`
-        Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
+        It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement.
     """
 
     __UNITS = {'Pa': 1,
                'kPa': 1e3,
                'MPa': 1e6,
                'GPa': 1e9}
 
@@ -2133,101 +2206,106 @@
         if isinstance(other, Stress):
             return self.__value/other.to(self.__unit).value
         else:
             return Stress(value = self.__value/other, unit = self.__unit)
 
     @property
     def value(self) -> Union[float, int]:
-        """Stress numerical value. The relative unit is expressed by the ``unit`` property.
+        """Stress numerical value. The relative unit is expressed by the :py:attr:`unit` property.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Stress numerical value.
 
-        Raises
-        ------
-        TypeError
-            If ``value`` is not a float or an integer.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`value` is not a :py:class:`float` or an :py:class:`int`.
         """
         return self.__value
 
     @property
     def unit(self) -> str:
-        """Symbol of the unit of measurement for stress. It must be a string.
+        """Symbol of the unit of measurement for stress. It must be a :py:class:`str`.
         Available units are:
 
         - ``'Pa'`` for pascal,
         - ``'kPa'`` for kilo-pascal,
         - ``'MPa'`` for mega-pascal,
         - ``'GPa'`` for giga-pascal.
 
         Returns
         -------
-        str
+        :py:class:`str`
             Symbol of the unit of measurement for stress.
 
-        Raises
-        ------
-        TypeError
-            If ``unit`` is not a string.
-        KeyError
-            If the ``unit`` is not among available ones.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`unit` is not a :py:class:`str`.
+           ``KeyError``
+               If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
     def to(self, target_unit: str, inplace: bool = False) -> 'Stress':
-        """Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
-        If ``inplace`` is ``True``, it overrides actual ``value`` and ``unit``, otherwise it returns a new instance with
-        the converted ``value`` and the ``target_unit`` as ``unit``.
+        """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement. \n
+        If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
+        instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
-        target_unit : str
+        ``target_unit`` : :py:class:`str`
             Target unit to which convert the current value.
-        inplace : bool, optional
+        ``inplace`` : :py:class:`bool`, optional
             Whether to override the current instance value. Default is ``False``, so it does not override the current
             value.
 
         Returns
         -------
-        Stress
+        :py:class:`Stress <gearpy.units.units.Stress>`
             Converted stress.
 
-        Raises
-        ------
-        TypeError
-            - If ``target_unit`` is not a string,
-            - if ``inplace`` is not a bool.
-        KeyError
-            If the ``target_unit`` is not among available ones.
-
-        Examples
-        --------
-        ``Stress`` instantiation.
-
-        >>> from gearpy.units import Stress
-        >>> s = Stress(1, 'GPa')
-        >>> s
-        ... 1 GPa
-
-        Conversion from giga-pascal to mega-pascal with ``inplace = False`` by default, so it does not override the
-        current value.
-
-        >>> s.to('MPa')
-        ... 1000.0 MPa
-        >>> s
-        ... 1 GPa
-
-        Conversion from giga-pascal to mega-pascal with ``inplace = True``, in order to override the current value.
-
-        >>> s.to('MPa', inplace = True)
-        ... 1000.0 MPa
-        >>> s
-        ... 1000.0 MPa
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If ``target_unit`` is not a :py:class:`str`,
+               - if ``inplace`` is not a :py:class:`bool`.
+           ``KeyError``
+               If the ``target_unit`` is not among available ones.
+
+        .. admonition:: Examples
+           :class: important
+
+           ``Stress`` instantiation.
+
+           >>> from gearpy.units import Stress
+           >>> s = Stress(1, 'GPa')
+           >>> s
+           ... 1 GPa
+
+           Conversion from giga-pascal to mega-pascal with ``inplace = False`` by default, so it does not override the
+           current value.
+
+           >>> s.to('MPa')
+           ... 1000.0 MPa
+           >>> s
+           ... 1 GPa
+
+           Conversion from giga-pascal to mega-pascal with ``inplace = True``, in order to override the current value.
+
+           >>> s.to('MPa', inplace = True)
+           ... 1000.0 MPa
+           >>> s
+           ... 1000.0 MPa
         """
         super().to(target_unit = target_unit, inplace = inplace)
 
         if target_unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{target_unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
@@ -2241,27 +2319,28 @@
             self.__unit = target_unit
             return self
         else:
             return Stress(value = target_value, unit = target_unit)
 
 
 class Current(UnitBase):
-    r"""``gearpy.units.units.Current`` object.
+    r""":py:class:`Current <gearpy.units.units.Current>` object.
 
     Attributes
     ----------
-    :py:attr:`unit` : str
+    :py:attr:`unit` : :py:class:`str`
         Symbol of the unit of measurement for electrical current.
-    :py:attr:`value` : float or int
+    :py:attr:`value` : :py:class:`float` or :py:class:`int`
         Electrical current numerical value.
 
     Methods
     -------
     :py:meth:`to`
-        Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
+        It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement.
     """
 
     __UNITS = {'A': 1,
                'mA': 1e-3,
                'uA': 1e-6}
 
     def __init__(self, value: Union[float, int], unit: str):
@@ -2302,100 +2381,105 @@
         if isinstance(other, Current):
             return self.__value/other.to(self.__unit).value
         else:
             return Current(value = self.__value/other, unit = self.__unit)
 
     @property
     def value(self) -> Union[float, int]:
-        """Electrical current numerical value. The relative unit is expressed by the ``unit`` property.
+        """Electrical current numerical value. The relative unit is expressed by the :py:attr:`unit` property.
 
         Returns
         -------
-        float or int
+        :py:class:`float` or :py:class:`int`
             Electrical current numerical value.
 
-        Raises
-        ------
-        TypeError
-            If ``value`` is not a float or an integer.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`value` is not a :py:class:`float` or an :py:class:`int`.
         """
         return self.__value
 
     @property
     def unit(self) -> str:
-        """Symbol of the unit of measurement for electrical current. It must be a string.
+        """Symbol of the unit of measurement for electrical current. It must be a :py:class:`str`.
         Available units are:
 
         - ``'A'`` for ampere,
         - ``'mA'`` for milli-ampere,
         - ``'uA'`` for micro-ampere.
 
         Returns
         -------
-        str
+        :py:class:`str`
             Symbol of the unit of measurement for electrical current.
 
-        Raises
-        ------
-        TypeError
-            If ``unit`` is not a string.
-        KeyError
-            If the ``unit`` is not among available ones.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`unit` is not a :py:class:`str`.
+           ``KeyError``
+               If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
     def to(self, target_unit: str, inplace: bool = False) -> 'Current':
-        """Converts actual ``value`` to a new value computed using ``target_unit`` as the reference unit of measurement.
-        If ``inplace`` is ``True``, it overrides actual ``value`` and ``unit``, otherwise it returns a new instance with
-        the converted ``value`` and the ``target_unit`` as ``unit``.
+        """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
+        measurement. \n
+        If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
+        instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
-        target_unit : str
-            Target unit to which convert the electrical current value.
-        inplace : bool, optional
+        ``target_unit`` : :py:class:`str`
+            Target unit to which convert the current value.
+        ``inplace`` : :py:class:`bool`, optional
             Whether to override the current instance value. Default is ``False``, so it does not override the current
             value.
 
         Returns
         -------
-        Current
+        :py:class:`Current <gearpy.units.units.Current>`
             Converted electrical current.
 
-        Raises
-        ------
-        TypeError
-            - If ``target_unit`` is not a string,
-            - if ``inplace`` is not a bool.
-        KeyError
-            If the ``target_unit`` is not among available ones.
-
-        Examples
-        --------
-        ``Current`` instantiation.
-
-        >>> from gearpy.units import Current
-        >>> i = Current(1, 'A')
-        >>> i
-        ... 1 A
-
-        Conversion from ampere to milli-ampere with ``inplace = False`` by default, so it does not override the current
-        value.
-
-        >>> i.to('mA')
-        ... 1000.0 mA
-        >>> i
-        ... 1 A
-
-        Conversion from ampere to milli-ampere with ``inplace = True``, in order to override the current value.
-
-        >>> i.to('mA', inplace = True)
-        ... 1000.0 mA
-        >>> i
-        ... 1000.0 mA
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If ``target_unit`` is not a :py:class:`str`,
+               - if ``inplace`` is not a :py:class:`bool`.
+           ``KeyError``
+               If the ``target_unit`` is not among available ones.
+
+        .. admonition:: Examples
+           :class: important
+
+           ``Current`` instantiation.
+
+           >>> from gearpy.units import Current
+           >>> i = Current(1, 'A')
+           >>> i
+           ... 1 A
+
+           Conversion from ampere to milli-ampere with ``inplace = False`` by default, so it does not override the
+           current value.
+
+           >>> i.to('mA')
+           ... 1000.0 mA
+           >>> i
+           ... 1 A
+
+           Conversion from ampere to milli-ampere with ``inplace = True``, in order to override the current value.
+
+           >>> i.to('mA', inplace = True)
+           ... 1000.0 mA
+           >>> i
+           ... 1000.0 mA
         """
         super().to(target_unit = target_unit, inplace = inplace)
 
         if target_unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{target_unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
```

### Comparing `gearpy-0.6.0/gearpy/utils/animate.py` & `gearpy-0.7.0/gearpy/utils/animate.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,93 +15,98 @@
                                        current_unit: Optional[str] = 'A',
                                        figsize: Optional[tuple] = None,
                                        line_color: Optional[str] = None,
                                        marker_color: Optional[str] = None,
                                        marker_size: Optional[Union[float, int]] = None,
                                        padding: Optional[Union[float, int]] = 0.1,
                                        show: Optional[bool] = True) -> FuncAnimation:
-    """Generates an animation of a DC motor torque-speed and torque-current characteristic curves and relative working
-    points during the simulation. \n
+    """It generates an animation of a :py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>` torque-speed and
+    torque-current characteristic curves and relative working points during the simulation. \n
     Each simulated time step is a frame on the animation. \n
     It generates two subplots, one for each characteristic curve. It is possible to isolate a single characteristic to
     be plotted with optional parameters ``torque_speed_curve`` and ``torque_current_curve``. \n
-    The characteristic curves can be modified by the motor pulse width modulation ``pwm``. \n
+    The characteristic curves can be modified by the motor pulse width modulation
+    :py:attr:`DCMotor.pwm <gearpy.mechanical_objects.dc_motor.DCMotor.pwm>`. \n
     Plotted values' units are managed with optional parameters ``angular_speed_unit``, ``torque_unit`` and
     ``current_unit``. \n
     Aesthetic parameters are managed with optional parameters ``figsize``, ``line_color``, ``marker_color``,
     ``marker_size`` and  ``padding``.
 
     Parameters
     ----------
-    motor : DCMotor
+    ``motor`` : :py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>`
         DC motor whose characteristic curves and working point have to be animated.
-    time : list
+    ``time`` : :py:class:`list`
         The list of ``Time`` computed by the solver.
-    interval : float or int, optional
+    ``interval`` : :py:class:`float` or :py:class:`int`, optional
         Delay between animation frames in milliseconds. If not provided defaults to ``200``.
-    torque_speed_curve : bool, optional
+    ``torque_speed_curve`` : :py:class:`bool`, optional
         Whether to plot the torque-speed characteristic curve. Default is ``True``.
-    torque_current_curve : bool, optional
+    ``torque_current_curve`` : :py:class:`bool`, optional
         Whether to plot the torque-current characteristic curve. Default is ``True``.
-    angular_speed_unit : str, optional
+    ``angular_speed_unit`` : :py:class:`str`, optional
         Symbol of the unit of measurement to which convert the angular speed values in the plot. It must be a string.
-        Default is ``'rad/s'``.
-    torque_unit : str, optional
+        Default is ``'rad/s'``. See :py:attr:`AngularSpeed.unit <gearpy.units.units.AngularSpeed.unit>` for more
+        details.
+    ``torque_unit`` : :py:class:`str`, optional
         Symbol of the unit of measurement to which convert the torque values in the plot. It must be a string. Default
-        is ``'Nm'``.
-    current_unit : str, optional
+        is ``'Nm'``. See :py:attr:`Torque.unit <gearpy.units.units.Torque.unit>` for more details.
+    ``current_unit`` : :py:class:`str`, optional
         Symbol of the unit of measurement to which convert the electric current values in the plot. It must be a string.
-        Default is ``'A'``.
-    figsize : tuple, optional
+        Default is ``'A'``. See :py:attr:`Current.unit <gearpy.units.units.Current.unit>` for more details.
+    ``figsize`` : :py:class:`tuple`, optional
         Width and height of the window size, in inches. If not provided defaults to ``[6.4, 4.8]``.
-    line_color : str, optional
+    ``line_color`` : :py:class:`str`, optional
         Color of the characteristic curve lines. If not provided defaults to ``'#1f77b4'``.
-    marker_color : str, optional
+    ``marker_color`` : :py:class:`str`, optional
         Color of the motor working point marker. If not provided defaults to ``'#ff7f0e'``.
-    marker_size : float or int, optional
+    ``marker_size`` : :py:class:`float` or :py:class:`int`, optional
         Size, in points, of the motor working point marker. If not provided defaults to ``6``.
-    padding : float or int, optional
+    ``padding`` : :py:class:`float` or :py:class:`int`, optional
         Extra-space to be taken around each motor characteristics extreme points. It is expressed in percent points of
         the extreme point value. Default is ``0.1``, so it is taken 10% space around each characteristic extreme points.
-    show : bool, optional
+    ``show`` : :py:class:`bool`, optional
         Whether to show the animation. Default is ``True``.
 
-    Raises
-    ------
-    TypeError
-        - If ``motor`` is not an instance of ``DCMotor``,
-        - if ``time`` is not a list,
-        - if an element of ``time`` is not an instance of ``Time``,
-        - if ``interval`` is not a float or an integer,
-        - if ``torque_speed_curve`` is not a bool,
-        - if ``torque_current_curve`` is not a bool,
-        - if ``angular_speed_unit`` is not a string,
-        - if ``torque_unit`` is not a string,
-        - if ``current_unit`` is not a string,
-        - if ``figsize`` is not a tuple,
-        - if an element of ``figsize`` is not a float or an integer,
-        - if ``line_color`` is not a string,
-        - if ``marker_color`` is not a string,
-        - if ``marker_size`` is not a float or an integer,
-        - if ``padding`` is not a float or an integer,
-        - if ``show`` is not a bool.
-    ValueError
-        - If ``time`` is an empty list,
-        - if both ``torque_speed_curve`` and ``torque_current_curve`` are set to ``False``,
-        - if ``torque_current_curve`` is set to ``True`` but ``motor`` cannot compute ``electric_current`` property,
-        - if ``figsize`` has not exactly two elements: one for width and the other for height,
-        - if ``padding`` is negative.
-
-    See Also
-    --------
-    :py:attr:`gearpy.mechanical_objects.dc_motor.DCMotor.angular_speed`
-    :py:attr:`gearpy.mechanical_objects.dc_motor.DCMotor.driving_torque`
-    :py:attr:`gearpy.mechanical_objects.dc_motor.DCMotor.electric_current`
-    :py:attr:`gearpy.mechanical_objects.dc_motor.DCMotor.time_variables`
-    :py:attr:`gearpy.mechanical_objects.dc_motor.DCMotor.pwm`
+    .. admonition:: Raises
+       :class: warning
+
+       ``TypeError``
+           - If ``motor`` is not an instance of :py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>`,
+           - if ``time`` is not a :py:class:`list`,
+           - if an element of ``time`` is not an instance of :py:class:`Time <gearpy.units.units.Time>`,
+           - if ``interval`` is not a :py:class:`float` or an :py:class:`int`,
+           - if ``torque_speed_curve`` is not a :py:class:`bool`,
+           - if ``torque_current_curve`` is not a :py:class:`bool`,
+           - if ``angular_speed_unit`` is not a :py:class:`str`,
+           - if ``torque_unit`` is not a :py:class:`str`,
+           - if ``current_unit`` is not a :py:class:`str`,
+           - if ``figsize`` is not a :py:class:`tuple`,
+           - if an element of ``figsize`` is not a :py:class:`float` or an :py:class:`int`,
+           - if ``line_color`` is not a :py:class:`str`,
+           - if ``marker_color`` is not a :py:class:`str`,
+           - if ``marker_size`` is not a :py:class:`float` or an :py:class:`int`,
+           - if ``padding`` is not a :py:class:`float` or an :py:class:`int`,
+           - if ``show`` is not a :py:class:`bool`.
+       ``ValueError``
+           - If ``time`` is an empty :py:class:`list`,
+           - if both ``torque_speed_curve`` and ``torque_current_curve`` are set to ``False``,
+           - if ``torque_current_curve`` is set to ``True`` but ``motor`` cannot compute
+             :py:attr:`DCMotor.electric_current <gearpy.mechanical_objects.dc_motor.DCMotor.electric_current>` property,
+           - if ``figsize`` has not exactly two elements: one for width and the other for height,
+           - if ``padding`` is negative.
+
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:attr:`DCMotor.angular_speed <gearpy.mechanical_objects.dc_motor.DCMotor.angular_speed>` \n
+       :py:attr:`DCMotor.driving_torque <gearpy.mechanical_objects.dc_motor.DCMotor.driving_torque>` \n
+       :py:attr:`DCMotor.electric_current <gearpy.mechanical_objects.dc_motor.DCMotor.electric_current>` \n
+       :py:attr:`DCMotor.time_variables <gearpy.mechanical_objects.dc_motor.DCMotor.time_variables>` \n
+       :py:attr:`DCMotor.pwm <gearpy.mechanical_objects.dc_motor.DCMotor.pwm>`
     """
     if not isinstance(motor, DCMotor):
         raise TypeError(f"Parameter 'motor' must be an instance of {DCMotor.__name__!r}.")
 
     if not isinstance(time, list):
         raise TypeError("Parameter 'time' must be a list.")
```

### Comparing `gearpy-0.6.0/gearpy.egg-info/SOURCES.txt` & `gearpy-0.7.0/gearpy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-README.md
+README.rst
 setup.py
 gearpy/__init__.py
 gearpy/powertrain.py
 gearpy/solver.py
 gearpy.egg-info/PKG-INFO
 gearpy.egg-info/SOURCES.txt
 gearpy.egg-info/dependency_links.txt
@@ -26,15 +26,22 @@
 gearpy/motor_control/rules/reach_angular_position.py
 gearpy/motor_control/rules/rules_base.py
 gearpy/motor_control/rules/start_limit_current.py
 gearpy/motor_control/rules/start_proportional_to_angular_position.py
 gearpy/motor_control/rules/utils.py
 gearpy/sensors/__init__.py
 gearpy/sensors/absolute_rotary_encoder.py
+gearpy/sensors/amperometer.py
+gearpy/sensors/sensor_base.py
 gearpy/sensors/tachometer.py
 gearpy/sensors/timer.py
 gearpy/units/__init__.py
 gearpy/units/unit_base.py
 gearpy/units/units.py
 gearpy/utils/__init__.py
 gearpy/utils/animate.py
-gearpy/utils/relations.py
+gearpy/utils/export.py
+gearpy/utils/relations.py
+gearpy/utils/stop_condition/__init__.py
+gearpy/utils/stop_condition/operator.py
+gearpy/utils/stop_condition/operator_base.py
+gearpy/utils/stop_condition/stop_condition.py
```

### Comparing `gearpy-0.6.0/setup.py` & `gearpy-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 import subprocess
 
 version = subprocess.run(['git', 'describe', '--tags'], stdout = subprocess.PIPE).stdout.decode('utf-8').strip()
 
-with open('README.md', 'r') as f:
+with open('README.rst', 'r') as f:
     long_description = f.read()
 
 def read_requirements(path: str):
     with open(path) as file:
         lines = file.readlines()
 
     return [line.replace('==', ' >= ').replace('\n', '') for line in lines]
@@ -19,15 +19,15 @@
 
 
 setup(name = 'gearpy',
       version = version,
       description = "Python package for mechanical transmission analysis",
       packages = find_packages(where = '.'),
       long_description = long_description,
-      long_description_content_type = 'text/markdown',
+      long_description_content_type = 'text/x-rst',
       url = 'https://github.com/AndreaBlengino/gearpy',
       project_urls = {'Source': 'https://github.com/AndreaBlengino/gearpy',
                       'Tracker': 'https://github.com/AndreaBlengino/gearpy/issues',
                       'Documentation': 'https://gearpy.readthedocs.io/en/latest/index.html'},
       author = 'Andrea Blengino',
       author_email = 'ing.andrea.blengino@gmail.com',
       license = 'GNU GPL3',
```

