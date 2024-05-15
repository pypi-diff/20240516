# Comparing `tmp/guibbon-0.1.5.tar.gz` & `tmp/guibbon-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guibbon-0.1.5.tar", max compression
+gzip compressed data, was "guibbon-0.2.0.tar", max compression
```

## Comparing `guibbon-0.1.5.tar` & `guibbon-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0    17803 2024-03-22 15:15:25.978749 guibbon-0.1.5/guibbon/__init__.py
--rw-r--r--   0        0        0      115 2024-03-22 15:15:25.979762 guibbon-0.1.5/guibbon/colors.py
--rw-r--r--   0        0        0    10151 2024-03-22 15:15:25.979762 guibbon-0.1.5/guibbon/image_viewer.py
--rw-r--r--   0        0        0    14678 2024-03-22 15:15:25.980761 guibbon-0.1.5/guibbon/interactive_overlays.py
--rw-r--r--   0        0        0     3619 2024-03-22 15:15:25.981795 guibbon-0.1.5/guibbon/keyboard_event_handler.py
--rw-r--r--   0        0        0     1971 2024-03-22 15:15:25.981795 guibbon-0.1.5/guibbon/transform_matrix.py
--rw-r--r--   0        0        0     1338 2024-03-22 15:15:25.982806 guibbon-0.1.5/guibbon/typedef.py
--rw-r--r--   0        0        0      595 2024-03-22 15:15:25.983805 guibbon-0.1.5/guibbon/widgets/button_widget.py
--rw-r--r--   0        0        0     1556 2024-03-22 15:15:25.983805 guibbon-0.1.5/guibbon/widgets/check_button_list_widget.py
--rw-r--r--   0        0        0      900 2024-03-22 15:15:26.002393 guibbon-0.1.5/guibbon/widgets/check_button_widget.py
--rw-r--r--   0        0        0     2171 2024-03-22 15:15:26.003405 guibbon-0.1.5/guibbon/widgets/color_picker_widget.py
--rw-r--r--   0        0        0     2611 2024-03-22 15:15:26.004402 guibbon-0.1.5/guibbon/widgets/radio_buttons_widget.py
--rw-r--r--   0        0        0     1718 2024-03-22 15:15:26.004402 guibbon-0.1.5/guibbon/widgets/slider_widget.py
--rw-r--r--   0        0        0      182 2024-03-22 15:15:26.005402 guibbon-0.1.5/guibbon/widgets/widget.py
--rw-r--r--   0        0        0    35823 2024-03-22 15:06:53.741731 guibbon-0.1.5/LICENSE
--rw-r--r--   0        0        0     1880 2024-03-24 00:03:52.577545 guibbon-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      795 2024-03-24 00:05:13.374398 guibbon-0.1.5/README_user.md
--rw-r--r--   0        0        0     1681 1970-01-01 00:00:00.000000 guibbon-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1119 2024-05-15 19:03:45.959060 guibbon-0.2.0/docs/index.md
+-rw-r--r--   0        0        0    19225 2024-05-15 21:12:18.939024 guibbon-0.2.0/guibbon/__init__.py
+-rw-r--r--   0        0        0      115 2024-04-26 16:30:25.103312 guibbon-0.2.0/guibbon/colors.py
+-rw-r--r--   0        0        0     1951 2024-05-15 19:03:45.970011 guibbon-0.2.0/guibbon/icons/icon32.png
+-rw-r--r--   0        0        0    10339 2024-05-15 19:03:45.971080 guibbon-0.2.0/guibbon/image_viewer.py
+-rw-r--r--   0        0        0    14678 2024-04-26 16:30:25.106312 guibbon-0.2.0/guibbon/interactive_overlays.py
+-rw-r--r--   0        0        0     3619 2024-04-26 16:30:25.107312 guibbon-0.2.0/guibbon/keyboard_event_handler.py
+-rw-r--r--   0        0        0     1971 2024-04-26 16:30:25.108312 guibbon-0.2.0/guibbon/transform_matrix.py
+-rw-r--r--   0        0        0     1350 2024-05-15 19:03:45.972197 guibbon-0.2.0/guibbon/typedef.py
+-rw-r--r--   0        0        0      595 2024-04-26 16:30:25.109311 guibbon-0.2.0/guibbon/widgets/button_widget.py
+-rw-r--r--   0        0        0     1556 2024-04-26 16:30:25.109311 guibbon-0.2.0/guibbon/widgets/check_button_list_widget.py
+-rw-r--r--   0        0        0      900 2024-04-26 16:30:25.110312 guibbon-0.2.0/guibbon/widgets/check_button_widget.py
+-rw-r--r--   0        0        0     2259 2024-05-15 19:03:45.973337 guibbon-0.2.0/guibbon/widgets/color_picker_widget.py
+-rw-r--r--   0        0        0     2611 2024-04-26 16:30:25.156312 guibbon-0.2.0/guibbon/widgets/radio_buttons_widget.py
+-rw-r--r--   0        0        0     1973 2024-05-15 19:03:45.974240 guibbon-0.2.0/guibbon/widgets/slider_widget.py
+-rw-r--r--   0        0        0     3511 2024-05-15 19:03:45.975288 guibbon-0.2.0/guibbon/widgets/treeview_widget.py
+-rw-r--r--   0        0        0      182 2024-04-26 16:30:25.182314 guibbon-0.2.0/guibbon/widgets/widget.py
+-rw-r--r--   0        0        0    35823 2024-04-26 16:30:24.817313 guibbon-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1981 2024-05-15 19:03:45.978573 guibbon-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1944 1970-01-01 00:00:00.000000 guibbon-0.2.0/PKG-INFO
```

### Comparing `guibbon-0.1.5/guibbon/__init__.py` & `guibbon-0.2.0/guibbon/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+import re
 import time
 import tkinter as tk
 from typing import Dict, Optional, Type, List, Sequence, Any, Tuple
 
 import cv2
 import numpy as np
 
