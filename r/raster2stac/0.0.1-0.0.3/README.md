# Comparing `tmp/raster2stac-0.0.1.tar.gz` & `tmp/raster2stac-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster2stac-0.0.1.tar", last modified: Wed Mar 20 21:27:46 2024, max compression
+gzip compressed data, was "raster2stac-0.0.3.tar", last modified: Wed Apr 10 09:36:31 2024, max compression
```

## Comparing `raster2stac-0.0.1.tar` & `raster2stac-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rbalogun (1149420415) domain users (1149400513)        0 2024-03-20 21:27:46.500182 raster2stac-0.0.1/
--rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)     1105 2024-03-20 20:41:44.000000 raster2stac-0.0.1/LICENSE
--rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)     8947 2024-03-20 21:27:46.500182 raster2stac-0.0.1/PKG-INFO
--rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)     7956 2024-03-20 20:41:44.000000 raster2stac-0.0.1/README.md
--rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)     1029 2024-03-20 21:27:29.000000 raster2stac-0.0.1/pyproject.toml
-drwxr-xr-x   0 rbalogun (1149420415) domain users (1149400513)        0 2024-03-20 21:27:46.500182 raster2stac-0.0.1/raster2stac/
--rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)      303 2024-03-20 20:48:04.000000 raster2stac-0.0.1/raster2stac/__init__.py
--rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)       21 2024-03-20 20:41:44.000000 raster2stac-0.0.1/raster2stac/_version.py
--rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)    41274 2024-03-20 20:41:44.000000 raster2stac-0.0.1/raster2stac/raster2stac.py
--rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)    14551 2024-03-20 20:41:44.000000 raster2stac-0.0.1/raster2stac/rioxarray_stac.py
-drwxr-xr-x   0 rbalogun (1149420415) domain users (1149400513)        0 2024-03-20 21:27:46.500182 raster2stac-0.0.1/raster2stac.egg-info/
--rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)     8947 2024-03-20 21:27:46.000000 raster2stac-0.0.1/raster2stac.egg-info/PKG-INFO
--rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)      286 2024-03-20 21:27:46.000000 raster2stac-0.0.1/raster2stac.egg-info/SOURCES.txt
--rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)        1 2024-03-20 21:27:46.000000 raster2stac-0.0.1/raster2stac.egg-info/dependency_links.txt
--rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)       12 2024-03-20 21:27:46.000000 raster2stac-0.0.1/raster2stac.egg-info/top_level.txt
--rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)       38 2024-03-20 21:27:46.500182 raster2stac-0.0.1/setup.cfg
--rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)      537 2024-03-20 21:18:11.000000 raster2stac-0.0.1/setup.py
+drwxr-xr-x   0 rbalogun (1149420415) domain users (1149400513)        0 2024-04-10 09:36:31.304528 raster2stac-0.0.3/
+-rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)     1105 2024-04-09 08:20:39.000000 raster2stac-0.0.3/LICENSE
+-rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)     8983 2024-04-10 09:36:31.304528 raster2stac-0.0.3/PKG-INFO
+-rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)     8014 2024-04-09 08:44:28.000000 raster2stac-0.0.3/README.md
+-rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)     1177 2024-04-10 09:34:03.000000 raster2stac-0.0.3/pyproject.toml
+drwxr-xr-x   0 rbalogun (1149420415) domain users (1149400513)        0 2024-04-10 09:36:31.304528 raster2stac-0.0.3/raster2stac/
+-rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)      303 2024-04-09 08:20:39.000000 raster2stac-0.0.3/raster2stac/__init__.py
+-rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)       21 2024-04-09 08:20:39.000000 raster2stac-0.0.3/raster2stac/_version.py
+-rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)    42257 2024-04-09 08:39:12.000000 raster2stac-0.0.3/raster2stac/raster2stac.py
+-rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)    14551 2024-04-09 08:20:39.000000 raster2stac-0.0.3/raster2stac/rioxarray_stac.py
+drwxr-xr-x   0 rbalogun (1149420415) domain users (1149400513)        0 2024-04-10 09:36:31.304528 raster2stac-0.0.3/raster2stac.egg-info/
+-rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)     8983 2024-04-10 09:36:31.000000 raster2stac-0.0.3/raster2stac.egg-info/PKG-INFO
+-rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)      286 2024-04-10 09:36:31.000000 raster2stac-0.0.3/raster2stac.egg-info/SOURCES.txt
+-rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)        1 2024-04-10 09:36:31.000000 raster2stac-0.0.3/raster2stac.egg-info/dependency_links.txt
+-rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)       12 2024-04-10 09:36:31.000000 raster2stac-0.0.3/raster2stac.egg-info/top_level.txt
+-rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)       38 2024-04-10 09:36:31.304528 raster2stac-0.0.3/setup.cfg
+-rw-r--r--   0 rbalogun (1149420415) domain users (1149400513)       37 2024-04-10 09:35:38.000000 raster2stac-0.0.3/setup.py
```

### Comparing `raster2stac-0.0.1/LICENSE` & `raster2stac-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `raster2stac-0.0.1/PKG-INFO` & `raster2stac-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: raster2stac
-Version: 0.0.1
+Version: 0.0.3
 Summary: Create valid STAC Collections, Items and Assets given already existing raster datasets
-Author: Michele Claus
 Author-email: Michele Claus <michele.claus@eurac.edu>
 Project-URL: Homepage, https://gitlab.inf.unibz.it/earth_observation_public/raster-to-stac
 Project-URL: Issues, https://gitlab.inf.unibz.it/earth_observation_public/raster-to-stac/-/issues
 Keywords: STAC,Metadata,Cloud-Optimized GeoTIFFs,Kerchunk,NetCDF
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -209,10 +208,21 @@
 >     spatial_ref  float64 8B 0.0
 >   * time         (time) datetime64[ns] 6kB 2001-01-01 2001-01-02 ... 2002-12-31
 >   * bands        (bands) object 16B 'sp' 't2m'
 > Attributes:
 >     NCO:      netCDF Operators version 5.1.9 (Homepage = http://nco.sf.net, C...
 
 ```
