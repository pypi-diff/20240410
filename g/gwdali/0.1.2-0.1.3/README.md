# Comparing `tmp/gwdali-0.1.2.tar.gz` & `tmp/gwdali-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdali-0.1.2.tar", last modified: Wed Feb 28 20:00:41 2024, max compression
+gzip compressed data, was "gwdali-0.1.3.tar", last modified: Wed Apr 10 15:32:32 2024, max compression
```

## Comparing `gwdali-0.1.2.tar` & `gwdali-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-02-28 20:00:41.721552 gwdali-0.1.2/
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-02-28 20:00:41.717553 gwdali-0.1.2/GWDALI/
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-02-28 20:00:41.721552 gwdali-0.1.2/GWDALI/Detectors_Sensitivity/
--rwxrwxr-x   0 josiel    (1000) josiel    (1000)    78018 2024-02-12 16:14:07.000000 gwdali-0.1.2/GWDALI/Detectors_Sensitivity/Sn_CE.txt
--rwxrwxr-x   0 josiel    (1000) josiel    (1000)    78021 2024-02-12 16:14:07.000000 gwdali-0.1.2/GWDALI/Detectors_Sensitivity/Sn_ET.txt
--rwxrwxr-x   0 josiel    (1000) josiel    (1000)    83058 2024-02-12 16:14:07.000000 gwdali-0.1.2/GWDALI/Detectors_Sensitivity/Sn_K.txt
--rwxrwxr-x   0 josiel    (1000) josiel    (1000)    56323 2024-02-12 16:14:07.000000 gwdali-0.1.2/GWDALI/Detectors_Sensitivity/Sn_L.txt
--rwxrwxr-x   0 josiel    (1000) josiel    (1000)    84000 2024-02-12 16:14:07.000000 gwdali-0.1.2/GWDALI/Detectors_Sensitivity/Sn_V.txt
--rw-rw-r--   0 josiel    (1000) josiel    (1000)       14 2024-02-12 16:14:07.000000 gwdali-0.1.2/GWDALI/Detectors_Sensitivity/__init__.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)      921 2024-02-12 16:14:07.000000 gwdali-0.1.2/GWDALI/Detectors_Sensitivity/plot_Sn.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     6775 2024-02-28 19:45:58.000000 gwdali-0.1.2/GWDALI/GWDALI.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)      143 2024-02-12 16:14:07.000000 gwdali-0.1.2/GWDALI/__init__.py
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-02-28 20:00:41.721552 gwdali-0.1.2/GWDALI/lib/
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     3080 2024-02-12 16:14:07.000000 gwdali-0.1.2/GWDALI/lib/Angles_lib.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     4429 2024-02-28 18:56:54.000000 gwdali-0.1.2/GWDALI/lib/Auxiliar.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     5858 2024-02-12 16:14:07.000000 gwdali-0.1.2/GWDALI/lib/Corner_Plots.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     2685 2024-02-12 16:14:07.000000 gwdali-0.1.2/GWDALI/lib/Dictionaries.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     7867 2024-02-28 19:57:38.000000 gwdali-0.1.2/GWDALI/lib/Diff_Signal_Tensors.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     4274 2024-02-28 19:45:01.000000 gwdali-0.1.2/GWDALI/lib/Get_Tensors.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     7382 2024-02-28 19:57:19.000000 gwdali-0.1.2/GWDALI/lib/Likelihood.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     4305 2024-02-12 16:14:07.000000 gwdali-0.1.2/GWDALI/lib/Waveforms.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)      145 2024-02-12 16:14:07.000000 gwdali-0.1.2/GWDALI/lib/__init__.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     1519 2024-02-07 21:23:28.000000 gwdali-0.1.2/LICENSE
--rw-r--r--   0 josiel    (1000) josiel    (1000)     5178 2024-02-28 20:00:41.721552 gwdali-0.1.2/PKG-INFO
--rw-r--r--   0 josiel    (1000) josiel    (1000)     4822 2023-07-17 17:42:50.000000 gwdali-0.1.2/README.md
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-02-28 20:00:41.721552 gwdali-0.1.2/gwdali.egg-info/
--rw-r--r--   0 josiel    (1000) josiel    (1000)     5178 2024-02-28 20:00:41.000000 gwdali-0.1.2/gwdali.egg-info/PKG-INFO
--rw-r--r--   0 josiel    (1000) josiel    (1000)      689 2024-02-28 20:00:41.000000 gwdali-0.1.2/gwdali.egg-info/SOURCES.txt
--rw-r--r--   0 josiel    (1000) josiel    (1000)        1 2024-02-28 20:00:41.000000 gwdali-0.1.2/gwdali.egg-info/dependency_links.txt
--rw-r--r--   0 josiel    (1000) josiel    (1000)        7 2024-02-28 20:00:41.000000 gwdali-0.1.2/gwdali.egg-info/top_level.txt
--rw-rw-r--   0 josiel    (1000) josiel    (1000)       38 2024-02-28 20:00:41.721552 gwdali-0.1.2/setup.cfg
--rw-r--r--   0 josiel    (1000) josiel    (1000)      767 2024-02-28 19:59:12.000000 gwdali-0.1.2/setup.py
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-04-10 15:32:32.466494 gwdali-0.1.3/
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-04-10 15:32:32.454492 gwdali-0.1.3/GWDALI/
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-04-10 15:32:32.462494 gwdali-0.1.3/GWDALI/Detectors_Sensitivity/
+-rwxrwxr-x   0 josiel    (1000) josiel    (1000)    78018 2024-02-12 16:14:07.000000 gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_CE.txt
+-rwxrwxr-x   0 josiel    (1000) josiel    (1000)    78021 2024-02-12 16:14:07.000000 gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_ET.txt
+-rwxrwxr-x   0 josiel    (1000) josiel    (1000)    83058 2024-02-12 16:14:07.000000 gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_K.txt
+-rwxrwxr-x   0 josiel    (1000) josiel    (1000)    56323 2024-02-12 16:14:07.000000 gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_L.txt
+-rwxrwxr-x   0 josiel    (1000) josiel    (1000)    84000 2024-02-12 16:14:07.000000 gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_V.txt
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)       14 2024-02-12 16:14:07.000000 gwdali-0.1.3/GWDALI/Detectors_Sensitivity/__init__.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)      921 2024-02-12 16:14:07.000000 gwdali-0.1.3/GWDALI/Detectors_Sensitivity/plot_Sn.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     6741 2024-03-08 17:26:00.000000 gwdali-0.1.3/GWDALI/GWDALI.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)      143 2024-02-12 16:14:07.000000 gwdali-0.1.3/GWDALI/__init__.py
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-04-10 15:32:32.466494 gwdali-0.1.3/GWDALI/lib/
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     3381 2024-03-07 16:18:03.000000 gwdali-0.1.3/GWDALI/lib/Angles_lib.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     4429 2024-02-29 14:02:42.000000 gwdali-0.1.3/GWDALI/lib/Auxiliar.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     5858 2024-02-29 14:02:42.000000 gwdali-0.1.3/GWDALI/lib/Corner_Plots.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     2685 2024-02-29 14:02:42.000000 gwdali-0.1.3/GWDALI/lib/Dictionaries.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     8866 2024-04-10 14:58:57.000000 gwdali-0.1.3/GWDALI/lib/Diff_Signal_Tensors.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     4303 2024-03-08 17:28:57.000000 gwdali-0.1.3/GWDALI/lib/Get_Tensors.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     8245 2024-04-09 20:19:01.000000 gwdali-0.1.3/GWDALI/lib/Likelihood.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     4181 2024-04-09 19:50:18.000000 gwdali-0.1.3/GWDALI/lib/Waveforms.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)      145 2024-02-29 14:02:42.000000 gwdali-0.1.3/GWDALI/lib/__init__.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     1519 2024-02-07 21:23:28.000000 gwdali-0.1.3/LICENSE
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     5178 2024-04-10 15:32:32.466494 gwdali-0.1.3/PKG-INFO
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     4822 2023-07-17 17:42:50.000000 gwdali-0.1.3/README.md
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-04-10 15:32:32.466494 gwdali-0.1.3/gwdali.egg-info/
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     5178 2024-04-10 15:32:32.000000 gwdali-0.1.3/gwdali.egg-info/PKG-INFO
+-rw-r--r--   0 josiel    (1000) josiel    (1000)      689 2024-04-10 15:32:32.000000 gwdali-0.1.3/gwdali.egg-info/SOURCES.txt
+-rw-r--r--   0 josiel    (1000) josiel    (1000)        1 2024-04-10 15:32:32.000000 gwdali-0.1.3/gwdali.egg-info/dependency_links.txt
+-rw-r--r--   0 josiel    (1000) josiel    (1000)        7 2024-04-10 15:32:32.000000 gwdali-0.1.3/gwdali.egg-info/top_level.txt
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)       38 2024-04-10 15:32:32.466494 gwdali-0.1.3/setup.cfg
+-rw-r--r--   0 josiel    (1000) josiel    (1000)      767 2024-04-10 15:31:33.000000 gwdali-0.1.3/setup.py
```

### Comparing `gwdali-0.1.2/GWDALI/Detectors_Sensitivity/Sn_CE.txt` & `gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_CE.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.2/GWDALI/Detectors_Sensitivity/Sn_ET.txt` & `gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_ET.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.2/GWDALI/Detectors_Sensitivity/Sn_K.txt` & `gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_K.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.2/GWDALI/Detectors_Sensitivity/Sn_L.txt` & `gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_L.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.2/GWDALI/Detectors_Sensitivity/Sn_V.txt` & `gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_V.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.2/GWDALI/Detectors_Sensitivity/plot_Sn.py` & `gwdali-0.1.3/GWDALI/Detectors_Sensitivity/plot_Sn.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.2/GWDALI/GWDALI.py` & `gwdali-0.1.3/GWDALI/GWDALI.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import matplotlib.pyplot as plt
 import os, shutil, sys
 import warnings ; warnings.filterwarnings("ignore")
 #===========================
 #----Internal_libs----------
 #===========================
 import GWDALI.lib.Waveforms as wf
