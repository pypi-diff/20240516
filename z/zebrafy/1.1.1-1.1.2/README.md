# Comparing `tmp/zebrafy-1.1.1.tar.gz` & `tmp/zebrafy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zebrafy-1.1.1.tar", last modified: Sun May 12 01:59:26 2024, max compression
+gzip compressed data, was "zebrafy-1.1.2.tar", last modified: Thu May 16 06:16:10 2024, max compression
```

## Comparing `zebrafy-1.1.1.tar` & `zebrafy-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-12 01:59:26.310485 zebrafy-1.1.1/
--rw-r--r--   0 m         (1000) m         (1000)     7652 2023-08-06 02:30:03.000000 zebrafy-1.1.1/LICENSE.txt
--rw-r--r--   0 m         (1000) m         (1000)    11154 2024-05-12 01:59:26.310485 zebrafy-1.1.1/PKG-INFO
--rw-r--r--   0 m         (1000) m         (1000)     9661 2024-05-12 01:57:46.000000 zebrafy-1.1.1/README.rst
--rw-r--r--   0 m         (1000) m         (1000)     1780 2024-05-12 01:57:16.000000 zebrafy-1.1.1/pyproject.toml
--rw-r--r--   0 m         (1000) m         (1000)       38 2024-05-12 01:59:26.310485 zebrafy-1.1.1/setup.cfg
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-12 01:59:26.310485 zebrafy-1.1.1/tests/
--rw-r--r--   0 m         (1000) m         (1000)    21962 2024-05-12 01:58:41.000000 zebrafy-1.1.1/tests/test_zebrafy.py
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-12 01:59:26.310485 zebrafy-1.1.1/zebrafy/
--rw-r--r--   0 m         (1000) m         (1000)      196 2024-05-12 01:58:20.000000 zebrafy-1.1.1/zebrafy/__init__.py
--rw-r--r--   0 m         (1000) m         (1000)     3401 2023-10-28 06:18:28.000000 zebrafy-1.1.1/zebrafy/crc.py
--rw-r--r--   0 m         (1000) m         (1000)     6644 2024-03-24 00:36:09.000000 zebrafy-1.1.1/zebrafy/graphic_field.py
--rw-r--r--   0 m         (1000) m         (1000)    11276 2024-03-24 00:36:09.000000 zebrafy-1.1.1/zebrafy/zebrafy_image.py
--rw-r--r--   0 m         (1000) m         (1000)    11394 2024-05-12 01:56:42.000000 zebrafy-1.1.1/zebrafy/zebrafy_pdf.py
--rw-r--r--   0 m         (1000) m         (1000)     5654 2024-03-24 00:36:09.000000 zebrafy-1.1.1/zebrafy/zebrafy_zpl.py
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-12 01:59:26.310485 zebrafy-1.1.1/zebrafy.egg-info/
--rw-r--r--   0 m         (1000) m         (1000)    11154 2024-05-12 01:59:26.000000 zebrafy-1.1.1/zebrafy.egg-info/PKG-INFO
--rw-r--r--   0 m         (1000) m         (1000)      344 2024-05-12 01:59:26.000000 zebrafy-1.1.1/zebrafy.egg-info/SOURCES.txt
--rw-r--r--   0 m         (1000) m         (1000)        1 2024-05-12 01:59:26.000000 zebrafy-1.1.1/zebrafy.egg-info/dependency_links.txt
--rw-r--r--   0 m         (1000) m         (1000)      107 2024-05-12 01:59:26.000000 zebrafy-1.1.1/zebrafy.egg-info/requires.txt
--rw-r--r--   0 m         (1000) m         (1000)        8 2024-05-12 01:59:26.000000 zebrafy-1.1.1/zebrafy.egg-info/top_level.txt
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-16 06:16:10.856267 zebrafy-1.1.2/
+-rw-r--r--   0 m         (1000) m         (1000)     7652 2023-08-06 02:30:03.000000 zebrafy-1.1.2/LICENSE.txt
+-rw-r--r--   0 m         (1000) m         (1000)    11576 2024-05-16 06:16:10.856267 zebrafy-1.1.2/PKG-INFO
+-rw-r--r--   0 m         (1000) m         (1000)    10083 2024-05-16 06:12:27.000000 zebrafy-1.1.2/README.rst
+-rw-r--r--   0 m         (1000) m         (1000)     1780 2024-05-16 06:04:12.000000 zebrafy-1.1.2/pyproject.toml
+-rw-r--r--   0 m         (1000) m         (1000)       38 2024-05-16 06:16:10.856267 zebrafy-1.1.2/setup.cfg
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-16 06:16:10.856267 zebrafy-1.1.2/tests/
+-rw-r--r--   0 m         (1000) m         (1000)    23562 2024-05-16 06:03:54.000000 zebrafy-1.1.2/tests/test_zebrafy.py
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-16 06:16:10.856267 zebrafy-1.1.2/zebrafy/
+-rw-r--r--   0 m         (1000) m         (1000)      196 2024-05-16 06:04:01.000000 zebrafy-1.1.2/zebrafy/__init__.py
+-rw-r--r--   0 m         (1000) m         (1000)     3401 2024-05-16 01:49:32.000000 zebrafy-1.1.2/zebrafy/crc.py
+-rw-r--r--   0 m         (1000) m         (1000)     6644 2024-05-16 01:49:53.000000 zebrafy-1.1.2/zebrafy/graphic_field.py
+-rw-r--r--   0 m         (1000) m         (1000)    12300 2024-05-16 06:02:35.000000 zebrafy-1.1.2/zebrafy/zebrafy_image.py
+-rw-r--r--   0 m         (1000) m         (1000)    12363 2024-05-16 06:02:35.000000 zebrafy-1.1.2/zebrafy/zebrafy_pdf.py
+-rw-r--r--   0 m         (1000) m         (1000)     5654 2024-05-16 01:48:59.000000 zebrafy-1.1.2/zebrafy/zebrafy_zpl.py
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-16 06:16:10.856267 zebrafy-1.1.2/zebrafy.egg-info/
+-rw-r--r--   0 m         (1000) m         (1000)    11576 2024-05-16 06:16:10.000000 zebrafy-1.1.2/zebrafy.egg-info/PKG-INFO
+-rw-r--r--   0 m         (1000) m         (1000)      344 2024-05-16 06:16:10.000000 zebrafy-1.1.2/zebrafy.egg-info/SOURCES.txt
+-rw-r--r--   0 m         (1000) m         (1000)        1 2024-05-16 06:16:10.000000 zebrafy-1.1.2/zebrafy.egg-info/dependency_links.txt
+-rw-r--r--   0 m         (1000) m         (1000)      107 2024-05-16 06:16:10.000000 zebrafy-1.1.2/zebrafy.egg-info/requires.txt
+-rw-r--r--   0 m         (1000) m         (1000)        8 2024-05-16 06:16:10.000000 zebrafy-1.1.2/zebrafy.egg-info/top_level.txt
```

### Comparing `zebrafy-1.1.1/LICENSE.txt` & `zebrafy-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.1/PKG-INFO` & `zebrafy-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zebrafy
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python library for converting PDF and images to Zebra Programming Language (ZPL)
 Author-email: Miika Nissi <miika@miikanissi.com>
 Maintainer-email: Miika Nissi <miika@miikanissi.com>
 License: LGPLv3
 Project-URL: Homepage, https://github.com/miikanissi/zebrafy/
 Project-URL: Documentation, https://zebrafy.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
