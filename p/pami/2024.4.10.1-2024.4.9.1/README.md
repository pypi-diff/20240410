# Comparing `tmp/pami-2024.4.10.1.tar.gz` & `tmp/pami-2024.4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pami-2024.4.10.1.tar", last modified: Wed Apr 10 09:16:05 2024, max compression
+gzip compressed data, was "pami-2024.4.9.1.tar", last modified: Tue Apr  9 02:13:28 2024, max compression
```

## Comparing `pami-2024.4.10.1.tar` & `pami-2024.4.9.1.tar`

### file list

```diff
@@ -1,505 +1,505 @@
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.121743 pami-2024.4.10.1/
--rw-r--r--   0 vanithak   (502) staff       (20)    35149 2024-03-12 04:33:29.000000 pami-2024.4.10.1/LICENSE
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.541239 pami-2024.4.10.1/PAMI/
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.546302 pami-2024.4.10.1/PAMI/AssociationRules/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/AssociationRules/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.553180 pami-2024.4.10.1/PAMI/AssociationRules/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    14314 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/AssociationRules/basic/ARWithConfidence.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14661 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/AssociationRules/basic/ARWithLeverage.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14622 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/AssociationRules/basic/ARWithLift.py
--rw-r--r--   0 vanithak   (502) staff       (20)    20378 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/AssociationRules/basic/RuleMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/AssociationRules/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6594 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/AssociationRules/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)      139 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.554058 pami-2024.4.10.1/PAMI/correlatedPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/correlatedPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.560713 pami-2024.4.10.1/PAMI/correlatedPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    27142 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/correlatedPattern/basic/CoMine.py
--rw-r--r--   0 vanithak   (502) staff       (20)    29081 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/correlatedPattern/basic/CoMinePlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/correlatedPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6208 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/correlatedPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.561665 pami-2024.4.10.1/PAMI/coveragePattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/coveragePattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.565540 pami-2024.4.10.1/PAMI/coveragePattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    15616 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/coveragePattern/basic/CMine.py
--rw-r--r--   0 vanithak   (502) staff       (20)    18923 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/coveragePattern/basic/CPPG.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/coveragePattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7155 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/coveragePattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.571201 pami-2024.4.10.1/PAMI/extras/
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.579329 pami-2024.4.10.1/PAMI/extras/DF2DB/
--rw-r--r--   0 vanithak   (502) staff       (20)     4360 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/DF2DB/DF2DB.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4287 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/DF2DB/DF2DBPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)    10331 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/DF2DB/DenseFormatDF.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5413 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/DF2DB/SparseFormatDF.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/DF2DB/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3103 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/DF2DB/createTDB.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6948 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/DF2DB/denseDF2DBPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)    11940 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/DF2DB/denseDF2DB_dump.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5336 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.582062 pami-2024.4.10.1/PAMI/extras/calculateMISValues/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/calculateMISValues/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6468 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/extras/calculateMISValues/usingBeta.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6499 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/extras/calculateMISValues/usingSD.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7350 2024-04-10 08:52:08.000000 pami-2024.4.10.1/PAMI/extras/convertMultiTSIntoFuzzy.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.592381 pami-2024.4.10.1/PAMI/extras/dbStats/
--rw-r--r--   0 vanithak   (502) staff       (20)    14951 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/extras/dbStats/FuzzyDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    13796 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/extras/dbStats/MultipleTimeSeriesFuzzyDatabaseStats.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16034 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/dbStats/SequentialDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16883 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/extras/dbStats/TemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12839 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/extras/dbStats/TransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15120 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/extras/dbStats/UncertainTemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    11953 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/extras/dbStats/UncertainTransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12679 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/dbStats/UtilityDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/dbStats/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.605188 pami-2024.4.10.1/PAMI/extras/fuzzyTransformation/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/fuzzyTransformation/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5238 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/fuzzyTransformation/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)     8594 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
--rw-r--r--   0 vanithak   (502) staff       (20)     8792 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzy.py
--rw-r--r--   0 vanithak   (502) staff       (20)     8313 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.609547 pami-2024.4.10.1/PAMI/extras/generateDatabase/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/generateDatabase/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5685 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     9558 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5971 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5157 2024-04-10 08:52:08.000000 pami-2024.4.10.1/PAMI/extras/generateLatexGraphFile.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.617943 pami-2024.4.10.1/PAMI/extras/graph/
--rw-r--r--   0 vanithak   (502) staff       (20)     3223 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/graph/DF2Fig.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3577 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/graph/DF2Tex.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/graph/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2750 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/graph/plotLineGraphFromDictionary.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3599 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4465 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/graph/visualizeFuzzyPatterns.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4240 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/graph/visualizePatterns.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.619034 pami-2024.4.10.1/PAMI/extras/image2Database/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/image2Database/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.620944 pami-2024.4.10.1/PAMI/extras/imageProcessing/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/imageProcessing/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6488 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/imageProcessing/imagery2Databases.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.624379 pami-2024.4.10.1/PAMI/extras/messaging/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/messaging/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)      533 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/messaging/discord.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1575 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/messaging/gmail.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.629247 pami-2024.4.10.1/PAMI/extras/neighbours/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/neighbours/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4789 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/neighbours/findNeighborsUsingEuclideanDistanceforPointInfo.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4415 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4310 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5013 2024-04-10 08:52:08.000000 pami-2024.4.10.1/PAMI/extras/plotPointOnMap.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5183 2024-04-10 08:52:08.000000 pami-2024.4.10.1/PAMI/extras/plotPointOnMap_dump.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.630745 pami-2024.4.10.1/PAMI/extras/sampleDatasets/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/sampleDatasets/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4024 2024-04-10 08:52:08.000000 pami-2024.4.10.1/PAMI/extras/scatterPlotSpatialPoints.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.639136 pami-2024.4.10.1/PAMI/extras/stats/
--rw-r--r--   0 vanithak   (502) staff       (20)    12724 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/stats/TransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/stats/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4144 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/stats/graphDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15998 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/stats/sequentialDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16926 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/stats/temporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12692 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/stats/utilityDatabase.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.678081 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/
--rw-r--r--   0 vanithak   (502) staff       (20)     8471 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/TemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5543 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/TransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2325 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2254 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTransactions.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2539 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialUncertainTransaction.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1880 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/createSyntheticTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1843 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/createSyntheticTransactions.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2117 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2066 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTransactions.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2262 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/createSyntheticUtility.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/fuzzyDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1121 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/generateTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1111 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/generateTransactional.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1625 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/generateUncertainTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1610 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/generateUncertainTransactional.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3613 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/generateUtilityTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3603 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/generateUtilityTransactional.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/georeferencedTemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/georeferencedTransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4324 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/syntheticUtilityDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3283 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/temporalDatabaseGen.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4842 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/utilityDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3240 2024-04-10 08:52:08.000000 pami-2024.4.10.1/PAMI/extras/topKPatterns.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2322 2024-04-10 08:52:08.000000 pami-2024.4.10.1/PAMI/extras/uncertaindb_convert.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.680101 pami-2024.4.10.1/PAMI/extras/visualize/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/extras/visualize/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1897 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/extras/visualize/graphs.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.681948 pami-2024.4.10.1/PAMI/faultTolerantFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/faultTolerantFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.691122 pami-2024.4.10.1/PAMI/faultTolerantFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    15253 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    24431 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/faultTolerantFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6856 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.693222 pami-2024.4.10.1/PAMI/frequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.704357 pami-2024.4.10.1/PAMI/frequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    15220 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/basic/Apriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14362 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/basic/ECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14885 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/basic/ECLATDiffset.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15362 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/basic/ECLATbitset.py
--rw-r--r--   0 vanithak   (502) staff       (20)    22703 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/basic/FPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7867 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.709788 pami-2024.4.10.1/PAMI/frequentPattern/closed/
--rw-r--r--   0 vanithak   (502) staff       (20)    22294 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/closed/CHARM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/closed/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6580 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/closed/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.725306 pami-2024.4.10.1/PAMI/frequentPattern/cuda/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/cuda/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5980 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/cuda/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15188 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/cuda/cuApriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16228 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/cuda/cuAprioriBit.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14636 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/cuda/cuEclat.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16604 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/cuda/cuEclatBit.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16419 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    21681 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15055 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.729909 pami-2024.4.10.1/PAMI/frequentPattern/maximal/
--rw-r--r--   0 vanithak   (502) staff       (20)    27531 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/maximal/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6561 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/maximal/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.738053 pami-2024.4.10.1/PAMI/frequentPattern/pyspark/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/pyspark/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5573 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/pyspark/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16543 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/pyspark/parallelApriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14856 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/pyspark/parallelECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19026 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.743591 pami-2024.4.10.1/PAMI/frequentPattern/topk/
--rw-r--r--   0 vanithak   (502) staff       (20)    16687 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/topk/FAE.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/topk/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4575 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/frequentPattern/topk/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.744776 pami-2024.4.10.1/PAMI/fuzzyCorrelatedPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyCorrelatedPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.757531 pami-2024.4.10.1/PAMI/fuzzyCorrelatedPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    32988 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6645 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.759047 pami-2024.4.10.1/PAMI/fuzzyFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.765581 pami-2024.4.10.1/PAMI/fuzzyFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    25855 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    32901 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6428 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.766867 pami-2024.4.10.1/PAMI/fuzzyGeoreferencedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.772688 pami-2024.4.10.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    29496 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    32795 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6724 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.774615 pami-2024.4.10.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.780280 pami-2024.4.10.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    33628 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    39030 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6618 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.781831 pami-2024.4.10.1/PAMI/fuzzyPartialPeriodicPatterns/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyPartialPeriodicPatterns/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.785819 pami-2024.4.10.1/PAMI/fuzzyPartialPeriodicPatterns/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    25016 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/fuzzyPartialPeriodicPatterns/basic/F3PMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyPartialPeriodicPatterns/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6463 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyPartialPeriodicPatterns/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.786937 pami-2024.4.10.1/PAMI/fuzzyPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.793382 pami-2024.4.10.1/PAMI/fuzzyPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    29275 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    32773 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6678 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.794473 pami-2024.4.10.1/PAMI/geoReferencedPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.798478 pami-2024.4.10.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    23633 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6782 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.799661 pami-2024.4.10.1/PAMI/georeferencedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/georeferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.805269 pami-2024.4.10.1/PAMI/georeferencedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    23719 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    22366 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/georeferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6689 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/georeferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.807775 pami-2024.4.10.1/PAMI/georeferencedFrequentSequencePattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/georeferencedFrequentSequencePattern/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6690 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/georeferencedFrequentSequencePattern/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.809136 pami-2024.4.10.1/PAMI/georeferencedPartialPeriodicPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/georeferencedPartialPeriodicPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.812241 pami-2024.4.10.1/PAMI/georeferencedPartialPeriodicPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    23257 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6178 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.813411 pami-2024.4.10.1/PAMI/highUtilityFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilityFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.817018 pami-2024.4.10.1/PAMI/highUtilityFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    41228 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilityFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6179 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilityFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.819103 pami-2024.4.10.1/PAMI/highUtilityGeoreferencedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.824081 pami-2024.4.10.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    46718 2024-04-09 02:02:27.000000 pami-2024.4.10.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6307 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.825502 pami-2024.4.10.1/PAMI/highUtilityPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilityPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.837093 pami-2024.4.10.1/PAMI/highUtilityPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    37128 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/highUtilityPattern/basic/EFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)    30770 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/highUtilityPattern/basic/HMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    32709 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/highUtilityPattern/basic/UPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilityPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5166 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilityPattern/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    20285 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/highUtilityPattern/basic/efimParallel.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.841267 pami-2024.4.10.1/PAMI/highUtilityPattern/parallel/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilityPattern/parallel/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5166 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilityPattern/parallel/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    18207 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/highUtilityPattern/parallel/efimparallel.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.847860 pami-2024.4.10.1/PAMI/highUtilityPatternsInStreams/
--rw-r--r--   0 vanithak   (502) staff       (20)    32873 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/highUtilityPatternsInStreams/HUPMS.py
--rw-r--r--   0 vanithak   (502) staff       (20)    35784 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilityPatternsInStreams/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5193 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilityPatternsInStreams/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.852396 pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6716 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.858693 pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    35564 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)    40140 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5934 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.862980 pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/topk/
--rw-r--r--   0 vanithak   (502) staff       (20)    40254 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/topk/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6618 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/topk/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.864286 pami-2024.4.10.1/PAMI/localPeriodicPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/localPeriodicPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.871003 pami-2024.4.10.1/PAMI/localPeriodicPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    36343 2024-04-10 08:52:08.000000 pami-2024.4.10.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    25563 2024-04-10 08:52:08.000000 pami-2024.4.10.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    24596 2024-04-10 08:52:08.000000 pami-2024.4.10.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/localPeriodicPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     8385 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/localPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.874305 pami-2024.4.10.1/PAMI/multipleMinimumSupportBasedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.879361 pami-2024.4.10.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    25470 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    23153 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5921 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.880796 pami-2024.4.10.1/PAMI/partialPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.886258 pami-2024.4.10.1/PAMI/partialPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    28279 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    22083 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5398 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.887892 pami-2024.4.10.1/PAMI/partialPeriodicPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.898632 pami-2024.4.10.1/PAMI/partialPeriodicPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    26417 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4329 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/basic/Gabstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26878 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    20736 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5520 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.902552 pami-2024.4.10.1/PAMI/partialPeriodicPattern/closed/
--rw-r--r--   0 vanithak   (502) staff       (20)    24133 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/closed/PPPClose.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/closed/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5605 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/closed/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.906790 pami-2024.4.10.1/PAMI/partialPeriodicPattern/maximal/
--rw-r--r--   0 vanithak   (502) staff       (20)    29141 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/maximal/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4278 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/maximal/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.910482 pami-2024.4.10.1/PAMI/partialPeriodicPattern/pyspark/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/pyspark/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5765 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/pyspark/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    30910 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.917349 pami-2024.4.10.1/PAMI/partialPeriodicPattern/topk/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/topk/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6441 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/topk/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    20928 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.921871 pami-2024.4.10.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/
--rw-r--r--   0 vanithak   (502) staff       (20)    28158 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5556 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.923027 pami-2024.4.10.1/PAMI/periodicCorrelatedPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicCorrelatedPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.926535 pami-2024.4.10.1/PAMI/periodicCorrelatedPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    27514 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6640 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.928005 pami-2024.4.10.1/PAMI/periodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.954865 pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    17905 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28583 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26383 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)    18106 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/PFPMC.py
--rw-r--r--   0 vanithak   (502) staff       (20)    36300 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      726 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6545 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26643 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/parallelPFPGrowth.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.960212 pami-2024.4.10.1/PAMI/periodicFrequentPattern/closed/
--rw-r--r--   0 vanithak   (502) staff       (20)    24312 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/closed/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6539 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/closed/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.965131 pami-2024.4.10.1/PAMI/periodicFrequentPattern/cuda/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/cuda/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6568 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/cuda/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    23867 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    18982 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.969174 pami-2024.4.10.1/PAMI/periodicFrequentPattern/maximal/
--rw-r--r--   0 vanithak   (502) staff       (20)    31832 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/maximal/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7869 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/maximal/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.972348 pami-2024.4.10.1/PAMI/periodicFrequentPattern/pyspark/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/pyspark/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5219 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/pyspark/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26749 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.974642 pami-2024.4.10.1/PAMI/periodicFrequentPattern/topk/
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.979719 pami-2024.4.10.1/PAMI/periodicFrequentPattern/topk/TopkPFP/
--rw-r--r--   0 vanithak   (502) staff       (20)    19951 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6862 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/topk/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.983260 pami-2024.4.10.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4589 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    17514 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.984725 pami-2024.4.10.1/PAMI/recurringPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/recurringPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.987949 pami-2024.4.10.1/PAMI/recurringPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    29135 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/recurringPattern/basic/RPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/recurringPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6637 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/recurringPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.989477 pami-2024.4.10.1/PAMI/relativeFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/relativeFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.994063 pami-2024.4.10.1/PAMI/relativeFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    30349 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/relativeFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4261 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/relativeFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.995103 pami-2024.4.10.1/PAMI/relativeHighUtilityPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/relativeHighUtilityPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.998637 pami-2024.4.10.1/PAMI/relativeHighUtilityPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    35406 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/relativeHighUtilityPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6052 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/relativeHighUtilityPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:04.999662 pami-2024.4.10.1/PAMI/sequence/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/sequence/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.000277 pami-2024.4.10.1/PAMI/sequentialPatternMining/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/sequentialPatternMining/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.005946 pami-2024.4.10.1/PAMI/sequentialPatternMining/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    42265 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/sequentialPatternMining/basic/SPADE.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19986 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/sequentialPatternMining/basic/SPAM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/sequentialPatternMining/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6569 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/sequentialPatternMining/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    24786 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/sequentialPatternMining/basic/prefixSpan.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.010018 pami-2024.4.10.1/PAMI/sequentialPatternMining/closed/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/sequentialPatternMining/closed/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6285 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/sequentialPatternMining/closed/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/sequentialPatternMining/closed/bide.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.010498 pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.016615 pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    19114 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26504 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    21391 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7271 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.020349 pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/topK/
--rw-r--r--   0 vanithak   (502) staff       (20)    27859 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7173 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.021725 pami-2024.4.10.1/PAMI/subgraphMining/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.034548 pami-2024.4.10.1/PAMI/subgraphMining/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1241 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2396 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/basic/dfsCode.py
--rw-r--r--   0 vanithak   (502) staff       (20)      772 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/basic/edge.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2616 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/basic/extendedEdge.py
--rw-r--r--   0 vanithak   (502) staff       (20)      670 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/basic/frequentSubgraph.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4943 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/basic/graph.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28244 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/basic/gspan.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1748 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/basic/sparseTriangularMatrix.py
--rw-r--r--   0 vanithak   (502) staff       (20)      826 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/basic/vertex.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.057604 pami-2024.4.10.1/PAMI/subgraphMining/topK/
--rw-r--r--   0 vanithak   (502) staff       (20)     1949 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/topK/DFSCode.py
--rw-r--r--   0 vanithak   (502) staff       (20)      593 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/topK/DFSThread.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/topK/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1316 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/topK/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)      772 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/topK/edge.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2613 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/topK/extendedEdge.py
--rw-r--r--   0 vanithak   (502) staff       (20)      674 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/topK/frequentSubgraph.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4295 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/topK/graph.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1486 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/topK/sparseTriangularMatrix.py
--rw-r--r--   0 vanithak   (502) staff       (20)    20979 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/topK/tkg.py
--rw-r--r--   0 vanithak   (502) staff       (20)      818 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/subgraphMining/topK/vertex.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.062465 pami-2024.4.10.1/PAMI/uncertainFaultTolerantFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)    17358 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6756 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.064055 pami-2024.4.10.1/PAMI/uncertainFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/uncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.078629 pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    28610 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26391 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19572 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/TUFP.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19454 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/TubeP.py
--rw-r--r--   0 vanithak   (502) staff       (20)    27790 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/TubeS.py
--rw-r--r--   0 vanithak   (502) staff       (20)    25664 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19522 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4945 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.079576 pami-2024.4.10.1/PAMI/uncertainGeoreferencedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.083689 pami-2024.4.10.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    30868 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4986 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.084942 pami-2024.4.10.1/PAMI/uncertainPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.091107 pami-2024.4.10.1/PAMI/uncertainPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    33395 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    33912 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6536 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.092475 pami-2024.4.10.1/PAMI/weightedFrequentNeighbourhoodPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.096765 pami-2024.4.10.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    30821 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6603 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.098458 pami-2024.4.10.1/PAMI/weightedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/weightedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.101756 pami-2024.4.10.1/PAMI/weightedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    27246 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/weightedFrequentPattern/basic/WFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/weightedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6659 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/weightedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.102839 pami-2024.4.10.1/PAMI/weightedFrequentRegularPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/weightedFrequentRegularPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.105607 pami-2024.4.10.1/PAMI/weightedFrequentRegularPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    30320 2024-04-09 02:02:26.000000 pami-2024.4.10.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/weightedFrequentRegularPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7495 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.107108 pami-2024.4.10.1/PAMI/weightedUncertainFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/weightedUncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.110936 pami-2024.4.10.1/PAMI/weightedUncertainFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    31958 2024-03-29 21:11:29.000000 pami-2024.4.10.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4771 2024-03-12 04:33:29.000000 pami-2024.4.10.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    67287 2024-04-10 09:16:05.120757 pami-2024.4.10.1/PKG-INFO
--rw-r--r--   0 vanithak   (502) staff       (20)    65842 2024-04-10 08:52:08.000000 pami-2024.4.10.1/README.md
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-10 09:16:05.116153 pami-2024.4.10.1/pami.egg-info/
--rw-r--r--   0 vanithak   (502) staff       (20)    67287 2024-04-10 09:16:04.000000 pami-2024.4.10.1/pami.egg-info/PKG-INFO
--rw-r--r--   0 vanithak   (502) staff       (20)    18058 2024-04-10 09:16:04.000000 pami-2024.4.10.1/pami.egg-info/SOURCES.txt
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-04-10 09:16:04.000000 pami-2024.4.10.1/pami.egg-info/dependency_links.txt
--rw-r--r--   0 vanithak   (502) staff       (20)      237 2024-04-10 09:16:04.000000 pami-2024.4.10.1/pami.egg-info/requires.txt
--rw-r--r--   0 vanithak   (502) staff       (20)        5 2024-04-10 09:16:04.000000 pami-2024.4.10.1/pami.egg-info/top_level.txt
--rw-r--r--   0 vanithak   (502) staff       (20)       38 2024-04-10 09:16:05.121942 pami-2024.4.10.1/setup.cfg
--rw-r--r--   0 vanithak   (502) staff       (20)     1496 2024-04-10 09:15:40.000000 pami-2024.4.10.1/setup.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.602975 pami-2024.4.9.1/
+-rw-r--r--   0 vanithak   (502) staff       (20)    35149 2024-03-12 04:33:29.000000 pami-2024.4.9.1/LICENSE
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.793712 pami-2024.4.9.1/PAMI/
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.795296 pami-2024.4.9.1/PAMI/AssociationRules/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/AssociationRules/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.809616 pami-2024.4.9.1/PAMI/AssociationRules/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    14314 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/AssociationRules/basic/ARWithConfidence.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14661 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/AssociationRules/basic/ARWithLeverage.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14622 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/AssociationRules/basic/ARWithLift.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    20378 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/AssociationRules/basic/RuleMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/AssociationRules/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6594 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/AssociationRules/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      139 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.811156 pami-2024.4.9.1/PAMI/correlatedPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/correlatedPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.817103 pami-2024.4.9.1/PAMI/correlatedPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    27142 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/correlatedPattern/basic/CoMine.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    29081 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/correlatedPattern/basic/CoMinePlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/correlatedPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6208 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/correlatedPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.818346 pami-2024.4.9.1/PAMI/coveragePattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/coveragePattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.826282 pami-2024.4.9.1/PAMI/coveragePattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    15616 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/coveragePattern/basic/CMine.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    18923 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/coveragePattern/basic/CPPG.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/coveragePattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7155 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/coveragePattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.838845 pami-2024.4.9.1/PAMI/extras/
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.853335 pami-2024.4.9.1/PAMI/extras/DF2DB/
+-rw-r--r--   0 vanithak   (502) staff       (20)     4360 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/DF2DB.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4287 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/DF2DBPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    10331 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/DenseFormatDF.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5413 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/SparseFormatDF.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3103 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/createTDB.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6948 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/denseDF2DBPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    11940 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/denseDF2DB_dump.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5336 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.858573 pami-2024.4.9.1/PAMI/extras/calculateMISValues/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/calculateMISValues/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6468 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/calculateMISValues/usingBeta.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6499 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/calculateMISValues/usingSD.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6964 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/convertMultiTSIntoFuzzy.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.876165 pami-2024.4.9.1/PAMI/extras/dbStats/
+-rw-r--r--   0 vanithak   (502) staff       (20)    14951 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/dbStats/FuzzyDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    13796 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/dbStats/MultipleTimeSeriesFuzzyDatabaseStats.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16034 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/dbStats/SequentialDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16883 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/dbStats/TemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    12839 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/dbStats/TransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    15120 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/dbStats/UncertainTemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    11953 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/dbStats/UncertainTransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    12679 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/dbStats/UtilityDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/dbStats/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.880811 pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5238 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     8594 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     8792 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzy.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     8313 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.889684 pami-2024.4.9.1/PAMI/extras/generateDatabase/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/generateDatabase/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5685 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     9558 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5971 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5156 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/generateLatexGraphFile.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.901708 pami-2024.4.9.1/PAMI/extras/graph/
+-rw-r--r--   0 vanithak   (502) staff       (20)     3223 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/graph/DF2Fig.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3577 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/graph/DF2Tex.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/graph/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2750 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/graph/plotLineGraphFromDictionary.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3599 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4465 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/graph/visualizeFuzzyPatterns.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4240 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/graph/visualizePatterns.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.904228 pami-2024.4.9.1/PAMI/extras/image2Database/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/image2Database/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.906815 pami-2024.4.9.1/PAMI/extras/imageProcessing/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/imageProcessing/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6488 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/imageProcessing/imagery2Databases.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.911056 pami-2024.4.9.1/PAMI/extras/messaging/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/messaging/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      533 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/messaging/discord.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1575 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/messaging/gmail.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.917378 pami-2024.4.9.1/PAMI/extras/neighbours/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/neighbours/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4789 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/neighbours/findNeighborsUsingEuclideanDistanceforPointInfo.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4415 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4310 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5011 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/plotPointOnMap.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5182 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/plotPointOnMap_dump.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.922472 pami-2024.4.9.1/PAMI/extras/sampleDatasets/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/sampleDatasets/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4023 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/scatterPlotSpatialPoints.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.932869 pami-2024.4.9.1/PAMI/extras/stats/
+-rw-r--r--   0 vanithak   (502) staff       (20)    12724 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/stats/TransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/stats/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4144 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/stats/graphDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    15998 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/stats/sequentialDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16926 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/stats/temporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    12692 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/stats/utilityDatabase.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.964837 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/
+-rw-r--r--   0 vanithak   (502) staff       (20)     8471 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/TemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5543 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/TransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2325 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2254 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTransactions.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2539 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialUncertainTransaction.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1880 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1843 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticTransactions.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2117 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2066 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTransactions.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2262 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticUtility.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/fuzzyDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1121 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1111 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateTransactional.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1625 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateUncertainTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1610 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateUncertainTransactional.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3613 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateUtilityTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3603 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateUtilityTransactional.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/georeferencedTemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/georeferencedTransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4324 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/syntheticUtilityDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3283 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/temporalDatabaseGen.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4842 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/utilityDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3238 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/topKPatterns.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2321 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/uncertaindb_convert.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.969666 pami-2024.4.9.1/PAMI/extras/visualize/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/visualize/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1897 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/visualize/graphs.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.971091 pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.976128 pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    15253 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    24431 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6856 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.977409 pami-2024.4.9.1/PAMI/frequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.988154 pami-2024.4.9.1/PAMI/frequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    15220 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/basic/Apriori.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14362 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/basic/ECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14885 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/basic/ECLATDiffset.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    15362 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/basic/ECLATbitset.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    22703 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/basic/FPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7867 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.991640 pami-2024.4.9.1/PAMI/frequentPattern/closed/
+-rw-r--r--   0 vanithak   (502) staff       (20)    22294 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/closed/CHARM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/closed/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6580 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/closed/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.052468 pami-2024.4.9.1/PAMI/frequentPattern/cuda/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5980 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    15188 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/cuApriori.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16228 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/cuAprioriBit.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14636 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/cuEclat.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16604 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/cuEclatBit.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16419 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    21681 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    15055 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.056713 pami-2024.4.9.1/PAMI/frequentPattern/maximal/
+-rw-r--r--   0 vanithak   (502) staff       (20)    27531 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/maximal/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6561 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/maximal/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.064878 pami-2024.4.9.1/PAMI/frequentPattern/pyspark/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/pyspark/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5573 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/pyspark/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16543 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/pyspark/parallelApriori.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14856 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/pyspark/parallelECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19026 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.073549 pami-2024.4.9.1/PAMI/frequentPattern/topk/
+-rw-r--r--   0 vanithak   (502) staff       (20)    16687 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/topk/FAE.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/topk/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4575 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/topk/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.075074 pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.080427 pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    32988 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6645 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.085119 pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.092414 pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    25855 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    32901 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6428 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.094061 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.101426 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    29496 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    32795 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6724 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.103125 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.110674 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    33628 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    39030 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6618 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.114640 pami-2024.4.9.1/PAMI/fuzzyPartialPeriodicPatterns/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyPartialPeriodicPatterns/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.121669 pami-2024.4.9.1/PAMI/fuzzyPartialPeriodicPatterns/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    25016 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyPartialPeriodicPatterns/basic/F3PMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyPartialPeriodicPatterns/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6463 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyPartialPeriodicPatterns/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.122749 pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.128995 pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    29275 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    32773 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6678 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.130182 pami-2024.4.9.1/PAMI/geoReferencedPeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.138617 pami-2024.4.9.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    23633 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6782 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.139762 pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.145864 pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    23719 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    22366 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6689 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.148990 pami-2024.4.9.1/PAMI/georeferencedFrequentSequencePattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/georeferencedFrequentSequencePattern/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6690 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/georeferencedFrequentSequencePattern/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.150420 pami-2024.4.9.1/PAMI/georeferencedPartialPeriodicPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/georeferencedPartialPeriodicPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.155070 pami-2024.4.9.1/PAMI/georeferencedPartialPeriodicPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    23257 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6178 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.156998 pami-2024.4.9.1/PAMI/highUtilityFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.160629 pami-2024.4.9.1/PAMI/highUtilityFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    41228 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6179 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.162526 pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.169244 pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    46718 2024-04-09 02:02:27.000000 pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6307 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.170240 pami-2024.4.9.1/PAMI/highUtilityPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.178668 pami-2024.4.9.1/PAMI/highUtilityPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    37128 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/basic/EFIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    30770 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/basic/HMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    32709 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/basic/UPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5166 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    20285 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/basic/efimParallel.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.185414 pami-2024.4.9.1/PAMI/highUtilityPattern/parallel/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/parallel/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5166 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/parallel/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    18207 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/parallel/efimparallel.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.191526 pami-2024.4.9.1/PAMI/highUtilityPatternsInStreams/
+-rw-r--r--   0 vanithak   (502) staff       (20)    32873 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/highUtilityPatternsInStreams/HUPMS.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    35784 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityPatternsInStreams/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5193 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityPatternsInStreams/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.194856 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6716 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.201955 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    35564 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    40140 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5934 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.205999 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/topk/
+-rw-r--r--   0 vanithak   (502) staff       (20)    40254 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/topk/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6618 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/topk/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.207268 pami-2024.4.9.1/PAMI/localPeriodicPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/localPeriodicPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.214488 pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    34480 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    23965 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    22949 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     8385 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.217320 pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.222491 pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    25470 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    23153 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5921 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.224344 pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.234442 pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    28279 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    22083 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5398 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.235758 pami-2024.4.9.1/PAMI/partialPeriodicPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.251077 pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    26417 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4329 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/Gabstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26878 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    20736 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5520 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.257160 pami-2024.4.9.1/PAMI/partialPeriodicPattern/closed/
+-rw-r--r--   0 vanithak   (502) staff       (20)    24133 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/closed/PPPClose.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/closed/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5605 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/closed/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.274878 pami-2024.4.9.1/PAMI/partialPeriodicPattern/maximal/
+-rw-r--r--   0 vanithak   (502) staff       (20)    29141 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/maximal/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4278 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/maximal/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.286087 pami-2024.4.9.1/PAMI/partialPeriodicPattern/pyspark/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/pyspark/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5765 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/pyspark/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    30910 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.293743 pami-2024.4.9.1/PAMI/partialPeriodicPattern/topk/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/topk/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6441 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/topk/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    20928 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.303465 pami-2024.4.9.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/
+-rw-r--r--   0 vanithak   (502) staff       (20)    28158 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5556 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.309577 pami-2024.4.9.1/PAMI/periodicCorrelatedPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicCorrelatedPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.319198 pami-2024.4.9.1/PAMI/periodicCorrelatedPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    27514 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6640 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.320539 pami-2024.4.9.1/PAMI/periodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.340954 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    17905 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    28583 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26383 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    18106 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PFPMC.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    36300 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      726 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6545 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26643 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/parallelPFPGrowth.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.347343 pami-2024.4.9.1/PAMI/periodicFrequentPattern/closed/
+-rw-r--r--   0 vanithak   (502) staff       (20)    24312 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/closed/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6539 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/closed/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.356329 pami-2024.4.9.1/PAMI/periodicFrequentPattern/cuda/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/cuda/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6568 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/cuda/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    23867 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    18982 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.363446 pami-2024.4.9.1/PAMI/periodicFrequentPattern/maximal/
+-rw-r--r--   0 vanithak   (502) staff       (20)    31832 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/maximal/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7869 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/maximal/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.373650 pami-2024.4.9.1/PAMI/periodicFrequentPattern/pyspark/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/pyspark/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5219 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/pyspark/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26749 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.376040 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.383726 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/TopkPFP/
+-rw-r--r--   0 vanithak   (502) staff       (20)    19951 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6862 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.387608 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4589 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    17514 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.389862 pami-2024.4.9.1/PAMI/recurringPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/recurringPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.394287 pami-2024.4.9.1/PAMI/recurringPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    29135 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/recurringPattern/basic/RPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/recurringPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6637 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/recurringPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.396535 pami-2024.4.9.1/PAMI/relativeFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/relativeFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.403016 pami-2024.4.9.1/PAMI/relativeFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    30349 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/relativeFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4261 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/relativeFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.404650 pami-2024.4.9.1/PAMI/relativeHighUtilityPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/relativeHighUtilityPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.407969 pami-2024.4.9.1/PAMI/relativeHighUtilityPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    35406 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/relativeHighUtilityPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6052 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/relativeHighUtilityPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.410534 pami-2024.4.9.1/PAMI/sequence/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/sequence/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.411261 pami-2024.4.9.1/PAMI/sequentialPatternMining/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.421832 pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    42265 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/SPADE.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19986 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/SPAM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6569 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    24786 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/prefixSpan.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.426003 pami-2024.4.9.1/PAMI/sequentialPatternMining/closed/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/closed/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6285 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/closed/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/closed/bide.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.427496 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.436338 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    19114 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26504 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    21391 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7271 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.440665 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/topK/
+-rw-r--r--   0 vanithak   (502) staff       (20)    27859 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7173 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.441985 pami-2024.4.9.1/PAMI/subgraphMining/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.456287 pami-2024.4.9.1/PAMI/subgraphMining/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1241 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2396 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/dfsCode.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      772 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/edge.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2616 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/extendedEdge.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      670 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/frequentSubgraph.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4943 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/graph.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    28244 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/gspan.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1748 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/sparseTriangularMatrix.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      826 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/vertex.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.478210 pami-2024.4.9.1/PAMI/subgraphMining/topK/
+-rw-r--r--   0 vanithak   (502) staff       (20)     1949 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/DFSCode.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      593 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/DFSThread.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1316 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      772 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/edge.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2613 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/extendedEdge.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      674 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/frequentSubgraph.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4295 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/graph.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1486 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/sparseTriangularMatrix.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    20979 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/tkg.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      818 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/vertex.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.482255 pami-2024.4.9.1/PAMI/uncertainFaultTolerantFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)    17358 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6756 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.483938 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.506622 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    28610 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26391 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19572 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/TUFP.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19454 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/TubeP.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    27790 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/TubeS.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    25664 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19522 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4945 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.508127 pami-2024.4.9.1/PAMI/uncertainGeoreferencedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.520288 pami-2024.4.9.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    30868 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4986 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.524799 pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.537346 pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    33395 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    33912 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6536 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.538277 pami-2024.4.9.1/PAMI/weightedFrequentNeighbourhoodPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.546173 pami-2024.4.9.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    30821 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6603 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.549586 pami-2024.4.9.1/PAMI/weightedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.558446 pami-2024.4.9.1/PAMI/weightedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    27246 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentPattern/basic/WFIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6659 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.563418 pami-2024.4.9.1/PAMI/weightedFrequentRegularPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentRegularPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.574205 pami-2024.4.9.1/PAMI/weightedFrequentRegularPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    30320 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentRegularPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7495 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.575583 pami-2024.4.9.1/PAMI/weightedUncertainFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedUncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.579690 pami-2024.4.9.1/PAMI/weightedUncertainFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    31958 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4771 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    67204 2024-04-09 02:13:28.599349 pami-2024.4.9.1/PKG-INFO
+-rw-r--r--   0 vanithak   (502) staff       (20)    65760 2024-03-29 21:11:29.000000 pami-2024.4.9.1/README.md
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.589956 pami-2024.4.9.1/pami.egg-info/
+-rw-r--r--   0 vanithak   (502) staff       (20)    67204 2024-04-09 02:13:27.000000 pami-2024.4.9.1/pami.egg-info/PKG-INFO
+-rw-r--r--   0 vanithak   (502) staff       (20)    18058 2024-04-09 02:13:27.000000 pami-2024.4.9.1/pami.egg-info/SOURCES.txt
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-04-09 02:13:27.000000 pami-2024.4.9.1/pami.egg-info/dependency_links.txt
+-rw-r--r--   0 vanithak   (502) staff       (20)      237 2024-04-09 02:13:27.000000 pami-2024.4.9.1/pami.egg-info/requires.txt
+-rw-r--r--   0 vanithak   (502) staff       (20)        5 2024-04-09 02:13:27.000000 pami-2024.4.9.1/pami.egg-info/top_level.txt
+-rw-r--r--   0 vanithak   (502) staff       (20)       38 2024-04-09 02:13:28.603191 pami-2024.4.9.1/setup.cfg
+-rw-r--r--   0 vanithak   (502) staff       (20)     1494 2024-04-09 02:13:23.000000 pami-2024.4.9.1/setup.py
```

### Comparing `pami-2024.4.10.1/LICENSE` & `pami-2024.4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/AssociationRules/basic/ARWithConfidence.py` & `pami-2024.4.9.1/PAMI/AssociationRules/basic/ARWithConfidence.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/AssociationRules/basic/ARWithLeverage.py` & `pami-2024.4.9.1/PAMI/AssociationRules/basic/ARWithLeverage.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/AssociationRules/basic/ARWithLift.py` & `pami-2024.4.9.1/PAMI/AssociationRules/basic/ARWithLift.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/AssociationRules/basic/RuleMiner.py` & `pami-2024.4.9.1/PAMI/AssociationRules/basic/RuleMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/AssociationRules/basic/abstract.py` & `pami-2024.4.9.1/PAMI/AssociationRules/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/correlatedPattern/__init__.py` & `pami-2024.4.9.1/PAMI/correlatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/correlatedPattern/basic/CoMine.py` & `pami-2024.4.9.1/PAMI/correlatedPattern/basic/CoMine.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/correlatedPattern/basic/CoMinePlus.py` & `pami-2024.4.9.1/PAMI/correlatedPattern/basic/CoMinePlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/correlatedPattern/basic/__init__.py` & `pami-2024.4.9.1/PAMI/correlatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/correlatedPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/correlatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/coveragePattern/basic/CMine.py` & `pami-2024.4.9.1/PAMI/coveragePattern/basic/CMine.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/coveragePattern/basic/CPPG.py` & `pami-2024.4.9.1/PAMI/coveragePattern/basic/CPPG.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/coveragePattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/coveragePattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/DF2DB/DF2DB.py` & `pami-2024.4.9.1/PAMI/extras/DF2DB/DF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/DF2DB/DF2DBPlus.py` & `pami-2024.4.9.1/PAMI/extras/DF2DB/DF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/DF2DB/DenseFormatDF.py` & `pami-2024.4.9.1/PAMI/extras/DF2DB/DenseFormatDF.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/DF2DB/SparseFormatDF.py` & `pami-2024.4.9.1/PAMI/extras/DF2DB/SparseFormatDF.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/DF2DB/createTDB.py` & `pami-2024.4.9.1/PAMI/extras/DF2DB/createTDB.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/DF2DB/denseDF2DBPlus.py` & `pami-2024.4.9.1/PAMI/extras/DF2DB/denseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/DF2DB/denseDF2DB_dump.py` & `pami-2024.4.9.1/PAMI/extras/DF2DB/denseDF2DB_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py` & `pami-2024.4.9.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/calculateMISValues/usingBeta.py` & `pami-2024.4.9.1/PAMI/extras/calculateMISValues/usingBeta.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/calculateMISValues/usingSD.py` & `pami-2024.4.9.1/PAMI/extras/calculateMISValues/usingSD.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/convertMultiTSIntoFuzzy.py` & `pami-2024.4.9.1/PAMI/extras/convertMultiTSIntoFuzzy.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,19 @@
 #
 #     from PAMI.extras.syntheticDataGenerator import convertMultiTSIntoFuzzy as fuz
 #
 #     obj = fuz.convertMultiTSIntoFuzzy(iFile, FuzFile)
 #
 #     obj.save()
 #
