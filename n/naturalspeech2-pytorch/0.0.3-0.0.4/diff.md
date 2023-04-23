# Comparing `tmp/naturalspeech2-pytorch-0.0.3.tar.gz` & `tmp/naturalspeech2-pytorch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naturalspeech2-pytorch-0.0.3.tar", last modified: Sat Apr 22 19:10:51 2023, max compression
+gzip compressed data, was "naturalspeech2-pytorch-0.0.4.tar", last modified: Sun Apr 23 16:10:58 2023, max compression
```

## Comparing `naturalspeech2-pytorch-0.0.3.tar` & `naturalspeech2-pytorch-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:10:51.409813 naturalspeech2-pytorch-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 19:10:35.000000 naturalspeech2-pytorch-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-22 19:10:51.409813 naturalspeech2-pytorch-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-22 19:10:35.000000 naturalspeech2-pytorch-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:10:51.409813 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-22 19:10:35.000000 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22955 2023-04-22 19:10:35.000000 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch/naturalspeech2_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:10:51.409813 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-22 19:10:51.000000 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-22 19:10:51.000000 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:10:51.000000 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-22 19:10:51.000000 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-22 19:10:51.000000 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 19:10:51.409813 naturalspeech2-pytorch-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-22 19:10:35.000000 naturalspeech2-pytorch-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:10:58.682590 naturalspeech2-pytorch-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 16:10:47.000000 naturalspeech2-pytorch-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 16:10:58.682590 naturalspeech2-pytorch-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-23 16:10:47.000000 naturalspeech2-pytorch-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:10:58.682590 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-23 16:10:47.000000 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25501 2023-04-23 16:10:47.000000 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch/naturalspeech2_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:10:58.682590 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 16:10:58.000000 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-23 16:10:58.000000 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:10:58.000000 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-23 16:10:58.000000 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 16:10:58.000000 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 16:10:58.682590 naturalspeech2-pytorch-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-23 16:10:47.000000 naturalspeech2-pytorch-0.0.4/setup.py
```

### Comparing `naturalspeech2-pytorch-0.0.3/LICENSE` & `naturalspeech2-pytorch-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `naturalspeech2-pytorch-0.0.3/PKG-INFO` & `naturalspeech2-pytorch-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalspeech2-pytorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: Natural Speech 2 - Pytorch
 Home-page: https://github.com/lucidrains/naturalspeech2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,latent diffusion,speech synthesis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `naturalspeech2-pytorch-0.0.3/README.md` & `naturalspeech2-pytorch-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch/naturalspeech2_pytorch.py` & `naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch/naturalspeech2_pytorch.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,30 @@
     if exists(val):
         return val
     return d() if callable(d) else d
 
 def identity(t, *args, **kwargs):
     return t
 
+# sinusoidal positional embeds
+
+class LearnedSinusoidalPosEmb(nn.Module):
+    def __init__(self, dim):
+        super().__init__()
+        assert (dim % 2) == 0
+        half_dim = dim // 2
+        self.weights = nn.Parameter(torch.randn(half_dim))
+
+    def forward(self, x):
+        x = rearrange(x, 'b -> b 1')
+        freqs = x * rearrange(self.weights, 'd -> 1 d') * 2 * math.pi
+        fouriered = torch.cat((freqs.sin(), freqs.cos()), dim = -1)
+        fouriered = torch.cat((x, fouriered), dim = -1)
+        return fouriered
+
 # model, which is wavenet + transformer
 
 class CausalConv1d(nn.Conv1d):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         kernel_size, = self.kernel_size
         dilation, = self.dilation
@@ -64,25 +80,44 @@
 class WavenetResBlock(nn.Module):
     def __init__(
         self,
         dim,
         *,
         dilation,
         kernel_size = 3,
-        skip_conv = False
+        skip_conv = False,
+        dim_time_mult = None
     ):
         super().__init__()
+
+        self.cond_time = exists(dim_time_mult)
+        self.to_time_cond = None
+
+        if self.cond_time:
+            self.to_time_cond = nn.Linear(dim * dim_time_mult, dim * 2)
+
         self.conv = CausalConv1d(dim, dim, kernel_size, dilation = dilation)
         self.res_conv = CausalConv1d(dim, dim, 1)
         self.skip_conv = CausalConv1d(dim, dim, 1) if skip_conv else None
 
-    def forward(self, x):
+    def forward(self, x, t = None):
+
+        if self.cond_time:
+            assert exists(t)
+            t = self.to_time_cond(t)
+            t = rearrange(t, 'b c -> b c 1')
+            t_gamma, t_beta = t.chunk(2, dim = -2)
+
         res = self.res_conv(x)
 
         x = self.conv(x)
