# Comparing `tmp/movoid_robotframework_selenium-1.2.4.tar.gz` & `tmp/movoid_robotframework_selenium-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_robotframework_selenium-1.2.4.tar", last modified: Wed May  8 15:01:02 2024, max compression
+gzip compressed data, was "movoid_robotframework_selenium-1.2.5.tar", last modified: Thu May 16 16:35:36 2024, max compression
```

## Comparing `movoid_robotframework_selenium-1.2.4.tar` & `movoid_robotframework_selenium-1.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 15:01:02.950703 movoid_robotframework_selenium-1.2.4/
--rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework_selenium-1.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0      439 2024-05-08 15:01:02.949683 movoid_robotframework_selenium-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework_selenium-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 15:01:02.928758 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/
--rw-rw-rw-   0        0        0      311 2024-02-20 17:47:42.000000 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 15:01:02.932885 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/action/
--rw-rw-rw-   0        0        0      218 2024-02-20 05:59:20.000000 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/action/__init__.py
--rw-rw-rw-   0        0        0    12876 2024-04-20 10:51:34.000000 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/action/action.py
--rw-rw-rw-   0        0        0     6393 2024-05-08 14:59:24.000000 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/action/action.pyi
--rw-rw-rw-   0        0        0     9778 2024-05-07 13:18:52.000000 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/common.py
--rw-rw-rw-   0        0        0     2717 2024-05-08 14:59:18.000000 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/common.pyi
--rw-rw-rw-   0        0        0      268 2024-02-20 05:59:20.000000 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/main.py
-drwxrwxrwx   0        0        0        0 2024-05-08 15:01:02.941174 movoid_robotframework_selenium-1.2.4/movoid_robotframework_selenium.egg-info/
--rw-rw-rw-   0        0        0      439 2024-05-08 15:01:02.000000 movoid_robotframework_selenium-1.2.4/movoid_robotframework_selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      555 2024-05-08 15:01:02.000000 movoid_robotframework_selenium-1.2.4/movoid_robotframework_selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 15:01:02.000000 movoid_robotframework_selenium-1.2.4/movoid_robotframework_selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-05-08 15:01:02.000000 movoid_robotframework_selenium-1.2.4/movoid_robotframework_selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-05-08 15:01:02.000000 movoid_robotframework_selenium-1.2.4/movoid_robotframework_selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 15:01:02.951715 movoid_robotframework_selenium-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      748 2024-05-08 15:00:49.000000 movoid_robotframework_selenium-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:35:36.370159 movoid_robotframework_selenium-1.2.5/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework_selenium-1.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      439 2024-05-16 16:35:36.368165 movoid_robotframework_selenium-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework_selenium-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 16:35:36.354212 movoid_robotframework_selenium-1.2.5/RobotFrameworkSelenium/
+-rw-rw-rw-   0        0        0      311 2024-02-20 17:47:42.000000 movoid_robotframework_selenium-1.2.5/RobotFrameworkSelenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:35:36.359188 movoid_robotframework_selenium-1.2.5/RobotFrameworkSelenium/action/
+-rw-rw-rw-   0        0        0      218 2024-02-20 05:59:20.000000 movoid_robotframework_selenium-1.2.5/RobotFrameworkSelenium/action/__init__.py
+-rw-rw-rw-   0        0        0    15168 2024-05-16 16:35:03.000000 movoid_robotframework_selenium-1.2.5/RobotFrameworkSelenium/action/action.py
+-rw-rw-rw-   0        0        0     8019 2024-05-16 16:35:03.000000 movoid_robotframework_selenium-1.2.5/RobotFrameworkSelenium/action/action.pyi
+-rw-rw-rw-   0        0        0     9765 2024-05-16 16:35:03.000000 movoid_robotframework_selenium-1.2.5/RobotFrameworkSelenium/common.py
+-rw-rw-rw-   0        0        0     2717 2024-05-08 14:59:18.000000 movoid_robotframework_selenium-1.2.5/RobotFrameworkSelenium/common.pyi
+-rw-rw-rw-   0        0        0      268 2024-02-20 05:59:20.000000 movoid_robotframework_selenium-1.2.5/RobotFrameworkSelenium/main.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:35:36.368165 movoid_robotframework_selenium-1.2.5/movoid_robotframework_selenium.egg-info/
+-rw-rw-rw-   0        0        0      439 2024-05-16 16:35:36.000000 movoid_robotframework_selenium-1.2.5/movoid_robotframework_selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2024-05-16 16:35:36.000000 movoid_robotframework_selenium-1.2.5/movoid_robotframework_selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 16:35:36.000000 movoid_robotframework_selenium-1.2.5/movoid_robotframework_selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-05-16 16:35:36.000000 movoid_robotframework_selenium-1.2.5/movoid_robotframework_selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-05-16 16:35:36.000000 movoid_robotframework_selenium-1.2.5/movoid_robotframework_selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 16:35:36.370159 movoid_robotframework_selenium-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      748 2024-05-16 16:35:20.000000 movoid_robotframework_selenium-1.2.5/setup.py
```

### Comparing `movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/action/action.py` & `movoid_robotframework_selenium-1.2.5/RobotFrameworkSelenium/action/action.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 import pathlib
 import re
 import time
 from typing import List, Union
 
 import cv2
