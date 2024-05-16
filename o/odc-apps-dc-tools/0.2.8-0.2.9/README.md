# Comparing `tmp/odc-apps-dc-tools-0.2.8.tar.gz` & `tmp/odc-apps-dc-tools-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odc-apps-dc-tools-0.2.8.tar", last modified: Fri Nov 18 04:17:00 2022, max compression
+gzip compressed data, was "odc-apps-dc-tools-0.2.9.tar", last modified: Mon Feb 20 06:03:05 2023, max compression
```

## Comparing `odc-apps-dc-tools-0.2.8.tar` & `odc-apps-dc-tools-0.2.9.tar`

### file list

```diff
@@ -1,34 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 04:17:00.199834 odc-apps-dc-tools-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6714 2022-11-18 04:17:00.199834 odc-apps-dc-tools-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6266 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 04:17:00.195834 odc-apps-dc-tools-0.2.8/odc/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 04:17:00.195834 odc-apps-dc-tools-0.2.8/odc/apps/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 04:17:00.199834 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4110 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/_docs.py
--rw-r--r--   0 runner    (1001) docker     (122)    13942 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/_stac.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     5201 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/add_update_products.py
--rw-r--r--   0 runner    (1001) docker     (122)     4041 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/azure_to_dc.py
--rw-r--r--   0 runner    (1001) docker     (122)     7664 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/cop_dem_to_dc.py
--rw-r--r--   0 runner    (1001) docker     (122)     7095 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/esa_worldcover_to_dc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9343 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/export_md.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2806 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/fs_to_dc.py
--rw-r--r--   0 runner    (1001) docker     (122)     5765 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/index_from_tar.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5282 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/s3_to_dc.py
--rw-r--r--   0 runner    (1001) docker     (122)    13917 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/sqs_to_dc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9136 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/stac_api_to_dc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/thredds_to_dc.py
--rw-r--r--   0 runner    (1001) docker     (122)    10757 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 04:17:00.199834 odc-apps-dc-tools-0.2.8/odc_apps_dc_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6714 2022-11-18 04:17:00.000000 odc-apps-dc-tools-0.2.8/odc_apps_dc_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      860 2022-11-18 04:17:00.000000 odc-apps-dc-tools-0.2.8/odc_apps_dc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-18 04:17:00.000000 odc-apps-dc-tools-0.2.8/odc_apps_dc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      595 2022-11-18 04:17:00.000000 odc-apps-dc-tools-0.2.8/odc_apps_dc_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-18 04:16:59.000000 odc-apps-dc-tools-0.2.8/odc_apps_dc_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      219 2022-11-18 04:17:00.000000 odc-apps-dc-tools-0.2.8/odc_apps_dc_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2022-11-18 04:17:00.000000 odc-apps-dc-tools-0.2.8/odc_apps_dc_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      170 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2022-11-18 04:17:00.199834 odc-apps-dc-tools-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-18 04:16:38.000000 odc-apps-dc-tools-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 06:03:05.176609 odc-apps-dc-tools-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-02-20 06:03:05.176609 odc-apps-dc-tools-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 06:03:05.168609 odc-apps-dc-tools-0.2.9/odc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 06:03:05.168609 odc-apps-dc-tools-0.2.9/odc/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 06:03:05.172609 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/_stac.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/add_update_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/azure_to_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/cop_dem_to_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/esa_worldcover_to_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/export_md.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2686 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/fs_to_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/index_from_tar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5282 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/s3_to_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14191 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/sqs_to_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/stac_api_to_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/thredds_to_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 06:03:05.172609 odc-apps-dc-tools-0.2.9/odc_apps_dc_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-02-20 06:03:05.000000 odc-apps-dc-tools-0.2.9/odc_apps_dc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-02-20 06:03:05.000000 odc-apps-dc-tools-0.2.9/odc_apps_dc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 06:03:05.000000 odc-apps-dc-tools-0.2.9/odc_apps_dc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-02-20 06:03:05.000000 odc-apps-dc-tools-0.2.9/odc_apps_dc_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 06:03:04.000000 odc-apps-dc-tools-0.2.9/odc_apps_dc_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-20 06:03:05.000000 odc-apps-dc-tools-0.2.9/odc_apps_dc_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-20 06:03:05.000000 odc-apps-dc-tools-0.2.9/odc_apps_dc_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-02-20 06:03:05.176609 odc-apps-dc-tools-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 06:03:05.176609 odc-apps-dc-tools-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/tests/test_add_update_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/tests/test_cop_dem_to_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/tests/test_esa_worldcover_to_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/tests/test_fs_to_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/tests/test_s3_to_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/tests/test_sns_publishing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/tests/test_sqs_to_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/tests/test_stac_api_to_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-02-20 06:02:50.000000 odc-apps-dc-tools-0.2.9/tests/test_stac_transform.py
```

### Comparing `odc-apps-dc-tools-0.2.8/LICENSE` & `odc-apps-dc-tools-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `odc-apps-dc-tools-0.2.8/PKG-INFO` & `odc-apps-dc-tools-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odc-apps-dc-tools
-Version: 0.2.8
+Version: 0.2.9
 Summary: CLI utils for working with a datacube index
 Home-page: https://github.com/opendatacube/odc-tools/
 Author: Open Data Cube
 Author-email: 
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
```

