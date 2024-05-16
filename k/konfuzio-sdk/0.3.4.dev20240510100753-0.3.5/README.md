# Comparing `tmp/konfuzio_sdk-0.3.4.dev20240510100753.tar.gz` & `tmp/konfuzio_sdk-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konfuzio_sdk-0.3.4.dev20240510100753.tar", last modified: Sat May 11 03:27:43 2024, max compression
+gzip compressed data, was "konfuzio_sdk-0.3.5.tar", last modified: Wed May 15 19:43:30 2024, max compression
```

## Comparing `konfuzio_sdk-0.3.4.dev20240510100753.tar` & `konfuzio_sdk-0.3.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:27:43.970110 konfuzio_sdk-0.3.4.dev20240510100753/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-11 03:27:43.970110 konfuzio_sdk-0.3.4.dev20240510100753/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:27:43.962109 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   207592 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    27450 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/settings_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:27:43.962109 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/tokenizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/tokenizer/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:27:43.962109 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    75617 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/document_categorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    51309 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/file_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/image.py
--rw-r--r--   0 runner    (1001) docker     (127)   102313 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/information_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:27:43.966109 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-11 03:27:43.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-11 03:27:43.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 03:27:43.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-11 03:27:43.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-11 03:27:43.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 03:27:43.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 03:27:43.970110 konfuzio_sdk-0.3.4.dev20240510100753/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:27:43.966109 konfuzio_sdk-0.3.4.dev20240510100753/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    23531 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   169232 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:43:30.339739 konfuzio_sdk-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-15 19:43:30.339739 konfuzio_sdk-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:43:30.327739 konfuzio_sdk-0.3.5/konfuzio_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   209636 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27953 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/settings_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:43:30.331739 konfuzio_sdk-0.3.5/konfuzio_sdk/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/tokenizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/tokenizer/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:43:30.331739 konfuzio_sdk-0.3.5/konfuzio_sdk/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/trainer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75617 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/trainer/document_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51309 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/trainer/file_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/trainer/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102313 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/trainer/information_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/trainer/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/trainer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/konfuzio_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:43:30.335739 konfuzio_sdk-0.3.5/konfuzio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-15 19:43:30.000000 konfuzio_sdk-0.3.5/konfuzio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-15 19:43:30.000000 konfuzio_sdk-0.3.5/konfuzio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:43:30.000000 konfuzio_sdk-0.3.5/konfuzio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 19:43:30.000000 konfuzio_sdk-0.3.5/konfuzio_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-15 19:43:30.000000 konfuzio_sdk-0.3.5/konfuzio_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 19:43:30.000000 konfuzio_sdk-0.3.5/konfuzio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:43:30.339739 konfuzio_sdk-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:43:30.335739 konfuzio_sdk-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    23531 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   169232 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/tests/test_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10316 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/tests/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-05-15 19:43:22.000000 konfuzio_sdk-0.3.5/tests/test_utils.py
```

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/LICENSE.md` & `konfuzio_sdk-0.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/PKG-INFO` & `konfuzio_sdk-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.3.4.dev20240510100753
+Version: 0.3.5
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2023.7.22
```

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/README.md` & `konfuzio_sdk-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/api.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/api.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/cli.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/data.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4010,17 +4010,51 @@
                                 and annotation['label']['name'] == 'NO_LABEL'
                             )
                         )
                     ]
 
                 if raw_annotations:
                     for raw_annotation in raw_annotations:
-                        raw_annotation['annotation_set_id'] = raw_annotation.pop('section')
-                        raw_annotation['label_set_id'] = raw_annotation.pop('section_label_id')
-                        _ = Annotation(document=self, id_=raw_annotation['id'], **raw_annotation)
+                        # for backward compatibility - to enable loading projects with old and new structure of folders
+                        # and files / json5 metadata
+                        if 'annotation_set' in raw_annotation:
+                            raw_annotation['annotation_set_id'] = raw_annotation.pop('annotation_set')
+                        else:
+                            raw_annotation['annotation_set_id'] = raw_annotation.pop('section')
+                        if 'label_set' in raw_annotation:
+                            raw_annotation['label_set_id'] = raw_annotation.pop('label_set')['id']
+                        else:
+                            raw_annotation['label_set_id'] = raw_annotation.pop('section_label_id')
+                        raw_annotation.pop('document', None)
+                        if isinstance(raw_annotation['label'], int):
+                            label = self.project.get_label_by_id(id_=raw_annotation['label'])
+                        else:
+                            label = self.project.get_label_by_id(id_=raw_annotation['label']['id'])
+                        # same with 'label'
+                        raw_annotation.pop('label', None)
+                        # same with 'span'/'bboxes'
+                        if 'span' in raw_annotation:
+                            raw_spans = raw_annotation['span']
+                            raw_annotation.pop('span', None)
+                        else:
+                            raw_spans = raw_annotation['bboxes']
+                        spans = [
+                            Span(start_offset=span['start_offset'], end_offset=span['end_offset']) for span in raw_spans
+                        ]
+                        # same with 'annotation_set'
+                        if (
+                            raw_annotation['annotation_set_id']
+                            and not self.project.get_label_set_by_id(
+                                raw_annotation['label_set_id']
+                            ).has_multiple_annotation_sets
+                        ):
+                            raw_annotation.pop('annotation_set_id', None)
+                        _ = Annotation(
+                            document=self, id_=raw_annotation['id'], label=label, spans=spans, **raw_annotation
+                        )
 
         return self._annotations.values()
 
     def propose_splitting(self, splitting_ai) -> List:
         """Propose splitting for a multi-file Document.
 
         :param splitting_ai: An initialized SplittingAI class
```

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/evaluate.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/extras.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/extras.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/normalize.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/normalize.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,22 @@
     # check for ,22,95 (obscured edge case)
     elif (
         ln > 2 and offset_string[0] == '‚' and offset_string[-3] == ','
     ):  # first comma is a very different comma ('‚' != ',')
         offset_string = offset_string[1:].replace(',', '.')  # => 22.95
         if all(x.isdecimal() for x in offset_string.split('.')):
             _float = _normalize_to_float_safe(offset_string)
+    # check for 1.213467, 200.3212415 and all floats with multiple digits after the decimal separator and no thousand
+    # separators
+    elif '.' in offset_string and offset_string.count('.') == 1:
+        if len(offset_string.split('.')[1]) > 5:
+            _float = _normalize_to_float_safe(offset_string)
+    elif ',' in offset_string and offset_string.count(',') == 1:
+        if len(offset_string.split(',')[1]) > 5:
+            _float = _normalize_to_float_safe(offset_string.replace(',', '.'))
     elif all(char in ROMAN_NUMS.keys() for char in offset_string):
         normalization = roman_to_float(offset_string)
     else:
         logger.debug(
             'Could not convert >>' + offset_string + '<< to positive/absolute float (no conversion case found)'
         )
```

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/regex.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/samples.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/settings_importer.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/settings_importer.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/tokenizer/base.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/tokenizer/base.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/tokenizer/paragraph_and_sentence.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/tokenizer/paragraph_and_sentence.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/tokenizer/regex.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/tokenizer/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/base.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/trainer/base.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/document_categorization.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/trainer/document_categorization.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/file_splitting.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/trainer/file_splitting.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/image.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/trainer/image.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/information_extraction.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/trainer/information_extraction.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/tokenization.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/trainer/tokenization.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/utils.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/urls.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/utils.py` & `konfuzio_sdk-0.3.5/konfuzio_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/PKG-INFO` & `konfuzio_sdk-0.3.5/konfuzio_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.3.4.dev20240510100753
+Version: 0.3.5
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2023.7.22
```

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/SOURCES.txt` & `konfuzio_sdk-0.3.5/konfuzio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/requires.txt` & `konfuzio_sdk-0.3.5/konfuzio_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/setup.py` & `konfuzio_sdk-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_api.py` & `konfuzio_sdk-0.3.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_cli.py` & `konfuzio_sdk-0.3.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_data.py` & `konfuzio_sdk-0.3.5/tests/test_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -664,15 +664,15 @@
         pipeline.test_documents = pipeline.category.test_documents()
         pipeline.df_train, pipeline.label_feature_list = pipeline.feature_function(
             documents=pipeline.documents, require_revised_annotations=False
         )
         pipeline.fit()
         evaluation = pipeline.evaluate_full(strict=False, use_training_docs=True)
         outliers = label.get_probable_outliers_by_confidence(evaluation, 0.9)
-        assert len(outliers) == 2
+        assert len(outliers) >= 2
         outlier_spans = [span.offset_string for annotation in outliers for span in annotation.spans]
         assert '24.05.2018' in outlier_spans
 
     def test_find_outlier_annotations_by_normalization(self):
         """Test finding the Annotations that do not correspond the Label's data type."""
         project = Project(id_=TEST_PROJECT_ID)
         label = project.get_label_by_name('Austellungsdatum')
```

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_evaluate.py` & `konfuzio_sdk-0.3.5/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_extras.py` & `konfuzio_sdk-0.3.5/tests/test_extras.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_normalize.py` & `konfuzio_sdk-0.3.5/tests/test_normalize.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,14 +244,18 @@
     ('..1..2.3..3333.', None, None),
     ('114433,8,60', None, None),
     ('165a', None, None),
     ('0,0-3,0', None, None),
     ('3,6-4.8', None, None),
     ('0,1–1,112', None, None),
     ('21231.41–124.4124,52', None, None),
+    ('1.214141', 1.214141, None),
+    ('22,1231', 22.1231, None),
+    ('0,543255', 0.543255, None),
+    ('3.141528743253920', 3.141528743253920, None),
     # ('12.', 12.0, 0), undefined test cases:
     # ('1.', 1.0, 0),
     # ('.', None, 0),
     # ('.1', 0.1, 0),
     # ('.123', 0.123, 0),
 ]
```

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_regex.py` & `konfuzio_sdk-0.3.5/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_samples.py` & `konfuzio_sdk-0.3.5/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_urls.py` & `konfuzio_sdk-0.3.5/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_utils.py` & `konfuzio_sdk-0.3.5/tests/test_utils.py`

 * *Files identical despite different names*