@@ -44,17 +44,17 @@
     :target: https://github.com/miikanissi/zebrafy/actions/workflows/ci.yml
     :alt: CI
 
 .. image:: https://readthedocs.org/projects/zebrafy/badge/?version=latest
     :target: https://zebrafy.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/badge/pypi-1.1.1-blue
-    :target: https://pypi.org/project/zebrafy/
-    :alt: PyPi Package
+.. image:: https://img.shields.io/pypi/v/zebrafy
+    :target: https://pypi.org/project/zebrafy
+    :alt: Zebrafy PyPi Package
 
 .. image:: https://img.shields.io/badge/license-LGPLv3-green
     :target: https://www.gnu.org/licenses/lgpl-3.0.en.html#license-text
     :alt: License
 
 **Zebrafy** is a Python 3 library for converting PDF and images to and from
 `Zebra Programming Language (ZPL) <https://en.wikipedia.org/wiki/Zebra_Programming_Language>`_
@@ -88,25 +88,28 @@
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``height``           | Height of the image in the resulting ZPL, ``0`` to use original image/PDF height (default ``0``)             |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``pos_x``            | Pixel x position of the graphic field in resulting ZPL (default ``0``)                                       |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``pos_y``            | Pixel y position of the graphic field in resulting ZPL (default ``0``)                                       |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
+| ``rotation``         | Rotates the image by the specified degree (``0``, ``90``, ``180`` or ``270``, default ``0``)                 |
++----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``complete_zpl``     | Add ZPL header and footer or only get the ZPL graphic field output (``True`` or ``False``, default ``True``) |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 
 Additionally, **ZebrafyPDF** supports the following optional parameters:
 
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | Parameter            | Description                                                                                                  |
 +======================+==============================================================================================================+
 | ``split_pages``      | Split the PDF into separate ZPL labels for each page (``True`` or ``False``, default ``False``)              |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 
