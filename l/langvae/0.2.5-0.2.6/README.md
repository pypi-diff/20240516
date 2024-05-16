# Comparing `tmp/langvae-0.2.5.tar.gz` & `tmp/langvae-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langvae-0.2.5.tar", last modified: Wed May 15 07:23:39 2024, max compression
+gzip compressed data, was "langvae-0.2.6.tar", last modified: Thu May 16 13:33:06 2024, max compression
```

## Comparing `langvae-0.2.5.tar` & `langvae-0.2.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.888749 langvae-0.2.5/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)    35149 2023-03-15 12:32:16.000000 langvae-0.2.5/LICENSE
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.888059 langvae-0.2.5/LangVAE.egg-info/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3642 2024-05-15 07:23:39.000000 langvae-0.2.5/LangVAE.egg-info/PKG-INFO
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      857 2024-05-15 07:23:39.000000 langvae-0.2.5/LangVAE.egg-info/SOURCES.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-15 07:23:39.000000 langvae-0.2.5/LangVAE.egg-info/dependency_links.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       34 2024-05-15 07:23:39.000000 langvae-0.2.5/LangVAE.egg-info/requires.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        8 2024-05-15 07:23:39.000000 langvae-0.2.5/LangVAE.egg-info/top_level.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3642 2024-05-15 07:23:39.888419 langvae-0.2.5/PKG-INFO
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2906 2024-05-14 13:36:08.000000 langvae-0.2.5/README.md
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.880791 langvae-0.2.5/langvae/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       62 2024-05-14 12:28:12.000000 langvae-0.2.5/langvae/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.883539 langvae-0.2.5/langvae/arch/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        0 2024-01-26 18:39:44.000000 langvae-0.2.5/langvae/arch/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2687 2024-05-14 12:28:12.000000 langvae-0.2.5/langvae/arch/cvae.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     9372 2024-05-15 00:19:05.000000 langvae-0.2.5/langvae/arch/vae.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.884340 langvae-0.2.5/langvae/data_conversion/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        0 2024-01-12 01:44:56.000000 langvae-0.2.5/langvae/data_conversion/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     6052 2024-05-15 01:16:04.000000 langvae-0.2.5/langvae/data_conversion/tokenization.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.885438 langvae-0.2.5/langvae/decoders/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       94 2024-05-14 12:28:12.000000 langvae-0.2.5/langvae/decoders/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     5246 2024-05-14 12:28:12.000000 langvae-0.2.5/langvae/decoders/sentence.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3614 2024-05-14 12:28:12.000000 langvae-0.2.5/langvae/decoders/sentence_annotated.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.886378 langvae-0.2.5/langvae/encoders/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       94 2024-05-14 12:28:12.000000 langvae-0.2.5/langvae/encoders/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2548 2024-02-08 19:30:25.000000 langvae-0.2.5/langvae/encoders/sentence.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3041 2024-05-14 12:28:12.000000 langvae-0.2.5/langvae/encoders/sentence_annotated.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.886991 langvae-0.2.5/langvae/pipelines/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       52 2024-03-18 10:49:43.000000 langvae-0.2.5/langvae/pipelines/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4668 2024-03-18 10:49:43.000000 langvae-0.2.5/langvae/pipelines/lang_training.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.887704 langvae-0.2.5/langvae/trainers/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      111 2024-03-18 10:49:43.000000 langvae-0.2.5/langvae/trainers/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4055 2024-05-14 12:28:12.000000 langvae-0.2.5/langvae/trainers/cyclical_schedule_kl.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      693 2024-05-15 07:22:19.000000 langvae-0.2.5/pyproject.toml
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       33 2024-05-14 19:59:00.000000 langvae-0.2.5/requirements.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-15 07:23:39.888823 langvae-0.2.5/setup.cfg
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      889 2024-05-15 07:22:19.000000 langvae-0.2.5/setup.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 13:33:06.800272 langvae-0.2.6/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)    35149 2023-03-15 12:32:16.000000 langvae-0.2.6/LICENSE
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 13:33:06.799714 langvae-0.2.6/LangVAE.egg-info/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3642 2024-05-16 13:33:06.000000 langvae-0.2.6/LangVAE.egg-info/PKG-INFO
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      857 2024-05-16 13:33:06.000000 langvae-0.2.6/LangVAE.egg-info/SOURCES.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-16 13:33:06.000000 langvae-0.2.6/LangVAE.egg-info/dependency_links.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       34 2024-05-16 13:33:06.000000 langvae-0.2.6/LangVAE.egg-info/requires.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        8 2024-05-16 13:33:06.000000 langvae-0.2.6/LangVAE.egg-info/top_level.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3642 2024-05-16 13:33:06.800020 langvae-0.2.6/PKG-INFO
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2906 2024-05-14 13:36:08.000000 langvae-0.2.6/README.md
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 13:33:06.793716 langvae-0.2.6/langvae/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       62 2024-05-14 12:28:12.000000 langvae-0.2.6/langvae/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 13:33:06.795922 langvae-0.2.6/langvae/arch/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        0 2024-01-26 18:39:44.000000 langvae-0.2.6/langvae/arch/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4351 2024-05-16 09:06:53.000000 langvae-0.2.6/langvae/arch/cvae.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     9456 2024-05-16 09:06:53.000000 langvae-0.2.6/langvae/arch/vae.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 13:33:06.796353 langvae-0.2.6/langvae/data_conversion/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        0 2024-01-12 01:44:56.000000 langvae-0.2.6/langvae/data_conversion/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     9638 2024-05-16 12:06:43.000000 langvae-0.2.6/langvae/data_conversion/tokenization.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 13:33:06.797356 langvae-0.2.6/langvae/decoders/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       94 2024-05-14 12:28:12.000000 langvae-0.2.6/langvae/decoders/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     7129 2024-05-16 12:31:46.000000 langvae-0.2.6/langvae/decoders/sentence.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     5443 2024-05-16 12:31:53.000000 langvae-0.2.6/langvae/decoders/sentence_annotated.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 13:33:06.798236 langvae-0.2.6/langvae/encoders/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       94 2024-05-14 12:28:12.000000 langvae-0.2.6/langvae/encoders/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4833 2024-05-16 12:31:46.000000 langvae-0.2.6/langvae/encoders/sentence.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     5102 2024-05-16 12:35:53.000000 langvae-0.2.6/langvae/encoders/sentence_annotated.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 13:33:06.798786 langvae-0.2.6/langvae/pipelines/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       52 2024-03-18 10:49:43.000000 langvae-0.2.6/langvae/pipelines/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4668 2024-03-18 10:49:43.000000 langvae-0.2.6/langvae/pipelines/lang_training.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 13:33:06.799341 langvae-0.2.6/langvae/trainers/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      111 2024-03-18 10:49:43.000000 langvae-0.2.6/langvae/trainers/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4055 2024-05-14 12:28:12.000000 langvae-0.2.6/langvae/trainers/cyclical_schedule_kl.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      693 2024-05-16 12:36:39.000000 langvae-0.2.6/pyproject.toml
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       33 2024-05-14 19:59:00.000000 langvae-0.2.6/requirements.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-16 13:33:06.800330 langvae-0.2.6/setup.cfg
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      889 2024-05-16 12:36:20.000000 langvae-0.2.6/setup.py
```

### Comparing `langvae-0.2.5/LICENSE` & `langvae-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `langvae-0.2.5/LangVAE.egg-info/PKG-INFO` & `langvae-0.2.6/LangVAE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langvae
-Version: 0.2.5
+Version: 0.2.6
 Summary: LangVAE: Large Language VAEs made simple
 Home-page: 
 Author: Danilo S. Carvalho
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>
 Project-URL: Homepage, https://github.com/neuro-symbolic-ai/LangVAE
 Project-URL: Issues, https://github.com/neuro-symbolic-ai/LangVAE/issues
 Keywords: vae,llm,generative,nlp
```

