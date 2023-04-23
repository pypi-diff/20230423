# Comparing `tmp/promptcli-1.0.5.tar.gz` & `tmp/promptcli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptcli-1.0.5.tar", last modified: Thu Mar  9 16:07:30 2023, max compression
+gzip compressed data, was "promptcli-2.0.0.tar", last modified: Sun Apr 23 16:33:43 2023, max compression
```

## Comparing `promptcli-1.0.5.tar` & `promptcli-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:07:30.374238 promptcli-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-09 16:07:22.000000 promptcli-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-03-09 16:07:30.374238 promptcli-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-03-09 16:07:22.000000 promptcli-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:07:30.374238 promptcli-1.0.5/prompt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 16:07:22.000000 promptcli-1.0.5/prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-03-09 16:07:22.000000 promptcli-1.0.5/prompt/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:07:30.374238 promptcli-1.0.5/promptcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-03-09 16:07:30.000000 promptcli-1.0.5/promptcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-09 16:07:30.000000 promptcli-1.0.5/promptcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 16:07:30.000000 promptcli-1.0.5/promptcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-09 16:07:30.000000 promptcli-1.0.5/promptcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-09 16:07:30.000000 promptcli-1.0.5/promptcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-09 16:07:30.000000 promptcli-1.0.5/promptcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 16:07:30.374238 promptcli-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-09 16:07:22.000000 promptcli-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:33:43.641070 promptcli-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-23 16:33:30.000000 promptcli-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-23 16:33:43.641070 promptcli-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-23 16:33:30.000000 promptcli-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:33:43.637070 promptcli-2.0.0/prompt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:33:30.000000 promptcli-2.0.0/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-23 16:33:30.000000 promptcli-2.0.0/prompt/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:33:43.641070 promptcli-2.0.0/promptcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-23 16:33:43.000000 promptcli-2.0.0/promptcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-23 16:33:43.000000 promptcli-2.0.0/promptcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:33:43.000000 promptcli-2.0.0/promptcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-23 16:33:43.000000 promptcli-2.0.0/promptcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 16:33:43.000000 promptcli-2.0.0/promptcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 16:33:43.000000 promptcli-2.0.0/promptcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 16:33:43.641070 promptcli-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-23 16:33:30.000000 promptcli-2.0.0/setup.py
```

### Comparing `promptcli-1.0.5/LICENSE` & `promptcli-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptcli-1.0.5/PKG-INFO` & `promptcli-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptcli
-Version: 1.0.5
+Version: 2.0.0
 Summary: A command line application to help wrap the OpenAI ChatGPT api.
 Home-page: https://github.com/raiyanyahya/prompt
 Author: Raiyan Yahya
 Author-email: raiyanyahyadeveloper@gmail.com
 License: MIT
 Description: [![Actions Status](https://github.com/raiyanyahya/prompt/workflows/Build%20Test/badge.svg)](https://github.com/raiyanyahya/prompt/actions) [![Actions Status](https://github.com/raiyanyahya/prompt/workflows/Package%20Release/badge.svg)](https://github.com/raiyanyahya/prompt/actions) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=raiyanyahya_prompt&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=raiyanyahya_prompt) [![CodeQL](https://github.com/raiyanyahya/prompt/workflows/CodeQL/badge.svg)](https://github.com/raiyanyahya/prompt/actions?query=workflow%3ACodeQL) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/05a21e6c4ed4494ba39e2ee43b2327d2)](https://www.codacy.com/gh/raiyanyahya/prompt/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=raiyanyahya/prompt&amp;utm_campaign=Badge_Grade) [![](https://img.shields.io/badge/python-3.6+-blue.svg)] [![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
         
@@ -12,15 +12,15 @@
         
         ![](https://gifyu.com/images/demo.gif)
         
         `prompt` is designed to provide users a command-line interface for the ChatGPT API, which uses OpenAI's GPT language model to generate text based on user input.
         
         The application helps you start a `session` with ChatGPT so that the `context` is preserved and longer conversions with contexts are considered. The user's prompts and the responses are sent back to ChatGPT everytime.
         
-        The ChatGPT api usage depends on the number of tokens used and it is important that you use the tokens wisely. After a prompt has been answered the application will resend the last prompt and answer in the next prompt, this makes sure you can have a continued conversion with ChatGPT ` much like using ChatGPT in a single chat session `. This makes the token count larger and larger as you continue to chat. If you are not concerned with context use the `--clear` flag which will save your token usage.
+        The ChatGPT api usage depends on the number of tokens used and it is important that you use the tokens wisely. After a prompt has been answered the application will resend the last prompt and answer in the next prompt, this makes sure you can have a continued conversion with ChatGPT ` much like using ChatGPT in a single chat session `. This makes the token count larger and larger as you continue to chat. If you are not concerned with context use the `--clear` flag which will save your token usage. Use the `model` option to add 
         
         I hope you find it useful.
         
         
         ## Configuration
         
         The application requires you to have an api token to query the OpenAI's ChatGPT api. You can read about and get it here https://platform.openai.com/account/api-keys .
@@ -40,14 +40,15 @@
         Usage: prompt [OPTIONS] COMMAND [ARGS]...
         
           🥝 A command line application to interact with OpenAI's ChatGPT.
         
         Options:
           --version     Show the version and exit.
           --clear    🌊 Clear the context each round of chat
+          --model    🔄 The OpenAI model type.
           --help        Show this message and exit.
         
         Commands:
           update  🔐 Update the OpenAI API key.
         ```
```

### Comparing `promptcli-1.0.5/README.md` & `promptcli-2.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ![](https://gifyu.com/images/demo.gif)
 
 `prompt` is designed to provide users a command-line interface for the ChatGPT API, which uses OpenAI's GPT language model to generate text based on user input.
 
 The application helps you start a `session` with ChatGPT so that the `context` is preserved and longer conversions with contexts are considered. The user's prompts and the responses are sent back to ChatGPT everytime.
 
-The ChatGPT api usage depends on the number of tokens used and it is important that you use the tokens wisely. After a prompt has been answered the application will resend the last prompt and answer in the next prompt, this makes sure you can have a continued conversion with ChatGPT ` much like using ChatGPT in a single chat session `. This makes the token count larger and larger as you continue to chat. If you are not concerned with context use the `--clear` flag which will save your token usage.
+The ChatGPT api usage depends on the number of tokens used and it is important that you use the tokens wisely. After a prompt has been answered the application will resend the last prompt and answer in the next prompt, this makes sure you can have a continued conversion with ChatGPT ` much like using ChatGPT in a single chat session `. This makes the token count larger and larger as you continue to chat. If you are not concerned with context use the `--clear` flag which will save your token usage. Use the `model` option to add 
 
 I hope you find it useful.
 
 
 ## Configuration
 
 The application requires you to have an api token to query the OpenAI's ChatGPT api. You can read about and get it here https://platform.openai.com/account/api-keys .
@@ -32,14 +32,15 @@
 Usage: prompt [OPTIONS] COMMAND [ARGS]...
 
   🥝 A command line application to interact with OpenAI's ChatGPT.
 
 Options:
   --version     Show the version and exit.
   --clear    🌊 Clear the context each round of chat
+  --model    🔄 The OpenAI model type.
   --help        Show this message and exit.
 
 Commands:
   update  🔐 Update the OpenAI API key.
 ```
```

### Comparing `promptcli-1.0.5/prompt/cli.py` & `promptcli-2.0.0/prompt/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,31 +22,32 @@
             api_key = input("🔑 Enter your OpenAI API key: ")
             with open(config_file, "w", encoding="UTF-8") as f:
                 f.write(f'{{"api_key": "{api_key}"}}')
     openai.api_key = api_key or getenv("OPENAI_API_KEY")
 
 
 @click.group(invoke_without_command=True)
-@click.version_option(version="1.0.5")
+@click.version_option(version="2.0.0")
 @click.option("--clear", is_flag=True, help="🌊 Clear the context each round of chat")
-def cli(clear):
+@click.option("--model", default="gpt-3.5-turbo", help="🔄 The OpenAI model type.")
+def cli(clear,model):
     """🥝 A command line application to interact with OpenAI's ChatGPT."""
     configure_openai()
     session_data = []
     click.echo("")
     click.echo(" 🥝 Session started. Enter 'exit' to end the session.")
     while True:
         user_input = click.prompt("➡ ")
         session_data.append({"role": "user", "content": user_input})
         if user_input.lower() == "exit":
             break
         try:
             with console.status("Waiting for chatgpt...", spinner="dots8Bit"):
                 completion = openai.ChatCompletion.create(
-                    model="gpt-3.5-turbo", messages=session_data
+                    model=model, messages=session_data
                 )
                 print(completion["choices"][0]["message"]["content"])
                 print("")
                 session_data.append(
                     {
                         "role": "system",
                         "content": completion["choices"][0]["message"]["content"],
```

### Comparing `promptcli-1.0.5/promptcli.egg-info/PKG-INFO` & `promptcli-2.0.0/promptcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptcli
-Version: 1.0.5
+Version: 2.0.0
 Summary: A command line application to help wrap the OpenAI ChatGPT api.
 Home-page: https://github.com/raiyanyahya/prompt
 Author: Raiyan Yahya
 Author-email: raiyanyahyadeveloper@gmail.com
 License: MIT
 Description: [![Actions Status](https://github.com/raiyanyahya/prompt/workflows/Build%20Test/badge.svg)](https://github.com/raiyanyahya/prompt/actions) [![Actions Status](https://github.com/raiyanyahya/prompt/workflows/Package%20Release/badge.svg)](https://github.com/raiyanyahya/prompt/actions) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=raiyanyahya_prompt&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=raiyanyahya_prompt) [![CodeQL](https://github.com/raiyanyahya/prompt/workflows/CodeQL/badge.svg)](https://github.com/raiyanyahya/prompt/actions?query=workflow%3ACodeQL) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/05a21e6c4ed4494ba39e2ee43b2327d2)](https://www.codacy.com/gh/raiyanyahya/prompt/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=raiyanyahya/prompt&amp;utm_campaign=Badge_Grade) [![](https://img.shields.io/badge/python-3.6+-blue.svg)] [![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
         
@@ -12,15 +12,15 @@
         
         ![](https://gifyu.com/images/demo.gif)
         
         `prompt` is designed to provide users a command-line interface for the ChatGPT API, which uses OpenAI's GPT language model to generate text based on user input.
         
         The application helps you start a `session` with ChatGPT so that the `context` is preserved and longer conversions with contexts are considered. The user's prompts and the responses are sent back to ChatGPT everytime.
         
-        The ChatGPT api usage depends on the number of tokens used and it is important that you use the tokens wisely. After a prompt has been answered the application will resend the last prompt and answer in the next prompt, this makes sure you can have a continued conversion with ChatGPT ` much like using ChatGPT in a single chat session `. This makes the token count larger and larger as you continue to chat. If you are not concerned with context use the `--clear` flag which will save your token usage.
+        The ChatGPT api usage depends on the number of tokens used and it is important that you use the tokens wisely. After a prompt has been answered the application will resend the last prompt and answer in the next prompt, this makes sure you can have a continued conversion with ChatGPT ` much like using ChatGPT in a single chat session `. This makes the token count larger and larger as you continue to chat. If you are not concerned with context use the `--clear` flag which will save your token usage. Use the `model` option to add 
         
         I hope you find it useful.
         
         
         ## Configuration
         
         The application requires you to have an api token to query the OpenAI's ChatGPT api. You can read about and get it here https://platform.openai.com/account/api-keys .
@@ -40,14 +40,15 @@
         Usage: prompt [OPTIONS] COMMAND [ARGS]...
         
           🥝 A command line application to interact with OpenAI's ChatGPT.
         
         Options:
           --version     Show the version and exit.
           --clear    🌊 Clear the context each round of chat
+          --model    🔄 The OpenAI model type.
           --help        Show this message and exit.
         
         Commands:
           update  🔐 Update the OpenAI API key.
         ```
```

### Comparing `promptcli-1.0.5/setup.py` & `promptcli-2.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     long_description = file.read()
 
 
 setup(
     name="promptcli",
     python_requires=">3.5",
     options={"bdist_wheel": {"universal": "1"}},
-    version="1.0.5",
+    version="2.0.0",
     description="A command line application to help wrap the OpenAI ChatGPT api.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raiyanyahya/prompt",
     author="Raiyan Yahya",
     license="MIT",
     author_email="raiyanyahyadeveloper@gmail.com",
     keywords=["cli", "developer tools", "productivity", "openai", "chatgpt"],
     packages=find_packages(),
-    install_requires=["click==8.1.3", "openai==0.27.0", "rich==13.3.1"],
+    install_requires=["click==8.1.3", "openai==0.27.4", "rich==13.3.4"],
     entry_points={"console_scripts": ["prompt=prompt.cli:cli"]},
 )
```

