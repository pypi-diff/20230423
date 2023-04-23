# Comparing `tmp/mcqq-tool-0.0.3.tar.gz` & `tmp/mcqq-tool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcqq-tool-0.0.3.tar", last modified: Sun Apr 23 06:40:51 2023, max compression
+gzip compressed data, was "mcqq-tool-0.0.4.tar", last modified: Sun Apr 23 07:27:50 2023, max compression
```

## Comparing `mcqq-tool-0.0.3.tar` & `mcqq-tool-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 06:40:51.572990 mcqq-tool-0.0.3/
--rw-rw-rw-   0        0        0    35184 2023-04-21 09:49:28.000000 mcqq-tool-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      511 2023-04-23 06:40:51.572481 mcqq-tool-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       82 2023-04-21 08:06:01.000000 mcqq-tool-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 06:40:51.565647 mcqq-tool-0.0.3/mcqq_tool/
--rw-rw-rw-   0        0        0       33 2023-04-22 04:16:51.000000 mcqq-tool-0.0.3/mcqq_tool/__init__.py
--rw-rw-rw-   0        0        0     4283 2023-04-23 06:09:58.000000 mcqq-tool-0.0.3/mcqq_tool/common.py
--rw-rw-rw-   0        0        0     1873 2023-04-23 06:00:48.000000 mcqq-tool-0.0.3/mcqq_tool/config.py
-drwxrwxrwx   0        0        0        0 2023-04-23 06:40:51.571400 mcqq-tool-0.0.3/mcqq_tool/model/
--rw-rw-rw-   0        0        0      597 2023-04-21 08:09:17.000000 mcqq-tool-0.0.3/mcqq_tool/model/__init__.py
--rw-rw-rw-   0        0        0     1041 2023-04-21 08:09:17.000000 mcqq-tool-0.0.3/mcqq_tool/model/basemodel.py
--rw-rw-rw-   0        0        0      640 2023-04-21 08:09:17.000000 mcqq-tool-0.0.3/mcqq_tool/model/minecraft.py
--rw-rw-rw-   0        0        0     1389 2023-04-21 08:09:17.000000 mcqq-tool-0.0.3/mcqq_tool/model/spigot.py
--rw-rw-rw-   0        0        0    13352 2023-04-23 06:28:43.000000 mcqq-tool-0.0.3/mcqq_tool/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-23 06:40:51.569398 mcqq-tool-0.0.3/mcqq_tool.egg-info/
--rw-rw-rw-   0        0        0      511 2023-04-23 06:40:51.000000 mcqq-tool-0.0.3/mcqq_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-23 06:40:51.000000 mcqq-tool-0.0.3/mcqq_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 06:40:51.000000 mcqq-tool-0.0.3/mcqq_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-04-23 06:40:51.000000 mcqq-tool-0.0.3/mcqq_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-23 06:40:51.000000 mcqq-tool-0.0.3/mcqq_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 06:40:51.572990 mcqq-tool-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-04-23 06:37:23.000000 mcqq-tool-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:27:50.139073 mcqq-tool-0.0.4/
+-rw-rw-rw-   0        0        0    35184 2023-04-21 09:49:28.000000 mcqq-tool-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      511 2023-04-23 07:27:50.139073 mcqq-tool-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2023-04-21 08:06:01.000000 mcqq-tool-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 07:27:50.131065 mcqq-tool-0.0.4/mcqq_tool/
+-rw-rw-rw-   0        0        0       33 2023-04-22 04:16:51.000000 mcqq-tool-0.0.4/mcqq_tool/__init__.py
+-rw-rw-rw-   0        0        0     4283 2023-04-23 06:09:58.000000 mcqq-tool-0.0.4/mcqq_tool/common.py
+-rw-rw-rw-   0        0        0     1879 2023-04-23 07:27:30.000000 mcqq-tool-0.0.4/mcqq_tool/config.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:27:50.137071 mcqq-tool-0.0.4/mcqq_tool/model/
+-rw-rw-rw-   0        0        0      597 2023-04-21 08:09:17.000000 mcqq-tool-0.0.4/mcqq_tool/model/__init__.py
+-rw-rw-rw-   0        0        0     1041 2023-04-21 08:09:17.000000 mcqq-tool-0.0.4/mcqq_tool/model/basemodel.py
+-rw-rw-rw-   0        0        0      640 2023-04-21 08:09:17.000000 mcqq-tool-0.0.4/mcqq_tool/model/minecraft.py
+-rw-rw-rw-   0        0        0     1389 2023-04-21 08:09:17.000000 mcqq-tool-0.0.4/mcqq_tool/model/spigot.py
+-rw-rw-rw-   0        0        0    13352 2023-04-23 06:28:43.000000 mcqq-tool-0.0.4/mcqq_tool/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:27:50.134068 mcqq-tool-0.0.4/mcqq_tool.egg-info/
+-rw-rw-rw-   0        0        0      511 2023-04-23 07:27:50.000000 mcqq-tool-0.0.4/mcqq_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-04-23 07:27:50.000000 mcqq-tool-0.0.4/mcqq_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 07:27:50.000000 mcqq-tool-0.0.4/mcqq_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-04-23 07:27:50.000000 mcqq-tool-0.0.4/mcqq_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 07:27:50.000000 mcqq-tool-0.0.4/mcqq_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 07:27:50.139073 mcqq-tool-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-04-23 07:27:38.000000 mcqq-tool-0.0.4/setup.py
```

### Comparing `mcqq-tool-0.0.3/LICENSE` & `mcqq-tool-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.3/mcqq_tool/common.py` & `mcqq-tool-0.0.4/mcqq_tool/common.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.3/mcqq_tool/config.py` & `mcqq-tool-0.0.4/mcqq_tool/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,8 +56,8 @@
     # 服务器列表
     mc_qq_server_list: Optional[List[Server]] = Field(default_factory=list)
     # MCRcon 密码
     mc_qq_rcon_password: Optional[str] = "password"
     # Rcon 字典
     mc_qq_rcon_dict: Optional[Dict[str, int]] = Field(default_factory=dict)
     # MC_QQ 频道管理员身份组
-    mc_qq_guild_admin_roles: Optional[List[str]] = ["频道主", "管理员"]
+    mc_qq_guild_admin_roles: Optional[List[str]] = ["频道主", "超级管理员"]
```

### Comparing `mcqq-tool-0.0.3/mcqq_tool/model/__init__.py` & `mcqq-tool-0.0.4/mcqq_tool/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.3/mcqq_tool/model/basemodel.py` & `mcqq-tool-0.0.4/mcqq_tool/model/basemodel.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.3/mcqq_tool/model/minecraft.py` & `mcqq-tool-0.0.4/mcqq_tool/model/minecraft.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.3/mcqq_tool/model/spigot.py` & `mcqq-tool-0.0.4/mcqq_tool/model/spigot.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.3/mcqq_tool/utils.py` & `mcqq-tool-0.0.4/mcqq_tool/utils.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.3/setup.py` & `mcqq-tool-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="mcqq-tool",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.3",  # 程序版本
+    version="0.0.4",  # 程序版本
     author="17TheWord",  # 项目作者
     author_email="17theword@gmail.com",  # 作者邮件
     description="MC_QQ 工具包",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/17TheWord/mcqq-tool",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