+
 Getting Started
 ---------------
 
 Installation
 ^^^^^^^^^^^^
 
 .. code-block:: console
@@ -154,14 +157,15 @@
           invert=True,
           dither=False,
           threshold=128,
           width=720,
           height=1280,
           pos_x=100,
           pos_y=100,
+          rotation=90,
           complete_zpl=True,
       ).to_zpl()
 
   with open("output.zpl", "w") as zpl:
       zpl.write(zpl_string)
 
 Alternatively, **ZebrafyImage** also accepts PIL Image as the image parameter instead of
@@ -191,15 +195,15 @@
   with open("source.pdf", "rb") as pdf:
       zpl_string = ZebrafyPDF(pdf.read()).to_zpl()
 
   with open("output.zpl", "w") as zpl:
       zpl.write(zpl_string)
 
 **ZebrafyPDF** conversion supports the same optional parameters as **ZebrafyImage**
-conversion:
+conversion, with the addition of the ``split_pages`` parameter to split the PDF pages:
 
 .. code-block:: python
 
   from zebrafy import ZebrafyPDF
 
   with open("source.pdf", "rb") as pdf:
       zpl_string = ZebrafyPDF(
@@ -208,15 +212,17 @@
           invert=True,
           dither=False,
           threshold=128,
           width=720,
           height=1280,
           pos_x=100,
           pos_y=100,
+          rotation=90,
           complete_zpl=True,
+          split_pages=True,
       ).to_zpl()
 
   with open("output.zpl", "w") as zpl:
       zpl.write(zpl_string)
 
 ZPL to PDF or Images with **ZebrafyZPL**
 """"""""""""""""""""""""""""""""""""""""
```

### Comparing `zebrafy-1.1.1/README.rst` & `zebrafy-1.1.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     :target: https://github.com/miikanissi/zebrafy/actions/workflows/ci.yml
     :alt: CI
 
 .. image:: https://readthedocs.org/projects/zebrafy/badge/?version=latest
     :target: https://zebrafy.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/badge/pypi-1.1.1-blue
-    :target: https://pypi.org/project/zebrafy/
-    :alt: PyPi Package
+.. image:: https://img.shields.io/pypi/v/zebrafy
+    :target: https://pypi.org/project/zebrafy
+    :alt: Zebrafy PyPi Package
 
 .. image:: https://img.shields.io/badge/license-LGPLv3-green
     :target: https://www.gnu.org/licenses/lgpl-3.0.en.html#license-text
     :alt: License
 
 **Zebrafy** is a Python 3 library for converting PDF and images to and from
 `Zebra Programming Language (ZPL) <https://en.wikipedia.org/wiki/Zebra_Programming_Language>`_
@@ -52,25 +52,28 @@
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``height``           | Height of the image in the resulting ZPL, ``0`` to use original image/PDF height (default ``0``)             |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``pos_x``            | Pixel x position of the graphic field in resulting ZPL (default ``0``)                                       |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``pos_y``            | Pixel y position of the graphic field in resulting ZPL (default ``0``)                                       |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
+| ``rotation``         | Rotates the image by the specified degree (``0``, ``90``, ``180`` or ``270``, default ``0``)                 |
++----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``complete_zpl``     | Add ZPL header and footer or only get the ZPL graphic field output (``True`` or ``False``, default ``True``) |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 
 Additionally, **ZebrafyPDF** supports the following optional parameters:
 
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | Parameter            | Description                                                                                                  |
 +======================+==============================================================================================================+
 | ``split_pages``      | Split the PDF into separate ZPL labels for each page (``True`` or ``False``, default ``False``)              |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 
+
 Getting Started
 ---------------
 
 Installation
 ^^^^^^^^^^^^
 
 .. code-block:: console
@@ -118,14 +121,15 @@
           invert=True,
           dither=False,
           threshold=128,
           width=720,
           height=1280,
           pos_x=100,
           pos_y=100,
+          rotation=90,
           complete_zpl=True,
       ).to_zpl()
 
   with open("output.zpl", "w") as zpl:
       zpl.write(zpl_string)
 
 Alternatively, **ZebrafyImage** also accepts PIL Image as the image parameter instead of
@@ -155,15 +159,15 @@
   with open("source.pdf", "rb") as pdf:
       zpl_string = ZebrafyPDF(pdf.read()).to_zpl()
 
   with open("output.zpl", "w") as zpl:
       zpl.write(zpl_string)
 
 **ZebrafyPDF** conversion supports the same optional parameters as **ZebrafyImage**
-conversion:
+conversion, with the addition of the ``split_pages`` parameter to split the PDF pages:
 
 .. code-block:: python
 
   from zebrafy import ZebrafyPDF
 
   with open("source.pdf", "rb") as pdf:
       zpl_string = ZebrafyPDF(
@@ -172,15 +176,17 @@
           invert=True,
           dither=False,
           threshold=128,
           width=720,
           height=1280,
           pos_x=100,
           pos_y=100,
+          rotation=90,
           complete_zpl=True,
+          split_pages=True,
       ).to_zpl()
 
   with open("output.zpl", "w") as zpl:
       zpl.write(zpl_string)
 
 ZPL to PDF or Images with **ZebrafyZPL**
 """"""""""""""""""""""""""""""""""""""""
