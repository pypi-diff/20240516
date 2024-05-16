# Comparing `tmp/hello_world_demo-1.0.0.tar.gz` & `tmp/hello_world_demo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_world_demo-1.0.0.tar", last modified: Thu May 16 04:51:32 2024, max compression
+gzip compressed data, was "hello_world_demo-1.0.1.tar", last modified: Thu May 16 05:11:25 2024, max compression
```

## Comparing `hello_world_demo-1.0.0.tar` & `hello_world_demo-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-16 04:51:32.290800 hello_world_demo-1.0.0/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      125 2024-05-16 04:51:32.290674 hello_world_demo-1.0.0/PKG-INFO
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-16 04:51:32.289860 hello_world_demo-1.0.0/hello_world/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       87 2024-05-16 04:44:14.000000 hello_world_demo-1.0.0/hello_world/__init__.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       71 2024-05-16 04:44:49.000000 hello_world_demo-1.0.0/hello_world/greeting.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      166 2024-05-16 04:45:20.000000 hello_world_demo-1.0.0/hello_world/math_utils.py
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-16 04:51:32.290495 hello_world_demo-1.0.0/hello_world_demo.egg-info/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      125 2024-05-16 04:51:32.000000 hello_world_demo-1.0.0/hello_world_demo.egg-info/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      242 2024-05-16 04:51:32.000000 hello_world_demo-1.0.0/hello_world_demo.egg-info/SOURCES.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-05-16 04:51:32.000000 hello_world_demo-1.0.0/hello_world_demo.egg-info/dependency_links.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       12 2024-05-16 04:51:32.000000 hello_world_demo-1.0.0/hello_world_demo.egg-info/top_level.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-05-16 04:51:32.290845 hello_world_demo-1.0.0/setup.cfg
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      215 2024-05-16 04:48:17.000000 hello_world_demo-1.0.0/setup.py
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-16 05:11:25.385383 hello_world_demo-1.0.1/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      125 2024-05-16 05:11:25.385229 hello_world_demo-1.0.1/PKG-INFO
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-16 05:11:25.384456 hello_world_demo-1.0.1/hello_world/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      137 2024-05-16 05:08:13.000000 hello_world_demo-1.0.1/hello_world/__init__.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       71 2024-05-16 04:44:49.000000 hello_world_demo-1.0.1/hello_world/greeting.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      166 2024-05-16 04:45:20.000000 hello_world_demo-1.0.1/hello_world/math_utils.py
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-16 05:11:25.385014 hello_world_demo-1.0.1/hello_world_demo.egg-info/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      125 2024-05-16 05:11:25.000000 hello_world_demo-1.0.1/hello_world_demo.egg-info/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      242 2024-05-16 05:11:25.000000 hello_world_demo-1.0.1/hello_world_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-05-16 05:11:25.000000 hello_world_demo-1.0.1/hello_world_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       12 2024-05-16 05:11:25.000000 hello_world_demo-1.0.1/hello_world_demo.egg-info/top_level.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-05-16 05:11:25.385431 hello_world_demo-1.0.1/setup.cfg
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      215 2024-05-16 05:10:34.000000 hello_world_demo-1.0.1/setup.py
```

