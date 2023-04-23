# Comparing `tmp/neuralogic-0.7.5.tar.gz` & `tmp/neuralogic-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralogic-0.7.5.tar", last modified: Fri Apr  7 19:40:36 2023, max compression
+gzip compressed data, was "neuralogic-0.7.6.tar", last modified: Sun Apr 23 16:05:33 2023, max compression
```

## Comparing `neuralogic-0.7.5.tar` & `neuralogic-0.7.6.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-07 19:40:25.000000 neuralogic-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-04-07 19:40:36.401836 neuralogic-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-04-07 19:40:25.000000 neuralogic-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.389835 neuralogic-0.7.5/neuralogic/
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 19:40:34.000000 neuralogic-0.7.5/neuralogic/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.389835 neuralogic-0.7.5/neuralogic/core/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.389835 neuralogic-0.7.5/neuralogic/core/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/builder/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/builder/dataset_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.389835 neuralogic-0.7.5/neuralogic/core/constructs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.393835 neuralogic-0.7.5/neuralogic/core/constructs/function/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/function/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/function/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/function/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/function/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/function/softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/java_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.393835 neuralogic-0.7.5/neuralogic/core/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/settings/settings_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.393835 neuralogic-0.7.5/neuralogic/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/dataset/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/dataset/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/dataset/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/dataset/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/dataset/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.393835 neuralogic-0.7.5/neuralogic/db/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/db/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.393835 neuralogic-0.7.5/neuralogic/db/pg/
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/db/pg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/db/pg/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.393835 neuralogic-0.7.5/neuralogic/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/inference/evaluation_inference_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/inference/inference_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.393835 neuralogic-0.7.5/neuralogic/jar/
--rw-r--r--   0 runner    (1001) docker     (123)  2007653 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/jar/NeuraLogic.jar
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/jar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.393835 neuralogic-0.7.5/neuralogic/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/nn/evaluator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/evaluator/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/java.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/nn/module/
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/nn/module/general/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/gru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/rvnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/nn/module/gnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/appnp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/gatv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/gin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/gsage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/res_gated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/rgcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/sg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/nn/module/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/meta/magnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/meta/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/torch_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/optim/adam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/optim/lr_scheduler/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/optim/lr_scheduler/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/optim/lr_scheduler/lr_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/optim/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/optim/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.389835 neuralogic-0.7.5/neuralogic/utils/data/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/atomEmbeddings3.txt
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/bondEmbeddings3.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/
--rw-r--r--   0 runner    (1001) docker     (123)   402216 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/queries.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/template.txt_merged.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/embeddings.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_crosssum.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_elementProduct.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_gnn.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_graphlets.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_partial.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_product.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/data/datasets/nations/
--rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/nations/embeddings.txt
--rw-r--r--   0 runner    (1001) docker     (123)    38585 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/nations/examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)   205423 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/nations/queries.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/nations/template.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.389835 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/family/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/family/examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/family/queries.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/family/template.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/trains/
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/trains/examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/trains/queries.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/trains/template.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.389835 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/generalized/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/generalized/examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/generalized/template.txt
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/generalized/texamples.txt
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/generalized/ztexamples.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/naive/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/naive/template.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/naive/trainExamples.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/solution/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/solution/template.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/solution/testExamples.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/vectorized/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/vectorized/template.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/vectorized/trainExamples.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/visualize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.389835 neuralogic-0.7.5/neuralogic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-04-07 19:40:36.000000 neuralogic-0.7.5/neuralogic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-04-07 19:40:36.000000 neuralogic-0.7.5/neuralogic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 19:40:36.000000 neuralogic-0.7.5/neuralogic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 19:40:36.000000 neuralogic-0.7.5/neuralogic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-07 19:40:36.000000 neuralogic-0.7.5/neuralogic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-07 19:40:25.000000 neuralogic-0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 19:40:36.401836 neuralogic-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-07 19:40:25.000000 neuralogic-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.592146 neuralogic-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-23 16:05:22.000000 neuralogic-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-04-23 16:05:33.592146 neuralogic-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-04-23 16:05:22.000000 neuralogic-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.564146 neuralogic-0.7.6/neuralogic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 16:05:32.000000 neuralogic-0.7.6/neuralogic/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.568146 neuralogic-0.7.6/neuralogic/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.568146 neuralogic-0.7.6/neuralogic/core/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/builder/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/builder/dataset_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.568146 neuralogic-0.7.6/neuralogic/core/constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/constructs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/constructs/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.572146 neuralogic-0.7.6/neuralogic/core/constructs/function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/constructs/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/constructs/function/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/constructs/function/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/constructs/function/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/constructs/function/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/constructs/function/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/constructs/java_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/constructs/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/constructs/predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/constructs/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/constructs/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.572146 neuralogic-0.7.6/neuralogic/core/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/settings/settings_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/core/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.572146 neuralogic-0.7.6/neuralogic/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/dataset/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/dataset/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/dataset/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/dataset/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/dataset/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.572146 neuralogic-0.7.6/neuralogic/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/db/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.572146 neuralogic-0.7.6/neuralogic/db/pg/
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/db/pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/db/pg/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.572146 neuralogic-0.7.6/neuralogic/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/inference/evaluation_inference_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/inference/inference_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.572146 neuralogic-0.7.6/neuralogic/jar/
+-rw-r--r--   0 runner    (1001) docker     (123)  2007653 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/jar/NeuraLogic.jar
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/jar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.572146 neuralogic-0.7.6/neuralogic/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.572146 neuralogic-0.7.6/neuralogic/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.576146 neuralogic-0.7.6/neuralogic/nn/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/evaluator/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.576146 neuralogic-0.7.6/neuralogic/nn/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.580146 neuralogic-0.7.6/neuralogic/nn/module/general/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/general/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/general/gru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/general/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/general/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/general/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/general/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/general/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/general/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/general/rvnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/general/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.584146 neuralogic-0.7.6/neuralogic/nn/module/gnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/gnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/gnn/appnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/gnn/gatv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/gnn/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/gnn/gin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/gnn/gsage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/gnn/res_gated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/gnn/rgcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/gnn/sg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/gnn/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.584146 neuralogic-0.7.6/neuralogic/nn/module/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/meta/magnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/meta/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/module/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/nn/torch_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.584146 neuralogic-0.7.6/neuralogic/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/optim/adam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.584146 neuralogic-0.7.6/neuralogic/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/optim/lr_scheduler/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/optim/lr_scheduler/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/optim/lr_scheduler/lr_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/optim/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/optim/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.584146 neuralogic-0.7.6/neuralogic/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.584146 neuralogic-0.7.6/neuralogic/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.560146 neuralogic-0.7.6/neuralogic/utils/data/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.584146 neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/atomEmbeddings3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/bondEmbeddings3.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.588146 neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/mutagenesis/
+-rw-r--r--   0 runner    (1001) docker     (123)   402216 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/mutagenesis/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/mutagenesis/queries.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/mutagenesis/template.txt_merged.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.588146 neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/embeddings.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_crosssum.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_elementProduct.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_gnn.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_graphlets.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_partial.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_product.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.592146 neuralogic-0.7.6/neuralogic/utils/data/datasets/nations/
+-rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/nations/embeddings.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38585 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/nations/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   205423 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/nations/queries.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/nations/template.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.564146 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.592146 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/family/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/family/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/family/queries.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/family/template.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.592146 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/trains/
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/trains/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/trains/queries.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/trains/template.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.564146 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/xor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.592146 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/xor/generalized/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/xor/generalized/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/xor/generalized/template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/xor/generalized/texamples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/xor/generalized/ztexamples.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.592146 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/xor/naive/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/xor/naive/template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/xor/naive/trainExamples.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.592146 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/xor/solution/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/xor/solution/template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/xor/solution/testExamples.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.592146 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/xor/vectorized/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/xor/vectorized/template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/xor/vectorized/trainExamples.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.592146 neuralogic-0.7.6/neuralogic/utils/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-04-23 16:05:22.000000 neuralogic-0.7.6/neuralogic/utils/visualize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:05:33.568146 neuralogic-0.7.6/neuralogic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-04-23 16:05:33.000000 neuralogic-0.7.6/neuralogic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-04-23 16:05:33.000000 neuralogic-0.7.6/neuralogic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:05:33.000000 neuralogic-0.7.6/neuralogic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-23 16:05:33.000000 neuralogic-0.7.6/neuralogic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 16:05:33.000000 neuralogic-0.7.6/neuralogic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-23 16:05:22.000000 neuralogic-0.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 16:05:33.592146 neuralogic-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-23 16:05:22.000000 neuralogic-0.7.6/setup.py
```

### Comparing `neuralogic-0.7.5/LICENSE` & `neuralogic-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/PKG-INFO` & `neuralogic-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralogic
-Version: 0.7.5
+Version: 0.7.6
 Summary: PyNeuraLogic lets you use Python to create Differentiable Logic Programs.
 Home-page: https://github.com/LukasZahradnik/PyNeuraLogic
 Author: Lukáš Zahradník
 Author-email: lukaszahradnik96@seznam.cz
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neuralogic Version: 0.7.5 Summary: PyNeuraLogic
+Metadata-Version: 2.1 Name: neuralogic Version: 0.7.6 Summary: PyNeuraLogic
 lets you use Python to create Differentiable Logic Programs. Home-page: https:/
 /github.com/LukasZahradnik/PyNeuraLogic Author: LukÃ¡Å¡ ZahradnÃ­k Author-
 email: lukaszahradnik96@seznam.cz License: MIT Classifier: License :: OSI
 Approved :: MIT License Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `neuralogic-0.7.5/README.md` & `neuralogic-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/__init__.py` & `neuralogic-0.7.6/neuralogic/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/__init__.py` & `neuralogic-0.7.6/neuralogic/core/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/builder/builder.py` & `neuralogic-0.7.6/neuralogic/core/builder/builder.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/builder/components.py` & `neuralogic-0.7.6/neuralogic/core/builder/components.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/builder/dataset_builder.py` & `neuralogic-0.7.6/neuralogic/core/builder/dataset_builder.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/constructs/factories.py` & `neuralogic-0.7.6/neuralogic/core/constructs/factories.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/constructs/function/__init__.py` & `neuralogic-0.7.6/neuralogic/core/constructs/function/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/constructs/function/concat.py` & `neuralogic-0.7.6/neuralogic/core/constructs/function/concat.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/constructs/function/function.py` & `neuralogic-0.7.6/neuralogic/core/constructs/function/function.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/constructs/function/reshape.py` & `neuralogic-0.7.6/neuralogic/core/constructs/function/reshape.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/constructs/function/slice.py` & `neuralogic-0.7.6/neuralogic/core/constructs/function/slice.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/constructs/function/softmax.py` & `neuralogic-0.7.6/neuralogic/core/constructs/function/softmax.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/constructs/java_objects.py` & `neuralogic-0.7.6/neuralogic/core/constructs/java_objects.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/constructs/metadata.py` & `neuralogic-0.7.6/neuralogic/core/constructs/metadata.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/constructs/predicate.py` & `neuralogic-0.7.6/neuralogic/core/constructs/predicate.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/constructs/relation.py` & `neuralogic-0.7.6/neuralogic/core/constructs/relation.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/constructs/rule.py` & `neuralogic-0.7.6/neuralogic/core/constructs/rule.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/settings/__init__.py` & `neuralogic-0.7.6/neuralogic/core/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/settings/settings_proxy.py` & `neuralogic-0.7.6/neuralogic/core/settings/settings_proxy.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/sources.py` & `neuralogic-0.7.6/neuralogic/core/sources.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/core/template.py` & `neuralogic-0.7.6/neuralogic/core/template.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/dataset/__init__.py` & `neuralogic-0.7.6/neuralogic/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/dataset/base.py` & `neuralogic-0.7.6/neuralogic/dataset/base.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/dataset/csv.py` & `neuralogic-0.7.6/neuralogic/dataset/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,18 +101,20 @@
             line = fp.readline()
 
             if not line or not line.strip():
                 break
 
             terms = line.strip().split(self.sep)
             if use_columns is None:
-                line_relation = relation([(term.strip() if len(term.strip()) else replace_empty) for term in terms])
+                line_relation = relation(
+                    [(term.strip().lower() if len(term.strip()) else replace_empty) for term in terms]
+                )
             else:
                 line_relation = relation(
-                    [(terms[i].strip() if len(terms[i].strip()) else replace_empty) for i in use_columns]
+                    [(terms[i].strip().lower() if len(terms[i].strip()) else replace_empty) for i in use_columns]
                 )
 
             if value_column is None:
                 if default_value is not None:
                     line_relation = line_relation[float(default_value)]
             else:
                 value = terms[value_column].strip()
```

