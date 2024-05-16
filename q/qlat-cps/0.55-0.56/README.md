# Comparing `tmp/qlat_cps-0.55.tar.gz` & `tmp/qlat_cps-0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlat_cps-0.55.tar", last modified: Sun Mar 10 05:28:54 2024, max compression
+gzip compressed data, was "qlat_cps-0.56.tar", last modified: Wed Mar 13 22:33:23 2024, max compression
```

## Comparing `qlat_cps-0.55.tar` & `qlat_cps-0.56.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-rw-r--   0        0        0       42 2024-03-10 05:23:56.000000 qlat_cps-0.55/README.md
--rw-rw-r--   0        0        0     1393 2024-03-10 05:23:56.000000 qlat_cps-0.55/depend-cps/meson.build
--rw-rw-r--   0        0        0     2508 2024-03-10 05:23:56.000000 qlat_cps-0.55/depend-qlat/meson.build
--rw-r--r--   0        0        0     1010 2024-03-10 05:23:56.000000 qlat_cps-0.55/meson.build
--rw-rw-r--   0        0        0      532 2024-03-10 05:23:56.000000 qlat_cps-0.55/pyproject.toml
--rw-rw-r--   0        0        0        0 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/__init__.pxd
--rw-rw-r--   0        0        0      117 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/__init__.py
--rw-rw-r--   0        0        0      316 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/__main__.py
--rw-rw-r--   0        0        0       70 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/all.pxd
--rw-rw-r--   0        0        0      496 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/c.py
--rw-rw-r--   0        0        0       67 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/cp.pxd
--rw-rw-r--   0        0        0      809 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/cp.pyx
--rw-rw-r--   0        0        0      466 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/everything.pxd
--rw-rw-r--   0        0        0     1146 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/get_include_dir.py
--rw-rw-r--   0        0        0       54 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/include/meson.build
--rw-rw-r--   0        0        0      145 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/include/qlat-cps/meson.build
--rw-rw-r--   0        0        0      413 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/include/qlat-cps/qlat-cps.h
--rw-rw-r--   0        0        0       44 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/init.py
--rw-rw-r--   0        0        0      570 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/lib/init.cpp
--rw-rw-r--   0        0        0      323 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/lib/meson.build
--rw-rw-r--   0        0        0     2041 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/lib/prop.cpp
--rw-rw-r--   0        0        0      545 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/meson.build
--rw-rw-r--   0        0        0       58 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/prop.py
--rw-rw-r--   0        0        0      105 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/scripts/meson.build
--rw-rw-r--   0        0        0      749 2024-03-10 05:23:56.000000 qlat_cps-0.55/qlat_cps/scripts/qlat_cps_config.py
--rw-r--r--   0        0        0      309 2024-03-10 05:28:54.612616 qlat_cps-0.55/PKG-INFO
+-rw-rw-r--   0        0        0       42 2024-03-13 22:07:50.000000 qlat_cps-0.56/README.md
+-rw-rw-r--   0        0        0     1393 2024-03-13 22:07:50.000000 qlat_cps-0.56/depend-cps/meson.build
+-rw-rw-r--   0        0        0     2508 2024-03-13 22:07:50.000000 qlat_cps-0.56/depend-qlat/meson.build
+-rw-r--r--   0        0        0     1010 2024-03-13 22:07:50.000000 qlat_cps-0.56/meson.build
+-rw-rw-r--   0        0        0      532 2024-03-13 22:07:50.000000 qlat_cps-0.56/pyproject.toml
+-rw-rw-r--   0        0        0        0 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/__init__.pxd
+-rw-rw-r--   0        0        0      117 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/__init__.py
+-rw-rw-r--   0        0        0      316 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/__main__.py
+-rw-rw-r--   0        0        0       70 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/all.pxd
+-rw-rw-r--   0        0        0      496 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/c.py
+-rw-rw-r--   0        0        0       67 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/cp.pxd
+-rw-rw-r--   0        0        0      809 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/cp.pyx
+-rw-rw-r--   0        0        0      466 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/everything.pxd
+-rw-rw-r--   0        0        0     1146 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/get_include_dir.py
+-rw-rw-r--   0        0        0       54 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/include/meson.build
+-rw-rw-r--   0        0        0      145 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/include/qlat-cps/meson.build
+-rw-rw-r--   0        0        0      413 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/include/qlat-cps/qlat-cps.h
+-rw-rw-r--   0        0        0       44 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/init.py
+-rw-rw-r--   0        0        0      570 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/lib/init.cpp
+-rw-rw-r--   0        0        0      323 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/lib/meson.build
+-rw-rw-r--   0        0        0     2041 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/lib/prop.cpp
+-rw-rw-r--   0        0        0      545 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/meson.build
+-rw-rw-r--   0        0        0       58 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/prop.py
+-rw-rw-r--   0        0        0      105 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/scripts/meson.build
+-rw-rw-r--   0        0        0      749 2024-03-13 22:07:50.000000 qlat_cps-0.56/qlat_cps/scripts/qlat_cps_config.py
+-rw-r--r--   0        0        0      309 2024-03-13 22:33:23.910849 qlat_cps-0.56/PKG-INFO
```

### Comparing `qlat_cps-0.55/depend-cps/meson.build` & `qlat_cps-0.56/depend-cps/meson.build`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.55/depend-qlat/meson.build` & `qlat_cps-0.56/depend-qlat/meson.build`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.55/meson.build` & `qlat_cps-0.56/meson.build`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project('qlat-cps', 'cpp', 'cython',
-  version: '0.55',
+  version: '0.56',
   license: 'GPL-3.0-or-later',
   default_options: [
     'warning_level=1',
     'cpp_std=c++14',
     'libdir=lib',
     'optimization=2',
     'debug=false',
```

### Comparing `qlat_cps-0.55/pyproject.toml` & `qlat_cps-0.56/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.55/qlat_cps/cp.pyx` & `qlat_cps-0.56/qlat_cps/cp.pyx`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.55/qlat_cps/get_include_dir.py` & `qlat_cps-0.56/qlat_cps/get_include_dir.py`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.55/qlat_cps/lib/init.cpp` & `qlat_cps-0.56/qlat_cps/lib/init.cpp`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.55/qlat_cps/lib/prop.cpp` & `qlat_cps-0.56/qlat_cps/lib/prop.cpp`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.55/qlat_cps/meson.build` & `qlat_cps-0.56/qlat_cps/meson.build`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.55/qlat_cps/scripts/qlat_cps_config.py` & `qlat_cps-0.56/qlat_cps/scripts/qlat_cps_config.py`

 * *Files identical despite different names*

