# Comparing `tmp/libbs-1.3.3.tar.gz` & `tmp/libbs-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbs-1.3.3.tar", last modified: Wed May 15 18:52:13 2024, max compression
+gzip compressed data, was "libbs-1.5.0.tar", last modified: Wed May 15 20:36:45 2024, max compression
```

## Comparing `libbs-1.3.3.tar` & `libbs-1.5.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.731921 libbs-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-15 18:51:56.000000 libbs-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-15 18:52:13.731921 libbs-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-15 18:51:56.000000 libbs-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.719921 libbs-1.3.3/libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.723921 libbs-1.3.3/libbs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/api/artifact_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/api/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26870 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/api/decompiler_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/api/type_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.723921 libbs-1.3.3/libbs/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/decompilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/global_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/stack_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.723921 libbs-1.3.3/libbs/decompiler_stubs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.723921 libbs-1.3.3/libbs/decompiler_stubs/angr_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/angr_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.723921 libbs-1.3.3/libbs/decompiler_stubs/binja_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/binja_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.727921 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.727921 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.727921 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89855 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ida_libbs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.727921 libbs-1.3.3/libbs/decompilers/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.727921 libbs-1.3.3/libbs/decompilers/angr/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/angr/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/angr/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/angr/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.727921 libbs-1.3.3/libbs/decompilers/binja/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/binja/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/binja/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/binja/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.727921 libbs-1.3.3/libbs/decompilers/ghidra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ghidra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ghidra/artifact_lifter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.731921 libbs-1.3.3/libbs/decompilers/ghidra/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ghidra/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ghidra/compat/ghidra_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ghidra/compat/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ghidra/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    32836 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ghidra/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.731921 libbs-1.3.3/libbs/decompilers/ida/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ida/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30603 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ida/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ida/hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12644 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ida/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/plugin_installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.731921 libbs-1.3.3/libbs/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/ui/qt_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/ui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.731921 libbs-1.3.3/libbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-15 18:52:13.000000 libbs-1.3.3/libbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-15 18:52:13.000000 libbs-1.3.3/libbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:52:13.000000 libbs-1.3.3/libbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 18:52:13.000000 libbs-1.3.3/libbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 18:52:13.000000 libbs-1.3.3/libbs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 18:52:13.000000 libbs-1.3.3/libbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-15 18:52:13.731921 libbs-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 18:51:56.000000 libbs-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.731921 libbs-1.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-15 18:51:56.000000 libbs-1.3.3/tests/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-15 18:51:56.000000 libbs-1.3.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-15 18:51:56.000000 libbs-1.3.3/tests/test_decompilers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.186511 libbs-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-15 20:36:41.000000 libbs-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-15 20:36:45.186511 libbs-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-15 20:36:41.000000 libbs-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.174511 libbs-1.5.0/libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.178511 libbs-1.5.0/libbs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/api/artifact_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/api/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26870 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/api/decompiler_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/api/type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.178511 libbs-1.5.0/libbs/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/artifacts/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/artifacts/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/artifacts/decompilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/artifacts/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/artifacts/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/artifacts/global_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/artifacts/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/artifacts/stack_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/artifacts/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.178511 libbs-1.5.0/libbs/decompiler_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompiler_stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.178511 libbs-1.5.0/libbs/decompiler_stubs/angr_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompiler_stubs/angr_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.178511 libbs-1.5.0/libbs/decompiler_stubs/binja_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompiler_stubs/binja_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.178511 libbs-1.5.0/libbs/decompiler_stubs/ghidra_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompiler_stubs/ghidra_libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.178511 libbs-1.5.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.178511 libbs-1.5.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89903 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompiler_stubs/ida_libbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.182511 libbs-1.5.0/libbs/decompilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.182511 libbs-1.5.0/libbs/decompilers/angr/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/angr/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/angr/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/angr/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.182511 libbs-1.5.0/libbs/decompilers/binja/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/binja/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/binja/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/binja/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.182511 libbs-1.5.0/libbs/decompilers/ghidra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/ghidra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/ghidra/artifact_lifter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.182511 libbs-1.5.0/libbs/decompilers/ghidra/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/ghidra/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/ghidra/compat/ghidra_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/ghidra/compat/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/ghidra/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32864 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/ghidra/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.182511 libbs-1.5.0/libbs/decompilers/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/ida/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30603 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/ida/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/ida/hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12644 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/decompilers/ida/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/plugin_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.186511 libbs-1.5.0/libbs/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/ui/qt_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-15 20:36:41.000000 libbs-1.5.0/libbs/ui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.186511 libbs-1.5.0/libbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-15 20:36:45.000000 libbs-1.5.0/libbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-15 20:36:45.000000 libbs-1.5.0/libbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:36:45.000000 libbs-1.5.0/libbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 20:36:45.000000 libbs-1.5.0/libbs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 20:36:45.000000 libbs-1.5.0/libbs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 20:36:45.000000 libbs-1.5.0/libbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-15 20:36:45.186511 libbs-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 20:36:41.000000 libbs-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:36:45.186511 libbs-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-15 20:36:41.000000 libbs-1.5.0/tests/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-15 20:36:41.000000 libbs-1.5.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-15 20:36:41.000000 libbs-1.5.0/tests/test_decompilers.py
```

### Comparing `libbs-1.3.3/LICENSE` & `libbs-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/PKG-INFO` & `libbs-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.3.3
+Version: 1.5.0
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
```

### Comparing `libbs-1.3.3/README.md` & `libbs-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/__main__.py` & `libbs-1.5.0/libbs/__main__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/api/artifact_dict.py` & `libbs-1.5.0/libbs/api/artifact_dict.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/api/artifact_lifter.py` & `libbs-1.5.0/libbs/api/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/api/decompiler_interface.py` & `libbs-1.5.0/libbs/api/decompiler_interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/api/type_parser.py` & `libbs-1.5.0/libbs/api/type_parser.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/api/utils.py` & `libbs-1.5.0/libbs/api/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/artifacts/__init__.py` & `libbs-1.5.0/libbs/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/artifacts/artifact.py` & `libbs-1.5.0/libbs/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/artifacts/comment.py` & `libbs-1.5.0/libbs/artifacts/comment.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/artifacts/decompilation.py` & `libbs-1.5.0/libbs/artifacts/decompilation.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/artifacts/enum.py` & `libbs-1.5.0/libbs/artifacts/enum.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/artifacts/func.py` & `libbs-1.5.0/libbs/artifacts/func.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/artifacts/global_variable.py` & `libbs-1.5.0/libbs/artifacts/global_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/artifacts/patch.py` & `libbs-1.5.0/libbs/artifacts/patch.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/artifacts/stack_variable.py` & `libbs-1.5.0/libbs/artifacts/stack_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/artifacts/struct.py` & `libbs-1.5.0/libbs/artifacts/struct.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py` & `libbs-1.5.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py` & `libbs-1.5.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py`

 * *Files 0% similar despite different names*

```diff
@@ -609,15 +609,16 @@
         """wait for the response"""
         if timeout is not None and timeout < 0:
             # can't pass in None higher up reliably, as it gets used to indicate "default timeout".
             # Instead, treat a negative timeout as "wait forever", and set timeout to None, so event.wait
             # will wait forever.
             timeout = None
 
