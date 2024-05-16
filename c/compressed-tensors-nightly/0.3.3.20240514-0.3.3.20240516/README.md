# Comparing `tmp/compressed_tensors_nightly-0.3.3.20240514-py3-none-any.whl.zip` & `tmp/compressed_tensors_nightly-0.3.3.20240516-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,44 +1,45 @@
-Zip file size: 58586 bytes, number of entries: 42
--rw-r--r--  2.0 unx      789 b- defN 24-May-14 15:27 compressed_tensors/__init__.py
--rw-r--r--  2.0 unx      755 b- defN 24-May-14 15:27 compressed_tensors/base.py
--rw-r--r--  2.0 unx     1512 b- defN 24-May-14 15:27 compressed_tensors/version.py
--rw-r--r--  2.0 unx      935 b- defN 24-May-14 15:27 compressed_tensors/compressors/__init__.py
--rw-r--r--  2.0 unx     2061 b- defN 24-May-14 15:27 compressed_tensors/compressors/base.py
--rw-r--r--  2.0 unx     1257 b- defN 24-May-14 15:27 compressed_tensors/compressors/dense.py
--rw-r--r--  2.0 unx     5403 b- defN 24-May-14 15:27 compressed_tensors/compressors/helpers.py
--rw-r--r--  2.0 unx     4023 b- defN 24-May-14 15:27 compressed_tensors/compressors/int_quantized.py
--rw-r--r--  2.0 unx    10426 b- defN 24-May-14 15:27 compressed_tensors/compressors/model_compressor.py
--rw-r--r--  2.0 unx     8632 b- defN 24-May-14 15:27 compressed_tensors/compressors/sparse_bitmask.py
--rw-r--r--  2.0 unx      704 b- defN 24-May-14 15:27 compressed_tensors/config/__init__.py
--rw-r--r--  2.0 unx     1416 b- defN 24-May-14 15:27 compressed_tensors/config/base.py
--rw-r--r--  2.0 unx     1317 b- defN 24-May-14 15:27 compressed_tensors/config/dense.py
--rw-r--r--  2.0 unx     1308 b- defN 24-May-14 15:27 compressed_tensors/config/sparse_bitmask.py
--rw-r--r--  2.0 unx      760 b- defN 24-May-14 15:27 compressed_tensors/quantization/__init__.py
--rw-r--r--  2.0 unx     4360 b- defN 24-May-14 15:27 compressed_tensors/quantization/quant_args.py
--rw-r--r--  2.0 unx     8042 b- defN 24-May-14 15:27 compressed_tensors/quantization/quant_config.py
--rw-r--r--  2.0 unx     1480 b- defN 24-May-14 15:27 compressed_tensors/quantization/quant_scheme.py
--rw-r--r--  2.0 unx      798 b- defN 24-May-14 15:27 compressed_tensors/quantization/lifecycle/__init__.py
--rw-r--r--  2.0 unx     7573 b- defN 24-May-14 15:27 compressed_tensors/quantization/lifecycle/apply.py
--rw-r--r--  2.0 unx     1776 b- defN 24-May-14 15:27 compressed_tensors/quantization/lifecycle/calibration.py
--rw-r--r--  2.0 unx     2247 b- defN 24-May-14 15:27 compressed_tensors/quantization/lifecycle/compressed.py
--rw-r--r--  2.0 unx    11267 b- defN 24-May-14 15:27 compressed_tensors/quantization/lifecycle/forward.py
--rw-r--r--  2.0 unx     1726 b- defN 24-May-14 15:27 compressed_tensors/quantization/lifecycle/frozen.py
--rw-r--r--  2.0 unx     3697 b- defN 24-May-14 15:27 compressed_tensors/quantization/lifecycle/initialize.py
--rw-r--r--  2.0 unx      745 b- defN 24-May-14 15:27 compressed_tensors/quantization/observers/__init__.py
--rw-r--r--  2.0 unx     5156 b- defN 24-May-14 15:27 compressed_tensors/quantization/observers/base.py
--rw-r--r--  2.0 unx     2166 b- defN 24-May-14 15:27 compressed_tensors/quantization/observers/helpers.py
--rw-r--r--  2.0 unx     1859 b- defN 24-May-14 15:27 compressed_tensors/quantization/observers/memoryless.py
--rw-r--r--  2.0 unx     3071 b- defN 24-May-14 15:27 compressed_tensors/quantization/observers/min_max.py
--rw-r--r--  2.0 unx      656 b- defN 24-May-14 15:27 compressed_tensors/quantization/utils/__init__.py
--rw-r--r--  2.0 unx     4214 b- defN 24-May-14 15:27 compressed_tensors/quantization/utils/helpers.py
--rw-r--r--  2.0 unx      658 b- defN 24-May-14 15:27 compressed_tensors/registry/__init__.py
--rw-r--r--  2.0 unx    11890 b- defN 24-May-14 15:27 compressed_tensors/registry/registry.py
--rw-r--r--  2.0 unx      665 b- defN 24-May-14 15:27 compressed_tensors/utils/__init__.py
--rw-r--r--  2.0 unx     1735 b- defN 24-May-14 15:27 compressed_tensors/utils/helpers.py
--rw-r--r--  2.0 unx     8502 b- defN 24-May-14 15:27 compressed_tensors/utils/safetensors_load.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-14 15:29 compressed_tensors_nightly-0.3.3.20240514.dist-info/LICENSE
--rw-r--r--  2.0 unx     4056 b- defN 24-May-14 15:29 compressed_tensors_nightly-0.3.3.20240514.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-14 15:29 compressed_tensors_nightly-0.3.3.20240514.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-May-14 15:29 compressed_tensors_nightly-0.3.3.20240514.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4271 b- defN 24-May-14 15:29 compressed_tensors_nightly-0.3.3.20240514.dist-info/RECORD
-42 files, 145376 bytes uncompressed, 51490 bytes compressed:  64.6%
+Zip file size: 62874 bytes, number of entries: 43
+-rw-r--r--  2.0 unx      789 b- defN 24-May-16 00:03 compressed_tensors/__init__.py
+-rw-r--r--  2.0 unx      755 b- defN 24-May-16 00:03 compressed_tensors/base.py
+-rw-r--r--  2.0 unx     1512 b- defN 24-May-16 00:03 compressed_tensors/version.py
+-rw-r--r--  2.0 unx      992 b- defN 24-May-16 00:03 compressed_tensors/compressors/__init__.py
+-rw-r--r--  2.0 unx     2134 b- defN 24-May-16 00:03 compressed_tensors/compressors/base.py
+-rw-r--r--  2.0 unx     1257 b- defN 24-May-16 00:03 compressed_tensors/compressors/dense.py
+-rw-r--r--  2.0 unx     5403 b- defN 24-May-16 00:03 compressed_tensors/compressors/helpers.py
+-rw-r--r--  2.0 unx     4744 b- defN 24-May-16 00:03 compressed_tensors/compressors/int_quantized.py
+-rw-r--r--  2.0 unx    10426 b- defN 24-May-16 00:03 compressed_tensors/compressors/model_compressor.py
+-rw-r--r--  2.0 unx     7885 b- defN 24-May-16 00:03 compressed_tensors/compressors/pack_quantized.py
+-rw-r--r--  2.0 unx     8632 b- defN 24-May-16 00:03 compressed_tensors/compressors/sparse_bitmask.py
+-rw-r--r--  2.0 unx      704 b- defN 24-May-16 00:03 compressed_tensors/config/__init__.py
+-rw-r--r--  2.0 unx     1454 b- defN 24-May-16 00:03 compressed_tensors/config/base.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-May-16 00:03 compressed_tensors/config/dense.py
+-rw-r--r--  2.0 unx     1308 b- defN 24-May-16 00:03 compressed_tensors/config/sparse_bitmask.py
+-rw-r--r--  2.0 unx      760 b- defN 24-May-16 00:03 compressed_tensors/quantization/__init__.py
+-rw-r--r--  2.0 unx     4360 b- defN 24-May-16 00:03 compressed_tensors/quantization/quant_args.py
+-rw-r--r--  2.0 unx     8042 b- defN 24-May-16 00:03 compressed_tensors/quantization/quant_config.py
+-rw-r--r--  2.0 unx     1480 b- defN 24-May-16 00:03 compressed_tensors/quantization/quant_scheme.py
+-rw-r--r--  2.0 unx      798 b- defN 24-May-16 00:03 compressed_tensors/quantization/lifecycle/__init__.py
+-rw-r--r--  2.0 unx     7625 b- defN 24-May-16 00:03 compressed_tensors/quantization/lifecycle/apply.py
+-rw-r--r--  2.0 unx     1776 b- defN 24-May-16 00:03 compressed_tensors/quantization/lifecycle/calibration.py
+-rw-r--r--  2.0 unx     2247 b- defN 24-May-16 00:03 compressed_tensors/quantization/lifecycle/compressed.py
+-rw-r--r--  2.0 unx    11373 b- defN 24-May-16 00:03 compressed_tensors/quantization/lifecycle/forward.py
+-rw-r--r--  2.0 unx     1726 b- defN 24-May-16 00:03 compressed_tensors/quantization/lifecycle/frozen.py
+-rw-r--r--  2.0 unx     3697 b- defN 24-May-16 00:03 compressed_tensors/quantization/lifecycle/initialize.py
+-rw-r--r--  2.0 unx      745 b- defN 24-May-16 00:03 compressed_tensors/quantization/observers/__init__.py
+-rw-r--r--  2.0 unx     5156 b- defN 24-May-16 00:03 compressed_tensors/quantization/observers/base.py
+-rw-r--r--  2.0 unx     2166 b- defN 24-May-16 00:03 compressed_tensors/quantization/observers/helpers.py
+-rw-r--r--  2.0 unx     1859 b- defN 24-May-16 00:03 compressed_tensors/quantization/observers/memoryless.py
+-rw-r--r--  2.0 unx     3071 b- defN 24-May-16 00:03 compressed_tensors/quantization/observers/min_max.py
+-rw-r--r--  2.0 unx      656 b- defN 24-May-16 00:03 compressed_tensors/quantization/utils/__init__.py
+-rw-r--r--  2.0 unx     6017 b- defN 24-May-16 00:03 compressed_tensors/quantization/utils/helpers.py
+-rw-r--r--  2.0 unx      658 b- defN 24-May-16 00:03 compressed_tensors/registry/__init__.py
+-rw-r--r--  2.0 unx    11890 b- defN 24-May-16 00:03 compressed_tensors/registry/registry.py
+-rw-r--r--  2.0 unx      665 b- defN 24-May-16 00:03 compressed_tensors/utils/__init__.py
+-rw-r--r--  2.0 unx     1735 b- defN 24-May-16 00:03 compressed_tensors/utils/helpers.py
+-rw-r--r--  2.0 unx     8502 b- defN 24-May-16 00:03 compressed_tensors/utils/safetensors_load.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-16 00:07 compressed_tensors_nightly-0.3.3.20240516.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5633 b- defN 24-May-16 00:07 compressed_tensors_nightly-0.3.3.20240516.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 00:07 compressed_tensors_nightly-0.3.3.20240516.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-May-16 00:07 compressed_tensors_nightly-0.3.3.20240516.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4376 b- defN 24-May-16 00:07 compressed_tensors_nightly-0.3.3.20240516.dist-info/RECORD
+43 files, 157793 bytes uncompressed, 55606 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -21,14 +21,17 @@
 
 Filename: compressed_tensors/compressors/int_quantized.py
 Comment: 
 
 Filename: compressed_tensors/compressors/model_compressor.py
 Comment: 
 
