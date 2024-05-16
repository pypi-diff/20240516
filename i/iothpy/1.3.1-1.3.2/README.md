# Comparing `tmp/iothpy-1.3.1.tar.gz` & `tmp/iothpy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iothpy-1.3.1.tar", last modified: Sat May  4 06:39:01 2024, max compression
+gzip compressed data, was "iothpy-1.3.2.tar", last modified: Thu May 16 09:34:49 2024, max compression
```

## Comparing `iothpy-1.3.1.tar` & `iothpy-1.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-04 06:39:01.797777 iothpy-1.3.1/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1068 2024-05-04 06:34:10.000000 iothpy-1.3.1/CMakeLists.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    26526 2024-03-26 14:33:52.000000 iothpy-1.3.1/LICENSE
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      145 2024-03-26 14:33:52.000000 iothpy-1.3.1/MANIFEST.in
--rw-r--r--   0 francesco  (1000) francesco  (1000)     6516 2024-05-04 06:39:01.797777 iothpy-1.3.1/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6180 2024-03-26 14:33:52.000000 iothpy-1.3.1/README.md
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-04 06:39:01.781777 iothpy-1.3.1/_skbuild/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-04 06:39:01.781777 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-04 06:39:01.781777 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-04 06:39:01.789777 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2779 2024-05-04 06:31:09.000000 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/__init__.py
--rw-r--r--   0 francesco  (1000) francesco  (1000)    87544 2024-05-04 06:31:09.000000 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/_const_linkadd.cpython-312-x86_64-linux-gnu.so
--rw-r--r--   0 francesco  (1000) francesco  (1000)   193896 2024-05-04 06:31:09.000000 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/_iothpy.cpython-312-x86_64-linux-gnu.so
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    14359 2024-05-04 06:31:09.000000 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/msocket.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2411 2024-05-04 06:31:09.000000 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/override.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4400 2024-05-04 06:31:09.000000 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/stack.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-04 06:39:01.793777 iothpy-1.3.1/iothpy/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2779 2024-05-04 06:34:10.000000 iothpy-1.3.1/iothpy/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    30003 2024-05-04 06:34:10.000000 iothpy-1.3.1/iothpy/const_linkadd.c
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7268 2024-05-04 06:34:10.000000 iothpy-1.3.1/iothpy/iothpy.c
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    78783 2024-03-26 14:33:52.000000 iothpy-1.3.1/iothpy/iothpy_socket.c
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      983 2024-03-26 14:33:52.000000 iothpy-1.3.1/iothpy/iothpy_socket.h
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    38819 2024-05-04 06:34:10.000000 iothpy-1.3.1/iothpy/iothpy_stack.c
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      260 2024-03-26 14:33:52.000000 iothpy-1.3.1/iothpy/iothpy_stack.h
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    14359 2024-03-26 14:33:52.000000 iothpy-1.3.1/iothpy/msocket.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2411 2024-03-26 14:33:52.000000 iothpy-1.3.1/iothpy/override.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4400 2024-04-04 11:20:54.000000 iothpy-1.3.1/iothpy/stack.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2892 2024-03-26 14:33:52.000000 iothpy-1.3.1/iothpy/utils.c
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      680 2024-03-26 14:33:52.000000 iothpy-1.3.1/iothpy/utils.h
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-04 06:39:01.797777 iothpy-1.3.1/iothpy.egg-info/
--rw-r--r--   0 francesco  (1000) francesco  (1000)     6516 2024-05-04 06:39:01.000000 iothpy-1.3.1/iothpy.egg-info/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      838 2024-05-04 06:39:01.000000 iothpy-1.3.1/iothpy.egg-info/SOURCES.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2024-05-04 06:39:01.000000 iothpy-1.3.1/iothpy.egg-info/dependency_links.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        7 2024-05-04 06:39:01.000000 iothpy-1.3.1/iothpy.egg-info/top_level.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       75 2024-03-26 14:33:52.000000 iothpy-1.3.1/pyproject.toml
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2024-05-04 06:39:01.797777 iothpy-1.3.1/setup.cfg
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1592 2024-05-04 06:34:10.000000 iothpy-1.3.1/setup.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-16 09:34:49.585854 iothpy-1.3.2/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2024-05-16 07:43:54.000000 iothpy-1.3.2/CMakeLists.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    26526 2024-03-26 14:33:52.000000 iothpy-1.3.2/LICENSE
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      145 2024-03-26 14:33:52.000000 iothpy-1.3.2/MANIFEST.in
+-rw-r--r--   0 francesco  (1000) francesco  (1000)     6516 2024-05-16 09:34:49.585854 iothpy-1.3.2/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     6180 2024-03-26 14:33:52.000000 iothpy-1.3.2/README.md
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-16 09:34:49.569854 iothpy-1.3.2/_skbuild/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-16 09:34:49.569854 iothpy-1.3.2/_skbuild/linux-x86_64-3.12/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-16 09:34:49.569854 iothpy-1.3.2/_skbuild/linux-x86_64-3.12/cmake-install/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-16 09:34:49.577854 iothpy-1.3.2/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2779 2024-05-16 07:44:06.000000 iothpy-1.3.2/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/__init__.py
+-rw-r--r--   0 francesco  (1000) francesco  (1000)    87544 2024-05-16 07:44:06.000000 iothpy-1.3.2/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/_const_linkadd.cpython-312-x86_64-linux-gnu.so
+-rw-r--r--   0 francesco  (1000) francesco  (1000)   193896 2024-05-16 07:44:06.000000 iothpy-1.3.2/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/_iothpy.cpython-312-x86_64-linux-gnu.so
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    14359 2024-05-16 07:44:06.000000 iothpy-1.3.2/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/msocket.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2411 2024-05-16 07:44:06.000000 iothpy-1.3.2/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/override.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4400 2024-05-16 07:44:06.000000 iothpy-1.3.2/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/stack.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-16 09:34:49.585854 iothpy-1.3.2/iothpy/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2779 2024-05-04 06:34:10.000000 iothpy-1.3.2/iothpy/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    30003 2024-05-04 06:34:10.000000 iothpy-1.3.2/iothpy/const_linkadd.c
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     7268 2024-05-04 06:34:10.000000 iothpy-1.3.2/iothpy/iothpy.c
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    78783 2024-03-26 14:33:52.000000 iothpy-1.3.2/iothpy/iothpy_socket.c
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      983 2024-03-26 14:33:52.000000 iothpy-1.3.2/iothpy/iothpy_socket.h
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    38819 2024-05-16 07:37:18.000000 iothpy-1.3.2/iothpy/iothpy_stack.c
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      260 2024-03-26 14:33:52.000000 iothpy-1.3.2/iothpy/iothpy_stack.h
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    14359 2024-03-26 14:33:52.000000 iothpy-1.3.2/iothpy/msocket.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2411 2024-03-26 14:33:52.000000 iothpy-1.3.2/iothpy/override.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4400 2024-04-04 11:20:54.000000 iothpy-1.3.2/iothpy/stack.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2892 2024-03-26 14:33:52.000000 iothpy-1.3.2/iothpy/utils.c
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      680 2024-03-26 14:33:52.000000 iothpy-1.3.2/iothpy/utils.h
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-16 09:34:49.585854 iothpy-1.3.2/iothpy.egg-info/
+-rw-r--r--   0 francesco  (1000) francesco  (1000)     6516 2024-05-16 09:34:49.000000 iothpy-1.3.2/iothpy.egg-info/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      838 2024-05-16 09:34:49.000000 iothpy-1.3.2/iothpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2024-05-16 09:34:49.000000 iothpy-1.3.2/iothpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        7 2024-05-16 09:34:49.000000 iothpy-1.3.2/iothpy.egg-info/top_level.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       75 2024-03-26 14:33:52.000000 iothpy-1.3.2/pyproject.toml
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2024-05-16 09:34:49.589854 iothpy-1.3.2/setup.cfg
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1592 2024-05-16 09:33:17.000000 iothpy-1.3.2/setup.py
```

### Comparing `iothpy-1.3.1/CMakeLists.txt` & `iothpy-1.3.2/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,14 @@
   if(NOT ${HEADER}_OK)
     message(FATAL_ERROR "header file ${HEADER} not found")
   endif()
 endforeach(HEADER)
 
 # Target for python extension module
 add_library(_iothpy MODULE iothpy/iothpy.c iothpy/iothpy_socket.c iothpy/iothpy_stack.c iothpy/utils.c)
