# Comparing `tmp/qrawl-0.2.0.tar.gz` & `tmp/qrawl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrawl-0.2.0.tar", max compression
+gzip compressed data, was "qrawl-0.2.1.tar", max compression
```

## Comparing `qrawl-0.2.0.tar` & `qrawl-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11558 2024-04-10 20:13:30.588327 qrawl-0.2.0/LICENSE
--rw-r--r--   0        0        0      794 2024-05-15 23:43:12.405635 qrawl-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-09 08:01:21.111154 qrawl-0.2.0/qrawl/__init__.py
--rw-r--r--   0        0        0     1267 2024-04-09 07:59:51.136473 qrawl-0.2.0/qrawl/common.py
--rw-r--r--   0        0        0      322 2024-05-01 06:43:35.164934 qrawl-0.2.0/qrawl/exceptions.py
--rw-r--r--   0        0        0       28 2024-04-05 07:23:15.121016 qrawl-0.2.0/qrawl/google_sheets/__init__.py
--rw-r--r--   0        0        0     2224 2024-04-10 20:17:48.321751 qrawl-0.2.0/qrawl/google_sheets/column.py
--rw-r--r--   0        0        0       56 2024-04-09 23:05:42.684682 qrawl-0.2.0/qrawl/playwright/async_api/__init__.py
--rw-r--r--   0        0        0     4002 2024-04-10 20:18:37.778395 qrawl-0.2.0/qrawl/playwright/async_api/async_playwright.py
--rw-r--r--   0        0        0      663 2024-04-05 06:47:08.312708 qrawl-0.2.0/qrawl/playwright/async_api/common.py
--rw-r--r--   0        0        0       55 2024-04-09 23:05:16.406743 qrawl-0.2.0/qrawl/playwright/sync_api/__init__.py
--rw-r--r--   0        0        0      587 2024-04-09 23:01:33.394056 qrawl-0.2.0/qrawl/playwright/sync_api/common.py
--rw-r--r--   0        0        0     3933 2024-04-11 06:02:26.308965 qrawl-0.2.0/qrawl/playwright/sync_api/sync_playwright.py
--rw-r--r--   0        0        0        0 2024-04-03 00:46:13.447864 qrawl-0.2.0/qrawl/scrapy/__init__.py
--rw-r--r--   0        0        0       33 2024-04-10 20:18:05.787009 qrawl-0.2.0/qrawl/selenium/__init__.py
--rw-r--r--   0        0        0     7026 2024-05-05 01:32:19.143557 qrawl-0.2.0/qrawl/selenium/browsermob_proxy_wrapper.py
--rw-r--r--   0        0        0     2034 2024-05-01 20:20:39.665636 qrawl-0.2.0/qrawl/selenium/exceptions.py
--rw-r--r--   0        0        0    14947 2024-05-15 23:41:11.154806 qrawl-0.2.0/qrawl/selenium/selenium.py
--rw-r--r--   0        0        0     2870 2024-05-15 22:58:40.129052 qrawl-0.2.0/qrawl/selenium/wait.py
--rw-r--r--   0        0        0     1321 2024-04-05 07:18:07.077122 qrawl-0.2.0/qrawl/xpath.py
--rw-r--r--   0        0        0       37 2024-04-10 20:13:30.588327 qrawl-0.2.0/README.md
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 qrawl-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-10 20:13:30.588327 qrawl-0.2.1/LICENSE
+-rw-r--r--   0        0        0      794 2024-05-16 00:46:31.677047 qrawl-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-09 08:01:21.111154 qrawl-0.2.1/qrawl/__init__.py
+-rw-r--r--   0        0        0     1267 2024-04-09 07:59:51.136473 qrawl-0.2.1/qrawl/common.py
+-rw-r--r--   0        0        0      322 2024-05-01 06:43:35.164934 qrawl-0.2.1/qrawl/exceptions.py
+-rw-r--r--   0        0        0       28 2024-04-05 07:23:15.121016 qrawl-0.2.1/qrawl/google_sheets/__init__.py
+-rw-r--r--   0        0        0     2224 2024-04-10 20:17:48.321751 qrawl-0.2.1/qrawl/google_sheets/column.py
+-rw-r--r--   0        0        0       56 2024-04-09 23:05:42.684682 qrawl-0.2.1/qrawl/playwright/async_api/__init__.py
+-rw-r--r--   0        0        0     4002 2024-04-10 20:18:37.778395 qrawl-0.2.1/qrawl/playwright/async_api/async_playwright.py
+-rw-r--r--   0        0        0      663 2024-04-05 06:47:08.312708 qrawl-0.2.1/qrawl/playwright/async_api/common.py
+-rw-r--r--   0        0        0       55 2024-04-09 23:05:16.406743 qrawl-0.2.1/qrawl/playwright/sync_api/__init__.py
+-rw-r--r--   0        0        0      587 2024-04-09 23:01:33.394056 qrawl-0.2.1/qrawl/playwright/sync_api/common.py
+-rw-r--r--   0        0        0     3933 2024-04-11 06:02:26.308965 qrawl-0.2.1/qrawl/playwright/sync_api/sync_playwright.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:46:13.447864 qrawl-0.2.1/qrawl/scrapy/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-10 20:18:05.787009 qrawl-0.2.1/qrawl/selenium/__init__.py
+-rw-r--r--   0        0        0     7026 2024-05-05 01:32:19.143557 qrawl-0.2.1/qrawl/selenium/browsermob_proxy_wrapper.py
+-rw-r--r--   0        0        0     2681 2024-05-16 00:38:08.502330 qrawl-0.2.1/qrawl/selenium/exceptions.py
+-rw-r--r--   0        0        0    15018 2024-05-16 00:43:45.377209 qrawl-0.2.1/qrawl/selenium/selenium.py
+-rw-r--r--   0        0        0     2870 2024-05-15 22:58:40.129052 qrawl-0.2.1/qrawl/selenium/wait.py
+-rw-r--r--   0        0        0     1321 2024-04-05 07:18:07.077122 qrawl-0.2.1/qrawl/xpath.py
+-rw-r--r--   0        0        0       37 2024-04-10 20:13:30.588327 qrawl-0.2.1/README.md
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 qrawl-0.2.1/PKG-INFO
```

### Comparing `qrawl-0.2.0/LICENSE` & `qrawl-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.0/pyproject.toml` & `qrawl-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qrawl"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python Crawling Utilities."
 authors = ["GGLionCross"]
 license = "Apache 2.0"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `qrawl-0.2.0/qrawl/common.py` & `qrawl-0.2.1/qrawl/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.0/qrawl/google_sheets/column.py` & `qrawl-0.2.1/qrawl/google_sheets/column.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.0/qrawl/playwright/async_api/async_playwright.py` & `qrawl-0.2.1/qrawl/playwright/async_api/async_playwright.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.0/qrawl/playwright/async_api/common.py` & `qrawl-0.2.1/qrawl/playwright/async_api/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.0/qrawl/playwright/sync_api/common.py` & `qrawl-0.2.1/qrawl/playwright/sync_api/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.0/qrawl/playwright/sync_api/sync_playwright.py` & `qrawl-0.2.1/qrawl/playwright/sync_api/sync_playwright.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.0/qrawl/selenium/browsermob_proxy_wrapper.py` & `qrawl-0.2.1/qrawl/selenium/browsermob_proxy_wrapper.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.0/qrawl/selenium/exceptions.py` & `qrawl-0.2.1/qrawl/selenium/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,32 @@
         message="<y>Module 'undetected_chromedriver' not installed.",
     ):
         self.message = ctext(message)
         super().__init__(self.message)
 
 
 # * MISCELLANEOUS Exceptions
+class ChromePathAndVersionUnnecessary(Exception):
+    # Raise this when undetected_chromedriver is not installed
+    def __init__(
+        self,
+        message="<y>QSelenium: Both 'chrome_path' and 'chrome_version' are unnecessary. Only set 1.",
+    ):
+        self.message = ctext(message)
+        super().__init__(self.message)
+
+
+class FailedToGetChromeVersion(Exception):
+    # Raise this when browsermob proxy path is missing
+    def __init__(self, chrome_path):
+        message = f"<r>Failed to get chrome version. Chrome Path: {chrome_path}."
+        self.message = ctext(message)
+        super().__init__(self.message)
+
+
 class MissingBrowsermobProxyPath(Exception):
     # Raise this when browsermob proxy path is missing
     def __init__(
         self,
         message="<y>'browsermob_proxy_path' is empty. Check your proxy configuration.",
     ):
         self.message = ctext(message)
```

