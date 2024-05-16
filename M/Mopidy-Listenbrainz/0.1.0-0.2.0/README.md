# Comparing `tmp/Mopidy-Listenbrainz-0.1.0.tar.gz` & `tmp/mopidy_listenbrainz-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mopidy-Listenbrainz-0.1.0.tar", last modified: Mon Dec 27 19:33:26 2021, max compression
+gzip compressed data, was "mopidy_listenbrainz-0.2.0.tar", last modified: Thu May 16 18:23:33 2024, max compression
```

## Comparing `Mopidy-Listenbrainz-0.1.0.tar` & `mopidy_listenbrainz-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2021-12-27 19:33:26.831288 Mopidy-Listenbrainz-0.1.0/
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2021-12-27 19:33:26.828288 Mopidy-Listenbrainz-0.1.0/.github/
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2021-12-27 19:33:26.829288 Mopidy-Listenbrainz-0.1.0/.github/workflows/
--rw-r--r--   0 m         (1000) m         (1000)     1566 2021-12-17 03:02:28.000000 Mopidy-Listenbrainz-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0 m         (1000) m         (1000)      477 2021-12-17 03:02:28.000000 Mopidy-Listenbrainz-0.1.0/.github/workflows/release.yml
--rw-r--r--   0 m         (1000) m         (1000)    11357 2021-12-17 03:02:28.000000 Mopidy-Listenbrainz-0.1.0/LICENSE
--rw-r--r--   0 m         (1000) m         (1000)      236 2021-12-17 03:02:28.000000 Mopidy-Listenbrainz-0.1.0/MANIFEST.in
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2021-12-27 19:33:26.830288 Mopidy-Listenbrainz-0.1.0/Mopidy_Listenbrainz.egg-info/
--rw-r--r--   0 m         (1000) m         (1000)     3096 2021-12-27 19:33:26.000000 Mopidy-Listenbrainz-0.1.0/Mopidy_Listenbrainz.egg-info/PKG-INFO
--rw-r--r--   0 m         (1000) m         (1000)      623 2021-12-27 19:33:26.000000 Mopidy-Listenbrainz-0.1.0/Mopidy_Listenbrainz.egg-info/SOURCES.txt
--rw-r--r--   0 m         (1000) m         (1000)        1 2021-12-27 19:33:26.000000 Mopidy-Listenbrainz-0.1.0/Mopidy_Listenbrainz.egg-info/dependency_links.txt
--rw-r--r--   0 m         (1000) m         (1000)       59 2021-12-27 19:33:26.000000 Mopidy-Listenbrainz-0.1.0/Mopidy_Listenbrainz.egg-info/entry_points.txt
--rw-r--r--   0 m         (1000) m         (1000)        1 2021-12-17 04:51:27.000000 Mopidy-Listenbrainz-0.1.0/Mopidy_Listenbrainz.egg-info/not-zip-safe
--rw-r--r--   0 m         (1000) m         (1000)      297 2021-12-27 19:33:26.000000 Mopidy-Listenbrainz-0.1.0/Mopidy_Listenbrainz.egg-info/requires.txt
--rw-r--r--   0 m         (1000) m         (1000)       20 2021-12-27 19:33:26.000000 Mopidy-Listenbrainz-0.1.0/Mopidy_Listenbrainz.egg-info/top_level.txt
--rw-r--r--   0 m         (1000) m         (1000)     3096 2021-12-27 19:33:26.831288 Mopidy-Listenbrainz-0.1.0/PKG-INFO
--rw-r--r--   0 m         (1000) m         (1000)     2145 2021-12-27 19:32:56.000000 Mopidy-Listenbrainz-0.1.0/README.rst
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2021-12-27 19:33:26.830288 Mopidy-Listenbrainz-0.1.0/mopidy_listenbrainz/
--rw-r--r--   0 m         (1000) m         (1000)      702 2021-12-18 18:34:08.000000 Mopidy-Listenbrainz-0.1.0/mopidy_listenbrainz/__init__.py
--rw-r--r--   0 m         (1000) m         (1000)       66 2021-12-17 04:24:28.000000 Mopidy-Listenbrainz-0.1.0/mopidy_listenbrainz/ext.conf
--rw-r--r--   0 m         (1000) m         (1000)     2060 2021-12-18 18:34:43.000000 Mopidy-Listenbrainz-0.1.0/mopidy_listenbrainz/frontend.py
--rw-r--r--   0 m         (1000) m         (1000)     2048 2021-12-18 18:35:34.000000 Mopidy-Listenbrainz-0.1.0/mopidy_listenbrainz/listenbrainz.py
--rw-r--r--   0 m         (1000) m         (1000)      342 2021-12-17 03:02:28.000000 Mopidy-Listenbrainz-0.1.0/pyproject.toml
--rw-r--r--   0 m         (1000) m         (1000)     1506 2021-12-27 19:33:26.831288 Mopidy-Listenbrainz-0.1.0/setup.cfg
--rw-r--r--   0 m         (1000) m         (1000)       38 2021-12-17 03:02:28.000000 Mopidy-Listenbrainz-0.1.0/setup.py
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2021-12-27 19:33:26.830288 Mopidy-Listenbrainz-0.1.0/tests/
--rw-r--r--   0 m         (1000) m         (1000)        0 2021-12-17 03:02:28.000000 Mopidy-Listenbrainz-0.1.0/tests/__init__.py
--rw-r--r--   0 m         (1000) m         (1000)      703 2021-12-17 05:24:55.000000 Mopidy-Listenbrainz-0.1.0/tests/test_extension.py
--rw-r--r--   0 m         (1000) m         (1000)     5386 2021-12-18 03:30:00.000000 Mopidy-Listenbrainz-0.1.0/tests/test_frontend.py
--rw-r--r--   0 m         (1000) m         (1000)      415 2021-12-17 03:07:22.000000 Mopidy-Listenbrainz-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:23:33.700580 mopidy_listenbrainz-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:23:33.696580 mopidy_listenbrainz-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:23:33.696580 mopidy_listenbrainz-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:23:33.700580 mopidy_listenbrainz-0.2.0/Mopidy_Listenbrainz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-16 18:23:33.000000 mopidy_listenbrainz-0.2.0/Mopidy_Listenbrainz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-16 18:23:33.000000 mopidy_listenbrainz-0.2.0/Mopidy_Listenbrainz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:23:33.000000 mopidy_listenbrainz-0.2.0/Mopidy_Listenbrainz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-16 18:23:33.000000 mopidy_listenbrainz-0.2.0/Mopidy_Listenbrainz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:23:33.000000 mopidy_listenbrainz-0.2.0/Mopidy_Listenbrainz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-16 18:23:33.000000 mopidy_listenbrainz-0.2.0/Mopidy_Listenbrainz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 18:23:33.000000 mopidy_listenbrainz-0.2.0/Mopidy_Listenbrainz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-16 18:23:33.700580 mopidy_listenbrainz-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:23:33.700580 mopidy_listenbrainz-0.2.0/mopidy_listenbrainz/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/mopidy_listenbrainz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/mopidy_listenbrainz/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/mopidy_listenbrainz/ext.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/mopidy_listenbrainz/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/mopidy_listenbrainz/listenbrainz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/mopidy_listenbrainz/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-16 18:23:33.700580 mopidy_listenbrainz-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:23:33.700580 mopidy_listenbrainz-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/tests/test_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-16 18:23:30.000000 mopidy_listenbrainz-0.2.0/tox.ini
```

### Comparing `Mopidy-Listenbrainz-0.1.0/LICENSE` & `mopidy_listenbrainz-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Mopidy-Listenbrainz-0.1.0/Mopidy_Listenbrainz.egg-info/PKG-INFO` & `mopidy_listenbrainz-0.2.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: Mopidy-Listenbrainz
-Version: 0.1.0
-Summary: Mopidy extension for recording played tracks as listens to Listenbrainz
-Home-page: https://github.com/suaviloquence/mopidy-listenbrainz
-Author: suaviloquence
-Author-email: stein.magnus@jodal.no
-License: Apache License, Version 2.0
-Platform: UNKNOWN
-Classifier: Environment :: No Input/Output (Daemon)
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Multimedia :: Sound/Audio :: Players
-Requires-Python: >=3.7
-Provides-Extra: lint
-Provides-Extra: test
-Provides-Extra: dev
-License-File: LICENSE
-
 *******************
 Mopidy-Listenbrainz
 *******************
 
 .. image:: https://img.shields.io/pypi/v/Mopidy-Listenbrainz
     :target: https://pypi.org/project/Mopidy-Listenbrainz/
     :alt: Latest PyPI version
