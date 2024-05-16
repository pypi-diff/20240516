# Comparing `tmp/p4adev_tools-0.0.2.tar.gz` & `tmp/p4adev_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p4adev_tools-0.0.2.tar", max compression
+gzip compressed data, was "p4adev_tools-0.0.3.tar", max compression
```

## Comparing `p4adev_tools-0.0.2.tar` & `p4adev_tools-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11324 2024-04-09 03:49:43.737319 p4adev_tools-0.0.2/LICENSE
--rw-r--r--   0        0        0     2552 2024-04-09 03:55:23.282300 p4adev_tools-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      122 2024-04-09 03:09:16.596456 p4adev_tools-0.0.2/src/p4adev_tools/__init__.py
--rw-r--r--   0        0        0     1522 2024-04-09 03:55:19.269300 p4adev_tools-0.0.2/src/p4adev_tools/ftp_server.py
--rw-r--r--   0        0        0     6720 2024-04-09 03:14:10.625439 p4adev_tools-0.0.2/src/p4adev_tools/ipykernel_threaded.py
--rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 p4adev_tools-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-09 03:49:43.737319 p4adev_tools-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2852 2024-05-17 18:58:29.953466 p4adev_tools-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-04-09 03:09:16.596456 p4adev_tools-0.0.3/src/p4adev_tools/__init__.py
+-rw-r--r--   0        0        0     1867 2024-05-17 18:50:42.707491 p4adev_tools-0.0.3/src/p4adev_tools/ftp_server.py
+-rw-r--r--   0        0        0     6778 2024-05-17 18:46:40.430505 p4adev_tools-0.0.3/src/p4adev_tools/ipykernel_threaded.py
+-rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 p4adev_tools-0.0.3/PKG-INFO
```

### Comparing `p4adev_tools-0.0.2/LICENSE` & `p4adev_tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `p4adev_tools-0.0.2/pyproject.toml` & `p4adev_tools-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "p4adev_tools"
-version = "0.0.2"
+version = "0.0.3"
 description = "Collection of widgets for the older kivymd 1.1.1 lib (material design 2)."
 authors = ["BlackCatDevel0per <bcdev@mail.ru>"]
 license = "Apache 2.0"
 
 packages = [
     { include = "p4adev_tools", from = "src" },
 ]
 
 [tool.poetry.urls]
 Homepage = "https://github.com/BlackCatDevel0per/p4adev_tools"
 Documentation = "https://github.com/BlackCatDevel0per/p4adev_tools"
 Repository = "https://github.com/BlackCatDevel0per/p4adev_tools"
 
 # TODO: Execute without wait to end (poetry will closed while task is pending)
+# List commands with `poetry user-commands`
 [tool.poetry-plugin-commands]
 stree = "tree src"
 # TODO: Make some examples (like kivy garden or etc.)
 run-ftpserv = "PYTHONPATH=src:. poetry run python src/p4adev_tools/ftp_server.py"
 run-ipyk = "PYTHONPATH=src:. poetry run python src/p4adev_tools/ipykernel_threaded.py"
 
 [tool.ruff]
@@ -115,31 +116,44 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 plyer = "^2.1.0"
 
 
-[tool.poetry.group.main]
+[tool.poetry-plugin-deps-juice]
+"poetry" = [
+	"base",
+]
+
+
+[tool.poetry.group.base]
 optional = false
 
-[tool.poetry.group.main.dependencies]
+[tool.poetry.group.base.dependencies]
 pyftpdlib = "^1.5.9"
 ipykernel = "^6.29.4"
 jedi = "0.19.1"
 ipython = "8.12.3"
 
 # TODO: Replace it..
 background-zmq-ipython = "^1.20220901.135250"
 
+[tool.poetry.group.poetry-plugins]
+optional = true
+
+[tool.poetry.group.poetry-plugins.dependencies]
+poetry-plugin-commands = "^0.0.9"
+poetry-plugin-deps-juice = "^0.0.3"
+
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-poetry-plugin-commands = "^0.0.8"
+poetry-plugin-commands = "^0.0.9"
 
 pytest = "^7.4.2"
 pytest-dependency = "^0.5.1"
 ruff = "^0.0.292"
 build = "^1.0.3"
 setuptools = "^69.0.3"
 wheel = "^0.42.0"
@@ -148,10 +162,11 @@
 ftputil = "^5.1.0"
 
 [tool.poetry.group.other.dependencies]
 rich = "^13.7.0"
 
 
 [build-system]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `p4adev_tools-0.0.2/src/p4adev_tools/ipykernel_threaded.py` & `p4adev_tools-0.0.3/src/p4adev_tools/ipykernel_threaded.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,17 @@
 
 	# Force disable debugpy
 	import ipykernel.debugger as ipydbg
 	ipydbg._is_debugpy_available = False  # noqa: SLF001
 
 	if platform == 'android':
 		# Set to app dir near `.kivy` dir
-		dir_aipyp = os_environ['IPYTHONDIR'] = os_environ['ANDROID_ARGUMENT'] + '/' + '.ipython'
+		dir_aipyp = os_environ['IPYTHONDIR'] = os_environ.get(
+			'ANDROID_APP_CONF_PATH', os_environ.get('ANDROID_ARGUMENT', '.'),
+		) + '/' + '.ipython'
 		file_kfp = Path(dir_aipyp, kfn)
 
 		mkdirs(dir_aipyp, exist_ok=True)
 
 		del dir_aipyp
 
 	ipy_conf: dict = {
```

### Comparing `p4adev_tools-0.0.2/PKG-INFO` & `p4adev_tools-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p4adev_tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Collection of widgets for the older kivymd 1.1.1 lib (material design 2).
 License: Apache 2.0
 Author: BlackCatDevel0per
 Author-email: bcdev@mail.ru
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,11 +12,12 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: background-zmq-ipython (>=1.20220901.135250,<2.0.0)
 Requires-Dist: ipykernel (>=6.29.4,<7.0.0)
 Requires-Dist: ipython (==8.12.3)
 Requires-Dist: jedi (==0.19.1)
+Requires-Dist: plyer (>=2.1.0,<3.0.0)
 Requires-Dist: pyftpdlib (>=1.5.9,<2.0.0)
 Project-URL: Documentation, https://github.com/BlackCatDevel0per/p4adev_tools
 Project-URL: Homepage, https://github.com/BlackCatDevel0per/p4adev_tools
 Project-URL: Repository, https://github.com/BlackCatDevel0per/p4adev_tools
```

