# Comparing `tmp/netlink-alchemy-0.0.0.tar.gz` & `tmp/netlink-alchemy-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netlink-alchemy-0.0.0.tar", max compression
+gzip compressed data, was "netlink-alchemy-0.0.1.tar", max compression
```

## Comparing `netlink-alchemy-0.0.0.tar` & `netlink-alchemy-0.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      185 2022-07-12 08:49:20.084452 netlink-alchemy-0.0.0/netlink/alchemy/__init__.py
--rw-r--r--   0        0        0     1968 2022-07-12 08:47:54.424376 netlink-alchemy-0.0.0/netlink/alchemy/_integer.py
--rw-r--r--   0        0        0      798 2022-07-12 08:38:10.868956 netlink-alchemy-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      258 2022-07-12 08:45:28.102091 netlink-alchemy-0.0.0/README.md
--rw-r--r--   0        0        0      977 2022-07-12 08:53:56.276618 netlink-alchemy-0.0.0/setup.py
--rw-r--r--   0        0        0     1098 2022-07-12 08:53:56.276618 netlink-alchemy-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      185 2022-07-12 08:49:20.084452 netlink-alchemy-0.0.1/netlink/alchemy/__init__.py
+-rw-r--r--   0        0        0     1968 2022-07-12 08:47:54.424376 netlink-alchemy-0.0.1/netlink/alchemy/_integer.py
+-rw-r--r--   0        0        0      801 2023-12-04 11:04:44.710211 netlink-alchemy-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      258 2022-07-12 08:45:28.102091 netlink-alchemy-0.0.1/README.md
+-rw-r--r--   0        0        0      978 2023-12-04 11:39:11.399235 netlink-alchemy-0.0.1/setup.py
+-rw-r--r--   0        0        0     1049 2023-12-04 11:39:11.399235 netlink-alchemy-0.0.1/PKG-INFO
```

### Comparing `netlink-alchemy-0.0.0/netlink/alchemy/_integer.py` & `netlink-alchemy-0.0.1/netlink/alchemy/_integer.py`

 * *Files identical despite different names*

### Comparing `netlink-alchemy-0.0.0/pyproject.toml` & `netlink-alchemy-0.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "netlink-alchemy"
-version = "0.0.0"
+version = "0.0.1"
 description = "Extensions for SQL Alchemy"
 license = "MIT"
 authors = ["Bernhard Radermacher <bernhard.radermacher@netlink-consulting.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/netlink_python/netlink-sharepoint"
 keywords = ["SQL SQLAlchemy Alchemy MySQL MariaDB"]
 classifiers = ["Topic :: Software Development"]
 packages = [ { include = "netlink/alchemy" } ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
-SQLAlchemy = "^1.4.39"
+python = ">=3.8,<3.12"
+SQLAlchemy = "^2.0.23"
 
 [tool.poetry.dev-dependencies]
-black = "^22.3.0"
-pytest = "^7.1.2"
+black = "^23.11.0"
+pytest = "^7.4.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `netlink-alchemy-0.0.0/setup.py` & `netlink-alchemy-0.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 packages = \
 ['alchemy']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['SQLAlchemy>=1.4.39,<2.0.0']
+['SQLAlchemy>=2.0.23,<3.0.0']
 
 setup_kwargs = {
     'name': 'netlink-alchemy',
-    'version': '0.0.0',
+    'version': '0.0.1',
     'description': 'Extensions for SQL Alchemy',
     'long_description': '# netlink-alchemy\n\nExtensions for SQL Alchemy\n\nAdditional Types (implemented for MySQL and MariaDB):\n\n- `TinyInteger`\n- `UnsignedTinyInteger`\n\n- `UnsignedSmallInteger`\n\n- `MediumInteger`\n- `UnsignedMediumInteger`\n\n- `UnsignedInteger`\n\n- `UnsignedBigInteger`\n',
     'author': 'Bernhard Radermacher',
     'author_email': 'bernhard.radermacher@netlink-consulting.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/netlink_python/netlink-sharepoint',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `netlink-alchemy-0.0.0/PKG-INFO` & `netlink-alchemy-0.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: netlink-alchemy
-Version: 0.0.0
+Version: 0.0.1
 Summary: Extensions for SQL Alchemy
 Home-page: https://gitlab.com/netlink_python/netlink-sharepoint
 License: MIT
 Keywords: SQL SQLAlchemy Alchemy MySQL MariaDB
 Author: Bernhard Radermacher
 Author-email: bernhard.radermacher@netlink-consulting.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
-Requires-Dist: SQLAlchemy (>=1.4.39,<2.0.0)
+Requires-Dist: SQLAlchemy (>=2.0.23,<3.0.0)
 Project-URL: Repository, https://gitlab.com/netlink_python/netlink-sharepoint
 Description-Content-Type: text/markdown
 
 # netlink-alchemy
 
 Extensions for SQL Alchemy
```

