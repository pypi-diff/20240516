# Comparing `tmp/g4f_xn-0.0.1.tar.gz` & `tmp/g4f_xn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f_xn-0.0.1.tar", last modified: Thu May 16 19:59:07 2024, max compression
+gzip compressed data, was "g4f_xn-0.0.2.tar", last modified: Thu May 16 21:03:35 2024, max compression
```

## Comparing `g4f_xn-0.0.1.tar` & `g4f_xn-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 19:59:07.445726 g4f_xn-0.0.1/
--rw-rw-rw-   0        0        0     1083 2024-05-16 19:53:32.000000 g4f_xn-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      652 2024-05-16 19:59:07.445726 g4f_xn-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1608 2024-05-16 19:56:26.000000 g4f_xn-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 19:59:07.430101 g4f_xn-0.0.1/g4f_xn/
--rw-rw-rw-   0        0        0      121 2024-05-15 11:02:49.000000 g4f_xn-0.0.1/g4f_xn/__init__.py
--rw-rw-rw-   0        0        0     1280 2024-05-16 19:56:26.000000 g4f_xn-0.0.1/g4f_xn/gpt.py
--rw-rw-rw-   0        0        0      352 2024-05-16 19:34:22.000000 g4f_xn-0.0.1/g4f_xn/misc.py
--rw-rw-rw-   0        0        0      805 2024-05-16 12:55:08.000000 g4f_xn-0.0.1/g4f_xn/output.py
--rw-rw-rw-   0        0        0     3272 2024-05-16 19:56:26.000000 g4f_xn-0.0.1/g4f_xn/test_providers.py
-drwxrwxrwx   0        0        0        0 2024-05-16 19:59:07.445726 g4f_xn-0.0.1/g4f_xn.egg-info/
--rw-rw-rw-   0        0        0      652 2024-05-16 19:59:07.000000 g4f_xn-0.0.1/g4f_xn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-16 19:59:07.000000 g4f_xn-0.0.1/g4f_xn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 19:59:07.000000 g4f_xn-0.0.1/g4f_xn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-16 19:59:07.000000 g4f_xn-0.0.1/g4f_xn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 19:59:07.000000 g4f_xn-0.0.1/g4f_xn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 19:59:07.445726 g4f_xn-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      878 2024-05-16 19:54:02.000000 g4f_xn-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:03:35.396850 g4f_xn-0.0.2/
+-rw-rw-rw-   0        0        0     1083 2024-05-16 19:53:32.000000 g4f_xn-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      612 2024-05-16 21:03:35.396850 g4f_xn-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1608 2024-05-16 20:38:48.000000 g4f_xn-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 21:03:35.396850 g4f_xn-0.0.2/g4f_xn/
+-rw-rw-rw-   0        0        0      121 2024-05-16 20:54:53.000000 g4f_xn-0.0.2/g4f_xn/__init__.py
+-rw-rw-rw-   0        0        0     1280 2024-05-16 19:56:26.000000 g4f_xn-0.0.2/g4f_xn/gpt.py
+-rw-rw-rw-   0        0        0      352 2024-05-16 19:34:22.000000 g4f_xn-0.0.2/g4f_xn/misc.py
+-rw-rw-rw-   0        0        0      805 2024-05-16 12:55:08.000000 g4f_xn-0.0.2/g4f_xn/output.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:03:35.396850 g4f_xn-0.0.2/g4f_xn/sound/
+-rw-rw-rw-   0        0        0        0 2024-05-16 20:55:17.000000 g4f_xn-0.0.2/g4f_xn/sound/__init__.py
+-rw-rw-rw-   0        0        0     1670 2024-05-16 19:56:26.000000 g4f_xn-0.0.2/g4f_xn/sound.py
+-rw-rw-rw-   0        0        0     3272 2024-05-16 19:56:26.000000 g4f_xn-0.0.2/g4f_xn/test_providers.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:03:35.396850 g4f_xn-0.0.2/g4f_xn.egg-info/
+-rw-rw-rw-   0        0        0      612 2024-05-16 21:03:35.000000 g4f_xn-0.0.2/g4f_xn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-05-16 21:03:35.000000 g4f_xn-0.0.2/g4f_xn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 21:03:35.000000 g4f_xn-0.0.2/g4f_xn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-16 21:03:35.000000 g4f_xn-0.0.2/g4f_xn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 21:03:35.000000 g4f_xn-0.0.2/g4f_xn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 21:03:35.396850 g4f_xn-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      829 2024-05-16 21:01:39.000000 g4f_xn-0.0.2/setup.py
```

### Comparing `g4f_xn-0.0.1/LICENSE` & `g4f_xn-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f_xn-0.0.1/PKG-INFO` & `g4f_xn-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: g4f_xn
-Version: 0.0.1
+Version: 0.0.2
 Summary: library for easy access to GPT models based on g4f
 Author: Xandr0v
 Author-email: <olegalexandrov468@gmail.com>
-Keywords: python,video,stream,video stream,camera stream,sockets
+Keywords: python,g4f,gpt
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: g4f
```

### Comparing `g4f_xn-0.0.1/README.md` & `g4f_xn-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `g4f_xn-0.0.1/g4f_xn/gpt.py` & `g4f_xn-0.0.2/g4f_xn/gpt.py`

 * *Files identical despite different names*

### Comparing `g4f_xn-0.0.1/g4f_xn/output.py` & `g4f_xn-0.0.2/g4f_xn/output.py`

 * *Files identical despite different names*

### Comparing `g4f_xn-0.0.1/g4f_xn/test_providers.py` & `g4f_xn-0.0.2/g4f_xn/test_providers.py`

 * *Files identical despite different names*

### Comparing `g4f_xn-0.0.1/g4f_xn.egg-info/PKG-INFO` & `g4f_xn-0.0.2/g4f_xn.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: g4f_xn
-Version: 0.0.1
+Version: 0.0.2
 Summary: library for easy access to GPT models based on g4f
 Author: Xandr0v
 Author-email: <olegalexandrov468@gmail.com>
-Keywords: python,video,stream,video stream,camera stream,sockets
+Keywords: python,g4f,gpt
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: g4f
```

### Comparing `g4f_xn-0.0.1/setup.py` & `g4f_xn-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'library for easy access to GPT models based on g4f'
 LONG_DESCRIPTION = 'long description. Will change in the future'
 
 # Setting up
 setup(
     name="g4f_xn",
     version=VERSION,
     author="Xandr0v",
     author_email="<olegalexandrov468@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['g4f', 'pyaudio', 'colorama', 'ffmpeg-downloader'],
-    keywords=['python', 'video', 'stream', 'video stream', 'camera stream', 'sockets'],
+    keywords=['python', 'g4f', 'gpt'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

