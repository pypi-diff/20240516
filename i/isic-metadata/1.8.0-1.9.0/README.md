# Comparing `tmp/isic_metadata-1.8.0.tar.gz` & `tmp/isic_metadata-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isic_metadata-1.8.0.tar", last modified: Wed May 15 20:34:43 2024, max compression
+gzip compressed data, was "isic_metadata-1.9.0.tar", last modified: Wed May 15 20:48:09 2024, max compression
```

## Comparing `isic_metadata-1.8.0.tar` & `isic_metadata-1.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:34:43.857272 isic_metadata-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:34:43.849272 isic_metadata-1.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:34:43.853272 isic_metadata-1.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-15 20:34:43.857272 isic_metadata-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:34:43.853272 isic_metadata-1.8.0/isic_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/isic_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/isic_metadata/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    13559 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/isic_metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/isic_metadata/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/isic_metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:34:43.857272 isic_metadata-1.8.0/isic_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-15 20:34:43.000000 isic_metadata-1.8.0/isic_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-15 20:34:43.000000 isic_metadata-1.8.0/isic_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:34:43.000000 isic_metadata-1.8.0/isic_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 20:34:43.000000 isic_metadata-1.8.0/isic_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 20:34:43.000000 isic_metadata-1.8.0/isic_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:34:43.857272 isic_metadata-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:34:43.853272 isic_metadata-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/tests/test_dependent_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:48:09.957281 isic_metadata-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:48:09.949281 isic_metadata-1.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:48:09.953281 isic_metadata-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-15 20:48:09.957281 isic_metadata-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:48:09.953281 isic_metadata-1.9.0/isic_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/isic_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/isic_metadata/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13589 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/isic_metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/isic_metadata/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/isic_metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:48:09.957281 isic_metadata-1.9.0/isic_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-15 20:48:09.000000 isic_metadata-1.9.0/isic_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-15 20:48:09.000000 isic_metadata-1.9.0/isic_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:48:09.000000 isic_metadata-1.9.0/isic_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 20:48:09.000000 isic_metadata-1.9.0/isic_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 20:48:09.000000 isic_metadata-1.9.0/isic_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:48:09.957281 isic_metadata-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:48:09.957281 isic_metadata-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/tests/test_dependent_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-15 20:47:57.000000 isic_metadata-1.9.0/tox.ini
```

### Comparing `isic_metadata-1.8.0/.github/workflows/ci.yml` & `isic_metadata-1.9.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.8.0/.github/workflows/release.yml` & `isic_metadata-1.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.8.0/.gitignore` & `isic_metadata-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.8.0/LICENSE` & `isic_metadata-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.8.0/PKG-INFO` & `isic_metadata-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-metadata
-Version: 1.8.0
+Version: 1.9.0
 Home-page: https://github.com/ImageMarkup/isic-metadata
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-metadata/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-metadata
 Keywords: requests
```

### Comparing `isic_metadata-1.8.0/isic_metadata/__init__.py` & `isic_metadata-1.9.0/isic_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.8.0/isic_metadata/fields.py` & `isic_metadata-1.9.0/isic_metadata/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,17 @@
 
 class ImageTypeEnum(str, Enum):
     dermoscopic = "dermoscopic"
     clinical_overview = "clinical: overview"
     clinical_close_up = "clinical: close-up"
     tbp_tile_close_up = "TBP tile: close-up"
     tbp_tile_overview = "TBP tile: overview"
+    # Note that RCM types need to be added to validate_rcm_fields
     rcm_macroscopic = "RCM: macroscopic"
+    rcm_tile = "RCM: tile"
 
 
 class DermoscopicTypeEnum(str, Enum):
     contact_polarized = "contact polarized"
     contact_non_polarized = "contact non-polarized"
     non_contact_polarized = "non-contact polarized"
```

### Comparing `isic_metadata-1.8.0/isic_metadata/metadata.py` & `isic_metadata-1.9.0/isic_metadata/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,15 +360,15 @@
 
         if not self.rcm_case_id:
             return self
 
         if not self.image_type:
             raise error_missing_field("rcm_case_id", "image_type")
 
-        if self.image_type != ImageTypeEnum.rcm_macroscopic:
+        if self.image_type not in [ImageTypeEnum.rcm_macroscopic, ImageTypeEnum.rcm_tile]:
             raise error_incompatible_fields(
                 "rcm_case_id", "image_type", field2_value=ImageTypeEnum.rcm_macroscopic
             )
 
         return self
 
     @model_validator(mode="after")
```

### Comparing `isic_metadata-1.8.0/isic_metadata.egg-info/PKG-INFO` & `isic_metadata-1.9.0/isic_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-metadata
-Version: 1.8.0
+Version: 1.9.0
 Home-page: https://github.com/ImageMarkup/isic-metadata
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-metadata/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-metadata
 Keywords: requests
```

### Comparing `isic_metadata-1.8.0/isic_metadata.egg-info/SOURCES.txt` & `isic_metadata-1.9.0/isic_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.8.0/pyproject.toml` & `isic_metadata-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.8.0/setup.py` & `isic_metadata-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.8.0/tests/test_batch.py` & `isic_metadata-1.9.0/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.8.0/tests/test_dependent_fields.py` & `isic_metadata-1.9.0/tests/test_dependent_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
 def test_rcm_case_id_requires_rcm_image_type():
     with pytest.raises(ValidationError) as excinfo:
         MetadataRow.model_validate({"rcm_case_id": "12345"})
     assert len(excinfo.value.errors()) == 1
     assert "rcm_case_id requires setting image_type" in excinfo.value.errors()[0]["msg"]
 
-    MetadataRow.model_validate({"rcm_case_id": "12345", "image_type": "RCM: macroscopic"})
+    MetadataRow.model_validate({"rcm_case_id": "12345", "image_type": "RCM: tile"})
 
 
 def test_rcm_model_checks_disabling():
     with pytest.raises(ValidationError) as excinfo:
         MetadataRow(rcm_case_id="12345")
     assert len(excinfo.value.errors()) == 1
     assert "rcm_case_id requires setting image_type" in excinfo.value.errors()[0]["msg"]
```

### Comparing `isic_metadata-1.8.0/tests/test_fields.py` & `isic_metadata-1.9.0/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.8.0/tox.ini` & `isic_metadata-1.9.0/tox.ini`

 * *Files identical despite different names*

