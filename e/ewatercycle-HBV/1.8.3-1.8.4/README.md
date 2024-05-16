# Comparing `tmp/ewatercycle_hbv-1.8.3.tar.gz` & `tmp/ewatercycle_hbv-1.8.4.tar.gz`

## Comparing `ewatercycle_hbv-1.8.3.tar` & `ewatercycle_hbv-1.8.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/.readthedocs.yaml
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/CHANGELOG.md
--rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/plugin_guide.md
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/.idea/.gitignore
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/.idea/ewatercycle-hbv-numpy.iml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/.idea/misc.xml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/docs/Makefile
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/docs/conf.py
--rw-r--r--   0        0        0    55896 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/docs/example_model_run_HBV.ipynb
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/docs/make.bat
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/docs/model.rst
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/docs/requirements.txt
--rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/docs/_images/model_layout.png
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/docs/_static/README.rst
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/src/ewatercycle_HBV/__init__.py
--rw-r--r--   0        0        0    15335 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/src/ewatercycle_HBV/forcing.py
--rw-r--r--   0        0        0     9175 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/src/ewatercycle_HBV/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/tests/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/tests/test_forcing.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/tests/test_model.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/LICENSE.txt
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/README.md
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/pyproject.toml
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/.readthedocs.yaml
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/CHANGELOG.md
+-rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/plugin_guide.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/.idea/.gitignore
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/.idea/ewatercycle-hbv-numpy.iml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/.idea/misc.xml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/docs/Makefile
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/docs/conf.py
+-rw-r--r--   0        0        0    55896 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/docs/example_model_run_HBV.ipynb
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/docs/make.bat
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/docs/model.rst
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/docs/requirements.txt
+-rw-r--r--   0        0        0    96659 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/docs/_images/model_layout.png
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/docs/_static/README.rst
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/src/ewatercycle_HBV/__init__.py
+-rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/src/ewatercycle_HBV/forcing.py
+-rw-r--r--   0        0        0     9175 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/src/ewatercycle_HBV/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/tests/__init__.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/tests/test_forcing.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/tests/test_model.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/LICENSE.txt
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/README.md
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/pyproject.toml
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.4/PKG-INFO
```

### Comparing `ewatercycle_hbv-1.8.3/.readthedocs.yaml` & `ewatercycle_hbv-1.8.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.3/CHANGELOG.md` & `ewatercycle_hbv-1.8.4/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -43,8 +43,10 @@
 ### 1.8.0
 - Refactor potential evaporation from `pev` to `evspsblpot` & `tasmean` to `tas` to match convention
 #### 1.8.1
 - Rename `LumpedCamelsForcing` to `CamelsForcing`
 #### 1.8.2
 - No longer removes config on `finalize`, should be up to user
 #### 1.8.3
-- Local model: `HBVLocal` also availible in wrapper
+- Local model: `HBVLocal` also availible in wrapper
+#### 1.8.4
+- On generation of forcing adds a unique id (string) to be able to generate a lot of forcing at once
```

### Comparing `ewatercycle_hbv-1.8.3/plugin_guide.md` & `ewatercycle_hbv-1.8.4/plugin_guide.md`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.3/.github/workflows/python-publish.yml` & `ewatercycle_hbv-1.8.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.3/.github/workflows/test.yml` & `ewatercycle_hbv-1.8.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.3/docs/Makefile` & `ewatercycle_hbv-1.8.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.3/docs/conf.py` & `ewatercycle_hbv-1.8.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.3/docs/example_model_run_HBV.ipynb` & `ewatercycle_hbv-1.8.4/docs/example_model_run_HBV.ipynb`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.3/docs/index.rst` & `ewatercycle_hbv-1.8.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.3/docs/make.bat` & `ewatercycle_hbv-1.8.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.3/docs/model.rst` & `ewatercycle_hbv-1.8.4/docs/model.rst`

 * *Files 15% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 
 Model
 ===========================================
 
 HBV (Hydrologiska Byråns Vattenbalansavdelning) is a conceptual
 hydrological model. For more information on it’s history, see this
 `paper <https://hess.copernicus.org/articles/26/1371/2022/>`__.
