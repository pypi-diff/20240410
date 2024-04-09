# Comparing `tmp/scorecard_generator-2.1.8.tar.gz` & `tmp/scorecard_generator-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorecard_generator-2.1.8.tar", last modified: Tue Apr  9 18:37:21 2024, max compression
+gzip compressed data, was "scorecard_generator-2.1.9.tar", last modified: Tue Apr  9 21:24:28 2024, max compression
```

## Comparing `scorecard_generator-2.1.8.tar` & `scorecard_generator-2.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 18:37:21.559526 scorecard_generator-2.1.8/
--rw-rw-rw-   0        0        0     1088 2024-01-22 03:40:39.000000 scorecard_generator-2.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0    10351 2024-04-09 18:37:21.555987 scorecard_generator-2.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     9212 2024-04-09 18:37:03.000000 scorecard_generator-2.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 18:37:21.508652 scorecard_generator-2.1.8/scorecard_generator/
--rw-rw-rw-   0        0        0      201 2024-03-18 05:47:42.000000 scorecard_generator-2.1.8/scorecard_generator/__init__.py
--rw-rw-rw-   0        0        0    13118 2024-04-09 18:31:25.000000 scorecard_generator-2.1.8/scorecard_generator/scorecard.py
-drwxrwxrwx   0        0        0        0 2024-04-09 18:37:21.539705 scorecard_generator-2.1.8/scorecard_generator.egg-info/
--rw-rw-rw-   0        0        0    10351 2024-04-09 18:37:21.000000 scorecard_generator-2.1.8/scorecard_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-04-09 18:37:21.000000 scorecard_generator-2.1.8/scorecard_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 18:37:21.000000 scorecard_generator-2.1.8/scorecard_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-09 18:37:21.000000 scorecard_generator-2.1.8/scorecard_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-09 18:37:21.000000 scorecard_generator-2.1.8/scorecard_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 18:37:21.559526 scorecard_generator-2.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1328 2024-04-09 18:36:41.000000 scorecard_generator-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 21:24:28.883145 scorecard_generator-2.1.9/
+-rw-rw-rw-   0        0        0     1088 2024-01-22 03:40:39.000000 scorecard_generator-2.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0    10351 2024-04-09 21:24:28.867506 scorecard_generator-2.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9212 2024-04-09 21:24:17.000000 scorecard_generator-2.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 21:24:28.807496 scorecard_generator-2.1.9/scorecard_generator/
+-rw-rw-rw-   0        0        0      201 2024-03-18 05:47:42.000000 scorecard_generator-2.1.9/scorecard_generator/__init__.py
+-rw-rw-rw-   0        0        0    14154 2024-04-09 21:23:15.000000 scorecard_generator-2.1.9/scorecard_generator/scorecard.py
+drwxrwxrwx   0        0        0        0 2024-04-09 21:24:28.867506 scorecard_generator-2.1.9/scorecard_generator.egg-info/
+-rw-rw-rw-   0        0        0    10351 2024-04-09 21:24:28.000000 scorecard_generator-2.1.9/scorecard_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-04-09 21:24:28.000000 scorecard_generator-2.1.9/scorecard_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 21:24:28.000000 scorecard_generator-2.1.9/scorecard_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-09 21:24:28.000000 scorecard_generator-2.1.9/scorecard_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-09 21:24:28.000000 scorecard_generator-2.1.9/scorecard_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 21:24:28.883145 scorecard_generator-2.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2024-04-09 21:24:10.000000 scorecard_generator-2.1.9/setup.py
```

### Comparing `scorecard_generator-2.1.8/LICENSE.txt` & `scorecard_generator-2.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scorecard_generator-2.1.8/PKG-INFO` & `scorecard_generator-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecard_generator
-Version: 2.1.8
+Version: 2.1.9
 Summary: A Python Library for Creating Scorecards From Classification Models.
 Home-page: https://github.com/knowusuboaky/scorecard_generator
 Author: Kwadwo Daddy Nyame Owusu - Boakye
 Author-email: kwadwo.owusuboakye@outlook.com
 Keywords: scorecard,classification,woe,linear,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -41,15 +41,15 @@
 
 ## Installation
 
 You can install the Scorecard Generator via pip:
 
 ``` bash
 
-pip install scorecard_generator==2.1.8
+pip install scorecard_generator==2.1.9
 ```
 
 ## Load Package
 ``` bash
 
 from scorecard_generator import scorecard
 ```
