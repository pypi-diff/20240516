# Comparing `tmp/uber_turbo-0.1.2.tar.gz` & `tmp/uber_turbo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uber_turbo-0.1.2.tar", max compression
+gzip compressed data, was "uber_turbo-0.1.3.tar", max compression
```

## Comparing `uber_turbo-0.1.2.tar` & `uber_turbo-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4816 2024-05-09 13:27:12.762546 uber_turbo-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     4226 2024-05-09 13:27:12.762648 uber_turbo-0.1.2/README.md
--rw-r--r--   0        0        0      503 2024-05-09 14:05:56.997464 uber_turbo-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       56 2024-05-09 13:27:12.763402 uber_turbo-0.1.2/turbo/__init__.py
--rw-r--r--   0        0        0     3760 2024-05-09 13:27:12.763477 uber_turbo-0.1.2/turbo/gp.py
--rw-r--r--   0        0        0    11981 2024-05-09 13:27:12.763599 uber_turbo-0.1.2/turbo/turbo_1.py
--rw-r--r--   0        0        0    10583 2024-05-09 13:27:12.763731 uber_turbo-0.1.2/turbo/turbo_m.py
--rw-r--r--   0        0        0     1746 2024-05-09 13:27:12.763795 uber_turbo-0.1.2/turbo/utils.py
--rw-r--r--   0        0        0     4803 1970-01-01 00:00:00.000000 uber_turbo-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4816 2024-05-09 13:27:12.762546 uber_turbo-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     4226 2024-05-09 13:27:12.762648 uber_turbo-0.1.3/README.md
+-rw-r--r--   0        0        0      451 2024-05-16 14:41:45.256456 uber_turbo-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-05-09 13:27:12.763402 uber_turbo-0.1.3/turbo/__init__.py
+-rw-r--r--   0        0        0     3760 2024-05-09 13:27:12.763477 uber_turbo-0.1.3/turbo/gp.py
+-rw-r--r--   0        0        0    11981 2024-05-09 13:27:12.763599 uber_turbo-0.1.3/turbo/turbo_1.py
+-rw-r--r--   0        0        0    10583 2024-05-09 13:27:12.763731 uber_turbo-0.1.3/turbo/turbo_m.py
+-rw-r--r--   0        0        0     1746 2024-05-09 13:27:12.763795 uber_turbo-0.1.3/turbo/utils.py
+-rw-r--r--   0        0        0     4807 1970-01-01 00:00:00.000000 uber_turbo-0.1.3/PKG-INFO
```

### Comparing `uber_turbo-0.1.2/LICENSE.md` & `uber_turbo-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uber_turbo-0.1.2/README.md` & `uber_turbo-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `uber_turbo-0.1.2/turbo/gp.py` & `uber_turbo-0.1.3/turbo/gp.py`

 * *Files identical despite different names*

### Comparing `uber_turbo-0.1.2/turbo/turbo_1.py` & `uber_turbo-0.1.3/turbo/turbo_1.py`

 * *Files identical despite different names*

### Comparing `uber_turbo-0.1.2/turbo/turbo_m.py` & `uber_turbo-0.1.3/turbo/turbo_m.py`

 * *Files identical despite different names*

### Comparing `uber_turbo-0.1.2/turbo/utils.py` & `uber_turbo-0.1.3/turbo/utils.py`

 * *Files identical despite different names*

### Comparing `uber_turbo-0.1.2/PKG-INFO` & `uber_turbo-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: uber-turbo
-Version: 0.1.2
+Version: 0.1.3
 Summary: Packaged fork from uber-research/TuRBO
 License: https://github.com/uber-research/TuRBO/blob/master/LICENSE.md
 Author: Uber Reasearch
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: gpytorch (==0.3.6)
+Requires-Dist: gpytorch (>=1.11,<2.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: torch (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 ## Overview
 
 This is the code-release for the TuRBO algorithm from ***Scalable Global Optimization via Local Bayesian Optimization*** appearing in NeurIPS 2019. This is an implementation for the noise-free case and may not work well if observations are noisy as the center of the trust region should be chosen based on the posterior mean in this case.
```

