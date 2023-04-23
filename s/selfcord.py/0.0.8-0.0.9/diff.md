# Comparing `tmp/selfcord.py-0.0.8.tar.gz` & `tmp/selfcord.py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcord.py-0.0.8.tar", last modified: Sun Nov 27 03:04:25 2022, max compression
+gzip compressed data, was "selfcord.py-0.0.9.tar", last modified: Sun Nov 27 20:34:13 2022, max compression
```

## Comparing `selfcord.py-0.0.8.tar` & `selfcord.py-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 03:04:25.555037 selfcord.py-0.0.8/
--rw-r--r--   0 shell     (1000) shell     (1001)     2338 2022-11-27 03:04:25.551704 selfcord.py-0.0.8/PKG-INFO
--rw-r--r--   0 shell     (1000) shell     (1001)     2050 2022-11-20 03:11:59.000000 selfcord.py-0.0.8/README.md
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 03:04:25.545037 selfcord.py-0.0.8/selfcord/
--rw-r--r--   0 shell     (1000) shell     (1001)       82 2022-11-11 20:03:04.000000 selfcord.py-0.0.8/selfcord/__init__.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 03:04:25.548370 selfcord.py-0.0.8/selfcord/api/
--rw-r--r--   0 shell     (1000) shell     (1001)      127 2022-11-11 20:02:32.000000 selfcord.py-0.0.8/selfcord/api/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)      527 2022-11-11 01:44:22.000000 selfcord.py-0.0.8/selfcord/api/errors.py
--rw-r--r--   0 shell     (1000) shell     (1001)     7824 2022-11-11 01:44:22.000000 selfcord.py-0.0.8/selfcord/api/events.py
--rw-r--r--   0 shell     (1000) shell     (1001)    14476 2022-11-24 14:11:05.000000 selfcord.py-0.0.8/selfcord/api/gateway.py
--rw-r--r--   0 shell     (1000) shell     (1001)     7642 2022-11-24 14:12:34.000000 selfcord.py-0.0.8/selfcord/api/http.py
--rw-r--r--   0 shell     (1000) shell     (1001)    13164 2022-11-27 03:02:07.000000 selfcord.py-0.0.8/selfcord/bot.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 03:04:25.551704 selfcord.py-0.0.8/selfcord/models/
--rw-r--r--   0 shell     (1000) shell     (1001)      412 2022-11-21 22:16:05.000000 selfcord.py-0.0.8/selfcord/models/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)    13093 2022-11-24 14:12:20.000000 selfcord.py-0.0.8/selfcord/models/channel.py
--rw-r--r--   0 shell     (1000) shell     (1001)      902 2022-11-21 18:38:16.000000 selfcord.py-0.0.8/selfcord/models/client.py
--rw-r--r--   0 shell     (1000) shell     (1001)      697 2022-10-31 21:14:11.000000 selfcord.py-0.0.8/selfcord/models/emoji.py
--rw-r--r--   0 shell     (1000) shell     (1001)     5149 2022-11-21 17:56:07.000000 selfcord.py-0.0.8/selfcord/models/guild.py
--rw-r--r--   0 shell     (1000) shell     (1001)      783 2022-11-21 18:38:32.000000 selfcord.py-0.0.8/selfcord/models/member.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1558 2022-11-17 17:14:15.000000 selfcord.py-0.0.8/selfcord/models/message.py
--rw-r--r--   0 shell     (1000) shell     (1001)     2125 2022-10-18 15:17:31.000000 selfcord.py-0.0.8/selfcord/models/permission.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1360 2022-11-22 16:33:43.000000 selfcord.py-0.0.8/selfcord/models/role.py
--rw-r--r--   0 shell     (1000) shell     (1001)     2993 2022-11-21 18:40:17.000000 selfcord.py-0.0.8/selfcord/models/user.py
--rw-r--r--   0 shell     (1000) shell     (1001)      999 2022-10-25 00:32:59.000000 selfcord.py-0.0.8/selfcord/models/webhook.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 03:04:25.551704 selfcord.py-0.0.8/selfcord/utils/
--rw-r--r--   0 shell     (1000) shell     (1001)      150 2022-11-27 03:03:09.000000 selfcord.py-0.0.8/selfcord/utils/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)    12664 2022-11-24 15:50:53.000000 selfcord.py-0.0.8/selfcord/utils/command.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 03:04:25.548370 selfcord.py-0.0.8/selfcord.py.egg-info/
--rw-r--r--   0 shell     (1000) shell     (1001)     2338 2022-11-27 03:04:25.000000 selfcord.py-0.0.8/selfcord.py.egg-info/PKG-INFO
--rw-r--r--   0 shell     (1000) shell     (1001)      687 2022-11-27 03:04:25.000000 selfcord.py-0.0.8/selfcord.py.egg-info/SOURCES.txt
--rw-r--r--   0 shell     (1000) shell     (1001)        1 2022-11-27 03:04:25.000000 selfcord.py-0.0.8/selfcord.py.egg-info/dependency_links.txt
--rw-r--r--   0 shell     (1000) shell     (1001)       66 2022-11-27 03:04:25.000000 selfcord.py-0.0.8/selfcord.py.egg-info/requires.txt
--rw-r--r--   0 shell     (1000) shell     (1001)        9 2022-11-27 03:04:25.000000 selfcord.py-0.0.8/selfcord.py.egg-info/top_level.txt
--rw-r--r--   0 shell     (1000) shell     (1001)       38 2022-11-27 03:04:25.555037 selfcord.py-0.0.8/setup.cfg
--rw-r--r--   0 shell     (1000) shell     (1001)     1004 2022-11-27 03:04:23.000000 selfcord.py-0.0.8/setup.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 20:34:13.666568 selfcord.py-0.0.9/
+-rw-r--r--   0 shell     (1000) shell     (1001)     2338 2022-11-27 20:34:13.666568 selfcord.py-0.0.9/PKG-INFO
+-rw-r--r--   0 shell     (1000) shell     (1001)     2050 2022-11-20 03:11:59.000000 selfcord.py-0.0.9/README.md
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 20:34:13.653235 selfcord.py-0.0.9/selfcord/
+-rw-r--r--   0 shell     (1000) shell     (1001)       82 2022-11-11 20:03:04.000000 selfcord.py-0.0.9/selfcord/__init__.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 20:34:13.656568 selfcord.py-0.0.9/selfcord/api/
+-rw-r--r--   0 shell     (1000) shell     (1001)      127 2022-11-11 20:02:32.000000 selfcord.py-0.0.9/selfcord/api/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      527 2022-11-11 01:44:22.000000 selfcord.py-0.0.9/selfcord/api/errors.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     7824 2022-11-11 01:44:22.000000 selfcord.py-0.0.9/selfcord/api/events.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    14476 2022-11-24 14:11:05.000000 selfcord.py-0.0.9/selfcord/api/gateway.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     7642 2022-11-24 14:12:34.000000 selfcord.py-0.0.9/selfcord/api/http.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    13164 2022-11-27 03:02:07.000000 selfcord.py-0.0.9/selfcord/bot.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 20:34:13.663235 selfcord.py-0.0.9/selfcord/models/
+-rw-r--r--   0 shell     (1000) shell     (1001)      412 2022-11-21 22:16:05.000000 selfcord.py-0.0.9/selfcord/models/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    13093 2022-11-24 14:12:20.000000 selfcord.py-0.0.9/selfcord/models/channel.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      902 2022-11-21 18:38:16.000000 selfcord.py-0.0.9/selfcord/models/client.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      697 2022-10-31 21:14:11.000000 selfcord.py-0.0.9/selfcord/models/emoji.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     5149 2022-11-21 17:56:07.000000 selfcord.py-0.0.9/selfcord/models/guild.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      783 2022-11-21 18:38:32.000000 selfcord.py-0.0.9/selfcord/models/member.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1558 2022-11-17 17:14:15.000000 selfcord.py-0.0.9/selfcord/models/message.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     2125 2022-10-18 15:17:31.000000 selfcord.py-0.0.9/selfcord/models/permission.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1360 2022-11-22 16:33:43.000000 selfcord.py-0.0.9/selfcord/models/role.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     2993 2022-11-21 18:40:17.000000 selfcord.py-0.0.9/selfcord/models/user.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      999 2022-10-25 00:32:59.000000 selfcord.py-0.0.9/selfcord/models/webhook.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 20:34:13.666568 selfcord.py-0.0.9/selfcord/utils/
+-rw-r--r--   0 shell     (1000) shell     (1001)      150 2022-11-27 03:03:09.000000 selfcord.py-0.0.9/selfcord/utils/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    12664 2022-11-24 15:50:53.000000 selfcord.py-0.0.9/selfcord/utils/command.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 20:34:13.653235 selfcord.py-0.0.9/selfcord.py.egg-info/
+-rw-r--r--   0 shell     (1000) shell     (1001)     2338 2022-11-27 20:34:13.000000 selfcord.py-0.0.9/selfcord.py.egg-info/PKG-INFO
+-rw-r--r--   0 shell     (1000) shell     (1001)      687 2022-11-27 20:34:13.000000 selfcord.py-0.0.9/selfcord.py.egg-info/SOURCES.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)        1 2022-11-27 20:34:13.000000 selfcord.py-0.0.9/selfcord.py.egg-info/dependency_links.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)       75 2022-11-27 20:34:13.000000 selfcord.py-0.0.9/selfcord.py.egg-info/requires.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)        9 2022-11-27 20:34:13.000000 selfcord.py-0.0.9/selfcord.py.egg-info/top_level.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)       38 2022-11-27 20:34:13.666568 selfcord.py-0.0.9/setup.cfg
+-rw-r--r--   0 shell     (1000) shell     (1001)     1016 2022-11-27 20:34:09.000000 selfcord.py-0.0.9/setup.py
```

### Comparing `selfcord.py-0.0.8/PKG-INFO` & `selfcord.py-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell of OMEGA
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
```

### Comparing `selfcord.py-0.0.8/README.md` & `selfcord.py-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord/api/errors.py` & `selfcord.py-0.0.9/selfcord/api/errors.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord/api/events.py` & `selfcord.py-0.0.9/selfcord/api/events.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord/api/gateway.py` & `selfcord.py-0.0.9/selfcord/api/gateway.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord/api/http.py` & `selfcord.py-0.0.9/selfcord/api/http.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord/bot.py` & `selfcord.py-0.0.9/selfcord/bot.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord/models/channel.py` & `selfcord.py-0.0.9/selfcord/models/channel.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord/models/client.py` & `selfcord.py-0.0.9/selfcord/models/client.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord/models/emoji.py` & `selfcord.py-0.0.9/selfcord/models/emoji.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord/models/guild.py` & `selfcord.py-0.0.9/selfcord/models/guild.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord/models/member.py` & `selfcord.py-0.0.9/selfcord/models/member.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord/models/message.py` & `selfcord.py-0.0.9/selfcord/models/message.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord/models/permission.py` & `selfcord.py-0.0.9/selfcord/models/permission.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord/models/role.py` & `selfcord.py-0.0.9/selfcord/models/role.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord/models/user.py` & `selfcord.py-0.0.9/selfcord/models/user.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord/models/webhook.py` & `selfcord.py-0.0.9/selfcord/models/webhook.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord/utils/command.py` & `selfcord.py-0.0.9/selfcord/utils/command.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/selfcord.py.egg-info/PKG-INFO` & `selfcord.py-0.0.9/selfcord.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell of OMEGA
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
```

### Comparing `selfcord.py-0.0.8/selfcord.py.egg-info/SOURCES.txt` & `selfcord.py-0.0.9/selfcord.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.8/setup.py` & `selfcord.py-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 this_directory = Path(__file__).parent
 if __name__ == "__main__":
     this_directory = Path(__file__).parent
     long_description = ( this_directory /"README.md").read_text()
     setup(
         name="selfcord.py",
         packages=find_packages(include=['selfcord', 'selfcord.api', 'selfcord.utils', 'selfcord.models']),
-        version="0.0.8",
+        version="0.0.9",
         description="A Discord API wrapper designed for selfbots!",
         readme="README.md",
         author="Shell of OMEGA",
         license="MIT",
-        install_requires=["aiohttp==3.7.4.post0","aioconsole==0.3.3", "websockets==10.1", "importlib"],
+        install_requires=["aiohttp==3.7.4.post0","aioconsole==0.3.3", "websockets==10.1", "importlib", "requests"],
         setup_requires=['pytest-runner'],
         tests_require=['pytest'],
         test_suite='tests',
         keywords=["selfbot", "discord", "discordapi", "discordwrapper"],
         long_description=long_description,
         url="https://github.com/Shell1010/Selfcord",
         long_description_content_type="text/markdown",
```

