# Comparing `tmp/kicad_parts_placer-0.1.2.tar.gz` & `tmp/kicad_parts_placer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kicad_parts_placer-0.1.2.tar", last modified: Tue Dec 19 02:24:44 2023, max compression
+gzip compressed data, was "kicad_parts_placer-0.1.3.tar", last modified: Tue Dec 19 02:25:54 2023, max compression
```

## Comparing `kicad_parts_placer-0.1.2.tar` & `kicad_parts_placer-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-12-19 02:24:44.201830 kicad_parts_placer-0.1.2/
--rw-rw-r--   0 simon     (1000) simon     (1000)     3653 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.2/CONTRIBUTING.rst
--rw-rw-r--   0 simon     (1000) simon     (1000)       89 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.2/HISTORY.rst
--rw-rw-r--   0 simon     (1000) simon     (1000)     1070 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.2/LICENSE
--rw-rw-r--   0 simon     (1000) simon     (1000)      241 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.2/MANIFEST.in
--rw-rw-r--   0 simon     (1000) simon     (1000)     4810 2023-12-19 02:24:44.201830 kicad_parts_placer-0.1.2/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)     3975 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.2/README.md
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-12-19 02:24:44.201830 kicad_parts_placer-0.1.2/docs/
--rw-rw-r--   0 simon     (1000) simon     (1000)      619 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.2/docs/Makefile
--rwxrwxr-x   0 simon     (1000) simon     (1000)     4918 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.2/docs/conf.py
--rw-rw-r--   0 simon     (1000) simon     (1000)       33 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.2/docs/contributing.rst
--rw-rw-r--   0 simon     (1000) simon     (1000)       28 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.2/docs/history.rst
--rw-rw-r--   0 simon     (1000) simon     (1000)      304 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.2/docs/index.rst
--rw-rw-r--   0 simon     (1000) simon     (1000)     1198 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.2/docs/installation.rst
--rw-rw-r--   0 simon     (1000) simon     (1000)      816 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.2/docs/make.bat
--rw-rw-r--   0 simon     (1000) simon     (1000)       91 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.2/docs/usage.rst
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-12-19 02:24:44.201830 kicad_parts_placer-0.1.2/kicad_parts_placer/
--rw-rw-r--   0 simon     (1000) simon     (1000)      147 2023-12-19 02:14:25.000000 kicad_parts_placer-0.1.2/kicad_parts_placer/__init__.py
--rwxrwxr-x   0 simon     (1000) simon     (1000)     3200 2023-12-19 02:20:27.000000 kicad_parts_placer-0.1.2/kicad_parts_placer/cli.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     3731 2023-12-19 02:22:49.000000 kicad_parts_placer-0.1.2/kicad_parts_placer/kicad_parts_placer.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-12-19 02:24:44.201830 kicad_parts_placer-0.1.2/kicad_parts_placer.egg-info/
--rw-rw-r--   0 simon     (1000) simon     (1000)     4810 2023-12-19 02:24:44.000000 kicad_parts_placer-0.1.2/kicad_parts_placer.egg-info/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)      653 2023-12-19 02:24:44.000000 kicad_parts_placer-0.1.2/kicad_parts_placer.egg-info/SOURCES.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-12-19 02:24:44.000000 kicad_parts_placer-0.1.2/kicad_parts_placer.egg-info/dependency_links.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       68 2023-12-19 02:24:44.000000 kicad_parts_placer-0.1.2/kicad_parts_placer.egg-info/entry_points.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-12-19 02:24:44.000000 kicad_parts_placer-0.1.2/kicad_parts_placer.egg-info/not-zip-safe
--rw-rw-r--   0 simon     (1000) simon     (1000)       52 2023-12-19 02:24:44.000000 kicad_parts_placer-0.1.2/kicad_parts_placer.egg-info/requires.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       19 2023-12-19 02:24:44.000000 kicad_parts_placer-0.1.2/kicad_parts_placer.egg-info/top_level.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)      390 2023-12-19 02:24:44.201830 kicad_parts_placer-0.1.2/setup.cfg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1530 2023-12-19 02:14:25.000000 kicad_parts_placer-0.1.2/setup.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-12-19 02:24:44.201830 kicad_parts_placer-0.1.2/tests/
--rw-rw-r--   0 simon     (1000) simon     (1000)       48 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.2/tests/__init__.py
--rw-rw-r--   0 simon     (1000) simon     (1000)      929 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.2/tests/test_kicad_parts_placer.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-12-19 02:25:54.910416 kicad_parts_placer-0.1.3/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3653 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.3/CONTRIBUTING.rst
+-rw-rw-r--   0 simon     (1000) simon     (1000)       89 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.3/HISTORY.rst
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1070 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.3/LICENSE
+-rw-rw-r--   0 simon     (1000) simon     (1000)      241 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.3/MANIFEST.in
+-rw-rw-r--   0 simon     (1000) simon     (1000)     4811 2023-12-19 02:25:54.910416 kicad_parts_placer-0.1.3/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3975 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.3/README.md
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-12-19 02:25:54.910416 kicad_parts_placer-0.1.3/docs/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      619 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.3/docs/Makefile
+-rwxrwxr-x   0 simon     (1000) simon     (1000)     4918 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.3/docs/conf.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)       33 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.3/docs/contributing.rst
+-rw-rw-r--   0 simon     (1000) simon     (1000)       28 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.3/docs/history.rst
+-rw-rw-r--   0 simon     (1000) simon     (1000)      304 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.3/docs/index.rst
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1198 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.3/docs/installation.rst
+-rw-rw-r--   0 simon     (1000) simon     (1000)      816 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.3/docs/make.bat
+-rw-rw-r--   0 simon     (1000) simon     (1000)       91 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.3/docs/usage.rst
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-12-19 02:25:54.910416 kicad_parts_placer-0.1.3/kicad_parts_placer/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      147 2023-12-19 02:25:51.000000 kicad_parts_placer-0.1.3/kicad_parts_placer/__init__.py
+-rwxrwxr-x   0 simon     (1000) simon     (1000)     3200 2023-12-19 02:20:27.000000 kicad_parts_placer-0.1.3/kicad_parts_placer/cli.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3731 2023-12-19 02:22:49.000000 kicad_parts_placer-0.1.3/kicad_parts_placer/kicad_parts_placer.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-12-19 02:25:54.910416 kicad_parts_placer-0.1.3/kicad_parts_placer.egg-info/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     4811 2023-12-19 02:25:54.000000 kicad_parts_placer-0.1.3/kicad_parts_placer.egg-info/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)      653 2023-12-19 02:25:54.000000 kicad_parts_placer-0.1.3/kicad_parts_placer.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-12-19 02:25:54.000000 kicad_parts_placer-0.1.3/kicad_parts_placer.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       68 2023-12-19 02:25:54.000000 kicad_parts_placer-0.1.3/kicad_parts_placer.egg-info/entry_points.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-12-19 02:25:54.000000 kicad_parts_placer-0.1.3/kicad_parts_placer.egg-info/not-zip-safe
+-rw-rw-r--   0 simon     (1000) simon     (1000)       52 2023-12-19 02:25:54.000000 kicad_parts_placer-0.1.3/kicad_parts_placer.egg-info/requires.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       19 2023-12-19 02:25:54.000000 kicad_parts_placer-0.1.3/kicad_parts_placer.egg-info/top_level.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)      390 2023-12-19 02:25:54.914415 kicad_parts_placer-0.1.3/setup.cfg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1531 2023-12-19 02:25:51.000000 kicad_parts_placer-0.1.3/setup.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-12-19 02:25:54.910416 kicad_parts_placer-0.1.3/tests/
+-rw-rw-r--   0 simon     (1000) simon     (1000)       48 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.3/tests/__init__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)      929 2023-12-19 01:37:37.000000 kicad_parts_placer-0.1.3/tests/test_kicad_parts_placer.py
```

### Comparing `kicad_parts_placer-0.1.2/CONTRIBUTING.rst` & `kicad_parts_placer-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `kicad_parts_placer-0.1.2/LICENSE` & `kicad_parts_placer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kicad_parts_placer-0.1.2/PKG-INFO` & `kicad_parts_placer-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kicad_parts_placer
-Version: 0.1.2
-Summary: Place components in a kicad file programatically.
+Version: 0.1.3
+Summary: Place components in a kicad file programmatically.
 Home-page: https://github.com/snhobbs/kicad-parts-placer.git
 Author: Simon Hobbs
 Author-email: simon.hobbs@electrooptical.net
 License: MIT license
 Keywords: kicad_parts_placer
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `kicad_parts_placer-0.1.2/README.md` & `kicad_parts_placer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kicad_parts_placer-0.1.2/docs/Makefile` & `kicad_parts_placer-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kicad_parts_placer-0.1.2/docs/conf.py` & `kicad_parts_placer-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kicad_parts_placer-0.1.2/docs/installation.rst` & `kicad_parts_placer-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `kicad_parts_placer-0.1.2/docs/make.bat` & `kicad_parts_placer-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kicad_parts_placer-0.1.2/kicad_parts_placer/cli.py` & `kicad_parts_placer-0.1.3/kicad_parts_placer/cli.py`

 * *Files identical despite different names*

