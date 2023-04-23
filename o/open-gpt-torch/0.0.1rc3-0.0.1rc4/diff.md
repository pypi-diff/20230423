# Comparing `tmp/open_gpt_torch-0.0.1rc3.tar.gz` & `tmp/open_gpt_torch-0.0.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_gpt_torch-0.0.1rc3.tar", max compression
+gzip compressed data, was "open_gpt_torch-0.0.1rc4.tar", max compression
```

## Comparing `open_gpt_torch-0.0.1rc3.tar` & `open_gpt_torch-0.0.1rc4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    10825 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/LICENSE
--rw-r--r--   0        0        0     7513 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/README.md
--rw-r--r--   0        0        0      453 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/__init__.py
--rw-r--r--   0        0        0      474 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/adapter.py
--rw-r--r--   0        0        0      503 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/executor.py
--rw-r--r--   0        0        0     2544 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/factory.py
--rw-r--r--   0        0        0      844 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/helper.py
--rw-r--r--   0        0        0      349 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/hub.py
--rw-r--r--   0        0        0      349 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/logging.py
--rw-r--r--   0        0        0        0 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/flamingo/__init__.py
--rw-r--r--   0        0        0     4994 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/flamingo/flamingo_lm.py
--rw-r--r--   0        0        0     5878 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/flamingo/loading.py
--rw-r--r--   0        0        0     8828 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/flamingo/modeling.py
--rw-r--r--   0        0        0        0 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/flan/__init__.py
--rw-r--r--   0        0        0      863 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/flan/loading.py
--rw-r--r--   0        0        0      445 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/hf_model.py
--rw-r--r--   0        0        0        0 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/llama/__init__.py
--rw-r--r--   0        0        0     1245 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/llama/loading.py
--rw-r--r--   0        0        0        0 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/pythia/__init__.py
--rw-r--r--   0        0        0     1077 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/pythia/loading.py
--rw-r--r--   0        0        0     2862 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/profile.py
--rw-r--r--   0        0        0      931 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/serve.py
--rw-r--r--   0        0        0     1894 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/pyproject.toml
--rw-r--r--   0        0        0    19730 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.1rc3/PKG-INFO
+-rw-r--r--   0        0        0    10825 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/LICENSE
+-rw-r--r--   0        0        0     7518 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/README.md
+-rw-r--r--   0        0        0      453 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/__init__.py
+-rw-r--r--   0        0        0      474 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/adapter.py
+-rw-r--r--   0        0        0      503 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/executor.py
+-rw-r--r--   0        0        0     2598 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/factory.py
+-rw-r--r--   0        0        0     1767 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/helper.py
+-rw-r--r--   0        0        0      349 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/hub.py
+-rw-r--r--   0        0        0      349 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/logging.py
+-rw-r--r--   0        0        0        0 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/flamingo/__init__.py
+-rw-r--r--   0        0        0     5274 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/flamingo/flamingo_lm.py
+-rw-r--r--   0        0        0     5658 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/flamingo/loading.py
+-rw-r--r--   0        0        0     8561 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/flamingo/modeling.py
+-rw-r--r--   0        0        0        0 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/flan/__init__.py
+-rw-r--r--   0        0        0      863 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/flan/loading.py
+-rw-r--r--   0        0        0      638 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/hf_model.py
+-rw-r--r--   0        0        0        0 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/llama/__init__.py
+-rw-r--r--   0        0        0      846 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/llama/loading.py
+-rw-r--r--   0        0        0        0 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/pythia/__init__.py
+-rw-r--r--   0        0        0     1077 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/pythia/loading.py
+-rw-r--r--   0        0        0     2862 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/profile.py
+-rw-r--r--   0        0        0      931 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/serve.py
+-rw-r--r--   0        0        0     1887 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/pyproject.toml
+-rw-r--r--   0        0        0    19765 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.1rc4/PKG-INFO
```

### Comparing `open_gpt_torch-0.0.1rc3/LICENSE` & `open_gpt_torch-0.0.1rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc3/README.md` & `open_gpt_torch-0.0.1rc4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 You can view our roadmap with features that are planned, started, and completed on the [Roadmap discussion](discussions/categories/roadmap) category.
 
 ## Installation
 
 Install the package with pip:
 
 ```bash
-pip install open_gpts
+pip install open_gpt_torch
 ```
 
 ## Quickstart
 
 ```python
 import open_gpt
```

