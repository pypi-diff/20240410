# Comparing `tmp/JayttleProcess-0.1.4-py3-none-any.whl.zip` & `tmp/JayttleProcess-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,12 @@
-Zip file size: 21967 bytes, number of entries: 7
+Zip file size: 35315 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat     2441 b- defN 24-Apr-10 05:07 JayttleProcess/CommonDecorator.py
 -rw-rw-rw-  2.0 fat     4727 b- defN 24-Mar-19 06:31 JayttleProcess/ComputerControl.py
--rw-rw-rw-  2.0 fat    85880 b- defN 24-Mar-26 14:44 JayttleProcess/TimeSeriesDataMethod.py
+-rw-rw-rw-  2.0 fat      613 b- defN 24-Apr-08 05:57 JayttleProcess/EntertainmentCode.py
+-rw-rw-rw-  2.0 fat    16303 b- defN 24-Apr-10 06:43 JayttleProcess/SQLCommonUse.py
+-rw-rw-rw-  2.0 fat   117579 b- defN 24-Apr-08 05:24 JayttleProcess/TimeSeriesDataMethod.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-14 14:39 JayttleProcess/__init__.py
--rw-rw-rw-  2.0 fat      436 b- defN 24-Mar-26 14:44 JayttleProcess-0.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-26 14:44 JayttleProcess-0.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-Mar-26 14:44 JayttleProcess-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      591 b- defN 24-Mar-26 14:44 JayttleProcess-0.1.4.dist-info/RECORD
-7 files, 91741 bytes uncompressed, 20907 bytes compressed:  77.2%
+-rw-rw-rw-  2.0 fat      631 b- defN 24-Apr-10 06:46 JayttleProcess-0.1.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-10 06:46 JayttleProcess-0.1.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-10 06:46 JayttleProcess-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      861 b- defN 24-Apr-10 06:46 JayttleProcess-0.1.5.dist-info/RECORD
+10 files, 143262 bytes uncompressed, 33831 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -1,22 +1,31 @@
+Filename: JayttleProcess/CommonDecorator.py
+Comment: 
+
 Filename: JayttleProcess/ComputerControl.py
 Comment: 
 
+Filename: JayttleProcess/EntertainmentCode.py
+Comment: 
+
+Filename: JayttleProcess/SQLCommonUse.py
+Comment: 
+
 Filename: JayttleProcess/TimeSeriesDataMethod.py
 Comment: 
 
 Filename: JayttleProcess/__init__.py
 Comment: 
 
-Filename: JayttleProcess-0.1.4.dist-info/METADATA
+Filename: JayttleProcess-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: JayttleProcess-0.1.4.dist-info/WHEEL
+Filename: JayttleProcess-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: JayttleProcess-0.1.4.dist-info/top_level.txt
+Filename: JayttleProcess-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: JayttleProcess-0.1.4.dist-info/RECORD
+Filename: JayttleProcess-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## JayttleProcess/TimeSeriesDataMethod.py

