# Comparing `tmp/sirji-tools-0.0.8.tar.gz` & `tmp/sirji-tools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-tools-0.0.8.tar", last modified: Fri Apr  5 16:01:58 2024, max compression
+gzip compressed data, was "sirji-tools-0.0.9.tar", last modified: Fri Apr  5 16:16:46 2024, max compression
```

## Comparing `sirji-tools-0.0.8.tar` & `sirji-tools-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:01:58.933234 sirji-tools-0.0.8/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3979 2024-04-05 16:01:58.932506 sirji-tools-0.0.8/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3587 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 16:01:58.933497 sirji-tools-0.0.8/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      671 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:01:58.918079 sirji-tools-0.0.8/sirji_tools/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:01:58.926242 sirji-tools-0.0.8/sirji_tools/crawler/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       58 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/crawler/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      926 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/crawler/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      685 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/crawler/crawler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      942 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/crawler/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1106 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/crawler/github_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1268 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/crawler/pdf_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1347 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/crawler/web_page_handler.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:01:58.927555 sirji-tools-0.0.8/sirji_tools/logger/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      242 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/logger/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3847 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/logger/logger.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:01:58.928724 sirji-tools-0.0.8/sirji_tools/search/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       57 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/search/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1776 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/search/search.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:01:58.931676 sirji-tools-0.0.8/sirji_tools.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3979 2024-04-05 16:01:58.000000 sirji-tools-0.0.8/sirji_tools.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      681 2024-04-05 16:01:58.000000 sirji-tools-0.0.8/sirji_tools.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 16:01:58.000000 sirji-tools-0.0.8/sirji_tools.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       70 2024-04-05 16:01:58.000000 sirji-tools-0.0.8/sirji_tools.egg-info/requires.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       12 2024-04-05 16:01:58.000000 sirji-tools-0.0.8/sirji_tools.egg-info/top_level.txt
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:01:58.931014 sirji-tools-0.0.8/tests/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1660 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/tests/test_crawler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2537 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/tests/test_logger.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2139 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/tests/test_pdf_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2022 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/tests/test_search.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:16:46.184535 sirji-tools-0.0.9/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4144 2024-04-05 16:16:46.184106 sirji-tools-0.0.9/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3752 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 16:16:46.184632 sirji-tools-0.0.9/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      671 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:16:46.175122 sirji-tools-0.0.9/sirji_tools/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/sirji_tools/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:16:46.179627 sirji-tools-0.0.9/sirji_tools/crawler/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       58 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/sirji_tools/crawler/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      926 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/sirji_tools/crawler/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      685 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/sirji_tools/crawler/crawler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      942 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/sirji_tools/crawler/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1106 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/sirji_tools/crawler/github_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1268 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/sirji_tools/crawler/pdf_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1347 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/sirji_tools/crawler/web_page_handler.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:16:46.180381 sirji-tools-0.0.9/sirji_tools/logger/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      242 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/sirji_tools/logger/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3847 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/sirji_tools/logger/logger.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:16:46.181452 sirji-tools-0.0.9/sirji_tools/search/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       57 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/sirji_tools/search/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1776 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/sirji_tools/search/search.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:16:46.183605 sirji-tools-0.0.9/sirji_tools.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4144 2024-04-05 16:16:46.000000 sirji-tools-0.0.9/sirji_tools.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      681 2024-04-05 16:16:46.000000 sirji-tools-0.0.9/sirji_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 16:16:46.000000 sirji-tools-0.0.9/sirji_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       70 2024-04-05 16:16:46.000000 sirji-tools-0.0.9/sirji_tools.egg-info/requires.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       12 2024-04-05 16:16:46.000000 sirji-tools-0.0.9/sirji_tools.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:16:46.183183 sirji-tools-0.0.9/tests/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1660 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/tests/test_crawler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2537 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/tests/test_logger.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2139 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/tests/test_pdf_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2022 2024-04-05 16:16:41.000000 sirji-tools-0.0.9/tests/test_search.py
```

### Comparing `sirji-tools-0.0.8/LICENSE` & `sirji-tools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.8/PKG-INFO` & `sirji-tools-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirji-tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Crawler and search tools used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -61,14 +61,20 @@
 
 Install the package from PyPi:
 
 ```zsh
 pip install sirji-tools
 ```
 
