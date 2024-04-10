# Comparing `tmp/gwas_tools-0.14.7-py3-none-any.whl.zip` & `tmp/gwas_tools-0.14.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 61532 bytes, number of entries: 27
--rw-rw-r--  2.0 unx      850 b- defN 24-Mar-19 14:37 gwas_tools/__init__.py
+Zip file size: 61662 bytes, number of entries: 27
+-rw-rw-r--  2.0 unx      850 b- defN 24-Apr-10 20:24 gwas_tools/__init__.py
 -rw-rw-r--  2.0 unx      757 b- defN 23-Feb-27 19:30 gwas_tools/algorithms/__init__.py
--rw-rw-r--  2.0 unx    11593 b- defN 24-Mar-12 10:49 gwas_tools/algorithms/scattered_light.py
+-rw-rw-r--  2.0 unx    12000 b- defN 24-Apr-10 20:24 gwas_tools/algorithms/scattered_light.py
 -rw-rw-r--  2.0 unx     9260 b- defN 23-Dec-05 17:32 gwas_tools/algorithms/scattered_light_gwf.py
 -rw-rw-r--  2.0 unx     5635 b- defN 23-Feb-27 19:30 gwas_tools/algorithms/scattered_light_raw.py
 -rw-rw-r--  2.0 unx      757 b- defN 23-Feb-27 19:30 gwas_tools/automation/__init__.py
 -rw-rw-r--  2.0 unx     9869 b- defN 23-Feb-27 19:30 gwas_tools/automation/scripts.py
 -rw-rw-r--  2.0 unx      757 b- defN 23-Feb-27 19:30 gwas_tools/common/__init__.py
 -rw-rw-r--  2.0 unx     4953 b- defN 24-Mar-12 09:10 gwas_tools/common/defines.py
 -rw-rw-r--  2.0 unx      757 b- defN 23-Feb-27 19:30 gwas_tools/helpers/__init__.py
@@ -17,13 +17,13 @@
 -rw-rw-r--  2.0 unx      757 b- defN 23-Feb-27 19:30 gwas_tools/summary_pages/__init__.py
 -rw-rw-r--  2.0 unx     8279 b- defN 23-Dec-17 19:02 gwas_tools/summary_pages/daily_correlations_page.py
 -rw-rw-r--  2.0 unx     9852 b- defN 24-Feb-11 15:48 gwas_tools/summary_pages/scattered_light_page.py
 -rw-rw-r--  2.0 unx      757 b- defN 23-Feb-27 19:30 gwas_tools/utils/__init__.py
 -rw-rw-r--  2.0 unx    25112 b- defN 24-Mar-12 09:26 gwas_tools/utils/file_utils.py
 -rw-rw-r--  2.0 unx    27945 b- defN 24-Mar-19 13:49 gwas_tools/utils/plot_utils.py
 -rw-rw-r--  2.0 unx    19188 b- defN 24-Mar-12 10:01 gwas_tools/utils/signal_utils.py
--rw-rw-r--  2.0 unx    35149 b- defN 24-Mar-23 08:37 gwas_tools-0.14.7.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2877 b- defN 24-Mar-23 08:37 gwas_tools-0.14.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-23 08:37 gwas_tools-0.14.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 24-Mar-23 08:37 gwas_tools-0.14.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2400 b- defN 24-Mar-23 08:37 gwas_tools-0.14.7.dist-info/RECORD
-27 files, 200312 bytes uncompressed, 57616 bytes compressed:  71.2%
+-rw-rw-r--  2.0 unx    35149 b- defN 24-Apr-10 20:26 gwas_tools-0.14.8.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2877 b- defN 24-Apr-10 20:26 gwas_tools-0.14.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-10 20:26 gwas_tools-0.14.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 24-Apr-10 20:26 gwas_tools-0.14.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2400 b- defN 24-Apr-10 20:26 gwas_tools-0.14.8.dist-info/RECORD
+27 files, 200719 bytes uncompressed, 57746 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -60,23 +60,23 @@
 
 Filename: gwas_tools/utils/plot_utils.py
 Comment: 
 
 Filename: gwas_tools/utils/signal_utils.py
 Comment: 
 
