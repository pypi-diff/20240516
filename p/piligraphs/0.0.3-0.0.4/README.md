# Comparing `tmp/piligraphs-0.0.3.tar.gz` & `tmp/piligraphs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piligraphs-0.0.3.tar", max compression
+gzip compressed data, was "piligraphs-0.0.4.tar", max compression
```

## Comparing `piligraphs-0.0.3.tar` & `piligraphs-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11558 2023-12-07 15:54:15.675037 piligraphs-0.0.3/LICENSE
--rw-r--r--   0        0        0       97 2023-12-07 14:43:02.655732 piligraphs-0.0.3/piligraphs/__init__.py
--rw-r--r--   0        0        0     1302 2023-12-07 14:20:59.058385 piligraphs-0.0.3/piligraphs/basegraph.py
--rw-r--r--   0        0        0      769 2023-12-30 20:50:51.309868 piligraphs-0.0.3/piligraphs/item.py
--rw-r--r--   0        0        0     6211 2023-12-30 20:53:33.115931 piligraphs-0.0.3/piligraphs/linechart.py
--rw-r--r--   0        0        0     5006 2023-12-07 15:30:20.286276 piligraphs-0.0.3/piligraphs/piechart.py
--rw-r--r--   0        0        0     6494 2023-12-30 20:51:59.771037 piligraphs-0.0.3/piligraphs/radarchart.py
--rw-r--r--   0        0        0     1159 2023-12-05 12:56:32.289188 piligraphs-0.0.3/piligraphs/size.py
--rw-r--r--   0        0        0     3506 2023-12-30 20:53:56.430561 piligraphs-0.0.3/piligraphs/utils.py
--rw-r--r--   0        0        0      414 2023-12-30 20:55:12.397308 piligraphs-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      635 2023-12-30 20:55:44.860721 piligraphs-0.0.3/README.md
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 piligraphs-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-12-07 15:54:15.675037 piligraphs-0.0.4/LICENSE
+-rw-r--r--   0        0        0      145 2024-05-14 13:21:11.131930 piligraphs-0.0.4/piligraphs/__init__.py
+-rw-r--r--   0        0        0     6142 2024-05-15 09:43:37.430276 piligraphs-0.0.4/piligraphs/funcgraph.py
+-rw-r--r--   0        0        0     1482 2024-05-14 13:20:33.858580 piligraphs-0.0.4/piligraphs/graph.py
+-rw-r--r--   0        0        0     7231 2024-05-15 09:43:42.245524 piligraphs-0.0.4/piligraphs/linechart.py
+-rw-r--r--   0        0        0     1119 2024-05-15 09:43:19.322384 piligraphs-0.0.4/piligraphs/node.py
+-rw-r--r--   0        0        0     5703 2024-05-15 09:23:19.805282 piligraphs-0.0.4/piligraphs/piechart.py
+-rw-r--r--   0        0        0     7555 2024-05-15 09:43:50.054767 piligraphs-0.0.4/piligraphs/radarchart.py
+-rw-r--r--   0        0        0     3113 2024-05-16 08:53:49.165677 piligraphs-0.0.4/piligraphs/utils.py
+-rw-r--r--   0        0        0      412 2024-05-12 15:23:19.816380 piligraphs-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1322 2024-05-16 08:52:26.375254 piligraphs-0.0.4/README.md
+-rw-r--r--   0        0        0     1786 1970-01-01 00:00:00.000000 piligraphs-0.0.4/PKG-INFO
```

### Comparing `piligraphs-0.0.3/LICENSE` & `piligraphs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `piligraphs-0.0.3/piligraphs/item.py` & `piligraphs-0.0.4/piligraphs/node.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 from pinkie import Color
 
-from .utils import get_color
 
+class Node:
+    """Class representing a graph node."""
 
-class GraphItem:
-    """Class representing a graph item."""
-    def __init__(self,
-                 *,
-                 color: Color | int | str | tuple[int, int, int] | tuple[int, int, int, int] | None = ...,
-                 weight: int | float = 1) -> None:
-        self.color = get_color(color)
+    def __init__(
+        self,
+        *,
+        weight: int | float = 1,
+        color: Color | int | str | tuple[int, int, int] | tuple[int, int, int, int] | None = ...
+    ) -> None:
         self.weight = weight
+        self.color = color
 
     @property
+    def weight(self) -> int:
+        """Line thickness."""
+        return self._thickness
+    
+    @weight.setter
+    def weight(self, value: int | float):
+        if isinstance(value, (int, float)):
+            self._weight = value
+        else:
+            raise TypeError(f"weight must be an int or float, not {type(value).__name__}")
+    
+    @property
     def color(self) -> Color | None:
+        """Node color."""
         return self._color
     
     @color.setter
-    def color(self, value: Color):
-        self._color = get_color(value)
-
-    @property
-    def weight(self) -> int | float:
-        return self._weight
-    
-    @weight.setter
-    def weight(self, value: int | float):
-        self._weight = value
-    
+    def color(self, value: Color | int | str | tuple | None):
+        if isinstance(value, Color) or value is None:
+            self._color = value
+        elif value is ...:
+            self._color = Color.random()
+        else:
+            self._color = Color(value)
```

