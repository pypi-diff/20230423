# Comparing `tmp/gptroles-0.1.4.tar.gz` & `tmp/gptroles-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptroles-0.1.4.tar", max compression
+gzip compressed data, was "gptroles-0.1.5.tar", max compression
```

## Comparing `gptroles-0.1.4.tar` & `gptroles-0.1.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     2137 2023-04-01 03:07:06.030934 gptroles-0.1.4/README.md
--rw-r--r--   0        0        0     1416 2023-04-15 05:27:01.167116 gptroles-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-25 07:27:32.555216 gptroles-0.1.4/src/gptroles/__init__.py
--rw-r--r--   0        0        0     8227 2023-04-15 05:23:51.694822 gptroles-0.1.4/src/gptroles/gpt.py
--rwxr-xr-x   0        0        0      362 2023-03-27 06:58:42.730588 gptroles-0.1.4/src/gptroles/main.py
--rw-r--r--   0        0        0     4291 2023-04-15 05:05:52.057413 gptroles-0.1.4/src/gptroles/prompts.py
--rw-r--r--   0        0        0     2691 2023-03-30 03:55:23.236618 gptroles-0.1.4/src/gptroles/settings.py
--rw-r--r--   0        0        0     2548 2023-03-26 11:35:18.704005 gptroles-0.1.4/src/gptroles/ui/__init__.py
--rw-r--r--   0        0        0     3964 2023-03-22 00:43:25.483064 gptroles-0.1.4/src/gptroles/ui/indicator.py
--rw-r--r--   0        0        0     7865 2023-03-29 02:53:12.335631 gptroles-0.1.4/src/gptroles/ui/mainwindow.py
--rw-r--r--   0        0        0     5694 2023-03-27 08:49:54.163978 gptroles-0.1.4/src/gptroles/ui/settings.py
--rw-r--r--   0        0        0      400 2023-03-26 09:51:13.621608 gptroles-0.1.4/src/gptroles/ui/utils.py
--rw-r--r--   0        0        0      228 2023-03-27 00:46:15.259885 gptroles-0.1.4/src/gptroles/ui/web/.parcelrc
--rw-r--r--   0        0        0     2009 2023-04-16 13:41:20.468421 gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.153c3a09.css
--rw-r--r--   0        0        0     7750 2023-04-16 13:41:20.488421 gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.153c3a09.css.map
--rw-r--r--   0        0        0    49775 2023-04-16 13:41:20.471754 gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.17936317.js
--rw-r--r--   0        0        0   101157 2023-04-16 13:41:20.508421 gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.17936317.js.map
--rw-r--r--   0        0        0   119598 2023-04-16 13:41:20.471754 gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.1ee3acf6.js
--rw-r--r--   0        0        0   235444 2023-04-16 13:41:20.508421 gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.1ee3acf6.js.map
--rw-r--r--   0        0        0     1225 2023-04-16 13:41:20.468421 gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.28944a1e.css
--rw-r--r--   0        0        0     3155 2023-04-16 13:41:20.485088 gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.28944a1e.css.map
--rw-r--r--   0        0        0     2904 2023-04-16 13:41:20.468421 gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.3361cb26.css
--rw-r--r--   0        0        0     9300 2023-04-16 13:41:20.485088 gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.3361cb26.css.map
--rw-r--r--   0        0        0   306402 2023-04-16 13:41:20.471754 gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.5d2f6e12.js
--rw-r--r--   0        0        0  1180907 2023-04-16 13:41:20.508421 gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.5d2f6e12.js.map
--rw-r--r--   0        0        0     2623 2023-04-16 13:41:20.468421 gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.html
--rw-r--r--   0        0        0     1339 2023-04-16 13:41:20.518421 gptroles-0.1.4/src/gptroles/ui/web/dist/highlight.min.css
--rw-r--r--   0        0        0   125548 2023-04-16 13:41:20.521754 gptroles-0.1.4/src/gptroles/ui/web/dist/highlight.min.js
--rw-r--r--   0        0        0    49718 2023-04-16 13:41:20.521754 gptroles-0.1.4/src/gptroles/ui/web/dist/marked.min.js
--rw-r--r--   0        0        0   176522 2023-03-27 00:13:54.460535 gptroles-0.1.4/src/gptroles/ui/web/package-lock.json
--rw-r--r--   0        0        0     1000 2023-03-27 08:05:28.938604 gptroles-0.1.4/src/gptroles/ui/web/package.json
--rwxr-xr-x   0        0        0       11 2023-03-27 00:46:30.043137 gptroles-0.1.4/src/gptroles/ui/web/package.sh
--rwxr-xr-x   0        0        0       73 2023-03-27 01:00:04.668667 gptroles-0.1.4/src/gptroles/ui/web/postpackage.sh
--rw-r--r--   0        0        0   561154 2023-03-27 00:17:37.279312 gptroles-0.1.4/src/gptroles/ui/web/release.zip
--rw-r--r--   0        0        0     3284 2023-03-27 08:34:53.138923 gptroles-0.1.4/src/gptroles/ui/web/src/chatpage.html
--rw-r--r--   0        0        0    12708 2023-04-15 05:27:55.596817 gptroles-0.1.4/src/gptroles/ui/web/src/index.js
--rw-r--r--   0        0        0     1339 2023-03-24 05:56:45.666620 gptroles-0.1.4/src/gptroles/ui/web/src/static/highlight.min.css
--rw-r--r--   0        0        0   125548 2023-03-24 04:28:37.005641 gptroles-0.1.4/src/gptroles/ui/web/src/static/highlight.min.js
--rw-r--r--   0        0        0    49718 2023-03-24 03:18:19.065454 gptroles-0.1.4/src/gptroles/ui/web/src/static/marked.min.js
--rw-r--r--   0        0        0     4738 2023-04-01 03:05:20.124849 gptroles-0.1.4/src/gptroles/ui/web/src/style.css
--rw-r--r--   0        0        0     1687 2023-03-27 03:17:53.649958 gptroles-0.1.4/src/gptroles/ui/web/src/term.js
--rw-r--r--   0        0        0        0 2023-03-27 03:48:29.829882 gptroles-0.1.4/src/gptroles/ui/widgets/__init__.py
--rw-r--r--   0        0        0     1820 2023-03-27 07:09:19.593760 gptroles-0.1.4/src/gptroles/ui/widgets/borderlesswindow.py
--rw-r--r--   0        0        0    11535 2023-03-30 04:22:13.364449 gptroles-0.1.4/src/gptroles/ui/widgets/chatbox.py
--rw-r--r--   0        0        0      241 2023-03-26 11:35:08.187396 gptroles-0.1.4/src/gptroles/ui/widgets/chatmsg.py
--rw-r--r--   0        0        0     3052 2023-03-30 04:27:37.789336 gptroles-0.1.4/src/gptroles/ui/widgets/netprompts.py
--rw-r--r--   0        0        0     8038 2023-03-27 04:56:22.120869 gptroles-0.1.4/src/gptroles/ui/widgets/nterminal.py
--rw-r--r--   0        0        0     3690 2023-03-27 04:32:05.015531 gptroles-0.1.4/src/gptroles/ui/widgets/terminal/__init__.py
--rw-r--r--   0        0        0     1447 2023-03-27 04:25:00.374528 gptroles-0.1.4/src/gptroles/ui/widgets/terminal/console.py
--rw-r--r--   0        0        0     7827 2023-03-27 04:22:25.575378 gptroles-0.1.4/src/gptroles/ui/widgets/terminal/settingsdialog.py
--rw-r--r--   0        0        0     1456 2023-03-24 07:44:48.051048 gptroles-0.1.4/src/gptroles/utils.py
--rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 gptroles-0.1.4/setup.py
--rw-r--r--   0        0        0     3142 1970-01-01 00:00:00.000000 gptroles-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2137 2023-04-01 03:07:06.030934 gptroles-0.1.5/README.md
+-rw-r--r--   0        0        0     1416 2023-04-23 16:29:39.873116 gptroles-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-25 07:27:32.555216 gptroles-0.1.5/src/gptroles/__init__.py
+-rw-r--r--   0        0        0     8244 2023-04-23 16:29:04.273311 gptroles-0.1.5/src/gptroles/gpt.py
+-rwxr-xr-x   0        0        0      362 2023-03-27 06:58:42.730588 gptroles-0.1.5/src/gptroles/main.py
+-rw-r--r--   0        0        0     4291 2023-04-15 05:05:52.057413 gptroles-0.1.5/src/gptroles/prompts.py
+-rw-r--r--   0        0        0     2691 2023-03-30 03:55:23.236618 gptroles-0.1.5/src/gptroles/settings.py
+-rw-r--r--   0        0        0     2548 2023-03-26 11:35:18.704005 gptroles-0.1.5/src/gptroles/ui/__init__.py
+-rw-r--r--   0        0        0     3964 2023-03-22 00:43:25.483064 gptroles-0.1.5/src/gptroles/ui/indicator.py
+-rw-r--r--   0        0        0     7865 2023-03-29 02:53:12.335631 gptroles-0.1.5/src/gptroles/ui/mainwindow.py
+-rw-r--r--   0        0        0     5694 2023-03-27 08:49:54.163978 gptroles-0.1.5/src/gptroles/ui/settings.py
+-rw-r--r--   0        0        0      400 2023-03-26 09:51:13.621608 gptroles-0.1.5/src/gptroles/ui/utils.py
+-rw-r--r--   0        0        0      228 2023-03-27 00:46:15.259885 gptroles-0.1.5/src/gptroles/ui/web/.parcelrc
+-rw-r--r--   0        0        0     2009 2023-04-23 16:30:51.036059 gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.153c3a09.css
+-rw-r--r--   0        0        0     7750 2023-04-23 16:30:51.056059 gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.153c3a09.css.map
+-rw-r--r--   0        0        0    49775 2023-04-23 16:30:51.036059 gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.17936317.js
+-rw-r--r--   0        0        0   101157 2023-04-23 16:30:51.086058 gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.17936317.js.map
+-rw-r--r--   0        0        0   119598 2023-04-23 16:30:51.039392 gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.1ee3acf6.js
+-rw-r--r--   0        0        0   235444 2023-04-23 16:30:51.089392 gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.1ee3acf6.js.map
+-rw-r--r--   0        0        0     1225 2023-04-23 16:30:51.036059 gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.28944a1e.css
+-rw-r--r--   0        0        0     3155 2023-04-23 16:30:51.062725 gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.28944a1e.css.map
+-rw-r--r--   0        0        0     2904 2023-04-23 16:30:51.036059 gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.3361cb26.css
+-rw-r--r--   0        0        0     9300 2023-04-23 16:30:51.052725 gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.3361cb26.css.map
+-rw-r--r--   0        0        0   306402 2023-04-23 16:30:51.039392 gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.5d2f6e12.js
+-rw-r--r--   0        0        0  1180907 2023-04-23 16:30:51.089392 gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.5d2f6e12.js.map
+-rw-r--r--   0        0        0     2623 2023-04-23 16:30:51.032725 gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.html
+-rw-r--r--   0        0        0     1339 2023-04-23 16:30:51.102725 gptroles-0.1.5/src/gptroles/ui/web/dist/highlight.min.css
+-rw-r--r--   0        0        0   125548 2023-04-23 16:30:51.102725 gptroles-0.1.5/src/gptroles/ui/web/dist/highlight.min.js
+-rw-r--r--   0        0        0    49718 2023-04-23 16:30:51.106058 gptroles-0.1.5/src/gptroles/ui/web/dist/marked.min.js
+-rw-r--r--   0        0        0   176522 2023-03-27 00:13:54.460535 gptroles-0.1.5/src/gptroles/ui/web/package-lock.json
+-rw-r--r--   0        0        0     1000 2023-03-27 08:05:28.938604 gptroles-0.1.5/src/gptroles/ui/web/package.json
+-rwxr-xr-x   0        0        0       11 2023-03-27 00:46:30.043137 gptroles-0.1.5/src/gptroles/ui/web/package.sh
+-rwxr-xr-x   0        0        0       73 2023-03-27 01:00:04.668667 gptroles-0.1.5/src/gptroles/ui/web/postpackage.sh
+-rw-r--r--   0        0        0   561154 2023-03-27 00:17:37.279312 gptroles-0.1.5/src/gptroles/ui/web/release.zip
+-rw-r--r--   0        0        0     3284 2023-03-27 08:34:53.138923 gptroles-0.1.5/src/gptroles/ui/web/src/chatpage.html
+-rw-r--r--   0        0        0    12708 2023-04-15 05:27:55.596817 gptroles-0.1.5/src/gptroles/ui/web/src/index.js
+-rw-r--r--   0        0        0     1339 2023-03-24 05:56:45.666620 gptroles-0.1.5/src/gptroles/ui/web/src/static/highlight.min.css
+-rw-r--r--   0        0        0   125548 2023-03-24 04:28:37.005641 gptroles-0.1.5/src/gptroles/ui/web/src/static/highlight.min.js
+-rw-r--r--   0        0        0    49718 2023-03-24 03:18:19.065454 gptroles-0.1.5/src/gptroles/ui/web/src/static/marked.min.js
+-rw-r--r--   0        0        0     4738 2023-04-01 03:05:20.124849 gptroles-0.1.5/src/gptroles/ui/web/src/style.css
+-rw-r--r--   0        0        0     1687 2023-03-27 03:17:53.649958 gptroles-0.1.5/src/gptroles/ui/web/src/term.js
+-rw-r--r--   0        0        0        0 2023-03-27 03:48:29.829882 gptroles-0.1.5/src/gptroles/ui/widgets/__init__.py
+-rw-r--r--   0        0        0     1820 2023-03-27 07:09:19.593760 gptroles-0.1.5/src/gptroles/ui/widgets/borderlesswindow.py
+-rw-r--r--   0        0        0    11535 2023-03-30 04:22:13.364449 gptroles-0.1.5/src/gptroles/ui/widgets/chatbox.py
+-rw-r--r--   0        0        0      241 2023-03-26 11:35:08.187396 gptroles-0.1.5/src/gptroles/ui/widgets/chatmsg.py
+-rw-r--r--   0        0        0     3052 2023-03-30 04:27:37.789336 gptroles-0.1.5/src/gptroles/ui/widgets/netprompts.py
+-rw-r--r--   0        0        0     8038 2023-03-27 04:56:22.120869 gptroles-0.1.5/src/gptroles/ui/widgets/nterminal.py
+-rw-r--r--   0        0        0     3690 2023-03-27 04:32:05.015531 gptroles-0.1.5/src/gptroles/ui/widgets/terminal/__init__.py
+-rw-r--r--   0        0        0     1447 2023-03-27 04:25:00.374528 gptroles-0.1.5/src/gptroles/ui/widgets/terminal/console.py
+-rw-r--r--   0        0        0     7827 2023-03-27 04:22:25.575378 gptroles-0.1.5/src/gptroles/ui/widgets/terminal/settingsdialog.py
+-rw-r--r--   0        0        0     1456 2023-03-24 07:44:48.051048 gptroles-0.1.5/src/gptroles/utils.py
+-rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 gptroles-0.1.5/setup.py
+-rw-r--r--   0        0        0     3142 1970-01-01 00:00:00.000000 gptroles-0.1.5/PKG-INFO
```

### Comparing `gptroles-0.1.4/README.md` & `gptroles-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/pyproject.toml` & `gptroles-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gptroles"
-version = "0.1.4"
+version = "0.1.5"
 description = "Interact with chatgpt and assign different roles"
 authors = [
     "Blipk A.D."
 ]
 homepage = "https://github.com/blipk/gptroles"
 repository = "https://github.com/blipk/gptroles"
 documentation = "https://github.com/blipk/gptroles"
