# Comparing `tmp/mujoco-mjx-3.1.3.tar.gz` & `tmp/mujoco-mjx-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mujoco-mjx-3.1.3.tar", last modified: Tue Mar  5 21:09:16 2024, max compression
+gzip compressed data, was "mujoco-mjx-3.1.4.tar", last modified: Wed Apr 10 17:18:45 2024, max compression
```

## Comparing `mujoco-mjx-3.1.3.tar` & `mujoco-mjx-3.1.4.tar`

### file list

```diff
@@ -1,108 +1,121 @@
-drwxr-sr-x   0 root         (0)     1002        0 2024-03-05 21:09:16.931487 mujoco-mjx-3.1.3/
--rw-r--r--   0 root         (0)     1002    11358 2024-03-05 21:09:09.000000 mujoco-mjx-3.1.3/LICENSE
--rw-rw-r--   0 root         (0)     1002       41 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1002     3382 2024-03-05 21:09:16.931487 mujoco-mjx-3.1.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1002     2063 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/README.md
-drwxr-sr-x   0 root         (0)     1002        0 2024-03-05 21:09:16.887483 mujoco-mjx-3.1.3/mujoco/
-drwxr-sr-x   0 root         (0)     1002        0 2024-03-05 21:09:16.891484 mujoco-mjx-3.1.3/mujoco/mjx/
--rw-rw-r--   0 root         (0)     1002     2268 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/__init__.py
-drwxr-sr-x   0 root         (0)     1002        0 2024-03-05 21:09:16.899484 mujoco-mjx-3.1.3/mujoco/mjx/_src/
--rw-rw-r--   0 root         (0)     1002      674 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/__init__.py
--rw-rw-r--   0 root         (0)     1002     1701 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/collision_base.py
--rw-rw-r--   0 root         (0)     1002    25021 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/collision_convex.py
--rw-rw-r--   0 root         (0)     1002    14120 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/collision_driver.py
--rw-rw-r--   0 root         (0)     1002    17856 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/collision_driver_test.py
--rw-rw-r--   0 root         (0)     1002     4453 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/collision_primitive.py
--rw-rw-r--   0 root         (0)     1002    12899 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/constraint.py
--rw-rw-r--   0 root         (0)     1002     3831 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/constraint_test.py
--rw-rw-r--   0 root         (0)     1002     4792 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/dataclasses.py
--rw-rw-r--   0 root         (0)     1002    10263 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/device.py
--rw-rw-r--   0 root         (0)     1002     6540 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/device_test.py
--rw-rw-r--   0 root         (0)     1002    10865 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/forward.py
--rw-rw-r--   0 root         (0)     1002     6422 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/forward_test.py
--rw-rw-r--   0 root         (0)     1002    14295 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/io.py
--rw-rw-r--   0 root         (0)     1002    16652 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/io_test.py
--rw-rw-r--   0 root         (0)     1002    10647 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/math.py
--rw-rw-r--   0 root         (0)     1002     7514 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/math_test.py
--rw-rw-r--   0 root         (0)     1002     7884 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/mesh.py
--rw-rw-r--   0 root         (0)     1002     4285 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/mesh_test.py
--rw-rw-r--   0 root         (0)     1002     4472 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/passive.py
--rw-rw-r--   0 root         (0)     1002     2566 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/passive_test.py
--rw-rw-r--   0 root         (0)     1002     8487 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/ray.py
--rw-rw-r--   0 root         (0)     1002     9529 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/ray_test.py
--rw-rw-r--   0 root         (0)     1002    16662 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/scan.py
--rw-rw-r--   0 root         (0)     1002     9042 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/scan_test.py
--rw-rw-r--   0 root         (0)     1002    17959 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/smooth.py
--rw-rw-r--   0 root         (0)     1002     5546 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/smooth_test.py
--rw-rw-r--   0 root         (0)     1002    12100 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/solver.py
--rw-rw-r--   0 root         (0)     1002     4426 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/solver_test.py
--rw-rw-r--   0 root         (0)     1002     5911 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/support.py
--rw-rw-r--   0 root         (0)     1002     4658 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/support_test.py
--rw-rw-r--   0 root         (0)     1002    11963 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/test_util.py
--rw-rw-r--   0 root         (0)     1002    28817 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/_src/types.py
-drwxr-sr-x   0 root         (0)     1002        0 2024-03-05 21:09:16.899484 mujoco-mjx-3.1.3/mujoco/mjx/integration_test/
--rw-rw-r--   0 root         (0)     1002     3045 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/integration_test/collision_driver_test.py
--rw-rw-r--   0 root         (0)     1002     2222 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/integration_test/forward_test.py
--rw-rw-r--   0 root         (0)     1002     2539 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/integration_test/smooth_test.py
-drwxr-sr-x   0 root         (0)     1002        0 2024-03-05 21:09:16.899484 mujoco-mjx-3.1.3/mujoco/mjx/test_data/
-drwxr-sr-x   0 root         (0)     1002        0 2024-03-05 21:09:16.899484 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/
--rw-rw-r--   0 root         (0)     1002     1792 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/README.md
-drwxr-sr-x   0 root         (0)     1002        0 2024-03-05 21:09:16.915486 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/
--rw-rw-r--   0 root         (0)     1002   429334 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/abduction.stl
--rw-rw-r--   0 root         (0)     1002    14998 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/barkour_v0_mjx.xml
--rw-rw-r--   0 root         (0)     1002  1169584 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/body.stl
--rw-rw-r--   0 root         (0)     1002    23384 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/foot.stl
--rw-rw-r--   0 root         (0)     1002   739084 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/handle.stl
--rw-rw-r--   0 root         (0)     1002   267584 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/head.stl
--rw-rw-r--   0 root         (0)     1002   163984 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/head_mount.stl
--rw-rw-r--   0 root         (0)     1002   523084 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/lower_leg_1to1.stl
--rw-rw-r--   0 root         (0)     1002  1199984 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/powercable.stl
--rw-rw-r--   0 root         (0)     1002   530834 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/upper_left_1.stl
--rw-rw-r--   0 root         (0)     1002   628484 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/upper_left_2.stl
--rw-rw-r--   0 root         (0)     1002  1500284 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/upper_left_3.stl
--rw-rw-r--   0 root         (0)     1002  1106034 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/upper_right_1.stl
--rw-rw-r--   0 root         (0)     1002   670284 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/upper_right_2.stl
--rw-rw-r--   0 root         (0)     1002  1521284 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/upper_right_3.stl
--rw-rw-r--   0 root         (0)     1002     1677 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/constraints.xml
--rw-rw-r--   0 root         (0)     1002     2366 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/convex.xml
-drwxr-sr-x   0 root         (0)     1002        0 2024-03-05 21:09:16.919486 mujoco-mjx-3.1.3/mujoco/mjx/test_data/humanoid/
--rw-rw-r--   0 root         (0)     1002      909 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/humanoid/README.md
--rw-rw-r--   0 root         (0)     1002   397686 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/humanoid/humanoid.png
--rw-rw-r--   0 root         (0)     1002    11271 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/humanoid/humanoid.xml
-drwxr-sr-x   0 root         (0)     1002        0 2024-03-05 21:09:16.919486 mujoco-mjx-3.1.3/mujoco/mjx/test_data/meshes/
--rw-rw-r--   0 root         (0)     1002     1884 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/meshes/dodecahedron.stl
--rw-rw-r--   0 root         (0)     1002      384 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/meshes/pyramid.stl
--rw-rw-r--   0 root         (0)     1002      284 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/meshes/tetrahedron.stl
--rw-rw-r--   0 root         (0)     1002     3776 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/pendula.xml
--rw-rw-r--   0 root         (0)     1002     1231 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/ray.xml
-drwxr-sr-x   0 root         (0)     1002        0 2024-03-05 21:09:16.919486 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/
--rw-rw-r--   0 root         (0)     1002      961 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/README.md
-drwxr-sr-x   0 root         (0)     1002        0 2024-03-05 21:09:16.931487 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/
--rw-rw-r--   0 root         (0)     1002   341254 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/f_distal_pst.obj
--rw-rw-r--   0 root         (0)     1002    34351 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/f_knuckle.obj
--rw-rw-r--   0 root         (0)     1002    25738 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/f_middle.obj
--rw-rw-r--   0 root         (0)     1002    64846 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/f_proximal.obj
--rw-rw-r--   0 root         (0)     1002    80439 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/forearm_0.obj
--rw-rw-r--   0 root         (0)     1002  1433615 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/forearm_1.obj
--rw-rw-r--   0 root         (0)     1002    26812 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/forearm_collision.obj
--rw-rw-r--   0 root         (0)     1002    88696 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/lf_metacarpal.obj
--rw-rw-r--   0 root         (0)     1002   118690 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/mounting_plate.obj
--rw-rw-r--   0 root         (0)     1002   775747 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/palm.obj
--rw-rw-r--   0 root         (0)     1002   300842 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/th_distal_pst.obj
--rw-rw-r--   0 root         (0)     1002    75080 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/th_middle.obj
--rw-rw-r--   0 root         (0)     1002    23772 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/th_proximal.obj
--rw-rw-r--   0 root         (0)     1002   110838 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/wrist.obj
--rw-rw-r--   0 root         (0)     1002    18308 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/right_hand.xml
--rw-rw-r--   0 root         (0)     1002     1112 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/scene_right.xml
--rw-rw-r--   0 root         (0)     1002  1315458 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/shadow_hand.png
--rw-rw-r--   0 root         (0)     1002     3811 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/testspeed.py
--rw-rw-r--   0 root         (0)     1002     2538 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/mujoco/mjx/viewer.py
-drwxr-sr-x   0 root         (0)     1002        0 2024-03-05 21:09:16.931487 mujoco-mjx-3.1.3/mujoco_mjx.egg-info/
--rw-r--r--   0 root         (0)     1002     3382 2024-03-05 21:09:16.000000 mujoco-mjx-3.1.3/mujoco_mjx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1002     3629 2024-03-05 21:09:16.000000 mujoco-mjx-3.1.3/mujoco_mjx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1002        1 2024-03-05 21:09:16.000000 mujoco-mjx-3.1.3/mujoco_mjx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1002       96 2024-03-05 21:09:16.000000 mujoco-mjx-3.1.3/mujoco_mjx.egg-info/entry_points.txt
--rw-r--r--   0 root         (0)     1002       65 2024-03-05 21:09:16.000000 mujoco-mjx-3.1.3/mujoco_mjx.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1002        7 2024-03-05 21:09:16.000000 mujoco-mjx-3.1.3/mujoco_mjx.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1002     1437 2024-03-05 21:01:39.000000 mujoco-mjx-3.1.3/pyproject.toml
--rw-r--r--   0 root         (0)     1002       38 2024-03-05 21:09:16.931487 mujoco-mjx-3.1.3/setup.cfg
+drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.080092 mujoco-mjx-3.1.4/
+-rw-r--r--   0 root         (0)     1002    11358 2024-04-10 17:18:38.000000 mujoco-mjx-3.1.4/LICENSE
+-rw-rw-r--   0 root         (0)     1002       41 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0)     1002     3382 2024-04-10 17:18:45.080092 mujoco-mjx-3.1.4/PKG-INFO
+-rw-rw-r--   0 root         (0)     1002     2063 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/README.md
+drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.032087 mujoco-mjx-3.1.4/mujoco/
+drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.036088 mujoco-mjx-3.1.4/mujoco/mjx/
+-rw-rw-r--   0 root         (0)     1002     2372 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/__init__.py
+drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.044088 mujoco-mjx-3.1.4/mujoco/mjx/_src/
+-rw-rw-r--   0 root         (0)     1002      674 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/__init__.py
+-rw-rw-r--   0 root         (0)     1002     1787 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_base.py
+-rw-rw-r--   0 root         (0)     1002    32800 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_convex.py
+-rw-rw-r--   0 root         (0)     1002    14855 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_driver.py
+-rw-rw-r--   0 root         (0)     1002    26782 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_driver_test.py
+-rw-rw-r--   0 root         (0)     1002     4957 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_primitive.py
+-rw-rw-r--   0 root         (0)     1002     4744 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_sdf.py
+-rw-rw-r--   0 root         (0)     1002    12899 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/constraint.py
+-rw-rw-r--   0 root         (0)     1002     3831 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/constraint_test.py
+-rw-rw-r--   0 root         (0)     1002     4792 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/dataclasses.py
+-rw-rw-r--   0 root         (0)     1002    10540 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/device.py
+-rw-rw-r--   0 root         (0)     1002     6540 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/device_test.py
+-rw-rw-r--   0 root         (0)     1002    10865 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/forward.py
+-rw-rw-r--   0 root         (0)     1002     6422 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/forward_test.py
+-rw-rw-r--   0 root         (0)     1002    14803 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/io.py
+-rw-rw-r--   0 root         (0)     1002    17818 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/io_test.py
+-rw-rw-r--   0 root         (0)     1002    10768 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/math.py
+-rw-rw-r--   0 root         (0)     1002     7514 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/math_test.py
+-rw-rw-r--   0 root         (0)     1002    11153 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/mesh.py
+-rw-rw-r--   0 root         (0)     1002     5700 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/mesh_test.py
+-rw-rw-r--   0 root         (0)     1002     4472 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/passive.py
+-rw-rw-r--   0 root         (0)     1002     2566 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/passive_test.py
+-rw-rw-r--   0 root         (0)     1002     8487 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/ray.py
+-rw-rw-r--   0 root         (0)     1002     9529 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/ray_test.py
+-rw-rw-r--   0 root         (0)     1002    16662 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/scan.py
+-rw-rw-r--   0 root         (0)     1002     9042 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/scan_test.py
+-rw-rw-r--   0 root         (0)     1002    17959 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/smooth.py
+-rw-rw-r--   0 root         (0)     1002     5546 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/smooth_test.py
+-rw-rw-r--   0 root         (0)     1002    12100 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/solver.py
+-rw-rw-r--   0 root         (0)     1002     4426 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/solver_test.py
+-rw-rw-r--   0 root         (0)     1002     5910 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/support.py
+-rw-rw-r--   0 root         (0)     1002     4658 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/support_test.py
+-rw-rw-r--   0 root         (0)     1002    13854 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/test_util.py
+-rw-rw-r--   0 root         (0)     1002    29238 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/types.py
+drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.044088 mujoco-mjx-3.1.4/mujoco/mjx/integration_test/
+-rw-rw-r--   0 root         (0)     1002     3045 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/integration_test/collision_driver_test.py
+-rw-rw-r--   0 root         (0)     1002     2222 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/integration_test/forward_test.py
+-rw-rw-r--   0 root         (0)     1002     2539 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/integration_test/smooth_test.py
+drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.044088 mujoco-mjx-3.1.4/mujoco/mjx/test_data/
+drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.044088 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/
+-rw-rw-r--   0 root         (0)     1002     1792 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/README.md
+drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.060090 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/
+-rw-rw-r--   0 root         (0)     1002   429334 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/abduction.stl
+-rw-rw-r--   0 root         (0)     1002    14998 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/barkour_v0_mjx.xml
+-rw-rw-r--   0 root         (0)     1002  1169584 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/body.stl
+-rw-rw-r--   0 root         (0)     1002    23384 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/foot.stl
+-rw-rw-r--   0 root         (0)     1002   739084 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/handle.stl
+-rw-rw-r--   0 root         (0)     1002   267584 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/head.stl
+-rw-rw-r--   0 root         (0)     1002   163984 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/head_mount.stl
+-rw-rw-r--   0 root         (0)     1002   523084 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/lower_leg_1to1.stl
+-rw-rw-r--   0 root         (0)     1002  1199984 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/powercable.stl
+-rw-rw-r--   0 root         (0)     1002   530834 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_left_1.stl
+-rw-rw-r--   0 root         (0)     1002   628484 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_left_2.stl
+-rw-rw-r--   0 root         (0)     1002  1500284 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_left_3.stl
+-rw-rw-r--   0 root         (0)     1002  1106034 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_right_1.stl
+-rw-rw-r--   0 root         (0)     1002   670284 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_right_2.stl
+-rw-rw-r--   0 root         (0)     1002  1521284 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_right_3.stl
+-rw-rw-r--   0 root         (0)     1002     1677 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/constraints.xml
+-rw-rw-r--   0 root         (0)     1002     2366 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/convex.xml
+drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.064090 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/
+-rw-rw-r--   0 root         (0)     1002     7750 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/01_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    13884 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/02_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    19973 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/03_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    26060 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/04_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    32147 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/05_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    38237 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/06_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    44328 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/07_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    50416 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/08_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    56509 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/09_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    62687 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/10_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002      909 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/README.md
+-rw-rw-r--   0 root         (0)     1002   397686 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/humanoid.png
+-rw-rw-r--   0 root         (0)     1002    11271 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/humanoid.xml
+drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.064090 mujoco-mjx-3.1.4/mujoco/mjx/test_data/meshes/
+-rw-rw-r--   0 root         (0)     1002     1884 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/meshes/dodecahedron.stl
+-rw-rw-r--   0 root         (0)     1002      384 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/meshes/pyramid.stl
+-rw-rw-r--   0 root         (0)     1002      284 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/meshes/tetrahedron.stl
+-rw-rw-r--   0 root         (0)     1002     3776 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/pendula.xml
+-rw-rw-r--   0 root         (0)     1002     1231 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/ray.xml
+drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.068091 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/
+-rw-rw-r--   0 root         (0)     1002      961 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/README.md
+drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.076091 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/
+-rw-rw-r--   0 root         (0)     1002   341254 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_distal_pst.obj
+-rw-rw-r--   0 root         (0)     1002     6447 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_distal_pst_214.obj
+-rw-rw-r--   0 root         (0)     1002    34351 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_knuckle.obj
+-rw-rw-r--   0 root         (0)     1002    25738 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_middle.obj
+-rw-rw-r--   0 root         (0)     1002    64846 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_proximal.obj
+-rw-rw-r--   0 root         (0)     1002    80439 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/forearm_0.obj
+-rw-rw-r--   0 root         (0)     1002  1433615 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/forearm_1.obj
+-rw-rw-r--   0 root         (0)     1002    26812 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/forearm_collision.obj
+-rw-rw-r--   0 root         (0)     1002    88696 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/lf_metacarpal.obj
+-rw-rw-r--   0 root         (0)     1002   118690 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/mounting_plate.obj
+-rw-rw-r--   0 root         (0)     1002   775747 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/palm.obj
+-rw-rw-r--   0 root         (0)     1002   300842 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/th_distal_pst.obj
+-rw-rw-r--   0 root         (0)     1002     5639 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/th_distal_pst_190.obj
+-rw-rw-r--   0 root         (0)     1002    75080 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/th_middle.obj
+-rw-rw-r--   0 root         (0)     1002    23772 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/th_proximal.obj
+-rw-rw-r--   0 root         (0)     1002   110838 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/wrist.obj
+-rw-rw-r--   0 root         (0)     1002    18568 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/right_hand.xml
+-rw-rw-r--   0 root         (0)     1002     1112 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/scene_right.xml
+-rw-rw-r--   0 root         (0)     1002  1315458 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/shadow_hand.png
+-rw-rw-r--   0 root         (0)     1002     2747 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/testspeed.py
+-rw-rw-r--   0 root         (0)     1002     2462 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/viewer.py
+drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.080092 mujoco-mjx-3.1.4/mujoco_mjx.egg-info/
+-rw-r--r--   0 root         (0)     1002     3382 2024-04-10 17:18:45.000000 mujoco-mjx-3.1.4/mujoco_mjx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1002     4255 2024-04-10 17:18:45.000000 mujoco-mjx-3.1.4/mujoco_mjx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1002        1 2024-04-10 17:18:45.000000 mujoco-mjx-3.1.4/mujoco_mjx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1002       96 2024-04-10 17:18:45.000000 mujoco-mjx-3.1.4/mujoco_mjx.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0)     1002       65 2024-04-10 17:18:45.000000 mujoco-mjx-3.1.4/mujoco_mjx.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1002        7 2024-04-10 17:18:45.000000 mujoco-mjx-3.1.4/mujoco_mjx.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1002     1437 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/pyproject.toml
+-rw-r--r--   0 root         (0)     1002       38 2024-04-10 17:18:45.080092 mujoco-mjx-3.1.4/setup.cfg
```

### Comparing `mujoco-mjx-3.1.3/LICENSE` & `mujoco-mjx-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/PKG-INFO` & `mujoco-mjx-3.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mujoco-mjx
-Version: 3.1.3
+Version: 3.1.4
 Summary: MuJoCo XLA (MJX)
 Author-email: Google DeepMind <mujoco@deepmind.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/google-deepmind/mujoco/tree/main/mjx