-import GWDALI.lib.Angles_lib as geo
 import GWDALI.lib.Dictionaries as gwdict
 import GWDALI.lib.Diff_Signal_Tensors as gwfunc
 import GWDALI.lib.Corner_Plots as corner
 import GWDALI.lib.Auxiliar as Aux
 from .lib.Likelihood import get_posterior
 from .lib.Get_Tensors import Get_Tensors
 #===========================
@@ -54,25 +53,25 @@
 	return Sn0, freq0
 
 def get_strain_snr(gw_prms,detectors,approximant='TaylorF2',fmin=1.,fmax=1.e4,fsize=3.e3):
 	Strains, SNR = [], []
 	rho2 = 0
 
 	freq = 10**np.linspace(np.log10(fmin), np.log10(fmax), int(fsize))
+	det_a = detectors[0]
 	for idx in range(len(detectors)):
-		det = detectors[idx]
-		Sn0, freq0 = get_Sn(det)
+		det_b = detectors[idx]
+		Sn0, freq0 = get_Sn(det_b)
 		func_Sn = interp1d(freq0,Sn0,fill_value=np.inf,bounds_error=False)
-		detectors[idx]['freq'] = freq
-		detectors[idx]['Sn']   = func_Sn(freq)
+		det_b['freq'] = freq
+		det_b['Sn']   = func_Sn(freq)
 
-		h 	  = gwfunc.Signal(gw_prms, det, approximant)
-		SNR2  = gwfunc.ScalarProduct(det['freq'], det['Sn'],h,h)
+		h 	  = gwfunc.Signal(gw_prms, [det_a, det_b], approximant)
+		SNR2  = gwfunc.ScalarProduct(det_b['freq'], det_b['Sn'],h,h)
 		rho2 += SNR2
-		#print('#####'*10)
 		Strains.append(h)
 		SNR.append(np.sqrt(SNR2))
 
 	hp, hx, freq = gwfunc.GW_Polarizations(gw_prms,freq, approximant)
 
 	return [hp,hx,freq], Strains, SNR, np.sqrt(rho2)
 #-------------------------------------------------------
```

### Comparing `gwdali-0.1.2/GWDALI/lib/Angles_lib.py` & `gwdali-0.1.3/GWDALI/lib/Angles_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,8 +78,22 @@
 def ObsAngles(alpha0,beta0,iota,psi0,lon,lat,rot):
 	phi   = lon*np.pi/180
 	theta = (90-lat)*np.pi/180
 	ksi   = rot*np.pi/180
 
 	alpha_obs, beta_obs = AngTransf(alpha0,beta0,theta,phi,ksi)
 	psi_obs = poll_ang(alpha0,beta0,iota,psi0,theta,phi,ksi)
-	return alpha_obs, beta_obs, psi_obs
+	return alpha_obs, beta_obs, psi_obs
+
+rad = np.pi/180
+R_earth = 6371.e3
+c = 299792458.
+
+def get_TimeDelay(det,prms):
+	alpha0 = prms['RA']*rad
+	beta0  = (90-prms['Dec'])*rad
+	phi    = det['lon']*rad
+	theta  = (90-det['lat'])*rad
+	ksi    = det['rot']*rad
+
+	_, beta_a = AngTransf(alpha0,beta0,theta,phi,ksi)
+	return np.cos(beta_a)*R_earth/c
```

### Comparing `gwdali-0.1.2/GWDALI/lib/Auxiliar.py` & `gwdali-0.1.3/GWDALI/lib/Auxiliar.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.2/GWDALI/lib/Corner_Plots.py` & `gwdali-0.1.3/GWDALI/lib/Corner_Plots.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.2/GWDALI/lib/Dictionaries.py` & `gwdali-0.1.3/GWDALI/lib/Dictionaries.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.2/GWDALI/lib/Diff_Signal_Tensors.py` & `gwdali-0.1.3/GWDALI/lib/Diff_Signal_Tensors.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from scipy.interpolate import interp1d
 from scipy.integrate import trapezoid
 from scipy.optimize import root
 
 rad = np.pi/180
 deg = 1./rad
 
-c = 299792458 # m/s
+c = 299792458. # m/s
 R_earth = 6371.e3 # meters
 
 PSD, labels_tex = gwdict.Load_Dictionaries()
 
 #----------------------------------------------
 # m1(m2,Mc) or m2(m1,Mc)
 def func_mMc(x,args):
@@ -35,14 +35,37 @@
 	return m1, m2
 #----------------------------------------------
 def eta_m2(eta,m2): # return m1
 	return 0.5*(m2/eta)*( (1-2*eta) + np.sqrt(1-4*eta))
 def eta_m1(eta,m1): # return m2
 	return 0.5*(m1/eta)*( (1-2*eta) - np.sqrt(1-4*eta))
 #----------------------------------------------
