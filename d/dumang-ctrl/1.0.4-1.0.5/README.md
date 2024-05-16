# Comparing `tmp/dumang_ctrl-1.0.4.tar.gz` & `tmp/dumang_ctrl-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumang_ctrl-1.0.4.tar", max compression
+gzip compressed data, was "dumang_ctrl-1.0.5.tar", max compression
```

## Comparing `dumang_ctrl-1.0.4.tar` & `dumang_ctrl-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2024-03-12 02:51:43.000000 dumang_ctrl-1.0.4/LICENSE
--rw-r--r--   0        0        0     1690 2024-03-23 05:53:52.000000 dumang_ctrl-1.0.4/README.md
--rw-r--r--   0        0        0      269 2024-03-15 21:49:22.000000 dumang_ctrl-1.0.4/dumang_ctrl/__init__.py
--rw-r--r--   0        0        0        0 2024-03-12 02:51:43.000000 dumang_ctrl-1.0.4/dumang_ctrl/dumang/__init__.py
--rw-r--r--   0        0        0      179 2024-03-14 22:10:35.000000 dumang_ctrl-1.0.4/dumang_ctrl/dumang/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    51833 2024-03-23 05:21:18.000000 dumang_ctrl-1.0.4/dumang_ctrl/dumang/__pycache__/common.cpython-311.pyc
--rw-r--r--   0        0        0    36432 2024-03-26 22:21:14.000000 dumang_ctrl-1.0.4/dumang_ctrl/dumang/common.py
--rw-r--r--   0        0        0     6409 2024-03-26 05:08:34.000000 dumang_ctrl-1.0.4/dumang_ctrl/dumang/gui.py
--rw-r--r--   0        0        0        0 2024-03-12 02:51:43.000000 dumang_ctrl-1.0.4/dumang_ctrl/tools/__init__.py
--rw-r--r--   0        0        0      178 2024-03-14 22:10:35.000000 dumang_ctrl-1.0.4/dumang_ctrl/tools/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    12982 2024-03-14 23:08:11.000000 dumang_ctrl-1.0.4/dumang_ctrl/tools/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     8610 2024-03-23 04:36:08.000000 dumang_ctrl-1.0.4/dumang_ctrl/tools/__pycache__/sync.cpython-311.pyc
--rw-r--r--   0        0        0     9902 2024-03-26 05:08:34.000000 dumang_ctrl-1.0.4/dumang_ctrl/tools/config.py
--rw-r--r--   0        0        0     4828 2024-03-26 22:19:33.000000 dumang_ctrl-1.0.4/dumang_ctrl/tools/sync.py
--rw-r--r--   0        0        0     1860 2024-04-11 04:11:32.769369 dumang_ctrl-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2430 1970-01-01 00:00:00.000000 dumang_ctrl-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-12 02:51:43.000000 dumang_ctrl-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1698 2024-04-11 04:30:57.737137 dumang_ctrl-1.0.5/README.md
+-rw-r--r--   0        0        0      269 2024-03-15 21:49:22.000000 dumang_ctrl-1.0.5/dumang_ctrl/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-12 02:51:43.000000 dumang_ctrl-1.0.5/dumang_ctrl/dumang/__init__.py
+-rw-r--r--   0        0        0      179 2024-03-14 22:10:35.000000 dumang_ctrl-1.0.5/dumang_ctrl/dumang/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    51833 2024-03-23 05:21:18.000000 dumang_ctrl-1.0.5/dumang_ctrl/dumang/__pycache__/common.cpython-311.pyc
+-rw-r--r--   0        0        0    36432 2024-03-26 22:21:14.000000 dumang_ctrl-1.0.5/dumang_ctrl/dumang/common.py
+-rw-r--r--   0        0        0     6347 2024-05-16 06:03:27.183469 dumang_ctrl-1.0.5/dumang_ctrl/dumang/gui.py
+-rw-r--r--   0        0        0        0 2024-03-12 02:51:43.000000 dumang_ctrl-1.0.5/dumang_ctrl/tools/__init__.py
+-rw-r--r--   0        0        0      178 2024-03-14 22:10:35.000000 dumang_ctrl-1.0.5/dumang_ctrl/tools/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    12982 2024-03-14 23:08:11.000000 dumang_ctrl-1.0.5/dumang_ctrl/tools/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     8610 2024-03-23 04:36:08.000000 dumang_ctrl-1.0.5/dumang_ctrl/tools/__pycache__/sync.cpython-311.pyc
+-rw-r--r--   0        0        0    10056 2024-05-16 06:02:32.170683 dumang_ctrl-1.0.5/dumang_ctrl/tools/config.py
+-rw-r--r--   0        0        0     4828 2024-03-26 22:19:33.000000 dumang_ctrl-1.0.5/dumang_ctrl/tools/sync.py
+-rw-r--r--   0        0        0     1860 2024-05-16 06:04:58.108067 dumang_ctrl-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2438 1970-01-01 00:00:00.000000 dumang_ctrl-1.0.5/PKG-INFO
```

### Comparing `dumang_ctrl-1.0.4/LICENSE` & `dumang_ctrl-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dumang_ctrl-1.0.4/README.md` & `dumang_ctrl-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 The PyPI package can be found at https://pypi.org/project/dumang-ctrl/
 
 ### Using Arch Linux
 
 ![ArchLinux](https://img.shields.io/badge/Arch_Linux-1793D1?style=for-the-badge&logo=arch-linux&logoColor=white)
 
-Using your AUR helper of choice install the `dumang-ctrl` [package](https://aur.archlinux.org/packages/dumang-ctrl).
+Using your AUR helper of choice install the `dumang-ctrl-git` [package](https://aur.archlinux.org/packages/dumang-ctrl-git).
 
 ## Usage
 
 Please refer to the [Github Pages](https://mayanez.github.io/dumang-keyboard-ctrl/) or `docs/`.
 
 ## Build (for Development)
```

### Comparing `dumang_ctrl-1.0.4/dumang_ctrl/dumang/__pycache__/common.cpython-311.pyc` & `dumang_ctrl-1.0.5/dumang_ctrl/dumang/__pycache__/common.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dumang_ctrl-1.0.4/dumang_ctrl/dumang/common.py` & `dumang_ctrl-1.0.5/dumang_ctrl/dumang/common.py`

 * *Files identical despite different names*

### Comparing `dumang_ctrl-1.0.4/dumang_ctrl/dumang/gui.py` & `dumang_ctrl-1.0.5/dumang_ctrl/dumang/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import sys
-
 from PyQt6 import QtGui
 from PyQt6.QtCore import *
 from PyQt6.QtWidgets import *
 
 from .common import *
 
 
@@ -66,15 +64,14 @@
         kbd.put(p)
         self._last_item = item
 
     def _on_itemLeave(self, kbd):
         p = LightPulsePacket(
             False, self.keys[self.item(self._last_item.row(), 0).data(0)].key)
         kbd.put(p)
-        pass
 
 
 class KBDWidget(QWidget):
 
     def __init__(self, parent, kbd):
         super(QWidget, self).__init__(parent)
         self.layout = QVBoxLayout(self)
@@ -99,15 +96,14 @@
 
 class KBDTab(QWidget):
 
     def __init__(self, parent, kbd):
         super(QWidget, self).__init__(parent)
         self.layout = QVBoxLayout(self)
         self.layout.setAlignment(Qt.AlignmentFlag.AlignTop)
-
         self.kbd_serial_label = QLabel(f"Board Serial: {kbd.serial}")
         self.layout.addWidget(self.kbd_serial_label)
         self.kbd_firmware_label = QLabel(
             f"Firmware: v{kbd.version[0]}.{kbd.version[1]}")
         self.layout.addWidget(self.kbd_firmware_label)
 
         # TODO: Refresh Button & Display DKM Firmware Versions & Color
@@ -148,15 +144,14 @@
 
         # Add tabs to widget
         self.layout.addWidget(self.tabs)
         self.setLayout(self.layout)
 
     @pyqtSlot()
     def on_click(self):
-        print("\n")
         for currentQTableWidgetItem in self.tableWidget.selectedItems():
             print(currentQTableWidgetItem.row(),
                   currentQTableWidgetItem.column(),
                   currentQTableWidgetItem.text())
 
 
 class App(QMainWindow):
@@ -169,20 +164,19 @@
         self.width = 500
         self.height = 500
         self.setWindowTitle(self.title)
         self.setGeometry(self.left, self.top, self.width, self.height)
         self.center()
 
     def center(self):
-        pass
         centerPoint = QtGui.QGuiApplication.primaryScreen().availableGeometry(
         ).center()
         self.move(centerPoint - self.frameGeometry().center())
 
 
 def inspect_gui(kbd1, kbd2=None):
     init = QApplication([])
     app = App()
     kbds = [kbd for kbd in [kbd1, kbd2] if kbd is not None]
     app.setCentralWidget(KBDTabs(app, kbds))
     app.show()
-    sys.exit(init.exec())
+    return init.exec()
```

### Comparing `dumang_ctrl-1.0.4/dumang_ctrl/tools/__pycache__/config.cpython-311.pyc` & `dumang_ctrl-1.0.5/dumang_ctrl/tools/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dumang_ctrl-1.0.4/dumang_ctrl/tools/__pycache__/sync.cpython-311.pyc` & `dumang_ctrl-1.0.5/dumang_ctrl/tools/__pycache__/sync.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dumang_ctrl-1.0.4/dumang_ctrl/tools/config.py` & `dumang_ctrl-1.0.5/dumang_ctrl/tools/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,16 +311,26 @@
 
 
 @cli.command(help="Inspect the current configuration via a GUI")
 @click.pass_context
 def inspect(ctx):
     logger.info("Launching GUI")
     from dumang_ctrl.dumang.gui import inspect_gui
+    kbds = ctx.obj[CTX_KEYBOARDS_KEY]
+    threads = ctx.obj[CTX_THREADS_KEY]
 
-    inspect_gui(*ctx.obj[CTX_KEYBOARDS_KEY])
+    gui = inspect_gui(*kbds)
 
-    for t in ctx.obj[CTX_THREADS_KEY]:
+    for kbd in kbds:
+        kbd.kill_threads()
+
+    for t in threads:
         t.join()
 
+    for kbd in kbds:
+        kbd.close()
+
+    sys.exit(gui)
+
 
 if __name__ == "__main__":
     cli(obj={})
```

### Comparing `dumang_ctrl-1.0.4/dumang_ctrl/tools/sync.py` & `dumang_ctrl-1.0.5/dumang_ctrl/tools/sync.py`

 * *Files identical despite different names*

### Comparing `dumang_ctrl-1.0.4/pyproject.toml` & `dumang_ctrl-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dumang-ctrl"
-version = "1.0.4"
+version = "1.0.5"
 description = "Dumang DK6 Tools"
 authors = ["Miguel A. Arroyo <email@arroyo.me>"]
 repository = "https://github.com/mayanez/dumang-keyboard-ctrl"
 documentation = "https://mayanez.github.io/dumang-keyboard-ctrl/"
 readme = "README.md"
 license = "LICENSE"
 packages = [
```

### Comparing `dumang_ctrl-1.0.4/PKG-INFO` & `dumang_ctrl-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumang-ctrl
-Version: 1.0.4
+Version: 1.0.5
 Summary: Dumang DK6 Tools
 Home-page: https://github.com/mayanez/dumang-keyboard-ctrl
 License: LICENSE
 Author: Miguel A. Arroyo
 Author-email: email@arroyo.me
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
@@ -51,15 +51,15 @@
 
 The PyPI package can be found at https://pypi.org/project/dumang-ctrl/
 
 ### Using Arch Linux
 
 ![ArchLinux](https://img.shields.io/badge/Arch_Linux-1793D1?style=for-the-badge&logo=arch-linux&logoColor=white)
 
-Using your AUR helper of choice install the `dumang-ctrl` [package](https://aur.archlinux.org/packages/dumang-ctrl).
+Using your AUR helper of choice install the `dumang-ctrl-git` [package](https://aur.archlinux.org/packages/dumang-ctrl-git).
 
 ## Usage
 
 Please refer to the [Github Pages](https://mayanez.github.io/dumang-keyboard-ctrl/) or `docs/`.
 
 ## Build (for Development)
```

