# Comparing `tmp/t_ocr-1.4.8.tar.gz` & `tmp/t_ocr-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t_ocr-1.4.8.tar", last modified: Mon Mar 18 17:34:23 2024, max compression
+gzip compressed data, was "t_ocr-1.4.9.tar", last modified: Mon Mar 18 18:50:05 2024, max compression
```

## Comparing `t_ocr-1.4.8.tar` & `t_ocr-1.4.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-18 17:34:23.000335 t_ocr-1.4.8/
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-03-18 17:33:35.000000 t_ocr-1.4.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      839 2024-03-18 17:34:23.000335 t_ocr-1.4.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-03-18 17:33:35.000000 t_ocr-1.4.8/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-03-18 17:33:35.000000 t_ocr-1.4.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-03-18 17:33:35.000000 t_ocr-1.4.8/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      553 2024-03-18 17:34:23.000335 t_ocr-1.4.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      964 2024-03-18 17:33:35.000000 t_ocr-1.4.8/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-18 17:34:22.996335 t_ocr-1.4.8/t_ocr/
--rw-rw-rw-   0 root         (0) root         (0)      271 2024-03-18 17:33:35.000000 t_ocr-1.4.8/t_ocr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2024-03-18 17:33:35.000000 t_ocr-1.4.8/t_ocr/_config.py
--rw-rw-rw-   0 root         (0) root         (0)     3909 2024-03-18 17:33:35.000000 t_ocr-1.4.8/t_ocr/aws.py
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-03-18 17:33:35.000000 t_ocr-1.4.8/t_ocr/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    15431 2024-03-18 17:33:35.000000 t_ocr-1.4.8/t_ocr/free_ocr.py
--rw-rw-rw-   0 root         (0) root         (0)    18336 2024-03-18 17:33:35.000000 t_ocr-1.4.8/t_ocr/ocr.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-18 17:34:23.000335 t_ocr-1.4.8/t_ocr/ocr_tools/
--rw-rw-rw-   0 root         (0) root         (0)     1723 2024-03-18 17:33:35.000000 t_ocr-1.4.8/t_ocr/ocr_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14937 2024-03-18 17:33:35.000000 t_ocr-1.4.8/t_ocr/ocr_tools/address.py
--rw-rw-rw-   0 root         (0) root         (0)     9006 2024-03-18 17:33:35.000000 t_ocr-1.4.8/t_ocr/ocr_tools/fields_search.py
--rw-rw-rw-   0 root         (0) root         (0)     7831 2024-03-18 17:33:35.000000 t_ocr-1.4.8/t_ocr/ocr_tools/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3089 2024-03-18 17:33:35.000000 t_ocr-1.4.8/t_ocr/ocr_tools/ocr_tools.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-18 17:34:23.000335 t_ocr-1.4.8/t_ocr/ocr_tools/patterns/
--rw-rw-rw-   0 root         (0) root         (0)      448 2024-03-18 17:33:35.000000 t_ocr-1.4.8/t_ocr/ocr_tools/patterns/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2628 2024-03-18 17:33:35.000000 t_ocr-1.4.8/t_ocr/ocr_tools/patterns/patterns.py
--rw-rw-rw-   0 root         (0) root         (0)     6264 2024-03-18 17:33:35.000000 t_ocr-1.4.8/t_ocr/ocr_tools/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     7661 2024-03-18 17:33:35.000000 t_ocr-1.4.8/t_ocr/pages.py
--rw-rw-rw-   0 root         (0) root         (0)    16836 2024-03-18 17:33:35.000000 t_ocr-1.4.8/t_ocr/textract.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-18 17:34:23.000335 t_ocr-1.4.8/t_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)      839 2024-03-18 17:34:22.000000 t_ocr-1.4.8/t_ocr.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      644 2024-03-18 17:34:22.000000 t_ocr-1.4.8/t_ocr.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-18 17:34:22.000000 t_ocr-1.4.8/t_ocr.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-18 17:34:22.000000 t_ocr-1.4.8/t_ocr.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-03-18 17:34:22.000000 t_ocr-1.4.8/t_ocr.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        6 2024-03-18 17:34:22.000000 t_ocr-1.4.8/t_ocr.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-18 17:34:23.000335 t_ocr-1.4.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-03-18 17:33:35.000000 t_ocr-1.4.8/tests/test_t_ocr.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-18 18:50:05.658368 t_ocr-1.4.9/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-03-18 18:49:19.000000 t_ocr-1.4.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      839 2024-03-18 18:50:05.658368 t_ocr-1.4.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-03-18 18:49:19.000000 t_ocr-1.4.9/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-03-18 18:49:19.000000 t_ocr-1.4.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-03-18 18:49:19.000000 t_ocr-1.4.9/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      553 2024-03-18 18:50:05.658368 t_ocr-1.4.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      964 2024-03-18 18:49:19.000000 t_ocr-1.4.9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-18 18:50:05.654368 t_ocr-1.4.9/t_ocr/
+-rw-rw-rw-   0 root         (0) root         (0)      271 2024-03-18 18:49:19.000000 t_ocr-1.4.9/t_ocr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2024-03-18 18:49:19.000000 t_ocr-1.4.9/t_ocr/_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2024-03-18 18:49:19.000000 t_ocr-1.4.9/t_ocr/aws.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-03-18 18:49:19.000000 t_ocr-1.4.9/t_ocr/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15431 2024-03-18 18:49:19.000000 t_ocr-1.4.9/t_ocr/free_ocr.py
+-rw-rw-rw-   0 root         (0) root         (0)    18337 2024-03-18 18:49:19.000000 t_ocr-1.4.9/t_ocr/ocr.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-18 18:50:05.658368 t_ocr-1.4.9/t_ocr/ocr_tools/
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2024-03-18 18:49:19.000000 t_ocr-1.4.9/t_ocr/ocr_tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14937 2024-03-18 18:49:19.000000 t_ocr-1.4.9/t_ocr/ocr_tools/address.py
+-rw-rw-rw-   0 root         (0) root         (0)     9006 2024-03-18 18:49:19.000000 t_ocr-1.4.9/t_ocr/ocr_tools/fields_search.py
+-rw-rw-rw-   0 root         (0) root         (0)     7831 2024-03-18 18:49:19.000000 t_ocr-1.4.9/t_ocr/ocr_tools/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3089 2024-03-18 18:49:19.000000 t_ocr-1.4.9/t_ocr/ocr_tools/ocr_tools.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-18 18:50:05.658368 t_ocr-1.4.9/t_ocr/ocr_tools/patterns/
+-rw-rw-rw-   0 root         (0) root         (0)      448 2024-03-18 18:49:19.000000 t_ocr-1.4.9/t_ocr/ocr_tools/patterns/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2024-03-18 18:49:19.000000 t_ocr-1.4.9/t_ocr/ocr_tools/patterns/patterns.py
+-rw-rw-rw-   0 root         (0) root         (0)     6264 2024-03-18 18:49:19.000000 t_ocr-1.4.9/t_ocr/ocr_tools/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7661 2024-03-18 18:49:19.000000 t_ocr-1.4.9/t_ocr/pages.py
+-rw-rw-rw-   0 root         (0) root         (0)    16836 2024-03-18 18:49:19.000000 t_ocr-1.4.9/t_ocr/textract.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-18 18:50:05.658368 t_ocr-1.4.9/t_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      839 2024-03-18 18:50:05.000000 t_ocr-1.4.9/t_ocr.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      644 2024-03-18 18:50:05.000000 t_ocr-1.4.9/t_ocr.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-18 18:50:05.000000 t_ocr-1.4.9/t_ocr.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-18 18:50:05.000000 t_ocr-1.4.9/t_ocr.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-03-18 18:50:05.000000 t_ocr-1.4.9/t_ocr.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-03-18 18:50:05.000000 t_ocr-1.4.9/t_ocr.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-18 18:50:05.658368 t_ocr-1.4.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-03-18 18:49:19.000000 t_ocr-1.4.9/tests/test_t_ocr.py
```

### Comparing `t_ocr-1.4.8/PKG-INFO` & `t_ocr-1.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_ocr
-Version: 1.4.8
+Version: 1.4.9
 Summary: Thoughtful OCR Package
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtfulautomation.com
 Keywords: thoughtful-ocr,t-ocr,t_ocr
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_ocr-1.4.8/setup.cfg` & `t_ocr-1.4.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.4.8
+current_version = 1.4.9
 commit = True
 tag = False
 
 [bumpversion:file:setup.py]
 search = {current_version}
 replace = {new_version}