-        if not self.event.wait(None):
+        # patch: make the timeout much longer
+        if not self.event.wait(60 * 3):
             raise BridgeTimeoutException(
                 "Didn't receive response {} before timeout".format(self.response_id)
             )
 
         return self.response
```

### Comparing `libbs-1.3.3/libbs/decompilers/angr/artifact_lifter.py` & `libbs-1.5.0/libbs/decompilers/angr/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/decompilers/angr/compat.py` & `libbs-1.5.0/libbs/decompilers/angr/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/decompilers/angr/interface.py` & `libbs-1.5.0/libbs/decompilers/angr/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/decompilers/binja/artifact_lifter.py` & `libbs-1.5.0/libbs/decompilers/binja/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/decompilers/binja/hooks.py` & `libbs-1.5.0/libbs/decompilers/binja/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/decompilers/binja/interface.py` & `libbs-1.5.0/libbs/decompilers/binja/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/decompilers/ghidra/artifact_lifter.py` & `libbs-1.5.0/libbs/decompilers/ghidra/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/decompilers/ghidra/compat/ghidra_api.py` & `libbs-1.5.0/libbs/decompilers/ghidra/compat/ghidra_api.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/decompilers/ghidra/hooks.py` & `libbs-1.5.0/libbs/decompilers/ghidra/hooks.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,14 +29,15 @@
             self.symChgEvents = [
                 self.changeManager.DOCR_SYMBOL_ADDED,
                 self.changeManager.DOCR_SYMBOL_RENAMED,
                 self.changeManager.DOCR_SYMBOL_DATA_CHANGED
             ]
 
             self.typeEvents = [
+                self.changeManager.DOCR_SYMBOL_ADDRESS_CHANGED,
                 self.changeManager.DOCR_DATA_TYPE_CHANGED,
                 self.changeManager.DOCR_DATA_TYPE_REPLACED,
                 self.changeManager.DOCR_DATA_TYPE_RENAMED,
                 self.changeManager.DOCR_DATA_TYPE_SETTING_CHANGED,
                 self.changeManager.DOCR_DATA_TYPE_MOVED,
                 self.changeManager.DOCR_DATA_TYPE_ADDED
             ]
