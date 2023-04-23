# Comparing `tmp/helyos_agent_sdk-0.3.0.tar.gz` & `tmp/helyos_agent_sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helyos_agent_sdk-0.3.0.tar", max compression
+gzip compressed data, was "helyos_agent_sdk-0.4.0.tar", max compression
```

## Comparing `helyos_agent_sdk-0.3.0.tar` & `helyos_agent_sdk-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       88 2023-01-26 14:16:59.066461 helyos_agent_sdk-0.3.0/helyos_agent_sdk/__init__.py
--rw-r--r--   0        0        0    12352 2023-04-10 14:11:35.649809 helyos_agent_sdk-0.3.0/helyos_agent_sdk/client.py
--rw-r--r--   0        0        0    14965 2023-01-26 14:16:49.073494 helyos_agent_sdk-0.3.0/helyos_agent_sdk/connector.py
--rw-r--r--   0        0        0      463 2023-04-10 14:06:03.061672 helyos_agent_sdk-0.3.0/helyos_agent_sdk/exceptions.py
--rw-r--r--   0        0        0     3404 2023-01-26 14:13:46.295378 helyos_agent_sdk-0.3.0/helyos_agent_sdk/models.py
--rw-r--r--   0        0        0     1071 2023-01-26 14:13:46.186379 helyos_agent_sdk-0.3.0/LICENSE
--rw-r--r--   0        0        0     1107 2023-04-10 14:12:16.868334 helyos_agent_sdk-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2589 2023-02-01 14:18:16.120422 helyos_agent_sdk-0.3.0/README.md
--rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 helyos_agent_sdk-0.3.0/setup.py
--rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 helyos_agent_sdk-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       88 2023-01-26 14:16:59.066461 helyos_agent_sdk-0.4.0/helyos_agent_sdk/__init__.py
+-rw-r--r--   0        0        0    14824 2023-04-20 14:39:37.636614 helyos_agent_sdk-0.4.0/helyos_agent_sdk/client.py
+-rw-r--r--   0        0        0    14965 2023-01-26 14:16:49.073494 helyos_agent_sdk-0.4.0/helyos_agent_sdk/connector.py
+-rw-r--r--   0        0        0      463 2023-04-10 14:06:03.061672 helyos_agent_sdk-0.4.0/helyos_agent_sdk/exceptions.py
+-rw-r--r--   0        0        0     3404 2023-01-26 14:13:46.295378 helyos_agent_sdk-0.4.0/helyos_agent_sdk/models.py
+-rw-r--r--   0        0        0     1071 2023-01-26 14:13:46.186379 helyos_agent_sdk-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1107 2023-04-20 13:23:00.871923 helyos_agent_sdk-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2589 2023-02-01 14:18:16.120422 helyos_agent_sdk-0.4.0/README.md
+-rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 helyos_agent_sdk-0.4.0/setup.py
+-rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 helyos_agent_sdk-0.4.0/PKG-INFO
```

### Comparing `helyos_agent_sdk-0.3.0/helyos_agent_sdk/client.py` & `helyos_agent_sdk-0.4.0/helyos_agent_sdk/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,92 @@
 from datetime import datetime as dt
 from functools import wraps
 import pika
-from .exceptions import *
-
 from Crypto.PublicKey import RSA
 from Crypto.Cipher import PKCS1_OAEP
-import os, json
+import os, json, ssl
+from .exceptions import *
 
 AGENTS_UL_EXCHANGE = os.environ.get('AGENTS_UL_EXCHANGE', "xchange_helyos.agents.ul")
 AGENTS_DL_EXCHANGE = os.environ.get('AGENTS_DL_EXCHANGE', "xchange_helyos.agents.dl")
 AGENT_ANONYMOUS_EXCHANGE = os.environ.get('AGENT_ANONYMOUS_EXCHANGE', "xchange_helyos.agents.anonymous")
 REGISTRATION_TOKEN = os.environ.get('REGISTRATION_TOKEN','0000-0000-0000-0000-0000')
 
 