### Comparing `open_gpt_torch-0.0.1rc3/open_gpt/factory.py` & `open_gpt_torch-0.0.1rc4/open_gpt/factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from pathlib import Path
 from typing import Optional, Union
 
 import torch
 from loguru import logger
 
+from .helper import auto_dtype_and_device
+
 
 def list_models():
     """List the available models."""
     ...
 
 
 def load_state_dict(model: torch.nn.Module, checkpoint: Union[str, 'Path']):
@@ -18,60 +20,63 @@
     """
     ...
 
 
 def create_model_and_transforms(
     model_name: str,
     device: Optional[Union[str, torch.device]] = None,
-    precision: Optional[str] = 'fp32',
+    precision: Optional[str] = None,
     **kwargs,
 ):
     """Create a model of the given name.
 
     :param model_name: The name of the model to create.
     :param device: The device to create the model on.
     :param precision: The precision to use for the model.
     :param kwargs: Additional arguments to pass to the model.
     :return: The model.
     """
 
-    if not device:
-        device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+    dtype, device = auto_dtype_and_device(precision, device)
 
     # TODO: Add support for loading config based on model name
     model_config = {}
 
-    logger.debug(f'Loading model: {model_name}')
+    logger.info(
+        f'Loading "{model_name}" with precision: `{dtype}` on device: `{device}`'
+    )
 
     if model_name.startswith('openflamingo/OpenFlamingo'):
         from .models.flamingo.loading import load_model_and_transforms
 
         model_config = {
-            'clip_model_name': 'ViT-L-14::openai',
+            'vision_model_name_or_path': 'ViT-L-14::openai',
             'lang_model_name_or_path': 'llama_7B',
             'tokenizer_name_or_path': 'llama_7B',
         }
-        return load_model_and_transforms(model_name, device=device, **model_config)
+        return load_model_and_transforms(
+            model_name, device=device, dtype=dtype, **model_config
+        )
     elif model_name.startswith('facebook/llama'):
         from .models.llama.loading import load_model_and_tokenizer
 
         model_config = {
             'model_name_or_path': 'llama_7B',
             'tokenizer_name_or_path': 'llama_7B',
         }
-        return load_model_and_tokenizer(**model_config)
+        return load_model_and_tokenizer(
+            model_name, device=device, dtype=dtype, **model_config
+        )
     elif model_name.startswith('google/flan'):
-        from .helper import infer_dtype
         from .models.flan.loading import load_model_and_tokenizer
 
         return load_model_and_tokenizer(
-            model_name, device=device, dtype=infer_dtype(precision), **model_config
+            model_name, device=device, dtype=dtype, **model_config
         )
     elif model_name.startswith('EleutherAI/pythia'):
-        from .helper import infer_dtype
         from .models.pythia.loading import load_model_and_tokenizer
 
         return load_model_and_tokenizer(
-            model_name, device=device, dtype=infer_dtype(precision), **model_config
+            model_name, device=device, dtype=dtype, **model_config
         )
     else:
         raise ValueError(f'Unknown model name: {model_name}')
```

### Comparing `open_gpt_torch-0.0.1rc3/open_gpt/models/flamingo/flamingo_lm.py` & `open_gpt_torch-0.0.1rc4/open_gpt/models/flamingo/flamingo_lm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import random
+from typing import Optional, Union
 
+import torch
 import torch.nn as nn
 from open_flamingo.src.helpers import GatedCrossAttentionBlock
 from open_flamingo.src.utils import getattr_recursive, setattr_recursive
 
+from ...helper import auto_dtype_and_device
+
 
 class FlamingoLayer(nn.Module):
     def __init__(self, gated_cross_attn_layer, decoder_layer):
         super().__init__()
         self.gated_cross_attn_layer = gated_cross_attn_layer
         self.decoder_layer = decoder_layer
         self.vis_x = None
@@ -72,15 +76,16 @@
 
     def init_flamingo(
         self,
         media_token_id,
         vis_hidden_size,
         cross_attn_every_n_layers,
         use_media_placement_augmentation,
-        dtype=None,
+        device: Optional[Union[str, 'torch.device']] = None,
+        dtype: Optional[Union[str, 'torch.dtype']] = None,
     ):
         """
         Initialize Flamingo by adding a new gated cross attn to the decoder. Store the media token id for computing the media locations.
         """
 
         self.gated_cross_attn_layers = nn.ModuleList(
             [
@@ -102,16 +107,18 @@
                 ]
             )
         )
         self.media_token_id = media_token_id
         self.use_media_placement_augmentation = use_media_placement_augmentation
         self.initialized_flamingo = True
 
-        if dtype is not None and str(dtype) == 'torch.float16':
+        dtype, device = auto_dtype_and_device(dtype, device)
+        if str(dtype) == 'torch.float16':
             self.gated_cross_attn_layers.half()
+        self.gated_cross_attn_layers.to(device)
 
     def forward(self, *input, **kwargs):
         """Condition the Flamingo layers on the media locations before forward()"""
 
         if not self.initialized_flamingo:
             raise ValueError(
                 "Flamingo layers are not initialized. Please call `init_flamingo` first."
```

### Comparing `open_gpt_torch-0.0.1rc3/open_gpt/models/flamingo/loading.py` & `open_gpt_torch-0.0.1rc4/open_gpt/models/flamingo/loading.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,50 @@
-from typing import TYPE_CHECKING, Optional, Union
+from typing import Optional, Union
 
 import open_clip
-
-# from open_flamingo.src.flamingo_lm import FlamingoLMMixin
+import torch
+from loguru import logger
 from open_flamingo.src.utils import extend_instance
 
-from ..llama.loading import load_model_and_tokenizer
-from .flamingo_lm import FlamingoLMMixin
-from .modeling import FlamingoModel
-
-if TYPE_CHECKING:
-    import torch
-
 
 def load_model_and_transforms(
     model_name_or_path: str,
-    clip_model_name: str,
+    vision_model_name_or_path: str,
     lang_model_name_or_path: str,
-    tokenizer_name_or_path: str,
-    decoder_layers_attr_name: str = None,
-    device: Optional[Union[str, 'torch.device']] = 'cpu',
+    tokenizer_name_or_path: Optional[str] = None,
+    decoder_layers_attr_name: Optional[str] = None,
+    device: 'torch.device' = torch.device('cuda'),
+    dtype: 'torch.dtype' = torch.float16,
     **kwargs,
 ):
     """Load a Flamingo model and its associated image and text processors.
 
     :param model_name_or_path: The name or path of the model to load.
