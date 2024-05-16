# Comparing `tmp/dyff_schema-0.5.3.tar.gz` & `tmp/dyff_schema-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_schema-0.5.3.tar", last modified: Fri May 10 22:00:25 2024, max compression
+gzip compressed data, was "dyff_schema-0.6.0.tar", last modified: Thu May 16 21:19:53 2024, max compression
```

## Comparing `dyff_schema-0.5.3.tar` & `dyff_schema-0.6.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:00:25.073479 dyff_schema-0.5.3/
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1398 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1686 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3458 2024-05-10 22:00:25.073479 dyff_schema-0.5.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2312 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:00:25.059479 dyff_schema-0.5.3/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:00:25.065479 dyff_schema-0.5.3/dyff/schema/
--rw-rw-rw-   0 root         (0) root         (0)     1031 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/copydoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:00:25.066479 dyff_schema-0.5.3/dyff/schema/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/dataset/vision.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/ids.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:00:25.067479 dyff_schema-0.5.3/dyff/schema/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/platform.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     3788 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/quantity.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/requests.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:00:25.067479 dyff_schema-0.5.3/dyff/schema/v0/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/v0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:00:25.069479 dyff_schema-0.5.3/dyff/schema/v0/r1/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/v0/r1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23552 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/v0/r1/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)    17139 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/v0/r1/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:00:25.070479 dyff_schema-0.5.3/dyff/schema/v0/r1/dataset/
--rw-rw-rw-   0 root         (0) root         (0)     2553 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/v0/r1/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12312 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/v0/r1/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/v0/r1/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/v0/r1/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/v0/r1/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/v0/r1/dataset/vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:00:25.071479 dyff_schema-0.5.3/dyff/schema/v0/r1/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/v0/r1/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5320 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/v0/r1/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)    59933 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/v0/r1/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     7814 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/v0/r1/requests.py
--rw-rw-rw-   0 root         (0) root         (0)    10720 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/v0/r1/test.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/v0/r1/version.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/dyff/schema/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:00:25.072479 dyff_schema-0.5.3/dyff_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3458 2024-05-10 22:00:25.000000 dyff_schema-0.5.3/dyff_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1358 2024-05-10 22:00:25.000000 dyff_schema-0.5.3/dyff_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 22:00:25.000000 dyff_schema-0.5.3/dyff_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-05-10 22:00:25.000000 dyff_schema-0.5.3/dyff_schema.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-10 22:00:25.000000 dyff_schema-0.5.3/dyff_schema.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 22:00:25.073479 dyff_schema-0.5.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:00:25.072479 dyff_schema-0.5.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1449 2024-05-10 22:00:19.000000 dyff_schema-0.5.3/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.901949 dyff_schema-0.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-05-16 21:19:53.901949 dyff_schema-0.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.886949 dyff_schema-0.6.0/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.893949 dyff_schema-0.6.0/dyff/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/copydoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.894949 dyff_schema-0.6.0/dyff/schema/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/dataset/vision.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/ids.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.895949 dyff_schema-0.6.0/dyff/schema/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/quantity.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.895949 dyff_schema-0.6.0/dyff/schema/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.897949 dyff_schema-0.6.0/dyff/schema/v0/r1/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23552 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)    17139 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.898949 dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12312 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.898949 dyff_schema-0.6.0/dyff/schema/v0/r1/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)    60712 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     8490 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    10720 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.900949 dyff_schema-0.6.0/dyff_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-05-16 21:19:53.000000 dyff_schema-0.6.0/dyff_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-05-16 21:19:53.000000 dyff_schema-0.6.0/dyff_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 21:19:53.000000 dyff_schema-0.6.0/dyff_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-16 21:19:53.000000 dyff_schema-0.6.0/dyff_schema.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-16 21:19:53.000000 dyff_schema-0.6.0/dyff_schema.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 21:19:53.901949 dyff_schema-0.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.900949 dyff_schema-0.6.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/tests/test_import.py
```

### Comparing `dyff_schema-0.5.3/.gitlab-ci.yml` & `dyff_schema-0.6.0/.gitlab-ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     file:
       - detect-secrets.yml
   - project: buildgarden/pipelines/prettier
     ref: 0.3.2
     file:
       - prettier.yml
   - project: buildgarden/pipelines/python
-    ref: 0.9.1
+    ref: 0.10.0
     file:
       - python-autoflake.yml
       - python-black.yml
       - python-build-sdist.yml
       - python-build-wheel.yml
       - python-isort.yml
       - python-mypy.yml