+The actual model implemented here sit looks most like the original model from `1976 <https://urn.kb.se/resolve?urn=urn:nbn:se:smhi:diva-573>`__.
 
-This current implementation is *without* a snow reservoir as shown in the diagram below.
+
+This current implementation is with a snow reservoir as shown in the diagram below.
 
 .. image:: _images/model_layout.png
    :width: 600
    :alt: `Link <https://github.com/Daafip/HBV-bmi/blob/main/model_layout.png?raw=true>`__
 
 This implementation of the model uses a Markov Chain structure to allow it to be compatible with `Data Assimilation <https://github.com/Daafip/eWaterCycle-DA>`__.
 Testing it compared to a normal implementation showed this doesn't affect how the model performs.
```

### Comparing `ewatercycle_hbv-1.8.3/docs/_static/README.rst` & `ewatercycle_hbv-1.8.4/docs/_static/README.rst`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.3/src/ewatercycle_HBV/forcing.py` & `ewatercycle_hbv-1.8.4/src/ewatercycle_HBV/forcing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Forcing related functionality for HBV, see `eWaterCyle documentation <https://ewatercycle.readthedocs.io/en/latest/autoapi/ewatercycle/base/forcing/index.html>`_ for more detail."""
 # Based on https://github.com/eWaterCycle/ewatercycle-marrmot/blob/main/src/ewatercycle_marrmot/forcing.py
 
 from datetime import datetime
 from pathlib import Path
 from typing import Optional
+import random
+import string
 
 import pandas as pd
 import xarray as xr
 import numpy as np
 
 from ewatercycle.base.forcing import DefaultForcing
