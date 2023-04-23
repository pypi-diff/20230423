# Comparing `tmp/Anilist-0.9.0.tar.gz` & `tmp/Anilist-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Anilist-0.9.0.tar", last modified: Sun Apr 23 02:43:09 2023, max compression
+gzip compressed data, was "Anilist-0.9.1.tar", last modified: Sun Apr 23 03:00:36 2023, max compression
```

## Comparing `Anilist-0.9.0.tar` & `Anilist-0.9.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.225318 Anilist-0.9.0/
-drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.061417 Anilist-0.9.0/Anilist/
--rw-rw-rw-   0        0        0      188 2023-04-22 21:40:55.000000 Anilist-0.9.0/Anilist/__init__.py
--rw-rw-rw-   0        0        0     1072 2023-04-22 06:25:28.000000 Anilist-0.9.0/Anilist/anilist_types.py
-drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.125378 Anilist-0.9.0/Anilist/auth/
--rw-rw-rw-   0        0        0      749 2023-04-23 02:39:40.000000 Anilist-0.9.0/Anilist/auth/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-04-23 01:27:00.000000 Anilist-0.9.0/Anilist/auth/auth.py
--rw-rw-rw-   0        0        0      993 2023-04-22 22:01:35.000000 Anilist-0.9.0/Anilist/auth/code.py
--rw-rw-rw-   0        0        0      503 2023-04-21 03:30:49.000000 Anilist-0.9.0/Anilist/auth/token.py
-drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.140368 Anilist-0.9.0/Anilist/client/
--rw-rw-rw-   0        0        0       98 2023-04-21 03:31:08.000000 Anilist-0.9.0/Anilist/client/__init__.py
--rw-rw-rw-   0        0        0     2573 2023-04-22 22:13:50.000000 Anilist-0.9.0/Anilist/client/client.py
--rw-rw-rw-   0        0        0      477 2023-04-21 20:55:21.000000 Anilist-0.9.0/Anilist/client/mutation.py
--rw-rw-rw-   0        0        0     1072 2023-04-23 02:38:44.000000 Anilist-0.9.0/Anilist/client/query.py
-drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.143366 Anilist-0.9.0/Anilist/errors/
--rw-rw-rw-   0        0        0       55 2023-04-21 04:04:44.000000 Anilist-0.9.0/Anilist/errors/__init__.py
--rw-rw-rw-   0        0        0      998 2023-04-21 04:21:59.000000 Anilist-0.9.0/Anilist/errors/request.py
-drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.167360 Anilist-0.9.0/Anilist/mutation/
--rw-rw-rw-   0        0        0       41 2023-04-21 03:30:29.000000 Anilist-0.9.0/Anilist/mutation/__init__.py
--rw-rw-rw-   0        0        0      962 2023-04-22 06:24:47.000000 Anilist-0.9.0/Anilist/mutation/media_list.py
--rw-rw-rw-   0        0        0      393 2023-04-22 06:22:20.000000 Anilist-0.9.0/Anilist/mutation/mutable.py
-drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.175346 Anilist-0.9.0/Anilist/query/
--rw-rw-rw-   0        0        0      132 2023-04-22 21:50:16.000000 Anilist-0.9.0/Anilist/query/__init__.py
--rw-rw-rw-   0        0        0      721 2023-04-23 02:37:43.000000 Anilist-0.9.0/Anilist/query/media_entry.py
--rw-rw-rw-   0        0        0      769 2023-04-23 02:37:57.000000 Anilist-0.9.0/Anilist/query/media_list.py
--rw-rw-rw-   0        0        0     6825 2023-04-23 02:36:40.000000 Anilist-0.9.0/Anilist/query/query.py
-drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.179345 Anilist-0.9.0/Anilist/scheme/
--rw-rw-rw-   0        0        0      139 2023-04-22 22:02:36.000000 Anilist-0.9.0/Anilist/scheme/__init__.py
--rw-rw-rw-   0        0        0      662 2023-04-22 01:52:21.000000 Anilist-0.9.0/Anilist/scheme/media_scheme.py
--rw-rw-rw-   0        0        0     4017 2023-04-23 02:11:42.000000 Anilist-0.9.0/Anilist/scheme/scheme.py
-drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.190338 Anilist-0.9.0/Anilist/utils/
--rw-rw-rw-   0        0        0       92 2023-04-21 03:29:38.000000 Anilist-0.9.0/Anilist/utils/__init__.py
--rw-rw-rw-   0        0        0      190 2023-04-21 03:11:45.000000 Anilist-0.9.0/Anilist/utils/consts.py
--rw-rw-rw-   0        0        0     1571 2023-04-20 22:06:18.000000 Anilist-0.9.0/Anilist/utils/logging.py
--rw-rw-rw-   0        0        0     2933 2023-04-23 02:02:48.000000 Anilist-0.9.0/Anilist/utils/object.py
-drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.193336 Anilist-0.9.0/Anilist/vars/
--rw-rw-rw-   0        0        0       22 2023-04-21 06:57:34.000000 Anilist-0.9.0/Anilist/vars/__init__.py
--rw-rw-rw-   0        0        0     2070 2023-04-23 01:31:18.000000 Anilist-0.9.0/Anilist/vars/vars.py
-drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.094398 Anilist-0.9.0/Anilist.egg-info/
--rw-rw-rw-   0        0        0      563 2023-04-23 02:43:08.000000 Anilist-0.9.0/Anilist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      916 2023-04-23 02:43:08.000000 Anilist-0.9.0/Anilist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 02:43:08.000000 Anilist-0.9.0/Anilist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 02:43:08.000000 Anilist-0.9.0/Anilist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1080 2023-04-20 22:07:52.000000 Anilist-0.9.0/LICENSE
--rw-rw-rw-   0        0        0      563 2023-04-23 02:43:09.224318 Anilist-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-20 21:05:02.000000 Anilist-0.9.0/README.md
--rw-rw-rw-   0        0        0      601 2023-04-23 02:41:38.000000 Anilist-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 02:43:09.226316 Anilist-0.9.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.221320 Anilist-0.9.0/tests/
--rw-rw-rw-   0        0        0     1334 2023-04-22 21:40:22.000000 Anilist-0.9.0/tests/test_externals.py
--rw-rw-rw-   0        0        0      223 2023-04-22 21:39:23.000000 Anilist-0.9.0/tests/test_internals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:00:36.914919 Anilist-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:00:36.906919 Anilist-0.9.1/Anilist/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/anilist_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:00:36.910919 Anilist-0.9.1/Anilist/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/auth/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/auth/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:00:36.910919 Anilist-0.9.1/Anilist/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/client/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/client/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:00:36.910919 Anilist-0.9.1/Anilist/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/errors/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:00:36.910919 Anilist-0.9.1/Anilist/mutation/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/mutation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/mutation/media_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/mutation/mutable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:00:36.910919 Anilist-0.9.1/Anilist/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/query/media_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/query/media_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/query/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:00:36.914919 Anilist-0.9.1/Anilist/scheme/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/scheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/scheme/media_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/scheme/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:00:36.914919 Anilist-0.9.1/Anilist/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/utils/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/utils/object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:00:36.914919 Anilist-0.9.1/Anilist/vars/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/vars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-23 03:00:22.000000 Anilist-0.9.1/Anilist/vars/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:00:36.910919 Anilist-0.9.1/Anilist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-23 03:00:36.000000 Anilist-0.9.1/Anilist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-23 03:00:36.000000 Anilist-0.9.1/Anilist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 03:00:36.000000 Anilist-0.9.1/Anilist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 03:00:36.000000 Anilist-0.9.1/Anilist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-23 03:00:22.000000 Anilist-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-23 03:00:36.914919 Anilist-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-23 03:00:22.000000 Anilist-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-23 03:00:22.000000 Anilist-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 03:00:36.914919 Anilist-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:00:36.914919 Anilist-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-23 03:00:22.000000 Anilist-0.9.1/tests/test_externals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-23 03:00:22.000000 Anilist-0.9.1/tests/test_internals.py
```

### Comparing `Anilist-0.9.0/Anilist/auth/code.py` & `Anilist-0.9.1/Anilist/auth/code.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,60 @@
-00000000: 696d 706f 7274 2073 6f63 6b65 740d 0a69  import socket..i
-00000010: 6d70 6f72 7420 7265 0d0a 696d 706f 7274  mport re..import
-00000020: 2077 6562 6272 6f77 7365 720d 0a0d 0a70   webbrowser....p
-00000030: 6174 203d 2072 652e 636f 6d70 696c 6528  at = re.compile(
-00000040: 7227 5c3f 636f 6465 3d28 2e2a 3f29 285c  r'\?code=(.*?)(\
-00000050: 267c 5c72 7c20 7c5c 6e29 2729 0d0a 0d0a  &|\r| |\n)')....
-00000060: 6465 6620 6765 745f 636f 6465 2863 6c69  def get_code(cli
-00000070: 656e 745f 6964 293a 0d0a 2020 2020 7765  ent_id):..    we
-00000080: 6262 726f 7773 6572 2e6f 7065 6e28 6622  bbrowser.open(f"
-00000090: 6874 7470 733a 2f2f 616e 696c 6973 742e  https://anilist.
-000000a0: 636f 2f61 7069 2f76 322f 6f61 7574 682f  co/api/v2/oauth/
-000000b0: 6175 7468 6f72 697a 653f 636c 6965 6e74  authorize?client
-000000c0: 5f69 643d 7b63 6c69 656e 745f 6964 7d26  _id={client_id}&
-000000d0: 7265 6469 7265 6374 5f75 7269 3d68 7474  redirect_uri=htt
-000000e0: 703a 2f2f 3132 372e 302e 302e 313a 3830  p://127.0.0.1:80
-000000f0: 3030 2f26 7265 7370 6f6e 7365 5f74 7970  00/&response_typ
-00000100: 653d 636f 6465 222c 2061 7574 6f72 6169  e=code", autorai
-00000110: 7365 3d54 7275 6529 0d0a 2020 2020 0d0a  se=True)..    ..
-00000120: 2020 2020 7769 7468 2073 6f63 6b65 742e      with socket.
-00000130: 736f 636b 6574 2873 6f63 6b65 742e 4146  socket(socket.AF
-00000140: 5f49 4e45 542c 2073 6f63 6b65 742e 534f  _INET, socket.SO
-00000150: 434b 5f53 5452 4541 4d29 2061 7320 733a  CK_STREAM) as s:
-00000160: 0d0a 2020 2020 2020 2020 732e 6269 6e64  ..        s.bind
-00000170: 2828 2231 3237 2e30 2e30 2e31 222c 2038  (("127.0.0.1", 8
-00000180: 3030 3029 290d 0a20 2020 2020 2020 2073  000))..        s
-00000190: 2e6c 6973 7465 6e28 290d 0a20 2020 2020  .listen()..     
-000001a0: 2020 2063 6f6e 6e2c 205f 203d 2073 2e61     conn, _ = s.a
-000001b0: 6363 6570 7428 290d 0a20 2020 2020 2020  ccept()..       
-000001c0: 2063 6f64 6520 3d20 4e6f 6e65 0d0a 2020   code = None..  
-000001d0: 2020 2020 2020 6461 7461 203d 2063 6f6e        data = con
-000001e0: 6e2e 7265 6376 2831 3032 3429 0d0a 2020  n.recv(1024)..  
-000001f0: 2020 2020 2020 6966 206e 6f74 2064 6174        if not dat
-00000200: 613a 0d0a 2020 2020 2020 2020 2020 2020  a:..            
-00000210: 7265 7475 726e 2063 6f64 650d 0a20 2020  return code..   
-00000220: 2020 2020 200d 0a20 2020 2020 2020 2063       ..        c
-00000230: 6f6e 6e2e 7365 6e64 2822 4854 5450 2f31  onn.send("HTTP/1
-00000240: 2e31 2032 3030 204f 4b5c 6e22 2e65 6e63  .1 200 OK\n".enc
-00000250: 6f64 6528 2929 0d0a 2020 2020 2020 2020  ode())..        
-00000260: 636f 6e6e 2e73 656e 6428 2243 6f6e 7465  conn.send("Conte
-00000270: 6e74 2d54 7970 653a 2074 6578 742f 6874  nt-Type: text/ht
-00000280: 6d6c 5c6e 5c6e 222e 656e 636f 6465 2829  ml\n\n".encode()
-00000290: 290d 0a20 2020 2020 2020 2063 6f6e 6e2e  )..        conn.
-000002a0: 7365 6e64 2822 5c6e 222e 656e 636f 6465  send("\n".encode
-000002b0: 2829 290d 0a20 2020 2020 2020 2063 6f6e  ())..        con
-000002c0: 6e2e 7365 6e64 2822 2222 0d0a 2020 2020  n.send("""..    
-000002d0: 2020 2020 2020 2020 3c68 746d 6c3e 0d0a          <html>..
+00000000: 696d 706f 7274 2073 6f63 6b65 740a 696d  import socket.im
+00000010: 706f 7274 2072 650a 696d 706f 7274 2077  port re.import w
+00000020: 6562 6272 6f77 7365 720a 0a70 6174 203d  ebbrowser..pat =
+00000030: 2072 652e 636f 6d70 696c 6528 7227 5c3f   re.compile(r'\?
+00000040: 636f 6465 3d28 2e2a 3f29 285c 267c 5c72  code=(.*?)(\&|\r
+00000050: 7c20 7c5c 6e29 2729 0a0a 6465 6620 6765  | |\n)')..def ge
+00000060: 745f 636f 6465 2863 6c69 656e 745f 6964  t_code(client_id
+00000070: 293a 0a20 2020 2077 6562 6272 6f77 7365  ):.    webbrowse
+00000080: 722e 6f70 656e 2866 2268 7474 7073 3a2f  r.open(f"https:/
+00000090: 2f61 6e69 6c69 7374 2e63 6f2f 6170 692f  /anilist.co/api/
+000000a0: 7632 2f6f 6175 7468 2f61 7574 686f 7269  v2/oauth/authori
+000000b0: 7a65 3f63 6c69 656e 745f 6964 3d7b 636c  ze?client_id={cl
+000000c0: 6965 6e74 5f69 647d 2672 6564 6972 6563  ient_id}&redirec
+000000d0: 745f 7572 693d 6874 7470 3a2f 2f31 3237  t_uri=http://127
+000000e0: 2e30 2e30 2e31 3a38 3030 302f 2672 6573  .0.0.1:8000/&res
+000000f0: 706f 6e73 655f 7479 7065 3d63 6f64 6522  ponse_type=code"
+00000100: 2c20 6175 746f 7261 6973 653d 5472 7565  , autoraise=True
+00000110: 290a 2020 2020 0a20 2020 2077 6974 6820  ).    .    with 
+00000120: 736f 636b 6574 2e73 6f63 6b65 7428 736f  socket.socket(so
+00000130: 636b 6574 2e41 465f 494e 4554 2c20 736f  cket.AF_INET, so
+00000140: 636b 6574 2e53 4f43 4b5f 5354 5245 414d  cket.SOCK_STREAM
+00000150: 2920 6173 2073 3a0a 2020 2020 2020 2020  ) as s:.        
+00000160: 732e 6269 6e64 2828 2231 3237 2e30 2e30  s.bind(("127.0.0
+00000170: 2e31 222c 2038 3030 3029 290a 2020 2020  .1", 8000)).    
+00000180: 2020 2020 732e 6c69 7374 656e 2829 0a20      s.listen(). 
+00000190: 2020 2020 2020 2063 6f6e 6e2c 205f 203d         conn, _ =
+000001a0: 2073 2e61 6363 6570 7428 290a 2020 2020   s.accept().    
+000001b0: 2020 2020 636f 6465 203d 204e 6f6e 650a      code = None.
+000001c0: 2020 2020 2020 2020 6461 7461 203d 2063          data = c
+000001d0: 6f6e 6e2e 7265 6376 2831 3032 3429 0a20  onn.recv(1024). 
+000001e0: 2020 2020 2020 2069 6620 6e6f 7420 6461         if not da
+000001f0: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
+00000200: 7265 7475 726e 2063 6f64 650a 2020 2020  return code.    
+00000210: 2020 2020 0a20 2020 2020 2020 2063 6f6e      .        con
+00000220: 6e2e 7365 6e64 2822 4854 5450 2f31 2e31  n.send("HTTP/1.1
+00000230: 2032 3030 204f 4b5c 6e22 2e65 6e63 6f64   200 OK\n".encod
+00000240: 6528 2929 0a20 2020 2020 2020 2063 6f6e  e()).        con
+00000250: 6e2e 7365 6e64 2822 436f 6e74 656e 742d  n.send("Content-
+00000260: 5479 7065 3a20 7465 7874 2f68 746d 6c5c  Type: text/html\
+00000270: 6e5c 6e22 2e65 6e63 6f64 6528 2929 0a20  n\n".encode()). 
+00000280: 2020 2020 2020 2063 6f6e 6e2e 7365 6e64         conn.send
+00000290: 2822 5c6e 222e 656e 636f 6465 2829 290a  ("\n".encode()).
+000002a0: 2020 2020 2020 2020 636f 6e6e 2e73 656e          conn.sen
+000002b0: 6428 2222 220a 2020 2020 2020 2020 2020  d(""".          
+000002c0: 2020 3c68 746d 6c3e 0a20 2020 2020 2020    <html>.       
+000002d0: 2020 2020 2020 2020 203c 626f 6479 3e0a           <body>.
 000002e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002f0: 3c62 6f64 793e 0d0a 2020 2020 2020 2020  <body>..        
-00000300: 2020 2020 2020 2020 2020 2020 3c68 313e              <h1>
-00000310: 4175 7468 2063 6f6d 706c 6574 6564 3c2f  Auth completed</
-00000320: 6831 3e0d 0a20 2020 2020 2020 2020 2020  h1>..           
-00000330: 2020 2020 203c 2f62 6f64 793e 0d0a 2020       </body>..  
-00000340: 2020 2020 2020 2020 2020 3c2f 6874 6d6c            </html
-00000350: 3e0d 0a20 2020 2020 2020 2022 2222 2e65  >..        """.e
-00000360: 6e63 6f64 6528 2929 0d0a 2020 2020 2020  ncode())..      
-00000370: 2020 636f 6e6e 2e63 6c6f 7365 2829 0d0a    conn.close()..
-00000380: 0d0a 2020 2020 2020 2020 636f 6465 203d  ..        code =
-00000390: 2070 6174 2e66 696e 6461 6c6c 2864 6174   pat.findall(dat
-000003a0: 612e 6465 636f 6465 2827 7574 662d 3827  a.decode('utf-8'
-000003b0: 2929 5b30 5d5b 305d 0d0a 2020 2020 2020  ))[0][0]..      
-000003c0: 2020 0d0a 2020 2020 7265 7475 726e 2063    ..    return c
-000003d0: 6f64 650d 0a0d 0a20 2020 2020 2020 200d  ode....        .
-000003e0: 0a                                       .
+000002f0: 2020 2020 3c68 313e 4175 7468 2063 6f6d      <h1>Auth com
+00000300: 706c 6574 6564 3c2f 6831 3e0a 2020 2020  pleted</h1>.    
+00000310: 2020 2020 2020 2020 2020 2020 3c2f 626f              </bo
+00000320: 6479 3e0a 2020 2020 2020 2020 2020 2020  dy>.            
+00000330: 3c2f 6874 6d6c 3e0a 2020 2020 2020 2020  </html>.        
+00000340: 2222 222e 656e 636f 6465 2829 290a 2020  """.encode()).  
+00000350: 2020 2020 2020 636f 6e6e 2e63 6c6f 7365        conn.close
+00000360: 2829 0a0a 2020 2020 2020 2020 636f 6465  ()..        code
+00000370: 203d 2070 6174 2e66 696e 6461 6c6c 2864   = pat.findall(d
+00000380: 6174 612e 6465 636f 6465 2827 7574 662d  ata.decode('utf-
+00000390: 3827 2929 5b30 5d5b 305d 0a20 2020 2020  8'))[0][0].     
+000003a0: 2020 200a 2020 2020 7265 7475 726e 2063     .    return c
+000003b0: 6f64 650a 0a20 2020 2020 2020 200a       ode..        .
```

### Comparing `Anilist-0.9.0/Anilist/client/client.py` & `Anilist-0.9.1/Anilist/client/client.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import requests, logging
-from Anilist.scheme.scheme import Scheme
-
-from Anilist.utils import AnilistObject, AnilistLogger, consts
-from Anilist.errors import RequestError
-from Anilist.vars.vars import Vars
-class Client:
-
-    URI = consts.API_URI
-    DEFAULT_HEADERS = consts.DEFAULT_HEADERS
-
-    def __init__(self, auth, level, max_pages=100):
-        self._auth = auth
-        self._headers = None
-        self._max = max_pages
-        _ = AnilistLogger(level)
-
-    def _page_request(self, query, vars: Vars, k, f=lambda x: x):        
-        pg = vars._json["page"]
-
-        temp = []
-
-        while pg <= self._max:
-            resp = self._request(query, vars)
-            data = ([f(v) for v in resp.Page[k]])
-
-            temp.extend(data)
-
-            if data == []:
-                break
-
-            pg += 1
-            vars.update("page", pg)
-
-        return temp
-
-    def _request(self, query: str, vars: Vars):
-
-        log = AnilistLogger()
-        log.info(f"Sending request to URI {self.URI} with headers {self.headers}")
-        log.debug(f"The query is {query}\n The variables are {vars}")
-        
-        req = requests.post(self.URI, json={
-            "query": query,
-            "variables": vars._json,
-        }, headers = self.headers)
-
-        resp = req.json()
-
-        log.info(f"Received response to request with status code {req.status_code}")
-
-        if "errors" in resp and resp["errors"] != []:
-            raise RequestError.from_json(resp["errors"][0])
-        
-        obj = AnilistObject(resp["data"])
-        return obj
-        
-    def _create_query(self, vars, *schs: Scheme, head_sch: Scheme=None):
-        schs = list(schs) if head_sch is None else head_sch.sub_schemes(*schs)
-        if vars._names == "":
-            return """
-            {} {{
-                {}
-            }}
-            """.format(self._query_type(), Scheme._construct(*schs))
-        return """
-            {} ({}) {{
-                {}
-            }}
-        """.format(self._query_type(), vars._names, Scheme._construct(*schs))
-
-        return query
-    
-    def _query_type(self):
-        return "null"
-    
-    @property
-    def headers(self):
-        if self._headers == None:
-            self._headers = self._gen_headers()
-        
-        return self._headers
-        
-    def _gen_headers(self):
-        temp = self.DEFAULT_HEADERS
-
-        if self._auth != None:
-            temp["Authorization"] = f"Bearer {self._auth.token}"
-
-        return temp
-
-
-
+import requests, logging
+from Anilist.scheme.scheme import Scheme
+
+from Anilist.utils import AnilistObject, AnilistLogger, consts
+from Anilist.errors import RequestError
+from Anilist.vars.vars import Vars
+class Client:
+
+    URI = consts.API_URI
+    DEFAULT_HEADERS = consts.DEFAULT_HEADERS
+
+    def __init__(self, auth, level, max_pages=100):
+        self._auth = auth
+        self._headers = None
+        self._max = max_pages
+        _ = AnilistLogger(level)
+
+    def _page_request(self, query, vars: Vars, k, f=lambda x: x):        
+        pg = vars._json["page"]
+
+        temp = []
+
+        while pg <= self._max:
+            resp = self._request(query, vars)
+            data = ([f(v) for v in resp.Page[k]])
+
+            temp.extend(data)
+
+            if data == []:
+                break
+
+            pg += 1
+            vars.update("page", pg)
+
+        return temp
+
+    def _request(self, query: str, vars: Vars):
+
+        log = AnilistLogger()
+        log.info(f"Sending request to URI {self.URI} with headers {self.headers}")
+        log.debug(f"The query is {query}\n The variables are {vars}")
+        
+        req = requests.post(self.URI, json={
+            "query": query,
+            "variables": vars._json,
+        }, headers = self.headers)
+
+        resp = req.json()
+
+        log.info(f"Received response to request with status code {req.status_code}")
+
+        if "errors" in resp and resp["errors"] != []:
+            raise RequestError.from_json(resp["errors"][0])
+        
+        obj = AnilistObject(resp["data"])
+        return obj
+        
+    def _create_query(self, vars, *schs: Scheme, head_sch: Scheme=None):
+        schs = list(schs) if head_sch is None else head_sch.sub_schemes(*schs)
+        if vars._names == "":
+            return """
+            {} {{
+                {}
+            }}
+            """.format(self._query_type(), Scheme._construct(*schs))
+        return """
+            {} ({}) {{
+                {}
+            }}
+        """.format(self._query_type(), vars._names, Scheme._construct(*schs))
+
+        return query
+    
+    def _query_type(self):
+        return "null"
+    
+    @property
+    def headers(self):
+        if self._headers == None:
+            self._headers = self._gen_headers()
+        
+        return self._headers
+        
+    def _gen_headers(self):
+        temp = self.DEFAULT_HEADERS
+
+        if self._auth != None:
+            temp["Authorization"] = f"Bearer {self._auth.token}"
+
+        return temp
+
+
+
```

### Comparing `Anilist-0.9.0/Anilist/client/query.py` & `Anilist-0.9.1/Anilist/client/query.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-    
-from Anilist.client import Client
-from Anilist.query import MediaEntryQuery
-from Anilist.query import MediaListQuery
-
-import logging
-
-from Anilist.vars.vars import Vars
-
-class QueryClient(Client):
-    """
-    A hub that creates various interfaces that interact with the Anilist API
-
-    :param level: The logging level for this client
-    :type level: :class:`~int`   
-    """
-
-    def __init__(self, level=logging.INFO, **kwargs):
-        """Constructor method
-        """
-        Client.__init__(self, None, level, **kwargs)
-
-    def _query_type(self):
-        return "query"
-
-    def media_list(self, *, languages=["english"], sizes=["extraLarge"]):
-        """Creates a :class:`~.query.MediaListQuery` object
-        """
-        return MediaListQuery(client=self, languages=languages, sizes=sizes)
-    
-    def media_entry(self, *, languages=["english"], sizes=["extraLarge"]):
-        """Creates a :class:`~.query.MediaEntryQuery` object
-        """
-        return MediaEntryQuery(client=self, languages=languages, sizes=sizes)
+    
+from Anilist.client import Client
+from Anilist.query import MediaEntryQuery
+from Anilist.query import MediaListQuery
+
+import logging
+
+from Anilist.vars.vars import Vars
+
+class QueryClient(Client):
+    """
+    A hub that creates various interfaces that interact with the Anilist API
+
+    :param level: The logging level for this client
+    :type level: :class:`~int`   
+    """
+
+    def __init__(self, level=logging.INFO, **kwargs):
+        """Constructor method
+        """
+        Client.__init__(self, None, level, **kwargs)
+
+    def _query_type(self):
+        return "query"
+
+    def media_list(self, *, languages=["english"], sizes=["extraLarge"]):
+        """Creates a :class:`~.query.MediaListQuery` object
+        """
+        return MediaListQuery(client=self, languages=languages, sizes=sizes)
+    
+    def media_entry(self, *, languages=["english"], sizes=["extraLarge"]):
+        """Creates a :class:`~.query.MediaEntryQuery` object
+        """
+        return MediaEntryQuery(client=self, languages=languages, sizes=sizes)
```

### Comparing `Anilist-0.9.0/Anilist/errors/request.py` & `Anilist-0.9.1/Anilist/errors/request.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-class RequestError(Exception):
-    
-    def __init__(self, message: str, code: int, locations: list[tuple[int, int]]):
-        super().__init__()
-
-        self._message = message
-        self._code = code
-        self._line = locations[0][0]
-        self._column = locations[0][1]
-
-    def __str__(self):
-        return f"API Request returned error with code {self._code}. Error at line {self._line}, column {self._column}: '{self._message}' Use DEBUG logging level to view the query."
-
-    @classmethod
-    def from_json(cls, json_obj):
-        vars = [json_obj["message"], json_obj["status"], [(i["line"], i["column"]) for i in json_obj["locations"]]]
-        if "validation" not in json_obj:
-            return cls(*vars)
-        return MutationRequestError(json_obj["validation"], *vars)
-
-class MutationRequestError(RequestError):
-    
-    def __init__(self, validation, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._validation = validation
+class RequestError(Exception):
+    
+    def __init__(self, message: str, code: int, locations: list[tuple[int, int]]):
+        super().__init__()
+
+        self._message = message
+        self._code = code
+        self._line = locations[0][0]
+        self._column = locations[0][1]
+
+    def __str__(self):
+        return f"API Request returned error with code {self._code}. Error at line {self._line}, column {self._column}: '{self._message}' Use DEBUG logging level to view the query."
+
+    @classmethod
+    def from_json(cls, json_obj):
+        vars = [json_obj["message"], json_obj["status"], [(i["line"], i["column"]) for i in json_obj["locations"]]]
+        if "validation" not in json_obj:
+            return cls(*vars)
+        return MutationRequestError(json_obj["validation"], *vars)
+
+class MutationRequestError(RequestError):
+    
+    def __init__(self, validation, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._validation = validation
```

### Comparing `Anilist-0.9.0/Anilist/mutation/media_list.py` & `Anilist-0.9.1/Anilist/mutation/media_list.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from Anilist.client.client import Client
-from Anilist.mutation.mutable import Mutable
-from Anilist.scheme import Scheme
-from Anilist.vars import Vars
-
-
-class MediaEntryMutable(Mutable):
-    
-    def __init__(self, id, client: Client):
-        self._id = id
-        self._client = client
-
-    def set_score(self, score: float):
-
-        self._mutate(Scheme().id, Scheme().score, head_sch=Scheme().SaveMediaListEntry, id=self._id, score=score)
-
-        return "OK"
-    
-    def delete(self):
-        
-        self._mutate(Scheme().deleted, head_sch=Scheme().DeleteMediaListEntry, id=self._id)
-
-        return "OK"
-
-    @classmethod
-    def _from_media_id(cls, client: Client, media_id):
-        vars = Vars(mediaId=media_id)
-        q = client._create_query(vars, Scheme().id, head_sch=Scheme().SaveMediaListEntry(mediaId='$mediaId'))
-
-        resp = client._request(q, vars)
-
-        return cls(resp.SaveMediaListEntry.id, client)
+from Anilist.client.client import Client
+from Anilist.mutation.mutable import Mutable
+from Anilist.scheme import Scheme
+from Anilist.vars import Vars
+
+
+class MediaEntryMutable(Mutable):
+    
+    def __init__(self, id, client: Client):
+        self._id = id
+        self._client = client
+
+    def set_score(self, score: float):
+
+        self._mutate(Scheme().id, Scheme().score, head_sch=Scheme().SaveMediaListEntry, id=self._id, score=score)
+
+        return "OK"
+    
+    def delete(self):
+        
+        self._mutate(Scheme().deleted, head_sch=Scheme().DeleteMediaListEntry, id=self._id)
+
+        return "OK"
+
+    @classmethod
+    def _from_media_id(cls, client: Client, media_id):
+        vars = Vars(mediaId=media_id)
+        q = client._create_query(vars, Scheme().id, head_sch=Scheme().SaveMediaListEntry(mediaId='$mediaId'))
+
+        resp = client._request(q, vars)
+
+        return cls(resp.SaveMediaListEntry.id, client)
```

### Comparing `Anilist-0.9.0/Anilist/query/media_list.py` & `Anilist-0.9.1/Anilist/query/media_list.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from Anilist.scheme import *
-from Anilist.vars import Vars
-from Anilist.client.client import Client
-from Anilist.query.query import Query
-class MediaListQuery(Query):
-    """
-    An interface for making Queries for media lists to the Anilist API
-
-        
-    .. warning::
-
-        This usually should not be created manually, instead use :meth:`QueryClient.media_list() <.client.QueryClient.media_list>`
-
-    """
-    
-    def __init__(self, client: Client, languages=["english"], sizes=["extraLarge"]):
-        super().__init__(client, 'mediaList', 'MediaList', [
-            mediaScheme().id, 
-            *[mediaScheme().title[lang] for lang in languages], 
-            *[mediaScheme().coverImage[size] for size in sizes]
-        ])
-    
-    
+from Anilist.scheme import *
+from Anilist.vars import Vars
+from Anilist.client.client import Client
+from Anilist.query.query import Query
+class MediaListQuery(Query):
+    """
+    An interface for making Queries for media lists to the Anilist API
+
+        
+    .. warning::
+
+        This usually should not be created manually, instead use :meth:`QueryClient.media_list() <.client.QueryClient.media_list>`
+
+    """
+    
+    def __init__(self, client: Client, languages=["english"], sizes=["extraLarge"]):
+        super().__init__(client, 'mediaList', 'MediaList', [
+            mediaScheme().id, 
+            *[mediaScheme().title[lang] for lang in languages], 
+            *[mediaScheme().coverImage[size] for size in sizes]
+        ])
+    
+
```

### Comparing `Anilist-0.9.0/Anilist/query/query.py` & `Anilist-0.9.1/Anilist/query/query.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-from Anilist.client import Client
-from Anilist.scheme.scheme import Scheme
-from Anilist.vars.vars import Vars
-
-
-class Query:
-    """An interface to make Queries to the Anilist API
-    This should usually not be used, instead use one of the subclasses
-
-    .. warning::
-
-        This usually should not be created manually
-
-    :param client: A :class:`~Anilist.client.QueryClient` to make requests
-    :type client: :class:`~.client.Client`
-        
-    :param head_nama: Name of the head :class:`~.scheme.Scheme` when in a Page object
-    :type head_nama: :class:`~str`
-
-    :param head_namb: Name of the head :class:`~.scheme.Scheme` when in a Query object
-    :type head_namb: :class:`~str`
-
-    :param defa: List of default :class:`~.scheme.Scheme`\s 
-    :type defa: list[:class:`~.scheme.Scheme`]
-
-    Example:
-
-    .. code-block:: python
-
-        
-        client = Anilist.QueryClient()
-        schs = Scheme().Media(type="$type", search="$search").sub_schemes(
-            Scheme().id,
-            Scheme().title.english
-        )
-        vars = Vars(type=AnilistMediaType("ANIME"), search="One Piece")
-        result = client._request(client._create_query(vars, *schs), vars)
-
-        # This is equivalent to using the following shortcut:
-        media_search = Anilist.QueryClient().media_entry()
-        media_search.search(
-            Scheme().id,
-            Scheme().title.english,
-
-            type=AnilistMediaType("ANIME"),
-            search="One Piece"
-        )
-        result = media_search.results_take_one()
-    """
-
-    def __init__(self, client: Client, head_nama, head_namb, defa):
-        self._results = []
-        self._client = client
-        self._head_name = (head_nama, head_namb)
-        self._base_schs = (Scheme()[head_namb], Scheme()[head_nama])
-
-        self.DEFAULT_QUERY = defa
-
-    def _query(self, *schs: Scheme, vars, head_sch, paginate=True, page=1, per_page=100):
-        r = []
-
-        if not paginate:
-
-            q = self._client._create_query(vars, *schs, head_sch=head_sch)
-            resp = self._client._request(q, vars)
-
-            r.append(resp[self._head_name[1]])
-
-        else:
-
-            vars = Vars._merge(vars, Vars(page=page, perPage=per_page))
-            q = self._client._create_query(vars, *schs, head_sch=Scheme._combine(Scheme().Page(page = '$page', perPage = '$perPage'), head_sch))
-
-            r = self._client._page_request(q, vars, self._head_name[0])
-        
-        self._results += r
-
-    
-    def get_base_sch(self, paginate):
-        return self._base_schs[0] if not paginate else self._base_schs[1]
-    
-    def search(self, *schs: Scheme, default=True, per_page: int=100, page: int=1, paginate=False, **kwargs):
-        """Send a query to the Anilist API and add the results to the result tray
-
-        :param schs: The Schemes to search for,
-            they will be appended to the specific Query object's head :class:`~.scheme.Scheme`
-        :type schs: tuple[:class:`~.scheme.Scheme`]
-
-        *Keyword Args*: 
-
-        :param default: Whether to add the specific Query object's default :class:`~.scheme.Scheme`\s (the default is True)
-        :type default: bool, optional
-
-        :param paginate: Whether to request a single element or pages of the element,
-            if set to True then several results will be added to the result tray (the default is False)
-        :type paginate: bool, optional
-
-        :param per_page: The number of objects to query per page, this is useless if paginate is set to False (the default is 100)
-        :type per_page: int, optional
-
-        :param page: The page to start on (the default is 1)
-        :type page: int, optional
-
-        *\*\*kwargs*:
-        
-        The kwargs pairs are all used to create the search query,
-        they are added as arguments to the specific Query object's head :class:`~.scheme.Scheme`
-
-        For example if you are using a :class:`~.query.MediaEntryQuery`:
-
-        .. code-block:: python
-
-            # ... get a MediaEntryQuery
-            media_search = ... # media_search is a MediaEntryQuery
-
-            media_search.search(
-                # Search schemes
-                Scheme().id
-                Scheme().status
-                Scheme().episodes
-                
-                # Search parameters
-                default=True
-                paginate=True
-                per_page=50
-                page=1
-
-                # Search arguments
-                type=AnilistMediaType("ANIME")
-                search="One Piece"
-            )
-
-            # This generates the following query and variables:
-            #
-            # Query:
-            #
-            # query (
-            #   $type: MediaType, 
-            #   $search: String, 
-            #   $perPage: Int, 
-            #   $page: Int
-            # ) {
-            #   Page (page: $page, perPage: $perPage) {
-            #       media (type: $type, search: $search) {
-            #           id
-            #           status
-            #           episodes
-            #       }
-            #    }
-            # }
-            #
-            # Variables:
-            #
-            # {
-            #   "search": "One Piece", 
-            #   "type": "ANIME", 
-            #   "perPage" 50, 
-            #   "page": 1
-            # }
-
-        """
-        # the main way to interact with this object
-        vars = Vars(**kwargs)
-
-        if default:
-            schs = list(schs)
-            schs.extend(self.DEFAULT_QUERY)
-
-        head_sch = self.get_base_sch(paginate)(**vars._as_query())
-        return self._query(*schs, head_sch=head_sch, vars=vars, paginate=paginate, per_page=per_page, page=page)
-
-    def results_take_all(self):
-        """Returns the whole result tray and empties it
-        """
-        r = self._results
-        self._results = []
-        return r
-    
-    def results_take_front(self):
-        """Returns the first element of the result tray
-        and removes it from the tray.
-                
-        :raises KeyError: If the Query Result is empty
-
-        :return: First element of the query's results tray
-        :rtype: AnilistObject
-        """
-        r = self._results[0]
-        self._results = self._results[1:]
-        return r
-    
-    def results_take_back(self):
-        """Returns the last element of the Query Result
-        and removes it from the Query Result
-
-        :raises KeyError: If the Query Result is empty
-
-        :return: Last element of the query's results tray
-        :rtype: :class:`AnilistObject`
-        """
-        r = self._results[-1]
-        self._results = self._results[:-1]
-        return r
-
+from Anilist.client import Client
+from Anilist.scheme.scheme import Scheme
+from Anilist.vars.vars import Vars
+
+
+class Query:
+    """An interface to make Queries to the Anilist API
+    This should usually not be used, instead use one of the subclasses
+
+    .. warning::
+
+        This usually should not be created manually
+
+    :param client: A :class:`~Anilist.client.QueryClient` to make requests
+    :type client: :class:`~.client.Client`
+        
+    :param head_name1: Name of the head :class:`~.scheme.Scheme` when in a Page object
+    :type head_nama: :class:`~str`
+
+    :param head_name2: Name of the head :class:`~.scheme.Scheme` when in a Query object
+    :type head_namb: :class:`~str`
+
+    :param defa: List of default :class:`~.scheme.Scheme`\s 
+    :type defa: list[:class:`~.scheme.Scheme`]
+
+    Example:
+
+    .. code-block:: python
+
+        
+        client = Anilist.QueryClient()
+        schs = Scheme().Media(type="$type", search="$search").sub_schemes(
+            Scheme().id,
+            Scheme().title.english
+        )
+        vars = Vars(type=AnilistMediaType("ANIME"), search="One Piece")
+        result = client._request(client._create_query(vars, *schs), vars)
+
+        # This is equivalent to using the following shortcut:
+        media_search = Anilist.QueryClient().media_entry()
+        media_search.search(
+            Scheme().id,
+            Scheme().title.english,
+
+            type=AnilistMediaType("ANIME"),
+            search="One Piece"
+        )
+        result = media_search.results_take_one()
+    """
+
+    def __init__(self, client: Client, head_name1, head_name2, defa):
+        self._results = []
+        self._client = client
+        self._head_name = (head_name1, head_name2)
+        self._base_schs = (Scheme()[head_name2], Scheme()[head_name1])
+
+        self.DEFAULT_QUERY = defa
+
+    def _query(self, *schs: Scheme, vars, head_sch, paginate=True, page=1, per_page=100):
+        r = []
+
+        if not paginate:
+
+            q = self._client._create_query(vars, *schs, head_sch=head_sch)
+            resp = self._client._request(q, vars)
+
+            r.append(resp[self._head_name[1]])
+
+        else:
+
+            vars = Vars._merge(vars, Vars(page=page, perPage=per_page))
+            q = self._client._create_query(vars, *schs, head_sch=Scheme._combine(Scheme().Page(page = '$page', perPage = '$perPage'), head_sch))
+
+            r = self._client._page_request(q, vars, self._head_name[0])
+        
+        self._results += r
+
+    
+    def get_base_sch(self, paginate):
+        return self._base_schs[0] if not paginate else self._base_schs[1]
+    
+    def search(self, *schs: Scheme, default=True, per_page: int=100, page: int=1, paginate=False, **kwargs):
+        """Send a query to the Anilist API and add the results to the result tray
+
+        :param schs: The Schemes to search for,
+            they will be appended to the specific Query object's head :class:`~.scheme.Scheme`
+        :type schs: tuple[:class:`~.scheme.Scheme`]
+
+        *Keyword Args*: 
+
+        :param default: Whether to add the specific Query object's default :class:`~.scheme.Scheme`\s (the default is True)
+        :type default: bool, optional
+
+        :param paginate: Whether to request a single element or pages of the element,
+            if set to True then several results will be added to the result tray (the default is False)
+        :type paginate: bool, optional
+
+        :param per_page: The number of objects to query per page, this is useless if paginate is set to False (the default is 100)
+        :type per_page: int, optional
+
+        :param page: The page to start on (the default is 1)
+        :type page: int, optional
+
+        *\*\*kwargs*:
+        
+        The kwargs pairs are all used to create the search query,
+        they are added as arguments to the specific Query object's head :class:`~.scheme.Scheme`
+
+        For example if you are using a :class:`~.query.MediaEntryQuery`:
+
+        .. code-block:: python
+
+            # ... get a MediaEntryQuery
+            media_search = ... # media_search is a MediaEntryQuery
+
+            media_search.search(
+                # Search schemes
+                Scheme().id
+                Scheme().status
+                Scheme().episodes
+                
+                # Search parameters
+                default=True
+                paginate=True
+                per_page=50
+                page=1
+
+                # Search arguments
+                type=AnilistMediaType("ANIME")
+                search="One Piece"
+            )
+
+            # This generates the following query and variables:
+            #
+            # Query:
+            #
+            # query (
+            #   $type: MediaType, 
+            #   $search: String, 
+            #   $perPage: Int, 
+            #   $page: Int
+            # ) {
+            #   Page (page: $page, perPage: $perPage) {
+            #       media (type: $type, search: $search) {
+            #           id
+            #           status
+            #           episodes
+            #       }
+            #    }
+            # }
+            #
+            # Variables:
+            #
+            # {
+            #   "search": "One Piece", 
+            #   "type": "ANIME", 
+            #   "perPage" 50, 
+            #   "page": 1
+            # }
+
+        """
+        # the main way to interact with this object
+        vars = Vars(**kwargs)
+
+        if default:
+            schs = list(schs)
+            schs.extend(self.DEFAULT_QUERY)
+
+        head_sch = self.get_base_sch(paginate)(**vars._as_query())
+        return self._query(*schs, head_sch=head_sch, vars=vars, paginate=paginate, per_page=per_page, page=page)
+
+    def results_take_all(self):
+        """Returns the whole result tray and empties it
+        """
+        r = self._results
+        self._results = []
+        return r
+    
+    def results_take_front(self):
+        """Returns the first element of the result tray
+        and removes it from the tray.
+                
+        :raises KeyError: If the Query Result is empty
+
+        :return: First element of the query's results tray
+        :rtype: AnilistObject
+        """
+        r = self._results[0]
+        self._results = self._results[1:]
+        return r
+    
+    def results_take_back(self):
+        """Returns the last element of the Query Result
+        and removes it from the Query Result
+
+        :raises KeyError: If the Query Result is empty
+
+        :return: Last element of the query's results tray
+        :rtype: :class:`AnilistObject`
+        """
+        r = self._results[-1]
+        self._results = self._results[:-1]
+        return r
+
```

### Comparing `Anilist-0.9.0/Anilist/scheme/media_scheme.py` & `Anilist-0.9.1/Anilist/scheme/media_scheme.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from .scheme import Scheme
-
-class MediaScheme(Scheme):
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._layers.append("Media")
-        self(**kwargs)
-
-class mediaScheme(Scheme):
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._layers.append("media")
-        self(**kwargs)
-
-class mediaListScheme(Scheme):
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._layers.append("mediaList")
-        self(**kwargs)
-
-class MediaListScheme(Scheme):
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._layers.append("MediaList")
+from .scheme import Scheme
+
+class MediaScheme(Scheme):
+    def __init__(self, **kwargs):
+        super().__init__()
+        self._layers.append("Media")
+        self(**kwargs)
+
+class mediaScheme(Scheme):
+    def __init__(self, **kwargs):
+        super().__init__()
+        self._layers.append("media")
+        self(**kwargs)
+
+class mediaListScheme(Scheme):
+    def __init__(self, **kwargs):
+        super().__init__()
+        self._layers.append("mediaList")
+        self(**kwargs)
+
+class MediaListScheme(Scheme):
+    def __init__(self, **kwargs):
+        super().__init__()
+        self._layers.append("MediaList")
         self(**kwargs)
```

### Comparing `Anilist-0.9.0/Anilist/scheme/scheme.py` & `Anilist-0.9.1/Anilist/scheme/scheme.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-class Scheme:
-    """    
-    The main way to select fields to query in Anilist requests
-    
-    For example the following list of Schemes:
-
-    .. code-block:: python
-
-        Scheme().FieldA(id='$idVariable')
-            .sub_schemes(
-                Scheme().FieldB, 
-                Scheme().FieldB.FieldC, 
-                Scheme().FieldD
-            )
-
-    will be parsed into a query by the :class:`~.client.Client` as::
-    
-        FieldA (id: $idVariable) {
-            FieldB {
-                FieldC
-            }
-            FieldD
-        }
-    
-    .. note::
-        Schemes are parsed by :meth:`Client._create_query() <.client.Client._create_query>`
-        Which is automatically called by :meth:`Query.search() <.query.Query.search>`
-
-        Depending on the query parameters and the client type this will be wrapped into either a `query { }` block, a `query { Page { } }` block or a `mutation { }` block
-
-    """
-
-    def __init__(self):
-        self._layers = []
-        self._up = {}
-
-    def sub_schemes(self, *schs):
-        """Appends this :class:`~.Scheme` at the beginning of all of the :class:`~.Scheme`\s provided and returns them
-
-        :param schs: List of :class:`~.Scheme`\s to append to this one
-        :type schs: tuple[:class:`~.Scheme`], optional
-
-        Example: 
-
-        .. code-block:: python
-
-            Scheme().FieldA.sub_schemes(
-                Scheme().FieldB
-                Scheme().FieldB.FieldC
-                Scheme().FieldD
-            )
-
-            # is equivalent to
-
-            [
-                Scheme().FieldA,
-                Scheme().FieldA.FieldB
-                Scheme().FieldA.FieldB.FieldC
-                Scheme().FieldA.FieldD
-            ]
-            
-        """
-        return [Scheme._combine(self, sch) for sch in schs] + [self]
-
-
-    def __getattr__(self, k):
-        return self[k]
-    
-    def __getitem__(self, k):
-        self._layers.append(k)
-        return self
-    
-    def __call__(self, **kwargs):
-        d = dict(**kwargs)
-        if d != {}:
-            self._up[self._layers[-1]] = f"{self._layers[-1]} ({', '.join([f'{k}: {v}' for k, v in d.items()])})"
-        return self
-    
-    def _replace_head(self, pat, r):
-        self._layers[0] = str(self._layers[0]).replace(pat, r)
-        tch = []
-        for k, v in self._up.items():
-            if k == pat:
-                tch.append(k)
-
-        for k in tch:
-            self._up[r] = str(self._up.pop(k)).replace(pat, r)
-
-        return self
-    
-    @classmethod
-    def _construct(cls, *schs):
-        d = {k: v for sch in schs for k, v in sch._up.items()}
-        return construct_query_as_string(construct_query(list(schs)), d)
-    
-    @classmethod
-    def _combine(cls, scha, schb):
-        n = cls()
-        n._layers = scha._layers + schb._layers
-        n._up = scha._up | schb._up
-        return n
-    
-def construct_query(schs: list[Scheme]):
-    temp = {}
-
-    for sch in schs:
-        sch = sch._layers
-        if not sch[0] in temp:
-            temp[sch[0]] = {}
-        for i in range(1, len(sch)):
-            if not sch[i] in get_nest_list(get_numbers_up_to(i), temp, i, sch):
-                get_nest_list(get_numbers_up_to(i), temp, i, sch)[sch[i]] = {}
-
-    
-    return temp
-
-
-def construct_query_as_string(d, l, ss=""):
-    if type(d) != dict:
-        return str(d)
-    
-    s = ""
-
-    for k, v in d.items():
-        nk = k if k not in l else l[k]
-        if v == {}:
-            s = f"{s}{ss}{nk}\n"
-        else:
-            t = construct_query_as_string(v, l, f'{ss}  ')
-            t = t[0:-1]
-            s = f"{s}{ss}{nk} {{\n{t}\n{ss}}}\n"
-
-    return s
-
-
-def get_numbers_up_to(i):
-    l = []
-    n = i
-    while n > 0:
-        l.append(n)
-        n -= 1
-    
-    return l
-
-def get_nest_list(n, l, m, sch):
-    prev = l
-    for i in n:
-        prev = prev[sch[m-i]]
-    return prev
-    
+class Scheme:
+    """    
+    The main way to select fields to query in Anilist requests
+    
+    For example the following list of Schemes:
+
+    .. code-block:: python
+
+        Scheme().FieldA(id='$idVariable')
+            .sub_schemes(
+                Scheme().FieldB, 
+                Scheme().FieldB.FieldC, 
+                Scheme().FieldD
+            )
+
+    will be parsed into a query by the :class:`~.client.Client` as::
+    
+        FieldA (id: $idVariable) {
+            FieldB {
+                FieldC
+            }
+            FieldD
+        }
+    
+    .. note::
+        Schemes are parsed by :meth:`Client._create_query() <.client.Client._create_query>`
+        Which is automatically called by :meth:`Query.search() <.query.Query.search>`
+
+        Depending on the query parameters and the client type this will be wrapped into either a `query { }` block, a `query { Page { } }` block or a `mutation { }` block
+
+    """
+
+    def __init__(self):
+        self._layers = []
+        self._up = {}
+
+    def sub_schemes(self, *schs):
+        """Appends this :class:`~.Scheme` at the beginning of all of the :class:`~.Scheme`\s provided and returns them
+
+        :param schs: List of :class:`~.Scheme`\s to append to this one
+        :type schs: tuple[:class:`~.Scheme`], optional
+
+        Example: 
+
+        .. code-block:: python
+
+            Scheme().FieldA.sub_schemes(
+                Scheme().FieldB
+                Scheme().FieldB.FieldC
+                Scheme().FieldD
+            )
+
+            # is equivalent to
+
+            [
+                Scheme().FieldA,
+                Scheme().FieldA.FieldB
+                Scheme().FieldA.FieldB.FieldC
+                Scheme().FieldA.FieldD
+            ]
+            
+        """
+        return [Scheme._combine(self, sch) for sch in schs] + [self]
+
+
+    def __getattr__(self, k):
+        return self[k]
+    
+    def __getitem__(self, k):
+        self._layers.append(k)
+        return self
+    
+    def __call__(self, **kwargs):
+        d = dict(**kwargs)
+        if d != {}:
+            self._up[self._layers[-1]] = f"{self._layers[-1]} ({', '.join([f'{k}: {v}' for k, v in d.items()])})"
+        return self
+    
+    def _replace_head(self, pat, r):
+        self._layers[0] = str(self._layers[0]).replace(pat, r)
+        tch = []
+        for k, v in self._up.items():
+            if k == pat:
+                tch.append(k)
+
+        for k in tch:
+            self._up[r] = str(self._up.pop(k)).replace(pat, r)
+
+        return self
+    
+    @classmethod
+    def _construct(cls, *schs):
+        d = {k: v for sch in schs for k, v in sch._up.items()}
+        return construct_query_as_string(construct_query(list(schs)), d)
+    
+    @classmethod
+    def _combine(cls, scha, schb):
+        n = cls()
+        n._layers = scha._layers + schb._layers
+        n._up = scha._up | schb._up
+        return n
+    
+def construct_query(schs: list[Scheme]):
+    temp = {}
+
+    for sch in schs:
+        sch = sch._layers
+        if not sch[0] in temp:
+            temp[sch[0]] = {}
+        for i in range(1, len(sch)):
+            if not sch[i] in get_nest_list(get_numbers_up_to(i), temp, i, sch):
+                get_nest_list(get_numbers_up_to(i), temp, i, sch)[sch[i]] = {}
+
+    
+    return temp
+
+
+def construct_query_as_string(d, l, ss=""):
+    if type(d) != dict:
+        return str(d)
+    
+    s = ""
+
+    for k, v in d.items():
+        nk = k if k not in l else l[k]
+        if v == {}:
+            s = f"{s}{ss}{nk}\n"
+        else:
+            t = construct_query_as_string(v, l, f'{ss}  ')
+            t = t[0:-1]
+            s = f"{s}{ss}{nk} {{\n{t}\n{ss}}}\n"
+
+    return s
+
+
+def get_numbers_up_to(i):
+    l = []
+    n = i
+    while n > 0:
+        l.append(n)
+        n -= 1
+    
+    return l
+
+def get_nest_list(n, l, m, sch):
+    prev = l
+    for i in n:
+        prev = prev[sch[m-i]]
+    return prev
+
```

### Comparing `Anilist-0.9.0/Anilist/utils/logging.py` & `Anilist-0.9.1/Anilist/utils/logging.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import logging
-
-class AnilistFormatter(logging.Formatter):
-
-    black = "\x1b[30;20m"
-    blue = "\x1b[34;20m"
-    green = "\x1b[32;20m"
-    grey = "\x1b[38;20m"
-    yellow = "\x1b[33;20m"
-    red = "\x1b[31;20m"
-    bold_red = "\x1b[31;1m"
-    reset = "\x1b[0m"
-    format = "[%(asctime)s]: %(levelname)s - %(message)s (%(filename)s:%(lineno)d)"
-
-    FORMATS = {
-        logging.DEBUG: green + format + reset,
-        logging.INFO: blue + format + reset,
-        logging.WARNING: yellow + format + reset,
-        logging.ERROR: red + format + reset,
-        logging.CRITICAL: bold_red + format + reset
-    }
-
-    def format(self, record):
-        log_fmt = self.FORMATS.get(record.levelno)
-        formatter = logging.Formatter(log_fmt)
-        return formatter.format(record)
-    
-# Singleton
-class AnilistLogger:
-    _instance = None
-    _done = False
-
-    def __init__(self, level = logging.INFO):
-        if not AnilistLogger._done:
-            logger = logging.getLogger("AnilistLogger")
-            logger.setLevel(level)
-
-            ch = logging.StreamHandler()
-            ch.setLevel(level)
-
-            ch.setFormatter(AnilistFormatter())
-
-            logger.addHandler(ch)
-
-            self._logger = logger
-            AnilistLogger._done = True
-
-    def __new__(cls, *args, **kwargs):
-        if cls._instance is None:
-            cls._instance = super(AnilistLogger, cls).__new__(cls)
-        
-        return cls._instance
-
-    def __getattr__(self, k):
+import logging
+
+class AnilistFormatter(logging.Formatter):
+
+    black = "\x1b[30;20m"
+    blue = "\x1b[34;20m"
+    green = "\x1b[32;20m"
+    grey = "\x1b[38;20m"
+    yellow = "\x1b[33;20m"
+    red = "\x1b[31;20m"
+    bold_red = "\x1b[31;1m"
+    reset = "\x1b[0m"
+    format = "[%(asctime)s]: %(levelname)s - %(message)s (%(filename)s:%(lineno)d)"
+
+    FORMATS = {
+        logging.DEBUG: green + format + reset,
+        logging.INFO: blue + format + reset,
+        logging.WARNING: yellow + format + reset,
+        logging.ERROR: red + format + reset,
+        logging.CRITICAL: bold_red + format + reset
+    }
+
+    def format(self, record):
+        log_fmt = self.FORMATS.get(record.levelno)
+        formatter = logging.Formatter(log_fmt)
+        return formatter.format(record)
+    
+# Singleton
+class AnilistLogger:
+    _instance = None
+    _done = False
+
+    def __init__(self, level = logging.INFO):
+        if not AnilistLogger._done:
+            logger = logging.getLogger("AnilistLogger")
+            logger.setLevel(level)
+
+            ch = logging.StreamHandler()
+            ch.setLevel(level)
+
+            ch.setFormatter(AnilistFormatter())
+
+            logger.addHandler(ch)
+
+            self._logger = logger
+            AnilistLogger._done = True
+
+    def __new__(cls, *args, **kwargs):
+        if cls._instance is None:
+            cls._instance = super(AnilistLogger, cls).__new__(cls)
+        
+        return cls._instance
+
+    def __getattr__(self, k):
         return self._logger.__getattribute__(k)
```

### Comparing `Anilist-0.9.0/Anilist/utils/object.py` & `Anilist-0.9.1/Anilist/utils/object.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-class AnilistObject:
-    """An object representing data sent by the Anilist API
-    
-    .. warning:: 
-    
-        This should never be created manually
-
-    .. note::
-        
-        The attributes for any specific :class:`~AnilistObject` are the same as for the :class:`~.scheme.Scheme` provided in the request
-
-    Example:
-
-    .. code-block:: python
-
-        ###! In a raw Client request
-        client = Anilist.QueryClient()
-        query = \"\"\"
-            Media (type: $type, search: $search) {
-                id
-                title {
-                    english
-                }
-            }
-        \"\"\"
-        result = client._request(
-            query,
-            vars=Vars(type=AnilistMediaType("ANIME"), search="One Piece")
-        )
-        # result is an AnilistObject with the following attributes
-        id = result.Media.id
-        english_title = result.Media.title.english
-
-        ###! In a basic Client request
-        client = Anilist.QueryClient()
-        schs = Scheme().Media(type="$type", search="$search").sub_schemes(
-            Scheme().id,
-            Scheme().title.english
-        )
-        vars = Vars(type=AnilistMediaType("ANIME"), search="One Piece")
-        result = client._request(client._create_query(vars, *schs), vars)
-
-        # result is an AnilistObject with the following attributes
-        id = result.Media.id
-        english_title = result.Media.title.english
-
-        
-
-        ###! Using the Query API
-        media_search = Anilist.QueryClient().media_entry()
-        media_search.search(
-            Scheme().id,
-            Scheme().title.english,
-
-            type=AnilistMediaType("ANIME"),
-            search="One Piece"
-        )
-        result = media_search.results_take_one()
-
-        # The Query API automatically returns 
-        # only the inner part of the request
-        # so you do not need to do 'result.Media'
-        # result is an AnilistObject with the following attributes
-        id = result.id
-        english_title = result.title.english
-        # This one is added because the MediaEntryQuery API 
-        # has coverImage.extraLarge as a default field to query
-        extra_large_cover = result.coverImage.extraLarge
-        
-    """
-    
-    def __init__(self, json_object):
-        self.__dict = {}
-        for k, v in json_object.items():
-            if type(v) is dict:
-                self.__dict[k] = AnilistObject(v)
-            elif type(v) is list:
-                self.__dict[k] = [AnilistObject(el) if type(el) is dict else el for el in v]
-            else:
-                self.__dict[k] = v
-
-    def __getattr__(self, k):
-        return self.__dict[k]
-    
-    def __getitem__(self, k):
-        return self.__dict[k]
-    
-    def __str__(self):
-        return str(self.__dict)
-    
-    def __repr__(self):
+class AnilistObject:
+    """An object representing data sent by the Anilist API
+    
+    .. warning:: 
+    
+        This should never be created manually
+
+    .. note::
+        
+        The attributes for any specific :class:`~AnilistObject` are the same as for the :class:`~.scheme.Scheme` provided in the request
+
+    Example:
+
+    .. code-block:: python
+
+        ###! In a raw Client request
+        client = Anilist.QueryClient()
+        query = \"\"\"
+            Media (type: $type, search: $search) {
+                id
+                title {
+                    english
+                }
+            }
+        \"\"\"
+        result = client._request(
+            query,
+            vars=Vars(type=AnilistMediaType("ANIME"), search="One Piece")
+        )
+        # result is an AnilistObject with the following attributes
+        id = result.Media.id
+        english_title = result.Media.title.english
+
+        ###! In a basic Client request
+        client = Anilist.QueryClient()
+        schs = Scheme().Media(type="$type", search="$search").sub_schemes(
+            Scheme().id,
+            Scheme().title.english
+        )
+        vars = Vars(type=AnilistMediaType("ANIME"), search="One Piece")
+        result = client._request(client._create_query(vars, *schs), vars)
+
+        # result is an AnilistObject with the following attributes
+        id = result.Media.id
+        english_title = result.Media.title.english
+
+        
+
+        ###! Using the Query API
+        media_search = Anilist.QueryClient().media_entry()
+        media_search.search(
+            Scheme().id,
+            Scheme().title.english,
+
+            type=AnilistMediaType("ANIME"),
+            search="One Piece"
+        )
+        result = media_search.results_take_one()
+
+        # The Query API automatically returns 
+        # only the inner part of the request
+        # so you do not need to do 'result.Media'
+        # result is an AnilistObject with the following attributes
+        id = result.id
+        english_title = result.title.english
+        # This one is added because the MediaEntryQuery API 
+        # has coverImage.extraLarge as a default field to query
+        extra_large_cover = result.coverImage.extraLarge
+        
+    """
+    
+    def __init__(self, json_object):
+        self.__dict = {}
+        for k, v in json_object.items():
+            if type(v) is dict:
+                self.__dict[k] = AnilistObject(v)
+            elif type(v) is list:
+                self.__dict[k] = [AnilistObject(el) if type(el) is dict else el for el in v]
+            else:
+                self.__dict[k] = v
+
+    def __getattr__(self, k):
+        return self.__dict[k]
+    
+    def __getitem__(self, k):
+        return self.__dict[k]
+    
+    def __str__(self):
+        return str(self.__dict)
+    
+    def __repr__(self):
         return str(self)
```

### Comparing `Anilist-0.9.0/Anilist/vars/vars.py` & `Anilist-0.9.1/Anilist/vars/vars.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from Anilist.anilist_types import AnilistType
-
-class Vars:
-    """
-    Set of request variables that can be used in Schemes
-    Each variable can be referenced by Schemes by prefixing their name with '$'
-
-    Example::
-        
-        client = QueryClient()
-        # $type and $search
-        # reference the Vars' 'type' and 'search' kwargs
-        schs = Scheme().Media(type="$type", search="$search").sub_schemes(
-            Scheme().id,
-            Scheme().title.english
-        )
-        vars = Vars(type=AnilistMediaType("ANIME"), search="One Piece")
-        result = client._request(client._create_query(vars, *schs), vars)
-
-        ## This is equivalent to using the following shortcut:
-        media_search = QueryClient().media_entry()
-        media_search.search(
-            Scheme().id,
-            Scheme().title.english,
-
-            type=AnilistMediaType("ANIME"),
-            search="One Piece"
-        )
-        result = media_search.results_take_one()
-    """
-    
-    def __init__(self, **kwargs):
-        dic = dict(kwargs)
-        l = []
-        for k, v in dic.items(): 
-            if isinstance(v, AnilistType):
-                dic[k] = v.get_inner()
-                l.append(f"${k}: {v.__class__.ANILIST_TYPE_NAME}")
-            else:
-                l.append(f"${k}: {AnilistType(v).__class__.ANILIST_TYPE_NAME}")
-
-
-        self._dic = dic
-        self._vars = l
-
-    def update(self, k, v):
-        if isinstance(v, AnilistType):
-            self._dic[k] = v.get_inner()
-        else:
-            self._dic[k] = v
-
-    def _as_query(self):
-        temp = {}
-
-        for k, v in self._dic.items():
-            temp[k] = f"${k}"
-
-        return temp
-
-    @property
-    def _names(self):
-        return ', '.join(self._vars)
-    
-    @property
-    def _json(self):
-        return self._dic
-    
-    @classmethod 
-    def _merge(cls, vara, varb):
-        n = Vars()
-
-        n._vars = vara._vars + varb._vars
-        n._dic = vara._dic | varb._dic
-
-        return n
+from Anilist.anilist_types import AnilistType
+
+class Vars:
+    """
+    Set of request variables that can be used in Schemes
+    Each variable can be referenced by Schemes by prefixing their name with '$'
+
+    Example::
+        
+        client = QueryClient()
+        # $type and $search
+        # reference the Vars' 'type' and 'search' kwargs
+        schs = Scheme().Media(type="$type", search="$search").sub_schemes(
+            Scheme().id,
+            Scheme().title.english
+        )
+        vars = Vars(type=AnilistMediaType("ANIME"), search="One Piece")
+        result = client._request(client._create_query(vars, *schs), vars)
+
+        ## This is equivalent to using the following shortcut:
+        media_search = QueryClient().media_entry()
+        media_search.search(
+            Scheme().id,
+            Scheme().title.english,
+
+            type=AnilistMediaType("ANIME"),
+            search="One Piece"
+        )
+        result = media_search.results_take_one()
+    """
+    
+    def __init__(self, **kwargs):
+        dic = dict(kwargs)
+        l = []
+        for k, v in dic.items(): 
+            if isinstance(v, AnilistType):
+                dic[k] = v.get_inner()
+                l.append(f"${k}: {v.__class__.ANILIST_TYPE_NAME}")
+            else:
+                l.append(f"${k}: {AnilistType(v).__class__.ANILIST_TYPE_NAME}")
+
+
+        self._dic = dic
+        self._vars = l
+
+    def update(self, k, v):
+        if isinstance(v, AnilistType):
+            self._dic[k] = v.get_inner()
+        else:
+            self._dic[k] = v
+
+    def _as_query(self):
+        temp = {}
+
+        for k, v in self._dic.items():
+            temp[k] = f"${k}"
+
+        return temp
+
+    @property
+    def _names(self):
+        return ', '.join(self._vars)
+    
+    @property
+    def _json(self):
+        return self._dic
+    
+    @classmethod 
+    def _merge(cls, vara, varb):
+        n = Vars()
+
+        n._vars = vara._vars + varb._vars
+        n._dic = vara._dic | varb._dic
+
+        return n
```

### Comparing `Anilist-0.9.0/Anilist.egg-info/PKG-INFO` & `Anilist-0.9.1/Anilist.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1
-Name: Anilist
-Version: 0.9.0
-Summary: Anilist API wrapper
-Author-email: Ann Mauduy-Decius <ann.mauduy.decius@gmail.com>
-Project-URL: Homepage, https://github.com/xxxAnn/Anilist.py
-Project-URL: Bug Tracker, https://github.com/xxxAnn/Anilist.py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-I'll do a documentation one day, probably!
+Metadata-Version: 2.1
+Name: Anilist
+Version: 0.9.1
+Summary: Anilist API wrapper
+Author-email: Ann Mauduy-Decius <ann.mauduy.decius@gmail.com>
+Project-URL: Homepage, https://github.com/xxxAnn/Anilist.py
+Project-URL: Bug Tracker, https://github.com/xxxAnn/Anilist.py/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+I'll do a documentation one day, probably!
```

### Comparing `Anilist-0.9.0/Anilist.egg-info/SOURCES.txt` & `Anilist-0.9.1/Anilist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Anilist-0.9.0/LICENSE` & `Anilist-0.9.1/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2023 Ann Mauduy-Decius
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2023 Ann Mauduy-Decius
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `Anilist-0.9.0/PKG-INFO` & `Anilist-0.9.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1
-Name: Anilist
-Version: 0.9.0
-Summary: Anilist API wrapper
-Author-email: Ann Mauduy-Decius <ann.mauduy.decius@gmail.com>
-Project-URL: Homepage, https://github.com/xxxAnn/Anilist.py
-Project-URL: Bug Tracker, https://github.com/xxxAnn/Anilist.py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-I'll do a documentation one day, probably!
+Metadata-Version: 2.1
+Name: Anilist
+Version: 0.9.1
+Summary: Anilist API wrapper
+Author-email: Ann Mauduy-Decius <ann.mauduy.decius@gmail.com>
+Project-URL: Homepage, https://github.com/xxxAnn/Anilist.py
+Project-URL: Bug Tracker, https://github.com/xxxAnn/Anilist.py/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+I'll do a documentation one day, probably!
```

### Comparing `Anilist-0.9.0/pyproject.toml` & `Anilist-0.9.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "Anilist"
-version = "0.9.0"
-authors = [
-  { name="Ann Mauduy-Decius", email="ann.mauduy.decius@gmail.com" },
-]
-description = "Anilist API wrapper"
-readme = "README.md"
-requires-python = ">=3.10"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/xxxAnn/Anilist.py"
-"Bug Tracker" = "https://github.com/xxxAnn/Anilist.py/issues"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "Anilist"
+version = "0.9.1"
+authors = [
+  { name="Ann Mauduy-Decius", email="ann.mauduy.decius@gmail.com" },
+]
+description = "Anilist API wrapper"
+readme = "README.md"
+requires-python = ">=3.10"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/xxxAnn/Anilist.py"
+"Bug Tracker" = "https://github.com/xxxAnn/Anilist.py/issues"
```

