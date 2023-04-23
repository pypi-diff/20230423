# Comparing `tmp/hallon-0.0.1.tar.gz` & `tmp/hallon-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hallon-0.0.1.tar", last modified: Sun Apr 23 08:03:37 2023, max compression
+gzip compressed data, was "hallon-0.0.2.tar", last modified: Sun Apr 23 13:12:33 2023, max compression
```

## Comparing `hallon-0.0.1.tar` & `hallon-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-23 08:03:37.729922 hallon-0.0.1/
--rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 hallon-0.0.1/LICENSE
--rw-r--r--   0 taiyuan    (501) staff       (20)     1950 2023-04-23 08:03:37.729791 hallon-0.0.1/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)      410 2023-04-23 08:02:07.000000 hallon-0.0.1/README.md
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-23 08:03:37.728736 hallon-0.0.1/hallon/
--rw-r--r--   0 taiyuan    (501) staff       (20)      115 2023-04-22 09:31:47.000000 hallon-0.0.1/hallon/__init__.py
--rw-r--r--   0 taiyuan    (501) staff       (20)     3127 2023-04-23 04:31:20.000000 hallon-0.0.1/hallon/cli.py
--rw-r--r--   0 taiyuan    (501) staff       (20)       48 2023-04-22 12:23:12.000000 hallon-0.0.1/hallon/exception.py
--rw-r--r--   0 taiyuan    (501) staff       (20)      151 2023-04-22 12:14:31.000000 hallon-0.0.1/hallon/func.py
--rw-r--r--   0 taiyuan    (501) staff       (20)      488 2023-04-22 10:50:41.000000 hallon-0.0.1/hallon/lang.py
--rw-r--r--   0 taiyuan    (501) staff       (20)     6791 2023-04-23 07:33:00.000000 hallon-0.0.1/hallon/switch.py
--rw-r--r--   0 taiyuan    (501) staff       (20)     3642 2023-04-22 10:48:07.000000 hallon-0.0.1/hallon/tools.py
--rw-r--r--   0 taiyuan    (501) staff       (20)     4355 2023-04-23 07:46:07.000000 hallon-0.0.1/hallon/topo.py
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-23 08:03:37.729596 hallon-0.0.1/hallon.egg-info/
--rw-r--r--   0 taiyuan    (501) staff       (20)     1950 2023-04-23 08:03:37.000000 hallon-0.0.1/hallon.egg-info/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)      310 2023-04-23 08:03:37.000000 hallon-0.0.1/hallon.egg-info/SOURCES.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-23 08:03:37.000000 hallon-0.0.1/hallon.egg-info/dependency_links.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       69 2023-04-23 08:03:37.000000 hallon-0.0.1/hallon.egg-info/entry_points.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        7 2023-04-23 08:03:37.000000 hallon-0.0.1/hallon.egg-info/top_level.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-23 08:03:37.729975 hallon-0.0.1/setup.cfg
--rw-r--r--   0 taiyuan    (501) staff       (20)      699 2023-04-23 08:02:07.000000 hallon-0.0.1/setup.py
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-23 13:12:33.366270 hallon-0.0.2/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 hallon-0.0.2/LICENSE
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1956 2023-04-23 13:12:33.366146 hallon-0.0.2/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)      416 2023-04-23 13:12:06.000000 hallon-0.0.2/README.md
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-23 13:12:33.365050 hallon-0.0.2/hallon/
+-rw-r--r--   0 taiyuan    (501) staff       (20)      115 2023-04-22 09:31:47.000000 hallon-0.0.2/hallon/__init__.py
+-rw-r--r--   0 taiyuan    (501) staff       (20)        0 2023-04-23 08:15:17.000000 hallon-0.0.2/hallon/ap.py
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3317 2023-04-23 12:40:18.000000 hallon-0.0.2/hallon/cli.py
+-rw-r--r--   0 taiyuan    (501) staff       (20)       48 2023-04-22 12:23:12.000000 hallon-0.0.2/hallon/exception.py
+-rw-r--r--   0 taiyuan    (501) staff       (20)      151 2023-04-22 12:14:31.000000 hallon-0.0.2/hallon/func.py
+-rw-r--r--   0 taiyuan    (501) staff       (20)      488 2023-04-22 10:50:41.000000 hallon-0.0.2/hallon/lang.py
+-rw-r--r--   0 taiyuan    (501) staff       (20)     8581 2023-04-23 12:32:00.000000 hallon-0.0.2/hallon/switch.py
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3642 2023-04-22 10:48:07.000000 hallon-0.0.2/hallon/tools.py
+-rw-r--r--   0 taiyuan    (501) staff       (20)     4498 2023-04-23 13:10:48.000000 hallon-0.0.2/hallon/topo.py
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-23 13:12:33.365953 hallon-0.0.2/hallon.egg-info/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1956 2023-04-23 13:12:33.000000 hallon-0.0.2/hallon.egg-info/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)      323 2023-04-23 13:12:33.000000 hallon-0.0.2/hallon.egg-info/SOURCES.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-23 13:12:33.000000 hallon-0.0.2/hallon.egg-info/dependency_links.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       69 2023-04-23 13:12:33.000000 hallon-0.0.2/hallon.egg-info/entry_points.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        7 2023-04-23 13:12:33.000000 hallon-0.0.2/hallon.egg-info/top_level.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-23 13:12:33.366313 hallon-0.0.2/setup.cfg
+-rw-r--r--   0 taiyuan    (501) staff       (20)      699 2023-04-23 13:12:06.000000 hallon-0.0.2/setup.py
```

### Comparing `hallon-0.0.1/LICENSE` & `hallon-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hallon-0.0.1/PKG-INFO` & `hallon-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hallon
-Version: 0.0.1
+Version: 0.0.2
 Summary: hallon is a package for network debugging
 Home-page: https://github.com/RyanYuanSun/hallon
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
@@ -41,15 +41,15 @@
 ```bash
 pip install hallon
 ```
 
 ## Usage
 ### Generate network topology
 ```shell
-hallon -nt -cadr 47.104.22.0 -cusr admin -cpas ruijie@123 -cprt 63275 -cenpas ruijie@123 -upas ruijie@123 -uprt 23
+hallon -nt -cadr 47.104.22.0 -cusr admin -cpas ruijie@123 -cprt 63275 -cenpas ruijie@123 -upas ruijie@123 -uprt 23 -tt 5
 ```
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/) License
 
 Copyright (c) 2023 Ryan Alloriadonis
