# Comparing `tmp/alacorder-79.7.0.tar.gz` & `tmp/alacorder-79.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-79.7.0.tar", max compression
+gzip compressed data, was "alacorder-79.7.1.tar", max compression
```

## Comparing `alacorder-79.7.0.tar` & `alacorder-79.7.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.7.0/LICENSE
--rw-r--r--   0        0        0     9378 2023-04-22 21:04:19.345850 alacorder-79.7.0/README.md
--rw-r--r--   0        0        0      679 2023-04-23 16:40:28.032022 alacorder-79.7.0/pyproject.toml
--rw-r--r--   0        0        0     9208 2023-04-21 18:06:44.921207 alacorder-79.7.0/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb
--rw-r--r--   0        0        0   138382 2023-04-21 18:24:49.412475 alacorder-79.7.0/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.7.0/src/alacorder/.python-version
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.7.0/src/alacorder/__init__.py
--rw-r--r--   0        0        0   139978 2023-04-23 16:40:07.746618 alacorder-79.7.0/src/alacorder/__main__.py
--rw-r--r--   0        0        0   139978 2023-04-23 16:40:14.007977 alacorder-79.7.0/src/alacorder/alac.py
--rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.7.0/src/alacorder/~$E 302 Portfolio.docx
--rw-r--r--   0        0        0    10268 1970-01-01 00:00:00.000000 alacorder-79.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.7.1/LICENSE
+-rw-r--r--   0        0        0     9378 2023-04-22 21:04:19.345850 alacorder-79.7.1/README.md
+-rw-r--r--   0        0        0      679 2023-04-23 17:52:08.589809 alacorder-79.7.1/pyproject.toml
+-rw-r--r--   0        0        0     9208 2023-04-21 18:06:44.921207 alacorder-79.7.1/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb
+-rw-r--r--   0        0        0   138382 2023-04-21 18:24:49.412475 alacorder-79.7.1/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.7.1/src/alacorder/.python-version
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.7.1/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   137934 2023-04-23 17:52:27.672176 alacorder-79.7.1/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   137934 2023-04-23 17:53:39.392846 alacorder-79.7.1/src/alacorder/alac.py
+-rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.7.1/src/alacorder/~$E 302 Portfolio.docx
+-rw-r--r--   0        0        0    10268 1970-01-01 00:00:00.000000 alacorder-79.7.1/PKG-INFO
```

### Comparing `alacorder-79.7.0/LICENSE` & `alacorder-79.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-79.7.0/README.md` & `alacorder-79.7.1/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-79.7.0/pyproject.toml` & `alacorder-79.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "79.7.0"
+version = "79.7.1"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-79.7.0/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb` & `alacorder-79.7.1/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `alacorder-79.7.0/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-79.7.1/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.7.0/src/alacorder/__init__.py` & `alacorder-79.7.1/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.7.0/src/alacorder/__main__.py` & `alacorder-79.7.1/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,25 +16,25 @@
     tqdm, 
     xlsxwriter, 
     xlsx2csv
 
 """
 
 name = "ALACORDER"
-version = "79.7.0"
+version = "79.7.1"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 if autoload_graphical_user_interface:
     import PySimpleGUI as sg
-
 import polars as pl
+import os, sys, time, glob, re
+import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
-import click, fitz, selenium, os, sys, time, glob, re, xlsxwriter, threading, platform
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.chrome.options import Options
 
 pl.Config.set_tbl_rows(20)
 pl.Config.set_fmt_str_lengths(100)
@@ -48,37 +48,36 @@
 
 prt = print
 
 def plog(*msg, cf=None):
     global prt
     if len(msg) == 1:
         msg = msg[0]
-        if isinstance(cf, pl.dataframe.frame.DataFrame):
+        if isinstance(cf, dict):
             try:
-                if cf['LOG']:
+                if cf['LOG'] == True:
                     prt(msg)
             except:
                 prt(msg)
         elif cf == None:
             prt(msg)
         elif type(cf) == bool and cf:
             prt(msg)
     elif len(msg) > 1:
         for m in msg:
-            if cf == None:
-                prt(m)
-            elif type(cf) == bool and cf:
-                prt(m)
-            elif type(cf) != bool:
+            if isinstance(cf, dict):
                 try:
-                    bl = cf["LOG"]
-                    if bl:
+                    if cf['LOG'] == True:
                         prt(m)
                 except:
-                    pass
+                    prt(m)
+            elif cf == None:
+                prt(m)
+            elif type(cf) == bool and cf:
+                prt(m)
 
 print = plog
 
 
 def dlog(*msg, cf=None):
     if type(cf) == bool:
         if cf:
@@ -102,14 +101,16 @@
 
 
 def loadgui():
     """
     Load PySimpleGUI tk graphical interface
     """
     import PySimpleGUI as sg
+    import platform
+    import threading
 
     psys = platform.system()
     plat = platform.platform()
     if "Darwin" in (plat, psys) or "macOS" in (plat, psys):  # set MacOS element sizes
         HEADER_FONT, LOGO_FONT, ASCII_FONT, BODY_FONT, WINDOW_RESIZE, WINDOW_SIZE = (
             "Default 22",
             "Courier 20",
@@ -318,15 +319,15 @@
                 """Export data tables from\ncase archive or directory.""",
                 font=HEADER_FONT,
                 pad=(5, 5),
             )
         ],
         [
             sg.Text(
-                """Alacorder processes case detail PDFs and case text archives into data\ntables suitable for research purposes. Export to an Excel spreadsheet\nto export all tables, or select a table to export to .csv, .parquet,\nor .json.""",
+                """Alacorder processes case detail PDFs and case text archives into data\ntables suitable for research purposes. Enter PDF directory or case text\narchive path and output file path (.xlsx, .xls) to begin.""",
                 pad=(5, 5),
             )
         ],
         [
             sg.Text("Input Path: "),
             sg.InputText(
                 tooltip="PDF directory or full text archive (.parquet, .json, .csv)",
@@ -343,31 +344,14 @@
             sg.InputText(
                 tooltip="Multitable export (.xlsx, .xls) or single-table export (.xlsx, .xls, .json, .csv)",
                 size=[39, 10],
                 key="TB-OUTPUTPATH",
             ),
         ],
         [
-            sg.Radio("All Tables (.xlsx, .xls)", "TABLE", key="TB-ALL", default=True),
-            sg.Radio("Cases", "TABLE", key="TB-CASES", default=False),
-            sg.Radio("Charges", "TABLE", key="TB-CHARGES", default=False),
-            sg.Radio("Fees", "TABLE", key="TB-FEES", default=False),
-        ],
-        [
-            sg.Radio("Case Action Summary", "TABLE", key="TB-CAS", default=False),
-            sg.Radio("Witnesses", "TABLE", key="TB-WITNESSES", default=False),
-            sg.Radio("Images", "TABLE", key="TB-IMAGES", default=False),
-        ],
-        [
-            sg.Radio("Attorneys", "TABLE", key="TB-ATTORNEYS", default=False),
-            sg.Radio("Settings", "TABLE", key="TB-SETTINGS", default=False),
-            sg.Radio("Disposition", "TABLE", key="TB-DISPOSITION", default=False),
-            sg.Radio("Filing", "TABLE", key="TB-FILING", default=False),
-        ],
-        [
             sg.Text("Max cases: "),
             sg.Input(key="TB-COUNT", default_text="0", size=[5, 1]),
             sg.Checkbox("Allow Overwrite", key="TB-OVERWRITE", default=True),
         ],
         [
             sg.Button(
                 "Export Table",
@@ -485,70 +469,37 @@
                 if empty_query(window["SQ-INPUTPATH"].get()):
                     sg.popup("Alacorder created query template.")
                 else:
                     sg.popup(
                         "Enter valid path with .xlsx extension in Input Path box and try again."
                     )
         elif event == "TB":
+            # print(event, values)
             if (
                 window["TB-INPUTPATH"].get() == ""
                 or window["TB-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
-            if bool(window["TB-ALL"]) == True:
-                tabl = "all"
-            elif bool(window["TB-CASES"]) == True:
-                tabl = "cases"
-            elif bool(window["TB-CHARGES"]) == True:
-                tabl = "charges"
-            elif bool(window["TB-FEES"]) == True:
-                tabl = "fees"
-            elif bool(window["TB-CAS"]) == True:
-                tabl = "case-action-summary"
-            elif bool(window["TB-IMAGES"]) == True:
-                tabl = "images"
-            elif bool(window["TB-ATTORNEYS"]) == True:
-                tabl = "attorneys"
-            elif bool(window["TB-WITNESSES"]) == True:
-                tabl = "witnesses"
-            elif bool(window["TB-DISPOSITION"]) == True:
-                tabl = "disposition"
-            elif bool(window["TB-FILING"]) == True:
-                tabl = "filing"
             else:
-                continue
-            try:
-                try:
-                    count = int(window["TB-COUNT"].get().strip())
-                except:
-                    count = 0
-                try:
-                    cf = set(
-                        window["TB-INPUTPATH"].get(),
-                        window["TB-OUTPUTPATH"].get(),
-                        count=count,
-                        table=tabl,
-                        log=True,
-                        overwrite=window["TB-OVERWRITE"].get(),
-                        no_prompt=True,
-                        debug=False,
-                        archive=False,
-                        window=window,
-                    )
-                except:
-                    print("Check configuration and try again.")
-                    window["TB"].update(disabled=False)
-                    continue
+                cf = set(
+                    window["TB-INPUTPATH"].get(),
+                    window["TB-OUTPUTPATH"].get(),
+                    count=int(window["TB-COUNT"].get()),
+                    table="all",
+                    log=True,
+                    overwrite=window["TB-OVERWRITE"].get(),
+                    no_prompt=True,
+                    debug=False,
+                    archive=False,
+                    window=window,
+                )
+                # except:
                 window["TB"].update(disabled=True)
                 threading.Thread(target=init, args=[cf], daemon=True).start()
                 continue
-            except:
-                print("Check configuration and try again.")
-                window["TB"].update(disabled=False)
-                continue
         elif event == "MA":
             if (
                 window["MA-INPUTPATH"].get() == ""
                 or window["MA-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
                 window["MA"].update(disabled=False)
@@ -1071,15 +1022,14 @@
 def charges(cf, debug=False):
     """
     Start charges table collection using configuration object `cf`.
     """
     df = read(cf)
     print("Parsing charges...", cf=cf)
     ac = explode_charges(df)
-    print("Still parsing...", cf=cf)
     ch = split_charges(ac)
     if not cf["NO_WRITE"]:
         print("Writing to export...", cf=cf)
         write(ch, cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return ch
@@ -1088,15 +1038,14 @@
 def fees(cf, debug=False):
     """
     Start fee sheet collection using configuration object `cf`.
     """
     df = read(cf)
     print("Parsing fee sheets...", cf=cf)
     af = explode_fees(df)
-    print("Still parsing...", cf=cf)
     fs = split_fees(af)
     if not cf["NO_WRITE"]:
         print("Writing to export...", cf=cf)
         write(fs, cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return fs
@@ -1539,14 +1488,15 @@
         "NO_UPDATE": no_update,
         "FETCH": fetch,
         "ALA_CUSTOMER_ID": cID,
         "ALA_USER_ID": uID,
         "ALA_PASSWORD": pwd,
         "FETCH_SKIP": qskip,
         "FETCH_MAX": qmax,
+        "LOG": log,
         "NO_WRITE": no_write,
         "NO_PROMPT": no_prompt,
         "OVERWRITE": overwrite,
         "EXISTING_OUTPUT": existing_output,
         "DEBUG": debug,
         "WINDOW": window,
     }
@@ -1576,17 +1526,20 @@
         aptxt = []
         print("Extracting text...", cf=cf)
         if cf['WINDOW']:
             cf['WINDOW'].write_event_value("PROGRESS_TOTAL", len(queue))
             for i, pp in enumerate(queue):
                 aptxt += [extract_text(pp)]
                 cf['WINDOW'].write_event_value("PROGRESS", i + 1)
-        else:
+        elif cf['LOG']:
             for pp in tqdm(queue):
                 aptxt += [extract_text(pp)]
+        else:
+            for pp in queue:
+                aptxt += [extract_text(pp)]
         archive = pl.DataFrame(
             {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
         )
         archive = archive.with_columns(
             pl.col("AllPagesText")
             .str.replace_all(r"\n", " ")
             .alias("AllPagesTextNoNewLine")
@@ -1600,17 +1553,20 @@
             aptxt = []
             print("Extracting text...", cf=cf)
             if cf['WINDOW']:
                 cf['WINDOW'].write_event_value("PROGRESS_TOTAL", len(queue))
                 for i, pp in enumerate(queue):
                     aptxt += [extract_text(pp)]
                     cf['WINDOW'].write_event_value("PROGRESS", i + 1)
-            else:
+            elif cf['LOG']:
                 for pp in tqdm(queue):
                     aptxt += [extract_text(pp)]
+            else:
+                for pp in queue:
+                    aptxt += [extract_text(pp)]
         archive = pl.DataFrame(
             {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
         )
         archive = archive.with_columns(
             pl.col("AllPagesText")
             .str.replace_all(r"\n", " ")
             .alias("AllPagesTextNoNewLine")
@@ -1621,17 +1577,20 @@
         aptxt = []
         print("Extracting text...", cf=cf)
         if cf['WINDOW']:
             cf['WINDOW'].write_event_value("PROGRESS_TOTAL", len(queue))
             for i, pp in enumerate(queue):
                 aptxt += [extract_text(pp)]
                 cf['WINDOW'].write_event_value("PROGRESS", i + 1)
-        else:
+        elif cf['LOG']:
             for pp in tqdm(queue):
                 aptxt += [extract_text(pp)]
+        else:
+            for pp in queue:
+                aptxt += [extract_text(pp)]
         archive = pl.DataFrame(
             {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
         )
         archive = archive.with_columns(
             pl.col("AllPagesText")
             .str.replace_all(r"\n", " ")
             .alias("AllPagesTextNoNewLine")
```

