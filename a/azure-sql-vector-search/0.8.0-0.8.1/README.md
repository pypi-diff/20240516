# Comparing `tmp/azure_sql_vector_search-0.8.0.tar.gz` & `tmp/azure_sql_vector_search-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_sql_vector_search-0.8.0.tar", last modified: Thu May 16 00:04:25 2024, max compression
+gzip compressed data, was "azure_sql_vector_search-0.8.1.tar", last modified: Thu May 16 00:10:01 2024, max compression
```

## Comparing `azure_sql_vector_search-0.8.0.tar` & `azure_sql_vector_search-0.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 isekpo     (501) staff       (20)        0 2024-05-16 00:04:25.238138 azure_sql_vector_search-0.8.0/
--rw-r--r--   0 isekpo     (501) staff       (20)     1078 2024-05-14 16:08:51.000000 azure_sql_vector_search-0.8.0/LICENSE
--rw-r--r--   0 isekpo     (501) staff       (20)    11838 2024-05-16 00:04:25.237141 azure_sql_vector_search-0.8.0/PKG-INFO
--rw-r--r--   0 isekpo     (501) staff       (20)    11411 2024-05-16 00:00:37.000000 azure_sql_vector_search-0.8.0/README.md
-drwxr-xr-x   0 isekpo     (501) staff       (20)        0 2024-05-16 00:04:25.204646 azure_sql_vector_search-0.8.0/azure_sql_vector_search/
--rw-r--r--   0 isekpo     (501) staff       (20)      277 2024-05-15 10:49:14.000000 azure_sql_vector_search-0.8.0/azure_sql_vector_search/__init__.py
--rw-r--r--   0 isekpo     (501) staff       (20)     8979 2024-05-15 23:51:45.000000 azure_sql_vector_search-0.8.0/azure_sql_vector_search/classic_vector_search.py
--rw-r--r--   0 isekpo     (501) staff       (20)      239 2024-05-15 10:53:04.000000 azure_sql_vector_search-0.8.0/azure_sql_vector_search/models.py
--rw-r--r--   0 isekpo     (501) staff       (20)     7271 2024-05-15 23:51:58.000000 azure_sql_vector_search-0.8.0/azure_sql_vector_search/native_vector_search.py
--rw-r--r--   0 isekpo     (501) staff       (20)     7908 2024-05-15 23:50:08.000000 azure_sql_vector_search-0.8.0/azure_sql_vector_search/vector_search_base.py
-drwxr-xr-x   0 isekpo     (501) staff       (20)        0 2024-05-16 00:04:25.236037 azure_sql_vector_search-0.8.0/azure_sql_vector_search.egg-info/
--rw-r--r--   0 isekpo     (501) staff       (20)    11838 2024-05-16 00:04:24.000000 azure_sql_vector_search-0.8.0/azure_sql_vector_search.egg-info/PKG-INFO
--rw-r--r--   0 isekpo     (501) staff       (20)      473 2024-05-16 00:04:24.000000 azure_sql_vector_search-0.8.0/azure_sql_vector_search.egg-info/SOURCES.txt
--rw-r--r--   0 isekpo     (501) staff       (20)        1 2024-05-16 00:04:24.000000 azure_sql_vector_search-0.8.0/azure_sql_vector_search.egg-info/dependency_links.txt
--rw-r--r--   0 isekpo     (501) staff       (20)       47 2024-05-16 00:04:24.000000 azure_sql_vector_search-0.8.0/azure_sql_vector_search.egg-info/requires.txt
--rw-r--r--   0 isekpo     (501) staff       (20)       24 2024-05-16 00:04:24.000000 azure_sql_vector_search-0.8.0/azure_sql_vector_search.egg-info/top_level.txt
--rw-r--r--   0 isekpo     (501) staff       (20)       38 2024-05-16 00:04:25.238281 azure_sql_vector_search-0.8.0/setup.cfg
--rw-r--r--   0 isekpo     (501) staff       (20)      689 2024-05-16 00:00:37.000000 azure_sql_vector_search-0.8.0/setup.py
+drwxr-xr-x   0 isekpo     (501) staff       (20)        0 2024-05-16 00:10:01.066294 azure_sql_vector_search-0.8.1/
+-rw-r--r--   0 isekpo     (501) staff       (20)     1078 2024-05-14 16:08:51.000000 azure_sql_vector_search-0.8.1/LICENSE
+-rw-r--r--   0 isekpo     (501) staff       (20)    11838 2024-05-16 00:10:01.064627 azure_sql_vector_search-0.8.1/PKG-INFO
+-rw-r--r--   0 isekpo     (501) staff       (20)    11411 2024-05-16 00:00:37.000000 azure_sql_vector_search-0.8.1/README.md
+drwxr-xr-x   0 isekpo     (501) staff       (20)        0 2024-05-16 00:10:01.028591 azure_sql_vector_search-0.8.1/azure_sql_vector_search/
+-rw-r--r--   0 isekpo     (501) staff       (20)      277 2024-05-15 10:49:14.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search/__init__.py
+-rw-r--r--   0 isekpo     (501) staff       (20)     8979 2024-05-15 23:51:45.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search/classic_vector_search.py
+-rw-r--r--   0 isekpo     (501) staff       (20)      239 2024-05-15 10:53:04.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search/models.py
+-rw-r--r--   0 isekpo     (501) staff       (20)     7271 2024-05-15 23:51:58.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search/native_vector_search.py
+-rw-r--r--   0 isekpo     (501) staff       (20)     7908 2024-05-15 23:50:08.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search/vector_search_base.py
+drwxr-xr-x   0 isekpo     (501) staff       (20)        0 2024-05-16 00:10:01.047203 azure_sql_vector_search-0.8.1/azure_sql_vector_search.egg-info/
+-rw-r--r--   0 isekpo     (501) staff       (20)    11838 2024-05-16 00:10:00.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search.egg-info/PKG-INFO
+-rw-r--r--   0 isekpo     (501) staff       (20)      473 2024-05-16 00:10:00.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search.egg-info/SOURCES.txt
+-rw-r--r--   0 isekpo     (501) staff       (20)        1 2024-05-16 00:10:00.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search.egg-info/dependency_links.txt
+-rw-r--r--   0 isekpo     (501) staff       (20)       47 2024-05-16 00:10:00.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search.egg-info/requires.txt
+-rw-r--r--   0 isekpo     (501) staff       (20)       24 2024-05-16 00:10:00.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search.egg-info/top_level.txt
+-rw-r--r--   0 isekpo     (501) staff       (20)       38 2024-05-16 00:10:01.066496 azure_sql_vector_search-0.8.1/setup.cfg
+-rw-r--r--   0 isekpo     (501) staff       (20)      689 2024-05-16 00:04:33.000000 azure_sql_vector_search-0.8.1/setup.py
```

### Comparing `azure_sql_vector_search-0.8.0/LICENSE` & `azure_sql_vector_search-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `azure_sql_vector_search-0.8.0/PKG-INFO` & `azure_sql_vector_search-0.8.1/azure_sql_vector_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: azure_sql_vector_search
-Version: 0.8.0
+Name: azure-sql-vector-search
+Version: 0.8.1
 Summary: Azure SQL Vector Search Clients
 Home-page: https://github.com/projectAcetylcholine/sql_vector_search
 Author: Microsoft Corporation
 License: MIT License
 Keywords: azure sql vector search langchain
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `azure_sql_vector_search-0.8.0/README.md` & `azure_sql_vector_search-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `azure_sql_vector_search-0.8.0/azure_sql_vector_search/classic_vector_search.py` & `azure_sql_vector_search-0.8.1/azure_sql_vector_search/classic_vector_search.py`

 * *Files identical despite different names*