```

### Comparing `hallon-0.0.1/hallon/cli.py` & `hallon-0.0.2/hallon/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse
-from hallon import lang
+from hallon import lang, topo
 
 
 def show_welcome(l):
     print(lang.get_msg("welcome_msg", l))
 
 
 def show_version(l):
@@ -26,39 +26,43 @@
     parser.add_argument("-cusr", "--core_username", type=str, help="username for logging in to the core switch", default="admin")
     parser.add_argument("-cpas", "--core_password", type=str, help="password for logging in to the core switch")
     parser.add_argument("-cenpas", "--core_enable_password", type=str, help="enable password for the core switch")
     parser.add_argument("-uprt", "--unified_port", type=int, help="general telnet port", default=23)
     parser.add_argument("-uusr", "--unified_username", type=str, help="general username for telnet login")
     parser.add_argument("-upas", "--unified_password", type=str, help="general password for telnet login")
     parser.add_argument("-uenpas", "--unified_enable_password", type=str, help="general enable password for telnet")
+    parser.add_argument("-tt", "--telnet_timeout", type=float, help="telnet global timeout", default=1)
 
     args = parser.parse_args()
 
     cli_lang = args.cli_lang.strip().lower()
     multi_proc_num = args.thread_num
     version_display = args.version
     network_topology = args.network_topology
 
     if version_display:
         show_version(cli_lang)
         exit()
 
+    if args.telnet_timeout <= 0:
+        parser.error("--telnet_timeout must be greater than 0")
+
     if network_topology:
         if args.network_topology and (args.core_address is None or args.core_password is None or args.core_enable_password is None):
             parser.error("--network_topology requires --core_address, --core_password and --core_enable_password")
         else:
             if args.unified_username is None:
                 args.unified_username = args.core_username
             if args.unified_password is None:
                 args.unified_password = args.core_password
             if args.unified_enable_password is None:
                 args.unified_enable_password = args.core_enable_password
             from hallon import func
             if func.is_ipv4(args.core_address.strip()) and 0 <= args.core_port <= 65536:
-                generate_topology(cli_lang, args)
+                topo.main(args)
             else:
                 parser.error("--core_address/--core_port invalid.")
         exit()
 
     if cli_lang not in lang.get_lang():
         # raise ValueError("Bad argument: -l, supported language:", lang.get_lang())
         print("Bad argument: -l, supported languages:", lang.get_lang(), ", default language:", lang.get_default_lang())