+Filename: compressed_tensors/compressors/pack_quantized.py
+Comment: 
+
 Filename: compressed_tensors/compressors/sparse_bitmask.py
 Comment: 
 
 Filename: compressed_tensors/config/__init__.py
 Comment: 
 
 Filename: compressed_tensors/config/base.py
@@ -105,23 +108,23 @@
 
 Filename: compressed_tensors/utils/helpers.py
 Comment: 
 
 Filename: compressed_tensors/utils/safetensors_load.py
 Comment: 
 
-Filename: compressed_tensors_nightly-0.3.3.20240514.dist-info/LICENSE
+Filename: compressed_tensors_nightly-0.3.3.20240516.dist-info/LICENSE
 Comment: 
 
-Filename: compressed_tensors_nightly-0.3.3.20240514.dist-info/METADATA
+Filename: compressed_tensors_nightly-0.3.3.20240516.dist-info/METADATA
 Comment: 
 
-Filename: compressed_tensors_nightly-0.3.3.20240514.dist-info/WHEEL
+Filename: compressed_tensors_nightly-0.3.3.20240516.dist-info/WHEEL
 Comment: 
 
-Filename: compressed_tensors_nightly-0.3.3.20240514.dist-info/top_level.txt
+Filename: compressed_tensors_nightly-0.3.3.20240516.dist-info/top_level.txt
 Comment: 
 
