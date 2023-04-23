# Comparing `tmp/Scrapy-Distributed-2020.12.1.tar.gz` & `tmp/Scrapy-Distributed-2023.4.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scrapy-Distributed-2020.12.1.tar", last modified: Sat Feb 20 14:04:31 2021, max compression
+gzip compressed data, was "Scrapy-Distributed-2023.4.23.tar", last modified: Sun Apr 23 05:20:18 2023, max compression
```

## Comparing `Scrapy-Distributed-2020.12.1.tar` & `Scrapy-Distributed-2023.4.23.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-20 14:04:31.038767 Scrapy-Distributed-2020.12.1/
--rw-r--r--   0 runner    (1001) docker     (116)       33 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     7903 2021-02-20 14:04:31.038767 Scrapy-Distributed-2020.12.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5144 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-20 14:04:31.034767 Scrapy-Distributed-2020.12.1/Scrapy_Distributed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7903 2021-02-20 14:04:30.000000 Scrapy-Distributed-2020.12.1/Scrapy_Distributed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1432 2021-02-20 14:04:30.000000 Scrapy-Distributed-2020.12.1/Scrapy_Distributed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-20 14:04:30.000000 Scrapy-Distributed-2020.12.1/Scrapy_Distributed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-20 14:04:30.000000 Scrapy-Distributed-2020.12.1/Scrapy_Distributed.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       77 2021-02-20 14:04:30.000000 Scrapy-Distributed-2020.12.1/Scrapy_Distributed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       19 2021-02-20 14:04:30.000000 Scrapy-Distributed-2020.12.1/Scrapy_Distributed.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       76 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/requirements-install.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-20 14:04:31.034767 Scrapy-Distributed-2020.12.1/scrapy_distributed/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-20 14:04:31.034767 Scrapy-Distributed-2020.12.1/scrapy_distributed/amqp_utils/
--rw-r--r--   0 runner    (1001) docker     (116)       84 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/amqp_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      791 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/amqp_utils/connection.py
--rw-r--r--   0 runner    (1001) docker     (116)      314 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/amqp_utils/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-20 14:04:31.034767 Scrapy-Distributed-2020.12.1/scrapy_distributed/common/
--rw-r--r--   0 runner    (1001) docker     (116)       74 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      839 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/common/queue_config.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-20 14:04:31.034767 Scrapy-Distributed-2020.12.1/scrapy_distributed/dupefilters/
--rw-r--r--   0 runner    (1001) docker     (116)       73 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/dupefilters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5319 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/dupefilters/redis_bloom.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-20 14:04:31.038767 Scrapy-Distributed-2020.12.1/scrapy_distributed/middlewares/
--rw-r--r--   0 runner    (1001) docker     (116)       85 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3731 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/middlewares/amqp.py
--rw-r--r--   0 runner    (1001) docker     (116)      231 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/middlewares/common.py
--rw-r--r--   0 runner    (1001) docker     (116)     2487 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/middlewares/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-20 14:04:31.038767 Scrapy-Distributed-2020.12.1/scrapy_distributed/pipelines/
--rw-r--r--   0 runner    (1001) docker     (116)       75 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2289 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/pipelines/amqp.py
--rw-r--r--   0 runner    (1001) docker     (116)     2704 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/pipelines/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-20 14:04:31.038767 Scrapy-Distributed-2020.12.1/scrapy_distributed/queues/
--rw-r--r--   0 runner    (1001) docker     (116)      520 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6574 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/queues/amqp.py
--rw-r--r--   0 runner    (1001) docker     (116)      733 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/queues/common.py
--rw-r--r--   0 runner    (1001) docker     (116)     6379 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/queues/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-20 14:04:31.038767 Scrapy-Distributed-2020.12.1/scrapy_distributed/redis_utils/
--rw-r--r--   0 runner    (1001) docker     (116)       46 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/redis_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2382 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/redis_utils/connection.py
--rw-r--r--   0 runner    (1001) docker     (116)      441 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/redis_utils/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-20 14:04:31.038767 Scrapy-Distributed-2020.12.1/scrapy_distributed/schedulers/
--rw-r--r--   0 runner    (1001) docker     (116)      601 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6110 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/schedulers/common.py
--rw-r--r--   0 runner    (1001) docker     (116)      371 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/schedulers/redis_bloom.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-20 14:04:31.038767 Scrapy-Distributed-2020.12.1/scrapy_distributed/spiders/
--rw-r--r--   0 runner    (1001) docker     (116)       84 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/spiders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1126 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/spiders/redis_bloom.py
--rw-r--r--   0 runner    (1001) docker     (116)     3429 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/scrapy_distributed/spiders/sitemap.py
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-02-20 14:04:31.038767 Scrapy-Distributed-2020.12.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2147 2021-02-20 14:04:21.000000 Scrapy-Distributed-2020.12.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:20:18.123217 Scrapy-Distributed-2023.4.23/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-23 05:20:18.123217 Scrapy-Distributed-2023.4.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:20:18.119217 Scrapy-Distributed-2023.4.23/Scrapy_Distributed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-23 05:20:18.000000 Scrapy-Distributed-2023.4.23/Scrapy_Distributed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-23 05:20:18.000000 Scrapy-Distributed-2023.4.23/Scrapy_Distributed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 05:20:18.000000 Scrapy-Distributed-2023.4.23/Scrapy_Distributed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 05:20:18.000000 Scrapy-Distributed-2023.4.23/Scrapy_Distributed.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 05:20:18.000000 Scrapy-Distributed-2023.4.23/Scrapy_Distributed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-23 05:20:18.000000 Scrapy-Distributed-2023.4.23/Scrapy_Distributed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/requirements-install.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:20:18.119217 Scrapy-Distributed-2023.4.23/scrapy_distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:20:18.119217 Scrapy-Distributed-2023.4.23/scrapy_distributed/amqp_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/amqp_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/amqp_utils/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/amqp_utils/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:20:18.119217 Scrapy-Distributed-2023.4.23/scrapy_distributed/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/common/queue_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:20:18.119217 Scrapy-Distributed-2023.4.23/scrapy_distributed/dupefilters/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/dupefilters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/dupefilters/redis_bloom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:20:18.119217 Scrapy-Distributed-2023.4.23/scrapy_distributed/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/middlewares/amqp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/middlewares/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/middlewares/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:20:18.119217 Scrapy-Distributed-2023.4.23/scrapy_distributed/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/pipelines/amqp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/pipelines/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:20:18.123217 Scrapy-Distributed-2023.4.23/scrapy_distributed/queues/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/queues/amqp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/queues/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/queues/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:20:18.123217 Scrapy-Distributed-2023.4.23/scrapy_distributed/redis_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/redis_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/redis_utils/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/redis_utils/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:20:18.123217 Scrapy-Distributed-2023.4.23/scrapy_distributed/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/schedulers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/schedulers/redis_bloom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:20:18.123217 Scrapy-Distributed-2023.4.23/scrapy_distributed/spiders/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/spiders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/spiders/redis_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/scrapy_distributed/spiders/sitemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 05:20:18.123217 Scrapy-Distributed-2023.4.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-23 05:20:08.000000 Scrapy-Distributed-2023.4.23/setup.py
```

### Comparing `Scrapy-Distributed-2020.12.1/README.md` & `Scrapy-Distributed-2023.4.23/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -52,55 +52,72 @@
 && python setup.py install
 ```
 
 There is a simple demo in [`examples/simple_example`]((examples/)). Here is the fast way to use `Scrapy-Distributed`.
 
 ### [Examples of RabbitMQ](examples/rabbitmq_example)
 
+If you don't have the required environment for tests:
+
 ```bash
 # pull and run a RabbitMQ container.