-#     obj.mine()
+#     obj.startMine()
 #
 
-
-
-
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
@@ -52,15 +49,16 @@
 
                 from PAMI.extras.syntheticDataGenerator import convertMultiTSIntoFuzzy as fuz
 
                 obj = fuz.convertMultiTSIntoFuzzy(iFile, FuzFile)
 
                 obj.save()
 
-                obj.mine()
+                obj.startMine()
+
 
     """
 
 
     def __init__(self, iFile: str,  FuzFile: str) -> None:
         #super().__init__(iFile, nFile, FuzFile, minSup, maxPer, sep)
         self._iFile = iFile
@@ -165,32 +163,22 @@
                     s = s +  item + '.' + self._LabelKeyOne[k]  + '\t'
                     ss = ss + str(round(self.list[k], 2))+ '\t'
             s2 = s1 + ':' + s + ':' + ss
             # print(s2)
             # break
             writer.write("%s\n" %s2)
 
-    @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
+
     def startMine(self) -> None:
-        """
-        Frequent pattern mining process will start from here
+        """ Frequent pattern mining process will start from here
         """
         
         self._creatingItemSets()
         self._fuzzyMembershipFunc()
         self._finalPatterns = {}
-
-    def mine(self) -> None:
-        """
-        Frequent pattern mining process will start from here
-        """
-
-        self._creatingItemSets()
-        self._fuzzyMembershipFunc()
-        self._finalPatterns = {}
         
 if __name__ == "__main__":
     convertMultipleTSIntoFuzzy(sys.argv[1], sys.argv[2])
