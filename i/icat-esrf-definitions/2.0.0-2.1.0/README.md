# Comparing `tmp/icat-esrf-definitions-2.0.0.tar.gz` & `tmp/icat-esrf-definitions-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icat-esrf-definitions-2.0.0.tar", last modified: Wed Mar 27 17:37:49 2024, max compression
+gzip compressed data, was "icat-esrf-definitions-2.1.0.tar", last modified: Wed Apr 10 19:25:02 2024, max compression
```

## Comparing `icat-esrf-definitions-2.0.0.tar` & `icat-esrf-definitions-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 17:37:49.691550 icat-esrf-definitions-2.0.0/
--rw-r--r--   0 root         (0) root         (0)     6362 2024-03-27 17:37:49.691550 icat-esrf-definitions-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5691 2024-03-27 17:36:34.000000 icat-esrf-definitions-2.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-03-27 17:36:34.000000 icat-esrf-definitions-2.0.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      946 2024-03-27 17:37:49.691550 icat-esrf-definitions-2.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-27 17:36:34.000000 icat-esrf-definitions-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 17:37:49.691550 icat-esrf-definitions-2.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 17:37:49.691550 icat-esrf-definitions-2.0.0/src/icat_esrf_definitions/
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-27 17:36:34.000000 icat-esrf-definitions-2.0.0/src/icat_esrf_definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)   134886 2024-03-27 17:37:40.000000 icat-esrf-definitions-2.0.0/src/icat_esrf_definitions/hdf5_cfg.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 17:37:49.691550 icat-esrf-definitions-2.0.0/src/icat_esrf_definitions.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6362 2024-03-27 17:37:49.000000 icat-esrf-definitions-2.0.0/src/icat_esrf_definitions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      364 2024-03-27 17:37:49.000000 icat-esrf-definitions-2.0.0/src/icat_esrf_definitions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 17:37:49.000000 icat-esrf-definitions-2.0.0/src/icat_esrf_definitions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-03-27 17:37:49.000000 icat-esrf-definitions-2.0.0/src/icat_esrf_definitions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-27 17:37:49.000000 icat-esrf-definitions-2.0.0/src/icat_esrf_definitions.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:25:02.364925 icat-esrf-definitions-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)     6362 2024-04-10 19:25:02.364925 icat-esrf-definitions-2.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5691 2024-04-10 11:48:26.000000 icat-esrf-definitions-2.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-10 11:48:26.000000 icat-esrf-definitions-2.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-04-10 19:25:02.364925 icat-esrf-definitions-2.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-04-10 11:48:26.000000 icat-esrf-definitions-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:25:02.360925 icat-esrf-definitions-2.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:25:02.360925 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-10 19:25:00.000000 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   137625 2024-04-10 19:20:41.000000 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions/hdf5_cfg.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:25:02.364925 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6362 2024-04-10 19:25:02.000000 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      364 2024-04-10 19:25:02.000000 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 19:25:02.000000 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-10 19:25:02.000000 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-10 19:25:02.000000 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions.egg-info/top_level.txt
```

### Comparing `icat-esrf-definitions-2.0.0/PKG-INFO` & `icat-esrf-definitions-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icat-esrf-definitions
-Version: 2.0.0
+Version: 2.1.0
 Summary: ESRF ICAT definitions
 Home-page: https://gitlab.esrf.fr/icat/hdf5-master-config/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/icat/hdf5-master-config/
 Project-URL: Documentation, https://gitlab.esrf.fr/icat/hdf5-master-config/
```

### Comparing `icat-esrf-definitions-2.0.0/README.md` & `icat-esrf-definitions-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `icat-esrf-definitions-2.0.0/setup.cfg` & `icat-esrf-definitions-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `icat-esrf-definitions-2.0.0/src/icat_esrf_definitions/hdf5_cfg.xml` & `icat-esrf-definitions-2.1.0/src/icat_esrf_definitions/hdf5_cfg.xml`

 * *Files 0% similar despite different names*

#### Comparing `icat-esrf-definitions-2.0.0/src/icat_esrf_definitions/hdf5_cfg.xml` & `icat-esrf-definitions-2.1.0/src/icat_esrf_definitions/hdf5_cfg.xml`

```diff
@@ -557,14 +557,30 @@
       <distance ESRF_description="Effective distance from sample Distance as seen by radiation from sample. This number should be negative to signify that it is upstream of the sample." NAPItype="NX_CHAR">${InstrumentSource_distance}</distance>
       <name ESRF_description="Name of source" NAPItype="NX_CHAR">${InstrumentSource_name}</name>
       <type ESRF_description="type of radiation source (pick one from the enumerated list and spell exactly). Spallation Neutron Source, Pulsed Reactor Neutron Source, Reactor Neutron Source, Synchrotron X-ray Source, Pulsed Muon Source, Rotating Anode X-ray,Fixed Tube X-ray,UV Laser,Free-Electron Laser,Optical Laser,Ion Source,UV Plasma Source" NAPItype="NX_CHAR">${InstrumentSource_type}</type>
       <probe ESRF_description="type of radiation probe" NAPItype="NX_CHAR">${InstrumentSource_probe}</probe>
       <emittance_x ESRF_description="Source emittance (nm-rad) in X (horizontal) direction." NAPItype="NX_CHAR">${InstrumentSource_emittance_x}</emittance_x>
       <emittance_y ESRF_description="Source emittance (nm-rad) in Y (horizontal) direction." NAPItype="NX_CHAR">${InstrumentSource_emittance_y}</emittance_y>
     </group>
