# Comparing `tmp/PyEmailerAJM-1.3.tar.gz` & `tmp/PyEmailerAJM-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEmailerAJM-1.3.tar", last modified: Tue May 14 11:59:58 2024, max compression
+gzip compressed data, was "PyEmailerAJM-1.4.tar", last modified: Thu May 16 12:31:58 2024, max compression
```

## Comparing `PyEmailerAJM-1.3.tar` & `PyEmailerAJM-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 11:59:58.435606 PyEmailerAJM-1.3/
--rw-rw-rw-   0        0        0     1084 2023-09-12 19:19:18.000000 PyEmailerAJM-1.3/LICENSE.txt
--rw-rw-rw-   0        0        0      513 2024-05-14 11:59:58.436600 PyEmailerAJM-1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 11:59:58.408640 PyEmailerAJM-1.3/PyEmailerAJM/
--rw-rw-rw-   0        0        0    10428 2024-05-14 11:50:42.000000 PyEmailerAJM-1.3/PyEmailerAJM/PyEmailerAJM.py
--rw-rw-rw-   0        0        0      109 2023-09-13 15:44:18.000000 PyEmailerAJM-1.3/PyEmailerAJM/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:59:58.432576 PyEmailerAJM-1.3/PyEmailerAJM.egg-info/
--rw-rw-rw-   0        0        0      513 2024-05-14 11:59:58.000000 PyEmailerAJM-1.3/PyEmailerAJM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-05-14 11:59:58.000000 PyEmailerAJM-1.3/PyEmailerAJM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 11:59:58.000000 PyEmailerAJM-1.3/PyEmailerAJM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 11:59:58.000000 PyEmailerAJM-1.3/PyEmailerAJM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-14 11:59:58.000000 PyEmailerAJM-1.3/PyEmailerAJM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      388 2024-05-14 11:38:54.000000 PyEmailerAJM-1.3/README.md
--rw-rw-rw-   0        0        0       86 2024-05-14 11:59:58.440594 PyEmailerAJM-1.3/setup.cfg
--rw-rw-rw-   0        0        0      600 2024-05-14 11:51:15.000000 PyEmailerAJM-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:31:58.052281 PyEmailerAJM-1.4/
+-rw-rw-rw-   0        0        0     1084 2023-09-12 19:19:18.000000 PyEmailerAJM-1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      513 2024-05-16 12:31:58.053320 PyEmailerAJM-1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 12:31:58.027365 PyEmailerAJM-1.4/PyEmailerAJM/
+-rw-rw-rw-   0        0        0    11749 2024-05-16 11:47:45.000000 PyEmailerAJM-1.4/PyEmailerAJM/PyEmailerAJM.py
+-rw-rw-rw-   0        0        0      109 2023-09-13 15:44:18.000000 PyEmailerAJM-1.4/PyEmailerAJM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:31:58.050323 PyEmailerAJM-1.4/PyEmailerAJM.egg-info/
+-rw-rw-rw-   0        0        0      513 2024-05-16 12:31:57.000000 PyEmailerAJM-1.4/PyEmailerAJM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-16 12:31:57.000000 PyEmailerAJM-1.4/PyEmailerAJM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:31:57.000000 PyEmailerAJM-1.4/PyEmailerAJM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 12:31:57.000000 PyEmailerAJM-1.4/PyEmailerAJM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-16 12:31:57.000000 PyEmailerAJM-1.4/PyEmailerAJM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      545 2024-05-16 12:24:41.000000 PyEmailerAJM-1.4/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-16 12:31:58.057267 PyEmailerAJM-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-05-16 11:59:38.000000 PyEmailerAJM-1.4/setup.py
```

### Comparing `PyEmailerAJM-1.3/LICENSE.txt` & `PyEmailerAJM-1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyEmailerAJM-1.3/PKG-INFO` & `PyEmailerAJM-1.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: PyEmailerAJM
-Version: 1.3
+Version: 1.4
 Summary: Allows for automating sending Email with the Outlook Desktop client. Future releases will add more client support
 Home-page: https://github.com/amcsparron2793-Water/PyEmailer
 Author: Amcsparron
 Author-email: amcsparron@albanyny.gov
 License: MIT License
-Download-URL: https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.3.tar.gz
+Download-URL: https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.4.tar.gz
 Keywords: Outlook,Email,Automation
 Platform: UNKNOWN
 License-File: LICENSE.txt
 
 UNKNOWN