+Run the following command to install playwright:
+
+```zsh
+playwright install
+```
+
 ## Usage
 
 ### Environment Variables
 
 Ensure that following environment variables are set:
 
 ```zsh
@@ -118,14 +124,20 @@
 3. Set the environment variables as described above.
 4. Install the package in editable mode by running the following command from repository root:
 
 ```zsh
 pip install -e .
 ```
 
+5. Run the following command to install playwright:
+
+```zsh
+playwright install
+```
+
 ## Running Tests and Coverage Analysis
 
 Follow the above mentioned steps for "contributors", before running the test cases.
 
 ```zsh
 # Install testing dependencies
 pip install pytest coverage
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sirji-tools Version: 0.0.8 Summary: Crawler and
+Metadata-Version: 2.1 Name: sirji-tools Version: 0.0.9 Summary: Crawler and
 search tools used by Sirji. Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji License: MIT Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: requests==2.31.0 Requires-
 Dist: pypdf2==3.0.1 Requires-Dist: markdownify==0.11.6 Requires-Dist:
 playwright==1.42.0
                                  _[_S_i_r_j_i_ _L_o_g_o_]
             SSiirrjjii iiss aann OOppeenn SSoouurrccee AAII SSooffttwwaarree DDeevveellooppmmeenntt AAggeenntt..
@@ -12,16 +12,17 @@
               [GitHub Repo stars][GitHub forks][GitHub watchers]
 ## Sirji Tools `sirji-tools` is a PyPI package that provides tools for: -
 Crawling (downloading web pages to markdown files) - Searching on Google -
 Custom Logging ## Installation ### Setup Virtual Environment We recommend
 setting up a virtual environment to isolate Python dependencies, ensuring
 project-specific packages without conflicting with system-wide installations.
 ```zsh python3 -m venv venv source venv/bin/activate ``` ### Install Package
-Install the package from PyPi: ```zsh pip install sirji-tools ``` ## Usage ###
-Environment Variables Ensure that following environment variables are set:
+Install the package from PyPi: ```zsh pip install sirji-tools ``` Run the
+following command to install playwright: ```zsh playwright install ``` ## Usage
+### Environment Variables Ensure that following environment variables are set:
 ```zsh export SIRJI_WORKSPACE="Absolute folder path for Sirji to use as it's
 workspace. Note that a .sirji folder will be created inside it." export
 SIRJI_RUN_ID='Unique alphanumeric ID for each run. Note that a sub folder named
 by this ID will be created inside of .sirji folder to store logs, etc.' ``` ###
 Crawl URLs Crawl URLs tool will be used to crawl the web pages and extract the
 information from the web pages. And store the information for the further
 processing by researcher. ```python from sirji_tools import crawl_urls urls =
@@ -33,13 +34,14 @@
 ``` ### Logger Logger tool will be used to log the information in the log file.
 It will be used to log the information to show the progress of the execution.
 ```python from sirji_tools.logger import p_logger p_logger.info("Log line
 here") ``` ## For Contributors 1. Fork and clone the repository. 2. Create and
 activate the virtual environment as described above. 3. Set the environment
 variables as described above. 4. Install the package in editable mode by
 running the following command from repository root: ```zsh pip install -e . ```
-## Running Tests and Coverage Analysis Follow the above mentioned steps for
+5. Run the following command to install playwright: ```zsh playwright install
+``` ## Running Tests and Coverage Analysis Follow the above mentioned steps for
 "contributors", before running the test cases. ```zsh # Install testing
 dependencies pip install pytest coverage # Execute tests pytest # Measure
 coverage, excluding test files coverage run --omit="tests/*" -m pytest coverage
 report ``` ## License Distributed under the MIT License. See `LICENSE` for more
 information.
```

### Comparing `sirji-tools-0.0.8/README.md` & `sirji-tools-0.0.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -46,14 +46,20 @@
 
 Install the package from PyPi:
 
 ```zsh
 pip install sirji-tools
 ```
 
