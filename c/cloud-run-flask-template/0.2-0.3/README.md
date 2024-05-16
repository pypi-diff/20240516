# Comparing `tmp/cloud_run_flask_template-0.2.tar.gz` & `tmp/cloud_run_flask_template-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_run_flask_template-0.2.tar", last modified: Wed May 15 12:53:58 2024, max compression
+gzip compressed data, was "cloud_run_flask_template-0.3.tar", last modified: Wed May 15 13:01:02 2024, max compression
```

## Comparing `cloud_run_flask_template-0.2.tar` & `cloud_run_flask_template-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:53:58.646081 cloud_run_flask_template-0.2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1069 2024-05-15 12:35:36.000000 cloud_run_flask_template-0.2/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     2508 2024-05-15 12:53:58.646081 cloud_run_flask_template-0.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1959 2024-05-15 12:50:36.000000 cloud_run_flask_template-0.2/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:53:58.642081 cloud_run_flask_template-0.2/cloud_run_flask_template/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:37:37.000000 cloud_run_flask_template-0.2/cloud_run_flask_template/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3884 2024-05-15 12:38:04.000000 cloud_run_flask_template-0.2/cloud_run_flask_template/generator.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:53:58.642081 cloud_run_flask_template-0.2/cloud_run_flask_template.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     2508 2024-05-15 12:53:58.000000 cloud_run_flask_template-0.2/cloud_run_flask_template.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      391 2024-05-15 12:53:58.000000 cloud_run_flask_template-0.2/cloud_run_flask_template.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-15 12:53:58.000000 cloud_run_flask_template-0.2/cloud_run_flask_template.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       97 2024-05-15 12:53:58.000000 cloud_run_flask_template-0.2/cloud_run_flask_template.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       46 2024-05-15 12:53:58.000000 cloud_run_flask_template-0.2/cloud_run_flask_template.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-15 12:53:58.000000 cloud_run_flask_template-0.2/cloud_run_flask_template.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-15 12:53:58.646081 cloud_run_flask_template-0.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1008 2024-05-15 12:53:22.000000 cloud_run_flask_template-0.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 13:01:02.458067 cloud_run_flask_template-0.3/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1069 2024-05-15 12:35:36.000000 cloud_run_flask_template-0.3/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     2386 2024-05-15 13:01:02.458067 cloud_run_flask_template-0.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1836 2024-05-15 12:59:47.000000 cloud_run_flask_template-0.3/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 13:01:02.454067 cloud_run_flask_template-0.3/cloud_run_flask_template/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:37:37.000000 cloud_run_flask_template-0.3/cloud_run_flask_template/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3884 2024-05-15 12:38:04.000000 cloud_run_flask_template-0.3/cloud_run_flask_template/generator.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 13:01:02.454067 cloud_run_flask_template-0.3/cloud_run_flask_template.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     2386 2024-05-15 13:01:02.000000 cloud_run_flask_template-0.3/cloud_run_flask_template.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      391 2024-05-15 13:01:02.000000 cloud_run_flask_template-0.3/cloud_run_flask_template.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-15 13:01:02.000000 cloud_run_flask_template-0.3/cloud_run_flask_template.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       97 2024-05-15 13:01:02.000000 cloud_run_flask_template-0.3/cloud_run_flask_template.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       46 2024-05-15 13:01:02.000000 cloud_run_flask_template-0.3/cloud_run_flask_template.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-15 13:01:02.000000 cloud_run_flask_template-0.3/cloud_run_flask_template.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-15 13:01:02.458067 cloud_run_flask_template-0.3/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1009 2024-05-15 13:00:42.000000 cloud_run_flask_template-0.3/setup.py
```

### Comparing `cloud_run_flask_template-0.2/LICENSE` & `cloud_run_flask_template-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud_run_flask_template-0.2/PKG-INFO` & `cloud_run_flask_template-0.3/cloud_run_flask_template.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
-Name: cloud_run_flask_template
-Version: 0.2
+Name: cloud-run-flask-template
+Version: 0.3
 Summary: A template for Google Cloud Run Flask development
-Home-page: https://github.com/yourusername/cloud_run_flask_template
-Author: Your Name
-Author-email: your.email@example.com
+Home-page: https://github.com/Yash-Kavaiya/gcloudrun-flaskpython
+Author: Yash Kavaiya
+Author-email: yash.kavaiya3@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask==3.0.3
 Requires-Dist: gunicorn==22.0.0
 Requires-Dist: Werkzeug==3.0.3
 
-Sure, here's a README.md template that you can use to provide instructions and information about your package:
 
-```markdown
 # Cloud Run Flask Template
 
 [![PyPI version](https://badge.fury.io/py/cloud-run-flask-template.svg)](https://badge.fury.io/py/cloud-run-flask-template)
 
 A template for quickly setting up a Flask application for Google Cloud Run deployment.
 
 ## Installation
```

### Comparing `cloud_run_flask_template-0.2/README.md` & `cloud_run_flask_template-0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-Sure, here's a README.md template that you can use to provide instructions and information about your package:
 
-```markdown
 # Cloud Run Flask Template
 
 [![PyPI version](https://badge.fury.io/py/cloud-run-flask-template.svg)](https://badge.fury.io/py/cloud-run-flask-template)
 
 A template for quickly setting up a Flask application for Google Cloud Run deployment.
 
 ## Installation
```

### Comparing `cloud_run_flask_template-0.2/cloud_run_flask_template/generator.py` & `cloud_run_flask_template-0.3/cloud_run_flask_template/generator.py`

 * *Files identical despite different names*

### Comparing `cloud_run_flask_template-0.2/cloud_run_flask_template.egg-info/PKG-INFO` & `cloud_run_flask_template-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
-Name: cloud-run-flask-template
-Version: 0.2
+Name: cloud_run_flask_template
+Version: 0.3
 Summary: A template for Google Cloud Run Flask development
-Home-page: https://github.com/yourusername/cloud_run_flask_template
-Author: Your Name
-Author-email: your.email@example.com
+Home-page: https://github.com/Yash-Kavaiya/gcloudrun-flaskpython
+Author: Yash Kavaiya
+Author-email: yash.kavaiya3@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask==3.0.3
 Requires-Dist: gunicorn==22.0.0
 Requires-Dist: Werkzeug==3.0.3
 
-Sure, here's a README.md template that you can use to provide instructions and information about your package:
 
-```markdown
 # Cloud Run Flask Template
 
 [![PyPI version](https://badge.fury.io/py/cloud-run-flask-template.svg)](https://badge.fury.io/py/cloud-run-flask-template)
 
 A template for quickly setting up a Flask application for Google Cloud Run deployment.
 
 ## Installation
```

### Comparing `cloud_run_flask_template-0.2/setup.py` & `cloud_run_flask_template-0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 # Read the contents of your README file
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='cloud_run_flask_template',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'cloud_run_flask_template = cloud_run_flask_template.generator:generate_project'
         ]
     },
     install_requires=[
         'Flask==3.0.3',
         'gunicorn==22.0.0',
         'Werkzeug==3.0.3'
     ],
-    author='Your Name',
-    author_email='your.email@example.com',
+    author='Yash Kavaiya',
+    author_email='yash.kavaiya3@gmail.com',
     description='A template for Google Cloud Run Flask development',
     long_description=long_description,  # Set the long description here
     long_description_content_type='text/markdown',
-    url='https://github.com/yourusername/cloud_run_flask_template',
+    url='https://github.com/Yash-Kavaiya/gcloudrun-flaskpython',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