-Project-URL: Documentation, https://mujoco.readthedocs.io/en/3.1.3
+Project-URL: Documentation, https://mujoco.readthedocs.io/en/3.1.4
 Project-URL: Repository, https://github.com/google-deepmind/mujoco/tree/main/mjx
-Project-URL: Changelog, https://mujoco.readthedocs.io/en/3.1.3/changelog.html
+Project-URL: Changelog, https://mujoco.readthedocs.io/en/3.1.4/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -23,15 +23,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: absl-py
 Requires-Dist: etils[epath]
 Requires-Dist: jax
 Requires-Dist: jaxlib
-Requires-Dist: mujoco>=3.1.3.dev0
+Requires-Dist: mujoco>=3.1.4.dev0
 Requires-Dist: scipy
 Requires-Dist: trimesh
 
 # MuJoCo XLA (MJX)
 
 [![PyPI Python Version][pypi-versions-badge]][pypi]
 [![PyPI version][pypi-badge]][pypi]
```

### Comparing `mujoco-mjx-3.1.3/README.md` & `mujoco-mjx-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/__init__.py` & `mujoco-mjx-3.1.4/mujoco/mjx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Public API for MJX."""
 
 # pylint:disable=g-importing-member
 from mujoco.mjx._src.collision_driver import collision
+from mujoco.mjx._src.collision_driver import get_params
 from mujoco.mjx._src.collision_driver import ncon
 from mujoco.mjx._src.constraint import count_constraints
 from mujoco.mjx._src.constraint import make_constraint
 from mujoco.mjx._src.device import device_get_into
 from mujoco.mjx._src.device import device_put
 from mujoco.mjx._src.forward import euler
 from mujoco.mjx._src.forward import forward
@@ -44,8 +45,9 @@
 from mujoco.mjx._src.smooth import kinematics
 from mujoco.mjx._src.smooth import rne
 from mujoco.mjx._src.smooth import transmission
 from mujoco.mjx._src.solver import solve
 from mujoco.mjx._src.support import full_m
 from mujoco.mjx._src.support import is_sparse
 from mujoco.mjx._src.support import mul_m
+from mujoco.mjx._src.test_util import benchmark
 from mujoco.mjx._src.types import *
```

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/__init__.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/collision_base.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,16 +46,18 @@
 
   geom_id: jax.Array
   pos: jax.Array
   mat: jax.Array
   size: jax.Array
   face: Optional[jax.Array] = None
   vert: Optional[jax.Array] = None
-  edge: Optional[jax.Array] = None
+  edge_dir: Optional[jax.Array] = None
   facenorm: Optional[jax.Array] = None
+  edge: Optional[jax.Array] = None
+  edge_face_normal: Optional[jax.Array] = None
 
 
 class SolverParams(PyTreeNode):
   """Contact solver params."""
 
   friction: jax.Array
   solref: jax.Array
```

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/collision_convex.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_convex.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Convex collisions."""
 
+import functools
 from typing import Tuple
 
 import jax
 from jax import numpy as jp
 from mujoco.mjx._src import math
 # pylint: disable=g-importing-member
 from mujoco.mjx._src.collision_base import Contact
@@ -173,14 +174,229 @@
   bp = b - poly
   dist_bp = jp.abs(bp.dot(bc)) + dist_mask
   dist_ap = jp.abs(ap.dot(ac)) + dist_mask
   d_idx = (dist_bp + dist_ap).argmax() % poly.shape[0]
   return jp.array([a_idx, b_idx, c_idx, d_idx])
 
 
+def plane_convex(plane: GeomInfo, convex: GeomInfo) -> Contact:
+  """Calculates contacts between a plane and a convex object."""
+  vert = convex.vert
+
+  # get points in the convex frame
+  plane_pos = convex.mat.T @ (plane.pos - convex.pos)
+  n = convex.mat.T @ plane.mat[:, 2]
+  support = (plane_pos - vert) @ n
+  idx = _manifold_points(vert, support > 0, n)
+  pos = vert[idx]
+
+  # convert to world frame
+  pos = convex.pos + pos @ convex.mat.T
+  n = plane.mat[:, 2]
+
+  frame = jp.stack([math.make_frame(n)] * 4, axis=0)
+  unique = jp.tril(idx == idx[:, None]).sum(axis=1) == 1
+  dist = jp.where(unique, -support[idx], 1)
+  pos = pos - 0.5 * dist[:, None] * n
+  return dist, pos, frame
+
+
+def sphere_convex(sphere: GeomInfo, convex: GeomInfo) -> Contact:
+  """Calculates contact between a sphere and a convex object."""
+  faces = convex.face
+  normals = convex.facenorm
+
+  # Put sphere in convex frame.
+  sphere_pos = convex.mat.T @ (sphere.pos - convex.pos)
+
+  # Get support from face normals.
+  @jax.vmap
+  def get_support(faces, normal):
+    pos = sphere_pos - normal * sphere.size[0]
+    return jp.dot(pos - faces[0], normal)
+
+  support = get_support(faces, normals)
+  has_separating_axis = jp.any(support >= 0)
+
+  # Pick the face with the best separating axis.
+  best_idx = support.argmax()
+  face = faces[best_idx]
+  face_normal = normals[best_idx]
+
+  # Get closest point between the polygon face and the sphere center point.
+  # Project the sphere center point onto poly plane. If it's inside polygon
+  # side planes, then we're done.
+  pt = _project_pt_onto_plane(sphere_pos, face[0], face_normal)
+  edge_p0 = jp.roll(face, 1, axis=0)
+  edge_p1 = face
+  side_normals = jax.vmap(jp.cross, in_axes=[0, None])(
+      edge_p1 - edge_p0,
+      face_normal,
+  )
+  edge_dist = jax.vmap(
+      lambda plane_pt, plane_norm: (pt - plane_pt).dot(plane_norm)
+  )(edge_p0, side_normals)
+  pt_on_face = jp.all(edge_dist <= 0)  # lte to handle degenerate edges
+
+  # If the point is outside side planes, project onto the closest side plane
+  # that the point is in front of.
+  degenerate_edge = jp.all(side_normals == 0, axis=1)
+  behind = edge_dist < 0.0
+  edge_dist = jp.where(degenerate_edge | behind, 1e12, edge_dist)
+  idx = edge_dist.argmin()
+  edge_pt = math.closest_segment_point(edge_p0[idx], edge_p1[idx], pt)
+  pt = jp.where(pt_on_face, pt, edge_pt)
+
+  # Get the normal, dist, and contact position.
+  pt_normal, d = math.normalize_with_norm(pt - sphere_pos)
+  # Ensure normal points towards convex centroid.
+  inside = jp.dot(pt, pt_normal) > 0
+  sign = jp.where(inside, -1, 1)
+  n = jp.where(pt_on_face | (d < 1e-6), -face_normal, sign * pt_normal)
+  d *= sign
+
+  spt = sphere_pos + n * sphere.size[0]
+  dist = jp.where(has_separating_axis, 1.0, d - sphere.size[0])
+  pos = (pt + spt) * 0.5
+
+  # Go back to world frame.
+  n = convex.mat @ n
+  pos = convex.mat @ pos + convex.pos
+
+  return jax.tree_map(
+      lambda x: jp.expand_dims(x, axis=0), (dist, pos, math.make_frame(n))
+  )
+
+
+def capsule_convex(cap: GeomInfo, convex: GeomInfo) -> Contact:
+  """Calculates contacts between a capsule and a convex object."""
+  # Get convex transformed normals, faces, and vertices.
+  faces = convex.face
+  normals = convex.facenorm
+
+  # Put capsule in convex frame.
+  cap_pos = convex.mat.T @ (cap.pos - convex.pos)
+  axis, length = cap.mat[:, 2], cap.size[1]
+  axis = convex.mat.T @ axis
+  seg = axis * length
+  cap_pts = jp.array([
+      cap_pos - seg,
+      cap_pos + seg,
+  ])
+
+  # Get support from face normals.
+  @jax.vmap
+  def get_support(face, normal):
+    pts = cap_pts - normal * cap.size[0]
+    sup = jax.vmap(lambda x: jp.dot(x - face[0], normal))(pts)
+    return sup.min()
+
+  support = get_support(faces, normals)
+  has_support = jp.all(support < 0)
+
+  # Pick the face with minimal penetration.
+  best_idx = support.argmax()
+  face = faces[best_idx]
+  normal = normals[best_idx]
+
+  # Clip the segment against side planes and create two contact points against
+  # the face.
+  edge_p0 = jp.roll(face, 1, axis=0)
+  edge_p1 = face
+  side_planes = jax.vmap(jp.cross, in_axes=[0, None])(
+      edge_p1 - edge_p0,
+      normal,
+  )
+  cap_pts_clipped, mask = _clip_edge_to_planes(
+      cap_pts[0], cap_pts[1], edge_p0, side_planes
+  )
+  cap_pts_clipped = cap_pts_clipped - normal * cap.size[0]
+  face_pts = jax.vmap(_project_pt_onto_plane, in_axes=[0, None, None])(
+      cap_pts_clipped, face[0], normal
+  )
+  # Create variables for the face contact.
+  pos = (cap_pts_clipped + face_pts) * 0.5
+  contact_normal = -jp.stack([normal] * 2, 0)
+  face_penetration = jp.where(
+      mask & has_support, jp.dot(face_pts - cap_pts_clipped, normal), -1
+  )
+
+  # Pick a potential shallow edge contact.
+  def get_edge_axis(edge):
+    edge_closest_pt, cap_closest_pt = math.closest_segment_to_segment_points(
+        edge[0], edge[1], cap_pts[0], cap_pts[1]
+    )
+    edge_dir = edge_closest_pt - cap_closest_pt
+    degenerate_edge_dir = jp.sum(jp.square(edge_dir)) < 1e-6
+    edge_axis, edge_dist = math.normalize_with_norm(edge_dir)
+    return (
+        edge_dist,
+        edge_axis,
+        degenerate_edge_dir,
+        edge_closest_pt,
+        cap_closest_pt,
+    )
+
+  edge = jp.take(convex.vert, convex.edge, axis=0)
+  edge_face_normal = convex.edge_face_normal  # pytype: disable=attribute-error
+
+  res = jax.vmap(get_edge_axis)(edge.reshape(-1, 2, 3))
+  e_idx = jp.abs(res[0]).argmin()
+  (
+      edge_dist,
+      edge_axis,
+      degenerate_edge_dir,
+      edge_closest_pt,
+      cap_closest_pt,
+  ) = jax.tree_map(lambda x, i=e_idx: jp.take(x, i, axis=0), res)
+
+  edge_face_normals = edge_face_normal[e_idx]
+  edge_voronoi_front = ((edge_face_normals @ edge_axis) < 0).all()
+  shallow = ~degenerate_edge_dir & edge_voronoi_front
+  edge_penetration = jp.where(shallow, cap.size[0] - edge_dist, -1)
+
+  # Determine edge contact position.
+  edge_pos = (
+      edge_closest_pt + (cap_closest_pt + edge_axis * cap.size[0])
+  ) * 0.5
+  edge_dir_parallel_to_face = (
+      jp.abs(edge_axis.dot(normal)) > 0.99
+  ) & ~degenerate_edge_dir
+  min_face_penetration = face_penetration.min()
+  has_edge_contact = (
+      (edge_penetration > 0)
+      # prefer edge contact if the edge is smaller than face penetration
+      & jp.where(
+          min_face_penetration > 0,
+          edge_penetration < min_face_penetration,
+          True,
+      )
+      # prefer face contact if the edge axis is parallel to the face normal
+      & ~edge_dir_parallel_to_face
+      # make sure we have a shallow contact
+      & edge_voronoi_front
+  )
+
+  # Get the contact info.
+  pos = jp.where(has_edge_contact, pos.at[0].set(edge_pos), pos)
+  n = jp.where(
+      has_edge_contact, contact_normal.at[0].set(edge_axis), contact_normal
+  )
+
+  # Go back to world frame.
+  pos = convex.pos + pos @ convex.mat.T
+  n = n @ convex.mat.T
+
+  dist = -jp.where(
+      has_edge_contact, jp.array([edge_penetration, -1]), face_penetration
+  )
+  frame = jax.vmap(math.make_frame)(n)
+  return dist, pos, frame
+
+
 def _project_pt_onto_plane(
     pt: jax.Array, plane_pt: jax.Array, plane_normal: jax.Array
 ) -> jax.Array:
   """Projects a point onto a plane along the plane normal."""
   dist = (pt - plane_pt).dot(plane_normal)
   return pt - dist * plane_normal
 
@@ -392,15 +608,15 @@
 
   dist = jp.where(mask_pts, -penetration, jp.ones_like(penetration))
   pos = contact_pts
   normal = -jp.stack([sep_axis] * 4, 0)
   return dist, pos, normal
 
 
