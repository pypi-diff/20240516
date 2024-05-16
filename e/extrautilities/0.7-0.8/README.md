# Comparing `tmp/extrautilities-0.7.tar.gz` & `tmp/extrautilities-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrautilities-0.7.tar", last modified: Tue May 14 17:51:18 2024, max compression
+gzip compressed data, was "extrautilities-0.8.tar", last modified: Thu May 16 14:49:50 2024, max compression
```

## Comparing `extrautilities-0.7.tar` & `extrautilities-0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 17:51:18.599098 extrautilities-0.7/
-drwxrwxrwx   0        0        0        0 2024-05-14 17:51:18.579395 extrautilities-0.7/ExtraUtils/
--rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-0.7/ExtraUtils/RateLimit.py
--rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-0.7/ExtraUtils/__init__.py
--rw-rw-rw-   0        0        0     1766 2024-05-13 18:01:30.000000 extrautilities-0.7/ExtraUtils/asyncTokens.py
--rw-rw-rw-   0        0        0     1491 2024-05-14 17:48:41.000000 extrautilities-0.7/ExtraUtils/timeBasedToken.py
--rw-rw-rw-   0        0        0     2361 2024-05-14 17:51:18.598591 extrautilities-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1514 2024-05-12 12:05:10.000000 extrautilities-0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 17:51:18.597080 extrautilities-0.7/extrautilities.egg-info/
--rw-rw-rw-   0        0        0     2361 2024-05-14 17:51:18.000000 extrautilities-0.7/extrautilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-05-14 17:51:18.000000 extrautilities-0.7/extrautilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 17:51:18.000000 extrautilities-0.7/extrautilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-14 17:51:18.000000 extrautilities-0.7/extrautilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-14 17:51:18.000000 extrautilities-0.7/extrautilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 17:51:18.599098 extrautilities-0.7/setup.cfg
--rw-rw-rw-   0        0        0     1069 2024-05-14 17:51:12.000000 extrautilities-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:49:50.341063 extrautilities-0.8/
+drwxrwxrwx   0        0        0        0 2024-05-16 14:49:50.323236 extrautilities-0.8/ExtraUtils/
+-rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-0.8/ExtraUtils/RateLimit.py
+-rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-0.8/ExtraUtils/__init__.py
+-rw-rw-rw-   0        0        0     1766 2024-05-13 18:01:30.000000 extrautilities-0.8/ExtraUtils/asyncTokens.py
+-rw-rw-rw-   0        0        0     3936 2024-05-16 14:48:13.000000 extrautilities-0.8/ExtraUtils/timeBasedToken.py
+-rw-rw-rw-   0        0        0     3307 2024-05-16 14:49:50.340257 extrautilities-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2457 2024-05-16 14:47:20.000000 extrautilities-0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 14:49:50.338747 extrautilities-0.8/extrautilities.egg-info/
+-rw-rw-rw-   0        0        0     3307 2024-05-16 14:49:50.000000 extrautilities-0.8/extrautilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-05-16 14:49:50.000000 extrautilities-0.8/extrautilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 14:49:50.000000 extrautilities-0.8/extrautilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 14:49:50.000000 extrautilities-0.8/extrautilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 14:49:50.000000 extrautilities-0.8/extrautilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 14:49:50.341063 extrautilities-0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-14 19:44:32.000000 extrautilities-0.8/setup.py
```

### Comparing `extrautilities-0.7/ExtraUtils/RateLimit.py` & `extrautilities-0.8/ExtraUtils/RateLimit.py`

 * *Files identical despite different names*

### Comparing `extrautilities-0.7/ExtraUtils/asyncTokens.py` & `extrautilities-0.8/ExtraUtils/asyncTokens.py`

 * *Files identical despite different names*

### Comparing `extrautilities-0.7/PKG-INFO` & `extrautilities-0.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,64 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 0.7
+Version: 0.8
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
-Keywords: RateLimit,asyncTokens
+Keywords: RateLimit,timeBasedToken
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # ExtraUtils
-will provide a bunch of small functionalities to speedup developement.
+will provide a bunch of small functionalities to speedup development.
 
