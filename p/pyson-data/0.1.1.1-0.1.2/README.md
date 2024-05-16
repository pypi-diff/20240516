# Comparing `tmp/pyson_data-0.1.1.1.tar.gz` & `tmp/pyson_data-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "pyson_data-0.1.2.tar", last modified: Mon May  6 17:12:05 2024, max compression
```

## Comparing `pyson_data-0.1.1.1.tar` & `pyson_data-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/src/pyson_data/__init__.py
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/src/pyson_data/pyson.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/tests/example.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/tests/example.pyson
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/.gitignore
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/LICENSE
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/README.md
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 pyson_data-0.1.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:12:05.321302 pyson_data-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-06 17:11:58.000000 pyson_data-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-06 17:12:05.321302 pyson_data-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-06 17:11:58.000000 pyson_data-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-06 17:11:58.000000 pyson_data-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:12:05.321302 pyson_data-0.1.2/pyson_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-06 17:12:05.000000 pyson_data-0.1.2/pyson_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-06 17:12:05.000000 pyson_data-0.1.2/pyson_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:12:05.000000 pyson_data-0.1.2/pyson_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:12:05.000000 pyson_data-0.1.2/pyson_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 17:12:05.321302 pyson_data-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-06 17:11:58.000000 pyson_data-0.1.2/setup.py
```

### Comparing `pyson_data-0.1.1.1/LICENSE` & `pyson_data-0.1.2/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2018 ComputingSquid, OmegaGodzilla66, CoolSchnoodle, Josh-co-dev
+Copyright (c) 2024 ComputingSquid, OmegaGodzilla66, CoolSchnoodle, nmd102, Josh-co-dev
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyson_data-0.1.1.1/README.md` & `pyson_data-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # PYSON #
-##### Maintained by: [OmegaGodzilla66](https://github.com/OmegaGodzilla66), [ComputingSquid](https://github.com/ProbablyComputingSquid), and [CoolSchnoodle](https://github.com/coolSchnoodle) #####
+##### Maintained by: [OmegaGodzilla66](https://github.com/OmegaGodzilla66), [ComputingSquid](https://github.com/ProbablyComputingSquid), [CoolSchnoodle](https://github.com/coolSchnoodle), and [nmd102](https://github.com/nmd102) #####
 
 
 ## Overview ##
 The purpose of this project is to provide a python-based alternative to JSON. This is a (almost) fully functional JSON-inspired data management system!
 
 ## How to Use ##
 **THIS PROJECT IS NOT YET FINISHED! DOCUMENTATION IS ONLY SHOWN FOR COMPLETED FEATURES. SOME FEATURES MAY BREAK DUE TO CONTINUED DEVELOPMENT. IF YOU SEE A PROBLEM, PLEASE LET ME KNOW!**
 <br>Believe it or not, this project is surprisingly easy to use.<br>
 <br> The only thing you have to do is `pip install pyson-data` ! From then, you can just `import pyson_data as pyson`, and use functions as normal!
 Support for other languages may come soon.<br>
 
 ## quickstart ## 
