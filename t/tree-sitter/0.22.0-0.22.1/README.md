# Comparing `tmp/tree-sitter-0.22.0.tar.gz` & `tmp/tree-sitter-0.22.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-sitter-0.22.0.tar", last modified: Mon May 13 19:37:28 2024, max compression
+gzip compressed data, was "tree-sitter-0.22.1.tar", last modified: Thu May 16 12:04:15 2024, max compression
```

## Comparing `tree-sitter-0.22.0.tar` & `tree-sitter-0.22.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.694662 tree-sitter-0.22.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-05-13 19:37:28.694662 tree-sitter-0.22.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:37:28.694662 tree-sitter-0.22.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.686662 tree-sitter-0.22.0/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.686662 tree-sitter-0.22.0/tree_sitter/binding/
--rw-r--r--   0 runner    (1001) docker     (127)    11697 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/language.c
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/lookahead_iterator.c
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/lookahead_names_iterator.c
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/module.c
--rw-r--r--   0 runner    (1001) docker     (127)    30759 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/node.c
--rw-r--r--   0 runner    (1001) docker     (127)    16982 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/parser.c
--rw-r--r--   0 runner    (1001) docker     (127)    26415 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/query.c
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/range.c
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/tree.c
--rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/tree_cursor.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.686662 tree-sitter-0.22.0/tree_sitter/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.686662 tree-sitter-0.22.0/tree_sitter/core/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.686662 tree-sitter-0.22.0/tree_sitter/core/lib/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.686662 tree-sitter-0.22.0/tree_sitter/core/lib/include/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (127)    40024 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/include/tree_sitter/api.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.694662 tree-sitter-0.22.0/tree_sitter/core/lib/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/alloc.c
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/alloc.h
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/array.h
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/atomic.h
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/clock.h
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/error_costs.h
--rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/get_changed_ranges.c
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/get_changed_ranges.h
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/host.h
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/language.c
--rw-r--r--   0 runner    (1001) docker     (127)     8368 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/language.h
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/length.h
--rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/lexer.c
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/lexer.h
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/lib.c
--rw-r--r--   0 runner    (1001) docker     (127)    22016 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/node.c
--rw-r--r--   0 runner    (1001) docker     (127)    73664 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/parser.h
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/point.h
--rw-r--r--   0 runner    (1001) docker     (127)   141258 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/query.c
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/reduce_action.h
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/reusable_node.h
--rw-r--r--   0 runner    (1001) docker     (127)    28201 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/stack.c
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/stack.h
--rw-r--r--   0 runner    (1001) docker     (127)    35490 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/subtree.c
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/subtree.h
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/tree.c
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/tree.h
--rw-r--r--   0 runner    (1001) docker     (127)    22905 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/tree_cursor.c
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/tree_cursor.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.694662 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/ICU_SHA
--rw-r--r--   0 runner    (1001) docker     (127)    21001 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/ptypes.h
--rw-r--r--   0 runner    (1001) docker     (127)    14865 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/umachine.h
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/urename.h
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/utf.h
--rw-r--r--   0 runner    (1001) docker     (127)    23878 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/utf16.h
--rw-r--r--   0 runner    (1001) docker     (127)    31698 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/utf8.h
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode.h
--rw-r--r--   0 runner    (1001) docker     (127)    59477 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/wasm_store.c
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/wasm_store.h
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.686662 tree-sitter-0.22.0/tree_sitter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-05-13 19:37:28.000000 tree-sitter-0.22.0/tree_sitter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-13 19:37:28.000000 tree-sitter-0.22.0/tree_sitter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:37:28.000000 tree-sitter-0.22.0/tree_sitter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-13 19:37:28.000000 tree-sitter-0.22.0/tree_sitter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 19:37:28.000000 tree-sitter-0.22.0/tree_sitter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:04:15.252871 tree-sitter-0.22.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-05-16 12:04:15.252871 tree-sitter-0.22.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8787 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:04:15.252871 tree-sitter-0.22.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:04:15.244871 tree-sitter-0.22.1/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/tree_sitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10486 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/tree_sitter/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:04:15.244871 tree-sitter-0.22.1/tree_sitter/binding/
+-rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/tree_sitter/binding/language.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/tree_sitter/binding/lookahead_iterator.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/tree_sitter/binding/lookahead_names_iterator.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/tree_sitter/binding/module.c
+-rw-r--r--   0 runner    (1001) docker     (127)    30760 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/tree_sitter/binding/node.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16932 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/tree_sitter/binding/parser.c
+-rw-r--r--   0 runner    (1001) docker     (127)    26415 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/tree_sitter/binding/query.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/tree_sitter/binding/range.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/tree_sitter/binding/tree.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13651 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/tree_sitter/binding/tree_cursor.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:04:15.240871 tree-sitter-0.22.1/tree_sitter/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:04:15.240871 tree-sitter-0.22.1/tree_sitter/core/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:04:15.240871 tree-sitter-0.22.1/tree_sitter/core/lib/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:04:15.244871 tree-sitter-0.22.1/tree_sitter/core/lib/include/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (127)    40024 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/include/tree_sitter/api.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:04:15.252871 tree-sitter-0.22.1/tree_sitter/core/lib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/alloc.c
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/alloc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/atomic.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/clock.h
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/error_costs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/get_changed_ranges.c
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/get_changed_ranges.h
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/host.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/language.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8368 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/language.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/length.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/lexer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/lexer.h
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/lib.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22016 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/node.c
+-rw-r--r--   0 runner    (1001) docker     (127)    73664 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/parser.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/point.h
+-rw-r--r--   0 runner    (1001) docker     (127)   141258 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/query.c
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/reduce_action.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/reusable_node.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28201 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/stack.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/stack.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35490 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/subtree.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/subtree.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/tree.c
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/tree.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22905 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/tree_cursor.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/tree_cursor.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:04:15.252871 tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode/ICU_SHA
+-rw-r--r--   0 runner    (1001) docker     (127)    21001 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode/ptypes.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14865 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode/umachine.h
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode/urename.h
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode/utf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23878 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode/utf16.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31698 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode/utf8.h
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode.h
+-rw-r--r--   0 runner    (1001) docker     (127)    59477 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/wasm_store.c
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-16 12:04:11.000000 tree-sitter-0.22.1/tree_sitter/core/lib/src/wasm_store.h
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:04:09.000000 tree-sitter-0.22.1/tree_sitter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:04:15.244871 tree-sitter-0.22.1/tree_sitter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-05-16 12:04:15.000000 tree-sitter-0.22.1/tree_sitter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-16 12:04:15.000000 tree-sitter-0.22.1/tree_sitter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:04:15.000000 tree-sitter-0.22.1/tree_sitter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-16 12:04:15.000000 tree-sitter-0.22.1/tree_sitter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 12:04:15.000000 tree-sitter-0.22.1/tree_sitter.egg-info/top_level.txt
```

### Comparing `tree-sitter-0.22.0/LICENSE` & `tree-sitter-0.22.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/PKG-INFO` & `tree-sitter-0.22.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-sitter
-Version: 0.22.0
+Version: 0.22.1
 Summary: Python bindings to the Tree-sitter parsing library
 Author-email: Max Brunsfeld <maxbrunsfeld@gmail.com>
 Project-URL: Homepage, https://tree-sitter.github.io/tree-sitter/
 Project-URL: Source, https://github.com/tree-sitter/py-tree-sitter
 Project-URL: Documentation, https://tree-sitter.github.io/py-tree-sitter/
 Keywords: incremental,parsing,tree-sitter
 Classifier: Intended Audience :: Developers
