# Comparing `tmp/fedbase-0.9.4.tar.gz` & `tmp/fedbase-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedbase-0.9.4.tar", last modified: Tue Apr  4 07:09:26 2023, max compression
+gzip compressed data, was "fedbase-0.9.5.tar", last modified: Sun Apr 23 01:06:07 2023, max compression
```

## Comparing `fedbase-0.9.4.tar` & `fedbase-0.9.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 07:09:26.153522 fedbase-0.9.4/
--rw-rw-rw-   0        0        0     1083 2021-11-25 09:10:20.000000 fedbase-0.9.4/LICENSE
--rw-rw-rw-   0        0        0     2297 2023-04-04 07:09:26.153522 fedbase-0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2022-04-16 12:00:00.000000 fedbase-0.9.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 07:09:26.101108 fedbase-0.9.4/fedbase/
--rw-rw-rw-   0        0        0       16 2021-11-25 09:27:32.000000 fedbase-0.9.4/fedbase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:09:26.137522 fedbase-0.9.4/fedbase/baselines/
--rw-rw-rw-   0        0        0     1191 2023-02-03 00:08:19.000000 fedbase-0.9.4/fedbase/baselines/Central.py
--rw-rw-rw-   0        0        0     2262 2023-02-03 05:50:50.000000 fedbase-0.9.4/fedbase/baselines/Ditto.py
--rw-rw-rw-   0        0        0     2500 2023-04-04 05:15:36.000000 fedbase-0.9.4/fedbase/baselines/Fedavg.py
--rw-rw-rw-   0        0        0     2543 2023-02-03 05:50:54.000000 fedbase-0.9.4/fedbase/baselines/Fedavg_finetune.py
--rw-rw-rw-   0        0        0     2147 2023-02-04 11:27:20.000000 fedbase-0.9.4/fedbase/baselines/Local.py
--rw-rw-rw-   0        0        0      213 2023-02-07 09:23:33.000000 fedbase-0.9.4/fedbase/baselines/__init__.py
--rw-rw-rw-   0        0        0     2777 2023-02-03 00:02:30.000000 fedbase-0.9.4/fedbase/baselines/fedavg_ensemble.py
--rw-rw-rw-   0        0        0     2368 2023-02-03 00:08:39.000000 fedbase-0.9.4/fedbase/baselines/fedprox.py
--rw-rw-rw-   0        0        0     2890 2023-02-03 00:02:10.000000 fedbase-0.9.4/fedbase/baselines/fedprox_ensemble.py
--rw-rw-rw-   0        0        0     3142 2023-02-03 00:15:00.000000 fedbase-0.9.4/fedbase/baselines/fesem.py
--rw-rw-rw-   0        0        0     4966 2023-03-06 06:29:23.000000 fedbase-0.9.4/fedbase/baselines/fesem_con.py
--rw-rw-rw-   0        0        0     3774 2023-02-17 00:15:09.000000 fedbase-0.9.4/fedbase/baselines/ifca.py
--rw-rw-rw-   0        0        0     4378 2023-03-06 06:23:47.000000 fedbase-0.9.4/fedbase/baselines/ifca_con.py
--rw-rw-rw-   0        0        0     4701 2023-04-04 05:17:58.000000 fedbase-0.9.4/fedbase/baselines/ifca_res.py
--rw-rw-rw-   0        0        0     4330 2023-02-18 08:23:21.000000 fedbase-0.9.4/fedbase/baselines/wecfl.py
--rw-rw-rw-   0        0        0     4944 2023-02-24 00:32:13.000000 fedbase-0.9.4/fedbase/baselines/wecfl_con.py
--rw-rw-rw-   0        0        0     4413 2023-02-18 08:56:27.000000 fedbase-0.9.4/fedbase/baselines/wecfl_res.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:09:26.140521 fedbase-0.9.4/fedbase/model/
--rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.4/fedbase/model/__init__.py
--rw-rw-rw-   0        0        0     7655 2023-02-18 03:01:07.000000 fedbase-0.9.4/fedbase/model/model.py
--rw-rw-rw-   0        0        0     9298 2021-11-25 11:00:44.000000 fedbase-0.9.4/fedbase/model/resnet.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:09:26.142522 fedbase-0.9.4/fedbase/nodes/
--rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.4/fedbase/nodes/__init__.py
--rw-rw-rw-   0        0        0    14825 2023-04-04 04:53:22.000000 fedbase-0.9.4/fedbase/nodes/node.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:09:26.144523 fedbase-0.9.4/fedbase/server/
--rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.4/fedbase/server/__init__.py
--rw-rw-rw-   0        0        0     5838 2023-04-04 05:15:22.000000 fedbase-0.9.4/fedbase/server/server.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:09:26.152523 fedbase-0.9.4/fedbase/utils/
--rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.4/fedbase/utils/__init__.py
--rw-rw-rw-   0        0        0    14531 2023-01-26 03:50:21.000000 fedbase-0.9.4/fedbase/utils/data_loader.py
--rw-rw-rw-   0        0        0     6168 2021-11-25 11:00:44.000000 fedbase-0.9.4/fedbase/utils/femnist.py
--rw-rw-rw-   0        0        0      944 2021-12-15 01:18:16.000000 fedbase-0.9.4/fedbase/utils/model_utils.py
--rw-rw-rw-   0        0        0     1602 2022-05-15 12:45:37.000000 fedbase-0.9.4/fedbase/utils/utils.py
--rw-rw-rw-   0        0        0     1125 2022-12-08 06:10:12.000000 fedbase-0.9.4/fedbase/utils/visualize.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:09:26.118653 fedbase-0.9.4/fedbase.egg-info/
--rw-rw-rw-   0        0        0     2297 2023-04-04 07:09:25.000000 fedbase-0.9.4/fedbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1165 2023-04-04 07:09:26.000000 fedbase-0.9.4/fedbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 07:09:25.000000 fedbase-0.9.4/fedbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-04 07:09:25.000000 fedbase-0.9.4/fedbase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 07:09:26.153522 fedbase-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-04-04 07:09:15.000000 fedbase-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:06:07.627728 fedbase-0.9.5/
+-rw-rw-rw-   0        0        0     1083 2021-11-25 09:10:20.000000 fedbase-0.9.5/LICENSE
+-rw-rw-rw-   0        0        0     2297 2023-04-23 01:06:07.626731 fedbase-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1783 2022-04-16 12:00:00.000000 fedbase-0.9.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 01:06:07.573728 fedbase-0.9.5/fedbase/
+-rw-rw-rw-   0        0        0       16 2021-11-25 09:27:32.000000 fedbase-0.9.5/fedbase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:06:07.613729 fedbase-0.9.5/fedbase/baselines/
+-rw-rw-rw-   0        0        0     1191 2023-02-03 00:08:19.000000 fedbase-0.9.5/fedbase/baselines/Central.py
+-rw-rw-rw-   0        0        0     2442 2023-04-04 07:24:24.000000 fedbase-0.9.5/fedbase/baselines/Ditto.py
+-rw-rw-rw-   0        0        0     2504 2023-04-04 07:25:03.000000 fedbase-0.9.5/fedbase/baselines/Fedavg.py
+-rw-rw-rw-   0        0        0     2721 2023-04-04 07:25:55.000000 fedbase-0.9.5/fedbase/baselines/Fedavg_finetune.py
+-rw-rw-rw-   0        0        0     2147 2023-02-04 11:27:20.000000 fedbase-0.9.5/fedbase/baselines/Local.py
+-rw-rw-rw-   0        0        0      213 2023-02-07 09:23:33.000000 fedbase-0.9.5/fedbase/baselines/__init__.py
+-rw-rw-rw-   0        0        0     2970 2023-04-04 07:26:42.000000 fedbase-0.9.5/fedbase/baselines/fedavg_ensemble.py
+-rw-rw-rw-   0        0        0     2561 2023-04-04 07:25:15.000000 fedbase-0.9.5/fedbase/baselines/fedprox.py
+-rw-rw-rw-   0        0        0     3083 2023-04-04 07:23:54.000000 fedbase-0.9.5/fedbase/baselines/fedprox_ensemble.py
+-rw-rw-rw-   0        0        0     3142 2023-02-03 00:15:00.000000 fedbase-0.9.5/fedbase/baselines/fesem.py
+-rw-rw-rw-   0        0        0     5123 2023-04-04 07:41:10.000000 fedbase-0.9.5/fedbase/baselines/fesem_con.py
+-rw-rw-rw-   0        0        0     3774 2023-02-17 00:15:09.000000 fedbase-0.9.5/fedbase/baselines/ifca.py
+-rw-rw-rw-   0        0        0     4378 2023-03-06 06:23:47.000000 fedbase-0.9.5/fedbase/baselines/ifca_con.py
+-rw-rw-rw-   0        0        0     4701 2023-04-04 05:17:58.000000 fedbase-0.9.5/fedbase/baselines/ifca_res.py
+-rw-rw-rw-   0        0        0     4330 2023-02-18 08:23:21.000000 fedbase-0.9.5/fedbase/baselines/wecfl.py
+-rw-rw-rw-   0        0        0     4852 2023-04-23 01:04:22.000000 fedbase-0.9.5/fedbase/baselines/wecfl_con.py
+-rw-rw-rw-   0        0        0     4413 2023-02-18 08:56:27.000000 fedbase-0.9.5/fedbase/baselines/wecfl_res.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:06:07.616731 fedbase-0.9.5/fedbase/model/
+-rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.5/fedbase/model/__init__.py
+-rw-rw-rw-   0        0        0     7655 2023-02-18 03:01:07.000000 fedbase-0.9.5/fedbase/model/model.py
+-rw-rw-rw-   0        0        0     9298 2021-11-25 11:00:44.000000 fedbase-0.9.5/fedbase/model/resnet.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:06:07.618729 fedbase-0.9.5/fedbase/nodes/
+-rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.5/fedbase/nodes/__init__.py
+-rw-rw-rw-   0        0        0    14825 2023-04-04 04:53:22.000000 fedbase-0.9.5/fedbase/nodes/node.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:06:07.619729 fedbase-0.9.5/fedbase/server/
+-rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.5/fedbase/server/__init__.py
+-rw-rw-rw-   0        0        0     5838 2023-04-04 05:15:22.000000 fedbase-0.9.5/fedbase/server/server.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:06:07.625729 fedbase-0.9.5/fedbase/utils/
+-rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.5/fedbase/utils/__init__.py
+-rw-rw-rw-   0        0        0    14531 2023-04-23 01:05:04.000000 fedbase-0.9.5/fedbase/utils/data_loader.py
+-rw-rw-rw-   0        0        0     6168 2021-11-25 11:00:44.000000 fedbase-0.9.5/fedbase/utils/femnist.py
+-rw-rw-rw-   0        0        0      944 2021-12-15 01:18:16.000000 fedbase-0.9.5/fedbase/utils/model_utils.py
+-rw-rw-rw-   0        0        0     1694 2023-04-23 01:03:36.000000 fedbase-0.9.5/fedbase/utils/tools.py
+-rw-rw-rw-   0        0        0     1125 2022-12-08 06:10:12.000000 fedbase-0.9.5/fedbase/utils/visualize.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:06:07.592727 fedbase-0.9.5/fedbase.egg-info/
+-rw-rw-rw-   0        0        0     2297 2023-04-23 01:06:07.000000 fedbase-0.9.5/fedbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1165 2023-04-23 01:06:07.000000 fedbase-0.9.5/fedbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 01:06:07.000000 fedbase-0.9.5/fedbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 01:06:07.000000 fedbase-0.9.5/fedbase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 01:06:07.627728 fedbase-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-04-23 01:05:53.000000 fedbase-0.9.5/setup.py
```

### Comparing `fedbase-0.9.4/LICENSE` & `fedbase-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.4/PKG-INFO` & `fedbase-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedbase
-Version: 0.9.4
+Version: 0.9.5
 Summary: An easy, silly, DIY Federated Learning framework with many baselines for individual researchers.
 Home-page: https://github.com/jie-ma-ai/FedBase
 Author: Jie MA
 Author-email: ustcmj@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedbase-0.9.4/README.md` & `fedbase-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.4/fedbase/baselines/Central.py` & `fedbase-0.9.5/fedbase/baselines/Central.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.4/fedbase/baselines/Ditto.py` & `fedbase-0.9.5/fedbase/baselines/Local.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from fedbase.server.server import server_class
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 import os
 from functools import partial
 
