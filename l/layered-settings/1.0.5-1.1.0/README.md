# Comparing `tmp/layered-settings-1.0.5.tar.gz` & `tmp/layered-settings-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\layered-settings-1.0.5.tar", last modified: Sun Apr 25 22:42:56 2021, max compression
+gzip compressed data, was "layered-settings-1.1.0.tar", last modified: Thu May 16 16:55:57 2024, max compression
```

## Comparing `layered-settings-1.0.5.tar` & `layered-settings-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxrwxrwx   0        0        0        0 2021-04-25 22:42:56.969489 layered-settings-1.0.5/
--rw-rw-rw-   0        0        0     3119 2021-04-25 22:42:56.969489 layered-settings-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2068 2021-04-25 22:30:49.000000 layered-settings-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2021-04-25 22:42:56.933488 layered-settings-1.0.5/layered_settings/
--rw-rw-rw-   0        0        0      115 2021-04-25 22:30:49.000000 layered-settings-1.0.5/layered_settings/__init__.py
--rw-rw-rw-   0        0        0     2956 2021-04-25 22:30:49.000000 layered-settings-1.0.5/layered_settings/layered_settings.py
-drwxrwxrwx   0        0        0        0 2021-04-25 22:42:56.966490 layered-settings-1.0.5/layered_settings/loaders/
--rw-rw-rw-   0        0        0      241 2021-04-25 22:30:49.000000 layered-settings-1.0.5/layered_settings/loaders/__init__.py
--rw-rw-rw-   0        0        0      389 2021-03-23 19:42:18.000000 layered-settings-1.0.5/layered_settings/loaders/base_loader.py
--rw-rw-rw-   0        0        0      334 2021-04-25 22:30:49.000000 layered-settings-1.0.5/layered_settings/loaders/callable_loader.py
--rw-rw-rw-   0        0        0     1056 2021-03-23 19:42:18.000000 layered-settings-1.0.5/layered_settings/loaders/config_parser_loader.py
--rw-rw-rw-   0        0        0      332 2021-04-25 22:30:49.000000 layered-settings-1.0.5/layered_settings/loaders/dict_loader.py
--rw-rw-rw-   0        0        0     1134 2021-04-25 22:39:54.000000 layered-settings-1.0.5/layered_settings/loaders/env_loader.py
--rw-rw-rw-   0        0        0     1969 2021-04-25 22:30:49.000000 layered-settings-1.0.5/layered_settings/loaders/ssm_loader.py
-drwxrwxrwx   0        0        0        0 2021-04-25 22:42:56.958488 layered-settings-1.0.5/layered_settings.egg-info/
--rw-rw-rw-   0        0        0     3119 2021-04-25 22:42:56.000000 layered-settings-1.0.5/layered_settings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2021-04-25 22:42:56.000000 layered-settings-1.0.5/layered_settings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-04-25 22:42:56.000000 layered-settings-1.0.5/layered_settings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-04-25 22:40:16.000000 layered-settings-1.0.5/layered_settings.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2021-04-25 22:42:56.000000 layered-settings-1.0.5/layered_settings.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2021-04-25 22:42:56.000000 layered-settings-1.0.5/layered_settings.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2021-04-25 22:42:56.971487 layered-settings-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      844 2021-04-25 22:40:30.000000 layered-settings-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2021-04-25 22:42:56.968488 layered-settings-1.0.5/tests/
--rw-rw-rw-   0        0        0        0 2021-03-23 19:42:18.000000 layered-settings-1.0.5/tests/__init__.py
--rw-rw-rw-   0        0        0     3269 2021-04-25 22:30:49.000000 layered-settings-1.0.5/tests/tests.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:55:57.434359 layered-settings-1.1.0/
+-rw-rw-rw-   0        0        0     1091 2021-03-23 19:42:18.000000 layered-settings-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3043 2024-05-16 16:55:57.434359 layered-settings-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2457 2024-05-16 16:52:21.000000 layered-settings-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 16:55:57.407834 layered-settings-1.1.0/layered_settings/
+-rw-rw-rw-   0        0        0      115 2021-04-25 22:30:49.000000 layered-settings-1.1.0/layered_settings/__init__.py
+-rw-rw-rw-   0        0        0     2956 2021-04-25 22:30:49.000000 layered-settings-1.1.0/layered_settings/layered_settings.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:55:57.430359 layered-settings-1.1.0/layered_settings/loaders/
+-rw-rw-rw-   0        0        0      301 2024-05-16 16:52:21.000000 layered-settings-1.1.0/layered_settings/loaders/__init__.py
+-rw-rw-rw-   0        0        0      389 2021-03-23 19:42:18.000000 layered-settings-1.1.0/layered_settings/loaders/base_loader.py
+-rw-rw-rw-   0        0        0      334 2021-04-25 22:30:49.000000 layered-settings-1.1.0/layered_settings/loaders/callable_loader.py
+-rw-rw-rw-   0        0        0     1056 2021-03-23 19:42:18.000000 layered-settings-1.1.0/layered_settings/loaders/config_parser_loader.py
+-rw-rw-rw-   0        0        0      332 2021-04-25 22:30:49.000000 layered-settings-1.1.0/layered_settings/loaders/dict_loader.py
+-rw-rw-rw-   0        0        0     1134 2021-04-25 22:39:54.000000 layered-settings-1.1.0/layered_settings/loaders/env_loader.py
+-rw-rw-rw-   0        0        0     2897 2024-05-16 16:52:21.000000 layered-settings-1.1.0/layered_settings/loaders/secrets_manager_loader.py
+-rw-rw-rw-   0        0        0     1969 2021-04-25 22:30:49.000000 layered-settings-1.1.0/layered_settings/loaders/ssm_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:55:57.420845 layered-settings-1.1.0/layered_settings.egg-info/
+-rw-rw-rw-   0        0        0     3043 2024-05-16 16:55:57.000000 layered-settings-1.1.0/layered_settings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2024-05-16 16:55:57.000000 layered-settings-1.1.0/layered_settings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 16:55:57.000000 layered-settings-1.1.0/layered_settings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-04-25 22:40:16.000000 layered-settings-1.1.0/layered_settings.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2024-05-16 16:55:57.000000 layered-settings-1.1.0/layered_settings.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-16 16:55:57.000000 layered-settings-1.1.0/layered_settings.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      370 2021-03-23 19:42:18.000000 layered-settings-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-05-16 16:55:57.435362 layered-settings-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      892 2024-05-16 16:52:21.000000 layered-settings-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:55:57.432359 layered-settings-1.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2021-03-23 19:42:18.000000 layered-settings-1.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     3269 2021-04-25 22:30:49.000000 layered-settings-1.1.0/tests/tests.py
```

### Comparing `layered-settings-1.0.5/PKG-INFO` & `layered-settings-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,79 @@
 Metadata-Version: 2.1
 Name: layered-settings