-TODO: write later
+Refer to the project wiki [here](https://github.com/OmegaGodzilla66/PYSON/wiki)
 
 ## documentation ##
-Documentation has been moved to the project wiki [here](https://github.com/OmegaGodzilla66/PYSON/wiki) to decrease clutter in the README.
+Documentation has also been moved to the project wiki [here](https://github.com/OmegaGodzilla66/PYSON/wiki) to decrease clutter in the README.
 
 ## Supported Types ##
 There are 4 supported types: int, float, str, and list
 <br><br>
 - An int is a whole number that can be any value<br>
 - A str is a list of text (quotes not required)<br>
 - A list is a list of values, which currently have to all be strings. List items are seperated by the (*) seperator.
 Currently there is no escaping support. I don't really know why you would use that value normally in a list. <br> 
 - A float is a decimal number, that can be any value<br>
 
 More supported types may be added. 
 
 ## Changelog ##
+- v0.1.2: Refactored pyson.py
 - v0.1.1: Added writeMultiple function, various bug fixes
 - v0.1.0-alpha: package & release deployed to pypi, merged code to main, and resolved all merge conflicts! truly a cause for celebration 🎉
 - v0.0.9: coolSchnoodle and nmd102 made code fixes and README fixes
 - v0.0.8: Added updateData function
 - v0.0.7: Fixed errors, refactored bad code
 - v0.0.6: Added floats
 - v0.0.5: Updated naming system, ported to github!
```

### Comparing `pyson_data-0.1.1.1/pyproject.toml` & `pyson_data-0.1.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyson_data"
-version = "0.1.1.1"
+version = "0.1.2"
 authors = [
   { name="josh-co", email="omegaraspberrypi@gmail.com" },
 ]
 description = "Pyson package for .pyson data format support"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -14,11 +14,11 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/ProbablyComputingSquid/PYSON/"
 Issues = "https://github.com/ProbablyComputingSquid/PYSON/issues"
 
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
 [tool.hatch.build.targets.wheel]
 packages = ["src/pyson_data"]
```

### Comparing `pyson_data-0.1.1.1/PKG-INFO` & `pyson_data-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,55 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: pyson_data
-Version: 0.1.1.1
+Version: 0.1.2
 Summary: Pyson package for .pyson data format support
+Home-page: https://github.com/OmegaGodzilla66/PYSON
+Author: josh-co-dev
+Author-email: josh-co <omegaraspberrypi@gmail.com>
 Project-URL: Homepage, https://github.com/ProbablyComputingSquid/PYSON/
 Project-URL: Issues, https://github.com/ProbablyComputingSquid/PYSON/issues
-Author-email: josh-co <omegaraspberrypi@gmail.com>
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # PYSON #
-##### Maintained by: [OmegaGodzilla66](https://github.com/OmegaGodzilla66), [ComputingSquid](https://github.com/ProbablyComputingSquid), and [CoolSchnoodle](https://github.com/coolSchnoodle) #####
+##### Maintained by: [OmegaGodzilla66](https://github.com/OmegaGodzilla66), [ComputingSquid](https://github.com/ProbablyComputingSquid), [CoolSchnoodle](https://github.com/coolSchnoodle), and [nmd102](https://github.com/nmd102) #####
 
 
 ## Overview ##
 The purpose of this project is to provide a python-based alternative to JSON. This is a (almost) fully functional JSON-inspired data management system!
 
 ## How to Use ##
 **THIS PROJECT IS NOT YET FINISHED! DOCUMENTATION IS ONLY SHOWN FOR COMPLETED FEATURES. SOME FEATURES MAY BREAK DUE TO CONTINUED DEVELOPMENT. IF YOU SEE A PROBLEM, PLEASE LET ME KNOW!**
 <br>Believe it or not, this project is surprisingly easy to use.<br>
 <br> The only thing you have to do is `pip install pyson-data` ! From then, you can just `import pyson_data as pyson`, and use functions as normal!
 Support for other languages may come soon.<br>
 
 ## quickstart ## 
-TODO: write later
+Refer to the project wiki [here](https://github.com/OmegaGodzilla66/PYSON/wiki)
 
 ## documentation ##
-Documentation has been moved to the project wiki [here](https://github.com/OmegaGodzilla66/PYSON/wiki) to decrease clutter in the README.
+Documentation has also been moved to the project wiki [here](https://github.com/OmegaGodzilla66/PYSON/wiki) to decrease clutter in the README.
 
 ## Supported Types ##
 There are 4 supported types: int, float, str, and list
 <br><br>
 - An int is a whole number that can be any value<br>
 - A str is a list of text (quotes not required)<br>
 - A list is a list of values, which currently have to all be strings. List items are seperated by the (*) seperator.
 Currently there is no escaping support. I don't really know why you would use that value normally in a list. <br> 
 - A float is a decimal number, that can be any value<br>
 
 More supported types may be added. 
 
 ## Changelog ##
+- v0.1.2: Refactored pyson.py
 - v0.1.1: Added writeMultiple function, various bug fixes
 - v0.1.0-alpha: package & release deployed to pypi, merged code to main, and resolved all merge conflicts! truly a cause for celebration 🎉
 - v0.0.9: coolSchnoodle and nmd102 made code fixes and README fixes
 - v0.0.8: Added updateData function
 - v0.0.7: Fixed errors, refactored bad code
 - v0.0.6: Added floats
 - v0.0.5: Updated naming system, ported to github!
```

