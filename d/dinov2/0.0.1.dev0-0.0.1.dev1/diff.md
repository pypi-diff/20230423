# Comparing `tmp/dinov2-0.0.1.dev0-py3-none-any.whl.zip` & `tmp/dinov2-0.0.1.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,61 @@
-Zip file size: 1094 bytes, number of entries: 4
--rw-rw-r--  2.0 unx      363 b- defN 23-Apr-22 22:17 dinov2-0.0.1.dev0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-22 22:17 dinov2-0.0.1.dev0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-22 22:17 dinov2-0.0.1.dev0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      312 b- defN 23-Apr-22 22:17 dinov2-0.0.1.dev0.dist-info/RECORD
-4 files, 774 bytes uncompressed, 480 bytes compressed:  38.0%
+Zip file size: 88013 bytes, number of entries: 59
+-rw-rw-r--  2.0 unx      226 b- defN 23-Apr-22 22:35 dinov2/__init__.py
+-rw-rw-r--  2.0 unx      684 b- defN 23-Apr-22 22:30 dinov2/configs/__init__.py
+-rw-rw-r--  2.0 unx     2568 b- defN 23-Apr-22 22:30 dinov2/configs/ssl_default_config.yaml
+-rw-rw-r--  2.0 unx      444 b- defN 23-Apr-22 22:30 dinov2/data/__init__.py
+-rw-rw-r--  2.0 unx     1001 b- defN 23-Apr-22 22:30 dinov2/data/adapters.py
+-rw-rw-r--  2.0 unx     3980 b- defN 23-Apr-22 22:30 dinov2/data/augmentations.py
+-rw-rw-r--  2.0 unx     2001 b- defN 23-Apr-22 22:30 dinov2/data/collate.py
+-rw-rw-r--  2.0 unx     6714 b- defN 23-Apr-22 22:30 dinov2/data/loaders.py
+-rw-rw-r--  2.0 unx     2948 b- defN 23-Apr-22 22:30 dinov2/data/masking.py
+-rw-rw-r--  2.0 unx     7648 b- defN 23-Apr-22 22:30 dinov2/data/samplers.py
+-rw-rw-r--  2.0 unx     3059 b- defN 23-Apr-22 22:30 dinov2/data/transforms.py
+-rw-rw-r--  2.0 unx      270 b- defN 23-Apr-22 22:30 dinov2/data/datasets/__init__.py
+-rw-rw-r--  2.0 unx      979 b- defN 23-Apr-22 22:30 dinov2/data/datasets/decoders.py
+-rw-rw-r--  2.0 unx     1512 b- defN 23-Apr-22 22:30 dinov2/data/datasets/extended.py
+-rw-rw-r--  2.0 unx     9572 b- defN 23-Apr-22 22:30 dinov2/data/datasets/image_net.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-Apr-22 22:30 dinov2/data/datasets/image_net_22k.py
+-rw-rw-r--  2.0 unx     8579 b- defN 23-Apr-22 22:30 dinov2/distributed/__init__.py
+-rw-rw-r--  2.0 unx      198 b- defN 23-Apr-22 22:30 dinov2/eval/__init__.py
+-rw-rw-r--  2.0 unx    14428 b- defN 23-Apr-22 22:30 dinov2/eval/knn.py
+-rw-rw-r--  2.0 unx    21399 b- defN 23-Apr-22 22:30 dinov2/eval/linear.py
+-rw-rw-r--  2.0 unx    15111 b- defN 23-Apr-22 22:30 dinov2/eval/log_regression.py
+-rw-rw-r--  2.0 unx     3908 b- defN 23-Apr-22 22:30 dinov2/eval/metrics.py
+-rw-rw-r--  2.0 unx     2064 b- defN 23-Apr-22 22:30 dinov2/eval/setup.py
+-rw-rw-r--  2.0 unx     5208 b- defN 23-Apr-22 22:30 dinov2/eval/utils.py
+-rw-rw-r--  2.0 unx     5118 b- defN 23-Apr-22 22:30 dinov2/fsdp/__init__.py
+-rw-rw-r--  2.0 unx      414 b- defN 23-Apr-22 22:30 dinov2/layers/__init__.py
+-rw-rw-r--  2.0 unx     2501 b- defN 23-Apr-22 22:30 dinov2/layers/attention.py
+-rw-rw-r--  2.0 unx     9332 b- defN 23-Apr-22 22:30 dinov2/layers/block.py
+-rw-rw-r--  2.0 unx     2010 b- defN 23-Apr-22 22:30 dinov2/layers/dino_head.py
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Apr-22 22:30 dinov2/layers/drop_path.py
+-rw-rw-r--  2.0 unx      823 b- defN 23-Apr-22 22:30 dinov2/layers/layer_scale.py
+-rw-rw-r--  2.0 unx     1272 b- defN 23-Apr-22 22:30 dinov2/layers/mlp.py
+-rw-rw-r--  2.0 unx     2832 b- defN 23-Apr-22 22:30 dinov2/layers/patch_embed.py
+-rw-rw-r--  2.0 unx     1859 b- defN 23-Apr-22 22:30 dinov2/layers/swiglu_ffn.py
+-rw-rw-r--  2.0 unx     3287 b- defN 23-Apr-22 22:30 dinov2/logging/__init__.py
+-rw-rw-r--  2.0 unx     6223 b- defN 23-Apr-22 22:30 dinov2/logging/helpers.py
+-rw-rw-r--  2.0 unx      317 b- defN 23-Apr-22 22:30 dinov2/loss/__init__.py
+-rw-rw-r--  2.0 unx     3650 b- defN 23-Apr-22 22:30 dinov2/loss/dino_clstoken_loss.py
+-rw-rw-r--  2.0 unx     5721 b- defN 23-Apr-22 22:30 dinov2/loss/ibot_patch_loss.py
+-rw-rw-r--  2.0 unx     1611 b- defN 23-Apr-22 22:30 dinov2/loss/koleo_loss.py
+-rw-rw-r--  2.0 unx     1313 b- defN 23-Apr-22 22:30 dinov2/models/__init__.py
+-rw-rw-r--  2.0 unx    12689 b- defN 23-Apr-22 22:30 dinov2/models/vision_transformer.py
+-rw-rw-r--  2.0 unx      198 b- defN 23-Apr-22 22:30 dinov2/run/__init__.py
+-rw-rw-r--  2.0 unx     3277 b- defN 23-Apr-22 22:30 dinov2/run/submit.py
+-rw-rw-r--  2.0 unx      279 b- defN 23-Apr-22 22:30 dinov2/train/__init__.py
+-rw-rw-r--  2.0 unx    18688 b- defN 23-Apr-22 22:30 dinov2/train/ssl_meta_arch.py
+-rw-rw-r--  2.0 unx    10684 b- defN 23-Apr-22 22:30 dinov2/train/train.py
+-rw-rw-r--  2.0 unx      198 b- defN 23-Apr-22 22:30 dinov2/utils/__init__.py
+-rw-rw-r--  2.0 unx     3013 b- defN 23-Apr-22 22:30 dinov2/utils/cluster.py
+-rw-rw-r--  2.0 unx     2214 b- defN 23-Apr-22 22:30 dinov2/utils/config.py
+-rw-rw-r--  2.0 unx     1107 b- defN 23-Apr-22 22:30 dinov2/utils/dtype.py
+-rw-rw-r--  2.0 unx     3585 b- defN 23-Apr-22 22:30 dinov2/utils/param_groups.py
+-rw-rw-r--  2.0 unx     3242 b- defN 23-Apr-22 22:30 dinov2/utils/utils.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-22 22:35 dinov2-0.0.1.dev1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    11515 b- defN 23-Apr-22 22:35 dinov2-0.0.1.dev1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-22 22:35 dinov2-0.0.1.dev1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       63 b- defN 23-Apr-22 22:35 dinov2-0.0.1.dev1.dist-info/dependency_links.txt
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-22 22:35 dinov2-0.0.1.dev1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4873 b- defN 23-Apr-22 22:35 dinov2-0.0.1.dev1.dist-info/RECORD
+59 files, 261309 bytes uncompressed, 80359 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -1,13 +1,178 @@
-Filename: dinov2-0.0.1.dev0.dist-info/METADATA
+Filename: dinov2/__init__.py
 Comment: 
 
