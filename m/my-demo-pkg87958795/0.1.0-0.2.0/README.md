# Comparing `tmp/my_demo_pkg87958795-0.1.0.tar.gz` & `tmp/my_demo_pkg87958795-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\my_demo_pkg87958795-0.1.0.tar", last modified: Wed May 15 18:21:34 2024, max compression
+gzip compressed data, was "dist\my_demo_pkg87958795-0.2.0.tar", last modified: Wed May 15 18:48:45 2024, max compression
```

## Comparing `my_demo_pkg87958795-0.1.0.tar` & `my_demo_pkg87958795-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 18:21:34.436811 my_demo_pkg87958795-0.1.0/
--rw-rw-rw-   0        0        0      427 2024-05-15 18:21:34.435806 my_demo_pkg87958795-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-05-15 17:44:21.000000 my_demo_pkg87958795-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 18:21:34.434875 my_demo_pkg87958795-0.1.0/my_demo_pkg87958795.egg-info/
--rw-rw-rw-   0        0        0      427 2024-05-15 18:21:34.000000 my_demo_pkg87958795-0.1.0/my_demo_pkg87958795.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-15 18:21:34.000000 my_demo_pkg87958795-0.1.0/my_demo_pkg87958795.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 18:21:34.000000 my_demo_pkg87958795-0.1.0/my_demo_pkg87958795.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 18:21:34.000000 my_demo_pkg87958795-0.1.0/my_demo_pkg87958795.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 18:21:34.438800 my_demo_pkg87958795-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      420 2024-05-15 18:21:24.000000 my_demo_pkg87958795-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:48:45.116919 my_demo_pkg87958795-0.2.0/
+-rw-rw-rw-   0        0        0      427 2024-05-15 18:48:45.115925 my_demo_pkg87958795-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-05-15 17:44:21.000000 my_demo_pkg87958795-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 18:48:45.114911 my_demo_pkg87958795-0.2.0/my_demo_pkg87958795.egg-info/
+-rw-rw-rw-   0        0        0      427 2024-05-15 18:48:45.000000 my_demo_pkg87958795-0.2.0/my_demo_pkg87958795.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-15 18:48:45.000000 my_demo_pkg87958795-0.2.0/my_demo_pkg87958795.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 18:48:45.000000 my_demo_pkg87958795-0.2.0/my_demo_pkg87958795.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 18:48:45.000000 my_demo_pkg87958795-0.2.0/my_demo_pkg87958795.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 18:48:45.117918 my_demo_pkg87958795-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      418 2024-05-15 18:48:42.000000 my_demo_pkg87958795-0.2.0/setup.py
```