### Comparing `qrawl-0.2.0/qrawl/selenium/selenium.py` & `qrawl-0.2.1/qrawl/selenium/selenium.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     from seleniumwire import webdriver as sw
 except ModuleNotFoundError:
     sw = None
 
 # Local Libraries
 # Make it so installing browsermobproxy is optional
 from .browsermob_proxy_wrapper import BrowsermobProxyWrapper
+from .exceptions import FailedToGetChromeVersion
 from .exceptions import SeleniumWireAndUndetectedChromedriverIncompatible
 from .exceptions import SeleniumWireNotInstalled
 from .exceptions import UndetectedChromedriverNotInstalled
 from .wait import QSeleniumWait
 
 
 class QSelenium(QSeleniumWait):
@@ -39,16 +40,15 @@
     # https://chromedriver.storage.googleapis.com/
     DEFAULT_CHROME_VERSION = "114.0.5735.90"
 
     def __init__(
         self,
         chrome_options: dict,
         chrome_capabilities: dict = {},
-        chrome_path: str = "",
-        chrome_version: str = "",
+        driver_path: str = "",
         clear_cookies: bool = False,
         bmp_options: dict = {},  # browsermob proxy
         use_selenium_wire: bool = False,
         use_undetected_chromedriver: bool = False,
         initialize_driver: bool = True,
         timeout_default: int = 10,
         use_logger: bool = False,
@@ -89,16 +89,17 @@
         self._set_chrome_options(chrome_options)
 
         # Set chrome capabilities
         self._chrome_capabilities = None
         self._set_chrome_capabilities(chrome_capabilities)
 
         # Set chromedriver path
-        self._chrome_path = None
-        self._set_chrome_path(chrome_path, chrome_version)
+        self._driver_path = None
+        chrome_version = chrome_options.get("version")
+        self._set_driver_path(driver_path, chrome_version)
 
         # Automatically initialize the driver by default on object creation.
         self._dr = None
         if initialize_driver:
             self.initialize_driver()
 
             # Try this to avoid tracking cookies potentially flagging your bot.
@@ -135,33 +136,34 @@
             "proxy": {
                 "http": f"{proxy_url}",
                 "https": f"{proxy_url}",
                 "verify_ssl": True,
             },
         }
 
