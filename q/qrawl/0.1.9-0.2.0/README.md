# Comparing `tmp/qrawl-0.1.9.tar.gz` & `tmp/qrawl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrawl-0.1.9.tar", max compression
+gzip compressed data, was "qrawl-0.2.0.tar", max compression
```

## Comparing `qrawl-0.1.9.tar` & `qrawl-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0    11558 2024-04-10 20:13:30.588327 qrawl-0.1.9/LICENSE
--rw-r--r--   0        0        0      794 2024-05-01 07:29:17.131925 qrawl-0.1.9/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-09 08:01:21.111154 qrawl-0.1.9/qrawl/__init__.py
--rw-r--r--   0        0        0     1267 2024-04-09 07:59:51.136473 qrawl-0.1.9/qrawl/common.py
--rw-r--r--   0        0        0      322 2024-05-01 06:43:35.164934 qrawl-0.1.9/qrawl/exceptions.py
--rw-r--r--   0        0        0       28 2024-04-05 07:23:15.121016 qrawl-0.1.9/qrawl/google_sheets/__init__.py
--rw-r--r--   0        0        0     2224 2024-04-10 20:17:48.321751 qrawl-0.1.9/qrawl/google_sheets/column.py
--rw-r--r--   0        0        0       56 2024-04-09 23:05:42.684682 qrawl-0.1.9/qrawl/playwright/async_api/__init__.py
--rw-r--r--   0        0        0     4002 2024-04-10 20:18:37.778395 qrawl-0.1.9/qrawl/playwright/async_api/async_playwright.py
--rw-r--r--   0        0        0      663 2024-04-05 06:47:08.312708 qrawl-0.1.9/qrawl/playwright/async_api/common.py
--rw-r--r--   0        0        0       55 2024-04-09 23:05:16.406743 qrawl-0.1.9/qrawl/playwright/sync_api/__init__.py
--rw-r--r--   0        0        0      587 2024-04-09 23:01:33.394056 qrawl-0.1.9/qrawl/playwright/sync_api/common.py
--rw-r--r--   0        0        0     3933 2024-04-11 06:02:26.308965 qrawl-0.1.9/qrawl/playwright/sync_api/sync_playwright.py
--rw-r--r--   0        0        0        0 2024-04-03 00:46:13.447864 qrawl-0.1.9/qrawl/scrapy/__init__.py
--rw-r--r--   0        0        0       33 2024-04-10 20:18:05.787009 qrawl-0.1.9/qrawl/selenium/__init__.py
--rw-r--r--   0        0        0     6692 2024-05-01 07:28:34.269298 qrawl-0.1.9/qrawl/selenium/browsermob_proxy_wrapper.py
--rw-r--r--   0        0        0     1948 2024-05-01 07:26:17.833098 qrawl-0.1.9/qrawl/selenium/exceptions.py
--rw-r--r--   0        0        0    15799 2024-05-01 06:29:28.782685 qrawl-0.1.9/qrawl/selenium/selenium.py
--rw-r--r--   0        0        0     1321 2024-04-05 07:18:07.077122 qrawl-0.1.9/qrawl/xpath.py
--rw-r--r--   0        0        0       37 2024-04-10 20:13:30.588327 qrawl-0.1.9/README.md
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 qrawl-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-10 20:13:30.588327 qrawl-0.2.0/LICENSE
+-rw-r--r--   0        0        0      794 2024-05-15 23:43:12.405635 qrawl-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-09 08:01:21.111154 qrawl-0.2.0/qrawl/__init__.py
+-rw-r--r--   0        0        0     1267 2024-04-09 07:59:51.136473 qrawl-0.2.0/qrawl/common.py
+-rw-r--r--   0        0        0      322 2024-05-01 06:43:35.164934 qrawl-0.2.0/qrawl/exceptions.py
+-rw-r--r--   0        0        0       28 2024-04-05 07:23:15.121016 qrawl-0.2.0/qrawl/google_sheets/__init__.py
+-rw-r--r--   0        0        0     2224 2024-04-10 20:17:48.321751 qrawl-0.2.0/qrawl/google_sheets/column.py
+-rw-r--r--   0        0        0       56 2024-04-09 23:05:42.684682 qrawl-0.2.0/qrawl/playwright/async_api/__init__.py
+-rw-r--r--   0        0        0     4002 2024-04-10 20:18:37.778395 qrawl-0.2.0/qrawl/playwright/async_api/async_playwright.py
+-rw-r--r--   0        0        0      663 2024-04-05 06:47:08.312708 qrawl-0.2.0/qrawl/playwright/async_api/common.py
+-rw-r--r--   0        0        0       55 2024-04-09 23:05:16.406743 qrawl-0.2.0/qrawl/playwright/sync_api/__init__.py
+-rw-r--r--   0        0        0      587 2024-04-09 23:01:33.394056 qrawl-0.2.0/qrawl/playwright/sync_api/common.py
+-rw-r--r--   0        0        0     3933 2024-04-11 06:02:26.308965 qrawl-0.2.0/qrawl/playwright/sync_api/sync_playwright.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:46:13.447864 qrawl-0.2.0/qrawl/scrapy/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-10 20:18:05.787009 qrawl-0.2.0/qrawl/selenium/__init__.py
+-rw-r--r--   0        0        0     7026 2024-05-05 01:32:19.143557 qrawl-0.2.0/qrawl/selenium/browsermob_proxy_wrapper.py
+-rw-r--r--   0        0        0     2034 2024-05-01 20:20:39.665636 qrawl-0.2.0/qrawl/selenium/exceptions.py
+-rw-r--r--   0        0        0    14947 2024-05-15 23:41:11.154806 qrawl-0.2.0/qrawl/selenium/selenium.py
+-rw-r--r--   0        0        0     2870 2024-05-15 22:58:40.129052 qrawl-0.2.0/qrawl/selenium/wait.py
+-rw-r--r--   0        0        0     1321 2024-04-05 07:18:07.077122 qrawl-0.2.0/qrawl/xpath.py
+-rw-r--r--   0        0        0       37 2024-04-10 20:13:30.588327 qrawl-0.2.0/README.md
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 qrawl-0.2.0/PKG-INFO
```

### Comparing `qrawl-0.1.9/LICENSE` & `qrawl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.9/pyproject.toml` & `qrawl-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qrawl"
-version = "0.1.9"
+version = "0.2.0"
 description = "Python Crawling Utilities."
 authors = ["GGLionCross"]
 license = "Apache 2.0"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `qrawl-0.1.9/qrawl/common.py` & `qrawl-0.2.0/qrawl/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.9/qrawl/google_sheets/column.py` & `qrawl-0.2.0/qrawl/google_sheets/column.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.9/qrawl/playwright/async_api/async_playwright.py` & `qrawl-0.2.0/qrawl/playwright/async_api/async_playwright.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.9/qrawl/playwright/async_api/common.py` & `qrawl-0.2.0/qrawl/playwright/async_api/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.9/qrawl/playwright/sync_api/common.py` & `qrawl-0.2.0/qrawl/playwright/sync_api/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.9/qrawl/playwright/sync_api/sync_playwright.py` & `qrawl-0.2.0/qrawl/playwright/sync_api/sync_playwright.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.9/qrawl/selenium/browsermob_proxy_wrapper.py` & `qrawl-0.2.0/qrawl/selenium/browsermob_proxy_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Standard Libraries
 from base64 import b64decode
 import json
 import time
 
 # Third-party Libraries
-from lytils import cprint
-from lytils.file import LyFile
+from lytils.logger import LyLogger
 from lytils.regex import match
 from selenium.common.exceptions import TimeoutException
 
 # * OPTIONAL IMPORTS
 try:
     from browsermobproxy import Server
 except ModuleNotFoundError:
@@ -23,29 +22,43 @@
 # Local Libraries
 from .exceptions import BrowsermobProxyNotInstalled
 from .exceptions import MissingBrowsermobProxyPath
 from .exceptions import PsutilNotInstalled
 
 
 class BrowsermobProxyWrapper:
-    def __init__(self, browsermob_proxy_path: str, port=9090, debug: bool = False):
-        self._debug = debug
+    def __init__(
+        self,
+        browsermob_proxy_path: str,
+        port: int = 9090,
+        log_path="logs/BMP",
+        log_level="warning",
+    ):
+        """
+        Wrapper for browsermob-proxy utility for Selenium.
+
+        Args:
+            browsermob_proxy_path (str): Path of browsermob proxy installation.
+            port (int): Port to run browsermob proxy server on.
+            log_path (str): Directory path to store browsermob proxy related logs.
+            log_level (str): Level of logs desired. From least to most: debug > info > warning > error > critical.
+        """
+
         if Server is None:
             raise BrowsermobProxyNotInstalled
         if psutil is None:
             raise PsutilNotInstalled
         if not browsermob_proxy_path:
             raise MissingBrowsermobProxyPath
 
-        options = {"port": port}
+        self.log_path = log_path
+        self.log_level = log_level
 
-        if self._debug:
-            cprint(f"<y>DEBUG: BMP browsermob_proxy_path = {browsermob_proxy_path}")
-            cprint(f"<y>DEBUG: BMP port = {port}")
-            options.update({"log_path": "browsermob-proxy.log"})
+        options = {"port": port}
+        options.update({"log_path": f"{log_path}/browsermob-proxy.log"})
 
         self.kill_existing_bmp()  # Kill existing browsermob proxies before starting
         self._server = Server(browsermob_proxy_path, options=options)
         self._client = None
 
     def kill_existing_bmp(self):
         for proc in psutil.process_iter():
@@ -83,16 +96,20 @@
             "captureBinaryContent": True,
         }
         self._client.new_har(name, options=options)
 
     def har(self):
         return self._client.har
 
-    def _get_response_from_content(self, content: dict, debug: bool = False):
-        debug_path = "debug/BMP/_get_response_from_content.txt"
+    def _get_response_from_content(self, content: dict):
+        logger = LyLogger(
+            "bmp_get_response_from_content"
+            f"{self.log_path}/_get_response_from_content.log",
+            level=self.log_level,
+        )
 
         try:
             # No decoding necessary
             return json.loads(content["text"])
 
         except json.decoder.JSONDecodeError:
             # response -> content -> text is not a json string
@@ -101,104 +118,104 @@
             if encoding == "base64":
                 charset = match(r"(?<=charset=).+", content["mimeType"])
                 decoded_bytes = b64decode(content["text"])
 
                 # decoded_str = decoded_bytes.decode(charset)
                 decoded_str = decoded_bytes.decode(charset)
 
-                if debug:
-                    # Print request url and response
-                    append_line(debug_path, decoded_str)
+                logger.debug(decoded_str)
 
                 return json.loads(decoded_str)
 
         except KeyError:
             # response -> content -> text does not exist
             raise KeyError
 
     def wait_for_response(
         self,
         partial_request_url: str,
         poll_interval: int = 1,
         timeout: int = 10,
-        debug: bool = False,
     ):
         """
         Either returns a response or raises a timeout exception.
         """
-        debug_file = LyFile("debug/BMP/wait_for_response.txt")
-        if debug:
-            debug_file.create()
+        logger = LyLogger(
+            "bmp_wait_for_response" f"{self.log_path}/_wait_for_response.log",
+            level=self.log_level,
+        )
 
         start_time = time.time()  # Record start time for timeout
 
         while time.time() - start_time < timeout:
 
             for entry in self._client.har["log"]["entries"]:
 
                 if partial_request_url in json.dumps(entry["request"]["url"]):
 
-                    if debug:
-                        # Print request url and response
-                        debug_file.append(entry["request"]["url"])
-                        debug_file.append_json(entry["response"])
+                    # Print request url and response
+                    logger.debug_json(
+                        f'BMP: {entry["request"]["url"]}:',
+                        entry["response"],
+                    )
 
                     content = entry["response"]["content"]
 
                     try:
                         # No decoding necessary
-                        return self._get_response_from_content(content, debug=True)
+                        return self._get_response_from_content(content)
 
                     except KeyError:
                         # response -> content -> text does not exist
                         continue
 
             # ping requests against after interval has passed
             time.sleep(poll_interval)
 
         # If code reaches outside of loop, it is because of timeout.
 
-        if debug:
-            duration = time.time() - start_time
-            debug_file.append(f"Timed out. Duration: {round(duration, 3)} seconds.")
+        duration = time.time() - start_time
+        logger.info(f"Timed out. Duration: {round(duration, 3)} seconds.")
 
         raise TimeoutException
 
     # Troubleshoot request urls
     def get_request_urls(self):
         request_urls = []
         for entry in self._client.har["log"]["entries"]:
             request_urls.append(entry["request"]["url"])
         return request_urls
 
-    def get_responses(self, partial_request_url: str, debug: bool = False):
-        debug_file = LyFile("debug/BMP/get_responses.txt")
-        if debug:
-            debug_file.create()
+    def get_responses(self, partial_request_url: str):
+        logger = LyLogger(
+            "bmp_get_responses" f"{self.log_path}/get_responses.log",
+            level=self.log_level,
+        )
 
         responses = []
         for entry in self._client.har["log"]["entries"]:
 
             if partial_request_url in entry["request"]["url"]:
 
-                if debug:
-                    # Print request url and response
-                    debug_file.append(entry["request"]["url"])
-                    debug_file.append_json(entry["response"])
+                # Print request url and response
+                logger.debug_json(
+                    f'BMP: {entry["request"]["url"]}:',
+                    entry["response"],
+                )
 
                 content = entry["response"]["content"]
 
                 try:
-                    response = self._get_response_from_content(content, debug=False)
+                    response = self._get_response_from_content(content)
                     responses.append(response)
 
                 except KeyError:
                     continue
 
-        if debug and len(responses) == 0:
-            debug_file.append(f"url '{partial_request_url}' not found.")
+        if len(responses) == 0:
+            logger.info(f"Url '{partial_request_url}' not found.")
 
         return responses
 
     def close(self):
         self._client.close()
         self._server.stop()
```

