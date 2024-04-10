# Comparing `tmp/PyComplexHeatmap-1.7.0.tar.gz` & `tmp/PyComplexHeatmap-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComplexHeatmap-1.7.0.tar", last modified: Sat Apr  6 18:33:36 2024, max compression
+gzip compressed data, was "PyComplexHeatmap-1.7.1.tar", last modified: Wed Apr 10 19:15:48 2024, max compression
```

## Comparing `PyComplexHeatmap-1.7.0.tar` & `PyComplexHeatmap-1.7.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:33:36.068538 PyComplexHeatmap-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:33:36.036538 PyComplexHeatmap-1.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:33:36.036538 PyComplexHeatmap-1.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:33:36.036538 PyComplexHeatmap-1.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-06 18:33:36.068538 PyComplexHeatmap-1.7.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:33:36.040538 PyComplexHeatmap-1.7.0/PyComplexHeatmap/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-06 18:33:34.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    63135 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)    79542 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/clustermap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21771 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/dotHeatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    19871 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/oncoPrint.py
--rw-r--r--   0 runner    (1001) docker     (127)    26848 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:33:36.068538 PyComplexHeatmap-1.7.0/PyComplexHeatmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-06 18:33:35.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-06 18:33:36.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:33:35.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 18:33:35.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:33:36.068538 PyComplexHeatmap-1.7.0/comparison/
--rw-r--r--   0 runner    (1001) docker     (127)    88559 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/ComplexHeatmap.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   319414 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/ComplexHeatmap.png
--rw-r--r--   0 runner    (1001) docker     (127)   159236 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/PyComplexHeatmap.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   669615 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/PyComplexHeatmap.png
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/README.md
--rw-r--r--   0 runner    (1001) docker     (127) 15584021 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/beta.csv
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/compare.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/df_col.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2909164 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/df_row.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/heatmap.R
--rw-r--r--   0 runner    (1001) docker     (127)   182760 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/heatmap.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-06 18:33:12.000000 PyComplexHeatmap-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:33:36.068538 PyComplexHeatmap-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-06 18:33:12.000000 PyComplexHeatmap-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:48.043738 PyComplexHeatmap-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:48.011738 PyComplexHeatmap-1.7.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:48.011738 PyComplexHeatmap-1.7.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:48.011738 PyComplexHeatmap-1.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-10 19:15:48.039738 PyComplexHeatmap-1.7.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:48.015738 PyComplexHeatmap-1.7.1/PyComplexHeatmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 19:15:46.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63152 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79542 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/clustermap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21507 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/dotHeatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19871 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/oncoPrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26848 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:48.039738 PyComplexHeatmap-1.7.1/PyComplexHeatmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-10 19:15:47.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-10 19:15:48.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:15:47.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 19:15:47.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:48.039738 PyComplexHeatmap-1.7.1/comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)    88559 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/ComplexHeatmap.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   319414 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/ComplexHeatmap.png
+-rw-r--r--   0 runner    (1001) docker     (127)   159236 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/PyComplexHeatmap.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   669615 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/PyComplexHeatmap.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/README.md
+-rw-r--r--   0 runner    (1001) docker     (127) 15584021 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/beta.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/compare.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/df_col.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2909164 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/df_row.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/heatmap.R
+-rw-r--r--   0 runner    (1001) docker     (127)   182760 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/heatmap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-10 19:15:14.000000 PyComplexHeatmap-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:15:48.043738 PyComplexHeatmap-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-10 19:15:14.000000 PyComplexHeatmap-1.7.1/setup.py
```

### Comparing `PyComplexHeatmap-1.7.0/.github/FUNDING.yml` & `PyComplexHeatmap-1.7.1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/.github/ISSUE_TEMPLATE/bug_report.md` & `PyComplexHeatmap-1.7.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/.github/ISSUE_TEMPLATE/feature_request.md` & `PyComplexHeatmap-1.7.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/.github/workflows/python-publish.yml` & `PyComplexHeatmap-1.7.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/CITATION.cff` & `PyComplexHeatmap-1.7.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/LICENSE` & `PyComplexHeatmap-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/PKG-INFO` & `PyComplexHeatmap-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.7.0
+Version: 1.7.1
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Wubin Ding
@@ -162,15 +162,15 @@
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#Custom-annotation">
                 <img src="docs/images/gallery10.png" title="Custom annotation" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