-def run(dataset_splited, batch_size, num_nodes, model, objective, optimizer, global_rounds, local_steps, reg, device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
+
+def run(dataset_splited, batch_size, num_nodes, model, objective, optimizer, global_rounds, local_steps, device = torch.device('cuda' if torch.cuda.is_available() else 'cpu'), log_file=True):
     # dt = data_process(dataset)
     # train_splited, test_splited = dt.split_dataset(num_nodes, split['split_para'], split['split_method'])
     train_splited, test_splited, split_para = dataset_splited
 
     server = server_class(device)
     server.assign_model(model())
 
@@ -37,18 +38,17 @@
     server.distribute(nodes, list(range(num_nodes)))
 
     # train!
     for i in range(global_rounds):
         print('-------------------Global round %d start-------------------' % (i))
         # single-processing!
         for j in range(num_nodes):
-            nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_fedprox, reg_model = server.model, lam= reg))
+            nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step))
             nodes[j].local_test()
-        # server aggregation
-        server.aggregate(nodes, list(range(num_nodes)))
         # test accuracy
         server.acc(nodes, list(range(num_nodes)))
 
     # log
-    log(os.path.basename(__file__)[:-3] + '_' + str(reg) + '_' + split_para , nodes, server)
+    if log_file:
+        log(os.path.basename(__file__)[:-3] + '_' + split_para, nodes, server)
 
     return [nodes[i].model for i in range(num_nodes)]
