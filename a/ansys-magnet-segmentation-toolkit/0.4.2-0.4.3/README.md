# Comparing `tmp/ansys_magnet_segmentation_toolkit-0.4.2.tar.gz` & `tmp/ansys_magnet_segmentation_toolkit-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_magnet_segmentation_toolkit-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_magnet_segmentation_toolkit-0.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_magnet_segmentation_toolkit-0.4.2.tar` & `ansys_magnet_segmentation_toolkit-0.4.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1089 2024-05-15 15:28:35.413612 ansys_magnet_segmentation_toolkit-0.4.2/LICENSE
--rw-r--r--   0        0        0     3174 2024-05-15 15:28:35.413612 ansys_magnet_segmentation_toolkit-0.4.2/README.rst
--rw-r--r--   0        0        0     1711 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1234 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/__init__.py
--rw-r--r--   0        0        0     1213 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/backend/__init__.py
--rw-r--r--   0        0        0      304 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/backend/aedt_properties.toml
--rw-r--r--   0        0        0     1949 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/backend/api.py
--rw-r--r--   0        0        0     2986 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/backend/models.py
--rw-r--r--   0        0        0     3791 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/backend/run_backend.py
--rw-r--r--   0        0        0     1233 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/backend/workflows/__init__.py
--rw-r--r--   0        0        0    17731 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/backend/workflows/aedt.py
--rw-r--r--   0        0        0     4100 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/run_toolkit.py
--rw-r--r--   0        0        0     1153 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/__init__.py
--rw-r--r--   0        0        0    11628 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/actions.py
--rw-r--r--   0        0        0     1219 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/frontend_properties.toml
--rw-r--r--   0        0        0     2471 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/models.py
--rw-r--r--   0        0        0     7558 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/run_frontend.py
--rw-r--r--   0        0        0        0 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/__init__.py
--rw-r--r--   0        0        0     2505 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_column.py
--rw-r--r--   0        0        0     1961 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_column.ui
--rw-r--r--   0        0        0     6616 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_menu.py
--rw-r--r--   0        0        0     2958 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_page.py
--rw-r--r--   0        0        0     2125 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_page.ui
--rw-r--r--   0        0        0     2536 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_column.py
--rw-r--r--   0        0        0     1967 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_column.ui
--rw-r--r--   0        0        0    10286 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_menu.py
--rw-r--r--   0        0        0     5658 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_page.py
--rw-r--r--   0        0        0     5227 2024-05-15 15:28:35.417612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_page.ui
--rw-r--r--   0        0        0     1153 2024-05-15 15:28:35.421612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/__init__.py
--rw-r--r--   0        0        0     2515 2024-05-15 15:28:35.421612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_column.py
--rw-r--r--   0        0        0     1963 2024-05-15 15:28:35.421612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_column.ui
--rw-r--r--   0        0        0    15672 2024-05-15 15:28:35.421612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_menu.py
--rw-r--r--   0        0        0    15823 2024-05-15 15:28:35.421612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_page.py
--rw-r--r--   0        0        0    16820 2024-05-15 15:28:35.421612 ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_page.ui
--rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 ansys_magnet_segmentation_toolkit-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-05-16 07:50:03.618427 ansys_magnet_segmentation_toolkit-0.4.3/LICENSE
+-rw-r--r--   0        0        0     3174 2024-05-16 07:50:03.618427 ansys_magnet_segmentation_toolkit-0.4.3/README.rst
+-rw-r--r--   0        0        0     1711 2024-05-16 07:50:03.622427 ansys_magnet_segmentation_toolkit-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1234 2024-05-16 07:50:03.622427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/__init__.py
+-rw-r--r--   0        0        0     1213 2024-05-16 07:50:03.622427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/__init__.py
+-rw-r--r--   0        0        0      304 2024-05-16 07:50:03.622427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/aedt_properties.toml
+-rw-r--r--   0        0        0     1949 2024-05-16 07:50:03.622427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/api.py
+-rw-r--r--   0        0        0     2986 2024-05-16 07:50:03.622427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/models.py
+-rw-r--r--   0        0        0     3791 2024-05-16 07:50:03.622427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/run_backend.py
+-rw-r--r--   0        0        0     1233 2024-05-16 07:50:03.622427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/workflows/__init__.py
+-rw-r--r--   0        0        0    17731 2024-05-16 07:50:03.622427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/workflows/aedt.py
+-rw-r--r--   0        0        0     4100 2024-05-16 07:50:03.622427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/run_toolkit.py
+-rw-r--r--   0        0        0     1153 2024-05-16 07:50:03.622427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/__init__.py
+-rw-r--r--   0        0        0    11628 2024-05-16 07:50:03.622427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/actions.py
+-rw-r--r--   0        0        0     1219 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/frontend_properties.toml
+-rw-r--r--   0        0        0     2471 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/models.py
+-rw-r--r--   0        0        0     7558 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/run_frontend.py
+-rw-r--r--   0        0        0        0 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/__init__.py
+-rw-r--r--   0        0        0     2505 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_column.py
+-rw-r--r--   0        0        0     1961 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_column.ui
+-rw-r--r--   0        0        0     6616 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_menu.py
+-rw-r--r--   0        0        0     2958 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_page.py
+-rw-r--r--   0        0        0     2125 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_page.ui
+-rw-r--r--   0        0        0     2536 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_column.py
+-rw-r--r--   0        0        0     1967 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_column.ui
+-rw-r--r--   0        0        0    10286 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_menu.py
+-rw-r--r--   0        0        0     5658 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_page.py
+-rw-r--r--   0        0        0     5227 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_page.ui
+-rw-r--r--   0        0        0     1153 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/__init__.py
+-rw-r--r--   0        0        0     2515 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_column.py
+-rw-r--r--   0        0        0     1963 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_column.ui
+-rw-r--r--   0        0        0    15672 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_menu.py
+-rw-r--r--   0        0        0    15823 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_page.py
+-rw-r--r--   0        0        0    16820 2024-05-16 07:50:03.626427 ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_page.ui
+-rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 ansys_magnet_segmentation_toolkit-0.4.3/PKG-INFO
```

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/LICENSE` & `ansys_magnet_segmentation_toolkit-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/README.rst` & `ansys_magnet_segmentation_toolkit-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/pyproject.toml` & `ansys_magnet_segmentation_toolkit-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/__init__.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """
 ToolkitBackend dedicated to magnet segmentation.
 """
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
```

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/backend/__init__.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/backend/api.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/api.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/backend/models.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/models.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/backend/run_backend.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/run_backend.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/backend/workflows/__init__.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/backend/workflows/aedt.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/workflows/aedt.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/run_toolkit.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/run_toolkit.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/__init__.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/actions.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/actions.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/frontend_properties.toml` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/frontend_properties.toml`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/models.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/models.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/run_frontend.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/run_frontend.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_column.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_column.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_column.ui` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_column.ui`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_menu.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_menu.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_page.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_page.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_page.ui` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_page.ui`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_column.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_column.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_column.ui` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_column.ui`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_menu.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_menu.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_page.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_page.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_page.ui` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_page.ui`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/__init__.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_column.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_column.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_column.ui` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_column.ui`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_menu.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_menu.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_page.py` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_page.py`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_page.ui` & `ansys_magnet_segmentation_toolkit-0.4.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_page.ui`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.4.2/PKG-INFO` & `ansys_magnet_segmentation_toolkit-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-magnet-segmentation-toolkit
-Version: 0.4.2
+Version: 0.4.3
 Summary: Toolkit used for automating the segmentation and skew of interior permanent magnet (IPM) and surface permanent magnet (SPM) motors using Ansys Electronics Desktop (AEDT)
 Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