-from RobotFrameworkBasic import robot_log_keyword, do_until_check, do_when_error, RfError
+from RobotFrameworkBasic import robot_log_keyword, do_until_check, do_when_error, RfError, wait_until_stable
 from movoid_function import reset_function_default_value
 from movoid_package import importing
 from selenium.webdriver import Keys
 from selenium.webdriver.remote.webelement import WebElement
 
 BasicCommon = importing('..common', 'BasicCommon')
 
@@ -85,15 +85,19 @@
         find_elements = []
         if find_attribute is None:
             find_elements = tar_elements
             self.print(f'find {len(find_elements)} elements only locator <{find_locator}>')
         else:
             self.print(f'find {len(tar_elements)} elements <{find_locator}> first')
             for i_element, one_element in enumerate(tar_elements):
-                tar_value = one_element.get_attribute(find_attribute)
+                try:
+                    tar_value = one_element.get_attribute(find_attribute)
+                except:
+                    self.print(f'{find_attribute} of <{find_locator}>({i_element}) can not be read, pass it')
+                    continue
                 self.print(f'{find_attribute} of <{find_locator}>({i_element}) is:{tar_value}')
                 if regex:
                     check_result = bool(re.search(find_value, tar_value))
                     self.print(f'{check_result}: <{find_value}> in <{tar_value}>')
                 else:
                     check_result = find_value == tar_value
                     self.print(f'{check_result}: <{find_value}> == <{tar_value}>')
@@ -187,14 +191,30 @@
     @robot_log_keyword
     def selenium_check_element_count_change_loop(self, check_locator):
         now_count = len(self.selenium_find_elements_by_locator(check_locator))
         re_bool = now_count != self._check_element_count_value
         self.print(f'we find {check_locator} count of {now_count} {"!=" if re_bool else "=="}{self._check_element_count_value}')
         return re_bool
 
+    @robot_log_keyword
+    def selenium_check_stable_element_attribute_unchanged_init(self, check_locator, check_attribute='innerText'):
+        tar_element = self.selenium_find_element_by_locator(check_locator)
+        self._check_element_attribute_change_value = tar_element.get_attribute(check_attribute)
+        return False
+
+    @robot_log_keyword
+    def selenium_check_stable_element_attribute_unchanged_loop(self, check_locator, check_attribute='innerText'):
+        tar_element = self.selenium_find_element_by_locator(check_locator)
+        temp_value = tar_element.get_attribute(check_attribute)
+        re_bool = self._check_element_attribute_change_value == temp_value
+        if re_bool is False:
+            self._check_element_attribute_change_value = temp_value
+        self.print(f'we find {check_attribute} of {check_locator} is {temp_value}{"==" if re_bool else "!="}{self._check_element_attribute_change_value}')
+        return re_bool
+
     def always_true(self):
         return True
 
     @robot_log_keyword
     @do_when_error(selenium_take_full_screenshot)
     @do_until_check(always_true, selenium_click_element_with_offset)
     def selenium_click_until_available(self):
@@ -263,7 +283,35 @@
         pass
 
     @robot_log_keyword
     @do_when_error(selenium_take_full_screenshot)
     @do_until_check(selenium_click_element_with_offset, selenium_check_element_count_change_loop, init_check_function=selenium_check_element_count_change_init)
     def selenium_click_until_element_count_change(self):
         pass
+
+    @robot_log_keyword
+    @do_when_error(selenium_take_full_screenshot)
+    @wait_until_stable(selenium_check_contain_element)
+    def selenium_wait_until_stable_find_element(self):
+        pass
+
+    @robot_log_keyword
+    @do_when_error(selenium_take_full_screenshot)
+    @wait_until_stable(selenium_check_contain_elements)
+    def selenium_wait_until_stable_find_elements(self):
+        pass
+
+    @reset_function_default_value(selenium_wait_until_stable_find_element)
+    def selenium_wait_until_stable_not_find_element(self, check_exist=False):
+        pass
+
+    @robot_log_keyword
+    @do_when_error(selenium_take_full_screenshot)
+    @wait_until_stable(selenium_find_element_with_attribute)
+    def selenium_wait_until_stable_find_element_attribute(self):
+        pass
+
+    @robot_log_keyword
+    @do_when_error(selenium_take_full_screenshot)
+    @wait_until_stable(selenium_check_stable_element_attribute_unchanged_loop, init_check_function=selenium_check_stable_element_attribute_unchanged_init)
+    def selenium_wait_until_stable_attribute_unchanged(self):
+        pass
```

### Comparing `movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/action/action.pyi` & `movoid_robotframework_selenium-1.2.5/RobotFrameworkSelenium/action/action.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 	def selenium_input_delete_all_and_input(self, input_locator, input_text):	...
 	def selenium_check_contain_element(self, check_locator, check_exist = True):	...
 	def selenium_check_contain_elements(self, check_locator, check_count = 1):	...
 	def selenium_check_element_attribute_change_init(self, check_locator, check_attribute = 'innerText'):	...
 	def selenium_check_element_attribute_change_loop(self, check_locator, check_attribute = 'innerText'):	...
 	def selenium_check_element_count_change_init(self, check_locator):	...
 	def selenium_check_element_count_change_loop(self, check_locator):	...