```

### Comparing `t_ocr-1.4.8/setup.py` & `t_ocr-1.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,10 +25,10 @@
     include_package_data=True,
     install_requires=install_requirements,
     keywords="thoughtful-ocr, t-ocr, t_ocr",
     name="t_ocr",
     packages=find_packages(include=["t_ocr", "t_ocr.*"]),
     test_suite="tests",
     url="https://www.thoughtful.ai/",
-    version="1.4.8",
+    version="1.4.9",
     zip_safe=False,
 )
```

### Comparing `t_ocr-1.4.8/t_ocr/aws.py` & `t_ocr-1.4.9/t_ocr/aws.py`

 * *Files identical despite different names*

### Comparing `t_ocr-1.4.8/t_ocr/free_ocr.py` & `t_ocr-1.4.9/t_ocr/free_ocr.py`

 * *Files identical despite different names*

### Comparing `t_ocr-1.4.8/t_ocr/ocr.py` & `t_ocr-1.4.9/t_ocr/ocr.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         self.__session = boto3.Session(
             aws_access_key_id=response["Credentials"]["AccessKeyId"],
             aws_secret_access_key=response["Credentials"]["SecretAccessKey"],
             aws_session_token=response["Credentials"]["SessionToken"],
             region_name=region,
         )
 
