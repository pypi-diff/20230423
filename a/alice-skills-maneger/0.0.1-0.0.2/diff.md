# Comparing `tmp/alice_skills_maneger-0.0.1.tar.gz` & `tmp/alice-skills-maneger-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alice_skills_maneger-0.0.1.tar", last modified: Sat Apr 22 04:27:06 2023, max compression
+gzip compressed data, was "alice-skills-maneger-0.0.2.tar", last modified: Sat Apr 22 06:57:04 2023, max compression
```

## Comparing `alice_skills_maneger-0.0.1.tar` & `alice-skills-maneger-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 04:27:06.528880 alice_skills_maneger-0.0.1/
--rw-rw-rw-   0        0        0       17 2023-04-21 19:36:12.000000 alice_skills_maneger-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      732 2023-04-22 04:27:06.520794 alice_skills_maneger-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1254 2023-04-21 23:05:03.000000 alice_skills_maneger-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 04:27:06.504685 alice_skills_maneger-0.0.1/alice_skills_maneger.egg-info/
--rw-rw-rw-   0        0        0      732 2023-04-22 04:27:06.000000 alice_skills_maneger-0.0.1/alice_skills_maneger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-04-22 04:27:06.000000 alice_skills_maneger-0.0.1/alice_skills_maneger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 04:27:06.000000 alice_skills_maneger-0.0.1/alice_skills_maneger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-22 04:27:06.000000 alice_skills_maneger-0.0.1/alice_skills_maneger.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       66 2023-04-22 04:27:06.000000 alice_skills_maneger-0.0.1/alice_skills_maneger.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-22 04:27:06.000000 alice_skills_maneger-0.0.1/alice_skills_maneger.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-22 04:27:06.520794 alice_skills_maneger-0.0.1/asm/
--rw-rw-rw-   0        0        0      156 2023-04-21 20:38:56.000000 alice_skills_maneger-0.0.1/asm/__init__.py
--rw-rw-rw-   0        0        0     4073 2023-04-21 23:05:04.000000 alice_skills_maneger-0.0.1/asm/__main__.py
--rw-rw-rw-   0        0        0    20199 2023-04-21 23:05:00.000000 alice_skills_maneger-0.0.1/asm/alice_skills_manager.py
--rw-rw-rw-   0        0        0     2202 2023-04-21 22:58:17.000000 alice_skills_maneger-0.0.1/asm/exceptions.py
--rw-rw-rw-   0        0        0    19210 2023-04-21 22:58:25.000000 alice_skills_maneger-0.0.1/asm/skill_entry.py
--rw-rw-rw-   0        0        0     6581 2023-04-21 23:04:59.000000 alice_skills_maneger-0.0.1/asm/skill_repo.py
--rw-rw-rw-   0        0        0     2623 2023-04-21 23:04:58.000000 alice_skills_maneger-0.0.1/asm/skill_state.py
--rw-rw-rw-   0        0        0     2993 2023-04-21 22:58:21.000000 alice_skills_maneger-0.0.1/asm/util.py
--rw-rw-rw-   0        0        0       42 2023-04-22 04:27:06.528880 alice_skills_maneger-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1538 2023-04-22 04:25:55.000000 alice_skills_maneger-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:57:04.572166 alice-skills-maneger-0.0.2/
+-rw-rw-rw-   0        0        0       17 2023-04-21 19:36:12.000000 alice-skills-maneger-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      692 2023-04-22 06:57:04.572166 alice-skills-maneger-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1254 2023-04-21 23:05:03.000000 alice-skills-maneger-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 06:57:04.532164 alice-skills-maneger-0.0.2/alice_skills_manager/
+-rw-rw-rw-   0        0        0      173 2023-04-22 05:22:51.000000 alice-skills-maneger-0.0.2/alice_skills_manager/__init__.py
+-rw-rw-rw-   0        0        0     4124 2023-04-22 05:50:43.000000 alice-skills-maneger-0.0.2/alice_skills_manager/__main__.py
+-rw-rw-rw-   0        0        0    20301 2023-04-22 05:21:47.000000 alice-skills-maneger-0.0.2/alice_skills_manager/alice_skills_manager.py
+-rw-rw-rw-   0        0        0     2202 2023-04-21 22:58:17.000000 alice-skills-maneger-0.0.2/alice_skills_manager/exceptions.py
+-rw-rw-rw-   0        0        0    19261 2023-04-22 05:22:25.000000 alice-skills-maneger-0.0.2/alice_skills_manager/skill_entry.py
+-rw-rw-rw-   0        0        0     6632 2023-04-22 05:51:00.000000 alice-skills-maneger-0.0.2/alice_skills_manager/skill_repo.py
+-rw-rw-rw-   0        0        0     2623 2023-04-21 23:04:58.000000 alice-skills-maneger-0.0.2/alice_skills_manager/skill_state.py
+-rw-rw-rw-   0        0        0     2993 2023-04-21 22:58:21.000000 alice-skills-maneger-0.0.2/alice_skills_manager/util.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:57:04.572166 alice-skills-maneger-0.0.2/alice_skills_maneger.egg-info/
+-rw-rw-rw-   0        0        0      692 2023-04-22 06:57:04.000000 alice-skills-maneger-0.0.2/alice_skills_maneger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2023-04-22 06:57:04.000000 alice-skills-maneger-0.0.2/alice_skills_maneger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 06:57:04.000000 alice-skills-maneger-0.0.2/alice_skills_maneger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-22 06:57:04.000000 alice-skills-maneger-0.0.2/alice_skills_maneger.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       66 2023-04-22 06:57:04.000000 alice-skills-maneger-0.0.2/alice_skills_maneger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-22 06:57:04.000000 alice-skills-maneger-0.0.2/alice_skills_maneger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 06:57:04.572166 alice-skills-maneger-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1482 2023-04-22 06:20:45.000000 alice-skills-maneger-0.0.2/setup.py
```

### Comparing `alice_skills_maneger-0.0.1/PKG-INFO` & `alice-skills-maneger-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: alice_skills_maneger
-Version: 0.0.1
+Name: alice-skills-maneger
+Version: 0.0.2
 Summary: Alice Skills Manager
 Home-page: https://github.com/Alice-IA/alice-skills-manager
