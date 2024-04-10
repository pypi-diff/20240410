# Comparing `tmp/DynamicRoutingTask-0.1.95.tar.gz` & `tmp/DynamicRoutingTask-0.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DynamicRoutingTask-0.1.95.tar", last modified: Tue Apr  9 01:02:14 2024, max compression
+gzip compressed data, was "DynamicRoutingTask-0.1.96.tar", last modified: Wed Apr 10 02:07:36 2024, max compression
```

## Comparing `DynamicRoutingTask-0.1.95.tar` & `DynamicRoutingTask-0.1.96.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:02:14.814663 DynamicRoutingTask-0.1.95/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:02:14.814663 DynamicRoutingTask-0.1.95/Analysis/
--rw-r--r--   0 runner    (1001) docker     (127)    34540 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/DynamicRoutingAnalysisUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    64516 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/RLmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/RLmodelHPC.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/RLmodelSlurm.py
--rw-r--r--   0 runner    (1001) docker     (127)    34502 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/RLmodel_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    18931 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/behaviorClustering.py
--rw-r--r--   0 runner    (1001) docker     (127)   124608 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/dr_analysis_sam.py
--rw-r--r--   0 runner    (1001) docker     (127)   110108 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/dr_behav_figs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18638 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/dr_ephys_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    21061 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/glm_hmm_sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    32899 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/ncb_meeting_01272023.py
--rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/npc_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    87697 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/presentation_June2023.py
--rw-r--r--   0 runner    (1001) docker     (127)    13758 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/regressionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    69812 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/sac_may2023.py
--rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/sessionSummaryFigs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/sound_ephys_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/sound_sync_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/variableBlockDur.py
--rw-r--r--   0 runner    (1001) docker     (127)    56355 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/DynamicRouting1.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/DynamicRouting1_postSessionAnalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:02:14.814663 DynamicRoutingTask-0.1.95/DynamicRoutingTask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-09 01:02:14.000000 DynamicRoutingTask-0.1.95/DynamicRoutingTask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-09 01:02:14.000000 DynamicRoutingTask-0.1.95/DynamicRoutingTask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 01:02:14.000000 DynamicRoutingTask-0.1.95/DynamicRoutingTask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 01:02:14.000000 DynamicRoutingTask-0.1.95/DynamicRoutingTask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 01:02:14.000000 DynamicRoutingTask-0.1.95/DynamicRoutingTask.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:02:14.814663 DynamicRoutingTask-0.1.95/OptoGui/
--rw-r--r--   0 runner    (1001) docker     (127)    34068 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/OptoGui/OptoGui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/OptoTagging.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-09 01:02:14.814663 DynamicRoutingTask-0.1.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/RFMapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:02:14.814663 DynamicRoutingTask-0.1.95/SamStimGui/
--rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/SamStimGui/SamStimGui.py
--rw-r--r--   0 runner    (1001) docker     (127)    62349 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/TaskControl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/TaskUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/camstimControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-09 01:02:11.000000 DynamicRoutingTask-0.1.95/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/runTask.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 01:02:14.814663 DynamicRoutingTask-0.1.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/startTask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:07:36.467995 DynamicRoutingTask-0.1.96/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:07:36.463995 DynamicRoutingTask-0.1.96/Analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)    34706 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/DynamicRoutingAnalysisUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64516 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/RLmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/RLmodelHPC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/RLmodelSlurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34502 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/RLmodel_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18931 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/behaviorClustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124608 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/dr_analysis_sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110109 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/dr_behav_figs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18638 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/dr_ephys_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21061 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/glm_hmm_sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32899 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/ncb_meeting_01272023.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/npc_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87697 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/presentation_June2023.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13758 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/regressionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69812 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/sac_may2023.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/sessionSummaryFigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/sound_ephys_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/sound_sync_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/variableBlockDur.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56355 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/DynamicRouting1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/DynamicRouting1_postSessionAnalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:07:36.467995 DynamicRoutingTask-0.1.96/DynamicRoutingTask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-10 02:07:36.000000 DynamicRoutingTask-0.1.96/DynamicRoutingTask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-10 02:07:36.000000 DynamicRoutingTask-0.1.96/DynamicRoutingTask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 02:07:36.000000 DynamicRoutingTask-0.1.96/DynamicRoutingTask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-10 02:07:36.000000 DynamicRoutingTask-0.1.96/DynamicRoutingTask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 02:07:36.000000 DynamicRoutingTask-0.1.96/DynamicRoutingTask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:07:36.463995 DynamicRoutingTask-0.1.96/OptoGui/
+-rw-r--r--   0 runner    (1001) docker     (127)    34068 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/OptoGui/OptoGui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/OptoTagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-10 02:07:36.467995 DynamicRoutingTask-0.1.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/RFMapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:07:36.463995 DynamicRoutingTask-0.1.96/SamStimGui/
+-rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/SamStimGui/SamStimGui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62349 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/TaskControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/TaskUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/camstimControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-10 02:07:33.000000 DynamicRoutingTask-0.1.96/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/runTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 02:07:36.467995 DynamicRoutingTask-0.1.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/startTask.py
```

### Comparing `DynamicRoutingTask-0.1.95/Analysis/DynamicRoutingAnalysisUtils.py` & `DynamicRoutingTask-0.1.96/Analysis/DynamicRoutingAnalysisUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,14 +334,15 @@
             try:
                 data = {'start time': pd.to_datetime(obj.startTime,format='%Y%m%d_%H%M%S'),
                         'rig name': obj.rigName,
                         'task version': obj.taskVersion,
                         'hits': obj.hitCount,
                         'd\' same modality': np.round(obj.dprimeSameModal,2),
                         'd\' other modality go stim': np.round(obj.dprimeOtherModalGo,2),
+                        'quiescent violations': obj.quiescentViolationFrames.size,
                         'pass': 0,
                         'ignore': 0}  
                 if df is None:
                     df = pd.DataFrame(data)
                     sessionInd = 0
                 else:
                     if 'rig name' not in df.columns:
@@ -522,14 +523,15 @@
                 data = {'start time': pd.to_datetime(obj.startTime,format='%Y%m%d_%H%M%S'),
                         'rig name': obj.rigName,
                         'computer name': obj.computerName,
                         'task version': obj.taskVersion,
                         'hits': obj.hitCount,
                         'd\' same modality': np.round(obj.dprimeSameModal,2),
                         'd\' other modality go stim': np.round(obj.dprimeOtherModalGo,2),
+                        'quiescent violations': obj.quiescentViolationFrames.size,
                         'ignore': 0}  
                 if df is None:
                     df = pd.DataFrame(data)
                     sessionInd = 0
                 else:
                     sessionInd = df['start time'] == data['start time']
                     sessionInd = np.where(sessionInd)[0][0] if sessionInd.sum()>0 else df.shape[0]
```

### Comparing `DynamicRoutingTask-0.1.95/Analysis/RLmodel.py` & `DynamicRoutingTask-0.1.96/Analysis/RLmodel.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/Analysis/RLmodelHPC.py` & `DynamicRoutingTask-0.1.96/Analysis/RLmodelHPC.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/Analysis/RLmodelSlurm.py` & `DynamicRoutingTask-0.1.96/Analysis/RLmodelSlurm.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/Analysis/RLmodel_old.py` & `DynamicRoutingTask-0.1.96/Analysis/RLmodel_old.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/Analysis/behaviorClustering.py` & `DynamicRoutingTask-0.1.96/Analysis/behaviorClustering.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/Analysis/dr_analysis_sam.py` & `DynamicRoutingTask-0.1.96/Analysis/dr_analysis_sam.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/Analysis/dr_behav_figs.py` & `DynamicRoutingTask-0.1.96/Analysis/dr_behav_figs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1170,15 +1170,15 @@
 ax.set_ylabel('Cumulative Fraction of Variance Explained')
 plt.tight_layout()
 
 nPC = np.where((np.cumsum(eigVal)/eigVal.sum())>0.95)[0][0]+1
 
 clustId,linkageMat = cluster(pcaData[:,:nPC],nClusters=nClust)
 
-newClustOrder = [3,1,2,4]
+newClustOrder = [2,1,4,3]
 newClustId = clustId.copy()
 for i,c in enumerate(newClustOrder):
     newClustId[clustId==c] = i+1
 clustId = newClustId
 
 clustData['clustId'] = clustId
 clustLabels = np.unique(clustId)
