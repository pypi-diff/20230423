# Comparing `tmp/shell_genie-0.2.8.tar.gz` & `tmp/shell_genie-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_genie-0.2.8.tar", max compression
+gzip compressed data, was "shell_genie-0.2.9.tar", max compression
```

## Comparing `shell_genie-0.2.8.tar` & `shell_genie-0.2.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-03-03 15:05:30.551971 shell_genie-0.2.8/LICENSE
--rw-r--r--   0        0        0     2920 2023-03-03 15:01:52.844187 shell_genie-0.2.8/README.md
--rw-r--r--   0        0        0      794 2023-03-03 15:05:39.335020 shell_genie-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-22 22:26:29.534745 shell_genie-0.2.8/shell_genie/__init__.py
--rw-r--r--   0        0        0     3051 2023-01-30 13:00:22.270249 shell_genie-0.2.8/shell_genie/backends.py
--rw-r--r--   0        0        0     3958 2023-01-27 13:43:18.139705 shell_genie-0.2.8/shell_genie/main.py
--rw-r--r--   0        0        0      948 2023-01-27 13:32:00.578123 shell_genie-0.2.8/shell_genie/utils.py
--rw-r--r--   0        0        0     3951 1970-01-01 00:00:00.000000 shell_genie-0.2.8/setup.py
--rw-r--r--   0        0        0     3631 1970-01-01 00:00:00.000000 shell_genie-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-03-03 15:05:30.551971 shell_genie-0.2.9/LICENSE
+-rw-r--r--   0        0        0     2936 2023-04-23 17:11:36.558299 shell_genie-0.2.9/README.md
+-rw-r--r--   0        0        0      794 2023-04-23 17:22:49.574283 shell_genie-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-22 22:26:29.534745 shell_genie-0.2.9/shell_genie/__init__.py
+-rw-r--r--   0        0        0     3498 2023-04-23 17:22:33.245351 shell_genie-0.2.9/shell_genie/backends.py
+-rw-r--r--   0        0        0     3990 2023-04-23 17:17:35.785426 shell_genie-0.2.9/shell_genie/main.py
+-rw-r--r--   0        0        0      957 2023-04-23 17:08:47.704274 shell_genie-0.2.9/shell_genie/utils.py
+-rw-r--r--   0        0        0     3967 1970-01-01 00:00:00.000000 shell_genie-0.2.9/setup.py
+-rw-r--r--   0        0        0     3647 1970-01-01 00:00:00.000000 shell_genie-0.2.9/PKG-INFO
```

### Comparing `shell_genie-0.2.8/LICENSE` & `shell_genie-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_genie-0.2.8/README.md` & `shell_genie-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 1. First, you need to initialize the tool by running the following command:
 
    ```shell
    shell-genie init
    ```
 
