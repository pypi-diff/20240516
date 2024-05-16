# Comparing `tmp/qtharmony-0.2.9.tar.gz` & `tmp/qtharmony-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtharmony-0.2.9.tar", max compression
+gzip compressed data, was "qtharmony-0.3.0.tar", max compression
```

## Comparing `qtharmony-0.2.9.tar` & `qtharmony-0.3.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.2.9/LICENSE
--rw-r--r--   0        0        0     2340 2024-05-14 07:15:03.814438 qtharmony-0.2.9/README.md
--rw-r--r--   0        0        0      609 2024-05-14 15:55:11.671215 qtharmony-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.2.9/qtharmony/__init__.py
--rw-r--r--   0        0        0       22 2024-05-14 15:55:11.674548 qtharmony-0.2.9/qtharmony/config/__init__.py
--rw-r--r--   0        0        0      233 2024-05-14 15:55:11.674548 qtharmony-0.2.9/qtharmony/config/config.py
--rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.2.9/qtharmony/constructor/__init__.py
--rw-r--r--   0        0        0      628 2024-05-14 15:55:11.674548 qtharmony-0.2.9/qtharmony/constructor/initialize.py
--rw-r--r--   0        0        0      120 2024-05-14 15:55:11.674548 qtharmony-0.2.9/qtharmony/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-14 15:55:11.674548 qtharmony-0.2.9/qtharmony/core/dialog.py
--rw-r--r--   0        0        0      151 2024-05-14 15:55:11.674548 qtharmony-0.2.9/qtharmony/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-14 15:55:11.674548 qtharmony-0.2.9/qtharmony/core/font.py
--rw-r--r--   0        0        0      876 2024-05-14 15:55:11.674548 qtharmony-0.2.9/qtharmony/core/load.py
--rw-r--r--   0        0        0      576 2024-05-14 15:55:11.674548 qtharmony-0.2.9/qtharmony/core/sizes.py
--rw-r--r--   0        0        0     1235 2024-05-14 15:55:11.674548 qtharmony-0.2.9/qtharmony/core/stylesheet.py
--rw-r--r--   0        0        0       80 2024-05-14 15:55:11.674548 qtharmony-0.2.9/qtharmony/core/theme/__init__.py
--rw-r--r--   0        0        0     1295 2024-05-14 15:55:11.674548 qtharmony-0.2.9/qtharmony/core/theme/theme_builder.py
--rw-r--r--   0        0        0     2345 2024-05-14 15:55:11.674548 qtharmony-0.2.9/qtharmony/core/theme/theme_manager.py
--rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.2.9/qtharmony/resources/__init__.py
--rw-r--r--   0        0        0     4435 2024-05-14 07:15:03.814438 qtharmony-0.2.9/qtharmony/resources/themes/dark-default.json
--rw-r--r--   0        0        0     4611 2024-05-12 12:26:40.223721 qtharmony-0.2.9/qtharmony/resources/themes/dark-green.json
--rw-r--r--   0        0        0     4563 2024-05-12 11:50:16.451713 qtharmony-0.2.9/qtharmony/resources/themes/light-default.json
--rw-r--r--   0        0        0     4560 2024-05-12 12:20:22.144106 qtharmony-0.2.9/qtharmony/resources/themes/light-green.json
--rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.2.9/qtharmony/resources/ui/Icon.png
--rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.2.9/qtharmony/resources/ui/Logo.png
--rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.2.9/qtharmony/resources/ui/angle-down.png
--rw-r--r--   0        0        0      464 2024-05-12 11:50:16.451713 qtharmony-0.2.9/qtharmony/widgets/__init__.py
--rw-r--r--   0        0        0     2396 2024-05-14 15:55:11.674548 qtharmony-0.2.9/qtharmony/widgets/basic/button.py
--rw-r--r--   0        0        0     2721 2024-05-14 15:55:11.674548 qtharmony-0.2.9/qtharmony/widgets/basic/check_box.py
--rw-r--r--   0        0        0     2564 2024-05-14 15:55:11.677882 qtharmony-0.2.9/qtharmony/widgets/basic/digital_entry.py
--rw-r--r--   0        0        0     3537 2024-05-14 15:55:11.677882 qtharmony-0.2.9/qtharmony/widgets/basic/drop_down_menu.py
--rw-r--r--   0        0        0     2575 2024-05-14 15:55:11.677882 qtharmony-0.2.9/qtharmony/widgets/basic/entry.py
--rw-r--r--   0        0        0      918 2024-05-14 15:55:11.677882 qtharmony-0.2.9/qtharmony/widgets/basic/frame.py
--rw-r--r--   0        0        0     2789 2024-05-14 15:55:11.677882 qtharmony-0.2.9/qtharmony/widgets/basic/groups.py
--rw-r--r--   0        0        0     3257 2024-05-14 15:55:11.677882 qtharmony-0.2.9/qtharmony/widgets/basic/label.py
--rw-r--r--   0        0        0     3851 2024-05-14 15:55:11.677882 qtharmony-0.2.9/qtharmony/widgets/basic/path_entry.py
--rw-r--r--   0        0        0     1995 2024-05-14 15:55:11.677882 qtharmony-0.2.9/qtharmony/widgets/basic/radio_button.py
--rw-r--r--   0        0        0     2055 2024-05-14 15:55:11.677882 qtharmony-0.2.9/qtharmony/widgets/basic/splitter.py
--rw-r--r--   0        0        0       61 2024-05-12 07:41:31.423989 qtharmony-0.2.9/qtharmony/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.2.9/qtharmony/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.2.9/qtharmony/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      147 2024-05-12 11:50:16.451713 qtharmony-0.2.9/qtharmony/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0      108 2024-05-12 11:50:16.451713 qtharmony-0.2.9/qtharmony/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0        0 2024-05-12 11:50:16.451713 qtharmony-0.2.9/qtharmony/widgets/basic/styles/frame.css
--rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.2.9/qtharmony/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.2.9/qtharmony/widgets/basic/styles/label.css
--rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.2.9/qtharmony/widgets/basic/styles/path_entry.css
--rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.2.9/qtharmony/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0        0 2024-05-12 07:41:31.423989 qtharmony-0.2.9/qtharmony/widgets/basic/styles/splitter.css
--rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.2.9/qtharmony/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0     1574 2024-05-14 15:55:11.677882 qtharmony-0.2.9/qtharmony/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.2.9/qtharmony/windows/__init__.py
--rw-r--r--   0        0        0     2679 2024-05-14 15:55:11.677882 qtharmony-0.2.9/qtharmony/windows/main_window.py
--rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.2.9/qtharmony/windows/styles/main_window.css
--rw-r--r--   0        0        0     3082 1970-01-01 00:00:00.000000 qtharmony-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2340 2024-05-14 07:15:03.814438 qtharmony-0.3.0/README.md
+-rw-r--r--   0        0        0      312 2024-05-16 07:29:16.152505 qtharmony-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.3.0/qtharmony/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-14 15:55:11.674548 qtharmony-0.3.0/qtharmony/config/__init__.py
+-rw-r--r--   0        0        0      233 2024-05-14 15:55:11.674548 qtharmony-0.3.0/qtharmony/config/config.py
+-rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.3.0/qtharmony/constructor/__init__.py
+-rw-r--r--   0        0        0      628 2024-05-14 15:55:11.674548 qtharmony-0.3.0/qtharmony/constructor/initialize.py
+-rw-r--r--   0        0        0      120 2024-05-14 15:55:11.674548 qtharmony-0.3.0/qtharmony/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-14 15:55:11.674548 qtharmony-0.3.0/qtharmony/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-14 15:55:11.674548 qtharmony-0.3.0/qtharmony/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-14 15:55:11.674548 qtharmony-0.3.0/qtharmony/core/font.py
+-rw-r--r--   0        0        0      876 2024-05-14 15:55:11.674548 qtharmony-0.3.0/qtharmony/core/load.py
+-rw-r--r--   0        0        0      576 2024-05-14 15:55:11.674548 qtharmony-0.3.0/qtharmony/core/sizes.py
+-rw-r--r--   0        0        0     1235 2024-05-14 15:55:11.674548 qtharmony-0.3.0/qtharmony/core/stylesheet.py
+-rw-r--r--   0        0        0       80 2024-05-14 15:55:11.674548 qtharmony-0.3.0/qtharmony/core/theme/__init__.py
+-rw-r--r--   0        0        0     1295 2024-05-14 15:55:11.674548 qtharmony-0.3.0/qtharmony/core/theme/theme_builder.py
+-rw-r--r--   0        0        0     2345 2024-05-14 15:55:11.674548 qtharmony-0.3.0/qtharmony/core/theme/theme_manager.py
+-rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.3.0/qtharmony/resources/__init__.py
+-rw-r--r--   0        0        0     4715 2024-05-14 17:26:45.157068 qtharmony-0.3.0/qtharmony/resources/themes/dark-default.json
+-rw-r--r--   0        0        0     4611 2024-05-12 12:26:40.223721 qtharmony-0.3.0/qtharmony/resources/themes/dark-green.json
+-rw-r--r--   0        0        0     4563 2024-05-12 11:50:16.451713 qtharmony-0.3.0/qtharmony/resources/themes/light-default.json
+-rw-r--r--   0        0        0     4560 2024-05-12 12:20:22.144106 qtharmony-0.3.0/qtharmony/resources/themes/light-green.json
+-rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.3.0/qtharmony/resources/ui/Icon.png
+-rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.3.0/qtharmony/resources/ui/Logo.png
+-rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.3.0/qtharmony/resources/ui/angle-down.png
+-rw-r--r--   0        0        0      464 2024-05-12 11:50:16.451713 qtharmony-0.3.0/qtharmony/widgets/__init__.py
+-rw-r--r--   0        0        0     2396 2024-05-14 15:55:11.674548 qtharmony-0.3.0/qtharmony/widgets/basic/button.py
+-rw-r--r--   0        0        0     2721 2024-05-14 15:55:11.674548 qtharmony-0.3.0/qtharmony/widgets/basic/check_box.py
+-rw-r--r--   0        0        0     2564 2024-05-14 15:55:11.677882 qtharmony-0.3.0/qtharmony/widgets/basic/digital_entry.py
+-rw-r--r--   0        0        0     3537 2024-05-14 15:55:11.677882 qtharmony-0.3.0/qtharmony/widgets/basic/drop_down_menu.py
+-rw-r--r--   0        0        0     2575 2024-05-14 15:55:11.677882 qtharmony-0.3.0/qtharmony/widgets/basic/entry.py
+-rw-r--r--   0        0        0      918 2024-05-14 15:55:11.677882 qtharmony-0.3.0/qtharmony/widgets/basic/frame.py
+-rw-r--r--   0        0        0     2789 2024-05-14 15:55:11.677882 qtharmony-0.3.0/qtharmony/widgets/basic/groups.py
+-rw-r--r--   0        0        0     3257 2024-05-14 15:55:11.677882 qtharmony-0.3.0/qtharmony/widgets/basic/label.py
+-rw-r--r--   0        0        0     3851 2024-05-14 15:55:11.677882 qtharmony-0.3.0/qtharmony/widgets/basic/path_entry.py
+-rw-r--r--   0        0        0     1995 2024-05-14 15:55:11.677882 qtharmony-0.3.0/qtharmony/widgets/basic/radio_button.py
+-rw-r--r--   0        0        0     2179 2024-05-16 07:25:54.940616 qtharmony-0.3.0/qtharmony/widgets/basic/splitter.py
+-rw-r--r--   0        0        0       61 2024-05-12 07:41:31.423989 qtharmony-0.3.0/qtharmony/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.3.0/qtharmony/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.3.0/qtharmony/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      147 2024-05-12 11:50:16.451713 qtharmony-0.3.0/qtharmony/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0      108 2024-05-12 11:50:16.451713 qtharmony-0.3.0/qtharmony/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0        0 2024-05-12 11:50:16.451713 qtharmony-0.3.0/qtharmony/widgets/basic/styles/frame.css
+-rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.3.0/qtharmony/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.3.0/qtharmony/widgets/basic/styles/label.css
+-rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.3.0/qtharmony/widgets/basic/styles/path_entry.css
+-rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.3.0/qtharmony/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0        0 2024-05-12 07:41:31.423989 qtharmony-0.3.0/qtharmony/widgets/basic/styles/splitter.css
+-rw-r--r--   0        0        0        0 2024-05-14 17:18:13.597694 qtharmony-0.3.0/qtharmony/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0     1286 2024-05-14 17:27:19.628796 qtharmony-0.3.0/qtharmony/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.3.0/qtharmony/windows/__init__.py
+-rw-r--r--   0        0        0     2679 2024-05-14 15:55:11.677882 qtharmony-0.3.0/qtharmony/windows/main_window.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.3.0/qtharmony/windows/styles/main_window.css
+-rw-r--r--   0        0        0     2785 1970-01-01 00:00:00.000000 qtharmony-0.3.0/PKG-INFO
```

### Comparing `qtharmony-0.2.9/LICENSE` & `qtharmony-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/README.md` & `qtharmony-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/constructor/initialize.py` & `qtharmony-0.3.0/qtharmony/constructor/initialize.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/core/dialog.py` & `qtharmony-0.3.0/qtharmony/core/dialog.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/core/font.py` & `qtharmony-0.3.0/qtharmony/core/font.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/core/load.py` & `qtharmony-0.3.0/qtharmony/core/load.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/core/sizes.py` & `qtharmony-0.3.0/qtharmony/core/sizes.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/core/stylesheet.py` & `qtharmony-0.3.0/qtharmony/core/stylesheet.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/core/theme/theme_builder.py` & `qtharmony-0.3.0/qtharmony/core/theme/theme_builder.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/core/theme/theme_manager.py` & `qtharmony-0.3.0/qtharmony/core/theme/theme_manager.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/resources/themes/dark-default.json` & `qtharmony-0.3.0/qtharmony/resources/themes/dark-default.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'WidgetsList'": "OrderedDict([('object-name', 'QListWidget#widgets-list'), ('', "*

 * *                  "OrderedDict([('background-color', '#404040'), ('border-radius', '6px'), "*

 * *                  "('border', 'none')])), ('::item', OrderedDict([('min-height', '100px')]))])"}*

```diff
@@ -165,9 +165,20 @@
         "object-name": "QSplitter#splitter"
     },
     "TextBox": {
         "": {
             "background-color": "green"
         },
         "object-name": "QPlainTextEdit#text-box"
+    },
+    "WidgetsList": {
+        "": {
+            "background-color": "#404040",
+            "border": "none",
+            "border-radius": "6px"
+        },
+        "::item": {
+            "min-height": "100px"
+        },
+        "object-name": "QListWidget#widgets-list"
     }
 }
```

### Comparing `qtharmony-0.2.9/qtharmony/resources/themes/dark-green.json` & `qtharmony-0.3.0/qtharmony/resources/themes/dark-green.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/resources/themes/light-default.json` & `qtharmony-0.3.0/qtharmony/resources/themes/light-default.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/resources/themes/light-green.json` & `qtharmony-0.3.0/qtharmony/resources/themes/light-green.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/resources/ui/Icon.png` & `qtharmony-0.3.0/qtharmony/resources/ui/Icon.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/resources/ui/Logo.png` & `qtharmony-0.3.0/qtharmony/resources/ui/Logo.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/resources/ui/angle-down.png` & `qtharmony-0.3.0/qtharmony/resources/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/widgets/basic/button.py` & `qtharmony-0.3.0/qtharmony/widgets/basic/button.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/widgets/basic/check_box.py` & `qtharmony-0.3.0/qtharmony/widgets/basic/check_box.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/widgets/basic/digital_entry.py` & `qtharmony-0.3.0/qtharmony/widgets/basic/digital_entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/widgets/basic/drop_down_menu.py` & `qtharmony-0.3.0/qtharmony/widgets/basic/drop_down_menu.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/widgets/basic/entry.py` & `qtharmony-0.3.0/qtharmony/widgets/basic/entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/widgets/basic/frame.py` & `qtharmony-0.3.0/qtharmony/widgets/basic/frame.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/widgets/basic/groups.py` & `qtharmony-0.3.0/qtharmony/widgets/basic/groups.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/widgets/basic/label.py` & `qtharmony-0.3.0/qtharmony/widgets/basic/label.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/widgets/basic/path_entry.py` & `qtharmony-0.3.0/qtharmony/widgets/basic/path_entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/widgets/basic/radio_button.py` & `qtharmony-0.3.0/qtharmony/widgets/basic/radio_button.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/qtharmony/widgets/basic/splitter.py` & `qtharmony-0.3.0/qtharmony/widgets/basic/splitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,18 +43,21 @@
         self.setObjectName(object_name)
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/splitter.css", 
             name=self.__class__.__name__, obj_name=f"QSplitter#{self.objectName()}",
             stylesheet=stylesheet
         )
 
-    def addWidget(self, widget):
+    def addWidget(self, widget, stretch: Optional[int] = None):
         """
         Adds a widget to the splitter and sets it as non-collapsible.
 
         Args:
             widget (QWidget): The widget to be added to the splitter.
         """
 
         super().addWidget(widget)
-        self.setCollapsible(self.indexOf(widget), False)
+        index = self.indexOf(widget)
+
+        if stretch is not None: self.setStretchFactor(index, stretch)
+        self.setCollapsible(index, False)
```

### Comparing `qtharmony-0.2.9/qtharmony/windows/main_window.py` & `qtharmony-0.3.0/qtharmony/windows/main_window.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.9/PKG-INFO` & `qtharmony-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: QtHarmony
-Version: 0.2.9
-Summary: QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development.
+Version: 0.3.0
+Summary: 
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

