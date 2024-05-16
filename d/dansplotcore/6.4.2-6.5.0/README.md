# Comparing `tmp/dansplotcore-6.4.2.tar.gz` & `tmp/dansplotcore-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dansplotcore-6.4.2.tar", last modified: Tue May 14 22:57:22 2024, max compression
+gzip compressed data, was "dansplotcore-6.5.0.tar", last modified: Thu May 16 21:56:10 2024, max compression
```

## Comparing `dansplotcore-6.4.2.tar` & `dansplotcore-6.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-14 22:57:22.189026 dansplotcore-6.4.2/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-05-14 22:57:22.189026 dansplotcore-6.4.2/PKG-INFO
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-14 22:57:22.189026 dansplotcore-6.4.2/dansplotcore/
--rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.4.2/dansplotcore/__init__.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     5030 2024-05-14 22:54:52.000000 dansplotcore-6.4.2/dansplotcore/media.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     9713 2024-05-13 23:40:36.000000 dansplotcore-6.4.2/dansplotcore/plot.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.4.2/dansplotcore/primitives.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2234 2024-05-14 19:17:01.000000 dansplotcore-6.4.2/dansplotcore/process.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     9735 2024-05-14 22:54:33.000000 dansplotcore-6.4.2/dansplotcore/show.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.4.2/dansplotcore/transforms.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     7455 2024-04-02 20:00:09.000000 dansplotcore-6.4.2/dansplotcore/vector_text.py
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-14 22:57:22.189026 dansplotcore-6.4.2/dansplotcore.egg-info/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-05-14 22:57:22.000000 dansplotcore-6.4.2/dansplotcore.egg-info/PKG-INFO
--rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-05-14 22:57:22.000000 dansplotcore-6.4.2/dansplotcore.egg-info/SOURCES.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-05-14 22:57:22.000000 dansplotcore-6.4.2/dansplotcore.egg-info/dependency_links.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-05-14 22:57:22.000000 dansplotcore-6.4.2/dansplotcore.egg-info/requires.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-05-14 22:57:22.000000 dansplotcore-6.4.2/dansplotcore.egg-info/top_level.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-05-14 22:57:22.189026 dansplotcore-6.4.2/setup.cfg
--rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-05-14 22:56:26.000000 dansplotcore-6.4.2/setup.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-16 21:56:10.312446 dansplotcore-6.5.0/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-05-16 21:56:10.312446 dansplotcore-6.5.0/PKG-INFO
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-16 21:56:10.312446 dansplotcore-6.5.0/dansplotcore/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.5.0/dansplotcore/__init__.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     5030 2024-05-14 22:54:52.000000 dansplotcore-6.5.0/dansplotcore/media.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     9713 2024-05-13 23:40:36.000000 dansplotcore-6.5.0/dansplotcore/plot.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.5.0/dansplotcore/primitives.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2234 2024-05-14 19:17:01.000000 dansplotcore-6.5.0/dansplotcore/process.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)    10016 2024-05-16 21:54:43.000000 dansplotcore-6.5.0/dansplotcore/show.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.5.0/dansplotcore/transforms.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     7455 2024-04-02 20:00:09.000000 dansplotcore-6.5.0/dansplotcore/vector_text.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-16 21:56:10.312446 dansplotcore-6.5.0/dansplotcore.egg-info/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-05-16 21:56:10.000000 dansplotcore-6.5.0/dansplotcore.egg-info/PKG-INFO
+-rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-05-16 21:56:10.000000 dansplotcore-6.5.0/dansplotcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-05-16 21:56:10.000000 dansplotcore-6.5.0/dansplotcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-05-16 21:56:10.000000 dansplotcore-6.5.0/dansplotcore.egg-info/requires.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-05-16 21:56:10.000000 dansplotcore-6.5.0/dansplotcore.egg-info/top_level.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-05-16 21:56:10.312446 dansplotcore-6.5.0/setup.cfg
+-rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-05-16 21:55:43.000000 dansplotcore-6.5.0/setup.py
```

### Comparing `dansplotcore-6.4.2/dansplotcore/media.py` & `dansplotcore-6.5.0/dansplotcore/media.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.4.2/dansplotcore/plot.py` & `dansplotcore-6.5.0/dansplotcore/plot.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.4.2/dansplotcore/primitives.py` & `dansplotcore-6.5.0/dansplotcore/primitives.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.4.2/dansplotcore/process.py` & `dansplotcore-6.5.0/dansplotcore/process.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.4.2/dansplotcore/show.py` & `dansplotcore-6.5.0/dansplotcore/show.py`

 * *Files 5% similar despite different names*

```diff
@@ -136,14 +136,19 @@
         view.x += x/media.width () * (view.w - new_view_w)
         view.y += y/media.height() * (view.h - new_view_h)
         view.w = new_view_w
         view.h = new_view_h
         media.view_set(*view.tuple())
         if plot.late_vertexors:
             construct(plot, view, media.width(), media.height())
+    def square(view):
+        view.w = view.h * media.width() / media.height()
+        media.view_set(*view.tuple())
+        if plot.late_vertexors:
+            construct(plot, view, media.width(), media.height())
     reset()
     construct(plot, view, w, h)
     def on_resize(w, h):
         zoom(view, w/media.width(), h/media.height(), w/2, h/2)
         if plot.late_vertexors:
             construct(plot, view, media.width(), media.height())
     def on_mouse_drag(dx, dy):
@@ -172,14 +177,17 @@
             return
         if key == ' ':
             reset()
             return
         if key == 'Return':
             media.capture()
             return
+        if key == 'x':
+            square(view)
+            return
     def on_draw():
         media.clear()
         plot.buffer.draw()
         margin_x = 5.0 / media.width()  * view.w
         margin_y = 5.0 / media.height() * view.h
         # draw texts
         texter = media.Texter()
```

### Comparing `dansplotcore-6.4.2/dansplotcore/transforms.py` & `dansplotcore-6.5.0/dansplotcore/transforms.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.4.2/dansplotcore/vector_text.py` & `dansplotcore-6.5.0/dansplotcore/vector_text.py`

 * *Files identical despite different names*

