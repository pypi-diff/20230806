# Comparing `tmp/pami-2023.8.2.1.tar.gz` & `tmp/pami-2023.8.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pami-2023.8.2.1.tar", last modified: Wed Aug  2 11:09:06 2023, max compression
+gzip compressed data, was "pami-2023.8.6.1.tar", last modified: Sun Aug  6 15:39:11 2023, max compression
```

## Comparing `pami-2023.8.2.1.tar` & `pami-2023.8.6.1.tar`

### file list

```diff
@@ -1,435 +1,439 @@
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.756582 pami-2023.8.2.1/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-08-02 11:00:06.000000 pami-2023.8.2.1/LICENSE
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.697593 pami-2023.8.2.1/PAMI/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.697800 pami-2023.8.2.1/PAMI/AssociationRules/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:18.000000 pami-2023.8.2.1/PAMI/AssociationRules/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.698797 pami-2023.8.2.1/PAMI/AssociationRules/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13175 2023-08-02 11:00:35.000000 pami-2023.8.2.1/PAMI/AssociationRules/basic/ARWithConfidence.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12870 2023-08-02 11:00:35.000000 pami-2023.8.2.1/PAMI/AssociationRules/basic/ARWithLeverage.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13078 2023-08-02 11:00:35.000000 pami-2023.8.2.1/PAMI/AssociationRules/basic/ARWithLift.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12384 2023-08-02 11:00:35.000000 pami-2023.8.2.1/PAMI/AssociationRules/basic/RuleMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:35.000000 pami-2023.8.2.1/PAMI/AssociationRules/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6455 2023-08-02 11:00:35.000000 pami-2023.8.2.1/PAMI/AssociationRules/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2023-08-02 11:00:11.000000 pami-2023.8.2.1/PAMI/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.698957 pami-2023.8.2.1/PAMI/correlatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:29.000000 pami-2023.8.2.1/PAMI/correlatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.699709 pami-2023.8.2.1/PAMI/correlatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24834 2023-08-02 11:00:53.000000 pami-2023.8.2.1/PAMI/correlatedPattern/basic/CoMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26312 2023-08-02 11:00:53.000000 pami-2023.8.2.1/PAMI/correlatedPattern/basic/CoMinePlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:53.000000 pami-2023.8.2.1/PAMI/correlatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6065 2023-08-02 11:00:53.000000 pami-2023.8.2.1/PAMI/correlatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.700070 pami-2023.8.2.1/PAMI/coveragePattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:33.000000 pami-2023.8.2.1/PAMI/coveragePattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.700713 pami-2023.8.2.1/PAMI/coveragePattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13863 2023-08-02 11:01:01.000000 pami-2023.8.2.1/PAMI/coveragePattern/basic/CMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15929 2023-08-02 11:01:01.000000 pami-2023.8.2.1/PAMI/coveragePattern/basic/CPPG.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:01:01.000000 pami-2023.8.2.1/PAMI/coveragePattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7018 2023-08-02 11:01:01.000000 pami-2023.8.2.1/PAMI/coveragePattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.701813 pami-2023.8.2.1/PAMI/extras/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.704998 pami-2023.8.2.1/PAMI/extras/DF2DB/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-08-02 11:00:51.000000 pami-2023.8.2.1/PAMI/extras/DF2DB/DF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2243 2023-08-02 11:00:51.000000 pami-2023.8.2.1/PAMI/extras/DF2DB/DF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:51.000000 pami-2023.8.2.1/PAMI/extras/DF2DB/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1607 2023-08-02 11:00:51.000000 pami-2023.8.2.1/PAMI/extras/DF2DB/createTDB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4192 2023-08-02 11:00:51.000000 pami-2023.8.2.1/PAMI/extras/DF2DB/denseDF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4917 2023-08-02 11:00:51.000000 pami-2023.8.2.1/PAMI/extras/DF2DB/denseDF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     9942 2023-08-02 11:00:51.000000 pami-2023.8.2.1/PAMI/extras/DF2DB/denseDF2DB_dump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3607 2023-08-02 11:00:51.000000 pami-2023.8.2.1/PAMI/extras/DF2DB/sparseDF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3359 2023-08-02 11:00:51.000000 pami-2023.8.2.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:26.000000 pami-2023.8.2.1/PAMI/extras/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.705422 pami-2023.8.2.1/PAMI/extras/calculateMISValues/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:51.000000 pami-2023.8.2.1/PAMI/extras/calculateMISValues/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3741 2023-08-02 11:00:51.000000 pami-2023.8.2.1/PAMI/extras/calculateMISValues/usingBeta.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3794 2023-08-02 11:00:51.000000 pami-2023.8.2.1/PAMI/extras/calculateMISValues/usingSD.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.707044 pami-2023.8.2.1/PAMI/extras/dbStats/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/dbStats/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13043 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15604 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/dbStats/sequencialDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14610 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/dbStats/temporalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     9436 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/dbStats/transactionalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13229 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    10040 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    11775 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/dbStats/utilityDatabaseStats.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.708330 pami-2023.8.2.1/PAMI/extras/fuzzyTransformation/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/fuzzyTransformation/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/fuzzyTransformation/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5925 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5919 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5803 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.708994 pami-2023.8.2.1/PAMI/extras/generateDatabase/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:47.000000 pami-2023.8.2.1/PAMI/extras/generateDatabase/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2877 2023-08-02 11:00:47.000000 pami-2023.8.2.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7092 2023-08-02 11:00:47.000000 pami-2023.8.2.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3444 2023-08-02 11:00:47.000000 pami-2023.8.2.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3593 2023-08-02 11:00:26.000000 pami-2023.8.2.1/PAMI/extras/generateLatexGraphFile.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.710049 pami-2023.8.2.1/PAMI/extras/graph/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:47.000000 pami-2023.8.2.1/PAMI/extras/graph/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1429 2023-08-02 11:00:47.000000 pami-2023.8.2.1/PAMI/extras/graph/dataFrameInToFigures.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2954 2023-08-02 11:00:47.000000 pami-2023.8.2.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1143 2023-08-02 11:00:47.000000 pami-2023.8.2.1/PAMI/extras/graph/plotLineGraphFromDictionary.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1753 2023-08-02 11:00:47.000000 pami-2023.8.2.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2428 2023-08-02 11:00:47.000000 pami-2023.8.2.1/PAMI/extras/graph/visualizePatterns.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.710257 pami-2023.8.2.1/PAMI/extras/image2Database/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/image2Database/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.710578 pami-2023.8.2.1/PAMI/extras/imageProcessing/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/imageProcessing/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4582 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/imageProcessing/imagery2Databases.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.711073 pami-2023.8.2.1/PAMI/extras/neighbours/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/extras/neighbours/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2834 2023-08-02 11:00:47.000000 pami-2023.8.2.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2651 2023-08-02 11:00:47.000000 pami-2023.8.2.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3031 2023-08-02 11:00:27.000000 pami-2023.8.2.1/PAMI/extras/plotPointOnMap.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3214 2023-08-02 11:00:27.000000 pami-2023.8.2.1/PAMI/extras/plotPointOnMap_dump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-08-02 11:00:27.000000 pami-2023.8.2.1/PAMI/extras/scatterPlotSpatialPoints.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.712617 pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:47.000000 pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2332 2023-08-02 11:00:50.000000 pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2297 2023-08-02 11:00:51.000000 pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2555 2023-08-02 11:00:50.000000 pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1887 2023-08-02 11:00:51.000000 pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1860 2023-08-02 11:00:50.000000 pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2126 2023-08-02 11:00:50.000000 pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2079 2023-08-02 11:00:50.000000 pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2265 2023-08-02 11:00:50.000000 pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1827 2023-08-02 11:00:27.000000 pami-2023.8.2.1/PAMI/extras/topKPatterns.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      473 2023-08-02 11:00:26.000000 pami-2023.8.2.1/PAMI/extras/uncertaindb_convert.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.712783 pami-2023.8.2.1/PAMI/faultTolerantFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:29.000000 pami-2023.8.2.1/PAMI/faultTolerantFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.713550 pami-2023.8.2.1/PAMI/faultTolerantFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13292 2023-08-02 11:00:53.000000 pami-2023.8.2.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21358 2023-08-02 11:00:53.000000 pami-2023.8.2.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:53.000000 pami-2023.8.2.1/PAMI/faultTolerantFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6766 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.713733 pami-2023.8.2.1/PAMI/frequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:33.000000 pami-2023.8.2.1/PAMI/frequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.715185 pami-2023.8.2.1/PAMI/frequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13219 2023-08-02 11:00:59.000000 pami-2023.8.2.1/PAMI/frequentPattern/basic/Apriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12611 2023-08-02 11:00:59.000000 pami-2023.8.2.1/PAMI/frequentPattern/basic/ECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13190 2023-08-02 11:00:59.000000 pami-2023.8.2.1/PAMI/frequentPattern/basic/ECLATDiffset.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13538 2023-08-02 11:00:59.000000 pami-2023.8.2.1/PAMI/frequentPattern/basic/ECLATbitset.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20301 2023-08-02 11:00:59.000000 pami-2023.8.2.1/PAMI/frequentPattern/basic/FPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:59.000000 pami-2023.8.2.1/PAMI/frequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7733 2023-08-02 11:00:59.000000 pami-2023.8.2.1/PAMI/frequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.715746 pami-2023.8.2.1/PAMI/frequentPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19938 2023-08-02 11:00:59.000000 pami-2023.8.2.1/PAMI/frequentPattern/closed/CHARM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:59.000000 pami-2023.8.2.1/PAMI/frequentPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6445 2023-08-02 11:00:59.000000 pami-2023.8.2.1/PAMI/frequentPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.717131 pami-2023.8.2.1/PAMI/frequentPattern/cuda/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:57.000000 pami-2023.8.2.1/PAMI/frequentPattern/cuda/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-08-02 11:00:57.000000 pami-2023.8.2.1/PAMI/frequentPattern/cuda/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13299 2023-08-02 11:00:57.000000 pami-2023.8.2.1/PAMI/frequentPattern/cuda/cuApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14252 2023-08-02 11:00:57.000000 pami-2023.8.2.1/PAMI/frequentPattern/cuda/cuAprioriBit.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12925 2023-08-02 11:00:57.000000 pami-2023.8.2.1/PAMI/frequentPattern/cuda/cuEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14001 2023-08-02 11:00:57.000000 pami-2023.8.2.1/PAMI/frequentPattern/cuda/cuEclatBit.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    11538 2023-08-02 11:00:57.000000 pami-2023.8.2.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13872 2023-08-02 11:00:57.000000 pami-2023.8.2.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    10731 2023-08-02 11:00:57.000000 pami-2023.8.2.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.717580 pami-2023.8.2.1/PAMI/frequentPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25156 2023-08-02 11:00:59.000000 pami-2023.8.2.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:59.000000 pami-2023.8.2.1/PAMI/frequentPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6436 2023-08-02 11:00:59.000000 pami-2023.8.2.1/PAMI/frequentPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.718297 pami-2023.8.2.1/PAMI/frequentPattern/pyspark/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:59.000000 pami-2023.8.2.1/PAMI/frequentPattern/pyspark/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5605 2023-08-02 11:00:57.000000 pami-2023.8.2.1/PAMI/frequentPattern/pyspark/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13545 2023-08-02 11:00:57.000000 pami-2023.8.2.1/PAMI/frequentPattern/pyspark/parallelApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    11987 2023-08-02 11:00:59.000000 pami-2023.8.2.1/PAMI/frequentPattern/pyspark/parallelECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16531 2023-08-02 11:00:57.000000 pami-2023.8.2.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.718788 pami-2023.8.2.1/PAMI/frequentPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14742 2023-08-02 11:00:57.000000 pami-2023.8.2.1/PAMI/frequentPattern/topk/FAE.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:57.000000 pami-2023.8.2.1/PAMI/frequentPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2023-08-02 11:00:57.000000 pami-2023.8.2.1/PAMI/frequentPattern/topk/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.718935 pami-2023.8.2.1/PAMI/fuzzyCorrelatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:35.000000 pami-2023.8.2.1/PAMI/fuzzyCorrelatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.719437 pami-2023.8.2.1/PAMI/fuzzyCorrelatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25498 2023-08-02 11:01:07.000000 pami-2023.8.2.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:01:07.000000 pami-2023.8.2.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6635 2023-08-02 11:01:07.000000 pami-2023.8.2.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.719588 pami-2023.8.2.1/PAMI/fuzzyFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:33.000000 pami-2023.8.2.1/PAMI/fuzzyFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.720282 pami-2023.8.2.1/PAMI/fuzzyFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20910 2023-08-02 11:01:07.000000 pami-2023.8.2.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26294 2023-08-02 11:01:04.000000 pami-2023.8.2.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:01:04.000000 pami-2023.8.2.1/PAMI/fuzzyFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6450 2023-08-02 11:01:04.000000 pami-2023.8.2.1/PAMI/fuzzyFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.720432 pami-2023.8.2.1/PAMI/fuzzyGeoreferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:30.000000 pami-2023.8.2.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.721128 pami-2023.8.2.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24180 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27153 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.721294 pami-2023.8.2.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:27.000000 pami-2023.8.2.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.722136 pami-2023.8.2.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27023 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32449 2023-08-02 11:00:51.000000 pami-2023.8.2.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2023-08-02 11:00:51.000000 pami-2023.8.2.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.722451 pami-2023.8.2.1/PAMI/fuzzyPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:29.000000 pami-2023.8.2.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.723146 pami-2023.8.2.1/PAMI/fuzzyPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23711 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26218 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6668 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.723295 pami-2023.8.2.1/PAMI/geoReferencedPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:27.000000 pami-2023.8.2.1/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.723753 pami-2023.8.2.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19950 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6774 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.723924 pami-2023.8.2.1/PAMI/georeferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:26.000000 pami-2023.8.2.1/PAMI/georeferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.724658 pami-2023.8.2.1/PAMI/georeferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20059 2023-08-02 11:00:40.000000 pami-2023.8.2.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19117 2023-08-02 11:00:40.000000 pami-2023.8.2.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:40.000000 pami-2023.8.2.1/PAMI/georeferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6680 2023-08-02 11:00:40.000000 pami-2023.8.2.1/PAMI/georeferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.724913 pami-2023.8.2.1/PAMI/georeferencedFrequentSequencePattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:33.000000 pami-2023.8.2.1/PAMI/georeferencedFrequentSequencePattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6676 2023-08-02 11:00:33.000000 pami-2023.8.2.1/PAMI/georeferencedFrequentSequencePattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.725062 pami-2023.8.2.1/PAMI/georeferencedPartialPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:27.000000 pami-2023.8.2.1/PAMI/georeferencedPartialPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.725561 pami-2023.8.2.1/PAMI/georeferencedPartialPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19894 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6165 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.725715 pami-2023.8.2.1/PAMI/highUtilityFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:33.000000 pami-2023.8.2.1/PAMI/highUtilityFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.726158 pami-2023.8.2.1/PAMI/highUtilityFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35398 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/highUtilityFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6081 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/highUtilityFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.726316 pami-2023.8.2.1/PAMI/highUtilityGeoreferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:26.000000 pami-2023.8.2.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.726788 pami-2023.8.2.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    39928 2023-08-02 11:00:40.000000 pami-2023.8.2.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6181 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.726961 pami-2023.8.2.1/PAMI/highUtilityPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:33.000000 pami-2023.8.2.1/PAMI/highUtilityPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.728428 pami-2023.8.2.1/PAMI/highUtilityPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32744 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/highUtilityPattern/basic/EFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24844 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/highUtilityPattern/basic/HMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26560 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/highUtilityPattern/basic/UPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/highUtilityPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/highUtilityPattern/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16478 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/highUtilityPattern/basic/efimParallel.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.728979 pami-2023.8.2.1/PAMI/highUtilityPattern/parallel/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/highUtilityPattern/parallel/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/highUtilityPattern/parallel/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16480 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/highUtilityPattern/parallel/efimparallel.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.729747 pami-2023.8.2.1/PAMI/highUtilityPatternsInStreams/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    29434 2023-08-02 11:00:33.000000 pami-2023.8.2.1/PAMI/highUtilityPatternsInStreams/HUPMS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33678 2023-08-02 11:00:33.000000 pami-2023.8.2.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:33.000000 pami-2023.8.2.1/PAMI/highUtilityPatternsInStreams/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-08-02 11:00:33.000000 pami-2023.8.2.1/PAMI/highUtilityPatternsInStreams/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.730056 pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:26.000000 pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6718 2023-08-02 11:00:26.000000 pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.730766 pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27644 2023-08-02 11:00:42.000000 pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    34623 2023-08-02 11:00:42.000000 pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:42.000000 pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5955 2023-08-02 11:00:42.000000 pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.731274 pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35216 2023-08-02 11:00:42.000000 pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:42.000000 pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6625 2023-08-02 11:00:42.000000 pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/topk/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.731427 pami-2023.8.2.1/PAMI/localPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:18.000000 pami-2023.8.2.1/PAMI/localPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.732282 pami-2023.8.2.1/PAMI/localPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32664 2023-08-02 11:00:35.000000 pami-2023.8.2.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21999 2023-08-02 11:00:35.000000 pami-2023.8.2.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21120 2023-08-02 11:00:35.000000 pami-2023.8.2.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:35.000000 pami-2023.8.2.1/PAMI/localPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8378 2023-08-02 11:00:35.000000 pami-2023.8.2.1/PAMI/localPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.732442 pami-2023.8.2.1/PAMI/multipleMinimumSupportBasedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:27.000000 pami-2023.8.2.1/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.733224 pami-2023.8.2.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22994 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22318 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5913 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.733537 pami-2023.8.2.1/PAMI/partialPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:29.000000 pami-2023.8.2.1/PAMI/partialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.734101 pami-2023.8.2.1/PAMI/partialPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27316 2023-08-02 11:00:53.000000 pami-2023.8.2.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21102 2023-08-02 11:00:53.000000 pami-2023.8.2.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:53.000000 pami-2023.8.2.1/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5392 2023-08-02 11:00:53.000000 pami-2023.8.2.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.734287 pami-2023.8.2.1/PAMI/partialPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:26.000000 pami-2023.8.2.1/PAMI/partialPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.735291 pami-2023.8.2.1/PAMI/partialPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    50844 2023-08-02 11:00:43.000000 pami-2023.8.2.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4195 2023-08-02 11:00:43.000000 pami-2023.8.2.1/PAMI/partialPeriodicPattern/basic/Gabstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24330 2023-08-02 11:00:43.000000 pami-2023.8.2.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17878 2023-08-02 11:00:43.000000 pami-2023.8.2.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:43.000000 pami-2023.8.2.1/PAMI/partialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5572 2023-08-02 11:00:43.000000 pami-2023.8.2.1/PAMI/partialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.735724 pami-2023.8.2.1/PAMI/partialPeriodicPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21069 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/partialPeriodicPattern/closed/PPPClose.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:43.000000 pami-2023.8.2.1/PAMI/partialPeriodicPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5595 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/partialPeriodicPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.736176 pami-2023.8.2.1/PAMI/partialPeriodicPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28482 2023-08-02 11:00:43.000000 pami-2023.8.2.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:43.000000 pami-2023.8.2.1/PAMI/partialPeriodicPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-08-02 11:00:43.000000 pami-2023.8.2.1/PAMI/partialPeriodicPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.736575 pami-2023.8.2.1/PAMI/partialPeriodicPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/partialPeriodicPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7837 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/partialPeriodicPattern/topk/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17705 2023-08-02 11:00:44.000000 pami-2023.8.2.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.737101 pami-2023.8.2.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26067 2023-08-02 11:00:29.000000 pami-2023.8.2.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:29.000000 pami-2023.8.2.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-08-02 11:00:29.000000 pami-2023.8.2.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.737241 pami-2023.8.2.1/PAMI/periodicCorrelatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:33.000000 pami-2023.8.2.1/PAMI/periodicCorrelatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.737652 pami-2023.8.2.1/PAMI/periodicCorrelatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27518 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/periodicCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/periodicCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.737784 pami-2023.8.2.1/PAMI/periodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:18.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.739778 pami-2023.8.2.1/PAMI/periodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15591 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25146 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24942 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16311 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/basic/PFPMC.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33244 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6525 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.740236 pami-2023.8.2.1/PAMI/periodicFrequentPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21540 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6538 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.740845 pami-2023.8.2.1/PAMI/periodicFrequentPattern/cuda/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/cuda/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/cuda/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19356 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17474 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.741303 pami-2023.8.2.1/PAMI/periodicFrequentPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28740 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7873 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.741667 pami-2023.8.2.1/PAMI/periodicFrequentPattern/pyspark/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/pyspark/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5378 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/pyspark/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24444 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.741833 pami-2023.8.2.1/PAMI/periodicFrequentPattern/topk/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.742287 pami-2023.8.2.1/PAMI/periodicFrequentPattern/topk/TopkPFP/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18066 2023-08-02 11:01:07.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:01:07.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6898 2023-08-02 11:01:07.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/topk/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.742727 pami-2023.8.2.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:01:07.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4583 2023-08-02 11:01:07.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17235 2023-08-02 11:01:07.000000 pami-2023.8.2.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.742896 pami-2023.8.2.1/PAMI/recurringPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:27.000000 pami-2023.8.2.1/PAMI/recurringPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.743296 pami-2023.8.2.1/PAMI/recurringPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26300 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/recurringPattern/basic/RPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/recurringPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6632 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/recurringPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.743432 pami-2023.8.2.1/PAMI/relativeFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:33.000000 pami-2023.8.2.1/PAMI/relativeFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.743872 pami-2023.8.2.1/PAMI/relativeFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26215 2023-08-02 11:01:01.000000 pami-2023.8.2.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:01:03.000000 pami-2023.8.2.1/PAMI/relativeFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-08-02 11:01:01.000000 pami-2023.8.2.1/PAMI/relativeFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.744000 pami-2023.8.2.1/PAMI/relativeHighUtilityPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:26.000000 pami-2023.8.2.1/PAMI/relativeHighUtilityPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.744959 pami-2023.8.2.1/PAMI/relativeHighUtilityPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33570 2023-08-02 11:00:42.000000 pami-2023.8.2.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:42.000000 pami-2023.8.2.1/PAMI/relativeHighUtilityPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7391 2023-08-02 11:00:42.000000 pami-2023.8.2.1/PAMI/relativeHighUtilityPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.745109 pami-2023.8.2.1/PAMI/sequence/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:29.000000 pami-2023.8.2.1/PAMI/sequence/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.745205 pami-2023.8.2.1/PAMI/sequentialPatternMining/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:18.000000 pami-2023.8.2.1/PAMI/sequentialPatternMining/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.745984 pami-2023.8.2.1/PAMI/sequentialPatternMining/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    41062 2023-08-02 11:00:37.000000 pami-2023.8.2.1/PAMI/sequentialPatternMining/basic/SPADE.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18133 2023-08-02 11:00:37.000000 pami-2023.8.2.1/PAMI/sequentialPatternMining/basic/SPAM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:37.000000 pami-2023.8.2.1/PAMI/sequentialPatternMining/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6554 2023-08-02 11:00:37.000000 pami-2023.8.2.1/PAMI/sequentialPatternMining/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22592 2023-08-02 11:00:37.000000 pami-2023.8.2.1/PAMI/sequentialPatternMining/basic/prefixSpan.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.746388 pami-2023.8.2.1/PAMI/sequentialPatternMining/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:35.000000 pami-2023.8.2.1/PAMI/sequentialPatternMining/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6279 2023-08-02 11:00:37.000000 pami-2023.8.2.1/PAMI/sequentialPatternMining/closed/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:35.000000 pami-2023.8.2.1/PAMI/sequentialPatternMining/closed/bide.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.746487 pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:33.000000 pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.747262 pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16326 2023-08-02 11:01:01.000000 pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25134 2023-08-02 11:01:01.000000 pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17903 2023-08-02 11:01:01.000000 pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:01:01.000000 pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7258 2023-08-02 11:01:01.000000 pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.747784 pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/topK/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26386 2023-08-02 11:01:01.000000 pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:01:01.000000 pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7177 2023-08-02 11:01:01.000000 pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.748226 pami-2023.8.2.1/PAMI/uncertainFaultTolerantFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14997 2023-08-02 11:00:34.000000 pami-2023.8.2.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:35.000000 pami-2023.8.2.1/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6766 2023-08-02 11:00:33.000000 pami-2023.8.2.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.748374 pami-2023.8.2.1/PAMI/uncertainFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:26.000000 pami-2023.8.2.1/PAMI/uncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.750019 pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25974 2023-08-02 11:00:40.000000 pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26009 2023-08-02 11:00:40.000000 pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18710 2023-08-02 11:00:40.000000 pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/TUFP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27060 2023-08-02 11:00:40.000000 pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/TubeP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27823 2023-08-02 11:00:40.000000 pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/TubeS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25507 2023-08-02 11:00:40.000000 pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19046 2023-08-02 11:00:40.000000 pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:40.000000 pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4962 2023-08-02 11:00:40.000000 pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.750159 pami-2023.8.2.1/PAMI/uncertainGeoreferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:33.000000 pami-2023.8.2.1/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.751804 pami-2023.8.2.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28817 2023-08-02 11:01:03.000000 pami-2023.8.2.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:01:03.000000 pami-2023.8.2.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5005 2023-08-02 11:01:03.000000 pami-2023.8.2.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.752062 pami-2023.8.2.1/PAMI/uncertainPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-02 11:00:18.000000 pami-2023.8.2.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.752938 pami-2023.8.2.1/PAMI/uncertainPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31092 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31324 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6551 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.753090 pami-2023.8.2.1/PAMI/weightedFrequentNeighbourhoodPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:26.000000 pami-2023.8.2.1/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.753542 pami-2023.8.2.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27481 2023-08-02 11:00:41.000000 pami-2023.8.2.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:41.000000 pami-2023.8.2.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6693 2023-08-02 11:00:40.000000 pami-2023.8.2.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.753695 pami-2023.8.2.1/PAMI/weightedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:31.000000 pami-2023.8.2.1/PAMI/weightedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.754161 pami-2023.8.2.1/PAMI/weightedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23859 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/weightedFrequentPattern/basic/WFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/weightedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6737 2023-08-02 11:00:56.000000 pami-2023.8.2.1/PAMI/weightedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.754320 pami-2023.8.2.1/PAMI/weightedFrequentRegularPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:18.000000 pami-2023.8.2.1/PAMI/weightedFrequentRegularPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.754757 pami-2023.8.2.1/PAMI/weightedFrequentRegularPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27228 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/weightedFrequentRegularPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7555 2023-08-02 11:00:38.000000 pami-2023.8.2.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.754911 pami-2023.8.2.1/PAMI/weightedUncertainFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:00:29.000000 pami-2023.8.2.1/PAMI/weightedUncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.755382 pami-2023.8.2.1/PAMI/weightedUncertainFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    29074 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4782 2023-08-02 11:00:52.000000 pami-2023.8.2.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    61265 2023-08-02 11:09:06.756423 pami-2023.8.2.1/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    60578 2023-08-02 11:00:06.000000 pami-2023.8.2.1/README.md
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 11:09:06.756112 pami-2023.8.2.1/pami.egg-info/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    61265 2023-08-02 11:09:06.000000 pami-2023.8.2.1/pami.egg-info/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15414 2023-08-02 11:09:06.000000 pami-2023.8.2.1/pami.egg-info/SOURCES.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 11:09:06.000000 pami-2023.8.2.1/pami.egg-info/dependency_links.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      189 2023-08-02 11:09:06.000000 pami-2023.8.2.1/pami.egg-info/requires.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2023-08-02 11:09:06.000000 pami-2023.8.2.1/pami.egg-info/top_level.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-08-02 11:09:06.756627 pami-2023.8.2.1/setup.cfg
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1405 2023-08-02 11:02:47.000000 pami-2023.8.2.1/setup.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.534173 pami-2023.8.6.1/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-07-24 10:04:09.000000 pami-2023.8.6.1/LICENSE
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.467364 pami-2023.8.6.1/PAMI/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.467549 pami-2023.8.6.1/PAMI/AssociationRules/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/AssociationRules/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.470125 pami-2023.8.6.1/PAMI/AssociationRules/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13175 2023-07-25 12:32:03.000000 pami-2023.8.6.1/PAMI/AssociationRules/basic/ARWithConfidence.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12870 2023-07-25 12:32:03.000000 pami-2023.8.6.1/PAMI/AssociationRules/basic/ARWithLeverage.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13078 2023-07-25 12:32:03.000000 pami-2023.8.6.1/PAMI/AssociationRules/basic/ARWithLift.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12384 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/AssociationRules/basic/RuleMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/AssociationRules/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6455 2023-07-25 07:30:57.000000 pami-2023.8.6.1/PAMI/AssociationRules/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.470362 pami-2023.8.6.1/PAMI/correlatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/correlatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.471689 pami-2023.8.6.1/PAMI/correlatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24834 2023-07-25 12:32:03.000000 pami-2023.8.6.1/PAMI/correlatedPattern/basic/CoMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26312 2023-07-25 12:32:03.000000 pami-2023.8.6.1/PAMI/correlatedPattern/basic/CoMinePlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/correlatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6065 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/correlatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.471835 pami-2023.8.6.1/PAMI/coveragePattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/coveragePattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.472526 pami-2023.8.6.1/PAMI/coveragePattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13863 2023-07-25 12:32:03.000000 pami-2023.8.6.1/PAMI/coveragePattern/basic/CMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15929 2023-07-26 05:11:46.000000 pami-2023.8.6.1/PAMI/coveragePattern/basic/CPPG.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/coveragePattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7018 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/coveragePattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.473625 pami-2023.8.6.1/PAMI/extras/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.474899 pami-2023.8.6.1/PAMI/extras/DF2DB/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/DF2DB/DF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2243 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/DF2DB/DF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/DF2DB/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1607 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/DF2DB/createTDB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4192 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/DF2DB/denseDF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4917 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/DF2DB/denseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9942 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/DF2DB/denseDF2DB_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3607 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/DF2DB/sparseDF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3359 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.475267 pami-2023.8.6.1/PAMI/extras/calculateMISValues/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/calculateMISValues/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3741 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/calculateMISValues/usingBeta.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3794 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/calculateMISValues/usingSD.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.476605 pami-2023.8.6.1/PAMI/extras/dbStats/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/dbStats/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13043 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15113 2023-08-06 15:38:03.000000 pami-2023.8.6.1/PAMI/extras/dbStats/sequentialDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14610 2023-07-30 05:40:09.000000 pami-2023.8.6.1/PAMI/extras/dbStats/temporalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9475 2023-08-06 15:38:03.000000 pami-2023.8.6.1/PAMI/extras/dbStats/transactionalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13229 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    10040 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11775 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/dbStats/utilityDatabaseStats.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.477250 pami-2023.8.6.1/PAMI/extras/fuzzyTransformation/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/fuzzyTransformation/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/fuzzyTransformation/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5925 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5919 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5803 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.477838 pami-2023.8.6.1/PAMI/extras/generateDatabase/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/generateDatabase/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2877 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7092 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3444 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3593 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/generateLatexGraphFile.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.478774 pami-2023.8.6.1/PAMI/extras/graph/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/graph/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1429 2023-07-28 06:47:15.000000 pami-2023.8.6.1/PAMI/extras/graph/dataFrameInToFigures.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2954 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1143 2023-08-02 06:55:18.000000 pami-2023.8.6.1/PAMI/extras/graph/plotLineGraphFromDictionary.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1753 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2428 2023-08-02 09:17:46.000000 pami-2023.8.6.1/PAMI/extras/graph/visualizePatterns.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.479025 pami-2023.8.6.1/PAMI/extras/image2Database/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/image2Database/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.479258 pami-2023.8.6.1/PAMI/extras/imageProcessing/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/imageProcessing/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4582 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/imageProcessing/imagery2Databases.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.479648 pami-2023.8.6.1/PAMI/extras/neighbours/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/neighbours/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2834 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2651 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3031 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/plotPointOnMap.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3214 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/plotPointOnMap_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/scatterPlotSpatialPoints.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.480916 pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2332 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2297 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2555 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1887 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1860 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2126 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2079 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2265 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1827 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/topKPatterns.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      473 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/extras/uncertaindb_convert.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.481054 pami-2023.8.6.1/PAMI/faultTolerantFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/faultTolerantFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.482396 pami-2023.8.6.1/PAMI/faultTolerantFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13539 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21425 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/faultTolerantFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6766 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.482563 pami-2023.8.6.1/PAMI/frequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/frequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.483716 pami-2023.8.6.1/PAMI/frequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13211 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/basic/Apriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12603 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/basic/ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13581 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/basic/ECLATDiffset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13664 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/basic/ECLATbitset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20368 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/basic/FPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/frequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7733 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/frequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.484444 pami-2023.8.6.1/PAMI/frequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19938 2023-07-28 04:20:39.000000 pami-2023.8.6.1/PAMI/frequentPattern/closed/CHARM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/frequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6445 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/frequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.485914 pami-2023.8.6.1/PAMI/frequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/frequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5835 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/cuda/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13146 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/cuda/cuApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13904 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/cuda/cuAprioriBit.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12502 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/cuda/cuEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14048 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/cuda/cuEclatBit.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14219 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16723 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13776 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.486469 pami-2023.8.6.1/PAMI/frequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25085 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/frequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6436 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/frequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.487162 pami-2023.8.6.1/PAMI/frequentPattern/pyspark/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/frequentPattern/pyspark/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5611 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/pyspark/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14955 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/pyspark/parallelApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12298 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/pyspark/parallelECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16532 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.487672 pami-2023.8.6.1/PAMI/frequentPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14742 2023-07-28 04:20:39.000000 pami-2023.8.6.1/PAMI/frequentPattern/topk/FAE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/frequentPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/frequentPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.487830 pami-2023.8.6.1/PAMI/fuzzyCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/fuzzyCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.488373 pami-2023.8.6.1/PAMI/fuzzyCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25491 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6635 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.488658 pami-2023.8.6.1/PAMI/fuzzyFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/fuzzyFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.489569 pami-2023.8.6.1/PAMI/fuzzyFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20917 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26298 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/fuzzyFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6450 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/fuzzyFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.489840 pami-2023.8.6.1/PAMI/fuzzyGeoreferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.490940 pami-2023.8.6.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24180 2023-07-29 15:37:17.000000 pami-2023.8.6.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27143 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.491122 pami-2023.8.6.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.492137 pami-2023.8.6.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27023 2023-07-29 15:44:25.000000 pami-2023.8.6.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32449 2023-07-29 15:44:25.000000 pami-2023.8.6.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.492345 pami-2023.8.6.1/PAMI/fuzzyPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.493370 pami-2023.8.6.1/PAMI/fuzzyPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23759 2023-08-04 05:55:40.000000 pami-2023.8.6.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26218 2023-07-28 04:20:39.000000 pami-2023.8.6.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6668 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.493598 pami-2023.8.6.1/PAMI/geoReferencedPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.494304 pami-2023.8.6.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19950 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6774 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.494516 pami-2023.8.6.1/PAMI/georeferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-25 07:30:57.000000 pami-2023.8.6.1/PAMI/georeferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.496016 pami-2023.8.6.1/PAMI/georeferencedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20059 2023-07-25 07:30:57.000000 pami-2023.8.6.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19117 2023-07-25 07:30:57.000000 pami-2023.8.6.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.6.1/PAMI/georeferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6680 2023-07-25 07:30:57.000000 pami-2023.8.6.1/PAMI/georeferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.496326 pami-2023.8.6.1/PAMI/georeferencedFrequentSequencePattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/georeferencedFrequentSequencePattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6676 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/georeferencedFrequentSequencePattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.496493 pami-2023.8.6.1/PAMI/georeferencedPartialPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/georeferencedPartialPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.497511 pami-2023.8.6.1/PAMI/georeferencedPartialPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19894 2023-07-29 16:51:12.000000 pami-2023.8.6.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6165 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.497753 pami-2023.8.6.1/PAMI/highUtilityFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.498220 pami-2023.8.6.1/PAMI/highUtilityFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35398 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6081 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.498377 pami-2023.8.6.1/PAMI/highUtilityGeoreferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.499567 pami-2023.8.6.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    39928 2023-07-29 16:07:24.000000 pami-2023.8.6.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6181 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.499841 pami-2023.8.6.1/PAMI/highUtilityPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.501384 pami-2023.8.6.1/PAMI/highUtilityPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32744 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityPattern/basic/EFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24844 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityPattern/basic/HMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26560 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityPattern/basic/UPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityPattern/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16478 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityPattern/basic/efimParallel.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.501820 pami-2023.8.6.1/PAMI/highUtilityPattern/parallel/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityPattern/parallel/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityPattern/parallel/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16480 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityPattern/parallel/efimparallel.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.502440 pami-2023.8.6.1/PAMI/highUtilityPatternsInStreams/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29434 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityPatternsInStreams/HUPMS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33678 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityPatternsInStreams/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilityPatternsInStreams/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.502758 pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6718 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.503569 pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27644 2023-07-29 16:07:24.000000 pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    34623 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5955 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.503984 pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35216 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6625 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.504155 pami-2023.8.6.1/PAMI/localPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/localPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.504963 pami-2023.8.6.1/PAMI/localPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32664 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21999 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21120 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/localPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8378 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/localPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.505111 pami-2023.8.6.1/PAMI/multipleMinimumSupportBasedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.506057 pami-2023.8.6.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22994 2023-07-29 11:47:49.000000 pami-2023.8.6.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22318 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5913 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.506438 pami-2023.8.6.1/PAMI/partialPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.507084 pami-2023.8.6.1/PAMI/partialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27316 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21102 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5392 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.507241 pami-2023.8.6.1/PAMI/partialPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.508398 pami-2023.8.6.1/PAMI/partialPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    50844 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4195 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/basic/Gabstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24330 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17878 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5572 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.508913 pami-2023.8.6.1/PAMI/partialPeriodicPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21069 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/closed/PPPClose.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5595 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.509412 pami-2023.8.6.1/PAMI/partialPeriodicPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28482 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.510125 pami-2023.8.6.1/PAMI/partialPeriodicPattern/pyspark/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-06 15:38:03.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/pyspark/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5572 2023-08-01 01:42:22.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/pyspark/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    30356 2023-08-01 01:42:22.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.511183 pami-2023.8.6.1/PAMI/partialPeriodicPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7837 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/topk/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17705 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.511970 pami-2023.8.6.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26067 2023-07-29 16:46:35.000000 pami-2023.8.6.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.512117 pami-2023.8.6.1/PAMI/periodicCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.512616 pami-2023.8.6.1/PAMI/periodicCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27518 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.512767 pami-2023.8.6.1/PAMI/periodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.514476 pami-2023.8.6.1/PAMI/periodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15591 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25146 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24942 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16311 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/basic/PFPMC.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33244 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6525 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.514921 pami-2023.8.6.1/PAMI/periodicFrequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21540 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6538 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.515595 pami-2023.8.6.1/PAMI/periodicFrequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/cuda/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19356 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17474 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.516173 pami-2023.8.6.1/PAMI/periodicFrequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28740 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7873 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.516871 pami-2023.8.6.1/PAMI/periodicFrequentPattern/pyspark/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-28 05:36:37.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/pyspark/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5378 2023-07-28 05:41:12.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/pyspark/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24444 2023-07-28 13:21:57.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.517389 pami-2023.8.6.1/PAMI/periodicFrequentPattern/topk/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.517888 pami-2023.8.6.1/PAMI/periodicFrequentPattern/topk/TopkPFP/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18066 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6898 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/topk/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.518431 pami-2023.8.6.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4583 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17235 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.518624 pami-2023.8.6.1/PAMI/recurringPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/recurringPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.519068 pami-2023.8.6.1/PAMI/recurringPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26300 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/recurringPattern/basic/RPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/recurringPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6632 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/recurringPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.519212 pami-2023.8.6.1/PAMI/relativeFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/relativeFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.519698 pami-2023.8.6.1/PAMI/relativeFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26215 2023-08-01 01:42:22.000000 pami-2023.8.6.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/relativeFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/relativeFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.519839 pami-2023.8.6.1/PAMI/relativeHighUtilityPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/relativeHighUtilityPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.520251 pami-2023.8.6.1/PAMI/relativeHighUtilityPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33570 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/relativeHighUtilityPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7391 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/relativeHighUtilityPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.520394 pami-2023.8.6.1/PAMI/sequence/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/sequence/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.520503 pami-2023.8.6.1/PAMI/sequentialPatternMining/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/sequentialPatternMining/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.521458 pami-2023.8.6.1/PAMI/sequentialPatternMining/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    41062 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/sequentialPatternMining/basic/SPADE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18133 2023-08-02 09:17:46.000000 pami-2023.8.6.1/PAMI/sequentialPatternMining/basic/SPAM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/sequentialPatternMining/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6554 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/sequentialPatternMining/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22592 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/sequentialPatternMining/basic/prefixSpan.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.522103 pami-2023.8.6.1/PAMI/sequentialPatternMining/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/sequentialPatternMining/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6279 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/sequentialPatternMining/closed/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/sequentialPatternMining/closed/bide.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.522202 pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.523543 pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16326 2023-07-29 11:25:56.000000 pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25134 2023-07-29 11:57:55.000000 pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17903 2023-07-29 11:57:55.000000 pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7258 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.524065 pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/topK/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26386 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7177 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.524430 pami-2023.8.6.1/PAMI/uncertainFaultTolerantFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14997 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6766 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.524567 pami-2023.8.6.1/PAMI/uncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/uncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.526134 pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25974 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26009 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18710 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/TUFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27060 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/TubeP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27823 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/TubeS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25507 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19046 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4962 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.526278 pami-2023.8.6.1/PAMI/uncertainGeoreferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.6.1/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.527421 pami-2023.8.6.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28817 2023-07-25 07:30:57.000000 pami-2023.8.6.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.6.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5005 2023-07-25 07:30:57.000000 pami-2023.8.6.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.527577 pami-2023.8.6.1/PAMI/uncertainPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.528370 pami-2023.8.6.1/PAMI/uncertainPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31092 2023-07-29 11:28:40.000000 pami-2023.8.6.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31324 2023-07-29 11:28:40.000000 pami-2023.8.6.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6551 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.528585 pami-2023.8.6.1/PAMI/weightedFrequentNeighbourhoodPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.529351 pami-2023.8.6.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27481 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6693 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.529499 pami-2023.8.6.1/PAMI/weightedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/weightedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.530124 pami-2023.8.6.1/PAMI/weightedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23859 2023-07-29 11:29:36.000000 pami-2023.8.6.1/PAMI/weightedFrequentPattern/basic/WFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/weightedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6737 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/weightedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.530386 pami-2023.8.6.1/PAMI/weightedFrequentRegularPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/weightedFrequentRegularPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.531278 pami-2023.8.6.1/PAMI/weightedFrequentRegularPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27228 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/weightedFrequentRegularPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7555 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.531460 pami-2023.8.6.1/PAMI/weightedUncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/weightedUncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.532563 pami-2023.8.6.1/PAMI/weightedUncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29074 2023-07-29 11:29:37.000000 pami-2023.8.6.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4782 2023-07-24 10:04:09.000000 pami-2023.8.6.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    61265 2023-08-06 15:39:11.533973 pami-2023.8.6.1/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    60578 2023-08-02 07:28:07.000000 pami-2023.8.6.1/README.md
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-06 15:39:11.533537 pami-2023.8.6.1/pami.egg-info/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    61265 2023-08-06 15:39:11.000000 pami-2023.8.6.1/pami.egg-info/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15566 2023-08-06 15:39:11.000000 pami-2023.8.6.1/pami.egg-info/SOURCES.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-06 15:39:11.000000 pami-2023.8.6.1/pami.egg-info/dependency_links.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      189 2023-08-06 15:39:11.000000 pami-2023.8.6.1/pami.egg-info/requires.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2023-08-06 15:39:11.000000 pami-2023.8.6.1/pami.egg-info/top_level.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-08-06 15:39:11.534279 pami-2023.8.6.1/setup.cfg
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1405 2023-08-06 15:38:22.000000 pami-2023.8.6.1/setup.py
```

### Comparing `pami-2023.8.2.1/LICENSE` & `pami-2023.8.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/AssociationRules/basic/ARWithConfidence.py` & `pami-2023.8.6.1/PAMI/AssociationRules/basic/ARWithConfidence.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/AssociationRules/basic/ARWithLeverage.py` & `pami-2023.8.6.1/PAMI/AssociationRules/basic/ARWithLeverage.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/AssociationRules/basic/ARWithLift.py` & `pami-2023.8.6.1/PAMI/AssociationRules/basic/ARWithLift.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/AssociationRules/basic/RuleMiner.py` & `pami-2023.8.6.1/PAMI/AssociationRules/basic/RuleMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/AssociationRules/basic/abstract.py` & `pami-2023.8.6.1/PAMI/AssociationRules/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/correlatedPattern/__init__.py` & `pami-2023.8.6.1/PAMI/correlatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/correlatedPattern/basic/CoMine.py` & `pami-2023.8.6.1/PAMI/correlatedPattern/basic/CoMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/correlatedPattern/basic/CoMinePlus.py` & `pami-2023.8.6.1/PAMI/correlatedPattern/basic/CoMinePlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/correlatedPattern/basic/__init__.py` & `pami-2023.8.6.1/PAMI/correlatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/correlatedPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/correlatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/coveragePattern/basic/CMine.py` & `pami-2023.8.6.1/PAMI/coveragePattern/basic/CMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/coveragePattern/basic/CPPG.py` & `pami-2023.8.6.1/PAMI/coveragePattern/basic/CPPG.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/coveragePattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/coveragePattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/DF2DB/DF2DB.py` & `pami-2023.8.6.1/PAMI/extras/DF2DB/DF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/DF2DB/DF2DBPlus.py` & `pami-2023.8.6.1/PAMI/extras/DF2DB/DF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/DF2DB/createTDB.py` & `pami-2023.8.6.1/PAMI/extras/DF2DB/createTDB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/DF2DB/denseDF2DB.py` & `pami-2023.8.6.1/PAMI/extras/DF2DB/denseDF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/DF2DB/denseDF2DBPlus.py` & `pami-2023.8.6.1/PAMI/extras/DF2DB/denseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/DF2DB/denseDF2DB_dump.py` & `pami-2023.8.6.1/PAMI/extras/DF2DB/denseDF2DB_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/DF2DB/sparseDF2DB.py` & `pami-2023.8.6.1/PAMI/extras/DF2DB/sparseDF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py` & `pami-2023.8.6.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/calculateMISValues/usingBeta.py` & `pami-2023.8.6.1/PAMI/extras/calculateMISValues/usingBeta.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/calculateMISValues/usingSD.py` & `pami-2023.8.6.1/PAMI/extras/calculateMISValues/usingSD.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py` & `pami-2023.8.6.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/dbStats/sequencialDatabaseStats.py` & `pami-2023.8.6.1/PAMI/extras/dbStats/sequentialDatabaseStats.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,23 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-"""
+import statistics
+import validators
+from urllib.request import urlopen
+import PAMI.extras.graph.plotLineGraphFromDictionary as plt
+import sys
+
+
+class sequentialDatabaseStats():
+    """
         sequentialDatabaseStats is to get stats of database like avarage, minimun, maximum  and so on.
 
         Reference:
         ----------
 
         ----------
             :param inputFile: file :