+def get_iota(prms):
+	if("cos_iota" in prms.keys() ):
+		iota = np.arccos(prms['cos_iota']) # rad
+	elif("iota" in prms.keys() ):
+		iota = prms['iota'] # rad
+	else:
+		print(">> Parameter 'iota' not found!")
+		print(">> Received Parameters:", list(prms.keys()))
+		quit()
+	return iota
+
+def get_dL(prms):
+	if("ln_dL" in prms.keys()):
+		dL = np.exp( prms['ln_dL'] ) * 1.e3
+	elif("inv_dL" in prms.keys()):
+		dL = 1.e3/prms['inv_dL']
+	elif("DL" in prms.keys()):
+		dL = prms["DL"] * 1.e3
+	else:
+		print(">> Parameter 'DL' not found!")
+		print(">> Received Parameters:", list(prms.keys()))
+		quit()
+	return dL
 
 def get_mass(prms):
 	keys = list(prms.keys())
 	Mass = {}	
 	for key in keys:
 		if( key in ['m1','m2','q','eta','Mc'] ):
 			Mass[key] = prms[key]
@@ -107,17 +130,17 @@
 def ScalarProduct(freq,Sn,A,B):
 	return 4*np.real( trapezoid( A*np.conj(B)/Sn, freq) )
 
 def GW_Polarizations(params, freq, approx):
 	keys = list(params.keys())
 	
 	m1, m2   = get_mass(params)
-	DL       = params['DL']*1.e3      # Gpc --> Mpc
-	iota     = params['iota']         # rad
-	psi      = params['psi']          # rad
+	iota 	 = get_iota(params) # rad
+	DL       = get_dL(params)   # Mpc
+	psi      = params['psi']    # rad
 
 	sx1 = params['sx1']
 	sy1 = params['sy1']
 	sz1 = params['sz1']
 	sx2 = params['sx2']
 	sy2 = params['sy2']
 	sz2 = params['sz2']
@@ -125,42 +148,48 @@
 	s1 = [sx1, sy1, sz1]
 	s2 = [sx2, sy2, sz2]
 
 	hp, hx, freq0 = wf.Waveforms(m1,m2,iota,DL,s1,s2,freq, approx=approx)
 
 	return hp, hx, freq0
 
-def Signal(params, det, approx):
+# det: abreviation of detector
+def Signal(params,dets,approx):
 	alpha    = params['RA']*rad       # rad
 	beta     = (90-params['Dec'])*rad # rad
-	iota     = params['iota']         # rad
 	psi      = params['psi']          # rad
 	t_coal   = params['t_coal']       # sec
 	phi_coal = params['phi_coal']     # rad
-	
-	name  = det['name']
-	freq  = det['freq'].copy()
-	lon   = det['lon'] # deg
-	lat   = det['lat'] # deg
-	rot   = det['rot'] # deg
+	iota = get_iota(params) # rad
 
-	alpha_obs, beta_obs, psi_obs = geo.ObsAngles(alpha,beta,iota,psi,lon,lat,rot)
+	det_a, det_b = dets
+	tau_a    = geo.get_TimeDelay(det_a,params) # sec (time-delay between det_a and geocenter)
+	tau_b    = geo.get_TimeDelay(det_b,params) # sec (time-delay between det_b and geocenter)
+	tau_ab = (tau_a - tau_b) # time_delay (between det_a and det_b)
+
+	name  = det_b['name']
+	freq  = det_b['freq'].copy()
+	lon   = det_b['lon'] # deg
+	lat   = det_b['lat'] # deg
+	rot   = det_b['rot'] # deg
 
-	t_delay = np.cos(beta_obs)*R_earth/c # time delay between detector and center of Earth
-
-	Fp, Fx = Pattern_Func(alpha_obs,beta_obs,psi_obs,det['shape']*rad)
+	alpha_obs, beta_obs, psi_obs = geo.ObsAngles(alpha,beta,iota,psi,lon,lat,rot)
+	Fp, Fx = Pattern_Func(alpha_obs,beta_obs,psi_obs,det_b['shape']*rad)
 	hp, hx, freq0 = GW_Polarizations(params, freq, approx)
 
-	Phase = 2*np.pi*freq0*(t_coal+t_delay) - phi_coal
+	# t_coal := t_(0,a)
+	# tau_ab := tau_a - tau_b = t_(0,a) - t_(0,b)
+	# t_(0,b) = t_(0,a) - tau_ab
+	Phase = 2*np.pi*freq0*(t_coal-tau_ab) - phi_coal
 	H = (Fp*hp + Fx*hx)*np.exp(1.j*Phase)
 	
-	gw_signal = interp1d(freq0,H,bounds_error=False,fill_value='extrapolate')
-	h = gw_signal(freq)
+	#gw_signal = interp1d(freq0,H,bounds_error=False,fill_value='extrapolate')
+	#h = gw_signal(freq)
 
-	return h	
+	return H
 
 #-------------------------------------------------
 
 # eps (standard) = 1.e-6
 def split_prms(params,x,eps, diff_order):
 	p = params[x]
 	dx = np.max([eps,eps*p])
@@ -170,64 +199,70 @@
 	P3 = params.copy() ; P3[x] = p + dx
 	if(diff_order == 2): return [P1,P2], dx
 	elif(diff_order==4): return [P0,P1,P2,P3], dx
 	else:
 		print("\n\t Invalid diff_order! Allowed values: [2,4] ")
 		quit()
 
-def Diff1(x, params, det, approx, eps, diff_order):
+def Diff1(x, params, dets, approx, eps, diff_order):
 	Ps, dx = split_prms(params,x,eps, diff_order)
-	Y = [Signal(P, det, approx) for P in Ps]
+	Y = [Signal(P, dets, approx) for P in Ps]
 	if(diff_order == 2): return (Y[1]-Y[0])/dx
 	elif(diff_order==4): return 4*(Y[2]-Y[1])/(3*dx) - (Y[3]-Y[0])/(6*dx)
 
-def Diff2(xi, xj, params, det, approx, eps, diff_order):
+def Diff2(xi, xj, params, dets, approx, eps, diff_order):
 	Ps, dx = split_prms(params,xi,eps, diff_order)
-	Y = [Diff1(xj, P, det, approx, eps, diff_order) for P in Ps]
+	Y = [Diff1(xj, P, dets, approx, eps, diff_order) for P in Ps]
 	if(diff_order == 2): return (Y[1]-Y[0])/dx
 	elif(diff_order==4): return 4*(Y[2]-Y[1])/(3*dx) - (Y[3]-Y[0])/(6*dx)
 
-def Diff3(xi, xj, xk, params, det, approx, eps, diff_order):
+def Diff3(xi, xj, xk, params, dets, approx, eps, diff_order):
 	Ps, dx = split_prms(params,xi,eps, diff_order)
-	Y = [Diff2(xj,xk, P, det, approx, eps, diff_order) for P in Ps]
+	Y = [Diff2(xj,xk, P, dets, approx, eps, diff_order) for P in Ps]
 	if(diff_order == 2): return (Y[1]-Y[0])/dx
 	elif(diff_order==4): return 4*(Y[2]-Y[1])/(3*dx) - (Y[3]-Y[0])/(6*dx)
 
 #-------------------------------------------------#-------------------------------------------------
 #-------------------------------------------------#-------------------------------------------------
 
