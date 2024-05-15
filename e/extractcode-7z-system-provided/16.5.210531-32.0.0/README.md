# Comparing `tmp/extractcode_7z_system_provided-16.5.210531.tar.gz` & `tmp/extractcode_7z_system_provided-32.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/extractcode_7z_system_provided-16.5.210531.tar", last modified: Mon May 31 10:38:24 2021, max compression
+gzip compressed data, was "extractcode_7z_system_provided-32.0.0.tar", last modified: Wed May 15 23:52:37 2024, max compression
```

## Comparing `extractcode_7z_system_provided-16.5.210531.tar` & `extractcode_7z_system_provided-32.0.0.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxrwxr-x   0 pombreda  (1000) pombreda  (1000)        0 2021-05-31 10:38:24.000000 extractcode_7z_system_provided-16.5.210531/
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)      253 2021-04-23 08:43:12.000000 extractcode_7z_system_provided-16.5.210531/README.rst
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)     2814 2020-12-21 18:18:50.000000 extractcode_7z_system_provided-16.5.210531/LICENSE.txt
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)      210 2021-05-31 10:38:24.000000 extractcode_7z_system_provided-16.5.210531/setup.cfg
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)       93 2021-03-30 11:59:05.000000 extractcode_7z_system_provided-16.5.210531/MANIFEST.in
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)    11358 2021-03-30 11:59:07.000000 extractcode_7z_system_provided-16.5.210531/apache-2.0.LICENSE
-drwxrwxr-x   0 pombreda  (1000) pombreda  (1000)        0 2021-05-31 10:38:24.000000 extractcode_7z_system_provided-16.5.210531/src/
-drwxrwxr-x   0 pombreda  (1000) pombreda  (1000)        0 2021-05-31 10:38:24.000000 extractcode_7z_system_provided-16.5.210531/src/extractcode_7z_system_provided.egg-info/
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)        1 2021-01-22 13:06:57.000000 extractcode_7z_system_provided-16.5.210531/src/extractcode_7z_system_provided.egg-info/not-zip-safe
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)      453 2021-05-31 10:38:24.000000 extractcode_7z_system_provided-16.5.210531/src/extractcode_7z_system_provided.egg-info/SOURCES.txt
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)       78 2021-05-31 10:38:24.000000 extractcode_7z_system_provided-16.5.210531/src/extractcode_7z_system_provided.egg-info/entry_points.txt
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)        1 2021-05-31 10:38:24.000000 extractcode_7z_system_provided-16.5.210531/src/extractcode_7z_system_provided.egg-info/dependency_links.txt
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)       15 2021-05-31 10:38:24.000000 extractcode_7z_system_provided-16.5.210531/src/extractcode_7z_system_provided.egg-info/top_level.txt
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)      632 2021-05-31 10:38:24.000000 extractcode_7z_system_provided-16.5.210531/src/extractcode_7z_system_provided.egg-info/PKG-INFO
-drwxrwxr-x   0 pombreda  (1000) pombreda  (1000)        0 2021-05-31 10:38:24.000000 extractcode_7z_system_provided-16.5.210531/src/extractcode_7z/
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)     2012 2021-05-30 20:04:44.000000 extractcode_7z_system_provided-16.5.210531/src/extractcode_7z/__init__.py
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)     1282 2021-05-31 10:24:56.000000 extractcode_7z_system_provided-16.5.210531/setup.py
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)      632 2021-05-31 10:38:24.000000 extractcode_7z_system_provided-16.5.210531/PKG-INFO
+drwxr-xr-x   0 jono       (501) staff       (20)        0 2024-05-15 23:52:37.526549 extractcode_7z_system_provided-32.0.0/
+-rwxr-xr-x   0 jono       (501) staff       (20)     2814 2024-04-30 00:28:14.000000 extractcode_7z_system_provided-32.0.0/LICENSE.txt
+-rwxr-xr-x   0 jono       (501) staff       (20)       93 2024-04-30 00:28:14.000000 extractcode_7z_system_provided-32.0.0/MANIFEST.in
+-rw-r--r--   0 jono       (501) staff       (20)      681 2024-05-15 23:52:37.526671 extractcode_7z_system_provided-32.0.0/PKG-INFO
+-rwxr-xr-x   0 jono       (501) staff       (20)      253 2024-04-30 00:28:14.000000 extractcode_7z_system_provided-32.0.0/README.rst
+-rw-r--r--   0 jono       (501) staff       (20)    11358 2024-04-30 00:28:14.000000 extractcode_7z_system_provided-32.0.0/apache-2.0.LICENSE
+-rwxr-xr-x   0 jono       (501) staff       (20)      210 2024-05-15 23:52:37.526926 extractcode_7z_system_provided-32.0.0/setup.cfg
+-rwxr-xr-x   0 jono       (501) staff       (20)     1277 2024-05-15 23:50:33.000000 extractcode_7z_system_provided-32.0.0/setup.py
+drwxr-xr-x   0 jono       (501) staff       (20)        0 2024-05-15 23:52:37.523584 extractcode_7z_system_provided-32.0.0/src/
+drwxr-xr-x   0 jono       (501) staff       (20)        0 2024-05-15 23:52:37.524532 extractcode_7z_system_provided-32.0.0/src/extractcode_7z/
+-rwxr-xr-x   0 jono       (501) staff       (20)     2593 2024-05-15 23:50:33.000000 extractcode_7z_system_provided-32.0.0/src/extractcode_7z/__init__.py
+drwxr-xr-x   0 jono       (501) staff       (20)        0 2024-05-15 23:52:37.525642 extractcode_7z_system_provided-32.0.0/src/extractcode_7z/__pycache__/
+-rw-r--r--   0 jono       (501) staff       (20)     1740 2024-05-07 22:59:44.000000 extractcode_7z_system_provided-32.0.0/src/extractcode_7z/__pycache__/__init__.cpython-310-pytest-7.1.2.pyc
+-rw-r--r--   0 jono       (501) staff       (20)     1634 2024-05-01 02:27:14.000000 extractcode_7z_system_provided-32.0.0/src/extractcode_7z/__pycache__/__init__.cpython-310-pytest-8.2.0.pyc
+-rw-r--r--   0 jono       (501) staff       (20)     1631 2024-05-07 23:00:04.000000 extractcode_7z_system_provided-32.0.0/src/extractcode_7z/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 jono       (501) staff       (20)     2678 2024-05-15 16:07:59.000000 extractcode_7z_system_provided-32.0.0/src/extractcode_7z/__pycache__/__init__.cpython-311-pytest-7.1.2.pyc
+-rw-r--r--   0 jono       (501) staff       (20)     2543 2024-05-15 16:08:08.000000 extractcode_7z_system_provided-32.0.0/src/extractcode_7z/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jono       (501) staff       (20)     2115 2024-05-01 03:06:30.000000 extractcode_7z_system_provided-32.0.0/src/extractcode_7z/__pycache__/__init__.cpython-312-pytest-7.1.2.pyc
+-rw-r--r--   0 jono       (501) staff       (20)     2425 2024-05-14 23:53:14.000000 extractcode_7z_system_provided-32.0.0/src/extractcode_7z/__pycache__/__init__.cpython-312-pytest-8.2.0.pyc
+-rw-r--r--   0 jono       (501) staff       (20)     2312 2024-05-14 23:53:30.000000 extractcode_7z_system_provided-32.0.0/src/extractcode_7z/__pycache__/__init__.cpython-312.pyc
+drwxr-xr-x   0 jono       (501) staff       (20)        0 2024-05-15 23:52:37.526439 extractcode_7z_system_provided-32.0.0/src/extractcode_7z_system_provided.egg-info/
+-rw-r--r--   0 jono       (501) staff       (20)      681 2024-05-15 23:52:37.000000 extractcode_7z_system_provided-32.0.0/src/extractcode_7z_system_provided.egg-info/PKG-INFO
+-rw-r--r--   0 jono       (501) staff       (20)      966 2024-05-15 23:52:37.000000 extractcode_7z_system_provided-32.0.0/src/extractcode_7z_system_provided.egg-info/SOURCES.txt
+-rw-r--r--   0 jono       (501) staff       (20)        1 2024-05-15 23:52:37.000000 extractcode_7z_system_provided-32.0.0/src/extractcode_7z_system_provided.egg-info/dependency_links.txt
+-rw-r--r--   0 jono       (501) staff       (20)       77 2024-05-15 23:52:37.000000 extractcode_7z_system_provided-32.0.0/src/extractcode_7z_system_provided.egg-info/entry_points.txt
+-rw-r--r--   0 jono       (501) staff       (20)        1 2024-04-30 01:22:56.000000 extractcode_7z_system_provided-32.0.0/src/extractcode_7z_system_provided.egg-info/not-zip-safe
+-rw-r--r--   0 jono       (501) staff       (20)       15 2024-05-15 23:52:37.000000 extractcode_7z_system_provided-32.0.0/src/extractcode_7z_system_provided.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `extractcode_7z_system_provided-16.5.210531/LICENSE.txt` & `extractcode_7z_system_provided-32.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `extractcode_7z_system_provided-16.5.210531/apache-2.0.LICENSE` & `extractcode_7z_system_provided-32.0.0/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `extractcode_7z_system_provided-16.5.210531/src/extractcode_7z_system_provided.egg-info/PKG-INFO` & `extractcode_7z_system_provided-32.0.0/src/extractcode_7z_system_provided.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: extractcode-7z-system-provided
-Version: 16.5.210531
+Version: 32.0.0
 Summary: A ScanCode path provider plugin to provide system package provided sevenzip binary.
 Home-page: https://github.com/nexB/scancode-plugins
 Author: nexB
 Author-email: info@aboutcode.org
 License: apache-2.0 AND lgpl-2.1 and unrar and brian-gladman-3-clause
-Description: A ScanCode path provider plugin to provide system package provided sevenzip binary.
 Keywords: open source,extractcode,libarchive
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
+License-File: LICENSE.txt
+License-File: README.rst
+License-File: apache-2.0.LICENSE
+
+A ScanCode path provider plugin to provide system package provided sevenzip binary.
```