@@ -91,38 +99,15 @@
             _ap=alg.sequentialDatabaseStats(inputfile,sep)
             _ap.readDatabase()
             _ap.printStats()
             _ap.plotGraphs()
         Credits:
         --------
             The complete program was written by Shota Suzuki  under the supervision of Professor Rage Uday Kiran.
-"""
-
-import statistics
-import validators
-from urllib.request import urlopen
-import PAMI.extras.graph.plotLineGraphFromDictionary as plt
-import sys
-class sequentialDatabaseStats():
     """
-           :Description:  sequentialDatabaseStats is class to get stats of database.
-
-
-           :param inputFile: file :
-               input file path
-           :param database: dict :
-               store time stamp and its ()separated by subsequence)
-           :param seqLengthList: list :
-               store size of all sequence
-           :param subSeqLengthList: list :
-               store size of all subsequence
-           :param sep: str
-               separator in file. Default is tab space.
-
-              """
 
     def __init__(self, inputFile, sep='\t'):
         """
         :param inputFile: input file name or path
         :type inputFile: str
         """
         self.inputFile = inputFile
@@ -338,15 +323,16 @@
         transactionLength = {}
         for sublen in self.subSeqLengthList:
             for length in sublen:
                 transactionLength[length] = transactionLength.get(length, 0)
                 transactionLength[length] += 1
         return {k: v for k, v in sorted(transactionLength.items(), key=lambda x: x[0])}
 
-
+    def run(self):
+        self.readDatabase()
 
     def printStats(self):
         """
         to print the all status of sequence database
         Returns:
 
         """
@@ -380,12 +366,12 @@
 if __name__ == '__main__':
     _ap=str()
     if len(sys.argv)==3 or len(sys.argv)==2:
         if len(sys.argv)==3:
             _ap=sequentialDatabaseStats(sys.argv[1],sys.argv[2])
         if len(sys.argv) == 2:
             _ap = sequentialDatabaseStats(sys.argv[1])
-        _ap.readDatabase()
+        _ap.run()
         _ap.printStats()
         _ap.plotGraphs()
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.8.2.1/PAMI/extras/dbStats/temporalDatabaseStats.py` & `pami-2023.8.6.1/PAMI/extras/dbStats/temporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/dbStats/transactionalDatabaseStats.py` & `pami-2023.8.6.1/PAMI/extras/dbStats/transactionalDatabaseStats.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,16 +240,17 @@
 
             'Transactions': [['a', 'd', 'e'], ['b', 'a', 'f', 'g', 'h'], ['b', 'a', 'd', 'f'], ['b', 'a', 'c'],
                              ['a', 'd', 'g', 'k'],
 
                              ['b', 'd', 'g', 'c', 'i'], ['b', 'd', 'g', 'e', 'j']]}
 
     # data = pd.DataFrame.from_dict('transactional_T10I4D100K.csv')
+    import PAMI.extras.graph.plotLineGraphFromDictionary as plt
     import pandas as pd
-    # obj = transactionalDatabaseStats('transactional_BMS1.txt', ',')
+    # obj = transactionalDatabaseStats(data)
     obj = transactionalDatabaseStats(pd.DataFrame(data))
     obj.run()
     obj.printStats()
     obj.plotGraphs()
```

### Comparing `pami-2023.8.2.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py` & `pami-2023.8.6.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py` & `pami-2023.8.6.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/dbStats/utilityDatabaseStats.py` & `pami-2023.8.6.1/PAMI/extras/dbStats/utilityDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/fuzzyTransformation/abstract.py` & `pami-2023.8.6.1/PAMI/extras/fuzzyTransformation/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py` & `pami-2023.8.6.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py` & `pami-2023.8.6.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py` & `pami-2023.8.6.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py` & `pami-2023.8.6.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py` & `pami-2023.8.6.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py` & `pami-2023.8.6.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/generateLatexGraphFile.py` & `pami-2023.8.6.1/PAMI/extras/generateLatexGraphFile.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/graph/dataFrameInToFigures.py` & `pami-2023.8.6.1/PAMI/extras/graph/dataFrameInToFigures.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py` & `pami-2023.8.6.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/graph/plotLineGraphFromDictionary.py` & `pami-2023.8.6.1/PAMI/extras/graph/plotLineGraphFromDictionary.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py` & `pami-2023.8.6.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/graph/visualizePatterns.py` & `pami-2023.8.6.1/PAMI/extras/graph/visualizePatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/imageProcessing/imagery2Databases.py` & `pami-2023.8.6.1/PAMI/extras/imageProcessing/imagery2Databases.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py` & `pami-2023.8.6.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py` & `pami-2023.8.6.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/plotPointOnMap.py` & `pami-2023.8.6.1/PAMI/extras/plotPointOnMap.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/plotPointOnMap_dump.py` & `pami-2023.8.6.1/PAMI/extras/plotPointOnMap_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/scatterPlotSpatialPoints.py` & `pami-2023.8.6.1/PAMI/extras/scatterPlotSpatialPoints.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py` & `pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py` & `pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py` & `pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py` & `pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py` & `pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py` & `pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py` & `pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py` & `pami-2023.8.6.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/extras/topKPatterns.py` & `pami-2023.8.6.1/PAMI/extras/topKPatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py` & `pami-2023.8.6.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     
             obj.startMine()
     
             patterns = obj.getPatterns()
     
             print("Total number of fault-tolerant frequent patterns:",  len(patterns))
     
-            obj.savePatterns("outputFile")
+            obj.save("outputFile")
     
             memUSS = obj.getMemoryUSS()
     
             print("Total Memory in USS:",  memUSS)
     
             memRSS = obj.getMemoryRSS()
     
@@ -244,14 +244,26 @@
                 if i not in self._mapSupport:
                     self._mapSupport[i] = 1
                 else:
                     self._mapSupport[i] += 1
         self._mapSupport = {k: v for k, v in self._mapSupport.items() if v >= self._itemSup}
 
     def _countItemSupport(self, itemset):
+        """
+
+        This function is used to count the  itemSupport
+        Parameters:
+        ----------
+            itemSet: frequent itemSet that generated
+
+        Returns:
+        -------
+            patterns with original item names.
+
+        """
         tids = {}
         res = True
         count = 0
         for x in self._Database:
             if abs(len(itemset) - len(set(x) & set(itemset))) <= self._faultTolerance:
                 count += 1
         return count
```

### Comparing `pami-2023.8.2.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py` & `pami-2023.8.6.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py`

 * *Files 1% similar despite different names*

```diff
@@ -614,14 +614,16 @@
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self.__finalPatterns
 
     def printResults(self):
+        """ this function is used to print the results
+        """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.8.2.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/__init__.py` & `pami-2023.8.6.1/PAMI/frequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/basic/Apriori.py` & `pami-2023.8.6.1/PAMI/frequentPattern/basic/Apriori.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
              obj.startMine()
 
              frequentPatterns = obj.getPatterns()
 
              print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-             obj.savePatterns(oFile)
+             obj.save(oFile)
 
              Df = obj.getPatternInDataFrame()
 
              memUSS = obj.getMemoryUSS()
 
              print("Total Memory in USS:", memUSS)
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/basic/ECLAT.py` & `pami-2023.8.6.1/PAMI/frequentPattern/basic/ECLAT.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
             obj.startMine()
 
             frequentPatterns = obj.getPatterns()
 
             print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-            obj.savePatterns(oFile)
+            obj.save(oFile)
 
             Df = obj.getPatternInDataFrame()
 
             memUSS = obj.getMemoryUSS()
 
             print("Total Memory in USS:", memUSS)
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/basic/ECLATDiffset.py` & `pami-2023.8.6.1/PAMI/frequentPattern/basic/ECLATDiffset.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,14 +234,24 @@
         # for x, y in self._diffSets.items():
         #     print(x, y)
         uniqueItem.sort()
         # print()
         return uniqueItem
 
     def _runDeclat(self, candidateList):
+        """It will generate the combinations of frequent items
+
+                :param candidateList :it represents the items with their respective transaction identifiers
+
+                :type candidateList: list
+
+                :return: returning transaction dictionary
+
+                :rtype: dict
+                """
 
         newList = []
         for i in range(0, len(candidateList)):
             item1 = candidateList[i]
             iList = item1.split()
             for j in range(i + 1, len(candidateList)):
                 item2 = candidateList[j]
@@ -351,14 +361,16 @@
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
+        """ this function is used to print the results
+        """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/basic/ECLATbitset.py` & `pami-2023.8.6.1/PAMI/frequentPattern/basic/ECLATbitset.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
                 obj.startMine()
 
                 frequentPatterns = obj.getPatterns()
 
                 print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-                obj.savePatterns(oFile)
+                obj.save(oFile)
 
                 Df = obj.getPatternInDataFrame()
 
                 memUSS = obj.getMemoryUSS()
 
                 print("Total Memory in USS:", memUSS)
 
@@ -224,16 +224,23 @@
         frequentTidData = {k: v for k, v in tidData.items() if len(v) >= self._minSup}
         frequentTidData = dict(sorted(frequentTidData.items(), reverse=True, key=lambda x: len(x[1])))
         return frequentTidData
 
     def tidToBitset(self,itemset):
         """
         This function converts tid list to bitset.