-def Fisher_ij(xi,xj, params, det, approx, eps, diff_order): # [1,1]
-	Dxi = Diff1(xi, params, det, approx, eps, diff_order)
-	Dxj = Diff1(xj, params, det, approx, eps, diff_order)
+def Fisher_ij(xi,xj, params, dets, approx, eps, diff_order): # [1,1]
+	det = dets[1]
+	Dxi = Diff1(xi, params, dets, approx, eps, diff_order)
+	Dxj = Diff1(xj, params, dets, approx, eps, diff_order)
 	return ScalarProduct(det['freq'], det['Sn'], Dxi, Dxj )
 
 #-------------------------------------------------#-------------------------------------------------
 # (arXiv:2203.02670)
 
-def Doublet3(xi,xj,xk, params, det, approx, eps, diff_order): # [1,2]
-	D_i  = Diff1(xi, params, det, approx, eps, diff_order)
-	D_jk = Diff2(xj,xk, params, det, approx, eps, diff_order)
+def Doublet12(xi,xj,xk, params, dets, approx, eps, diff_order): # [1,2]
+	det = dets[1]
+	D_i  = Diff1(xi, params, dets, approx, eps, diff_order)
+	D_jk = Diff2(xj,xk, params, dets, approx, eps, diff_order)
 	return ScalarProduct(det['freq'], det['Sn'], D_i, D_jk)
 
-def Doublet4(xi,xj,xk,xl, params, det, approx, eps, diff_order): # [2,2]
-	D_ij = Diff2(xi,xj, params, det, approx, eps, diff_order)
-	D_kl = Diff2(xk,xl, params, det, approx, eps, diff_order)
+def Doublet22(xi,xj,xk,xl, params, dets, approx, eps, diff_order): # [2,2]
+	det = dets[1]
+	D_ij = Diff2(xi,xj, params, dets, approx, eps, diff_order)
+	D_kl = Diff2(xk,xl, params, dets, approx, eps, diff_order)
 	return ScalarProduct(det['freq'], det['Sn'], D_ij, D_kl)
 
 #-------------------------------------------------#-------------------------------------------------
 
-def Triplet4(xi,xj,xk,xl, params, det, approx, eps, diff_order): # [1,3]
-	D_i   = Diff1(xi, params, det, approx, eps, diff_order)
-	D_jkl = Diff3(xj,xk,xl, params, det, approx, eps, diff_order)
+def Triplet13(xi,xj,xk,xl, params, dets, approx, eps, diff_order): # [1,3]
+	det = dets[1]
+	D_i   = Diff1(xi, params, dets, approx, eps, diff_order)
+	D_jkl = Diff3(xj,xk,xl, params, dets, approx, eps, diff_order)
 	return ScalarProduct(det['freq'], det['Sn'], D_i, D_jkl)
 
-def Triplet5(xi,xj,xk,xl,xm, params, det, approx, eps, diff_order): # [2,3]
-	D_ij  = Diff2(xi,xj, params, det, approx, eps, diff_order)
-	D_klm = Diff3(xk,xl,xm, params, det, approx, eps, diff_order)
+def Triplet23(xi,xj,xk,xl,xm, params, dets, approx, eps, diff_order): # [2,3]
+	det = dets[1]
+	D_ij  = Diff2(xi,xj, params, dets, approx, eps, diff_order)
+	D_klm = Diff3(xk,xl,xm, params, dets, approx, eps, diff_order)
 	return ScalarProduct(det['freq'], det['Sn'], D_ij, D_klm)
 
-def Triplet6(xi,xj,xk,xl,xm,xn, params, det, approx, eps, diff_order): # [3,3]
-	D_ijk = Diff3(xi,xj,xk, params, det, approx, eps, diff_order)
-	D_lmn = Diff3(xl,xm,xn, params, det, approx, eps, diff_order)
+def Triplet33(xi,xj,xk,xl,xm,xn, params, dets, approx, eps, diff_order): # [3,3]
+	det = dets[1]
+	D_ijk = Diff3(xi,xj,xk, params, dets, approx, eps, diff_order)
+	D_lmn = Diff3(xl,xm,xn, params, dets, approx, eps, diff_order)
 	return ScalarProduct(det['freq'], det['Sn'], D_ijk, D_lmn)
 
 #-------------------------------------------------#-------------------------------------------------
```

### Comparing `gwdali-0.1.2/GWDALI/lib/Get_Tensors.py` & `gwdali-0.1.3/GWDALI/lib/Get_Tensors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os, sys
 import numpy as np
-import GWDALI.lib.Angles_lib as geo
 import GWDALI.lib.Dictionaries as dct
 import GWDALI.lib.Diff_Signal_Tensors as gw
 import GWDALI.lib.Auxiliar as sym
 
 from itertools import permutations
 from tqdm import trange
 
 deg2rad = np.pi/180
+c = 299792458. # m/s
+R_earth = 6371.e3 # meters
 
 PSD, labels_tex = dct.Load_Dictionaries()
 
 def pmt(vec):
 	x, y = [ list(xx) for xx in list(permutations(vec)) ] , []
 	for a in x:
 		if(not a in y): y.append(a)
@@ -20,43 +21,43 @@
 
 def Get_Tensors(FreeParams, gw_prms, detectors, dali_method, approx, step_size, diff_order, hide_info):
 	
 	Np = len(FreeParams)
 	rho2 = 0
 
 	Fisher = np.zeros([Np, Np])
-	Db3    = np.zeros([Np, Np, Np])
-	Db4    = np.zeros([Np, Np, Np, Np])
-	Tp4    = np.zeros([Np, Np, Np, Np])
-	Tp5    = np.zeros([Np, Np, Np, Np, Np])
-	Tp6    = np.zeros([Np, Np, Np, Np, Np, Np])
+	Db12    = np.zeros([Np, Np, Np])
+	Db22    = np.zeros([Np, Np, Np, Np])
+	Tp13    = np.zeros([Np, Np, Np, Np])
+	Tp23    = np.zeros([Np, Np, Np, Np, Np])
+	Tp33    = np.zeros([Np, Np, Np, Np, Np, Np])
 
 	num_det = 1
 	GwData = [] ; SNR = []
-	for det in detectors:
-
+	det_a = detectors[0]
+	for det_b in detectors:
+		dets = [det_a, det_b]
 		#-----------------------------------
 		# Computing Signal to Noise 
-		#-----------------------------------
-		# from Derivative_Tensors.py
-		h 	  = gw.Signal(gw_prms, det, approx)
-		SNR2  = gw.ScalarProduct(det['freq'], det['Sn'],h,h)
+		h 	  = gw.Signal(gw_prms, dets, approx)#*ExpT
+
+		SNR2  = gw.ScalarProduct(det_b['freq'], det_b['Sn'],h,h)
 		rho2 += SNR2
 		GwData.append(h) ; SNR.append(np.sqrt(SNR2))
 		#------------------------------------------------------
 		# Computing Fisher Matrix
 		#------------------------------------------------------
 
-		if(not hide_info): print("\n\n\t Computing Fisher %s(%d) ..." % (det['name'],num_det))
+		if(not hide_info): print("\n\n\t Computing Fisher %s(%d) ..." % (det_b['name'],num_det))
 		for i in range(Np):
 			for j in range(i+1):
 				if(not hide_info): print('Fisher: [%d-%d]' % (i+1,j+1), end='\r')
 				xj = FreeParams[j]
 				xi = FreeParams[i]