-Author: jarbasAI, Matthew Scholefield, Mycroft AI
-Author-email: jarbasai@mailfence.com, matthew331199@gmail.com, dev@mycroft.ai
+Author: jarbasAI, Alice-IA
+Author-email: jarbasai@mailfence.com, yuiassistant@gmail.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `alice_skills_maneger-0.0.1/README.md` & `alice-skills-maneger-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alice_skills_maneger-0.0.1/alice_skills_maneger.egg-info/PKG-INFO` & `alice-skills-maneger-0.0.2/alice_skills_maneger.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: alice-skills-maneger
-Version: 0.0.1
+Version: 0.0.2
 Summary: Alice Skills Manager
 Home-page: https://github.com/Alice-IA/alice-skills-manager
-Author: jarbasAI, Matthew Scholefield, Mycroft AI
-Author-email: jarbasai@mailfence.com, matthew331199@gmail.com, dev@mycroft.ai
+Author: jarbasAI, Alice-IA
+Author-email: jarbasai@mailfence.com, yuiassistant@gmail.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `alice_skills_maneger-0.0.1/asm/__main__.py` & `alice-skills-maneger-0.0.2/alice_skills_manager/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import sys
 from logging import ERROR, INFO
 
-from asm.exceptions import AsmException
-from asm.alice_skills_manager import AliceSkillsManager
-from asm.skill_repo import SkillRepo
+from alice_skills_manager.exceptions import AsmException
+from alice_skills_manager.alice_skills_manager import AliceSkillsManager
+from alice_skills_manager.skill_repo import SkillRepo
 
 LOG = logging.getLogger(__name__)
 
 
 def get_error_code(error_cls):
     return 1 + (sum(map(ord, error_cls.__name__)) % 255)
```

### Comparing `alice_skills_maneger-0.0.1/asm/alice_skills_manager.py` & `alice-skills-maneger-0.0.2/alice_skills_manager/alice_skills_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 from functools import wraps
 from glob import glob
 from os import path
 from typing import Dict, List
 
 from xdg import BaseDirectory
 