-(In active developement, so if you have any suggestions, to make other developers life easier, feel free to submit them.)
+(In active development, so if you have any suggestions, to make other developers' life easier, feel free to submit them.)
+
+# Latest addition
+
+### TimeBasedToken()
+Generates a time-based token using two keys: a primary and a secondary. Ideal for encrypting traffic between devices or services without sharing the actual tokens.
+
+**How it works:**
+- Utilizes a unified timestamp, rounded to the nearest tenth of a second.
+- Uses the primary token as is.
+- Applies a transformation to the secondary token for added security.
+
+**Example:**
+```py
+primary = "1a2b3c4d5e6f7g8h9i0j1k2l3m4n5o6p"
+secondary = "7q8r9s0t1u2v3w4x5y6z7a8b9c0d1e2f"
+def main():
+    final_token = TimeBasedToken(primary, secondary)
+
+    print(final_token.regenerate())
+    enc = final_token.encrypt("Hello World, i am going to be encrypted and decrypted again. : )")
+    print(enc)
+    dec = final_token.decrypt(enc)
+    print(dec)
+
+if __name__ == "__main__":
+    main()
+```
 
-Currently ExtraUtils only has one feature.
 ### RateLimiter()
+Limits the rate of operations to prevent overloading. Configurable thresholds, decay rates, and behaviors on limit reaching.
+
+**Example**
 ```py
 # A very simplified example
 from ExtraUtils import RateLimiter
 rate_limit = RateLimiter(10,15,5,1,True)
 # threshold (10) -> increments before rate_limit.hit is set to True
 # upperCap (15) -> the highest value the trigger counter will go
 # decay_rate (5) -> the amount in triggers to be decremented each decay cycle
```

### Comparing `extrautilities-0.7/README.md` & `extrautilities-0.8/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,43 @@
 # ExtraUtils
-will provide a bunch of small functionalities to speedup developement.
+will provide a bunch of small functionalities to speedup development.
 
-(In active developement, so if you have any suggestions, to make other developers life easier, feel free to submit them.)
+(In active development, so if you have any suggestions, to make other developers' life easier, feel free to submit them.)
+
+# Latest addition
+
+### TimeBasedToken()
+Generates a time-based token using two keys: a primary and a secondary. Ideal for encrypting traffic between devices or services without sharing the actual tokens.
+
+**How it works:**
+- Utilizes a unified timestamp, rounded to the nearest tenth of a second.
+- Uses the primary token as is.
+- Applies a transformation to the secondary token for added security.
+
+**Example:**
+```py
+primary = "1a2b3c4d5e6f7g8h9i0j1k2l3m4n5o6p"
+secondary = "7q8r9s0t1u2v3w4x5y6z7a8b9c0d1e2f"
+def main():
+    final_token = TimeBasedToken(primary, secondary)
+
+    print(final_token.regenerate())
+    enc = final_token.encrypt("Hello World, i am going to be encrypted and decrypted again. : )")
+    print(enc)
+    dec = final_token.decrypt(enc)
+    print(dec)
+
+if __name__ == "__main__":
+    main()
+```
 
-Currently ExtraUtils only has one feature.
 ### RateLimiter()
+Limits the rate of operations to prevent overloading. Configurable thresholds, decay rates, and behaviors on limit reaching.
+
+**Example**
 ```py
 # A very simplified example
 from ExtraUtils import RateLimiter
 rate_limit = RateLimiter(10,15,5,1,True)
 # threshold (10) -> increments before rate_limit.hit is set to True
 # upperCap (15) -> the highest value the trigger counter will go
 # decay_rate (5) -> the amount in triggers to be decremented each decay cycle
```

### Comparing `extrautilities-0.7/extrautilities.egg-info/PKG-INFO` & `extrautilities-0.8/extrautilities.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,64 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 0.7
+Version: 0.8
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
-Keywords: RateLimit,asyncTokens
+Keywords: RateLimit,timeBasedToken
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # ExtraUtils
-will provide a bunch of small functionalities to speedup developement.
+will provide a bunch of small functionalities to speedup development.
 
-(In active developement, so if you have any suggestions, to make other developers life easier, feel free to submit them.)
+(In active development, so if you have any suggestions, to make other developers' life easier, feel free to submit them.)
+
+# Latest addition
+
+### TimeBasedToken()
+Generates a time-based token using two keys: a primary and a secondary. Ideal for encrypting traffic between devices or services without sharing the actual tokens.
+
+**How it works:**
+- Utilizes a unified timestamp, rounded to the nearest tenth of a second.
+- Uses the primary token as is.
+- Applies a transformation to the secondary token for added security.
+
+**Example:**
+```py
+primary = "1a2b3c4d5e6f7g8h9i0j1k2l3m4n5o6p"
+secondary = "7q8r9s0t1u2v3w4x5y6z7a8b9c0d1e2f"
+def main():
+    final_token = TimeBasedToken(primary, secondary)
+
+    print(final_token.regenerate())
+    enc = final_token.encrypt("Hello World, i am going to be encrypted and decrypted again. : )")
+    print(enc)
+    dec = final_token.decrypt(enc)
+    print(dec)
+
+if __name__ == "__main__":
+    main()
+```
 
-Currently ExtraUtils only has one feature.
 ### RateLimiter()
+Limits the rate of operations to prevent overloading. Configurable thresholds, decay rates, and behaviors on limit reaching.
+
+**Example**
 ```py
 # A very simplified example
 from ExtraUtils import RateLimiter
 rate_limit = RateLimiter(10,15,5,1,True)
 # threshold (10) -> increments before rate_limit.hit is set to True
 # upperCap (15) -> the highest value the trigger counter will go
 # decay_rate (5) -> the amount in triggers to be decremented each decay cycle
```

### Comparing `extrautilities-0.7/setup.py` & `extrautilities-0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='extrautilities',
-    version='0.7',
+    version='0.8',
     packages=find_packages(),
     description='This package provides a few extra utilities for Python, like a "RateLimiter" class.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='Unlicensed',
@@ -18,10 +18,10 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
-    keywords='RateLimit, asyncTokens',
-    install_requires=["extradecorators", "cryptography"],
+    keywords='RateLimit, timeBasedToken',
+    install_requires=["extradecorators", "cryptography","pycryptodome"],
 )
```

