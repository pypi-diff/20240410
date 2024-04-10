# Comparing `tmp/obsinthe-0.0.2.tar.gz` & `tmp/obsinthe-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsinthe-0.0.2.tar", max compression
+gzip compressed data, was "obsinthe-0.0.3.tar", max compression
```

## Comparing `obsinthe-0.0.2.tar` & `obsinthe-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0    10767 2024-03-12 08:34:34.610560 obsinthe-0.0.2/LICENSE
--rw-r--r--   0        0        0        0 2024-03-16 20:49:21.445270 obsinthe-0.0.2/obsinthe/alerts/__init__.py
--rw-r--r--   0        0        0     2597 2024-03-16 21:26:02.968241 obsinthe-0.0.2/obsinthe/alerts/grouping.py
--rw-r--r--   0        0        0      461 2024-03-16 20:51:58.249890 obsinthe-0.0.2/obsinthe/deps.py
--rw-r--r--   0        0        0     1683 2024-03-12 08:34:34.610560 obsinthe-0.0.2/obsinthe/openshift/symptoms.py
--rw-r--r--   0        0        0       82 2024-03-12 08:34:34.610560 obsinthe-0.0.2/obsinthe/prometheus/__init__.py
--rw-r--r--   0        0        0     6125 2024-03-12 08:34:34.611560 obsinthe-0.0.2/obsinthe/prometheus/client.py
--rw-r--r--   0        0        0    14504 2024-04-02 16:13:31.363148 obsinthe-0.0.2/obsinthe/prometheus/data.py
--rw-r--r--   0        0        0     6684 2024-04-02 16:13:31.364148 obsinthe-0.0.2/obsinthe/prometheus/loader.py
--rw-r--r--   0        0        0      220 2024-03-13 08:48:30.757290 obsinthe-0.0.2/obsinthe/testing/prometheus/__init__.py
--rw-r--r--   0        0        0     3641 2024-03-15 14:22:32.493265 obsinthe-0.0.2/obsinthe/testing/prometheus/alerts.py
--rw-r--r--   0        0        0     6985 2024-03-14 15:58:16.316398 obsinthe-0.0.2/obsinthe/testing/prometheus/builder.py
--rw-r--r--   0        0        0     1765 2024-03-13 16:36:00.559546 obsinthe-0.0.2/obsinthe/testing/prometheus/client.py
--rw-r--r--   0        0        0      418 2024-03-12 08:34:34.611560 obsinthe-0.0.2/obsinthe/utils/jupyter.py
--rw-r--r--   0        0        0     3857 2024-03-13 12:58:00.771010 obsinthe-0.0.2/obsinthe/utils/time.py
--rw-r--r--   0        0        0     1241 2024-03-16 21:25:10.376036 obsinthe-0.0.2/obsinthe/vis/alerts.py
--rw-r--r--   0        0        0      807 2024-03-18 17:49:01.381766 obsinthe-0.0.2/obsinthe/vis/clustering.py
--rw-r--r--   0        0        0     1249 2024-04-02 16:13:35.799167 obsinthe-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 obsinthe-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    10767 2024-03-12 08:34:34.610560 obsinthe-0.0.3/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-16 20:49:21.445270 obsinthe-0.0.3/obsinthe/alerts/__init__.py
+-rw-r--r--   0        0        0     2597 2024-03-16 21:26:02.968241 obsinthe-0.0.3/obsinthe/alerts/grouping.py
+-rw-r--r--   0        0        0      461 2024-03-16 20:51:58.249890 obsinthe-0.0.3/obsinthe/deps.py
+-rw-r--r--   0        0        0     1683 2024-03-12 08:34:34.610560 obsinthe-0.0.3/obsinthe/openshift/symptoms.py
+-rw-r--r--   0        0        0       82 2024-03-12 08:34:34.610560 obsinthe-0.0.3/obsinthe/prometheus/__init__.py
+-rw-r--r--   0        0        0     6125 2024-03-12 08:34:34.611560 obsinthe-0.0.3/obsinthe/prometheus/client.py
+-rw-r--r--   0        0        0    15539 2024-04-10 11:44:09.559431 obsinthe-0.0.3/obsinthe/prometheus/data.py
+-rw-r--r--   0        0        0     6684 2024-04-02 16:13:31.364148 obsinthe-0.0.3/obsinthe/prometheus/loader.py
+-rw-r--r--   0        0        0      220 2024-03-13 08:48:30.757290 obsinthe-0.0.3/obsinthe/testing/prometheus/__init__.py
+-rw-r--r--   0        0        0     3641 2024-03-15 14:22:32.493265 obsinthe-0.0.3/obsinthe/testing/prometheus/alerts.py
+-rw-r--r--   0        0        0     6985 2024-03-14 15:58:16.316398 obsinthe-0.0.3/obsinthe/testing/prometheus/builder.py
+-rw-r--r--   0        0        0     1765 2024-03-13 16:36:00.559546 obsinthe-0.0.3/obsinthe/testing/prometheus/client.py
+-rw-r--r--   0        0        0      394 2024-04-10 11:44:09.559431 obsinthe-0.0.3/obsinthe/utils/data.py
+-rw-r--r--   0        0        0      418 2024-03-12 08:34:34.611560 obsinthe-0.0.3/obsinthe/utils/jupyter.py
+-rw-r--r--   0        0        0     3496 2024-04-10 11:44:09.559431 obsinthe-0.0.3/obsinthe/utils/time.py
+-rw-r--r--   0        0        0     1241 2024-03-16 21:25:10.376036 obsinthe-0.0.3/obsinthe/vis/alerts.py
+-rw-r--r--   0        0        0      807 2024-03-18 17:49:01.381766 obsinthe-0.0.3/obsinthe/vis/clustering.py
+-rw-r--r--   0        0        0     1249 2024-04-10 11:44:34.485681 obsinthe-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 obsinthe-0.0.3/PKG-INFO
```

### Comparing `obsinthe-0.0.2/LICENSE` & `obsinthe-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.2/obsinthe/alerts/grouping.py` & `obsinthe-0.0.3/obsinthe/alerts/grouping.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.2/obsinthe/openshift/symptoms.py` & `obsinthe-0.0.3/obsinthe/openshift/symptoms.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.2/obsinthe/prometheus/client.py` & `obsinthe-0.0.3/obsinthe/prometheus/client.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.2/obsinthe/prometheus/data.py` & `obsinthe-0.0.3/obsinthe/prometheus/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,25 +174,42 @@
         df.drop(columns=["intervals"], inplace=True)
 
         df = pd.concat([df, intervals], axis=1)
         return IntervalsDataset(df)
 
 
 class IntervalsDataset(DatasetBase):
