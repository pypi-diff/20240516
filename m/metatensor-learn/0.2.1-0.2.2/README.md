# Comparing `tmp/metatensor-learn-0.2.1.tar.gz` & `tmp/metatensor_learn-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metatensor-learn-0.2.1.tar", last modified: Fri Mar  1 16:58:38 2024, max compression
+gzip compressed data, was "metatensor_learn-0.2.2.tar", last modified: Thu May 16 14:04:25 2024, max compression
```

## Comparing `metatensor-learn-0.2.1.tar` & `metatensor_learn-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:58:38.968113 metatensor-learn-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-01 16:58:16.000000 metatensor-learn-0.2.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-01 16:58:16.000000 metatensor-learn-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-01 16:58:16.000000 metatensor-learn-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-01 16:58:38.968113 metatensor-learn-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-01 16:58:16.000000 metatensor-learn-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:58:38.964113 metatensor-learn-0.2.1/metatensor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:58:38.964113 metatensor-learn-0.2.1/metatensor/learn/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-01 16:58:16.000000 metatensor-learn-0.2.1/metatensor/learn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-01 16:58:16.000000 metatensor-learn-0.2.1/metatensor/learn/_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:58:38.968113 metatensor-learn-0.2.1/metatensor/learn/data/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-01 16:58:16.000000 metatensor-learn-0.2.1/metatensor/learn/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-03-01 16:58:16.000000 metatensor-learn-0.2.1/metatensor/learn/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-01 16:58:16.000000 metatensor-learn-0.2.1/metatensor/learn/data/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-03-01 16:58:16.000000 metatensor-learn-0.2.1/metatensor/learn/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:58:38.968113 metatensor-learn-0.2.1/metatensor/learn/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-01 16:58:16.000000 metatensor-learn-0.2.1/metatensor/learn/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-03-01 16:58:16.000000 metatensor-learn-0.2.1/metatensor/learn/nn/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-03-01 16:58:16.000000 metatensor-learn-0.2.1/metatensor/learn/nn/module_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:58:38.968113 metatensor-learn-0.2.1/metatensor_learn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-01 16:58:38.000000 metatensor-learn-0.2.1/metatensor_learn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-01 16:58:38.000000 metatensor-learn-0.2.1/metatensor_learn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 16:58:38.000000 metatensor-learn-0.2.1/metatensor_learn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-01 16:58:38.000000 metatensor-learn-0.2.1/metatensor_learn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-01 16:58:38.000000 metatensor-learn-0.2.1/metatensor_learn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 16:58:38.000000 metatensor-learn-0.2.1/metatensor_learn.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 16:58:38.000000 metatensor-learn-0.2.1/n_commits_since_last_tag
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-03-01 16:58:16.000000 metatensor-learn-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 16:58:38.968113 metatensor-learn-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-03-01 16:58:16.000000 metatensor-learn-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:58:38.968113 metatensor-learn-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-01 16:58:16.000000 metatensor-learn-0.2.1/tests/test_dummmy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:04:25.218068 metatensor_learn-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-16 14:04:25.218068 metatensor_learn-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:04:25.210067 metatensor_learn-0.2.2/metatensor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:04:25.214067 metatensor_learn-0.2.2/metatensor/learn/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/metatensor/learn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/metatensor/learn/_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:04:25.214067 metatensor_learn-0.2.2/metatensor/learn/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/metatensor/learn/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/metatensor/learn/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/metatensor/learn/data/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/metatensor/learn/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:04:25.214067 metatensor_learn-0.2.2/metatensor/learn/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/metatensor/learn/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/metatensor/learn/nn/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/metatensor/learn/nn/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/metatensor/learn/nn/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/metatensor/learn/nn/module_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/metatensor/learn/nn/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/metatensor/learn/nn/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/metatensor/learn/nn/silu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/metatensor/learn/nn/tanh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:04:25.218068 metatensor_learn-0.2.2/metatensor_learn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-16 14:04:25.000000 metatensor_learn-0.2.2/metatensor_learn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-16 14:04:25.000000 metatensor_learn-0.2.2/metatensor_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:04:25.000000 metatensor_learn-0.2.2/metatensor_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 14:04:25.000000 metatensor_learn-0.2.2/metatensor_learn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 14:04:25.000000 metatensor_learn-0.2.2/metatensor_learn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:04:24.000000 metatensor_learn-0.2.2/metatensor_learn.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:04:25.000000 metatensor_learn-0.2.2/n_commits_since_last_tag
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 14:04:25.218068 metatensor_learn-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:04:25.218068 metatensor_learn-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-16 14:04:01.000000 metatensor_learn-0.2.2/tests/test_dummmy.py
```

### Comparing `metatensor-learn-0.2.1/LICENSE` & `metatensor_learn-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metatensor-learn-0.2.1/PKG-INFO` & `metatensor_learn-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: metatensor-learn
-Version: 0.2.1
+Version: 0.2.2
 Summary: Building blocks for the atomistic machine learning models based on PyTorch and NumPy
 Author: Guillaume Fraux, Davide Tisi, Philip Loche, Joseph W. Abbott, Jigyasa Nigam, Chiheb Ben Mahmoud
 License: BSD-3-Clause
