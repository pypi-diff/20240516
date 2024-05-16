# Comparing `tmp/gddoc2yml-0.1.1.tar.gz` & `tmp/gddoc2yml-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gddoc2yml-0.1.1.tar", last modified: Fri May  3 06:14:58 2024, max compression
+gzip compressed data, was "gddoc2yml-0.2.0.tar", last modified: Thu May 16 06:41:44 2024, max compression
```

## Comparing `gddoc2yml-0.1.1.tar` & `gddoc2yml-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:14:58.208474 gddoc2yml-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-05-03 06:14:58.208474 gddoc2yml-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 06:14:58.208474 gddoc2yml-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:14:58.200474 gddoc2yml-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:14:58.204474 gddoc2yml-0.1.1/src/gddoc2yml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/src/gddoc2yml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20580 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/src/gddoc2yml/gdxml2yml.py
--rw-r--r--   0 runner    (1001) docker     (127)    44642 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/src/gddoc2yml/gdxml_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)   106910 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/src/gddoc2yml/make_rst.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/src/gddoc2yml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:14:58.208474 gddoc2yml-0.1.1/src/gddoc2yml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-05-03 06:14:58.000000 gddoc2yml-0.1.1/src/gddoc2yml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-03 06:14:58.000000 gddoc2yml-0.1.1/src/gddoc2yml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 06:14:58.000000 gddoc2yml-0.1.1/src/gddoc2yml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-03 06:14:58.000000 gddoc2yml-0.1.1/src/gddoc2yml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 06:14:58.000000 gddoc2yml-0.1.1/src/gddoc2yml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 06:14:58.000000 gddoc2yml-0.1.1/src/gddoc2yml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:14:58.204474 gddoc2yml-0.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:14:58.208474 gddoc2yml-0.1.1/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/tests/classes/CollisionObject3D.xml
--rw-r--r--   0 runner    (1001) docker     (127)    79398 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/tests/classes/Node.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20604 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/tests/classes/Node3D.xml
--rw-r--r--   0 runner    (1001) docker     (127)    54560 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/tests/classes/Object.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/tests/classes/PhysicsBody3D.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/tests/classes/StaticBody3D.xml
--rw-r--r--   0 runner    (1001) docker     (127)    14229 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/tests/classes/int.xml
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/tests/test_console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-03 06:14:44.000000 gddoc2yml-0.1.1/tests/test_gdxml2yml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:41:44.453034 gddoc2yml-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-05-16 06:41:44.453034 gddoc2yml-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 06:41:44.453034 gddoc2yml-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:41:44.449034 gddoc2yml-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:41:44.453034 gddoc2yml-0.2.0/src/gddoc2yml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/src/gddoc2yml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/src/gddoc2yml/gdxml2xrefmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19164 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/src/gddoc2yml/gdxml2yml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46947 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/src/gddoc2yml/gdxml_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106910 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/src/gddoc2yml/make_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/src/gddoc2yml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:41:44.453034 gddoc2yml-0.2.0/src/gddoc2yml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-05-16 06:41:44.000000 gddoc2yml-0.2.0/src/gddoc2yml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-16 06:41:44.000000 gddoc2yml-0.2.0/src/gddoc2yml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 06:41:44.000000 gddoc2yml-0.2.0/src/gddoc2yml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-16 06:41:44.000000 gddoc2yml-0.2.0/src/gddoc2yml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 06:41:44.000000 gddoc2yml-0.2.0/src/gddoc2yml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 06:41:44.000000 gddoc2yml-0.2.0/src/gddoc2yml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:41:44.453034 gddoc2yml-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:41:44.453034 gddoc2yml-0.2.0/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/tests/classes/CollisionObject3D.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    79398 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/tests/classes/Node.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20604 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/tests/classes/Node3D.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    54560 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/tests/classes/Object.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/tests/classes/PhysicsBody3D.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/tests/classes/StaticBody3D.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    14229 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/tests/classes/int.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/tests/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-16 06:41:26.000000 gddoc2yml-0.2.0/tests/test_gdxml2yml.py
```

### Comparing `gddoc2yml-0.1.1/LICENSE` & `gddoc2yml-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.1.1/PKG-INFO` & `gddoc2yml-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gddoc2yml
-Version: 0.1.1
+Version: 0.2.0
 Summary: Convert godot xml docs to docfx yml
 Author-email: Nick Maltbie <nick.dmalt@gmail.com>
 Project-URL: Homepage, https://github.com/nicholas-maltbie/gddoc2yml
 Project-URL: Issues, https://github.com/nicholas-maltbie/gddoc2yml/issues
 Project-URL: GitHub, https://github.com/nicholas-maltbie/gddoc2yml
 Project-URL: Changelog, https://github.com/nicholas-maltbie/gddoc2yml/blob/main/CHANGELOG.md
 Keywords: godot,docfx,yml,xml,documentation
