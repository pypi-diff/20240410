# Comparing `tmp/rats_apps-0.1.2.dev1-py3-none-any.whl.zip` & `tmp/rats_apps-0.1.2.dev6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -4,12 +4,12 @@
 -rw-r--r--  2.0 unx      539 b- defN 80-Jan-01 00:00 rats/apps/_composite_container.py
 -rw-r--r--  2.0 unx     3089 b- defN 80-Jan-01 00:00 rats/apps/_container.py
 -rw-r--r--  2.0 unx      457 b- defN 80-Jan-01 00:00 rats/apps/_ids.py
 -rw-r--r--  2.0 unx      188 b- defN 80-Jan-01 00:00 rats/apps/_namespaces.py
 -rw-r--r--  2.0 unx      839 b- defN 80-Jan-01 00:00 rats/apps/_plugin_container.py
 -rw-r--r--  2.0 unx     1304 b- defN 80-Jan-01 00:00 rats/apps/_scoping.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 rats/apps/py.typed
--rw-r--r--  2.0 unx      716 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev1.dist-info/WHEEL
--rw-r--r--  2.0 unx       86 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1045 b- defN 16-Jan-01 00:00 rats_apps-0.1.2.dev1.dist-info/RECORD
+-rw-r--r--  2.0 unx      716 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev6.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       86 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev6.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1045 b- defN 16-Jan-01 00:00 rats_apps-0.1.2.dev6.dist-info/RECORD
 13 files, 14318 bytes uncompressed, 4925 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: rats/apps/_scoping.py
 Comment: 
 
 Filename: rats/apps/py.typed
 Comment: 
 
-Filename: rats_apps-0.1.2.dev1.dist-info/METADATA
+Filename: rats_apps-0.1.2.dev6.dist-info/METADATA
 Comment: 
 
-Filename: rats_apps-0.1.2.dev1.dist-info/WHEEL
+Filename: rats_apps-0.1.2.dev6.dist-info/WHEEL
 Comment: 
 
-Filename: rats_apps-0.1.2.dev1.dist-info/entry_points.txt
+Filename: rats_apps-0.1.2.dev6.dist-info/entry_points.txt
 Comment: 
 
-Filename: rats_apps-0.1.2.dev1.dist-info/RECORD
+Filename: rats_apps-0.1.2.dev6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rats_apps-0.1.2.dev1.dist-info/RECORD` & `rats_apps-0.1.2.dev6.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -3,11 +3,11 @@
 rats/apps/_composite_container.py,sha256=-o942CbRgczz2GXDN1gABF8vLTKDOXGddOpob1tZaNw,539
 rats/apps/_container.py,sha256=dm1wRAuPWM0hV2BtNyBmfZ-cybId55w7oua4rvKuiis,3089
 rats/apps/_ids.py,sha256=dxWCPMpMA_vpaTDJEKNByIBJaX97Db203XqWLhaOezo,457
 rats/apps/_namespaces.py,sha256=THUV_Xj5PtweC23Ob-zsSpk8exC4fT-qRwjpQ6IDm0U,188
 rats/apps/_plugin_container.py,sha256=jKD1ft5Ph-DJU7fw2NKC7_FKwSqhWTvZoJTd7lHt6_s,839
 rats/apps/_scoping.py,sha256=-5hl0RoOdQGkxWLIn42hthMUyX8_84sV8H3u40y-gIU,1304
 rats/apps/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rats_apps-0.1.2.dev1.dist-info/METADATA,sha256=rruFi8kx_YgyUixzfULJ-c2QgStNJOx0BzXFjo6RggY,716
-rats_apps-0.1.2.dev1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-rats_apps-0.1.2.dev1.dist-info/entry_points.txt,sha256=Vu1IgAPQvL4xMJzW_OG2JSPFac7HalCHyXiRr0-OfCI,86
-rats_apps-0.1.2.dev1.dist-info/RECORD,,
+rats_apps-0.1.2.dev6.dist-info/METADATA,sha256=N7hlG8xu1DhseCv2Krrt2-g5-5QoQw_8T4XDEY03OzA,716
+rats_apps-0.1.2.dev6.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+rats_apps-0.1.2.dev6.dist-info/entry_points.txt,sha256=Vu1IgAPQvL4xMJzW_OG2JSPFac7HalCHyXiRr0-OfCI,86
+rats_apps-0.1.2.dev6.dist-info/RECORD,,
```

