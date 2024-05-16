# Comparing `tmp/sarcharts-0.2.0.tar.gz` & `tmp/sarcharts-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarcharts-0.2.0.tar", last modified: Tue May 14 15:54:05 2024, max compression
+gzip compressed data, was "sarcharts-0.2.1.tar", last modified: Wed May 15 13:14:57 2024, max compression
```

## Comparing `sarcharts-0.2.0.tar` & `sarcharts-0.2.1.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.928699 sarcharts-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.920699 sarcharts-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.924699 sarcharts-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-14 15:54:00.000000 sarcharts-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-14 15:54:00.000000 sarcharts-0.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 15:54:05.000000 sarcharts-0.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 15:54:05.000000 sarcharts-0.2.0/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 15:54:00.000000 sarcharts-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-14 15:54:05.928699 sarcharts-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-14 15:54:00.000000 sarcharts-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.924699 sarcharts-0.2.0/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-14 15:54:00.000000 sarcharts-0.2.0/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   137178 2024-05-14 15:54:00.000000 sarcharts-0.2.0/doc/sarcharts.png
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-14 15:54:00.000000 sarcharts-0.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.924699 sarcharts-0.2.0/sarcharts/
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.928699 sarcharts-0.2.0/sarcharts/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/bin/sarcharts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.920699 sarcharts-0.2.0/sarcharts/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.928699 sarcharts-0.2.0/sarcharts/html/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/html/css/sarcharts.css
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/html/css/ul-select.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.928699 sarcharts-0.2.0/sarcharts/html/img/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/html/img/chevron.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.928699 sarcharts-0.2.0/sarcharts/html/js/
--rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/html/js/chart.umd.js
--rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/html/js/chartjs-plugin-zoom.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/html/js/hammer.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/html/js/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/html/js/ul-select.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.928699 sarcharts-0.2.0/sarcharts/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/lib/chartjs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/lib/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/lib/sadf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/lib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.928699 sarcharts-0.2.0/sarcharts/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/templates/chart.html
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.928699 sarcharts-0.2.0/sarcharts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-14 15:54:05.000000 sarcharts-0.2.0/sarcharts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-14 15:54:05.000000 sarcharts-0.2.0/sarcharts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:54:05.000000 sarcharts-0.2.0/sarcharts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 15:54:05.000000 sarcharts-0.2.0/sarcharts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:54:05.000000 sarcharts-0.2.0/sarcharts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 15:54:05.000000 sarcharts-0.2.0/sarcharts.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 15:54:05.000000 sarcharts-0.2.0/sarcharts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 15:54:05.000000 sarcharts-0.2.0/sarcharts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 15:54:05.928699 sarcharts-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-14 15:54:00.000000 sarcharts-0.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-14 15:54:00.000000 sarcharts-0.2.0/test-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-14 15:54:00.000000 sarcharts-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:14:57.451750 sarcharts-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:14:57.439750 sarcharts-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:14:57.443750 sarcharts-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-15 13:14:52.000000 sarcharts-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-15 13:14:52.000000 sarcharts-0.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 13:14:57.000000 sarcharts-0.2.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 13:14:57.000000 sarcharts-0.2.1/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 13:14:52.000000 sarcharts-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-15 13:14:57.451750 sarcharts-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-15 13:14:52.000000 sarcharts-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:14:57.443750 sarcharts-0.2.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-15 13:14:52.000000 sarcharts-0.2.1/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   109472 2024-05-15 13:14:52.000000 sarcharts-0.2.1/doc/sarcharts.png
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-15 13:14:52.000000 sarcharts-0.2.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:14:57.443750 sarcharts-0.2.1/sarcharts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:14:57.447750 sarcharts-0.2.1/sarcharts/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/bin/sarcharts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:14:57.443750 sarcharts-0.2.1/sarcharts/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:14:57.447750 sarcharts-0.2.1/sarcharts/html/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/html/css/sarcharts.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/html/css/ul-select.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:14:57.447750 sarcharts-0.2.1/sarcharts/html/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/html/img/chevron.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:14:57.447750 sarcharts-0.2.1/sarcharts/html/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/html/js/chart.umd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34500 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/html/js/chartjs-plugin-annotation.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/html/js/chartjs-plugin-zoom.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/html/js/hammer.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/html/js/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/html/js/ul-select.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:14:57.447750 sarcharts-0.2.1/sarcharts/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/lib/chartjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/lib/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/lib/sadf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/lib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:14:57.447750 sarcharts-0.2.1/sarcharts/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/templates/chart.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-15 13:14:52.000000 sarcharts-0.2.1/sarcharts/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:14:57.447750 sarcharts-0.2.1/sarcharts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-15 13:14:57.000000 sarcharts-0.2.1/sarcharts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-15 13:14:57.000000 sarcharts-0.2.1/sarcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:14:57.000000 sarcharts-0.2.1/sarcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 13:14:57.000000 sarcharts-0.2.1/sarcharts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:14:57.000000 sarcharts-0.2.1/sarcharts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 13:14:57.000000 sarcharts-0.2.1/sarcharts.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 13:14:57.000000 sarcharts-0.2.1/sarcharts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 13:14:57.000000 sarcharts-0.2.1/sarcharts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-15 13:14:57.451750 sarcharts-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-15 13:14:52.000000 sarcharts-0.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-15 13:14:52.000000 sarcharts-0.2.1/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-15 13:14:52.000000 sarcharts-0.2.1/tox.ini
```

### Comparing `sarcharts-0.2.0/.github/workflows/python-publish.yml` & `sarcharts-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.0/.pylintrc` & `sarcharts-0.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.0/LICENSE` & `sarcharts-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.0/PKG-INFO` & `sarcharts-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.2.0
+Version: 0.2.1
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `sarcharts-0.2.0/README.md` & `sarcharts-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.0/doc/README.md` & `sarcharts-0.2.1/doc/README.md`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.0/sarcharts/__init__.py` & `sarcharts-0.2.1/sarcharts/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,18 +100,20 @@
             # shutil.rmtree(self.args.outputpath)
         os.makedirs(self.args.outputpath + "/sar")
         shutil.copytree(os.path.dirname(
                         os.path.realpath(__file__)) + "/html",
                         self.args.outputpath + "/html")
 
     def main(self):