-Version: 1.0.5
-Summary: Flexible, simple, extensible settings loader from environment, AWS SSM, configparser .ini, and more.
+Version: 1.1.0
+Summary: Flexible, simple, extensible settings loader from environment, AWS SSM, AWS Secrets Manager, configparser .ini, and more.
 Home-page: https://github.com/mathandpencil/layered-settings
 Author: Scott Stafford
 Author-email: scott.stafford+layered@gmail.com
-License: UNKNOWN
-Description: # layered-settings
-        
-        `layered-settings` is a simple and configurable hierarchical settings library for Python, including Django, Flask, or any other
-        scripts that need settings from potentially a variety of sources. With it you can load
-        settings from the environment, Amazon's SSM, local configparser .ini files, and more.
-        
-        ## Installation
-        
-        The package is available on pip as `layered-settings`. Run:
-        
-        `pip install layered-settings`
-        
-        If you want to use the AWS SSM layer, include the [ssm] extra:
-        
-        `pip install layered-settings[ssm]`
-        
-        then import via:
-        
-        `from layered_settings import initialize_settings, loaders`
-        
-        ## Example Usage
-        
-        ```python
-        import os
-        from layered_settings import initialize_settings
-        from layered_settings import loaders
-        
-        get_setting = initialize_settings(
-            sources=[
-                # Lowest priority is setting-defaults.ini.  All configuration values should be defaulted in here.
-                # The `loaders.ConfigParserLoader` is optional - if you pass a string ending in .ini, it wraps it in
-                # a `loaders.ConfigParserLoader` for you.
-                loaders.ConfigParserLoader(os.path.join(SCRIPT_DIR, "setting-defaults.ini")),
-        
-                # Next priority is a "user" settings file.
-                os.path.expanduser("~/.app-settings.ini"),
-        
-                # You can include a dictionary in the sources too...
-                {
-                    "general": {"CLIENT_NAME": "client"},
-                    "email": {"EMAIL_HOST": "smtp.example.com", "EMAIL_PORT": 25},
-                },
-        
-                # If we are able/willing to reach out to AWS, do so.  A `None` in the initialize_settings sources
-                # will simply be ignored.
-                loaders.SSMLoader(f"/app/stage/", aws_region="us-east-1") if ALLOW_SSM_CONFIGURATION else None,
-        
-                # Top priority -- env var in the format APP__section__key.
-                loaders.EnvLoader("APP__{section}__{key}"),
-            ]
-        )
-        
-        DATABASE_HOST = get_setting("database", "DATABASE_HOST")
-        AWS_SECRET_KEY = get_setting("aws", "AWS_SECRET_KEY")
-        ...
-        ```
-        
-        ## Frameworks Supported
-        
-        This library is tested using Python 3.x.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: ssm
+Provides-Extra: aws
+License-File: LICENSE
+
+# layered-settings
+
+`layered-settings` is a simple and configurable hierarchical settings library for Python, including Django, Flask, or any other
+scripts that need settings from potentially a variety of sources. With it you can load
+settings from the environment, Amazon's SSM, Amazon's Secrets Manager, local configparser .ini files, and more.
+
+## Installation
+
+The package is available on pip as `layered-settings`. Run:
+
+`pip install layered-settings`
+
+If you want to use the AWS SSM layer or Secrets Manager layer, include the [aws] extra:
+
+`pip install layered-settings[aws]`
+
+then import via:
+
+`from layered_settings import initialize_settings, loaders`
+
+## Example Usage
+
+```python
+import os
+from layered_settings import initialize_settings
+from layered_settings import loaders
+
+get_setting = initialize_settings(
+    sources=[
+        # Lowest priority is setting-defaults.ini.  All configuration values should be defaulted in here.
+        # The `loaders.ConfigParserLoader` is optional - if you pass a string ending in .ini, it wraps it in
+        # a `loaders.ConfigParserLoader` for you.
+        loaders.ConfigParserLoader(os.path.join(SCRIPT_DIR, "setting-defaults.ini")),
+
+        # Next priority is a "user" settings file.
+        os.path.expanduser("~/.app-settings.ini"),
+
+        # You can include a dictionary in the sources too...
+        {
+            "general": {"CLIENT_NAME": "client"},
+            "email": {"EMAIL_HOST": "smtp.example.com", "EMAIL_PORT": 25},
+        },
+
+        # Secrets Manager works similar to SSM. If the secret is a json object, the object's keys will be the layered setting "key"
+        # If the secret is just plain text, the secret's name will be used as the key
+        loaders.SecretsManagerLoader(f"/app/stage/", aws_region="us-east-1") if ALLOW_SSM_CONFIGURATION else None,
+
+        # If we are able/willing to reach out to AWS, do so.  A `None` in the initialize_settings sources
+        # will simply be ignored.
+        loaders.SSMLoader(f"/app/stage/", aws_region="us-east-1") if ALLOW_SSM_CONFIGURATION else None,
+
+        # Top priority -- env var in the format APP__section__key.
+        loaders.EnvLoader("APP__{section}__{key}"),
+    ]
+)
+
+DATABASE_HOST = get_setting("database", "DATABASE_HOST")
+AWS_SECRET_KEY = get_setting("aws", "AWS_SECRET_KEY")
+...
+```
+
+## Frameworks Supported
+
+This library is tested using Python 3.x.
```

### Comparing `layered-settings-1.0.5/README.md` & `layered-settings-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # layered-settings
 
 `layered-settings` is a simple and configurable hierarchical settings library for Python, including Django, Flask, or any other
 scripts that need settings from potentially a variety of sources. With it you can load