### Comparing `azure_sql_vector_search-0.8.0/azure_sql_vector_search/native_vector_search.py` & `azure_sql_vector_search-0.8.1/azure_sql_vector_search/native_vector_search.py`

 * *Files identical despite different names*

### Comparing `azure_sql_vector_search-0.8.0/azure_sql_vector_search/vector_search_base.py` & `azure_sql_vector_search-0.8.1/azure_sql_vector_search/vector_search_base.py`

 * *Files identical despite different names*

### Comparing `azure_sql_vector_search-0.8.0/azure_sql_vector_search.egg-info/PKG-INFO` & `azure_sql_vector_search-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: azure-sql-vector-search
-Version: 0.8.0
+Name: azure_sql_vector_search
+Version: 0.8.1
 Summary: Azure SQL Vector Search Clients
 Home-page: https://github.com/projectAcetylcholine/sql_vector_search
 Author: Microsoft Corporation
 License: MIT License
 Keywords: azure sql vector search langchain
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `azure_sql_vector_search-0.8.0/setup.py` & `azure_sql_vector_search-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as readme_file:
     project_long_description = readme_file.read()
 
 project_description = "Azure SQL Vector Search Clients"
 
 setup(
     name='azure_sql_vector_search',
-    version='0.8.0',
+    version='0.8.1',
     author='Microsoft Corporation',
     url="https://github.com/projectAcetylcholine/sql_vector_search",
     packages=find_packages(),
     install_requires=['pyodbc >= 5.1.0', 'sqlalchemy >= 2.0.30', 'numpy >= 1.26.4'],
     license='MIT License',
     description=project_description,
     keywords="azure sql vector search langchain",
```

