# Comparing `tmp/honeybee-display-0.3.7.tar.gz` & `tmp/honeybee-display-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-display-0.3.7.tar", last modified: Tue Apr  9 20:33:53 2024, max compression
+gzip compressed data, was "dist/honeybee-display-0.3.8.tar", last modified: Thu May 16 17:31:24 2024, max compression
```

## Comparing `honeybee-display-0.3.7.tar` & `honeybee-display-0.3.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/aperture.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/attr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14389 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/colorobj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/door.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display/energy/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/energy/colorobj.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/face.py
--rw-r--r--   0 runner    (1001) docker     (127)    24915 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display/radiance/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/radiance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/room.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/shade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/shademesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:31:24.000000 honeybee-display-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-16 17:31:24.000000 honeybee-display-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:31:24.000000 honeybee-display-0.3.8/honeybee_display/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/honeybee_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/honeybee_display/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/honeybee_display/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/honeybee_display/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/honeybee_display/attr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:31:24.000000 honeybee-display-0.3.8/honeybee_display/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/honeybee_display/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14389 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/honeybee_display/colorobj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/honeybee_display/door.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:31:24.000000 honeybee-display-0.3.8/honeybee_display/energy/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/honeybee_display/energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/honeybee_display/energy/colorobj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/honeybee_display/face.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24915 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/honeybee_display/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:31:24.000000 honeybee-display-0.3.8/honeybee_display/radiance/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/honeybee_display/radiance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/honeybee_display/room.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/honeybee_display/shade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/honeybee_display/shademesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:31:24.000000 honeybee-display-0.3.8/honeybee_display.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-16 17:31:24.000000 honeybee-display-0.3.8/honeybee_display.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-16 17:31:24.000000 honeybee-display-0.3.8/honeybee_display.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 17:31:24.000000 honeybee-display-0.3.8/honeybee_display.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 17:31:24.000000 honeybee-display-0.3.8/honeybee_display.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-16 17:31:24.000000 honeybee-display-0.3.8/honeybee_display.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 17:31:24.000000 honeybee-display-0.3.8/honeybee_display.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-16 17:31:24.000000 honeybee-display-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-16 17:30:21.000000 honeybee-display-0.3.8/setup.py
```

### Comparing `honeybee-display-0.3.7/LICENSE` & `honeybee-display-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.7/PKG-INFO` & `honeybee-display-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-display
-Version: 0.3.7
+Version: 0.3.8
 Summary: Adds methods to translate honeybee objects to VisualizationSets.
 Home-page: https://github.com/ladybug-tools/honeybee-display
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-display-0.3.7/README.md` & `honeybee-display-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.7/dev-requirements.txt` & `honeybee-display-0.3.8/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.7/honeybee_display/_extend_honeybee.py` & `honeybee-display-0.3.8/honeybee_display/_extend_honeybee.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.7/honeybee_display/aperture.py` & `honeybee-display-0.3.8/honeybee_display/aperture.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.7/honeybee_display/attr.py` & `honeybee-display-0.3.8/honeybee_display/attr.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.7/honeybee_display/cli/__init__.py` & `honeybee-display-0.3.8/honeybee_display/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """honeybee-display commands."""
 import click
 import sys
 import os
 import logging
 import json
 import pickle
+import tempfile
+import uuid
 
 from honeybee.model import Model
 from honeybee.cli import main
 
 from honeybee_display.attr import FaceAttribute, RoomAttribute
 
 _logger = logging.getLogger(__name__)
