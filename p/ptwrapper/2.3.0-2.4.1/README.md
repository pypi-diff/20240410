# Comparing `tmp/ptwrapper-2.3.0-py3-none-any.whl.zip` & `tmp/ptwrapper-2.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 98007 bytes, number of entries: 34
+Zip file size: 98365 bytes, number of entries: 34
 -rw-r--r--  2.0 unx       70 b- defN 80-Jan-01 00:00 ptwrapper/.flake8
 -rw-r--r--  2.0 unx      105 b- defN 80-Jan-01 00:00 ptwrapper/__init__.py
--rw-r--r--  2.0 unx     9169 b- defN 80-Jan-01 00:00 ptwrapper/cli.py
--rw-r--r--  2.0 unx    37103 b- defN 80-Jan-01 00:00 ptwrapper/config/age/cfg_agm_jui_multibody.xml
--rwxr-xr-x  2.0 unx      526 b- defN 80-Jan-01 00:00 ptwrapper/config/age/cfg_agm_jui_multibody_event_definitions.xml
--rwxr-xr-x  2.0 unx    22766 b- defN 80-Jan-01 00:00 ptwrapper/config/age/cfg_agm_jui_multibody_fixed_definitions.xml
+-rw-r--r--  2.0 unx     9266 b- defN 80-Jan-01 00:00 ptwrapper/cli.py
+-rw-r--r--  2.0 unx    40099 b- defN 80-Jan-01 00:00 ptwrapper/config/age/cfg_agm_jui_multibody.xml
+-rw-r--r--  2.0 unx      526 b- defN 80-Jan-01 00:00 ptwrapper/config/age/cfg_agm_jui_multibody_event_definitions.xml
+-rw-r--r--  2.0 unx    22766 b- defN 80-Jan-01 00:00 ptwrapper/config/age/cfg_agm_jui_multibody_fixed_definitions.xml
 -rw-r--r--  2.0 unx    10910 b- defN 80-Jan-01 00:00 ptwrapper/config/age/cfg_agm_jui_multibody_predefined_block.xml
 -rw-r--r--  2.0 unx   291598 b- defN 80-Jan-01 00:00 ptwrapper/config/ise/BRF_MAL_SGICD_2_1_300101_351005.brf
 -rw-r--r--  2.0 unx    67932 b- defN 80-Jan-01 00:00 ptwrapper/config/ise/RES_C50_SA_CELLS_EFFICIENCY_310101_351003.csv
 -rw-r--r--  2.0 unx     5204 b- defN 80-Jan-01 00:00 ptwrapper/config/ise/eps.cfg
 -rw-r--r--  2.0 unx    76839 b- defN 80-Jan-01 00:00 ptwrapper/config/ise/events.juice.def
 -rw-r--r--  2.0 unx       59 b- defN 80-Jan-01 00:00 ptwrapper/config/ise/phs_com_res_sa_cells_count.asc
 -rw-r--r--  2.0 unx     7011 b- defN 80-Jan-01 00:00 ptwrapper/config/ise/units.def
@@ -24,13 +24,13 @@
 -rw-r--r--  2.0 unx      357 b- defN 80-Jan-01 00:00 ptwrapper/input/edf/juice__spacecraft_ssmm.edf
 -rw-r--r--  2.0 unx   930286 b- defN 80-Jan-01 00:00 ptwrapper/input/itl/TBD.itl
 -rw-r--r--  2.0 unx      259 b- defN 80-Jan-01 00:00 ptwrapper/input/itl/TOP_timelines.itl
 -rw-r--r--  2.0 unx      970 b- defN 80-Jan-01 00:00 ptwrapper/input/itl/downlink.itl
 -rw-r--r--  2.0 unx    27700 b- defN 80-Jan-01 00:00 ptwrapper/input/itl/platform.itl
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 ptwrapper/py.typed
 -rw-r--r--  2.0 unx     8034 b- defN 80-Jan-01 00:00 ptwrapper/utils.py
