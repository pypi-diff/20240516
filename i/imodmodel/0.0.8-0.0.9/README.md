# Comparing `tmp/imodmodel-0.0.8.tar.gz` & `tmp/imodmodel-0.0.9.tar.gz`

## Comparing `imodmodel-0.0.8.tar` & `imodmodel-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 imodmodel-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 imodmodel-0.0.8/MANIFEST.in
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 imodmodel-0.0.8/mkdocs.yml
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 imodmodel-0.0.8/.github/workflows/build-and-deploy-docs.yml
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 imodmodel-0.0.8/.github/workflows/test_and_deploy.yml
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 imodmodel-0.0.8/docs/index.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 imodmodel-0.0.8/src/imodmodel/__init__.py
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 imodmodel-0.0.8/src/imodmodel/binary_specification.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 imodmodel-0.0.8/src/imodmodel/dataframe.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 imodmodel-0.0.8/src/imodmodel/functions.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 imodmodel-0.0.8/src/imodmodel/models.py
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 imodmodel-0.0.8/src/imodmodel/parsers.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 imodmodel-0.0.8/tests/conftest.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 imodmodel-0.0.8/tests/test_functional_api.py
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 imodmodel-0.0.8/tests/test_parsers.py
--rw-r--r--   0        0        0   333087 2020-02-02 00:00:00.000000 imodmodel-0.0.8/tests/test_data/meshed_contour_example.mod
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 imodmodel-0.0.8/tests/test_data/two_contour_example.mod
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 imodmodel-0.0.8/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 imodmodel-0.0.8/LICENSE
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 imodmodel-0.0.8/README.md
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 imodmodel-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 imodmodel-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 imodmodel-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 imodmodel-0.0.9/MANIFEST.in
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 imodmodel-0.0.9/mkdocs.yml
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 imodmodel-0.0.9/.github/workflows/build-and-deploy-docs.yml
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 imodmodel-0.0.9/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 imodmodel-0.0.9/docs/index.md
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 imodmodel-0.0.9/src/imodmodel/__init__.py
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 imodmodel-0.0.9/src/imodmodel/binary_specification.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 imodmodel-0.0.9/src/imodmodel/dataframe.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 imodmodel-0.0.9/src/imodmodel/functions.py
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 imodmodel-0.0.9/src/imodmodel/models.py
+-rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 imodmodel-0.0.9/src/imodmodel/parsers.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 imodmodel-0.0.9/tests/conftest.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 imodmodel-0.0.9/tests/test_functional_api.py
+-rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 imodmodel-0.0.9/tests/test_parsers.py
+-rw-r--r--   0        0        0   333087 2020-02-02 00:00:00.000000 imodmodel-0.0.9/tests/test_data/meshed_contour_example.mod
+-rw-r--r--   0        0        0    46618 2020-02-02 00:00:00.000000 imodmodel-0.0.9/tests/test_data/meshed_curvature_example.mod
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 imodmodel-0.0.9/tests/test_data/two_contour_example.mod
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 imodmodel-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 imodmodel-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 imodmodel-0.0.9/README.md
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 imodmodel-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 imodmodel-0.0.9/PKG-INFO
```

### Comparing `imodmodel-0.0.8/.pre-commit-config.yaml` & `imodmodel-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `imodmodel-0.0.8/mkdocs.yml` & `imodmodel-0.0.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `imodmodel-0.0.8/.github/workflows/build-and-deploy-docs.yml` & `imodmodel-0.0.9/.github/workflows/build-and-deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `imodmodel-0.0.8/.github/workflows/test_and_deploy.yml` & `imodmodel-0.0.9/.github/workflows/test_and_deploy.yml`

 * *Files 8% similar despite different names*

```diff
@@ -34,18 +34,19 @@
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install setuptools pytest
+          pip install setuptools pytest pipx
           pip install -e .
+          pipx install hatch
       - name: Test with pytest
-        run: pytest -v -p no:warnings tests
+        run: hatch run all:test -v -p no:warnings tests
         env:
           PLATFORM: ${{ matrix.platform }}
 
       - name: Coverage
         uses: codecov/codecov-action@v1
 
   deploy:
```

### Comparing `imodmodel-0.0.8/docs/index.md` & `imodmodel-0.0.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `imodmodel-0.0.8/src/imodmodel/binary_specification.py` & `imodmodel-0.0.9/src/imodmodel/binary_specification.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,14 +57,21 @@
     }
     CONTOUR_HEADER = {
         'psize': 'i',
         'flags': 'I',
         'time': 'i',
         'surf': 'i',
     }