### Comparing `neuralogic-0.7.5/neuralogic/dataset/db.py` & `neuralogic-0.7.6/neuralogic/dataset/db.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/dataset/file.py` & `neuralogic-0.7.6/neuralogic/dataset/file.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/dataset/logic.py` & `neuralogic-0.7.6/neuralogic/dataset/logic.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/dataset/tensor.py` & `neuralogic-0.7.6/neuralogic/dataset/tensor.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/db/converter.py` & `neuralogic-0.7.6/neuralogic/db/converter.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/db/pg/__init__.py` & `neuralogic-0.7.6/neuralogic/db/pg/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/db/pg/helpers.py` & `neuralogic-0.7.6/neuralogic/db/pg/helpers.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/inference/evaluation_inference_engine.py` & `neuralogic-0.7.6/neuralogic/inference/evaluation_inference_engine.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/inference/inference_engine.py` & `neuralogic-0.7.6/neuralogic/inference/inference_engine.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/jar/NeuraLogic.jar` & `neuralogic-0.7.6/neuralogic/jar/NeuraLogic.jar`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/logging/__init__.py` & `neuralogic-0.7.6/neuralogic/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/base.py` & `neuralogic-0.7.6/neuralogic/nn/base.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/evaluator/java.py` & `neuralogic-0.7.6/neuralogic/nn/evaluator/java.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/functional.py` & `neuralogic-0.7.6/neuralogic/nn/functional.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/init.py` & `neuralogic-0.7.6/neuralogic/nn/init.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/java.py` & `neuralogic-0.7.6/neuralogic/nn/java.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/loss.py` & `neuralogic-0.7.6/neuralogic/nn/loss.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/__init__.py` & `neuralogic-0.7.6/neuralogic/nn/module/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/general/attention.py` & `neuralogic-0.7.6/neuralogic/nn/module/general/attention.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/general/gru.py` & `neuralogic-0.7.6/neuralogic/nn/module/general/gru.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/general/linear.py` & `neuralogic-0.7.6/neuralogic/nn/module/general/linear.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/general/lstm.py` & `neuralogic-0.7.6/neuralogic/nn/module/general/lstm.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/general/mlp.py` & `neuralogic-0.7.6/neuralogic/nn/module/general/mlp.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/general/pooling.py` & `neuralogic-0.7.6/neuralogic/nn/module/general/pooling.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/general/positional_encoding.py` & `neuralogic-0.7.6/neuralogic/nn/module/general/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/general/rnn.py` & `neuralogic-0.7.6/neuralogic/nn/module/general/rnn.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/general/rvnn.py` & `neuralogic-0.7.6/neuralogic/nn/module/general/rvnn.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/general/transformer.py` & `neuralogic-0.7.6/neuralogic/nn/module/general/transformer.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/gnn/appnp.py` & `neuralogic-0.7.6/neuralogic/nn/module/gnn/appnp.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/gnn/gatv2.py` & `neuralogic-0.7.6/neuralogic/nn/module/gnn/gatv2.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/gnn/gcn.py` & `neuralogic-0.7.6/neuralogic/nn/module/gnn/gcn.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/gnn/gin.py` & `neuralogic-0.7.6/neuralogic/nn/module/gnn/gin.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/gnn/gsage.py` & `neuralogic-0.7.6/neuralogic/nn/module/gnn/gsage.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/gnn/res_gated.py` & `neuralogic-0.7.6/neuralogic/nn/module/gnn/res_gated.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/gnn/rgcn.py` & `neuralogic-0.7.6/neuralogic/nn/module/gnn/rgcn.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/gnn/sg.py` & `neuralogic-0.7.6/neuralogic/nn/module/gnn/sg.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/gnn/tag.py` & `neuralogic-0.7.6/neuralogic/nn/module/gnn/tag.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/meta/magnn.py` & `neuralogic-0.7.6/neuralogic/nn/module/meta/magnn.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/module/meta/meta.py` & `neuralogic-0.7.6/neuralogic/nn/module/meta/meta.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/nn/torch_function.py` & `neuralogic-0.7.6/neuralogic/nn/torch_function.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/optim/adam.py` & `neuralogic-0.7.6/neuralogic/optim/adam.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/optim/lr_scheduler/arithmetic.py` & `neuralogic-0.7.6/neuralogic/optim/lr_scheduler/arithmetic.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/optim/lr_scheduler/geometric.py` & `neuralogic-0.7.6/neuralogic/optim/lr_scheduler/geometric.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/optim/lr_scheduler/lr_decay.py` & `neuralogic-0.7.6/neuralogic/optim/lr_scheduler/lr_decay.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/optim/optimizer.py` & `neuralogic-0.7.6/neuralogic/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/optim/sgd.py` & `neuralogic-0.7.6/neuralogic/optim/sgd.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/utils/data/__init__.py` & `neuralogic-0.7.6/neuralogic/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/atomEmbeddings3.txt` & `neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/atomEmbeddings3.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/examples.txt` & `neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/mutagenesis/examples.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/template.txt_merged.txt` & `neuralogic-0.7.6/neuralogic/utils/data/datasets/molecules/mutagenesis/template.txt_merged.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/utils/data/datasets/nations/embeddings.txt` & `neuralogic-0.7.6/neuralogic/utils/data/datasets/nations/embeddings.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/utils/data/datasets/nations/examples.txt` & `neuralogic-0.7.6/neuralogic/utils/data/datasets/nations/examples.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/utils/data/datasets/nations/queries.txt` & `neuralogic-0.7.6/neuralogic/utils/data/datasets/nations/queries.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/trains/examples.txt` & `neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/trains/examples.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/trains/template.txt` & `neuralogic-0.7.6/neuralogic/utils/data/datasets/simple/trains/template.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic/utils/visualize/__init__.py` & `neuralogic-0.7.6/neuralogic/utils/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/neuralogic.egg-info/PKG-INFO` & `neuralogic-0.7.6/neuralogic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralogic
-Version: 0.7.5
+Version: 0.7.6
 Summary: PyNeuraLogic lets you use Python to create Differentiable Logic Programs.
 Home-page: https://github.com/LukasZahradnik/PyNeuraLogic
 Author: Lukáš Zahradník
 Author-email: lukaszahradnik96@seznam.cz
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neuralogic Version: 0.7.5 Summary: PyNeuraLogic
+Metadata-Version: 2.1 Name: neuralogic Version: 0.7.6 Summary: PyNeuraLogic
 lets you use Python to create Differentiable Logic Programs. Home-page: https:/
 /github.com/LukasZahradnik/PyNeuraLogic Author: LukÃ¡Å¡ ZahradnÃ­k Author-
 email: lukaszahradnik96@seznam.cz License: MIT Classifier: License :: OSI
 Approved :: MIT License Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `neuralogic-0.7.5/neuralogic.egg-info/SOURCES.txt` & `neuralogic-0.7.6/neuralogic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.5/setup.py` & `neuralogic-0.7.6/setup.py`

 * *Files identical despite different names*