### Comparing `odc-apps-dc-tools-0.2.8/README.md` & `odc-apps-dc-tools-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/_docs.py` & `odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/_docs.py`

 * *Files identical despite different names*

### Comparing `odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/_stac.py` & `odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/_stac.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """
 Tools for STAC to EO3 translation
 """
 import math
+import numpy
+from eodatasets3.serialise import from_doc
+from eodatasets3.stac import to_stac_item
 from pathlib import Path
+from toolz import get_in
 from typing import Any, Dict, Optional, Tuple
+from urlpath import URL
 from uuid import UUID
 
-import numpy
+from datacube.model import Dataset
 from datacube.utils.geometry import Geometry
-from toolz import get_in
-from urlpath import URL
-
 from ._docs import odc_uuid
 
-from eodatasets3.serialise import from_doc
-from eodatasets3.stac import to_stac_item
-from datacube.model import Dataset
-
 Document = Dict[str, Any]
 
 # This is an old hack, should be refactored out
 DEA_LANDSAT_PRODUCTS = ["ga_ls8c_ard_3", "ga_ls7e_ard_3", "ga_ls8t_ard_3"]
 
 # This is hack for not changing the current behavior of DEAfrica sentinel-2
 # It is not ideal but to remain the impact minimum
```

### Comparing `odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/add_update_products.py` & `odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/add_update_products.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Add or update a list of ODC products. Intended to be used to
 systematically maintain a CSV of products and synchronise it with
 a database"""
 
+from collections import Counter, namedtuple
+
+import click
+import fsspec
 import logging
 import sys
-from collections import Counter, namedtuple
+import yaml
 from csv import DictReader
 from typing import Any, Dict, List, Optional, Generator, Tuple
 
-import click
 import datacube
-import fsspec
-import yaml
 from datacube import Datacube
 from odc.apps.dc_tools.utils import (
     update_if_exists_flag,
     statsd_gauge_reporting,
     statsd_setting,
 )
