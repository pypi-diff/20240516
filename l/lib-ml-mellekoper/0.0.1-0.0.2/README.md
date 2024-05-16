# Comparing `tmp/lib_ml_mellekoper-0.0.1.tar.gz` & `tmp/lib_ml_mellekoper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_ml_mellekoper-0.0.1.tar", last modified: Fri May 10 16:55:20 2024, max compression
+gzip compressed data, was "lib_ml_mellekoper-0.0.2.tar", last modified: Thu May 16 13:16:42 2024, max compression
```

## Comparing `lib_ml_mellekoper-0.0.1.tar` & `lib_ml_mellekoper-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 16:55:20.039229 lib_ml_mellekoper-0.0.1/
--rw-rw-rw-   0        0        0      542 2024-05-10 16:55:20.037228 lib_ml_mellekoper-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       38 2024-05-10 15:18:26.000000 lib_ml_mellekoper-0.0.1/README.md
--rw-rw-rw-   0        0        0      511 2024-05-10 16:36:33.000000 lib_ml_mellekoper-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 16:55:20.040227 lib_ml_mellekoper-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-10 16:55:19.996226 lib_ml_mellekoper-0.0.1/src/
--rw-rw-rw-   0        0        0      445 2024-05-10 16:36:33.000000 lib_ml_mellekoper-0.0.1/src/Preprocess.py
--rw-rw-rw-   0        0        0        0 2024-05-10 16:36:33.000000 lib_ml_mellekoper-0.0.1/src/__init__.py
--rw-rw-rw-   0        0        0     1046 2024-05-10 16:36:33.000000 lib_ml_mellekoper-0.0.1/src/get_tokenizer.py
-drwxrwxrwx   0        0        0        0 2024-05-10 16:55:20.035230 lib_ml_mellekoper-0.0.1/src/lib_ml_mellekoper.egg-info/
--rw-rw-rw-   0        0        0      542 2024-05-10 16:55:19.000000 lib_ml_mellekoper-0.0.1/src/lib_ml_mellekoper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-05-10 16:55:19.000000 lib_ml_mellekoper-0.0.1/src/lib_ml_mellekoper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 16:55:19.000000 lib_ml_mellekoper-0.0.1/src/lib_ml_mellekoper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-10 16:55:19.000000 lib_ml_mellekoper-0.0.1/src/lib_ml_mellekoper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:16:42.747653 lib_ml_mellekoper-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 13:16:42.747653 lib_ml_mellekoper-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-16 13:16:38.000000 lib_ml_mellekoper-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-16 13:16:38.000000 lib_ml_mellekoper-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:16:42.747653 lib_ml_mellekoper-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:16:42.743653 lib_ml_mellekoper-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:16:42.747653 lib_ml_mellekoper-0.0.2/src/lib_ml_mellekoper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 13:16:42.000000 lib_ml_mellekoper-0.0.2/src/lib_ml_mellekoper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-16 13:16:42.000000 lib_ml_mellekoper-0.0.2/src/lib_ml_mellekoper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:16:42.000000 lib_ml_mellekoper-0.0.2/src/lib_ml_mellekoper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 13:16:42.000000 lib_ml_mellekoper-0.0.2/src/lib_ml_mellekoper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:16:42.747653 lib_ml_mellekoper-0.0.2/src/lib_ml_remla/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-16 13:16:38.000000 lib_ml_mellekoper-0.0.2/src/lib_ml_remla/Preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:16:38.000000 lib_ml_mellekoper-0.0.2/src/lib_ml_remla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-16 13:16:38.000000 lib_ml_mellekoper-0.0.2/src/lib_ml_remla/get_tokenizer.py
```

### Comparing `lib_ml_mellekoper-0.0.1/src/get_tokenizer.py` & `lib_ml_mellekoper-0.0.2/src/lib_ml_remla/get_tokenizer.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from joblib import dump
-from tensorflow.keras.preprocessing.text import Tokenizer
-
-# check data locations with extraction from drive
-with open("dataset/train.txt", "r", encoding="utf-8") as file:
-    train = [line.strip() for line in file.readlines()[1:]]
-raw_x_train = [line.split("\t")[1] for line in train]
-raw_y_train = [line.split("\t")[0] for line in train]
-
-with open("dataset/test.txt", "r", encoding="utf-8") as file:
-    test = [line.strip() for line in file.readlines()]
-raw_x_test = [line.split("\t")[1] for line in test]
-raw_y_test = [line.split("\t")[0] for line in test]
-
-with open("dataset/val.txt", "r", encoding="utf-8") as file:
-    val = [line.strip() for line in file.readlines()]
-raw_x_val = [line.split("\t")[1] for line in val]
-raw_y_val = [line.split("\t")[0] for line in val]
-tokenizer = Tokenizer(lower=True, char_level=True, oov_token='-n-')
-tokenizer.fit_on_texts(raw_x_train + raw_x_val + raw_x_test)
-char_index = tokenizer.word_index
-SEQUENCE_LENGTH = 200
-
+from joblib import dump
+from tensorflow.keras.preprocessing.text import Tokenizer
+
+# check data locations with extraction from drive
+with open("dataset/train.txt", "r", encoding="utf-8") as file:
+    train = [line.strip() for line in file.readlines()[1:]]
+raw_x_train = [line.split("\t")[1] for line in train]
+raw_y_train = [line.split("\t")[0] for line in train]
+
+with open("dataset/test.txt", "r", encoding="utf-8") as file:
+    test = [line.strip() for line in file.readlines()]
+raw_x_test = [line.split("\t")[1] for line in test]
+raw_y_test = [line.split("\t")[0] for line in test]
+
+with open("dataset/val.txt", "r", encoding="utf-8") as file:
+    val = [line.strip() for line in file.readlines()]
+raw_x_val = [line.split("\t")[1] for line in val]
+raw_y_val = [line.split("\t")[0] for line in val]
+tokenizer = Tokenizer(lower=True, char_level=True, oov_token='-n-')
+tokenizer.fit_on_texts(raw_x_train + raw_x_val + raw_x_test)
+char_index = tokenizer.word_index
+SEQUENCE_LENGTH = 200
+
 dump(tokenizer, 'tokenizer.joblib')
```