```

### Comparing `scorecard_generator-2.1.8/README.md` & `scorecard_generator-2.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ## Installation
 
 You can install the Scorecard Generator via pip:
 
 ``` bash
 
-pip install scorecard_generator==2.1.8
+pip install scorecard_generator==2.1.9
 ```
 
 ## Load Package
 ``` bash
 
 from scorecard_generator import scorecard
 ```
```

### Comparing `scorecard_generator-2.1.8/scorecard_generator/scorecard.py` & `scorecard_generator-2.1.9/scorecard_generator/scorecard.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,23 +193,46 @@
             coeff_df = pd.concat([coeff_df, intercept_df], ignore_index=True)
         else:
             print("Model does not provide coefficients or feature importances.")
             return None
     except AttributeError:
         return "This classification method does not support this operation."
 
+    # Create the new column by splitting the "Feature Name" at the first underscore and keeping the part before it
+    coeff_df['Category'] = coeff_df['Feature Name'].apply(lambda x: x.split('_', 1)[0])
+
     # Calculate min and max sum of coefficients excluding the intercept
-    min_coef = coeff_df[coeff_df['Feature Name'] != 'Intercept']['Coefficients'].min()
-    max_coef = coeff_df[coeff_df['Feature Name'] != 'Intercept']['Coefficients'].max()
-    min_sum_coef = min_coef
-    max_sum_coef = max_coef
 
-    # Score calculation for all features
-    coeff_df['Score - Calculation'] = (coeff_df['Coefficients'] * (max_score - min_score) / (max_sum_coef - min_sum_coef)).round().astype(int)
-    
+    ## Minimum sum of coefficient
+    min_sum_coef = coeff_df.groupby('Category')['Coefficients'].min().sum()
+    max_sum_coef = coeff_df.groupby('Category')['Coefficients'].min().sum()
+
+    # Ensure the denominator is not zero to avoid division by zero
+    denominator = max_sum_coef - min_sum_coef
+    if denominator == 0:
+
+        min_sum_coef = coeff_df['Coefficients'].min()
+        max_sum_coef = coeff_df['Coefficients'].max()
+
+        denominator = max_sum_coef - min_sum_coef
+        if denominator == 0:
+            raise ValueError("Coefficient variation is zero: Please verify the input data or consider using a model that can handle this scenario.")
+
+    # Perform the calculation
+    coeff_df['Score - Calculation'] = coeff_df['Coefficients'] * (max_score - min_score) / denominator
+
+
+    # Now, safely convert to integers
+    # Check for and handle infinite values
+    coeff_df['Score - Calculation'] = np.where(np.isfinite(coeff_df['Score - Calculation']), coeff_df['Score - Calculation'].round(), np.nan)
+
+    # Replace NaN values in 'Coefficients' with 0 before calculation
+    coeff_df['Coefficients'].fillna(0, inplace=True)
+    coeff_df['Score - Calculation'] = coeff_df['Score - Calculation'].astype(int)
+
     # Find the position of the intercept
     n = coeff_df.index[coeff_df['Feature Name'] == 'Intercept'].tolist()[0]
     
     # Update the calculated score of the Intercept
     coeff_df.loc[n, 'Score - Calculation'] = (
         ((coeff_df.loc[n, 'Coefficients'] - min_sum_coef) / 
         (max_sum_coef - min_sum_coef)) * (max_score - min_score) + min_score).round().astype(int)
```

### Comparing `scorecard_generator-2.1.8/scorecard_generator.egg-info/PKG-INFO` & `scorecard_generator-2.1.9/scorecard_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecard_generator
-Version: 2.1.8
+Version: 2.1.9
 Summary: A Python Library for Creating Scorecards From Classification Models.
 Home-page: https://github.com/knowusuboaky/scorecard_generator
 Author: Kwadwo Daddy Nyame Owusu - Boakye
 Author-email: kwadwo.owusuboakye@outlook.com
 Keywords: scorecard,classification,woe,linear,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -41,15 +41,15 @@
 
 ## Installation
 
 You can install the Scorecard Generator via pip:
 
 ``` bash
 
-pip install scorecard_generator==2.1.8
+pip install scorecard_generator==2.1.9
 ```
 
 ## Load Package
 ``` bash
 
 from scorecard_generator import scorecard
 ```
```

### Comparing `scorecard_generator-2.1.8/setup.py` & `scorecard_generator-2.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='scorecard_generator',
-    version='2.1.8',
+    version='2.1.9',
     packages=find_packages(),
     description='A Python Library for Creating Scorecards From Classification Models.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Kwadwo Daddy Nyame Owusu - Boakye',
     author_email='kwadwo.owusuboakye@outlook.com',
     url='https://github.com/knowusuboaky/scorecard_generator',
```