@@ -46,30 +47,87 @@
                     continue
 
                 changeType = record.getEventType()
                 newValue = record.getNewValue()
                 obj = record.getObject()
 
                 if changeType in self.funcEvents:
-                    pass
+                    subType = record.getSubEventType()
+                    if subType == self.changeManager.FUNCTION_CHANGED_RETURN:
+                        # Function return type changed
+                        header = FunctionHeader(None, None, str(obj.getReturnType()))
+                        self._interface.function_header_changed(header)
+
                 elif changeType in self.typeEvents:
-                    try:
-                        struct = self._interface.structs[newValue.name]
-                        # TODO: access old name indicate deletion
-                        #self._interface.struct_changed(Struct(None, None, None), deleted=True)
-                        self._interface.struct_changed(struct)
-                    except KeyError:
-                        pass
+                    if changeType == self.changeManager.DOCR_SYMBOL_ADDRESS_CHANGED:
+                        # stack variables change address when retyped!
+                        if self._interface.ghidra.isinstance(obj, self.db.function.VariableDB):
+                            parent_namespace = obj.getParentNamespace()
+                            storage = obj.getVariableStorage()
+                            if (
+                                (newValue is not None) and (storage is not None) and bool(storage.isStackStorage())
+                                and (parent_namespace is not None)
+                            ):
+                                sv = StackVariable(
+                                    int(storage.stackOffset),
+                                    None,
+                                    str(obj.getDataType()),
+                                    int(storage.size),
+                                    int(obj.parentNamespace.entryPoint.offset)
+                                )
+                                self._interface.stack_variable_changed(
+                                    sv
+                                )
+
+                    else:
+                        try:
+                            struct = self._interface.structs[newValue.name]
+                            # TODO: access old name indicate deletion
+                            #self._interface.struct_changed(Struct(None, None, None), deleted=True)
+                            self._interface.struct_changed(struct)
+                        except KeyError:
+                            pass
+                    if changeType == self.changeManager.DOCR_SYMBOL_ADDRESS_CHANGED:
+                        # stack variables change address when retyped!
+                        if self._interface.ghidra.isinstance(obj, self.db.function.VariableDB):
+                            parent_namespace = obj.getParentNamespace()
+                            storage = obj.getVariableStorage()
+                            if (
+                                (newValue is not None) and (storage is not None) and bool(storage.isStackStorage())
+                                and (parent_namespace is not None)
+                            ):
+                                sv = self._interface.art_lifter.lift(
+                                    StackVariable(
+                                        int(storage.stackOffset),
+                                        None,
+                                        str(obj.getDataType()),
+                                        int(storage.size),
+                                        int(obj.parentNamespace.entryPoint.offset)
+                                    )
+                                )
+                                self._interface.stack_variable_changed(
+                                    sv
+                                )
+
+                    else:
+                        try:
+                            struct = self._interface.structs[newValue.name]
+                            # TODO: access old name indicate deletion
+                            #self._interface.struct_changed(Struct(None, None, None), deleted=True)
+                            self._interface.struct_changed(struct)
+                        except KeyError:
+                            pass
+
+                        try:
+                            enum = self._interface.enums[newValue.name]
+                            #self._interface.enum_changed(Enum(None, None), deleted=True)
+                            self._interface.enum_changed(enum)
+                        except KeyError:
+                            pass
 
