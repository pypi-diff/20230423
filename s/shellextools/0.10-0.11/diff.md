# Comparing `tmp/shellextools-0.10.tar.gz` & `tmp/shellextools-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellextools-0.10.tar", last modified: Sat Apr 22 12:06:12 2023, max compression
+gzip compressed data, was "shellextools-0.11.tar", last modified: Sun Apr 23 15:56:17 2023, max compression
```

## Comparing `shellextools-0.10.tar` & `shellextools-0.11.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 12:06:12.341042 shellextools-0.10/
--rw-rw-rw-   0        0        0     1148 2023-04-22 12:05:54.000000 shellextools-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      137 2023-04-22 12:05:52.000000 shellextools-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     3573 2023-04-22 12:06:12.341042 shellextools-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     2923 2023-04-22 12:04:58.000000 shellextools-0.10/README.md
--rw-rw-rw-   0        0        0       85 2023-04-22 12:06:12.342041 shellextools-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1899 2023-04-22 12:06:11.000000 shellextools-0.10/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 12:06:12.336056 shellextools-0.10/shellextools/
--rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 shellextools-0.10/shellextools/LICENSE
--rw-rw-rw-   0        0        0     2923 2023-04-22 12:04:58.000000 shellextools-0.10/shellextools/README.md
--rw-rw-rw-   0        0        0    47555 2023-04-22 11:58:23.000000 shellextools-0.10/shellextools/__init__.py
--rw-rw-rw-   0        0        0      267 2023-04-22 12:06:11.000000 shellextools-0.10/shellextools/requirements.txt
--rw-rw-rw-   0        0        0     8735 2023-04-22 12:06:11.000000 shellextools-0.10/shellextools/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-22 12:06:12.340045 shellextools-0.10/shellextools.egg-info/
--rw-rw-rw-   0        0        0     3573 2023-04-22 12:06:12.000000 shellextools-0.10/shellextools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-04-22 12:06:12.000000 shellextools-0.10/shellextools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 12:06:12.000000 shellextools-0.10/shellextools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      255 2023-04-22 12:06:12.000000 shellextools-0.10/shellextools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-22 12:06:12.000000 shellextools-0.10/shellextools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 15:56:17.208249 shellextools-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-04-23 15:56:03.000000 shellextools-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      209 2023-04-23 15:56:03.000000 shellextools-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     3573 2023-04-23 15:56:17.208249 shellextools-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2923 2023-04-22 12:39:53.000000 shellextools-0.11/README.md
+-rw-rw-rw-   0        0        0       85 2023-04-23 15:56:17.209247 shellextools-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1861 2023-04-23 15:56:16.000000 shellextools-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 15:56:17.203235 shellextools-0.11/shellextools/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 shellextools-0.11/shellextools/LICENSE
+-rw-rw-rw-   0        0        0     2923 2023-04-22 12:39:53.000000 shellextools-0.11/shellextools/README.md
+-rw-rw-rw-   0        0        0    47690 2023-04-23 15:38:04.000000 shellextools-0.11/shellextools/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-04-23 15:51:51.000000 shellextools-0.11/shellextools/getmultifiles.py
+-rw-rw-rw-   0        0        0     2555 2023-04-23 15:50:28.000000 shellextools-0.11/shellextools/loggax3.py
+-rw-rw-rw-   0        0        0      248 2023-04-23 15:56:16.000000 shellextools-0.11/shellextools/requirements.txt
+-rw-rw-rw-   0        0        0     9983 2023-04-23 15:56:16.000000 shellextools-0.11/shellextools/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-23 15:56:17.207252 shellextools-0.11/shellextools.egg-info/
+-rw-rw-rw-   0        0        0     3573 2023-04-23 15:56:16.000000 shellextools-0.11/shellextools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-04-23 15:56:17.000000 shellextools-0.11/shellextools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 15:56:16.000000 shellextools-0.11/shellextools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      236 2023-04-23 15:56:16.000000 shellextools-0.11/shellextools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-23 15:56:16.000000 shellextools-0.11/shellextools.egg-info/top_level.txt
```

### Comparing `shellextools-0.10/LICENSE.rst` & `shellextools-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `shellextools-0.10/PKG-INFO` & `shellextools-0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellextools
-Version: 0.10
+Version: 0.11
 Summary: Adds Python functions/methods to the Windows context menu
 Home-page: https://github.com/hansalemaos/shellextools
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: Windows context menu,python,nutika
 Classifier: Development Status :: 4 - Beta
```

### Comparing `shellextools-0.10/README.md` & `shellextools-0.11/README.md`

 * *Files identical despite different names*

