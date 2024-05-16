# Comparing `tmp/tclint-0.2.4.tar.gz` & `tmp/tclint-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tclint-0.2.4.tar", last modified: Wed Apr 24 03:21:02 2024, max compression
+gzip compressed data, was "tclint-0.2.5.tar", last modified: Thu May 16 02:21:39 2024, max compression
```

## Comparing `tclint-0.2.4.tar` & `tclint-0.2.5.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.636049 tclint-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-24 03:20:54.000000 tclint-0.2.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.624049 tclint-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.624049 tclint-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-24 03:20:54.000000 tclint-0.2.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-24 03:20:54.000000 tclint-0.2.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 03:20:54.000000 tclint-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-24 03:20:54.000000 tclint-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-24 03:21:02.636049 tclint-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-24 03:20:54.000000 tclint-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-24 03:20:54.000000 tclint-0.2.4/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 03:20:54.000000 tclint-0.2.4/dev-constraints.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.628049 tclint-0.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-24 03:20:54.000000 tclint-0.2.4/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-24 03:20:54.000000 tclint-0.2.4/docs/violations.md
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-24 03:20:54.000000 tclint-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 03:21:02.636049 tclint-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.624049 tclint-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.628049 tclint-0.2.4/src/tclint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 03:21:02.000000 tclint-0.2.4/src/tclint/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    25942 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.632049 tclint-0.2.4/src/tclint/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25927 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/commands/builtin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/commands/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27503 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/syntax_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/tclint.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/violations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.636049 tclint-0.2.4/src/tclint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-24 03:21:02.000000 tclint-0.2.4/src/tclint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-24 03:21:02.000000 tclint-0.2.4/src/tclint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 03:21:02.000000 tclint-0.2.4/src/tclint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-24 03:21:02.000000 tclint-0.2.4/src/tclint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-24 03:21:02.000000 tclint-0.2.4/src/tclint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 03:21:02.000000 tclint-0.2.4/src/tclint.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.632049 tclint-0.2.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.636049 tclint-0.2.4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/backslash-spacing.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/backslash-spacing.txt
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/blank-lines.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/blank-lines.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/clean.tcl
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/clean.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/dirty.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/dirty.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/example.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/example.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/expr-format.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/expr-format.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/indent.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/indent.txt
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/indent_lists.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/indent_lists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/lines.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/lines.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/spaces-in-braces.tcl
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/spaces-in-braces.toml
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/spaces-in-braces.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/special-comments.tcl
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/special-comments.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/tclint.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (127)    17815 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/test_tclint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:39.390583 tclint-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-16 02:21:33.000000 tclint-0.2.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:39.378583 tclint-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:39.378583 tclint-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-16 02:21:33.000000 tclint-0.2.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-16 02:21:33.000000 tclint-0.2.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-16 02:21:33.000000 tclint-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-16 02:21:33.000000 tclint-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-16 02:21:39.390583 tclint-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-16 02:21:33.000000 tclint-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-16 02:21:33.000000 tclint-0.2.5/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 02:21:33.000000 tclint-0.2.5/dev-constraints.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:39.378583 tclint-0.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-16 02:21:33.000000 tclint-0.2.5/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-16 02:21:33.000000 tclint-0.2.5/docs/violations.md
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-16 02:21:33.000000 tclint-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 02:21:39.390583 tclint-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:39.378583 tclint-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:39.382583 tclint-0.2.5/src/tclint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:33.000000 tclint-0.2.5/src/tclint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 02:21:39.000000 tclint-0.2.5/src/tclint/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25942 2024-05-16 02:21:33.000000 tclint-0.2.5/src/tclint/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:39.382583 tclint-0.2.5/src/tclint/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-16 02:21:33.000000 tclint-0.2.5/src/tclint/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25927 2024-05-16 02:21:33.000000 tclint-0.2.5/src/tclint/commands/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-16 02:21:33.000000 tclint-0.2.5/src/tclint/commands/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-16 02:21:33.000000 tclint-0.2.5/src/tclint/commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-16 02:21:33.000000 tclint-0.2.5/src/tclint/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-05-16 02:21:33.000000 tclint-0.2.5/src/tclint/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-16 02:21:33.000000 tclint-0.2.5/src/tclint/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27321 2024-05-16 02:21:33.000000 tclint-0.2.5/src/tclint/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-16 02:21:33.000000 tclint-0.2.5/src/tclint/syntax_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-16 02:21:33.000000 tclint-0.2.5/src/tclint/tclint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-16 02:21:33.000000 tclint-0.2.5/src/tclint/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-16 02:21:33.000000 tclint-0.2.5/src/tclint/violations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:39.390583 tclint-0.2.5/src/tclint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-16 02:21:39.000000 tclint-0.2.5/src/tclint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-16 02:21:39.000000 tclint-0.2.5/src/tclint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 02:21:39.000000 tclint-0.2.5/src/tclint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 02:21:39.000000 tclint-0.2.5/src/tclint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-16 02:21:39.000000 tclint-0.2.5/src/tclint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 02:21:39.000000 tclint-0.2.5/src/tclint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:39.382583 tclint-0.2.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:39.390583 tclint-0.2.5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/backslash-spacing.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/backslash-spacing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/blank-lines.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/blank-lines.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/clean.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/clean.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/dirty.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/dirty.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/example.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/example.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/expr-format.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/expr-format.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/indent.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/indent.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/indent_lists.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/indent_lists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/lines.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/lines.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/spaces-in-braces.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/spaces-in-braces.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/spaces-in-braces.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/special-comments.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/special-comments.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/data/tclint.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18591 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-16 02:21:33.000000 tclint-0.2.5/tests/test_tclint.py
```

### Comparing `tclint-0.2.4/.github/workflows/ci.yml` & `tclint-0.2.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/.github/workflows/release.yml` & `tclint-0.2.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/LICENSE` & `tclint-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/PKG-INFO` & `tclint-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclint
-Version: 0.2.4
+Version: 0.2.5
 Summary: A CLI utility for linting and analyzing Tcl code.
 Author-email: Noah Moroze <me@noahmoroze.com>
 License: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ply==3.11