-    :param clip_model_name: The name of the CLIP model to use.
+    :param vision_model_name_or_path: The name or path of the vision model to use.
     :param lang_model_name_or_path: The name or path of the language model to use.
-    :param tokenizer_name_or_path: The name or path of the tokenizer to use.
+    :param tokenizer_name_or_path: The name or path of the tokenizer to use. If not specified, the tokenizer associated with the model will be used.
     :param decoder_layers_attr_name: The name of the attribute that specifies the decoder layers.
     :param device: The device to load the model on.
+    :param dtype: The dtype to load the model with.
     """
 
-    from accelerate.hooks import (
-        AlignDevicesHook,
-        add_hook_to_module,
-        attach_align_device_hook_on_blocks,
+    from ...helper import cast_precision
+    from ..llama.loading import (
+        load_model_and_tokenizer as load_llama_model_and_tokenizer,
     )
+    from .flamingo_lm import FlamingoLMMixin
+    from .modeling import FlamingoModel
 
     # load the vision model
-    model_name, *pretrained = clip_model_name.split("::")
+    precision = cast_precision(dtype)
+    model_name, *pretrained = vision_model_name_or_path.split("::")
     pretrained = pretrained[0] if len(pretrained) == 1 else 'openai'
     clip_model, _, image_processor = open_clip.create_model_and_transforms(
-        model_name, pretrained=pretrained, device='cuda', precision='fp16'
+        model_name, pretrained=pretrained, device=device, precision=precision
     )
-    clip_model.to('cuda')
     # set the vision encoder to output the visual features
     clip_model.visual.output_tokens = True
 
     # remove text encoder to save footprint and memory
     if hasattr(clip_model, 'text'):
         del clip_model.text
     elif hasattr(clip_model, 'transformer'):
@@ -63,34 +59,31 @@
     #     offload=None,
     #     offload_buffers=False,
     #     weights_map=None,
     #     preload_module_classes=None,
     # )
 
     # load the language model
-    lang_model, tokenizer = load_model_and_tokenizer(
+    lang_model, tokenizer = load_llama_model_and_tokenizer(
         model_name_or_path=lang_model_name_or_path,
         tokenizer_name_or_path=tokenizer_name_or_path,
+        device=device,
+        dtype=dtype,
     )
 
-    # # Hotfix for the flamingo forward issue due to the HF accelerate hooks
-
-    # device_map = lang_model.hf_device_map
-    # offload = {name: device in ['cpu', 'disk'] for name, device in device_map.items()}
-
-    # lang_model = remove_hook_from_module(lang_model, recurse=True)
-
     # add Flamingo special tokens to the tokenizer
     tokenizer.add_special_tokens(
         {"additional_special_tokens": ["<|endofchunk|>", "<image>"]}
     )
     if tokenizer.pad_token is None:
         # Issue: GPT models don't have a pad token, which we use to
         # modify labels for the loss.
         tokenizer.add_special_tokens({"pad_token": "<PAD>"})
+    # For generation padding tokens should be on the left
+    tokenizer.padding_side = "left"
 
     extend_instance(lang_model, FlamingoLMMixin)
 
     if decoder_layers_attr_name is None:
         decoder_layers_attr_name = _infer_decoder_layers_attr_name(lang_model)
     lang_model.set_decoder_layers_attr_name(decoder_layers_attr_name)
     lang_model.resize_token_embeddings(len(tokenizer))
@@ -98,54 +91,50 @@
     flamingo_config = {
         "image_size": open_clip.get_model_config(model_name)["vision_cfg"]["width"],
         "cross_attn_every_n_layers": 4,
         "end_chunk_token_id": tokenizer.encode("<|endofchunk|>")[-1],
         "media_token_id": tokenizer.encode("<image>")[-1],
     }
 
-    # execution_device = next(iter(lang_model.parameters())).device
-    # add_hook_to_module(lang_model, AlignDevicesHook(io_same_device=True), append=True)
-    #
-    # attach_align_device_hook_on_blocks(
-    #     lang_model,
-    #     execution_device=execution_device,
-    #     offload=None,
-    #     offload_buffers=False,
-    #     weights_map=None,
-    #     preload_module_classes=None,
-    # )
-
     model = FlamingoModel(
         clip_model,
         lang_model,
         model_config=flamingo_config,
         device=device,
-        dtype='torch.float16',
+        dtype=dtype,
     )
 
     # Freeze all parameters
     model.requires_grad_(False)
     assert sum(p.numel() for p in model.parameters() if p.requires_grad) == 0
 
     # Unfreeze perceiver, gated_cross_attn_layers, and LM input embeddings
     model.perceiver.requires_grad_(True)
-    model.language_model.gated_cross_attn_layers.requires_grad_(True)
+    model.lang_encoder.gated_cross_attn_layers.requires_grad_(True)
     # TODO: only unfreeze the input embeddings of the additional special tokens
-    model.language_model.get_input_embeddings().requires_grad_(True)
+    model.lang_encoder.get_input_embeddings().requires_grad_(True)
 
-    print(
+    logger.debug(
         f"Flamingo model initialized with {sum(p.numel() for p in model.parameters() if p.requires_grad)} trainable parameters"
     )
 
     # grab model checkpoint from huggingface hub
-    import torch
+    import os
+
     from huggingface_hub import hf_hub_download
 
-    # checkpoint_path = hf_hub_download(model_name_or_path, "checkpoint.pt")
-    # model.load_state_dict(torch.load(checkpoint_path), strict=False)
+    hf_token = os.environ.get("HF_TOKEN")
+    assert (
+        hf_token is not None
+    ), "Please set HF_TOKEN environment variable to download model from HuggingFace Hub"
+
+    checkpoint_path = hf_hub_download(
+        model_name_or_path, "checkpoint.pt", token=hf_token
+    )
+    model.load_state_dict(torch.load(checkpoint_path), strict=False)
 
     return model, tokenizer, image_processor
 
 
 def _infer_decoder_layers_attr_name(model):
     for k in __KNOWN_DECODER_LAYERS_ATTR_NAMES:
         if k.lower() in model.__class__.__name__.lower():
```

### Comparing `open_gpt_torch-0.0.1rc3/open_gpt/models/flamingo/modeling.py` & `open_gpt_torch-0.0.1rc4/open_gpt/models/flamingo/modeling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,68 @@
 from typing import Callable, Optional, Union
 
 import torch
 from einops import rearrange
+from loguru import logger
 from open_flamingo.src.helpers import PerceiverResampler
 from torch import nn
 
+from ...helper import auto_dtype_and_device
+
 
 class FlamingoModel(nn.Module):
     def __init__(
         self,
         vision_encoder: 'nn.Module',
         language_model: 'nn.Module',
+        device: Optional[Union[str, 'torch.device']] = None,
+        dtype: Optional[Union[str, 'torch.dtype']] = None,
         model_config: dict = {},
-        device: Optional[Union[str, 'torch.device']] = 'cpu',
-        dtype: Optional[Union[str, 'torch.dtype']] = 'torch.float32',
         **kwargs,
     ):
         """An open source version of DeepMind's Flamingo model!
         Adapted from the original implementation at https://github.com/mlfoundations/open_flamingo
 
         :param vision_encoder: the vision encoder to extract visual features, e.g. CLIP model
         :param language_model: the language model to extract textual features and generate the output texts, e.g., LLaMa model
         :param model_config: a dictionary of model configuration
         :param device: the device to run the model on
         :param dtype: the data type to run the model on
         :param kwargs: other arguments
         """
         super().__init__()
 
-        self.model_config = model_config
+        self.dtype, self.device = auto_dtype_and_device(dtype, device)
 
+        self.model_config = model_config
         self.vision_encoder = vision_encoder
-        self.language_model = language_model
+        self.lang_encoder = language_model
 
         self.perceiver = PerceiverResampler(dim=self.model_config['image_size'])
-        if str(dtype) == 'torch.float16':
+        if str(self.dtype) == 'torch.float16':
             self.perceiver.half()
-
-        self.perceiver.to(device)
+        elif str(self.dtype) == 'torch.int8':
+            raise NotImplementedError('int8 is not supported yet')
+        self.perceiver.to(self.device)
 
         self.media_token_id = model_config['media_token_id']
         self.end_chunk_token_id = model_config['end_chunk_token_id']
 
-        self.language_model.init_flamingo(
+        logger.debug(
+            f"media_token_id: {self.media_token_id}, end_chunk_token_id: {self.end_chunk_token_id}"
+        )
+
+        self.lang_encoder.init_flamingo(
             media_token_id=self.media_token_id,
             vis_hidden_size=model_config['image_size'],
             cross_attn_every_n_layers=model_config['cross_attn_every_n_layers'],
             use_media_placement_augmentation=False,
             dtype=dtype,
+            device=device,
         )
-        self.language_model.gated_cross_attn_layers.to(device)
 
     def forward(
         self,
         vision_inputs: 'torch.Tensor',
         text_inputs: 'torch.Tensor',
         attention_mask: Optional['torch.Tensor'] = None,
         labels: Optional['torch.Tensor'] = None,
@@ -68,23 +77,23 @@
         :param attention_mask: attention mask, 1 for tokens that are not masked, 0 for masked tokens. Defaults to None.
         :param labels: labels for computing the language modeling loss. Defaults to None.
         :param past_key_values: cached past key and values for fast decoding. Defaults to None.
         """
 
         self._vision_encode(vision_inputs)
 
