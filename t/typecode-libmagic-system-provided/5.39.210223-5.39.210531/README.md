# Comparing `tmp/typecode_libmagic-system-provided-5.39.210223.tar.gz` & `tmp/typecode_libmagic-system-provided-5.39.210531.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/typecode_libmagic-system-provided-5.39.210223.tar", last modified: Tue Feb 23 23:51:19 2021, max compression
+gzip compressed data, was "dist/typecode_libmagic-system-provided-5.39.210531.tar", last modified: Mon May 31 10:39:29 2021, max compression
```

## Comparing `typecode_libmagic-system-provided-5.39.210223.tar` & `typecode_libmagic-system-provided-5.39.210531.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 pombreda  (1000) pombreda  (1000)        0 2021-02-23 23:51:19.000000 typecode_libmagic-system-provided-5.39.210223/
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)       86 2020-12-21 18:18:50.000000 typecode_libmagic-system-provided-5.39.210223/README.rst
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)     1435 2021-01-22 10:34:21.000000 typecode_libmagic-system-provided-5.39.210223/bsd-simplified-darwin.LICENSE
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)      404 2021-02-23 23:51:19.000000 typecode_libmagic-system-provided-5.39.210223/setup.cfg
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)     1229 2021-01-22 10:41:21.000000 typecode_libmagic-system-provided-5.39.210223/bsd-simplified.LICENSE
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)       93 2021-02-16 07:04:29.000000 typecode_libmagic-system-provided-5.39.210223/MANIFEST.in
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)    11358 2020-05-11 16:21:47.000000 typecode_libmagic-system-provided-5.39.210223/apache-2.0.LICENSE
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)     2247 2021-01-22 11:06:47.000000 typecode_libmagic-system-provided-5.39.210223/libmagic.ABOUT
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)     1571 2021-01-22 10:42:40.000000 typecode_libmagic-system-provided-5.39.210223/bsd-original.LICENSE
-drwxrwxr-x   0 pombreda  (1000) pombreda  (1000)        0 2021-02-23 23:51:19.000000 typecode_libmagic-system-provided-5.39.210223/src/
-drwxrwxr-x   0 pombreda  (1000) pombreda  (1000)        0 2021-02-23 23:51:19.000000 typecode_libmagic-system-provided-5.39.210223/src/typecode_libmagic_system_provided.egg-info/
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)        1 2021-01-22 13:07:12.000000 typecode_libmagic-system-provided-5.39.210223/src/typecode_libmagic_system_provided.egg-info/not-zip-safe
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)      678 2021-02-23 23:51:19.000000 typecode_libmagic-system-provided-5.39.210223/src/typecode_libmagic_system_provided.egg-info/SOURCES.txt
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)       82 2021-02-23 23:51:19.000000 typecode_libmagic-system-provided-5.39.210223/src/typecode_libmagic_system_provided.egg-info/entry_points.txt
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)        1 2021-02-23 23:51:19.000000 typecode_libmagic-system-provided-5.39.210223/src/typecode_libmagic_system_provided.egg-info/dependency_links.txt
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)       18 2021-02-23 23:51:19.000000 typecode_libmagic-system-provided-5.39.210223/src/typecode_libmagic_system_provided.egg-info/top_level.txt
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)      742 2021-02-23 23:51:19.000000 typecode_libmagic-system-provided-5.39.210223/src/typecode_libmagic_system_provided.egg-info/PKG-INFO
-drwxrwxr-x   0 pombreda  (1000) pombreda  (1000)        0 2021-02-23 23:51:19.000000 typecode_libmagic-system-provided-5.39.210223/src/typecode_libmagic/
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)     2994 2021-01-22 11:12:48.000000 typecode_libmagic-system-provided-5.39.210223/src/typecode_libmagic/__init__.py
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)      697 2021-01-22 10:41:53.000000 typecode_libmagic-system-provided-5.39.210223/isc.LICENSE
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)     1861 2021-01-22 11:06:47.000000 typecode_libmagic-system-provided-5.39.210223/libmagic.NOTICE
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)    12512 2021-01-22 10:42:25.000000 typecode_libmagic-system-provided-5.39.210223/gpl-1.0.LICENSE
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)      508 2021-01-22 11:06:04.000000 typecode_libmagic-system-provided-5.39.210223/typecode-libmagic.ABOUT
--rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)     1408 2021-02-23 09:32:48.000000 typecode_libmagic-system-provided-5.39.210223/setup.py
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)        0 2021-01-22 10:42:59.000000 typecode_libmagic-system-provided-5.39.210223/public-domain.LICENSE
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)     1414 2021-01-22 10:41:41.000000 typecode_libmagic-system-provided-5.39.210223/bsd-new.LICENSE
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)      742 2021-02-23 23:51:19.000000 typecode_libmagic-system-provided-5.39.210223/PKG-INFO
--rw-rw-r--   0 pombreda  (1000) pombreda  (1000)      644 2021-01-22 10:42:15.000000 typecode_libmagic-system-provided-5.39.210223/gpl-1.0-plus.LICENSE
+drwxrwxr-x   0 pombreda  (1000) pombreda  (1000)        0 2021-05-31 10:39:29.000000 typecode_libmagic-system-provided-5.39.210531/
+-rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)      166 2021-05-30 20:04:44.000000 typecode_libmagic-system-provided-5.39.210531/README.rst
+-rw-rw-r--   0 pombreda  (1000) pombreda  (1000)     1435 2021-03-30 11:59:06.000000 typecode_libmagic-system-provided-5.39.210531/bsd-simplified-darwin.LICENSE
+-rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)      404 2021-05-31 10:39:29.000000 typecode_libmagic-system-provided-5.39.210531/setup.cfg
+-rw-rw-r--   0 pombreda  (1000) pombreda  (1000)     1229 2021-03-30 11:59:05.000000 typecode_libmagic-system-provided-5.39.210531/bsd-simplified.LICENSE
+-rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)       93 2021-03-30 11:59:05.000000 typecode_libmagic-system-provided-5.39.210531/MANIFEST.in
+-rw-rw-r--   0 pombreda  (1000) pombreda  (1000)    11358 2021-03-30 11:59:07.000000 typecode_libmagic-system-provided-5.39.210531/apache-2.0.LICENSE
+-rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)     2247 2021-03-30 11:59:06.000000 typecode_libmagic-system-provided-5.39.210531/libmagic.ABOUT
+-rw-rw-r--   0 pombreda  (1000) pombreda  (1000)     1571 2021-03-30 11:59:07.000000 typecode_libmagic-system-provided-5.39.210531/bsd-original.LICENSE
+drwxrwxr-x   0 pombreda  (1000) pombreda  (1000)        0 2021-05-31 10:39:29.000000 typecode_libmagic-system-provided-5.39.210531/src/
+drwxrwxr-x   0 pombreda  (1000) pombreda  (1000)        0 2021-05-31 10:39:29.000000 typecode_libmagic-system-provided-5.39.210531/src/typecode_libmagic_system_provided.egg-info/
+-rw-rw-r--   0 pombreda  (1000) pombreda  (1000)        1 2021-01-22 13:07:12.000000 typecode_libmagic-system-provided-5.39.210531/src/typecode_libmagic_system_provided.egg-info/not-zip-safe
+-rw-rw-r--   0 pombreda  (1000) pombreda  (1000)      678 2021-05-31 10:39:29.000000 typecode_libmagic-system-provided-5.39.210531/src/typecode_libmagic_system_provided.egg-info/SOURCES.txt
+-rw-rw-r--   0 pombreda  (1000) pombreda  (1000)       82 2021-05-31 10:39:28.000000 typecode_libmagic-system-provided-5.39.210531/src/typecode_libmagic_system_provided.egg-info/entry_points.txt
+-rw-rw-r--   0 pombreda  (1000) pombreda  (1000)        1 2021-05-31 10:39:28.000000 typecode_libmagic-system-provided-5.39.210531/src/typecode_libmagic_system_provided.egg-info/dependency_links.txt
+-rw-rw-r--   0 pombreda  (1000) pombreda  (1000)       18 2021-05-31 10:39:28.000000 typecode_libmagic-system-provided-5.39.210531/src/typecode_libmagic_system_provided.egg-info/top_level.txt
+-rw-rw-r--   0 pombreda  (1000) pombreda  (1000)      742 2021-05-31 10:39:28.000000 typecode_libmagic-system-provided-5.39.210531/src/typecode_libmagic_system_provided.egg-info/PKG-INFO
+drwxrwxr-x   0 pombreda  (1000) pombreda  (1000)        0 2021-05-31 10:39:29.000000 typecode_libmagic-system-provided-5.39.210531/src/typecode_libmagic/
+-rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)     3196 2021-05-30 20:04:44.000000 typecode_libmagic-system-provided-5.39.210531/src/typecode_libmagic/__init__.py
+-rw-rw-r--   0 pombreda  (1000) pombreda  (1000)      697 2021-03-30 11:59:05.000000 typecode_libmagic-system-provided-5.39.210531/isc.LICENSE
+-rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)     1861 2021-03-30 11:59:07.000000 typecode_libmagic-system-provided-5.39.210531/libmagic.NOTICE
+-rw-rw-r--   0 pombreda  (1000) pombreda  (1000)    12512 2021-03-30 11:59:05.000000 typecode_libmagic-system-provided-5.39.210531/gpl-1.0.LICENSE
+-rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)      508 2021-03-30 11:59:05.000000 typecode_libmagic-system-provided-5.39.210531/typecode-libmagic.ABOUT
+-rwxrwxr-x   0 pombreda  (1000) pombreda  (1000)     1408 2021-05-31 10:24:56.000000 typecode_libmagic-system-provided-5.39.210531/setup.py
+-rw-rw-r--   0 pombreda  (1000) pombreda  (1000)        0 2021-03-30 11:59:05.000000 typecode_libmagic-system-provided-5.39.210531/public-domain.LICENSE
+-rw-rw-r--   0 pombreda  (1000) pombreda  (1000)     1414 2021-03-30 11:59:06.000000 typecode_libmagic-system-provided-5.39.210531/bsd-new.LICENSE
+-rw-rw-r--   0 pombreda  (1000) pombreda  (1000)      742 2021-05-31 10:39:29.000000 typecode_libmagic-system-provided-5.39.210531/PKG-INFO
+-rw-rw-r--   0 pombreda  (1000) pombreda  (1000)      644 2021-03-30 11:59:06.000000 typecode_libmagic-system-provided-5.39.210531/gpl-1.0-plus.LICENSE
```

### Comparing `typecode_libmagic-system-provided-5.39.210223/bsd-simplified-darwin.LICENSE` & `typecode_libmagic-system-provided-5.39.210531/bsd-simplified-darwin.LICENSE`

 * *Files identical despite different names*

### Comparing `typecode_libmagic-system-provided-5.39.210223/bsd-simplified.LICENSE` & `typecode_libmagic-system-provided-5.39.210531/bsd-simplified.LICENSE`

 * *Files identical despite different names*

### Comparing `typecode_libmagic-system-provided-5.39.210223/apache-2.0.LICENSE` & `typecode_libmagic-system-provided-5.39.210531/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `typecode_libmagic-system-provided-5.39.210223/libmagic.ABOUT` & `typecode_libmagic-system-provided-5.39.210531/libmagic.ABOUT`

 * *Files identical despite different names*