-				Fij = gw.Fisher_ij(xi, xj, gw_prms, det, approx, step_size, diff_order)
+				Fij = gw.Fisher_ij(xi, xj, gw_prms, dets, approx, step_size, diff_order)
 				Fisher[i][j] += Fij
 
 				if(i!=j): Fisher[j][i] += Fij
 		if(not hide_info): print("\n\n\t\tFisher Concluded!!!\n\n")
 		#------------------------------------------------------
 		# Computing Doublet/Triplet (arXiv:2203.02670)
 		#------------------------------------------------------
@@ -64,61 +65,61 @@
 		idxs_doub, idxs_trip = sym.get_indep_indexies(Np)
 		
 		if(dali_method in ["Doublet","Triplet"]):
 			indepD_12, indepD_22 = idxs_doub
 			# --------------Doublet(1,2)--------------		
 			for Idx2 in indepD_12:
 				i, j, k = Idx2
-				value = gw.Doublet3(*[FreeParams[ii] for ii in Idx2],gw_prms,det,approx, step_size, diff_order)
+				value = gw.Doublet12(*[FreeParams[ii] for ii in Idx2],gw_prms,dets,approx, step_size, diff_order)
 				for p in pmt([j,k]):
 					jj, kk = p
-					Db3[i][jj][kk] += value
+					Db12[i][jj][kk] += value
 			# --------------Doublet(2,2)--------------
 			for Idx2 in indepD_22:
 				i, j, k, l = Idx2
-				value = gw.Doublet4(*[FreeParams[ii] for ii in Idx2],gw_prms,det,approx, step_size, diff_order)
+				value = gw.Doublet22(*[FreeParams[ii] for ii in Idx2],gw_prms,dets,approx, step_size, diff_order)
 				for p1 in pmt([i,j]):
 					ii, jj = p1
 					for p2 in pmt([k,l]):
 						kk, ll = p2
-						Db4[ii][jj][kk][ll] += value
-						if(not hide_info): print('(%s) [Sym] Doublet: '%det['name'], i, j, k, l,'...'*10, end='\r')
+						Db22[ii][jj][kk][ll] += value
+						if(not hide_info): print('(%s) [Sym] Doublet: '%det_b['name'], i, j, k, l,'...'*10, end='\r')
 			#*****************************#*****************************#*****************************
 			if(dali_method == 'Triplet'):
 				indepT_13, indepT_23, indepT_33 = idxs_trip
 				# --------------Triplet(1,3)--------------
 				for Idx3 in indepT_13:
 					i, j, k, l = Idx3
-					value = gw.Triplet4(*[FreeParams[ii] for ii in Idx3],gw_prms,det,approx, step_size, diff_order)
+					value = gw.Triplet13(*[FreeParams[ii] for ii in Idx3],gw_prms,dets,approx, step_size, diff_order)
 					for p in pmt([j,k,l]):
 						jj, kk, ll = p
-						Tp4[i][jj][kk][ll] += value
+						Tp13[i][jj][kk][ll] += value
 				# --------------Triplet(2,3)--------------
 				for Idx3 in indepT_23:
 					i, j, k, l, m = Idx3
-					value = gw.Triplet5(*[FreeParams[ii] for ii in Idx3],gw_prms,det,approx, step_size, diff_order)
+					value = gw.Triplet23(*[FreeParams[ii] for ii in Idx3],gw_prms,dets,approx, step_size, diff_order)
 					for p1 in pmt([i,j]):
 						ii, jj = p1
 						for p2 in pmt([k,l,m]):
 							kk, ll, mm = p2
-							Tp5[ii][jj][kk][ll][mm] += value
+							Tp23[ii][jj][kk][ll][mm] += value
 				# --------------Triplet(3,3)--------------
 				for Idx3 in indepT_33:
 					i, j, k, l, m, n = Idx3
-					value = gw.Triplet6(*[FreeParams[ii] for ii in Idx3],gw_prms,det,approx, step_size, diff_order)
+					value = gw.Triplet33(*[FreeParams[ii] for ii in Idx3],gw_prms,dets,approx, step_size, diff_order)
 					for p1 in pmt([i,j,k]):
 						ii, jj, kk = p1
 						for p2 in pmt([l,m,n]):
 							ll, mm, nn = p2
-							Tp6[ii][jj][kk][ll][mm][nn] += value
-							if(not hide_info): print('(%s) [Sym] Triplet: '%det['name'], i, j, k, l, m, n,'...'*10, end='\r')
+							Tp33[ii][jj][kk][ll][mm][nn] += value
+							if(not hide_info): print('(%s) [Sym] Triplet: '%det_b['name'], i, j, k, l, m, n,'...'*10, end='\r')
 		# --------------# --------------# --------------					
 
 	SNR_sum = np.sqrt(rho2)
 	if(not hide_info):
-		print("\n >> SNR = ", SNR_sum)
-		print(" >> 100/SNR = %.2e" % (100/SNR_sum) + '%\n')
+		print(" >> SNR = ", SNR_sum)
+		print(" >> 100/SNR = %.2e" % (100/SNR_sum) + '%')
 
-	Doublet = [Db3, Db4]
-	Triplet = [Tp4, Tp5, Tp6]
+	Doublet = [Db12, Db22]
+	Triplet = [Tp13, Tp23, Tp33]
 
 	return [SNR, GwData, Fisher , Doublet, Triplet]
```

### Comparing `gwdali-0.1.2/GWDALI/lib/Likelihood.py` & `gwdali-0.1.3/GWDALI/lib/Likelihood.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,36 +16,39 @@
 bilby.core.utils.setup_logger(log_level=50)
 
 #--------------------------------------------------
 class GW_likelihood(bilby.Likelihood):
 	def __init__(self,args):
 		aux = {}
 		self.FreeParams = args[0]
-		self.Data       = args[1]
+		self.h_data       = args[1]
 		self.GWparams   = args[2]
 		self.DetAp		= args[3]
 		for f in args[0]: aux[f] = None
 		super().__init__(aux)
 
 	def log_likelihood(self):
 		Np = len(self.FreeParams)
 		params = self.GWparams.copy()
 		for fp in self.FreeParams:
 			params[fp] = self.parameters[fp]
 			
 		loglike = 0 ; ndet = 0
-		detectors, approximant = self.DetAp 
+		detectors, approximant = self.DetAp
 
-		for det in detectors:
-			h = gwfunc.Signal(params, det, approximant)
-			diff = self.Data[ndet]-h
-			loglike -= 0.5*gwfunc.ScalarProduct(det['freq'],det['Sn'],diff,diff)
+		det_a = detectors[0]
+		for det_b in detectors:
+			dets = [det_a, det_b]
+			h_model = gwfunc.Signal(params, dets, approximant)#*ExpT
+
+			diff = self.h_data[ndet]-h_model
+			loglike -= 0.5*gwfunc.ScalarProduct(det_b['freq'],det_b['Sn'],diff,diff)
 			ndet += 1
 			
-		if(np.isnan(loglike) or np.isinf(loglike)): loglike = -1.e9
+		if(np.isnan(loglike)): loglike = -np.inf
 		return loglike
 #--------------------------------------------------
 
 class DALI_likelihood(bilby.Likelihood):
 	def __init__(self,args):
 		self.FreeParams  = args[0]
 		self.Theta0      = args[1]