-        # import ipdb; ipdb.set_trace()
         if len(self.args.sarfilespaths) > 0:
             sarfiles = util.get_filelist(self.args.sarfilespaths)
-            util.debug(self.args, 'D', "sarfiles: " + str(sarfiles))
-            charts = Sadf().sar_to_chartjs(self.args, sarfiles)
-            ChartJS().write_files(self.args, charts)
-            util.debug(self.args, '', "Open SarCharts in default browser.")
-            webbrowser.open(self.args.outputpath, 0, True)
-        else:
-            self.parser.print_help()
-            util.debug(self.args, 'E', "No valid `sa` files on provided path.")
+            if len(sarfiles) > 0:
+                util.debug(self.args, 'D', "sarfiles: " + str(sarfiles))
+                charts = Sadf().sar_to_chartjs(self.args, sarfiles)
+                ChartJS().write_files(self.args, charts)
+                util.debug(self.args, '', "Open SarCharts in default browser.")
+                webbrowser.open(self.args.outputpath, 0, True)
+            else:
+                self.parser.print_help()
+                util.debug(
+                    self.args, 'E',
+                    f"No valid `sa??` files in `{self.args.sarfilespaths}`.")
```

### Comparing `sarcharts-0.2.0/sarcharts/html/css/sarcharts.css` & `sarcharts-0.2.1/sarcharts/html/css/sarcharts.css`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.0/sarcharts/html/css/ul-select.css` & `sarcharts-0.2.1/sarcharts/html/css/ul-select.css`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.0/sarcharts/html/js/chart.umd.js` & `sarcharts-0.2.1/sarcharts/html/js/chart.umd.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.0/sarcharts/html/js/chartjs-plugin-zoom.min.js` & `sarcharts-0.2.1/sarcharts/html/js/chartjs-plugin-zoom.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.0/sarcharts/html/js/hammer.min.js` & `sarcharts-0.2.1/sarcharts/html/js/hammer.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.0/sarcharts/html/js/jquery.js` & `sarcharts-0.2.1/sarcharts/html/js/jquery.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.0/sarcharts/html/js/ul-select.js` & `sarcharts-0.2.1/sarcharts/html/js/ul-select.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.0/sarcharts/lib/chartjs.py` & `sarcharts-0.2.1/sarcharts/lib/chartjs.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
                     "xlabels": sorted(nodecharts['xlabels']),
                     "sysname": nodecharts['sysname'],
                     "release": nodecharts['release'],
                     "machine": nodecharts['machine'],
                     "numberofcpus": nodecharts['number-of-cpus'],
                     "timezone": nodecharts['timezone'],
                     "details": csvdata,
