# Comparing `tmp/fig2sketch-0.2.9.tar.gz` & `tmp/fig2sketch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fig2sketch-0.2.9.tar", last modified: Fri Mar  1 16:23:36 2024, max compression
+gzip compressed data, was "fig2sketch-0.3.0.tar", last modified: Thu May 16 15:25:49 2024, max compression
```

## Comparing `fig2sketch-0.2.9.tar` & `fig2sketch-0.3.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:36.539939 fig2sketch-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-03-01 16:23:36.535939 fig2sketch-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 16:23:36.539939 fig2sketch-0.2.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:36.527939 fig2sketch-0.2.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:36.531939 fig2sketch-0.2.9/src/converter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/artboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/document.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/font.py
--rw-r--r--   0 runner    (1001) docker     (127)    34002 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/font_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/positioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/prototype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/shape.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/shape_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/shape_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/slice.py
--rw-r--r--   0 runner    (1001) docker     (127)    12979 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/converter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:36.535939 fig2sketch-0.2.9/src/fig2sketch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-03-01 16:23:36.000000 fig2sketch-0.2.9/src/fig2sketch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-01 16:23:36.000000 fig2sketch-0.2.9/src/fig2sketch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 16:23:36.000000 fig2sketch-0.2.9/src/fig2sketch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-01 16:23:36.000000 fig2sketch-0.2.9/src/fig2sketch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-01 16:23:36.000000 fig2sketch-0.2.9/src/fig2sketch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-01 16:23:36.000000 fig2sketch-0.2.9/src/fig2sketch.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3382 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/fig2sketch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:36.535939 fig2sketch-0.2.9/src/figformat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/figformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/figformat/decodefig.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/figformat/fig2tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/figformat/kiwi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/figformat/vector_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:36.535939 fig2sketch-0.2.9/src/sketchformat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/layer_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/layer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/layer_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/prototype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:23:36.535939 fig2sketch-0.2.9/src/sketchformat/serialize/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/serialize/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/serialize/orjson.py
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-03-01 16:23:30.000000 fig2sketch-0.2.9/src/sketchformat/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:49.288202 fig2sketch-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-16 15:25:49.288202 fig2sketch-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:25:49.288202 fig2sketch-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:49.280202 fig2sketch-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:49.284202 fig2sketch-0.3.0/src/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/artboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/font.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34002 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/font_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/positioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/prototype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/shape_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/shape_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12979 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:49.288202 fig2sketch-0.3.0/src/fig2sketch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-16 15:25:49.000000 fig2sketch-0.3.0/src/fig2sketch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-16 15:25:49.000000 fig2sketch-0.3.0/src/fig2sketch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:25:49.000000 fig2sketch-0.3.0/src/fig2sketch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 15:25:49.000000 fig2sketch-0.3.0/src/fig2sketch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-16 15:25:49.000000 fig2sketch-0.3.0/src/fig2sketch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 15:25:49.000000 fig2sketch-0.3.0/src/fig2sketch.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3382 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/fig2sketch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:49.284202 fig2sketch-0.3.0/src/figformat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/figformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/figformat/decodefig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/figformat/fig2tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/figformat/kiwi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/figformat/vector_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:49.288202 fig2sketch-0.3.0/src/sketchformat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/layer_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/layer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/layer_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/prototype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:49.288202 fig2sketch-0.3.0/src/sketchformat/serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/serialize/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/serialize/orjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/text.py
```

### Comparing `fig2sketch-0.2.9/LICENSE` & `fig2sketch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/PKG-INFO` & `fig2sketch-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fig2sketch
-Version: 0.2.9
+Version: 0.3.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Pillow==9.3.0
-Requires-Dist: fonttools==4.38.0
+Requires-Dist: Pillow==10.3.0
+Requires-Dist: fonttools==4.43.0
 Requires-Dist: appdirs==1.4.4
 Provides-Extra: fast
 Requires-Dist: fig-kiwi==0.1.0; extra == "fast"
 Provides-Extra: dev
 Requires-Dist: black==24.2.0; extra == "dev"
 Requires-Dist: mypy==0.991; extra == "dev"
