# Comparing `tmp/xztrainer-0.9.4.tar.gz` & `tmp/xztrainer-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xztrainer-0.9.4.tar", max compression
+gzip compressed data, was "xztrainer-0.9.5.tar", max compression
```

## Comparing `xztrainer-0.9.4.tar` & `xztrainer-0.9.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      894 2023-04-23 16:06:51.334314 xztrainer-0.9.4/pyproject.toml
--rw-r--r--   0        0        0       46 1970-01-01 00:00:00.000000 xztrainer-0.9.4/src/xztrainer/__init__.py
--rw-r--r--   0        0        0      256 2023-03-14 15:54:26.631822 xztrainer-0.9.4/src/xztrainer/functional.py
--rw-r--r--   0        0        0     1414 1970-01-01 00:00:00.000000 xztrainer-0.9.4/src/xztrainer/logger/__init__.py
--rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 xztrainer-0.9.4/src/xztrainer/logger/compose.py
--rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 xztrainer-0.9.4/src/xztrainer/logger/null.py
--rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 xztrainer-0.9.4/src/xztrainer/logger/stream.py
--rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 xztrainer-0.9.4/src/xztrainer/logger/tensorboard.py
--rw-r--r--   0        0        0     1614 2023-04-23 16:06:34.685368 xztrainer-0.9.4/src/xztrainer/model.py
--rw-r--r--   0        0        0      743 2023-03-10 15:49:26.715934 xztrainer-0.9.4/src/xztrainer/rng.py
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 xztrainer-0.9.4/src/xztrainer/sampler.py
--rw-r--r--   0        0        0      409 2023-03-10 15:49:26.707934 xztrainer-0.9.4/src/xztrainer/setup_helper.py
--rw-r--r--   0        0        0    25454 2023-04-23 16:07:28.392193 xztrainer-0.9.4/src/xztrainer/xztrainer.py
--rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 xztrainer-0.9.4/setup.py
--rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 xztrainer-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0      894 2023-04-23 16:11:10.258766 xztrainer-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0       46 1970-01-01 00:00:00.000000 xztrainer-0.9.5/src/xztrainer/__init__.py
+-rw-r--r--   0        0        0      256 2023-03-14 15:54:26.631822 xztrainer-0.9.5/src/xztrainer/functional.py
+-rw-r--r--   0        0        0     1414 1970-01-01 00:00:00.000000 xztrainer-0.9.5/src/xztrainer/logger/__init__.py
+-rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 xztrainer-0.9.5/src/xztrainer/logger/compose.py
+-rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 xztrainer-0.9.5/src/xztrainer/logger/null.py
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 xztrainer-0.9.5/src/xztrainer/logger/stream.py
+-rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 xztrainer-0.9.5/src/xztrainer/logger/tensorboard.py
+-rw-r--r--   0        0        0     1614 2023-04-23 16:06:34.685368 xztrainer-0.9.5/src/xztrainer/model.py
+-rw-r--r--   0        0        0      743 2023-03-10 15:49:26.715934 xztrainer-0.9.5/src/xztrainer/rng.py
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 xztrainer-0.9.5/src/xztrainer/sampler.py
+-rw-r--r--   0        0        0      409 2023-03-10 15:49:26.707934 xztrainer-0.9.5/src/xztrainer/setup_helper.py
+-rw-r--r--   0        0        0    24069 2023-04-23 16:12:03.787658 xztrainer-0.9.5/src/xztrainer/xztrainer.py
+-rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 xztrainer-0.9.5/setup.py
+-rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 xztrainer-0.9.5/PKG-INFO
```

### Comparing `xztrainer-0.9.4/pyproject.toml` & `xztrainer-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xztrainer"
-version = "0.9.4"
+version = "0.9.5"
 description = "A customizable training pipeline for PyTorch"
 authors = ["Maxim Afanasyev <mr.applexz@gmail.com>"]
 license = "MPL-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 tqdm = ">=4.62.3"
```

### Comparing `xztrainer-0.9.4/src/xztrainer/logger/__init__.py` & `xztrainer-0.9.5/src/xztrainer/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.4/src/xztrainer/logger/compose.py` & `xztrainer-0.9.5/src/xztrainer/logger/compose.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.4/src/xztrainer/logger/stream.py` & `xztrainer-0.9.5/src/xztrainer/logger/stream.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.4/src/xztrainer/logger/tensorboard.py` & `xztrainer-0.9.5/src/xztrainer/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.4/src/xztrainer/model.py` & `xztrainer-0.9.5/src/xztrainer/model.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.4/src/xztrainer/rng.py` & `xztrainer-0.9.5/src/xztrainer/rng.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.4/src/xztrainer/sampler.py` & `xztrainer-0.9.5/src/xztrainer/sampler.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.4/src/xztrainer/xztrainer.py` & `xztrainer-0.9.5/src/xztrainer/xztrainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,16 @@
 
 
 @dataclass
 class BaseTrainContext(BaseContext):
     logger: LoggingEngine
     scaler: Optional[GradScaler]
     optimizer: Optimizer