```

### Comparing `odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/azure_to_dc.py` & `odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/azure_to_dc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Crawl Thredds for prefixes and fetch YAML's for indexing
 and dump them into a Datacube instance
 """
+import click
 import json
 import logging
+from odc.azure import download_blob, find_blobs
 from typing import List, Optional
 
-import click
 from datacube import Datacube
 from datacube.index.hl import Doc2Dataset
 from odc.apps.dc_tools._stac import stac_transform
 from odc.apps.dc_tools.utils import (
     allow_unsafe,
     archive_less_mature,
     index_update_dataset,
     statsd_gauge_reporting,
     statsd_setting,
     transform_stac,
     update_flag,
     update_if_exists_flag,
     publish_action,
 )
-from odc.azure import download_blob, find_blobs
 
 
 def stream_blob_urls(account_url, container_name, credential, blobs: List[str]):
     for blob in blobs:
         doc, uri, _ = download_blob(account_url, container_name, credential, blob)
         yield (json.loads(doc), uri)
```

### Comparing `odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/cop_dem_to_dc.py` & `odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/cop_dem_to_dc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 #!/usr/bin/env python3
 """
 Index the Copernicus DEM automatically.
 """
+import click
 import concurrent.futures
 import logging
+import pystac
+import rasterio
 import sys
 from math import ceil, floor
+from rio_stac import create_stac_item
 from typing import Tuple
 
-import click
-import pystac
-import rasterio
 from datacube import Datacube
 from datacube.index.hl import Doc2Dataset
 from datacube.utils import read_documents
 from odc.apps.dc_tools.utils import (
     SkippedException,
     archive_less_mature,
     bbox,
     index_update_dataset,
     limit,
     update_if_exists_flag,
     publish_action,
     statsd_gauge_reporting,
     statsd_setting,
 )
-from rio_stac import create_stac_item
-
 from ._stac import stac_transform
 
 PRODUCTS = {
     "cop_30": (
         "https://raw.githubusercontent.com/opendatacube/"
         "datacube-dataset-config/master/products/dem_cop_30.odc-product.yaml"
     ),
```

### Comparing `odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/esa_worldcover_to_dc.py` & `odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/esa_worldcover_to_dc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 #!/usr/bin/env python3
 """
 Index the ESA Worldcover data automatically.
 """
+import click
 import concurrent.futures
 import logging
+import pystac
+import rasterio
 import sys
 from math import ceil, floor
+from rio_stac import create_stac_item
 from typing import Tuple
 
-import click
-import pystac
-import rasterio
 from datacube import Datacube
 from datacube.index.hl import Doc2Dataset
 from datacube.utils import read_documents
 from odc.apps.dc_tools.utils import (
     bbox,
     index_update_dataset,
     limit,
     update_if_exists_flag,
     archive_less_mature,
     statsd_gauge_reporting,
     statsd_setting,
     publish_action,
 )
-from rio_stac import create_stac_item
-
 from ._stac import stac_transform
 
 PRODUCT = (
     "https://raw.githubusercontent.com/opendatacube/"
-    "datacube-dataset-config/master/products/esa_worldcover.odc-product.yaml"
+    "datacube-dataset-config/master/products/esa_worldcover_{year}.odc-product.yaml"
 )
 
 # URIs need north/south, which is N00 and east/west, which is E000
 URI_TEMPLATE = (
     "https://esa-worldcover.s3.eu-central-1.amazonaws.com/"
-    "v100/2020/map/ESA_WorldCover_10m_2020_v100_{ns}{ew}_Map.tif"
+    "{algo}/{year}/map/ESA_WorldCover_10m_{year}_{algo}_{ns}{ew}_Map.tif"
 )
 
+map_version = dict(algo="v100", year="2020")
+
 
 def _unpack_bbox(bounding_box: str) -> Tuple[int, int, int, int]:
     """Set up a left, bottom, right, top bbox with 3 degree offset"""
     left = floor(bounding_box[0])
     bottom = floor(bounding_box[1])
     right = ceil(bounding_box[2])
     top = ceil(bounding_box[3])
@@ -61,15 +62,15 @@
     bottom = bottom - bottom_offset
     right = right - right_offset
     top = top - top_offset
     return left, bottom, right, top
 
 
 def add_odc_product(dc: Datacube):
-    for _, doc in read_documents(PRODUCT):
+    for _, doc in read_documents(PRODUCT.format(year=map_version["year"])):
         dc.index.products.add_document(doc)
     print("Product definition added")
 
 
 def get_tile_uris(bounding_box: str) -> Tuple[str, str]:
     # Validate the bounding_box
     if bounding_box is None:
@@ -97,34 +98,39 @@
             else:
                 x_str = f"E{x:03d}"
             if y < 0:
                 y_str = f"S{abs(y):02d}"
             else:
                 y_str = f"N{y:02d}"
             yield (
-                URI_TEMPLATE.format(ns=y_str, ew=x_str),
+                URI_TEMPLATE.format(
+                    ns=y_str,
+                    ew=x_str,
+                    algo=map_version["algo"],
+                    year=map_version["year"],
+                ),
                 f"{x_str}_{y_str}",
             )
 
 
 def process_uri_tile(
     uri_tile: Tuple[str, str, str],
     dc: Datacube,
     doc2ds: Doc2Dataset,
     update_if_exists: bool = True,
     archive_less_mature: bool = False,
     publish_action: str = None,
 ) -> Tuple[pystac.Item, str]:
-    product_name = "esa_worldcover"
+    product_name = "esa_worldcover_" + map_version["year"]
     uri, tile = uri_tile
     properties = {
         "odc:product": product_name,
         "odc:region_code": tile,
-        "start_datetime": "2020-01-01",
-        "end_datetime": "2020-12-31",
+        "start_datetime": map_version["year"] + "-01-01",
+        "end_datetime": map_version["year"] + "-12-31",
     }
 
     with rasterio.Env(aws_unsigned=True, GDAL_DISABLE_READDIR_ON_OPEN="EMPTY_DIR"):
         item = create_stac_item(
             uri,
             collection=product_name,
             with_proj=True,
@@ -144,14 +150,20 @@
         publish_action=publish_action,
         stac_doc=item.to_dict(),
     )
 
     return True
 
 
+def select_map_version(version: str):
+    if str(version) == "2021":
+        map_version["year"] = "2021"
+        map_version["algo"] = "v200"
+
+
 def esa_wc_to_dc(
     dc: Datacube,
     bounding_box,
     limit: int,
     update: bool,
     n_workers: int = 100,
     archive_less_mature: bool = False,
@@ -215,28 +227,38 @@
 @click.option(
     "--workers",
     default=20,
     type=int,
     help="Number of threads to use to process, default 20",
 )
 @statsd_setting
+@click.option(
+    "--version",
+    default="2020",
+    type=str,
+    help="Select version of world cover map, default 2020",
+)
 def cli(
     limit,
     update_if_exists,
     bbox,
     add_product,
     archive_less_mature,
     workers,
     statsd_setting,
     publish_action,
+    version,
 ):
     """
     Index the ESA WorldCover product automatically.
     """
 
+    # Select map version
+    select_map_version(version)
+
     dc = Datacube()
 
     if add_product:
         add_odc_product(dc)
 
     print(f"Indexing ESA WorldCover with bounding box of {bbox}")
```

### Comparing `odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/export_md.py` & `odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/export_md.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,19 @@
     --config metadata_transform_config.yaml --output-dir /g/data/u46/users/aj9439/metadata
     --limit 10
 The config file contains the grid mappings to band names:
     grids:
       default: ['3', '4', '5']
       swir: ['1', '2']
 """