-        :param itemset:
-        :return:
+
+        Parameters:
+        ----------
+            itemSet: frequent itemset that generated
+
+        Returns:
+        -------
+            patterns with original item names.
+
         """
         bitset = {}
 
         for k,v in itemset.items():
             bitset[k] = 0b1
             bitset[k] = (bitset[k] << int(v[0])) | 0b1
             for i in range(1,len(v)):
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/basic/FPGrowth.py` & `pami-2023.8.6.1/PAMI/frequentPattern/basic/FPGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,14 +597,16 @@
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self.__finalPatterns
     
     def printResults(self):
+        """ this function is used to print the results
+        """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/frequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/closed/CHARM.py` & `pami-2023.8.6.1/PAMI/frequentPattern/closed/CHARM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/closed/abstract.py` & `pami-2023.8.6.1/PAMI/frequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/cuda/abstract.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/cuda/cuApriori.py` & `pami-2023.8.6.1/PAMI/frequentPattern/cuda/cuApriori.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Apriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
+# cuApriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
 #
 #
 # **Importing this algorithm into a python program**
 # ----------------------------------------------------
 #
 #     import PAMI.frequentPattern.cuda.cuApriori as alg
 #
@@ -45,20 +45,20 @@
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 
-# from PAMI.frequentPattern.cuda import abstract as _ab
-import abstract as _ab
+from PAMI.frequentPattern.cuda import abstract as _ab
+# import abstract as _ab
 
 class cuApriori(_ab._frequentPatterns):
     """