-Project-URL: homepage, https://lab-cosmo.github.io/metatensor/latest/
-Project-URL: documentation, https://lab-cosmo.github.io/metatensor/latest/
+Project-URL: homepage, https://docs.metatensor.org/latest/
+Project-URL: documentation, https://docs.metatensor.org/latest/
 Project-URL: repository, https://github.com/lab-cosmo/metatensor
-Project-URL: changelog, https://lab-cosmo.github.io/metatensor/latest/learn/CHANGELOG.html
+Project-URL: changelog, https://docs.metatensor.org/latest/learn/CHANGELOG.html
 Keywords: machine learning,molecular modeling
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `metatensor-learn-0.2.1/metatensor/learn/_backend.py` & `metatensor_learn-0.2.2/metatensor/learn/_backend.py`

 * *Files identical despite different names*

### Comparing `metatensor-learn-0.2.1/metatensor/learn/data/collate.py` & `metatensor_learn-0.2.2/metatensor/learn/data/collate.py`

 * *Files identical despite different names*

### Comparing `metatensor-learn-0.2.1/metatensor/learn/data/dataloader.py` & `metatensor_learn-0.2.2/metatensor/learn/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `metatensor-learn-0.2.1/metatensor/learn/data/dataset.py` & `metatensor_learn-0.2.2/metatensor/learn/data/dataset.py`

 * *Files identical despite different names*

### Comparing `metatensor-learn-0.2.1/metatensor/learn/nn/module_map.py` & `metatensor_learn-0.2.2/metatensor/learn/nn/module_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,14 +252,20 @@
         """
         Apply the modules on each block in ``tensor``. ``tensor`` must have the same
         set of keys as the modules used to initialize this :py:class:`ModuleMap`.
 
         :param tensor:
             input tensor map
         """
+        self._in_keys = self._in_keys.to(tensor.device)
+        if self._out_properties is not None:
+            self._out_properties = [
+                label.to(tensor.device) for label in self._out_properties
+            ]
+
         out_blocks: List[TensorBlock] = []
         for key, block in tensor.items():
             out_block = self.forward_block(key, block)
 
             for parameter, gradient in block.gradients():
                 if len(gradient.gradients_list()) != 0:
                     raise NotImplementedError(
```

### Comparing `metatensor-learn-0.2.1/metatensor_learn.egg-info/PKG-INFO` & `metatensor_learn-0.2.2/metatensor_learn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: metatensor-learn
-Version: 0.2.1
+Version: 0.2.2
 Summary: Building blocks for the atomistic machine learning models based on PyTorch and NumPy
 Author: Guillaume Fraux, Davide Tisi, Philip Loche, Joseph W. Abbott, Jigyasa Nigam, Chiheb Ben Mahmoud
 License: BSD-3-Clause
-Project-URL: homepage, https://lab-cosmo.github.io/metatensor/latest/
-Project-URL: documentation, https://lab-cosmo.github.io/metatensor/latest/
+Project-URL: homepage, https://docs.metatensor.org/latest/
+Project-URL: documentation, https://docs.metatensor.org/latest/
 Project-URL: repository, https://github.com/lab-cosmo/metatensor
-Project-URL: changelog, https://lab-cosmo.github.io/metatensor/latest/learn/CHANGELOG.html
+Project-URL: changelog, https://docs.metatensor.org/latest/learn/CHANGELOG.html
 Keywords: machine learning,molecular modeling
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `metatensor-learn-0.2.1/pyproject.toml` & `metatensor_learn-0.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -22,18 +22,18 @@
     "Topic :: Scientific/Engineering :: Chemistry",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [project.urls]
-homepage = "https://lab-cosmo.github.io/metatensor/latest/"
-documentation = "https://lab-cosmo.github.io/metatensor/latest/"
+homepage = "https://docs.metatensor.org/latest/"
+documentation = "https://docs.metatensor.org/latest/"
 repository = "https://github.com/lab-cosmo/metatensor"
-changelog = "https://lab-cosmo.github.io/metatensor/latest/learn/CHANGELOG.html"
+changelog = "https://docs.metatensor.org/latest/learn/CHANGELOG.html"
 
 ### ======================================================================== ###
 [build-system]
 requires = [
     "setuptools >=68",
     "packaging >=23",
 ]
```

### Comparing `metatensor-learn-0.2.1/setup.py` & `metatensor_learn-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 ROOT = os.path.realpath(os.path.dirname(__file__))
 METATENSOR_OPERATIONS = os.path.realpath(
     os.path.join(ROOT, "..", "metatensor-operations")
 )
 
-METATENSOR_LEARN_VERSION = "0.2.1"
+METATENSOR_LEARN_VERSION = "0.2.2"
 
 
 class bdist_egg_disabled(bdist_egg):
     """Disabled version of bdist_egg
 
     Prevents setup.py install performing setuptools' default easy_install,
     which it should never ever do.
```