### Comparing `piligraphs-0.0.3/piligraphs/linechart.py` & `piligraphs-0.0.4/piligraphs/radarchart.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,195 +1,246 @@
 from pinkie import Color
 from PIL import Image, ImageDraw
 
-from .basegraph import BaseGraph
-from .size import Size
-from .utils import get_color, limit, interpolate, Interpolation
-
-
-class LineChart(BaseGraph):
-    """Class representing a Line chart."""
-    def __init__(self,
-                 *,
-                 size: Size | tuple[int, int],
-                 thickness: int = 1,
-                 fill: Color | int | str | tuple[int, int, int] | tuple[int, int, int, int] | None = ...,
-                 outline: Color | int | str | tuple[int, int, int] | tuple[int, int, int, int] | None = ...,
-                 point_width: int = 0,
-                 all_points: bool = False,
-                 num_points: int = 0,
-                 interpol: Interpolation = 'linear',
-                 min_height: int = 0) -> None:
-        """
-        LineChart constructor.
+from .graph import NodeGraph
+from .utils import interpolate, linear_to_circle, Interpolation
+
 
+class RadarChart(NodeGraph):
+    """Class representing a radar chart."""
+
+    def __init__(
+        self,
+        radius: int,
+        *,
+        thickness: int = 1,
+        fill: Color | int | str | tuple[int, int, int] | tuple[int, int, int, int] | None = ...,
+        outline: Color | int | str | tuple[int, int, int] | tuple[int, int, int, int] | None = ...,
+        pwidth: int = 0,
+        onlysrc: bool = True,
+        npoints: int | None = None,
+        interp: Interpolation = 'linear',
+        angle: int | float = 0,
+        minr: int = 0
+    ) -> None:
+        """
         Attributes
         ----------
-        size: `Size` | `tuple[int, int]`
-            Graph image size.
+        radius: `int`
+            Radius of the chart shape.
         thickness: `int`
             Line thickness.
         fill: `Color`
-            Fill color.
+            Fill color. If = `...`, generates a random color.
         outline: `Color`
-            Line color.
-        point_width: `int`
+            Line color. If = `...`, generates a random color.
+        pwidth: `int`
             Point width.
-        all_points: `bool`
-            If `True`, all points (including intermediate ones) will be drawn.
-            Otherwise, only source points will be displayed.
-        num_points: `int`
-            Number of points. If <= 0, equals to the number of items.
-        interpol: `Interpolation`
+        onlysrc: `bool`
+            To draw bold dots only in source points (without interpolated ones).
+        npoints: `int` | `None`
+            Number of points. If `None`, equals to the number of nodes.
+        interp: `str`
             Kind of interpolation. Used to make a smooth curve.
