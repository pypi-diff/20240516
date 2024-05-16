# Comparing `tmp/effidict-0.0.6.tar.gz` & `tmp/effidict-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "effidict-0.0.6.tar", last modified: Tue Apr 30 15:30:06 2024, max compression
+gzip compressed data, was "effidict-0.0.7.tar", last modified: Thu May 16 13:37:50 2024, max compression
```

## Comparing `effidict-0.0.6.tar` & `effidict-0.0.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.269612 effidict-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.261613 effidict-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.265612 effidict-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-30 15:29:56.000000 effidict-0.0.6/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-30 15:29:56.000000 effidict-0.0.6/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-30 15:29:56.000000 effidict-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-30 15:29:56.000000 effidict-0.0.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-30 15:29:56.000000 effidict-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-30 15:30:06.269612 effidict-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-30 15:29:56.000000 effidict-0.0.6/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)    87532 2024-04-30 15:29:56.000000 effidict-0.0.6/comparative_notebook.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.265612 effidict-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-30 15:29:56.000000 effidict-0.0.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:29:56.000000 effidict-0.0.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.265612 effidict-0.0.6/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.265612 effidict-0.0.6/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    93746 2024-04-30 15:29:56.000000 effidict-0.0.6/docs/source/_static/logo_effidict.png
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-30 15:29:56.000000 effidict-0.0.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-30 15:29:56.000000 effidict-0.0.6/docs/source/effidict.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-30 15:29:56.000000 effidict-0.0.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-30 15:29:56.000000 effidict-0.0.6/docs/source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.265612 effidict-0.0.6/effidict/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 15:29:56.000000 effidict-0.0.6/effidict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-30 15:29:56.000000 effidict-0.0.6/effidict/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 15:30:06.000000 effidict-0.0.6/effidict/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-30 15:29:56.000000 effidict-0.0.6/effidict/db_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-04-30 15:29:56.000000 effidict-0.0.6/effidict/lru_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.269612 effidict-0.0.6/effidict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-30 15:30:06.000000 effidict-0.0.6/effidict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-30 15:30:06.000000 effidict-0.0.6/effidict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:30:06.000000 effidict-0.0.6/effidict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 15:30:06.000000 effidict-0.0.6/effidict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 15:30:06.000000 effidict-0.0.6/effidict.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.269612 effidict-0.0.6/images/
--rw-r--r--   0 runner    (1001) docker     (127)    59857 2024-04-30 15:29:56.000000 effidict-0.0.6/images/comparative.png
--rw-r--r--   0 runner    (1001) docker     (127)    51212 2024-04-30 15:29:56.000000 effidict-0.0.6/images/custom_100.png
--rw-r--r--   0 runner    (1001) docker     (127)    55710 2024-04-30 15:29:56.000000 effidict-0.0.6/images/custom_1000.png
--rw-r--r--   0 runner    (1001) docker     (127)    45813 2024-04-30 15:29:56.000000 effidict-0.0.6/images/custom_1000_db.png
--rw-r--r--   0 runner    (1001) docker     (127)    45280 2024-04-30 15:29:56.000000 effidict-0.0.6/images/custom_1000_db_10.png
--rw-r--r--   0 runner    (1001) docker     (127)   195221 2024-04-30 15:29:56.000000 effidict-0.0.6/images/logo_effidict.png
--rw-r--r--   0 runner    (1001) docker     (127)    93746 2024-04-30 15:29:56.000000 effidict-0.0.6/images/logo_effidict_no_bg.png
--rw-r--r--   0 runner    (1001) docker     (127)    55050 2024-04-30 15:29:56.000000 effidict-0.0.6/images/named_tuple.png
--rw-r--r--   0 runner    (1001) docker     (127)    55777 2024-04-30 15:29:56.000000 effidict-0.0.6/images/normal_dict.png
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-30 15:29:56.000000 effidict-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:30:06.269612 effidict-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.269612 effidict-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:29:56.000000 effidict-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-30 15:29:56.000000 effidict-0.0.6/tests/test_db_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-30 15:29:56.000000 effidict-0.0.6/tests/test_lru_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-30 15:29:56.000000 effidict-0.0.6/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:37:50.865218 effidict-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:37:50.857219 effidict-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:37:50.861219 effidict-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-16 13:37:39.000000 effidict-0.0.7/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-16 13:37:39.000000 effidict-0.0.7/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-16 13:37:39.000000 effidict-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-16 13:37:39.000000 effidict-0.0.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-16 13:37:39.000000 effidict-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-16 13:37:50.865218 effidict-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-16 13:37:39.000000 effidict-0.0.7/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)    87532 2024-05-16 13:37:39.000000 effidict-0.0.7/comparative_notebook.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:37:50.861219 effidict-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-16 13:37:39.000000 effidict-0.0.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:37:39.000000 effidict-0.0.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:37:50.861219 effidict-0.0.7/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:37:50.861219 effidict-0.0.7/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    93746 2024-05-16 13:37:39.000000 effidict-0.0.7/docs/source/_static/logo_effidict.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-16 13:37:39.000000 effidict-0.0.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-16 13:37:39.000000 effidict-0.0.7/docs/source/effidict.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-16 13:37:39.000000 effidict-0.0.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-16 13:37:39.000000 effidict-0.0.7/docs/source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:37:50.861219 effidict-0.0.7/effidict/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-16 13:37:39.000000 effidict-0.0.7/effidict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-16 13:37:39.000000 effidict-0.0.7/effidict/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 13:37:50.000000 effidict-0.0.7/effidict/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-16 13:37:39.000000 effidict-0.0.7/effidict/db_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-05-16 13:37:39.000000 effidict-0.0.7/effidict/lru_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:37:50.865218 effidict-0.0.7/effidict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-16 13:37:50.000000 effidict-0.0.7/effidict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-16 13:37:50.000000 effidict-0.0.7/effidict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:37:50.000000 effidict-0.0.7/effidict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 13:37:50.000000 effidict-0.0.7/effidict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 13:37:50.000000 effidict-0.0.7/effidict.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:37:50.865218 effidict-0.0.7/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    59857 2024-05-16 13:37:39.000000 effidict-0.0.7/images/comparative.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51212 2024-05-16 13:37:39.000000 effidict-0.0.7/images/custom_100.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55710 2024-05-16 13:37:39.000000 effidict-0.0.7/images/custom_1000.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45813 2024-05-16 13:37:39.000000 effidict-0.0.7/images/custom_1000_db.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45280 2024-05-16 13:37:39.000000 effidict-0.0.7/images/custom_1000_db_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)   195221 2024-05-16 13:37:39.000000 effidict-0.0.7/images/logo_effidict.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93746 2024-05-16 13:37:39.000000 effidict-0.0.7/images/logo_effidict_no_bg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55050 2024-05-16 13:37:39.000000 effidict-0.0.7/images/named_tuple.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55777 2024-05-16 13:37:39.000000 effidict-0.0.7/images/normal_dict.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-16 13:37:39.000000 effidict-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:37:50.865218 effidict-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:37:50.865218 effidict-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:37:39.000000 effidict-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-16 13:37:39.000000 effidict-0.0.7/tests/test_db_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-16 13:37:39.000000 effidict-0.0.7/tests/test_lru_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-16 13:37:39.000000 effidict-0.0.7/utils.py
```

### Comparing `effidict-0.0.6/.github/workflows/release.yaml` & `effidict-0.0.7/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/.github/workflows/test.yml` & `effidict-0.0.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/.readthedocs.yaml` & `effidict-0.0.7/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/LICENSE` & `effidict-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/PKG-INFO` & `effidict-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effidict
-Version: 0.0.6
+Version: 0.0.7
 Summary: Fast Python package providing enhanced dictionary-like data structures with advanced caching capabilities.
 Author-email: Isra Mekki <isra.mekki@helmholtz-munich.de>, Lisa Barros de Andrade e Sousa <lisa.barros.andrade.sousa@gmail.com>, Francesco Campi <francesco.campi@helmholtz-munich.de>
 Maintainer-email: Isra Mekki <isra.mekki@helmholtz-munich.de>
 Project-URL: documentation, https://oligo-designer-toolsuite.readthedocs.io/
 Project-URL: repository, https://github.com/HelmholtzAI-Consultants-Munich/oligo-designer-toolsuite
 Keywords: data structures,efficient dictionary
 Classifier: Programming Language :: Python :: 3
