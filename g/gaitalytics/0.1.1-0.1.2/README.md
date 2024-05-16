# Comparing `tmp/gaitalytics-0.1.1.tar.gz` & `tmp/gaitalytics-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitalytics-0.1.1.tar", last modified: Mon Mar 11 16:19:11 2024, max compression
+gzip compressed data, was "gaitalytics-0.1.2.tar", last modified: Thu May 16 15:16:17 2024, max compression
```

## Comparing `gaitalytics-0.1.1.tar` & `gaitalytics-0.1.2.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 16:19:11.506896 gaitalytics-0.1.1/
--rw-rw-rw-   0        0        0      764 2024-03-11 16:16:16.000000 gaitalytics-0.1.1/.bumpversion.cfg
--rw-rw-rw-   0        0        0     2238 2024-03-11 16:16:16.000000 gaitalytics-0.1.1/.cookiecutterrc
--rw-rw-rw-   0        0        0      195 2024-02-12 14:08:10.000000 gaitalytics-0.1.1/.coveragerc
--rw-rw-rw-   0        0        0      373 2024-02-12 14:08:10.000000 gaitalytics-0.1.1/.editorconfig
-drwxrwxrwx   0        0        0        0 2024-03-11 16:19:11.411687 gaitalytics-0.1.1/.github/
-drwxrwxrwx   0        0        0        0 2024-03-11 16:19:11.451991 gaitalytics-0.1.1/.github/workflows/
--rw-rw-rw-   0        0        0     2585 2024-02-15 10:01:51.000000 gaitalytics-0.1.1/.github/workflows/github-actions.yml
--rw-rw-rw-   0        0        0      708 2024-02-12 14:08:10.000000 gaitalytics-0.1.1/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      296 2024-02-12 14:08:10.000000 gaitalytics-0.1.1/.readthedocs.yml
--rw-rw-rw-   0        0        0       97 2024-02-12 14:08:10.000000 gaitalytics-0.1.1/AUTHORS.rst
--rw-rw-rw-   0        0        0       94 2024-02-12 14:08:10.000000 gaitalytics-0.1.1/CHANGELOG.rst
--rw-rw-rw-   0        0        0     2499 2024-02-12 14:08:10.000000 gaitalytics-0.1.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1110 2024-02-12 14:08:10.000000 gaitalytics-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      483 2024-03-11 15:44:18.000000 gaitalytics-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2625 2024-03-11 16:19:11.505876 gaitalytics-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2736 2024-03-11 16:16:16.000000 gaitalytics-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-11 16:19:11.459763 gaitalytics-0.1.1/ci/
--rw-rw-rw-   0        0        0     2951 2024-02-14 17:40:32.000000 gaitalytics-0.1.1/ci/bootstrap.py
--rw-rw-rw-   0        0        0       78 2024-02-12 14:08:10.000000 gaitalytics-0.1.1/ci/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-03-11 16:19:11.413819 gaitalytics-0.1.1/ci/templates/
-drwxrwxrwx   0        0        0        0 2024-03-11 16:19:11.413819 gaitalytics-0.1.1/ci/templates/.github/
-drwxrwxrwx   0        0        0        0 2024-03-11 16:19:11.461766 gaitalytics-0.1.1/ci/templates/.github/workflows/
--rw-rw-rw-   0        0        0     2030 2024-02-12 14:08:10.000000 gaitalytics-0.1.1/ci/templates/.github/workflows/github-actions.yml
--rw-rw-rw-   0        0        0     1256 2024-02-14 17:41:47.000000 gaitalytics-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      804 2024-02-12 14:08:10.000000 gaitalytics-0.1.1/pytest.ini
--rw-rw-rw-   0        0        0       42 2024-03-11 16:19:11.507946 gaitalytics-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3152 2024-03-11 16:16:16.000000 gaitalytics-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:19:11.416724 gaitalytics-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-11 16:19:11.487811 gaitalytics-0.1.1/src/gaitalytics/
--rw-rw-rw-   0        0        0       23 2024-03-11 16:16:16.000000 gaitalytics-0.1.1/src/gaitalytics/__init__.py
--rw-rw-rw-   0        0        0      385 2024-02-12 14:08:10.000000 gaitalytics-0.1.1/src/gaitalytics/__main__.py
--rw-rw-rw-   0        0        0    22566 2024-03-11 15:48:43.000000 gaitalytics-0.1.1/src/gaitalytics/analysis.py
--rw-rw-rw-   0        0        0    13212 2024-03-11 15:40:17.000000 gaitalytics-0.1.1/src/gaitalytics/api.py
--rw-rw-rw-   0        0        0    16461 2024-03-11 15:40:18.000000 gaitalytics-0.1.1/src/gaitalytics/c3d_reader.py
--rw-rw-rw-   0        0        0      772 2024-02-12 14:08:10.000000 gaitalytics-0.1.1/src/gaitalytics/cli.py
--rw-rw-rw-   0        0        0     6751 2024-03-11 15:40:17.000000 gaitalytics-0.1.1/src/gaitalytics/cycle.py
--rw-rw-rw-   0        0        0     3743 2024-03-11 15:40:17.000000 gaitalytics-0.1.1/src/gaitalytics/cycle_normalisation.py
--rw-rw-rw-   0        0        0    19634 2024-02-16 13:24:18.000000 gaitalytics-0.1.1/src/gaitalytics/events.py
--rw-rw-rw-   0        0        0     4734 2024-03-11 15:40:17.000000 gaitalytics-0.1.1/src/gaitalytics/file.py
--rw-rw-rw-   0        0        0    12781 2024-03-11 15:40:18.000000 gaitalytics-0.1.1/src/gaitalytics/model.py
--rw-rw-rw-   0        0        0    11216 2024-02-16 13:24:18.000000 gaitalytics-0.1.1/src/gaitalytics/modelling.py
--rw-rw-rw-   0        0        0     2511 2024-03-11 15:40:17.000000 gaitalytics-0.1.1/src/gaitalytics/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:19:11.501632 gaitalytics-0.1.1/src/gaitalytics.egg-info/
--rw-rw-rw-   0        0        0     2625 2024-03-11 16:19:11.000000 gaitalytics-0.1.1/src/gaitalytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      992 2024-03-11 16:19:11.000000 gaitalytics-0.1.1/src/gaitalytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 16:19:11.000000 gaitalytics-0.1.1/src/gaitalytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-03-11 16:19:11.000000 gaitalytics-0.1.1/src/gaitalytics.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-03-11 16:19:11.000000 gaitalytics-0.1.1/src/gaitalytics.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       93 2024-03-11 16:19:11.000000 gaitalytics-0.1.1/src/gaitalytics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-11 16:19:11.000000 gaitalytics-0.1.1/src/gaitalytics.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-11 16:19:11.503715 gaitalytics-0.1.1/tests/
--rw-rw-rw-   0        0        0      231 2024-02-12 14:08:10.000000 gaitalytics-0.1.1/tests/test_gaitalytics.py
--rw-rw-rw-   0        0        0     1731 2024-03-11 15:40:36.000000 gaitalytics-0.1.1/tox.ini
+drwxrwxrwx   0        0        0        0 2024-05-16 15:16:17.171577 gaitalytics-0.1.2/
+-rw-rw-rw-   0        0        0      764 2024-05-16 15:14:21.000000 gaitalytics-0.1.2/.bumpversion.cfg
+-rw-rw-rw-   0        0        0     2238 2024-05-16 15:14:21.000000 gaitalytics-0.1.2/.cookiecutterrc
+-rw-rw-rw-   0        0        0      195 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/.coveragerc
+-rw-rw-rw-   0        0        0      373 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/.editorconfig
+drwxrwxrwx   0        0        0        0 2024-05-16 15:16:17.126477 gaitalytics-0.1.2/.github/
+drwxrwxrwx   0        0        0        0 2024-05-16 15:16:17.145992 gaitalytics-0.1.2/.github/workflows/
+-rw-rw-rw-   0        0        0     2585 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/.github/workflows/github-actions.yml
+-rw-rw-rw-   0        0        0      708 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      296 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/.readthedocs.yml
+-rw-rw-rw-   0        0        0       97 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0       94 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     2499 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1110 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      536 2024-05-16 15:03:09.000000 gaitalytics-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    16231 2024-05-16 15:16:17.170555 gaitalytics-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    16063 2024-05-16 15:14:21.000000 gaitalytics-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-16 15:16:17.146999 gaitalytics-0.1.2/ci/
+-rw-rw-rw-   0        0        0     2951 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/ci/bootstrap.py
+-rw-rw-rw-   0        0        0       78 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/ci/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 15:16:17.127491 gaitalytics-0.1.2/ci/templates/
+drwxrwxrwx   0        0        0        0 2024-05-16 15:16:17.128515 gaitalytics-0.1.2/ci/templates/.github/
+drwxrwxrwx   0        0        0        0 2024-05-16 15:16:17.148017 gaitalytics-0.1.2/ci/templates/.github/workflows/
+-rw-rw-rw-   0        0        0     2030 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/ci/templates/.github/workflows/github-actions.yml
+-rw-rw-rw-   0        0        0     1258 2024-05-16 15:07:56.000000 gaitalytics-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      804 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/pytest.ini
+drwxrwxrwx   0        0        0        0 2024-05-16 15:16:17.128515 gaitalytics-0.1.2/resources/
+drwxrwxrwx   0        0        0        0 2024-05-16 15:16:17.149028 gaitalytics-0.1.2/resources/logo/
+-rw-rw-rw-   0        0        0    46124 2024-05-16 08:08:25.000000 gaitalytics-0.1.2/resources/logo/Gaitalytics_noBackground.png
+-rw-rw-rw-   0        0        0       42 2024-05-16 15:16:17.171577 gaitalytics-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     3152 2024-05-16 15:14:21.000000 gaitalytics-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:16:17.129532 gaitalytics-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 15:16:17.162303 gaitalytics-0.1.2/src/gaitalytics/
+-rw-rw-rw-   0        0        0       23 2024-05-16 15:14:21.000000 gaitalytics-0.1.2/src/gaitalytics/__init__.py
+-rw-rw-rw-   0        0        0      385 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/src/gaitalytics/__main__.py
+-rw-rw-rw-   0        0        0    22495 2024-05-16 11:52:44.000000 gaitalytics-0.1.2/src/gaitalytics/analysis.py
+-rw-rw-rw-   0        0        0    12808 2024-05-07 09:38:31.000000 gaitalytics-0.1.2/src/gaitalytics/api.py
+-rw-rw-rw-   0        0        0    14521 2024-05-16 15:08:24.000000 gaitalytics-0.1.2/src/gaitalytics/c3d_reader.py
+-rw-rw-rw-   0        0        0      772 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/src/gaitalytics/cli.py
+-rw-rw-rw-   0        0        0     6143 2024-05-07 09:26:53.000000 gaitalytics-0.1.2/src/gaitalytics/cycle.py
+-rw-rw-rw-   0        0        0     3834 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/src/gaitalytics/cycle_normalisation.py
+-rw-rw-rw-   0        0        0    19634 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/src/gaitalytics/events.py
+-rw-rw-rw-   0        0        0     3966 2024-05-07 09:44:08.000000 gaitalytics-0.1.2/src/gaitalytics/file.py
+-rw-rw-rw-   0        0        0    12570 2024-05-07 09:44:08.000000 gaitalytics-0.1.2/src/gaitalytics/model.py
+-rw-rw-rw-   0        0        0    11216 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/src/gaitalytics/modelling.py
+-rw-rw-rw-   0        0        0     2511 2024-05-06 05:55:04.000000 gaitalytics-0.1.2/src/gaitalytics/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:16:17.168493 gaitalytics-0.1.2/src/gaitalytics.egg-info/
+-rw-rw-rw-   0        0        0    16231 2024-05-16 15:16:17.000000 gaitalytics-0.1.2/src/gaitalytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1036 2024-05-16 15:16:17.000000 gaitalytics-0.1.2/src/gaitalytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 15:16:17.000000 gaitalytics-0.1.2/src/gaitalytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-16 15:16:17.000000 gaitalytics-0.1.2/src/gaitalytics.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-16 15:16:01.000000 gaitalytics-0.1.2/src/gaitalytics.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       93 2024-05-16 15:16:17.000000 gaitalytics-0.1.2/src/gaitalytics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-16 15:16:17.000000 gaitalytics-0.1.2/src/gaitalytics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 15:16:17.169540 gaitalytics-0.1.2/tests/
+-rw-rw-rw-   0        0        0      231 2024-05-06 05:55:05.000000 gaitalytics-0.1.2/tests/test_gaitalytics.py
+-rw-rw-rw-   0        0        0     1723 2024-05-16 15:06:02.000000 gaitalytics-0.1.2/tox.ini
```

### Comparing `gaitalytics-0.1.1/.bumpversion.cfg` & `gaitalytics-0.1.2/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.1
+current_version = 0.1.2
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `gaitalytics-0.1.1/.cookiecutterrc` & `gaitalytics-0.1.2/.cookiecutterrc`

 * *Files 0% similar despite different names*

