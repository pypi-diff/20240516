# Comparing `tmp/alliance_platform_frontend-0.0.5.tar.gz` & `tmp/alliance_platform_frontend-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alliance_platform_frontend-0.0.5.tar", last modified: Mon May 13 01:21:01 2024, max compression
+gzip compressed data, was "alliance_platform_frontend-0.0.6.tar", last modified: Mon May 13 05:05:21 2024, max compression
```

## Comparing `alliance_platform_frontend-0.0.5.tar` & `alliance_platform_frontend-0.0.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     2946 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/README.md
--rw-r--r--   0        0        0       22 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/__init__.py
--rw-r--r--   0        0        0      784 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/button.py
--rw-r--r--   0        0        0     1839 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/date_picker.py
--rw-r--r--   0        0        0     2524 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/icon.py
--rw-r--r--   0        0        0     1421 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/inline_alert.py
--rw-r--r--   0        0        0     1464 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/menubar.py
--rw-r--r--   0        0        0     2075 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/misc.py
--rw-r--r--   0        0        0     1622 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/pagination.py
--rw-r--r--   0        0        0     2270 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/table.py
--rw-r--r--   0        0        0     1127 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/time_input.py
--rw-r--r--   0        0        0     1243 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/utils.py
--rw-r--r--   0        0        0      358 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/apps.py
--rw-r--r--   0        0        0      633 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/__init__.py
--rw-r--r--   0        0        0     2402 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/asset_registry.py
--rw-r--r--   0        0        0    16050 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/base.py
--rw-r--r--   0        0        0    17210 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/context.py
--rw-r--r--   0        0        0     2507 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/middleware.py
--rw-r--r--   0        0        0    13537 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/ssr.py
--rw-r--r--   0        0        0     7051 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/vanilla_extract.py
--rw-r--r--   0        0        0    34218 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/vite.py
--rw-r--r--   0        0        0      175 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/vitePreload.ts
--rw-r--r--   0        0        0    11144 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/dom_possible_standard_names.py
--rw-r--r--   0        0        0        0 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/forms/__init__.py
--rw-r--r--   0        0        0     1620 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/forms/renderers.py
--rw-r--r--   0        0        0     5340 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/management/commands/extract_frontend_assets.py
--rw-r--r--   0        0        0     9471 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/prop_handlers.py
--rw-r--r--   0        0        0        0 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/py.typed
--rw-r--r--   0        0        0     8806 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/settings.py
--rw-r--r--   0        0        0     2684 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/templates/bundler_dev_check.html
--rw-r--r--   0        0        0        0 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/__init__.py
--rw-r--r--   0        0        0     5451 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/alliance_ui.py
--rw-r--r--   0        0        0    13141 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/bundler.py
--rw-r--r--   0        0        0     9664 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/form.py
--rw-r--r--   0        0        0    64472 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/react.py
--rw-r--r--   0        0        0     4316 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/vanilla_extract.py
--rw-r--r--   0        0        0     3283 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/util.py
--rw-r--r--   0        0        0     2120 2024-05-13 01:21:01.663164 alliance_platform_frontend-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     2503 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/fixtures/build_test/manifest.json
--rw-r--r--   0        0        0       39 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/fixtures/development-css-mappings/login_css_ts.json
--rw-r--r--   0        0        0       30 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/fixtures/production-css-mappings/login_css_ts.json
--rw-r--r--   0        0        0      648 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/fixtures/server_build_test/manifest.json
--rw-r--r--   0        0        0     7955 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/test_alliance_ui_templatetags.py
--rw-r--r--   0        0        0    12764 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/test_bundler.py
--rw-r--r--   0        0        0    41503 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/test_bundler_templatetags.py
--rw-r--r--   0        0        0     5837 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/test_context.py
--rw-r--r--   0        0        0      721 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     2384 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/test_utils/bundler.py
--rw-r--r--   0        0        0     4424 1970-01-01 00:00:00.000000 alliance_platform_frontend-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2946 2024-05-13 05:04:54.754269 alliance_platform_frontend-0.0.6/README.md
+-rw-r--r--   0        0        0       22 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/__init__.py
+-rw-r--r--   0        0        0      784 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/button.py
+-rw-r--r--   0        0        0     1839 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/date_picker.py
+-rw-r--r--   0        0        0     2524 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/icon.py
+-rw-r--r--   0        0        0     1421 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/inline_alert.py
+-rw-r--r--   0        0        0     1464 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/menubar.py
+-rw-r--r--   0        0        0     2075 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/misc.py
+-rw-r--r--   0        0        0     1622 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/pagination.py
+-rw-r--r--   0        0        0     2270 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/table.py
+-rw-r--r--   0        0        0     1127 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/time_input.py
+-rw-r--r--   0        0        0     1243 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/utils.py
+-rw-r--r--   0        0        0      358 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/apps.py
+-rw-r--r--   0        0        0      633 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/__init__.py
+-rw-r--r--   0        0        0     2402 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/asset_registry.py
+-rw-r--r--   0        0        0    16050 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/base.py
+-rw-r--r--   0        0        0    17210 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/context.py
+-rw-r--r--   0        0        0     2507 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/middleware.py
+-rw-r--r--   0        0        0    13537 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/ssr.py
+-rw-r--r--   0        0        0     7051 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/vanilla_extract.py
+-rw-r--r--   0        0        0    34218 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/vite.py
+-rw-r--r--   0        0        0      175 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/vitePreload.ts
+-rw-r--r--   0        0        0    11144 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/dom_possible_standard_names.py
+-rw-r--r--   0        0        0        0 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/forms/__init__.py
+-rw-r--r--   0        0        0     1620 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/forms/renderers.py
+-rw-r--r--   0        0        0     5340 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/management/commands/extract_frontend_assets.py
+-rw-r--r--   0        0        0     9471 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/prop_handlers.py
+-rw-r--r--   0        0        0        0 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/py.typed
+-rw-r--r--   0        0        0     8806 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/settings.py
+-rw-r--r--   0        0        0     2684 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/templates/bundler_dev_check.html
+-rw-r--r--   0        0        0        0 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/templatetags/__init__.py
+-rw-r--r--   0        0        0     5451 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/templatetags/alliance_ui.py
+-rw-r--r--   0        0        0    13141 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/templatetags/bundler.py
+-rw-r--r--   0        0        0     9664 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/templatetags/form.py
+-rw-r--r--   0        0        0    64013 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/templatetags/react.py
+-rw-r--r--   0        0        0     4316 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/templatetags/vanilla_extract.py
+-rw-r--r--   0        0        0     3283 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/alliance_platform/frontend/util.py
+-rw-r--r--   0        0        0     2120 2024-05-13 05:05:21.926646 alliance_platform_frontend-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     2503 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/tests/fixtures/build_test/manifest.json
+-rw-r--r--   0        0        0       39 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/tests/fixtures/development-css-mappings/login_css_ts.json
+-rw-r--r--   0        0        0       30 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/tests/fixtures/production-css-mappings/login_css_ts.json
+-rw-r--r--   0        0        0      648 2024-05-13 05:04:54.758269 alliance_platform_frontend-0.0.6/tests/fixtures/server_build_test/manifest.json
+-rw-r--r--   0        0        0     7955 2024-05-13 05:04:54.762269 alliance_platform_frontend-0.0.6/tests/test_alliance_ui_templatetags.py
+-rw-r--r--   0        0        0    12764 2024-05-13 05:04:54.762269 alliance_platform_frontend-0.0.6/tests/test_bundler.py
+-rw-r--r--   0        0        0    41503 2024-05-13 05:04:54.762269 alliance_platform_frontend-0.0.6/tests/test_bundler_templatetags.py
+-rw-r--r--   0        0        0     5837 2024-05-13 05:04:54.762269 alliance_platform_frontend-0.0.6/tests/test_context.py
+-rw-r--r--   0        0        0      721 2024-05-13 05:04:54.762269 alliance_platform_frontend-0.0.6/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     2384 2024-05-13 05:04:54.762269 alliance_platform_frontend-0.0.6/tests/test_utils/bundler.py
+-rw-r--r--   0        0        0     4424 1970-01-01 00:00:00.000000 alliance_platform_frontend-0.0.6/PKG-INFO
```

### Comparing `alliance_platform_frontend-0.0.5/README.md` & `alliance_platform_frontend-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/button.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/button.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/date_picker.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/date_picker.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/icon.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/icon.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/inline_alert.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/inline_alert.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/menubar.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/menubar.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/misc.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/misc.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/pagination.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/pagination.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/table.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/table.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/time_input.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/time_input.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/utils.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/alliance_ui/utils.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/__init__.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/__init__.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/asset_registry.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/asset_registry.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/base.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/base.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/context.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/context.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/middleware.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/middleware.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/ssr.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/ssr.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/vanilla_extract.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/vanilla_extract.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/vite.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/bundler/vite.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/dom_possible_standard_names.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/dom_possible_standard_names.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/forms/renderers.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/forms/renderers.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/management/commands/extract_frontend_assets.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/management/commands/extract_frontend_assets.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/prop_handlers.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/prop_handlers.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/settings.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/settings.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/templates/bundler_dev_check.html` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/templates/bundler_dev_check.html`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/alliance_ui.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/templatetags/alliance_ui.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/bundler.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/templatetags/bundler.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/form.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/templatetags/form.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/react.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/templatetags/react.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from alliance_platform.codegen.typescript import FunctionDeclaration
 from alliance_platform.codegen.typescript import Identifier
 from alliance_platform.codegen.typescript import ImportDefaultSpecifier
 from alliance_platform.codegen.typescript import ImportSpecifier
 from alliance_platform.codegen.typescript import JsxAttribute
 from alliance_platform.codegen.typescript import JsxElement
 from alliance_platform.codegen.typescript import MultiLineComment