-    :Description: Apriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
+    :Description: cuApriori is one of the fundamental algorithm to discover frequent patterns using Cuda in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
 
     :Reference:  Agrawal, R., Imieli ́nski, T., Swami, A.: Mining association rules between sets of items in large databases.
             In: SIGMOD. pp. 207–216 (1993), https://doi.org/10.1145/170035.170072
 
     :param  iFile: str :
                    Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
@@ -115,15 +115,15 @@
 
              obj.startMine()
 
              frequentPatterns = obj.getPatterns()
 
              print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-             obj.savePatterns(oFile)
+             obj.save(oFile)
 
              Df = obj.getPatternInDataFrame()
 
              memUSS = obj.getMemoryUSS()
 
              print("Total Memory in USS:", memUSS)
 
@@ -141,29 +141,42 @@
 
              The complete program was written by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
 
     """
 
     _ab._cp.cuda.Device(0).use()
 
-
-
     _minSup = float()
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
 
+    _sumKernel = _ab._cp.RawKernel(r'''
+
+    #define uint32_t unsigned int
 
+    extern "C" __global__
 
+    void sumKernel(uint32_t *d_a, uint32_t *sum, uint32_t numElements)
+    {
+        uint32_t i = blockDim.x * blockIdx.x + threadIdx.x;
+        if (i < numElements)
+        {  
+            atomicAdd(&sum[0], __popc(d_a[i]));
+        }
+        return;    
+    }
+
+    ''', 'sumKernel')
 
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
 
 
         """
@@ -214,81 +227,72 @@
         if type(value) is str:
             if '.' in value:
                 value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
-    
-    def _arraysAndItems(self):
-        """ 
-        Convert the items into arrays for cupy and store them in a dictionary variable
-
-        :return: dictionary variable
-        
-        """
-
 
+    def arraysAndItems(self):
         ArraysAndItems = {}
 
         for i in range(len(self._Database)):
             for j in self._Database[i]:
                 j = tuple([j])
                 if j not in ArraysAndItems:
                     ArraysAndItems[j] = [i]
                 else:
                     ArraysAndItems[j].append(i)
 
         newArraysAndItems = {}
 
-        for k,v in ArraysAndItems.items():
+        for k, v in ArraysAndItems.items():
             ArraysAndItems[k] = _ab._cp.array(v, dtype=_ab._np.uint32)
             if len(v) >= self._minSup:
                 self._finalPatterns[k] = len(v)
                 newArraysAndItems[k] = ArraysAndItems[k]
 
         return newArraysAndItems
 
-    
     def startMine(self):
         """
             Frequent pattern mining process will start from here
         """
         self._Database = []
         self._startTime = _ab._time.time()
         self._creatingItemSets()
         self._minSup = self._convert(self._minSup)
 
-        ArraysAndItems = self._arraysAndItems()
+        ArraysAndItems = self.arraysAndItems()
 
         while len(ArraysAndItems) > 0:
             # print("Total number of ArraysAndItems:", len(ArraysAndItems))
             newArraysAndItems = {}
             keys = list(ArraysAndItems.keys())
             for i in range(len(ArraysAndItems)):
                 # print(i, "/", len(ArraysAndItems), end="\r")
                 iList = list(keys[i])
-                for j in range(i+1, len(ArraysAndItems)):
+                for j in range(i + 1, len(ArraysAndItems)):
                     jList = list(keys[j])
                     union = tuple(sorted(set(iList + jList)))
-                    intersect = _ab._cp.intersect1d(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]], assume_unique=True)
+                    intersect = _ab._cp.intersect1d(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]],
+                                                    assume_unique=True)
                     if len(intersect) >= self._minSup and union not in self._finalPatterns:
                         newArraysAndItems[union] = intersect
                         self._finalPatterns[union] = len(intersect)
             ArraysAndItems = newArraysAndItems
             # print()
 
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
         print("Frequent patterns were generated successfully using cuApriori algorithm ")
-            
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
 
         :rtype: float
@@ -359,15 +363,14 @@
         this function is used to print results
         """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in s:", self.getRuntime())
 
-
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
             _ap = cuApriori(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
             _ap = cuApriori(_ab._sys.argv[1], _ab._sys.argv[3])
@@ -377,15 +380,9 @@
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in s:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
 
 
-    _ap = cuApriori("/home/tarun/PAMI/PAMI/frequentPattern/cuda/test.txt", 2, " ")
-    _ap = cuApriori("/home/tarun/Transactional_T10I4D100K.csv", 450, "\t")
-    _ap.startMine()
-    print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
-    print("Total Memory in USS:", _ap.getMemoryUSS())
-    print("Total Memory in RSS", _ap.getMemoryRSS())
-    print("Total ExecutionTime in s:", _ap.getRuntime())
+
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/cuda/cuAprioriBit.py` & `pami-2023.8.6.1/PAMI/frequentPattern/cuda/cuAprioriBit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Apriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
+# cuAprioriBit is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
 #
 #
 # **Importing this algorithm into a python program**
 # ----------------------------------------------------
 #
 #     import PAMI.frequentPattern.cuda.cuAprioriBit as alg
 #
@@ -44,21 +44,21 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-
 # from PAMI.frequentPattern.cuda import abstract as _ab
 import abstract as _ab
 
+
 class cuAprioriBit(_ab._frequentPatterns):
     """
-    :Description: Apriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
+    :Description: cuAprioriBit is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
 
     :Reference:  Agrawal, R., Imieli ́nski, T., Swami, A.: Mining association rules between sets of items in large databases.
             In: SIGMOD. pp. 207–216 (1993), https://doi.org/10.1145/170035.170072
 
     :param  iFile: str :
                    Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
@@ -115,15 +115,15 @@
 
              obj.startMine()
 
              frequentPatterns = obj.getPatterns()
 
              print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-             obj.savePatterns(oFile)
+             obj.save(oFile)
 
              Df = obj.getPatternInDataFrame()
 
              memUSS = obj.getMemoryUSS()
 
              print("Total Memory in USS:", memUSS)
 
@@ -139,15 +139,14 @@
     **Credits:**
     -------------
 
              The complete program was written by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
 
     """
 
-
     _minSup = float()
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
@@ -169,18 +168,14 @@
             atomicAdd(&sum[0], __popc(d_a[i]));
         }
         return;    
     }
 
     ''', 'sumKernel')
 
-
-
-
-
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
 
 
         """
         self._Database = []
@@ -230,52 +225,50 @@
         if type(value) is str:
             if '.' in value:
                 value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
-    
+
     def arraysAndItems(self):
         ArraysAndItems = {}
 
         for i in range(len(self._Database)):
             for j in self._Database[i]:
                 j = tuple([j])
                 if j not in ArraysAndItems:
                     ArraysAndItems[j] = [i]
                 else:
                     ArraysAndItems[j].append(i)
 
         newArraysAndItems = {}
 
-        for k,v in ArraysAndItems.items():
+        for k, v in ArraysAndItems.items():
             ArraysAndItems[k] = _ab._np.array(v, dtype=_ab._np.uint32)
             if len(v) >= self._minSup:
                 self._finalPatterns[k] = len(v)
                 newArraysAndItems[k] = ArraysAndItems[k]
 
         return newArraysAndItems
-    
+
     def createBitRepresentation(self, ArraysAndItems):
         bitRep = {}
         arraySize = len(self._Database) // 32 + 1 if len(self._Database) % 32 != 0 else len(self._Database) // 32
 
-
         for k, v in ArraysAndItems.items():
             bitRep[k] = _ab._np.zeros(arraySize, dtype=_ab._np.uint32)
             for i in v:
                 bitRep[k][i // 32] |= 1 << 31 - (i % 32)
 
         for k, v in bitRep.items():
             bitRep[k] = _ab._cp.array(v)
 
         return bitRep
 
-    
     def startMine(self):
         """
             Frequent pattern mining process will start from here
         """
         self._Database = []
         self._startTime = _ab._time.time()
         self._creatingItemSets()
@@ -287,18 +280,19 @@
         while len(ArraysAndItems) > 0:
             # print("Total number of ArraysAndItems:", len(ArraysAndItems))
             newArraysAndItems = {}
             keys = list(ArraysAndItems.keys())
             for i in range(len(ArraysAndItems)):
                 # print(i, "/", len(ArraysAndItems), end="\r")
                 iList = list(keys[i])
-                for j in range(i+1, len(ArraysAndItems)):   
+                for j in range(i + 1, len(ArraysAndItems)):
                     unionData = _ab._cp.bitwise_and(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]])
                     sum = _ab._cp.zeros(1, dtype=_ab._np.uint32)
