# Comparing `tmp/frequenz-client-common-0.1.0.tar.gz` & `tmp/frequenz-client-common-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-client-common-0.1.0.tar", last modified: Wed Mar 20 20:44:08 2024, max compression
+gzip compressed data, was "frequenz-client-common-0.2.0.tar", last modified: Thu May 16 14:39:09 2024, max compression
```

## Comparing `frequenz-client-common-0.1.0.tar` & `frequenz-client-common-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:44:08.755751 frequenz-client-common-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-20 20:43:55.000000 frequenz-client-common-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-20 20:43:55.000000 frequenz-client-common-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-03-20 20:44:08.755751 frequenz-client-common-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-20 20:43:55.000000 frequenz-client-common-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-20 20:43:55.000000 frequenz-client-common-0.1.0/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-03-20 20:43:55.000000 frequenz-client-common-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 20:44:08.755751 frequenz-client-common-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:44:08.751751 frequenz-client-common-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:44:08.751751 frequenz-client-common-0.1.0/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:44:08.751751 frequenz-client-common-0.1.0/src/frequenz/client/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:44:08.751751 frequenz-client-common-0.1.0/src/frequenz/client/common/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-20 20:43:55.000000 frequenz-client-common-0.1.0/src/frequenz/client/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-20 20:43:55.000000 frequenz-client-common-0.1.0/src/frequenz/client/common/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:44:08.751751 frequenz-client-common-0.1.0/src/frequenz/client/common/metric/
--rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-03-20 20:43:55.000000 frequenz-client-common-0.1.0/src/frequenz/client/common/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:44:08.751751 frequenz-client-common-0.1.0/src/frequenz/client/common/microgrid/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-20 20:43:55.000000 frequenz-client-common-0.1.0/src/frequenz/client/common/microgrid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:44:08.751751 frequenz-client-common-0.1.0/src/frequenz/client/common/microgrid/components/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-20 20:43:55.000000 frequenz-client-common-0.1.0/src/frequenz/client/common/microgrid/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:44:08.755751 frequenz-client-common-0.1.0/src/frequenz/client/common/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-20 20:43:55.000000 frequenz-client-common-0.1.0/src/frequenz/client/common/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 20:43:55.000000 frequenz-client-common-0.1.0/src/frequenz/client/common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:44:08.755751 frequenz-client-common-0.1.0/src/frequenz_client_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-03-20 20:44:08.000000 frequenz-client-common-0.1.0/src/frequenz_client_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-20 20:44:08.000000 frequenz-client-common-0.1.0/src/frequenz_client_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 20:44:08.000000 frequenz-client-common-0.1.0/src/frequenz_client_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-20 20:44:08.000000 frequenz-client-common-0.1.0/src/frequenz_client_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-20 20:44:08.000000 frequenz-client-common-0.1.0/src/frequenz_client_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:39:09.054202 frequenz-client-common-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 14:38:55.000000 frequenz-client-common-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-16 14:38:55.000000 frequenz-client-common-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-16 14:39:09.054202 frequenz-client-common-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-16 14:38:55.000000 frequenz-client-common-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-16 14:38:55.000000 frequenz-client-common-0.2.0/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-16 14:38:55.000000 frequenz-client-common-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 14:39:09.054202 frequenz-client-common-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:39:09.050202 frequenz-client-common-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:39:09.050202 frequenz-client-common-0.2.0/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:39:09.050202 frequenz-client-common-0.2.0/src/frequenz/client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:39:09.054202 frequenz-client-common-0.2.0/src/frequenz/client/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-16 14:38:55.000000 frequenz-client-common-0.2.0/src/frequenz/client/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-16 14:38:55.000000 frequenz-client-common-0.2.0/src/frequenz/client/common/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:39:09.054202 frequenz-client-common-0.2.0/src/frequenz/client/common/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-16 14:38:55.000000 frequenz-client-common-0.2.0/src/frequenz/client/common/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:39:09.054202 frequenz-client-common-0.2.0/src/frequenz/client/common/microgrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-16 14:38:55.000000 frequenz-client-common-0.2.0/src/frequenz/client/common/microgrid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:39:09.054202 frequenz-client-common-0.2.0/src/frequenz/client/common/microgrid/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-16 14:38:55.000000 frequenz-client-common-0.2.0/src/frequenz/client/common/microgrid/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:39:09.054202 frequenz-client-common-0.2.0/src/frequenz/client/common/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-16 14:38:55.000000 frequenz-client-common-0.2.0/src/frequenz/client/common/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:38:55.000000 frequenz-client-common-0.2.0/src/frequenz/client/common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:39:09.054202 frequenz-client-common-0.2.0/src/frequenz_client_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-16 14:39:09.000000 frequenz-client-common-0.2.0/src/frequenz_client_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-16 14:39:09.000000 frequenz-client-common-0.2.0/src/frequenz_client_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:39:09.000000 frequenz-client-common-0.2.0/src/frequenz_client_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-16 14:39:09.000000 frequenz-client-common-0.2.0/src/frequenz_client_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 14:39:09.000000 frequenz-client-common-0.2.0/src/frequenz_client_common.egg-info/top_level.txt
```

### Comparing `frequenz-client-common-0.1.0/LICENSE` & `frequenz-client-common-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-client-common-0.1.0/PKG-INFO` & `frequenz-client-common-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-client-common
-Version: 0.1.0
+Version: 0.2.0
 Summary: Common code and utilities for Frequenz API clients
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-client-common-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-client-common-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-client-common-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-client-common-python
```

### Comparing `frequenz-client-common-0.1.0/README.md` & `frequenz-client-common-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-client-common-0.1.0/pyproject.toml` & `frequenz-client-common-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Software Development :: Libraries",
   "Typing :: Typed",
 ]
 requires-python = ">= 3.11, < 4"
 dependencies = [
   "typing-extensions >= 4.5.0, < 5",
-  "frequenz-api-common >= 0.5.4, < 6",
+  "frequenz-api-common >= 0.6.0, < 7",
 ]
 dynamic = ["version"]
 
 [[project.authors]]
 name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
 