+import click
 import logging
+import yaml
 from pathlib import Path
 
-import click
-import yaml
 from datacube import Datacube
 from datacube.storage import BandInfo
 from datacube.testutils.io import native_geobox
 
 _LOG = logging.getLogger(__name__)
 
 
@@ -36,25 +36,24 @@
 
 @cli.command()
 @click.option("--product", required=True, help="Which product?")
 @click.option(
     "--config", required=True, help="The configuration file for transformation"
 )
 @click.option(
-    "--output-dir", required=True, help="New metadata yaml file is written to this dir"
+    "--output-dir", required=True, help="New metadata YAML file is written to this dir"
 )
 @click.option("--limit", help="maximum number of datasets to process")
 @click.pass_obj
 def transform(index, product, config, output_dir, limit):
-
     # Get the product
     dataset_type = index.products.get_by_name(product)
 
-    with open(config, "r") as config_file:
-        cfg = yaml.load(config_file) or dict()
+    with open(config, "r", encoding="utf8") as config_file:
+        cfg = yaml.load(config_file) or {}
 
     # Is this a ingested product?
     if dataset_type.grid_spec is not None:
         transform_ingested_datasets(index, product, cfg, Path(output_dir), limit)
     else:
         transform_indexed_datasets(index, product, cfg, Path(output_dir), limit)
 
@@ -67,28 +66,27 @@
 
     dataset_ids = index.datasets.search_returning(
         limit=limit, field_names=("id",), product=product
     )
 
     grids_done = False
     for dataset_id in dataset_ids:
-
         dataset = index.datasets.get(dataset_id.id, include_sources=True)
 
         if not dataset.uris:
-            _LOG.warn("Empty uris or No uris (skippins): %s", dataset_id)
+            _LOG.warning("Empty uris or No uris (skippins): %s", dataset_id)
             continue
 
         if not grids_done:
             # setup grids
             grids = get_grids(dataset, config.get("grids"))
 
             # got to try to compute grids until shape is not default [1, 1]
             grids_done = all(
-                [[1, 1] != grid["shape"] for _, grid in grids["grids"].items()]
+                [1, 1] != grid["shape"] for _, grid in grids["grids"].items()
             )
 
         dataset_sections = (grids,) + _variable_sections_of_metadata(dataset, config)
         _make_and_write_dataset(get_output_file(dataset, output_dir), *dataset_sections)
 
 
 def transform_indexed_datasets(index, product, config, output_dir, limit):
