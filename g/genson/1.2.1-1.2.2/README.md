# Comparing `tmp/genson-1.2.1.tar.gz` & `tmp/genson-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/genson-1.2.1.tar", last modified: Fri Apr 24 01:09:25 2020, max compression
+gzip compressed data, was "dist/genson-1.2.2.tar", last modified: Wed Aug 19 17:03:41 2020, max compression
```

## Comparing `genson-1.2.1.tar` & `genson-1.2.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 jrw        (501) staff       (20)        0 2020-04-24 01:09:25.000000 genson-1.2.1/
--rw-r--r--   0 jrw        (501) staff       (20)    32767 2020-04-24 01:09:25.000000 genson-1.2.1/PKG-INFO
--rw-r--r--   0 jrw        (501) staff       (20)     1102 2014-11-16 07:56:30.000000 genson-1.2.1/LICENSE
-drwxr-xr-x   0 jrw        (501) staff       (20)        0 2020-04-24 01:09:25.000000 genson-1.2.1/test/
--rw-r--r--   0 jrw        (501) staff       (20)     2293 2018-01-02 17:11:11.000000 genson-1.2.1/test/test_bin.py
--rw-r--r--   0 jrw        (501) staff       (20)     4018 2018-01-02 00:54:44.000000 genson-1.2.1/test/test_gen_multi.py
--rw-r--r--   0 jrw        (501) staff       (20)     1173 2018-12-03 04:31:49.000000 genson-1.2.1/test/test_misuse.py
--rw-r--r--   0 jrw        (501) staff       (20)        0 2016-06-19 11:34:00.000000 genson-1.2.1/test/__init__.py
--rw-r--r--   0 jrw        (501) staff       (20)     3345 2019-04-09 04:31:19.000000 genson-1.2.1/test/test_add_single.py
--rw-r--r--   0 jrw        (501) staff       (20)     3208 2020-04-24 00:24:39.000000 genson-1.2.1/test/test_builder.py
--rw-r--r--   0 jrw        (501) staff       (20)     4460 2020-04-24 00:43:39.000000 genson-1.2.1/test/test_add_multi.py
--rw-r--r--   0 jrw        (501) staff       (20)     2022 2020-04-17 05:58:55.000000 genson-1.2.1/test/test_custom.py
--rw-r--r--   0 jrw        (501) staff       (20)     6278 2019-04-09 02:50:12.000000 genson-1.2.1/test/test_gen_single.py
--rw-r--r--   0 jrw        (501) staff       (20)     2195 2020-04-17 05:58:55.000000 genson-1.2.1/test/base.py
--rw-r--r--   0 jrw        (501) staff       (20)     2725 2018-01-02 00:54:44.000000 genson-1.2.1/test/test_seed_schema.py
-drwxr-xr-x   0 jrw        (501) staff       (20)        0 2020-04-24 01:09:25.000000 genson-1.2.1/bin/
--rwxr-xr-x   0 jrw        (501) staff       (20)      166 2018-01-02 03:43:09.000000 genson-1.2.1/bin/genson.py
--rwxr-xr-x   0 jrw        (501) staff       (20)      278 2016-06-19 11:34:00.000000 genson-1.2.1/bin/test.py
--rw-r--r--   0 jrw        (501) staff       (20)      115 2014-11-29 10:49:56.000000 genson-1.2.1/MANIFEST.in
--rwxr-xr-x   0 jrw        (501) staff       (20)     2012 2020-04-24 00:33:06.000000 genson-1.2.1/setup.py
-drwxr-xr-x   0 jrw        (501) staff       (20)        0 2020-04-24 01:09:25.000000 genson-1.2.1/genson/
--rw-r--r--   0 jrw        (501) staff       (20)      325 2020-04-17 05:58:55.000000 genson-1.2.1/genson/__init__.py
-drwxr-xr-x   0 jrw        (501) staff       (20)        0 2020-04-24 01:09:25.000000 genson-1.2.1/genson/schema/
-drwxr-xr-x   0 jrw        (501) staff       (20)        0 2020-04-24 01:09:25.000000 genson-1.2.1/genson/schema/strategies/
--rw-r--r--   0 jrw        (501) staff       (20)     3312 2020-04-24 00:24:54.000000 genson-1.2.1/genson/schema/strategies/object.py
--rw-r--r--   0 jrw        (501) staff       (20)     2103 2020-04-17 05:58:55.000000 genson-1.2.1/genson/schema/strategies/scalar.py
--rw-r--r--   0 jrw        (501) staff       (20)      522 2020-04-17 05:58:55.000000 genson-1.2.1/genson/schema/strategies/__init__.py
--rw-r--r--   0 jrw        (501) staff       (20)     2166 2020-04-17 05:58:55.000000 genson-1.2.1/genson/schema/strategies/array.py
--rw-r--r--   0 jrw        (501) staff       (20)     2229 2020-04-24 00:09:44.000000 genson-1.2.1/genson/schema/strategies/base.py
--rw-r--r--   0 jrw        (501) staff       (20)        0 2018-01-02 00:54:44.000000 genson-1.2.1/genson/schema/__init__.py
--rw-r--r--   0 jrw        (501) staff       (20)     5562 2020-04-23 22:38:45.000000 genson-1.2.1/genson/schema/builder.py
--rw-r--r--   0 jrw        (501) staff       (20)     4749 2020-04-23 23:58:16.000000 genson-1.2.1/genson/schema/node.py
--rw-r--r--   0 jrw        (501) staff       (20)     4174 2018-01-02 19:05:51.000000 genson-1.2.1/genson/cli.py
--rw-r--r--   0 jrw        (501) staff       (20)     3575 2020-04-24 00:39:18.000000 genson-1.2.1/HISTORY.rst
--rw-r--r--   0 jrw        (501) staff       (20)      318 2020-04-17 05:58:55.000000 genson-1.2.1/AUTHORS.rst
--rw-r--r--   0 jrw        (501) staff       (20)      128 2020-04-24 01:09:25.000000 genson-1.2.1/setup.cfg
--rw-r--r--   0 jrw        (501) staff       (20)    22062 2020-04-24 01:00:42.000000 genson-1.2.1/README.rst
-drwxr-xr-x   0 jrw        (501) staff       (20)        0 2020-04-24 01:09:25.000000 genson-1.2.1/genson.egg-info/
--rw-r--r--   0 jrw        (501) staff       (20)    32767 2020-04-24 01:09:25.000000 genson-1.2.1/genson.egg-info/PKG-INFO
--rw-r--r--   0 jrw        (501) staff       (20)        1 2016-10-07 02:58:56.000000 genson-1.2.1/genson.egg-info/zip-safe
--rw-r--r--   0 jrw        (501) staff       (20)      784 2020-04-24 01:09:25.000000 genson-1.2.1/genson.egg-info/SOURCES.txt
--rw-r--r--   0 jrw        (501) staff       (20)       44 2020-04-24 01:09:25.000000 genson-1.2.1/genson.egg-info/entry_points.txt
--rw-r--r--   0 jrw        (501) staff       (20)        7 2020-04-24 01:09:25.000000 genson-1.2.1/genson.egg-info/top_level.txt
--rw-r--r--   0 jrw        (501) staff       (20)        1 2020-04-24 01:09:25.000000 genson-1.2.1/genson.egg-info/dependency_links.txt
+drwxr-xr-x   0 jrw        (501) staff       (20)        0 2020-08-19 17:03:41.000000 genson-1.2.2/
+-rw-r--r--   0 jrw        (501) staff       (20)    33577 2020-08-19 17:03:41.000000 genson-1.2.2/PKG-INFO
+-rw-r--r--   0 jrw        (501) staff       (20)     1102 2014-11-16 07:56:30.000000 genson-1.2.2/LICENSE
+drwxr-xr-x   0 jrw        (501) staff       (20)        0 2020-08-19 17:03:41.000000 genson-1.2.2/test/
+-rw-r--r--   0 jrw        (501) staff       (20)     3120 2020-08-19 17:03:32.000000 genson-1.2.2/test/test_bin.py
+-rw-r--r--   0 jrw        (501) staff       (20)     4018 2018-01-02 00:54:44.000000 genson-1.2.2/test/test_gen_multi.py
+-rw-r--r--   0 jrw        (501) staff       (20)     1173 2018-12-03 04:31:49.000000 genson-1.2.2/test/test_misuse.py
+-rw-r--r--   0 jrw        (501) staff       (20)        0 2020-08-18 04:21:28.000000 genson-1.2.2/test/__init__.py
+-rw-r--r--   0 jrw        (501) staff       (20)     3345 2019-04-09 04:31:19.000000 genson-1.2.2/test/test_add_single.py
+-rw-r--r--   0 jrw        (501) staff       (20)     3208 2020-04-24 00:24:39.000000 genson-1.2.2/test/test_builder.py
+-rw-r--r--   0 jrw        (501) staff       (20)     4460 2020-04-24 00:43:39.000000 genson-1.2.2/test/test_add_multi.py
+-rw-r--r--   0 jrw        (501) staff       (20)     2022 2020-04-17 05:58:55.000000 genson-1.2.2/test/test_custom.py
+-rw-r--r--   0 jrw        (501) staff       (20)     6278 2019-04-09 02:50:12.000000 genson-1.2.2/test/test_gen_single.py
+-rw-r--r--   0 jrw        (501) staff       (20)     2195 2020-04-17 05:58:55.000000 genson-1.2.2/test/base.py
+-rw-r--r--   0 jrw        (501) staff       (20)     2725 2020-08-19 17:03:32.000000 genson-1.2.2/test/test_seed_schema.py
+drwxr-xr-x   0 jrw        (501) staff       (20)        0 2020-08-19 17:03:41.000000 genson-1.2.2/bin/
+-rwxr-xr-x   0 jrw        (501) staff       (20)      166 2018-01-02 03:43:09.000000 genson-1.2.2/bin/genson.py
+-rwxr-xr-x   0 jrw        (501) staff       (20)      278 2020-08-19 17:03:32.000000 genson-1.2.2/bin/test.py
+-rw-r--r--   0 jrw        (501) staff       (20)      115 2014-11-29 10:49:56.000000 genson-1.2.2/MANIFEST.in
+-rwxr-xr-x   0 jrw        (501) staff       (20)     2187 2020-08-19 17:03:32.000000 genson-1.2.2/setup.py
+drwxr-xr-x   0 jrw        (501) staff       (20)        0 2020-08-19 17:03:41.000000 genson-1.2.2/genson/
+-rw-r--r--   0 jrw        (501) staff       (20)      367 2020-08-19 17:03:32.000000 genson-1.2.2/genson/__init__.py
+drwxr-xr-x   0 jrw        (501) staff       (20)        0 2020-08-19 17:03:41.000000 genson-1.2.2/genson/schema/
+drwxr-xr-x   0 jrw        (501) staff       (20)        0 2020-08-19 17:03:41.000000 genson-1.2.2/genson/schema/strategies/
+-rw-r--r--   0 jrw        (501) staff       (20)     3312 2020-04-24 00:24:54.000000 genson-1.2.2/genson/schema/strategies/object.py
+-rw-r--r--   0 jrw        (501) staff       (20)     2103 2020-08-18 04:39:58.000000 genson-1.2.2/genson/schema/strategies/scalar.py
+-rw-r--r--   0 jrw        (501) staff       (20)      522 2020-04-17 05:58:55.000000 genson-1.2.2/genson/schema/strategies/__init__.py
+-rw-r--r--   0 jrw        (501) staff       (20)     2166 2020-04-17 05:58:55.000000 genson-1.2.2/genson/schema/strategies/array.py
+-rw-r--r--   0 jrw        (501) staff       (20)     2229 2020-04-24 00:09:44.000000 genson-1.2.2/genson/schema/strategies/base.py
+-rw-r--r--   0 jrw        (501) staff       (20)        0 2018-01-02 00:54:44.000000 genson-1.2.2/genson/schema/__init__.py
+-rw-r--r--   0 jrw        (501) staff       (20)     5562 2020-04-23 22:38:45.000000 genson-1.2.2/genson/schema/builder.py
+-rw-r--r--   0 jrw        (501) staff       (20)     4749 2020-04-23 23:58:16.000000 genson-1.2.2/genson/schema/node.py
+-rw-r--r--   0 jrw        (501) staff       (20)     5818 2020-08-15 22:21:50.000000 genson-1.2.2/genson/cli.py
+-rw-r--r--   0 jrw        (501) staff       (20)     3752 2020-08-15 22:44:05.000000 genson-1.2.2/HISTORY.rst
+-rw-r--r--   0 jrw        (501) staff       (20)      318 2020-04-17 05:58:55.000000 genson-1.2.2/AUTHORS.rst
+-rw-r--r--   0 jrw        (501) staff       (20)      128 2020-08-19 17:03:41.000000 genson-1.2.2/setup.cfg
+-rw-r--r--   0 jrw        (501) staff       (20)    22551 2020-08-19 17:03:32.000000 genson-1.2.2/README.rst
+drwxr-xr-x   0 jrw        (501) staff       (20)        0 2020-08-19 17:03:41.000000 genson-1.2.2/genson.egg-info/
+-rw-r--r--   0 jrw        (501) staff       (20)    33577 2020-08-19 17:03:40.000000 genson-1.2.2/genson.egg-info/PKG-INFO
+-rw-r--r--   0 jrw        (501) staff       (20)        1 2016-10-07 02:58:56.000000 genson-1.2.2/genson.egg-info/zip-safe
+-rw-r--r--   0 jrw        (501) staff       (20)      784 2020-08-19 17:03:40.000000 genson-1.2.2/genson.egg-info/SOURCES.txt
+-rw-r--r--   0 jrw        (501) staff       (20)       44 2020-08-19 17:03:40.000000 genson-1.2.2/genson.egg-info/entry_points.txt
+-rw-r--r--   0 jrw        (501) staff       (20)        7 2020-08-19 17:03:40.000000 genson-1.2.2/genson.egg-info/top_level.txt
+-rw-r--r--   0 jrw        (501) staff       (20)        1 2020-08-19 17:03:40.000000 genson-1.2.2/genson.egg-info/dependency_links.txt
```

### Comparing `genson-1.2.1/PKG-INFO` & `genson-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: genson
-Version: 1.2.1
+Version: 1.2.2
 Summary: GenSON is a powerful, user-friendly JSON Schema generator.
 Home-page: https://github.com/wolverdude/genson/
 Author: Jon Wolverton
 Author-email: wolverton.jr@gmail.com
 License: MIT
 Download-URL: https://github.com/wolverdude/GenSON/tarball/v0.2s.0
 Description: GenSON