```

### Comparing `zebrafy-1.1.1/pyproject.toml` & `zebrafy-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zebrafy"
-version = "1.1.1"
+version = "1.1.2"
 description = "Python library for converting PDF and images to Zebra Programming Language (ZPL)"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Operating System :: OS Independent",
     "Natural Language :: English",
     "Programming Language :: Python",
```

### Comparing `zebrafy-1.1.1/tests/test_zebrafy.py` & `zebrafy-1.1.2/tests/test_zebrafy.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             os.path.join(os.path.join(os.path.dirname(__file__), "static"), file_name),
             open_mode,
         ) as file:
             return file.read()
 
     def test_version(self):
         """Test package version."""
-        self.assertEqual(__version__, "1.1.1")
+        self.assertEqual(__version__, "1.1.2")
 
     ###########
     # CRC Tests
     ###########
     def test_crc_data_bytes(self):
         with self.assertRaises(ValueError):
             CRC(None)
@@ -191,14 +191,27 @@
         im = Image.new(mode="RGB", size=(200, 200))
         zebrafy_image = ZebrafyImage(im)
         with self.assertRaises(ValueError):
             zebrafy_image.pos_y = None
         with self.assertRaises(TypeError):
             zebrafy_image.pos_y = "123"
 
+    def test_zebrafy_image_rotation(self):
+        """Test ZebrafyImage rotation input"""
+        im = Image.new(mode="RGB", size=(200, 200))
+        zebrafy_image = ZebrafyImage(im)
+        with self.assertRaises(ValueError):
+            zebrafy_image.rotation = None
+        with self.assertRaises(TypeError):
+            zebrafy_image.rotation = "123"
+        with self.assertRaises(TypeError):
+            zebrafy_image.rotation = 90.0
+        with self.assertRaises(ValueError):
+            zebrafy_image.rotation = 45
+
     def test_zebrafy_image_complete_zpl(self):
         """Test ZebrafyImage complete_zpl input"""
         im = Image.new(mode="RGB", size=(200, 200))
         zebrafy_image = ZebrafyImage(im)
         with self.assertRaises(ValueError):
             zebrafy_image.complete_zpl = None
         with self.assertRaises(TypeError):