@@ -96,19 +94,18 @@
     Transform metadata of an indexed product. All sections of metadata are computed
     per dataset.
     """
 
     for dataset_id in index.datasets.search_returning(
         limit=limit, field_names=("id",), product=product
     ):
-
         dataset = index.datasets.get(dataset_id.id, include_sources=True)
 
         if not dataset.uris:
-            _LOG.warn("Empty or No uris (skipping): %s", dataset_id)
+            _LOG.warning("Empty or No uris (skipping): %s", dataset_id)
             continue
 
         grids = get_grids(dataset, config.get("grids"))
 
         dataset_sections = (grids,) + _variable_sections_of_metadata(dataset, config)
         _make_and_write_dataset(get_output_file(dataset, output_dir), *dataset_sections)
 
@@ -126,15 +123,15 @@
 def _variable_sections_of_metadata(dataset, config):
     """
     Compute variable sections (i.e. those sections that vary per dataset)
     """
     new_dataset = {
         "id": str(dataset.id),
         "crs": "EPSG:" + str(dataset.crs.epsg),
-        "location": [uri for uri in dataset.uris],
+        "location": list(dataset.uris),
         "file_format": dataset.metadata_doc.get("format", ""),
     }
 
     return (
         new_dataset,
         get_geometry(dataset),
         get_measurements(dataset, config.get("grids")),
@@ -144,19 +141,19 @@
 
 
 def _make_and_write_dataset(out_file_name, *args):
     """
     Assemble the metadata sections and write out.
     """
 
-    dataset = dict()
+    dataset = {}
     for arg in args:
         dataset.update(arg)
 
-    with open(out_file_name, "w") as out_file:
+    with open(out_file_name, "w", encoding="utf8") as out_file:
         yaml.dump(dataset, out_file, default_flow_style=False)
 
 
 def get_geometry(dataset):
     """
     Extract and return geometry coordinates as a list in a dictionary:
     returns
@@ -168,15 +165,15 @@
     }
     or
     empty dictionary
     """
 
     valid_data = dataset._gs.get("valid_data")
 
-    return {"geometry": valid_data} if valid_data else dict()
+    return {"geometry": valid_data} if valid_data else {}
 
 
 def get_grids(dataset, band_grids=None):
     """
     'band_grids' specify bands for each grid as in:
     {
         default: [swir1, swir2]
@@ -197,23 +194,21 @@
 
     if not band_grids:
         # Assume all measurements belong to default grid
         shape, trans = get_shape_and_transform(dataset, dataset.measurements)
 
         return {"grids": {"default": {"shape": list(shape), "transform": list(trans)}}}
     else:
-        grids = dict()
+        grids = {}
         for grid_name in band_grids:
-
             shape, trans = get_shape_and_transform(dataset, band_grids[grid_name])
 
             grids[grid_name] = {"shape": list(shape), "transform": list(trans)}
 
         if not band_grids.get("default"):
-
             specified_bands = set()
             for grid in band_grids:
                 specified_bands.update(band_grids[grid])
             all_bands = set(list(dataset.measurements))
 
             default_bands = all_bands - specified_bands
 
@@ -229,21 +224,23 @@
     Get shape and transform for the given set of measurements. It try
     each measurement until it succeeds.
     """
 
     for m in measurements:
         try:
             geo = native_geobox(dataset, [m])
-        except Exception:
-            _LOG.warn("Failed to compute shape and transform %s", m)
+        except Exception:  # pylint: disable=broad-except
+            _LOG.warning("Failed to compute shape and transform %s", m)
             continue
         return geo.shape, geo.transform
 
     # All the bands failed use default shape [1,1]
-    _LOG.warn("All measurements failed to compute shape and transform %s", measurements)
+    _LOG.warning(
+        "All measurements failed to compute shape and transform %s", measurements
+    )
     return [1, 1], dataset.transform
 
 
 def get_measurements(dataset, band_grids=None):
     """
     Extract and return measurement paths in a dictionary:
     Returns
@@ -259,22 +256,21 @@
         ...
       }
     }
     """
     grids_map = (
         {m: grid for grid in band_grids for m in band_grids[grid] if grid != "default"}
         if band_grids
-        else dict()
+        else {}
     )
 
-    measurements = dict()
+    measurements = {}
     for m in dataset.measurements:
-
         if m not in dataset.type.measurements:
-            _LOG.warn("Measurement not in product definition (skipping): %s", m)
+            _LOG.warning("Measurement not in product definition (skipping): %s", m)
             continue
 
         band_info = BandInfo(dataset, m)
         measurements[m] = {"path": dataset.measurements[m]["path"]}
 
         if band_info.band and band_info.band != 1:
             measurements[m]["band"] = band_info.band
@@ -296,34 +292,35 @@
       {
         'datetime': time,
         'odc:creation_datetime': creation_time,
         ...
       }
     }
     """