-def connect_rabbitmq(rabbitmq_host, rabbitmq_port, username, passwd, temporary=False):
+def connect_rabbitmq(rabbitmq_host, rabbitmq_port, username, passwd, enable_ssl=False, ca_certificate=None, temporary=False):
     credentials = pika.PlainCredentials(username, passwd)
+    if enable_ssl:
+        context = ssl.create_default_context(cadata=ca_certificate)
+        if ca_certificate is not None:
+            context.check_hostname = True
+            context.verify_mode =  ssl.CERT_REQUIRED
+        else:
+            context.check_hostname = False
+            context.verify_mode =  ssl.CERT_NONE
+
+        ssl_options = pika.SSLOptions(context, rabbitmq_host)
+    else:
+        ssl_options = None
+
+
+
     if temporary:
-        params = pika.ConnectionParameters(rabbitmq_host,  rabbitmq_port, '/', credentials,heartbeat=60, blocked_connection_timeout=60)
+        params = pika.ConnectionParameters(rabbitmq_host,  rabbitmq_port, '/', credentials,heartbeat=60, blocked_connection_timeout=60,
+                                            ssl_options=ssl_options)
     else:
-        params = pika.ConnectionParameters(rabbitmq_host,  rabbitmq_port, '/', credentials,heartbeat=3600,blocked_connection_timeout=300)
+        params = pika.ConnectionParameters(rabbitmq_host,  rabbitmq_port, '/', credentials,heartbeat=3600,blocked_connection_timeout=300,
+                                            ssl_options=ssl_options )
     _connection = pika.BlockingConnection(params)
     return _connection    
 
 
 def generate_private_public_keys():
     key = RSA.generate(2048)
     priv = key.export_key(format='PEM')
     pub = key.publickey().export_key(format='PEM')
     return priv, pub
     
 
 
 class HelyOSClient():
-    connection = None
-    channel = None
-    checkin_data = None
-    tries = 0
+
     
-    def __init__(self, rabbitmq_host, rabbitmq_port=5672, uuid=None, pubkey=None):
+    def __init__(self, rabbitmq_host, rabbitmq_port=5672, uuid=None, enable_ssl=False, ca_certificate=None,  pubkey=None):
         """ HelyOS client class
 
-            The client implements several functions to make it easier to
-            interact with rabbitMQ. It reads the rabbitMQ exchange names from environment variables
-            and it encloses the routing-key names as properties.
+            The client implements several functions to facilitate the
+            interaction with RabbitMQ. It reads the RabbitMQ exchange names from environment variables
+            and it provides the helyOS routing-key names as properties.
 
             :param rabbitmq_host: RabbitMQ host name (e.g rabbitmq.mydomain.com)
             :type rabbitmq_host: str
             :param rabbitmq_port: RabbitMQ port, defaults to 5672
             :type rabbitmq_port: int
             :param uuid: universal unique identifier fot the agent
             :type uuid: str
-            :param pubkey: RSA public key to be saved in helyOS core, defaults to None
-            :type pubkey: str, optional
+            :param enable_ssl: Enable rabbitmq SSL connection, default False.
+            :type enable_ssl: boolean, optional
+            :param ca_certificate: Certificate authority of the RabbitMQ server, defaults to None
+            :type ca_certificate: string (PEM format), optional
+            :param pubkey: RSA public key can be saved in helyOS core, defaults to None
+            :type pubkey:  string (PEM format), optional
 
         """
         self.rabbitmq_host = rabbitmq_host
         self.rabbitmq_port = rabbitmq_port
+        self.ca_certificate = ca_certificate
         self.uuid = uuid
+        self.enable_ssl = enable_ssl
+
+        self.connection = None
+        self.channel = None
+        self.checkin_data = None
+        self.tries = 0
+        self.rbmq_username = None
+        self.rbmq_password = None
         
         if pubkey is None:
             self.private_key, self.public_key = generate_private_public_keys()
         else:
             self.public_key = pubkey
 
         self.rabbitmq_host = rabbitmq_host    