@@ -11,18 +13,37 @@
 from .typedef import Image_t, CallbackPoint, CallbackPolygon, CallbackRect, Point2DList, InteractivePolygon, CallbackMouse
 from .widgets.button_widget import ButtonWidget, CallbackButton
 from .widgets.check_button_list_widget import CheckButtonListWidget, CallbackCheckButtonList
 from .widgets.check_button_widget import CheckButtonWidget, CallbackCheckButton
 from .widgets.color_picker_widget import ColorPickerWidget, CallbackColorPicker
 from .widgets.radio_buttons_widget import RadioButtonsWidget, CallbackRadioButtons
 from .widgets.slider_widget import SliderWidget, CallbackSlider
+from .widgets.treeview_widget import TreeviewWidget, CallbackTreeview, TreeNode
 from .widgets.widget import WidgetInterface
 
-__version__ = "0.0.0"
-__version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
+__version__ = "0.2.0"
+
+
+def compute_version_info():
+    mtch = re.match(r"(\d+).(\d+).(\d+)((-dev)?)$", __version__)
+
+    if mtch is None:
+        return [(0, 0, 0), ""]
+
+    major = mtch.group(1)
+    minor = mtch.group(2)
+    build_nb = mtch.group(3)
+
+    count: int = 0 if mtch.lastindex is None else mtch.lastindex
+    mode = "dev" if count >= 4 else ""
+
+    return [(major, minor, build_nb), mode]
+
+
+__version_info__ = compute_version_info()
 
 
 def inject(cv2_package):
     cv2_package.createTrackbar = createTrackbar
     cv2_package.destroyAllWindows = not_implemented_error
     cv2_package.destroyWindow = not_implemented_error
     cv2_package.getMouseWheelDelta = not_implemented_error
@@ -174,14 +195,18 @@
     return Guibbon.get_instance(winname).create_check_button_list(name, options, on_change, initial_values)
 
 
 def create_color_picker(winname: str, name: str, on_change: CallbackColorPicker, initial_color_rgb: Optional[Tuple[int, int, int]] = None) -> ColorPickerWidget:
     return Guibbon.get_instance(winname).create_color_picker(name, on_change, initial_color_rgb)
 
 
+def create_treeview(winname: str, name: str, tree: TreeNode, on_click: CallbackTreeview) -> TreeviewWidget:
+    return Guibbon.get_instance(winname).create_treeview(name, tree, on_click)
+
+
 def createInteractivePoint(
         windowName,
         point_xy,
         label="",
         on_click: CallbackPoint = None,
         on_drag: CallbackPoint = None,
         on_release: CallbackPoint = None,
@@ -195,14 +220,17 @@
         point_xy_list,
         label="",
         on_click: CallbackPolygon = None,
         on_drag: CallbackPolygon = None,
         on_release: CallbackPolygon = None,
         magnet_points: Optional[Point2DList] = None,
 ) -> InteractivePolygon:
+    """
+    Draws a polygon over the displayed image. The corners of the polygon can be dragged by the user, triggering a callback.
+    """
     ipolygon: InteractivePolygon
     ipolygon = Guibbon.get_instance(windowName).image_viewer.createInteractivePolygon(point_xy_list, label, on_click, on_drag, on_release, magnet_points)
     return ipolygon
 
 
 def createInteractiveRectangle(
         windowName,
@@ -210,20 +238,23 @@
         point1_xy,
         label="",
         on_click: CallbackRect = None,
         on_drag: CallbackRect = None,
         on_release: CallbackRect = None,
         magnet_points: Optional[Point2DList] = None,
 ) -> InteractivePolygon:
+    """Create and returns object of type createInteractiveRectangle windows named windowName."""
     irect: InteractivePolygon
     irect = Guibbon.get_instance(windowName).image_viewer.createInteractiveRectangle(point0_xy, point1_xy, label, on_click, on_drag, on_release, magnet_points)
     return irect
 
 
 class Guibbon:
+    """The Guibbon object contains the list of open windows"""
+
     root: tk.Tk
     is_alive: bool = False
     instances: Dict[str, "Guibbon"] = {}
     active_instance_name: Optional[str]
     is_timeout: bool
     keyboard: KeyboardEventHandler
 
@@ -294,14 +325,16 @@
             Guibbon.init()
 
         # Make master root windows invisible
         self.window = tk.Toplevel(Guibbon.root)  # type: ignore
         self.window.protocol("WM_DELETE_WINDOW", self.on_closing)  # add callback when user closes the window
         self.winname = winname
         self.window.title(self.winname)
+        icon = tk.PhotoImage(file=os.path.join(os.path.dirname(__file__), "icons", "icon32.png"))
+        self.window.iconphoto(False, icon)
 
         self.window.bind("<KeyPress>", Guibbon.keyboard.on_event)
         self.window.bind("<KeyRelease>", Guibbon.keyboard.on_event)
 
         self.frame = tk.Frame(master=self.window, bg=COLORS.background)
 
         # Load an image in the script
@@ -389,14 +422,20 @@
 
     def create_color_picker(self, name: str, on_change: CallbackColorPicker, initial_color_rgb: Optional[Tuple[int, int, int]] = None) -> ColorPickerWidget:
         tk_frame = tk.Frame(self.ctrl_frame)
         cpw = ColorPickerWidget(tk_frame, name, on_change, initial_color_rgb)
         tk_frame.pack(padx=4, pady=4, side=tk.TOP, fill=tk.X, expand=1)
         return cpw
 
