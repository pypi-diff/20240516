# Comparing `tmp/kakao_api_vet1ments-0.1.5.tar.gz` & `tmp/kakao_api_vet1ments-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kakao_api_vet1ments-0.1.5.tar", last modified: Thu May 16 15:29:32 2024, max compression
+gzip compressed data, was "kakao_api_vet1ments-0.1.6.tar", last modified: Thu May 16 15:34:27 2024, max compression
```

## Comparing `kakao_api_vet1ments-0.1.5.tar` & `kakao_api_vet1ments-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:29:32.618887 kakao_api_vet1ments-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-16 15:29:24.000000 kakao_api_vet1ments-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-16 15:29:32.618887 kakao_api_vet1ments-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 15:29:24.000000 kakao_api_vet1ments-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:29:32.618887 kakao_api_vet1ments-0.1.5/kakao_api/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 15:29:24.000000 kakao_api_vet1ments-0.1.5/kakao_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 15:29:24.000000 kakao_api_vet1ments-0.1.5/kakao_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-16 15:29:24.000000 kakao_api_vet1ments-0.1.5/kakao_api/kakao_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-16 15:29:24.000000 kakao_api_vet1ments-0.1.5/kakao_api/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-16 15:29:24.000000 kakao_api_vet1ments-0.1.5/kakao_api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:29:32.618887 kakao_api_vet1ments-0.1.5/kakao_api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 15:29:24.000000 kakao_api_vet1ments-0.1.5/kakao_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-16 15:29:24.000000 kakao_api_vet1ments-0.1.5/kakao_api/utils/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:29:32.618887 kakao_api_vet1ments-0.1.5/kakao_api_vet1ments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-16 15:29:32.000000 kakao_api_vet1ments-0.1.5/kakao_api_vet1ments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-16 15:29:32.000000 kakao_api_vet1ments-0.1.5/kakao_api_vet1ments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:29:32.000000 kakao_api_vet1ments-0.1.5/kakao_api_vet1ments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 15:29:32.000000 kakao_api_vet1ments-0.1.5/kakao_api_vet1ments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 15:29:32.000000 kakao_api_vet1ments-0.1.5/kakao_api_vet1ments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:29:32.618887 kakao_api_vet1ments-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-16 15:29:31.000000 kakao_api_vet1ments-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:34:27.261412 kakao_api_vet1ments-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-16 15:34:18.000000 kakao_api_vet1ments-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-16 15:34:27.261412 kakao_api_vet1ments-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 15:34:18.000000 kakao_api_vet1ments-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:34:27.261412 kakao_api_vet1ments-0.1.6/kakao_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 15:34:18.000000 kakao_api_vet1ments-0.1.6/kakao_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 15:34:18.000000 kakao_api_vet1ments-0.1.6/kakao_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-16 15:34:18.000000 kakao_api_vet1ments-0.1.6/kakao_api/kakao_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-16 15:34:18.000000 kakao_api_vet1ments-0.1.6/kakao_api/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-16 15:34:18.000000 kakao_api_vet1ments-0.1.6/kakao_api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:34:27.261412 kakao_api_vet1ments-0.1.6/kakao_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 15:34:18.000000 kakao_api_vet1ments-0.1.6/kakao_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-16 15:34:18.000000 kakao_api_vet1ments-0.1.6/kakao_api/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:34:27.261412 kakao_api_vet1ments-0.1.6/kakao_api_vet1ments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-16 15:34:27.000000 kakao_api_vet1ments-0.1.6/kakao_api_vet1ments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-16 15:34:27.000000 kakao_api_vet1ments-0.1.6/kakao_api_vet1ments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:34:27.000000 kakao_api_vet1ments-0.1.6/kakao_api_vet1ments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 15:34:27.000000 kakao_api_vet1ments-0.1.6/kakao_api_vet1ments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 15:34:27.000000 kakao_api_vet1ments-0.1.6/kakao_api_vet1ments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:34:27.261412 kakao_api_vet1ments-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-16 15:34:25.000000 kakao_api_vet1ments-0.1.6/setup.py
```

### Comparing `kakao_api_vet1ments-0.1.5/LICENSE` & `kakao_api_vet1ments-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kakao_api_vet1ments-0.1.5/kakao_api/kakao_api.py` & `kakao_api_vet1ments-0.1.6/kakao_api/kakao_api.py`

 * *Files identical despite different names*

### Comparing `kakao_api_vet1ments-0.1.5/kakao_api/types.py` & `kakao_api_vet1ments-0.1.6/kakao_api/types.py`

 * *Files identical despite different names*

### Comparing `kakao_api_vet1ments-0.1.5/kakao_api/urls.py` & `kakao_api_vet1ments-0.1.6/kakao_api/urls.py`

 * *Files identical despite different names*

### Comparing `kakao_api_vet1ments-0.1.5/kakao_api/utils/singleton.py` & `kakao_api_vet1ments-0.1.6/kakao_api/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `kakao_api_vet1ments-0.1.5/setup.py` & `kakao_api_vet1ments-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name='kakao_api_vet1ments',
     description="카카오 로그인 rest api",
-    version='0.1.5',
+    version='0.1.6',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.11.0',
     author="no hong seok",
     author_email="vet1ments@naver.com",
     maintainer="no hong seok",
     maintainer_email="vet1ments@naver.com",
```