-    def merge_overlaps(self, threshold=timedelta(0), columns=None):
+    def merge_overlaps(self, threshold=timedelta(0), columns=None, keep_rest=False):
         """Merge overlapping time intervals.
 
         Considering a list of time-intervals at the input, merge the rows
         that have the same columns values + have some time overlaps.
+
+        By default, the resulting intervals columns will be
+        `columns + ["start", "end", "sub_intervals"]`.
+
+        To keep the original columns, set `keep_rest=True`. It will keep all
+        original columns except the `start` and `end`. This can potentially lead
+        to multiple rows with the same values in `columns + ['start', 'end']`,
+        but different in the rest of the columns.
         """
         if self.df.empty:
             return self
 
         df = self.df
 
+        df_base = None
+        if keep_rest:
+            df_base = self.df.drop(columns=["start", "end"], axis=1).drop_duplicates()
+
+        if columns is None:
+            columns = list(df.columns.drop(["start", "end"]))
+
+        df = df[columns + ["start", "end"]]
+
         def _identify_intervals(sub_df):
             if len(sub_df) == 1:
                 sub_df["interval_label"] = 0
                 return sub_df
             previous_ends = [None]
             for i in range(1, len(sub_df)):
                 previous_end = sub_df.iloc[i - 1]["end"]
@@ -203,38 +220,42 @@
                 previous_ends.append(previous_end)
 
             sub_df["previous_end"] = previous_ends
             period_start = (sub_df["start"] - sub_df["previous_end"]) > threshold
             sub_df["interval_label"] = period_start.cumsum()
             return sub_df
 
-        if columns is None:
-            columns = list(df.columns.drop(["start", "end"]))
         df = df.sort_values("start")
 
         interval_labels = df.groupby(
             columns, observed=True, as_index=False, dropna=False, group_keys=False
         ).apply(_identify_intervals)
 
         intervals = interval_labels.groupby(
             columns + ["interval_label"],
             observed=True,
             as_index=True,
             dropna=False,
             group_keys=True,
         ).agg(start=("start", "min"), end=("end", "max"))
+
         intervals["sub_intervals"] = interval_labels.groupby(
             columns + ["interval_label"],
             observed=True,
             as_index=True,
             dropna=False,
             group_keys=True,
         ).apply(lambda df: list(zip(df["start"], df["end"])))
 
         intervals.reset_index(inplace=True)
