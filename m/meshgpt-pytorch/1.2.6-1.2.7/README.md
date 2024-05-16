# Comparing `tmp/meshgpt_pytorch-1.2.6.tar.gz` & `tmp/meshgpt_pytorch-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshgpt_pytorch-1.2.6.tar", last modified: Tue May 14 23:31:29 2024, max compression
+gzip compressed data, was "meshgpt_pytorch-1.2.7.tar", last modified: Thu May 16 12:38:23 2024, max compression
```

## Comparing `meshgpt_pytorch-1.2.6.tar` & `meshgpt_pytorch-1.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:31:29.065259 meshgpt_pytorch-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-14 23:31:24.000000 meshgpt_pytorch-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-14 23:31:29.065259 meshgpt_pytorch-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9245 2024-05-14 23:31:24.000000 meshgpt_pytorch-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:31:29.061259 meshgpt_pytorch-1.2.6/meshgpt_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-14 23:31:24.000000 meshgpt_pytorch-1.2.6/meshgpt_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-14 23:31:24.000000 meshgpt_pytorch-1.2.6/meshgpt_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    50559 2024-05-14 23:31:24.000000 meshgpt_pytorch-1.2.6/meshgpt_pytorch/meshgpt_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-14 23:31:24.000000 meshgpt_pytorch-1.2.6/meshgpt_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 23:31:24.000000 meshgpt_pytorch-1.2.6/meshgpt_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:31:29.065259 meshgpt_pytorch-1.2.6/meshgpt_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-14 23:31:29.000000 meshgpt_pytorch-1.2.6/meshgpt_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-14 23:31:29.000000 meshgpt_pytorch-1.2.6/meshgpt_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 23:31:29.000000 meshgpt_pytorch-1.2.6/meshgpt_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-14 23:31:29.000000 meshgpt_pytorch-1.2.6/meshgpt_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 23:31:29.000000 meshgpt_pytorch-1.2.6/meshgpt_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 23:31:29.065259 meshgpt_pytorch-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-14 23:31:24.000000 meshgpt_pytorch-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:38:23.008121 meshgpt_pytorch-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-16 12:38:03.000000 meshgpt_pytorch-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-16 12:38:23.008121 meshgpt_pytorch-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-05-16 12:38:03.000000 meshgpt_pytorch-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:38:23.008121 meshgpt_pytorch-1.2.7/meshgpt_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-16 12:38:03.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-16 12:38:03.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50646 2024-05-16 12:38:03.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch/meshgpt_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-16 12:38:03.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 12:38:03.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:38:23.008121 meshgpt_pytorch-1.2.7/meshgpt_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-16 12:38:22.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-16 12:38:23.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:38:22.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-16 12:38:23.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 12:38:23.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:38:23.008121 meshgpt_pytorch-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-16 12:38:03.000000 meshgpt_pytorch-1.2.7/setup.py
```

### Comparing `meshgpt_pytorch-1.2.6/LICENSE` & `meshgpt_pytorch-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.6/PKG-INFO` & `meshgpt_pytorch-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshgpt-pytorch
-Version: 1.2.6
+Version: 1.2.7
 Summary: MeshGPT Pytorch
 Home-page: https://github.com/lucidrains/meshgpt-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,mesh generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshgpt_pytorch-1.2.6/README.md` & `meshgpt_pytorch-1.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 - <a href="https://github.com/qixuema">Quexi Ma</a> for finding numerous bugs with automatic eos handling
 
 - <a href="https://github.com/thuliu-yt16">Yingtian</a> for finding a bug with the gaussian blurring of the positions for spatial label smoothing
 
 - <a href="https://github.com/MarcusLoppe">Marcus</a> yet again for running the experiments to validate that it is possible to extend the system from triangles to <a href="https://github.com/lucidrains/meshgpt-pytorch/issues/54#issuecomment-1906789076">quads</a>
 
+- <a href="https://github.com/MarcusLoppe">Marcus</a> for identifying <a href="https://github.com/lucidrains/meshgpt-pytorch/issues/80">an issue</a> with text conditioning and for running all the experiments that led to it being resolved
+
 ## Install
 
 ```bash
 $ pip install meshgpt-pytorch
 ```
 
 ## Usage
```

#### html2text {}

```diff
@@ -8,54 +8,56 @@
 for making my life easy - _M_a_r_c_u_s for the initial code review (pointing out some
 missing derived features) as well as running the first successful end-to-end
 experiments - _M_a_r_c_u_s for the _f_i_r_s_t_ _s_u_c_c_e_s_s_f_u_l_ _t_r_a_i_n_i_n_g of a collection of
 shapes conditioned on labels - _Q_u_e_x_i_ _M_a for finding numerous bugs with
 automatic eos handling - _Y_i_n_g_t_i_a_n for finding a bug with the gaussian blurring
 of the positions for spatial label smoothing - _M_a_r_c_u_s yet again for running the
 experiments to validate that it is possible to extend the system from triangles
