# Comparing `tmp/lavague_drivers_selenium-0.1.1.tar.gz` & `tmp/lavague_drivers_selenium-0.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_drivers_selenium-0.1.1.tar", max compression
+gzip compressed data, was "lavague_drivers_selenium-0.1.1.post1.tar", max compression
```

## Comparing `lavague_drivers_selenium-0.1.1.tar` & `lavague_drivers_selenium-0.1.1.post1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       34 2024-05-15 19:17:05.222186 lavague_drivers_selenium-0.1.1/README.md
--rw-r--r--   0        0        0       57 2024-05-15 19:17:05.222186 lavague_drivers_selenium-0.1.1/lavague/drivers/selenium/__init__.py
--rw-r--r--   0        0        0    12962 2024-05-15 19:17:05.222186 lavague_drivers_selenium-0.1.1/lavague/drivers/selenium/base.py
--rw-r--r--   0        0        0      976 2024-05-15 21:18:31.036236 lavague_drivers_selenium-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 lavague_drivers_selenium-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       34 2024-05-15 22:13:36.166566 lavague_drivers_selenium-0.1.1.post1/README.md
+-rw-r--r--   0        0        0       57 2024-05-15 22:13:36.166566 lavague_drivers_selenium-0.1.1.post1/lavague/drivers/selenium/__init__.py
+-rw-r--r--   0        0        0    11746 2024-05-15 22:13:36.166566 lavague_drivers_selenium-0.1.1.post1/lavague/drivers/selenium/base.py
+-rw-r--r--   0        0        0      982 2024-05-15 22:13:36.170566 lavague_drivers_selenium-0.1.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 lavague_drivers_selenium-0.1.1.post1/PKG-INFO
```

### Comparing `lavague_drivers_selenium-0.1.1/lavague/drivers/selenium/base.py` & `lavague_drivers_selenium-0.1.1.post1/lavague/drivers/selenium/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,49 +19,26 @@
         get_selenium_driver: Optional[Callable[[], WebDriver]] = None,
     ):
         super().__init__(url, get_selenium_driver)
 
     def default_init_code(self) -> Any:
         # these imports are necessary as they will be pasted to the output
         from selenium import webdriver
-        from selenium.webdriver.chrome.service import Service
         from selenium.webdriver.common.by import By
         from selenium.webdriver.chrome.options import Options
         from selenium.webdriver.common.keys import Keys
         from selenium.webdriver.common.action_chains import ActionChains
-        import os.path
 
         chrome_options = Options()
-        chrome_options.add_argument("--headless")  # Ensure GUI is off
+        chrome_options.add_argument("--headless")
         chrome_options.add_argument("--no-sandbox")
-        chrome_options.add_argument("--window-size=1600,900")
 
-        homedir = os.path.expanduser("~")
-
-        # Paths to the chromedriver files
-        path_linux = f"{homedir}/chromedriver-linux64/chromedriver"
-        path_testing = f"{homedir}/chromedriver-testing/chromedriver"
-        path_mac = (
-            "Google Chrome for Testing.app/Contents/MacOS/Google Chrome for Testing"
-        )
-
-        # To avoid breaking change kept legacy linux64 path
-        if os.path.exists(path_linux):
-            chrome_options.binary_location = f"{homedir}/chrome-linux64/chrome"
-            webdriver_service = Service(f"{homedir}/chromedriver-linux64/chromedriver")
-        elif os.path.exists(path_testing):
-            if os.path.exists(f"{homedir}/chrome-testing/{path_mac}"):
-                chrome_options.binary_location = f"{homedir}/chrome-testing/{path_mac}"
-            # Can add support here for other chrome binaries with else if statements
-            webdriver_service = Service(f"{homedir}/chromedriver-testing/chromedriver")
-        else:
-            raise FileNotFoundError("Neither chromedriver file exists.")
-
-        driver = webdriver.Chrome(service=webdriver_service, options=chrome_options)
-        return driver
+        self.driver = webdriver.Chrome(options=chrome_options)
+        self.resize_driver(1024, 1024)
+        return self.driver
 
     def get_driver(self) -> WebDriver:
         return self.driver
 
     def resize_driver(self, width, height) -> None:
         # Selenium is only being able to set window size and not viewport size
         self.driver.set_window_size(width, height)
```

### Comparing `lavague_drivers_selenium-0.1.1/pyproject.toml` & `lavague_drivers_selenium-0.1.1.post1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-drivers-selenium"
-version = "0.1.1"
+version = "0.1.1-post1"
 description = "Selenium integration for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_drivers_selenium-0.1.1/PKG-INFO` & `lavague_drivers_selenium-0.1.1.post1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-drivers-selenium
-Version: 0.1.1
+Version: 0.1.1.post1
 Summary: Selenium integration for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,selenium
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

