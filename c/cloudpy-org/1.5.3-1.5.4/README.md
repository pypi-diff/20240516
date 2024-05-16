# Comparing `tmp/cloudpy_org-1.5.3.tar.gz` & `tmp/cloudpy_org-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.5.3.tar", last modified: Wed May  8 09:16:44 2024, max compression
+gzip compressed data, was "dist\cloudpy_org-1.5.4.tar", last modified: Thu May 16 20:45:49 2024, max compression
```

## Comparing `cloudpy_org-1.5.3.tar` & `cloudpy_org-1.5.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 09:16:44.227509 cloudpy_org-1.5.3/
--rw-rw-rw-   0        0        0      935 2024-05-08 09:16:44.226511 cloudpy_org-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.5.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 09:16:44.085909 cloudpy_org-1.5.3/cloudpy_org/
--rw-rw-rw-   0        0        0     3171 2024-05-08 09:15:35.000000 cloudpy_org-1.5.3/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    32752 2024-05-08 09:08:18.000000 cloudpy_org-1.5.3/cloudpy_org/aws.py
--rw-rw-rw-   0        0        0    41925 2024-05-08 09:08:25.000000 cloudpy_org-1.5.3/cloudpy_org/client_usage.py
--rw-rw-rw-   0        0        0    13614 2024-05-08 09:08:33.000000 cloudpy_org-1.5.3/cloudpy_org/docs.py
--rw-rw-rw-   0        0        0     3924 2024-05-08 09:08:40.000000 cloudpy_org-1.5.3/cloudpy_org/imgedit.py
--rw-rw-rw-   0        0        0    50259 2024-05-08 09:08:48.000000 cloudpy_org-1.5.3/cloudpy_org/tools.py
--rw-rw-rw-   0        0        0     4998 2024-05-08 09:08:55.000000 cloudpy_org-1.5.3/cloudpy_org/web.py
-drwxrwxrwx   0        0        0        0 2024-05-08 09:16:44.197219 cloudpy_org-1.5.3/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      935 2024-05-08 09:16:42.000000 cloudpy_org-1.5.3/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-05-08 09:16:43.000000 cloudpy_org-1.5.3/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 09:16:42.000000 cloudpy_org-1.5.3/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-08 09:16:42.000000 cloudpy_org-1.5.3/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-08 09:16:42.000000 cloudpy_org-1.5.3/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 09:16:44.227929 cloudpy_org-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1324 2024-05-08 09:11:43.000000 cloudpy_org-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:45:49.624537 cloudpy_org-1.5.4/
+-rw-rw-rw-   0        0        0      935 2024-05-16 20:45:49.623994 cloudpy_org-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.5.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 20:45:49.439348 cloudpy_org-1.5.4/cloudpy_org/
+-rw-rw-rw-   0        0        0     3240 2024-05-16 20:39:34.000000 cloudpy_org-1.5.4/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    32752 2024-05-16 20:39:43.000000 cloudpy_org-1.5.4/cloudpy_org/aws.py
+-rw-rw-rw-   0        0        0    80029 2024-05-16 20:39:48.000000 cloudpy_org-1.5.4/cloudpy_org/client_usage.py
+-rw-rw-rw-   0        0        0    13614 2024-05-16 20:39:53.000000 cloudpy_org-1.5.4/cloudpy_org/docs.py
+-rw-rw-rw-   0        0        0     3924 2024-05-01 08:43:26.000000 cloudpy_org-1.5.4/cloudpy_org/imgedit.py
+-rw-rw-rw-   0        0        0    51895 2024-05-16 20:40:00.000000 cloudpy_org-1.5.4/cloudpy_org/tools.py
+-rw-rw-rw-   0        0        0     4998 2024-05-16 20:40:17.000000 cloudpy_org-1.5.4/cloudpy_org/web.py
+-rw-rw-rw-   0        0        0    10189 2024-05-16 20:40:06.000000 cloudpy_org-1.5.4/cloudpy_org/web_client_usage.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:45:49.594975 cloudpy_org-1.5.4/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      935 2024-05-16 20:45:47.000000 cloudpy_org-1.5.4/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2024-05-16 20:45:48.000000 cloudpy_org-1.5.4/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 20:45:47.000000 cloudpy_org-1.5.4/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2024-05-16 20:45:47.000000 cloudpy_org-1.5.4/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-16 20:45:47.000000 cloudpy_org-1.5.4/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 20:45:49.625038 cloudpy_org-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1352 2024-05-16 20:45:19.000000 cloudpy_org-1.5.4/setup.py
```

### Comparing `cloudpy_org-1.5.3/PKG-INFO` & `cloudpy_org-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.5.3
+Version: 1.5.4
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.5.3/cloudpy_org/__init__.py` & `cloudpy_org-1.5.4/cloudpy_org/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,16 @@
  'eu-west-1': {'long_name': 'Europe (Ireland)', 'code': 'euw1'},
  'eu-west-2': {'long_name': 'Europe (London)', 'code': 'euw2'},
  'eu-west-3': {'long_name': 'Europe (Paris)', 'code': 'euw3'},
  'eu-north-1': {'long_name': 'Europe (Stockholm)', 'code': 'eun1'},
  'sa-east-1': {'long_name': 'South America (São Paulo)', 'code': 'sae1'}}
 subscription_url = 'https://www.cloudpy.org'
 msh = 'secure'
