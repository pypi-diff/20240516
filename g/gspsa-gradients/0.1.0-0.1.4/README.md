# Comparing `tmp/gspsa-gradients-0.1.0.tar.gz` & `tmp/gspsa_gradients-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspsa-gradients-0.1.0.tar", last modified: Thu May 16 12:55:55 2024, max compression
+gzip compressed data, was "gspsa_gradients-0.1.4.tar", last modified: Thu May 16 14:10:46 2024, max compression
```

## Comparing `gspsa-gradients-0.1.0.tar` & `gspsa_gradients-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 periyamn  (1002) periyamn  (1002)        0 2024-05-16 12:55:55.589613 gspsa-gradients-0.1.0/
--rw-rw-r--   0 periyamn  (1002) periyamn  (1002)    11357 2024-04-24 18:51:44.000000 gspsa-gradients-0.1.0/LICENSE
--rw-r--r--   0 periyamn  (1002) periyamn  (1002)      330 2024-05-16 12:55:55.589613 gspsa-gradients-0.1.0/PKG-INFO
-drwxrwxr-x   0 periyamn  (1002) periyamn  (1002)        0 2024-05-16 12:55:55.585613 gspsa-gradients-0.1.0/gspsa_gradients/
--rw-rw-r--   0 periyamn  (1002) periyamn  (1002)      278 2024-05-16 07:47:23.000000 gspsa-gradients-0.1.0/gspsa_gradients/__init__.py
-drwxrwxr-x   0 periyamn  (1002) periyamn  (1002)        0 2024-05-16 12:55:55.585613 gspsa-gradients-0.1.0/gspsa_gradients/qiskit_gradient/
--rw-rw-r--   0 periyamn  (1002) periyamn  (1002)       41 2024-04-24 21:03:23.000000 gspsa-gradients-0.1.0/gspsa_gradients/qiskit_gradient/__init__.py
--rw-rw-r--   0 periyamn  (1002) periyamn  (1002)     7037 2024-05-16 07:27:44.000000 gspsa-gradients-0.1.0/gspsa_gradients/qiskit_gradient/gspsa.py
-drwxrwxr-x   0 periyamn  (1002) periyamn  (1002)        0 2024-05-16 12:55:55.585613 gspsa-gradients-0.1.0/gspsa_gradients/tfq_gradient/
--rw-rw-r--   0 periyamn  (1002) periyamn  (1002)       32 2024-05-15 11:16:55.000000 gspsa-gradients-0.1.0/gspsa_gradients/tfq_gradient/__init__.py
--rw-rw-r--   0 periyamn  (1002) periyamn  (1002)    12397 2024-05-16 07:27:50.000000 gspsa-gradients-0.1.0/gspsa_gradients/tfq_gradient/gspsa.py
-drwxrwxr-x   0 periyamn  (1002) periyamn  (1002)        0 2024-05-16 12:55:55.585613 gspsa-gradients-0.1.0/gspsa_gradients.egg-info/
--rw-r--r--   0 periyamn  (1002) periyamn  (1002)      330 2024-05-16 12:55:55.000000 gspsa-gradients-0.1.0/gspsa_gradients.egg-info/PKG-INFO
--rw-rw-r--   0 periyamn  (1002) periyamn  (1002)      402 2024-05-16 12:55:55.000000 gspsa-gradients-0.1.0/gspsa_gradients.egg-info/SOURCES.txt
--rw-rw-r--   0 periyamn  (1002) periyamn  (1002)        1 2024-05-16 12:55:55.000000 gspsa-gradients-0.1.0/gspsa_gradients.egg-info/dependency_links.txt
--rw-rw-r--   0 periyamn  (1002) periyamn  (1002)       78 2024-05-16 12:55:55.000000 gspsa-gradients-0.1.0/gspsa_gradients.egg-info/requires.txt
--rw-rw-r--   0 periyamn  (1002) periyamn  (1002)       32 2024-05-16 12:55:55.000000 gspsa-gradients-0.1.0/gspsa_gradients.egg-info/top_level.txt
--rw-rw-r--   0 periyamn  (1002) periyamn  (1002)       38 2024-05-16 12:55:55.589613 gspsa-gradients-0.1.0/setup.cfg
--rw-rw-r--   0 periyamn  (1002) periyamn  (1002)      347 2024-05-16 12:30:35.000000 gspsa-gradients-0.1.0/setup.py
+drwxrwxr-x   0 periyamn  (1002) periyamn  (1002)        0 2024-05-16 14:10:46.265345 gspsa_gradients-0.1.4/
+-rw-rw-r--   0 periyamn  (1002) periyamn  (1002)    11357 2024-04-24 18:51:44.000000 gspsa_gradients-0.1.4/LICENSE
+-rw-r--r--   0 periyamn  (1002) periyamn  (1002)     4133 2024-05-16 14:10:46.265345 gspsa_gradients-0.1.4/PKG-INFO
+drwxrwxr-x   0 periyamn  (1002) periyamn  (1002)        0 2024-05-16 14:10:46.265345 gspsa_gradients-0.1.4/gspsa_gradients/
+-rw-rw-r--   0 periyamn  (1002) periyamn  (1002)      278 2024-05-16 07:47:23.000000 gspsa_gradients-0.1.4/gspsa_gradients/__init__.py
+drwxrwxr-x   0 periyamn  (1002) periyamn  (1002)        0 2024-05-16 14:10:46.265345 gspsa_gradients-0.1.4/gspsa_gradients/qiskit_gradient/
+-rw-rw-r--   0 periyamn  (1002) periyamn  (1002)       41 2024-04-24 21:03:23.000000 gspsa_gradients-0.1.4/gspsa_gradients/qiskit_gradient/__init__.py
+-rw-rw-r--   0 periyamn  (1002) periyamn  (1002)     7037 2024-05-16 07:27:44.000000 gspsa_gradients-0.1.4/gspsa_gradients/qiskit_gradient/gspsa.py
+drwxrwxr-x   0 periyamn  (1002) periyamn  (1002)        0 2024-05-16 14:10:46.265345 gspsa_gradients-0.1.4/gspsa_gradients/tfq_gradient/
+-rw-rw-r--   0 periyamn  (1002) periyamn  (1002)       32 2024-05-15 11:16:55.000000 gspsa_gradients-0.1.4/gspsa_gradients/tfq_gradient/__init__.py
+-rw-rw-r--   0 periyamn  (1002) periyamn  (1002)    12397 2024-05-16 07:27:50.000000 gspsa_gradients-0.1.4/gspsa_gradients/tfq_gradient/gspsa.py
+drwxrwxr-x   0 periyamn  (1002) periyamn  (1002)        0 2024-05-16 14:10:46.265345 gspsa_gradients-0.1.4/gspsa_gradients.egg-info/
+-rw-r--r--   0 periyamn  (1002) periyamn  (1002)     4133 2024-05-16 14:10:46.000000 gspsa_gradients-0.1.4/gspsa_gradients.egg-info/PKG-INFO
+-rw-rw-r--   0 periyamn  (1002) periyamn  (1002)      418 2024-05-16 14:10:46.000000 gspsa_gradients-0.1.4/gspsa_gradients.egg-info/SOURCES.txt
+-rw-rw-r--   0 periyamn  (1002) periyamn  (1002)        1 2024-05-16 14:10:46.000000 gspsa_gradients-0.1.4/gspsa_gradients.egg-info/dependency_links.txt
+-rw-rw-r--   0 periyamn  (1002) periyamn  (1002)       72 2024-05-16 14:10:46.000000 gspsa_gradients-0.1.4/gspsa_gradients.egg-info/requires.txt
+-rw-rw-r--   0 periyamn  (1002) periyamn  (1002)       16 2024-05-16 14:10:46.000000 gspsa_gradients-0.1.4/gspsa_gradients.egg-info/top_level.txt
+-rw-rw-r--   0 periyamn  (1002) periyamn  (1002)      746 2024-05-16 14:10:36.000000 gspsa_gradients-0.1.4/pyproject.toml
+-rw-rw-r--   0 periyamn  (1002) periyamn  (1002)     3344 2024-05-16 13:38:11.000000 gspsa_gradients-0.1.4/readme.md
+-rw-rw-r--   0 periyamn  (1002) periyamn  (1002)       38 2024-05-16 14:10:46.265345 gspsa_gradients-0.1.4/setup.cfg
```

### Comparing `gspsa-gradients-0.1.0/LICENSE` & `gspsa_gradients-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gspsa-gradients-0.1.0/gspsa_gradients/qiskit_gradient/gspsa.py` & `gspsa_gradients-0.1.4/gspsa_gradients/qiskit_gradient/gspsa.py`

 * *Files identical despite different names*

### Comparing `gspsa-gradients-0.1.0/gspsa_gradients/tfq_gradient/gspsa.py` & `gspsa_gradients-0.1.4/gspsa_gradients/tfq_gradient/gspsa.py`

 * *Files identical despite different names*

