# Comparing `tmp/scimap-2.0.3.tar.gz` & `tmp/scimap-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scimap-2.0.3.tar", max compression
+gzip compressed data, was "scimap-2.0.4.tar", max compression
```

## Comparing `scimap-2.0.3.tar` & `scimap-2.0.4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1101 2023-12-22 12:20:25.774355 scimap-2.0.3/LICENSE
--rw-r--r--   0        0        0     2759 2024-04-02 17:41:31.643157 scimap-2.0.3/README.md
--rw-r--r--   0        0        0     2522 2024-04-02 18:20:11.098348 scimap-2.0.3/pyproject.toml
--rw-r--r--   0        0        0      391 2024-04-01 23:22:15.513728 scimap-2.0.3/scimap/__init__.py
--rw-r--r--   0        0        0       21 2021-07-01 20:47:33.000000 scimap-2.0.3/scimap/__main__.py
--rw-r--r--   0        0        0        0 2021-07-01 20:47:33.000000 scimap-2.0.3/scimap/cli/__init__.py
--rw-r--r--   0        0        0     5559 2023-04-20 14:28:15.443473 scimap-2.0.3/scimap/cli/_scimap_mcmicro.py
--rw-r--r--   0        0        0      592 2023-04-20 14:28:51.699589 scimap-2.0.3/scimap/cli/test.py
--rw-r--r--   0        0        0        0 2024-04-01 23:21:46.158522 scimap-2.0.3/scimap/external/__init__.py
--rw-r--r--   0        0        0      297 2024-03-20 19:13:27.572207 scimap-2.0.3/scimap/helpers/__init__.py
--rw-r--r--   0        0        0     7715 2024-03-20 20:49:48.491605 scimap-2.0.3/scimap/helpers/_classify.py
--rw-r--r--   0        0        0     6938 2024-03-12 20:54:07.000000 scimap-2.0.3/scimap/helpers/addROI_omero.py
--rw-r--r--   0        0        0     3141 2023-11-21 19:42:38.615795 scimap-2.0.3/scimap/helpers/add_roi_scatter.py
--rw-r--r--   0        0        0    17024 2024-03-01 20:05:28.511793 scimap-2.0.3/scimap/helpers/animate.py
--rw-r--r--   0        0        0     7031 2024-03-01 20:14:20.029603 scimap-2.0.3/scimap/helpers/classify.py
--rw-r--r--   0        0        0     1897 2024-03-20 19:41:09.893157 scimap-2.0.3/scimap/helpers/downloadDemoData.py
--rw-r--r--   0        0        0     5065 2024-03-01 20:24:14.533825 scimap-2.0.3/scimap/helpers/dropFeatures.py
--rw-r--r--   0        0        0     4944 2024-03-20 13:25:21.701481 scimap-2.0.3/scimap/helpers/merge_adata_obs.py
--rw-r--r--   0        0        0     3601 2024-03-01 20:40:16.298072 scimap-2.0.3/scimap/helpers/rename.py
--rw-r--r--   0        0        0     6194 2024-03-20 01:42:22.133668 scimap-2.0.3/scimap/helpers/scimap_to_csv.py
--rw-r--r--   0        0        0      766 2024-03-19 18:17:18.230168 scimap-2.0.3/scimap/plotting/__init__.py
--rw-r--r--   0        0        0    16878 2024-04-02 18:20:06.395257 scimap-2.0.3/scimap/plotting/addROI_image.py
--rw-r--r--   0        0        0     6564 2024-03-02 01:59:56.790600 scimap-2.0.3/scimap/plotting/cluster_plots.py
--rw-r--r--   0        0        0     8369 2024-03-02 01:55:48.580935 scimap-2.0.3/scimap/plotting/densityPlot2D.py
--rw-r--r--   0        0        0     8772 2024-03-20 13:51:51.354626 scimap-2.0.3/scimap/plotting/distPlot.py
--rw-r--r--   0        0        0     6709 2024-03-02 01:59:44.870855 scimap-2.0.3/scimap/plotting/foldchange.py
--rw-r--r--   0        0        0    11271 2024-04-02 18:18:12.032282 scimap-2.0.3/scimap/plotting/gate_finder.py
--rw-r--r--   0        0        0    11207 2024-03-18 18:24:57.598183 scimap-2.0.3/scimap/plotting/groupCorrelation.py
--rw-r--r--   0        0        0    18210 2024-03-18 18:41:06.721737 scimap-2.0.3/scimap/plotting/heatmap.py
--rw-r--r--   0        0        0     9552 2024-04-02 18:18:20.828150 scimap-2.0.3/scimap/plotting/image_viewer.py
--rw-r--r--   0        0        0    10417 2024-03-18 18:24:52.838506 scimap-2.0.3/scimap/plotting/markerCorrelation.py
--rw-r--r--   0        0        0     7419 2024-03-02 01:59:15.476562 scimap-2.0.3/scimap/plotting/pie.py
--rw-r--r--   0        0        0    12242 2024-03-19 18:32:03.627202 scimap-2.0.3/scimap/plotting/spatialInteractionNetwork.py
--rw-r--r--   0        0        0    10165 2024-03-19 01:23:30.046016 scimap-2.0.3/scimap/plotting/spatial_distance.py
--rw-r--r--   0        0        0    11795 2024-03-19 12:21:07.752382 scimap-2.0.3/scimap/plotting/spatial_interaction.py
--rw-r--r--   0        0        0     5060 2024-03-19 19:10:54.724495 scimap-2.0.3/scimap/plotting/spatial_pscore.py
--rw-r--r--   0        0        0    12601 2024-03-17 15:26:02.182943 scimap-2.0.3/scimap/plotting/spatial_scatterPlot.py
--rw-r--r--   0        0        0     7727 2024-03-02 01:58:34.424269 scimap-2.0.3/scimap/plotting/stacked_barplot.py
--rw-r--r--   0        0        0    12547 2024-03-18 18:34:47.607355 scimap-2.0.3/scimap/plotting/umap.py
--rw-r--r--   0        0        0    18847 2024-03-02 01:58:10.302280 scimap-2.0.3/scimap/plotting/voronoi.py
--rw-r--r--   0        0        0      129 2024-03-17 18:13:28.725249 scimap-2.0.3/scimap/preprocessing/__init__.py
--rw-r--r--   0        0        0     4929 2024-03-01 22:07:39.817117 scimap-2.0.3/scimap/preprocessing/combat.py
--rw-r--r--   0        0        0     3979 2024-03-17 19:14:56.795915 scimap-2.0.3/scimap/preprocessing/log1p.py
--rw-r--r--   0        0        0    11153 2024-03-13 21:27:02.000000 scimap-2.0.3/scimap/preprocessing/mcmicro_to_scimap.py
--rw-r--r--   0        0        0     3642 2024-03-18 00:27:18.438422 scimap-2.0.3/scimap/preprocessing/ngraph.py
--rw-r--r--   0        0        0    17838 2024-02-29 22:11:30.005842 scimap-2.0.3/scimap/preprocessing/rescale.py
--rw-r--r--   0        0        0  2003213 2021-07-01 20:47:33.000000 scimap-2.0.3/scimap/tests/_data/example_data.csv
--rw-r--r--   0        0        0  1590001 2021-07-01 20:47:33.000000 scimap-2.0.3/scimap/tests/_data/example_data.h5ad
--rw-r--r--   0        0        0     1908 2021-07-01 20:47:33.000000 scimap-2.0.3/scimap/tests/_data/phenotype_workflow.csv
--rw-r--r--   0        0        0     1265 2024-03-02 02:51:31.375137 scimap-2.0.3/scimap/tests/test_helpers.py
--rw-r--r--   0        0        0      982 2024-03-02 02:50:46.201820 scimap-2.0.3/scimap/tests/test_preprocessing.py
--rw-r--r--   0        0        0     4675 2024-03-02 02:49:28.903918 scimap-2.0.3/scimap/tests/test_tools.py
--rw-r--r--   0        0        0      568 2024-03-02 02:44:25.945510 scimap-2.0.3/scimap/tools/__init__.py
--rw-r--r--   0        0        0    20200 2024-03-19 23:48:54.910997 scimap-2.0.3/scimap/tools/cluster.py
--rw-r--r--   0        0        0    10598 2024-03-18 21:08:47.269456 scimap-2.0.3/scimap/tools/foldchange.py
--rw-r--r--   0        0        0    18754 2024-03-01 13:54:09.563795 scimap-2.0.3/scimap/tools/phenotype_cells.py
--rw-r--r--   0        0        0    12714 2024-03-19 20:32:33.950090 scimap-2.0.3/scimap/tools/spatial_aggregate.py
--rw-r--r--   0        0        0     8731 2024-03-02 03:07:59.502620 scimap-2.0.3/scimap/tools/spatial_cluster.py
--rw-r--r--   0        0        0     9097 2024-03-19 23:43:08.527959 scimap-2.0.3/scimap/tools/spatial_count.py
--rw-r--r--   0        0        0     6224 2024-03-01 14:13:55.522643 scimap-2.0.3/scimap/tools/spatial_distance.py
--rw-r--r--   0        0        0    13752 2024-03-20 01:28:34.142208 scimap-2.0.3/scimap/tools/spatial_expression.py
--rw-r--r--   0        0        0    12059 2024-03-19 12:11:34.371207 scimap-2.0.3/scimap/tools/spatial_interaction.py
--rw-r--r--   0        0        0    11333 2024-03-01 18:59:27.631718 scimap-2.0.3/scimap/tools/spatial_lda.py
--rw-r--r--   0        0        0    12452 2024-03-19 18:49:22.715271 scimap-2.0.3/scimap/tools/spatial_pscore.py
--rw-r--r--   0        0        0    18461 2024-03-19 21:36:08.728628 scimap-2.0.3/scimap/tools/spatial_similarity_search.py
--rw-r--r--   0        0        0     3830 2024-03-01 19:23:35.518742 scimap-2.0.3/scimap/tools/umap.py
--rw-r--r--   0        0        0     4780 1970-01-01 00:00:00.000000 scimap-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-12-22 12:20:25.000000 scimap-2.0.4/LICENSE
+-rw-r--r--   0        0        0     2546 2024-04-10 20:01:33.497274 scimap-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2987 2024-04-02 18:28:23.000000 scimap-2.0.4/README.md
+-rw-r--r--   0        0        0      391 2024-04-01 23:22:15.000000 scimap-2.0.4/scimap/__init__.py
+-rw-r--r--   0        0        0       21 2021-07-01 20:47:33.000000 scimap-2.0.4/scimap/__main__.py
+-rw-r--r--   0        0        0        0 2021-07-01 20:47:33.000000 scimap-2.0.4/scimap/cli/__init__.py
+-rw-r--r--   0        0        0     5559 2023-04-20 14:28:15.000000 scimap-2.0.4/scimap/cli/_scimap_mcmicro.py
+-rw-r--r--   0        0        0      592 2023-04-20 14:28:51.000000 scimap-2.0.4/scimap/cli/test.py
+-rw-r--r--   0        0        0        0 2024-04-01 23:21:46.000000 scimap-2.0.4/scimap/external/__init__.py
+-rw-r--r--   0        0        0      297 2024-03-20 19:13:27.000000 scimap-2.0.4/scimap/helpers/__init__.py
+-rw-r--r--   0        0        0     7715 2024-03-20 20:49:48.000000 scimap-2.0.4/scimap/helpers/_classify.py
+-rw-r--r--   0        0        0     3141 2023-11-21 19:42:38.000000 scimap-2.0.4/scimap/helpers/add_roi_scatter.py
+-rw-r--r--   0        0        0     6938 2024-03-12 20:54:07.191329 scimap-2.0.4/scimap/helpers/addROI_omero.py
+-rw-r--r--   0        0        0    17024 2024-03-01 20:05:28.000000 scimap-2.0.4/scimap/helpers/animate.py
+-rw-r--r--   0        0        0     7031 2024-03-01 20:14:20.000000 scimap-2.0.4/scimap/helpers/classify.py
+-rw-r--r--   0        0        0     1897 2024-03-20 19:41:09.000000 scimap-2.0.4/scimap/helpers/downloadDemoData.py
+-rw-r--r--   0        0        0     5065 2024-03-01 20:24:14.000000 scimap-2.0.4/scimap/helpers/dropFeatures.py
+-rw-r--r--   0        0        0     4944 2024-03-20 13:25:21.000000 scimap-2.0.4/scimap/helpers/merge_adata_obs.py
+-rw-r--r--   0        0        0     3601 2024-03-01 20:40:16.000000 scimap-2.0.4/scimap/helpers/rename.py
+-rw-r--r--   0        0        0     6194 2024-03-20 01:42:22.000000 scimap-2.0.4/scimap/helpers/scimap_to_csv.py
+-rw-r--r--   0        0        0      766 2024-03-19 18:17:18.000000 scimap-2.0.4/scimap/plotting/__init__.py
+-rw-r--r--   0        0        0    16878 2024-04-02 18:20:06.000000 scimap-2.0.4/scimap/plotting/addROI_image.py
+-rw-r--r--   0        0        0     6564 2024-03-02 01:59:56.000000 scimap-2.0.4/scimap/plotting/cluster_plots.py
+-rw-r--r--   0        0        0     8369 2024-03-02 01:55:48.000000 scimap-2.0.4/scimap/plotting/densityPlot2D.py
+-rw-r--r--   0        0        0     8772 2024-03-20 13:51:51.000000 scimap-2.0.4/scimap/plotting/distPlot.py
+-rw-r--r--   0        0        0     6709 2024-03-02 01:59:44.000000 scimap-2.0.4/scimap/plotting/foldchange.py
+-rw-r--r--   0        0        0    11271 2024-04-02 18:18:12.000000 scimap-2.0.4/scimap/plotting/gate_finder.py
+-rw-r--r--   0        0        0    11207 2024-03-18 18:24:57.000000 scimap-2.0.4/scimap/plotting/groupCorrelation.py
+-rw-r--r--   0        0        0    18210 2024-03-18 18:41:06.000000 scimap-2.0.4/scimap/plotting/heatmap.py
+-rw-r--r--   0        0        0     9552 2024-04-02 18:18:20.000000 scimap-2.0.4/scimap/plotting/image_viewer.py
+-rw-r--r--   0        0        0    10417 2024-03-18 18:24:52.000000 scimap-2.0.4/scimap/plotting/markerCorrelation.py
+-rw-r--r--   0        0        0     7419 2024-03-02 01:59:15.000000 scimap-2.0.4/scimap/plotting/pie.py
+-rw-r--r--   0        0        0    10165 2024-03-19 01:23:30.000000 scimap-2.0.4/scimap/plotting/spatial_distance.py
+-rw-r--r--   0        0        0    11795 2024-03-19 12:21:07.000000 scimap-2.0.4/scimap/plotting/spatial_interaction.py
+-rw-r--r--   0        0        0     5060 2024-03-19 19:10:54.000000 scimap-2.0.4/scimap/plotting/spatial_pscore.py
+-rw-r--r--   0        0        0    12601 2024-03-17 15:26:02.000000 scimap-2.0.4/scimap/plotting/spatial_scatterPlot.py
+-rw-r--r--   0        0        0    12242 2024-03-19 18:32:03.000000 scimap-2.0.4/scimap/plotting/spatialInteractionNetwork.py
+-rw-r--r--   0        0        0     7727 2024-03-02 01:58:34.000000 scimap-2.0.4/scimap/plotting/stacked_barplot.py
+-rw-r--r--   0        0        0    12547 2024-03-18 18:34:47.000000 scimap-2.0.4/scimap/plotting/umap.py
+-rw-r--r--   0        0        0    18847 2024-03-02 01:58:10.000000 scimap-2.0.4/scimap/plotting/voronoi.py
+-rw-r--r--   0        0        0      129 2024-03-17 18:13:28.000000 scimap-2.0.4/scimap/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4929 2024-03-01 22:07:39.000000 scimap-2.0.4/scimap/preprocessing/combat.py
+-rw-r--r--   0        0        0     3979 2024-03-17 19:14:56.000000 scimap-2.0.4/scimap/preprocessing/log1p.py
+-rw-r--r--   0        0        0    11153 2024-03-13 21:27:02.666498 scimap-2.0.4/scimap/preprocessing/mcmicro_to_scimap.py
+-rw-r--r--   0        0        0     3642 2024-03-18 00:27:18.000000 scimap-2.0.4/scimap/preprocessing/ngraph.py
+-rw-r--r--   0        0        0    17838 2024-02-29 22:11:30.000000 scimap-2.0.4/scimap/preprocessing/rescale.py
+-rw-r--r--   0        0        0  2003213 2021-07-01 20:47:33.000000 scimap-2.0.4/scimap/tests/_data/example_data.csv
+-rw-r--r--   0        0        0  1590001 2021-07-01 20:47:33.000000 scimap-2.0.4/scimap/tests/_data/example_data.h5ad
+-rw-r--r--   0        0        0     1908 2021-07-01 20:47:33.000000 scimap-2.0.4/scimap/tests/_data/phenotype_workflow.csv
+-rw-r--r--   0        0        0     1265 2024-03-02 02:51:31.000000 scimap-2.0.4/scimap/tests/test_helpers.py
+-rw-r--r--   0        0        0      982 2024-03-02 02:50:46.000000 scimap-2.0.4/scimap/tests/test_preprocessing.py
+-rw-r--r--   0        0        0     4675 2024-03-02 02:49:28.000000 scimap-2.0.4/scimap/tests/test_tools.py
+-rw-r--r--   0        0        0      568 2024-03-02 02:44:25.000000 scimap-2.0.4/scimap/tools/__init__.py
+-rw-r--r--   0        0        0    20200 2024-03-19 23:48:54.000000 scimap-2.0.4/scimap/tools/cluster.py
+-rw-r--r--   0        0        0    10598 2024-03-18 21:08:47.000000 scimap-2.0.4/scimap/tools/foldchange.py
+-rw-r--r--   0        0        0    18754 2024-03-01 13:54:09.000000 scimap-2.0.4/scimap/tools/phenotype_cells.py
+-rw-r--r--   0        0        0    12714 2024-03-19 20:32:33.000000 scimap-2.0.4/scimap/tools/spatial_aggregate.py
+-rw-r--r--   0        0        0     8731 2024-03-02 03:07:59.000000 scimap-2.0.4/scimap/tools/spatial_cluster.py
+-rw-r--r--   0        0        0     9097 2024-03-19 23:43:08.000000 scimap-2.0.4/scimap/tools/spatial_count.py
+-rw-r--r--   0        0        0     6224 2024-03-01 14:13:55.000000 scimap-2.0.4/scimap/tools/spatial_distance.py
+-rw-r--r--   0        0        0    13752 2024-03-20 01:28:34.000000 scimap-2.0.4/scimap/tools/spatial_expression.py
+-rw-r--r--   0        0        0    12059 2024-03-19 12:11:34.000000 scimap-2.0.4/scimap/tools/spatial_interaction.py
+-rw-r--r--   0        0        0    11333 2024-03-01 18:59:27.000000 scimap-2.0.4/scimap/tools/spatial_lda.py
+-rw-r--r--   0        0        0    12452 2024-03-19 18:49:22.000000 scimap-2.0.4/scimap/tools/spatial_pscore.py
+-rw-r--r--   0        0        0    18461 2024-03-19 21:36:08.000000 scimap-2.0.4/scimap/tools/spatial_similarity_search.py
+-rw-r--r--   0        0        0     3830 2024-03-01 19:23:35.000000 scimap-2.0.4/scimap/tools/umap.py
+-rw-r--r--   0        0        0     5053 1970-01-01 00:00:00.000000 scimap-2.0.4/PKG-INFO
```

### Comparing `scimap-2.0.3/LICENSE` & `scimap-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/README.md` & `scimap-2.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -24,26 +24,28 @@
 # If you have conda installed
 conda create --name scimap python=3.10
 conda activate scimap
 ```
 
 Install `scimap` directly into an activated virtual environment:
   
-**By default, we recommend installing scimap alongside napari for visualization purposes. Please note that napari requires a GUI toolkit like PyQt. If you encounter any errors due to your operating system, you should install scimap and napari separately, following napari's documentation.**
+**Firstly, we suggest installing `scimap` and `napari` together to enable visualization out of the box. Keep in mind, `napari` needs a GUI toolkit, such as PyQt. If you run into any issues because of your computer's operating system, install `scimap` and `napari` separately by following the guidance in `napari's` documentation.**
+
+Here's how you can install both using pip:
 
 ```python
 pip install scimap[napari]
 ```
 
