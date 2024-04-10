# Comparing `tmp/fintoolsap-1.6.7.tar.gz` & `tmp/fintoolsap-1.6.8.tar.gz`

## Comparing `fintoolsap-1.6.7.tar` & `fintoolsap-1.6.8.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/FinToolsAP.code-workspace
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/FinToolsAP.yaml
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/src/FinToolsAP/Decorators.py
--rw-r--r--   0        0        0    19279 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/src/FinToolsAP/LaTeXBuilder.py
--rw-r--r--   0        0        0    70970 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/src/FinToolsAP/LocalDatabase.py
--rw-r--r--   0        0        0    32200 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/src/FinToolsAP/PortfolioSorts.py
--rw-r--r--   0        0        0    37157 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/src/FinToolsAP/UtilityFunctions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/src/FinToolsAP/__init__.py
--rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/src/FinToolsAP/_config.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/src/FinToolsAP/_download_script.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/src/FinToolsAP/_util_funcs.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/src/FinToolsAP/base_files/DatabaseParameters.py
--rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/src/FinToolsAP/base_files/ExampleCreateTable.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/src/FinToolsAP/base_files/ExampleExtraScript.py
--rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_BMME_sorts.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_Bond.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_DB_construction.py
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_FF_factors.py
--rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_breakpoint_construction.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_create_all_factors.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_csv_import.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_csv_to_sql.py
--rw-r--r--   0        0        0    27112 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_martin_output.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_query_BTDS.py
--rw-r--r--   0        0        0    30780 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_query_Bank.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_query_CRSP.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_query_CRSPMF.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_query_Factors.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_query_IBES.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_query_IH.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_query_MF.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_query_MFCH.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_query_MFHoldings.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_query_MFLinks.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_score_characteristics.py
--rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_sorting.py
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_univariate_sorts.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/TEST_virtual_environment.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/tests/test.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/LICENSE
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/pyproject.toml
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 fintoolsap-1.6.7/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/FinToolsAP.code-workspace
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/FinToolsAP.yaml
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/src/FinToolsAP/Decorators.py
+-rw-r--r--   0        0        0    19279 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/src/FinToolsAP/LaTeXBuilder.py
+-rw-r--r--   0        0        0    72335 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/src/FinToolsAP/LocalDatabase.py
+-rw-r--r--   0        0        0    32200 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/src/FinToolsAP/PortfolioSorts.py
+-rw-r--r--   0        0        0    44601 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/src/FinToolsAP/UtilityFunctions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/src/FinToolsAP/__init__.py
+-rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/src/FinToolsAP/_config.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/src/FinToolsAP/_download_script.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/src/FinToolsAP/_util_funcs.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/src/FinToolsAP/base_files/DatabaseParameters.py
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/src/FinToolsAP/base_files/ExampleCreateTable.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/src/FinToolsAP/base_files/ExampleExtraScript.py
+-rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_BMME_sorts.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_Bond.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_DB_construction.py
+-rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_FF_factors.py
+-rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_breakpoint_construction.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_create_all_factors.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_csv_import.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_csv_to_sql.py
+-rw-r--r--   0        0        0    27112 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_martin_output.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_query_BTDS.py
+-rw-r--r--   0        0        0    30780 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_query_Bank.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_query_CRSP.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_query_CRSPMF.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_query_Factors.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_query_IBES.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_query_IH.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_query_MF.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_query_MFCH.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_query_MFHoldings.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_query_MFLinks.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_raw_query.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_score_characteristics.py
+-rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_sorting.py
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_univariate_sorts.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/TEST_virtual_environment.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/tests/test.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/LICENSE
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/README.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/pyproject.toml
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 fintoolsap-1.6.8/PKG-INFO
```

### Comparing `fintoolsap-1.6.7/src/FinToolsAP/Decorators.py` & `fintoolsap-1.6.8/src/FinToolsAP/Decorators.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/src/FinToolsAP/LaTeXBuilder.py` & `fintoolsap-1.6.8/src/FinToolsAP/LaTeXBuilder.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/src/FinToolsAP/LocalDatabase.py` & `fintoolsap-1.6.8/src/FinToolsAP/LocalDatabase.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
  
 # standard python imports
+import re
 import os
 import sys
 import zlib
 import time
 import numpy
 import pandas
 import shutil
@@ -1527,14 +1528,62 @@
                     # Add the string with padding to the maximum length
                     formatted_string += strings_list[index].ljust(max_length + 2)
 
             # Add a newline character at the end of each row
             formatted_string += "\n"
 
         return(formatted_string)
