# Comparing `tmp/jupyterlite_sphinx-0.9.2.tar.gz` & `tmp/jupyterlite_sphinx-0.9.3.tar.gz`

## Comparing `jupyterlite_sphinx-0.9.2.tar` & `jupyterlite_sphinx-0.9.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.2/jupyterlite_sphinx/__init__.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.2/jupyterlite_sphinx/jupyterlite_sphinx.css
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.2/jupyterlite_sphinx/jupyterlite_sphinx.js
--rw-r--r--   0        0        0    14989 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.2/jupyterlite_sphinx/jupyterlite_sphinx.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.2/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.2/LICENSE
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.2/README.md
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.3/jupyterlite_sphinx/__init__.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.3/jupyterlite_sphinx/jupyterlite_sphinx.css
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.3/jupyterlite_sphinx/jupyterlite_sphinx.js
+-rw-r--r--   0        0        0    15005 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.3/jupyterlite_sphinx/jupyterlite_sphinx.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.3/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.3/LICENSE
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.3/README.md
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.3/PKG-INFO
```

### Comparing `jupyterlite_sphinx-0.9.2/jupyterlite_sphinx/jupyterlite_sphinx.css` & `jupyterlite_sphinx-0.9.3/jupyterlite_sphinx/jupyterlite_sphinx.css`

 * *Files identical despite different names*

### Comparing `jupyterlite_sphinx-0.9.2/jupyterlite_sphinx/jupyterlite_sphinx.js` & `jupyterlite_sphinx-0.9.3/jupyterlite_sphinx/jupyterlite_sphinx.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -29,9 +29,13 @@
     params.forEach(param => {
         value = pageParams.get(param);
         if (value !== null) {
             iframeUrl.searchParams.append(param, value);
         }
     });
 
-    return iframeUrl.toString().replace(baseURL, '');
+    if (iframeUrl.searchParams.size) {
+        return `${iframeSrc.split('?')[0]}?${iframeUrl.searchParams.toString()}`;
+    } else {
+        return iframeSrc;
+    }
 }
```

### Comparing `jupyterlite_sphinx-0.9.2/jupyterlite_sphinx/jupyterlite_sphinx.py` & `jupyterlite_sphinx-0.9.3/jupyterlite_sphinx/jupyterlite_sphinx.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         rawsource="",
         *children,
         iframe_src="",
         width="100%",
         height="100%",
         prompt=False,
         prompt_color=None,
-        search_params=[],
+        search_params="false",
         **attributes,
     ):
         super().__init__(
             "",
             iframe_src=iframe_src,
             width=width,
             height=height,
@@ -217,15 +217,15 @@
     def run(self):
         width = self.options.pop("width", "100%")
         height = self.options.pop("height", "100%")
 
         prompt = self.options.pop("prompt", False)
         prompt_color = self.options.pop("prompt_color", None)
 
-        search_params = search_params_parser(self.options.pop("search_params", ""))
+        search_params = search_params_parser(self.options.pop("search_params", False))
 
         prefix = os.path.relpath(
             os.path.join(self.env.app.srcdir, JUPYTERLITE_DIR),
             os.path.dirname(self.get_source_info()[0]),
         )
 
         return [
@@ -258,15 +258,15 @@
     def run(self):
         width = self.options.pop("width", "100%")
         height = self.options.pop("height", "1000px")
 
         prompt = self.options.pop("prompt", False)
         prompt_color = self.options.pop("prompt_color", None)
 
-        search_params = search_params_parser(self.options.pop("search_params", ""))
+        search_params = search_params_parser(self.options.pop("search_params", False))
 
         source_location = os.path.dirname(self.get_source_info()[0])
 
         prefix = os.path.relpath(
             os.path.join(self.env.app.srcdir, JUPYTERLITE_DIR), source_location
         )
 
@@ -500,15 +500,15 @@
 
     app.add_js_file("jupyterlite_sphinx.js")
 
 
 def search_params_parser(search_params: str) -> str:
     pattern = re.compile(r"^\[(?:\s*[\"']{1}([^=\s\,&=\?\/]+)[\"']{1}\s*\,?)+\]$")
     if not search_params:
-        return ""
+        return "false"
     if search_params in ["True", "False"]:
         return search_params.lower()
     elif pattern.match(search_params):
         return search_params.replace('"', "'")
     else:
         raise ValueError(
             'The search_params directive must be either True, False or ["param1", "param2"].\n'
```

### Comparing `jupyterlite_sphinx-0.9.2/LICENSE` & `jupyterlite_sphinx-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlite_sphinx-0.9.2/pyproject.toml` & `jupyterlite_sphinx-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlite_sphinx-0.9.2/PKG-INFO` & `jupyterlite_sphinx-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlite-sphinx
-Version: 0.9.2
+Version: 0.9.3
 Summary: Sphinx extension for deploying JupyterLite
 Author: JupyterLite Contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2022, JupyterLite Contributors
         All rights reserved.
```