@@ -129,15 +155,15 @@
 
         return wrap
 
     def __connect_as_anonymous(self):
 
         # step 1 - connect anonymously
         try:
-            temp_connection = connect_rabbitmq(self.rabbitmq_host, self.rabbitmq_port,'anonymous', 'anonymous', temporary=True)        
+            temp_connection = connect_rabbitmq(self.rabbitmq_host, self.rabbitmq_port,'anonymous', 'anonymous', self.enable_ssl, temporary=True)        
             self.guest_channel = temp_connection.channel()
         except Exception as inst:
             print(inst)
             raise HelyOSAnonymousConnectionError(
                     "Not able to connect as anonymous to rabbitMQ to perform check in.")
     
         
@@ -153,38 +179,58 @@
         # step 2 - creates a temporary queue to receive checkin response
         temp_queue = self.guest_channel.queue_declare(queue='', exclusive=True)            
         self.checkin_response_queue = temp_queue.method.queue 
         self.guest_channel.basic_consume(queue=self.checkin_response_queue, auto_ack=True, on_message_callback=self.__checkin_callback)
 
 
     def connect_rabbitmq(self, username, password):
-        """ Connect to RabbitMQ 
+        """
+        Creates the connection between agent and the RabbitMQ server.
+        
+        .. code-block:: python
 
+            helyos_client = HelyOSClient(host='myrabbitmq.com', port=5672, uuid='3452345-52453-43525')
+            helyos_client.connect_rabbitmq('my_username', 'secret_password') #  <===
+                      
+        
         :param username:  username previously registered in RabbitMQ server
         :type username: str
         :param password: password previously registered in RabbitMQ server'
         :type password: str
         """
 
         try:
-            self.connection = connect_rabbitmq(self.rabbitmq_host, self.rabbitmq_port, username, password) 
+            self.connection = connect_rabbitmq(self.rabbitmq_host, 
+            self.rabbitmq_port, username, password, self.enable_ssl, self.ca_certificate) 
             self.channel = self.connection.channel()
             self.rbmq_username = username
 
         except Exception as inst:
             print(inst)
             raise HelyOSAccountConnectionError(
                     f"Not able to connect as {username} to rabbitMQ to perform check in.")
 
 
 
     def perform_checkin(self, yard_uid, status='free', agent_data={}):
-        """ Check in the agent: The checkin procedure registers an agent to a specific yard, and retrives the data about this yard. 
-            If the agent does not have a rabbitMQ account, helyOS will create an rabbitmq account using the agent's uuid as username.
-            Username and password are transmitted to the agent inside the check-in data.
+        """ 
+        The check-in procedure registers the agent to a specific yard. helyOS will publish the relevant data about the yard 
+        and the CA certificate of the RabbitMQ server, which is relevant for SSL connections. Use the method `get_checkin_result()` to retrieve these data.
+
+        The method `connect_rabbitmq()` should run before the check-in, otherwise, it will be assumed that the agent does not have yet a RabbitMQ account.
+        In this case, if the environment variable REGISTRATION_TOKEN is set, helyOS will create a RabbitMQ account using the 
+        uuid as username and returns a password, which can be found in the property `rbmq_password`. This password should be safely stored.
+
+        .. code-block:: python
+
+            helyos_client = HelyOSClient(host='myrabbitmq.com', port=5672, uuid='3452345-52453-43525')
+            helyos_client.connect_rabbitmq('my_username', 'secret_password')
+            helyos_client.perform_checkin(yard_uid='yard_A', status='free')  #  <===
+            helyOS_client.get_checkin_result()                               #  <===
+                       
 
         :param yard_uid: Yard UID
         :type yard_uid: str
         :param status: Agent status, defaults to 'free'
         :type status: str
         """
         if self.connection:
@@ -223,38 +269,44 @@
         body = received_message['body']
         response_code = body.get('response_code', 500)
         if response_code!='200':
             print(body)
             message  = body.get('message', "Check in refused")
             raise HelyOSCheckinError(f"{message}: code {response_code}")
             
-        password = body.get('rbmq_password', None)
+        password = body.pop('rbmq_password', None)
+        self.ca_certificate =  body.get('ca_certificate', self.ca_certificate)
+        
         try:
             if password:
-                self.connection = connect_rabbitmq(self.rabbitmq_host, self.rabbitmq_port, body['rbmq_username'], password)
+                self.connection = connect_rabbitmq(self.rabbitmq_host, self.rabbitmq_port, body['rbmq_username'], password, self.enable_ssl, self.ca_certificate)
                 self.channel = self.connection.channel()
                 self.rbmq_username = body['rbmq_username']
+                self.rbmq_password = password
+
+                print('uuid', self.uuid)
                 print('username', body['rbmq_username'])
-                print('password', body['rbmq_password'])
+                print('password', len(password)*'*')
+
             self.uuid = received_message['uuid']
             self.checkin_data = body
             ch.stop_consuming()
             
-            print('uuid', self.uuid)
 
         except  Exception as inst: 
             self.tries += 1
             print(f"try {self.tries}")
             if self.tries > 3:
                 ch.stop_consuming()
 
 
     @auth_required            
     def publish(self, routing_key, message, encrypted=False, exchange=AGENTS_UL_EXCHANGE):
         """ Publish message in RabbitMQ
+
             :param routing_key: RabbitMQ routing_key 
             :type routing_key: str
             :param encrypted: If this message should be encrypted, defaults to False
             :type encrypted: str
             :param exchange: RabbitMQ exchange, defaults to env.AGENTS_UL_EXCHANGE
             :type exchange: str
         """
```

### Comparing `helyos_agent_sdk-0.3.0/helyos_agent_sdk/connector.py` & `helyos_agent_sdk-0.4.0/helyos_agent_sdk/connector.py`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.3.0/helyos_agent_sdk/models.py` & `helyos_agent_sdk-0.4.0/helyos_agent_sdk/models.py`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.3.0/LICENSE` & `helyos_agent_sdk-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.3.0/pyproject.toml` & `helyos_agent_sdk-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "helyos_agent_sdk"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["Carlos Viol Barbosa <you@example.com>"]
 readme = "README.md"
 packages = [{include = "helyos_agent_sdk"}]
 keywords = ["autonomous driving", "helyos", "sdk"]
 
 homepage = "https://helyos.ivi.fraunhofer.de"