### Comparing `qrawl-0.1.9/qrawl/selenium/exceptions.py` & `qrawl-0.2.0/qrawl/selenium/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 from lytils import ctext
 
 
-# BMP Exceptions
+# * MODULE NOT INSTALLED Exceptions
 class BrowsermobProxyNotInstalled(Exception):
     # Raise this when browsermob proxy path is missing
     def __init__(
         self,
         message="Module 'browsermob-proxy' not installed.",
     ):
         self.message = ctext(message)
         super().__init__(self.message)
 
 
-class MissingBrowsermobProxyPath(Exception):
-    # Raise this when browsermob proxy path is missing
+class PsutilNotInstalled(Exception):
+    # Raise this when undetected_chromedriver is not installed
     def __init__(
         self,
-        message="<y>'browsermob_proxy_path' is empty. Check your proxy configuration.",
+        message="<y>Module 'psutil' not installed.",
     ):
         self.message = ctext(message)
         super().__init__(self.message)
 
 
-class PsutilNotInstalled(Exception):
+class SeleniumWireNotInstalled(Exception):
     # Raise this when undetected_chromedriver is not installed
     def __init__(
         self,
-        message="<y>Module 'psutil' not installed.",
+        message="<y>Module 'selenium-wire' not installed or 'blinker@1.7.0' is not installed.",
     ):
         self.message = ctext(message)
         super().__init__(self.message)
 
 