-docker run -d --name rabbitmq -p 0.0.0.0:15672:15672 -p 0.0.0.0:5672:5672 rabbitmq:3
-# enable rabbitmq_management
-docker exec -it <rabbitmq-container-id> /bin/bash
-cd /etc/rabbitmq/
-rabbitmq-plugins enable rabbitmq_management
+docker run -d --name rabbitmq -p 0.0.0.0:15672:15672 -p 0.0.0.0:5672:5672 rabbitmq:3-management
 
 # pull and run a RedisBloom container.
-docker run -d --name redis-redisbloom -p 6379:6379 redislabs/rebloom:latest
+docker run -d --name redisbloom -p 6379:6379 redis/redis-stack
 
 cd examples/rabbitmq_example
 python run_simple_example.py
+```
 
+Or you can use docker compose:
+
+```bash
+docker compose -f ./docker-compose.dev.yaml up -d
+cd examples/rabbitmq_example
+python run_simple_example.py
 ```
 
 ### [Examples of Kafka](examples/kafka_example)
 
+If you don't have the required environment for tests:
+
 ```bash
 # make sure you have a Kafka running on localhost:9092
 # pull and run a RedisBloom container.
-docker run -d --name redis-redisbloom -p 6379:6379 redislabs/rebloom:latest
+docker run -d --name redisbloom -p 6379:6379 redis/redis-stack
 
 cd examples/kafka_example
 python run_simple_example.py
