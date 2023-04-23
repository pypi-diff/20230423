# Comparing `tmp/revChatGPT-4.2.5.tar.gz` & `tmp/revChatGPT-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-4.2.5.tar", last modified: Wed Apr 19 00:35:23 2023, max compression
+gzip compressed data, was "revChatGPT-5.0.0.tar", last modified: Sun Apr 23 13:19:43 2023, max compression
```

## Comparing `revChatGPT-4.2.5.tar` & `revChatGPT-5.0.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:35:23.014792 revChatGPT-4.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-04-19 00:35:23.014792 revChatGPT-4.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-19 00:35:22.000000 revChatGPT-4.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 00:35:23.014792 revChatGPT-4.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:35:23.014792 revChatGPT-4.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:35:23.014792 revChatGPT-4.2.5/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    47161 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:35:23.014792 revChatGPT-4.2.5/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:35:23.014792 revChatGPT-4.2.5/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-04-19 00:35:23.000000 revChatGPT-4.2.5/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-19 00:35:23.000000 revChatGPT-4.2.5/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:35:23.000000 revChatGPT-4.2.5/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-19 00:35:23.000000 revChatGPT-4.2.5/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 00:35:23.000000 revChatGPT-4.2.5/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:19:43.738466 revChatGPT-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-04-23 13:19:43.738466 revChatGPT-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-04-23 13:19:43.000000 revChatGPT-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 13:19:43.738466 revChatGPT-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:19:43.734466 revChatGPT-5.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:19:43.738466 revChatGPT-5.0.0/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    49256 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:19:43.738466 revChatGPT-5.0.0/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/src/revChatGPT/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:19:43.738466 revChatGPT-5.0.0/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-04-23 13:19:43.000000 revChatGPT-5.0.0/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-23 13:19:43.000000 revChatGPT-5.0.0/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 13:19:43.000000 revChatGPT-5.0.0/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-23 13:19:43.000000 revChatGPT-5.0.0/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 13:19:43.000000 revChatGPT-5.0.0/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:19:43.738466 revChatGPT-5.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/tests/test_recipient.py
```

### Comparing `revChatGPT-4.2.5/LICENSE` & `revChatGPT-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.5/PKG-INFO` & `revChatGPT-5.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.2.5
+Version: 5.0.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -48,15 +48,15 @@
 
 ### Suport Python Version
 
 - Minimum - Python3.9
 - Recommend - Python3.11+
 
 <details>
-  
+
   <summary>
 
 # V1 Standard ChatGPT
 
 Due to recent tightening of OpenAI's security, the default endpoint has been swapped over to one provided by @pengzhile. It is not open source and privacy is not guarenteed. Use it at your own risk. I am working on an open source implementation with the latest changes but that could take a while.
 
 </summary>