@@ -33,35 +33,44 @@
 
 Install gddoc2yml via pip
 
 ```bash
 python3 -m pip install gddoc2yml
 ```
 
-Then you will have the gdxml2yml command available:
+Then you will have the gdxml2yml and gdxml2xrefmap command available:
 
 <!-- markdownlint-disable MD013 -->
 
 ```bash
-gdxml2yml
-    usage: gdxml2yml [-h] [--filter FILTER] path [path ...] output
-    gdxml2yml: error: the following arguments are required: path, output
-
 gdxml2yml -h
     usage: gdxml2yml [-h] [--filter FILTER] path [path ...] output
 
     Convert godot documentation xml file to yml for docfx.
 
     positional arguments:
     path             A path to an XML file or a directory containing XML files to parse.
     output           output folder to store all generated yml files.
 
     options:
     -h, --help       show this help message and exit
     --filter FILTER  The filepath pattern for XML files to filter
+
+gdxml2xrefmap -h
+    usage: gdxml2xrefmap [-h] [--filter FILTER] path [path ...] output
+
+    Convert godot documentation xml files into a xrefmap compatible with DoxFx.
+
+    positional arguments:
+    path             A path to an XML file or a directory containing XML files to parse.
+    output           output path to store xrefmap.
+
+    options:
+    -h, --help       show this help message and exit
+    --filter FILTER  The filepath pattern for XML files to filter.
 ```
 
 <!-- markdownlint-enable MD013 -->
 
 ## Using gddoc2yml
 
 Export xml docs for your project with godot, us gdxml2yml to generate yml api,
@@ -103,14 +112,37 @@
     {
         "files": ["*.yml"],
         "src": "api",
         "dest": "api"
     },
     ```
 
+### Generating xrefmap for Godot Docs
+
+Included is an additional command, `gdxml2xrefmap` to generate
+an xrefmap for the godot docs.
+
+```bash
+gdxml2xrefmap godot/doc/classes godot/modules out/godot_xrefmap.yml
+```
+
+**Note** the build for this repo contains an xrefmap that points to godot's
+documentation. You can reference this in your `docfx.json` file as a `xref`
+like so:
+
+```json
+{
+  "build": {
+    "xref": [
+      "https://gddoc2yml.nickmaltbie.com/xrefmap/godot_xrefmap.yml"
+    ]
+  }
+}
+```
+
 ## References
 
 * [Godot -- CLI Reference](https://docs.godotengine.org/en/stable/tutorials/editor/command_line_tutorial.html#command-line-reference)
 * [Godot -- make_rst.py](https://github.com/godotengine/godot/blob/master/doc/tools/make_rst.py)
 * [DocFx -- Github](https://github.com/dotnet/docfx)
 * [DocFx -- Introduction to Multiple Languages Support](https://xxred.gitee.io/docfx/tutorial/universalreference/intro_multiple_langs_support.html)
 * [DocFx -- Custom Template](https://dotnet.github.io/docfx/docs/template.html?tabs=modern#custom-template)
@@ -186,12 +218,15 @@
 Build godot docs using latest gddoc2yml.
 
 ```bash
 # Install from repo
 python3 -m pip install .
 
 # Generate docs using gdxml2yml
-gdxml2yml godot/doc/classes godot/modules godot/platform/android/doc_classes doc/api
+gdxml2yml godot/doc/classes godot/modules godot/platform/android/doc_classes doc/godot/api
+
+# Generate xrefmap using gdxml2xrefmap
+gdxml2xrefmap godot/doc/classes godot/modules doc/xrefmap/godot_xrefmap.yml
 
 # Startup docfx website
 dotnet tool run docfx --serve doc/docfx.json
 ```
```

### Comparing `gddoc2yml-0.1.1/README.md` & `gddoc2yml-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,35 +7,44 @@
 
 Install gddoc2yml via pip
 
 ```bash
 python3 -m pip install gddoc2yml
 ```
 
