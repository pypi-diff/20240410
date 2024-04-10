# Comparing `tmp/spectrum_image-0.2.4.tar.gz` & `tmp/spectrum_image-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_image-0.2.4.tar", last modified: Thu Apr  4 05:05:48 2024, max compression
+gzip compressed data, was "spectrum_image-0.2.5.tar", last modified: Wed Apr 10 01:20:33 2024, max compression
```

## Comparing `spectrum_image-0.2.4.tar` & `spectrum_image-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-04 05:05:48.603479 spectrum_image-0.2.4/
--rw-r--r--   0 sung       (501) staff       (20)    35149 2024-03-12 18:53:01.000000 spectrum_image-0.2.4/LICENSE
--rw-r--r--   0 sung       (501) staff       (20)     1781 2024-04-04 05:05:48.603272 spectrum_image-0.2.4/PKG-INFO
--rw-r--r--   0 sung       (501) staff       (20)      977 2024-03-18 03:44:13.000000 spectrum_image-0.2.4/README.md
--rw-r--r--   0 sung       (501) staff       (20)      864 2024-04-04 05:05:39.000000 spectrum_image-0.2.4/pyproject.toml
--rw-r--r--   0 sung       (501) staff       (20)       38 2024-04-04 05:05:48.603521 spectrum_image-0.2.4/setup.cfg
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-04 05:05:48.599546 spectrum_image-0.2.4/src/
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-04 05:05:48.602400 spectrum_image-0.2.4/src/spectrum_image/
--rw-r--r--   0 sung       (501) staff       (20)    51585 2024-04-04 05:05:19.000000 spectrum_image-0.2.4/src/spectrum_image/SI.py
--rw-r--r--   0 sung       (501) staff       (20)    69473 2024-03-30 23:57:52.000000 spectrum_image-0.2.4/src/spectrum_image/SI_bckup.py
--rw-r--r--   0 sung       (501) staff       (20)     1466 2024-03-26 23:43:32.000000 spectrum_image-0.2.4/src/spectrum_image/SI_lineshapes.py
--rw-r--r--   0 sung       (501) staff       (20)     7832 2024-04-03 04:35:18.000000 spectrum_image-0.2.4/src/spectrum_image/SI_util.py
--rw-r--r--   0 sung       (501) staff       (20)      280 2024-03-12 18:53:01.000000 spectrum_image-0.2.4/src/spectrum_image/__init__.py
--rw-r--r--   0 sung       (501) staff       (20)    12873 2024-04-04 04:22:31.000000 spectrum_image-0.2.4/src/spectrum_image/eels_bgsub.py
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-04 05:05:48.603070 spectrum_image-0.2.4/src/spectrum_image.egg-info/
--rw-r--r--   0 sung       (501) staff       (20)     1781 2024-04-04 05:05:48.000000 spectrum_image-0.2.4/src/spectrum_image.egg-info/PKG-INFO
--rw-r--r--   0 sung       (501) staff       (20)      427 2024-04-04 05:05:48.000000 spectrum_image-0.2.4/src/spectrum_image.egg-info/SOURCES.txt
--rw-r--r--   0 sung       (501) staff       (20)        1 2024-04-04 05:05:48.000000 spectrum_image-0.2.4/src/spectrum_image.egg-info/dependency_links.txt
--rw-r--r--   0 sung       (501) staff       (20)       52 2024-04-04 05:05:48.000000 spectrum_image-0.2.4/src/spectrum_image.egg-info/requires.txt
--rw-r--r--   0 sung       (501) staff       (20)       15 2024-04-04 05:05:48.000000 spectrum_image-0.2.4/src/spectrum_image.egg-info/top_level.txt
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-10 01:20:33.590579 spectrum_image-0.2.5/
+-rw-r--r--   0 sung       (501) staff       (20)    35149 2024-03-12 18:53:01.000000 spectrum_image-0.2.5/LICENSE
+-rw-r--r--   0 sung       (501) staff       (20)     1726 2024-04-10 01:20:33.590388 spectrum_image-0.2.5/PKG-INFO
+-rw-r--r--   0 sung       (501) staff       (20)      922 2024-04-10 01:05:24.000000 spectrum_image-0.2.5/README.md
+-rw-r--r--   0 sung       (501) staff       (20)      863 2024-04-10 01:20:19.000000 spectrum_image-0.2.5/pyproject.toml
+-rw-r--r--   0 sung       (501) staff       (20)       38 2024-04-10 01:20:33.590622 spectrum_image-0.2.5/setup.cfg
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-10 01:20:33.587623 spectrum_image-0.2.5/src/
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-10 01:20:33.589444 spectrum_image-0.2.5/src/spectrum_image/
+-rw-r--r--   0 sung       (501) staff       (20)    51688 2024-04-10 01:11:02.000000 spectrum_image-0.2.5/src/spectrum_image/EELS.py
+-rw-r--r--   0 sung       (501) staff       (20)     1466 2024-03-26 23:43:32.000000 spectrum_image-0.2.5/src/spectrum_image/EELS_lineshapes.py
+-rw-r--r--   0 sung       (501) staff       (20)    12298 2024-04-10 01:08:18.000000 spectrum_image-0.2.5/src/spectrum_image/EELS_util.py
+-rw-r--r--   0 sung       (501) staff       (20)    28413 2024-04-04 21:13:52.000000 spectrum_image-0.2.5/src/spectrum_image/RIXS.py
+-rw-r--r--   0 sung       (501) staff       (20)    69473 2024-03-30 23:57:52.000000 spectrum_image-0.2.5/src/spectrum_image/SI_bckup.py
+-rw-r--r--   0 sung       (501) staff       (20)      280 2024-03-12 18:53:01.000000 spectrum_image-0.2.5/src/spectrum_image/__init__.py
+-rw-r--r--   0 sung       (501) staff       (20)    13294 2024-04-07 21:36:17.000000 spectrum_image-0.2.5/src/spectrum_image/eels_bgsub.py
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-10 01:20:33.590197 spectrum_image-0.2.5/src/spectrum_image.egg-info/
+-rw-r--r--   0 sung       (501) staff       (20)     1726 2024-04-10 01:20:33.000000 spectrum_image-0.2.5/src/spectrum_image.egg-info/PKG-INFO
+-rw-r--r--   0 sung       (501) staff       (20)      460 2024-04-10 01:20:33.000000 spectrum_image-0.2.5/src/spectrum_image.egg-info/SOURCES.txt
+-rw-r--r--   0 sung       (501) staff       (20)        1 2024-04-10 01:20:33.000000 spectrum_image-0.2.5/src/spectrum_image.egg-info/dependency_links.txt
+-rw-r--r--   0 sung       (501) staff       (20)       52 2024-04-10 01:20:33.000000 spectrum_image-0.2.5/src/spectrum_image.egg-info/requires.txt
+-rw-r--r--   0 sung       (501) staff       (20)       15 2024-04-10 01:20:33.000000 spectrum_image-0.2.5/src/spectrum_image.egg-info/top_level.txt
```

### Comparing `spectrum_image-0.2.4/LICENSE` & `spectrum_image-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2.4/PKG-INFO` & `spectrum_image-0.2.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: spectrum_image
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python Package for EELS (Electron Energy Loss Spectroscopy) Analysis
 Author-email: Suk Hyun Sung <sukhsung@umich.edu>