```

### Comparing `tclint-0.2.4/README.md` & `tclint-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/docs/configuration.md` & `tclint-0.2.5/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/docs/violations.md` & `tclint-0.2.5/docs/violations.md`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/pyproject.toml` & `tclint-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/src/tclint/checks.py` & `tclint-0.2.5/src/tclint/checks.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/src/tclint/commands/__init__.py` & `tclint-0.2.5/src/tclint/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/src/tclint/commands/builtin.py` & `tclint-0.2.5/src/tclint/commands/builtin.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/src/tclint/commands/plugins.py` & `tclint-0.2.5/src/tclint/commands/plugins.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/src/tclint/commands/utils.py` & `tclint-0.2.5/src/tclint/commands/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -93,32 +93,43 @@
         # to handle this case. We require each command argument to correspond to
         # one child node, but multiple quoted or braced word arguments can be
         # combined into a single subcommand when interpreted eval-style. This
         # requirement exists to facilitate style checking, if we had a separate
         # CST for style checks and AST for logical checks we may be able to
         # handle it.
 
-        # TODO: once we have warnings, we could refactor to make this non-fatal
-        # and at least parse these arguments as lists to facilitate style
-        # checks.
-
         raise CommandArgError(
             f"unable to parse multiple {command} arguments when one includes a braced"
             " or quoted word"
         )
 
-    eval_args = []
+    # Construct the body of the eval taking whitespace into account to ensure we get
+    # style checking.
+
+    eval_script = ""
+    prev_arg_end_pos = None
     for arg in args:
         contents = arg.contents
         if contents is None:
             # TODO: flag sort of eval-specific violation? Common patterns will
             # often trigger this, and it seems useful to be able to turn it off
             raise CommandArgError(
                 f"{command} received an argument with a substitution, unable to parse"
                 " its arguments"
             )
-        eval_args.append(contents)
 
-    script = parser.parse(" ".join(eval_args), pos=(args[0].pos))
+        if prev_arg_end_pos is not None:
+            if prev_arg_end_pos[0] != arg.line:
+                # If we have multiple args on the same line, we know there must be a
+                # backslash newline. Add it so the parsing works.
+                eval_script += "\\\n" * (arg.line - prev_arg_end_pos[0])
+                eval_script += " " * (arg.col - 1)
+            else:
+                eval_script += " " * (arg.col - prev_arg_end_pos[1])
+        eval_script += contents
+
+        prev_arg_end_pos = arg.end_pos
+
+    script = parser.parse(eval_script, pos=(args[0].pos))
     script.end_pos = args[-1].end_pos
 
     return [script]
```

