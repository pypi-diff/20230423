# Comparing `tmp/benimang-0.1.9.tar.gz` & `tmp/benimang-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-0.1.9.tar", last modified: Fri Oct 28 09:01:46 2022, max compression
+gzip compressed data, was "benimang-0.2.0.tar", last modified: Sun Apr 23 09:43:26 2023, max compression
```

## Comparing `benimang-0.1.9.tar` & `benimang-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2022-10-28 09:01:46.457092 benimang-0.1.9/
--rw-rw-rw-   0        0        0       29 2022-09-20 03:37:30.000000 benimang-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0      237 2022-10-28 09:01:46.456090 benimang-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-09-20 03:37:30.000000 benimang-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2022-10-28 09:01:46.448090 benimang-0.1.9/beni/
--rw-rw-rw-   0        0        0        0 2022-09-20 06:33:04.000000 benimang-0.1.9/beni/__init__.py
--rw-rw-rw-   0        0        0     6223 2022-09-20 06:33:43.000000 benimang-0.1.9/beni/bbyte.py
--rw-rw-rw-   0        0        0     2284 2022-09-20 06:33:51.000000 benimang-0.1.9/beni/bcache.py
--rw-rw-rw-   0        0        0     5599 2022-09-20 06:35:27.000000 benimang-0.1.9/beni/bcmd.py
--rw-rw-rw-   0        0        0     1906 2022-09-20 03:37:31.000000 benimang-0.1.9/beni/bcolor.py
--rw-rw-rw-   0        0        0     2399 2022-10-27 02:37:37.000000 benimang-0.1.9/beni/bexecute.py
--rw-rw-rw-   0        0        0     2034 2022-09-20 06:35:50.000000 benimang-0.1.9/beni/bfile.py
--rw-rw-rw-   0        0        0     3638 2022-09-20 06:33:02.000000 benimang-0.1.9/beni/bfunc.py
--rw-rw-rw-   0        0        0     4764 2022-10-28 08:51:07.000000 benimang-0.1.9/beni/bhttp.py
--rw-rw-rw-   0        0        0     2277 2022-09-20 06:16:29.000000 benimang-0.1.9/beni/binput.py
--rw-rw-rw-   0        0        0     4564 2022-09-28 06:55:00.000000 benimang-0.1.9/beni/block.py
--rw-rw-rw-   0        0        0     4147 2022-09-20 07:52:06.000000 benimang-0.1.9/beni/blog.py
--rw-rw-rw-   0        0        0     3078 2022-09-20 06:35:50.000000 benimang-0.1.9/beni/bpath.py
--rw-rw-rw-   0        0        0     2418 2022-09-20 06:35:43.000000 benimang-0.1.9/beni/bplaywright.py
--rw-rw-rw-   0        0        0      838 2022-09-20 06:16:57.000000 benimang-0.1.9/beni/bprogress.py
--rw-rw-rw-   0        0        0     3191 2022-10-28 08:51:46.000000 benimang-0.1.9/beni/bqiniu.py
--rw-rw-rw-   0        0        0     5596 2022-09-20 03:37:31.000000 benimang-0.1.9/beni/bsqlite.py
--rw-rw-rw-   0        0        0      896 2022-09-20 06:35:39.000000 benimang-0.1.9/beni/bstorage.py
--rw-rw-rw-   0        0        0     1970 2022-09-20 06:17:21.000000 benimang-0.1.9/beni/btable.py
--rw-rw-rw-   0        0        0     2935 2022-09-20 06:35:27.000000 benimang-0.1.9/beni/btask.py
--rw-rw-rw-   0        0        0      862 2022-09-20 06:35:08.000000 benimang-0.1.9/beni/btime.py
--rw-rw-rw-   0        0        0     1995 2022-10-28 07:34:47.000000 benimang-0.1.9/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2022-10-28 09:01:46.454090 benimang-0.1.9/benimang.egg-info/
--rw-rw-rw-   0        0        0      237 2022-10-28 09:01:46.000000 benimang-0.1.9/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2022-10-28 09:01:46.000000 benimang-0.1.9/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-28 09:01:46.000000 benimang-0.1.9/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2022-10-28 09:01:46.000000 benimang-0.1.9/benimang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2022-10-28 09:01:46.000000 benimang-0.1.9/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      389 2022-10-28 09:01:43.000000 benimang-0.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-10-28 09:01:46.457092 benimang-0.1.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-10-28 09:01:46.455089 benimang-0.1.9/test/
--rw-rw-rw-   0        0        0      604 2022-09-20 06:17:36.000000 benimang-0.1.9/test/test_sample.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:43:26.964404 benimang-0.2.0/
+-rw-rw-rw-   0        0        0       29 2022-09-20 03:37:30.000000 benimang-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      258 2023-04-23 09:43:26.963407 benimang-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-09-20 03:37:30.000000 benimang-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 09:43:26.953405 benimang-0.2.0/beni/
+-rw-rw-rw-   0        0        0        0 2022-09-20 06:33:04.000000 benimang-0.2.0/beni/__init__.py
+-rw-rw-rw-   0        0        0     6223 2022-09-20 06:33:43.000000 benimang-0.2.0/beni/bbyte.py
+-rw-rw-rw-   0        0        0     6312 2023-04-20 08:42:14.000000 benimang-0.2.0/beni/bcache.py
+-rw-rw-rw-   0        0        0    10173 2023-04-23 09:39:10.000000 benimang-0.2.0/beni/bcmd.py
+-rw-rw-rw-   0        0        0     1906 2022-09-20 03:37:31.000000 benimang-0.2.0/beni/bcolor.py
+-rw-rw-rw-   0        0        0     2460 2023-04-20 08:42:43.000000 benimang-0.2.0/beni/bexecute.py
+-rw-rw-rw-   0        0        0     2139 2023-04-21 01:32:03.000000 benimang-0.2.0/beni/bfile.py
+-rw-rw-rw-   0        0        0     5009 2023-04-23 08:32:41.000000 benimang-0.2.0/beni/bfunc.py
+-rw-rw-rw-   0        0        0     5855 2023-04-21 01:32:29.000000 benimang-0.2.0/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2310 2023-04-23 08:04:15.000000 benimang-0.2.0/beni/binput.py
+-rw-rw-rw-   0        0        0     5653 2023-04-20 09:28:08.000000 benimang-0.2.0/beni/block.py
+-rw-rw-rw-   0        0        0     4175 2023-04-21 01:58:47.000000 benimang-0.2.0/beni/blog.py
+-rw-rw-rw-   0        0        0     5585 2023-04-23 08:15:55.000000 benimang-0.2.0/beni/bpath.py
+-rw-rw-rw-   0        0        0     2418 2023-04-21 01:24:20.000000 benimang-0.2.0/beni/bplaywright.py
+-rw-rw-rw-   0        0        0      841 2023-02-27 04:00:30.000000 benimang-0.2.0/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3845 2023-04-23 09:28:40.000000 benimang-0.2.0/beni/bqiniu.py
+-rw-rw-rw-   0        0        0    10553 2023-04-21 01:31:13.000000 benimang-0.2.0/beni/bsqlite.py
+-rw-rw-rw-   0        0        0      859 2023-04-21 02:20:59.000000 benimang-0.2.0/beni/bstorage.py
+-rw-rw-rw-   0        0        0     1974 2022-11-09 09:34:30.000000 benimang-0.2.0/beni/btable.py
+-rw-rw-rw-   0        0        0     2941 2023-04-20 08:53:07.000000 benimang-0.2.0/beni/btask.py
+-rw-rw-rw-   0        0        0     1574 2023-02-28 02:25:16.000000 benimang-0.2.0/beni/btime.py
+-rw-rw-rw-   0        0        0     2397 2023-04-23 07:11:54.000000 benimang-0.2.0/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:43:26.960407 benimang-0.2.0/benimang.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-04-23 09:43:26.000000 benimang-0.2.0/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-04-23 09:43:26.000000 benimang-0.2.0/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 09:43:26.000000 benimang-0.2.0/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-23 09:43:26.000000 benimang-0.2.0/benimang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       93 2023-04-23 09:43:26.000000 benimang-0.2.0/benimang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-23 09:43:26.000000 benimang-0.2.0/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      567 2023-04-23 08:17:41.000000 benimang-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 09:43:26.964404 benimang-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 09:43:26.962407 benimang-0.2.0/test/
+-rw-rw-rw-   0        0        0      638 2023-02-24 01:48:48.000000 benimang-0.2.0/test/test_sample.py
```

### Comparing `benimang-0.1.9/beni/bbyte.py` & `benimang-0.2.0/beni/bbyte.py`

 * *Files identical despite different names*

### Comparing `benimang-0.1.9/beni/bcolor.py` & `benimang-0.2.0/beni/bcolor.py`

 * *Files identical despite different names*

### Comparing `benimang-0.1.9/beni/bexecute.py` & `benimang-0.2.0/beni/bexecute.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any
 
 from beni import bbyte, bpath
 
 
 async def winscp(winscp_exe: Path | str, key_file: str, server: str, cmd_list: list[str], show_cmd: bool = True):
     logFile = bpath.getUser('executeWinScp.log')