### Comparing `extractcode_7z_system_provided-16.5.210531/src/extractcode_7z/__init__.py` & `extractcode_7z_system_provided-32.0.0/src/extractcode_7z/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,34 +23,45 @@
         locations of the 7zip exe and shared libraries as installed on various
         Linux distros or on FreeBSD.
         """
         lib_dir = None
         lib_7z = environ.get('EXTRACTCODE_7Z_PATH')
         if not lib_7z:
             mainstream_system = platform.system().lower()
+
             if mainstream_system == 'linux':
                 distribution = platform.linux_distribution()[0].lower()
                 debian_based_distro = ['ubuntu', 'mint', 'debian']
                 rpm_based_distro = ['fedora', 'redhat']
 
                 if distribution in debian_based_distro:
                     lib_dir = '/usr/lib/p7zip'
-
+                    lib_7z = path.join(lib_dir, '7zr')
                 elif distribution in rpm_based_distro:
                     lib_dir = '/usr/libexec/p7zip'
-
+                    lib_7z = path.join(lib_dir, '7za')
                 else:
                     raise Exception('Unsupported system: {}'.format(distribution))
             elif mainstream_system == 'freebsd':
-                lib_dir = '/usr/local/libexec/p7zip'
-            lib_7z = path.join(lib_dir, '7z')
+                lib_dir = '/usr/local/bin'
+                lib_7z = path.join(lib_dir, '7z')
+            elif mainstream_system == 'darwin':
+                # This assumes that p7zip was installed using Homebrew
+                lib_dir = '/opt/homebrew/lib/p7zip'
+                lib_7z = path.join(lib_dir, '7z')
         else:
             lib_dir = path.dirname(lib_7z)
 
+        # Check that path exist
+        if not path.exists(lib_7z):
+            raise Exception(
+                'p7zip not found. Please refer to the scancode-toolkit '
+                'documentation on how to install p7zip for your system.'
+            )
+
         locations = {
             # extractcode.sevenzip.libdir is not used anymore and deprecated
             # but we are keeping it around for now for backward compatibility
             'extractcode.sevenzip.libdir': lib_dir,
             'extractcode.sevenzip.exe': lib_7z,
         }
-
         return locations
```

### Comparing `extractcode_7z_system_provided-16.5.210531/setup.py` & `extractcode_7z_system_provided-32.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup
 
 
 desc = '''A ScanCode path provider plugin to provide system package provided sevenzip binary.'''
 
 setup(
     name='extractcode_7z_system_provided',
-    version='16.5.210531',
+    version='32.0.0',
     license='apache-2.0 AND lgpl-2.1 and unrar and brian-gladman-3-clause',
     description=desc,
     long_description=desc,
     author='nexB',
     author_email='info@aboutcode.org',
     url='https://github.com/nexB/scancode-plugins',
     packages=find_packages('src'),
```

### Comparing `extractcode_7z_system_provided-16.5.210531/PKG-INFO` & `extractcode_7z_system_provided-32.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: extractcode_7z_system_provided
-Version: 16.5.210531
+Version: 32.0.0
 Summary: A ScanCode path provider plugin to provide system package provided sevenzip binary.
 Home-page: https://github.com/nexB/scancode-plugins
 Author: nexB
 Author-email: info@aboutcode.org
 License: apache-2.0 AND lgpl-2.1 and unrar and brian-gladman-3-clause
-Description: A ScanCode path provider plugin to provide system package provided sevenzip binary.
 Keywords: open source,extractcode,libarchive
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
+License-File: LICENSE.txt
+License-File: README.rst
+License-File: apache-2.0.LICENSE
+
+A ScanCode path provider plugin to provide system package provided sevenzip binary.
```