+from alliance_platform.codegen.typescript import Node as TypescriptNode
 from alliance_platform.codegen.typescript import PropertyAccessExpression
 from alliance_platform.codegen.typescript import ReturnStatement
 from alliance_platform.codegen.typescript import StringLiteral
 from alliance_platform.codegen.typescript import UnconvertibleValueException
 from alliance_platform.codegen.typescript import convert_to_node
 from allianceutils.template import build_html_attrs
 from allianceutils.template import is_static_expression
@@ -570,29 +571,25 @@
     _requires_wrapper_component: bool
     #: Tracks the name of all identifiers generated so far. This is used to ensure uniqueness.
     _used_identifiers: list[str]
     #: Used by ``create_jsx_element`` to detect when the template name changes so it can output a comment.
     _last_template_origin_name: str | None
     #: Used by ``create_jsx_element`` to track the specified value for the ``include_template_origin`` kwarg in the root node
     _last_include_template_origin: bool
-    #: Any nodes that should be added to the start of the generated content. This can be used by ``ComponentProp`` handlers to add code outside the component.
-    #: For example, populating a cache should be done once and not on every render.
-    _leading_nodes: list[Node]
 
     def __init__(self, node: ComponentNode):
         self.node = node
         self.bundler = node.bundler
         self._writer = TypescriptSourceFileWriter(
             resolve_import_url=self._resolve_import_url,
         )
         self._requires_wrapper_component = False
         self._used_identifiers = []
         self._last_template_origin_name = None
         self._last_include_template_origin = False