-class SeleniumWireAndUndetectedChromedriverIncompatible(Exception):
+class UndetectedChromedriverNotInstalled(Exception):
     # Raise this when undetected_chromedriver is not installed
     def __init__(
         self,
-        message="<y>Selenium Wire and Undetected Chromedriver are incompatible. Please only set 'use_selenium_wire' OR 'use_undetected_chromedriver'.",
+        message="<y>Module 'undetected_chromedriver' not installed.",
     ):
         self.message = ctext(message)
         super().__init__(self.message)
 
 
-class SeleniumWireNotInstalled(Exception):
-    # Raise this when undetected_chromedriver is not installed
+# * MISCELLANEOUS Exceptions
+class MissingBrowsermobProxyPath(Exception):
+    # Raise this when browsermob proxy path is missing
     def __init__(
         self,
-        message="<y>Module 'seleniumwire' not installed.",
+        message="<y>'browsermob_proxy_path' is empty. Check your proxy configuration.",
     ):
         self.message = ctext(message)
         super().__init__(self.message)
 
 
-class UndetectedChromedriverNotInstalled(Exception):
+class SeleniumWireAndUndetectedChromedriverIncompatible(Exception):
     # Raise this when undetected_chromedriver is not installed
     def __init__(
         self,
-        message="<y>Module 'undetected_chromedriver' not installed.",
+        message="<y>Selenium Wire and Undetected Chromedriver are incompatible. Please only set 'use_selenium_wire' OR 'use_undetected_chromedriver'.",
     ):
         self.message = ctext(message)
         super().__init__(self.message)