### Comparing `langvae-0.2.5/LangVAE.egg-info/SOURCES.txt` & `langvae-0.2.6/LangVAE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langvae-0.2.5/PKG-INFO` & `langvae-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langvae
-Version: 0.2.5
+Version: 0.2.6
 Summary: LangVAE: Large Language VAEs made simple
 Home-page: 
 Author: Danilo S. Carvalho
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>
 Project-URL: Homepage, https://github.com/neuro-symbolic-ai/LangVAE
 Project-URL: Issues, https://github.com/neuro-symbolic-ai/LangVAE/issues
 Keywords: vae,llm,generative,nlp
```

### Comparing `langvae-0.2.5/README.md` & `langvae-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `langvae-0.2.5/langvae/arch/cvae.py` & `langvae-0.2.6/langvae/arch/cvae.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,62 +7,103 @@
 from pythae.models.vae import VAEConfig
 from langvae.arch.vae import LangVAE
 from langvae.encoders import AnnotatedSentenceEncoder
 from langvae.decoders import SentenceDecoder
 
 
 class LangCVAE(LangVAE):
+    """
+    A subclass of LangVAE implementing a Conditional Variational Autoencoder (CVAE).
+    This model extends LangVAE by incorporating conditional variables into the latent space, allowing for
+    controlled text generation based on specified input annotations.
+
+    Attributes:
+        emb2z (nn.Linear): A linear transformation layer used to project encoded annotations into the latent space.
+
+    Args:
+        model_config (VAEConfig): Configuration settings for the VAE model.
+        encoder (Optional[AnnotatedSentenceEncoder]): Language encoder model that processes input data and returns sentence embeddings.
+        decoder (Optional[SentenceDecoder]): The decoder that generates text from latent representations.
+    """
     def __init__(
             self,
             model_config: VAEConfig,
             encoder: Optional[AnnotatedSentenceEncoder],
             decoder: Optional[SentenceDecoder]
     ):
         decoder = type(decoder)(decoder.decoder.config.name_or_path,
-                                encoder.encoder.config.hidden_size * (encoder.num_annotations + 1),
+                                model_config.latent_dim * 2 * encoder.num_annotations,
                                 decoder.max_len,
                                 decoder.device,
                                 decoder.load_in_4bit,
                                 decoder.device_map,
                                 decoder.max_look_behind)
         decoder.debug = True
         super().__init__(model_config=model_config, encoder=encoder, decoder=decoder)
-        self.z2emb = nn.Linear(model_config.latent_dim, encoder.encoder.config.hidden_size, device=self.device)
+        self.emb2z = nn.Linear(encoder.encoder.config.hidden_size, model_config.latent_dim, device=self.device)
 
     def forward(self, inputs: BaseDataset, **kwargs):
+        """
+        Defines the forward pass of the LangCVAE model.
+
+        Args:
+            inputs (BaseDataset): The input dataset entries containing text data and conditional variables.
+
+        Returns:
+            ModelOutput: A structured output containing loss values, reconstructed data, and latent variables.
+        """
         x = inputs["data"]
 
         encoder_output = self.encoder(x)
         mu, log_var = encoder_output.embedding, encoder_output.log_covariance
         std = torch.exp(0.5 * log_var)
         z, eps = self._sample_gauss(mu, std)
         cond_vars = encoder_output["embedding_lbls"]
-        recon_x = self.decoder(torch.cat([torch.cat((self.z2emb(z), cvar), dim=-1) for cvar in cond_vars], dim=-1))["reconstruction"]
+        recon_x = self.decoder(torch.cat([torch.cat((z, self.emb2z(cvar)), dim=-1) for cvar in cond_vars], dim=-1))["reconstruction"]
 
         loss, recon_loss, kld = self.loss_function(recon_x, x, mu, log_var, z)
 
         output = ModelOutput(
             recon_loss=recon_loss,
             reg_loss=kld,
             loss=loss,
             recon_x=recon_x,
             z=z,
         )
 
         return output
 
     def encode_z(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+        """
+        Encodes input data into latent variables and conditional variables.
+
+        Args:
+            x (Tensor): Input tensor to be encoded.
+
+        Returns:
+            Tuple[Tensor, Tensor]: A tuple containing the latent variables and conditional variables.
+        """
         encoded = self.encoder(x)
         mu, log_var = encoded["embedding"], encoded["log_covariance"]
         cond_vars = encoded["embedding_lbls"]
         std = torch.exp(0.5 * log_var)
         z, eps = self._sample_gauss(mu, std)
 
         return z, cond_vars
 
     def decode_sentences(self, z: Tensor, cond_vars: Sequence[Tensor]) -> List[str]:
-        cond_z = torch.cat([torch.cat((self.z2emb(z), cvar), dim=-1) for cvar in cond_vars], dim=-1)
+        """
+        Decodes latent and conditional variables into sentences.
+
+        Args:
+            z (Tensor): Latent variables.
+            cond_vars (Sequence[Tensor]): Conditional variables associated with the latent variables.
+
+        Returns:
+            List[str]: A list of generated sentences.
+        """
+        cond_z = torch.cat([torch.cat((z, self.emb2z(cvar)), dim=-1) for cvar in cond_vars], dim=-1)
         generated = self.decoder(cond_z)["reconstruction"]
         sents = self.decoder.tokenizer.batch_decode(torch.argmax(generated, dim=-1), skip_special_tokens=True)
 
         return sents
```