-        min_height: `int`
-            Minimum height from bottom of the graph.
+        angle: `int` | `float`
+            Start angle of the chart.
+        minr: `int`
+            Minimum distance between the center and a point.
         """
         super().__init__()
 
-        self.size = size
+        self.radius = radius
         self.thickness = thickness
-        self.fill = get_color(fill)
-        self.outline = get_color(outline)
-        self.point_width = point_width
-        self.all_points = all_points
-        self.num_points = num_points
-        self.interpol = interpol
-        self.min_height = min_height
-
-    @property
-    def size(self) -> Size:
-        """Graph size."""
-        return self._size
-    
-    @size.setter
-    def size(self, value: Size | tuple[int, int]):
-        if not isinstance(value, Size): 
-            value = Size(value)
-
-        self._size = value
-
+        self.fill = fill
+        self.outline = outline
+        self.pwidth = pwidth
+        self.onlysrc = onlysrc
+        self.npoints = npoints
+        self.interp = interp
+        self.angle = angle
+        self.minr = minr
+
+    @property
+    def radius(self) -> int:
+        """Chart radius."""
+        return self._radius
+    
+    @radius.setter
+    def radius(self, value: int):
+        if isinstance(value, int):
+            self._radius = value
+        else:
+            raise TypeError(f"radius must be an int, not {type(value).__name__}")
+        
     @property
     def thickness(self) -> int:
-        """Stroke thickness."""
+        """Line thickness."""
         return self._thickness
     
     @thickness.setter
     def thickness(self, value: int):
-        self._thickness = value
+        if isinstance(value, int):
+            self._thickness = value
+        else:
+            raise TypeError(f"thickness must be an int, not {type(value).__name__}")
 
     @property
-    def fill(self) -> Color:
-        """Fill color."""
+    def fill(self) -> Color | None:
+        """Shape color. If `None`, no shape will be drawn."""
         return self._fill
     
     @fill.setter
-    def fill(self, value: Color):
-        self._fill = value
+    def fill(self, value: Color | int | str | tuple | None):
+        if isinstance(value, Color) or value is None:
+            self._fill = value
+        elif value is ...:
+            self._fill = Color.random()
+        else:
+            self._fill = Color(value)
 
     @property
-    def outline(self) -> Color:
-        """Outline color."""
+    def outline(self) -> Color | None:
+        """Line color. If `None`, no line will be drawn."""
         return self._outline
     
     @outline.setter
-    def outline(self, value: Color):
-        self._outline = value
+    def outline(self, value: Color | int | str | tuple | None):
+        if isinstance(value, Color) or value is None:
+            self._outline = value
+        elif value is ...:
+            self._outline = Color.random()
+        else:
+            self._outline = Color(value)
 
     @property
-    def point_width(self) -> int:
-        """Stroke points width."""
-        return self._point_width
+    def pwidth(self) -> int:
+        """Point width."""
+        return self._pwidth
+    
+    @pwidth.setter
+    def pwidth(self, value: int):
+        if isinstance(value, int):
+            self._pwidth = value
+        else:
+            raise TypeError(f"pwidth must be an int, not {type(value).__name__}")
     
-    @point_width.setter
-    def point_width(self, value: int):
-        self._point_width = value
-
     @property
-    def all_points(self) -> bool:
-        """Draw all points or not."""
-        return self._all_points
+    def onlysrc(self) -> bool:
+        """To draw only source points without interpolated ones."""
+        return self._onlysrc
     
-    @all_points.setter
-    def all_points(self, value: bool):
-        self._all_points = value
+    @onlysrc.setter
+    def onlysrc(self, value: bool):
+        if isinstance(value, bool):
+            self._onlysrc = value
+        else:
+            raise TypeError(f"onlysrc must be a bool, not {type(value).__name__}")
 
     @property
-    def num_points(self) -> int:
+    def npoints(self) -> int | None:
         """Number of points."""
-        return self._num_points
+        return self._npoints
     
-    @num_points.setter
-    def num_points(self, value: int):
-        self._num_points = value
-
+    @npoints.setter
+    def npoints(self, value: int | None):
+        if isinstance(value, int) or value is None:
+            self._npoints = value
+        else:
+            raise TypeError(f"npoints must be an int or None, not {type(value).__name__}")
+        
     @property
-    def interpol(self) -> Interpolation:
-        """Kinf of interpolation."""
-        return self._interpol
+    def interp(self) -> Interpolation:
+        """Kind of interpolation."""
+        return self._interp
+    
+    @interp.setter
+    def interp(self, value: Interpolation):
+        if isinstance(value, Interpolation):
+            self._interp = value
+        else:
+            raise TypeError("interp must be a valid string")
     
-    @interpol.setter
-    def interpol(self, value: Interpolation):
-        self._interpol = value
-
     @property
-    def min_height(self) -> int:
-        """Min height (max y value in the image coordinates)."""
-        return self._min_height
+    def angle(self) -> int | float:
+        """Start angle."""
+        return self._angle
     
-    @min_height.setter
-    def min_height(self, value: int):
-        if (hasattr(self, '_radius')
-            and self.size.height < value):
-            raise ValueError("'min_height' can not be bigger than 'size.height'")
-        self._min_height = value
+    @angle.setter
+    def angle(self, value: int | float):
+        if isinstance(value, (int, float)):
+            self._angle = value
+        else:
+            raise TypeError(f"angle must be an int or float, not {type(value).__name__}")
+        
+    @property
+    def minr(self) -> int:
+        """Minimal distance from center to point."""
+        return self._minr
+    
+    @minr.setter
+    def minr(self, value: int):
+        if isinstance(value, int):
+            self._minr = value
+        else:
+            raise TypeError(f"minr must be an int, not {type(value).__name__}")
 
     def draw(self) -> Image.Image:
-        image = Image.new('RGBA', tuple(self.size))
-        num_items = len(self.items)
+        w = self.radius * 2
+        image = Image.new('RGBA', (w, w))
 
-        if num_items == 0:
+        if len(self.nodes) == 0:
             return image
+
+        nodes = self.nodes.copy()
+        nodes.append(nodes[0])
+        num_nodes = len(nodes)
         
         draw = ImageDraw.Draw(image)
-        thickness = self.thickness or 1
-        num = self.num_points if self.num_points > 0 else num_items
-        max_weight = max((i.weight for i in self.items))
-        p_radius = self.point_width / 2 if self.point_width > 0 else thickness / 2
-        if max_weight == 0:
-            limited_y = [self.size.height - p_radius] * num_items
-        else:
-            limited_y = limit(
-                [max_weight - item.weight for item in self.items], 
-                p_radius, 
-                self.size.height - p_radius - self.min_height)
-
-        space_between_points = self.size.width / (num_items - 1)
-        limited_x = limit(
-            [space_between_points * i for i in range(num_items)], 
-            p_radius, 
-            self.size.width - p_radius)
-        
-        points = list(zip(limited_x, limited_y))
-        smooth_points = interpolate(points, num, kind=self.interpol)
+
+        thickness = self.thickness
+        num = self.npoints if self.npoints is not None else num_nodes
+        max_weight = max((i.weight for i in nodes))
+        radius = self.pwidth / 2 if self.pwidth > 0 else thickness / 2
+ 
+        source_p = list(zip(
+            [w / (num_nodes - 1) * i for i in range(num_nodes)], 
+            [max_weight - node.weight for node in nodes]
+        ))
+        smooth_p = interpolate(source_p, num, kind=self.interp)
+        circle_p = linear_to_circle(
+            smooth_p, 
+            self.radius - self.pwidth, 
+            self.minr,
+            self.angle
+        )
 
         if self.fill:
             draw.polygon(
-                [(p_radius, self.size.height)] 
-                + smooth_points 
-                + [(self.size.width-p_radius, self.size.height)],
-                fill=self.fill.rgba, width=0)
+                circle_p,
+                fill=self.fill.rgba, 
+                outline=self.outline.rgba,
+                width=0
+            )
 
         if self.outline:
-            draw.line(smooth_points, fill=self.outline.rgba, width=thickness, joint='curve')
-
-            big_points = (points[0], points[num_items-1])
-            if self.point_width:
-                big_points = smooth_points if self.all_points else points
+            draw.line(
+                circle_p, 
+                fill=self.outline.rgba, 
+                width=thickness, 
+                joint='curve'
+            )
+
+            bold_p = (circle_p[0],)
+            if self.pwidth > 0:
+                step = num // num_nodes
+                bold_p = circle_p[::step] if self.onlysrc and step else circle_p
 
-            for point in big_points:
+            for p in bold_p:
                 draw.ellipse(
-                    (point[0] - p_radius, point[1] - p_radius,
-                     point[0] + p_radius, point[1] + p_radius),
-                     fill=self.outline.rgba, width=0)
+                    (p[0] - radius, p[1] - radius,
+                    p[0] + radius, p[1] + radius),
+                    fill=self.outline.rgba, 
+                    width=0
+                )
 
         return image
+
```

### Comparing `piligraphs-0.0.3/piligraphs/radarchart.py` & `piligraphs-0.0.4/piligraphs/linechart.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,209 +1,234 @@
 from pinkie import Color
 from PIL import Image, ImageDraw
 
-from .basegraph import BaseGraph
-from .utils import get_color, interpolate, Interpolation, linear_to_circle
+from .graph import NodeGraph
+from .utils import limit, interpolate, Interpolation
 
 
-class RadarChart(BaseGraph):
-    """Class representing a Radar chart."""
-    def __init__(self,
-                 *,
-                 radius: int,
-                 thickness: int = 1,
-                 fill: Color | int | str | tuple[int, int, int] | tuple[int, int, int, int] | None = ...,
-                 outline: Color | int | str | tuple[int, int, int] | tuple[int, int, int, int] | None = ...,
-                 point_width: int = 0,
-                 all_points: bool = False,
-                 num_points: int = 0,
-                 interpol: Interpolation = 'linear',
-                 angle: int = 0,
-                 min_radius: int = 0) -> None:
-        """
-        RadarChart constructor.
+class LineChart(NodeGraph):
+    """Class representing a line chart."""
 