```

### Comparing `PyEmailerAJM-1.3/PyEmailerAJM/PyEmailerAJM.py` & `PyEmailerAJM-1.4/PyEmailerAJM/PyEmailerAJM.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #! python3
 """
 PyEmailerAJM.py
 
 install win32 with pip install pywin32
 """
-from os.path import isfile, abspath, isabs, join
+from os import environ
+from os.path import isfile, abspath, isabs, join, isdir
 
 # imports
 
 # install win32 with pip install pywin32
 import win32com.client as win32
 # This is installed as part of pywin32
 from pythoncom import com_error
@@ -18,17 +19,20 @@
 class EmailerNotSetupError(Exception):
     ...
 
 
 class PyEmailer:
     # the email tab_char
     tab_char = '&emsp;'
+    signature_dir_path = join((environ['USERPROFILE']),
+                              'AppData\\Roaming\\Microsoft\\Signatures\\')
 
     def __init__(self, display_window: bool,
                  send_emails: bool, logger: Logger = None,
+                 email_sig_filename: str = None,
                  auto_send: bool = False,
                  email_app_name: str = 'outlook.application'):
 
         if logger:
             self._logger = logger
         else:
             self._logger = Logger("DUMMY")
@@ -50,14 +54,45 @@
             self.email_app = win32.Dispatch(self.email_app_name)
             self._mapi_ns = self.email_app.GetNamespace('MAPI')
             self.email = self.email_app.CreateItem(0)
         except com_error as e:
             self._logger.error(e, exc_info=True)
             raise e
 
+        self._email_signature = None
+        self.email_sig_filename = email_sig_filename
+
+    @property
+    def email_signature(self):
+        return self._email_signature
+
+    @email_signature.getter
+    def email_signature(self):
+        signature_full_path = join(self.signature_dir_path, self.email_sig_filename)
+        if isdir(self.signature_dir_path):
+            pass
+        else:
+            try:
+                raise NotADirectoryError(f"{self.signature_dir_path} does not exist.")
+            except NotADirectoryError as e:
+                self._logger.warning(e)
+                self._email_signature = None
+
+        if isfile(signature_full_path):
+            with open(signature_full_path, 'r', encoding='utf-16') as f:
+                self._email_signature = f.read().strip()
+        else:
+            try:
+                raise FileNotFoundError(f"{signature_full_path} does not exist.")
+            except FileNotFoundError as e:
+                self._logger.warning(e)
+                self._email_signature = None
+
+        return self._email_signature
+
     def _GetReadFolder(self, email_dir_index: int = 6):
         # 6 = inbox
         self.read_folder = self._mapi_ns.GetDefaultFolder(email_dir_index)
         return self.read_folder
 
     def GetMessages(self, folder_index=None):
         if isinstance(folder_index, int):
```

### Comparing `PyEmailerAJM-1.3/PyEmailerAJM.egg-info/PKG-INFO` & `PyEmailerAJM-1.4/PyEmailerAJM.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: PyEmailerAJM
-Version: 1.3
+Version: 1.4
 Summary: Allows for automating sending Email with the Outlook Desktop client. Future releases will add more client support
 Home-page: https://github.com/amcsparron2793-Water/PyEmailer
 Author: Amcsparron
 Author-email: amcsparron@albanyny.gov
 License: MIT License
-Download-URL: https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.3.tar.gz
+Download-URL: https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.4.tar.gz
 Keywords: Outlook,Email,Automation
 Platform: UNKNOWN
 License-File: LICENSE.txt
 
 UNKNOWN
```

### Comparing `PyEmailerAJM-1.3/setup.py` & `PyEmailerAJM-1.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 setup(
     name='PyEmailerAJM',
-    version='1.3',
+    version='1.4',
     packages=['PyEmailerAJM'],
     url='https://github.com/amcsparron2793-Water/PyEmailer',
-    download_url='https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.3.tar.gz',
+    download_url='https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.4.tar.gz',
     keywords=["Outlook", "Email", "Automation"],
     install_requires=['pywin32'],
     license='MIT License',
     author='Amcsparron',
     author_email='amcsparron@albanyny.gov',
     description='Allows for automating sending Email with the Outlook Desktop client. Future releases will add more client support'
 )
```

