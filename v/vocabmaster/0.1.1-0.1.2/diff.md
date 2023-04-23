# Comparing `tmp/vocabmaster-0.1.1.tar.gz` & `tmp/vocabmaster-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocabmaster-0.1.1.tar", last modified: Sun Apr 23 16:52:20 2023, max compression
+gzip compressed data, was "vocabmaster-0.1.2.tar", last modified: Sun Apr 23 17:59:58 2023, max compression
```

## Comparing `vocabmaster-0.1.1.tar` & `vocabmaster-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 16:52:20.915228 vocabmaster-0.1.1/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-08 02:37:38.000000 vocabmaster-0.1.1/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2661 2023-04-23 16:52:20.915228 vocabmaster-0.1.1/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2528 2023-04-23 16:24:36.000000 vocabmaster-0.1.1/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-04-23 16:52:20.915228 vocabmaster-0.1.1/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-04-23 16:50:11.000000 vocabmaster-0.1.1/setup.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 16:52:20.915228 vocabmaster-0.1.1/vocabmaster/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-04-09 03:24:19.000000 vocabmaster-0.1.1/vocabmaster/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17800 2023-04-23 15:46:10.000000 vocabmaster-0.1.1/vocabmaster/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4200 2023-04-16 12:02:38.000000 vocabmaster-0.1.1/vocabmaster/config_handler.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    10681 2023-04-16 12:02:38.000000 vocabmaster-0.1.1/vocabmaster/csv_handler.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5606 2023-04-23 14:36:17.000000 vocabmaster-0.1.1/vocabmaster/gpt_integration.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7282 2023-04-20 14:45:02.000000 vocabmaster-0.1.1/vocabmaster/utils.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 16:52:20.915228 vocabmaster-0.1.1/vocabmaster.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2661 2023-04-23 16:52:20.000000 vocabmaster-0.1.1/vocabmaster.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      390 2023-04-23 16:52:20.000000 vocabmaster-0.1.1/vocabmaster.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-04-23 16:52:20.000000 vocabmaster-0.1.1/vocabmaster.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-04-23 16:52:20.000000 vocabmaster-0.1.1/vocabmaster.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      277 2023-04-23 16:52:20.000000 vocabmaster-0.1.1/vocabmaster.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-04-23 16:52:20.000000 vocabmaster-0.1.1/vocabmaster.egg-info/top_level.txt
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 17:59:58.735184 vocabmaster-0.1.2/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-08 02:37:38.000000 vocabmaster-0.1.2/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2693 2023-04-23 17:59:58.725184 vocabmaster-0.1.2/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2560 2023-04-23 17:55:42.000000 vocabmaster-0.1.2/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-04-23 17:59:58.735184 vocabmaster-0.1.2/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-04-23 17:59:52.000000 vocabmaster-0.1.2/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 17:59:58.725184 vocabmaster-0.1.2/vocabmaster/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-04-09 03:24:19.000000 vocabmaster-0.1.2/vocabmaster/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    18035 2023-04-23 17:51:07.000000 vocabmaster-0.1.2/vocabmaster/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4200 2023-04-16 12:02:38.000000 vocabmaster-0.1.2/vocabmaster/config_handler.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    10681 2023-04-16 12:02:38.000000 vocabmaster-0.1.2/vocabmaster/csv_handler.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5606 2023-04-23 14:36:17.000000 vocabmaster-0.1.2/vocabmaster/gpt_integration.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7282 2023-04-20 14:45:02.000000 vocabmaster-0.1.2/vocabmaster/utils.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 17:59:58.725184 vocabmaster-0.1.2/vocabmaster.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2693 2023-04-23 17:59:58.000000 vocabmaster-0.1.2/vocabmaster.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      390 2023-04-23 17:59:58.000000 vocabmaster-0.1.2/vocabmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-04-23 17:59:58.000000 vocabmaster-0.1.2/vocabmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-04-23 17:59:58.000000 vocabmaster-0.1.2/vocabmaster.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      277 2023-04-23 17:59:58.000000 vocabmaster-0.1.2/vocabmaster.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-04-23 17:59:58.000000 vocabmaster-0.1.2/vocabmaster.egg-info/top_level.txt
```

### Comparing `vocabmaster-0.1.1/LICENSE` & `vocabmaster-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.1/PKG-INFO` & `vocabmaster-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: vocabmaster
-Version: 0.1.1
-Author: sderev
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # VocabMaster
 
 Master new languages with this user-friendly CLI tool, designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience.
 
 ## Features
 
 * Record vocabulary words with ease