-**If installation fails due to pyqt6; install scimap without napari.**
+**If you encounter a problem with PyQt6 during the installation, you can install `scimap` alone first. Later on, if you find you need `napari`, you can go ahead and install it by itself.**
 
-```python
+To install just `scimap`:
 
+```python
 pip install scimap
-
 ```
 
 After installation, the package can be imported as:
 
 ```python
 $ python
 >>> import scimap as sm
```

### Comparing `scimap-2.0.3/pyproject.toml` & `scimap-2.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "SCIMAP"
-version = "2.0.3"
+version = "2.0.4"
 description = "Spatial Single-Cell Analysis Toolkit"
 
 license = "MIT"
 
 authors = ["Ajit Johnson Nirmal <ajitjohnson.n@gmail.com>"]
 
 readme = "README.md"
@@ -50,14 +50,15 @@
 gensim = "^4.3.2"
 mkdocs-material = "^9.4.8"
 napari-ome-zarr = {version = "^0.4.0", optional = true}
 llvmlite = "^0.41.1"
 combat = "^0.3.3"
 mpl-scatter-density = "^0.7"
 pyqt6 = {version = "^6.6.1", optional = true}
+scikit-learn = "^1.4.2"
 
 [tool.poetry.extras]
 napari = ["pyqt6", "napari-ome-zarr", "napari"]
 
 [tool.poetry.dev-dependencies]
 
 # Formatters