-def _sat_hull_hull(
+def _sat_bruteforce(
     faces_a: jax.Array,
     faces_b: jax.Array,
     vertices_a: jax.Array,
     vertices_b: jax.Array,
     normals_a: jax.Array,
     normals_b: jax.Array,
     unique_edges_a: jax.Array,
@@ -410,62 +626,72 @@
 
   Given two convex hulls, the Separating Axis Test finds a separating axis
   between all edge pairs and face pairs. Edge pairs create a single contact
   point and face pairs create a contact manifold (up to four contact points).
   We return both the edge and face contacts. Valid contacts can be checked with
   dist < 0. Resulting edge contacts should be preferred over face contacts.
 
+  This method checks all separating axes via a brute force support function, and
+  is thus costly to run over large meshes, but is more performant for smaller
+  meshes (boxes, tetrahedra, etc.).
+
   Args:
-    faces_a: An ndarray of hull A's polygon faces.
-    faces_b: An ndarray of hull B's polygon faces.
+    faces_a: Faces for hull A.
+    faces_b: Faces for hull B.
     vertices_a: Vertices for hull A.
     vertices_b: Vertices for hull B.
-    normals_a: Normal vectors for hull A's polygon faces.
-    normals_b: Normal vectors for hull B's polygon faces.
+    normals_a: Normal vectors for hull A faces.
+    normals_b: Normal vectors for hull B faces.
     unique_edges_a: Unique edges for hull A.
     unique_edges_b: Unique edges for hull B.
 
   Returns:
     tuple of dist, pos, and normal
   """
   # get the separating axes
-  edge_dir_a = unique_edges_a[:, 0] - unique_edges_a[:, 1]
-  edge_dir_b = unique_edges_b[:, 0] - unique_edges_b[:, 1]
+  v_norm = jax.vmap(math.normalize)
+  edge_dir_a = v_norm(unique_edges_a[:, 0] - unique_edges_a[:, 1])
+  edge_dir_b = v_norm(unique_edges_b[:, 0] - unique_edges_b[:, 1])
   edge_dir_a_r = jp.tile(edge_dir_a, reps=(unique_edges_b.shape[0], 1))
   edge_dir_b_r = jp.repeat(edge_dir_b, repeats=unique_edges_a.shape[0], axis=0)
-  edge_edge_axes = jax.vmap(jp.cross)(edge_dir_a_r, edge_dir_b_r)
-  edge_edge_axes = jax.vmap(lambda x: math.normalize(x, axis=0))(
-      edge_edge_axes
+  edge_axes = jax.vmap(jp.cross)(edge_dir_a_r, edge_dir_b_r)
+  degenerate_edge_axes = (edge_axes**2).sum(axis=1) < 1e-6
+  edge_axes = jax.vmap(lambda x: math.normalize(x, axis=0))(edge_axes)
+  n_norm = normals_a.shape[0] + normals_b.shape[0]
+  degenerate_axes = jp.concatenate(
+      [jp.array([False] * n_norm), degenerate_edge_axes]
   )
 
-  axes = jp.concatenate([normals_a, normals_b, edge_edge_axes])
+  axes = jp.concatenate([normals_a, normals_b, edge_axes])
 
   # for each separating axis, get the support
   @jax.vmap
-  def get_support(axis):
-    support_a = jax.vmap(jp.dot, in_axes=[None, 0])(axis, vertices_a)
-    support_b = jax.vmap(jp.dot, in_axes=[None, 0])(axis, vertices_b)
+  def get_support(axis, is_degenerate):
+    # the matmul here is more performant with vmap(dot)
+    dot = functools.partial(jp.dot, precision=jax.lax.Precision.HIGH)
+    support_a = jax.vmap(dot, in_axes=[None, 0])(axis, vertices_a)
+    support_b = jax.vmap(dot, in_axes=[None, 0])(axis, vertices_b)
     dist1 = support_a.max() - support_b.min()
     dist2 = support_b.max() - support_a.min()
     sign = jp.where(dist1 > dist2, -1, 1)
     dist = jp.minimum(dist1, dist2)
-    dist = jp.where(~jp.all(axis == 0.0), dist, 1e6)  # degenerate axis
+    dist = jp.where(~is_degenerate, dist, 1e6)  # degenerate axis
     return dist, sign
 
-  support, sign = get_support(axes)
+  support, sign = get_support(axes, degenerate_axes)
 
   # choose the best separating axis
   best_idx = jp.argmin(support)
   best_sign = sign[best_idx]
   best_axis = axes[best_idx]
   is_edge_contact = best_idx >= (normals_a.shape[0] + normals_b.shape[0])
 
   # get the (reference) face most aligned with the separating axis
-  dist_a = jax.vmap(jp.dot, in_axes=[None, 0])(best_axis, normals_a)
-  dist_b = jax.vmap(jp.dot, in_axes=[None, 0])(best_axis, normals_b)
+  dist_a = normals_a @ best_axis
+  dist_b = normals_b @ best_axis
   a_max = dist_a.argmax()
   b_max = dist_b.argmax()
   a_min = dist_a.argmin()
   b_min = dist_b.argmin()
 
   ref_face = jp.where(best_sign > 0, faces_a[a_max], faces_b[b_max])
   ref_face_norm = jp.where(best_sign > 0, normals_a[a_max], normals_b[b_max])
@@ -492,180 +718,159 @@
       dist,
   )
   pos = jp.where(is_edge_contact, jp.tile(pos[idx], (4, 1)), pos)
 
   return dist, pos, normal
 
 
-def plane_convex(plane: GeomInfo, convex: GeomInfo) -> Contact:
-  """Calculates contacts between a plane and a convex object."""
-  vert = convex.vert
-
-  # get points in the convex frame
-  plane_pos = convex.mat.T @ (plane.pos - convex.pos)
-  n = convex.mat.T @ plane.mat[:, 2]
-  support = (plane_pos - vert) @ n
-  idx = _manifold_points(vert, support > 0, n)
-  pos = vert[idx]
+def _arcs_intersect(
+    a: jax.Array, b: jax.Array, c: jax.Array, d: jax.Array
+) -> jax.Array:
+  """Tests if arcs AB and CD on the unit sphere intersect."""
+  ba, dc = jp.cross(b, a), jp.cross(d, c)
+  cba, dba = jp.dot(c, ba), jp.dot(d, ba)
+  adc, bdc = jp.dot(a, dc), jp.dot(b, dc)
+  return (cba * dba < 0) & (adc * bdc < 0) & (cba * bdc > 0)
 
-  # convert to world frame
-  pos = convex.pos + pos @ convex.mat.T
-  n = plane.mat[:, 2]
 
-  frame = jp.stack([math.make_frame(n)] * 4, axis=0)
-  unique = jp.tril(idx == idx[:, None]).sum(axis=1) == 1
-  dist = jp.where(unique, -support[idx], 1)
-  pos = pos - 0.5 * dist[:, None] * n
-  return dist, pos, frame
+def _sat_gaussmap(
+    centroid_a: jax.Array,
+    faces_a: jax.Array,
+    faces_b: jax.Array,
+    vertices_a: jax.Array,
+    vertices_b: jax.Array,
+    normals_a: jax.Array,
+    normals_b: jax.Array,
+    edges_a: jax.Array,
+    edges_b: jax.Array,
+    edge_face_normals_a: jax.Array,
+    edge_face_normals_b: jax.Array,
+) -> Tuple[jax.Array, jax.Array, jax.Array]:
+  """Runs the Separating Axis Test for a pair of hulls.
 
+  Runs the separating axis test for all faces. Tests edge separating axes via
+  edge intersections on gauss maps for all edge pairs. h/t to Dirk Gregorius
+  for the implementation details and gauss map trick.
 
-def sphere_convex(sphere: GeomInfo, convex: GeomInfo) -> Contact:
-  """Calculates contact between a sphere and a convex object."""
-  faces = convex.face
-  normals = convex.facenorm
+  Args:
+    centroid_a: Centroid of hull A.
+    faces_a: Faces for hull A.
+    faces_b: Faces for hull B.
+    vertices_a: Vertices for hull A.
+    vertices_b: Vertices for hull B.
+    normals_a: Normal vectors for hull A faces.
+    normals_b: Normal vectors for hull B faces.
+    edges_a: Edges for hull A.
+    edges_b: Edges for hull B.
+    edge_face_normals_a: Face normals for edges in hull A.
+    edge_face_normals_b: Face normals for edges in hull B.
 
-  # Put sphere in convex frame.
-  sphere_pos = convex.mat.T @ (sphere.pos - convex.pos)
+  Returns:
+    tuple of dist, pos, and normal
+  """
+  # Handle face separating axes.
+  axes = jp.concatenate([normals_a, -normals_b])
 
-  # Get support from face normals.
   @jax.vmap
-  def get_support(faces, normal):
-    pos = sphere_pos - normal * sphere.size[0]
-    return jp.dot(pos - faces[0], normal)
+  def get_support(axis):
+    # the matmul here is more performant with vmap(dot)
+    dot = functools.partial(jp.dot, precision=jax.lax.Precision.HIGH)
+    support_a = jax.vmap(dot, in_axes=[None, 0])(axis, vertices_a)
+    support_b = jax.vmap(dot, in_axes=[None, 0])(axis, vertices_b)
+    dist = support_a.max() - support_b.min()
+    separating = dist < 0
+    dist = jp.where(dist < 0, 1e6, dist)
+    return dist, separating
 
-  support = get_support(faces, normals)
+  support, separating = get_support(axes)
+  is_face_separating = separating.any()
 
-  # Pick the face with minimal penetration as long as it has support.
-  support = jp.where(support >= 0, -1e12, support)
-  best_idx = support.argmax()
-  face = faces[best_idx]
-  normal = normals[best_idx]
+  # choose the best separating axis
+  best_idx = jp.argmin(support)
+  best_axis = axes[best_idx]
 
-  # Get closest point between the polygon face and the sphere center point.
-  # Project the sphere center point onto poly plane. If it's inside polygon
-  # edge normals, then we're done.
-  pt = _project_pt_onto_plane(sphere_pos, face[0], normal)
-  edge_p0 = jp.roll(face, 1, axis=0)
-  edge_p1 = face
-  edge_normals = jax.vmap(jp.cross, in_axes=[0, None])(
-      edge_p1 - edge_p0,
-      normal,
+  # get the (reference) face most aligned with the separating axis
+  dist_a = normals_a @ best_axis
+  dist_b = normals_b @ -best_axis
+  face_a_idx = dist_a.argmax()
+  face_b_idx = dist_b.argmax()
+
+  cond = best_idx < normals_a.shape[0]
+  ref_face = jp.where(cond, faces_a[face_a_idx], faces_b[face_b_idx])
+  incident_face = jp.where(cond, faces_b[face_b_idx], faces_a[face_a_idx])
+  ref_face_norm = jp.where(cond, normals_a[face_a_idx], normals_b[face_b_idx])
+  incident_face_norm = jp.where(
+      cond, normals_b[face_b_idx], normals_a[face_a_idx]
   )
-  edge_dist = jax.vmap(
-      lambda plane_pt, plane_norm: (pt - plane_pt).dot(plane_norm)
-  )(edge_p0, edge_normals)
-  inside = jp.all(edge_dist <= 0)  # lte to handle degenerate edges
-
-  # If the point is outside edge normals, project onto the closest edge plane
-  # that the point is in front of.
-  degenerate_edge = jp.all(edge_normals == 0, axis=1)
-  behind = edge_dist < 0.0
-  edge_dist = jp.where(degenerate_edge | behind, 1e12, edge_dist)
-  idx = edge_dist.argmin()
-  edge_pt = math.closest_segment_point(edge_p0[idx], edge_p1[idx], pt)
-
-  pt = jp.where(inside, pt, edge_pt)
-
-  # Get the normal, dist, and contact position.
-  n, d = math.normalize_with_norm(pt - sphere_pos)
-  spt = sphere_pos + n * sphere.size[0]
-  dist = d - sphere.size[0]
-  pos = (pt + spt) * 0.5
 
-  # Go back to world frame.
-  n = convex.mat @ n
-  pos = convex.mat @ pos + convex.pos
-
-  return jax.tree_map(
-      lambda x: jp.expand_dims(x, axis=0), (dist, pos, math.make_frame(n))
+  dist, pos, normal = _create_contact_manifold(
+      ref_face,
+      incident_face,
+      ref_face_norm,
+      incident_face_norm,
+      -best_axis,
   )
 
-
-def capsule_convex(cap: GeomInfo, convex: GeomInfo) -> Contact:
-  """Calculates contacts between a capsule and a convex object."""
-  # Get convex transformed normals, faces, and vertices.
-  faces = convex.face
-  normals = convex.facenorm
-
-  # Put capsule in convex frame.
-  cap_pos = convex.mat.T @ (cap.pos - convex.pos)
-  axis, length = cap.mat[:, 2], cap.size[1]
-  axis = convex.mat.T @ axis
-  seg = axis * length
-  cap_pts = jp.array([
-      cap_pos - seg,
-      cap_pos + seg,
-  ])
-
-  # Get support from face normals.
-  @jax.vmap
-  def get_support(face, normal):
-    pts = cap_pts - normal * cap.size[0]
-    sup = jax.vmap(lambda x: jp.dot(x - face[0], normal))(pts)
-    return sup.min()
-
-  support = get_support(faces, normals)
-  has_support = jp.all(support < 0)
-
-  # Pick the face with minimal penetration as long as it has support.
-  support = jp.where(support >= 0, -1e12, support)
-  best_idx = support.argmax()
-  face = faces[best_idx]
-  normal = normals[best_idx]
-
-  # Clip the edge against side planes and create two contact points against the
-  # face.
-  edge_p0 = jp.roll(face, 1, axis=0)
-  edge_p1 = face
-  edge_normals = jax.vmap(jp.cross, in_axes=[0, None])(
-      edge_p1 - edge_p0,
-      normal,
-  )
-  cap_pts_clipped, mask = _clip_edge_to_planes(
-      cap_pts[0], cap_pts[1], edge_p0, edge_normals
-  )
-  cap_pts_clipped = cap_pts_clipped - normal * cap.size[0]
-  face_pts = jax.vmap(_project_pt_onto_plane, in_axes=[0, None, None])(
-      cap_pts_clipped, face[0], normal
+  # Handle edge separating axes by checking all edge pairs.
+  a_idx = jp.tile(jp.arange(edges_a.shape[0]), reps=edges_b.shape[0])
+  b_idx = jp.repeat(
+      jp.arange(edges_b.shape[0]), repeats=edges_a.shape[0], axis=0
+  )
+  normal_a_1 = edge_face_normals_a[a_idx, 0]
+  normal_a_2 = edge_face_normals_a[a_idx, 1]
+  normal_b_1 = edge_face_normals_b[b_idx, 0]
+  normal_b_2 = edge_face_normals_b[b_idx, 1]
+  is_minkowski_face = jax.vmap(_arcs_intersect)(
+      normal_a_1, normal_a_2, -normal_b_1, -normal_b_2
+  )
+
+  # get distances
+  edge_a_dir = jax.vmap(math.normalize)(edges_a[:, 0] - edges_a[:, 1])[a_idx]
+  edge_b_dir = jax.vmap(math.normalize)(edges_b[:, 0] - edges_b[:, 1])[b_idx]
+  edges_a, edges_b = edges_a[a_idx], edges_b[b_idx]
+  edge_a_pt, edge_a_pt_2 = edges_a[:, 0], edges_a[:, 1]
+  edge_b_pt, edge_b_pt_2 = edges_b[:, 0], edges_b[:, 1]
+
+  def get_normals(a_dir, a_pt, b_dir):
+    edge_axis = jp.cross(a_dir, b_dir)
+    degenerate_edge_axis = jp.sum(edge_axis**2) < 1e-6
+    edge_axis = math.normalize(edge_axis)
+    # correct normal to point from a to b, object b is at the origin
+    sign = jp.where(jp.dot(edge_axis, a_pt - centroid_a) > 0.0, 1.0, -1.0)
+    return edge_axis * sign, degenerate_edge_axis
+
+  edge_axes, degenerate_edge_axes = jax.vmap(get_normals)(
+      edge_a_dir, edge_a_pt, edge_b_dir)
+  edge_dist = jax.vmap(jp.dot)(edge_axes, edge_b_pt - edge_a_pt)
+  # handle degenerate axis
+  edge_dist = jp.where(degenerate_edge_axes, -jp.inf, edge_dist)
+  # ensure edges create minkowski face
+  edge_dist = jp.where(is_minkowski_face, edge_dist, -jp.inf)
+
+  best_edge_idx = edge_dist.argmax()
+  best_edge_dist = edge_dist[best_edge_idx]
+  is_edge_contact = jp.where(
+      dist.max() < 0, best_edge_dist > dist.max() - 1e-6,
+      (best_edge_dist < 0) & ~jp.isinf(best_edge_dist)
   )
-  # Create variables for the face contact.
-  pos = (cap_pts_clipped + face_pts) * 0.5
-  norm = jp.stack([normal] * 2, 0)
-  penetration = jp.where(
-      mask & has_support, jp.dot(face_pts - cap_pts_clipped, normal), -1
+  is_edge_contact = is_edge_contact & ~is_face_separating
+  normal = jp.where(is_edge_contact, edge_axes[best_edge_idx], normal)
+  dist = jp.where(
+      is_edge_contact,
+      jp.array([best_edge_dist, 1, 1, 1]),
+      dist,
   )
+  a_closest, b_closest = math.closest_segment_to_segment_points(
+      edge_a_pt[best_edge_idx], edge_a_pt_2[best_edge_idx],
+      edge_b_pt[best_edge_idx], edge_b_pt_2[best_edge_idx])
+  pos = jp.where(
+      is_edge_contact,
+      jp.tile(0.5 * (a_closest + b_closest), (4, 1)), pos)
 
-  # Get a potential edge contact.
-  edge_closest, cap_closest = jax.vmap(
-      math.closest_segment_to_segment_points, in_axes=[0, 0, None, None]
-  )(edge_p0, edge_p1, cap_pts[0], cap_pts[1])
-  e_idx = ((edge_closest - cap_closest) ** 2).sum(axis=1).argmin()
-  cap_closest_pt, edge_closest_pt = cap_closest[e_idx], edge_closest[e_idx]
-  edge_axis = cap_closest_pt - edge_closest_pt
-  edge_axis, edge_dist = math.normalize_with_norm(edge_axis)
-  edge_pos = (
-      edge_closest_pt + (cap_closest_pt - edge_axis * cap.size[0])
-  ) * 0.5
-  edge_norm = edge_axis
-  edge_penetration = cap.size[0] - edge_dist
-  has_edge_contact = edge_penetration > 0
-
-  # Get the contact info.
-  pos = jp.where(has_edge_contact, pos.at[0].set(edge_pos), pos)
-  n = -jp.where(has_edge_contact, norm.at[0].set(edge_norm), norm)
-
-  # Go back to world frame.
-  pos = convex.pos + pos @ convex.mat.T
-  n = n @ convex.mat.T
-
-  dist = -jp.where(
-      has_edge_contact, penetration.at[0].set(edge_penetration), penetration
-  )
-  frame = jax.vmap(math.make_frame)(n)
-  return dist, pos, frame
+  return dist, pos, normal
 
 
 def convex_convex(c1: GeomInfo, c2: GeomInfo) -> Contact:
   """Calculates contacts between two convex objects."""
   if c1.face is None or c2.face is None or c1.vert is None or c2.vert is None:
     raise AssertionError('Mesh info missing.')
   # pad face vertices so that we can broadcast between geom1 and geom2
@@ -695,24 +900,49 @@
 
   vertices1 = to_local_pos + c1.vert @ to_local_mat.T
   vertices2 = c2.vert
 
   unique_edges1 = jp.take(vertices1, c1.edge, axis=0)
   unique_edges2 = jp.take(vertices2, c2.edge, axis=0)
 
-  dist, pos, normal = _sat_hull_hull(
-      faces1,
-      faces2,
-      vertices1,
-      vertices2,
-      normals1,
-      normals2,
-      unique_edges1,
-      unique_edges2,
-  )
+  edges1 = jp.take(vertices1, c1.edge, axis=0)
+  edges2 = jp.take(vertices2, c2.edge, axis=0)
+
+  edge_face_normals1 = c1.edge_face_normal @ to_local_mat.T
+  edge_face_normals2 = c2.edge_face_normal
+
+  enable_bruteforce = (
+      unique_edges1.shape[0] * unique_edges2.shape[0]
+      < edges1[0].shape[0] * edges2[0].shape[0]
+  )
+  if enable_bruteforce:
+    dist, pos, normal = _sat_bruteforce(
+        faces1,
+        faces2,
+        vertices1,
+        vertices2,
+        normals1,
+        normals2,
+        unique_edges1,
+        unique_edges2,
+    )
+  else:
+    dist, pos, normal = _sat_gaussmap(
+        to_local_pos,
+        faces1,
+        faces2,
+        vertices1,
+        vertices2,
+        normals1,
+        normals2,
+        edges1,
+        edges2,
+        edge_face_normals1,
+        edge_face_normals2,
+    )
 
   # Go back to world frame.
   pos = c2.pos + pos @ c2.mat.T
   normal = normal @ c2.mat.T
   normal = -normal if swapped else normal
 
   frame = jax.vmap(math.make_frame)(normal)
```

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/collision_driver.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,57 +10,62 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Collide geometries."""
 
-from typing import Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
 
 import jax
 from jax import numpy as jp
 import mujoco
 from mujoco.mjx._src import collision_base
+from mujoco.mjx._src import mesh
 from mujoco.mjx._src import support
-from mujoco.mjx._src import math
 # pylint: disable=g-importing-member
 from mujoco.mjx._src.collision_base import Candidate
 from mujoco.mjx._src.collision_base import CandidateSet
 from mujoco.mjx._src.collision_base import GeomInfo
 from mujoco.mjx._src.collision_base import SolverParams
 from mujoco.mjx._src.collision_convex import capsule_convex
 from mujoco.mjx._src.collision_convex import convex_convex
 from mujoco.mjx._src.collision_convex import plane_convex
 from mujoco.mjx._src.collision_convex import sphere_convex
 from mujoco.mjx._src.collision_primitive import capsule_capsule
 from mujoco.mjx._src.collision_primitive import plane_capsule
+from mujoco.mjx._src.collision_primitive import plane_ellipsoid
 from mujoco.mjx._src.collision_primitive import plane_sphere
 from mujoco.mjx._src.collision_primitive import sphere_capsule
 from mujoco.mjx._src.collision_primitive import sphere_sphere
+from mujoco.mjx._src.collision_sdf import capsule_ellipsoid
+from mujoco.mjx._src.collision_sdf import ellipsoid_ellipsoid
 from mujoco.mjx._src.types import Contact
 from mujoco.mjx._src.types import Data
 from mujoco.mjx._src.types import DisableBit
 from mujoco.mjx._src.types import GeomType
 from mujoco.mjx._src.types import Model
 # pylint: enable=g-importing-member
 
-
 # pair-wise collision functions
 _COLLISION_FUNC = {
     (GeomType.PLANE, GeomType.SPHERE): plane_sphere,
     (GeomType.PLANE, GeomType.CAPSULE): plane_capsule,
     (GeomType.PLANE, GeomType.BOX): plane_convex,
+    (GeomType.PLANE, GeomType.ELLIPSOID): plane_ellipsoid,
     (GeomType.PLANE, GeomType.MESH): plane_convex,
     (GeomType.SPHERE, GeomType.SPHERE): sphere_sphere,
     (GeomType.SPHERE, GeomType.CAPSULE): sphere_capsule,
     (GeomType.SPHERE, GeomType.BOX): sphere_convex,
     (GeomType.SPHERE, GeomType.MESH): sphere_convex,
     (GeomType.CAPSULE, GeomType.CAPSULE): capsule_capsule,
     (GeomType.CAPSULE, GeomType.BOX): capsule_convex,
+    (GeomType.CAPSULE, GeomType.ELLIPSOID): capsule_ellipsoid,
     (GeomType.CAPSULE, GeomType.MESH): capsule_convex,
+    (GeomType.ELLIPSOID, GeomType.ELLIPSOID): ellipsoid_ellipsoid,
     (GeomType.BOX, GeomType.BOX): convex_convex,
     (GeomType.BOX, GeomType.MESH): convex_convex,
     (GeomType.MESH, GeomType.MESH): convex_convex,
 }
 
 
 def get_collision_fn(
@@ -87,15 +92,26 @@
     return
   if t1 == GeomType.PLANE and t2 == GeomType.HFIELD:
     return
 
   def mesh_key(i):
     convex_data = [[None] * m.ngeom] * 3
     if isinstance(m, Model):
-      convex_data = [m.geom_convex_face, m.geom_convex_vert, m.geom_convex_edge]
+      convex_data = [
+          m.geom_convex_face,
+          m.geom_convex_vert,
+          m.geom_convex_edge_dir,
+      ]
+    elif isinstance(m, mujoco.MjModel):
+      kwargs = mesh.get(m)
+      convex_data = [
+          kwargs['geom_convex_face'],
+          kwargs['geom_convex_vert'],
+          kwargs['geom_convex_edge_dir'],
+      ]
     key = tuple((-1,) if v[i] is None else v[i].shape for v in convex_data)
     return key
 
   k1, k2 = mesh_key(g1), mesh_key(g2)
 
   candidates = {(c.geom1, c.geom2) for c in result.get((t1, t2, k1, k2), [])}
   if (g1, g2) in candidates:
@@ -173,48 +189,76 @@
   solimp = mix_fn(m.geom_solimp[g1], m.geom_solimp[g2], mix)
   margin = jp.maximum(m.geom_margin[g1], m.geom_margin[g2])
   gap = jp.maximum(m.geom_gap[g1], m.geom_gap[g2])
 
   return SolverParams(friction, solref, solreffriction, solimp, margin, gap)
 
 
+def get_params(
+    m: Union[Model, mujoco.MjModel], candidates: Sequence[Candidate]
+) -> Tuple[List[int], List[int], SolverParams]:
+  """Gets solver params for a list of collision candidates."""
+  # group sol params by different candidate types
+  typ_cands = {}
+  for c in candidates:
+    typ = (c.ipair > -1, c.geomp > -1)
+    typ_cands.setdefault(typ, []).append(c)
+
+  geom1, geom2, params = [], [], []
+  for (pair, priority), candidates in typ_cands.items():
+    geom1.extend([c.geom1 for c in candidates])
+    geom2.extend([c.geom2 for c in candidates])
+    if pair:
+      params.append(_pair_params(m, candidates))
+    elif priority:
+      params.append(_priority_params(m, candidates))
+    else:
+      params.append(_dynamic_params(m, candidates))
+
+  params = jax.tree_map(lambda *x: jp.concatenate(x), *params)
+  return geom1, geom2, params
+
+
 def _pair_info(
     m: Model, d: Data, geom1: Sequence[int], geom2: Sequence[int]
 ) -> Tuple[GeomInfo, GeomInfo, Sequence[Dict[str, Optional[int]]]]:
   """Returns geom pair info for calculating collision."""
-  g1, g2 = jp.array(geom1), jp.array(geom2)
-  info1 = GeomInfo(
-      g1,
-      d.geom_xpos[g1],
-      d.geom_xmat[g1],
-      m.geom_size[g1],
-  )
-  info2 = GeomInfo(
-      g2,
-      d.geom_xpos[g2],
-      d.geom_xmat[g2],
-      m.geom_size[g2],
-  )
-  in_axes1 = in_axes2 = jax.tree_map(lambda x: 0, info1)
-  if m.geom_convex_face[geom1[0]] is not None:
-    info1 = info1.replace(
-        face=jp.stack([m.geom_convex_face[i] for i in geom1]),
-        vert=jp.stack([m.geom_convex_vert[i] for i in geom1]),
-        edge=jp.stack([m.geom_convex_edge[i] for i in geom1]),
-        facenorm=jp.stack([m.geom_convex_facenormal[i] for i in geom1]),
-    )
-    in_axes1 = in_axes1.replace(face=0, vert=0, edge=0, facenorm=0)
-  if m.geom_convex_face[geom2[0]] is not None:
-    info2 = info2.replace(
-        face=jp.stack([m.geom_convex_face[i] for i in geom2]),
-        vert=jp.stack([m.geom_convex_vert[i] for i in geom2]),
-        edge=jp.stack([m.geom_convex_edge[i] for i in geom2]),
-        facenorm=jp.stack([m.geom_convex_facenormal[i] for i in geom2]),
+  def mesh_info(geom):
+    g = jp.array(geom)
+    info = GeomInfo(
+        g,
+        d.geom_xpos[g],
+        d.geom_xmat[g],
+        m.geom_size[g],
     )
-    in_axes2 = in_axes2.replace(face=0, vert=0, edge=0, facenorm=0)
+    in_axes = jax.tree_map(lambda x: 0, info)
+    is_mesh = m.geom_convex_face[geom[0]] is not None
+    if is_mesh:
+      info = info.replace(
+          face=jp.stack([m.geom_convex_face[i] for i in geom]),
+          vert=jp.stack([m.geom_convex_vert[i] for i in geom]),
+          edge_dir=jp.stack([m.geom_convex_edge_dir[i] for i in geom]),
+          facenorm=jp.stack([m.geom_convex_facenormal[i] for i in geom]),
+          edge=jp.stack([m.geom_convex_edge[i] for i in geom]),
+          edge_face_normal=jp.stack(
+              [m.geom_convex_edge_face_normal[i] for i in geom]
+          ),
+      )
+      in_axes = in_axes.replace(
+          face=0,
+          vert=0,
+          edge_dir=0,
+          facenorm=0,
+          edge=0,
+          edge_face_normal=0,
+      )
+    return info, in_axes
+
+  info1, in_axes1 = mesh_info(geom1)
+  info2, in_axes2 = mesh_info(geom2)
   return info1, info2, [in_axes1, in_axes2]
 
 
 def _body_pair_filter(
     m: Union[Model, mujoco.MjModel], b1: int, b2: int
 ) -> bool:
   """Filters body pairs for collision."""
@@ -259,43 +303,25 @@
     candidates: Sequence[Candidate],
 ) -> Contact:
   """Collides a geom pair."""
   fn = get_collision_fn(geom_types)
   if not fn:
     return Contact.zero()
 
-  # group sol params by different candidate types
-  typ_cands = {}
-  for c in candidates:
-    typ = (c.ipair > -1, c.geomp > -1)
-    typ_cands.setdefault(typ, []).append(c)
-
-  geom1, geom2, params = [], [], []
-  for (pair, priority), candidates in typ_cands.items():
-    geom1.extend([c.geom1 for c in candidates])
-    geom2.extend([c.geom2 for c in candidates])
-    if pair:
-      params.append(_pair_params(m, candidates))
-    elif priority:
-      params.append(_priority_params(m, candidates))
-    else:
-      params.append(_dynamic_params(m, candidates))
-
-  params = jax.tree_map(lambda *x: jp.concatenate(x), *params)
+  geom1, geom2, params = get_params(m, candidates)
   g1, g2, in_axes = _pair_info(m, d, geom1, geom2)
 
   # Run a crude version of broadphase.
   max_pairs = int(support.get_custom_numeric(m, 'max_geom_pairs'))
   run_broadphase = _broadphase_enabled(geom_types, len(geom1), max_pairs)
   n_pairs = max_pairs if run_broadphase else len(geom1)
   if run_broadphase:
     # broadphase over geom pairs, using bounding spheres
-    size1 = jp.max(m.geom_size[jp.array(geom1)], axis=-1)
-    size2 = jp.max(m.geom_size[jp.array(geom2)], axis=-1)
-    # TODO(btaba): consider re-using collision info for (sphere, sphere)
+    size1 = jp.max(m.geom_size[g1.geom_id], axis=-1)
+    size2 = jp.max(m.geom_size[g2.geom_id], axis=-1)
     dists = jax.vmap(jp.linalg.norm)(g2.pos - g1.pos) - (size1 + size2)
     _, idx = jax.lax.top_k(-dists, k=n_pairs)
     g1, g2, params = jax.tree_map(
         lambda x, idx=idx: x[idx, ...], (g1, g2, params)
     )
 
   # call contact function
```

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/collision_driver_test.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_driver_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -128,19 +128,145 @@
           <joint axis="1 0 0" type="free"/>
           <geom size="0.5 0.5 0.5" type="box"/>
         </body>
       </worldbody>
     </mujoco>
   """
 
-  def test_sphere_convex(self):
+  def test_sphere_convex_face(self):
+    # no contact
+    xml = self._SPHERE_CONVEX.replace(
+        '<body pos="0.52 0 0.52">', '<body pos="0.55 0 0.5">'
+    )
+    d, dx = _collide(xml)
+    self.assertEmpty(d.contact.dist)
+    self.assertGreater(dx.contact.dist, 0)
+
+    # face contact
+    xml = self._SPHERE_CONVEX.replace(
+        '<body pos="0.52 0 0.52">', '<body pos="0.51 0 0.25">'
+    )
+    d, dx = _collide(xml)
+    for field in dataclasses.fields(Contact):
+      _assert_attr_eq(dx.contact, d.contact, field.name, 'face', 1e-4)
+
+    # deep face contact
+    xml = self._SPHERE_CONVEX.replace(
+        '<body pos="0.52 0 0.52">', '<body pos="0.48 0 0.47">'
+    )
+    d, dx = _collide(xml)
+    self.assertTrue((dx.contact.dist < 0).all())
+    self.assertTrue((d.contact.dist < 0).all())
+    np.testing.assert_allclose(dx.contact.dist, [-0.07], atol=1e-5)
+    np.testing.assert_array_almost_equal(dx.contact.pos, d.contact.pos)
+    np.testing.assert_array_almost_equal(
+        dx.contact.frame, d.contact.frame.reshape((-1, 3, 3))
+    )
+
+  def test_sphere_convex_edge(self):
+    # edge contact
     d, dx = _collide(self._SPHERE_CONVEX)
+    for field in dataclasses.fields(Contact):
+      _assert_attr_eq(dx.contact, d.contact, field.name, 'edge', 1e-4)
 
+    # deep edge penetration
+    xml = self._SPHERE_CONVEX.replace(
+        '<body pos="0.52 0 0.52">', '<body pos="0.49 0 0.49">'
+    )
+    d, dx = _collide(xml)
+    self.assertTrue((dx.contact.dist < 0).all())
+    self.assertTrue((d.contact.dist < 0).all())
+    np.testing.assert_allclose(dx.contact.dist, [-0.06], atol=1e-5)
+    np.testing.assert_array_almost_equal(dx.contact.pos, d.contact.pos)
+    np.testing.assert_array_almost_equal(
+        dx.contact.frame, d.contact.frame.reshape((-1, 3, 3))
+    )
+
+    # vertex contact
+    xml = self._SPHERE_CONVEX.replace(
+        '<body pos="0.52 0 0.52">', '<body pos="0.5 0.52 0.51">'
+    )
+    d, dx = _collide(xml)
     for field in dataclasses.fields(Contact):
-      _assert_attr_eq(dx.contact, d.contact, field.name, 'sphere_convex', 1e-4)
+      _assert_attr_eq(dx.contact, d.contact, field.name, 'vertex', 1e-4)
+
+    # sphere center on vertex
+    xml = self._SPHERE_CONVEX.replace(
+        '<body pos="0.52 0 0.52">', '<body pos="0.5 0 0.5">'
+    )
+    d, dx = _collide(xml)
+    for field in dataclasses.fields(Contact):
+      _assert_attr_eq(dx.contact, d.contact, field.name, 'vertex_center', 1e-4)
+
+
+class EllipsoidCollisionTest(parameterized.TestCase):
+
+  _ELLIPSOID_PLANE = """
+    <mujoco>
+      <worldbody>
+        <geom name="floor" size="0 0 .05" type="plane"/>
+        <body pos="0 0 0.03" euler="45 0 0">
+          <freejoint/>
+          <geom size=".15 .03 .05" type="ellipsoid"/>
+        </body>
+      </worldbody>
+    </mujoco>
+  """
+
+  def test_plane_ellipsoid(self):
+    """Tests ellipsoid plane contact."""
+    d, dx = _collide(self._ELLIPSOID_PLANE)
+    self.assertLess(dx.contact.dist[0], 0)
+    for field in dataclasses.fields(Contact):
+      _assert_attr_eq(
+          dx.contact, d.contact, field.name, 'ellipsoid-plane', 1e-5)
+
+  _ELLIPSOID_ELLIPSOID = """
+    <mujoco>
+      <worldbody>
+        <body>
+          <geom size=".15 .03 .05" type="ellipsoid"/>
+        </body>
+        <body pos="0 0 0.09">
+          <freejoint/>
+          <geom size=".15 .03 .05" type="ellipsoid"/>
+        </body>
+      </worldbody>
+    </mujoco>
+  """
+
+  def test_ellipsoid_ellipsoid(self):
+    """Tests ellipsoid ellipsoid contact."""
+    d, dx = _collide(self._ELLIPSOID_ELLIPSOID)
+    self.assertLess(dx.contact.dist[0], 0)
+    for field in dataclasses.fields(Contact):
+      _assert_attr_eq(
+          dx.contact, d.contact, field.name, 'ellipsoid-ellipsoid', 1e-5)
+
+  _ELLIPSOID_CAPSULE = """
+    <mujoco>
+      <worldbody>
+        <body>
+          <geom size=".15 .03 .05" type="ellipsoid"/>
+        </body>
+        <body pos="0 0 0.0999">
+          <freejoint/>
+          <geom size=".05" fromto="-.1 0 0 .1 0 0" type="capsule"/>
+        </body>
+      </worldbody>
+    </mujoco>
+  """
+
+  def test_capsule_ellipsoid(self):
+    """Tests ellipsoid capsule contact."""
+    d, dx = _collide(self._ELLIPSOID_CAPSULE)
+    self.assertLess(dx.contact.dist[0], 0)
+    for field in dataclasses.fields(Contact):
+      _assert_attr_eq(
+          dx.contact, d.contact, field.name, 'ellipsoid-capsule', 1e-4)
 
 
 class CapsuleCollisionTest(parameterized.TestCase):
   _CAP_PLANE = """
     <mujoco>
       <worldbody>
         <geom size="40 40 40" type="plane"/>
@@ -208,31 +334,55 @@
     )
 
   _CAP_BOX = """
     <mujoco>
       <worldbody>
         <body pos="0 0 0.54">
           <joint axis="1 0 0" type="free"/>
-          <geom fromto="-0.4 0 0 0.4 0 0" size="0.05" type="capsule"/>
+          <geom fromto="-0.4 0 0 1.0 0 0" size="0.05" type="capsule"/>
         </body>
         <body>
           <joint axis="1 0 0" type="free"/>
           <geom size="0.5 0.5 0.5" type="box"/>
         </body>
       </worldbody>
     </mujoco>
   """
 
-  def test_capsule_convex(self):
-    """Tests a capsule-convex collision for a face contact."""
+  def test_capsule_convex_face(self):
+    """Tests face contact."""
     d, dx = _collide(self._CAP_BOX)
 
+    # sort positions for comparison
+    idx = np.lexsort((dx.contact.pos[:, 0], dx.contact.pos[:, 1]))
+    dx = dx.tree_replace({'contact.pos': dx.contact.pos[idx]})
+    idx = np.lexsort((d.contact.pos[:, 0], d.contact.pos[:, 1]))
+    d.contact.pos[:] = d.contact.pos[idx]
+    d.contact.frame[:] = d.contact.frame[idx]
+    d.contact.dist[:] = d.contact.dist[idx]
+
     for field in dataclasses.fields(Contact):
       _assert_attr_eq(dx.contact, d.contact, field.name, 'capsule_convex', 1e-4)
 
+  def test_capsule_convex_face_deep(self):
+    """Tests deep face penetration."""
+    xml = self._CAP_BOX.replace('<body pos="0 0 0.54">', '<body pos="0 0 0.4">')
+
+    _, dx = _collide(xml)
+    self.assertTrue((dx.contact.dist < 0).all())
+    np.testing.assert_array_almost_equal(
+        dx.contact.pos, np.array([[0.5, 0, 0.425], [-0.4, 0, 0.425]])
+    )
+    np.testing.assert_array_almost_equal(
+        dx.contact.dist, np.array([-0.15, -0.15])
+    )
+    np.testing.assert_array_almost_equal(
+        dx.contact.frame[:, 0], np.array([[0, 0, -1]] * 2)
+    )
+
   _CAP_EDGE_BOX = """
     <mujoco>
       <worldbody>
         <body pos="0.5 0 0.55" euler="0 30 0">
           <joint axis="1 0 0" type="free"/>
           <geom fromto="-0.6 0 0 0.6 0 0" size="0.05" type="capsule"/>
         </body>
@@ -241,25 +391,83 @@
           <geom size="0.5 0.5 0.5" type="box"/>
         </body>
       </worldbody>
     </mujoco>
   """
 
   def test_capsule_convex_edge(self):
-    """Tests a capsule-convex collision for an edge contact."""
+    """Tests edge contact."""
     d, dx = _collide(self._CAP_EDGE_BOX)
 
     c = dx.contact
     self.assertEqual(c.pos.shape[0], 2)
     self.assertGreater(c.dist[1], 0)
     # extract the contact point with penetration
     c = jax.tree_map(lambda x: jp.take(x, 0, axis=0)[None], dx.contact)
     for field in dataclasses.fields(Contact):
       _assert_attr_eq(c, d.contact, field.name, 'capsule_convex_edge', 1e-4)
 
+  def test_capsule_convex_edge_deep(self):
+    """Tests deep edge penetration."""
+    xml = self._CAP_EDGE_BOX.replace(
+        '<body pos="0.5 0 0.55"', '<body pos="0.5 0 0.42"'
+    )
+    _, dx = _collide(xml)
+
+    np.testing.assert_array_equal(dx.contact.dist < 0, np.array([True, False]))
+    np.testing.assert_array_almost_equal(dx.contact.dist[0], np.array([-0.13]))
+    np.testing.assert_array_almost_equal(
+        dx.contact.pos[0], np.array([0.5, 0, 0.435]), decimal=3
+    )
+    np.testing.assert_array_almost_equal(
+        dx.contact.frame[0, 0], np.array([0, 0, -1]), decimal=3
+    )
+
+  def test_capsule_convex_edge_shallow_tip(self):
+    """Tests shallow edge penetration on the tip of the capsule."""
+    # the capsule sphere is inside the edge voronoi region, so there is an
+    # edge contact
+    xml = self._CAP_EDGE_BOX.replace(
+        '<geom fromto="-0.6 0 0 0.6 0 0" size="0.05"',
+        '<geom fromto="0.6 0 0.6 -0.05 0 0" size="0.1"',
+    )
+    xml = xml.replace('<body pos="0.5 0 0.55"', '<body pos="0.58 0 0.55"')
+    d, dx = _collide(xml)
+
+    c = dx.contact
+    self.assertEqual(c.pos.shape[0], 2)
+    self.assertGreater(c.dist[1], 0)
+    # extract the contact point with penetration
+    c = jax.tree_map(lambda x: jp.take(x, 0, axis=0)[None], dx.contact)
+    for field in dataclasses.fields(Contact):
+      _assert_attr_eq(c, d.contact, field.name, 'edge_shallow_tip1', 1e-4)
+    np.testing.assert_array_almost_equal(
+        dx.contact.frame[0][0, :3], np.array([-0.43952, 0.0, -0.898233])
+    )
+
+    # the capsule sphere is outside the edge voronoi region, so there is a
+    # face contact
+    xml = self._CAP_EDGE_BOX.replace(
+        '<geom fromto="-0.6 0 0 0.6 0 0" size="0.05"',
+        '<geom fromto="-0.6 0 0.6 -0.05 0 0" size="0.1"',
+    )
+    xml = xml.replace('<body pos="0.5 0 0.55"', '<body pos="0.5 0 0.52"')
+    d, dx = _collide(xml)
+
+    c = dx.contact
+    self.assertEqual(c.pos.shape[0], 2)
+    self.assertGreater(c.dist[1], 0)
+    # extract the contact point with penetration
+    c = jax.tree_map(lambda x: jp.take(x, 0, axis=0)[None], dx.contact)
+    for field in dataclasses.fields(Contact):
+      _assert_attr_eq(c, d.contact, field.name, 'edge_shallow_tip2', 1e-4)
+    np.testing.assert_array_almost_equal(
+        dx.contact.frame[0][0, :3], np.array([0.0, 0.0, -1.0])
+    )
+
 
 class ConvexTest(absltest.TestCase):
   """Tests the convex contact functions."""
 
   _BOX_PLANE = """
     <mujoco>
       <worldbody>
@@ -293,16 +501,15 @@
         </body>
       </worldbody>
     </mujoco>
   """
 
   def test_flat_box_plane(self):
     """Tests box collision with a plane."""
-    with jax.disable_jit():
-      d, dx = _collide(self._FLAT_BOX_PLANE)
+    d, dx = _collide(self._FLAT_BOX_PLANE)
 
     np.testing.assert_array_less(dx.contact.dist, 0)
 
     # sort positions for comparison
     idx = np.lexsort((dx.contact.pos[:, 0], dx.contact.pos[:, 1]))
     dx = dx.tree_replace({'contact.pos': dx.contact.pos[idx]})
     idx = np.lexsort((d.contact.pos[:, 0], d.contact.pos[:, 1]))
@@ -367,49 +574,83 @@
     c = jax.tree_map(lambda x: jp.take(x, 0, axis=0)[None], dx.contact)
     for field in dataclasses.fields(Contact):
       _assert_attr_eq(c, d.contact, field.name, 'box_box_edge', 1e-2)
 
   _CONVEX_CONVEX = """
     <mujoco>
       <asset>
-        <mesh name="tetrahedron" file="meshes/tetrahedron.stl" scale="0.1 0.1 0.1" />
         <mesh name="dodecahedron" file="meshes/dodecahedron.stl" scale="0.01 0.01 0.01" />
       </asset>
       <worldbody>
         <body pos="0.0 2.0 0.096">
           <joint axis="1 0 0" type="free"/>
-          <geom size="0.2 0.2 0.2" type="mesh" mesh="tetrahedron"/>
+          <geom size="0.2 0.2 0.2" type="mesh" mesh="dodecahedron"/>
         </body>
-        <body pos="0.0 2.0 0.289" euler="0.1 -0.1 45">
+        <body pos="0.0 2.0 0.281" euler="0.1 -0.1 45">
           <joint axis="1 0 0" type="free"/>
           <geom size="0.1 0.1 0.1" type="mesh" mesh="dodecahedron"/>
         </body>
       </worldbody>
     </mujoco>
   """
 
   def test_convex_convex(self):
-    """Tests generic convex-convex collision."""
+    """Tests generic convex-convex collision via _sat_gaussmap."""
     directory = epath.resource_path('mujoco.mjx')
     assets = {
-        'meshes/tetrahedron.stl': (
-            directory / 'test_data' / 'meshes/tetrahedron.stl'
-        ).read_bytes(),
         'meshes/dodecahedron.stl': (
             directory / 'test_data' / 'meshes/dodecahedron.stl'
         ).read_bytes(),
     }
     _, dx = _collide(self._CONVEX_CONVEX, assets=assets)
     c = dx.contact
 
     # Only one contact point for an edge contact.
     self.assertLess(c.dist[0], 0)
     np.testing.assert_array_less(0, c.dist[1:])
     np.testing.assert_array_almost_equal(c.frame[0, 0], np.array([0, 0, 1]))
 
+  _CONVEX_CONVEX_THIN = """
+    <mujoco>
+      <asset>
+        <mesh name="poly"
+         vertex="0.3 0 0  0 0.5 0  -0.3 0 0  0 -0.5 0  0 -1 1  0 1 1"
+         face="0 1 5  0 5 4  0 4 3  3 4 2  2 4 5  1 2 5  0 2 1  0 3 2"/>
+      </asset>
+      <worldbody>
+        <body pos="0.0 2.0 0.35" euler="0 0 90">
+          <freejoint/>
+          <geom size="0.2 0.2 0.2" type="mesh" mesh="poly"/>
+        </body>
+        <body pos="0.0 2.0 2.281" euler="180 0 0">
+          <freejoint/>
+          <geom size="0.2 0.2 0.2" type="mesh" mesh="poly"/>
+        </body>
+      </worldbody>
+    </mujoco>
+  """
+
+  def test_convex_convex_edge(self):
+    """Tests convex-convex collisions with edge contact via _sat_gaussmap."""
+    _, dx = _collide(self._CONVEX_CONVEX_THIN)
+    c = dx.contact
+
+    # Only one contact point for an edge contact.
+    self.assertLess(c.dist[0], 0)
+    np.testing.assert_array_less(0, c.dist[1:])
+    np.testing.assert_array_almost_equal(c.frame[0, 0], np.array([0, 0, 1]))
+    np.testing.assert_array_almost_equal(
+        c.pos[0], np.array([0, 2, 1.3155]), decimal=5)
+
+    _, dx = _collide(
+        self._CONVEX_CONVEX_THIN.replace(
+            'pos="0.0 2.0 0.35"', 'pos="0.0 2.0 0"'))
+    c = dx.contact
+    self.assertTrue((c.dist > 0).all())
+
 
 class BodyPairFilterTest(absltest.TestCase):
   """Tests that certain body pairs get filtered."""
 
   _SELF_COLLISION = """
     <mujoco>
       <worldbody>
@@ -488,14 +729,39 @@
 
   def test_disable_contact(self):
     m = test_util.load_test_file('constraints.xml')
     m.opt.disableflags |= DisableBit.CONTACT
     ncon = collision_driver.ncon(m)
     self.assertEqual(ncon, 0)
 
+  def test_ncon_meshes(self):
+    m = test_util.load_test_file('shadow_hand/scene_right.xml')
+
+    ncon = collision_driver.ncon(m)
+    self.assertEqual(ncon, 15)
+
+    mx = mjx.put_model(m)
+    ncon = collision_driver.ncon(mx)
+    self.assertEqual(ncon, 15)
+
+    # get rid of max_contact_points, test only max_geom_pairs
+    for i in range(m.nnumeric):
+      name_ = (
+          m.names[m.name_numericadr[i] :].decode('utf-8').split('\x00', 1)[0]
+      )
+      if name_ == 'max_contact_points':
+        m.numeric_data[m.numeric_adr[i]] = -1
+
+    ncon = collision_driver.ncon(m)
+    self.assertEqual(ncon, 98)
+
+    mx = mjx.put_model(m)
+    ncon = collision_driver.ncon(mx)
+    self.assertEqual(ncon, 98)
+
 
 class TopKContactTest(absltest.TestCase):
   """Tests top-k contacts."""
 
   _CAPSULES = """
     <mujoco>
       <custom>
@@ -561,30 +827,29 @@
         </body>
       </worldbody>
     </mujoco>
   """
 
   def test_max_pair(self):
     """Tests contact culling before the collision functions were dispatched."""
-    with jax.disable_jit():
-      m = mujoco.MjModel.from_xml_string(self._CAPSULES_MAX_PAIR)
-      mx_top_k = mjx.put_model(m)
-      mx_all = mx_top_k.replace(
-          nnumeric=0, name_numericadr=np.array([]), numeric_data=np.array([])
-      )
-      d = mujoco.MjData(m)
-      dx = mjx.put_data(m, d)
+    m = mujoco.MjModel.from_xml_string(self._CAPSULES_MAX_PAIR)
+    mx_top_k = mjx.put_model(m)
+    mx_all = mx_top_k.replace(
+        nnumeric=0, name_numericadr=np.array([]), numeric_data=np.array([])
+    )
+    d = mujoco.MjData(m)
+    dx = mjx.put_data(m, d)
+
+    collision_jit_fn = jax.jit(mjx.collision)
+    kinematics_jit_fn = jax.jit(mjx.kinematics)
+    dx = kinematics_jit_fn(mx_all, dx)
 
-      collision_jit_fn = jax.jit(mjx.collision)
-      kinematics_jit_fn = jax.jit(mjx.kinematics)
-      dx = kinematics_jit_fn(mx_all, dx)
-
-      dx_all = collision_jit_fn(mx_all, dx)
-      dx_top_k = collision_jit_fn(mx_top_k, dx)
-
-      self.assertEqual(dx_all.contact.dist.shape, (6,))
-      self.assertEqual(dx_top_k.contact.dist.shape, (2,))
-      self.assertTrue((dx_top_k.contact.dist < 0).all())
+    dx_all = collision_jit_fn(mx_all, dx)
+    dx_top_k = collision_jit_fn(mx_top_k, dx)
+
+    self.assertEqual(dx_all.contact.dist.shape, (6,))
+    self.assertEqual(dx_top_k.contact.dist.shape, (2,))
+    self.assertTrue((dx_top_k.contact.dist < 0).all())
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/collision_primitive.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_primitive.py`

 * *Files 15% similar despite different names*

```diff
@@ -61,14 +61,27 @@
     dist, pos = _plane_sphere(n, plane.pos, cap.pos + offset, cap.size[0])
     dist = jp.expand_dims(dist, axis=0)
     pos = jp.expand_dims(pos, axis=0)
     contacts.append((dist, pos, frame))
   return jax.tree_map(lambda *x: jp.concatenate(x), *contacts)
 
 
+def plane_ellipsoid(plane: GeomInfo, ellipsoid: GeomInfo) -> Contact:
+  """Calculates one contact between an ellipsoid and a plane."""
+  n = plane.mat[:, 2]
+  size = ellipsoid.size
+  sphere_support = -math.normalize((ellipsoid.mat.T @ n) * size)
+  pos = ellipsoid.pos + ellipsoid.mat @ (sphere_support * size)
+  dist = jp.dot(n, pos - plane.pos)
+  pos = pos - n * dist * 0.5
+  return jax.tree_map(
+      lambda x: jp.expand_dims(x, axis=0), (dist, pos, math.make_frame(n))
+  )
+
+
 def _sphere_sphere(
     pos1: jax.Array, radius1: jax.Array, pos2: jax.Array, radius2: jax.Array
 ) -> Contact:
   """Returns the penetration, contact point, and normal between two spheres."""
   n, dist = math.normalize_with_norm(pos2 - pos1)
   n = jp.where(dist == 0.0, jp.array([1.0, 0.0, 0.0]), n)
   dist = dist - (radius1 + radius2)
@@ -117,10 +130,11 @@
   return jax.tree_map(
       lambda x: jp.expand_dims(x, axis=0), (dist, pos, math.make_frame(n))
   )
 
 # store ncon as function attributes
 plane_sphere.ncon = 1
 plane_capsule.ncon = 2
+plane_ellipsoid.ncon = 1
 sphere_sphere.ncon = 1
 sphere_capsule.ncon = 1
 capsule_capsule.ncon = 1
```

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/constraint.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/constraint.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/constraint_test.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/constraint_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/dataclasses.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/dataclasses.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/device.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,25 +134,30 @@
   ):
     raise NotImplementedError('Only condim=3 is supported.')
 
   if m.ntendon:
     raise NotImplementedError('Tendons are not supported.')
 
   # check collision geom types
-  candidate_set = collision_driver.collision_candidates(m)
-  for g1, g2, *_ in candidate_set:
+  for (g1, g2, *_), c in collision_driver.collision_candidates(m).items():
     g1, g2 = mujoco.mjtGeom(g1), mujoco.mjtGeom(g2)
     if g1 == mujoco.mjtGeom.mjGEOM_PLANE and g2 in (
         mujoco.mjtGeom.mjGEOM_PLANE,
         mujoco.mjtGeom.mjGEOM_HFIELD,
     ):
       # MuJoCo does not collide planes with other planes or hfields
       continue
     if collision_driver.get_collision_fn((g1, g2)) is None:
       raise NotImplementedError(f'({g1}, {g2}) collisions not implemented.')
+    *_, params = collision_driver.get_params(m, c)
+    margin_gap = not np.allclose(np.concatenate([params.margin, params.gap]), 0)
+    if mujoco.mjtGeom.mjGEOM_MESH in (g1, g2) and margin_gap:
+      raise NotImplementedError(
+          f'Margin and gap not implemented for ({g1}, {g2})'
+      )
 
   # TODO(erikfrey): warn for high solver iterations, nefc, etc.
 
   # mjNDISABLE is not a DisableBit flag, so must be explicitly ignored
   disablebit_members = set(mujoco.mjtDisableBit.__members__.values()) - {
       mujoco.mjtDisableBit.mjNDISABLE}
   unsupported_disable = disablebit_members - {
```

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/device_test.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/device_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/forward.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/forward.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/forward_test.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/forward_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/io.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,18 +87,24 @@
   if m.ntendon:
     raise NotImplementedError('tendons are not supported')
 
   if (m.geom_condim != 3).any() or (m.pair_dim != 3).any():
     raise NotImplementedError('only condim=3 is supported')
 
   # check collision geom types
-  for g1, g2, *_ in collision_driver.collision_candidates(m):
+  for (g1, g2, *_), c in collision_driver.collision_candidates(m).items():
+    g1, g2 = mujoco.mjtGeom(g1), mujoco.mjtGeom(g2)
     if collision_driver.get_collision_fn((g1, g2)) is None:
-      g1, g2 = mujoco.mjtGeom(g1), mujoco.mjtGeom(g2)
       raise NotImplementedError(f'({g1}, {g2}) has no collision function')
+    *_, params = collision_driver.get_params(m, c)
+    margin_gap = not np.allclose(np.concatenate([params.margin, params.gap]), 0)
+    if mujoco.mjtGeom.mjGEOM_MESH in (g1, g2) and margin_gap:
+      raise NotImplementedError(
+          f'Margin and gap not implemented for ({g1}, {g2})'
+      )
 
   for enum_field, enum_type, mj_type in (
       (m.actuator_biastype, types.BiasType, mujoco.mjtBias),
       (m.actuator_dyntype, types.DynType, mujoco.mjtDyn),
       (m.actuator_gaintype, types.GainType, mujoco.mjtGain),
       (m.actuator_trntype, types.TrnType, mujoco.mjtTrn),
       (m.eq_type, types.EqType, mujoco.mjtEq),
@@ -168,15 +174,15 @@
       qpos=jp.array(m.qpos0),
       qvel=zero_nv,
       act=zero_na,
       qacc_warmstart=zero_nv,
       ctrl=zero_nu,
       qfrc_applied=zero_nv,
       xfrc_applied=zero_nbody_6,
-      eq_active=jp.zeros(m.neq, dtype=int),
+      eq_active=jp.zeros(m.neq, dtype=jp.uint8),
       qacc=zero_nv,
       act_dot=zero_na,
       xpos=zero_nbody_3,
       xquat=jp.zeros((m.nbody, 4), dtype=float),
       xmat=zero_nbody_3_3,
       xipos=zero_nbody_3,
       ximat=zero_nbody_3_3,
@@ -209,14 +215,15 @@
       efc_aref=zero_nefc,
       qfrc_actuator=zero_nv,
       qfrc_smooth=zero_nv,
       qacc_smooth=zero_nv,
       qfrc_constraint=zero_nv,
       qfrc_inverse=zero_nv,
       efc_force=zero_nefc,
+      userdata=jp.zeros(m.nuserdata, dtype=float),
   )
 
   return d
 
 
 def _get_contact(
     c: mujoco._structs._MjContactList,
@@ -229,14 +236,15 @@
     value = getattr(cx, field.name)[con_id]
     if field.name == 'frame':
       value = value.reshape((-1, 9))
     getattr(c, field.name)[:] = value
 
   ncon = cx.dist.shape[0]
   c.efc_address[:] = np.arange(efc_start, efc_start + ncon * 4, 4)[con_id]
+  c.dim[:] = 3
 
 
 def get_data(
     m: mujoco.MjModel, d: types.Data
 ) -> Union[mujoco.MjData, List[mujoco.MjData]]:
   """Gets mjx.Data from a device, resulting in mujoco.MjData or List[MjData]."""
   batched = len(d.qpos.shape) > 1
@@ -370,14 +378,17 @@
       for f in types.Data.fields()
       if f.type is jax.Array
   }
 
   for fname in ('xmat', 'ximat', 'geom_xmat', 'site_xmat', 'cam_xmat'):
     fields[fname] = fields[fname].reshape((-1, 3, 3))
 
+  # MJX does not support islanding, so only transfer the first solver_niter
+  fields['solver_niter'] = fields['solver_niter'][0]
+
   # pad efc fields: MuJoCo efc arrays are sparse for inactive constraints.
   # efc_J is also optionally column-sparse (typically for large nv).  MJX is
   # neither: it contains zeros for inactive constraints, and efc_J is always
   # (nefc, nv).  this may change in the future.
   if mujoco.mj_isSparse(m):
     nr = d.efc_J_rownnz.shape[0]
     efc_j = np.zeros((nr, m.nv))
```

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/io_test.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/io_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     np.testing.assert_allclose(mx.body_parentid, m.body_parentid)
     np.testing.assert_allclose(mx.geom_type, m.geom_type)
     np.testing.assert_allclose(mx.geom_bodyid, m.geom_bodyid)
     np.testing.assert_almost_equal(mx.geom_solref, m.geom_solref)
     np.testing.assert_almost_equal(mx.geom_pos, m.geom_pos)
     self.assertLen(mx.geom_convex_face, 6)
     self.assertLen(mx.geom_convex_vert, 6)
-    self.assertLen(mx.geom_convex_edge, 6)
+    self.assertLen(mx.geom_convex_edge_dir, 6)
     self.assertLen(mx.geom_convex_facenormal, 6)
 
     np.testing.assert_allclose(mx.jnt_type, m.jnt_type)
     np.testing.assert_allclose(mx.jnt_dofadr, m.jnt_dofadr)
     np.testing.assert_allclose(mx.jnt_bodyid, m.jnt_bodyid)
     np.testing.assert_allclose(mx.jnt_limited, m.jnt_limited)
     np.testing.assert_almost_equal(mx.jnt_axis, m.jnt_axis)
@@ -205,14 +205,33 @@
             <body>
               <freejoint/>
               <geom size="0.05"/>
             </body>
           </worldbody>
         </mujoco>"""))
 
+  def test_margin_gap_mesh_not_implemented(self):
+    with self.assertRaises(NotImplementedError):
+      mjx.put_model(mujoco.MjModel.from_xml_string("""
+        <mujoco>
+          <asset>
+            <mesh name="box" vertex="-1 -1 -1 1 -1 -1 1 1 -1 1 1 1 1 -1 1 -1 1 -1 -1 1 1 -1 -1 1" scale="1 1 1"/>
+          </asset>
+          <worldbody>
+            <body>
+              <freejoint/>
+              <geom type="mesh" mesh="box" margin="0.3"/>
+            </body>
+            <body>
+              <freejoint/>
+              <geom size="0.05"/>
+            </body>
+          </worldbody>
+        </mujoco>"""))
+
 
 class DataIOTest(parameterized.TestCase):
   """IO tests for mjx.Data."""
 
   def test_make_data(self):
     """Test that make_data returns the correct shapes."""
 
@@ -430,9 +449,24 @@
     # only 1 contact active
     self.assertEqual(d_2.contact.dist.shape, (1,))
     self.assertEqual(d_2.ncon, 1)
     np.testing.assert_allclose(d_2.contact.dist, d.contact.dist)
     self.assertEqual(d_2.contact.frame.shape, (1, 9))
     np.testing.assert_allclose(d_2.contact.frame, d.contact.frame)
 
+  def test_make_matches_put(self):
+    """Test that make_data produces a pytree that matches put_data."""
+
+    m = mujoco.MjModel.from_xml_string(_MULTIPLE_CONSTRAINTS)
+    d = mujoco.MjData(m)
+    mujoco.mj_step(m, d, 2)
+    dx = mjx.put_data(m, d)
+
+    step_fn = lambda d: d.replace(time=d.time + 1)
+    step_fn_jit = jax.jit(step_fn).lower(dx).compile()
+
+    # placing an MjData onto device should yield the same treedef mjx.Data as
+    # calling make_data.  they should be interchangeable for jax functions:
+    step_fn_jit(mjx.make_data(m))
+
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/math.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/math.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,14 +241,19 @@
   tri_id = jp.array([[0, 3, 4], [3, 1, 5], [4, 5, 2]])  # cinert inr order
   inr, pos, mass = i[tri_id], i[6:9], i[9]
   ang = jp.dot(inr, v[:3]) + jp.cross(pos, v[3:])
   vel = mass * v[3:] - jp.cross(pos, v[:3])
   return jp.concatenate((ang, vel))
 
 
+def sign(x: jax.Array) -> jax.Array:
+  """Returns the sign of x in the set {-1, 1}."""
+  return jp.where(x < 0, -1, 1)
+
+
 def transform_motion(vel: jax.Array, offset: jax.Array, rotmat: jax.Array):
   """Transform spatial motion.
 
   Args:
     vel: (6,) spatial motion (3 angular, 3 linear)
     offset: (3,) translation
     rotmat: (3, 3) rotation
```

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/math_test.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/math_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/mesh.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/mesh.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,16 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Mesh processing."""
 
+import collections
+import dataclasses
 import itertools
-from typing import Dict, Optional, Sequence, Tuple
+from typing import Dict, List, Optional, Sequence, Tuple
+import warnings
 
 import mujoco
 # pylint: disable=g-importing-member
 from mujoco.mjx._src.types import GeomType
 from mujoco.mjx._src.types import Model
 # pylint: enable=g-importing-member
 import numpy as np
@@ -40,16 +43,18 @@
 ]
 # pyformat: enable
 _MAX_HULL_FACE_VERTICES = 20
 _CONVEX_CACHE: Dict[Tuple[int, int], Dict[str, np.ndarray]] = {}
 _DERIVED_ARGS = [
     'geom_convex_face',
     'geom_convex_vert',
-    'geom_convex_edge',
+    'geom_convex_edge_dir',
     'geom_convex_facenormal',
+    'geom_convex_edge',
+    'geom_convex_edge_face_normal',
 ]
 DERIVED = {(Model, d) for d in _DERIVED_ARGS}
 
 
 def _box(size: np.ndarray):
   """Creates a mesh for a box with rectangular faces."""
   box_corners = np.array(_BOX_CORNERS)
@@ -69,16 +74,16 @@
   edge0 = face_vert[:, 1, :] - face_vert[:, 0, :]
   edge1 = face_vert[:, -1, :] - face_vert[:, 0, :]
   face_norm = np.cross(edge0, edge1)
   face_norm = face_norm / np.linalg.norm(face_norm, axis=1).reshape((-1, 1))
   return face_norm
 
 
-def _get_unique_edges(vert: np.ndarray, face: np.ndarray) -> np.ndarray:
-  """Returns unique edges.
+def _get_unique_edge_dir(vert: np.ndarray, face: np.ndarray) -> np.ndarray:
+  """Returns unique edge directions.
 
   Args:
     vert: (n_vert, 3) vertices
     face: (n_face, n_vert) face index array
 
   Returns:
     edges: tuples of vertex indexes for each edge
@@ -105,14 +110,51 @@
   )
   matches = np.tril(matches).sum(axis=-1)
   unique_edge_idx = np.where(matches == 1)[0]
 
   return edges[unique_edge_idx]
 
 
+def _get_edge_normals(
+    face: np.ndarray, face_norm: np.ndarray
+) -> Tuple[np.ndarray, np.ndarray]:
+  """Returns face edges and face edge normals."""
+  # get face edges and scatter the face norms
+  r_face = np.roll(face, 1, axis=1)
+  face_edge = np.array([face, r_face]).transpose((1, 2, 0))
+  face_edge.sort(axis=2)
+  face_edge_flat = np.concatenate(face_edge)
+  edge_face_idx = np.repeat(np.arange(face.shape[0]), face.shape[1])
+  edge_face_norm = face_norm[edge_face_idx]
+
+  # get the edge normals associated with each edge
+  edge_map_list = collections.defaultdict(list)
+  for i in range(face_edge_flat.shape[0]):
+    if face_edge_flat[i][0] == face_edge_flat[i][1]:
+      continue
+    edge_map_list[tuple(face_edge_flat[i])].append(edge_face_norm[i])
+
+  edges, edge_face_normals = [], []
+  for k, v in edge_map_list.items():
+    v = np.array(v)
+    if len(v) > 2:
+      # Meshes can be of poor quality and contain edges adjacent to more than
+      # two faces. We take the first two unique face normals.
+      v = np.unique(v, axis=0)[:2]
+    elif len(v) == 1:
+      # Some edges are either degenerate or _MAX_HULL_FACE_VERTICES was hit
+      # and face vertices were down sampled. In either case, we ignore these
+      # edges.
+      continue
+    edges.append(k)
+    edge_face_normals.append(v)
+
+  return np.array(edges), np.array(edge_face_normals)
+
+
 def _convex_hull_2d(points: np.ndarray, normal: np.ndarray) -> np.ndarray:
   """Calculates the convex hull for a set of points on a plane."""
   # project points onto the closest axis plane
   best_axis = np.abs(np.eye(3).dot(normal)).argmax()
   axis = np.eye(3)[best_axis]
   d = points.dot(axis).reshape((-1, 1))
   axis_points = points - d * axis
@@ -124,15 +166,24 @@
   order_ *= np.where(best_axis == 1, -1, 1)
   hull_point_idx = c.vertices[::order_]
   assert (axis_points - c.points).sum() == 0
 
   return hull_point_idx
 
 
-def _merge_coplanar(tm: trimesh.Trimesh) -> np.ndarray:
+@dataclasses.dataclass
+class MeshInfo:
+  name: str
+  vert: np.ndarray
+  face: np.ndarray
+  convex_vert: Optional[np.ndarray]
+  convex_face: Optional[np.ndarray]
+
+
+def _merge_coplanar(tm: trimesh.Trimesh, mesh_info: MeshInfo) -> np.ndarray:
   """Merges coplanar facets."""
   if not tm.facets:
     return tm.faces.copy()  # no facets
   if not tm.faces.shape[0]:
     raise ValueError('Mesh has no faces.')
 
   # Get faces.
@@ -148,14 +199,21 @@
     normal = tm.facets_normal[i]
 
     # convert triangulated facet to a polygon
     hull_point_idx = _convex_hull_2d(points, normal)
     face = point_idx[hull_point_idx]
 
     # resize faces that exceed max polygon vertices
+    if face.shape[0] > _MAX_HULL_FACE_VERTICES:
+      warnings.warn(
+          f'Mesh "{mesh_info.name}" has a coplanar face with more than'
+          f' {_MAX_HULL_FACE_VERTICES} vertices. This may lead to performance '
+          'issues and inaccuracies in collision detection. Consider '
+          'decimating the mesh.'
+      )
     every = face.shape[0] // _MAX_HULL_FACE_VERTICES + 1
     face = face[::every]
     facets.append(face)
 
   # Pad facets so that they can be stacked.
   max_len = max(f.shape[0] for f in facets) if facets else faces.shape[1]
   assert max_len <= _MAX_HULL_FACE_VERTICES
@@ -169,69 +227,110 @@
     return np.array(facets)  # no faces, return facets
 
   # Merge faces and facets.
   faces = np.pad(faces, ((0, 0), (0, max_len - faces.shape[1])), 'edge')
   return np.concatenate([faces, facets])
 
 
-def _get_faces_verts(
+def _mesh_info(
     m: mujoco.MjModel,
-) -> Tuple[Sequence[np.ndarray], Sequence[np.ndarray]]:
-  """Extracts mesh faces and vertices from MjModel."""
-  verts, faces = [], []
+) -> List[MeshInfo]:
+  """Extracts mesh info from MjModel."""
+  mesh_infos = []
   for i in range(m.nmesh):
+    name = mujoco.mj_id2name(m, mujoco.mjtObj.mjOBJ_MESH.value, i)
+
     last = (i + 1) >= m.nmesh
     face_start = m.mesh_faceadr[i]
     face_end = m.mesh_faceadr[i + 1] if not last else m.mesh_face.shape[0]
     face = m.mesh_face[face_start:face_end]
-    faces.append(face)
 
     vert_start = m.mesh_vertadr[i]
     vert_end = m.mesh_vertadr[i + 1] if not last else m.mesh_vert.shape[0]
     vert = m.mesh_vert[vert_start:vert_end]
-    verts.append(vert)
-  return verts, faces
+
+    graphadr = m.mesh_graphadr[i]
+    if graphadr < 0:
+      mesh_infos.append(MeshInfo(name, vert, face, None, None))
+      continue
+
+    graph = m.mesh_graph[graphadr:]
+    numvert, numface = graph[0], graph[1]
+
+    # unused vert_edgeadr
+    # vert_edgeadr = graph[2 : numvert + 2]
+    last_idx = numvert + 2
+
+    vert_globalid = graph[last_idx : last_idx + numvert]
+    last_idx += numvert
+
+    # unused edge_localid
+    # edge_localid = graph[last_idx : last_idx + numvert + 3 * numface]
+    last_idx += numvert + 3 * numface
+
+    face_globalid = graph[last_idx : last_idx + 3 * numface]
+    face_globalid = face_globalid.reshape((numface, 3))
+
+    convex_vert = vert[vert_globalid]
+    vertex_map = dict(zip(vert_globalid, np.arange(vert_globalid.shape[0])))
+    convex_face = np.vectorize(vertex_map.get)(face_globalid)
+    mesh_infos.append(MeshInfo(name, vert, face, convex_vert, convex_face))
+
+  return mesh_infos
 
 
 def _geom_mesh_kwargs(
-    vert: np.ndarray, face: np.ndarray
+    mesh_info: MeshInfo,
 ) -> Dict[str, np.ndarray]:
   """Generates convex mesh attributes for mjx.Model."""
-  tm = trimesh.Trimesh(vertices=vert, faces=face)
-  tm_convex = trimesh.convex.convex_hull(tm)
+  tm_convex = trimesh.Trimesh(
+      vertices=mesh_info.convex_vert, faces=mesh_info.convex_face
+  )
   vert = np.array(tm_convex.vertices)
-  face = _merge_coplanar(tm_convex)
+  face = _merge_coplanar(tm_convex, mesh_info)
+  facenormal = _get_face_norm(vert, face)
+  edge, edge_face_normal = _get_edge_normals(face, facenormal)
   return {
       'geom_convex_face': vert[face],
       'geom_convex_face_vert_idx': face,
       'geom_convex_vert': vert,
-      'geom_convex_edge': _get_unique_edges(vert, face),
-      'geom_convex_facenormal': _get_face_norm(vert, face),
+      'geom_convex_edge_dir': _get_unique_edge_dir(vert, face),
+      'geom_convex_facenormal': facenormal,
+      'geom_convex_edge': edge,
+      'geom_convex_edge_face_normal': edge_face_normal,
   }
 
 
 def get(m: mujoco.MjModel) -> Dict[str, Sequence[Optional[np.ndarray]]]:
   """Derives geom mesh attributes for mjx.Model from MjModel."""
   kwargs = {k: [] for k in _DERIVED_ARGS}
-  verts, faces = _get_faces_verts(m)
+  mesh_infos = _mesh_info(m)
   geom_con = m.geom_conaffinity | m.geom_contype
   for geomid in range(m.ngeom):
+    mesh_info = None
     dataid = m.geom_dataid[geomid]
     if not geom_con[geomid]:
       # ignore visual-only meshes
       kwargs = {k: kwargs[k] + [None] for k in _DERIVED_ARGS}
       continue
     elif m.geom_type[geomid] == GeomType.BOX:
       vert, face = _box(m.geom_size[geomid])
-    elif dataid >= 0:
-      vert, face = verts[dataid], faces[dataid]
-    else:
+      mesh_info = MeshInfo(
+          name='box',
+          vert=vert,
+          face=face,
+          convex_vert=vert,
+          convex_face=face,
+      )
+    elif dataid < 0:
       kwargs = {k: kwargs[k] + [None] for k in _DERIVED_ARGS}
       continue
 
+    mesh_info = mesh_info or mesh_infos[dataid]
+    vert, face = mesh_info.vert, mesh_info.face
     key = (hash(vert.data.tobytes()), hash(face.data.tobytes()))
     if key not in _CONVEX_CACHE:
-      _CONVEX_CACHE[key] = _geom_mesh_kwargs(vert, face)
+      _CONVEX_CACHE[key] = _geom_mesh_kwargs(mesh_info)
 
     kwargs = {k: kwargs[k] + [_CONVEX_CACHE[key][k]] for k in _DERIVED_ARGS}
 
   return kwargs
```

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/mesh_test.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/mesh_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 """Tests for mesh.py."""
 
 from absl.testing import absltest
 from mujoco.mjx._src import mesh
 import numpy as np
+import trimesh
 
 
 class GeomMeshKwargsTest(absltest.TestCase):
 
   def test_pyramid(self):
     """Tests that a triangulated pyramid converts to merged coplanar faces."""
     vert = np.array([
@@ -29,15 +30,26 @@
         [-0.025, -0.05, 0.05],
         [-0.025, 0.05, -0.05],
         [0.075, 0.0, 0.0],
     ])
     face = np.array(
         [[0, 1, 2], [0, 3, 1], [0, 4, 3], [0, 2, 4], [2, 1, 4], [1, 3, 4]]
     )
-    h = mesh._geom_mesh_kwargs(vert, face)
+    tm = trimesh.Trimesh(vertices=vert, faces=face)
+    tm_convex = trimesh.convex.convex_hull(tm)
+    convex_vert = np.array(tm_convex.vertices)
+    convex_face = np.array(tm_convex.faces)
+    mesh_info = mesh.MeshInfo(
+        name='test',
+        vert=vert,
+        face=face,
+        convex_vert=convex_vert,
+        convex_face=convex_face,
+    )
+    h = mesh._geom_mesh_kwargs(mesh_info)
 
     # get index of vertices in h['geom_convex_vert'] for vertices in vert
     dist = np.repeat(vert, vert.shape[0], axis=0) - np.tile(
         h['geom_convex_vert'], (vert.shape[0], 1)
     )
     dist = (dist**2).sum(axis=1).reshape((vert.shape[0], -1))
     vidx = np.argmin(dist, axis=0)
@@ -53,24 +65,60 @@
         (0, 3, 4), (1, 3, 4), (0, 2, 4), (0, 1, 2, 3), (1, 2, 4)])
     self.assertSequenceEqual(
         face_verts,
         expected_face_verts,
     )
 
     # check edges
-    unique_edge = np.vectorize(map_.get)(h['geom_convex_edge'])
+    unique_edge = np.vectorize(map_.get)(h['geom_convex_edge_dir'])
     unique_edge = np.array(sorted(unique_edge.tolist()))
     np.testing.assert_array_equal(
         unique_edge,
         np.array([[0, 2], [0, 3], [0, 4], [1, 4], [2, 4], [3, 4]]),
     )
 
     # face normals
     self.assertEqual(h['geom_convex_facenormal'].shape, (5, 3))
 
+    # face edges
+    edges = h['geom_convex_edge']
+    edges = np.vectorize(map_.get)(edges)
+    mask = edges[:, 0] != edges[:, 1]
+    edges = edges[mask]
+    sort_col_idx = np.argsort(edges, axis=1)
+    edges = np.take_along_axis(edges, sort_col_idx, axis=1)
+    sort_row_idx = np.lexsort((edges[:, 1], edges[:, 0]))
+    edges = edges[sort_row_idx]
+    np.testing.assert_array_equal(
+        edges,
+        np.array([
+            [0, 2],
+            [0, 3],
+            [0, 4],
+            [1, 2],
+            [1, 3],
+            [1, 4],
+            [2, 4],
+            [3, 4],
+        ]),
+    )
+
+    # face edge normals
+    edge_normal = h['geom_convex_edge_face_normal']
+    edge_normal = edge_normal[mask]
+    edge_normal = np.take_along_axis(
+        edge_normal, sort_col_idx[..., None], axis=1
+    )
+    edge_normal = edge_normal[sort_row_idx]
+    edge_normal_02 = np.array([[0.4472136, -0.0, 0.89442719], [-1.0, 0.0, 0.0]])
+    np.testing.assert_array_almost_equal(
+        edge_normal[:1],
+        np.array([edge_normal_02]),
+    )
+
 
 class ConvexHull2DTest(absltest.TestCase):
 
   def test_convex_hull_2d_axis1(self):
     """Tests for the correct winding order of a polgyon with +y normal."""
     pts = np.array([
         [-0.04634297, -0.06652775, 0.05853534],
@@ -105,15 +153,15 @@
 
   def test_tetrahedron_edges(self):
     """Tests unique edges for a tetrahedron."""
     vert = np.array(
         [[-0.1, 0.0, -0.1], [0.0, 0.1, 0.1], [0.1, 0.0, -0.1], [0.0, -0.1, 0.1]]
     )
     face = np.array([[0, 1, 2], [0, 2, 3], [0, 3, 1], [2, 1, 3]])
-    idx = mesh._get_unique_edges(vert, face)
+    idx = mesh._get_unique_edge_dir(vert, face)
     np.testing.assert_array_equal(
         idx, np.array([[0, 1], [0, 2], [0, 3], [1, 2], [1, 3], [2, 3]])
     )
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/passive.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/passive.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/passive_test.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/passive_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/ray.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/ray.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/ray_test.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/ray_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/scan.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/scan.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/scan_test.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/scan_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/smooth.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/smooth.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/smooth_test.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/smooth_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/solver.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/solver.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/solver_test.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/solver_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/support.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/support.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Engine support functions."""
-
 from typing import Optional, Tuple, Union
 
 import jax
 from jax import numpy as jp
 import mujoco
 from mujoco.mjx._src import math
 from mujoco.mjx._src import scan
```

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/support_test.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/support_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/test_util.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/test_util.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,22 +10,104 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Utilities for testing."""
 
+import os
 import sys
+import time
 from typing import Dict, Tuple
 from xml.etree import ElementTree as ET
 
 from etils import epath
+import jax
 import mujoco
+# pylint: disable=g-importing-member
+from mujoco.mjx._src import forward
+from mujoco.mjx._src import io
+# pylint: enable=g-importing-member
 import numpy as np
 
+
+def _measure(fn, *args) -> Tuple[float, float]:
+  """Reports jit time and op time for a function."""
+
+  beg = time.perf_counter()
+  compiled_fn = fn.lower(*args).compile()
+  end = time.perf_counter()
+  jit_time = end - beg
+
+  beg = time.perf_counter()
+  result = compiled_fn(*args)
+  jax.block_until_ready(result)
+  end = time.perf_counter()
+  run_time = end - beg
+
+  return jit_time, run_time
+
+
+def benchmark(
+    m: mujoco.MjModel,
+    nstep: int = 1000,
+    batch_size: int = 1024,
+    unroll_steps: int = 1,
+    solver: str = 'cg',
+    iterations: int = 1,
+    ls_iterations: int = 4,
+) -> Tuple[float, float, int]:
+  """Benchmark a model."""
+
+  xla_flags = os.environ.get('XLA_FLAGS', '')
+  xla_flags += ' --xla_gpu_triton_gemm_any=True'
+  os.environ['XLA_FLAGS'] = xla_flags
+
+  m.opt.solver = {
+      'cg': mujoco.mjtSolver.mjSOL_CG,
+      'newton': mujoco.mjtSolver.mjSOL_NEWTON,
+  }[solver.lower()]
+  m.opt.iterations = iterations
+  m.opt.ls_iterations = ls_iterations
+  m = io.put_model(m)
+
+  @jax.pmap
+  def init(key):
+    key = jax.random.split(key, batch_size // jax.device_count())
+
+    @jax.vmap
+    def random_init(key):
+      d = io.make_data(m)
+      qvel = 0.01 * jax.random.normal(key, shape=(m.nv,))
+      d = d.replace(qvel=qvel)
+      return d
+
+    return random_init(key)
+
+  key = jax.random.split(jax.random.key(0), jax.device_count())
+  d = init(key)
+  jax.block_until_ready(d)
+
+  @jax.pmap
+  def unroll(d):
+    @jax.vmap
+    def step(d, _):
+      d = forward.step(m, d)
+      return d, None
+
+    d, _ = jax.lax.scan(step, d, None, length=nstep, unroll=unroll_steps)
+
+    return d
+
+  jit_time, run_time = _measure(unroll, d)
+  steps = nstep * batch_size
+
+  return jit_time, run_time, steps
+
+
 _ACTUATOR_TYPES = ['motor', 'velocity', 'position', 'general', 'intvelocity']
 _DYN_TYPES = ['none', 'integrator', 'filter', 'filterexact']
 _DYN_PRMS = ['0.189', '2.1']
 _JOINT_TYPES = ['free', 'hinge', 'slide', 'ball']
 _JOINT_AXES = ['1 0 0', '0 1 0', '0 0 1']
 _FRICTIONS = ['1.2 0.003 0.0002', '0.2 0.0001 0.0005']
 _KP_POS = ['1', '2']
```

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/_src/types.py` & `mujoco-mjx-3.1.4/mujoco/mjx/_src/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,14 +306,15 @@
     nmeshvert: number of vertices in all meshes
     nmeshface: number of triangular faces in all meshes
     nmat: number of materials
     npair: number of predefined geom pairs
     nexclude: number of excluded geom pairs
     neq: number of equality constraints
     nnumeric: number of numeric custom fields
+    nuserdata: size of userdata array
     nM: number of non-zeros in sparse inertia matrix
     opt: physics options
     stat: model statistics
     qpos0: qpos values at default pose                        (nq,)
     qpos_spring: reference pose for springs                   (nq,)
     body_parentid: id of body's parent                        (nbody,)
     body_rootid: id of root above body                        (nbody,)
@@ -390,16 +391,18 @@
     mat_rgba: rgba                                            (nmat, 4)
     mesh_vertadr: first vertex address                        (nmesh x 1)
     mesh_faceadr: first face address                          (nmesh x 1)
     mesh_vert: vertex positions for all meshes                (nmeshvert, 3)
     mesh_face: vertex face data                               (nmeshface, 3)
     geom_convex_face: vertex face data, MJX only              (ngeom,)
     geom_convex_vert: vertex data, MJX only                   (ngeom,)
-    geom_convex_edge: unique edge data, MJX only              (ngeom,)
+    geom_convex_edge_dir: unique edge direction, MJX only     (ngeom,)
     geom_convex_facenormal: normal face data, MJX only        (ngeom,)
+    geom_convex_face_edge: edges for each face                (ngeom,)
+    geom_convex_face_edge_normal: edge normals for each face  (ngeom,)
     pair_dim: contact dimensionality                          (npair,)
     pair_geom1: id of geom1                                   (npair,)
     pair_geom2: id of geom2                                   (npair,)
     pair_solref: solver reference: contact normal             (npair, mjNREF)
     pair_solreffriction: solver reference: contact friction   (npair, mjNREF)
     pair_solimp: solver impedance: contact                    (npair, mjNIMP)
     pair_margin: include in solver if dist<margin-gap         (npair,)
@@ -448,14 +451,15 @@
   nmeshvert: int
   nmeshface: int
   nmat: int
   npair: int
   nexclude: int
   neq: int
   nnumeric: int
+  nuserdata: int
   nM: int  # pylint:disable=invalid-name
   opt: Option
   stat: Statistic
   qpos0: jax.Array
   qpos_spring: jax.Array
   body_parentid: np.ndarray
   body_rootid: np.ndarray
@@ -535,16 +539,18 @@
   mesh_face: np.ndarray
   mat_rgba: np.ndarray
   pair_dim: np.ndarray
   pair_geom1: np.ndarray
   pair_geom2: np.ndarray
   geom_convex_face: List[Optional[jax.Array]]
   geom_convex_vert: List[Optional[jax.Array]]
-  geom_convex_edge: List[Optional[jax.Array]]
+  geom_convex_edge_dir: List[Optional[jax.Array]]
   geom_convex_facenormal: List[Optional[jax.Array]]
+  geom_convex_edge: List[Optional[jax.Array]]
+  geom_convex_edge_face_normal: List[Optional[jax.Array]]
   pair_solref: jax.Array
   pair_solreffriction: jax.Array
   pair_solimp: jax.Array
   pair_margin: jax.Array
   pair_gap: jax.Array
   pair_friction: jax.Array
   exclude_signature: np.ndarray
@@ -677,14 +683,15 @@
     qfrc_actuator: actuator force                                 (nv,)
     qfrc_smooth: net unconstrained force                          (nv,)
     qacc_smooth: unconstrained acceleration                       (nv,)
     qfrc_constraint: constraint force                             (nv,)
     qfrc_inverse: net external force; should equal:               (nv,)
       qfrc_applied + J'*xfrc_applied + qfrc_actuator
     efc_force: constraint force in constraint space               (nefc,)
+    userdata: user data, not touched by engine                    (nuserdata,)
   """
   # solver statistics:
   solver_niter: jax.Array
   # global properties:
   time: jax.Array
   # state:
   qpos: jax.Array
@@ -695,14 +702,16 @@
   ctrl: jax.Array
   qfrc_applied: jax.Array
   xfrc_applied: jax.Array
   eq_active: jax.Array
   # dynamics:
   qacc: jax.Array
   act_dot: jax.Array
+  # user data:
+  userdata: jax.Array
   # position dependent:
   xpos: jax.Array
   xquat: jax.Array
   xmat: jax.Array
   xipos: jax.Array
   ximat: jax.Array
   xanchor: jax.Array
```

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/integration_test/collision_driver_test.py` & `mujoco-mjx-3.1.4/mujoco/mjx/integration_test/collision_driver_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/integration_test/forward_test.py` & `mujoco-mjx-3.1.4/mujoco/mjx/integration_test/forward_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/integration_test/smooth_test.py` & `mujoco-mjx-3.1.4/mujoco/mjx/integration_test/smooth_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/README.md` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/README.md`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/abduction.stl` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/abduction.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/barkour_v0_mjx.xml` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/barkour_v0_mjx.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/body.stl` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/body.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/foot.stl` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/foot.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/handle.stl` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/handle.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/head.stl` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/head.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/head_mount.stl` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/head_mount.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/lower_leg_1to1.stl` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/lower_leg_1to1.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/powercable.stl` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/powercable.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/upper_left_1.stl` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_left_1.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/upper_left_2.stl` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_left_2.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/upper_left_3.stl` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_left_3.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/upper_right_1.stl` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_right_1.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/upper_right_2.stl` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_right_2.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/barkour_v0/assets/upper_right_3.stl` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_right_3.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/constraints.xml` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/constraints.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/convex.xml` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/convex.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/humanoid/README.md` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/README.md`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/humanoid/humanoid.png` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/humanoid.png`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/humanoid/humanoid.xml` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/humanoid.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/meshes/dodecahedron.stl` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/meshes/dodecahedron.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/pendula.xml` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/pendula.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/ray.xml` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/ray.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/README.md` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/README.md`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/f_distal_pst.obj` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_distal_pst.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/f_knuckle.obj` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_knuckle.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/f_middle.obj` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_middle.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/f_proximal.obj` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_proximal.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/forearm_0.obj` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/forearm_0.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/forearm_1.obj` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/forearm_1.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/forearm_collision.obj` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/forearm_collision.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/lf_metacarpal.obj` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/lf_metacarpal.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/mounting_plate.obj` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/mounting_plate.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/palm.obj` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/palm.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/th_distal_pst.obj` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/th_distal_pst.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/th_middle.obj` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/th_middle.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/th_proximal.obj` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/th_proximal.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/assets/wrist.obj` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/wrist.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/right_hand.xml` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/right_hand.xml`

 * *Files 1% similar despite different names*

#### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/right_hand.xml` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/right_hand.xml`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <mujoco model="right_shadow_hand">
   <compiler angle="radian" meshdir="assets" autolimits="true"/>
-  <option impratio="10" iterations="1" ls_iterations="4">
+  <option impratio="10" iterations="1" ls_iterations="4" timestep="0.001">
     <flag eulerdamp="disable"/>
   </option>
   <custom>
     <numeric data="15" name="max_contact_points"/>
     <numeric data="15" name="max_geom_pairs"/>
   </custom>
   <default>
@@ -64,15 +64,15 @@
       </default>
       <default class="plastic">
         <geom solimp="0.5 0.99 0.0001" solref="0.005 1"/>
         <default class="plastic_visual">
           <geom type="mesh" material="black" contype="0" conaffinity="0" group="2"/>
         </default>
         <default class="plastic_collision">
-          <geom group="3" contype="0" conaffinity="1"/>
+          <geom group="3" contype="1" conaffinity="1"/>
         </default>
       </default>
     </default>
   </default>
   <asset>
     <material name="black" specular="0.5" shininess="0.25" rgba="0.16355 0.16355 0.16355 1"/>
     <material name="gray" specular="0.0" shininess="0.25" rgba="0.80848 0.80848 0.80848 1"/>
@@ -82,33 +82,35 @@
     <mesh class="right_hand" file="forearm_collision.obj"/>
     <mesh class="right_hand" file="wrist.obj"/>
     <mesh class="right_hand" file="palm.obj"/>
     <mesh class="right_hand" file="f_knuckle.obj"/>
     <mesh class="right_hand" file="f_proximal.obj"/>
     <mesh class="right_hand" file="f_middle.obj"/>
     <mesh class="right_hand" file="f_distal_pst.obj"/>
+    <mesh class="right_hand" file="f_distal_pst_214.obj"/>
     <mesh class="right_hand" file="lf_metacarpal.obj"/>
     <mesh class="right_hand" file="th_proximal.obj"/>
     <mesh class="right_hand" file="th_middle.obj"/>
     <mesh class="right_hand" file="th_distal_pst.obj"/>
+    <mesh class="right_hand" file="th_distal_pst_190.obj"/>
   </asset>
   <worldbody>
     <body name="rh_forearm" childclass="right_hand" quat="1 -1 1 -1">
       <inertial mass="3" pos="0 0 0.09" diaginertia="0.0138 0.0138 0.00744"/>
       <geom class="plastic_visual" mesh="forearm_0" material="gray"/>
       <geom class="plastic_visual" mesh="forearm_1"/>
-      <geom class="plastic_collision" type="mesh" mesh="forearm_collision" conaffinity="0"/>
+      <geom class="plastic_collision" type="mesh" mesh="forearm_collision" conaffinity="0" contype="0"/>
       <geom class="plastic_collision" size="0.035 0.035 0.035" pos="0 -0.01 0.181" quat="0.924909 0 0.380188 0" type="box" conaffinity="0"/>
       <body name="rh_wrist" pos="0 -0.01 0.21301">
         <inertial mass="0.1" pos="0 0 0.029" quat="0.5 0.5 0.5 0.5" diaginertia="6.4e-05 4.38e-05 3.5e-05"/>
         <joint class="wrist_y" name="rh_WRJ2"/>
         <geom class="plastic_visual" mesh="wrist" material="metallic"/>
-        <geom size="0.0135 0.015" quat="0.499998 0.5 0.5 -0.500002" type="cylinder" class="plastic_collision" conaffinity="0"/>
-        <geom size="0.011 0.005" pos="-0.026 0 0.034" quat="1 0 1 0" type="cylinder" class="plastic_collision" conaffinity="0"/>
-        <geom size="0.011 0.005" pos="0.031 0 0.034" quat="1 0 1 0" type="cylinder" class="plastic_collision" conaffinity="0"/>
+        <geom size="0.0135 0.015" quat="0.499998 0.5 0.5 -0.500002" type="cylinder" class="plastic_collision" conaffinity="0" contype="0"/>
+        <geom size="0.011 0.005" pos="-0.026 0 0.034" quat="1 0 1 0" type="cylinder" class="plastic_collision" conaffinity="0" contype="0"/>
+        <geom size="0.011 0.005" pos="0.031 0 0.034" quat="1 0 1 0" type="cylinder" class="plastic_collision" conaffinity="0" contype="0"/>
         <geom size="0.0135 0.009 0.005" pos="-0.021 0 0.011" quat="0.923879 0 0.382684 0" type="box" class="plastic_collision" conaffinity="0"/>
         <geom size="0.0135 0.009 0.005" pos="0.026 0 0.01" quat="0.923879 0 -0.382684 0" type="box" class="plastic_collision" conaffinity="0"/>
         <body name="rh_palm" pos="0 0 0.034">
           <inertial mass="0.3" pos="0 0 0.035" quat="1 0 0 1" diaginertia="0.0005287 0.0003581 0.000191"/>
           <joint class="wrist_x" name="rh_WRJ1"/>
           <site name="grasp_site" pos="0 -.035 0.09" group="4"/>
           <geom class="plastic_visual" mesh="palm"/>
@@ -120,136 +122,136 @@
           <geom size="0.011 0.0025 0.015" pos="0.0125 -0.015 0.004" quat="0.971338 0 0 -0.237703" type="box" class="plastic_collision" conaffinity="2"/>
           <geom size="0.009 0.012 0.002" pos="0.011 0 0.089" type="box" class="plastic_collision" conaffinity="2"/>
           <geom size="0.01 0.012 0.02" pos="-0.03 0 0.009" type="box" class="plastic_collision" conaffinity="2"/>
           <body name="rh_ffknuckle" pos="0.033 0 0.095">
             <inertial mass="0.008" pos="0 0 0" quat="0.5 0.5 -0.5 0.5" diaginertia="3.2e-07 2.6e-07 2.6e-07"/>
             <joint name="rh_FFJ4" class="knuckle"/>
             <geom pos="0 0 0.0005" class="plastic_visual" mesh="f_knuckle" material="metallic"/>
-            <geom size="0.009 0.009" quat="1 0 1 0" type="cylinder" class="plastic_collision" conaffinity="0"/>
+            <geom size="0.009 0.009" quat="1 0 1 0" type="cylinder" class="plastic_collision" conaffinity="0" contype="0"/>
             <body name="rh_ffproximal">
               <inertial mass="0.03" pos="0 0 0.0225" quat="1 0 0 1" diaginertia="1e-05 9.8e-06 1.8e-06"/>
               <joint name="rh_FFJ3" class="proximal"/>
               <geom class="plastic_visual" mesh="f_proximal"/>
-              <geom size="0.009 0.02" pos="0 0 0.025" type="capsule" class="plastic_collision" contype="1"/>
+              <geom size="0.009 0.02" pos="0 0 0.025" type="capsule" class="plastic_collision"/>
               <body name="rh_ffmiddle" pos="0 0 0.045">
                 <inertial mass="0.017" pos="0 0 0.0125" quat="1 0 0 1" diaginertia="2.7e-06 2.6e-06 8.7e-07"/>
                 <joint name="rh_FFJ2" class="middle_distal"/>
                 <geom class="plastic_visual" mesh="f_middle"/>
-                <geom size="0.009 0.0125" pos="0 0 0.0125" type="capsule" class="plastic_collision" contype="1"/>
+                <geom size="0.009 0.0125" pos="0 0 0.0125" type="capsule" class="plastic_collision"/>
                 <body name="rh_ffdistal" pos="0 0 0.025">
                   <inertial mass="0.013" pos="0 0 0.0130769" quat="1 0 0 1" diaginertia="1.28092e-06 1.12092e-06 5.3e-07"/>
                   <joint name="rh_FFJ1" class="middle_distal"/>
                   <geom class="plastic_visual" mesh="f_distal_pst"/>
-                  <geom class="plastic_collision" type="mesh" mesh="f_distal_pst"/>
+                  <geom class="plastic_collision" type="mesh" mesh="f_distal_pst_214" contype="0" conaffinity="2"/>
                 </body>
               </body>
             </body>
           </body>
           <body name="rh_mfknuckle" pos="0.011 0 0.099">
             <inertial mass="0.008" pos="0 0 0" quat="0.5 0.5 -0.5 0.5" diaginertia="3.2e-07 2.6e-07 2.6e-07"/>
             <joint name="rh_MFJ4" class="knuckle"/>
             <geom pos="0 0 0.0005" class="plastic_visual" mesh="f_knuckle" material="metallic"/>
-            <geom size="0.009 0.009" quat="1 0 1 0" type="cylinder" class="plastic_collision" conaffinity="0"/>
+            <geom size="0.009 0.009" quat="1 0 1 0" type="cylinder" class="plastic_collision" conaffinity="0" contype="0"/>
             <body name="rh_mfproximal">
               <inertial mass="0.03" pos="0 0 0.0225" quat="1 0 0 1" diaginertia="1e-05 9.8e-06 1.8e-06"/>
               <joint name="rh_MFJ3" class="proximal"/>
               <geom class="plastic_visual" mesh="f_proximal"/>
-              <geom size="0.009 0.02" pos="0 0 0.025" type="capsule" class="plastic_collision" contype="1"/>
+              <geom size="0.009 0.02" pos="0 0 0.025" type="capsule" class="plastic_collision"/>
               <body name="rh_mfmiddle" pos="0 0 0.045">
                 <inertial mass="0.017" pos="0 0 0.0125" quat="1 0 0 1" diaginertia="2.7e-06 2.6e-06 8.7e-07"/>
                 <joint name="rh_MFJ2" class="middle_distal"/>
                 <geom class="plastic_visual" mesh="f_middle"/>
-                <geom size="0.009 0.0125" pos="0 0 0.0125" type="capsule" class="plastic_collision" contype="1"/>
+                <geom size="0.009 0.0125" pos="0 0 0.0125" type="capsule" class="plastic_collision"/>
                 <body name="rh_mfdistal" pos="0 0 0.025">
                   <inertial mass="0.013" pos="0 0 0.0130769" quat="1 0 0 1" diaginertia="1.28092e-06 1.12092e-06 5.3e-07"/>
                   <joint name="rh_MFJ1" class="middle_distal"/>
                   <geom class="plastic_visual" mesh="f_distal_pst"/>
-                  <geom class="plastic_collision" type="mesh" mesh="f_distal_pst"/>
+                  <geom class="plastic_collision" type="mesh" mesh="f_distal_pst_214" contype="0" conaffinity="2"/>
                 </body>
               </body>
             </body>
           </body>
           <body name="rh_rfknuckle" pos="-0.011 0 0.095">
             <inertial mass="0.008" pos="0 0 0" quat="0.5 0.5 -0.5 0.5" diaginertia="3.2e-07 2.6e-07 2.6e-07"/>
             <joint name="rh_RFJ4" class="knuckle" axis="0 1 0"/>
             <geom pos="0 0 0.0005" class="plastic_visual" mesh="f_knuckle" material="metallic"/>
-            <geom size="0.009 0.009" quat="1 0 1 0" type="cylinder" class="plastic_collision" conaffinity="0"/>
+            <geom size="0.009 0.009" quat="1 0 1 0" type="cylinder" class="plastic_collision" conaffinity="0" contype="0"/>
             <body name="rh_rfproximal">
               <inertial mass="0.03" pos="0 0 0.0225" quat="1 0 0 1" diaginertia="1e-05 9.8e-06 1.8e-06"/>
               <joint name="rh_RFJ3" class="proximal"/>
               <geom class="plastic_visual" mesh="f_proximal"/>
-              <geom size="0.009 0.02" pos="0 0 0.025" type="capsule" class="plastic_collision" contype="1"/>
+              <geom size="0.009 0.02" pos="0 0 0.025" type="capsule" class="plastic_collision"/>
               <body name="rh_rfmiddle" pos="0 0 0.045">
                 <inertial mass="0.017" pos="0 0 0.0125" quat="1 0 0 1" diaginertia="2.7e-06 2.6e-06 8.7e-07"/>
                 <joint name="rh_RFJ2" class="middle_distal"/>
                 <geom class="plastic_visual" mesh="f_middle"/>
-                <geom size="0.009 0.0125" pos="0 0 0.0125" type="capsule" class="plastic_collision" contype="1"/>
+                <geom size="0.009 0.0125" pos="0 0 0.0125" type="capsule" class="plastic_collision"/>
                 <body name="rh_rfdistal" pos="0 0 0.025">
                   <inertial mass="0.013" pos="0 0 0.0130769" quat="1 0 0 1" diaginertia="1.28092e-06 1.12092e-06 5.3e-07"/>
                   <joint name="rh_RFJ1" class="middle_distal"/>
                   <geom class="plastic_visual" mesh="f_distal_pst"/>
-                  <geom class="plastic_collision" type="mesh" mesh="f_distal_pst"/>
+                  <geom class="plastic_collision" type="mesh" mesh="f_distal_pst_214" contype="0" conaffinity="2"/>
                 </body>
               </body>
             </body>
           </body>
           <body name="rh_lfmetacarpal" pos="-0.033 0 0.02071">
             <inertial mass="0.03" pos="0 0 0.04" quat="1 0 0 1" diaginertia="1.638e-05 1.45e-05 4.272e-06"/>
             <joint name="rh_LFJ5" class="metacarpal"/>
             <geom class="plastic_visual" mesh="lf_metacarpal"/>
             <geom size="0.011 0.012 0.025" pos="0.002 0 0.033" type="box" class="plastic_collision"/>
             <body name="rh_lfknuckle" pos="0 0 0.06579">
               <inertial mass="0.008" pos="0 0 0" quat="0.5 0.5 -0.5 0.5" diaginertia="3.2e-07 2.6e-07 2.6e-07"/>
               <joint name="rh_LFJ4" class="knuckle" axis="0 1 0"/>
               <geom pos="0 0 0.0005" class="plastic_visual" mesh="f_knuckle" material="metallic"/>
-              <geom size="0.009 0.009" quat="1 0 1 0" type="cylinder" class="plastic_collision" conaffinity="0"/>
+              <geom size="0.009 0.009" quat="1 0 1 0" type="cylinder" class="plastic_collision" conaffinity="0" contype="0"/>
               <body name="rh_lfproximal">
                 <inertial mass="0.03" pos="0 0 0.0225" quat="1 0 0 1" diaginertia="1e-05 9.8e-06 1.8e-06"/>
                 <joint name="rh_LFJ3" class="proximal"/>
                 <geom class="plastic_visual" mesh="f_proximal"/>
-                <geom size="0.009 0.02" pos="0 0 0.025" type="capsule" class="plastic_collision" contype="1"/>
+                <geom size="0.009 0.02" pos="0 0 0.025" type="capsule" class="plastic_collision"/>
                 <body name="rh_lfmiddle" pos="0 0 0.045">
                   <inertial mass="0.017" pos="0 0 0.0125" quat="1 0 0 1" diaginertia="2.7e-06 2.6e-06 8.7e-07"/>
                   <joint name="rh_LFJ2" class="middle_distal"/>
                   <geom class="plastic_visual" mesh="f_middle"/>
-                  <geom size="0.009 0.0125" pos="0 0 0.0125" type="capsule" class="plastic_collision" contype="1"/>
+                  <geom size="0.009 0.0125" pos="0 0 0.0125" type="capsule" class="plastic_collision"/>
                   <body name="rh_lfdistal" pos="0 0 0.025">
                     <inertial mass="0.013" pos="0 0 0.0130769" quat="1 0 0 1" diaginertia="1.28092e-06 1.12092e-06 5.3e-07"/>
                     <joint name="rh_LFJ1" class="middle_distal"/>
                     <geom class="plastic_visual" mesh="f_distal_pst"/>
-                    <geom class="plastic_collision" type="mesh" mesh="f_distal_pst"/>
+                    <geom class="plastic_collision" type="mesh" mesh="f_distal_pst_214" contype="0" conaffinity="2"/>
                   </body>
                 </body>
               </body>
             </body>
           </body>
           <body name="rh_thbase" pos="0.034 -0.00858 0.029" quat="0.92388 0 0.382683 0">
             <inertial mass="0.01" pos="0 0 0" diaginertia="1.6e-07 1.6e-07 1.6e-07"/>
             <joint name="rh_THJ5" class="thbase"/>
             <geom class="plastic_collision" size="0.013"/>
             <body name="rh_thproximal">
               <inertial mass="0.04" pos="0 0 0.019" diaginertia="1.36e-05 1.36e-05 3.13e-06"/>
               <joint name="rh_THJ4" class="thproximal"/>
               <geom class="plastic_visual" mesh="th_proximal"/>
-              <geom class="plastic_collision" size="0.0105 0.009" pos="0 0 0.02" type="capsule" contype="1"/>
+              <geom class="plastic_collision" size="0.0105 0.009" pos="0 0 0.02" type="capsule"/>
               <body name="rh_thhub" pos="0 0 0.038">
                 <inertial mass="0.005" pos="0 0 0" diaginertia="1e-06 1e-06 3e-07"/>
                 <joint name="rh_THJ3" class="thhub"/>
-                <geom size="0.011" class="plastic_collision" contype="1"/>
+                <geom size="0.011" class="plastic_collision"/>
                 <body name="rh_thmiddle">
                   <inertial mass="0.02" pos="0 0 0.016" diaginertia="5.1e-06 5.1e-06 1.21e-06"/>
                   <joint name="rh_THJ2" class="thmiddle"/>
                   <geom class="plastic_visual" mesh="th_middle"/>
-                  <geom size="0.009 0.009" pos="0 0 0.012" type="capsule" class="plastic_collision" contype="1"/>
+                  <geom size="0.009 0.009" pos="0 0 0.012" type="capsule" class="plastic_collision"/>
                   <geom size="0.01" pos="0 0 0.03" class="plastic_collision"/>
                   <body name="rh_thdistal" pos="0 0 0.032" quat="1 0 0 -1">
                     <inertial mass="0.017" pos="0 0 0.0145588" quat="1 0 0 1" diaginertia="2.37794e-06 2.27794e-06 1e-06"/>
                     <joint name="rh_THJ1" class="thdistal"/>
                     <geom class="plastic_visual" mesh="th_distal_pst"/>
-                    <geom class="plastic_collision" type="mesh" mesh="th_distal_pst"/>
+                    <geom class="plastic_collision" type="mesh" mesh="th_distal_pst_190" contype="0" conaffinity="2"/>
                   </body>
                 </body>
               </body>
             </body>
           </body>
         </body>
       </body>
```

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/scene_right.xml` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/scene_right.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/test_data/shadow_hand/shadow_hand.png` & `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/shadow_hand.png`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.3/mujoco/mjx/viewer.py` & `mujoco-mjx-3.1.4/mujoco/mjx/viewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,14 @@
   elapsed = time.time() - start
   print(f'Compilation took {elapsed}s.')
 
   with mujoco.viewer.launch_passive(m, d) as v:
     while True:
       start = time.time()
 
-      # TODO(robotics-simulation): debug xfrc_applied sometimes causing NaN
       # TODO(robotics-simulation): recompile when changing disable flags, etc.
       dx = dx.replace(ctrl=d.ctrl, xfrc_applied=d.xfrc_applied)
       dx = dx.replace(qpos=d.qpos, qvel=d.qvel, time=d.time)  # handle resets
       mx = mx.tree_replace({
           'opt.gravity': m.opt.gravity,
           'opt.tolerance': m.opt.tolerance,
           'opt.ls_tolerance': m.opt.ls_tolerance,
```

### Comparing `mujoco-mjx-3.1.3/mujoco_mjx.egg-info/PKG-INFO` & `mujoco-mjx-3.1.4/mujoco_mjx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mujoco-mjx
-Version: 3.1.3
+Version: 3.1.4
 Summary: MuJoCo XLA (MJX)
 Author-email: Google DeepMind <mujoco@deepmind.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/google-deepmind/mujoco/tree/main/mjx
-Project-URL: Documentation, https://mujoco.readthedocs.io/en/3.1.3
+Project-URL: Documentation, https://mujoco.readthedocs.io/en/3.1.4
 Project-URL: Repository, https://github.com/google-deepmind/mujoco/tree/main/mjx
-Project-URL: Changelog, https://mujoco.readthedocs.io/en/3.1.3/changelog.html
+Project-URL: Changelog, https://mujoco.readthedocs.io/en/3.1.4/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -23,15 +23,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: absl-py
 Requires-Dist: etils[epath]
 Requires-Dist: jax
 Requires-Dist: jaxlib
-Requires-Dist: mujoco>=3.1.3.dev0
+Requires-Dist: mujoco>=3.1.4.dev0
 Requires-Dist: scipy
 Requires-Dist: trimesh
 
 # MuJoCo XLA (MJX)
 
 [![PyPI Python Version][pypi-versions-badge]][pypi]
 [![PyPI version][pypi-badge]][pypi]
```

### Comparing `mujoco-mjx-3.1.3/mujoco_mjx.egg-info/SOURCES.txt` & `mujoco-mjx-3.1.4/mujoco_mjx.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 mujoco/mjx/viewer.py
 mujoco/mjx/_src/__init__.py
 mujoco/mjx/_src/collision_base.py
 mujoco/mjx/_src/collision_convex.py
 mujoco/mjx/_src/collision_driver.py
 mujoco/mjx/_src/collision_driver_test.py
 mujoco/mjx/_src/collision_primitive.py
+mujoco/mjx/_src/collision_sdf.py
 mujoco/mjx/_src/constraint.py
 mujoco/mjx/_src/constraint_test.py
 mujoco/mjx/_src/dataclasses.py
 mujoco/mjx/_src/device.py
 mujoco/mjx/_src/device_test.py
 mujoco/mjx/_src/forward.py
 mujoco/mjx/_src/forward_test.py
@@ -57,35 +58,47 @@
 mujoco/mjx/test_data/barkour_v0/assets/powercable.stl
 mujoco/mjx/test_data/barkour_v0/assets/upper_left_1.stl
 mujoco/mjx/test_data/barkour_v0/assets/upper_left_2.stl
 mujoco/mjx/test_data/barkour_v0/assets/upper_left_3.stl
 mujoco/mjx/test_data/barkour_v0/assets/upper_right_1.stl
 mujoco/mjx/test_data/barkour_v0/assets/upper_right_2.stl
 mujoco/mjx/test_data/barkour_v0/assets/upper_right_3.stl
+mujoco/mjx/test_data/humanoid/01_humanoids.xml
+mujoco/mjx/test_data/humanoid/02_humanoids.xml
+mujoco/mjx/test_data/humanoid/03_humanoids.xml
+mujoco/mjx/test_data/humanoid/04_humanoids.xml
+mujoco/mjx/test_data/humanoid/05_humanoids.xml
+mujoco/mjx/test_data/humanoid/06_humanoids.xml
+mujoco/mjx/test_data/humanoid/07_humanoids.xml
+mujoco/mjx/test_data/humanoid/08_humanoids.xml
+mujoco/mjx/test_data/humanoid/09_humanoids.xml
+mujoco/mjx/test_data/humanoid/10_humanoids.xml
 mujoco/mjx/test_data/humanoid/README.md
 mujoco/mjx/test_data/humanoid/humanoid.png
 mujoco/mjx/test_data/humanoid/humanoid.xml
 mujoco/mjx/test_data/meshes/dodecahedron.stl
 mujoco/mjx/test_data/meshes/pyramid.stl
 mujoco/mjx/test_data/meshes/tetrahedron.stl
 mujoco/mjx/test_data/shadow_hand/README.md
 mujoco/mjx/test_data/shadow_hand/right_hand.xml
 mujoco/mjx/test_data/shadow_hand/scene_right.xml
 mujoco/mjx/test_data/shadow_hand/shadow_hand.png
 mujoco/mjx/test_data/shadow_hand/assets/f_distal_pst.obj
+mujoco/mjx/test_data/shadow_hand/assets/f_distal_pst_214.obj
 mujoco/mjx/test_data/shadow_hand/assets/f_knuckle.obj
 mujoco/mjx/test_data/shadow_hand/assets/f_middle.obj
 mujoco/mjx/test_data/shadow_hand/assets/f_proximal.obj
 mujoco/mjx/test_data/shadow_hand/assets/forearm_0.obj
 mujoco/mjx/test_data/shadow_hand/assets/forearm_1.obj
 mujoco/mjx/test_data/shadow_hand/assets/forearm_collision.obj
 mujoco/mjx/test_data/shadow_hand/assets/lf_metacarpal.obj
 mujoco/mjx/test_data/shadow_hand/assets/mounting_plate.obj
 mujoco/mjx/test_data/shadow_hand/assets/palm.obj
 mujoco/mjx/test_data/shadow_hand/assets/th_distal_pst.obj
+mujoco/mjx/test_data/shadow_hand/assets/th_distal_pst_190.obj
 mujoco/mjx/test_data/shadow_hand/assets/th_middle.obj
 mujoco/mjx/test_data/shadow_hand/assets/th_proximal.obj
 mujoco/mjx/test_data/shadow_hand/assets/wrist.obj
 mujoco_mjx.egg-info/PKG-INFO
 mujoco_mjx.egg-info/SOURCES.txt
 mujoco_mjx.egg-info/dependency_links.txt
 mujoco_mjx.egg-info/entry_points.txt
```

### Comparing `mujoco-mjx-3.1.3/pyproject.toml` & `mujoco-mjx-3.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="mujoco-mjx"
-version = "3.1.3"
+version = "3.1.4"
 authors = [
     {name = "Google DeepMind", email = "mujoco@deepmind.com"},
 ]
 description = "MuJoCo XLA (MJX)"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {text = "Apache License 2.0"}
 classifiers = [
@@ -27,21 +27,21 @@
 ]
 requires-python = ">=3.8"
 dependencies = [
     "absl-py",
     "etils[epath]",
     "jax",
     "jaxlib",
-    "mujoco>=3.1.3.dev0",
+    "mujoco>=3.1.4.dev0",
     "scipy",
     "trimesh",
 ]
 
 [project.scripts]
 mjx-testspeed = "mujoco.mjx.testspeed:main"
 mjx-viewer = "mujoco.mjx.viewer:main"
 
 [project.urls]
 Homepage = "https://github.com/google-deepmind/mujoco/tree/main/mjx"
-Documentation = "https://mujoco.readthedocs.io/en/3.1.3"
+Documentation = "https://mujoco.readthedocs.io/en/3.1.4"
 Repository = "https://github.com/google-deepmind/mujoco/tree/main/mjx"
-Changelog = "https://mujoco.readthedocs.io/en/3.1.3/changelog.html"
+Changelog = "https://mujoco.readthedocs.io/en/3.1.4/changelog.html"
```

