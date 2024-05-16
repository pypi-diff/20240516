# Comparing `tmp/vision_mamba-0.0.5.tar.gz` & `tmp/vision_mamba-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_mamba-0.0.5.tar", max compression
+gzip compressed data, was "vision_mamba-0.0.6.tar", max compression
```

## Comparing `vision_mamba-0.0.5.tar` & `vision_mamba-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2024-01-21 23:06:37.273005 vision_mamba-0.0.5/LICENSE
--rw-r--r--   0        0        0     1767 2024-04-30 03:23:54.672675 vision_mamba-0.0.5/README.md
--rw-r--r--   0        0        0     1364 2024-04-30 03:28:16.769518 vision_mamba-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-30 03:23:54.692729 vision_mamba-0.0.5/vision_mamba/__init__.py
--rw-r--r--   0        0        0     7822 2024-04-30 03:24:57.742893 vision_mamba-0.0.5/vision_mamba/model.py
--rw-r--r--   0        0        0     2487 1970-01-01 00:00:00.000000 vision_mamba-0.0.5/setup.py
--rw-r--r--   0        0        0     2771 1970-01-01 00:00:00.000000 vision_mamba-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-01-21 23:06:37.273005 vision_mamba-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1767 2024-04-30 03:23:54.672675 vision_mamba-0.0.6/README.md
+-rw-r--r--   0        0        0     1365 2024-05-16 17:39:39.505078 vision_mamba-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-30 03:23:54.692729 vision_mamba-0.0.6/vision_mamba/__init__.py
+-rw-r--r--   0        0        0     7903 2024-05-16 17:37:45.826484 vision_mamba-0.0.6/vision_mamba/model.py
+-rw-r--r--   0        0        0     2488 1970-01-01 00:00:00.000000 vision_mamba-0.0.6/setup.py
+-rw-r--r--   0        0        0     2722 1970-01-01 00:00:00.000000 vision_mamba-0.0.6/PKG-INFO
```

### Comparing `vision_mamba-0.0.5/LICENSE` & `vision_mamba-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_mamba-0.0.5/README.md` & `vision_mamba-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `vision_mamba-0.0.5/pyproject.toml` & `vision_mamba-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-mamba"
-version = "0.0.5"
+version = "0.0.6"
 description = "Vision Mamba - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/VisionMamba"
 documentation = "https://github.com/kyegomez/VisionMamba"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/kyegomez/VisionMamba"
@@ -18,15 +18,15 @@
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.9"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 zetascale = "*"
 einops = "*"
 torch = "*"
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.6"
 types-toml = "^0.10.8.1"
```

### Comparing `vision_mamba-0.0.5/vision_mamba/model.py` & `vision_mamba-0.0.6/vision_mamba/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """VisionMambaBlock module."""
 
 import torch
 from einops import rearrange, repeat
 from einops.layers.torch import Rearrange
 from torch import nn, Tensor
 from zeta.nn import SSM
+from einops import reduce
 
 
 # Pair
 def pair(t):
     return t if isinstance(t, tuple) else (t, t)
 
 
@@ -268,10 +269,12 @@
         # Forward pass with the layers
         for layer in self.layers:
             x = layer(x)
             print(f"Layer: {x.shape}")
 
         # Latent
         x = self.to_latent(x)
+        
+        x = reduce(x, "b s d -> b d", "mean")
 
         # Output head with the cls tokens
         return self.output_head(x)
```

### Comparing `vision_mamba-0.0.5/setup.py` & `vision_mamba-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['einops', 'torch', 'zetascale']
 
 setup_kwargs = {
     'name': 'vision-mamba',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'Vision Mamba - Pytorch',
     'long_description': '[![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)\n\n# Vision Mamba\nImplementation of Vision Mamba from the paper: "Vision Mamba: Efficient Visual Representation Learning with Bidirectional State Space Model" It\'s 2.8x faster than DeiT and saves 86.8% GPU memory when performing batch inference to extract features on high-res images. \n\n[PAPER LINK](https://arxiv.org/abs/2401.09417)\n\n## Installation\n\n```bash\npip install vision-mamba\n```\n\n# Usage\n```python\n\nimport torch\nfrom vision_mamba.model import Vim\n\n# Create a random tensor\nx = torch.randn(1, 3, 224, 224)\n\n# Create an instance of the Vim model\nmodel = Vim(\n    dim=256,  # Dimension of the model\n    heads=8,  # Number of attention heads\n    dt_rank=32,  # Rank of the dynamic routing tensor\n    dim_inner=256,  # Inner dimension of the model\n    d_state=256,  # State dimension of the model\n    num_classes=1000,  # Number of output classes\n    image_size=224,  # Size of the input image\n    patch_size=16,  # Size of the image patch\n    channels=3,  # Number of input channels\n    dropout=0.1,  # Dropout rate\n    depth=12,  # Depth of the model\n)\n\n# Perform a forward pass through the model\nout = model(x)\n\n# Print the shape and output of the forward pass\nprint(out.shape)\nprint(out)\n\n\n\n```\n\n\n\n## Citation\n```bibtex\n@misc{zhu2024vision,\n    title={Vision Mamba: Efficient Visual Representation Learning with Bidirectional State Space Model}, \n    author={Lianghui Zhu and Bencheng Liao and Qian Zhang and Xinlong Wang and Wenyu Liu and Xinggang Wang},\n    year={2024},\n    eprint={2401.09417},\n    archivePrefix={arXiv},\n    primaryClass={cs.CV}\n}\n```\n\n# License\nMIT\n\n\n# Todo\n- [ ] Fix the encoder block with the forward and backward convolutions\n- [ ] Make a training script for imagenet',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/VisionMamba',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `vision_mamba-0.0.5/PKG-INFO` & `vision_mamba-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: vision-mamba
-Version: 0.0.5
+Version: 0.0.6
 Summary: Vision Mamba - Pytorch
 Home-page: https://github.com/kyegomez/VisionMamba
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: einops
 Requires-Dist: torch
 Requires-Dist: zetascale
```