-Filename: gwas_tools-0.14.7.dist-info/LICENSE
+Filename: gwas_tools-0.14.8.dist-info/LICENSE
 Comment: 
 
-Filename: gwas_tools-0.14.7.dist-info/METADATA
+Filename: gwas_tools-0.14.8.dist-info/METADATA
 Comment: 
 
-Filename: gwas_tools-0.14.7.dist-info/WHEEL
+Filename: gwas_tools-0.14.8.dist-info/WHEEL
 Comment: 
 
-Filename: gwas_tools-0.14.7.dist-info/top_level.txt
+Filename: gwas_tools-0.14.8.dist-info/top_level.txt
 Comment: 
 
-Filename: gwas_tools-0.14.7.dist-info/RECORD
+Filename: gwas_tools-0.14.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gwas_tools/__init__.py

```diff
@@ -11,9 +11,9 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 
-__version__ = "0.14.7"
+__version__ = "0.14.8"
 __authors__ = "Stefano Bianchi, Alessandro Longo, Guillermo Valdes"
```

## gwas_tools/algorithms/scattered_light.py

```diff
@@ -141,14 +141,23 @@
     for k in range(imfs.shape[1]):
         upper_env = signal_utils.upper_envelope(imfs[:, k])[1:]
         upper_env = signal_utils.smooth(upper_env, smooth_win)
         envelopes[:, k] = upper_env
         for l in range(predictor.shape[1]):
             corrs[k, l] = signal_utils.get_correlation_between(predictor[:, l], upper_env)
 
+    # print list of imfs and corrs
+    max_corrs_to_print = 10
+    corrs_ord_idx = np.argsort(corrs, axis=1)
+    for k in range(imfs.shape[1]):
+        print("IMF {}".format(k + 1))
+        imf_corrs = corrs_ord_idx[k, :][::-1]
+        for i in range(min(max_corrs_to_print, len(imf_corrs))):
+            print("  - Predictor: {} - Rho: {:.3f}".format(channels_list[imf_corrs[i]], corrs[k, imf_corrs[i]]))
+
     if save_data:
         # save instantaneous amplitudes and imfs
         file_utils.save_envelopes(envelopes, "_".join(target_channel_name.split(":")), out_path)
         file_utils.save_imfs(imfs, "_".join(target_channel_name.split(":")), out_path)
 
     # max correlations
     max_vals = np.max(corrs, axis=1)
```

## Comparing `gwas_tools-0.14.7.dist-info/LICENSE` & `gwas_tools-0.14.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gwas_tools-0.14.7.dist-info/METADATA` & `gwas_tools-0.14.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwas_tools
-Version: 0.14.7
+Version: 0.14.8
 Summary: Utils functions to build a pipeline for scattered light noise hunting in gravitational waves detectors.
 Home-page: https://github.com/FisicaTre/gwas_tools
 Author: Stefano Bianchi, Alessandro Longo, Guillermo Valdes
 Author-email: stefanobianchi9@gmail.com
 License: GPLv3.0
 Project-URL: Bug Reports, https://github.com/FisicaTre/gwas_tools/issues
 Project-URL: Source, https://github.com/FisicaTre/gwas_tools
```

## Comparing `gwas_tools-0.14.7.dist-info/RECORD` & `gwas_tools-0.14.8.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-gwas_tools/__init__.py,sha256=uraX5LqU_NNVaF3apWszyo2ezRfSg9db5u1vTzHJ31U,850
+gwas_tools/__init__.py,sha256=AEaLOZ1Nxou4b1s-JGIf7J_g4ehu5YNrp0LyNCoz7zE,850
 gwas_tools/algorithms/__init__.py,sha256=qT18Dif5mWxCzDnnsywYhZ4ZZvn7R9nh49qu_havJBQ,757