-   This will prompt you to select a backend (either `openai-gpt3` or `free-genie`) and provide any additional information that is required (e.g. your own [OpenAI API](https://openai.com/api/) key for `openai-gpt3`).
+   This will prompt you to select a backend (either `openai-gpt3.5-turbo` or `free-genie`) and provide any additional information that is required (e.g. your own [OpenAI API](https://openai.com/api/) key for `openai-gpt3.5-turbo`).
 
    The `free-genie` backend is free to use. I'm hosting it, and as you can imagine I'm not a big corporation with unlimited money, so there's no guarantee that it will be available at all times. My goal is to generate a dataset of commands to fine-tune a model later on (this is mentioned during the initialization process).
 
 2. Once you have initialized the tool, you can start asking the genie what you want to do. For example, you may ask it to find all the `json` files in the current directory that are larger than 1MB:
 
    ```shell
    shell-genie ask "find all json files in the current directory that are larger than 1MB"
```

### Comparing `shell_genie-0.2.8/pyproject.toml` & `shell_genie-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shell-genie"
-version = "0.2.8"
+version = "0.2.9"
 description = "Shell Genie is a command-line tool that lets you interact with the terminal in plain English. You ask the genie what you want to do and it will give you the command you need."
 authors = ["Dylan Castillo <dylanjcastillo@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shell_genie"}]
 license = "MIT"
 
 [tool.poetry.scripts]
```

### Comparing `shell_genie-0.2.8/shell_genie/backends.py` & `shell_genie-0.2.9/shell_genie/backends.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,35 +22,47 @@
         openai.api_key = api_key
 
     def _build_prompt(self, wish: str, explain: bool = False):
         explain_text = ""
         format_text = "Command: <insert_command_here>"
 
         if explain:
-            explain_text = "In addition, provide a detailed description of how the provided command works."
-            format_text = "Command: <insert_command_here>\n Description: <insert_description_here>"
+            explain_text = (
+                "Also, provide a detailed description of how the command works."
+            )
+            format_text = "Command: <insert_command_here>\n Description: <insert_description_here> (the description should be in the same language the user is using)"
 
-        prompt = f"""You're a command line tool that generates CLI commands for the user.
-        Format: {format_text}
-        Instructions: Write a CLI command that does the following: {wish}. It must work on {self.os_fullname} using {self.shell}. {explain_text}
-        """
+        prompt = f"""Instructions: Write a CLI command that does the following: {wish}. Make sure the command is correct and works on {self.os_fullname} using {self.shell}. {explain_text}
 
+        Format: {format_text}
+        """.strip()
         return prompt
 
     def ask(self, wish: str, explain: bool = False):
 
         prompt = self._build_prompt(wish, explain)
 
-        response = openai.Completion.create(
-            model="text-davinci-003",
-            prompt=prompt,
+        response = openai.ChatCompletion.create(
+            model="gpt-3.5-turbo",
+            messages=[
+                {
+                    "role": "system",
+                    "content": "You're a command line tool that generates CLI commands for the user.",
+                },
+                {"role": "user", "content": prompt},
+            ],
             max_tokens=300 if explain else 180,
             temperature=0,
         )
-        responses_processed = response.choices[0].text.strip().split("\n")
+        responses_processed = (
+            response["choices"][0]["message"]["content"].strip().split("\n")
+        )
+        responses_processed = [
+            x.strip() for x in responses_processed if len(x.strip()) > 0
+        ]
         command = responses_processed[0].replace("Command:", "").strip()
 
         description = None
         if explain:
             description = responses_processed[1].split("Description: ")[1]
 
         return command, description
@@ -87,13 +99,13 @@
         requests.post(
             url=self.url + "/post_execute",
             json={
                 "wish": wish,
                 "explain": explain,
                 "os_fullname": self.os_fullname,
                 "shell": self.shell,
-               "command": command,
+                "command": command,
                 "description": description,
                 "correct": feedback,
             },
         )
         return
```

### Comparing `shell_genie-0.2.8/shell_genie/main.py` & `shell_genie-0.2.9/shell_genie/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 APP_NAME = ".shell_genie"
 app = typer.Typer()
 
 
 @app.command()
 def init():
 
-    backend = Prompt.ask("Select backend:", choices=["openai-gpt3", "free-genie"])
+    backend = Prompt.ask(
+        "Select backend:", choices=["openai-gpt-3.5-turbo", "free-genie"]
+    )
     additional_params = {}
 
-    if backend == "openai-gpt3":
+    if backend == "openai-gpt-3.5-turbo":
         additional_params["openai_api_key"] = Prompt.ask("Enter a OpenAI API key")
 
     if backend == "free-genie":
         print(
             "[yellow]Note that this server will store the requested command, OS, and shell version to improve the model. Also, I cannot guarantee that the server will be up and running 24/7.[/yellow]"
         )
         if not Confirm.ask("Do you want to continue?"):
```

### Comparing `shell_genie-0.2.8/shell_genie/utils.py` & `shell_genie-0.2.9/shell_genie/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     if oper_sys == "Linux":
         return (oper_sys, platform.freedesktop_os_release()["PRETTY_NAME"])
     return (None, None)
 
 
 def get_backend(**config: dict):
     backend_name = config["backend"]
-    if backend_name == "openai-gpt3":
+    if backend_name == "openai-gpt-3.5-turbo":
         return OpenAIGenie(
             api_key=config["openai_api_key"],
             os_fullname=config["os_fullname"],
             shell=config["shell"],
         )
     elif backend_name == "free-genie":
         return FreeTrialGenie(
```

### Comparing `shell_genie-0.2.8/setup.py` & `shell_genie-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['openai>=0.26.0,<1.0.0', 'pyperclip>=1.8.2,<2.0.0', 'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['shell-genie = shell_genie.main:app']}
 
 setup_kwargs = {
     'name': 'shell-genie',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Shell Genie is a command-line tool that lets you interact with the terminal in plain English. You ask the genie what you want to do and it will give you the command you need.',
-    'long_description': '# 🧞\u200d♂️ Shell Genie\n\n_Your wishes are my commands._\n\nShell Genie is a command-line tool that lets you interact with the terminal in plain English. You ask the genie what you want to do and it will give you the command you need.\n\n## Installation\n\nThe recommended way to install Shell Genie is using [pipx](https://pypa.github.io/pipx/):\n\n1. Install Python 3.10 or higher.\n2. Install [pipx](https://github.com/pypa/pipx#install-pipx).\n3. Install Shell Genie: `pipx install shell-genie`\n\nAlternatively, you can install it using pip:\n\n1. Install Python 3.10 or higher.\n2. Create a virtual environment in your preferred location: `python -m venv .venv`\n3. Activate the virtual environment: `source .venv/bin/activate`\n4. Install Shell Genie: `pip install shell-genie`\n\n## How to use\n\n1. First, you need to initialize the tool by running the following command:\n\n   ```shell\n   shell-genie init\n   ```\n\n   This will prompt you to select a backend (either `openai-gpt3` or `free-genie`) and provide any additional information that is required (e.g. your own [OpenAI API](https://openai.com/api/) key for `openai-gpt3`).\n\n   The `free-genie` backend is free to use. I\'m hosting it, and as you can imagine I\'m not a big corporation with unlimited money, so there\'s no guarantee that it will be available at all times. My goal is to generate a dataset of commands to fine-tune a model later on (this is mentioned during the initialization process).\n\n2. Once you have initialized the tool, you can start asking the genie what you want to do. For example, you may ask it to find all the `json` files in the current directory that are larger than 1MB:\n\n   ```shell\n   shell-genie ask "find all json files in the current directory that are larger than 1MB"\n   ```\n\n   You\'ll see an output similar to this:\n\n   ```shell\n   Command: find . -name "*.json" -size +1M\n   Do you want to run this command? [y/n]:\n   ```\n\n   If you have questions about how the command works, you can ask the genie to explain it:\n\n   ```shell\n   shell-genie ask "find all json files in the current directory that are larger than 1MB" --explain\n   ```\n\n   And you\'ll see an output similar to this:\n\n   ```shell\n   Command: find . -name "*.json" -size +1M\n   Description: This command will search the current directory for all... (shortened for brevity)\n   Do you want to run the command? [y/n]:\n   ```\n\n3. Run the command if you want to. If you\'re using `free-genie`, and you want to help improve the tool, you can provide feedback after you\'ve run the command.\n\n## Examples\n\nHere are two short videos showing how to use the tool:\n\n- [Ask genie for a command](https://youtu.be/QM-fwgnGzDc)\n- [Ask genie to explain a command](https://youtu.be/Qi3w3abI4oE)\n\n## Limitations\n\nAs you can imagine not all the commands provided by the genie work as expected. Use them at your own risk.\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
+    'long_description': '# 🧞\u200d♂️ Shell Genie\n\n_Your wishes are my commands._\n\nShell Genie is a command-line tool that lets you interact with the terminal in plain English. You ask the genie what you want to do and it will give you the command you need.\n\n## Installation\n\nThe recommended way to install Shell Genie is using [pipx](https://pypa.github.io/pipx/):\n\n1. Install Python 3.10 or higher.\n2. Install [pipx](https://github.com/pypa/pipx#install-pipx).\n3. Install Shell Genie: `pipx install shell-genie`\n\nAlternatively, you can install it using pip:\n\n1. Install Python 3.10 or higher.\n2. Create a virtual environment in your preferred location: `python -m venv .venv`\n3. Activate the virtual environment: `source .venv/bin/activate`\n4. Install Shell Genie: `pip install shell-genie`\n\n## How to use\n\n1. First, you need to initialize the tool by running the following command:\n\n   ```shell\n   shell-genie init\n   ```\n\n   This will prompt you to select a backend (either `openai-gpt3.5-turbo` or `free-genie`) and provide any additional information that is required (e.g. your own [OpenAI API](https://openai.com/api/) key for `openai-gpt3.5-turbo`).\n\n   The `free-genie` backend is free to use. I\'m hosting it, and as you can imagine I\'m not a big corporation with unlimited money, so there\'s no guarantee that it will be available at all times. My goal is to generate a dataset of commands to fine-tune a model later on (this is mentioned during the initialization process).\n\n2. Once you have initialized the tool, you can start asking the genie what you want to do. For example, you may ask it to find all the `json` files in the current directory that are larger than 1MB:\n\n   ```shell\n   shell-genie ask "find all json files in the current directory that are larger than 1MB"\n   ```\n\n   You\'ll see an output similar to this:\n\n   ```shell\n   Command: find . -name "*.json" -size +1M\n   Do you want to run this command? [y/n]:\n   ```\n\n   If you have questions about how the command works, you can ask the genie to explain it:\n\n   ```shell\n   shell-genie ask "find all json files in the current directory that are larger than 1MB" --explain\n   ```\n\n   And you\'ll see an output similar to this:\n\n   ```shell\n   Command: find . -name "*.json" -size +1M\n   Description: This command will search the current directory for all... (shortened for brevity)\n   Do you want to run the command? [y/n]:\n   ```\n\n3. Run the command if you want to. If you\'re using `free-genie`, and you want to help improve the tool, you can provide feedback after you\'ve run the command.\n\n## Examples\n\nHere are two short videos showing how to use the tool:\n\n- [Ask genie for a command](https://youtu.be/QM-fwgnGzDc)\n- [Ask genie to explain a command](https://youtu.be/Qi3w3abI4oE)\n\n## Limitations\n\nAs you can imagine not all the commands provided by the genie work as expected. Use them at your own risk.\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
     'author': 'Dylan Castillo',
     'author_email': 'dylanjcastillo@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `shell_genie-0.2.8/PKG-INFO` & `shell_genie-0.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-genie
-Version: 0.2.8
+Version: 0.2.9
 Summary: Shell Genie is a command-line tool that lets you interact with the terminal in plain English. You ask the genie what you want to do and it will give you the command you need.
 License: MIT
 Author: Dylan Castillo
 Author-email: dylanjcastillo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -40,15 +40,15 @@
 
 1. First, you need to initialize the tool by running the following command:
 
    ```shell
    shell-genie init
    ```
 
-   This will prompt you to select a backend (either `openai-gpt3` or `free-genie`) and provide any additional information that is required (e.g. your own [OpenAI API](https://openai.com/api/) key for `openai-gpt3`).
+   This will prompt you to select a backend (either `openai-gpt3.5-turbo` or `free-genie`) and provide any additional information that is required (e.g. your own [OpenAI API](https://openai.com/api/) key for `openai-gpt3.5-turbo`).
 
    The `free-genie` backend is free to use. I'm hosting it, and as you can imagine I'm not a big corporation with unlimited money, so there's no guarantee that it will be available at all times. My goal is to generate a dataset of commands to fine-tune a model later on (this is mentioned during the initialization process).
 
 2. Once you have initialized the tool, you can start asking the genie what you want to do. For example, you may ask it to find all the `json` files in the current directory that are larger than 1MB:
 
    ```shell
    shell-genie ask "find all json files in the current directory that are larger than 1MB"
```