@@ -280,14 +293,21 @@
     def test_image_to_zpl_pos_x_pos_y(self):
         """Test image to ZPL with pos_x and pos_y."""
         gf_zpl = ZebrafyImage(
             self._read_static_file("test_image.png"), pos_x=100, pos_y=200
         ).to_zpl()
         self.assertEqual(gf_zpl, self._read_static_file("test_image_pos_x_pos_y.zpl"))
 
+    def test_image_to_zpl_rotation(self):
+        """Test image to ZPL with rotation."""
+        gf_zpl = ZebrafyImage(
+            self._read_static_file("test_image.png"), rotation=90
+        ).to_zpl()
+        self.assertEqual(gf_zpl, self._read_static_file("test_image_rotation.zpl"))
+
     def test_multiple_image_to_zpl(self):
         """Test multiple images to ZPL with default options."""
         gf_zpl = ZebrafyImage(
             self._read_static_file("test_image.png"),
             complete_zpl=False,
         ).to_zpl()
         complete_zpl = "^XA\n" + gf_zpl + "\n" + gf_zpl + "\n^XZ\n"
@@ -389,14 +409,27 @@
         pdf = self._read_static_file("test_pdf.pdf")
         zebrafy_pdf = ZebrafyPDF(pdf)
         with self.assertRaises(ValueError):
             zebrafy_pdf.pos_y = None
         with self.assertRaises(TypeError):
             zebrafy_pdf.pos_y = "123"
 
+    def test_zebrafy_pdf_rotation(self):
+        """Test ZebrafyPDF rotation"""
+        pdf = self._read_static_file("test_pdf.pdf")
+        zebrafy_pdf = ZebrafyPDF(pdf)
+        with self.assertRaises(ValueError):
+            zebrafy_pdf.rotation = None
+        with self.assertRaises(TypeError):
+            zebrafy_pdf.rotation = "123"
+        with self.assertRaises(TypeError):
+            zebrafy_pdf.rotation = 90.0
+        with self.assertRaises(ValueError):
+            zebrafy_pdf.rotation = 45
+
     def test_zebrafy_pdf_complete_zpl(self):
         """Test ZebrafyPDF complete_zpl input"""
         pdf = self._read_static_file("test_pdf.pdf")
         zebrafy_pdf = ZebrafyPDF(pdf)
         with self.assertRaises(ValueError):
             zebrafy_pdf.complete_zpl = None
         with self.assertRaises(TypeError):
@@ -461,14 +494,21 @@
     def test_pdf_to_zpl_width_height(self):
         """Test PDF to ZPL with set width and height."""
         gf_zpl = ZebrafyPDF(
             self._read_static_file("test_pdf.pdf"), width=720, height=1280
         ).to_zpl()
         self.assertEqual(gf_zpl, self._read_static_file("test_pdf_width_height.zpl"))
 
+    def test_pdf_to_zpl_rotation(self):
+        """Test PDF to ZPL with rotation."""
+        gf_zpl = ZebrafyPDF(
+            self._read_static_file("test_pdf.pdf"), rotation=90
+        ).to_zpl()
+        self.assertEqual(gf_zpl, self._read_static_file("test_pdf_rotation.zpl"))
+
     def test_pdf_to_zpl_split_pages(self):
         """Test PDF to ZPL with split pages."""
         gf_zpl = ZebrafyPDF(
             self._read_static_file("test_pdf.pdf"), split_pages=True
         ).to_zpl()
         self.assertEqual(gf_zpl, self._read_static_file("test_pdf_split_pages.zpl"))