+from ewatercycle.util import get_time
 
 
 RENAME_CAMELS = {'total_precipitation_sum':'pr',
                  'potential_evaporation_sum':'evspsblpot',
                  'streamflow':'Q',
                  'temperature_2m_min':'tasmin',
                  'temperature_2m_max':'tasmax',
@@ -256,21 +259,22 @@
 
             ds_tas, ds_name_tas = self.crop_ds(ds_tas, "external")
             self.tas = ds_name_tas
 
             return ds_pr, ds_evspsblpot, ds_tas
 
     def crop_ds(self, ds: xr.Dataset, name: str):
-        start = np.datetime64(self.start_time)
-        end = np.datetime64(self.end_time)
+        start = pd.Timestamp(get_time(self.start_time)).tz_convert(None)
+        end = pd.Timestamp(get_time(self.end_time)).tz_convert(None)
         ds = ds.isel(time=(ds['time'].values >= start) & (ds['time'].values <= end))
 
         time = str(datetime.now())[:-10].replace(":", "_")
-        # TODO maybe change this time aspect? can get quite large - or simply remove in finalize
-        ds_name = f"HBV_forcing_{name}_{time}.nc"
+        letters = string.ascii_lowercase + string.ascii_uppercase
+        unique_identifier = ''.join((random.choice(letters)) for _ in range(5))
+        ds_name = f"HBV_forcing_{name}_{time}_{unique_identifier}.nc"
         out_dir = self.directory / ds_name
         if not out_dir.exists():
             ds.to_netcdf(out_dir)
 
         return ds, ds_name
 
     def file_not_found_error(self):
```

### Comparing `ewatercycle_hbv-1.8.3/src/ewatercycle_HBV/model.py` & `ewatercycle_hbv-1.8.4/src/ewatercycle_HBV/model.py`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.3/.gitignore` & `ewatercycle_hbv-1.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.3/LICENSE.txt` & `ewatercycle_hbv-1.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.3/README.md` & `ewatercycle_hbv-1.8.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 [![github license badge](https://img.shields.io/github/license/Daafip/ewatercycle-hbv)](https://github.com/Daafip/ewatercycle-hbv)
 [![fair-software badge](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B%20%20%E2%97%8B-yellow)](https://fair-software.eu)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Daafip_ewatercycle-hbv&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=Daafip_ewatercycle-hbv)
 
 
 This package is based on the [Leaky bucket](https://github.com/eWaterCycle/ewatercycle-leakybucket/tree/main) & is a wrapper for the [HBV-bmi](https://github.com/Daafip/HBV-bmi) model. 
 
-HBV (Hydrologiska Byråns Vattenbalansavdelning) is a conceptual hydrological model. For more information on it's history, see this [paper](https://hess.copernicus.org/articles/26/1371/2022/).
-
-This current implementation is _without_ a snow reservoir. 
+HBV (Hydrologiska Byråns Vattenbalansavdelning) is a conceptual hydrological model. For more information on its history, see this [paper](https://hess.copernicus.org/articles/26/1371/2022/).
+The actual model implemented here sit looks most like the original model from [1976](https://urn.kb.se/resolve?urn=urn:nbn:se:smhi:diva-5738).
+See documentation for schematic of model layout. 
 
 ## Installation
 Install this package alongside your eWaterCycle installation
 
 ```console
 pip install ewatercycle-hbv
 ```
```

### Comparing `ewatercycle_hbv-1.8.3/pyproject.toml` & `ewatercycle_hbv-1.8.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 path = "src/ewatercycle_HBV/__init__.py"
 
 [project]
 name = "ewatercycle-HBV"
 description = "Implementation of HBV for eWaterCycle"
 readme = "README.md"
 license = "Apache-2.0"
-version = "1.8.3"
+version = "1.8.4"
 authors = [
   { name = "David Haasnoot", email = "davidhaasnoot@gmail.com" },
 ]
 keywords = ["ewatercycle", "hydrology"]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
```

### Comparing `ewatercycle_hbv-1.8.3/PKG-INFO` & `ewatercycle_hbv-1.8.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ewatercycle-HBV
-Version: 1.8.3
+Version: 1.8.4
 Summary: Implementation of HBV for eWaterCycle
 Project-URL: homepage, https://github.com/Daafip/ewatercycle-hbv
 Author-email: David Haasnoot <davidhaasnoot@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Keywords: ewatercycle,hydrology
 Classifier: Intended Audience :: Developers
@@ -24,17 +24,17 @@
 [![github license badge](https://img.shields.io/github/license/Daafip/ewatercycle-hbv)](https://github.com/Daafip/ewatercycle-hbv)
 [![fair-software badge](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B%20%20%E2%97%8B-yellow)](https://fair-software.eu)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Daafip_ewatercycle-hbv&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=Daafip_ewatercycle-hbv)
 
 
 This package is based on the [Leaky bucket](https://github.com/eWaterCycle/ewatercycle-leakybucket/tree/main) & is a wrapper for the [HBV-bmi](https://github.com/Daafip/HBV-bmi) model. 
 
-HBV (Hydrologiska Byråns Vattenbalansavdelning) is a conceptual hydrological model. For more information on it's history, see this [paper](https://hess.copernicus.org/articles/26/1371/2022/).
-
-This current implementation is _without_ a snow reservoir. 
+HBV (Hydrologiska Byråns Vattenbalansavdelning) is a conceptual hydrological model. For more information on its history, see this [paper](https://hess.copernicus.org/articles/26/1371/2022/).
+The actual model implemented here sit looks most like the original model from [1976](https://urn.kb.se/resolve?urn=urn:nbn:se:smhi:diva-5738).
+See documentation for schematic of model layout. 
 
 ## Installation
 Install this package alongside your eWaterCycle installation
 
 ```console
 pip install ewatercycle-hbv
 ```
```