```

### Comparing `effidict-0.0.6/Readme.md` & `effidict-0.0.7/Readme.md`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/comparative_notebook.ipynb` & `effidict-0.0.7/comparative_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/docs/Makefile` & `effidict-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/docs/source/_static/logo_effidict.png` & `effidict-0.0.7/docs/source/_static/logo_effidict.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/docs/source/conf.py` & `effidict-0.0.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/docs/source/index.rst` & `effidict-0.0.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/effidict/_base.py` & `effidict-0.0.7/effidict/_base.py`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/effidict/db_dict.py` & `effidict-0.0.7/effidict/db_dict.py`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/effidict/lru_dict.py` & `effidict-0.0.7/effidict/lru_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,19 @@
         # Problem with joblib: don't delete the storage_path if called by joblib
         called_by_joblib = any(
             record.function == "_process_worker" for record in inspect.stack()
         )
 
         if not called_by_joblib:
             shutil.rmtree(self.storage_path)
+        else:
+            try:
+                shutil.rmtree(self.storage_path)
+            except:
+                pass
 
         del self.memory
 
 
 class LRUDBDict(EffiDictBase):
     """
     A class implementing a Least Recently Used (LRU) cache with a SQLite backend.
```

### Comparing `effidict-0.0.6/effidict.egg-info/PKG-INFO` & `effidict-0.0.7/effidict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effidict
-Version: 0.0.6
+Version: 0.0.7
 Summary: Fast Python package providing enhanced dictionary-like data structures with advanced caching capabilities.
 Author-email: Isra Mekki <isra.mekki@helmholtz-munich.de>, Lisa Barros de Andrade e Sousa <lisa.barros.andrade.sousa@gmail.com>, Francesco Campi <francesco.campi@helmholtz-munich.de>
 Maintainer-email: Isra Mekki <isra.mekki@helmholtz-munich.de>
 Project-URL: documentation, https://oligo-designer-toolsuite.readthedocs.io/
 Project-URL: repository, https://github.com/HelmholtzAI-Consultants-Munich/oligo-designer-toolsuite
 Keywords: data structures,efficient dictionary
 Classifier: Programming Language :: Python :: 3