```diff
@@ -50,12 +50,12 @@
     scrutinizer: "no"
     setup_py_uses_setuptools_scm: "no"
     sphinx_docs: "yes"
     sphinx_docs_hosting: "https://python-gaitalytics.readthedocs.org"
     sphinx_doctest: "no"
     sphinx_theme: "sphinx-rtd-theme"
     test_matrix_separate_coverage: "no"
-    version: 0.1.1
+    version: 0.1.2
     version_manager: "bump2version"
     website: "https://github.com/cereneo-foundation/python-gaitalytics"
     year_from: "2024"
     year_to: "2024"
```

### Comparing `gaitalytics-0.1.1/.github/workflows/github-actions.yml` & `gaitalytics-0.1.2/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.1/.pre-commit-config.yaml` & `gaitalytics-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.1/CONTRIBUTING.rst` & `gaitalytics-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.1/LICENSE` & `gaitalytics-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.1/ci/bootstrap.py` & `gaitalytics-0.1.2/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.1/ci/templates/.github/workflows/github-actions.yml` & `gaitalytics-0.1.2/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.1/pyproject.toml` & `gaitalytics-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -33,20 +33,20 @@
     "RSE", # flake8-raise
     "RUF", # ruff-specific rules
     "S", # flake8-bandit
     "UP", # pyupgrade
     "W", # pycodestyle warnings
 ]
 src = ["src", "tests"]
-target-version = "py39"
+target-version = "py311"
 
 [tool.ruff.lint.flake8-pytest-style]
 fixture-parentheses = false
 mark-parentheses = false
 
 [tool.ruff.lint.isort]
 forced-separate = ["conftest"]
 force-single-line = true
 
 [tool.black]
 line-length = 140
-target-version = ["py39"]
+target-version = ["py311"]
```

### Comparing `gaitalytics-0.1.1/pytest.ini` & `gaitalytics-0.1.2/pytest.ini`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.1/setup.py` & `gaitalytics-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="gaitalytics",
-    version="0.1.1",
+    version="0.1.2",
     license="MIT",
     description="Python package to extract gait analytic parameters for different kind of recordings (i.e. MOCAP, Force Plate)",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
     author="André Böni",
```

### Comparing `gaitalytics-0.1.1/src/gaitalytics/analysis.py` & `gaitalytics-0.1.2/src/gaitalytics/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,14 @@
         return data_table
 
     def get_all_point_data(self, cycle_context) -> list[model.ExtractedCyclePoint]:
         extracted_cycles = self._data_list[self._data_condition]
         context_cycle = extracted_cycles.cycle_points[cycle_context]
         return context_cycle.points
 
-    def get_subject_data(self) -> model.SubjectMeasures:
-        return self._data_list[self._data_condition].subject
-
     def get_cycles_meta_data(self, cycle_context: model.GaitEventContext) -> dict[str, any]:
         return self._data_list[self._data_condition].cycle_points[cycle_context].meta_data
 
     @staticmethod
     def split_by_phase(data: np.ndarray, meta_data: dict[str:any]) -> [np.ndarray, np.ndarray]:
         events = meta_data["Foot Off_IPSI"]
         standing = data.copy()
@@ -285,15 +282,15 @@
 
     def _calculate_step_width_side(
         self, context_position_x: np.ndarray, contra_position_x: np.ndarray, context: model.GaitEventContext
     ) -> dict[str, np.ndarray]:
         width = np.ndarray(len(context_position_x))
         for cycle_number in range(len(context_position_x)):
             width_c = abs(context_position_x[cycle_number][0] - contra_position_x[cycle_number][0])
-            width[cycle_number] = width_c / self.get_subject_data().body_height
+            width[cycle_number] = width_c
         return {f"{context.name}_step_width": width}
 
 
 class _LimbCircumductionAnalysis(AbstractAnalysis):
 
     def get_data_condition(self) -> model.ExtractedCycleDataCondition:
         return model.ExtractedCycleDataCondition.RAW_DATA
@@ -311,41 +308,40 @@
         results = self._calculate_limb_circumduction_side(right_malleoli_x_right, model.GaitEventContext.RIGHT)
         results.update(self._calculate_limb_circumduction_side(left_malleoli_x_left, model.GaitEventContext.LEFT))
         return results
 
     def _calculate_limb_circumduction_side(self, data_malleoli_x: np.ndarray, context: model.GaitEventContext) -> dict[str, np.ndarray]:
         column_label = f"{context.name}_limb_circumduction"
         limb_circum = np.ndarray(len(data_malleoli_x))