-Then you will have the gdxml2yml command available:
+Then you will have the gdxml2yml and gdxml2xrefmap command available:
 
 <!-- markdownlint-disable MD013 -->
 
 ```bash
-gdxml2yml
-    usage: gdxml2yml [-h] [--filter FILTER] path [path ...] output
-    gdxml2yml: error: the following arguments are required: path, output
-
 gdxml2yml -h
     usage: gdxml2yml [-h] [--filter FILTER] path [path ...] output
 
     Convert godot documentation xml file to yml for docfx.
 
     positional arguments:
     path             A path to an XML file or a directory containing XML files to parse.
     output           output folder to store all generated yml files.
 
     options:
     -h, --help       show this help message and exit
     --filter FILTER  The filepath pattern for XML files to filter
+
+gdxml2xrefmap -h
+    usage: gdxml2xrefmap [-h] [--filter FILTER] path [path ...] output
+
+    Convert godot documentation xml files into a xrefmap compatible with DoxFx.
+
+    positional arguments:
+    path             A path to an XML file or a directory containing XML files to parse.
+    output           output path to store xrefmap.
+
+    options:
+    -h, --help       show this help message and exit
+    --filter FILTER  The filepath pattern for XML files to filter.
 ```
 
 <!-- markdownlint-enable MD013 -->
 
 ## Using gddoc2yml
 
 Export xml docs for your project with godot, us gdxml2yml to generate yml api,
@@ -77,14 +86,37 @@
     {
         "files": ["*.yml"],
         "src": "api",
         "dest": "api"
     },
     ```
 
+### Generating xrefmap for Godot Docs
+
+Included is an additional command, `gdxml2xrefmap` to generate
+an xrefmap for the godot docs.
+
+```bash
+gdxml2xrefmap godot/doc/classes godot/modules out/godot_xrefmap.yml
+```
+
+**Note** the build for this repo contains an xrefmap that points to godot's
+documentation. You can reference this in your `docfx.json` file as a `xref`
+like so:
+
+```json
+{
+  "build": {
+    "xref": [
+      "https://gddoc2yml.nickmaltbie.com/xrefmap/godot_xrefmap.yml"
+    ]
+  }
+}
+```
+
 ## References
 
 * [Godot -- CLI Reference](https://docs.godotengine.org/en/stable/tutorials/editor/command_line_tutorial.html#command-line-reference)
 * [Godot -- make_rst.py](https://github.com/godotengine/godot/blob/master/doc/tools/make_rst.py)
 * [DocFx -- Github](https://github.com/dotnet/docfx)
 * [DocFx -- Introduction to Multiple Languages Support](https://xxred.gitee.io/docfx/tutorial/universalreference/intro_multiple_langs_support.html)
 * [DocFx -- Custom Template](https://dotnet.github.io/docfx/docs/template.html?tabs=modern#custom-template)
@@ -160,12 +192,15 @@
 Build godot docs using latest gddoc2yml.
 
 ```bash
 # Install from repo
 python3 -m pip install .
 
 # Generate docs using gdxml2yml
-gdxml2yml godot/doc/classes godot/modules godot/platform/android/doc_classes doc/api
+gdxml2yml godot/doc/classes godot/modules godot/platform/android/doc_classes doc/godot/api
+
+# Generate xrefmap using gdxml2xrefmap
+gdxml2xrefmap godot/doc/classes godot/modules doc/xrefmap/godot_xrefmap.yml
 
 # Startup docfx website
 dotnet tool run docfx --serve doc/docfx.json
 ```
```

### Comparing `gddoc2yml-0.1.1/pyproject.toml` & `gddoc2yml-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "pathvalidate>=3.2.0", "PyYAML>=6.0.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gddoc2yml"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Nick Maltbie", email="nick.dmalt@gmail.com" },
 ]
 description = "Convert godot xml docs to docfx yml"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
@@ -37,7 +37,8 @@
 Homepage = "https://github.com/nicholas-maltbie/gddoc2yml"
 Issues = "https://github.com/nicholas-maltbie/gddoc2yml/issues"
 GitHub = "https://github.com/nicholas-maltbie/gddoc2yml"
 Changelog = "https://github.com/nicholas-maltbie/gddoc2yml/blob/main/CHANGELOG.md"
 
 [project.scripts]
 gdxml2yml = "gddoc2yml.gdxml2yml:main"
+gdxml2xrefmap = "gddoc2yml.gdxml2xrefmap:main"
```

### Comparing `gddoc2yml-0.1.1/src/gddoc2yml/gdxml2yml.py` & `gddoc2yml-0.2.0/src/gddoc2yml/gdxml2yml.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,23 @@
 # ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import argparse
 import os
 import pathvalidate
 import re
-import xml.etree.ElementTree as ET
 import yaml
 
-from .make_rst import AnnotationDef, MethodDef, SignalDef, State, PropertyDef, \
-    ClassDef, EnumDef, TypeName, print_error
-from .gdxml_helpers import format_text_block, make_link, make_method_signature, \
-    full_type_name, make_setter_signature, make_getter_signature, get_method_qualifiers, get_method_return_type
+from .make_rst import AnnotationDef, MethodDef, SignalDef, State, \
+    PropertyDef, ClassDef, EnumDef, TypeName
 from typing import Dict, List, Tuple, Union
