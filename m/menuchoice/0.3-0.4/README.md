# Comparing `tmp/menuchoice-0.3.tar.gz` & `tmp/menuchoice-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "menuchoice-0.3.tar", last modified: Sun May 12 03:46:58 2024, max compression
+gzip compressed data, was "menuchoice-0.4.tar", last modified: Thu May 16 03:47:23 2024, max compression
```

## Comparing `menuchoice-0.3.tar` & `menuchoice-0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-12 03:46:58.709096 menuchoice-0.3/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1793 2024-05-12 03:46:58.709096 menuchoice-0.3/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1055 2024-05-12 03:45:48.000000 menuchoice-0.3/README.md
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-12 03:46:58.709096 menuchoice-0.3/menuchoice/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     4916 2024-05-12 02:28:07.000000 menuchoice-0.3/menuchoice/__init__.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      643 2024-05-10 05:16:56.000000 menuchoice-0.3/menuchoice/_validator.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-12 03:46:58.709096 menuchoice-0.3/menuchoice/cursor_control/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     6201 2024-05-12 03:37:00.000000 menuchoice-0.3/menuchoice/cursor_control/_cursorInput.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      142 2024-05-10 03:13:36.000000 menuchoice-0.3/menuchoice/exceptions.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-12 03:46:58.709096 menuchoice-0.3/menuchoice.egg-info/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1793 2024-05-12 03:46:58.000000 menuchoice-0.3/menuchoice.egg-info/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      269 2024-05-12 03:46:58.000000 menuchoice-0.3/menuchoice.egg-info/SOURCES.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-05-12 03:46:58.000000 menuchoice-0.3/menuchoice.egg-info/dependency_links.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       11 2024-05-12 03:46:58.000000 menuchoice-0.3/menuchoice.egg-info/top_level.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-05-12 03:46:58.709096 menuchoice-0.3/setup.cfg
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1028 2024-05-10 10:49:41.000000 menuchoice-0.3/setup.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-16 03:47:23.256565 menuchoice-0.4/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1844 2024-05-16 03:47:23.256565 menuchoice-0.4/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1055 2024-05-12 03:45:48.000000 menuchoice-0.4/README.md
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-16 03:47:23.255565 menuchoice-0.4/menuchoice/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     5408 2024-05-14 04:16:08.000000 menuchoice-0.4/menuchoice/__init__.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      643 2024-05-10 05:16:56.000000 menuchoice-0.4/menuchoice/_validator.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-16 03:47:23.255565 menuchoice-0.4/menuchoice/cursor_control/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     7161 2024-05-16 03:40:53.000000 menuchoice-0.4/menuchoice/cursor_control/_cursorInput.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      882 2024-05-14 10:44:56.000000 menuchoice-0.4/menuchoice/cursor_control/_textHandler.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      142 2024-05-10 03:13:36.000000 menuchoice-0.4/menuchoice/exceptions.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-16 03:47:23.256565 menuchoice-0.4/menuchoice.egg-info/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1844 2024-05-16 03:47:23.000000 menuchoice-0.4/menuchoice.egg-info/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      311 2024-05-16 03:47:23.000000 menuchoice-0.4/menuchoice.egg-info/SOURCES.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-05-16 03:47:23.000000 menuchoice-0.4/menuchoice.egg-info/dependency_links.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       11 2024-05-16 03:47:23.000000 menuchoice-0.4/menuchoice.egg-info/top_level.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-05-16 03:47:23.256565 menuchoice-0.4/setup.cfg
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1078 2024-05-16 03:44:34.000000 menuchoice-0.4/setup.py
```

### Comparing `menuchoice-0.3/PKG-INFO` & `menuchoice-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: menuchoice
-Version: 0.3
+Version: 0.4
 Summary: Command line menu selector.
 Home-page: https://github.com/xyzpw/menuchoice/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Keywords: menu selector,item selector,ansi
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
```

### Comparing `menuchoice-0.3/README.md` & `menuchoice-0.4/README.md`

 * *Files identical despite different names*

### Comparing `menuchoice-0.3/menuchoice/__init__.py` & `menuchoice-0.4/menuchoice/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import curses
 import re
 from .cursor_control import _cursorInput
 from .exceptions import *
 from . import _validator
 
-__version__ = "0.3"
+__version__ = "0.4"
 __author__ = "xyzpw"
 __description__ = "Command line menu selector."
 __license__ = "MIT"
 
 class MenuSelector:
     """Contains items which can be prompted via a menu selector."""
     def __init__(self, items: list | dict, title: str = None, description: str = None):
@@ -79,7 +79,15 @@
             usrChoices = [(i, list(self.items)[i]) for i in selectedIndexes] if selectedIndexes != None else []
         else:
             selectedIndexes = curses.wrapper(_cursorInput.cursorArrowMenu, menu, arrow, center)
             usrChoices = [(selectedIndexes, list(self.items)[selectedIndexes])] if selectedIndexes != None else []
         if not _validator.validateItemSelectionCount(max_items, usrChoices):
             raise MenuItemError("number of items selected is out of range")
         return usrChoices
+    def highlight_select(self, center: bool = False):
+        """Highlights the options at the current line index.
+
+        :param center: positions the menu selector to the center of the terminal"""
+        menuComponents = self.items, self.title, self.description
+        selectedIndex = curses.wrapper(_cursorInput.highlightSelectMenu, menuComponents, center)
+        usrChoice = [(selectedIndex, list(self.items)[selectedIndex])] if selectedIndex != None else []
+        return usrChoice
```

### Comparing `menuchoice-0.3/menuchoice/_validator.py` & `menuchoice-0.4/menuchoice/_validator.py`

 * *Files identical despite different names*

### Comparing `menuchoice-0.3/menuchoice/cursor_control/_cursorInput.py` & `menuchoice-0.4/menuchoice/cursor_control/_cursorInput.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import curses
 import re
 import shutil