+
+        if self.cond_time:
+            x = x * t_gamma + t_beta
+
         x = x.tanh() * x.sigmoid()
 
         x = x + res
 
         skip = None
         if exists(self.skip_conv):
             skip = self.skip_conv(x)
@@ -93,164 +128,225 @@
 class WavenetStack(nn.Module):
     def __init__(
         self,
         dim,
         *,
         layers,
         kernel_size = 3,
-        has_skip = False
+        has_skip = False,
+        dim_time_mult = None
     ):
         super().__init__()
         dilations = 2 ** torch.arange(layers)
 
         self.has_skip = has_skip
         self.blocks = mlist([])
 
         for dilation in dilations.tolist():
             block = WavenetResBlock(
                 dim = dim,
                 kernel_size = kernel_size,
                 dilation = dilation,
-                skip_conv = has_skip
+                skip_conv = has_skip,
+                dim_time_mult = dim_time_mult
             )
 
             self.blocks.append(block)
 
-    def forward(self, x):
+    def forward(self, x, t):
         residuals = []
         skips = []
 
         if isinstance(x, torch.Tensor):
             x = (x,) * len(self.blocks)
 
         for block_input, block in zip(x, self.blocks):
-            residual, skip = block(block_input)
+            residual, skip = block(block_input, t)
 
             residuals.append(residual)
             skips.append(skip)
 
         if self.has_skip:
             return torch.stack(skips)
 
         return residuals
 
 class Wavenet(nn.Module):
     def __init__(
         self,
         dim,
         *,
-        init_conv_kernel = 3,
         stacks,
-        layers
+        layers,
+        init_conv_kernel = 3,
+        dim_time_mult = None
     ):
         super().__init__()
         self.init_conv = CausalConv1d(dim, dim, init_conv_kernel)
         self.stacks = mlist([])
 
         for ind in range(stacks):
             is_last = ind == (stacks - 1)
 
             stack = WavenetStack(
                 dim,
                 layers = layers,
+                dim_time_mult = dim_time_mult,
                 has_skip = is_last
             )
 
             self.stacks.append(stack)
 
         self.final_conv = CausalConv1d(dim, dim, 1)
 
-    def forward(self, x):
+    def forward(self, x, t = None):
+
         x = self.init_conv(x)
 
         for stack in self.stacks:
-            x = stack(x)
+            x = stack(x, t)
 
         return self.final_conv(x.sum(dim = 0))
 
 class RMSNorm(nn.Module):
-    def __init__(self, dim):
+    def __init__(self, dim, scale = True):
         super().__init__()
         self.scale = dim ** 0.5
-        self.gamma = nn.Parameter(torch.ones(dim))
+        self.gamma = nn.Parameter(torch.ones(dim)) if scale else None
 
     def forward(self, x):
-        return F.normalize(x, dim = -1) * self.scale * self.gamma
+        gamma = default(self.gamma, 1)
+        return F.normalize(x, dim = -1) * self.scale * gamma
 
 class Transformer(nn.Module):
     def __init__(
         self,
         dim,
         *,
         depth,
         dim_head = 64,
         heads = 8,
         ff_mult = 4,
-        ff_causal_conv = False
+        ff_causal_conv = False,
+        dim_time_mult = None
     ):
         super().__init__()
         self.dim = dim
         self.layers = mlist([])
 
+        cond_time = exists(dim_time_mult)
+
+        self.to_time_cond = None
+        self.cond_time = cond_time
+
+        if cond_time:
+            self.to_time_cond = nn.Linear(dim * dim_time_mult, dim * 4)
+
         for _ in range(depth):
             self.layers.append(mlist([
+                RMSNorm(dim, scale = not cond_time),
                 Attention(dim = dim, dim_head = dim_head, heads = heads),
+                RMSNorm(dim, scale = not cond_time),
                 FeedForward(dim = dim, mult = ff_mult, causal_conv = ff_causal_conv)
             ]))
 
         self.to_pred = nn.Sequential(
             RMSNorm(dim),
             nn.Linear(dim, dim, bias = False)
         )
 
     def forward(
         self,
         x,
         times = None
     ):