+Run the following command to install playwright:
+
+```zsh
+playwright install
+```
+
 ## Usage
 
 ### Environment Variables
 
 Ensure that following environment variables are set:
 
 ```zsh
@@ -103,14 +109,20 @@
 3. Set the environment variables as described above.
 4. Install the package in editable mode by running the following command from repository root:
 
 ```zsh
 pip install -e .
 ```
 
+5. Run the following command to install playwright:
+
+```zsh
+playwright install
+```
+
 ## Running Tests and Coverage Analysis
 
 Follow the above mentioned steps for "contributors", before running the test cases.
 
 ```zsh
 # Install testing dependencies
 pip install pytest coverage
```

#### html2text {}

```diff
@@ -6,16 +6,17 @@
               [GitHub Repo stars][GitHub forks][GitHub watchers]
 ## Sirji Tools `sirji-tools` is a PyPI package that provides tools for: -
 Crawling (downloading web pages to markdown files) - Searching on Google -
 Custom Logging ## Installation ### Setup Virtual Environment We recommend
 setting up a virtual environment to isolate Python dependencies, ensuring
 project-specific packages without conflicting with system-wide installations.
 ```zsh python3 -m venv venv source venv/bin/activate ``` ### Install Package
-Install the package from PyPi: ```zsh pip install sirji-tools ``` ## Usage ###
-Environment Variables Ensure that following environment variables are set:
+Install the package from PyPi: ```zsh pip install sirji-tools ``` Run the
+following command to install playwright: ```zsh playwright install ``` ## Usage
+### Environment Variables Ensure that following environment variables are set:
 ```zsh export SIRJI_WORKSPACE="Absolute folder path for Sirji to use as it's
 workspace. Note that a .sirji folder will be created inside it." export
 SIRJI_RUN_ID='Unique alphanumeric ID for each run. Note that a sub folder named
 by this ID will be created inside of .sirji folder to store logs, etc.' ``` ###
 Crawl URLs Crawl URLs tool will be used to crawl the web pages and extract the
 information from the web pages. And store the information for the further
 processing by researcher. ```python from sirji_tools import crawl_urls urls =
@@ -27,13 +28,14 @@
 ``` ### Logger Logger tool will be used to log the information in the log file.
 It will be used to log the information to show the progress of the execution.
 ```python from sirji_tools.logger import p_logger p_logger.info("Log line
 here") ``` ## For Contributors 1. Fork and clone the repository. 2. Create and
 activate the virtual environment as described above. 3. Set the environment
 variables as described above. 4. Install the package in editable mode by
 running the following command from repository root: ```zsh pip install -e . ```
-## Running Tests and Coverage Analysis Follow the above mentioned steps for
+5. Run the following command to install playwright: ```zsh playwright install
+``` ## Running Tests and Coverage Analysis Follow the above mentioned steps for
 "contributors", before running the test cases. ```zsh # Install testing
 dependencies pip install pytest coverage # Execute tests pytest # Measure
 coverage, excluding test files coverage run --omit="tests/*" -m pytest coverage
 report ``` ## License Distributed under the MIT License. See `LICENSE` for more
 information.
```

### Comparing `sirji-tools-0.0.8/setup.py` & `sirji-tools-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-tools',
-    version='0.0.8',
+    version='0.0.9',
     author='Sirji',
     description='Crawler and search tools used by Sirji.',
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
```

### Comparing `sirji-tools-0.0.8/sirji_tools/crawler/base.py` & `sirji-tools-0.0.9/sirji_tools/crawler/base.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.8/sirji_tools/crawler/crawler.py` & `sirji-tools-0.0.9/sirji_tools/crawler/crawler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.8/sirji_tools/crawler/factory.py` & `sirji-tools-0.0.9/sirji_tools/crawler/factory.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.8/sirji_tools/crawler/github_handler.py` & `sirji-tools-0.0.9/sirji_tools/crawler/github_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.8/sirji_tools/crawler/pdf_handler.py` & `sirji-tools-0.0.9/sirji_tools/crawler/pdf_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.8/sirji_tools/crawler/web_page_handler.py` & `sirji-tools-0.0.9/sirji_tools/crawler/web_page_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.8/sirji_tools/logger/logger.py` & `sirji-tools-0.0.9/sirji_tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.8/sirji_tools/search/search.py` & `sirji-tools-0.0.9/sirji_tools/search/search.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.8/sirji_tools.egg-info/PKG-INFO` & `sirji-tools-0.0.9/sirji_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirji-tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Crawler and search tools used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -61,14 +61,20 @@
 
 Install the package from PyPi:
 
 ```zsh
 pip install sirji-tools
 ```
 