```

### Comparing `fedbase-0.9.4/fedbase/baselines/Fedavg.py` & `fedbase-0.9.5/fedbase/baselines/Fedavg.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         # optim
         nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
 
     del train_splited, test_splited
 
     # initialize parameters to nodes
     server.distribute([nodes[i].model for i in range(num_nodes)])
-
     weight_list = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
+    
     # train!
     for i in range(global_rounds):
         print('-------------------Global round %d start-------------------' % (i))
         # single-processing!
         for j in range(num_nodes):
             nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step))
         # server aggregation and distribution
```

### Comparing `fedbase-0.9.4/fedbase/baselines/Fedavg_finetune.py` & `fedbase-0.9.5/fedbase/baselines/Fedavg_finetune.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,33 +31,34 @@
         nodes[i].assign_objective(objective())
         # optim
         nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
     
     del train_splited, test_splited
 
     # initialize parameters to nodes
-    server.distribute(nodes, list(range(num_nodes)))
+    weight_list = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
+    server.distribute([nodes[i].model for i in range(num_nodes)])
 
     # train!
     for i in range(global_rounds):
         print('-------------------Global round %d start-------------------' % (i))
         # single-processing!
         for j in range(num_nodes):
             nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step))
         # server aggregation and distribution
-        server.aggregate(nodes, list(range(num_nodes)))
-        server.distribute(nodes, list(range(num_nodes)))
+        server.model.load_state_dict(server.aggregate([nodes[i].model for i in range(num_nodes)], weight_list))
+        server.distribute([nodes[i].model for i in range(num_nodes)])
         # test accuracy
         for j in range(num_nodes):
             nodes[j].local_test()