+    MESH_HEADER = {
+        'vsize': 'i',
+        'lsize': 'i',
+        'flag': 'I',
+        'time': 'h',
+        'surf': 'h',
+    }
     IMAT = {
         'ambient': 'B',
         'diffuse': 'B',
         'specular': 'B',
         'shininess': 'B',
         'fillred': 'B',
         'fillgreen': 'B',
@@ -100,15 +107,11 @@
     SIZE = NotImplemented
     MESH = NotImplemented
     MINX = NotImplemented
     LABL = NotImplemented
     OLBL = NotImplemented
     CLIP = NotImplemented
     MCLP = NotImplemented
-    MOST = NotImplemented
-    OBST = NotImplemented
-    COST = NotImplemented
-    MEST = NotImplemented
     SLAN = NotImplemented
     MEPA = NotImplemented
     SKLI = NotImplemented
     OGRP = NotImplemented
```

### Comparing `imodmodel-0.0.8/src/imodmodel/dataframe.py` & `imodmodel-0.0.9/src/imodmodel/dataframe.py`

 * *Files identical despite different names*

### Comparing `imodmodel-0.0.8/tests/test_data/meshed_contour_example.mod` & `imodmodel-0.0.9/tests/test_data/meshed_contour_example.mod`

 * *Files identical despite different names*

### Comparing `imodmodel-0.0.8/tests/test_data/two_contour_example.mod` & `imodmodel-0.0.9/tests/test_data/two_contour_example.mod`

 * *Files identical despite different names*

### Comparing `imodmodel-0.0.8/.gitignore` & `imodmodel-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `imodmodel-0.0.8/LICENSE` & `imodmodel-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `imodmodel-0.0.8/README.md` & `imodmodel-0.0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 Read [IMOD model files](https://bio3d.colorado.edu/imod/doc/binspec.html) 
 as [pandas dataframes](https://pandas.pydata.org/) 
 in Python.
 
 
 ## Usage
 
+### As pandas DataFrame
+
 ```python
 import imodmodel
 
 df = imodmodel.read('my_model_file.mod')
 ```
 
 ```ipython
@@ -27,14 +29,39 @@
 2          0           0  51.333332  45.666668  80.0
 3          0           0  87.333336  49.666668  80.0
 4          0           0  76.000000  82.000000  80.0
 
 
 ```
 
+### As ImodModel object
+
+```python
+from imodmodel import ImodModel
+model = ImodModel.from_file("my_model_file.mod")
+```
+
+```ipython
+In [3]: model.objects[0].contours[0].points
+Out[3]: 
+array([[  6.875,  62.875, 124.   ], ...])
+
+In [4]: model.objects[0].meshes[0].vertices
+Out[4]: 
+array([[ 6.87500000e+00,  6.28750000e+01,  1.24000000e+02], ...])
+
+In [5]: model.objects[0].meshes[0].indices
+Out[5]: 
+array([[156,  18, 152], ...])
+
+In [6]: model.objects[0].meshes[0].face_values
+Out[6]: 
+array([0., 0., 35.22094345, ...])
+```
+
 That's it!
 
 ## Installation
 `imodmodel` can be installed from the [Python Package Index](https://pypi.org/) (PyPI)
 
 ```shell
 pip install imodmodel
```

### Comparing `imodmodel-0.0.8/pyproject.toml` & `imodmodel-0.0.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -96,14 +96,34 @@
     "D413", # Missing blank line after last section
     "D416", # Section name should end with a colon
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*.py" = ["D"]
 
+[tool.hatch.envs.default]
+dependencies = [
+  "pytest",
+]
+
+[tool.hatch.envs.default.scripts]
+test = "pytest {args:tests}"
+
+[tool.hatch.envs.all]
+matrix-name-format = "{variable}_{value}"
+
+[[tool.hatch.envs.all.matrix]]
+pydantic_version = ["1","2"]
+
+[tool.hatch.envs.all.overrides]
+matrix.pydantic_version.dependencies = [
+    { value="pydantic<2", if = ["1"] },
+    { value="pydantic>=2", if = ["2"] }
+]
+
 # https://docs.pytest.org/en/6.2.x/customize.html
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["tests"]
 filterwarnings = [
     "error",
     "ignore::DeprecationWarning"
```

### Comparing `imodmodel-0.0.8/PKG-INFO` & `imodmodel-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imodmodel
-Version: 0.0.8
+Version: 0.0.9
 Summary: IMOD model files as pandas DataFrames in Python.
 Project-URL: homepage, https://github.com/teamtomo/imodmodel
 Project-URL: repository, https://github.com/teamtomo/imodmodel
 Author: Alister Burt
 Author-email: alisterburt@gmail.com
 License: BSD 3-Clause License
 License-File: LICENSE
@@ -45,14 +45,16 @@
 Read [IMOD model files](https://bio3d.colorado.edu/imod/doc/binspec.html) 
 as [pandas dataframes](https://pandas.pydata.org/) 
 in Python.
 
 
 ## Usage
 
+### As pandas DataFrame
+
 ```python
 import imodmodel
 
 df = imodmodel.read('my_model_file.mod')
 ```
 
 ```ipython
@@ -64,14 +66,39 @@
 2          0           0  51.333332  45.666668  80.0
 3          0           0  87.333336  49.666668  80.0
 4          0           0  76.000000  82.000000  80.0
 
 
 ```
 
+### As ImodModel object
+
+```python
+from imodmodel import ImodModel
+model = ImodModel.from_file("my_model_file.mod")
+```
+
+```ipython
+In [3]: model.objects[0].contours[0].points
+Out[3]: 
+array([[  6.875,  62.875, 124.   ], ...])
+
+In [4]: model.objects[0].meshes[0].vertices
+Out[4]: 
+array([[ 6.87500000e+00,  6.28750000e+01,  1.24000000e+02], ...])
+
+In [5]: model.objects[0].meshes[0].indices
+Out[5]: 
+array([[156,  18, 152], ...])
+
+In [6]: model.objects[0].meshes[0].face_values
+Out[6]: 
+array([0., 0., 35.22094345, ...])
+```
+
 That's it!
 
 ## Installation
 `imodmodel` can be installed from the [Python Package Index](https://pypi.org/) (PyPI)
 
 ```shell
 pip install imodmodel
```

