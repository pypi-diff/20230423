# Comparing `tmp/MeUtils-2023.4.6.14.19.58.tar.gz` & `tmp/MeUtils-2023.4.6.14.28.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeUtils-2023.4.6.14.19.58.tar", last modified: Thu Apr  6 06:19:58 2023, max compression
+gzip compressed data, was "MeUtils-2023.4.6.14.28.33.tar", last modified: Thu Apr  6 06:28:33 2023, max compression
```

## Comparing `MeUtils-2023.4.6.14.19.58.tar` & `MeUtils-2023.4.6.14.28.33.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.722129 MeUtils-2023.4.6.14.19.58/
--rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      249 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/MANIFEST.in
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.678947 MeUtils-2023.4.6.14.19.58/MeUtils.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     1858 2023-04-06 06:19:58.000000 MeUtils-2023.4.6.14.19.58/MeUtils.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     7161 2023-04-06 06:19:58.000000 MeUtils-2023.4.6.14.19.58/MeUtils.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-06 06:19:58.000000 MeUtils-2023.4.6.14.19.58/MeUtils.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)      193 2023-04-06 06:19:58.000000 MeUtils-2023.4.6.14.19.58/MeUtils.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)      949 2023-04-06 06:19:58.000000 MeUtils-2023.4.6.14.19.58/MeUtils.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)       17 2023-04-06 06:19:58.000000 MeUtils-2023.4.6.14.19.58/MeUtils.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1858 2023-04-06 06:19:58.721978 MeUtils-2023.4.6.14.19.58/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/README.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.683547 MeUtils-2023.4.6.14.19.58/meutils/
--rw-r--r--   0 betterme   (501) staff       (20)      348 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1762 2023-03-27 05:01:30.000000 MeUtils-2023.4.6.14.19.58/meutils/_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.685303 MeUtils-2023.4.6.14.19.58/meutils/annzoo/
--rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/annzoo/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/annzoo/ann.py
--rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/annzoo/ann_faiss.py
--rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/annzoo/ann_gensim.py
--rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/annzoo/ann_service.py
--rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/annzoo/ann_v1.py
--rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/annzoo/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/annzoo/milvus.py
--rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/annzoo/shake_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.685463 MeUtils-2023.4.6.14.19.58/meutils/asyncio_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/asyncio_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5306 2023-03-26 11:15:57.000000 MeUtils-2023.4.6.14.19.58/meutils/cache_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.686762 MeUtils-2023.4.6.14.19.58/meutils/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2828 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/clis/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/clis/cron.py
--rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/clis/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/clis/gunicorn.conf.py
--rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/clis/monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)     1018 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/clis/nesc.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.687381 MeUtils-2023.4.6.14.19.58/meutils/cmds/
--rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/cmds/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/cmds/cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/cmds/hdfs_cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/cmds/subprocess_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.687697 MeUtils-2023.4.6.14.19.58/meutils/coding/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/coding/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/coding/find132.py
--rw-r--r--   0 betterme   (501) staff       (20)     8164 2023-04-04 15:33:02.000000 MeUtils-2023.4.6.14.19.58/meutils/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.687995 MeUtils-2023.4.6.14.19.58/meutils/comp_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/comp_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/comp_utils/reverse_metric.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.693695 MeUtils-2023.4.6.14.19.58/meutils/data/
--rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2023.4.6.14.19.58/meutils/data/SimHei.ttf
--rw-r--r--   0 betterme   (501) staff       (20)       19 2023-04-06 06:19:58.000000 MeUtils-2023.4.6.14.19.58/meutils/data/VERSION
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/data/_FLAG
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/data/_SUCCESS
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/data/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/data/coordinate.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.698917 MeUtils-2023.4.6.14.19.58/meutils/datamodels/
--rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/datamodels/ArticleInfo.py
--rw-r--r--   0 betterme   (501) staff       (20)      467 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/datamodels/DataType.py
--rw-r--r--   0 betterme   (501) staff       (20)      247 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/datamodels/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      454 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/datamodels/nesc.py
--rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/date_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.699596 MeUtils-2023.4.6.14.19.58/meutils/db/
--rw-r--r--   0 betterme   (501) staff       (20)     4817 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/db/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/db/mongo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/db/neo4j.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.701102 MeUtils-2023.4.6.14.19.58/meutils/decorators/
--rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/decorators/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1679 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/decorators/ai.py
--rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/decorators/catch.py
--rw-r--r--   0 betterme   (501) staff       (20)     6248 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/decorators/common.py
--rw-r--r--   0 betterme   (501) staff       (20)    15575 2023-04-06 06:19:56.000000 MeUtils-2023.4.6.14.19.58/meutils/decorators/decorator.py
--rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/decorators/decorator_demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      527 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/decorators/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2115 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/decorators/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/decorators/retry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2023.4.6.14.19.58/meutils/decorators/scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)     3536 2023-03-31 02:35:37.000000 MeUtils-2023.4.6.14.19.58/meutils/dist_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.701377 MeUtils-2023.4.6.14.19.58/meutils/easy_search/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/easy_search/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-03-28 05:10:55.000000 MeUtils-2023.4.6.14.19.58/meutils/easy_search/es.py
--rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2023.4.6.14.19.58/meutils/hash_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/import_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.702098 MeUtils-2023.4.6.14.19.58/meutils/io/
--rw-r--r--   0 betterme   (501) staff       (20)     1590 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/io/file.py
--rw-r--r--   0 betterme   (501) staff       (20)     2290 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/io/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     8580 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/io/tf_io.py
--rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/jinja_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2512 2023-04-02 12:55:05.000000 MeUtils-2023.4.6.14.19.58/meutils/log_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.703357 MeUtils-2023.4.6.14.19.58/meutils/notice/
--rw-r--r--   0 betterme   (501) staff       (20)      837 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/notice/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/notice/emails.py
--rw-r--r--   0 betterme   (501) staff       (20)      703 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/notice/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/notice/file_post.py
--rw-r--r--   0 betterme   (501) staff       (20)     2229 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/notice/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/notice/wechat_.py
--rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/notice/wecom.py
--rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/notice/weekmeet.py
--rw-r--r--   0 betterme   (501) staff       (20)     3181 2023-03-31 02:35:37.000000 MeUtils-2023.4.6.14.19.58/meutils/np_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.704392 MeUtils-2023.4.6.14.19.58/meutils/office_automation/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/office_automation/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2023.4.6.14.19.58/meutils/office_automation/doc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1263 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/office_automation/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2023.4.6.14.19.58/meutils/office_automation/pdm.py
--rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2023.4.6.14.19.58/meutils/office_automation/pdm_run.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.704674 MeUtils-2023.4.6.14.19.58/meutils/office_automation/report/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/office_automation/report/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.705645 MeUtils-2023.4.6.14.19.58/meutils/other/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/other/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/other/besttable.py
--rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2023.4.6.14.19.58/meutils/other/crontab.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.706494 MeUtils-2023.4.6.14.19.58/meutils/pandas_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/pandas_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/pandas_utils/opt.py
--rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/pandas_utils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2535 2023-04-04 04:10:37.000000 MeUtils-2023.4.6.14.19.58/meutils/path_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6916 2023-03-31 09:29:39.000000 MeUtils-2023.4.6.14.19.58/meutils/pipe.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.707452 MeUtils-2023.4.6.14.19.58/meutils/plots/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/plots/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/plots/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/plots/echarts.py
--rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/plots/metrics.py
--rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/plots/plot_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.708497 MeUtils-2023.4.6.14.19.58/meutils/request_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     2461 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/request_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1472 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/request_utils/crawler.py
--rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2023.4.6.14.19.58/meutils/request_utils/download.py
--rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/request_utils/results.py
--rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/request_utils/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)      644 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/request_utils/公网ip.py
--rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/sftp.py
--rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/sk_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     1398 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/smooth_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.708644 MeUtils-2023.4.6.14.19.58/meutils/spark/
--rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/spark/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.709306 MeUtils-2023.4.6.14.19.58/meutils/str_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/str_utils/Translator.py
--rw-r--r--   0 betterme   (501) staff       (20)     6417 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/str_utils/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.709873 MeUtils-2023.4.6.14.19.58/meutils/str_utils/__translater/
--rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/str_utils/__translater/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/str_utils/__translater/tencent.py
--rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/str_utils/__translater/translater.py
--rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/str_utils/__translater/youdao.py
--rw-r--r--   0 betterme   (501) staff       (20)      936 2023-03-27 05:26:36.000000 MeUtils-2023.4.6.14.19.58/meutils/str_utils/json_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      430 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/str_utils/regular_expression.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.711340 MeUtils-2023.4.6.14.19.58/meutils/templates/
--rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/demo.conf
--rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/demo.j2
--rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/demox.py
--rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/df_html.j2
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.712720 MeUtils-2023.4.6.14.19.58/meutils/templates/dockerfiles/
--rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/dockerfiles/Dockerfile
--rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/dockerfiles/Dockerfile_me
--rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/dockerfiles/Dockerfile_milvus
--rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/dockerfiles/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/dockerfiles/docker_build_push.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/dockerfiles/docker_push.sh
--rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/hegui.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.712886 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/
--rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/cookiecutter.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.716294 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.716491 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
--rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.718608 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.718756 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
--rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
--rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.719063 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.719409 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.719879 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/tpl.docx
--rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/templates/合规日报模板.docx
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.720789 MeUtils-2023.4.6.14.19.58/meutils/tools/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/tools/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/tools/cprint.py
--rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/tools/machine_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/tools/seize.py
--rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/tools/service_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/tools/sys_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      360 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/typings.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:19:58.721644 MeUtils-2023.4.6.14.19.58/meutils/ui/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-21 00:52:16.000000 MeUtils-2023.4.6.14.19.58/meutils/ui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1658 2023-03-21 01:20:09.000000 MeUtils-2023.4.6.14.19.58/meutils/ui/bar.py
--rw-r--r--   0 betterme   (501) staff       (20)      546 2023-03-21 01:21:30.000000 MeUtils-2023.4.6.14.19.58/meutils/ui/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/meutils/zk_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-06 06:19:58.722173 MeUtils-2023.4.6.14.19.58/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2307 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.19.58/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.724788 MeUtils-2023.4.6.14.28.33/
+-rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      249 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/MANIFEST.in
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.694846 MeUtils-2023.4.6.14.28.33/MeUtils.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     1858 2023-04-06 06:28:33.000000 MeUtils-2023.4.6.14.28.33/MeUtils.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     7161 2023-04-06 06:28:33.000000 MeUtils-2023.4.6.14.28.33/MeUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-06 06:28:33.000000 MeUtils-2023.4.6.14.28.33/MeUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      193 2023-04-06 06:28:33.000000 MeUtils-2023.4.6.14.28.33/MeUtils.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      949 2023-04-06 06:28:33.000000 MeUtils-2023.4.6.14.28.33/MeUtils.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       17 2023-04-06 06:28:33.000000 MeUtils-2023.4.6.14.28.33/MeUtils.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1858 2023-04-06 06:28:33.724618 MeUtils-2023.4.6.14.28.33/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/README.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.697312 MeUtils-2023.4.6.14.28.33/meutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      348 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1762 2023-03-27 05:01:30.000000 MeUtils-2023.4.6.14.28.33/meutils/_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.698677 MeUtils-2023.4.6.14.28.33/meutils/annzoo/
+-rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/annzoo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/annzoo/ann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/annzoo/ann_faiss.py
+-rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/annzoo/ann_gensim.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/annzoo/ann_service.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/annzoo/ann_v1.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/annzoo/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/annzoo/milvus.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/annzoo/shake_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.698819 MeUtils-2023.4.6.14.28.33/meutils/asyncio_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/asyncio_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5306 2023-03-26 11:15:57.000000 MeUtils-2023.4.6.14.28.33/meutils/cache_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.699864 MeUtils-2023.4.6.14.28.33/meutils/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2828 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/clis/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/clis/cron.py
+-rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/clis/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/clis/gunicorn.conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/clis/monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1018 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/clis/nesc.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.700383 MeUtils-2023.4.6.14.28.33/meutils/cmds/
+-rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/cmds/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/cmds/cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/cmds/hdfs_cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/cmds/subprocess_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.700647 MeUtils-2023.4.6.14.28.33/meutils/coding/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/coding/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/coding/find132.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8164 2023-04-04 15:33:02.000000 MeUtils-2023.4.6.14.28.33/meutils/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.700919 MeUtils-2023.4.6.14.28.33/meutils/comp_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/comp_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/comp_utils/reverse_metric.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.706823 MeUtils-2023.4.6.14.28.33/meutils/data/
+-rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2023.4.6.14.28.33/meutils/data/SimHei.ttf
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2023-04-06 06:28:33.000000 MeUtils-2023.4.6.14.28.33/meutils/data/VERSION
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/data/_FLAG
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/data/_SUCCESS
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/data/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/data/coordinate.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.707358 MeUtils-2023.4.6.14.28.33/meutils/datamodels/
+-rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/datamodels/ArticleInfo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      467 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/datamodels/DataType.py
+-rw-r--r--   0 betterme   (501) staff       (20)      247 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/datamodels/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      454 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/datamodels/nesc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/date_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.707773 MeUtils-2023.4.6.14.28.33/meutils/db/
+-rw-r--r--   0 betterme   (501) staff       (20)     4817 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/db/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/db/mongo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/db/neo4j.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.709149 MeUtils-2023.4.6.14.28.33/meutils/decorators/
+-rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/decorators/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1679 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/decorators/ai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/decorators/catch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6248 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/decorators/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2023.4.6.14.28.33/meutils/decorators/decorator.py
+-rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/decorators/decorator_demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      527 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/decorators/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2115 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/decorators/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/decorators/retry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2023.4.6.14.28.33/meutils/decorators/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3536 2023-03-31 02:35:37.000000 MeUtils-2023.4.6.14.28.33/meutils/dist_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.709412 MeUtils-2023.4.6.14.28.33/meutils/easy_search/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/easy_search/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-03-28 05:10:55.000000 MeUtils-2023.4.6.14.28.33/meutils/easy_search/es.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2023.4.6.14.28.33/meutils/hash_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/import_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.709941 MeUtils-2023.4.6.14.28.33/meutils/io/
+-rw-r--r--   0 betterme   (501) staff       (20)     1590 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/io/file.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2290 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/io/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8580 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/io/tf_io.py
+-rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/jinja_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2512 2023-04-02 12:55:05.000000 MeUtils-2023.4.6.14.28.33/meutils/log_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.711049 MeUtils-2023.4.6.14.28.33/meutils/notice/
+-rw-r--r--   0 betterme   (501) staff       (20)      837 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/notice/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/notice/emails.py
+-rw-r--r--   0 betterme   (501) staff       (20)      703 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/notice/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/notice/file_post.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2229 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/notice/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/notice/wechat_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/notice/wecom.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/notice/weekmeet.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3181 2023-03-31 02:35:37.000000 MeUtils-2023.4.6.14.28.33/meutils/np_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.711635 MeUtils-2023.4.6.14.28.33/meutils/office_automation/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/office_automation/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2023.4.6.14.28.33/meutils/office_automation/doc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1263 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/office_automation/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2023.4.6.14.28.33/meutils/office_automation/pdm.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2023.4.6.14.28.33/meutils/office_automation/pdm_run.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.711770 MeUtils-2023.4.6.14.28.33/meutils/office_automation/report/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/office_automation/report/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.712191 MeUtils-2023.4.6.14.28.33/meutils/other/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/other/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/other/besttable.py
+-rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2023.4.6.14.28.33/meutils/other/crontab.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.712615 MeUtils-2023.4.6.14.28.33/meutils/pandas_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/pandas_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/pandas_utils/opt.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/pandas_utils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2535 2023-04-04 04:10:37.000000 MeUtils-2023.4.6.14.28.33/meutils/path_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6916 2023-03-31 09:29:39.000000 MeUtils-2023.4.6.14.28.33/meutils/pipe.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.713311 MeUtils-2023.4.6.14.28.33/meutils/plots/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/plots/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/plots/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/plots/echarts.py
+-rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/plots/metrics.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/plots/plot_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.714071 MeUtils-2023.4.6.14.28.33/meutils/request_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     2461 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/request_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1472 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/request_utils/crawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2023.4.6.14.28.33/meutils/request_utils/download.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/request_utils/results.py
+-rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/request_utils/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)      644 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/request_utils/公网ip.py
+-rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/sftp.py
+-rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/sk_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1398 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/smooth_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.714199 MeUtils-2023.4.6.14.28.33/meutils/spark/
+-rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/spark/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.714741 MeUtils-2023.4.6.14.28.33/meutils/str_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/str_utils/Translator.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6417 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/str_utils/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.715313 MeUtils-2023.4.6.14.28.33/meutils/str_utils/__translater/
+-rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/str_utils/__translater/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/str_utils/__translater/tencent.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/str_utils/__translater/translater.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/str_utils/__translater/youdao.py
+-rw-r--r--   0 betterme   (501) staff       (20)      936 2023-03-27 05:26:36.000000 MeUtils-2023.4.6.14.28.33/meutils/str_utils/json_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      430 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/str_utils/regular_expression.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.716991 MeUtils-2023.4.6.14.28.33/meutils/templates/
+-rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/demo.conf
+-rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/demo.j2
+-rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/demox.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/df_html.j2
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.718046 MeUtils-2023.4.6.14.28.33/meutils/templates/dockerfiles/
+-rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/dockerfiles/Dockerfile
+-rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/dockerfiles/Dockerfile_me
+-rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/dockerfiles/Dockerfile_milvus
+-rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/dockerfiles/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/dockerfiles/docker_build_push.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/dockerfiles/docker_push.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/hegui.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.718178 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/
+-rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/cookiecutter.json
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.720412 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.720542 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.722023 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.722162 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
+-rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
+-rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.722443 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.722708 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.723130 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/tpl.docx
+-rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/templates/合规日报模板.docx
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.723933 MeUtils-2023.4.6.14.28.33/meutils/tools/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/tools/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/tools/cprint.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/tools/machine_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/tools/seize.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/tools/service_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/tools/sys_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      360 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/typings.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:28:33.724336 MeUtils-2023.4.6.14.28.33/meutils/ui/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-21 00:52:16.000000 MeUtils-2023.4.6.14.28.33/meutils/ui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1658 2023-03-21 01:20:09.000000 MeUtils-2023.4.6.14.28.33/meutils/ui/bar.py
+-rw-r--r--   0 betterme   (501) staff       (20)      546 2023-03-21 01:21:30.000000 MeUtils-2023.4.6.14.28.33/meutils/ui/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/meutils/zk_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-06 06:28:33.724837 MeUtils-2023.4.6.14.28.33/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2307 2023-03-20 02:44:39.000000 MeUtils-2023.4.6.14.28.33/setup.py
```

### Comparing `MeUtils-2023.4.6.14.19.58/LICENSE` & `MeUtils-2023.4.6.14.28.33/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/MeUtils.egg-info/PKG-INFO` & `MeUtils-2023.4.6.14.28.33/MeUtils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2023.4.6.14.19.58
+Version: 2023.4.6.14.28.33
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
```

### Comparing `MeUtils-2023.4.6.14.19.58/MeUtils.egg-info/SOURCES.txt` & `MeUtils-2023.4.6.14.28.33/MeUtils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/MeUtils.egg-info/requires.txt` & `MeUtils-2023.4.6.14.28.33/MeUtils.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -21,44 +21,44 @@
 schedule
 
 [ai]
 faiss-gpu
 gensim
 
 [all]