@@ -112,16 +114,15 @@
 @click.option(
     '--output-format', '-of', help='Text for the output format of the resulting '
     'VisualizationSet File (.vsf). Choose from: vsf, json, pkl, vtkjs, html. Note '
     'that both vsf and json refer to the the JSON version of the VisualizationSet '
     'file and the distinction between the two is only for help in coordinating file '
     'extensions (since both .vsf and .json can be acceptable). Also note that '
     'ladybug-vtk must be installed in order for the vtkjs or html options to be usable '
-    'and the html format refers to a web page with the vtkjs file embedded within it. '
-    'The vtkjs and html options also require an explicit --output-file to be specified.',
+    'and the html format refers to a web page with the vtkjs file embedded within it.',
     type=str, default='vsf', show_default=True)
 @click.option(
     '--output-file', help='Optional file to output the JSON string of '
     'the config object. By default, it will be printed out to stdout',
     type=click.File('w'), default='-', show_default=True)
 def model_to_vis_set(
         model_file, color_by, wireframe, mesh, show_color_by,
@@ -166,30 +167,42 @@
         elif output_format == 'pkl':
             if output_file.name != '<stdout>':
                 out_folder, out_file = os.path.split(output_file.name)
                 vis_set.to_pkl(out_file, out_folder)
             else:
                 output_file.write(pickle.dumps(vis_set.to_dict()))
         elif output_format in ('vtkjs', 'html'):
-            assert output_file.name != '<stdout>', \
-                'Must specify an --output-file to use --output-format vtkjs.'
-            out_folder, out_file = os.path.split(output_file.name)
-            try:
+            if output_file.name == '<stdout>':  # get a temporary file
+                out_file = str(uuid.uuid4())[:6]
+                out_folder = tempfile.gettempdir()
+            else:
+                out_folder, out_file = os.path.split(output_file.name)
                 if out_file.endswith('.vtkjs'):
                     out_file = out_file[:-6]
                 elif out_file.endswith('.html'):
                     out_file = out_file[:-5]
+            try:
                 if output_format == 'vtkjs':
                     vis_set.to_vtkjs(output_folder=out_folder, file_name=out_file)
                 if output_format == 'html':
                     vis_set.to_html(output_folder=out_folder, file_name=out_file)
             except AttributeError as ae:
                 raise AttributeError(
                     'Ladybug-vtk must be installed in order to use --output-format '
                     'vtkjs.\n{}'.format(ae))
+            if output_file.name == '<stdout>':  # load file contents to stdout
+                out_file_ext = out_file + '.' + output_format
+                out_file_path = os.path.join(out_folder, out_file_ext)
+                if output_format == 'html':
+                    with open(out_file_path, encoding='utf-8') as of:
+                        f_contents = of.read()
+                else:  # vtkjs can only be read as binary
+                    with open(out_file_path, 'rb') as of:
+                        f_contents = of.read()
+                output_file.write(f_contents)
         else:
             raise ValueError('Unrecognized output-format "{}".'.format(output_format))
     except Exception as e:
         _logger.exception('Failed to translate Model to VisualizationSet.\n{}'.format(e))
         sys.exit(1)
     else:
         sys.exit(0)
```

### Comparing `honeybee-display-0.3.7/honeybee_display/colorobj.py` & `honeybee-display-0.3.8/honeybee_display/colorobj.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.7/honeybee_display/door.py` & `honeybee-display-0.3.8/honeybee_display/door.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.7/honeybee_display/energy/colorobj.py` & `honeybee-display-0.3.8/honeybee_display/energy/colorobj.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.7/honeybee_display/face.py` & `honeybee-display-0.3.8/honeybee_display/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.7/honeybee_display/model.py` & `honeybee-display-0.3.8/honeybee_display/model.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.7/honeybee_display/room.py` & `honeybee-display-0.3.8/honeybee_display/room.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.7/honeybee_display/shade.py` & `honeybee-display-0.3.8/honeybee_display/shade.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.7/honeybee_display/shademesh.py` & `honeybee-display-0.3.8/honeybee_display/shademesh.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.7/honeybee_display.egg-info/PKG-INFO` & `honeybee-display-0.3.8/honeybee_display.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-display
-Version: 0.3.7
+Version: 0.3.8
 Summary: Adds methods to translate honeybee objects to VisualizationSets.
 Home-page: https://github.com/ladybug-tools/honeybee-display
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-display-0.3.7/honeybee_display.egg-info/SOURCES.txt` & `honeybee-display-0.3.8/honeybee_display.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.7/setup.py` & `honeybee-display-0.3.8/setup.py`

 * *Files identical despite different names*