-to _q_u_a_d_s ## Install ```bash $ pip install meshgpt-pytorch ``` ## Usage
-```python import torch from meshgpt_pytorch import ( MeshAutoencoder,
-MeshTransformer ) # autoencoder autoencoder = MeshAutoencoder
-( num_discrete_coors = 128 ) # mock inputs vertices = torch.randn((2, 121, 3))
-# (batch, num vertices, coor (3)) faces = torch.randint(0, 121, (2, 64, 3)) #
-(batch, num faces, vertices (3)) # make sure faces are padded with `-1` for
-variable lengthed meshes # forward in the faces loss = autoencoder( vertices =
-vertices, faces = faces ) loss.backward() # after much training... # you can
-pass in the raw face data above to train a transformer to model this sequence
-of face vertices transformer = MeshTransformer( autoencoder, dim = 512,
-max_seq_len = 768 ) loss = transformer( vertices = vertices, faces = faces )
-loss.backward() # after much training of transformer, you can now sample novel
-3d assets faces_coordinates, face_mask = transformer.generate() # (batch, num
-faces, vertices (3), coordinates (3)), (batch, num faces) # now post process
-for the generated 3d asset ``` For _t_e_x_t_-_c_o_n_d_i_t_i_o_n_e_d_ _3_d_ _s_h_a_p_e_ _s_y_n_t_h_e_s_i_s, simply
-set `condition_on_text = True` on your `MeshTransformer`, and then pass in your
-list of descriptions as the `texts` keyword argument ex. ```python transformer
-= MeshTransformer( autoencoder, dim = 512, max_seq_len = 768, condition_on_text
-= True ) loss = transformer( vertices = vertices, faces = faces, texts = ['a
-high chair', 'a small teapot'], ) loss.backward() # after much training of
-transformer, you can now sample novel 3d assets conditioned on text
-faces_coordinates, face_mask = transformer.generate( texts = ['a long table'],
-cond_scale = 3. # a cond_scale > 1. will enable classifier free guidance - can
-be placed anywhere from 3. - 10. ) ``` If you want to tokenize meshes, for use
-in your multimodal transformer, simply invoke `.tokenize` on your autoencoder
-(or same method on autoencoder trainer instance for the exponentially smoothed
-model) ```python mesh_token_ids = autoencoder.tokenize( vertices = vertices,
-faces = faces ) # (batch, num face vertices, residual quantized layer) ``` ##
-Todo - [x] autoencoder - [x] encoder sageconv with torch geometric - [x] proper
-scatter mean accounting for padding for meaning the vertices and RVQ the
-vertices before gathering back for decoder - [x] complete decoder and
-reconstruction loss + commitment loss - [x] handle variable lengthed faces -
-[x] add option to use residual LFQ, latest quantization development that scales
-code utilization - [x] xcit linear attention in encoder and decoder - [x]
-figure out how to auto-derive `face_edges` directly from faces and vertices -
-[x] embed any derived values (area, angles, etc) from the vertices before sage
-convs - [ ] add an extra graph conv stage in the encoder, where vertices are
-enriched with their connected vertex neighbors, before aggregating into faces.
-make optional - [ ] allow for encoder to noise the vertices, so autoencoder is
-a bit denoising. consider conditioning decoder on noise level, if varying - [ ]
+to _q_u_a_d_s - _M_a_r_c_u_s for identifying _a_n_ _i_s_s_u_e with text conditioning and for
+running all the experiments that led to it being resolved ## Install ```bash $
+pip install meshgpt-pytorch ``` ## Usage ```python import torch from
+meshgpt_pytorch import ( MeshAutoencoder, MeshTransformer ) # autoencoder
+autoencoder = MeshAutoencoder( num_discrete_coors = 128 ) # mock inputs
+vertices = torch.randn((2, 121, 3)) # (batch, num vertices, coor (3)) faces =
+torch.randint(0, 121, (2, 64, 3)) # (batch, num faces, vertices (3)) # make
+sure faces are padded with `-1` for variable lengthed meshes # forward in the
+faces loss = autoencoder( vertices = vertices, faces = faces ) loss.backward()
+# after much training... # you can pass in the raw face data above to train a
+transformer to model this sequence of face vertices transformer =
+MeshTransformer( autoencoder, dim = 512, max_seq_len = 768 ) loss = transformer
+( vertices = vertices, faces = faces ) loss.backward() # after much training of
+transformer, you can now sample novel 3d assets faces_coordinates, face_mask =
+transformer.generate() # (batch, num faces, vertices (3), coordinates (3)),
+(batch, num faces) # now post process for the generated 3d asset ``` For _t_e_x_t_-
+_c_o_n_d_i_t_i_o_n_e_d_ _3_d_ _s_h_a_p_e_ _s_y_n_t_h_e_s_i_s, simply set `condition_on_text = True` on your
+`MeshTransformer`, and then pass in your list of descriptions as the `texts`
+keyword argument ex. ```python transformer = MeshTransformer( autoencoder, dim
+= 512, max_seq_len = 768, condition_on_text = True ) loss = transformer
+( vertices = vertices, faces = faces, texts = ['a high chair', 'a small
+teapot'], ) loss.backward() # after much training of transformer, you can now
+sample novel 3d assets conditioned on text faces_coordinates, face_mask =
+transformer.generate( texts = ['a long table'], cond_scale = 3. # a cond_scale
+> 1. will enable classifier free guidance - can be placed anywhere from 3. -
+10. ) ``` If you want to tokenize meshes, for use in your multimodal
+transformer, simply invoke `.tokenize` on your autoencoder (or same method on
+autoencoder trainer instance for the exponentially smoothed model) ```python
+mesh_token_ids = autoencoder.tokenize( vertices = vertices, faces = faces ) #
+(batch, num face vertices, residual quantized layer) ``` ## Todo - [x]
+autoencoder - [x] encoder sageconv with torch geometric - [x] proper scatter
+mean accounting for padding for meaning the vertices and RVQ the vertices
+before gathering back for decoder - [x] complete decoder and reconstruction
+loss + commitment loss - [x] handle variable lengthed faces - [x] add option to
+use residual LFQ, latest quantization development that scales code utilization
+- [x] xcit linear attention in encoder and decoder - [x] figure out how to
+auto-derive `face_edges` directly from faces and vertices - [x] embed any
+derived values (area, angles, etc) from the vertices before sage convs - [ ]
+add an extra graph conv stage in the encoder, where vertices are enriched with
+their connected vertex neighbors, before aggregating into faces. make optional
+- [ ] allow for encoder to noise the vertices, so autoencoder is a bit
+denoising. consider conditioning decoder on noise level, if varying - [ ]
 transformer - [x] properly mask out eos logit during generation - [x] make sure
 it trains - [x] take care of sos token automatically - [x] take care of eos
 token automatically if sequence length or mask is passed in - [x] handle
 variable lengthed faces - [x] on forwards - [x] on generation, do all eos logic
 + substitute everything after eos with pad id - [x] generation + cache kv - [x]
 trainer wrapper with hf accelerate - [x] autoencoder - take care of ema - [x]
 transformer - [x] text conditioning using own CFG library - [x] complete
