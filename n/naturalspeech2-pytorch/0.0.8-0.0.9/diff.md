# Comparing `tmp/naturalspeech2-pytorch-0.0.8.tar.gz` & `tmp/naturalspeech2-pytorch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naturalspeech2-pytorch-0.0.8.tar", last modified: Sun Apr 23 17:25:20 2023, max compression
+gzip compressed data, was "naturalspeech2-pytorch-0.0.9.tar", last modified: Sun Apr 23 17:55:15 2023, max compression
```

## Comparing `naturalspeech2-pytorch-0.0.8.tar` & `naturalspeech2-pytorch-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:25:20.099473 naturalspeech2-pytorch-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 17:25:09.000000 naturalspeech2-pytorch-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 17:25:20.099473 naturalspeech2-pytorch-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-23 17:25:09.000000 naturalspeech2-pytorch-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:25:20.099473 naturalspeech2-pytorch-0.0.8/naturalspeech2_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-23 17:25:09.000000 naturalspeech2-pytorch-0.0.8/naturalspeech2_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-23 17:25:09.000000 naturalspeech2-pytorch-0.0.8/naturalspeech2_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    25834 2023-04-23 17:25:09.000000 naturalspeech2-pytorch-0.0.8/naturalspeech2_pytorch/naturalspeech2_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:25:20.099473 naturalspeech2-pytorch-0.0.8/naturalspeech2_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 17:25:20.000000 naturalspeech2-pytorch-0.0.8/naturalspeech2_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-23 17:25:20.000000 naturalspeech2-pytorch-0.0.8/naturalspeech2_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:25:20.000000 naturalspeech2-pytorch-0.0.8/naturalspeech2_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-23 17:25:20.000000 naturalspeech2-pytorch-0.0.8/naturalspeech2_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 17:25:20.000000 naturalspeech2-pytorch-0.0.8/naturalspeech2_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:25:20.099473 naturalspeech2-pytorch-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-23 17:25:09.000000 naturalspeech2-pytorch-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:55:15.233986 naturalspeech2-pytorch-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 17:55:04.000000 naturalspeech2-pytorch-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 17:55:15.233986 naturalspeech2-pytorch-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-23 17:55:04.000000 naturalspeech2-pytorch-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:55:15.233986 naturalspeech2-pytorch-0.0.9/naturalspeech2_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-23 17:55:04.000000 naturalspeech2-pytorch-0.0.9/naturalspeech2_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-23 17:55:04.000000 naturalspeech2-pytorch-0.0.9/naturalspeech2_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-04-23 17:55:04.000000 naturalspeech2-pytorch-0.0.9/naturalspeech2_pytorch/naturalspeech2_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:55:15.233986 naturalspeech2-pytorch-0.0.9/naturalspeech2_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 17:55:15.000000 naturalspeech2-pytorch-0.0.9/naturalspeech2_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-23 17:55:15.000000 naturalspeech2-pytorch-0.0.9/naturalspeech2_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:55:15.000000 naturalspeech2-pytorch-0.0.9/naturalspeech2_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-23 17:55:15.000000 naturalspeech2-pytorch-0.0.9/naturalspeech2_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 17:55:15.000000 naturalspeech2-pytorch-0.0.9/naturalspeech2_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:55:15.233986 naturalspeech2-pytorch-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-23 17:55:04.000000 naturalspeech2-pytorch-0.0.9/setup.py
```

### Comparing `naturalspeech2-pytorch-0.0.8/LICENSE` & `naturalspeech2-pytorch-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `naturalspeech2-pytorch-0.0.8/PKG-INFO` & `naturalspeech2-pytorch-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalspeech2-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Natural Speech 2 - Pytorch
 Home-page: https://github.com/lucidrains/naturalspeech2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,latent diffusion,speech synthesis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `naturalspeech2-pytorch-0.0.8/README.md` & `naturalspeech2-pytorch-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `naturalspeech2-pytorch-0.0.8/naturalspeech2_pytorch/attend.py` & `naturalspeech2-pytorch-0.0.9/naturalspeech2_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `naturalspeech2-pytorch-0.0.8/naturalspeech2_pytorch/naturalspeech2_pytorch.py` & `naturalspeech2-pytorch-0.0.9/naturalspeech2_pytorch/naturalspeech2_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -471,15 +471,16 @@
         noise_schedule = 'sigmoid',
         objective = 'v',
         schedule_kwargs: dict = dict(),
         time_difference = 0.,
         min_snr_loss_weight = True,
         min_snr_gamma = 5,
         train_prob_self_cond = 0.9,