+	def selenium_check_stable_element_attribute_unchanged_init(self, check_locator, check_attribute = 'innerText'):	...
+	def selenium_check_stable_element_attribute_unchanged_loop(self, check_locator, check_attribute = 'innerText'):	...
 	def always_true(self):	...
 	def selenium_click_until_available(self, click_locator, x = 0, y = 0, operate = 'click', screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_interval = 0.2, error = True):
 		"""
 		"""
 		...
 	def selenium_wait_until_find_element(self, check_locator, check_exist = True, screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_interval = 0.2, error = True):
 		"""
@@ -88,9 +90,29 @@
 		"""
 		"""
 		...
 	def selenium_click_until_element_count_change(self, click_locator, check_locator, x = 0, y = 0, operate = 'click', screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_interval = 0.2, error = True):
 		"""
 		"""
 		...
+	def selenium_wait_until_stable_find_element(self, check_locator, check_exist = True, screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, stable_time = 3.0, check_interval = 0.2, error = True):
+		"""
+		"""
+		...
+	def selenium_wait_until_stable_find_elements(self, check_locator, check_count = 1, screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, stable_time = 3.0, check_interval = 0.2, error = True):
+		"""
+		"""
+		...
+	def selenium_wait_until_stable_not_find_element(self, check_locator, check_exist = False, screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, stable_time = 3.0, check_interval = 0.2, error = True):
+		"""
+		"""
+		...
+	def selenium_wait_until_stable_find_element_attribute(self, find_locator, find_value = '', find_attribute = 'innerText', regex = True, check_bool = True, screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, stable_time = 3.0, check_interval = 0.2, error = True):
+		"""
+		"""
+		...
+	def selenium_wait_until_stable_attribute_unchanged(self, check_locator, check_attribute = 'innerText', screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, stable_time = 3.0, check_interval = 0.2, error = True):
+		"""
+		"""
+		...
 	...
```

### Comparing `movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/common.py` & `movoid_robotframework_selenium-1.2.5/RobotFrameworkSelenium/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Author        : Sun YiFan-Movoid
 # Time          : 2024/2/16 18:47
 # Description   : 
 """
 import base64
 import math
 import os
-from typing import List, Tuple, Union
+from typing import List, Tuple, Union, Any
 
 import cv2
 import numpy as np
 import robot.libraries.BuiltIn
 import selenium.webdriver.chrome.webdriver
 from RobotFrameworkBasic import RobotBasic, robot_log_keyword, RfError
 from Selenium2Library import Selenium2Library
@@ -125,16 +125,15 @@
                 cv2.imwrite(tar_path_split[0] + '(cut)' + tar_path_split[1], cut_image)
         self.print(f'the shape of cut screenshot is {cut_image.shape}')
         return cut_image
 
     @robot_log_keyword
     def selenium_take_screenshot(self, screenshot_locator=None, image_name='python-screenshot.png', rename=True):
         if self.screenshot_root is None:
-            self.selenium_log_screenshot(screenshot_locator)
-            return None, None
+            return self.selenium_log_screenshot(screenshot_locator), None
         else:
             tar_name = image_name
             ind = 1
             tar_path = self.selenium_get_full_screenshot_path(tar_name)
             while rename and os.path.isfile(tar_path):
                 ind += 1
                 name, post = os.path.splitext(image_name)
```

### Comparing `movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/common.pyi` & `movoid_robotframework_selenium-1.2.5/RobotFrameworkSelenium/common.pyi`

 * *Files identical despite different names*

### Comparing `movoid_robotframework_selenium-1.2.4/movoid_robotframework_selenium.egg-info/SOURCES.txt` & `movoid_robotframework_selenium-1.2.5/movoid_robotframework_selenium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `movoid_robotframework_selenium-1.2.4/setup.py` & `movoid_robotframework_selenium-1.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='movoid_robotframework_selenium',
-    version='1.2.4',
+    version='1.2.5',
     packages=find_packages(),
     url='',
     license='',
     author='movoid',
     author_email='bobrobotsun@163.com',
     description='',
     long_description=long_description,
```