--rw-r--r--  2.0 unx    13025 b- defN 80-Jan-01 00:00 ptwrapper-2.3.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     8774 b- defN 80-Jan-01 00:00 ptwrapper-2.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ptwrapper-2.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 ptwrapper-2.3.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     3153 b- defN 16-Jan-01 00:00 ptwrapper-2.3.0.dist-info/RECORD
-34 files, 1529883 bytes uncompressed, 92839 bytes compressed:  93.9%
+-rw-r--r--  2.0 unx    13025 b- defN 80-Jan-01 00:00 ptwrapper-2.4.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     8774 b- defN 80-Jan-01 00:00 ptwrapper-2.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ptwrapper-2.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 ptwrapper-2.4.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     3153 b- defN 16-Jan-01 00:00 ptwrapper-2.4.1.dist-info/RECORD
+34 files, 1532976 bytes uncompressed, 93197 bytes compressed:  93.9%
```

## zipnote {}

```diff
@@ -81,23 +81,23 @@
 
 Filename: ptwrapper/py.typed
 Comment: 
 
 Filename: ptwrapper/utils.py
 Comment: 
 
-Filename: ptwrapper-2.3.0.dist-info/LICENSE.txt
+Filename: ptwrapper-2.4.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: ptwrapper-2.3.0.dist-info/METADATA
+Filename: ptwrapper-2.4.1.dist-info/METADATA
 Comment: 
 
-Filename: ptwrapper-2.3.0.dist-info/WHEEL
+Filename: ptwrapper-2.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: ptwrapper-2.3.0.dist-info/entry_points.txt
+Filename: ptwrapper-2.4.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ptwrapper-2.3.0.dist-info/RECORD
+Filename: ptwrapper-2.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ptwrapper/cli.py

```diff
@@ -148,29 +148,29 @@
                 sh.move(mga_bc_path, os.path.join(output_dir, f'juice_mga_{fname}.bc'))
                 sh.move(os.path.join(root_scenario_path, 'output', 'juice_mga_ptr.csv'),
                         os.path.join(output_dir, f'juice_mga_{fname}.csv'))
             else:
                 print(f'MGA CSV and CK files not generated.')
 
         if not args.no_power:
-            print(f'Renaming power.csv to {fname}_power.csv')
+            print(f'Renaming power.csv to {fname.lower()}_v01_power.csv')
             sh.move(os.path.join(root_scenario_path, 'output', 'power.csv'),
-                    os.path.join(output_dir, f'{fname}_power.csv'))
+                    os.path.join(output_dir, f'{fname.lower()}_v01_power.csv'))
 
-        print(f'Renaming ptr_resolved.ptx to {fname}_resolved.ptx')
+        print(f'Renaming ptr_resolved.ptx to {fname.lower()}_v01_resolved.ptx')
         sh.move(os.path.join(root_scenario_path, 'output', 'ptr_resolved.ptx'),
-                os.path.join(output_dir, f'{fname}_resolved.ptx'))
+                os.path.join(output_dir, f'{fname.lower()}_v01_resolved.ptx'))
 
-        print(f'Renaming juice_sc_ptr.bc to {fname}.bc')
+        print(f'Renaming juice_sc_ptr.bc to juice_sc_{fname.lower()}_v01.bc')
         sh.move(os.path.join(root_scenario_path, 'output', 'juice_sc_ptr.bc'),
-                os.path.join(output_dir, f'juice_sc_{fname}.bc'))
+                os.path.join(output_dir, f'juice_sc_{fname.lower()}_v01.bc'))
 
-        print(f'Renaming log.json to {fname}_log.json')
+        print(f'Renaming log.json to {fname.lower()}_log.json')
         sh.move(os.path.join(root_scenario_path, 'output', 'log.json'),
-                os.path.join(output_dir, f'{fname}_log.json'))
+                os.path.join(output_dir, f'{fname.lower()}_log.json'))
 
         print('Cleaning up OSVE execution files and directories')
         os.remove(os.path.join(root_scenario_path, 'input', 'PTR_PT_V1.ptx'))
         os.remove(os.path.join(root_scenario_path, 'input', 'downlink.evf'))
         os.remove(os.path.join(root_scenario_path, 'input', 'TOP_events.evf'))
         sh.rmtree(os.path.join(root_scenario_path, 'input', 'edf'))
         sh.rmtree(os.path.join(root_scenario_path, 'input', 'itl'))
```

