# Comparing `tmp/fig2sketch-0.2.8.tar.gz` & `tmp/fig2sketch-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fig2sketch-0.2.8.tar", last modified: Fri Mar  1 10:34:48 2024, max compression
+gzip compressed data, was "fig2sketch-0.2.9.tar", last modified: Fri Mar  1 16:23:36 2024, max compression
```

## Comparing `fig2sketch-0.2.8.tar` & `fig2sketch-0.2.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:34:48.872708 fig2sketch-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-03-01 10:34:48.872708 fig2sketch-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 10:34:48.872708 fig2sketch-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:34:48.864708 fig2sketch-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:34:48.864708 fig2sketch-0.2.8/src/converter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/artboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/document.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/font.py
--rw-r--r--   0 runner    (1001) docker     (127)    34002 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/font_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/positioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/prototype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/shape.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/shape_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/shape_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/slice.py
--rw-r--r--   0 runner    (1001) docker     (127)    12979 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/converter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:34:48.868708 fig2sketch-0.2.8/src/fig2sketch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-03-01 10:34:48.000000 fig2sketch-0.2.8/src/fig2sketch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-01 10:34:48.000000 fig2sketch-0.2.8/src/fig2sketch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 10:34:48.000000 fig2sketch-0.2.8/src/fig2sketch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-01 10:34:48.000000 fig2sketch-0.2.8/src/fig2sketch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-01 10:34:48.000000 fig2sketch-0.2.8/src/fig2sketch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-01 10:34:48.000000 fig2sketch-0.2.8/src/fig2sketch.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3382 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/fig2sketch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:34:48.868708 fig2sketch-0.2.8/src/figformat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/figformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/figformat/decodefig.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/figformat/fig2tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/figformat/kiwi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/figformat/vector_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:34:48.868708 fig2sketch-0.2.8/src/sketchformat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/sketchformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/sketchformat/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/sketchformat/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/sketchformat/layer_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/sketchformat/layer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/sketchformat/layer_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/sketchformat/prototype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:34:48.868708 fig2sketch-0.2.8/src/sketchformat/serialize/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/sketchformat/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/sketchformat/serialize/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/sketchformat/serialize/orjson.py
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/sketchformat/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-03-01 10:34:41.000000 fig2sketch-0.2.8/src/sketchformat/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:36.539939 fig2sketch-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-03-01 16:23:36.535939 fig2sketch-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 16:23:36.539939 fig2sketch-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:36.527939 fig2sketch-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:36.531939 fig2sketch-0.2.9/src/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/artboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/font.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34002 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/font_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/positioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/prototype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/shape_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/shape_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12979 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:36.535939 fig2sketch-0.2.9/src/fig2sketch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-03-01 16:23:36.000000 fig2sketch-0.2.9/src/fig2sketch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-01 16:23:36.000000 fig2sketch-0.2.9/src/fig2sketch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 16:23:36.000000 fig2sketch-0.2.9/src/fig2sketch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-01 16:23:36.000000 fig2sketch-0.2.9/src/fig2sketch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-01 16:23:36.000000 fig2sketch-0.2.9/src/fig2sketch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-01 16:23:36.000000 fig2sketch-0.2.9/src/fig2sketch.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3382 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/fig2sketch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:36.535939 fig2sketch-0.2.9/src/figformat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/figformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/figformat/decodefig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/figformat/fig2tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/figformat/kiwi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/figformat/vector_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:36.535939 fig2sketch-0.2.9/src/sketchformat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/layer_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/layer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/layer_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/prototype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:36.535939 fig2sketch-0.2.9/src/sketchformat/serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/serialize/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/serialize/orjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/text.py
```

### Comparing `fig2sketch-0.2.8/LICENSE` & `fig2sketch-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/PKG-INFO` & `fig2sketch-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fig2sketch
-Version: 0.2.8
+Version: 0.2.9
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Pillow==9.3.0
 Requires-Dist: fonttools==4.38.0
 Requires-Dist: appdirs==1.4.4
 Provides-Extra: fast
