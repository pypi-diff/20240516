# Comparing `tmp/rocm_docs_core-1.1.0.tar.gz` & `tmp/rocm_docs_core-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocm_docs_core-1.1.0.tar", last modified: Wed Apr 24 15:45:55 2024, max compression
+gzip compressed data, was "rocm_docs_core-1.1.1.tar", last modified: Fri Apr 26 22:51:10 2024, max compression
```

## Comparing `rocm_docs_core-1.1.0.tar` & `rocm_docs_core-1.1.1.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.862615 rocm_docs_core-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-24 15:45:55.862615 rocm_docs_core-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:45:55.862615 rocm_docs_core-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.838615 rocm_docs_core-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.838615 rocm_docs_core-1.1.0/src/rocm_docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.838615 rocm_docs_core-1.1.0/src/rocm_docs/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.838615 rocm_docs_core-1.1.0/src/rocm_docs/data/_doxygen/
--rw-r--r--   0 runner    (1001) docker     (127)    72476 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/data/_doxygen/extra_stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/data/_doxygen/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/data/_doxygen/header.html
--rw-r--r--   0 runner    (1001) docker     (127)    37255 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/data/_doxygen/stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/data/projects.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/data/projects.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/doxygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)    17085 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.842615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/404.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.842615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/components/article-info.html
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/components/left-side-menu.html
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/components/toggle-primary-sidebar.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.834615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.842615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/footer.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/header.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/left-side-menu.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.842615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/footer.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/header.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/left-side-menu.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.842615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/footer.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/header.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/left-side-menu.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.842615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/sections/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/sections/footer-content.html
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/sections/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.846615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.838615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.858615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/
--rwxr-xr-x   0 runner    (1001) docker     (127)    20756 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    16748 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    21924 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    17872 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    20780 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    16808 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    21876 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    17876 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    20672 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    16756 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    21820 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    17780 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    20172 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    16372 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    21248 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    17384 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    20664 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    16696 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    21520 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    17544 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    27552 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    22132 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    29388 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    23712 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    27592 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    22184 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    29392 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    23824 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    27456 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    22212 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    29224 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    23676 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    26652 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    21516 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    28292 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    22904 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    27376 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    22040 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    28704 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    23168 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    29304 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    23704 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    27520 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    22084 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    21856 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    17820 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    20712 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    16740 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts.css
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.858615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      925 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1760 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)    10074 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/rdcMisc.js
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css
--rw-r--r--   0 runner    (1001) docker     (127)    19276 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/rocm_header.css
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/theme_mode_captions.js
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.858615 rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-24 15:45:55.000000 rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-24 15:45:55.000000 rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:45:55.000000 rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-24 15:45:55.000000 rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-24 15:45:55.000000 rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 15:45:55.000000 rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.858615 rocm_docs_core-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/tests/test_doxygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/tests/test_sites.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.726653 rocm_docs_core-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-26 22:51:10.726653 rocm_docs_core-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 22:51:10.726653 rocm_docs_core-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.698653 rocm_docs_core-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.702653 rocm_docs_core-1.1.1/src/rocm_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.702653 rocm_docs_core-1.1.1/src/rocm_docs/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.702653 rocm_docs_core-1.1.1/src/rocm_docs/data/_doxygen/
+-rw-r--r--   0 runner    (1001) docker     (127)    72476 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/data/_doxygen/extra_stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/data/_doxygen/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/data/_doxygen/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)    37255 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/data/_doxygen/stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/data/projects.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/data/projects.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17085 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.706653 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/404.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.706653 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/components/article-info.html
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/components/left-side-menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/components/toggle-primary-sidebar.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.698653 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/flavors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.706653 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/flavors/rocm/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/flavors/rocm/footer.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/flavors/rocm/header.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/flavors/rocm/left-side-menu.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.706653 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/footer.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/header.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/left-side-menu.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.706653 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/footer.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/header.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/left-side-menu.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.706653 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/sections/footer-content.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/sections/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.710653 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.698653 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.718653 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20756 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16748 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21924 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17872 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20780 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16808 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21876 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17876 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20672 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16756 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21820 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17780 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20172 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16372 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21248 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17384 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20664 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16696 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21520 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17544 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27552 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22132 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29388 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23712 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27592 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22184 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29392 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23824 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27456 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22212 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29224 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23676 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26652 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21516 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28292 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22904 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27376 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22040 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28704 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23168 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29304 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23704 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27520 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22084 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21856 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17820 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20712 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16740 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.722653 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      925 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1760 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10074 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/rdcMisc.js
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css
+-rw-r--r--   0 runner    (1001) docker     (127)    19276 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/rocm_header.css
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/theme_mode_captions.js
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/src/rocm_docs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.722653 rocm_docs_core-1.1.1/src/rocm_docs_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-26 22:51:10.000000 rocm_docs_core-1.1.1/src/rocm_docs_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-26 22:51:10.000000 rocm_docs_core-1.1.1/src/rocm_docs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 22:51:10.000000 rocm_docs_core-1.1.1/src/rocm_docs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-26 22:51:10.000000 rocm_docs_core-1.1.1/src/rocm_docs_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-26 22:51:10.000000 rocm_docs_core-1.1.1/src/rocm_docs_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 22:51:10.000000 rocm_docs_core-1.1.1/src/rocm_docs_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:10.722653 rocm_docs_core-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/tests/test_doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 22:51:01.000000 rocm_docs_core-1.1.1/tests/test_sites.py
```

### Comparing `rocm_docs_core-1.1.0/LICENSE.txt` & `rocm_docs_core-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/PKG-INFO` & `rocm_docs_core-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocm-docs-core
-Version: 1.1.0
+Version: 1.1.1
 Summary: Core utilities for all ROCm documentation on RTD
 Author-email: Lauren Wrubleski <Lauren.Wrubleski@amd.com>
 Project-URL: repository, https://github.com/RadeonOpenCompute/rocm-docs-core
 Project-URL: documentation, https://docs.amd.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rocm_docs_core-1.1.0/README.md` & `rocm_docs_core-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/pyproject.toml` & `rocm_docs_core-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'rocm-docs-core'
