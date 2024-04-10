# Comparing `tmp/wolta-0.1.7.tar.gz` & `tmp/wolta-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolta-0.1.7.tar", last modified: Sat Apr  6 14:27:52 2024, max compression
+gzip compressed data, was "wolta-0.1.8.tar", last modified: Wed Apr 10 00:51:45 2024, max compression
```

## Comparing `wolta-0.1.7.tar` & `wolta-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 14:27:52.808456 wolta-0.1.7/
--rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0    15098 2024-04-06 14:27:52.807434 wolta-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    13874 2024-04-02 23:36:26.000000 wolta-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 14:27:52.808456 wolta-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1209 2024-04-06 14:27:50.000000 wolta-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 14:27:52.784788 wolta-0.1.7/wolta/
--rw-rw-rw-   0        0        0      113 2024-03-31 11:58:39.000000 wolta-0.1.7/wolta/__init__.py
--rw-rw-rw-   0        0        0     7843 2024-04-06 14:27:03.000000 wolta-0.1.7/wolta/data_tools.py
--rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.1.7/wolta/feature_tools.py
--rw-rw-rw-   0        0        0    18051 2024-04-06 14:08:07.000000 wolta-0.1.7/wolta/model_tools.py
--rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.1.7/wolta/progressive_tools.py
-drwxrwxrwx   0        0        0        0 2024-04-06 14:27:52.805801 wolta-0.1.7/wolta.egg-info/
--rw-rw-rw-   0        0        0    15098 2024-04-06 14:27:52.000000 wolta-0.1.7/wolta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-04-06 14:27:52.000000 wolta-0.1.7/wolta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 14:27:52.000000 wolta-0.1.7/wolta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-06 14:27:52.000000 wolta-0.1.7/wolta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       61 2024-04-06 14:27:52.000000 wolta-0.1.7/wolta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 00:51:45.072917 wolta-0.1.8/
+-rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0    17575 2024-04-10 00:51:45.072917 wolta-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    16268 2024-04-10 00:49:00.000000 wolta-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 00:51:45.073954 wolta-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2024-04-10 00:51:27.000000 wolta-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 00:51:45.022791 wolta-0.1.8/wolta/
+-rw-rw-rw-   0        0        0      113 2024-03-31 11:58:39.000000 wolta-0.1.8/wolta/__init__.py
+-rw-rw-rw-   0        0        0    11272 2024-04-10 00:37:03.000000 wolta-0.1.8/wolta/data_tools.py
+-rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.1.8/wolta/feature_tools.py
+-rw-rw-rw-   0        0        0    18051 2024-04-06 14:08:07.000000 wolta-0.1.8/wolta/model_tools.py
+-rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.1.8/wolta/progressive_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-10 00:51:45.071893 wolta-0.1.8/wolta.egg-info/
+-rw-rw-rw-   0        0        0    17575 2024-04-10 00:51:44.000000 wolta-0.1.8/wolta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-10 00:51:44.000000 wolta-0.1.8/wolta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 00:51:44.000000 wolta-0.1.8/wolta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-10 00:51:44.000000 wolta-0.1.8/wolta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       61 2024-04-10 00:51:44.000000 wolta-0.1.8/wolta.egg-info/top_level.txt
```

### Comparing `wolta-0.1.7/LICENSE.txt` & `wolta-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wolta-0.1.7/PKG-INFO` & `wolta-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.1.7
+Version: 0.1.8
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -109,14 +109,66 @@
 
 df = pd.read_csv('data.csv')
 df['output'] = make_numerics(df['output'])
 ```
 
 ***
 
+### transform_data
+
+**Returns**:
+1. transformed X
+2. transformed y
+3. if strategy ends with 'm', amin_x
+4. if strategy ends with 'm', amin_y
+
+**Parameters**:
+
+* X
+* y
+* strategy, {'log', 'log-m', 'log2', 'log2-m', 'log10', 'log10-m', 'sqrt', 'sqrt-m', 'cbrt'}, by default 'log-m'
+
+If you concern about situations like sqrt(0) or log(0), use strategies which ends with 'm' (means manipulated).
+
+***
+
+### transform_pred
+
+This function is designed for make predictions realistic and handles back-transformation.
+
+**Returns**: back-transformed y
+
+**Parameters**:
+
+* y_pred
+* strategy, {'log', 'log-m', 'log2', 'log2-m', 'log10', 'log10-m', 'sqrt', 'sqrt-m', 'cbrt'}, by default 'log-m'
+* amin_y, int, by default 0. amin_y is used min y value in transform_data if data was manipulated and it is required if a strategy which ends with 'm' was selected.
+
+***
+
+### make_categorical
+
+It places regression outputs into three sub-classes according to mean and standard deviation. Normal distribution is required.
+
+**Returns**: 
+1. y
+the other outputs are returned if only normal-extra is selected
+2. the min value of array
+3. the max value of array
+4. the standard deviation of array
+5. the mean value of array
+6. the result of mean - standard deviation
+7. the result of mean + standard deviation
+
+**Parameters**:
+* y
+* strategy, {'normal', 'normal-extra'}, default by, 'normal'
+
+***
+
 ### create_chunks
 
 **Parameters**:
 
 * path, _string_
 * sample_amount, _int_, sample amount for each chunk
 * target_dir, _string_, directory path to save chunks, by default, None
@@ -175,14 +227,24 @@
 
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
 X_train, X_test = scale_x(X_train, X_test)
 ```
 
 ***
 