+```
 
+Or you can use docker compose:
+
+```bash
+docker compose -f ./docker-compose.dev.yaml up -d
+cd examples/kafka_example
+python run_simple_example.py
 ```
 
 ## RabbitMQ Support
 
 If you don't have the required environment for tests:
 
 ```bash
 # pull and run a RabbitMQ container.
-docker run -d --name rabbitmq -p 0.0.0.0:15672:15672 -p 0.0.0.0:5672:5672 rabbitmq:3
-# enable rabbitmq_management
-docker exec -it <rabbitmq-container-id> /bin/bash
-cd /etc/rabbitmq/
-rabbitmq-plugins enable rabbitmq_management
+docker run -d --name rabbitmq -p 0.0.0.0:15672:15672 -p 0.0.0.0:5672:5672 rabbitmq:3-management
+
 # pull and run a RedisBloom container.
-docker run -d --name redis-redisbloom -p 6379:6379 redislabs/rebloom:latest
+docker run -d --name redisbloom -p 6379:6379 redis/redis-stack
+```
+
+Or you can use docker compose:
+
+```bash
+docker compose -f ./docker-compose.dev.yaml up -d
 ```
 
 ### **Step 1:**
 
 Only by change `SCHEDULER`, `DUPEFILTER_CLASS` and add some configs, you can get a distributed crawler in a moment.
 
 ```
```

### Comparing `Scrapy-Distributed-2020.12.1/Scrapy_Distributed.egg-info/SOURCES.txt` & `Scrapy-Distributed-2023.4.23/Scrapy_Distributed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Scrapy-Distributed-2020.12.1/scrapy_distributed/amqp_utils/connection.py` & `Scrapy-Distributed-2023.4.23/scrapy_distributed/amqp_utils/connection.py`

 * *Files identical despite different names*

### Comparing `Scrapy-Distributed-2020.12.1/scrapy_distributed/common/queue_config.py` & `Scrapy-Distributed-2023.4.23/scrapy_distributed/common/queue_config.py`

 * *Files identical despite different names*

### Comparing `Scrapy-Distributed-2020.12.1/scrapy_distributed/dupefilters/redis_bloom.py` & `Scrapy-Distributed-2023.4.23/scrapy_distributed/dupefilters/redis_bloom.py`

 * *Files identical despite different names*

### Comparing `Scrapy-Distributed-2020.12.1/scrapy_distributed/middlewares/amqp.py` & `Scrapy-Distributed-2023.4.23/scrapy_distributed/middlewares/amqp.py`

 * *Files identical despite different names*

### Comparing `Scrapy-Distributed-2020.12.1/scrapy_distributed/middlewares/kafka.py` & `Scrapy-Distributed-2023.4.23/scrapy_distributed/middlewares/kafka.py`

 * *Files identical despite different names*

### Comparing `Scrapy-Distributed-2020.12.1/scrapy_distributed/pipelines/amqp.py` & `Scrapy-Distributed-2023.4.23/scrapy_distributed/pipelines/amqp.py`

 * *Files identical despite different names*

### Comparing `Scrapy-Distributed-2020.12.1/scrapy_distributed/pipelines/kafka.py` & `Scrapy-Distributed-2023.4.23/scrapy_distributed/pipelines/kafka.py`

 * *Files identical despite different names*

### Comparing `Scrapy-Distributed-2020.12.1/scrapy_distributed/queues/__init__.py` & `Scrapy-Distributed-2023.4.23/scrapy_distributed/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `Scrapy-Distributed-2020.12.1/scrapy_distributed/queues/amqp.py` & `Scrapy-Distributed-2023.4.23/scrapy_distributed/queues/amqp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import json
 import logging
 from typing import Dict
 
 from scrapy.http.request import Request
-from scrapy_distributed.queues.common import BytesDump, keys_string
+from scrapy_distributed.queues.common import BytesDump, keys_string, get_method
 from scrapy.utils.misc import load_object
 
-from scrapy.utils.reqser import _get_method, request_to_dict
+from scrapy.utils.reqser import request_to_dict
 from w3lib.util import to_unicode
 from scrapy_distributed.queues import IQueue
 import time
 
 import pika
 
 from scrapy_distributed.amqp_utils import connection
@@ -171,40 +171,40 @@
         """Create Request object from a dict.
 
         If a spider is given, it will try to resolve the callbacks looking at the
         spider for methods with the same name.
         """
         cb = d.get("callback", None)
         if cb and spider:
-            cb = _get_method(spider, cb)
+            cb = get_method(spider, cb)
         eb = d.get("errback", None)
         if eb and spider:
-            eb = _get_method(spider, eb)
+            eb = get_method(spider, eb)
         request_cls = load_object(d.get("_class", None)) if "_class" in d else Request
         return request_cls(
             url=to_unicode(d.get("url", None)),
             callback=cb,
             errback=eb,
             method=d.get("method", None),
             headers=d.get("headers", None),
             body=d.get("body", None),
             cookies=d.get("cookies", None),
             meta=d.get("meta", None),
-            encoding=d.get("_encoding", None),
+            encoding=d.get("_encoding", "utf-8"),
             priority=d.get("priority", 0),
             dont_filter=d.get("dont_filter", True),
             flags=d.get("flags", None),
+            cb_kwargs=d.get('cb_kwargs', None),
         )
 
     @classmethod
     def _request_to_dict(cls, request, spider=None):
         d = request_to_dict(request, spider)
         new_dict = dict()
         for key, value in d.items():
             if value:
                 new_dict[key] = value
         logger.debug(f"request_to_dict: {d}")
         return new_dict
 
 
-
 __all__ = ["RabbitQueue"]
```

