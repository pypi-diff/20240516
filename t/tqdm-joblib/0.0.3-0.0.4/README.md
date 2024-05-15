# Comparing `tmp/tqdm_joblib-0.0.3.tar.gz` & `tmp/tqdm_joblib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tqdm_joblib-0.0.3.tar", last modified: Mon Feb 20 09:26:32 2023, max compression
+gzip compressed data, was "tqdm_joblib-0.0.4.tar", last modified: Wed May 15 22:01:46 2024, max compression
```

## Comparing `tqdm_joblib-0.0.3.tar` & `tqdm_joblib-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 louisabraham   (501) staff       (20)        0 2023-02-20 09:26:32.604833 tqdm_joblib-0.0.3/
--rw-r--r--   0 louisabraham   (501) staff       (20)      276 2023-02-20 09:26:32.604646 tqdm_joblib-0.0.3/PKG-INFO
--rw-r--r--   0 louisabraham   (501) staff       (20)      397 2023-02-20 09:23:04.000000 tqdm_joblib-0.0.3/README.md
--rw-r--r--   0 louisabraham   (501) staff       (20)       38 2023-02-20 09:26:32.604894 tqdm_joblib-0.0.3/setup.cfg
--rw-r--r--   0 louisabraham   (501) staff       (20)      382 2023-02-20 09:23:06.000000 tqdm_joblib-0.0.3/setup.py
-drwxr-xr-x   0 louisabraham   (501) staff       (20)        0 2023-02-20 09:26:32.603573 tqdm_joblib-0.0.3/tqdm_joblib/
--rw-r--r--   0 louisabraham   (501) staff       (20)      875 2023-02-20 09:23:04.000000 tqdm_joblib-0.0.3/tqdm_joblib/__init__.py
-drwxr-xr-x   0 louisabraham   (501) staff       (20)        0 2023-02-20 09:26:32.604448 tqdm_joblib-0.0.3/tqdm_joblib.egg-info/
--rw-r--r--   0 louisabraham   (501) staff       (20)      276 2023-02-20 09:26:32.000000 tqdm_joblib-0.0.3/tqdm_joblib.egg-info/PKG-INFO
--rw-r--r--   0 louisabraham   (501) staff       (20)      216 2023-02-20 09:26:32.000000 tqdm_joblib-0.0.3/tqdm_joblib.egg-info/SOURCES.txt
--rw-r--r--   0 louisabraham   (501) staff       (20)        1 2023-02-20 09:26:32.000000 tqdm_joblib-0.0.3/tqdm_joblib.egg-info/dependency_links.txt
--rw-r--r--   0 louisabraham   (501) staff       (20)        5 2023-02-20 09:26:32.000000 tqdm_joblib-0.0.3/tqdm_joblib.egg-info/requires.txt
--rw-r--r--   0 louisabraham   (501) staff       (20)       12 2023-02-20 09:26:32.000000 tqdm_joblib-0.0.3/tqdm_joblib.egg-info/top_level.txt
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2024-05-15 22:01:46.575090 tqdm_joblib-0.0.4/
+-rw-r--r--   0 louis      (501) staff       (20)      268 2024-05-15 22:01:46.574869 tqdm_joblib-0.0.4/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      528 2024-05-15 21:58:33.000000 tqdm_joblib-0.0.4/README.md
+-rw-r--r--   0 louis      (501) staff       (20)       38 2024-05-15 22:01:46.575136 tqdm_joblib-0.0.4/setup.cfg
+-rw-r--r--   0 louis      (501) staff       (20)      382 2024-05-15 21:58:47.000000 tqdm_joblib-0.0.4/setup.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2024-05-15 22:01:46.573843 tqdm_joblib-0.0.4/tqdm_joblib/
+-rw-r--r--   0 louis      (501) staff       (20)     1154 2024-05-15 21:56:38.000000 tqdm_joblib-0.0.4/tqdm_joblib/__init__.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2024-05-15 22:01:46.574678 tqdm_joblib-0.0.4/tqdm_joblib.egg-info/
+-rw-r--r--   0 louis      (501) staff       (20)      268 2024-05-15 22:01:46.000000 tqdm_joblib-0.0.4/tqdm_joblib.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      216 2024-05-15 22:01:46.000000 tqdm_joblib-0.0.4/tqdm_joblib.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2024-05-15 22:01:46.000000 tqdm_joblib-0.0.4/tqdm_joblib.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)        5 2024-05-15 22:01:46.000000 tqdm_joblib-0.0.4/tqdm_joblib.egg-info/requires.txt
+-rw-r--r--   0 louis      (501) staff       (20)       12 2024-05-15 22:01:46.000000 tqdm_joblib-0.0.4/tqdm_joblib.egg-info/top_level.txt
```

