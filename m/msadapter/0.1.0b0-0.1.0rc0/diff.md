# Comparing `tmp/msadapter-0.1.0b0.tar.gz` & `tmp/msadapter-0.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\msadapter-0.1.0b0.tar", last modified: Mon Mar 27 08:54:53 2023, max compression
+gzip compressed data, was "dist\msadapter-0.1.0rc0.tar", last modified: Sun Apr 23 06:32:42 2023, max compression
```

## Comparing `msadapter-0.1.0b0.tar` & `msadapter-0.1.0rc0.tar`

### file list

```diff
@@ -1,292 +1,386 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/
--rw-rw-rw-   0        0        0    11641 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:51.000000 msadapter-0.1.0b0/msadapter/
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:51.000000 msadapter-0.1.0b0/msadapter/pytorch/
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:51.000000 msadapter-0.1.0b0/msadapter/pytorch/autograd/
--rw-rw-rw-   0        0        0     1693 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/autograd/function.py
--rw-rw-rw-   0        0        0      543 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/autograd/variable.py
--rw-rw-rw-   0        0        0      319 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/autograd/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:51.000000 msadapter-0.1.0b0/msadapter/pytorch/common/
--rw-rw-rw-   0        0        0      288 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/common/device.py
--rw-rw-rw-   0        0        0     2342 2023-03-27 08:01:51.000000 msadapter-0.1.0b0/msadapter/pytorch/common/dtype.py
--rw-rw-rw-   0        0        0     2793 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/common/_inner.py
--rw-rw-rw-   0        0        0      707 2023-03-27 08:01:51.000000 msadapter-0.1.0b0/msadapter/pytorch/common/__init__.py
--rw-rw-rw-   0        0        0     1243 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/conflict_functional.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:51.000000 msadapter-0.1.0b0/msadapter/pytorch/cuda/
--rw-rw-rw-   0        0        0      921 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/cuda/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:51.000000 msadapter-0.1.0b0/msadapter/pytorch/fft/
--rw-rw-rw-   0        0        0      710 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/fft/fft.py
--rw-rw-rw-   0        0        0      111 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/fft/__init__.py
--rw-rw-rw-   0        0        0    97936 2023-03-27 08:01:51.000000 msadapter-0.1.0b0/msadapter/pytorch/functional.py
--rw-rw-rw-   0        0        0     3764 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/hub.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:51.000000 msadapter-0.1.0b0/msadapter/pytorch/linalg/
--rw-rw-rw-   0        0        0     2449 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/linalg/linalg.py
--rw-rw-rw-   0        0        0      302 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/linalg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/
--rw-rw-rw-   0        0        0    88545 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/functional.py
--rw-rw-rw-   0        0        0     5280 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/init.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/
--rw-rw-rw-   0        0        0    20371 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/activation.py
--rw-rw-rw-   0        0        0     7954 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/adaptive.py
--rw-rw-rw-   0        0        0    16893 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/batchnorm.py
--rw-rw-rw-   0        0        0      665 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/channelshuffle.py
--rw-rw-rw-   0        0        0    34578 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/container.py
--rw-rw-rw-   0        0        0    30800 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/conv.py
--rw-rw-rw-   0        0        0      831 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/distance.py
--rw-rw-rw-   0        0        0     8874 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/dropout.py
--rw-rw-rw-   0        0        0     1145 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/flatten.py
--rw-rw-rw-   0        0        0     1503 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/fold.py
--rw-rw-rw-   0        0        0     5802 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/linear.py
--rw-rw-rw-   0        0        0    13085 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/loss.py
--rw-rw-rw-   0        0        0    12797 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/module.py
--rw-rw-rw-   0        0        0     5199 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/normalization.py
--rw-rw-rw-   0        0        0    10627 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/padding.py
--rw-rw-rw-   0        0        0      908 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/pixel_shuffle.py
--rw-rw-rw-   0        0        0    17187 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/pooling.py
--rw-rw-rw-   0        0        0    22674 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/rnn.py
--rw-rw-rw-   0        0        0     3901 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/sparse.py
--rw-rw-rw-   0        0        0        0 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/transformer.py
--rw-rw-rw-   0        0        0     1384 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/unpooling.py
--rw-rw-rw-   0        0        0     3279 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/upsampling.py
--rw-rw-rw-   0        0        0     3880 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/utils.py
--rw-rw-rw-   0        0        0     3711 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/modules/__init__.py
--rw-rw-rw-   0        0        0    15449 2023-03-27 03:19:46.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/parameter.py
--rw-rw-rw-   0        0        0      250 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:52.000000 msadapter-0.1.0b0/msadapter/pytorch/optim/
--rw-rw-rw-   0        0        0     1174 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/optim/__init__.py
--rw-rw-rw-   0        0        0      300 2023-03-27 08:20:24.000000 msadapter-0.1.0b0/msadapter/pytorch/package_info.py
--rw-rw-rw-   0        0        0      261 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/random.py
--rw-rw-rw-   0        0        0     2073 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/serialization.py
--rw-rw-rw-   0        0        0     1508 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/storage.py
--rw-rw-rw-   0        0        0   129042 2023-03-27 08:20:24.000000 msadapter-0.1.0b0/msadapter/pytorch/tensor.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:52.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:52.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/
--rw-rw-rw-   0        0        0      217 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/backward_compatibility.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/communication/
--rw-rw-rw-   0        0        0     2864 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/communication/eventloop.py
--rw-rw-rw-   0        0        0     6760 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/communication/iter.py
--rw-rw-rw-   0        0        0     6275 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/communication/map.py
--rw-rw-rw-   0        0        0     1246 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/communication/messages.py
--rw-rw-rw-   0        0        0     8517 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/communication/protocol.py
--rw-rw-rw-   0        0        0     1452 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/communication/queue.py
--rw-rw-rw-   0        0        0      133 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/communication/__init__.py
--rw-rw-rw-   0        0        0    53721 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/dataloader.py
--rw-rw-rw-   0        0        0     7342 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/dataloader_experimental.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/dataframe/
--rw-rw-rw-   0        0        0     9141 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/dataframe/dataframes.py
--rw-rw-rw-   0        0        0     2993 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/dataframe/dataframe_wrapper.py
--rw-rw-rw-   0        0        0     4478 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/dataframe/datapipes.py
--rw-rw-rw-   0        0        0      573 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/dataframe/structures.py
--rw-rw-rw-   0        0        0      370 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/dataframe/__init__.py
--rw-rw-rw-   0        0        0    15969 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/datapipe.py
--rw-rw-rw-   0        0        0    10154 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/gen_pyi.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/
--rw-rw-rw-   0        0        0     6639 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/callable.py
--rw-rw-rw-   0        0        0     6497 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/combinatorics.py
--rw-rw-rw-   0        0        0    22823 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/combining.py
--rw-rw-rw-   0        0        0     2568 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/filelister.py
--rw-rw-rw-   0        0        0     3423 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/fileopener.py
--rw-rw-rw-   0        0        0    12923 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/grouping.py
--rw-rw-rw-   0        0        0     2843 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/routeddecoder.py
--rw-rw-rw-   0        0        0     3928 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/selecting.py
--rw-rw-rw-   0        0        0     1396 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/streamreader.py
--rw-rw-rw-   0        0        0     1838 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/utils.py
--rw-rw-rw-   0        0        0     2136 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/map/
--rw-rw-rw-   0        0        0     1880 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/map/callable.py
--rw-rw-rw-   0        0        0     2453 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/map/combinatorics.py
--rw-rw-rw-   0        0        0     3854 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/map/combining.py
--rw-rw-rw-   0        0        0     2658 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/map/grouping.py
--rw-rw-rw-   0        0        0     1577 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/map/utils.py
--rw-rw-rw-   0        0        0      732 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/map/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/utils/
--rw-rw-rw-   0        0        0     8258 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/utils/common.py
--rw-rw-rw-   0        0        0    11353 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/utils/decoder.py
--rw-rw-rw-   0        0        0        0 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/utils/__init__.py
--rw-rw-rw-   0        0        0     7932 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/_decorator.py
--rw-rw-rw-   0        0        0    25355 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/_typing.py
--rw-rw-rw-   0        0        0       64 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/__init__.py
--rw-rw-rw-   0        0        0    13840 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/dataset.py
--rw-rw-rw-   0        0        0     6458 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/distributed.py
--rw-rw-rw-   0        0        0     3236 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/graph.py
--rw-rw-rw-   0        0        0     2740 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/graph_settings.py
--rw-rw-rw-   0        0        0    11003 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/sampler.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/_utils/
--rw-rw-rw-   0        0        0    16232 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/_utils/collate.py
--rw-rw-rw-   0        0        0     1978 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/_utils/fetch.py
--rw-rw-rw-   0        0        0     2842 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/_utils/pin_memory.py
--rw-rw-rw-   0        0        0    10347 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/_utils/queue.py
--rw-rw-rw-   0        0        0      446 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/_utils/serialization.py
--rw-rw-rw-   0        0        0     3687 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/_utils/signal_handling.py
--rw-rw-rw-   0        0        0    13959 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/_utils/worker.py
--rw-rw-rw-   0        0        0     1889 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/_utils/__init__.py
--rw-rw-rw-   0        0        0     1844 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/data/__init__.py
--rw-rw-rw-   0        0        0       42 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:51.000000 msadapter-0.1.0b0/msadapter/pytorch/_ref/
--rw-rw-rw-   0        0        0      619 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/_ref/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:51.000000 msadapter-0.1.0b0/msadapter/pytorch/_register/
--rw-rw-rw-   0        0        0     1567 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/_register/getitem_impl.py
--rw-rw-rw-   0        0        0     6927 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/_register/register_multitype_ops.py
--rw-rw-rw-   0        0        0     2720 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/_register/register_standard_method.py
--rw-rw-rw-   0        0        0     8407 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/_register/register_utils.py
--rw-rw-rw-   0        0        0     2861 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/_register/__init__.py
--rw-rw-rw-   0        0        0       31 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/_six.py
--rw-rw-rw-   0        0        0     1120 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/_utils.py
--rw-rw-rw-   0        0        0     1955 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/pytorch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/torchvision/
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/
--rw-rw-rw-   0        0        0     9543 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/caltech.py
--rw-rw-rw-   0        0        0     9835 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/celeba.py
--rw-rw-rw-   0        0        0     6020 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/cifar.py
--rw-rw-rw-   0        0        0    10458 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/cityscapes.py
--rw-rw-rw-   0        0        0     3504 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/clevr.py
--rw-rw-rw-   0        0        0     4076 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/coco.py
--rw-rw-rw-   0        0        0     2466 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/country211.py
--rw-rw-rw-   0        0        0     4039 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/dtd.py
--rw-rw-rw-   0        0        0     2111 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/eurosat.py
--rw-rw-rw-   0        0        0     2675 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/fakedata.py
--rw-rw-rw-   0        0        0     2858 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/fer2013.py
--rw-rw-rw-   0        0        0     4675 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/fgvc_aircraft.py
--rw-rw-rw-   0        0        0     5505 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/flickr.py
--rw-rw-rw-   0        0        0     4714 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/flowers102.py
--rw-rw-rw-   0        0        0    12256 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/folder.py
--rw-rw-rw-   0        0        0     3806 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/food101.py
--rw-rw-rw-   0        0        0     3845 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/gtsrb.py
--rw-rw-rw-   0        0        0     6005 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/hmdb51.py
--rw-rw-rw-   0        0        0     8666 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/imagenet.py
--rw-rw-rw-   0        0        0    10348 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/inaturalist.py
--rw-rw-rw-   0        0        0    13732 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/kinetics.py
--rw-rw-rw-   0        0        0     5758 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/kitti.py
--rw-rw-rw-   0        0        0    10537 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/lfw.py
--rw-rw-rw-   0        0        0     5842 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/lsun.py
--rw-rw-rw-   0        0        0    21873 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/mnist.py
--rw-rw-rw-   0        0        0     4193 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/omniglot.py
--rw-rw-rw-   0        0        0     5197 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/oxford_iiit_pet.py
--rw-rw-rw-   0        0        0     5518 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/pcam.py
--rw-rw-rw-   0        0        0     8512 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/phototour.py
--rw-rw-rw-   0        0        0     7371 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/places365.py
--rw-rw-rw-   0        0        0     3643 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/rendered_sst2.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/samplers/
--rw-rw-rw-   0        0        0     6706 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/samplers/clip_sampler.py
--rw-rw-rw-   0        0        0      164 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/samplers/__init__.py
--rw-rw-rw-   0        0        0     5325 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/sbd.py
--rw-rw-rw-   0        0        0     4317 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/sbu.py
--rw-rw-rw-   0        0        0     3179 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/semeion.py
--rw-rw-rw-   0        0        0     4964 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/stanford_cars.py
--rw-rw-rw-   0        0        0     7470 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/stl10.py
--rw-rw-rw-   0        0        0     2819 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/sun397.py
--rw-rw-rw-   0        0        0     4895 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/svhn.py
--rw-rw-rw-   0        0        0     5546 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/ucf101.py
--rw-rw-rw-   0        0        0     3535 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/usps.py
--rw-rw-rw-   0        0        0    17743 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/utils.py
--rw-rw-rw-   0        0        0    17624 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/video_utils.py
--rw-rw-rw-   0        0        0     4330 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/vision.py
--rw-rw-rw-   0        0        0     9580 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/voc.py
--rw-rw-rw-   0        0        0     8508 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/widerface.py
--rw-rw-rw-   0        0        0    19338 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/_optical_flow.py
--rw-rw-rw-   0        0        0     2662 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/datasets/__init__.py
--rw-rw-rw-   0        0        0     3287 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/extension.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/torchvision/io/
--rw-rw-rw-   0        0        0    10212 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/io/image.py
--rw-rw-rw-   0        0        0    15836 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/io/video.py
--rw-rw-rw-   0        0        0     7115 2023-03-27 08:01:51.000000 msadapter-0.1.0b0/msadapter/torchvision/io/video_reader.py
--rw-rw-rw-   0        0        0      224 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/io/_load_gpu_decoder.py
--rw-rw-rw-   0        0        0    20289 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/io/_video_opt.py
--rw-rw-rw-   0        0        0     1635 2023-03-27 08:01:51.000000 msadapter-0.1.0b0/msadapter/torchvision/io/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/torchvision/models/
--rw-rw-rw-   0        0        0     2222 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/alexnet.py
--rw-rw-rw-   0        0        0    12928 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/densenet.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/torchvision/models/detection/
--rw-rw-rw-   0        0        0    11887 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/detection/anchor_utils.py
--rw-rw-rw-   0        0        0     8006 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/detection/backbone_utils.py
--rw-rw-rw-   0        0        0    23338 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/detection/faster_rcnn.py
--rw-rw-rw-   0        0        0     4679 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/detection/generalized_rcnn.py
--rw-rw-rw-   0        0        0      800 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/detection/image_list.py
--rw-rw-rw-   0        0        0    18548 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/detection/keypoint_rcnn.py
--rw-rw-rw-   0        0        0    18177 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/detection/mask_rcnn.py
--rw-rw-rw-   0        0        0    28227 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/detection/retinanet.py
--rw-rw-rw-   0        0        0    34737 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/detection/roi_heads.py
--rw-rw-rw-   0        0        0    15780 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/detection/rpn.py
--rw-rw-rw-   0        0        0    27587 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/detection/ssd.py
--rw-rw-rw-   0        0        0    10765 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/detection/ssdlite.py
--rw-rw-rw-   0        0        0    12324 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/detection/transform.py
--rw-rw-rw-   0        0        0    16497 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/detection/_utils.py
--rw-rw-rw-   0        0        0      154 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/detection/__init__.py
--rw-rw-rw-   0        0        0    12044 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/googlenet.py
--rw-rw-rw-   0        0        0    17699 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/inception.py
--rw-rw-rw-   0        0        0    11625 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/mnasnet.py
--rw-rw-rw-   0        0        0      199 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/mobilenet.py
--rw-rw-rw-   0        0        0     8103 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/mobilenetv2.py
--rw-rw-rw-   0        0        0    12228 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/mobilenetv3.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/torchvision/models/quantization/
--rw-rw-rw-   0        0        0      301 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/quantization/googlenet.py
--rw-rw-rw-   0        0        0      321 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/quantization/inception.py
--rw-rw-rw-   0        0        0      203 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/quantization/mobilenet.py
--rw-rw-rw-   0        0        0      309 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/quantization/mobilenetv2.py
--rw-rw-rw-   0        0        0      323 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/quantization/mobilenetv3.py
--rw-rw-rw-   0        0        0      545 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/quantization/resnet.py
--rw-rw-rw-   0        0        0      734 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/quantization/shufflenetv2.py
--rw-rw-rw-   0        0        0      130 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/quantization/__init__.py
--rw-rw-rw-   0        0        0    15558 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/resnet.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/torchvision/models/segmentation/
--rw-rw-rw-   0        0        0     3131 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/segmentation/deeplabv3.py
--rw-rw-rw-   0        0        0     1207 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/segmentation/fcn.py
--rw-rw-rw-   0        0        0     2583 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/segmentation/lraspp.py
--rw-rw-rw-   0        0        0     8976 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/segmentation/segmentation.py
--rw-rw-rw-   0        0        0     1084 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/segmentation/_utils.py
--rw-rw-rw-   0        0        0       98 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/segmentation/__init__.py
--rw-rw-rw-   0        0        0     8648 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/shufflenetv2.py
--rw-rw-rw-   0        0        0     5868 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/squeezenet.py
--rw-rw-rw-   0        0        0     7412 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/utils.py
--rw-rw-rw-   0        0        0     7741 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/vgg.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/torchvision/models/video/
--rw-rw-rw-   0        0        0    11271 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/video/resnet.py
--rw-rw-rw-   0        0        0       23 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/video/__init__.py
--rw-rw-rw-   0        0        0     2684 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/_utils.py
--rw-rw-rw-   0        0        0      466 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/
--rw-rw-rw-   0        0        0    14968 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/boxes.py
--rw-rw-rw-   0        0        0     2757 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/ciou_loss.py
--rw-rw-rw-   0        0        0     7524 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/deform_conv.py
--rw-rw-rw-   0        0        0     3188 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/diou_loss.py
--rw-rw-rw-   0        0        0     6011 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/drop_block.py
--rw-rw-rw-   0        0        0     7799 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/feature_pyramid_network.py
--rw-rw-rw-   0        0        0     2045 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/focal_loss.py
--rw-rw-rw-   0        0        0     2506 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/giou_loss.py
--rw-rw-rw-   0        0        0    12389 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/misc.py
--rw-rw-rw-   0        0        0    12092 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/poolers.py
--rw-rw-rw-   0        0        0     3467 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/ps_roi_align.py
--rw-rw-rw-   0        0        0     3151 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/ps_roi_pool.py
--rw-rw-rw-   0        0        0     4480 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/roi_align.py
--rw-rw-rw-   0        0        0     2643 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/roi_pool.py
--rw-rw-rw-   0        0        0     2085 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/stochastic_depth.py
--rw-rw-rw-   0        0        0     2520 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/_box_convert.py
--rw-rw-rw-   0        0        0     3992 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/_utils.py
--rw-rw-rw-   0        0        0     1968 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/ops/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/msadapter/torchvision/transforms/
--rw-rw-rw-   0        0        0    30034 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/transforms/autoaugment.py
--rw-rw-rw-   0        0        0    67500 2023-03-27 08:01:51.000000 msadapter-0.1.0b0/msadapter/torchvision/transforms/functional.py
--rw-rw-rw-   0        0        0    13644 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/transforms/functional_pil.py
--rw-rw-rw-   0        0        0    38427 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/transforms/functional_tensor.py
--rw-rw-rw-   0        0        0    96834 2023-03-27 03:19:46.000000 msadapter-0.1.0b0/msadapter/torchvision/transforms/transforms.py
--rw-rw-rw-   0        0        0     4125 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/transforms/_functional_video.py
--rw-rw-rw-   0        0        0      843 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/transforms/_pil_constants.py
--rw-rw-rw-   0        0        0     8296 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/transforms/_presets.py
--rw-rw-rw-   0        0        0     5183 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/transforms/_transforms_video.py
--rw-rw-rw-   0        0        0       55 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/transforms/__init__.py
--rw-rw-rw-   0        0        0    20994 2023-03-27 08:01:51.000000 msadapter-0.1.0b0/msadapter/torchvision/utils.py
--rw-rw-rw-   0        0        0     2131 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/_internally_replaced_utils.py
--rw-rw-rw-   0        0        0      966 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/torchvision/_utils.py
--rw-rw-rw-   0        0        0     2847 2023-03-27 08:01:51.000000 msadapter-0.1.0b0/msadapter/torchvision/__init__.py
--rw-rw-rw-   0        0        0     2950 2023-03-27 08:01:51.000000 msadapter-0.1.0b0/msadapter/utils.py
--rw-rw-rw-   0        0        0      152 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/msadapter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 08:54:51.000000 msadapter-0.1.0b0/msadapter.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-27 08:54:50.000000 msadapter-0.1.0b0/msadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4381 2023-03-27 08:54:50.000000 msadapter-0.1.0b0/msadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11268 2023-03-27 08:54:50.000000 msadapter-0.1.0b0/msadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-03-27 08:54:50.000000 msadapter-0.1.0b0/msadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4381 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/PKG-INFO
--rw-rw-rw-   0        0        0     3248 2023-03-24 07:06:51.000000 msadapter-0.1.0b0/README.rst
--rw-rw-rw-   0        0        0       42 2023-03-27 08:54:53.000000 msadapter-0.1.0b0/setup.cfg
--rw-rw-rw-   0        0        0     2678 2023-03-27 08:25:23.000000 msadapter-0.1.0b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/
+-rw-rw-rw-   0        0        0    11641 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:41.000000 msadapter-0.1.0rc0/msadapter/
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:41.000000 msadapter-0.1.0rc0/msadapter/pytorch/
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:41.000000 msadapter-0.1.0rc0/msadapter/pytorch/autograd/
+-rw-rw-rw-   0        0        0     1693 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/autograd/function.py
+-rw-rw-rw-   0        0        0      543 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/autograd/variable.py
+-rw-rw-rw-   0        0        0      319 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/autograd/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:41.000000 msadapter-0.1.0rc0/msadapter/pytorch/common/
+-rw-rw-rw-   0        0        0      288 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/common/device.py
+-rw-rw-rw-   0        0        0     2342 2023-03-27 08:01:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/common/dtype.py
+-rw-rw-rw-   0        0        0     2803 2023-04-20 07:18:55.000000 msadapter-0.1.0rc0/msadapter/pytorch/common/_inner.py
+-rw-rw-rw-   0        0        0      707 2023-03-27 08:01:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/common/__init__.py
+-rw-rw-rw-   0        0        0     1243 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/conflict_functional.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:41.000000 msadapter-0.1.0rc0/msadapter/pytorch/cuda/
+-rw-rw-rw-   0        0        0     1006 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/pytorch/cuda/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:41.000000 msadapter-0.1.0rc0/msadapter/pytorch/fft/
+-rw-rw-rw-   0        0        0      710 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/fft/fft.py
+-rw-rw-rw-   0        0        0      111 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/fft/__init__.py
+-rw-rw-rw-   0        0        0   100140 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/pytorch/functional.py
+-rw-rw-rw-   0        0        0     3764 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/hub.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:41.000000 msadapter-0.1.0rc0/msadapter/pytorch/linalg/
+-rw-rw-rw-   0        0        0     6480 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/pytorch/linalg/linalg.py
+-rw-rw-rw-   0        0        0      482 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/pytorch/linalg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:41.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/
+-rw-rw-rw-   0        0        0    93153 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/functional.py
+-rw-rw-rw-   0        0        0     5280 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/init.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/
+-rw-rw-rw-   0        0        0    22082 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/activation.py
+-rw-rw-rw-   0        0        0     8129 2023-04-20 07:18:55.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/adaptive.py
+-rw-rw-rw-   0        0        0    17059 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/batchnorm.py
+-rw-rw-rw-   0        0        0      665 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/channelshuffle.py
+-rw-rw-rw-   0        0        0    39051 2023-04-20 07:18:55.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/container.py
+-rw-rw-rw-   0        0        0    27414 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/conv.py
+-rw-rw-rw-   0        0        0      831 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/distance.py
+-rw-rw-rw-   0        0        0     8874 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/dropout.py
+-rw-rw-rw-   0        0        0     1145 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/flatten.py
+-rw-rw-rw-   0        0        0     1503 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/fold.py
+-rw-rw-rw-   0        0        0     5658 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/linear.py
+-rw-rw-rw-   0        0        0    12848 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/loss.py
+-rw-rw-rw-   0        0        0    26532 2023-04-14 07:20:16.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/module.py
+-rw-rw-rw-   0        0        0     5199 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/normalization.py
+-rw-rw-rw-   0        0        0    10890 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/padding.py
+-rw-rw-rw-   0        0        0      908 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/pixel_shuffle.py
+-rw-rw-rw-   0        0        0    14859 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/pooling.py
+-rw-rw-rw-   0        0        0    22114 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/rnn.py
+-rw-rw-rw-   0        0        0     3901 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/sparse.py
+-rw-rw-rw-   0        0        0    13056 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/transformer.py
+-rw-rw-rw-   0        0        0     1384 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/unpooling.py
+-rw-rw-rw-   0        0        0     3279 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/upsampling.py
+-rw-rw-rw-   0        0        0     3946 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/utils.py
+-rw-rw-rw-   0        0        0     3879 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/__init__.py
+-rw-rw-rw-   0        0        0    15537 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/parameter.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/utils/
+-rw-rw-rw-   0        0        0     1448 2023-04-14 07:20:16.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/utils/rnn.py
+-rw-rw-rw-   0        0        0      108 2023-04-14 07:20:16.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/utils/__init__.py
+-rw-rw-rw-   0        0        0      292 2023-04-14 07:20:16.000000 msadapter-0.1.0rc0/msadapter/pytorch/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/pytorch/optim/
+-rw-rw-rw-   0        0        0     1174 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/optim/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-23 06:31:12.000000 msadapter-0.1.0rc0/msadapter/pytorch/package_info.py
+-rw-rw-rw-   0        0        0      261 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/random.py
+-rw-rw-rw-   0        0        0     2073 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/serialization.py
+-rw-rw-rw-   0        0        0     1508 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/storage.py
+-rw-rw-rw-   0        0        0   135120 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/pytorch/tensor.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/
+-rw-rw-rw-   0        0        0      217 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/backward_compatibility.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/communication/
+-rw-rw-rw-   0        0        0     2864 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/communication/eventloop.py
+-rw-rw-rw-   0        0        0     6760 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/communication/iter.py
+-rw-rw-rw-   0        0        0     6275 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/communication/map.py
+-rw-rw-rw-   0        0        0     1246 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/communication/messages.py
+-rw-rw-rw-   0        0        0     8517 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/communication/protocol.py
+-rw-rw-rw-   0        0        0     1452 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/communication/queue.py
+-rw-rw-rw-   0        0        0      133 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/communication/__init__.py
+-rw-rw-rw-   0        0        0    53721 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/dataloader.py
+-rw-rw-rw-   0        0        0     7342 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/dataloader_experimental.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/dataframe/
+-rw-rw-rw-   0        0        0     9141 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/dataframe/dataframes.py
+-rw-rw-rw-   0        0        0     2993 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/dataframe/dataframe_wrapper.py
+-rw-rw-rw-   0        0        0     4478 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/dataframe/datapipes.py
+-rw-rw-rw-   0        0        0      573 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/dataframe/structures.py
+-rw-rw-rw-   0        0        0      370 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/dataframe/__init__.py
+-rw-rw-rw-   0        0        0    15969 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/datapipe.py
+-rw-rw-rw-   0        0        0    10154 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/gen_pyi.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/
+-rw-rw-rw-   0        0        0     6639 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/callable.py
+-rw-rw-rw-   0        0        0     6497 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/combinatorics.py
+-rw-rw-rw-   0        0        0    22823 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/combining.py
+-rw-rw-rw-   0        0        0     2568 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/filelister.py
+-rw-rw-rw-   0        0        0     3423 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/fileopener.py
+-rw-rw-rw-   0        0        0    12923 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/grouping.py
+-rw-rw-rw-   0        0        0     2843 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/routeddecoder.py
+-rw-rw-rw-   0        0        0     3928 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/selecting.py
+-rw-rw-rw-   0        0        0     1396 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/streamreader.py
+-rw-rw-rw-   0        0        0     1838 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/utils.py
+-rw-rw-rw-   0        0        0     2136 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/map/
+-rw-rw-rw-   0        0        0     1880 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/map/callable.py
+-rw-rw-rw-   0        0        0     2453 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/map/combinatorics.py
+-rw-rw-rw-   0        0        0     3854 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/map/combining.py
+-rw-rw-rw-   0        0        0     2658 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/map/grouping.py
+-rw-rw-rw-   0        0        0     1577 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/map/utils.py
+-rw-rw-rw-   0        0        0      732 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/map/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/utils/
+-rw-rw-rw-   0        0        0     8258 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/utils/common.py
+-rw-rw-rw-   0        0        0    11353 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/utils/decoder.py
+-rw-rw-rw-   0        0        0        0 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/utils/__init__.py
+-rw-rw-rw-   0        0        0     7932 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/_decorator.py
+-rw-rw-rw-   0        0        0    25355 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/_typing.py
+-rw-rw-rw-   0        0        0       64 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/__init__.py
+-rw-rw-rw-   0        0        0    13840 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/dataset.py
+-rw-rw-rw-   0        0        0     6458 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/distributed.py
+-rw-rw-rw-   0        0        0     3236 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/graph.py
+-rw-rw-rw-   0        0        0     2740 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/graph_settings.py
+-rw-rw-rw-   0        0        0    11003 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/sampler.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/_utils/
+-rw-rw-rw-   0        0        0    16232 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/_utils/collate.py
+-rw-rw-rw-   0        0        0     1978 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/_utils/fetch.py
+-rw-rw-rw-   0        0        0     2842 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/_utils/pin_memory.py
+-rw-rw-rw-   0        0        0    10449 2023-04-20 07:18:55.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/_utils/queue.py
+-rw-rw-rw-   0        0        0      446 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/_utils/serialization.py
+-rw-rw-rw-   0        0        0     3687 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/_utils/signal_handling.py
+-rw-rw-rw-   0        0        0    13959 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/_utils/worker.py
+-rw-rw-rw-   0        0        0     1889 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/_utils/__init__.py
+-rw-rw-rw-   0        0        0     1844 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/data/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:41.000000 msadapter-0.1.0rc0/msadapter/pytorch/_ref/
+-rw-rw-rw-   0        0        0      619 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/_ref/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:41.000000 msadapter-0.1.0rc0/msadapter/pytorch/_register/
+-rw-rw-rw-   0        0        0     1567 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/_register/getitem_impl.py
+-rw-rw-rw-   0        0        0     6927 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/_register/register_multitype_ops.py
+-rw-rw-rw-   0        0        0     2720 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/_register/register_standard_method.py
+-rw-rw-rw-   0        0        0     8407 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/_register/register_utils.py
+-rw-rw-rw-   0        0        0     2861 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/_register/__init__.py
+-rw-rw-rw-   0        0        0     1656 2023-04-18 03:05:56.000000 msadapter-0.1.0rc0/msadapter/pytorch/_register_numpy_primitive.py
+-rw-rw-rw-   0        0        0       31 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/_six.py
+-rw-rw-rw-   0        0        0     1120 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/pytorch/_utils.py
+-rw-rw-rw-   0        0        0     1962 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/pytorch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/backend/
+-rw-rw-rw-   0        0        0     1949 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/backend/common.py
+-rw-rw-rw-   0        0        0      747 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/backend/no_backend.py
+-rw-rw-rw-   0        0        0    17175 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/torchaudio/backend/soundfile_backend.py
+-rw-rw-rw-   0        0        0    17442 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/torchaudio/backend/sox_io_backend.py
+-rw-rw-rw-   0        0        0     2517 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/torchaudio/backend/utils.py
+-rw-rw-rw-   0        0        0      148 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/backend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/compliance/
+-rw-rw-rw-   0        0        0    39145 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/compliance/kaldi.py
+-rw-rw-rw-   0        0        0       53 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/compliance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/
+-rw-rw-rw-   0        0        0     7197 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/cmuarctic.py
+-rw-rw-rw-   0        0        0     6394 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/cmudict.py
+-rw-rw-rw-   0        0        0     2598 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/commonvoice.py
+-rw-rw-rw-   0        0        0     4324 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/dr_vctk.py
+-rw-rw-rw-   0        0        0    25270 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/gtzan.py
+-rw-rw-rw-   0        0        0     3722 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/librilight_limited.py
+-rw-rw-rw-   0        0        0     3635 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/librimix.py
+-rw-rw-rw-   0        0        0     5445 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/librispeech.py
+-rw-rw-rw-   0        0        0     5912 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/libritts.py
+-rw-rw-rw-   0        0        0     3557 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/ljspeech.py
+-rw-rw-rw-   0        0        0     3893 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/quesst14.py
+-rw-rw-rw-   0        0        0     6808 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/speechcommands.py
+-rw-rw-rw-   0        0        0     8790 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/tedlium.py
+-rw-rw-rw-   0        0        0     6971 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/utils.py
+-rw-rw-rw-   0        0        0     5763 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/vctk.py
+-rw-rw-rw-   0        0        0     3085 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/yesno.py
+-rw-rw-rw-   0        0        0      791 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/functional/
+-rw-rw-rw-   0        0        0    66050 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/torchaudio/functional/filtering.py
+-rw-rw-rw-   0        0        0    88483 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/torchaudio/functional/functional.py
+-rw-rw-rw-   0        0        0     2135 2023-03-27 03:19:46.000000 msadapter-0.1.0rc0/msadapter/torchaudio/functional/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/io/
+-rw-rw-rw-   0        0        0     3747 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/io/_compat.py
+-rw-rw-rw-   0        0        0    26654 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/io/_stream_reader.py
+-rw-rw-rw-   0        0        0      670 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/io/__init__.py
+-rw-rw-rw-   0        0        0     5352 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/kaldi_io.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/
+-rw-rw-rw-   0        0        0    10897 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/conformer.py
+-rw-rw-rw-   0        0        0    12509 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/conv_tasnet.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/decoder/
+-rw-rw-rw-   0        0        0    13224 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/decoder/_ctc_decoder.py
+-rw-rw-rw-   0        0        0     1036 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/decoder/__init__.py
+-rw-rw-rw-   0        0        0     2999 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/deepspeech.py
+-rw-rw-rw-   0        0        0    39940 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/emformer.py
+-rw-rw-rw-   0        0        0    37770 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/rnnt.py
+-rw-rw-rw-   0        0        0    13753 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/rnnt_decoder.py
+-rw-rw-rw-   0        0        0    48757 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/tacotron2.py
+-rw-rw-rw-   0        0        0     3457 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/wav2letter.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/wav2vec2/
+-rw-rw-rw-   0        0        0    44569 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/wav2vec2/components.py
+-rw-rw-rw-   0        0        0    53501 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/wav2vec2/model.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/wav2vec2/utils/
+-rw-rw-rw-   0        0        0     9981 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/wav2vec2/utils/import_fairseq.py
+-rw-rw-rw-   0        0        0     3309 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/wav2vec2/utils/import_huggingface.py
+-rw-rw-rw-   0        0        0      201 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/wav2vec2/utils/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/wav2vec2/__init__.py
+-rw-rw-rw-   0        0        0    16233 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/wavernn.py
+-rw-rw-rw-   0        0        0     1380 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/pipelines/
+-rw-rw-rw-   0        0        0    14693 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/pipelines/rnnt_pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/pipelines/_tts/
+-rw-rw-rw-   0        0        0    16765 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/pipelines/_tts/impl.py
+-rw-rw-rw-   0        0        0    11948 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/pipelines/_tts/interface.py
+-rw-rw-rw-   0        0        0     5283 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/pipelines/_tts/utils.py
+-rw-rw-rw-   0        0        0      472 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/pipelines/_tts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/pipelines/_wav2vec2/
+-rw-rw-rw-   0        0        0    50379 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/pipelines/_wav2vec2/impl.py
+-rw-rw-rw-   0        0        0     3536 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/pipelines/_wav2vec2/utils.py
+-rw-rw-rw-   0        0        0        0 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/pipelines/_wav2vec2/__init__.py
+-rw-rw-rw-   0        0        0     2139 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/pipelines/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/sox_effects/
+-rw-rw-rw-   0        0        0    12614 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/sox_effects/sox_effects.py
+-rw-rw-rw-   0        0        0      534 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/sox_effects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/transforms/
+-rw-rw-rw-   0        0        0    22717 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/torchaudio/transforms/_multi_channel.py
+-rw-rw-rw-   0        0        0    91176 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/torchaudio/transforms/_transforms.py
+-rw-rw-rw-   0        0        0     1023 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/transforms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/utils/
+-rw-rw-rw-   0        0        0     3086 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/utils/download.py
+-rw-rw-rw-   0        0        0     1833 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/utils/ffmpeg_utils.py
+-rw-rw-rw-   0        0        0     2923 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/utils/sox_utils.py
+-rw-rw-rw-   0        0        0      312 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/utils/__init__.py
+-rw-rw-rw-   0        0        0       86 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/version.py
+-rw-rw-rw-   0        0        0     3848 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/_extension.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchaudio/_internal/
+-rw-rw-rw-   0        0        0     4241 2023-03-27 03:19:46.000000 msadapter-0.1.0rc0/msadapter/torchaudio/_internal/module_utils.py
+-rw-rw-rw-   0        0        0      140 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchaudio/_internal/__init__.py
+-rw-rw-rw-   0        0        0      720 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/msadapter/torchaudio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchvision/
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/
+-rw-rw-rw-   0        0        0     9543 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/caltech.py
+-rw-rw-rw-   0        0        0     9835 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/celeba.py
+-rw-rw-rw-   0        0        0     6020 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/cifar.py
+-rw-rw-rw-   0        0        0    10458 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/cityscapes.py
+-rw-rw-rw-   0        0        0     3504 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/clevr.py
+-rw-rw-rw-   0        0        0     4076 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/coco.py
+-rw-rw-rw-   0        0        0     2466 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/country211.py
+-rw-rw-rw-   0        0        0     4039 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/dtd.py
+-rw-rw-rw-   0        0        0     2111 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/eurosat.py
+-rw-rw-rw-   0        0        0     2675 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/fakedata.py
+-rw-rw-rw-   0        0        0     2858 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/fer2013.py
+-rw-rw-rw-   0        0        0     4675 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/fgvc_aircraft.py
+-rw-rw-rw-   0        0        0     5505 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/flickr.py
+-rw-rw-rw-   0        0        0     4714 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/flowers102.py
+-rw-rw-rw-   0        0        0    12256 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/folder.py
+-rw-rw-rw-   0        0        0     3806 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/food101.py
+-rw-rw-rw-   0        0        0     3845 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/gtsrb.py
+-rw-rw-rw-   0        0        0     6005 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/hmdb51.py
+-rw-rw-rw-   0        0        0     8666 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/imagenet.py
+-rw-rw-rw-   0        0        0    10348 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/inaturalist.py
+-rw-rw-rw-   0        0        0    13732 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/kinetics.py
+-rw-rw-rw-   0        0        0     5758 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/kitti.py
+-rw-rw-rw-   0        0        0    10537 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/lfw.py
+-rw-rw-rw-   0        0        0     5842 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/lsun.py
+-rw-rw-rw-   0        0        0    21873 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/mnist.py
+-rw-rw-rw-   0        0        0     4193 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/omniglot.py
+-rw-rw-rw-   0        0        0     5197 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/oxford_iiit_pet.py
+-rw-rw-rw-   0        0        0     5518 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/pcam.py
+-rw-rw-rw-   0        0        0     8512 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/phototour.py
+-rw-rw-rw-   0        0        0     7371 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/places365.py
+-rw-rw-rw-   0        0        0     3643 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/rendered_sst2.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/samplers/
+-rw-rw-rw-   0        0        0     6706 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/samplers/clip_sampler.py
+-rw-rw-rw-   0        0        0      164 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/samplers/__init__.py
+-rw-rw-rw-   0        0        0     5325 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/sbd.py
+-rw-rw-rw-   0        0        0     4317 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/sbu.py
+-rw-rw-rw-   0        0        0     3179 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/semeion.py
+-rw-rw-rw-   0        0        0     4964 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/stanford_cars.py
+-rw-rw-rw-   0        0        0     7470 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/stl10.py
+-rw-rw-rw-   0        0        0     2819 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/sun397.py
+-rw-rw-rw-   0        0        0     4895 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/svhn.py
+-rw-rw-rw-   0        0        0     5546 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/ucf101.py
+-rw-rw-rw-   0        0        0     3535 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/usps.py
+-rw-rw-rw-   0        0        0    17743 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/utils.py
+-rw-rw-rw-   0        0        0    17624 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/video_utils.py
+-rw-rw-rw-   0        0        0     4330 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/vision.py
+-rw-rw-rw-   0        0        0     9580 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/voc.py
+-rw-rw-rw-   0        0        0     8508 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/widerface.py
+-rw-rw-rw-   0        0        0    19338 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/_optical_flow.py
+-rw-rw-rw-   0        0        0     2662 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/datasets/__init__.py
+-rw-rw-rw-   0        0        0     3287 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/extension.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchvision/io/
+-rw-rw-rw-   0        0        0    10212 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/io/image.py
+-rw-rw-rw-   0        0        0    15836 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/io/video.py
+-rw-rw-rw-   0        0        0     7115 2023-03-27 08:01:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/io/video_reader.py
+-rw-rw-rw-   0        0        0      224 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/io/_load_gpu_decoder.py
+-rw-rw-rw-   0        0        0    20289 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/io/_video_opt.py
+-rw-rw-rw-   0        0        0     1635 2023-03-27 08:01:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/io/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/
+-rw-rw-rw-   0        0        0     2222 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/alexnet.py
+-rw-rw-rw-   0        0        0    12928 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/densenet.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/detection/
+-rw-rw-rw-   0        0        0    11887 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/detection/anchor_utils.py
+-rw-rw-rw-   0        0        0     8006 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/detection/backbone_utils.py
+-rw-rw-rw-   0        0        0    23338 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/detection/faster_rcnn.py
+-rw-rw-rw-   0        0        0     4679 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/detection/generalized_rcnn.py
+-rw-rw-rw-   0        0        0      800 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/detection/image_list.py
+-rw-rw-rw-   0        0        0    18548 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/detection/keypoint_rcnn.py
+-rw-rw-rw-   0        0        0    18177 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/detection/mask_rcnn.py
+-rw-rw-rw-   0        0        0    28227 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/detection/retinanet.py
+-rw-rw-rw-   0        0        0    34737 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/detection/roi_heads.py
+-rw-rw-rw-   0        0        0    15780 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/detection/rpn.py
+-rw-rw-rw-   0        0        0    27587 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/detection/ssd.py
+-rw-rw-rw-   0        0        0    10765 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/detection/ssdlite.py
+-rw-rw-rw-   0        0        0    12324 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/detection/transform.py
+-rw-rw-rw-   0        0        0    16497 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/detection/_utils.py
+-rw-rw-rw-   0        0        0      154 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/detection/__init__.py
+-rw-rw-rw-   0        0        0    12044 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/googlenet.py
+-rw-rw-rw-   0        0        0    17699 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/inception.py
+-rw-rw-rw-   0        0        0    11625 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/mnasnet.py
+-rw-rw-rw-   0        0        0      199 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/mobilenet.py
+-rw-rw-rw-   0        0        0     8103 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/mobilenetv2.py
+-rw-rw-rw-   0        0        0    12228 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/mobilenetv3.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/quantization/
+-rw-rw-rw-   0        0        0      301 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/quantization/googlenet.py
+-rw-rw-rw-   0        0        0      321 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/quantization/inception.py
+-rw-rw-rw-   0        0        0      203 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/quantization/mobilenet.py
+-rw-rw-rw-   0        0        0      309 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/quantization/mobilenetv2.py
+-rw-rw-rw-   0        0        0      323 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/quantization/mobilenetv3.py
+-rw-rw-rw-   0        0        0      545 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/quantization/resnet.py
+-rw-rw-rw-   0        0        0      734 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/quantization/shufflenetv2.py
+-rw-rw-rw-   0        0        0      130 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/quantization/__init__.py
+-rw-rw-rw-   0        0        0    15558 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/resnet.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/segmentation/
+-rw-rw-rw-   0        0        0     3131 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/segmentation/deeplabv3.py
+-rw-rw-rw-   0        0        0     1207 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/segmentation/fcn.py
+-rw-rw-rw-   0        0        0     2583 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/segmentation/lraspp.py
+-rw-rw-rw-   0        0        0     8976 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/segmentation/segmentation.py
+-rw-rw-rw-   0        0        0     1084 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/segmentation/_utils.py
+-rw-rw-rw-   0        0        0       98 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     8648 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/shufflenetv2.py
+-rw-rw-rw-   0        0        0     5868 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/squeezenet.py
+-rw-rw-rw-   0        0        0     7412 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/utils.py
+-rw-rw-rw-   0        0        0     7741 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/vgg.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/video/
+-rw-rw-rw-   0        0        0    11271 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/video/resnet.py
+-rw-rw-rw-   0        0        0       23 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/video/__init__.py
+-rw-rw-rw-   0        0        0     2684 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/_utils.py
+-rw-rw-rw-   0        0        0      466 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/
+-rw-rw-rw-   0        0        0    14968 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/boxes.py
+-rw-rw-rw-   0        0        0     2757 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/ciou_loss.py
+-rw-rw-rw-   0        0        0     7524 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/deform_conv.py
+-rw-rw-rw-   0        0        0     3188 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/diou_loss.py
+-rw-rw-rw-   0        0        0     6011 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/drop_block.py
+-rw-rw-rw-   0        0        0     7799 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/feature_pyramid_network.py
+-rw-rw-rw-   0        0        0     2045 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/focal_loss.py
+-rw-rw-rw-   0        0        0     2506 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/giou_loss.py
+-rw-rw-rw-   0        0        0    12389 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/misc.py
+-rw-rw-rw-   0        0        0    12092 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/poolers.py
+-rw-rw-rw-   0        0        0     3467 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/ps_roi_align.py
+-rw-rw-rw-   0        0        0     3151 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/ps_roi_pool.py
+-rw-rw-rw-   0        0        0     4480 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/roi_align.py
+-rw-rw-rw-   0        0        0     2643 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/roi_pool.py
+-rw-rw-rw-   0        0        0     2085 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/stochastic_depth.py
+-rw-rw-rw-   0        0        0     2520 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/_box_convert.py
+-rw-rw-rw-   0        0        0     3992 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/_utils.py
+-rw-rw-rw-   0        0        0     1968 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/ops/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/msadapter/torchvision/transforms/
+-rw-rw-rw-   0        0        0    30044 2023-04-20 07:18:55.000000 msadapter-0.1.0rc0/msadapter/torchvision/transforms/autoaugment.py
+-rw-rw-rw-   0        0        0    67510 2023-04-20 07:18:55.000000 msadapter-0.1.0rc0/msadapter/torchvision/transforms/functional.py
+-rw-rw-rw-   0        0        0    13654 2023-04-20 07:18:55.000000 msadapter-0.1.0rc0/msadapter/torchvision/transforms/functional_pil.py
+-rw-rw-rw-   0        0        0    38427 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/transforms/functional_tensor.py
+-rw-rw-rw-   0        0        0    96844 2023-04-20 07:18:55.000000 msadapter-0.1.0rc0/msadapter/torchvision/transforms/transforms.py
+-rw-rw-rw-   0        0        0     4125 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/transforms/_functional_video.py
+-rw-rw-rw-   0        0        0      843 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/transforms/_pil_constants.py
+-rw-rw-rw-   0        0        0     8296 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/transforms/_presets.py
+-rw-rw-rw-   0        0        0     5183 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/transforms/_transforms_video.py
+-rw-rw-rw-   0        0        0       55 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/transforms/__init__.py
+-rw-rw-rw-   0        0        0    20994 2023-03-27 08:01:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/utils.py
+-rw-rw-rw-   0        0        0     2131 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/_internally_replaced_utils.py
+-rw-rw-rw-   0        0        0      966 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/_utils.py
+-rw-rw-rw-   0        0        0     2847 2023-03-27 08:01:51.000000 msadapter-0.1.0rc0/msadapter/torchvision/__init__.py
+-rw-rw-rw-   0        0        0     3253 2023-04-23 03:15:04.000000 msadapter-0.1.0rc0/msadapter/utils.py
+-rw-rw-rw-   0        0        0      152 2023-03-24 07:06:51.000000 msadapter-0.1.0rc0/msadapter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:41.000000 msadapter-0.1.0rc0/msadapter.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-23 06:32:41.000000 msadapter-0.1.0rc0/msadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     4393 2023-04-23 06:32:41.000000 msadapter-0.1.0rc0/msadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    14582 2023-04-23 06:32:41.000000 msadapter-0.1.0rc0/msadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 06:32:41.000000 msadapter-0.1.0rc0/msadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4393 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/PKG-INFO
+-rw-rw-rw-   0        0        0     3259 2023-04-11 02:58:52.000000 msadapter-0.1.0rc0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-23 06:32:42.000000 msadapter-0.1.0rc0/setup.cfg
+-rw-rw-rw-   0        0        0     2676 2023-04-23 06:31:12.000000 msadapter-0.1.0rc0/setup.py
```

### Comparing `msadapter-0.1.0b0/LICENSE` & `msadapter-0.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/autograd/function.py` & `msadapter-0.1.0rc0/msadapter/pytorch/autograd/function.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/autograd/variable.py` & `msadapter-0.1.0rc0/msadapter/pytorch/autograd/variable.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/common/dtype.py` & `msadapter-0.1.0rc0/msadapter/pytorch/common/dtype.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/common/_inner.py` & `msadapter-0.1.0rc0/msadapter/pytorch/common/_inner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-from mindspore.ops import constexpr
+from mindspore.ops.primitive import _primexpr
 from msadapter.pytorch.tensor import cast_to_adapter_tensor, Tensor
 from msadapter.utils import pynative_mode_condition, graph_mode_condition
 
 
 def _out_limit_pynative(out, op_name):
     if out is not None and graph_mode_condition():  # TODO: ms_function
         raise ValueError('In MindSpore static graph mode, `out` in `{}` shoud be None, '
@@ -53,15 +53,15 @@
 
         raise ValueError('In MindSpore static graph mode, `inplace` in `{}` shoud not be Ture, '
                          'please set inplace=False and use return value instead of `input`.'.format(op_name))
 
     return cast_to_adapter_tensor(output)
 
 
-@constexpr
+@_primexpr
 def _inplace_limit_pynative(inplace, op_name):
     if inplace is True and graph_mode_condition(): # TODO: ms_function
         raise ValueError('In MindSpore static graph mode, `inplace` in `{}` shoud not be Ture, '
                          'please set inplace=False and use return value instead of `input`.'.format(op_name))
 
 def _inplace_assign(input, inplace, output):
     if inplace is True:
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/common/__init__.py` & `msadapter-0.1.0rc0/msadapter/pytorch/common/__init__.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/conflict_functional.py` & `msadapter-0.1.0rc0/msadapter/pytorch/conflict_functional.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/cuda/__init__.py` & `msadapter-0.1.0rc0/msadapter/pytorch/cuda/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 def device_count():
     # TODO Use this method when supported
     # init()
     # return get_group_size()
     return 1
 
 def set_device(device):
-    if device in ("gpu", 'GPU'):
+    if isinstance(device, int):
+        ms.context.set_context(device_id=device)
+    elif device in ("gpu", 'GPU'):
         ms.context.set_context(device_target="GPU")
     elif device in ("cpu", "CPU"):
         ms.context.set_context(device_target="CPU")
     elif device in ("ascend", "Ascend"):
         ms.context.set_context(device_target="Ascend")
     else:
         raise ValueError("device must be cpu, gpu, ascend or CPU, GPU, Ascend.")
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/fft/fft.py` & `msadapter-0.1.0rc0/msadapter/pytorch/fft/fft.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/functional.py` & `msadapter-0.1.0rc0/msadapter/pytorch/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-import collections
 import warnings
 import numbers
 import math
-from functools import lru_cache
+# from functools import lru_cache
 import numpy as np
 from scipy import signal
 import mindspore as ms
 from mindspore import ops
 from mindspore.common import dtype as mstype
-from mindspore.ops import constexpr
-from mindspore.common.seed import _get_graph_seed
+from mindspore.ops.primitive import _primexpr
 from mindspore.ops._primitive_cache import _get_cache_prim
 
 from msadapter.pytorch.tensor import tensor, cast_to_ms_tensor, cast_to_adapter_tensor
 from msadapter.utils import unsupported_attr, get_backend, pynative_mode_condition, is_under_gpu_context, \
-                             is_under_ascend_context,is_under_cpu_context, _infer_size, _GLOBAL_LRU_CACHE_SIZE
+                             is_under_ascend_context,is_under_cpu_context, _infer_size, \
+                             set_name_tuple
 from msadapter.pytorch.tensor import Tensor as adapter_tensor
 from msadapter.pytorch.common._inner import _out_inplace_assign, _out_limit_pynative, \
                                              _out_inplace_assign_with_adapter_tensor
 from msadapter.pytorch.common.dtype import _TypeDict, all_int_type
 from msadapter.pytorch.common.device import Device
 from msadapter.pytorch.common import pi
 
@@ -183,36 +182,36 @@
     return input.flatten(start_dim, end_dim)
 
 
 def unflatten(input, dim, sizes):
     return input.unflatten(dim, sizes)
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE)
 def _check_transpose_dim(dim, rank):
     if dim >= rank or dim < -rank:
         raise ValueError("dim is out of bound, should be in range [{}, {})"
                 .format(-rank, rank))
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE)
 def _get_transpose_perm(input_shape, dim0, dim1):
     rank = len(input_shape)
     _check_transpose_dim(dim0, rank)
     _check_transpose_dim(dim1, rank)
     _perm = list(range(rank))
     _perm[dim0] = dim1
     _perm[dim1] = dim0
     return tuple(_perm)
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE)
 def _get_transpose_perm_ascend(input_shape, dim0, dim1):
     rank = len(input_shape)
     _check_transpose_dim(dim0, rank)
     _check_transpose_dim(dim1, rank)
     _perm = list(range(rank))
     _dim0 = dim0 if dim0 >=0 else dim0 + rank
     _dim1 = dim1 if dim1 >=0 else dim1 + rank