### Comparing `Scrapy-Distributed-2020.12.1/scrapy_distributed/queues/kafka.py` & `Scrapy-Distributed-2023.4.23/scrapy_distributed/queues/kafka.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
+
 import json
 import logging
 from scrapy.http.request import Request
 from scrapy.utils.misc import load_object
 
-from scrapy.utils.reqser import _get_method, request_to_dict
+from scrapy.utils.reqser import request_to_dict
 from w3lib.util import to_unicode
-from scrapy_distributed.queues.common import BytesDump, keys_string
+from scrapy_distributed.queues.common import BytesDump, keys_string, get_method
 
 from kafka.admin import KafkaAdminClient, NewTopic
 from kafka import KafkaProducer
 from kafka import KafkaConsumer
 from scrapy_distributed.queues import IQueue
 from scrapy_distributed.common.queue_config import KafkaQueueConfig
 import time
@@ -74,16 +73,16 @@
         self.connect()
 
     @classmethod
     def from_queue_conf(cls, connection_conf, queue_conf: KafkaQueueConfig):
         return cls(
             connection_conf,
             name=queue_conf.topic,
-            num_partitions = queue_conf.num_partitions,
-            replication_factor = queue_conf.replication_factor,
+            num_partitions=queue_conf.num_partitions,
+            replication_factor=queue_conf.replication_factor,
             arguments=queue_conf.arguments,
         )
 
     def __len__(self):
         """Return the length of the queue"""
         return 1
 
@@ -104,53 +103,51 @@
         if not body:
             return None
         request = self._make_request(body, scheduler)
         return request
 
     def _make_request(self, body, scheduler):
         return self._request_from_dict(
-            json.loads(body.decode()), scheduler.spider 
+            json.loads(body.decode()), scheduler.spider
         )
 
     @_try_operation
     def push(self, request, scheduler, headers=None, partition=0):
         """Push a message"""
         body: str = json.dumps(
-                keys_string(self._request_to_dict(request, scheduler.spider)),
-                cls=BytesDump,
-            )
+            keys_string(self._request_to_dict(request, scheduler.spider)),
+            cls=BytesDump,
+        )
         logger.debug(f"push message, body: {body}")
         self.producer.send(self.topic, body.encode(), partition=partition)
 
-
     def connect(self):
         """Make a connection"""
         logger.info(f"connect kafka: {self.connection_conf}")
         if self.admin_client:
             try:
                 self.admin_client.close()
             except:
                 pass
         self.admin_client = KafkaAdminClient(bootstrap_servers=self.connection_conf)