```

### Comparing `fig2sketch-0.2.8/README.md` & `fig2sketch-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/pyproject.toml` & `fig2sketch-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/artboard.py` & `fig2sketch-0.2.9/src/converter/artboard.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/base.py` & `fig2sketch-0.2.9/src/converter/base.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/component.py` & `fig2sketch-0.2.9/src/converter/component.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/context.py` & `fig2sketch-0.2.9/src/converter/context.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/convert.py` & `fig2sketch-0.2.9/src/converter/convert.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/document.py` & `fig2sketch-0.2.9/src/converter/document.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/font.py` & `fig2sketch-0.2.9/src/converter/font.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/font_features.py` & `fig2sketch-0.2.9/src/converter/font_features.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/group.py` & `fig2sketch-0.2.9/src/converter/group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/instance.py` & `fig2sketch-0.2.9/src/converter/instance.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/meta.py` & `fig2sketch-0.2.9/src/converter/meta.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/page.py` & `fig2sketch-0.2.9/src/converter/page.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/positioning.py` & `fig2sketch-0.2.9/src/converter/positioning.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/prototype.py` & `fig2sketch-0.2.9/src/converter/prototype.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/rectangle.py` & `fig2sketch-0.2.9/src/converter/rectangle.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/shape_group.py` & `fig2sketch-0.2.9/src/converter/shape_group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/shape_path.py` & `fig2sketch-0.2.9/src/converter/shape_path.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/style.py` & `fig2sketch-0.2.9/src/converter/style.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/symbol.py` & `fig2sketch-0.2.9/src/converter/symbol.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/text.py` & `fig2sketch-0.2.9/src/converter/text.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/tree.py` & `fig2sketch-0.2.9/src/converter/tree.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/user.py` & `fig2sketch-0.2.9/src/converter/user.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/converter/utils.py` & `fig2sketch-0.2.9/src/converter/utils.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/fig2sketch.egg-info/PKG-INFO` & `fig2sketch-0.2.9/src/fig2sketch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fig2sketch
-Version: 0.2.8
+Version: 0.2.9
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Pillow==9.3.0
 Requires-Dist: fonttools==4.38.0
 Requires-Dist: appdirs==1.4.4
 Provides-Extra: fast
```

### Comparing `fig2sketch-0.2.8/src/fig2sketch.egg-info/SOURCES.txt` & `fig2sketch-0.2.9/src/fig2sketch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/fig2sketch.py` & `fig2sketch-0.2.9/src/fig2sketch.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/figformat/decodefig.py` & `fig2sketch-0.2.9/src/figformat/decodefig.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/figformat/fig2tree.py` & `fig2sketch-0.2.9/src/figformat/fig2tree.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/figformat/kiwi.py` & `fig2sketch-0.2.9/src/figformat/kiwi.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/figformat/vector_network.py` & `fig2sketch-0.2.9/src/figformat/vector_network.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/sketchformat/common.py` & `fig2sketch-0.2.9/src/sketchformat/common.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/sketchformat/document.py` & `fig2sketch-0.2.9/src/sketchformat/document.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/sketchformat/layer_common.py` & `fig2sketch-0.2.9/src/sketchformat/layer_common.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/sketchformat/layer_group.py` & `fig2sketch-0.2.9/src/sketchformat/layer_group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/sketchformat/layer_shape.py` & `fig2sketch-0.2.9/src/sketchformat/layer_shape.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/sketchformat/prototype.py` & `fig2sketch-0.2.9/src/sketchformat/prototype.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/sketchformat/serialize/json.py` & `fig2sketch-0.2.9/src/sketchformat/serialize/json.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/sketchformat/serialize/orjson.py` & `fig2sketch-0.2.9/src/sketchformat/serialize/orjson.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/sketchformat/style.py` & `fig2sketch-0.2.9/src/sketchformat/style.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.8/src/sketchformat/text.py` & `fig2sketch-0.2.9/src/sketchformat/text.py`

 * *Files identical despite different names*