-Project-URL: Homepage, https://github.com/sukhsung/spectrum_image
-Project-URL: Repository, https://github.com/sukhsung/spectrum_image
-Project-URL: Bug Tracker, https://github.com/sukhsung/spectrum_image/issues
+Project-URL: Homepage, https://github.com/sukhsung/spectrum-image
+Project-URL: Repository, https://github.com/sukhsung/spectrum-image
+Project-URL: Bug Tracker, https://github.com/sukhsung/spectrum-image/issues
 Keywords: Electron Microscopy,EELS,TEM,STEM,Electron Energy Loss Spectroscopy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -38,14 +38,12 @@
 `matplotlib`
 `jupyterlab`
 `ipympl`
 `scipy`
 `tqdm`
 `numpy`
 `lmfit`
-
-## Optional Dependencies for running example notebook
 `hyperspy`
 `tifffile`
 
 ## Acknowledgements
 Some functionalities (background subtraction, local background averaging) was copied from eels.py of https://github.com/paradimdata/Cornell_EM_SummerSchool_2021/tree/main/Tutorial%204%20-%20Spectroscopy
```

### Comparing `spectrum_image-0.2.4/pyproject.toml` & `spectrum_image-0.2.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [build-system]
 requires = ["setuptools>=69"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spectrum_image"
-version = "0.2.4"
+version = "0.2.5"
 dependencies = [
   "numpy",
   "matplotlib",
   "jupyterlab",
   "ipympl",
   "scipy",
   "tqdm",
   "lmfit"
 ]
 requires-python = ">=3.10"
 authors = [
-  {name = "Suk Hyun Sung", email = "sukhsung@umich.edu"},
+  {name = "Suk Hyun Sung", email = "sukhsung@umich.edu"}
 ]
 description = "Python Package for EELS (Electron Energy Loss Spectroscopy) Analysis"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 keywords = ["Electron Microscopy", "EELS", "TEM", "STEM", "Electron Energy Loss Spectroscopy"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Programming Language :: Python"
 ]
 
 [project.urls]
-Homepage = "https://github.com/sukhsung/spectrum_image"
-Repository = "https://github.com/sukhsung/spectrum_image"
-"Bug Tracker" = "https://github.com/sukhsung/spectrum_image/issues"
+Homepage = "https://github.com/sukhsung/spectrum-image"
+Repository = "https://github.com/sukhsung/spectrum-image"
+"Bug Tracker" = "https://github.com/sukhsung/spectrum-image/issues"
```

### Comparing `spectrum_image-0.2.4/src/spectrum_image/SI.py` & `spectrum_image-0.2.5/src/spectrum_image/EELS.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,31 +70,32 @@
         self.fig=plt.figure(figsize=figsize,layout='constrained')
 
         self.ax = {}
         self.ax['inel']=self.fig.add_axes([0.025,0.1,0.45,0.8]) # Image
         self.ax['spec']=self.fig.add_axes([0.525,0.45,0.45,0.45]) # Spectrum
         self.ax['spec2'] = self.fig.add_axes([0.525,0.45,0.45,0.20]) # Spec 2
         self.ax['ck_ysetting'] = self.fig.add_axes([0.85,0.89,0.13,0.07]) # Y-lock chkbox
-        self.ax['ck_roi2'] = self.fig.add_axes([0.025,0.10,0.15,0.05]) # ROI2 chkbox
-        self.ax['ck_adf'] = self.fig.add_axes([0.18,0.10,0.15,0.05]) # adf chkbox
+        self.ax['ck_roi2'] = self.fig.add_axes([0.025,0.0,0.15,0.05]) # ROI2 chkbox
+        if self.adf is not None:
+            self.ax['ck_adf'] = self.fig.add_axes([0.18,0.0,0.15,0.05]) # adf chkbox
         self.ax['e_view']=self.fig.add_axes([0.625,0.30,0.25,0.05]) # Range slider
         self.ax['e_bsub']=self.fig.add_axes([0.625,0.25,0.25,0.05]) # Range slider
         self.ax['e_int'] =self.fig.add_axes([0.625,0.20,0.25,0.05]) # Range slider
         self.ax['btn_fit']=self.fig.add_axes([0.520,0.1,0.125,0.1]) # Fit Buttons
         self.ax['btn_fbsub']=self.fig.add_axes([0.655,0.1,0.1,0.1]) # Fast Int Button
         self.ax['btn_bsub']=self.fig.add_axes([0.765,0.1,0.1,0.1]) # Int Button 
         self.ax['ck_fit']=self.fig.add_axes([0.875,0.1,0.1,0.1]) # Axis for Fit settings
 
         self.ax['lc_tx'] = self.fig.add_axes([0.875,0.06,0.1,0.025]) # LC settings
         self.ax['lba_tx'] = self.fig.add_axes([0.875,0.03,0.1,0.025]) # LBA settings
 
         ## Initialize plot handles
         self.h = {}
         ################## ax['inel'] ######################
-        self.h['inel'] = self.ax['inel'].imshow( self.im_inel,cmap = cmap)
+        self.h['inel'] = self.ax['inel'].matshow( self.im_inel,cmap = cmap)
         self.ax['inel'].set_axis_off()
         self.ax['inel'].set_title('Inelastic image')
 
         ################## ax['spec'] #######################
         self.h['spec1'], =self.ax['spec'].plot(self.energy, self.spectrum1,color='crimson')
         self.h['bsub1'], =self.ax['spec'].plot(self.energy, self.bsub1,color='k',alpha=0)
         self.h['fit1'],  =self.ax['spec'].plot(self.energy, self.bsub1_fit,color='palevioletred',alpha=0)
@@ -133,17 +134,18 @@
         self.ui['ck_fit'].on_clicked( lambda v: self.onclick_ck_fit() )
 
         self.ui['ck_roi2'] = CheckButtons(ax=self.ax['ck_roi2'], labels= ["Enable ROI 2"],
                                         actives=[False], check_props={'facecolor': 'k'} )
         self.ui['ck_roi2'].on_clicked( lambda v: self.onclick_ck_roi2() )
         self.roi2_enabled = False
 
-        self.ui['ck_adf'] = CheckButtons(ax=self.ax['ck_adf'], labels= ["Toggle ADF"],
-                                        actives=[False], check_props={'facecolor': 'k'} )
-        self.ui['ck_adf'].on_clicked( lambda v: self.onclick_ck_adf() )
+        if self.adf is not None:
+            self.ui['ck_adf'] = CheckButtons(ax=self.ax['ck_adf'], labels= ["Toggle ADF"],
+                                            actives=[False], check_props={'facecolor': 'k'} )
+            self.ui['ck_adf'].on_clicked( lambda v: self.onclick_ck_adf() )
         self.adf_enabled = False
 
 
         self.ui['lc_tx'] = TextBox(self.ax['lc_tx'], "LC: ", textalignment="left")
         self.ui['lc_tx'].on_submit( self.onchange_lc )
         self.ui['lc_tx'].set_val( '(5, 95)')
         self.ui['lc_tx'].set_active( False )
@@ -442,15 +444,15 @@
                     if self.fit_check:
                         minval = min( 0.9*self.bsub2[slidermin:slidermax].min(),
                                     0)
                 else:
                     maxval =  1.2*self.spectrum2[slidermin:slidermax].max()
                     minval =  0.8*self.spectrum2[slidermin:slidermax].min()
 
-                    self.ax['spec2'].set_ylim([minval,maxval])
+                self.ax['spec2'].set_ylim([minval,maxval])
 
 
     ############### Event Handlers ###################
     def onclick_figure( self, event ):
         if event.inaxes in [self.ax['inel']]:
             if event.button == MouseButton.LEFT:
                 # Left Click on Inelastic Image
@@ -592,15 +594,15 @@
         self.ax['ck_ysetting'] = self.fig.add_axes([0.85,0.89,0.13,0.07]) # Y-lock chkbox
         self.ax['ck_roi2'] = self.fig.add_axes([0.025,0.10,0.15,0.05]) # ROI2 chkbox
         self.ax['e_view']=self.fig.add_axes([0.625,0.30,0.25,0.05]) # Range slider
 
         ## Initialize plot handles
         self.h = {}
         ################## ax['inel'] ######################
-        self.h['inel'] = self.ax['inel'].imshow( self.im_inel,cmap = cmap,origin='lower' )
+        self.h['inel'] = self.ax['inel'].matshow( self.im_inel,cmap = cmap,aspect=self.ny/self.ne ,origin='lower')
         self.ax['inel'].set_axis_off()
         self.ax['inel'].set_title('Inelastic image')
 
         ################## ax['spec'] #######################
         self.h['spec1'], =self.ax['spec'].plot(self.energy, self.spectrum1,color='crimson')
         self.ax['spec'].axhline(0,color='k',linestyle='--',alpha=0.3)
         self.ax['spec'].set_ylim([self.spectrum1.min(),self.spectrum1.max()])
@@ -657,14 +659,15 @@
         
 
         self.fig.canvas.mpl_connect( 'motion_notify_event', 
                                     lambda event: self.onclick_figure_browser(event))
 
 
         self.rescale_yrange()
+
         # return results_dict,selector_collection
 
     def onclick_figure_browser( self, event ):
         if event.inaxes in [self.ax['inel']]:
             if event.button == MouseButton.LEFT:
                 # Left Click on Inelastic Image
                 self.update_spectrum1()
@@ -726,15 +729,15 @@
 
         self.ax['lc_tx'] = self.fig.add_axes([0.875,0.06,0.1,0.025]) # LC settings
         self.ax['lba_tx'] = self.fig.add_axes([0.875,0.03,0.1,0.025]) # LBA settings
 
         ## Initialize plot handles
         self.h = {}
         ################## ax['inel'] ######################
-        self.h['inel'] = self.ax['inel'].imshow( self.im_inel,cmap = cmap,origin='lower' )
+        self.h['inel'] = self.ax['inel'].matshow( self.im_inel,cmap = cmap,origin='lower' )
         self.ax['inel'].set_axis_off()
         self.ax['inel'].set_title('Inelastic image')
 
         ################## ax['spec'] #######################
         self.h['spec1'], =self.ax['spec'].plot(self.energy, self.spectrum1,color='crimson')
         self.h['bsub1'], =self.ax['spec'].plot(self.energy, self.bsub1,color='k',alpha=0)
         self.h['fit1'],  =self.ax['spec'].plot(self.energy, self.bsub1_fit,color='palevioletred',alpha=0)
```

### Comparing `spectrum_image-0.2.4/src/spectrum_image/SI_bckup.py` & `spectrum_image-0.2.5/src/spectrum_image/SI_bckup.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2.4/src/spectrum_image/SI_lineshapes.py` & `spectrum_image-0.2.5/src/spectrum_image/EELS_lineshapes.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2.4/src/spectrum_image/eels_bgsub.py` & `spectrum_image-0.2.5/src/spectrum_image/eels_bgsub.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,15 +150,21 @@
     For Y = Ax + b + error with fixed 'A':
         Y' = b + error. MSE is minimized when b = mean(Y)
     """
     ### Load Fit Options
     if (fit_options is None):
         fit_options = options_bgsub()
 
-    xdim, ydim, zdim = np.shape( si )
+    if len(np.shape(si)) == 2:
+        tempx,tempz = np.shape(si)
+        si = np.reshape(si,(tempx,1,tempz))
+    if len(np.shape(si)) == 1:
+        tempz = len(si)
+        si = np.reshape(si,(1,1,tempz))
+    xdim, ydim, zdim = np.shape(si)
 
     fit_start_ch, fit_end_ch = np.searchsorted(energy, edge.e_bsub)
     y_win = si[:,:,fit_start_ch:fit_end_ch]
     e_win = np.reshape( energy[fit_start_ch:fit_end_ch], (1,1,(fit_end_ch-fit_start_ch)) )
     e_sub = np.reshape( energy[fit_start_ch:], (1,1,zdim-fit_start_ch) )
 
     bg_SI = np.zeros_like( si )  
@@ -172,15 +178,15 @@
         y_fit = np.exp( c_fit + rval*np.log(e_sub) )
 
     if fit_options.fit == 'exp':
         c_fit = np.reshape( np.mean( np.log(y_win)-rval*e_win, axis=(2)), (xdim,ydim,1))
         y_fit = np.exp( c_fit + rval*e_sub )
 
     bg_SI[:,:,fit_start_ch:] = si[:,:,fit_start_ch:] - y_fit
-    return bg_SI
+    return np.squeeze(bg_SI)
 
 def bgsub_SI_linearized( si, energy, edge, fit_options=None):
     """
     Quick background subtraction based on fixed 'r' value
     For Y = Ax + b + error with fixed 'A':
         Y' = b + error. MSE is minimized when b = mean(Y)
     """
@@ -191,14 +197,21 @@
     fit_start_ch, fit_end_ch = np.searchsorted(energy, edge.e_bsub)
     if (fit_end_ch - fit_start_ch)<2:
         fit_end_ch = fit_start_ch+2
     e_win = np.atleast_2d( energy[fit_start_ch:fit_end_ch] ).T
     e_sub = np.atleast_2d( energy[fit_start_ch:] ).T
     zdim = len(energy)
 
+    if len(np.shape(si)) == 2:
+        tempx,tempz = np.shape(si)
+        si = np.reshape(si,(tempx,1,tempz))
+    if len(np.shape(si)) == 1:
+        tempz = len(si)
+        si = np.reshape(si,(1,1,tempz))
+
     xdim, ydim, zdim = np.shape( si )
     y_win = si[:,:,fit_start_ch:fit_end_ch]
     y_win = np.reshape( y_win, (xdim*ydim, len(e_win))).T
 
     bg_SI = np.zeros_like( si )  
     if fit_options.fit == 'lin':
         e_win = np.insert( e_win, 0, 1, axis=1)
```

### Comparing `spectrum_image-0.2.4/src/spectrum_image.egg-info/PKG-INFO` & `spectrum_image-0.2.5/src/spectrum_image.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: spectrum_image
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python Package for EELS (Electron Energy Loss Spectroscopy) Analysis
 Author-email: Suk Hyun Sung <sukhsung@umich.edu>
-Project-URL: Homepage, https://github.com/sukhsung/spectrum_image
-Project-URL: Repository, https://github.com/sukhsung/spectrum_image
-Project-URL: Bug Tracker, https://github.com/sukhsung/spectrum_image/issues
+Project-URL: Homepage, https://github.com/sukhsung/spectrum-image
+Project-URL: Repository, https://github.com/sukhsung/spectrum-image
+Project-URL: Bug Tracker, https://github.com/sukhsung/spectrum-image/issues
 Keywords: Electron Microscopy,EELS,TEM,STEM,Electron Energy Loss Spectroscopy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -38,14 +38,12 @@
 `matplotlib`
 `jupyterlab`
 `ipympl`
 `scipy`
 `tqdm`
 `numpy`
 `lmfit`
-
-## Optional Dependencies for running example notebook
 `hyperspy`
 `tifffile`
 
 ## Acknowledgements
 Some functionalities (background subtraction, local background averaging) was copied from eels.py of https://github.com/paradimdata/Cornell_EM_SummerSchool_2021/tree/main/Tutorial%204%20-%20Spectroscopy
```