```

### Comparing `meshgpt_pytorch-1.2.6/meshgpt_pytorch/data.py` & `meshgpt_pytorch-1.2.7/meshgpt_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.6/meshgpt_pytorch/meshgpt_pytorch.py` & `meshgpt_pytorch-1.2.7/meshgpt_pytorch/meshgpt_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1034,15 +1034,15 @@
         coarse_pre_gateloop_depth = 2,
         fine_pre_gateloop_depth = 2,
         gateloop_use_heinsen = False,
         fine_attn_depth = 2,
         fine_attn_dim_head = 32,
         fine_attn_heads = 8,
         pad_id = -1,
-        num_sos_tokens = 1,
+        num_sos_tokens = None,
         condition_on_text = False,
         text_condition_model_types = ('t5',),
         text_condition_cond_drop_prob = 0.25,
         quads = False,
     ):
         super().__init__()
         self.num_vertices_per_face = 3 if not quads else 4
@@ -1058,14 +1058,15 @@
         self.num_quantizers = autoencoder.num_quantizers
 
         self.eos_token_id = self.codebook_size
 
         # the fine transformer sos token
         # as well as a projection of pooled text embeddings to condition it
 
+        num_sos_tokens = default(num_sos_tokens, 1 if not condition_on_text else 4)
         assert num_sos_tokens > 0
 
         self.num_sos_tokens = num_sos_tokens
         self.sos_token = nn.Parameter(torch.randn(num_sos_tokens, dim))
 
         # they use axial positional embeddings
```

### Comparing `meshgpt_pytorch-1.2.6/meshgpt_pytorch/trainer.py` & `meshgpt_pytorch-1.2.7/meshgpt_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.6/meshgpt_pytorch.egg-info/PKG-INFO` & `meshgpt_pytorch-1.2.7/meshgpt_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshgpt-pytorch
-Version: 1.2.6
+Version: 1.2.7
 Summary: MeshGPT Pytorch
 Home-page: https://github.com/lucidrains/meshgpt-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,mesh generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshgpt_pytorch-1.2.6/setup.py` & `meshgpt_pytorch-1.2.7/setup.py`

 * *Files identical despite different names*

