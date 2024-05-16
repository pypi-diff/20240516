# Comparing `tmp/sigstore-3.0.0rc1.tar.gz` & `tmp/sigstore-3.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigstore-3.0.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sigstore-3.0.0rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sigstore-3.0.0rc1.tar` & `sigstore-3.0.0rc2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0    11358 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/LICENSE
--rw-r--r--   0        0        0    18625 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/README.md
--rw-r--r--   0        0        0     3969 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0      958 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/__init__.py
--rw-r--r--   0        0        0      726 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/__main__.py
--rw-r--r--   0        0        0    31481 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_cli.py
--rw-r--r--   0        0        0      738 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/__init__.py
--rw-r--r--   0        0        0      882 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/fulcio/__init__.py
--rw-r--r--   0        0        0    11999 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/fulcio/client.py
--rw-r--r--   0        0        0     4414 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/merkle.py
--rw-r--r--   0        0        0      653 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/oidc/__init__.py
--rw-r--r--   0        0        0    15962 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/oidc/oauth.py
--rw-r--r--   0        0        0     1634 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/rekor/__init__.py
--rw-r--r--   0        0        0     7293 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/rekor/checkpoint.py
--rw-r--r--   0        0        0     8028 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/rekor/client.py
--rw-r--r--   0        0        0     8688 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/sct.py
--rw-r--r--   0        0        0    10909 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/trustroot.py
--rw-r--r--   0        0        0     5819 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/tuf.py
--rw-r--r--   0        0        0     1247 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_store/__init__.py
--rw-r--r--   0        0        0     6388 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_store/prod/root.json
--rw-r--r--   0        0        0     4567 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_store/prod/trusted_root.json
--rw-r--r--   0        0        0     1871 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_store/staging/root.json
--rw-r--r--   0        0        0     7256 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_store/staging/trusted_root.json
--rw-r--r--   0        0        0    11933 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_utils.py
--rw-r--r--   0        0        0     7723 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/dsse.py
--rw-r--r--   0        0        0     3391 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/errors.py
--rw-r--r--   0        0        0     1779 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/hashes.py
--rw-r--r--   0        0        0    18257 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/models.py
--rw-r--r--   0        0        0    15939 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/oidc.py
--rw-r--r--   0        0        0    11866 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/sign.py
--rw-r--r--   0        0        0     1280 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/verify/__init__.py
--rw-r--r--   0        0        0     8755 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/verify/policy.py
--rw-r--r--   0        0        0    13885 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/verify/verifier.py
--rw-r--r--   0        0        0    20876 1970-01-01 00:00:00.000000 sigstore-3.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-07 16:13:23.098981 sigstore-3.0.0rc2/LICENSE
+-rw-r--r--   0        0        0    18625 2024-05-07 16:13:23.098981 sigstore-3.0.0rc2/README.md
+-rw-r--r--   0        0        0     3988 2024-05-07 16:13:23.098981 sigstore-3.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      958 2024-05-07 16:13:23.098981 sigstore-3.0.0rc2/sigstore/__init__.py
+-rw-r--r--   0        0        0      726 2024-05-07 16:13:23.098981 sigstore-3.0.0rc2/sigstore/__main__.py
+-rw-r--r--   0        0        0    31481 2024-05-07 16:13:23.098981 sigstore-3.0.0rc2/sigstore/_cli.py
+-rw-r--r--   0        0        0      738 2024-05-07 16:13:23.098981 sigstore-3.0.0rc2/sigstore/_internal/__init__.py
+-rw-r--r--   0        0        0      882 2024-05-07 16:13:23.098981 sigstore-3.0.0rc2/sigstore/_internal/fulcio/__init__.py
+-rw-r--r--   0        0        0    11999 2024-05-07 16:13:23.098981 sigstore-3.0.0rc2/sigstore/_internal/fulcio/client.py
+-rw-r--r--   0        0        0     4414 2024-05-07 16:13:23.098981 sigstore-3.0.0rc2/sigstore/_internal/merkle.py
+-rw-r--r--   0        0        0      653 2024-05-07 16:13:23.098981 sigstore-3.0.0rc2/sigstore/_internal/oidc/__init__.py
+-rw-r--r--   0        0        0    15962 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/_internal/oidc/oauth.py
+-rw-r--r--   0        0        0     1634 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/_internal/rekor/__init__.py
+-rw-r--r--   0        0        0     7293 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/_internal/rekor/checkpoint.py
+-rw-r--r--   0        0        0     8028 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/_internal/rekor/client.py
+-rw-r--r--   0        0        0     8688 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/_internal/sct.py
+-rw-r--r--   0        0        0    10909 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/_internal/trustroot.py
+-rw-r--r--   0        0        0     5819 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/_internal/tuf.py
+-rw-r--r--   0        0        0     1247 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/_store/__init__.py
+-rw-r--r--   0        0        0     6388 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/_store/prod/root.json
+-rw-r--r--   0        0        0     4567 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/_store/prod/trusted_root.json
+-rw-r--r--   0        0        0     1871 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/_store/staging/root.json
+-rw-r--r--   0        0        0     7256 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/_store/staging/trusted_root.json
+-rw-r--r--   0        0        0    11933 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/_utils.py
+-rw-r--r--   0        0        0     7723 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/dsse.py
+-rw-r--r--   0        0        0     3391 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/errors.py
+-rw-r--r--   0        0        0     1779 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/hashes.py
+-rw-r--r--   0        0        0    18257 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/models.py
+-rw-r--r--   0        0        0    15939 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/oidc.py
+-rw-r--r--   0        0        0        0 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/py.typed
+-rw-r--r--   0        0        0    11866 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/sign.py
+-rw-r--r--   0        0        0     1280 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/verify/__init__.py
+-rw-r--r--   0        0        0    15240 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/verify/policy.py
+-rw-r--r--   0        0        0    13885 2024-05-07 16:13:23.102981 sigstore-3.0.0rc2/sigstore/verify/verifier.py
+-rw-r--r--   0        0        0    20905 1970-01-01 00:00:00.000000 sigstore-3.0.0rc2/PKG-INFO
```

### Comparing `sigstore-3.0.0rc1/LICENSE` & `sigstore-3.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/README.md` & `sigstore-3.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/pyproject.toml` & `sigstore-3.0.0rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   "Topic :: Security",
   "Topic :: Security :: Cryptography",
 ]
 dependencies = [
   "cryptography >= 42",
   "id >= 1.1.0",
   "importlib_resources ~= 5.7; python_version < '3.11'",
+  "pyasn1 ~= 0.6",
   "pydantic >= 2,< 3",
   "pyjwt >= 2.1",
   "pyOpenSSL >= 23.0.0",
   "requests",
   "rich ~= 13.0",
   "rfc8785 ~= 0.1.2",
   "sigstore-protobuf-specs ~= 0.3.1",
@@ -58,15 +59,15 @@
   # HACK(ww): interrogate needs setuptools to provide `pkg_resources` on Python 3.12+;
   # remove this when https://github.com/econchick/interrogate/issues/164 is resolved.
   "setuptools",
   "interrogate",
   "mypy ~= 1.1",
   # NOTE(ww): ruff is under active development, so we pin conservatively here
   # and let Dependabot periodically perform this update.
-  "ruff < 0.4.3",
+  "ruff < 0.4.4",
   "types-requests",
   "types-pyOpenSSL",
 ]
 doc = ["pdoc"]
 dev = ["build", "bump >= 1.3.2", "sigstore[doc,test,lint]"]
 
 [tool.coverage.run]
