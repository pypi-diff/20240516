# Comparing `tmp/scriptonite-1.0.1.tar.gz` & `tmp/scriptonite-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scriptonite-1.0.1.tar", max compression
+gzip compressed data, was "scriptonite-1.0.2.tar", max compression
```

## Comparing `scriptonite-1.0.1.tar` & `scriptonite-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,17 @@
--rw-r--r--   0        0        0     1006 2024-04-24 07:19:42.027260 scriptonite-1.0.1/README.md
--rw-r--r--   0        0        0      565 2024-04-25 14:08:58.570789 scriptonite-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      132 2024-04-24 10:20:40.388982 scriptonite-1.0.1/scriptonite/__init__.py
--rw-r--r--   0        0        0     6711 2024-04-25 13:24:13.508953 scriptonite-1.0.1/scriptonite/configuration.py
--rw-r--r--   0        0        0     3684 2024-04-25 13:39:04.091012 scriptonite-1.0.1/scriptonite/email.py
--rw-r--r--   0        0        0     6271 2024-04-25 14:08:15.594753 scriptonite-1.0.1/scriptonite/logging.py
--rw-r--r--   0        0        0     2144 2024-04-25 13:24:15.083137 scriptonite-1.0.1/scriptonite/utilities.py
--rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 scriptonite-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-29 14:08:55.063171 scriptonite-1.0.2/README.md
+-rw-r--r--   0        0        0      565 2024-05-15 16:20:40.769565 scriptonite-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-04-27 05:42:22.943283 scriptonite-1.0.2/scriptonite/.DS_Store
+-rw-r--r--   0        0        0      132 2024-04-24 10:20:40.388982 scriptonite-1.0.2/scriptonite/__init__.py
+-rw-r--r--   0        0        0     6783 2024-05-15 16:19:59.128391 scriptonite-1.0.2/scriptonite/configuration.py
+-rw-r--r--   0        0        0     6712 2024-05-15 15:55:39.000000 scriptonite-1.0.2/scriptonite/configuration.py~
+-rw-r--r--   0        0        0     3684 2024-04-29 16:07:52.050753 scriptonite-1.0.2/scriptonite/email.py
+-rw-r--r--   0        0        0     6271 2024-04-25 14:08:15.594753 scriptonite-1.0.2/scriptonite/logging.py
+-rw-r--r--   0        0        0       19 2024-04-25 15:42:01.543140 scriptonite-1.0.2/scriptonite/notify/__init__.py
+-rw-r--r--   0        0        0      196 2024-04-25 15:42:02.383198 scriptonite-1.0.2/scriptonite/notify/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      788 2024-04-25 15:42:02.384359 scriptonite-1.0.2/scriptonite/notify/__pycache__/base.cpython-312.pyc
+-rw-r--r--   0        0        0      501 2024-04-29 16:07:15.493378 scriptonite-1.0.2/scriptonite/notify/base.py
+-rw-r--r--   0        0        0     1008 2024-04-29 16:09:29.291161 scriptonite-1.0.2/scriptonite/notify/email.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:38:24.516242 scriptonite-1.0.2/scriptonite/notify/pushover.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:38:19.071336 scriptonite-1.0.2/scriptonite/notify/slack.py
+-rw-r--r--   0        0        0     2144 2024-04-25 13:24:15.083137 scriptonite-1.0.2/scriptonite/utilities.py
+-rw-r--r--   0        0        0     1706 1970-01-01 00:00:00.000000 scriptonite-1.0.2/PKG-INFO
```

### Comparing `scriptonite-1.0.1/README.md` & `scriptonite-1.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 log = Logger()
 
 log.info('Hello World!')
 ```
 
 #### Configuration
 
+For more complete configuration management, you can use [Dynaconf](https://www.dynaconf.com/)
+
 ```
 from scriptonite.configuration import Configuration
 
 configuration = Configuration(configfile="config.yaml",
                               env_prefix="MYCONFIG")
 
 ```
```

### Comparing `scriptonite-1.0.1/pyproject.toml` & `scriptonite-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scriptonite"
-version = "1.0.1"
+version = "1.0.2"
 description = "A toolkit for scripting in Python"
 authors = ["Andrea Mistrali <andrea@mistrali.pw>"]
 maintainers = ["Andrea Mistrali <andrea@mistrali.pw>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `scriptonite-1.0.1/scriptonite/configuration.py` & `scriptonite-1.0.2/scriptonite/configuration.py~`

 * *Files 0% similar despite different names*

```diff
@@ -41,21 +41,22 @@
         :param configfile: a configuration file to read
         :param file_loader: the loader to use to parse the config file,
                             defaults to `yaml_load` function, you can use
                             `json.load` or `toml.load` to parse other formats
         """
         super().__init__(defaults or {})
 
-        if env_prefix:
-            self.from_environ(prefix=env_prefix)
-
         if configfile:
             self.from_file(filename=configfile,
                            load=file_loader)
 
+        if env_prefix:
+            self.from_environ(prefix=env_prefix)
+
+
     def from_environ(self,
                      prefix: str = "APP_CONFIG",
                      loads: t.Callable[[str], t.Any] = json.loads) -> bool:
         """
         Loads configuration parsing environment variables.
         Prefix is the prefix of the variables (that will be stripped).
         Variables can build structures, using `__` as separator
```

### Comparing `scriptonite-1.0.1/scriptonite/email.py` & `scriptonite-1.0.2/scriptonite/email.py`

 * *Files identical despite different names*

### Comparing `scriptonite-1.0.1/scriptonite/logging.py` & `scriptonite-1.0.2/scriptonite/logging.py`

 * *Files identical despite different names*

### Comparing `scriptonite-1.0.1/scriptonite/utilities.py` & `scriptonite-1.0.2/scriptonite/utilities.py`

 * *Files identical despite different names*

### Comparing `scriptonite-1.0.1/PKG-INFO` & `scriptonite-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scriptonite
-Version: 1.0.1
+Version: 1.0.2
 Summary: A toolkit for scripting in Python
 License: GPL-3.0-or-later
 Author: Andrea Mistrali
 Author-email: andrea@mistrali.pw
 Maintainer: Andrea Mistrali
 Maintainer-email: andrea@mistrali.pw
 Requires-Python: >=3.10,<4.0
@@ -58,14 +58,16 @@
 log = Logger()
 
 log.info('Hello World!')
 ```
 
 #### Configuration
 
+For more complete configuration management, you can use [Dynaconf](https://www.dynaconf.com/)
+
 ```
 from scriptonite.configuration import Configuration
 
 configuration = Configuration(configfile="config.yaml",
                               env_prefix="MYCONFIG")
 
 ```
```

