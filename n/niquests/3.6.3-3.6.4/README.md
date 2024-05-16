# Comparing `tmp/niquests-3.6.3.tar.gz` & `tmp/niquests-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon May  6 07:01:50 2024, max compression
+gzip compressed data, last modified: Thu May 16 05:51:35 2024, max compression
```

## Comparing `niquests-3.6.3.tar` & `niquests-3.6.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      718 2024-05-06 07:01:50.000000 niquests-3.6.3/AUTHORS.rst
--rw-r--r--   0        0        0    86599 2024-05-06 07:01:50.000000 niquests-3.6.3/HISTORY.md
--rw-r--r--   0        0        0      377 2024-05-06 07:01:50.000000 niquests-3.6.3/Makefile
--rw-r--r--   0        0        0       38 2024-05-06 07:01:50.000000 niquests-3.6.3/NOTICE
--rw-r--r--   0        0        0      201 2024-05-06 07:01:50.000000 niquests-3.6.3/SECURITY.md
--rw-r--r--   0        0        0      233 2024-05-06 07:01:50.000000 niquests-3.6.3/requirements-dev.txt
--rw-r--r--   0        0        0        1 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/.nojekyll
--rw-r--r--   0        0        0     7664 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/Makefile
--rw-r--r--   0        0        0     5355 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/api.rst
--rw-r--r--   0        0        0    12305 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/conf.py
--rw-r--r--   0        0        0     4084 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/index.rst
--rw-r--r--   0        0        0     7253 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/make.bat
--rw-r--r--   0        0        0      185 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/requirements.txt
--rw-r--r--   0        0        0     2990 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/_static/custom.css
--rw-r--r--   0        0        0   306086 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/_static/requests-sidebar.png
--rw-r--r--   0        0        0     7360 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/community/faq.rst
--rw-r--r--   0        0        0     2720 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/community/recommended.rst
--rw-r--r--   0        0        0     1782 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/community/release-process.rst
--rw-r--r--   0        0        0      285 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/community/support.rst
--rw-r--r--   0        0        0      324 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/community/updates.rst
--rw-r--r--   0        0        0      945 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/community/vulnerabilities.rst
--rw-r--r--   0        0        0       48 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/dev/authors.rst
--rw-r--r--   0        0        0     5768 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/dev/contributing.rst
--rw-r--r--   0        0        0     1885 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/dev/migrate.rst
--rw-r--r--   0        0        0    52818 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/user/advanced.rst
--rw-r--r--   0        0        0     6315 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/user/authentication.rst
--rw-r--r--   0        0        0     1046 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/user/install.rst
--rw-r--r--   0        0        0    34594 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/user/quickstart.rst
--rw-r--r--   0        0        0     3071 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/__init__.py
--rw-r--r--   0        0        0      534 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/__version__.py
--rw-r--r--   0        0        0    47120 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/_async.py
--rw-r--r--   0        0        0     2852 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/_compat.py
--rw-r--r--   0        0        0      480 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/_constant.py
--rw-r--r--   0        0        0     5942 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/_typing.py
--rw-r--r--   0        0        0    86896 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/adapters.py
--rw-r--r--   0        0        0    27567 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/api.py
--rw-r--r--   0        0        0     9906 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/auth.py
--rw-r--r--   0        0        0    19872 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/cookies.py
--rw-r--r--   0        0        0     4363 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/exceptions.py
--rw-r--r--   0        0        0     5248 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/help.py
--rw-r--r--   0        0        0     2776 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/hooks.py
--rw-r--r--   0        0        0    62733 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/models.py
--rw-r--r--   0        0        0        0 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/py.typed
--rw-r--r--   0        0        0    69084 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/sessions.py
--rw-r--r--   0        0        0     4284 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/status_codes.py
--rw-r--r--   0        0        0     6973 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/structures.py
--rw-r--r--   0        0        0    37300 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/utils.py
--rw-r--r--   0        0        0      119 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/extensions/__init__.py
--rw-r--r--   0        0        0    22348 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/extensions/_async_ocsp.py
--rw-r--r--   0        0        0    21009 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/extensions/_ocsp.py
--rw-r--r--   0        0        0    16942 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/extensions/_picotls.py
--rw-r--r--   0        0        0       80 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/__init__.py
--rw-r--r--   0        0        0     2193 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/conftest.py
--rw-r--r--   0        0        0     7540 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_async.py
--rw-r--r--   0        0        0      875 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_help.py
--rw-r--r--   0        0        0      893 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_hooks.py
--rw-r--r--   0        0        0     4022 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_live.py
--rw-r--r--   0        0        0    15985 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_lowlevel.py
--rw-r--r--   0        0        0     3722 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_multiplexed.py
--rw-r--r--   0        0        0    99906 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_requests.py
--rw-r--r--   0        0        0     2725 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_structures.py
--rw-r--r--   0        0        0     6213 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_testserver.py
--rw-r--r--   0        0        0    26728 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_utils.py
--rw-r--r--   0        0        0      613 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/utils.py
--rw-r--r--   0        0        0        0 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/testserver/__init__.py
--rw-r--r--   0        0        0     3882 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/testserver/server.py
--rw-r--r--   0        0        0      362 2024-05-06 07:01:50.000000 niquests-3.6.3/.gitignore
--rw-r--r--   0        0        0    10142 2024-05-06 07:01:50.000000 niquests-3.6.3/LICENSE
--rw-r--r--   0        0        0    10884 2024-05-06 07:01:50.000000 niquests-3.6.3/README.md
--rw-r--r--   0        0        0     3662 2024-05-06 07:01:50.000000 niquests-3.6.3/pyproject.toml
--rw-r--r--   0        0        0    13245 2024-05-06 07:01:50.000000 niquests-3.6.3/PKG-INFO
+-rw-r--r--   0        0        0      718 2024-05-16 05:51:35.000000 niquests-3.6.4/AUTHORS.rst
+-rw-r--r--   0        0        0    86817 2024-05-16 05:51:35.000000 niquests-3.6.4/HISTORY.md
+-rw-r--r--   0        0        0      377 2024-05-16 05:51:35.000000 niquests-3.6.4/Makefile
+-rw-r--r--   0        0        0       38 2024-05-16 05:51:35.000000 niquests-3.6.4/NOTICE
+-rw-r--r--   0        0        0      201 2024-05-16 05:51:35.000000 niquests-3.6.4/SECURITY.md
+-rw-r--r--   0        0        0      233 2024-05-16 05:51:35.000000 niquests-3.6.4/requirements-dev.txt
+-rw-r--r--   0        0        0        1 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/.nojekyll
+-rw-r--r--   0        0        0     7664 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/Makefile
+-rw-r--r--   0        0        0     5355 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/api.rst
+-rw-r--r--   0        0        0    12305 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/conf.py
+-rw-r--r--   0        0        0     4084 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/index.rst
+-rw-r--r--   0        0        0     7253 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/make.bat
+-rw-r--r--   0        0        0      185 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/requirements.txt
+-rw-r--r--   0        0        0     2990 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/_static/custom.css
+-rw-r--r--   0        0        0   306086 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/_static/requests-sidebar.png
+-rw-r--r--   0        0        0     7360 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/community/faq.rst
+-rw-r--r--   0        0        0     2720 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/community/recommended.rst
+-rw-r--r--   0        0        0     1782 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/community/release-process.rst
+-rw-r--r--   0        0        0      285 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/community/support.rst
+-rw-r--r--   0        0        0      324 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/community/updates.rst
+-rw-r--r--   0        0        0      945 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/community/vulnerabilities.rst
+-rw-r--r--   0        0        0       48 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/dev/authors.rst
+-rw-r--r--   0        0        0     5768 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/dev/contributing.rst
+-rw-r--r--   0        0        0     1885 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/dev/migrate.rst
+-rw-r--r--   0        0        0    52818 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/user/advanced.rst
+-rw-r--r--   0        0        0     6315 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/user/authentication.rst
+-rw-r--r--   0        0        0     1046 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/user/install.rst
+-rw-r--r--   0        0        0    34594 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/user/quickstart.rst
+-rw-r--r--   0        0        0     3071 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/__init__.py
+-rw-r--r--   0        0        0      534 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/__version__.py
+-rw-r--r--   0        0        0    47120 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/_async.py
+-rw-r--r--   0        0        0     2852 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/_compat.py
+-rw-r--r--   0        0        0      480 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/_constant.py
+-rw-r--r--   0        0        0     5942 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/_typing.py
+-rw-r--r--   0        0        0    86896 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/adapters.py
+-rw-r--r--   0        0        0    27567 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/api.py
+-rw-r--r--   0        0        0     9906 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/auth.py
+-rw-r--r--   0        0        0    19872 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/cookies.py
+-rw-r--r--   0        0        0     4363 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/exceptions.py
+-rw-r--r--   0        0        0     5248 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/help.py
+-rw-r--r--   0        0        0     2776 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/hooks.py
+-rw-r--r--   0        0        0    62733 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/models.py
+-rw-r--r--   0        0        0        0 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/py.typed
+-rw-r--r--   0        0        0    69360 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/sessions.py
+-rw-r--r--   0        0        0     4284 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/status_codes.py
+-rw-r--r--   0        0        0     7042 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/structures.py
+-rw-r--r--   0        0        0    37300 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/utils.py
+-rw-r--r--   0        0        0      119 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/extensions/__init__.py
+-rw-r--r--   0        0        0    22400 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/extensions/_async_ocsp.py
+-rw-r--r--   0        0        0    21160 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/extensions/_ocsp.py
+-rw-r--r--   0        0        0    16942 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/extensions/_picotls.py
+-rw-r--r--   0        0        0       80 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/__init__.py
+-rw-r--r--   0        0        0     2193 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/conftest.py
+-rw-r--r--   0        0        0     7540 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_async.py
+-rw-r--r--   0        0        0      875 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_help.py
+-rw-r--r--   0        0        0      893 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_hooks.py
+-rw-r--r--   0        0        0     4022 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_live.py
+-rw-r--r--   0        0        0    15985 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_lowlevel.py
+-rw-r--r--   0        0        0     3722 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_multiplexed.py
+-rw-r--r--   0        0        0    99906 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_requests.py
+-rw-r--r--   0        0        0     2725 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_structures.py
+-rw-r--r--   0        0        0     6213 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_testserver.py
+-rw-r--r--   0        0        0    26728 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_utils.py
+-rw-r--r--   0        0        0      613 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/utils.py
+-rw-r--r--   0        0        0        0 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/testserver/__init__.py
+-rw-r--r--   0        0        0     3882 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/testserver/server.py
+-rw-r--r--   0        0        0      362 2024-05-16 05:51:35.000000 niquests-3.6.4/.gitignore
+-rw-r--r--   0        0        0    10142 2024-05-16 05:51:35.000000 niquests-3.6.4/LICENSE
+-rw-r--r--   0        0        0    10884 2024-05-16 05:51:35.000000 niquests-3.6.4/README.md
+-rw-r--r--   0        0        0     3660 2024-05-16 05:51:35.000000 niquests-3.6.4/pyproject.toml
+-rw-r--r--   0        0        0    13243 2024-05-16 05:51:35.000000 niquests-3.6.4/PKG-INFO
```

### Comparing `niquests-3.6.3/AUTHORS.rst` & `niquests-3.6.4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/HISTORY.md` & `niquests-3.6.4/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Release History
 ===============
 