```

### Comparing `pami-2024.4.10.1/PAMI/extras/dbStats/FuzzyDatabase.py` & `pami-2024.4.9.1/PAMI/extras/dbStats/FuzzyDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/dbStats/MultipleTimeSeriesFuzzyDatabaseStats.py` & `pami-2024.4.9.1/PAMI/extras/dbStats/MultipleTimeSeriesFuzzyDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/dbStats/SequentialDatabase.py` & `pami-2024.4.9.1/PAMI/extras/dbStats/SequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/dbStats/TemporalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/dbStats/TemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/dbStats/TransactionalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/dbStats/TransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/dbStats/UncertainTemporalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/dbStats/UncertainTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/dbStats/UncertainTransactionalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/dbStats/UncertainTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/dbStats/UtilityDatabase.py` & `pami-2024.4.9.1/PAMI/extras/dbStats/UtilityDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/fuzzyTransformation/abstract.py` & `pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py` & `pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzy.py` & `pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py` & `pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/generateLatexGraphFile.py` & `pami-2024.4.9.1/PAMI/extras/generateLatexGraphFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,16 @@
 #
 #     obj = fuz.generateLatexGraphFile(idf)
 #
 #     obj.save()
 #
 
 
-
-
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
```

### Comparing `pami-2024.4.10.1/PAMI/extras/graph/DF2Fig.py` & `pami-2024.4.9.1/PAMI/extras/graph/DF2Fig.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/graph/DF2Tex.py` & `pami-2024.4.9.1/PAMI/extras/graph/DF2Tex.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/graph/plotLineGraphFromDictionary.py` & `pami-2024.4.9.1/PAMI/extras/graph/plotLineGraphFromDictionary.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py` & `pami-2024.4.9.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/graph/visualizeFuzzyPatterns.py` & `pami-2024.4.9.1/PAMI/extras/graph/visualizeFuzzyPatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/graph/visualizePatterns.py` & `pami-2024.4.9.1/PAMI/extras/graph/visualizePatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/imageProcessing/imagery2Databases.py` & `pami-2024.4.9.1/PAMI/extras/imageProcessing/imagery2Databases.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/messaging/discord.py` & `pami-2024.4.9.1/PAMI/extras/messaging/discord.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/messaging/gmail.py` & `pami-2024.4.9.1/PAMI/extras/messaging/gmail.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/neighbours/findNeighborsUsingEuclideanDistanceforPointInfo.py` & `pami-2024.4.9.1/PAMI/extras/neighbours/findNeighborsUsingEuclideanDistanceforPointInfo.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py` & `pami-2024.4.9.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py` & `pami-2024.4.9.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/plotPointOnMap.py` & `pami-2024.4.9.1/PAMI/extras/plotPointOnMap.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 #     from PAMI.extras.syntheticDataGenerator import plotPointOnMap as plt
 #
 #     obj = plt.plotPointOnMap(" ", 10, "\t")
 #
 #     obj.save()
 #
 