### Comparing `typecode_libmagic-system-provided-5.39.210223/bsd-original.LICENSE` & `typecode_libmagic-system-provided-5.39.210531/bsd-original.LICENSE`

 * *Files identical despite different names*

### Comparing `typecode_libmagic-system-provided-5.39.210223/src/typecode_libmagic_system_provided.egg-info/SOURCES.txt` & `typecode_libmagic-system-provided-5.39.210531/src/typecode_libmagic_system_provided.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `typecode_libmagic-system-provided-5.39.210223/src/typecode_libmagic_system_provided.egg-info/PKG-INFO` & `typecode_libmagic-system-provided-5.39.210531/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: typecode-libmagic-system-provided
-Version: 5.39.210223
+Name: typecode_libmagic-system-provided
+Version: 5.39.210531
 Summary: A ScanCode path provider plugin to provide a system package provided libmagic binary and database.
 Home-page: https://github.com/nexB/scancode-plugins
 Author: nexB
 Author-email: info@aboutcode.org
 License: apache-2.0 AND bsd-simplified-darwin AND (bsd-simplified AND public-domain AND bsd-new AND isc AND (bsd-new OR gpl-1.0-plus) AND bsd-original)
 Description: A ScanCode path provider plugin to provide a system package provided libmagic binary and database.
 Keywords: open source,typecode,libmagic