-        server.acc(nodes, list(range(num_nodes)))
+        server.acc(nodes, weight_list)
 
     # fine tune
     for j in range(num_nodes):
         nodes[j].local_update_steps(finetune_steps, partial(nodes[j].train_single_step))
         nodes[j].local_test()
-    server.acc(nodes, list(range(num_nodes)))
+    server.acc(nodes, weight_list)
 
     # log
     log(os.path.basename(__file__)[:-3] + '_' + split_para, nodes, server)
 
     return [nodes[i].model for i in range(num_nodes)]
```

### Comparing `fedbase-0.9.4/fedbase/baselines/Local.py` & `fedbase-0.9.5/fedbase/baselines/Ditto.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from fedbase.server.server import server_class
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 import os
 from functools import partial
 
-
-def run(dataset_splited, batch_size, num_nodes, model, objective, optimizer, global_rounds, local_steps, device = torch.device('cuda' if torch.cuda.is_available() else 'cpu'), log_file=True):
+def run(dataset_splited, batch_size, num_nodes, model, objective, optimizer, global_rounds, local_steps, reg, device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
     # dt = data_process(dataset)
     # train_splited, test_splited = dt.split_dataset(num_nodes, split['split_para'], split['split_method'])
     train_splited, test_splited, split_para = dataset_splited
 
     server = server_class(device)
     server.assign_model(model())
 
@@ -31,24 +30,26 @@
         nodes[i].assign_objective(objective())
         # optim
         nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
     
     del train_splited, test_splited
 
     # initialize parameters to nodes
-    server.distribute(nodes, list(range(num_nodes)))
-
+    weight_list = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
+    server.distribute([nodes[i].model for i in range(num_nodes)])
+    
     # train!
     for i in range(global_rounds):
         print('-------------------Global round %d start-------------------' % (i))
         # single-processing!
         for j in range(num_nodes):
-            nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step))
+            nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_fedprox, reg_model = server.model, lam= reg))
             nodes[j].local_test()