-
-
-
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
```

### Comparing `pami-2024.4.10.1/PAMI/extras/plotPointOnMap_dump.py` & `pami-2024.4.9.1/PAMI/extras/plotPointOnMap_dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,17 @@
 #
 #     from PAMI.extras.syntheticDataGenerator import plotPointOnMap_dump as plt
 #
 #     obj = plt.plotPointOnMap_dump(" ", 10, "\t")
 #
 #     obj.save()
 #
-
-
-
-
+#
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
```

### Comparing `pami-2024.4.10.1/PAMI/extras/scatterPlotSpatialPoints.py` & `pami-2024.4.9.1/PAMI/extras/scatterPlotSpatialPoints.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 #   from PAMI.extras.syntheticDataGenerator import scatterPlotSpatialPoints as plt
 #
 #   obj = plt.scatterPlotSpatialPoints(iFile, "\t")
 #
 #   obj.save()
 #
 
-
-
-
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
@@ -50,14 +47,15 @@
 
                 from PAMI.extras.syntheticDataGenerator import scatterPlotSpatialPoints as plt
 
                 obj = plt.scatterPlotSpatialPoints(iFile, "\t" )
 
                 obj.save(oFile)
 
+
     """
 
     def __init__(self, iFile: str, sep: str = '\t') ->None:
 
         self._iFile = iFile
         self._sep = sep
```

### Comparing `pami-2024.4.10.1/PAMI/extras/stats/TransactionalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/stats/TransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/stats/graphDatabase.py` & `pami-2024.4.9.1/PAMI/extras/stats/graphDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/stats/sequentialDatabase.py` & `pami-2024.4.9.1/PAMI/extras/stats/sequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/stats/temporalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/stats/temporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/stats/utilityDatabase.py` & `pami-2024.4.9.1/PAMI/extras/stats/utilityDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/TemporalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/TemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/TransactionalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/TransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTemporal.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTransactions.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialUncertainTransaction.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialUncertainTransaction.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/createSyntheticTemporal.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/createSyntheticTransactions.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTemporal.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTransactions.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/createSyntheticUtility.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticUtility.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/generateTemporal.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/generateTransactional.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateTransactional.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/generateUncertainTemporal.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateUncertainTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/generateUncertainTransactional.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateUncertainTransactional.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/generateUtilityTemporal.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateUtilityTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/generateUtilityTransactional.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateUtilityTransactional.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/syntheticUtilityDatabase.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/syntheticUtilityDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/temporalDatabaseGen.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/temporalDatabaseGen.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/syntheticDataGenerator/utilityDatabase.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/utilityDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/extras/topKPatterns.py` & `pami-2024.4.9.1/PAMI/extras/topKPatterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 #     from PAMI.extras.syntheticDataGenerator import topKPatterns as tK
 #
 #     obj = tK.topKPatterns(" ", 10, "\t")
 #
 #     obj.save()
 #
 
-
-
-
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
```

### Comparing `pami-2024.4.10.1/PAMI/extras/uncertaindb_convert.py` & `pami-2024.4.9.1/PAMI/extras/uncertaindb_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,18 +7,16 @@
 #
 #     obj = un.predictedClass2Transaction(predicted_classes, 0.8)
 #
 #     obj.save()
 #
 
 
-
-
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
```

### Comparing `pami-2024.4.10.1/PAMI/extras/visualize/graphs.py` & `pami-2024.4.9.1/PAMI/extras/visualize/graphs.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py` & `pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py` & `pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/frequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/basic/Apriori.py` & `pami-2024.4.9.1/PAMI/frequentPattern/basic/Apriori.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/basic/ECLAT.py` & `pami-2024.4.9.1/PAMI/frequentPattern/basic/ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/basic/ECLATDiffset.py` & `pami-2024.4.9.1/PAMI/frequentPattern/basic/ECLATDiffset.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/basic/ECLATbitset.py` & `pami-2024.4.9.1/PAMI/frequentPattern/basic/ECLATbitset.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/basic/FPGrowth.py` & `pami-2024.4.9.1/PAMI/frequentPattern/basic/FPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/frequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/closed/CHARM.py` & `pami-2024.4.9.1/PAMI/frequentPattern/closed/CHARM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/closed/abstract.py` & `pami-2024.4.9.1/PAMI/frequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/cuda/abstract.py` & `pami-2024.4.9.1/PAMI/frequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/cuda/cuApriori.py` & `pami-2024.4.9.1/PAMI/frequentPattern/cuda/cuApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/cuda/cuAprioriBit.py` & `pami-2024.4.9.1/PAMI/frequentPattern/cuda/cuAprioriBit.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/cuda/cuEclat.py` & `pami-2024.4.9.1/PAMI/frequentPattern/cuda/cuEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/cuda/cuEclatBit.py` & `pami-2024.4.9.1/PAMI/frequentPattern/cuda/cuEclatBit.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py` & `pami-2024.4.9.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py` & `pami-2024.4.9.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py` & `pami-2024.4.9.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py` & `pami-2024.4.9.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/maximal/__init__.py` & `pami-2024.4.9.1/PAMI/frequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/maximal/abstract.py` & `pami-2024.4.9.1/PAMI/frequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/pyspark/abstract.py` & `pami-2024.4.9.1/PAMI/frequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/pyspark/parallelApriori.py` & `pami-2024.4.9.1/PAMI/frequentPattern/pyspark/parallelApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/pyspark/parallelECLAT.py` & `pami-2024.4.9.1/PAMI/frequentPattern/pyspark/parallelECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py` & `pami-2024.4.9.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/topk/FAE.py` & `pami-2024.4.9.1/PAMI/frequentPattern/topk/FAE.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/frequentPattern/topk/abstract.py` & `pami-2024.4.9.1/PAMI/frequentPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyCorrelatedPattern/__init__.py` & `pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py` & `pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py` & `pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyFrequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py` & `pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py` & `pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py` & `pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py` & `pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py` & `pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py` & `pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyPartialPeriodicPatterns/basic/F3PMiner.py` & `pami-2024.4.9.1/PAMI/fuzzyPartialPeriodicPatterns/basic/F3PMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyPartialPeriodicPatterns/basic/abstract.py` & `pami-2024.4.9.1/PAMI/fuzzyPartialPeriodicPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py` & `pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py` & `pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py` & `pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py` & `pami-2024.4.9.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/georeferencedFrequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py` & `pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py` & `pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/georeferencedFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/georeferencedFrequentSequencePattern/abstract.py` & `pami-2024.4.9.1/PAMI/georeferencedFrequentSequencePattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py` & `pami-2024.4.9.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py` & `pami-2024.4.9.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilityFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/highUtilityFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py` & `pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilityPattern/basic/EFIM.py` & `pami-2024.4.9.1/PAMI/highUtilityPattern/basic/EFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilityPattern/basic/HMiner.py` & `pami-2024.4.9.1/PAMI/highUtilityPattern/basic/HMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilityPattern/basic/UPGrowth.py` & `pami-2024.4.9.1/PAMI/highUtilityPattern/basic/UPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilityPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/highUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilityPattern/basic/efimParallel.py` & `pami-2024.4.9.1/PAMI/highUtilityPattern/basic/efimParallel.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilityPattern/parallel/abstract.py` & `pami-2024.4.9.1/PAMI/highUtilityPattern/parallel/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilityPattern/parallel/efimparallel.py` & `pami-2024.4.9.1/PAMI/highUtilityPattern/parallel/efimparallel.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilityPatternsInStreams/HUPMS.py` & `pami-2024.4.9.1/PAMI/highUtilityPatternsInStreams/HUPMS.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py` & `pami-2024.4.9.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilityPatternsInStreams/abstract.py` & `pami-2024.4.9.1/PAMI/highUtilityPatternsInStreams/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/__init__.py` & `pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/abstract.py` & `pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py` & `pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py` & `pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py` & `pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/highUtilitySpatialPattern/topk/abstract.py` & `pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py` & `pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,47 +4,45 @@
 # lengths where a pattern is continuously periodic, while the minDur (minimal duration) measure ensures that those
 # time-intervals have a minimum duration.
 #
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#             from PAMI.localPeriodicPattern.basic import LPPGrowth as alg
+#     from PAMI.localPeriodicPattern.basic import LPPGrowth as alg
 #
-#             obj = alg.LPPGrowth(iFile, maxPer, maxSoPer, minDur)
+#     obj = alg.LPPGrowth(iFile, maxPer, maxSoPer, minDur)
 #
-#             obj.mine()
+#     obj.startMine()
 #
-#             localPeriodicPatterns = obj.getPatterns()
+#     localPeriodicPatterns = obj.getPatterns()
 #
-#             print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
+#     print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
 #
-#             obj.save(oFile)
+#     obj.save(oFile)
 #
-#             Df = obj.getPatternsAsDataFrame()
+#     Df = obj.getPatternsAsDataFrame()
 #
-#             memUSS = obj.getMemoryUSS()
+#     memUSS = obj.getMemoryUSS()
 #
-#             print(f'Total memory in USS: {memUSS}')
+#     print(f'Total memory in USS: {memUSS}')
 #
-#             memRSS = obj.getMemoryRSS()
+#     memRSS = obj.getMemoryRSS()
 #
-#             print(f'Total memory in RSS: {memRSS}')
+#     print(f'Total memory in RSS: {memRSS}')
 #
-#             runtime = obj.getRuntime()
+#     runtime = obj.getRuntime()
+#
+#     print(f'Total execution time in seconds: {runtime})
 #
-#             print(f'Total execution time in seconds: {runtime})
 #
-
-
-
 
 
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
@@ -58,15 +56,14 @@
 
 """
 
 
 
 from PAMI.localPeriodicPattern.basic import abstract as _ab
 from typing import List, Dict, Tuple, Set, Union, Any, Generator