+    def __init__(
+        self,
+        size: tuple[int, int],
+        *,
+        thickness: int = 1,
+        fill: Color | int | str | tuple[int, int, int] | tuple[int, int, int, int] | None = ...,
+        outline: Color | int | str | tuple[int, int, int] | tuple[int, int, int, int] | None = ...,
+        pwidth: int = 0,
+        onlysrc: bool = False,
+        npoints: int | None = None,
+        interp: Interpolation = 'linear',
+        minh: int = 0
+    ) -> None:
+        """
         Attributes
         ----------
-        radius: `int`
-            Radius of the chart shape.
+        size: `tuple[int, int]`
+            Image width and height.
         thickness: `int`
             Line thickness.
-        fill: `Color`
-            Fill color.
-        outline: `Color`
-            Line color.
-        point_width: `int`
+        fill: `Color` | `None`
+            Fill color. If = `...`, generates a random color.
+        outline: `Color` | `None`
+            Line color. If = `...`, generates a random color.
+        pwidth: `int`
             Point width.
-        all_points: `bool`
-            If `True`, all points (including intermediate ones) will be drawn.
-            Otherwise, only source points will be displayed.
-        num_points: `int`
-            Number of points. If <= 0, equals to the number of items.
-        interpol: `Interpolation`
+        onlysrc: `bool`
+            To draw bold dots only in source points (without interpolated ones).
+        npoints: `int`
+            Number of points. If <= 0, equals to the number of nodes.
+        interp: `str`
             Kind of interpolation. Used to make a smooth curve.
-        angle: `int`
-            Start angle of the chart.
-        min_radius: `int`
-            Minimum distance between the center and the point.
+        minh: `int`
+            Minimum height from the bottom of the graph.
         """
         super().__init__()
 