@@ -27,19 +20,19 @@
 
 You can install VocabMaster using pip. The package includes all the required dependencies. Simply run the following command:
 
 ```
 pip install vocabmaster
 ```
 
-### Install via pipx (recommended)
+### Install via `pipx` (recommended)
 
-pipx is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. We recommend using pipx to install VocabMaster.
+`pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. We recommend using `pipx` to install VocabMaster.
 
-First, install pipx if you haven't already:
+**First, install `pipx` if you haven't already:**
 
 * On macOS and Linux:
 
   ```
   python3 -m pip install --user pipx
   python3 -m pipx ensurepath
   ```
@@ -47,22 +40,24 @@
 * On Windows:
 
   ```
   py -m pip install --user pipx
   py -m pipx ensurepath
   ```
 
-Once pipx is installed, you can install VocabMaster using the following command:
+**Once `pipx` is installed, you can install VocabMaster using the following command:**
 
 ```
 pipx install vocabmaster
 ```
 
 ### Shell Completion
 
+You should have autocompletion after the installation. If that's not the case, you can follow the instructions below.
+
 To enable shell completion for bash or zsh, source the completion file (see the `completion` folder) related to your shell by adding the following line to your `.bashrc` or `.zshrc` file:
 
 #### For bash:
 
 ```
 source /path/to/vocabmaster/completion/vocabmaster.bash
 ```
@@ -77,33 +72,31 @@
 
 ## Usage
 
 Before using VocabMaster, you need to set up the OpenAI API key, which is required for the translations and usage examples. Follow the instructions provided within the CLI tool to configure the API key.
 
 Below is an example of common commands and their usage:
 
-1. Set up a new language pair:
+### Set up a new language pair:
 
 ```
 vocabmaster setup
 ```
 
-2. Add words to your vocabulary list:
+### Add words to your vocabulary list:
 
 ```
 vocabmaster add to have
 ```
 
-3. Generate an Anki deck from your vocabulary list:
+### Generate an Anki deck from your vocabulary list:
 
 ```
 vocabmaster translate
 ```
 
-For detailed help on each command, run:
+### For detailed help on each command, run:
 
 ```
 vocabmaster <command> --help
 ```
 
-For more information, please visit the [VocabMaster GitHub repository](https://github.com/sderev/vocabmaster).
-
```

### Comparing `vocabmaster-0.1.1/README.md` & `vocabmaster-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: vocabmaster
+Version: 0.1.2
+Author: sderev
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # VocabMaster
 
 Master new languages with this user-friendly CLI tool, designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience.
 
 ## Features
 
 * Record vocabulary words with ease
@@ -20,19 +27,19 @@
 
 You can install VocabMaster using pip. The package includes all the required dependencies. Simply run the following command:
 
 ```
 pip install vocabmaster
 ```
 
-### Install via pipx (recommended)
+### Install via `pipx` (recommended)
 
-pipx is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. We recommend using pipx to install VocabMaster.
+`pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. We recommend using `pipx` to install VocabMaster.
 
-First, install pipx if you haven't already:
+**First, install `pipx` if you haven't already:**
 
 * On macOS and Linux:
 
   ```
   python3 -m pip install --user pipx
   python3 -m pipx ensurepath
   ```
@@ -40,22 +47,24 @@
 * On Windows:
 
   ```
   py -m pip install --user pipx
   py -m pipx ensurepath
   ```
 
-Once pipx is installed, you can install VocabMaster using the following command:
+**Once `pipx` is installed, you can install VocabMaster using the following command:**
 
 ```
 pipx install vocabmaster
 ```
 
 ### Shell Completion
 
+You should have autocompletion after the installation. If that's not the case, you can follow the instructions below.
+
 To enable shell completion for bash or zsh, source the completion file (see the `completion` folder) related to your shell by adding the following line to your `.bashrc` or `.zshrc` file:
 
 #### For bash:
 
 ```
 source /path/to/vocabmaster/completion/vocabmaster.bash
 ```
@@ -70,33 +79,31 @@
 
 ## Usage
 
 Before using VocabMaster, you need to set up the OpenAI API key, which is required for the translations and usage examples. Follow the instructions provided within the CLI tool to configure the API key.
 
 Below is an example of common commands and their usage:
 
-1. Set up a new language pair:
+### Set up a new language pair:
 
 ```
 vocabmaster setup
 ```
 
-2. Add words to your vocabulary list:
+### Add words to your vocabulary list:
 
 ```
 vocabmaster add to have
 ```
 
-3. Generate an Anki deck from your vocabulary list:
+### Generate an Anki deck from your vocabulary list:
 
 ```
 vocabmaster translate
 ```
 
-For detailed help on each command, run:
+### For detailed help on each command, run:
 
 ```
 vocabmaster <command> --help
 ```
 
-For more information, please visit the [VocabMaster GitHub repository](https://github.com/sderev/vocabmaster).
-
```