+3.6.4 (2024-05-16)
+------------------
+
+**Changed**
+- Avoid parsing X509 peer certificate in the certificate revocation check process over and over again.
+- Avoid iterating over header items redundantly or needlessly.
+
 3.6.3 (2024-05-06)
 ------------------
 
 **Fixed**
 - Fixed encoding data with None values and other objects. This was a regression introduced in our v3. #119
 
 **Changed**
```

### Comparing `niquests-3.6.3/docs/Makefile` & `niquests-3.6.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/docs/api.rst` & `niquests-3.6.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/docs/conf.py` & `niquests-3.6.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/docs/index.rst` & `niquests-3.6.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/docs/make.bat` & `niquests-3.6.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/docs/_static/custom.css` & `niquests-3.6.4/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/docs/_static/requests-sidebar.png` & `niquests-3.6.4/docs/_static/requests-sidebar.png`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/docs/community/faq.rst` & `niquests-3.6.4/docs/community/faq.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/docs/community/recommended.rst` & `niquests-3.6.4/docs/community/recommended.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/docs/community/release-process.rst` & `niquests-3.6.4/docs/community/release-process.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/docs/community/vulnerabilities.rst` & `niquests-3.6.4/docs/community/vulnerabilities.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/docs/dev/contributing.rst` & `niquests-3.6.4/docs/dev/contributing.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/docs/dev/migrate.rst` & `niquests-3.6.4/docs/dev/migrate.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/docs/user/advanced.rst` & `niquests-3.6.4/docs/user/advanced.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/docs/user/authentication.rst` & `niquests-3.6.4/docs/user/authentication.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/docs/user/install.rst` & `niquests-3.6.4/docs/user/install.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/docs/user/quickstart.rst` & `niquests-3.6.4/docs/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/src/niquests/__init__.py` & `niquests-3.6.4/src/niquests/__init__.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/src/niquests/__version__.py` & `niquests-3.6.4/src/niquests/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 __title__: str = "niquests"
 __description__: str = "Python HTTP for Humans."
 __url__: str = "https://niquests.readthedocs.io"
 
 __version__: str
-__version__ = "3.6.3"
+__version__ = "3.6.4"
 
-__build__: int = 0x030603
+__build__: int = 0x030604
 __author__: str = "Kenneth Reitz"
 __author_email__: str = "me@kennethreitz.org"
 __license__: str = "Apache-2.0"
 __copyright__: str = "Copyright Kenneth Reitz"
 __cake__: str = "\u2728 \U0001f370 \u2728"
```