+from .gdxml_helpers import make_link, format_text_block, full_type_name, \
+    make_method_signature, get_method_uid, get_method_qualifiers, get_method_return_type, \
+    make_setter_signature, make_getter_signature, get_class_uid, get_signal_uid, \
+    get_constant_uid, get_theme_uid, get_class_state_from_docs
 
 
 yml_mime_managed_reference_prefix = "### YamlMime:ManagedReference"
 yml_mime_toc_prefix = "### YamlMime:TableOfContent"
 
 
 def dir_path(string):
@@ -173,27 +174,23 @@
     return {
         "uid": full_name,
         "name": full_name,
     }
 
 
 def _get_method_yml(
-        class_name: str,
+        class_def: ClassDef,
         method_def: Union[AnnotationDef, MethodDef, SignalDef],
-        state: State, method_type: str,
-        always_include_parenthesis: bool
+        state: State, method_type: str
 ) -> Tuple[Dict[str, Dict], Dict]:
     references = {}
-    signature_short = make_method_signature(
-        method_def, False, False, False, state, True, always_include_parenthesis)
-    signature_spaces = make_method_signature(
-        method_def, True, False, False, state, False, always_include_parenthesis)
-    signature_spaces_named = make_method_signature(
-        method_def, True, True, False, state, False, always_include_parenthesis)
-    full_name = f"{class_name}.{signature_short}"
+    signature_short = make_method_signature(method_def, False, False, False, state, True)
+    signature_spaces = make_method_signature(method_def, True, False, False, state, False)
+    signature_spaces_named = make_method_signature(method_def, True, True, False, state, False)
+    full_name = get_method_uid(method_def, class_def, state)
 
     summary = ""
     if method_def.qualifiers:
         summary += f"Qualifiers: {get_method_qualifiers(method_def)}\n\n"
     summary += format_text_block(method_def.description.strip(), method_def, state)
 
     syntax = f"{signature_spaces_named}"
@@ -203,28 +200,28 @@
 
     method_yml = {
         "uid": full_name,
         "commentId": f"M:{full_name}",
         "id": signature_short,
         "langs": ["gdscript", "csharp"],
         "name": signature_spaces,
-        "nameWithType": f"{class_name}.{signature_spaces}",
+        "nameWithType": f"{class_def.name}.{signature_spaces}",
         "type": method_type,
         "syntax": {
             "content": syntax,
             "parameters": [
                 {
                     "id": parameter.name,
                     "type": parameter.type_name.type_name,
                 }
                 for parameter in method_def.parameters
             ],
         },
         "summary": summary,
-        "parent": class_name,
+        "parent": class_def.name,
     }
 
     # add all types of parameter as references
     for parameter in method_def.parameters:
         references[parameter.type_name.type_name] = _make_reference_yml(parameter.type_name, state)
 
     return references, method_yml
@@ -272,15 +269,15 @@
 
     return property_yml
 
 
 def _get_class_yml(  # noqa: C901 # TODO: Fix this function!
         class_name: str, class_def: ClassDef, state: State) -> str:
     class_yml = {
-        "uid": class_name,
+        "uid": get_class_uid(class_def),
         "commentId": "T:" + class_name,
         "id": class_name,
         "langs": ["gdscript", "csharp"],
         "name": class_name,
         "nameWithType": class_name,
         "type": "Class",
     }
@@ -322,21 +319,21 @@
     #  https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/xmldoc/recommended-tags#seealso
     if len(class_def.tutorials) > 0:
         class_yml["seealso"] = _get_seealso_list(class_def)
 
     # Signal descriptions
     signals = []
     for signal in class_def.signals.values():
