# Comparing `tmp/statedict2pytree-0.2.0.tar.gz` & `tmp/statedict2pytree-0.3.0.tar.gz`

## Comparing `statedict2pytree-0.2.0.tar` & `statedict2pytree-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    50334 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/package-lock.json
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/package.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/tailwind.config.js
--rw-r--r--   0        0        0   336449 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/torch2jax.png
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/examples/convert_resnet.py
--rw-r--r--   0        0        0    97404 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/examples/doggo.jpeg
--rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/examples/resnet.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/examples/test_resnet_inference.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/statedict2pytree/__init__.py
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/statedict2pytree/statedict2pytree.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/statedict2pytree/static/input.css
--rw-r--r--   0        0        0    40813 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/statedict2pytree/static/output.css
--rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/statedict2pytree/templates/index.html
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/.gitignore
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/README.md
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 statedict2pytree-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    50334 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/package-lock.json
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/package.json
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/pyrightconfig.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/tailwind.config.js
+-rw-r--r--   0        0        0   336449 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/torch2jax.png
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/examples/convert_resnet.py
+-rw-r--r--   0        0        0    97404 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/examples/doggo.jpeg
+-rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/examples/resnet.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/examples/test_resnet_inference.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/statedict2pytree/__init__.py
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/statedict2pytree/statedict2pytree.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/statedict2pytree/static/input.css
+-rw-r--r--   0        0        0    40813 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/statedict2pytree/static/output.css
+-rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/statedict2pytree/templates/index.html
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/tests/test_conv.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/tests/test_linear.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/.gitignore
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/README.md
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/PKG-INFO
```

### Comparing `statedict2pytree-0.2.0/package-lock.json` & `statedict2pytree-0.3.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.2.0/torch2jax.png` & `statedict2pytree-0.3.0/torch2jax.png`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.2.0/examples/doggo.jpeg` & `statedict2pytree-0.3.0/examples/doggo.jpeg`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.2.0/examples/resnet.py` & `statedict2pytree-0.3.0/examples/resnet.py`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.2.0/examples/test_resnet_inference.py` & `statedict2pytree-0.3.0/examples/test_resnet_inference.py`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.2.0/statedict2pytree/statedict2pytree.py` & `statedict2pytree-0.3.0/statedict2pytree/statedict2pytree.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import functools as ft
 import re
 
 import equinox as eqx
 import flask
 import jax
+import numpy as np
 from beartype.typing import Optional
 from jaxtyping import PyTree
 from loguru import logger
 from penzai import pz
 from pydantic import BaseModel
 
 
@@ -27,14 +28,21 @@
     type: str
 
 
 PYTREE: Optional[PyTree] = None
 STATE_DICT: Optional[dict] = None
 
 
+def can_reshape(shape1, shape2):
+    product1 = np.prod(shape1)
+    product2 = np.prod(shape2)
+
+    return product1 == product2
+
+
 def get_node(
     tree: PyTree, targets: list[str], log_when_not_found: bool = False
 ) -> PyTree | None:
     if len(targets) == 0 or tree is None:
         return tree
     else:
         next_target: str = targets[0]
@@ -142,40 +150,46 @@
     return flask.render_template(
         "index.html",
         pytree_fields=pytree_fields,
         torch_fields=state_dict_to_fields(STATE_DICT),
     )
 
 
+def autoconvert(pytree: PyTree, state_dict: dict) -> tuple[PyTree, eqx.nn.State]:
+    jax_fields = pytree_to_fields(pytree)
+    torch_fields = state_dict_to_fields(state_dict)
+    return convert(jax_fields, torch_fields, pytree, state_dict)
+
+
 def convert(
     jax_fields: list[JaxField],
     torch_fields: list[TorchField],
     pytree: PyTree,
     state_dict: dict,
-):
+) -> tuple[PyTree, eqx.nn.State]:
     identity = lambda *args, **kwargs: pytree
     model, state = eqx.nn.make_with_state(identity)()
     state_paths: list[tuple[JaxField, TorchField]] = []
     for jax_field, torch_field in zip(jax_fields, torch_fields):
-        if jax_field.shape != torch_field.shape:
+        if not can_reshape(jax_field.shape, torch_field.shape):
             raise ValueError(
                 "Fields have incompatible shapes!"
                 f"{jax_field.shape=} != {torch_field.shape=}"
             )
         path = jax_field.path.split(".")[1:]
         if "StateIndex" in jax_field.type:
             state_paths.append((jax_field, torch_field))
 
         else:
             where = ft.partial(get_node, targets=path)
             if where(model) is not None:
                 model = eqx.tree_at(
                     where,
                     model,
-                    state_dict[torch_field.path],
+                    state_dict[torch_field.path].reshape(jax_field.shape),
                 )
     result: dict[str, list[TorchField]] = {}
     for tuple_item in state_paths:
         path_prefix = tuple_item[0].path.split(".")[1:-1]
         prefix_key = ".".join(path_prefix)
         if prefix_key not in result:
             result[prefix_key] = []