-    props = dict()
-    props["datetime"] = dataset.center_time
-    props["odc:processing_datetime"] = dataset.indexed_time
-
-    return {"properties": props}
+    return {
+        "properties": {
+            "datetime": dataset.center_time,
+            "odc:processing_datetime": dataset.indexed_time,
+        }
+    }
 
 
 def get_lineage(dataset):
     """
     Extract immediate parents.
     {
       'lineage':
       {
         'nbar': [id1, id2],
         'pq': [id3]
         ...
       }
     }
     """
-    lineage = dict()
+    lineage = {}
     for classifier in dataset.sources:
         lineage[classifier] = str(dataset.sources[classifier].id)
     return {"lineage": lineage}
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/fs_to_dc.py` & `odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/fs_to_dc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,26 @@
+import click
 import json
 import logging
+import yaml
 from pathlib import Path
-from typing import Generator, Optional
 
-import click
 import datacube
-import yaml
 from datacube.index.hl import Doc2Dataset
 from odc.apps.dc_tools._stac import stac_transform
 from odc.apps.dc_tools.utils import (
     allow_unsafe,
     archive_less_mature,
     index_update_dataset,
     update_if_exists_flag,
     publish_action,
     statsd_setting,
     statsd_gauge_reporting,
     transform_stac,
 )
-from odc.apps.dc_tools._stac import stac_transform
-import logging
-
-
-import yaml
 
 logging.basicConfig(
     level=logging.WARNING,
     format="%(asctime)s: %(levelname)s: %(message)s",
     datefmt="%m/%d/%Y %I:%M:%S",
 )
 
@@ -50,15 +44,14 @@
     allow_unsafe,
     stac,
     statsd_setting,
     glob,
     archive_less_mature,
     publish_action,
 ):
-
     dc = datacube.Datacube()
     doc2ds = Doc2Dataset(dc.index)
 
     if glob is None:
         glob = "**/*.json" if stac else "**/*.yaml"
 
     files_to_process = Path(input_directory).glob(glob)
```

### Comparing `odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/index_from_tar.py` & `odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/index_from_tar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """ Index datasets from tar arachive
 """
 
-import sys
-
 import click
-import datacube
-from datacube.utils.changes import allow_any
+import sys
 from odc.io.tar import tar_doc_stream, tar_mode
 from odc.io.timer import RateEstimator
 
