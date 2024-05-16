# Comparing `tmp/hscloud-0.0.0.9.tar.gz` & `tmp/hscloud-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscloud-0.0.0.9.tar", last modified: Mon May 13 07:31:21 2024, max compression
+gzip compressed data, was "hscloud-1.0.0.tar", last modified: Thu May 16 09:27:32 2024, max compression
```

## Comparing `hscloud-0.0.0.9.tar` & `hscloud-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 07:31:21.726324 hscloud-0.0.0.9/
--rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.0.9/LICENSE
--rw-rw-rw-   0        0        0      432 2024-05-13 07:31:21.724324 hscloud-0.0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2505 2024-05-09 10:10:45.000000 hscloud-0.0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 07:31:21.703324 hscloud-0.0.0.9/hscloud/
--rw-rw-rw-   0        0        0      258 2024-05-09 07:57:46.000000 hscloud-0.0.0.9/hscloud/__init__.py
--rw-rw-rw-   0        0        0     4082 2024-05-13 07:30:19.000000 hscloud-0.0.0.9/hscloud/helpers.py
--rw-rw-rw-   0        0        0     2313 2024-05-13 07:29:46.000000 hscloud-0.0.0.9/hscloud/hscloud.py
--rw-rw-rw-   0        0        0      443 2024-05-13 07:25:23.000000 hscloud-0.0.0.9/hscloud/hscloudexception.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:31:21.723324 hscloud-0.0.0.9/hscloud.egg-info/
--rw-rw-rw-   0        0        0      432 2024-05-13 07:31:21.000000 hscloud-0.0.0.9/hscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2024-05-13 07:31:21.000000 hscloud-0.0.0.9/hscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 07:31:21.000000 hscloud-0.0.0.9/hscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-13 07:31:21.000000 hscloud-0.0.0.9/hscloud.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-05-13 07:31:21.000000 hscloud-0.0.0.9/hscloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-13 07:31:21.000000 hscloud-0.0.0.9/hscloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 07:31:21.726324 hscloud-0.0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      887 2024-05-13 07:31:00.000000 hscloud-0.0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:27:32.534044 hscloud-1.0.0/
+-rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      429 2024-05-16 09:27:32.532043 hscloud-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2505 2024-05-09 10:10:45.000000 hscloud-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 09:27:32.514042 hscloud-1.0.0/hscloud/
+-rw-rw-rw-   0        0        0      258 2024-05-09 07:57:46.000000 hscloud-1.0.0/hscloud/__init__.py
+-rw-rw-rw-   0        0        0     4092 2024-05-16 09:23:17.000000 hscloud-1.0.0/hscloud/helpers.py
+-rw-rw-rw-   0        0        0     1972 2024-05-13 07:37:07.000000 hscloud-1.0.0/hscloud/hscloud.py
+-rw-rw-rw-   0        0        0      443 2024-05-13 07:25:23.000000 hscloud-1.0.0/hscloud/hscloudexception.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:27:32.530044 hscloud-1.0.0/hscloud.egg-info/
+-rw-rw-rw-   0        0        0      429 2024-05-16 09:27:32.000000 hscloud-1.0.0/hscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2024-05-16 09:27:32.000000 hscloud-1.0.0/hscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 09:27:32.000000 hscloud-1.0.0/hscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-16 09:27:32.000000 hscloud-1.0.0/hscloud.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-05-16 09:27:32.000000 hscloud-1.0.0/hscloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 09:27:32.000000 hscloud-1.0.0/hscloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 09:27:32.534044 hscloud-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      884 2024-05-16 09:24:51.000000 hscloud-1.0.0/setup.py
```

### Comparing `hscloud-0.0.0.9/README.md` & `hscloud-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `hscloud-0.0.0.9/hscloud/helpers.py` & `hscloud-1.0.0/hscloud/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Optional
 from hscloud.hscloudexception import HsCloudException, HsCloudAccessDeniedException, HsCloudFlowControlException
 
 class Helpers:
 
     @staticmethod
     def login(username=None, password=None):
-        base_url = 'http://10.10.20.109:2070'
+        base_url = 'https://open-api-us.dreo-cloud.com'
 
         headers = {
             'Content-Type': 'application/json',
             'UA': 'openapi/1.0.0'
         }
 
         params = {
```

### Comparing `hscloud-0.0.0.9/hscloud/hscloud.py` & `hscloud-1.0.0/hscloud/hscloud.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,19 +52,8 @@
             logger.error(e)
             return None
         except HsCloudFlowControlException as e:
             logger.error(e)
             return None
 
     def update_status(self, devicesn, **kwargs):
-        try:
-            Helpers.update(self.endpoint, self.access_token, devicesn, **kwargs)
-            return True
-        except HsCloudException as e:
-            logger.error(e)
-            return False
-        except HsCloudAccessDeniedException as e:
-            logger.error(e)
-            return False
-        except HsCloudFlowControlException as e:
-            logger.error(e)
-            return False
+        return Helpers.update(self.endpoint, self.access_token, devicesn, **kwargs)
```

### Comparing `hscloud-0.0.0.9/setup.py` & `hscloud-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name = 'hscloud',
     packages = ['hscloud'],
     include_package_data=True,
-    version = '0.0.0.9',
+    version = '1.0.0',
     license='MIT',
     description = 'Library to login to Dreo cloud and get device info.',
     author = 'Kane Wang',
     author_email = 'app@hesung.com',
     url = 'https://github.com/dreo-team/hscloud',
-    download_url = 'https://github.com/dreo-team/hscloud/dist/hscloud-0.0.11.tar.gz',
+    download_url = 'https://github.com/dreo-team/hscloud/dist/hscloud-1.0.0.tar.gz',
     install_requires=[
         'requests',
         'tzlocal',
         'click',
         'pycryptodome'
     ],
     entry_points='''
```

