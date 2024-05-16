# Comparing `tmp/flexible_dict-2.0.3.tar.gz` & `tmp/flexible_dict-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexible_dict-2.0.3.tar", last modified: Tue May 14 10:39:12 2024, max compression
+gzip compressed data, was "flexible_dict-2.1.0.tar", last modified: Thu May 16 13:52:56 2024, max compression
```

## Comparing `flexible_dict-2.0.3.tar` & `flexible_dict-2.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:39:12.784003 flexible_dict-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-14 10:39:12.784003 flexible_dict-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      117 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:39:12.784003 flexible_dict-2.0.3/flexible_dict/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/flexible_dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/flexible_dict/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-14 10:39:12.000000 flexible_dict-2.0.3/flexible_dict/_dist_ver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/flexible_dict/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26283 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/flexible_dict/json_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:39:12.784003 flexible_dict-2.0.3/flexible_dict/script/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/flexible_dict/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/flexible_dict/script/class_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/flexible_dict/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/flexible_dict/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:39:12.784003 flexible_dict-2.0.3/flexible_dict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-14 10:39:12.000000 flexible_dict-2.0.3/flexible_dict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-14 10:39:12.000000 flexible_dict-2.0.3/flexible_dict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:39:12.000000 flexible_dict-2.0.3/flexible_dict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 10:39:12.000000 flexible_dict-2.0.3/flexible_dict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/run_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:39:12.784003 flexible_dict-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:52:56.424510 flexible_dict-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-16 13:52:56.424510 flexible_dict-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-16 13:52:51.000000 flexible_dict-2.1.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      117 2024-05-16 13:52:51.000000 flexible_dict-2.1.0/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:52:56.420510 flexible_dict-2.1.0/flexible_dict/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-16 13:52:51.000000 flexible_dict-2.1.0/flexible_dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-16 13:52:51.000000 flexible_dict-2.1.0/flexible_dict/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-16 13:52:56.000000 flexible_dict-2.1.0/flexible_dict/_dist_ver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-16 13:52:51.000000 flexible_dict-2.1.0/flexible_dict/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29652 2024-05-16 13:52:51.000000 flexible_dict-2.1.0/flexible_dict/json_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:52:56.420510 flexible_dict-2.1.0/flexible_dict/script/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 13:52:51.000000 flexible_dict-2.1.0/flexible_dict/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-16 13:52:51.000000 flexible_dict-2.1.0/flexible_dict/script/class_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-16 13:52:51.000000 flexible_dict-2.1.0/flexible_dict/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-16 13:52:51.000000 flexible_dict-2.1.0/flexible_dict/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:52:56.424510 flexible_dict-2.1.0/flexible_dict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-16 13:52:56.000000 flexible_dict-2.1.0/flexible_dict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-16 13:52:56.000000 flexible_dict-2.1.0/flexible_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:52:56.000000 flexible_dict-2.1.0/flexible_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 13:52:56.000000 flexible_dict-2.1.0/flexible_dict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-16 13:52:51.000000 flexible_dict-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 13:52:51.000000 flexible_dict-2.1.0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-05-16 13:52:51.000000 flexible_dict-2.1.0/run_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:52:56.424510 flexible_dict-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-16 13:52:51.000000 flexible_dict-2.1.0/tox.ini
```

### Comparing `flexible_dict-2.0.3/PKG-INFO` & `flexible_dict-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexible_dict
-Version: 2.0.3
+Version: 2.1.0
 Summary: A flexible way to access dict data instead of built-in dict.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/flexible_dict
 Description-Content-Type: text/markdown
 Requires-Dist: dataclasses; python_version < "3.7"
 Requires-Dist: typing_extensions; python_version < "3.8"
```

### Comparing `flexible_dict-2.0.3/README.md` & `flexible_dict-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `flexible_dict-2.0.3/flexible_dict/__main__.py` & `flexible_dict-2.1.0/flexible_dict/__main__.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-2.0.3/flexible_dict/adapter.py` & `flexible_dict-2.1.0/flexible_dict/adapter.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-2.0.3/flexible_dict/json_object.py` & `flexible_dict-2.1.0/flexible_dict/json_object.py`

 * *Files 18% similar despite different names*

