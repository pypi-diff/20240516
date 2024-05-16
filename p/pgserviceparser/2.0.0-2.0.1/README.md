# Comparing `tmp/pgserviceparser-2.0.0.tar.gz` & `tmp/pgserviceparser-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgserviceparser-2.0.0.tar", last modified: Wed Apr 17 07:44:21 2024, max compression
+gzip compressed data, was "pgserviceparser-2.0.1.tar", last modified: Tue Apr 30 13:42:17 2024, max compression
```

## Comparing `pgserviceparser-2.0.0.tar` & `pgserviceparser-2.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/.github/workflows/docs_builder.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/.github/workflows/wheel.yml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/docs/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/pgserviceparser/
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/pgserviceparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/pgserviceparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-17 07:44:21.000000 pgserviceparser-2.0.0/pgserviceparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-17 07:44:21.000000 pgserviceparser-2.0.0/pgserviceparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:44:21.000000 pgserviceparser-2.0.0/pgserviceparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 07:44:21.000000 pgserviceparser-2.0.0/pgserviceparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/test/data/service_base.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/test/test_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:42:17.419590 pgserviceparser-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:42:17.415590 pgserviceparser-2.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:42:17.419590 pgserviceparser-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/.github/workflows/docs_builder.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/.github/workflows/wheel.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-30 13:42:17.419590 pgserviceparser-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:42:17.419590 pgserviceparser-2.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:42:17.419590 pgserviceparser-2.0.1/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/docs/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:42:17.419590 pgserviceparser-2.0.1/pgserviceparser/
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/pgserviceparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:42:17.419590 pgserviceparser-2.0.1/pgserviceparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-30 13:42:17.000000 pgserviceparser-2.0.1/pgserviceparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-30 13:42:17.000000 pgserviceparser-2.0.1/pgserviceparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:42:17.000000 pgserviceparser-2.0.1/pgserviceparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 13:42:17.000000 pgserviceparser-2.0.1/pgserviceparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:42:17.419590 pgserviceparser-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:42:17.419590 pgserviceparser-2.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:42:17.419590 pgserviceparser-2.0.1/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/test/data/service_base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-30 13:42:04.000000 pgserviceparser-2.0.1/test/test_lib.py
```

### Comparing `pgserviceparser-2.0.0/.github/workflows/docs_builder.yml` & `pgserviceparser-2.0.1/.github/workflows/docs_builder.yml`

 * *Files identical despite different names*

### Comparing `pgserviceparser-2.0.0/.github/workflows/release.yml` & `pgserviceparser-2.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pgserviceparser-2.0.0/.github/workflows/test.yml` & `pgserviceparser-2.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pgserviceparser-2.0.0/.github/workflows/wheel.yml` & `pgserviceparser-2.0.1/.github/workflows/wheel.yml`

 * *Files identical despite different names*

### Comparing `pgserviceparser-2.0.0/.pre-commit-config.yaml` & `pgserviceparser-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pgserviceparser-2.0.0/LICENSE` & `pgserviceparser-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pgserviceparser-2.0.0/PKG-INFO` & `pgserviceparser-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgserviceparser
-Version: 2.0.0
+Version: 2.0.1
 Summary: A package parsing the PostgreSQL connection service file
 Author-email: David Signer <info@opengis.ch>, Julien Moura <julien.moura@oslandia.com>, Germán Carrillo <info@opengis.ch>, Denis Rouzaud <info@opengis.ch>
 License: MIT License
 Project-URL: homepage, https://opengisch.github.io/pgserviceparser/
 Project-URL: repository, https://github.com/opengisch/pgserviceparser
 Project-URL: tracker, https://github.com/opengisch/pgserviceparser/issues
 Keywords: postgres,service
```

### Comparing `pgserviceparser-2.0.0/README.md` & `pgserviceparser-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pgserviceparser-2.0.0/pgserviceparser/__init__.py` & `pgserviceparser-2.0.1/pgserviceparser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
     config = full_config(conf_file_path)
     if service_name not in config:
         raise ServiceNotFound(service_name)
 
     config[service_name][setting_key] = setting_value
     with open(conf_file_path or conf_path(), "w") as configfile:
-        config.write(configfile)
+        config.write(configfile, space_around_delimiters=False)
 
 
 def write_service(
     service_name: str,
     settings: dict,
     conf_file_path: Optional[str] = None,
 ):
@@ -112,15 +112,15 @@
     """
     config = full_config(conf_file_path)
     if service_name not in config:
         raise ServiceNotFound(service_name)
 
     config[service_name] = settings.copy()
     with open(conf_file_path or conf_path(), "w") as configfile:
-        config.write(configfile)
+        config.write(configfile, space_around_delimiters=False)
 
 
 def service_names(conf_file_path: Optional[str] = None) -> list[str]:
     """Returns all service names in a list.
 
     Args:
         conf_file_path: path to the pg_service.conf. If None the `conf_path()` is used, defaults to None
```

### Comparing `pgserviceparser-2.0.0/pgserviceparser.egg-info/PKG-INFO` & `pgserviceparser-2.0.1/pgserviceparser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgserviceparser
-Version: 2.0.0
+Version: 2.0.1
 Summary: A package parsing the PostgreSQL connection service file
 Author-email: David Signer <info@opengis.ch>, Julien Moura <julien.moura@oslandia.com>, Germán Carrillo <info@opengis.ch>, Denis Rouzaud <info@opengis.ch>
 License: MIT License
 Project-URL: homepage, https://opengisch.github.io/pgserviceparser/
 Project-URL: repository, https://github.com/opengisch/pgserviceparser
 Project-URL: tracker, https://github.com/opengisch/pgserviceparser/issues
 Keywords: postgres,service
```

### Comparing `pgserviceparser-2.0.0/pgserviceparser.egg-info/SOURCES.txt` & `pgserviceparser-2.0.1/pgserviceparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pgserviceparser-2.0.0/pyproject.toml` & `pgserviceparser-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pgserviceparser-2.0.0/test/test_lib.py` & `pgserviceparser-2.0.1/test/test_lib.py`

 * *Files 20% similar despite different names*

```diff
@@ -51,23 +51,41 @@
 
         # Create setting
         write_service_setting("service_1", "new_key", "new_value")
         conf = service_config("service_1")
         self.assertIn("new_key", conf)
         self.assertEqual(conf["new_key"], "new_value")
 
+        self.assertEqual(
+            open(self.service_file_path).read().find(" = "),
+            -1,
+            "Whitespaces between delimiters were found, but should not be present",
+        )
+
         # Overwrite setting
         write_service_setting("service_1", "port", "1")
         conf = service_config("service_1")
         self.assertEqual(conf["port"], "1")
 
+        self.assertEqual(
+            open(self.service_file_path).read().find(" = "),
+            -1,
+            "Whitespaces between delimiters were found, but should not be present",
+        )
+
     def test_write_service(self):
         self.assertRaises(ServiceNotFound, write_service, "non_existing_service", {"key": "value"})
 
         # Overwrite the whole service_3 config using service_2 params
         config_3 = service_config("service_3")
         self.assertEqual(
             config_3, {"host": "host_3", "dbname": "db_3", "port": "3333", "user": "user_3", "password": "pwd_3"}
         )
         config_2 = service_config("service_2")
         write_service("service_3", config_2)
         self.assertEqual(service_config("service_3"), config_2)
+
+        self.assertEqual(
+            open(self.service_file_path).read().find(" = "),
+            -1,
+            "Whitespaces between delimiters were found, but should not be present",
+        )
```

