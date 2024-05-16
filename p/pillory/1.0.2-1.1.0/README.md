# Comparing `tmp/pillory-1.0.2.tar.gz` & `tmp/pillory-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillory-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pillory-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pillory-1.0.2.tar` & `pillory-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,17 @@
--rw-r--r--   0        0        0      797 2024-04-11 23:14:04.031983 pillory-1.0.2/.circleci/config.yml
--rw-r--r--   0        0        0       18 2024-04-11 23:14:04.031983 pillory-1.0.2/.gitignore
--rw-r--r--   0        0        0      359 2024-04-11 23:14:04.031983 pillory-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     9161 2024-04-11 23:14:04.031983 pillory-1.0.2/LICENSE
--rw-r--r--   0        0        0     4361 2024-04-11 23:14:04.031983 pillory-1.0.2/README.md
--rw-r--r--   0        0        0     1321 2024-04-11 23:14:04.031983 pillory-1.0.2/dev-requirements.txt
--rwxr-xr-x   0        0        0     3188 2024-04-11 23:14:04.031983 pillory-1.0.2/pillory.py
--rw-r--r--   0        0        0      587 2024-04-11 23:14:04.031983 pillory-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3082 2024-04-11 23:14:04.031983 pillory-1.0.2/test_example.py
--rw-r--r--   0        0        0      513 2024-04-11 23:14:04.031983 pillory-1.0.2/test_pillory.py
--rw-r--r--   0        0        0     4898 1970-01-01 00:00:00.000000 pillory-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      797 2024-05-16 16:02:52.985870 pillory-1.1.0/.circleci/config.yml
+-rw-r--r--   0        0        0       50 2024-05-16 16:02:52.985870 pillory-1.1.0/.gitignore
+-rw-r--r--   0        0        0      359 2024-05-16 16:02:52.985870 pillory-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9161 2024-05-16 16:02:52.985870 pillory-1.1.0/LICENSE
+-rw-r--r--   0        0        0      354 2024-05-16 16:02:52.985870 pillory-1.1.0/Makefile
+-rw-r--r--   0        0        0     4793 2024-05-16 16:02:52.985870 pillory-1.1.0/README.md
+-rw-r--r--   0        0        0     1372 2024-05-16 16:02:52.985870 pillory-1.1.0/dev-requirements.txt
+-rw-r--r--   0        0        0       41 2024-05-16 16:02:52.985870 pillory-1.1.0/example/__init__.py
+-rw-r--r--   0        0        0      311 2024-05-16 16:02:52.985870 pillory-1.1.0/example/definition.py
+-rw-r--r--   0        0        0      180 2024-05-16 16:02:52.985870 pillory-1.1.0/example/empty/README.txt
+-rw-r--r--   0        0        0      649 2024-05-16 16:02:52.985870 pillory-1.1.0/example/test_use.py
+-rw-r--r--   0        0        0      222 2024-05-16 16:02:52.985870 pillory-1.1.0/example/use.py
+-rwxr-xr-x   0        0        0     8572 2024-05-16 16:02:52.985870 pillory-1.1.0/pillory.py
+-rw-r--r--   0        0        0     1093 2024-05-16 16:02:52.985870 pillory-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1245 2024-05-16 16:02:52.985870 pillory-1.1.0/test_example.py
+-rw-r--r--   0        0        0     2599 2024-05-16 16:02:52.985870 pillory-1.1.0/test_pillory.py
+-rw-r--r--   0        0        0     5376 1970-01-01 00:00:00.000000 pillory-1.1.0/PKG-INFO
```

### Comparing `pillory-1.0.2/.circleci/config.yml` & `pillory-1.1.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `pillory-1.0.2/LICENSE` & `pillory-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pillory-1.0.2/README.md` & `pillory-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -62,16 +62,14 @@
 * No --help text.
 * No console script entry point (pillory command), have to use with python -m.
 * Only takes one path or glob.
 * Only tested with Python 3.10.
 * No config file support.
 * No comments to ignore rules.
 * Not fast.
-* Must import modules. Doesn't work well with frameworks like Django that
-  require special setup for things like settings before importing.
 * Globs have to be relative to the current directory.
 * No further explanations for the errors.
 * No pretty error handling, just tracebacks.
 * Will error when mocking something in the module under test, which is arguably
   "OK".
 * No pre-commit integration.
 
@@ -120,7 +118,25 @@
 The example tests have a more complicated setup to include the file system and
 command line args. Try to limit the number of example tests. The tests use
 doctest to easily check the outputs. You can run them with:
 
 ```
 python test_example.py -v
 ```
+
+To run all the different tests and see the coverage given you can use:
+
+```
+make
+```
+
+The default make target is the coverage report in HTML format. You can look at
+the file in a browser, or if you don’t want to leave the terminal but still want
+a line by line coverage report, you can use [browsh][browsh] as your browser.
+You can run the tests, start a HTTP server, and view the report in browsh with
+this oneliner:
+
+```
+( make && cd build/htmlcov && python -m http.server 8081 &>/dev/null & browsh http://localhost:8081 ; kill $! )
+```
+
+[browsh]: https://www.brow.sh
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pillory-1.0.2/dev-requirements.txt` & `pillory-1.1.0/dev-requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     # via requests
 cfgv==3.4.0
     # via pre-commit
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via pip-tools
+coverage==7.5.1
+    # via pillory (pyproject.toml)
 distlib==0.3.8
     # via virtualenv
 docutils==0.20.1
     # via flit
 filelock==3.13.3
     # via virtualenv
 flit==3.9.0
```

### Comparing `pillory-1.0.2/PKG-INFO` & `pillory-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pillory
-Version: 1.0.2
+Version: 1.1.0
 Summary: A linter to scrutinize how you are using mocks in Python.
 Author-email: Fergal Armstrong <patio.algebra0i@icloud.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
+Requires-Dist: coverage~=7.5 ; extra == "dev"
 Requires-Dist: flit~=3.9 ; extra == "dev"
 Requires-Dist: pip-tools~=7.4 ; extra == "dev"
 Requires-Dist: pre-commit~=3.7 ; extra == "dev"
 Requires-Dist: ruff~=0.3 ; extra == "dev"
 Project-URL: Home, https://github.com/fffergal/pillory
 Provides-Extra: dev
 
@@ -76,16 +77,14 @@
 * No --help text.
 * No console script entry point (pillory command), have to use with python -m.
 * Only takes one path or glob.
 * Only tested with Python 3.10.
 * No config file support.
 * No comments to ignore rules.
 * Not fast.
-* Must import modules. Doesn't work well with frameworks like Django that
-  require special setup for things like settings before importing.
 * Globs have to be relative to the current directory.
 * No further explanations for the errors.
 * No pretty error handling, just tracebacks.
 * Will error when mocking something in the module under test, which is arguably
   "OK".
 * No pre-commit integration.
 
@@ -135,7 +134,25 @@
 command line args. Try to limit the number of example tests. The tests use
 doctest to easily check the outputs. You can run them with:
 
 ```
 python test_example.py -v
 ```
 
+To run all the different tests and see the coverage given you can use:
+
+```
+make
+```
+
+The default make target is the coverage report in HTML format. You can look at
+the file in a browser, or if you don’t want to leave the terminal but still want
+a line by line coverage report, you can use [browsh][browsh] as your browser.
+You can run the tests, start a HTTP server, and view the report in browsh with
+this oneliner:
+
+```
+( make && cd build/htmlcov && python -m http.server 8081 &>/dev/null & browsh http://localhost:8081 ; kill $! )
+```
+
+[browsh]: https://www.brow.sh
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

