# Comparing `tmp/cuminai-0.0.1.dev116.tar.gz` & `tmp/cuminai-0.0.1.dev165.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuminai-0.0.1.dev116.tar", max compression
+gzip compressed data, was "cuminai-0.0.1.dev165.tar", max compression
```

## Comparing `cuminai-0.0.1.dev116.tar` & `cuminai-0.0.1.dev165.tar`

### file list

```diff
@@ -1,4 +1,9 @@
--rw-r--r--   0        0        0        0 2024-05-11 10:43:34.264020 cuminai-0.0.1.dev116/cuminai/__init__.py
--rw-r--r--   0        0        0      386 2024-05-11 12:18:07.023058 cuminai-0.0.1.dev116/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-11 10:43:34.264020 cuminai-0.0.1.dev116/README.md
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 cuminai-0.0.1.dev116/PKG-INFO
+-rw-r--r--   0        0        0       75 2024-05-12 07:46:46.527637 cuminai-0.0.1.dev165/cuminai/__init__.py
+-rw-r--r--   0        0        0      691 2024-05-15 18:12:16.655249 cuminai-0.0.1.dev165/cuminai/constants.py
+-rw-r--r--   0        0        0     2466 2024-05-15 10:54:39.551320 cuminai-0.0.1.dev165/cuminai/contextstores.py
+-rw-r--r--   0        0        0    12061 2024-05-16 05:54:42.498882 cuminai-0.0.1.dev165/cuminai/creator.py
+-rw-r--r--   0        0        0      520 2024-05-15 10:40:50.032155 cuminai-0.0.1.dev165/cuminai/validator.py
+-rw-r--r--   0        0        0    11558 2024-05-11 18:16:30.219425 cuminai-0.0.1.dev165/LICENSE
+-rw-r--r--   0        0        0      569 2024-05-16 05:51:20.992730 cuminai-0.0.1.dev165/pyproject.toml
+-rw-r--r--   0        0        0     1350 2024-05-16 05:53:31.413774 cuminai-0.0.1.dev165/README.md
+-rw-r--r--   0        0        0     2036 1970-01-01 00:00:00.000000 cuminai-0.0.1.dev165/PKG-INFO
```