+                    "restarts": nodecharts['restarts'],
                     "pages": sorted(nodecharts['activities'].keys()),
                     "colors": self.colors,
                     "hostname": nodename,
                     "hostnames": charts.keys()
                     }
                 parent = (
                     os.path.dirname(
```

### Comparing `sarcharts-0.2.0/sarcharts/lib/progressbar.py` & `sarcharts-0.2.1/sarcharts/lib/progressbar.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.0/sarcharts/lib/sadf.py` & `sarcharts-0.2.1/sarcharts/lib/sadf.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,23 @@
                     charts[nodename] = {
                         "sysname": hdata['sysname'],
                         "release": hdata['release'],
                         "machine": hdata['machine'],
                         "number-of-cpus": hdata['number-of-cpus'],
                         "timezone": hdata['timezone'],
                         "xlabels": [],
-                        "activities": {}
+                        "activities": {},
+                        "restarts": []
                         }
+                for istats in range(len(hdata['restarts'])):
+                    for r in hdata['restarts'][istats].values():
+                        date = f"{r['date']} {r['time']}"
+                        if util.in_date_range(args, date):
+                            charts[nodename]['restarts'].append(date)
+                            charts[nodename]['xlabels'].append(date)
                 for istats in range(len(hdata['statistics'])):
                     for act, adata in hdata['statistics'][istats].items():
                         pbi += 1
                         pb.print_bar(pbi, f"data {act}.")
                         if act == "timestamp":
                             date = f"{adata['date']} {adata['time']}"
                             if (date not in charts[nodename]['xlabels']
@@ -176,13 +183,13 @@
                         if item not in charts[nodename]['activities'][activity]['datasets'].keys():
                             charts[nodename]['activities'][activity]['datasets'][item] = []
                             for h in headers:
                                 charts[nodename]['activities'][activity]['datasets'][item].append({
                                     "label": h,
                                     "values": []
                                     })
-                        for i in range(len(fields[datastart:])):
-                            charts[nodename]['activities'][activity]['datasets'][item][i]['values'].append({
+                        for f in range(len(fields[datastart:])):
+                            charts[nodename]['activities'][activity]['datasets'][item][f]['values'].append({
                                     'x': fields[2],
-                                    'y': fields[i+datastart]
+                                    'y': fields[f+datastart]
                                     })
         return charts
```

### Comparing `sarcharts-0.2.0/sarcharts/lib/util.py` & `sarcharts-0.2.1/sarcharts/lib/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import fnmatch
 from pathlib import Path
 import subprocess
 
 
 def debug(args, sev, msg):
+    if args.quiet:
+        return
     C = {
         'I': '\033[0;34m',
         'D': '\033[01;36m',
         '': '\033[0;32m',
         'W': '\033[93m',
         'E': '\033[0;31m',
         'RESET': '\033[0m'
```

### Comparing `sarcharts-0.2.0/sarcharts/templates/chart.html` & `sarcharts-0.2.1/sarcharts/templates/chart.html`

 * *Files 15% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>sarcharts {{ hostname }}</title>
     <link rel="stylesheet" href="html/css/sarcharts.css" />
     <link rel="stylesheet" href="html/css/ul-select.css" />
     <script src="html/js/jquery.js"></script>
-    <script src="html/js/chart.umd.js"></script>
     <script src="html/js/hammer.min.js"></script>
-    <script src="html/js/chartjs-plugin-zoom.min.js"></script>
     <script src="html/js/ul-select.js"></script>
+    <script src="html/js/chart.umd.js"></script>
+    <script src="html/js/chartjs-plugin-zoom.min.js"></script>
+    <script src="html/js/chartjs-plugin-annotation.min.js"></script>
 
 </head>
 <body>
 <section class="container">
   {% include "header.html" %}
   <div class="activities">
     <ul>
@@ -32,14 +33,37 @@
 <script>
 $('.i_inactive').click(function() {
   $(".i_active").attr("class","i_inactive");
   $(this).attr("class","i_active");
   showChart($(this).text());
 });
 
+
+{% for i in range(restarts|length) %}
+const restart{{ i }} = {
+  type: 'line',
+  borderColor: 'rgba(255, 0, 0, 0.4)',
+  borderWidth: 1,
+  display: (ctx) => ctx.chart.isDatasetVisible(1),
+  label: {
+    display: true,
+    content: 'restart',
+    position: 'start',
+    backgroundColor: 'transparent',
+    opacity: 0,
+    rotation: 90,
+    xAdjust: 5,
+    font: { size: 10 },
+    color: 'rgba(255, 0, 0, 0.4)'
+  },
+  scaleID: 'x',
+  value: '{{ restarts[i] }}'
+};
+{% endfor %}
+
 function showChart(name) {
   myChart.destroy();
   myChart = new Chart(ctx, {
     type: 'line',
       data: {
         labels: myCharts[name]['labels'],
         datasets: myCharts[name]['datasets']
@@ -47,14 +71,21 @@
     options: {
       maintainAspectRatio: false,
       responsive: true,
       plugins: {
         legend: {
           position: 'top'
         },
+        annotation: {
+          annotations: {
+            {% for i in range(restarts|length) %}
+              restart{{ i }}{{ ", " if not loop.last else "" }}
+            {% endfor %}
+          }
+        },
         zoom: {
           zoom: {
             drag: {
               enabled: true
             },
             wheel: {
               enabled: true,
@@ -95,15 +126,15 @@
 $(document).ready(function () {
   showChart($('.i_inactive').first().text());
   $('.i_inactive').first().attr("class", "i_active");
 
   selhost="{{ hostname }}"
   $('#hostlist').ulSelect(function(elem) {
       selhost=$(elem).text()
-      window.location = selhost+"_cpu-load.html"
+      window.location = selhost+"_{{ pages[0] }}.html"
   });
   selchart="{{ chart }}"
   $('#chartlist').ulSelect(function(elem) {
       selchart=$(elem).text()
       window.location = selhost+"_"+selchart+".html"
   });
```

### Comparing `sarcharts-0.2.0/sarcharts/templates/header.html` & `sarcharts-0.2.1/sarcharts/templates/header.html`

 * *Files 26% similar despite different names*

```diff
@@ -22,10 +22,15 @@
     </div>
     <div class="info">
         <ul>
             <li><b>release:</b> {{ release }}</li>
             <li><b>machine:</b> {{ machine}}</li>
             <li><b>cpunumber:</b> {{ numberofcpus }}</li>
             <li><b>starttime:</b> {{ xlabels[0] }} {{ timezone }}</li>
-            <li><b>endtime:</b> {{ xlabels[-1] }} {{ timezone }}</li></h3>
+            <li><b>endtime:</b> {{ xlabels[-1] }} {{ timezone }}</li>
+        </ul><!--
+        {% for r in restarts %}
+            <br> {{r}}
+        {% endfor %}
+        -->
     </div>
```

### Comparing `sarcharts-0.2.0/sarcharts.egg-info/PKG-INFO` & `sarcharts-0.2.1/sarcharts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.2.0
+Version: 0.2.1
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `sarcharts-0.2.0/sarcharts.egg-info/SOURCES.txt` & `sarcharts-0.2.1/sarcharts.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 sarcharts.egg-info/top_level.txt
 sarcharts/bin/__init__.py
 sarcharts/bin/sarcharts.py
 sarcharts/html/css/sarcharts.css
 sarcharts/html/css/ul-select.css
 sarcharts/html/img/chevron.svg
 sarcharts/html/js/chart.umd.js
+sarcharts/html/js/chartjs-plugin-annotation.min.js
 sarcharts/html/js/chartjs-plugin-zoom.min.js
 sarcharts/html/js/hammer.min.js
 sarcharts/html/js/jquery.js
 sarcharts/html/js/ul-select.js
 sarcharts/lib/chartjs.py
 sarcharts/lib/progressbar.py
 sarcharts/lib/sadf.py
```

### Comparing `sarcharts-0.2.0/setup.cfg` & `sarcharts-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.0/setup.py` & `sarcharts-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.0/tox.ini` & `sarcharts-0.2.1/tox.ini`

 * *Files identical despite different names*