-    def login_via_aws(self, aws_credentials: dict, okta_credentials: dict):
+    def login_via_okta(self, aws_credentials: dict, okta_credentials: dict):
         """
         Login to AWS Textract with Okta.
 
         Args:
             aws_credentials (dict): AWS credentials.
             okta_credentials (dict): Okta credentials.
         """
```

### Comparing `t_ocr-1.4.8/t_ocr/ocr_tools/__init__.py` & `t_ocr-1.4.9/t_ocr/ocr_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `t_ocr-1.4.8/t_ocr/ocr_tools/address.py` & `t_ocr-1.4.9/t_ocr/ocr_tools/address.py`

 * *Files identical despite different names*

### Comparing `t_ocr-1.4.8/t_ocr/ocr_tools/fields_search.py` & `t_ocr-1.4.9/t_ocr/ocr_tools/fields_search.py`

 * *Files identical despite different names*

### Comparing `t_ocr-1.4.8/t_ocr/ocr_tools/models.py` & `t_ocr-1.4.9/t_ocr/ocr_tools/models.py`

 * *Files identical despite different names*

### Comparing `t_ocr-1.4.8/t_ocr/ocr_tools/ocr_tools.py` & `t_ocr-1.4.9/t_ocr/ocr_tools/ocr_tools.py`

 * *Files identical despite different names*

### Comparing `t_ocr-1.4.8/t_ocr/ocr_tools/patterns/patterns.py` & `t_ocr-1.4.9/t_ocr/ocr_tools/patterns/patterns.py`

 * *Files identical despite different names*

### Comparing `t_ocr-1.4.8/t_ocr/ocr_tools/validators.py` & `t_ocr-1.4.9/t_ocr/ocr_tools/validators.py`

 * *Files identical despite different names*

### Comparing `t_ocr-1.4.8/t_ocr/pages.py` & `t_ocr-1.4.9/t_ocr/pages.py`

 * *Files identical despite different names*

### Comparing `t_ocr-1.4.8/t_ocr/textract.py` & `t_ocr-1.4.9/t_ocr/textract.py`

 * *Files identical despite different names*

### Comparing `t_ocr-1.4.8/t_ocr.egg-info/PKG-INFO` & `t_ocr-1.4.9/t_ocr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_ocr
-Version: 1.4.8
+Version: 1.4.9
 Summary: Thoughtful OCR Package
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtfulautomation.com
 Keywords: thoughtful-ocr,t-ocr,t_ocr
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_ocr-1.4.8/t_ocr.egg-info/SOURCES.txt` & `t_ocr-1.4.9/t_ocr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