```

### Comparing `statedict2pytree-0.2.0/statedict2pytree/static/output.css` & `statedict2pytree-0.3.0/statedict2pytree/static/output.css`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.2.0/statedict2pytree/templates/index.html` & `statedict2pytree-0.3.0/statedict2pytree/templates/index.html`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.2.0/.gitignore` & `statedict2pytree-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.2.0/README.md` & `statedict2pytree-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
 The goal of this package is to simplify the conversion from PyTorch models into JAX PyTrees (which can be used e.g. in Equinox). The way this works is by putting both models side my side and aligning the weights in the right order. Then, all statedict2pytree is doing, is iterating over both lists and matching the weight matrices.
 
 Usually, if you _declared the fields in the same order as in the PyTorch model_, you don't have to rearrange anything -- but the option is there if you need it.
 
 (Theoretically, you can rearrange the model in any way you like - e.g. last layer as the first layer - as long as the shapes match!)
 
+## Shape Matching? What's that?
+
+Currently, there is no sophisticated shape matching in place. Two matrices are considered "matching" if the product of their shape match. For example:
+
+1. (8, 1, 1) and (8, ) match, because (8 _ 1 _ 1 = 8)
+
 ## Get Started
 
 ### Installation
 
 Run
 
 ```bash
@@ -96,7 +102,22 @@
     pytree: PyTree,
     state_dict: dict,
 ):
 ...
 ```
 
 If your models already have the right "order", then you might as well use this function directly. Note that the lists `jax_fields` and `torch_fields` must have the same length and each matching entry must have the same shape!
+
+For the full, automatic experience, use `autoconvert`:
+
+```python
+import statedict2pytree as s2p
+
+my_model = Model(...)
+state_dict = ...
+
+model, state = s2p.autoconvert(my_model, state_dict)
+
+```
+
+This will however only work if your PyTree fields have been declared
+in the same order as they appear in the state dict!
```

### Comparing `statedict2pytree-0.2.0/pyproject.toml` & `statedict2pytree-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "statedict2pytree"
-version = "0.2.0"
+version = "0.3.0"
 description = "Converts torch models into PyTrees for Equinox"
 readme = "README.md"
 requires-python = "~=3.10"
 authors = [{ name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev" }]
 dependencies = [
     "jax",
     "equinox>=0.11.4",
@@ -12,15 +12,15 @@
     "beartype",
     "typing_extensions",
     "loguru",
     "jaxtyping",
     "torch",
     "flask",
     "pydantic",
-    "penzai"
+    "penzai",
 ]
 [project.optional-dependencies]
 dev = ["nox", "pre-commit", "pytest", "mkdocs"]
 
 [tool.ruff]
 extend-include = ["*.ipynb"]
 src = []
```

### Comparing `statedict2pytree-0.2.0/PKG-INFO` & `statedict2pytree-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: statedict2pytree
-Version: 0.2.0
+Version: 0.3.0
 Summary: Converts torch models into PyTrees for Equinox
 Author-email: "Artur A. Galstyan" <mail@arturgalstyan.dev>
 Requires-Python: ~=3.10
 Requires-Dist: beartype
 Requires-Dist: equinox>=0.11.4
 Requires-Dist: flask
 Requires-Dist: jax
@@ -28,14 +28,20 @@
 
 The goal of this package is to simplify the conversion from PyTorch models into JAX PyTrees (which can be used e.g. in Equinox). The way this works is by putting both models side my side and aligning the weights in the right order. Then, all statedict2pytree is doing, is iterating over both lists and matching the weight matrices.
 
 Usually, if you _declared the fields in the same order as in the PyTorch model_, you don't have to rearrange anything -- but the option is there if you need it.
 
 (Theoretically, you can rearrange the model in any way you like - e.g. last layer as the first layer - as long as the shapes match!)
 
+## Shape Matching? What's that?
+
+Currently, there is no sophisticated shape matching in place. Two matrices are considered "matching" if the product of their shape match. For example:
+
+1. (8, 1, 1) and (8, ) match, because (8 _ 1 _ 1 = 8)
+
 ## Get Started
 
 ### Installation
 
 Run
 
 ```bash
@@ -120,7 +126,22 @@
     pytree: PyTree,
     state_dict: dict,
 ):
 ...
 ```
 
 If your models already have the right "order", then you might as well use this function directly. Note that the lists `jax_fields` and `torch_fields` must have the same length and each matching entry must have the same shape!
+
+For the full, automatic experience, use `autoconvert`:
+
+```python
+import statedict2pytree as s2p
+
+my_model = Model(...)
+state_dict = ...
+
+model, state = s2p.autoconvert(my_model, state_dict)
+
+```
+
+This will however only work if your PyTree fields have been declared
+in the same order as they appear in the state dict!
```

