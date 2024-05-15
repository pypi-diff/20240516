# Comparing `tmp/extractcode_libarchive_system_provided-3.5.1.210531.tar.gz` & `tmp/extractcode_libarchive_system_provided-32.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/extractcode_libarchive_system_provided-3.5.1.210531.tar", last modified: Mon May 31 10:38:26 2021, max compression
+gzip compressed data, was "extractcode_libarchive_system_provided-32.0.0.tar", last modified: Wed May 15 23:52:57 2024, max compression
```

## Comparing `extractcode_libarchive_system_provided-3.5.1.210531.tar` & `extractcode_libarchive_system_provided-32.0.0.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxrwxr-x   0 pombreda  (1000) pombreda  (1000)        0 2021-05-31 10:38:26.000000 extractcode_libarchive_system_provided-3.5.1.210531/
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)      274 2021-04-23 08:43:12.000000 extractcode_libarchive_system_provided-3.5.1.210531/README.rst
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)     7216 2020-12-21 18:18:50.000000 extractcode_libarchive_system_provided-3.5.1.210531/LICENSE.txt
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)      210 2021-05-31 10:38:26.000000 extractcode_libarchive_system_provided-3.5.1.210531/setup.cfg
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)       93 2021-03-30 11:59:07.000000 extractcode_libarchive_system_provided-3.5.1.210531/MANIFEST.in
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)    11358 2021-03-30 11:59:06.000000 extractcode_libarchive_system_provided-3.5.1.210531/apache-2.0.LICENSE
-drwxrwxr-x   0 pombreda  (1000) pombreda  (1000)        0 2021-05-31 10:38:26.000000 extractcode_libarchive_system_provided-3.5.1.210531/src/
-drwxrwxr-x   0 pombreda  (1000) pombreda  (1000)        0 2021-05-31 10:38:26.000000 extractcode_libarchive_system_provided-3.5.1.210531/src/extractcode_libarchive_system_provided.egg-info/
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)        1 2021-01-22 13:06:59.000000 extractcode_libarchive_system_provided-3.5.1.210531/src/extractcode_libarchive_system_provided.egg-info/not-zip-safe
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)      509 2021-05-31 10:38:26.000000 extractcode_libarchive_system_provided-3.5.1.210531/src/extractcode_libarchive_system_provided.egg-info/SOURCES.txt
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)       94 2021-05-31 10:38:26.000000 extractcode_libarchive_system_provided-3.5.1.210531/src/extractcode_libarchive_system_provided.egg-info/entry_points.txt
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)        1 2021-05-31 10:38:26.000000 extractcode_libarchive_system_provided-3.5.1.210531/src/extractcode_libarchive_system_provided.egg-info/dependency_links.txt
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)       23 2021-05-31 10:38:26.000000 extractcode_libarchive_system_provided-3.5.1.210531/src/extractcode_libarchive_system_provided.egg-info/top_level.txt
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)      634 2021-05-31 10:38:26.000000 extractcode_libarchive_system_provided-3.5.1.210531/src/extractcode_libarchive_system_provided.egg-info/PKG-INFO
-drwxrwxr-x   0 pombreda  (1000) pombreda  (1000)        0 2021-05-31 10:38:26.000000 extractcode_libarchive_system_provided-3.5.1.210531/src/extractcode_libarchive/
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)     1984 2021-05-30 20:04:44.000000 extractcode_libarchive_system_provided-3.5.1.210531/src/extractcode_libarchive/__init__.py
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)     1288 2021-05-31 10:24:56.000000 extractcode_libarchive_system_provided-3.5.1.210531/setup.py
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)      634 2021-05-31 10:38:26.000000 extractcode_libarchive_system_provided-3.5.1.210531/PKG-INFO
+drwxr-xr-x   0 jono       (501) staff       (20)        0 2024-05-15 23:52:57.479456 extractcode_libarchive_system_provided-32.0.0/
+-rwxr-xr-x   0 jono       (501) staff       (20)     7216 2024-04-30 00:28:14.000000 extractcode_libarchive_system_provided-32.0.0/LICENSE.txt
+-rwxr-xr-x   0 jono       (501) staff       (20)       93 2024-04-30 00:28:14.000000 extractcode_libarchive_system_provided-32.0.0/MANIFEST.in
+-rw-r--r--   0 jono       (501) staff       (20)      682 2024-05-15 23:52:57.479523 extractcode_libarchive_system_provided-32.0.0/PKG-INFO
+-rwxr-xr-x   0 jono       (501) staff       (20)      274 2024-04-30 00:28:14.000000 extractcode_libarchive_system_provided-32.0.0/README.rst
+-rw-r--r--   0 jono       (501) staff       (20)    11358 2024-04-30 00:28:14.000000 extractcode_libarchive_system_provided-32.0.0/apache-2.0.LICENSE
+-rwxr-xr-x   0 jono       (501) staff       (20)      210 2024-05-15 23:52:57.479742 extractcode_libarchive_system_provided-32.0.0/setup.cfg
+-rwxr-xr-x   0 jono       (501) staff       (20)     1282 2024-05-15 23:50:33.000000 extractcode_libarchive_system_provided-32.0.0/setup.py
+drwxr-xr-x   0 jono       (501) staff       (20)        0 2024-05-15 23:52:57.476635 extractcode_libarchive_system_provided-32.0.0/src/
+drwxr-xr-x   0 jono       (501) staff       (20)        0 2024-05-15 23:52:57.477560 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive/
+-rwxr-xr-x   0 jono       (501) staff       (20)     2684 2024-05-15 23:50:33.000000 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive/__init__.py
+drwxr-xr-x   0 jono       (501) staff       (20)        0 2024-05-15 23:52:57.478524 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive/__pycache__/
+-rw-r--r--   0 jono       (501) staff       (20)     1879 2024-05-02 18:01:23.000000 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive/__pycache__/__init__.cpython-310-pytest-7.1.2.pyc
+-rw-r--r--   0 jono       (501) staff       (20)     1772 2024-05-01 02:27:14.000000 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive/__pycache__/__init__.cpython-310-pytest-8.2.0.pyc
+-rw-r--r--   0 jono       (501) staff       (20)     1770 2024-05-02 18:03:11.000000 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 jono       (501) staff       (20)     2896 2024-05-15 16:07:59.000000 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive/__pycache__/__init__.cpython-311-pytest-7.1.2.pyc
+-rw-r--r--   0 jono       (501) staff       (20)     2761 2024-05-15 16:08:08.000000 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jono       (501) staff       (20)     2448 2024-05-01 03:06:30.000000 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive/__pycache__/__init__.cpython-312-pytest-7.1.2.pyc
+-rw-r--r--   0 jono       (501) staff       (20)     2643 2024-05-14 23:53:14.000000 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive/__pycache__/__init__.cpython-312-pytest-8.2.0.pyc
+-rw-r--r--   0 jono       (501) staff       (20)     2530 2024-05-14 23:53:30.000000 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive/__pycache__/__init__.cpython-312.pyc
+drwxr-xr-x   0 jono       (501) staff       (20)        0 2024-05-15 23:52:57.479345 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive_system_provided.egg-info/
+-rw-r--r--   0 jono       (501) staff       (20)      682 2024-05-15 23:52:57.000000 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive_system_provided.egg-info/PKG-INFO
+-rw-r--r--   0 jono       (501) staff       (20)     1086 2024-05-15 23:52:57.000000 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive_system_provided.egg-info/SOURCES.txt
+-rw-r--r--   0 jono       (501) staff       (20)        1 2024-05-15 23:52:57.000000 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive_system_provided.egg-info/dependency_links.txt
+-rw-r--r--   0 jono       (501) staff       (20)       93 2024-05-15 23:52:57.000000 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive_system_provided.egg-info/entry_points.txt
+-rw-r--r--   0 jono       (501) staff       (20)        1 2024-04-30 01:23:13.000000 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive_system_provided.egg-info/not-zip-safe
+-rw-r--r--   0 jono       (501) staff       (20)       23 2024-05-15 23:52:57.000000 extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive_system_provided.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `extractcode_libarchive_system_provided-3.5.1.210531/LICENSE.txt` & `extractcode_libarchive_system_provided-32.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `extractcode_libarchive_system_provided-3.5.1.210531/apache-2.0.LICENSE` & `extractcode_libarchive_system_provided-32.0.0/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `extractcode_libarchive_system_provided-3.5.1.210531/src/extractcode_libarchive_system_provided.egg-info/PKG-INFO` & `extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive_system_provided.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: extractcode-libarchive-system-provided
-Version: 3.5.1.210531
+Version: 32.0.0
 Summary: A ScanCode path provider plugin to provide a system package provided libarchive shared library.
 Home-page: https://github.com/nexB/scancode-plugins
 Author: nexB
 Author-email: info@aboutcode.org
 License: apache-2.0 AND bsd-simplified
-Description: A ScanCode path provider plugin to provide a system package provided libarchive shared library.
 Keywords: open source,extractcode,libarchive
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
+License-File: LICENSE.txt
+License-File: README.rst
+License-File: apache-2.0.LICENSE
+
+A ScanCode path provider plugin to provide a system package provided libarchive shared library.
```