@@ -60,16 +63,16 @@
 		Np = len(self.FreeParams)
 		for fp in self.FreeParams:
 			Theta  = self.parameters[fp]
 			Theta0 = self.Theta0[i] ; i += 1
 			dX.append(Theta-Theta0) # Fixed!!!
 
 		Fij , Doublet , Triplet = self.Tensors
-		Db3, Db4 = Doublet
-		Tp4, Tp5, Tp6 = Triplet
+		Db12, Db22 = Doublet
+		Tp13, Tp23, Tp33 = Triplet
 
 		dX  = np.array(dX)
 		dX2 = np.outer(dX,dX)
 		dX3 = np.outer(dX2,dX)
 		dX4 = np.outer(dX3,dX)
 		dX5 = np.outer(dX4,dX)
 		dX6 = np.outer(dX5,dX)
@@ -77,73 +80,92 @@
 		dX2 = np.ravel(dX2)
 		dX3 = np.ravel(dX3)
 		dX4 = np.ravel(dX4)
 		dX5 = np.ravel(dX5)
 		dX6 = np.ravel(dX6)
 
 		# From arXiv:2203.02670
-		# logL = logL0 - (1/2)Fisher * dTheta_ij - [ (1/2)Db3 * dTheta_ijk  + (1/8) * dTheta_ijkl ]
-		#        - [ (1/6)Tp4 * dTheta_ijkl + (1/12) * dTheta_ijklm + (1/72) * dTheta_ijklmn ] + ...
+		# logL = logL0 - (1/2)Fisher * dTheta_ij - [ (1/2)Db12 * dTheta_ijk  + (1/8) * dTheta_ijkl ]
+		#        - [ (1/6)Tp13 * dTheta_ijkl + (1/12) * dTheta_ijklm + (1/72) * dTheta_ijklmn ] + ...
 		
 		loglike = -np.sum(Fij*dX2)/2
-		loglike -= np.sum(Db3*dX3)/2 + np.sum(Db4*dX4)/8
-		loglike -= np.sum(Tp4*dX4)/6 + np.sum(Tp5*dX5)/12 + np.sum(Tp6*dX6)/72
+		loglike -= np.sum(Db12*dX3)/2 + np.sum(Db22*dX4)/8
+		loglike -= np.sum(Tp13*dX4)/6 + np.sum(Tp23*dX5)/12 + np.sum(Tp33*dX6)/72
 
-		if(np.isnan(loglike) or np.isnan(loglike)): return -1.e9
+		if(np.isnan(loglike)): loglike = -np.inf
 		else: return loglike
 
 #----------------------------------------
 # Prior(DL): dVc/dz
 #---------------------------------------- 
 z      = np.linspace(1.e-3,10,1000) ; dz = z[1]-z[0]# redshift
 Vc     = cosmo.comoving_volume(z).value
 priorD = np.diff(Vc)/np.diff(z)
 z   = z[1:]-dz/2
 XdL = cosmo.luminosity_distance(z).value / 1.e3 # dL in Gpc
 YdL = priorD/sum(priorD)
 #----------------------------------------
-d1 = cosmo.luminosity_distance(1.e-3).value / 1.e3 # Gpc
-d2 = cosmo.luminosity_distance(5.0).value / 1.e3   # Gpc
+# Prior(1/DL): dVc/dz * dL^2
+# p(x)dx = p(x)|dx/dy| dy -> p(y) = p(x)|dx/dy|
+#---------------------------------------- 
+XidL = 1./XdL ; idxs = np.argsort(XidL)
+XidL = XidL[idxs]
+YidL = YdL[idxs] * XdL[idxs]**2
+YidL = YidL/sum(YidL)
+#----------------------------------------
+# Prior(logDL): dVc/dz * dL
+#---------------------------------------- 
+XlogDL = np.log(XdL) ; idxs = np.argsort(XlogDL)
+XlogDL = XlogDL[idxs]
+YlogDL = YdL[idxs] * XdL[idxs]
+YlogDL = YlogDL/sum(YlogDL)
+#----------------------------------------
+d1, d2 = XdL[0] , XdL[-1]
+id1, id2 = XidL[0] , XidL[-1]
+lD1, lD2 = XlogDL[0] , XlogDL[-1]
 #----------------------------------------
 # Pior(Dec): cos(Dec[degrees])
 Xdec = np.linspace(-90,90,1000)
 Ydec = np.cos(Xdec*np.pi/180)
 Ydec/=sum(Ydec)
 #----------------------------------------
 