-        scale = 1.                      # this will be set to < 1. for better convergence when training on higher resolution images
+        rvq_cross_entropy_loss_weight = 0.,    # default this to off until we are sure it is working. not totally sold that this is critical
+        scale = 1.                             # this will be set to < 1. for better convergence when training on higher resolution images
     ):
         super().__init__()
         self.model = model
         self.codec = codec
 
         assert not exists(codec) or model.dim == codec.codebook_dim, f'transformer model dimension {model.dim} must be equal to codec dimension {codec.codebook_dim}'
 
@@ -519,14 +520,18 @@
         self.train_prob_self_cond = train_prob_self_cond
 
         # min snr loss weight
 
         self.min_snr_loss_weight = min_snr_loss_weight
         self.min_snr_gamma = min_snr_gamma
 
+        # weight of the cross entropy loss to residual vq codebooks
+
+        self.rvq_cross_entropy_loss_weight = rvq_cross_entropy_loss_weight
+
     @property
     def device(self):
         return next(self.model.parameters()).device
 
     def get_sampling_timesteps(self, batch, *, device):
         times = torch.linspace(1., 0., self.timesteps + 1, device = device)
         times = repeat(times, 't -> b t', b = batch)
@@ -674,25 +679,26 @@
                 audio = rearrange(audio, 'b 1 n -> b n')
 
         return audio
 
     def forward(
         self,
         audio,
+        codes = None,
         *args,
         **kwargs
     ):
         is_raw_audio = audio.ndim == 2
 
         assert not (is_raw_audio and not exists(self.codec)), 'codec must be passed in if one were to train on raw audio'
 
         if is_raw_audio:
             with torch.no_grad():
                 self.codec.eval()
-                audio, *_ = self.codec(audio, return_encoded = True)
+                audio, codes, _ = self.codec(audio, return_encoded = True)
 
         batch, n, d, device = *audio.shape, self.device
 
         assert d == self.dim, f'codec codebook dimension {d} must match model dimensions {self.dim}'
 
         # sample random times
 
@@ -737,15 +743,33 @@
 
         elif self.objective == 'x0':
             loss_weight = maybe_clipped_snr
 
         elif self.objective == 'v':
             loss_weight = maybe_clipped_snr / (snr + 1)
 
-        return (loss * loss_weight).mean()
+        loss =  (loss * loss_weight).mean()
+
+        # cross entropy loss to codebooks
+
+        if self.rvq_cross_entropy_loss_weight == 0 or not exists(codes):
+            return loss
+
+        if self.objective == 'x0':
+            x_start = pred
+
+        elif self.objective == 'eps':
+            x_start = safe_div(audio - sigma * pred, alpha)
+
+        elif self.objective == 'v':
+            x_start = alpha * audio - sigma * pred
+
+        _, ce_loss = self.codec.rq(x_start, codes)
+
+        return loss + self.rvq_cross_entropy_loss_weight * ce_loss
 
 # trainer
 
 def cycle(dl):
     while True:
         for data in dl:
             yield data
```

### Comparing `naturalspeech2-pytorch-0.0.8/naturalspeech2_pytorch.egg-info/PKG-INFO` & `naturalspeech2-pytorch-0.0.9/naturalspeech2_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalspeech2-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Natural Speech 2 - Pytorch
 Home-page: https://github.com/lucidrains/naturalspeech2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,latent diffusion,speech synthesis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `naturalspeech2-pytorch-0.0.8/setup.py` & `naturalspeech2-pytorch-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'naturalspeech2-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.8',
+  version = '0.0.9',
   license='MIT',
   description = 'Natural Speech 2 - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/naturalspeech2-pytorch',
   keywords = [
```

