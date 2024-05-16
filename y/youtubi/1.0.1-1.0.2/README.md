# Comparing `tmp/youtubi-1.0.1.tar.gz` & `tmp/youtubi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtubi-1.0.1.tar", last modified: Wed Mar 27 09:40:51 2024, max compression
+gzip compressed data, was "youtubi-1.0.2.tar", last modified: Thu May 16 15:53:43 2024, max compression
```

## Comparing `youtubi-1.0.1.tar` & `youtubi-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 09:40:51.204649 youtubi-1.0.1/
--rw-r--r--   0 root         (0) root         (0)     1046 2024-03-27 09:40:51.203649 youtubi-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      629 2024-03-27 09:40:41.000000 youtubi-1.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-27 09:40:51.204649 youtubi-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2600 2024-03-27 09:40:41.000000 youtubi-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 09:40:51.201648 youtubi-1.0.1/youtubi/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-03-27 09:40:41.000000 youtubi-1.0.1/youtubi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 09:40:51.203649 youtubi-1.0.1/youtubi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1046 2024-03-27 09:40:51.000000 youtubi-1.0.1/youtubi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2024-03-27 09:40:51.000000 youtubi-1.0.1/youtubi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 09:40:51.000000 youtubi-1.0.1/youtubi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-03-27 09:40:51.000000 youtubi-1.0.1/youtubi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-27 09:40:51.000000 youtubi-1.0.1/youtubi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:53:43.288905 youtubi-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1444 2024-05-16 15:53:43.287905 youtubi-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-16 15:53:33.000000 youtubi-1.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 15:53:43.288905 youtubi-1.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2024-05-16 15:53:33.000000 youtubi-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:53:43.286905 youtubi-1.0.2/youtubi/
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-16 15:53:33.000000 youtubi-1.0.2/youtubi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:53:43.287905 youtubi-1.0.2/youtubi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1444 2024-05-16 15:53:43.000000 youtubi-1.0.2/youtubi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2024-05-16 15:53:43.000000 youtubi-1.0.2/youtubi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 15:53:43.000000 youtubi-1.0.2/youtubi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-05-16 15:53:43.000000 youtubi-1.0.2/youtubi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-16 15:53:43.000000 youtubi-1.0.2/youtubi.egg-info/top_level.txt
```

### Comparing `youtubi-1.0.1/PKG-INFO` & `youtubi-1.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: youtubi
-Version: 1.0.1
-Summary: Python Package made by Mhadhbi Issam . 
+Version: 1.0.2
+Summary: Download youtube videos 
 Home-page: https://gitlab.com/isampypi/youtubi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: pytube
+Requires-Dist: lxml
+Requires-Dist: beautifulsoup4
 
 # youtubi
 
+Download youtube videos python library .
 
 # Install  : 
 ```bash
 pip install youtubi
 ```
 
 ## Example : 
+### Download list of videos urls 
 ```python 
 
 from youtubi import process 
 
 urls= """
 https://youtu.be/oaxWxSdytTk?si=DNJOpBMtJyrmaMQR
 https://youtu.be/Ljmv9joEXiM?si=I55FFgGCgsZ3Km8w
@@ -34,7 +38,20 @@
 https://youtu.be/hM1Bk4cEFmg?si=WQlRpNPg6b-67Agd
 https://youtu.be/DPGR_LyDKNE?si=8Yaeww2zxaQ3xSv3
 https://youtu.be/D5hU4ICEB3o?si=HHTbWCo6knD6n5Xp
 """
 process(urls)
 # process(text, output_path = "./videos")
 ```
+### Download list of videos of channel 
+copy outter html of page where plylist is shown in the page , then 
+```python 
+
+process(urls)
+from youtubi import process , get_channel
+
+html_text = "....."
+urls = get_channel(html_text)
+process(urls)
+# process(text, output_path = "./videos")
+```
+
```

### Comparing `youtubi-1.0.1/setup.py` & `youtubi-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             packages=find_packages(),
             author= author  ,
             author_email=author_email   ,
             description= description,
             long_description=open("README.md").read(),
             long_description_content_type="text/markdown",
             url= url    ,
-            install_requires=["pytube"]  ,
+            install_requires=["pytube","lxml", "beautifulsoup4"]  ,
             classifiers=[
                 'Programming Language :: Python :: 3',
                 'License :: OSI Approved :: MIT License',
                 'Operating System :: OS Independent',
             ],
         )
     def get_versions(self) :
```

### Comparing `youtubi-1.0.1/youtubi.egg-info/PKG-INFO` & `youtubi-1.0.2/youtubi.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: youtubi
-Version: 1.0.1
-Summary: Python Package made by Mhadhbi Issam . 
+Version: 1.0.2
+Summary: Download youtube videos 
 Home-page: https://gitlab.com/isampypi/youtubi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: pytube
+Requires-Dist: lxml
+Requires-Dist: beautifulsoup4
 
 # youtubi
 
+Download youtube videos python library .
 
 # Install  : 
 ```bash
 pip install youtubi
 ```
 
 ## Example : 
+### Download list of videos urls 
 ```python 
 
 from youtubi import process 
 
 urls= """
 https://youtu.be/oaxWxSdytTk?si=DNJOpBMtJyrmaMQR
 https://youtu.be/Ljmv9joEXiM?si=I55FFgGCgsZ3Km8w
@@ -34,7 +38,20 @@
 https://youtu.be/hM1Bk4cEFmg?si=WQlRpNPg6b-67Agd
 https://youtu.be/DPGR_LyDKNE?si=8Yaeww2zxaQ3xSv3
 https://youtu.be/D5hU4ICEB3o?si=HHTbWCo6knD6n5Xp
 """
 process(urls)
 # process(text, output_path = "./videos")
 ```
+### Download list of videos of channel 
+copy outter html of page where plylist is shown in the page , then 
+```python 
+
+process(urls)
+from youtubi import process , get_channel
+
+html_text = "....."
+urls = get_channel(html_text)
+process(urls)
+# process(text, output_path = "./videos")
+```
+
```