+
+        if df_base is not None:
+            intervals = df_base.merge(intervals, on=columns)
+            intervals.reset_index(drop=True, inplace=True)
+
         intervals.drop("interval_label", axis=1, inplace=True)
 
         return IntervalsDataset(intervals)
 
     def correct_for_resolution(self, resolution: timedelta = DEFAULT_RESOLUTION):
         """Correct the end times of the intervals.
 
@@ -267,16 +288,19 @@
 
     def __iter__(self):
         return iter(self.datasets)
 
     def __repr__(self):
         return f"DatasetCollection with {len(self.datasets)} datasets"
 
-    def fmap(self, fn):
-        return DatasetCollection([fn(ds) for ds in self.datasets])
+    def fmap(self, fn, progress: bool = False, *args, **kwargs):
+        collection = self.datasets
+        if progress:
+            collection = tqdm(collection)
+        return DatasetCollection([fn(ds, *args, **kwargs) for ds in collection])
 
     def query(self, *args, **kwargs):
         return self.fmap(lambda ds: ds.query(*args, **kwargs))
 
     def flatten(self):
         if len(self.datasets) == 0:
             raise ValueError("No datasets to flatten")
@@ -357,15 +381,17 @@
     if is_datetime(ts):
         ts = ts.astype(int) // 1e9
     period_start = ts.diff() > resolution.total_seconds()
     df["interval_label"] = period_start.cumsum()
     return df
 
 
-def intervals_concat_days(ds_collection, threshold=timedelta(0)):
+def intervals_concat_days(
+    ds_collection, threshold=timedelta(0), merge_columns=None, keep_rest=False
+):
     ret_dfs = []
     to_merge_left = None
     for day_ds in tqdm(ds_collection.datasets):
         day_df = day_ds.df
         # Merge the left over from the previous day.
 
         if to_merge_left is not None:
@@ -378,14 +404,16 @@
             # merge the intervals
             merged_df = (
                 IntervalsDataset(
                     pd.concat([to_merge_left, to_merge_right], ignore_index=True)
                 )
                 .merge_overlaps(
                     threshold=threshold,
+                    columns=merge_columns,
+                    keep_rest=keep_rest,
                 )
                 .df
             )
             if "sub_intervals" in merged_df.columns:
                 merged_df.drop("sub_intervals", axis=1, inplace=True)
 
             # Replace the intervals in to_merge_right with the merged ones.
```

### Comparing `obsinthe-0.0.2/obsinthe/prometheus/loader.py` & `obsinthe-0.0.3/obsinthe/prometheus/loader.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.2/obsinthe/testing/prometheus/alerts.py` & `obsinthe-0.0.3/obsinthe/testing/prometheus/alerts.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.2/obsinthe/testing/prometheus/builder.py` & `obsinthe-0.0.3/obsinthe/testing/prometheus/builder.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.2/obsinthe/testing/prometheus/client.py` & `obsinthe-0.0.3/obsinthe/testing/prometheus/client.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.2/obsinthe/utils/time.py` & `obsinthe-0.0.3/obsinthe/utils/time.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from collections import defaultdict
 from datetime import datetime
 from datetime import timedelta
 from datetime import timezone
 from functools import reduce
-from hashlib import sha256
 from typing import Dict
 
 import numpy as np
 import pandas as pd
 from dateutil.rrule import DAILY
 from dateutil.rrule import rrule
 
@@ -19,26 +18,14 @@
     return time.astimezone(timezone.utc)
 
 
 def datetime_start_of_day(dt: datetime) -> datetime:
     return datetime.combine(dt.date(), datetime.min.time(), tzinfo=timezone.utc)
 
 
-def add_row_digest(df: pd.DataFrame, exclude) -> pd.DataFrame:
-    def hash_row(r):
-        return sha256(
-            ("".join(sorted(f"{k,v}" for (k, v) in r.to_dict().items()))).encode(
-                "utf-8"
-            )
-        ).hexdigest()
-
-    df["digest"] = df.drop(exclude, axis=1).apply(hash_row, axis=1)
-    return df
-
-
 def gen_daily_intervals(start, end):
     start, end = normalize_tz(start), normalize_tz(end)
     ticks = [
         d.replace(tzinfo=timezone.utc)
         for d in rrule(DAILY, dtstart=start.date(), until=end.date())
     ]
     ints = list(zip(ticks, ticks[1:]))
```

### Comparing `obsinthe-0.0.2/obsinthe/vis/alerts.py` & `obsinthe-0.0.3/obsinthe/vis/alerts.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.2/obsinthe/vis/clustering.py` & `obsinthe-0.0.3/obsinthe/vis/clustering.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.2/pyproject.toml` & `obsinthe-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "obsinthe"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = []
 packages = [
   {include = "obsinthe"},
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `obsinthe-0.0.2/PKG-INFO` & `obsinthe-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsinthe
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
```