-def get_posterior(FreeParams, Theta0, Detection_Dict, GwData, approximant, Detectors, Tensors, dali_method, sampler_method, npoints,new_priors):
-	Priors_std = {}
-	Priors_std['DL']   = bilby.core.prior.Interped(name='DL',xx=XdL,yy=YdL,minimum=d1, maximum=d2) # Gpc
-	Priors_std['iota']  = bilby.core.prior.Sine(name='iota', minimum=0, maximum=np.pi) # radians
-	Priors_std['psi']   = bilby.core.prior.Uniform(name='psi',minimum=0, maximum=np.pi) # radians
-	#----------------------------#----------------------------#----------------------------
-	Priors_std['alpha'] = bilby.core.prior.Uniform(name='alpha',minimum=-np.pi, maximum=np.pi) # radians
-	Priors_std['beta']  = bilby.core.prior.Sine(name='beta',minimum=0, maximum=np.pi) # radians
-	#----------------------------#----------------------------#----------------------------
-	Priors_std['RA']    = bilby.core.prior.Uniform(name='RA',minimum=-180, maximum=180) # degrees
-	Priors_std['Dec']   = bilby.core.prior.Interped(name='Dec',xx=Xdec,yy=Ydec,minimum=-90, maximum=90) # degrees
-	#----------------------------#----------------------------#----------------------------
-	Priors_std['m1']    = bilby.core.prior.Uniform(name='m1',minimum=0.1, maximum=100) # solar mass
-	Priors_std['m2']    = bilby.core.prior.Uniform(name='m2',minimum=0.1, maximum=100) # solar mass
-	#----------------------------#----------------------------#----------------------------
-	Priors_std['Mc']    = bilby.core.prior.Uniform(name='Mc',minimum=0.1, maximum=100) # solar mass
-	Priors_std['eta']   = bilby.core.prior.Uniform(name='eta',minimum=1.e-3, maximum=1./4)
-	Priors_std['q']     = bilby.core.prior.Uniform(name='q',minimum=1.e-3, maximum=1.0)
-	#----------------------------#----------------------------#----------------------------
-	Priors_std['sx1']    = bilby.core.prior.Uniform(name='sx1',minimum=0, maximum=1.0)
-	Priors_std['sy1']    = bilby.core.prior.Uniform(name='sy1',minimum=0, maximum=1.0)
-	Priors_std['sz1']    = bilby.core.prior.Uniform(name='sz1',minimum=0, maximum=1.0)
-	Priors_std['sx2']    = bilby.core.prior.Uniform(name='sx2',minimum=0, maximum=1.0)
-	Priors_std['sy2']    = bilby.core.prior.Uniform(name='sy2',minimum=0, maximum=1.0)
-	Priors_std['sz2']    = bilby.core.prior.Uniform(name='sz2',minimum=0, maximum=1.0)
-	#----------------------------#----------------------------#----------------------------
-	Priors_std['phi_coal']  = bilby.core.prior.Uniform(name='phi_coal',minimum=0, maximum=2*np.pi) # radians
-	Priors_std['t_coal']    = bilby.core.prior.Uniform(name='t_coal',minimum=0, maximum=3600) # seconds
-	#----------------------------#----------------------------#----------------------------
+Priors_std = {}
+Priors_std['DL']	   = bilby.core.prior.Interped(name='DL',xx=XdL,yy=YdL,minimum=d1, maximum=d2) # Gpc
+Priors_std['inv_dL']   = bilby.core.prior.Interped(name='inv_dL',xx=XidL,yy=YidL,minimum=id1, maximum=id2) # 1./Gpc
+Priors_std['ln_dL']    = bilby.core.prior.Interped(name='ln_dL',xx=XlogDL,yy=YlogDL,minimum=lD1, maximum=lD2) # ln(Gpc)
+Priors_std['iota']	   = bilby.core.prior.Sine(name='iota', minimum=0, maximum=np.pi) # radians
+Priors_std['cos_iota'] = bilby.core.prior.Uniform(name='cos_iota',minimum=-1., maximum=1.) # radians
+Priors_std['psi']      = bilby.core.prior.Uniform(name='psi',minimum=0, maximum=np.pi) # radians
+#----------------------------#----------------------------#----------------------------
+Priors_std['alpha'] = bilby.core.prior.Uniform(name='alpha',minimum=-np.pi, maximum=np.pi) # radians
+Priors_std['beta']  = bilby.core.prior.Sine(name='beta',minimum=0, maximum=np.pi) # radians
+#----------------------------#----------------------------#----------------------------
+Priors_std['RA']    = bilby.core.prior.Uniform(name='RA',minimum=-180, maximum=180) # degrees
+Priors_std['Dec']   = bilby.core.prior.Interped(name='Dec',xx=Xdec,yy=Ydec,minimum=-90, maximum=90) # degrees
+#----------------------------#----------------------------#----------------------------
+Priors_std['m1']    = bilby.core.prior.Uniform(name='m1',minimum=0.1, maximum=100) # solar mass
+Priors_std['m2']    = bilby.core.prior.Uniform(name='m2',minimum=0.1, maximum=100) # solar mass
+#----------------------------#----------------------------#----------------------------
+Priors_std['Mc']    = bilby.core.prior.Uniform(name='Mc',minimum=0.1, maximum=100) # solar mass
+Priors_std['eta']   = bilby.core.prior.Uniform(name='eta',minimum=1.e-3, maximum=1./4)
+Priors_std['q']     = bilby.core.prior.Uniform(name='q',minimum=1.e-3, maximum=1.0)
+#----------------------------#----------------------------#----------------------------
+Priors_std['sx1']    = bilby.core.prior.Uniform(name='sx1',minimum=0, maximum=1.0)
+Priors_std['sy1']    = bilby.core.prior.Uniform(name='sy1',minimum=0, maximum=1.0)
+Priors_std['sz1']    = bilby.core.prior.Uniform(name='sz1',minimum=0, maximum=1.0)
+Priors_std['sx2']    = bilby.core.prior.Uniform(name='sx2',minimum=0, maximum=1.0)
+Priors_std['sy2']    = bilby.core.prior.Uniform(name='sy2',minimum=0, maximum=1.0)
+Priors_std['sz2']    = bilby.core.prior.Uniform(name='sz2',minimum=0, maximum=1.0)
+#----------------------------#----------------------------#----------------------------
+Priors_std['phi_coal']  = bilby.core.prior.Uniform(name='phi_coal',minimum=0, maximum=2*np.pi) # radians
+Priors_std['t_coal']    = bilby.core.prior.Uniform(name='t_coal',minimum=0, maximum=3600) # seconds
+#----------------------------#----------------------------#----------------------------
 
+def get_posterior(FreeParams, Theta0, Detection_Dict, GwData, approximant, Detectors, Tensors, dali_method, sampler_method, npoints,new_priors):
 	Priors = {}
 	for fp in FreeParams: Priors[fp] = Priors_std[fp]
 	if(new_priors!=None):
 		for fp in new_priors.keys():
 			try:
 				Xval, Yval = new_priors[fp]
 				Yval /= sum(Yval)
@@ -158,15 +180,15 @@
 		Fisher, Doublet, Triplet = Tensors
 		Fisher = np.ravel(Fisher)
 		Doublet = [np.ravel(Doublet[i]) for i in range(2)]
 		Triplet = [np.ravel(Triplet[i]) for i in range(3)]
 		Tensors = [Fisher,Doublet,Triplet]
 		likelihood = DALI_likelihood([FreeParams, Theta0, Tensors, dali_method])
 
-	outdir = 'outdir_%s_%d/' % (dali_method, int(np.random.uniform(0,300))  )
+	outdir = 'outdir_%s_%d/' % (dali_method, int(np.random.uniform(0,1000))  )
 	if(os.path.isdir(outdir)):
 		shutil.rmtree(outdir)
 
 	#----------------------------
 	# Running Sampler
 	#----------------------------
 	print("\t >> Method:", dali_method)
```

### Comparing `gwdali-0.1.2/GWDALI/lib/Waveforms.py` & `gwdali-0.1.3/GWDALI/lib/Waveforms.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,20 +13,15 @@
 	import lal
 	import lalsimulation as lalsim
 except:
 	print(wrn)
 
 M_sun = 1.98e30
 G = 6.673e-11
-c = 299792458 # m/s
-
-def integ(x,y): # Integral [Trapezoid Method]
-	n = len(x) ; I = 0
-	for i in range(1,n): I += 0.5*(y[i]+y[i-1])*(x[i]-x[i-1])
-	return I	
+c = 299792458. # m/s
 
 #==============================================================================================
 # LAL WAVEFORMS
 #==============================================================================================
 
 def Waveform_lal(m1, m2, iota, DL, s1, s2, freq, approx):
 	dF = np.average(np.diff(freq)) #1 
@@ -34,15 +29,15 @@
 
 	sx1, sy1, sz1 = s1
 	sx2, xy2, sz2 = s2
 	
 	phi_ref = 0.
 	f_ref = 0.
 
-	DL *= 3.086e22
+	DL *= 3.086e22 # Mpc -> meters
 	hp,hx=lalsim.SimInspiralChooseFDWaveform(m1*M_sun,m2*M_sun, sx1, sy1, sz1, sx2, xy2, sz2, DL,
 											iota, phi_ref, 0., 0., 0., dF, f_low, f_max, f_ref, None,
 											lalsim.GetApproximantFromString(approx))
 	
 	hp = hp.data.data ; hp[np.isnan(hp)] = 0
 	hx = hx.data.data ; hx[np.isnan(hx)] = 0
 
@@ -50,81 +45,88 @@
 	freq0 = np.linspace(0,dF*(N-1),N)
 
 	return hp, hx, freq0
 
 #==============================================================================================
 # PYTHON WAVEFORMS ( Leading Order and TaylorF2(3.5PN) )
 #==============================================================================================
