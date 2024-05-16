# Comparing `tmp/fguard-1.0.0.tar.gz` & `tmp/fguard-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fguard-1.0.0.tar", last modified: Thu May 16 16:49:45 2024, max compression
+gzip compressed data, was "fguard-1.1.0.tar", last modified: Thu May 16 17:21:04 2024, max compression
```

## Comparing `fguard-1.0.0.tar` & `fguard-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 16:49:45.245358 fguard-1.0.0/
--rw-rw-rw-   0        0        0    35823 2024-05-16 13:10:42.000000 fguard-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2575 2024-05-16 16:49:45.245358 fguard-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2025 2024-05-16 16:39:03.000000 fguard-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 16:49:45.229746 fguard-1.0.0/fguard/
--rw-rw-rw-   0        0        0        0 2024-05-16 13:14:49.000000 fguard-1.0.0/fguard/__init__.py
--rw-rw-rw-   0        0        0    13941 2024-05-16 16:32:23.000000 fguard-1.0.0/fguard/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-16 16:49:45.245358 fguard-1.0.0/fguard.egg-info/
--rw-rw-rw-   0        0        0     2575 2024-05-16 16:49:45.000000 fguard-1.0.0/fguard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-05-16 16:49:45.000000 fguard-1.0.0/fguard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 16:49:45.000000 fguard-1.0.0/fguard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-16 16:49:45.000000 fguard-1.0.0/fguard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      152 2024-05-16 16:49:45.000000 fguard-1.0.0/fguard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 16:49:45.000000 fguard-1.0.0/fguard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      213 2024-05-16 13:56:19.000000 fguard-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 16:49:45.245358 fguard-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1054 2024-05-16 16:49:24.000000 fguard-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:21:04.682975 fguard-1.1.0/
+-rw-rw-rw-   0        0        0    35823 2024-05-16 13:10:42.000000 fguard-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2824 2024-05-16 17:21:04.682975 fguard-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2274 2024-05-16 17:18:39.000000 fguard-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 17:21:04.667354 fguard-1.1.0/fguard/
+-rw-rw-rw-   0        0        0        0 2024-05-16 13:14:49.000000 fguard-1.1.0/fguard/__init__.py
+-rw-rw-rw-   0        0        0    13941 2024-05-16 16:32:23.000000 fguard-1.1.0/fguard/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:21:04.682975 fguard-1.1.0/fguard/core/
+-rw-rw-rw-   0        0        0        0 2024-05-16 17:09:53.000000 fguard-1.1.0/fguard/core/__init__.py
+-rw-rw-rw-   0        0        0     8600 2024-05-15 13:38:39.000000 fguard-1.1.0/fguard/core/communication.py
+-rw-rw-rw-   0        0        0     5082 2024-05-14 21:41:18.000000 fguard-1.1.0/fguard/core/handler.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:21:04.682975 fguard-1.1.0/fguard/core/unet/
+-rw-rw-rw-   0        0        0        0 2024-05-16 17:10:02.000000 fguard-1.1.0/fguard/core/unet/__init__.py
+-rw-rw-rw-   0        0        0     1786 2024-05-16 12:47:52.000000 fguard-1.1.0/fguard/core/unet/unet_model.py
+-rw-rw-rw-   0        0        0     2679 2024-04-25 20:53:17.000000 fguard-1.1.0/fguard/core/unet/unet_parts.py
+-rw-rw-rw-   0        0        0     2713 2024-05-14 21:45:33.000000 fguard-1.1.0/fguard/core/utils.py
+-rw-rw-rw-   0        0        0     5225 2024-05-16 12:40:10.000000 fguard-1.1.0/fguard/core/vision.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:21:04.682975 fguard-1.1.0/fguard.egg-info/
+-rw-rw-rw-   0        0        0     2824 2024-05-16 17:21:04.000000 fguard-1.1.0/fguard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2024-05-16 17:21:04.000000 fguard-1.1.0/fguard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 17:21:04.000000 fguard-1.1.0/fguard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-16 17:21:04.000000 fguard-1.1.0/fguard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      152 2024-05-16 17:21:04.000000 fguard-1.1.0/fguard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 17:21:04.000000 fguard-1.1.0/fguard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      213 2024-05-16 13:56:19.000000 fguard-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 17:21:04.698593 fguard-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1070 2024-05-16 17:20:41.000000 fguard-1.1.0/setup.py
```

### Comparing `fguard-1.0.0/LICENSE` & `fguard-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fguard-1.0.0/PKG-INFO` & `fguard-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: fguard
-Version: 1.0.0
+Version: 1.1.0
 Summary: Detect deforestation on area over a given period of time
 Home-page: https://forestguardian.ru/
 Author: Ivan Gronsky
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Forest Guard CLI
 