-target_link_libraries(_iothpy -lioth -liothconf -liothdns)
+target_link_libraries(_iothpy -lioth -liothconf -liothdns -lpicoxnet)
 python_extension_module(_iothpy)
 
 add_library(_const_linkadd MODULE iothpy/const_linkadd.c)
 python_extension_module(_const_linkadd)
 
 install(TARGETS _iothpy _const_linkadd LIBRARY DESTINATION iothpy)
```

### Comparing `iothpy-1.3.1/LICENSE` & `iothpy-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/PKG-INFO` & `iothpy-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iothpy
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python library for internet of threads
 Home-page: https://github.com/ramenguy99/iothpy
 Author: Dario Mylonopoulos
 Author-email: dmylos@yahoo.it
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `iothpy-1.3.1/README.md` & `iothpy-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/__init__.py` & `iothpy-1.3.2/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/__init__.py`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/_const_linkadd.cpython-312-x86_64-linux-gnu.so` & `iothpy-1.3.2/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/_const_linkadd.cpython-312-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/_iothpy.cpython-312-x86_64-linux-gnu.so` & `iothpy-1.3.2/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/_iothpy.cpython-312-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/msocket.py` & `iothpy-1.3.2/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/msocket.py`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/override.py` & `iothpy-1.3.2/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/override.py`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/stack.py` & `iothpy-1.3.2/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/stack.py`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/iothpy/__init__.py` & `iothpy-1.3.2/iothpy/__init__.py`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/iothpy/const_linkadd.c` & `iothpy-1.3.2/iothpy/const_linkadd.c`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/iothpy/iothpy.c` & `iothpy-1.3.2/iothpy/iothpy.c`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/iothpy/iothpy_socket.c` & `iothpy-1.3.2/iothpy/iothpy_socket.c`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/iothpy/iothpy_socket.h` & `iothpy-1.3.2/iothpy/iothpy_socket.h`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/iothpy/iothpy_stack.c` & `iothpy-1.3.2/iothpy/iothpy_stack.c`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/iothpy/msocket.py` & `iothpy-1.3.2/iothpy/msocket.py`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/iothpy/override.py` & `iothpy-1.3.2/iothpy/override.py`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/iothpy/stack.py` & `iothpy-1.3.2/iothpy/stack.py`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/iothpy/utils.c` & `iothpy-1.3.2/iothpy/utils.c`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/iothpy/utils.h` & `iothpy-1.3.2/iothpy/utils.h`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/iothpy.egg-info/PKG-INFO` & `iothpy-1.3.2/iothpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iothpy
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python library for internet of threads
 Home-page: https://github.com/ramenguy99/iothpy
 Author: Dario Mylonopoulos
 Author-email: dmylos@yahoo.it
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `iothpy-1.3.1/iothpy.egg-info/SOURCES.txt` & `iothpy-1.3.2/iothpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.1/setup.py` & `iothpy-1.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 long_description = ""
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup (
        #setuptools options
        name = 'iothpy',
-       version = '1.3.1',
+       version = '1.3.2',
        author = 'Dario Mylonopoulos',
        author_email = 'dmylos@yahoo.it',
        url = 'https://github.com/ramenguy99/iothpy',
        description = 'Python library for internet of threads',
        long_description = long_description,
        long_description_content_type="text/markdown",
        packages = ["iothpy"],
```