```

### Comparing `zebrafy-1.1.1/zebrafy/crc.py` & `zebrafy-1.1.2/zebrafy/crc.py`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.1/zebrafy/graphic_field.py` & `zebrafy-1.1.2/zebrafy/graphic_field.py`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.1/zebrafy/zebrafy_image.py` & `zebrafy-1.1.2/zebrafy/zebrafy_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,16 @@
     to ``128``
     :param width: Width of the image in the resulting ZPL. If ``0``, use default image \
     width, defaults to ``0``
     :param height: Height of the image in the resulting ZPL. If ``0``, use default \
     image height, defaults to ``0``
     :param pos_x: X position of the image on the resulting ZPL, defaults to ``0``
     :param pos_y: Y position of the image on the resulting ZPL, defaults to ``0``
+    :param rotation: Additional rotation in degrees ``0``, ``90``, ``180``, or \
+    ``270``, defaults to ``0``
     :param complete_zpl: Return a complete ZPL with header and footer included. \
     Otherwise return only the graphic field, defaults to ``True``
 
     .. deprecated:: 1.1.0
         The `compression_type` parameter is deprecated in favor of `format` and will \
         be removed in version 2.0.0.
     """
@@ -78,14 +80,15 @@
         invert: bool = None,
         dither: bool = None,
         threshold: int = None,
         width: int = None,
         height: int = None,
         pos_x: int = None,
         pos_y: int = None,
+        rotation: int = None,
         complete_zpl: bool = None,
     ):
         self.image = image
         if format is None:
             if compression_type is None:
                 format = "ASCII"
             else:
@@ -108,14 +111,17 @@
         self.height = height
         if pos_x is None:
             pos_x = 0
         self.pos_x = pos_x
         if pos_y is None:
             pos_y = 0
         self.pos_y = pos_y
+        if rotation is None:
+            rotation = 0
+        self.rotation = rotation
         if complete_zpl is None:
             complete_zpl = True
         self.complete_zpl = complete_zpl
 
     image = property(operator.attrgetter("_image"))
 
     @image.setter
@@ -247,14 +253,34 @@
             raise TypeError(
                 "Y position must be an integer. {param_type} was given.".format(
                     param_type=type(y)
                 )
             )
         self._pos_y = y
 
+    rotation = property(operator.attrgetter("_rotation"))
+
+    @rotation.setter
+    def rotation(self, r):
+        if r is None:
+            raise ValueError("Rotation cannot be empty.")
+        if not isinstance(r, int):
+            raise TypeError(
+                "Rotation must be an integer. {param_type} was given.".format(
+                    param_type=type(r)
+                )
+            )
+        if r not in [0, 90, 180, 270]:
+            raise ValueError(
+                'Rotation must be "0", "90", "180" or "270". {param} was given.'.format(
+                    param=r
+                )
+            )
+        self._rotation = r
+
     complete_zpl = property(operator.attrgetter("_complete_zpl"))
 
     @complete_zpl.setter
     def complete_zpl(self, c):
         if c is None:
             raise ValueError("Complete ZPL cannot be empty.")
         if not isinstance(c, bool):
@@ -284,14 +310,18 @@
         printer or a ZPL graphic field if complete_zpl is not set.
         """
         if isinstance(self._image, bytes):
             pil_image = Image.open(BytesIO(self._image))
         else:
             pil_image = self._image
 
+        # Rotate image based on given parameters
+        if self._rotation:
+            pil_image = pil_image.rotate(self._rotation, expand=False)
+
         # Resize image if width or height defined in parameters
         if self._width or self._height:
             width, height = pil_image.size
             if self._width:
                 width = self._width
             if self._height:
                 height = self._height