```diff
@@ -432,15 +432,16 @@
                 # But deal field here just in case.
                 if isinstance(getattr(cls, field.name, None), Field):
                     if self.is_missing(field.init_default):
                         delattr(cls, name)
                     else:
                         setattr(cls, name, field.init_default)
             else:
-                setattr(cls, name, self.build_property(field))
+                if name in cls.__dict__:
+                    delattr(cls, name)
                 fields[name] = field
 
         # Do we have any Field members that don't also have annotations?
         for name, value in cls.__dict__.items():
             if isinstance(value, Field) and name not in cls_annotations:
                 raise TypeError(f'{name!r} is a field but has no type annotation')
 
@@ -458,15 +459,16 @@
         #
         # self_name is what "self" is called in this function: don't
         # hard-code "self", since that might be a field name.
         if frozen:
             return f'BUILTINS.object.__setattr__({self_name},{name!r},{value})'
         return f'{self_name}.{name}={value}'
 
-    def _init_fn(self, fields: List[Field], self_name: str, d_name='_', ds_name='__', kwargs_name='___'):
+    def _init_fn(self, fields: List[Field], self_name: str, d_name='_', ds_name='__',
+                 k_name='__k', v_name='__v', kwargs_name='___'):
         _locals: dict = {
             'MISSING': MISSING,
             'dict': dict,
         }
         _locals.update((f'_type_{f.name}', f.type) for f in fields)
         _locals.update((f'_key_{f.name}', f.key) for f in fields)
 
@@ -609,18 +611,93 @@
         ))
 
         # if function name is `items`, overwrite method `keys()` and method `values()`
         if func_name == 'items':
             self._set_new_attribute(self.cls, 'keys', self._iter_field_keys_fn('keys', 'self'))
             self._set_new_attribute(self.cls, 'values', self._iter_field_values_fn('values', 'self'))
 
+    def _getattr_fn(self, fields: List[Field], self_name='self', item_name='item', funcs_name='funcs'):
+        funcs = {f.name: self.build_getter(f) for f in fields}
+        _locals = {
+            funcs_name: funcs,
+            'AttributeError': AttributeError,
+        }
+        args = [self_name, item_name]
+        body_lines = [
+            f"if {item_name} in {funcs_name}:",
+            f" return {funcs_name}[{item_name}]({self_name})",
+            f"raise AttributeError()",
+        ]
+        return self._create_fn('__getattr__', args, body_lines, _locals=_locals)
+
+    def add_getattr_func(self):
+        fields = [f for f in self.fields.values() if f._field_type is _FIELD_DICTKEY]
+        self._set_new_attribute(self.cls, '__getattr__', self._getattr_fn(fields))
+
+    def _getattribute_fn(self, fields: List[Field], self_name='self', item_name='item', funcs_name='funcs'):
+        funcs = {f.name: self.build_getter(f) for f in fields}
+        _locals = {
+            funcs_name: funcs,
+        }
+        args = [self_name, item_name]
+        body_lines = [
+            f"if {item_name} in {funcs_name}:",
+            f" return {funcs_name}[{item_name}]({self_name})",
+            f"return super(object, {self_name}).__getattribute__({item_name})",
+        ]
+        return self._create_fn('__getattribute__', args, body_lines, _locals=_locals)
+
+    def add_getattribute_func(self):
+        fields = [f for f in self.fields.values() if f._field_type is _FIELD_DICTKEY]
+        self._set_new_attribute(self.cls, '__getattribute__', self._getattribute_fn(fields))
+
+    def _setattr_fn(self, fields: List[Field], self_name='self', key_name='key',
+                    value_name='value', funcs_name='funcs'):
+        funcs = {f.name: self.build_setter(f) for f in fields}
+        _locals = {
+            funcs_name: funcs,
+        }
+        args = [self_name, key_name, value_name]
+        body_lines = [
+            f"if {key_name} in {funcs_name}:",
+            f" {funcs_name}[{key_name}]({self_name}, {key_name}, {value_name})",
+            f"return super().__setattr__({key_name}, {value_name})",
+        ]
+        return self._create_fn('__setattr__', args, body_lines, _locals=_locals)
+
+    def add_setattr_func(self):
+        fields = [f for f in self.fields.values() if f._field_type is _FIELD_DICTKEY]
+        self._set_new_attribute(self.cls, '__setattr__', self._setattr_fn(fields))
+
+    def _delattr_fn(self, fields: List[Field], self_name='self', item_name='item', funcs_name='funcs'):
+        funcs = {f.name: self.build_deleter(f) for f in fields}
+        _locals = {
+            funcs_name: funcs,
+        }
+        args = [self_name, item_name]
+        body_lines = [
+            f"if {item_name} in {funcs_name}:",
+            f" return {funcs_name}[{item_name}]({self_name}, {item_name})",
+            f"return super().__delattr__({item_name})",
+        ]
+        return self._create_fn('__delattr__', args, body_lines, _locals=_locals)
+
+    def add_delattr_func(self):
+        fields = [f for f in self.fields.values() if f._field_type is _FIELD_DICTKEY]
+        self._set_new_attribute(self.cls, '__delattr__', self._delattr_fn(fields))
+
     def add_class_methods(self):
         """
         add some class methods
         """
+        self.add_getattr_func()
+        # self.add_getattribute_func()
+        self.add_setattr_func()
+        self.add_delattr_func()
+
         if self.config.create_init_func:
             self.add_init_func()
 
         if self.config.create_iter_func:
             self.add_iter_fields_func()
 
     def _process(self):
```

### Comparing `flexible_dict-2.0.3/flexible_dict/script/class_builder.py` & `flexible_dict-2.1.0/flexible_dict/script/class_builder.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-2.0.3/flexible_dict/utils.py` & `flexible_dict-2.1.0/flexible_dict/utils.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-2.0.3/flexible_dict.egg-info/PKG-INFO` & `flexible_dict-2.1.0/flexible_dict.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexible_dict
-Version: 2.0.3
+Version: 2.1.0
 Summary: A flexible way to access dict data instead of built-in dict.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/flexible_dict
 Description-Content-Type: text/markdown
 Requires-Dist: dataclasses; python_version < "3.7"
 Requires-Dist: typing_extensions; python_version < "3.8"
```

### Comparing `flexible_dict-2.0.3/pyproject.toml` & `flexible_dict-2.1.0/pyproject.toml`

 * *Files identical despite different names*