-Filename: dinov2-0.0.1.dev0.dist-info/WHEEL
+Filename: dinov2/configs/__init__.py
 Comment: 
 
-Filename: dinov2-0.0.1.dev0.dist-info/top_level.txt
+Filename: dinov2/configs/ssl_default_config.yaml
 Comment: 
 
-Filename: dinov2-0.0.1.dev0.dist-info/RECORD
+Filename: dinov2/data/__init__.py
+Comment: 
+
+Filename: dinov2/data/adapters.py
+Comment: 
+
+Filename: dinov2/data/augmentations.py
+Comment: 
+
+Filename: dinov2/data/collate.py
+Comment: 
+
+Filename: dinov2/data/loaders.py
+Comment: 
+
+Filename: dinov2/data/masking.py
+Comment: 
+
+Filename: dinov2/data/samplers.py
+Comment: 
+
+Filename: dinov2/data/transforms.py
+Comment: 
+
+Filename: dinov2/data/datasets/__init__.py
+Comment: 
+
+Filename: dinov2/data/datasets/decoders.py
+Comment: 
+
+Filename: dinov2/data/datasets/extended.py
+Comment: 
+
+Filename: dinov2/data/datasets/image_net.py
+Comment: 
+
+Filename: dinov2/data/datasets/image_net_22k.py
+Comment: 
+
+Filename: dinov2/distributed/__init__.py
+Comment: 
+
+Filename: dinov2/eval/__init__.py
+Comment: 
+
+Filename: dinov2/eval/knn.py
+Comment: 
+
+Filename: dinov2/eval/linear.py
+Comment: 
+
+Filename: dinov2/eval/log_regression.py
+Comment: 
+
+Filename: dinov2/eval/metrics.py
+Comment: 
+
+Filename: dinov2/eval/setup.py
+Comment: 
+
+Filename: dinov2/eval/utils.py
+Comment: 
+
+Filename: dinov2/fsdp/__init__.py
+Comment: 
+
+Filename: dinov2/layers/__init__.py
+Comment: 
+
+Filename: dinov2/layers/attention.py
+Comment: 
+
+Filename: dinov2/layers/block.py
+Comment: 
+
+Filename: dinov2/layers/dino_head.py
+Comment: 
+
+Filename: dinov2/layers/drop_path.py
+Comment: 
+
+Filename: dinov2/layers/layer_scale.py
+Comment: 
+
+Filename: dinov2/layers/mlp.py
+Comment: 
+
+Filename: dinov2/layers/patch_embed.py
+Comment: 
+
+Filename: dinov2/layers/swiglu_ffn.py
+Comment: 
+
+Filename: dinov2/logging/__init__.py
+Comment: 
+
+Filename: dinov2/logging/helpers.py
+Comment: 
+
+Filename: dinov2/loss/__init__.py
+Comment: 
+
+Filename: dinov2/loss/dino_clstoken_loss.py
+Comment: 
+
+Filename: dinov2/loss/ibot_patch_loss.py
+Comment: 
+
+Filename: dinov2/loss/koleo_loss.py
+Comment: 
+
+Filename: dinov2/models/__init__.py
+Comment: 
+
+Filename: dinov2/models/vision_transformer.py
+Comment: 
+
+Filename: dinov2/run/__init__.py
+Comment: 
+
+Filename: dinov2/run/submit.py
+Comment: 
+
+Filename: dinov2/train/__init__.py
+Comment: 
+
+Filename: dinov2/train/ssl_meta_arch.py
+Comment: 
+
+Filename: dinov2/train/train.py
+Comment: 
+
+Filename: dinov2/utils/__init__.py
+Comment: 
+
+Filename: dinov2/utils/cluster.py
+Comment: 
+
+Filename: dinov2/utils/config.py
+Comment: 
+
+Filename: dinov2/utils/dtype.py
+Comment: 
+
+Filename: dinov2/utils/param_groups.py
+Comment: 
+
+Filename: dinov2/utils/utils.py
+Comment: 
+
+Filename: dinov2-0.0.1.dev1.dist-info/LICENSE
+Comment: 
+
+Filename: dinov2-0.0.1.dev1.dist-info/METADATA
+Comment: 
+
+Filename: dinov2-0.0.1.dev1.dist-info/WHEEL
+Comment: 
+
+Filename: dinov2-0.0.1.dev1.dist-info/dependency_links.txt
+Comment: 
+
+Filename: dinov2-0.0.1.dev1.dist-info/top_level.txt
+Comment: 
+
+Filename: dinov2-0.0.1.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

