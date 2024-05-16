# Comparing `tmp/netlink-core-1.1.1.tar.gz` & `tmp/netlink-core-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netlink-core-1.1.1.tar", max compression
+gzip compressed data, was "netlink-core-1.1.2.tar", max compression
```

## Comparing `netlink-core-1.1.1.tar` & `netlink-core-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2022-03-08 08:32:23.896000 netlink-core-1.1.1/LICENSE.md
--rw-r--r--   0        0        0      258 2023-09-17 08:07:34.824629 netlink-core-1.1.1/netlink/core/__init__.py
--rw-r--r--   0        0        0     2951 2023-09-17 08:07:34.855904 netlink-core-1.1.1/netlink/core/attribute_mapping.py
--rw-r--r--   0        0        0      383 2022-06-30 12:06:16.640368 netlink-core-1.1.1/netlink/core/cli.py
--rw-r--r--   0        0        0     1779 2022-07-09 10:16:28.731139 netlink-core-1.1.1/netlink/core/config.py
--rw-r--r--   0        0        0     1562 2023-09-17 08:07:34.855904 netlink-core-1.1.1/netlink/core/configuration.py
--rw-r--r--   0        0        0      684 2022-06-30 12:06:16.648364 netlink-core-1.1.1/netlink/core/generation.py
--rw-r--r--   0        0        0      606 2023-09-17 08:07:34.855904 netlink-core-1.1.1/netlink/core/mapping.py
--rw-r--r--   0        0        0     1230 2023-09-17 08:07:34.887168 netlink-core-1.1.1/netlink/core/named_mapping.py
--rw-r--r--   0        0        0      296 2022-07-01 06:48:21.523504 netlink-core-1.1.1/netlink/core/singleton.py
--rw-r--r--   0        0        0      822 2023-11-17 07:43:25.149905 netlink-core-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2315 2022-10-21 07:08:40.058788 netlink-core-1.1.1/README.md
--rw-r--r--   0        0        0     3251 2023-11-17 07:43:37.559999 netlink-core-1.1.1/setup.py
--rw-r--r--   0        0        0     3075 2023-11-17 07:43:37.559999 netlink-core-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-03-08 08:32:23.896000 netlink-core-1.1.2/LICENSE.md
+-rw-r--r--   0        0        0      258 2023-09-17 08:07:34.824629 netlink-core-1.1.2/netlink/core/__init__.py
+-rw-r--r--   0        0        0     2951 2023-09-17 08:07:34.855904 netlink-core-1.1.2/netlink/core/attribute_mapping.py
+-rw-r--r--   0        0        0      383 2022-06-30 12:06:16.640368 netlink-core-1.1.2/netlink/core/cli.py
+-rw-r--r--   0        0        0     1779 2022-07-09 10:16:28.731139 netlink-core-1.1.2/netlink/core/config.py
+-rw-r--r--   0        0        0     1562 2023-09-17 08:07:34.855904 netlink-core-1.1.2/netlink/core/configuration.py
+-rw-r--r--   0        0        0      684 2022-06-30 12:06:16.648364 netlink-core-1.1.2/netlink/core/generation.py
+-rw-r--r--   0        0        0      606 2023-09-17 08:07:34.855904 netlink-core-1.1.2/netlink/core/mapping.py
+-rw-r--r--   0        0        0     1230 2023-09-17 08:07:34.887168 netlink-core-1.1.2/netlink/core/named_mapping.py
+-rw-r--r--   0        0        0      296 2022-07-01 06:48:21.523504 netlink-core-1.1.2/netlink/core/singleton.py
+-rw-r--r--   0        0        0      835 2024-05-16 06:48:39.141387 netlink-core-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2315 2022-10-21 07:08:40.058788 netlink-core-1.1.2/README.md
+-rw-r--r--   0        0        0     3254 2024-05-16 06:49:47.648021 netlink-core-1.1.2/setup.py
+-rw-r--r--   0        0        0     3078 2024-05-16 06:49:47.648021 netlink-core-1.1.2/PKG-INFO
```

### Comparing `netlink-core-1.1.1/LICENSE.md` & `netlink-core-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `netlink-core-1.1.1/netlink/core/attribute_mapping.py` & `netlink-core-1.1.2/netlink/core/attribute_mapping.py`

 * *Files identical despite different names*

### Comparing `netlink-core-1.1.1/netlink/core/config.py` & `netlink-core-1.1.2/netlink/core/config.py`

 * *Files identical despite different names*

### Comparing `netlink-core-1.1.1/netlink/core/configuration.py` & `netlink-core-1.1.2/netlink/core/configuration.py`

 * *Files identical despite different names*

### Comparing `netlink-core-1.1.1/netlink/core/generation.py` & `netlink-core-1.1.2/netlink/core/generation.py`

 * *Files identical despite different names*

### Comparing `netlink-core-1.1.1/netlink/core/mapping.py` & `netlink-core-1.1.2/netlink/core/mapping.py`

 * *Files identical despite different names*