```

### Comparing `effidict-0.0.6/effidict.egg-info/SOURCES.txt` & `effidict-0.0.7/effidict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/images/comparative.png` & `effidict-0.0.7/images/comparative.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/images/custom_100.png` & `effidict-0.0.7/images/custom_100.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/images/custom_1000.png` & `effidict-0.0.7/images/custom_1000.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/images/custom_1000_db.png` & `effidict-0.0.7/images/custom_1000_db.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/images/custom_1000_db_10.png` & `effidict-0.0.7/images/custom_1000_db_10.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/images/logo_effidict.png` & `effidict-0.0.7/images/logo_effidict.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/images/logo_effidict_no_bg.png` & `effidict-0.0.7/images/logo_effidict_no_bg.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/images/named_tuple.png` & `effidict-0.0.7/images/named_tuple.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/images/normal_dict.png` & `effidict-0.0.7/images/normal_dict.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/pyproject.toml` & `effidict-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/tests/test_db_dict.py` & `effidict-0.0.7/tests/test_db_dict.py`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/tests/test_lru_dict.py` & `effidict-0.0.7/tests/test_lru_dict.py`

 * *Files identical despite different names*

### Comparing `effidict-0.0.6/utils.py` & `effidict-0.0.7/utils.py`

 * *Files identical despite different names*