```

### Comparing `zebrafy-1.1.1/zebrafy/zebrafy_pdf.py` & `zebrafy-1.1.2/zebrafy/zebrafy_pdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     to ``128``
     :param width: Width of the PDF in the resulting ZPL. If ``0``, use default PDF \
     width, defaults to ``0``
     :param height: Height of the PDF in the resulting ZPL. If ``0``, use default \
     PDF height, defaults to ``0``
     :param pos_x: X position of the PDF on the resulting ZPL, defaults to ``0``
     :param pos_y: Y position of the PDF on the resulting ZPL, defaults to ``0``
+    :param rotation: Additional rotation in degrees ``0``, ``90``, ``180``, or \
+    ``270``, defaults to ``0``
     :param split_pages: Split each PDF page as a new ZPL label  \
     (only applies if complete_zpl is set), defaults to ``False``
     :param complete_zpl: Return a complete ZPL with header and footer included. \
     Otherwise return only the graphic field, defaults to ``True``
 
     .. deprecated:: 1.1.0
         The `compression_type` parameter is deprecated in favor of `format` and will \
@@ -77,14 +79,15 @@
         invert: bool = None,
         dither: bool = None,
         threshold: int = None,
         width: int = None,
         height: int = None,
         pos_x: int = None,
         pos_y: int = None,
+        rotation: int = None,
         split_pages: bool = None,
         complete_zpl: bool = None,
     ):
         self.pdf_bytes = pdf_bytes
         if format is None:
             if compression_type is None:
                 format = "ASCII"
@@ -108,14 +111,17 @@
         self.height = height
         if pos_x is None:
             pos_x = 0
         self.pos_x = pos_x
         if pos_y is None:
             pos_y = 0
         self.pos_y = pos_y
+        if rotation is None:
+            rotation = 0
+        self.rotation = rotation
         if split_pages is None:
             split_pages = False
         self.split_pages = split_pages
         if complete_zpl is None:
             complete_zpl = True
         self.complete_zpl = complete_zpl
 
@@ -251,14 +257,34 @@
             raise TypeError(
                 "Y position must be an integer. {param_type} was given.".format(
                     param_type=type(y)
                 )
             )
         self._pos_y = y
 
+    rotation = property(operator.attrgetter("_rotation"))
+
+    @rotation.setter
+    def rotation(self, r):
+        if r is None:
+            raise ValueError("Rotation cannot be empty.")
+        if not isinstance(r, int):
+            raise TypeError(
+                "Rotation must be an integer. {param_type} was given.".format(
+                    param_type=type(r)
+                )
+            )
+        if r not in [0, 90, 180, 270]:
+            raise ValueError(
+                'Rotation must be "0", "90", "180" or "270". {param} was given.'.format(
+                    param=r
+                )
+            )
+        self._rotation = r
+
     split_pages = property(operator.attrgetter("_split_pages"))
 
     @split_pages.setter
     def split_pages(self, s):
         if s is None:
             raise ValueError("Split pages cannot be empty.")
         if not isinstance(s, bool):