-    bpath.remove(logFile)
+    await bpath.remove(logFile)
     ary = [
         'option batch abort',
         'option transfer binary',
         f'open sftp://{server} -privatekey={key_file} -hostkey=*',
     ]
     ary += cmd_list
     ary += [
@@ -22,35 +22,36 @@
     cmd = f'{winscp_exe} /log={logFile} /loglevel=0 /command ' + ' '.join("%s" % x for x in ary)
     if show_cmd:
         print(cmd)
     return await run(cmd)
 
 
 async def runTry(*args: Any, output: str = '', error: str = ''):
-    outputBytes, errorBytes = await runQuiet(*args)
+    outputBytes, errorBytes, _ = await runQuiet(*args)
     if output and output not in bbyte.decode(outputBytes):
         raise Exception(f'命令执行失败: {" ".join([str(x) for x in args])}')
     if error and error not in bbyte.decode(errorBytes):
         raise Exception(f'命令执行失败: {" ".join([str(x) for x in args])}')
 
 
 async def runQuiet(*args: Any):
     proc = await asyncio.create_subprocess_shell(
         ' '.join([str(x) for x in args]),
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
     )
-    return await proc.communicate()
+    return await proc.communicate() + (proc.returncode or 0,)
 
 
 async def run(*args: Any):
     proc = await asyncio.create_subprocess_shell(
         ' '.join([str(x) for x in args]),
     )
-    return await proc.communicate()
+    await proc.communicate()
+    return proc.returncode or 0
 
 # -------------------------------------------------------
 
 # def execute(*pars: str, show_cmd: bool = True, show_output: bool = False, ignore_error: bool = False):
 #     cmd = ' '.join(pars)
 #     if show_cmd:
 #         info(cmd)
```

### Comparing `benimang-0.1.9/beni/bfile.py` & `benimang-0.2.0/beni/bfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,71 +4,75 @@
 import aiofiles
 
 from beni import bfunc, block, bpath
 
 _limit = 50
 
 
-@block.limit(_limit)
+@block.useLimit(_limit)
 async def writeText(file: Path | str, content: str, encoding: str = 'utf8', newline: str = '\n'):
-    if type(file) is not Path:
-        file = bpath.get(file)
-    bpath.make(file.parent)
+    file = bpath.get(file)
+    await bpath.make(file.parent)
     async with aiofiles.open(file, 'w', encoding=encoding, newline=newline) as f:
         return await f.write(content)
 
 
-@block.limit(_limit)
+@block.useLimit(_limit)
 async def writeBytes(file: Path | str, data: bytes):
-    if type(file) is not Path:
-        file = bpath.get(file)
-    bpath.make(file.parent)
+    file = bpath.get(file)
+    await bpath.make(file.parent)
     async with aiofiles.open(file, 'wb') as f:
         return await f.write(data)
 
 
-@block.limit(_limit)
+@block.useLimit(_limit)
 async def writeYaml(file: Path | str, data: Any):
     import yaml
     await writeText(file, yaml.safe_dump(data))
 
 
-@block.limit(_limit)
+@block.useLimit(_limit)
 async def writeJson(file: Path | str, data: Any, mini: bool = True):
     if mini:
         await writeText(file, bfunc.jsonDumpsMini(data))
     else:
         import json
         await writeText(file, json.dumps(data, ensure_ascii=False, sort_keys=True, indent=4))
 
 
-@block.limit(_limit)
+@block.useLimit(_limit)
 async def readText(file: Path | str, encoding: str = 'utf8', newline: str = '\n'):
     async with aiofiles.open(file, 'r', encoding=encoding, newline=newline) as f:
         return await f.read()
 
 
-@block.limit(_limit)
+@block.useLimit(_limit)
 async def readBytes(file: Path | str):
     async with aiofiles.open(file, 'rb') as f:
         return await f.read()
 
 
-@block.limit(_limit)
+@block.useLimit(_limit)
 async def readYaml(file: Path | str):
     import yaml
     return yaml.safe_load(
         await readText(file)
     )
 
 
-@block.limit(_limit)
+@block.useLimit(_limit)
 async def readJson(file: Path | str):
-    import json
-    return json.loads(
+    import orjson
+    return orjson.loads(await readBytes(file))
+
+
+@block.useLimit(_limit)
+async def readToml(file: Path | str):
+    import tomllib
+    return tomllib.loads(
         await readText(file)
     )
 
 
 async def md5File(file: Path | str):
     return bfunc.md5Bytes(
         await readBytes(file)
```

### Comparing `benimang-0.1.9/beni/bhttp.py` & `benimang-0.2.0/beni/bhttp.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 def _makeHttpHeaders(headers: dict[str, Any] | None = None):
     if headers:
         return _httpHeaders | headers
     else:
         return dict(_httpHeaders)
 
 
-@block.limit(_limit)
+@block.useLimit(_limit)
 async def get(
     url: str,
     *,
     headers: dict[str, Any] | None = None,
     timeout: int = 10,
     retry: int | None = None,
 ):
@@ -88,15 +88,15 @@
     timeout: int = 10,
     retry: int | None = None,
 ):
     result = await getBytes(url, headers=headers, timeout=timeout, retry=retry)
     return orjson.loads(result)
 
 
-@block.limit(_limit)
+@block.useLimit(_limit)
 async def post(
     url: str,
     *,
     data: bytes | dict[str, Any] | None = None,
     headers: dict[str, Any] | None = None,
     timeout: int = 10,
     retry: int | None = None,
@@ -116,38 +116,91 @@
                         raise Exception('http get result is empty')
                     return result, response
         except:
             if retry <= 0:
                 raise
 
 
-@block.limit(_limit)
+async def postBytes(
+    url: str,
+    *,
+    data: bytes | dict[str, Any] | None = None,
+    headers: dict[str, Any] | None = None,
+    timeout: int = 10,
+    retry: int | None = None,
+):
+    resultBytes, _ = await post(
+        url,
+        data=data,
+        headers=headers,
+        timeout=timeout,
+        retry=retry,
+    )
+    return resultBytes
+
+
+async def postStr(
+    url: str,
+    *,
+    data: bytes | dict[str, Any] | None = None,
+    headers: dict[str, Any] | None = None,
+    timeout: int = 10,
+    retry: int | None = None,
+):
+    return (await postBytes(
+        url,
+        data=data,
+        headers=headers,
+        timeout=timeout,
+        retry=retry,
+    )).decode()
+
+
+async def postJson(
+    url: str,
+    *,
+    data: bytes | dict[str, Any] | None = None,
+    headers: dict[str, Any] | None = None,
+    timeout: int = 10,
+    retry: int | None = None,
+):
+    return orjson.loads(
+        await postBytes(
+            url,
+            data=data,
+            headers=headers,
+            timeout=timeout,
+            retry=retry,
+        )
+    )
+
+
+@block.useLimit(_limit)
 async def download(url: str, file: Path | str, timeout: int = 300):
     # total_size: int = 0
     # download_size: int = 0
     try:
+        file = bpath.get(file)
         async with aiohttp.ClientSession() as session:
             async with session.get(url, headers=_httpHeaders, timeout=timeout) as response:
-                if type(file) is not Path:
-                    file = bpath.get(file)
-                bpath.make(file.parent)
+                await bpath.make(file.parent)
                 assert response.content_length, '下载内容为空'
                 # total_size = response.content_length
                 async with aiofiles.open(file, 'wb') as f:
                     while True:
                         data = await response.content.read(1024 * 1024)
                         if data:
                             await f.write(data)
                             # download_size += len(data)
                         else:
                             break
         # 注意：因为gzip在内部解压，所以导致对不上
         # assert total_size and total_size == download_size, '下载为文件不完整'
     except:
-        bpath.remove(file)
+        await bpath.remove(file)
         raise
 
 
 def setDefaultRetry(value: int):
     global _defaultRetry
     _defaultRetry = value
```

### Comparing `benimang-0.1.9/beni/binput.py` & `benimang-0.2.0/beni/binput.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-import asyncio
 import getpass
 import random
 from typing import Any, Callable, Coroutine, cast
 
-import aioconsole
-
 from beni import bcolor
 
 
 async def hold(msg: str | None = None, password: bool = False, *exitvalue_list: str):
     msg = msg or '测试暂停，输入exit可以退出'
     msg = f'{msg}: '
     exitvalue_list = exitvalue_list or ('exit',)
     while True:
         if password:
             inputValue = getpass.getpass(msg)
         else:
+            import aioconsole
             inputValue = cast(str, await aioconsole.ainput(msg))
         if (inputValue in exitvalue_list) or ('*' in exitvalue_list):
             return inputValue
 
 
 async def confirm(msg: str = '确认'):
     code = f'{random.randint(1, 999):03}'
@@ -37,14 +35,15 @@
     print('-' * 30)
     print()
     for msg, inputDisplay, _, _ in data:
         if inputDisplay:
             msg += f' [ {_getRemindMsg(inputDisplay)} ]'
         print(msg)
     print()
+    import aioconsole
     while True:
         value = cast(str, await aioconsole.ainput('输入选择：'))
         isMatch = False
         result = None
         for msg, inputDisplay, inputValue, handler in data:
             inputValue = inputValue or inputDisplay or msg
             if type(inputValue) is str:
@@ -52,21 +51,22 @@
             else:
                 try:
                     isMatch = cast(Callable[[str], bool], inputValue)(value)
                 except:
                     pass
             if isMatch:
                 if handler:
-                    result = asyncio.run(handler(value))
+                    result = await handler(value)
                     break
         if isMatch and result is not False:
             return value
 
 
 async def inputCheck(msg: str, check: Callable[[str], Any]):
+    import aioconsole
     while True:
         try:
             value = cast(str, await aioconsole.ainput(f'{msg}：'))
             if check(value):
                 return value
         except:
             pass
```

### Comparing `benimang-0.1.9/beni/blog.py` & `benimang-0.2.0/beni/blog.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import logging
 import re
 from pathlib import Path
 from typing import Any
 
 from colorama import Fore
 
@@ -81,15 +82,15 @@
                 setattr(result, 'write', self._write)
                 return result
 
             def _write(self, msg: str):
                 msg = self._xx.sub('', msg)
                 self._write_func(msg)
 
-        bpath.make(logFile.parent)
+        asyncio.run(bpath.make(logFile.parent))
         fileLoggerHandler = CustomFileHandler(logFile, delay=True)
         fileLoggerHandler.setFormatter(loggerFormatter)
         fileLoggerHandler.setLevel(loggerLevel)
         logger.addHandler(fileLoggerHandler)
 
 
 def debug(msg: Any, wrap: bool = False, *args: Any, **kwargs: Any):
```

### Comparing `benimang-0.1.9/beni/bplaywright.py` & `benimang-0.2.0/beni/bplaywright.py`

 * *Files identical despite different names*

### Comparing `benimang-0.1.9/beni/bprogress.py` & `benimang-0.2.0/beni/bprogress.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 async def run(
     taskList: Sequence[Coroutine[Any, Any, _ReturnType]],
     itemLimit: int = 999999,
 ) -> Sequence[_ReturnType]:
     print()
     with tqdm(total=len(taskList), ncols=70) as progress:
-        @block.limit(itemLimit)
+        @block.useLimit(itemLimit)
         async def task(x: Coroutine[Any, Any, _ReturnType]):
             result = await x
             progress.update()
             return result
         resultList = await asyncio.gather(*[task(x) for x in taskList])
     print()
     return resultList
```

### Comparing `benimang-0.1.9/beni/bsqlite.py` & `benimang-0.2.0/beni/block.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,174 +1,187 @@
-from __future__ import annotations
-
-import asyncio
-import sqlite3
-from contextlib import asynccontextmanager
-from pathlib import Path
-from typing import Any, Iterable, Sequence, cast
-
-import aiosqlite
-
-sqlite3.register_converter(
-    "bool",
-    lambda x: x not in (
-        b'',
-        b'0',
-        # None, # 如果是None根本就不会进来，这里判断也没有意义
-    )
-)
-
-
-class SqliteDbPool():
-
-    def __init__(self, db_file: str | Path, count: int = 9):
-        self._avaliable_list: asyncio.Queue[_SqliteDbRead] = asyncio.Queue()
-        self._using_list: list[_SqliteDbRead] = []
-        self._readlock_list: list[asyncio.Lock] = []
-        self._dbwrite: _SqliteDbWrite | None = None
-        self._writelock = asyncio.Lock()
-        self._db_file = db_file
-        self._count = count
-
-    async def close(self):
-        while self._using_list or not self._avaliable_list.empty():
-            xx = await self._avaliable_list.get()
-            await xx.close()
-        await self._writelock.acquire()
-        if self._dbwrite:
-            await self._dbwrite.close()
-        self._writelock.release()
-
-    async def _getDbRead(self):
-        if len(self._using_list) < self._count:
-            if self._avaliable_list.empty():
-                db = _SqliteDbRead()
-                await db.connect(self._db_file)
-            else:
-                db = self._avaliable_list.get_nowait()
-        else:
-            db = await self._avaliable_list.get()
-        self._using_list.append(db)
-        return db
-
-    def _releaseDbRead(self, db: _SqliteDbRead):
-        self._using_list.remove(db)
-        self._avaliable_list.put_nowait(db)
-
-    @asynccontextmanager
-    async def read(self):
-        lock = asyncio.Lock()
-        await lock.acquire()
-        db = await self._getDbRead()
-        if self._writelock.locked():
-            await self._writelock.acquire()
-            self._readlock_list.append(lock)
-            self._writelock.release()
-        else:
-            self._readlock_list.append(lock)
-        try:
-            yield db
-        finally:
-            self._releaseDbRead(db)
-            self._readlock_list.remove(lock)
-            lock.release()
-
-    @asynccontextmanager
-    async def write(self):
-        await self._writelock.acquire()
-        while self._readlock_list:
-            lock = self._readlock_list[0]
-            await lock.acquire()
-            lock.release()
-        if not self._dbwrite:
-            self._dbwrite = _SqliteDbWrite()
-            await self._dbwrite.connect(self._db_file)
-        db = self._dbwrite
-        try:
-            yield db
-            await db.commit()
-        except:
-            await db.rollback()
-            raise
-        finally:
-            self._writelock.release()
-
-
-class _SqliteDbRead():
-
-    _db: aiosqlite.Connection
-
-    async def connect(self, db_file: Path | str):
-        self._db = await aiosqlite.connect(db_file, detect_types=sqlite3.PARSE_DECLTYPES)
-        self._db.row_factory = sqlite3.Row
-
-    async def fetchAll(self, sql: str, parameters: Iterable[Any] | None = None):
-        async with self._db.execute(sql, parameters) as cursor:
-            return cast(list[sqlite3.Row], await cursor.fetchall())
-
-    async def fetchOne(self, sql: str, parameters: Iterable[Any] | None = None):
-        async with self._db.execute(sql, parameters) as cursor:
-            return await cursor.fetchone()
-
-    async def close(self):
-        await self._db.close()
-
-
-class _SqliteDbWrite(_SqliteDbRead):
-
-    async def insert(self, table: str, data: dict[str, Any]):
-        keylist = sorted(data.keys())
-        fieldname_list = ','.join([f'"{x}"' for x in keylist])
-        placement_list = ','.join(['?' for _ in range(len(keylist))])
-        fieldvalue_list = [data[x] for x in keylist]
-        async with self._db.execute(
-            f'''
-            INSERT INTO "{table}" ({fieldname_list}) 
-            VALUES 
-                ({placement_list});
-            ''',
-            fieldvalue_list,
-        ) as cursor:
-            return cursor.lastrowid
-
-    async def insertMany(self, table: str, dataList: Sequence[dict[str, Any]]):
-        keyset: set[str] = set()
-        for data in dataList:
-            keyset.update(data.keys())
-        keylist = sorted(keyset)
-        fieldname_list = ','.join([f'`{x}`' for x in keylist])
-        placement_list = ','.join(['?' for _ in range(len(keylist))])
-        fieldvalue_list = [[data.get(key) for key in keylist] for data in dataList]
-        async with self._db.executemany(
-            f'''
-            INSERT INTO "{table}" ({fieldname_list}) 
-            VALUES 
-                ({placement_list});
-            ''',
-            fieldvalue_list
-        ) as _cursor:
-            pass
-
-    async def insertOrReplace(self, table: str, data: dict[str, Any]):
-        keylist = sorted(data.keys())
-        fieldname_list = ','.join([f'"{x}"' for x in keylist])
-        placement_list = ','.join(['?' for _ in range(len(keylist))])
-        fieldvalue_list = [data[x] for x in keylist]
-        async with self._db.execute(
-            f'''
-            INSERT OR REPLACE INTO "{table}" ({fieldname_list}) 
-            VALUES 
-                ({placement_list});
-            ''',
-            fieldvalue_list,
-        ) as _cursor:
-            pass
-
-    async def execute(self, sql: str, parameters: Iterable[Any] | None = None):
-        async with self._db.execute(sql, parameters) as cursor:
-            return cursor.rowcount
-
-    async def commit(self):
-        await self._db.commit()
-
-    async def rollback(self):
-        await self._db.rollback()
+from __future__ import annotations
+
+import asyncio
+import inspect
+from contextlib import asynccontextmanager
+from functools import wraps
+from pathlib import Path
+from typing import Any, Callable, cast
+
+from beni import bfunc, binput, bpath
+
+
+@asynccontextmanager
+async def useFileLock(*keys: str, timeout: float = 0, quite: bool = False):
+    import portalocker
+    lock_list: list[portalocker.Lock] = []
+    keyfile_list: list[Path] = []
+    for key in keys:
+        lock, keyfile = await _lock_acquire(key, timeout, quite)
+        lock_list.append(lock)
+        keyfile_list.append(keyfile)
+    try:
+        yield
+    finally:
+        for lock in lock_list:
+            lock.release()
+        for keyfile in keyfile_list:
+            try:
+                await bpath.remove(keyfile)
+            except:
+                pass
+
+
+async def _lock_acquire(key: str, timeout: float = 0, quite: bool = False):
+    '''不对外部提供，只提供给 async_keylock 方法使用'''
+    keyfile = bpath.getWorkspace(f'.lock/{bfunc.crcStr(key)}.lock')
+    await bpath.make(keyfile.parent)
+    import portalocker
+    while True:
+        try:
+            lock = portalocker.Lock(keyfile, timeout=timeout, fail_when_locked=timeout == 0)
+            f = lock.acquire()
+            f.write(key)
+            f.flush()
+            break
+        except:
+            if quite:
+                raise Exception(f'资源被锁定无法继续操作 key={key} keyfile={keyfile}')
+            else:
+                async def __retry(_):
+                    print('正在重试...')
+
+                async def __exit(_):
+                    raise Exception(f'资源被锁定无法继续操作 - {key}')
+
+                asyncio.run(
+                    binput.select(
+                        ('重试', 'retry', None, __retry),
+                        ('退出', 'exit', None, __exit),
+                    )
+                )
+    return lock, keyfile
+
+
+# ------------------------------------------------------------------------------------------------------------------------
+
+
+def useLimit(limit: int = 1):
+    def wraperfun(func: bfunc.AsyncFun) -> bfunc.AsyncFun:
+        @wraps(func)
+        async def wraper(*args: Any, **kwargs: Any):
+            funid = id(inspect.unwrap(func))
+            if funid not in _limit_dict:
+                _limit_dict[funid] = _Limit(limit)
+            try:
+                await _limit_dict[funid].wait()
+                return await func(*args, **kwargs)
+            finally:
+                await _limit_dict[funid].release()
+        return cast(Any, wraper)
+    return wraperfun
+
+
+async def setLimit(func: Callable[..., Any], limit: int):
+    funid = id(inspect.unwrap(func))
+    if funid not in _limit_dict:
+        _limit_dict[funid] = _Limit(limit)
+    await _limit_dict[funid].set_limit(limit)
+
+
+_limit_dict: dict[int, _Limit] = {}
+
+
+class _Limit():
+
+    _queue: asyncio.Queue[Any]
+    _running: int
+
+    def __init__(self, limit: int):
+        self._limit = limit
+        self._queue = asyncio.Queue()
+        self._running = 0
+        while self._queue.qsize() < self._limit:
+            self._queue.put_nowait(True)
+
+    async def wait(self):
+        await self._queue.get()
+        self._running += 1
+
+    async def release(self):
+        if self._queue.qsize() < self._limit:
+            await self._queue.put(True)
+        self._running -= 1
+
+    async def set_limit(self, limit: int):
+        self._limit = limit
+        while self._running + self._queue.qsize() < self._limit:
+            await self._queue.put(True)
+        while self._running + self._queue.qsize() > self._limit:
+            if self._queue.empty():
+                break
+            await self._queue.get()
+
+
+# ------------------------------------------------------------------------------------------------------------------------
+
+
+class RWLock():
+
+    def __init__(self, maxNum: int) -> None:
+        self._maxNum = maxNum
+        self._readNum = 0
+        self._writeNum = 0
+        self._onReadFinished = asyncio.Event()
+        self._onWriteFinished = asyncio.Event()
+
+    def _getNum(self):
+        return self._readNum + self._writeNum
+
+    async def getRead(self):
+        while True:
+            if self._writeNum:
+                self._onWriteFinished.clear()
+                await self._onWriteFinished.wait()
+            elif self._getNum() >= self._maxNum:
+                self._onReadFinished.clear()
+                await self._onReadFinished.wait()
+            else:
+                self._readNum += 1
+                break
+
+    def releaseRead(self):
+        self._readNum -= 1
+        if not self._readNum:
+            self._onReadFinished.set()
+
+    @asynccontextmanager
+    async def useRead(self):
+        await self.getRead()
+        try:
+            yield
+        finally:
+            self.releaseRead()
+
+    async def getWrite(self):
+        while True:
+            if self._readNum:
+                self._onReadFinished.clear()
+                await self._onReadFinished.wait()
+            elif self._writeNum:
+                self._onWriteFinished.clear()
+                await self._onWriteFinished.wait()
+            else:
+                self._writeNum += 1
+                break
+
+    def releaseWrite(self):
+        self._writeNum -= 1
+        self._onWriteFinished.set()
+
+    @asynccontextmanager
+    async def useWrite(self):
+        await self.getWrite()
+        try:
+            yield
+        finally:
+            self.releaseWrite()
```

### Comparing `benimang-0.1.9/beni/bstorage.py` & `benimang-0.2.0/beni/bstorage.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,22 +13,21 @@
 
 async def set(key: str, value: Any):
     storageFile = _getStorageFile(key)
     await bfile.writeYaml(storageFile, value)
 
 
 async def clear(*keyList: str):
-    for key in keyList:
-        storageFile = _getStorageFile(key)
-        bpath.remove(storageFile)
+    await bpath.remove(*[_getStorageFile(key) for key in keyList])
 
 
 async def clearAll():
-    for storageFile in bpath.listFile(_storagePath):
-        bpath.remove(storageFile)
+    fileList = await bpath.listFile(_storagePath)
+    await bpath.remove(*fileList)
+
 
 # ------------------------------------------------------------------------------------------
 
 _storagePath: Final = bpath.getWorkspace('.storage')
 
 
 def _getStorageFile(key: str):
```

### Comparing `benimang-0.1.9/beni/btable.py` & `benimang-0.2.0/beni/btable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Any, Callable, Final, Sequence, Tuple, TypeVar
 
 import colorama
-from prettytable import PrettyTable
 
 from beni import bcolor
 
 _T = TypeVar('_T')
 
 
 def get(
@@ -14,14 +13,15 @@
     title: str | None = None,
     fields: Sequence[Tuple[str, Callable[[_T], Any]]],
     rowcolor: Callable[[list[Any]], Any] | None = None,
     extend: list[list[Any]] | None = None,
     isPrint: bool = False,
 ):
     header_color: Final = colorama.Fore.YELLOW
+    from prettytable import PrettyTable
     table = PrettyTable()
     if title:
         table.title = bcolor.getStr(title, header_color)
     field_funclist: list[Callable[[_T], Any]] = []
     field_namelist: list[str] = []
     align_dict: dict[str, str] = {}
     for i in range(len(fields)):
```

### Comparing `benimang-0.1.9/beni/btask.py` & `benimang-0.2.0/beni/btask.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         try:
             if _logFile:
                 logfile_list = list(_logFile.parent.glob('*.log'))
                 logfile_list.remove(_logFile)
                 logfile_list.sort(key=lambda x: x.stat().st_ctime, reverse=True)
                 logfile_list = logfile_list[_HOLD_LOGFILE_COUNT:]
                 for logfile in logfile_list:
-                    bpath.remove(logfile)
+                    await bpath.remove(logfile)
         except:
             pass
 
 
 def setLogPath(logpath: Path):
     if _startTime:
         blog.warning('task.setLogDir 必须在任务启动前调用，本次忽略执行')
```

### Comparing `benimang-0.1.9/beni/bzip.py` & `benimang-0.2.0/beni/bzip.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,66 @@
 from pathlib import Path
 from typing import Any, Callable
 from zipfile import ZIP_DEFLATED, ZipFile
 
-from beni import bpath, bexecute
+from beni import bexecute, bpath
 
 
-def zipFile(to_file: Path | str, path_dict: dict[str, Path]):
-    if type(to_file) is not Path:
-        to_file = bpath.get(to_file)
-    bpath.make(to_file.parent)
-    with ZipFile(to_file, 'w', ZIP_DEFLATED) as f:
+async def _zip(zfile: Path, path_dict: dict[str, Path]):
+    await bpath.make(zfile.parent)
+    with ZipFile(zfile, 'w', ZIP_DEFLATED) as f:
         for fname in sorted(path_dict.keys()):
             file = path_dict[fname]
             if file.is_file():
                 f.write(file, fname)
 
 
-def zipFolder(to_file: Path | str, dir: Path, filter_func: Callable[[Path], bool] | None = None):
-    ary = bpath.listPath(dir, True)
-    if filter_func:
-        ary = list(filter(filter_func, ary))
-    zipFile(to_file, {str(x.relative_to(dir)): x for x in ary})
-
-
-def extract(file: Path | str, to_dir: Path | str | None = None):
-    if type(file) is not Path:
-        file = bpath.get(file)
-    to_dir = to_dir or file.parent
+async def zipFile(zfile: Path | str, targetFile: Path | str, name: str | None = None):
+    zfile = bpath.get(zfile)
+    targetFile = bpath.get(targetFile)
+    if name is None:
+        name = targetFile.name
+    await _zip(zfile, {name: targetFile})
+
+
+async def zipFolder(zfile: Path | str, targetDir: Path | str, filterFunc: Callable[[Path], bool] | None = None):
+    zfile = bpath.get(zfile)
+    targetDir = bpath.get(targetDir)
+    ary = await bpath.listPath(targetDir, True)
+    if filterFunc:
+        ary = list(filter(filterFunc, ary))
+    await _zip(zfile, {str(x.relative_to(targetDir)): x for x in ary})
+
+
+async def unzip(file: Path | str, outputDir: Path | str | None = None):
+    file = bpath.get(file)
+    outputDir = outputDir or file.parent
     with ZipFile(file) as f:
         for subFile in sorted(f.namelist()):
             try:
                 # zipfile 代码中指定了cp437，这里会导致中文乱码
                 encodeSubFile = subFile.encode('cp437').decode('gbk')
             except:
                 encodeSubFile = subFile
-            f.extract(subFile, to_dir)
+            f.extract(subFile, outputDir)
             # 处理压缩包中的中文文件名在windows下乱码
             if subFile != encodeSubFile:
-                toFile = bpath.get(to_dir, encodeSubFile)
-                bpath.get(to_dir, subFile).rename(toFile)
+                toFile = bpath.get(outputDir, encodeSubFile)
+                bpath.get(outputDir, subFile).rename(toFile)
 
 
 async def sevenZip(zfile: Path | str, target: Path | str):
-    await _runSeven('7zr', 'a', zfile, target)
+    await _runSeven('a', zfile, target)
 
 
 async def sevenUnzip(zfile: Path | str, output: Path | str):
-    await _runSeven('7zr', 'x', f'-o{output}', zfile)
+    await _runSeven('x', f'-o{output}', zfile)
+
+
+async def sevenRename(zfile: Path | str, fromName: str, toName: str):
+    await _runSeven('rn', zfile, fromName, toName)
 
 
 async def _runSeven(*parList: Any):
-    resultBytes, errorBytes = await bexecute.runQuiet(*parList)
-    assert not errorBytes, errorBytes.decode()
-    assert b'Everything is Ok' in resultBytes, resultBytes.decode()
+    resultBytes, errorBytes, _ = await bexecute.runQuiet('7zr', *parList)
+    assert not errorBytes, errorBytes.decode('gbk')
+    assert b'Everything is Ok' in resultBytes, resultBytes.decode('gbk')
```

### Comparing `benimang-0.1.9/benimang.egg-info/SOURCES.txt` & `benimang-0.2.0/benimang.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 beni/btask.py
 beni/btime.py
 beni/bzip.py
 benimang.egg-info/PKG-INFO
 benimang.egg-info/SOURCES.txt
 benimang.egg-info/dependency_links.txt
 benimang.egg-info/entry_points.txt
+benimang.egg-info/requires.txt
 benimang.egg-info/top_level.txt
 test/test_sample.py
```

### Comparing `benimang-0.1.9/test/test_sample.py` & `benimang-0.2.0/test/test_sample.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-00000000: 2727 270d 0a0d 0ae5 bfab e68d b7e9 94ae  '''.............
-00000010: efbc 88e9 bb98 e8ae a4ef bc89 0d0a 4354  ..............CT
-00000020: 524c 2b3b 2041 2020 2020 2020 2020 e689  RL+; A        ..
-00000030: a7e8 a18c e585 a8e9 83a8 e58d 95e5 8583  ................
-00000040: e6b5 8be8 af95 0d0a 4354 524c 2b3b 2045  ........CTRL+; E
-00000050: 2020 2020 2020 2020 e58f aae6 89a7 e8a1          ........
-00000060: 8ce4 b88a e6ac a1e5 87ba e994 99e7 9a84  ................
-00000070: e794 a8e4 be8b 0d0a 4354 524c 2b3b 2043  ........CTRL+; C
-00000080: 2020 2020 2020 2020 e6b8 85e9 99a4 e7bb          ........
-00000090: 93e6 9e9c 0d0a 4354 524c 2b3b 2043 5452  ......CTRL+; CTR
-000000a0: 4c2b 4120 2020 e8b0 83e8 af95 e585 a8e9  L+A   ..........
-000000b0: 83a8 e58d 95e5 8583 e6b5 8be8 af95 0d0a  ................
-000000c0: 4354 524c 2b3b 2043 5452 4c2b 4520 2020  CTRL+; CTRL+E   
-000000d0: e58f aae8 b083 e8af 95e4 b88a e6ac a1e5  ................
-000000e0: 87ba e994 99e7 9a84 e794 a8e4 be8b 0d0a  ................
-000000f0: 0d0a 2727 270d 0a0d 0a23 20e5 9fba e7a1  ..'''....# .....
-00000100: 80e7 94a8 e6b3 9520 2d2d 2d2d 2d2d 2d2d  ....... --------
-00000110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000000: 2320 2727 270d 0a0d 0a23 20e5 bfab e68d  # '''....# .....
+00000010: b7e9 94ae efbc 88e9 bb98 e8ae a4ef bc89  ................
+00000020: 0d0a 2320 4354 524c 2b3b 2041 2020 2020  ..# CTRL+; A    
+00000030: 2020 2020 e689 a7e8 a18c e585 a8e9 83a8      ............
+00000040: e58d 95e5 8583 e6b5 8be8 af95 0d0a 2320  ..............# 
+00000050: 4354 524c 2b3b 2045 2020 2020 2020 2020  CTRL+; E        
+00000060: e58f aae6 89a7 e8a1 8ce4 b88a e6ac a1e5  ................
+00000070: 87ba e994 99e7 9a84 e794 a8e4 be8b 0d0a  ................
+00000080: 2320 4354 524c 2b3b 2043 2020 2020 2020  # CTRL+; C      
+00000090: 2020 e6b8 85e9 99a4 e7bb 93e6 9e9c 0d0a    ..............
+000000a0: 2320 4354 524c 2b3b 2043 5452 4c2b 4120  # CTRL+; CTRL+A 
+000000b0: 2020 e8b0 83e8 af95 e585 a8e9 83a8 e58d    ..............
+000000c0: 95e5 8583 e6b5 8be8 af95 0d0a 2320 4354  ............# CT
+000000d0: 524c 2b3b 2043 5452 4c2b 4520 2020 e58f  RL+; CTRL+E   ..
+000000e0: aae8 b083 e8af 95e4 b88a e6ac a1e5 87ba  ................
+000000f0: e994 99e7 9a84 e794 a8e4 be8b 0d0a 0d0a  ................
+00000100: 2320 2727 270d 0a0d 0a23 2023 20e5 9fba  # '''....# # ...
+00000110: e7a1 80e7 94a8 e6b3 9520 2d2d 2d2d 2d2d  ......... ------
 00000120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d  ---------------.
-00000150: 0a0d 0a69 6d70 6f72 7420 7079 7465 7374  ...import pytest
-00000160: 0d0a 6672 6f6d 2062 656e 6920 696d 706f  ..from beni impo
-00000170: 7274 2062 6874 7470 0d0a 0d0a 0d0a 6465  rt bhttp......de
-00000180: 6620 7465 7374 5f70 7269 6e74 2829 3a0d  f test_print():.
-00000190: 0a20 2020 2070 7269 6e74 2831 3233 290d  .    print(123).
-000001a0: 0a0d 0a0d 0a40 7079 7465 7374 2e6d 6172  .....@pytest.mar
-000001b0: 6b2e 6173 796e 6369 6f0d 0a61 7379 6e63  k.asyncio..async
-000001c0: 2064 6566 2074 6573 745f 6874 7470 4765   def test_httpGe
-000001d0: 7428 293a 0d0a 2020 2020 7265 7375 6c74  t():..    result
-000001e0: 2c20 5f20 3d20 6177 6169 7420 6268 7474  , _ = await bhtt
-000001f0: 702e 6765 7428 2768 7474 7073 3a2f 2f77  p.get('https://w
-00000200: 7777 2e62 6169 6475 2e63 6f6d 2729 0d0a  ww.baidu.com')..
-00000210: 2020 2020 6173 7365 7274 2027 3c74 6974      assert '<tit
-00000220: 6c65 3ee7 99be e5ba a6e4 b880 e4b8 8bef  le>.............
-00000230: bc8c e4bd a0e5 b0b1 e79f a5e9 8193 3c2f  ..............</
-00000240: 7469 746c 653e 2720 696e 2072 6573 756c  title>' in resul
-00000250: 742e 6465 636f 6465 2829 0d0a            t.decode()..
+00000140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000160: 2d0d 0a0d 0a23 2069 6d70 6f72 7420 7079  -....# import py
+00000170: 7465 7374 0d0a 2320 6672 6f6d 2062 656e  test..# from ben
+00000180: 6920 696d 706f 7274 2062 6874 7470 0d0a  i import bhttp..
+00000190: 0d0a 0d0a 2320 6465 6620 7465 7374 5f70  ....# def test_p
+000001a0: 7269 6e74 2829 3a0d 0a23 2020 2020 2070  rint():..#     p
+000001b0: 7269 6e74 2831 3233 290d 0a0d 0a0d 0a23  rint(123)......#
+000001c0: 2040 7079 7465 7374 2e6d 6172 6b2e 6173   @pytest.mark.as
+000001d0: 796e 6369 6f0d 0a23 2061 7379 6e63 2064  yncio..# async d
+000001e0: 6566 2074 6573 745f 6874 7470 4765 7428  ef test_httpGet(
+000001f0: 293a 0d0a 2320 2020 2020 7265 7375 6c74  ):..#     result
+00000200: 2c20 5f20 3d20 6177 6169 7420 6268 7474  , _ = await bhtt
+00000210: 702e 6765 7428 2768 7474 7073 3a2f 2f77  p.get('https://w
+00000220: 7777 2e62 6169 6475 2e63 6f6d 2729 0d0a  ww.baidu.com')..
+00000230: 2320 2020 2020 6173 7365 7274 2027 3c74  #     assert '<t
+00000240: 6974 6c65 3ee7 99be e5ba a6e4 b880 e4b8  itle>...........
+00000250: 8bef bc8c e4bd a0e5 b0b1 e79f a5e9 8193  ................
+00000260: 3c2f 7469 746c 653e 2720 696e 2072 6573  </title>' in res
+00000270: 756c 742e 6465 636f 6465 2829 0d0a       ult.decode()..
```

