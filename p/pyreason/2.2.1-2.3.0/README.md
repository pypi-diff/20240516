# Comparing `tmp/pyreason-2.2.1.tar.gz` & `tmp/pyreason-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-2.2.1.tar", last modified: Thu Mar 28 14:48:25 2024, max compression
+gzip compressed data, was "pyreason-2.3.0.tar", last modified: Thu May 16 20:01:06 2024, max compression
```

## Comparing `pyreason-2.2.1.tar` & `pyreason-2.3.0.tar`

### file list

```diff
@@ -1,74 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.532416 pyreason-2.2.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1493 2024-03-28 14:48:21.000000 pyreason-2.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-28 14:48:21.000000 pyreason-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-03-28 14:48:25.532416 pyreason-2.2.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     3304 2024-03-28 14:48:21.000000 pyreason-2.2.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      135 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.524416 pyreason-2.2.1/pyreason/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1015 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.520416 pyreason-2.2.1/pyreason/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.524416 pyreason-2.2.1/pyreason/examples/hello-world/
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/examples/hello-world/friends_graph.graphml
--rwxr-xr-x   0 runner    (1001) docker     (127)    30372 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.524416 pyreason-2.2.1/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.524416 pyreason-2.2.1/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3398 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6555 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.524416 pyreason-2.2.1/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      431 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1356 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4655 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.524416 pyreason-2.2.1/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/facts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/facts/fact.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1011 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1011 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.528416 pyreason-2.2.1/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    98141 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/interpretation/interpretation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/interpretation/interpretation_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    99238 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/interpretation/interpretation_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.528416 pyreason-2.2.1/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1897 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.528416 pyreason-2.2.1/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.528416 pyreason-2.2.1/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6241 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6015 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4186 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2933 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10479 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4779 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.528416 pyreason-2.2.1/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2845 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.528416 pyreason-2.2.1/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1218 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/rules/rule.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1188 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/rules/rule_internal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.532416 pyreason-2.2.1/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4801 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4551 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3691 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2763 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/utils/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/utils/rule_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      834 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8756 2024-03-28 14:48:21.000000 pyreason-2.2.1/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.532416 pyreason-2.2.1/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-03-28 14:48:25.000000 pyreason-2.2.1/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-28 14:48:25.000000 pyreason-2.2.1/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:48:25.000000 pyreason-2.2.1/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 14:48:25.000000 pyreason-2.2.1/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-28 14:48:25.000000 pyreason-2.2.1/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 14:48:25.532416 pyreason-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-28 14:48:21.000000 pyreason-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:48:25.532416 pyreason-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-03-28 14:48:21.000000 pyreason-2.2.1/tests/test_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-03-28 14:48:21.000000 pyreason-2.2.1/tests/test_hello_world_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.427091 pyreason-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-16 20:01:02.000000 pyreason-2.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-16 20:01:02.000000 pyreason-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-16 20:01:06.427091 pyreason-2.3.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3553 2024-05-16 20:01:02.000000 pyreason-2.3.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      135 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.419091 pyreason-2.3.0/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1046 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.415090 pyreason-2.3.0/pyreason/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.419091 pyreason-2.3.0/pyreason/examples/hello-world/
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/examples/hello-world/friends_graph.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30431 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.423091 pyreason-2.3.0/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.423091 pyreason-2.3.0/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3398 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6555 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.423091 pyreason-2.3.0/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      431 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1356 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4655 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.423091 pyreason-2.3.0/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/facts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/facts/fact.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1011 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1011 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.423091 pyreason-2.3.0/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    98141 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/interpretation/interpretation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/interpretation/interpretation_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99238 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/interpretation/interpretation_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.423091 pyreason-2.3.0/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1897 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.423091 pyreason-2.3.0/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.427091 pyreason-2.3.0/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6241 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6015 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4186 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2933 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10479 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4779 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.427091 pyreason-2.3.0/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2845 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.427091 pyreason-2.3.0/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1166 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/rules/rule.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1188 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/rules/rule_internal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.427091 pyreason-2.3.0/pyreason/scripts/threshold/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/threshold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/threshold/threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.427091 pyreason-2.3.0/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4801 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4551 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3691 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2763 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/utils/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8324 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/utils/rule_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      834 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8756 2024-05-16 20:01:02.000000 pyreason-2.3.0/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.427091 pyreason-2.3.0/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-16 20:01:06.000000 pyreason-2.3.0/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-16 20:01:06.000000 pyreason-2.3.0/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:01:06.000000 pyreason-2.3.0/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-16 20:01:06.000000 pyreason-2.3.0/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 20:01:06.000000 pyreason-2.3.0/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:01:06.427091 pyreason-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-16 20:01:02.000000 pyreason-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:01:06.427091 pyreason-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-16 20:01:02.000000 pyreason-2.3.0/tests/test_custom_thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-16 20:01:02.000000 pyreason-2.3.0/tests/test_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-16 20:01:02.000000 pyreason-2.3.0/tests/test_hello_world_parallel.py
```

### Comparing `pyreason-2.2.1/PKG-INFO` & `pyreason-2.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,113 +1,73 @@
-Metadata-Version: 2.1
-Name: pyreason
-Version: 2.2.1
-Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
-Home-page: https://github.com/lab-v2/pyreason
-Author: Dyuman Aditya
-Author-email: dyuman.aditya@gmail.com
-License: BSD 3-clause
-Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
-Project-URL: Repository, https://github.com/lab-v2/pyreason
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: networkx
-Requires-Dist: pyyaml
-Requires-Dist: pandas
-Requires-Dist: numba
-Requires-Dist: numpy
-Requires-Dist: memory_profiler
-Requires-Dist: pytest
-
-# PyReason
 <img src="https://raw.githubusercontent.com/lab-v2/pyreason/main/media/pyreason_logo.jpg"/>
 