-cloudpy_org_version='1.5.3'
+cloudpy_org_version='1.5.4'
 gsep = {'user_email_sep': '-0-', '@': '-1-', '.': '-2-'}
 from cloudpy_org.tools import processing_tools,unique_id
 from cloudpy_org.docs import auto_document,convert_jupiter_notebook_to_html,documentation_from_folder
 from cloudpy_org.aws import aws_framework_manager,aws_framework_manager_client,gen_aws_auth_token,gen_new_service_token,configure_aws,get_my_aws_service_token,authenticate_with_token,delete_biscuit,co_token_auth
 from cloudpy_org.web import flask_website
 from cloudpy_org.imgedit import colors
 from cloudpy_org.client_usage import cloudpy_org_aws_framework_client
-
+#from cloudpy_org_base.web_client_usage import cloudpy_org_web_client
```

### Comparing `cloudpy_org-1.5.3/cloudpy_org/aws.py` & `cloudpy_org-1.5.4/cloudpy_org/aws.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.5.3/cloudpy_org/docs.py` & `cloudpy_org-1.5.4/cloudpy_org/docs.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.5.3/cloudpy_org/imgedit.py` & `cloudpy_org-1.5.4/cloudpy_org/imgedit.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.5.3/cloudpy_org/tools.py` & `cloudpy_org-1.5.4/cloudpy_org/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,16 +33,20 @@
 import inspect
 from os import walk
 import s3fs
 import random
 import time
 import re
 unique_id = lambda: int(round(time.time() * 100000))
+
+
+ 
 class processing_tools:
     def __init__(self,data:dict={},bucket_name:str='',region_name:str="us-east-2",local:bool=False,third_part:str=None):
+        self.regex = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,15}\b'
         self.current_path = os.getcwd() + "/"
         self.aws_auth_token_expired = True
         self.aws_authenticated = False
         self.aws_auth_error_message = ""
         self.__third_part = third_part
         self.__local = local
         self.aux = {}
@@ -73,14 +77,51 @@
             self.fs = s3fs.S3FileSystem()
         except:
             self.fs = None
         try:
             self.load_metadata()
         except:
             ...
+    #__________________________________________________________________________    
+    def validate_password_format(self,input_str:str,include_symbols:bool=False):
+        SpecialSym =['$', '@', '#', '%']
+        rslt = 'ok'
+        if len(input_str) < 6:
+            rslt = 'Length should be at least 6'
+        if len(input_str) > 20:
+            rslt = 'Length should be not be greater than 20'
+        with_digit = False
+        with_upper = False
+        with_lower = False
+        with_sym = False
+        for char in input_str:
+            if ord(char) >= 48 and ord(char) <= 57:
+                with_digit = True
+            elif ord(char) >= 65 and ord(char) <= 90:
+                with_upper = True
+            elif ord(char) >= 97 and ord(char) <= 122:
+                with_lower = True
+            elif char in SpecialSym:
+                with_sym = True
+        if not with_digit:
+            rslt = 'Password should have at least one numeral'
+        if not with_upper:
+            rslt = 'Password should have at least one uppercase letter'
+        if not with_lower:
+            rslt = 'Password should have at least one lowercase letter'
+        if include_symbols:
+            if not with_sym:
+                rslt = 'Password should have at least one of the symbols $@#'
+        return rslt
+    #__________________________________________________________________________
+    def validate_str_as_email(self,input_str:str):
+        if(re.fullmatch(self.regex, input_str)):
+            return True
+        else:
+            return False
     #__________________________________________________________________________
     def camel_to_snake(self,input_str):
         rslt = input_str.replace(' ','_')\
         .replace('__','_')\
         .replace('__','_')\
         .replace('__','')
         rslt = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', rslt)
```

### Comparing `cloudpy_org-1.5.3/cloudpy_org/web.py` & `cloudpy_org-1.5.4/cloudpy_org/web.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.5.3/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.5.4/cloudpy_org.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.5.3
+Version: 1.5.4
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.5.3/setup.py` & `cloudpy_org-1.5.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.5.3",
+    version="1.5.4",
     description="Cloud data pipeline organization and automation library. Includes AWS framework manager API.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
@@ -27,9 +27,9 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
     packages=["cloudpy_org"],
     include_package_data=True,
-    install_requires=["pandas","pandasql","boto3","awswrangler","tqdm","numpy","cryptography","s3fs"]
+    install_requires=["pandas","pandasql","boto3","awswrangler","tqdm","botocore","numpy","cryptography","s3fs","pillow","flask"]
 )
```

