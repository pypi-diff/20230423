# Comparing `tmp/taichu-serve-2.0.18.tar.gz` & `tmp/taichu-serve-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-serve-2.0.18.tar", last modified: Sun Apr 23 01:47:26 2023, max compression
+gzip compressed data, was "taichu-serve-2.0.9.tar", last modified: Wed Apr 19 02:34:49 2023, max compression
```

## Comparing `taichu-serve-2.0.18.tar` & `taichu-serve-2.0.9.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-23 01:47:26.547162 taichu-serve-2.0.18/
--rw-r--r--   0 chen       (501) staff       (20)      236 2023-04-23 01:47:26.547005 taichu-serve-2.0.18/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)     6754 2023-04-21 10:57:51.000000 taichu-serve-2.0.18/README.md
--rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-23 01:47:26.547211 taichu-serve-2.0.18/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)     1065 2023-04-23 01:47:22.000000 taichu-serve-2.0.18/setup.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-23 01:47:26.544486 taichu-serve-2.0.18/taichu_serve/
--rw-r--r--   0 chen       (501) staff       (20)     3738 2023-04-21 07:11:30.000000 taichu-serve-2.0.18/taichu_serve/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     9573 2023-04-21 07:11:30.000000 taichu-serve-2.0.18/taichu_serve/app.py
--rw-r--r--   0 chen       (501) staff       (20)     8284 2023-04-21 09:53:18.000000 taichu-serve-2.0.18/taichu_serve/command.py
--rw-r--r--   0 chen       (501) staff       (20)      934 2023-04-18 09:03:28.000000 taichu-serve-2.0.18/taichu_serve/common.py
--rw-r--r--   0 chen       (501) staff       (20)     4181 2023-04-23 01:45:05.000000 taichu-serve-2.0.18/taichu_serve/dockerfile.py
--rw-r--r--   0 chen       (501) staff       (20)     1521 2023-04-14 04:52:00.000000 taichu-serve-2.0.18/taichu_serve/error_code.py
--rw-r--r--   0 chen       (501) staff       (20)     6336 2023-04-12 06:27:59.000000 taichu-serve-2.0.18/taichu_serve/grpc_predict_v2_pb2.py
--rw-r--r--   0 chen       (501) staff       (20)    13010 2023-04-13 09:06:46.000000 taichu-serve-2.0.18/taichu_serve/grpc_predict_v2_pb2_grpc.py
--rw-r--r--   0 chen       (501) staff       (20)     5042 2023-04-19 06:55:46.000000 taichu-serve-2.0.18/taichu_serve/grpc_server.py
--rw-r--r--   0 chen       (501) staff       (20)     2274 2023-04-21 09:59:46.000000 taichu-serve-2.0.18/taichu_serve/log.py
--rw-r--r--   0 chen       (501) staff       (20)     5471 2023-04-21 06:11:44.000000 taichu-serve-2.0.18/taichu_serve/model_server.py
--rw-r--r--   0 chen       (501) staff       (20)      205 2023-04-13 09:06:46.000000 taichu-serve-2.0.18/taichu_serve/ratelimiter.py
--rw-r--r--   0 chen       (501) staff       (20)     3167 2023-04-21 10:57:51.000000 taichu-serve-2.0.18/taichu_serve/settings.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-23 01:47:26.545733 taichu-serve-2.0.18/taichu_serve/template/
--rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.18/taichu_serve/template/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)      833 2023-04-21 07:11:30.000000 taichu-serve-2.0.18/taichu_serve/template/model_service.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-23 01:47:26.546689 taichu-serve-2.0.18/taichu_serve/template/test/
--rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.18/taichu_serve/template/test/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)      691 2023-04-20 09:26:47.000000 taichu-serve-2.0.18/taichu_serve/template/test/grpc_client.py
--rw-r--r--   0 chen       (501) staff       (20)      286 2023-04-20 09:26:47.000000 taichu-serve-2.0.18/taichu_serve/template/test/http_client.py
--rw-r--r--   0 chen       (501) staff       (20)      932 2023-04-20 09:26:47.000000 taichu-serve-2.0.18/taichu_serve/template/test/stream_grpc_client.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-23 01:47:26.545454 taichu-serve-2.0.18/taichu_serve.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)      236 2023-04-23 01:47:26.000000 taichu-serve-2.0.18/taichu_serve.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      834 2023-04-23 01:47:26.000000 taichu-serve-2.0.18/taichu_serve.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-23 01:47:26.000000 taichu-serve-2.0.18/taichu_serve.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-23 01:47:26.000000 taichu-serve-2.0.18/taichu_serve.egg-info/entry_points.txt
--rw-r--r--   0 chen       (501) staff       (20)       53 2023-04-23 01:47:26.000000 taichu-serve-2.0.18/taichu_serve.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-23 01:47:26.000000 taichu-serve-2.0.18/taichu_serve.egg-info/top_level.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.797402 taichu-serve-2.0.9/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-19 02:34:49.797253 taichu-serve-2.0.9/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-19 02:34:49.797443 taichu-serve-2.0.9/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      947 2023-04-19 02:34:18.000000 taichu-serve-2.0.9/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.793674 taichu-serve-2.0.9/taichu_serve/
+-rw-r--r--   0 chen       (501) staff       (20)     3398 2023-04-14 02:56:12.000000 taichu-serve-2.0.9/taichu_serve/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     9214 2023-04-14 05:19:23.000000 taichu-serve-2.0.9/taichu_serve/app.py
+-rw-r--r--   0 chen       (501) staff       (20)     5479 2023-04-19 02:05:09.000000 taichu-serve-2.0.9/taichu_serve/command.py
+-rw-r--r--   0 chen       (501) staff       (20)      934 2023-04-18 09:03:28.000000 taichu-serve-2.0.9/taichu_serve/common.py
+-rw-r--r--   0 chen       (501) staff       (20)     2118 2023-04-19 02:34:18.000000 taichu-serve-2.0.9/taichu_serve/dockerfile.py
+-rw-r--r--   0 chen       (501) staff       (20)     1521 2023-04-14 04:52:00.000000 taichu-serve-2.0.9/taichu_serve/error_code.py
+-rw-r--r--   0 chen       (501) staff       (20)     6336 2023-04-12 06:27:59.000000 taichu-serve-2.0.9/taichu_serve/grpc_predict_v2_pb2.py
+-rw-r--r--   0 chen       (501) staff       (20)    13010 2023-04-13 09:06:46.000000 taichu-serve-2.0.9/taichu_serve/grpc_predict_v2_pb2_grpc.py
+-rw-r--r--   0 chen       (501) staff       (20)     4697 2023-04-17 04:31:53.000000 taichu-serve-2.0.9/taichu_serve/grpc_server.py
+-rw-r--r--   0 chen       (501) staff       (20)     2104 2023-04-14 09:24:14.000000 taichu-serve-2.0.9/taichu_serve/log.py
+-rw-r--r--   0 chen       (501) staff       (20)     5444 2023-04-14 01:39:52.000000 taichu-serve-2.0.9/taichu_serve/model_server.py
+-rw-r--r--   0 chen       (501) staff       (20)      205 2023-04-13 09:06:46.000000 taichu-serve-2.0.9/taichu_serve/ratelimiter.py
+-rw-r--r--   0 chen       (501) staff       (20)     2253 2023-04-19 01:27:54.000000 taichu-serve-2.0.9/taichu_serve/settings.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.795889 taichu-serve-2.0.9/taichu_serve/template/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.9/taichu_serve/template/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      123 2023-04-18 08:48:18.000000 taichu-serve-2.0.9/taichu_serve/template/config.ini
+-rw-r--r--   0 chen       (501) staff       (20)      741 2023-04-18 03:02:30.000000 taichu-serve-2.0.9/taichu_serve/template/customize_service.py
+-rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-18 03:02:30.000000 taichu-serve-2.0.9/taichu_serve/template/requirements.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.796946 taichu-serve-2.0.9/taichu_serve/template/test/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.9/taichu_serve/template/test/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      690 2023-04-18 08:48:18.000000 taichu-serve-2.0.9/taichu_serve/template/test/grpc_client.py
+-rw-r--r--   0 chen       (501) staff       (20)      285 2023-04-18 08:45:26.000000 taichu-serve-2.0.9/taichu_serve/template/test/http_client.py
+-rw-r--r--   0 chen       (501) staff       (20)      931 2023-04-18 08:48:18.000000 taichu-serve-2.0.9/taichu_serve/template/test/stream_grpc_client.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.794937 taichu-serve-2.0.9/taichu_serve.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      900 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/entry_points.txt
+-rw-r--r--   0 chen       (501) staff       (20)       53 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/top_level.txt
```

### Comparing `taichu-serve-2.0.18/setup.py` & `taichu-serve-2.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,23 +8,19 @@
 
 if __name__ == '__main__':
     name = 'taichu-serve'
 
     requirements = ['grpcio', 'grpcio-tools', 'protobuf',
                     'Flask', 'gunicorn', 'requests']
 
