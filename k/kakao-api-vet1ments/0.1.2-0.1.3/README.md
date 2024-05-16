# Comparing `tmp/kakao_api_vet1ments-0.1.2.tar.gz` & `tmp/kakao_api_vet1ments-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kakao_api_vet1ments-0.1.2.tar", last modified: Thu May 16 15:19:07 2024, max compression
+gzip compressed data, was "kakao_api_vet1ments-0.1.3.tar", last modified: Thu May 16 15:24:08 2024, max compression
```

## Comparing `kakao_api_vet1ments-0.1.2.tar` & `kakao_api_vet1ments-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:19:07.037118 kakao_api_vet1ments-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-16 15:18:59.000000 kakao_api_vet1ments-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-16 15:19:07.037118 kakao_api_vet1ments-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:18:59.000000 kakao_api_vet1ments-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:19:07.033118 kakao_api_vet1ments-0.1.2/kakao_api/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 15:18:59.000000 kakao_api_vet1ments-0.1.2/kakao_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 15:18:59.000000 kakao_api_vet1ments-0.1.2/kakao_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-16 15:18:59.000000 kakao_api_vet1ments-0.1.2/kakao_api/kakao_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-16 15:18:59.000000 kakao_api_vet1ments-0.1.2/kakao_api/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-16 15:18:59.000000 kakao_api_vet1ments-0.1.2/kakao_api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:19:07.033118 kakao_api_vet1ments-0.1.2/kakao_api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 15:18:59.000000 kakao_api_vet1ments-0.1.2/kakao_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-16 15:18:59.000000 kakao_api_vet1ments-0.1.2/kakao_api/utils/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:19:07.037118 kakao_api_vet1ments-0.1.2/kakao_api_vet1ments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-16 15:19:06.000000 kakao_api_vet1ments-0.1.2/kakao_api_vet1ments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-16 15:19:07.000000 kakao_api_vet1ments-0.1.2/kakao_api_vet1ments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:19:06.000000 kakao_api_vet1ments-0.1.2/kakao_api_vet1ments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 15:19:06.000000 kakao_api_vet1ments-0.1.2/kakao_api_vet1ments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 15:19:06.000000 kakao_api_vet1ments-0.1.2/kakao_api_vet1ments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:19:07.037118 kakao_api_vet1ments-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-16 15:19:05.000000 kakao_api_vet1ments-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:24:08.388635 kakao_api_vet1ments-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-16 15:24:00.000000 kakao_api_vet1ments-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-16 15:24:08.388635 kakao_api_vet1ments-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 15:24:00.000000 kakao_api_vet1ments-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:24:08.388635 kakao_api_vet1ments-0.1.3/kakao_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 15:24:00.000000 kakao_api_vet1ments-0.1.3/kakao_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 15:24:00.000000 kakao_api_vet1ments-0.1.3/kakao_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-16 15:24:00.000000 kakao_api_vet1ments-0.1.3/kakao_api/kakao_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-16 15:24:00.000000 kakao_api_vet1ments-0.1.3/kakao_api/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-16 15:24:00.000000 kakao_api_vet1ments-0.1.3/kakao_api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:24:08.388635 kakao_api_vet1ments-0.1.3/kakao_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 15:24:00.000000 kakao_api_vet1ments-0.1.3/kakao_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-16 15:24:00.000000 kakao_api_vet1ments-0.1.3/kakao_api/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:24:08.388635 kakao_api_vet1ments-0.1.3/kakao_api_vet1ments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-16 15:24:08.000000 kakao_api_vet1ments-0.1.3/kakao_api_vet1ments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-16 15:24:08.000000 kakao_api_vet1ments-0.1.3/kakao_api_vet1ments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:24:08.000000 kakao_api_vet1ments-0.1.3/kakao_api_vet1ments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 15:24:08.000000 kakao_api_vet1ments-0.1.3/kakao_api_vet1ments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 15:24:08.000000 kakao_api_vet1ments-0.1.3/kakao_api_vet1ments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:24:08.388635 kakao_api_vet1ments-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-16 15:24:06.000000 kakao_api_vet1ments-0.1.3/setup.py
```

### Comparing `kakao_api_vet1ments-0.1.2/LICENSE` & `kakao_api_vet1ments-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kakao_api_vet1ments-0.1.2/kakao_api/kakao_api.py` & `kakao_api_vet1ments-0.1.3/kakao_api/kakao_api.py`

 * *Files identical despite different names*

### Comparing `kakao_api_vet1ments-0.1.2/kakao_api/types.py` & `kakao_api_vet1ments-0.1.3/kakao_api/types.py`

 * *Files identical despite different names*

### Comparing `kakao_api_vet1ments-0.1.2/kakao_api/urls.py` & `kakao_api_vet1ments-0.1.3/kakao_api/urls.py`

 * *Files identical despite different names*

### Comparing `kakao_api_vet1ments-0.1.2/kakao_api/utils/singleton.py` & `kakao_api_vet1ments-0.1.3/kakao_api/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `kakao_api_vet1ments-0.1.2/setup.py` & `kakao_api_vet1ments-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name='kakao_api_vet1ments',
     description="카카오 로그인 rest api",
-    version='0.1.2',
+    version='0.1.3',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.11.0',
     author="no hong seok",
     author_email="vet1ments@naver.com",
     maintainer="no hong seok",
     maintainer_email="vet1ments@naver.com",
```