```

### Comparing `qrawl-0.1.9/qrawl/selenium/selenium.py` & `qrawl-0.2.0/qrawl/selenium/selenium.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Standard Libraries
 import random
 import time
 
 # Third-party Libraries
 from lytils import cprint, cinput, print_trace, pause
+from lytils.logger import LyLogger
 from selenium.common.exceptions import TimeoutException, WebDriverException
 from selenium.webdriver import Chrome, ChromeOptions
 from selenium.webdriver import DesiredCapabilities
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
@@ -26,47 +27,51 @@
 
 # Local Libraries
 # Make it so installing browsermobproxy is optional
 from .browsermob_proxy_wrapper import BrowsermobProxyWrapper
 from .exceptions import SeleniumWireAndUndetectedChromedriverIncompatible
 from .exceptions import SeleniumWireNotInstalled
 from .exceptions import UndetectedChromedriverNotInstalled
+from .wait import QSeleniumWait
 
 
-class QSelenium:
+class QSelenium(QSeleniumWait):
     # Latest release can be found at:
     # https://chromedriver.storage.googleapis.com/
-    _DEFAULT_CHROMEDRIVER_VERSION = "114.0.5735.90"
+    DEFAULT_CHROME_VERSION = "114.0.5735.90"
 
     def __init__(
         self,
         chrome_options: dict,
         chrome_capabilities: dict = {},
-        chromedriver_path: str = "",
-        chromedriver_version: str = "",
+        chrome_path: str = "",
+        chrome_version: str = "",
         clear_cookies: bool = False,
         bmp_options: dict = {},  # browsermob proxy
-        use_undetected_chromedriver: bool = False,
         use_selenium_wire: bool = False,
+        use_undetected_chromedriver: bool = False,
         initialize_driver: bool = True,
         timeout_default: int = 10,
-        debug: bool = False,
+        use_logger: bool = False,
     ):
         # * Raise errors IMMEDIATELY if desired imports are not available