```

### Comparing `helyos_agent_sdk-0.3.0/README.md` & `helyos_agent_sdk-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.3.0/setup.py` & `helyos_agent_sdk-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['dataclasses-json>=0.5.7,<0.6.0',
  'pika>=1.3.1,<2.0.0',
  'pycryptodome>=3.15.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'helyos-agent-sdk',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': '',
     'long_description': '<div id="top"></div>\n\n<!-- PROJECT LOGO -->\n<br />\n<div align="center">\n  <a href="https://github.com/">\n    <img src="helyos_logo.png" alt="Logo"  height="80">\n    <img src="truck.png" alt="Logo"  height="80">\n  </a>\n\n  <h3 align="center">helyOS Agent SDK</h3>\n\n  <p align="center">\n    Methods and data strrctures to connect autonomous vehicles to helyOS.\n    <br />\n    <a href="https://fraunhoferivi.github.io/helyOS-agent-sdk/"><strong>Explore the docs »</strong></a>\n    <br />\n    <br />\n    <a href="https://github.com/">View Demo</a>\n    ·\n    <a href="https://github.com/FraunhoferIVI/helyOS-agent-sdk/issues">Report Bug</a>\n    ·\n    <a href="https://github.com/FraunhoferIVI/helyOS-agent-sdk/issues">Request Feature</a>\n  </p>\n</div>\n\n## About The Project\n\nThe helyos-agent-sdk python package encloses methods and data structures definitions that facilitate the connection to helyOS core through rabbitMQ.\n\n### List of features\n\n*   RabbitMQ client to communicate with helyOS. \n*   Check-in method.\n*   Agent and assignment status definitions. \n*   Easy access to helyOS assignments via callbacks. \n*   Application-level encryption.\n\n### Install\n\n```\npip install helyos_agent_sdk\n\n```\n### Usage\n\n```python\nos.environ[\'AGENTS_UL_EXCHANGE\'] = "xchange_helyos.agents.ul"\nos.environ[\'AGENTS_DL_EXCHANGE\'] = "xchange_helyos.agents.dl"\nos.environ[\'AGENT_ANONYMOUS_EXCHANGE\'] = "xchange_helyos.agents.anonymous"\nfrom helyos_agent_sdk import HelyOSClient, AgentConnector\n\n# Check in\ninitial_agent_data = {\'name\': "vehicle name", \'pose\': {\'x\':-30167, \'y\':-5415, \'orientations\':[0, 0]}, \'geometry\':{"my_custom_format": {}}}\nhelyOS_client = HelyOSClient(rabbitmq_host, rabbitmq_port, uuid=AGENT_UID)\nhelyOS_client.perform_checkin(yard_uid=\'1\', agent_data=initial_agent_data, status="free")\nhelyOS_client.get_checkin_result()\n\n\n# Communication\nagent_connector = AgentConnector(helyOS_client)\nagent_connector.publish_sensors(x=-30167, y=3000, z=0, orientations=[1500, 0], sensor= {"my_custom_format": {}})\n\n# ... #\n\nagentConnector.publish_state(status, resources, assignment_status)\n\n# ... #\n\nagentConnector.consume_instant_action_messages(my_reserve_callback, my_release_callback, my_cancel_assignm_callback, any_other_callback)\nagentConnector.consume_assignment_messages(my_assignment_callback)\nagentConnector.start_consuming()\n\n\n```\n\n\n### Contributing\n\nKeep it simple. Keep it minimal.\n\n### Authors \n\n*   Carlos E. Viol Barbosa\n*   ...\n\n### License\n\nThis project is licensed under the MIT License',
     'author': 'Carlos Viol Barbosa',
     'author_email': 'you@example.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://helyos.ivi.fraunhofer.de',
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['helyos_agent_sdk'] package_data = \ {'': ['*']} install_requires = \
 ['dataclasses-json>=0.5.7,<0.6.0', 'pika>=1.3.1,<2.0.0',
 'pycryptodome>=3.15.0,<4.0.0'] setup_kwargs = { 'name': 'helyos-agent-sdk',
-'version': '0.3.0', 'description': '', 'long_description': '
+'version': '0.4.0', 'description': '', 'long_description': '
 \n\n\n
 \n
                           \n \n_[Logo]\n_[Logo]\n\n\n
                           **** helyOS Agent SDK ****
                                      \n\n
   \n Methods and data strrctures to connect autonomous vehicles to helyOS.\n
                            \n Explore_the_docs_Â»\n
```

### Comparing `helyos_agent_sdk-0.3.0/PKG-INFO` & `helyos_agent_sdk-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helyos-agent-sdk
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Home-page: https://helyos.ivi.fraunhofer.de
 Keywords: autonomous driving,helyos,sdk
 Author: Carlos Viol Barbosa
 Author-email: you@example.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: helyos-agent-sdk Version: 0.3.0 Summary: Home-page:
+Metadata-Version: 2.1 Name: helyos-agent-sdk Version: 0.4.0 Summary: Home-page:
 https://helyos.ivi.fraunhofer.de Keywords: autonomous driving,helyos,sdk
 Author: Carlos Viol Barbosa Author-email: you@example.com Requires-Python:
 >=3.7,<4.0 Classifier: Environment :: Console Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