-    def _set_chrome_path(self, path: str = "", version: str = ""):
+    def _set_driver_path(self, path: str = "", version: str = ""):
         if path != "":
-            self._chrome_path = path
-            self.logger.info(f"Chrome Path: {path}")
+            self._driver_path = path
         else:
             v = ""
             if version != "":
                 v = version
             else:
                 v = QSelenium.DEFAULT_CHROME_VERSION
 
             self.logger.info(f"Chrome Version: {v}")
 
             # Automatically installs chromedriver with specified version
             try:
-                self._chrome_path = ChromeDriverManager(version=v).install()
+                self._driver_path = ChromeDriverManager(version=v).install()
             except:
                 # Alternative parameter name: driver_version
-                self._chrome_path = ChromeDriverManager(driver_version=v).install()
+                self._driver_path = ChromeDriverManager(driver_version=v).install()
+
+        self.logger.info(f"Driver Path: {self._driver_path}")
 
     def _set_chrome_options(self, chrome_options: dict):
         o = ChromeOptions()
 
         # Adding argument to disable the AutomationControlled flag
         o.add_argument("--disable-blink-features=AutomationControlled")
 
@@ -213,17 +215,17 @@
             o.add_argument(f"--headless")
 
         # Utilizing browsermob proxy
         if self._bmp is not None:
             o.add_argument(f"--proxy-server={self._bmp.proxy_url()}")
             self.logger.debug(f"Proxy Server: {self._bmp.proxy_url()}")
 
-        if chrome_options.get("chrome_exe_path"):
-            o.binary_location = chrome_options["chrome_exe_path"]
-            self.logger.debug(f"Chrome Exe: {chrome_options['chrome_exe_path']}")
+        if chrome_options.get("chrome_path"):
+            o.binary_location = chrome_options["chrome_path"]
+            self.logger.debug(f"Chrome Path: {chrome_options['chrome_path']}")
 
         self._chrome_options = o
         return self._chrome_options
 
     def _set_chrome_capabilities(self, chrome_capabilities: dict):
         c = DesiredCapabilities.CHROME.copy()
 
@@ -257,20 +259,20 @@
                     ),
                 }
             )
 
         if self._use_uc:
             chrome_params.update(
                 {
-                    "driver_executable_path": self._chrome_path,
+                    "driver_executable_path": self._driver_path,
                     "browser_executable_path": self._chrome_options.binary_location,
                 }
             )
         else:
-            chrome_params.update({"service": Service(self._chrome_path)})
+            chrome_params.update({"service": Service(self._driver_path)})
 
         if self._use_uc:
             self._dr = uc.Chrome(**chrome_params)
         elif self._use_sw:
             self._dr = sw.Chrome(**chrome_params)
         else:
             self._dr = Chrome(**chrome_params)
```

### Comparing `qrawl-0.2.0/qrawl/selenium/wait.py` & `qrawl-0.2.1/qrawl/selenium/wait.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.0/qrawl/xpath.py` & `qrawl-0.2.1/qrawl/xpath.py`

 * *Files identical despite different names*