-Filename: compressed_tensors_nightly-0.3.3.20240514.dist-info/RECORD
+Filename: compressed_tensors_nightly-0.3.3.20240516.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## compressed_tensors/compressors/__init__.py

```diff
@@ -15,8 +15,9 @@
 # flake8: noqa
 
 from .base import Compressor
 from .dense import DenseCompressor
 from .helpers import load_compressed, save_compressed, save_compressed_model
 from .int_quantized import IntQuantizationCompressor
 from .model_compressor import ModelCompressor
+from .pack_quantized import PackedQuantizationCompressor
 from .sparse_bitmask import BitmaskCompressor, BitmaskTensor
```

## compressed_tensors/compressors/base.py

```diff
@@ -50,10 +50,11 @@
         """
         Reads a compressed state dict located at path_to_model_or_tensors
         and returns a generator for sequentially decompressing back to a
         dense state dict
 
         :param model_path: path to compressed safetensors model (directory with
             one or more safetensors files) or compressed tensors file
+        :param device: optional device to load intermediate weights into
         :return: compressed state dict
         """
         raise NotImplementedError()
```

## compressed_tensors/compressors/int_quantized.py

```diff
@@ -14,15 +14,17 @@
 
 import logging
 from typing import Dict, Generator, Tuple
 
 import torch
 from compressed_tensors.compressors import Compressor
 from compressed_tensors.config import CompressionFormat
+from compressed_tensors.quantization import QuantizationArgs
 from compressed_tensors.quantization.lifecycle.forward import dequantize, quantize
+from compressed_tensors.quantization.utils import can_quantize
 from compressed_tensors.utils import get_nested_weight_mappings, merge_names
 from safetensors import safe_open
 from torch import Tensor
 from tqdm import tqdm
 
 
 __all__ = ["IntQuantizationCompressor"]
@@ -36,34 +38,42 @@
     Integer compression for quantized models. Weight of each quantized layer is
     converted from its original float type to the format specified by the layer's
     quantization scheme.
     """
 
     COMPRESSION_PARAM_NAMES = ["weight", "weight_scale", "weight_zero_point"]
 
-    def compress(self, model_state: Dict[str, Tensor], **kwargs) -> Dict[str, Tensor]:
-        model_quant_args = kwargs["model_quant_args"]
+    def compress(
+        self,
+        model_state: Dict[str, Tensor],
+        model_quant_args: Dict[str, QuantizationArgs],
+        **kwargs,
+    ) -> Dict[str, Tensor]:
+        """
+        Compresses a dense state dict
+
+        :param model_state: state dict of uncompressed model
+        :param model_quant_args: quantization args for each quantized weight, needed for
+        quantize function to calculate bit depth
+        :return: compressed state dict
+        """
         compressed_dict = {}
         _LOGGER.debug(
             f"Compressing model with {len(model_state)} parameterized layers..."
         )
 
         for name, value in tqdm(model_state.items(), desc="Compressing model"):
             if name.endswith(".weight"):
                 prefix = name.removesuffix(".weight")
                 scale = model_state.get(merge_names(prefix, "weight_scale"), None)
                 zp = model_state.get(merge_names(prefix, "weight_zero_point"), None)
                 if scale is not None and zp is not None:
                     # weight is quantized, compress it
                     quant_args = model_quant_args[prefix]
-                    try:
-                        bit_depth = torch.finfo(value.dtype).bits
-                    except TypeError:
-                        bit_depth = torch.iinfo(value.dtype).bits
-                    if bit_depth > quant_args.num_bits:
+                    if can_quantize(value, quant_args):
                         # only quantize if not already quantized
                         value = quantize(
                             x=value,
                             scale=scale,
                             zero_point=zp,
                             args=quant_args,
                             dtype=torch.int8,
@@ -72,14 +82,24 @@
             compressed_dict[name] = value.to("cpu")
 
         return compressed_dict
 
     def decompress(
         self, path_to_model_or_tensors: str, device: str = "cpu"
     ) -> Generator[Tuple[str, Tensor], None, None]:
+        """
+        Reads a compressed state dict located at path_to_model_or_tensors
+        and returns a generator for sequentially decompressing back to a
+        dense state dict
+
+        :param model_path: path to compressed safetensors model (directory with
+            one or more safetensors files) or compressed tensors file
+        :param device: optional device to load intermediate weights into
+        :return: compressed state dict
+        """
         weight_mappings = get_nested_weight_mappings(
             path_to_model_or_tensors, self.COMPRESSION_PARAM_NAMES
         )
         for weight_name in weight_mappings.keys():
             weight_data = {}
             for param_name, safe_path in weight_mappings[weight_name].items():
                 full_name = merge_names(weight_name, param_name)
```