-        for attn, ff in self.layers:
-            x = attn(x) + x
-            x = ff(x) + x
+        if self.cond_time:
+            assert exists(times)
+            t = self.to_time_cond(times)
+            t = rearrange(t, 'b d -> b 1 d')
+            t_attn_gamma, t_attn_beta, t_ff_gamma, t_ff_beta = t.chunk(4, dim = -1)
+
+        for attn_norm, attn, ff_norm, ff in self.layers:
+            res = x
+            x = attn_norm(x)
+
+            if self.cond_time:
+                x = x * t_attn_gamma + t_attn_beta
+
+            x = attn(x) + res
+
+            res = x
+            x = ff_norm(x)
+
+            if self.cond_time:
+                x = x * t_ff_gamma + t_ff_beta
+
+            x = ff(x) + res
 
         return self.to_pred(x)
 
 class Model(nn.Module):
     def __init__(
         self,
         dim,
         *,
         depth,
         dim_head = 64,
         heads = 8,
         ff_mult = 4,
         wavenet_layers = 8,
-        wavenet_stacks = 4
+        wavenet_stacks = 4,
+        dim_time_mult = 4
     ):
         super().__init__()
+        self.dim = dim
+
+        # time condition
+
+        dim_time = dim * dim_time_mult
+
+        self.to_time_cond = Sequential(
+            LearnedSinusoidalPosEmb(dim),
+            nn.Linear(dim + 1, dim_time),
+            nn.SiLU()
+        )
+
+        # wavenet
+
         self.wavenet = Wavenet(
             dim = dim,
             stacks = wavenet_stacks,
-            layers = wavenet_layers
+            layers = wavenet_layers,
+            dim_time_mult = dim_time_mult
         )
 
+        # transformer
+
         self.transformer = Transformer(
             dim = dim,
             depth = depth,
             dim_head = dim_head,
             heads = heads,
             ff_mult = ff_mult,
-            ff_causal_conv = True
+            ff_causal_conv = True,
+            dim_time_mult = dim_time_mult
         )
 
-    def forward(self, x):
+    def forward(
+        self,
+        x,
+        times
+    ):
+        t = self.to_time_cond(times)
+
         x = rearrange(x, 'b n d -> b d n')
-        x = self.wavenet(x)
+        x = self.wavenet(x, t)
         x = rearrange(x, 'b d n -> b n d')
 
-        x = self.transformer(x)
+        x = self.transformer(x, t)
         return x
 
 # feedforward
 
 class GEGLU(nn.Module):
     def forward(self, x):
         x, gate = x.chunk(2, dim = -1)
@@ -264,15 +360,14 @@
         conv = nn.Sequential(
             Rearrange('b n d -> b d n'),
             CausalConv1d(dim_inner, dim_inner, 3),
             Rearrange('b d n -> b n d'),
         )
 
     return Sequential(
-        RMSNorm(dim),
         nn.Linear(dim, dim_inner * 2),
         GEGLU(),
         conv,
         nn.Linear(dim_inner, dim)
     )
 
 # attention
@@ -287,23 +382,20 @@
     ):
         super().__init__()
         self.scale = dim_head ** -0.5
         self.heads = heads
 
         dim_inner = dim_head * heads
 
-        self.norm = RMSNorm(dim)
         self.to_qkv = nn.Linear(dim, dim_inner * 3, bias = False)
         self.to_out = nn.Linear(dim_inner, dim, bias = False)
 
     def forward(self, x):
         h = self.heads
 
-        x = self.norm(x)
-
         q, k, v = self.to_qkv(x).chunk(3, dim = -1)
         q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> b h n d', h = h), (q, k, v))
 
         q = q * self.scale
 
         sim = einsum('b h i d, b h j d -> b h i j', q, k)
 
@@ -376,15 +468,15 @@
         train_prob_self_cond = 0.9,
         scale = 1.                      # this will be set to < 1. for better convergence when training on higher resolution images
     ):
         super().__init__()
         self.model = model
         self.codec = codec
 
-        assert not exists(codec) or model.dim == codec.codebook_dim, 'transformer model dimension must be equal to codec dimension'
+        assert not exists(codec) or model.dim == codec.codebook_dim, f'transformer model dimension {model.dim} must be equal to codec dimension {codec.codebook_dim}'
 
         self.dim = codec.codebook_dim if exists(codec) else model.dim
 
         assert objective in {'x0', 'eps', 'v'}, 'objective must be either predict x0 or noise'
         self.objective = objective
 
         if noise_schedule == "linear":
```

### Comparing `naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch.egg-info/PKG-INFO` & `naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalspeech2-pytorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: Natural Speech 2 - Pytorch
 Home-page: https://github.com/lucidrains/naturalspeech2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,latent diffusion,speech synthesis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `naturalspeech2-pytorch-0.0.3/setup.py` & `naturalspeech2-pytorch-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'naturalspeech2-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.3',
+  version = '0.0.4',
   license='MIT',
   description = 'Natural Speech 2 - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/naturalspeech2-pytorch',
   keywords = [
```