@@ -1190,15 +1190,15 @@
     for s in np.unique(clustData['sessionStartTime'][mi]):
         clustData['trialCluster'][m][s] = []
         si = clustData['sessionStartTime']==s
         for n,c in zip(clustData['nBlockTrials'][mi & si],clustId[mi & si]):
             clustData['trialCluster'][m][s].extend(np.zeros(n)+c)
         clustData['trialCluster'][m][s] = np.array(clustData['trialCluster'][m][s])
             
-np.save(os.path.join(baseDir,'Sam','clustData.npy'),clustData)
+#np.save(os.path.join(baseDir,'Sam','clustData.npy'),clustData)
 
 
 plt.figure(facecolor='w')
 ax = plt.subplot(1,1,1)
 colorThresh = 0 if nClust<2 else linkageMat[::-1,2][nClust-2]
 scipy.cluster.hierarchy.set_link_color_palette(list(clustColors))
 scipy.cluster.hierarchy.dendrogram(linkageMat,ax=ax,truncate_mode=None,p=7,color_threshold=colorThresh,above_threshold_color='k',labels=None,no_labels=True)
```

### Comparing `DynamicRoutingTask-0.1.95/Analysis/dr_ephys_analysis.py` & `DynamicRoutingTask-0.1.96/Analysis/dr_ephys_analysis.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/Analysis/glm_hmm_sam.py` & `DynamicRoutingTask-0.1.96/Analysis/glm_hmm_sam.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/Analysis/ncb_meeting_01272023.py` & `DynamicRoutingTask-0.1.96/Analysis/ncb_meeting_01272023.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/Analysis/npc_analysis.py` & `DynamicRoutingTask-0.1.96/Analysis/npc_analysis.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/Analysis/presentation_June2023.py` & `DynamicRoutingTask-0.1.96/Analysis/presentation_June2023.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/Analysis/regressionModel.py` & `DynamicRoutingTask-0.1.96/Analysis/regressionModel.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/Analysis/sac_may2023.py` & `DynamicRoutingTask-0.1.96/Analysis/sac_may2023.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/Analysis/sessionSummaryFigs.py` & `DynamicRoutingTask-0.1.96/Analysis/sessionSummaryFigs.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/Analysis/sound_ephys_analysis.py` & `DynamicRoutingTask-0.1.96/Analysis/sound_ephys_analysis.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/Analysis/sound_sync_test.py` & `DynamicRoutingTask-0.1.96/Analysis/sound_sync_test.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/Analysis/variableBlockDur.py` & `DynamicRoutingTask-0.1.96/Analysis/variableBlockDur.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/DynamicRouting1.py` & `DynamicRoutingTask-0.1.96/DynamicRouting1.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/DynamicRouting1_postSessionAnalysis.py` & `DynamicRoutingTask-0.1.96/DynamicRouting1_postSessionAnalysis.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/DynamicRoutingTask.egg-info/SOURCES.txt` & `DynamicRoutingTask-0.1.96/DynamicRoutingTask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/OptoGui/OptoGui.py` & `DynamicRoutingTask-0.1.96/OptoGui/OptoGui.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/OptoTagging.py` & `DynamicRoutingTask-0.1.96/OptoTagging.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/RFMapping.py` & `DynamicRoutingTask-0.1.96/RFMapping.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/SamStimGui/SamStimGui.py` & `DynamicRoutingTask-0.1.96/SamStimGui/SamStimGui.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/TaskControl.py` & `DynamicRoutingTask-0.1.96/TaskControl.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/TaskUtils.py` & `DynamicRoutingTask-0.1.96/TaskUtils.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/camstimControl.py` & `DynamicRoutingTask-0.1.96/camstimControl.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/pyproject.toml` & `DynamicRoutingTask-0.1.96/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "DynamicRoutingTask"
-version = "0.1.95"
+version = "0.1.96"
 dependencies = [
     "h5py",
     "numpy",
     "pandas",
     "scipy",
     "matplotlib",
 ]
```

### Comparing `DynamicRoutingTask-0.1.95/runTask.py` & `DynamicRoutingTask-0.1.96/runTask.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.95/startTask.py` & `DynamicRoutingTask-0.1.96/startTask.py`

 * *Files identical despite different names*