-                    self._sumKernel((len(unionData) // 32 + 1,), (32,), (unionData, sum, _ab._cp.uint32(len(unionData))))
+                    self._sumKernel((len(unionData) // 32 + 1,), (32,),
+                                    (unionData, sum, _ab._cp.uint32(len(unionData))))
                     sum = sum[0]
                     jList = list(keys[j])
                     union = tuple(sorted(set(iList + jList)))
                     if sum >= self._minSup and union not in self._finalPatterns:
                         newArraysAndItems[union] = unionData
                         string = "\t".join(union)
                         self._finalPatterns[string] = sum
@@ -308,15 +302,14 @@
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
         print("Frequent patterns were generated successfully using cuAprioriBit algorithm ")
-            
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
 
         :rtype: float
@@ -379,21 +372,23 @@
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        """this function is used to print the result"""
+        """this function is used to print the result
+        """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:", self.getRuntime())
 
 
+
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
             _ap = cuAprioriBit(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
             _ap = cuAprioriBit(_ab._sys.argv[1], _ab._sys.argv[3])
@@ -402,14 +397,8 @@
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
 
-    _ap = cuAprioriBit("/home/tarun/Transactional_T10I4D100K.csv", 450, "\t")
-    _ap.startMine()
-    print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
-    _ap.save(_ab._sys.argv[2])
-    print("Total Memory in USS:", _ap.getMemoryUSS())
-    print("Total Memory in RSS", _ap.getMemoryRSS())
-    print("Total ExecutionTime in s:", _ap.getRuntime())
+
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/cuda/cuEclat.py` & `pami-2023.8.6.1/PAMI/frequentPattern/cuda/cuEclat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
+# cuECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 #
 #
 # **Importing this algorithm into a python program**
 # ----------------------------------------------------
 #
 #     import PAMI.frequentPattern.cuda.cuEclat as alg
 #
@@ -10,15 +10,15 @@
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.savePatterns(oFile)
+#     obj.save(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -115,15 +115,15 @@
 
              obj.startMine()
 
              frequentPatterns = obj.getPatterns()
 
              print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-             obj.savePatterns(oFile)
+             obj.save(oFile)
 
              Df = obj.getPatternInDataFrame()
 
              memUSS = obj.getMemoryUSS()
 
              print("Total Memory in USS:", memUSS)
 
@@ -377,15 +377,9 @@
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in s:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
 
 
-    _ap = cuEclat("/home/tarun/PAMI/PAMI/frequentPattern/cuda/test.txt", 2, " ")
-    _ap = cuEclat("/home/tarun/Transactional_T10I4D100K.csv", 450, "\t")
-    _ap.startMine()
-    print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
-    print("Total Memory in USS:", _ap.getMemoryUSS())
-    print("Total Memory in RSS", _ap.getMemoryRSS())
-    print("Total ExecutionTime in s:", _ap.getRuntime())
+
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/cuda/cuEclatBit.py` & `pami-2023.8.6.1/PAMI/frequentPattern/cuda/cuEclatBit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
+# cuECLATBit is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 #
 #
 # **Importing this algorithm into a python program**
 # ----------------------------------------------------
 #
 #     import PAMI.frequentPattern.cuda.cuEclatBit as alg
 #
@@ -115,15 +115,15 @@
 
              obj.startMine()
 
              frequentPatterns = obj.getPatterns()
 
              print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-             obj.savePatterns(oFile)
+             obj.save(oFile)
 
              Df = obj.getPatternInDataFrame()
 
              memUSS = obj.getMemoryUSS()
 
              print("Total Memory in USS:", memUSS)
 
@@ -408,14 +408,15 @@
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
 
-    _ap = cuEclatBit("/home/tarun/Transactional_T10I4D100K.csv", 450, "\t")
+"""_ap = cuEclat("/home/tarun/PAMI/PAMI/frequentPattern/cuda/test.txt", 2, " ")
+    _ap = cuEclat("/home/tarun/Transactional_T10I4D100K.csv", 450, "\t")
     _ap.startMine()
     print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
-    _ap.save(_ab._sys.argv[2])
     print("Total Memory in USS:", _ap.getMemoryUSS())
     print("Total Memory in RSS", _ap.getMemoryRSS())
-    print("Total ExecutionTime in s:", _ap.getRuntime())
+    print("Total ExecutionTime in s:", _ap.getRuntime())"""
+
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py` & `pami-2023.8.6.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# Apriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
-#
+# cudaAprioriGCT is one of the fundamental algorithm to discover frequent patterns using CUDA in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
 #
+
 # **Importing this algorithm into a python program**
 # ----------------------------------------------------
 #
-#     import PAMI.frequentPattern.cuda.cuAprioriBit as alg
+#     import PAMI.frequentPattern.cuda.cudaAprioriGCT as alg
 #
-#     obj = alg.cuAprioriBit(iFile, minSup)
+#     obj = alg.cuAprioriGCT(iFile, minSup)
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
@@ -44,44 +44,42 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-
-
+from PAMI.frequentPattern.basic import abstract as _ab
+# import abstract as _ab
 
 import os
 import csv
 import time
 import numpy as np
 import pycuda.gpuarray as gpuarray
 import pycuda.autoinit
 import psutil
 
 
-class cudaAprioriGCT:
+class cudaAprioriGCT(_ab._frequentPatterns):
     """
-        :Description: Apriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
+        :Description: cudaAprioriGCT is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
 
         :Reference:  Agrawal, R., Imieli ́nski, T., Swami, A.: Mining association rules between sets of items in large databases.
                 In: SIGMOD. pp. 207–216 (1993), https://doi.org/10.1145/170035.170072
 
         :param  iFile: str :
                        Name of the Input file to mine complete set of frequent patterns
         :param  oFile: str :
                        Name of the output file to store complete set of frequent patterns
         :param  minSup: int :
                        The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count. Otherwise, it will be treated as float.
         :param  sep: str :
                        This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
-
-
         :Attributes:
 
             startTime : float
               To record the start time of the mining process
 
             endTime : float
               To record the completion time of the mining process
@@ -113,25 +111,25 @@
 
 
         **Importing this algorithm into a python program**
         ----------------------------------------------------
 
         .. code-block:: python
 
-                 import PAMI.frequentPattern.cuda.cuAprioriBit as alg
+                 import PAMI.frequentPattern.cuda.cuAprioriGCT as alg
 
-                 obj = alg.cuAprioriBit(iFile, minSup)
+                 obj = alg.cuAprioriGCT(iFile, minSup)
 
                  obj.startMine()
 
                  frequentPatterns = obj.getPatterns()
 
                  print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-                 obj.savePatterns(oFile)
+                 obj.save(oFile)
 
                  Df = obj.getPatternInDataFrame()
 
                  memUSS = obj.getMemoryUSS()
 
                  print("Total Memory in USS:", memUSS)
 
@@ -151,186 +149,245 @@
 
         """
 
     __time = 0
     __memRSS = 0
     __memUSS = 0
     __GPU_MEM = 0
-    filePath = ""
-    sep = ""
-    minSup = 0
-    Patterns = {}
-
-    def __init__(self, filePath, sep, minSup):
-        self.filePath = filePath
-        self.sep = sep
-        self.minSup = minSup
+    _minSup = 0
+    _finalPatterns = {}
+
+    def __init__(self, filePath, minSup, sep):
+        self._iFile = filePath
+        self._sep = sep
+        self._minSup = minSup
         self.__time = 0
         self.__memRSS = 0
         self.__memUSS = 0
 
-    def read_data(self, data_path, sep):
+    def __creatingItemSets(self):
         """
-        param data_path:
-        type data_path:
-        param sep:
-        type sep:
+            Storing the complete transactions of the database/input file in a database variable
+
+
         """
-        data = []
-        if not os.path.isfile(data_path):
-            raise ValueError('Invalid data path.' + data_path)
-        with open(data_path, 'r') as f:
-            file = csv.reader(f, delimiter=sep, quotechar='\r')
-            lineNo = 1
-            for row in file:
-                data.append([str(item) for item in row if item != ''])
-                lineNo += 1
-        return data, lineNo
-
-    def write_result(self, result, result_path):
-        """
-        param result:
-        type result:
-        param result_path:
-        type result_path:
-        """
-        file = open(result_path, 'w')
-        for itemset, support in result.items():
-            file.write(str(itemset) + ' : ' + str(support) + '\n')
-        file.close()
+        self.__Database = []
+        if isinstance(self._iFile, _ab._pd.DataFrame):
+            if self._iFile.empty:
+                print("its empty..")
+            i = self._iFile.columns.values.tolist()
+            if 'Transactions' in i:
+                self.__Database = self._iFile['Transactions'].tolist()
+
+            # print(self.Database)
+        if isinstance(self._iFile, str):
+            if _ab._validators.url(self._iFile):
+                data = _ab._urlopen(self._iFile)
+                for line in data:
+                    line.strip()
+                    line = line.decode("utf-8")
+                    temp = [i.rstrip() for i in line.split(self._sep)]
+                    temp = [x for x in temp if x]
+                    self.__Database.append(temp)
+            else:
+                try:
+                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                        for line in f:
+                            line = line.strip()
+                            temp = [i.rstrip() for i in line.split(self._sep)]
+                            temp = [x for x in temp if x]
+                            self.__Database.append(temp)
+                except IOError:
+                    print("File Not Found")
+                    quit()
+
+    def __convert(self, value):
+        """
+        to convert the type of user specified minSup value
+
+        :param value: user specified minSup value
+
+        :return: converted type
+        """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self.__Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (len(self.__Database) * value)
+            else:
+                value = int(value)
+        return value
 
-    def compute_vertical_bitvector_data(self, data):
+    def compute_vertical_bitvector_data(self):
         """
-        param data:
-        type data:
+        Converting database into bit vector
 
         """
-        #---build item to idx mapping---#
+        # ---build item to idx mapping---#
         idx = 0
         item2idx = {}
-        for transaction in data:
+        for transaction in self.__Database:
             for item in transaction:
                 if not item in item2idx:
                     item2idx[item] = idx
                     idx += 1
         idx2item = {idx: str(int(item)) for item, idx in item2idx.items()}
-        #---build vertical data---#
-        vb_data = np.zeros((len(item2idx), len(data)), dtype=np.uint16)
-        for trans_id, transaction in enumerate(data):
+        # ---build vertical data---#
+        vb_data = np.zeros((len(item2idx), len(self.__Database)), dtype=np.uint16)
+        for trans_id, transaction in enumerate(self.__Database):
             for item in transaction:
                 vb_data[item2idx[item], trans_id] = 1
         vb_data = gpuarray.to_gpu(vb_data.astype(np.uint16))
         return vb_data, idx2item
 
-    def getTime(self):
+    def getRuntime(self):
         """Calculating the total amount of time taken by the mining process
-        :return: returning total amount of runtime taken by the mining process
-        :rtype: float
+            :return: returning total amount of runtime taken by the mining process
+            :rtype: float
          """
         return self.__time
 
-    def getMEMORYRSS(self):
+    def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
-
-                    :return: returning RSS memory consumed by the mining process
-
-                    :rtype: float
+            :return: returning RSS memory consumed by the mining process
+            :rtype: float
         """
 
-
         return self.__memRSS
 
-    def getMEMORYUSS(self):
+    def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
-
-                        :return: returning USS memory consumed by the mining process
-
-                        :rtype: float
-                        """
+            :return: returning USS memory consumed by the mining process
+            :rtype: float
+        """
         return self.__memUSS
 
     def getGPUMemory(self):
+        """
+        To calculate the total memory consumed by GPU
+        :return: return GPU memory
+        :rtype: int
+        """
 
         return self.__GPU_MEM
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
+            :return: returning frequent patterns
+            :rtype: dict
+        """
+        return self._finalPatterns
 
-                        :return: returning frequent patterns
+    def get_numberOfPatterns(self):
+        return len(self._finalPatterns)
 
-                        :rtype: dict
-                        """
-        return self.Patterns
+    def getPatternsAsDataFrame(self):
+        """Storing final frequent patterns in a dataframe
+        :return: returning frequent patterns in a dataframe
+        :rtype: pd.DataFrame
+        """
 
-    def get_numberOfPatterns(self):
-        return len(self.Patterns)
+        dataFrame = {}
+        data = []
+        for a, b in self._finalPatterns.items():
+            data.append([a, b])
+            dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+        return dataFrame
+
+    def save(self, outFile):
+        """
+        Complete set of frequent patterns will be loaded in to an output file
+        :param outFile: name of the output file
+        :type outFile: file
+        """
+        self._oFile = outFile
+        writer = open(self._oFile, 'w+')
+        for x, y in self._finalPatterns.items():
+            if type(x) == tuple:
+                pattern = ""
+                for item in x:
+                    pattern = pattern + str(item) + " "
+                s1 = pattern + ":" + str(y)
+            else:
+                s1 = str(x) + ":" + str(y)
+            writer.write("%s \n" % s1)
 
     def startMine(self):
         """
             Frequent pattern mining process will start from here
         """
         startTime = time.time()
         basePattern = {}
         final = {}
 
-        data, lineNo = self.read_data(self.filePath, self.sep)
-        vb_data, idx2item = self.compute_vertical_bitvector_data(data)
-        if self.minSup < 1:
-            self.minSup = int(lineNo * self.minSup)
+        self.__creatingItemSets()
+        self._minSup = self.__convert(self._minSup)
+        minSup = self._minSup
+        vb_data, idx2item = self.compute_vertical_bitvector_data()
 
         for i in range(len(vb_data)):
-            if gpuarray.sum(vb_data[i]).get() >= self.minSup:
+            if gpuarray.sum(vb_data[i]).get() >= self._minSup:
                 basePattern[idx2item[i]] = [i]
                 final[idx2item[i]] = gpuarray.sum(vb_data[i]).get()
 
         while len(basePattern) > 0:
             temp = {}
             keysList = list(basePattern.keys())
             valuesList = list(basePattern.values())
-            for i in range(len(basePattern)-1):
+            for i in range(len(basePattern) - 1):
                 keyI = keysList[i].split(" ")
                 keyI = [int(x) for x in keyI]
 
-                for j in range(i+1, len(basePattern)):
+                for j in range(i + 1, len(basePattern)):
                     keyJ = keysList[j].split(" ")
                     keyJ = [int(x) for x in keyJ]
                     values = set(valuesList[i])
                     for val in valuesList[j]:
                         values.add(val)
                     values = list(sorted(values))
                     totalArray = vb_data[values[0]]
                     for k in range(1, len(values)):
                         totalArray = totalArray.__mul__(vb_data[values[k]])
                     support = gpuarray.sum(totalArray).get()
-                    if support >= self.minSup:
+                    if support >= self._minSup:
                         combinedKey = " ".join(
                             str(x) for x in sorted(set(keyI) | set(keyJ)))
                         temp[combinedKey] = values
                         final[str(combinedKey)] = support
             basePattern = temp
 
         self.__time = time.time() - startTime
         self.__memRSS = psutil.Process(os.getpid()).memory_info().rss
         self.__memUSS = psutil.Process(os.getpid()).memory_full_info().uss
-        self.Patterns = final
+        self._finalPatterns = final
         self.__GPU_MEM = vb_data.nbytes
 
-    def printStats(self):
+    def printResults(self):
         """ this function is used to print the results
         """
         print("Total number of Coverage Patterns:", len(self.getPatterns()))
+        print("GPU MEM: ", _ap.getGPUMemory())
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:",  self.getRuntime())
+        print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
-    filePath = "datasets\\transactional_T10I4D100K.csv"
-    sep = "\t"
-    support = 500
-    cudaAprioriGCT = cudaAprioriGCT(filePath, sep, support)
-    cudaAprioriGCT.startMine()
-    print("Time: ", cudaAprioriGCT.get_time())
-    print("Memory RSS: ", cudaAprioriGCT.get_memRSS())
-    print("Memory USS: ", cudaAprioriGCT.get_memUSS())
-    print("GPU MEM: ", cudaAprioriGCT.get_GPU_MEM())
-    print("Patterns: ", cudaAprioriGCT.get_numberOfPatterns())
+    _ap = str()
+    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
+        if len(_ab._sys.argv) == 5:
+            _ap = cudaAprioriGCT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+        if len(_ab._sys.argv) == 4:
+            _ap = cudaAprioriGCT(_ab._sys.argv[1], _ab._sys.argv[3])
+        _ap.startMine()
+        print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
+        _ap.save(_ab._sys.argv[2])
+        print("Total Memory in USS:", _ap.getMemoryUSS())
+        print("Total Memory in RSS", _ap.getMemoryRSS())
+        print("GPU MEM: ", _ap.getGPUMemory())
+        print("Total ExecutionTime in ms:", _ap.getRuntime())
+    else:
+        print("Error! The number of input parameters do not match the total number of parameters provided")
+
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py` & `pami-2023.8.6.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Apriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
+# cudaAprioriTID is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
 #
 #
 # **Importing this algorithm into a python program**
 # ----------------------------------------------------
 #
 #     import PAMI.frequentPattern.cuda.cuAprioriBit as alg
 #
@@ -46,21 +46,21 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 
 
-
+import abstract as _ab
 
 import os
 import csv
 import time
 import numpy as np
-import pycuda.gpuarray as gpuarray
+import pycuda.gpuarray as _gpuarray
 import pycuda.autoinit
 import psutil
 import pycuda.driver as cuda
 from pycuda.compiler import SourceModule
 import pycuda
 
 deviceIntersection = SourceModule("""
@@ -152,15 +152,15 @@
 
              obj.startMine()
 
              frequentPatterns = obj.getPatterns()
 
              print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-             obj.savePatterns(oFile)
+             obj.save(oFile)
 
              Df = obj.getPatternInDataFrame()
 
              memUSS = obj.getMemoryUSS()
 
              print("Total Memory in USS:", memUSS)
 
@@ -181,37 +181,104 @@
     """
 
     __time = 0
     __memRSS = 0
     __memUSS = 0
     __GPU_MEM = 0
     filePath = ""
-    sep = ""
-    minSup = 0
+    _iFile = " "
+    _sep = ""
+    _minSup = 0
     Patterns = {}
 
     def __init__(self, filePath, sep, minSup):
         self.filePath = filePath
         self.sep = sep
         self.minSup = minSup
         self.__time = 0
         self.__memRSS = 0
         self.__memUSS = 0
 
-    def _readFile(self, fileName, separator):
+    def _creatingItemSets(self):
+        """
+            Storing the complete transactions of the database/input file in a database variable
+
+
+        """
+        self._Database = {}
+        lineNumber = 1
+        if isinstance(self._iFile, _ab._pd.DataFrame):
+            temp = []
+            if self._iFile.empty:
+                print("its empty..")
+            i = self._iFile.columns.values.tolist()
+            if 'Transactions' in i:
+                temp = self._iFile['Transactions'].tolist()
+
+            for k in temp:
+                self._Database.append(set(k))
+        if isinstance(self._iFile, str):
+            if _ab._validators.url(self._iFile):
+                data = _ab._urlopen(self._iFile)
+                for line in data:
+                    line.strip()
+                    line = line.decode("utf-8")
+                    for i in range(len(line)):
+                        if line[i] in self._Database:
+                            self._Database[i].append(lineNumber)
+                        else:
+                            self._Database[i] = [lineNumber]
+                    lineNumber += 1
+
+                    temp = [i.rstrip() for i in line.split(self._sep)]
+                    temp = [x for x in temp if x]
+                    self._Database.append(set(temp))
+            else:
+                try:
+                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                        for line in f:
+                            line.strip()
+                            temp = [i.rstrip() for i in line.split(self._sep)]
+                            temp = [x for x in temp if x]
+                            self._Database.append(set(temp))
+                except IOError:
+                    print("File Not Found")
+                    quit()
+
+    def _convert(self, value):
+        """
+        to convert the type of user specified minSup value
+
+        :param value: user specified minSup value
+
+        :return: converted type
         """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (len(self._Database) * value)
+            else:
+                value = int(value)
+        return value
+
+    """def _readFile(self, fileName, separator):
+        
         Reads a file and stores the data in a dictionary
 
         Args:
             fileName: string
             separator: string
 
         Returns:
             dictionary: dictionary
-        """
+        
         file = open(fileName, 'r')
         dictionary = {}
         lineNumber = 1
         for line in file:
             line = line.strip()
             line = line.split(separator)
             for i in range(len(line)):
@@ -221,71 +288,76 @@
                     dictionary[line[i]] = [lineNumber]
             lineNumber += 1
 
         # sort dictionary by size of values
         dictionary = dict(
             sorted(dictionary.items(), key=lambda x: len(x[1]), reverse=True))
         return dictionary, lineNumber
-
-    def get_time(self):
+        """
+    def getRuntime(self):
         """Calculating the total amount of time taken by the mining process
 
                 :return: returning total amount of runtime taken by the mining process
 
                 :rtype: float
                 """
 
         return self.__time
 
-    def get_memRSS(self):
+    def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
                 :return: returning RSS memory consumed by the mining process
 
                 :rtype: float
                 """
         return self.__memRSS
 
-    def get_memUSS(self):
+    def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
                 :return: returning USS memory consumed by the mining process
 
                 :rtype: float
                 """
         return self.__memUSS
 
-    def get_GPU_MEM(self):
+    def getGPUMemory(self):
+        """
+           To calculate the total memory consumed by GPU
+           :return: return GPU memory
+           :rtype: int
+        """
+
         return self.__GPU_MEM
 
-    def get_Patterns(self):
+    def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
-
-                :return: returning frequent patterns
-
-                :rtype: dict
-                """
+               :return: returning frequent patterns
+               :rtype: dict
+        """
         return self.Patterns
 
     def get_numberOfPatterns(self):
         return len(self.Patterns)
 
     def startMine(self):
         """
                    Frequent pattern mining process will start from here
                """
         dev_Intersection = deviceIntersection.get_function("intersection")
         startTime = time.time()
         final = {}
 
-        data, lineNo = self._readFile(self.filePath, self.sep)
-        if self.minSup < 1:
-            self.minSup = int(lineNo * self.minSup)
+        self._creatingItemSets()
+        self._minSup = self._convert(self._minSup)
+        minSup = self._minSup
 
-        data = dict(filter(lambda x: len(x[1]) >= self.minSup, data.items()))
+
+        data = dict(filter(lambda x: len(x[1]) >= self.minSup, self._Database()))
         for key, value in data.items():
             final[key] = len(value)
 
         while len(data) > 1:
             # sort data by size of values
             data = dict(
                 sorted(data.items(), key=lambda x: len(x[1]), reverse=True))
@@ -382,17 +454,24 @@
         self.__time = time.time() - startTime
         self.__memRSS = psutil.Process(os.getpid()).memory_info().rss
         self.__memUSS = psutil.Process(os.getpid()).memory_full_info().uss
         self.Patterns = final
 
 
 if __name__ == "__main__":
-    filePath = "datasets\\transactional_T10I4D100K.csv"
-    sep = "\t"
-    support = 500
-    cudaAprioriTID = cudaAprioriTID(filePath, sep, support)
-    cudaAprioriTID.startMine()
-    print("Time: ", cudaAprioriTID.get_time())
-    print("Memory RSS: ", cudaAprioriTID.get_memRSS())
-    print("Memory USS: ", cudaAprioriTID.get_memUSS())
-    print("GPU MEM: ", cudaAprioriTID.get_GPU_MEM())
-    print("Patterns: ", cudaAprioriTID.get_numberOfPatterns())
+    _ap = str()
+    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
+        if len(_ab._sys.argv) == 5:
+            _ap = cudaAprioriTID(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+        if len(_ab._sys.argv) == 4:
+            _ap = cudaAprioriTID(_ab._sys.argv[1], _ab._sys.argv[3])
+        _ap.startMine()
+        print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
+        _ap.save(_ab._sys.argv[2])
+        print("Total Memory in USS:", _ap.getMemoryUSS())
+        print("Total Memory in RSS", _ap.getMemoryRSS())
+        print("GPU MEM: ", _ap.getGPUMemory())
+        print("Total ExecutionTime in ms:", _ap.getRuntime())
+    else:
+        print("Error! The number of input parameters do not match the total number of parameters provided")
+
+
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py` & `pami-2023.8.6.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+# cudaEclatGCT is one of the fundamental algorithm to discover frequent patterns in a transactional database. It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It  employs downward closure property to  reduce the search space effectively.
+#
+# **Importing this algorithm into a python program**
+# --------------------------------------------------------
+#
+#     from PAMI.frequentPattern.cuda.cudaEclatGCT as alg
+#
+#     obj = alg.FPGrowth(iFile, minSup)
+#
+#     obj.startMine()
+#
+#     frequentPatterns = obj.getPatterns()
+#
+#     print("Total number of Frequent Patterns:", len(frequentPatterns))
+#
+#     obj.save(oFile)
+#
+#     Df = obj.getPatternInDataFrame()
+#
+#     memUSS = obj.getMemoryUSS()
+#
+#     print("Total Memory in USS:", memUSS)
+#
+#     memRSS = obj.getMemoryRSS()
+#
+#     print("Total Memory in RSS", memRSS)
+#
+#     run = obj.getRuntime()
+#
+#     print("Total ExecutionTime in seconds:", run)
 #
 #
 #
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
@@ -14,19 +44,24 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
+from PAMI.frequentPattern.basic import abstract as _ab
+
+minSup = str()
+_ab._sys.setrecursionlimit(20000)
+
 import os
 import csv
 import time
 import numpy as np
-import pycuda.gpuarray as gpuarray
+import pycuda.gpuarray as _gpuarray
 import pycuda.autoinit
 import psutil
 
 
 class cudaEclatGCT:
     """
             :Description: Apriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
@@ -113,133 +148,173 @@
 
             **Credits:**
             -------------
 
                      The complete program was written by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
 
             """
-    
+
     __time = 0
     __memRSS = 0
     __memUSS = 0
     __GPU_MEM = 0
-    filePath = ""
-    sep = ""
-    minSup = 0
-    Patterns = {}
-
-    def __init__(self, filePath, sep, minSup):
-        self.filePath = filePath
-        self.sep = sep
-        self.minSup = minSup
+    _minSup = 0
+    _finalPatterns = {}
+
+    def __init__(self, filePath, minSup, sep):
+        self._iFile = filePath
+        self._sep = sep
+        self._minSup = minSup
         self.__time = 0
         self.__memRSS = 0
         self.__memUSS = 0
 
-    def read_data(self, data_path, sep):
-        """
-                param data_path:
-                type data_path:
-                param sep:
-                type sep:
-                """
+    """def read_data(self, data_path, sep):
+
+
         data = []
         if not os.path.isfile(data_path):
             raise ValueError('Invalid data path.' + data_path)
         with open(data_path, 'r') as f:
             file = csv.reader(f, delimiter=sep, quotechar='\r')
             lineNo = 1
             for row in file:
                 data.append([str(item) for item in row if item != ''])
                 lineNo += 1
-        return data, lineNo
+        return data, lineNo"""
 
-    def write_result(self, result, result_path):
+    def __creatingItemSets(self):
+        """
+            Storing the complete transactions of the database/input file in a database variable
         """
-                param result:
-                type result:
-                param result_path:
-                type result_path:
-                """
-        file = open(result_path, 'w')
-        for itemset, support in result.items():
-            file.write(str(itemset) + ' : ' + str(support) + '\n')
-        file.close()
+        self.__Database = []
+        if isinstance(self._iFile, _ab._pd.DataFrame):
+            if self._iFile.empty:
+                print("its empty..")
+            i = self._iFile.columns.values.tolist()
+            if 'Transactions' in i:
+                self.__Database = self._iFile['Transactions'].tolist()
+
+            # print(self.Database)
+        if isinstance(self._iFile, str):
+            if _ab._validators.url(self._iFile):
+                data = _ab._urlopen(self._iFile)
+                for line in data:
+                    line.strip()
+                    line = line.decode("utf-8")
+                    temp = [i.rstrip() for i in line.split(self._sep)]
+                    temp = [x for x in temp if x]
+                    self.__Database.append(temp)
+            else:
+                try:
+                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                        for line in f:
+                            line = line.strip()
+                            temp = [i.rstrip() for i in line.split(self._sep)]
+                            temp = [x for x in temp if x]
+                            self.__Database.append(temp)
+                except IOError:
+                    print("File Not Found")
+                    quit()
 
-    def compute_vertical_bitvector_data(self, data):
+    def __convert(self, value):
         """
-                param data:
-                type data:
+        to convert the type of user specified minSup value
 
-                """
-        #---build item to idx mapping---#
+        :param value: user specified minSup value
+
+        :return: converted type
+        """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self.__Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (len(self.__Database) * value)
+            else:
+                value = int(value)
+        return value
+
+    def compute_vertical_bitvector_data(self):
+        """
+            converting  database into bit vector
+        """
+        # ---build item to idx mapping---#
         idx = 0
         item2idx = {}
-        for transaction in data:
+        for transaction in self.__Database:
             for item in transaction:
                 if not item in item2idx:
                     item2idx[item] = idx
                     idx += 1
         idx2item = {idx: str(int(item)) for item, idx in item2idx.items()}
-        #---build vertical data---#
-        vb_data = np.zeros((len(item2idx), len(data)), dtype=np.uint16)
-        for trans_id, transaction in enumerate(data):
+        # ---build vertical data---#
+        vb_data = np.zeros((len(item2idx), len(self.__Database)), dtype=np.uint16)
+        for trans_id, transaction in enumerate(self.__Database):
             for item in transaction:
                 vb_data[item2idx[item], trans_id] = 1
-        vb_data = gpuarray.to_gpu(vb_data.astype(np.uint16))
+        vb_data = _gpuarray.to_gpu(vb_data.astype(np.uint16))
         return vb_data, idx2item
 
-    def get_time(self):
+    def getRuntime(self):
         """Calculating the total amount of time taken by the mining process
                 :return: returning total amount of runtime taken by the mining process
                 :rtype: float
         """
         return self.__time
 
-    def get_memRSS(self):
+    def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
-
-                            :return: returning RSS memory consumed by the mining process
-
-                            :rtype: float
+               :return: returning RSS memory consumed by the mining process
+               :rtype: float
         """
         return self.__memRSS
 
-    def get_memUSS(self):
+    def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
-
              :return: returning USS memory consumed by the mining process
-
              :rtype: float
         """
         return self.__memUSS
 
-    def get_GPU_MEM(self):
+    def getGPUMemory(self):
+        """
+        To calculate the total memory consumed by GPU
+        :return: return GPU memory
+        :rtype: int
+        """
 
         return self.__GPU_MEM
 
-    def get_Patterns(self):
+    def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
 
                 :return: returning frequent patterns
 
                 :rtype: dict
         """
-        return self.Patterns
+        return self._finalPatterns
 
     def get_numberOfPatterns(self):
-        return len(self.Patterns)
+
+        return len(self._finalPatterns)
 
     def eclat(self, basePattern, final, vb_data, idx2item, item2idx):
         """ param basePattern:
             type basePattern:
             param final:
             type final:
             param vb_data:
             type vb_data:
+            param dx2item:
+            type dx2item:
+            param item2idx:
+            type item2idx:
 
         """
         newBasePattern = []
         for i in range(0, len(basePattern)):
             item1 = basePattern[i]
             i1_list = item1.split()
             for j in range(i + 1, len(basePattern)):
@@ -250,55 +325,59 @@
                     unionOfKey.sort()
                     valueList = []
                     for key in unionOfKey:
                         valueList.append(item2idx[key])
                     total = vb_data[valueList[0]]
                     for k in range(1, len(valueList)):
                         total = total.__mul__(vb_data[valueList[k]])
-                    support = gpuarray.sum(total).get()
-                    if support >= self.minSup:
+                    support = _gpuarray.sum(total).get()
+                    if support >= self._minSup:
                         newBasePattern.append(" ".join(unionOfKey))
                         final[" ".join(unionOfKey)] = support
 
         if len(newBasePattern) > 0:
             self.eclat(newBasePattern, final, vb_data, idx2item, item2idx)
 
     def startMine(self):
         """
-                    Frequent pattern mining process will start from here
+          Frequent pattern mining process will start from here
         """
         startTime = time.time()
         basePattern = []
         final = {}
 
-        data, lineNo = self.read_data(self.filePath, self.sep)
-        vb_data, idx2item = self.compute_vertical_bitvector_data(data)
-        if self.minSup < 1:
-            self.minSup = int(lineNo * self.minSup)
+        self.__creatingItemSets()
+        self._minSup = self.__convert(self._minSup)
+        minSup = self._minSup
+        vb_data, idx2item = self.compute_vertical_bitvector_data()
 
         for i in range(len(vb_data)):
-            if gpuarray.sum(vb_data[i]).get() >= self.minSup:
+            if _gpuarray.sum(vb_data[i]).get() >= self._minSup:
                 basePattern.append(idx2item[i])
-                final[idx2item[i]] = gpuarray.sum(vb_data[i]).get()
+                final[idx2item[i]] = _gpuarray.sum(vb_data[i]).get()
 
         # reverse idx2item
         item2idx = {idx2item[i]: i for i in idx2item}
         self.eclat(basePattern, final, vb_data, idx2item, item2idx)
         self.__time = time.time() - startTime
         self.__memRSS = psutil.Process(os.getpid()).memory_info().rss
         self.__memUSS = psutil.Process(os.getpid()).memory_full_info().uss
-        self.Patterns = final
+        self._finalPatterns = final
         self.__GPU_MEM = vb_data.nbytes
 
 
 if __name__ == "__main__":
-    filePath = "datasets\\transactional_T10I4D100K.csv"
-    # filePath = "file.txt"
-    sep = "\t"
-    support = 500
-    cudaEclatGCT = cudaEclatGCT(filePath, sep, support)
-    cudaEclatGCT.startMine()
-    print("Time: ", cudaEclatGCT.get_time())
-    print("Memory RSS: ", cudaEclatGCT.get_memRSS())
-    print("Memory USS: ", cudaEclatGCT.get_memUSS())
-    print("GPU MEM: ", cudaEclatGCT.get_GPU_MEM())
-    print("Patterns: ", cudaEclatGCT.get_numberOfPatterns())
+    _ap = str()
+    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
+        if len(_ab._sys.argv) == 5:
+            _ap = cudaEclatGCT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+        if len(_ab._sys.argv) == 4:
+            _ap = cudaEclatGCT(_ab._sys.argv[1], _ab._sys.argv[3])
+        _ap.startMine()
+        print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
+        _ap.save(_ap._sys.argv[2])
+        print("Total Memory in USS:", _ap.getMemoryUSS())
+        print("Total Memory in RSS", _ap.getMemoryRSS())
+        print("GPU MEM: ", _ap.getGPUMemory())
+        print("Total ExecutionTime in ms:", _ap.getRuntime())
+    else:
+        print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py` & `pami-2023.8.6.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
 #
 #
 
+
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -276,15 +277,15 @@
             for la in info:
                 tail.append(la)
             sub = head + tail
             if maximalTree.checkerSub(sub) == 1:
                 for pat in range(len(condPatterns)):
                     conditional_tree.addConditionalTransaction(condPatterns[pat], tids[pat])
                 if len(condPatterns) >= 1:
-                    conditional_tree.generatePatterns(pattern, patterns)
+                    conditional_tree.generatePatterns(pattern, patterns, maximalTree)
                 else:
                     maximalTree.addTransaction(pattern)
                     patterns[tuple(pattern)] = self.info[i]
             self.removeNode(i)
 
 
 class _MNode(object):
@@ -586,18 +587,18 @@
                 if tr[i] in oneLength:
                     list2.append(self._rank[tr[i]])
             if len(list2) >= 2:
                 list2.sort()
                 list1.append(list2)
         return list1
 
-    @staticmethod
-    def _buildTree(data, info):
+
+    def _buildTree(self, data, info):
         """
-        creating the root node as null in fp-tree and adding all transactions into tree.
+        creating the root node as null in fp-tree and and adding all transactions into tree.
         :param data: updated transactions
         :param info: rank of items in transactions
         :return: fp-tree
         """
         rootNode = _Tree()
         rootNode.info = info.copy()
         for i in range(len(data)):
@@ -654,16 +655,16 @@
         updatedTransactions = self._updateTransactions(generatedItems)
         for x, y in self._rank.items():
             self._rankdup[y] = x
         info = {self._rank[k]: v for k, v in generatedItems.items()}
         patterns = {}
         self._finalPatterns = {}
         self._maximalTree = _MPTree()
-        Tree = self._buildTree(updatedTransactions, info, self._maximalTree)
-        Tree.generatePatterns([], patterns)
+        Tree = self._buildTree(updatedTransactions, info)
+        Tree.generatePatterns([], patterns, self._maximalTree)
         for x, y in patterns.items():
             pattern = str()
             x = self._convertItems(x)
             for i in x:
                 pattern = pattern + i + "\t"
             self._finalPatterns[pattern] = y
         self._endTime = _ab._time.time()
@@ -716,15 +717,15 @@
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to an output file
+        """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
@@ -738,18 +739,14 @@
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
     
     def printResults(self):
-        """
-         this function is used to print the results
-
-        """
         print('Total number of Maximal Frequent Patterns: ' + str(self.getPatterns()))
         print('Runtime: ' + str(self.getRuntime()))
         print('Memory (RSS): ' + str(self.getMemoryRSS()))
         print('Memory (USS): ' + str(self.getMemoryUSS()))
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/maximal/__init__.py` & `pami-2023.8.6.1/PAMI/frequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/maximal/abstract.py` & `pami-2023.8.6.1/PAMI/frequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/pyspark/abstract.py` & `pami-2023.8.6.1/PAMI/frequentPattern/pyspark/abstract.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,16 +69,16 @@
         :param iFile: Input file name or path of the input file
         :type iFile: str or DataFrame
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
-        :param numWorkers: The user can specify numWorkers as the number of cores which are used.
-        :type numWorkers: int
+        :param numPartitions: The user can specify numWorkers as the number of cores which are used.
+        :type numPartitions: int
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
         self._minSup = minSup
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/pyspark/parallelApriori.py` & `pami-2023.8.6.1/PAMI/frequentPattern/pyspark/parallelApriori.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     
                 obj.startMine()
     
                 frequentPatterns = obj.getPatterns()
     
                 print("Total number of Frequent Patterns:", len(frequentPatterns))
     
-                obj.savePatterns(oFile)
+                obj.save(oFile)
     
                 Df = obj.getPatternInDataFrame()
     
                 memUSS = obj.getMemoryUSS()
     
                 print("Total Memory in USS:", memUSS)
     
@@ -157,14 +157,48 @@
     _memoryRSS = float()
     _numPartitions = int()
     _lno = int()
 
     def __init__(self, iFile, minSup, numWorkers, sep='\t'):
         super().__init__(iFile, minSup, int(numWorkers), sep)
 
+    def _creatingItemSets(self):
+        """
+            Storing the complete transactions of the database/input file in a database variable
+
+
+        """
+        self._Database = []
+        if isinstance(self._iFile, _ab._pd.DataFrame):
+            if self._iFile.empty:
+                print("its empty..")
+            i = self._iFile.columns.values.tolist()
+            if 'Transactions' in i:
+                self._Database = self._iFile['Transactions'].tolist()
+        if isinstance(self._iFile, str):
+            if _ab._validators.url(self._iFile):
+                data = _ab._urlopen(self._iFile)
+                for line in data:
+                    line.strip()
+                    line = line.decode("utf-8")
+                    temp = [i.rstrip() for i in line.split(self._sep)]
+                    temp = [x for x in temp if x]
+                    self._Database.append(temp)
+            else:
+                try:
+                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                        for line in f:
+                            line.strip()
+                            temp = [i.rstrip() for i in line.split(self._sep)]
+                            temp = [x for x in temp if x]
+                            #print(line)
+                            self._Database.append(temp)
+                except IOError:
+                    print("File Not Found")
+                    quit()
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryUSS
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/pyspark/parallelECLAT.py` & `pami-2023.8.6.1/PAMI/frequentPattern/pyspark/parallelECLAT.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Parallel Eclat is an algorithm to discover frequent patterns in a transactional database. This program employs parallel apriori property (or downward closure property) to  reduce the search space effectively.
+# ParallelEclat is an algorithm to discover frequent patterns in a transactional database. This program employs parallel apriori property (or downward closure property) to  reduce the search space effectively.
 #
 # **Importing this algorithm into a python program**
 #  ----------------------------------------------------
 #
 #
 #     import PAMI.frequentPattern.pyspark.parallelECLAT as alg
 #
@@ -44,27 +44,25 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-
-
-
-
-# from pyspark import SparkConf, SparkContext
+from pyspark import SparkConf, SparkContext
 # import abstract as _ab
 from PAMI.frequentPattern.pyspark import abstract as _ab
+from abc import ABC as _ABC, abstractmethod as _abstractmethod
 
 
 class parallelECLAT(_ab._frequentPatterns):
     """
 
-    :Description: Parallel Eclat is an algorithm to discover frequent patterns in a transactional database. This program employs parallel apriori property (or downward closure property) to  reduce the search space effectively.
+    :Description: ParallelEclat is an algorithm to discover frequent patterns in a transactional database.
+     This program employs parallel apriori property (or downward closure property) to  reduce the search space effectively.
 
     :Reference:
 
     :param  iFile: str :
                    Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
@@ -92,58 +90,58 @@
 
         memoryRSS : float
           To store the total amount of RSS memory consumed by the program
 
         lno : int
                 the number of transactions
 
-    
+
     **Methods to execute code on terminal**
     ----------------------------------------------------
-    
+
             Format:
                       >>> python3 parallelECLAT.py <inputFile> <outputFile> <minSup> <numWorkers>
-    
+
             Example:
                       >>> python3 parallelECLAT.py sampleDB.txt patterns.txt 10.0 3
-    
+
             .. note:: minSup will be considered in percentage of database transactions
-    
-    
+
+
     **Importing this algorithm into a python program**
     ----------------------------------------------------
     .. code-block:: python
-    
+
                 import PAMI.frequentPattern.pyspark.parallelECLAT as alg
-    
+
                 obj = alg.parallelECLAT(iFile, minSup, numWorkers)
-    
+
                 obj.startMine()
-    
+
                 frequentPatterns = obj.getPatterns()
-    
+
                 print("Total number of Frequent Patterns:", len(frequentPatterns))
-    
-                obj.savePatterns(oFile)
-    
+
+                obj.save(oFile)
+
                 Df = obj.getPatternInDataFrame()
-    
+
                 memUSS = obj.getMemoryUSS()
-    
+
                 print("Total Memory in USS:", memUSS)
-    
+
                 memRSS = obj.getMemoryRSS()
-    
+
                 print("Total Memory in RSS", memRSS)
-    
+
                 run = obj.getRuntime()
-    
+
                 print("Total ExecutionTime in seconds:", run)
-    
-    
+
+
     **Credits:**
     ----------------------------------------------------
              The complete program was written by Yudai Masu under the supervision of Professor Rage Uday Kiran.
 
     """
 
     _minSup = float()
@@ -154,15 +152,15 @@
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _lno = int()
 
-    def __init__(self, iFile, minSup, numWorkers, sep='\t'):
+    def __init__(self, iFile, minSup, numWorkers, sep="\t"):
         super().__init__(iFile, minSup, int(numWorkers), sep)
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
@@ -224,15 +222,16 @@
         Function to send the set of frequent patterns after completion of the mining process
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def _genPatterns(self, suffix, pattern, data):
-        """ param suffix:
+        """ This function is used to generate patterns
+            param suffix:
             return:
             param pattern:
             return:
             param data:
             type:
         """
         freqPatterns = {}
@@ -241,14 +240,22 @@
             tid = pattern[1].intersection(data[i][1])
             if len(tid) >= self._minSup:
                 freqPattern = pattern[0] + ' ' + data[i][0]
                 freqPatterns[freqPattern] = len(tid)
                 freqPatterns.update(self._genPatterns(data[i], (freqPattern, tid), data))
         return freqPatterns
 
+    def printResults(self):
+        """ this function is used to print the results
+        """
+        print("Total number of Frequent Patterns:", len(self.getPatterns()))
+        print("Total Memory in USS:", self.getMemoryUSS())
+        print("Total Memory in RSS", self.getMemoryRSS())
+        print("Total ExecutionTime in ms:", self.getRuntime())
+
     def _convert(self, value):
         """
         To convert the user specified minSup value
         :param value: user specified minSup value
         :return: converted type
         """
         print(value, type(value))
@@ -278,33 +285,32 @@
 
         data = sc.textFile(self._iFile, self._numPartitions) \
             .map(lambda line: [int(y) for y in line.rstrip().split(self._sep)]).persist()
         self._lno = data.count()
         self._minSup = self._convert(self._minSup)
 
         frequentItems = None
-        if 'transactional' in self._iFile:
-            frequentItems = data.zipWithIndex() \
-                .flatMap(lambda x: [(str(item), x[1]) for item in x[0]]) \
-                .groupByKey() \
-                .filter(lambda x: len(x[1]) >= self._minSup) \
-                .sortBy(lambda x: len(x[1])) \
-                .mapValues(set) \
-                .persist()
-            data.unpersist()
-        elif 'temporal' in self._iFile:
-            frequentItems = data.flatMap(lambda trans: [(str(item), trans[0]) for item in trans[1:]]) \
-                .groupByKey() \
-                .filter(lambda x: len(x[1]) >= self._minSup) \
-                .mapValues(set) \
-                .persist()
-            data.unpersist()
-        else:
-            pass
-            # print("may be not able to process the input file")
+        frequentItems = data.zipWithIndex() \
+            .flatMap(lambda x: [(str(item), x[1]) for item in x[0]]) \
+            .groupByKey() \
+            .filter(lambda x: len(x[1]) >= self._minSup) \
+            .sortBy(lambda x: len(x[1])) \
+            .mapValues(set) \
+            .persist()
+        data.unpersist()
+        # elif 'temporal' in self._iFile:
+        #     frequentItems = data.flatMap(lambda trans: [(str(item), trans[0]) for item in trans[1:]]) \
+        #         .groupByKey() \
+        #         .filter(lambda x: len(x[1]) >= self._minSup) \
+        #         .mapValues(set) \
+        #         .persist()
+        #     data.unpersist()
+        # else:
+        #     pass
+        #     # print("may be not able to process the input file")
 
         freqItems = dict(frequentItems.collect())
         # print(len(freqItems))
         self._finalPatterns = {k: len(v) for k, v in freqItems.items()}
 
         freqPatterns = list(frequentItems.map(lambda x: self._genPatterns(x, x, list(freqItems.items())))
                             .filter(lambda x: len(x) != 0).collect())
@@ -325,15 +331,15 @@
         if len(_ab._sys.argv) == 6:
             _ap = parallelECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
             _ap = parallelECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         _ap.startMine()
         _finalPatterns = _ap.getPatterns()
         print("Total number of Frequent Patterns:", len(_finalPatterns))
-        # _ap.savePatterns(_ab._sys.argv[2])
+        _ap.save(_ab._sys.argv[2])
         _memUSS = _ap.getMemoryUSS()
         print("Total Memory in USS:", _memUSS)
         _memRSS = _ap.getMemoryRSS()
         print("Total Memory in RSS", _memRSS)
         _run = _ap.getRuntime()
         print("Total ExecutionTime in ms:", _run)
     else:
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py` & `pami-2023.8.6.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,14 +457,15 @@
                 value = (self._lno * value)
             else:
                 value = int(value)
         else:
             print("minSup is not correct")
         return value
 
+
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
         if len(_ab._sys.argv) == 6:
             _ap = parallelFPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
             _ap = parallelFPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
```

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/topk/FAE.py` & `pami-2023.8.6.1/PAMI/frequentPattern/topk/FAE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/frequentPattern/topk/abstract.py` & `pami-2023.8.6.1/PAMI/frequentPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/fuzzyCorrelatedPattern/__init__.py` & `pami-2023.8.6.1/PAMI/fuzzyCorrelatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py` & `pami-2023.8.6.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,16 +163,16 @@
                 else:
                     temp = mapOfRegions[t1]
                     mapOfRegions = temp + 1
 
 
 class _Pair:
     """
-            A class to store item and it's quantity together
-        """
+         A class to store item and it's quantity together
+    """
 
     def __init__(self):
         """
             A Class to Store item and its quantity together
         """
         self.item = 0
         self.quantity = 0
```

### Comparing `pami-2023.8.2.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py` & `pami-2023.8.6.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/fuzzyFrequentPattern/__init__.py` & `pami-2023.8.6.1/PAMI/fuzzyFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py` & `pami-2023.8.6.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,46 +403,46 @@
                     remainUtil += revisedTransaction[j].quantity
                 remainingUtility = remainUtil
                 if mapItemsToFFLIST.get(pair.item) is not None:
                     FFListOfItem = mapItemsToFFLIST[pair.item]
                     element = _Element(tid, pair.quantity, remainingUtility)
                     FFListOfItem.addElement(element)
             tid += 1
-        self._FSFIMining(self._itemSetBuffer, 0, listOfffilist, self._minSup)
+        self._FFIMining(self._itemSetBuffer, 0, listOfffilist, self._minSup)
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
 
-    def _FSFIMining(self, prefix, prefixLen, FSFIM, minSup):
+    def _FFIMining(self, prefix, prefixLen, FSFIM, minSup):
         """Generates ffi from prefix
 
         :param prefix: the prefix patterns of ffi
         :type prefix: len
         :param prefixLen: the length of prefix
         :type prefixLen: int
         :param FSFIM: the Fuzzy list of prefix itemSets
         :type FSFIM: list
         :param minSup: the minimum support of
-        :type minSup:int
+        :type minSup: int or flaot
         """
         for i in range(0, len(FSFIM)):
             X = FSFIM[i]
             if X.sumIUtil >= minSup:
                 self._WriteOut(prefix, prefixLen, X.item, X.sumIUtil)
             if X.sumRUtil >= minSup:
                 exULs = []
                 for j in range(i + 1, len(FSFIM)):
                     Y = FSFIM[j]
                     exULs.append(self._construct(X, Y))
                     self._joinsCnt += 1
                 self._itemSetBuffer.insert(prefixLen, X.item)
-                self._FSFIMining(self._itemSetBuffer, prefixLen + 1, exULs, minSup)
+                self._FFIMining(self._itemSetBuffer, prefixLen + 1, exULs, minSup)
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
```

### Comparing `pami-2023.8.2.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py` & `pami-2023.8.6.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#     from PAMI.fuzzyFrequentPattern import FFIMiner as alg
+#     from PAMI.fuzzyFrequentPattern import FFIMiner_old as alg
 #
 #     obj = alg.FFIMiner("input.txt", 2)
 #
 #     obj.startMine()
 #
 #     fuzzyFrequentPattern = obj.getPatterns()
 #
```

### Comparing `pami-2023.8.2.1/PAMI/fuzzyFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/fuzzyFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py` & `pami-2023.8.6.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py` & `pami-2023.8.6.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py` & `pami-2023.8.6.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
                 value = (self._dbLen * value)
             else:
                 value = int(value)
         return value
 
     def _creatingItemSets(self):
         """
-                    Storing the complete transactions of the database/input file in a database variable
+          Storing the complete transactions of the database/input file in a database variable
 
         """
         self._transactions, self._fuzzyValues = [], []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
```

### Comparing `pami-2023.8.2.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py` & `pami-2023.8.6.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py` & `pami-2023.8.6.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py` & `pami-2023.8.6.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py` & `pami-2023.8.6.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         self.maxPeriod = 0
 
     def addElement(self, element):
         """
             A Method that add a new element to FFList
 
             :param element: an element to be added to FFList
-            :param type: Element
+            :type element: Element
         """
         self.sumLUtil += element.lUtils
         self.sumRUtil += element.rUtils
         self.elements.append(element)
         self.maxPeriod = max(self.maxPeriod, element.period)
 
     def printElement(self):
@@ -154,16 +154,17 @@
 
         Fuzzy Periodic Frequent Pattern Miner is desired to find all fuzzy periodic frequent patterns which is
         on-trivial and challenging problem to its huge search space.we are using efficient pruning
         techniques to reduce the search space.
 
     Reference:
     -----------
-        Lin, N.P., & Chueh, H. (2007). Fuzzy correlation rules mining.
-        https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.416.6053&rep=rep1&type=pdf
+       R. U. Kiran et al., "Discovering Fuzzy Periodic-Frequent Patterns in Quantitative Temporal Databases,"
+        2020 IEEE International Conference on Fuzzy Systems (FUZZ-IEEE), Glasgow, UK, 2020, pp.
+        1-8, doi: 10.1109/FUZZ48607.2020.9177579.
 
     Attributes:
     ----------
         iFile : file
             Name of the input file to mine complete set of fuzzy spatial frequent patterns
         oFile : file
                Name of the oFile file to store complete set of fuzzy spatial frequent patterns
@@ -274,15 +275,15 @@
     Credits:
     -------
             The complete program was written by Sai Chitra.B under the supervision of Professor Rage Uday Kiran.
 
     """
     _startTime = float()
     _endTime = float()
-    _minSup = str()
+    _minSup = float()
     _maxPer = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _sep = " "
@@ -406,14 +407,15 @@
                 if item in self._mapItemSum:
                     self._mapItemSum[item] += quantities[i]
                 else:
                     self._mapItemSum[item] = quantities[i]
         listOfFFIList = []
         mapItemsToFFLIST = {}
         # self._minSup = self._convert(self._minSup)
+        self._minSup = float(self._minSup)
         self._maxPer = self._convert(self._maxPer)
         for item1 in self._mapItemSum.keys():
             item = item1
             if self._mapItemSum[item] >= self._minSup:
                 fUList = _FFList(item)
                 k = tuple([item])
                 mapItemsToFFLIST[k] = fUList
@@ -451,47 +453,45 @@
                         if lastTIDs[pair.item] == tid:
                             element = _Element(tid, pair.quantity, remainingUtility, maxTID - tid)
                         else:
                             lastTid = FFListOfItem.elements[-1].tid
                             curPer = tid - lastTid
                             element = _Element(tid, pair.quantity, remainingUtility, curPer)
                     FFListOfItem.addElement(element)
-        self._FSFIMining(self._itemSetBuffer, 0, listOfFFIList, self._minSup)
+        self._FPFPMining(self._itemSetBuffer, 0, listOfFFIList)
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
 
-    def _FSFIMining(self, prefix, prefixLen, fsFim, minSup):
+    def _FPFPMining(self, prefix, prefixLen, fsFim):
 
         """Generates FPFP from prefix
 
         :param prefix: the prefix patterns of FPFP
         :type prefix: len
         :param prefixLen: the length of prefix
         :type prefixLen: int
         :param fsFim: the Fuzzy list of prefix itemSets
         :type fsFim: list
-        :param minSup: the minimum support of
-        :type minSup:int
         """
         for i in range(0, len(fsFim)):
             X = fsFim[i]
-            if X.sumLUtil >= minSup and X.maxPeriod <= self._maxPer:
+            if X.sumLUtil >= self._minSup and X.maxPeriod <= self._maxPer:
                 self._WriteOut(prefix, prefixLen, X.item, X.sumLUtil, X.maxPeriod)
-            if X.sumRUtil >= minSup:
+            if X.sumRUtil >= self._minSup:
                 exULs = []
                 for j in range(i + 1, len(fsFim)):
                     Y = fsFim[j]
                     exULs.append(self._construct(X, Y))
                     self._joinsCnt += 1
                 self._itemSetBuffer.insert(prefixLen, X.item)
-                self._FSFIMining(self._itemSetBuffer, prefixLen + 1, exULs, minSup, )
+                self._FPFPMining(self._itemSetBuffer, prefixLen + 1, exULs)
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
```

### Comparing `pami-2023.8.2.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py` & `pami-2023.8.6.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py` & `pami-2023.8.6.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py` & `pami-2023.8.6.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/georeferencedFrequentPattern/__init__.py` & `pami-2023.8.6.1/PAMI/georeferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py` & `pami-2023.8.6.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py` & `pami-2023.8.6.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/georeferencedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/georeferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/georeferencedFrequentSequencePattern/abstract.py` & `pami-2023.8.6.1/PAMI/georeferencedFrequentSequencePattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py` & `pami-2023.8.6.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py` & `pami-2023.8.6.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilityFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/highUtilityFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py` & `pami-2023.8.6.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py` & `pami-2023.8.6.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilityPattern/basic/EFIM.py` & `pami-2023.8.6.1/PAMI/highUtilityPattern/basic/EFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilityPattern/basic/HMiner.py` & `pami-2023.8.6.1/PAMI/highUtilityPattern/basic/HMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilityPattern/basic/UPGrowth.py` & `pami-2023.8.6.1/PAMI/highUtilityPattern/basic/UPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilityPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/highUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilityPattern/basic/efimParallel.py` & `pami-2023.8.6.1/PAMI/highUtilityPattern/basic/efimParallel.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilityPattern/parallel/abstract.py` & `pami-2023.8.6.1/PAMI/highUtilityPattern/parallel/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilityPattern/parallel/efimparallel.py` & `pami-2023.8.6.1/PAMI/highUtilityPattern/parallel/efimparallel.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilityPatternsInStreams/HUPMS.py` & `pami-2023.8.6.1/PAMI/highUtilityPatternsInStreams/HUPMS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py` & `pami-2023.8.6.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilityPatternsInStreams/abstract.py` & `pami-2023.8.6.1/PAMI/highUtilityPatternsInStreams/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/__init__.py` & `pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/abstract.py` & `pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py` & `pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py` & `pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py` & `pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/highUtilitySpatialPattern/topk/abstract.py` & `pami-2023.8.6.1/PAMI/highUtilitySpatialPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py` & `pami-2023.8.6.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py` & `pami-2023.8.6.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py` & `pami-2023.8.6.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/localPeriodicPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/localPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py` & `pami-2023.8.6.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py` & `pami-2023.8.6.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py` & `pami-2023.8.6.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py` & `pami-2023.8.6.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicPattern/__init__.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicPattern/basic/Gabstract.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPattern/basic/Gabstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicPattern/basic/__init__.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicPattern/closed/PPPClose.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPattern/closed/PPPClose.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicPattern/closed/abstract.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicPattern/maximal/__init__.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicPattern/maximal/abstract.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicPattern/topk/abstract.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py` & `pami-2023.8.6.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicCorrelatedPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/periodicCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/__init__.py` & `pami-2023.8.6.1/PAMI/partialPeriodicPattern/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/basic/PFPMC.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/basic/PFPMC.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/basic/__init__.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/closed/__init__.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/closed/abstract.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/cuda/abstract.py` & `pami-2023.8.6.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,25 +21,22 @@
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
-import cupy as _cp
-import numpy as _np
 from urllib.request import urlopen as _urlopen
 
 
 class _periodicFrequentPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every periodic-frequent pattern mining algorithm must
         employ in PAMI
-
-    Attributes:
-    ----------
+       Attributes
+        ----------
         iFile : str
             Input file name or path of the input file
         minSup: int or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
@@ -59,17 +56,16 @@
             Storing the complete set of patterns in a dictionary variable
         oFile : str
             Name of the output file to store complete set of periodic-frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
-
-    Methods:
-    -------
+        Methods
+        -------
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
             Complete set of periodic-frequent patterns will be loaded in to a output file
         getPatternsAsDataFrame()
@@ -92,28 +88,28 @@
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param maxPer: The user can specify maxPer either in count or proportion of database size.
             If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
             Otherwise, it will be treated as float.
             Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
         :type maxPer: int or float or str
-        :param sep: separator used in user specified input file
-        :type sep: str
+        :param sep: The user specified seperator used in the input file
+        :type maxPer: str
         """
 
         self._iFile = iFile
         self._minSup = minSup
         self._maxPer = maxPer
         self._sep = sep
+        self._oFile = str()
         self._finalPatterns = {}
+        self._memoryUSS = float()
+        self._memoryRSS = float()
         self._startTime = float()
         self._endTime = float()
-        self._memoryRSS = float()
-        self._memoryUSS = float()
-        self._oFile = " "
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -122,15 +118,14 @@
         """Complete set of periodic-frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
         """Complete set of periodic-frequent patterns will be saved in to an output file from this function
-
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
@@ -154,10 +149,10 @@
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def printResults(self):
-        """ To print results of the execution."""
+        """ To print all the results of execution"""
 
         pass
```

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/maximal/__init__.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/closed/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/maximal/abstract.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/pyspark/abstract.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/recurringPattern/basic/RPGrowth.py` & `pami-2023.8.6.1/PAMI/recurringPattern/basic/RPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/recurringPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/recurringPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py` & `pami-2023.8.6.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/relativeFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/relativeFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py` & `pami-2023.8.6.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/relativeHighUtilityPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/relativeHighUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/sequentialPatternMining/basic/SPADE.py` & `pami-2023.8.6.1/PAMI/sequentialPatternMining/basic/SPADE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/sequentialPatternMining/basic/SPAM.py` & `pami-2023.8.6.1/PAMI/sequentialPatternMining/basic/SPAM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/sequentialPatternMining/basic/abstract.py` & `pami-2023.8.6.1/PAMI/sequentialPatternMining/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/sequentialPatternMining/basic/prefixSpan.py` & `pami-2023.8.6.1/PAMI/sequentialPatternMining/basic/prefixSpan.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/sequentialPatternMining/closed/abstract.py` & `pami-2023.8.6.1/PAMI/sequentialPatternMining/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py` & `pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py` & `pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py` & `pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py` & `pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py` & `pami-2023.8.6.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py` & `pami-2023.8.6.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py` & `pami-2023.8.6.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainFrequentPattern/__init__.py` & `pami-2023.8.6.1/PAMI/periodicFrequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py` & `pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py` & `pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/TUFP.py` & `pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/TUFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/TubeP.py` & `pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/TubeP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/TubeS.py` & `pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/TubeS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py` & `pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py` & `pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/uncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py` & `pami-2023.8.6.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py` & `pami-2023.8.6.1/PAMI/uncertainFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py` & `pami-2023.8.6.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py` & `pami-2023.8.6.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/frequentPattern/cuda/abstract.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,34 +21,36 @@
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
+import cupy as _cp
+import numpy as _np
 from urllib.request import urlopen as _urlopen
+import pycuda.gpuarray as _gpuarray
+import pycuda.autoinit
+import pycuda.driver as _cuda
+from pycuda.compiler import _SourceModule
 
 
-class _periodicFrequentPatterns(_ABC):
-    """ This abstract base class defines the variables and methods that every periodic-frequent pattern mining algorithm must
+class _frequentPatterns(_ABC):
+    """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
-       Attributes
-        ----------
+
+    Attributes:
+    ----------
         iFile : str
             Input file name or path of the input file
         minSup: int or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-        maxPer: int or float or str
-            The user can specify maxPer either in count or proportion of database size.
-            If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator.
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
@@ -56,16 +58,17 @@
             Storing the complete set of patterns in a dictionary variable
         oFile : str
             Name of the output file to store complete set of periodic-frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
-        Methods
-        -------
+
+    Methods:
+    -------
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
             Complete set of periodic-frequent patterns will be loaded in to a output file
         getPatternsAsDataFrame()
@@ -74,42 +77,36 @@
             Total amount of USS memory consumed by the program will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the program will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the program will be retrieved from this function
     """
 
-    def __init__(self, iFile, minSup, maxPer, sep = '\t'):
+    def __init__(self, iFile, minSup, sep = '\t'):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
-        :param maxPer: The user can specify maxPer either in count or proportion of database size.
-            If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
-        :type maxPer: int or float or str
-        :param sep: The user specified seperator used in the input file
-        :type maxPer: str
+        :param sep: separator used in user specified input file
+        :type sep: str
         """
 
         self._iFile = iFile
         self._minSup = minSup
-        self._maxPer = maxPer
         self._sep = sep
-        self._oFile = str()
         self._finalPatterns = {}
-        self._memoryUSS = float()
-        self._memoryRSS = float()
         self._startTime = float()
         self._endTime = float()
+        self._memoryRSS = float()
+        self._memoryUSS = float()
+        self._oFile = " "
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -118,14 +115,15 @@
         """Complete set of periodic-frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
         """Complete set of periodic-frequent patterns will be saved in to an output file from this function
+
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
@@ -149,10 +147,10 @@
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def printResults(self):
-        """ To print all the results of execution"""
+        """ To print results of the execution."""
 
         pass
```

### Comparing `pami-2023.8.2.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py` & `pami-2023.8.6.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/weightedFrequentPattern/basic/WFIM.py` & `pami-2023.8.6.1/PAMI/weightedFrequentPattern/basic/WFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/weightedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/weightedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py` & `pami-2023.8.6.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py` & `pami-2023.8.6.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py` & `pami-2023.8.6.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/PKG-INFO` & `pami-2023.8.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2023.8.2.1
+Version: 2023.8.6.1
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayLab/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pami-2023.8.2.1/README.md` & `pami-2023.8.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pami-2023.8.2.1/pami.egg-info/PKG-INFO` & `pami-2023.8.6.1/pami.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2023.8.2.1
+Version: 2023.8.6.1
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayLab/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pami-2023.8.2.1/pami.egg-info/SOURCES.txt` & `pami-2023.8.6.1/pami.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 PAMI/extras/DF2DB/sparseDF2DB.py
 PAMI/extras/DF2DB/sparseDF2DBPlus.py
 PAMI/extras/calculateMISValues/__init__.py
 PAMI/extras/calculateMISValues/usingBeta.py
 PAMI/extras/calculateMISValues/usingSD.py
 PAMI/extras/dbStats/__init__.py
 PAMI/extras/dbStats/fuzzyDatabaseStats.py
-PAMI/extras/dbStats/sequencialDatabaseStats.py
+PAMI/extras/dbStats/sequentialDatabaseStats.py
 PAMI/extras/dbStats/temporalDatabaseStats.py
 PAMI/extras/dbStats/transactionalDatabaseStats.py
 PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
 PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
 PAMI/extras/dbStats/utilityDatabaseStats.py
 PAMI/extras/fuzzyTransformation/__init__.py
 PAMI/extras/fuzzyTransformation/abstract.py
@@ -207,14 +207,17 @@
 PAMI/partialPeriodicPattern/basic/abstract.py
 PAMI/partialPeriodicPattern/closed/PPPClose.py
 PAMI/partialPeriodicPattern/closed/__init__.py
 PAMI/partialPeriodicPattern/closed/abstract.py
 PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
 PAMI/partialPeriodicPattern/maximal/__init__.py
 PAMI/partialPeriodicPattern/maximal/abstract.py
+PAMI/partialPeriodicPattern/pyspark/__init__.py
+PAMI/partialPeriodicPattern/pyspark/abstract.py
+PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py
 PAMI/partialPeriodicPattern/topk/__init__.py
 PAMI/partialPeriodicPattern/topk/abstract.py
 PAMI/partialPeriodicPattern/topk/k3PMiner.py
 PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
 PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
 PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
 PAMI/periodicCorrelatedPattern/__init__.py
```

### Comparing `pami-2023.8.2.1/setup.py` & `pami-2023.8.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pami',
-    version='2023.08.02.01',
+    version='2023.08.06.01',
     author='Rage Uday Kiran',
     author_email='uday.rage@gmail.com',
     description='This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     url='https://github.com/udayLab/PAMI',
```