```diff
@@ -5,46 +5,70 @@
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
 import statsmodels.api as sm
 from statsmodels.tsa.arima.model import ARIMA
 from statsmodels.tsa.ar_model import AutoReg
 from statsmodels.stats.diagnostic import acorr_ljungbox
 import pandas as pd
-from sklearn.cluster import KMeans,DBSCAN
-from sklearn.linear_model import Ridge ,Lasso, LassoCV,ElasticNet
-from sklearn.metrics import root_mean_squared_error, mean_absolute_error,r2_score,mean_squared_error
+from sklearn.cluster import KMeans, DBSCAN, AgglomerativeClustering 
+from sklearn.linear_model import Ridge , Lasso, LassoCV, ElasticNet, LinearRegression
+from sklearn.metrics import root_mean_squared_error, mean_absolute_error, r2_score, mean_squared_error, silhouette_score, davies_bouldin_score, calinski_harabasz_score, silhouette_score, v_measure_score
 from scipy.spatial.distance import euclidean
-from sklearn.preprocessing import PolynomialFeatures
+from sklearn.preprocessing import PolynomialFeatures, StandardScaler
 from sklearn.pipeline import make_pipeline
+from sklearn.mixture import GaussianMixture
+from sklearn.model_selection import GridSearchCV
 from scipy import signal,fft
-from scipy.stats import t,shapiro,pearsonr,f_oneway
-from scipy.signal import hilbert,find_peaks
+from scipy.cluster import hierarchy
+from scipy.stats import t, shapiro, pearsonr, f_oneway, gaussian_kde
+from scipy.signal import hilbert, find_peaks
 from PyEMD import EMD,EEMD, CEEMDAN
-from typing import List, Optional
+from typing import List, Optional, Tuple, Union
 import pywt
 import warnings
-
+import time
+"""
+python:
+O(n)算法: 输入n: 1,000,000 耗时: 15.312433242797852 ms
+O(n^2)算法输入n: 10,000 耗时: 1610.5492115020752 ms
+O(nlogn)算法输入n: 10,000 耗时: 5.4988861083984375 ms 
+"""
 # region 字体设置
 plt.rcParams['font.sans-serif'] = ['SimSun']  # 指定宋体为默认字体
 plt.rcParams['font.sans-serif'] = 'SimSun'  # 使用指定的中文字体
 # 禁用特定警告
 warnings.filterwarnings('ignore', category=UserWarning, append=True)
-# 或者设置为指定分辨率（2560x1440）
-plt.figure(figsize=(25.6, 14.4))  # 单位是英寸
+# 或者关闭所有警告
+warnings.filterwarnings("ignore")
 # endregion
 class TimeSeriesData:
-    def __init__(self, value, datetime):
+    def __init__(self, value, date_time_str):
         self.value = value
-        self.datetime = datetime
+        self.datetime = datetime.strptime(date_time_str, "%Y-%m-%d %H:%M:%S")
 
     def __str__(self):
         return f"Value: {self.value}, Datetime: {self.datetime}"
+
+# region 无关功能
+def show_prcoess_time(start_time: float, addTxt: Optional[str] = None) -> None:
+    end_time: float = time.time()  # 记录程序结束时间
+    runtime: float = end_time - start_time  # 计算程序运行时间
+    if addTxt is not None:
+        print(f"{addTxt}运行时间:{runtime:.2f} 秒")
+    else:
+        print(f"程序运行时间:{runtime:.2f} 秒")
+
+def check_data_type(data: np.ndarray) ->None:
+    print("数据类型:", type(data))
+    print("形状:", data.shape)
+
+# endregion
 # region 基础功能
 def load_csv_data(data_file = "D:\python_proj\Data_dynamics\data_month_1.txt"):
-    num_data_to_read = 10000
+    num_data_to_read = 100000
     time_series_data = []
     count = 0
 
     with open(data_file, 'r') as file:
         for line in file:
             line_data = line.strip().split('\t')
             value = float(line_data[1])
@@ -174,40 +198,31 @@
     for i in range(1, len(time_series_data)):
         current_value = time_series_data[i].value
         previous_value = time_series_data[i-1].value
         change_rate = (current_value - previous_value) / previous_value
         change_rates.append(change_rate)
     return change_rates
 
-def get_x_values(data: List) -> List[int]:
+def get_x_values(data: List[TimeSeriesData]) -> List[int]:
     """获取时间步作为x值"""
     # 获取时间步作为x值
     x = []
     for i in range(len(data)):
         x.append(i)
     return x
 
-def get_y_values(data: List) -> List[float]:
+def get_y_values(data: List[TimeSeriesData]) -> List[float]:
     """获取数值作为y值"""
-    # 获取数值作为y值
-    y = []
-    for i in range(len(data)):
-        y.append(data[i].value)
+    # 使用列表推导式获取数值作为y值
+    y = [entry.value for entry in data]
     return y
 
-def fit_polynomial_trend(data: List, degree: int = 3) -> np.ndarray:
-    """拟合多项式趋势线"""
-    # 拟合多项式趋势线
-    x = get_x_values(data)
-    y = get_y_values(data)
-    coefficients = np.polyfit(x, y, degree)
-    trend_line = np.polyval(coefficients, x)
-    return trend_line
 
-def calculate_trend_line_residuals(data: List, trend_line: np.ndarray) -> np.ndarray:
+
+def calculate_trend_line_residuals(data: List[TimeSeriesData], trend_line: np.ndarray) -> np.ndarray:
     """计算残差"""
     y = get_y_values(data)
     residuals = np.array(y) - trend_line
     return residuals
 
 def plot_residuals(residuals: np.ndarray, SaveFilePath: Optional[str] = None) -> None:
     """绘制残差图"""
@@ -233,14 +248,24 @@
     return r_squared
 
 def calculate_durbin_watson(residuals: np.ndarray) -> float:
     """手动计算德宾沃森统计量"""
     diff_residuals = np.diff(residuals)  # 计算残差的差分
     durbin_watson_statistic = np.sum(diff_residuals ** 2) / np.sum(residuals ** 2)
     return durbin_watson_statistic
+# endregion
+# region 拟合多项式趋势线
+def fit_polynomial_trend(data: List, degree: int = 3) -> np.ndarray:
+    """拟合多项式趋势线"""
+    # 拟合多项式趋势线
+    x = get_x_values(data)
+    y = get_y_values(data)
+    coefficients = np.polyfit(x, y, degree)
+    trend_line = np.polyval(coefficients, x)
+    return trend_line
 
 def calculate_trend_line_r_squared(data: List, trend_line: np.ndarray) -> float:
     """计算趋势线拟合度"""
     y = get_y_values(data)
     y_mean = np.mean(y)
     
     # 计算总平方和 TSS
@@ -305,15 +330,15 @@
     """找到 Ridge 回归模型最佳的阶数"""
     x = get_x_values(data)
     y = get_y_values(data)
     x = np.array(x)
     y = np.array(y)
 
     best_degree = None
-    best_r_squared = -1  # 初始化为负数，确保能够更新
+    best_r_squared = -1  # 初始化为负数,确保能够更新
     best_mae = float('inf')  # 初始化为正无穷
     best_mape = float('inf')  # 初始化为正无穷
     best_bic = float('inf')  # 初始化为正无穷
 
     for degree in range(1, 21):  # 假设循环从1到21的范围
         # 创建 Polynomial 特征转换器
         polynomial_features = PolynomialFeatures(degree=degree)
@@ -332,14 +357,17 @@
         # 计算矫正决定系数
         n = len(y)
         adjusted_r_squared = 1 - (1 - r_squared) * (n - 1) / (n - degree - 1)
 
         # 计算误差平方和 SSE
         sse = np.sum((y - y_pred) ** 2)
 
+         # 计算均方误差 MSE
+        mse = mean_squared_error(y, y_pred)
+
         # 计算平均绝对误差 MAE
         mae = mean_absolute_error(y, y_pred)
 
         # 计算平均绝对百分比误差 MAPE
         mape = np.mean(np.abs((y - y_pred) / y)) * 100
 
         # 计算模型参数数量
@@ -347,15 +375,15 @@
         
         # 计算 AIC 值
         aic = 2 * num_params - 2 * np.log(np.sum((y - y_pred) ** 2))
 
         # 计算 BIC 值
         bic = n * np.log(sse / n) + num_params * np.log(n)
 
-        print(f"Degree {degree}: R方值 = {r_squared}, 矫正R方值 = {adjusted_r_squared}, SSE = {sse}, MAE = {mae}, MAPE = {mape}, AIC = {aic}, BIC = {bic}")
+        print(f"Degree {degree}: R方值 = {r_squared}, 矫正R方值 = {adjusted_r_squared}, SSE = {sse},  MSE = {mse},MAE = {mae}, MAPE = {mape}, AIC = {aic}, BIC = {bic}")
 
         if r_squared > best_r_squared:
             best_r_squared = r_squared
             best_degree = degree
 
         if mae < best_mae:
             best_mae = mae
@@ -373,15 +401,15 @@
     """找到 Lasso 回归模型最佳的阶数"""
     x = get_x_values(data)
     y = get_y_values(data)
     x=np.array(x)
     y=np.array(y)
 
     best_degree = None
-    best_r_squared = -1  # 初始化为负数，确保能够更新
+    best_r_squared = -1  # 初始化为负数,确保能够更新
 
     for degree in range(1, 21):  # 假设循环从1到21的范围
         # 创建 Polynomial 特征转换器
         polynomial_features = PolynomialFeatures(degree=degree)
         X_poly = polynomial_features.fit_transform(x.reshape(-1, 1))
 
         # 创建 Lasso 回归模型
@@ -520,15 +548,15 @@
         if BIC < best_BIC:
             best_BIC = BIC
             best_degree = degree
 
     print(f"最佳Degree: {best_degree}, 对应的最佳BIC值: {best_BIC}")
     return best_degree, best_BIC
 
-def fit_Ridge_polynomial_trend(data, degree=13, alpha=1.0):
+def fit_Ridge_polynomial_trend(data: List[TimeSeriesData], degree: int=11, alpha: float=1.0) -> np.ndarray:
     """使用岭回归拟合多项式趋势线"""
     x = np.array(get_x_values(data))
     y = np.array([point.value for point in data])
 
     # 创建 Polynomial 特征转换器
     polynomial_features = PolynomialFeatures(degree=degree)
     X_poly = polynomial_features.fit_transform(x.reshape(-1, 1))
@@ -538,15 +566,15 @@
     ridge.fit(X_poly, y)
 
     # 预测拟合结果
     y_pred = ridge.predict(X_poly)
 
     return y_pred
 
-def fit_Lasso_polynomial_trend(data, degree=13, alpha=1.0):
+def fit_Lasso_polynomial_trend(data: List[TimeSeriesData], degree: int=11, alpha: float=1.0) -> np.ndarray:
     """使用Lasso回归拟合多项式趋势线"""
     x = np.array(get_x_values(data))
     y = np.array([point.value for point in data])
 
     # 创建 Polynomial 特征转换器
     polynomial_features = PolynomialFeatures(degree=degree)
     X_poly = polynomial_features.fit_transform(x.reshape(-1, 1))
@@ -556,15 +584,15 @@
     lasso.fit(X_poly, y)
 
     # 预测拟合结果
     y_pred = lasso.predict(X_poly)
 
     return y_pred
 
-def fit_ElasticNet_polynomial_trend(data, degree=13, alpha=1.0, l1_ratio=0.5):
+def fit_ElasticNet_polynomial_trend(data: List[TimeSeriesData], degree: int=11, alpha: float=1.0, l1_ratio: float=0.5) -> np.ndarray:
     """使用弹性网络回归拟合多项式趋势线"""
     x = np.array(get_x_values(data))
     y = np.array([point.value for point in data])
 
     # 创建 Polynomial 特征转换器
     polynomial_features = PolynomialFeatures(degree=degree)
     X_poly = polynomial_features.fit_transform(x.reshape(-1, 1))
@@ -663,15 +691,15 @@
     elif min_bic == bic_lasso:
         print("Lasso回归模型的拟合效果最好 (最小BIC)")
     elif min_bic == bic_elastic:
         print("ElasticNet回归模型的拟合效果最好 (最小BIC)")
     else:
         print("多项式回归模型的拟合效果最好 (最小BIC)")
 
-def plot_polynomial_trend(data, y_pred, SaveFilePath=None):
+def plot_polynomial_trend(data: List[TimeSeriesData], y_pred: Union[List[float], np.ndarray], SaveFilePath: Optional[str] = None):
     """绘制多项式趋势线"""
     # 提取日期时间和数值信息
     datetimes = [point.datetime for point in data]
     values = [point.value for point in data]
 
     # 修改标签和标题的文本为中文
     plt.figure(figsize=(25.6, 14.4))  # 设置图形大小
@@ -745,14 +773,304 @@
         ('elastic', 'polynomial'): pearsonr(elastic_pred, polynomial_pred)[0]
     }
 
     # 计算ANOVA
     f_statistic, p_value = f_oneway(ridge_pred, lasso_pred, elastic_pred, polynomial_pred)
 
     return euclidean_distances, pearson_correlations, f_statistic, p_value
+
+def find_Ridge_best_degree_without_print(data:List[TimeSeriesData]) -> int:
+    """找到 Ridge 回归模型最佳的阶数"""
+    x = get_x_values(data)
+    y = get_y_values(data)
+    x = np.array(x)
+    y = np.array(y)
+
+    best_degree = None
+    best_bic = float('inf')  # 初始化为正无穷
+
+    for degree in range(1, 16):  # 假设循环从1到21的范围
+        # 创建 Polynomial 特征转换器
+        polynomial_features = PolynomialFeatures(degree=degree)
+        X_poly = polynomial_features.fit_transform(x.reshape(-1, 1))
+
+        # 创建 Ridge 回归模型
+        ridge = Ridge()
+        ridge.fit(X_poly, y)
+
+        # 计算预测值
+        y_pred = ridge.predict(X_poly)
+
+        # 计算矫正决定系数
+        n = len(y)
+
+        # 计算误差平方和 SSE
+        sse = np.sum((y - y_pred) ** 2)
+
+        # 计算模型参数数量
+        num_params = X_poly.shape[1]
+        
+        # 计算 AIC 值
+
+        # 计算 BIC 值
+        bic = n * np.log(sse / n) + num_params * np.log(n)
+
+        
+        # 更新最佳degree和对应的评价指标
+        if bic < best_bic:
+            best_degree = degree
+            best_bic = bic
+
+    return best_degree
+
+
+def calculate_acceleration(data: List[TimeSeriesData]) -> List[float]:
+    """
+    计算加速度序列
+    时间复杂度为 ( O(n) )
+    """
+    accelerations = []
+    for i in range(1, len(data) - 1):
+        dt1 = (data[i].datetime - data[i-1].datetime).total_seconds()
+        dt2 = (data[i+1].datetime - data[i].datetime).total_seconds()
+        dv1 = data[i].value - data[i-1].value
+        dv2 = data[i+1].value - data[i].value
+        acceleration = (dv2/dt2 - dv1/dt1) / ((dt1 + dt2) / 2)
+        accelerations.append(acceleration)
+    return accelerations
+
+def calculate_acceleration_for_cycles(data: List[TimeSeriesData]) -> List[List[float]]:
+    """
+    计算每个“圈”的加速度序列。
+    时间复杂度为 ( O(n) ),其中 n 是数据点的数量。
+    """
+    # 提取值序列
+    values = np.array([point.value for point in data])
+
+    # 寻找峰值
+    peaks, _ = find_peaks(values)
+
+    # 如果没有找到足够的峰值,则返回空列表
+    if len(peaks) < 2:
+        return []
+
+    # 计算每个圈的加速度
+    cycle_accelerations = []
+    for i in range(len(peaks) - 1):
+        cycle_data = data[peaks[i]:peaks[i + 1] + 1]
+        accelerations = calculate_acceleration(cycle_data)
+        cycle_accelerations.append(accelerations)
+
+    return cycle_accelerations
+def plot_acceleration(data: List[TimeSeriesData], accelerations: List[float], SaveFilePath: Optional[str]=None) -> None:
+    timestamps = [data[i].datetime for i in range(1, len(data) - 1)]
+    
+    plt.figure(figsize=(10, 5))
+    plt.plot(timestamps, accelerations, color='blue', marker='.', linestyle='-')  # 将 marker 参数设置为更小的点
+    plt.title('加速度随时间变化图')
+    plt.xlabel('时间戳')
+    plt.ylabel('加速度')
+    plt.xticks(rotation=45)
+    plt.grid(True)
+    plt.tight_layout()
+    if SaveFilePath is not None:
+        plt.savefig(SaveFilePath) 
+    else:
+        plt.show()
+        
+    plt.close()
+
+def adaptive_polynomial_fitting(data: List[TimeSeriesData], initial_threshold: float) -> np.ndarray:
+    """
+    自适应拟合趋势线
+    外层循环:外层循环 while n < N - 1: 的执行次数取决于数据的长度 N。假设数据长度为 N,那么外层循环的执行次数为 N 次,时间复杂度为 O(N)。
+    内层循环:内层循环 while n + r < N - 1:在最坏情况下,内层循环的执行次数可能会达到 O(N)。
+    拟合趋势线和计算相关系数:假设这两个步骤的时间复杂度为 O(M),其中 M 是数据的长度和拟合多项式的阶数中较大的一个。
+    总的时间复杂度可以近似为 O(N^2 * M),其中 N 是数据的长度,M 是拟合多项式的阶数。
+    """
+    N = len(data)
+    trend_lines = []  # 存储所有拟合的趋势线
+    accelerations = calculate_acceleration(data)  # 预先计算所有加速度值
+
+    n = 0
+    original_threshold = initial_threshold  # 保存原始阈值
+
+    while n < N - 1:
+        r = 1
+        while n + r < N - 1:
+            segment_accelerations = accelerations[n:n+r]
+            Δa = max(segment_accelerations) - min(segment_accelerations)
+            if Δa > initial_threshold:
+                break
+            r += 1
+        segment_data = data[n:n+r]
+        # 拟合多项式趋势线并计算相关系数
+        best_degree = find_Ridge_best_degree_without_print(segment_data)
+        trend_line = fit_Ridge_polynomial_trend(segment_data, best_degree)
+        correlation = np.corrcoef(np.array([point.value for point in segment_data]), trend_line)[0, 1]
+        
+        # 检查相关系数是否满足条件
+        if correlation < 0.8:
+            initial_threshold *= 0.9  # 调整阈值
+            continue
+        
+        # 将当前窗口的拟合趋势线添加到列表中
+        trend_lines.append(trend_line)  
+
+        # 更新索引并重置r
+        n += r
+        r = 1
+        
+        # 恢复原始阈值
+        initial_threshold = original_threshold
+
+    # 将所有拟合的趋势线连接起来,得到完整的趋势线
+    complete_trend_line = np.concatenate(trend_lines)
+    print(f"complete_trend_line: {len(complete_trend_line)}")  
+    return complete_trend_line
+
+def split_time_series_data(data: List[TimeSeriesData], break_points: List[int]) -> List[List[TimeSeriesData]]:
+    """根据隔断点将时序数据分割成不同的分组"""
+    groups = []
+    start_index = 0
+
+    for break_point in break_points:
+        group = data[start_index:break_point]
+        groups.append(group)
+        start_index = break_point
+
+    # 添加最后一个分组
+    groups.append(data[start_index:])
+
+    return groups
+
+def fit_and_concatenate_trend_lines(segmented_data: List[List[TimeSeriesData]]) -> np.ndarray:
+    """拟合多项式趋势线并将所有拟合的趋势线连接起来"""
+    trend_lines = []
+
+    for segment_data in segmented_data:
+        # 拟合多项式趋势线并计算相关系数
+        best_degree = find_Ridge_best_degree_without_print(segment_data)
+        trend_line = fit_Ridge_polynomial_trend(segment_data, best_degree)
+        trend_lines.append(trend_line)
+
+    complete_trend_line = np.concatenate(trend_lines)
+    return complete_trend_line
+
+def adaptive_polynomial_fitting_in_std(data: List[TimeSeriesData]) -> np.ndarray:
+    values = [entry.value for entry in data]
+    std_value = np.std(values)
+    original_threshold = std_value / 2.0
+
+    initial_threshold = original_threshold
+    trend_lines = []  # 存储所有拟合的趋势线
+    n, N= 0, len(data)
+    while n < N - 1:
+        r = 1
+        while n + r < N - 1:
+            segment_data = data[n:n+r]
+            values = [entry.value for entry in segment_data]
+            std_value = np.std(values)
+            # print(f"{std_value}\t{initial_threshold} n: {n} r: {r} ")
+            if std_value > initial_threshold:
+                break
+            r += 1
+        # 拟合多项式趋势线并计算相关系数
+        best_degree = find_Ridge_best_degree_without_print(segment_data)
+        trend_line = fit_Ridge_polynomial_trend(segment_data, best_degree)
+        correlation = np.corrcoef(np.array([point.value for point in segment_data]), trend_line)[0, 1]
+        # print(f"tl: {len(trend_line)}, sgd: {len(segment_data)} n: {n} r: {r} correlation: {correlation}")
+
+        # 检查相关系数是否满足条件
+        if correlation < 0.8:
+            initial_threshold *= 0.9  # 调整阈值
+            continue
+        
+        # 将当前窗口的拟合趋势线添加到列表中
+        trend_lines.append(trend_line)  
+        
+        # 更新索引并重置r
+        n += r
+        r = 1
+        
+        # 恢复原始阈值
+        initial_threshold = original_threshold
+        # 将所有拟合的趋势线连接起来,得到完整的趋势线
+
+    complete_trend_line = np.concatenate(trend_lines)
+    # print(f"complete_trend_line: {len(complete_trend_line)}")  
+    return complete_trend_line
+
+
+def adaptive_polynomial_fitting_in_cusum(data: List[TimeSeriesData]) -> np.ndarray:
+    """
+    基于cusum值自适应拟合趋势线
+    """
+    cusum_values = cusum(data, 1)
+    original_threshold = determine_threshold(cusum_values)   
+    initial_threshold = original_threshold
+    trend_lines = []  # 存储所有拟合的趋势线
+    n, N= 0, len(data)
+    while n < N - 1:
+        r = 1
+        while n + r < N - 1:
+            segment_data = data[n:n+r]
+            cusum_total_value = cusum_total(segment_data)
+            print(f"{cusum_total_value}\t{initial_threshold} n: {n} r: {r} ")
+            if cusum_total_value > initial_threshold:
+                break
+            r += 1
+        # 拟合多项式趋势线并计算相关系数
+        best_degree = find_Ridge_best_degree_without_print(segment_data)
+        trend_line = fit_Ridge_polynomial_trend(segment_data, best_degree)
+        correlation = np.corrcoef(np.array([point.value for point in segment_data]), trend_line)[0, 1]
+        print(f"tl: {len(trend_line)}, sgd: {len(segment_data)} n: {n} r: {r} correlation: {correlation}")
+
+        # 检查相关系数是否满足条件
+        if correlation < 0.8:
+            initial_threshold *= 0.9  # 调整阈值
+            continue
+        
+        # 将当前窗口的拟合趋势线添加到列表中
+        trend_lines.append(trend_line)  
+        
+        # 更新索引并重置r
+        n += r
+        r = 1
+        
+        # 恢复原始阈值
+        initial_threshold = original_threshold
+        # 将所有拟合的趋势线连接起来,得到完整的趋势线
+
+    complete_trend_line = np.concatenate(trend_lines)
+    # print(f"complete_trend_line: {len(complete_trend_line)}")  
+    return complete_trend_line
+
+def calculate_cusum(time_series: List[TimeSeriesData], target: float) -> Tuple[List[float], List[float]]:
+    """
+    """
+    cusum_pos = [0]  # Positive CUSUM values
+    cusum_neg = [0]  # Negative CUSUM values
+    for data in time_series[1:]:  # Skipping the first element as we've initialized with it
+        deviation = data.value - target
+        cusum_pos.append(max(0, cusum_pos[-1] + deviation))
+        cusum_neg.append(min(0, cusum_neg[-1] + deviation))
+    return cusum_pos, cusum_neg
+
+def plot_cusum_pos_and_neg(cusum_pos: List[float], cusum_neg: List[float]) -> None:
+    # 绘图
+    plt.figure(figsize=(12, 6))
+    plt.plot(cusum_pos, label='CUSUM正向', color='blue')
+    plt.plot(cusum_neg, label='CUSUM负向', color='red')
+    plt.axhline(y=0, color='k', linestyle='--')  # 目标线
+    plt.xlabel('观测数目')
+    plt.ylabel('CUSUM值')
+    plt.title('CUSUM控制图')
+    plt.legend()
+    plt.show()
 # endregion
 # region 频域分析
 def fourier_transform(TimeSeriesData):
     """对TimeSeriesData对象进行傅里叶变换"""
     values = [data.value for data in TimeSeriesData]
     transformed_values = np.fft.fft(values)
     return transformed_values
@@ -1316,29 +1634,67 @@
         current_statistic = abs(cumulative_sum[i] - cumulative_sum[n-i-1])
         if current_statistic > max_test_statistic:
             max_test_statistic = current_statistic
             change_point = i
 
     return change_point, max_test_statistic
 
-def cusum(data, threshold=1):
+def cusum(data: List[TimeSeriesData], threshold: float=1) -> List[float]:
     """
     计算CUSUM
-    # 设置阈值,根据具体情况调整
+    设置阈值,根据具体情况调整
     """
     # 计算CUSUM
     cusum_values = [0]  # 起始值为0
    
     for i in range(1, len(data)):
         diff = data[i].value - data[i-1].value
         cusum_values.append(max(0, cusum_values[i-1] + diff - threshold))
     
     return cusum_values
 
-def plot_cusum(data,cusum_values, SaveFilePath=None):
+
+def cusum_total(data: List[TimeSeriesData], threshold: float=1) -> float:
+    """
+    计算整段数据的CUSUM值
+    """
+    cusum_value = 0  # 初始CUSUM值为0
+
+    for i in range(1, len(data)):
+        diff = data[i].value - data[i-1].value
+        cusum_value = max(0, cusum_value + diff - threshold)
+    
+    return cusum_value
+
+def save_list_to_txt(data: List[float], filename: str):
+    with open(filename, 'w') as file:
+        for item in data:
+            file.write(str(item) + '\n')
+
+def cusum_z_transform(data: List[TimeSeriesData], threshold: float=1) -> List[float]:
+    """
+    计算CUSUM
+    # 设置阈值,根据具体情况调整
+    """
+    # 计算CUSUM
+    cusum_values = [0]  # 起始值为0
+
+    for i in range(1, len(data)):
+        diff = data[i].value - data[i-1].value
+        cusum_values.append(max(0, cusum_values[i-1] + diff - threshold))
+
+    # 对CUSUM序列进行Z变换
+    cusum_array = np.array(cusum_values)
+    cusum_mean = np.mean(cusum_array)
+    cusum_std = np.std(cusum_array)
+    z_transformed = (cusum_array - cusum_mean) / cusum_std
+
+    return z_transformed
+
+def plot_cusum(data: List[TimeSeriesData], cusum_values: List[float], SaveFilePath: Optional[str] = None) -> None:
     """绘制CUSUM"""
     # 绘制CUSUM
     x = np.arange(len(data))
     y = get_y_values(data)
     plt.figure(figsize=(25.6, 14.4))  # 单位是英寸
     plt.plot(x, y, label='时序数据')
     plt.plot(x, cusum_values, label='CUSUM')
@@ -1348,38 +1704,55 @@
     plt.title('时序数据的CUSUM')
     if SaveFilePath is not None:
         plt.savefig(SaveFilePath)
     else: 
         plt.show()
     plt.close()
 
+def plot_cusum_in_threshold(cusum: List[float], threshold: float, SaveFilePath: Optional[str] = None) -> None:
+    plt.plot(cusum)
+    plt.axhline(threshold, color='red', linestyle='--')  # Add horizontal line at the threshold
+    plt.xlabel('时间点')
+    plt.ylabel('CUSUM')
+    plt.title('CUSUM控制图')
+    if SaveFilePath is not None:
+        plt.savefig(SaveFilePath)
+    else: 
+        plt.show()
+    plt.close()
+
+def determine_threshold(cusum: List[float]) -> float:
+    std = np.std(cusum)
+    threshold = 3 * std  # Adjust the multiplier as needed
+    return threshold
+
 def detect_cusum_threshold(cusum_values, threshold):
     """
     对cusum_values设置阈值,并将超过阈值的值作为变化点
     """
     change_points = []
     for i, value in enumerate(cusum_values):
         if value > threshold:
             change_points.append(i)
     
     return change_points
 
-def detect_cusum_diff_threshold(cusum_values, threshold):
+def detect_cusum_diff_threshold(cusum_values: List[float], threshold: float) -> List[int]:
     """
-    计算相邻CUSUM值的差异diff，如果差异超过了设定的阈值threshold
+    计算相邻CUSUM值的差异diff,如果差异超过了设定的阈值threshold
     """
     change_points = []
   
     for i in range(1, len(cusum_values)):
         diff = cusum_values[i] - cusum_values[i-1]
         if diff > threshold:
             change_points.append(i)
     
     return change_points
-def detect_cusum_window(cusum_values, threshold, window_size):
+def detect_cusum_window(cusum_values: List[float], threshold: float, window_size: int) -> List[int]:
     """
     滑动窗口来检测连续的CUSUM值
     使用启发式规则:一些经验法则建议窗口大小选择为数据点总数的一定比例,例如窗口大小为数据总点数的1/10或1/20。
     统计方法:可以根据数据的统计特征来选择阈值。例如,基于数据的标准差、平均值等来设置阈值,使得超过阈值的CUSUM值被认为是结构性变化点。
     可视化和交互:可以通过可视化CUSUM图形,并与领域专家或数据分析人员进行交互来优化阈值的选择。观察图形中的结构性变化,根据专家意见或实际需求来调整阈值。
     """
     change_points = []
@@ -1388,41 +1761,73 @@
         sub_cusum = cusum_values[i-window_size:i+1]
 
         if all(value >= threshold for value in sub_cusum):
             change_points.append(i)
     
     return change_points
 
-def calculate_rolling_std(data, window_size):
+def calculate_rolling_std(data: List[TimeSeriesData], window_size: int) -> List[float]:
     """滚动标准差来检测波动性的变动"""
     values = [item.value for item in data]  # 提取时序数据中的值
     rolling_std = np.std(values[:window_size])  # 初始窗口的标准差
     std_values = [rolling_std]
 
     for i in range(window_size, len(values)):
         window_values = values[i-window_size+1:i+1]
         rolling_std = np.std(window_values)
         std_values.append(rolling_std)
     
     return std_values
-def plot_std_values(std_values, SaveFilePath=None):
+
+
+def calculate_cumulative_std(data: List[TimeSeriesData]) -> List[float]:
+    """计算每个点到data[0:n]的标准差"""
+    values = [item.value for item in data]  # 提取时序数据中的值
+    std_values = []
+
+    for i in range(1, len(values) + 1):
+        std_values.append(np.std(values[:i]))
+
+    return std_values
+
+def plot_std_values(std_values: List[float], SaveFilePath: Optional[str] = None) -> None:
     x = range(len(std_values))  # x轴为数据点的索引
     y = std_values  # y轴为滚动标准差的值
     plt.figure(figsize=(25.6, 14.4))  # 单位是英寸
     plt.plot(x, y)
     plt.xlabel('数据点')  # x轴标签
     plt.ylabel('标准差')  # y轴标签
     plt.title('滚动标准差')  # 图表标题
     if SaveFilePath is not None:
         plt.savefig(SaveFilePath)
     else: 
         plt.show()
     plt.close()
 
-def apply_grubbs_test(data, alpha=0.05):
+
+def calculate_cumulative_std_with_break(data: List[TimeSeriesData], threshold: float = 1.5) -> Tuple[List[float], List[int]]:
+    """计算每个点到data[0:n]的标准差，如果超过阈值则隔断，并记录隔断点的索引位置"""
+    values = [item.value for item in data]  # 提取时序数据中的值
+    std_values = []
+    break_points = []  # 记录隔断点的索引位置
+    start_index = 0  # 开始计算的索引
+
+    for i in range(1, len(values) + 1):
+        current_std = np.std(values[start_index:i])
+        if current_std > threshold:
+            # 如果当前的标准差超过了阈值，记录隔断点的索引位置，并重置开始索引为当前位置
+            start_index = i - 1  # 重置为当前位置，因为i是从1开始的
+            std_values.append(None)  # 使用 None 表示隔断点
+            break_points.append(start_index)
+        else:
+            std_values.append(current_std)
+
+    return std_values, break_points
+
+def apply_grubbs_test(data: List[TimeSeriesData], alpha: float=0.05) -> List[float]:
     """实现格拉布斯检验函数"""
     values = [item.value for item in data]
     n = len(values)
     outliers = []
 
     while True:
         mean = np.mean(values)
@@ -1437,36 +1842,36 @@
 
         outliers.append(data.pop(max_residual_idx))
         values = [item.value for item in data]
         n -= 1
 
     return outliers
 
-def calculate_z_scores(data):
+def calculate_z_scores(data: List[TimeSeriesData]) -> List[float]:
     """计算Z分数"""
     values = [item.value for item in data]
     mean = np.mean(values)
     std = np.std(values)
     z_scores = []
     for item in data:
         z_score = (item.value - mean) / std
         z_scores.append(z_score)
     return z_scores
-def detect_outliers(z_scores, threshold=3):
-    """标记异常值：
+def detect_outliers(z_scores: List[float], threshold: float=3) -> List[float]:
+    """标记异常值:
     z_scores = calculate_z_scores(data)
     outliers = detect_outliers(z_scores, threshold=3)
     """
     outliers = []
     for i, z_score in enumerate(z_scores):
         if z_score < -threshold or z_score > threshold:
             outliers.append(i)
     return outliers
 
-def apply_dbscan_clustering(data, epsilon, min_samples):
+def apply_dbscan_clustering(data: List[TimeSeriesData], epsilon, min_samples):
     """
     实现DBSCAN聚类函数
     epsilon = 0.5  # DBSCAN的邻域半径
     min_samples = 5  # 聚类的最小样本数
     clusters = apply_dbscan_clustering(data, epsilon, min_samples)
     """
     values = np.array([item.value for item in data]).reshape(-1, 1)
@@ -1491,26 +1896,127 @@
         mean_after = np.mean(window_values[window_size // 2:])
         std_dev = np.std(window_values)
         t_statistic = (mean_after - mean_before) / (std_dev / np.sqrt(window_size // 2))
         p_value = 2 * (1 - t.cdf(abs(t_statistic), df=window_size - 1))
         results.append((time_series_data[i + window_size // 2].datetime, t_statistic, p_value))
     
     return results
+
+def calculate_control_limits(data):
+    values = np.array([point.value for point in data])
+    n = len(data)  # 样本大小
+    sigma = np.std(values)  # 样本标准差
+    X_bar = np.mean(values)  # 样本均值
+    CL_X_bar = X_bar
+    UCL_X_bar = X_bar + 3 * sigma / np.sqrt(n)  # 上控制限
+    LCL_X_bar = X_bar - 3 * sigma / np.sqrt(n)  # 下控制限
+
+    R_values = np.abs(np.diff(values))  # 计算样本范围
+    CL_R = np.mean(R_values)  # 样本范围的均值
+    UCL_R = 3 * CL_R  # 上控制限
+    LCL_R = 0  # 下控制限
+
+    return CL_X_bar, UCL_X_bar, LCL_X_bar, CL_R, UCL_R, LCL_R
+
+def plot_x_hart_control_chart(data: List[TimeSeriesData], SaveFilePath: Optional[str]=None) -> None:
+    CL_X_bar, UCL_X_bar, LCL_X_bar, CL_R, UCL_R, LCL_R = calculate_control_limits(data)
+
+    values = [point.value for point in data]
+    dates = [point.datetime for point in data]
+
+    plt.figure(figsize=(12, 6))
+
+    plt.subplot(2, 1, 1)
+    plt.plot(dates, values, 'b-', label='数据值')
+    plt.axhline(y=CL_X_bar, color='r', linestyle='--', label='中心线')
+    plt.axhline(y=UCL_X_bar, color='g', linestyle='--', label='上控制限')
+    plt.axhline(y=LCL_X_bar, color='g', linestyle='--', label='下控制限')
+    plt.title('X-bar 控制图')
+    plt.xlabel('日期')
+    plt.ylabel('数值')
+    plt.legend()
+
+    plt.subplot(2, 1, 2)
+    R_values = np.abs(np.diff(values))
+    plt.plot(dates[:-1], R_values, 'b-', label='R 值')
+    plt.axhline(y=CL_R, color='r', linestyle='--', label='中心线')
+    plt.axhline(y=UCL_R, color='g', linestyle='--', label='上控制限')
+    plt.axhline(y=LCL_R, color='g', linestyle='--', label='下控制限')
+    plt.title('R 控制图')
+    plt.xlabel('日期')
+    plt.ylabel('范围')
+    plt.legend()
+
+    plt.tight_layout()
+    if SaveFilePath is not None:
+        plt.savefig(SaveFilePath) 
+    else:
+        plt.show()
+    plt.close()
+
+def ewma(data, alpha=0.2):
+    """
+    计算指数加权移动平均
+    :param data: 数据序列
+    :param alpha: 平滑系数,控制对最新观测值的权重,通常取值范围为[0, 1]
+    :return: 指数加权移动平均序列
+    """
+    ewma_values = [data[0].value]  # 初始化第一个值为初始EWMA值
+    for i in range(1, len(data)):
+        ewma_values.append(alpha * data[i].value + (1 - alpha) * ewma_values[-1])
+    return np.array(ewma_values)
+
+def calculate_control_limits_ewma(data, alpha=0.2):
+    """
+    计算EWMA控制图的控制限
+    :param data: 数据序列
+    :param alpha: 平滑系数
+    :return: CL, UCL, LCL:中心线、上控制限、下控制限
+    """
+    ewma_values = ewma(data, alpha)
+    CL = np.mean(ewma_values)  # 中心线即为EWMA序列的均值
+    std_dev = np.std(ewma_values)  # 计算EWMA序列的标准差
+
+    # 计算控制限
+    UCL = CL + 3 * std_dev
+    LCL = CL - 3 * std_dev
+
+    return CL, UCL, LCL
+
+def plot_control_limits_ewma(data: List[TimeSeriesData], alpha=0.2, SaveFilePath: Optional[str]=None) -> None:
+    # 将数据转换为列表以便计算
+    data_values = [point.value for point in data]
+
+    # 计算EWMA控制图的控制限
+    CL, UCL, LCL = calculate_control_limits_ewma(data, alpha)
+
+    # 绘制EWMA控制图
+    plt.plot(data_values, label='数据')
+    plt.plot([CL] * len(data_values), 'r--', label='中心线')
+    plt.plot([UCL] * len(data_values), 'g--', label='上控制限')
+    plt.plot([LCL] * len(data_values), 'b--', label='下控制限')
+    plt.xlabel('样本')
+    plt.ylabel('数值')
+    plt.title('指数加权移动平均控制图')
+    plt.legend()
+    if SaveFilePath is not None:
+        plt.savefig(SaveFilePath) 
+    else:
+        plt.show()
+    plt.close()
 # endregion
 # region scikit-learn使用
 def calculate_similarity(ts1, ts2, similarity_metric='euclidean'):
     """
     计算两个时间序列之间的相似性或差异性
-
     Args:
         ts1 (list or numpy array): 第一个时间序列
         ts2 (list or numpy array): 第二个时间序列
         similarity_metric (str, optional): 相似性度量方法,默认为'euclidean'(欧氏距离)。可选值包括'euclidean'(欧氏距离),
                                             'pearson'(皮尔逊相关系数)。
-
     Returns:
         float: 两个时间序列之间的相似性或差异性值
     """
     if similarity_metric == 'euclidean':
         # 计算欧氏距离
         similarity = euclidean(ts1, ts2)
     elif similarity_metric == 'pearson':
@@ -2380,26 +2886,336 @@
     plt.plot(denoised_signal, label='去噪后信号')
     plt.xlabel('时间')
     plt.ylabel('幅值')
     plt.title('时序信号去噪')
     plt.legend()
     plt.show()
 # endregion
+# region 概率论相关
+def kernel_density_estimation(data: List[TimeSeriesData], SaveFilePath: Optional[str]=None) -> None:
+    # 从TimeSeriesData对象列表中提取值,并将其转换为numpy数组
+    values = np.array([data_point.value for data_point in data])
+
+    # 使用高斯核函数创建核密度估计对象
+    kde = gaussian_kde(values)
+
+    # 定义用于计算核密度函数的数据点集合
+    density_x = np.linspace(min(values), max(values), 100)
+
+    # 计算核密度估计的概率密度函数值
+    density_y = kde(density_x)
+
+    # 绘制核密度估计结果
+    plt.plot(density_x, density_y)
+    plt.xlabel('数值')
+    plt.ylabel('密度')
+    plt.title('核密度估计')
+    if SaveFilePath is not None:
+        plt.savefig(SaveFilePath) 
+    else:
+        plt.show()
+    plt.close()
+# endregion
+# region 聚类分析np.ndarray
+def cluster_analysis(complete_trend_line: np.ndarray, num_clusters: int) -> np.ndarray:
+    """使用 K-means 聚类算法对趋势线进行聚类分析"""
+    # Reshape the trend line array to be a column vector
+    trend_line_vector = complete_trend_line.reshape(-1, 1)
+
+    # Initialize KMeans model
+    kmeans = KMeans(n_clusters=num_clusters, random_state=0)
+
+    # Fit KMeans model to the trend line data
+    kmeans.fit(trend_line_vector)
+
+    # Get the cluster labels
+    cluster_labels = kmeans.labels_
+
+    return cluster_labels
+
+def cluster_analysis_GMM(complete_trend_line: np.ndarray, num_clusters: int) -> np.ndarray:
+    """使用高斯混合聚类算法GMM 对趋势线进行聚类分析"""
+    # Reshape the trend line array to be a column vector
+    trend_line_vector = complete_trend_line.reshape(-1, 1)
+
+    # Initialize Gaussian Mixture model
+    gmm = GaussianMixture(n_components=num_clusters, random_state=0)
+
+    # Fit Gaussian Mixture model to the trend line data
+    gmm.fit(trend_line_vector)
+
+    # Predict the cluster labels
+    cluster_labels = gmm.predict(trend_line_vector)
+
+    return cluster_labels
+
+def cluster_analysis_GMM_in_GridSearchCV(complete_trend_line: np.ndarray) -> np.ndarray:
+    """使用高斯混合聚类算法对趋势线进行聚类分析"""
+    # Reshape the trend line array to be a column vector
+    trend_line_vector = complete_trend_line.reshape(-1, 1)
+
+    # 定义参数网格
+    param_grid = {'n_components': np.arange(2, 11)}  # 可以根据需求调整范围
+
+    # 初始化 Gaussian Mixture model
+    gmm = GaussianMixture(random_state=0)
+
+    # 使用 GridSearchCV 寻找最优参数值
+    grid_search = GridSearchCV(gmm, param_grid, cv=5)  # 5折交叉验证
+    grid_search.fit(trend_line_vector)
+
+    # 打印最优参数值
+    print("最优的 n_components 参数值:", grid_search.best_params_)
+
+    # 使用最优参数值重新训练模型
+    best_gmm = grid_search.best_estimator_
+    best_gmm.fit(trend_line_vector)
+
+    # 预测聚类标签
+    cluster_labels = best_gmm.predict(trend_line_vector)
+
+    return cluster_labels
+
+def cluster_analysis_AgglomerativeClustering(complete_trend_line: np.ndarray, num_clusters: int) -> np.ndarray:
+    """使用层次聚类算法对趋势线进行聚类分析"""
+    # Reshape the trend line array to be a column vector
+    trend_line_vector = complete_trend_line.reshape(-1, 1)
+
+    # Initialize Agglomerative Clustering model
+    agg_clustering = AgglomerativeClustering(n_clusters=num_clusters)
+
+    # Fit Agglomerative Clustering model to the trend line data
+    cluster_labels = agg_clustering.fit_predict(trend_line_vector)
+
+    return cluster_labels
+
+def cluster_analysis_DBSCAN(complete_trend_line: np.ndarray, eps: float = 0.5, min_samples: int = 2) -> np.ndarray:
+    """
+    使用DBSCAN算法对趋势线进行聚类分析
+    参数：
+        - complete_trend_line: 包含完整趋势线的数组
+        - eps: DBSCAN算法中的邻域半径
+        - min_samples: DBSCAN算法中的最小样本数
+    返回值：
+        - cluster_labels: 聚类标签数组
+    """
+    # Reshape the trend line array to be a column vector
+    trend_line_vector = complete_trend_line.reshape(-1, 1)
+
+    # Initialize DBSCAN model
+    dbscan = DBSCAN(eps=eps, min_samples=min_samples)
+
+    # Fit DBSCAN model to the trend line data
+    cluster_labels = dbscan.fit_predict(trend_line_vector)
+
+    return cluster_labels
+
+def cluster_cluster_labels_with_score(complete_trend_line: np.ndarray, cluster_labels: np.ndarray) -> tuple:
+    """
+    """
+    # 将趋势线数组重塑为列向量
+    trend_line_vector = complete_trend_line.reshape(-1, 1)
+
+    # 计算轮廓系数
+    silhouette = silhouette_score(trend_line_vector, cluster_labels)
+
+    # 计算 Davies-Bouldin 指数
+    davies_bouldin = davies_bouldin_score(trend_line_vector, cluster_labels)
+
+    # 计算 Calinski-Harabasz 指数
+    calinski_harabasz = calinski_harabasz_score(trend_line_vector, cluster_labels)
+
+    return silhouette, davies_bouldin, calinski_harabasz
+
+def elbow_method(complete_trend_line: np.ndarray, max_clusters: int) -> None:
+    """
+    使用平均肘法选择最优的聚类数
+    参数：
+        - complete_trend_line: 包含完整趋势线的数组
+        - max_clusters: 最大的聚类数
+    """
+    # Reshape the trend line array to be a column vector
+    trend_line_vector = complete_trend_line.reshape(-1, 1)
+    
+    # 存储每个聚类数的平均轮廓系数
+    silhouette_scores = []
+    
+    # 计算每个聚类数对应的平均轮廓系数
+    for i in range(2, max_clusters + 1):
+        kmeans = KMeans(n_clusters=i, random_state=0)
+        cluster_labels = kmeans.fit_predict(trend_line_vector)
+        silhouette_avg = silhouette_score(trend_line_vector, cluster_labels)
+        silhouette_scores.append(silhouette_avg)
+    
+    # 绘制肘部法则图
+    plt.plot(range(2, max_clusters + 1), silhouette_scores, marker='o', label='平均轮廓系数')
+    plt.xlabel('聚类数')
+    plt.ylabel('平均轮廓系数')
+    plt.title('平均肘法')
+    for i, txt in enumerate(silhouette_scores):
+        plt.annotate(round(txt, 2), (i+2, silhouette_scores[i]), textcoords="offset points", xytext=(0,10), ha='center')
+    plt.legend()
+    plt.show()
+
+def elbow_method_GMM(complete_trend_line: np.ndarray, max_clusters: int) -> None:
+    """
+    使用肘部法则选择最优的聚类数
+    参数：
+        - complete_trend_line: 包含完整趋势线的数组
+        - max_clusters: 最大的聚类数
+    """
+    # Reshape the trend line array to be a column vector
+    trend_line_vector = complete_trend_line.reshape(-1, 1)
+    
+    # 存储每个聚类数的似然函数值
+    likelihoods = []
+    
+    # 计算每个聚类数对应的似然函数值
+    for i in range(1, max_clusters + 1):
+        gmm = GaussianMixture(n_components=i, random_state=0)
+        gmm.fit(trend_line_vector)
+        likelihoods.append(gmm.score(trend_line_vector))
+    
+    # 绘制肘部法则图
+    plt.plot(range(1, max_clusters + 1), likelihoods, marker='o', label='似然函数值')
+    plt.xlabel('聚类数')
+    plt.ylabel('对数似然函数值')
+    plt.title('肘部法则')
+    for i, txt in enumerate(likelihoods):
+        plt.annotate(round(txt, 2), (i+1, likelihoods[i]), textcoords="offset points", xytext=(0,10), ha='center')
+    plt.legend()
+    plt.show()
+
+def cluster_evaluation(complete_trend_line: np.ndarray, cluster_labels: np.ndarray, true_labels: np.ndarray) -> tuple:
+    """
+    评估聚类模型的拟合优度和聚类结果与原始类别之间的契合度
+    参数：
+        - complete_trend_line: 包含完整趋势线的数组
+        - cluster_labels: 聚类标签数组
+        - true_labels: 真实的类别标签数组
+    返回值：
+        - silhouette: Silhouette Score
+        - v_measure: V-Measure Score
+    """
+    # 计算 Silhouette Score
+    silhouette = silhouette_score(complete_trend_line.reshape(-1, 1), cluster_labels)
+    
+    # 计算 V-Measure Score
+    v_measure = v_measure_score(true_labels, cluster_labels)
+    
+    return silhouette, v_measure
+
+def visualize_clusters(complete_trend_line: np.ndarray, cluster_labels: np.ndarray) -> None:
+    """可视化聚类分析结果"""
+    plt.figure(figsize=(10, 6))
+
+    # 绘制散点图，按照聚类标签进行着色
+    plt.scatter(np.arange(len(complete_trend_line)), complete_trend_line, c=cluster_labels, cmap='viridis', alpha=0.5, s=10)
+
+    # 标记聚类中心
+    cluster_centers = []
+    for i in range(max(cluster_labels) + 1):
+        cluster_center = np.mean(complete_trend_line[cluster_labels == i])
+        cluster_centers.append(cluster_center)
+        plt.scatter(np.arange(len(complete_trend_line))[cluster_labels == i], complete_trend_line[cluster_labels == i], label=f'Cluster {i}', alpha=0.5, s=10)
+        plt.plot([0, len(complete_trend_line)], [cluster_center, cluster_center], 'k--')
+
+    plt.title('趋势线的聚类分析')
+    plt.xlabel('数据点')
+    plt.ylabel('数值')
+    plt.legend()
+    plt.grid(True)
+    plt.show()
+
+def normalize_features(features: np.ndarray) -> np.ndarray:
+    """标准化特征"""
+    scaler = StandardScaler()
+    scaled_features = scaler.fit_transform(features)
+    return scaled_features
+
+# endregion
+
+
+# # 创建 TimeSeriesData 实例
+start_time = time.time()  # 记录程序开始时间
+data = load_csv_data("D:\python_proj2\daily_data_1.txt")
+
+
+# 计算 value 的平均值
+mean_value = np.mean([point.value for point in data])
+# 减去平均值
+for point in data:
+    point.value -= mean_value
+    point.value = point.value * 1000
+#TODO:基于累积和-休哈特控制图的趋势项自适应拟合
+#TODO:基于EWMA控制图的趋势项自适应拟合
+
+# target_value = 0  # Set an appropriate target value based on your data context
+# cusum_pos, cusum_neg = calculate_cusum(data, target_value)
+# plot_cusum_pos_and_neg(cusum_pos, cusum_neg)
+# region 基于累计标准差隔断分组的拟合趋势线
+
+# std_values = calculate_rolling_std(data, 60)
+
+# show_prcoess_time(start_time, "adaptive_polynomial_fitting")
+
+# values = [entry.value for entry in data]
+# std_value = np.std(values)
+# value_np = np.asarray(values)
+# threshold = std_value / 2.0
+
+
+# std_values, break_points = calculate_cumulative_std_with_break(data, threshold)
+# segmented_data = split_time_series_data(data, break_points)
+# complete_trend_line = fit_and_concatenate_trend_lines(segmented_data)
+# plot_polynomial_trend(data, complete_trend_line)
+# endregion
+# region 做聚类分析的实验
+# max_clusters = 10
+
+# # 使用肘部法则选择最优聚类数
+# # elbow_method(complete_trend_line, max_clusters)
+
+# num_clusters = 3
+# cluster_labels = cluster_analysis_DBSCAN(complete_trend_line, num_clusters)
+# silhouette, davies_bouldin, calinski_harabasz = cluster_cluster_labels_with_score(complete_trend_line, cluster_labels)
+
+# print("轮廓系数:", silhouette)
+# print("Davies-Bouldin 指数:", davies_bouldin)
+# print("Calinski-Harabasz 指数:", calinski_harabasz)
+# check_data_type(cluster_labels)
+# visualize_clusters(complete_trend_line, cluster_labels)
+# endregion
 
-# # # 创建 TimeSeriesData 实例
-# data = load_csv_data()
-# # 计算 value 的平均值
-# mean_value = np.mean([point.value for point in data])
-# # 减去平均值
-# for point in data:
-#     point.value -= mean_value
-#     point.value =point.value*1000
+# region 自适应趋势拟合实验
+# plot_control_limits_ewma(data)
 
-# plot_TimeSeriesData(isShow=True,TimeSeriesData=data)
 
+# plot_x_hart_control_chart(data)
+
+# cusum_values = cusum(data, 0.5)
+# threshold = determine_threshold(cusum_values)
+# plot_cusum_in_threshold(cusum_values, threshold)
+# print(threshold)
+# save_list_to_txt(cusum_values, 'data.txt')
+# adaptive_polynomial_fitting_in_cusum(data)
+
+
+
+# accelerations=calculate_acceleration(data)
+# print(f"Origin: {len(data)}, acc: {len(accelerations)}")
+# # plot_acceleration(data, accelerations)
+complete_trend_line = adaptive_polynomial_fitting(data, 11.5)
+# print(f"Origin: {len(data)}, complete_trend_line: {len(complete_trend_line)}")
+
+show_prcoess_time(start_time, "adaptive_polynomial_fitting")
+plot_polynomial_trend(data[1:len(data)], complete_trend_line)
+# endregion
+
+# region 趋势线评估实验
 # degree=11
 # alpha=1.0
 # y_pred=fit_Ridge_polynomial_trend(data,11)
 # residuals=calculate_trend_line_residuals(data,y_pred)
 # plot_residuals(residuals)
 # durbin_watson_statistic=calculate_durbin_watson(residuals)
 # print("Durbin-Watson statistic (德宾沃森统计量):", durbin_watson_statistic)
@@ -2411,19 +3227,21 @@
 # print("P值:", p_value)
 
 # ridge_pred=fit_Ridge_polynomial_trend(data,degree,alpha)
 # lasso_pred=fit_Lasso_polynomial_trend(data,degree)
 # elastic_pred=fit_ElasticNet_polynomial_trend(data,degree)
 # polynomial_pred=fit_polynomial_trend(data,degree)
 # euclidean_distances, pearson_correlations, f_statistic, p_value = compare_trend_lines(ridge_pred, lasso_pred, elastic_pred, polynomial_pred)
-# print("欧几里得距离：", euclidean_distances)
-# print("皮尔逊相关系数：", pearson_correlations)
-# print("ANOVA F统计量：", f_statistic)
-# print("ANOVA p值：", p_value)
+# print("欧几里得距离:", euclidean_distances)
+# print("皮尔逊相关系数:", pearson_correlations)
+# print("ANOVA F统计量:", f_statistic)
+# print("ANOVA p值:", p_value)
 # # 执行滑动T检验
 # window_size = 10
 # significance_level = 0.05
 # results = sliding_t_test(data, window_size, significance_level)
 
 # # 打印检验结果
 # for result in results:
 #     print("时间:", result[0],"T统计量:", result[1],"P值:", result[2],"显著性结果:", "存在显著的突变" if result[2] < significance_level else "无显著的突变")
+
+# endregion
```

