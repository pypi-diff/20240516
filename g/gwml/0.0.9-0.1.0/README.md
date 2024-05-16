# Comparing `tmp/gwml-0.0.9-py3-none-any.whl.zip` & `tmp/gwml-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,58 @@
-Zip file size: 2299 bytes, number of entries: 9
--rw-r--r--  2.0 unx       22 b- defN 24-May-14 09:31 gwml/__init__.py
--rw-r--r--  2.0 unx      125 b- defN 24-May-08 00:38 gwml/example.py
--rw-r--r--  2.0 unx       22 b- defN 24-May-14 09:31 gwml/lib/__init__.py
--rw-r--r--  2.0 unx      167 b- defN 24-May-14 09:16 gwml/lib/example.py
--rw-r--r--  2.0 unx       28 b- defN 24-May-14 09:31 gwml-0.0.9.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      645 b- defN 24-May-14 09:31 gwml-0.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-14 09:31 gwml-0.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-May-14 09:31 gwml-0.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      663 b- defN 24-May-14 09:31 gwml-0.0.9.dist-info/RECORD
-9 files, 1769 bytes uncompressed, 1157 bytes compressed:  34.6%
+Zip file size: 78253 bytes, number of entries: 56
+-rw-r--r--  2.0 unx        0 b- defN 24-May-14 09:40 gwml/__init__.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-May-16 05:28 gwml/command.py
+-rw-r--r--  2.0 unx      206 b- defN 24-May-16 05:31 gwml/main.py
+-rw-r--r--  2.0 unx      104 b- defN 24-May-16 05:28 gwml/mldump.py
+-rw-r--r--  2.0 unx       42 b- defN 24-May-14 09:41 gwml/module1.py
+-rw-r--r--  2.0 unx       43 b- defN 24-May-14 09:41 gwml/module2.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-14 09:40 gwml/lib/__init__.py
+-rw-r--r--  2.0 unx       43 b- defN 24-May-14 09:41 gwml/lib/libmodule1.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:40 gwml/lib/common/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:40 gwml/lib/common/Environment/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:40 gwml/lib/common/Environment/oracle/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:40 gwml/lib/common/Environment/oracle/lib/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:40 gwml/lib/common/automl/__init__.py
+-rw-r--r--  2.0 unx    16836 b- defN 24-May-16 05:39 gwml/lib/common/automl/automl.py
+-rw-r--r--  2.0 unx     4447 b- defN 24-May-16 05:39 gwml/lib/common/automl/test.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:40 gwml/lib/common/datalib/__init__.py
+-rw-r--r--  2.0 unx    20015 b- defN 24-May-16 05:39 gwml/lib/common/datalib/dataLib.py
+-rw-r--r--  2.0 unx    22096 b- defN 24-May-16 05:39 gwml/lib/common/datalib/dataLibCustom.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:40 gwml/lib/common/decorator/__init__.py
+-rw-r--r--  2.0 unx     5894 b- defN 24-May-16 05:39 gwml/lib/common/decorator/regDecorator.py
+-rw-r--r--  2.0 unx     2718 b- defN 24-May-16 05:39 gwml/lib/common/decorator/error/WedaErrorDecorator.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:40 gwml/lib/common/decorator/error/__init__.py
+-rw-r--r--  2.0 unx     2293 b- defN 24-May-16 05:39 gwml/lib/common/decorator/logger/Logger.py
+-rw-r--r--  2.0 unx     2462 b- defN 24-May-16 05:39 gwml/lib/common/decorator/logger/WedaLogDecorator.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:40 gwml/lib/common/decorator/logger/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:41 gwml/lib/common/evaluation/__init__.py
+-rw-r--r--  2.0 unx    49881 b- defN 24-May-16 05:39 gwml/lib/common/evaluation/evaluation.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:41 gwml/lib/common/graph/__init__.py
+-rw-r--r--  2.0 unx    18136 b- defN 24-May-16 05:39 gwml/lib/common/graph/causalAnalysis.py
+-rw-r--r--  2.0 unx    23627 b- defN 24-May-16 05:39 gwml/lib/common/graph/graph.py
+-rw-r--r--  2.0 unx     7319 b- defN 24-May-16 05:39 gwml/lib/common/graph/graphCluster.py
+-rw-r--r--  2.0 unx    10162 b- defN 24-May-16 05:39 gwml/lib/common/graph/graphTs.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:41 gwml/lib/common/operation/__init__.py
+-rw-r--r--  2.0 unx     8535 b- defN 24-May-16 05:39 gwml/lib/common/operation/condition.py
+-rw-r--r--  2.0 unx    21596 b- defN 24-May-16 05:39 gwml/lib/common/operation/operation.py
+-rw-r--r--  2.0 unx      422 b- defN 24-May-16 05:39 gwml/lib/common/operation/postprocessing.py
+-rw-r--r--  2.0 unx      401 b- defN 24-May-16 05:39 gwml/lib/common/operation/preprocessing.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:41 gwml/lib/common/sender/__init__.py
+-rw-r--r--  2.0 unx     1493 b- defN 24-May-16 05:39 gwml/lib/common/sender/sender.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:41 gwml/lib/common/sfds/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:41 gwml/lib/common/sfds/reg/__init__.py
+-rw-r--r--  2.0 unx     5565 b- defN 24-May-16 05:39 gwml/lib/common/sfds/reg/regDecorator.py
+-rw-r--r--  2.0 unx     1181 b- defN 24-May-16 05:39 gwml/lib/common/sfds/reg/regModel.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:41 gwml/lib/common/trainer/__init__.py
+-rw-r--r--  2.0 unx    11934 b- defN 24-May-16 05:39 gwml/lib/common/trainer/customTrainer.py
+-rw-r--r--  2.0 unx    10834 b- defN 24-May-16 05:39 gwml/lib/common/trainer/regTrainer.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:41 gwml/lib/common/utils/__init__.py
+-rw-r--r--  2.0 unx     2317 b- defN 24-May-16 05:39 gwml/lib/common/utils/utils.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:40 gwml/lib/reg/__init__.py
+-rw-r--r--  2.0 unx     5213 b- defN 24-May-16 05:39 gwml/lib/reg/regDecorator.py
+-rw-r--r--  2.0 unx    24363 b- defN 24-May-16 05:39 gwml/lib/reg/regTrainer.py
+-rw-r--r--  2.0 unx       49 b- defN 24-May-16 05:42 gwml-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 05:42 gwml-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 24-May-16 05:42 gwml-0.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 24-May-16 05:42 gwml-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4959 b- defN 24-May-16 05:42 gwml-0.1.0.dist-info/RECORD
+56 files, 287240 bytes uncompressed, 70233 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -1,28 +1,169 @@
 Filename: gwml/__init__.py
 Comment: 
 