-settings from the environment, Amazon's SSM, local configparser .ini files, and more.
+settings from the environment, Amazon's SSM, Amazon's Secrets Manager, local configparser .ini files, and more.
 
 ## Installation
 
 The package is available on pip as `layered-settings`. Run:
 
 `pip install layered-settings`
 
-If you want to use the AWS SSM layer, include the [ssm] extra:
+If you want to use the AWS SSM layer or Secrets Manager layer, include the [aws] extra:
 
-`pip install layered-settings[ssm]`
+`pip install layered-settings[aws]`
 
 then import via:
 
 `from layered_settings import initialize_settings, loaders`
 
 ## Example Usage
 
@@ -37,14 +37,18 @@
 
         # You can include a dictionary in the sources too...
         {
             "general": {"CLIENT_NAME": "client"},
             "email": {"EMAIL_HOST": "smtp.example.com", "EMAIL_PORT": 25},
         },
 
+        # Secrets Manager works similar to SSM. If the secret is a json object, the object's keys will be the layered setting "key"
+        # If the secret is just plain text, the secret's name will be used as the key
+        loaders.SecretsManagerLoader(f"/app/stage/", aws_region="us-east-1") if ALLOW_SSM_CONFIGURATION else None,
+
         # If we are able/willing to reach out to AWS, do so.  A `None` in the initialize_settings sources
         # will simply be ignored.
         loaders.SSMLoader(f"/app/stage/", aws_region="us-east-1") if ALLOW_SSM_CONFIGURATION else None,
 
         # Top priority -- env var in the format APP__section__key.
         loaders.EnvLoader("APP__{section}__{key}"),
     ]