-Requires-Dist: pytest==7.2.0; extra == "dev"
+Requires-Dist: pytest==8.2.0; extra == "dev"
 Requires-Dist: fig-kiwi==0.1.0; extra == "dev"
 
 # .fig to Sketch converter
 
 fig2sketch is a command line tool that converts .fig files into Sketch design documents (.sketch), which can then be opened with [Sketch](https://www.sketch.com/) applications.
 
 ## How it works
```

### Comparing `fig2sketch-0.2.9/README.md` & `fig2sketch-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/pyproject.toml` & `fig2sketch-0.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [project]
 name = "fig2sketch"
 readme = "README.md"
 requires-python = ">=3.10"
 dynamic = ["version"]
-dependencies = ["Pillow==9.3.0", "fonttools==4.38.0", "appdirs==1.4.4"]
+dependencies = ["Pillow==10.3.0", "fonttools==4.43.0", "appdirs==1.4.4"]
 
 [project.scripts]
 fig2sketch = "fig2sketch:main"
 
 [build-system]
 requires = ["setuptools>=41", "setuptools-git-versioning<2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools-git-versioning]
 enabled = true
 
 [project.optional-dependencies]
 fast = ["fig-kiwi==0.1.0"]
-dev = ["black==24.2.0", "mypy==0.991", "pytest==7.2.0", "fig-kiwi==0.1.0"]
+dev = ["black==24.2.0", "mypy==0.991", "pytest==8.2.0", "fig-kiwi==0.1.0"]
 
 [tool.black]
 line-length = 99
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
```

### Comparing `fig2sketch-0.2.9/src/converter/artboard.py` & `fig2sketch-0.3.0/src/converter/artboard.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/base.py` & `fig2sketch-0.3.0/src/converter/base.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/component.py` & `fig2sketch-0.3.0/src/converter/component.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/context.py` & `fig2sketch-0.3.0/src/converter/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from urllib.error import HTTPError
 from . import component, page, font
 from sketchformat.document import Swatch
 from typing import Sequence, Tuple, Optional, Dict, IO, List
 
 
 def find_symbols(node: dict) -> List[Sequence[int]]:
     if node["type"] == "SYMBOL":
@@ -12,27 +13,33 @@
     for child in node.get("children", []):
         found += find_symbols(child)
 
     return found
 
 
 class Context:
-    def init(self, components_page: Optional[dict], id_map: Dict[Sequence[int], dict]) -> None:
+    def init(
+        self, components_page: Optional[dict], id_map: Dict[Sequence[int], dict], color_space: str
+    ) -> None:
+        self._color_space = color_space
         self._sketch_components: Dict[Sequence[int], Swatch] = {}
         self.symbols_page = None
         self._node_by_id = id_map
         self._used_fonts: Dict[Tuple[str, str], Tuple[IO[bytes], str]] = {}
         self._component_symbols = (
             {s: False for s in find_symbols(components_page)} if components_page else {}
         )
 
         # Where to position symbols of the specified width
         # width -> (x, y)
         self._symbol_position = {0: [0, 0]}
 
+    def color_space(self) -> int:
+        return 2 if self._color_space == "DISPLAY_P3" else 1
+
     def component(self, cid: Sequence[int]) -> Tuple[dict, Optional[Swatch]]:
         fig_component = self.fig_node(cid)
 
         # See if we can convert this component to a Sketch swatch
         sketch_component = self._sketch_components.get(cid)
         if not sketch_component:
             sketch_component = component.convert(fig_component)
@@ -58,16 +65,22 @@
         font_descriptor = (fig_font_name["family"], fig_font_name["style"])
         font_info = self._used_fonts.get(font_descriptor)
         if font_info:
             return font_info[1]
 
         try:
             font_file, font_name = font.get_webfont(*font_descriptor)
-        except:
-            logging.warning(f"Could not download font {font_descriptor}")
+        except Exception as e:
+            if isinstance(e, font.FontNotFoundError) or (
+                isinstance(e, HTTPError) and e.code == 404
+            ):
+                logging.warning(f"Could not find font {font_descriptor} via Google Fonts")
+            else:
+                logging.warning(f"Could not download font {font_descriptor}: {e}")
+
             font_file = None
             if fig_font_name["postscript"]:
                 font_name = fig_font_name["postscript"]
             else:
                 font_name = f"{fig_font_name['family']}-{fig_font_name['style']}"
 
         self._used_fonts[font_descriptor] = (font_file, font_name)
```

### Comparing `fig2sketch-0.2.9/src/converter/convert.py` & `fig2sketch-0.3.0/src/converter/convert.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,20 @@
     fig: dict, id_map: Dict[Sequence[int], dict], output: zipfile.ZipFile
 ) -> None:
     fig_pages, components_page = separate_pages(fig["document"]["children"])
 
     # We should either bring the fonts to the same indexed_components to pass
     # them as parameter or move the indexed components to the component file
     # and store there the components, for consistency purposes
-    context.init(components_page, id_map)
+    if "documentColorProfile" in fig["document"]:
+        color_space = fig["document"]["documentColorProfile"]
+    else:
+        color_space = "sRGB"
+
+    context.init(components_page, id_map, color_space)
 
     # Convert all normal pages
     sketch_pages: List[Page] = convert_pages(fig_pages, output)
 
     sketch_document = document.convert(sketch_pages, output)
     sketch_user = user.convert(sketch_pages)
     sketch_meta = meta.convert(sketch_pages)
```

### Comparing `fig2sketch-0.2.9/src/converter/document.py` & `fig2sketch-0.3.0/src/converter/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             "colorAssets": [],
             "gradientAssets": [],
             "images": [],
             "colors": [],
             "gradients": [],
             "exportPresets": [],
         },
