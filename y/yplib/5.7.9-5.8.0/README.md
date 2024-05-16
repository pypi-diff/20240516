# Comparing `tmp/yplib-5.7.9.tar.gz` & `tmp/yplib-5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yplib-5.7.9.tar", last modified: Wed May 15 07:00:07 2024, max compression
+gzip compressed data, was "yplib-5.8.0.tar", last modified: Thu May 16 07:21:45 2024, max compression
```

## Comparing `yplib-5.7.9.tar` & `yplib-5.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 07:00:07.888701 yplib-5.7.9/
--rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.7.9/LICENSE
--rw-rw-rw-   0        0        0      355 2024-05-15 07:00:07.888701 yplib-5.7.9/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.7.9/README.md
--rw-rw-rw-   0        0        0       42 2024-05-15 07:00:07.888701 yplib-5.7.9/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-05-15 07:00:03.000000 yplib-5.7.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:00:07.873701 yplib-5.7.9/yplib/
--rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.7.9/yplib/__init__.py
--rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.7.9/yplib/chart.py
--rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.7.9/yplib/chart_html.py
--rw-rw-rw-   0        0        0    12851 2024-05-15 06:59:51.000000 yplib-5.7.9/yplib/db.py
--rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.7.9/yplib/file.py
--rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.7.9/yplib/http_util.py
--rw-rw-rw-   0        0        0    41438 2024-05-08 04:02:59.000000 yplib-5.7.9/yplib/index.py
--rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.7.9/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.7.9/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.7.9/yplib/markdown.py
--rw-rw-rw-   0        0        0     2246 2024-05-07 06:14:17.000000 yplib-5.7.9/yplib/multi_thread.py
--rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.7.9/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:00:07.888701 yplib-5.7.9/yplib.egg-info/
--rw-rw-rw-   0        0        0      355 2024-05-15 07:00:07.000000 yplib-5.7.9/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-15 07:00:07.000000 yplib-5.7.9/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 07:00:07.000000 yplib-5.7.9/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-15 07:00:07.000000 yplib-5.7.9/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 07:21:45.068454 yplib-5.8.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.8.0/LICENSE
+-rw-rw-rw-   0        0        0      355 2024-05-16 07:21:45.068454 yplib-5.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.8.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 07:21:45.068454 yplib-5.8.0/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-05-16 07:21:13.000000 yplib-5.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:21:45.068454 yplib-5.8.0/yplib/
+-rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.8.0/yplib/__init__.py
+-rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.8.0/yplib/chart.py
+-rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.8.0/yplib/chart_html.py
+-rw-rw-rw-   0        0        0    12851 2024-05-15 06:59:51.000000 yplib-5.8.0/yplib/db.py
+-rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.8.0/yplib/file.py
+-rw-rw-rw-   0        0        0     7361 2024-05-16 07:20:59.000000 yplib-5.8.0/yplib/http_util.py
+-rw-rw-rw-   0        0        0    41438 2024-05-08 04:02:59.000000 yplib-5.8.0/yplib/index.py
+-rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.8.0/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.8.0/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.8.0/yplib/markdown.py
+-rw-rw-rw-   0        0        0     2246 2024-05-07 06:14:17.000000 yplib-5.8.0/yplib/multi_thread.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.8.0/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:21:45.068454 yplib-5.8.0/yplib.egg-info/
+-rw-rw-rw-   0        0        0      355 2024-05-16 07:21:44.000000 yplib-5.8.0/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-16 07:21:44.000000 yplib-5.8.0/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 07:21:44.000000 yplib-5.8.0/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-16 07:21:44.000000 yplib-5.8.0/yplib.egg-info/top_level.txt
```

### Comparing `yplib-5.7.9/LICENSE` & `yplib-5.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-5.7.9/setup.py` & `yplib-5.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yplib",
-    version="5.7.9",
+    version="5.8.0",
     author="yangpu",
     author_email="wantwaterfish@gmail.com",
     description="util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yplib-5.7.9/yplib/__init__.py` & `yplib-5.8.0/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.9/yplib/chart.py` & `yplib-5.8.0/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.9/yplib/chart_html.py` & `yplib-5.8.0/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.9/yplib/db.py` & `yplib-5.8.0/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.9/yplib/file.py` & `yplib-5.8.0/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.9/yplib/http_util.py` & `yplib-5.8.0/yplib/http_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,42 +41,42 @@
 # verify  : verify
 # r_json : 返回的数据是否是一个 json 类型的数据
 def do_get_response(url=None,
                     session=None,
                     headers=None,
                     cookie=None,
                     auth=None,
-                    timeout=100,
+                    timeout=1000,
                     verify=False):
     if session is None:
         session = requests.session()
     requests.packages.urllib3.disable_warnings()
     return session.get(url=url, headers=headers, auth=auth, timeout=timeout, verify=verify, cookies=cookie)
 
 
 def do_get(url=None,
            session=None,
            headers=None,
            cookie=None,
            auth=None,
-           timeout=100,
+           timeout=1000,
            verify=False,
            r_json=False):
     response = do_get_response(url=url, session=session, headers=headers, cookie=cookie, auth=auth, timeout=timeout, verify=verify)
     response.encoding = 'utf-8'
     return json.loads(response.text.strip()) if r_json else response.text.strip()
 
 
 # 返回的是一个 json 数据
 def do_get_json(url=None,
                 session=None,
                 headers=None,
                 cookie=None,
                 auth=None,
-                timeout=100,
+                timeout=1000,
                 verify=False):
     return do_get(url=url, session=session, headers=headers, cookie=cookie, auth=auth, timeout=timeout, verify=verify,
                   r_json=True)
 
 
 # 下载
 # file_name   : 文件名 , 默认 txt