@@ -63,16 +63,15 @@
 ```
 
 ### Basic parsing
 
 Create a `Parser` and configure it to use a language:
 
 ```python
-parser = Parser()
-parser.set_language(PY_LANGUAGE)
+parser = Parser(PY_LANGUAGE)
 ```
 
 Parse some source code:
 
 ```python
 tree = parser.parse(
     bytes(
@@ -157,15 +156,15 @@
 function_call_name_node = function_call_node.child_by_field_name("function")
 assert function_call_name_node.type == "identifier"
 
 function_call_args_node = function_call_node.child_by_field_name("arguments")
 assert function_call_args_node.type == "argument_list"
 
 
-assert root_node.sexp() == (
+assert str(root_node) == (
     "(module "
         "(function_definition "
             "name: (identifier) "
             "parameters: (parameters) "
             "body: (block "
                 "(if_statement "
                     "condition: (identifier) "
@@ -175,15 +174,15 @@
                             "arguments: (argument_list))))))))"
 )
 ```
 
 Or, to use the byte offset with UTF-16 encoding:
 
 ```python
-parser.set_language(JAVASCRIPT)
+parser.language = JAVASCRIPT
 source_code = bytes("'😎' && '🐍'", "utf16")
 
 def read(byte_position, _):
     return source_code[byte_position: byte_position + 2]
 
 tree = parser.parse(read, encoding="utf16")
 root_node = tree.root_node
```

### Comparing `tree-sitter-0.22.0/README.md` & `tree-sitter-0.22.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,15 @@
 ```
 
 ### Basic parsing
 
 Create a `Parser` and configure it to use a language:
 
 ```python
-parser = Parser()
-parser.set_language(PY_LANGUAGE)
+parser = Parser(PY_LANGUAGE)
 ```
 
 Parse some source code:
 
 ```python
 tree = parser.parse(
     bytes(
@@ -134,15 +133,15 @@
 function_call_name_node = function_call_node.child_by_field_name("function")
 assert function_call_name_node.type == "identifier"
 
 function_call_args_node = function_call_node.child_by_field_name("arguments")
 assert function_call_args_node.type == "argument_list"
 
 
-assert root_node.sexp() == (
+assert str(root_node) == (
     "(module "
         "(function_definition "
             "name: (identifier) "
             "parameters: (parameters) "
             "body: (block "
                 "(if_statement "
                     "condition: (identifier) "
@@ -152,15 +151,15 @@
                             "arguments: (argument_list))))))))"
 )
 ```
 
 Or, to use the byte offset with UTF-16 encoding:
 
 ```python
-parser.set_language(JAVASCRIPT)
+parser.language = JAVASCRIPT
 source_code = bytes("'😎' && '🐍'", "utf16")
 
 def read(byte_position, _):
     return source_code[byte_position: byte_position + 2]
 
 tree = parser.parse(read, encoding="utf16")
 root_node = tree.root_node
```

### Comparing `tree-sitter-0.22.0/pyproject.toml` & `tree-sitter-0.22.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=43"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tree-sitter"
-version = "0.22.0"
+version = "0.22.1"
 description = "Python bindings to the Tree-sitter parsing library"
 keywords = ["incremental", "parsing", "tree-sitter"]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: C",
```

### Comparing `tree-sitter-0.22.0/setup.py` & `tree-sitter-0.22.1/setup.py`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/__init__.py` & `tree-sitter-0.22.1/tree_sitter/__init__.py`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/__init__.pyi` & `tree-sitter-0.22.1/tree_sitter/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,14 @@
     def field_id_for_name(self, name: str, /) -> int | None: ...
     def next_state(self, state: int, id: int, /) -> int: ...
     def lookahead_iterator(self, state: int, /) -> LookaheadIterator | None: ...
     def query(self, source: str, /) -> Query: ...
     def __repr__(self) -> str: ...
     def __eq__(self, other: Any, /) -> bool: ...
     def __ne__(self, other: Any, /) -> bool: ...
-    def __int__(self) -> int: ...
-    def __index__(self) -> int: ...
     def __hash__(self) -> int: ...
 
 @final
 class Node:
     @property
     def id(self) -> int: ...
     @property
@@ -183,15 +181,15 @@
     ) -> None: ...
     def walk(self) -> TreeCursor: ...
     def changed_ranges(self, new_tree: Tree) -> list[Range]: ...
 
 @final
 class TreeCursor:
     @property
-    def node(self) -> Node: ...
+    def node(self) -> Node | None: ...
     @property
     def field_id(self) -> int | None: ...
     @property
     def field_name(self) -> str | None: ...
     @property
     def depth(self) -> int: ...
     @property
@@ -300,18 +298,18 @@
     @property
     def language(self) -> Language: ...
     @property
     def current_symbol(self) -> int: ...
     @property
     def current_symbol_name(self) -> str: ...
     @deprecated("Use `reset_state()` instead")
-    def reset(self, language: _Ptr, state: int, /) -> None: ...
+    def reset(self, language: _Ptr, state: int, /) -> bool: ...
 
     # TODO(0.24): rename to reset
-    def reset_state(self, state: int, language: Language | None = None) -> None: ...
+    def reset_state(self, state: int, language: Language | None = None) -> bool: ...
     def iter_names(self) -> Iterator[str]: ...
     def __next__(self) -> int: ...
 
 @final
 class Range:
     def __init__(
         self,
```

### Comparing `tree-sitter-0.22.0/tree_sitter/binding/language.c` & `tree-sitter-0.22.1/tree_sitter/binding/language.c`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,14 @@
                                 (Py_uintptr_t)self->language, self->version, self->name);
 #else
     return PyUnicode_FromFormat("<Language id=%" PRIuPTR ", version=%u>",
                                 (Py_uintptr_t)self->language, self->version);
 #endif
 }
 
-PyObject *language_int(Language *self) { return PyLong_FromVoidPtr(self->language); }
-
 Py_hash_t language_hash(Language *self) { return (Py_hash_t)self->language; }
 
 PyObject *language_compare(Language *self, PyObject *other, int op) {
     if ((op != Py_EQ && op != Py_NE) || !IS_INSTANCE(other, language_type)) {
         Py_RETURN_NOTIMPLEMENTED;
     }
 
@@ -296,16 +294,14 @@
     {Py_tp_init, language_init},
     {Py_tp_repr, language_repr},
     {Py_tp_hash, language_hash},
     {Py_tp_richcompare, language_compare},
     {Py_tp_dealloc, language_dealloc},
     {Py_tp_methods, language_methods},
     {Py_tp_getset, language_accessors},
-    {Py_nb_int, language_int},
-    {Py_nb_index, language_int},
     {0, NULL},
 };
 
 PyType_Spec language_type_spec = {
     .name = "tree_sitter.Language",
     .basicsize = sizeof(Language),
     .itemsize = 0,
```

### Comparing `tree-sitter-0.22.0/tree_sitter/binding/lookahead_iterator.c` & `tree-sitter-0.22.1/tree_sitter/binding/lookahead_iterator.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/binding/lookahead_names_iterator.c` & `tree-sitter-0.22.1/tree_sitter/binding/lookahead_names_iterator.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/binding/module.c` & `tree-sitter-0.22.1/tree_sitter/binding/module.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/binding/node.c` & `tree-sitter-0.22.1/tree_sitter/binding/node.c`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     TSNode child = ts_node_child_by_field_name(self->node, name, length);
     if (ts_node_is_null(child)) {
         Py_RETURN_NONE;
     }
     return node_new_internal(state, child, self->tree);
 }
 
-PyObject *node_children_by_field_id_internal(Node *self, TSFieldId field_id) {
+static PyObject *node_children_by_field_id_internal(Node *self, TSFieldId field_id) {
     ModuleState *state = GET_MODULE_STATE(self);
     PyObject *result = PyList_New(0);
 
     if (field_id == 0) {
         return result;
     }
 
@@ -214,15 +214,15 @@
     if (!PyArg_ParseTuple(args, "l:field_name_for_child", &index)) {
         return NULL;
     }
     if (index < 0) {
         PyErr_SetString(PyExc_ValueError, "child index must be positive");
         return NULL;
     }
-    if ((uint32_t)index >= ts_node_named_child_count(self->node)) {
+    if ((uint32_t)index >= ts_node_child_count(self->node)) {
         PyErr_SetString(PyExc_IndexError, "child index out of range");
         return NULL;
     }
 
     const char *field_name = ts_node_field_name_for_child(self->node, index);
     if (field_name == NULL) {
         Py_RETURN_NONE;
```

### Comparing `tree-sitter-0.22.0/tree_sitter/binding/parser.c` & `tree-sitter-0.22.1/tree_sitter/binding/parser.c`

 * *Files 0% similar despite different names*

```diff
@@ -291,16 +291,15 @@
             PyMem_Free(ranges);
             return -1;
         }
         ranges[i] = ((Range *)range)->range;
     }
 
     if (!ts_parser_set_included_ranges(self->parser, ranges, length)) {
-        PyErr_SetString(PyExc_ValueError,
-                        "Included ranges must not overlap or end before it starts");
+        PyErr_SetString(PyExc_ValueError, "Included ranges cannot overlap");
         PyMem_Free(ranges);
         return -1;
     }
 
     PyMem_Free(ranges);
     return 0;
 }
```

### Comparing `tree-sitter-0.22.0/tree_sitter/binding/query.c` & `tree-sitter-0.22.1/tree_sitter/binding/query.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/binding/range.c` & `tree-sitter-0.22.1/tree_sitter/binding/range.c`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,25 @@
         "start_point", "end_point", "start_byte", "end_byte", NULL,
     };
     if (!PyArg_ParseTupleAndKeywords(args, kwargs, "(II)(II)II:__init__", keywords, &start_row,
                                      &start_col, &end_row, &end_col, &start_byte, &end_byte)) {
         return -1;
     }
 
+    if (start_row > end_row || (start_row == end_row && start_col > end_col)) {
+        PyErr_Format(PyExc_ValueError, "Invalid point range: (%u, %u) to (%u, %u)", start_row,
+                     start_col, end_row, end_col);
+        return -1;
+    }
+
+    if (start_byte > end_byte) {
+        PyErr_Format(PyExc_ValueError, "Invalid byte range: %u to %u", start_byte, end_byte);
+        return -1;
+    }
+
     self->range.start_point.row = start_row;
     self->range.start_point.column = start_col;
     self->range.end_point.row = end_row;
     self->range.end_point.column = end_col;
     self->range.start_byte = start_byte;
     self->range.end_byte = end_byte;
```

### Comparing `tree-sitter-0.22.0/tree_sitter/binding/tree.c` & `tree-sitter-0.22.1/tree_sitter/binding/tree.c`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,17 @@
     if (!PyArg_ParseTuple(args, "I(II):root_node_with_offset", &offset_bytes, &offset_extent.row,
                           &offset_extent.column)) {
         return NULL;
     }
 
     ModuleState *state = GET_MODULE_STATE(self);
     TSNode node = ts_tree_root_node_with_offset(self->tree, offset_bytes, offset_extent);
+    if (ts_node_is_null(node)) {
+        Py_RETURN_NONE;
+    }
     return node_new_internal(state, node, (PyObject *)self);
 }
 
 PyObject *tree_walk(Tree *self, PyObject *Py_UNUSED(args)) {
     ModuleState *state = GET_MODULE_STATE(self);
     TreeCursor *tree_cursor = PyObject_New(TreeCursor, state->tree_cursor_type);
     if (tree_cursor == NULL) {
```

### Comparing `tree-sitter-0.22.0/tree_sitter/binding/tree_cursor.c` & `tree-sitter-0.22.1/tree_sitter/binding/tree_cursor.c`

 * *Files 1% similar despite different names*

```diff
@@ -104,42 +104,45 @@
 }
 
 PyObject *tree_cursor_goto_first_child_for_byte(TreeCursor *self, PyObject *args) {
     uint32_t byte;
     if (!PyArg_ParseTuple(args, "I:goto_first_child_for_byte", &byte)) {
         return NULL;
     }
+
     int64_t result = ts_tree_cursor_goto_first_child_for_byte(&self->cursor, byte);
-    if (result) {
-        Py_XDECREF(self->node);
-        self->node = NULL;
+    if (result == -1) {
+        Py_RETURN_FALSE;
     }
-    return PyBool_FromLong(result);
+    Py_XDECREF(self->node);
+    self->node = NULL;
+    Py_RETURN_TRUE;
 }
 
 PyObject *tree_cursor_goto_first_child_for_point(TreeCursor *self, PyObject *args) {
-    uint32_t row, column;
-    if (!PyArg_ParseTuple(args, "(II):goto_first_child_for_point", &row, &column)) {
-        if (PyArg_ParseTuple(args, "II:goto_first_child_for_point", &row, &column)) {
+    TSPoint point;
+    if (!PyArg_ParseTuple(args, "(II):goto_first_child_for_point", &point.row, &point.column)) {
+        if (PyArg_ParseTuple(args, "II:goto_first_child_for_point", &point.row, &point.column)) {
             PyErr_Clear();
             if (REPLACE("TreeCursor.goto_first_child_for_point(row, col)",
                         "TreeCursor.goto_first_child_for_point(point)") < 0) {
                 return NULL;
             }
         } else {
             return NULL;
         }
     }
-    int64_t result =
-        ts_tree_cursor_goto_first_child_for_point(&self->cursor, (TSPoint){row, column});
-    if (result) {
-        Py_XDECREF(self->node);
-        self->node = NULL;
+
+    int64_t result = ts_tree_cursor_goto_first_child_for_point(&self->cursor, point);
+    if (result == -1) {
+        Py_RETURN_FALSE;
     }
-    return PyBool_FromLong(result);
+    Py_XDECREF(self->node);
+    self->node = NULL;
+    Py_RETURN_TRUE;
 }
 
 PyObject *tree_cursor_reset(TreeCursor *self, PyObject *args) {
     ModuleState *state = GET_MODULE_STATE(self);
     PyObject *node_obj;
     if (!PyArg_ParseTuple(args, "O!:reset", state->node_type, &node_obj)) {
         return NULL;
```

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/include/tree_sitter/api.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/include/tree_sitter/api.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/alloc.c` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/alloc.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/alloc.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/alloc.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/array.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/array.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/atomic.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/atomic.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/clock.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/clock.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/get_changed_ranges.c` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/get_changed_ranges.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/get_changed_ranges.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/get_changed_ranges.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/host.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/host.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/language.c` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/language.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/language.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/language.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/length.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/length.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/lexer.c` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/lexer.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/lexer.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/lexer.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/node.c` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/node.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/parser.c` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/parser.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/parser.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/parser.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/point.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/point.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/query.c` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/query.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/reduce_action.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/reduce_action.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/reusable_node.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/reusable_node.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/stack.c` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/stack.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/stack.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/stack.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/subtree.c` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/subtree.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/subtree.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/subtree.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/tree.c` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/tree.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/tree.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/tree.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/tree_cursor.c` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/tree_cursor.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/tree_cursor.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/tree_cursor.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/LICENSE` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/README.md` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode/README.md`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/umachine.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode/umachine.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/utf16.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode/utf16.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/utf8.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode/utf8.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/unicode.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/wasm_store.c` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/wasm_store.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter/core/lib/src/wasm_store.h` & `tree-sitter-0.22.1/tree_sitter/core/lib/src/wasm_store.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.22.0/tree_sitter.egg-info/PKG-INFO` & `tree-sitter-0.22.1/tree_sitter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-sitter
-Version: 0.22.0
+Version: 0.22.1
 Summary: Python bindings to the Tree-sitter parsing library
 Author-email: Max Brunsfeld <maxbrunsfeld@gmail.com>
 Project-URL: Homepage, https://tree-sitter.github.io/tree-sitter/
 Project-URL: Source, https://github.com/tree-sitter/py-tree-sitter
 Project-URL: Documentation, https://tree-sitter.github.io/py-tree-sitter/
 Keywords: incremental,parsing,tree-sitter
 Classifier: Intended Audience :: Developers
@@ -63,16 +63,15 @@
 ```
 
 ### Basic parsing
 
 Create a `Parser` and configure it to use a language:
 
 ```python
-parser = Parser()
-parser.set_language(PY_LANGUAGE)
+parser = Parser(PY_LANGUAGE)
 ```
 
 Parse some source code:
 
 ```python
 tree = parser.parse(
     bytes(
@@ -157,15 +156,15 @@
 function_call_name_node = function_call_node.child_by_field_name("function")
 assert function_call_name_node.type == "identifier"
 
 function_call_args_node = function_call_node.child_by_field_name("arguments")
 assert function_call_args_node.type == "argument_list"
 
 
-assert root_node.sexp() == (
+assert str(root_node) == (
     "(module "
         "(function_definition "
             "name: (identifier) "
             "parameters: (parameters) "
             "body: (block "
                 "(if_statement "
                     "condition: (identifier) "
@@ -175,15 +174,15 @@
                             "arguments: (argument_list))))))))"
 )
 ```
 
 Or, to use the byte offset with UTF-16 encoding:
 
 ```python
-parser.set_language(JAVASCRIPT)
+parser.language = JAVASCRIPT
 source_code = bytes("'😎' && '🐍'", "utf16")
 
 def read(byte_position, _):
     return source_code[byte_position: byte_position + 2]
 
 tree = parser.parse(read, encoding="utf16")
 root_node = tree.root_node
```

### Comparing `tree-sitter-0.22.0/tree_sitter.egg-info/SOURCES.txt` & `tree-sitter-0.22.1/tree_sitter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