-gwas_tools/algorithms/scattered_light.py,sha256=4Fxxs1qVqNdfN6RyfnBzCTAQkudgedkjKnEJlxEzc9Y,11593
+gwas_tools/algorithms/scattered_light.py,sha256=0wTK42NKl0qT3ibJOrRwlUyo8Zzrx4C5zu28h9DbLiM,12000
 gwas_tools/algorithms/scattered_light_gwf.py,sha256=0fsOG3CrN1hdCXoQ5aW2xEDQY7LcWLWcOce8yb-28-o,9260
 gwas_tools/algorithms/scattered_light_raw.py,sha256=kEqX1lamC-eC7ABKONXeHUqzbYvRjR27XJZ8w7xF5lw,5635
 gwas_tools/automation/__init__.py,sha256=qT18Dif5mWxCzDnnsywYhZ4ZZvn7R9nh49qu_havJBQ,757
 gwas_tools/automation/scripts.py,sha256=HmrqqXgVK8WNfKITyMBbk8BdwvTXotOsFx5up0tWqTg,9869
 gwas_tools/common/__init__.py,sha256=qT18Dif5mWxCzDnnsywYhZ4ZZvn7R9nh49qu_havJBQ,757
 gwas_tools/common/defines.py,sha256=odyN905zk_07LNm6l1Xla2-C5i1igG38diSoqm3mCTs,4953
 gwas_tools/helpers/__init__.py,sha256=qT18Dif5mWxCzDnnsywYhZ4ZZvn7R9nh49qu_havJBQ,757
@@ -16,12 +16,12 @@
 gwas_tools/summary_pages/__init__.py,sha256=qT18Dif5mWxCzDnnsywYhZ4ZZvn7R9nh49qu_havJBQ,757
 gwas_tools/summary_pages/daily_correlations_page.py,sha256=FKH75HK1z27Kcb1YyoE4cO0DhIEqo-m3HBJHWP6cVSc,8279
 gwas_tools/summary_pages/scattered_light_page.py,sha256=vDDsbZp7G11qFLJyTpEJx0Kd3a0gFMvmGByk0h5UdeM,9852
 gwas_tools/utils/__init__.py,sha256=qT18Dif5mWxCzDnnsywYhZ4ZZvn7R9nh49qu_havJBQ,757
 gwas_tools/utils/file_utils.py,sha256=Ne2UG0Yv1wcavTyt2UW8bi4Wkjs50AZUeltFElt_l6c,25112
 gwas_tools/utils/plot_utils.py,sha256=LyMo5Ra-k6621yAwPF3kbJK4e8Fl6g8AuM650GawI28,27945
 gwas_tools/utils/signal_utils.py,sha256=sBFiV9dhuMy-gvdJ6Xir3z94iYifhkpDrwcvUnyH7WQ,19188
-gwas_tools-0.14.7.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-gwas_tools-0.14.7.dist-info/METADATA,sha256=y7mHNufu-RCbzyeLJwCK8cUaMyhIGGtFF0vNeH0ClJg,2877
-gwas_tools-0.14.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-gwas_tools-0.14.7.dist-info/top_level.txt,sha256=opq89zT-Pmouhdx0CiHl5Aa0yIMXlhuokWcQuMn1zUU,11
-gwas_tools-0.14.7.dist-info/RECORD,,
+gwas_tools-0.14.8.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+gwas_tools-0.14.8.dist-info/METADATA,sha256=fyF90leyJz3vdFLmH0UCTuUORIOLE9ZRYDdHHEK1Pfo,2877
+gwas_tools-0.14.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+gwas_tools-0.14.8.dist-info/top_level.txt,sha256=opq89zT-Pmouhdx0CiHl5Aa0yIMXlhuokWcQuMn1zUU,11
+gwas_tools-0.14.8.dist-info/RECORD,,
```