@@ -89,15 +89,15 @@
 def do_download(url=None,
                 file_name=None,
                 file_path='download',
                 session=None,
                 headers=None,
                 cookie=None,
                 auth=None,
-                timeout=100,
+                timeout=1000,
                 verify=False):
     if session is None:
         session = requests.session()
     requests.packages.urllib3.disable_warnings()
     response = session.get(url=url, headers=headers, auth=auth, timeout=timeout, verify=verify, cookies=cookie)
     if response.status_code != 200:
         to_log_file('error', url, response.status_code)
@@ -148,15 +148,15 @@
 def do_post_response(url=None,
                      data=None,
                      is_form_data=False,
                      session=None,
                      headers=None,
                      cookie=None,
                      auth=None,
-                     timeout=100,
+                     timeout=1000,
                      verify=False):
     # headers = {'Content-Type': 'application/x-www-form-urlencoded'}
     # data = {}
     # data['appkey'] = APP_KEY
     # data['secretkey'] = SECRET_KEY
     # data['content'] = content
     # data['phone'] = obtainMobileIndonesia(mobile)
@@ -182,14 +182,14 @@
 def do_post(url=None,
             data=None,
             is_form_data=False,
             session=None,
             headers=None,
             cookie=None,
             auth=None,
-            timeout=100,
+            timeout=1000,
             verify=False,
             r_json=False):
     response = do_post_response(url=url, data=data, is_form_data=is_form_data, session=session, headers=headers, cookie=cookie, auth=auth, timeout=timeout,
                                 verify=verify)
     response.encoding = 'utf-8'
     return json.loads(response.text.strip()) if r_json else response.text.strip()
```

### Comparing `yplib-5.7.9/yplib/index.py` & `yplib-5.8.0/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.9/yplib/mail.py` & `yplib-5.8.0/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.9/yplib/mail_html.py` & `yplib-5.8.0/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.9/yplib/markdown.py` & `yplib-5.8.0/yplib/markdown.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.9/yplib/multi_thread.py` & `yplib-5.8.0/yplib/multi_thread.py`

 * *Files identical despite different names*