## compressed_tensors/config/base.py

```diff
@@ -22,14 +22,15 @@
 __all__ = ["SparsityCompressionConfig", "CompressionFormat"]
 
 
 class CompressionFormat(Enum):
     dense = "dense"
     sparse_bitmask = "sparse-bitmask"
     int_quantized = "int-quantized"
+    pack_quantized = "pack-quantized"
 
 
 class SparsityCompressionConfig(RegistryMixin, BaseModel):
     """
     Base data class for storing sparsity compression parameters
 
     :param format: name of compression format
```

## compressed_tensors/quantization/lifecycle/apply.py

```diff
@@ -26,15 +26,18 @@
 from compressed_tensors.quantization.lifecycle.initialize import (
     initialize_module_for_quantization,
 )
 from compressed_tensors.quantization.quant_config import (
     QuantizationConfig,
     QuantizationStatus,
 )
-from compressed_tensors.quantization.utils import iter_named_leaf_modules
+from compressed_tensors.quantization.utils import (
+    infer_quantization_status,
+    iter_named_leaf_modules,
+)
 from compressed_tensors.utils.safetensors_load import get_safetensors_folder
 from torch.nn import Module
 
 
 __all__ = [
     "load_pretrained_quantization",
     "apply_quantization_config",
@@ -117,15 +120,15 @@
 def apply_quantization_status(model: Module, status: QuantizationStatus):
     """
     Applies in place the quantization lifecycle up to the given status
 
     :param model: model to apply quantization to
     :param status: status to update the module to
     """
-    current_status = _infer_status(model)
+    current_status = infer_quantization_status(model)
 
     if status >= QuantizationStatus.INITIALIZED > current_status:
         model.apply(initialize_module_for_quantization)
 
     if current_status < status >= QuantizationStatus.CALIBRATION > current_status:
         model.apply(set_module_for_calibration)
```