-Check out website for **documentation** and more info - **https://forestguardian.ru/**.
+Check our website for **documentation** and more info - **https://forestguardian.ru/**.
 Forest Guard CLI using Click framework.
 
 # About
 
 Our goal is to look for deforestation area and track them in time period on satellite images. For example:
 
 <img src='readme-images/example.png' width='400'>
@@ -37,38 +37,46 @@
 
 We download data from Sentinel Hub (https://www.sentinel-hub.com). We work only with L1C and L2A satellites. You need API token for this.
 
 ## Preparation
 
 Use venv!
 - [ ] Install requirements using this command:
-```
+```bash
 pip install -r requirements/dev.txt
 ```
 - [ ] Wake the `setup.py` up:
-```
+```bash
 pip install .
 ```
 This will give you the opportunity to use `fguard`.
 
 ## Usage
 
 - Add credentials to a programm:
-```
+```bash
 fguard config [вЂ“f вЂњpath/to/config/settings.tomlвЂќ] | [--id вЂњYOUR_IDвЂќ --token вЂњYOUR_TOKENвЂќ]
 ```
 - Request:
-```
+```bash
 fguard request [вЂ“f вЂњpath/to/config/settings.tomlвЂќ] | [-c  c1 c2 c3 c4 -t t1 t2] вЂњoutput/folderвЂќ {-s "size" вЂ“d "detector" --isolate}
 ```
 This will save images in output folder. Also saves json files of all events (new, add, merge).
 - Erase cache, config file, etc:
+```bash
+fguard delete [--cache] | [--config] | [--model]
 ```
-fguard delete [--cache] | [--config]
+- To use `net` detector you need to download model:
+```bash
+fguard net --update
 ```
+It can be also used to update model (we still train it).
+
+
+For more info check our website - **https://forestguardian.ru/**.
 
 ### Example of toml settings file
 
 - `config-settings-example.toml`
 ```toml
 [config]
 id = ""
```

### Comparing `fguard-1.0.0/README.md` & `fguard-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Forest Guard CLI
 
-Check out website for **documentation** and more info - **https://forestguardian.ru/**.
+Check our website for **documentation** and more info - **https://forestguardian.ru/**.
 Forest Guard CLI using Click framework.
 
 # About
 
 Our goal is to look for deforestation area and track them in time period on satellite images. For example:
 
 <img src='readme-images/example.png' width='400'>
@@ -22,38 +22,46 @@
 
 We download data from Sentinel Hub (https://www.sentinel-hub.com). We work only with L1C and L2A satellites. You need API token for this.
 
 ## Preparation
 
 Use venv!
 - [ ] Install requirements using this command:
-```
+```bash
 pip install -r requirements/dev.txt
 ```
 - [ ] Wake the `setup.py` up:
-```
+```bash
 pip install .
 ```
 This will give you the opportunity to use `fguard`.
 
 ## Usage
 
 - Add credentials to a programm:
-```
+```bash
 fguard config [–f “path/to/config/settings.toml”] | [--id “YOUR_ID” --token “YOUR_TOKEN”]
 ```
 - Request:
-```
+```bash
 fguard request [–f “path/to/config/settings.toml”] | [-c  c1 c2 c3 c4 -t t1 t2] “output/folder” {-s "size" –d "detector" --isolate}
 ```
 This will save images in output folder. Also saves json files of all events (new, add, merge).
 - Erase cache, config file, etc:
+```bash
+fguard delete [--cache] | [--config] | [--model]
 ```
-fguard delete [--cache] | [--config]
+- To use `net` detector you need to download model:
+```bash
+fguard net --update
 ```
+It can be also used to update model (we still train it).
+
+
+For more info check our website - **https://forestguardian.ru/**.
 
 ### Example of toml settings file
 
 - `config-settings-example.toml`
 ```toml
 [config]
 id = ""
```

### Comparing `fguard-1.0.0/fguard/cli.py` & `fguard-1.1.0/fguard/cli.py`

 * *Files identical despite different names*

### Comparing `fguard-1.0.0/fguard.egg-info/PKG-INFO` & `fguard-1.1.0/fguard.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: fguard
-Version: 1.0.0
+Version: 1.1.0
 Summary: Detect deforestation on area over a given period of time
 Home-page: https://forestguardian.ru/
 Author: Ivan Gronsky
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Forest Guard CLI
 
-Check out website for **documentation** and more info - **https://forestguardian.ru/**.
+Check our website for **documentation** and more info - **https://forestguardian.ru/**.
 Forest Guard CLI using Click framework.
 
 # About
 
 Our goal is to look for deforestation area and track them in time period on satellite images. For example:
 
 <img src='readme-images/example.png' width='400'>
@@ -37,38 +37,46 @@
 
 We download data from Sentinel Hub (https://www.sentinel-hub.com). We work only with L1C and L2A satellites. You need API token for this.
 
 ## Preparation
 
 Use venv!
 - [ ] Install requirements using this command:
-```
+```bash
 pip install -r requirements/dev.txt
 ```
 - [ ] Wake the `setup.py` up:
-```
+```bash
 pip install .
 ```
 This will give you the opportunity to use `fguard`.
 
 ## Usage
 
 - Add credentials to a programm:
-```
+```bash
 fguard config [вЂ“f вЂњpath/to/config/settings.tomlвЂќ] | [--id вЂњYOUR_IDвЂќ --token вЂњYOUR_TOKENвЂќ]
 ```
 - Request:
-```
+```bash
 fguard request [вЂ“f вЂњpath/to/config/settings.tomlвЂќ] | [-c  c1 c2 c3 c4 -t t1 t2] вЂњoutput/folderвЂќ {-s "size" вЂ“d "detector" --isolate}
 ```
 This will save images in output folder. Also saves json files of all events (new, add, merge).
 - Erase cache, config file, etc:
+```bash
+fguard delete [--cache] | [--config] | [--model]
 ```
-fguard delete [--cache] | [--config]
+- To use `net` detector you need to download model:
+```bash
+fguard net --update
 ```
+It can be also used to update model (we still train it).
+
+
+For more info check our website - **https://forestguardian.ru/**.
 
 ### Example of toml settings file
 
 - `config-settings-example.toml`
 ```toml
 [config]
 id = ""
```

### Comparing `fguard-1.0.0/setup.py` & `fguard-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import setuptools
 
 setuptools.setup(
     name="fguard",
-    version="1.0.0",
+    version="1.1.0",
     url="https://forestguardian.ru/",
     author="Ivan Gronsky",
     description="Detect deforestation on area over a given period of time",
     long_description=open("README.MD").read(),
     long_description_content_type='text/markdown',
     license="GPL-3.0",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.3',
-    packages=["fguard"],
+    packages=setuptools.find_packages(),
     install_requires=[
         "click==8.1.7",
         "eo-learn==1.5.2",
         "joblib==1.3.2",
         "numpy==1.26.3",
         "opencv-python==4.8.1.78",
         "platformdirs==4.2.1",
```