### Comparing `alacorder-79.7.0/src/alacorder/alac.py` & `alacorder-79.7.1/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,25 +16,25 @@
     tqdm, 
     xlsxwriter, 
     xlsx2csv
 
 """
 
 name = "ALACORDER"
-version = "79.7.0"
+version = "79.7.1"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 if autoload_graphical_user_interface:
     import PySimpleGUI as sg
-
 import polars as pl
+import os, sys, time, glob, re
+import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
-import click, fitz, selenium, os, sys, time, glob, re, xlsxwriter, threading, platform
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.chrome.options import Options
 
 pl.Config.set_tbl_rows(20)
 pl.Config.set_fmt_str_lengths(100)
@@ -48,37 +48,36 @@
 
 prt = print
 
 def plog(*msg, cf=None):
     global prt
     if len(msg) == 1:
         msg = msg[0]
-        if isinstance(cf, pl.dataframe.frame.DataFrame):
+        if isinstance(cf, dict):
             try:
-                if cf['LOG']:
+                if cf['LOG'] == True:
                     prt(msg)
             except:
                 prt(msg)
         elif cf == None:
             prt(msg)
         elif type(cf) == bool and cf:
             prt(msg)
     elif len(msg) > 1:
         for m in msg:
-            if cf == None:
-                prt(m)
-            elif type(cf) == bool and cf:
-                prt(m)
-            elif type(cf) != bool:
+            if isinstance(cf, dict):
                 try:
-                    bl = cf["LOG"]
-                    if bl:
+                    if cf['LOG'] == True:
                         prt(m)
                 except:
-                    pass
+                    prt(m)
+            elif cf == None:
+                prt(m)
+            elif type(cf) == bool and cf:
+                prt(m)
 
 print = plog
 
 
 def dlog(*msg, cf=None):
     if type(cf) == bool:
         if cf:
@@ -102,14 +101,16 @@
 
 
 def loadgui():
     """
     Load PySimpleGUI tk graphical interface
     """
     import PySimpleGUI as sg
+    import platform
+    import threading
 
     psys = platform.system()
     plat = platform.platform()
     if "Darwin" in (plat, psys) or "macOS" in (plat, psys):  # set MacOS element sizes
         HEADER_FONT, LOGO_FONT, ASCII_FONT, BODY_FONT, WINDOW_RESIZE, WINDOW_SIZE = (
             "Default 22",
             "Courier 20",
@@ -318,15 +319,15 @@
                 """Export data tables from\ncase archive or directory.""",
                 font=HEADER_FONT,
                 pad=(5, 5),
             )
         ],
         [
             sg.Text(
-                """Alacorder processes case detail PDFs and case text archives into data\ntables suitable for research purposes. Export to an Excel spreadsheet\nto export all tables, or select a table to export to .csv, .parquet,\nor .json.""",
+                """Alacorder processes case detail PDFs and case text archives into data\ntables suitable for research purposes. Enter PDF directory or case text\narchive path and output file path (.xlsx, .xls) to begin.""",
                 pad=(5, 5),
             )
         ],
         [
             sg.Text("Input Path: "),
             sg.InputText(
                 tooltip="PDF directory or full text archive (.parquet, .json, .csv)",
@@ -343,31 +344,14 @@
             sg.InputText(
                 tooltip="Multitable export (.xlsx, .xls) or single-table export (.xlsx, .xls, .json, .csv)",
                 size=[39, 10],
                 key="TB-OUTPUTPATH",
             ),
         ],
         [
-            sg.Radio("All Tables (.xlsx, .xls)", "TABLE", key="TB-ALL", default=True),
-            sg.Radio("Cases", "TABLE", key="TB-CASES", default=False),
-            sg.Radio("Charges", "TABLE", key="TB-CHARGES", default=False),
-            sg.Radio("Fees", "TABLE", key="TB-FEES", default=False),
-        ],
-        [
-            sg.Radio("Case Action Summary", "TABLE", key="TB-CAS", default=False),
-            sg.Radio("Witnesses", "TABLE", key="TB-WITNESSES", default=False),
-            sg.Radio("Images", "TABLE", key="TB-IMAGES", default=False),
-        ],
-        [
-            sg.Radio("Attorneys", "TABLE", key="TB-ATTORNEYS", default=False),
-            sg.Radio("Settings", "TABLE", key="TB-SETTINGS", default=False),
-            sg.Radio("Disposition", "TABLE", key="TB-DISPOSITION", default=False),
-            sg.Radio("Filing", "TABLE", key="TB-FILING", default=False),
-        ],
-        [
             sg.Text("Max cases: "),
             sg.Input(key="TB-COUNT", default_text="0", size=[5, 1]),
             sg.Checkbox("Allow Overwrite", key="TB-OVERWRITE", default=True),
         ],
         [
             sg.Button(
                 "Export Table",
@@ -485,70 +469,37 @@
                 if empty_query(window["SQ-INPUTPATH"].get()):
                     sg.popup("Alacorder created query template.")
                 else:
                     sg.popup(
                         "Enter valid path with .xlsx extension in Input Path box and try again."
                     )
         elif event == "TB":
+            # print(event, values)
             if (
                 window["TB-INPUTPATH"].get() == ""
                 or window["TB-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
-            if bool(window["TB-ALL"]) == True:
-                tabl = "all"
-            elif bool(window["TB-CASES"]) == True:
-                tabl = "cases"
-            elif bool(window["TB-CHARGES"]) == True:
-                tabl = "charges"
-            elif bool(window["TB-FEES"]) == True:
-                tabl = "fees"
-            elif bool(window["TB-CAS"]) == True:
-                tabl = "case-action-summary"
-            elif bool(window["TB-IMAGES"]) == True:
-                tabl = "images"
-            elif bool(window["TB-ATTORNEYS"]) == True:
-                tabl = "attorneys"
-            elif bool(window["TB-WITNESSES"]) == True:
-                tabl = "witnesses"
-            elif bool(window["TB-DISPOSITION"]) == True:
-                tabl = "disposition"
-            elif bool(window["TB-FILING"]) == True:
-                tabl = "filing"
             else:
-                continue
-            try:
-                try:
-                    count = int(window["TB-COUNT"].get().strip())
-                except:
-                    count = 0
-                try:
-                    cf = set(
-                        window["TB-INPUTPATH"].get(),
-                        window["TB-OUTPUTPATH"].get(),
-                        count=count,
-                        table=tabl,
-                        log=True,
-                        overwrite=window["TB-OVERWRITE"].get(),
-                        no_prompt=True,
-                        debug=False,
-                        archive=False,
-                        window=window,
-                    )
-                except:
-                    print("Check configuration and try again.")
-                    window["TB"].update(disabled=False)
-                    continue
+                cf = set(
+                    window["TB-INPUTPATH"].get(),
+                    window["TB-OUTPUTPATH"].get(),
+                    count=int(window["TB-COUNT"].get()),
+                    table="all",
+                    log=True,
+                    overwrite=window["TB-OVERWRITE"].get(),
+                    no_prompt=True,
+                    debug=False,
+                    archive=False,
+                    window=window,
+                )
+                # except:
                 window["TB"].update(disabled=True)
                 threading.Thread(target=init, args=[cf], daemon=True).start()
                 continue
-            except:
-                print("Check configuration and try again.")
-                window["TB"].update(disabled=False)
-                continue
         elif event == "MA":
             if (
                 window["MA-INPUTPATH"].get() == ""
                 or window["MA-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
                 window["MA"].update(disabled=False)
@@ -1071,15 +1022,14 @@
 def charges(cf, debug=False):
     """
     Start charges table collection using configuration object `cf`.
     """
     df = read(cf)
     print("Parsing charges...", cf=cf)
     ac = explode_charges(df)
-    print("Still parsing...", cf=cf)
     ch = split_charges(ac)
     if not cf["NO_WRITE"]:
         print("Writing to export...", cf=cf)
         write(ch, cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return ch
@@ -1088,15 +1038,14 @@
 def fees(cf, debug=False):
     """
     Start fee sheet collection using configuration object `cf`.
     """
     df = read(cf)
     print("Parsing fee sheets...", cf=cf)
     af = explode_fees(df)
-    print("Still parsing...", cf=cf)
     fs = split_fees(af)
     if not cf["NO_WRITE"]:
         print("Writing to export...", cf=cf)
         write(fs, cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return fs
@@ -1539,14 +1488,15 @@
         "NO_UPDATE": no_update,
         "FETCH": fetch,
         "ALA_CUSTOMER_ID": cID,
         "ALA_USER_ID": uID,
         "ALA_PASSWORD": pwd,
         "FETCH_SKIP": qskip,
         "FETCH_MAX": qmax,
+        "LOG": log,
         "NO_WRITE": no_write,
         "NO_PROMPT": no_prompt,
         "OVERWRITE": overwrite,
         "EXISTING_OUTPUT": existing_output,
         "DEBUG": debug,
         "WINDOW": window,
     }
@@ -1576,17 +1526,20 @@
         aptxt = []
         print("Extracting text...", cf=cf)
         if cf['WINDOW']:
             cf['WINDOW'].write_event_value("PROGRESS_TOTAL", len(queue))
             for i, pp in enumerate(queue):
                 aptxt += [extract_text(pp)]
                 cf['WINDOW'].write_event_value("PROGRESS", i + 1)
-        else:
+        elif cf['LOG']:
             for pp in tqdm(queue):
                 aptxt += [extract_text(pp)]
+        else:
+            for pp in queue:
+                aptxt += [extract_text(pp)]
         archive = pl.DataFrame(
             {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
         )
         archive = archive.with_columns(
             pl.col("AllPagesText")
             .str.replace_all(r"\n", " ")
             .alias("AllPagesTextNoNewLine")
@@ -1600,17 +1553,20 @@
             aptxt = []
             print("Extracting text...", cf=cf)
             if cf['WINDOW']:
                 cf['WINDOW'].write_event_value("PROGRESS_TOTAL", len(queue))
                 for i, pp in enumerate(queue):
                     aptxt += [extract_text(pp)]
                     cf['WINDOW'].write_event_value("PROGRESS", i + 1)
-            else:
+            elif cf['LOG']:
                 for pp in tqdm(queue):
                     aptxt += [extract_text(pp)]
+            else:
+                for pp in queue:
+                    aptxt += [extract_text(pp)]
         archive = pl.DataFrame(
             {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
         )
         archive = archive.with_columns(
             pl.col("AllPagesText")
             .str.replace_all(r"\n", " ")
             .alias("AllPagesTextNoNewLine")
@@ -1621,17 +1577,20 @@
         aptxt = []
         print("Extracting text...", cf=cf)
         if cf['WINDOW']:
             cf['WINDOW'].write_event_value("PROGRESS_TOTAL", len(queue))
             for i, pp in enumerate(queue):
                 aptxt += [extract_text(pp)]
                 cf['WINDOW'].write_event_value("PROGRESS", i + 1)
-        else:
+        elif cf['LOG']:
             for pp in tqdm(queue):
                 aptxt += [extract_text(pp)]
+        else:
+            for pp in queue:
+                aptxt += [extract_text(pp)]
         archive = pl.DataFrame(
             {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
         )
         archive = archive.with_columns(
             pl.col("AllPagesText")
             .str.replace_all(r"\n", " ")
             .alias("AllPagesTextNoNewLine")
```

### Comparing `alacorder-79.7.0/PKG-INFO` & `alacorder-79.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 79.7.0
+Version: 79.7.1
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