-
-def GW_Amplitude(m1,m2,DL,freq):
-	DL *= 3.086e22     # DL [meters]
-	M = m1+m2			 # Total Mass
-	eta = m1*m2/M**2   # Symmetric Mass Ratio
-	M *= M_sun
-	Mc = M*eta**(3./5) # Chirp Mass
-	R_isco = 6*(G*M)/c**2
-	f_isco = np.sqrt(G*M/R_isco**3)/np.pi # gw frequency at R=R_isco
-	Cutoff = np.ones(len(freq))*(freq<4*f_isco)
-	return Cutoff*pow(freq,-7./6)*np.sqrt(5./(24*c**3))*pow(np.pi,-2./3)*pow(G*Mc,5./6)/DL
-	
-def GW_Phase_Simple(m1,m2,freq):
-	M = m1+m2			 # Total Mass
-	eta = m1*m2/M**2   # Symmetric Mass Ratio
-	M *= M_sun
-	GM_c3 = G*M/c**3
-	phase = (3./(128*eta))/(np.pi*GM_c3*freq)**(5./3)
-	return phase
 	
 def GW_Phase_TaylorF2(m1,m2,freq):
 	M = m1+m2
 	eta = m1*m2/M**2
 	M *= M_sun
 	GM_c3 = G*M/c**3
 	
 	A = list(np.zeros(8))
 	A[0] = 1.
 	A[1] = 0.
 	A[2] = (3715./756) + (55./9)*eta 
 	A[3] = -16*np.pi
 	A[4] = (15293365./508032) + (27145*eta/504) + (3085*eta**2/72)
 	A[5] = np.pi*((38645./756) - (65*eta/9))*(1.+np.log((6.**1.5)*np.pi*GM_c3*freq))
-	A[6] = (11583231236531./4694215680) - (640*np.pi**2/3) - (6848*np.euler_gamma/21) + (-(15737765635./3048192)+(2255*np.pi**2/12))*eta + (76055*eta**2/1728) - (127825*eta**3/1296) - (6848./63)*np.log(64*np.pi*GM_c3*freq)
+	A[6] = (11583231236531./4694215680) - (640*np.pi**2/3) - (6848*np.euler_gamma/21)\
+		 + (-(15737765635./3048192)+(2255*np.pi**2/12))*eta + (76055*eta**2/1728)\
+		 - (127825*eta**3/1296) - (6848./63)*np.log(64*np.pi*GM_c3*freq)
 	A[7] = np.pi*((77096675./254016) + (378515*eta/1512) - (74045*eta**2/756))
 
 	phase = np.zeros(len(freq))  # 3.5PN Corrections from idx>0
 	for idx in range(0,8):
 		phase += A[idx]*(np.pi*GM_c3*freq)**((idx-5)/3)
 	phase *= 3./(128*eta)
 
 	return phase
 
-#-----------------------------------------------------------------------------------------------
+def GW_Amplitude(m1,m2,DL,freq):
+	DL *= 3.086e22     # DL [meters]
+	M = m1+m2			 # Total Mass
+	eta = m1*m2/M**2   # Symmetric Mass Ratio
+	M *= M_sun
+	Mc = M*eta**(3./5) # Chirp Mass
+	R_isco = 6*(G*M)/c**2
+	f_isco = np.sqrt(G*M/R_isco**3)/np.pi # gw frequency at R=R_isco
+	Cutoff = np.ones(len(freq))*(freq<4*f_isco)
+	return Cutoff*pow(freq,-7./6)*np.sqrt(5./(24*c**3))*pow(np.pi,-2./3)*pow(G*Mc,5./6)/DL
 
 def Waveform_TaylorF2(m1, m2, iota, DL, s1, s2, freq): # Sathyaprakash-Schutz(2009)
 	Amp   = GW_Amplitude(m1,m2,DL,freq)
 	phase = GW_Phase_TaylorF2(m1,m2,freq)
 	
 	exp = np.exp(1.j*(phase-np.pi/4))
 
-	cos_iota = np.cos(iota)
-	Gp, Gx = 0.5*(1.+cos_iota*cos_iota), 1.j*cos_iota
+	u = np.cos(iota)
+	Gp, Gx = 0.5*(1.+u*u), 1.j*u
 	Hplus  = Gp*Amp*exp
 	Hcross = Gx*Amp*exp
 
-	return Hplus, Hcross, freq #, Amp, exp
+	return Hplus, Hcross, freq
 		
 def Waveform_Simple(m1, m2, iota, DL, s1, s2, freq):
-	Amp = GW_Amplitude(m1,m2,DL,freq)
-	phase = GW_Phase_Simple(m1,m2,freq)
+	m1 *= M_sun ; m2 *= M_sun
+	M = m1+m2		   # Total Mass
+	eta = m1*m2/M**2   # Symmetric Mass Ratio
+	Mc = eta**(3./5) * M
+	DL *= 3.086e22
+
+	h0 = np.sqrt(5./24) * (G*Mc/c**3)**(5./6) / (np.pi**(2./3)*DL/c)
+	phase = (3./128) * (np.pi * G * Mc * freq / c**3)**(-5./3)
+
+	R_isco = 6*G*M/c**2
+	f_isco = np.sqrt(G*M/R_isco**3) / np.pi
+	cutoff = freq<f_isco
+
+	Phase = - np.pi/4 + (3./128)*(np.pi*G*Mc*freq/c**3)**(-5./3)
+	u = np.cos(iota)
+
+	Gp = 0.5*(1+u*u)
+	Gx = 1.j*u
+
+	hp = h0*Gp*freq**(-7./6)*np.exp(1.j*Phase) * cutoff
+	hx = h0*Gx*freq**(-7./6)*np.exp(1.j*Phase) * cutoff
 	
-	cos_iota = np.cos(iota)
-	Gp, Gx = 0.5*(1.+cos_iota*cos_iota), cos_iota
-	Hplus  = Gp*Amp*np.exp(1.j*(phase-np.pi/4))
-	Hcross = Gx*Amp*np.exp(1.j*(phase+np.pi/4))
-	return Hplus, Hcross, freq
+	return hp, hx, freq
 
 #-----------------------------------------------------------------------------------------------
 
 def Waveforms(m1, m2, iota, DL, s1, s2, freq, approx):
 	if approx == 'Leading_Order':
 		return Waveform_Simple(m1, m2, iota, DL, s1, s2, freq)
 	elif approx == 'TaylorF2_py':
```

### Comparing `gwdali-0.1.2/LICENSE` & `gwdali-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.2/PKG-INFO` & `gwdali-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdali
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Fisher-Based Software for Parameter Estimation from Gravitational Waves
 Author: Josiel Mendonça Soares de Souza
 Author-email: josiel.jms7@gmail.com
 License: BSD 3-Clause License
 Keywords: fisher matrix,gravitational waves,gw,dali
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gwdali-0.1.2/README.md` & `gwdali-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.2/gwdali.egg-info/PKG-INFO` & `gwdali-0.1.3/gwdali.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdali
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Fisher-Based Software for Parameter Estimation from Gravitational Waves
 Author: Josiel Mendonça Soares de Souza
 Author-email: josiel.jms7@gmail.com
 License: BSD 3-Clause License
 Keywords: fisher matrix,gravitational waves,gw,dali
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gwdali-0.1.2/gwdali.egg-info/SOURCES.txt` & `gwdali-0.1.3/gwdali.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.2/setup.py` & `gwdali-0.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md",'r') as arq:
 	readme = arq.read()
 
 setup(
 	name = 'gwdali',
-	version = '0.1.2',
+	version = '0.1.3',
 	license = 'BSD 3-Clause License',
 	author  = 'Josiel Mendonça Soares de Souza',
 	long_description = readme,
 	long_description_content_type = "text/markdown",
 	author_email = 'josiel.jms7@gmail.com',
 	keywords = 'fisher matrix, gravitational waves, gw, dali',
 	description = 'A Fisher-Based Software for Parameter Estimation from Gravitational Waves',
```

