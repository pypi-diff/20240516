# Comparing `tmp/gunshotmatch_reports-0.7.0.tar.gz` & `tmp/gunshotmatch_reports-0.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gunshotmatch_reports-0.7.0.tar", last modified: Thu May 16 16:02:06 2024, max compression
+gzip compressed data, was "gunshotmatch_reports-0.7.0b1.tar", last modified: Wed May  8 16:09:05 2024, max compression
```

## Comparing `gunshotmatch_reports-0.7.0.tar` & `gunshotmatch_reports-0.7.0b1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-16 16:02:06.656824 gunshotmatch_reports-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-16 16:02:06.652824 gunshotmatch_reports-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-16 16:02:06.656824 gunshotmatch_reports-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-16 16:02:06.656824 gunshotmatch_reports-0.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-16 16:02:06.652824 gunshotmatch_reports-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-16 16:01:43.728613 gunshotmatch_reports-0.7.0/gunshotmatch_reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-16 16:01:43.728613 gunshotmatch_reports-0.7.0/gunshotmatch_reports/chromatogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-16 16:01:43.728613 gunshotmatch_reports-0.7.0/gunshotmatch_reports/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-05-16 16:01:43.728613 gunshotmatch_reports-0.7.0/gunshotmatch_reports/alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-16 16:01:43.728613 gunshotmatch_reports-0.7.0/gunshotmatch_reports/peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:01:43.728613 gunshotmatch_reports-0.7.0/gunshotmatch_reports/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-08 16:09:05.772384 gunshotmatch_reports-0.7.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-08 16:09:05.776384 gunshotmatch_reports-0.7.0b1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-08 16:09:05.776384 gunshotmatch_reports-0.7.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-08 16:09:05.776384 gunshotmatch_reports-0.7.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-08 16:09:05.776384 gunshotmatch_reports-0.7.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-08 16:08:40.500232 gunshotmatch_reports-0.7.0b1/gunshotmatch_reports/chromatogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-08 16:08:40.500232 gunshotmatch_reports-0.7.0b1/gunshotmatch_reports/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-08 16:08:40.500232 gunshotmatch_reports-0.7.0b1/gunshotmatch_reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:08:40.500232 gunshotmatch_reports-0.7.0b1/gunshotmatch_reports/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-05-08 16:08:40.500232 gunshotmatch_reports-0.7.0b1/gunshotmatch_reports/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-08 16:08:40.500232 gunshotmatch_reports-0.7.0b1/gunshotmatch_reports/peaks.py
```

### Comparing `gunshotmatch_reports-0.7.0/PKG-INFO` & `gunshotmatch_reports-0.7.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.2
 Name: gunshotmatch-reports
-Version: 0.7.0
+Version: 0.7.0b1
 Summary: PDF Report Generation for GunShotMatch.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Home-page: https://github.com/GunShotMatch/gunshotmatch-reports
 Project-URL: Issue Tracker, https://github.com/GunShotMatch/gunshotmatch-reports/issues
 Project-URL: Source Code, https://github.com/GunShotMatch/gunshotmatch-reports
 Project-URL: Documentation, https://gunshotmatch-reports.readthedocs.io/en/latest
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: domdf-python-tools>=3.8.0.post2
 Requires-Dist: libgunshotmatch>=0.5.0
-Requires-Dist: libgunshotmatch-mpl>=0.6.0
+Requires-Dist: libgunshotmatch-mpl>=0.6.0b1
 Requires-Dist: matplotlib>=3.7.2
 Requires-Dist: reportlab>=4.0.9
 Requires-Dist: svglib>=1.5.1
 Description-Content-Type: text/x-rst
 
 
 =====================
@@ -117,15 +117,15 @@
 .. |license| image:: https://img.shields.io/github/license/GunShotMatch/gunshotmatch-reports
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/GunShotMatch/gunshotmatch-reports
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-reports/v0.7.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-reports/v0.7.0b1
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/GunShotMatch/gunshotmatch-reports
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/commit/master
 	:alt: GitHub last commit
```

### Comparing `gunshotmatch_reports-0.7.0/pyproject.toml` & `gunshotmatch_reports-0.7.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "gunshotmatch-reports"
-version = "0.7.0"
+version = "0.7.0b1"
 description = "PDF Report Generation for GunShotMatch."
 readme = "README.rst"
 keywords = []
 dynamic = []
 dependencies = [
     "domdf-python-tools>=3.8.0.post2",
     "libgunshotmatch>=0.5.0",
-    "libgunshotmatch-mpl>=0.6.0",
+    "libgunshotmatch-mpl>=0.6.0b1",
     "matplotlib>=3.7.2",
     "reportlab>=4.0.9",
     "svglib>=1.5.1",
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `gunshotmatch_reports-0.7.0/README.rst` & `gunshotmatch_reports-0.7.0b1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 .. |license| image:: https://img.shields.io/github/license/GunShotMatch/gunshotmatch-reports
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/GunShotMatch/gunshotmatch-reports
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-reports/v0.7.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-reports/v0.7.0b1
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/GunShotMatch/gunshotmatch-reports
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/commit/master
 	:alt: GitHub last commit
```

### Comparing `gunshotmatch_reports-0.7.0/LICENSE` & `gunshotmatch_reports-0.7.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `gunshotmatch_reports-0.7.0/gunshotmatch_reports/__init__.py` & `gunshotmatch_reports-0.7.0b1/gunshotmatch_reports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020-2024 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.7.0"
+__version__: str = "0.7.0b1"
 __email__: str = "dominic@davis-foster.co.uk"
```

### Comparing `gunshotmatch_reports-0.7.0/gunshotmatch_reports/chromatogram.py` & `gunshotmatch_reports-0.7.0b1/gunshotmatch_reports/chromatogram.py`

 * *Files identical despite different names*

### Comparing `gunshotmatch_reports-0.7.0/gunshotmatch_reports/utils.py` & `gunshotmatch_reports-0.7.0b1/gunshotmatch_reports/utils.py`

 * *Files identical despite different names*

### Comparing `gunshotmatch_reports-0.7.0/gunshotmatch_reports/alignment.py` & `gunshotmatch_reports-0.7.0b1/gunshotmatch_reports/alignment.py`

 * *Files identical despite different names*

### Comparing `gunshotmatch_reports-0.7.0/gunshotmatch_reports/peaks.py` & `gunshotmatch_reports-0.7.0b1/gunshotmatch_reports/peaks.py`

 * *Files identical despite different names*

