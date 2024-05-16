# Comparing `tmp/astrosampler-0.1.0.tar.gz` & `tmp/astrosampler-0.2.0.tar.gz`

## Comparing `astrosampler-0.1.0.tar` & `astrosampler-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 astrosampler-0.1.0/requirements.txt
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 astrosampler-0.1.0/.github/workflows/pr-testing.yml
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 astrosampler-0.1.0/.github/workflows/pr-validation.yml
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 astrosampler-0.1.0/.github/workflows/test-and-release.yml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 astrosampler-0.1.0/astrosampler/__init__.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 astrosampler-0.1.0/astrosampler/sampler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrosampler-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 astrosampler-0.1.0/tests/sampler_test.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 astrosampler-0.1.0/.gitignore
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 astrosampler-0.1.0/LICENSE
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 astrosampler-0.1.0/README.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 astrosampler-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 astrosampler-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 astrosampler-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 astrosampler-0.2.0/.github/workflows/pr-testing.yml
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 astrosampler-0.2.0/.github/workflows/pr-validation.yml
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 astrosampler-0.2.0/.github/workflows/test-and-release.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 astrosampler-0.2.0/astrosampler/__init__.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 astrosampler-0.2.0/astrosampler/imf.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 astrosampler-0.2.0/astrosampler/sampler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrosampler-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 astrosampler-0.2.0/tests/imf_test.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 astrosampler-0.2.0/tests/sampler_test.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 astrosampler-0.2.0/.gitignore
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 astrosampler-0.2.0/LICENSE
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 astrosampler-0.2.0/README.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 astrosampler-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 astrosampler-0.2.0/PKG-INFO
```

### Comparing `astrosampler-0.1.0/.github/workflows/test-and-release.yml` & `astrosampler-0.2.0/.github/workflows/test-and-release.yml`

 * *Files identical despite different names*

### Comparing `astrosampler-0.1.0/astrosampler/sampler.py` & `astrosampler-0.2.0/astrosampler/sampler.py`

 * *Files identical despite different names*

### Comparing `astrosampler-0.1.0/LICENSE` & `astrosampler-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astrosampler-0.1.0/pyproject.toml` & `astrosampler-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name="astrosampler"
-version="0.1.0"
+version="0.2.0"
 authors = [
     { name="Matthew Whitaker", email="sub6resources@gmail.com" },
 ]
 dependencies = [
     "numpy",
 ]
 description="A package for sampling typical distributions in astronomy"
```

