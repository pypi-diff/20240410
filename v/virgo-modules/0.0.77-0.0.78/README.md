# Comparing `tmp/virgo_modules-0.0.77.tar.gz` & `tmp/virgo_modules-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgo_modules-0.0.77.tar", last modified: Mon Apr  8 18:00:08 2024, max compression
+gzip compressed data, was "virgo_modules-0.0.78.tar", last modified: Wed Apr 10 16:57:04 2024, max compression
```

## Comparing `virgo_modules-0.0.77.tar` & `virgo_modules-0.0.78.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 18:00:08.665646 virgo_modules-0.0.77/
--rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.77/LICENSE
--rw-rw-rw-   0        0        0      859 2024-04-08 18:00:08.662644 virgo_modules-0.0.77/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.77/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 18:00:08.665646 virgo_modules-0.0.77/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-04-08 17:58:53.000000 virgo_modules-0.0.77/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:00:08.581644 virgo_modules-0.0.77/virgo_app/
-drwxrwxrwx   0        0        0        0 2024-04-08 18:00:08.606644 virgo_modules-0.0.77/virgo_app/virgo_modules/
--rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.77/virgo_app/virgo_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:00:08.659650 virgo_modules-0.0.77/virgo_app/virgo_modules/src/
--rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.77/virgo_app/virgo_modules/src/__init__.py
--rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.77/virgo_app/virgo_modules/src/aws_utils.py
--rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.77/virgo_app/virgo_modules/src/edge_utils.py
--rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.77/virgo_app/virgo_modules/src/pull_artifacts.py
--rw-rw-rw-   0        0        0    64053 2024-04-04 18:20:37.000000 virgo_modules-0.0.77/virgo_app/virgo_modules/src/re_utils.py
--rw-rw-rw-   0        0        0   142729 2024-04-08 17:58:53.000000 virgo_modules-0.0.77/virgo_app/virgo_modules/src/ticketer_source.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:00:08.628644 virgo_modules-0.0.77/virgo_app/virgo_modules.egg-info/
--rw-rw-rw-   0        0        0      859 2024-04-08 18:00:07.000000 virgo_modules-0.0.77/virgo_app/virgo_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-04-08 18:00:07.000000 virgo_modules-0.0.77/virgo_app/virgo_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 18:00:07.000000 virgo_modules-0.0.77/virgo_app/virgo_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      276 2024-04-08 18:00:07.000000 virgo_modules-0.0.77/virgo_app/virgo_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-08 18:00:07.000000 virgo_modules-0.0.77/virgo_app/virgo_modules.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 16:57:04.881308 virgo_modules-0.0.78/
+-rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.78/LICENSE
+-rw-rw-rw-   0        0        0     1411 2024-04-10 16:57:04.875333 virgo_modules-0.0.78/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.78/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 16:57:04.882305 virgo_modules-0.0.78/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-04-10 16:49:15.000000 virgo_modules-0.0.78/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:57:04.672096 virgo_modules-0.0.78/virgo_app/
+drwxrwxrwx   0        0        0        0 2024-04-10 16:57:04.682094 virgo_modules-0.0.78/virgo_app/virgo_modules/
+-rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.78/virgo_app/virgo_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:57:04.867304 virgo_modules-0.0.78/virgo_app/virgo_modules/src/
+-rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.78/virgo_app/virgo_modules/src/__init__.py
+-rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.78/virgo_app/virgo_modules/src/aws_utils.py
+-rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.78/virgo_app/virgo_modules/src/edge_utils.py
+-rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.78/virgo_app/virgo_modules/src/pull_artifacts.py
+-rw-rw-rw-   0        0        0    67272 2024-04-10 16:56:38.000000 virgo_modules-0.0.78/virgo_app/virgo_modules/src/re_utils.py
+-rw-rw-rw-   0        0        0   142729 2024-04-08 17:58:53.000000 virgo_modules-0.0.78/virgo_app/virgo_modules/src/ticketer_source.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:57:04.720096 virgo_modules-0.0.78/virgo_app/virgo_modules.egg-info/
+-rw-rw-rw-   0        0        0     1411 2024-04-10 16:57:03.000000 virgo_modules-0.0.78/virgo_app/virgo_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-04-10 16:57:04.000000 virgo_modules-0.0.78/virgo_app/virgo_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 16:57:03.000000 virgo_modules-0.0.78/virgo_app/virgo_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      276 2024-04-10 16:57:03.000000 virgo_modules-0.0.78/virgo_app/virgo_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-10 16:57:03.000000 virgo_modules-0.0.78/virgo_app/virgo_modules.egg-info/top_level.txt
```

### Comparing `virgo_modules-0.0.77/LICENSE` & `virgo_modules-0.0.78/LICENSE`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.77/setup.py` & `virgo_modules-0.0.78/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("virgo_app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="virgo_modules",
-    version="0.0.77",
+    version="0.0.78",
     description="data processing and statistical modeling using stock market data",
     package_dir={"": "virgo_app"},
     packages=find_packages(where="virgo_app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelmayhem92/virgo_module",
     author="Miguel Mayhuire",
```