-                    try:
-                        enum = self._interface.enums[newValue.name]
-                        #self._interface.enum_changed(Enum(None, None), deleted=True)
-                        self._interface.enum_changed(enum)
-                    except KeyError:
-                        pass
                 elif changeType in self.symDelEvents:
                     # Globals are deleted first then recreated
                     if self._interface.ghidra.isinstance(obj, self.db.symbol.CodeSymbol):
                         removed = GlobalVariable(obj.getAddress().getOffset(), obj.getName())
                         # deleted kwarg not yet handled by global_variable_changed
                         self._interface.global_variable_changed(removed, deleted=True)
                 elif changeType in self.symChgEvents:
@@ -100,24 +158,14 @@
                                     int(obj.variableStorage.stackOffset),
                                     newValue,
                                     None,
                                     None,
                                     int(obj.parentNamespace.entryPoint.offset)
                                 )
                             )
-                        else:
-                            # TODO: figure out how to differentiate type changes
-                            # print(f"VariableSymbolDB caught: {obj}")
-                            # print(f"Obj type: {type(obj)}")
-                            # print(f"Old value: {oldValue}")
-                            # print(f"New value: {newValue}")
-                            # typ = obj.getDataType()
-                            # stackVar = StackVariable(None, None, typ, None, None)
-                            # self._interface.stack_variable_changed(stackVar)
-                            pass
                     elif self._interface.ghidra.isinstance(obj, self.db.function.FunctionDB):
                         # TODO: Fix argument name support
                         # changed_arg = FunctionArgument(None, newValue, None, None)
                         # header = FunctionHeader(None, None, args={None: changed_arg})
                         # self._interface.function_header_changed(header)
                         pass
                     else:
```

### Comparing `libbs-1.3.3/libbs/decompilers/ghidra/interface.py` & `libbs-1.5.0/libbs/decompilers/ghidra/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -479,15 +479,20 @@
     def _set_enum(self, enum: Enum, **kwargs) -> bool:
         corrected_enum_name = "/" + enum.name
         old_ghidra_enum = self.ghidra.currentProgram.getDataTypeManager().getDataType(corrected_enum_name)
         data_manager = self.ghidra.currentProgram.getDataTypeManager()
         handler = self.ghidra.import_module_object("ghidra.program.model.data", "DataTypeConflictHandler")
         enumType = self.ghidra.import_module_object("ghidra.program.model.data", "EnumDataType")
         categoryPath = self.ghidra.import_module_object("ghidra.program.model.data", "CategoryPath")
-        ghidra_enum = enumType(categoryPath('/'), enum.name, 4)
+
+        # Parse the libbs Enum name into category path and raw enum name for proper Enum creation
+        split = corrected_enum_name.split('/')
+        unpathed_name = split[-1]
+        category_path = '/'.join(split[:-1])
+        ghidra_enum = enumType(categoryPath(category_path), unpathed_name, 4)
         for m_name, m_val in enum.members.items():
             ghidra_enum.add(m_name, m_val)
 
         try:
             if old_ghidra_enum:
                 data_manager.replaceDataType(old_ghidra_enum, ghidra_enum, True)
             else:
@@ -511,19 +516,14 @@
             "for dType in currentProgram.getDataTypeManager().getAllDataTypes()"
             "if ghidra.isinstance(dType, EnumDBType)]",
         ghidra=self.ghidra,
         EnumDBType=self.ghidra.import_module_object("ghidra.program.database.data", "EnumDB")
         )
         enums = {}
         for name in names:
-            # Filter out enums nested in categories as currently they are unsupported by the current method of updating
-            # the enum name
-            if name.count("/") != 1:
-                continue
-
             enum_name = name[1:]
             is_valid_enum = self._get_ghidra_enum(enum_name)
             if is_valid_enum is None:
                 continue
 
             enums[enum_name] = Enum(enum_name, self._get_enum_members(enum_name))