+### is_normal
+
+**Returns**: Boolean
+<br>
+if data has normal distribution returns true, else returns false
+<br>
+**Parameter**: y
+
+***
+
 ### examine_floats
 
 **Returns**: _list_ with full of column names which supplies the requested situation
 
 **Parameters**:
 * df, _pandas dataframe_
 * float_columns, _string list_, column names which has float data
@@ -370,14 +432,35 @@
 This class has those functions:
 
 * fit(X_train, y_train)
 * predict(X_test), returns y_pred
 
 ***
 
+### DistRegressor
+
+This regression approach provides a hybrid solution for problems which have output space in wide range thanks to normal distribution. 
+
+**Parameters**:
+* verbose, boolean, by default, True
+* clf_model, classification model class, by default, None (If it is None, CatBoostClassifier is used with default parameters except iterations, iterations has 20 as value)
+* clf_params, parameters for classification model in dict form, by default, None
+* reg_model, regression model, by default, None (If it is None, CatBoostRegressor is used with default parameters except iterations, iterations has 20 as value)
+* reg_params, parameters for regression model in dict form, by default, None
+
+This class has those functions:
+
+* fit(X_train, y_train)
+* predict(X_test), returns y_pred
+
+***
+
+
+***
+
 ### examine_time
 
 It calculates the fitting time for a model and also returns the trained model.
 
 **Returns**: 
 1. int
 2. model
```

### Comparing `wolta-0.1.7/README.md` & `wolta-0.1.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -86,14 +86,66 @@
 
 df = pd.read_csv('data.csv')
 df['output'] = make_numerics(df['output'])
 ```
 
 ***
 
+### transform_data
+
+**Returns**:
+1. transformed X
+2. transformed y
+3. if strategy ends with 'm', amin_x
+4. if strategy ends with 'm', amin_y
+
+**Parameters**:
+
+* X
+* y
+* strategy, {'log', 'log-m', 'log2', 'log2-m', 'log10', 'log10-m', 'sqrt', 'sqrt-m', 'cbrt'}, by default 'log-m'
+
+If you concern about situations like sqrt(0) or log(0), use strategies which ends with 'm' (means manipulated).
+
+***
+
+### transform_pred
+
+This function is designed for make predictions realistic and handles back-transformation.
+
+**Returns**: back-transformed y
+
+**Parameters**:
+
+* y_pred
+* strategy, {'log', 'log-m', 'log2', 'log2-m', 'log10', 'log10-m', 'sqrt', 'sqrt-m', 'cbrt'}, by default 'log-m'
+* amin_y, int, by default 0. amin_y is used min y value in transform_data if data was manipulated and it is required if a strategy which ends with 'm' was selected.
+
+***
+
+### make_categorical
+
+It places regression outputs into three sub-classes according to mean and standard deviation. Normal distribution is required.
+
+**Returns**: 
+1. y
+the other outputs are returned if only normal-extra is selected
+2. the min value of array
+3. the max value of array
+4. the standard deviation of array
+5. the mean value of array
+6. the result of mean - standard deviation
+7. the result of mean + standard deviation
+
+**Parameters**:
+* y
+* strategy, {'normal', 'normal-extra'}, default by, 'normal'
+
+***
+
 ### create_chunks
 
 **Parameters**:
 
 * path, _string_
 * sample_amount, _int_, sample amount for each chunk
 * target_dir, _string_, directory path to save chunks, by default, None
@@ -152,14 +204,24 @@
 
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
 X_train, X_test = scale_x(X_train, X_test)
 ```
 
 ***
 
+### is_normal
+
+**Returns**: Boolean
+<br>
+if data has normal distribution returns true, else returns false
+<br>
+**Parameter**: y
+
+***
+
 ### examine_floats
 
 **Returns**: _list_ with full of column names which supplies the requested situation
 
 **Parameters**:
 * df, _pandas dataframe_
 * float_columns, _string list_, column names which has float data
@@ -347,14 +409,35 @@
 This class has those functions:
 
 * fit(X_train, y_train)
 * predict(X_test), returns y_pred
 
 ***
 
