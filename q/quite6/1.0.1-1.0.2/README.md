# Comparing `tmp/quite6-1.0.1.tar.gz` & `tmp/quite6-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quite6-1.0.1.tar", last modified: Wed May 15 06:38:27 2024, max compression
+gzip compressed data, was "quite6-1.0.2.tar", last modified: Thu May 16 14:16:31 2024, max compression
```

## Comparing `quite6-1.0.1.tar` & `quite6-1.0.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-15 06:38:27.940408 quite6-1.0.1/
--rw-r--r--   0 wangcong   (502) staff       (20)     1074 2024-05-14 10:15:26.000000 quite6-1.0.1/LICENSE
--rw-r--r--   0 wangcong   (502) staff       (20)      104 2024-05-14 10:15:26.000000 quite6-1.0.1/MANIFEST.in
--rw-r--r--   0 wangcong   (502) staff       (20)     3754 2024-05-15 06:38:27.939640 quite6-1.0.1/PKG-INFO
--rw-r--r--   0 wangcong   (502) staff       (20)     2936 2024-05-14 10:15:26.000000 quite6-1.0.1/README.rst
--rw-r--r--   0 wangcong   (502) staff       (20)        6 2024-05-15 06:37:36.000000 quite6-1.0.1/RELEASE-VERSION
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-15 06:38:27.880146 quite6-1.0.1/quite6/
--rw-r--r--   0 wangcong   (502) staff       (20)      272 2024-05-14 11:46:55.000000 quite6-1.0.1/quite6/__init__.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-15 06:38:27.887631 quite6-1.0.1/quite6/controller/
--rw-r--r--   0 wangcong   (502) staff       (20)      211 2024-05-13 08:52:57.000000 quite6-1.0.1/quite6/controller/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)      606 2024-05-14 14:24:17.000000 quite6-1.0.1/quite6/controller/dialog_ui_controller.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2634 2024-05-14 14:24:17.000000 quite6-1.0.1/quite6/controller/file_dialog_controller.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1616 2024-05-14 14:24:17.000000 quite6-1.0.1/quite6/controller/widget_controller.py
--rw-r--r--   0 wangcong   (502) staff       (20)     3514 2024-05-14 03:41:05.000000 quite6-1.0.1/quite6/controller/widget_ui_controller.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-15 06:38:27.889075 quite6-1.0.1/quite6/core/
--rw-r--r--   0 wangcong   (502) staff       (20)      203 2024-05-14 10:47:48.000000 quite6-1.0.1/quite6/core/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1326 2024-05-14 10:43:54.000000 quite6-1.0.1/quite6/core/event_loop.py
--rw-r--r--   0 wangcong   (502) staff       (20)      281 2024-05-14 10:43:54.000000 quite6-1.0.1/quite6/core/timer.py
--rw-r--r--   0 wangcong   (502) staff       (20)     3712 2024-05-14 15:04:01.000000 quite6-1.0.1/quite6/deferred_function.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-15 06:38:27.890609 quite6-1.0.1/quite6/gui/
--rw-r--r--   0 wangcong   (502) staff       (20)     1118 2024-05-14 11:49:59.000000 quite6-1.0.1/quite6/gui/__init__.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-15 06:38:27.896164 quite6-1.0.1/quite6/gui/interfaces/
--rw-r--r--   0 wangcong   (502) staff       (20)      554 2024-05-13 08:52:57.000000 quite6-1.0.1/quite6/gui/interfaces/__init__.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-15 06:38:27.899013 quite6-1.0.1/quite6/gui/interfaces/ability_interfaces/
--rw-r--r--   0 wangcong   (502) staff       (20)      120 2024-05-13 08:52:57.000000 quite6-1.0.1/quite6/gui/interfaces/ability_interfaces/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)      188 2024-05-13 08:52:57.000000 quite6-1.0.1/quite6/gui/interfaces/ability_interfaces/class_exec_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1092 2024-05-14 10:57:04.000000 quite6-1.0.1/quite6/gui/interfaces/ability_interfaces/container_ability_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      539 2024-05-14 03:20:46.000000 quite6-1.0.1/quite6/gui/interfaces/base_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      303 2024-05-13 08:52:57.000000 quite6-1.0.1/quite6/gui/interfaces/changed_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      470 2024-05-14 08:19:12.000000 quite6-1.0.1/quite6/gui/interfaces/closed_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      307 2024-05-14 10:57:04.000000 quite6-1.0.1/quite6/gui/interfaces/excited_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      199 2024-05-14 10:57:04.000000 quite6-1.0.1/quite6/gui/interfaces/focus_in_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      201 2024-05-14 10:57:04.000000 quite6-1.0.1/quite6/gui/interfaces/focus_out_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      322 2024-05-14 10:57:04.000000 quite6-1.0.1/quite6/gui/interfaces/row_changed_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      298 2024-05-13 08:52:57.000000 quite6-1.0.1/quite6/gui/interfaces/showed_signal_interface.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-15 06:38:27.900169 quite6-1.0.1/quite6/gui/layouts/
--rw-r--r--   0 wangcong   (502) staff       (20)       40 2024-05-13 08:52:57.000000 quite6-1.0.1/quite6/gui/layouts/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2712 2024-05-14 14:37:29.000000 quite6-1.0.1/quite6/gui/layouts/square_layout.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-15 06:38:27.904734 quite6-1.0.1/quite6/gui/paint/
--rw-r--r--   0 wangcong   (502) staff       (20)      129 2024-05-13 08:52:57.000000 quite6-1.0.1/quite6/gui/paint/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)     5089 2024-05-14 14:37:29.000000 quite6-1.0.1/quite6/gui/paint/painter.py
--rw-r--r--   0 wangcong   (502) staff       (20)      502 2024-05-14 11:03:11.000000 quite6-1.0.1/quite6/gui/paint/pen.py
--rw-r--r--   0 wangcong   (502) staff       (20)      904 2024-05-14 11:03:11.000000 quite6-1.0.1/quite6/gui/paint/point.py
--rw-r--r--   0 wangcong   (502) staff       (20)      280 2024-05-14 11:03:11.000000 quite6-1.0.1/quite6/gui/paint/scaling.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1471 2024-05-14 11:03:11.000000 quite6-1.0.1/quite6/gui/paint/size.py
--rw-r--r--   0 wangcong   (502) staff       (20)      398 2024-05-14 10:17:44.000000 quite6-1.0.1/quite6/gui/qt_gui.py
--rw-r--r--   0 wangcong   (502) staff       (20)      311 2024-05-14 10:15:26.000000 quite6-1.0.1/quite6/gui/ui_extension.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-15 06:38:27.931229 quite6-1.0.1/quite6/gui/widgets/
--rw-r--r--   0 wangcong   (502) staff       (20)      798 2024-05-14 11:10:25.000000 quite6-1.0.1/quite6/gui/widgets/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)      383 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/action.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2454 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/combo_box.py
--rw-r--r--   0 wangcong   (502) staff       (20)      926 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/date_edit.py
--rw-r--r--   0 wangcong   (502) staff       (20)      683 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/date_time_edit.py
--rw-r--r--   0 wangcong   (502) staff       (20)      780 2024-05-14 11:51:50.000000 quite6-1.0.1/quite6/gui/widgets/dialog.py
--rw-r--r--   0 wangcong   (502) staff       (20)      195 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/dock_widget.py
--rw-r--r--   0 wangcong   (502) staff       (20)      721 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/double_spin_box.py
--rw-r--r--   0 wangcong   (502) staff       (20)      189 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/group_box.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1627 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/input_dialog.py
--rw-r--r--   0 wangcong   (502) staff       (20)      736 2024-05-14 14:37:29.000000 quite6-1.0.1/quite6/gui/widgets/label.py
--rw-r--r--   0 wangcong   (502) staff       (20)      183 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/layout.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1004 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/line_edit.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2347 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/list_widget.py
--rw-r--r--   0 wangcong   (502) staff       (20)      697 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/main_window.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2904 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/plot_widget.py
--rw-r--r--   0 wangcong   (502) staff       (20)      676 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/push_button.py
--rw-r--r--   0 wangcong   (502) staff       (20)      680 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/radio_button.py
--rw-r--r--   0 wangcong   (502) staff       (20)      582 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/shortcut.py
--rw-r--r--   0 wangcong   (502) staff       (20)      693 2024-05-14 11:54:28.000000 quite6-1.0.1/quite6/gui/widgets/spin_box.py
--rw-r--r--   0 wangcong   (502) staff       (20)     6529 2024-05-14 11:32:31.000000 quite6-1.0.1/quite6/gui/widgets/table_view.py
--rw-r--r--   0 wangcong   (502) staff       (20)     9397 2024-05-14 14:37:29.000000 quite6-1.0.1/quite6/gui/widgets/table_widget.py
--rw-r--r--   0 wangcong   (502) staff       (20)      720 2024-05-14 11:37:12.000000 quite6-1.0.1/quite6/gui/widgets/text_edit.py
--rw-r--r--   0 wangcong   (502) staff       (20)      926 2024-05-14 11:37:12.000000 quite6-1.0.1/quite6/gui/widgets/time_edit.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1326 2024-05-14 14:37:29.000000 quite6-1.0.1/quite6/gui/widgets/widget.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-15 06:38:27.936323 quite6-1.0.1/quite6/tools/
--rw-r--r--   0 wangcong   (502) staff       (20)      110 2024-05-14 11:51:08.000000 quite6-1.0.1/quite6/tools/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1207 2024-05-15 06:35:06.000000 quite6-1.0.1/quite6/tools/load_qrc.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2461 2024-05-14 15:28:56.000000 quite6-1.0.1/quite6/tools/load_ui.py
--rw-r--r--   0 wangcong   (502) staff       (20)      315 2024-05-14 14:37:29.000000 quite6-1.0.1/quite6/tools/process.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-15 06:38:27.937487 quite6-1.0.1/quite6.egg-info/
--rw-r--r--   0 wangcong   (502) staff       (20)     3754 2024-05-15 06:38:27.000000 quite6-1.0.1/quite6.egg-info/PKG-INFO
--rw-r--r--   0 wangcong   (502) staff       (20)     2394 2024-05-15 06:38:27.000000 quite6-1.0.1/quite6.egg-info/SOURCES.txt
--rw-r--r--   0 wangcong   (502) staff       (20)        1 2024-05-15 06:38:27.000000 quite6-1.0.1/quite6.egg-info/dependency_links.txt
--rw-r--r--   0 wangcong   (502) staff       (20)       46 2024-05-15 06:38:27.000000 quite6-1.0.1/quite6.egg-info/requires.txt
--rw-r--r--   0 wangcong   (502) staff       (20)        7 2024-05-15 06:38:27.000000 quite6-1.0.1/quite6.egg-info/top_level.txt
--rw-r--r--   0 wangcong   (502) staff       (20)     2557 2024-05-14 10:15:26.000000 quite6-1.0.1/readme.md
--rw-r--r--   0 wangcong   (502) staff       (20)       45 2024-05-14 10:15:26.000000 quite6-1.0.1/requirements.txt
--rw-r--r--   0 wangcong   (502) staff       (20)      154 2024-05-15 06:38:27.941409 quite6-1.0.1/setup.cfg
--rw-r--r--   0 wangcong   (502) staff       (20)     1633 2024-05-14 10:15:26.000000 quite6-1.0.1/setup.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2173 2024-05-14 10:15:26.000000 quite6-1.0.1/version.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-16 14:16:31.523256 quite6-1.0.2/
+-rw-r--r--   0 wangcong   (502) staff       (20)     1074 2024-05-14 10:15:26.000000 quite6-1.0.2/LICENSE
+-rw-r--r--   0 wangcong   (502) staff       (20)      104 2024-05-14 10:15:26.000000 quite6-1.0.2/MANIFEST.in
+-rw-r--r--   0 wangcong   (502) staff       (20)     3749 2024-05-16 14:16:31.522829 quite6-1.0.2/PKG-INFO
+-rw-r--r--   0 wangcong   (502) staff       (20)     2936 2024-05-14 10:15:26.000000 quite6-1.0.2/README.rst
+-rw-r--r--   0 wangcong   (502) staff       (20)        6 2024-05-16 14:16:10.000000 quite6-1.0.2/RELEASE-VERSION
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-16 14:16:31.403466 quite6-1.0.2/quite6/
+-rw-r--r--   0 wangcong   (502) staff       (20)      272 2024-05-14 11:46:55.000000 quite6-1.0.2/quite6/__init__.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-16 14:16:31.418006 quite6-1.0.2/quite6/controller/
+-rw-r--r--   0 wangcong   (502) staff       (20)      211 2024-05-13 08:52:57.000000 quite6-1.0.2/quite6/controller/__init__.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      606 2024-05-14 14:24:17.000000 quite6-1.0.2/quite6/controller/dialog_ui_controller.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2634 2024-05-14 14:24:17.000000 quite6-1.0.2/quite6/controller/file_dialog_controller.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1616 2024-05-14 14:24:17.000000 quite6-1.0.2/quite6/controller/widget_controller.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     3514 2024-05-14 03:41:05.000000 quite6-1.0.2/quite6/controller/widget_ui_controller.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-16 14:16:31.424983 quite6-1.0.2/quite6/core/
+-rw-r--r--   0 wangcong   (502) staff       (20)      203 2024-05-14 10:47:48.000000 quite6-1.0.2/quite6/core/__init__.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1326 2024-05-14 10:43:54.000000 quite6-1.0.2/quite6/core/event_loop.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      281 2024-05-14 10:43:54.000000 quite6-1.0.2/quite6/core/timer.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     3712 2024-05-14 15:04:01.000000 quite6-1.0.2/quite6/deferred_function.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-16 14:16:31.430913 quite6-1.0.2/quite6/gui/
+-rw-r--r--   0 wangcong   (502) staff       (20)     1118 2024-05-14 11:49:59.000000 quite6-1.0.2/quite6/gui/__init__.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-16 14:16:31.449722 quite6-1.0.2/quite6/gui/interfaces/
+-rw-r--r--   0 wangcong   (502) staff       (20)      554 2024-05-13 08:52:57.000000 quite6-1.0.2/quite6/gui/interfaces/__init__.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-16 14:16:31.455805 quite6-1.0.2/quite6/gui/interfaces/ability_interfaces/
+-rw-r--r--   0 wangcong   (502) staff       (20)      120 2024-05-13 08:52:57.000000 quite6-1.0.2/quite6/gui/interfaces/ability_interfaces/__init__.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      188 2024-05-13 08:52:57.000000 quite6-1.0.2/quite6/gui/interfaces/ability_interfaces/class_exec_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1092 2024-05-14 10:57:04.000000 quite6-1.0.2/quite6/gui/interfaces/ability_interfaces/container_ability_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      539 2024-05-14 03:20:46.000000 quite6-1.0.2/quite6/gui/interfaces/base_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      303 2024-05-13 08:52:57.000000 quite6-1.0.2/quite6/gui/interfaces/changed_signal_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      470 2024-05-14 08:19:12.000000 quite6-1.0.2/quite6/gui/interfaces/closed_signal_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      307 2024-05-14 10:57:04.000000 quite6-1.0.2/quite6/gui/interfaces/excited_signal_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      199 2024-05-14 10:57:04.000000 quite6-1.0.2/quite6/gui/interfaces/focus_in_signal_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      201 2024-05-14 10:57:04.000000 quite6-1.0.2/quite6/gui/interfaces/focus_out_signal_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      322 2024-05-14 10:57:04.000000 quite6-1.0.2/quite6/gui/interfaces/row_changed_signal_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      298 2024-05-13 08:52:57.000000 quite6-1.0.2/quite6/gui/interfaces/showed_signal_interface.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-16 14:16:31.458988 quite6-1.0.2/quite6/gui/layouts/
+-rw-r--r--   0 wangcong   (502) staff       (20)       40 2024-05-13 08:52:57.000000 quite6-1.0.2/quite6/gui/layouts/__init__.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2712 2024-05-14 14:37:29.000000 quite6-1.0.2/quite6/gui/layouts/square_layout.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-16 14:16:31.469203 quite6-1.0.2/quite6/gui/paint/
+-rw-r--r--   0 wangcong   (502) staff       (20)      129 2024-05-13 08:52:57.000000 quite6-1.0.2/quite6/gui/paint/__init__.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     5089 2024-05-14 14:37:29.000000 quite6-1.0.2/quite6/gui/paint/painter.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      502 2024-05-14 11:03:11.000000 quite6-1.0.2/quite6/gui/paint/pen.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      904 2024-05-14 11:03:11.000000 quite6-1.0.2/quite6/gui/paint/point.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      280 2024-05-14 11:03:11.000000 quite6-1.0.2/quite6/gui/paint/scaling.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1471 2024-05-14 11:03:11.000000 quite6-1.0.2/quite6/gui/paint/size.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      398 2024-05-14 10:17:44.000000 quite6-1.0.2/quite6/gui/qt_gui.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      311 2024-05-14 10:15:26.000000 quite6-1.0.2/quite6/gui/ui_extension.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-16 14:16:31.512239 quite6-1.0.2/quite6/gui/widgets/
+-rw-r--r--   0 wangcong   (502) staff       (20)      798 2024-05-14 11:10:25.000000 quite6-1.0.2/quite6/gui/widgets/__init__.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      383 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/action.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2454 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/combo_box.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      926 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/date_edit.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      683 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/date_time_edit.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      780 2024-05-14 11:51:50.000000 quite6-1.0.2/quite6/gui/widgets/dialog.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      195 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/dock_widget.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      721 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/double_spin_box.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      189 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/group_box.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1627 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/input_dialog.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      736 2024-05-14 14:37:29.000000 quite6-1.0.2/quite6/gui/widgets/label.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      183 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/layout.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1004 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/line_edit.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2347 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/list_widget.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      697 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/main_window.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2904 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/plot_widget.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      676 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/push_button.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      680 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/radio_button.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      582 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/shortcut.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      693 2024-05-14 11:54:28.000000 quite6-1.0.2/quite6/gui/widgets/spin_box.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     6529 2024-05-14 11:32:31.000000 quite6-1.0.2/quite6/gui/widgets/table_view.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     9397 2024-05-14 14:37:29.000000 quite6-1.0.2/quite6/gui/widgets/table_widget.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      720 2024-05-14 11:37:12.000000 quite6-1.0.2/quite6/gui/widgets/text_edit.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      926 2024-05-14 11:37:12.000000 quite6-1.0.2/quite6/gui/widgets/time_edit.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1326 2024-05-14 14:37:29.000000 quite6-1.0.2/quite6/gui/widgets/widget.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-16 14:16:31.518099 quite6-1.0.2/quite6/tools/
+-rw-r--r--   0 wangcong   (502) staff       (20)      110 2024-05-14 11:51:08.000000 quite6-1.0.2/quite6/tools/__init__.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1207 2024-05-15 06:35:06.000000 quite6-1.0.2/quite6/tools/load_qrc.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2461 2024-05-14 15:28:56.000000 quite6-1.0.2/quite6/tools/load_ui.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      315 2024-05-14 14:37:29.000000 quite6-1.0.2/quite6/tools/process.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-16 14:16:31.520023 quite6-1.0.2/quite6.egg-info/
+-rw-r--r--   0 wangcong   (502) staff       (20)     3749 2024-05-16 14:16:31.000000 quite6-1.0.2/quite6.egg-info/PKG-INFO
+-rw-r--r--   0 wangcong   (502) staff       (20)     2394 2024-05-16 14:16:31.000000 quite6-1.0.2/quite6.egg-info/SOURCES.txt
+-rw-r--r--   0 wangcong   (502) staff       (20)        1 2024-05-16 14:16:31.000000 quite6-1.0.2/quite6.egg-info/dependency_links.txt
+-rw-r--r--   0 wangcong   (502) staff       (20)       41 2024-05-16 14:16:31.000000 quite6-1.0.2/quite6.egg-info/requires.txt
+-rw-r--r--   0 wangcong   (502) staff       (20)        7 2024-05-16 14:16:31.000000 quite6-1.0.2/quite6.egg-info/top_level.txt
+-rw-r--r--   0 wangcong   (502) staff       (20)     2557 2024-05-14 10:15:26.000000 quite6-1.0.2/readme.md
+-rw-r--r--   0 wangcong   (502) staff       (20)       40 2024-05-16 14:15:45.000000 quite6-1.0.2/requirements.txt
+-rw-r--r--   0 wangcong   (502) staff       (20)      154 2024-05-16 14:16:31.524736 quite6-1.0.2/setup.cfg
+-rw-r--r--   0 wangcong   (502) staff       (20)     1633 2024-05-14 10:15:26.000000 quite6-1.0.2/setup.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2173 2024-05-14 10:15:26.000000 quite6-1.0.2/version.py
```

### Comparing `quite6-1.0.1/LICENSE` & `quite6-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/PKG-INFO` & `quite6-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quite6
-Version: 1.0.1
+Version: 1.0.2
 Summary: QT UI Extension
 Home-page: https://github.com/KD-Group/quite6
 Author: SF-Zhou
 Author-email: sfzhou.scut@gmail.com
 License: MIT
 Keywords: qt ui
 Classifier: Development Status :: 3 - Alpha
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: st
-Requires-Dist: prett6==1.2
+Requires-Dist: prett6
 Requires-Dist: PySide6
 Requires-Dist: typing
 Requires-Dist: pyqtgraph
 Requires-Dist: numpy
 
 quite6: QT UI Extension for Python3
 ==================================