+        # server aggregation
+        server.model.load_state_dict(server.aggregate([nodes[i].model for i in range(num_nodes)], weight_list))
         # test accuracy
-        server.acc(nodes, list(range(num_nodes)))
+        server.acc(nodes, weight_list)
 
     # log
-    if log_file:
-        log(os.path.basename(__file__)[:-3] + '_' + split_para, nodes, server)
+    log(os.path.basename(__file__)[:-3] + '_' + str(reg) + '_' + split_para , nodes, server)
 
     return [nodes[i].model for i in range(num_nodes)]
```

### Comparing `fedbase-0.9.4/fedbase/baselines/fedavg_ensemble.py` & `fedbase-0.9.5/fedbase/baselines/fedavg_ensemble.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,29 +30,30 @@
             nodes[i].assign_model(model())
             # objective
             nodes[i].assign_objective(objective())
             # optim
             nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
 
         # initialize parameters to nodes
-        server.distribute(nodes, list(range(num_nodes)))
+        weight_list = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
+        server.distribute([nodes[i].model for i in range(num_nodes)])
 
         # train!
         for i in range(global_rounds):
             print('-------------------Global round %d start-------------------' % (i))
             # single-processing!
             for j in range(num_nodes):
                 nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step))
             # server aggregation and distribution
-            server.aggregate(nodes, list(range(num_nodes)))
-            server.distribute(nodes, list(range(num_nodes)))
+            server.model.load_state_dict(server.aggregate([nodes[i].model for i in range(num_nodes)], weight_list))
+            server.distribute([nodes[i].model for i in range(num_nodes)])
             # test accuracy
             for j in range(num_nodes):
                 nodes[j].local_test()
-            server.acc(nodes, list(range(num_nodes)))
+            server.acc(nodes, weight_list)
 
         # ensemble
         models.append(server.model)
 
     # test ensemble
     print('test ensemble\n')
     for j in range(num_nodes):
```

### Comparing `fedbase-0.9.4/fedbase/baselines/fedprox.py` & `fedbase-0.9.5/fedbase/baselines/fedprox.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,27 +30,28 @@
         nodes[i].assign_objective(objective())
         # optim
         nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
     
     del train_splited, test_splited
 
     # initialize parameters to nodes
-    server.distribute(nodes, list(range(num_nodes)))
-
+    weight_list = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
+    server.distribute([nodes[i].model for i in range(num_nodes)])
+    
     # train!
     for i in range(global_rounds):
         print('-------------------Global round %d start-------------------' % (i))
         # single-processing!
         for j in range(num_nodes):
             nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_fedprox, reg_model = server.model, lam= reg))
         # server aggregation and distribution
-        server.aggregate(nodes, list(range(num_nodes)))
-        server.distribute(nodes, list(range(num_nodes)))
+        server.model.load_state_dict(server.aggregate([nodes[i].model for i in range(num_nodes)], weight_list))
+        server.distribute([nodes[i].model for i in range(num_nodes)])
         # test accuracy
         for j in range(num_nodes):
             nodes[j].local_test()
-        server.acc(nodes, list(range(num_nodes)))
+        server.acc(nodes, weight_list)
 
     # log
     log(os.path.basename(__file__)[:-3] + '_' + str(reg) + '_' + split_para , nodes, server)
 
     return server.model