+### DistRegressor
+
+This regression approach provides a hybrid solution for problems which have output space in wide range thanks to normal distribution. 
+
+**Parameters**:
+* verbose, boolean, by default, True
+* clf_model, classification model class, by default, None (If it is None, CatBoostClassifier is used with default parameters except iterations, iterations has 20 as value)
+* clf_params, parameters for classification model in dict form, by default, None
+* reg_model, regression model, by default, None (If it is None, CatBoostRegressor is used with default parameters except iterations, iterations has 20 as value)
+* reg_params, parameters for regression model in dict form, by default, None
+
+This class has those functions:
+
+* fit(X_train, y_train)
+* predict(X_test), returns y_pred
+
+***
+
+
+***
+
 ### examine_time
 
 It calculates the fitting time for a model and also returns the trained model.
 
 **Returns**: 
 1. int
 2. model
```

### Comparing `wolta-0.1.7/setup.py` & `wolta-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 DESCRIPTION = 'Data Science Library'
 LONG_DESCRIPTION = 'A package for data science'
 
 setup(
     name="wolta",
     version=VERSION,
     author="iamalreadynoob",
```

### Comparing `wolta-0.1.7/wolta/feature_tools.py` & `wolta-0.1.8/wolta/feature_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.7/wolta/model_tools.py` & `wolta-0.1.8/wolta/model_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.7/wolta/progressive_tools.py` & `wolta-0.1.8/wolta/progressive_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.7/wolta.egg-info/PKG-INFO` & `wolta-0.1.8/wolta.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.1.7
+Version: 0.1.8
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -109,14 +109,66 @@
 
 df = pd.read_csv('data.csv')
 df['output'] = make_numerics(df['output'])
 ```
 
 ***
 
+### transform_data
+
+**Returns**:
+1. transformed X
+2. transformed y
+3. if strategy ends with 'm', amin_x
+4. if strategy ends with 'm', amin_y
+
+**Parameters**:
+
+* X
+* y
+* strategy, {'log', 'log-m', 'log2', 'log2-m', 'log10', 'log10-m', 'sqrt', 'sqrt-m', 'cbrt'}, by default 'log-m'
+
+If you concern about situations like sqrt(0) or log(0), use strategies which ends with 'm' (means manipulated).
+
+***
+
+### transform_pred
+
+This function is designed for make predictions realistic and handles back-transformation.
+
+**Returns**: back-transformed y
+
+**Parameters**:
+
+* y_pred
+* strategy, {'log', 'log-m', 'log2', 'log2-m', 'log10', 'log10-m', 'sqrt', 'sqrt-m', 'cbrt'}, by default 'log-m'
+* amin_y, int, by default 0. amin_y is used min y value in transform_data if data was manipulated and it is required if a strategy which ends with 'm' was selected.
+
+***
+
+### make_categorical
+
+It places regression outputs into three sub-classes according to mean and standard deviation. Normal distribution is required.
+
+**Returns**: 
+1. y
+the other outputs are returned if only normal-extra is selected
+2. the min value of array
+3. the max value of array
+4. the standard deviation of array
+5. the mean value of array
+6. the result of mean - standard deviation
+7. the result of mean + standard deviation
+
+**Parameters**:
+* y
+* strategy, {'normal', 'normal-extra'}, default by, 'normal'
+
+***
+
 ### create_chunks
 
 **Parameters**:
 
 * path, _string_
 * sample_amount, _int_, sample amount for each chunk
 * target_dir, _string_, directory path to save chunks, by default, None
@@ -175,14 +227,24 @@
 
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
 X_train, X_test = scale_x(X_train, X_test)
 ```
 
 ***
 
+### is_normal
+
+**Returns**: Boolean
+<br>
+if data has normal distribution returns true, else returns false
+<br>
+**Parameter**: y
+
+***
+
 ### examine_floats
 
 **Returns**: _list_ with full of column names which supplies the requested situation
 
 **Parameters**:
 * df, _pandas dataframe_
 * float_columns, _string list_, column names which has float data
@@ -370,14 +432,35 @@
 This class has those functions:
 
 * fit(X_train, y_train)
 * predict(X_test), returns y_pred
 
 ***
 
+### DistRegressor
+
+This regression approach provides a hybrid solution for problems which have output space in wide range thanks to normal distribution. 
+
+**Parameters**:
+* verbose, boolean, by default, True
+* clf_model, classification model class, by default, None (If it is None, CatBoostClassifier is used with default parameters except iterations, iterations has 20 as value)
+* clf_params, parameters for classification model in dict form, by default, None
+* reg_model, regression model, by default, None (If it is None, CatBoostRegressor is used with default parameters except iterations, iterations has 20 as value)
+* reg_params, parameters for regression model in dict form, by default, None
+
+This class has those functions:
+
+* fit(X_train, y_train)
+* predict(X_test), returns y_pred
+
+***
+
+
+***
+
 ### examine_time
 
 It calculates the fitting time for a model and also returns the trained model.
 
 **Returns**: 
 1. int
 2. model
```