### Comparing `netlink-core-1.1.1/netlink/core/named_mapping.py` & `netlink-core-1.1.2/netlink/core/named_mapping.py`

 * *Files identical despite different names*

### Comparing `netlink-core-1.1.1/pyproject.toml` & `netlink-core-1.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "netlink-core"
-version = "1.1.1"
+version = "1.1.2"
 description = "Core components of NetLink tools"
 license = "MIT"
 authors = ["Bernhard Radermacher <bernhard.radermacher@netlink-consulting.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/netlink_python/netlink-core.git"
 classifiers = ["Topic :: Software Development"]
 packages = [ { include = "netlink/core" } ]
 
 [tool.poetry.scripts]
 create_netlink_defaults = 'netlink.core.cli:create_netlink_defaults'
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.13"
+python = ">=3.8,<=3.12"
 toml = ">=0.10.2"
-PyYAML = ">=6.0"
+PyYAML = ">=6.0.1"
 
 [tool.poetry.dev-dependencies]
-black = "^23.11.0"
-pytest = "^7.4.3"
+black = ">=24.4.2"
+pytest = ">=8.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-line-length = 120
-target-version = ['py38', 'py39', 'py310', 'py311']
+line-length = 150
+target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
```

### Comparing `netlink-core-1.1.1/README.md` & `netlink-core-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `netlink-core-1.1.1/setup.py` & `netlink-core-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 packages = \
 ['core']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['PyYAML>=6.0', 'toml>=0.10.2']
+['PyYAML>=6.0.1', 'toml>=0.10.2']
 
 entry_points = \
 {'console_scripts': ['create_netlink_defaults = '
                      'netlink.core.cli:create_netlink_defaults']}
 
 setup_kwargs = {
     'name': 'netlink-core',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'Core components of NetLink tools',
     'long_description': "# netlink-core\n\nCore components of NetLink tools\n\n## Updates\n\n### 0.0.4\n\nAdd `netlink.core.Mapping` Abstract class, must implement `__init__`.\n\nThis provides a small set of functionality share by my collection of tools:\n\n- [netlink-crypt](https://pypi.org/project/netlink-crypt/)\n- [netlink-logging](https://pypi.org/project/netlink-logging/)\n- [netlink-sap-rfc](https://pypi.org/project/netlink-sap-rfc/)\n- [netlink-sharepoint](https://pypi.org/project/netlink-sharepoint/)\n\n## Contents\n\n- Centralized configuration using [TOML](https://toml.io/en/)\n  in the users home directory (subdirectory `.netlink`).\n\n### Classes\n\n#### netlink.core.AttributeMapping\n\nbehaves like an immutable mapping, adding access to all items via property notation:\n\n      a['b'] == a.b\n\nThis is propagated through all levels, when parameter `deep` is `True` (default):\n\n      a['b']['c']['d'] == a.b.c.d\n\n| Parameter      | Default        |                                                                                               |\n|----------------|----------------|-----------------------------------------------------------------------------------------------|\n| value          | **mandatory**  | Mapping containing information. Might be deep.                                                |\n| deep           | `True`         | Items within the mapping will be copied, not referenced (implemented for Lists and Mappings). |\n| case_sensitive | `False`        | If **False**, ignore case when retrieving items or attributes.                                |\n| under          | `True`         | Try dash (`-`) if underscore (`_`) in name not found. |\n\n#### netlink.core.Singleton\n\nis a base class to be inherited from to make all instances of a class the same.\n\n#### netlink.core.Config\n\nis a Singleton that provides configuration information (will be initialized the first time).\n\n### Scripts\n\n- `create_netlink_defaults` creates a TOML file containing all currently internal defaults in the users home directory (\n  subdirectory `.netlink`). If the file already exist, the current file is copied as a backup with extension `.001`.\n\n## Installation\n\nUse your preferred tool to install from [PyPI](https://pypi.org/). I prefer [Poetry](https://python-poetry.org/).\n\n[//]: # (## Roadmap)\n\n[//]: # (## Contributing)\n\n## License\n\nMIT\n",
     'author': 'Bernhard Radermacher',
     'author_email': 'bernhard.radermacher@netlink-consulting.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/netlink_python/netlink-core.git',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.13',
+    'python_requires': '>=3.8,<=3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `netlink-core-1.1.1/PKG-INFO` & `netlink-core-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: netlink-core
-Version: 1.1.1
+Version: 1.1.2
 Summary: Core components of NetLink tools
 Home-page: https://gitlab.com/netlink_python/netlink-core.git
 License: MIT
 Author: Bernhard Radermacher
 Author-email: bernhard.radermacher@netlink-consulting.com
-Requires-Python: >=3.8,<3.13
+Requires-Python: >=3.8,<=3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
-Requires-Dist: PyYAML (>=6.0)
+Requires-Dist: PyYAML (>=6.0.1)
 Requires-Dist: toml (>=0.10.2)
 Project-URL: Repository, https://gitlab.com/netlink_python/netlink-core.git
 Description-Content-Type: text/markdown
 
 # netlink-core
 
 Core components of NetLink tools
```