-        body_height = self.get_subject_data().body_height
         if np.nanmean(data_malleoli_x) < 0:
             data_malleoli_x = data_malleoli_x * -1
 
         for cycle_number in range(len(data_malleoli_x)):
             data = data_malleoli_x[cycle_number]
             data = data[~np.isnan(data)]
             max_value = np.nanmax(data)
             start_value = data[0]
             limb_circum[cycle_number] = max_value - start_value
-        limb_circum = limb_circum / body_height
+        limb_circum = limb_circum
 
         return {column_label: limb_circum}
 
 
 class _StepLengthAnalysis(AbstractAnalysis):
 
     def get_data_condition(self) -> model.ExtractedCycleDataCondition:
         return model.ExtractedCycleDataCondition.RAW_DATA
 
     def _analyse(self, by_phase: bool) -> dict:
         logger.info("analyse: _Step Length")
 
         left_heel_y_left = self.get_point_data(model.TranslatedLabel.LEFT_HEEL, model.GaitEventContext.LEFT)[model.AxesNames.y.value]
-        right_heel_y_left = self.get_point_data(model.TranslatedLabel.RIGHT_HEEL, model.GaitEventContext.RIGHT)[model.AxesNames.y.value]
+        right_heel_y_left = self.get_point_data(model.TranslatedLabel.RIGHT_HEEL, model.GaitEventContext.LEFT)[model.AxesNames.y.value]
 
-        left_heel_y_right = self.get_point_data(model.TranslatedLabel.LEFT_HEEL, model.GaitEventContext.LEFT)[model.AxesNames.y.value]
+        left_heel_y_right = self.get_point_data(model.TranslatedLabel.LEFT_HEEL, model.GaitEventContext.RIGHT)[model.AxesNames.y.value]
         right_heel_y_right = self.get_point_data(model.TranslatedLabel.RIGHT_HEEL, model.GaitEventContext.RIGHT)[model.AxesNames.y.value]
 
         left = self._calculate_step_length(left_heel_y_left, right_heel_y_left, model.GaitEventContext.LEFT)
         right = self._calculate_step_length(left_heel_y_right, right_heel_y_right, model.GaitEventContext.RIGHT)
         left.update(right)
         return left
 
@@ -372,19 +368,17 @@
 
         right = self._calculate_step_height(right_heel_z_right, model.GaitEventContext.RIGHT)
         left = self._calculate_step_height(left_heel_z_left, model.GaitEventContext.LEFT)
         right.update(left)
         return right
 
     def _calculate_step_height(self, context_position_x: np.ndarray, context: model.GaitEventContext) -> dict[str, np.ndarray]:
-        body_height = self.get_subject_data().body_height
         height = np.ndarray(len(context_position_x))
         for cycle_number in range(len(context_position_x)):
             height[cycle_number] = np.nanmax(context_position_x[cycle_number]) - np.nanmin(context_position_x[cycle_number])
-        height = height / body_height
 
         return {f"{context.name}_step_height": height}
 
 
 class _CycleDurationAnalysis(AbstractAnalysis):
 
     def get_data_condition(self) -> model.ExtractedCycleDataCondition:
@@ -397,48 +391,54 @@
         right_meta = self.get_cycles_meta_data(model.GaitEventContext.LEFT)
         left = self._calculate_cycle_duration(left_meta, model.GaitEventContext.LEFT)
         right = self._calculate_cycle_duration(right_meta, model.GaitEventContext.RIGHT)
         right.update(left)
         return right
 
     def _calculate_cycle_duration(self, meta_data: dict[str, any], context: model.GaitEventContext) -> dict[str, np.ndarray]:
-        frequency = self.get_subject_data().mocap_frequency
+        frequency = 100
         cycle_length = meta_data["end_frame"] - meta_data["start_frame"]
         cycle_duration = cycle_length / frequency
-        step_duration = meta_data["Foot Off_IPSI"] - meta_data["start_frame"] / frequency
-        swing_length = meta_data["end_frame"] - meta_data["Foot Off_IPSI"] / frequency
-        double_support_duration = meta_data["Foot Off_CONTRA"] - meta_data["start_frame"] / frequency
-        single_support_duration = meta_data["Foot Off_CONTRA"] - meta_data["Foot Strike_CONTRA"] / frequency
+        # step_duration = meta_data["Foot Off_IPSI"] - meta_data["start_frame"] / frequency
+        # TODO: Find litetrautre for step duration
+        stand_duration = meta_data["Foot Off_IPSI"] / frequency
+        swing_duration = (cycle_length - meta_data["Foot Off_IPSI"]) / frequency
+        double_support_duration = (
+            meta_data["Foot Off_CONTRA"] + (meta_data["Foot Off_IPSI"] - meta_data["Foot Strike_CONTRA"])
+        ) / frequency
+        single_support_duration = (
+            (meta_data["Foot Strike_CONTRA"] - meta_data["Foot Off_CONTRA"]) + (cycle_length - meta_data["Foot Off_IPSI"])
+        ) / frequency
 
-        perc_stand_duration = step_duration / cycle_duration
-        perc_swing_duration = swing_length / cycle_duration
+        perc_stand_duration = stand_duration / cycle_duration
+        perc_swing_duration = swing_duration / cycle_duration
         perc_double_support_duration = double_support_duration / cycle_duration
         perc_single_support_duration = single_support_duration / cycle_duration
         return {
-            f"{context.name}_cycle_duration": cycle_duration,
-            f"{context.name}_step_duration": step_duration,
-            f"{context.name}_swing_duration": perc_swing_duration,
-            f"{context.name}_stand_duration": perc_stand_duration,
-            f"{context.name}_double_support_duration": perc_double_support_duration,
-            f"{context.name}_single_support_duration": perc_single_support_duration,
+            f"{context.name}_cycle_duration_s": cycle_duration,
+            #   f"{context.name}_step_duration": step_duration,
+            f"{context.name}_swing_duration_prec": perc_swing_duration,
+            f"{context.name}_stand_duration_prec": perc_stand_duration,
+            f"{context.name}_double_support_duration_prec": perc_double_support_duration,
+            f"{context.name}_single_support_duration_prec": perc_single_support_duration,
         }
 
     # drag_duration_gc = np.zeros(len(data))  # %GC
     # drag_duration_swing = np.zeros(len(data))  # %swing
     # stride_speed = np.zeros(len(data))  # m/s
     # stride_length_com = np.zeros(len(data))  # %BH
     # stride_speed_com = np.zeros(len(data))  # m/s
     # length_foot_trajectory = np.zeros(len(data))  # %BH
     # length_com_trajectory = np.zeros(len(data))  # %BH
     # lateral_movement_during_swing = np.zeros(len(data))  # BH%
     # max_hip_vertical_amplitude = np.zeros(len(data))  # BH%
 
 
 class MinimalToeClearance(AbstractAnalysis):
-    logger.info("analyse: Minia")
+    logger.info("analyse: Minimal Toe Clearance")
 
     def get_data_condition(self) -> model.ExtractedCycleDataCondition:
         return model.ExtractedCycleDataCondition.RAW_DATA
 
     def _analyse(self, by_phase: bool) -> dict:
         right_toe_z = self.get_point_data(model.TranslatedLabel.RIGHT_META_2, model.GaitEventContext.RIGHT)
         left_toe_z = self.get_point_data(model.TranslatedLabel.LEFT_META_2, model.GaitEventContext.LEFT)
```

### Comparing `gaitalytics-0.1.1/src/gaitalytics/api.py` & `gaitalytics-0.1.2/src/gaitalytics/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 GAIT_EVENT_METHODE_FP = "Forceplate"
 GAIT_EVENT_METHODE_LIST = (GAIT_EVENT_METHODE_MARKER, GAIT_EVENT_METHODE_FP)
 
 GAIT_EVENT_CHECKER_CONTEXT = "context"
 GAIT_EVENT_CHECKER_SPACING = "spacing"
 GAIT_EVENT_CHECKER_LIST = (GAIT_EVENT_CHECKER_CONTEXT, GAIT_EVENT_CHECKER_SPACING)
 