+Run the following command to install playwright:
+
+```zsh
+playwright install
+```
+
 ## Usage
 
 ### Environment Variables
 
 Ensure that following environment variables are set:
 
 ```zsh
@@ -118,14 +124,20 @@
 3. Set the environment variables as described above.
 4. Install the package in editable mode by running the following command from repository root:
 
 ```zsh
 pip install -e .
 ```
 
+5. Run the following command to install playwright:
+
+```zsh
+playwright install
+```
+
 ## Running Tests and Coverage Analysis
 
 Follow the above mentioned steps for "contributors", before running the test cases.
 
 ```zsh
 # Install testing dependencies
 pip install pytest coverage
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sirji-tools Version: 0.0.8 Summary: Crawler and
+Metadata-Version: 2.1 Name: sirji-tools Version: 0.0.9 Summary: Crawler and
 search tools used by Sirji. Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji License: MIT Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: requests==2.31.0 Requires-
 Dist: pypdf2==3.0.1 Requires-Dist: markdownify==0.11.6 Requires-Dist:
 playwright==1.42.0
                                  _[_S_i_r_j_i_ _L_o_g_o_]
             SSiirrjjii iiss aann OOppeenn SSoouurrccee AAII SSooffttwwaarree DDeevveellooppmmeenntt AAggeenntt..
@@ -12,16 +12,17 @@
               [GitHub Repo stars][GitHub forks][GitHub watchers]
 ## Sirji Tools `sirji-tools` is a PyPI package that provides tools for: -
 Crawling (downloading web pages to markdown files) - Searching on Google -
 Custom Logging ## Installation ### Setup Virtual Environment We recommend
 setting up a virtual environment to isolate Python dependencies, ensuring
 project-specific packages without conflicting with system-wide installations.
 ```zsh python3 -m venv venv source venv/bin/activate ``` ### Install Package
-Install the package from PyPi: ```zsh pip install sirji-tools ``` ## Usage ###
-Environment Variables Ensure that following environment variables are set:
+Install the package from PyPi: ```zsh pip install sirji-tools ``` Run the
+following command to install playwright: ```zsh playwright install ``` ## Usage
+### Environment Variables Ensure that following environment variables are set:
 ```zsh export SIRJI_WORKSPACE="Absolute folder path for Sirji to use as it's
 workspace. Note that a .sirji folder will be created inside it." export
 SIRJI_RUN_ID='Unique alphanumeric ID for each run. Note that a sub folder named
 by this ID will be created inside of .sirji folder to store logs, etc.' ``` ###
 Crawl URLs Crawl URLs tool will be used to crawl the web pages and extract the
 information from the web pages. And store the information for the further
 processing by researcher. ```python from sirji_tools import crawl_urls urls =
@@ -33,13 +34,14 @@
 ``` ### Logger Logger tool will be used to log the information in the log file.
 It will be used to log the information to show the progress of the execution.
 ```python from sirji_tools.logger import p_logger p_logger.info("Log line
 here") ``` ## For Contributors 1. Fork and clone the repository. 2. Create and
 activate the virtual environment as described above. 3. Set the environment
 variables as described above. 4. Install the package in editable mode by
 running the following command from repository root: ```zsh pip install -e . ```
-## Running Tests and Coverage Analysis Follow the above mentioned steps for
+5. Run the following command to install playwright: ```zsh playwright install
+``` ## Running Tests and Coverage Analysis Follow the above mentioned steps for
 "contributors", before running the test cases. ```zsh # Install testing
 dependencies pip install pytest coverage # Execute tests pytest # Measure
 coverage, excluding test files coverage run --omit="tests/*" -m pytest coverage
 report ``` ## License Distributed under the MIT License. See `LICENSE` for more
 information.
```

### Comparing `sirji-tools-0.0.8/sirji_tools.egg-info/SOURCES.txt` & `sirji-tools-0.0.9/sirji_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.8/tests/test_crawler.py` & `sirji-tools-0.0.9/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.8/tests/test_logger.py` & `sirji-tools-0.0.9/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.8/tests/test_pdf_handler.py` & `sirji-tools-0.0.9/tests/test_pdf_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.8/tests/test_search.py` & `sirji-tools-0.0.9/tests/test_search.py`

 * *Files identical despite different names*