@@ -39,47 +39,47 @@
 dev-flake8 = [
   "flake8 == 7.0.0",
   "flake8-docstrings == 1.7.0",
   "flake8-pyproject == 1.2.3",  # For reading the flake8 config from pyproject.toml
   "pydoclint == 0.4.1",
   "pydocstyle == 6.3.0",
 ]
-dev-formatting = ["black == 24.2.0", "isort == 5.13.2"]
+dev-formatting = ["black == 24.4.2", "isort == 5.13.2"]
 dev-mkdocs = [
-  "black == 24.2.0",
-  "Markdown==3.5.2",
+  "black == 24.4.2",
+  "Markdown==3.6",
   "mike == 2.0.0",
   "mkdocs-gen-files == 0.5.0",
   "mkdocs-literate-nav == 0.6.1",
   "mkdocs-macros-plugin == 1.0.5",
-  "mkdocs-material == 9.5.12",
-  "mkdocstrings[python] == 0.24.1",
+  "mkdocs-material == 9.5.20",
+  "mkdocstrings[python] == 0.25.0",
   "frequenz-repo-config[lib] == 0.9.1",
 ]
 dev-mypy = [
-  "mypy == 1.8.0",
-  "types-Markdown == 3.5.0.20240129",
+  "mypy == 1.10.0",
+  "types-Markdown == 3.6.0.20240316",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-client-common[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
 dev-noxfile = [
-  "nox == 2023.4.22",
+  "nox == 2024.4.15",
   "frequenz-repo-config[lib] == 0.9.1",
 ]
 dev-pylint = [
   "pylint == 3.1.0",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-client-common[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
 dev-pytest = [
-  "pytest == 8.1.0",
+  "pytest == 8.2.0",
   "frequenz-repo-config[extra-lint-examples] == 0.9.1",
-  "pytest-mock == 3.12.0",
-  "pytest-asyncio == 0.23.5",
-  "async-solipsism == 0.5",
+  "pytest-mock == 3.14.0",
+  "pytest-asyncio == 0.23.6",
+  "async-solipsism == 0.6",
 ]
 dev = [
   "frequenz-client-common[dev-mkdocs,dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
 ]
 
 [project.urls]
 Documentation = "https://frequenz-floss.github.io/frequenz-client-common-python/"
```

### Comparing `frequenz-client-common-0.1.0/src/frequenz/client/common/metric/__init__.py` & `frequenz-client-common-0.2.0/src/frequenz/client/common/metric/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,21 +22,24 @@
     DC_VOLTAGE = PBMetric.METRIC_DC_VOLTAGE
     DC_CURRENT = PBMetric.METRIC_DC_CURRENT
     DC_POWER = PBMetric.METRIC_DC_POWER
 
     # General AC electricity metrics
     AC_FREQUENCY = PBMetric.METRIC_AC_FREQUENCY
     AC_VOLTAGE = PBMetric.METRIC_AC_VOLTAGE
-    AC_VOLTAGE_PHASE_1 = PBMetric.METRIC_AC_VOLTAGE_PHASE_1
-    AC_VOLTAGE_PHASE_2 = PBMetric.METRIC_AC_VOLTAGE_PHASE_2
-    AC_VOLTAGE_PHASE_3 = PBMetric.METRIC_AC_VOLTAGE_PHASE_3
-    AC_APPARENT_CURRENT = PBMetric.METRIC_AC_APPARENT_CURRENT
-    AC_APPARENT_CURRENT_PHASE_1 = PBMetric.METRIC_AC_APPARENT_CURRENT_PHASE_1
-    AC_APPARENT_CURRENT_PHASE_2 = PBMetric.METRIC_AC_APPARENT_CURRENT_PHASE_2
-    AC_APPARENT_CURRENT_PHASE_3 = PBMetric.METRIC_AC_APPARENT_CURRENT_PHASE_3
+    AC_VOLTAGE_PHASE_1_N = PBMetric.METRIC_AC_VOLTAGE_PHASE_1_N
+    AC_VOLTAGE_PHASE_2_N = PBMetric.METRIC_AC_VOLTAGE_PHASE_2_N
+    AC_VOLTAGE_PHASE_3_N = PBMetric.METRIC_AC_VOLTAGE_PHASE_3_N
+    AC_VOLTAGE_PHASE_1_PHASE_2 = PBMetric.METRIC_AC_VOLTAGE_PHASE_1_PHASE_2
+    AC_VOLTAGE_PHASE_2_PHASE_3 = PBMetric.METRIC_AC_VOLTAGE_PHASE_2_PHASE_3
+    AC_VOLTAGE_PHASE_3_PHASE_1 = PBMetric.METRIC_AC_VOLTAGE_PHASE_3_PHASE_1
+    AC_CURRENT = PBMetric.METRIC_AC_CURRENT
+    AC_CURRENT_PHASE_1 = PBMetric.METRIC_AC_CURRENT_PHASE_1
+    AC_CURRENT_PHASE_2 = PBMetric.METRIC_AC_CURRENT_PHASE_2
+    AC_CURRENT_PHASE_3 = PBMetric.METRIC_AC_CURRENT_PHASE_3
 
     # AC power metrics
     AC_APPARENT_POWER = PBMetric.METRIC_AC_APPARENT_POWER
     AC_APPARENT_POWER_PHASE_1 = PBMetric.METRIC_AC_APPARENT_POWER_PHASE_1
     AC_APPARENT_POWER_PHASE_2 = PBMetric.METRIC_AC_APPARENT_POWER_PHASE_2
     AC_APPARENT_POWER_PHASE_3 = PBMetric.METRIC_AC_APPARENT_POWER_PHASE_3
     AC_ACTIVE_POWER = PBMetric.METRIC_AC_ACTIVE_POWER
@@ -85,18 +88,26 @@
     )
     AC_REACTIVE_ENERGY = PBMetric.METRIC_AC_REACTIVE_ENERGY
     AC_REACTIVE_ENERGY_PHASE_1 = PBMetric.METRIC_AC_REACTIVE_ENERGY_PHASE_1
     AC_REACTIVE_ENERGY_PHASE_2 = PBMetric.METRIC_AC_REACTIVE_ENERGY_PHASE_2
     AC_REACTIVE_ENERGY_PHASE_3 = PBMetric.METRIC_AC_REACTIVE_ENERGY_PHASE_3
 
     # AC harmonics
-    AC_THD_CURRENT = PBMetric.METRIC_AC_THD_CURRENT
-    AC_THD_CURRENT_PHASE_1 = PBMetric.METRIC_AC_THD_CURRENT_PHASE_1
-    AC_THD_CURRENT_PHASE_2 = PBMetric.METRIC_AC_THD_CURRENT_PHASE_2
-    AC_THD_CURRENT_PHASE_3 = PBMetric.METRIC_AC_THD_CURRENT_PHASE_3
+    AC_TOTAL_HARMONIC_DISTORTION_CURRENT = (
+        PBMetric.METRIC_AC_TOTAL_HARMONIC_DISTORTION_CURRENT
+    )
+    AC_TOTAL_HARMONIC_DISTORTION_CURRENT_PHASE_1 = (
+        PBMetric.METRIC_AC_TOTAL_HARMONIC_DISTORTION_CURRENT_PHASE_1
+    )
+    AC_TOTAL_HARMONIC_DISTORTION_CURRENT_PHASE_2 = (
+        PBMetric.METRIC_AC_TOTAL_HARMONIC_DISTORTION_CURRENT_PHASE_2
+    )
+    AC_TOTAL_HARMONIC_DISTORTION_CURRENT_PHASE_3 = (
+        PBMetric.METRIC_AC_TOTAL_HARMONIC_DISTORTION_CURRENT_PHASE_3
+    )
 
     # General BMS metrics
     BATTERY_CAPACITY = PBMetric.METRIC_BATTERY_CAPACITY
     BATTERY_SOC_PCT = PBMetric.METRIC_BATTERY_SOC_PCT
     BATTERY_TEMPERATURE = PBMetric.METRIC_BATTERY_TEMPERATURE
 
     # General inverter metrics
```

### Comparing `frequenz-client-common-0.1.0/src/frequenz/client/common/microgrid/components/__init__.py` & `frequenz-client-common-0.2.0/src/frequenz/client/common/microgrid/components/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-client-common-0.1.0/src/frequenz/client/common/pagination/__init__.py` & `frequenz-client-common-0.2.0/src/frequenz/client/common/pagination/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-client-common-0.1.0/src/frequenz_client_common.egg-info/PKG-INFO` & `frequenz-client-common-0.2.0/src/frequenz_client_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-client-common
-Version: 0.1.0
+Version: 0.2.0
 Summary: Common code and utilities for Frequenz API clients
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-client-common-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-client-common-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-client-common-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-client-common-python
```

### Comparing `frequenz-client-common-0.1.0/src/frequenz_client_common.egg-info/SOURCES.txt` & `frequenz-client-common-0.2.0/src/frequenz_client_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frequenz-client-common-0.1.0/src/frequenz_client_common.egg-info/requires.txt` & `frequenz-client-common-0.2.0/src/frequenz_client_common.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 typing-extensions<5,>=4.5.0
-frequenz-api-common<6,>=0.5.4
+frequenz-api-common<7,>=0.6.0
 
 [dev]
 frequenz-client-common[dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]
 
 [dev-flake8]
 flake8==7.0.0
 flake8-docstrings==1.7.0
 flake8-pyproject==1.2.3
 pydoclint==0.4.1
 pydocstyle==6.3.0
 
 [dev-formatting]
-black==24.2.0
+black==24.4.2
 isort==5.13.2
 
 [dev-mkdocs]
-black==24.2.0
-Markdown==3.5.2
+black==24.4.2
+Markdown==3.6
 mike==2.0.0
 mkdocs-gen-files==0.5.0
 mkdocs-literate-nav==0.6.1
 mkdocs-macros-plugin==1.0.5
-mkdocs-material==9.5.12
-mkdocstrings[python]==0.24.1
+mkdocs-material==9.5.20
+mkdocstrings[python]==0.25.0
 frequenz-repo-config[lib]==0.9.1
 
 [dev-mypy]
-mypy==1.8.0
-types-Markdown==3.5.0.20240129
+mypy==1.10.0
+types-Markdown==3.6.0.20240316
 frequenz-client-common[dev-mkdocs,dev-noxfile,dev-pytest]
 
 [dev-noxfile]
-nox==2023.4.22
+nox==2024.4.15
 frequenz-repo-config[lib]==0.9.1
 
 [dev-pylint]
 pylint==3.1.0
 frequenz-client-common[dev-mkdocs,dev-noxfile,dev-pytest]
 
 [dev-pytest]
-pytest==8.1.0
+pytest==8.2.0
 frequenz-repo-config[extra-lint-examples]==0.9.1
-pytest-mock==3.12.0
-pytest-asyncio==0.23.5
-async-solipsism==0.5
+pytest-mock==3.14.0
+pytest-asyncio==0.23.6
+async-solipsism==0.6
```