### Comparing `langvae-0.2.5/langvae/arch/vae.py` & `langvae-0.2.6/langvae/arch/vae.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,16 +95,16 @@
 
 class LangVAE(VAE):
     """
     A language-oriented Variational Autoencoder (VAE) that can be used for text generation.
 
     Args:
         model_config (VAEConfig): The configuration of the VAE model.
-        encoder (Optional[BaseEncoder]): Language encoder model to be used.
-        decoder (Optional[BaseDecoder]): Language decoder model to be used.
+        encoder (Optional[BaseEncoder]): Language encoder model that processes input data and returns sentence embeddings.
+        decoder (Optional[BaseDecoder]): Language decoder model that generates text from latent representations.
     """
 
     def __init__(
             self,
             model_config: VAEConfig,
             encoder: Optional[BaseEncoder],
             decoder: Optional[BaseDecoder]
```

### Comparing `langvae-0.2.5/langvae/decoders/sentence.py` & `langvae-0.2.6/langvae/decoders/sentence.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,32 @@
 from torch import nn, Tensor
 from transformers import AutoTokenizer, AutoModelForCausalLM, PreTrainedModel
 from pythae.models.nn import BaseDecoder
 from pythae.models.base.base_utils import ModelOutput
 
 
 class SentenceDecoder(BaseDecoder):
+    """
+    Decoder class for generating sentences from latent representations.
+
+    This decoder uses a pre-trained causal language model to generate text from latent representations.
+    It outputs token probability distribution tensors (B x S x V), where :math:`B` is the batch size, :math:`S`
+    is the maximum sentence length and :math:`V` is the decoder vocabulary size.
+
+    Attributes:
+        model_path (str): Path/locator to the pre-trained language model.
+        latent_size (int): Size of the latent space.
+        max_len (int): Maximum length (in tokens) of the generated sentences.
+        device (torch.device): Device on which the model and data are allocated (e.g., 'cpu', 'cuda').
+        load_in_4bit (bool): Flag indicating whether to load the model in 4-bit quantisation mode for memory efficiency.
+        device_map (str): Device map configuration for model parallelism.
+        max_look_behind (int): Maximum number of tokens to look behind for context in generation.
+        args (ModelConfig, optional): Additional configuration arguments.
+    """
+
     def __init__(self, model_path: str,
                  latent_size: int,
                  max_len: int,
                  device: torch.device = "cpu",
                  load_in_4bit: bool = False,
                  device_map: str = None,
                  max_look_behind: int = 20,
@@ -20,14 +38,17 @@
             self.decoder = AutoModelForCausalLM.from_pretrained(model_path, load_in_4bit=load_in_4bit,
                                                                 torch_dtype="auto", device_map=device_map)
         else:
             self.decoder = AutoModelForCausalLM.from_pretrained(model_path, load_in_4bit=load_in_4bit, torch_dtype="auto")
             if (not load_in_4bit):
                 self.decoder = self.decoder.to(device)
 
+        self.decoder.eval()
+        self.decoder.requires_grad_(False)
+
         self.load_in_4bit = load_in_4bit
         self.tokenizer = AutoTokenizer.from_pretrained(model_path, padding_side="left", add_prefix_space=True)
         self.tokenizer.pad_token = self.tokenizer.eos_token
         self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
         self.max_len = max_len
         self.device_map = device_map
         self.max_look_behind = max_look_behind
@@ -35,28 +56,44 @@
         embedding_dim = self.decoder.get_input_embeddings().embedding_dim
 
         dec_ids = torch.unsqueeze(torch.tensor([self.tokenizer.pad_token_id] * 2, dtype=torch.int64, device=self.device), dim=-1)
         pkv = self.decoder(dec_ids).past_key_values
         self.pkv_dims = pkv[0][0].shape[1:]
         self.pkv_dtype = pkv[0][0].dtype
 
+        print("pkv_dims:", self.pkv_dims)
+        print("num_hidden_layers:", self.decoder.config.num_hidden_layers)
+        print("hidden_size:", self.decoder.config.hidden_size)
+        print("latent_size:", latent_size)
+
         self.context_embedder = nn.Linear(latent_size, max_len * embedding_dim, dtype=self.pkv_dtype, device=self.device)
         self.context_hidden = nn.Linear(
             latent_size,
-            self.decoder.config.hidden_size * self.decoder.config.num_hidden_layers * 2, # self.pkv_dims[0] * self.pkv_dims[1] * self.pkv_dims[2] == self.decoder.config.hidden_size
+            self.pkv_dims[0] * self.pkv_dims[1] * self.pkv_dims[2] * self.decoder.config.num_hidden_layers * 2, # self.pkv_dims[0] * self.pkv_dims[1] * self.pkv_dims[2] == self.decoder.config.hidden_size
             dtype=self.pkv_dtype,
             device=self.device
         )
         self.dropout = nn.Dropout(p=0.4)
 
         self.decoder.eval()
         self.dbg_counter = 0
         self.debug = False
 
     def forward(self, z: Tensor) -> ModelOutput:
+        """
+        Processes the input latent tensor through the decoder to generate sentences.
+
+        Args:
+            z (Tensor): Input tensor containing latent representations.
+
+        Returns:
+            ModelOutput: The generated sentences as a ModelOutput object: token probability distribution
+            tensors (B x S x V), where :math:`B` is the batch size, :math:`S is the maximum sentence length and
+            :math:`V` is the decoder vocabulary size.
+        """
         # Fix for pythae device allocation bug
         if (not self.load_in_4bit):
             self.decoder = self.decoder.to(self.device)
         else:
             self.device = self.decoder.device
         self.context_hidden = self.context_hidden.to(self.device)
         self.context_embedder = self.context_embedder.to(self.device)
```

### Comparing `langvae-0.2.5/langvae/decoders/sentence_annotated.py` & `langvae-0.2.6/langvae/decoders/sentence_annotated.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,27 +3,59 @@
 from torch import nn, Tensor
 from transformers import AutoTokenizer, AutoModelForCausalLM, PreTrainedModel
 from pythae.models.base.base_utils import ModelOutput
 from .sentence import SentenceDecoder
 
 
 class AnnotatedSentenceDecoder(SentenceDecoder):
+    """
+    Decoder class for generating sentences from latent representations.
+
+    Extends :class:`~langvae.decoders.SentenceDecoder` to allow generation of token annotations alongside tokens.
+    Annotation tokens are specified by the input data, which should contain mappings (decoder tokens -> labels).
+    It outputs token probability distribution tensors (B x S x A·V), where :math:`B` is the batch size, :math:`S`
+    is the maximum sentence length, :math:`A` is the number of annotations and :math:`V` is the decoder vocabulary size.
+
+    Attributes:
+        model_path (str): Path/locator to the pre-trained language model.
+        latent_size (int): Size of the latent space.
+        num_annotations (int): Number of annotations.
+        max_len (int): Maximum length (in tokens) of the generated sentences.
+        device (torch.device): Device on which the model and data are allocated (e.g., 'cpu', 'cuda').
+        load_in_4bit (bool): Flag indicating whether to load the model in 4-bit quantisation mode for memory efficiency.
+        device_map (str): Device map configuration for model parallelism.
+        max_look_behind (int): Maximum number of tokens to look behind for context in generation.
+        args (ModelConfig, optional): Additional configuration arguments.
+    """
+
     def __init__(self, model_path: str,
                  latent_size: int,
                  max_len: int,
                  num_annotations: int,
                  device: str = "cpu",
                  load_in_4bit: bool = False,
                  device_map: str = None,
                  max_look_behind: int = 20,
                  args=None):  # Args is a ModelConfig instance
         super().__init__(model_path, latent_size, max_len, device, load_in_4bit, device_map, max_look_behind, args)
         self.num_annotations = num_annotations
 
     def forward(self, z: Tensor) -> ModelOutput:
+        """
+        Processes the input latent tensor through the decoder to generate sentences.
+
+        Args:
+            z (Tensor): Input tensor containing latent representations.
+
+        Returns:
+            ModelOutput: The generated sentences as a ModelOutput object: token probability distribution
+            tensors (B x S x A·V), where :math:`B` is the batch size, :math:`S` is the maximum sentence length,
+            :math:`A` is the number of annotations and :math:`V` is the decoder vocabulary size.
+        """
+
         # Fix for pythae device allocation bug
         if (not self.load_in_4bit):
             self.decoder = self.decoder.to(self.device)
         else:
             self.device = self.decoder.device
         self.context_hidden = self.context_hidden.to(self.device)
         self.context_embedder = self.context_embedder.to(self.device)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `langvae-0.2.5/langvae/pipelines/lang_training.py` & `langvae-0.2.6/langvae/pipelines/lang_training.py`

 * *Files identical despite different names*

### Comparing `langvae-0.2.5/langvae/trainers/cyclical_schedule_kl.py` & `langvae-0.2.6/langvae/trainers/cyclical_schedule_kl.py`

 * *Files identical despite different names*

### Comparing `langvae-0.2.5/pyproject.toml` & `langvae-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "langvae"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Danilo S. Carvalho", email="danilo.carvalho@manchester.ac.uk" }
 ]
 description = "LangVAE: Large Language VAEs made simple"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `langvae-0.2.5/setup.py` & `langvae-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     install_requires = [str(x).strip() for x in all_reqs]
 
     return install_requires
 
 
 setup(
     name='LangVAE',
-    version='0.2.5',
+    version='0.2.6',
     packages=[
         'langvae',
         'langvae.arch',
         'langvae.decoders',
         'langvae.encoders',
         'langvae.data_conversion',
         'langvae.pipelines',
```