## compressed_tensors/quantization/lifecycle/forward.py

```diff
@@ -225,15 +225,18 @@
 
     return output
 
 
 def wrap_module_forward_quantized(module: Module, scheme: QuantizationScheme):
     # expects a module already initialized and injected with the parameters in
     # initialize_module_for_quantization
-    forward_func_orig = module.forward.__func__
+    if hasattr(module.forward, "__func__"):
+        forward_func_orig = module.forward.__func__
+    else:
+        forward_func_orig = module.forward.func
 
     @wraps(forward_func_orig)  # ensures docstring, names, etc are propagated
     def wrapped_forward(self, *args, **kwargs):
         input_ = args[0]
 
         if scheme.input_activations is not None:
             # calibrate and (fake) quantize input activations when applicable
```

## compressed_tensors/quantization/utils/helpers.py

```diff
@@ -8,30 +8,51 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Tuple
+import logging
+from typing import Optional, Tuple
 
 import torch
 from compressed_tensors.quantization.observers.base import Observer
 from torch.nn import Module
 from tqdm import tqdm
 
 
 __all__ = [
+    "infer_quantization_status",
     "is_module_quantized",
     "is_model_quantized",
     "iter_named_leaf_modules",
     "module_type",
     "calculate_compression_ratio",
+    "get_torch_bit_depth",
+    "can_quantize",
 ]
 
+_LOGGER: logging.Logger = logging.getLogger(__name__)
+
+
+def infer_quantization_status(model: Module) -> Optional["QuantizationStatus"]:  # noqa
+    """
+    Checks the quantization status of a model. Assumes all modules in the model have
+    the same status, so only the first quantized model is checked.
+
+    :param model: model to check quantization status for
+    :return: quantization status if the model is quantized, otherwise None
+    """
+    for module in model.modules():
+        status = getattr(module, "quantization_status", None)
+        if status is not None:
+            return status
+    return None
+
 
 def is_module_quantized(module: Module) -> bool:
     """
     Check if a module is quantized, based on the existence of a non-empty quantization
     scheme
 
     :param module: pytorch module to check
@@ -96,14 +117,49 @@
                 if not isinstance(child, Observer):
                     has_non_observer_children = True
 
             if not has_non_observer_children:
                 yield name, submodule
 
 
+def get_torch_bit_depth(value: torch.Tensor) -> int:
+    """
+    Determine the number of bits used to represent the dtype of a tensor
+
+    :param value: tensor to check bit depth of
+    :return: bit depth of each element in the value tensor
+    """
+    try:
+        bit_depth = torch.finfo(value.dtype).bits
+    except TypeError:
+        bit_depth = torch.iinfo(value.dtype).bits
+
+    return bit_depth
+
+
+def can_quantize(value: torch.Tensor, quant_args: "QuantizationArgs") -> bool:  # noqa
+    """
+    Checks if value can be quantized by quant_args.
+
+    :param value: tensor to check for quantization
+    :param quant_args: QuantizationArgs to use for quantization
+    :return: False if value is already quantized to quant_args or value is incompatible
+    with quant_args, True if value can be quantized with quant_args
+    """
+    bit_depth = get_torch_bit_depth(value)
+    requested_depth = quant_args.num_bits
+    if bit_depth < quant_args.num_bits:
+        _LOGGER.warn(
+            f"Can't quantize tensor with bit depth {bit_depth} to {requested_depth}."
+            "The QuantizationArgs provided are not compatible with the input tensor."
+        )
+
+    return bit_depth > quant_args.num_bits
+
+
 def calculate_compression_ratio(model: Module) -> float:
     """
     Calculates the quantization compression ratio of a pytorch model, based on the
     number of bits needed to represent the total weights in compressed form. Does not
     take into account activation quantizatons.
 
     :param model: pytorch module to calculate compression ratio for
@@ -112,18 +168,15 @@
     total_compressed = 0.0
     total_uncompressed = 0.0
     for name, submodule in tqdm(
         iter_named_leaf_modules(model),
         desc="Calculating quantization compression ratio",
     ):
         for parameter in model.parameters():
-            try:
-                uncompressed_bits = torch.finfo(parameter.dtype).bits
-            except TypeError:
-                uncompressed_bits = torch.iinfo(parameter.dtype).bits
+            uncompressed_bits = get_torch_bit_depth(parameter)
             compressed_bits = uncompressed_bits
             if is_module_quantized(submodule):
                 compressed_bits = submodule.quantization_scheme.weights.num_bits
 
             num_weights = parameter.numel()
             total_compressed += compressed_bits * num_weights
             total_uncompressed += uncompressed_bits * num_weights
```

