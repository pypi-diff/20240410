# Comparing `tmp/pyroll_core-2.1.5.tar.gz` & `tmp/pyroll_core-2.1.6.tar.gz`

## Comparing `pyroll_core-2.1.5.tar` & `pyroll_core-2.1.6.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/__init__.py
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/config.py
--rw-r--r--   0        0        0    17140 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/hooks.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/log.py
--rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/repr.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/shapes.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/disk_elements/__init__.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/disk_elements/disk_element_unit.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/disk_elements/hookimpls.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/__init__.py
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/base.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/equivalent_ripped_groove.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/flat.py
--rw-r--r--   0        0        0     9604 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/generic_elongation.py
--rw-r--r--   0        0        0    13557 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/generic_elongation_solvers.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/hexagonal.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/spline.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/boxes/__init__.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/boxes/box.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/boxes/constricted_box.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/boxes/upset_box.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/diamonds/__init__.py
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/diamonds/diamond.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/diamonds/gothic.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/diamonds/square.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/ovals/__init__.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/ovals/circular_oval.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/ovals/constricted_circular_oval.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/ovals/constricted_swedish_oval.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/ovals/flat_oval.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/ovals/oval_3radii.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/ovals/oval_3radii_flanked.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/ovals/swedish_oval.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/ovals/upset_oval.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/rounds/__init__.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/rounds/false_round.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/grooves/rounds/round.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/profile/__init__.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/profile/hookimpls.py
--rw-r--r--   0        0        0    28273 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/profile/profile.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/roll/__init__.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/roll/hookimpls.py
--rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/roll/roll.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/roll_pass/__init__.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/roll_pass/deformation_unit.py
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/roll_pass/roll_pass.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/roll_pass/three_roll_pass.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/roll_pass/hookimpls/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/roll_pass/hookimpls/deformation_unit.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/roll_pass/hookimpls/disk_element.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/roll_pass/hookimpls/helpers.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/roll_pass/hookimpls/profile.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/roll_pass/hookimpls/roll.py
--rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/roll_pass/hookimpls/roll_pass.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/rotator/__init__.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/rotator/hookimpls.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/rotator/rotator.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/sequence/__init__.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/sequence/hookimpls.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/sequence/sequence.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/transport/__init__.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/transport/cooling_pipe.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/transport/transport.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/transport/hookimpls/__init__.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/transport/hookimpls/cooling_pipe.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/transport/hookimpls/transport.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/unit/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/unit/hookimpls.py
--rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyroll/core/unit/unit.py
--rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/.gitignore
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/LICENSE
--rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/README.md
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/hatch.toml
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/pyproject.toml
--rw-r--r--   0        0        0     8514 2020-02-02 00:00:00.000000 pyroll_core-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/__init__.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/config.py
+-rw-r--r--   0        0        0    17140 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/hooks.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/log.py
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/repr.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/shapes.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/disk_elements/__init__.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/disk_elements/disk_element_unit.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/disk_elements/hookimpls.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/__init__.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/base.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/equivalent_ripped_groove.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/flat.py
+-rw-r--r--   0        0        0     9604 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/generic_elongation.py
+-rw-r--r--   0        0        0    13557 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/generic_elongation_solvers.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/hexagonal.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/spline.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/boxes/__init__.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/boxes/box.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/boxes/constricted_box.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/boxes/upset_box.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/diamonds/__init__.py
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/diamonds/diamond.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/diamonds/gothic.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/diamonds/square.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/ovals/__init__.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/ovals/circular_oval.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/ovals/constricted_circular_oval.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/ovals/constricted_swedish_oval.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/ovals/flat_oval.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/ovals/oval_3radii.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/ovals/oval_3radii_flanked.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/ovals/swedish_oval.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/ovals/upset_oval.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/rounds/__init__.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/rounds/false_round.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/grooves/rounds/round.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/profile/__init__.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/profile/hookimpls.py
+-rw-r--r--   0        0        0    29204 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/profile/profile.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/roll/__init__.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/roll/hookimpls.py
+-rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/roll/roll.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/roll_pass/__init__.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/roll_pass/deformation_unit.py
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/roll_pass/roll_pass.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/roll_pass/three_roll_pass.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/roll_pass/hookimpls/__init__.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/roll_pass/hookimpls/deformation_unit.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/roll_pass/hookimpls/disk_element.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/roll_pass/hookimpls/helpers.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/roll_pass/hookimpls/profile.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/roll_pass/hookimpls/roll.py
+-rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/roll_pass/hookimpls/roll_pass.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/rotator/__init__.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/rotator/hookimpls.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/rotator/rotator.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/sequence/__init__.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/sequence/hookimpls.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/sequence/sequence.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/transport/__init__.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/transport/cooling_pipe.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/transport/transport.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/transport/hookimpls/__init__.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/transport/hookimpls/cooling_pipe.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/transport/hookimpls/transport.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/unit/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/unit/hookimpls.py
+-rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyroll/core/unit/unit.py
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/.gitignore
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/LICENSE
+-rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/README.md
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/hatch.toml
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0     8514 2020-02-02 00:00:00.000000 pyroll_core-2.1.6/PKG-INFO
```

### Comparing `pyroll_core-2.1.5/pyroll/core/__init__.py` & `pyroll_core-2.1.6/pyroll/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .profile import *
 from .rotator import Rotator
 from .sequence import PassSequence
 from .hooks import Hook, HookHost, HookFunction, root_hooks
 from .disk_elements import DiskElementUnit
 from .config import Config, config
 