-from deprecated import deprecated
 
 class Node:
     """
     A class used to represent the node of localPeriodicPatternTree
 
     :Attributes:
 
@@ -93,22 +90,16 @@
         self.child = []
         self.nodeLink = None
         self.tidList = set()
 
     def getChild(self, item: int) -> 'Node':
         """
         This function is used to get child node from the parent node
-
-        :param item: item of the parent node
-
-        :type item: int
-
+        :param item:
         :return: if node have node of item, then return it. if node don't have return []
-
-        :rtype: Node
         """
         for child in self.child:
             if child.item == item:
                 return child
         return []
 
 
@@ -146,15 +137,14 @@
         """
         add transaction into tree
 
         :param transaction: it represents the one transaction in database
         :type transaction: list
         :param tid: represents the timestamp of transaction
         :type tid: list or int
-        :return: None
         """
         current = self.root
         for item in transaction:
             child = current.getChild(item)
             if not child:
                 newNode = Node()
                 newNode.item = item
@@ -170,30 +160,28 @@
         """
         fix node link
 
         :param item: it represents item name of newNode
         :type item: string
         :param newNode: it represents node which is added
         :type newNode: Node
-        :return: None
         """
         if item in self.nodeLinks:
             lastNode = self.nodeLinks[item]
             lastNode.nodeLink = newNode
         self.nodeLinks[item] = newNode
         if item not in self.firstNodeLink:
             self.firstNodeLink[item] = newNode
 
     def deleteNode(self, item: int) -> None:
         """
         delete the node from tree
 
         :param item: it represents the item name of node
         :type item: str
-        :return: None
         """
         deleteNode = self.firstNodeLink[item]
         parentNode = deleteNode.parent
         parentNode.child.remove(deleteNode)
         parentNode.child += deleteNode.child
         parentNode.tidList |= deleteNode.tidList
         for child in deleteNode.child:
@@ -211,15 +199,14 @@
         """
         create prefix tree by path
 
         :param path: it represents path to root from prefix node
         :type path: list
         :param tidList: it represents tid of each item
         :type tidList: list
-        :return: None
         """
         currentNode = self.root
         for item in path:
             child = currentNode.getChild(item)
             if not child:
                 newNode = Node()
                 newNode.item = item
@@ -244,17 +231,17 @@
 
     :Reference:
 
         Fournier-Viger, P., Yang, P., Kiran, R. U., Ventura, S., Luna, J. M.. (2020). Mining Local Periodic Patterns in
         a Discrete Sequence. Information Sciences, Elsevier, to appear. [ppt] DOI: 10.1016/j.ins.2020.09.044
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of local periodic pattern's
+                   Name of the Input file to mine complete set of frequent pattern's
     :param  oFile: str :
-                   Name of the output file to store complete set of local periodic patterns
+                   Name of the output file to store complete set of frequent patterns
     :param  minDur: str:
                    Minimal duration in seconds between consecutive periods of time-intervals where a pattern is continuously periodic.
     :param  maxPer: float:
                    Controls the maximum number of transactions in which any two items within a pattern can reappear.
     :param  maxSoPer: float:
                    Controls the maximum number of time periods between consecutive periods of time-intervals where a pattern is continuously periodic.
 
@@ -308,15 +295,15 @@
                 Create LPPTree of local periodic item from input data.
             patternGrowth(tree, prefix, prefixPFList)
                 Execute pattern growth algorithm. It is important function in this program.
             calculatePTL(tsList)
                 Calculate PTL from input tsList as integer list.
             calculatePTLbit(tsList)
                 Calculate PTL from input tsList as bit vector.
-            mine()
+            startMine()
                 Mining process will start from here.
             getMemoryUSS()
                 Total amount of USS memory consumed by the mining process will be retrieved from this function.
             getMemoryRSS()
                 Total amount of RSS memory consumed by the mining process will be retrieved from this function.
             getRuntime()
                 Total amount of runtime taken by the mining process will be retrieved from this function.
@@ -324,38 +311,31 @@
                 return local periodic patterns and its PTL
             save(oFile)
                 Complete set of local periodic patterns will be loaded in to an output file.
             getPatternsAsDataFrame()
                 Complete set of local periodic patterns will be loaded in to a dataframe.
 
     **Executing the code on terminal:**
-    ---------------------------------------
-
-    .. code-block:: console
-
-      Format:
+    -------------------------------------
+            Format:
+                    >>> python3 LPPMGrowth.py <inputFile> <outputFile> <maxPer> <minSoPer> <minDur>
 
-      (.venv) $ python3 LPPMGrowth.py <inputFile> <outputFile> <maxPer> <minSoPer> <minDur>
-
-      Example Usage:
-
-      (.venv) $ python3 LPPMGrowth.py sampleDB.txt patterns.txt 0.3 0.4 0.5
-
-    .. note: minDur will be considered as time interval between two consecutive periods
+            Examples:
+                    >>> python3 LPPMGrowth.py sampleDB.txt patterns.txt 0.3 0.4 0.5
 
 
     **Sample run of importing the code:**
     ----------------------------------------
     .. code-block:: python
 
             from PAMI.localPeriodicPattern.basic import LPPGrowth as alg
 
             obj = alg.LPPGrowth(iFile, maxPer, maxSoPer, minDur)
 
-            obj.mine()
+            obj.startMine()
 
             localPeriodicPatterns = obj.getPatterns()
 
             print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
 
             obj.save(oFile)
 
@@ -601,15 +581,14 @@
 
         :param tree: The root node of prefix tree.
         :type tree: Node or Tree
         :param prefix: Prefix item list.
         :type prefix: list
         :param prefixPFList: tsList of prefix patterns.
         :type prefixPFList: dict or list
-        :return: None
         """
         items = list(prefixPFList)
         if not prefix:
             items = reversed(items)
         for item in items:
             prefixCopy = prefix.copy()
             prefixCopy.append(item)
@@ -658,15 +637,14 @@
     def __calculatePTL(self, tsList: List[int]) -> set:
         """
         Calculate PTL from input tsList as integer list
 
         :param tsList: It is tsList which store time stamp as integer.
         :type tsList: list
         :return: PTL
-        :rtype: set
         """
         start = -1
         PTL = set()
         tsList = sorted(tsList)
         tsPre = tsList[0]
         soPer = ' '
         for ts in tsList[1:]:
@@ -692,15 +670,14 @@
     def __calculatePTLbit(self, tsList: List[int]) -> set:
         """
         Calculate PTL from input tsList as bit vector.
 
         :param tsList: It is tsList which store time stamp as bit vector.
         :type tsList: list
         :return: PTL
-        :rtype: set
         """
         tsList = list(bin(tsList))
         tsList = tsList[2:]
         start = -1
         currentTs = 1
         PTL = set()
         tsPre = ' '
@@ -739,31 +716,28 @@
         return PTL
 
     def __convert(self, value: Any) -> float:
         """
         to convert the type of user specified minSup value
 
         :param value: user specified minSup value
-        :type value: int or float or str
         :return: converted type
-        :rtype: float
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
             value = (len(self.__Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
                 value = (len(self.__Database) * value)
             else:
                 value = int(value)
         return value
 
-    @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
     def startMine(self) -> None:
         """
         Mining process start from here.
         """
         self._localPeriodicPatterns__startTime = _ab._time.time()
         self._localPeriodicPatterns__finalPatterns = {}
         self.__creatingItemSets()
@@ -777,68 +751,43 @@
         self._localPeriodicPatterns__endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._localPeriodicPatterns__memoryUSS = float()
         self._localPeriodicPatterns__memoryRSS = float()
         self._localPeriodicPatterns__memoryUSS = process.memory_full_info().uss
         self._localPeriodicPatterns__memoryRSS = process.memory_info().rss
 
-    def mine(self) -> None:
-        """
-        Mining process start from here.
-        """
-        self._localPeriodicPatterns__startTime = _ab._time.time()
-        self._localPeriodicPatterns__finalPatterns = {}
-        self.__creatingItemSets()
-        self._localPeriodicPatterns__maxPer = self.__convert(self._localPeriodicPatterns__maxPer)
-        self._localPeriodicPatterns__maxSoPer = self.__convert(self._localPeriodicPatterns__maxSoPer)
-        self._localPeriodicPatterns__minDur = self.__convert(self._localPeriodicPatterns__minDur)
-        self.__createTSList()
-        self.__generateLPP()
-        self.__createLPPTree()
-        self.__patternGrowth(self.__root, [], self.__items)
-        self._localPeriodicPatterns__endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
-        self._localPeriodicPatterns__memoryUSS = float()
-        self._localPeriodicPatterns__memoryRSS = float()
-        self._localPeriodicPatterns__memoryUSS = process.memory_full_info().uss
-        self._localPeriodicPatterns__memoryRSS = process.memory_info().rss
-
     def getMemoryUSS(self) -> float:
-        """
-        Total amount of USS memory consumed by the mining process will be retrieved from this function
+        """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__memoryUSS
 
     def getMemoryRSS(self) -> float:
-        """
-        Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__memoryRSS
 
     def getRuntime(self) -> float:
-        """
-        Calculating the total amount of runtime taken by the mining process
+        """Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__endTime - self._localPeriodicPatterns__startTime
 
     def getPatternsAsDataFrame(self) -> '_ab._pd.DataFrame':
-        """
-        Storing final local periodic patterns in a dataframe
+        """Storing final local periodic patterns in a dataframe
 
         :return: returning local periodic patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
@@ -852,31 +801,29 @@
 
     def save(self, outFile: str) -> None:
         """
         Complete set of local periodic patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: csv file
-        :return: None
         """
         self._localPeriodicPatterns__oFile = outFile
         writer = open(self._localPeriodicPatterns__oFile, 'w+')
         for x, y in self._localPeriodicPatterns__finalPatterns.items():
             pat = str()
             for i in x:
                 pat = pat + i + '\t'
             pat = pat + ":"
             for i in y:
                 pat = pat + str(i) + '\t'
             patternsAndPTL = pat.strip()
             writer.write("%s \n" % patternsAndPTL)
 
     def getPatterns(self) -> Dict:
-        """
-        Function to send the set of local periodic patterns after completion of the mining process
+        """ Function to send the set of local periodic patterns after completion of the mining process
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._localPeriodicPatterns__finalPatterns
 
     def printResults(self) -> None:
@@ -893,15 +840,14 @@
     _ap = str()
     if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
         if len(_ab._sys.argv) == 6:
             _ap = LPPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
             _ap = LPPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
         _ap.startMine()
