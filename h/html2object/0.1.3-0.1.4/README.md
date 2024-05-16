# Comparing `tmp/html2object-0.1.3.tar.gz` & `tmp/html2object-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2object-0.1.3.tar", last modified: Wed May 15 13:23:12 2024, max compression
+gzip compressed data, was "html2object-0.1.4.tar", last modified: Wed May 15 17:46:48 2024, max compression
```

## Comparing `html2object-0.1.3.tar` & `html2object-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:12.097100 html2object-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 13:23:02.000000 html2object-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-15 13:23:12.097100 html2object-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-15 13:23:02.000000 html2object-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:12.093100 html2object-0.1.3/html2object/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 13:23:02.000000 html2object-0.1.3/html2object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-15 13:23:02.000000 html2object-0.1.3/html2object/html2object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-15 13:23:02.000000 html2object-0.1.3/html2object/html_element.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:12.097100 html2object-0.1.3/html2object.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-15 13:23:12.000000 html2object-0.1.3/html2object.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-15 13:23:12.000000 html2object-0.1.3/html2object.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:23:12.000000 html2object-0.1.3/html2object.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 13:23:12.000000 html2object-0.1.3/html2object.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:23:12.097100 html2object-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-15 13:23:02.000000 html2object-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:12.093100 html2object-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:02.000000 html2object-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-15 13:23:02.000000 html2object-0.1.3/tests/test_html2object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-15 13:23:02.000000 html2object-0.1.3/tests/test_html_element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:46:48.650209 html2object-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 17:46:39.000000 html2object-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-15 17:46:48.650209 html2object-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-15 17:46:39.000000 html2object-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:46:48.650209 html2object-0.1.4/html2object/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 17:46:39.000000 html2object-0.1.4/html2object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-15 17:46:39.000000 html2object-0.1.4/html2object/html2object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-15 17:46:39.000000 html2object-0.1.4/html2object/html_element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:46:48.650209 html2object-0.1.4/html2object.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-15 17:46:48.000000 html2object-0.1.4/html2object.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-15 17:46:48.000000 html2object-0.1.4/html2object.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:46:48.000000 html2object-0.1.4/html2object.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 17:46:48.000000 html2object-0.1.4/html2object.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 17:46:48.650209 html2object-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-15 17:46:39.000000 html2object-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:46:48.650209 html2object-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:46:39.000000 html2object-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-15 17:46:39.000000 html2object-0.1.4/tests/test_html2object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-15 17:46:39.000000 html2object-0.1.4/tests/test_html_element.py
```

### Comparing `html2object-0.1.3/LICENSE` & `html2object-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `html2object-0.1.3/PKG-INFO` & `html2object-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2object
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools to handle the CRUD of .html files as objects.
 Home-page: https://github.com/boterop/html2object
 Author: boterop
 Author-email: boterop22@gmail.com
 Keywords: html,utils,html_utils,html_element,html_parser,html_writer,html_reader,html_crud,html_object,html_file,html_utils.py,html_element.py,html_parser.py,html_writer.py,html_reader.py,html_crud.py,html_object.py,html_file.py,html2object,html2object.py,html2object.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `html2object-0.1.3/README.md` & `html2object-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `html2object-0.1.3/html2object/html2object.py` & `html2object-0.1.4/html2object/html2object.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,33 +7,31 @@
 
 def remove_element(html: str, name: str = "([a-zA-Z][a-zA-Z0-9]*)") -> tuple:
     regex_closed_element_tag = rf"<{name}\b[^\/>]*\/>"
     element = get_element(html, name)
     if re.match(regex_closed_element_tag, element):
         return re.sub(element, "", html, 1)
     children = get_child(html, name=name)
-    return (
-        html.replace(element, "", 1)
-        .replace(children, "", 1)
-        .replace(f"</{name}>", "", 1)
-        .strip()
-    )
+    html = html.replace(element, "", 1)
+    if children:
+        html = html.replace(children, "", 1)
+    return html.replace(f"</{name}>", "", 1).strip()
 
 
 def get_name(html: str) -> str:
     return re.search(r"<([a-zA-Z][a-zA-Z0-9]*)\b", html).group().replace("<", "")
 
 
 def get_attributes(html: str) -> dict:
-    attribs = re.search(r"<([a-zA-Z][a-zA-Z0-9]*)\b([^>]*)>", html)[2].strip()
-    attribs_list = attribs.split(" ")
-    attribs_list = _fix_attrs(attribs_list)
+    attrib = re.search(r"<([a-zA-Z][a-zA-Z0-9]*)\b([^>]*)>", html)[2].strip()
+    attrib_list = attrib.split(" ")
+    attrib_list = _fix_attrs(attrib_list)
     attributes = {}
     last_key = ""
-    for attr in attribs_list:
+    for attr in attrib_list:
         if attr not in ["", "/"]:
             attr_div = attr.strip().split("=", 1)
             key = attr_div[0]
             if len(attr_div) == 1:
                 key = last_key
                 value = f"{attributes[key]} {attr_div[0]}"
             else:
@@ -41,35 +39,40 @@
             last_key = key
             attributes[key] = value
     return attributes
 
 
 def get_child(html: str, *, name: str) -> str:
     element = get_element(html, name=name)
-    if re.match(rf"<{name}\b[^\/>]*\/>", element):
+
+    if re.match(rf"<{name}\b([^>]*)\/>", element):
         return None
-    children = re.findall(rf"<\/?{name}\b[^>]*>", html)
-    children.pop(0)
+    (start_index, end_index) = get_tag_content_index(html, tag_name=name)
+    return html[start_index:end_index].strip()
+
+
+def get_tag_content_index(html: str, *, tag_name: str) -> tuple:
+    (_, start_index) = re.search(rf"<{tag_name}\b[^>]*>", html).span()
+    tags = re.findall(rf"<\/?{tag_name}\b[^>]*>", html)
+    tags.pop(0)
     element_end = 1
     count = 0
-    for element_tag in children:
+    for element_tag in tags:
         if re.match(r"<\/", element_tag):
             element_end -= 1
         else:
             element_end += 1
             count += 1
         if element_end < 1:
             break
-    for _ in range(count):
-        html = re.sub(rf"<\/{name}>", "<remove>", html, 1)
-    (_, start_index) = re.search(rf"<{name}\b[^>]*>", html).span()
-    (end_index, _) = re.search(rf"<\/{name}>", html).span()
-    html = re.sub("<remove>", f"</{name}>", html)
-    end_index = end_index - ((5 - len(name)) * count)
-    return html[start_index:end_index].strip()
+    if count > 0:
+        html = re.sub(rf"<\/{tag_name}>", "<remove>", html, count)
+    (end_index, _) = re.search(rf"<\/{tag_name}>", html).span()
+    end_index = end_index - ((5 - len(tag_name)) * count)
+    return (start_index, end_index)
 
 
 def _fix_attrs(attrs: list) -> list:
     no_splitable = [",", ":", ";"]
     new_list = []
     mix = None
     for attr in attrs:
```