## Comparing `compressed_tensors_nightly-0.3.3.20240514.dist-info/LICENSE` & `compressed_tensors_nightly-0.3.3.20240516.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `compressed_tensors_nightly-0.3.3.20240514.dist-info/RECORD` & `compressed_tensors_nightly-0.3.3.20240516.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 compressed_tensors/__init__.py,sha256=SV1csvHUVCd8kHXz6UDZim1HZ_fAVG3vfk-j_4Bb6hY,789
 compressed_tensors/base.py,sha256=OA2TOLP1gP3LSH7gp508eqr2ZtDQ-pqRHElCp-aB0vs,755
 compressed_tensors/version.py,sha256=V8krJZctm43D4AGQhJY6dB0MvP1-T9TJ8BcGa8kESrI,1512
-compressed_tensors/compressors/__init__.py,sha256=xUiZjKof5nxsmd_whbuTlmJNx54aJQeyTQhYjKsU6oo,935
-compressed_tensors/compressors/base.py,sha256=ictzKWJgE80MSzu5ZG4FY6EdEHgP9LaTYn73NvLDRRM,2061
+compressed_tensors/compressors/__init__.py,sha256=3yyoNICHll3F4HS6Yu-cgNZpDhfuobFNWCs6DrPcUyQ,992
+compressed_tensors/compressors/base.py,sha256=LWEgbpgTxzmoqQ7Xhq2OQszUgWoDtFuGCiV1Y8nlBGw,2134
 compressed_tensors/compressors/dense.py,sha256=G_XHbvuENyupIKlXSITOQgvPkNkcMEOLcLWQr70V9EE,1257
 compressed_tensors/compressors/helpers.py,sha256=k9avlkmeYj6vkOAvl-MgcixtP7ib24SCfhzZ-RusXfw,5403