@@ -224,41 +223,28 @@
 def transpose(input, dim0, dim1):
     if is_under_ascend_context():
         input_ms = cast_to_ms_tensor(input)
         out = ms.ops.transpose(input_ms, _get_transpose_perm_ascend(input.shape, dim0, dim1))
         return cast_to_adapter_tensor(out)
 
     input_ms = cast_to_ms_tensor(input)
-    out = ops.transpose(input_ms, _get_transpose_perm(input.shape, dim0, dim1))
+    if input.nelement() == 0:
+        out_shape = list(input.shape)
+        out_shape[dim0], out_shape[dim1] = out_shape[dim1], out_shape[dim0]
+        out = input.reshape(tuple(out_shape))
+    else:
+        out = ops.transpose(input_ms, _get_transpose_perm(input.shape, dim0, dim1))
     return cast_to_adapter_tensor(out)
 
 
 def multinomial(input, num_samples, replacement=False, *, generator=None, out=None):
     unsupported_attr(generator)
     if generator is not None:
         warnings.warn("torch.multinomal don't support generator now.")
     input_tensor = cast_to_ms_tensor(input).astype(mstype.float32)
-
-    # TODO: Ascend to support 1-dimention input
-    if is_under_ascend_context():
-        _input_rank = len(input.shape)
-        if _input_rank == 1:
-            input_tensor = input_tensor.expand_dims(axis=0)
-        if not replacement:
-            output = ms.ops.multinomial(input_tensor, num_samples, replacement)
-        else:
-            # TODO: Multinomial not support on Ascend
-            seed0, seed1 = _get_graph_seed(None, "multinomial")
-            _op = ms.ops.Multinomial(seed0, seed1)
-            _op.set_device("CPU")
-            output = _op(input_tensor, num_samples)
-        if _input_rank == 1:
-            output = output[0]
-        return _out_inplace_assign(out, output, "multinomial")
-
     output = ms.ops.multinomial(input_tensor, num_samples, replacement)
     return _out_inplace_assign(out, output, "multinomial")
 
 
 def randperm(n, *, generator=None, out=None, dtype=mstype.int64, layout=None, device=None,
              requires_grad=False, pin_memory=False):
     unsupported_attr(generator)
@@ -332,42 +318,43 @@
     unsupported_attr(layout)
     unsupported_attr(device)
     unsupported_attr(requires_grad)
     unsupported_attr(memory_format)
     if dtype is None:
         dtype = ms.float32
     #TODO:replace whith mindspore.ops.empty_like
-    ouput = ms.numpy.empty_like(input, dtype=dtype)
-    return cast_to_adapter_tensor(ouput)
+    output = ms.numpy.empty_like(input, dtype=dtype)
+    return cast_to_adapter_tensor(output)
 
 
 def full(size, fill_value, out=None, dtype=None, layout=None, device=None, requires_grad=False):
     unsupported_attr(layout)
     unsupported_attr(device)
     unsupported_attr(requires_grad)
-    #TODO:replace whith mindspore.ops.full
-    output = ms.numpy.full(size, fill_value, dtype)
+    if dtype is None:
+        dtype = ms.float32
+    output = ms.ops.full(size, fill_value, dtype=dtype)
     return _out_inplace_assign(out, output, "full")
 
 
 def full_like(input, fill_value, dtype=None, layout=None, device=None, requires_grad=False, memory_format=None):
     unsupported_attr(layout)
     unsupported_attr(device)
     unsupported_attr(requires_grad)
     unsupported_attr(memory_format)
-    #TODO:replace whith mindspore.ops.full_like
-    output = ms.numpy.full_like(input, fill_value=fill_value, dtype=dtype)
+    output = ms.ops.full_like(input, fill_value=fill_value, dtype=dtype)
     return cast_to_adapter_tensor(output)
 
 
 def where(condition, x=None, y=None):
     if x is None and y is None:
         return nonzero(condition, as_tuple=True)
-    #TODO: replace with ms.ops.where
-    output = ms.numpy.where(condition, x, y)
+    x = cast_to_ms_tensor(x)
+    y = cast_to_ms_tensor(y)
+    output = ms.ops.where(condition, x, y)
     return cast_to_adapter_tensor(output)
 
 
 def rand(*size, out=None, dtype=None, layout=None, device=None, requires_grad=False, pin_memory=False):
     unsupported_attr(layout)
     unsupported_attr(device)
     unsupported_attr(requires_grad)
@@ -430,35 +417,31 @@
     input = cast_to_ms_tensor(input)
     other = cast_to_ms_tensor(other)
     output = ms.ops.atan2(input, other)
     return _out_inplace_assign(out, output, "atan2")
 
 
 def clamp(input, min=None, max=None, out=None):
-    # TODO:replace whith mindspore.ops.clamp
     input_ms = cast_to_ms_tensor(input)
-    type = input_ms.dtype
-    if min is not None and max is not None and min > max:
-        output = ms.ops.ones_like(input_ms).astype(type)*max
-    else:
-        if min is not None:
-            min = ms.Tensor(min, type)
-        if max is not None:
-            max = ms.Tensor(max, type)
-        output = ms.ops.clip_by_value(input_ms, min, max)
+    if is_under_ascend_context() and input_ms.dtype == ms.float64:
+        input_ms = input_ms.astype(ms.float32)
+        output = ms.ops.clamp(input_ms, min, max)
+        output = output.astype(ms.float64)
+    else:
+        output = ms.ops.clamp(input_ms, min, max)
     return _out_inplace_assign(out, output, "clamp")
 
 
 def cos(input, out=None):
     input = cast_to_ms_tensor(input)
     output = ms.ops.cos(input)
     return _out_inplace_assign(out, output, "cos")
 
 
-@constexpr
+@_primexpr
 def device(type=None, index=None):
     if type is not None:
         if isinstance(type, str):
             if ':' in type:
                 if index is not None:
                     raise ValueError(f"`type` must not include an index because index was passed explicitly: {type}")
                 _target, _id = type.split(':')
@@ -485,18 +468,16 @@
     input = cast_to_ms_tensor(input)
     other = cast_to_ms_tensor(other)
     output = ms.ops.fmod(input, other)
     return _out_inplace_assign(out, output, "fmod")
 
 
 def frac(input, out=None):
-    #TODO outout = input - floor(abs(input)) * sing(input)
     input = cast_to_ms_tensor(input)
-    input = ms.numpy.array(input)
-    output = input - ms.numpy.floor(ms.numpy.abs(input)) * ms.numpy.sign(input)
+    output = ms.ops.frac(input)
     return _out_inplace_assign(out, output, "frac")
 
 
 def log10(input, out=None):
     input = cast_to_ms_tensor(input)
     output = ms.ops.log10(input)
     return _out_inplace_assign(out, output, "log10")