-Filename: gwml/example.py
+Filename: gwml/command.py
+Comment: 
+
+Filename: gwml/main.py
+Comment: 
+
+Filename: gwml/mldump.py
+Comment: 
+
+Filename: gwml/module1.py
+Comment: 
+
+Filename: gwml/module2.py
 Comment: 
 
 Filename: gwml/lib/__init__.py
 Comment: 
 
-Filename: gwml/lib/example.py
+Filename: gwml/lib/libmodule1.py
+Comment: 
+
+Filename: gwml/lib/common/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/Environment/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/Environment/oracle/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/Environment/oracle/lib/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/automl/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/automl/automl.py
+Comment: 
+
+Filename: gwml/lib/common/automl/test.py
+Comment: 
+
+Filename: gwml/lib/common/datalib/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/datalib/dataLib.py
+Comment: 
+
+Filename: gwml/lib/common/datalib/dataLibCustom.py
+Comment: 
+
+Filename: gwml/lib/common/decorator/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/decorator/regDecorator.py
+Comment: 
+
+Filename: gwml/lib/common/decorator/error/WedaErrorDecorator.py
+Comment: 
+
+Filename: gwml/lib/common/decorator/error/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/decorator/logger/Logger.py
+Comment: 
+
+Filename: gwml/lib/common/decorator/logger/WedaLogDecorator.py
+Comment: 
+
+Filename: gwml/lib/common/decorator/logger/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/evaluation/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/evaluation/evaluation.py
+Comment: 
+
+Filename: gwml/lib/common/graph/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/graph/causalAnalysis.py
+Comment: 
+
+Filename: gwml/lib/common/graph/graph.py
+Comment: 
+
+Filename: gwml/lib/common/graph/graphCluster.py
+Comment: 
+
+Filename: gwml/lib/common/graph/graphTs.py
+Comment: 
+
+Filename: gwml/lib/common/operation/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/operation/condition.py
+Comment: 
+
+Filename: gwml/lib/common/operation/operation.py
+Comment: 
+
+Filename: gwml/lib/common/operation/postprocessing.py
+Comment: 
+
+Filename: gwml/lib/common/operation/preprocessing.py
+Comment: 
+
+Filename: gwml/lib/common/sender/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/sender/sender.py
+Comment: 
+
+Filename: gwml/lib/common/sfds/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/sfds/reg/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/sfds/reg/regDecorator.py
+Comment: 
+
+Filename: gwml/lib/common/sfds/reg/regModel.py
+Comment: 
+
+Filename: gwml/lib/common/trainer/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/trainer/customTrainer.py
+Comment: 
+
+Filename: gwml/lib/common/trainer/regTrainer.py
+Comment: 
+
+Filename: gwml/lib/common/utils/__init__.py
+Comment: 
+
+Filename: gwml/lib/common/utils/utils.py
+Comment: 
+
+Filename: gwml/lib/reg/__init__.py
+Comment: 
+
+Filename: gwml/lib/reg/regDecorator.py
+Comment: 
+
+Filename: gwml/lib/reg/regTrainer.py
 Comment: 
 
-Filename: gwml-0.0.9.dist-info/LICENSE.txt
+Filename: gwml-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: gwml-0.0.9.dist-info/METADATA
+Filename: gwml-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: gwml-0.0.9.dist-info/WHEEL
+Filename: gwml-0.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: gwml-0.0.9.dist-info/top_level.txt
+Filename: gwml-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gwml-0.0.9.dist-info/RECORD
+Filename: gwml-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gwml/__init__.py

```diff
@@ -1,2 +0,0 @@
-00000000: 5f5f 7665 7273 696f 6e5f 5f20 3d20 2230  __version__ = "0
-00000010: 2e30 2e39 220a                           .0.9".
```

## gwml/lib/__init__.py

```diff
@@ -1,2 +0,0 @@
-00000000: 5f5f 7665 7273 696f 6e5f 5f20 3d20 2230  __version__ = "0
-00000010: 2e30 2e39 220a                           .0.9".
```