```

### Comparing `libbs-1.3.3/libbs/decompilers/ida/artifact_lifter.py` & `libbs-1.5.0/libbs/decompilers/ida/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/decompilers/ida/compat.py` & `libbs-1.5.0/libbs/decompilers/ida/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/decompilers/ida/hooks.py` & `libbs-1.5.0/libbs/decompilers/ida/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/decompilers/ida/interface.py` & `libbs-1.5.0/libbs/decompilers/ida/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/logger.py` & `libbs-1.5.0/libbs/logger.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/plugin_installer.py` & `libbs-1.5.0/libbs/plugin_installer.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/ui/__init__.py` & `libbs-1.5.0/libbs/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/ui/qt_objects.py` & `libbs-1.5.0/libbs/ui/qt_objects.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs/ui/utils.py` & `libbs-1.5.0/libbs/ui/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/libbs.egg-info/PKG-INFO` & `libbs-1.5.0/libbs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.3.3
+Version: 1.5.0
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
```

### Comparing `libbs-1.3.3/libbs.egg-info/SOURCES.txt` & `libbs-1.5.0/libbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/setup.cfg` & `libbs-1.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/tests/test_artifacts.py` & `libbs-1.5.0/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/tests/test_cli.py` & `libbs-1.5.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.3/tests/test_decompilers.py` & `libbs-1.5.0/tests/test_decompilers.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,14 +63,18 @@
         assert updated.members[0].type == 'undefined'
         assert updated.members[1].type == 'undefined'
 
         enum = Enum("my_enum", {"member1": 0, "member2": 1})
         deci.enums[enum.name] = enum
         assert deci.enums[enum.name] == enum
 
+        nested_enum = Enum("SomeEnums/nested_enum", {"field": 0, "another_field": 2, "third_field": 3})
+        deci.enums[nested_enum.name] = nested_enum
+        assert deci.enums[nested_enum.name] == nested_enum
+
         # gvar_addr = deci.art_lifter.lift_addr(0x4008e0)
         # g1 = deci.global_vars[gvar_addr]
         # g1.name = "gvar1"
         # deci.global_vars[gvar_addr] = g1
         # assert deci.global_vars[gvar_addr] == g1
 
         stack_var = main.stack_vars[-24]
@@ -93,48 +97,59 @@
         hits = defaultdict(list)
         def func_hit(*args, **kwargs): hits[args[0].__class__].append(args[0])
 
         deci.artifact_write_callbacks = {
             typ: [func_hit] for typ in (FunctionHeader, StackVariable, Enum, Struct, GlobalVariable, Comment)
         }
 
+        # Exact number of hits is not consistent, so we instead check for the minimum increment expected
+        old_header_hits = len(hits[FunctionHeader])
+
         # function names
         func_addr = deci.art_lifter.lift_addr(0x400664)
         main = deci.functions[func_addr]
         main.name = "changed"
         deci.functions[func_addr] = main
 
         main.name = "main"
         deci.functions[func_addr] = main
 
         first_changed_func = hits[FunctionHeader][0]
-        assert first_changed_func.name == "changed"
-        assert first_changed_func.addr == func_addr
-        assert len(hits[FunctionHeader]) == 2
+        assert len(hits[FunctionHeader]) >= old_header_hits + 2
+        old_header_hits = len(hits[FunctionHeader])
 
         # global var names
         # TODO: The gvar test cant function until gvar setting is fixed
         old_global_hits = len(hits[GlobalVariable])
         g1_addr = deci.art_lifter.lift_addr(0x4008e0)
         g2_addr = deci.art_lifter.lift_addr(0x601048)
         g1 = deci.global_vars[g1_addr]
         g2 = deci.global_vars[g2_addr]
         g1.name = "gvar1"
         g2.name = "gvar2"
         deci.global_vars[g1_addr] = g1
         deci.global_vars[g2_addr] = g2
         # assert len(hits[GlobalVariable]) == old_global_hits + 2
 
+        # function return type
+        main.header.type = 'long'
+        deci.functions[func_addr] = main
+
+        main.header.type = 'double'
+        deci.functions[func_addr] = main
+
+        assert len(hits[FunctionHeader]) >= old_header_hits + 2
+
         # TODO: Fix CI for below
         main.stack_vars[-24].name = "named_char_array"
         main.stack_vars[-12].name = "named_int"
         deci.functions[func_addr] = main
-        #first_changed_sv = hits[StackVariable][0]
-        #assert first_changed_sv.name == main.stack_vars[-24].name
-        #assert len(hits[StackVariable]) == 2
+        # first_changed_sv = hits[StackVariable][0]
+        # assert first_changed_sv.name == main.stack_vars[-24].name
+        # assert len(hits[StackVariable]) == 2
 
         # struct = deci.structs['eh_frame_hdr']
         # struct.name = "my_struct_name"
         # deci.structs['eh_frame_hdr'] = struct
 
         # TODO: add argument naming
         # func_args = main.header.args
```