@@ -517,61 +498,65 @@
 def sin(input, out=None):
     input = cast_to_ms_tensor(input)
     output = ms.ops.sin(input)
     return _out_inplace_assign(out, output, "sin")
 
 
 def max(input, dim=None, keepdim=False, *, out=None):
-    #TODO: not supprt GRAPH_MODE, not supper max(input, other)
+    #TODO: not supper max(input, other)
     input = cast_to_ms_tensor(input)
     type = input.dtype
     input = input.astype(ms.float32)
     if dim is None:
         output = input.max(axis=dim, keepdims=keepdim).astype(type)
+        return _out_inplace_assign(out, output, "max")
+    value, indice = ms.ops.max(input, dim, keepdim)
+    value = value.astype(type)
+    if pynative_mode_condition():
+        point = set_name_tuple('max')
+        rlt = point(cast_to_adapter_tensor(value), cast_to_adapter_tensor(indice))
         if out is not None:
-            ops.assign(out, output)
-            return out
-        return cast_to_adapter_tensor(output)
-    output = list(ms.ops.max(input, axis=dim, keep_dims=keepdim))
-    value = output[1].astype(type)
-    indice = output[0]
-    point = collections.namedtuple('max', 'values,indices')
-    rlt = point(cast_to_adapter_tensor(value), cast_to_adapter_tensor(indice))
-    if out is not None:
-        if pynative_mode_condition():
             if len(out) != 2 or not isinstance(out[0], adapter_tensor) or not isinstance(out[1], adapter_tensor):
                 raise TypeError("In msadapter.torch.max(), `out` should be tuple of Tensors.")
             out[0].assign_value(value)
             out[1].assign_value(indice)
             return out
-        else:
-            raise ValueError('In MindSpore static graph mode, `out` in `max` shoud be None, '
-                             'please set out=None and use return value instead of `out`.')
-    return rlt
+        return rlt
+
+    if out is not None:
+        raise ValueError('In MindSpore static graph mode, `out` in `max` shoud be None, '
+            'please set out=None and use return value instead of `out`.')
+    return cast_to_adapter_tensor(value), cast_to_adapter_tensor(indice)
 
 
 def min(input, dim=None, keepdim=False, *, out=None):
     # TODO: Right Now, not support 'min(input, other, *, out=None)'
     input = cast_to_ms_tensor(input)
+    type = input.dtype
+    input = input.astype(ms.float32)
     if dim is None:
-        return cast_to_adapter_tensor(input.min())
-
-    indices, result = ms.ops.min(input, axis=dim, keep_dims=keepdim)
-    if out is not None:
-        if pynative_mode_condition():
+        output = input.min(dim, keepdim).astype(type)
+        return _out_inplace_assign(out, output, "min")
+    result, indices = ms.ops.min(input, dim, keepdim)
+    result = result.astype(type)
+    if pynative_mode_condition():
+        point = set_name_tuple('min')
+        rlt = point(cast_to_adapter_tensor(result), cast_to_adapter_tensor(indices))
+        if out is not None:
             if len(out) != 2 or not isinstance(out[0], adapter_tensor) or not isinstance(out[1], adapter_tensor):
                 raise TypeError("In msadapter.torch.min(), `out` should be tuple of Tensors.")
             out[0].assign_value(result)
             out[1].assign_value(indices)
             return out
-        else:
-            raise ValueError('In MindSpore static graph mode, `out` in `min` shoud be None, '
-                             'please set out=None and use return value instead of `out`.')
-    return cast_to_adapter_tensor(result), cast_to_adapter_tensor(indices)
+        return rlt
 
+    if out is not None:
+        raise ValueError('In MindSpore static graph mode, `out` in `min` shoud be None, '
+                            'please set out=None and use return value instead of `out`.')
+    return cast_to_adapter_tensor(result), cast_to_adapter_tensor(indices)
 
 def fmax(input, other, *, out=None):
     output = input.fmax(other)
     return _out_inplace_assign_with_adapter_tensor(out, output, "fmax")
 
 
 def fmin(input, other, *, out=None):
@@ -682,19 +667,17 @@
     other = cast_to_ms_tensor(other)
     output = ms.ops.matmul(input, other)
     return _out_inplace_assign(out, output, "matmul")
 
 
 def norm(input, p='fro', dim=None, keepdim=False, out=None, dtype=None):
     input = cast_to_ms_tensor(input)
-    #TODO :ms.ops.norm is not ready, ms.numpy.norm function is also not complete.
     if dtype is None:
         dtype = ms.float32
-    input = ms.numpy.array(input, dtype=dtype)
-    output = ms.numpy.norm(input, ord=p, axis=dim, keepdims=keepdim)
+    output = ms.ops.norm(input, ord=p, dim=dim, keepdim=keepdim)
     output = output.astype(dtype)
     return _out_inplace_assign(out, output, "norm")
 
 
 def stft(input, n_fft, hop_length=None, win_length=None, window=None, center=True,
          pad_mode='reflect', normalized=False, onesided=None, return_complex=None):
     unsupported_attr(normalized)
@@ -858,16 +841,15 @@
 
     output = ms.ops.gather(_input_params, _input_indices, _axis)
     return _out_inplace_assign(out, output, "index_select")
 
 def sort(input, dim=-1, descending=False, stable=False, *, out=None):
     unsupported_attr(stable)
     input = cast_to_ms_tensor(input)
-    # TODO: ops.sort() should be replaced.
-    output = ms.ops.Sort(dim, descending)(input)
+    output = ms.ops.sort(input, dim, descending)
     return _out_inplace_assign(out, output, "sort")
 
 
 def msort(input, *, out=None):
     output = input.msort()
     return _out_inplace_assign(out, output, "msort")
 
@@ -889,19 +871,16 @@
             output = input
         else:
             output = ms.ops.squeeze(input_ms, dim)
     else:
         output = ms.ops.squeeze(input_ms)
     return cast_to_adapter_tensor(output)
 
-
 def from_numpy(np_data):
-    # return cast_to_adapter_tensor(ms.Tensor.from_numpy(np_data))
-    return cast_to_adapter_tensor(ms.Tensor(np_data))
-
+    return cast_to_adapter_tensor(ms.Tensor.from_numpy(np_data))
 
 def absolute(input, *, out=None):
     input = cast_to_ms_tensor(input)
     output = ms.ops.absolute(input)
     return _out_inplace_assign(out, output, "absolute")
 
 
@@ -1418,27 +1397,44 @@
 
 def logical_xor(input, other, *, out=None):
     if isinstance(input, adapter_tensor):
         input = cast_to_ms_tensor(input).astype(ms.bool_)
     if isinstance(other, adapter_tensor):
         other = cast_to_ms_tensor(other).astype(ms.bool_)
 
-    # TODO: ms.ops.logical_xor to supported GPU and Ascend
-    if is_under_ascend_context() or is_under_gpu_context():
+    # TODO: ms.ops.logical_xor to supported GPU
+    if is_under_gpu_context():
         output = ms.numpy.logical_xor(input, other)
     else:
         output = ms.ops.logical_xor(input, other)
     return _out_inplace_assign(out, output, "logical_xor")
 
 
 def logit(input, eps=None, *, out=None):
     input = cast_to_ms_tensor(input)
     output = ms.ops.logit(input, eps)
     return _out_inplace_assign(out, output, "logit")
 
+def lu(input, get_infos=False, pivot=True, *, out=None):
+    output = input.lu(pivot=pivot, get_infos=get_infos)
+    return _out_inplace_assign_with_adapter_tensor(out, output, "lu")
+
+#TODO: Enable after upgrading
+def lu_unpack(LU_data, LU_pivots, unpack_data=True, unpack_pivots=True, *, out=None):
+    LU_data = cast_to_ms_tensor(LU_data)
+    LU_pivots = cast_to_ms_tensor(LU_pivots)
+    output = ms.ops.lu_unpack(LU_data, LU_pivots, unpack_data=unpack_data, unpack_pivots=unpack_pivots)
+    return _out_inplace_assign(out, output, "lu_unpack")
+
+# TODO: currently not support return qr as second result
+def lstsq(A, x, *, out=None):
+    #TODO: ms.ops.lstsq not support GPU and Ascend, currently use numpy func
+    output = A.lstsq(x, 'torch.lstsq')
+    return _out_inplace_assign_with_adapter_tensor(out, output, "lstsq")
+
 def frombuffer(buffer, *, dtype = None, count=- 1, offset=0, requires_grad=False):
     unsupported_attr(requires_grad)
     np_dtype = _TypeDict[dtype]
     output = np.frombuffer(buffer=buffer, dtype=np_dtype, count=count, offset=offset)
     return adapter_tensor(output, dtype=dtype)
 
 def as_strided(input, size, stride, storage_offset=None):
@@ -1481,26 +1477,42 @@
 
 def minimum(input, other, *, out=None):
     input = cast_to_ms_tensor(input)
     other = cast_to_ms_tensor(other)
     output = ms.ops.minimum(input, other)
     return _out_inplace_assign(out, output, "minimum")
 
+def polygamma(n, input, *, out=None):
+    n = ms.Tensor(n)
+    input_ms = cast_to_ms_tensor(input)
+    output = ms.ops.polygamma(n, input_ms)
+    return _out_inplace_assign(out, output, "polygamma")
+
+def searchsorted(sorted_sequence, value, *, out_int32=False, right=False, side='left', out=None, sorter=None):
+    if sorter is not None:
+        warnings.warn("torch.searchsorted don't support sorter now.")
+    #TODO:right and side has the same usage, thus set the side to unable
+    if side == 'right':
+        right = True
+    sorted_sequence = cast_to_ms_tensor(sorted_sequence)
+    value = cast_to_ms_tensor(value)
+    if sorted_sequence.dtype not in (ms.int64, ms.int32) or value.dtype not in (ms.int64, ms.int32):
+        value = value.astype(ms.int64)
+        sorted_sequence = sorted_sequence.astype(ms.int64)
+    output = ms.ops.searchsorted(sorted_sequence, value, out_int32=out_int32, right=right)
+    return _out_inplace_assign(out, output, "searchsorted")
 
 def sigmoid(input, *, out=None):
-    #TODO: ms.ops.sigmoid() not support float64
     input = cast_to_ms_tensor(input)
-    # output = 1 / (ms.ops.exp(0 - input) + 1)
-    sigmoid_op = _get_cache_prim(ms.ops.Sigmoid)()
-    if input.dtype == ms.float64:
+    if is_under_ascend_context() and input.dtype == ms.float64:
         input = input.astype(ms.float32)
-        output = sigmoid_op(input)
+        output = ms.ops.sigmoid(input)
         output = output.astype(ms.float64)
     else:
-        output = sigmoid_op(input)
+        output = ms.ops.sigmoid(input)
     return _out_inplace_assign(out, output, "sigmoid")
 
 
 def softmax(input, dim, dtype=None, *, out=None):
     input = cast_to_ms_tensor(input)
     if dtype is not None:
         input = input.astype(dtype)
@@ -1530,17 +1542,24 @@
     input = cast_to_ms_tensor(input)
     other = cast_to_ms_tensor(other)
     output = ms.ops.hypot(input, other)
     return _out_inplace_assign(out, output, "hypot")
 
 
 def i0(input, *, out=None):
+    # TODO：ms.ops.bessel_i0 to support on Ascend
+    if is_under_ascend_context():
+        input_np = input.numpy()
+        output = ms.Tensor.from_numpy(np.i0(input_np))
+        if input.dtype in all_int_type:
+            output = output.astype(ms.float32)
+        return cast_to_adapter_tensor(output)
+
     input = cast_to_ms_tensor(input)
-    float_type = [ms.float16, ms.half, ms.float32, ms.single, ms.float64, ms.double]
-    if input.dtype not in float_type:
+    if input.dtype in all_int_type:
         input = input.astype(ms.float32)
     output = ms.ops.bessel_i0(input)
     return _out_inplace_assign(out, output, "i0")
 
 def igamma(input, other, *, out=None):
     output = input.igamma(other)
     return _out_inplace_assign_with_adapter_tensor(out, output, "igamma")
@@ -1591,25 +1610,26 @@
         output = input-input-input
     else:
         output = 0 - input
     return _out_inplace_assign(out, output, "negative")
 
 
 def nextafter(input, other, *, out=None):
-    # TODO: not found mindspore.ops.nextafter
-    input_np = input.asnumpy()
-    other_np = other.asnumpy()
-    output_np = np.nextafter(input_np, other_np)
-    output = ms.Tensor(output_np)
+    input = cast_to_ms_tensor(input)
+    other = cast_to_ms_tensor(other)
+    output = ms.ops.nextafter(input, other)
     return _out_inplace_assign(out, output, "nextafter")
 
 
 def positive(input):
     return input
 
+def qr(input, some=True, *, out=None):
+    output = input.qr(some)
+    return _out_inplace_assign_with_adapter_tensor(out, output, "qr")
 
 def rad2deg(input, *, out=None):
     input = cast_to_ms_tensor(input)
     if not input.is_floating_point():
         input = input.astype(ms.float32)
     output = ms.ops.rad2deg(input)
     return _out_inplace_assign(out, output, "rad2deg")
@@ -1637,14 +1657,21 @@
 def rsqrt(input, *, out=None):
     input = cast_to_ms_tensor(input)
     if 'Bool' in str(input.dtype) or 'Int' in str(input.dtype):
         input = input.astype(ms.float32)
     output = ms.ops.rsqrt(input)
     return _out_inplace_assign(out, output, "rsqrt")
 
+def roll(input, shifts, dims=None, *, out=None):
+    output = input.roll(shifts, dims=dims)
+    return _out_inplace_assign_with_adapter_tensor(out, output, "roll")
+
+def rot90(input, k, dims, *, out=None):
+    output = input.rot90(k, dims)
+    return _out_inplace_assign_with_adapter_tensor(out, output, "rot90")
 
 def sgn(input, *, out=None):
     input = cast_to_ms_tensor(input)
     if 'Bool' in str(input.dtype) or 'Int' in str(input.dtype):
         type = input.dtype
         input = input.astype(ms.float32)
         output = ms.ops.sgn(input).astype(type)
@@ -1704,16 +1731,15 @@
 def trace(input):
     input = cast_to_ms_tensor(input)
     output = input.trace()
     return cast_to_adapter_tensor(output)
 
 def tril(input, diagonal=0, *, out=None):
     input = cast_to_ms_tensor(input)
-    # TODO: To use ms.ops.tril after it supported on Ascend
-    output = ms.numpy.tril(input, diagonal)
+    output = ms.ops.tril(input, diagonal)
     return _out_inplace_assign(out, output, "tril")
 
 def conj(input):
     input = cast_to_ms_tensor(input)
     output = input.conj()
     return cast_to_adapter_tensor(output)
 
@@ -1938,16 +1964,16 @@
 def masked_select(input, mask, *, out=None):
     x = cast_to_ms_tensor(input)
     mask = cast_to_ms_tensor(mask)
     output = ms.ops.masked_select(x, mask)
     return _out_inplace_assign(out, output, "masked_select")
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE)
 def _get_select_out_shape(input_shape, dim):
     shape = [input_shape[i] for i in range(len(input_shape)) if i != dim]
     return tuple(shape)
 
 
 def select(input, dim, index):
     return input.select(dim, index)
@@ -2360,40 +2386,46 @@
         output = ms.ops.ger(input, vec2)
         output = output.astype(_out_dtype)
     else:
         output = ms.ops.ger(input, vec2)
     return _out_inplace_assign(out, output, "ger")
 
 def svd(input, some=True, compute_uv=True, *, out=None):
-    input = cast_to_ms_tensor(input)
-    s, u, v = ms.ops.svd(input, not some, compute_uv)
-    output = (u, s, v)
-    return _out_inplace_assign(out, output, "svd")
+    output = input.svd(some, compute_uv)
+    return _out_inplace_assign_with_adapter_tensor(out, output, "svd")
 
 def unique_consecutive(input, return_inverse=False, return_counts=False, dim=None) :
     input = cast_to_ms_tensor(input)
     output = ms.ops.unique_consecutive(input, return_idx=return_inverse, return_counts=return_counts, axis=dim)
     return cast_to_adapter_tensor(output)
 
 def block_diag(*tensors):
     inputs = cast_to_ms_tensor(tensors)
     output = ms.ops.block_diag(*inputs)
     return cast_to_adapter_tensor(output)
+
 def logspace(start, end, steps, base=10.0, *, out=None, dtype=None, layout=None, device=None, requires_grad=False):
     unsupported_attr(layout)
     unsupported_attr(device)
     unsupported_attr(requires_grad)
     start = ms.Tensor(start, dtype=dtype)
     end = ms.Tensor(end, dtype=dtype)
-    # TODO: For later version the base should be int type, enable atfer version upgrading
-    # base = base.astype(int32)
+    if base % 1 != 0:
+        raise ValueError("For logspace, base only support integer")
+    base = int(base)
+    if dtype is None:
+        dtype = ms.float32
+    _dtype = dtype
+
     if start.dtype in all_int_type or end.dtype in all_int_type or dtype in all_int_type:
         start = start.astype(mstype.float32)
         end = end.astype(mstype.float32)
-    output = ms.ops.logspace(start, end, steps, base, dtype=dtype)
+        _dtype = mstype.float32
+    output = ms.ops.logspace(start, end, steps, base, dtype=_dtype)
+    output = output.astype(dtype)
     return _out_inplace_assign(out, output, "logspace")
 
 def column_stack(tensors, *, out=None):
     tensors = cast_to_ms_tensor(tensors)
     output = ms.ops.column_stack(tensors)
     return _out_inplace_assign(out, output, "column_stack")
 
@@ -2415,15 +2447,20 @@
 def swapdims(input, dim0, dim1):
     input = cast_to_ms_tensor(input)
     output = ms.ops.swapdims(input, dim0, dim1)
     return cast_to_adapter_tensor(output)
 
 def swapaxes(input, axis0, axis1):
     input = cast_to_ms_tensor(input)
-    output = ms.ops.swapaxes(input, axis0, axis1)
+    if input.nelement() == 0:
+        out_shape = list(input.shape)
+        out_shape[axis0], out_shape[axis1] = out_shape[axis1], out_shape[axis0]
+        output = input.reshape(tuple(out_shape))
+    else:
+        output = ms.ops.swapaxes(input, axis0, axis1)
     return cast_to_adapter_tensor(output)
 
 def row_stack(tensors, *, out=None):
     tensors = cast_to_ms_tensor(tensors)
     output = ms.ops.vstack(tensors)
     return _out_inplace_assign(out, output, "row_stack")
 
@@ -2700,14 +2737,19 @@
         return _out_inplace_assign(out, output, "matrix_power")
     else:
         raise NotImplementedError("for adapter, matrix_power neither supported on GPU nor ascend.")
 
 def poisson(input, generator=None):
     if generator is not None:
         raise NotImplementedError("adapter not support generator.")
+    if is_under_ascend_context():
+        input_np = input.numpy()
+        output = from_numpy(np.random.poisson(input_np, None)).to(dtype=input.dtype)
+        return output
+
     input_ms = cast_to_ms_tensor(input)
     shape = ms.Tensor([], mstype.int32)
     output = ms.ops.random_poisson(shape, input_ms, dtype=input_ms.dtype)
     return cast_to_adapter_tensor(output)
 
 def eig(input, *, out=None):
     if not is_under_gpu_context():
@@ -2750,7 +2792,17 @@
         shape = mean.shape
         dtype = mean.dtype
     output = ms.ops.normal(shape, mean, std).astype(dtype)
     return _out_inplace_assign(out, output, "normal")
 
 def orgqr(input, tau):
     return input.orgqr(tau)
+
+def vander(x, N=None, increasing=False, *, out=None):
+    x = cast_to_ms_tensor(x)
+    #TODO: need to use ops func
+    output = ms.numpy.vander(x, N, increasing)
+    return _out_inplace_assign(out, output, "vander")
+
+def bernoulli(input, *, generator=None, out=None):
+    output = input.bernoulli(generator=generator)
+    return _out_inplace_assign(out, output, "bernoulli")
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/hub.py` & `msadapter-0.1.0rc0/msadapter/pytorch/hub.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/functional.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/functional.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """Functional interface"""
 import math
 import warnings
-from functools import lru_cache
+from typing import Iterable
+# from functools import lru_cache
 import numpy as np
 import mindspore as ms
 import mindspore.nn as nn
-from mindspore.ops import constexpr
+from mindspore.ops.primitive import _primexpr
 from mindspore.ops.operations.nn_ops import TripletMarginLoss as TripletMarginLossOp
 from mindspore.ops._primitive_cache import _get_cache_prim
 from mindspore.ops.function.math_func import _expand, _check_same_type
 
-from msadapter.utils import unsupported_attr, _GLOBAL_LRU_CACHE_SIZE_NN
+# from msadapter.utils import unsupported_attr, is_under_ascend_context, _GLOBAL_LRU_CACHE_SIZE_NN
+from msadapter.utils import unsupported_attr, is_under_ascend_context
 from msadapter.pytorch.tensor import Tensor, cast_to_ms_tensor, cast_to_adapter_tensor
 from msadapter.pytorch.common._inner import _inplace_assign_pynative
 from msadapter.pytorch.common.dtype import all_int_type
 from msadapter.pytorch.nn.modules.utils import _do_pad, _is_zero_paddings, _pair,\
                                                 _repeat_tuple
 
 all = [
@@ -96,19 +98,21 @@
     'pixel_unshuffle',
     'one_hot',
 
     'embedding',
     'max_pool2d',
 
     'fold',
-    'unfold'
+    'unfold',
+
+    'multi_head_attention_forward'
 ]
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_adaptive_pool_args(input_shape, output_size):
     _, _, h, w = input_shape
     if isinstance(output_size, int):
         output_size = [output_size, ] * 2
     condition = [0, ] * 2
     out_h = output_size[0] + condition[0] * h
     out_w = output_size[1] + condition[1] * w
@@ -141,37 +145,122 @@
     return cast_to_adapter_tensor(out)
 
 def adaptive_avg_pool3d(input, output_size):
     input = cast_to_ms_tensor(input)
     output = ms.ops.adaptive_avg_pool3d(input, output_size)
     return cast_to_adapter_tensor(output)
 
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+def _get_adaptive_max_pool1d_const(input_shape, output_size):
+    _, _, width = input_shape
+    stride = width // output_size
+    kernel_size = width - (output_size - 1) * stride
+    stride = (1, width // output_size)
+    kernel_size = (1, kernel_size)
+    return kernel_size, stride
+
 def adaptive_max_pool1d(input, output_size, return_indices=False):
     input = cast_to_ms_tensor(input)
     ndim = input.ndim
     if ndim == 2:
         input = input.expand_dims(0)
-        if return_indices:
-            raise ValueError('keyword argument return_indices is ont supported.')
-        output = ms.ops.adaptive_max_pool1d(input, output_size)
-        output = output.squeeze(0)
+
+    if return_indices:
+        input_shape = ms.ops.shape(input)
+        _kernel_size, _stride = _get_adaptive_max_pool1d_const(input_shape, output_size)
+        max_pool = _get_cache_prim(ms.ops.MaxPoolWithArgmaxV2)(kernel_size=_kernel_size, strides=_stride,
+                                                               pads=0, dilation=(1, 1), argmax_type=ms.int32)
+        input = input.expand_dims(-2)
+        out, idx = max_pool(input)
+        out = out.squeeze(-2)
+        idx = idx.squeeze(-2)
+        if ndim == 2:
+            out = out.squeeze(0)
+            idx = idx.squeeze(0)
+        output = (out, idx)
     else:
-        if return_indices:
-            raise ValueError('keyword argument return_indices is ont supported.')
-        output = ms.ops.adaptive_max_pool1d(input, output_size)
+        # TODO: ms.ops.adaptive_max_pool1d has some bug, use it in the future
+        input_shape = ms.ops.shape(input)
+        _kernel_size, _stride = _get_adaptive_max_pool1d_const(input_shape, output_size)
+        max_pool_ = _get_cache_prim(ms.ops.MaxPool)(kernel_size=_kernel_size, strides=_stride)
+        input = input.expand_dims(-2)
+        out = max_pool_(input)
+        out = out.squeeze(-2)
+        if ndim == 2:
+            out = out.squeeze(0)
+        output = out
+
     return cast_to_adapter_tensor(output)
 
+
 def adaptive_max_pool2d(input, output_size, return_indices=False):
     input = cast_to_ms_tensor(input)
     output = ms.ops.adaptive_max_pool2d(input, output_size, return_indices)
     return cast_to_adapter_tensor(output)
 
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+def _get_adaptive_max_pool3d_output_size(input_shape, output_size):
+    if not isinstance(output_size, Iterable):
+        output_size = [output_size, ] * 3
+    condition = [0,] * 3
+    if None in output_size:
+        output_size = list(output_size)
+        if output_size[0] is None:
+            condition[0] = 1
+            output_size[0] = 0
+        if output_size[1] is None:
+            condition[1] = 1
+            output_size[1] = 0
+        if output_size[2] is None:
+            condition[2] = 1
+            output_size[2] = 0
+    _, _, d, h, w = input_shape
+    out_d = output_size[0] + condition[0] * d
+    out_h = output_size[1] + condition[1] * h
+    out_w = output_size[2] + condition[2] * w
+    return out_d, out_h, out_w
+
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+def _get_adaptive_max_pool3d_stride(input_shape, output_size):
+    out_d, out_h, out_w = output_size
+    _, _, d, h, w = input_shape
+    stride_d = d // out_d
+    kernel_d = d - (out_d - 1) * stride_d
+    stride_h = h // out_h
+    kernel_h = h - (out_h - 1) * stride_h
+    stride_w = w // out_w
+    kernel_w = w - (out_w - 1) * stride_w
+
+    return kernel_d, kernel_h, kernel_w, stride_d, stride_h, stride_w
+
 def adaptive_max_pool3d(input, output_size, return_indices=False):
     input = cast_to_ms_tensor(input)
-    output = ms.ops.adaptive_max_pool3d(input, output_size, return_indices)
+    input_shape = ms.ops.shape(input)
+    _output_size = _get_adaptive_max_pool3d_output_size(input_shape, output_size)
+
+    if is_under_ascend_context():
+        # TODO: Ascend not support ms.ops.adaptive_max_pool3d, use MaxPool3D instead
+        # MaxPool3D result is not the same as adaptive_max_pool3d, but the shape.
+        # Implement below do not affect the converge of trainning.
+        if return_indices:
+            raise NotImplementedError("For adaptive_max_pool3d, return_indices is not supported yet.")
+
+        kernel_d, kernel_h, kernel_w, stride_d, stride_h, stride_w = \
+            _get_adaptive_max_pool3d_stride(input_shape, _output_size)
+
+        avg_pool = ms.ops.MaxPool3D(kernel_size=(kernel_d, kernel_h, kernel_w),
+                                    strides=(stride_d, stride_h, stride_w),
+                                    pad_mode="valid", data_format="NCDHW")
+        output = avg_pool(input)
+    else:
+        output = ms.ops.adaptive_max_pool3d(input, _output_size, return_indices)
+
     return cast_to_adapter_tensor(output)
 
 def pad(input, pad, mode="constant", value=0):
     if mode == "replicate":
         mode = "edge"
 
     value = ms.Tensor(value, dtype=input.dtype)
@@ -302,28 +391,19 @@
     if size is None and scale_factor is None:
         raise ValueError("either size or scale_factor should be defined")
 
     if size is not None and scale_factor is not None:
         raise ValueError("only one of size or scale_factor should be defined")
 
     def linear_func(input):
-        #TODO: if switch the mindspore version, delete the next four lines
-        if align_corners is True:
-            trans_mode = 'align_corners'
-        else:
-            trans_mode = 'half_pixel'
-
-        _size =_upsample_common_process_size(size=size, scale_factor=scale_factor, shape=input.shape)
+        _size =_upsample_common_process_size(size, scale_factor, input.shape)
 
         input = cast_to_ms_tensor(input)
-        #TODO: if switch the mindspore version, change the code to
-        #out = ms.ops.interpolate(input, scale_factor=None, size=_size,
-        #                        align_corners=align_corners, mode=mode)
-        out = ms.ops.interpolate(input, scales=None, sizes=_size,
-                                coordinate_transformation_mode=trans_mode, mode=mode)
+        out = ms.ops.interpolate(input, scale_factor=None, size=_size,
+                                 align_corners=align_corners, mode=mode)
 
         return cast_to_adapter_tensor(out)
 
     def bllinear_func(input):
         return upsample_bilinear(input, size=size, scale_factor=scale_factor, align_corners=align_corners)
 
     def resize_nearest_neighbor_func(input):
@@ -337,16 +417,16 @@
         raise ValueError("Until now, `mode` beside 'linear', 'bilinear', 'nearest' are not supported")
 
     func = mode_func[mode]
 
     out = func(input)
     return out
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_softmax_dim(ndim):
     if ndim in (0, 1, 3):
         ret = 0
     else:
         ret = 1
     return ret
 
@@ -391,16 +471,16 @@
         input = input.astype(ms.float32)
     output = ms.ops.tanh(input)
     return cast_to_adapter_tensor(output)
 
 
 def tanhshrink(input):
     input = cast_to_ms_tensor(input)
-    ouput = input - ms.ops.functional.tanh(input)
-    return cast_to_adapter_tensor(ouput)
+    output = input - ms.ops.functional.tanh(input)
+    return cast_to_adapter_tensor(output)
 
 
 def glu(input, dim=-1):
     if input.dim() == 0:
         raise RuntimeError("glu does not support scalars because halving size must be even")
     if input.shape[dim] % 2 == 1:
         raise RuntimeError("Halving dimension must be even, but dimension {} is size {}".format(dim,input.shape[dim]))
@@ -448,16 +528,20 @@
 
     ret = ms.ops.select(mask, input, ret_mask)
     return cast_to_adapter_tensor(ret)
 
 
 def sigmoid(input):
     input = cast_to_ms_tensor(input)
-    sigmoid_op = _get_cache_prim(ms.ops.Sigmoid)()
-    out = sigmoid_op(input)
+    if is_under_ascend_context() and input.dtype == ms.float64:
+        input = input.astype(ms.float32)
+        out = ms.ops.sigmoid(input)
+        out = out.astype(ms.float64)
+    else:
+        out = ms.ops.sigmoid(input)
     return cast_to_adapter_tensor(out)
 
 
 def hardsigmoid(input, inplace=False):
     input_ms = cast_to_ms_tensor(input)
     hardsigmoid_op = _get_cache_prim(ms.ops.HSigmoid)()
     out = hardsigmoid_op(input_ms)
@@ -476,30 +560,29 @@
         warnings.warn("`eps` parameter is deprecated and has no effect.")
     logits = cast_to_ms_tensor(logits)
     out = ms.ops.gumbel_softmax(logits, tau, hard, dim)
     return cast_to_adapter_tensor(out)
 
 
 def threshold(input, threshold, value, inplace=False):
+    #TODO: threshold---function name and input name is same will raise error on Graph mode.
     input_ms = cast_to_ms_tensor(input)
-    cond = ms.ops.gt(input_ms, threshold)
-    value = ms.ops.fill(input_ms.dtype, input_ms.shape, value)
-    out = ms.ops.select(cond, input_ms, value)
+    out = ms.ops.threshold(input_ms, threshold, value)
     return _inplace_assign_pynative(input, inplace, out, "threshold")
 
 
 rrelu_ = rrelu
 relu_ = relu
 elu_ = elu
 hardtanh_ = hardtanh
 leaky_relu_ = leaky_relu
 threshold_ = threshold
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_reduce_string(size_average, reduce):
     if size_average is None:
         size_average = True
     if reduce is None:
         reduce = True
 
     if size_average and reduce:
@@ -517,16 +600,16 @@
 def smooth_l1_loss(input, target, size_average=None, reduce=None, reduction='mean', beta=1.0):
     if reduce is not None or size_average is not None:
         reduction = _get_reduce_string(size_average, reduce)
 
     input = cast_to_ms_tensor(input)
     target = cast_to_ms_tensor(target)
     output = ms.ops.smooth_l1_loss(input, target, beta, reduction)
-    if reduction != 'none' and output.shape == 1:
-        return Tensor(output[0])
+    if reduction != 'none' and len(output.shape) == 1:
+        return cast_to_adapter_tensor(output[0])
     return cast_to_adapter_tensor(output)
 
 def _get_loss(x, reduction):
     """
     Computes the loss.
     """
     if reduction is None or reduction == 'none':
@@ -600,15 +683,15 @@
     #TODO: length do not support tuple
     if not isinstance(input_lengths, Tensor) or not isinstance(target_lengths, Tensor):
         raise TypeError("'input_lengths' and 'target_lengths' only support Tensor now")
     if isinstance(input_lengths, Tensor) and isinstance(target_lengths, Tensor):
         input_lengths = cast_to_ms_tensor(input_lengths)
         target_lengths = cast_to_ms_tensor(target_lengths)
 
-    if targets.dtype not in {ms.int32, ms.int64} \
+    if targets.dtype not in (ms.int32, ms.int64) \
             or not (targets.dtype == input_lengths.dtype and targets.dtype == target_lengths.dtype):
         targets = targets.astype(ms.int64)
         input_lengths = input_lengths.astype(ms.int64)
         target_lengths = target_lengths.astype(ms.int64)
     result, _ = ms.ops.ctc_loss(log_probs, targets, input_lengths, target_lengths, blank, reduction, zero_infinity)
     return cast_to_adapter_tensor(result)
 
@@ -719,25 +802,25 @@
         if pos_weight is None:
             pos_weight = ones_input
 
     result = ms.ops.binary_cross_entropy_with_logits(input, target, weight, pos_weight, reduction)
     return cast_to_adapter_tensor(result)
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _upsample_common_check(size, scale_factor):
     if size is None and scale_factor is None:
         raise ValueError("either size or scale_factor should be defined.")
 
     if size is not None and scale_factor is not None:
         raise ValueError("only one of size or scale_factor should be defined.")
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _upsample_common_process_size(size, scale_factor, shape):
     input_shape = list(shape)
     input_rank = len(shape)
     if scale_factor is not None:
         size_ = input_shape[2:]
         for i, _ in enumerate(size_):
             size_[i] *= scale_factor
@@ -780,23 +863,16 @@
     if len(input_shape) != 4:
         raise ValueError("Until now, upsample_bilinear only support 4-D input.")
 
     _upsample_common_check(size, scale_factor)
     size_ = _upsample_common_process_size(size, scale_factor, input_shape)
 
     input = cast_to_ms_tensor(input)
-    #TODO: if switch the mindspore version, delete the next four lines
-    if align_corners is True:
-        _cor_mode = "align_corners"
-    else:
-        _cor_mode = "half_pixel"
 
-    #TODO: if switch the mindspore version, change the code to
-    # result = ms.ops.interpolate(input, size=size_, align_corners=align_corners, mode="bilinear")
-    result = ms.ops.interpolate(input, sizes=size_, coordinate_transformation_mode=_cor_mode, mode="bilinear")
+    result = ms.ops.interpolate(input, size=size_, align_corners=align_corners, mode="bilinear")
     return cast_to_adapter_tensor(result)
 
 def pairwise_distance(x1, x2, p=2.0, eps=1e-06, keepdim=False):
     x1 = cast_to_ms_tensor(x1)
     x2 = cast_to_ms_tensor(x2)
     input = x1-x2+eps
     input_p = ms.ops.pow(ms.ops.abs(input), p)
@@ -890,17 +966,15 @@
                       "1D dropout behavior is desired - input is interpreted as shape (N, C, L), where C "
                       "is the channel dim. This behavior will change in a future release to interpret the "
                       "input as one without a batch dimension, i.e. shape (C, H, W). To maintain the 1D "
                       "channel-wise dropout behavior, please switch to using dropout1d instead.")
         return dropout1d(input, p, training, inplace)
 
     input_ms = cast_to_ms_tensor(input)