### Comparing `kicad_parts_placer-0.1.2/kicad_parts_placer/kicad_parts_placer.py` & `kicad_parts_placer-0.1.3/kicad_parts_placer/kicad_parts_placer.py`

 * *Files identical despite different names*

### Comparing `kicad_parts_placer-0.1.2/kicad_parts_placer.egg-info/PKG-INFO` & `kicad_parts_placer-0.1.3/kicad_parts_placer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kicad-parts-placer
-Version: 0.1.2
-Summary: Place components in a kicad file programatically.
+Version: 0.1.3
+Summary: Place components in a kicad file programmatically.
 Home-page: https://github.com/snhobbs/kicad-parts-placer.git
 Author: Simon Hobbs
 Author-email: simon.hobbs@electrooptical.net
 License: MIT license
 Keywords: kicad_parts_placer
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `kicad_parts_placer-0.1.2/kicad_parts_placer.egg-info/SOURCES.txt` & `kicad_parts_placer-0.1.3/kicad_parts_placer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kicad_parts_placer-0.1.2/setup.py` & `kicad_parts_placer-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
-    description="Place components in a kicad file programatically.",
+    description="Place components in a kicad file programmatically.",
     entry_points={
         'console_scripts': [
             'kicad_parts_placer=kicad_parts_placer.cli:main',
         ],
     },
     install_requires=requirements,
     license="MIT license",
@@ -45,10 +45,10 @@
     include_package_data=True,
     keywords='kicad_parts_placer',
     name='kicad_parts_placer',
     packages=find_packages(include=['kicad_parts_placer', 'kicad_parts_placer.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/snhobbs/kicad-parts-placer.git',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

### Comparing `kicad_parts_placer-0.1.2/tests/test_kicad_parts_placer.py` & `kicad_parts_placer-0.1.3/tests/test_kicad_parts_placer.py`

 * *Files identical despite different names*

