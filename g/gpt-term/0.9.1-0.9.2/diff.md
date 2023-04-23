# Comparing `tmp/gpt-term-0.9.1.tar.gz` & `tmp/gpt-term-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-term-0.9.1.tar", last modified: Sun Apr 23 04:09:47 2023, max compression
+gzip compressed data, was "gpt-term-0.9.2.tar", last modified: Sun Apr 23 14:29:03 2023, max compression
```

## Comparing `gpt-term-0.9.1.tar` & `gpt-term-0.9.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 junpenglu   (501) staff       (20)        0 2023-04-23 04:09:47.911801 gpt-term-0.9.1/
--rw-r--r--   0 junpenglu   (501) staff       (20)     1066 2023-03-03 17:11:42.000000 gpt-term-0.9.1/LICENSE
--rw-r--r--   0 junpenglu   (501) staff       (20)    11340 2023-04-23 04:09:47.911628 gpt-term-0.9.1/PKG-INFO
--rw-r--r--   0 junpenglu   (501) staff       (20)    10931 2023-04-19 09:15:11.000000 gpt-term-0.9.1/README.md
--rwxr-xr-x   0 junpenglu   (501) staff       (20)    43918 2023-04-23 03:25:52.000000 gpt-term-0.9.1/chat.py
--rw-r--r--   0 junpenglu   (501) staff       (20)      909 2023-04-22 15:13:05.000000 gpt-term-0.9.1/config.ini
-drwxr-xr-x   0 junpenglu   (501) staff       (20)        0 2023-04-23 04:09:47.911333 gpt-term-0.9.1/gpt_term.egg-info/
--rw-r--r--   0 junpenglu   (501) staff       (20)    11340 2023-04-23 04:09:47.000000 gpt-term-0.9.1/gpt_term.egg-info/PKG-INFO
--rw-r--r--   0 junpenglu   (501) staff       (20)      239 2023-04-23 04:09:47.000000 gpt-term-0.9.1/gpt_term.egg-info/SOURCES.txt
--rw-r--r--   0 junpenglu   (501) staff       (20)        1 2023-04-23 04:09:47.000000 gpt-term-0.9.1/gpt_term.egg-info/dependency_links.txt
--rw-r--r--   0 junpenglu   (501) staff       (20)       39 2023-04-23 04:09:47.000000 gpt-term-0.9.1/gpt_term.egg-info/entry_points.txt
--rw-r--r--   0 junpenglu   (501) staff       (20)       81 2023-04-23 04:09:47.000000 gpt-term-0.9.1/gpt_term.egg-info/requires.txt
--rw-r--r--   0 junpenglu   (501) staff       (20)        5 2023-04-23 04:09:47.000000 gpt-term-0.9.1/gpt_term.egg-info/top_level.txt
--rw-r--r--   0 junpenglu   (501) staff       (20)       38 2023-04-23 04:09:47.911860 gpt-term-0.9.1/setup.cfg
--rw-r--r--   0 junpenglu   (501) staff       (20)      990 2023-04-23 03:30:59.000000 gpt-term-0.9.1/setup.py
+drwxr-xr-x   0 junpenglu   (501) staff       (20)        0 2023-04-23 14:29:03.426869 gpt-term-0.9.2/
+-rw-r--r--   0 junpenglu   (501) staff       (20)     1066 2023-03-03 17:11:42.000000 gpt-term-0.9.2/LICENSE
+-rw-r--r--   0 junpenglu   (501) staff       (20)    12210 2023-04-23 14:29:03.426611 gpt-term-0.9.2/PKG-INFO
+-rw-r--r--   0 junpenglu   (501) staff       (20)    11801 2023-04-23 14:19:42.000000 gpt-term-0.9.2/README.md
+-rwxr-xr-x   0 junpenglu   (501) staff       (20)      117 2023-04-23 08:19:58.000000 gpt-term-0.9.2/chat.py
+-rw-r--r--   0 junpenglu   (501) staff       (20)      909 2023-04-22 15:13:05.000000 gpt-term-0.9.2/config.ini
+drwxr-xr-x   0 junpenglu   (501) staff       (20)        0 2023-04-23 14:29:03.424237 gpt-term-0.9.2/gpt_term/
+-rw-r--r--   0 junpenglu   (501) staff       (20)       21 2023-04-23 13:38:43.000000 gpt-term-0.9.2/gpt_term/__init__.py
+-rwxr-xr-x   0 junpenglu   (501) staff       (20)    43404 2023-04-23 13:37:33.000000 gpt-term-0.9.2/gpt_term/main.py
+drwxr-xr-x   0 junpenglu   (501) staff       (20)        0 2023-04-23 14:29:03.426283 gpt-term-0.9.2/gpt_term.egg-info/
+-rw-r--r--   0 junpenglu   (501) staff       (20)    12210 2023-04-23 14:29:03.000000 gpt-term-0.9.2/gpt_term.egg-info/PKG-INFO
+-rw-r--r--   0 junpenglu   (501) staff       (20)      277 2023-04-23 14:29:03.000000 gpt-term-0.9.2/gpt_term.egg-info/SOURCES.txt
+-rw-r--r--   0 junpenglu   (501) staff       (20)        1 2023-04-23 14:29:03.000000 gpt-term-0.9.2/gpt_term.egg-info/dependency_links.txt
+-rw-r--r--   0 junpenglu   (501) staff       (20)       48 2023-04-23 14:29:03.000000 gpt-term-0.9.2/gpt_term.egg-info/entry_points.txt
+-rw-r--r--   0 junpenglu   (501) staff       (20)       91 2023-04-23 14:29:03.000000 gpt-term-0.9.2/gpt_term.egg-info/requires.txt
+-rw-r--r--   0 junpenglu   (501) staff       (20)       14 2023-04-23 14:29:03.000000 gpt-term-0.9.2/gpt_term.egg-info/top_level.txt
+-rw-r--r--   0 junpenglu   (501) staff       (20)       38 2023-04-23 14:29:03.426930 gpt-term-0.9.2/setup.cfg
+-rw-r--r--   0 junpenglu   (501) staff       (20)     1053 2023-04-23 12:48:57.000000 gpt-term-0.9.2/setup.py
```

### Comparing `gpt-term-0.9.1/LICENSE` & `gpt-term-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-term-0.9.1/PKG-INFO` & `gpt-term-0.9.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: gpt-term
-Version: 0.9.1
-Summary: Use ChatGPT in terminal
-Home-page: https://github.com/xiaoxx970/chatgpt-in-terminal
-Author: xiaoxx970
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Chat with GPT in Terminal
 
 [![English badge](https://img.shields.io/badge/%E8%8B%B1%E6%96%87-English-blue)](./README.md)
 [![简体中文 badge](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-Simplified%20Chinese-blue)](./README.zh-CN.md)
 [![Platform badge](https://img.shields.io/badge/Platform-MacOS%7CWindows%7CLinux-green)]()
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
 
@@ -25,27 +11,30 @@
 
 Supports history retrieval with the up arrow key, optional multi-line questions, and tokens counting.
 
 Slash (/) commands are available in the chat box to toggle multi-line submit mode, undo the last question and answer, modify the system prompt and more, see the available commands below for details.
 
 Supports saving chat messages to a JSON file and loading them from the file.
 
-![example](README.assets/small.gif)
+![example](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/small.gif)
 
 Uses the [gpt-3.5-turbo](https://platform.openai.com/docs/guides/chat/chat-completions-beta) model, which is the same model used by ChatGPT (Free Edition), as default.
 
 ## Changelog
 
-### 2023-04-15
-
-- Added the ability to create a line break in single-line mode using `Esc` + `Enter`
+### 2023-04-23
+Released `gpt-term` on [Pypi](https://pypi.org/project/gpt-term/), started version control. No need to clone the project locally anymore, simply use the `pip` command to install gpt-term.
 
 <details>
   <summary>More Change log</summary>
 
+### 2023-04-15
+
+- Added the ability to create a line break in single-line mode using `Esc` + `Enter`
+
 ### 2023-04-13
 
 - Added the function of generating and setting the terminal title in the background, and now the client will use the summary of the first question content as the terminal title
 
 ### 2023-04-09
 
 - Add filename generate function, client will suggest the summary of the first question as filename when save command executed.
@@ -79,102 +68,83 @@
 
 ## Preparation
 
 1. An OpenAI API key. You need to register an OpenAI account and obtain an API key.
 
    OpenAI's API key can be generated on the page opened by clicking "View API keys" in the upper right corner of the homepage, direct link: https://platform.openai.com/account/api-keys
 
-   ![image-20230303233352970](README.assets/image-20230303233352970.png)
+   ![image-20230303233352970](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/image-20230303233352970.png)
 
-2. [Python](https://www.python.org/downloads/) version 3.6 or higher.
-3. [git](https://git-scm.com/downloads)
+2. [Python](https://www.python.org/downloads/) version 3.7 or higher.
 
 ## Installation
 
-1. Clone the repo and enter the directory
 
-   ```shell
-   git clone https://github.com/xiaoxx970/chatgpt-in-terminal.git
-   cd ./chatgpt-in-terminal
-   ```
-   
-2. Rename the `.env.example` file in the current directory to `.env`.
+1. Install `GPT-Term` using `pip`
 
    ```shell
-   mv .env.example .env
+   pip3 install gpt-term
    ```
 
-   Edit the `.env` file and modify the `OPENAI_API_KEY` variable to your API Key.
+2. Configure the API Key
 
    ```shell
-   OPENAI_API_KEY=your_API_Key
+   gpt-term --set-apikey YOUR_API_KEY
    ```
 
-   > If the `.env` file is not configured, you can also enter the API Key directly at runtime, but it will only be effective for the current session.
-   
-3. Install the dependencies in the `requirements.txt` file using the `pip` command.
-
-   ```shell
-   pip3 install -r requirements.txt
-   ```
+   > If you don't configure the API Key now, you can enter it when prompted during runtime.
 
 ## Update
 
-If you want to update the script to the latest version, run the following command in this project's directory:
+To update `GPT-Term` to the latest version, run the following command in your terminal:
 
 ```sh
-git pull
-pip3 install -r requirements.txt
+pip3 install --upgrade gpt-term
 ```
 
-> If git error is reported
->
-> ```shell
-> error: Your local changes to the following files would be overwritten by merge:
->          .env
-> Please commit your changes or stash them before you merge.
-> Aborting
-> ```
->
-> Just untrack the .env file from git first (doesn't delete the local .env file)
->
-> ```sh
-> git rm --cache .env
-> ```
->
-> Then run the `git pull` command above 
+> If there is a new version, `GPT-Term` will prompt the user to update upon exiting.
 
 ## How to Use
 
 Run with the following command:
 
 ```shell
-python3 chat.py
+gpt-term
 ```
 
 When entering a question in single-line mode, use `Esc` + `Enter` to start a new line, and use `Enter` to submit the question.
 
-> Original chat logs will be saved to `chat.log`
+> Original chat logs will be saved to `~/.gpt-term/chat.log`
 
 ### Available Arguments
 
 | Arguments     | Description                     | Example                                       |
 | ------------- | ------------------------------- | --------------------------------------------- |
 | -h, --help    | show this help message and exit | `chat.py --help`                              |
 | --load FILE   | Load chat history from file     | `chat.py --load chat_history_code_check.json` |
 | --key API_KEY | choose the API key to load      | `chat.py --key OPENAI_API_KEY1`               |
 | --model MODEL | choose the AI model to use      | `chat.py --model gpt-3.5-turbo`               |
 | -m, --multi   | Enable multi-line mode          | `chat.py --multi`                             |
 | -r, --raw     | Enable raw mode                 | `chat.py --raw`                               |
+| --set-apikey KEY        | Set the OpenAI API key                                   | `gpt-term --set-apikey sk-xxx`   |
+| --set-timeout SEC       | Set the maximum wait time for API requests               | `gpt-term --set-timeout 10`      |
+| --set-gentitle BOOL     | Set whether to auto-generate a title for the chat        | `gpt-term --set-gentitle True`   |
+| --set-saveperfix PERFIX | Set the save prefix for chat history files               | `gpt-term --set-saveperfix chat_history_` |
+| --set-loglevel LEVEL    | Set the log level: DEBUG, INFO, WARNING, ERROR, CRITICAL | `gpt-term --set-loglevel DEBUG`  |
 
 > Multi-line mode and raw mode can be used simultaneously
 
-### `.env` configuration file
+### Configuration File
 
-```shell
+The configuration file is located at `~/.gpt-term/config.ini` and is autogenerated. It can be modified using the program's `--set` option or edited manually.
+
+The default configuration is as follows:
+
+```ini config.ini
+[DEFAULT]
 # API key for OpenAI
 OPENAI_API_KEY=
 
 # The maximum waiting time for API requests, the default is 30s
 OPENAI_API_TIMEOUT=30
 
 # Whether to automatically generate titles for conversations, enabled by default (generating titles will consume a small amount of tokens)
@@ -238,18 +208,20 @@
 
 - `/title [new_title]`: Set terminal title for this chat
 
   > If new_title is not provided, a new title will be generated based on first question
 
 - `/timeout [new_timeout]`: Modify API timeout.
 
-  > The default timeout is 30 seconds, it can also be configured by setting `OPENAI_API_TIMEOUT=` in the `.env` file.
+  > The default timeout is 30 seconds, it can also be configured by setting `OPENAI_API_TIMEOUT=` in the `~/.gpt-term/config.ini` file.
   
 - `/undo`: Delete the previous question and answer
 
+- `/version`: Display the local and remote versions of `GPT-Term`
+
 - `/help`: Display available commands
 
 - `/exit`: Exit the application
 
 ### Exit Words
 
 In the chat, use exit words to end the current session. Exit words include:
@@ -266,33 +238,41 @@
 
 > Current price: $0.002 / 1K tokens, Free Edition rate limit: 20 requests / min (`gpt-3.5-turbo`)
 
 ## Dependencies
 
 Thanks to the following projects for providing strong support for this script:
 
-- [rich](https://github.com/Textualize/rich): For rendering rich text in the terminal
-- [python-dotenv](https://github.com/theskumar/python-dotenv): For loading environment variables from `.env` file
+- [requests](https://github.com/psf/requests): For handling HTTP requests
+- [pyperclip](https://github.com/asweigart/pyperclip): A cross-platform clipboard operation library
+- [rich](https://github.com/willmcgugan/rich): For outputting rich text in the terminal
 - [prompt_toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit): Command-line input processing library
+- [sseclient-py](https://github.com/btubbs/sseclient-py): For implementing streaming output of answers
+- [tiktoken](https://github.com/OpenAI/tiktoken): A library for calculating and processing OpenAI API tokens
 
 ## Contributing
 
 Feel free to dive in! [Open an issue](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/new) or submit PRs.
 
 ### Contributors
 
 This project exists thanks to all the people who contribute. 
 <a href="https://github.com/xiaoxx970/chatgpt-in-terminal/graphs/contributors"><img src="https://opencollective.com/chatgpt-in-terminal/contributors.svg?width=890&button=false" /></a>
 
 ## Project Structure
 
-```bash
-├── README.md           # Documentation
-├── chat.py             # Project code
-├── requirements.txt    # Dependency package list
-├── chat.log            # Chat log generated after chatting
-└── .env                # Storage API key and other settings
+```sh
+.
+├── LICENSE                   # License
+├── README.md                 # Documentation
+├── chat.py                   # Script entry point
+├── config.ini                # API key storage and other settings
+├── gpt_term                  # Project package folder
+│   ├── __init__.py
+│   └── main.py               # Main program
+├── requirements.txt          # List of dependencies
+└── setup.py
 ```
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE).
+This project is licensed under the [MIT License](LICENSE).
```

### Comparing `gpt-term-0.9.1/README.md` & `gpt-term-0.9.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: gpt-term
+Version: 0.9.2
+Summary: Use ChatGPT in terminal
+Home-page: https://github.com/xiaoxx970/chatgpt-in-terminal
+Author: xiaoxx970
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## Chat with GPT in Terminal
 
 [![English badge](https://img.shields.io/badge/%E8%8B%B1%E6%96%87-English-blue)](./README.md)
 [![简体中文 badge](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-Simplified%20Chinese-blue)](./README.zh-CN.md)
 [![Platform badge](https://img.shields.io/badge/Platform-MacOS%7CWindows%7CLinux-green)]()
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
 
@@ -11,27 +25,30 @@
 
 Supports history retrieval with the up arrow key, optional multi-line questions, and tokens counting.
 
 Slash (/) commands are available in the chat box to toggle multi-line submit mode, undo the last question and answer, modify the system prompt and more, see the available commands below for details.
 
 Supports saving chat messages to a JSON file and loading them from the file.
 
-![example](README.assets/small.gif)
+![example](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/small.gif)
 
 Uses the [gpt-3.5-turbo](https://platform.openai.com/docs/guides/chat/chat-completions-beta) model, which is the same model used by ChatGPT (Free Edition), as default.
 
 ## Changelog
 
-### 2023-04-15
-
-- Added the ability to create a line break in single-line mode using `Esc` + `Enter`
+### 2023-04-23
+Released `gpt-term` on [Pypi](https://pypi.org/project/gpt-term/), started version control. No need to clone the project locally anymore, simply use the `pip` command to install gpt-term.
 
 <details>
   <summary>More Change log</summary>
 
+### 2023-04-15
+
+- Added the ability to create a line break in single-line mode using `Esc` + `Enter`
+
 ### 2023-04-13
 
 - Added the function of generating and setting the terminal title in the background, and now the client will use the summary of the first question content as the terminal title
 
 ### 2023-04-09
 
 - Add filename generate function, client will suggest the summary of the first question as filename when save command executed.
@@ -65,102 +82,83 @@
 
 ## Preparation
 
 1. An OpenAI API key. You need to register an OpenAI account and obtain an API key.
 
    OpenAI's API key can be generated on the page opened by clicking "View API keys" in the upper right corner of the homepage, direct link: https://platform.openai.com/account/api-keys
 
-   ![image-20230303233352970](README.assets/image-20230303233352970.png)
+   ![image-20230303233352970](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/image-20230303233352970.png)
 
-2. [Python](https://www.python.org/downloads/) version 3.6 or higher.
-3. [git](https://git-scm.com/downloads)
+2. [Python](https://www.python.org/downloads/) version 3.7 or higher.
 
 ## Installation
 
-1. Clone the repo and enter the directory
 
-   ```shell
-   git clone https://github.com/xiaoxx970/chatgpt-in-terminal.git
-   cd ./chatgpt-in-terminal
-   ```
-   
-2. Rename the `.env.example` file in the current directory to `.env`.
+1. Install `GPT-Term` using `pip`
 
    ```shell
-   mv .env.example .env
+   pip3 install gpt-term
    ```
 
-   Edit the `.env` file and modify the `OPENAI_API_KEY` variable to your API Key.
+2. Configure the API Key
 
    ```shell
-   OPENAI_API_KEY=your_API_Key
+   gpt-term --set-apikey YOUR_API_KEY
    ```
 
-   > If the `.env` file is not configured, you can also enter the API Key directly at runtime, but it will only be effective for the current session.
-   
-3. Install the dependencies in the `requirements.txt` file using the `pip` command.
-
-   ```shell
-   pip3 install -r requirements.txt
-   ```
+   > If you don't configure the API Key now, you can enter it when prompted during runtime.
 
 ## Update
 
-If you want to update the script to the latest version, run the following command in this project's directory:
+To update `GPT-Term` to the latest version, run the following command in your terminal:
 
 ```sh
-git pull
-pip3 install -r requirements.txt
+pip3 install --upgrade gpt-term
 ```
 
-> If git error is reported
->
-> ```shell
-> error: Your local changes to the following files would be overwritten by merge:
->          .env
-> Please commit your changes or stash them before you merge.
-> Aborting
-> ```
->
-> Just untrack the .env file from git first (doesn't delete the local .env file)
->
-> ```sh
-> git rm --cache .env
-> ```
->
-> Then run the `git pull` command above 
+> If there is a new version, `GPT-Term` will prompt the user to update upon exiting.
 
 ## How to Use
 
 Run with the following command:
 
 ```shell
-python3 chat.py
+gpt-term
 ```
 
 When entering a question in single-line mode, use `Esc` + `Enter` to start a new line, and use `Enter` to submit the question.
 
-> Original chat logs will be saved to `chat.log`
+> Original chat logs will be saved to `~/.gpt-term/chat.log`
 
 ### Available Arguments
 
 | Arguments     | Description                     | Example                                       |
 | ------------- | ------------------------------- | --------------------------------------------- |
 | -h, --help    | show this help message and exit | `chat.py --help`                              |
 | --load FILE   | Load chat history from file     | `chat.py --load chat_history_code_check.json` |
 | --key API_KEY | choose the API key to load      | `chat.py --key OPENAI_API_KEY1`               |
 | --model MODEL | choose the AI model to use      | `chat.py --model gpt-3.5-turbo`               |
 | -m, --multi   | Enable multi-line mode          | `chat.py --multi`                             |
 | -r, --raw     | Enable raw mode                 | `chat.py --raw`                               |
+| --set-apikey KEY        | Set the OpenAI API key                                   | `gpt-term --set-apikey sk-xxx`   |
+| --set-timeout SEC       | Set the maximum wait time for API requests               | `gpt-term --set-timeout 10`      |
+| --set-gentitle BOOL     | Set whether to auto-generate a title for the chat        | `gpt-term --set-gentitle True`   |
+| --set-saveperfix PERFIX | Set the save prefix for chat history files               | `gpt-term --set-saveperfix chat_history_` |
+| --set-loglevel LEVEL    | Set the log level: DEBUG, INFO, WARNING, ERROR, CRITICAL | `gpt-term --set-loglevel DEBUG`  |
 
 > Multi-line mode and raw mode can be used simultaneously
 
-### `.env` configuration file
+### Configuration File
 
-```shell
+The configuration file is located at `~/.gpt-term/config.ini` and is autogenerated. It can be modified using the program's `--set` option or edited manually.
+
+The default configuration is as follows:
+
+```ini config.ini
+[DEFAULT]
 # API key for OpenAI
 OPENAI_API_KEY=
 
 # The maximum waiting time for API requests, the default is 30s
 OPENAI_API_TIMEOUT=30
 
 # Whether to automatically generate titles for conversations, enabled by default (generating titles will consume a small amount of tokens)
@@ -224,18 +222,20 @@
 
 - `/title [new_title]`: Set terminal title for this chat
 
   > If new_title is not provided, a new title will be generated based on first question
 
 - `/timeout [new_timeout]`: Modify API timeout.
 
-  > The default timeout is 30 seconds, it can also be configured by setting `OPENAI_API_TIMEOUT=` in the `.env` file.
+  > The default timeout is 30 seconds, it can also be configured by setting `OPENAI_API_TIMEOUT=` in the `~/.gpt-term/config.ini` file.
   
 - `/undo`: Delete the previous question and answer
 
+- `/version`: Display the local and remote versions of `GPT-Term`
+
 - `/help`: Display available commands
 
 - `/exit`: Exit the application
 
 ### Exit Words
 
 In the chat, use exit words to end the current session. Exit words include:
@@ -252,33 +252,41 @@
 
 > Current price: $0.002 / 1K tokens, Free Edition rate limit: 20 requests / min (`gpt-3.5-turbo`)
 
 ## Dependencies
 
 Thanks to the following projects for providing strong support for this script:
 
-- [rich](https://github.com/Textualize/rich): For rendering rich text in the terminal
-- [python-dotenv](https://github.com/theskumar/python-dotenv): For loading environment variables from `.env` file
+- [requests](https://github.com/psf/requests): For handling HTTP requests
+- [pyperclip](https://github.com/asweigart/pyperclip): A cross-platform clipboard operation library
+- [rich](https://github.com/willmcgugan/rich): For outputting rich text in the terminal
 - [prompt_toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit): Command-line input processing library
+- [sseclient-py](https://github.com/btubbs/sseclient-py): For implementing streaming output of answers
+- [tiktoken](https://github.com/OpenAI/tiktoken): A library for calculating and processing OpenAI API tokens
 
 ## Contributing
 
 Feel free to dive in! [Open an issue](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/new) or submit PRs.
 
 ### Contributors
 
 This project exists thanks to all the people who contribute. 
 <a href="https://github.com/xiaoxx970/chatgpt-in-terminal/graphs/contributors"><img src="https://opencollective.com/chatgpt-in-terminal/contributors.svg?width=890&button=false" /></a>
 
 ## Project Structure
 
-```bash
-├── README.md           # Documentation
-├── chat.py             # Project code
-├── requirements.txt    # Dependency package list
-├── chat.log            # Chat log generated after chatting
-└── .env                # Storage API key and other settings
+```sh
+.
+├── LICENSE                   # License
+├── README.md                 # Documentation
+├── chat.py                   # Script entry point
+├── config.ini                # API key storage and other settings
+├── gpt_term                  # Project package folder
+│   ├── __init__.py
+│   └── main.py               # Main program
+├── requirements.txt          # List of dependencies
+└── setup.py
 ```
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE).
+This project is licensed under the [MIT License](LICENSE).
```

### Comparing `gpt-term-0.9.1/chat.py` & `gpt-term-0.9.2/gpt_term/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,28 +16,30 @@
 from queue import Queue
 from typing import Dict, List
 
 import pyperclip
 import requests
 import sseclient
 import tiktoken
-from pkg_resources import get_distribution, parse_version, DistributionNotFound
+from packaging.version import parse as parse_version
 from prompt_toolkit import PromptSession, prompt
 from prompt_toolkit.completion import Completer, Completion
 from prompt_toolkit.key_binding import KeyBindings
 from prompt_toolkit.keys import Keys
 from prompt_toolkit.shortcuts import confirm
 from prompt_toolkit.styles import Style
 from prompt_toolkit.validation import ValidationError, Validator
 from rich import print as rprint
-from rich.console import Console
+from rich.console import Console, Group
 from rich.live import Live
 from rich.markdown import Markdown
 from rich.panel import Panel
 
+from . import __version__
+
 data_dir = os.path.expanduser("~") + "/.gpt-term"
 if not os.path.exists(data_dir):
     os.makedirs(data_dir)
     shutil.copy('config.ini', data_dir)
 
 # 日志记录到 chat.log，注释下面这行可不记录日志
 logging.basicConfig(filename=f'{data_dir}/chat.log', format='%(asctime)s %(name)s: %(levelname)-6s %(message)s',
@@ -48,15 +50,15 @@
 console = Console()
 
 style = Style.from_dict({
     "prompt": "ansigreen",  # 将提示符设置为绿色
 })
 
 remote_version = None
-local_version = None
+local_version = parse_version(__version__)
 threadlock_remote_version = threading.Lock()
 
 
 class ChatMode:
     raw_mode = False
     multi_line_mode = False
     stream_mode = True
@@ -779,16 +781,16 @@
                 console.print(
                     "[dim]Nothing to do. Avaliable delete command: `[bright_magenta]/delete first[/]` or `[bright_magenta]/delete all[/]`")
         else:
             chat_gpt.delete_first_conversation()
 
     elif command == '/version':
         threadlock_remote_version.acquire()
-        console.print(Panel(f"[bold blue]Local Version:[/]\t{str(local_version)}\n"
-                            f"[bold green]Remote Version:[/]\t{str(remote_version)}",
+        console.print(Panel(f"[bold blue]Local Version:[/]\tv{str(local_version)}\n"
+                            f"[bold green]Remote Version:[/]\tv{str(remote_version)}",
                             title='Version', title_align='left', width=28))
         threadlock_remote_version.release()
 
     elif command == '/exit':
         raise EOFError
 
     else:
@@ -845,49 +847,39 @@
         buffer = event.current_buffer
         if ChatMode.multi_line_mode:
             buffer.validate_and_handle()
         else:
             buffer.insert_text('\n')
 
     return key_bindings
-    
 
-def check_remote_update():
+
+def get_remote_version():
     global remote_version
-    response = requests.get(
-        url="https://api.github.com/repos/xiaoxx970/chatgpt-in-terminal/releases", timeout=10)
-    if response.status_code != 200:
+    try:
+        response = requests.get(
+            "https://pypi.org/pypi/gpt-term/json", timeout=10)
+        response.raise_for_status()
+        threadlock_remote_version.acquire()
+        remote_version = parse_version(response.json()["info"]["version"])
+        threadlock_remote_version.release()
+    except requests.RequestException as e:
         log.error("Get remote version failed")
+        log.exception(e)
         return
-    threadlock_remote_version.acquire()
-    remote_version = parse_version(response.json()[0]["tag_name"])
-    threadlock_remote_version.release()
-
-    # try:
-    #     response = requests.get(
-    #         "https://pypi.org/pypi/gpt-term/json", timeout=10)
-    #     response.raise_for_status()
-    #     threadlock_remote_version.acquire()
-    #     remote_version = parse_version(response.json()["info"]["version"])
-    #     threadlock_remote_version.release()
-    # except requests.RequestException as e:
-    #     log.error("Get remote version failed")
-    #     log.exception(e)
-    #     return
-
     log.debug(f"Remote version: {str(remote_version)}")
 
 
 def write_config(config_ini: ConfigParser):
     with open(f'{data_dir}/config.ini', 'w') as configfile:
         config_ini.write(configfile)
 
+
 def set_config_by_args(args: argparse.Namespace, config_ini: ConfigParser):
     config_need_to_set = {}
-
     if args.set_apikey:     config_need_to_set.update({"OPENAI_API_KEY"      : args.set_apikey})
     if args.set_timeout:    config_need_to_set.update({"OPENAI_API_TIMEOUT"  : args.set_timeout})
     if args.set_saveperfix: config_need_to_set.update({"CHAT_SAVE_PERFIX"    : args.set_saveperfix})
     if args.set_loglevel:   config_need_to_set.update({"LOG_LEVEL"           : args.set_loglevel})
     if args.set_gentitle:   config_need_to_set.update({"AUTO_GENERATE_TITLE" : args.set_gentitle})
 
     if len(config_need_to_set) == 0:
@@ -933,23 +925,18 @@
             f"[dim]Invalid log level: {e}, check config.ini file. Set log level to INFO.")
         log_level = logging.INFO
     log.setLevel(log_level)
     # log level set must be before debug logs, because default log level is INFO, and before new log level being set debug logs will not be written to log file
 
     log.info("GPT-Term start")
 
-    global local_version
-    if __name__ == "__main__":
-        local_version = 'unknown'
-    else:
-        local_version = parse_version(get_distribution('gpt-term').version)
     log.debug(f"Local version: {str(local_version)}")
     # get local version from pkg resource
 
-    check_remote_update_thread = threading.Thread(target=check_remote_update)
+    check_remote_update_thread = threading.Thread(target=get_remote_version)
     check_remote_update_thread.start()
     log.debug("Remote version get thread started")
     # try to get remote version and check update
 
     # if 'key' arg triggered, load the api key from config.ini with the given key-name;
     # otherwise load the api key with the key-name "OPENAI_API_KEY"
     if args.key:
@@ -1042,16 +1029,17 @@
             break
 
     log.info(f"Total tokens spent: {chat_gpt.total_tokens_spent}")
     console.print(
         f"[bright_magenta]Total tokens spent: [bold]{chat_gpt.total_tokens_spent}")
     
     threadlock_remote_version.acquire()
-    if remote_version and local_version !='unknown' and remote_version > local_version:
-        console.print(
-            f"New Version Available: [red]v{str(local_version)}[/] -> [green]v{str(remote_version)}[/]\n"
-            "Use `[bright_magenta]pip install --upgrade gpt-term[/]` to upgrade to latest version.\n"
-            "Visit our GitHub Site https://github.com/xiaoxx970/chatgpt-in-terminal to see what have been changed!")
+    if remote_version and remote_version > local_version:
+        console.print(Panel(Group(
+            Markdown("Use `pip install --upgrade gpt-term` to upgrade."),
+            Markdown("Visit our [GitHub Site](https://github.com/xiaoxx970/chatgpt-in-terminal) to see what have been changed!")),
+            title=f"New Version Available: [red]v{str(local_version)}[/] -> [green]v{str(remote_version)}[/]",
+            width=58, style="blue", title_align="left"))
     threadlock_remote_version.release()
 
 if __name__ == "__main__":
     main()
```

### Comparing `gpt-term-0.9.1/config.ini` & `gpt-term-0.9.2/config.ini`

 * *Files identical despite different names*

### Comparing `gpt-term-0.9.1/gpt_term.egg-info/PKG-INFO` & `gpt-term-0.9.2/gpt_term.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 0.9.1
+Version: 0.9.2
 Summary: Use ChatGPT in terminal
 Home-page: https://github.com/xiaoxx970/chatgpt-in-terminal
 Author: xiaoxx970
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Chat with GPT in Terminal
 
 [![English badge](https://img.shields.io/badge/%E8%8B%B1%E6%96%87-English-blue)](./README.md)
 [![简体中文 badge](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-Simplified%20Chinese-blue)](./README.zh-CN.md)
@@ -25,27 +25,30 @@
 
 Supports history retrieval with the up arrow key, optional multi-line questions, and tokens counting.
 
 Slash (/) commands are available in the chat box to toggle multi-line submit mode, undo the last question and answer, modify the system prompt and more, see the available commands below for details.
 
 Supports saving chat messages to a JSON file and loading them from the file.
 
-![example](README.assets/small.gif)
+![example](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/small.gif)
 
 Uses the [gpt-3.5-turbo](https://platform.openai.com/docs/guides/chat/chat-completions-beta) model, which is the same model used by ChatGPT (Free Edition), as default.
 
 ## Changelog
 
-### 2023-04-15
-
-- Added the ability to create a line break in single-line mode using `Esc` + `Enter`
+### 2023-04-23
+Released `gpt-term` on [Pypi](https://pypi.org/project/gpt-term/), started version control. No need to clone the project locally anymore, simply use the `pip` command to install gpt-term.
 
 <details>
   <summary>More Change log</summary>
 
+### 2023-04-15
+
+- Added the ability to create a line break in single-line mode using `Esc` + `Enter`
+
 ### 2023-04-13
 
 - Added the function of generating and setting the terminal title in the background, and now the client will use the summary of the first question content as the terminal title
 
 ### 2023-04-09
 
 - Add filename generate function, client will suggest the summary of the first question as filename when save command executed.
@@ -79,102 +82,83 @@
 
 ## Preparation
 
 1. An OpenAI API key. You need to register an OpenAI account and obtain an API key.
 
    OpenAI's API key can be generated on the page opened by clicking "View API keys" in the upper right corner of the homepage, direct link: https://platform.openai.com/account/api-keys
 
-   ![image-20230303233352970](README.assets/image-20230303233352970.png)
+   ![image-20230303233352970](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/image-20230303233352970.png)
 
-2. [Python](https://www.python.org/downloads/) version 3.6 or higher.
-3. [git](https://git-scm.com/downloads)
+2. [Python](https://www.python.org/downloads/) version 3.7 or higher.
 
 ## Installation
 
-1. Clone the repo and enter the directory
 
-   ```shell
-   git clone https://github.com/xiaoxx970/chatgpt-in-terminal.git
-   cd ./chatgpt-in-terminal
-   ```
-   
-2. Rename the `.env.example` file in the current directory to `.env`.
+1. Install `GPT-Term` using `pip`
 
    ```shell
-   mv .env.example .env
+   pip3 install gpt-term
    ```
 
-   Edit the `.env` file and modify the `OPENAI_API_KEY` variable to your API Key.
+2. Configure the API Key
 
    ```shell
-   OPENAI_API_KEY=your_API_Key
+   gpt-term --set-apikey YOUR_API_KEY
    ```
 
-   > If the `.env` file is not configured, you can also enter the API Key directly at runtime, but it will only be effective for the current session.
-   
-3. Install the dependencies in the `requirements.txt` file using the `pip` command.
-
-   ```shell
-   pip3 install -r requirements.txt
-   ```
+   > If you don't configure the API Key now, you can enter it when prompted during runtime.
 
 ## Update
 
-If you want to update the script to the latest version, run the following command in this project's directory:
+To update `GPT-Term` to the latest version, run the following command in your terminal:
 
 ```sh
-git pull
-pip3 install -r requirements.txt
+pip3 install --upgrade gpt-term
 ```
 
-> If git error is reported
->
-> ```shell
-> error: Your local changes to the following files would be overwritten by merge:
->          .env
-> Please commit your changes or stash them before you merge.
-> Aborting
-> ```
->
-> Just untrack the .env file from git first (doesn't delete the local .env file)
->
-> ```sh
-> git rm --cache .env
-> ```
->
-> Then run the `git pull` command above 
+> If there is a new version, `GPT-Term` will prompt the user to update upon exiting.
 
 ## How to Use
 
 Run with the following command:
 
 ```shell
-python3 chat.py
+gpt-term
 ```
 
 When entering a question in single-line mode, use `Esc` + `Enter` to start a new line, and use `Enter` to submit the question.
 
-> Original chat logs will be saved to `chat.log`
+> Original chat logs will be saved to `~/.gpt-term/chat.log`
 
 ### Available Arguments
 
 | Arguments     | Description                     | Example                                       |
 | ------------- | ------------------------------- | --------------------------------------------- |
 | -h, --help    | show this help message and exit | `chat.py --help`                              |
 | --load FILE   | Load chat history from file     | `chat.py --load chat_history_code_check.json` |
 | --key API_KEY | choose the API key to load      | `chat.py --key OPENAI_API_KEY1`               |
 | --model MODEL | choose the AI model to use      | `chat.py --model gpt-3.5-turbo`               |
 | -m, --multi   | Enable multi-line mode          | `chat.py --multi`                             |
 | -r, --raw     | Enable raw mode                 | `chat.py --raw`                               |
+| --set-apikey KEY        | Set the OpenAI API key                                   | `gpt-term --set-apikey sk-xxx`   |
+| --set-timeout SEC       | Set the maximum wait time for API requests               | `gpt-term --set-timeout 10`      |
+| --set-gentitle BOOL     | Set whether to auto-generate a title for the chat        | `gpt-term --set-gentitle True`   |
+| --set-saveperfix PERFIX | Set the save prefix for chat history files               | `gpt-term --set-saveperfix chat_history_` |
+| --set-loglevel LEVEL    | Set the log level: DEBUG, INFO, WARNING, ERROR, CRITICAL | `gpt-term --set-loglevel DEBUG`  |
 
 > Multi-line mode and raw mode can be used simultaneously
 
-### `.env` configuration file
+### Configuration File
 
-```shell
+The configuration file is located at `~/.gpt-term/config.ini` and is autogenerated. It can be modified using the program's `--set` option or edited manually.
+
+The default configuration is as follows:
+
+```ini config.ini
+[DEFAULT]
 # API key for OpenAI
 OPENAI_API_KEY=
 
 # The maximum waiting time for API requests, the default is 30s
 OPENAI_API_TIMEOUT=30
 
 # Whether to automatically generate titles for conversations, enabled by default (generating titles will consume a small amount of tokens)
@@ -238,18 +222,20 @@
 
 - `/title [new_title]`: Set terminal title for this chat
 
   > If new_title is not provided, a new title will be generated based on first question
 
 - `/timeout [new_timeout]`: Modify API timeout.
 
-  > The default timeout is 30 seconds, it can also be configured by setting `OPENAI_API_TIMEOUT=` in the `.env` file.
+  > The default timeout is 30 seconds, it can also be configured by setting `OPENAI_API_TIMEOUT=` in the `~/.gpt-term/config.ini` file.
   
 - `/undo`: Delete the previous question and answer
 
+- `/version`: Display the local and remote versions of `GPT-Term`
+
 - `/help`: Display available commands
 
 - `/exit`: Exit the application
 
 ### Exit Words
 
 In the chat, use exit words to end the current session. Exit words include:
@@ -266,33 +252,41 @@
 
 > Current price: $0.002 / 1K tokens, Free Edition rate limit: 20 requests / min (`gpt-3.5-turbo`)
 
 ## Dependencies
 
 Thanks to the following projects for providing strong support for this script:
 
-- [rich](https://github.com/Textualize/rich): For rendering rich text in the terminal
-- [python-dotenv](https://github.com/theskumar/python-dotenv): For loading environment variables from `.env` file
+- [requests](https://github.com/psf/requests): For handling HTTP requests
+- [pyperclip](https://github.com/asweigart/pyperclip): A cross-platform clipboard operation library
+- [rich](https://github.com/willmcgugan/rich): For outputting rich text in the terminal
 - [prompt_toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit): Command-line input processing library
+- [sseclient-py](https://github.com/btubbs/sseclient-py): For implementing streaming output of answers
+- [tiktoken](https://github.com/OpenAI/tiktoken): A library for calculating and processing OpenAI API tokens
 
 ## Contributing
 
 Feel free to dive in! [Open an issue](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/new) or submit PRs.
 
 ### Contributors
 
 This project exists thanks to all the people who contribute. 
 <a href="https://github.com/xiaoxx970/chatgpt-in-terminal/graphs/contributors"><img src="https://opencollective.com/chatgpt-in-terminal/contributors.svg?width=890&button=false" /></a>
 
 ## Project Structure
 
-```bash
-├── README.md           # Documentation
-├── chat.py             # Project code
-├── requirements.txt    # Dependency package list
-├── chat.log            # Chat log generated after chatting
-└── .env                # Storage API key and other settings
+```sh
+.
+├── LICENSE                   # License
+├── README.md                 # Documentation
+├── chat.py                   # Script entry point
+├── config.ini                # API key storage and other settings
+├── gpt_term                  # Project package folder
+│   ├── __init__.py
+│   └── main.py               # Main program
+├── requirements.txt          # List of dependencies
+└── setup.py
 ```
 
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
```

### Comparing `gpt-term-0.9.1/setup.py` & `gpt-term-0.9.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 from setuptools import find_packages, setup
+from gpt_term import __version__
 
 with open("README.md", 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 install_requires = [
     "requests",
     "pyperclip",
     "rich>=13.3.1",
     "prompt_toolkit>=3.0",
     "sseclient-py>=1.7.2",
-    "tiktoken"
+    "tiktoken",
+    "packaging"
 ]
 
 setup(
     name="gpt-term",
-    version="0.9.1",
+    version=__version__,
     author="xiaoxx970",
     description="Use ChatGPT in terminal",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xiaoxx970/chatgpt-in-terminal",
     license="MIT",
 
     packages=find_packages(),
     py_modules=["chat"],
     install_requires=install_requires,
     entry_points={
         "console_scripts": [
-            "gpt-term=chat:main"
+            "gpt-term=gpt_term.main:main"
         ]
     },
     data_files=[('', ['config.ini'])],
-    python_requires=">=3.8",
+    python_requires=">=3.7",
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ]
 )
```