@@ -169,15 +169,15 @@
 
 #### All API methods
 
 Refer to the [wiki](https://github.com/acheong08/ChatGPT/wiki/) for advanced developer usage.
 
 </details>
 
-<summary>  
+<summary>
 
 # V3 Official Chat API
 
 > Recently released by OpenAI
 >
 > - Paid
```

### Comparing `revChatGPT-4.2.5/README.md` & `revChatGPT-5.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 ### Suport Python Version
 
 - Minimum - Python3.9
 - Recommend - Python3.11+
 
 <details>
-  
+
   <summary>
 
 # V1 Standard ChatGPT
 
 Due to recent tightening of OpenAI's security, the default endpoint has been swapped over to one provided by @pengzhile. It is not open source and privacy is not guarenteed. Use it at your own risk. I am working on an open source implementation with the latest changes but that could take a while.
 
 </summary>
@@ -147,15 +147,15 @@
 
 #### All API methods
 
 Refer to the [wiki](https://github.com/acheong08/ChatGPT/wiki/) for advanced developer usage.
 
 </details>
 
-<summary>  
+<summary>
 
 # V3 Official Chat API
 
 > Recently released by OpenAI
 >
 > - Paid
```

### Comparing `revChatGPT-4.2.5/setup.py` & `revChatGPT-5.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="4.2.5",
+    version="5.0.0",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
@@ -28,14 +28,15 @@
     package_dir={"": "src"},
     py_modules=["revChatGPT"],
     package_data={"": ["*.json"]},
     install_requires=[
         "OpenAIAuth==0.3.6",
         "requests[socks]",
         "httpx[socks]",
+        "async_tio",
         "prompt-toolkit",
         "tiktoken>=0.3.0",
         "openai",
     ],
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Intended Audience :: Developers",
```

### Comparing `revChatGPT-4.2.5/src/revChatGPT/V1.py` & `revChatGPT-5.0.0/src/revChatGPT/V1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Standard ChatGPT
 """
 from __future__ import annotations
 
 import base64
+import binascii
 import contextlib
+import datetime
 import json
 import logging
 import time
 import uuid
 from functools import wraps
 from os import environ
 from os import getenv
@@ -21,14 +23,17 @@
 import requests
 from httpx import AsyncClient
 from OpenAIAuth import Authenticator
 from OpenAIAuth import Error as AuthError
 
 from . import __version__
 from . import typings as t
+from .recipient import PythonRecipient
+from .recipient import Recipient
+from .recipient import RecipientManager
 from .utils import create_completer
 from .utils import create_session
 from .utils import get_input
 
 if __name__ == "__main__":
     logging.basicConfig(
         format="%(asctime)s - %(name)s - %(levelname)s - %(funcName)s - %(message)s",
@@ -48,26 +53,31 @@
     """
 
     def decorator(func):
         wraps(func)
 
         def wrapper(*args, **kwargs):
             log.debug(
-                f"Entering {func.__name__} with args {args} and kwargs {kwargs}",
+                "Entering %s with args %s and kwargs %s",
+                func.__name__,
+                args,
+                kwargs,
             )
             start = time.time()
             out = func(*args, **kwargs)
             end = time.time()
             if is_timed:
                 log.debug(
-                    f"Exiting {func.__name__} with return value {out}. Took {end - start} seconds.",
+                    "Exiting %s with return value %s. Took %s seconds.",
+                    func.__name__,
+                    out,
+                    end - start,
                 )
             else:
-                log.debug(f"Exiting {func.__name__} with return value {out}")
-
+                log.debug("Exiting %s with return value %s", func.__name__, out)
             return out
 
         return wrapper
 
     return decorator
 
 
@@ -77,14 +87,16 @@
 
 
 class Chatbot:
     """
     Chatbot class for ChatGPT
     """
 
+    recipients: RecipientManager
+
     @logger(is_timed=True)
     def __init__(
         self,
         config: dict[str, str],
         conversation_id: str | None = None,
         parent_id: str | None = None,
         session_client=None,
@@ -94,19 +106,17 @@
         """Initialize a chatbot
 
         Args:
             config (dict[str, str]): Login and proxy info. Example:
                 {
                     "email": "OpenAI account email",
                     "password": "OpenAI account password",
-                    "session_token": "<session_token>"
                     "access_token": "<access_token>"
                     "proxy": "<proxy_url_string>",
                     "paid": True/False, # whether this is a plus account
-                    "_puid": "puid", # V4 only, if it is set, base_url will be changed to https://chat.openai.com/backend-api/
                 }
                 More details on these are available at https://github.com/acheong08/ChatGPT#configuration
             conversation_id (str | None, optional): Id of the conversation to continue on. Defaults to None.
             parent_id (str | None, optional): Id of the previous response message to continue on. Defaults to None.
             session_client (_type_, optional): _description_. Defaults to None.
 
         Raises:
@@ -147,69 +157,55 @@
                 "https": config["proxy"],
             }
             if isinstance(self.session, AsyncClient):
                 proxies = {
                     "http://": config["proxy"],
                     "https://": config["proxy"],
                 }
-                self.session = AsyncClient(proxies=proxies)
+                self.session = AsyncClient(proxies=proxies)  # type: ignore
             else:
                 self.session.proxies.update(proxies)
+
         self.conversation_id = conversation_id
         self.parent_id = parent_id
         self.conversation_mapping = {}
         self.conversation_id_prev_queue = []
         self.parent_id_prev_queue = []
         self.lazy_loading = lazy_loading
-
-        if "_puid" in self.config and self.config["_puid"]:
-            self.base_url = "https://chat.openai.com/backend-api/"
-            self.__set_puid(self.config["_puid"])
-        else:
-            self.base_url = base_url or BASE_URL
+        self.base_url = base_url or BASE_URL
+        self.recipients = RecipientManager()
 
         self.__check_credentials()
 
     @logger(is_timed=True)
     def __check_credentials(self) -> None:
         """Check login info and perform login
 
         Any one of the following is sufficient for login. Multiple login info can be provided at the same time and they will be used in the order listed below.
             - access_token
-            - session_token
             - email + password
 
         Raises:
             Exception: _description_
             AuthError: _description_
         """
         if "access_token" in self.config:
             self.set_access_token(self.config["access_token"])
-        elif "session_token" in self.config:
-            pass
         elif "email" not in self.config or "password" not in self.config:
             error = t.AuthenticationError("Insufficient login details provided!")
             raise error
         if "access_token" not in self.config:
             try:
                 self.login()
             except AuthError as error:
                 print(error.details)
                 print(error.status_code)
                 raise error
 
     @logger(is_timed=False)
-    def __set_puid(self, puid: str) -> None:
-        self.session.cookies.update(
-            {
-                "_puid": puid,
-            },
-        )
-
-    @logger(is_timed=False)
     def set_access_token(self, access_token: str) -> None:
         """Set access token in request header and self.config, then cache it to file.
 
         Args:
             access_token (str): access_token
         """
         self.session.headers.clear()
@@ -260,15 +256,15 @@
             try:
                 # Split access_token into 3 parts
                 s_access_token = access_token.split(".")
                 # Add padding to the middle part
                 s_access_token[1] += "=" * ((4 - len(s_access_token[1]) % 4) % 4)
                 d_access_token = base64.b64decode(s_access_token[1])
                 d_access_token = json.loads(d_access_token)
-            except base64.binascii.Error:
+            except binascii.Error:
                 error = t.Error(
                     source="__get_cached_access_token",
                     message="Invalid access token",
                     code=t.ErrorType.INVALID_ACCESS_TOKEN_ERROR,
                 )
                 raise error from None
             except json.JSONDecodeError:
@@ -325,49 +321,37 @@
             cached = json.load(open(self.cache_path, encoding="utf-8"))
         except (FileNotFoundError, json.decoder.JSONDecodeError):
             cached = {}
         return cached
 
     @logger(is_timed=True)
     def login(self) -> None:
-        if (
-            "email" not in self.config or "password" not in self.config
-        ) and "session_token" not in self.config:
+        """Login to OpenAI by email and password"""
+        if self.config.get("email") and self.config.get("password"):
             log.error("Insufficient login details provided!")
             error = t.AuthenticationError("Insufficient login details provided!")
             raise error
         auth = Authenticator(
             email_address=self.config.get("email"),
             password=self.config.get("password"),
             proxy=self.config.get("proxy"),
         )
-        if self.config.get("session_token"):
-            log.debug("Using session token")
-            auth.session.cookies.set(
-                "__Secure-next-auth.session-token",
-                self.config["session_token"],
-            )
-            auth.get_access_token()
-            if auth.access_token is None:
-                del self.config["session_token"]
-                self.login()
-                return
-        else:
-            log.debug("Using authenticator to get access token")
-            auth.begin()
-            auth.get_access_token()
+        log.debug("Using authenticator to get access token")
+        auth.begin()
+        auth.get_access_token()
 
         self.set_access_token(auth.access_token)
 
     @logger(is_timed=True)
     def __send_request(
         self,
         data: dict,
         auto_continue: bool = False,
         timeout: float = 360,
+        **kwargs,
     ) -> Generator[dict, None, None]:
         log.debug("Sending the payload")
 
         cid, pid = data["conversation_id"], data["parent_message_id"]
         model, message = None, ""
 
         self.conversation_id_prev_queue.append(cid)
@@ -434,29 +418,30 @@
             self.conversation_id = cid
 
         if not (auto_continue and finish_details == "max_tokens"):
             return
         message = message.strip("\n")
         for i in self.continue_write(
             conversation_id=cid,
-            model=model,
             timeout=timeout,
+            auto_continue=False,
         ):
             i["message"] = message + i["message"]
             yield i
 
     @logger(is_timed=True)
     def post_messages(
         self,
         messages: list[dict],
         conversation_id: str | None = None,
         parent_id: str | None = None,
         model: str | None = None,
         auto_continue: bool = False,
         timeout: float = 360,
+        **kwargs,
     ) -> Generator[dict, None, None]:
         """Ask a question to the chatbot
         Args:
             messages (list[dict]): The messages to send
             conversation_id (str | None, optional): UUID for the conversation to continue on. Defaults to None.
             parent_id (str | None, optional): UUID for the message to continue on. Defaults to None.
             model (str | None, optional): The model to use. Defaults to None.
@@ -488,15 +473,16 @@
         if not conversation_id and not parent_id:
             parent_id = str(uuid.uuid4())
 
         if conversation_id and not parent_id:
             if conversation_id not in self.conversation_mapping:
                 if self.lazy_loading:
                     log.debug(
-                        f"Conversation ID {conversation_id} not found in conversation mapping, try to get conversation history for the given ID",
+                        "Conversation ID %s not found in conversation mapping, try to get conversation history for the given ID",
+                        conversation_id,
                     )
                     with contextlib.suppress(Exception):
                         history = self.get_msg_history(conversation_id)
                         self.conversation_mapping[conversation_id] = history[
                             "current_node"
                         ]
                 else:
@@ -528,29 +514,30 @@
         )
 
     @logger(is_timed=True)
     def ask(
         self,
         prompt: str,
         conversation_id: str | None = None,
-        parent_id: str | None = None,
-        model: str | None = None,
+        parent_id: str = "",
+        model: str = "",
         auto_continue: bool = False,
         timeout: float = 360,
+        **kwargs,
     ) -> Generator[dict, None, None]:
         """Ask a question to the chatbot
         Args:
             prompt (str): The question
-            conversation_id (str | None, optional): UUID for the conversation to continue on. Defaults to None.
-            parent_id (str | None, optional): UUID for the message to continue on. Defaults to None.
-            model (str | None, optional): The model to use. Defaults to None.
+            conversation_id (str, optional): UUID for the conversation to continue on. Defaults to None.
+            parent_id (str, optional): UUID for the message to continue on. Defaults to "".
+            model (str, optional): The model to use. Defaults to "".
             auto_continue (bool, optional): Whether to continue the conversation automatically. Defaults to False.
             timeout (float, optional): Timeout for getting the full response, unit is second. Defaults to 360.
 
-        Yields: Generator[dict, None, None] - The response from the chatbot
+        Yields: The response from the chatbot
             dict: {
                 "message": str,
                 "conversation_id": str,
                 "parent_id": str,
                 "model": str,
                 "finish_details": str, # "max_tokens" or "stop"
                 "end_turn": bool,
@@ -580,19 +567,19 @@
         self,
         conversation_id: str | None = None,
         parent_id: str = "",
         model: str = "",
         auto_continue: bool = False,
         timeout: float = 360,
     ) -> Generator[dict, None, None]:
-        """let the chatbot continue to write
+        """let the chatbot continue to write.
         Args:
             conversation_id (str | None, optional): UUID for the conversation to continue on. Defaults to None.
-            parent_id (str | None, optional): UUID for the message to continue on. Defaults to None.
-            model (str | None, optional): The model to use. Defaults to None.
+            parent_id (str, optional): UUID for the message to continue on. Defaults to None.
+            model (str, optional): The model to use. Defaults to None.
             auto_continue (bool, optional): Whether to continue the conversation automatically. Defaults to False.
             timeout (float, optional): Timeout for getting the full response, unit is second. Defaults to 360.
 
         Yields:
             dict: {
                 "message": str,
                 "conversation_id": str,
@@ -617,15 +604,16 @@
         if not conversation_id and not parent_id:
             parent_id = str(uuid.uuid4())
 
         if conversation_id and not parent_id:
             if conversation_id not in self.conversation_mapping:
                 if self.lazy_loading:
                     log.debug(
-                        f"Conversation ID {conversation_id} not found in conversation mapping, try to get conversation history for the given ID",
+                        "Conversation ID %s not found in conversation mapping, try to get conversation history for the given ID",
+                        conversation_id,
                     )
                     with contextlib.suppress(Exception):
                         history = self.get_msg_history(conversation_id)
                         self.conversation_mapping[conversation_id] = history[
                             "current_node"
                         ]
                 else:
@@ -674,21 +662,21 @@
             response (_type_): _description_
 
         Raises:
             Error: _description_
         """
         try:
             response.raise_for_status()
-        except requests.exceptions.HTTPError as e:
+        except requests.exceptions.HTTPError as ex:
             error = t.Error(
                 source="OpenAI",
                 message=response.text,
                 code=response.status_code,
             )
-            raise error from e
+            raise error from ex
 
     @logger(is_timed=True)
     def get_conversations(
         self,
         offset: int = 0,
         limit: int = 20,
         encoding: str | None = None,
@@ -790,32 +778,25 @@
         """
         for _ in range(num):
             self.conversation_id = self.conversation_id_prev_queue.pop()
             self.parent_id = self.parent_id_prev_queue.pop()
 
 
 class AsyncChatbot(Chatbot):
-    """
-    Async Chatbot class for ChatGPT
-    """
+    """Async Chatbot class for ChatGPT"""
 
     def __init__(
         self,
         config: dict,
         conversation_id: str | None = None,
         parent_id: str = "",
         base_url: str = "",
     ) -> None:
         """
         Same as Chatbot class, but with async methods.
-
-        Note:
-            AsyncChatbot is not compatible with OpenAI Web API, I don't know why the stream method doesn't work.
-            (But the sync version works fine)
-            So, if you want to use AsyncChatbot, you don't need to set the "_puid" parameter in the config.
         """
         super().__init__(
             config=config,
             conversation_id=conversation_id,
             parent_id=parent_id,
             session_client=AsyncClient,
             base_url=base_url,
@@ -879,15 +860,15 @@
             if cid:
                 self.conversation_id = cid
 
         if not (auto_continue and finish_details == "max_tokens"):
             return
         async for msg in self.continue_write(
             conversation_id=cid,
-            auto_continue=auto_continue,
+            auto_continue=False,
             timeout=timeout,
         ):
             msg["message"] = message + msg["message"]
             yield msg
 
     async def post_messages(
         self,
@@ -1168,22 +1149,22 @@
             return False
         return True
 
     async def __check_response(self, response: httpx.Response) -> None:
         # 改成自带的错误处理
         try:
             response.raise_for_status()
-        except httpx.HTTPStatusError as e:
+        except httpx.HTTPStatusError as ex:
             await response.aread()
             error = t.Error(
                 source="OpenAI",
                 message=response.text,
                 code=response.status_code,
             )
-            raise error from e
+            raise error from ex
 
 
 get_input = logger(is_timed=False)(get_input)
 
 
 @logger(is_timed=False)
 def configure() -> dict:
@@ -1213,25 +1194,29 @@
     Main function for the chatGPT program.
     """
     chatbot = Chatbot(
         config,
         conversation_id=config.get("conversation_id"),
         parent_id=config.get("parent_id"),
     )
+    plugins: dict[str, Recipient] = {}
+    chatbot.recipients["python"] = PythonRecipient
 
     def handle_commands(command: str) -> bool:
         if command == "!help":
             print(
                 """
             !help - Show this message
             !reset - Forget the current conversation
             !config - Show the current configuration
+            !plugins - Show the current plugins
+            !switch x - Switch to plugin x. Need to reset the conversation to ativate the plugin.
             !rollback x - Rollback the conversation (x being the number of messages to rollback)
-            !exit - Exit this program
             !setconversation - Changes the conversation
+            !exit - Exit this program
             """,
             )
         elif command == "!reset":
             chatbot.reset_chat()
             print("Chat session successfully reset.")
         elif command == "!config":
             print(json.dumps(chatbot.config, indent=4))
@@ -1264,15 +1249,37 @@
             prev_text = ""
             for data in chatbot.continue_write():
                 message = data["message"][len(prev_text) :]
                 print(message, end="", flush=True)
                 prev_text = data["message"]
             print(bcolors.ENDC)
             print()
+        elif command == "!plugins":
+            print("Plugins:")
+            for plugin, docs in chatbot.recipients.available_recipients.items():
+                print(" [x] " if plugin in plugins else " [ ] ", plugin, ": ", docs)
+            print()
+        elif command.startswith("!switch"):
+            try:
+                plugin = command.split(" ")[1]
+                if plugin in plugins:
+                    del plugins[plugin]
+                else:
+                    plugins[plugin] = chatbot.recipients[plugin]()
+                print(
+                    f"Plugin {plugin} has been "
+                    + ("enabled" if plugin in plugins else "disabled"),
+                )
+                print()
+            except IndexError:
+                log.exception("Please include plugin name in command")
+                print("Please include plugin name in command")
         elif command == "!exit":
+            if isinstance(chatbot.session, httpx.AsyncClient):
+                chatbot.session.aclose()
             exit()
         else:
             return False
         return True
 
     session = create_session()
     completer = create_completer(
@@ -1280,34 +1287,88 @@
             "!help",
             "!reset",
             "!config",
             "!rollback",
             "!exit",
             "!setconversation",
             "!continue",
+            "!plugins",
+            "!switch",
         ],
     )
     print()
     try:
+        msg = {}
+        result = {}
+        times = 0
         while True:
-            print(f"{bcolors.OKBLUE + bcolors.BOLD}You: {bcolors.ENDC}")
+            if not msg:
+                times = 0
+                print(f"{bcolors.OKBLUE + bcolors.BOLD}You: {bcolors.ENDC}")
 
-            prompt = get_input(session=session, completer=completer)
-            if prompt.startswith("!") and handle_commands(prompt):
-                continue
+                prompt = get_input(session=session, completer=completer)
+                if prompt.startswith("!") and handle_commands(prompt):
+                    continue
+                if not chatbot.conversation_id and plugins:
+                    prompt = (
+                        (
+                            f"""You are ChatGPT.
+
+Knowledge cutoff: 2021-09
+Current date: {datetime.datetime.now().strftime("%Y-%m-%d")}
+
+###Available Tools:
+"""
+                            + ";".join(plugins)
+                            + "\n\n"
+                            + "\n\n".join([i.API_DOCS for i in plugins.values()])
+                        )
+                        + "\n\n\n\n"
+                        + prompt
+                    )
+                msg = {
+                    "id": str(uuid.uuid4()),
+                    "author": {"role": "user"},
+                    "content": {"content_type": "text", "parts": [prompt]},
+                }
+            else:
+                print(
+                    f"{bcolors.OKCYAN + bcolors.BOLD}{result['recipient'] if result['recipient'] != 'user' else 'You'}: {bcolors.ENDC}",
+                )
+                print(msg["content"]["parts"][0])
 
             print()
             print(f"{bcolors.OKGREEN + bcolors.BOLD}Chatbot: {bcolors.ENDC}")
             prev_text = ""
-            for data in chatbot.ask(prompt, auto_continue=True):
+            for data in chatbot.post_messages([msg], auto_continue=True):
+                result = data
                 message = data["message"][len(prev_text) :]
                 print(message, end="", flush=True)
                 prev_text = data["message"]
             print(bcolors.ENDC)
             print()
+
+            msg = {}
+            if not result.get("end_turn", True):
+                times += 1
+                if times >= 5:
+                    continue
+                api = plugins.get(result["recipient"], None)
+                if not api:
+                    msg = {
+                        "id": str(uuid.uuid4()),
+                        "author": {"role": "user"},
+                        "content": {
+                            "content_type": "text",
+                            "parts": [f"Error: No plugin {result['recipient']} found"],
+                        },
+                    }
+                    continue
+                msg = api.process(result)
+
     except (KeyboardInterrupt, EOFError):
         exit()
     except Exception as exc:
         error = t.CLIError("command line program unknown error")
         raise error from exc
```

### Comparing `revChatGPT-4.2.5/src/revChatGPT/V3.py` & `revChatGPT-5.0.0/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.5/src/revChatGPT/__main__.py` & `revChatGPT-5.0.0/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.5/src/revChatGPT/config/enable_internet.json` & `revChatGPT-5.0.0/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.5/src/revChatGPT/typings.py` & `revChatGPT-5.0.0/src/revChatGPT/typings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-from os import getenv
-from platform import python_version_tuple
-Any = object()
-
-SUPPORT_ADD_NOTES = [int(each) for each in python_version_tuple()][0] >= 3 and [
-    int(each) for each in python_version_tuple()
-][1] >= 11
-del python_version_tuple
+"""
+A module that contains all the types used in this project
+"""
+import os
+from enum import Enum
+from typing import Union
+
+
+SUPPORT_ADD_NOTES = [
+    int(each) for each in __import__("platform").python_version_tuple()
+][0] >= 3 and [int(each) for each in __import__("platform").python_version_tuple()][
+    1
+] >= 11
 
 
 class ChatbotError(Exception):
     """
     Base class for all Chatbot errors in this Project
     """
 
@@ -18,25 +23,21 @@
             super().add_note(
                 "Please check that the input is correct, or you can resolve this issue by filing an issue",
             )
             super().add_note("Project URL: https://github.com/acheong08/ChatGPT")
         super().__init__(*args)
 
 
-class MetaNotAllowInstance(type):
-    """
-    Metaclass that do not allow classes to be instantiated
+class ActionError(ChatbotError):
     """
+    Subclass of ChatbotError
 
-    def __call__(cls, *args: Any, **kwargs: Any) -> Any:
-        error = ActionNotAllowedError("This class is not allowed to be instantiated")
-        raise error
-
+    An object that throws an error because the execution of an operation is blocked
+    """
 
-class ActionError(ChatbotError):
     def __init__(self, *args: object) -> None:
         if SUPPORT_ADD_NOTES:
             super().add_note(
                 "The current operation is not allowed, which may be intentional",
             )
         super().__init__(*args)
 
@@ -44,49 +45,63 @@
 class ActionNotAllowedError(ActionError):
     """
     Subclass of ActionError
 
     An object that throws an error because the execution of an unalloyed operation is blocked
     """
 
-    pass
-
 
 class ActionRefuseError(ActionError):
-    pass
+    """
+    Subclass of ActionError
+
+    An object that throws an error because the execution of a refused operation is blocked.
+    """
 
 
 class CLIError(ChatbotError):
     """
     Subclass of ChatbotError
 
     The error caused by a CLI program error
     """
 
-    pass
+
+class ErrorType(Enum):
+    """
+    Enumeration class for different types of errors.
+    """
+
+    USER_ERROR = -1
+    UNKNOWN_ERROR = 0
+    SERVER_ERROR = 1
+    RATE_LIMIT_ERROR = 2
+    INVALID_REQUEST_ERROR = 3
+    EXPIRED_ACCESS_TOKEN_ERROR = 4
+    INVALID_ACCESS_TOKEN_ERROR = 5
+    PROHIBITED_CONCURRENT_QUERY_ERROR = 6
+    AUTHENTICATION_ERROR = 7
+    CLOUDFLARE_ERROR = 8
 
 
 class Error(ChatbotError):
     """
     Base class for exceptions in V1 module.
-    Error codes:
-    -1: User error
-    0: Unknown error
-    1: Server error
-    2: Rate limit error
-    3: Invalid request error
-    4: Expired access token error
-    5: Invalid access token error
-    6: Prohibited concurrent query error
     """
 
-    def __init__(self, source: str, message: str, code: int = 0, *args: object) -> None:
+    def __init__(
+        self,
+        source: str,
+        message: str,
+        *args: object,
+        code: Union[ErrorType, int] = ErrorType.UNKNOWN_ERROR,
+    ) -> None:
         self.source: str = source
         self.message: str = message
-        self.code: int = code
+        self.code: ErrorType | int = code
         super().__init__(*args)
 
     def __str__(self) -> str:
         return f"{self.source}: {self.message} (code: {self.code})"
 
     def __repr__(self) -> str:
         return f"{self.source}: {self.message} (code: {self.code})"
@@ -107,15 +122,16 @@
         super().__init__(*args)
 
 
 class APIConnectionError(ChatbotError):
     """
     Subclass of ChatbotError
 
-    An exception object thrown when an API connection fails or fails to connect due to network or other miscellaneous reasons
+    An exception object thrown when an API connection fails or fails to connect due to network or
+    other miscellaneous reasons
     """
 
     def __init__(self, *args: object) -> None:
         if SUPPORT_ADD_NOTES:
             super().add_note(
                 "Please check if there is a problem with your network connection",
             )
@@ -125,61 +141,39 @@
 class NotAllowRunning(ActionNotAllowedError):
     """
     Subclass of ActionNotAllowedError
 
     Direct startup is not allowed for some reason
     """
 
-    def __init__(self, *args: object) -> None:
-        super().__init__(*args)
-
 
 class ResponseError(APIConnectionError):
     """
     Subclass of APIConnectionError
 
     Error objects caused by API request errors due to network or other miscellaneous reasons
     """
 
-    pass
-
 
 class OpenAIError(APIConnectionError):
     """
     Subclass of APIConnectionError
 
     Error objects caused by OpenAI's own server errors
     """
 
-    pass
-
 
 class RequestError(APIConnectionError):
     """
     Subclass of APIConnectionError
 
-    There is a problem with the API response due to network or other miscellaneous reasons, or there is no reply to the object that caused the error at all
+    There is a problem with the API response due to network or other miscellaneous reasons, or there
+    is no reply to the object that caused the error at all
     """
 
-    pass
-
-
-class ErrorType(metaclass=MetaNotAllowInstance):
-    # define consts for the error codes
-    USER_ERROR = -1
-    UNKNOWN_ERROR = 0
-    SERVER_ERROR = 1
-    RATE_LIMIT_ERROR = 2
-    INVALID_REQUEST_ERROR = 3
-    EXPIRED_ACCESS_TOKEN_ERROR = 4
-    INVALID_ACCESS_TOKEN_ERROR = 5
-    PROHIBITED_CONCURRENT_QUERY_ERROR = 6
-    AUTHENTICATION_ERROR = 7
-    CLOUDFLARE_ERROR = 8
-
 
 class Colors:
     """
     Colors for printing
     """
 
     HEADER = "\033[95m"
@@ -189,17 +183,17 @@
     WARNING = "\033[93m"
     FAIL = "\033[91m"
     ENDC = "\033[0m"
     BOLD = "\033[1m"
     UNDERLINE = "\033[4m"
 
     def __init__(self) -> None:
-        if getenv("NO_COLOR"):
-            self.HEADER = ""
-            self.OKBLUE = ""
-            self.OKCYAN = ""
-            self.OKGREEN = ""
-            self.WARNING = ""
-            self.FAIL = ""
-            self.ENDC = ""
-            self.BOLD = ""
-            self.UNDERLINE = ""
+        if os.getenv("NO_COLOR"):
+            Colors.HEADER = ""
+            Colors.OKBLUE = ""
+            Colors.OKCYAN = ""
+            Colors.OKGREEN = ""
+            Colors.WARNING = ""
+            Colors.FAIL = ""
+            Colors.ENDC = ""
+            Colors.BOLD = ""
+            Colors.UNDERLINE = ""
```

### Comparing `revChatGPT-4.2.5/src/revChatGPT/utils.py` & `revChatGPT-5.0.0/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.5/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-5.0.0/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.2.5
+Version: 5.0.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -48,15 +48,15 @@
 
 ### Suport Python Version
 
 - Minimum - Python3.9
 - Recommend - Python3.11+
 
 <details>
-  
+
   <summary>
 
 # V1 Standard ChatGPT
 
 Due to recent tightening of OpenAI's security, the default endpoint has been swapped over to one provided by @pengzhile. It is not open source and privacy is not guarenteed. Use it at your own risk. I am working on an open source implementation with the latest changes but that could take a while.
 
 </summary>
@@ -169,15 +169,15 @@
 
 #### All API methods
 
 Refer to the [wiki](https://github.com/acheong08/ChatGPT/wiki/) for advanced developer usage.
 
 </details>
 
-<summary>  
+<summary>
 
 # V3 Official Chat API
 
 > Recently released by OpenAI
 >
 > - Paid
```