## ptwrapper/config/age/cfg_agm_jui_multibody.xml

### ptwrapper/config/age/cfg_agm_jui_multibody.xml

```diff
@@ -39,14 +39,15 @@
     <Param id="SE_MARGINPERCENT" type="PT_DOUBLE" description="Margin to be applied on the estimated slew duration. This is the percentage value that the estimated duration is extended to increase feasibility beyond the slew checker results." unit="%">10.0</Param>
     <Param id="SE_MARGINDELTA" type="PT_DOUBLE" description="Extra time to be added on the estimated slew duration. This is the amount of time that the estimated duration is further extended after being scaled by the percentage provided by SE_MARGINPERCENT." unit="s">0.0</Param>
     <Param id="SE_REPORT_SLEW_SOLUTION" type="PT_BOOL" description="Flag to indicate whether if slew solutions (before/after) should be reported to the user in order to void attitude constraint breaks (for example, momentum, torque, etc.).. Default is False." unit="False/True">true</Param>
     <Param id="SE_SLEW_SOLUTION_ACCURACY" type="PT_DOUBLE" description="Indicates the time accuracy in seconds at which the algorithm should stop looking for a solution. 1 minute could be a reasonable time accuracy. The higher the accuracy the longer the time the algorithm will try to find a solution, and therefore, it has an impact in the performance." unit="s">60.0</Param>
     <!-- Attitude generation algorithms -->
     <Param id="AG_DURATIONMIN" type="PT_DOUBLE" description="Minimum block duration allowed." unit="s">60.0</Param>
     <Param id="AG_PROFILETIMESTEP" type="PT_DOUBLE" description="Time step for the attitude profile generation." unit="s">1.0</Param>
+    <Param id="AG_GENCKDATATYPE" type="PT_STRING" description="Indicates AGM to generate CK Type 5 (CK5) or Type 6 (CK6) kernels. The default value is CK6." unit="">CK6</Param>
     <Param id="AG_SETTLINGTIMEBEFORE" type="PT_DOUBLE" description="Settling time at the start of a science pointing block." unit="s">0.0</Param>
     <Param id="AG_SETTLINGTIMEAFTER" type="PT_DOUBLE" description="Settling time at the end of a science pointing block, used only for visualization." unit="s">60.0</Param>
     <Param id="AG_COMPSETTLINGTIMEBEFORE" type="PT_DOUBLE" description="Settling time or Tranquilization time at the start of each composite internal science pointing slot (only used for visualization purpose)." unit="s">0.0</Param>
     <Param id="AG_COMPSETTLINGTIMEAFTER" type="PT_DOUBLE" description="Settling time at the end of each composite internal science pointing slot (only used for visualization purposes)." unit="s">60.0</Param>
     <Param id="AG_GAPDURATIONMIN" type="PT_DOUBLE" description="Minimum gap duration in timeline to try filling with the default pointing" unit="s">900.0</Param>
     <Param id="AG_FILLGAPSSTARTANDEND" type="PT_BOOL" description="Add default pointing if there is no pointing request between the scenario start time and the first block and the last block and the end of the scenario." unit="False/True">true</Param>
     <Param id="AG_MERGEBLOCKSWITHDEFAULTBLOCK" type="PT_BOOL" description="Flag to merge blocks with the default block" unit="False/True">true</Param>
@@ -185,90 +186,105 @@
     <Object parserName="Uranus" mnemonic="URANUS" spiceName="URANUS BARYCENTER" isBody="true" bufferPos="false" bufferPosTimeStep="600.0" bufferVel="false" bufferVelTimeStep="1200.0" gravity="0" orbitingName="Sun"/>
     <Object parserName="Neptune" mnemonic="NEPTUNE" spiceName="NEPTUNE BARYCENTER" isBody="true" bufferPos="false" bufferPosTimeStep="600.0" bufferVel="false" bufferVelTimeStep="1200.0" gravity="0" orbitingName="Sun"/>
     <Object parserName="Pluto" mnemonic="PLUTO" spiceName="PLUTO BARYCENTER" isBody="true" bufferPos="false" bufferPosTimeStep="600.0" bufferVel="false" bufferVelTimeStep="1200.0" gravity="0" orbitingName="Sun"/>
     <Object parserName="Jupiter" mnemonic="JUPITER" spiceName="JUPITER" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="1.2668653499E+17" orbitingName="Sun" isTargetObj="true" isReferenceObj="true"/>
     <Object parserName="Callisto" mnemonic="CALLISTO" spiceName="CALLISTO" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="7.1808100000E+12" orbitingName="Jupiter"/>
     <Object parserName="Europa" mnemonic="EUROPA" spiceName="EUROPA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="3.2034200000E+12" orbitingName="Jupiter"/>
     <Object parserName="Ganymede" mnemonic="GANYMEDE" spiceName="GANYMEDE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="9.8878300000E+12" orbitingName="Jupiter"/>
-    <Object parserName="Adrastea" mnemonic="ADRASTEA" spiceName="ADRASTEA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Aitne" mnemonic="AITNE" spiceName="AITNE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Io" mnemonic="IO" spiceName="IP" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
     <Object parserName="Amalthea" mnemonic="AMALTHEA" spiceName="AMALTHEA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Thebe" mnemonic="THEBE" spiceName="THEBE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Adrastea" mnemonic="ADRASTEA" spiceName="ADRASTEA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Metis" mnemonic="METIS" spiceName="METIS" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
     <Object parserName="Ananke" mnemonic="ANANKE" spiceName="ANANKE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Aoede" mnemonic="AOEDE" spiceName="AOEDE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Arche" mnemonic="ARCHE" spiceName="ARCHE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Autonoe" mnemonic="AUTONOE" spiceName="AUTONOE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Callirrhoe" mnemonic="CALLIRRHOE" spiceName="CALLIRRHOE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Carme" mnemonic="CARME" spiceName="CARME" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Carpo" mnemonic="CARPO" spiceName="CARPO" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Chaldene" mnemonic="CHALDENE" spiceName="CHALDENE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Cyllene" mnemonic="CYLLENE" spiceName="CYLLENE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Dia" mnemonic="DIA" spiceName="DIA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Eirene" mnemonic="EIRENE" spiceName="EIRENE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Elara" mnemonic="ELARA" spiceName="ELARA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Erinome" mnemonic="ERINOME" spiceName="ERINOME" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Ersa" mnemonic="ERSA" spiceName="ERSA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Euanthe" mnemonic="EUANTHE" spiceName="EUANTHE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Eukelade" mnemonic="EUKELADE" spiceName="EUKELADE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Eupheme" mnemonic="EUPHEME" spiceName="EUPHEME" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Euporie" mnemonic="EUPORIE" spiceName="EUPORIE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Eurydome" mnemonic="EURYDOME" spiceName="EURYDOME" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
     <Object parserName="Harpalyke" mnemonic="HARPALYKE" spiceName="HARPALYKE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Hegemone" mnemonic="HEGEMONE" spiceName="HEGEMONE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Helike" mnemonic="HELIKE" spiceName="HELIKE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Hermippe" mnemonic="HERMIPPE" spiceName="HERMIPPE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Herse" mnemonic="HERSE" spiceName="HERSE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Himalia" mnemonic="HIMALIA" spiceName="HIMALIA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Io" mnemonic="IO" spiceName="IO" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
     <Object parserName="Iocaste" mnemonic="IOCASTE" spiceName="IOCASTE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Isonoe" mnemonic="ISONOE" spiceName="ISONOE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Kale" mnemonic="KALE" spiceName="KALE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Kallichore" mnemonic="KALLICHORE" spiceName="KALLICHORE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Kalyke" mnemonic="KALYKE" spiceName="KALYKE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Kore" mnemonic="KORE" spiceName="KORE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Leda" mnemonic="LEDA" spiceName="LEDA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Lysithea" mnemonic="LYSITHEA" spiceName="LYSITHEA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Megaclite" mnemonic="MEGACLITE" spiceName="MEGACLITE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Metis" mnemonic="METIS" spiceName="METIS" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Mneme" mnemonic="MNEME" spiceName="MNEME" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Orthosie" mnemonic="ORTHOSIE" spiceName="ORTHOSIE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Pandia" mnemonic="PANDIA" spiceName="PANDIA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Pasiphae" mnemonic="PASIPHAE" spiceName="PASIPHAE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Pasithee" mnemonic="PASITHEE" spiceName="PASITHEE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Philophrosyne" mnemonic="PHILOPHROSYNE" spiceName="PHILOPHROSYNE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
     <Object parserName="Praxidike" mnemonic="PRAXIDIKE" spiceName="PRAXIDIKE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Thyone" mnemonic="THYONE" spiceName="THYONE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Hermippe" mnemonic="HERMIPPE" spiceName="HERMIPPE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Euanthe" mnemonic="EUANTHE" spiceName="EUANTHE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Euporie" mnemonic="EUPORIE" spiceName="EUPORIE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Orthosie" mnemonic="ORTHOSIE" spiceName="ORTHOSIE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Mneme" mnemonic="MNEME" spiceName="MNEME" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Thelxinoe" mnemonic="THELXINOE" spiceName="THELXINOE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Helike" mnemonic="HELIKE" spiceName="HELIKE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2010_J2" mnemonic="S2010_J2" spiceName="S2010_J2" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2016_J1" mnemonic="S2016_J1" spiceName="S2016_J1" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2003_J18" mnemonic="S2003_J18" spiceName="S2003_J18" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Eupheme" mnemonic="EUPHEME" spiceName="EUPHEME" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2017_J3" mnemonic="S2017_J3" spiceName="S2017_J3" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2017_J7" mnemonic="S2017_J7" spiceName="S2017_J7" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2017_J9" mnemonic="S2017_J9" spiceName="S2017_J9" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
     <Object parserName="S2003_J2" mnemonic="S2003_J2" spiceName="S2003_J2" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="S2003_J4" mnemonic="S2003_J4" spiceName="S2003_J4" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="S2003_J9" mnemonic="S2003_J9" spiceName="S2003_J9" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="S2003_J10" mnemonic="S2003_J10" spiceName="S2003_J10" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
     <Object parserName="S2003_J12" mnemonic="S2003_J12" spiceName="S2003_J12" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
     <Object parserName="S2003_J16" mnemonic="S2003_J16" spiceName="S2003_J16" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="S2003_J18" mnemonic="S2003_J18" spiceName="S2003_J18" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="S2003_J19" mnemonic="S2003_J19" spiceName="S2003_J19" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="S2003_J23" mnemonic="S2003_J23" spiceName="S2003_J23" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="S2003_J24" mnemonic="S2003_J24" spiceName="S2003_J24" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2021_J1" mnemonic="S2021_J1" spiceName="S2021_J1" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2021_J2" mnemonic="S2021_J2" spiceName="S2021_J2" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2021_J3" mnemonic="S2021_J3" spiceName="S2021_J3" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2022_J3" mnemonic="S2022_J3" spiceName="S2022_J3" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Carme" mnemonic="CARME" spiceName="CARME" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Taygete" mnemonic="TAYGETE" spiceName="TAYGETE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Chaldene" mnemonic="CHALDENE" spiceName="CHALDENE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Kalyke" mnemonic="KALYKE" spiceName="KALYKE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Erinome" mnemonic="ERINOME" spiceName="ERINOME" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Isonoe" mnemonic="ISONOE" spiceName="ISONOE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Aitne" mnemonic="AITNE" spiceName="AITNE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Kale" mnemonic="KALE" spiceName="KALE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Pasithee" mnemonic="PASITHEE" spiceName="PASITHEE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Arche" mnemonic="ARCHE" spiceName="ARCHE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Kallichore" mnemonic="KALLICHORE" spiceName="KALLICHORE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Eukelade" mnemonic="EUKEKADE" spiceName="EUKEKADE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Herse" mnemonic="HERSE" spiceName="HERSE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
     <Object parserName="S2010_J1" mnemonic="S2010_J1" spiceName="S2010_J1" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="S2010_J2" mnemonic="S2010_J2" spiceName="S2010_J2" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="S2011_J1" mnemonic="S2011_J1" spiceName="S2011_J1" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="S2011_J2" mnemonic="S2011_J2" spiceName="S2011_J2" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="S2016_J1" mnemonic="S2016_J1" spiceName="S2016_J1" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="S2017_J1" mnemonic="S2017_J1" spiceName="S2017_J1" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Eirene" mnemonic="EIRENE" spiceName="EIRENE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2003_J19" mnemonic="S2003_J19" spiceName="S2003_J19" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
     <Object parserName="S2017_J2" mnemonic="S2017_J2" spiceName="S2017_J2" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="S2017_J3" mnemonic="S2017_J3" spiceName="S2017_J3" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
     <Object parserName="S2017_J5" mnemonic="S2017_J5" spiceName="S2017_J5" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="S2017_J6" mnemonic="S2017_J6" spiceName="S2017_J6" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="S2017_J7" mnemonic="S2017_J7" spiceName="S2017_J7" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
     <Object parserName="S2017_J8" mnemonic="S2017_J8" spiceName="S2017_J8" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="S2017_J9" mnemonic="S2017_J9" spiceName="S2017_J9" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2011_J1" mnemonic="S2011_J1" spiceName="S2011_J1" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2003_J9" mnemonic="S2003_J9" spiceName="S2003_J9" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2003_J10" mnemonic="S2003_J10" spiceName="S2003_J10" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2003_J24" mnemonic="S2003_J24" spiceName="S2003_J24" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2018_J3" mnemonic="S2018_J3" spiceName="S2018_J3" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2021_J4" mnemonic="S2021_J4" spiceName="S2021_J4" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2021_J5" mnemonic="S2021_J5" spiceName="S2021_J5" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2021_J6" mnemonic="S2021_J6" spiceName="S2021_J6" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2016_J3" mnemonic="S2016_J3" spiceName="S2016_J3" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2022_J1" mnemonic="S2022_J1" spiceName="S2022_J1" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2022_J2" mnemonic="S2022_J2" spiceName="S2022_J2" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Pasiphae" mnemonic="PASIPHAE" spiceName="PASIPHAE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
     <Object parserName="Sinope" mnemonic="SINOPE" spiceName="SINOPE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Callirrhoe" mnemonic="CALLIRRHOE" spiceName="CALLIRRHOE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Megaclite" mnemonic="MEGACLITE" spiceName="MEGACLITE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Autonoe" mnemonic="AUTONOE" spiceName="AUTONOE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Eurydome" mnemonic="EURYDOME" spiceName="EURYDOME" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
     <Object parserName="Sponde" mnemonic="SPONDE" spiceName="SPONDE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Taygete" mnemonic="TAYGETE" spiceName="TAYGETE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Thebe" mnemonic="THEBE" spiceName="THEBE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Thelxinoe" mnemonic="THELXINOE" spiceName="THELXINOE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Hegemone" mnemonic="HEGEMONE" spiceName="HEGEMONE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Aoede" mnemonic="AOEDE" spiceName="AOEDE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Cyllene" mnemonic="CYLLENE" spiceName="CYLLENE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Kore" mnemonic="KORE" spiceName="KORE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2011_J2" mnemonic="S2011_J2" spiceName="S2011_J2" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Philophrosyne" mnemonic="PHILOPHROSYNE" spiceName="PHILOPHROSYNE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2017_J1" mnemonic="S2017_J1" spiceName="S2017_J1" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2017_J6" mnemonic="S2017_J6" spiceName="S2017_J6" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2003_J4" mnemonic="S2003_J4" spiceName="S2003_J4" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2003_J23" mnemonic="S2003_J23" spiceName="S2003_J23" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2016_J4" mnemonic="S2016_J4" spiceName="S2016_J4" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
     <Object parserName="Themisto" mnemonic="THEMISTO" spiceName="THEMISTO" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
-    <Object parserName="Thyone" mnemonic="THYONE" spiceName="THYONE" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Himalia" mnemonic="HIMALIA" spiceName="HIMALIA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Elara" mnemonic="ELARA" spiceName="ELARA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Lysithea" mnemonic="LYSITHEA" spiceName="LYSITHEA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Leda" mnemonic="LEDA" spiceName="LEDA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Dia" mnemonic="DIA" spiceName="DIA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Pandia" mnemonic="PANDIA" spiceName="PANDIA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Ersa" mnemonic="ERSA" spiceName="ERSA" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2011_J3" mnemonic="S2011_J3" spiceName="S2011_J3" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2018_J2" mnemonic="S2018_J2" spiceName="S2018_J2" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="Carpo" mnemonic="CARPO" spiceName="CARPO" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
+    <Object parserName="S2018_J4" mnemonic="S2018_J4" spiceName="S2018_J4" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
     <Object parserName="Valetudo" mnemonic="VALETUDO" spiceName="VALETUDO" isBody="true" bufferPos="true" bufferPosTimeStep="60.0" bufferVel="true" bufferVelTimeStep="60.0" gravity="0"/>
   </Objects>
   <Frames>
     <Frame parserName="EME2000" mnemonic="EME" spiceName="J2000" refFrame="INERTIAL" isDynamic="false" bufferAtt="false" bufferAttTimeStep="0" isReferenceFrame="true"/>
     <Frame parserName="JUPITER" mnemonic="CBE" spiceName="IAU_JUPITER" refFrame="INERTIAL" isDynamic="true" bufferAtt="true" bufferAttTimeStep="120.0"/>
     <Frame parserName="SC" mnemonic="SBF" spiceName="JUICE_SPACECRAFT" refFrame="SPACECRAFT" isDynamic="false" bufferAtt="false" bufferAttTimeStep="0"/>
     <Frame parserName="EUROPA" mnemonic="CBE" spiceName="IAU_EUROPA" refFrame="INERTIAL" isDynamic="true" bufferAtt="false" bufferAttTimeStep="0"/>
```