```

### Comparing `layered-settings-1.0.5/layered_settings/layered_settings.py` & `layered-settings-1.1.0/layered_settings/layered_settings.py`

 * *Files identical despite different names*

### Comparing `layered-settings-1.0.5/layered_settings/loaders/config_parser_loader.py` & `layered-settings-1.1.0/layered_settings/loaders/config_parser_loader.py`

 * *Files identical despite different names*

### Comparing `layered-settings-1.0.5/layered_settings/loaders/env_loader.py` & `layered-settings-1.1.0/layered_settings/loaders/env_loader.py`

 * *Files identical despite different names*

### Comparing `layered-settings-1.0.5/layered_settings/loaders/ssm_loader.py` & `layered-settings-1.1.0/layered_settings/loaders/ssm_loader.py`

 * *Files identical despite different names*

### Comparing `layered-settings-1.0.5/layered_settings.egg-info/PKG-INFO` & `layered-settings-1.1.0/layered_settings.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,79 @@
 Metadata-Version: 2.1
 Name: layered-settings
-Version: 1.0.5
-Summary: Flexible, simple, extensible settings loader from environment, AWS SSM, configparser .ini, and more.
+Version: 1.1.0
+Summary: Flexible, simple, extensible settings loader from environment, AWS SSM, AWS Secrets Manager, configparser .ini, and more.
 Home-page: https://github.com/mathandpencil/layered-settings
 Author: Scott Stafford
 Author-email: scott.stafford+layered@gmail.com