-    #TODO: if switch the mindspore version, change the code to
-    # out = ms.ops.dropout2d(input_ms, p)
-    out, _ = ms.ops.dropout2d(input_ms, p)
+    out = ms.ops.dropout2d(input_ms, p)
     return _inplace_assign_pynative(input, inplace, out, "dropout2d")
 
 
 def dropout3d(input, p=0.5, training=True, inplace=False):
     if p < 0.0 or p > 1.0:
         raise ValueError("dropout probability has to be between 0 and 1, " "but got {}".format(p))
     inp_dim = input.dim()
@@ -915,17 +989,15 @@
         return input
 
     is_batched = inp_dim == 5
 
     input_ms = cast_to_ms_tensor(input)
     if not is_batched:
         input_ms = ms.ops.expand_dims(input_ms, 0)
-    #TODO: if switch the mindspore version, change the code to
-    # out = ms.ops.dropout3d(input_ms, p)
-    out, _ = ms.ops.dropout3d(input_ms, p)
+    out = ms.ops.dropout3d(input_ms, p)
     if not is_batched:
         out = ms.ops.squeeze(out, 0)
 
     return _inplace_assign_pynative(input, inplace, out, "dropout3d")
 
 
 def dropout(input, p=0.5, training=True, inplace=False):
@@ -941,16 +1013,16 @@
     random_array = ms.Tensor(random_array_np, ms.float32)
     mask = (random_array > ms.Tensor(p, ms.float32))
     out = mask * 1.0 / (1.0-p) * input_ms
 
     return _inplace_assign_pynative(input, inplace, out, "dropout")
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_alpha_dropout_const(p):
     mean = 0.0
     var = 1.0
     scale = 1.0507009873554804934193349852946
     alpha = 1.6732632423543772848170429916717
     alpha_ = -scale * alpha
     q = 1.0 - p
@@ -1140,16 +1212,16 @@
         loss = ms.ops.multi_margin_loss(input, target, p=p, margin=margin, weight=weight, reduction=reduction)
         return cast_to_adapter_tensor(loss)
 
     loss = ms.ops.multi_margin_loss(input, target, p=p, margin=margin, weight=weight, reduction=reduction)
     return cast_to_adapter_tensor(loss)
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_avg_pool2d_const(kernel_size, stride, padding):
     if stride is None:
         stride = kernel_size
 
     padding = padding if isinstance(padding, tuple) else _pair(padding)
     return kernel_size, stride, padding
 