-    optimizer_wrapped: Optimizer
-    model_wrapped: Module
     scheduler: LRSchedulerProtocol
+    model_unwrapped: Module
 
     epoch: int
 
     @property
     def total_batches_in_epoch(self) -> int:
         return self.dataset_batches
 
@@ -137,16 +136,15 @@
             trainer=context.trainer,
             logger=context.logger,
             optimizer=context.optimizer,
             scaler=context.scaler,
             scheduler=context.scheduler,
             data_loader=context.evaluate_data_loader,
             model=context.model,
-            model_wrapped=context.model_wrapped,
-            optimizer_wrapped=context.optimizer_wrapped,
+            model_unwrapped=context.model_unwrapped,
             epoch=context.epoch,
             dataset_batches=context.dataset_batches
         )
 
 
 class InferContext(BaseContext):
     pass
@@ -168,47 +166,26 @@
     @abc.abstractmethod
     def update_metrics(self, model_outputs: Dict[str, List], metrics: Dict[str, Metric]):
         ...
 
     def calculate_composition_metrics(self, metric_values: Dict[str, float]) -> Dict[str, float]:
         return {}
 
-    def log(self, context: BaseTrainContext):
-        pass
-
-    def wrap_model_and_optimizer(self, model: Module, optimizer: Optimizer) -> Tuple[Module, Optimizer]:
-        return model, optimizer
-
-    def on_init_after_load(self, context: TrainContext, step: int):
-        pass
-
-    def on_step_before(self, context: TrainContext, step: int):
-        pass
-
-    def on_update_before(self, context: TrainContext, step: int):
-        pass
-
-    def on_step_after_forward(self, context: TrainContext, step: int):
+    def on_load(self, context: TrainContext, step: int):
         pass
 
-    def on_update_after_forward(self, context: TrainContext, step: int):
-        pass
-
-    def on_step_after_backward(self, context: TrainContext, step: int):
+    def log(self, context: BaseTrainContext):
         pass
 
-    def on_update_after_backward(self, context: TrainContext, step: int):
+    def on_update(self, context: TrainContext, step: int):
         pass
 
-    def on_update_after_optimization(self, context: TrainContext, step: int):
+    def on_pre_update(self, context: TrainContext, step: int):
         pass
 
-    def do_backward(self, context: TrainContext, loss: Tensor):
-        loss.backward()
-
 
 def _metrics_to_state_dict(metrics: Dict[str, Metric]) -> Dict[str, Dict[str, Any]]:
     return {k: v.state_dict() for k, v in metrics.items()}
 
 
 def _load_metrics_from_state_dict(metrics: Dict[str, Metric], state_dict: Dict[str, Dict[str, Any]]):
     for k, v in metrics.items():
@@ -315,43 +292,34 @@
             do_update = context.should_do_update_step(batch_i)
 
             if do_update:
                 context.logger.update_time_step(step)
 
             model_op_ctx = nullcontext() if self.config.amp_dtype is None else autocast(device_type='cuda',
                                                                                         dtype=self.config.amp_dtype)
-            self.trainable.on_step_before(context, step)
-            if do_update:
-                self.trainable.on_update_before(context, step)
-
             with model_op_ctx:
                 loss, model_out = self._forward_pass(context, data)
                 self._update_metrics(loss, model_out, context.metrics_print)
                 self._update_metrics(loss, model_out, context.metrics_train)
 
-            self.trainable.on_step_after_forward(context, step)
             if do_update:
-                self.trainable.on_update_after_forward(context, step)
-
-            if do_update and self.config.log_lr:
                 for group_i, group in enumerate(context.optimizer.param_groups):
                     context.logger.log_scalar(['lr', str(group_i)], group['lr'])
 
             # engine start
             with model_op_ctx:
                 loss = loss / context.get_number_of_accumulations(batch_i)
             if context.scaler is not None:
                 loss = context.scaler.scale(loss)
             # multiple consecutive loss.backward() sum up the gradients, so we need to divide loss by num of accumulations
-            self.trainable.do_backward(context, loss)
-            self.trainable.on_step_after_backward(context, loss)
+            loss.backward()
             if do_update:
                 if context.scaler is not None:
                     context.scaler.unscale_(context.optimizer)