-VERSION = "2.1.5"
+VERSION = "2.1.6"
 
 root_hooks.extend(
     [
         RollPass.roll_force,
         RollPass.Roll.roll_torque,
         RollPass.elongation_efficiency,
         Unit.power,
```

### Comparing `pyroll_core-2.1.5/pyroll/core/config.py` & `pyroll_core-2.1.6/pyroll/core/config.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/hooks.py` & `pyroll_core-2.1.6/pyroll/core/hooks.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/repr.py` & `pyroll_core-2.1.6/pyroll/core/repr.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/shapes.py` & `pyroll_core-2.1.6/pyroll/core/shapes.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/disk_elements/disk_element_unit.py` & `pyroll_core-2.1.6/pyroll/core/disk_elements/disk_element_unit.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/disk_elements/hookimpls.py` & `pyroll_core-2.1.6/pyroll/core/disk_elements/hookimpls.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/__init__.py` & `pyroll_core-2.1.6/pyroll/core/grooves/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/base.py` & `pyroll_core-2.1.6/pyroll/core/grooves/base.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/equivalent_ripped_groove.py` & `pyroll_core-2.1.6/pyroll/core/grooves/equivalent_ripped_groove.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/flat.py` & `pyroll_core-2.1.6/pyroll/core/grooves/flat.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/generic_elongation.py` & `pyroll_core-2.1.6/pyroll/core/grooves/generic_elongation.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/generic_elongation_solvers.py` & `pyroll_core-2.1.6/pyroll/core/grooves/generic_elongation_solvers.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/hexagonal.py` & `pyroll_core-2.1.6/pyroll/core/grooves/hexagonal.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/spline.py` & `pyroll_core-2.1.6/pyroll/core/grooves/spline.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/boxes/box.py` & `pyroll_core-2.1.6/pyroll/core/grooves/boxes/box.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/boxes/constricted_box.py` & `pyroll_core-2.1.6/pyroll/core/grooves/boxes/constricted_box.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/boxes/upset_box.py` & `pyroll_core-2.1.6/pyroll/core/grooves/boxes/upset_box.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/diamonds/diamond.py` & `pyroll_core-2.1.6/pyroll/core/grooves/diamonds/diamond.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/diamonds/gothic.py` & `pyroll_core-2.1.6/pyroll/core/grooves/diamonds/gothic.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/diamonds/square.py` & `pyroll_core-2.1.6/pyroll/core/grooves/diamonds/square.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/ovals/circular_oval.py` & `pyroll_core-2.1.6/pyroll/core/grooves/ovals/circular_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/ovals/constricted_circular_oval.py` & `pyroll_core-2.1.6/pyroll/core/grooves/ovals/constricted_circular_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/ovals/constricted_swedish_oval.py` & `pyroll_core-2.1.6/pyroll/core/grooves/ovals/constricted_swedish_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/ovals/flat_oval.py` & `pyroll_core-2.1.6/pyroll/core/grooves/ovals/flat_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/ovals/oval_3radii.py` & `pyroll_core-2.1.6/pyroll/core/grooves/ovals/oval_3radii.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/ovals/oval_3radii_flanked.py` & `pyroll_core-2.1.6/pyroll/core/grooves/ovals/oval_3radii_flanked.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/ovals/swedish_oval.py` & `pyroll_core-2.1.6/pyroll/core/grooves/ovals/swedish_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/ovals/upset_oval.py` & `pyroll_core-2.1.6/pyroll/core/grooves/ovals/upset_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/rounds/false_round.py` & `pyroll_core-2.1.6/pyroll/core/grooves/rounds/false_round.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/grooves/rounds/round.py` & `pyroll_core-2.1.6/pyroll/core/grooves/rounds/round.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/profile/hookimpls.py` & `pyroll_core-2.1.6/pyroll/core/profile/hookimpls.py`

 * *Files 23% similar despite different names*

```diff
@@ -66,14 +66,30 @@
 
 @Profile.thermal_diffusivity
 def thermal_diffusivity(self: Profile):
     if hasattr(self, "thermal_conductivity") and hasattr(self, "density") and hasattr(self, "specific_heat_capacity"):
         return self.thermal_conductivity / (self.density * self.specific_heat_capacity)
 
 
+
+@Profile.hydrostatic_stress
+def hydrostatic_stress(self: Profile):
+    if hasattr(self, "longitudinal_stress") and hasattr(self, "altitudinal_stress") and hasattr(self,
+                                                                                                "latitudinal_stress"):
+        return (self.longitudinal_stress + self.altitudinal_stress + self.latitudinal_stress) / 3
+
+
+@Profile.equivalent_stress
+def equivalent_stress(self: Profile):
+    if hasattr(self, "longitudinal_stress") and hasattr(self, "altitudinal_stress") and hasattr(self,
+                                                                                                "latitudinal_stress"):
+        return np.sqrt(1 / 2 * (self.longitudinal_stress - self.altitudinal_stress) ** 2 + (
+                self.altitudinal_stress - self.latitudinal_stress) ** 2 + (
+                               self.latitudinal_stress - self.longitudinal_stress) ** 2)
+
 @Profile.astm_grain_size_number
 def astm_grain_size_number(self: Profile):
     if self.has_set_or_cached("grain_size"):
         grain_diameter_inch = self.grain_size / 0.0254
         grain_area_square_inch = np.pi * (grain_diameter_inch / 2) ** 2
         grains_per_square_inch_1x_magnification = 1 / grain_area_square_inch
         grains_per_square_inch_100x_magnification = grains_per_square_inch_1x_magnification / (100 ** 2)
```

### Comparing `pyroll_core-2.1.5/pyroll/core/profile/profile.py` & `pyroll_core-2.1.6/pyroll/core/profile/profile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 from typing import Optional, Union, Callable
-from collections.abc import Iterable, Collection, Set
+from collections.abc import Set
 
 import numpy as np
 from shapely.affinity import translate, rotate
 from shapely.geometry import Point, LinearRing, Polygon, LineString
-from shapely.ops import clip_by_rect, unary_union
+from shapely.ops import clip_by_rect
 
 from ..config import Config
 from ..grooves import GrooveBase
 from ..hooks import HookHost, Hook
 
 
 class Profile(HookHost):
@@ -108,14 +108,39 @@
     microstructure_composition = Hook[dict[str, float]]()
     """Phase resp. constituent composition of the profile's material 
     as dict of constituent names to volume fractions (0 to 1)."""
 
     scale_thickness = Hook[float]()
     """Thickness of the scale covering the profile."""
 
+
+    longitudinal_stress = Hook[float]()
+    """Normal stress (principal stress) in rolling (x) direction. Positive means tension, negative pressure."""
+
+    altitudinal_stress = Hook[float]()
+    """Normal stress (principal stress) in thickness (y) direction. Positive means tension, negative pressure."""
+
+    latitudinal_stress = Hook[float]()
+    """Normal stress (principal stress) in width (z) direction. Positive means tension, negative pressure."""
+
+    longitudinal_strain = Hook[float]()
+    """Logarithmic normal strain (principal strain) in rolling (x) direction."""
+
+    altitudinal_strain = Hook[float]()
+    """Logarithmic normal strain (principal strain) in thickness (y) direction."""
+
+    latitudinal_strain = Hook[float]()
+    """Logarithmic normal strain (principal strain) in width (z) direction."""
+
+    hydrostatic_stress = Hook[float]()
+    """Hydrodynamic Stress."""
+
+    equivalent_stress = Hook[float]()
+    """Equivalent Stress."""
+
     deformation_activation_energy = Hook[float]()
     """Activation energy of deformation especially for calculation of Zener-Holomon-Parameter."""
 
     martensite_start_temperature = Hook[float]()
     """Martensite start temperature for the given chemical composition of the profile."""
 
     martensite_finish_temperature = Hook[float]()
@@ -131,14 +156,15 @@
     """Temperature at which austenite starts to transform into a mixture of ferrite and cementite during cooling."""
 
     ae3_temperature = Hook[float]()
     """Temperature above which the transformation of austenite into a mixture of ferrite and cementite is complete during cooling."""
 
     vickers_hardness = Hook[float]()
     """Vickers hardness of the cold profile material."""
+    
 
     def __init__(self, **kwargs):
         """Using the ``__init__`` is not recommended, use one of the factory class methods instead."""
         self.t = 0
         self.__dict__.update(kwargs)
         super().__init__()
```

### Comparing `pyroll_core-2.1.5/pyroll/core/roll/hookimpls.py` & `pyroll_core-2.1.6/pyroll/core/roll/hookimpls.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/roll/roll.py` & `pyroll_core-2.1.6/pyroll/core/roll/roll.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/roll_pass/deformation_unit.py` & `pyroll_core-2.1.6/pyroll/core/roll_pass/deformation_unit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,15 @@
+import numpy as np
+
+from typing import List
+from shapely.geometry import LineString
 from ..unit import Unit
 from ..hooks import Hook
+from shapely.geometry import LineString
+from typing import List
 
 
 class DeformationUnit(Unit):
     strain = Hook[float]()
     """Mean equivalent strain applied to the workpiece."""
 
     strain_rate = Hook[float]()
@@ -50,18 +56,39 @@
 
     free_surface_area = Hook[float]()
     """Area of free surface."""
 
     deformation_resistance = Hook[float]()
     """Equivalent deformation resistance (mean flow stress increased by deformation efficiency)."""
 
+    contact_pressure = Hook[float]()
+    """Pressure acting on the contact area."""
+
+    contact_friction = Hook[float]()
+    """Friction stress acting on the contact area."""
+
     zener_holomon_parameter = Hook[float]()
     """Temperature corrected strain rate acc. to Zener and Holomon."""
 
     class Profile(Unit.Profile):
         """Represents a profile in context of a deformation unit."""
 
+        contact_lines = Hook[List[LineString]]()
+        """List of lines that are in contact with tooling (rolls)."""
+
+        contact_angles = Hook[List[np.ndarray]]()
+        """List of contour angles that are in contact with tooling (rolls)."""
+
+        free_surface_lines = Hook[List[LineString]]()
+        """List of lines that are not in contact with tooling (rolls)."""
+
+        contact_width = Hook[float]()
+        """Projected width of contact lines."""
+
+        contact_depth = Hook[float]()
+        """Projected depth of contact lines."""
+
     class InProfile(Profile, Unit.InProfile):
         """Represents an incoming profile of a deformation unit."""
 
     class OutProfile(Profile, Unit.OutProfile):
         """Represents an outgoing profile of a deformation unit."""
```

### Comparing `pyroll_core-2.1.5/pyroll/core/roll_pass/roll_pass.py` & `pyroll_core-2.1.6/pyroll/core/roll_pass/roll_pass.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/roll_pass/three_roll_pass.py` & `pyroll_core-2.1.6/pyroll/core/roll_pass/three_roll_pass.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/roll_pass/hookimpls/helpers.py` & `pyroll_core-2.1.6/pyroll/core/roll_pass/hookimpls/helpers.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/roll_pass/hookimpls/profile.py` & `pyroll_core-2.1.6/pyroll/core/roll_pass/hookimpls/profile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from scipy.optimize import fixed_point
+import numpy as np
 from shapely.geometry import Polygon
+from shapely.affinity import translate, rotate
+from shapely.ops import linemerge
 
 from ..roll_pass import RollPass
 from ..three_roll_pass import ThreeRollPass
 
 from . import helpers
```

### Comparing `pyroll_core-2.1.5/pyroll/core/roll_pass/hookimpls/roll.py` & `pyroll_core-2.1.6/pyroll/core/roll_pass/hookimpls/roll.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/roll_pass/hookimpls/roll_pass.py` & `pyroll_core-2.1.6/pyroll/core/roll_pass/hookimpls/roll_pass.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/rotator/hookimpls.py` & `pyroll_core-2.1.6/pyroll/core/rotator/hookimpls.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/rotator/rotator.py` & `pyroll_core-2.1.6/pyroll/core/rotator/rotator.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/sequence/hookimpls.py` & `pyroll_core-2.1.6/pyroll/core/sequence/hookimpls.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/sequence/sequence.py` & `pyroll_core-2.1.6/pyroll/core/sequence/sequence.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/transport/cooling_pipe.py` & `pyroll_core-2.1.6/pyroll/core/transport/cooling_pipe.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/transport/transport.py` & `pyroll_core-2.1.6/pyroll/core/transport/transport.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/transport/hookimpls/cooling_pipe.py` & `pyroll_core-2.1.6/pyroll/core/transport/hookimpls/cooling_pipe.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/transport/hookimpls/transport.py` & `pyroll_core-2.1.6/pyroll/core/transport/hookimpls/transport.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/unit/hookimpls.py` & `pyroll_core-2.1.6/pyroll/core/unit/hookimpls.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyroll/core/unit/unit.py` & `pyroll_core-2.1.6/pyroll/core/unit/unit.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/.gitignore` & `pyroll_core-2.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/LICENSE` & `pyroll_core-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/README.md` & `pyroll_core-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/pyproject.toml` & `pyroll_core-2.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.1.5/PKG-INFO` & `pyroll_core-2.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroll-core
-Version: 2.1.5
+Version: 2.1.6
 Summary: PyRoll rolling simulation framework - core library.
 Project-URL: Homepage, https://pyroll-project.github.io
 Project-URL: Repository, https://github.com/pyroll-project/pyroll-core
 Project-URL: Documentation, https://pyroll.readthedocs.io/en/latest
 Author-email: Max Weiner <max.weiner@imf.tu-freiberg.de>, Christoph Renzing <christoph.renzing@imf.tu-freiberg.de>, Matthias Schmidtchen <matthias.schmidtchen@imf.tu-freiberg.de>, Max Stirl <max.stirl@imf.tu-freiberg.de>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
```