-        self._use_uc = use_undetected_chromedriver
-        if self._use_uc and uc == None:
+        if use_selenium_wire and use_undetected_chromedriver:
+            raise SeleniumWireAndUndetectedChromedriverIncompatible
+        if use_selenium_wire and sw == None:
+            # ! If selenium-wire is installed, and we are still raising this exception:
+            # ! it could be because the blinker package introduced a breaking change in 1.8.0+
+            # * It should work if you use blinker@1.7.0
+            raise SeleniumWireNotInstalled
+        if use_undetected_chromedriver and uc == None:
             raise UndetectedChromedriverNotInstalled
-        self._use_sw = use_selenium_wire
-        if self._use_sw and sw == None:
-            if self._use_uc:
-                raise SeleniumWireAndUndetectedChromedriverIncompatible
-            elif sw == None:
-                raise SeleniumWireNotInstalled
 
-        self._debug = debug
+        self.logger = LyLogger("QSelenium", use_logger=use_logger)
+
+        self._use_sw = use_selenium_wire
+        self._use_uc = use_undetected_chromedriver
         self._timeout_default = timeout_default
 
         # * Set DEFAULT headers here
         self._headers = {
             "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
             "sec-ch-ua": '"Not_A Brand";v="8", "Chromium";v="120", "Brave";v="120"',
             "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8",
@@ -84,16 +89,16 @@
         self._set_chrome_options(chrome_options)
 
         # Set chrome capabilities
         self._chrome_capabilities = None
         self._set_chrome_capabilities(chrome_capabilities)
 
         # Set chromedriver path
-        self._chromedriver_path = None
-        self._set_chromedriver_path(chromedriver_path, chromedriver_version)
+        self._chrome_path = None
+        self._set_chrome_path(chrome_path, chrome_version)
 
         # Automatically initialize the driver by default on object creation.
         self._dr = None
         if initialize_driver:
             self.initialize_driver()
 
             # Try this to avoid tracking cookies potentially flagging your bot.
@@ -111,55 +116,52 @@
         """
         Teardown Function
         """
         # Close driver if it was initialized
         if self._dr:
             self._dr.close()
             self._dr.quit()
+            self.logger.info("Driver closed.")
 
         # Close browsermob-proxy if it exists
         if self._bmp:
             self._bmp.close()
+            self.logger.info("Browsermob-proxy server closed.")
 
     # * PRIVATE Functions START
     # region
     def _get_seleniumwire_options(self, proxy_url: str):
         # Return the seleniumwire_options to be used with seleniumwire.webdriver.Chrome
         return {
             "proxy": {
                 "http": f"{proxy_url}",
                 "https": f"{proxy_url}",
                 "verify_ssl": True,
             },
         }
 
-    def _set_chromedriver_path(self, chromedriver_path: str, chromedriver_version: str):
-        # Get chromedriver version
-        version = ""
-        if chromedriver_version != "":
-            version = chromedriver_version
+    def _set_chrome_path(self, path: str = "", version: str = ""):
+        if path != "":
+            self._chrome_path = path
+            self.logger.info(f"Chrome Path: {path}")
         else:
-            version = QSelenium._DEFAULT_CHROMEDRIVER_VERSION
+            v = ""
+            if version != "":
+                v = version
+            else:
+                v = QSelenium.DEFAULT_CHROME_VERSION
 
-        # Latest release can be found at:
-        # https://chromedriver.storage.googleapis.com/
-        if self._debug:
-            cprint(f"<y>DEBUG: <w>Using chromedriver version {version}")
+            self.logger.info(f"Chrome Version: {v}")
 
-        if chromedriver_path != "":
-            self._chromedriver_path = chromedriver_path
-        else:
             # Automatically installs chromedriver with specified version
             try:
-                self._chromedriver_path = ChromeDriverManager(version=version).install()
+                self._chrome_path = ChromeDriverManager(version=v).install()
             except:
                 # Alternative parameter name: driver_version
-                self._chromedriver_path = ChromeDriverManager(
-                    driver_version=version
-                ).install()
+                self._chrome_path = ChromeDriverManager(driver_version=v).install()
 
     def _set_chrome_options(self, chrome_options: dict):
         o = ChromeOptions()
 
         # Adding argument to disable the AutomationControlled flag
         o.add_argument("--disable-blink-features=AutomationControlled")
 
@@ -199,25 +201,29 @@
         # o.add_argument('--disable-dev-shm-usage')
         # o.add_argument("--no-default-browser-check")
         # o.add_argument("--no-first-run")
         # o.binary_location = 'G:\My Drive\Programs\Google Chrome\GoogleChromePortable\App\Chrome-bin\chrome.exe'
 
         if chrome_options.get("user_data_path"):
             o.add_argument(f'--user-data-dir={chrome_options["user_data_path"]}')
+            self.logger.debug(f"User Data Path: {chrome_options['user_data_path']}")
         if chrome_options.get("profile_path"):
             o.add_argument(f'--profile-directory={chrome_options["profile_path"]}')
+            self.logger.debug(f"Profile Path: {chrome_options['profile_path']}")
         if chrome_options.get("headless"):
             o.add_argument(f"--headless")
 
         # Utilizing browsermob proxy
         if self._bmp is not None:
             o.add_argument(f"--proxy-server={self._bmp.proxy_url()}")
+            self.logger.debug(f"Proxy Server: {self._bmp.proxy_url()}")
 
         if chrome_options.get("chrome_exe_path"):
             o.binary_location = chrome_options["chrome_exe_path"]
+            self.logger.debug(f"Chrome Exe: {chrome_options['chrome_exe_path']}")
 
         self._chrome_options = o
         return self._chrome_options
 
     def _set_chrome_capabilities(self, chrome_capabilities: dict):
         c = DesiredCapabilities.CHROME.copy()
 
@@ -234,17 +240,16 @@
         self._chrome_capabilities = c
         return self._chrome_capabilities
 
     def _remove_navigator_webdriver(self):
         """
         Sets navigator.webdriver to undefined to avoid detection.
         """
-        self._dr.execute_script(
-            "Object.defineProperty(navigator, 'webdriver', {get: () => undefined})"
-        )
+        script = "Object.defineProperty(navigator, 'webdriver', {get: () => undefined})"
+        self._dr.execute_script(script)
 
     def _set_driver(self):
         chrome_params = {"options": self._chrome_options}
         if self._use_sw and self._bmp is not None:
             chrome_params.update(
                 {
                     "seleniumwire_options": self._get_seleniumwire_options(
@@ -252,28 +257,31 @@
                     ),
                 }
             )
 
         if self._use_uc:
             chrome_params.update(
                 {
-                    "driver_executable_path": self._chromedriver_path,
+                    "driver_executable_path": self._chrome_path,
                     "browser_executable_path": self._chrome_options.binary_location,
                 }
             )
         else:
-            chrome_params.update({"service": Service(self._chromedriver_path)})
+            chrome_params.update({"service": Service(self._chrome_path)})
 
         if self._use_uc:
             self._dr = uc.Chrome(**chrome_params)
         elif self._use_sw:
             self._dr = sw.Chrome(**chrome_params)
         else:
             self._dr = Chrome(**chrome_params)
 
+        # After setting driver, initialize QSeleniumWait
+        QSeleniumWait.__init__(self, self._dr, self._timeout_default)
+
         self._remove_navigator_webdriver()
 
     def _clear_cookies(self):
         self._dr.delete_all_cookies()
 
     # endregion
     # * PRIVATE Functions END
@@ -302,21 +310,21 @@
             print_trace()
 
         return self._dr
 
     def get_driver(self):
         return self._dr
 
-    def set_headers(self, headers: dict):
+    def set_headers(self, headers: dict = {}):
         self._headers.update(headers)
 
         def interceptor(request):
             # Delete previous headers to prevent duplicates
             # Then set real request headers
-            for key, value in self._headers.items():
+            for key, value in list(self._headers.items()):
                 del self._headers[key]
                 self._headers[key] = value
 
         # Set the Selenium Wire interceptor
         self._dr.request_interceptor = interceptor
 
     def get_headers(self):
@@ -384,48 +392,7 @@
 
                 # If error occurs, wait_time is exponentially increased
                 wait_time *= 2
                 time.sleep(wait_time)
 
     # endregion
     # * DELAY Functions END
-
-    # * WAIT Functions START
-    # region Wait Functions
-    def wait_until(self, condition, timeout=None):
-        if timeout is None:
-            timeout = self._timeout_default
-        return WebDriverWait(self._dr, timeout).until(condition)
-
-    def wait_until_clickable(self, descriptor, timeout=None):
-        if timeout is None:
-            timeout = self._timeout_default
-        return WebDriverWait(self._dr, timeout).until(
-            EC.element_to_be_clickable(descriptor)
-        )
-
-    def wait_for_element(self, descriptor, timeout=None):
-        if timeout is None:
-            timeout = self._timeout_default
-        return WebDriverWait(self._dr, timeout).until(
-            EC.presence_of_element_located(descriptor)
-        )
-
-    def wait_for_all_elements(self, descriptor, timeout=None):
-        if timeout is None:
-            timeout = self._timeout_default
-        return WebDriverWait(self._dr, timeout).until(
-            EC.presence_of_all_elements_located(descriptor)
-        )
-
-    def wait_for_text_not_empty(self, descriptor, timeout=None):
-        if timeout is None:
-            timeout = self._timeout_default
-        WebDriverWait(self._dr, timeout).until(
-            lambda driver: driver.find_element(*descriptor).text.strip() != ""
-        )
-        return WebDriverWait(self._dr, timeout).until(
-            EC.presence_of_element_located(descriptor)
-        )
-
-    # endregion
-    # * WAIT Functions END
```

### Comparing `qrawl-0.1.9/qrawl/xpath.py` & `qrawl-0.2.0/qrawl/xpath.py`

 * *Files identical despite different names*