### Comparing `html2object-0.1.3/html2object/html_element.py` & `html2object-0.1.4/html2object/html_element.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,17 @@
             self.children.append(child)
         return self
 
     def set_parent(self, parent: object) -> object:
         self.parent = parent
         return self
 
+    def add_attribute(self, key, value):
+        self.attributes[key] = value
+
     def find_element_by_id(self, id: str, pile: list = None) -> object | None:
         if pile is None:
             pile = []
         if self.id == id:
             return self
         if self.uuid in pile:
             return None
@@ -102,9 +105,9 @@
         if not html:
             return
         try:
             element = html_u.get_element(html)
             name = html_u.get_name(element)
             self.children.append(HtmlElement(html=html, parent=self))
             self._add_children(html_u.remove_element(html, name))
-        except AttributeError as e:
+        except AttributeError:
             self.children.append(html)
```

### Comparing `html2object-0.1.3/html2object.egg-info/PKG-INFO` & `html2object-0.1.4/html2object.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2object
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools to handle the CRUD of .html files as objects.
 Home-page: https://github.com/boterop/html2object
 Author: boterop
 Author-email: boterop22@gmail.com
 Keywords: html,utils,html_utils,html_element,html_parser,html_writer,html_reader,html_crud,html_object,html_file,html_utils.py,html_element.py,html_parser.py,html_writer.py,html_reader.py,html_crud.py,html_object.py,html_file.py,html2object,html2object.py,html2object.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `html2object-0.1.3/setup.py` & `html2object-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="html2object",
-    version="0.1.3",
+    version="0.1.4",
     author="boterop",
     author_email="boterop22@gmail.com",
     description="Tools to handle the CRUD of .html files as objects.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/boterop/html2object",
     packages=find_packages(),
```

### Comparing `html2object-0.1.3/tests/test_html2object.py` & `html2object-0.1.4/tests/test_html2object.py`

 * *Files identical despite different names*

### Comparing `html2object-0.1.3/tests/test_html_element.py` & `html2object-0.1.4/tests/test_html_element.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,23 @@
 
         result = parent.find_element_by_id("child3")
         self.assertEqual(result, child3)
 
         result = parent.find_element_by_id("nonexistent")
         self.assertIsNone(result)
 
+    def test_find_element_by_id_with_real_html(self):
+        parent = HtmlElement(open("tests/assets/index.html").read())
+
+        result = parent.find_element_by_id("info-image")
+        assert result.name == "img"
+        assert result.id == "info-image"
+        assert result.children is None
+        assert result.parent.name == "div"
+
     def test_str(self):
         element = HtmlElement(name="div", id="myDiv", attributes={"class": "container"})
         self.assertEqual(str(element), "<div id=myDiv class=container/>")
 
         element = HtmlElement(name="div")
         element.add_child("Hello, World!")
         self.assertEqual(str(element), "<div>Hello, World!</div>")
```