-        self.radius = radius
+        self.size = size
         self.thickness = thickness
-        self.fill = get_color(fill)
-        self.outline = get_color(outline)
-        self.point_width = point_width
-        self.all_points = all_points
-        self.num_points = num_points
-        self.interpol = interpol
-        self.angle = angle
-        self.min_radius = min_radius
-
-    @property
-    def radius(self) -> int:
-        """Radar shape radius."""
-        return self._radius
-    
-    @radius.setter
-    def radius(self, value: int):
-        if (hasattr(self, '_min_radius') 
-            and self.min_radius > value):
-            raise ValueError("'radius' can not be smaller than 'minimum'")
-        self._radius = value
-
+        self.fill = fill
+        self.outline = outline
+        self.pwidth = pwidth
+        self.onlysrc = onlysrc
+        self.npoints = npoints
+        self.interp = interp
+        self.minh = minh
+
+    @property
+    def size(self) -> tuple[int, int]:
+        """Image width and height."""
+        return self._size
+    
+    @size.setter
+    def size(self, value: tuple[int, int]):
+        if isinstance(value, tuple):
+            if len(value) != 2:
+                raise ValueError("size should contain 2 items")
+            self._size = value
+        else:
+            raise TypeError(f"size must be a tuple, not {type(value).__name__}")
+        
     @property
     def thickness(self) -> int:
-        """Stroke thickness."""
+        """Line thickness."""
         return self._thickness
     
     @thickness.setter
     def thickness(self, value: int):
-        self._thickness = value
+        if isinstance(value, int):
+            self._thickness = value
+        else:
+            raise TypeError(f"thickness must be an int, not {type(value).__name__}")
 
     @property
-    def fill(self) -> Color:
-        """Fill color."""
+    def fill(self) -> Color | None:
+        """Shape color. If `None`, no shape will be drawn."""
         return self._fill
     
     @fill.setter
-    def fill(self, value: Color):
-        self._fill = value
+    def fill(self, value: Color | int | str | tuple | None):
+        if isinstance(value, Color) or value is None:
+            self._fill = value
+        elif value is ...:
+            self._fill = Color.random()
+        else:
+            self._fill = Color(value)
 
     @property
-    def outline(self) -> Color:
-        """Outline color."""
+    def outline(self) -> Color | None:
+        """Line color. If `None`, no line will be drawn."""
         return self._outline
     
     @outline.setter
-    def outline(self, value: Color):
-        self._outline = value
+    def outline(self, value: Color | int | str | tuple | None):
+        if isinstance(value, Color) or value is None:
+            self._outline = value
+        elif value is ...:
+            self._outline = Color.random()
+        else:
+            self._outline = Color(value)
+
+    @property
+    def pwidth(self) -> int:
+        """Point width."""
+        return self._pwidth
+    
+    @pwidth.setter
+    def pwidth(self, value: int):
+        if isinstance(value, int):
+            self._pwidth = value
+        else:
+            raise TypeError(f"pwidth must be an int, not {type(value).__name__}")
+    
+    @property
+    def onlysrc(self) -> bool:
+        """To draw only source points without interpolated ones."""
+        return self._onlysrc
+    
+    @onlysrc.setter
+    def onlysrc(self, value: bool):
+        if isinstance(value, bool):
+            self._onlysrc = value
+        else:
+            raise TypeError(f"onlysrc must be a bool, not {type(value).__name__}")
 
     @property
-    def point_width(self) -> int:
-        """Stroke points width."""
-        return self._point_width
-    
-    @point_width.setter
-    def point_width(self, value: int):
-        self._point_width = value
-
-    @property
-    def all_points(self) -> bool:
-        """Draw all points or not."""
-        return self._all_points
-    
-    @all_points.setter
-    def all_points(self, value: bool):
-        self._all_points = value
-
-    @property
-    def num_points(self) -> int:
+    def npoints(self) -> int | None:
         """Number of points."""
-        return self._num_points
-    
-    @num_points.setter
-    def num_points(self, value: int):
-        self._num_points = value
-
-    @property
-    def interpol(self) -> Interpolation:
-        """Kinf of interpolation."""
-        return self._interpol
-    
-    @interpol.setter
-    def interpol(self, value: Interpolation):
-        self._interpol = value
-
-    @property
-    def angle(self) -> int | None:
-        """Chart start angle."""
-        return self._angle
+        return self._npoints
     
-    @angle.setter
-    def angle(self, value: int):
-        self._angle = value
-
+    @npoints.setter
+    def npoints(self, value: int | None):
+        if isinstance(value, int) or value is None:
+            self._npoints = value
+        else:
+            raise TypeError(f"npoints must be an int or None, not {type(value).__name__}")
+        
     @property