### Comparing `virgo_modules-0.0.77/virgo_app/virgo_modules/src/aws_utils.py` & `virgo_modules-0.0.78/virgo_app/virgo_modules/src/aws_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.77/virgo_app/virgo_modules/src/edge_utils.py` & `virgo_modules-0.0.78/virgo_app/virgo_modules/src/edge_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.77/virgo_app/virgo_modules/src/pull_artifacts.py` & `virgo_modules-0.0.78/virgo_app/virgo_modules/src/pull_artifacts.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.77/virgo_app/virgo_modules/src/re_utils.py` & `virgo_modules-0.0.78/virgo_app/virgo_modules/src/re_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1385,14 +1385,15 @@
         
     if save_path and save_aws:
         upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = save_aws + result_json_name, input_path = save_path+result_json_name, aws_credentials = aws_credentials)
         
     if show_result:
         print(curent_edge)
 
+## this function is going to be split and deprecated
 def create_feature_edge(model, data,feature_name, threshold, target_variables):
     '''
     get latest edge execution and edge probability
 
             Parameters:
                     model (obj): edge model artifact
                     data (pd.DataFrame): asset data
@@ -1413,8 +1414,78 @@
         type_use = 'low'
         if 'down' in pred_col:
             type_use = 'up' 
             
         result_df[f'signal_{type_use}_{feature_name}'] = np.where(result_df[pred_col] >= threshold,1,0)
         result_df[f'acc_{type_use}_{feature_name}'] = np.where(result_df[f'signal_{type_use}_{feature_name}'] == result_df[pred_col.replace('proba_','')],1,0)
     
-    return result_df
+    return result_df
+
+def produce_probas(model,data, target_variables):
+    """
+    produce probabilities given a model
+
+            Parameters:
+                    model (obj): edge model artifact
+                    data (pd.DataFrame): asset data
+                    target_variables (list): names of the target columns
+
+            Returns:
+                    result_df (pd.DataFrame): result dataframe with edges
+                    label_prediction (list): list of resulting label columns
+    """
+    label_prediction = ['proba_'+x for x in target_variables]
+    predictions = model.predict_proba(data)
+    predictions = pd.DataFrame(predictions, columns = label_prediction, index = data.index)
+    
+    result_df = pd.concat([data, predictions], axis=1)
+    result_df = result_df[['Date'] + target_variables + label_prediction]
+
+    return result_df, label_prediction
+
+def produce_signals(result_df, feature_name, threshold, label_prediction):
+    """
+    produce signals from probabilities
+
+            Parameters:
+                    result_df (pd.DataFrame): asset data with probabilities
+                    feature_name (str): edge feature name
+                    threshold (float): edge threshold
+                    label_prediction (list): list of resulting label columns
+
+            Returns:
+                    result_df (pd.DataFrame): result dataframe with edges and signals
+    """
+    for pred_col in label_prediction:
+        type_use = 'low'
+        if 'down' in pred_col:
+            type_use = 'up' 
+            
+        result_df[f'signal_{type_use}_{feature_name}'] = np.where(result_df[pred_col] >= threshold,1,0)
+        result_df[f'acc_{type_use}_{feature_name}'] = np.where(result_df[f'signal_{type_use}_{feature_name}'] == result_df[pred_col.replace('proba_','')],1,0)
+
+    return result_df
+
+def edge_probas_lines(data, threshold, plot = False, look_back = 750):
+    """
+    produce a plotly plot of edges and closing prices
+
+            Parameters:
+                    data (pd.DataFrame): asset data with edge probabilities
+                    plot (boolean): if true, display plot
+                    threshold (float): edge threshold
+                    look_back (int): number of rows back to display
+
+            Returns:
+                    fig (obj): plotly go object
+    """
+    df = data[['Date','Close','proba_target_down','proba_target_up']].iloc[-look_back:]
+    
+    fig = make_subplots(specs=[[{"secondary_y": True}]])
+    fig.add_trace(go.Scatter(x=df.Date, y=df.Close,mode='lines+markers',name='Close price'))
+    fig.add_trace(go.Scatter(x=df.Date, y=df.proba_target_down,mode='lines',marker = dict(color = 'coral'),name='go down'),secondary_y=True)
+    fig.add_trace(go.Scatter(x=df.Date, y=df.proba_target_up,mode='lines',marker = dict(opacity=0.1,size=80), name='go up'),secondary_y=True)
+    fig.add_shape(type="line", xref="paper", yref="y2",x0=0.02, y0=threshold, x1=0.9, y1=threshold,line=dict(color="red",dash="dash"),)
+    fig.update_layout(title_text="sirius - edge probabilities",width=1200,height = 500)
+    if plot:
+        fig.show()
+    return fig
```

### Comparing `virgo_modules-0.0.77/virgo_app/virgo_modules/src/ticketer_source.py` & `virgo_modules-0.0.78/virgo_app/virgo_modules/src/ticketer_source.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.77/virgo_app/virgo_modules.egg-info/SOURCES.txt` & `virgo_modules-0.0.78/virgo_app/virgo_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