### Comparing `tclint-0.2.4/src/tclint/comments.py` & `tclint-0.2.5/src/tclint/comments.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/src/tclint/config.py` & `tclint-0.2.5/src/tclint/config.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/src/tclint/lexer.py` & `tclint-0.2.5/src/tclint/lexer.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/src/tclint/parser.py` & `tclint-0.2.5/src/tclint/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,18 +160,14 @@
             raise CommandArgError(
                 f"error parsing command arguments, possibly malformed {routine} command"
             )
 
         if new_args is None:
             return args
 
-        # This constraint ensures the parse tree represents the shape of the
-        # code for style checking purposes (e.g. arg spacing)
-        assert len(new_args) == len(args)
-
         return new_args
 
     def parse_script(self, node):
         if node.contents is None:
             raise CommandArgError(
                 "expected braced word or word without substitutions in argument"
                 " interpreted as script"
```

### Comparing `tclint-0.2.4/src/tclint/syntax_tree.py` & `tclint-0.2.5/src/tclint/syntax_tree.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/src/tclint/tclint.py` & `tclint-0.2.5/src/tclint/tclint.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/src/tclint/violations.py` & `tclint-0.2.5/src/tclint/violations.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/src/tclint.egg-info/PKG-INFO` & `tclint-0.2.5/src/tclint.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclint
-Version: 0.2.4
+Version: 0.2.5
 Summary: A CLI utility for linting and analyzing Tcl code.
 Author-email: Noah Moroze <me@noahmoroze.com>
 License: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ply==3.11
```

### Comparing `tclint-0.2.4/src/tclint.egg-info/SOURCES.txt` & `tclint-0.2.5/src/tclint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/tests/data/blank-lines.txt` & `tclint-0.2.5/tests/data/blank-lines.txt`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/tests/data/dirty.txt` & `tclint-0.2.5/tests/data/dirty.txt`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/tests/data/expr-format.txt` & `tclint-0.2.5/tests/data/expr-format.txt`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/tests/data/indent.txt` & `tclint-0.2.5/tests/data/indent.txt`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/tests/data/indent_lists.tcl` & `tclint-0.2.5/tests/data/indent_lists.tcl`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/tests/data/spaces-in-braces.txt` & `tclint-0.2.5/tests/data/spaces-in-braces.txt`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/tests/data/tclint.toml` & `tclint-0.2.5/tests/data/tclint.toml`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/tests/test_config.py` & `tclint-0.2.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/tests/test_lint.py` & `tclint-0.2.5/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.4/tests/test_parser.py` & `tclint-0.2.5/tests/test_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -404,27 +404,52 @@
 def test_puts_blank():
     script = 'puts ""'
 
     tree = parse(script)
     assert tree == Script(Command(BareWord("puts"), QuotedWord()))
 
 
-@pytest.mark.skip(reason="we don't support parsing this anymore")
-def test_eval_braced_multi_arg():
-    script = "eval puts {a b c}"
+def test_eval_positions():
+    script = r"""eval  command  arg1\
+ arg2"""
 
     tree = parse(script)
     assert tree == Script(
         Command(
             BareWord("eval"),
-            Script(
-                Command(BareWord("puts"), BareWord("a"), BareWord("b"), BareWord("c"))
-            ),
+            Script(Command(BareWord("command"), BareWord("arg1"), BareWord("arg2"))),
         )
     )
+    eval_command = tree.children[0]
+    script = eval_command.args[0]
+    command = script.children[0]
+    assert command.children[0].pos == (1, 7)
+    assert command.children[1].pos == (1, 16)
+    assert command.children[2].pos == (2, 2)
+
+
+def test_eval_braced_multi_arg():
+    script = "eval puts {a b c}"
+
+    tree = parse(script)
+    assert tree == Script(
+        Command(BareWord("eval"), BareWord("puts"), BracedWord("a b c"))
+    )
+
+    # This reflects the actual Tcl semantics, but we currently treat this as
+    # un-parseable since we don't have a clean way to handle the positions of these
+    # items for style-checking purposes.
+    # assert tree == Script(
+    #     Command(
+    #         BareWord("eval"),
+    #         Script(
+    #             Command(BareWord("puts"), BareWord("a"), BareWord("b"), BareWord("c"))
+    #         ),
+    #     )
+    # )
 
 
 def test_eval():
     script = "eval {puts {a b c}}"
 
     tree = parse(script)
     assert tree == Script(
```

### Comparing `tclint-0.2.4/tests/test_tclint.py` & `tclint-0.2.5/tests/test_tclint.py`

 * *Files identical despite different names*

