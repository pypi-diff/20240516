# Comparing `tmp/visualgo-2024.5.15.tar.gz` & `tmp/visualgo-2024.5.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visualgo-2024.5.15.tar", last modified: Wed May 15 06:02:09 2024, max compression
+gzip compressed data, was "visualgo-2024.5.16.tar", last modified: Thu May 16 06:21:54 2024, max compression
```

## Comparing `visualgo-2024.5.15.tar` & `visualgo-2024.5.16.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.363858 visualgo-2024.5.15/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 06:02:01.000000 visualgo-2024.5.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 06:02:01.000000 visualgo-2024.5.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-15 06:02:09.363858 visualgo-2024.5.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-15 06:02:01.000000 visualgo-2024.5.15/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-15 06:02:01.000000 visualgo-2024.5.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:02:09.363858 visualgo-2024.5.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-15 06:02:01.000000 visualgo-2024.5.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.351858 visualgo-2024.5.15/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.355858 visualgo-2024.5.15/src/visualgo/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.355858 visualgo-2024.5.15/src/visualgo/logic/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25627 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/controller_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.355858 visualgo-2024.5.15/src/visualgo/logic/debugger/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.355858 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9242 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/bdb_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.359858 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_api/from_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_api/to_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.359858 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_impl/python_process_from_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_impl/python_process_to_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/py_debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.359858 visualgo-2024.5.15/src/visualgo/logic/static/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/static/static_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/static/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.359858 visualgo-2024.5.15/src/visualgo/logic/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/ui/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/ui/ui_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.363858 visualgo-2024.5.15/src/visualgo/structures/
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/Array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/BinaryTreeNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/BinaryTreeNodeBack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/DoublyLinkedList.py
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/Graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/LinkedList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/List.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/Node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/Queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/Set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/Stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/Tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/TreeNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/TwoWayNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.363858 visualgo-2024.5.15/src/visualgo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-15 06:02:09.000000 visualgo-2024.5.15/src/visualgo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-15 06:02:09.000000 visualgo-2024.5.15/src/visualgo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:02:09.000000 visualgo-2024.5.15/src/visualgo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 06:02:09.000000 visualgo-2024.5.15/src/visualgo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 06:02:09.000000 visualgo-2024.5.15/src/visualgo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:21:54.899174 visualgo-2024.5.16/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-16 06:21:45.000000 visualgo-2024.5.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 06:21:45.000000 visualgo-2024.5.16/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-16 06:21:54.899174 visualgo-2024.5.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-16 06:21:45.000000 visualgo-2024.5.16/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-16 06:21:45.000000 visualgo-2024.5.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 06:21:54.899174 visualgo-2024.5.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-16 06:21:45.000000 visualgo-2024.5.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:21:54.891174 visualgo-2024.5.16/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:21:54.891174 visualgo-2024.5.16/src/visualgo/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:21:54.891174 visualgo-2024.5.16/src/visualgo/logic/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25627 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/controller_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:21:54.895174 visualgo-2024.5.16/src/visualgo/logic/debugger/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/debugger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:21:54.895174 visualgo-2024.5.16/src/visualgo/logic/debugger/__private/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/debugger/__private/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9242 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/debugger/__private/bdb_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:21:54.895174 visualgo-2024.5.16/src/visualgo/logic/debugger/__private/comm_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/debugger/__private/comm_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/debugger/__private/comm_api/from_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/debugger/__private/comm_api/to_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:21:54.895174 visualgo-2024.5.16/src/visualgo/logic/debugger/__private/comm_impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/debugger/__private/comm_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/debugger/__private/comm_impl/python_process_from_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/debugger/__private/comm_impl/python_process_to_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/debugger/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/debugger/py_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/debugger/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:21:54.895174 visualgo-2024.5.16/src/visualgo/logic/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/static/static_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/static/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:21:54.895174 visualgo-2024.5.16/src/visualgo/logic/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/ui/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/logic/ui/ui_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:21:54.899174 visualgo-2024.5.16/src/visualgo/structures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/structures/Array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/structures/BinaryTreeNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/structures/BinaryTreeNodeBack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/structures/DoublyLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/structures/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/structures/LinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/structures/List.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/structures/Node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/structures/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/structures/Set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/structures/Stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/structures/Tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/structures/TreeNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/structures/TwoWayNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-16 06:21:45.000000 visualgo-2024.5.16/src/visualgo/structures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:21:54.899174 visualgo-2024.5.16/src/visualgo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-16 06:21:54.000000 visualgo-2024.5.16/src/visualgo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-16 06:21:54.000000 visualgo-2024.5.16/src/visualgo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 06:21:54.000000 visualgo-2024.5.16/src/visualgo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 06:21:54.000000 visualgo-2024.5.16/src/visualgo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 06:21:54.000000 visualgo-2024.5.16/src/visualgo.egg-info/top_level.txt
```

### Comparing `visualgo-2024.5.15/LICENSE` & `visualgo-2024.5.16/LICENSE`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/PKG-INFO` & `visualgo-2024.5.16/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualgo
-Version: 2024.5.15
+Version: 2024.5.16
 Summary: Enjoy classic datatypes and debug user python code
 Author: PFA-Visualgo
 License: MIT License
         
         Copyright (c) 2024 PFA-Visualgo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `visualgo-2024.5.15/pyproject.toml` & `visualgo-2024.5.16/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "visualgo"