-    long_description = ''
-    # with open('README.md', 'r') as f:
-    #     long_description = f.read()
-
     setup(
         name=name,
-        version='2.0.18',
+        version='2.0.9',
         description='taichu serve is a tool for serving deep learning inference',
-        long_description=long_description,
+        # long_description='',
         author='taichu platform team',
         # author_email='noreply@noreply.com',
         python_requires=">=3.6.0",
         url='',
         keywords='Serving Deep Learning Inference AI',
         packages=pkgs,
         install_requires=requirements,
```

### Comparing `taichu-serve-2.0.18/taichu_serve/__init__.py` & `taichu-serve-2.0.9/taichu_serve/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,42 +5,45 @@
 
 from abc import ABCMeta, abstractmethod
 from taichu_serve.model_server import BaseModelService
 
 logger = logging.getLogger(__name__)
 
 
-class ModelServer(BaseModelService):
+class Service(BaseModelService):
     '''SingleNodeModel defines abstraction for model service which loads a
     single model.
     '''
 
     def __init__(self, model_path):
-        super(ModelServer, self).__init__(model_path)
+        super(Service, self).__init__(model_path)
         self._ready = False
-        self._ctx = {}
 
     def warmup(self):
         start_time = time.time()
         self._warmup()
         self._ready = True
         logger.info('warmup time: ' + str((time.time() - start_time) * 1000) + 'ms')
 
-    def inference(self, data, request_id, stream=False):
-        """
+    def inference(self, data, request_id):
+        '''
         Wrapper function to run preprocess, inference and postprocess functions.
-        """
-        logger.info('recv request: ' + request_id)
 
-        context = self._ctx.get(request_id)
-        if context is None:
-            context = {}
-            if stream:
-                logger.info('create context for request: ' + request_id)
-                self._ctx[request_id] = context
+        Parameters
+        ----------
+        data : map of object
+            Raw input from request.
+
+        Returns
+        -------
+        list of outputs to be sent back to client.
+            data to be sent back
+        '''
+        logger.info('recv request: ' + request_id)
+        context = {}
 
         pre_start_time = time.time()
         data = self._preprocess(data, context=context)
         infer_start_time = time.time()
 
         # Update preprocess latency metric
         pre_time_in_ms = (infer_start_time - pre_start_time) * 1000
@@ -110,27 +113,18 @@
         Returns
         -------
         list of object
             list of outputs to be sent back.
         '''
         return data
 
-    def destroy_context(self, request_id):
-        logger.info('destroy context for request: ' + request_id)
-        if request_id in self._ctx:
-            del self._ctx[request_id]
-
     @abstractmethod
     def _warmup(self):
         pass
 
     @property
     def model_version(self):
         return '1'
 
     @property
     def ready(self):
         return self._ready
-
-    def run(self, *args, **kwargs):
-        from taichu_serve.command import cli
-        cli(*args, **kwargs)
```

### Comparing `taichu-serve-2.0.18/taichu_serve/app.py` & `taichu-serve-2.0.9/taichu_serve/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 DL webservice app
 """
+import ctypes
 import inspect
 import json
 import logging
 import os
 import threading
 import time
 import traceback
@@ -13,31 +14,28 @@
 
 from flask import Flask, request, g
 
 from taichu_serve.log import init_logger
 from taichu_serve.settings import parse_args
 from taichu_serve.ratelimiter import semaphore
 
-args = parse_args()
-if args.env == "prod":
-    init_logger(json_format=True)
-else:
-    init_logger()
-
+init_logger()
 
-app = Flask("app")
+app = Flask("aa")
 
 from taichu_serve.error_code import ModelNotFoundError, ModelPredictError, TooManyRequestsError
-from taichu_serve import ModelServer
+from taichu_serve import Service
 from taichu_serve.common import Local
 
 LOGGER = logging.getLogger(__name__)
 
 import multiprocessing
 
+args = parse_args()
+
 workers_status = []
 
 
 class WorkersPipeMgr(object):
     def __init__(self, num):
         self._list = []
         self._occupied = []
@@ -88,25 +86,29 @@
     model_service_file = args.service_file
 
     print(
         "model_path={} \n model_service_file={} "
         .format(model_path, model_service_file))
 
     module = load_service(os.path.join(model_path, model_service_file)
-                          ) if model_service_file else ModelServer
+                          ) if model_service_file else Service
     classes = [cls[1] for cls in inspect.getmembers(module, inspect.isclass)]
 
-    assert len(classes) > 0, "There should be one user defined service derived from ModelServer."
+    assert len(classes) > 0, "There should be one user defined service derived from ModelService."
 
     class_defs = list(
         filter(
-            lambda c: issubclass(c, ModelServer) and len(
+            lambda c: issubclass(c, Service) and len(
                 c.__subclasses__()) == 0, classes))
 
-    assert len(class_defs) > 0, "There should be one user defined service derived from ModelServer."
+    # if len(class_defs) != 1:
+    #     raise Exception(
+    #         'There should be one user defined service derived from ModelService.'
+    #     )
+    assert len(class_defs) > 0, "There should be one user defined service derived from ModelService."
 
     for c in class_defs:
         LOGGER.info("class_defs: %s", c.__name__)
         instance = c(model_path)
         # threading.Thread(target=instance.warmup).start()
         instance.warmup()
         dict_model_service[f'{str(c.__name__).lower()}_{instance.model_version.lower()}'] = instance
@@ -127,48 +129,36 @@
             if ins is None:
                 ret = {
                     'data': None,
                     'status': 'error',
                     'error': 'model not found',
                 }
             else:
-                method = data.get('method', None)
-                if method == 'destroy_context':
-                    ins.destroy_context(request_id)
-
-                    ret = {'status': 'ok'}
-                    continue
-
-                stream = data.get('stream', False)
                 ret = {
-                    'data': ins.inference(data.get('data'), request_id, stream=stream),
+                    'data': ins.inference(data.get('data'), request_id),
                     'status': 'ok',
                 }
         except Exception as e:
             LOGGER.error(traceback.format_exc())
             ret = {
                 'data': None,
                 'status': 'error',
                 'error': str(e),
             }
-        finally:
-            pipe.send(ret)
+        pipe.send(ret)
+
+    # return dict_model_service
 
 
-def model_inference(model_name, model_version, data, request_id, method=None):
+def model_inference(model_name, model_version, data, request_id):
     try:
         p = workers_pipe.acquire(request_id)
         if p is None:
             raise TooManyRequestsError()
-        payload = {'model_name': model_name, 'model_version': model_version, 'data': data, 'request_id': request_id}
-        if method:
-            payload['method'] = method
-        if method == 'stream_infer':
-            payload['stream'] = True
-        p.send(payload)
+        p.send({'model_name': model_name, 'model_version': model_version, 'data': data, 'request_id': request_id})
         ret = p.recv()
 
         if ret.get('status') == 'error':
             raise ModelPredictError(message=ret.get('error'))
         return ret.get('data')
     finally:
         if p is not None:
```

### Comparing `taichu-serve-2.0.18/taichu_serve/common.py` & `taichu-serve-2.0.9/taichu_serve/common.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.18/taichu_serve/dockerfile.py` & `taichu-serve-2.0.9/taichu_serve/dockerfile.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,40 +6,36 @@
 
 USER root
 
 WORKDIR /opt
 COPY ./launch.sh /opt/launch.sh
 COPY ./requirements.txt /opt/requirements.txt
 
-RUN chmod -R 777 /opt/launch.sh && chmod -R 777 /opt/requirements.txt
+RUN chmod -R 777 /opt
 RUN chmod -R 777 /home
 
 # 安装apt依赖
 {apt_install}
 
-RUN pip3 install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple --force-reinstall
+RUN pip3 install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple
 
 WORKDIR /home
 
 ENTRYPOINT ["/bin/bash", "-c"]
 CMD ["/opt/launch.sh"]
 
 # 构建镜像命令： docker build -t taichu-serve-env .
 # 运行镜像命令： docker run -it  -v $PWD:/home taichu-serve-env bash
-# 推送镜像命令： 
-#               docker tag taichu-serve-env swr.cn-central-221.ovaijisuan.com/wair/taichu-serve-env
-#               docker push swr.cn-central-221.ovaijisuan.com/wair/taichu-serve-env
 """
 
 launch_sh_template = """#!/bin/bash
 # 请不要修改这个文件
 # Do Not Modify This File
-set +e
 
-default_triton_grpc_port=8001
+default_triton_grpc_port=50000
 default_grpc_port=8080
 default_http_port=8081
 
 
 if [ -z $triton_grpc_port ];then
     triton_grpc_port=$default_triton_grpc_port
 fi
@@ -53,20 +49,17 @@
 
 if [ -z $MODEL_PACKAGE_PATH ];then
   echo "[FATAL] env MODEL_PACKAGE_PATH is not set"
   sleep 5
   exit 1
 fi
 
-# 生成临时的随机目录
-random_dir=$(cat /dev/urandom | tr -dc 'a-zA-Z0-9' | fold -w 8 | head -n 1)
-mkdir ~/$random_dir
-cd ~/$random_dir
-time cp -rf $MODEL_PACKAGE_PATH/* .
+# /mnt/publish-data/admin/taichuserver/project
 
+cd $MODEL_PACKAGE_PATH
 
 # 检查是否存在models目录
 if [ -d "models" ]; then
   echo "start tritonserver"
   # 启动tritonserver
   nohup tritonserver --model-repository=./models  --grpc-port=$triton_grpc_port  > tritonserver.log 2>&1 &
 
@@ -97,84 +90,9 @@
     fi
     rows=`echo $rows | sed 's/^[ \t]*//g' | sed 's/[ \t]*$//g'`
     echo "install $rows"
     apt-get install -y $rows
   done
 fi
 
-taichu_serve run  --env prod --grpc_port $grpc_port --http_port $http_port
-"""
-
-
-Dockerfile_deploy_template = """
-FROM {base_image}
-
-
-USER root
-
-WORKDIR /opt
-COPY ./launch.sh /opt/launch.sh
-COPY ./requirements.txt /opt/requirements.txt
-
-RUN chmod -R 777 /opt/launch.sh && chmod -R 777 /opt/requirements.txt
-
-# 安装apt依赖
-{apt_install}
-
-RUN pip3 install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple --force-reinstall
-
-WORKDIR /home
-RUN mkdir -p /home/project
-
-WORKDIR /home/project
-COPY . .
-RUN chmod -R 777 /home
-
-ENTRYPOINT ["/bin/bash", "-c"]
-CMD ["/opt/launch.sh"]
-
-# 构建镜像命令： docker build -t taichu-serve-env .
-# 运行镜像命令： docker run -it  -v $PWD:/home taichu-serve-env bash
-# 推送镜像命令： 
-#               docker tag taichu-serve-env swr.cn-central-221.ovaijisuan.com/wair/taichu-serve-env
-#               docker push swr.cn-central-221.ovaijisuan.com/wair/taichu-serve-env
-"""
-
-launch_sh_deploy_template = """#!/bin/bash
-# 请不要修改这个文件
-# Do Not Modify This File
-set +e
-
-default_triton_grpc_port=8001
-default_grpc_port=8080
-default_http_port=8081
-
-
-if [ -z $triton_grpc_port ];then
-    triton_grpc_port=$default_triton_grpc_port
-fi
-if [ -z $grpc_port ];then
-    grpc_port=$default_grpc_port
-fi
-if [ -z $http_port ];then
-    http_port=$default_http_port
-fi
-
-cd /home/project
-
-# 检查是否存在models目录
-if [ -d "models" ]; then
-  echo "start tritonserver"
-  set -e
-  
-  # 启动tritonserver
-  nohup tritonserver --model-repository=./models  --grpc-port=$triton_grpc_port  > tritonserver.log 2>&1 &
-
-  # 等待tritonserver启动
-  sleep 10
-  cat tritonserver.log
-  
-  set +e
-fi
-
-taichu_serve run  --env prod --grpc_port $grpc_port --http_port $http_port
+taichu_serve run --grpc_port $grpc_port --http_port $http_port
 """
```

### Comparing `taichu-serve-2.0.18/taichu_serve/error_code.py` & `taichu-serve-2.0.9/taichu_serve/error_code.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.18/taichu_serve/grpc_predict_v2_pb2.py` & `taichu-serve-2.0.9/taichu_serve/grpc_predict_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.18/taichu_serve/grpc_predict_v2_pb2_grpc.py` & `taichu-serve-2.0.9/taichu_serve/grpc_predict_v2_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.18/taichu_serve/grpc_server.py` & `taichu-serve-2.0.9/taichu_serve/grpc_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,40 +74,36 @@
 
         return resp
 
     @grpc_interceptor
     def ModelStreamInfer(self, request, context):
         # 检测是否有客户端断开连接
         request_id = str(uuid.uuid4())
-        try:
-            while context.is_active():
-                for req in request:
-                    logger.info('recv a request')
-                    if req.id and len(req.id) > 0:
-                        request_id = req.id
-
-                    rec_dict = parameters_to_dict(req.parameters)
-                    try:
-                        res = model_inference(req.model_name, req.model_version,
-                                              rec_dict, request_id, method='stream_infer')
-                    except Exception as e:
-                        logger.error('Algorithm crashed!, %s', str(e))
-                        logger.error(traceback.format_exc())
-                        raise ModelPredictError(message=str(e))
-
-                    resp = self.make_response(res)
-                    resp.model_name = req.model_name
-                    resp.model_version = req.model_version
-                    resp.id = request_id
-
-                    yield resp
-        finally:
-            logger.info('client disconnected')
-            model_inference(req.model_name, req.model_version,
-                            {}, request_id, method='destroy_context')
+
+        while context.is_active():
+            for req in request:
+                logger.info('recv a request')
+                if req.id and len(req.id) > 0:
+                    request_id = req.id
+
+                rec_dict = parameters_to_dict(req.parameters)
+                try:
+                    res = model_inference(req.model_name, req.model_version, rec_dict, request_id)
+                except Exception as e:
+                    logger.error('Algorithm crashed!, %s', str(e))
+                    logger.error(traceback.format_exc())
+                    raise ModelPredictError(message=str(e))
+
+
+                resp = self.make_response(res)
+                resp.model_name = req.model_name
+                resp.model_version = req.model_version
+                resp.id = request_id
+
+                yield resp
 
     def ServerLive(self, request, context):
         resp = grpc_predict_v2_pb2.ServerLiveResponse(
             live=True,
         )
         return resp
```

### Comparing `taichu-serve-2.0.18/taichu_serve/log.py` & `taichu-serve-2.0.9/taichu_serve/log.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,17 +53,14 @@
         for (k, v) in record.__dict__.items():
             if k not in exclude_fields:
                 data[k] = v
 
         return json.dumps(data, ensure_ascii=False)
 
 
-def init_logger(json_format: bool = False):
+def init_logger():
     logging.basicConfig(level=logging.INFO)
     logger = logging.getLogger()
     logger.handlers = []
     consoleHandler = logging.StreamHandler(stream=sys.stdout)
-    if json_format:
-        consoleHandler.setFormatter(JsonFormatter(datefmt='%Y-%m-%d %H:%M:%S'))
-    else:
-        consoleHandler.setFormatter(logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s'))
+    consoleHandler.setFormatter(JsonFormatter(datefmt='%Y-%m-%d %H:%M:%S'))
     logger.addHandler(consoleHandler)
```

### Comparing `taichu-serve-2.0.18/taichu_serve/model_server.py` & `taichu-serve-2.0.9/taichu_serve/model_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
     '''ModelService wraps up all preprocessing, inference and postprocessing
     functions used by model service. It is defined in a flexible manner to
     be easily extended to support different frameworks.
     '''
     __metaclass__ = ABCMeta
 
     def __init__(self, model_path):
-        self.model_path = model_path
+        self.ctx = None
 
     @abstractmethod
-    def inference(self, data, request_id, stream=False):
+    def inference(self, data, request_id):
         '''
         Wrapper function to run preprocess, inference and postprocess functions.
 
         Parameters
         ----------
         data : map of object
             Raw input from request.
```

### Comparing `taichu-serve-2.0.18/taichu_serve/template/test/grpc_client.py` & `taichu-serve-2.0.9/taichu_serve/template/test/grpc_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import grpc
 import taichu_serve.grpc_predict_v2_pb2 as grpc_predict_v2_pb2
 import taichu_serve.grpc_predict_v2_pb2_grpc as grpc_predict_v2_pb2_grpc
 
-model_name = "ModelService"
+model_name = "TestService"
 
 
 def run():
     conn = grpc.insecure_channel('localhost:8080')
     client = grpc_predict_v2_pb2_grpc.GRPCInferenceServiceStub(channel=conn)
 
     req = grpc_predict_v2_pb2.ModelInferRequest()
```

### Comparing `taichu-serve-2.0.18/taichu_serve/template/test/stream_grpc_client.py` & `taichu-serve-2.0.9/taichu_serve/template/test/stream_grpc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 import grpc
 import taichu_serve.grpc_predict_v2_pb2 as grpc_predict_v2_pb2
 import taichu_serve.grpc_predict_v2_pb2_grpc as grpc_predict_v2_pb2_grpc
 
-model_name = "ModelService"
+model_name = "TestService"
 
 
 def guide_list_features(stub):
     num = 5
 
     while True:
```

### Comparing `taichu-serve-2.0.18/taichu_serve.egg-info/SOURCES.txt` & `taichu-serve-2.0.9/taichu_serve.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-README.md
 setup.py
 taichu_serve/__init__.py
 taichu_serve/app.py
 taichu_serve/command.py
 taichu_serve/common.py
 taichu_serve/dockerfile.py
 taichu_serve/error_code.py
@@ -16,12 +15,14 @@
 taichu_serve.egg-info/PKG-INFO
 taichu_serve.egg-info/SOURCES.txt
 taichu_serve.egg-info/dependency_links.txt
 taichu_serve.egg-info/entry_points.txt
 taichu_serve.egg-info/requires.txt
 taichu_serve.egg-info/top_level.txt
 taichu_serve/template/__init__.py
-taichu_serve/template/model_service.py
+taichu_serve/template/config.ini
+taichu_serve/template/customize_service.py
+taichu_serve/template/requirements.txt
 taichu_serve/template/test/__init__.py
 taichu_serve/template/test/grpc_client.py
 taichu_serve/template/test/http_client.py
 taichu_serve/template/test/stream_grpc_client.py
```