```

### Comparing `fedbase-0.9.4/fedbase/baselines/fedprox_ensemble.py` & `fedbase-0.9.5/fedbase/baselines/fedprox_ensemble.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,29 +31,30 @@
             nodes[i].assign_model(model())
             # objective
             nodes[i].assign_objective(objective())
             # optim
             nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
 
         # initialize parameters to nodes
-        server.distribute(nodes, list(range(num_nodes)))
+        weight_list = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
+        server.distribute([nodes[i].model for i in range(num_nodes)])
 
         # train!
         for i in range(global_rounds):
             print('-------------------Global round %d start-------------------' % (i))
             # single-processing!
             for j in range(num_nodes):
                 nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_fedprox, reg_model = server.model, lam= reg))
             # server aggregation and distribution
-            server.aggregate(nodes, list(range(num_nodes)))
-            server.distribute(nodes, list(range(num_nodes)))
+            server.model.load_state_dict(server.aggregate([nodes[i].model for i in range(num_nodes)], weight_list))
+            server.distribute([nodes[i].model for i in range(num_nodes)])
             # test accuracy
             for j in range(num_nodes):
                 nodes[j].local_test()
-            server.acc(nodes, list(range(num_nodes)))
+            server.acc(nodes, weight_list)
         
         # ensemble
         models.append(server.model)
 
     # test ensemble
     print('test ensemble\n')
     for j in range(num_nodes):
```

### Comparing `fedbase-0.9.4/fedbase/baselines/fesem.py` & `fedbase-0.9.5/fedbase/baselines/fesem.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.4/fedbase/baselines/fesem_con.py` & `fedbase-0.9.5/fedbase/baselines/fesem_con.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         nodes[i].assign_objective(objective())
         # optim
         nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
     
     del train_splited, test_splited
 
     # initialize parameters to nodes
-    server.distribute(nodes, list(range(num_nodes)))
+    server.distribute([nodes[i].model for i in range(num_nodes)])
 
     # initialize K cluster model
     cluster_models = [model().to(device) for i in range(K)]
 
     # train!
     # b_list = []
     # uu_list = []
@@ -82,16 +82,18 @@
         #     nodes[k].grads = []
         
         # server clustering
         server.weighted_clustering(nodes, list(range(num_nodes)), K, weight_type= 'equal')
 
         # server aggregation and distribution by cluster
         for j in range(K):
-            server.aggregate(nodes, [i for i in list(range(num_nodes)) if nodes[i].label==j])
-            server.distribute(nodes, [i for i in list(range(num_nodes)) if nodes[i].label==j])
+            id_list = [i for i in list(range(num_nodes)) if nodes[i].label==j]
+            server.modelload_state_dict(server.aggregate([nodes[i] for i in id_list], \
+                [nodes[i].data_size/sum([nodes[i].data_size for i in id_list]) for i in id_list]))
+            server.distribute([nodes[i].model for i in id_list])
             cluster_models[j].load_state_dict(server.model.state_dict())
 
         # test accuracy
         for j in range(num_nodes):
             nodes[j].local_test()
         server.acc(nodes, list(range(num_nodes)))
```

### Comparing `fedbase-0.9.4/fedbase/baselines/ifca.py` & `fedbase-0.9.5/fedbase/baselines/ifca.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.4/fedbase/baselines/ifca_con.py` & `fedbase-0.9.5/fedbase/baselines/ifca_con.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.4/fedbase/baselines/ifca_res.py` & `fedbase-0.9.5/fedbase/baselines/ifca_res.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.4/fedbase/baselines/wecfl.py` & `fedbase-0.9.5/fedbase/baselines/wecfl.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.4/fedbase/baselines/wecfl_con.py` & `fedbase-0.9.5/fedbase/baselines/wecfl_con.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from fedbase.utils.data_loader import data_process, log
 from fedbase.utils.visualize import dimension_reduction
+from fedbase.utils.tools import add_
 from fedbase.nodes.node import node
 from fedbase.server.server import server_class
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 from fedbase.model.model import CNNCifar, CNNMnist
 import os