@@ -301,26 +327,27 @@
         :returns: A complete ZPL file string which can be sent to a ZPL compatible \
         printer or a ZPL graphic field if complete_zpl is not set.
         """
         # Open and convert image to grayscale
         pdf = PdfDocument(self._pdf_bytes)
         graphic_fields = []
         for page in pdf:
-            bitmap = page.render(scale=1, rotation=0)
+            bitmap = page.render(scale=1, rotation=self._rotation)
             pil_image = bitmap.to_pil()
             zebrafy_image = ZebrafyImage(
                 pil_image,
                 format=self._format,
                 invert=self._invert,
                 dither=self._dither,
                 threshold=self._threshold,
                 width=self._width,
                 height=self._height,
                 pos_x=self._pos_x,
                 pos_y=self._pos_y,
+                rotation=0,  # Rotation is already handled in the PDF rendering
                 complete_zpl=False,
             )
 
             page_zpl = zebrafy_image.to_zpl() + "\n"
 
             graphic_fields.append(page_zpl)
```

### Comparing `zebrafy-1.1.1/zebrafy/zebrafy_zpl.py` & `zebrafy-1.1.2/zebrafy/zebrafy_zpl.py`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.1/zebrafy.egg-info/PKG-INFO` & `zebrafy-1.1.2/zebrafy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zebrafy
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python library for converting PDF and images to Zebra Programming Language (ZPL)
 Author-email: Miika Nissi <miika@miikanissi.com>
 Maintainer-email: Miika Nissi <miika@miikanissi.com>
 License: LGPLv3
 Project-URL: Homepage, https://github.com/miikanissi/zebrafy/
 Project-URL: Documentation, https://zebrafy.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
@@ -44,17 +44,17 @@
     :target: https://github.com/miikanissi/zebrafy/actions/workflows/ci.yml
     :alt: CI
 
 .. image:: https://readthedocs.org/projects/zebrafy/badge/?version=latest
     :target: https://zebrafy.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/badge/pypi-1.1.1-blue
-    :target: https://pypi.org/project/zebrafy/
-    :alt: PyPi Package
+.. image:: https://img.shields.io/pypi/v/zebrafy
+    :target: https://pypi.org/project/zebrafy
+    :alt: Zebrafy PyPi Package
 
 .. image:: https://img.shields.io/badge/license-LGPLv3-green
     :target: https://www.gnu.org/licenses/lgpl-3.0.en.html#license-text
     :alt: License
 
 **Zebrafy** is a Python 3 library for converting PDF and images to and from
 `Zebra Programming Language (ZPL) <https://en.wikipedia.org/wiki/Zebra_Programming_Language>`_
@@ -88,25 +88,28 @@
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``height``           | Height of the image in the resulting ZPL, ``0`` to use original image/PDF height (default ``0``)             |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``pos_x``            | Pixel x position of the graphic field in resulting ZPL (default ``0``)                                       |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``pos_y``            | Pixel y position of the graphic field in resulting ZPL (default ``0``)                                       |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
+| ``rotation``         | Rotates the image by the specified degree (``0``, ``90``, ``180`` or ``270``, default ``0``)                 |
++----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``complete_zpl``     | Add ZPL header and footer or only get the ZPL graphic field output (``True`` or ``False``, default ``True``) |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 
 Additionally, **ZebrafyPDF** supports the following optional parameters:
 
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | Parameter            | Description                                                                                                  |
 +======================+==============================================================================================================+
 | ``split_pages``      | Split the PDF into separate ZPL labels for each page (``True`` or ``False``, default ``False``)              |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 
+
 Getting Started
 ---------------
 
 Installation
 ^^^^^^^^^^^^
 
 .. code-block:: console
@@ -154,14 +157,15 @@
           invert=True,
           dither=False,
           threshold=128,
           width=720,
           height=1280,
           pos_x=100,
           pos_y=100,
+          rotation=90,
           complete_zpl=True,
       ).to_zpl()
 
   with open("output.zpl", "w") as zpl:
       zpl.write(zpl_string)
 
 Alternatively, **ZebrafyImage** also accepts PIL Image as the image parameter instead of
@@ -191,15 +195,15 @@
   with open("source.pdf", "rb") as pdf:
       zpl_string = ZebrafyPDF(pdf.read()).to_zpl()
 
   with open("output.zpl", "w") as zpl:
       zpl.write(zpl_string)
 
 **ZebrafyPDF** conversion supports the same optional parameters as **ZebrafyImage**
-conversion:
+conversion, with the addition of the ``split_pages`` parameter to split the PDF pages:
 
 .. code-block:: python
 
   from zebrafy import ZebrafyPDF
 
   with open("source.pdf", "rb") as pdf:
       zpl_string = ZebrafyPDF(
@@ -208,15 +212,17 @@
           invert=True,
           dither=False,
           threshold=128,
           width=720,
           height=1280,
           pos_x=100,
           pos_y=100,
+          rotation=90,
           complete_zpl=True,
+          split_pages=True,
       ).to_zpl()
 
   with open("output.zpl", "w") as zpl:
       zpl.write(zpl_string)
 
 ZPL to PDF or Images with **ZebrafyZPL**
 """"""""""""""""""""""""""""""""""""""""
```