+import datacube
+from datacube.utils.changes import allow_any
 from ._docs import from_yaml_doc_stream
 from ._stac import stac_transform
 
 
 def from_tar_file(tarfname, index, mk_uri, mode, doc_transform=None, **kwargs):
     """returns a sequence of tuples where each tuple is either
 
@@ -115,15 +114,14 @@
     ignore_lineage,
     update,
     gzip,
     xz,
     protocol,
     stac,
 ):
-
     # Ensure :// is present in prefix
     prefix = protocol.rstrip("://") + "://"
     if prefix.startswith("file"):
         prefix = prefix + "/"
 
     if ignore_lineage:
         auto_add_lineage = False
@@ -160,15 +158,15 @@
             if ds is not None:
                 try:
                     if update:
                         index.datasets.update(ds, allowed_changes)
                     else:
                         index.datasets.add(ds, with_lineage=auto_add_lineage)
 
-                except Exception as e:
+                except Exception as e:  # pylint: disable=broad-except
                     n_failed += 1
                     report_error(str(e))
             else:
                 n_failed += 1
                 report_error(err)
 
             fps()
```

### Comparing `odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/s3_to_dc.py` & `odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/s3_to_dc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 """Build S3 iterators using odc-tools
 and index datasets found into RDS
 """
+import click
 import logging
 import sys
+from odc.aio import S3Fetcher, s3_find_glob
 from typing import Tuple
 
-import click
 from datacube import Datacube
 from datacube.index.hl import Doc2Dataset
-from odc.aio import S3Fetcher, s3_find_glob
 from odc.apps.dc_tools._docs import parse_doc_stream
 from odc.apps.dc_tools._stac import stac_transform, stac_transform_absolute
 from odc.apps.dc_tools.utils import (
     IndexingException,
     SkippedException,
     allow_unsafe,
     archive_less_mature,
```

### Comparing `odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/sqs_to_dc.py` & `odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/sqs_to_dc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 #!/usr/bin/env python3
 """Index datasets found from an SQS queue into Postgres
 """
+import boto3
+import click
 import json
 import logging
+import pandas as pd
+import requests
 import sys
 import uuid
+from botocore import UNSIGNED
+from botocore.config import Config
+from odc.aws.queue import get_messages, publish_to_topic
 from pathlib import PurePath
+from toolz import dicttoolz
 from typing import Tuple
+from yaml import safe_load
 
-import boto3
-import click
-import pandas as pd
-import requests
-from botocore import UNSIGNED
-from botocore.config import Config
 from datacube import Datacube
 from datacube.index.hl import Doc2Dataset
 from datacube.utils import documents
 from odc.apps.dc_tools.utils import (
     IndexingException,
     SkippedException,
     allow_unsafe,
@@ -33,18 +36,14 @@
     transform_stac_absolute,
     archive_less_mature,
     update_flag,
     update_if_exists_flag,
     verify_lineage,
     publish_action,
 )
-from odc.aws.queue import get_messages, publish_to_topic
-from toolz import dicttoolz
-from yaml import safe_load
-
 from ._stac import stac_transform, stac_transform_absolute, ds_to_stac
 
 # Added log handler
 logging.basicConfig(level=logging.WARNING, handlers=[logging.StreamHandler()])
 
 
 def extract_metadata_from_message(message):
@@ -58,14 +57,21 @@
 
     if metadata:
         return metadata
     else:
         raise IndexingException("Failed to load metadata from the SQS message")
 
 
+def extract_action_from_message(message):
+    attributes = message.message_attributes
+    if attributes:
+        return dicttoolz.get_in(["action", "StringValue"], attributes)
+    return None
+
+
 def handle_json_message(metadata, transform, odc_metadata_link):
     odc_yaml_uri = None
     uri = None
 
     if odc_metadata_link:
         if odc_metadata_link.startswith("STAC-LINKS-REL:"):
             rel_val = odc_metadata_link.replace("STAC-LINKS-REL:", "")
@@ -100,15 +106,15 @@
     message, metadata: dict, record_path: tuple, no_sign_request: bool = False
 ) -> Tuple[dict, str]:
     """[summary]
 
     Args:
         message (Message resource)
         metadata (dict): [description]