```

### Comparing `typecode_libmagic-system-provided-5.39.210223/src/typecode_libmagic/__init__.py` & `typecode_libmagic-system-provided-5.39.210531/src/typecode_libmagic/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,55 +18,61 @@
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
-from os import path
 import platform
+from os import environ
+from os import path
 
 from plugincode.location_provider import LocationProviderPlugin
 
 
 class LibmagicPaths(LocationProviderPlugin):
     def get_locations(self):
         """
         Return a mapping of {location key: location} providing the installation
         locations of the libmagic shared library as installed on various Linux
         distros or on FreeBSD.
         """
+
         system_arch = platform.machine()
         mainstream_system = platform.system().lower()
         if mainstream_system == 'linux':
             distribution = platform.linux_distribution()[0].lower()
             debian_based_distro = ['ubuntu', 'mint', 'debian']
             rpm_based_distro = ['fedora', 'redhat']
 
             if distribution in debian_based_distro:
-                data_dir = '/usr/lib/file'
+                db_dir = '/usr/lib/file'
                 lib_dir = '/usr/lib/'+system_arch+'-linux-gnu'
 
             elif distribution in rpm_based_distro:
-                data_dir = '/usr/share/misc'
+                db_dir = '/usr/share/misc'
                 lib_dir = '/usr/lib64'
 
             else:
                 raise Exception('Unsupported system: {}'.format(distribution))
 
