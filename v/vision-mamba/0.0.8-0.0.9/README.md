# Comparing `tmp/vision_mamba-0.0.8.tar.gz` & `tmp/vision_mamba-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_mamba-0.0.8.tar", max compression
+gzip compressed data, was "vision_mamba-0.0.9.tar", max compression
```

## Comparing `vision_mamba-0.0.8.tar` & `vision_mamba-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2024-01-21 23:06:37.273005 vision_mamba-0.0.8/LICENSE
--rw-r--r--   0        0        0     1825 2024-05-16 18:11:03.814209 vision_mamba-0.0.8/README.md
--rw-r--r--   0        0        0     1365 2024-05-16 18:11:20.793170 vision_mamba-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       54 2024-05-16 18:11:03.794021 vision_mamba-0.0.8/vision_mamba/__init__.py
--rw-r--r--   0        0        0     7949 2024-05-16 18:11:03.794779 vision_mamba-0.0.8/vision_mamba/model.py
--rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 vision_mamba-0.0.8/setup.py
--rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 vision_mamba-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-01-21 23:06:37.273005 vision_mamba-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1825 2024-05-16 18:11:03.814209 vision_mamba-0.0.9/README.md
+-rw-r--r--   0        0        0     1365 2024-05-16 18:11:45.287650 vision_mamba-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-05-16 18:11:03.794021 vision_mamba-0.0.9/vision_mamba/__init__.py
+-rw-r--r--   0        0        0     7949 2024-05-16 18:11:03.794779 vision_mamba-0.0.9/vision_mamba/model.py
+-rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 vision_mamba-0.0.9/setup.py
+-rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 vision_mamba-0.0.9/PKG-INFO
```

### Comparing `vision_mamba-0.0.8/LICENSE` & `vision_mamba-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_mamba-0.0.8/README.md` & `vision_mamba-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `vision_mamba-0.0.8/pyproject.toml` & `vision_mamba-0.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-mamba"
-version = "0.0.8"
+version = "0.0.9"
 description = "Vision Mamba - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/VisionMamba"
 documentation = "https://github.com/kyegomez/VisionMamba"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/kyegomez/VisionMamba"
```

### Comparing `vision_mamba-0.0.8/vision_mamba/model.py` & `vision_mamba-0.0.9/vision_mamba/model.py`

 * *Files identical despite different names*

### Comparing `vision_mamba-0.0.8/setup.py` & `vision_mamba-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['einops', 'torch', 'zetascale']
 
 setup_kwargs = {
     'name': 'vision-mamba',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Vision Mamba - Pytorch',
     'long_description': '[![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)\n\n# Vision Mamba\nImplementation of Vision Mamba from the paper: "Vision Mamba: Efficient Visual Representation Learning with Bidirectional State Space Model" It\'s 2.8x faster than DeiT and saves 86.8% GPU memory when performing batch inference to extract features on high-res images. \n\n[PAPER LINK](https://arxiv.org/abs/2401.09417)\n\n## Installation\n\n```bash\npip install vision-mamba\n```\n\n# Usage\n```python\nimport torch\nfrom vision_mamba import Vim\n\n# Forward pass\nx = torch.randn(1, 3, 224, 224)  # Input tensor with shape (batch_size, channels, height, width)\n\n# Model\nmodel = Vim(\n    dim=256,  # Dimension of the transformer model\n    heads=8,  # Number of attention heads\n    dt_rank=32,  # Rank of the dynamic routing matrix\n    dim_inner=256,  # Inner dimension of the transformer model\n    d_state=256,  # Dimension of the state vector\n    num_classes=1000,  # Number of output classes\n    image_size=224,  # Size of the input image\n    patch_size=16,  # Size of each image patch\n    channels=3,  # Number of input channels\n    dropout=0.1,  # Dropout rate\n    depth=12,  # Depth of the transformer model\n)\n\n# Forward pass\nout = model(x)  # Output tensor from the model\nprint(out.shape)  # Print the shape of the output tensor\nprint(out)  # Print the output tensor\n\n\n\n```\n\n\n\n## Citation\n```bibtex\n@misc{zhu2024vision,\n    title={Vision Mamba: Efficient Visual Representation Learning with Bidirectional State Space Model}, \n    author={Lianghui Zhu and Bencheng Liao and Qian Zhang and Xinlong Wang and Wenyu Liu and Xinggang Wang},\n    year={2024},\n    eprint={2401.09417},\n    archivePrefix={arXiv},\n    primaryClass={cs.CV}\n}\n```\n\n# License\nMIT\n\n\n\n# Todo\n- [ ] Create training script for imagenet\n- [ ] Create a visual mamba for facial recognition',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/VisionMamba',
```

### Comparing `vision_mamba-0.0.8/PKG-INFO` & `vision_mamba-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-mamba
-Version: 0.0.8
+Version: 0.0.9
 Summary: Vision Mamba - Pytorch
 Home-page: https://github.com/kyegomez/VisionMamba
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.10,<4.0
```

