# Comparing `tmp/InputPowertools-1.0.1.tar.gz` & `tmp/inputpowertools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InputPowertools-1.0.1.tar", last modified: Sun Mar 20 16:55:32 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `InputPowertools-1.0.1.tar` & `inputpowertools-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-20 16:55:32.269028 InputPowertools-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     4507 2022-03-20 16:55:32.269028 InputPowertools-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3646 2022-03-20 16:55:14.000000 InputPowertools-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-20 16:55:32.269028 InputPowertools-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-03-20 16:55:14.000000 InputPowertools-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-20 16:55:32.269028 InputPowertools-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-20 16:55:32.269028 InputPowertools-1.0.1/src/InputPowertools/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-03-20 16:55:14.000000 InputPowertools-1.0.1/src/InputPowertools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5088 2022-03-20 16:55:14.000000 InputPowertools-1.0.1/src/InputPowertools/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    10696 2022-03-20 16:55:14.000000 InputPowertools-1.0.1/src/InputPowertools/input.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-20 16:55:32.269028 InputPowertools-1.0.1/src/InputPowertools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4507 2022-03-20 16:55:31.000000 InputPowertools-1.0.1/src/InputPowertools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-03-20 16:55:32.000000 InputPowertools-1.0.1/src/InputPowertools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-20 16:55:31.000000 InputPowertools-1.0.1/src/InputPowertools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-03-20 16:55:32.000000 InputPowertools-1.0.1/src/InputPowertools.egg-info/top_level.txt
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/.ignore
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/Pipfile
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/.idea/InputPowertools.iml
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/.idea/git_toolbox_prj.xml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    10292 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/examples/example 1.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/examples/example 2.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/src/InputPowertools/__init__.py
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/src/InputPowertools/cli.py
+-rw-r--r--   0        0        0    10696 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/src/InputPowertools/input.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/.gitignore
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/README.md
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 inputpowertools-1.0.2/PKG-INFO
```

### Comparing `InputPowertools-1.0.1/PKG-INFO` & `inputpowertools-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: InputPowertools
-Version: 1.0.1
+Version: 1.0.2
 Summary: Kind of like a non intrusive addon for the standard input()
-Home-page: https://github.com/MAA28/InputPowertools
+Project-URL: Homepage, https://github.com/MAA28/InputPowertools
+Project-URL: Issues, https://github.com/MAA28/InputPowertools/issues
 Author: MAA28
-Author-email: malteaschenbach@gmail.com
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/MAA28/InputPowertools/issues
-Project-URL: Source, https://github.com/MAA28/InputPowertools/
 Keywords: cli,command line
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6, <4
+Classifier: Topic :: Software Development :: User Interfaces
+Requires-Python: >=3.8
+Requires-Dist: colorama
+Requires-Dist: docstring-parser
+Requires-Dist: typical
+Requires-Dist: typing
 Description-Content-Type: text/markdown
 
 # InputPowertools
 > Eliminate the annoyances of getting input or building a cli in python!
 ## Prolog
 I love using **c**ommand **l**ine **i**nterfaces and I think most people like building these small tools as well, but its really annoying to have to build the interface between the user and your program, hence I build this python package to take care of this part for you.
 ## Installation
@@ -136,9 +136,7 @@
 ```
 ### Analysing the function parameters to generate cli
 ```
 $ python examples/example\ 1.py  --a lol --b "this is a value with spaces" --c 4 2 "test123" --d
 
 a='lol' b='this is a value with spaces' c=[4, 2, 'test123'] d=True
 ```
-
-
```

### Comparing `InputPowertools-1.0.1/README.md` & `inputpowertools-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `InputPowertools-1.0.1/src/InputPowertools/cli.py` & `inputpowertools-1.0.2/src/InputPowertools/cli.py`

 * *Files identical despite different names*

### Comparing `InputPowertools-1.0.1/src/InputPowertools/input.py` & `inputpowertools-1.0.2/src/InputPowertools/input.py`

 * *Files identical despite different names*