```

### Comparing `sigstore-3.0.0rc1/sigstore/__init__.py` & `sigstore-3.0.0rc2/sigstore/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 Otherwise, here are some quick starting points:
 
 * `sigstore.verify`: verifying of Sigstore signatures,
   including flexible policy control
 * `sigstore.sign`: creation of Sigstore signatures
 """
 
-__version__ = "3.0.0rc1"
+__version__ = "3.0.0rc2"
```

### Comparing `sigstore-3.0.0rc1/sigstore/__main__.py` & `sigstore-3.0.0rc2/sigstore/__main__.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_cli.py` & `sigstore-3.0.0rc2/sigstore/_cli.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_internal/__init__.py` & `sigstore-3.0.0rc2/sigstore/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_internal/fulcio/__init__.py` & `sigstore-3.0.0rc2/sigstore/_internal/fulcio/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_internal/fulcio/client.py` & `sigstore-3.0.0rc2/sigstore/_internal/fulcio/client.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_internal/merkle.py` & `sigstore-3.0.0rc2/sigstore/_internal/merkle.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_internal/oidc/__init__.py` & `sigstore-3.0.0rc2/sigstore/_internal/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_internal/oidc/oauth.py` & `sigstore-3.0.0rc2/sigstore/_internal/oidc/oauth.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_internal/rekor/__init__.py` & `sigstore-3.0.0rc2/sigstore/_internal/rekor/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_internal/rekor/checkpoint.py` & `sigstore-3.0.0rc2/sigstore/_internal/rekor/checkpoint.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_internal/rekor/client.py` & `sigstore-3.0.0rc2/sigstore/_internal/rekor/client.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_internal/sct.py` & `sigstore-3.0.0rc2/sigstore/_internal/sct.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_internal/trustroot.py` & `sigstore-3.0.0rc2/sigstore/_internal/trustroot.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_internal/tuf.py` & `sigstore-3.0.0rc2/sigstore/_internal/tuf.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_store/__init__.py` & `sigstore-3.0.0rc2/sigstore/_store/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_store/prod/root.json` & `sigstore-3.0.0rc2/sigstore/_store/prod/root.json`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_store/prod/trusted_root.json` & `sigstore-3.0.0rc2/sigstore/_store/prod/trusted_root.json`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_store/staging/root.json` & `sigstore-3.0.0rc2/sigstore/_store/staging/root.json`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_store/staging/trusted_root.json` & `sigstore-3.0.0rc2/sigstore/_store/staging/trusted_root.json`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/_utils.py` & `sigstore-3.0.0rc2/sigstore/_utils.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/dsse.py` & `sigstore-3.0.0rc2/sigstore/dsse.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/errors.py` & `sigstore-3.0.0rc2/sigstore/errors.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/hashes.py` & `sigstore-3.0.0rc2/sigstore/hashes.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/models.py` & `sigstore-3.0.0rc2/sigstore/models.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/oidc.py` & `sigstore-3.0.0rc2/sigstore/oidc.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/sign.py` & `sigstore-3.0.0rc2/sigstore/sign.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/verify/__init__.py` & `sigstore-3.0.0rc2/sigstore/verify/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/sigstore/verify/verifier.py` & `sigstore-3.0.0rc2/sigstore/verify/verifier.py`

 * *Files identical despite different names*

### Comparing `sigstore-3.0.0rc1/PKG-INFO` & `sigstore-3.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigstore
-Version: 3.0.0rc1
+Version: 3.0.0rc2
 Summary: A tool for signing Python package distributions
 Author-email: Sigstore Authors <sigstore-dev@googlegroups.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Requires-Dist: cryptography >= 42
 Requires-Dist: id >= 1.1.0
 Requires-Dist: importlib_resources ~= 5.7; python_version < '3.11'
+Requires-Dist: pyasn1 ~= 0.6
 Requires-Dist: pydantic >= 2,< 3
 Requires-Dist: pyjwt >= 2.1
 Requires-Dist: pyOpenSSL >= 23.0.0
 Requires-Dist: requests
 Requires-Dist: rich ~= 13.0
 Requires-Dist: rfc8785 ~= 0.1.2
 Requires-Dist: sigstore-protobuf-specs ~= 0.3.1
@@ -33,15 +34,15 @@
 Requires-Dist: bump >= 1.3.2 ; extra == "dev"
 Requires-Dist: sigstore[doc,test,lint] ; extra == "dev"
 Requires-Dist: pdoc ; extra == "doc"
 Requires-Dist: bandit ; extra == "lint"
 Requires-Dist: setuptools ; extra == "lint"
 Requires-Dist: interrogate ; extra == "lint"
 Requires-Dist: mypy ~= 1.1 ; extra == "lint"
-Requires-Dist: ruff < 0.4.3 ; extra == "lint"
+Requires-Dist: ruff < 0.4.4 ; extra == "lint"
 Requires-Dist: types-requests ; extra == "lint"
 Requires-Dist: types-pyOpenSSL ; extra == "lint"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pretend ; extra == "test"
 Requires-Dist: coverage[toml] ; extra == "test"
 Project-URL: Documentation, https://sigstore.github.io/sigstore-python/
```