+    
+def raw_query(query: str, 
+              con: str, 
+              return_type: str = 'pandas'
+            ) -> pandas.DataFrame | polars.DataFrame:
+
+    query = query.lower()
+
+    # only select statements
+    if(query[0:6] != 'select'):
+        raise ValueError(f'query: this function only works for select statements')
+    
+    # find index of FROM
+    from_idx = re.search(r'\b(from)\b', query).start()
+    
+    # parse query vars
+    query_vars_str = query[7:from_idx].strip()
+
+    connection = sqlite3.connect(con)
+    cursor = connection.cursor()
+
+    if('*' in query_vars_str):
+        cols_cur = cursor.execute(f"""{query} LIMIT 1""")
+        cols = list(map(lambda x: x[0], cols_cur.description))
+        query_vars = [col.lower().strip() for col in cols]
+    else:
+        query_vars = [s.strip() for s in query_vars_str.split(',')]
+
+    # query vars
+    result = cursor.execute(query)
+    data = result.fetchall()
+    connection.close()
+
+    # convert from list of tuples to list of lists
+    data = [list(d) for d in data]
+
+    if(return_type == 'pandas'):
+        df = pandas.DataFrame(data, columns = query_vars)
+    elif(return_type == 'polars'):
+        df = polars.DataFrame(data, schema = query_vars)
+    else:
+        raise ValueError(f'return_type: expected string `pandas` or `polars`, got {return_type}')
+
+    return(df)
+
+
+    
+
```

### Comparing `fintoolsap-1.6.7/src/FinToolsAP/PortfolioSorts.py` & `fintoolsap-1.6.8/src/FinToolsAP/PortfolioSorts.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/src/FinToolsAP/UtilityFunctions.py` & `fintoolsap-1.6.8/src/FinToolsAP/UtilityFunctions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
 # standard imports
+import os
 import tqdm
 import numpy
 import typing
 import polars
 import pandas
+import pathlib
 import functools