@@ -1181,28 +1253,28 @@
             out = out.squeeze(0)
         else:
             input = _do_pad(input, _padding)
             out = avg_pool_ops(input)
     return cast_to_adapter_tensor(out)
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_local_response_norm_const(x_dim, size):
     if x_dim < 3:
         raise ValueError("Expected 3D or higher dimensionality"
                          f"input (got {x_dim} dimensions)")
 
     if x_dim == 3:
         return ((size//2, (size-1)//2), (0, 0))
 
     return ((size//2, (size-1)//2), (0, 0), (0, 0))
 
 def local_response_norm(input, size, alpha=0.0001, beta=0.75, k=1.0):
-    if input.size() == 0:
+    if len(input.shape) == 0:
         return input
 
     dim = input.dim()
     _pad = _get_local_response_norm_const(dim, size)
 
     input = cast_to_ms_tensor(input)
     div = ms.ops.mul(input, input).expand_dims(axis=1)
@@ -1346,28 +1418,19 @@
 
         return upsample_bilinear(input, size, scale_factor, align_corners=align_corners)
 
     if mode == 'linear':
         if input.dim() != 3:
             raise ValueError(f"'linear' mode only support 3D input, but got {input.dim()}D")
 
-        #TODO: if switch the mindspore version, delete the next four lines
-        if align_corners is True:
-            trans_mode = 'align_corners'
-        else:
-            trans_mode = 'half_pixel'
-
-        _size =_upsample_common_process_size(size=size, scale_factor=scale_factor, shape=input.shape)
+        _size =_upsample_common_process_size(size, scale_factor, input.shape)
 
         input = cast_to_ms_tensor(input)
-        #TODO: if switch the mindspore version, change the code to
-        #out = ms.ops.interpolate(input, scale_factor=None, size=_size,
-        #                        align_corners=align_corners, mode=mode)
-        out = ms.ops.interpolate(input, scales=None, sizes=_size,
-                                     coordinate_transformation_mode=trans_mode, mode=mode)
+        out = ms.ops.interpolate(input, scale_factor=None, size=_size,
+                                 align_corners=align_corners, mode=mode)
         return cast_to_adapter_tensor(out)
 
     if mode in ['bicubic', 'trilinear', 'area', 'nearest-exact']:
         raise NotImplementedError(f"For interpolate: currently not support mode '{mode}'")
 
     raise NotImplementedError(
         "Input Error: Only 3D, 4D and 5D input Tensors supported"
@@ -1422,89 +1485,91 @@
 
 
 def grid_sample(input, grid, mode='bilinear', padding_mode='zeros', align_corners=None):
     input = cast_to_ms_tensor(input)
     grid = cast_to_ms_tensor(grid)
     if align_corners is None:
         align_corners = False
-    output = ms.ops.grid_sample(input, grid, interpolation_mode=mode,
+    output = ms.ops.grid_sample(input, grid, mode=mode,
                                 padding_mode=padding_mode, align_corners=align_corners)
     output = cast_to_adapter_tensor(output)
     return output
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _check_conv1d_input_shape(input_shape):
     if len(input_shape) != 3:
         raise ValueError(f"For 'conv1d', the dimension of input must be 3d, but got {len(input_shape)}.")
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_conv1d_const(stride, padding, dilation):
     if isinstance(stride, tuple):
         stride = stride[0]
     pad_mode = "pad"
     if isinstance(padding, int):
-        padding = (0, 0, padding, padding)
+        padding = (0, padding)
     elif isinstance(padding, tuple):
-        padding = (0, 0, padding[0], padding[0])
+        padding = (0, padding[0])
     else:
         pad_mode = padding
         padding = 0
     if isinstance(dilation, tuple):
         dilation = dilation[0]
+    dilation = (1, dilation)
     return pad_mode, stride, padding, dilation
 
 
 def conv1d(input, weight, bias=None, stride=1, padding=0, dilation=1, groups=1):
     # TODO: not support float64, change to float32 now
     input_ms = cast_to_ms_tensor(input)
-    weight_ms = cast_to_ms_tensor(weight)
+    # do not cast weight because will lose gradient
+    # weight_ms = cast_to_ms_tensor(weight)
+    weight_ms = weight
     is_float64 = False
     if input_ms.dtype in (ms.float64, ms.double):
         input_ms = input_ms.astype(ms.float32)
         weight_ms = weight_ms.astype(ms.float32)
         is_float64 = True
 
     input_shape = input_ms.shape
     _check_conv1d_input_shape(input_shape)
     _pad_mode, _stride, _padding, _dilation = _get_conv1d_const(stride, padding, dilation)
     input_ms = ms.ops.expand_dims(input_ms, 2)
     weight_ms = ms.ops.expand_dims(weight_ms, 2)
-    output = ms.ops.conv2d(input_ms, weight_ms, _pad_mode, _padding, _stride, _dilation, groups)
+    output = ms.ops.conv2d(input_ms, weight_ms, None, _stride, _pad_mode, _padding, _dilation, groups)
     if bias is not None:
         # TODO: ms.ops.biasadd also not support float64
         if bias.dtype != output.dtype:
             bias = bias.astype(output.dtype)
         output = ms.ops.bias_add(output, bias)
     output = ms.ops.squeeze(output, 2)
 
     if is_float64:
         output = output.astype(ms.float64)
 
     return cast_to_adapter_tensor(output)
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_conv2d_const(stride, padding, dilation):
     if isinstance(stride, int):
         stride = (stride, stride)
     elif len(stride)==1:
         stride = (stride[0], stride[0])
     pad_mode = "pad"
     if isinstance(padding, int):
-        padding = (padding, padding, padding, padding)
+        padding = (padding, padding)
     elif isinstance(padding, tuple):
         if len(padding)==1:
-            padding = (padding[0], padding[0], padding[0], padding[0])
-        else:
-            padding = (padding[0], padding[0], padding[1], padding[1])
+            padding = (padding[0], padding[0])
+
     else:
         pad_mode = padding
         padding = 0
     if isinstance(dilation, int):
         dilation = (dilation, dilation)
     elif len(dilation) == 1:
         dilation = (dilation[0], dilation[0])
@@ -1521,41 +1586,41 @@
     is_float64 = False
     if input_ms.dtype in (ms.float64, ms.double):
         input_ms = input_ms.astype(ms.float32)
         weight_ms = weight_ms.astype(ms.float32)
         is_float64 = True
 
     _pad_mode, _stride, _padding, _dilation = _get_conv2d_const(stride, padding, dilation)
-    output = ms.ops.conv2d(input_ms, weight_ms, _pad_mode, _padding, _stride, _dilation, groups)
+    output = ms.ops.conv2d(input_ms, weight_ms, None, _stride, _pad_mode, _padding, _dilation, groups)
     if bias is not None:
         # TODO: ms.ops.biasadd also not support float64
         if bias.dtype != output.dtype:
             bias = bias.astype(output.dtype)
         output = ms.ops.bias_add(output, bias)
 
     if is_float64:
         output = output.astype(ms.float64)
 
     return cast_to_adapter_tensor(output)
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_maxpool2d_const_1(kernel_size, stride, padding):
     _kernel_size = kernel_size if isinstance(kernel_size, tuple) else (kernel_size, kernel_size)
     if stride is None:
         _stride = _kernel_size
     else:
         _stride = stride if isinstance(stride, tuple) else (stride, stride)
 
     _padding = padding if isinstance(padding, tuple) else (padding, padding)
     return _kernel_size, _stride, _padding
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_maxpool2d_const_2(kernel_size, stride, padding, dilation):
     _kernel_size = kernel_size + (1,) if isinstance(kernel_size, tuple) else (kernel_size, kernel_size, 1)
     if stride is None:
         _stride = _kernel_size
     else:
         _stride = stride + (1,) if isinstance(stride, tuple) else (stride, stride, 1)
     _padding = padding + (0,) if isinstance(padding, tuple) else (padding, padding, 0)
@@ -1647,26 +1712,26 @@
     indices = cast_to_ms_tensor(indices)
     if output_size is not None:
         output_size = tuple(output_size)
     out = ms.ops.max_unpool3d(input, indices, kernel_size, stride, padding, output_size)
     return cast_to_adapter_tensor(out)
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_linear_output_shape(input_shape, weight_shape, input_rank, weight_rank):
     shape_out= ()
     if input_rank > 1:
         shape_out = shape_out + input_shape[:-1]
     if weight_rank == 2:
         shape_out = shape_out + (weight_shape[0],)
     return shape_out
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _check_linear_shape(weight_rank, input_shape, weight_shape):
     if weight_rank not in (1, 2):
         raise ValueError("For nn.functional.linear, weight only support 2D or 1D input"
                             f"but got {weight_rank}D input")
 
     if input_shape[-1] != weight_shape[-1]:
         raise ValueError("For nn.functional.linear, size mismatch,"
@@ -1747,16 +1812,16 @@
                           _random_samples=None):
     input_ms = cast_to_ms_tensor(input_x)
     out = ms.ops.fractional_max_pool3d(input_ms, kernel_size, output_size, output_ratio, return_indices,
                                        _random_samples)
     return cast_to_adapter_tensor(out)
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_avg_pool1d_const(kernel_size, stride, padding):
     if isinstance(kernel_size, int):
         kernel_size = (kernel_size, 1)
     else:
         kernel_size = kernel_size + (1,)
     if stride is None:
         stride = (kernel_size, 1)
@@ -1788,16 +1853,16 @@
         input = input.expand_dims(-1)
         input = _do_pad(input, _pad)
         out = avg_pool_ops(input)
         out = out.squeeze(-1)
     return cast_to_adapter_tensor(out)
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_avg_pool3d_const(kernel_size, stride, padding, divisor_override):
     if stride is None:
         _stride = kernel_size
     else:
         _stride = stride
     if divisor_override is None:
         _divisor_override = 0
@@ -1825,16 +1890,16 @@
         out = out.squeeze(0)
     else:
         out = ms.ops.avg_pool3d(input_ms, kernel_size, _stride, _padding, ceil_mode, count_include_pad,
                                 _divisor_override)
     return cast_to_adapter_tensor(out)
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_maxpool1d_const_1(kernel_size, stride, padding, dilation):
     if isinstance(kernel_size, int):
         _kernel_size = (kernel_size, 1, 1)
     elif isinstance(kernel_size, tuple):
         _kernel_size = kernel_size + (1, 1)
     else:
         _kernel_size = kernel_size
@@ -1849,16 +1914,16 @@
         _stride = stride
 
     _padding = (padding, 0, 0)
     _dilation = (dilation, 1, 1)
     return _kernel_size, _stride, _padding, _dilation
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_maxpool1d_const_2(kernel_size, stride, padding):
     _kernel_size = (1, kernel_size)
     if stride is None:
         _stride = _kernel_size
     else:
         _stride = (1, stride)
     _padding = (0, padding)
@@ -1990,16 +2055,16 @@
         in_channels=in_channel, out_channels=out_channel, kernel_size=kernel_size, stride=stride,
         pad_mode=pad_mode, padding=padding, dilation=dilation, group=groups, has_bias=has_bias,
         weight_init=weight, bias_init=bias)
     out = _conv_2d_transpose(inputs)
     return cast_to_adapter_tensor(out)
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_conv_transpose3d_const(input_shape, weight_shape, groups, padding):
     if len(input_shape) != 5:
         raise ValueError("the rank of inputs tensor should be 5.")
     if len(weight_shape) != 5:
         raise ValueError("the rank of weight tensor should be 5")
 
     in_channel = input_shape[1]
@@ -2155,15 +2220,21 @@
 
 def prelu(input, weight):
     #TODO:ms.ops.prelu only suports float16 and float32, not float64.
     input = cast_to_ms_tensor(input)
     # weight will be Parameter and can not be cast to tensor, will lost weights.
     # ms.ops.prelu do not use tensor function of weight, so without cast_to_ms_tensor(weight), not effect.
     # weight = cast_to_ms_tensor(weight)
-    output = ms.ops.prelu(input, weight)
+    if is_under_ascend_context() and input.ndim < 2:
+        shape = input.shape
+        input = _expand(input, 2)
+        output = ms.ops.prelu(input, weight)
+        output = output.reshape(shape)
+    else:
+        output = ms.ops.prelu(input, weight)
     return cast_to_adapter_tensor(output)
 
 
 def poisson_nll_loss(input, target, log_input=True, full=False, size_average=None, eps=1e-08, reduce=None,
                      reduction='mean'):
     input_ms = cast_to_ms_tensor(input)
     target = cast_to_ms_tensor(target)
@@ -2210,29 +2281,28 @@
     elif reduction == "sum":
         ret = output.sum()
     else:
         ret = output
     return cast_to_adapter_tensor(ret)
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _get_conv3d_const(stride, padding, dilation):
     if isinstance(stride, int):
         stride = (stride, stride, stride)
     elif len(stride)==1:
         stride = (stride[0], stride[0], stride[0])
     pad_mode = "pad"
     if isinstance(padding, int):
-        padding = (padding, padding, padding, padding, padding, padding)
+        padding = (padding, padding, padding)
     elif isinstance(padding, tuple):
         if len(padding)==1:
-            padding = (padding[0], padding[0], padding[0], padding[0], padding[0], padding[0])
-        else:
-            padding = (padding[0], padding[0], padding[1], padding[1], padding[2], padding[2])
+            padding = (padding[0], padding[0], padding[0])
+
     else:
         pad_mode = padding
         padding = 0
     if isinstance(dilation, int):
         dilation = (dilation, dilation, dilation)
     elif len(dilation) == 1:
         dilation = (dilation[0], dilation[0], dilation[0])
@@ -2246,15 +2316,15 @@
     is_float64 = False
     if input_ms.dtype in (ms.float64, ms.double):
         input_ms = input_ms.astype(ms.float32)
         weight_ms = weight_ms.astype(ms.float32)
         is_float64 = True
 
     _pad_mode, _padding, _stride, _dilation = _get_conv3d_const(stride, padding, dilation)
-    output = ms.ops.conv3d(input_ms, weight_ms, _pad_mode, _padding, _stride, _dilation, groups)
+    output = ms.ops.conv3d(input_ms, weight_ms, None, _stride, _pad_mode, _padding, _dilation, groups)
     if bias is not None:
         # TODO: ms.ops.biasadd also not support float64
         if bias.dtype != output.dtype:
             bias = bias.astype(output.dtype)
         output = ms.ops.bias_add(output, bias)
 
     if is_float64:
@@ -2263,17 +2333,15 @@
     return cast_to_adapter_tensor(output)
 
 
 def unfold(input, kernel_size, dilation=1, padding=0, stride=1):
     # TODO: do not support on GPU
     input_ms = cast_to_ms_tensor(input)
     output = ms.ops.unfold(input_ms, kernel_size, dilation, padding, stride)
-    # TODO: Enable atfer version upgrading
-    #output = output.reshape(output.shape[0], output.shape[1] * output.shape[2], -1)
-    output = output.reshape(output.shape[0], output.shape[1], -1)
+    output = output.reshape(output.shape[0], output.shape[1] * output.shape[2], -1)
     return cast_to_adapter_tensor(output)
 
 
 def fold(input, output_size, kernel_size, dilation=1, padding=0, stride=1):
     # TODO: do not support on Ascend
     input_ms = cast_to_ms_tensor(input)
     ndim = input_ms.ndim
@@ -2285,7 +2353,41 @@
     else:
         shape_tmp = kernel_size[0] * kernel_size[1]
     input_ms = input_ms.reshape(shape[0], -1, shape_tmp, shape[2])
     output = ms.ops.fold(input_ms, ms.Tensor(output_size), kernel_size, dilation, padding, stride)
     if ndim == 2:
         output = output.squeeze(0)
     return cast_to_adapter_tensor(output)
+
+def multi_head_attention_forward(query, key, value, embed_dim_to_check, num_heads, in_proj_weight,
+                                 in_proj_bias, bias_k, bias_v, add_zero_attn, dropout_p, out_proj_weight,
+                                 out_proj_bias, training=True, key_padding_mask=None, attn_mask=None,
+                                 use_separate_proj_weight=False, q_proj_weight=None, k_proj_weight=None,
+                                 v_proj_weight=None, static_k=None, static_v=None, average_attn_weights=True,
+                                 k_is_v=False, q_is_k=False):
+    query = cast_to_ms_tensor(query)
+    key = cast_to_ms_tensor(key)
+    value = cast_to_ms_tensor(value)
+    key_padding_mask = cast_to_ms_tensor(key_padding_mask)
+    attn_mask = cast_to_ms_tensor(attn_mask)
+    static_k = cast_to_ms_tensor(static_k)
+    static_v = cast_to_ms_tensor(static_v)
+    in_proj_weight = ms.ops.Identity()(in_proj_weight) if in_proj_weight is not None else None
+    in_proj_bias = ms.ops.Identity()(in_proj_bias) if in_proj_bias is not None else None
+    bias_k = ms.ops.Identity()(bias_k) if bias_k is not None else None
+    bias_v = ms.ops.Identity()(bias_v) if bias_v is not None else None
+    out_proj_weight = ms.ops.Identity()(out_proj_weight) if out_proj_weight is not None else None
+    out_proj_bias = ms.ops.Identity()(out_proj_bias) if out_proj_bias is not None else None
+    q_proj_weight = ms.ops.Identity()(q_proj_weight) if q_proj_weight is not None else None
+    k_proj_weight = ms.ops.Identity()(k_proj_weight) if k_proj_weight is not None else None
+    v_proj_weight = ms.ops.Identity()(v_proj_weight) if v_proj_weight is not None else None
+    # TODO: older ver of torch doesn't have is_causal arg
+    attn_output, attn_output_weights = ms.ops.function.nn_func.multi_head_attention_forward(
+        query, key, value, embed_dim_to_check, num_heads,
+        in_proj_weight, in_proj_bias, bias_k, bias_v, add_zero_attn, dropout_p,
+        out_proj_weight, out_proj_bias, training=training,
+        key_padding_mask=key_padding_mask, attn_mask=attn_mask,
+        use_separate_proj_weight=use_separate_proj_weight,
+        q_proj_weight=q_proj_weight, k_proj_weight=k_proj_weight,
+        v_proj_weight=v_proj_weight, static_k=static_k, static_v=static_v,
+        average_attn_weights=average_attn_weights, k_is_v=k_is_v, q_is_k=q_is_k)
+    return cast_to_adapter_tensor(attn_output), cast_to_adapter_tensor(attn_output_weights)
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/init.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/init.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/activation.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/activation.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 import warnings
 import numpy as np
 from mindspore.ops import functional as F
 from mindspore.ops import operations as P
 from mindspore.common import dtype as mstype
 import mindspore as ms
 from mindspore import nn
-from mindspore._checkparam import Validator as validator
+import mindspore._checkparam as validator
 
+from msadapter.pytorch.functional import empty
 from msadapter.pytorch.nn.parameter import Parameter
 import msadapter.pytorch.nn.functional as ms_torch_nn_func
 from msadapter.pytorch.tensor import Tensor, tensor, cast_to_ms_tensor, cast_to_adapter_tensor
 from msadapter.utils import unsupported_attr
 from msadapter.pytorch.common._inner import _inplace_assign, _inplace_limit_pynative
 from .module import Module
+from .linear import Linear
+from ..init import constant_, xavier_normal_, xavier_uniform_
 
 __all__ = ['ReLU', 'Hardtanh', 'ReLU6', 'SiLU', 'Hardswish', 'LeakyReLU', 'Sigmoid', 'LogSigmoid', 'ELU', 'RReLU',
            'SELU', 'CELU', 'GELU', 'Mish', 'Softshrink', 'Tanh', 'Tanhshrink','Threshold', 'Softmax', 'LogSoftmax',
            'Softmin', 'Softsign', 'GLU', 'Hardshrink', 'MultiheadAttention', 'Hardsigmoid', 'PReLU', 'Softplus',
            'Softmax2d']
 
 
@@ -402,130 +405,141 @@
         self.inplace = inplace
 
     def forward(self, input):
         return ms_torch_nn_func.hardsigmoid(input, self.inplace)
 
 
 class MultiheadAttention(Module):
-    def __init__(self, embed_dim, num_heads, dropout=0.0, bias=True, add_bias_kv=False, \
-        add_zero_attn=False, kdim=None, vdim=None, batch_first=False, device=None, dtype=None):
-        super(MultiheadAttention, self).__init__()
-        if bias is not True:
-            raise ValueError(f"`bias` can only be set to 'True', but got {bias}")
-
-        if add_bias_kv:
-            raise ValueError(f"`add_bias_kv` can only be set to 'False', but got {add_bias_kv}")
-
-        if add_zero_attn:
-            raise ValueError(f"`add_zero_attn` can only be set to 'False', but got {add_zero_attn}")
-
-        unsupported_attr(kdim)
-        unsupported_attr(vdim)
+    def __init__(self, embed_dim, num_heads, dropout=0., bias=True, add_bias_kv=False, add_zero_attn=False,
+                 kdim=None, vdim=None, batch_first=False, device=None, dtype=None):
         unsupported_attr(device)
-
+        super(MultiheadAttention, self).__init__()
         self.embed_dim = embed_dim
+        self.kdim = kdim if kdim is not None else embed_dim
+        self.vdim = vdim if vdim is not None else embed_dim
+        self._qkv_same_embed_dim = self.kdim == embed_dim and self.vdim == embed_dim
+
         self.num_heads = num_heads
         self.dropout = dropout
-        self.add_bias_kv = add_bias_kv
-        self.add_zero_attn = add_zero_attn
-        self.kdim = kdim
-        self.vdim = vdim
         self.batch_first = batch_first
-        self.dtype = dtype
-
-        self.reduce_mean = ms.ops.ReduceMean()
-
-    def forward(self, query, key, value, key_padding_mask=None,
-                need_weights: bool=True, attn_mask=None,
-                average_attn_weights: bool=True):
-        unsupported_attr(key_padding_mask)
-        unsupported_attr(average_attn_weights)
-        if need_weights is True:
-            raise ValueError("Until now, `need_weights`='True' is not supported")
-
-        query = self._batch_tensor(query, 'query')
-        key = self._batch_tensor(key, 'key')
-        value = self._batch_tensor(value, 'value')
-        _batch_size = query.shape[0]
-        _src_seq_length = query.shape[1]
-        _tgt_seq_length = key.shape[1]
-
-        if attn_mask:
-            _attn_mask = self._process_mask(attn_mask, _batch_size)
+        self.head_dim = embed_dim // num_heads
+        if self.head_dim * num_heads != self.embed_dim:
+            raise ValueError("The init argument 'embed_dim' must be divisible by 'num_heads'.")
+
+        if self._qkv_same_embed_dim is False:
+            self.q_proj_weight = Parameter(empty((embed_dim, embed_dim), dtype=dtype))
+            self.k_proj_weight = Parameter(empty((embed_dim, self.kdim), dtype=dtype))
+            self.v_proj_weight = Parameter(empty((embed_dim, self.vdim), dtype=dtype))
+            self.in_proj_weight = None
         else:
-            _attn_mask = ms.ops.ones((_batch_size, _src_seq_length, _tgt_seq_length), mstype.float32)
+            self.in_proj_weight = Parameter(empty((3 * embed_dim, embed_dim), dtype=dtype))
+            self.q_proj_weight = None
+            self.k_proj_weight = None
+            self.v_proj_weight = None
 
-        self.ms_multihead_attention = ms.nn.transformer.MultiHeadAttention(
-            batch_size = _batch_size,
-            src_seq_length = _src_seq_length,
-            tgt_seq_length = _tgt_seq_length,
-            hidden_size=self.embed_dim,
-            num_heads=self.num_heads,
-            hidden_dropout_rate=self.dropout,
-            attention_dropout_rate=self.dropout,
-            compute_dtype=mstype.float32,
-            softmax_compute_type=mstype.float32,
-            param_init_type=mstype.float32,
-            use_past=False)
-        out, attn_output_weights = self.ms_multihead_attention(query, key, value, _attn_mask)
-
-        if not self.batch_first:
-            # ms default is (batch, seq, feature), batch_first
-            out = ms.ops.transpose(out, (1, 0, 2))
-
-        # if need_weights:
-        #     if average_attn_weights:
-        #         attn_output_weights = self.reduce_mean(attn_output_weights, 1)
-
-        #     if _batch_size == 1:
-        #         attn_output_weights = self.reduce_mean(attn_output_weights, 0)
-        # else:
-        #         attn_output_weights = None
-
-        if _batch_size == 1:
-            out = self.reduce_mean(out, 0)
-
-        # TODO
-        # Until Now, attn_output_weights is not the same as pytorch
-        attn_output_weights = None
-        return cast_to_adapter_tensor(out), cast_to_adapter_tensor(attn_output_weights)
-
-    def _batch_tensor(self, x, x_name: str):
-        x = cast_to_ms_tensor(x)
-        _rank = ms.ops.rank(x)
-        if _rank == 2:
-            out = ms.ops.expand_dims(x, 0)
-            return out
-
-        if _rank == 3:
-            if not self.batch_first:
-                out = ms.ops.transpose(x, (1, 0 ,2))
-            else:
-                out = x
-            return out
+        if bias:
+            self.in_proj_bias = Parameter(empty(3 * embed_dim, dtype=dtype))
+        else:
+            self.in_proj_bias = None
+        self.out_proj = Linear(embed_dim, embed_dim, bias=bias, dtype=dtype)
 
-        raise ValueError(f"For MultiheadAttention, rank of {x_name} should be 2 or 3, but got {_rank}")
+        if add_bias_kv:
+            self.bias_k = Parameter(empty((1, 1, embed_dim), dtype=dtype))
+            self.bias_v = Parameter(empty((1, 1, embed_dim), dtype=dtype))
+        else:
+            self.bias_k = self.bias_v = None
 
-    def _process_mask(self, mask, batch_size):
-        mask = cast_to_ms_tensor(mask)
-        _rank = ms.ops.rank(mask)
-        if _rank == 2:
-            out = ms.ops.expand_dims(mask, 0)
-            return out
-
-        if _rank == 3:
-            if mask.shape[0] != batch_size:
-                warnings.warn("Until now, `attn_mask` can only support shape (N, L, S)"
-                    "when `attn_mask` shape is (N * num_heads, L, S), pick the first (N, L, S) mask")
+        self.add_zero_attn = add_zero_attn
+        self.k_is_v = False
+        self.q_is_k = False
 
-            mask = mask[:batch_size,:]
-            return mask
+        self._reset_parameters()
 
-        raise ValueError(f"For MultiheadAttention, rank of mask should be 2 or 3, but got {_rank}")
+    def _reset_parameters(self):
+        if self._qkv_same_embed_dim:
+            xavier_uniform_(self.in_proj_weight)
+        else:
+            xavier_uniform_(self.q_proj_weight)
+            xavier_uniform_(self.k_proj_weight)
+            xavier_uniform_(self.v_proj_weight)
+
+        if self.in_proj_bias is not None:
+            constant_(self.in_proj_bias, 0.)
+            constant_(self.out_proj.bias, 0.)
+        if self.bias_k is not None:
+            xavier_normal_(self.bias_k)
+        if self.bias_v is not None:
+            xavier_normal_(self.bias_v)
+
+    def __call__(self, *args, **kwargs):
+        query = kwargs.get('query', args[0])
+        key = kwargs.get('key', args[1])
+        value = kwargs.get('value', args[2])
+        self.k_is_v = key is value
+        self.q_is_k = query is key
+        return super().__call__(*args, **kwargs)
+
+    def __setstate__(self, state):
+        # Support loading old MultiheadAttention checkpoints generated by v1.1.0
+        if '_qkv_same_embed_dim' not in state[1]:
+            state[1]['_qkv_same_embed_dim'] = True
+
+        super(MultiheadAttention, self).__setstate__(state)
+
+    def forward(self, query, key, value, key_padding_mask=None, need_weights=True, attn_mask=None,
+                average_attn_weights=True):
+        query = cast_to_ms_tensor(query)
+        key = cast_to_ms_tensor(key)
+        value = cast_to_ms_tensor(value)
+        key_padding_mask = cast_to_ms_tensor(key_padding_mask)
+        attn_mask = cast_to_ms_tensor(attn_mask)
+
+        is_batched = query.dim() == 3
+        if key_padding_mask is not None:
+            if key_padding_mask.dtype != ms.bool_ and not ms.ops.is_floating_point(key_padding_mask):
+                raise ValueError("only bool and floating types of key_padding_mask are supported")
+        if self.batch_first and is_batched:
+            # k_is_v and q_is_k preprocess in __call__ since Graph mode do not support `is`
+            if self.k_is_v:
+                if self.q_is_k:
+                    query = key = value = query.swapaxes(1, 0)
+                else:
+                    query, key = [x.swapaxes(1, 0) for x in (query, key)]
+                    value = key
+            else:
+                query, key, value = [x.swapaxes(1, 0) for x in (query, key, value)]
 
+        if not self._qkv_same_embed_dim:
+            # TODO: older ver of torch doesn't have is_causal arg
+            attn_output, attn_output_weights = ms_torch_nn_func.multi_head_attention_forward(
+                query, key, value, self.embed_dim, self.num_heads,
+                self.in_proj_weight, self.in_proj_bias,
+                self.bias_k, self.bias_v, self.add_zero_attn,
+                self.dropout, self.out_proj.weight, self.out_proj.bias,
+                training=self.training,
+                key_padding_mask=key_padding_mask,
+                attn_mask=attn_mask, use_separate_proj_weight=True,
+                q_proj_weight=self.q_proj_weight, k_proj_weight=self.k_proj_weight,
+                v_proj_weight=self.v_proj_weight, average_attn_weights=average_attn_weights,
+                k_is_v=self.k_is_v, q_is_k=self.q_is_k)
+        else:
+            attn_output, attn_output_weights = ms_torch_nn_func.multi_head_attention_forward(
+                query, key, value, self.embed_dim, self.num_heads,
+                self.in_proj_weight, self.in_proj_bias,
+                self.bias_k, self.bias_v, self.add_zero_attn,
+                self.dropout, self.out_proj.weight, self.out_proj.bias,
+                training=self.training,
+                key_padding_mask=key_padding_mask,
+                attn_mask=attn_mask, average_attn_weights=average_attn_weights,
+                k_is_v=self.k_is_v, q_is_k=self.q_is_k)
+        if self.batch_first and is_batched:
+            attn_output = attn_output.swapaxes(1, 0)
+        if need_weights:
+            return cast_to_adapter_tensor(attn_output), cast_to_adapter_tensor(attn_output_weights)
+        return (cast_to_adapter_tensor(attn_output),)
 
 class PReLU(Module):
     def __init__(self, num_parameters=1, init=0.25, device=None, dtype=None):
         super(PReLU, self).__init__()
         unsupported_attr(device)
         validator.check_positive_int(num_parameters, 'num_parameters', self.cls_name)
         if dtype is None:
@@ -583,10 +597,10 @@
 
 class Softmax2d(Module):
     def __init__(self):
         super(Softmax2d, self).__init__()
         self.softmax2d = ms.nn.Softmax2d()
 
     def forward(self, input):
-        if input.dim() not in {3, 4}:
+        if input.dim() not in (3, 4):
             raise RuntimeError("Softmax2d requires a 3D or 4D tensor as input")
         return self.softmax2d(input)
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/adaptive.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/adaptive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from collections import namedtuple
 
 import mindspore as ms
+from mindspore.ops.primitive import _primexpr
 from msadapter.pytorch.tensor import cast_to_ms_tensor, cast_to_adapter_tensor
-from msadapter.utils import unsupported_attr
+from msadapter.utils import unsupported_attr, pynative_mode_condition
 from .container import Sequential, ModuleList
 from .linear import Linear
 from .module import Module
 from ..functional import log_softmax
 
-_ASMoutput = namedtuple('_ASMoutput', ['output', 'loss'])
+@_primexpr
+def _ASMoutput():
+    return namedtuple('_ASMoutput', ['output', 'loss'])
 
 class AdaptiveLogSoftmaxWithLoss(Module):
     def __init__(self, in_features, n_classes, cutoffs, div_value=4., head_bias=False, device=None, dtype=None):
         super(AdaptiveLogSoftmaxWithLoss, self).__init__()
         unsupported_attr(device)
         cutoffs = list(cutoffs)
         # #TODO: pylint
@@ -135,15 +138,17 @@
         output += head_logprob.gather(1, gather_inds.unsqueeze(1)).squeeze()
         loss = (-output).mean()
         if not is_batched:
             output = output.squeeze(0)
 
         output = cast_to_adapter_tensor(output)
         loss = cast_to_adapter_tensor(loss)
-        return _ASMoutput(output, loss)
+        if pynative_mode_condition():
+            return _ASMoutput()(output, loss)
+        return output, loss
 
     def _get_full_log_prob(self, input, head_output):
         input = cast_to_ms_tensor(input)
         head_output = cast_to_ms_tensor(head_output)
         out = input.new_empty((head_output.shape[0], self.n_classes))
         head_logprob = log_softmax(head_output, dim=1)
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/batchnorm.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/batchnorm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import itertools
 
 import mindspore.ops as P
 from mindspore.ops.operations import _inner_ops as inner
 from mindspore.communication.management import get_group_size, get_rank
-from mindspore._checkparam import Validator as validator
-from mindspore._checkparam import Rel
+import mindspore._checkparam as validator
 from mindspore.communication import management
 import mindspore.context as context
 
 from msadapter.pytorch.nn import init
 from msadapter.pytorch.functional import empty
 from msadapter.pytorch.nn.parameter import Parameter
 from msadapter.utils import unsupported_attr
@@ -43,14 +42,17 @@
         self.num_features = num_features
         self.eps = eps
         self.momentum = momentum
         self.affine = affine
         self.track_running_stats = track_running_stats
         self.weight = Parameter(empty(num_features), requires_grad=affine)
         self.bias = Parameter(empty(num_features), requires_grad=affine)
+        # 'running_mean' and 'running_var' have to be Parameter
+        # because mindspore.ops.BatchNorm require them to be Parameter when 'is_training' is True
+        # so can not use register_buffer() for 'running_mean' and 'running_var'
         self.running_mean = Parameter(empty(num_features), requires_grad=False)
         self.running_var = Parameter(empty(num_features), requires_grad=False)
         self.reset_parameters()
         if not self.track_running_stats:
             self.momentum = 0.0
 
     def reset_running_stats(self):
@@ -95,15 +97,15 @@
 
     def _check_input_dim(self, input):
         raise NotImplementedError
 
     def _check_rank_ids(self, process_groups, rank_size):
         seen = set()
         for rid in itertools.chain(*process_groups):
-            validator.check_int_range(rid, 0, rank_size, Rel.INC_LEFT, "rank id in process_groups", self.cls_name)
+            validator.check_int_range(rid, 0, rank_size, validator.INC_LEFT, "rank id in process_groups", self.cls_name)
             if rid in seen:
                 raise ValueError(f"For '{self.cls_name}', rank id in 'process_groups' must not be duplicated, "
                                  f"but got {process_groups}.")
             seen.add(rid)
 
     def _create_sync_groups(self):
         for i in range(len(self.process_groups)):
@@ -134,27 +136,26 @@
                                    self.running_mean,
                                    self.running_var)[0]
         return cast_to_adapter_tensor(output)
 
 
 class BatchNorm1d(_BatchNorm):
     def _check_input_dim(self, input):
-        if len(input.shape) not in {2, 3}:
+        if len(input.shape) not in (2, 3):
             raise ValueError(
                 "expected 2D or 3D input (got {}D input)".format(input.dim())
             )
         return True
     def forward(self, input):
         self._check_input_dim(input)
 
         input = cast_to_ms_tensor(input)
         shape = input.shape
         if len(shape) == 3:
             input = input.transpose(0, 2, 1).reshape(-1, shape[1])
-        # TODO cast Parameter
             if self.training or (not self.training and not self.track_running_stats):
                 output = self.bn_train(input,
                                        self.weight,
                                        self.bias,
                                        self.running_mean,
                                        self.running_var)[0]
             else:
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/channelshuffle.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/channelshuffle.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/container.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/container.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from abc import abstractmethod
 import operator
+from itertools import chain
 from typing import Any, Dict, Iterable, Iterator, Mapping, Optional, Tuple, Union
 from collections import OrderedDict, abc as container_abcs
 from mindspore.nn.layer.container import _get_prefix_and_index, _valid_index, _valid_cell
 
 from msadapter.pytorch.tensor import Tensor, cast_to_adapter_tensor
 from msadapter.pytorch.nn.parameter import Parameter
 from msadapter.pytorch._ref import typename
@@ -93,18 +94,22 @@
                 self._is_dynamic_name.append(True)
         self.cell_list = list(self._cells.values())
 
     def __getitem__(self, index):
         if isinstance(index, slice):
             return self.__class__(
                 OrderedDict(list(self._cells.items())[index]))
+        if isinstance(index, Tensor):
+            index = int(index)
         index = _valid_index(len(self), index, self.__class__.__name__)
         return list(self._cells.values())[index]
 
     def __setitem__(self, index, module):
+        if isinstance(index, Tensor):
+            index = int(index)
         cls_name = self.__class__.__name__
         if _valid_cell(module, cls_name):
             prefix, _ = _get_prefix_and_index(self._cells)
             index = _valid_index(len(self), index, cls_name)
             key = list(self._cells.keys())[index]
             self._cells[key] = module
             module.update_parameters_name(prefix + key + ".")
@@ -137,14 +142,80 @@
                 temp_dict[key] = cell
         self._cells = temp_dict
         self.cell_list = list(self._cells.values())
 
     def __len__(self):
         return len(self._cells)
 
+    def __bool__(self):
+        return len(self._cells) != 0
+
+    def __add__(self, other):
+        if isinstance(other, Sequential):
+            ret = Sequential()
+            for layer in self:
+                self.append(ret, layer)
+            for layer in other:
+                self.append(ret, layer)
+            return ret
+        else:
+            raise ValueError('add operator supports only objects '
+                             'of Sequential class, but {} is given.'.format(
+                             str(type(other))))
+
+    def __iadd__(self, other):
+        if isinstance(other, Sequential):
+            offset = len(self)
+            for i, module in enumerate(other):
+                self.add_module(str(i + offset), module)
+            return self
+        else:
+            raise ValueError('add operator supports only objects '
+                             'of Sequential class, but {} is given.'.format(
+                             str(type(other))))
+
+    def __mul__(self, other):
+        if not isinstance(other, int):
+            raise TypeError(f"unsupported operand type(s) for *: {type(self)} and {type(other)}")
+        elif other <= 0:
+            raise ValueError(f"Non-positive multiplication factor {other} for {type(self)}")
+        else:
+            combined = Sequential()
+            offset = 0
+            for _ in range(other):
+                for module in self:
+                    combined.add_module(str(offset), module)
+                    offset += 1
+            return combined
+
+    def __rmul__(self, other):
+        return self.__mul__(other)
+
+    def __imul__(self, other):
+        if not isinstance(other, int):
+            raise TypeError(f"unsupported operand type(s) for *: {type(self)} and {type(other)}")
+        elif other <= 0:
+            raise ValueError(f"Non-positive multiplication factor {other} for {type(self)}")
+        else:
+            len_original = len(self)
+            offset = len(self)
+            for _ in range(other - 1):
+                for i in range(len_original):
+                    self.add_module(str(i + offset), self._cells[str(i)])
+                offset += len_original
+            return self
+
+    def __dir__(self):
+        keys = Module.__dir__(self)
+        keys = [key for key in keys if not key.isdigit()]
+        return keys
+
+    def __iter__(self):
+        return iter(self._cells.values())
+
     @property
     def _modules(self):
         return self._cells
 
     def set_grad(self, flag=True):
         self.requires_grad = flag
         for cell in self._cells.values():
@@ -173,14 +244,15 @@
         """
         if _valid_cell(module, self.__class__.__name__):
             prefix, _ = _get_prefix_and_index(self._cells)
             module.update_parameters_name(prefix + str(len(self)) + ".")
             self._is_dynamic_name.append(True)
             self._cells[str(len(self))] = module
         self.cell_list = list(self._cells.values())
+        return self
 
     def add_module(self, name, module):
         if not isinstance(module, Module) and module is not None:
             raise TypeError("{} is not a Module subclass".format(
                 module.__name__))
         elif hasattr(self, name) and name not in self._cells:
             raise KeyError("attribute '{}' already exists".format(name))
@@ -197,14 +269,50 @@
         self.cell_list = list(self._cells.values())
 
     def forward(self, input):
         for cell in self.cell_list:
             input = cell(input)
         return cast_to_adapter_tensor(input)
 
+    def pop(self, key):
+        v = self[key]
+        del self[key]
+        return v
+
+    def extend(self, sequential):
+        for layer in sequential:
+            self.append(layer)
+        return self
+
+    def insert(self, index, module):
+        """
+        Inserts a given Cell before a given index in the list.
+
+        Args:
+            index(int): The Insert index in the CellList.
+            cell(Cell): The Cell to be inserted.
+        """
+        cls_name = self.__class__.__name__
+        idx = _valid_index(len(self), index, cls_name)
+        _valid_cell(module, cls_name)
+        length = len(self)
+        prefix, key_index = _get_prefix_and_index(self._cells)
+        while length > idx:
+            if self._auto_prefix:
+                tmp_cell = self._cells[str(length-1)]
+                for _, param in tmp_cell.parameters_and_names():
+                    param.name = f'{prefix}{str(length)}{"."}{".".join(param.name.split(".")[key_index+1:])}'
+            self._cells[str(length)] = self._cells[str(length - 1)]
+            length -= 1
+        self._cells[str(idx)] = module
+        if self._auto_prefix:
+            module.update_parameters_name(prefix + str(idx) + ".")
+        self.cell_list = list(self._cells.values())
+        self._is_dynamic_name.insert(index, True)
+
 class _ModuleListBase:
     """
     An interface for base the Module as list.
 
     The sequential Module may be iterated using the construct method using for-in statement.
     But there are some scenarios that the construct method built-in does not fit.
     For convenience, we provide an interface that indicates the sequential
@@ -256,35 +364,41 @@
         _ModuleListBase.__init__(self)
         Module.__init__(self, auto_prefix)
         if len(args) == 1:
             self.extend(args[0])
 
 
     def __getitem__(self, index):
+        if isinstance(index, Tensor):
+            index = int(index)
         cls_name = self.__class__.__name__
         if isinstance(index, slice):
             return self.__class__(list(self._cells.values())[index])
         if isinstance(index, int):
             index = _valid_index(len(self), index, cls_name)
             return self._cells[str(index)]
         raise TypeError(f"For '{cls_name}', the type of 'index' must be int or slice, "
                         f"but got {type(index).__name__}.")
 
     def __setitem__(self, index, module):
+        if isinstance(index, Tensor):
+            index = int(index)
         cls_name = self.__class__.__name__
         if not isinstance(index, int) and _valid_cell(module, cls_name):
             raise TypeError(f"For '{cls_name}', the type of 'index' must be int, "
                             f"but got {type(index).__name__}.")
         index = _valid_index(len(self), index, cls_name)
         if self._auto_prefix:
             prefix, _ = _get_prefix_and_index(self._cells)
             module.update_parameters_name(prefix + str(index) + ".")
         self._cells[str(index)] = module
 
     def __delitem__(self, index):
+        if isinstance(index, Tensor):
+            index = int(index)
         cls_name = self.__class__.__name__
         if isinstance(index, int):
             index = _valid_index(len(self), index, cls_name)
             del self._cells[str(index)]
         elif isinstance(index, slice):
             keys = list(self._cells.keys())[index]
             for key in keys:
@@ -308,14 +422,25 @@
     def __iter__(self):
         return iter(self._cells.values())
 
     def __iadd__(self, modules):
         self.extend(modules)
         return self
 
+    def __add__(self, other):
+        combined = ModuleList()
+        for _, module in enumerate(chain(self, other)):
+            combined.append(module)
+        return combined
+
+    def pop(self, key):
+        v = self[key]
+        del self[key]
+        return v
+
     def insert(self, index, module):
         """
         Inserts a given Module before a given index in the list.
 
         Args:
             index(int): The Insert index in the ModuleList.
             module(Module): The Module to be inserted.
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/conv.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/conv.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import math
-from functools import lru_cache
+# from functools import lru_cache
 
 from mindspore.ops import operations as P
-from mindspore.ops import constexpr
+from mindspore.ops.primitive import _primexpr
 
 from msadapter.pytorch.nn.parameter import Parameter
 from msadapter.pytorch.nn import init
 from msadapter.pytorch.functional import empty
 from msadapter.utils import unsupported_attr
 from msadapter.pytorch.tensor import cast_to_ms_tensor, cast_to_adapter_tensor
-from msadapter.pytorch.nn.functional import conv2d, conv_transpose3d
-from .utils import _triple, _pair, _single, _reverse_repeat_tuple, _GLOBAL_LRU_CACHE_SIZE_NN
+from msadapter.pytorch.nn.functional import conv2d, conv_transpose3d, conv1d
+# from .utils import _triple, _pair, _single, _reverse_repeat_tuple, _GLOBAL_LRU_CACHE_SIZE_NN
+from .utils import _triple, _pair, _single, _reverse_repeat_tuple
 from .module import Module
 
 __all__ = ['Conv1d', 'Conv2d', 'Conv3d',
            'ConvTranspose1d', 'ConvTranspose2d', 'ConvTranspose3d',
            'LazyConv1d', 'LazyConv2d', 'LazyConv3d',
            'LazyConvTranspose1d', 'LazyConvTranspose2d', 'LazyConvTranspose3d']
 
@@ -51,14 +52,15 @@
         self.transposed = transposed
         self.output_padding = output_padding
         self.groups = groups
         self.padding_mode = padding_mode
         # MS add
         self.pad_mode = 'same'
         self.data_format = 'NCHW'
+        self.has_bias = bias
         if in_channels % groups != 0:
             raise ValueError('in_channels must be divisible by groups')
         if out_channels % groups != 0:
             raise ValueError('out_channels must be divisible by groups')
         valid_padding_strings = {'same', 'valid'}
         if isinstance(padding, str):
             if padding not in valid_padding_strings:
@@ -97,29 +99,26 @@
         if self.bias is not None:
             fan_in, _ = init._calculate_fan_in_and_fan_out(self.weight)
             if fan_in != 0:
                 bound = 1 / math.sqrt(fan_in)
                 init.uniform_(self.bias, -bound, bound)
 
     def extra_repr(self):
-        s = ('{in_channels}, {out_channels}, kernel_size={kernel_size}'
-             ', stride={stride}')
-        if self.padding != (0,) * len(self.padding):
-            s += ', padding={padding}'
-        if self.dilation != (1,) * len(self.dilation):
-            s += ', dilation={dilation}'
-        if self.output_padding != (0,) * len(self.output_padding):
-            s += ', output_padding={output_padding}'
-        if self.groups != 1:
-            s += ', groups={groups}'
-        if self.bias is None:
-            s += ', bias=False'
-        if self.padding_mode != 'zeros':
-            s += ', padding_mode={padding_mode}'
-        return s.format(**self.__dict__)
+        s = 'input_channels={}, output_channels={}, kernel_size={}, ' \
+            'stride={}, pad_mode={}, padding={}, dilation={}, ' \
+            'group={}, has_bias={}'.format(self.in_channels,
+                                           self.out_channels,
+                                           self.kernel_size,
+                                           self.stride,
+                                           self.pad_mode,
+                                           self.padding,
+                                           self.dilation,
+                                           self.groups,
+                                           self.has_bias)
+        return s
 
 
 class Conv1d(_ConvNd):
     r"""
         1D convolution layer.
 
         Calculates the 1D convolution on the input tensor which is typically of shape :math:`(N, C_{in}, L_{in})`,
@@ -148,70 +147,27 @@
         groups=1,
         bias=True,
         padding_mode='zeros',
         device=None,
         dtype=None
     ):
         factory_kwargs = {'device': device, 'dtype': dtype, 'transposed': False}
-        self.has_bias = False
-        if bias:
-            self.has_bias=True
-        kernel_size_ = (1, kernel_size) if isinstance(kernel_size, int) else (1, kernel_size[0])
-        stride_ = (1, stride if isinstance(stride, int) else stride[0])
-        dilation_ = (1, dilation) if isinstance(dilation, int) else (1, dilation[0])
+        kernel_size_ = _single(kernel_size)
+        stride_ = _single(stride)
         padding_ = padding if isinstance(padding, str) else _single(padding)
+        dilation_ = _single(dilation)
         super(Conv1d, self).__init__(in_channels, out_channels, kernel_size_, stride_, padding_, dilation_,
             _pair(0), groups, bias, padding_mode, **factory_kwargs)
 
         #TODO pad_mode in ['zeros', 'reflect', 'replicate', 'circular']
         if padding_mode in {'reflect', 'replicate', 'circular'}:
             raise ValueError("Pad mode '{}' is not currently supported.".format(padding_mode))
 
-        if padding == 0:
-            self.pad_mode = 'valid'
-            self.padding =(0, 0, 0, 0)
-        elif isinstance(self.padding, str):
-            self.pad_mode = self.padding
-            self.padding = 0
-        elif padding_mode == 'zeros':
-            self.pad_mode = "pad"
-            self.padding =(0, 0, padding, padding)
-
-        self.conv2d = P.Conv2D(out_channel=self.out_channels,
-                               kernel_size=self.kernel_size,
-                               mode=1,
-                               pad_mode=self.pad_mode,
-                               pad=self.padding,
-                               stride=self.stride,
-                               dilation=self.dilation,
-                               group=groups)
-        self.bias_add = P.BiasAdd()
-        self.expand_dims = P.ExpandDims()
-        self.squeeze = P.Squeeze(2)
-
     def forward(self, input):
-        input = cast_to_ms_tensor(input)
-        ndim = input.ndim
-        if ndim == 2:
-            input = input.expand_dims(0)
-            x = self.expand_dims(input, 2)
-            output = self.conv2d(x, self.weight)
-            if self.has_bias:
-                output = self.bias_add(output, self.bias)
-
-            output = self.squeeze(output)
-            output = output.squeeze(0)
-        else:
-            x = self.expand_dims(input, 2)
-            output = self.conv2d(x, self.weight)
-            if self.has_bias:
-                output = self.bias_add(output, self.bias)
-
-            output = self.squeeze(output)
-        return cast_to_adapter_tensor(output)
+        return conv1d(input, self.weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
 
 
 class Conv2d(_ConvNd):
     def __init__(self,
                  in_channels,
                  out_channels,
                  kernel_size,
@@ -279,18 +235,14 @@
         bias=True,
         padding_mode='zeros',
         device=None,
         dtype=None
     ):
         factory_kwargs = {'device': device, 'dtype': dtype, 'transposed': False}
 
-        self.has_bias = False
-        if bias:
-            self.has_bias=True
-
         kernel_size_ = _triple(kernel_size)
         stride_ = _triple(stride)
         padding_ = padding if isinstance(padding, str) else _triple(padding)
         dilation_ = _triple(dilation)
 
         super(Conv3d, self).__init__(in_channels, out_channels, kernel_size_, stride_, padding_, dilation_,
             _pair(0), groups, bias, padding_mode, **factory_kwargs)
@@ -335,16 +287,16 @@
         else:
             output = self.conv3d(input, self.weight)
             if self.has_bias:
                 output = self.bias_add(output, self.bias)
         return cast_to_adapter_tensor(output)
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _output_padding(output_padding, input_ndim, input_shape, output_size,
                     stride, padding, kernel_size,
                     num_spatial_dims, dilation=None):
     if output_size is None:
         ret = _single(output_padding)
     else:
         has_batch_dim = input_ndim == num_spatial_dims + 2
@@ -413,18 +365,14 @@
         dilation=1,
         padding_mode='zeros',
         device=None,
         dtype=None,
     ):
         factory_kwargs = {'device': device, 'dtype': dtype, 'transposed': True}
 
-        self.has_bias = False
-        if bias:
-            self.has_bias=True
-
         _padding = _single(padding)
         _kernel_size = (1, kernel_size) if isinstance(kernel_size, int) else (1, kernel_size[0])
         _stride = (1, stride) if isinstance(stride, int) else (1, stride[0])
         _dilation = (1, dilation) if isinstance(dilation, int) else (1, dilation[0])
 
         super(ConvTranspose1d, self).__init__(in_channels, out_channels, _kernel_size, _stride,
                                               _padding, _dilation, output_padding, groups, bias,
@@ -459,15 +407,15 @@
                                                       stride=self.stride,
                                                       dilation=self.dilation,
                                                       group=groups)
         self.bias_add = P.BiasAdd()
         self.expand_dims = P.ExpandDims()
         self.squeeze = P.Squeeze(2)
 
-    def construct(self, input, output_size=None):
+    def forward(self, input, output_size=None):
         if output_size is not None:
             raise ValueError("output_size '{}' is not currently supported.".format(output_size))
 
         x = cast_to_ms_tensor(input)
         ndim = x.ndim
         if ndim == 2:
             x = x.expand_dims(0)
@@ -499,30 +447,14 @@
 
             if self.has_bias:
                 output = self.bias_add(output, self.bias)
 
             output = self.squeeze(output)
         return cast_to_adapter_tensor(output)
 
-    def extend_repr(self):
-        s = 'input_channels={}, output_channels={}, kernel_size={}, ' \
-            'stride={}, pad_mode={}, padding={}, dilation={}, ' \
-            'group={}, has_bias={}, ' \
-            'weight_init={}'.format(self.in_channels,
-                                    self.out_channels,
-                                    self.kernel_size,
-                                    self.stride,
-                                    self.pad_mode,
-                                    self.padding,
-                                    self.dilation,
-                                    self.group,
-                                    self.bias,
-                                    self.weight_init,
-                                    )
-        return s
 
 
 class ConvTranspose2d(_ConvNd):
     r"""
     2D transposed convolution layer.
 
     Calculates a 2D transposed convolution, which can be regarded as Conv2d for the gradient of the input.
@@ -552,18 +484,14 @@
         dilation=1,
         padding_mode='zeros',
         device=None,
         dtype=None
     ):
         factory_kwargs = {'device': device, 'dtype': dtype, 'transposed': True}
 
-        self.has_bias = False
-        if bias:
-            self.has_bias=True
-
         _kernel_size = _pair(kernel_size)
         _stride = _pair(stride)
         _padding = _pair(padding)
         _dilation = _pair(dilation)
         output_padding = _pair(output_padding)
 
         super(ConvTranspose2d, self).__init__(in_channels, out_channels, _kernel_size, _stride, _padding, _dilation,
@@ -626,27 +554,14 @@
             w_out = _deconv_output_length(self.is_valid, self.is_same, self.is_pad, w, self.kernel_size[1],
                                           self.stride[1], self.dilation[1], self.padding_left + self.padding_right)
             output = self.conv2d_transpose(x, self.weight, (n, self.out_channels, h_out, w_out))
             if self.has_bias:
                 output = self.bias_add(output, self.bias)
         return cast_to_adapter_tensor(output)
 
-    def extend_repr(self):
-        s = 'input_channels={}, output_channels={}, kernel_size={}, ' \
-            'stride={}, pad_mode={}, padding={}, dilation={}, ' \
-            'group={}, has_bias={}'.format(self.in_channels,
-                                                  self.out_channels,
-                                                  self.kernel_size,
-                                                  self.stride,
-                                                  self.pad_mode,
-                                                  self.padding,
-                                                  self.dilation,
-                                                  self.group,
-                                                  self.has_bias)
-        return s
 
 
 class ConvTranspose3d(_ConvNd):
     r"""
        3D transposed convolution layer.
 
        Calculates a 3D transposed convolution, which can be regarded as Conv3d for the gradient of the input.
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/distance.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/distance.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/dropout.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/dropout.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/flatten.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/flatten.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/fold.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/fold.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/linear.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/linear.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,20 +88,17 @@
 
 
 class Identity(Module):
     def __init__(self, *args, **kwargs):
         super(Identity, self).__init__()
         unsupported_attr(args)
         unsupported_attr(kwargs)
-        self.identity = P.Identity()
 
     def forward(self, input):
-        input = cast_to_ms_tensor(input)
-        output = self.identity(input)
-        return cast_to_adapter_tensor(output)
+        return input
 
 LazyLinear = Linear
 
 class Bilinear(Module):
     def __init__(self, in1_features, in2_features, out_features, bias=True, device=None, dtype=None):
         super(Bilinear, self).__init__()
         self.in1_features = in1_features
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/loss.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,24 +275,20 @@
         input = cast_to_ms_tensor(input)
         target = cast_to_ms_tensor(target)
         out = self.hinge_embedding_loss(input, target)
         return cast_to_adapter_tensor(out)
 
 
 class MultiLabelMarginLoss(_Loss):
-    def __init__(self, size_average=None, reduce=None, reduction='mean'):
-        super(MultiLabelMarginLoss, self).__init__(size_average, reduce, reduction)
-        self.multilabel_margin_loss = ms.ops.MultilabelMarginLoss(reduction=self.reduction)
-
     def forward(self, input, target):
         input = cast_to_ms_tensor(input)
         target = cast_to_ms_tensor(target)
         if target.dtype == ms.int64:
             target = target.astype(ms.int32)
-        out = self.multilabel_margin_loss(input, target)
+        out = ms.ops.multilabel_margin_loss(input, target, self.reduction)
         return cast_to_adapter_tensor(out)
 
 
 class MultiLabelSoftMarginLoss(_WeightedLoss):
     def __init__(self, weight=None, size_average=None, reduce=None, reduction='mean'):
         super(MultiLabelSoftMarginLoss, self).__init__(weight, size_average, reduce, reduction)
         self.multilabel_soft_margin_loss = nn.MultiLabelSoftMarginLoss(weight=self.weight, reduction=self.reduction)
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/normalization.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/normalization.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/padding.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/padding.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,21 @@
 
     def __init__(self, padding):
         super(ReflectionPad3d, self).__init__(padding)
         self.pad_fun = nn.ReflectionPad3d(self.padding)
 
     def forward(self, input):
         input = cast_to_ms_tensor(input)
-        output = self.pad_fun(input)
+        if input.ndim == 5:
+            input_shape = input.shape
+            input = input.reshape((-1,) + input_shape[2:])
+            output = self.pad_fun(input)
+            output = output.reshape(input_shape[0:2] + output.shape[1:])
+        else:
+            output = self.pad_fun(input)
         return cast_to_adapter_tensor(output)
 
 
 class ZeroPad2d(ConstantPad2d):
     r"""Pads the input tensor boundaries with zero.
 
     For `N`-dimensional padding, use :func:`torch.nn.functional.pad()`.
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/pixel_shuffle.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/pixel_shuffle.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/pooling.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/pooling.py`

 * *Files 5% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         """Initialize AdaptiveMaxPool1d."""
         super(AdaptiveAvgPool1d, self).__init__(output_size)
         self.expand = P.ExpandDims()
         self.squeeze = P.Squeeze(2)
         self.output_size = output_size
         self.shape = F.shape
 
-    def construct(self, input):
+    def forward(self, input):
         input = cast_to_ms_tensor(input)
         _, _, width = self.shape(input)
         stride = width // self.output_size
         kernel_size = width - (self.output_size - 1) * stride
         stride = (1, width // self.output_size)
         kernel_size = (1, kernel_size)
 
@@ -223,47 +223,22 @@
         self.return_indices = return_indices
 
     def extra_repr(self) -> str:
         return 'output_size={}'.format(self.output_size)
 
 
 class AdaptiveMaxPool1d(_AdaptiveMaxPoolNd):
-
-    def __init__(self, output_size, return_indices = False):
+    def __init__(self, output_size, return_indices=False):
         """Initialize AdaptiveMaxPool1d."""
         super(AdaptiveMaxPool1d, self).__init__(output_size, return_indices)
-        self.expand = P.ExpandDims()
-        self.squeeze = P.Squeeze(2)
         self.output_size = output_size
-        self.shape = F.shape
         self.return_indices = return_indices
 
-    def construct(self, input):
-        input = cast_to_ms_tensor(input)
-        _, _, width = self.shape(input)
-        stride = width // self.output_size
-        kernel_size = width - (self.output_size - 1) * stride
-        stride = (1, width // self.output_size)
-        kernel_size = (1, kernel_size)
-        if self.return_indices:
-            max_pool = P.MaxPoolWithArgmax(kernel_size=kernel_size, strides=stride,
-                                            pad_mode='valid', data_format="NCHW")
-            x = self.expand(input, 2)
-            x, idx = max_pool(x)
-            x = self.squeeze(x)
-            # TODO: to avoid ascend not return ms.int32 but ms.uint16
-            idx = idx.astype(ms.int32)
-            idx = self.squeeze(idx)
-            return cast_to_adapter_tensor((x, idx))
-        else:
-            max_pool = P.MaxPool(kernel_size=kernel_size, strides=stride, pad_mode="valid", data_format="NCHW")
-            x = self.expand(input, 2)
-            x = max_pool(x)
-            x = self.squeeze(x)
-            return cast_to_adapter_tensor(x)
+    def forward(self, input):
+        return Adapter_F.adaptive_max_pool1d(input, self.output_size, self.return_indices)
 
 
 class AdaptiveMaxPool2d(_AdaptiveMaxPoolNd):
     def forward(self, input):
         input = cast_to_ms_tensor(input)
         if is_under_ascend_context() and len(input.shape) == 3:
             input = ms.ops.expand_dims(input, 0)
@@ -275,53 +250,24 @@
                 output = ms.ops.squeeze(output, 0)
         else:
             output = ms.ops.adaptive_max_pool2d(input, self.output_size, self.return_indices)
         return cast_to_adapter_tensor(output)
 
 
 class AdaptiveMaxPool3d(_AdaptiveMaxPoolNd):
-    def __init__(self, output_size, return_indices = False):
+    def __init__(self, output_size, return_indices=False):
+        # TODO: not support `return_indices` yet
+        if return_indices and is_under_ascend_context():
+            raise NotImplementedError('AdaptiveMaxPool3d doesn\'t  support return_indices on Ascend now.')
         super(AdaptiveMaxPool3d, self).__init__(output_size, return_indices)
-        self.output_size = output_size
-        self.shape = P.Shape()
-        if not isinstance(self.output_size, Iterable):
-            self.output_size = [self.output_size, ] * 3
-        self.condition = [0,] * 3
-        if None in self.output_size:
-            self.output_size = list(self.output_size)
-            if self.output_size[0] is None:
-                self.condition [0] = 1
-                self.output_size[0] = 0
-            if self.output_size[1] is None:
-                self.condition [1] = 1
-                self.output_size[1] = 0
-            if self.output_size[2] is None:
-                self.condition[2] = 1
-                self.output_size[2] = 0
-        if return_indices:
-            raise NotImplementedError('AdaptiveMaxPool3d doesn\'t  support return_indices now.')
-
+        self.return_indices = return_indices
 
     def forward(self, input):
-        input = cast_to_ms_tensor(input)
-        _, _, d, h, w = self.shape(input)
-        out_d = self.output_size[0] + self.condition[0] * d
-        out_h = self.output_size[1] + self.condition[1] * h
-        out_w = self.output_size[2] + self.condition[2] * w
-        stride_d = d // out_d
-        kernel_d = d - (out_d - 1) * stride_d
-        stride_h = h // out_h
-        kernel_h = h - (out_h - 1) * stride_h
-        stride_w = w // out_w
-        kernel_w = w - (out_w - 1) * stride_w
-        avg_pool = P.MaxPool3D(kernel_size=(kernel_d, kernel_h, kernel_w),
-                                strides=(stride_d, stride_h, stride_w),
-                                pad_mode="valid", data_format="NCDHW")
-        outputs = avg_pool(input)
-        return cast_to_adapter_tensor(outputs)
+        outputs = Adapter_F.adaptive_max_pool3d(input, self.output_size, self.return_indices)
+        return outputs
 
 
 class _LPPoolNd(Module):
     def __init__(self, norm_type, kernel_size, stride = None,
                  ceil_mode = False):
         super(_LPPoolNd, self).__init__()
         self.norm_type = norm_type
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/rnn.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/rnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,17 +231,15 @@
 
         if num_directions == 1:
             for i in range(self.num_layers):
                 w_ih, w_hh, b_ih, b_hh = self._get_weight_and_bias(num_directions, i, self.bias)
                 output, h_t = self.rnn_cell(pre_layer, hx[i], None, w_ih, w_hh, b_ih, b_hh)
                 h_n += (h_t,)
 
-                #TODO：modified after version upgrading
-                #pre_layer = ms.ops.dropout(output, 1 - self.dropout) \
-                pre_layer = ms.ops.dropout(output, 1 - self.dropout)[0] \
+                pre_layer = ms.ops.dropout(output, 1 - self.dropout) \
                     if (self.dropout != 0 and i < self.num_layers - 1) else output
         else:
             for i in range(self.num_layers):
                 w_ih, w_hh, b_ih, b_hh, w_ih_b, w_hh_b, b_ih_b, b_hh_b = \
                     self._get_weight_and_bias(num_directions, i, self.bias)
 
                 x_b = ms.ops.reverse(pre_layer, [0])
@@ -249,18 +247,16 @@
                 output_b, h_t_b = self.rnn_cell(x_b, hx[2 * i + 1], None, w_ih_b, w_hh_b, b_ih_b, b_hh_b)
 
                 output_b = ms.ops.reverse(output_b, [0])
                 output = ms.ops.concat((output, output_b), 2)
                 h_n += (h_t,)
                 h_n += (h_t_b,)
 
-                #TODO：modified after version upgrading
-                #pre_layer = ms.ops.dropout(output, 1 - self.dropout) \
-                pre_layer = ms.ops.dropout(output, 1 - self.dropout)[0] \
-                            if (self.dropout != 0 and i < self.num_layers - 1) else output
+                pre_layer = ms.ops.dropout(output, 1 - self.dropout) \
+                    if (self.dropout != 0 and i < self.num_layers - 1) else output
 
         h_n = ms.ops.concat(h_n, 0)
         h_n = h_n.view(hx.shape)
 
         if not is_batched:
             output = ms.ops.squeeze(output, 1)
             h_n = ms.ops.squeeze(h_n, 1)
@@ -362,18 +358,16 @@
 
                 h_i = (hx[0][i], hx[1][i])
                 output, hc_t = self.lstm_cell(pre_layer, h_i, None, w_ih, w_hh, b_ih, b_hh)
                 h_t, c_t = hc_t
                 h_n += (h_t,)
                 c_n += (c_t,)
 
-                #TODO：modified after version upgrading
-                #pre_layer = ms.ops.dropout(output, 1 - self.dropout) \
-                pre_layer = ms.ops.dropout(output, 1 - self.dropout)[0] \
-                            if (self.dropout != 0 and i < self.num_layers - 1) else output
+                pre_layer = ms.ops.dropout(output, 1 - self.dropout) \
+                    if (self.dropout != 0 and i < self.num_layers - 1) else output
         else:
             for i in range(self.num_layers):
                 w_ih, w_hh, b_ih, b_hh, w_ih_b, w_hh_b, b_ih_b, b_hh_b = \
                     self._get_weight_and_bias(num_directions, i, self.bias)
 
                 x_b = ms.ops.reverse(pre_layer, [0])
                 h_i = (hx[0][2 * i], hx[1][2 * i])
@@ -386,18 +380,16 @@
                 h_t, c_t = hc_t
                 h_t_b, c_t_b = hc_t_b
                 h_n += (h_t,)
                 h_n += (h_t_b,)
                 c_n += (c_t,)
                 c_n += (c_t_b,)
 
-                #TODO：modified after version upgrading
-                #pre_layer = ms.ops.dropout(output, 1 - self.dropout) \
-                pre_layer = ms.ops.dropout(output, 1 - self.dropout)[0] \
-                            if (self.dropout != 0 and i < self.num_layers - 1) else output
+                pre_layer = ms.ops.dropout(output, 1 - self.dropout) \
+                    if (self.dropout != 0 and i < self.num_layers - 1) else output
 
         h_n = ms.ops.concat(h_n, 0)
         h_n = h_n.view(hx[0].shape)
         c_n = ms.ops.concat(c_n, 0)
         c_n = c_n.view(hx[1].shape)
         if not is_batched:
             output = ms.ops.squeeze(output, 1)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/sparse.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/sparse.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/unpooling.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/unpooling.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/upsampling.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/upsampling.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/utils.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import collections
 from itertools import repeat
-from functools import lru_cache
+# from functools import lru_cache
 import mindspore as ms
 from mindspore.ops._primitive_cache import _get_cache_prim
-from mindspore.ops import constexpr
-from msadapter.utils import unsupported_attr,_GLOBAL_LRU_CACHE_SIZE, _GLOBAL_LRU_CACHE_SIZE_NN
+from mindspore.ops.primitive import _primexpr
+# from msadapter.utils import unsupported_attr,_GLOBAL_LRU_CACHE_SIZE, _GLOBAL_LRU_CACHE_SIZE_NN
+from msadapter.utils import unsupported_attr
 
 
 def _ntuple(n, name="parse"):
     def parse(x):
         if isinstance(x, (list, tuple)) and len(x) == 1:
             x = x[0]
         if isinstance(x, collections.abc.Iterable):
@@ -51,27 +52,27 @@
     Example:
         network-type padding: (padH, padW)
         function-pad-type padding:  (padH, padH, padW, padW)
     """
     return tuple(x for x in t for _ in range(n))
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE)
 def _is_zero_paddings(padding):
     if isinstance(padding, int):
         if padding == 0:
             return True
     elif isinstance(padding, collections.abc.Iterable):
         if not any(padding):
             return True
     return False
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _expand_padding_for_padv1(network_padding, x_ndim):
     r"""
     use for to get expand padding for ms.ops.Pad.
     `network_padding` must be type of iterable.
 
     Example:
         x_ndim = 4
@@ -88,16 +89,16 @@
         _pad.append(_pair(p))
     for _ in range(len(_pad), x_ndim):
         _pad.insert(0, (0, 0))
 
     return tuple(_pad)
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE_NN)
 def _reverse_padding(network_padding):
     r"""
     Reverse padding from network-type padding to functional.pad type padding.
 
     Example:
         network-type padding: (padH, padW)
         function-pad-type padding:  (padW, padW, padH, padH)
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/modules/__init__.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/modules/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .dropout import Dropout, Dropout1d, Dropout2d, Dropout3d, AlphaDropout, FeatureAlphaDropout
 from .upsampling import *
 from .normalization import *
 from .pixel_shuffle import *
 from .channelshuffle import *
 from .fold import *
 from .adaptive import AdaptiveLogSoftmaxWithLoss
+from .transformer import *
 
 __all__ = [
     'Linear',
     'LazyLinear',
     'Bilinear',
     'Flatten',
     'Unflatten',
@@ -179,9 +180,15 @@
     'CosineSimilarity',
 
     'Embedding',
 
     'PixelShuffle',
     'PixelUnshuffle',
 
-    'ChannelShuffle'
+    'ChannelShuffle',
+
+    'TransformerEncoderLayer',
+    'TransformerDecoderLayer',
+    'TransformerEncoder',
+    'TransformerDecoder',
+    'Transformer'
 ]
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/nn/parameter.py` & `msadapter-0.1.0rc0/msadapter/pytorch/nn/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 import numbers
 from copy import copy
 
 import mindspore as ms
 import mindspore.common.dtype as mstype
 from mindspore.common.initializer import initializer
-from mindspore._checkparam import Validator
+import mindspore._checkparam as Validator
 from mindspore._c_expression import Tensor as Tensor_
 from mindspore.parallel._tensor import _get_slice_index
 from mindspore.parallel._auto_parallel_context import auto_parallel_context
 from mindspore.parallel._ps_context import _is_role_worker, _is_role_sched, _clone_hash_table
 from mindspore.parallel._ps_context import _insert_accumu_init_info
 from mindspore.ops import functional as F
 from msadapter.pytorch.tensor import Tensor, cast_to_adapter_tensor
@@ -84,17 +84,17 @@
         data = self
         if self.init_mode is not None:
             data = self.init_mode
         else:
             # cast to break deep infinite loop while deepcopy
             data = Tensor(self)
         return (
-            Parameter, (data, self.name, self.requires_grad, self.layerwise_parallel))
+            Parameter, (data, self.requires_grad, self.name, self.layerwise_parallel))
 
-    def __init__(self, data, name=None, requires_grad=True, layerwise_parallel=False, parallel_optimizer=True):
+    def __init__(self, data, requires_grad=True, name=None, layerwise_parallel=False, parallel_optimizer=True):
         super().__init__(default_input=data, name=name, requires_grad=requires_grad,
                          layerwise_parallel=layerwise_parallel, parallel_optimizer=parallel_optimizer)
 
     def __deepcopy__(self, memodict):
         new_obj = Parameter(self)
         new_obj.name = self.name
         new_obj._inited_param = self._inited_param
@@ -309,14 +309,17 @@
         obj.init_mode = None
         obj.sliced = set_sliced
         return obj
 
     def requires_grad_(self, requires_grad=True):
         self.requires_grad = requires_grad
 
+    def detach(self):
+        return cast_to_adapter_tensor(ms.Parameter.value(self))
+
 class ParameterTuple(tuple):
     """
     Inherited from tuple, ParameterTuple  is used to save multiple parameter.
 
     Note:
         It is used to store the parameters of the network into the parameter tuple collection.
     """
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/optim/__init__.py` & `msadapter-0.1.0rc0/msadapter/pytorch/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/serialization.py` & `msadapter-0.1.0rc0/msadapter/pytorch/serialization.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/storage.py` & `msadapter-0.1.0rc0/msadapter/pytorch/storage.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/tensor.py` & `msadapter-0.1.0rc0/msadapter/pytorch/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-import collections
 import warnings
 import numbers
 import operator
-from functools import reduce, lru_cache
+# from functools import reduce, lru_cache
+from functools import reduce
 import numpy as np
 import mindspore as ms
+from mindspore import vmap
+import mindspore.scipy.linalg as ms_linalg
 from mindspore.common import dtype as mstype
-from mindspore.common._register_for_tensor import tensor_operator_registry
 import mindspore.ops as P
-from mindspore.ops import constexpr
+from mindspore.ops.primitive import _primexpr
 from mindspore.ops._primitive_cache import _get_cache_prim
 from mindspore.ops.operations import _inner_ops as inner
 from mindspore.common.initializer import _init_random_normal, _init_random_uniform, Zero
 from mindspore._c_expression import Tensor as Tensor_
-from mindspore._checkparam import Validator as validator
+
 from msadapter.utils import unsupported_attr, is_under_gpu_context, get_backend, \
                              is_under_ascend_context, _infer_size, _ascend_tensor_general_cast,\
-                             is_under_cpu_context, _GLOBAL_LRU_CACHE_SIZE
+                             is_under_cpu_context, ascend_raise_implement_error,\
+                             pynative_mode_condition, set_name_tuple
 import msadapter.pytorch.common.dtype as msdapter_dtype
 from msadapter.pytorch.common.device import Device
 from msadapter.pytorch.storage import _TypedStorage
 from msadapter.pytorch.common import pi
+from msadapter.pytorch._register_numpy_primitive import NumpyLstsq
 
 _dtypeDict = {
     'float16': mstype.float16,
     'float32': mstype.float32,
     'float64': mstype.float64,
     'int8': mstype.int8,
     'int16': mstype.int16,
@@ -93,16 +96,16 @@
     'ShortTensor': msdapter_dtype.int16,
     'IntTensor': msdapter_dtype.int32,
     'LongTensor': msdapter_dtype.int64,
     'BoolTensor': msdapter_dtype.bool
 }
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE)
 def _get_flatten_dst_shape(input_shape, start_dim, end_dim):
     rank = len(input_shape)
     if start_dim >= rank or start_dim < -rank:
         raise ValueError(f"Dimension out of range (expected to be in range of [{-rank}, "
                             f"{rank - 1}], but got {start_dim})")
 
     if end_dim >= rank or end_dim < -rank:
@@ -117,16 +120,16 @@
 
     dst_shape = list(input_shape[:start])
     dst_shape.append(-1)
     dst_shape.extend(list(input_shape[end + 1:]))
     return tuple(dst_shape)
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE)
 def _get_unflatten_size(input_shape, dim, sizes):
     input_rank = len(input_shape)
     if not isinstance(sizes, (tuple, list)):
         raise TypeError(f"Type of `sizes` should be `Tuple` or `List`, but got {type(sizes)}")
 
     if len(sizes) == 0:
         raise ValueError("`sizes` must be non-empty")
@@ -146,44 +149,43 @@
         raise ValueError(f"unflatten: Provided `sizes` {sizes} don't multiply up to the"
             f"size of dim {dim} ({input_shape[_dim]}) in the input tensor")
 
     out_shape = input_shape[:_dim] + tuple(sizes) + input_shape[_dim + 1:]
     return out_shape
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE)
 def _get_slice_scatter_const(x_shape, dim, start, end, step):
     x_rank = len(x_shape)
     dim = dim if dim >= 0 else dim + x_rank
     start = start if start else 0
     end = end if end else x_shape[dim]
     index = list(range(start, end, step))
     return x_rank, index, dim
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE)
 def _get_select_out_shape(input_shape, dim):
     shape = [input_shape[i] for i in range(len(input_shape)) if i != dim]
     return tuple(shape)
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE)
 def _get_unfold_indices(input_shape, dimension, size, step):
     if dimension < 0:
         dimension += len(input_shape)
     indices = []
     for i in range(0, input_shape[dimension] - size + 1, step):
         indices.append(list(range(i, i + size)))
 
     return indices, dimension
 
-
 class Tensor(ms.Tensor):
     def __init__(self, *data, dtype=None, inner=False, internal=False):
         def _process_data(data):
             _shape = None
             _input_data = None
             if len(data) == 1:
                 if isinstance(data[0], int):
@@ -216,22 +218,28 @@
         if inner is True:
             super(Tensor, self).__init__(*data, dtype=dtype)
         else:
             _input_data, _shape = _process_data(data)
             if _shape:
                 if dtype is None:
                     dtype = mstype.float32
-                super(Tensor, self).__init__(shape=_shape, dtype=dtype, init=Zero())
+                init_func = Zero()
+                init_func.__enable_zero_dim__ = True
+                super(Tensor, self).__init__(shape=_shape, dtype=dtype, init=init_func)
                 self.init_data()
             else:
                 if dtype is None:
                     if not isinstance(_input_data, (ms.Tensor, Tensor_, _TypedStorage)):
                         dtype=mstype.float32
                 super(Tensor, self).__init__(input_data=_input_data, dtype=dtype)
 
+    def __deepcopy__(self, memodict):
+        tensor_ms = cast_to_ms_tensor(self)
+        return Tensor(ms.Tensor.__deepcopy__(tensor_ms, memodict))
+
     def __neg__(self):
         tensor_ms = cast_to_ms_tensor(self)
         out = tensor_ms.__neg__()
         return cast_to_adapter_tensor(out)
 
     def __invert__(self):
         tensor_ms = cast_to_ms_tensor(self)
@@ -455,17 +463,16 @@
         if isinstance(index, ms.Tensor) and index.dtype == ms.bool_:
             # TODO: delete here after support to reshape empty tensor
             # TODO: not support GRAPH_MODE
             if not np.count_nonzero(index.asnumpy()):
                 out_shape = list(tensor_ms.shape[len(index.shape) - 1:])
                 out_shape[0] = 0
                 out_shape = tuple(out_shape)
-                #TODO: if switch the mindspore version, change the code to
-                # out = _get_cache_prim(ms.ops.Zeros)()(out_shape, tensor_ms.dtype)
-                out = ms.ops.zeros(out_shape, dtype=tensor_ms.dtype)
+                #TODO: ms.ops.zeros() currently has preblem handling input shape including 0
+                out = _get_cache_prim(ms.ops.Zeros)()(out_shape, tensor_ms.dtype)
                 return out
             ms_shape_len = len(tensor_ms.shape)
             index_shape_len = len(index.shape)
             out_shape = [-1]
             while index_shape_len < ms_shape_len:
                 out_shape.append(tensor_ms.shape[index_shape_len])
                 index = index.expand_dims(-1)
@@ -484,17 +491,16 @@
                         scale[i] = 0
                         tmp_shape[i] = 1
                 tmp_tensor = ms.ops.zeros(tuple(tmp_shape), dtype=tensor_ms.dtype)
                 tmp_out = tmp_tensor.__getitem__(index)
                 out_shape = list(tmp_out.shape)
                 for i in range(len(out_shape)):
                     out_shape[i] = out_shape[i] * scale[i]
-                #TODO: if switch the mindspore version, change the code to
-                #out = _get_cache_prim(ms.ops.Zeros)()(tuple(out_shape), tensor_ms.dtype)
-                out = ms.ops.zeros(tuple(out_shape), dtype=tensor_ms.dtype)
+                #TODO: ms.ops.zeros() currently has preblem handling input shape including 0
+                out = _get_cache_prim(ms.ops.Zeros)()(tuple(out_shape), tensor_ms.dtype)
             else:
                 out = tensor_ms.__getitem__(index)
         return out
 
     def __getitem__(self, index):
         out = cast_to_adapter_tensor(self._getitem_handler(index))
         if out is not self:
@@ -582,27 +588,24 @@
         output = ms.ops.fill(self.dtype, self.shape, 0.0)
         return cast_to_adapter_tensor(output)
 
     def zero_(self):
         output = self.zero_adapter()
         return _tensor_inplace_assign(self, output, "zero_", "zero_adapter")
 
-    def new_zeros(self, size, *, dtype=None, device=None, requires_grad=False, layout=None, pin_memory=False):
+    def new_zeros(self, *size, dtype=None, device=None, requires_grad=False):
         unsupported_attr(device)
         unsupported_attr(requires_grad)
-        unsupported_attr(layout)
-        if layout:
-            raise NotImplementedError("layout is not supported.")
-        unsupported_attr(pin_memory)
-        if pin_memory is True:
-            raise NotImplementedError("pin_memory is not supported to True.")
 
         if not dtype:
             dtype = self.dtype
 
+        if isinstance(size[0], tuple):
+            size = size[0]
+
         output = ms.ops.fill(dtype, size, 0.0)
         return cast_to_adapter_tensor(output)
 
     def new_full(self, size, fill_value, *, dtype=None, device=None, requires_grad=False,
                  layout=None, pin_memory=False):
         unsupported_attr(device)
         unsupported_attr(requires_grad)
@@ -671,15 +674,20 @@
         if isinstance(size[0], (list, tuple)):
             size = size[0]
         out = ms.ops.broadcast_to(input_ms, size)
         return cast_to_adapter_tensor(out)
 
     def sigmoid(self):
         input = cast_to_ms_tensor(self)
-        output = _get_cache_prim(P.Sigmoid)()(input)
+        if is_under_ascend_context() and input.dtype == ms.float64:
+            input = input.astype(ms.float32)
+            output = ms.ops.sigmoid(input)
+            output = output.astype(ms.float64)
+        else:
+            output = ms.ops.sigmoid(input)
         return cast_to_adapter_tensor(output)
 
     def sigmoid_(self):
         output = self.sigmoid()
         return _tensor_inplace_assign(self, output, "sigmoid_", "sigmoid")
 
     def float(self, memory_format=None):
@@ -705,20 +713,40 @@
 
     def signbit(self):
         input = cast_to_ms_tensor(self)
         output = ms.ops.signbit(input)
         return cast_to_adapter_tensor(output)
 
     def svd(self, some=True, compute_uv=True):