```

### Comparing `quite6-1.0.1/README.rst` & `quite6-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/controller/dialog_ui_controller.py` & `quite6-1.0.2/quite6/controller/dialog_ui_controller.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/controller/file_dialog_controller.py` & `quite6-1.0.2/quite6/controller/file_dialog_controller.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/controller/widget_controller.py` & `quite6-1.0.2/quite6/controller/widget_controller.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/controller/widget_ui_controller.py` & `quite6-1.0.2/quite6/controller/widget_ui_controller.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/core/event_loop.py` & `quite6-1.0.2/quite6/core/event_loop.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/deferred_function.py` & `quite6-1.0.2/quite6/deferred_function.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/__init__.py` & `quite6-1.0.2/quite6/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/interfaces/__init__.py` & `quite6-1.0.2/quite6/gui/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/interfaces/ability_interfaces/container_ability_interface.py` & `quite6-1.0.2/quite6/gui/interfaces/ability_interfaces/container_ability_interface.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/interfaces/base_interface.py` & `quite6-1.0.2/quite6/gui/interfaces/base_interface.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/layouts/square_layout.py` & `quite6-1.0.2/quite6/gui/layouts/square_layout.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/paint/painter.py` & `quite6-1.0.2/quite6/gui/paint/painter.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/paint/point.py` & `quite6-1.0.2/quite6/gui/paint/point.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/paint/size.py` & `quite6-1.0.2/quite6/gui/paint/size.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/__init__.py` & `quite6-1.0.2/quite6/gui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/combo_box.py` & `quite6-1.0.2/quite6/gui/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/date_edit.py` & `quite6-1.0.2/quite6/gui/widgets/date_edit.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/date_time_edit.py` & `quite6-1.0.2/quite6/gui/widgets/date_time_edit.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/dialog.py` & `quite6-1.0.2/quite6/gui/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/double_spin_box.py` & `quite6-1.0.2/quite6/gui/widgets/double_spin_box.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/input_dialog.py` & `quite6-1.0.2/quite6/gui/widgets/input_dialog.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/label.py` & `quite6-1.0.2/quite6/gui/widgets/label.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/line_edit.py` & `quite6-1.0.2/quite6/gui/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/list_widget.py` & `quite6-1.0.2/quite6/gui/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/main_window.py` & `quite6-1.0.2/quite6/gui/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/plot_widget.py` & `quite6-1.0.2/quite6/gui/widgets/plot_widget.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/push_button.py` & `quite6-1.0.2/quite6/gui/widgets/push_button.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/radio_button.py` & `quite6-1.0.2/quite6/gui/widgets/radio_button.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/shortcut.py` & `quite6-1.0.2/quite6/gui/widgets/shortcut.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/spin_box.py` & `quite6-1.0.2/quite6/gui/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/table_view.py` & `quite6-1.0.2/quite6/gui/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/table_widget.py` & `quite6-1.0.2/quite6/gui/widgets/table_widget.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/text_edit.py` & `quite6-1.0.2/quite6/gui/widgets/text_edit.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/time_edit.py` & `quite6-1.0.2/quite6/gui/widgets/time_edit.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/gui/widgets/widget.py` & `quite6-1.0.2/quite6/gui/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/tools/load_qrc.py` & `quite6-1.0.2/quite6/tools/load_qrc.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6/tools/load_ui.py` & `quite6-1.0.2/quite6/tools/load_ui.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/quite6.egg-info/PKG-INFO` & `quite6-1.0.2/quite6.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quite6
-Version: 1.0.1
+Version: 1.0.2
 Summary: QT UI Extension
 Home-page: https://github.com/KD-Group/quite6
 Author: SF-Zhou
 Author-email: sfzhou.scut@gmail.com
 License: MIT
 Keywords: qt ui
 Classifier: Development Status :: 3 - Alpha
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: st
-Requires-Dist: prett6==1.2
+Requires-Dist: prett6
 Requires-Dist: PySide6
 Requires-Dist: typing
 Requires-Dist: pyqtgraph
 Requires-Dist: numpy
 
 quite6: QT UI Extension for Python3
 ==================================
```

### Comparing `quite6-1.0.1/quite6.egg-info/SOURCES.txt` & `quite6-1.0.2/quite6.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/readme.md` & `quite6-1.0.2/readme.md`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/setup.py` & `quite6-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.1/version.py` & `quite6-1.0.2/version.py`

 * *Files identical despite different names*