-compressed_tensors/compressors/int_quantized.py,sha256=2NhcmkryvFA7pW-4gid06d7HYIWET5CmTVVK9bBxXQM,4023
+compressed_tensors/compressors/int_quantized.py,sha256=I0FqnjtwCiJvQxi9YyfA8aBeaR5csqtq1bOrVvRqJ1I,4744
 compressed_tensors/compressors/model_compressor.py,sha256=teohd0xTbcIDIuEfZrH-bZyAzHn2UZH2KJXT-7Gk3sw,10426
+compressed_tensors/compressors/pack_quantized.py,sha256=K03l8kFqejpapgcMU5hMm1-JIX1cUVvU-VybGSN6RWA,7885
 compressed_tensors/compressors/sparse_bitmask.py,sha256=TH77NDFJwvQeySY75YV6w1zskZC-JcUGpua4zCFOgTY,8632
 compressed_tensors/config/__init__.py,sha256=ZBqWn3r6ku1qfmlHHYp0mQueY0i7Pwhr9rbQk9dDlMc,704
-compressed_tensors/config/base.py,sha256=0DTHzK-MOtGSC7vGLRCjeFnzjYnm3ebCCLS4CrgDSlo,1416
+compressed_tensors/config/base.py,sha256=grf5tDaLep8i2-W_p7H-fW9DOGXDi4Zz7su7zjs1Qqc,1454
 compressed_tensors/config/dense.py,sha256=NgSxnFCnckU9-iunxEaqiFwqgdO7YYxlWKR74jNbjks,1317
 compressed_tensors/config/sparse_bitmask.py,sha256=pZUboRNZTu6NajGOQEFExoPknak5ynVAUeiiYpS1Gt8,1308
 compressed_tensors/quantization/__init__.py,sha256=83J5bPB7PavN2TfCoW7_vEDhfYpm4TDrqYO9vdSQ5bk,760
 compressed_tensors/quantization/quant_args.py,sha256=A6b2V8lhsM8Ho8RjlPBQdxRUDNWhqq-ie5E3RR2_GNg,4360
 compressed_tensors/quantization/quant_config.py,sha256=U6oEzheNK1d-0kHARzwepasnmS7HHqU_zGwoDBJ-lxU,8042
 compressed_tensors/quantization/quant_scheme.py,sha256=X3oqmZPiIKtX5tEKKUj-0N6hB68NeiU2b1GcQEQPadQ,1480
 compressed_tensors/quantization/lifecycle/__init__.py,sha256=ggRGWRqhCxCaTTDWRcgTVX3axnS2xV6rc5YvdzK7fSg,798
-compressed_tensors/quantization/lifecycle/apply.py,sha256=hidWZiq1FDddAWhivIVTplamyZiVb-rSnbPluNK2YKA,7573
+compressed_tensors/quantization/lifecycle/apply.py,sha256=whKfNGC_EZm0BC23AP7qWfjRe5OJVWmcZOpX7lryZZc,7625
 compressed_tensors/quantization/lifecycle/calibration.py,sha256=mLns4jlaWmBwOW8Jtlm5bMX-JET1AiZYUBO7qa-XuxI,1776
 compressed_tensors/quantization/lifecycle/compressed.py,sha256=VreB10xPwgSLQQlTu20UCrFpRS--cA7-lx5s7nrPPrg,2247