-
 ANALYSIS_TIMESERIES = analysis.TimeseriesAnalysis
 ANALYSIS_TOE_CLEARANCE = analysis.MinimalToeClearance
 ANALYSIS_SPATIO_TEMP = analysis.SpatioTemporalAnalysis
 ANALYSIS_CMOS = analysis.CMosAnalysis
 ANALYSIS_MOS = analysis.MosAnalysis
 ANALYSIS_LIST = (
     ANALYSIS_TIMESERIES,
@@ -200,15 +199,14 @@
 
 
 def extract_cycles(
     c3d_file_path: str | Path,
     configs: utils.ConfigProvider,
     buffer_output_path: str | Path,
     methode: str = CYCLE_METHOD_HEEL_STRIKE,
-    anomaly_checker: list[str] = GAIT_EVENT_CHECKER_LIST,
     file_handler_class: type[c3d_reader.FileHandler] = c3d_reader.BtkFileHandler,
 ) -> model.ExtractedCycles:
     """
     extracts and returns cycles from c3d. If a buffered path is delivered data will be stored in the path in separated
     csv file. Do not edit files and structure.
 
     :param file_handler_class: Define class for handling c3d files
@@ -224,29 +222,25 @@
     # check params for validity
     c3d_file_path_obj = Path(c3d_file_path)
     buffer_output_path_obj = Path(buffer_output_path)
 
     if methode not in [CYCLE_METHOD_HEEL_STRIKE, CYCLE_METHOD_TOE_OFF]:
         raise KeyError(f"{methode} is not a valid methode")
 
-    if not all(item in GAIT_EVENT_CHECKER_LIST for item in anomaly_checker):
-        raise KeyError(f"{anomaly_checker} are not a valid anomaly checker")
-
     # read c3d
     motion_file = file_handler_class(c3d_file_path_obj)
 
     # get anomaly detection
-    checker = _get_anomaly_checker(anomaly_checker)
 
     # choose cut method
     cycle_builder = None
     if methode == CYCLE_METHOD_TOE_OFF:
-        cycle_builder = cycle.ToeOffToToeOffCycleBuilder(checker)
+        cycle_builder = cycle.ToeOffToToeOffCycleBuilder()
     elif methode == CYCLE_METHOD_HEEL_STRIKE:
-        cycle_builder = cycle.HeelStrikeToHeelStrikeCycleBuilder(checker)
+        cycle_builder = cycle.HeelStrikeToHeelStrikeCycleBuilder()
 
     # get cycles
     cycles = cycle_builder.build_cycles(motion_file)
 
     # extract cycles
     cycle_data = cycle.extract_point_cycles(configs, cycles, motion_file)
 
@@ -339,18 +333,15 @@
             results.update(result)
 
     return results
 
 
 def _create_path_object(file_path: str | Path) -> Path:
     logger.debug("_create_path_object")
-    path_obj = Path(file_path)
-    if not path_obj.exists():
-        raise FileExistsError(f"{path_obj} does not exists")
-    return path_obj
+    return Path(file_path)
 
 
 def _get_anomaly_checker(anomaly_checker: list[str]) -> events.AbstractEventAnomalyChecker:
     """
     defines checker by list of inputs
 
     :param anomaly_checker: list of checker name
```

### Comparing `gaitalytics-0.1.1/src/gaitalytics/c3d_reader.py` & `gaitalytics-0.1.2/src/gaitalytics/c3d_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import importlib
 import logging
 from abc import ABC
 from abc import abstractmethod
 from pathlib import Path
 from statistics import mean
-from typing import Optional
-from typing import Union
 
 import numpy as np
 
 import gaitalytics.model as model
 
 ANALOG_VOLTAGE_PREFIX_LABEL = "Voltage."
 
@@ -42,15 +40,15 @@
         self.clear_events()
         self.set_events(list(sorted_keys.values()))
 
     @abstractmethod
     def read_file(self):
         pass
 
-    def write_file(self, out_file_path: Optional[Union[str, Path]] = None):
+    def write_file(self, out_file_path: str | Path | None = None):
         if out_file_path is None:
             out_file_path = self._file_path
         self._write_file(str(out_file_path))
 
     @abstractmethod
     def _write_file(self, out_file_path: str):
         pass
@@ -84,23 +82,19 @@
         pass
 
     @abstractmethod
     def get_actual_start_frame(self) -> int:
         pass
 
     @abstractmethod
-    def get_subject_measures(self) -> model.SubjectMeasures:
-        pass
-
-    @abstractmethod
     def get_points_size(self) -> int:
         pass
 
     @abstractmethod
-    def get_point(self, marker_index: Union[int, str]) -> model.Point:
+    def get_point(self, marker_index: int | str) -> model.Point:
         pass
 
     @abstractmethod
     def add_point(self, new_point: model.Point):
         pass
 
 
@@ -114,25 +108,14 @@
     def aqc(self):
         return self._aqc
 
     @aqc.setter
     def aqc(self, aqc):
         self._aqc = aqc
 
-    def get_subject_measures(self) -> model.SubjectMeasures:
-        body_mass = self._aqc.GetMetaData().GetChild("PROCESSING").GetChild("Bodymass").GetInfo().ToDouble()[0]
-        body_height = self._aqc.GetMetaData().GetChild("PROCESSING").GetChild("Height").GetInfo().ToDouble()[0]
-        left_leg_length = self._aqc.GetMetaData().GetChild("PROCESSING").GetChild("LLegLength").GetInfo().ToDouble()[0]
-        right_leg_length = self._aqc.GetMetaData().GetChild("PROCESSING").GetChild("RLegLength").GetInfo().ToDouble()[0]
-        name = self._aqc.GetMetaData().GetChild("SUBJECTS").GetChild("NAMES").GetInfo().ToString()[0].strip()
-        start_frame = self._aqc.GetMetaData().GetChild("TRIAL").GetChild("ACTUAL_START_FIELD").GetInfo().ToInt()[0]
-        frequency = self._aqc.GetMetaData().GetChild("TRIAL").GetChild("CAMERA_RATE").GetInfo().ToInt()[0]
-        subject = model.SubjectMeasures(body_mass, body_height, left_leg_length, right_leg_length, name, start_frame, frequency)
-        return subject
-
     def _write_file(self, out_file_path: str):
         """
         write a c3d with Btk
 
         Args:
             out_file_path (str): filename with its path
         """
@@ -181,15 +164,15 @@
 
     def get_point_frequency(self) -> int:
         return self._aqc.GetPointFrequency()
 
     def get_actual_start_frame(self) -> int:
         return self._aqc.GetMetaData().GetChild("TRIAL").GetChild("ACTUAL_START_FIELD").GetInfo().ToInt()[0] - 1
 
-    def get_point(self, marker_index: Union[int, str]) -> model.Point:
+    def get_point(self, marker_index: int | str) -> model.Point:
         return self.map_btk_point(self._aqc.GetPoint(marker_index))
 
     def get_points_size(self) -> int:
         return self._aqc.GetPointNumber()
 
     def add_point(self, new_point: model.Point):
         point = self.btk.btkPoint(new_point.type.value)
@@ -286,28 +269,18 @@
 
     def get_point_frequency(self) -> int:
         return self._c3d["parameters"]["TRIAL"]["CAMERA_RATE"]["value"][0]
 
     def get_actual_start_frame(self) -> int:
         return self._c3d["parameters"]["TRIAL"]["ACTUAL_START_FIELD"]["value"][0]
 
-    def get_subject_measures(self) -> model.SubjectMeasures:
-        body_mass = self._c3d["parameters"]["PROCESSING"]["Bodymass"]["value"]
-        body_height = self._c3d["parameters"]["PROCESSING"]["Height"]["value"]
-        left_leg_length = self._c3d["parameters"]["PROCESSING"]["LLegLength"]["value"]
-        right_leg_length = self._c3d["parameters"]["PROCESSING"]["RLegLength"]["value"]
-        name = self._c3d["parameters"]["SUBJECTS"]["NAMES"]["value"][0]
-        frequency = self._c3d["parameters"]["TRIAL"]["CAMERA_RATE"]["value"][0]
-        start_frame = self.get_actual_start_frame()
-        return model.SubjectMeasures(body_mass, body_height, left_leg_length, right_leg_length, name, start_frame, frequency)
-
     def get_points_size(self) -> int:
         return self._c3d["parameters"]["POINT"]["USED"]["value"].tolist()[0]
 
-    def get_point(self, marker_index: Union[int, str]) -> model.Point:
+    def get_point(self, marker_index: int | str) -> model.Point:
 
         if isinstance(marker_index, str):
             index = self._c3d["parameters"]["POINT"]["LABELS"]["value"].index(marker_index)
         else:
             index = marker_index
         return self.map_ez_point(index)
 
@@ -343,15 +316,15 @@
         point.values = values
         point.type = type
         point.residuals = residuals
         return point
 
     def _add_event(self, event: model.GaitEvent):
         """
-        This function adds an event, warning two events can have the same name (it wont't override it)
+        This function adds an event, warning two events can have the same name (it won't override it)
 
         """
         used = 0
         times = [[], []]
         contexts = []
         labels = []
         descriptions = []
```

### Comparing `gaitalytics-0.1.1/src/gaitalytics/cli.py` & `gaitalytics-0.1.2/src/gaitalytics/cli.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.1/src/gaitalytics/cycle.py` & `gaitalytics-0.1.2/src/gaitalytics/cycle.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,35 +10,28 @@
 import gaitalytics.model as model
 import gaitalytics.utils as utils
 
 
 # Cycle Builder
 class CycleBuilder(ABC):
 
-    def __init__(self, event_anomaly_checker: events.AbstractEventAnomalyChecker):
-        self.eventAnomalyChecker = event_anomaly_checker
-
     def build_cycles(self, file_handler: c3d_reader.FileHandler) -> model.GaitCycleList:
         if file_handler.get_events_size() < 1:
             raise AttributeError("No Events in File")
-        else:
-            [detected, detail_tuple] = self.eventAnomalyChecker.check_events(file_handler)
-            if detected:
-                raise RuntimeError(detail_tuple)
 
         return self._build(file_handler)
 
     @abstractmethod
     def _build(self, file_handler: c3d_reader.FileHandler) -> model.GaitCycleList:
         pass
 
 
 class EventCycleBuilder(CycleBuilder):
-    def __init__(self, event_anomaly_checker: events.AbstractEventAnomalyChecker, event: model.GaitEventLabel):
-        super().__init__(event_anomaly_checker)
+    def __init__(self, event: model.GaitEventLabel):
+        super().__init__()
         self.event_label = event.value
 
     def _build(self, file_handler: c3d_reader.FileHandler) -> model.GaitCycleList:
         gait_cycles = model.GaitCycleList()
         numbers = {model.GaitEventContext.LEFT.value: 0, model.GaitEventContext.RIGHT.value: 0}
         for event_index in range(file_handler.get_events_size()):
             start_event = file_handler.get_event(event_index)
@@ -56,21 +49,21 @@
                         gait_cycles.add_cycle(cycle)
                 except IndexError:
                     pass  # If events do not match in the end this will be raised
         return gait_cycles
 
 
 class HeelStrikeToHeelStrikeCycleBuilder(EventCycleBuilder):
-    def __init__(self, event_anomaly_checker: events.AbstractEventAnomalyChecker):
-        super().__init__(event_anomaly_checker, model.GaitEventLabel.FOOT_STRIKE)
+    def __init__(self):
+        super().__init__(model.GaitEventLabel.FOOT_STRIKE)
 
 
 class ToeOffToToeOffCycleBuilder(EventCycleBuilder):
-    def __init__(self, event_anomaly_checker: events.AbstractEventAnomalyChecker):
-        super().__init__(event_anomaly_checker, model.GaitEventLabel.FOOT_OFF)
+    def __init__(self):
+        super().__init__(model.GaitEventLabel.FOOT_OFF)
 
 
 def _create_empty_table(n_axis: int, n_cycles: int, n_frames) -> np.ndarray:
     return np.full((n_axis, n_cycles, n_frames), np.nan)
 
 
 # Cycle Extractor
@@ -116,15 +109,15 @@
     meta_data = _extract_general_cycle_data(cycles, model.GaitEventContext.LEFT)
     points_left.meta_data = meta_data
 
     meta_data = _extract_general_cycle_data(cycles, model.GaitEventContext.RIGHT)
     points_right.meta_data = meta_data
     points = {model.GaitEventContext.LEFT.value: points_left, model.GaitEventContext.RIGHT.value: points_right}
 
-    return model.ExtractedCycles(model.ExtractedCycleDataCondition.RAW_DATA, file_handler.get_subject_measures(), points)
+    return model.ExtractedCycles(model.ExtractedCycleDataCondition.RAW_DATA, points)
 
 
 def _extract_general_cycle_data(cycles: model.GaitCycleList, context: model.GaitEventContext) -> dict[str, np.ndarray]:
     def add_to_dict(
         key: str, value: int, cycle_number: int, dictionary: dict[str, np.ndarray], max_cycle_length: int
     ) -> dict[str : np.ndarray]:
```

### Comparing `gaitalytics-0.1.1/src/gaitalytics/cycle_normalisation.py` & `gaitalytics-0.1.2/src/gaitalytics/cycle_normalisation.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-from __future__ import annotations
-
-import copy
-from abc import ABC
-from abc import abstractmethod
-
-import numpy as np
-
-import gaitalytics.model as model
-
-
-class TimeNormalisationAlgorithm(ABC):
-
-    def __init__(self, number_frames: int = 100):
-        self._number_frames = number_frames
-        self._data_type_fiter = {
-            model.PointDataType.MARKERS,
-            model.PointDataType.ANGLES,
-            model.PointDataType.FORCES,
-            model.PointDataType.MOMENTS,
-            model.PointDataType.POWERS,
-            model.PointDataType.SCALARS,
-            model.PointDataType.REACTIONS,
-        }
-
-    def normalise(self, raw_data: model.ExtractedCycles) -> model.ExtractedCycles:
-        norm_data = copy.deepcopy(raw_data)
-        norm_data.data_condition = model.ExtractedCycleDataCondition.NORM_DATA
-        norm_data.cycle_points = self._create_context_points(raw_data.cycle_points)
-        return norm_data
-
-    def _create_context_points(
-        self, raw_cycles: dict[model.GaitEventContext, model.ExtractedContextCycles]
-    ) -> dict[model.GaitEventContext, model.ExtractedContextCycles]:
-        norm_cycles = copy.deepcopy(raw_cycles)
-        for key in norm_cycles:
-            raw_cycle_list = raw_cycles[key]
-            norm_cycle_list = copy.deepcopy(raw_cycle_list)
-
-            points: list[model.ExtractedCyclePoint] = []
-            for point in raw_cycle_list.points:
-                points.append(self._norm_point(point))
-            norm_cycle_list.points = points
-            norm_cycle_list.meta_data = self._norm_meta_data(raw_cycle_list.meta_data)
-            norm_cycles[key] = norm_cycle_list
-
-        return norm_cycles
-
-    def _norm_meta_data(self, raw_meta_data: dict[str, np.ndarray]) -> dict[str, np.ndarray]:
-        norm_meta_data = {}
-        cycle_length = raw_meta_data["length"]
-        for meta_key in raw_meta_data:
-            if meta_key == "end_frame" or meta_key == "start_frame":
-                norm_meta_data[meta_key] = raw_meta_data[meta_key]
-            elif not meta_key == "length":
-                norm_meta_data[meta_key] = self._define_event_frame(raw_meta_data[meta_key], cycle_length, self._number_frames)
-        return norm_meta_data
-
-    def _norm_point(self, point: model.ExtractedCyclePoint) -> model.ExtractedCyclePoint:
-        shape = point.data_table.shape
-        data_table = np.full((shape[0], shape[1], self._number_frames), np.nan)
-        new_point = copy.deepcopy(point)
-        for direction_index in range(point.data_table.shape[0]):
-            for cycle_number in range(point.data_table.shape[1]):
-                data_table[direction_index, cycle_number, :] = self._run_algorithm(
-                    point.data_table[direction_index, cycle_number, :], self._number_frames
-                )
-        new_point.data_table = data_table
-        return new_point
-
-    @abstractmethod
-    def _run_algorithm(self, data: np.array, number_frames: int = 100) -> np.array:
-        pass
-
-    @abstractmethod
-    def _define_event_frame(self, event_frames: np.array, frame_number_cycle: np.array, number_frames: int = 100) -> int:
-        pass
-
-
-class LinearTimeNormalisation(TimeNormalisationAlgorithm):
-
-    def _define_event_frame(self, event_frames: np.array, frame_number_cycle: np.array, number_frames: int = 100) -> int:
-        events = event_frames / frame_number_cycle * number_frames
-        return events.round()
-
-    def _run_algorithm(self, data: np.array, number_frames: int = 100) -> np.array:
-        data = np.array(data)
-        data = data[np.logical_not(np.isnan(data))]
-        times = np.arange(0, len(data), 1)
-        times_new = np.linspace(0, len(data), num=number_frames)
-        return np.interp(times_new, times, data)
+from __future__ import annotations
+
+import copy
+from abc import ABC
+from abc import abstractmethod
+
+import numpy as np
+
+import gaitalytics.model as model
+
+
+class TimeNormalisationAlgorithm(ABC):
+
+    def __init__(self, number_frames: int = 100):
+        self._number_frames = number_frames
+        self._data_type_fiter = {
+            model.PointDataType.MARKERS,
+            model.PointDataType.ANGLES,
+            model.PointDataType.FORCES,
+            model.PointDataType.MOMENTS,
+            model.PointDataType.POWERS,
+            model.PointDataType.SCALARS,
+            model.PointDataType.REACTIONS,
+        }
+
+    def normalise(self, raw_data: model.ExtractedCycles) -> model.ExtractedCycles:
+        norm_data = copy.deepcopy(raw_data)
+        norm_data.data_condition = model.ExtractedCycleDataCondition.NORM_DATA
+        norm_data.cycle_points = self._create_context_points(raw_data.cycle_points)
+        return norm_data
+
+    def _create_context_points(
+        self, raw_cycles: dict[model.GaitEventContext, model.ExtractedContextCycles]
+    ) -> dict[model.GaitEventContext, model.ExtractedContextCycles]:
+        norm_cycles = copy.deepcopy(raw_cycles)
+        for key in norm_cycles:
+            raw_cycle_list = raw_cycles[key]
+            norm_cycle_list = copy.deepcopy(raw_cycle_list)
+
+            points: list[model.ExtractedCyclePoint] = []
+            for point in raw_cycle_list.points:
+                points.append(self._norm_point(point))
+            norm_cycle_list.points = points
+            norm_cycle_list.meta_data = self._norm_meta_data(raw_cycle_list.meta_data)
+            norm_cycles[key] = norm_cycle_list
+
+        return norm_cycles
+
+    def _norm_meta_data(self, raw_meta_data: dict[str, np.ndarray]) -> dict[str, np.ndarray]:
+        norm_meta_data = {}
+        cycle_length = raw_meta_data["length"]
+        for meta_key in raw_meta_data:
+            if meta_key == "end_frame" or meta_key == "start_frame":
+                norm_meta_data[meta_key] = raw_meta_data[meta_key]
+            elif not meta_key == "length":
+                norm_meta_data[meta_key] = self._define_event_frame(raw_meta_data[meta_key], cycle_length, self._number_frames)
+        return norm_meta_data
+
+    def _norm_point(self, point: model.ExtractedCyclePoint) -> model.ExtractedCyclePoint:
+        shape = point.data_table.shape
+        data_table = np.full((shape[0], shape[1], self._number_frames), np.nan)
+        new_point = copy.deepcopy(point)
+        for direction_index in range(point.data_table.shape[0]):
+            for cycle_number in range(point.data_table.shape[1]):
+                data_table[direction_index, cycle_number, :] = self._run_algorithm(
+                    point.data_table[direction_index, cycle_number, :], self._number_frames
+                )
+        new_point.data_table = data_table
+        return new_point
+
+    @abstractmethod
+    def _run_algorithm(self, data: np.array, number_frames: int = 100) -> np.array:
+        pass
+
+    @abstractmethod
+    def _define_event_frame(self, event_frames: np.array, frame_number_cycle: np.array, number_frames: int = 100) -> int:
+        pass
+
+
+class LinearTimeNormalisation(TimeNormalisationAlgorithm):
+
+    def _define_event_frame(self, event_frames: np.array, frame_number_cycle: np.array, number_frames: int = 100) -> int:
+        events = event_frames / frame_number_cycle * number_frames
+        return events.round()
+
+    def _run_algorithm(self, data: np.array, number_frames: int = 100) -> np.array:
+        data = np.array(data)
+        data = data[np.logical_not(np.isnan(data))]
+        times = np.arange(0, len(data), 1)
+        times_new = np.linspace(0, len(data), num=number_frames)
+        return np.interp(times_new, times, data)
```

### Comparing `gaitalytics-0.1.1/src/gaitalytics/events.py` & `gaitalytics-0.1.2/src/gaitalytics/events.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.1/src/gaitalytics/file.py` & `gaitalytics-0.1.2/src/gaitalytics/file.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,32 +34,29 @@
 
 
 class Hdf5FileStore(FileStore):
     POINT_TYPE_ATTR = "point_type"
 
     def save_extracted_cycles(self, cycle_data: model.ExtractedCycles):
         with h5py.File(self.out_path, "a") as h5_file:
-            subject = cycle_data.subject
             data_con_group = h5_file.create_group(cycle_data.data_condition.value)
-            data_con_group.attrs.update(subject.__dict__)
+            # data_con_group.attrs.update(subject.__dict__)
             for cycle_points in cycle_data.cycle_points.values():
                 self._save_datatables(cycle_points, data_con_group)
 
     def read_extracted_cycles(self) -> dict[model.ExtractedCycleDataCondition, model.ExtractedCycles]:
         with h5py.File(self.out_path, "r") as h5_file:
             extracted_cycles = {}
             for h5_group_key in h5_file:
-                subject = self._create_subject(h5_file[h5_group_key])
-
                 points = {
                     model.GaitEventContext.LEFT: self._create_context_points(h5_file[h5_group_key], model.GaitEventContext.LEFT),
                     model.GaitEventContext.RIGHT: self._create_context_points(h5_file[h5_group_key], model.GaitEventContext.RIGHT),
                 }
                 condition = model.ExtractedCycleDataCondition(h5_group_key)
-                extracted_cycles[condition] = model.ExtractedCycles(condition, subject, points)
+                extracted_cycles[condition] = model.ExtractedCycles(condition, points)
         return extracted_cycles
 
     def save_analysis(self, analysis: dict[str, np.ndarray]) -> None:
         with h5py.File(self.out_path, "a") as h5_file:
             analysis_group = h5_file.create_group("analysis")
             for key, value in analysis.items():
                 analysis_group.create_dataset(key, data=value)
@@ -90,19 +87,7 @@
 
     def _create_point(self, h5_point: h5py.Dataset) -> model.ExtractedCyclePoint:
         point_type = model.PointDataType[h5_point.attrs[self.POINT_TYPE_ATTR]]
         label = self.config.get_translated_label(h5_point.name.split("/")[3], point_type)
         point = model.ExtractedCyclePoint(label, point_type)
         point.data_table = h5_point[:]
         return point
-
-    @staticmethod
-    def _create_subject(h5_group: h5py.Group) -> model.SubjectMeasures:
-        body_height = h5_group.attrs["body_height"]
-        body_mass = h5_group.attrs["body_mass"]
-        left_leg_length = h5_group.attrs["left_leg_length"]
-        right_leg_length = h5_group.attrs["right_leg_length"]
-        start_frame = h5_group.attrs["start_frame"]
-        subject = h5_group.attrs["subject"]
-        frequency = h5_group.attrs["mocap_frequency"]
-        subject_measure = model.SubjectMeasures(body_mass, body_height, left_leg_length, right_leg_length, subject, start_frame, frequency)
-        return subject_measure
```

### Comparing `gaitalytics-0.1.1/src/gaitalytics/modelling.py` & `gaitalytics-0.1.2/src/gaitalytics/modelling.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.1/src/gaitalytics/utils.py` & `gaitalytics-0.1.2/src/gaitalytics/utils.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.1/src/gaitalytics.egg-info/SOURCES.txt` & `gaitalytics-0.1.2/src/gaitalytics.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 pytest.ini
 setup.py
 tox.ini
 .github/workflows/github-actions.yml
 ci/bootstrap.py
 ci/requirements.txt
 ci/templates/.github/workflows/github-actions.yml
+resources/logo/Gaitalytics_noBackground.png
 src/gaitalytics/__init__.py
 src/gaitalytics/__main__.py
 src/gaitalytics/analysis.py
 src/gaitalytics/api.py
 src/gaitalytics/c3d_reader.py
 src/gaitalytics/cli.py
 src/gaitalytics/cycle.py
```

### Comparing `gaitalytics-0.1.1/tox.ini` & `gaitalytics-0.1.2/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -13,97 +13,96 @@
 000000c0: 696b 692f 656e 2f6c 6174 6573 742f 7573  iki/en/latest/us
 000000d0: 6572 5f67 7569 6465 2e68 746d 6c23 6765  er_guide.html#ge
 000000e0: 6e65 7261 7469 7665 2d65 6e76 6972 6f6e  nerative-environ
 000000f0: 6d65 6e74 730d 0a5b 746f 785d 0d0a 656e  ments..[tox]..en
 00000100: 766c 6973 7420 3d0d 0a20 2020 2063 6c65  vlist =..    cle
 00000110: 616e 2c0d 0a20 2020 2063 6865 636b 2c0d  an,..    check,.
 00000120: 0a20 2020 2064 6f63 732c 0d0a 2020 2020  .    docs,..    
-00000130: 7b70 7933 392c 7079 3331 302c 7079 3331  {py39,py310,py31
-00000140: 312c 7079 3331 327d 2c0d 0a20 2020 2072  1,py312},..    r
-00000150: 6570 6f72 740d 0a69 676e 6f72 655f 6261  eport..ignore_ba
-00000160: 7365 7079 7468 6f6e 5f63 6f6e 666c 6963  sepython_conflic
-00000170: 7420 3d20 7472 7565 0d0a 0d0a 5b74 6573  t = true....[tes
-00000180: 7465 6e76 5d0d 0a62 6173 6570 7974 686f  tenv]..basepytho
-00000190: 6e20 3d0d 0a20 2320 2020 7079 7079 3339  n =.. #   pypy39
-000001a0: 3a20 7b65 6e76 3a54 4f58 5059 5448 4f4e  : {env:TOXPYTHON
-000001b0: 3a70 7970 7933 2e39 7d0d 0a20 2023 2020  :pypy3.9}..  #  
-000001c0: 7079 7079 3331 303a 207b 656e 763a 544f  pypy310: {env:TO
-000001d0: 5850 5954 484f 4e3a 7079 7079 332e 3130  XPYTHON:pypy3.10
-000001e0: 7d0d 0a20 2020 2320 2070 7970 7933 3131  }..   #  pypy311
-000001f0: 3a20 7b65 6e76 3a54 4f58 5059 5448 4f4e  : {env:TOXPYTHON
-00000200: 3a70 7970 7933 2e31 317d 0d0a 2020 2020  :pypy3.11}..    
-00000210: 2320 7079 7079 3331 323a 207b 656e 763a  # pypy312: {env:
-00000220: 544f 5850 5954 484f 4e3a 7079 7079 332e  TOXPYTHON:pypy3.
-00000230: 3132 7d0d 0a20 2020 2070 7933 393a 207b  12}..    py39: {
-00000240: 656e 763a 544f 5850 5954 484f 4e3a 7079  env:TOXPYTHON:py
-00000250: 7468 6f6e 332e 397d 0d0a 2020 2020 7079  thon3.9}..    py
-00000260: 3331 303a 207b 656e 763a 544f 5850 5954  310: {env:TOXPYT
-00000270: 484f 4e3a 7079 7468 6f6e 332e 3130 7d0d  HON:python3.10}.
-00000280: 0a20 2020 2070 7933 3131 3a20 7b65 6e76  .    py311: {env
-00000290: 3a54 4f58 5059 5448 4f4e 3a70 7974 686f  :TOXPYTHON:pytho
-000002a0: 6e33 2e31 317d 0d0a 2020 2020 7079 3331  n3.11}..    py31
-000002b0: 323a 207b 656e 763a 544f 5850 5954 484f  2: {env:TOXPYTHO
-000002c0: 4e3a 7079 7468 6f6e 332e 3132 7d0d 0a20  N:python3.12}.. 
-000002d0: 2020 207b 626f 6f74 7374 7261 702c 636c     {bootstrap,cl
-000002e0: 6561 6e2c 6368 6563 6b2c 7265 706f 7274  ean,check,report
-000002f0: 2c64 6f63 732c 636f 6465 636f 767d 3a20  ,docs,codecov}: 
-00000300: 7b65 6e76 3a54 4f58 5059 5448 4f4e 3a70  {env:TOXPYTHON:p
-00000310: 7974 686f 6e33 7d0d 0a73 6574 656e 7620  ython3}..setenv 
-00000320: 3d0d 0a20 2020 2050 5954 484f 4e50 4154  =..    PYTHONPAT
-00000330: 483d 7b74 6f78 696e 6964 6972 7d2f 7465  H={toxinidir}/te
-00000340: 7374 730d 0a20 2020 2050 5954 484f 4e55  sts..    PYTHONU
-00000350: 4e42 5546 4645 5245 443d 7965 730d 0a70  NBUFFERED=yes..p
-00000360: 6173 7365 6e76 203d 0d0a 2020 2020 2a0d  assenv =..    *.
-00000370: 0a75 7365 6465 7665 6c6f 7020 3d20 6661  .usedevelop = fa
-00000380: 6c73 650d 0a64 6570 7320 3d0d 0a20 2020  lse..deps =..   
-00000390: 2070 7974 6573 740d 0a20 2020 2070 7974   pytest..    pyt
-000003a0: 6573 742d 636f 760d 0a63 6f6d 6d61 6e64  est-cov..command
-000003b0: 7320 3d0d 0a20 2020 207b 706f 7361 7267  s =..    {posarg
-000003c0: 733a 7079 7465 7374 202d 2d63 6f76 202d  s:pytest --cov -
-000003d0: 2d63 6f76 2d72 6570 6f72 743d 7465 726d  -cov-report=term
-000003e0: 2d6d 6973 7369 6e67 202d 2d63 6f76 2d72  -missing --cov-r
-000003f0: 6570 6f72 743d 786d 6c20 2d76 7620 7465  eport=xml -vv te
-00000400: 7374 737d 0d0a 0d0a 5b74 6573 7465 6e76  sts}....[testenv
-00000410: 3a63 6865 636b 5d0d 0a64 6570 7320 3d0d  :check]..deps =.
-00000420: 0a20 2020 2064 6f63 7574 696c 730d 0a20  .    docutils.. 
-00000430: 2020 2063 6865 636b 2d6d 616e 6966 6573     check-manifes
-00000440: 740d 0a20 2020 2070 7265 2d63 6f6d 6d69  t..    pre-commi
-00000450: 740d 0a20 2020 2072 6561 646d 652d 7265  t..    readme-re
-00000460: 6e64 6572 6572 0d0a 2020 2020 7079 676d  nderer..    pygm
-00000470: 656e 7473 0d0a 2020 2020 6973 6f72 740d  ents..    isort.
-00000480: 0a73 6b69 705f 696e 7374 616c 6c20 3d20  .skip_install = 
-00000490: 7472 7565 0d0a 636f 6d6d 616e 6473 203d  true..commands =
-000004a0: 0d0a 2020 2020 7079 7468 6f6e 2073 6574  ..    python set
-000004b0: 7570 2e70 7920 6368 6563 6b20 2d2d 7374  up.py check --st
-000004c0: 7269 6374 202d 2d6d 6574 6164 6174 6120  rict --metadata 
-000004d0: 2d2d 7265 7374 7275 6374 7572 6564 7465  --restructuredte
-000004e0: 7874 0d0a 2020 2020 6368 6563 6b2d 6d61  xt..    check-ma
-000004f0: 6e69 6665 7374 202e 0d0a 2020 2020 7072  nifest ...    pr
-00000500: 652d 636f 6d6d 6974 2072 756e 202d 2d61  e-commit run --a
-00000510: 6c6c 2d66 696c 6573 202d 2d73 686f 772d  ll-files --show-
-00000520: 6469 6666 2d6f 6e2d 6661 696c 7572 650d  diff-on-failure.
-00000530: 0a0d 0a5b 7465 7374 656e 763a 646f 6373  ...[testenv:docs
-00000540: 5d0d 0a75 7365 6465 7665 6c6f 7020 3d20  ]..usedevelop = 
-00000550: 7472 7565 0d0a 6465 7073 203d 0d0a 2020  true..deps =..  
-00000560: 2020 2d72 7b74 6f78 696e 6964 6972 7d2f    -r{toxinidir}/
-00000570: 646f 6373 2f72 6571 7569 7265 6d65 6e74  docs/requirement
-00000580: 732e 7478 740d 0a63 6f6d 6d61 6e64 7320  s.txt..commands 
-00000590: 3d0d 0a20 2020 2073 7068 696e 782d 6275  =..    sphinx-bu
-000005a0: 696c 6420 7b70 6f73 6172 6773 3a2d 457d  ild {posargs:-E}
-000005b0: 202d 6220 6874 6d6c 2064 6f63 7320 6469   -b html docs di
-000005c0: 7374 2f64 6f63 730d 0a20 2020 2073 7068  st/docs..    sph
-000005d0: 696e 782d 6275 696c 6420 2d62 206c 696e  inx-build -b lin
-000005e0: 6b63 6865 636b 2064 6f63 7320 6469 7374  kcheck docs dist
-000005f0: 2f64 6f63 730d 0a0d 0a5b 7465 7374 656e  /docs....[testen
-00000600: 763a 7265 706f 7274 5d0d 0a64 6570 7320  v:report]..deps 
-00000610: 3d0d 0a20 2020 2063 6f76 6572 6167 650d  =..    coverage.
-00000620: 0a73 6b69 705f 696e 7374 616c 6c20 3d20  .skip_install = 
-00000630: 7472 7565 0d0a 636f 6d6d 616e 6473 203d  true..commands =
-00000640: 0d0a 2020 2020 636f 7665 7261 6765 2072  ..    coverage r
-00000650: 6570 6f72 740d 0a20 2020 2063 6f76 6572  eport..    cover
-00000660: 6167 6520 6874 6d6c 0d0a 0d0a 5b74 6573  age html....[tes
-00000670: 7465 6e76 3a63 6c65 616e 5d0d 0a63 6f6d  tenv:clean]..com
-00000680: 6d61 6e64 7320 3d20 636f 7665 7261 6765  mands = coverage
-00000690: 2065 7261 7365 0d0a 736b 6970 5f69 6e73   erase..skip_ins
-000006a0: 7461 6c6c 203d 2074 7275 650d 0a64 6570  tall = true..dep
-000006b0: 7320 3d0d 0a20 2020 2063 6f76 6572 6167  s =..    coverag
-000006c0: 650d 0a                                  e..
+00000130: 7b70 7933 3131 2c70 7933 3132 7d2c 0d0a  {py311,py312},..
+00000140: 2020 2020 7265 706f 7274 0d0a 6967 6e6f      report..igno
+00000150: 7265 5f62 6173 6570 7974 686f 6e5f 636f  re_basepython_co
+00000160: 6e66 6c69 6374 203d 2074 7275 650d 0a0d  nflict = true...
+00000170: 0a5b 7465 7374 656e 765d 0d0a 6261 7365  .[testenv]..base
+00000180: 7079 7468 6f6e 203d 0d0a 2023 2020 2070  python =.. #   p
+00000190: 7970 7933 393a 207b 656e 763a 544f 5850  ypy39: {env:TOXP
+000001a0: 5954 484f 4e3a 7079 7079 332e 397d 0d0a  YTHON:pypy3.9}..
+000001b0: 2020 2320 2070 7970 7933 3130 3a20 7b65    #  pypy310: {e
+000001c0: 6e76 3a54 4f58 5059 5448 4f4e 3a70 7970  nv:TOXPYTHON:pyp
+000001d0: 7933 2e31 307d 0d0a 2020 2023 2020 7079  y3.10}..   #  py
+000001e0: 7079 3331 313a 207b 656e 763a 544f 5850  py311: {env:TOXP
+000001f0: 5954 484f 4e3a 7079 7079 332e 3131 7d0d  YTHON:pypy3.11}.
+00000200: 0a20 2020 2023 2070 7970 7933 3132 3a20  .    # pypy312: 
+00000210: 7b65 6e76 3a54 4f58 5059 5448 4f4e 3a70  {env:TOXPYTHON:p
+00000220: 7970 7933 2e31 327d 0d0a 2023 2020 2070  ypy3.12}.. #   p
+00000230: 7933 393a 207b 656e 763a 544f 5850 5954  y39: {env:TOXPYT
+00000240: 484f 4e3a 7079 7468 6f6e 332e 397d 0d0a  HON:python3.9}..
+00000250: 2020 2320 2070 7933 3130 3a20 7b65 6e76    #  py310: {env
+00000260: 3a54 4f58 5059 5448 4f4e 3a70 7974 686f  :TOXPYTHON:pytho
+00000270: 6e33 2e31 307d 0d0a 2020 2023 2070 7933  n3.10}..   # py3
+00000280: 3131 3a20 7b65 6e76 3a54 4f58 5059 5448  11: {env:TOXPYTH
+00000290: 4f4e 3a70 7974 686f 6e33 2e31 317d 0d0a  ON:python3.11}..
+000002a0: 2020 2020 7079 3331 323a 207b 656e 763a      py312: {env:
+000002b0: 544f 5850 5954 484f 4e3a 7079 7468 6f6e  TOXPYTHON:python
+000002c0: 332e 3132 7d0d 0a20 2020 207b 626f 6f74  3.12}..    {boot
+000002d0: 7374 7261 702c 636c 6561 6e2c 6368 6563  strap,clean,chec
+000002e0: 6b2c 7265 706f 7274 2c64 6f63 732c 636f  k,report,docs,co
+000002f0: 6465 636f 767d 3a20 7b65 6e76 3a54 4f58  decov}: {env:TOX
+00000300: 5059 5448 4f4e 3a70 7974 686f 6e33 7d0d  PYTHON:python3}.
+00000310: 0a73 6574 656e 7620 3d0d 0a20 2020 2050  .setenv =..    P
+00000320: 5954 484f 4e50 4154 483d 7b74 6f78 696e  YTHONPATH={toxin
+00000330: 6964 6972 7d2f 7465 7374 730d 0a20 2020  idir}/tests..   
+00000340: 2050 5954 484f 4e55 4e42 5546 4645 5245   PYTHONUNBUFFERE
+00000350: 443d 7965 730d 0a70 6173 7365 6e76 203d  D=yes..passenv =
+00000360: 0d0a 2020 2020 2a0d 0a75 7365 6465 7665  ..    *..usedeve
+00000370: 6c6f 7020 3d20 6661 6c73 650d 0a64 6570  lop = false..dep
+00000380: 7320 3d0d 0a20 2020 2070 7974 6573 740d  s =..    pytest.
+00000390: 0a20 2020 2070 7974 6573 742d 636f 760d  .    pytest-cov.
+000003a0: 0a63 6f6d 6d61 6e64 7320 3d0d 0a20 2020  .commands =..   
+000003b0: 207b 706f 7361 7267 733a 7079 7465 7374   {posargs:pytest
+000003c0: 202d 2d63 6f76 202d 2d63 6f76 2d72 6570   --cov --cov-rep
+000003d0: 6f72 743d 7465 726d 2d6d 6973 7369 6e67  ort=term-missing
+000003e0: 202d 2d63 6f76 2d72 6570 6f72 743d 786d   --cov-report=xm
+000003f0: 6c20 2d76 7620 7465 7374 737d 0d0a 0d0a  l -vv tests}....
+00000400: 5b74 6573 7465 6e76 3a63 6865 636b 5d0d  [testenv:check].
+00000410: 0a64 6570 7320 3d0d 0a20 2020 2064 6f63  .deps =..    doc
+00000420: 7574 696c 730d 0a20 2020 2063 6865 636b  utils..    check
+00000430: 2d6d 616e 6966 6573 740d 0a20 2020 2070  -manifest..    p
+00000440: 7265 2d63 6f6d 6d69 740d 0a20 2020 2072  re-commit..    r
+00000450: 6561 646d 652d 7265 6e64 6572 6572 0d0a  eadme-renderer..
+00000460: 2020 2020 7079 676d 656e 7473 0d0a 2020      pygments..  
+00000470: 2020 6973 6f72 740d 0a73 6b69 705f 696e    isort..skip_in
+00000480: 7374 616c 6c20 3d20 7472 7565 0d0a 636f  stall = true..co
+00000490: 6d6d 616e 6473 203d 0d0a 2020 2020 7079  mmands =..    py
+000004a0: 7468 6f6e 2073 6574 7570 2e70 7920 6368  thon setup.py ch
+000004b0: 6563 6b20 2d2d 7374 7269 6374 202d 2d6d  eck --strict --m
+000004c0: 6574 6164 6174 6120 2d2d 7265 7374 7275  etadata --restru
+000004d0: 6374 7572 6564 7465 7874 0d0a 2020 2020  cturedtext..    
+000004e0: 6368 6563 6b2d 6d61 6e69 6665 7374 202e  check-manifest .
+000004f0: 0d0a 2020 2020 7072 652d 636f 6d6d 6974  ..    pre-commit
+00000500: 2072 756e 202d 2d61 6c6c 2d66 696c 6573   run --all-files
+00000510: 202d 2d73 686f 772d 6469 6666 2d6f 6e2d   --show-diff-on-
+00000520: 6661 696c 7572 650d 0a0d 0a5b 7465 7374  failure....[test
+00000530: 656e 763a 646f 6373 5d0d 0a75 7365 6465  env:docs]..usede
+00000540: 7665 6c6f 7020 3d20 7472 7565 0d0a 6465  velop = true..de
+00000550: 7073 203d 0d0a 2020 2020 2d72 7b74 6f78  ps =..    -r{tox
+00000560: 696e 6964 6972 7d2f 646f 6373 2f72 6571  inidir}/docs/req
+00000570: 7569 7265 6d65 6e74 732e 7478 740d 0a63  uirements.txt..c
+00000580: 6f6d 6d61 6e64 7320 3d0d 0a20 2020 2073  ommands =..    s
+00000590: 7068 696e 782d 6275 696c 6420 7b70 6f73  phinx-build {pos
+000005a0: 6172 6773 3a2d 457d 202d 6220 6874 6d6c  args:-E} -b html
+000005b0: 2064 6f63 7320 6469 7374 2f64 6f63 730d   docs dist/docs.
+000005c0: 0a20 2020 2073 7068 696e 782d 6275 696c  .    sphinx-buil
+000005d0: 6420 2d62 206c 696e 6b63 6865 636b 2064  d -b linkcheck d
+000005e0: 6f63 7320 6469 7374 2f64 6f63 730d 0a0d  ocs dist/docs...
+000005f0: 0a5b 7465 7374 656e 763a 7265 706f 7274  .[testenv:report
+00000600: 5d0d 0a64 6570 7320 3d0d 0a20 2020 2063  ]..deps =..    c
+00000610: 6f76 6572 6167 650d 0a73 6b69 705f 696e  overage..skip_in
+00000620: 7374 616c 6c20 3d20 7472 7565 0d0a 636f  stall = true..co
+00000630: 6d6d 616e 6473 203d 0d0a 2020 2020 636f  mmands =..    co
+00000640: 7665 7261 6765 2072 6570 6f72 740d 0a20  verage report.. 
+00000650: 2020 2063 6f76 6572 6167 6520 6874 6d6c     coverage html
+00000660: 0d0a 0d0a 5b74 6573 7465 6e76 3a63 6c65  ....[testenv:cle
+00000670: 616e 5d0d 0a63 6f6d 6d61 6e64 7320 3d20  an]..commands = 
+00000680: 636f 7665 7261 6765 2065 7261 7365 0d0a  coverage erase..
+00000690: 736b 6970 5f69 6e73 7461 6c6c 203d 2074  skip_install = t
+000006a0: 7275 650d 0a64 6570 7320 3d0d 0a20 2020  rue..deps =..   
+000006b0: 2063 6f76 6572 6167 650d 0a               coverage..
```