@@ -92,14 +93,11 @@
 
         # test accuracy
         for j in range(num_nodes):
             nodes[j].local_test()
         server.acc(nodes, list(range(num_nodes)))
     
     # log
-    if not reg_lam:
-        log(os.path.basename(__file__)[:-3] + '_' + base + '_'+ str(K)  + '_' + split_para, nodes, server)
-    else:
-        log(os.path.basename(__file__)[:-3] + '_' + base + '_'+ str(K) + '_' + str(reg_lam) + '_' + split_para, nodes, server)
+    log(os.path.basename(__file__)[:-3] + add_(K) + add_(base) + add_(tmp) + add_(mu) + add_(reg_lam) + add_(split_para), nodes, server)
 
     return cluster_models
```

### Comparing `fedbase-0.9.4/fedbase/baselines/wecfl_res.py` & `fedbase-0.9.5/fedbase/baselines/wecfl_res.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.4/fedbase/model/model.py` & `fedbase-0.9.5/fedbase/model/model.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.4/fedbase/model/resnet.py` & `fedbase-0.9.5/fedbase/model/resnet.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.4/fedbase/nodes/node.py` & `fedbase-0.9.5/fedbase/nodes/node.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.4/fedbase/server/server.py` & `fedbase-0.9.5/fedbase/server/server.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.4/fedbase/utils/data_loader.py` & `fedbase-0.9.5/fedbase/utils/data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from torchvision import datasets, transforms
 import numpy as np
 from torch.utils.data import DataLoader, Dataset, random_split, Subset, ChainDataset, ConcatDataset
 import torch
 from torch._utils import _accumulate
 import matplotlib.pyplot as plt
 import matplotlib as mpl
-from fedbase.utils.utils import get_targets
+from fedbase.utils.tools import get_targets
 from fedbase.utils import femnist
 import os
 # import pickle
 import json
 import datetime as d
 import math
 import pandas as pd
```

### Comparing `fedbase-0.9.4/fedbase/utils/femnist.py` & `fedbase-0.9.5/fedbase/utils/femnist.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.4/fedbase/utils/model_utils.py` & `fedbase-0.9.5/fedbase/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.4/fedbase/utils/utils.py` & `fedbase-0.9.5/fedbase/utils/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,8 +41,12 @@
     #         dataset, (datasets.MNIST, datasets.ImageFolder,)
     # ):
     #     return torch.as_tensor(dataset.targets)
     # if isinstance(dataset, datasets.SVHN):
     #     return dataset.labels
 
     # raise NotImplementedError(f"Unknown dataset {dataset}!") 
-# find_files('./log/central*cifar10*')
+# find_files('./log/central*cifar10*')
+
+
+def add_(input_str):
+    return f'_{str(input_str)}' if input_str is not None else ''
```

### Comparing `fedbase-0.9.4/fedbase/utils/visualize.py` & `fedbase-0.9.5/fedbase/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.4/fedbase.egg-info/PKG-INFO` & `fedbase-0.9.5/fedbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedbase
-Version: 0.9.4
+Version: 0.9.5
 Summary: An easy, silly, DIY Federated Learning framework with many baselines for individual researchers.
 Home-page: https://github.com/jie-ma-ai/FedBase
 Author: Jie MA
 Author-email: ustcmj@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedbase-0.9.4/fedbase.egg-info/SOURCES.txt` & `fedbase-0.9.5/fedbase.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,9 +35,9 @@
 fedbase/nodes/node.py
 fedbase/server/__init__.py
 fedbase/server/server.py
 fedbase/utils/__init__.py
 fedbase/utils/data_loader.py
 fedbase/utils/femnist.py
 fedbase/utils/model_utils.py
-fedbase/utils/utils.py
+fedbase/utils/tools.py
 fedbase/utils/visualize.py
```

### Comparing `fedbase-0.9.4/setup.py` & `fedbase-0.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fedbase",
-    version="0.9.4",
+    version="0.9.5",
     author="Jie MA",
     # author_email="ustcmj@gmail.com, jie.ma-5@student.uts.edu.au",
     author_email="ustcmj@gmail.com",
     description="An easy, silly, DIY Federated Learning framework with many baselines for individual researchers.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jie-ma-ai/FedBase",
```

