# Comparing `tmp/litellm_types-0.0.4.tar.gz` & `tmp/litellm_types-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm_types-0.0.4.tar", last modified: Mon May 13 12:28:24 2024, max compression
+gzip compressed data, was "litellm_types-0.0.5.tar", last modified: Thu May 16 15:16:28 2024, max compression
```

## Comparing `litellm_types-0.0.4.tar` & `litellm_types-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-13 12:28:24.133077 litellm_types-0.0.4/
--rw-r--r--   0 salamanderxing   (501) staff       (20)    11357 2024-05-06 12:34:17.000000 litellm_types-0.0.4/LICENSE
--rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-13 12:28:24.132890 litellm_types-0.0.4/PKG-INFO
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-13 12:28:24.132071 litellm_types-0.0.4/litellm_types/
--rw-r--r--   0 salamanderxing   (501) staff       (20)        2 2024-05-05 16:42:41.000000 litellm_types-0.0.4/litellm_types/__init__.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)    11385 2024-05-13 11:48:57.000000 litellm_types-0.0.4/litellm_types/completion.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)      134 2024-05-05 16:26:12.000000 litellm_types-0.0.4/litellm_types/document.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)     3875 2024-05-13 12:00:51.000000 litellm_types-0.0.4/litellm_types/messages.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)      293 2024-05-05 16:23:45.000000 litellm_types-0.0.4/litellm_types/prompt.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)     1324 2024-05-13 11:50:02.000000 litellm_types-0.0.4/litellm_types/test.py
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-13 12:28:24.132710 litellm_types-0.0.4/litellm_types.egg-info/
--rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-13 12:28:24.000000 litellm_types-0.0.4/litellm_types.egg-info/PKG-INFO
--rw-r--r--   0 salamanderxing   (501) staff       (20)      352 2024-05-13 12:28:24.000000 litellm_types-0.0.4/litellm_types.egg-info/SOURCES.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-05-13 12:28:24.000000 litellm_types-0.0.4/litellm_types.egg-info/dependency_links.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       26 2024-05-13 12:28:24.000000 litellm_types-0.0.4/litellm_types.egg-info/requires.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       14 2024-05-13 12:28:24.000000 litellm_types-0.0.4/litellm_types.egg-info/top_level.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-05-13 12:28:24.133110 litellm_types-0.0.4/setup.cfg
--rw-r--r--   0 salamanderxing   (501) staff       (20)      263 2024-05-13 12:28:16.000000 litellm_types-0.0.4/setup.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-16 15:16:28.628689 litellm_types-0.0.5/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)    11357 2024-05-06 12:34:17.000000 litellm_types-0.0.5/LICENSE
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-16 15:16:28.628444 litellm_types-0.0.5/PKG-INFO
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-16 15:16:28.627221 litellm_types-0.0.5/litellm_types/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)        2 2024-05-05 16:42:41.000000 litellm_types-0.0.5/litellm_types/__init__.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)    11385 2024-05-13 11:48:57.000000 litellm_types-0.0.5/litellm_types/completion.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      134 2024-05-05 16:26:12.000000 litellm_types-0.0.5/litellm_types/document.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)     3875 2024-05-13 12:00:51.000000 litellm_types-0.0.5/litellm_types/messages.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      293 2024-05-05 16:23:45.000000 litellm_types-0.0.5/litellm_types/prompt.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)     1324 2024-05-13 11:50:02.000000 litellm_types-0.0.5/litellm_types/test.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-16 15:16:28.628168 litellm_types-0.0.5/litellm_types.egg-info/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-16 15:16:28.000000 litellm_types-0.0.5/litellm_types.egg-info/PKG-INFO
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      352 2024-05-16 15:16:28.000000 litellm_types-0.0.5/litellm_types.egg-info/SOURCES.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-05-16 15:16:28.000000 litellm_types-0.0.5/litellm_types.egg-info/dependency_links.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       26 2024-05-16 15:16:28.000000 litellm_types-0.0.5/litellm_types.egg-info/requires.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       14 2024-05-16 15:16:28.000000 litellm_types-0.0.5/litellm_types.egg-info/top_level.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-05-16 15:16:28.628749 litellm_types-0.0.5/setup.cfg
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      263 2024-05-16 15:16:03.000000 litellm_types-0.0.5/setup.py
```

### Comparing `litellm_types-0.0.4/LICENSE` & `litellm_types-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm_types-0.0.4/litellm_types/completion.py` & `litellm_types-0.0.5/litellm_types/completion.py`

 * *Files identical despite different names*

### Comparing `litellm_types-0.0.4/litellm_types/messages.py` & `litellm_types-0.0.5/litellm_types/messages.py`

 * *Files identical despite different names*

### Comparing `litellm_types-0.0.4/litellm_types/test.py` & `litellm_types-0.0.5/litellm_types/test.py`

 * *Files identical despite different names*