### Comparing `niquests-3.6.3/src/niquests/_async.py` & `niquests-3.6.4/src/niquests/_async.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/src/niquests/_compat.py` & `niquests-3.6.4/src/niquests/_compat.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/src/niquests/_typing.py` & `niquests-3.6.4/src/niquests/_typing.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/src/niquests/adapters.py` & `niquests-3.6.4/src/niquests/adapters.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/src/niquests/api.py` & `niquests-3.6.4/src/niquests/api.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/src/niquests/auth.py` & `niquests-3.6.4/src/niquests/auth.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/src/niquests/cookies.py` & `niquests-3.6.4/src/niquests/cookies.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/src/niquests/exceptions.py` & `niquests-3.6.4/src/niquests/exceptions.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/src/niquests/help.py` & `niquests-3.6.4/src/niquests/help.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/src/niquests/hooks.py` & `niquests-3.6.4/src/niquests/hooks.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/src/niquests/models.py` & `niquests-3.6.4/src/niquests/models.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/src/niquests/sessions.py` & `niquests-3.6.4/src/niquests/sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,25 +124,34 @@
     if session_setting is None:
         return request_setting
 
     if request_setting is None:
         return session_setting
 
     # Bypass if not a dictionary (e.g. verify)
-    if not (
+    if isinstance(session_setting, bool) or not (
         isinstance(session_setting, Mapping) and isinstance(request_setting, Mapping)
     ):
         return request_setting
 
-    merged_setting = dict_class(to_key_val_list(session_setting))
+    if hasattr(session_setting, "copy"):
+        merged_setting = (
+            session_setting.copy()
+            if session_setting.__class__ is dict_class
+            else dict_class(session_setting.copy())
+        )
+    else:
+        merged_setting = dict_class(to_key_val_list(session_setting))
+
     merged_setting.update(to_key_val_list(request_setting))
 
     # Remove keys that are set to None. Extract keys first to avoid altering
     # the dictionary during iteration.
-    none_keys = [k for (k, v) in merged_setting.items() if v is None]
+    none_keys = [k for k in merged_setting if merged_setting[k] is None]
+
     for key in none_keys:
         del merged_setting[key]
 
     return merged_setting
 
 
 def merge_hooks(
```

### Comparing `niquests-3.6.3/src/niquests/status_codes.py` & `niquests-3.6.4/src/niquests/status_codes.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/src/niquests/structures.py` & `niquests-3.6.4/src/niquests/structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,25 +122,29 @@
     def __len__(self) -> int:
         return len(self._store)
 
     def lower_items(self) -> typing.Iterator[tuple[bytes | str, bytes | str]]:
         """Like iteritems(), but with all lowercase keys."""
         return ((lowerkey, keyval[1]) for (lowerkey, keyval) in self._store.items())
 
+    def items(self):
+        for k in self._store:
+            yield self._store[k]
+
     def __eq__(self, other) -> bool:
         if isinstance(other, Mapping):
             other = CaseInsensitiveDict(other)
         else:
             return NotImplemented
         # Compare insensitively
         return dict(self.lower_items()) == dict(other.lower_items())
 
     # Copy is required
     def copy(self) -> CaseInsensitiveDict:
-        return CaseInsensitiveDict(self._store.values())
+        return CaseInsensitiveDict(self)
 
     def __repr__(self) -> str:
         return str(dict(self.items()))
 
     def __contains__(self, item: str) -> bool:  # type: ignore[override]
         return _lower_wrapper(item) in self._store
```

### Comparing `niquests-3.6.3/src/niquests/utils.py` & `niquests-3.6.4/src/niquests/utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/src/niquests/extensions/_async_ocsp.py` & `niquests-3.6.4/src/niquests/extensions/_async_ocsp.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,19 @@
     handle_server_hello,
     multiply_num_on_ec_point,
     num_to_bytes,
     async_recv_tls,
     async_recv_tls_and_decrypt,
     async_send_tls,
 )
-from ._ocsp import _str_fingerprint_of, readable_revocation_reason
+from ._ocsp import (
+    _str_fingerprint_of,
+    readable_revocation_reason,
+    _parse_x509_der_cached,
+)
 
 
 async def _ask_nicely_for_issuer(
     hostname: str, dst_address: tuple[str, int], timeout: int | float = 0.2
 ) -> Certificate | None:
     """When encountering a problem in development, one should always say that there is many solutions.
     From dirtiest to the cleanest, not always known but with progressive effort, we'll eventually land at the cleanest.
@@ -316,15 +320,15 @@
         if ep.startswith("http://")  # type: ignore
     ]
 
     # well... not all issued certificate have a OCSP entry. e.g. mkcert.
     if not endpoints:
         return
 
-    peer_certificate = Certificate(conn_info.certificate_der)
+    peer_certificate = _parse_x509_der_cached(conn_info.certificate_der)
 
     async with _SharedRevocationStatusCache.lock(peer_certificate):
         # this feature, by default, is reserved for a reasonable usage.
         if not strict:
             mean_rate_sec = _SharedRevocationStatusCache.rate()
             cache_count = len(_SharedRevocationStatusCache)
```

### Comparing `niquests-3.6.3/src/niquests/extensions/_ocsp.py` & `niquests-3.6.4/src/niquests/extensions/_ocsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import socket
 import ssl
 import threading
 import warnings
 from hashlib import sha256
 from random import randint
 from statistics import mean
+from functools import lru_cache
 
 from qh3._hazmat import (
     OCSPRequest,
     OCSPResponse,
     OCSPResponseStatus,
     OCSPCertStatus,
     Certificate,
@@ -48,14 +49,19 @@
     num_to_bytes,
     recv_tls,
     recv_tls_and_decrypt,
     send_tls,
 )
 
 
+@lru_cache(maxsize=64)
+def _parse_x509_der_cached(der: bytes) -> Certificate:
+    return Certificate(der)
+
+
 def _str_fingerprint_of(certificate: Certificate) -> str:
     return ":".join(
         [format(i, "02x") for i in sha256(certificate.public_bytes()).digest()]
     )
 
 
 def readable_revocation_reason(flag: ReasonFlags | None) -> str | None:
@@ -323,15 +329,15 @@
 
         if cache_count >= 10 and mean_rate_sec <= 1.0:
             _SharedRevocationStatusCache.hold = True
 
         if _SharedRevocationStatusCache.hold:
             return
 
-    peer_certificate = Certificate(conn_info.certificate_der)
+    peer_certificate = _parse_x509_der_cached(conn_info.certificate_der)
     cached_response = _SharedRevocationStatusCache.check(peer_certificate)
 
     if cached_response is not None:
         issuer_certificate = _SharedRevocationStatusCache.get_issuer_of(
             peer_certificate
         )
```

### Comparing `niquests-3.6.3/src/niquests/extensions/_picotls.py` & `niquests-3.6.4/src/niquests/extensions/_picotls.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/tests/conftest.py` & `niquests-3.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/tests/test_async.py` & `niquests-3.6.4/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/tests/test_help.py` & `niquests-3.6.4/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/tests/test_hooks.py` & `niquests-3.6.4/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/tests/test_live.py` & `niquests-3.6.4/tests/test_live.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/tests/test_lowlevel.py` & `niquests-3.6.4/tests/test_lowlevel.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/tests/test_multiplexed.py` & `niquests-3.6.4/tests/test_multiplexed.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/tests/test_requests.py` & `niquests-3.6.4/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/tests/test_structures.py` & `niquests-3.6.4/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/tests/test_testserver.py` & `niquests-3.6.4/tests/test_testserver.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/tests/test_utils.py` & `niquests-3.6.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/tests/utils.py` & `niquests-3.6.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/tests/testserver/server.py` & `niquests-3.6.4/tests/testserver/server.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/LICENSE` & `niquests-3.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/README.md` & `niquests-3.6.4/README.md`

 * *Files identical despite different names*

### Comparing `niquests-3.6.3/pyproject.toml` & `niquests-3.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "niquests"
 description = "Niquests is a simple, yet elegant, HTTP library. It is a drop-in replacement for Requests, which is under feature freeze."
 readme = "README.md"
 license-files = { paths = ["LICENSE"] }
 license = "Apache-2.0"
-keywords = ["requests", "http/2", "http/3", "QUIC", "http", "https", "http client", "http/1.1", "ocsp", "revocation", "tls", "multiplexed", "dns-over-quic", "doq", "dns-over-tls", "dot", "dns-over-https", "doh", "dnssec"]
+keywords = ["requests", "http2", "http3", "QUIC", "http", "https", "http client", "http/1.1", "ocsp", "revocation", "tls", "multiplexed", "dns-over-quic", "doq", "dns-over-tls", "dot", "dns-over-https", "doh", "dnssec"]
 authors = [
   {name = "Kenneth Reitz", email = "me@kennethreitz.org"}
 ]
 maintainers = [
   {name = "Ahmed R. TAHRI", email="ahmed.tahri@cloudnursery.dev"},
 ]
 classifiers = [
```

### Comparing `niquests-3.6.3/PKG-INFO` & `niquests-3.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.3
 Name: niquests
-Version: 3.6.3
+Version: 3.6.4
 Summary: Niquests is a simple, yet elegant, HTTP library. It is a drop-in replacement for Requests, which is under feature freeze.
 Project-URL: Changelog, https://github.com/jawah/niquests/blob/main/HISTORY.md
 Project-URL: Documentation, https://niquests.readthedocs.io
 Project-URL: Code, https://github.com/jawah/niquests
 Project-URL: Issue tracker, https://github.com/jawah/niquests/issues
 Author-email: Kenneth Reitz <me@kennethreitz.org>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
 License-Expression: Apache-2.0
 License-File: LICENSE
-Keywords: QUIC,dns-over-https,dns-over-quic,dns-over-tls,dnssec,doh,doq,dot,http,http client,http/1.1,http/2,http/3,https,multiplexed,ocsp,requests,revocation,tls
+Keywords: QUIC,dns-over-https,dns-over-quic,dns-over-tls,dnssec,doh,doq,dot,http,http client,http/1.1,http2,http3,https,multiplexed,ocsp,requests,revocation,tls
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