```

### Comparing `hallon-0.0.1/hallon/switch.py` & `hallon-0.0.2/hallon/switch.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,70 +32,122 @@
         return [tn, host_name]
     except:
         # print("Failed.")
         tn.close()
         return -1
 
 
+def decode_tel_info(raw):
+    try:
+        info = raw.decode('gb2312')
+        return info
+    except:
+        try:
+            info = raw.decode('utf-8')
+            return info
+        except:
+            raise ValueError
+
+
 def tel_login(tn, ip, user, pas, timeout=1, port=23):
     print("Telnet", ip, "...", end="")
     command = "telnet " + ip + " " + str(port)
     try:
         tn.write(command.encode('utf-8') + b'\n')
-        info = tn.read_until(b'Username:', timeout=5)
+        info_raw = tn.read_until(b'Username:', timeout=timeout)
         try:
-            info = info.decode('gb2312')
+            info = decode_tel_info(info_raw)
         except:
-            try:
-                info = info.decode('utf-8')
-            except:
-                print("Decoding error.")
-                tn.close()
-                return -2
-        if "Username" not in info:
-            print("Connection timeout.")
+            print("Decoding error.")
             tn.close()
-            return 0
-        tn.write(user.encode('utf-8') + b'\n')
-        tn.read_until(b'Password:')
-        tn.write(pas.encode('utf-8') + b'\n')
-        info = tn.read_until(b'>', timeout=5)
-        try:
-            info = info.decode('gb2312')
-        except:
-            try:
-                info = info.decode('utf-8')
-            except:
-                print("Decoding error.")
-                tn.close()
-                return -2
-        if ">" not in info:
-            print("Invalid credentials.")
+            return -2
+        if "Username:" not in info and "Password:" not in info:
+            print("Failed.")
             tn.close()
-            return -1
-        host_name = info[info.index("\n"):].strip()[:-1]
-        print("Login successful, device name:", host_name)
-        return [tn, host_name]
+            return 0
+        else:
+            if "Password:" in info:
+                tn.write(pas.encode('utf-8') + b'\n')
+                info_raw = tn.read_until(b'>', timeout=timeout)
+                try:
+                    info = decode_tel_info(info_raw)
+                except:
+                    print("Decoding error.")
+                    tn.close()
+                    return -2
+                if ">" not in info:
+                    print("Invalid credentials.")
+                    tn.close()
+                    return -1
+            if "Username:" in info:
+                tn.write(user.encode('utf-8') + b'\n')
+                info_raw = tn.read_until(b'Password:', timeout=timeout)
+                try:
+                    info = decode_tel_info(info_raw)
+                except:
+                    print("Decoding error.")
+                    tn.close()
+                    return -2
+                if "Password" in info:
+                    tn.write(pas.encode('utf-8') + b'\n')
+                    info_raw = tn.read_until(b'>', timeout=timeout)
+                    try:
+                        info = decode_tel_info(info_raw)
+                    except:
+                        print("Decoding error.")
+                        tn.close()
+                        return -2
+                    if ">" not in info:
+                        print("Invalid credentials.")
+                        tn.close()
+                        return -1
+                else:
+                    print("Failed.")
+                    tn.close()
+                    return 0
+                host_name = info[info.index("\n"):].strip()[:-1]
+                print("Login successful, device name:", host_name)
+                return [tn, host_name]
     except:
         print("Failed.")
         tn.close()
-        return -1
+        return 0
 
 
-def enable(tn, host_name, enpas):
-    # print("Enabling", host_name, "...", end="")
+def enable(tn, host_name, enpas, timeout):
     try:
+        tn.write(b'\n')
         tn.write("enable".encode('utf-8') + b'\n')
-        tn.read_until(b'Password:')
-        tn.write(enpas.encode('utf-8') + b'\n')
-        tn.read_until(bytes(host_name + '#', 'utf8'))
-        # print("Enabled.")
-        return tn
+        info_raw = tn.read_until(b'Password:', timeout=timeout)
+        try:
+            info = decode_tel_info(info_raw)
+        except:
+            tn.close()
+            return -2
+        if "Password:" not in info:
+            tn.close()
+            return 0
+        else:
+            tn.write(enpas.encode('utf-8') + b'\n')
+            info_raw = tn.read_until(bytes(host_name + '#', 'utf8'), timeout=timeout)
+            try:
+                info = decode_tel_info(info_raw)
+            except:
+                tn.close()
+                return -2
+            if host_name+"#" not in info:
+                if "Password:" in info:
+                    tn.close()
+                    return -1
+                else:
+                    tn.close()
+                    return 0
+            else:
+                return tn
     except:
