# Comparing `tmp/bgmi-5.0.0a2.tar.gz` & `tmp/bgmi-5.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgmi-5.0.0a2.tar", max compression
+gzip compressed data, was "bgmi-5.0.0a3.tar", max compression
```

## Comparing `bgmi-5.0.0a2.tar` & `bgmi-5.0.0a3.tar`

### file list

```diff
@@ -1,44 +1,42 @@
--rw-r--r--   0        0        0     1117 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/LICENSE
--rw-r--r--   0        0        0    14399 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/README.md
--rw-r--r--   0        0        0      176 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/__init__.py
--rw-r--r--   0        0        0       35 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/__main__.py
--rw-r--r--   0        0        0     6523 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/config.py
--rw-r--r--   0        0        0      240 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/downloader/__init__.py
--rw-r--r--   0        0        0     1862 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/downloader/aria2_rpc.py
--rw-r--r--   0        0        0     1558 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/downloader/deluge.py
--rw-r--r--   0        0        0     1752 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/downloader/qbittorrent.py
--rw-r--r--   0        0        0     1225 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/downloader/transmission.py
--rw-r--r--   0        0        0        0 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/front/__init__.py
--rw-r--r--   0        0        0     3230 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/front/admin.py
--rw-r--r--   0        0        0     2848 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/front/base.py
--rw-r--r--   0        0        0     2865 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/front/index.py
--rw-r--r--   0        0        0     3410 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/front/resources.py
--rw-r--r--   0        0        0     2272 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/front/server.py
--rw-r--r--   0        0        0      467 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/front/templates/download.xml
--rw-r--r--   0        0        0        0 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/lib/__init__.py
--rw-r--r--   0        0        0      492 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/lib/constants.py
--rw-r--r--   0        0        0    16873 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/lib/controllers.py
--rw-r--r--   0        0        0     1867 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/lib/download.py
--rw-r--r--   0        0        0      497 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/lib/fetch.py
--rw-r--r--   0        0        0     9695 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/lib/table.py
--rw-r--r--   0        0        0     1366 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/lib/update.py
--rw-r--r--   0        0        0    17010 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/main.py
--rw-r--r--   0        0        0       38 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/namespace.py
--rw-r--r--   0        0        0      163 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/others/cron.vbs
--rw-r--r--   0        0        0      922 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/others/crontab.sh
--rw-r--r--   0        0        0      543 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/others/me.ricterz.bgmi.plist
--rw-r--r--   0        0        0      499 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/others/nginx.conf
--rw-r--r--   0        0        0        0 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/plugin/__init__.py
--rw-r--r--   0        0        0      955 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/plugin/download.py
--rw-r--r--   0        0        0     7872 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/script.py
--rw-r--r--   0        0        0      875 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/session.py
--rw-r--r--   0        0        0     1430 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/setup.py
--rw-r--r--   0        0        0    10988 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/website/__init__.py
--rw-r--r--   0        0        0     8295 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/website/bangumi_moe.py
--rw-r--r--   0        0        0     6092 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/website/base.py
--rw-r--r--   0        0        0    13771 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/website/mikan.py
--rw-r--r--   0        0        0     1518 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/website/model.py
--rw-r--r--   0        0        0     9146 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/website/share_dmhy.py
--rw-r--r--   0        0        0     4556 2023-04-05 20:19:41.178937 bgmi-5.0.0a2/pyproject.toml
--rw-r--r--   0        0        0    16343 1970-01-01 00:00:00.000000 bgmi-5.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/LICENSE
+-rw-r--r--   0        0        0    14535 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/README.md
+-rw-r--r--   0        0        0      176 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/__main__.py
+-rw-r--r--   0        0        0     6657 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/config.py
+-rw-r--r--   0        0        0      271 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/downloader/__init__.py
+-rw-r--r--   0        0        0     1862 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/downloader/aria2_rpc.py
+-rw-r--r--   0        0        0     1536 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/downloader/deluge.py
+-rw-r--r--   0        0        0      312 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/downloader/noop.py
+-rw-r--r--   0        0        0     1752 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/downloader/qbittorrent.py
+-rw-r--r--   0        0        0     1225 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/downloader/transmission.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/front/__init__.py
+-rw-r--r--   0        0        0     1139 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/front/index.py
+-rw-r--r--   0        0        0     2439 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/front/resources.py
+-rw-r--r--   0        0        0     8538 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/front/routes.py
+-rw-r--r--   0        0        0     2340 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/front/server.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/lib/__init__.py
+-rw-r--r--   0        0        0      492 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/lib/constants.py
+-rw-r--r--   0        0        0    13619 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/lib/controllers.py
+-rw-r--r--   0        0        0     2965 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/lib/download.py
+-rw-r--r--   0        0        0      497 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/lib/fetch.py
+-rw-r--r--   0        0        0    11043 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/lib/table.py
+-rw-r--r--   0        0        0     1368 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/lib/update.py
+-rw-r--r--   0        0        0    19581 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/main.py
+-rw-r--r--   0        0        0       38 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/namespace.py
+-rw-r--r--   0        0        0      163 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/others/cron.vbs
+-rw-r--r--   0        0        0      543 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/others/me.ricterz.bgmi.plist
+-rw-r--r--   0        0        0        0 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/others/nginx.conf
+-rw-r--r--   0        0        0        0 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/plugin/__init__.py
+-rw-r--r--   0        0        0      822 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/plugin/download.py
+-rw-r--r--   0        0        0     6884 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/script.py
+-rw-r--r--   0        0        0      875 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/session.py
+-rw-r--r--   0        0        0     1862 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/setup.py
+-rw-r--r--   0        0        0    11194 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/website/__init__.py
+-rw-r--r--   0        0        0     8294 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/website/bangumi_moe.py
+-rw-r--r--   0        0        0     6086 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/website/base.py
+-rw-r--r--   0        0        0    13570 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/website/mikan.py
+-rw-r--r--   0        0        0     1537 2023-04-11 19:26:08.379632 bgmi-5.0.0a3/bgmi/website/model.py
+-rw-r--r--   0        0        0     9103 2023-04-11 19:26:08.383632 bgmi-5.0.0a3/bgmi/website/share_dmhy.py
+-rw-r--r--   0        0        0     5108 2023-04-11 19:26:08.391632 bgmi-5.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0    16526 1970-01-01 00:00:00.000000 bgmi-5.0.0a3/PKG-INFO
```

### Comparing `bgmi-5.0.0a2/LICENSE` & `bgmi-5.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a2/README.md` & `bgmi-5.0.0a3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 [![](https://codecov.io/gh/BGmi/BGmi/branch/master/graph/badge.svg)](https://codecov.io/gh/BGmi/BGmi/branch/master/graph/badge.svg)
 [![](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/BGmi/BGmi/blob/master/LICENSE)
 
 ## TODO
 
 ## 更新日志
 
+### V5
+
+- 为 `bgmi update` 命令默认启用 `--download` 参数
+- 重构 bgmi_http
+- 移除 '/resource/feed.xml'
+
 ### v4
 
 - 添加 `proxy` 设置
 - 新 WEB UI
 - 将配置项 `transmission.rpc_url` 重命名为 `transmission.rpc_host`.
 - 修复 Transmission 配置的默认值.
 
@@ -32,19 +38,20 @@
 - 停止支持 python2，3.4 和 3.5
 - Transmission rpc 认证设置
 - 支持 [deluge-rpc](https://www.deluge-torrent.org/)
 - 使用最大和最小集数筛选搜索结果
 
 ## 特性
 
-- 多个数据源可选: [bangumi_moe](https://bangumi.moe), [mikan_project](https://mikanani.me) 或者[dmhy](https://share.dmhy.org/)
+- 多个数据源可选: [bangumi_moe](https://bangumi.moe), [mikan_project](https://mikanani.me)
+  或者[dmhy](https://share.dmhy.org/)
 - 使用 aria2, transmission, qbittorrent 或者 deluge 来下载你的番剧.
 - 提供一个管理和观看订阅番剧的前端.
 - 弹幕支持
-- 提供 uTorrent 支持的 RSS Feed 和移动设备支持的 ICS 格式日历.
+- 提供移动设备支持的 ICS 格式日历.
 - Bangumi Script: 添加自己的番剧解析器
 - 番剧放松列表和剧集信息
 - 下载番剧时的过滤器(支持关键词,字幕组和正则)
 - 多平台支持: Windows, macOS 以及 Linux
 
 ![](./images/bgmi_cli.png?raw=true)
 ![](https://github.com/BGmi/BGmi-frontend/raw/master/.github/images/example.png)
@@ -111,14 +118,15 @@
 **`--help`选项同样适用于所有的子命令，readme 仅介绍了一些基础用法。**
 
 ## 配置 BGmi
 
 BGmi 提供两种方式配置BGmi的各项运行参数，分别为配置文件与环境变量。
 
 ### 配置文件
+
 bgmi 的配置文件位于 `${BGMI_PATH}/config.toml`, 在未设置 `BGMI_PATH` 环境变量时，`${BGMI_PATH}` 默认为 `~/.bgmi/`。
 
 查看当前 `BGmi` 设置:
 
 ```bash
 bgmi config # 查看当前各项设置默认值.
 ```
@@ -131,19 +139,19 @@
 max_path = 3 # 抓取数据时每个番剧最大抓取页数
 bangumi_moe_url = "https://bangumi.moe"
 share_dmhy_url = "https://share.dmhy.org"
 mikan_username = "" # 蜜柑计划的用户名
 mikan_password = "" # 蜜柑计划的密码
 enable_global_filters = true
 global_filters = [
-    "Leopard-Raws",
-    "hevc",
-    "x265",
-    "c-a Raws",
-    "U3-Web",
+  "Leopard-Raws",
+  "hevc",
+  "x265",
+  "c-a Raws",
+  "U3-Web",
 ]
 
 proxy = '' # http proxy example: http://127.0.0.1:1080
 
 [save_path_map] # 针对每部番剧设置下载路径
 '致不灭的你 第二季' = '/home/trim21/downloads/bangumi/致不灭的你/s2/' # 如果使用绝对路径，可能导致 web-ui 无法正确显示视频文件。
 '致不灭的你 第三季' = './致不灭的你/s3/' # 以 save_path 为基础路径的相对路径
@@ -173,36 +181,40 @@
 
 [deluge]
 rpc_url = "http://127.0.0.1:8112/json"
 rpc_password = "deluge"
 ```
 
 ### 环境变量
+
 当 BGmi 的配置文件还未初始化时，各项运行参数可由环境变量进行配置
 
 环境变量以 `BGMI_` 开头，全大写命名，且各级配置以 `_` 进行分割，如:
+
 ```
 BGMI_DATA_SOURCE=bangumi_moe    # 对应配置文件中的 data_source = "bangumi_moe"
 BGMI_HTTP_ADMIN_TOKEN=dYMj-Z4bDRoQfd3x    # 对应配置文件 [http] 分段中的 admin_token = "dYMj-Z4bDRoQfd3x"
 ...
 ```
 
 环境变量 *暂不支持* 配置以下项目
+
 ```
 enable_global_include_keywords
 enable_global_filters
 global_include_keywords
 global_filters
 [save_path_map]
 ```
+
 注: 当配置文件生成完毕后，运行配置将会以配置文件为准，环境变量仅用于生成第一份配置文件。
 
 ## 修改配置
 
-使用 `bgmi config set ...keys  --value '...'` 命令可以修改配置。
+使用 `bgmi config set ...keys --value '...'` 命令可以修改配置。
 
 如：
 
 ```shell
 bgmi config set http admin_token --value 'my super secret token'
 ```
 
@@ -227,15 +239,14 @@
 
 **如果更换的源为 `mikan_project`, 请先配置 `MIKAN_USERNAME` 和 `MIKAN_PASSWORD`**, 其它源不受影响
 
 ```bash
 bgmi source mikan_project
 ```
 
-
 ### 设置下载方式
 
 修改配置文件和对应的配置项
 
 ```toml
 download_delegate = "aria2-rpc" # download delegate
 ```
@@ -286,25 +297,23 @@
 bgmi filter "Re:CREATORS" --subtitle "" --include "" --exclude "" --regex "..."
 bgmi filter "Re:CREATORS" --regex "(DHR動研字幕組|豌豆字幕组).*(720P)"
 bgmi fetch "Re:CREATORS"
 ```
 
 ## 设置全局过滤关键词
 
-
 ### 包含
 
 默认不启用全局包含关键词，你可以设置 `enable_global_include_keywords = true` 启动此功能。
 
 ```toml
 enable_global_include_keywords = true
 global_include_keywords = ['1080']
 ```
 
-
 ### 排除
 
 有一些默认定义的全局过滤关键词，默认会排除标题包含以下关键词的种子。
 可以使用 `enable_global_filters = false` 禁止过滤全局关键词，
 
 ```toml
 enable_global_filters = true
@@ -336,15 +345,15 @@
 
 `bgmi search`命令默认不会显示重复的集数, 如果要显示重复的集数来方便过滤, 在命令后加上`--dupe`来显示全部的搜索结果
 
 手动修改最近下载的剧集
 
 ```bash
 bgmi list
-bgmi mark "Re:CREATORS" 1
+bgmi mark "Re:CREATORS" --episode 1
 ```
 
 ## 使用`bgmi_http`
 
 1.先下载所有更新中番剧的封面
 
 ```bash
@@ -416,15 +425,16 @@
 
 [me.ricterz.bgmi.plist](https://github.com/BGmi/BGmi/blob/master/bgmi/others/me.ricterz.bgmi.plist)
 
 ## 弹幕支持
 
 BGmi 使用[`DPlayer`](https://github.com/DIYgod/DPlayer)做为前端播放器
 
-如果你想要添加弹幕支持, 在这里[DPlayer#related-projects](https://github.com/DIYgod/DPlayer#related-projects)选择一个后端自行搭建, 或者使用`DPlayer`提供的现成接口`https://api.prprpr.me/dplayer/`
+如果你想要添加弹幕支持, 在这里[DPlayer#related-projects](https://github.com/DIYgod/DPlayer#related-projects)选择一个后端自行搭建,
+或者使用`DPlayer`提供的现成接口`https://api.prprpr.me/dplayer/`
 
 然后修改配置文件：
 
 ```toml
 [bgmi_http]
 danmaku_api_url = "https://api.prprpr.me/dplayer/"  # This api is provided by dplayer official
 ```
@@ -451,85 +461,89 @@
 schtasks /Delete /TN 'bgmi updater'
 ```
 
 ## 如果你对 python 有一点了解, 并且觉得还不够的话, 下面是为你准备的.
 
 ## Bangumi Script
 
-你可以写一个`BGmi Script`来解析你自己的想看的番剧或者美剧. BGmi 会加载你的 script, 视作一个番剧来对待. 而你所需要做的只是继承`ScriptBase`类, 然后实现特定的方法, 再把你的 script 文件放到`BGMI_PATH/script`文件夹内.
+你可以写一个`BGmi Script`来解析你自己的想看的番剧或者美剧. BGmi 会加载你的 script, 视作一个番剧来对待.
+而你所需要做的只是继承`ScriptBase`类, 然后实现特定的方法, 再把你的 script 文件放到`BGMI_PATH/script`文件夹内.
 
 Example: [./tests/script_example.py](./tests/script_example.py)
 
 `get_download_url()`返回一个`dict`, 以对应集数为键, 对应的下载链接为值
 
 ```python
 {
-    1: 'http://example.com/Bangumi/1/1.mp4',
-    2: 'http://example.com/Bangumi/1/2.torrent',
-    3: 'http://example.com/Bangumi/1/3.mp4'
+  1: 'http://example.com/Bangumi/1/1.mp4',
+  2: 'http://example.com/Bangumi/1/2.torrent',
+  3: 'http://example.com/Bangumi/1/3.mp4'
 }
 ```
 
+### 加载 scripts
+
+注意，scripts只会在运行 `bgmi update` 或者 `bgmi cal` 时被加载。如果你在 web ui 找不到对应的内容，请运行前面提到的命令并重试。
+
 ## BGmi 数据源
 
 通过扩展`bgmi.website.base.BaseWebsite`类并且实现对应的三个方法,你也可以简单的添加一个数据源
 
 每个方法具体的意义和返回值格式请参照每个方法对应的注释
 
 ```python
 from typing import List, Optional
 
 from bgmi.website.base import BaseWebsite
 from bgmi.website.model import Episode, WebsiteBangumi
 
 
 class DataSource(BaseWebsite):
-    def search_by_keyword(
-        self, keyword: str, count: int
-    ) -> List[Episode]:  # pragma: no cover
-        """
-
-        :param keyword: search key word
-        :param count: how many page to fetch from website
-        :return: list of episode search result
-        """
-        raise NotImplementedError
-
-    def fetch_bangumi_calendar(self,) -> List[WebsiteBangumi]:  # pragma: no cover
-        """
-        return a list of all bangumi and a list of all subtitle group
-
-        list of bangumi dict:
-        update time should be one of ['Sun', 'Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Unknown']
-        """
-        raise NotImplementedError
-
-    def fetch_episode_of_bangumi(
-        self, bangumi_id: str, max_page: int, subtitle_list: Optional[List[str]] = None
-    ) -> List[Episode]:  # pragma: no cover
-        """
-        get all episode by bangumi id
-
-        :param bangumi_id: bangumi_id
-        :param subtitle_list: list of subtitle group
-        :type subtitle_list: list
-        :param max_page: how many page you want to crawl if there is no subtitle list
-        :type max_page: int
-        :return: list of bangumi
-        """
-        raise NotImplementedError
-
-
-    def fetch_single_bangumi(self, bangumi_id: str) -> WebsiteBangumi:
-        """
-        fetch bangumi info when updating
-
-        :param bangumi_id: bangumi_id, or bangumi['keyword']
-        :type bangumi_id: str
-        :rtype: WebsiteBangumi
-        """
-        # return WebsiteBangumi(keyword=bangumi_id) if website don't has a page contains episodes and info
+  def search_by_keyword(
+    self, keyword: str, count: int
+  ) -> List[Episode]:  # pragma: no cover
+    """
+
+    :param keyword: search key word
+    :param count: how many page to fetch from website
+    :return: list of episode search result
+    """
+    raise NotImplementedError
+
+  def fetch_bangumi_calendar(self, ) -> List[WebsiteBangumi]:  # pragma: no cover
+    """
+    return a list of all bangumi and a list of all subtitle group
+
+    list of bangumi dict:
+    update time should be one of ['Sun', 'Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Unknown']
+    """
+    raise NotImplementedError
+
+  def fetch_episode_of_bangumi(
+    self, bangumi_id: str, max_page: int, subtitle_list: Optional[List[str]] = None
+  ) -> List[Episode]:  # pragma: no cover
+    """
+    get all episode by bangumi id
+
+    :param bangumi_id: bangumi_id
+    :param subtitle_list: list of subtitle group
+    :type subtitle_list: list
+    :param max_page: how many page you want to crawl if there is no subtitle list
+    :type max_page: int
+    :return: list of bangumi
+    """
+    raise NotImplementedError
+
+  def fetch_single_bangumi(self, bangumi_id: str) -> WebsiteBangumi:
+    """
+    fetch bangumi info when updating
+
+    :param bangumi_id: bangumi_id, or bangumi['keyword']
+    :type bangumi_id: str
+    :rtype: WebsiteBangumi
+    """
+    # return WebsiteBangumi(keyword=bangumi_id) if website don't has a page contains episodes and info
 ```
 
 ## License
 
 [MIT License](./LICENSE)
```

### Comparing `bgmi-5.0.0a2/bgmi/config.py` & `bgmi-5.0.0a3/bgmi/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,18 +25,24 @@
 def get_bgmi_home() -> Path:
     h = os.environ.get("BGMI_PATH")
 
     if h:
         return Path(h)
 
     if IS_WINDOWS:
-        home_dir = os.environ.get("USERPROFILE") or os.environ.get("HOME") or tempfile.gettempdir()
+        home_dir = os.environ.get("USERPROFILE") or os.environ.get("HOME")
+    else:
+        home_dir = os.environ.get("HOME")
+
+    if home_dir:
         return Path(home_dir).joinpath(".bgmi")
 
-    return Path(os.environ.get("HOME", "/tmp")).joinpath(".bgmi")
+    tmp_dir = Path(tempfile.gettempdir()).joinpath(".bgmi")
+    print(f"can't find user home, use temp dir {tmp_dir} as bgmi home")
+    return tmp_dir
 
 
 BGMI_PATH = get_bgmi_home().absolute()
 
 CONFIG_FILE_PATH = BGMI_PATH / "config.toml"
 
 
@@ -78,15 +84,15 @@
         description="webui admin token",
     )
     danmaku_api_url: str = Field(
         os.getenv("BGMI_HTTP_DANMAKU_API_URL") or "",
         description="danmaku api url, https://github.com/DIYgod/DPlayer#related-projects",
     )
     serve_static_files: bool = Field(
-        bool(os.getenv("BGMI_HTTP_SERVE_STATIC_FILES")), description="use tornado serving video files"
+        bool(os.getenv("BGMI_HTTP_SERVE_STATIC_FILES")), description="serve static files with main"
     )
 
 
 class Config(BaseSetting):
     data_source: Source = Field(
         os.getenv("BGMI_DATA_SOURCE") or Source.BangumiMoe, description="data source"
     )  # type: ignore
@@ -176,15 +182,15 @@
 if CONFIG_FILE_PATH.exists():
     try:
         cfg = Config.parse_obj(tomlkit.loads(CONFIG_FILE_PATH.read_text(encoding="utf8")).unwrap())
     except pydantic.ValidationError as e:
         print("配置文件错误，请手动编辑配置文件后重试")
         print("配置文件位置：", CONFIG_FILE_PATH)
         print(e)
-        raise SystemExit
+        raise SystemExit from e
 else:
     cfg = Config()
 
 
 def print_config() -> str:
     return tomlkit.dumps(json.loads(cfg.json()))
```

### Comparing `bgmi-5.0.0a2/bgmi/downloader/aria2_rpc.py` & `bgmi-5.0.0a3/bgmi/downloader/aria2_rpc.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a2/bgmi/downloader/deluge.py` & `bgmi-5.0.0a3/bgmi/downloader/deluge.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
     def add_download(self, url: str, save_path: str):
         options = {
             "add_paused": False,
             "move_completed": False,
             "download_location": save_path,
         }
-        e = self._call("core.add_torrent_url", [url, options])
-        return e
+        return self._call("core.add_torrent_url", [url, options])
 
     def _call(self, methods, params=None):
         if params is None:
             params = []
         r = self._session.post(
             cfg.deluge.rpc_url,
             headers={"Content-Type": "application/json"},
@@ -43,10 +42,10 @@
             timeout=10,
         )
 
         self._id += 1
         e = r.json()
 
         if "result" not in e:
-            raise RpcError("deluge error, reason: {}".format(e["error"]["message"]))
+            raise RpcError(f"deluge error, reason: {e['error']['message']}")
 
         return e["result"]
```

### Comparing `bgmi-5.0.0a2/bgmi/downloader/qbittorrent.py` & `bgmi-5.0.0a3/bgmi/downloader/qbittorrent.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a2/bgmi/downloader/transmission.py` & `bgmi-5.0.0a3/bgmi/downloader/transmission.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a2/bgmi/lib/controllers.py` & `bgmi-5.0.0a3/bgmi/lib/controllers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,33 @@
 import itertools
 import os.path
 import time
-from collections import defaultdict
-from operator import itemgetter
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 import filetype
 import requests.exceptions
 import sqlalchemy as sa
 
-from bgmi.config import Source, cfg
-from bgmi.lib.constants import BANGUMI_UPDATE_TIME, SUPPORT_WEBSITE
-from bgmi.lib.download import Episode, download_episodes
+from bgmi.config import cfg
+from bgmi.lib.download import download_episode
 from bgmi.lib.fetch import website
-from bgmi.lib.table import (
-    FOLLOWED_STATUS,
-    STATUS_DELETED,
-    STATUS_FOLLOWED,
-    STATUS_NOT_DOWNLOAD,
-    STATUS_UPDATED,
-    Bangumi,
-    Download,
-    Followed,
-    NotFoundError,
-    Session,
-    Subtitle,
-    recreate_source_relatively_table,
-)
+from bgmi.lib.table import Bangumi, Download, Followed, NotFoundError, Scripts, Session, Subtitle
 from bgmi.script import ScriptRunner
 from bgmi.utils import (
-    COLOR_END,
-    GREEN,
     convert_cover_url_to_path,
     download_cover,
     episode_filter_regex,
     logger,
     normalize_path,
     print_error,
     print_info,
     print_success,
     print_warning,
 )
+from bgmi.website.model import Episode
 
 ControllerResult = Dict[str, Any]
 
 
 def add(name: str, episode: Optional[int] = None) -> ControllerResult:
     """
     ret.name :str
@@ -52,45 +35,44 @@
     # action add
     # add bangumi by a list of bangumi name
     logger.debug("add name: {} episode: {}", name, episode)
     if not Bangumi.get_updating_bangumi():
         website.fetch(group_by_weekday=False)
 
     try:
-        bangumi_obj = Bangumi.fuzzy_get(name=name)
+        bangumi_obj = Bangumi.get(Bangumi.name.contains(name))
         name = bangumi_obj.name
     except Bangumi.NotFoundError:
         result = {
             "status": "error",
             "message": f"{name} not found, please check the name",
         }
         return result
 
     with Session.begin() as session:
         followed_obj: Optional[Followed] = session.scalar(
             sa.select(Followed).where(Followed.bangumi_name == bangumi_obj.name).limit(1)
         )
         if followed_obj is None:
-            followed_obj = Followed(status=STATUS_FOLLOWED, bangumi_name=bangumi_obj.name, episode=0)
+            followed_obj = Followed(status=Followed.STATUS_FOLLOWED, bangumi_name=bangumi_obj.name)
             session.add(followed_obj)
+        elif followed_obj.status == Followed.STATUS_FOLLOWED:
+            result = {
+                "status": "warning",
+                "message": f"{bangumi_obj.name} already followed",
+            }
+            return result
         else:
-            if followed_obj.status == STATUS_FOLLOWED:
-                result = {
-                    "status": "warning",
-                    "message": f"{bangumi_obj.name} already followed",
-                }
-                return result
-            else:
-                followed_obj.status = STATUS_FOLLOWED
+            followed_obj.status = Followed.STATUS_FOLLOWED
 
     if episode is None:
         episodes = website.get_maximum_episode(bangumi_obj, max_page=cfg.max_path)
-        followed_obj.episode = max(e.episode for e in episodes) if episodes else 0
+        followed_obj.episodes = sorted([e.episode for e in episodes]) if episodes else 0  # type: ignore
     else:
-        followed_obj.episode = episode
+        followed_obj.episodes = list(range(0, episode + 1))
 
     followed_obj.save()
 
     result = {"status": "success", "message": f"add {bangumi_obj.name} to subscribing bangumi list"}
     logger.debug(result)
     return result
 
@@ -100,15 +82,15 @@
     subtitle: Optional[str] = None,
     include: Optional[str] = None,
     exclude: Optional[str] = None,
     regex: Optional[str] = None,
 ) -> ControllerResult:
     result = {"status": "success", "message": ""}  # type: Dict[str, Any]
     try:
-        bangumi_obj = Bangumi.fuzzy_get(name=name)
+        bangumi_obj = Bangumi.get(Bangumi.name.contains(name))
     except Bangumi.NotFoundError:
         result["status"] = "error"
         result["message"] = f"Bangumi {name} does not exist."
         return result
 
     try:
         followed_filter_obj = Followed.get(Followed.bangumi_name == bangumi_obj.name)
@@ -167,15 +149,15 @@
             result["status"] = "warning"
             result["message"] = "all subscriptions have been deleted"
         else:
             print_error("user canceled")
     elif name:
         try:
             followed = Followed.get(Followed.bangumi_name == name)
-            followed.status = STATUS_DELETED
+            followed.status = Followed.STATUS_DELETED
             followed.save()
             result["status"] = "warning"
             result["message"] = f"Bangumi {name} has been deleted"
         except Followed.NotFoundError:
             result["status"] = "error"
             result["message"] = f"Bangumi {name} does not exist"
     else:
@@ -214,15 +196,15 @@
         if cover_to_be_download:
             print_info("Updating cover ...")
             download_cover(cover_to_be_download)
 
     runner = ScriptRunner()
     patch_list = runner.get_models_dict()
     for i in patch_list:
-        weekly_list[i["update_time"].lower()].append(i)
+        weekly_list[i["update_day"].lower()].append(i)
     logger.debug(weekly_list)
 
     # for web api, return all subtitle group info
     r = weekly_list  # type: Dict[str, List[Dict[str, Any]]]
     for day, value in weekly_list.items():
         for index, bangumi in enumerate(value):
             bangumi["cover"] = normalize_path(bangumi["cover"])
@@ -231,40 +213,14 @@
             ]
 
             r[day][index]["subtitle_group"] = subtitle_group
     logger.debug(r)
     return r
 
 
-def mark(name: str, episode: int) -> ControllerResult:
-    """
-
-    :param name: name of the bangumi you want to mark
-    :param episode: bangumi episode you want to mark
-    """
-    result = {}
-
-    try:
-        followed_obj = Followed.get(Followed.bangumi_name == name)
-    except Followed.NotFoundError:
-        runner = ScriptRunner()
-        followed_obj = runner.get_model(name)  # type: ignore
-        if not followed_obj:
-            result["status"] = "error"
-            result["message"] = f"Subscribe or Script <{name}> does not exist."
-            return result
-
-    followed_obj.episode = episode
-    followed_obj.save()
-
-    result["status"] = "success"
-    result["message"] = f"{name} has been mark as episode: {episode}"
-    return result
-
-
 def search(
     keyword: str,
     count: int = cfg.max_path,
     regex: Optional[str] = None,
     dupe: bool = False,
     min_episode: Optional[int] = None,
     max_episode: Optional[int] = None,
@@ -312,137 +268,130 @@
                 "min_episode": min_episode,
                 "max_episode": max_episode,
             },
             "data": [],
         }
 
 
-def source(data_source: str) -> ControllerResult:
-    result = {}
-    if data_source in list(map(itemgetter("id"), SUPPORT_WEBSITE)):
-        recreate_source_relatively_table()
-        cfg.data_source = Source(data_source)
-        cfg.save()
-        print_success("data source switch succeeds")
-        result["status"] = "success"
-        result["message"] = f"you have successfully change your data source to {data_source}"
-    else:
-        result["status"] = "error"
-        result["message"] = "please check your input. data source should be one of {}".format(
-            [x["id"] for x in SUPPORT_WEBSITE]
-        )
-    return result
-
-
-def update(names: List[str], download: Optional[bool] = False, not_ignore: bool = False) -> ControllerResult:
-    logger.debug("updating bangumi info with args: download: %r", download)
-    downloaded: List[Episode] = []
-    result: Dict[str, Any] = {
-        "status": "info",
-        "message": "",
-        "data": {"updated": [], "downloaded": downloaded},
-    }
+def update(names: List[str], download: Optional[bool] = False, not_ignore: bool = False) -> None:
+    logger.debug("updating bangumi info with args: download: {}", download)
 
     ignore = not bool(not_ignore)
-    print_info("marking bangumi status ...")
     now = int(time.time())
-
-    for follow in Followed.get_all_followed():
-        if follow.updated_time and int(follow.updated_time + 60 * 60 * 24) < now:
-            follow.status = STATUS_FOLLOWED
-            follow.save()
-
-    for script in ScriptRunner().scripts:
-        obj = script.Model().obj
-        if obj.updated_time and int(obj.updated_time + 60 * 60 * 24) < now:
-            obj.status = STATUS_FOLLOWED
-            obj.save()
-
     print_info("updating subscriptions ...")
 
     if not names:
-        updated_bangumi_obj = Followed.get_all_followed()
+        updated_bangumi_obj = [x[0] for x in Followed.get_all_followed()]
     else:
         updated_bangumi_obj = []
         for n in names:
             try:
                 f = Followed.get(Followed.bangumi_name == n)
                 updated_bangumi_obj.append(f)
             except Followed.NotFoundError:
                 logger.warning("missing followed bangumi '{}'", n)
 
     if download:
-        failed = [Episode.parse_obj(x) for x in Download.get_all_downloads(status=STATUS_NOT_DOWNLOAD)]
-        if failed:
+        need_re_download = []
+        failures = Download.get_all_downloads(status=Download.STATUS_NOT_DOWNLOAD)
+        followings: Dict[str, Followed] = {x.bangumi_name: x for x in Followed.all()}
+
+        if failures:
+            for fail in failures:
+                following = followings.get(fail.bangumi_name)
+                if not following:
+                    continue
+
+                if fail.episode in following.episodes:
+                    continue
+
+                need_re_download.append(fail)
+
+        if need_re_download:
             print_info("try to re-downloading previous failed torrents ...")
-            download_episodes(failed)
+            for d in need_re_download:
+                download_episode(
+                    Episode(
+                        title=d.title,
+                        episode=d.episode,
+                        download=d.download,
+                        name=d.bangumi_name,
+                    )
+                )
 
     runner = ScriptRunner()
-    script_download_queue = runner.run()
-    if script_download_queue and download:
-        download_episodes(script_download_queue)
-        downloaded.extend(script_download_queue)
-        print_info("downloading ...")
+
+    for script, all_episode_data in runner.run():
+        following = Followed.get(Followed.bangumi_name == script.bangumi_name)
+
+        if not download:
+            following.episodes = sorted({x.episode for x in all_episode_data} | set(following.episodes))
+            following.updated_time = now
+            following.save()
+        else:
+            download_episodes(all_episode_data, following)
 
     for subscribe in updated_bangumi_obj:
-        download_queue = []
         print_info(f"fetching {subscribe.bangumi_name} ...")
         try:
             bangumi_obj = Bangumi.get(Bangumi.name == subscribe.bangumi_name)
         except NotFoundError:
             logger.error("Bangumi<{}> does not exists.", subscribe.bangumi_name)
             continue
         try:
-            followed_obj = Followed.get(Followed.bangumi_name == subscribe.bangumi_name)
+            following = Followed.get(Followed.bangumi_name == subscribe.bangumi_name)
         except NotFoundError:
             logger.error("Followed<{}> is not followed.", subscribe.bangumi_name)
             continue
 
         try:
             all_episode_data = website.get_maximum_episode(
                 bangumi=bangumi_obj, ignore_old_row=ignore, max_page=cfg.max_path
             )
         except requests.exceptions.ConnectionError as e:
             print_warning(f"error {e} to fetch {bangumi_obj.name}, skip")
             continue
 
-        if all_episode_data:
-            episode = max(e.episode for e in all_episode_data)
+        if not all_episode_data:
+            continue
+
+        if not download:
+            following.episodes = sorted({x.episode for x in all_episode_data} | set(following.episodes))
+            following.save()
         else:
-            episode = 0
+            download_episodes(all_episode_data, following)
 
-        if episode > subscribe.episode:
-            episode_range = range(subscribe.episode, episode + 1)
-            print_success(f"{subscribe.bangumi_name} updated, episode: {episode:d}")
-            followed_obj.episode = episode
-            followed_obj.status = STATUS_UPDATED
-            followed_obj.updated_time = int(time.time())
-            followed_obj.save()
-            result["data"]["updated"].append({"bangumi": subscribe.bangumi_name, "episode": episode})
 
-            groups: Dict[int, List[Episode]] = {
-                key: list(value) for key, value in itertools.groupby(all_episode_data, lambda x: x.episode)
-            }
+def download_episodes(all_episode_data: List[Episode], following: Union[Followed, Scripts]) -> None:
+    groups: Dict[int, List[Episode]] = {
+        key: list(value) for key, value in itertools.groupby(all_episode_data, lambda x: x.episode)
+    }
 
-            for i in episode_range:
-                episodes = groups.get(i)
-                if episodes:
-                    download_queue.append(episodes.pop())
-
-        if download:
-            download_episodes(download_queue)
-            downloaded.extend(download_queue)
+    for ep, episodes in sorted(groups.items()):
+        if ep in following.episodes:
+            # already downloaded, skipping
+            continue
 
-    return result
+        print_success(f"{following.bangumi_name} updated, episode: {ep:d}")
+        following.status = Followed.STATUS_UPDATED
 
+        if episodes:
+            for e in episodes:
+                if download_episode(e):
+                    following.episodes.append(ep)  # type: ignore
+                    break
 
-def status_(name: str, status: int = STATUS_DELETED) -> ControllerResult:
+    following.updated_time = int(time.time())
+    following.save()
+
+
+def status_(name: str, status: int = Followed.STATUS_DELETED) -> ControllerResult:
     result = {"status": "success", "message": ""}
 
-    if (status not in FOLLOWED_STATUS) or (not status):
+    if (status not in Followed.FOLLOWED_STATUS) or (not status):
         result["status"] = "error"
         result["message"] = f"Invalid status: {status}"
         return result
 
     status = int(status)
 
     followed_obj = Followed.get(Followed.bangumi_name == name)
@@ -451,55 +400,7 @@
         result["message"] = f"Followed<{name}> does not exists"
         return result
 
     followed_obj.status = status
     followed_obj.save()
     result["message"] = f"Followed<{name}> has been marked as status {status}"
     return result
-
-
-def followed_bangumi() -> Dict[str, list]:
-    """
-
-    :return: list of bangumi followed
-    """
-    weekly_list_followed = Bangumi.get_updating_bangumi(status=STATUS_FOLLOWED)
-    weekly_list_updated = Bangumi.get_updating_bangumi(status=STATUS_UPDATED)
-    weekly_list = defaultdict(list)
-    for k, v in itertools.chain(weekly_list_followed.items(), weekly_list_updated.items()):
-        weekly_list[k].extend(v)
-    for bangumi_list in weekly_list.values():
-        for bangumi in bangumi_list:
-            bangumi["subtitle_group"] = Subtitle.get_subtitle_by_id(bangumi["subtitle_group"])
-    return weekly_list
-
-
-def list_() -> ControllerResult:
-    result = {}
-    weekday_order = BANGUMI_UPDATE_TIME
-    followed = followed_bangumi()
-
-    script_bangumi = ScriptRunner().get_models_dict()
-
-    if not followed and not script_bangumi:
-        result["status"] = "warning"
-        result["message"] = "you have not subscribed any bangumi"
-        return result
-
-    for i in script_bangumi:
-        i["subtitle_group"] = [{"name": "<BGmi Script>"}]
-        followed[i["update_time"].lower()].append(i)
-
-    result["status"] = "info"
-    result["message"] = ""
-    for weekday in weekday_order:
-        if followed[weekday.lower()]:
-            result["message"] += f"{GREEN}{weekday}. {COLOR_END}"
-            for j, bangumi in enumerate(followed[weekday.lower()]):
-                if bangumi["status"] in (STATUS_UPDATED, STATUS_FOLLOWED) and "episode" in bangumi:
-                    bangumi["name"] = f"{bangumi['name']}({bangumi['episode']:d})"
-                if j > 0:
-                    result["message"] += " " * 5
-                f = [x.name for x in bangumi["subtitle_group"]]
-                result["message"] += "{}: {}\n".format(bangumi["name"], ", ".join(f) if f else "<None>")
-
-    return result
```

### Comparing `bgmi-5.0.0a2/bgmi/lib/table.py` & `bgmi-5.0.0a3/bgmi/lib/table.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 import os
 import time
 from collections import defaultdict
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Type, TypeVar
 
 import sqlalchemy as sa
-from sqlalchemy import CHAR, Column, Integer, Text, create_engine
+import sqlalchemy.event
+from loguru import logger
+from sqlalchemy import CHAR, Column, Integer, Row, Text, create_engine
 from sqlalchemy.orm import DeclarativeBase, Mapped, sessionmaker
 
 from bgmi.config import cfg
 from bgmi.utils import episode_filter_regex
 from bgmi.website.model import Episode
 
-# bangumi status
-STATUS_UPDATING = 0
-STATUS_END = 1
-BANGUMI_STATUS = (STATUS_UPDATING, STATUS_END)
-
 # subscription status
-STATUS_DELETED = 0
-STATUS_FOLLOWED = 1
-STATUS_UPDATED = 2
-FOLLOWED_STATUS = (STATUS_DELETED, STATUS_FOLLOWED, STATUS_UPDATED)
-
-# download status
-STATUS_NOT_DOWNLOAD = 0
-STATUS_DOWNLOADING = 1
-STATUS_DOWNLOADED = 2
-DOWNLOAD_STATUS = (STATUS_NOT_DOWNLOAD, STATUS_DOWNLOADING, STATUS_DOWNLOADED)
 
-engine = create_engine(f"sqlite:///{cfg.db_path.absolute().as_posix()}")
+debug = os.getenv("DEBUG") in ["true", "True"]
+
+
+def before_cursor_execute(
+    _: Any, cursor: Any, statement: str, parameters: List[Any], *args: Any, **kwargs: Any
+) -> None:
+    logger.debug("executing sql {} {}", statement, parameters)
+    if debug:
+        print(statement, parameters)
 
+
+engine = create_engine(f"sqlite:///{cfg.db_path.absolute().as_posix()}")
+sqlalchemy.event.listen(engine, "before_cursor_execute", before_cursor_execute)
 Session = sessionmaker(engine, expire_on_commit=False)
 
 
 class NotFoundError(Exception):
     def __init__(self, cls: Type["Base"]) -> None:
         super().__init__(f"{cls} not found")
 
@@ -53,15 +51,19 @@
             return o
 
     @classmethod
     def all(cls: Type[T], *where: Any) -> List[T]:
         with Session.begin() as session:
             return list(session.scalars(sa.select(cls).where(*where)).all())
 
-    def save(self) -> None:
+    def save(self, tx: Optional[sa.orm.Session] = None) -> None:
+        if tx:
+            tx.add(self)
+            return
+
         with Session.begin() as session:
             session.add(self)
 
 
 if os.environ.get("DEV"):
     print(f"using database {cfg.db_path}")
 
@@ -71,29 +73,29 @@
     STATUS_UPDATING = 0
     STATUS_END = 1
 
     id: Mapped[str] = Column(Text, primary_key=True, nullable=False)  # type: ignore
 
     name: Mapped[str] = Column(Text, nullable=False, unique=True)  # type: ignore
     subtitle_group: Mapped[List[str]] = Column(sa.JSON, nullable=False, default=[], server_default="[]")  # type: ignore
-    update_time: Mapped[str] = Column(
+    update_day: Mapped[str] = Column(
         CHAR(5), nullable=False, default="Unknown", server_default="Unknown"
     )  # type: ignore
     cover: Mapped[str] = Column(Text, nullable=False, default="", server_default="")  # type: ignore
     status: Mapped[int] = Column(
         Integer, nullable=False, default=STATUS_UPDATING, server_default=str(STATUS_UPDATING)
     )  # type: ignore
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             id: str,
             name: str,
-            update_time: str = "Unknown",
+            update_day: str = "Unknown",
             subtitle_group: Optional[List[str]] = None,
             cover: str = "",
             status: int = STATUS_UPDATING,
         ):
             super().__init__()
 
     @classmethod
@@ -108,89 +110,97 @@
             if os.getenv("DEBUG"):  # pragma: no cover
                 print("ignore updating bangumi", [x.bangumi_name for x in un_updated_bangumi])
 
             # do not mark updating bangumi as STATUS_END
             session.execute(
                 sa.update(cls)
                 .where(cls.name.not_in([x.bangumi_name for x in un_updated_bangumi]))
-                .values(status=STATUS_END)
+                .values(status=cls.STATUS_END)
             )
 
     @classmethod
     def get_updating_bangumi(
         cls,
         status: Optional[int] = None,
     ) -> Dict[str, List[Dict[str, Any]]]:
         if status is None:
-            where = cls.status == STATUS_UPDATING
+            where = cls.status == cls.STATUS_UPDATING
         else:
-            where = (cls.status == STATUS_UPDATING) & (Followed.status == status)
+            where = (cls.status == cls.STATUS_UPDATING) & (Followed.status == status)
 
         with Session.begin() as session:
             data = (
-                session.query(cls, Followed.status, Followed.episode)
+                session.query(cls, Followed.status, Followed.episodes)
                 .outerjoin(Followed, cls.name == Followed.bangumi_name)
                 .where(where)
                 .all()
             )
 
         weekly_list = defaultdict(list)
         for bangumi_item, followed_status, episode in data:
-            weekly_list[bangumi_item.update_time.lower()].append(
-                {**bangumi_item.__dict__, "status": followed_status, "episode": episode}
+            weekly_list[bangumi_item.update_day.lower()].append(
+                {**bangumi_item.__dict__, "status": followed_status, "episode": max(episode) if episode else None}
             )
 
         return weekly_list
 
-    @classmethod
-    def fuzzy_get(cls, name: str) -> "Bangumi":
-        return cls.get(cls.name.contains(name))
-
 
 class Followed(Base):
     __tablename__ = "followed"
 
     STATUS_DELETED = 0
     STATUS_FOLLOWED = 1
     STATUS_UPDATED = 2
 
+    FOLLOWED_STATUS = (
+        STATUS_DELETED,
+        STATUS_FOLLOWED,
+        STATUS_UPDATED,
+    )
+
     bangumi_name: Mapped[str] = Column(Text, nullable=False, primary_key=True)  # type: ignore
-    episode: Mapped[int] = Column(Integer, nullable=False, default=0, server_default="0")  # type: ignore
+    episodes: Mapped[List[int]] = Column(sa.JSON, nullable=False, default=[], server_default="[]")  # type: ignore
     status: Mapped[int] = Column(
-        Integer, nullable=False, default=STATUS_UPDATING, server_default=str(STATUS_UPDATING)
+        Integer, nullable=False, default=STATUS_UPDATED, server_default=str(STATUS_UPDATED)
     )  # type: ignore
     updated_time: Mapped[int] = Column(Integer, nullable=False, default=0, server_default="0")  # type: ignore
     subtitle: List[str] = Column(sa.JSON, nullable=False, default=[], server_default="[]")  # type: ignore
     include: Mapped[List[str]] = Column(sa.JSON, nullable=False, default=[], server_default="[]")  # type: ignore
     exclude: Mapped[List[str]] = Column(sa.JSON, nullable=False, default=[], server_default="[]")  # type: ignore
     regex: Mapped[str] = Column(Text, nullable=False, default="", server_default="")  # type: ignore
 
+    is_script: Mapped[bool] = Column(sa.Boolean, nullable=False, default=False, server_default="0")  # type: ignore
+
+    @property
+    def episode(self) -> int:
+        if self.episodes:
+            return max(self.episodes)  # type: ignore
+        return 0
+
     @classmethod
     def delete_followed(cls, batch: bool = True) -> bool:
-        if not batch:
-            if not input("[+] are you sure want to CLEAR ALL THE BANGUMI? (y/N): ") == "y":
-                return False
+        if not batch and input("[+] are you sure want to CLEAR ALL THE BANGUMI? (y/N): ") != "y":
+            return False
 
         with Session.begin() as session:
             session.execute(sa.delete(cls))
         return True
 
     @classmethod
     def get_all_followed(
-        cls: Type["Followed"], status: int = STATUS_DELETED, bangumi_status: int = STATUS_UPDATING
-    ) -> List["Followed"]:
-        sql = (
-            sa.select(Followed)
-            .join(Bangumi, cls.bangumi_name == Bangumi.name)
-            .where(cls.status.isnot(status), Bangumi.status == bangumi_status)
-            .order_by(cls.updated_time.desc())
-        )
-
-        with Session() as s:
-            return list(s.scalars(sql))
+        cls: Type["Followed"], bangumi_status: int = Bangumi.STATUS_UPDATING
+    ) -> List[Row[Tuple["Followed", "Bangumi"]]]:
+        with Session() as tx:
+            return list(
+                tx.query(Followed, Bangumi)
+                .join(Bangumi, cls.bangumi_name == Bangumi.name)
+                .where(cls.status.isnot(cls.STATUS_DELETED), Bangumi.status == bangumi_status)
+                .order_by(cls.updated_time.desc())
+                .all()
+            )
 
     def apply_on_episodes(self, result: List[Episode]) -> List[Episode]:
         if self.include:
             # pylint:disable=no-member
             include_list = [s.strip().lower() for s in self.include]
             result = [e for e in result if e.contains_any_words(include_list)]
 
@@ -201,37 +211,58 @@
         if self.exclude:
             # pylint:disable=no-member
             exclude_list = [s.strip().lower() for s in self.exclude]
             result = [e for e in result if not e.contains_any_words(exclude_list)]
 
         return episode_filter_regex(data=result, regex=self.regex)
 
+    def save(self, tx: Optional[sa.orm.Session] = None) -> None:
+        self.episodes = sorted(set(self.episodes))
+        super().save(tx)
+
 
 class Download(Base):
     __tablename__ = "download"
 
+    STATUS_NOT_DOWNLOAD = 0
+    STATUS_DOWNLOADING = 1
+    STATUS_DOWNLOADED = 2
+
     id: Mapped[int] = Column(Integer, nullable=False, primary_key=True)  # type: ignore
     bangumi_name: Mapped[str] = Column("name", Text, nullable=False)  # type: ignore
     title: Mapped[str] = Column(Text, nullable=False)  # type: ignore
     episode: Mapped[int] = Column(Integer, nullable=False)  # type: ignore
     download: Mapped[str] = Column(Text, nullable=False)  # type: ignore
     status: Mapped[int] = Column(Integer, nullable=False)  # type: ignore
 
+    if TYPE_CHECKING:
+
+        def __init__(
+            self,
+            bangumi_name: str,
+            title: str,
+            episode: int,
+            download: str,
+            status: int,
+            id: Optional[int] = None,
+        ):
+            super().__init__()
+
     @classmethod
-    def get_all_downloads(cls, status: Optional[int] = None) -> List[dict]:
+    def get_all_downloads(cls, status: Optional[int] = None) -> List["Download"]:
         with Session.begin() as session:
             if status is None:
                 sql = sa.select(cls).where().order_by(cls.status)
             else:
                 sql = sa.select(cls).where(cls.status == status).order_by(cls.status)
 
-            return [x.__dict__ for x in session.scalars(sql)]
+            return list(session.scalars(sql).all())
 
     def downloaded(self) -> None:
-        self.status = STATUS_DOWNLOADED
+        self.status = self.STATUS_DOWNLOADED
         self.save()
 
 
 class Subtitle(Base):
     __tablename__ = "subtitle"
 
     id: Mapped[str] = Column(Text, nullable=False, primary_key=True)  # type: ignore
@@ -248,17 +279,23 @@
             return list(session.scalars(sa.select(cls).where(cls.name.in_(name_list))))
 
 
 class Scripts(Base):
     __tablename__ = "scripts"
 
     bangumi_name: Mapped[str] = Column(Text, primary_key=True, nullable=False, unique=True)  # type: ignore
-    episode: Mapped[int] = Column(Integer, nullable=False)  # type: ignore
+    episodes: Mapped[List[str]] = Column(sa.JSON, nullable=False, default=[], server_default="[]")  # type: ignore
     status: Mapped[int] = Column(Integer, nullable=False)  # type: ignore
     updated_time: Mapped[int] = Column(Integer, nullable=False, default=0, server_default="0")  # type: ignore
+    update_day: Mapped[str] = Column(Text, nullable=False, default="Unknown", server_default="Unknown")  # type: ignore
+    cover: Mapped[str] = Column(Text, nullable=False, default="", server_default="")  # type: ignore
+
+    def save(self, tx: Optional[sa.orm.Session] = None) -> None:
+        self.episodes = sorted(set(self.episodes))
+        super().save(tx)
 
 
 def recreate_source_relatively_table() -> None:
     with Session.begin() as session:
         for table in [Subtitle, Download, Followed, Bangumi]:
             session.execute(sa.delete(table))
```

### Comparing `bgmi-5.0.0a2/bgmi/lib/update.py` & `bgmi-5.0.0a3/bgmi/lib/update.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 def update_database() -> None:
     if not old_version_file.exists():
         old_version_file.write_text(__version__, encoding="utf8")
         return
 
     previous = packaging.version.parse(old_version_file.read_text(encoding="utf8").strip())
-    if previous < packaging.version.Version("5.0.0"):
+    if previous < packaging.version.Version("5.0.0a0"):
         print_error(
             (
                 "can't automatically upgrade from <5.0.0 version, "
                 + " please backup your .bgmi files, remove them and use `bgmi install`\n"
                 + RED
                 + "All Data will lost, you will need to re-add your bangumi after re-install"
                 + COLOR_END
```

### Comparing `bgmi-5.0.0a2/bgmi/main.py` & `bgmi-5.0.0a3/bgmi/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import datetime
 import itertools
 import os
 import platform
 import sys
+from collections import defaultdict
 from operator import itemgetter
-from typing import List, Mapping, Optional, Tuple
+from typing import Dict, List, Mapping, Optional, Sequence, Tuple
 
 import click
 import pydantic
 import sqlalchemy as sa
 import tomlkit
 import wcwidth
 from loguru import logger
-from tornado import template
 
 from bgmi import __version__
-from bgmi.config import BGMI_PATH, CONFIG_FILE_PATH, Config, cfg, write_default_config
+from bgmi.config import CONFIG_FILE_PATH, Config, Source, cfg, write_default_config
 from bgmi.lib import controllers as ctl
 from bgmi.lib.constants import BANGUMI_UPDATE_TIME, SPACIAL_APPEND_CHARS, SPACIAL_REMOVE_CHARS, SUPPORT_WEBSITE
-from bgmi.lib.download import download_episodes
+from bgmi.lib.download import download_downloads
 from bgmi.lib.fetch import website
-from bgmi.lib.table import STATUS_DELETED, STATUS_FOLLOWED, STATUS_UPDATED, Bangumi, Followed, Session, Subtitle
+from bgmi.lib.table import Bangumi, Download, Followed, Session, Subtitle, recreate_source_relatively_table
 from bgmi.lib.update import update_database
 from bgmi.script import ScriptRunner
 from bgmi.setup import create_dir, init_db, install_crontab
 from bgmi.utils import (
     COLOR_END,
     GREEN,
     RED,
@@ -61,44 +61,54 @@
 @click.pass_context
 def cli(ctx: click.Context) -> None:
     if ctx.command not in ["install", "upgrade", "complete"]:
         check_update()
 
 
 @cli.command(help="Install BGmi and frontend")
-def install() -> None:
+@click.option("--no-web", is_flag=True, default=False, help="Do not download web static files")
+def install(no_web: bool) -> None:
     need_to_init = False
-    if not os.path.exists(BGMI_PATH):
+    if not CONFIG_FILE_PATH.exists():
         need_to_init = True
-        print_warning(f"BGMI_PATH {BGMI_PATH} does not exist, installing")
 
     create_dir()
     init_db()
     if need_to_init:
         install_crontab()
 
     write_default_config()
     update_database()
-    get_web_admin(method="install")
+
+    if not no_web:
+        get_web_admin(method="install")
 
 
 @cli.command(help="upgrade from previous version")
 def upgrade() -> None:
     create_dir()
     update_database()
     check_update()
 
 
 @cli.command(
     help="Select date source bangumi_moe or mikan_project",
 )
-@click.argument("bangumi_source", required=True, type=click.Choice([x["id"] for x in SUPPORT_WEBSITE]))
-def source(bangumi_source: str) -> None:
-    result = ctl.source(data_source=bangumi_source)
-    globals()["print_{}".format(result["status"])](result["message"])
+@click.argument("source", required=True, type=click.Choice([x["id"] for x in SUPPORT_WEBSITE]))
+def source_cmd(source: str) -> None:
+    if source in list(map(itemgetter("id"), SUPPORT_WEBSITE)):
+        recreate_source_relatively_table()
+        cfg.data_source = Source(source)
+        cfg.save()
+        print_success("data source switch succeeds")
+        print_success(f"you have successfully change your data source to {source}")
+    else:
+        print_error(
+            "please check your input. data source should be one of {}".format([x["id"] for x in SUPPORT_WEBSITE])
+        )
 
 
 @cli.group()
 def config() -> None:
     ...
 
 
@@ -188,50 +198,54 @@
     )
     if result["status"] != "success":
         globals()["print_{}".format(result["status"])](result["message"])
     data = result["data"]
     for i in data:
         print(i.title)
     if download:
-        download_episodes(data)
-
-
-@cli.command("mark")
-@click.argument("name", required=True)
-@click.argument("episode", type=int, required=True)
-def mark(name: str, episode: int) -> None:
-    result = ctl.mark(name=name, episode=episode)
-    globals()["print_{}".format(result["status"])](result["message"])
+        download_downloads(
+            [
+                Download(
+                    bangumi_name=x.name,
+                    episode=x.episode,
+                    status=Download.STATUS_DOWNLOADING,
+                    download=x.download,
+                    title=x.title,
+                )
+                for x in data
+            ]
+        )
 
 
 @cli.command()
 @click.argument("names", nargs=-1)
 @click.option(
     "--episode",
     type=int,
     help="add bangumi and mark it as specified episode",
 )
 @click.option(
-    "--save-path", type=str, help='add config.save_path_map for bangumi, example: "./{bangumi_name}/S1/" "./名侦探柯南/S1/"'
+    "--save-path",
+    type=str,
+    help='add config.save_path_map for bangumi, example: "./{bangumi_name}/S1/" "./名侦探柯南/S1/"',
 )
 def add(names: List[str], episode: Optional[int], save_path: Optional[str]) -> None:
     """
     subscribe bangumi
 
     names: list of bangumi names to subscribe
 
     --save-path 同时修改 config 中的 `save_path_map`。
     """
     for name in names:
         result = ctl.add(name=name, episode=episode)
         globals()["print_{}".format(result["status"])](result["message"])
-        if save_path:
-            if result["status"] in ["success", "warning"]:
-                bangumi = Bangumi.fuzzy_get(name=name)
-                config_set(["save_path_map", bangumi.name], value=save_path.format(bangumi_name=bangumi.name))
+        if save_path and result["status"] in ["success", "warning"]:
+            bangumi = Bangumi.get(Bangumi.name.contains(name))
+            config_set(["save_path_map", bangumi.name], value=save_path.format(bangumi_name=bangumi.name))
 
 
 @cli.command()
 @click.argument("name", nargs=-1)
 @click.option(
     "--clear-all",
     "clear",
@@ -248,18 +262,61 @@
         ctl.delete("", clear_all=clear, batch=yes)
     else:
         for bangumi_name in name:
             result = ctl.delete(name=bangumi_name)
             globals()["print_{}".format(result["status"])](result["message"])
 
 
+def followed_bangumi() -> Dict[str, list]:
+    """
+
+    :return: list of bangumi followed
+    """
+    weekly_list_followed = Bangumi.get_updating_bangumi(status=Followed.STATUS_FOLLOWED)
+    weekly_list_updated = Bangumi.get_updating_bangumi(status=Followed.STATUS_UPDATED)
+    weekly_list = defaultdict(list)
+    for k, v in itertools.chain(weekly_list_followed.items(), weekly_list_updated.items()):
+        weekly_list[k].extend(v)
+    for bangumi_list in weekly_list.values():
+        for bangumi in bangumi_list:
+            bangumi["subtitle_group"] = Subtitle.get_subtitle_by_id(bangumi["subtitle_group"])
+    return weekly_list
+
+
 @cli.command("list", help="list subscribed bangumi")
 def list_command() -> None:
-    result = ctl.list_()
-    print(result["message"])
+    weekday_order = BANGUMI_UPDATE_TIME
+    followed = followed_bangumi()
+
+    script_bangumi = ScriptRunner().get_models_dict()
+
+    if not followed and not script_bangumi:
+        print_warning("you have not subscribed any bangumi")
+        return
+
+    for i in script_bangumi:
+        i["subtitle_group"] = []
+        followed[i["update_day"].lower()].append(i)
+
+    s = ""
+
+    for weekday in weekday_order:
+        if followed[weekday.lower()]:
+            s += f"{GREEN}{weekday}. {COLOR_END}"
+            for j, bangumi in enumerate(followed[weekday.lower()]):
+                if bangumi["status"] in (Followed.STATUS_UPDATED, Followed.STATUS_FOLLOWED) and "episode" in bangumi:
+                    bangumi["name"] = f"{bangumi['name']}({bangumi['episode']:d})"
+                if j > 0:
+                    s += " " * 5
+
+                f = [x.name for x in bangumi["subtitle_group"]]
+
+                s += "{}: {}\n".format(bangumi["name"], ", ".join(f) if f else "<None>")
+
+    print(s)
 
 
 @cli.command("filter", help="set bangumi episode filters")
 @click.argument("name", required=True)
 @click.option("--subtitle", help='Subtitle group name, split by ",".')
 @click.option(
     "--include",
@@ -364,45 +421,48 @@
     row = int(env_columns / col if env_columns / col <= 3 else 3)
 
     def print_line() -> None:
         num = col - 3
         split = "-" * num + "   "
         print(split * row)
 
-    for weekday in weekday_order + ("Unknown",):
+    for weekday in (*weekday_order, "Unknown"):
         if weekly_list[weekday.lower()]:
             print(
                 "{}{}. {}".format(
                     GREEN,
                     weekday if not today else f"Bangumi Schedule for Today ({weekday})",
                     COLOR_END,
                 ),
                 end="",
             )
             print()
             print_line()
+
+            weekly_list[weekday.lower()].sort(key=lambda x: x["episode"] or -999, reverse=True)
+
             for i, bangumi in enumerate(weekly_list[weekday.lower()]):
-                if bangumi["status"] in (STATUS_UPDATED, STATUS_FOLLOWED) and "episode" in bangumi:
+                if bangumi["status"] in (Followed.STATUS_UPDATED, Followed.STATUS_FOLLOWED) and "episode" in bangumi:
                     bangumi["name"] = "{}({:d})".format(bangumi["name"], bangumi["episode"])
 
                 width = wcwidth.wcswidth(bangumi["name"])
                 space_count = col - 2 - width
 
                 for s in SPACIAL_APPEND_CHARS:
                     if s in bangumi["name"]:
                         space_count += bangumi["name"].count(s)
 
                 for s in SPACIAL_REMOVE_CHARS:
                     if s in bangumi["name"]:
                         space_count -= bangumi["name"].count(s)
 
-                if bangumi["status"] == STATUS_FOLLOWED:
+                if bangumi["status"] == Followed.STATUS_FOLLOWED:
                     bangumi["name"] = "{}{}{}".format(YELLOW, bangumi["name"], COLOR_END)
 
-                if bangumi["status"] == STATUS_UPDATED:
+                if bangumi["status"] == Followed.STATUS_UPDATED:
                     bangumi["name"] = "{}{}{}".format(GREEN, bangumi["name"], COLOR_END)
                 try:
                     print(" " + bangumi["name"], " " * space_count, end="")
                 except UnicodeEncodeError:
                     continue
 
                 if (i + 1) % row == 0 or i + 1 == len(weekly_list[weekday.lower()]):
@@ -448,43 +508,77 @@
 
 @cli.command("update", help="Update bangumi calendar and subscribed bangumi episode.")
 @click.argument(
     "names",
     nargs=-1,
 )
 @click.option(
-    "-d", "--download", is_flag=True, default=False, help="Download specified episode of the bangumi when updated"
+    "-d", "--download", type=bool, default=True, help="Download specified episode of the bangumi when updated"
 )
 @click.option(
     "--not-ignore", "not_ignore", is_flag=True, help="Do not ignore the old bangumi detail rows (3 month ago)"
 )
 def update(names: List[str], download: bool, not_ignore: bool) -> None:
     """
     name: optional bangumi name list you want to update
     """
     ctl.update(names, download=download, not_ignore=not_ignore)
 
 
+template = {
+    "nginx.conf": """
+    server {
+    listen 80;
+    server_name { server_name };
+
+    root { front_static_path }{ os_sep };
+    autoindex on;
+    charset utf-8;
+
+    location /bangumi/ {
+        # ~/.bgmi/bangumi/
+        alias {{ save_path }}{{ os_sep }};
+    }
+
+    location /api {
+        proxy_pass http://127.0.0.1:8888;
+    }
+
+    location /resource {
+        proxy_pass http://127.0.0.1:8888;
+    }
+
+    location / {
+        # ~/.bgmi/front_static/;
+        alias { front_static_path }{ os_sep };
+    }
+
+}
+"""
+}
+
+
 @cli.command("gen")
 @click.argument("tpl", type=click.Choice(["nginx.conf"]))
 @click.option("--server-name", "server_name")
 def generate_config(tpl: str, server_name: str) -> None:
-    template_file_path = os.path.join(os.path.dirname(__file__), "others", "nginx.conf")
+    if tpl == "nginx.conf":
+        template_file_path = os.path.join(os.path.dirname(__file__), "others", "nginx.conf")
 
-    with open(template_file_path, encoding="utf8") as template_file:
-        shell_template = template.Template(template_file.read(), autoescape="")
+        with open(template_file_path, encoding="utf8") as template_file:
+            shell_template = template_file.read()
 
-    template_with_content = shell_template.generate(
-        server_name=server_name,
-        os_sep=os.sep,
-        front_static_path=str(cfg.front_static_path.as_posix()),
-        save_path=str(cfg.save_path.as_posix()),
-    )
+        template_with_content = shell_template.format(
+            server_name=server_name,
+            os_sep=os.sep,
+            front_static_path=str(cfg.front_static_path),
+            save_path=str(cfg.save_path),
+        )
 
-    print(template_with_content.decode("utf-8"))
+        print(template_with_content)
 
 
 @cli.command("history", help="list your history of following bangumi")
 def history() -> None:
     m = (
         "January",
         "February",
@@ -496,38 +590,34 @@
         "August",
         "September",
         "October",
         "November",
         "December",
     )
     with Session.begin() as session:
-        data = session.scalars(sa.select(Followed).order_by(Followed.updated_time.asc())).all()
+        data: Sequence[Followed] = session.scalars(sa.select(Followed).order_by(Followed.updated_time.asc())).all()
     bangumi_data = Bangumi.get_updating_bangumi()
     year = None
     month = None
 
     updating_bangumi = list(map(itemgetter("name"), itertools.chain(*bangumi_data.values())))
 
     print("Bangumi Timeline")
     for i in data:
-        if i.status == STATUS_DELETED:
+        if i.status == Followed.STATUS_DELETED:
             slogan = "ABANDON"
             color = RED
+        elif i.bangumi_name in updating_bangumi:
+            slogan = "FOLLOWING"
+            color = YELLOW
         else:
-            if i.bangumi_name in updating_bangumi:
-                slogan = "FOLLOWING"
-                color = YELLOW
-            else:
-                slogan = "FINISHED"
-                color = GREEN
+            slogan = "FINISHED"
+            color = GREEN
 
-        if not i.updated_time:
-            date = datetime.datetime.fromtimestamp(0)
-        else:
-            date = datetime.datetime.fromtimestamp(int(i.updated_time))
+        date = datetime.datetime.fromtimestamp(int(i.updated_time))
 
         if date.year != 1970:
             if date.year != year:
                 print(f"{GREEN}{str(date.year)}{COLOR_END}")
                 year = date.year
 
             if date.year == year and date.month != month:
```

### Comparing `bgmi-5.0.0a2/bgmi/others/me.ricterz.bgmi.plist` & `bgmi-5.0.0a3/bgmi/others/me.ricterz.bgmi.plist`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a2/bgmi/plugin/download.py` & `bgmi-5.0.0a3/bgmi/plugin/download.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,19 +18,14 @@
         """download episode
 
         :param url: torrent url or magnet link
         :param save_path: should passed to downloader, episode info has been joined.
         :return: task id
         """
 
-    @staticmethod
-    @abc.abstractmethod
-    def check_config() -> None:
-        """check current config, don't try to connect."""
-
     @abc.abstractmethod
     def get_status(self, id: str) -> DownloadStatus:
         """status of downloading task"""
 
 
 class MissingDependencyError(Exception):
     def __init__(self, message: str) -> None:
```

### Comparing `bgmi-5.0.0a2/bgmi/script.py` & `bgmi-5.0.0a3/bgmi/script.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import datetime
 import glob
 import os
-import time
 import traceback
 import types
 from importlib.machinery import SourceFileLoader
-from operator import itemgetter
 from typing import Any, Dict, Iterator, List, Optional, Tuple
 
 import sqlalchemy as sa
 
 from bgmi.config import cfg
-from bgmi.lib.download import Episode, download_episodes
 from bgmi.lib.fetch import DATA_SOURCE_MAP
-from bgmi.lib.table import STATUS_FOLLOWED, STATUS_UPDATED, Scripts, Session
-from bgmi.utils import print_info, print_success, print_warning
-from bgmi.website.model import WebsiteBangumi
+from bgmi.lib.table import Followed, Scripts, Session
+from bgmi.utils import print_error, print_info, print_warning
+from bgmi.website.model import Episode, WebsiteBangumi
 
 
 class ScriptRunner:
     _defined = None
     scripts = []  # type: List[ScriptBase]
     download_queue = []  # type: List[Episode]
 
@@ -62,75 +59,49 @@
     def get_models(self) -> List[WebsiteBangumi]:
         m = []
         for s in self.scripts:
             model = s.Model()
             m.append(
                 WebsiteBangumi(
                     name=model.bangumi_name,
-                    update_time=model.update_time,
+                    update_day=model.update_time,
                     id=model.bangumi_name,
                     cover=model.cover,
                 )
             )
         return m
 
     def get_models_dict(self) -> List[dict]:
         return [dict(script.Model()) for script in self.scripts if script.bangumi_name is not None]
 
-    @staticmethod
-    def make_dict(script: "ScriptBase") -> List[Dict[str, Any]]:
-        return [
-            {
-                "name": script.bangumi_name,
-                "title": f"[{script.bangumi_name}][{k}]",
-                "episode": k,
-                "download": v,
-            }
-            for k, v in script.get_download_url().items()
-        ]
-
-    def run(self, return_: bool = True, download: bool = False) -> List[Episode]:
+    def run(self) -> Iterator[Tuple[Scripts, List[Episode]]]:
         for script in self.scripts:
             print_info(f"fetching {script.bangumi_name} ...")
-            download_item = self.make_dict(script)
+
+            try:
+                download_item: List[Episode] = [
+                    Episode(
+                        name=script.bangumi_name,
+                        title=f"[{script.bangumi_name}][{k}]",
+                        episode=k,
+                        download=v,
+                    )
+                    for k, v in script.get_download_url().items()
+                ]
+            except Exception as e:
+                print_error(f"Failed to fetch script items\nerror: {e}", stop=False)
+                continue
 
             script_obj = script.Model().obj
 
             if not download_item:
                 print_info(f"Got nothing, quit script {script}.")
                 continue
 
-            max_episode = max(download_item, key=itemgetter("episode"))
-            episode = max_episode["episode"]
-            episode_range = range(script_obj.episode + 1, episode + 1)
-
-            if episode <= script_obj.episode:
-                continue
-
-            download_queue = []
-            for i in episode_range:
-                for e in download_item:
-                    if i == e["episode"]:
-                        download_queue.append(e)
-
-            print_success(f"{script.bangumi_name} updated, episode: {episode}")
-            script_obj.episode = episode
-            script_obj.status = STATUS_UPDATED
-            script_obj.updated_time = int(time.time())
-            script_obj.save()
-
-            if return_:
-                self.download_queue.extend(Episode(**x) for x in download_queue)
-                continue
-
-            if download:
-                print_success(f"Start downloading of {script}")
-                download_episodes([Episode(**x) for x in download_queue])
-
-        return self.download_queue
+            yield script_obj, download_item
 
     def get_download_cover(self) -> List[str]:
         return [script["cover"] for script in self.get_models_dict()]
 
 
 class ScriptBase:
     class Model:
@@ -152,32 +123,31 @@
         def __init__(self) -> None:
             if self.bangumi_name is not None:
                 with Session.begin() as session:
                     s: Scripts = session.scalar(sa.select(Scripts).where(Scripts.bangumi_name == self.bangumi_name))
                     if not s:
                         s = Scripts(
                             bangumi_name=self.bangumi_name,
-                            episode=0,
-                            status=STATUS_FOLLOWED,
+                            status=Followed.STATUS_FOLLOWED,
                             updated_time=0,
                         )
                         session.add(s)
 
                 self.obj = s
 
         def __iter__(self) -> Iterator[Tuple[str, Any]]:
-            for i in ("bangumi_name", "cover", "update_time"):
-                yield i, getattr(self, i)
-
             # patch for cal
+            yield "bangumi_name", self.bangumi_name
+            yield "cover", self.cover
+            yield "update_day", self.update_time
             yield "name", self.bangumi_name
             yield "status", self.obj.status
             yield "updated_time", self.obj.updated_time
             yield "subtitle_group", []
-            yield "episode", self.obj.episode
+            yield "episode", max(self.obj.episodes) if self.obj.episodes else 0
 
     @property
     def _data(self) -> dict:
         return {
             "bangumi_id": self.Model.bangumi_id,
             "subtitle_list": self.Model.subtitle_list,
             "max_page": int(self.Model.max_page),
@@ -218,24 +188,24 @@
 
         The keys `1`, `2`, `3` is the episode, the value is the url of bangumi.
         :return: dict
         """
         if self.source is not None:
             try:
                 source = DATA_SOURCE_MAP[self.source]()
-            except KeyError:
+            except KeyError as e:
                 raise ValueError(
                     "Script data source is invalid, usable sources: {}".format(", ".join(DATA_SOURCE_MAP.keys()))
-                )
+                ) from e
             ret = {}
             data = source.fetch_episode_of_bangumi(**self._data)
             for i in data:
                 if int(i.episode) not in data:
                     ret[int(i.episode)] = i.download
             return ret
-        else:
-            return {}
+
+        return {}
 
 
 if __name__ == "__main__":
     runner = ScriptRunner()
     runner.run()
```

### Comparing `bgmi-5.0.0a2/bgmi/session.py` & `bgmi-5.0.0a3/bgmi/session.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a2/bgmi/utils/__init__.py` & `bgmi-5.0.0a3/bgmi/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import functools
-import glob
 import gzip
+import itertools
 import json
 import os
 import re
 import struct
 import subprocess
 import sys
 import tarfile
 import time
 import traceback
 from io import BytesIO
 from multiprocessing.pool import ThreadPool
 from pathlib import Path
 from shutil import move, rmtree
-from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, TypeVar
 
 import requests
 import semver
 from anime_episode_parser import parse_episode as _parse_episode
 from loguru import logger
 from requests import Response
 
@@ -146,17 +146,17 @@
                     right,
                     bottom,
                     maxx,
                     maxy,
                 ) = struct.unpack("hhhhHhhhhhh", csbi.raw)
                 sizex = right - left + 1  # type: int
                 return sizex
-            else:
-                cols = int(subprocess.check_output("tput cols"))
-                return cols
+
+            cols = int(subprocess.check_output("tput cols"))
+            return cols
         except Exception:
             return _DEFAULT_TERMINAL_WIDTH
 
 
 FRONTEND_NPM_URL = "https://registry.npmjs.com/bgmi-frontend/"
 
 
@@ -210,29 +210,27 @@
                 print_info("Use 'bgmi install' to install BGmi frontend / download delegate")
             if not mark:
                 update()
                 raise SystemExit
         except Exception as e:
             print_warning(f"Error occurs when checking update, {str(e)}")
 
-    version_file = os.path.join(BGMI_PATH, "version")
-    if not os.path.exists(version_file):
-        with open(version_file, "w", encoding="utf8") as f:
+    version_file = BGMI_PATH.joinpath("version")
+    if not version_file.exists():
+        with version_file.open("w", encoding="utf8") as f:
             f.write(str(int(time.time())))
         update()
 
-    with open(version_file, encoding="utf8") as f:
-        try:
-            data = int(f.read())
-            if time.time() - 7 * 24 * 3600 > data:
-                with open(version_file, "w", encoding="utf8") as f:
-                    f.write(str(int(time.time())))
-                update()
-        except ValueError:
-            pass
+    try:
+        data = int(version_file.read_text(encoding="utf8"))
+        if time.time() - 7 * 24 * 3600 > data:
+            version_file.write_text(str(int(time.time())), encoding="utf8")
+            update()
+    except ValueError:
+        pass
 
 
 def parse_episode(episode_title: str) -> int:
     s, c = _parse_episode(episode_title)
     if c != 1:
         return 0
 
@@ -251,16 +249,16 @@
     url = url.replace("http://", "http/").replace("https://", "https/")
     illegal_char = [":", "*", "?", '"', "<", ">", "|", "'"]
     for char in illegal_char:
         url = url.replace(char, "")
 
     if url.startswith("/"):
         return url[1:]
-    else:
-        return url
+
+    return url
 
 
 def bangumi_save_path(bangumi_name: str) -> Path:
     name = normalize_path(bangumi_name)
 
     r = cfg.save_path_map.get(name)
     if r is None:
@@ -290,15 +288,15 @@
     tar = session.get(tar_url, timeout=60)
     tar.raise_for_status()
     admin_zip = BytesIO(tar.content)
     with gzip.GzipFile(fileobj=admin_zip) as f:
         tar_file = BytesIO(f.read())
 
     rmtree(cfg.front_static_path)
-    os.makedirs(cfg.front_static_path)
+    cfg.front_static_path.mkdir(parents=True, exist_ok=True)
 
     with tarfile.open(fileobj=tar_file) as tar_file_obj:
         tar_file_obj.extractall(path=cfg.front_static_path)
 
     for file in os.listdir(os.path.join(cfg.front_static_path, "package", "dist")):
         move(
             os.path.join(cfg.front_static_path, "package", "dist", file),
@@ -326,30 +324,45 @@
     dir_path = os.path.dirname(file_path)
 
     return dir_path, file_path
 
 
 def download_file(url: str) -> Optional[Response]:
     logger.debug("downloading {}", url)
-    if url.startswith("https://") or url.startswith("http://"):
+    if url.startswith(("https://", "http://")):
         print_info(f"Download: {url}")
         return session.get(url, timeout=60)
     return None
 
 
+T = TypeVar("T")
+
+
+def chunks(iterable: Iterable[T], size: int) -> Iterable[Iterable[T]]:
+    it = iter(iterable)
+    chunk = tuple(itertools.islice(it, size))
+    while chunk:
+        yield chunk
+        chunk = tuple(itertools.islice(it, size))
+
+
 def download_cover(cover_url_list: List[str]) -> None:
-    p = ThreadPool(4)
-    content_list = p.map(download_file, cover_url_list)
+    p = ThreadPool(3)
+    content_list = []
+
+    for chunk in chunks(cover_url_list, 9):
+        content_list.extend(p.map(download_file, chunk))
     p.close()
+
     for index, r in enumerate(content_list):
         if not r:
             continue
 
         dir_path, file_path = convert_cover_url_to_path(cover_url_list[index])
-        if not glob.glob(dir_path):
+        if not os.path.exists(dir_path):
             os.makedirs(dir_path)
         with open(file_path, "wb") as f:
             f.write(r.content)
 
 
 def episode_filter_regex(data: List[Episode], regex: Optional[str] = None) -> List[Episode]:
     """
```

### Comparing `bgmi-5.0.0a2/bgmi/website/bangumi_moe.py` & `bgmi-5.0.0a3/bgmi/website/bangumi_moe.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     for bangumi_item in data:
         subtitle_of_bangumi = process_subtitle(subtitle.get(bangumi_item["tag_id"], []))
         item = {
             "status": 0,
             "subtitle_group": [SubtitleGroup(id=id, name=name) for id, name in subtitle_of_bangumi.items()],
             "name": name[bangumi_item["tag_id"]],
             "id": bangumi_item["tag_id"],
-            "update_time": bangumi_update_time_known[(bangumi_item["showOn"] + 7) % 7],
+            "update_day": bangumi_update_time_known[(bangumi_item["showOn"] + 7) % 7],
             "cover": COVER_URL + bangumi_item["cover"],
         }
 
         if item["name"] is None:
             item["name"] = bangumi_item["name"]
 
         weekly_list.append(item)
```

### Comparing `bgmi-5.0.0a2/bgmi/website/base.py` & `bgmi-5.0.0a3/bgmi/website/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 from collections import defaultdict
 from typing import Any, List, Optional, TypeVar
 
 import sqlalchemy as sa
 
 from bgmi.config import cfg
-from bgmi.lib.table import STATUS_UPDATING, Bangumi, Followed, NotFoundError, Session, Subtitle
+from bgmi.lib.table import Bangumi, Followed, NotFoundError, Session, Subtitle
 from bgmi.utils import parse_episode
 from bgmi.website.model import Episode, WebsiteBangumi
 
 T = TypeVar("T", bound=dict)
 
 
 class BaseWebsite:
@@ -20,27 +20,27 @@
         """save bangumi to database"""
         with Session.begin() as session:
             subtitle_group = sorted([x.id for x in data.subtitle_group])
             try:
                 b = Bangumi.get(Bangumi.id == data.id)
 
                 b.cover = data.cover
-                b.update_time = data.update_time
-                b.status = STATUS_UPDATING
+                b.update_day = data.update_day
+                b.status = Bangumi.STATUS_UPDATING
                 b.subtitle_group = subtitle_group
 
                 session.add(b)
             except NotFoundError:
                 session.add(
                     Bangumi(
                         name=data.name,
                         id=data.id,
-                        update_time=data.update_time,
+                        update_day=data.update_day,
                         cover=data.cover,
-                        status=STATUS_UPDATING,
+                        status=Bangumi.STATUS_UPDATING,
                         subtitle_group=subtitle_group,
                     )
                 )
 
         for subtitle in data.subtitle_group:
             with Session.begin() as session:
                 s = session.scalar(sa.select(Subtitle).where(Subtitle.id == subtitle.id))
@@ -58,15 +58,15 @@
         Bangumi.delete_all()
         for bangumi in bangumi_result:
             self.save_bangumi(bangumi)
 
         if group_by_weekday:
             result_group_by_weekday = defaultdict(list)
             for bangumi in bangumi_result:
-                result_group_by_weekday[bangumi.update_time.lower()].append(bangumi)
+                result_group_by_weekday[bangumi.update_day.lower()].append(bangumi)
             return result_group_by_weekday
         return bangumi_result
 
     def get_maximum_episode(
         self,
         bangumi: Bangumi,
         ignore_old_row: bool = True,
```

### Comparing `bgmi-5.0.0a2/bgmi/website/mikan.py` & `bgmi-5.0.0a3/bgmi/website/mikan.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import datetime
 import time
 from collections import defaultdict
 from typing import List, Optional
 from xml.etree import ElementTree
 
 import bs4
@@ -50,18 +51,16 @@
     network
     """
     r = get_text(server_root)
     soup = bs4.BeautifulSoup(r, "html.parser")
     for day_of_week in [x for x in range(0, 9) if x != 7]:
         d = soup.find("div", attrs={"class": "sk-bangumi", "data-dayofweek": str(day_of_week)})
         if d:
-            try:
+            with contextlib.suppress(KeyError):
                 yield _CN_WEEK[_DAY_OF_WEEK[day_of_week]], d
-            except KeyError:
-                pass
 
 
 def parse_episodes(content, bangumi_id, subtitle_list=None) -> List[Episode]:
     result = []
     soup = BeautifulSoup(content, "html.parser")
     container = soup.find("div", class_="central-container")  # type:bs4.Tag
     episode_container_list = {}
@@ -74,17 +73,16 @@
         if class_names is not None and "episode-expand" in class_names:
             expand_subtitle_map[tag.attrs.get("data-subtitlegroupid", None)] = True
 
         subtitle_id = tag.attrs.get("id", False)
         if subtitle_list:
             if subtitle_id in subtitle_list:
                 episode_container_list[tag.attrs.get("id", None)] = tag.find_next_sibling("table")
-        else:
-            if subtitle_id:
-                episode_container_list[tag.attrs.get("id", None)] = tag.find_next_sibling("table")
+        elif subtitle_id:
+            episode_container_list[tag.attrs.get("id", None)] = tag.find_next_sibling("table")
 
     for subtitle_id, container in episode_container_list.items():
         _container = container
         if subtitle_id in expand_subtitle_map:
             expand_r = requests.get(
                 bangumi_episode_expand_api,
                 params={
@@ -97,21 +95,19 @@
             _container = expand_soup.find("table")
 
         for tr in _container.find_all("tr")[1:]:
             title = tr.find("a", class_="magnet-link-wrap").text
             time_string = tr.find_all("td")[2].string
             result.append(
                 Episode(
-                    **{
-                        "download": server_root[:-1] + tr.find_all("td")[-1].find("a").attrs.get("href", ""),
-                        "subtitle_group": str(subtitle_id),
-                        "title": title,
-                        "episode": parse_episode(title),
-                        "time": int(time.mktime(time.strptime(time_string, "%Y/%m/%d %H:%M"))),
-                    }
+                    download=server_root[:-1] + tr.find_all("td")[-1].find("a").attrs.get("href", ""),
+                    subtitle_group=str(subtitle_id),
+                    title=title,
+                    episode=parse_episode(title),
+                    time=int(time.mktime(time.strptime(time_string, "%Y/%m/%d %H:%M"))),
                 )
             )
 
     return result
 
 
 def parser_day_bangumi(soup) -> List[WebsiteBangumi]:
@@ -158,16 +154,15 @@
         return requests.get(url, params=params).text
 
     for _ in range(2):
         r = requests.get(url, params=params)
         if r.headers.get("content-type").startswith("text/html"):
             if "退出" in r.text:
                 return r.text
-            else:
-                mikan_login()
+            mikan_login()
         else:
             return r.text
 
     raise ValueError("mikan login failed")
 
 
 class Mikanani(BaseWebsite):
@@ -276,22 +271,22 @@
             else:
                 best_sim_match_group = (subgroup, subgroup_names, subgroup_links, sub_info)
                 break
 
         if not best_sim_match_group:
             return []
         subgroup, subgroup_names, subgroup_links, sub_info = best_sim_match_group
-        bangumiId, subgroupid = sub_info["bangumiId"], sub_info["subgroupid"]
-        rss_url = f"{server_root}RSS/Bangumi?bangumiId={bangumiId}&subgroupid={subgroupid}"
+        bangumi_id, subgroup_id = sub_info["bangumiId"], sub_info["subgroupid"]
+        rss_url = f"{server_root}RSS/Bangumi?bangumiId={bangumi_id}&subgroupid={subgroup_id}"
 
         subtitle_group = " ".join(subgroup_names)
         if subtitle:
-            print_info(f"Matched subtitle: {subtitle_group} ({subgroupid})")
+            print_info(f"Matched subtitle: {subtitle_group} ({subgroup_id})")
         else:
-            print_info(f"Use first subtitle: {subtitle_group} ({subgroupid})")
+            print_info(f"Use first subtitle: {subtitle_group} ({subgroup_id})")
 
         r = get_text(rss_url)
         rss_root = ElementTree.fromstring(r)
 
         result = []
         for item in rss_root[0].findall("item"):
             link_el = item.find("link")
@@ -327,34 +322,32 @@
         s = BeautifulSoup(r, "html.parser")
         td_list = s.find_all("tr", attrs={"class": "js-search-results-row"})
         for tr in td_list:
             title = tr.find("a", class_="magnet-link-wrap").text
             time_string = tr.find_all("td")[2].string
             result.append(
                 Episode(
-                    **{
-                        "download": tr.find("a", class_="magnet-link").attrs.get("data-clipboard-text", ""),
-                        "name": keyword,
-                        "title": title,
-                        "episode": self.parse_episode(title),
-                        "time": int(time.mktime(time.strptime(time_string, "%Y/%m/%d %H:%M"))),
-                    }
+                    download=tr.find("a", class_="magnet-link").attrs.get("data-clipboard-text", ""),
+                    name=keyword,
+                    title=title,
+                    episode=self.parse_episode(title),
+                    time=int(time.mktime(time.strptime(time_string, "%Y/%m/%d %H:%M"))),
                 )
             )
         return result
 
     def fetch_episode_of_bangumi(self, bangumi_id, max_page=cfg.max_path, subtitle_list=None):
         r = get_text(server_root + f"Home/Bangumi/{bangumi_id}")
         return parse_episodes(r, bangumi_id, subtitle_list)
 
     def fetch_bangumi_calendar(self) -> List[WebsiteBangumi]:
         bangumi_list = []
         for update_time, day in get_weekly_bangumi():
             for obj in parser_day_bangumi(day):
-                obj.update_time = update_time
+                obj.update_day = update_time
                 obj.cover = obj.cover.split("?")[0]
                 bangumi_list.append(obj)
         return bangumi_list
 
     def fetch_single_bangumi(
         self,
         bangumi_id: str,
@@ -363,11 +356,11 @@
     ) -> Optional[WebsiteBangumi]:
         html = get_text(server_root + f"Home/Bangumi/{bangumi_id}")
         info = self.parse_bangumi_details_page(html)
         return WebsiteBangumi(
             name=info["name"],
             id=bangumi_id,
             status=info["status"],
-            update_time=info["update_time"],
+            update_day=info["update_time"],
             subtitle_group=info["subtitle_group"],
             episodes=parse_episodes(html, bangumi_id, subtitle_list),
         )
```

### Comparing `bgmi-5.0.0a2/bgmi/website/model.py` & `bgmi-5.0.0a3/bgmi/website/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 
 
 class Episode(BaseModel):
     title: str
     download: str
     episode: int = 0
     time: int = 0
-    subtitle_group: Optional[str]
+    subtitle_group: Optional[str] = None
     name: str = ""
 
+    class Config:
+        orm_mode = True
+
     @staticmethod
     def remove_duplicated_bangumi(result: List["Episode"]) -> List["Episode"]:
         ret = []
         episodes = list({i.episode for i in result})
         for i in result:
             if i.episode in episodes:
                 ret.append(i)
@@ -34,23 +37,22 @@
 class SubtitleGroup(BaseModel):
     id: str
     name: str
 
 
 class WebsiteBangumi(BaseModel):
     id: str
-    update_time: str = "Unknown"
+    update_day: str = "Unknown"
     name: str = ""
     status: int = 0
     subtitle_group: List[SubtitleGroup] = []
     cover: str = ""
     episodes: List[Episode] = []
 
     @property
     def max_episode(self) -> int:
         return max(self.episodes, key=attrgetter("episode")).episode
 
-    @validator("update_time")
-    def validate_update_time(cls, v: str) -> str:
-        # pylint: disable=no-self-argument
+    @validator("update_day")
+    def validate_update_time(cls, v: str) -> str:  # noqa: N805
         assert v in BANGUMI_UPDATE_TIME, f"update time can be only one of {BANGUMI_UPDATE_TIME}"
         return v
```

### Comparing `bgmi-5.0.0a2/bgmi/website/share_dmhy.py` & `bgmi-5.0.0a3/bgmi/website/share_dmhy.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,23 +46,23 @@
         bs = BeautifulSoup(subtitle_raw, "html.parser")
         a_list = bs.find_all("a")
 
         for a in a_list:
             subtitle_group_name = a.get_text(strip=True)
             subtitle_group_id_raw = re.findall("team_id%3A(.+)$", a["href"])
 
-            if (len(subtitle_group_id_raw) == 0) or subtitle_group_name == "":
+            if (not subtitle_group_id_raw) or not subtitle_group_name:
                 continue
 
             subtitle_group_id = subtitle_group_id_raw[0]
 
             bangumi.subtitle_group.append(SubtitleGroup(id=subtitle_group_id, name=subtitle_group_name))
 
         bangumi.name = name
-        bangumi.update_time = update_time
+        bangumi.update_day = update_time
         bangumi.id = keyword
         bangumi.cover = base_url + cover
 
         # append to bangumi_list
         bangumi_list.append(bangumi)
 
     return bangumi_list
@@ -74,15 +74,15 @@
     bs = BeautifulSoup(content, "html.parser")
     li_list = bs.find_all("li", {"class": "team-item"})
 
     for li in li_list:
         subtitle_group_name = li.span.a.get("title")
         subtitle_group_id_raw = re.findall(r"team_id\/(.+)$", li.span.a.get("href"))
 
-        if (len(subtitle_group_id_raw) == 0) or subtitle_group_name == "":
+        if (not subtitle_group_id_raw) or not subtitle_group_name:
             continue
 
         subtitle_group_id = subtitle_group_id_raw[0]
         # append to subtitle_list
         subtitle_list.append({"id": subtitle_group_id, "name": subtitle_group_name})
 
     return subtitle_list
@@ -178,16 +178,16 @@
 
         bangumi_list = []
 
         url = base_url + "/cms/page/name/programme.html"
 
         r = fetch_url(url)
 
-        for update_time, array_name in week_days_mapping:
-            b_list = parse_bangumi_with_week_days(r, update_time, array_name)
+        for update_day, array_name in week_days_mapping:
+            b_list = parse_bangumi_with_week_days(r, update_day, array_name)
             bangumi_list.extend(b_list)
 
         return bangumi_list
 
     def search_by_tag(self, tag: str, subtitle: Optional[str] = None, count: Optional[int] = None) -> List[Episode]:
         print_error("dmhy not support search by tag")
         return []
@@ -254,17 +254,16 @@
                         continue
 
                     team_id_raw = re.findall(r"team_id\/(.*)$", href)
                     if len(team_id_raw) == 0:
                         continue
                     subtitle_group = team_id_raw[0]
 
-                if subtitle_list:
-                    if subtitle_group not in subtitle_list:
-                        continue
+                if subtitle_list and subtitle_group not in subtitle_list:
+                    continue
 
                 if os.environ.get("DEBUG", False):  # pragma: no cover
                     print(name, title, subtitle_group, download, episode, t)
 
                 result.append(
                     Episode(
                         title=title,
```

### Comparing `bgmi-5.0.0a2/pyproject.toml` & `bgmi-5.0.0a3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "bgmi"
-version = "5.0.0-alpha.2"
+version = "5.0.0-alpha.3"
 description = 'BGmi is a cli tool for subscribed bangumi.'
 authors = ["RicterZ <ricterzheng@gmail.com>"]
 readme = 'README.md'
 license = 'MIT'
 maintainers = ["Trim21 <i@trim21.me>"]
 homepage = 'https://github.com/BGmi/BGmi'
 repository = 'https://github.com/BGmi/BGmi'
@@ -39,58 +39,61 @@
 [tool.poetry.plugins] # entry-points
 
 [tool.poetry.plugins."bgmi.downloader"]
 "aria2-rpc" = 'bgmi.downloader:Aria2DownloadRPC'
 "transmission-rpc" = 'bgmi.downloader:TransmissionRPC'
 "deluge-rpc" = 'bgmi.downloader:DelugeRPC'
 "qbittorrent-webapi" = 'bgmi.downloader:QBittorrentWebAPI'
+"noop" = 'bgmi.downloader:Noop'
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
 beautifulsoup4 = '==4.12.0'
 requests = { extras = ["socks"], version = "2.28.2" }
-tornado = '==6.2'
 icalendar = '==5.0.4'
-sqlalchemy = "2.0.8"
+sqlalchemy = "2.0.9"
 wcwidth = "^0.2.6"
 pydantic = "==1.10.7"
 stevedore = "==5.0.0"
 filetype = "1.2.0"
 strsimpy = "0.2.1"
 tomlkit = "0.11.7"
 strenum = "0.4.10"
 anime-episode-parser = "^0.0.8"
 semver = "3.0.0"
 loguru = "0.6.0"
 click = "8.1.3"
+packaging = "23.0"
+uvicorn = { extras = ["standard"], version = "0.21.1" }
+fastapi = "0.95.0"
 # RPC library
 transmission-rpc = "==4.1.5"
 qbittorrent-api = "==2023.3.44"
-packaging = "23.0"
 
 [tool.poetry.group.dev.dependencies]
 # tests
 coverage = { version = "==7.2.2", extras = ['toml'] }
 pytest = "==7.2.2"
 pytest-github-actions-annotate-failures = "==0.1.8"
 requests-cache = "==1.0.1"
+httpx = "0.23.3"
 # lint
 pre-commit = '==3.2.2'
-mypy = "==1.1.1"
+mypy = "1.2.0"
 flake8 = { version = "==6.0.0", python = "^3.9" }
 flake8-comprehensions = "==3.11.1"
-flake8-bugbear = { version = "==23.3.23", python = '^3.9' }
 flake8-mutable = "1.2.0"
 flake8-pep3101 = "==2.0.0"
 flake8-2020 = "==1.7.0"
 flake8-pytest-style = "==1.7.2"
 flake8-pyproject = "1.2.3"
-pylint = "==2.17.2"
 # stubs
 types-requests = "==2.28.11.17"
+ruff = "0.0.261"
+
 [tool.coverage.report]
 exclude_lines = [
   'pragma: no cover',
   'if TYPE_CHECKING:',
   'if __name__ == "__main__":',
   'if typing.TYPE_CHECKING:',
   'raise NotImplementedError',
@@ -127,64 +130,141 @@
   "bgmi.downloader.*",
   "bgmi.website.mikan",
   "bgmi.website.bangumi_moe",
   "bgmi.website.share_dmhy",
 ]
 disallow_untyped_defs = false
 
-[tool.pylint]
-
-[tool.pylint.TYPECHECK]
-ignored-classes = ['sqlalchemy.orm.session.sessionmaker']
-
-[tool.pylint.format]
-max-line-length = 120
-
-[tool.pylint.messages_control]
-extension-pkg-whitelist = ['pydantic']
-disable = [
-  'fixme',
-  "consider-using-f-string",
-  "cell-var-from-loop",
-  "missing-function-docstring",
-  "missing-class-docstring",
-  "missing-module-docstring",
-  'raise-missing-from',
-  'invalid-name',
-  'too-many-locals',
-  'duplicate-code',
-  'too-few-public-methods',
-  'unused-argument',
-  'no-else-return',
-  'assignment-from-none',
-  'unused-variable',
-  'broad-except',
-  'too-many-nested-blocks',
-  'too-many-branches',
-  'redefined-outer-name',
-  'too-many-return-statements',
-  'too-many-statements',
-  'too-many-arguments',
-  'not-an-iterable',
-  'redefined-builtin',
-]
-
 [tool.black]
 line-length = 120
 target-version = ['py38', 'py39', 'py310']
 
 
 [tool.flake8]
 max-line-length = 120
-ignore = ['W503', 'E203']
+ignore = ['W503', 'E203', 'PT004']
 
-exclude = [
-  '.git',
-  '__pycache__',
-  '.venv',
-  'build',
-  'dist',
+exclude = ['.git', '__pycache__', '.venv', 'build', 'dist']
+
+per-file-ignores = ['bgmi/lib/constants.py:C408', 'bgmi/front/routes.py:B008']
+
+[tool.ruff]
+select = [
+  "B",
+  "C",
+  "E",
+  "F",
+  "G",
+  "I",
+  "N",
+  "Q",
+  "S",
+  "W",
+  "BLE",
+  "DJ",
+  "ERA",
+  "EXE",
+  "ICN",
+  "INP",
+  "ISC",
+  "NPY",
+  #  "DTZ",
+  #  "PTH",
+  "PD",
+  "PGH",
+  "PIE",
+  "PL",
+  "PT",
+  "PYI",
+  "RET",
+  "RSE",
+  "RUF",
+  "SIM",
+  "SLF",
+  "TCH",
+  "TID",
+  "TRY",
+  "YTT",
+]
+ignore = [
+  'BLE001',
+  'S301',
+  'S314',
+  'S101',
+  'N815',
+  'S104',
+  'C901',
+  'ISC003',
+  'PLR0913',
+  'I001',
+  'RUF001',
+  'SIM108',
+  'TCH003',
+  'RUF003',
+  'RET504',
+  'TRY300',
+  'TRY003',
+  'TRY201',
+  'TRY301',
+  'PLR0912',
+  'PLR0915',
+  'PLR2004',
+  'PGH003',
 ]
 
-per-file-ignores = [
-  'bgmi/lib/constants.py:C408'
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+fixable = [
+  "A",
+  "B",
+  "C",
+  "E",
+  "F",
+  "G",
+  "I",
+  "N",
+  "Q",
+  "S",
+  "W",
+  "BLE",
+  "DJ",
+  "DTZ",
+  "EM",
+  "ERA",
+  "EXE",
+  "FBT",
+  "ICN",
+  "INP",
+  "ISC",
+  "NPY",
+  "PD",
+  "PGH",
+  "PIE",
+  "PL",
+  "PT",
+  "PTH",
+  "PYI",
+  "RET",
+  "RSE",
+  "RUF",
+  "SIM",
+  "SLF",
+  "TCH",
+  "TID",
+  "TRY",
+  "YTT",
 ]
+unfixable = []
+
+
+# Same as Black.
+line-length = 120
+
+# Assume Python 3.10.
+target-version = "py38"
+
+[tool.ruff.mccabe]
+# Unlike Flake8, default to a complexity level of 10.
+max-complexity = 10
+
+[tool.ruff.per-file-ignores]
+'bgmi/lib/constants.py' = ['C408']
+'bgmi/front/routes.py' = ['B008']
```

### Comparing `bgmi-5.0.0a2/PKG-INFO` & `bgmi-5.0.0a3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgmi
-Version: 5.0.0a2
+Version: 5.0.0a3
 Summary: BGmi is a cli tool for subscribed bangumi.
 Home-page: https://github.com/BGmi/BGmi
 License: MIT
 Keywords: bangumi,bgmi,feed
 Author: RicterZ
 Author-email: ricterzheng@gmail.com
 Maintainer: Trim21
@@ -25,29 +25,30 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: anime-episode-parser (>=0.0.8,<0.0.9)
 Requires-Dist: beautifulsoup4 (==4.12.0)
 Requires-Dist: click (==8.1.3)
+Requires-Dist: fastapi (==0.95.0)
 Requires-Dist: filetype (==1.2.0)
 Requires-Dist: icalendar (==5.0.4)
 Requires-Dist: loguru (==0.6.0)
 Requires-Dist: packaging (==23.0)
 Requires-Dist: pydantic (==1.10.7)
 Requires-Dist: qbittorrent-api (==2023.3.44)
 Requires-Dist: requests[socks] (==2.28.2)
 Requires-Dist: semver (==3.0.0)
-Requires-Dist: sqlalchemy (==2.0.8)
+Requires-Dist: sqlalchemy (==2.0.9)
 Requires-Dist: stevedore (==5.0.0)
 Requires-Dist: strenum (==0.4.10)
 Requires-Dist: strsimpy (==0.2.1)
 Requires-Dist: tomlkit (==0.11.7)
-Requires-Dist: tornado (==6.2)
 Requires-Dist: transmission-rpc (==4.1.5)
+Requires-Dist: uvicorn[standard] (==0.21.1)
 Requires-Dist: wcwidth (>=0.2.6,<0.3.0)
 Project-URL: Repository, https://github.com/BGmi/BGmi
 Description-Content-Type: text/markdown
 
 # BGmi
 
 BGmi 是一个用来追番的命令行程序.
@@ -58,14 +59,20 @@
 [![](https://codecov.io/gh/BGmi/BGmi/branch/master/graph/badge.svg)](https://codecov.io/gh/BGmi/BGmi/branch/master/graph/badge.svg)
 [![](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/BGmi/BGmi/blob/master/LICENSE)
 
 ## TODO
 
 ## 更新日志
 
+### V5
+
+- 为 `bgmi update` 命令默认启用 `--download` 参数
+- 重构 bgmi_http
+- 移除 '/resource/feed.xml'
+
 ### v4
 
 - 添加 `proxy` 设置
 - 新 WEB UI
 - 将配置项 `transmission.rpc_url` 重命名为 `transmission.rpc_host`.
 - 修复 Transmission 配置的默认值.
 
@@ -82,19 +89,20 @@
 - 停止支持 python2，3.4 和 3.5
 - Transmission rpc 认证设置
 - 支持 [deluge-rpc](https://www.deluge-torrent.org/)
 - 使用最大和最小集数筛选搜索结果
 
 ## 特性
 
-- 多个数据源可选: [bangumi_moe](https://bangumi.moe), [mikan_project](https://mikanani.me) 或者[dmhy](https://share.dmhy.org/)
+- 多个数据源可选: [bangumi_moe](https://bangumi.moe), [mikan_project](https://mikanani.me)
+  或者[dmhy](https://share.dmhy.org/)
 - 使用 aria2, transmission, qbittorrent 或者 deluge 来下载你的番剧.
 - 提供一个管理和观看订阅番剧的前端.
 - 弹幕支持
-- 提供 uTorrent 支持的 RSS Feed 和移动设备支持的 ICS 格式日历.
+- 提供移动设备支持的 ICS 格式日历.
 - Bangumi Script: 添加自己的番剧解析器
 - 番剧放松列表和剧集信息
 - 下载番剧时的过滤器(支持关键词,字幕组和正则)
 - 多平台支持: Windows, macOS 以及 Linux
 
 ![](./images/bgmi_cli.png?raw=true)
 ![](https://github.com/BGmi/BGmi-frontend/raw/master/.github/images/example.png)
@@ -161,14 +169,15 @@
 **`--help`选项同样适用于所有的子命令，readme 仅介绍了一些基础用法。**
 
 ## 配置 BGmi
 
 BGmi 提供两种方式配置BGmi的各项运行参数，分别为配置文件与环境变量。
 
 ### 配置文件
+
 bgmi 的配置文件位于 `${BGMI_PATH}/config.toml`, 在未设置 `BGMI_PATH` 环境变量时，`${BGMI_PATH}` 默认为 `~/.bgmi/`。
 
 查看当前 `BGmi` 设置:
 
 ```bash
 bgmi config # 查看当前各项设置默认值.
 ```
@@ -181,19 +190,19 @@
 max_path = 3 # 抓取数据时每个番剧最大抓取页数
 bangumi_moe_url = "https://bangumi.moe"
 share_dmhy_url = "https://share.dmhy.org"
 mikan_username = "" # 蜜柑计划的用户名
 mikan_password = "" # 蜜柑计划的密码
 enable_global_filters = true
 global_filters = [
-    "Leopard-Raws",
-    "hevc",
-    "x265",
-    "c-a Raws",
-    "U3-Web",
+  "Leopard-Raws",
+  "hevc",
+  "x265",
+  "c-a Raws",
+  "U3-Web",
 ]
 
 proxy = '' # http proxy example: http://127.0.0.1:1080
 
 [save_path_map] # 针对每部番剧设置下载路径
 '致不灭的你 第二季' = '/home/trim21/downloads/bangumi/致不灭的你/s2/' # 如果使用绝对路径，可能导致 web-ui 无法正确显示视频文件。
 '致不灭的你 第三季' = './致不灭的你/s3/' # 以 save_path 为基础路径的相对路径
@@ -223,36 +232,40 @@
 
 [deluge]
 rpc_url = "http://127.0.0.1:8112/json"
 rpc_password = "deluge"
 ```
 
 ### 环境变量
+
 当 BGmi 的配置文件还未初始化时，各项运行参数可由环境变量进行配置
 
 环境变量以 `BGMI_` 开头，全大写命名，且各级配置以 `_` 进行分割，如:
+
 ```
 BGMI_DATA_SOURCE=bangumi_moe    # 对应配置文件中的 data_source = "bangumi_moe"
 BGMI_HTTP_ADMIN_TOKEN=dYMj-Z4bDRoQfd3x    # 对应配置文件 [http] 分段中的 admin_token = "dYMj-Z4bDRoQfd3x"
 ...
 ```
 
 环境变量 *暂不支持* 配置以下项目
+
 ```
 enable_global_include_keywords
 enable_global_filters
 global_include_keywords
 global_filters
 [save_path_map]
 ```
+
 注: 当配置文件生成完毕后，运行配置将会以配置文件为准，环境变量仅用于生成第一份配置文件。
 
 ## 修改配置
 
-使用 `bgmi config set ...keys  --value '...'` 命令可以修改配置。
+使用 `bgmi config set ...keys --value '...'` 命令可以修改配置。
 
 如：
 
 ```shell
 bgmi config set http admin_token --value 'my super secret token'
 ```
 
@@ -277,15 +290,14 @@
 
 **如果更换的源为 `mikan_project`, 请先配置 `MIKAN_USERNAME` 和 `MIKAN_PASSWORD`**, 其它源不受影响
 
 ```bash
 bgmi source mikan_project
 ```
 
-
 ### 设置下载方式
 
 修改配置文件和对应的配置项
 
 ```toml
 download_delegate = "aria2-rpc" # download delegate
 ```
@@ -336,25 +348,23 @@
 bgmi filter "Re:CREATORS" --subtitle "" --include "" --exclude "" --regex "..."
 bgmi filter "Re:CREATORS" --regex "(DHR動研字幕組|豌豆字幕组).*(720P)"
 bgmi fetch "Re:CREATORS"
 ```
 
 ## 设置全局过滤关键词
 
-
 ### 包含
 
 默认不启用全局包含关键词，你可以设置 `enable_global_include_keywords = true` 启动此功能。
 
 ```toml
 enable_global_include_keywords = true
 global_include_keywords = ['1080']
 ```
 
-
 ### 排除
 
 有一些默认定义的全局过滤关键词，默认会排除标题包含以下关键词的种子。
 可以使用 `enable_global_filters = false` 禁止过滤全局关键词，
 
 ```toml
 enable_global_filters = true
@@ -386,15 +396,15 @@
 
 `bgmi search`命令默认不会显示重复的集数, 如果要显示重复的集数来方便过滤, 在命令后加上`--dupe`来显示全部的搜索结果
 
 手动修改最近下载的剧集
 
 ```bash
 bgmi list
-bgmi mark "Re:CREATORS" 1
+bgmi mark "Re:CREATORS" --episode 1
 ```
 
 ## 使用`bgmi_http`
 
 1.先下载所有更新中番剧的封面
 
 ```bash
@@ -466,15 +476,16 @@
 
 [me.ricterz.bgmi.plist](https://github.com/BGmi/BGmi/blob/master/bgmi/others/me.ricterz.bgmi.plist)
 
 ## 弹幕支持
 
 BGmi 使用[`DPlayer`](https://github.com/DIYgod/DPlayer)做为前端播放器
 
-如果你想要添加弹幕支持, 在这里[DPlayer#related-projects](https://github.com/DIYgod/DPlayer#related-projects)选择一个后端自行搭建, 或者使用`DPlayer`提供的现成接口`https://api.prprpr.me/dplayer/`
+如果你想要添加弹幕支持, 在这里[DPlayer#related-projects](https://github.com/DIYgod/DPlayer#related-projects)选择一个后端自行搭建,
+或者使用`DPlayer`提供的现成接口`https://api.prprpr.me/dplayer/`
 
 然后修改配置文件：
 
 ```toml
 [bgmi_http]
 danmaku_api_url = "https://api.prprpr.me/dplayer/"  # This api is provided by dplayer official
 ```
@@ -501,86 +512,90 @@
 schtasks /Delete /TN 'bgmi updater'
 ```
 
 ## 如果你对 python 有一点了解, 并且觉得还不够的话, 下面是为你准备的.
 
 ## Bangumi Script
 
-你可以写一个`BGmi Script`来解析你自己的想看的番剧或者美剧. BGmi 会加载你的 script, 视作一个番剧来对待. 而你所需要做的只是继承`ScriptBase`类, 然后实现特定的方法, 再把你的 script 文件放到`BGMI_PATH/script`文件夹内.
+你可以写一个`BGmi Script`来解析你自己的想看的番剧或者美剧. BGmi 会加载你的 script, 视作一个番剧来对待.
+而你所需要做的只是继承`ScriptBase`类, 然后实现特定的方法, 再把你的 script 文件放到`BGMI_PATH/script`文件夹内.
 
 Example: [./tests/script_example.py](./tests/script_example.py)
 
 `get_download_url()`返回一个`dict`, 以对应集数为键, 对应的下载链接为值
 
 ```python
 {
-    1: 'http://example.com/Bangumi/1/1.mp4',
-    2: 'http://example.com/Bangumi/1/2.torrent',
-    3: 'http://example.com/Bangumi/1/3.mp4'
+  1: 'http://example.com/Bangumi/1/1.mp4',
+  2: 'http://example.com/Bangumi/1/2.torrent',
+  3: 'http://example.com/Bangumi/1/3.mp4'
 }
 ```
 
+### 加载 scripts
+
+注意，scripts只会在运行 `bgmi update` 或者 `bgmi cal` 时被加载。如果你在 web ui 找不到对应的内容，请运行前面提到的命令并重试。
+
 ## BGmi 数据源
 
 通过扩展`bgmi.website.base.BaseWebsite`类并且实现对应的三个方法,你也可以简单的添加一个数据源
 
 每个方法具体的意义和返回值格式请参照每个方法对应的注释
 
 ```python
 from typing import List, Optional
 
 from bgmi.website.base import BaseWebsite
 from bgmi.website.model import Episode, WebsiteBangumi
 
 
 class DataSource(BaseWebsite):
-    def search_by_keyword(
-        self, keyword: str, count: int
-    ) -> List[Episode]:  # pragma: no cover
-        """
-
-        :param keyword: search key word
-        :param count: how many page to fetch from website
-        :return: list of episode search result
-        """
-        raise NotImplementedError
-
-    def fetch_bangumi_calendar(self,) -> List[WebsiteBangumi]:  # pragma: no cover
-        """
-        return a list of all bangumi and a list of all subtitle group
-
-        list of bangumi dict:
-        update time should be one of ['Sun', 'Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Unknown']
-        """
-        raise NotImplementedError
-
-    def fetch_episode_of_bangumi(
-        self, bangumi_id: str, max_page: int, subtitle_list: Optional[List[str]] = None
-    ) -> List[Episode]:  # pragma: no cover
-        """
-        get all episode by bangumi id
-
-        :param bangumi_id: bangumi_id
-        :param subtitle_list: list of subtitle group
-        :type subtitle_list: list
-        :param max_page: how many page you want to crawl if there is no subtitle list
-        :type max_page: int
-        :return: list of bangumi
-        """
-        raise NotImplementedError
-
-
-    def fetch_single_bangumi(self, bangumi_id: str) -> WebsiteBangumi:
-        """
-        fetch bangumi info when updating
-
-        :param bangumi_id: bangumi_id, or bangumi['keyword']
-        :type bangumi_id: str
-        :rtype: WebsiteBangumi
-        """
-        # return WebsiteBangumi(keyword=bangumi_id) if website don't has a page contains episodes and info
+  def search_by_keyword(
+    self, keyword: str, count: int
+  ) -> List[Episode]:  # pragma: no cover
+    """
+
+    :param keyword: search key word
+    :param count: how many page to fetch from website
+    :return: list of episode search result
+    """
+    raise NotImplementedError
+
+  def fetch_bangumi_calendar(self, ) -> List[WebsiteBangumi]:  # pragma: no cover
+    """
+    return a list of all bangumi and a list of all subtitle group
+
+    list of bangumi dict:
+    update time should be one of ['Sun', 'Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Unknown']
+    """
+    raise NotImplementedError
+
+  def fetch_episode_of_bangumi(
+    self, bangumi_id: str, max_page: int, subtitle_list: Optional[List[str]] = None
+  ) -> List[Episode]:  # pragma: no cover
+    """
+    get all episode by bangumi id
+
+    :param bangumi_id: bangumi_id
+    :param subtitle_list: list of subtitle group
+    :type subtitle_list: list
+    :param max_page: how many page you want to crawl if there is no subtitle list
+    :type max_page: int
+    :return: list of bangumi
+    """
+    raise NotImplementedError
+
+  def fetch_single_bangumi(self, bangumi_id: str) -> WebsiteBangumi:
+    """
+    fetch bangumi info when updating
+
+    :param bangumi_id: bangumi_id, or bangumi['keyword']
+    :type bangumi_id: str
+    :rtype: WebsiteBangumi
+    """
+    # return WebsiteBangumi(keyword=bangumi_id) if website don't has a page contains episodes and info
 ```
 
 ## License
 
 [MIT License](./LICENSE)
```