@@ -66,25 +41,25 @@
 
 The following configuration values are available:
 
 - ``listenbrainz/enabled``: If the extension should be enabled or not.
   Defaults to enabled.
 - ``listenbrainz/token``: Your `Listenbrainz user token <https://listenbrainz.org/profile/>`_
 - ``listenbrainz/url``: The URL of the API of the Listenbrainz instance to record listens to (default: api.listenbrainz.org)
-
+- ``listenbrainz/import_playlists``: Whether to import Listenbrainz playlists (default: ``false``)
+- ``listenbrainz/search_schemes``: If non empty, the search for tracks in Mopidy's library is limited to results with the given schemes. The default value is ``"local:"`` to search tracks in Mopidy-Local library. It's recommended to customize the value according to your favorite backend but beware that not all backends support the required track search by ``musicbrainz_trackid`` (Mopidy-File, Mopidy-InternetArchive, Mopidy-Podcast, Mopidy-Somafm, Mopidy-Stream don't support such searches).
 
 Project resources
 =================
 
 - `Source code <https://github.com/suaviloquence/mopidy-listenbrainz>`_
 - `Issue tracker <https://github.com/suaviloquence/mopidy-listenbrainz/issues>`_
 - `Changelog <https://github.com/suaviloquence/mopidy-listenbrainz/releases>`_
 
 
 Credits
 =======
 
 - Fork of `Mopidy-Scrobbler <https://github.com/mopidy/mopidy-scrobbler>`__ by `Stein Magnus Jodal <https://github.com/jodal>`__
 - Current maintainer: `suaviloquence <https://github.com/suaviloquence>`__
+- Playlist support by `Matthias Meulien <https://github.com/orontee>`__
 - `Contributors <https://github.com/suaviloquence/mopidy-listenbrainz/graphs/contributors>`_
-
-
```

### Comparing `Mopidy-Listenbrainz-0.1.0/Mopidy_Listenbrainz.egg-info/SOURCES.txt` & `mopidy_listenbrainz-0.2.0/Mopidy_Listenbrainz.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -11,13 +11,15 @@
 Mopidy_Listenbrainz.egg-info/SOURCES.txt
 Mopidy_Listenbrainz.egg-info/dependency_links.txt
 Mopidy_Listenbrainz.egg-info/entry_points.txt
 Mopidy_Listenbrainz.egg-info/not-zip-safe
 Mopidy_Listenbrainz.egg-info/requires.txt
 Mopidy_Listenbrainz.egg-info/top_level.txt
 mopidy_listenbrainz/__init__.py
+mopidy_listenbrainz/backend.py
 mopidy_listenbrainz/ext.conf
 mopidy_listenbrainz/frontend.py
 mopidy_listenbrainz/listenbrainz.py
+mopidy_listenbrainz/playlists.py
 tests/__init__.py
 tests/test_extension.py
 tests/test_frontend.py
```

### Comparing `Mopidy-Listenbrainz-0.1.0/mopidy_listenbrainz/__init__.py` & `mopidy_listenbrainz-0.2.0/mopidy_listenbrainz/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,13 +15,19 @@
     def get_default_config(self):
         return config.read(pathlib.Path(__file__).parent / "ext.conf")
 
     def get_config_schema(self):
         schema = super().get_config_schema()
         schema["token"] = config.Secret()
         schema["url"] = config.String()
+        schema["import_playlists"] = config.Boolean()
+        schema["search_schemes"] = config.List(optional=True)
         return schema
 
     def setup(self, registry):
         from .frontend import ListenbrainzFrontend
 
         registry.add("frontend", ListenbrainzFrontend)
+
+        from .backend import ListenbrainzBackend
+
+        registry.add("backend", ListenbrainzBackend)
```

### Comparing `Mopidy-Listenbrainz-0.1.0/setup.cfg` & `mopidy_listenbrainz-0.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,49 @@
 [metadata]
 name = Mopidy-Listenbrainz
-version = 0.1.0
+version = 0.2.0
 url = https://github.com/suaviloquence/mopidy-listenbrainz
 author = suaviloquence
-author_email = stein.magnus@jodal.no
+author_email = m@mcarr.one
 license = Apache License, Version 2.0
 license_file = LICENSE
 description = Mopidy extension for recording played tracks as listens to Listenbrainz
 long_description = file: README.rst
 classifiers = 
 	Environment :: No Input/Output (Daemon)
 	Intended Audience :: End Users/Desktop
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Multimedia :: Sound/Audio :: Players
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 python_requires = >= 3.7
 install_requires = 
 	Mopidy >= 3.0.0
 	Pykka >= 2.0.1
 	setuptools
-	pylast >= 2.2.0
 
 [options.extras_require]
 lint = 
 	black
 	check-manifest
 	flake8
 	flake8-black
 	flake8-bugbear
 	flake8-import-order
-	isort[pyproject]
-test = 
-	pytest
-	pytest-cov
-dev = 
-	%(lint)s
-	%(test)s
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
 
 [options.entry_points]
```

### Comparing `Mopidy-Listenbrainz-0.1.0/tests/test_extension.py` & `mopidy_listenbrainz-0.2.0/tests/test_extension.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 from unittest import mock
 
 from mopidy_listenbrainz import Extension
-from mopidy_listenbrainz import frontend as frontend_lib
+from mopidy_listenbrainz import frontend as frontend_lib, backend as backend_lib
 
 
 def test_get_default_config():
     ext = Extension()
 
     config = ext.get_default_config()
 
     assert "[listenbrainz]" in config
     assert "enabled = true" in config
     assert "token =" in config
     assert "url =" in config
+    assert "import_playlists = false" in config
+    assert "search_schemes = local:" in config
 
 
 def test_get_config_schema():
     ext = Extension()
 
     schema = ext.get_config_schema()
 
     assert "token" in schema
     assert "url" in schema
+    assert "import_playlists" in schema
+    assert "search_schemes" in schema
 
 
 def test_setup():
     ext = Extension()
     registry = mock.Mock()
 
     ext.setup(registry)
 
-    registry.add.assert_called_once_with(
-        "frontend", frontend_lib.ListenbrainzFrontend
+    registry.add.assert_any_call(
+        "frontend",
+        frontend_lib.ListenbrainzFrontend,
+    )
+
+    registry.add.assert_any_call(
+        "backend",
+        backend_lib.ListenbrainzBackend,
     )
```