-        topic_list = []
-        topic_list.append(
-            NewTopic(name=self.topic, 
-                    num_partitions=self.num_partitions, 
-                    replication_factor=self.replication_factor))
+        topic_list = [NewTopic(name=self.topic,
+                               num_partitions=self.num_partitions,
+                               replication_factor=self.replication_factor)]
         try:
             self.admin_client.create_topics(new_topics=topic_list, validate_only=False)
         except Exception as e:
             logger.error(e)
 
         if self.producer:
             self.producer.close()
         self.producer = KafkaProducer(bootstrap_servers=self.connection_conf)
         if self.consumer:
             self.consumer.close()
-        self.consumer = KafkaConsumer(self.topic, group_id=f"{self.topic}.spider.consumer", bootstrap_servers=self.connection_conf)
+        self.consumer = KafkaConsumer(self.topic, group_id=f"{self.topic}.spider.consumer",
+                                      bootstrap_servers=self.connection_conf)
 
     def close(self):
         """Close channel"""
         logger.error(f"close Kafka connection")
         self.admin_client.close()
         self.producer.close()
         self.consumer.close()
@@ -164,29 +161,29 @@
         """Create Request object from a dict.
 
         If a spider is given, it will try to resolve the callbacks looking at the
         spider for methods with the same name.
         """
         cb = d.get("callback", None)
         if cb and spider:
-            cb = _get_method(spider, cb)
+            cb = get_method(spider, cb)
         eb = d.get("errback", None)
         if eb and spider:
-            eb = _get_method(spider, eb)
+            eb = get_method(spider, eb)
         request_cls = load_object(d.get("_class", None)) if "_class" in d else Request
         return request_cls(
             url=to_unicode(d.get("url", None)),
             callback=cb,
             errback=eb,
             method=d.get("method", None),
             headers=d.get("headers", None),
             body=d.get("body", None),
             cookies=d.get("cookies", None),
             meta=d.get("meta", None),
-            encoding=d.get("_encoding", None),
+            encoding=d.get("_encoding", "utf-8"),
             priority=d.get("priority", 0),
             dont_filter=d.get("dont_filter", True),
             flags=d.get("flags", None),
         )
 
     @classmethod
     def _request_to_dict(cls, request, spider=None):
@@ -195,8 +192,8 @@
         for key, value in d.items():
             if value:
                 new_dict[key] = value
         logger.debug(f"request_to_dict: {d}")
         return new_dict
 
 
-__all__ = ["RabbitQueue"]
+__all__ = ["KafkaQueue"]
```

### Comparing `Scrapy-Distributed-2020.12.1/scrapy_distributed/redis_utils/connection.py` & `Scrapy-Distributed-2023.4.23/scrapy_distributed/redis_utils/connection.py`

 * *Files identical despite different names*

### Comparing `Scrapy-Distributed-2020.12.1/scrapy_distributed/schedulers/__init__.py` & `Scrapy-Distributed-2023.4.23/scrapy_distributed/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `Scrapy-Distributed-2020.12.1/scrapy_distributed/schedulers/common.py` & `Scrapy-Distributed-2023.4.23/scrapy_distributed/schedulers/common.py`

 * *Files identical despite different names*

### Comparing `Scrapy-Distributed-2020.12.1/scrapy_distributed/spiders/redis_bloom.py` & `Scrapy-Distributed-2023.4.23/scrapy_distributed/spiders/redis_bloom.py`

 * *Files identical despite different names*

### Comparing `Scrapy-Distributed-2020.12.1/scrapy_distributed/spiders/sitemap.py` & `Scrapy-Distributed-2023.4.23/scrapy_distributed/spiders/sitemap.py`

 * *Files identical despite different names*

### Comparing `Scrapy-Distributed-2020.12.1/setup.py` & `Scrapy-Distributed-2023.4.23/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     return "".join(
         line for line in io.StringIO(content) if not line.startswith(".. comment::")
     )
 
 
 setup(
     name="Scrapy-Distributed",
-    version="2020.12.1",
+    version="2023.04.23",
     url="https://github.com/Insutanto/scrapy-distributed",
     project_urls={
         "Documentation": "https://github.com/Insutanto/scrapy-distributed",
         "Source": "https://github.com/Insutanto/scrapy-distributed",
         "Tracker": "https://github.com/Insutanto/scrapy-distributed/issues",
     },
     description="A series distributed components for Scrapy framework",
```