```

### Comparing `dyff_schema-0.5.3/.pre-commit-config.yaml` & `dyff_schema-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/.secrets.baseline` & `dyff_schema-0.6.0/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/CODE_OF_CONDUCT.md` & `dyff_schema-0.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/LICENSE` & `dyff_schema-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/PKG-INFO` & `dyff_schema-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.5.3
+Version: 0.6.0
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_schema-0.5.3/README.md` & `dyff_schema-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/dyff/schema/__init__.py` & `dyff_schema-0.6.0/dyff/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/dyff/schema/copydoc.py` & `dyff_schema-0.6.0/dyff/schema/copydoc.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/dyff/schema/ids.py` & `dyff_schema-0.6.0/dyff/schema/ids.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/dyff/schema/quantity.py` & `dyff_schema-0.6.0/dyff/schema/quantity.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/dyff/schema/v0/r1/adapters.py` & `dyff_schema-0.6.0/dyff/schema/v0/r1/adapters.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/dyff/schema/v0/r1/base.py` & `dyff_schema-0.6.0/dyff/schema/v0/r1/base.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/dyff/schema/v0/r1/dataset/__init__.py` & `dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/dyff/schema/v0/r1/dataset/arrow.py` & `dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/arrow.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/dyff/schema/v0/r1/dataset/binary.py` & `dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/binary.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/dyff/schema/v0/r1/dataset/text.py` & `dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/text.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/dyff/schema/v0/r1/io/vllm.py` & `dyff_schema-0.6.0/dyff/schema/v0/r1/io/vllm.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/dyff/schema/v0/r1/platform.py` & `dyff_schema-0.6.0/dyff/schema/v0/r1/platform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1093,14 +1093,24 @@
 
 
 class InferenceSessionAndToken(DyffSchemaBaseModel):
     inferencesession: InferenceSession
     token: str
 
 
+class InferenceSessionReference(DyffSchemaBaseModel):
+    session: str = pydantic.Field(
+        description="The ID of a running inference session.",
+    )
+
+    interface: InferenceInterface = pydantic.Field(
+        description="How to move data in and out of the service."
+    )
+
+
 class DatasetFilter(DyffSchemaBaseModel):
     """A rule for restrcting which instances in a Dataset are returned."""
 
     field: str
     relation: str
     value: str
 
@@ -1130,18 +1140,28 @@
 class Evaluation(DyffEntity, EvaluationBase):
     """A description of how to run an InferenceService on a Dataset to obtain a set of
     evaluation results."""
 
     kind: Literal["Evaluation"] = Entities.Evaluation.value
 
     inferenceSession: InferenceSessionSpec = pydantic.Field(
-        description="Specification of the InferenceSession that will perform inference for the evaluation.",
+        description="Specification of the InferenceSession that will perform"
+        " inference for the evaluation.",
+    )
+
+    inferenceSessionReference: Optional[str] = pydantic.Field(
+        default=None,
+        description="ID of a running inference session that will be used"
+        " for the evaluation instead of starting a new one.",
     )
 
     def dependencies(self) -> list[str]:
+        # TODO: It would be nice if the session could be a dependency,
+        # so that the client doesn't start until the session is ready, but
+        # dyff-orchestrator can't handle dependencies on sessions currently.
         return [self.dataset, self.inferenceSession.inferenceService.id]
 
     def resource_allocation(self) -> Optional[ResourceAllocation]:
         return None
 
 
 class ModuleBase(DyffSchemaBaseModel):
@@ -1863,14 +1883,15 @@
     "InferenceServiceRunner",
     "InferenceServiceRunnerKind",
     "InferenceServiceSources",
     "InferenceServiceSpec",
     "InferenceSession",
     "InferenceSessionAndToken",
     "InferenceSessionBase",
+    "InferenceSessionReference",
     "InferenceSessionSpec",
     "Label",
     "LabelKey",
     "LabelValue",
     "Labeled",
     "Measurement",
     "MeasurementLevel",
```

### Comparing `dyff_schema-0.5.3/dyff/schema/v0/r1/requests.py` & `dyff_schema-0.6.0/dyff/schema/v0/r1/requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,18 +69,35 @@
     inferenceService: str = pydantic.Field(description="InferenceService ID")
 
 
 class EvaluationCreateRequest(DyffEntityCreateRequest, EvaluationBase):
     """A description of how to run an InferenceService on a Dataset to obtain a set of
     evaluation results."""
 
-    inferenceSession: EvaluationInferenceSessionRequest = pydantic.Field(
+    inferenceSession: Optional[EvaluationInferenceSessionRequest] = pydantic.Field(
+        default=None,
         description="Specification of the InferenceSession that will perform inference for the evaluation.",
     )
 
+    inferenceSessionReference: Optional[str] = pydantic.Field(
+        default=None,
+        description="The ID of a running inference session that will be used"
+        " for the evaluation, instead of starting a new one.",
+    )
+
+    @pydantic.root_validator
+    def check_session_exactly_one(cls, values):
+        session = values.get("inferenceSession") is not None
+        session_ref = values.get("inferenceSessionReference") is not None
+        if not (session ^ session_ref):
+            raise ValueError(
+                "must specify exactly one of {inferenceSession, inferenceSessionReference}"
+            )
+        return values
+
 
 class MethodCreateRequest(DyffEntityCreateRequest, MethodBase):
     pass
 
 
 class ModelCreateRequest(DyffEntityCreateRequest, ModelSpec):
     pass
```

### Comparing `dyff_schema-0.5.3/dyff/schema/v0/r1/test.py` & `dyff_schema-0.6.0/dyff/schema/v0/r1/test.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/dyff_schema.egg-info/PKG-INFO` & `dyff_schema-0.6.0/dyff_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.5.3
+Version: 0.6.0
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_schema-0.5.3/dyff_schema.egg-info/SOURCES.txt` & `dyff_schema-0.6.0/dyff_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/pyproject.toml` & `dyff_schema-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.5.3/tests/test_import.py` & `dyff_schema-0.6.0/tests/test_import.py`

 * *Files identical despite different names*