-            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#Change-orentation-to-the-left">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/gene_enrichment_analysis.html#Plot">
                 <img src="docs/images/gallery12.png" title="Plot only the annotation with different orientations" align="center" width="250px">
             </a>
         </td>
     </tr>
 </table>
 
 ### [Advanced Usage](https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html)
```

### Comparing `PyComplexHeatmap-1.7.0/PyComplexHeatmap/annotations.py` & `PyComplexHeatmap-1.7.1/PyComplexHeatmap/annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,15 +455,15 @@
 		cmap="auto",
 		colors=None,
 		merge=False,
 		extend=False,
 		frac=0.2,
 		majority=True,
 		adjust_color=True,
-		luminance=0.5,
+		luminance=0.8,
 		height=None,
 		legend=False,
 		legend_kws=None,
 		relpos=None,
 		**plot_kws
 	):
 		super().__init__(
@@ -519,14 +519,15 @@
 			color="black",
 			shrinkA=shrink,
 			shrinkB=shrink,
 			relpos=rp,
 			patchA=None,
 			patchB=None,
 			connectionstyle=None,
+			linewidth=0.5
 		)
 		# arrow: ->, from text to point.
 		# self.plot_kws.setdefault('transform_rotates_text', False)
 		self.plot_kws.setdefault("arrowprops", {})
 		for k in arrowprops:
 			if k not in self.plot_kws['arrowprops']:
 				self.plot_kws['arrowprops'][k]=arrowprops[k]
```

### Comparing `PyComplexHeatmap-1.7.0/PyComplexHeatmap/clustermap.py` & `PyComplexHeatmap-1.7.1/PyComplexHeatmap/clustermap.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/PyComplexHeatmap/colors.py` & `PyComplexHeatmap-1.7.1/PyComplexHeatmap/colors.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/PyComplexHeatmap/dotHeatmap.py` & `PyComplexHeatmap-1.7.1/PyComplexHeatmap/dotHeatmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 		ax
 	colors : dict
 		colors to control the dot, keys should be the value in hue. if colors is a str, then colors will overwrite
 		the parameter `c`.
 	cmap : str of dict
 		control the colormap of the dot, if cmap is a dict, keys should be the values from hue dataframe.
 		If `cmap` is a str (such as 'Set1'), the parameter `colors` will overwrite the colors of dots.
-		If `cmap` wisas a dict, then this paramter will overwrite the `colors`, and colors can only control the
+		If `cmap` was a dict, then this paramter will overwrite the `colors`, and colors can only control the
 		colors for markers.
 	s : int, float, or dataframe
 		control the sizes of dot.
 	c : dataframe, or str
 		control the colors of dots.
 	marker : str, dataframe or dict
 		when marker is a dict, hue must not be None, and keys are categorical values from hue, values should be marker.
@@ -195,23 +195,14 @@
 			)  # vmax=vmax,vmin=vmin,
 	elif type(cmap) == dict and not hue is None:
 		for h in cmap:  # key are hue, values are cmap
 			# df1 = df.query("Hue==@h").copy()
 			df1 = df.loc[df.Hue==h].copy()
 			if df1.shape[0] == 0:
 				continue