+        if is_under_ascend_context():
+            input_np = self.numpy()
+            out = np.linalg.svd(input_np, not some, compute_uv)
+            if compute_uv:
+                u, s, v = out
+                u = ms.Tensor.from_numpy(u)
+                s = ms.Tensor.from_numpy(s)
+                v = np.swapaxes(v, -1, -2)
+                v = ms.Tensor.from_numpy(v)
+                output = (u, s, v)
+            else:
+                output = ms.Tensor.from_numpy(out)
+            return cast_to_adapter_tensor(output)
+
         input = cast_to_ms_tensor(self)
-        s, u, v = ms.ops.svd(input, not some, compute_uv)
-        output = (u, s, v)
+        output = ms.ops.svd(input, not some, compute_uv)
+        if compute_uv:
+            s, u, v = output
+            output = (u, s, v)
         return cast_to_adapter_tensor(output)
 
     def swapaxes(self, axis0, axis1):
+        if self.nelement() == 0:
+            out_shape = list(self.shape)
+            out_shape[axis0], out_shape[axis1] = out_shape[axis1], out_shape[axis0]
+            return self.reshape(tuple(out_shape))
         input = cast_to_ms_tensor(self)
         output = input.swapaxes(axis0, axis1)
         return cast_to_adapter_tensor(output)
 
     def swapdims(self, dim0, dim1):
         input = cast_to_ms_tensor(self)
         output = ms.ops.swapdims(input, dim0, dim1)
@@ -784,17 +812,20 @@
         output = ms.ops.mul(input, ms_value)
         return cast_to_adapter_tensor(output)
 
     def mul_(self, value):
         output = self.mul(value)
         return _tensor_inplace_assign(self, output, "mul_", "mul")
 
+    @property
     def device(self):
-        #TODO
-        pass
+        # Tensor.device and tensor.to(device) do not actually have effect in adapter
+        # because mindspore do not control a single tensor to a certain deivce
+        # So here for performance, return class Device with target and id.
+        return Device(get_backend(), 0)
 
     def div(self, value, *, rounding_mode=None) :
         input = cast_to_ms_tensor(self)
         value = cast_to_ms_tensor(value)
         output = ms.ops.div(input, value, rounding_mode=rounding_mode)
         return cast_to_adapter_tensor(output)
 
@@ -804,78 +835,81 @@
 
     def cpu(self):
         #TODO
         return self
 
     def min(self, dim=None, keepdim=False):
         input = cast_to_ms_tensor(self)
+        type = input.dtype
+        input = input.astype(ms.float32)
         if dim is None:
-            return cast_to_adapter_tensor(input.min())
+            output = input.min().astype(type)
+            return cast_to_adapter_tensor(output)
         #TODO
         # Until now, P.min do not support when `input` is type of `int32`, `int64``.
         if self.dtype == mstype.int64 or self.dtype == mstype.int32:
             if self.dtype == mstype.int64:
                 dtype_name = 'torch.int64'
             else:
                 dtype_name = 'torch.int32'
             raise TypeError("For 'Tensor.min', the type of `input` do not support `torch.int64` and "
                             "`torch.int32`, got {}.".format(dtype_name))
 
-        indices, result = P.min(input, axis=dim, keep_dims=keepdim)
+        result, indices = ms.ops.min(input, dim, keepdim)
+        result = result.astype(type)
+        if pynative_mode_condition():
+            point = set_name_tuple('min')
+            rlt = point(cast_to_adapter_tensor(result), cast_to_adapter_tensor(indices))
+            return rlt
         return cast_to_adapter_tensor(result), cast_to_adapter_tensor(indices)
 
     def max(self, dim=None, keepdim=False):
         input = cast_to_ms_tensor(self)
+        type = input.dtype
+        input = input.astype(ms.float32)
         if dim is None:
-            return cast_to_adapter_tensor(input.max())
+            output = input.max().astype(type)
+            return cast_to_adapter_tensor(output)
         # TODO: Until now, P.max do not support when `input` is type of `int32`, `int64``.
         if self.dtype == mstype.int64 or self.dtype == mstype.int32:
             if self.dtype == mstype.int64:
                 dtype_name = 'torch.int64'
             else:
                 dtype_name = 'torch.int32'
             raise TypeError("For 'Tensor.max', the type of `input` do not support `torch.int64` and "
                             "`torch.int32`, got {}.".format(dtype_name))
 
-        indices, result = P.max(input, axis=dim, keep_dims=keepdim)
+        result, indices = ms.ops.max(input, dim, keepdim)
+        result = result.astype(type)
+        if pynative_mode_condition():
+            point = set_name_tuple('max')
+            rlt = point(cast_to_adapter_tensor(result), cast_to_adapter_tensor(indices))
+            return rlt
         return cast_to_adapter_tensor(result), cast_to_adapter_tensor(indices)
 
     def numel(self):
         input = cast_to_ms_tensor(self)
         return P.size(input)
 
     def detach(self):
         input_ms = cast_to_ms_tensor(self)
         output = ms.ops.stop_gradient(input_ms)
         return cast_to_adapter_tensor(output)
 
     def sum(self, dim=None, keepdim=False, dtype=None):
         input = cast_to_ms_tensor(self)
         if dtype is not None:
-            input = input.astype(dtype) if dtype != mstype.bool_ else input.astype(mstype.int32)
-        elif self.dtype in msdapter_dtype.all_int_type:
+            input = input.astype(dtype) if dtype != mstype.bool_ else input.astype(mstype.bool_).astype(mstype.int64)
+        elif input.dtype in (msdapter_dtype.all_int_type, mstype.bool_):
             dtype = mstype.int64
             input = input.astype(dtype)
 
-        if not isinstance(keepdim, int):
-            raise TypeError("For 'Tensor.sum', the type of the argument 'keepdim' must be int, but "
-                            "got {}.".format(type(keepdim)))
-        if dim is None:
-            dim = ()
-        else:
-            dim = validator.check_and_canonicalize_axes(dim, input.ndim)
-
-        if not validator.check_type_support(input.dtype, 'GPU', (mstype.float64, mstype.float32, mstype.float16)):
-            input = input.astype(mstype.float32)
-        if 0 in self.shape:
-            input = tensor_operator_registry.get('make_tensor')([0], input.dtype)
-        res = tensor_operator_registry.get('sum')(bool(keepdim))(input, dim)
-        if dtype == mstype.bool_:
+        res = input.sum(dim, dtype, keepdim)
+        if dtype is not None and dtype == mstype.bool_:
             res = res.astype(mstype.bool_)
-
         return cast_to_adapter_tensor(res)
 
     def sum_to_size(self, *size):
         input = cast_to_ms_tensor(self)
         output = input.sum_to_size(*size)
         return cast_to_adapter_tensor(output)
 
@@ -924,20 +958,19 @@
         if isinstance(shape, list):
             shape = tuple(shape)
 
         input_size = self.shape
         if input_size[0] == 0:  # only support first element is 0
             numel = ms.ops.size(self)
             shape = _infer_size(shape, numel)
-            #TODO: if switch the mindspore version, change the code to
-            #output = _get_cache_prim(ms.ops.Zeros)()(shape, self.dtype)
-            output = ms.ops.zeros(shape, self.dtype)
+            #TODO: ms.ops.zeros() currently has preblem handling input shape including 0
+            output = _get_cache_prim(ms.ops.Zeros)()(shape, self.dtype)
         else:
             input = cast_to_ms_tensor(self)
-            output = tensor_operator_registry.get('reshape')()(input, shape)
+            output = ms.ops.reshape(input, shape)
         return cast_to_adapter_tensor(output)
 
     def view_as(self, other):
         return self.view(other.shape)
 
     def ndimension(self):
         input_ms = cast_to_ms_tensor(self)
@@ -1007,17 +1040,16 @@
 
     def reshape(self, *shape):
         input_ms = cast_to_ms_tensor(self)
         input_size = input_ms.shape
         if input_size[0] == 0:  # only support first element is 0
             numel = ms.ops.size(input_ms)
             shape = _infer_size(shape, numel)
-            #TODO: if switch the mindspore version, change the code to
-            #output = _get_cache_prim(ms.ops.Zeros)()(shape, input_ms.dtype)
-            output = ms.ops.zeros(shape, input_ms.dtype)
+            #TODO: ms.ops.zeros() currently has preblem handling input shape including 0
+            output = _get_cache_prim(ms.ops.Zeros)()(shape, input_ms.dtype)
         else:
             output = input_ms.reshape(*shape)
         return cast_to_adapter_tensor(output)
 
     def reshape_as(self, other):
         return self.reshape(other.shape)
 
@@ -1063,22 +1095,22 @@
     @property
     def ndim(self):
         return len(self.shape)
 
     def amax(self, dim=None, keepdim=False):
         input_ms = cast_to_ms_tensor(self)
         if dim is not None:
-            return cast_to_adapter_tensor(input_ms.amax(axis=dim, keep_dims=keepdim))
-        return cast_to_adapter_tensor(input_ms.amax(keep_dims=keepdim))
+            return cast_to_adapter_tensor(input_ms.amax(axis=dim, keepdims=keepdim))
+        return cast_to_adapter_tensor(input_ms.amax(keepdims=keepdim))
 
     def amin(self, dim=None, keepdim=False):
         input_ms = cast_to_ms_tensor(self)
         if dim is not None:
-            return cast_to_adapter_tensor(input_ms.amin(axis=dim, keep_dims=keepdim))
-        return cast_to_adapter_tensor(input_ms.amin(keep_dims=keepdim))
+            return cast_to_adapter_tensor(input_ms.amin(axis=dim, keepdims=keepdim))
+        return cast_to_adapter_tensor(input_ms.amin(keepdims=keepdim))
 
     def as_strided(self, size, stride, storage_offset=None):
         warnings.warn("not support output as a view.")
         input_ms = cast_to_ms_tensor(self)
         if len(size) != len(stride):
             raise RuntimeError("mismatch in length of strides and shape.")
         index = np.arange(0, size[0]*stride[0], stride[0])
@@ -1094,35 +1126,33 @@
 
     def bmm(self, batch2):
         input_ms = cast_to_ms_tensor(self)
         return cast_to_adapter_tensor(input_ms.bmm(batch2))
 
     def clamp(self, min=None, max=None):
         input_ms = cast_to_ms_tensor(self)
-        type = input_ms.dtype
-        if min is not None and max is not None and min > max:
-            output = ms.ops.ones_like(input_ms).astype(type)*max
-        else:
-            if min is not None:
-                min = ms.Tensor(min, type)
-            if max is not None:
-                max = ms.Tensor(max, type)
-            output = ms.ops.clip_by_value(input_ms, min, max)
+        if is_under_ascend_context() and input_ms.dtype == ms.float64:
+            input_ms = input_ms.astype(ms.float32)
+            output = ms.ops.clamp(input_ms, min, max)
+            output = output.astype(ms.float64)
+        else:
+            output = ms.ops.clamp(input_ms, min, max)
         return cast_to_adapter_tensor(output)
 
     def clamp_(self, min=None, max=None):
         output = self.clamp(min, max)
         return _tensor_inplace_assign(self, output, "clamp_", "clamp")
 
     def dim(self):
         return len(self.shape)
 
     def expand_as(self, other):
         input_ms = cast_to_ms_tensor(self)
-        output = input_ms.expand_as(other)
+        other_ms = cast_to_ms_tensor(other)
+        output = input_ms.expand_as(other_ms)
         return cast_to_adapter_tensor(output)
 
     def item(self):
         input_ms = cast_to_ms_tensor(self)
         if input_ms.size > 1:
             raise ValueError("only one element tensors can be converted to Python scalars")
         output = input_ms.reshape(-1).asnumpy().tolist()
@@ -1142,14 +1172,28 @@
         output = ms.ops.log2(input)
         return cast_to_adapter_tensor(output)
 
     def log2_(self):
         output = self.log2()
         return _tensor_inplace_assign(self, output, "log2_", "log2")
 
+    # TODO: currently not support return qr as second result
+    def lstsq(self, A, op_name='tensor.lstsq'):
+        input_ms = cast_to_ms_tensor(self)
+        A = cast_to_ms_tensor(A)
+        if is_under_cpu_context():
+            unsupported_attr(op_name)
+            output = ms.ops.lstsq(A, input_ms)
+            qr = ms.ops.zeros(A.shape, A.dtype)
+        else:
+            #TODO: ms.ops.lstsq not support GPU and Ascend, use numpy func
+            lstsq_op = NumpyLstsq(op_name)
+            output, qr = lstsq_op(input_ms, A)
+        return cast_to_adapter_tensor((output, qr))
+
     def matmul(self, tensor2):
         input_ms = cast_to_ms_tensor(self)
         tensor2_ms = cast_to_ms_tensor(tensor2)
         output = ms.ops.matmul(input_ms, tensor2_ms)
         return cast_to_adapter_tensor(output)
 
     def squeeze(self, dim=None):
@@ -1271,25 +1315,24 @@
             raise ValueError("The inputs of Tensor.to is abnormal, please check.")
 
         if len(args) > 1 and args[1] in _dtypeDict.values():
             return cast_to_adapter_tensor(input_ms.astype(args[1]))
         return self
 
     def sort(self, dim=-1, descending=False):
-        # TODO: ops.sort() should be replaced.
         input_ms = cast_to_ms_tensor(self)
         input_type = input_ms.dtype
         if 'Int' in str(input_type):
             input_ms = input_ms.astype(ms.float32)
-            sort_tensor, sort_index = ms.ops.Sort(dim, descending)(input_ms)
+            sort_tensor, sort_index = ms.ops.sort(input_ms, dim, descending)
             sort_tensor = sort_tensor.astype(input_type)
             sort_index = sort_index.astype(ms.int64)
             return cast_to_adapter_tensor((sort_tensor, sort_index))
         else:
-            output = _get_cache_prim(ms.ops.Sort)(dim, descending)(input_ms)
+            output = ms.ops.sort(input_ms, dim, descending)
         return cast_to_adapter_tensor(output)
 
     def msort(self):
         input_ms = cast_to_ms_tensor(self)
         input_type = input_ms.dtype
         if input_type in msdapter_dtype.all_int_type:
             input_ms = input_ms.astype(ms.float32)
@@ -1523,41 +1566,43 @@
         output = self.masked_fill(mask, value)
         return _tensor_inplace_assign(self, output, "masked_fill_", "masked_fill")
 
     def tolist(self):
         return self.numpy().tolist()
 
     def bernoulli(self, *, generator=None):
-        unsupported_attr(generator)
-        if generator:
-            raise NotImplementedError("generator is not supported.")
-        input_ms = cast_to_ms_tensor(self)
-
-        bernoulli_seed = ms.get_seed()
-        if not bernoulli_seed:
-            bernoulli_seed = -1
-        return cast_to_adapter_tensor(input_ms.bernoulli(input_ms, bernoulli_seed))
+        return self._bernoulli_adapter(self, generator=generator)
 
     def bernoulli_(self, p=0.5, *, generator=None):
-        output = self.bernoulli_adapter(p, generator=generator)
-        return _tensor_inplace_assign(self, output, "bernoulli_", "bernoulli_adapter")
+        output = self._bernoulli_adapter(p, generator=generator)
+        return _tensor_inplace_assign(self, output, "bernoulli_", "_bernoulli_adapter")
 
-    def bernoulli_adapter(self, p=0.5, *, generator=None):
-        unsupported_attr(generator)
+    def _bernoulli_adapter(self, p=0.5, *, generator=None):
         if generator:
             raise NotImplementedError("generator is not supported.")
         input_ms = cast_to_ms_tensor(self)
 
         bernoulli_seed = ms.get_seed()
         if not bernoulli_seed:
             bernoulli_seed = -1
         if not isinstance(p, (Tensor, float)):
             p = float(p)
-
-        return cast_to_adapter_tensor(input_ms.bernoulli(p, bernoulli_seed))
+        #TODO: Ascend currently not support ops.bernoulli, use numpy.random.binomial
+        if is_under_ascend_context():
+            if isinstance(p, ms.Tensor):
+                p = p.numpy()
+            # on Ascend, use numpy binomial to do forward computation
+            # here it doesn't need to consider the backward
+            # because torch.bernoulli return zero grad, and mindspore return zero grad here as well.
+            np_output = np.random.binomial(1, p, size=input_ms.shape)
+            output = ms.Tensor.from_numpy(np_output).to(dtype=input_ms.dtype)
+            return cast_to_adapter_tensor(output)
+        else:
+            p = cast_to_ms_tensor(p)
+            return cast_to_adapter_tensor(input_ms.bernoulli(p, bernoulli_seed))
 
     def round(self, decimals=0):
         input = cast_to_ms_tensor(self)
         if decimals == 0:
             output = ms.ops.round(input)
         else:
             p = 10 ** decimals
@@ -1897,26 +1942,36 @@
         x = cast_to_ms_tensor(self)
         y = cast_to_ms_tensor(other)
         #TODO: NAN is different
         output = ms.ops.minimum(x, y)
         return cast_to_adapter_tensor(output)
 
     def fmax(self, other):
+        if is_under_ascend_context() or is_under_gpu_context():
+            x_np = self.numpy()
+            y_np = other.numpy()
+            output = ms.Tensor.from_numpy(np.fmax(x_np, y_np))
+            return cast_to_adapter_tensor(output)
+
         x = cast_to_ms_tensor(self)
         y = cast_to_ms_tensor(other)
-        # TODO: ms.ops.fmax only support CPU and Ascend now
+        # TODO: ms.ops.fmax only support CPU now
         output = ms.ops.function.math_func.fmax(x, y)
         return cast_to_adapter_tensor(output)
 
     def fmin(self, other):
-        x = cast_to_ms_tensor(self)
-        y = cast_to_ms_tensor(other)
-        # TODO: ms.ops.fmin only support CPU and Ascend now
-        output = ms.ops.function.math_func.fmin(x, y)
-        return cast_to_adapter_tensor(output)
+        x_np = self.numpy()
+        y_np = other.numpy()
+        output = ms.Tensor.from_numpy(np.fmin(x_np, y_np))
+        return cast_to_adapter_tensor(output)
+        # TODO: ms.ops.fmin not support now
+        # x = cast_to_ms_tensor(self)
+        # y = cast_to_ms_tensor(other)
+        # output = ms.ops.function.math_func.fmin(x, y)
+        # return cast_to_adapter_tensor(output)
 
     def multiply(self, value):
         x = cast_to_ms_tensor(self)
         y = cast_to_ms_tensor(value)
         output = ms.ops.mul(x, y)
         return cast_to_adapter_tensor(output)
 
@@ -2647,19 +2702,18 @@
         start = _get_tensor_data(start)
         length = _get_tensor_data(length)
         output = ms.ops.narrow(input, dimension, start, length)
         return cast_to_adapter_tensor(output)
 
     def norm(self, p='fro', dim=None, keepdim=False, dtype=None):
         input = cast_to_ms_tensor(self)
-        #TODO :ms.ops.norm is not ready, ms.numpy.norm function is also not complete.
         if dtype is None:
             dtype = ms.float32
         input = input.astype(dtype)
-        output = ms.numpy.norm(input, ord=p, axis=dim, keepdims=keepdim)
+        output = ms.ops.norm(input, ord=p, dim=dim, keepdim=keepdim)
         output = output.astype(dtype)
         return cast_to_adapter_tensor(output)
 
     def xlogy(self, other):
         input = cast_to_ms_tensor(self)
         other = cast_to_ms_tensor(other)
         # TODO: To support more datatype on Ascend
@@ -2687,18 +2741,17 @@
         other = cast_to_ms_tensor(other)
         if input.is_complex():
             input = ms.ops.conj(input)
         output = ms.ops.inner(input, other)
         return cast_to_adapter_tensor(output)
 
     def where(self, condition, y):
-        #TODO: replace with ms.ops.where
         x = cast_to_ms_tensor(self)
         y = cast_to_ms_tensor(y)
-        output = ms.numpy.where(condition, x, y)
+        output = ms.ops.where(condition, x, y)
         return cast_to_adapter_tensor(output)
 
     def true_divide(self, divisor):
         input = cast_to_ms_tensor(self)
         other = cast_to_ms_tensor(divisor)
         if not input.is_floating_point():
             if isinstance(other, ms.Tensor):
@@ -2723,16 +2776,15 @@
 
     def triu_(self, diagonal=0):
         output = self.triu(diagonal)
         return _tensor_inplace_assign(self, output, "triu_", "triu")
 
     def tril(self, diagonal=0):
         input = cast_to_ms_tensor(self)
-        # TODO: To use ms.ops.tril after it supported on Ascend
-        output = ms.numpy.tril(input, diagonal)
+        output = ms.ops.tril(input, diagonal)
         return cast_to_adapter_tensor(output)
 
     def tril_(self, diagonal=0):
         output = self.tril(diagonal)
         return _tensor_inplace_assign(self, output, "tril_", "tril")
 
     def nanmean(self, dim=None, keepdim=False, *, dtype=None):
@@ -2910,16 +2962,16 @@
 
     def logical_xor(self, other):
         if isinstance(self, Tensor):
             input = cast_to_ms_tensor(self).astype(ms.bool_)
         if isinstance(other, Tensor):
             other = cast_to_ms_tensor(other).astype(ms.bool_)
 
-        # TODO: ms.ops.logical_xor to supported GPU and Ascend
-        if is_under_ascend_context() or is_under_gpu_context():
+        # TODO: ms.ops.logical_xor to supported GPU
+        if is_under_gpu_context():
             output = ms.numpy.logical_xor(input, other)
         else:
             output = ms.ops.logical_xor(input, other)
         return cast_to_adapter_tensor(output)
 
     def logical_xor_(self, other):
         # TODO: ms.ops.logical_xor to supported GPU and Ascend
@@ -2941,14 +2993,48 @@
         output = ms.ops.lerp(input_ms, end_ms, weight)
         return cast_to_adapter_tensor(output)
 
     def lerp_(self, end, weight):
         output = self.lerp(end, weight)
         return _tensor_inplace_assign(self, output, "lerp_", "lerp")
 
+    def lu(self, *, pivot=True, get_infos=False):
+        if get_infos:
+            output1, info = _lu_factor_ex(self, pivot=pivot)
+            output = output1 + (info,)
+        else:
+            output = _lu_factor(self, pivot=pivot)
+        return cast_to_adapter_tensor(output)
+
+
+    def lu_solve(self, LU, pivots, *, left=True, adjoint=False):
+        #TODO: Currently not supported on Ascend
+        ascend_raise_implement_error("lu_solve")
+        #TODO: Mindspore does not support left
+        if not left:
+            raise NotImplementedError("lu_factor currently not supported =False")
+        B = cast_to_ms_tensor(self)
+        LU = cast_to_ms_tensor(LU)
+        pivots = cast_to_ms_tensor(pivots).astype(ms.int32)
+        pivots = pivots - 1
+        A = (LU, pivots)
+        trans=2 if adjoint else 0
+        if LU.ndim == 2:
+            output = ms_linalg.lu_solve(A, B, trans=trans)
+        else:
+            if pynative_mode_condition():
+                output = vmap(ms_linalg.lu_solve, in_axes= (0, 0, None))(A, B, trans)
+            else:
+                #TODO:vmap function has bug on graph mode now
+                output = []
+                for i in range(B.shape[0]):
+                    output.append(ms_linalg.lu_solve((LU[i], pivots[i]), B[i], trans=trans))
+                output = ms.ops.stack(output)
+        return cast_to_adapter_tensor(output)
+
     def masked_select(self, mask):
         input_ms = cast_to_ms_tensor(self)
         mask_ms = cast_to_ms_tensor(mask)
         output = ms.ops.masked_select(input_ms, mask_ms)
         return cast_to_adapter_tensor(output)
 
     def angle(self):
@@ -3163,25 +3249,28 @@
 
     def rot90(self, k, dims):
         input_ms = cast_to_ms_tensor(self)
         output = ms.ops.rot90(input_ms, k, dims)
         return cast_to_adapter_tensor(output)
 
     def median(self, dim=None, keepdim=False):
-        def _process_out(value, indice):
-            point = collections.namedtuple('median', 'values,indices')
-            rlt = point(cast_to_adapter_tensor(value), cast_to_adapter_tensor(indice))
-            return rlt
         input = cast_to_ms_tensor(self)
         if dim is None:
-            output, _ = ms.ops.median(input, keepdims=keepdim)
+            # ms.ops.median can not compute the median value along all dimentions
+            # only ms.ops.Median(global_median=True) can do that.
+            # so can not replace ms.ops.Median to ms.ops.median
+            output, _ = _get_cache_prim(ms.ops.Median)(True)(input)
             return cast_to_adapter_tensor(output)
         else:
-            value, indices = ms.ops.median(input, axis=dim, keepdims=keepdim)
-            return _process_out(value, indices)
+            value, indices = ms.ops.median(input, dim, keepdim)
+            if pynative_mode_condition():
+                point = set_name_tuple('median')
+                rlt = point(cast_to_adapter_tensor(value), cast_to_adapter_tensor(indices))
+                return rlt
+            return cast_to_adapter_tensor(value), cast_to_adapter_tensor(indices)
 
     def frac(self):
         input_ms = cast_to_ms_tensor(self)
         output = ms.ops.frac(input_ms)
         return cast_to_adapter_tensor(output)
 
     def frac_(self):
@@ -3307,14 +3396,23 @@
 
     def orgqr(self, input2):
         input = cast_to_ms_tensor(self)
         input2 = cast_to_ms_tensor(input2)
         output = ms.ops.orgqr(input, input2)
         return cast_to_adapter_tensor(output)
 
+    def qr(self, some=True):
+        input_ms = cast_to_ms_tensor(self)
+        if some:
+            mode = "reduced"
+        else:
+            mode = "complete"
+        output = ms.ops.qr(input_ms, mode)
+        return cast_to_adapter_tensor(output)
+
 class _TypeTensor(Tensor):
     def __init__(self, *input_data, dtype_name):
         super(_TypeTensor, self).__init__(*input_data, dtype=dtype_name, inner=False)
 
 
 class ByteTensor(_TypeTensor):
     def __init__(self, *input_data):
@@ -3366,37 +3464,47 @@
 def cast_to_ms_tensor(inputs):
     """
     Cast MSAdapter.Tensor to MindSpore.Tensor before call mindspore API.
     """
     def _cast(inputs):
         if isinstance(inputs, Tensor):
             inputs = inner.convert_to_ms_tensor(inputs)
-        elif isinstance(inputs, (tuple, list)):
-            inputs = list(inputs)
+        elif isinstance(inputs, tuple):
+            inputs_list = list(inputs)
+            for id, value in enumerate(inputs):
+                inputs_list[id] = _cast(value)
+            inputs = tuple(inputs_list)
+        elif isinstance(inputs, list):
+            inputs_list = inputs
             for id, value in enumerate(inputs):
-                inputs[id] = _cast(value)
-            inputs = tuple(inputs)
+                inputs_list[id] = _cast(value)
+            inputs = inputs_list
         return inputs
 
     inputs = _cast(inputs)
     return inputs
 
 
 def cast_to_adapter_tensor(outputs):
     """
     Cast MindSpore.Tensor to MSAdapter.Tensor after call mindspore API.
     """
     def _cast(outputs):
         if isinstance(outputs, (ms.Tensor, Tensor_)):
             outputs = inner.convert_to_adapter_tensor(outputs)
-        elif isinstance(outputs, (tuple, list)):
+        elif isinstance(outputs, tuple):
             outputs_list = list(outputs)
             for id, value in enumerate(outputs):
                 outputs_list[id] = _cast(value)
             outputs = tuple(outputs_list)
+        elif isinstance(outputs, list):
+            outputs_list = outputs
+            for id, value in enumerate(outputs):
+                outputs_list[id] = _cast(value)
+            outputs = outputs_list
         return outputs
 
     outputs = _cast(outputs)
     return outputs
 
 
 def _tensor_inplace_assign(input, output, op_name, replace_op):
@@ -3427,7 +3535,42 @@
         other_ms = other_ms.astype(ms.float64)
     else:
         input_ms = input_ms.astype(ms.float32)
         other_ms = other_ms.astype(ms.float32)
         if input_type == ms.float32 or other_type == ms.float32:
             float_flag = False
     return input_ms, other_ms, float_flag
+
+def _lu_factor(A, *, pivot=True):
+    #TODO: Currently not supported on Ascend
+    ascend_raise_implement_error("lu_factor_ex")
+    #TODO: Mindspore does not support pivot=False condition
+    if not pivot:
+        raise NotImplementedError("lu_factor currently not supported pivot=False")
+    A = cast_to_ms_tensor(A)
+    if A.ndim == 2:
+        lu, pivots = ms_linalg.lu_factor(A, overwrite_a=False, check_finite=True)
+    else:
+        lu, pivots = vmap(ms_linalg.lu_factor, in_axes= (0, None, None))(A, False, True)
+    pivots = pivots + 1
+    output = (lu, pivots)
+    return output
+
+def _lu_factor_ex(A, *, pivot=True):
+    #TODO: Currently not supported on Ascend
+    ascend_raise_implement_error("lu_factor_ex")
+    #TODO: Mindspore does not support pivot=False condition
+    if not pivot:
+        raise NotImplementedError("lu_factor currently not supported pivot=False")
+    A = cast_to_ms_tensor(A)
+    if A.ndim == 2:
+        lu, pivots = ms_linalg.lu_factor(A, overwrite_a=False, check_finite=True)
+        #TODO: Mindspore not support check_errors
+        info = 0
+    else:
+        lu, pivots = vmap(ms_linalg.lu_factor, in_axes= (0, None, None))(A, False, True)
+        #TODO: Mindspore not support check_errors
+        #TODO: ms.ops.zeros() currently has preblem handling input shape including 0
+        info = _get_cache_prim(ms.ops.Zeros)()(A.shape[0], ms.int32)
+    pivots = pivots + 1
+    output = (lu, pivots)
+    return output, info
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/communication/eventloop.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/communication/eventloop.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/communication/iter.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/communication/iter.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/communication/map.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/communication/map.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/communication/messages.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/communication/messages.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/communication/protocol.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/communication/protocol.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/communication/queue.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/communication/queue.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/dataloader.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/dataloader_experimental.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/dataloader_experimental.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/dataframe/dataframes.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/dataframe/dataframes.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/dataframe/dataframe_wrapper.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/dataframe/dataframe_wrapper.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/dataframe/datapipes.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/dataframe/datapipes.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/dataframe/structures.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/dataframe/structures.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/datapipe.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/datapipe.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/gen_pyi.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/gen_pyi.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/callable.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/callable.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/combinatorics.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/combinatorics.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/combining.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/combining.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/filelister.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/filelister.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/fileopener.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/fileopener.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/grouping.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/grouping.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/routeddecoder.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/routeddecoder.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/selecting.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/selecting.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/streamreader.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/streamreader.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/utils.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/utils.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/iter/__init__.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/iter/__init__.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/map/callable.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/map/callable.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/map/combinatorics.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/map/combinatorics.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/map/combining.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/map/combining.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/map/grouping.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/map/grouping.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/map/utils.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/map/utils.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/map/__init__.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/map/__init__.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/utils/common.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/utils/common.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/utils/decoder.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/utils/decoder.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/_decorator.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/_decorator.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/datapipes/_typing.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/datapipes/_typing.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/dataset.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/distributed.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/distributed.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/graph.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/graph.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/graph_settings.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/graph_settings.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/sampler.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/sampler.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/_utils/collate.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/_utils/collate.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/_utils/fetch.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/_utils/fetch.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/_utils/pin_memory.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/_utils/pin_memory.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/_utils/queue.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/_utils/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,20 +109,20 @@
                     raise e
                 if exit_signal.is_set():
                     return
                 continue
 
     def put(self, data, timeout=None, list_buffer = None):
 