+geopy
+pandas_summary
+pymupd
+dataframe_image
+pandas-profiling[notebook]
+polars
 iteration_utilities
-simplejson
-fastapi[all]
 missingno
-jinja2
+thefuck
+faiss-cpu
 pretty_errors
-cachetools
-pymilvus
+streamlit
 thriftpy2
-polars
-pymupd
-pymysql
-thefuck
+pymilvus
+jinja2
+pymongo
 gensim
-streamlit
-faiss-cpu
+redis-py-cluster
+simplejson
+jmespath
 pyarrow
-jieba
 uvicorn
-dataframe_image
-pymongo
-geopy
-schedule
-reportlab
 seaborn
-redis-py-cluster
+jieba
+cachetools
+reportlab
 faiss-gpu
-jmespath
-pandas_summary
-pandas-profiling[notebook]
+fastapi[all]
+schedule
+pymysql
 
 [ann]
 pymilvus
 faiss-cpu
 
 [app]
 fastapi[all]
```

### Comparing `MeUtils-2023.4.6.14.19.58/PKG-INFO` & `MeUtils-2023.4.6.14.28.33/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2023.4.6.14.19.58
+Version: 2023.4.6.14.28.33
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
```

### Comparing `MeUtils-2023.4.6.14.19.58/README.md` & `MeUtils-2023.4.6.14.28.33/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/annzoo/ann.py` & `MeUtils-2023.4.6.14.28.33/meutils/annzoo/ann.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/annzoo/ann_faiss.py` & `MeUtils-2023.4.6.14.28.33/meutils/annzoo/ann_faiss.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/annzoo/ann_gensim.py` & `MeUtils-2023.4.6.14.28.33/meutils/annzoo/ann_gensim.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/annzoo/ann_service.py` & `MeUtils-2023.4.6.14.28.33/meutils/annzoo/ann_service.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/annzoo/ann_v1.py` & `MeUtils-2023.4.6.14.28.33/meutils/annzoo/ann_v1.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/annzoo/cli.py` & `MeUtils-2023.4.6.14.28.33/meutils/annzoo/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/annzoo/shake_demo.py` & `MeUtils-2023.4.6.14.28.33/meutils/annzoo/shake_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/cache_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/cache_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/clis/cli.py` & `MeUtils-2023.4.6.14.28.33/meutils/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/clis/conf.py` & `MeUtils-2023.4.6.14.28.33/meutils/clis/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/clis/cron.py` & `MeUtils-2023.4.6.14.28.33/meutils/clis/cron.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/clis/demo.py` & `MeUtils-2023.4.6.14.28.33/meutils/clis/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/clis/gunicorn.conf.py` & `MeUtils-2023.4.6.14.28.33/meutils/clis/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/clis/monitor.py` & `MeUtils-2023.4.6.14.28.33/meutils/clis/monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/clis/nesc.py` & `MeUtils-2023.4.6.14.28.33/meutils/clis/nesc.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/cmds/hdfs_cmd.py` & `MeUtils-2023.4.6.14.28.33/meutils/cmds/hdfs_cmd.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/cmds/subprocess_demo.py` & `MeUtils-2023.4.6.14.28.33/meutils/cmds/subprocess_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/coding/find132.py` & `MeUtils-2023.4.6.14.28.33/meutils/coding/find132.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/common.py` & `MeUtils-2023.4.6.14.28.33/meutils/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/comp_utils/reverse_metric.py` & `MeUtils-2023.4.6.14.28.33/meutils/comp_utils/reverse_metric.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/data/SimHei.ttf` & `MeUtils-2023.4.6.14.28.33/meutils/data/SimHei.ttf`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/data/coordinate.py` & `MeUtils-2023.4.6.14.28.33/meutils/data/coordinate.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/datamodels/ArticleInfo.py` & `MeUtils-2023.4.6.14.28.33/meutils/datamodels/ArticleInfo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/date_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/date_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/db/__init__.py` & `MeUtils-2023.4.6.14.28.33/meutils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/db/mongo.py` & `MeUtils-2023.4.6.14.28.33/meutils/db/mongo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/db/neo4j.py` & `MeUtils-2023.4.6.14.28.33/meutils/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/decorators/__init__.py` & `MeUtils-2023.4.6.14.28.33/meutils/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/decorators/ai.py` & `MeUtils-2023.4.6.14.28.33/meutils/decorators/ai.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/decorators/catch.py` & `MeUtils-2023.4.6.14.28.33/meutils/decorators/catch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/decorators/common.py` & `MeUtils-2023.4.6.14.28.33/meutils/decorators/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/decorators/decorator.py` & `MeUtils-2023.4.6.14.28.33/meutils/decorators/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,18 @@
             for res in caller(func, *(extras + args), **kw):
                 yield res
     else:
         def fun(*args, **kw):
             if not kwsyntax:
                 args, kw = fix(args, kw, sig)
             return caller(func, *(extras + args), **kw)
+
+    if not hasattr(func, '__name__'):
+        func.__name__ = func.__qualname__ = '__name__'
+
     fun.__name__ = func.__name__
     fun.__doc__ = func.__doc__
     fun.__wrapped__ = func
     fun.__signature__ = sig
     fun.__qualname__ = func.__qualname__
     # builtin functions like defaultdict.__setitem__ lack many attributes
     try:
@@ -270,17 +274,14 @@
         if func is None:
             return lambda func: decorate(func, caller, extras, kwsyntax)
         else:
             return decorate(func, caller, extras, kwsyntax)
 
     dec.__signature__ = sig.replace(parameters=dec_params)
 
-    if not hasattr(caller, '__name__'):
-        caller.__name__ = caller.__qualname__ = '__name__'
-
     dec.__name__ = caller.__name__
     dec.__doc__ = caller.__doc__
     dec.__wrapped__ = caller
     dec.__qualname__ = caller.__qualname__
     dec.__kwdefaults__ = getattr(caller, '__kwdefaults__', None)
     dec.__dict__.update(caller.__dict__)
     return dec
```

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/decorators/decorator_demo.py` & `MeUtils-2023.4.6.14.28.33/meutils/decorators/decorator_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/decorators/demo.py` & `MeUtils-2023.4.6.14.28.33/meutils/decorators/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/decorators/feishu.py` & `MeUtils-2023.4.6.14.28.33/meutils/decorators/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/decorators/retry.py` & `MeUtils-2023.4.6.14.28.33/meutils/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/decorators/scheduler.py` & `MeUtils-2023.4.6.14.28.33/meutils/decorators/scheduler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/dist_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/easy_search/es.py` & `MeUtils-2023.4.6.14.28.33/meutils/easy_search/es.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/hash_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/import_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/import_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/io/__init__.py` & `MeUtils-2023.4.6.14.28.33/meutils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/io/image.py` & `MeUtils-2023.4.6.14.28.33/meutils/io/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/io/tf_io.py` & `MeUtils-2023.4.6.14.28.33/meutils/io/tf_io.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/jinja_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/jinja_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/log_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/notice/__init__.py` & `MeUtils-2023.4.6.14.28.33/meutils/notice/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/notice/emails.py` & `MeUtils-2023.4.6.14.28.33/meutils/notice/emails.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/notice/feishu.py` & `MeUtils-2023.4.6.14.28.33/meutils/notice/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/notice/file_post.py` & `MeUtils-2023.4.6.14.28.33/meutils/notice/file_post.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/notice/wechat.py` & `MeUtils-2023.4.6.14.28.33/meutils/notice/wechat.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/notice/wechat_.py` & `MeUtils-2023.4.6.14.28.33/meutils/notice/wechat_.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/notice/wecom.py` & `MeUtils-2023.4.6.14.28.33/meutils/notice/wecom.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/notice/weekmeet.py` & `MeUtils-2023.4.6.14.28.33/meutils/notice/weekmeet.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/np_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/np_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/office_automation/pdf.py` & `MeUtils-2023.4.6.14.28.33/meutils/office_automation/pdf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/office_automation/pdm.py` & `MeUtils-2023.4.6.14.28.33/meutils/office_automation/pdm.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/office_automation/pdm_run.py` & `MeUtils-2023.4.6.14.28.33/meutils/office_automation/pdm_run.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/other/besttable.py` & `MeUtils-2023.4.6.14.28.33/meutils/other/besttable.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/other/crontab.py` & `MeUtils-2023.4.6.14.28.33/meutils/other/crontab.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/pandas_utils/opt.py` & `MeUtils-2023.4.6.14.28.33/meutils/pandas_utils/opt.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/pandas_utils/pd_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/pandas_utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/path_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/path_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/pd_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/pipe.py` & `MeUtils-2023.4.6.14.28.33/meutils/pipe.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/plots/demo.py` & `MeUtils-2023.4.6.14.28.33/meutils/plots/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/plots/echarts.py` & `MeUtils-2023.4.6.14.28.33/meutils/plots/echarts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/plots/metrics.py` & `MeUtils-2023.4.6.14.28.33/meutils/plots/metrics.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/plots/plot_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/plots/plot_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/request_utils/__init__.py` & `MeUtils-2023.4.6.14.28.33/meutils/request_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/request_utils/crawler.py` & `MeUtils-2023.4.6.14.28.33/meutils/request_utils/crawler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/request_utils/download.py` & `MeUtils-2023.4.6.14.28.33/meutils/request_utils/download.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/request_utils/results.py` & `MeUtils-2023.4.6.14.28.33/meutils/request_utils/results.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/request_utils/公网ip.py` & `MeUtils-2023.4.6.14.28.33/meutils/request_utils/公网ip.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/sftp.py` & `MeUtils-2023.4.6.14.28.33/meutils/sftp.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/sk_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/sk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/smooth_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/smooth_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/spark/__init__.py` & `MeUtils-2023.4.6.14.28.33/meutils/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/str_utils/Translator.py` & `MeUtils-2023.4.6.14.28.33/meutils/str_utils/Translator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/str_utils/__init__.py` & `MeUtils-2023.4.6.14.28.33/meutils/str_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/str_utils/__translater/tencent.py` & `MeUtils-2023.4.6.14.28.33/meutils/str_utils/__translater/tencent.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/str_utils/__translater/translater.py` & `MeUtils-2023.4.6.14.28.33/meutils/str_utils/__translater/translater.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/str_utils/__translater/youdao.py` & `MeUtils-2023.4.6.14.28.33/meutils/str_utils/__translater/youdao.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/str_utils/json_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/str_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/demo.j2` & `MeUtils-2023.4.6.14.28.33/meutils/templates/demo.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/demo.py` & `MeUtils-2023.4.6.14.28.33/meutils/templates/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/demox.py` & `MeUtils-2023.4.6.14.28.33/meutils/templates/demox.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/df_html.j2` & `MeUtils-2023.4.6.14.28.33/meutils/templates/df_html.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/dockerfiles/docker_build_push.py` & `MeUtils-2023.4.6.14.28.33/meutils/templates/dockerfiles/docker_build_push.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/hegui.py` & `MeUtils-2023.4.6.14.28.33/meutils/templates/hegui.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/cookiecutter.json` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py` & `MeUtils-2023.4.6.14.28.33/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/tpl.docx` & `MeUtils-2023.4.6.14.28.33/meutils/templates/tpl.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/templates/合规日报模板.docx` & `MeUtils-2023.4.6.14.28.33/meutils/templates/合规日报模板.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/tools/cprint.py` & `MeUtils-2023.4.6.14.28.33/meutils/tools/cprint.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/tools/machine_monitor.py` & `MeUtils-2023.4.6.14.28.33/meutils/tools/machine_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/tools/seize.py` & `MeUtils-2023.4.6.14.28.33/meutils/tools/seize.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/tools/service_monitor.py` & `MeUtils-2023.4.6.14.28.33/meutils/tools/service_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/ui/bar.py` & `MeUtils-2023.4.6.14.28.33/meutils/ui/bar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/ui/demo.py` & `MeUtils-2023.4.6.14.28.33/meutils/ui/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/meutils/zk_utils.py` & `MeUtils-2023.4.6.14.28.33/meutils/zk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.4.6.14.19.58/setup.py` & `MeUtils-2023.4.6.14.28.33/setup.py`

 * *Files identical despite different names*