-        _ap.mine()
         print("Total number of Local Periodic Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in seconds:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.4.10.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py` & `pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,46 +5,43 @@
 # time-intervals have a minimum duration.
 #
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#             from PAMI.localPeriodicPattern.basic import LPPMBreadth as alg
+#     from PAMI.localPeriodicPattern.basic import LPPMBreadth as alg
 #
-#             obj = alg.LPPMBreadth(iFile, maxPer, maxSoPer, minDur)
+#     obj = alg.LPPMBreadth(iFile, maxPer, maxSoPer, minDur)
 #
-#             obj.mine()
+#     obj.startMine()
 #
-#             localPeriodicPatterns = obj.getPatterns()
+#     localPeriodicPatterns = obj.getPatterns()
 #
-#             print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
+#     print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
 #
-#             obj.save(oFile)
+#     obj.save(oFile)
 #
-#             Df = obj.getPatternsAsDataFrame()
+#     Df = obj.getPatternsAsDataFrame()
 #
-#             memUSS = obj.getMemoryUSS()
+#     memUSS = obj.getMemoryUSS()
 #
-#             print(f'Total memory in USS: {memUSS}')
+#     print(f'Total memory in USS: {memUSS}')
 #
-#             memRSS = obj.getMemoryRSS()
+#     memRSS = obj.getMemoryRSS()
 #
-#             print(f'Total memory in RSS: {memRSS}')
+#     print(f'Total memory in RSS: {memRSS}')
 #
-#             runtime = obj.getRuntime()
+#     runtime = obj.getRuntime()
 #
-#             print(f'Total execution time in seconds: {runtime})
-#
-
-
+#     print(f'Total execution time in seconds: {runtime})
 
 
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
@@ -57,16 +54,14 @@
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 from PAMI.localPeriodicPattern.basic import abstract as _ab
 from typing import List, Dict, Tuple, Set, Union, Any, Generator
 import pandas as pd
-from deprecated import deprecated
-
 
 class LPPMBreadth(_ab._localPeriodicPatterns):
 
     """
     :Description:
 
         Local Periodic Patterns, which are patterns (sets of events) that have a periodic behavior in some non predefined
@@ -77,17 +72,17 @@
 
     :Reference:
 
         Fournier-Viger, P., Yang, P., Kiran, R. U., Ventura, S., Luna, J. M.. (2020). Mining Local Periodic Patterns in
         a Discrete Sequence. Information Sciences, Elsevier, to appear. [ppt] DOI: 10.1016/j.ins.2020.09.044
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of local periodic pattern's
+                   Name of the Input file to mine complete set of frequent pattern's
     :param  oFile: str :
-                   Name of the output file to store complete set of local periodic patterns
+                   Name of the output file to store complete set of frequent patterns
     :param  minDur: str:
                    Minimal duration in seconds between consecutive periods of time-intervals where a pattern is continuously periodic.
     :param  maxPer: float:
                    Controls the maximum number of transactions in which any two items within a pattern can reappear.
     :param  maxSoPer: float:
                    Controls the maximum number of time periods between consecutive periods of time-intervals where a pattern is continuously periodic.
 
@@ -128,15 +123,15 @@
             Create the tsList as bit vector from input data.
         generateLPP()
             Generate 1 length local periodic pattens by tsList and execute depth first search.
         calculatePTL(tsList)
             Calculate PTL from input tsList as bit vector
         LPPMBreathSearch(extensionOfP)
             Mining local periodic patterns using breadth first search.
-        mine()
+        startMine()
             Mining process will start from here.
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function.
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function.
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function.
@@ -144,37 +139,29 @@
             return local periodic patterns and its PTL
         save(oFile)
             Complete set of local periodic patterns will be loaded in to an output file.
         getPatternsAsDataFrame()
             Complete set of local periodic patterns will be loaded in to a dataframe.
 
     **Executing the code on terminal:**
-    --------------------------------------
-
-    .. code-block:: console
-
-      Format:
-
-      (.venv) $ python3 LPPBreadth.py <inputFile> <outputFile> <maxPer> <minSoPer> <minDur>
-
-      Example Usage:
-
-      (.venv) $ python3 LPPMBreadth.py sampleDB.txt patterns.txt 0.3 0.4 0.5
-
-    .. note: minDur will be considered as time interval between two consecutive periods
+    ------------------------------------
+            Format:
+                >>> python3 LPPBreadth.py <inputFile> <outputFile> <maxPer> <minSoPer> <minDur>
+            Examples:
+                >>> python3 LPPMBreadth.py sampleDB.txt patterns.txt 0.3 0.4 0.5
 
     **Sample run of importing the code:**
     -------------------------------------
     .. code-block:: python
     
             from PAMI.localPeriodicPattern.basic import LPPMBreadth as alg
 
             obj = alg.LPPMBreadth(iFile, maxPer, maxSoPer, minDur)
 
-            obj.mine()
+            obj.startMine()
 
             localPeriodicPatterns = obj.getPatterns()
 
             print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
 
             obj.save(oFile)
 
@@ -358,15 +345,14 @@
     def __calculatePTL(self, tsList: int) -> Set[Tuple[int, int]]:
         """
         calculate PTL from tsList as bit vector.
 
         :param tsList: it is one item's tsList which is used bit vector.
         :type tsList: int
         :return: it is PTL of input item.
-        :rtype: set
         """
         tsList = list(bin(tsList))
         tsList = tsList[2:]
         start = -1
         currentTs = 1
         PTL = set()
         tsPre = ' '
@@ -451,31 +437,28 @@
         return w1map
 
     def __convert(self, value: Union[int, float, str]) -> Union[int, float]:
         """
         to convert the type of user specified minSup value
 
         :param value: user specified minSup value
-        :type value: int or float or str
         :return: converted type
-        :rtype: int or float
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
             value = (len(self.__Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
                 value = (len(self.__Database) * value)
             else:
                 value = int(value)
         return value
 
-    @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
     def startMine(self) -> None:
         """
         Mining process start from here.
         """
         self._localPeriodicPatterns__startTime = _ab._time.time()
         self.__creatingItemSets()
         self._localPeriodicPatterns__maxPer = self.__convert(self._localPeriodicPatterns__maxPer)
@@ -487,66 +470,43 @@
         self._localPeriodicPatterns__endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._localPeriodicPatterns__memoryUSS = float()
         self._localPeriodicPatterns__memoryRSS = float()
         self._localPeriodicPatterns__memoryUSS = process.memory_full_info().uss
         self._localPeriodicPatterns__memoryRSS = process.memory_info().rss
 
-    def mine(self) -> None:
-        """
-        Mining process start from here.
-        """
-        self._localPeriodicPatterns__startTime = _ab._time.time()
-        self.__creatingItemSets()
-        self._localPeriodicPatterns__maxPer = self.__convert(self._localPeriodicPatterns__maxPer)
-        self._localPeriodicPatterns__maxSoPer = self.__convert(self._localPeriodicPatterns__maxSoPer)
-        self._localPeriodicPatterns__minDur = self.__convert(self._localPeriodicPatterns__minDur)
-        self._localPeriodicPatterns__finalPatterns = {}
-        self.__createTSList()
-        self.__generateLPP()
-        self._localPeriodicPatterns__endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
-        self._localPeriodicPatterns__memoryUSS = float()
-        self._localPeriodicPatterns__memoryRSS = float()
-        self._localPeriodicPatterns__memoryUSS = process.memory_full_info().uss
-        self._localPeriodicPatterns__memoryRSS = process.memory_info().rss
-
     def getMemoryUSS(self) -> float:
-        """
-        Total amount of USS memory consumed by the mining process will be retrieved from this function
+        """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__memoryUSS
 
     def getMemoryRSS(self) -> float:
-        """
-        Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__memoryRSS
 
     def getRuntime(self) -> float:
-        """
-        Calculating the total amount of runtime taken by the mining process
+        """Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__endTime - self._localPeriodicPatterns__startTime
 
     def getPatternsAsDataFrame(self) -> pd.DataFrame:
-        """
-        Storing final local periodic patterns in a dataframe
+        """Storing final local periodic patterns in a dataframe
 
         :return: returning local periodic patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
@@ -555,36 +515,33 @@
             for i in a:
                 pat = pat + i + ' '
             data.append([pat, b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'PTL'])
         return dataFrame
 
     def save(self, outFile: str) -> None:
-        """
-        Complete set of local periodic patterns will be loaded in to an output file
+        """Complete set of local periodic patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: csv file
-        :return: None
         """
         self._localPeriodicPatterns__oFile = outFile
         writer = open(self._localPeriodicPatterns__oFile, 'w+')
         for x, y in self._localPeriodicPatterns__finalPatterns.items():
             pat = str()
             for i in x:
                 pat = pat + i + '\t'
             pat = pat + ":"
             for i in y:
                 pat = pat + str(i) + '\t'
             patternsAndPTL = pat.strip()
             writer.write("%s \n" % patternsAndPTL)
 
     def getPatterns(self) -> Dict[Union[Tuple[str, ...], str], Set[Tuple[int, int]]]:
-        """
-        Function to send the set of local periodic patterns after completion of the mining process
+        """ Function to send the set of local periodic patterns after completion of the mining process
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._localPeriodicPatterns__finalPatterns
 
     def printResults(self) -> None:
@@ -601,15 +558,14 @@
     _ap = str()
     if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
         if len(_ab._sys.argv) == 6:
             _ap = LPPMBreadth(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
             _ap = LPPMBreadth(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
         _ap.startMine()
-        _ap.mine()
         print("Total number of Local Periodic Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in seconds:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.4.10.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py` & `pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,46 +4,42 @@
 # lengths where a pattern is continuously periodic, while the minDur (minimal duration) measure ensures that those
 # time-intervals have a minimum duration.
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#             from PAMI.localPeriodicPattern.basic import LPPMDepth as alg
+#     from PAMI.localPeriodicPattern.basic import LPPMDepth as alg
 #
-#             obj = alg.LPPMDepth(iFile, maxPer, maxSoPer, minDur)
+#     obj = alg.LPPMDepth(iFile, maxPer, maxSoPer, minDur)
 #
-#             obj.mine()
+#     obj.startMine()
 #
-#             localPeriodicPatterns = obj.getPatterns()
+#     localPeriodicPatterns = obj.getPatterns()
 #
-#             print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
+#     print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
 #
-#             obj.save(oFile)
+#     obj.save(oFile)
 #
-#             Df = obj.getPatternsAsDataFrame()
+#     Df = obj.getPatternsAsDataFrame()
 #
-#             memUSS = obj.getMemoryUSS()
+#     memUSS = obj.getMemoryUSS()
 #
-#             print(f'Total memory in USS: {memUSS}')
+#     print(f'Total memory in USS: {memUSS}')
 #
-#             memRSS = obj.getMemoryRSS()
+#     memRSS = obj.getMemoryRSS()
 #
-#             print(f'Total memory in RSS: {memRSS}')
+#     print(f'Total memory in RSS: {memRSS}')
 #
-#             runtime = obj.getRuntime()
+#     runtime = obj.getRuntime()
 #
-#             print(f'Total execution time in seconds: {runtime})
-#
-
-
-
+#     print(f'Total execution time in seconds: {runtime})
 
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
@@ -56,16 +52,14 @@
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 from PAMI.localPeriodicPattern.basic import abstract as _ab
 from typing import List, Dict, Tuple, Set, Union, Any, Generator
 import pandas as pd
-from deprecated import deprecated
-
 
 class LPPMDepth(_ab._localPeriodicPatterns):
 
     """
     :Description:
 
         Local Periodic Patterns, which are patterns (sets of events) that have a periodic behavior in some non predefined
@@ -76,17 +70,17 @@
 
     :Reference:
 
         Fournier-Viger, P., Yang, P., Kiran, R. U., Ventura, S., Luna, J. M.. (2020). Mining Local Periodic Patterns in
         a Discrete Sequence. Information Sciences, Elsevier, to appear. [ppt] DOI: 10.1016/j.ins.2020.09.044
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of local periodic pattern's
+                   Name of the Input file to mine complete set of frequent pattern's
     :param  oFile: str :
-                   Name of the output file to store complete set of local periodic patterns
+                   Name of the output file to store complete set of frequent patterns
     :param  minDur: str:
                    Minimal duration in seconds between consecutive periods of time-intervals where a pattern is continuously periodic.
     :param  maxPer: float:
                    Controls the maximum number of transactions in which any two items within a pattern can reappear.
     :param  maxSoPer: float:
                    Controls the maximum number of time periods between consecutive periods of time-intervals where a pattern is continuously periodic.
 
@@ -142,38 +136,32 @@
             return local periodic patterns and its PTL
         save(oFile)
             Complete set of local periodic patterns will be loaded in to an output file.
         getPatternsAsDataFrame()
             Complete set of local periodic patterns will be loaded in to a dataframe.
 
     **Executing the code on terminal:**
-    --------------------------------------
-
-    .. code-block:: console
-
-      Format:
-
-      (.venv) $ python3 LPPMDepth.py <inputFile> <outputFile> <maxPer> <minSoPer> <minDur>
+    -------------------------------------
+            Format:
 
-      Example Usage:
+                >>> python3 LPPMDepth.py <inputFile> <outputFile> <maxPer> <minSoPer> <minDur> <sep>
+            Examples:
 
-      (.venv) $ python3 LPPMDepth.py sampleDB.txt patterns.txt 0.3 0.4 0.5
-
-    .. note: minDur will be considered as time interval between two consecutive periods
+                >>> python3 LPPMDepth.py sampleDB.txt patterns.txt 0.3 0.4 0.5
 
 
     **Sample run of importing the code:**
     ----------------------------------------
     .. code-block:: python
 
             from PAMI.localPeriodicPattern.basic import LPPMDepth as alg
 
             obj = alg.LPPMDepth(iFile, maxPer, maxSoPer, minDur)
 
-            obj.mine()
+            obj.startMine()
 
             localPeriodicPatterns = obj.getPatterns()
 
             print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
 
             obj.save(oFile)
 
@@ -341,20 +329,19 @@
                 self._localPeriodicPatterns__finalPatterns[item] = PTL[item]
         I = sorted(list(I))
         # I = set(I)
         self.__LPPMDepthSearch(I)
 
     def __calculatePTL(self, tsList: int) -> Set[Tuple[int, int]]:
         """
-        calculate PTL from tsList as bit vector.
+         calculate PTL from tsList as bit vector.
 
         :param tsList: it is one item's tsList which is used bit vector.
         :type tsList: int
         :return: it is PTL of input item.
-        :rtype: set
         """
         tsList = list(bin(tsList))
         tsList = tsList[2:]
         start = -1
         currentTs = 1
         PTL = set()
         tsPre = ' '
@@ -394,15 +381,14 @@
 
     def __LPPMDepthSearch(self, extensionsOfP: List[Union[Tuple[str, ...], str]]) -> None:
         """
         Mining n-length local periodic pattens from n-1-length patterns by depth first search.
 
         :param extensionsOfP: it is n-1 length patterns list.
         :type extensionsOfP: list
-        :return: None
         """
         for x in range(len(extensionsOfP)-1):
             extensionsOfPx = set()
             for y in range(x+1,len(extensionsOfP)):
                 tspxy = self.__tsList[extensionsOfP[x]] & self.__tsList[extensionsOfP[y]]
                 PTL = self.__calculatePTL(tspxy)
                 if len(PTL) > 0:
@@ -422,51 +408,30 @@
                 self.__LPPMDepthSearch(list(extensionsOfPx))
 
     def __convert(self, value: Union[int, float, str]) -> Union[int, float]:
         """
         to convert the type of user specified minSup value
 
         :param value: user specified minSup value
-        :type value: int or float or str
         :return: converted type
-        :rtype: int or float
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
             value = (len(self.__Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
                 value = (len(self.__Database) * value)
             else:
                 value = int(value)
         return value
 
-    @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
-    def startMine(self) -> None:
-        """
-        Mining process start from here. This function calls createTSlist and generateLPP.
-        """
-        self._localPeriodicPatterns__startTime = _ab._time.time()
-        self._localPeriodicPatterns__finalPatterns = {}
-        self.__creatingItemSets()
-        self._localPeriodicPatterns__maxPer = self.__convert(self._localPeriodicPatterns__maxPer)
-        self._localPeriodicPatterns__maxSoPer = self.__convert(self._localPeriodicPatterns__maxSoPer)
-        self._localPeriodicPatterns__minDur = self.__convert(self._localPeriodicPatterns__minDur)
-        self.__createTSlist()
-        self.__generateLPP()
-        self._localPeriodicPatterns__endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
-        self._localPeriodicPatterns__memoryRSS = float()
-        self._localPeriodicPatterns__memoryUSS = float()
-        self._localPeriodicPatterns__memoryUSS = process.memory_full_info().uss
-        self._localPeriodicPatterns__memoryRSS = process.memory_info().rss
 
-    def mine(self) -> None:
+    def startMine(self) -> None:
         """
         Mining process start from here. This function calls createTSlist and generateLPP.
         """
         self._localPeriodicPatterns__startTime = _ab._time.time()
         self._localPeriodicPatterns__finalPatterns = {}
         self.__creatingItemSets()
         self._localPeriodicPatterns__maxPer = self.__convert(self._localPeriodicPatterns__maxPer)
@@ -478,36 +443,33 @@
         process = _ab._psutil.Process(_ab._os.getpid())
         self._localPeriodicPatterns__memoryRSS = float()
         self._localPeriodicPatterns__memoryUSS = float()
         self._localPeriodicPatterns__memoryUSS = process.memory_full_info().uss
         self._localPeriodicPatterns__memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self) -> float:
-        """
-        Total amount of USS memory consumed by the mining process will be retrieved from this function
+        """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__memoryUSS
 
     def getMemoryRSS(self) -> float:
-        """
-        Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__memoryRSS
 
     def getRuntime(self) -> float:
-        """
-        Calculating the total amount of runtime taken by the mining process
+        """Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__endTime - self._localPeriodicPatterns__startTime
 
@@ -531,31 +493,29 @@
 
     def save(self, outFile: str) -> None:
         """
         Complete set of local periodic patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: csv file
-        :return: None
         """
         self._localPeriodicPatterns__oFile = outFile
         writer = open(self._localPeriodicPatterns__oFile, 'w+')
         for x, y in self._localPeriodicPatterns__finalPatterns.items():
             pat = str()
             for i in x:
                 pat = pat + i + '\t'
             pat = pat + ":"
             for i in y:
                 pat = pat + str(i) + '\t'
             patternsAndPTL = pat.strip()
             writer.write("%s \n" % patternsAndPTL)
 
     def getPatterns(self) -> Dict[Union[Tuple[str, ...], str], Set[Tuple[int, int]]]:
-        """
-        Function to send the set of local periodic patterns after completion of the mining process
+        """ Function to send the set of local periodic patterns after completion of the mining process
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._localPeriodicPatterns__finalPatterns
 
     def printResults(self) -> None:
@@ -572,15 +532,14 @@
     _ap = str()
     if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
         if len(_ab._sys.argv) == 6:
             _ap = LPPMDepth(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
             _ap = LPPMDepth(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
         _ap.startMine()
-        _ap.mine()
         print("Total number of Local Periodic Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in seconds:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.4.10.1/PAMI/localPeriodicPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py` & `pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py` & `pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py` & `pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py` & `pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/__init__.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/basic/Gabstract.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/Gabstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/basic/__init__.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/closed/PPPClose.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/closed/PPPClose.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/closed/abstract.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/maximal/__init__.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/maximal/abstract.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/pyspark/__init__.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/pyspark/abstract.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/topk/abstract.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py` & `pami-2024.4.9.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicCorrelatedPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/periodicCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/PFPMC.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PFPMC.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/__init__.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/basic/parallelPFPGrowth.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/parallelPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/closed/__init__.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/closed/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/closed/abstract.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/cuda/abstract.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/maximal/__init__.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/maximal/abstract.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/pyspark/abstract.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/recurringPattern/basic/RPGrowth.py` & `pami-2024.4.9.1/PAMI/recurringPattern/basic/RPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/recurringPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/recurringPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py` & `pami-2024.4.9.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/relativeFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/relativeFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py` & `pami-2024.4.9.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/relativeHighUtilityPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/relativeHighUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/sequentialPatternMining/basic/SPADE.py` & `pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/SPADE.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/sequentialPatternMining/basic/SPAM.py` & `pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/SPAM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/sequentialPatternMining/basic/abstract.py` & `pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/sequentialPatternMining/basic/prefixSpan.py` & `pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/prefixSpan.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/sequentialPatternMining/closed/abstract.py` & `pami-2024.4.9.1/PAMI/sequentialPatternMining/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py` & `pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py` & `pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py` & `pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py` & `pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py` & `pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/basic/abstract.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/basic/dfsCode.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/dfsCode.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/basic/edge.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/edge.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/basic/extendedEdge.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/extendedEdge.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/basic/frequentSubgraph.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/frequentSubgraph.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/basic/graph.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/graph.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/basic/gspan.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/gspan.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/basic/sparseTriangularMatrix.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/sparseTriangularMatrix.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/basic/vertex.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/vertex.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/topK/DFSCode.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/DFSCode.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/topK/DFSThread.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/DFSThread.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/topK/abstract.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/topK/edge.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/edge.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/topK/extendedEdge.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/extendedEdge.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/topK/frequentSubgraph.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/frequentSubgraph.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/topK/graph.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/graph.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/topK/sparseTriangularMatrix.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/sparseTriangularMatrix.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/topK/tkg.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/tkg.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/subgraphMining/topK/vertex.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/vertex.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py` & `pami-2024.4.9.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py` & `pami-2024.4.9.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainFrequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/TUFP.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/TUFP.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/TubeP.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/TubeP.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/TubeS.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/TubeS.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py` & `pami-2024.4.9.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py` & `pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py` & `pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py` & `pami-2024.4.9.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/weightedFrequentPattern/basic/WFIM.py` & `pami-2024.4.9.1/PAMI/weightedFrequentPattern/basic/WFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/weightedFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/weightedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py` & `pami-2024.4.9.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py` & `pami-2024.4.9.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/PKG-INFO` & `pami-2024.4.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2024.4.10.1
+Version: 2024.4.9.1
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayLab/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -57,17 +57,14 @@
 [![Downloads](https://static.pepy.tech/badge/pami/month)](https://pepy.tech/project/pami)
 [![Downloads](https://static.pepy.tech/badge/pami/week)](https://pepy.tech/project/pami)
 
 [Click here for more information](https://pepy.tech/project/pami)
 
 
 # Introduction
-
-***
-
 PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in a wide-spectrum of datasets across multiple computing platforms. Useful links to utilize the services of this library were provided below:
 
 
 1. Youtube tutorial https://www.youtube.com/playlist?list=PLKP768gjVJmDer6MajaLbwtfC9ULVuaCZ
 
 2. Tutorials (Notebooks) https://github.com/UdayLab/PAMI/tree/main/notebooks
    
@@ -79,63 +76,50 @@
 
 6. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
 7. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
 
 8. Report issues https://github.com/UdayLab/PAMI/issues
 
-
 # Recent Updates  
 
-***
-
 - Version 2023.07.07: New algorithms: cuApriroi, cuAprioriBit, cuEclat, cuEclatBit, gPPMiner, cuGPFMiner, FPStream, HUPMS, SHUPGrowth New codes to generate synthetic databases
 - Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
 Total number of algorithms: 83
 
-
 # Features
 
-***
-
 - ✅ Well-tested and production-ready
 - 🔋 Highly optimized to our best effort, light-weight, and energy-efficient
 - 👀 Proper code documentation
 - 🍼 Ample examples of using various algorithms at [./notebooks](https://github.com/UdayLab/PAMI/tree/main/notebooks) folder
 - 🤖 Works with AI libraries such as TensorFlow, PyTorch, and sklearn. 
 - ⚡️ Supports Cuda and PySpark 
 - 🖥️ Operating System Independence
 - 🔬 Knowledge discovery in static data and streams
 - 🐎 Snappy
 - 🐻 Ease of use
 
-
-
 # Table of Content
 
-***
-
 - [Maintenance](#Maintenance)
 - [Try your first PAMI program](#try-your-first-PAMI-program)
 - [Reading Material](#Reading-Material)
+- [Tutorials](#Tutorials)
 - [License](#License)
 - [Documentation](#Documentation)
 - [Background](#Background)
 - [Getting Help](#Getting-Help)
 - [Discussion and Development](#Discussion-and-Development)
 - [Contribution to PAMI](#Contribution-to-PAMI)
-- [Tutorials](#Tutorials)
-
 
 # Maintenance
 
-***
-
   __Installation__
   
   1. Installing basic pami package (recommended)
 
 
          pip install pami
 
@@ -177,19 +161,16 @@
        
 
   __Information__ 
 
 
         pip show pami
 
-
 # *Try your first PAMI program*
 
-***
-
 ```shell
 $ python
 ```
 
 ```python
 # first import pami 
 from PAMI.frequentPattern.basic import FPGrowth as alg
@@ -211,68 +192,20 @@
 Total No of patterns: 4540
 Runtime: 8.749667644500732
 Memory (RSS): 522911744
 Memory (USS): 475353088
 ```
 
 # Reading Material
-
-***
-
 For more examples, refer this YouTube link [YouTube](https://www.youtube.com/playlist?list=PLKP768gjVJmDer6MajaLbwtfC9ULVuaCZ)
-
-
-# License
-
-***
-
-[![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
-
-
-# Documentation
-
-***
-
-The official documentation is hosted on [PAMI](https://pami-1.readthedocs.io).
-
-
-
-# Background
-
-***
-
-The idea and motivation to develop PAMI was from [Kitsuregawa Lab](https://www.tkl.iis.u-tokyo.ac.jp/new/resources?lang=en) at the University of Tokyo. Work on ``PAMI`` started at [University of Aizu](https://u-aizu.ac.jp/en/) in 2020 and
-has been under active development since then.
-
-
-# Getting Help
-
-***
-
-For any queries, the best place to go to is github Issues [GithubIssues](https://github.com/orgs/UdayLab/discussions/categories/q-a).
-
-
-# Discussion and Development
-
+ 
 ***
 
-In our GitHub repository, the primary platform for discussing development-related matters is the university lab. We encourage our team members and contributors to utilize this platform for a wide range of discussions, including bug reports, feature requests, design decisions, and implementation details.
-
-
-# Contribution to PAMI
-
-***
-
-We invite and encourage all community members to contribute, report bugs, fix bugs, enhance documentation, propose improvements, and share their creative ideas.
-
-
 # Tutorials 
 
-***
-
 ### 1. Pattern mining in binary transactional databases
 
 #### 1.1. Frequent pattern mining: [Sample](https://udaylab.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                      | Closed                                                                                                                                                                                                                                       | Maximal                                                                                                                                                                                                                                                     | Top-k                                                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                                             |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Apriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/Apriori.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>              | CHARM <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/closed/CHARM.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | maxFP-growth  <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/maximal/MaxFPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | FAE <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/topk/FAE.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | cudaAprioriGCT | parallelApriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/pyspark/parallelApriori.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>   |
@@ -461,14 +394,16 @@
 #### 5.1. Fuzzy Frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzyFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                   |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FFI-Miner <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/fuzzyFrequentPattern/basic/FFIMiner.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
 
+
+
 #### 5.2. Fuzzy correlated pattern mining: [Sample](https://udaylab.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                       |
 |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FCP-growth <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/fuzzyCorrelatedPattern/basic/FCPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
 
@@ -566,8 +501,28 @@
 ## 11. Mining patterns from Graphs
 
 #### 11.1. Frequent sub-graph mining
 | Basic                                                                                                                                                                                                                                      | topk                                                                                                                                                                                                                                  |
 |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
  | Gspan <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/subgraphMining/basic/gspan.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | TKG <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/subgraphMining/topk/tkg.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
-[Go to Top](#table-of-content)
+# License
+
+[![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
+
+# Documentation
+The official documentation is hosted on [PAMI](https://pami-1.readthedocs.io).
+
+# Background
+The idea and motivation to develop PAMI was from [Kitsuregawa Lab](https://www.tkl.iis.u-tokyo.ac.jp/new/resources?lang=en) at the University of Tokyo. Work on ``PAMI`` started at [University of Aizu](https://u-aizu.ac.jp/en/) in 2020 and
+has been under active development since then.
+
+# Getting Help
+For any queries, the best place to go to is github Issues [GithubIssues](https://github.com/orgs/UdayLab/discussions/categories/q-a).
+
+# Discussion and Development
+In our GitHub repository, the primary platform for discussing development-related matters is the university lab. We encourage our team members and contributors to utilize this platform for a wide range of discussions, including bug reports, feature requests, design decisions, and implementation details.
+
+# Contribution to PAMI
+We invite and encourage all community members to contribute, report bugs, fix bugs, enhance documentation, propose improvements, and share their creative ideas.
+
+[Go to Top](#table-of-contents)
```

### Comparing `pami-2024.4.10.1/README.md` & `pami-2024.4.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,14 @@
 [![Downloads](https://static.pepy.tech/badge/pami/month)](https://pepy.tech/project/pami)
 [![Downloads](https://static.pepy.tech/badge/pami/week)](https://pepy.tech/project/pami)
 
 [Click here for more information](https://pepy.tech/project/pami)
 
 
 # Introduction
-
-***
-
 PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in a wide-spectrum of datasets across multiple computing platforms. Useful links to utilize the services of this library were provided below:
 
 
 1. Youtube tutorial https://www.youtube.com/playlist?list=PLKP768gjVJmDer6MajaLbwtfC9ULVuaCZ
 
 2. Tutorials (Notebooks) https://github.com/UdayLab/PAMI/tree/main/notebooks
    
@@ -34,63 +31,50 @@
 
 6. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
 7. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
 
 8. Report issues https://github.com/UdayLab/PAMI/issues
 
-
 # Recent Updates  
 
-***
-
 - Version 2023.07.07: New algorithms: cuApriroi, cuAprioriBit, cuEclat, cuEclatBit, gPPMiner, cuGPFMiner, FPStream, HUPMS, SHUPGrowth New codes to generate synthetic databases
 - Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
 Total number of algorithms: 83
 
-
 # Features
 
-***
-
 - ✅ Well-tested and production-ready
 - 🔋 Highly optimized to our best effort, light-weight, and energy-efficient
 - 👀 Proper code documentation
 - 🍼 Ample examples of using various algorithms at [./notebooks](https://github.com/UdayLab/PAMI/tree/main/notebooks) folder
 - 🤖 Works with AI libraries such as TensorFlow, PyTorch, and sklearn. 
 - ⚡️ Supports Cuda and PySpark 
 - 🖥️ Operating System Independence
 - 🔬 Knowledge discovery in static data and streams
 - 🐎 Snappy
 - 🐻 Ease of use
 
-
-
 # Table of Content
 
-***
-
 - [Maintenance](#Maintenance)
 - [Try your first PAMI program](#try-your-first-PAMI-program)
 - [Reading Material](#Reading-Material)
+- [Tutorials](#Tutorials)
 - [License](#License)
 - [Documentation](#Documentation)
 - [Background](#Background)
 - [Getting Help](#Getting-Help)
 - [Discussion and Development](#Discussion-and-Development)
 - [Contribution to PAMI](#Contribution-to-PAMI)
-- [Tutorials](#Tutorials)
-
 
 # Maintenance
 
-***
-
   __Installation__
   
   1. Installing basic pami package (recommended)
 
 
          pip install pami
 
@@ -132,19 +116,16 @@
        
 
   __Information__ 
 
 
         pip show pami
 
-
 # *Try your first PAMI program*
 
-***
-
 ```shell
 $ python
 ```
 
 ```python
 # first import pami 
 from PAMI.frequentPattern.basic import FPGrowth as alg
@@ -166,68 +147,20 @@
 Total No of patterns: 4540
 Runtime: 8.749667644500732
 Memory (RSS): 522911744
 Memory (USS): 475353088
 ```
 
 # Reading Material
-
-***
-
 For more examples, refer this YouTube link [YouTube](https://www.youtube.com/playlist?list=PLKP768gjVJmDer6MajaLbwtfC9ULVuaCZ)
-
-
-# License
-
-***
-
-[![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
-
-
-# Documentation
-
-***
-
-The official documentation is hosted on [PAMI](https://pami-1.readthedocs.io).
-
-
-
-# Background
-
-***
-
-The idea and motivation to develop PAMI was from [Kitsuregawa Lab](https://www.tkl.iis.u-tokyo.ac.jp/new/resources?lang=en) at the University of Tokyo. Work on ``PAMI`` started at [University of Aizu](https://u-aizu.ac.jp/en/) in 2020 and
-has been under active development since then.
-
-
-# Getting Help
-
-***
-
-For any queries, the best place to go to is github Issues [GithubIssues](https://github.com/orgs/UdayLab/discussions/categories/q-a).
-
-
-# Discussion and Development
-
+ 
 ***
 
-In our GitHub repository, the primary platform for discussing development-related matters is the university lab. We encourage our team members and contributors to utilize this platform for a wide range of discussions, including bug reports, feature requests, design decisions, and implementation details.
-
-
-# Contribution to PAMI
-
-***
-
-We invite and encourage all community members to contribute, report bugs, fix bugs, enhance documentation, propose improvements, and share their creative ideas.
-
-
 # Tutorials 
 
-***
-
 ### 1. Pattern mining in binary transactional databases
 
 #### 1.1. Frequent pattern mining: [Sample](https://udaylab.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                      | Closed                                                                                                                                                                                                                                       | Maximal                                                                                                                                                                                                                                                     | Top-k                                                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                                             |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Apriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/Apriori.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>              | CHARM <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/closed/CHARM.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | maxFP-growth  <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/maximal/MaxFPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | FAE <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/topk/FAE.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | cudaAprioriGCT | parallelApriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/pyspark/parallelApriori.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>   |
@@ -416,14 +349,16 @@
 #### 5.1. Fuzzy Frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzyFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                   |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FFI-Miner <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/fuzzyFrequentPattern/basic/FFIMiner.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
 
+
+
 #### 5.2. Fuzzy correlated pattern mining: [Sample](https://udaylab.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                       |
 |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FCP-growth <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/fuzzyCorrelatedPattern/basic/FCPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
 
@@ -521,8 +456,28 @@
 ## 11. Mining patterns from Graphs
 
 #### 11.1. Frequent sub-graph mining
 | Basic                                                                                                                                                                                                                                      | topk                                                                                                                                                                                                                                  |
 |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
  | Gspan <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/subgraphMining/basic/gspan.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | TKG <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/subgraphMining/topk/tkg.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
-[Go to Top](#table-of-content)
+# License
+
+[![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
+
+# Documentation
+The official documentation is hosted on [PAMI](https://pami-1.readthedocs.io).
+
+# Background
+The idea and motivation to develop PAMI was from [Kitsuregawa Lab](https://www.tkl.iis.u-tokyo.ac.jp/new/resources?lang=en) at the University of Tokyo. Work on ``PAMI`` started at [University of Aizu](https://u-aizu.ac.jp/en/) in 2020 and
+has been under active development since then.
+
+# Getting Help
+For any queries, the best place to go to is github Issues [GithubIssues](https://github.com/orgs/UdayLab/discussions/categories/q-a).
+
+# Discussion and Development
+In our GitHub repository, the primary platform for discussing development-related matters is the university lab. We encourage our team members and contributors to utilize this platform for a wide range of discussions, including bug reports, feature requests, design decisions, and implementation details.
+
+# Contribution to PAMI
+We invite and encourage all community members to contribute, report bugs, fix bugs, enhance documentation, propose improvements, and share their creative ideas.
+
+[Go to Top](#table-of-contents)
```

### Comparing `pami-2024.4.10.1/pami.egg-info/PKG-INFO` & `pami-2024.4.9.1/pami.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2024.4.10.1
+Version: 2024.4.9.1
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayLab/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -57,17 +57,14 @@
 [![Downloads](https://static.pepy.tech/badge/pami/month)](https://pepy.tech/project/pami)
 [![Downloads](https://static.pepy.tech/badge/pami/week)](https://pepy.tech/project/pami)
 
 [Click here for more information](https://pepy.tech/project/pami)
 
 
 # Introduction
-
-***
-
 PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in a wide-spectrum of datasets across multiple computing platforms. Useful links to utilize the services of this library were provided below:
 
 
 1. Youtube tutorial https://www.youtube.com/playlist?list=PLKP768gjVJmDer6MajaLbwtfC9ULVuaCZ
 
 2. Tutorials (Notebooks) https://github.com/UdayLab/PAMI/tree/main/notebooks
    
@@ -79,63 +76,50 @@
 
 6. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
 7. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
 
 8. Report issues https://github.com/UdayLab/PAMI/issues
 
-
 # Recent Updates  
 
-***
-
 - Version 2023.07.07: New algorithms: cuApriroi, cuAprioriBit, cuEclat, cuEclatBit, gPPMiner, cuGPFMiner, FPStream, HUPMS, SHUPGrowth New codes to generate synthetic databases
 - Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
 Total number of algorithms: 83
 
-
 # Features
 
-***
-
 - ✅ Well-tested and production-ready
 - 🔋 Highly optimized to our best effort, light-weight, and energy-efficient
 - 👀 Proper code documentation
 - 🍼 Ample examples of using various algorithms at [./notebooks](https://github.com/UdayLab/PAMI/tree/main/notebooks) folder
 - 🤖 Works with AI libraries such as TensorFlow, PyTorch, and sklearn. 
 - ⚡️ Supports Cuda and PySpark 
 - 🖥️ Operating System Independence
 - 🔬 Knowledge discovery in static data and streams
 - 🐎 Snappy
 - 🐻 Ease of use
 
-
-
 # Table of Content
 
-***
-
 - [Maintenance](#Maintenance)
 - [Try your first PAMI program](#try-your-first-PAMI-program)
 - [Reading Material](#Reading-Material)
+- [Tutorials](#Tutorials)
 - [License](#License)
 - [Documentation](#Documentation)
 - [Background](#Background)
 - [Getting Help](#Getting-Help)
 - [Discussion and Development](#Discussion-and-Development)
 - [Contribution to PAMI](#Contribution-to-PAMI)
-- [Tutorials](#Tutorials)
-
 
 # Maintenance
 
-***
-
   __Installation__
   
   1. Installing basic pami package (recommended)
 
 
          pip install pami
 
@@ -177,19 +161,16 @@
        
 
   __Information__ 
 
 
         pip show pami
 
-
 # *Try your first PAMI program*
 
-***
-
 ```shell
 $ python
 ```
 
 ```python
 # first import pami 
 from PAMI.frequentPattern.basic import FPGrowth as alg
@@ -211,68 +192,20 @@
 Total No of patterns: 4540
 Runtime: 8.749667644500732
 Memory (RSS): 522911744
 Memory (USS): 475353088
 ```
 
 # Reading Material
-
-***
-
 For more examples, refer this YouTube link [YouTube](https://www.youtube.com/playlist?list=PLKP768gjVJmDer6MajaLbwtfC9ULVuaCZ)
-
-
-# License
-
-***
-
-[![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
-
-
-# Documentation
-
-***
-
-The official documentation is hosted on [PAMI](https://pami-1.readthedocs.io).
-
-
-
-# Background
-
-***
-
-The idea and motivation to develop PAMI was from [Kitsuregawa Lab](https://www.tkl.iis.u-tokyo.ac.jp/new/resources?lang=en) at the University of Tokyo. Work on ``PAMI`` started at [University of Aizu](https://u-aizu.ac.jp/en/) in 2020 and
-has been under active development since then.
-
-
-# Getting Help
-
-***
-
-For any queries, the best place to go to is github Issues [GithubIssues](https://github.com/orgs/UdayLab/discussions/categories/q-a).
-
-
-# Discussion and Development
-
+ 
 ***
 
-In our GitHub repository, the primary platform for discussing development-related matters is the university lab. We encourage our team members and contributors to utilize this platform for a wide range of discussions, including bug reports, feature requests, design decisions, and implementation details.
-
-
-# Contribution to PAMI
-
-***
-
-We invite and encourage all community members to contribute, report bugs, fix bugs, enhance documentation, propose improvements, and share their creative ideas.
-
-
 # Tutorials 
 
-***
-
 ### 1. Pattern mining in binary transactional databases
 
 #### 1.1. Frequent pattern mining: [Sample](https://udaylab.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                      | Closed                                                                                                                                                                                                                                       | Maximal                                                                                                                                                                                                                                                     | Top-k                                                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                                             |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Apriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/Apriori.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>              | CHARM <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/closed/CHARM.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | maxFP-growth  <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/maximal/MaxFPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | FAE <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/topk/FAE.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | cudaAprioriGCT | parallelApriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/pyspark/parallelApriori.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>   |
@@ -461,14 +394,16 @@
 #### 5.1. Fuzzy Frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzyFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                   |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FFI-Miner <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/fuzzyFrequentPattern/basic/FFIMiner.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
 
+
+
 #### 5.2. Fuzzy correlated pattern mining: [Sample](https://udaylab.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                       |
 |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FCP-growth <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/fuzzyCorrelatedPattern/basic/FCPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
 
@@ -566,8 +501,28 @@
 ## 11. Mining patterns from Graphs
 
 #### 11.1. Frequent sub-graph mining
 | Basic                                                                                                                                                                                                                                      | topk                                                                                                                                                                                                                                  |
 |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
  | Gspan <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/subgraphMining/basic/gspan.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | TKG <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/subgraphMining/topk/tkg.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
-[Go to Top](#table-of-content)
+# License
+
+[![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
+
+# Documentation
+The official documentation is hosted on [PAMI](https://pami-1.readthedocs.io).
+
+# Background
+The idea and motivation to develop PAMI was from [Kitsuregawa Lab](https://www.tkl.iis.u-tokyo.ac.jp/new/resources?lang=en) at the University of Tokyo. Work on ``PAMI`` started at [University of Aizu](https://u-aizu.ac.jp/en/) in 2020 and
+has been under active development since then.
+
+# Getting Help
+For any queries, the best place to go to is github Issues [GithubIssues](https://github.com/orgs/UdayLab/discussions/categories/q-a).
+
+# Discussion and Development
+In our GitHub repository, the primary platform for discussing development-related matters is the university lab. We encourage our team members and contributors to utilize this platform for a wide range of discussions, including bug reports, feature requests, design decisions, and implementation details.
+
+# Contribution to PAMI
+We invite and encourage all community members to contribute, report bugs, fix bugs, enhance documentation, propose improvements, and share their creative ideas.
+
+[Go to Top](#table-of-contents)
```

### Comparing `pami-2024.4.10.1/pami.egg-info/SOURCES.txt` & `pami-2024.4.9.1/pami.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pami-2024.4.10.1/setup.py` & `pami-2024.4.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pami',
-    version='2024.4.10.1',
+    version='2024.4.9.1',
     author='Rage Uday Kiran',
     author_email='uday.rage@gmail.com',
     description='This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     url='https://github.com/udayLab/PAMI',
@@ -39,8 +39,7 @@
         'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.5',
 )
-
```