-        output = self.language_model(
+        output = self.lang_encoder(
             input_ids=text_inputs,
             attention_mask=attention_mask,
             labels=labels,
             past_key_values=past_key_values,
             use_cache=False,
         )
 
-        self.language_model.clear_conditioned_layers()
+        self.lang_encoder.clear_conditioned_layers()
 
         return output
 
     def generate(
         self,
         vision_inputs: 'torch.Tensor',
         text_inputs: 'torch.Tensor',
@@ -95,15 +104,15 @@
         top_k: int = 0,
         top_p: float = 1.0,
         no_repeat_ngram_size: int = 0,
         prefix_allowed_tokens_fn: Optional[Callable] = None,
         length_penalty: float = 1.0,
         num_return_sequences: int = 1,
         do_sample: bool = False,
-        early_stopping: bool = False,
+        early_stopping: bool = True,
     ):
         """
         Generate text conditioned on vision and language inputs.
 
         :param vision_inputs: vision images input with shape (B, T, F, Channels, Height, Width).
                 Images in the same chunk are collated along T, and frames are collated along F
                 Currently only F=1 is supported (single-frame videos)
@@ -120,45 +129,37 @@
         :param num_return_sequences: number of return sequences. Defaults to 1.
         :param do_sample: whether to sample or not. Defaults to False.
         :param early_stopping: whether to stop early or not. Defaults to False.
 
         :return: text_inputs with generated tokens appended to it (batch_size, sequence_length)
         """
 
-        vision_inputs = vision_inputs.to(dtype=torch.float16)
-        vision_inputs = vision_inputs.cuda()
-        text_inputs = text_inputs.cuda()
+        vision_inputs = vision_inputs.to(dtype=self.dtype, device=self.device)
         if attention_mask is not None:
-            attention_mask = attention_mask.cuda()
+            attention_mask = attention_mask.to(self.device)
+        text_inputs = text_inputs.to(self.device)
 
         if num_beams > 1:
             vision_inputs = vision_inputs.repeat_interleave(num_beams, dim=0)
 
-        print(f'===> vision inputs device: {vision_inputs.device}')
+        _vision_x = self._vision_encode(vision_inputs=vision_inputs)
 
-        vision_x = self._vision_encode(vision_inputs=vision_inputs)
-
-        print(f'====> encode vision done {vision_x.device}...')
-
-        if not self.language_model.initialized_flamingo:
+        if not self.lang_encoder.initialized_flamingo:
             raise ValueError(
                 "Flamingo layers are not initialized. Please call `init_flamingo` first."
             )
 
         media_locations = text_inputs == self.media_token_id
         attend_previous = False
 
-        for layer in self.language_model.get_decoder().layers:
+        for layer in self.lang_encoder.get_decoder().layers:
             layer.condition_media_locations(media_locations)
             layer.condition_attend_previous(attend_previous)
 
-        print(f'===> start generation ...')
-        print(f'===> text device: {text_inputs.device}')
-        print(f'===> attention_mask device: {attention_mask.device}')
-        output = self.language_model.generate(
+        output = self.lang_encoder.generate(
             text_inputs,
             attention_mask=attention_mask,
             eos_token_id=self.end_chunk_token_id,
             num_beams=num_beams,
             max_new_tokens=max_new_tokens,
             temperature=temperature,
             top_k=top_k,
@@ -167,15 +168,15 @@
             no_repeat_ngram_size=no_repeat_ngram_size,
             length_penalty=length_penalty,
             num_return_sequences=num_return_sequences,
             do_sample=do_sample,
             early_stopping=early_stopping,
         )
 
-        self.language_model.clear_conditioned_layers()
+        self.lang_encoder.clear_conditioned_layers()
         return output
 
     def _vision_encode(self, vision_inputs: 'torch.Tensor') -> 'torch.Tensor':
         """
         Compute media tokens from vision input by passing it through vision encoder and conditioning language model.
 
         :param vision_inputs: vision images input with shape (B, T, F, channels, height, width).
@@ -188,28 +189,20 @@
 
         assert (
             vision_inputs.ndim == 6
         ), "vision_inputs should be of shape (B, T, F, Channels, Height, Width)"
         B, T, F = vision_inputs.shape[:3]
         assert F == 1, "Only single frame supported"
 
-        # device = next(iter(self.vision_encoder.parameters())).device
-        # print(f'===> encoder device: {device}')
-        vision_inputs = vision_inputs.to('cuda')
-
         vision_x = rearrange(vision_inputs, "B T F c h w -> (B T F) c h w")
 
         with torch.no_grad():
             vision_x = self.vision_encoder.visual(vision_x)[1]
 
         vision_x = rearrange(vision_x, "(B T F) v d -> B T F v d", B=B, T=T, F=F)
 
         vision_x = self.perceiver(vision_x)  # reshapes to (B, T, n, d)
 
-        # device = next(iter(self.language_model.parameters())).device
-
-        vision_x = vision_x.to('cuda')
-
-        for layer in self.language_model._get_decoder_layers():
+        for layer in self.lang_encoder._get_decoder_layers():
             layer.condition_vis_x(vision_x)
 
         return vision_x
```

### Comparing `open_gpt_torch-0.0.1rc3/open_gpt/models/flan/loading.py` & `open_gpt_torch-0.0.1rc4/open_gpt/models/flan/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc3/open_gpt/models/pythia/loading.py` & `open_gpt_torch-0.0.1rc4/open_gpt/models/pythia/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc3/open_gpt/profile.py` & `open_gpt_torch-0.0.1rc4/open_gpt/profile.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc3/open_gpt/serve.py` & `open_gpt_torch-0.0.1rc4/open_gpt/serve.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc3/pyproject.toml` & `open_gpt_torch-0.0.1rc4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open_gpt_torch"
-version = "0.0.1rc3"
+version = "0.0.1rc4"
 description = "An open-source implementation of large-scale language model (LLM)."
 
 license = "Apache-2.0"
 
 authors = [
     "Felix Wang <felix.wang@jina.ai>"
 ]
@@ -32,15 +32,15 @@
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 # Compatible Python versions
 python = ">=3.8"
-# torch = "^1.9,<2.0.0" # a meta device requires torch >= 1.9.0
+torch = "<2.0.0" # a meta device requires torch >= 1.9.0
 loguru = "^0.5"
 click = "^8.1.3"
 numpy = "^1.21.2"
 einops = "^0.6.0"
 transformers = "^4.12.5"
 open_clip_torch = "~2.16.0"
 accelerate = "^0.18.0"
```

### Comparing `open_gpt_torch-0.0.1rc3/PKG-INFO` & `open_gpt_torch-0.0.1rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-gpt-torch
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: An open-source implementation of large-scale language model (LLM).
 Home-page: https://open-gpt.jina.ai
 License: Apache-2.0
 Keywords: Pytorch,LLM,GPT
 Author: Felix Wang
 Author-email: felix.wang@jina.ai
 Requires-Python: >=3.8
@@ -24,14 +24,15 @@
 Requires-Dist: accelerate (>=0.18.0,<0.19.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: einops (>=0.6.0,<0.7.0)
 Requires-Dist: loguru (>=0.5,<0.6)
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
 Requires-Dist: open-flamingo (>=0.0,<0.1) ; extra == "flamingo"
 Requires-Dist: open_clip_torch (>=2.16.0,<2.17.0)
+Requires-Dist: torch (<2.0.0)
 Requires-Dist: transformers (>=4.12.5,<5.0.0)
 Project-URL: Repository, https://github.com/jina-ai/open_gpt
 Description-Content-Type: text/markdown
 
 # OpenGPT
 
 `OpenGPT` is an open-source _cloud-native_ large **multi-modal models** (LMMs) serving solution. 
@@ -58,15 +59,15 @@
 You can view our roadmap with features that are planned, started, and completed on the [Roadmap discussion](discussions/categories/roadmap) category.
 
 ## Installation
 
 Install the package with pip:
 
 ```bash
-pip install open_gpts
+pip install open_gpt_torch
 ```
 
 ## Quickstart
 
 ```python
 import open_gpt
```