## Comparing `ptwrapper-2.3.0.dist-info/LICENSE.txt` & `ptwrapper-2.4.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `ptwrapper-2.3.0.dist-info/METADATA` & `ptwrapper-2.4.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptwrapper
-Version: 2.3.0
+Version: 2.4.1
 Summary: A Pointing Tool OSVE wrapper
 Home-page: https://juigitlab.esac.esa.int/core-system/uplink/auxiliary-tools/ptwrapper
 License: European Space Agency Public License (ESA-PL) Permissive (Type 3) – v2.4
 Author: Marc Costa
 Author-email: marc.costa@ext.esa.int
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: osve (>=2.3.0)
+Requires-Dist: osve (>=2.4.1)
 Project-URL: Documentation, https://.github.io/ptwrapper
 Project-URL: Repository, https://juigitlab.esac.esa.int/core-system/uplink/auxiliary-tools/ptwrapper
 Description-Content-Type: text/markdown
 
 # Pointing Tool Wrapper
 
 A JUICE SOC [Pointing Tool](https://juicept.esac.esa.int/) wrapper (`PTwrapper`) for WINDOWS, LINUX, and MACOSX for use in a local computer.
```

## Comparing `ptwrapper-2.3.0.dist-info/RECORD` & `ptwrapper-2.4.1.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ptwrapper/.flake8,sha256=UgR2mYSjvCLP_ER2I0VU3upkJ2Y_B3JwglJGvD15WXU,70
 ptwrapper/__init__.py,sha256=WN_fzmZXIM_pH5hNq3pPbjT4RpikTNws_yHxb_ihF6g,105
-ptwrapper/cli.py,sha256=FkypWf2ue66w4_efrykogYQO7YA-tipwnUXvG7chEJ8,9169
-ptwrapper/config/age/cfg_agm_jui_multibody.xml,sha256=T4zeLtcezm8g4KGeg0mmOFrt8_9q-QtpPpLMh3l696E,37103
+ptwrapper/cli.py,sha256=ZnUQeId3_s29inIwvnc1yuVzOhDrgPJEgoFf8lNB4bQ,9266
+ptwrapper/config/age/cfg_agm_jui_multibody.xml,sha256=5e1s3O5UARC95YPchg33JtDBH8TsT1FC3G1wT3YLLfY,40099
 ptwrapper/config/age/cfg_agm_jui_multibody_event_definitions.xml,sha256=1kSXUl6N9c-on-IRgU6kwHpreOG5SO4RMBEUs3zfaGY,526
 ptwrapper/config/age/cfg_agm_jui_multibody_fixed_definitions.xml,sha256=i50h9wGSHNJYx_MtEBels1C4l2UMy2Ul6otjgxHXgbY,22766
 ptwrapper/config/age/cfg_agm_jui_multibody_predefined_block.xml,sha256=3Z0JSpL00-YamLuKlRx6BDBaFkUcymRajVMkNlO6s4U,10910
 ptwrapper/config/ise/BRF_MAL_SGICD_2_1_300101_351005.brf,sha256=LNx70gN7U9oF0z2uNISOGqmCRMVt250e7Qz7lzFNL9Q,291598
 ptwrapper/config/ise/RES_C50_SA_CELLS_EFFICIENCY_310101_351003.csv,sha256=5mUkNx_FLAeTfyVoV7W6l53Li8kAddTd8MDZEF6c4Io,67932
 ptwrapper/config/ise/eps.cfg,sha256=OgonoOMAQwVY_sYSzeOXzWhDmJk3-Wg1GonlmyGQWi8,5204
 ptwrapper/config/ise/events.juice.def,sha256=UIR4CWxt-wsy4hXSXQrIzw-h4f0bJ0j3sQZZ9rNzQLg,76839
@@ -23,12 +23,12 @@
 ptwrapper/input/edf/juice__spacecraft_ssmm.edf,sha256=wSaVuFvxXHiqvWwuI3pYumn1dkfdsgzzyqbCBK-wGAE,357
 ptwrapper/input/itl/TBD.itl,sha256=37bBrMFjKm-tGUqcvFmXLrQ5mqiC2bZ1RX8h-ljvI6o,930286
 ptwrapper/input/itl/TOP_timelines.itl,sha256=UX-bQ6gHjWMIl-IWGM4wribvMncG-Gdou_sc1fqjrVE,259
 ptwrapper/input/itl/downlink.itl,sha256=-XNnuedKH5o4gSEgkR-O80yONvVYD9_tBgAv31iTGdc,970
 ptwrapper/input/itl/platform.itl,sha256=zRBHvWXaxp52fUq7d9BdARu6Y2rz72goZi-HDWsnSyc,27700
 ptwrapper/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ptwrapper/utils.py,sha256=JdNvuoPrTbWOFMQcASl0PcpO_Mtkk4PEY_CgJpFzGBI,8034
-ptwrapper-2.3.0.dist-info/LICENSE.txt,sha256=cp9o7IsgRfqJDX7sA_QAhNxt9eRAKFUVKP97iKAvYjU,13025
-ptwrapper-2.3.0.dist-info/METADATA,sha256=_bKoSLHr4bM3IbTmiTSVBCQUH3ZYX-M6enMdDSNBVtY,8774
-ptwrapper-2.3.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-ptwrapper-2.3.0.dist-info/entry_points.txt,sha256=KkPDhCD1nMkGrEddcxHN62q-iicBZc8rQ3DIo3jqXks,47
-ptwrapper-2.3.0.dist-info/RECORD,,
+ptwrapper-2.4.1.dist-info/LICENSE.txt,sha256=cp9o7IsgRfqJDX7sA_QAhNxt9eRAKFUVKP97iKAvYjU,13025
+ptwrapper-2.4.1.dist-info/METADATA,sha256=55wPqO1hQaLhABi2Q9JNv_GG76ik3xhcG_1xHSxtxpA,8774
+ptwrapper-2.4.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+ptwrapper-2.4.1.dist-info/entry_points.txt,sha256=KkPDhCD1nMkGrEddcxHN62q-iicBZc8rQ3DIo3jqXks,47
+ptwrapper-2.4.1.dist-info/RECORD,,
```