```

### Comparing `gptroles-0.1.4/src/gptroles/gpt.py` & `gptroles-0.1.5/src/gptroles/gpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
             return ("Error", str(e))
         except openai.APIError as e:
             print("API", e)
             return ("Error", str(e))
         except openai.InvalidRequestError as e:
             print(e)
             if "maximum context length" in e._message:
-                if len(prompt_chain) == 0:
+                if prompt_chain and len(prompt_chain) == 0:
                     return ("Error", str(e))
                 return self.ask(prompt, prompt_chain, message_role, trim=trim+1)
             else:
                 print(e)
                 return ("Error", str(e))
         self.history.add_ai_message(answer)
```

### Comparing `gptroles-0.1.4/src/gptroles/prompts.py` & `gptroles-0.1.5/src/gptroles/prompts.py`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/settings.py` & `gptroles-0.1.5/src/gptroles/settings.py`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/__init__.py` & `gptroles-0.1.5/src/gptroles/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/indicator.py` & `gptroles-0.1.5/src/gptroles/ui/indicator.py`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/mainwindow.py` & `gptroles-0.1.5/src/gptroles/ui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/settings.py` & `gptroles-0.1.5/src/gptroles/ui/settings.py`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.153c3a09.css` & `gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.153c3a09.css`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.153c3a09.css.map` & `gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.153c3a09.css.map`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.17936317.js` & `gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.17936317.js`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.17936317.js.map` & `gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.17936317.js.map`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.1ee3acf6.js` & `gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.1ee3acf6.js`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.1ee3acf6.js.map` & `gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.1ee3acf6.js.map`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.28944a1e.css` & `gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.28944a1e.css`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.28944a1e.css.map` & `gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.28944a1e.css.map`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.3361cb26.css` & `gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.3361cb26.css`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.3361cb26.css.map` & `gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.3361cb26.css.map`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.5d2f6e12.js` & `gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.5d2f6e12.js`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.5d2f6e12.js.map` & `gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.5d2f6e12.js.map`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/dist/chatpage.html` & `gptroles-0.1.5/src/gptroles/ui/web/dist/chatpage.html`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/dist/highlight.min.css` & `gptroles-0.1.5/src/gptroles/ui/web/dist/highlight.min.css`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/dist/highlight.min.js` & `gptroles-0.1.5/src/gptroles/ui/web/dist/highlight.min.js`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/dist/marked.min.js` & `gptroles-0.1.5/src/gptroles/ui/web/dist/marked.min.js`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/package-lock.json` & `gptroles-0.1.5/src/gptroles/ui/web/package-lock.json`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/package.json` & `gptroles-0.1.5/src/gptroles/ui/web/package.json`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/release.zip` & `gptroles-0.1.5/src/gptroles/ui/web/release.zip`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/src/chatpage.html` & `gptroles-0.1.5/src/gptroles/ui/web/src/chatpage.html`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/src/index.js` & `gptroles-0.1.5/src/gptroles/ui/web/src/index.js`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/src/static/highlight.min.css` & `gptroles-0.1.5/src/gptroles/ui/web/src/static/highlight.min.css`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/src/static/highlight.min.js` & `gptroles-0.1.5/src/gptroles/ui/web/src/static/highlight.min.js`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/src/static/marked.min.js` & `gptroles-0.1.5/src/gptroles/ui/web/src/static/marked.min.js`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/src/style.css` & `gptroles-0.1.5/src/gptroles/ui/web/src/style.css`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/web/src/term.js` & `gptroles-0.1.5/src/gptroles/ui/web/src/term.js`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/widgets/borderlesswindow.py` & `gptroles-0.1.5/src/gptroles/ui/widgets/borderlesswindow.py`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/widgets/chatbox.py` & `gptroles-0.1.5/src/gptroles/ui/widgets/chatbox.py`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/widgets/netprompts.py` & `gptroles-0.1.5/src/gptroles/ui/widgets/netprompts.py`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/widgets/nterminal.py` & `gptroles-0.1.5/src/gptroles/ui/widgets/nterminal.py`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/widgets/terminal/__init__.py` & `gptroles-0.1.5/src/gptroles/ui/widgets/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/widgets/terminal/console.py` & `gptroles-0.1.5/src/gptroles/ui/widgets/terminal/console.py`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/ui/widgets/terminal/settingsdialog.py` & `gptroles-0.1.5/src/gptroles/ui/widgets/terminal/settingsdialog.py`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/src/gptroles/utils.py` & `gptroles-0.1.5/src/gptroles/utils.py`

 * *Files identical despite different names*

### Comparing `gptroles-0.1.4/setup.py` & `gptroles-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 entry_points = \
 {'console_scripts': ['devtest = mypackage:test.run_tests',
                      'main = gptroles.main:main']}
 
 setup_kwargs = {
     'name': 'gptroles',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Interact with chatgpt and assign different roles',
     'long_description': '\n## GPT Roles\nSimple PyQT chatbox that connects to a chat session with ChatGPT, along with some extra desktop integration features.\n\nWritten as an experiment with Qt and understanding the role of LLMs in virtual assistant applications.\n\n![Screenshot of GPT Roles](doc/screenshot.png)\n![Demo video of GPT Roles](doc/demo.webm)\n\n#### Roleplayer\nIt has a "roleplaying" root prompt that attempts to make implementing more roles into ChatGPT easier.\nYou can add "roles" to the root prompt, by default there are some roles related to commands and programming.\n\nYou can also change the root prompt to something else entirely, there\'s a list of some prompts that are sourced online, see features.\n\n###### Command Role\n\nNot fully implemented\n\n    - RoleGPT can request web pages or from APIs to answer your questions.\n        e.g. get current prices or latest news.\n    - Provide basic shell commands that will be automatically be run, to find or list files etc\n    - Instructions to format markdown for the programming features\n\n#### App Features\n\nProgramming related features:\n\n    - Run shell or python code in markdown blocks directly in the chat interface\n    - Edit the markdown blocks in the chat box\n    - Copy or save markdown blocks to a file\n\nAdditional features:\n\n    - Easily switch or add more "roles"\n    - Remove the roleplaying root prompt and set it as you please\n    - List roles from jailbreakchat.com and set them as the root prompt\n\nChat related features:\n\n    - TODO Shows which messages are in the current prompt chain and can be added/removed\n    - TODO Show alternate choices and commit to conversation\n\n\n#### Installing/Running\n\n###### From pip\nInstall the module and install desktop launcher integration:\n\n`pip install gptroles && ./install.sh`\n\n\n###### From source with Poetry\n```shell\npoetry install && poetry run main\n```\n\n###### Packaged AppImage/PyInstaller\n\n`TODO`\n\n###### Development installation\n\nUse the `dev.sh` script.\n\n```shell\n# This only needs to be run once\n./dev.sh build && ./dev.sh sysinstall && ./dev.sh install\n\n# Then you can run with the install and dev environment matching code\n./dev.sh run\n```',
     'author': 'Blipk A.D.',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/blipk/gptroles',
```

### Comparing `gptroles-0.1.4/PKG-INFO` & `gptroles-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptroles
-Version: 0.1.4
+Version: 0.1.5
 Summary: Interact with chatgpt and assign different roles
 Home-page: https://github.com/blipk/gptroles
 License: MIT
 Keywords: gptroles,ChatGPT,GPT,LLM,ML
 Author: Blipk A.D.
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