-compressed_tensors/quantization/lifecycle/forward.py,sha256=THoaTfl1GeiixqzGqI8ISt03qxBd-wNc4Fsf1V3nZ54,11267
+compressed_tensors/quantization/lifecycle/forward.py,sha256=sXo7ReS2ehHFwbtwUbhPnsnnj-CZ3iyAZKmUzHxjTKc,11373
 compressed_tensors/quantization/lifecycle/frozen.py,sha256=h1XYt89MouBTf3jTYLG_6OdFxIu5q2N8tPjsy6J4E6Y,1726
 compressed_tensors/quantization/lifecycle/initialize.py,sha256=U6g9qifSF6pagQZQZEwd-rwWC6uQ_dZXn1wg6nr1Abg,3697
 compressed_tensors/quantization/observers/__init__.py,sha256=DNH31NQYrIBBcmHsMyFA6whh4pbRsLwuNa6L8AeXaGc,745
 compressed_tensors/quantization/observers/base.py,sha256=X7zeeFj42JxP_5dX2XbEGHcqLrkiV53-nJN3qhW2NA8,5156
 compressed_tensors/quantization/observers/helpers.py,sha256=JwALNfBYY9Eyl8Q180t0lGh8szumQj8TygfNl-isErs,2166
 compressed_tensors/quantization/observers/memoryless.py,sha256=ZHTPh4aURE8LvHBFaP--HIC2JanMX5-VRdIkE2JHthw,1859
 compressed_tensors/quantization/observers/min_max.py,sha256=s2I40pzTXrVAjIsavNt6TLAl7-qDUmdc43Xd5rb4XAY,3071
 compressed_tensors/quantization/utils/__init__.py,sha256=VdtEmP0bvuND_IGQnyqUPc5lnFp-1_yD7StKSX4x80w,656
-compressed_tensors/quantization/utils/helpers.py,sha256=dDfGR9PRNeKoqD50qoFPRXwsNckFRc38Ao2UrE_69Tk,4214
+compressed_tensors/quantization/utils/helpers.py,sha256=NzAH18Cn_-mTAR87y6IlcQU5gC393XSjgNKC9CRkr78,6017
 compressed_tensors/registry/__init__.py,sha256=FwLSNYqfIrb5JD_6OK_MT4_svvKTN_nEhpgQlQvGbjI,658
 compressed_tensors/registry/registry.py,sha256=fxjOjh2wklCvJhQxwofdy-zV8q7MkQ85SLG77nml2iA,11890
 compressed_tensors/utils/__init__.py,sha256=5DrYjoZbaEvSkJcC-GRSbM_RBHVF4tG9gMd3zsJnjLw,665
 compressed_tensors/utils/helpers.py,sha256=h0jfl9drs5FAx40tCHRcVtJqXixB5hT5yq_IG2aY_-w,1735
 compressed_tensors/utils/safetensors_load.py,sha256=wo9UirGrGlenBqZeqotvpCT7D5MEdjCo2J3HeRaIFoU,8502
-compressed_tensors_nightly-0.3.3.20240514.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-compressed_tensors_nightly-0.3.3.20240514.dist-info/METADATA,sha256=kQhsyTU2oXTX41J5rPQLSIMTVcXskMxS9Cj1EI4QuUI,4056
-compressed_tensors_nightly-0.3.3.20240514.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-compressed_tensors_nightly-0.3.3.20240514.dist-info/top_level.txt,sha256=w2i-GyPs2s1UwVxvutSvN_lM22SXC2hQFBmoMcPnV7Y,19
-compressed_tensors_nightly-0.3.3.20240514.dist-info/RECORD,,
+compressed_tensors_nightly-0.3.3.20240516.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+compressed_tensors_nightly-0.3.3.20240516.dist-info/METADATA,sha256=C_J0XMNZOkW4H6xwMbRX8ryXtoxksTo9CoMk25yoO-0,5633
+compressed_tensors_nightly-0.3.3.20240516.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+compressed_tensors_nightly-0.3.3.20240516.dist-info/top_level.txt,sha256=w2i-GyPs2s1UwVxvutSvN_lM22SXC2hQFBmoMcPnV7Y,19
+compressed_tensors_nightly-0.3.3.20240516.dist-info/RECORD,,
```