-    def min_radius(self) -> int:
-        """Minimum distance between center and point."""
-        return self._min_radius
-    
-    @min_radius.setter
-    def min_radius(self, value: int):
-        if (hasattr(self, '_radius')
-            and self.radius < value):
-            raise ValueError("'min_radius' can not be bigger than 'radius'")
-        self._min_radius = value
+    def interp(self) -> Interpolation:
+        """Kind of interpolation."""
+        return self._interp
+    
+    @interp.setter
+    def interp(self, value: Interpolation):
+        if isinstance(value, Interpolation):
+            self._interp = value
+        else:
+            raise TypeError("interp must be a valid string")
+    
+    @property
+    def minh(self) -> int:
+        """Minimal point height."""
+        return self._minh
+    
+    @minh.setter
+    def minh(self, value: int):
+        if isinstance(value, int):
+            self._minh = value
+        else:
+            raise TypeError(f"minh must be an int, not {type(value).__name__}")
 
     def draw(self) -> Image.Image:
-        image = Image.new('RGBA', (self.radius * 2,)*2)
-        items = self.items
-        items.append(items[0])
-        num_items = len(items)
+        image = Image.new('RGBA', self.size)
+        num_nodes = len(self.nodes)
 
-        if num_items == 0:
+        if num_nodes == 0:
             return image
         
         draw = ImageDraw.Draw(image)
-        thickness = self.thickness or 1
-        num = self.num_points if self.num_points > 0 else num_items
-        max_weight = max((i.weight for i in items))
-        p_radius = self.point_width / 2 if self.point_width > 0 else thickness / 2
-        space_between_points = image.size[0] / (num_items - 1)
-      
-        points = list(zip(
-            [space_between_points * i for i in range(num_items)], 
-            [max_weight - item.weight for item in items]))
-        smooth_points = interpolate(points, num, kind=self.interpol)
-        circle_points = linear_to_circle(
-            smooth_points, 
-            self.radius - self.point_width, 
-            self.min_radius,
-            self.angle)
+
+        w, h = self.size
+        thickness = self.thickness
+        num = self.npoints if self.npoints else num_nodes
+        max_weight = max((i.weight for i in self.nodes))
+        radius = self.pwidth / 2 if self.pwidth > 0 else thickness / 2
+
+        lim_xs = limit(
+            [w / (num_nodes - 1) * i for i in range(num_nodes)], 
+            radius, 
+            w - radius
+        )
+
+        if max_weight == 0:
+            lim_ys = [h - radius] * num_nodes
+        else:
+            lim_ys = limit(
+                [max_weight - node.weight for node in self.nodes], 
+                radius, 
+                h - radius - self.minh
+            )
+        
+        source_p = list(zip(lim_xs, lim_ys))
+        smooth_p = interpolate(source_p, num, kind=self.interp)
 
         if self.fill:
             draw.polygon(
-                circle_points,
+                [(radius, h)] + smooth_p + [(w - radius, h)],
                 fill=self.fill.rgba, 
-                outline=self.outline.rgba,
-                width=0)
+                width=0
+            )
 
         if self.outline:
             draw.line(
-                circle_points + [circle_points[0]], 
+                smooth_p, 
                 fill=self.outline.rgba, 
                 width=thickness, 
-                joint='curve')
+                joint='curve'
+            )
 
-            big_points = (circle_points[0],)
-            if self.point_width > 0:
-                big_points = circle_points if self.all_points else circle_points[::num//num_items]
+            bald_p = (source_p[0], source_p[num_nodes-1])
+            if self.pwidth:
+                bald_p = source_p if self.onlysrc else smooth_p
 
-            for point in big_points:
+            for x, y in bald_p:
                 draw.ellipse(
-                    (point[0] - p_radius, point[1] - p_radius,
-                    point[0] + p_radius, point[1] + p_radius),
-                    fill=self.outline.rgba, width=0)
+                    (
+                        (x - radius, y - radius),
+                        (x + radius, y + radius)
+                    ),
+                    fill=self.outline.rgba, 
+                    width=0
+                )
 
         return image