-        def shareput(data, bufferlist):
+        def shareput(data):
+            bufferlist = []
             for r in data:
                 if isinstance(r, (tuple, list)):
-                    buf = []
+                    buf = shareput(r)
                     bufferlist.append(buf)
-                    shareput(r, bufferlist=buf)
                 else:
                     # the map:pyfunc is a yield generator which can't be serialize
                     if isinstance(r, types.GeneratorType):
                         raise TypeError("Cannot pickle {} object, please verify pyfunc return with numpy array"
                                         .format(type(r)))
                     if (isinstance(r, np.ndarray) and r.size > self.min_shared_mem
                             and self.put_start_bytes + r.nbytes < self.seg_size):
@@ -148,24 +148,25 @@
                                     + "MB."
                                 )
                                 self.print_error = False
                                 self.count.value += 1
                         if isinstance(r, torch.Tensor):
                             r.asnumpy()
                         bufferlist.append((self.data_immediate, r))
-
+            if isinstance(data, tuple):
+                return tuple(bufferlist)
+            return bufferlist
         if isinstance(data, ExceptionHandler):  # pylint: disable=too-many-nested-blocks
             super().put(data, timeout=timeout)
         else:
-            name_list = []
             self.seg_pos.value = (self.seg_pos.value + 1) % self.num_seg
             seg_pos = self.seg_pos.value
             self.put_start_bytes = 0
             # TODO  (idx, data) data (data,) 、(data, label)、 ((data, data), label) 、((data, data), (label, label)), ({}, label)
-            shareput(data, bufferlist=name_list)
+            name_list = shareput(data)
             super().put(name_list, timeout=timeout)
             # note above could generate a queue full exception.  It will be handled by teh caller
             # only increment seg_pos after successfully adding to metadata queue
 
     def get_until(self, timeout=None, exit_signal=None):
         """Get data from the queue. Block until timeout is reached or exit_signal is set."""
         while True:
@@ -185,17 +186,17 @@
                 continue
             return r
 
     def get(self, timeout=None):
         result = super().get(timeout=timeout)
         if isinstance(result, ExceptionHandler):
             return result
-        r = []
         self.get_start_bytes = 0
-        def shareget(result, res):
+        def shareget(result):
+            res = []
             for x in result:
                 if x[0] == self.data_shared:
                     seg_pos = x[1]
                     byte = x[2]
                     dtype = x[3]
                     shape = x[4]
                     start_offset = self.get_start_bytes
@@ -206,22 +207,22 @@
                         data2 = np.copy(data)
                         res.append(data2)
                     else:
                         res.append(data)
                 elif x[0] == self.data_immediate:
                     res.append(x[1])
                 elif isinstance(x[0], (list, tuple)):
-                    cur = []
+                    cur = shareget(x)
                     res.append(cur)
-                    shareget(x, cur)
                 else:
                     raise RuntimeError("SharedQueue, invalid entry in metadata.")
-
-        shareget(result, r)
-        return tuple(r)
+            if isinstance(result, tuple):
+                return tuple(res)
+            return res
+        return shareget(result)
 
     def __del__(self):
         shm_list_len = len(self.shm_list)
         for idx in range(shm_list_len):
             del self.shm_list[shm_list_len - idx - 1]
         del self.shm_list
```

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/_utils/signal_handling.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/_utils/signal_handling.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/_utils/worker.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/_utils/worker.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/_utils/__init__.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/utils/data/__init__.py` & `msadapter-0.1.0rc0/msadapter/pytorch/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/_ref/__init__.py` & `msadapter-0.1.0rc0/msadapter/pytorch/_ref/__init__.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/_register/getitem_impl.py` & `msadapter-0.1.0rc0/msadapter/pytorch/_register/getitem_impl.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/_register/register_multitype_ops.py` & `msadapter-0.1.0rc0/msadapter/pytorch/_register/register_multitype_ops.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/_register/register_standard_method.py` & `msadapter-0.1.0rc0/msadapter/pytorch/_register/register_standard_method.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/_register/register_utils.py` & `msadapter-0.1.0rc0/msadapter/pytorch/_register/register_utils.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/_register/__init__.py` & `msadapter-0.1.0rc0/msadapter/pytorch/_register/__init__.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/_utils.py` & `msadapter-0.1.0rc0/msadapter/pytorch/_utils.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/pytorch/__init__.py` & `msadapter-0.1.0rc0/msadapter/pytorch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import msadapter.pytorch.fft as fft
 from msadapter.pytorch import autograd
 from msadapter.pytorch.package_info import __version__, VERSION, version
 from msadapter.pytorch.random import *
 from msadapter.pytorch.storage import *
 from msadapter.pytorch.serialization import *
 import msadapter.pytorch.linalg as linalg
-from msadapter.pytorch.linalg import *
+from msadapter.pytorch.linalg import lu_solve
 
 def _assert(condition, message):
     assert condition, message
 
 def is_tensor(obj):
     r"""Returns True if `obj` is a msadapter.pytorch tensor.
```

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/caltech.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/caltech.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/celeba.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/celeba.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/cifar.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/cityscapes.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/clevr.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/clevr.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/coco.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/country211.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/country211.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/dtd.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/dtd.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/eurosat.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/eurosat.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/fakedata.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/fakedata.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/fer2013.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/fer2013.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/fgvc_aircraft.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/fgvc_aircraft.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/flickr.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/flickr.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/flowers102.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/flowers102.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/folder.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/folder.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/food101.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/food101.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/gtsrb.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/gtsrb.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/hmdb51.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/hmdb51.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/imagenet.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/imagenet.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/inaturalist.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/inaturalist.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/kinetics.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/kinetics.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/kitti.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/kitti.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/lfw.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/lfw.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/lsun.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/lsun.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/mnist.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/omniglot.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/omniglot.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/oxford_iiit_pet.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/oxford_iiit_pet.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/pcam.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/pcam.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/phototour.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/phototour.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/places365.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/places365.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/rendered_sst2.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/rendered_sst2.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/samplers/clip_sampler.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/samplers/clip_sampler.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/sbd.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/sbd.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/sbu.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/sbu.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/semeion.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/semeion.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/stanford_cars.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/stanford_cars.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/stl10.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/stl10.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/sun397.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/sun397.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/svhn.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/svhn.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/ucf101.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/ucf101.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/usps.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/usps.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/utils.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/video_utils.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/video_utils.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/vision.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/vision.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/voc.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/widerface.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/widerface.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/_optical_flow.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/_optical_flow.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/datasets/__init__.py` & `msadapter-0.1.0rc0/msadapter/torchvision/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/extension.py` & `msadapter-0.1.0rc0/msadapter/torchvision/extension.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/io/image.py` & `msadapter-0.1.0rc0/msadapter/torchvision/io/image.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/io/video.py` & `msadapter-0.1.0rc0/msadapter/torchvision/io/video.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/io/video_reader.py` & `msadapter-0.1.0rc0/msadapter/torchvision/io/video_reader.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/io/_video_opt.py` & `msadapter-0.1.0rc0/msadapter/torchvision/io/_video_opt.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/io/__init__.py` & `msadapter-0.1.0rc0/msadapter/torchvision/io/__init__.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/alexnet.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/alexnet.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/densenet.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/densenet.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/detection/anchor_utils.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/detection/anchor_utils.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/detection/backbone_utils.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/detection/backbone_utils.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/detection/faster_rcnn.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/detection/faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/detection/generalized_rcnn.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/detection/generalized_rcnn.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/detection/image_list.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/detection/image_list.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/detection/keypoint_rcnn.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/detection/keypoint_rcnn.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/detection/mask_rcnn.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/detection/mask_rcnn.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/detection/retinanet.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/detection/retinanet.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/detection/roi_heads.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/detection/roi_heads.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/detection/rpn.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/detection/rpn.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/detection/ssd.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/detection/ssd.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/detection/ssdlite.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/detection/ssdlite.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/detection/transform.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/detection/transform.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/detection/_utils.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/detection/_utils.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/googlenet.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/googlenet.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/inception.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/inception.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/mnasnet.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/mnasnet.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/mobilenetv2.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/mobilenetv3.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/quantization/resnet.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/quantization/resnet.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/quantization/shufflenetv2.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/quantization/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/resnet.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/resnet.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/segmentation/deeplabv3.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/segmentation/deeplabv3.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/segmentation/fcn.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/segmentation/fcn.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/segmentation/lraspp.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/segmentation/lraspp.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/segmentation/segmentation.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/segmentation/_utils.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/segmentation/_utils.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/shufflenetv2.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/squeezenet.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/squeezenet.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/utils.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/utils.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/vgg.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/vgg.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/video/resnet.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/video/resnet.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/models/_utils.py` & `msadapter-0.1.0rc0/msadapter/torchvision/models/_utils.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/boxes.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/boxes.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/ciou_loss.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/ciou_loss.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/deform_conv.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/diou_loss.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/diou_loss.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/drop_block.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/drop_block.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/feature_pyramid_network.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/feature_pyramid_network.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/focal_loss.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/focal_loss.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/giou_loss.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/giou_loss.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/misc.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/misc.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/poolers.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/poolers.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/ps_roi_align.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/ps_roi_align.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/ps_roi_pool.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/ps_roi_pool.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/roi_align.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/roi_align.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/roi_pool.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/roi_pool.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/stochastic_depth.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/stochastic_depth.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/_box_convert.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/_box_convert.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/_utils.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/_utils.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/ops/__init__.py` & `msadapter-0.1.0rc0/msadapter/torchvision/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/transforms/autoaugment.py` & `msadapter-0.1.0rc0/msadapter/torchvision/transforms/autoaugment.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import math
 from enum import Enum
 from typing import List, Tuple, Optional, Dict
 
 import msadapter.pytorch as torch
 from msadapter.pytorch import Tensor
-from mindspore.ops import constexpr
+from mindspore.ops.primitive import _primexpr
 from msadapter.pytorch.tensor import cast_to_adapter_tensor
 from .functional import _is_numpy, msvision_mode_mapping
 import mindspore.dataset.vision as msvision
 from collections.abc import Sequence
 
 from . import functional as F, InterpolationMode
 
@@ -554,20 +554,20 @@
                     "Contrast": (torch.linspace(0.0, 0.9, num_bins), True),
                     "Sharpness": (torch.linspace(0.0, 0.9, num_bins), True),
                 }
             )
         return s
 
     # @torch.jit.unused
-    # @constexpr
+    # @_primexpr
     def _pil_to_tensor(self, img) -> Tensor:
         return F.pil_to_tensor(img)
 
     # @torch.jit.unused
-    # @constexpr
+    # @_primexpr
     def _tensor_to_pil(self, img: Tensor):
         return F.to_pil_image(img)
 
     def _sample_dirichlet(self, params: Tensor) -> Tensor:
         # Must be on a separate method so that we can overwrite it in tests.
         return torch._sample_dirichlet(params)
```

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/transforms/functional.py` & `msadapter-0.1.0rc0/msadapter/torchvision/transforms/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from enum import Enum
 from typing import List, Tuple, Any, Optional
 
 import numpy as np
 import msadapter.pytorch as torch
 from PIL import Image
 from msadapter.pytorch import Tensor
-from mindspore.ops import constexpr
+from mindspore.ops.primitive import _primexpr
 from mindspore.dataset.vision import Inter
 
 try:
     import accimage
 except ImportError:
     accimage = None
 
@@ -138,20 +138,20 @@
     #     _log_api_usage_once(get_image_num_channels)
     if isinstance(img, torch.Tensor):
         return F_t.get_image_num_channels(img)
 
     return F_pil.get_image_num_channels(img)
 
 
-# @constexpr
+# @_primexpr
 def _is_numpy(img: Any) -> bool:
     return isinstance(img, np.ndarray)
 
 
-# @constexpr
+# @_primexpr
 def _is_numpy_image(img: Any) -> bool:
     return img.ndim in {2, 3}
 
 
 def to_tensor(pic) -> Tensor:
     """Convert a ``PIL Image`` or ``numpy.ndarray`` to tensor.
     This function does not support torchscript.
@@ -1282,15 +1282,15 @@
         center_f = [1.0 * (c - s * 0.5) for c, s in zip(center, [width, height])]
 
     translate_f = [1.0 * t for t in translate]
     matrix = _get_inverse_affine_matrix(center_f, angle, translate_f, scale, shear)
     return F_t.affine(img, matrix=matrix, interpolation=interpolation.value, fill=fill)
 
 
-# @constexpr
+# @_primexpr
 def to_grayscale(img, num_output_channels=1):
     """Convert PIL image of any mode (RGB, HSV, LAB, etc) to grayscale version of image.
     This transform does not support torch Tensor.
 
     Args:
         img (PIL Image): PIL Image to be converted to grayscale.
         num_output_channels (int): number of channels of the output image. Value can be 1 or 3. Default is 1.
```

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/transforms/functional_pil.py` & `msadapter-0.1.0rc0/msadapter/torchvision/transforms/functional_pil.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,107 +3,107 @@
 import numbers
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
 from PIL import Image, ImageOps, ImageEnhance
 from typing_extensions import Literal
-from mindspore.ops import constexpr
+from mindspore.ops.primitive import _primexpr
 
 try:
     import accimage
 except ImportError:
     accimage = None
 from . import _pil_constants
 
 
-# @constexpr
+# @_primexpr
 def _is_pil_image(img: Any) -> bool:
     if accimage is not None:
         return isinstance(img, (Image.Image, accimage.Image))
     else:
         return isinstance(img, Image.Image)
 
 
-# @constexpr
+# @_primexpr
 def get_dimensions(img: Any) -> List[int]:
     if _is_pil_image(img):
         if hasattr(img, "getbands"):
             channels = len(img.getbands())
         else:
             channels = img.channels
         width, height = img.size
         return [channels, height, width]
     raise TypeError(f"Unexpected type {type(img)}")
 
 
-# @constexpr
+# @_primexpr
 def get_image_size(img: Any) -> List[int]:
     if _is_pil_image(img):
         return list(img.size)
     raise TypeError(f"Unexpected type {type(img)}")
 
 
-# @constexpr
+# @_primexpr
 def get_image_num_channels(img: Any) -> int:
     if _is_pil_image(img):
         if hasattr(img, "getbands"):
             return len(img.getbands())
         else:
             return img.channels
     raise TypeError(f"Unexpected type {type(img)}")
 
 
-# @constexpr
+# @_primexpr
 def hflip(img: Image.Image) -> Image.Image:
     if not _is_pil_image(img):
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
 
     return img.transpose(_pil_constants.FLIP_LEFT_RIGHT)
 
 
-# @constexpr
+# @_primexpr
 def vflip(img: Image.Image) -> Image.Image:
     if not _is_pil_image(img):
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
 
     return img.transpose(_pil_constants.FLIP_TOP_BOTTOM)
 
 
-# @constexpr
+# @_primexpr
 def adjust_brightness(img: Image.Image, brightness_factor: float) -> Image.Image:
     if not _is_pil_image(img):
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
 
     enhancer = ImageEnhance.Brightness(img)
     img = enhancer.enhance(brightness_factor)
     return img
 
 
-# @constexpr
+# @_primexpr
 def adjust_contrast(img: Image.Image, contrast_factor: float) -> Image.Image:
     if not _is_pil_image(img):
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
 
     enhancer = ImageEnhance.Contrast(img)
     img = enhancer.enhance(contrast_factor)
     return img
 
 
-# @constexpr
+# @_primexpr
 def adjust_saturation(img: Image.Image, saturation_factor: float) -> Image.Image:
     if not _is_pil_image(img):
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
 
     enhancer = ImageEnhance.Color(img)
     img = enhancer.enhance(saturation_factor)
     return img
 
 
-# @constexpr
+# @_primexpr
 def adjust_hue(img: Image.Image, hue_factor: float) -> Image.Image:
     if not (-0.5 <= hue_factor <= 0.5):
         raise ValueError(f"hue_factor ({hue_factor}) is not in [-0.5, 0.5].")
 
     if not _is_pil_image(img):
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
 
@@ -119,15 +119,15 @@
         np_h += np.uint8(hue_factor * 255)
     h = Image.fromarray(np_h, "L")
 
     img = Image.merge("HSV", (h, s, v)).convert(input_mode)
     return img
 
 
-# @constexpr
+# @_primexpr
 def adjust_gamma(
     img: Image.Image,
     gamma: float,
     gain: float = 1.0,
 ) -> Image.Image:
 
     if not _is_pil_image(img):
@@ -141,15 +141,15 @@
     gamma_map = [int((255 + 1 - 1e-3) * gain * pow(ele / 255.0, gamma)) for ele in range(256)] * 3
     img = img.point(gamma_map)  # use PIL's point-function to accelerate this part
 
     img = img.convert(input_mode)
     return img
 
 
-# @constexpr
+# @_primexpr
 def pad(
     img: Image.Image,
     padding: Union[int, List[int], Tuple[int, ...]],
     fill: Optional[Union[float, List[float], Tuple[float, ...]]] = 0,
     padding_mode: Literal["constant", "edge", "reflect", "symmetric"] = "constant",
 ) -> Image.Image:
 
@@ -221,30 +221,30 @@
         # Grayscale image
         if len(img.shape) == 2:
             img = np.pad(img, ((pad_top, pad_bottom), (pad_left, pad_right)), padding_mode)
 
         return Image.fromarray(img)
 
 
-# @constexpr
+# @_primexpr
 def crop(
     img: Image.Image,
     top: int,
     left: int,
     height: int,
     width: int,
 ) -> Image.Image:
 
     if not _is_pil_image(img):
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
 
     return img.crop((left, top, left + width, top + height))
 
 
-# @constexpr
+# @_primexpr
 def resize(
     img: Image.Image,
     size: Union[Sequence[int], int],
     interpolation: int = _pil_constants.BILINEAR,
     max_size: Optional[int] = None,
 ) -> Image.Image:
 
@@ -281,15 +281,15 @@
             raise ValueError(
                 "max_size should only be passed if size specifies the length of the smaller edge, "
                 "i.e. size should be an int or a sequence of length 1 in torchscript mode."
             )
         return img.resize(size[::-1], interpolation)
 
 
-# @constexpr
+# @_primexpr
 def _parse_fill(
     fill: Optional[Union[float, List[float], Tuple[float, ...]]],
     img: Image.Image,
     name: str = "fillcolor",
 ) -> Dict[str, Optional[Union[float, List[float], Tuple[float, ...]]]]:
 
     # Process fill color for affine transforms
@@ -310,15 +310,15 @@
             fill = tuple(int(x) for x in fill)
         else:
             fill = int(fill)
 
     return {name: fill}
 
 
-# @constexpr
+# @_primexpr
 def affine(
     img: Image.Image,
     matrix: List[float],
     interpolation: int = _pil_constants.NEAREST,
     fill: Optional[Union[float, List[float], Tuple[float, ...]]] = 0,
 ) -> Image.Image:
 
@@ -326,15 +326,15 @@
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
 
     output_size = img.size
     opts = _parse_fill(fill, img)
     return img.transform(output_size, _pil_constants.AFFINE, matrix, interpolation, **opts)
 
 
-# @constexpr
+# @_primexpr
 def rotate(
     img: Image.Image,
     angle: float,
     interpolation: int = _pil_constants.NEAREST,
     expand: bool = False,
     center: Optional[Tuple[int, int]] = None,
     fill: Optional[Union[float, List[float], Tuple[float, ...]]] = 0,
@@ -343,15 +343,15 @@
     if not _is_pil_image(img):
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
 
     opts = _parse_fill(fill, img)
     return img.rotate(angle, interpolation, expand, center, **opts)
 
 
-# @constexpr
+# @_primexpr
 def perspective(
     img: Image.Image,
     perspective_coeffs: float,
     interpolation: int = _pil_constants.BICUBIC,
     fill: Optional[Union[float, List[float], Tuple[float, ...]]] = 0,
 ) -> Image.Image:
 
@@ -359,15 +359,15 @@
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
 
     opts = _parse_fill(fill, img)
 
     return img.transform(img.size, _pil_constants.PERSPECTIVE, perspective_coeffs, interpolation, **opts)
 
 
-# @constexpr
+# @_primexpr
 def to_grayscale(img: Image.Image, num_output_channels: int) -> Image.Image:
     if not _is_pil_image(img):
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
 
     if num_output_channels == 1:
         img = img.convert("L")
     elif num_output_channels == 3:
@@ -377,50 +377,50 @@
         img = Image.fromarray(np_img, "RGB")
     else:
         raise ValueError("num_output_channels should be either 1 or 3")
 
     return img
 
 
-# @constexpr
+# @_primexpr
 def invert(img: Image.Image) -> Image.Image:
     if not _is_pil_image(img):
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
     return ImageOps.invert(img)
 
 
-# @constexpr
+# @_primexpr
 def posterize(img: Image.Image, bits: int) -> Image.Image:
     if not _is_pil_image(img):
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
     return ImageOps.posterize(img, bits)
 
 
-# @constexpr
+# @_primexpr
 def solarize(img: Image.Image, threshold: int) -> Image.Image:
     if not _is_pil_image(img):
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
     return ImageOps.solarize(img, threshold)
 
 
-# @constexpr
+# @_primexpr
 def adjust_sharpness(img: Image.Image, sharpness_factor: float) -> Image.Image:
     if not _is_pil_image(img):
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
 
     enhancer = ImageEnhance.Sharpness(img)
     img = enhancer.enhance(sharpness_factor)
     return img
 
 
-# @constexpr
+# @_primexpr
 def autocontrast(img: Image.Image) -> Image.Image:
     if not _is_pil_image(img):
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
     return ImageOps.autocontrast(img)
 
 
-# @constexpr
+# @_primexpr
 def equalize(img: Image.Image) -> Image.Image:
     if not _is_pil_image(img):
         raise TypeError(f"img should be PIL Image. Got {type(img)}")
     return ImageOps.equalize(img)
```

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/transforms/functional_tensor.py` & `msadapter-0.1.0rc0/msadapter/torchvision/transforms/functional_tensor.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/transforms/transforms.py` & `msadapter-0.1.0rc0/msadapter/torchvision/transforms/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numbers
 import random
 import warnings
 from collections.abc import Sequence
 from typing import Tuple, List, Optional
 
 import msadapter.pytorch as torch
-from mindspore.ops import constexpr
+from mindspore.ops.primitive import _primexpr
 from msadapter.pytorch import Tensor
 import mindspore.dataset.vision as msvision
 import mindspore.dataset.transforms as mstransforms
 from .functional import _is_numpy, _is_numpy_image
 import numpy as np
 
 try:
```

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/transforms/_functional_video.py` & `msadapter-0.1.0rc0/msadapter/torchvision/transforms/_functional_video.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/transforms/_pil_constants.py` & `msadapter-0.1.0rc0/msadapter/torchvision/transforms/_pil_constants.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/transforms/_presets.py` & `msadapter-0.1.0rc0/msadapter/torchvision/transforms/_presets.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/transforms/_transforms_video.py` & `msadapter-0.1.0rc0/msadapter/torchvision/transforms/_transforms_video.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/utils.py` & `msadapter-0.1.0rc0/msadapter/torchvision/utils.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/_internally_replaced_utils.py` & `msadapter-0.1.0rc0/msadapter/torchvision/_internally_replaced_utils.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/_utils.py` & `msadapter-0.1.0rc0/msadapter/torchvision/_utils.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/torchvision/__init__.py` & `msadapter-0.1.0rc0/msadapter/torchvision/__init__.py`

 * *Files identical despite different names*

### Comparing `msadapter-0.1.0b0/msadapter/utils.py` & `msadapter-0.1.0rc0/msadapter/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-from functools import lru_cache
+import collections
+# from functools import lru_cache
 import mindspore as ms
 from mindspore import context
-from mindspore.ops import constexpr
+from mindspore.ops.primitive import _primexpr
 
 
 _GLOBAL_LRU_CACHE_SIZE = 4
 _GLOBAL_LRU_CACHE_SIZE_NN = 256
 
 
 def unsupported_attr(attr):
     """
     To mark the attribute that is not currently supported.
     """
     return attr
 
-@constexpr
+@_primexpr
 def pynative_mode_condition():
     return context.get_context("mode") == context.PYNATIVE_MODE
 
-@constexpr
+@_primexpr
 def graph_mode_condition():
     return context.get_context("mode") == context.GRAPH_MODE
 
-@constexpr
+@_primexpr
 def get_backend():
     return context.get_context("device_target")
 
-@constexpr
+@_primexpr
 def is_under_gpu_context():
     return get_backend() == 'GPU'
 
-@constexpr
+@_primexpr
 def is_under_ascend_context():
     return get_backend() == 'Ascend'
 
-@constexpr
+@_primexpr
 def is_under_cpu_context():
     return get_backend() == 'CPU'
 
+@_primexpr
+def ascend_raise_implement_error(func):
+    if is_under_ascend_context():
+        raise NotImplementedError(func + " currently not support on Ascend")
+
+@_primexpr
+def set_name_tuple(name):
+    return collections.namedtuple(name, 'values, indices')
+
 _AscendGenernalConvertDict = {
     ms.float64: ms.float32,
     ms.int8: ms.float16,
     ms.int16: ms.float16,
     ms.int32: ms.float32,
     ms.int64: ms.float32,
     ms.uint8: ms.float16,
@@ -72,16 +82,16 @@
 
     _to_dtype = _AscendGenernalConvertDict.get(input.dtype)
     if _to_dtype:
         return input.astype(_to_dtype)
     return input
 
 
-@constexpr
-@lru_cache(_GLOBAL_LRU_CACHE_SIZE)
+@_primexpr
+# @lru_cache(_GLOBAL_LRU_CACHE_SIZE)
 def _infer_size(shape, numel):
     if len(shape) == 1 and isinstance(shape[0], tuple):
         shape = shape[0]
 
     dim = None
     newsize = 1
     for i, d in enumerate(shape):
```

### Comparing `msadapter-0.1.0b0/msadapter.egg-info/PKG-INFO` & `msadapter-0.1.0rc0/msadapter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msadapter
-Version: 0.1.0b0
+Version: 0.1.0rc0
 Summary: MSAdapter is a toolkit for support the PyTorch model running on Ascend.
 Home-page: https://openi.pcl.ac.cn/OpenI/MSAdapter 
 Author: Peng Cheng Lab, HUAWEI
 Author-email: pcl.openi@pcl.ac.cn
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -94,15 +94,15 @@
     import msadapter.pytorch.nn as nn
     import mindspore as ms
 
     net = MLP()
     net.train()
     epochs = 500
     criterion = nn.CrossEntropyLoss()
-    optimizer = torch.optim.SGD(net.parameters(), lr=0.01, momentum=0.9, weight_decay=0.0005)
+    optimizer = ms.nn.SGD(net.trainable_params(), learning_rate=0.01, momentum=0.9, weight_decay=0.0005)
 
     # Define the training process
     loss_net = ms.nn.WithLossCell(net, criterion)
     train_net = ms.nn.TrainOneStepCell(loss_net, optimizer)
 
     for i in range(epochs):
         for X, y in train_data:
```

### Comparing `msadapter-0.1.0b0/PKG-INFO` & `msadapter-0.1.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msadapter
-Version: 0.1.0b0
+Version: 0.1.0rc0
 Summary: MSAdapter is a toolkit for support the PyTorch model running on Ascend.
 Home-page: https://openi.pcl.ac.cn/OpenI/MSAdapter 
 Author: Peng Cheng Lab, HUAWEI
 Author-email: pcl.openi@pcl.ac.cn
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -94,15 +94,15 @@
     import msadapter.pytorch.nn as nn
     import mindspore as ms
 
     net = MLP()
     net.train()
     epochs = 500
     criterion = nn.CrossEntropyLoss()
-    optimizer = torch.optim.SGD(net.parameters(), lr=0.01, momentum=0.9, weight_decay=0.0005)
+    optimizer = ms.nn.SGD(net.trainable_params(), learning_rate=0.01, momentum=0.9, weight_decay=0.0005)
 
     # Define the training process
     loss_net = ms.nn.WithLossCell(net, criterion)
     train_net = ms.nn.TrainOneStepCell(loss_net, optimizer)
 
     for i in range(epochs):
         for X, y in train_data:
```

### Comparing `msadapter-0.1.0b0/README.rst` & `msadapter-0.1.0rc0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     import msadapter.pytorch.nn as nn
     import mindspore as ms
 
     net = MLP()
     net.train()
     epochs = 500
     criterion = nn.CrossEntropyLoss()
-    optimizer = torch.optim.SGD(net.parameters(), lr=0.01, momentum=0.9, weight_decay=0.0005)
+    optimizer = ms.nn.SGD(net.trainable_params(), learning_rate=0.01, momentum=0.9, weight_decay=0.0005)
 
     # Define the training process
     loss_net = ms.nn.WithLossCell(net, criterion)
     train_net = ms.nn.TrainOneStepCell(loss_net, optimizer)
 
     for i in range(epochs):
         for X, y in train_data:
```

### Comparing `msadapter-0.1.0b0/setup.py` & `msadapter-0.1.0rc0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from __future__ import absolute_import
 from setuptools import setup, find_packages
 import os, codecs
 
 MAJOR = 0
 MINOR = 1
 PATCH = 0
-PRE_RELEASE = 'beta'
+PRE_RELEASE = 'rc'
 # Use the following formatting: (major, minor, patch, prerelease)
 VERSION = (MAJOR, MINOR, PATCH, PRE_RELEASE)
 
 if os.path.exists('README.rst'):
     # codec is used for consistent encoding
     long_description = codecs.open(
         os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.rst'), 'r', 'utf-8'
```