-			if isinstance(colors, str):
-				df1["C"] = colors
-			elif isinstance(kwargs.get("c", None), str):
-				df1["C"] = kwargs.get("c", None)
-			else:
-				df1["C"] = df1.S.values
-				# print(df1.C.describe())
-			# if pd.isna(df1.C.iloc[0]):
-			#     print(locals())
 			kwargs["cmap"] = cmap[h]
 			for mk in df1.Markers.unique():
 				# df2 = df1.query("Markers==@mk").copy()
 				df2 = df1.loc[df1.Markers==mk].copy()
 				kwargs["marker"] = mk
 				ax.scatter(
 					x=df2.X.values,
```

### Comparing `PyComplexHeatmap-1.7.0/PyComplexHeatmap/example.py` & `PyComplexHeatmap-1.7.1/PyComplexHeatmap/example.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/PyComplexHeatmap/oncoPrint.py` & `PyComplexHeatmap-1.7.1/PyComplexHeatmap/oncoPrint.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/PyComplexHeatmap/utils.py` & `PyComplexHeatmap-1.7.1/PyComplexHeatmap/utils.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/PyComplexHeatmap.egg-info/PKG-INFO` & `PyComplexHeatmap-1.7.1/PyComplexHeatmap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.7.0
+Version: 1.7.1
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Wubin Ding
@@ -162,15 +162,15 @@
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#Custom-annotation">
                 <img src="docs/images/gallery10.png" title="Custom annotation" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
-            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#Change-orentation-to-the-left">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/gene_enrichment_analysis.html#Plot">
                 <img src="docs/images/gallery12.png" title="Plot only the annotation with different orientations" align="center" width="250px">
             </a>
         </td>
     </tr>
 </table>
 
 ### [Advanced Usage](https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html)
```

### Comparing `PyComplexHeatmap-1.7.0/PyComplexHeatmap.egg-info/SOURCES.txt` & `PyComplexHeatmap-1.7.1/PyComplexHeatmap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/README.md` & `PyComplexHeatmap-1.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#Custom-annotation">
                 <img src="docs/images/gallery10.png" title="Custom annotation" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
-            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#Change-orentation-to-the-left">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/gene_enrichment_analysis.html#Plot">
                 <img src="docs/images/gallery12.png" title="Plot only the annotation with different orientations" align="center" width="250px">
             </a>
         </td>
     </tr>
 </table>
 
 ### [Advanced Usage](https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html)
```

### Comparing `PyComplexHeatmap-1.7.0/comparison/ComplexHeatmap.pdf` & `PyComplexHeatmap-1.7.1/comparison/ComplexHeatmap.pdf`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/comparison/ComplexHeatmap.png` & `PyComplexHeatmap-1.7.1/comparison/ComplexHeatmap.png`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/comparison/PyComplexHeatmap.pdf` & `PyComplexHeatmap-1.7.1/comparison/PyComplexHeatmap.pdf`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/comparison/PyComplexHeatmap.png` & `PyComplexHeatmap-1.7.1/comparison/PyComplexHeatmap.png`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/comparison/README.md` & `PyComplexHeatmap-1.7.1/comparison/README.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/comparison/beta.csv` & `PyComplexHeatmap-1.7.1/comparison/beta.csv`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/comparison/df_col.csv` & `PyComplexHeatmap-1.7.1/comparison/df_col.csv`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/comparison/df_row.csv` & `PyComplexHeatmap-1.7.1/comparison/df_row.csv`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/comparison/heatmap.R` & `PyComplexHeatmap-1.7.1/comparison/heatmap.R`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/comparison/heatmap.ipynb` & `PyComplexHeatmap-1.7.1/comparison/heatmap.ipynb`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/comparison/heatmap.py` & `PyComplexHeatmap-1.7.1/comparison/heatmap.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/pyproject.toml` & `PyComplexHeatmap-1.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.0/setup.py` & `PyComplexHeatmap-1.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 long_description = (this_directory / "README.md").read_text()
 # print(long_description)
 
 # release new version
 setup(
     name="PyComplexHeatmap",
 	use_scm_version=True,  # {'version_scheme': 'python-simplified-semver',"local_scheme": "no-local-version"},
-	setup_requires=['setuptools_scm','fastcluster'],
+	setup_requires=['setuptools_scm'],
     description="A Python package to plot complex heatmap",
     # long_description="#PyComplexHeatmap\n##Documentation:https://dingwb.github.io/PyComplexHeatmap/build/html/index.html",
     # long_description_content_type='text/markdown',
     author="Wubin Ding",
     author_email="ding.wu.bin.gm@gmail.com",
     url="https://github.com/DingWB/PyComplexHeatmap",
     packages=["PyComplexHeatmap"],  # src
-    # install_requires=['matplotlib>=3.3.1','pandas'],
+    install_requires=["matplotlib<3.8.0","numpy","pandas>=1.3.5", "scipy","fastcluster"],
     include_package_data=True,
 )
 # rm -rf dist && rm -rf PyComplexHeatmap/PyComplexHeatmap.egg-info/
 # python setup.py sdist bdist_wheel
 # twine upload dist/*
```