-License: UNKNOWN
-Description: # layered-settings
-        
-        `layered-settings` is a simple and configurable hierarchical settings library for Python, including Django, Flask, or any other
-        scripts that need settings from potentially a variety of sources. With it you can load
-        settings from the environment, Amazon's SSM, local configparser .ini files, and more.
-        
-        ## Installation
-        
-        The package is available on pip as `layered-settings`. Run:
-        
-        `pip install layered-settings`
-        
-        If you want to use the AWS SSM layer, include the [ssm] extra:
-        
-        `pip install layered-settings[ssm]`
-        
-        then import via:
-        
-        `from layered_settings import initialize_settings, loaders`
-        
-        ## Example Usage
-        
-        ```python
-        import os
-        from layered_settings import initialize_settings
-        from layered_settings import loaders
-        
-        get_setting = initialize_settings(
-            sources=[
-                # Lowest priority is setting-defaults.ini.  All configuration values should be defaulted in here.
-                # The `loaders.ConfigParserLoader` is optional - if you pass a string ending in .ini, it wraps it in
-                # a `loaders.ConfigParserLoader` for you.
-                loaders.ConfigParserLoader(os.path.join(SCRIPT_DIR, "setting-defaults.ini")),
-        
-                # Next priority is a "user" settings file.
-                os.path.expanduser("~/.app-settings.ini"),
-        
-                # You can include a dictionary in the sources too...
-                {
-                    "general": {"CLIENT_NAME": "client"},
-                    "email": {"EMAIL_HOST": "smtp.example.com", "EMAIL_PORT": 25},
-                },
-        
-                # If we are able/willing to reach out to AWS, do so.  A `None` in the initialize_settings sources
-                # will simply be ignored.
-                loaders.SSMLoader(f"/app/stage/", aws_region="us-east-1") if ALLOW_SSM_CONFIGURATION else None,
-        
-                # Top priority -- env var in the format APP__section__key.
-                loaders.EnvLoader("APP__{section}__{key}"),
-            ]
-        )
-        
-        DATABASE_HOST = get_setting("database", "DATABASE_HOST")
-        AWS_SECRET_KEY = get_setting("aws", "AWS_SECRET_KEY")
-        ...
-        ```
-        
-        ## Frameworks Supported
-        
-        This library is tested using Python 3.x.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: ssm
+Provides-Extra: aws
+License-File: LICENSE
+
+# layered-settings
+
+`layered-settings` is a simple and configurable hierarchical settings library for Python, including Django, Flask, or any other
+scripts that need settings from potentially a variety of sources. With it you can load
+settings from the environment, Amazon's SSM, Amazon's Secrets Manager, local configparser .ini files, and more.
+
+## Installation
+
+The package is available on pip as `layered-settings`. Run:
+
+`pip install layered-settings`
+
+If you want to use the AWS SSM layer or Secrets Manager layer, include the [aws] extra:
+
+`pip install layered-settings[aws]`
+
+then import via:
+
+`from layered_settings import initialize_settings, loaders`
+
+## Example Usage
+
+```python
+import os
+from layered_settings import initialize_settings
+from layered_settings import loaders
+
+get_setting = initialize_settings(
+    sources=[
+        # Lowest priority is setting-defaults.ini.  All configuration values should be defaulted in here.
+        # The `loaders.ConfigParserLoader` is optional - if you pass a string ending in .ini, it wraps it in
+        # a `loaders.ConfigParserLoader` for you.
+        loaders.ConfigParserLoader(os.path.join(SCRIPT_DIR, "setting-defaults.ini")),
+
+        # Next priority is a "user" settings file.
+        os.path.expanduser("~/.app-settings.ini"),
+
+        # You can include a dictionary in the sources too...
+        {
+            "general": {"CLIENT_NAME": "client"},
+            "email": {"EMAIL_HOST": "smtp.example.com", "EMAIL_PORT": 25},
+        },
+
+        # Secrets Manager works similar to SSM. If the secret is a json object, the object's keys will be the layered setting "key"
+        # If the secret is just plain text, the secret's name will be used as the key
+        loaders.SecretsManagerLoader(f"/app/stage/", aws_region="us-east-1") if ALLOW_SSM_CONFIGURATION else None,
+
+        # If we are able/willing to reach out to AWS, do so.  A `None` in the initialize_settings sources
+        # will simply be ignored.
+        loaders.SSMLoader(f"/app/stage/", aws_region="us-east-1") if ALLOW_SSM_CONFIGURATION else None,
+
+        # Top priority -- env var in the format APP__section__key.
+        loaders.EnvLoader("APP__{section}__{key}"),
+    ]
+)
+
+DATABASE_HOST = get_setting("database", "DATABASE_HOST")
+AWS_SECRET_KEY = get_setting("aws", "AWS_SECRET_KEY")
+...
+```
+
+## Frameworks Supported
+
+This library is tested using Python 3.x.
```

### Comparing `layered-settings-1.0.5/layered_settings.egg-info/SOURCES.txt` & `layered-settings-1.1.0/layered_settings.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 layered_settings/__init__.py
 layered_settings/layered_settings.py
 layered_settings.egg-info/PKG-INFO
 layered_settings.egg-info/SOURCES.txt
 layered_settings.egg-info/dependency_links.txt
@@ -11,10 +13,11 @@
 layered_settings.egg-info/top_level.txt
 layered_settings/loaders/__init__.py
 layered_settings/loaders/base_loader.py
 layered_settings/loaders/callable_loader.py
 layered_settings/loaders/config_parser_loader.py
 layered_settings/loaders/dict_loader.py
 layered_settings/loaders/env_loader.py
+layered_settings/loaders/secrets_manager_loader.py
 layered_settings/loaders/ssm_loader.py
 tests/__init__.py
 tests/tests.py
```

### Comparing `layered-settings-1.0.5/setup.py` & `layered-settings-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="layered-settings",
-    version="1.0.5",
-    description="Flexible, simple, extensible settings loader from environment, AWS SSM, configparser .ini, and more.",
+    version="1.1.0",
+    description="Flexible, simple, extensible settings loader from environment, AWS SSM, AWS Secrets Manager, configparser .ini, and more.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mathandpencil/layered-settings",
     author="Scott Stafford",
     author_email="scott.stafford+layered@gmail.com",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     zip_safe=False,
     extras_require={
         "ssm": ["boto3"],
+        "aws": ["boto3"],
     },
 )
```

### Comparing `layered-settings-1.0.5/tests/tests.py` & `layered-settings-1.1.0/tests/tests.py`

 * *Files identical despite different names*