+from . import _textHandler
 
 def getMenuComponents(menuString: str):
     menuLines = menuString.splitlines()
     for l in range(len(menuLines)):
         if re.search(r"^0.\s.*?(?=$|\s)", menuLines[l]) != None:
             meta = menuLines[:l] if l != 0 else None
             menuLines = menuLines[l:]
@@ -29,19 +30,15 @@
     while True:
         stdscr.clear()
         stdscr.refresh()
         menuLines, menuMeta = getMenuComponents(menuString)
         rewrittenMenu = rewriteMenu(menuString, menuArrow, currentLineIndex)
         if menuMeta != None:
             if center:
-                lengthiestStr = 0
-                for s in menuMeta:
-                    lengthiestStr = len(s) if len(s) > lengthiestStr else lengthiestStr
-                metaSpacing = getCenteredPos()[0] - lengthiestStr//2
-                menuMeta = [f"{metaSpacing * ' '}{menuMeta[i]}" for i in range(len(menuMeta))]
+                menuMeta = _textHandler.centerArrayItems(menuMeta)
             stdscr.addstr("\n\n".join(menuMeta) + "\n\n")
         if center: rewrittenMenu = makeStrCentered(rewrittenMenu, True)
         stdscr.addstr(rewrittenMenu, currentLineIndex)
         keyPressed = stdscr.getch()
         if keyPressed == curses.KEY_UP:
             nextLineIndex = currentLineIndex - 1
             currentLineIndex = nextLineIndex if currentLineIndex > 0 else len(menuLines) - 1
@@ -98,20 +95,16 @@
     stdscr.refresh()
     while True:
         stdscr.clear()
         menuLines, menuMeta = getMenuComponents(menuString)
         rewrittenMenu = rewriteMultiselectMenu(menuString, currentLineIndex, selectedItems, allowAll)
         if menuMeta != None:
             if center:
-                lengthiestStr = 0
-                for s in menuMeta:
-                    lengthiestStr = len(s) if len(s) > lengthiestStr else lengthiestStr
-                metaSpacing = getCenteredPos()[0] - lengthiestStr//2
-                menuMeta = [f"{' '*metaSpacing}{menuMeta[i]}" for i in range(len(menuMeta))]
-                stdscr.addstr("\n\n".join(menuMeta) + "\n\n")
+                menuMeta = _textHandler.centerArrayItems(menuMeta)
+            stdscr.addstr("\n\n".join(menuMeta) + "\n\n")
         if center: rewrittenMenu = makeStrCentered(rewrittenMenu, True)
         stdscr.addstr(rewrittenMenu, currentLineIndex)
         keyPressed = stdscr.getch()
         if keyPressed == curses.KEY_UP:
             nextLineIndex = currentLineIndex - 1
             currentLineIndex = int(nextLineIndex) if currentLineIndex > 0 else len(menuLines) - 1
         elif keyPressed == curses.KEY_DOWN:
@@ -124,7 +117,36 @@
             if currentLineIndex == len(menuLines) - 1:
                 return selectedItems if bool(selectedItems) else None
             else:
                 if currentLineIndex not in selectedItems and (maxItemCount <= len(selectedItems) if maxItemCount != None else False):
                     continue
                 selectedItems.append(currentLineIndex) if not currentLineIndex in selectedItems else selectedItems.pop(selectedItems.index(currentLineIndex))
 
+
+def highlightSelectMenu(stdscr, menuComponents: tuple, center: bool = False):
+    curses.curs_set(0)
+    currentLineIndex = 0
+    menuLines: list = menuComponents[0]
+    menuTitle, menuDescription = menuComponents[1], menuComponents[2]
+    centerSpacing = _textHandler.getItemSpacing(menuLines)
+    while True:
+        stdscr.clear()
+        stdscr.refresh()
+        if menuTitle != None:
+            if center: stdscr.addstr(_textHandler.getItemSpacing([menuTitle]))
+            stdscr.addstr(menuTitle + "\n\n")
+        if menuDescription != None:
+            if center: stdscr.addstr(_textHandler.getItemSpacing([menuDescription]))
+            stdscr.addstr(menuDescription + "\n\n")
+        if center: stdscr.addstr(_textHandler.getCenteredNewlines(menuLines))
+        for l in menuLines:
+            _strToAdd = "%s\n" % l
+            if center: stdscr.addstr(centerSpacing)
+            stdscr.addstr(_strToAdd) if menuLines.index(l) != currentLineIndex else stdscr.addstr(_strToAdd, curses.A_REVERSE)
+            del _strToAdd
+        keyPressed = stdscr.getch()
+        if keyPressed == curses.KEY_DOWN:
+            currentLineIndex = currentLineIndex + 1 if currentLineIndex != len(menuLines) - 1 else 0
+        elif keyPressed == curses.KEY_UP:
+            currentLineIndex = currentLineIndex - 1 if currentLineIndex != 0 else len(menuLines) - 1
+        elif keyPressed in [curses.KEY_ENTER, 10]:
+            return currentLineIndex
```

### Comparing `menuchoice-0.3/menuchoice.egg-info/PKG-INFO` & `menuchoice-0.4/menuchoice.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: menuchoice
-Version: 0.3
+Version: 0.4
 Summary: Command line menu selector.
 Home-page: https://github.com/xyzpw/menuchoice/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Keywords: menu selector,item selector,ansi
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
```

### Comparing `menuchoice-0.3/setup.py` & `menuchoice-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     url="https://github.com/xyzpw/menuchoice/",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Environment :: Console",
         "Environment :: Console :: Curses",
         "Intended Audience :: Developers",
     ],
     keywords=[
```