-                self.trainable.on_update_after_backward(context, step)
+                self.trainable.on_pre_update(context, step)
                 l2_grad_norm = torch.norm(
                     torch.stack(
                         [torch.norm(p.grad.detach(), 2.0)
                          for p in context.model.parameters()
                          if p.grad is not None]
                     ),
                     2
@@ -360,22 +328,22 @@
                 max_norm = context.trainer.config.gradient_clipping
                 if max_norm > 0:
                     clip_grad_norm_(context.model.parameters(), max_norm=max_norm)
                 if context.scaler is not None:
                     context.scaler.step(context.optimizer)
                     context.scaler.update()
                 else:
-                    context.optimizer_wrapped.step()
+                    context.optimizer.step()
                 if context.scheduler is not None:
                     context.scheduler.step()
-                context.optimizer_wrapped.zero_grad()
+                context.optimizer.zero_grad()
             # engine end
 
             if do_update:
-                self.trainable.on_update_after_optimization(context, step)
+                self.trainable.on_update(context, step)
 
                 if context.should_perform_step_action(self.config.print_steps, batch_i):
                     self._log_trainable(context, context.metrics_print)
 
                 if context.evaluate_data_loader and context.should_perform_step_action(self.config.eval_steps,
                                                                                        batch_i):
                     self._set_evaluating_state(context)
@@ -457,27 +425,26 @@
     def train(self, train_data: Dataset, eval_data: Dataset, resume_from: int = -1):
         exp_name = self.config.experiment_name
         batches_in_epoch = self._calculate_batches_in_epoch(train_data)
         total_train_steps = self._calculate_total_steps(train_data)
 
 
         # Initialize and wrap model, optimizer and scheduler
-        model = self.model
-        optim = self.config.optimizer(model)
-        model_wrap, optim_wrap = self.trainable.wrap_model_and_optimizer(model, optim)
+        optim = self.config.optimizer(self.model)
         if self.config.amp_dtype is not None:
             scaler = GradScaler()
         else:
             scaler = None
         if self.config.scheduler and self.config.scheduler_type:
             scheduler = self.config.scheduler(optim, total_train_steps)
             scheduler_type = self.config.scheduler_type
         else:
             scheduler = None
             scheduler_type = None
+        model = self.model
 
         metrics_print = self._create_metrics()
         metrics_train = self._create_metrics()
         metrics_eval = self._create_metrics()
 
         # Load the state
         state = self._load(resume_from)
@@ -535,33 +502,32 @@
                         batch_size=self.config.batch_size,
                         sampler=train_sampler
                     )
                     context = TrainContext(
                             trainer=self,
                             logger=logger,
                             optimizer=optim,
-                            optimizer_wrapped=optim_wrap,
                             scaler=scaler,
                             scheduler=_scheduler,
                             data_loader=train_dl,
                             sampler=train_sampler,
                             model=model,
-                            model_wrapped=model_wrap,
+                            model_unwrapped=self.model,
                             epoch=epoch,
                             total_steps=total_train_steps,
                             evaluate_data_loader=eval_dl,
                             dataset_batches=batches_in_epoch,
                             shift_batch_i=shift_batch_i,
                             progress_bar=progress_bar,
                             metrics_print=metrics_print,
                             metrics_train=metrics_train,
                             metrics_evaluate=metrics_eval
                         )
                     if epoch == start_from_epoch:
-                        self.trainable.on_init_after_load(context, context.get_step_from_batch(context.get_actual_batch_i(0)))
+                        self.trainable.on_load(context, context.get_step_from_batch(context.get_actual_batch_i(0)))
                     self._train_epoch(context)
 
                     if scheduler_type == SchedulerType.EPOCH:
                         scheduler.step()
         return exp_name
 
     def load_last_checkpoint(self):
```

### Comparing `xztrainer-0.9.4/setup.py` & `xztrainer-0.9.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 extras_require = \
 {'numpy': ['numpy>=1.24.2'],
  'tensorboard': ['tensorboard>=2.8.0'],
  'torch': ['torch>=1.10.0']}
 
 setup_kwargs = {
     'name': 'xztrainer',
-    'version': '0.9.4',
+    'version': '0.9.5',
     'description': 'A customizable training pipeline for PyTorch',
     'long_description': 'None',
     'author': 'Maxim Afanasyev',
     'author_email': 'mr.applexz@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `xztrainer-0.9.4/PKG-INFO` & `xztrainer-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xztrainer
-Version: 0.9.4
+Version: 0.9.5
 Summary: A customizable training pipeline for PyTorch
 License: MPL-2.0
 Author: Maxim Afanasyev
 Author-email: mr.applexz@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