+import statsmodels.api
 
 def group_quantile(df: pandas.DataFrame | polars.DataFrame, 
                    gr: typing.Optional[typing.Union[str, list[str]]] = None, 
                    vr: typing.Optional[typing.Union[str, list[str]]] = None, 
                    q: typing.Optional[int] = None,
                    quantiles: typing.Optional[dict[str, typing.Union[int, list[float]]]] = None,
                    interpolation: typing.Optional[str] = 'linear',
@@ -841,10 +844,198 @@
                 df = df.cast({f'{var}_scr{n}': polars.Int64})
             except Exception as e:
                 print(e)
                 raise TypeError(f'one of the keyword arguments is incompatible with polars.qcut or polars.qcut raised the exception above')
         else:
             raise TypeError(f'df: expected type pandas.DataFrame or polars.DataFrame, got {type(df).__name__!r}')
 
-
     return(df)
 
+def lh_regression(endog: typing.Union[list, numpy.ndarray, pandas.Series], 
+                  exog: typing.Union[list, numpy.ndarray, pandas.Series], 
+                  horizon: int, 
+                  se_type: typing.Union[str, list[str]],
+                  add_constant: bool = True
+                ) -> typing.Tuple:
+    
+    """
+    Perform linear regression with a rolling window approach.
+
+    Parameters:
+    - endog (Union[list, numpy.ndarray, pandas.Series]): The dependent variable.
+    - exog (Union[list, numpy.ndarray, pandas.Series]): The independent variable.
+    - horizon (int): The number of periods to roll the window.
+    - se_type (Union[str, list[str]]): Type of standard error(s) to 
+        calculate.
+    - add_constant (bool, optional): Whether to add a constant to 
+        the independent variable. Default is True.
+
+    Returns:
+    Tuple: A tuple containing:
+        - float: The estimated coefficient for the independent variable.
+        - dict: A dictionary containing standard error(s) with their 
+            corresponding type as keys.
+        - float: The R-squared value of the regression.
+        - numpy.ndarray: The residuals of the regression.
+
+    Notes:
+    - If endog or exog is a pandas Series, it will be converted to a 
+        numpy array for processing.
+    - The rolling window approach is implemented by differencing the 
+        dependent variable over the horizon.
+    - Standard error types supported:
+        - 'R': Robust standard errors (HC0).
+        - 'NW': Newey-West standard errors (HAC) with maxlags set to the horizon.
+        - 'HH': Heteroskedasticity and autocorrelation robust standard 
+            errors (HAC) with maxlags set to the horizon and uniform kernel.
+        - Any other string: Assumes the string corresponds to a specific 
+            covariance type.
+    """
+    
+    if(isinstance(endog, pandas.Series)):
+        endog = endog.values
+
+    if(isinstance(endog, pandas.Series)):
+        exog = exog.values
+
+    ### k-horizon difference
+    _Y =(numpy.roll(endog, -horizon) - endog)[:-horizon]
+
+    if(add_constant):
+        _X = statsmodels.api.add_constant(exog[:-horizon])
+
+    _model_fit = statsmodels.api.OLS(_Y, _X).fit()
+
+    ### point estimate
+    _beta = _model_fit.params.iloc[-1]
+    
+    if(isinstance(se_type, str)):
+        se_type = [se_type]
+
+    ### SEs:
+    _ses = {}
+    for _se in se_type:
+        if(_se == 'R'):
+            _ses[_se] = _model_fit.get_robustcov_results(cov_type = 'HC0').bse[-1]
+        elif(_se == 'NW'):
+            _ses[_se] = _model_fit.get_robustcov_results(cov_type = 'HAC', 
+                                                         maxlags = horizon
+                                                        ).bse[-1]
+        elif(_se == 'HH'):
+            _ses[_se] = _model_fit.get_robustcov_results(cov_type = 'HAC', 
+                                                         maxlags = horizon, 
+                                                         kernel = 'uniform'
+                                                        ).bse[-1]
+        else:
+            _ses[_se] = _model_fit.get_robustcov_results(cov_type = _se).bse[-1]
+
+    # R^2
+    _r2 = _model_fit.rsquared
+
+    # Resiudals
+    _resid = _model_fit.resid
+    
+    return(_beta, _ses, _r2, _resid)
+
+def long_horizon_regssions(endog: typing.Union[list, numpy.ndarray, pandas.Series], 
+                           exog: typing.Union[list, numpy.ndarray, pandas.Series], 
+                           se_type: typing.Union[str, list[str]],
+                           horizons: typing.Union[int, list[int]] = 10,
+                           add_constant: bool = True,
+                           return_resid: bool = False
+                        ) -> pandas.DataFrame:
+    
+    """
+    Perform linear regression with a rolling window approach for multiple horizons.
+
+    Parameters:
+    - endog (Union[list, numpy.ndarray, pandas.Series]): The dependent variable.
+    - exog (Union[list, numpy.ndarray, pandas.Series]): The independent variable.
+    - se_type (Union[str, list[str]]): Type of standard error(s) to calculate.
+    - horizons (Union[int, list[int]], optional): The list of horizons or maximum 
+        horizon if integer provided. Default is 10.
+    - add_constant (bool, optional): Whether to add a constant to the independent 
+        variable. Default is True.
+    - return_resid (bool, optional): Whether to return residuals in addition to 
+        regression results. Default is False.
+
+    Returns:
+    pandas.DataFrame: A DataFrame containing regression results for each horizon.
+    
+    If return_resid is True, a tuple containing the DataFrame and a dictionary 
+        of residuals for each horizon is returned.
+    """
+    
+    if(isinstance(horizons, int)):
+        horizons = list(range(1, horizons + 1))
+
+    res = pandas.DataFrame(index = horizons)
+    resids = {}
+    for k in horizons:
+        _b, _ses, _r2, _resid = lh_regression(endog = endog, 
+                                              exog = exog, 
+                                              horizon = k,
+                                              se_type = se_type, 
+                                              add_constant = add_constant
+                                            )
+        res.loc[k, 'b'] = _b
+        for _se, _values in _ses.items():
+            res.loc[k, _se] = _values
+        res.loc[k, 'R2'] = _r2
+        resids[k] = _resid
+
+    if(return_resid):
+        return(res, resids)
+    else:
+        return(res)
+    
+def list_dir(path: typing.Union[str, pathlib.Path],
+             only_dir: bool = False,
+             extension: str = None,
+             only_files: bool = True,
+             keep_hidden: bool = False,
+             absolute_paths: bool = False
+            ) -> list[str]:
+    """
+    List directories and/or files in a given path with optional filtering.
+
+    Parameters:
+    - path (Union[str, pathlib.Path]): The path to list contents from.
+    - only_dir (bool, optional): Whether to list only directories. Default is False.
+    - extension (str, optional): Filter files by extension. Default is None.
+    - only_files (bool, optional): Whether to list only files. Default is True.
+    - keep_hidden (bool, optional): Whether to include hidden files. Default is False.
+    - absolute_paths (bool, optional): Whether to return absolute paths. Default is False.
+
+    Returns:
+    list[str]: A list of directory and/or file names.
+
+    Notes:
+    - If only_dir is True, only directories will be included.
+    - If only_files is True, only files will be included.
+    - If keep_hidden is True, hidden files will be included.
+    - If extension is provided, only files with that extension will be included.
+    - If absolute_paths is True, the full paths of directories and/or files will be returned.
+    """
+    
+    path = pathlib.Path(path)
+    path = path.resolve()
+    _tmp = os.listdir(path)
+
+    res = []
+    for _obj in _tmp:
+        _obj_path = path / _obj
+        if(_obj_path.is_dir() and only_dir):
+            res.append(_obj)
+        elif(_obj_path.is_file() and only_files):
+            if(keep_hidden or not _obj_path.stem.startswith('.')):
+                if(extension is None or _obj_path.suffix == extension):
+                    res.append(_obj)
+    if(absolute_paths):
+        res = [str(path / f) for f in res]
+
+    return(res)
+    
+                
+
+
+
```

### Comparing `fintoolsap-1.6.7/src/FinToolsAP/_config.py` & `fintoolsap-1.6.8/src/FinToolsAP/_config.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/src/FinToolsAP/_download_script.py` & `fintoolsap-1.6.8/src/FinToolsAP/_download_script.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/src/FinToolsAP/_util_funcs.py` & `fintoolsap-1.6.8/src/FinToolsAP/_util_funcs.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/src/FinToolsAP/base_files/DatabaseParameters.py` & `fintoolsap-1.6.8/src/FinToolsAP/base_files/DatabaseParameters.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/src/FinToolsAP/base_files/ExampleCreateTable.py` & `fintoolsap-1.6.8/src/FinToolsAP/base_files/ExampleCreateTable.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/src/FinToolsAP/base_files/ExampleExtraScript.py` & `fintoolsap-1.6.8/src/FinToolsAP/base_files/ExampleExtraScript.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_BMME_sorts.py` & `fintoolsap-1.6.8/tests/TEST_BMME_sorts.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_FF_factors.py` & `fintoolsap-1.6.8/tests/TEST_FF_factors.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_breakpoint_construction.py` & `fintoolsap-1.6.8/tests/TEST_breakpoint_construction.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_create_all_factors.py` & `fintoolsap-1.6.8/tests/TEST_create_all_factors.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_csv_import.py` & `fintoolsap-1.6.8/tests/TEST_csv_import.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_csv_to_sql.py` & `fintoolsap-1.6.8/tests/TEST_csv_to_sql.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_martin_output.py` & `fintoolsap-1.6.8/tests/TEST_martin_output.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_query_BTDS.py` & `fintoolsap-1.6.8/tests/TEST_query_BTDS.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_query_Bank.py` & `fintoolsap-1.6.8/tests/TEST_query_Bank.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_query_CRSP.py` & `fintoolsap-1.6.8/tests/TEST_query_CRSP.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_query_CRSPMF.py` & `fintoolsap-1.6.8/tests/TEST_query_CRSPMF.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_query_Factors.py` & `fintoolsap-1.6.8/tests/TEST_query_Factors.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_query_IBES.py` & `fintoolsap-1.6.8/tests/TEST_query_IBES.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_query_IH.py` & `fintoolsap-1.6.8/tests/TEST_query_IH.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_query_MF.py` & `fintoolsap-1.6.8/tests/TEST_query_MF.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_query_MFCH.py` & `fintoolsap-1.6.8/tests/TEST_query_MFCH.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_query_MFHoldings.py` & `fintoolsap-1.6.8/tests/TEST_query_MFHoldings.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_query_MFLinks.py` & `fintoolsap-1.6.8/tests/TEST_query_MFLinks.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_score_characteristics.py` & `fintoolsap-1.6.8/tests/TEST_score_characteristics.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_sorting.py` & `fintoolsap-1.6.8/tests/TEST_sorting.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_univariate_sorts.py` & `fintoolsap-1.6.8/tests/TEST_univariate_sorts.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/TEST_virtual_environment.py` & `fintoolsap-1.6.8/tests/TEST_virtual_environment.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/tests/test.py` & `fintoolsap-1.6.8/tests/test.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/LICENSE` & `fintoolsap-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/README.md` & `fintoolsap-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.6.7/pyproject.toml` & `fintoolsap-1.6.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "FinToolsAP"
-version = "1.6.7"
+version = "1.6.8"
 authors = [
   { name="Andrew Maurice Perry", email="andrewpe@berkeley.edu" },
 ]
 description = "Package that includes many tools commonly used in finance. Also includes a local database."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `fintoolsap-1.6.7/PKG-INFO` & `fintoolsap-1.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: FinToolsAP
-Version: 1.6.7
+Version: 1.6.8
 Summary: Package that includes many tools commonly used in finance. Also includes a local database.
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Andrew Maurice Perry <andrewpe@berkeley.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

