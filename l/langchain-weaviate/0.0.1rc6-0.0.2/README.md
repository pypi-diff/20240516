# Comparing `tmp/langchain_weaviate-0.0.1rc6.tar.gz` & `tmp/langchain_weaviate-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_weaviate-0.0.1rc6.tar", max compression
+gzip compressed data, was "langchain_weaviate-0.0.2.tar", max compression
```

## Comparing `langchain_weaviate-0.0.1rc6.tar` & `langchain_weaviate-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-04-05 01:22:22.759948 langchain_weaviate-0.0.1rc6/LICENSE
--rw-r--r--   0        0        0     1770 2024-04-05 01:22:22.759948 langchain_weaviate-0.0.1rc6/README.md
--rw-r--r--   0        0        0      106 2024-04-05 01:22:22.759948 langchain_weaviate-0.0.1rc6/langchain_weaviate/__init__.py
--rw-r--r--   0        0        0     2083 2024-04-05 01:22:22.759948 langchain_weaviate-0.0.1rc6/langchain_weaviate/_math.py
--rw-r--r--   0        0        0        0 2024-04-05 01:22:22.759948 langchain_weaviate-0.0.1rc6/langchain_weaviate/py.typed
--rw-r--r--   0        0        0     1794 2024-04-05 01:22:22.759948 langchain_weaviate-0.0.1rc6/langchain_weaviate/utils.py
--rw-r--r--   0        0        0    18248 2024-04-05 01:22:22.759948 langchain_weaviate-0.0.1rc6/langchain_weaviate/vectorstores.py
--rw-r--r--   0        0        0     2334 2024-04-05 01:22:22.759948 langchain_weaviate-0.0.1rc6/pyproject.toml
--rw-r--r--   0        0        0     2397 1970-01-01 00:00:00.000000 langchain_weaviate-0.0.1rc6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-16 03:11:09.064927 langchain_weaviate-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1770 2024-05-16 03:11:09.064927 langchain_weaviate-0.0.2/README.md
+-rw-r--r--   0        0        0      106 2024-05-16 03:11:09.064927 langchain_weaviate-0.0.2/langchain_weaviate/__init__.py
+-rw-r--r--   0        0        0     2083 2024-05-16 03:11:09.064927 langchain_weaviate-0.0.2/langchain_weaviate/_math.py
+-rw-r--r--   0        0        0        0 2024-05-16 03:11:09.064927 langchain_weaviate-0.0.2/langchain_weaviate/py.typed
+-rw-r--r--   0        0        0     1794 2024-05-16 03:11:09.064927 langchain_weaviate-0.0.2/langchain_weaviate/utils.py
+-rw-r--r--   0        0        0    18248 2024-05-16 03:11:09.064927 langchain_weaviate-0.0.2/langchain_weaviate/vectorstores.py
+-rw-r--r--   0        0        0     3116 2024-05-16 03:11:09.068927 langchain_weaviate-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 langchain_weaviate-0.0.2/PKG-INFO
```

### Comparing `langchain_weaviate-0.0.1rc6/LICENSE` & `langchain_weaviate-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_weaviate-0.0.1rc6/README.md` & `langchain_weaviate-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `langchain_weaviate-0.0.1rc6/langchain_weaviate/_math.py` & `langchain_weaviate-0.0.2/langchain_weaviate/_math.py`

 * *Files identical despite different names*

### Comparing `langchain_weaviate-0.0.1rc6/langchain_weaviate/utils.py` & `langchain_weaviate-0.0.2/langchain_weaviate/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_weaviate-0.0.1rc6/langchain_weaviate/vectorstores.py` & `langchain_weaviate-0.0.2/langchain_weaviate/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langchain_weaviate-0.0.1rc6/PKG-INFO` & `langchain_weaviate-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: langchain-weaviate
-Version: 0.0.1rc6
+Version: 0.0.2
 Summary: An integration package connecting Weaviate and LangChain
+Home-page: https://github.com/langchain-ai/langchain-weaviate
+License: MIT
 Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain-core (>=0.1.33,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.33,<0.3)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: simsimd (>=3.6.1,<5.0.0)
 Requires-Dist: weaviate-client (>=4.0.0,<5.0.0)
+Project-URL: Repository, https://github.com/langchain-ai/langchain-weaviate
+Project-URL: Source Code, https://github.com/langchain-ai/langchain-weaviate/tree/main/libs/weaviate
 Description-Content-Type: text/markdown
 
 # langchain-weaviate
 
 ## About
 
 This package contains the [Weaviate](https://github.com/weaviate/weaviate) integrations for [LangChain](https://github.com/langchain-ai/langchain).
```