-        # print("Enter enable mode failed.")
         tn.close()
         return 0
 
 
 def lldp_lookup(tn, host_name):
     try:
         # print("Looking for neighbors of", host_name + "...", end="")
```

### Comparing `hallon-0.0.1/hallon/tools.py` & `hallon-0.0.2/hallon/tools.py`

 * *Files identical despite different names*

### Comparing `hallon-0.0.1/hallon/topo.py` & `hallon-0.0.2/hallon/topo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,118 +1,104 @@
-from hallon import exception
 from hallon import switch
-
-
-def run(l, args):
-    from hallon import cli
-    cli.show_welcome(l)
-    main(args)
-
-
-def get_lldp_dict(target):
-    print("123")
+import ipaddress
 
 
 def login_to_core_and_enable(core_ip, core_user, core_pass, timeout, core_port, core_en_pass):
-    # login to core switch
-    tn_ini = switch.core_login(core_ip, core_user, core_pass, 1, core_port)
-    if not tn_ini:
+    tn_ini = switch.core_login(core_ip, core_user, core_pass, timeout, core_port)
+    if type(tn_ini) == int:
         return 0
     else:
         host_name = tn_ini[1]
         tn = tn_ini[0]
 
         # enter enable mode
-        tn = switch.enable(tn, host_name, core_en_pass)
-        if not tn:
+        tn = switch.enable(tn, host_name, core_en_pass, timeout)
+        if type(tn) == int:
             return 0
         else:
             return [tn, host_name]
 
 
 def main(args):
-    from hallon import switch
-
-    lldp_all = {}
-    lldp_search_tree = []
-    lldp_search_tree_history = []
+    # variables
+    lldp_all = {}  # dictionary for lldp info dict of all network nodes
+    lldp_search_tree = []  # pending nodes list
+    lldp_search_tree_history = []  # processed nodes list
+    lldp_search_failed = []  # failed nodes list
 
     # parse arguments
     core_ip = args.core_address
     core_pass = args.core_password.strip()
     core_port = args.core_port
     core_en_pass = args.core_enable_password.strip()
     core_user = args.core_username.strip()
     uni_user = args.unified_username.strip()
     uni_pass = args.unified_password.strip()
     uni_port = args.unified_port
     uni_en_pass = args.unified_enable_password.strip()
+    timeout = args.telnet_timeout
 
+    # initialization
     lldp_search_tree.append(core_ip)
-    lldp_search_tree_history.append(core_ip)
-    tn_obj = login_to_core_and_enable(core_ip, core_user, core_pass, 1, core_port, core_en_pass)
-    if not tn_obj:
-        exit()
-    host_name = tn_obj[1]
-    tn = tn_obj[0]
-
-    # get lldp info of core
-    tn_lldp_obj = switch.lldp_lookup(tn, host_name)
-    if not tn_lldp_obj:
-        exit()
-    tn = tn_lldp_obj[0]
-    switch.disconnect(tn)
-    lldp_dict = tn_lldp_obj[1]
-    lldp_all[core_ip] = lldp_dict
-    if lldp_dict["lldp_num"] > 0:
-        for i in lldp_dict['lldp_detail']:
-            if "Management address" in lldp_dict["lldp_detail"][i]["info"].keys():
-                if lldp_dict["lldp_detail"][i]["info"]["Management address"] not in lldp_search_tree_history:
-                    lldp_search_tree.append(lldp_dict["lldp_detail"][i]["info"]["Management address"])
-    lldp_search_tree.remove(core_ip)
 
-    # start depth-first-search
+    # start dfs algo
     while len(lldp_search_tree) > 0:
         for ip in lldp_search_tree:
             print("Pending:", len(lldp_search_tree))
             print("Archived:", len(lldp_all))
-            print("Failed:", len(lldp_search_tree_history) - len(lldp_all))
+            print("Failed:", len(lldp_search_failed))
             print("Total processed:", len(lldp_search_tree_history))