### Comparing `shellextools-0.10/setup.py` & `shellextools-0.11/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''Adds Python functions/methods to the Windows context menu'''
 
 # Setting up
 setup(
     name="shellextools",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/shellextools',
     author="Johannes Fischer",
     author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
 long_description = long_description,
 long_description_content_type="text/markdown",
-    #packages=['amiadmin', 'ctypestoast', 'downloadunzip', 'escape_windows_filepath', 'flatten_any_dict_iterable_or_whatsoever', 'flatten_everything', 'isiter', 'list_all_files_recursively', 'list_files_with_timestats', 'reggisearch', 'subprocess_alive', 'subprocesskiller', 'tolerant_isinstance', 'touchtouch'],
+    #packages=['amiadmin', 'ctypestoast', 'downloadunzip', 'escape_windows_filepath', 'flatten_any_dict_iterable_or_whatsoever', 'flatten_everything', 'hackyargparser', 'isiter', 'list_all_files_recursively', 'lockexclusive', 'ordered_set', 'reggisearch', 'tolerant_isinstance', 'touchtouch'],
     keywords=['Windows context menu', 'python', 'nutika'],
     classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
-    install_requires=['amiadmin', 'ctypestoast', 'downloadunzip', 'escape_windows_filepath', 'flatten_any_dict_iterable_or_whatsoever', 'flatten_everything', 'isiter', 'list_all_files_recursively', 'list_files_with_timestats', 'reggisearch', 'subprocess_alive', 'subprocesskiller', 'tolerant_isinstance', 'touchtouch'],
+    install_requires=['amiadmin', 'ctypestoast', 'downloadunzip', 'escape_windows_filepath', 'flatten_any_dict_iterable_or_whatsoever', 'flatten_everything', 'hackyargparser', 'isiter', 'list_all_files_recursively', 'lockexclusive', 'ordered_set', 'reggisearch', 'tolerant_isinstance', 'touchtouch'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```

### Comparing `shellextools-0.10/shellextools/LICENSE` & `shellextools-0.11/shellextools/LICENSE`

 * *Files identical despite different names*

### Comparing `shellextools-0.10/shellextools/README.md` & `shellextools-0.11/shellextools/README.md`

 * *Files identical despite different names*

### Comparing `shellextools-0.10/shellextools/__init__.py` & `shellextools-0.11/shellextools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,34 +11,45 @@
 from escape_windows_filepath import escape_windows_path
 from flatten_any_dict_iterable_or_whatsoever import (
     fla_tu,
 )
 from flatten_everything import flatten_everything
 from functools import reduce, partial
 from isiter import isiter
-from list_files_with_timestats import (
-    get_folder_file_complete_path,
-)
 from tolerant_isinstance import isinstance_tolerant
 from touchtouch import touch
 from typing import Union, List, Optional
 import isiter
 import os
 import pickle
 import re
 import shutil
 import stat
 import tempfile
-from subprocess_alive import is_process_alive
-from subprocesskiller import get_pro_properties, subprocess_timeout, kill_process_children_parents, kill_subprocs, kill_pid
 from amiadmin import am_i_admin
 from downloadunzip import extract,copy_folder_to_another_folder,zip_folder,download_and_extract
 from list_all_files_recursively import get_folder_file_complete_path
 from reggisearch import search_values
 from ctypestoast import show_notification,show_notification_threaded
+from time import sleep as sleep_
+from math import floor
+
+
+def sleep(secs):
+    if secs == 0:
+        return
+    maxrange = 50 * secs
+    if isinstance(maxrange, float):
+        sleeplittle = floor(maxrange)
+        sleep_((maxrange - sleeplittle) / 50)
+        maxrange = int(sleeplittle)
+    if maxrange > 0:
+        for _ in range(maxrange):
+            sleep_(0.016)
+
 
 nested_dict = lambda: defaultdict(nested_dict)
 MB_OK = 0x0
 MB_OKCXL = 0x01
 MB_YESNOCXL = 0x03
 MB_YESNO = 0x04
 MB_HELP = 0x4000
```

### Comparing `shellextools-0.10/shellextools/thirdparty.json` & `shellextools-0.11/shellextools/thirdparty.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.828125%*

 * *Differences: {'5': "{'Name': 'lockexclusive'}",*

 * * '6': "{'Name': 'reggisearch', 'Version': '0.10'}",*

 * * 'insert': "[(3, OrderedDict([('License', 'MIT'), ('LicenseText', '\\n\\n The MIT License "*

 * *           '(MIT)\\n\\n Copyright (c) 2023 Johannes Fischer\\n\\n \\n\\n Permission is hereby '*

 * *           'granted, free of charge, to any person obtaining a copy\\n\\n of this software and '*

 * *           'associated documentation files (the "Software"), to deal\\n\\n in the Software without '*

 * *           'restriction, including with […]*

```diff
@@ -15,29 +15,35 @@
         "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2023 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
         "Name": "downloadunzip",
         "Version": "0.10"
     },
     {
         "License": "MIT",
+        "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2023 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
+        "Name": "hackyargparser",
+        "Version": "0.12"
+    },
+    {
+        "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2022 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
         "Name": "isiter",
         "Version": "0.10"
     },
     {
         "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2023 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
-        "Name": "reggisearch",
+        "Name": "lockexclusive",
         "Version": "0.10"
     },
     {
         "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2023 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
-        "Name": "subprocesskiller",
-        "Version": "0.11"
+        "Name": "reggisearch",
+        "Version": "0.10"
     },
     {
         "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2022 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
         "Name": "touchtouch",
         "Version": "0.11"
     }
```

### Comparing `shellextools-0.10/shellextools.egg-info/PKG-INFO` & `shellextools-0.11/shellextools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellextools
-Version: 0.10
+Version: 0.11
 Summary: Adds Python functions/methods to the Windows context menu
 Home-page: https://github.com/hansalemaos/shellextools
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: Windows context menu,python,nutika
 Classifier: Development Status :: 4 - Beta
```