### Comparing `extractcode_libarchive_system_provided-3.5.1.210531/src/extractcode_libarchive/__init__.py` & `extractcode_libarchive_system_provided-32.0.0/src/extractcode_libarchive/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,34 +21,46 @@
         locations of the libarchive shared library as installed on various Linux
         distros or on FreeBSD.
         """
         lib_archive = environ.get('EXTRACTCODE_LIBARCHIVE_PATH')
         if not lib_archive:
             system_arch = platform.machine()
             mainstream_system = platform.system().lower()
+
             if mainstream_system == 'linux':
                 distribution = platform.linux_distribution()[0].lower()
                 debian_based_distro = ['ubuntu', 'mint', 'debian']
                 rpm_based_distro = ['fedora', 'redhat']
 
                 if distribution in debian_based_distro:
                     lib_dir = '/usr/lib/'+system_arch+'-linux-gnu'
-
                 elif distribution in rpm_based_distro:
                     lib_dir = '/usr/lib64'
-
                 else:
                     raise Exception('Unsupported system: {}'.format(distribution))
 
+                lib_archive = path.join(lib_dir, 'libarchive.so.13')
             elif mainstream_system == 'freebsd':
-                if path.isdir('/usr/local/'):
-                    lib_dir = '/usr/local/lib'
-                else:
-                    lib_dir = '/usr/lib'
-            lib_archive = path.join(lib_dir, 'libarchive.so')
+                lib_archive = ''
+                for lib_dir in ('/usr/local/lib', '/usr/lib'):
+                    possible_lib_archive = path.join(lib_dir, 'libarchive.so')
+                    if path.exists(possible_lib_archive):
+                        lib_archive = possible_lib_archive
+                        break
+            elif mainstream_system == 'darwin':
+                # This assumes that libarchive was installed using Homebrew
+                lib_dir = '/opt/homebrew/opt/libarchive/lib'
+                lib_archive = path.join(lib_dir, 'libarchive.dylib')
         else:
             lib_dir = path.dirname(lib_archive)
 
+        # Check that path exists
+        if not path.exists(lib_archive):
+            raise Exception(
+                'libarchive not found. Please refer to the scancode-toolkit '
+                'documentation on how to install libarchive for your system.'
+            )
+
         locations = {
             'extractcode.libarchive.dll': lib_archive,
         }
         return locations
```

### Comparing `extractcode_libarchive_system_provided-3.5.1.210531/setup.py` & `extractcode_libarchive_system_provided-32.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup
 
 
 desc = '''A ScanCode path provider plugin to provide a system package provided libarchive shared library.'''
 
 setup(
     name='extractcode_libarchive_system_provided',
-    version='3.5.1.210531',
+    version='32.0.0',
     license='apache-2.0 AND bsd-simplified',
     description=desc,
     long_description=desc,
     author='nexB',
     author_email='info@aboutcode.org',
     url='https://github.com/nexB/scancode-plugins',
     packages=find_packages('src'),
```

### Comparing `extractcode_libarchive_system_provided-3.5.1.210531/PKG-INFO` & `extractcode_libarchive_system_provided-32.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: extractcode_libarchive_system_provided
-Version: 3.5.1.210531
+Version: 32.0.0
 Summary: A ScanCode path provider plugin to provide a system package provided libarchive shared library.
 Home-page: https://github.com/nexB/scancode-plugins
 Author: nexB
 Author-email: info@aboutcode.org
 License: apache-2.0 AND bsd-simplified
-Description: A ScanCode path provider plugin to provide a system package provided libarchive shared library.
 Keywords: open source,extractcode,libarchive
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
+License-File: LICENSE.txt
+License-File: README.rst
+License-File: apache-2.0.LICENSE
+
+A ScanCode path provider plugin to provide a system package provided libarchive shared library.
```