-from asm import GitException
-from asm.exceptions import (
+from alice_skills_manager import GitException
+from alice_skills_manager.exceptions import (
     AlreadyInstalled,
     AlreadyRemoved,
     AsmException,
     MultipleSkillMatches,
     RemoveException,
     SkillNotFound
 )
-from asm.skill_entry import SkillEntry
-from asm.skill_repo import SkillRepo
-from asm.skill_state import (
+from alice_skills_manager.skill_entry import SkillEntry
+from alice_skills_manager.skill_repo import SkillRepo
+from alice_skills_manager.skill_state import (
     initialize_skill_state,
     get_skill_state,
     write_device_skill_state,
     load_device_skill_state,
     device_skill_state_hash
 )
-from asm.util import cached_property, AsmProcessLock
+from alice_skills_manager.util import cached_property, AsmProcessLock
 
 LOG = logging.getLogger(__name__)
 
 CURRENT_SKILLS_DATA_VERSION = 2
 ONE_DAY = 86400
```

### Comparing `alice_skills_maneger-0.0.1/asm/exceptions.py` & `alice-skills-maneger-0.0.2/alice_skills_manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `alice_skills_maneger-0.0.1/asm/skill_entry.py` & `alice-skills-maneger-0.0.2/alice_skills_manager/skill_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from shutil import rmtree, move
 from subprocess import PIPE, Popen
 from tempfile import mktemp, gettempdir
 from threading import Lock
 from typing import Callable
 from pako import PakoManager
 
-from asm import SkillRequirementsException, git_to_asm_exceptions
-from asm.exceptions import PipRequirementsException, \
+from alice_skills_manager import SkillRequirementsException, git_to_asm_exceptions
+from alice_skills_manager.exceptions import PipRequirementsException, \
     SystemRequirementsException, AlreadyInstalled, SkillModified, \
     AlreadyRemoved, RemoveException, CloneException, NotInstalled, GitException
-from asm.util import cached_property, Git
+from alice_skills_manager.util import cached_property, Git
 
 LOG = logging.getLogger(__name__)
 
 # Branches which can be switched from when updating
 # TODO Make this configurable
 SWITCHABLE_BRANCHES = ['master']
```

### Comparing `alice_skills_maneger-0.0.1/asm/skill_repo.py` & `alice-skills-maneger-0.0.2/alice_skills_manager/skill_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import json
 from tempfile import gettempdir
 
 from xdg import BaseDirectory
 from git import Repo
 from git.exc import GitCommandError, GitError
 
-from asm import git_to_asm_exceptions
-from asm.exceptions import AsmException
-from asm.util import cached_property, Git
+from alice_skills_manager import git_to_asm_exceptions
+from alice_skills_manager.exceptions import AsmException
+from alice_skills_manager.util import cached_property, Git
 import logging
 import requests
 
 LOG = logging.getLogger(__name__)
 
 ALICE_SKILLS_DATA = ("https://raw.githubusercontent.com/"
                        "MycroftAI/mycroft-skills-data")
```

### Comparing `alice_skills_maneger-0.0.1/asm/skill_state.py` & `alice-skills-maneger-0.0.2/alice_skills_manager/skill_state.py`

 * *Files identical despite different names*

### Comparing `alice_skills_maneger-0.0.1/asm/util.py` & `alice-skills-maneger-0.0.2/alice_skills_manager/util.py`

 * *Files identical despite different names*

### Comparing `alice_skills_maneger-0.0.1/setup.py` & `alice-skills-maneger-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,42 +2,41 @@
 
 from setuptools import setup
 
 BASEDIR = os.path.abspath(os.path.dirname(__file__))
 
 def required(requirements_file):
     """ Read requirements file and remove comments and empty lines. """
-    with open(os.path.join(BASEDIR, requirements_file), 'r') as file_handler:
-        requirements = file_handler.read().splitlines()
+    with open(os.path.join(BASEDIR, requirements_file), 'r') as file_r:
+        requirements = file_r.read().splitlines()
         return [pkg for pkg in requirements
                 if pkg.strip() and not pkg.startswith("#")]
 
 
 setup(
-    name='alice_skills_maneger',
-    version='0.0.1',
-    packages=['asm'],
+    name='alice-skills-maneger',
+    version='0.0.2',
+    packages=['alice_skills_manager'],
     install_requires=required('requirements/requirements.txt'),
     tests_require=required('requirements/tests.txt'),
     python_requires='>=3.6',
     url='https://github.com/Alice-IA/alice-skills-manager',
     license='Apache-2.0',
-    author='jarbasAI, Matthew Scholefield, Mycroft AI',
-    author_email='jarbasai@mailfence.com, matthew331199@gmail.com, '
-                 'dev@mycroft.ai',
+    author='jarbasAI, Alice-IA',
+    author_email='jarbasai@mailfence.com, yuiassistant@gmail.com',
     description='Alice Skills Manager',
     long_description_content_type="text/markdown",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     entry_points={
         'console_scripts': {
-            'alice_skills_maneger=asm.__main__:main'
+            'asm=alice_skills_manager.__main__:main'
         }
     },
 )
```