-
```

### Comparing `piligraphs-0.0.3/piligraphs/utils.py` & `piligraphs-0.0.4/piligraphs/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,61 @@
 import math
 import numpy as np
-from pinkie import Color
 from scipy.interpolate import interp1d
 from typing import Literal
 
 
+Interpolation = Literal[
+    'linear',
+    'nearest',
+    'nearest-up',
+    'zero',
+    'slinear',
+    'quadratic',
+    'cubic',
+    'previous',
+    'next'
+]
+
+
 def rgb_to_hex(_rgb: tuple[int, int, int], /):
     return '{:02x}{:02x}{:02x}'.format(_rgb[0], _rgb[1], _rgb[2])
 
 
 def hex_to_rgb(_hex: str, /):
     return tuple(int(_hex.strip('#')[i:i+2], 16) for i in (0, 2, 4))
 
 
 def num_to_rgb(_num: int, /):
-    return ((_num >> 16) & 255,
-            (_num >> 8) & 255,
-            _num & 255)
+    return (
+        (_num >> 16) & 255,
+        (_num >> 8) & 255,
+        _num & 255
+    )
 
 
 def rgb_to_num(_rgb: tuple[int, int, int], /):
     return (_rgb[0] << 16) + (_rgb[1] << 8) + _rgb[2]
 
 
 def circle_xy(radius: int, distance: int, angle: int):
     rad = math.radians(angle)
-    return (radius + distance * math.cos(rad),
-            radius + distance * math.sin(rad))
-
-
-def get_color(color, /):
-    """
-    Returns
-    -------
-    `Color` or `None` if color is `None`.
-    """
-    if isinstance(color, Color):
-        return color
-    elif color == ...:
-        return Color.random()
-    elif color is not None:
-        return Color(color)
-    else:
-        return Color((0, 0, 0, 0))
-    
-
-Interpolation = Literal[
-    'linear',
-    'nearest',
-    'nearest-up',
-    'zero',
-    'slinear',
-    'quadratic',
-    'cubic',
-    'previous',
-    'next'
-]
+    return (
+        radius + distance * math.cos(rad),
+        radius + distance * math.sin(rad)
+    )
 
 
 def interpolate(
-        points: list[tuple[int, int]], 
-        num: int | None = None, 
-        kind: Interpolation = 'linear') -> list[tuple[int, int]]:
+    points: list[tuple[int, int]], 
+    num: int | None = None, 
+    kind: str = 'linear'
+) -> list[tuple[int, int]]:
     """
-    Interpolate list of points to make a smooth curve.
+    Interpolate a list of points to make a smooth curve.
 
     Attributes
     ----------
     points: `list[tuple[int, int]]`
         List of points. Every point must be a tuple containing 2 integers: x and y.
     num: `int` | `None`
         Number of points. If `None`, double the length of the list of points is set.
@@ -83,19 +71,20 @@
     x_new = np.linspace(min(x), max(x), num)
     y_new = np.clip(inter(x_new), min(y), max(y))
 
     return list(zip(x_new, y_new))
 
 
 def limit(
-        values: list[int | float],
-        minv: int | float,
-        maxv: int | float,
-        *,
-        copy: bool = True) -> np.ndarray:
+    values: list[int | float],
+    minv: int | float,
+    maxv: int | float,
+    *,
+    copy: bool = True
+) -> np.ndarray:
     """
     Limit array to specific range.
 
     Attributes
     ----------
     values: `list[int | float]`
         List of values.
@@ -115,18 +104,19 @@
     m = (maxv - minv) / (_max - _min)
     b = maxv - m * _max
 
     return m * array + b
 
 
 def linear_to_circle(
-        points: list[tuple[int, int]], 
-        radius: int, 
-        min_radius: int = 0, 
-        angle: int = 0) -> list[tuple[int, int]]:
+    points: list[tuple[int, int]], 
+    radius: int, 
+    min_radius: int = 0, 
+    angle: int = 0
+) -> list[tuple[int, int]]:
     """
     Convert linear points to circular.
 
     Attributes
     ----------
     points: `list[tuple[int, int]]`
         List of points.
```