-            lib_dll = path.join(lib_dir, 'libmagic.so');
+            dll_loc = path.join(lib_dir, 'libmagic.so')
 
         elif mainstream_system == 'freebsd':
             if path.isdir('/usr/local/'):
                 lib_dir = '/usr/local'
             else:
                 lib_dir = '/usr'
 
-            lib_dll = path.join(lib_dir, 'lib/libmagic.so')
-            data_dir = path.join(lib_dir,'share/file')
+            dll_loc = path.join(lib_dir, 'lib/libmagic.so')
+            db_dir = path.join(lib_dir,'share/file')
+
+        magicdb_loc = path.join(db_dir, 'magic.mgc')
 
         locations = {
+            # typecode.libmagic.libdir is not used anymore and deprecated
+            # but we are keeping it around for now for backward compatibility
             'typecode.libmagic.libdir': lib_dir,
-            'typecode.libmagic.dll': lib_dll,
-            'typecode.libmagic.db': path.join(data_dir, 'magic.mgc'),
+            'typecode.libmagic.dll': dll_loc,
+            'typecode.libmagic.db': magicdb_loc,
             }
         return locations
```

### Comparing `typecode_libmagic-system-provided-5.39.210223/isc.LICENSE` & `typecode_libmagic-system-provided-5.39.210531/isc.LICENSE`

 * *Files identical despite different names*

### Comparing `typecode_libmagic-system-provided-5.39.210223/libmagic.NOTICE` & `typecode_libmagic-system-provided-5.39.210531/libmagic.NOTICE`

 * *Files identical despite different names*

### Comparing `typecode_libmagic-system-provided-5.39.210223/gpl-1.0.LICENSE` & `typecode_libmagic-system-provided-5.39.210531/gpl-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `typecode_libmagic-system-provided-5.39.210223/setup.py` & `typecode_libmagic-system-provided-5.39.210531/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup
 
 
 desc = '''A ScanCode path provider plugin to provide a system package provided libmagic binary and database.'''
 
 setup(
     name='typecode_libmagic-system-provided',
-    version='5.39.210223',
+    version='5.39.210531',
     license=(
         'apache-2.0 AND bsd-simplified-darwin AND (bsd-simplified AND public-domain AND '
         'bsd-new AND isc AND (bsd-new OR gpl-1.0-plus) AND bsd-original)'
     ),
     description=desc,
     long_description=desc,
     author='nexB',
```

### Comparing `typecode_libmagic-system-provided-5.39.210223/bsd-new.LICENSE` & `typecode_libmagic-system-provided-5.39.210531/bsd-new.LICENSE`

 * *Files identical despite different names*

### Comparing `typecode_libmagic-system-provided-5.39.210223/PKG-INFO` & `typecode_libmagic-system-provided-5.39.210531/src/typecode_libmagic_system_provided.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: typecode_libmagic-system-provided
-Version: 5.39.210223
+Name: typecode-libmagic-system-provided
+Version: 5.39.210531
 Summary: A ScanCode path provider plugin to provide a system package provided libmagic binary and database.
 Home-page: https://github.com/nexB/scancode-plugins
 Author: nexB
 Author-email: info@aboutcode.org
 License: apache-2.0 AND bsd-simplified-darwin AND (bsd-simplified AND public-domain AND bsd-new AND isc AND (bsd-new OR gpl-1.0-plus) AND bsd-original)
 Description: A ScanCode path provider plugin to provide a system package provided libmagic binary and database.
 Keywords: open source,typecode,libmagic
```

### Comparing `typecode_libmagic-system-provided-5.39.210223/gpl-1.0-plus.LICENSE` & `typecode_libmagic-system-provided-5.39.210531/gpl-1.0-plus.LICENSE`

 * *Files identical despite different names*