+    <group NX_class="NXsource" groupName="laser01">
+      <name ESRF_description="https://manual.nexusformat.org/classes/base_classes/NXsource.html#nxsource-name-field" NAPItype="NX_CHAR">${InstrumentLaser01_name}</name>
+      <type ESRF_description="Type of source. https://manual.nexusformat.org/classes/base_classes/NXsource.html#nxsource-type-field" NAPItype="NX_CHAR">${InstrumentLaser01_type}</type>
+      <probe ESRF_description="Type of radiation. https://manual.nexusformat.org/classes/base_classes/NXsource.html#nxsource-probe-field" NAPItype="NX_CHAR">${InstrumentLaser01_probe}</probe>
+      <energy ESRF_description="Energy emitted in a single pulse. https://manual.nexusformat.org/classes/base_classes/NXsource.html#nxsource-energy-field" NAPItype="NX_FLOAT" units="J">${InstrumentLaser01_energy}</energy>
+      <pulse_width ESRF_description="Time between the start and end of a single pulse. https://manual.nexusformat.org/classes/base_classes/NXsource.html#nxsource-pulse-width-field" NAPItype="NX_FLOAT" units="s">${InstrumentLaser01_pulse_width}</pulse_width>
+      <delay ESRF_description="The time of the start of the laser pulse with respect to the start of the measurement (T=0)" NAPItype="NX_FLOAT" units="s">${InstrumentLaser01_delay}</delay>
+    </group>
+    <group NX_class="NXsource" groupName="laser02">
+      <name ESRF_description="https://manual.nexusformat.org/classes/base_classes/NXsource.html#nxsource-name-field" NAPItype="NX_CHAR">${InstrumentLaser02_name}</name>
+      <type ESRF_description="Type of source. https://manual.nexusformat.org/classes/base_classes/NXsource.html#nxsource-type-field" NAPItype="NX_CHAR">${InstrumentLaser02_type}</type>
+      <probe ESRF_description="Type of radiation. https://manual.nexusformat.org/classes/base_classes/NXsource.html#nxsource-probe-field" NAPItype="NX_CHAR">${InstrumentLaser02_probe}</probe>
+      <energy ESRF_description="Energy emitted in a single pulse. https://manual.nexusformat.org/classes/base_classes/NXsource.html#nxsource-energy-field" NAPItype="NX_FLOAT" units="J">${InstrumentLaser02_energy}</energy>
+      <pulse_width ESRF_description="Time between the start and end of a single pulse. https://manual.nexusformat.org/classes/base_classes/NXsource.html#nxsource-pulse-width-field" NAPItype="NX_FLOAT" units="s">${InstrumentLaser02_pulse_width}</pulse_width>
+      <delay ESRF_description="The time of the start of the laser pulse with respect to the start of the measurement (T=0)" NAPItype="NX_FLOAT" units="s">${InstrumentLaser02_delay}</delay>
+    </group>
     <group NX_class="NXslit" groupName="primary_slit">
       <name NAPItype="NX_CHAR">${InstrumentSlitPrimary_name}</name>
       <vertical_gap NAPItype="NX_CHAR">${InstrumentSlitPrimary_vertical_gap}</vertical_gap>
       <vertical_offset NAPItype="NX_CHAR">${InstrumentSlitPrimary_vertical_offset}</vertical_offset>
       <horizontal_gap NAPItype="NX_CHAR">${InstrumentSlitPrimary_horizontal_gap}</horizontal_gap>
       <horizontal_offset NAPItype="NX_CHAR">${InstrumentSlitPrimary_horizontal_offset}</horizontal_offset>
       <blade_up NAPItype="NX_CHAR">${InstrumentSlitPrimary_blade_up}</blade_up>
@@ -1222,14 +1238,15 @@
   <group NX_class="NXprocess" groupName="workflow">
     <name NAPItype="NX_CHAR">${Workflow_name}</name>
     <id NAPItype="NX_CHAR">${Workflow_id}</id>
     <type NAPItype="NX_CHAR">${Workflow_type}</type>
     <status NAPItype="NX_CHAR">${Workflow_status}</status>
   </group>
   <group NX_class="NXnote" groupName="external_references">
+    <neuroglancer NAPItype="NX_CHAR">${ExternalReferences_neuroglancer}</neuroglancer>
     <group NX_class="NXCite" groupName="publication">
       <doi NAPItype="NX_CHAR">${ExternalReferencesPublication_doi}</doi>
       <endnote NAPItype="NX_CHAR">${ExternalReferencesPublication_endnote}</endnote>
     </group>
     <group NX_class="NXCite" groupName="datacollector">
       <endnote NAPItype="NX_CHAR">${ExternalReferencesDatacollector_endnote}</endnote>
     </group>
```

### Comparing `icat-esrf-definitions-2.0.0/src/icat_esrf_definitions.egg-info/PKG-INFO` & `icat-esrf-definitions-2.1.0/src/icat_esrf_definitions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icat-esrf-definitions
-Version: 2.0.0
+Version: 2.1.0
 Summary: ESRF ICAT definitions
 Home-page: https://gitlab.esrf.fr/icat/hdf5-master-config/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/icat/hdf5-master-config/
 Project-URL: Documentation, https://gitlab.esrf.fr/icat/hdf5-master-config/
```