+
+## Contributing
+
+
+## Contributors
+
+
 ## License
 
 This project is distributed with MIT license - see 'LICENSE' for details.
+
+
+## External links
+
```

### Comparing `raster2stac-0.0.1/README.md` & `raster2stac-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -188,10 +188,21 @@
 >     spatial_ref  float64 8B 0.0
 >   * time         (time) datetime64[ns] 6kB 2001-01-01 2001-01-02 ... 2002-12-31
 >   * bands        (bands) object 16B 'sp' 't2m'
 > Attributes:
 >     NCO:      netCDF Operators version 5.1.9 (Homepage = http://nco.sf.net, C...
 
 ```
+
+## Contributing
+
+
+## Contributors
+
+
 ## License
 
 This project is distributed with MIT license - see 'LICENSE' for details.
+
+
+## External links
+
```

### Comparing `raster2stac-0.0.1/pyproject.toml` & `raster2stac-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = [
+      "setuptools>=61.0", "numpy", "pandas", "xarray",
+      "rioxarray", "pystac", "rio_stac", "boto3", "botocore",
+      "openeo[localprocessing]", "fsspec"
+      ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raster2stac"
-version = "0.0.1"
+version = "0.0.3"
 authors = [
   { name="Michele Claus", email="michele.claus@eurac.edu" },
 ]
 description = "Create valid STAC Collections, Items and Assets given already existing raster datasets"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `raster2stac-0.0.1/raster2stac/raster2stac.py` & `raster2stac-0.0.3/raster2stac/raster2stac.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """
-Raster2STAC - Extract STAC format metadata from raster data 
+Raster2STAC - Generate STAC metadata from raster data 
 
 This module provides a class `Raster2STAC` for extracting from raster data, represented as an `xr.DataArray`
-or a file path which links to a local .nc file (that will be converted in `xr.DataArray`), 
-SpatioTemporal Asset Catalog (STAC) format metadata JSON files.
-This allows the output data to be ingested into Eurac's STAC FastApi
+or a file path to netCDF(s) file(s), SpatioTemporal Asset Catalog (STAC) format metadata JSON files.
 
 Authors: Mercurio Lorenzo, Eurac Research - Inst. for Earth Observation, Bolzano/Bozen IT
 Authors: Michele Claus, Eurac Research - Inst. for Earth Observation, Bolzano/Bozen IT
-Date: 2024-03-06
+Date: 2024-03-24
 """
 import sys
 import datetime 
 import os 
 import pystac
 from pystac.utils import str_to_datetime
 import rasterio
@@ -53,15 +51,15 @@
 _log = logging.getLogger(__name__)
 
 
 DATACUBE_EXT_VERSION = "v1.0.0"
 
 class Raster2STAC():
     """
-    Raster2STAC Class - Converte dati raster nel formato STAC.
+    Raster2STAC Class - Convert raster data format into STAC metadata.
 
     Args:
         data: str or xr.DataArray
             Raster data as xr.DataArray or file path referring to a netCDF file.
         collection_id: str
             Identifier of the collection as a string (Example: 'blue-river-basin')
         collection_url: str
@@ -95,14 +93,16 @@
              Part of AWS S3 configuration: AWS region for S3.
         version: Optional[str] = None,
             Version of the STAC collection.
         license: Optional[str] = None,
             License information about STAC collection and its assets.
         sci_citation: Optional[str] = None
             Scientific citation(s) reference(s) about STAC collection.
+        write_collection_assets = False,
+            Include all assets in the STAC Collection, with unique keys.
     """
 
 
 
     def __init__(self,
                  data,
                  collection_id,
@@ -116,18 +116,21 @@
                  providers: Optional[list] = None,
                  links: Optional[list] = None,
                  stac_version="1.0.0",
                  s3_upload=False,
                  bucket_name = None,
                  bucket_file_prefix = None,
                  aws_region = None,
+                 aws_access_key = None,
+                 aws_secret_key = None,
                  version = None,
                  license = None,
                  sci_doi = None,
-                 sci_citation=None
+                 sci_citation=None,
+                 write_collection_assets=False
                 ):
         
         if ignore_warns == True:
             import warnings
             warnings.filterwarnings("ignore")
 
         self.data = data
@@ -144,14 +147,15 @@
         self.item_prefix = item_prefix
         self.description = description
         self.keywords = keywords
         self.providers = providers
         self.links = links
         self.stac_version = stac_version
         self.sci_doi = sci_doi
+        self.write_collection_assets = write_collection_assets
         self.extensions = [
             f"https://stac-extensions.github.io/projection/{PROJECTION_EXT_VERSION}/schema.json", 
             f"https://stac-extensions.github.io/raster/{RASTER_EXT_VERSION}/schema.json",
             f"https://stac-extensions.github.io/eo/{EO_EXT_VERSION}/schema.json",
             # f"https://stac-extensions.github.io/datacube/{DATACUBE_EXT_VERSION}/schema.json",
         ]
 
@@ -531,15 +535,15 @@
             extra_fields["sci:doi"] = self.sci_doi
         
         if self.sci_citation is not None or self.sci_doi is not None:
             self.extensions.append("https://stac-extensions.github.io/scientific/v1.0.0/schema.json")
     
 
         extra_fields["summaries"] = eo_info
-
+        self.extensions.append("https://stac-extensions.github.io/datacube/v2.2.0/schema.json")
         extra_fields["stac_extensions"] = self.extensions
 
         cube_dimensons = {
             self.X_DIM: {
                 "axis": "x",
                 "type": "spatial",
                 "extent": [float(self.data.coords[self.X_DIM].min()), float(self.data.coords[self.X_DIM].max())],
@@ -668,16 +672,16 @@
         self.T_DIM = self.data.openeo.temporal_dims[0]
         self.B_DIM = self.data.openeo.band_dims[0]
         _log.debug(f'Extracted label dimensions from input are:\nx dimension:{self.X_DIM}\ny dimension:{self.Y_DIM}\nbands dimension:{self.B_DIM}\ntemporal dimension:{self.T_DIM}')
 
         spatial_extents = []
         temporal_extents = []
 
-        item_list = []  # Create a list to store the items
-
+        # item_list = []  # Create a list to store the items
+        collection_assets = {}
         # Get the time dimension values
         time_values = self.data[self.T_DIM].values
         
         eo_info = {}
         
         #resetting CSV file
         open(f"{Path(self.output_folder)}/inline_items.csv", 'w+') 
@@ -761,30 +765,33 @@
                     
                     cloudcover = src_dst.get_tag_item("CLOUDCOVER", "IMAGERY")
                     # TODO: try to add this field to the COG. Currently not present in the files we write here.
                     if cloudcover is not None:
                         self.properties.update({"eo:cloud_cover": int(cloudcover)})
 
                     eo_info["eo:bands"] = [band_dict]
-
-                    pystac_assets.append(
-                        (
-                            band, 
-                            pystac.Asset(
+                    asset = pystac.Asset(
                                 href=link_path, 
                                 media_type=self.media_type,
                                 extra_fields={
                                     **proj_info,
                                     **raster_info, 
                                     **eo_info
                                 },
                                 roles=["data"],
-                            ),
+                            )
+                    pystac_assets.append(
+                        (
+                            band, 
+                            asset,
                         )
                     )
+                    if self.write_collection_assets:
+                        collection_assets[f"{item_id}_{band}"] = asset
+                        
             
             eo_info["eo:bands"] = eo_bands_list
 
             minx, miny, maxx, maxy = zip(*bboxes)
             bbox = [min(minx), min(miny), max(maxx), max(maxy)]
 
             # metadata_item_path = f"{self.fix_path_slash(time_slice_dir)}metadata.json"
@@ -902,15 +909,15 @@
         if self.sci_doi is not None:
             extra_fields["sci:doi"] = self.sci_doi
         
         if self.sci_citation is not None or self.sci_doi is not None:
             self.extensions.append("https://stac-extensions.github.io/scientific/v1.0.0/schema.json")
 
         extra_fields["summaries"] = eo_info
-
+        self.extensions.append("https://stac-extensions.github.io/datacube/v2.2.0/schema.json")
         extra_fields["stac_extensions"] = self.extensions
 
         cube_dimensons = {
             self.X_DIM: {
                 "axis": "x",
                 "type": "spatial",
                 "extent": [float(self.data.coords[self.X_DIM].min()), float(self.data.coords[self.X_DIM].max())],
@@ -931,21 +938,29 @@
             self.B_DIM: {
                 "type": "bands",
                 "values": list(self.data[self.B_DIM].values),
             }
         }
 
         extra_fields["cube:dimensions"] = cube_dimensons
-
-        self.stac_collection = pystac.collection.Collection(
-            id=self.collection_id,
-            description=self.description,
-            extent=pystac.Extent(spatial=s_ext, temporal=t_ext),
-            extra_fields=extra_fields,
-        )
+        if self.write_collection_assets:
+            self.stac_collection = pystac.collection.Collection(
+                id=self.collection_id,
+                description=self.description,
+                extent=pystac.Extent(spatial=s_ext, temporal=t_ext),
+                extra_fields=extra_fields,
+                assets = collection_assets
+            )
+        else:
+            self.stac_collection = pystac.collection.Collection(
+                id=self.collection_id,
+                description=self.description,
+                extent=pystac.Extent(spatial=s_ext, temporal=t_ext),
+                extra_fields=extra_fields
+            )
 
         
         self.stac_collection.add_link(
             pystac.Link(
                 pystac.RelType.ITEMS,
                 f"{self.fix_path_slash(self.collection_url)}{self.collection_id}/items",
                 media_type=pystac.MediaType.JSON,
```

### Comparing `raster2stac-0.0.1/raster2stac/rioxarray_stac.py` & `raster2stac-0.0.3/raster2stac/rioxarray_stac.py`

 * *Files identical despite different names*

### Comparing `raster2stac-0.0.1/raster2stac.egg-info/PKG-INFO` & `raster2stac-0.0.3/raster2stac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: raster2stac
-Version: 0.0.1
+Version: 0.0.3
 Summary: Create valid STAC Collections, Items and Assets given already existing raster datasets
-Author: Michele Claus
 Author-email: Michele Claus <michele.claus@eurac.edu>
 Project-URL: Homepage, https://gitlab.inf.unibz.it/earth_observation_public/raster-to-stac
 Project-URL: Issues, https://gitlab.inf.unibz.it/earth_observation_public/raster-to-stac/-/issues
 Keywords: STAC,Metadata,Cloud-Optimized GeoTIFFs,Kerchunk,NetCDF
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -209,10 +208,21 @@
 >     spatial_ref  float64 8B 0.0
 >   * time         (time) datetime64[ns] 6kB 2001-01-01 2001-01-02 ... 2002-12-31
 >   * bands        (bands) object 16B 'sp' 't2m'
 > Attributes:
 >     NCO:      netCDF Operators version 5.1.9 (Homepage = http://nco.sf.net, C...
 
 ```
+
+## Contributing
+
+
+## Contributors
+
+
 ## License
 
 This project is distributed with MIT license - see 'LICENSE' for details.
+
+
+## External links
+
```