@@ -59,44 +59,54 @@
         
         .. code-block:: bash
         
             $ genson --help
         
         .. code-block::
         
-            usage: genson.py [-h] [-d DELIM] [-i SPACES] [-s SCHEMA] [-$ URI] ...
+            usage: genson [-h] [--version] [-d DELIM] [-e ENCODING] [-i SPACES]
+                          [-s SCHEMA] [-$ SCHEMA_URI]
+                          ...
         
             Generate one, unified JSON Schema from one or more JSON objects and/or JSON
-            Schemas. It's compatible with Draft 6 and above.
+            Schemas. Compatible with JSON-Schema Draft 4 and above.
         
             positional arguments:
-              object                files containing JSON objects (defaults to stdin if no
-                                    arguments are passed)
+              object                Files containing JSON objects (defaults to stdin if no
+                                    arguments are passed).
         
             optional arguments:
-              -h, --help            show this help message and exit
+              -h, --help            Show this help message and exit.
+              --version             Show version number and exit.
               -d DELIM, --delimiter DELIM
-                                    set a delimiter - Use this option if the input files
+                                    Set a delimiter. Use this option if the input files
                                     contain multiple JSON objects/schemas. You can pass
                                     any string. A few cases ('newline', 'tab', 'space')
                                     will get converted to a whitespace character. If this
                                     option is omitted, the parser will try to auto-detect