-        self._leading_nodes = []
 
         # Resolve the import for createElement and use the returned Identifier for the jsx_transform
         self._writer.jsx_transform = self._writer.resolve_import(
             ap_frontend_settings.REACT_RENDER_COMPONENT_FILE,
             ImportSpecifier("createElement"),
             import_order_priority=HIGHEST_PRIORITY_IMPORT,
         )
@@ -736,19 +733,14 @@
         finally:
             self._last_template_origin_name = last_template_name
             self._include_template_origin = last_include_template_origin
 
     def generate_code(self, props: ComponentProps, container_id: str):
         jsx_element = self.create_jsx_element_node(self.node, props)
 
-        # This needs to happen after the jsx_element is created, as that is where props are processed that may trigger
-        # leading nodes to be added
-        for node in self._leading_nodes:
-            self._writer.add_node(node)
-
         # In some cases a wrapper component is needed, e.g. when using props that require hooks. This just wraps
         # the element in a wrapper function and returns the element. The props themselves may be a hook call, so we
         # don't have to specifically check for hooks here.
         if self._requires_wrapper_component:
             wrapper_id = Identifier("Wrapper")
             self._writer.add_node(
                 FunctionDeclaration(
@@ -788,17 +780,17 @@
         original_name = name
         while name in self._used_identifiers:
             name = f"{original_name}{counter}"
             counter += 1
         self._used_identifiers.append(name)
         return Identifier(name)
 
-    def add_leading_node(self, node: Node):
+    def add_leading_node(self, node: TypescriptNode):
         """Add a node that should be added to the top of the generated code."""
-        self._leading_nodes.append(node)
+        self._writer.add_leading_node(node)
 
 
 class OmitComponentFromRendering(Exception):
     """Raise this exception to indicate that the component should not be rendered.
 
     This can be used to indicate the component should not be rendered in certain circumstances, for example
     if a permission check is done to determine whether user can see certain content.
```

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/vanilla_extract.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/templatetags/vanilla_extract.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/alliance_platform/frontend/util.py` & `alliance_platform_frontend-0.0.6/alliance_platform/frontend/util.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/pyproject.toml` & `alliance_platform_frontend-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 include = [
     "alliance_platform/frontend/py.typed",
 ]
-version = "0.0.5"
+version = "0.0.6"
 
 [project.license]
 text = "BSD-2-Clause"
 
 [project.urls]
 issues = "https://github.com/AllianceSoftware/alliance-platform-py/issues"
 homepage = "https://github.com/AllianceSoftware/alliance-platform-py/packages/ap-frontend"
```

### Comparing `alliance_platform_frontend-0.0.5/tests/fixtures/build_test/manifest.json` & `alliance_platform_frontend-0.0.6/tests/fixtures/build_test/manifest.json`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/tests/fixtures/server_build_test/manifest.json` & `alliance_platform_frontend-0.0.6/tests/fixtures/server_build_test/manifest.json`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/tests/test_alliance_ui_templatetags.py` & `alliance_platform_frontend-0.0.6/tests/test_alliance_ui_templatetags.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/tests/test_bundler.py` & `alliance_platform_frontend-0.0.6/tests/test_bundler.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/tests/test_bundler_templatetags.py` & `alliance_platform_frontend-0.0.6/tests/test_bundler_templatetags.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/tests/test_context.py` & `alliance_platform_frontend-0.0.6/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/tests/test_utils/__init__.py` & `alliance_platform_frontend-0.0.6/tests/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/tests/test_utils/bundler.py` & `alliance_platform_frontend-0.0.6/tests/test_utils/bundler.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.5/PKG-INFO` & `alliance_platform_frontend-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alliance-platform-frontend
-Version: 0.0.5
+Version: 0.0.6
 Summary: Django integration for Frontend Bundlers & React
 Keywords: django,alliance,alliancesoftware
 Home-page: https://github.com/AllianceSoftware/alliance-platform-py/packages/ap-frontend
 Author-Email: Alliance Software <support@alliancesoftware.com.au>
 License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

