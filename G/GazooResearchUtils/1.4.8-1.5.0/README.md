# Comparing `tmp/GazooResearchUtils-1.4.8.tar.gz` & `tmp/GazooResearchUtils-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GazooResearchUtils-1.4.8.tar", last modified: Tue May 14 03:08:12 2024, max compression
+gzip compressed data, was "GazooResearchUtils-1.5.0.tar", last modified: Thu May 16 13:58:22 2024, max compression
```

## Comparing `GazooResearchUtils-1.4.8.tar` & `GazooResearchUtils-1.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-14 03:08:12.884564 GazooResearchUtils-1.4.8/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-14 03:08:12.884298 GazooResearchUtils-1.4.8/PKG-INFO
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-14 03:08:12.882341 GazooResearchUtils-1.4.8/app/
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-14 03:08:12.882825 GazooResearchUtils-1.4.8/app/GazooResearchUtils/
--rw-r--r--   0 andrewlim   (501) staff       (20)      134 2024-05-14 03:08:02.000000 GazooResearchUtils-1.4.8/app/GazooResearchUtils/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-14 03:08:12.883940 GazooResearchUtils-1.4.8/app/GazooResearchUtils/src/
--rw-r--r--   0 andrewlim   (501) staff       (20)     7602 2024-05-14 03:07:44.000000 GazooResearchUtils-1.4.8/app/GazooResearchUtils/src/Analysis.py
--rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.4.8/app/GazooResearchUtils/src/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-14 03:08:12.883587 GazooResearchUtils-1.4.8/app/GazooResearchUtils.egg-info/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-14 03:08:12.000000 GazooResearchUtils-1.4.8/app/GazooResearchUtils.egg-info/PKG-INFO
--rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-14 03:08:12.000000 GazooResearchUtils-1.4.8/app/GazooResearchUtils.egg-info/SOURCES.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-14 03:08:12.000000 GazooResearchUtils-1.4.8/app/GazooResearchUtils.egg-info/dependency_links.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-14 03:08:12.000000 GazooResearchUtils-1.4.8/app/GazooResearchUtils.egg-info/requires.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-14 03:08:12.000000 GazooResearchUtils-1.4.8/app/GazooResearchUtils.egg-info/top_level.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-14 03:08:12.884614 GazooResearchUtils-1.4.8/setup.cfg
--rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-14 03:08:09.000000 GazooResearchUtils-1.4.8/setup.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 13:58:22.062668 GazooResearchUtils-1.5.0/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-16 13:58:22.062443 GazooResearchUtils-1.5.0/PKG-INFO
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 13:58:22.060704 GazooResearchUtils-1.5.0/app/
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 13:58:22.061115 GazooResearchUtils-1.5.0/app/GazooResearchUtils/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      187 2024-05-16 13:57:19.000000 GazooResearchUtils-1.5.0/app/GazooResearchUtils/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 13:58:22.062108 GazooResearchUtils-1.5.0/app/GazooResearchUtils/src/
+-rw-r--r--   0 andrewlim   (501) staff       (20)     8153 2024-05-16 13:57:04.000000 GazooResearchUtils-1.5.0/app/GazooResearchUtils/src/Analysis.py
+-rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.5.0/app/GazooResearchUtils/src/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 13:58:22.061770 GazooResearchUtils-1.5.0/app/GazooResearchUtils.egg-info/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-16 13:58:22.000000 GazooResearchUtils-1.5.0/app/GazooResearchUtils.egg-info/PKG-INFO
+-rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-16 13:58:22.000000 GazooResearchUtils-1.5.0/app/GazooResearchUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-16 13:58:22.000000 GazooResearchUtils-1.5.0/app/GazooResearchUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-16 13:58:22.000000 GazooResearchUtils-1.5.0/app/GazooResearchUtils.egg-info/requires.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-16 13:58:22.000000 GazooResearchUtils-1.5.0/app/GazooResearchUtils.egg-info/top_level.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-16 13:58:22.062713 GazooResearchUtils-1.5.0/setup.cfg
+-rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-16 13:57:27.000000 GazooResearchUtils-1.5.0/setup.py
```