-[![Python Build](https://github.com/lab-v2/pyreason/actions/workflows/python-publish.yml/badge.svg)](https://github.com/lab-v2/pyreason/actions/workflows/python-publish.yml)
-[![Python version compatibility](https://github.com/lab-v2/pyreason/actions/workflows/python-package-version-test.yml/badge.svg)](https://github.com/lab-v2/pyreason/actions/workflows/python-package-version-test.yml)
+[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
+[![Documentation Status](https://readthedocs.org/projects/pyreason/badge/?version=latest)](https://pyreason.readthedocs.io/en/latest/?badge=latest)
+[![pypi](https://github.com/lab-v2/pyreason/actions/workflows/python-publish.yml/badge.svg)](https://github.com/lab-v2/pyreason/actions/workflows/python-publish.yml)
+[![Tests](https://github.com/lab-v2/pyreason/actions/workflows/python-package-version-test.yml/badge.svg)](https://github.com/lab-v2/pyreason/actions/workflows/python-package-version-test.yml)
+
 
 An explainable inference software supporting annotated, real valued, graph based and temporal logic.
 
 ## Links
 [📃 Paper](https://arxiv.org/abs/2302.13482)
 
 [📽️ Video](https://www.youtube.com/watch?v=E1PSl3KQCmo)
 
 [🌐 Website](https://neurosymbolic.asu.edu/pyreason/)
 
 [🏋️‍♂️ PyReason Gym](https://github.com/lab-v2/pyreason-gym)
 
-Check out the [PyReason Hello World](https://github.com/lab-v2/pyreason/blob/main/docs/hello-world.md) program if you're new, or want get get a feel for the software.
+[🗎 Documentation](https://pyreason.readthedocs.io/en/latest/)
+
+Check out the [PyReason Hello World](https://pyreason.readthedocs.io/en/latest/tutorials/Basic%20tutorial.html) program if you're new, or want get get a feel for the software.
 
 
 ## Table of Contents
   
 1. [Introduction](#1-introduction)
-2. [Install](#2-install)
-    * [Install as a Python Library](#21-install-as-a-python-library)
-    * [Install as a command line tool](#22-install-as-a-command-line-tool)
-3. [Usage](#3-usage)
-4. [Bibtex](#4-bibtex)
-5. [License](#5-license)
-6. [Contact](#6-contact)
+2. [Documentation](#2-documentation)
+3. [Install](#3-install)
+5. [Bibtex](#4-bibtex)
+6. [License](#5-license)
+7. [Contact](#6-contact)
 
 
 ## 1. Introduction
-PyReason makes use of 4 files:
+PyReason is a graphical inference tool that uses a set of logical rules and facts (initial conditions) to reason over graph structures. To get more details, refer to the paper/video/hello-world-example mentioned above.
 
-1. A GraphMl file containing the graph (required)
-2. A YAML file containing the pyreason rules (required)
-3. A YAML file containing the pyreason facts (optional but recommended)
-4. A YAML file containing the pyreason labels (optional but recommended)
-5. A YAML file containing the pyreason ipl (inconsistent predicate list) (optional)
+## 2. Documentation 
+All API documentation and code examples can be found on [ReadTheDocs](https://pyreason.readthedocs.io/en/latest/)
 
-The format of these files is very important. Please refer to the [example YAML files provided](https://github.com/lab-v2/pyreason/blob/main/pyreason/examples/example_yamls) when making your own rules/facts/labels/ipl. TODO: make doc for each format.
+## 3. Install
+PyReason can be installed as a python library using
 
-## 2. Install
-PyReason can be installed as a python library (recommended) or as a command line tool
-
-## 2.1 Install as a Python Library
-We import pyreason to initialize it for the first time, this may take a few minutes
 ```bash
 pip install pyreason
-python
-import pyreason
 ```
-
-## 2.2 Install as a Command Line Tool
-
-```bash
-git clone https://github.com/lab-v2/pyreason
-cd pyreason
-pip install -r requirements.txt
-python initialize.py
-```
-
-## 3. Usage
-Please refer to the documentation that is relevant to you
-1. [Usage as Python Library](https://github.com/lab-v2/pyreason/blob/main/docs/pyreason_library.md)
-2. [Usage as a Command Line Tool](https://github.com/lab-v2/pyreason/blob/main/docs/pyreason_cmd_line.md)
+The Python versions that are currently supported are `3.7`, `3.8`, `3.9`, `3.10`. If you want multi-core parallel support only `3.9` and `3.10` versions work due to limited numba support.
 
 ## 4. Bibtex
 If you used this software in your work please cite our paper
 
 Bibtex:
 ```
 @inproceedings{aditya_pyreason_2023,
 title = {{PyReason}: Software for Open World Temporal Logic},
 booktitle = {{AAAI} Spring Symposium},
 author = {Aditya, Dyuman and Mukherji, Kaustuv and Balasubramanian, Srikar and Chaudhary, Abhiraj and Shakarian, Paulo},
 year = {2023}}
 ```
 
 ## 5. License
-This repository is licensed under [BSD-3-Clause](https://github.com/lab-v2/pyreason/blob/main/LICENSE.md)
+This repository is licensed under [BSD-2-Clause](https://github.com/lab-v2/pyreason/blob/main/LICENSE.md).
+
+Trademark Permission PyReason™ and PyReason Design Logo <img src="https://raw.githubusercontent.com/lab-v2/pyreason/main/media/pyreason_logo.jpg" width="50"/>™ are trademarks of the Arizona Board of Regents/Arizona State University. Users of the software are permitted to use PyReason™ in association with the software for any purpose, provided such use is related to the software (e.g., Powered by PyReason™). Additionally, educational institutions are permitted to use the PyReason Design Logo <img src="https://raw.githubusercontent.com/lab-v2/pyreason/main/media/pyreason_logo.jpg" width="50"/>™ for non-commercial purposes.
+
 
 ## 6. Contact
 Dyuman Aditya - dyuman.aditya@asu.edu
 
 Kaustuv Mukherji - kmukher2@asu.edu
 
 Paulo Shakarian - pshak02@asu.edu
```

### Comparing `pyreason-2.2.1/pyreason/__init__.py` & `pyreason-2.3.0/pyreason/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,11 +19,14 @@
 
     settings.verbose = False
     load_graphml(graph_path)
     add_rule(Rule('popular(x) <-1 popular(y), Friends(x,y), owns(y,z), owns(x,z)', 'popular_rule'))
     add_fact(Fact('popular-fact', 'Mary', 'popular', [1, 1], 0, 2))
     reason(timesteps=2)
 
+    reset()
+    reset_rules()
+
     # Update cache status
     cache_status['initialized'] = True
     with open(cache_status_path, 'w') as file:
         yaml.dump(cache_status, file)
```

### Comparing `pyreason-2.2.1/pyreason/examples/hello-world/friends_graph.graphml` & `pyreason-2.3.0/pyreason/examples/hello-world/friends_graph.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/pyreason.py` & `pyreason-2.3.0/pyreason/pyreason.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from pyreason.scripts.utils.graphml_parser import GraphmlParser
 import pyreason.scripts.utils.yaml_parser as yaml_parser
 import pyreason.scripts.utils.rule_parser as rule_parser
 import pyreason.scripts.numba_wrapper.numba_types.label_type as label
 import pyreason.scripts.numba_wrapper.numba_types.rule_type as rule
 from pyreason.scripts.facts.fact import Fact
 from pyreason.scripts.rules.rule import Rule
+from pyreason.scripts.threshold.threshold import Threshold
 import pyreason.scripts.numba_wrapper.numba_types.fact_node_type as fact_node
 import pyreason.scripts.numba_wrapper.numba_types.fact_edge_type as fact_edge
 import pyreason.scripts.numba_wrapper.numba_types.interval_type as interval
 
 
 # USER VARIABLES
 class _Settings:
```

### Comparing `pyreason-2.2.1/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-2.3.0/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/args.py` & `pyreason-2.3.0/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/components/world.py` & `pyreason-2.3.0/pyreason/scripts/components/world.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/diffuse.py` & `pyreason-2.3.0/pyreason/scripts/diffuse.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/facts/fact.py` & `pyreason-2.3.0/pyreason/scripts/facts/fact.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/facts/fact_edge.py` & `pyreason-2.3.0/pyreason/scripts/facts/fact_edge.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/facts/fact_node.py` & `pyreason-2.3.0/pyreason/scripts/facts/fact_node.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/interpretation/interpretation.py` & `pyreason-2.3.0/pyreason/scripts/interpretation/interpretation.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/interpretation/interpretation_dict.py` & `pyreason-2.3.0/pyreason/scripts/interpretation/interpretation_dict.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/interpretation/interpretation_parallel.py` & `pyreason-2.3.0/pyreason/scripts/interpretation/interpretation_parallel.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/interval/interval.py` & `pyreason-2.3.0/pyreason/scripts/interval/interval.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-2.3.0/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-2.3.0/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-2.3.0/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-2.3.0/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-2.3.0/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-2.3.0/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/program/program.py` & `pyreason-2.3.0/pyreason/scripts/program/program.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/rules/rule.py` & `pyreason-2.3.0/pyreason/scripts/rules/rule.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 
 class Rule:
     """
     Example text:
             `'pred1(x,y) : [0.2, 1] <- pred2(a, b) : [1,1], pred3(b, c)'`
 
-    1. It is not possible to specify thresholds. Threshold is greater than or equal to 1 by default
-    2. It is not possible to have weights for different clauses. Weights are 1 by default with bias 0
-    TODO: Add threshold class where we can pass this as a parameter
+    1. It is not possible to have weights for different clauses. Weights are 1 by default with bias 0
     TODO: Add weights as a parameter
     """
-    def __init__(self, rule_text: str, name: str, infer_edges: bool = False, set_static: bool = False, immediate_rule: bool = False):
+    def __init__(self, rule_text: str, name: str, infer_edges: bool = False, set_static: bool = False, immediate_rule: bool = False, custom_thresholds=None):
         """
         :param rule_text: The rule in text format
         :param name: The name of the rule. This will appear in the rule trace
         :param infer_edges: Whether to infer new edges after edge rule fires
         :param set_static: Whether to set the atom in the head as static if the rule fires. The bounds will no longer change
         :param immediate_rule: Whether the rule is immediate. Immediate rules check for more applicable rules immediately after being applied
         """
-        self.rule = rule_parser.parse_rule(rule_text, name, infer_edges, set_static, immediate_rule)
+        if custom_thresholds is None:
+            custom_thresholds = []
+        self.rule = rule_parser.parse_rule(rule_text, name, custom_thresholds, infer_edges, set_static, immediate_rule)
```

### Comparing `pyreason-2.2.1/pyreason/scripts/rules/rule_internal.py` & `pyreason-2.3.0/pyreason/scripts/rules/rule_internal.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/utils/filter.py` & `pyreason-2.3.0/pyreason/scripts/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/utils/graphml_parser.py` & `pyreason-2.3.0/pyreason/scripts/utils/graphml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/utils/output.py` & `pyreason-2.3.0/pyreason/scripts/utils/output.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/utils/plotter.py` & `pyreason-2.3.0/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/utils/rule_parser.py` & `pyreason-2.3.0/pyreason/scripts/utils/rule_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 
 import pyreason.scripts.numba_wrapper.numba_types.rule_type as rule
 import pyreason.scripts.numba_wrapper.numba_types.label_type as label
 import pyreason.scripts.numba_wrapper.numba_types.interval_type as interval
 
 
-def parse_rule(rule_text: str, name: str, infer_edges: bool = False, set_static: bool = False, immediate_rule: bool = False) -> rule.Rule:
+def parse_rule(rule_text: str, name: str, custom_thresholds: list, infer_edges: bool = False, set_static: bool = False, immediate_rule: bool = False) -> rule.Rule:
     # First remove all spaces from line
     r = rule_text.replace(' ', '')
 
     # Separate into head and body
     head, body = r.split('<-')
 
     # Extract delta_t of rule if it exists else set it to 0
@@ -148,33 +148,43 @@
 
     # Array of thresholds to keep track of for each neighbor criterion. Form [(comparison, (number/percent, total/available), thresh)]
     thresholds = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, numba.types.UniTuple(numba.types.string, 2), numba.types.float64)))
 
     # Array to store clauses for nodes: node/edge, [subset]/[subset1, subset2], label, interval, operator
     clauses = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, label.label_type, numba.types.ListType(numba.types.string), interval.interval_type, numba.types.string)))
 
-    # Loop though clauses
+    # gather count of clauses for threshold validation
+    num_clauses = len(body_clauses)
+
+    if custom_thresholds and (len(custom_thresholds) != num_clauses):
+        raise Exception('The length of custom thresholds {} is not equal to number of clauses {}'
+                        .format(len(custom_thresholds), num_clauses))
+    
+    # If no custom thresholds provided, use defaults
+    # otherwise loop through user-defined thresholds and convert to numba compatible format
+    if not custom_thresholds:
+        for _ in range(num_clauses):
+            thresholds.append(('greater_equal', ('number', 'total'), 1.0))
+    else:  
+        for threshold in custom_thresholds:  
+            thresholds.append(threshold.to_tuple())
+
+    # # Loop though clauses
     for body_clause, predicate, variables, bounds in zip(body_clauses, body_predicates, body_variables, body_bounds):
         # Neigh criteria
         clause_type = 'node' if len(variables) == 1 else 'edge'
         op = _get_operator_from_clause(body_clause)
         if op:
             clause_type = 'comparison'
 
         subset = numba.typed.List(variables)
         l = label.Label(predicate)
         bnd = interval.closed(bounds[0], bounds[1])
         clauses.append((clause_type, l, subset, bnd, op))
 
-        # Threshold.
-        quantifier = 'greater_equal'
-        quantifier_type = ('number', 'total')
-        thresh = 1
-        thresholds.append((quantifier, quantifier_type, thresh))
-
     # Assert that there are two variables in the head of the rule if we infer edges
     # Add edges between head variables if necessary
     if infer_edges:
         var = '__target' if head_variables[0] == head_variables[1] else head_variables[1]
         edges = ('__target', var, target)
     else:
         edges = ('', '', label.Label(''))
```

### Comparing `pyreason-2.2.1/pyreason/scripts/utils/visuals.py` & `pyreason-2.3.0/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason/scripts/utils/yaml_parser.py` & `pyreason-2.3.0/pyreason/scripts/utils/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-2.2.1/pyreason.egg-info/PKG-INFO` & `pyreason-2.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 2.2.1
+Version: 2.3.0
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
@@ -18,96 +18,80 @@
 Requires-Dist: pyyaml
 Requires-Dist: pandas
 Requires-Dist: numba
 Requires-Dist: numpy
 Requires-Dist: memory_profiler
 Requires-Dist: pytest
 
-# PyReason
 <img src="https://raw.githubusercontent.com/lab-v2/pyreason/main/media/pyreason_logo.jpg"/>
 
-[![Python Build](https://github.com/lab-v2/pyreason/actions/workflows/python-publish.yml/badge.svg)](https://github.com/lab-v2/pyreason/actions/workflows/python-publish.yml)
-[![Python version compatibility](https://github.com/lab-v2/pyreason/actions/workflows/python-package-version-test.yml/badge.svg)](https://github.com/lab-v2/pyreason/actions/workflows/python-package-version-test.yml)
+[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
+[![Documentation Status](https://readthedocs.org/projects/pyreason/badge/?version=latest)](https://pyreason.readthedocs.io/en/latest/?badge=latest)
+[![pypi](https://github.com/lab-v2/pyreason/actions/workflows/python-publish.yml/badge.svg)](https://github.com/lab-v2/pyreason/actions/workflows/python-publish.yml)
+[![Tests](https://github.com/lab-v2/pyreason/actions/workflows/python-package-version-test.yml/badge.svg)](https://github.com/lab-v2/pyreason/actions/workflows/python-package-version-test.yml)
+
 
 An explainable inference software supporting annotated, real valued, graph based and temporal logic.
 
 ## Links
 [📃 Paper](https://arxiv.org/abs/2302.13482)
 
 [📽️ Video](https://www.youtube.com/watch?v=E1PSl3KQCmo)
 
 [🌐 Website](https://neurosymbolic.asu.edu/pyreason/)
 
 [🏋️‍♂️ PyReason Gym](https://github.com/lab-v2/pyreason-gym)
 
-Check out the [PyReason Hello World](https://github.com/lab-v2/pyreason/blob/main/docs/hello-world.md) program if you're new, or want get get a feel for the software.
+[🗎 Documentation](https://pyreason.readthedocs.io/en/latest/)
+
+Check out the [PyReason Hello World](https://pyreason.readthedocs.io/en/latest/tutorials/Basic%20tutorial.html) program if you're new, or want get get a feel for the software.
 
 
 ## Table of Contents
   
 1. [Introduction](#1-introduction)
-2. [Install](#2-install)
-    * [Install as a Python Library](#21-install-as-a-python-library)
-    * [Install as a command line tool](#22-install-as-a-command-line-tool)
-3. [Usage](#3-usage)
-4. [Bibtex](#4-bibtex)
-5. [License](#5-license)
-6. [Contact](#6-contact)
+2. [Documentation](#2-documentation)
+3. [Install](#3-install)
+5. [Bibtex](#4-bibtex)
+6. [License](#5-license)
+7. [Contact](#6-contact)
 
 
 ## 1. Introduction
-PyReason makes use of 4 files:
-
-1. A GraphMl file containing the graph (required)
-2. A YAML file containing the pyreason rules (required)
-3. A YAML file containing the pyreason facts (optional but recommended)
-4. A YAML file containing the pyreason labels (optional but recommended)
-5. A YAML file containing the pyreason ipl (inconsistent predicate list) (optional)
+PyReason is a graphical inference tool that uses a set of logical rules and facts (initial conditions) to reason over graph structures. To get more details, refer to the paper/video/hello-world-example mentioned above.
 
-The format of these files is very important. Please refer to the [example YAML files provided](https://github.com/lab-v2/pyreason/blob/main/pyreason/examples/example_yamls) when making your own rules/facts/labels/ipl. TODO: make doc for each format.
+## 2. Documentation 
+All API documentation and code examples can be found on [ReadTheDocs](https://pyreason.readthedocs.io/en/latest/)
 
-## 2. Install
-PyReason can be installed as a python library (recommended) or as a command line tool
+## 3. Install
+PyReason can be installed as a python library using
 
-## 2.1 Install as a Python Library
-We import pyreason to initialize it for the first time, this may take a few minutes
 ```bash
 pip install pyreason
-python
-import pyreason
-```
-
-## 2.2 Install as a Command Line Tool
-
-```bash
-git clone https://github.com/lab-v2/pyreason
-cd pyreason
-pip install -r requirements.txt
-python initialize.py
 ```
-
-## 3. Usage
-Please refer to the documentation that is relevant to you
-1. [Usage as Python Library](https://github.com/lab-v2/pyreason/blob/main/docs/pyreason_library.md)
-2. [Usage as a Command Line Tool](https://github.com/lab-v2/pyreason/blob/main/docs/pyreason_cmd_line.md)
+The Python versions that are currently supported are `3.7`, `3.8`, `3.9`, `3.10`. If you want multi-core parallel support only `3.9` and `3.10` versions work due to limited numba support.
 
 ## 4. Bibtex
 If you used this software in your work please cite our paper
 
 Bibtex:
 ```
 @inproceedings{aditya_pyreason_2023,
 title = {{PyReason}: Software for Open World Temporal Logic},
 booktitle = {{AAAI} Spring Symposium},
 author = {Aditya, Dyuman and Mukherji, Kaustuv and Balasubramanian, Srikar and Chaudhary, Abhiraj and Shakarian, Paulo},
 year = {2023}}
 ```
 
 ## 5. License
-This repository is licensed under [BSD-3-Clause](https://github.com/lab-v2/pyreason/blob/main/LICENSE.md)
+This repository is licensed under [BSD-2-Clause](https://github.com/lab-v2/pyreason/blob/main/LICENSE.md).
+
+Trademark Permission PyReason™ and PyReason Design Logo <img src="https://raw.githubusercontent.com/lab-v2/pyreason/main/media/pyreason_logo.jpg" width="50"/>™ are trademarks of the Arizona Board of Regents/Arizona State University. Users of the software are permitted to use PyReason™ in association with the software for any purpose, provided such use is related to the software (e.g., Powered by PyReason™). Additionally, educational institutions are permitted to use the PyReason Design Logo <img src="https://raw.githubusercontent.com/lab-v2/pyreason/main/media/pyreason_logo.jpg" width="50"/>™ for non-commercial purposes.
+
 
 ## 6. Contact
 Dyuman Aditya - dyuman.aditya@asu.edu
 
 Kaustuv Mukherji - kmukher2@asu.edu
 
 Paulo Shakarian - pshak02@asu.edu
```

### Comparing `pyreason-2.2.1/pyreason.egg-info/SOURCES.txt` & `pyreason-2.3.0/pyreason.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -39,17 +39,20 @@
 pyreason/scripts/numba_wrapper/numba_types/rule_type.py
 pyreason/scripts/numba_wrapper/numba_types/world_type.py
 pyreason/scripts/program/__init__.py
 pyreason/scripts/program/program.py
 pyreason/scripts/rules/__init__.py
 pyreason/scripts/rules/rule.py
 pyreason/scripts/rules/rule_internal.py
+pyreason/scripts/threshold/__init__.py
+pyreason/scripts/threshold/threshold.py
 pyreason/scripts/utils/__init__.py
 pyreason/scripts/utils/filter.py
 pyreason/scripts/utils/graphml_parser.py
 pyreason/scripts/utils/output.py
 pyreason/scripts/utils/plotter.py
 pyreason/scripts/utils/rule_parser.py
 pyreason/scripts/utils/visuals.py
 pyreason/scripts/utils/yaml_parser.py
+tests/test_custom_thresholds.py
 tests/test_hello_world.py
 tests/test_hello_world_parallel.py
```

### Comparing `pyreason-2.2.1/setup.py` & `pyreason-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pyreason',
-    version='2.2.1',
+    version='2.3.0',
     author='Dyuman Aditya',
     author_email='dyuman.aditya@gmail.com',
     description='An explainable inference software supporting annotated, real valued, graph based and temporal logic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/lab-v2/pyreason',
     license='BSD 3-clause',
```

### Comparing `pyreason-2.2.1/tests/test_hello_world.py` & `pyreason-2.3.0/tests/test_hello_world.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Test if the simple hello world program works
 import pyreason as pr
 
 
 def test_hello_world():
+    # Reset PyReason
+    pr.reset()
+    pr.reset_rules()
+
     # Modify the paths based on where you've stored the files we made above
     graph_path = './tests/friends_graph.graphml'
 
     # Modify pyreason settings to make verbose and to save the rule trace to a file
     pr.settings.verbose = True     # Print info to screen
 
     # Load all the files into pyreason
```

### Comparing `pyreason-2.2.1/tests/test_hello_world_parallel.py` & `pyreason-2.3.0/tests/test_hello_world_parallel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Test if the simple hello world program works
 import pyreason as pr
 
 
 def test_hello_world_parallel():
+    # Reset PyReason
+    pr.reset()
+    pr.reset_rules()
+
     # Modify the paths based on where you've stored the files we made above
     graph_path = './tests/friends_graph.graphml'
 
     # Modify pyreason settings to make verbose and to save the rule trace to a file
     pr.settings.verbose = True     # Print info to screen
     pr.settings.parallel_computing = True
```