-                                    boundaries
+                                    boundaries.
+              -e ENCODING, --encoding ENCODING
+                                    Use ENCODING instead of the default system encoding
+                                    when reading files. ENCODING must be a valid codec
+                                    name or alias.
               -i SPACES, --indent SPACES
-                                    pretty-print the output, indenting SPACES spaces
+                                    Pretty-print the output, indenting SPACES spaces.
               -s SCHEMA, --schema SCHEMA
-                                    file containing a JSON Schema (can be specified
-                                    multiple times to merge schemas)
-              -$ URI, --schema-uri URI
-                                    the value of the '$schema' keyword (defaults to
+                                    File containing a JSON Schema (can be specified
+                                    multiple times to merge schemas).
+              -$ SCHEMA_URI, --schema-uri SCHEMA_URI
+                                    The value of the '$schema' keyword (defaults to
                                     'http://json-schema.org/schema#' or can be specified
                                     in a schema with the -s option). If 'NULL' is passed,
                                     the "$schema" keyword will not be included in the
                                     result.
         
+        .. note::
+            The ``--encoding`` option is only available in Python 3.
+        
         GenSON Python API
         -----------------
         
         ``SchemaBuilder`` is the basic schema generator class. ``SchemaBuilder`` instances can be loaded up with existing schemas and objects before being serialized.
         
         .. code-block:: python
         
@@ -500,21 +510,23 @@
             >>> picky_builder.add_object(None) # this fails
             genson.schema.node.SchemaGenerationError: Could not find matching schema type for object: None
         
         
         Compatibility
         -------------
         
-        GenSON has been tested and verified using the following versions of Python:
+        GenSON has been tested and verified under the following Python versions:
         
-        * Python 2.7.11
+        * Python 2.7.13
         * Python 3.3.5
-        * Python 3.4.4
-        * Python 3.5.1
+        * Python 3.4.5
+        * Python 3.5.4
         * Python 3.6.2
+        * Python 3.7.3
+        * Python 3.8.2
         
         
         Contributing
         ------------
         
         When contributing, please follow these steps:
         
@@ -573,14 +585,20 @@
         .. _minimum number: https://json-schema.org/understanding-json-schema/reference/numeric.html#range
         .. _Flake8: https://pypi.python.org/pypi/flake8
         
         
         History
         =======
         
+        1.2.2
+        -----
+        
+        * add ``__version__`` attr to module and ``--version`` option to CLI tool
+        * add ``--encoding`` option to CLI tool that overrides default file encoding (fixes #47)
+        
         1.2.1
         -----
         
         * expose ``SchemaStrategy.__eq__()`` for extension
         * add support for Python 3.8
         * update Trove classifiers
         * **Bugfix**: ``SchemaBuilder.__eq__()`` wasn't matching the ``$schema`` keyword correctly
```

### Comparing `genson-1.2.1/LICENSE` & `genson-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/test/test_bin.py` & `genson-1.2.2/test/test_bin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import unittest
 import json
+from os import path
 from subprocess import Popen, PIPE
+from . import base
 from genson import SchemaBuilder
 
 BASE_SCHEMA = {"$schema": SchemaBuilder.DEFAULT_URI}
-
-binpath = 'bin/genson.py'
+BIN_PATH = path.abspath(path.join(__file__, '..', '..', 'bin', 'genson.py'))
+FIXTURE_PATH = path.abspath(path.join(__file__, '..', 'fixtures'))
 
 
 def run(args=[], stdin_data=None):
     """
     Run the ``genson`` executable as a subprocess and return
     (stdout, stderr). Some assuaging is necessary to maintain
     Python compatibility with both Python 2 and 3.
     """
-    bin = Popen([binpath] + args, stdin=PIPE, stdout=PIPE)
+    genson_process = Popen([BIN_PATH] + args, stdin=PIPE, stdout=PIPE)
     if stdin_data is not None:
         stdin_data = stdin_data.encode('utf-8')
-    (stdout, stderr) = bin.communicate(stdin_data)
-    bin.wait()
+    (stdout, stderr) = genson_process.communicate(stdin_data)
+    genson_process.wait()
     if isinstance(stdout, bytes):
         stdout = stdout.decode('utf-8')
     if isinstance(stderr, bytes):
         stderr = stderr.decode('utf-8')
     return (stdout, stderr)
 
 
@@ -59,7 +61,23 @@
     def test_delim_auto_whitespace(self):
         (stdout, stderr) = run(['-d', ''], '{"hi":"there"} \n\t{"hi":5}')
         self.assertEqual(stderr, None)
         self.assertEqual(
             json.loads(stdout),
             dict({"required": ["hi"], "type": "object", "properties": {
                 "hi": {"type": ["integer", "string"]}}}, **BASE_SCHEMA))
+
+    @base.only_for_python_version('>=3.3')
+    def test_encoding_unicode(self):
+        (stdout, stderr) = run(['-e', 'utf-8', path.join(FIXTURE_PATH, 'utf-8.json')])
+        self.assertEqual(stderr, None)
+        self.assertEqual(
+            json.loads(stdout),
+            dict({"type": "string"}, **BASE_SCHEMA))
+
+    @base.only_for_python_version('>=3.3')
+    def test_encoding_cp1252(self):
+        (stdout, stderr) = run(['-e', 'cp1252', path.join(FIXTURE_PATH, 'cp1252.json')])
+        self.assertEqual(stderr, None)
+        self.assertEqual(
+            json.loads(stdout),
+            dict({"type": "string"}, **BASE_SCHEMA))
```

### Comparing `genson-1.2.1/test/test_gen_multi.py` & `genson-1.2.2/test/test_gen_multi.py`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/test/test_misuse.py` & `genson-1.2.2/test/test_misuse.py`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/test/test_add_single.py` & `genson-1.2.2/test/test_add_single.py`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/test/test_builder.py` & `genson-1.2.2/test/test_builder.py`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/test/test_add_multi.py` & `genson-1.2.2/test/test_add_multi.py`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/test/test_custom.py` & `genson-1.2.2/test/test_custom.py`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/test/test_gen_single.py` & `genson-1.2.2/test/test_gen_single.py`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/test/base.py` & `genson-1.2.2/test/base.py`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/test/test_seed_schema.py` & `genson-1.2.2/test/test_seed_schema.py`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/setup.py` & `genson-1.2.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 #!/usr/bin/env python
+import re
 from setuptools import setup
 
 
+def get_version():
+    with open('genson/__init__.py') as f:
+        match = re.search(r"__version__ = '([\d\.]+)'", f.read())
+        return match.group(1)
+
+
 def get_long_docs(*filenames):
     """Build rst description from a set of files."""
     docs = []
     for filename in filenames:
         with open(filename, 'r') as f:
             docs.append(f.read())
 
     return "\n\n".join(docs)
 
 
 setup(
     name='genson',
-    version='1.2.1',
+    version=get_version(),
     description='GenSON is a powerful, user-friendly JSON Schema generator.',
     long_description=get_long_docs('README.rst', 'HISTORY.rst', 'AUTHORS.rst'),
     keywords=['json', 'schema', 'json-schema', 'jsonschema', 'object',
               'generate', 'generator', 'builder', 'merge',
               'draft 7', 'validate', 'validation'],
     url='https://github.com/wolverdude/genson/',
     download_url='https://github.com/wolverdude/GenSON/tarball/v0.2s.0',
```

### Comparing `genson-1.2.1/genson/schema/strategies/object.py` & `genson-1.2.2/genson/schema/strategies/object.py`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/genson/schema/strategies/scalar.py` & `genson-1.2.2/genson/schema/strategies/scalar.py`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/genson/schema/strategies/__init__.py` & `genson-1.2.2/genson/schema/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/genson/schema/strategies/array.py` & `genson-1.2.2/genson/schema/strategies/array.py`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/genson/schema/strategies/base.py` & `genson-1.2.2/genson/schema/strategies/base.py`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/genson/schema/builder.py` & `genson-1.2.2/genson/schema/builder.py`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/genson/schema/node.py` & `genson-1.2.2/genson/schema/node.py`

 * *Files identical despite different names*

### Comparing `genson-1.2.1/HISTORY.rst` & `genson-1.2.2/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 History
 =======
 
+1.2.2
+-----
+
+* add ``__version__`` attr to module and ``--version`` option to CLI tool
+* add ``--encoding`` option to CLI tool that overrides default file encoding (fixes #47)
+
 1.2.1
 -----
 
 * expose ``SchemaStrategy.__eq__()`` for extension
 * add support for Python 3.8
 * update Trove classifiers
 * **Bugfix**: ``SchemaBuilder.__eq__()`` wasn't matching the ``$schema`` keyword correctly
```

### Comparing `genson-1.2.1/README.rst` & `genson-1.2.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -50,44 +50,54 @@
 
 .. code-block:: bash
 
     $ genson --help
 
 .. code-block::
 
-    usage: genson.py [-h] [-d DELIM] [-i SPACES] [-s SCHEMA] [-$ URI] ...
+    usage: genson [-h] [--version] [-d DELIM] [-e ENCODING] [-i SPACES]
+                  [-s SCHEMA] [-$ SCHEMA_URI]
+                  ...
 
     Generate one, unified JSON Schema from one or more JSON objects and/or JSON
-    Schemas. It's compatible with Draft 6 and above.
+    Schemas. Compatible with JSON-Schema Draft 4 and above.
 
     positional arguments:
-      object                files containing JSON objects (defaults to stdin if no
-                            arguments are passed)
+      object                Files containing JSON objects (defaults to stdin if no
+                            arguments are passed).
 
     optional arguments:
-      -h, --help            show this help message and exit
+      -h, --help            Show this help message and exit.
+      --version             Show version number and exit.
       -d DELIM, --delimiter DELIM
-                            set a delimiter - Use this option if the input files
+                            Set a delimiter. Use this option if the input files
                             contain multiple JSON objects/schemas. You can pass
                             any string. A few cases ('newline', 'tab', 'space')
                             will get converted to a whitespace character. If this
                             option is omitted, the parser will try to auto-detect
-                            boundaries
+                            boundaries.
+      -e ENCODING, --encoding ENCODING
+                            Use ENCODING instead of the default system encoding
+                            when reading files. ENCODING must be a valid codec
+                            name or alias.
       -i SPACES, --indent SPACES
-                            pretty-print the output, indenting SPACES spaces
+                            Pretty-print the output, indenting SPACES spaces.
       -s SCHEMA, --schema SCHEMA
-                            file containing a JSON Schema (can be specified
-                            multiple times to merge schemas)
-      -$ URI, --schema-uri URI
-                            the value of the '$schema' keyword (defaults to
+                            File containing a JSON Schema (can be specified
+                            multiple times to merge schemas).
+      -$ SCHEMA_URI, --schema-uri SCHEMA_URI
+                            The value of the '$schema' keyword (defaults to
                             'http://json-schema.org/schema#' or can be specified
                             in a schema with the -s option). If 'NULL' is passed,
                             the "$schema" keyword will not be included in the
                             result.
 
+.. note::
+    The ``--encoding`` option is only available in Python 3.
+
 GenSON Python API
 -----------------
 
 ``SchemaBuilder`` is the basic schema generator class. ``SchemaBuilder`` instances can be loaded up with existing schemas and objects before being serialized.
 
 .. code-block:: python
 
@@ -491,21 +501,23 @@
     >>> picky_builder.add_object(None) # this fails
     genson.schema.node.SchemaGenerationError: Could not find matching schema type for object: None
 
 
 Compatibility
 -------------
 
-GenSON has been tested and verified using the following versions of Python:
+GenSON has been tested and verified under the following Python versions:
 
-* Python 2.7.11
+* Python 2.7.13
 * Python 3.3.5
-* Python 3.4.4
-* Python 3.5.1
+* Python 3.4.5
+* Python 3.5.4
 * Python 3.6.2
+* Python 3.7.3
+* Python 3.8.2
 
 
 Contributing
 ------------
 
 When contributing, please follow these steps:
```

### Comparing `genson-1.2.1/genson.egg-info/PKG-INFO` & `genson-1.2.2/genson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: genson
-Version: 1.2.1
+Version: 1.2.2
 Summary: GenSON is a powerful, user-friendly JSON Schema generator.
 Home-page: https://github.com/wolverdude/genson/
 Author: Jon Wolverton
 Author-email: wolverton.jr@gmail.com
 License: MIT
 Download-URL: https://github.com/wolverdude/GenSON/tarball/v0.2s.0
 Description: GenSON
@@ -59,44 +59,54 @@
         
         .. code-block:: bash
         
             $ genson --help
         
         .. code-block::
         
-            usage: genson.py [-h] [-d DELIM] [-i SPACES] [-s SCHEMA] [-$ URI] ...
+            usage: genson [-h] [--version] [-d DELIM] [-e ENCODING] [-i SPACES]
+                          [-s SCHEMA] [-$ SCHEMA_URI]
+                          ...
         
             Generate one, unified JSON Schema from one or more JSON objects and/or JSON
-            Schemas. It's compatible with Draft 6 and above.
+            Schemas. Compatible with JSON-Schema Draft 4 and above.
         
             positional arguments:
-              object                files containing JSON objects (defaults to stdin if no
-                                    arguments are passed)
+              object                Files containing JSON objects (defaults to stdin if no
+                                    arguments are passed).
         
             optional arguments:
-              -h, --help            show this help message and exit
+              -h, --help            Show this help message and exit.
+              --version             Show version number and exit.
               -d DELIM, --delimiter DELIM
-                                    set a delimiter - Use this option if the input files
+                                    Set a delimiter. Use this option if the input files
                                     contain multiple JSON objects/schemas. You can pass
                                     any string. A few cases ('newline', 'tab', 'space')
                                     will get converted to a whitespace character. If this
                                     option is omitted, the parser will try to auto-detect
-                                    boundaries
+                                    boundaries.
+              -e ENCODING, --encoding ENCODING
+                                    Use ENCODING instead of the default system encoding
+                                    when reading files. ENCODING must be a valid codec
+                                    name or alias.
               -i SPACES, --indent SPACES
-                                    pretty-print the output, indenting SPACES spaces
+                                    Pretty-print the output, indenting SPACES spaces.
               -s SCHEMA, --schema SCHEMA
-                                    file containing a JSON Schema (can be specified
-                                    multiple times to merge schemas)
-              -$ URI, --schema-uri URI
-                                    the value of the '$schema' keyword (defaults to
+                                    File containing a JSON Schema (can be specified
+                                    multiple times to merge schemas).
+              -$ SCHEMA_URI, --schema-uri SCHEMA_URI
+                                    The value of the '$schema' keyword (defaults to
                                     'http://json-schema.org/schema#' or can be specified
                                     in a schema with the -s option). If 'NULL' is passed,
                                     the "$schema" keyword will not be included in the
                                     result.
         
+        .. note::
+            The ``--encoding`` option is only available in Python 3.
+        
         GenSON Python API
         -----------------
         
         ``SchemaBuilder`` is the basic schema generator class. ``SchemaBuilder`` instances can be loaded up with existing schemas and objects before being serialized.
         
         .. code-block:: python
         
@@ -500,21 +510,23 @@
             >>> picky_builder.add_object(None) # this fails
             genson.schema.node.SchemaGenerationError: Could not find matching schema type for object: None
         
         
         Compatibility
         -------------
         
-        GenSON has been tested and verified using the following versions of Python:
+        GenSON has been tested and verified under the following Python versions:
         
-        * Python 2.7.11
+        * Python 2.7.13
         * Python 3.3.5
-        * Python 3.4.4
-        * Python 3.5.1
+        * Python 3.4.5
+        * Python 3.5.4
         * Python 3.6.2
+        * Python 3.7.3
+        * Python 3.8.2
         
         
         Contributing
         ------------
         
         When contributing, please follow these steps:
         
@@ -573,14 +585,20 @@
         .. _minimum number: https://json-schema.org/understanding-json-schema/reference/numeric.html#range
         .. _Flake8: https://pypi.python.org/pypi/flake8
         
         
         History
         =======
         
+        1.2.2
+        -----
+        
+        * add ``__version__`` attr to module and ``--version`` option to CLI tool
+        * add ``--encoding`` option to CLI tool that overrides default file encoding (fixes #47)
+        
         1.2.1
         -----
         
         * expose ``SchemaStrategy.__eq__()`` for extension
         * add support for Python 3.8
         * update Trove classifiers
         * **Bugfix**: ``SchemaBuilder.__eq__()`` wasn't matching the ``$schema`` keyword correctly
```

### Comparing `genson-1.2.1/genson.egg-info/SOURCES.txt` & `genson-1.2.2/genson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