-version = "2024.5.15"
+version = "2024.5.16"
 description = "Enjoy classic datatypes and debug user python code"
 readme = "README.md"
 authors = [{ name = "PFA-Visualgo" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `visualgo-2024.5.15/src/visualgo/logic/controller.py` & `visualgo-2024.5.16/src/visualgo/logic/controller.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/logic/controller_callbacks.py` & `visualgo-2024.5.16/src/visualgo/logic/controller_callbacks.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/logic/debugger/__private/bdb_layer.py` & `visualgo-2024.5.16/src/visualgo/logic/debugger/__private/bdb_layer.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_api/from_worker.py` & `visualgo-2024.5.16/src/visualgo/logic/debugger/__private/comm_api/from_worker.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_api/to_worker.py` & `visualgo-2024.5.16/src/visualgo/logic/debugger/__private/comm_api/to_worker.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_impl/python_process_from_worker.py` & `visualgo-2024.5.16/src/visualgo/logic/debugger/__private/comm_impl/python_process_from_worker.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_impl/python_process_to_worker.py` & `visualgo-2024.5.16/src/visualgo/logic/debugger/__private/comm_impl/python_process_to_worker.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/logic/debugger/debugger.py` & `visualgo-2024.5.16/src/visualgo/logic/debugger/debugger.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/logic/debugger/py_debugger.py` & `visualgo-2024.5.16/src/visualgo/logic/debugger/py_debugger.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/logic/debugger/types.py` & `visualgo-2024.5.16/src/visualgo/logic/debugger/types.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/logic/static/static_analysis.py` & `visualgo-2024.5.16/src/visualgo/logic/static/static_analysis.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/logic/ui/ui_callbacks.py` & `visualgo-2024.5.16/src/visualgo/logic/ui/ui_callbacks.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/structures/Array.py` & `visualgo-2024.5.16/src/visualgo/structures/Array.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/structures/BinaryTreeNode.py` & `visualgo-2024.5.16/src/visualgo/structures/BinaryTreeNode.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/structures/BinaryTreeNodeBack.py` & `visualgo-2024.5.16/src/visualgo/structures/BinaryTreeNodeBack.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/structures/DoublyLinkedList.py` & `visualgo-2024.5.16/src/visualgo/structures/DoublyLinkedList.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/structures/Graph.py` & `visualgo-2024.5.16/src/visualgo/structures/Graph.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/structures/LinkedList.py` & `visualgo-2024.5.16/src/visualgo/structures/LinkedList.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/structures/List.py` & `visualgo-2024.5.16/src/visualgo/structures/List.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/structures/Node.py` & `visualgo-2024.5.16/src/visualgo/structures/Node.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/structures/Queue.py` & `visualgo-2024.5.16/src/visualgo/structures/Queue.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/structures/Set.py` & `visualgo-2024.5.16/src/visualgo/structures/Set.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/structures/Stack.py` & `visualgo-2024.5.16/src/visualgo/structures/Stack.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/structures/Tree.py` & `visualgo-2024.5.16/src/visualgo/structures/Tree.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/structures/TreeNode.py` & `visualgo-2024.5.16/src/visualgo/structures/TreeNode.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/structures/TwoWayNode.py` & `visualgo-2024.5.16/src/visualgo/structures/TwoWayNode.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo/structures/__init__.py` & `visualgo-2024.5.16/src/visualgo/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.15/src/visualgo.egg-info/PKG-INFO` & `visualgo-2024.5.16/src/visualgo.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualgo
-Version: 2024.5.15
+Version: 2024.5.16
 Summary: Enjoy classic datatypes and debug user python code
 Author: PFA-Visualgo
 License: MIT License
         
         Copyright (c) 2024 PFA-Visualgo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `visualgo-2024.5.15/src/visualgo.egg-info/SOURCES.txt` & `visualgo-2024.5.16/src/visualgo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