+    def create_treeview(self, name: str, tree: TreeNode, on_click: CallbackTreeview) -> TreeviewWidget:
+        tk_frame = tk.Frame(self.ctrl_frame)
+        widget = TreeviewWidget(tk_frame, name, tree, on_click)
+        tk_frame.pack(padx=4, pady=4, side=tk.TOP, fill=tk.X, expand=1)
+        return widget
+
     def imshow(self, mat: Image_t, mode: Optional[str] = None, cv2_interpolation: Optional[int] = None):
         self.image_viewer.imshow(mat, mode, cv2_interpolation)
 
     def getWindowProperty(self, prop_id: int) -> float:
         """
         TODO: not all flags ar handled
             cv2.WND_PROP_FULLSCREEN:    fullscreen property (can be WINDOW_NORMAL or WINDOW_FULLSCREEN).
```

### Comparing `guibbon-0.1.5/guibbon/image_viewer.py` & `guibbon-0.2.0/guibbon/image_viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         if not isinstance(onMouse, types.FunctionType) and not isinstance(onMouse, types.MethodType):
             raise TypeError(f"onMouse must be a function, got {type(onMouse)} instead")
         if userdata is not None:
             raise NotImplementedError("userdata argument of function setMouseCallback is not handled in current version of guibbon")
 
         if self.onMouse is None:
             # <MODIFIER-MODIFIER-TYPE-DETAIL>
+            # see https://dafarry.github.io/tkinterbook/tkinter-events-and-bindings.htm
             self.canvas.bind("<Motion>", self.on_event)
             self.canvas.bind("<ButtonPress>", self.on_event)
             self.canvas.bind("<ButtonRelease>", self.on_event)
             self.canvas.bind("<MouseWheel>", self.on_event)
 
         self.onMouse = onMouse
 
@@ -221,14 +222,18 @@
 
     def imshow(self, mat: Image_t, mode: Optional[str] = None, cv2_interpolation: Optional[int] = None):
         mode = "fit" if mode is None else mode
         cv2_interpolation = cv2.INTER_LINEAR if cv2_interpolation is None else cv2_interpolation
 
         canh, canw = self.canvas_shape_hw
         imgh, imgw = mat.shape[:2]
+
+        if mat.dtype == float:
+            mat = (np.clip(mat, 0, 1) * 255).astype(np.uint8)
+
         mat = cv2.cvtColor(mat, cv2.COLOR_BGR2RGB)  # type: ignore
 
         img_space_matrix: TransformMatrix
         can_space_matrix: TransformMatrix
         if mode == "fit":
             img_space_matrix = tm.T((imgw / 2, imgh / 2)) @ tm.S((max(imgw, imgh), max(imgw, imgh)))
             can_space_matrix = tm.T((canw / 2, canh / 2)) @ tm.S((max(canw, canh), max(canw, canh)))
```

### Comparing `guibbon-0.1.5/guibbon/interactive_overlays.py` & `guibbon-0.2.0/guibbon/interactive_overlays.py`

 * *Files identical despite different names*

### Comparing `guibbon-0.1.5/guibbon/keyboard_event_handler.py` & `guibbon-0.2.0/guibbon/keyboard_event_handler.py`

 * *Files identical despite different names*

### Comparing `guibbon-0.1.5/guibbon/transform_matrix.py` & `guibbon-0.2.0/guibbon/transform_matrix.py`

 * *Files identical despite different names*

### Comparing `guibbon-0.1.5/guibbon/typedef.py` & `guibbon-0.2.0/guibbon/typedef.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 Point2D = Tuple[float, float]
 
 Point2DList = List[Point2D]
 
 CallbackRadioButtons = Optional[Callable[[int, str], NoReturn]]
 
 # foo(event) -> None
-CallbackPoint = Optional[Callable[[tk.Event], NoReturn]]
+CallbackPoint = Optional[Callable[[tk.EventType], NoReturn]]
 
 # foo(event, point_xy_list) -> None
-CallbackPolygon = Optional[Callable[[tk.Event, Point2DList], NoReturn]]
+CallbackPolygon = Optional[Callable[[tk.EventType, Point2DList], NoReturn]]
 
 # foo(event, point0_xy, point1_xy) -> None
-CallbackRect = Optional[Callable[[tk.Event, Point2D, Point2D], NoReturn]]
+CallbackRect = Optional[Callable[[tk.EventType, Point2D, Point2D], NoReturn]]
 
 # foo(cvevent, x, y, flag, param) -> None
 CallbackMouse = Optional[Callable[[int, int, int, int, None], NoReturn]]
 
 
 class InteractivePoint(metaclass=abc.ABCMeta):
     @abc.abstractmethod
```

### Comparing `guibbon-0.1.5/guibbon/widgets/button_widget.py` & `guibbon-0.2.0/guibbon/widgets/button_widget.py`

 * *Files identical despite different names*

### Comparing `guibbon-0.1.5/guibbon/widgets/check_button_list_widget.py` & `guibbon-0.2.0/guibbon/widgets/check_button_list_widget.py`

 * *Files identical despite different names*

### Comparing `guibbon-0.1.5/guibbon/widgets/check_button_widget.py` & `guibbon-0.2.0/guibbon/widgets/check_button_widget.py`

 * *Files identical despite different names*

### Comparing `guibbon-0.1.5/guibbon/widgets/color_picker_widget.py` & `guibbon-0.2.0/guibbon/widgets/color_picker_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,21 +36,22 @@
         for c in initial_color_rgb:
             assert isinstance(c, int)
         assert min(initial_color_rgb) >= 0
         assert max(initial_color_rgb) <= 255
         self.color_rgb: Tuple[int, int, int] = initial_color_rgb
 
         color_hex = convert_color_tuple3i_to_hexastr(self.color_rgb)
-        self.canvas = tk.Canvas(self.frame, bg=color_hex, bd=2, height=10)
-        self.canvas.bind("<Button-1>", self.callback)
+        self.canvas = tk.Canvas(self.frame, bg=color_hex, bd=3, height=10)
+        self.button = tk.Button(self.frame, text="Edit", command=self.callback)
 
-        self.canvas.pack(side=tk.LEFT, anchor=tk.W)
+        self.canvas.pack(padx=2, side=tk.LEFT, anchor=tk.W)
+        self.button.pack(padx=2, side=tk.LEFT, anchor=tk.W)
         self.frame.pack(padx=4, pady=4, side=tk.TOP, fill=tk.X, expand=1)
 
-    def callback(self, event):
+    def callback(self):
         colors = askcolor(title="Color Chooser")
         if colors[0] is not None:
             r, g, b = colors[0]
             self.color_rgb = (r, g, b)
         self.canvas["bg"] = convert_color_tuple3i_to_hexastr(self.color_rgb)
         self.on_change(self.color_rgb)
```

### Comparing `guibbon-0.1.5/guibbon/widgets/radio_buttons_widget.py` & `guibbon-0.2.0/guibbon/widgets/radio_buttons_widget.py`

 * *Files identical despite different names*

### Comparing `guibbon-0.1.5/guibbon/widgets/slider_widget.py` & `guibbon-0.2.0/guibbon/widgets/slider_widget.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 import tkinter as tk
 from typing import Callable, Any, Sequence
 
 CallbackSlider = Callable[[int, Any], None]
+
+
 class SliderWidget:
     def __init__(self, tk_frame: tk.Frame, slider_name: str, values: Sequence[Any], initial_index: int, on_change: CallbackSlider, widget_color):
-        self.name = slider_name
+        self.name = tk.StringVar()
+        self.name.set(slider_name)
+
         self.values = values
         self.on_change = on_change
         self.value_var = tk.StringVar()
 
-        tk.Label(tk_frame, text=self.name, bg=widget_color).pack(padx=2, side=tk.LEFT)
+        tk.Label(tk_frame, textvariable=self.name, bg=widget_color).pack(padx=2, side=tk.LEFT)
         self.value_var.set(self.values[initial_index])
         tk.Label(tk_frame, textvariable=self.value_var, bg=widget_color).pack(padx=2, side=tk.TOP)
         count = len(self.values)
         self.tk_scale = tk.Scale(tk_frame, from_=0, to=count - 1, orient=tk.HORIZONTAL, bg=widget_color, borderwidth=0, showvalue=False)
         self.tk_scale.set(initial_index)
 
         self.tk_scale["command"] = self.callback
         self.tk_scale.pack(padx=2, fill=tk.X, expand=1)
 
+    def __setattr__(self, key, value):
+        if key == "name" and key in self.__dict__.keys():
+            self.name.set(value)
+        else:
+            return super().__setattr__(key, value)
+
     def callback(self, index):
         val = self.values[int(index)]
         self.value_var.set(val)
         return self.on_change(index, val)
 
     def set_index(self, index, trigger_callback=True):
         self.tk_scale.set(index)
```

### Comparing `guibbon-0.1.5/LICENSE` & `guibbon-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `guibbon-0.1.5/pyproject.toml` & `guibbon-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,118 +1,124 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2267 7569 6262 6f6e 220d  ame = "guibbon".
-00000020: 0a76 6572 7369 6f6e 203d 2022 302e 312e  .version = "0.1.
-00000030: 3522 0d0a 6465 7363 7269 7074 696f 6e20  5"..description 
+00000020: 0a76 6572 7369 6f6e 203d 2022 302e 322e  .version = "0.2.
+00000030: 3022 0d0a 6465 7363 7269 7074 696f 6e20  0"..description 
 00000040: 3d20 2256 6572 7920 6869 6768 206c 6576  = "Very high lev
 00000050: 656c 2047 5549 2077 6974 6820 616e 2041  el GUI with an A
 00000060: 5049 2073 696d 696c 6172 2074 6f20 7468  PI similar to th
 00000070: 6520 4869 6768 4755 4920 6f66 204f 7065  e HighGUI of Ope
 00000080: 6e43 5622 0d0a 6175 7468 6f72 7320 3d20  nCV"..authors = 
 00000090: 5b22 4d61 6e75 2047 6972 6120 3c6d 616e  ["Manu Gira <man
 000000a0: 752e 6769 7261 406f 7574 6c6f 6f6b 2e63  u.gira@outlook.c
 000000b0: 6f6d 3e22 5d0d 0a72 6561 646d 6520 3d20  om>"]..readme = 
-000000c0: 2252 4541 444d 455f 7573 6572 2e6d 6422  "README_user.md"
-000000d0: 0d0a 7265 706f 7369 746f 7279 203d 2022  ..repository = "
-000000e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000000f0: 6f6d 2f4d 616e 7547 6972 612f 4775 6962  om/ManuGira/Guib
-00000100: 626f 6e2e 6769 7422 0d0a 6b65 7977 6f72  bon.git"..keywor
-00000110: 6473 203d 205b 2247 5549 222c 2022 546b  ds = ["GUI", "Tk
-00000120: 696e 7465 7222 2c20 224f 7065 6e43 5622  inter", "OpenCV"
-00000130: 5d0d 0a0d 0a5b 746f 6f6c 2e70 6f65 7472  ]....[tool.poetr
-00000140: 792e 7572 6c73 5d0d 0a22 4275 6720 5265  y.urls].."Bug Re
-00000150: 706f 7274 2220 3d20 2268 7474 7073 3a2f  port" = "https:/
-00000160: 2f67 6974 6875 622e 636f 6d2f 4d61 6e75  /github.com/Manu
-00000170: 4769 7261 2f47 7569 6262 6f6e 2f69 7373  Gira/Guibbon/iss
-00000180: 7565 7322 0d0a 0d0a 5b62 7569 6c64 2d73  ues"....[build-s
-00000190: 7973 7465 6d5d 0d0a 7265 7175 6972 6573  ystem]..requires
-000001a0: 203d 205b 2270 6f65 7472 792d 636f 7265   = ["poetry-core
-000001b0: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
-000001c0: 6420 3d20 2270 6f65 7472 792e 636f 7265  d = "poetry.core
-000001d0: 2e6d 6173 6f6e 7279 2e61 7069 220d 0a0d  .masonry.api"...
-000001e0: 0a5b 746f 6f6c 2e70 6f65 7472 792e 6465  .[tool.poetry.de
-000001f0: 7065 6e64 656e 6369 6573 5d0d 0a70 7974  pendencies]..pyt
-00000200: 686f 6e20 3d20 225e 332e 3722 0d0a 6f70  hon = "^3.7"..op
-00000210: 656e 6376 2d70 7974 686f 6e20 3d20 225e  encv-python = "^
-00000220: 342e 352e 342e 3630 220d 0a50 696c 6c6f  4.5.4.60"..Pillo
-00000230: 7720 3d20 225e 392e 312e 3022 0d0a 0d0a  w = "^9.1.0"....
-00000240: 5b74 6f6f 6c2e 706f 6574 7279 2e67 726f  [tool.poetry.gro
-00000250: 7570 2e64 6576 2e64 6570 656e 6465 6e63  up.dev.dependenc
-00000260: 6965 735d 0d0a 7079 7465 7374 203d 2022  ies]..pytest = "
-00000270: 5e37 2e32 2e32 220d 0a70 7974 6573 742d  ^7.2.2"..pytest-
-00000280: 636f 7620 3d20 225e 342e 302e 3022 0d0a  cov = "^4.0.0"..
-00000290: 7275 6666 203d 2022 5e30 2e31 2e35 220d  ruff = "^0.1.5".
-000002a0: 0a6d 7970 7920 3d20 225e 312e 342e 3122  .mypy = "^1.4.1"
-000002b0: 0d0a 0d0a 5b74 6f6f 6c2e 7079 7465 7374  ....[tool.pytest
-000002c0: 2e69 6e69 5f6f 7074 696f 6e73 5d0d 0a61  .ini_options]..a
-000002d0: 6464 6f70 7473 203d 2022 2d2d 636f 762d  ddopts = "--cov-
-000002e0: 7265 706f 7274 3d74 6572 6d20 2d2d 636f  report=term --co
-000002f0: 762d 7265 706f 7274 3d68 746d 6c3a 6275  v-report=html:bu
-00000300: 696c 642f 7079 7465 7374 5f63 6f76 6572  ild/pytest_cover
-00000310: 6167 655f 6874 6d6c 202d 2d63 6f76 3d67  age_html --cov=g
-00000320: 7569 6262 6f6e 220d 0a74 6573 7470 6174  uibbon"..testpat
-00000330: 6873 203d 205b 2274 6573 7473 225d 0d0a  hs = ["tests"]..
-00000340: 6361 6368 655f 6469 7220 3d20 2262 7569  cache_dir = "bui
-00000350: 6c64 2f2e 7079 7465 7374 5f63 6163 6865  ld/.pytest_cache
-00000360: 220d 0a0d 0a5b 746f 6f6c 2e63 6f76 6572  "....[tool.cover
-00000370: 6167 652e 7275 6e5d 0d0a 6461 7461 5f66  age.run]..data_f
-00000380: 696c 653d 2262 7569 6c64 2f2e 636f 7665  ile="build/.cove
-00000390: 7261 6765 220d 0a0d 0a5b 746f 6f6c 2e63  rage"....[tool.c
-000003a0: 6f76 6572 6167 652e 7265 706f 7274 5d0d  overage.report].
-000003b0: 0a23 2052 6567 6578 6573 2066 6f72 206c  .# Regexes for l
-000003c0: 696e 6573 2074 6f20 6578 636c 7564 6520  ines to exclude 
-000003d0: 6672 6f6d 2063 6f6e 7369 6465 7261 7469  from considerati
-000003e0: 6f6e 0d0a 6578 636c 7564 655f 616c 736f  on..exclude_also
-000003f0: 203d 205b 0d0a 2020 2020 2320 446f 6e27   = [..    # Don'
-00000400: 7420 636f 6d70 6c61 696e 2061 626f 7574  t complain about
-00000410: 206d 6973 7369 6e67 2064 6562 7567 2d6f   missing debug-o
-00000420: 6e6c 7920 636f 6465 3a0d 0a20 2020 2022  nly code:..    "
-00000430: 6465 6620 5f5f 7265 7072 5f5f 222c 0d0a  def __repr__",..
-00000440: 2020 2020 2269 6620 7365 6c66 5c5c 2e64      "if self\\.d
-00000450: 6562 7567 222c 0d0a 0d0a 2020 2020 2320  ebug",....    # 
-00000460: 446f 6e27 7420 636f 6d70 6c61 696e 2069  Don't complain i
-00000470: 6620 7465 7374 7320 646f 6e27 7420 6869  f tests don't hi
-00000480: 7420 6465 6665 6e73 6976 6520 6173 7365  t defensive asse
-00000490: 7274 696f 6e20 636f 6465 3a0d 0a20 2020  rtion code:..   
-000004a0: 2022 7261 6973 6520 4173 7365 7274 696f   "raise Assertio
-000004b0: 6e45 7272 6f72 222c 0d0a 2020 2020 2272  nError",..    "r
-000004c0: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
-000004d0: 7465 6445 7272 6f72 222c 0d0a 0d0a 2020  tedError",....  
-000004e0: 2020 2320 446f 6e27 7420 636f 6d70 6c61    # Don't compla
-000004f0: 696e 2069 6620 6e6f 6e2d 7275 6e6e 6162  in if non-runnab
-00000500: 6c65 2063 6f64 6520 6973 6e27 7420 7275  le code isn't ru
-00000510: 6e3a 0d0a 2020 2020 2269 6620 303a 222c  n:..    "if 0:",
-00000520: 0d0a 2020 2020 2269 6620 5f5f 6e61 6d65  ..    "if __name
-00000530: 5f5f 203d 3d20 2e5f 5f6d 6169 6e5f 5f2e  __ == .__main__.
-00000540: 3a22 2c0d 0a0d 0a20 2020 2023 2044 6f6e  :",....    # Don
-00000550: 2774 2063 6f6d 706c 6169 6e20 6162 6f75  't complain abou
-00000560: 7420 6162 7374 7261 6374 206d 6574 686f  t abstract metho
-00000570: 6473 2c20 7468 6579 2061 7265 6e27 7420  ds, they aren't 
-00000580: 7275 6e3a 0d0a 2020 2020 2240 2861 6263  run:..    "@(abc
-00000590: 5c5c 2e29 3f61 6273 7472 6163 746d 6574  \\.)?abstractmet
-000005a0: 686f 6422 2c0d 0a20 2020 205d 0d0a 0d0a  hod",..    ]....
-000005b0: 5b74 6f6f 6c2e 7275 6666 5d0d 0a6c 696e  [tool.ruff]..lin
-000005c0: 652d 6c65 6e67 7468 203d 2031 3630 0d0a  e-length = 160..
-000005d0: 6361 6368 652d 6469 7220 3d20 2262 7569  cache-dir = "bui
-000005e0: 6c64 2f2e 7275 6666 5f63 6163 6865 220d  ld/.ruff_cache".
-000005f0: 0a0d 0a5b 746f 6f6c 2e6d 7970 795d 0d0a  ...[tool.mypy]..
-00000600: 6368 6563 6b5f 756e 7479 7065 645f 6465  check_untyped_de
-00000610: 6673 203d 2074 7275 650d 0a64 6973 616c  fs = true..disal
-00000620: 6c6f 775f 616e 795f 6765 6e65 7269 6373  low_any_generics
-00000630: 203d 2074 7275 650d 0a69 676e 6f72 655f   = true..ignore_
-00000640: 6d69 7373 696e 675f 696d 706f 7274 7320  missing_imports 
-00000650: 3d20 7472 7565 0d0a 6e6f 5f69 6d70 6c69  = true..no_impli
-00000660: 6369 745f 6f70 7469 6f6e 616c 203d 2074  cit_optional = t
-00000670: 7275 650d 0a73 686f 775f 6572 726f 725f  rue..show_error_
-00000680: 636f 6465 7320 3d20 7472 7565 0d0a 7374  codes = true..st
-00000690: 7269 6374 5f65 7175 616c 6974 7920 3d20  rict_equality = 
-000006a0: 7472 7565 0d0a 7761 726e 5f72 6564 756e  true..warn_redun
-000006b0: 6461 6e74 5f63 6173 7473 203d 2074 7275  dant_casts = tru
-000006c0: 650d 0a77 6172 6e5f 7265 7475 726e 5f61  e..warn_return_a
-000006d0: 6e79 203d 2074 7275 650d 0a77 6172 6e5f  ny = true..warn_
-000006e0: 756e 7265 6163 6861 626c 6520 3d20 7472  unreachable = tr
-000006f0: 7565 0d0a 7761 726e 5f75 6e75 7365 645f  ue..warn_unused_
-00000700: 636f 6e66 6967 7320 3d20 7472 7565 0d0a  configs = true..
-00000710: 696d 706c 6963 6974 5f72 6565 7870 6f72  implicit_reexpor
-00000720: 7420 3d20 7472 7565 0d0a 7072 6574 7479  t = true..pretty
-00000730: 203d 2074 7275 650d 0a63 6163 6865 5f64   = true..cache_d
-00000740: 6972 203d 2022 6275 696c 642f 2e6d 7970  ir = "build/.myp
-00000750: 795f 6361 6368 6522                      y_cache"
+000000c0: 2264 6f63 732f 696e 6465 782e 6d64 220d  "docs/index.md".
+000000d0: 0a72 6570 6f73 6974 6f72 7920 3d20 2268  .repository = "h
+000000e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000000f0: 6d2f 4d61 6e75 4769 7261 2f47 7569 6262  m/ManuGira/Guibb
+00000100: 6f6e 2e67 6974 220d 0a6b 6579 776f 7264  on.git"..keyword
+00000110: 7320 3d20 5b22 4755 4922 2c20 2254 6b69  s = ["GUI", "Tki
+00000120: 6e74 6572 222c 2022 4f70 656e 4356 225d  nter", "OpenCV"]
+00000130: 0d0a 0d0a 5b74 6f6f 6c2e 706f 6574 7279  ....[tool.poetry
+00000140: 2e75 726c 735d 0d0a 2242 7567 2052 6570  .urls].."Bug Rep
+00000150: 6f72 7422 203d 2022 6874 7470 733a 2f2f  ort" = "https://
+00000160: 6769 7468 7562 2e63 6f6d 2f4d 616e 7547  github.com/ManuG
+00000170: 6972 612f 4775 6962 626f 6e2f 6973 7375  ira/Guibbon/issu
+00000180: 6573 220d 0a0d 0a5b 6275 696c 642d 7379  es"....[build-sy
+00000190: 7374 656d 5d0d 0a72 6571 7569 7265 7320  stem]..requires 
+000001a0: 3d20 5b22 706f 6574 7279 2d63 6f72 6522  = ["poetry-core"
+000001b0: 5d0d 0a62 7569 6c64 2d62 6163 6b65 6e64  ]..build-backend
+000001c0: 203d 2022 706f 6574 7279 2e63 6f72 652e   = "poetry.core.
+000001d0: 6d61 736f 6e72 792e 6170 6922 0d0a 0d0a  masonry.api"....
+000001e0: 5b74 6f6f 6c2e 706f 6574 7279 2e64 6570  [tool.poetry.dep
+000001f0: 656e 6465 6e63 6965 735d 0d0a 7079 7468  endencies]..pyth
+00000200: 6f6e 203d 2022 5e33 2e38 220d 0a6f 7065  on = "^3.8"..ope
+00000210: 6e63 762d 7079 7468 6f6e 203d 2022 5e34  ncv-python = "^4
+00000220: 2e35 2e34 2e36 3022 0d0a 5069 6c6c 6f77  .5.4.60"..Pillow
+00000230: 203d 2022 5e39 2e31 2e30 220d 0a0d 0a5b   = "^9.1.0"....[
+00000240: 746f 6f6c 2e70 6f65 7472 792e 6772 6f75  tool.poetry.grou
+00000250: 702e 6465 762e 6465 7065 6e64 656e 6369  p.dev.dependenci
+00000260: 6573 5d0d 0a70 7974 6573 7420 3d20 225e  es]..pytest = "^
+00000270: 372e 322e 3222 0d0a 7079 7465 7374 2d63  7.2.2"..pytest-c
+00000280: 6f76 203d 2022 5e34 2e30 2e30 220d 0a72  ov = "^4.0.0"..r
+00000290: 7566 6620 3d20 225e 302e 312e 3522 0d0a  uff = "^0.1.5"..
+000002a0: 6d79 7079 203d 2022 5e31 2e34 2e31 220d  mypy = "^1.4.1".
+000002b0: 0a6d 6b64 6f63 7320 3d20 225e 312e 352e  .mkdocs = "^1.5.
+000002c0: 3322 0d0a 6d6b 646f 6373 7472 696e 6773  3"..mkdocstrings
+000002d0: 203d 207b 6578 7472 6173 203d 205b 2270   = {extras = ["p
+000002e0: 7974 686f 6e22 5d2c 2076 6572 7369 6f6e  ython"], version
+000002f0: 203d 2022 5e30 2e32 342e 3322 7d0d 0a0d   = "^0.24.3"}...
+00000300: 0a0d 0a5b 746f 6f6c 2e70 7974 6573 742e  ...[tool.pytest.
+00000310: 696e 695f 6f70 7469 6f6e 735d 0d0a 6164  ini_options]..ad
+00000320: 646f 7074 7320 3d20 222d 2d63 6f76 2d72  dopts = "--cov-r
+00000330: 6570 6f72 743d 7465 726d 202d 2d63 6f76  eport=term --cov
+00000340: 2d72 6570 6f72 743d 6874 6d6c 3a62 7569  -report=html:bui
+00000350: 6c64 2f70 7974 6573 745f 636f 7665 7261  ld/pytest_covera
+00000360: 6765 5f68 746d 6c20 2d2d 636f 763d 6775  ge_html --cov=gu
+00000370: 6962 626f 6e22 0d0a 7465 7374 7061 7468  ibbon"..testpath
+00000380: 7320 3d20 5b22 7465 7374 7322 5d0d 0a63  s = ["tests"]..c
+00000390: 6163 6865 5f64 6972 203d 2022 6275 696c  ache_dir = "buil
+000003a0: 642f 2e70 7974 6573 745f 6361 6368 6522  d/.pytest_cache"
+000003b0: 0d0a 0d0a 5b74 6f6f 6c2e 636f 7665 7261  ....[tool.covera
+000003c0: 6765 2e72 756e 5d0d 0a64 6174 615f 6669  ge.run]..data_fi
+000003d0: 6c65 3d22 6275 696c 642f 2e63 6f76 6572  le="build/.cover
+000003e0: 6167 6522 0d0a 0d0a 5b74 6f6f 6c2e 636f  age"....[tool.co
+000003f0: 7665 7261 6765 2e72 6570 6f72 745d 0d0a  verage.report]..
+00000400: 2320 5265 6765 7865 7320 666f 7220 6c69  # Regexes for li
+00000410: 6e65 7320 746f 2065 7863 6c75 6465 2066  nes to exclude f
+00000420: 726f 6d20 636f 6e73 6964 6572 6174 696f  rom consideratio
+00000430: 6e0d 0a65 7863 6c75 6465 5f61 6c73 6f20  n..exclude_also 
+00000440: 3d20 5b0d 0a20 2020 2023 2044 6f6e 2774  = [..    # Don't
+00000450: 2063 6f6d 706c 6169 6e20 6162 6f75 7420   complain about 
+00000460: 6d69 7373 696e 6720 6465 6275 672d 6f6e  missing debug-on
+00000470: 6c79 2063 6f64 653a 0d0a 2020 2020 2264  ly code:..    "d
+00000480: 6566 205f 5f72 6570 725f 5f22 2c0d 0a20  ef __repr__",.. 
+00000490: 2020 2022 6966 2073 656c 665c 5c2e 6465     "if self\\.de
+000004a0: 6275 6722 2c0d 0a0d 0a20 2020 2023 2044  bug",....    # D
+000004b0: 6f6e 2774 2063 6f6d 706c 6169 6e20 6966  on't complain if
+000004c0: 2074 6573 7473 2064 6f6e 2774 2068 6974   tests don't hit
+000004d0: 2064 6566 656e 7369 7665 2061 7373 6572   defensive asser
+000004e0: 7469 6f6e 2063 6f64 653a 0d0a 2020 2020  tion code:..    
+000004f0: 2272 6169 7365 2041 7373 6572 7469 6f6e  "raise Assertion
+00000500: 4572 726f 7222 2c0d 0a20 2020 2022 7261  Error",..    "ra
+00000510: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
+00000520: 6564 4572 726f 7222 2c0d 0a0d 0a20 2020  edError",....   
+00000530: 2023 2044 6f6e 2774 2063 6f6d 706c 6169   # Don't complai
+00000540: 6e20 6966 206e 6f6e 2d72 756e 6e61 626c  n if non-runnabl
+00000550: 6520 636f 6465 2069 736e 2774 2072 756e  e code isn't run
+00000560: 3a0d 0a20 2020 2022 6966 2030 3a22 2c0d  :..    "if 0:",.
+00000570: 0a20 2020 2022 6966 205f 5f6e 616d 655f  .    "if __name_
+00000580: 5f20 3d3d 202e 5f5f 6d61 696e 5f5f 2e3a  _ == .__main__.:
+00000590: 222c 0d0a 0d0a 2020 2020 2320 446f 6e27  ",....    # Don'
+000005a0: 7420 636f 6d70 6c61 696e 2061 626f 7574  t complain about
+000005b0: 2061 6273 7472 6163 7420 6d65 7468 6f64   abstract method
+000005c0: 732c 2074 6865 7920 6172 656e 2774 2072  s, they aren't r
+000005d0: 756e 3a0d 0a20 2020 2022 4028 6162 635c  un:..    "@(abc\
+000005e0: 5c2e 293f 6162 7374 7261 6374 6d65 7468  \.)?abstractmeth
+000005f0: 6f64 222c 0d0a 2020 2020 5d0d 0a0d 0a5b  od",..    ]....[
+00000600: 746f 6f6c 2e72 7566 665d 0d0a 6c69 6e65  tool.ruff]..line
+00000610: 2d6c 656e 6774 6820 3d20 3136 300d 0a63  -length = 160..c
+00000620: 6163 6865 2d64 6972 203d 2022 6275 696c  ache-dir = "buil
+00000630: 642f 2e72 7566 665f 6361 6368 6522 0d0a  d/.ruff_cache"..
+00000640: 0d0a 5b74 6f6f 6c2e 6d79 7079 5d0d 0a63  ..[tool.mypy]..c
+00000650: 6865 636b 5f75 6e74 7970 6564 5f64 6566  heck_untyped_def
+00000660: 7320 3d20 7472 7565 0d0a 6469 7361 6c6c  s = true..disall
+00000670: 6f77 5f61 6e79 5f67 656e 6572 6963 7320  ow_any_generics 
+00000680: 3d20 7472 7565 0d0a 6967 6e6f 7265 5f6d  = true..ignore_m
+00000690: 6973 7369 6e67 5f69 6d70 6f72 7473 203d  issing_imports =
+000006a0: 2074 7275 650d 0a6e 6f5f 696d 706c 6963   true..no_implic
+000006b0: 6974 5f6f 7074 696f 6e61 6c20 3d20 7472  it_optional = tr
+000006c0: 7565 0d0a 7368 6f77 5f65 7272 6f72 5f63  ue..show_error_c
+000006d0: 6f64 6573 203d 2074 7275 650d 0a73 7472  odes = true..str
+000006e0: 6963 745f 6571 7561 6c69 7479 203d 2074  ict_equality = t
+000006f0: 7275 650d 0a77 6172 6e5f 7265 6475 6e64  rue..warn_redund
+00000700: 616e 745f 6361 7374 7320 3d20 7472 7565  ant_casts = true
+00000710: 0d0a 7761 726e 5f72 6574 7572 6e5f 616e  ..warn_return_an
+00000720: 7920 3d20 7472 7565 0d0a 7761 726e 5f75  y = true..warn_u
+00000730: 6e72 6561 6368 6162 6c65 203d 2074 7275  nreachable = tru
+00000740: 650d 0a77 6172 6e5f 756e 7573 6564 5f63  e..warn_unused_c
+00000750: 6f6e 6669 6773 203d 2074 7275 650d 0a69  onfigs = true..i
+00000760: 6d70 6c69 6369 745f 7265 6578 706f 7274  mplicit_reexport
+00000770: 203d 2074 7275 650d 0a70 7265 7474 7920   = true..pretty 
+00000780: 3d20 7472 7565 0d0a 6361 6368 655f 6469  = true..cache_di
+00000790: 7220 3d20 2262 7569 6c64 2f2e 6d79 7079  r = "build/.mypy
+000007a0: 5f63 6163 6865 220d 0a65 7863 6c75 6465  _cache"..exclude
+000007b0: 203d 2022 6275 696c 642f 220d 0a          = "build/"..
```

### Comparing `guibbon-0.1.5/PKG-INFO` & `guibbon-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 Metadata-Version: 2.1
 Name: guibbon
-Version: 0.1.5
+Version: 0.2.0
 Summary: Very high level GUI with an API similar to the HighGUI of OpenCV
 Home-page: https://github.com/ManuGira/Guibbon.git
 Keywords: GUI,Tkinter,OpenCV
 Author: Manu Gira
 Author-email: manu.gira@outlook.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Pillow (>=9.1.0,<10.0.0)
 Requires-Dist: opencv-python (>=4.5.4.60,<5.0.0.0)
 Project-URL: Bug Report, https://github.com/ManuGira/Guibbon/issues
 Project-URL: Repository, https://github.com/ManuGira/Guibbon.git
 Description-Content-Type: text/markdown
 
-# Guibbon with U
+# ![icon](images/icon32.png) Guibbon with U ![icon](images/icon32.png) 
 ![Tests](https://github.com/ManuGira/Guibbon/actions/workflows/tests.yml/badge.svg)
 
-High-level GUI with an API similar to the HighGUI of OpenCV. It allows to display an image and add GUI controllers such as
+### High-level GUI with an API similar to the HighGUI of OpenCV. 
+**If you know how to use the GUI of OpenCV, then you already know how to use Guibbon.**
+
+It allows to display an image and add GUI controllers such as:
+
  - Sliders (trackbar)
  - Buttons
  - Radio buttons
  - Check boxes
  - Color picker
  - Draggable points and polygons on the displayed image
  - Any custom widget that you write in Tkinter
 
-If you know how to use the GUI of OpenCV, then you already know how to use Guibbon. 
+### Reasons why you want to use Guibbon:
 
-Reasons why you want to use Guibbon:
- - It's using Tkinter which is natively installed in your python distribution
+ - It's fast to learn and fast to code.
+ - It's using Tkinter which is natively installed in most python distributions
  - Beside Tkinter, it only has 3 dependencies: numpy, opencv-python and pillow
- - You just need to display an image and add a few controllers to play with parameters
+ - It's less than 200 KB
+ - You can create your own custom widget.
+ 
+### Links
+
+* Source code hosted on [GitHub](https://github.com/ManuGira/Guibbon)
+* Package hosted on [PyPl](https://pypi.org/project/guibbon)
+* Documentation hosted on [Github Pages](https://manugira.github.io/Guibbon/)
```