-        record_path (tuple): [PATH for selectingthe s3 key path from the JSON message document]
+        record_path (tuple): [PATH for selecting the s3 key path from the JSON message document]
 
     Raises:
         IndexingException: [Catch s3 ]
 
     Returns:
         Tuple[dict, str]: [description]
     """
@@ -203,15 +209,14 @@
     allow_unsafe=False,
     odc_metadata_link=False,
     region_code_list_uri=None,
     archive_less_mature=None,
     publish_action=None,
     **kwargs,
 ) -> Tuple[int, int, int]:
-
     ds_success = 0
     ds_failed = 0
     ds_skipped = 0
 
     region_codes = None
     if region_code_list_uri:
         try:
@@ -231,15 +236,16 @@
     messages = get_messages(queue, limit)
 
     for message in messages:
         try:
             # Extract metadata from message
             metadata = extract_metadata_from_message(message)
             stac_doc = None
-            if archive:
+            action = extract_action_from_message(message)
+            if archive or action == "ARCHIVED":
                 # Archive metadata
                 do_archiving(metadata, dc, publish_action)
             else:
                 if not record_path:
                     if transform:
                         stac_doc = metadata
                     # Extract metadata and URI from a STAC or similar
@@ -327,15 +333,15 @@
     default=None,
     multiple=True,
     help="Filtering option for s3 path, i.e. 'L2/sentinel-2-nrt/S2MSIARD/*/*/ARD-METADATA.yaml'",
 )
 @click.option(
     "--region-code-list-uri",
     default=None,
-    help="A path to a list (one item per line, in txt or gzip format) of valide region_codes to include",
+    help="A path to a list (one item per line, in txt or gzip format) of valid region_codes to include",
 )
 @archive_less_mature
 @publish_action
 @click.argument("queue_name", type=str, nargs=1)
 @click.argument("product", type=str, nargs=1)
 def cli(
     skip_lineage,
```

### Comparing `odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/stac_api_to_dc.py` & `odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/stac_api_to_dc.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python3
 """Index datasets found from an SQS queue into Postgres
 """
+import click
 import concurrent
 import json
 import logging
 import os
+import pystac
 import sys
+from pystac.item import Item
+from pystac_client import Client
 from typing import Any, Dict, Generator, Optional, Tuple
 
-import click
-import pystac
 from datacube import Datacube
 from datacube.index.hl import Doc2Dataset
 from odc.apps.dc_tools._stac import stac_transform, stac_transform_absolute
 from odc.apps.dc_tools.utils import (
     SkippedException,
     allow_unsafe,
     archive_less_mature,
@@ -21,16 +23,14 @@
     index_update_dataset,
     limit,
     statsd_gauge_reporting,
     statsd_setting,
     update_if_exists_flag,
     publish_action,
 )
-from pystac.item import Item
-from pystac_client import Client
 
 logging.basicConfig(
     level=logging.WARNING,
     format="%(asctime)s: %(levelname)s: %(message)s",
     datefmt="%m/%d/%Y %I:%M:%S",
 )
```

### Comparing `odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/thredds_to_dc.py` & `odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/thredds_to_dc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """Crawl Thredds for prefixes and fetch YAML's for indexing
 and dump them into a Datacube instance
 """
+import click
 import logging
-import sys
+from odc.thredds import download_yamls, thredds_find_glob
 from typing import List, Tuple
 
-import click
 from datacube import Datacube
 from odc.apps.dc_tools.utils import statsd_gauge_reporting, statsd_setting
-from odc.thredds import download_yamls, thredds_find_glob
-
 from ._docs import from_yaml_doc_stream
 
 
 def dump_list_to_odc(
     yaml_content_list: List[Tuple[bytes, str, str]],
     dc: Datacube,
     products: List[str],
@@ -37,15 +35,15 @@
         else:
             logging.info(ds)
             # TODO: Potentially wrap this in transactions and batch to DB
             # TODO: Capture UUID's from YAML and perform a bulk has
             try:
                 dc.index.datasets.add(ds)
                 ds_added += 1
-            except Exception as e:
+            except Exception as e:  # pylint: disable=broad-except
                 logging.error(e)
                 ds_failed += 1
 
     return ds_added, ds_failed
 
 
 @click.command("thredds-to-dc")
```

### Comparing `odc-apps-dc-tools-0.2.8/odc/apps/dc_tools/utils.py` & `odc-apps-dc-tools-0.2.9/odc/apps/dc_tools/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,18 @@
+import click
 import logging
 import os
+import pkg_resources
+from datadog import statsd, initialize
+from odc.aws.queue import publish_to_topic
 from typing import Iterable, Optional, Union
 
-import click
-import pkg_resources
 from datacube import Datacube
 from datacube.index.hl import Doc2Dataset
 from datacube.utils import changes
-
-from datadog import statsd, initialize
-
-from odc.aws.queue import publish_to_topic
 from ._stac import ds_to_stac
 
 ESRI_LANDCOVER_BASE_URI = (
     "https://ai4edataeuwest.blob.core.windows.net/io-lulc/"
     "io-lulc-model-001-v01-composite-v03-supercell-v02-clip-v01/{id}_20200101-20210101.tif"
 )
```

### Comparing `odc-apps-dc-tools-0.2.8/odc_apps_dc_tools.egg-info/PKG-INFO` & `odc-apps-dc-tools-0.2.9/odc_apps_dc_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odc-apps-dc-tools
-Version: 0.2.8
+Version: 0.2.9
 Summary: CLI utils for working with a datacube index
 Home-page: https://github.com/opendatacube/odc-tools/
 Author: Open Data Cube
 Author-email: 
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
```

### Comparing `odc-apps-dc-tools-0.2.8/odc_apps_dc_tools.egg-info/entry_points.txt` & `odc-apps-dc-tools-0.2.9/odc_apps_dc_tools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `odc-apps-dc-tools-0.2.8/setup.cfg` & `odc-apps-dc-tools-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 	click
 	fsspec
 	pystac-client>=0.2.0
 	toolz
 	pyyaml
 	datacube>=1.8.9
 	odc_io
-	odc-cloud[ASYNC]
+	odc-cloud[ASYNC]>=0.2.3
 	pystac>=1.0.0
 	rio-stac
 	urlpath
 	datadog
 	eodatasets3
 
 [options.extras_require]
```

