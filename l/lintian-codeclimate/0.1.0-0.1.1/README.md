# Comparing `tmp/lintian_codeclimate-0.1.0.tar.gz` & `tmp/lintian_codeclimate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lintian_codeclimate-0.1.0.tar", last modified: Wed May 15 09:57:48 2024, max compression
+gzip compressed data, was "lintian_codeclimate-0.1.1.tar", last modified: Thu May 16 11:45:36 2024, max compression
```

## Comparing `lintian_codeclimate-0.1.0.tar` & `lintian_codeclimate-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 09:57:48.415068 lintian_codeclimate-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)      432 2024-05-15 09:57:42.000000 lintian_codeclimate-0.1.0/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-15 09:57:42.000000 lintian_codeclimate-0.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2470 2024-05-15 09:57:42.000000 lintian_codeclimate-0.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1083 2024-05-15 09:57:42.000000 lintian_codeclimate-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1265 2024-05-15 09:57:48.415068 lintian_codeclimate-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-15 09:57:42.000000 lintian_codeclimate-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 09:57:48.413068 lintian_codeclimate-0.1.0/lintian_codeclimate/
--rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-15 09:57:42.000000 lintian_codeclimate-0.1.0/lintian_codeclimate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2024-05-15 09:57:42.000000 lintian_codeclimate-0.1.0/lintian_codeclimate/__main__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-05-15 09:57:48.000000 lintian_codeclimate-0.1.0/lintian_codeclimate/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     3410 2024-05-15 09:57:42.000000 lintian_codeclimate-0.1.0/lintian_codeclimate/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 09:57:48.414068 lintian_codeclimate-0.1.0/lintian_codeclimate/tests/
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-15 09:57:42.000000 lintian_codeclimate-0.1.0/lintian_codeclimate/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2134 2024-05-15 09:57:42.000000 lintian_codeclimate-0.1.0/lintian_codeclimate/tests/test_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 09:57:48.414068 lintian_codeclimate-0.1.0/lintian_codeclimate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1265 2024-05-15 09:57:48.000000 lintian_codeclimate-0.1.0/lintian_codeclimate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      485 2024-05-15 09:57:48.000000 lintian_codeclimate-0.1.0/lintian_codeclimate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 09:57:48.000000 lintian_codeclimate-0.1.0/lintian_codeclimate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-15 09:57:48.000000 lintian_codeclimate-0.1.0/lintian_codeclimate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-15 09:57:48.000000 lintian_codeclimate-0.1.0/lintian_codeclimate.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1380 2024-05-15 09:57:42.000000 lintian_codeclimate-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 09:57:48.415068 lintian_codeclimate-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:45:36.047475 lintian_codeclimate-0.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)      432 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-05-16 11:45:36.047475 lintian_codeclimate-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:45:36.044475 lintian_codeclimate-0.1.1/lintian_codeclimate/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/lintian_codeclimate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/lintian_codeclimate/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-16 11:45:35.000000 lintian_codeclimate-0.1.1/lintian_codeclimate/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     7190 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/lintian_codeclimate/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:45:36.046475 lintian_codeclimate-0.1.1/lintian_codeclimate/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/lintian_codeclimate/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2134 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/lintian_codeclimate/tests/test_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:45:36.046475 lintian_codeclimate-0.1.1/lintian_codeclimate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-05-16 11:45:36.000000 lintian_codeclimate-0.1.1/lintian_codeclimate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      485 2024-05-16 11:45:36.000000 lintian_codeclimate-0.1.1/lintian_codeclimate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 11:45:36.000000 lintian_codeclimate-0.1.1/lintian_codeclimate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-16 11:45:36.000000 lintian_codeclimate-0.1.1/lintian_codeclimate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-16 11:45:36.000000 lintian_codeclimate-0.1.1/lintian_codeclimate.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1380 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 11:45:36.047475 lintian_codeclimate-0.1.1/setup.cfg
```

### Comparing `lintian_codeclimate-0.1.0/.gitignore` & `lintian_codeclimate-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lintian_codeclimate-0.1.0/.gitlab-ci.yml` & `lintian_codeclimate-0.1.1/.gitlab-ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -61,14 +61,15 @@
   script:
     - python -m pytest
         --cov lintian_codeclimate
         --junit-xml junit.xml
         --pyargs lintian_codeclimate.tests
         -ra
         -v
+    - python -m coverage xml -o coverage.xml
   artifacts:
     reports:
       # coverage report
       coverage_report:
         coverage_format: cobertura
         path: coverage.xml
       # test report
```

### Comparing `lintian_codeclimate-0.1.0/LICENSE` & `lintian_codeclimate-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lintian_codeclimate-0.1.0/PKG-INFO` & `lintian_codeclimate-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lintian-codeclimate
-Version: 0.1.0
+Version: 0.1.1
 Summary: Codeclimate parser for lintian
 Author-email: Duncan Macleod <macleoddm@cardiff.ac.uk>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/duncanmmacleod/lintian-codeclimate/
 Project-URL: Bug Tracker, https://gitlab.com/duncanmmacleod/lintian-codeclimate/-/issues/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lintian_codeclimate-0.1.0/lintian_codeclimate/tests/test_parser.py` & `lintian_codeclimate-0.1.1/lintian_codeclimate/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `lintian_codeclimate-0.1.0/lintian_codeclimate.egg-info/PKG-INFO` & `lintian_codeclimate-0.1.1/lintian_codeclimate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lintian-codeclimate
-Version: 0.1.0
+Version: 0.1.1
 Summary: Codeclimate parser for lintian
 Author-email: Duncan Macleod <macleoddm@cardiff.ac.uk>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/duncanmmacleod/lintian-codeclimate/
 Project-URL: Bug Tracker, https://gitlab.com/duncanmmacleod/lintian-codeclimate/-/issues/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lintian_codeclimate-0.1.0/pyproject.toml` & `lintian_codeclimate-0.1.1/pyproject.toml`

 * *Files identical despite different names*