-        signature_short = make_method_signature(signal, False, False, False, state, False, False)
-        signature_spaces = make_method_signature(signal, True, False, False, state, False, False)
-        signature_spaces_named = make_method_signature(signal, True, True, False, state, False, False)
-        full_name = f"{class_name}.{signature_short}"
+        signature_short = make_method_signature(signal, False, False, False, state, False)
+        signature_spaces = make_method_signature(signal, True, False, False, state, False)
+        signature_spaces_named = make_method_signature(signal, True, True, False, state, False)
+        signal_id = get_signal_uid(signal, class_def, state)
         signal_yml = {
-            "uid": full_name,
-            "commentId": f"E:{full_name}",
+            "uid": signal_id,
+            "commentId": f"E:{signal_id}",
             "id": signature_short,
             "langs": ["gdscript", "csharp"],
             "name": signature_spaces,
             "nameWithType": f"{class_name}.{signature_spaces}",
             "type": "Event",
             "syntax": {
                 "content": f"signal {signature_spaces_named}",
@@ -357,15 +354,15 @@
             references[parameter.type_name.type_name] = _make_reference_yml(parameter.type_name, state)
 
         signals.append(signal_yml)
 
     # Constant descriptions
     constants = []
     for constant in class_def.constants.values():
-        constant_id = f"{class_name}.{constant.name}"
+        constant_id = get_constant_uid(constant, class_def)
         constant_yml = {
             "uid": constant_id,
             "commentId": f"F:{constant_id}",
             "id": constant.name,
             "langs": ["gdscript", "csharp"],
             "name": constant.name,
             "nameWithType": constant_id,
@@ -379,15 +376,15 @@
         }
         constants.append(constant_yml)
 
     # Annotation descriptions
     annotations = []
     for method_list in class_def.annotations.values():
         for _, m in enumerate(method_list):
-            annotation_ref, annotation_yml = _get_method_yml(class_name, m, state, "Property", False)
+            annotation_ref, annotation_yml = _get_method_yml(class_def, m, state, "Property")
             annotation_yml["summary"] = "**Annotation**\n\n" + annotation_yml["summary"]
             references.update(annotation_ref)
             annotations.append(annotation_yml)
 
     # Property descriptions
     properties = []
     if any(not p.overrides for p in class_def.properties.values()) > 0:
@@ -398,36 +395,36 @@
             properties.append(property_yml)
             references[property_def.type_name.type_name] = _make_reference_yml(property_def.type_name, state)
 
     # Constructor, Method, Operator descriptions
     constructors = []
     for method_list in class_def.constructors.values():
         for _, m in enumerate(method_list):
-            constructor_ref, constructor_yml = _get_method_yml(class_name, m, state, "Constructor", True)
+            constructor_ref, constructor_yml = _get_method_yml(class_def, m, state, "Constructor")
             references.update(constructor_ref)
             constructors.append(constructor_yml)
 
     methods = []
     for method_list in class_def.methods.values():
         for _, m in enumerate(method_list):
-            method_ref, method_yml = _get_method_yml(class_name, m, state, "Method", True)
+            method_ref, method_yml = _get_method_yml(class_def, m, state, "Method")
             references.update(method_ref)
             constructors.append(method_yml)
 
     operators = []
     for method_list in class_def.operators.values():
         for _, m in enumerate(method_list):
-            operator_ref, operator_yml = _get_method_yml(class_name, m, state, "Operator", False)
+            operator_ref, operator_yml = _get_method_yml(class_def, m, state, "Operator")
             references.update(operator_ref)
             operators.append(operator_yml)
 
     # Theme property descriptions
     theme_properties = []
     for theme_item_def in class_def.theme_items.values():
-        theme_item_id = f"{class_name}.{theme_item_def.name}"
+        theme_item_id = get_theme_uid(theme_item_def, class_def)
         syntax = f"{theme_item_def.type_name.type_name} {theme_item_def.name}"
         if theme_item_def.default_value is not None:
             syntax = f" = {theme_item_def.default_value}"
         theme_yml = {
             "uid": theme_item_id,
             "commentId": f"P:{theme_item_id}",
             "id": theme_item_def.name,
@@ -455,65 +452,26 @@
     return yaml.dump(
         {
             "items": items,
             "references": list(references.values())
         }, default_flow_style=False, sort_keys=False)
 
 
-def _get_file_list(paths: List[str]) -> List[str]:
-    file_list: List[str] = []
-
-    for path in paths:
-        if os.path.isdir(path):
-            for root, subdirs, files in os.walk(path):
-                file_list += (os.path.join(root, filename) for filename in files if filename.endswith(".xml"))
-        elif os.path.isfile(path):
-            if not path.endswith(".xml"):
-                print(f'Got non-.xml file "{path}" in input, skipping.')
-                continue
-            file_list.append(path)
-
-    return file_list
-
-
-def _read_xml_data(files: List[str]) -> Dict[str, Tuple[ET.Element, str]]:
-    classes: Dict[str, Tuple[ET.Element, str]] = {}
-    for cur_file in _get_file_list(files):
-        tree = ET.parse(cur_file)
-        doc = tree.getroot()
-        name = doc.attrib["name"]
-        classes[name] = (doc, cur_file)
-
-    return classes
-
-
-def _get_class_state_from_docs(paths: List[str]) -> State:
-    files: List[str] = _get_file_list(paths)
-    classes: Dict[str, Tuple[ET.Element, str]] = _read_xml_data(files)
-    state = State()
-    for name, data in classes.items():
-        try:
-            state.parse_class(data[0], data[1])
-        except Exception as e:
-            print_error(f"{name}.xml: Exception while parsing class: {e}", state)
-    return state
-
-
 def _get_parser():
     parser = argparse.ArgumentParser(description='Convert godot documentation xml file to yml for docfx.')
     parser.add_argument("path", nargs="+", help="A path to an XML file or a directory containing XML files to parse.")
     parser.add_argument("--filter", default="", help="The filepath pattern for XML files to filter.")
     parser.add_argument('output', help='output folder to store all generated yml files.')
     return parser
 
 
 def main() -> None:
     args = _get_parser().parse_args()
 
-    state: State = _get_class_state_from_docs(args.path)
+    state: State = get_class_state_from_docs(args.path)
 
     # Create the output folder recursively if it doesn't already exist.
     os.makedirs(args.output, exist_ok=True)
     pattern = re.compile(args.filter)
 
     class_files = []
     state.sort_classes()
```

### Comparing `gddoc2yml-0.1.1/src/gddoc2yml/gdxml_helpers.py` & `gddoc2yml-0.2.0/src/gddoc2yml/gdxml_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,20 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING
 # BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
 # CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 # ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+import os
+import xml.etree.ElementTree as ET
+
 from .make_rst import State, DefinitionBase, TagState, MethodDef, \
     SignalDef, AnnotationDef, ParameterDef, ClassDef, PropertyDef, TypeName, \
+    ThemeItemDef, ConstantDef, \
     RESERVED_CODEBLOCK_TAGS, RESERVED_CROSSLINK_TAGS, GODOT_DOCS_PATTERN, \
     MARKUP_ALLOWED_PRECEDENT, MARKUP_ALLOWED_SUBSEQUENT
 from typing import List, Dict, TextIO, Tuple, Optional, Union
 
 GODOT_DOC_URL = "https://docs.godotengine.org/en/stable/"
 
 STYLES: Dict[str, str] = {}
@@ -975,21 +979,21 @@
 
 def make_method_signature(
     definition: Union[AnnotationDef, MethodDef, SignalDef],
     spaces: bool,
     named_params: bool,
     xref_param_types: bool,
     state: State,
-    sanitize: bool,
-    always_include_parenthesis: bool
+    sanitize: bool
 ) -> str:
     qualifiers = None
     if isinstance(definition, (MethodDef, AnnotationDef)):
         qualifiers = definition.qualifiers
 
+    always_include_parenthesis: bool = definition is MethodDef
     varargs = qualifiers is not None and "vararg" in qualifiers
     params = []
     for parameter in definition.parameters:
         type_name = parameter.type_name.type_name
         if xref_param_types:
             type_name = make_type(parameter.type_name.type_name, state)
 
@@ -1061,15 +1065,15 @@
     # Otherwise we fake it with the information we have available.
     else:
         setter_params: List[ParameterDef] = []
         setter_params.append(ParameterDef("value", property_def.type_name, None))
         setter = MethodDef(property_def.setter, TypeName("void"), setter_params, None, None)
 
     ret_type = make_type(get_method_return_type(setter), state)
-    signature = make_method_signature(setter, True, True, True, state, False, False)
+    signature = make_method_signature(setter, True, True, True, state, False)
     return f"{ret_type} {signature}"
 
 
 def make_getter_signature(class_def: ClassDef, property_def: PropertyDef, state: State) -> str:
     if property_def.getter is None:
         return ""
 
@@ -1078,9 +1082,70 @@
         getter = class_def.methods[property_def.getter][0]
     # Otherwise we fake it with the information we have available.
     else:
         getter_params: List[ParameterDef] = []
         getter = MethodDef(property_def.getter, property_def.type_name, getter_params, None, None)
 
     ret_type = make_type(get_method_return_type(getter), state)
-    signature = make_method_signature(getter, True, True, True, state, False, False)
+    signature = make_method_signature(getter, True, True, True, state, False)
     return f"{ret_type} {signature}"
+
+
+def get_file_list(paths: List[str]) -> List[str]:
+    file_list: List[str] = []
+
+    for path in paths:
+        if os.path.isdir(path):
+            for root, subdirs, files in os.walk(path):
+                file_list += (os.path.join(root, filename) for filename in files if filename.endswith(".xml"))
+        elif os.path.isfile(path):
+            if not path.endswith(".xml"):
+                print(f'Got non-.xml file "{path}" in input, skipping.')
+                continue
+            file_list.append(path)
+
+    return file_list
+
+
+def read_xml_data(files: List[str]) -> Dict[str, Tuple[ET.Element, str]]:
+    classes: Dict[str, Tuple[ET.Element, str]] = {}
+    for cur_file in get_file_list(files):
+        tree = ET.parse(cur_file)
+        doc = tree.getroot()
+        name = doc.attrib["name"]
+        classes[name] = (doc, cur_file)
+
+    return classes
+
+
+def get_class_state_from_docs(paths: List[str]) -> State:
+    files: List[str] = get_file_list(paths)
+    classes: Dict[str, Tuple[ET.Element, str]] = read_xml_data(files)
+    state = State()
+    for name, data in classes.items():
+        try:
+            state.parse_class(data[0], data[1])
+        except Exception as e:
+            print_error(f"{name}.xml: Exception while parsing class: {e}", state)
+    return state
+
+
+def get_class_uid(class_def: ClassDef) -> str:
+    return class_def.name
+
+
+def get_signal_uid(signal_def: SignalDef, class_def: ClassDef, state: State) -> str:
+    signature_short = make_method_signature(signal_def, False, False, False, state, False)
+    return f"{get_class_uid(class_def)}.{signature_short}"
+
+
+def get_constant_uid(constant_def: ConstantDef, class_def: ClassDef) -> str:
+    return f"{get_class_uid(class_def)}.{constant_def.name}"
+
+
+def get_method_uid(method_def: Union[AnnotationDef, MethodDef, SignalDef], class_def: ClassDef, state: State) -> str:
+    signature_short = make_method_signature(method_def, False, False, False, state, True)
+    return f"{get_class_uid(class_def)}.{signature_short}"
+
+
+def get_theme_uid(theme_item_def: ThemeItemDef, class_def: ClassDef) -> str:
+    return f"{get_class_uid(class_def)}.{theme_item_def.name}"
```

### Comparing `gddoc2yml-0.1.1/src/gddoc2yml/make_rst.py` & `gddoc2yml-0.2.0/src/gddoc2yml/make_rst.py`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.1.1/src/gddoc2yml.egg-info/PKG-INFO` & `gddoc2yml-0.2.0/src/gddoc2yml.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gddoc2yml
-Version: 0.1.1
+Version: 0.2.0
 Summary: Convert godot xml docs to docfx yml
 Author-email: Nick Maltbie <nick.dmalt@gmail.com>
 Project-URL: Homepage, https://github.com/nicholas-maltbie/gddoc2yml
 Project-URL: Issues, https://github.com/nicholas-maltbie/gddoc2yml/issues
 Project-URL: GitHub, https://github.com/nicholas-maltbie/gddoc2yml
 Project-URL: Changelog, https://github.com/nicholas-maltbie/gddoc2yml/blob/main/CHANGELOG.md
 Keywords: godot,docfx,yml,xml,documentation
@@ -33,35 +33,44 @@
 
 Install gddoc2yml via pip
 
 ```bash
 python3 -m pip install gddoc2yml
 ```
 
-Then you will have the gdxml2yml command available:
+Then you will have the gdxml2yml and gdxml2xrefmap command available:
 
 <!-- markdownlint-disable MD013 -->
 
 ```bash
-gdxml2yml
-    usage: gdxml2yml [-h] [--filter FILTER] path [path ...] output
-    gdxml2yml: error: the following arguments are required: path, output
-
 gdxml2yml -h
     usage: gdxml2yml [-h] [--filter FILTER] path [path ...] output
 
     Convert godot documentation xml file to yml for docfx.
 
     positional arguments:
     path             A path to an XML file or a directory containing XML files to parse.
     output           output folder to store all generated yml files.
 
     options:
     -h, --help       show this help message and exit
     --filter FILTER  The filepath pattern for XML files to filter
+
+gdxml2xrefmap -h
+    usage: gdxml2xrefmap [-h] [--filter FILTER] path [path ...] output
+
+    Convert godot documentation xml files into a xrefmap compatible with DoxFx.
+
+    positional arguments:
+    path             A path to an XML file or a directory containing XML files to parse.
+    output           output path to store xrefmap.
+
+    options:
+    -h, --help       show this help message and exit
+    --filter FILTER  The filepath pattern for XML files to filter.
 ```
 
 <!-- markdownlint-enable MD013 -->
 
 ## Using gddoc2yml
 
 Export xml docs for your project with godot, us gdxml2yml to generate yml api,
@@ -103,14 +112,37 @@
     {
         "files": ["*.yml"],
         "src": "api",
         "dest": "api"
     },
     ```
 
+### Generating xrefmap for Godot Docs
+
+Included is an additional command, `gdxml2xrefmap` to generate
+an xrefmap for the godot docs.
+
+```bash
+gdxml2xrefmap godot/doc/classes godot/modules out/godot_xrefmap.yml
+```
+
+**Note** the build for this repo contains an xrefmap that points to godot's
+documentation. You can reference this in your `docfx.json` file as a `xref`
+like so:
+
+```json
+{
+  "build": {
+    "xref": [
+      "https://gddoc2yml.nickmaltbie.com/xrefmap/godot_xrefmap.yml"
+    ]
+  }
+}
+```
+
 ## References
 
 * [Godot -- CLI Reference](https://docs.godotengine.org/en/stable/tutorials/editor/command_line_tutorial.html#command-line-reference)
 * [Godot -- make_rst.py](https://github.com/godotengine/godot/blob/master/doc/tools/make_rst.py)
 * [DocFx -- Github](https://github.com/dotnet/docfx)
 * [DocFx -- Introduction to Multiple Languages Support](https://xxred.gitee.io/docfx/tutorial/universalreference/intro_multiple_langs_support.html)
 * [DocFx -- Custom Template](https://dotnet.github.io/docfx/docs/template.html?tabs=modern#custom-template)
@@ -186,12 +218,15 @@
 Build godot docs using latest gddoc2yml.
 
 ```bash
 # Install from repo
 python3 -m pip install .
 
 # Generate docs using gdxml2yml
-gdxml2yml godot/doc/classes godot/modules godot/platform/android/doc_classes doc/api
+gdxml2yml godot/doc/classes godot/modules godot/platform/android/doc_classes doc/godot/api
+
+# Generate xrefmap using gdxml2xrefmap
+gdxml2xrefmap godot/doc/classes godot/modules doc/xrefmap/godot_xrefmap.yml
 
 # Startup docfx website
 dotnet tool run docfx --serve doc/docfx.json
 ```
```

### Comparing `gddoc2yml-0.1.1/src/gddoc2yml.egg-info/SOURCES.txt` & `gddoc2yml-0.2.0/src/gddoc2yml.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/gddoc2yml/__init__.py
+src/gddoc2yml/gdxml2xrefmap.py
 src/gddoc2yml/gdxml2yml.py
 src/gddoc2yml/gdxml_helpers.py
 src/gddoc2yml/make_rst.py
 src/gddoc2yml/version.py
 src/gddoc2yml.egg-info/PKG-INFO
 src/gddoc2yml.egg-info/SOURCES.txt
 src/gddoc2yml.egg-info/dependency_links.txt
```

### Comparing `gddoc2yml-0.1.1/tests/classes/CollisionObject3D.xml` & `gddoc2yml-0.2.0/tests/classes/CollisionObject3D.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.1.1/tests/classes/Node.xml` & `gddoc2yml-0.2.0/tests/classes/Node.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.1.1/tests/classes/Node3D.xml` & `gddoc2yml-0.2.0/tests/classes/Node3D.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.1.1/tests/classes/Object.xml` & `gddoc2yml-0.2.0/tests/classes/Object.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.1.1/tests/classes/PhysicsBody3D.xml` & `gddoc2yml-0.2.0/tests/classes/PhysicsBody3D.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.1.1/tests/classes/StaticBody3D.xml` & `gddoc2yml-0.2.0/tests/classes/StaticBody3D.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.1.1/tests/classes/int.xml` & `gddoc2yml-0.2.0/tests/classes/int.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.1.1/tests/test_console.py` & `gddoc2yml-0.2.0/tests/test_console.py`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.1.1/tests/test_gdxml2yml.py` & `gddoc2yml-0.2.0/tests/test_gdxml2yml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import os
 import tempfile
 import shutil
 import unittest
 
 from importlib.resources import files
-from src.gddoc2yml import gdxml2yml
+from src.gddoc2yml import gdxml_helpers
 from src.gddoc2yml.make_rst import State
 
 
 class MyTestCase1(unittest.TestCase):
     def test_class_yml_from_state(self):
         # Program expects files to be read from path location, not package
         # Setup temporary directory with xml docs
         xml_docs = [f for f in files("tests").joinpath("classes").iterdir() if f.is_file() and f.name.endswith(".xml")]
         with tempfile.TemporaryDirectory() as tmpdirname:
             for xml_doc in xml_docs:
                 shutil.copyfile(xml_doc, os.path.join(tmpdirname, xml_doc.name))
 
-            state: State = gdxml2yml._get_class_state_from_docs([tmpdirname])
+            state: State = gdxml_helpers.get_class_state_from_docs([tmpdirname])
             xml_files = [f for f in os.listdir(tmpdirname) if f.endswith(".xml")]
 
             assert len(xml_files) > 0
             assert len(state.classes) == len(xml_files)
 
 
 if __name__ == '__main__':
```