### Comparing `vocabmaster-0.1.1/setup.py` & `vocabmaster-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = file.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = [line.strip() for line in file]
 
 setup(
     name="vocabmaster",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "vocabmaster = vocabmaster.cli:vocabmaster",
         ]
     },
```

### Comparing `vocabmaster-0.1.1/vocabmaster/cli.py` & `vocabmaster-0.1.2/vocabmaster/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -513,17 +513,25 @@
     )
 
 
 def print_all_language_pairs():
     """
     Print all the language pairs that have been set up.
     """
-    click.echo()
     click.echo(f"{BLUE}The following language pairs have been set up:{RESET}")
     language_pairs = config_handler.get_all_language_pairs()
     for idx, language_pair in enumerate(language_pairs, start=1):
         click.echo(
             f"{idx}."
             f" {language_pair['language_to_learn']}:{language_pair['mother_tongue']}"
         )
     click.echo()
 
+vocabmaster.add_command(config)
+vocabmaster.add_command(anki)
+vocabmaster.add_command(translate)
+vocabmaster.add_command(add)
+vocabmaster.add_command(anki)
+vocabmaster.add_command(default)
+vocabmaster.add_command(show)
+vocabmaster.add_command(tokens)
+
```

### Comparing `vocabmaster-0.1.1/vocabmaster/config_handler.py` & `vocabmaster-0.1.2/vocabmaster/config_handler.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.1/vocabmaster/csv_handler.py` & `vocabmaster-0.1.2/vocabmaster/csv_handler.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.1/vocabmaster/gpt_integration.py` & `vocabmaster-0.1.2/vocabmaster/gpt_integration.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.1/vocabmaster/utils.py` & `vocabmaster-0.1.2/vocabmaster/utils.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.1/vocabmaster.egg-info/PKG-INFO` & `vocabmaster-0.1.2/vocabmaster.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocabmaster
-Version: 0.1.1
+Version: 0.1.2
 Author: sderev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VocabMaster
 
 Master new languages with this user-friendly CLI tool, designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience.
@@ -27,19 +27,19 @@
 
 You can install VocabMaster using pip. The package includes all the required dependencies. Simply run the following command:
 
 ```
 pip install vocabmaster
 ```
 
-### Install via pipx (recommended)
+### Install via `pipx` (recommended)
 
-pipx is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. We recommend using pipx to install VocabMaster.
+`pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. We recommend using `pipx` to install VocabMaster.
 
-First, install pipx if you haven't already:
+**First, install `pipx` if you haven't already:**
 
 * On macOS and Linux:
 
   ```
   python3 -m pip install --user pipx
   python3 -m pipx ensurepath
   ```
@@ -47,22 +47,24 @@
 * On Windows:
 
   ```
   py -m pip install --user pipx
   py -m pipx ensurepath
   ```
 
-Once pipx is installed, you can install VocabMaster using the following command:
+**Once `pipx` is installed, you can install VocabMaster using the following command:**
 
 ```
 pipx install vocabmaster
 ```
 
 ### Shell Completion
 
+You should have autocompletion after the installation. If that's not the case, you can follow the instructions below.
+
 To enable shell completion for bash or zsh, source the completion file (see the `completion` folder) related to your shell by adding the following line to your `.bashrc` or `.zshrc` file:
 
 #### For bash:
 
 ```
 source /path/to/vocabmaster/completion/vocabmaster.bash
 ```
@@ -77,33 +79,31 @@
 
 ## Usage
 
 Before using VocabMaster, you need to set up the OpenAI API key, which is required for the translations and usage examples. Follow the instructions provided within the CLI tool to configure the API key.
 
 Below is an example of common commands and their usage:
 
-1. Set up a new language pair:
+### Set up a new language pair:
 
 ```
 vocabmaster setup
 ```
 
-2. Add words to your vocabulary list:
+### Add words to your vocabulary list:
 
 ```
 vocabmaster add to have
 ```
 
-3. Generate an Anki deck from your vocabulary list:
+### Generate an Anki deck from your vocabulary list:
 
 ```
 vocabmaster translate
 ```
 
-For detailed help on each command, run:
+### For detailed help on each command, run:
 
 ```
 vocabmaster <command> --help
 ```
 
-For more information, please visit the [VocabMaster GitHub repository](https://github.com/sderev/vocabmaster).
-
```