-            print(lldp_search_tree)
-            print()
-            lldp_search_tree_history.append(ip)
-            tn_obj = login_to_core_and_enable(core_ip, core_user, core_pass, 1, core_port, core_en_pass)
-            if not tn_obj:
-                pass
-            else:
-                tn = tn_obj[0]
-                host_name = tn_obj[1]
-
-                # making telnet connection
-                tn_ini = switch.tel_login(tn, ip, uni_user, uni_pass, 1, uni_port)
-                if not tn_ini:
-                    pass
+            # telnet core switch and enter enable mode
+            tn_obj = login_to_core_and_enable(core_ip, core_user, core_pass, timeout, core_port, core_en_pass)
+            if type(tn_obj) == int:  # failed
+                print("Failed connecting to core switch.")
+                lldp_search_failed.append(ip)
+            else:  # success
+                tn = tn_obj[0]  # telnet obj
+                host_name = tn_obj[1]  # telnet device name
+
+                # start telnet pending nodes
+                if ip == core_ip:
+                    tn_ini = switch.tel_login(tn, ip, core_user, core_pass, timeout, core_port)
+                else:
+                    tn_ini = switch.tel_login(tn, ip, uni_user, uni_pass, timeout, uni_port)
+                if type(tn_ini) == int:
+                    print("Failed connecting to target.")
+                    lldp_search_failed.append(ip)
                 else:
                     tn = tn_ini[0]
                     host_name = tn_ini[1]
-                    tn = switch.enable(tn, host_name, uni_en_pass)
-                    if not tn:
-                        pass
+
+                    # enter enable mode
+                    tn = switch.enable(tn, host_name, uni_en_pass, timeout)
+                    if type(tn) == int:
+                        print("Failed enabling target.")
+                        lldp_search_failed.append(ip)
                     else:
-                        # get lldp info of core
+                        # lldp lookup in target
                         tn_lldp_obj = switch.lldp_lookup(tn, host_name)
-                        if not tn_lldp_obj:
-                            pass
+                        if type(tn_lldp_obj) == int:
+                            exit()
                         else:
                             tn = tn_lldp_obj[0]
-                            switch.disconnect(tn)
                             lldp_dict = tn_lldp_obj[1]
-                            lldp_all[ip] = lldp_dict
-                            if lldp_dict["lldp_num"] > 0:
+
+                            # close current telnet session
+                            switch.disconnect(tn)
+
+                            # detect public domain ip:
+                            if ipaddress.ip_address(ip).is_private:
+                                lldp_all[ip] = lldp_dict
+
+                            # process lldp_dict and update main variables
+                            if lldp_dict["lldp_num"] > 0:  # has neighbors
                                 for i in lldp_dict['lldp_detail']:
-                                    if "Management address" in lldp_dict["lldp_detail"][i]["info"].keys():
+                                    if "Management address" in lldp_dict["lldp_detail"][i]["info"].keys():  # has management ip
                                         if lldp_dict["lldp_detail"][i]["info"]["Management address"] not in lldp_search_tree_history and lldp_dict["lldp_detail"][i]["info"]["Management address"] not in lldp_search_tree:
                                             lldp_search_tree.append(lldp_dict["lldp_detail"][i]["info"]["Management address"])
             lldp_search_tree.remove(ip)
+            lldp_search_tree_history.append(ip)
 
-    # get interface info
-    # tn = switch.show_interface_status(tn, host_name)
+        print("Pending:", len(lldp_search_tree))
+        print("Archived:", len(lldp_all))
+        print("Failed:", len(lldp_search_failed))
+        print("Total processed:", len(lldp_search_tree_history))
```

### Comparing `hallon-0.0.1/hallon.egg-info/PKG-INFO` & `hallon-0.0.2/hallon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hallon
-Version: 0.0.1
+Version: 0.0.2
 Summary: hallon is a package for network debugging
 Home-page: https://github.com/RyanYuanSun/hallon
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
@@ -41,15 +41,15 @@
 ```bash
 pip install hallon
 ```
 
 ## Usage
 ### Generate network topology
 ```shell
-hallon -nt -cadr 47.104.22.0 -cusr admin -cpas ruijie@123 -cprt 63275 -cenpas ruijie@123 -upas ruijie@123 -uprt 23
+hallon -nt -cadr 47.104.22.0 -cusr admin -cpas ruijie@123 -cprt 63275 -cenpas ruijie@123 -upas ruijie@123 -uprt 23 -tt 5
 ```
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/) License
 
 Copyright (c) 2023 Ryan Alloriadonis
```

### Comparing `hallon-0.0.1/setup.py` & `hallon-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readfile(filename):
     with open(filename, 'r+') as f:
         return f.read()
 
 
 setup(
     name="hallon",
-    version="0.0.1",
+    version="0.0.2",
     description="hallon is a package for network debugging",
     long_description=readfile('README.md'),
     long_description_content_type='text/markdown',
     author="Ryan Alloriadonis",
     author_email="yuantai78@gmail.com",
     url="https://github.com/RyanYuanSun/hallon",
     py_modules=['hallon'],
```