```

### Comparing `scimap-2.0.3/scimap/cli/_scimap_mcmicro.py` & `scimap-2.0.4/scimap/cli/_scimap_mcmicro.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/cli/test.py` & `scimap-2.0.4/scimap/cli/test.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/helpers/_classify.py` & `scimap-2.0.4/scimap/helpers/_classify.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/helpers/addROI_omero.py` & `scimap-2.0.4/scimap/helpers/addROI_omero.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/helpers/add_roi_scatter.py` & `scimap-2.0.4/scimap/helpers/add_roi_scatter.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/helpers/animate.py` & `scimap-2.0.4/scimap/helpers/animate.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/helpers/classify.py` & `scimap-2.0.4/scimap/helpers/classify.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/helpers/downloadDemoData.py` & `scimap-2.0.4/scimap/helpers/downloadDemoData.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/helpers/dropFeatures.py` & `scimap-2.0.4/scimap/helpers/dropFeatures.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/helpers/merge_adata_obs.py` & `scimap-2.0.4/scimap/helpers/merge_adata_obs.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/helpers/rename.py` & `scimap-2.0.4/scimap/helpers/rename.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/helpers/scimap_to_csv.py` & `scimap-2.0.4/scimap/helpers/scimap_to_csv.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/__init__.py` & `scimap-2.0.4/scimap/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/addROI_image.py` & `scimap-2.0.4/scimap/plotting/addROI_image.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/cluster_plots.py` & `scimap-2.0.4/scimap/plotting/cluster_plots.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/densityPlot2D.py` & `scimap-2.0.4/scimap/plotting/densityPlot2D.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/distPlot.py` & `scimap-2.0.4/scimap/plotting/distPlot.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/foldchange.py` & `scimap-2.0.4/scimap/plotting/foldchange.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/gate_finder.py` & `scimap-2.0.4/scimap/plotting/gate_finder.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/groupCorrelation.py` & `scimap-2.0.4/scimap/plotting/groupCorrelation.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/heatmap.py` & `scimap-2.0.4/scimap/plotting/heatmap.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/image_viewer.py` & `scimap-2.0.4/scimap/plotting/image_viewer.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/markerCorrelation.py` & `scimap-2.0.4/scimap/plotting/markerCorrelation.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/pie.py` & `scimap-2.0.4/scimap/plotting/pie.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/spatialInteractionNetwork.py` & `scimap-2.0.4/scimap/plotting/spatialInteractionNetwork.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/spatial_distance.py` & `scimap-2.0.4/scimap/plotting/spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/spatial_interaction.py` & `scimap-2.0.4/scimap/plotting/spatial_interaction.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/spatial_pscore.py` & `scimap-2.0.4/scimap/plotting/spatial_pscore.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/spatial_scatterPlot.py` & `scimap-2.0.4/scimap/plotting/spatial_scatterPlot.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/stacked_barplot.py` & `scimap-2.0.4/scimap/plotting/stacked_barplot.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/umap.py` & `scimap-2.0.4/scimap/plotting/umap.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/plotting/voronoi.py` & `scimap-2.0.4/scimap/plotting/voronoi.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/preprocessing/combat.py` & `scimap-2.0.4/scimap/preprocessing/combat.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/preprocessing/log1p.py` & `scimap-2.0.4/scimap/preprocessing/log1p.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/preprocessing/mcmicro_to_scimap.py` & `scimap-2.0.4/scimap/preprocessing/mcmicro_to_scimap.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/preprocessing/ngraph.py` & `scimap-2.0.4/scimap/preprocessing/ngraph.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/preprocessing/rescale.py` & `scimap-2.0.4/scimap/preprocessing/rescale.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tests/_data/example_data.csv` & `scimap-2.0.4/scimap/tests/_data/example_data.csv`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tests/_data/example_data.h5ad` & `scimap-2.0.4/scimap/tests/_data/example_data.h5ad`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tests/_data/phenotype_workflow.csv` & `scimap-2.0.4/scimap/tests/_data/phenotype_workflow.csv`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tests/test_helpers.py` & `scimap-2.0.4/scimap/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tests/test_preprocessing.py` & `scimap-2.0.4/scimap/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tests/test_tools.py` & `scimap-2.0.4/scimap/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tools/__init__.py` & `scimap-2.0.4/scimap/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tools/cluster.py` & `scimap-2.0.4/scimap/tools/cluster.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tools/foldchange.py` & `scimap-2.0.4/scimap/tools/foldchange.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tools/phenotype_cells.py` & `scimap-2.0.4/scimap/tools/phenotype_cells.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tools/spatial_aggregate.py` & `scimap-2.0.4/scimap/tools/spatial_aggregate.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tools/spatial_cluster.py` & `scimap-2.0.4/scimap/tools/spatial_cluster.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tools/spatial_count.py` & `scimap-2.0.4/scimap/tools/spatial_count.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tools/spatial_distance.py` & `scimap-2.0.4/scimap/tools/spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tools/spatial_expression.py` & `scimap-2.0.4/scimap/tools/spatial_expression.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tools/spatial_interaction.py` & `scimap-2.0.4/scimap/tools/spatial_interaction.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tools/spatial_lda.py` & `scimap-2.0.4/scimap/tools/spatial_lda.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tools/spatial_pscore.py` & `scimap-2.0.4/scimap/tools/spatial_pscore.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tools/spatial_similarity_search.py` & `scimap-2.0.4/scimap/tools/spatial_similarity_search.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/scimap/tools/umap.py` & `scimap-2.0.4/scimap/tools/umap.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.3/PKG-INFO` & `scimap-2.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: scimap
-Version: 2.0.3
+Name: SCIMAP
+Version: 2.0.4
 Summary: Spatial Single-Cell Analysis Toolkit
 Home-page: https://pypi.org/project/scimap/
 License: MIT
 Keywords: image analysis,multiplex imaging,single cell analysis
 Author: Ajit Johnson Nirmal
 Author-email: ajitjohnson.n@gmail.com
 Requires-Python: >=3.9,<3.11
@@ -34,14 +34,15 @@
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: pandas (>=2.1.3,<3.0.0)
 Requires-Dist: plotly (>=5.18.0,<6.0.0)
 Requires-Dist: pyqt6 (>=6.6.1,<7.0.0) ; extra == "napari"
 Requires-Dist: pytest (>=7.4.3,<8.0.0)
 Requires-Dist: pytest-xvfb (>=3.0.0,<4.0.0)
 Requires-Dist: scanpy (>=1.9.6,<2.0.0)
+Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
 Requires-Dist: scipy (>=1.11.3,<2.0.0)
 Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Requires-Dist: shapely (>=2.0.2,<3.0.0)
 Requires-Dist: tifffile (>=2023.9.26,<2024.0.0)
 Requires-Dist: zarr (==2.10.3)
 Project-URL: Documentation, https://scimap.xyz
 Project-URL: Repository, https://github.com/labsyspharm/scimap
@@ -73,26 +74,28 @@
 # If you have conda installed
 conda create --name scimap python=3.10
 conda activate scimap
 ```
 
 Install `scimap` directly into an activated virtual environment:
   
-**By default, we recommend installing scimap alongside napari for visualization purposes. Please note that napari requires a GUI toolkit like PyQt. If you encounter any errors due to your operating system, you should install scimap and napari separately, following napari's documentation.**
+**Firstly, we suggest installing `scimap` and `napari` together to enable visualization out of the box. Keep in mind, `napari` needs a GUI toolkit, such as PyQt. If you run into any issues because of your computer's operating system, install `scimap` and `napari` separately by following the guidance in `napari's` documentation.**
+
+Here's how you can install both using pip:
 
 ```python
 pip install scimap[napari]
 ```
 
-**If installation fails due to pyqt6; install scimap without napari.**
+**If you encounter a problem with PyQt6 during the installation, you can install `scimap` alone first. Later on, if you find you need `napari`, you can go ahead and install it by itself.**
 
-```python
+To install just `scimap`:
 
+```python
 pip install scimap
-
 ```
 
 After installation, the package can be imported as:
 
 ```python
 $ python
 >>> import scimap as sm
```