-version = "1.1.0"
+version = "1.1.1"
 authors=[
   {name="Lauren Wrubleski", email="Lauren.Wrubleski@amd.com"}
 ]
 description ='Core utilities for all ROCm documentation on RTD'
 readme="README.md"
 classifiers = [
   "Programming Language :: Python :: 3",
@@ -68,15 +68,15 @@
 [tool.black]
 target-version = ["py310"]
 line-length = 80
 color = true
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.1.0"
+version = "1.1.1"
 version_files = ["pyproject.toml:^version", "docs/conf.py:^(version|release)"]
 tag_format = "v$version"
 annotated_tag = true
 
 [tool.isort]
 # https://github.com/timothycrosley/isort/
 py_version = "310"
```

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/__init__.py` & `rocm_docs_core-1.1.1/src/rocm_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/core.py` & `rocm_docs_core-1.1.1/src/rocm_docs/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 ) -> None:
     """Add article info headers to the configured HTML pages.
 
     The pages can be set in "article_pages" of the Sphinx configuration.
     """
     repo = git.repo.Repo(app.srcdir, search_parent_directories=True)
     for page in app.config.article_pages:
-        path_rel = app.project.doc2path(page["file"], basedir=False)
+        path_rel = app.project.doc2path(page["file"], False)
         path_html = Path(app.outdir, path_rel).with_suffix(".html")
         path_source = Path(app.srcdir, path_rel)
 
         # FIXME: This will silently skip all files when not building the default
         # `html` format (e.g `htmlzip`, `epub` or `pdf`)
         if not path_html.is_file():
             continue
@@ -201,15 +201,15 @@
     """
     repo = git.repo.Repo(app.srcdir, search_parent_directories=True)
     for docname in app.project.docnames:
         # skip pages with specific settings
         if docname in specific_pages:
             continue
 
-        page_rel = app.project.doc2path(docname, basedir=False)
+        page_rel = app.project.doc2path(docname, False)
         page = Path(app.outdir, page_rel).with_suffix(".html")
 
         # FIXME: This will silently skip all files when not building the default
         # `html` format (e.g `htmlzip`, `epub` or `pdf`)
         if not page.is_file():
             continue
 
@@ -329,14 +329,16 @@
     )
     app.add_config_value(
         "all_article_info_date", default="2023", rebuild="html", types=str
     )
     app.add_config_value(
         "all_article_info_read_time", default="", rebuild="html", types=str
     )
-    app.add_config_value("article_pages", default=[], rebuild="html", types=Any)
+    app.add_config_value(
+        "article_pages", default=[], rebuild="html", types=list
+    )
 
     # Run before notfound.extension sees the config (default priority(=500))
     app.connect("config-inited", _force_notfound_prefix, priority=400)
     app.connect("config-inited", _DefaultSettings.update_config)
     app.connect("build-finished", _set_article_info, priority=1000)
     return {"parallel_read_safe": True, "parallel_write_safe": True}
```

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/data/_doxygen/extra_stylesheet.css` & `rocm_docs_core-1.1.1/src/rocm_docs/data/_doxygen/extra_stylesheet.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/data/_doxygen/header.html` & `rocm_docs_core-1.1.1/src/rocm_docs/data/_doxygen/header.html`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/data/_doxygen/stylesheet.css` & `rocm_docs_core-1.1.1/src/rocm_docs/data/_doxygen/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/data/projects.schema.json` & `rocm_docs_core-1.1.1/src/rocm_docs/data/projects.schema.json`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/data/projects.yaml` & `rocm_docs_core-1.1.1/src/rocm_docs/data/projects.yaml`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/doxygen.py` & `rocm_docs_core-1.1.1/src/rocm_docs/doxygen.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         "-m",
         "doxysphinx",
         "build",
         "--doxygen_exe=" + str(doxygen_exe.absolute()),
     ]
     if doxyphinx_version.endswith("+tagfile.toc"):
         args.append("--tagfile_toc")
-    args += [app.srcdir, app.outdir, str(doxyfile)]
+    args += [str(app.srcdir), str(app.outdir), str(doxyfile)]
 
     try:
         subprocess.check_call(args, cwd=doxygen_root)
     except subprocess.CalledProcessError as err:
         raise RuntimeError(
             f"doxysphinx failed (exit code: {err.returncode})"
         ) from err
@@ -211,36 +211,36 @@
 
 def setup(app: Sphinx) -> dict[str, Any]:
     """Set up rocm_docs.doxygen as a Sphinx extension."""
     app.setup_extension("sphinx.ext.mathjax")
     app.setup_extension("breathe")
 
     app.add_config_value(
-        "doxygen_root", ".doxygen", rebuild="", types=[None, str, os.PathLike]
+        "doxygen_root", ".doxygen", rebuild="", types=[str, os.PathLike]
     )
     app.add_config_value(
         "doxygen_executable",
         None,
         rebuild="",
-        types=[None, str, "os.PathLike[Any]"],
+        types=[str, os.PathLike[Any]],
     )
     app.add_config_value(
         "doxyfile",
         lambda config: Path(config.doxygen_root, "Doxyfile"),
         rebuild="",
-        types=[None, str, "os.PathLike[Any]"],
+        types=[str, os.PathLike[Any]],
     )
     app.add_config_value(
         "doxygen_project",
         lambda config: {
             "name": "doxygen",
             "path": Path(config.doxygen_root, "docBin", "xml"),
         },
         rebuild="",
-        types=dict[str, Union[None, str, "os.PathLike[Any]"]],
+        types=dict[str, Union[str, "os.PathLike[Any]"]],
     )
     app.add_config_value("doxysphinx_enabled", False, rebuild="", types=bool)
     app.add_config_value("doxygen_html", None, rebuild="")
 
     # Should run before breathe sees their parameters, as we provide defaults.
     app.connect("config-inited", _run_doxygen, priority=400)
     # Has to run after projects.py config-inited, as it might set
```

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/formatting.py` & `rocm_docs_core-1.1.1/src/rocm_docs/formatting.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/projects.py` & `rocm_docs_core-1.1.1/src/rocm_docs/projects.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/components/article-info.html` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/components/article-info.html`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/header.jinja` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/flavors/rocm/header.jinja`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/header.jinja` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/header.jinja`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/header.jinja` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/header.jinja`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/sections/footer.html` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/sections/footer.html`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/sections/header.html` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/sections/header.html`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/custom.css` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/custom.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts.css` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts.css.map` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts.css.map`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts.scss` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/fonts.scss`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/rdcMisc.js` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/rdcMisc.js`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/rocm_header.css` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/rocm_header.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/theme_mode_captions.js` & `rocm_docs_core-1.1.1/src/rocm_docs/rocm_docs_theme/static/theme_mode_captions.js`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/theme.py` & `rocm_docs_core-1.1.1/src/rocm_docs/theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         announcement_info = "This page contains proposed changes for a future release of ROCm. Read the <a href='https://rocm.docs.amd.com/en/latest/'>latest Linux release of ROCm documentation</a> for your production environments."
 
     theme_opts.setdefault("announcement", announcement_info)
 
 
 def _update_theme_options(app: Sphinx) -> None:
     theme_opts = get_theme_options_dict(app)
-    _update_repo_opts(app.srcdir, theme_opts)
+    _update_repo_opts(str(app.srcdir), theme_opts)
 
     supported_flavors = ["rocm", "local", "rocm-docs-home", "rocm-blogs"]
     flavor = theme_opts.get("flavor", "rocm")
     if flavor not in supported_flavors:
         logger.error(
             f'Unsupported theme flavor "{flavor}", must be one of: {supported_flavors}.\n'
             "Using flavor={supported_flavors[0]}"
```

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs/util.py` & `rocm_docs_core-1.1.1/src/rocm_docs/util.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/PKG-INFO` & `rocm_docs_core-1.1.1/src/rocm_docs_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocm-docs-core
-Version: 1.1.0
+Version: 1.1.1
 Summary: Core utilities for all ROCm documentation on RTD
 Author-email: Lauren Wrubleski <Lauren.Wrubleski@amd.com>
 Project-URL: repository, https://github.com/RadeonOpenCompute/rocm-docs-core
 Project-URL: documentation, https://docs.amd.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/SOURCES.txt` & `rocm_docs_core-1.1.1/src/rocm_docs_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/tests/test_doxygen.py` & `rocm_docs_core-1.1.1/tests/test_doxygen.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/tests/test_meta.py` & `rocm_docs_core-1.1.1/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.0/tests/test_projects.py` & `rocm_docs_core-1.1.1/tests/test_projects.py`

 * *Files identical despite different names*