-        "colorSpace": 1,
+        "colorSpace": context.color_space(),
         "currentPageIndex": 0,
         "foreignLayerStyles": [],
         "foreignSymbols": [],
         "foreignTextStyles": [],
         "foreignSwatches": [],
         "layerStyles": {
             "_class": "sharedStyleContainer",
```

### Comparing `fig2sketch-0.2.9/src/converter/font.py` & `fig2sketch-0.3.0/src/converter/font.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 import appdirs
 import os
 import urllib.request
 import urllib.parse
+import json
+import logging
 from converter import utils
 from fontTools.ttLib import TTFont
 from sketchformat.document import FontReference, JsonFileReference
 from typing import IO, Tuple
 from zipfile import ZipFile
 
 fonts_cache_dir = appdirs.user_cache_dir("Fig2Sketch", "Sketch") + "/fonts"
 os.makedirs(fonts_cache_dir, exist_ok=True)
 
 
-class FontError(Exception):
+class FontNotFoundError(Exception):
     pass
 
 
-def retrieve_webfont(family):
-    WEB_FONT_BASE_URL = "http://fonts.google.com/download?family="
-    font_url = WEB_FONT_BASE_URL + urllib.parse.quote(family)
-    font_file = f"{fonts_cache_dir}/{family}.zip"
-
-    if not os.path.exists(font_file):
-        urllib.request.urlretrieve(font_url, font_file)
-
-    return ZipFile(font_file)
+def retrieve_webfont_family(family):
+    WEB_FONT_LIST_URL = "https://fonts.google.com/download/list?family="
+    list_url = WEB_FONT_LIST_URL + urllib.parse.quote(family)
+    list_response = urllib.request.urlopen(list_url)
+    return json.loads(bytearray(list_response.read())[5:])
 
 
 def get_webfont(family, subfamily):
-    font_zip = retrieve_webfont(family)
-    for fi in font_zip.infolist():
-        if not fi.filename.endswith((".ttf", ".otf")):
+    family_list = retrieve_webfont_family(family)
+
+    for fi in family_list["manifest"]["fileRefs"]:
+        filename = fi["filename"].replace("static/", "")
+        if not filename.endswith((".ttf", ".otf")):
             continue
+        if family.lower() in filename.lower() and subfamily.lower() in filename.lower():
+            font_file_path = f"{fonts_cache_dir}/{filename}"
+            if not os.path.exists(font_file_path):
+                urllib.request.urlretrieve(fi["url"], font_file_path)
+
+            font_file = open(font_file_path, "rb")
+            font_names = extract_names(font_file)
 
-        font_file = font_zip.open(fi.filename, "r")
-        font_names = extract_names(font_file)
-        if (
-            font_names["family"].lower() == family.lower()
-            and font_names["subfamily"].lower() == subfamily.lower()
-        ):
-            font_file.seek(0)
             return font_file, font_names["postscript"]
 
-    raise FontError(f"Could not find font {family} {subfamily}")
+    raise FontNotFoundError(f"Could not find font {family} {subfamily}")
 
 
 def convert(
     name: Tuple[str, str], font_file: IO[bytes], postscript: str, output_zip: ZipFile
 ) -> FontReference:
     family, subfamily = name
     data = font_file.read()
```

### Comparing `fig2sketch-0.2.9/src/converter/font_features.py` & `fig2sketch-0.3.0/src/converter/font_features.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/group.py` & `fig2sketch-0.3.0/src/converter/group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/instance.py` & `fig2sketch-0.3.0/src/converter/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import copy
+import copy, logging
 from . import base, group
 from .context import context
 from .config import config
 from converter import utils
 from sketchformat.layer_group import SymbolInstance, OverrideValue
 from sketchformat.style import Style
 from typing import List, Tuple
@@ -216,15 +216,19 @@
 
 
 def find_refs(node, ref_id):
     """Find all usages of a property in a symbol, recursively"""
     refs = [
         (ref, node.get("overrideKey", node["guid"]))
         for ref in node.get("componentPropRefs", [])
-        if ref["defID"] == ref_id and not ref.get("isDeleted", False)
+        if (
+            ("defID" in ref and ref["defID"] == ref_id)
+            or ("zombieFallbackName" in ref and ref["zombieFallbackName"] == ref_id)
+        )
+        and not ref.get("isDeleted", False)
     ]
 
     for ch in node.get("children", []):
         refs += find_refs(ch, ref_id)
 
     return refs
```

### Comparing `fig2sketch-0.2.9/src/converter/meta.py` & `fig2sketch-0.3.0/src/converter/meta.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/page.py` & `fig2sketch-0.3.0/src/converter/page.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/positioning.py` & `fig2sketch-0.3.0/src/converter/positioning.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/prototype.py` & `fig2sketch-0.3.0/src/converter/prototype.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/rectangle.py` & `fig2sketch-0.3.0/src/converter/rectangle.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/shape_group.py` & `fig2sketch-0.3.0/src/converter/shape_group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/shape_path.py` & `fig2sketch-0.3.0/src/converter/shape_path.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/style.py` & `fig2sketch-0.3.0/src/converter/style.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/symbol.py` & `fig2sketch-0.3.0/src/converter/symbol.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/text.py` & `fig2sketch-0.3.0/src/converter/text.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/tree.py` & `fig2sketch-0.3.0/src/converter/tree.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/user.py` & `fig2sketch-0.3.0/src/converter/user.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/converter/utils.py` & `fig2sketch-0.3.0/src/converter/utils.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/fig2sketch.egg-info/PKG-INFO` & `fig2sketch-0.3.0/src/fig2sketch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fig2sketch
-Version: 0.2.9
+Version: 0.3.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Pillow==9.3.0
-Requires-Dist: fonttools==4.38.0
+Requires-Dist: Pillow==10.3.0
+Requires-Dist: fonttools==4.43.0
 Requires-Dist: appdirs==1.4.4
 Provides-Extra: fast
 Requires-Dist: fig-kiwi==0.1.0; extra == "fast"
 Provides-Extra: dev
 Requires-Dist: black==24.2.0; extra == "dev"
 Requires-Dist: mypy==0.991; extra == "dev"
-Requires-Dist: pytest==7.2.0; extra == "dev"
+Requires-Dist: pytest==8.2.0; extra == "dev"
 Requires-Dist: fig-kiwi==0.1.0; extra == "dev"
 
 # .fig to Sketch converter
 
 fig2sketch is a command line tool that converts .fig files into Sketch design documents (.sketch), which can then be opened with [Sketch](https://www.sketch.com/) applications.
 
 ## How it works
```

### Comparing `fig2sketch-0.2.9/src/fig2sketch.egg-info/SOURCES.txt` & `fig2sketch-0.3.0/src/fig2sketch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/fig2sketch.py` & `fig2sketch-0.3.0/src/fig2sketch.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/figformat/decodefig.py` & `fig2sketch-0.3.0/src/figformat/decodefig.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/figformat/fig2tree.py` & `fig2sketch-0.3.0/src/figformat/fig2tree.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/figformat/kiwi.py` & `fig2sketch-0.3.0/src/figformat/kiwi.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/figformat/vector_network.py` & `fig2sketch-0.3.0/src/figformat/vector_network.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/sketchformat/common.py` & `fig2sketch-0.3.0/src/sketchformat/common.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/sketchformat/document.py` & `fig2sketch-0.3.0/src/sketchformat/document.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/sketchformat/layer_common.py` & `fig2sketch-0.3.0/src/sketchformat/layer_common.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/sketchformat/layer_group.py` & `fig2sketch-0.3.0/src/sketchformat/layer_group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/sketchformat/layer_shape.py` & `fig2sketch-0.3.0/src/sketchformat/layer_shape.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/sketchformat/prototype.py` & `fig2sketch-0.3.0/src/sketchformat/prototype.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/sketchformat/serialize/json.py` & `fig2sketch-0.3.0/src/sketchformat/serialize/json.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/sketchformat/serialize/orjson.py` & `fig2sketch-0.3.0/src/sketchformat/serialize/orjson.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/sketchformat/style.py` & `fig2sketch-0.3.0/src/sketchformat/style.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.9/src/sketchformat/text.py` & `fig2sketch-0.3.0/src/sketchformat/text.py`

 * *Files identical despite different names*

