# Comparing `tmp/va_am-0.1.1.tar.gz` & `tmp/va_am-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/cosmin/Documentos/GitHub/va_am/dist/.tmp-kgt17vei/va_am-0.1.1.tar", last modified: Tue Feb 20 12:04:42 2024, max compression
+gzip compressed data, was "va_am-0.1.2.tar", last modified: Wed Apr 10 08:50:52 2024, max compression
```

## Comparing `va_am-0.1.1.tar` & `va_am-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-02-20 12:04:42.000000 va_am-0.1.1/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    35149 2023-09-29 09:45:51.000000 va_am-0.1.1/LICENSE
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    46138 2024-02-20 12:04:42.000000 va_am-0.1.1/PKG-INFO
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     5078 2024-02-12 18:26:04.000000 va_am-0.1.1/README.md
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      756 2024-02-20 12:03:56.000000 va_am-0.1.1/pyproject.toml
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       38 2024-02-20 12:04:42.000000 va_am-0.1.1/setup.cfg
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       68 2023-09-28 11:32:10.000000 va_am-0.1.1/setup.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-02-20 12:04:42.000000 va_am-0.1.1/src/
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-02-20 12:04:42.000000 va_am-0.1.1/src/va_am/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      222 2024-02-20 12:03:10.000000 va_am-0.1.1/src/va_am/__init__.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       66 2023-09-28 11:12:58.000000 va_am-0.1.1/src/va_am/__main__.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-02-20 12:04:42.000000 va_am-0.1.1/src/va_am/utils/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    61061 2024-02-16 14:28:14.000000 va_am-0.1.1/src/va_am/utils/AutoEncoders.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2023-06-29 15:33:10.000000 va_am-0.1.1/src/va_am/utils/__init__.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     3123 2023-09-25 14:36:24.000000 va_am-0.1.1/src/va_am/utils/functions.py
--rw-r--r--   0 cosmin    (1000) cosmin    (1000)   101413 2024-02-20 11:28:25.000000 va_am-0.1.1/src/va_am/va_am.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-02-20 12:04:42.000000 va_am-0.1.1/src/va_am.egg-info/
--rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46138 2024-02-20 12:04:42.000000 va_am-0.1.1/src/va_am.egg-info/PKG-INFO
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      393 2024-02-20 12:04:42.000000 va_am-0.1.1/src/va_am.egg-info/SOURCES.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2024-02-20 12:04:42.000000 va_am-0.1.1/src/va_am.egg-info/dependency_links.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       46 2024-02-20 12:04:42.000000 va_am-0.1.1/src/va_am.egg-info/entry_points.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       71 2024-02-20 12:04:42.000000 va_am-0.1.1/src/va_am.egg-info/requires.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        6 2024-02-20 12:04:42.000000 va_am-0.1.1/src/va_am.egg-info/top_level.txt
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-04-10 08:50:52.080531 va_am-0.1.2/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    35149 2023-09-29 09:45:51.000000 va_am-0.1.2/LICENSE
+-rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-04-10 08:50:52.080531 va_am-0.1.2/PKG-INFO
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     5078 2024-02-12 18:26:04.000000 va_am-0.1.2/README.md
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      756 2024-04-10 08:48:41.000000 va_am-0.1.2/pyproject.toml
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       38 2024-04-10 08:50:52.080531 va_am-0.1.2/setup.cfg
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       68 2023-09-28 11:32:10.000000 va_am-0.1.2/setup.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-04-10 08:50:52.076531 va_am-0.1.2/src/
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-04-10 08:50:52.080531 va_am-0.1.2/src/va_am/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      222 2024-02-20 12:03:10.000000 va_am-0.1.2/src/va_am/__init__.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       66 2023-09-28 11:12:58.000000 va_am-0.1.2/src/va_am/__main__.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-04-10 08:50:52.080531 va_am-0.1.2/src/va_am/utils/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    61061 2024-02-16 14:28:14.000000 va_am-0.1.2/src/va_am/utils/AutoEncoders.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2023-06-29 15:33:10.000000 va_am-0.1.2/src/va_am/utils/__init__.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     3123 2023-09-25 14:36:24.000000 va_am-0.1.2/src/va_am/utils/functions.py
+-rw-r--r--   0 cosmin    (1000) cosmin    (1000)   102225 2024-04-05 12:17:06.000000 va_am-0.1.2/src/va_am/va_am.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-04-10 08:50:52.080531 va_am-0.1.2/src/va_am.egg-info/
+-rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-04-10 08:50:52.000000 va_am-0.1.2/src/va_am.egg-info/PKG-INFO
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      393 2024-04-10 08:50:52.000000 va_am-0.1.2/src/va_am.egg-info/SOURCES.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2024-04-10 08:50:52.000000 va_am-0.1.2/src/va_am.egg-info/dependency_links.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       46 2024-04-10 08:50:52.000000 va_am-0.1.2/src/va_am.egg-info/entry_points.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       71 2024-04-10 08:50:52.000000 va_am-0.1.2/src/va_am.egg-info/requires.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        6 2024-04-10 08:50:52.000000 va_am-0.1.2/src/va_am.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `va_am-0.1.1/LICENSE` & `va_am-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `va_am-0.1.1/PKG-INFO` & `va_am-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: va_am
-Version: 0.1.1
+Version: 0.1.2
 Summary: VA-AM method implementation
 Author-email: cosminmarina <cosmin.marina@uah.es>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,14 +682,23 @@
 Project-URL: Documentation, https://va-am.readthedocs.io/
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: sympy
+Requires-Dist: keras
+Requires-Dist: tensorflow
+Requires-Dist: xarray
+Requires-Dist: netcdf4
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: numpy
 
 # VA-AM
 
 <img src="https://raw.githubusercontent.com/cosminmarina/va_am/master/docs/_static/distribution.png" width="200" /> <img src="https://raw.githubusercontent.com/cosminmarina/va_am/master/docs/_static/identification.png" width="200" /> <img src="https://raw.githubusercontent.com/cosminmarina/va_am/master/docs/_static/identification2.png" width="200" /> <img src="https://raw.githubusercontent.com/cosminmarina/va_am/master/docs/_static/distribution2.png" width="200" />
 
 Documentation[#](#documentation "Permalink to this heading")
 --------------
```

### Comparing `va_am-0.1.1/README.md` & `va_am-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `va_am-0.1.1/pyproject.toml` & `va_am-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "va_am"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{name="cosminmarina", email="cosmin.marina@uah.es" }]
 description = "VA-AM method implementation"
 readme = "README.md"
 dependencies = ["requests","sympy","keras","tensorflow","xarray","netcdf4","matplotlib","pandas","numpy"]
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `va_am-0.1.1/src/va_am/utils/AutoEncoders.py` & `va_am-0.1.2/src/va_am/utils/AutoEncoders.py`

 * *Files identical despite different names*

### Comparing `va_am-0.1.1/src/va_am/utils/functions.py` & `va_am-0.1.2/src/va_am/utils/functions.py`

 * *Files identical despite different names*

### Comparing `va_am-0.1.1/src/va_am/va_am.py` & `va_am-0.1.2/src/va_am/va_am.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,20 +265,22 @@
     time_prediction = time_prs[minindex[:k]]
     prediction = data_temp.sel(time=time_prediction[:k])[temp_var_name].data
     prsf = data_prs[minindex[:k]]
 
     idx = np.random.choice(np.arange(prsf.shape[0]), size=iter, replace=replace_choice)
     
     selected_temp = prediction[idx,:,:]
+    #print(f'\nTime prediction: \n {np.shape(time_prediction)} \n {time_prediction}')
+    selected_time = time_prediction[idx]
     if is_not_encoded:
         selected_psr = prsf[idx,:,:,:]
     else:
         selected_psr = prsf[idx,:]
 
-    return selected_psr, selected_temp
+    return selected_psr, selected_temp, selected_time
 
 def calculate_interest_region(interest_region: Union[list, np.ndarray], latitude_min: int, latitude_max: int, longitude_min: int, longitude_max: int, resolution: Union[int, float] = 2, is_teleg: bool = False, secret_file:str = './secret.txt') -> list:
     """
       calculate_interest_region
        
       Method which transform latitude/longitude degrees to index. It is used to increase the speed of the methods by using numpy arrays insted of Dataset or DataArray.
         
@@ -537,20 +539,27 @@
             requests.get(url).json()
         raise message
         
     data_of_interest_temp = indust_temp.sel(time=slice(params["data_of_interest_init"],params["data_of_interest_end"]))
     data_of_interest_prs = indust_prs.sel(time=slice(params["data_of_interest_init"],params["data_of_interest_end"]))
     
     if params["remove_year"]:
-        indust_temp = indust_temp.drop_sel(time=(indust_temp.sel(time=slice(params["data_of_interest_init"][:4],params["data_of_interest_end"][:4]))).get_index('time'))
-        indust_prs = indust_prs.drop_sel(time=(indust_prs.sel(time=slice(params["data_of_interest_init"][:4],params["data_of_interest_end"][:4]))).get_index('time'))
+        print(params["data_of_interest_init"])
+        print(type(params["data_of_interest_init"]))
+        t_i = str(params["data_of_interest_init"].year)
+        t_f = str(params["data_of_interest_end"].year)
+        print(t_i, t_f)
+        a = (indust_temp.sel(time=slice(t_i,t_f))).get_index('time')
+        print(a)
+        indust_temp = indust_temp.drop_sel(time=(indust_temp.sel(time=slice(str(params["data_of_interest_init"].year),str(params["data_of_interest_end"].year)))).get_index('time'))
+        indust_prs = indust_prs.drop_sel(time=(indust_prs.sel(time=slice(str(params["data_of_interest_init"].year),str(params["data_of_interest_end"].year)))).get_index('time'))
         if params["period"] == 'pre':
             if datetime.datetime.strptime(params["data_of_interest_init"], "%Y-%m-%d") < datetime.datetime.strptime(params["pre_end"], "%Y-%m-%d"):
-                pre_indust_temp = pre_indust_temp.drop_sel(time=(pre_indust_temp.sel(time=slice(params["data_of_interest_init"][:4],params["data_of_interest_end"][:4]))).get_index('time'))
-                pre_indust_prs = pre_indust_prs.drop_sel(time=(pre_indust_prs.sel(time=slice(params["data_of_interest_init"][:4],params["data_of_interest_end"][:4]))).get_index('time'))        
+                pre_indust_temp = pre_indust_temp.drop_sel(time=(pre_indust_temp.sel(time=slice(str(params["data_of_interest_init"].year),str(params["data_of_interest_end"].year)))).get_index('time'))
+                pre_indust_prs = pre_indust_prs.drop_sel(time=(pre_indust_prs.sel(time=slice(str(params["data_of_interest_init"].year),str(params["data_of_interest_end"].year)))).get_index('time'))        
     else:
         indust_temp = indust_temp.drop_sel(time=(indust_temp.sel(time=slice(params["data_of_interest_init"],params["data_of_interest_end"]))).get_index('time'))
         indust_prs = indust_prs.drop_sel(time=(indust_prs.sel(time=slice(params["data_of_interest_init"],params["data_of_interest_end"]))).get_index('time'))
         if params["period"] == 'pre':
             if datetime.datetime.strptime(params["data_of_interest_init"], "%Y-%m-%d") < datetime.datetime.strptime(params["pre_end"], "%Y-%m-%d"):
                 pre_indust_temp = pre_indust_temp.drop_sel(time=(pre_indust_temp.sel(time=slice(params["data_of_interest_init"],params["data_of_interest_end"]))).get_index('time'))
                 pre_indust_prs = pre_indust_prs.drop_sel(time=(pre_indust_prs.sel(time=slice(params["data_of_interest_init"],params["data_of_interest_end"]))).get_index('time'))
@@ -856,49 +865,53 @@
     reconstruction_Pre_AE = []
     reconstruction_Post_Analog = []
     reconstruction_Post_AE = []
     for i in range(params["iter"]):
         if params["period"] in ['both', 'pre']:
             dict_stats[f'WithoutAE-Pre{i}'] = [np.abs(data_of_interest_prs - analog_pre[0][i]).sum()/img_size,
                                     np.abs(data_of_interest_temp[params["temp_var_name"]].data - analog_pre[1][i])[:,int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]].mean(),
-                                    analog_pre[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]].mean()-273.15]
+                                    analog_pre[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]].mean()-273.15,
+                                    str(analog_pre[2][i].data)[:10]]
             reconstruction_Pre_Analog.append(analog_pre[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]])
         else:
             dict_stats[f'WithoutAE-Pre{i}'] = [np.nan, np.nan, np.nan]
         
         if params["period"] in ['both', 'post']:
             dict_stats[f'WithoutAE-Post{i}'] = [np.abs(data_of_interest_prs - analog_ind[0][i]).sum()/img_size,
                                     np.abs(data_of_interest_temp[params["temp_var_name"]].data - analog_ind[1][i])[:,int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]].mean(),
-                                    analog_ind[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]].mean()-273.15]
+                                    analog_ind[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]].mean()-273.15,
+                                    str(analog_ind[2][i].data)[:10]]
             reconstruction_Post_Analog.append(analog_ind[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]])
         else:
             dict_stats[f'WithoutAE-Post{i}'] = [np.nan, np.nan, np.nan]
         
         if params["period"] in ['both', 'pre']:
             dict_stats[f'WithAE-Pre-Pre{i}'] = [np.abs(data_of_interest_prs_encoded_pre - latent_analog_pre[0][i]).sum()/img_size,
                                         np.abs(data_of_interest_temp[params["temp_var_name"]].data - latent_analog_pre[1][i])[:,int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]].mean(),
-                                        latent_analog_pre[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]].mean()-273.15]
+                                        latent_analog_pre[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]].mean()-273.15,
+                                        str(latent_analog_pre[2][i].data)[:10]]
             reconstruction_Pre_AE.append(latent_analog_pre[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]])
         else:
             dict_stats[f'WithAE-Pre-Pre{i}'] = [np.nan, np.nan, np.nan]
 
         if params["period"] in ['both', 'post']:
             dict_stats[f'WithAE-Post-Post{i}'] = [np.abs(data_of_interest_prs_encoded_ind - latent_analog_ind[0][i]).sum()/img_size,
                                     np.abs(data_of_interest_temp[params["temp_var_name"]].data - latent_analog_ind[1][i])[:,int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]].mean(),
-                                    latent_analog_ind[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]].mean()-273.15]
+                                    latent_analog_ind[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]].mean()-273.15,
+                                    str(latent_analog_ind[2][i].data)[:10]]
             reconstruction_Post_AE.append(latent_analog_ind[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]])
         else:
             dict_stats[f'WithAE-Post-Post{i}'] = [np.nan, np.nan, np.nan]
 
         dict_stats[f'Original{i}']=[0,0,((data_of_interest_temp[params["temp_var_name"]].data)[:,int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]]).mean()-273.15]
         
         if params["verbose"]:
             print(f'Iteration {i} finished')
 
-    df_stats = pd.DataFrame.from_dict(dict_stats,orient='index',columns=['prs-diff','temp-diff','temp'])
+    df_stats = pd.DataFrame.from_dict(dict_stats,orient='index',columns=['prs-diff','temp-diff','temp','time'])
     Path("./comparison-csv").mkdir(parents=True, exist_ok=True)
     df_stats.to_csv(f'./comparison-csv/{params["season"]}{params["name"]}x{params["iter"]}-{params["data_of_interest_init"]}-epoch{params["n_epochs"]}-latent{params["latent_dim"]}-k{params["k"]}-arch{params["arch"]}-{"VAE" if params["use_VAE"] else "noVAE"}-analog-comparision-stats{current.year}-{current.month}-{current.day}-{current.hour}-{current.minute}-{current.second}.csv'.replace(" ","").replace("'", "").replace(",",""))
     return reconstruction_Pre_Analog, reconstruction_Post_Analog, reconstruction_Pre_AE, reconstruction_Post_AE
 
 
 def identify_heatwave_days(params: dict) -> Union[list, np.ndarray]:
     """
```

### Comparing `va_am-0.1.1/src/va_am.egg-info/PKG-INFO` & `va_am-0.1.2/src/va_am.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: va-am
-Version: 0.1.1
+Name: va_am
+Version: 0.1.2
 Summary: VA-AM method implementation
 Author-email: cosminmarina <cosmin.marina@uah.es>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,14 +682,23 @@
 Project-URL: Documentation, https://va-am.readthedocs.io/
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: sympy
+Requires-Dist: keras
+Requires-Dist: tensorflow
+Requires-Dist: xarray
+Requires-Dist: netcdf4
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: numpy
 
 # VA-AM
 
 <img src="https://raw.githubusercontent.com/cosminmarina/va_am/master/docs/_static/distribution.png" width="200" /> <img src="https://raw.githubusercontent.com/cosminmarina/va_am/master/docs/_static/identification.png" width="200" /> <img src="https://raw.githubusercontent.com/cosminmarina/va_am/master/docs/_static/identification2.png" width="200" /> <img src="https://raw.githubusercontent.com/cosminmarina/va_am/master/docs/_static/distribution2.png" width="200" />
 
 Documentation[#](#documentation "Permalink to this heading")
 --------------
```

