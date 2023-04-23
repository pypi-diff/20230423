# Comparing `tmp/act-workers-2.1.8.tar.gz` & `tmp/act-workers-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "act-workers-2.1.8.tar", last modified: Wed Mar 15 09:44:48 2023, max compression
+gzip compressed data, was "act-workers-2.1.9.tar", last modified: Wed Mar 22 12:00:10 2023, max compression
```

## Comparing `act-workers-2.1.8.tar` & `act-workers-2.1.9.tar`

### file list

```diff
@@ -1,61 +1,64 @@
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-15 09:44:48.710867 act-workers-2.1.8/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      767 2022-02-02 11:57:58.000000 act-workers-2.1.8/LICENSE
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    11846 2023-03-15 09:44:48.710867 act-workers-2.1.8/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    11365 2022-08-15 10:14:14.000000 act-workers-2.1.8/README.md
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-15 09:44:48.707534 act-workers-2.1.8/act/
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-15 09:44:48.710867 act-workers-2.1.8/act/workers/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        0 2022-02-02 11:57:58.000000 act-workers-2.1.8/act/workers/__init__.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     5906 2022-02-02 11:57:58.000000 act-workers-2.1.8/act/workers/act_feed.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     9717 2022-02-02 11:57:58.000000 act-workers-2.1.8/act/workers/alienvault_otx.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     7122 2023-01-03 08:36:38.000000 act-workers-2.1.8/act/workers/argus_case.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    12606 2022-10-12 05:35:34.000000 act-workers-2.1.8/act/workers/attack.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     2627 2023-03-15 09:44:45.000000 act-workers-2.1.8/act/workers/country_regions.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-15 09:44:48.710867 act-workers-2.1.8/act/workers/etc/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     6746 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/etc/act.ini
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      258 2022-02-02 11:57:58.000000 act-workers-2.1.8/act/workers/etc/search_jobs.ini
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     9848 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/fact_chain_helper.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     6194 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/generic_uploader.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    14201 2022-12-15 09:04:24.000000 act-workers-2.1.8/act/workers/hybrid_analysis_feed.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     2891 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/ip_asn_history.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     2837 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/ip_filter.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    14954 2022-02-02 11:57:58.000000 act-workers-2.1.8/act/workers/isight.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-15 09:44:48.710867 act-workers-2.1.8/act/workers/libs/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        0 2022-02-02 11:57:58.000000 act-workers-2.1.8/act/workers/libs/__init__.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    12651 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/libs/argus.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     8285 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/libs/misp.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     5092 2023-01-03 08:36:38.000000 act-workers-2.1.8/act/workers/libs/mnemonic.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3677 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/libs/ta_list_methods.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     5412 2022-02-02 11:57:58.000000 act-workers-2.1.8/act/workers/libs/urlcache.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     5412 2023-03-15 09:44:45.000000 act-workers-2.1.8/act/workers/libs/worker.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     6866 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/misp_feeds.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     6983 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/mnemonic_pdns.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     9019 2022-11-08 08:48:50.000000 act-workers-2.1.8/act/workers/scio.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     6916 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/search_graph.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    11935 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/shadowserver_asn.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     7508 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/shadowserver_enrich.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    12103 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/ta_helper.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     2161 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/template.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     8944 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/thaicert.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3391 2022-02-02 11:57:58.000000 act-workers-2.1.8/act/workers/tool_alias.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     2292 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/update_ta_aliases_list.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     4963 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/url_shorter_unpack.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    12609 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/veris.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    18735 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/vt.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     2001 2022-08-05 06:45:05.000000 act-workers-2.1.8/act/workers/worker_config.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-15 09:44:48.710867 act-workers-2.1.8/act_workers.egg-info/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    11846 2023-03-15 09:44:48.000000 act-workers-2.1.8/act_workers.egg-info/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1423 2023-03-15 09:44:48.000000 act-workers-2.1.8/act_workers.egg-info/SOURCES.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2023-03-15 09:44:48.000000 act-workers-2.1.8/act_workers.egg-info/dependency_links.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1321 2023-03-15 09:44:48.000000 act-workers-2.1.8/act_workers.egg-info/entry_points.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        4 2023-03-15 09:44:48.000000 act-workers-2.1.8/act_workers.egg-info/namespace_packages.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      125 2023-03-15 09:44:48.000000 act-workers-2.1.8/act_workers.egg-info/requires.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        4 2023-03-15 09:44:48.000000 act-workers-2.1.8/act_workers.egg-info/top_level.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2022-02-02 11:58:28.000000 act-workers-2.1.8/act_workers.egg-info/zip-safe
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       62 2023-03-15 09:44:48.714200 act-workers-2.1.8/setup.cfg
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3312 2023-03-15 09:44:45.000000 act-workers-2.1.8/setup.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-15 09:44:48.710867 act-workers-2.1.8/test/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     5192 2022-02-02 11:57:58.000000 act-workers-2.1.8/test/test_argus_case.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2360 2022-02-02 11:57:58.000000 act-workers-2.1.8/test/test_config.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2071 2022-08-05 06:45:05.000000 act-workers-2.1.8/test/test_misp.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3512 2022-03-29 08:14:21.000000 act-workers-2.1.8/test/test_scio.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3815 2022-02-02 11:57:58.000000 act-workers-2.1.8/test/test_worker.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-22 12:00:10.111632 act-workers-2.1.9/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      767 2022-02-02 11:57:58.000000 act-workers-2.1.9/LICENSE
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    11846 2023-03-22 12:00:10.111632 act-workers-2.1.9/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    11365 2022-08-15 10:14:14.000000 act-workers-2.1.9/README.md
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-22 12:00:10.108299 act-workers-2.1.9/act/
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-22 12:00:10.108299 act-workers-2.1.9/act/workers/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        0 2022-02-02 11:57:58.000000 act-workers-2.1.9/act/workers/__init__.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     5906 2022-02-02 11:57:58.000000 act-workers-2.1.9/act/workers/act_feed.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     9717 2022-02-02 11:57:58.000000 act-workers-2.1.9/act/workers/alienvault_otx.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     7122 2023-01-03 08:36:38.000000 act-workers-2.1.9/act/workers/argus_case.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    12606 2022-10-12 05:35:34.000000 act-workers-2.1.9/act/workers/attack.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     2627 2023-03-15 09:44:45.000000 act-workers-2.1.9/act/workers/country_regions.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-22 12:00:10.108299 act-workers-2.1.9/act/workers/etc/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     6877 2023-03-22 12:00:06.000000 act-workers-2.1.9/act/workers/etc/act.ini
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      258 2022-02-02 11:57:58.000000 act-workers-2.1.9/act/workers/etc/search_jobs.ini
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     9848 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/fact_chain_helper.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     6194 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/generic_uploader.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    14201 2022-12-15 09:04:24.000000 act-workers-2.1.9/act/workers/hybrid_analysis_feed.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     2891 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/ip_asn_history.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     2837 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/ip_filter.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    14954 2022-02-02 11:57:58.000000 act-workers-2.1.9/act/workers/isight.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-22 12:00:10.111632 act-workers-2.1.9/act/workers/libs/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        0 2022-02-02 11:57:58.000000 act-workers-2.1.9/act/workers/libs/__init__.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    12651 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/libs/argus.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3833 2023-03-22 12:00:06.000000 act-workers-2.1.9/act/workers/libs/fact_chain.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     8733 2023-03-22 12:00:06.000000 act-workers-2.1.9/act/workers/libs/mandiant_ti_v4.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     8285 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/libs/misp.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     5092 2023-01-03 08:36:38.000000 act-workers-2.1.9/act/workers/libs/mnemonic.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3677 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/libs/ta_list_methods.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     5412 2022-02-02 11:57:58.000000 act-workers-2.1.9/act/workers/libs/urlcache.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     5412 2023-03-15 09:44:45.000000 act-workers-2.1.9/act/workers/libs/worker.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     5512 2023-03-22 12:00:06.000000 act-workers-2.1.9/act/workers/mandiant_ti.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     6866 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/misp_feeds.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     6983 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/mnemonic_pdns.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     9019 2022-11-08 08:48:50.000000 act-workers-2.1.9/act/workers/scio.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     6916 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/search_graph.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    11935 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/shadowserver_asn.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     7508 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/shadowserver_enrich.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     8457 2023-03-22 12:00:06.000000 act-workers-2.1.9/act/workers/ta_helper.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     2161 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/template.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     8944 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/thaicert.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3391 2022-02-02 11:57:58.000000 act-workers-2.1.9/act/workers/tool_alias.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     2292 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/update_ta_aliases_list.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     4963 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/url_shorter_unpack.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    12609 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/veris.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    18735 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/vt.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     2001 2022-08-05 06:45:05.000000 act-workers-2.1.9/act/workers/worker_config.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-22 12:00:10.111632 act-workers-2.1.9/act_workers.egg-info/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    11846 2023-03-22 12:00:10.000000 act-workers-2.1.9/act_workers.egg-info/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1516 2023-03-22 12:00:10.000000 act-workers-2.1.9/act_workers.egg-info/SOURCES.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2023-03-22 12:00:10.000000 act-workers-2.1.9/act_workers.egg-info/dependency_links.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1377 2023-03-22 12:00:10.000000 act-workers-2.1.9/act_workers.egg-info/entry_points.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        4 2023-03-22 12:00:10.000000 act-workers-2.1.9/act_workers.egg-info/namespace_packages.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      125 2023-03-22 12:00:10.000000 act-workers-2.1.9/act_workers.egg-info/requires.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        4 2023-03-22 12:00:10.000000 act-workers-2.1.9/act_workers.egg-info/top_level.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2022-02-02 11:58:28.000000 act-workers-2.1.9/act_workers.egg-info/zip-safe
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       62 2023-03-22 12:00:10.111632 act-workers-2.1.9/setup.cfg
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3383 2023-03-22 12:00:06.000000 act-workers-2.1.9/setup.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-22 12:00:10.111632 act-workers-2.1.9/test/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     5192 2022-02-02 11:57:58.000000 act-workers-2.1.9/test/test_argus_case.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2360 2022-02-02 11:57:58.000000 act-workers-2.1.9/test/test_config.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2071 2022-08-05 06:45:05.000000 act-workers-2.1.9/test/test_misp.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3512 2022-03-29 08:14:21.000000 act-workers-2.1.9/test/test_scio.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3815 2022-02-02 11:57:58.000000 act-workers-2.1.9/test/test_worker.py
```

### Comparing `act-workers-2.1.8/LICENSE` & `act-workers-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/PKG-INFO` & `act-workers-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: act-workers
-Version: 2.1.8
+Version: 2.1.9
 Summary: ACT workers
 Home-page: https://github.com/mnemonic-no/act-workers
 Author: mnemonic AS
 Author-email: opensource@mnemonic.no
 License: ISC
 Keywords: ACT,mnemonic
 Classifier: Development Status :: 4 - Beta
```

### Comparing `act-workers-2.1.8/README.md` & `act-workers-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/act_feed.py` & `act-workers-2.1.9/act/workers/act_feed.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/alienvault_otx.py` & `act-workers-2.1.9/act/workers/alienvault_otx.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/argus_case.py` & `act-workers-2.1.9/act/workers/argus_case.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/attack.py` & `act-workers-2.1.9/act/workers/attack.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/country_regions.py` & `act-workers-2.1.9/act/workers/country_regions.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/etc/act.ini` & `act-workers-2.1.9/act/workers/etc/act.ini`

 * *Files 1% similar despite different names*

```diff
@@ -254,7 +254,14 @@
 origin-description = FireEye Threat Intelligence (isight)
 access-mode = RoleBased
 # publickey =
 # privatekey =
 # root = https://api.isightpartners.com
 # days = 1
 # debugdir =
+
+[mandiant_ti]
+origin-name = mandiant
+origin-description = Mandiant Threat Intelligence
+access-mode = RoleBased
+# key =
+# secret =
```

### Comparing `act-workers-2.1.8/act/workers/fact_chain_helper.py` & `act-workers-2.1.9/act/workers/fact_chain_helper.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/generic_uploader.py` & `act-workers-2.1.9/act/workers/generic_uploader.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/hybrid_analysis_feed.py` & `act-workers-2.1.9/act/workers/hybrid_analysis_feed.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/ip_asn_history.py` & `act-workers-2.1.9/act/workers/ip_asn_history.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/ip_filter.py` & `act-workers-2.1.9/act/workers/ip_filter.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/isight.py` & `act-workers-2.1.9/act/workers/isight.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/libs/argus.py` & `act-workers-2.1.9/act/workers/libs/argus.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/libs/misp.py` & `act-workers-2.1.9/act/workers/libs/misp.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/libs/mnemonic.py` & `act-workers-2.1.9/act/workers/libs/mnemonic.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/libs/ta_list_methods.py` & `act-workers-2.1.9/act/workers/libs/ta_list_methods.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/libs/urlcache.py` & `act-workers-2.1.9/act/workers/libs/urlcache.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/libs/worker.py` & `act-workers-2.1.9/act/workers/libs/worker.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/misp_feeds.py` & `act-workers-2.1.9/act/workers/misp_feeds.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/mnemonic_pdns.py` & `act-workers-2.1.9/act/workers/mnemonic_pdns.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/scio.py` & `act-workers-2.1.9/act/workers/scio.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/search_graph.py` & `act-workers-2.1.9/act/workers/search_graph.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/shadowserver_asn.py` & `act-workers-2.1.9/act/workers/shadowserver_asn.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/shadowserver_enrich.py` & `act-workers-2.1.9/act/workers/shadowserver_enrich.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/ta_helper.py` & `act-workers-2.1.9/act/workers/veris.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,407 +1,403 @@
 #!/usr/bin/env python3
 
-"""
-Threat Actor Helper worker
+"""Veris worker for the ACT platform
 
-Create common placeholders based on known information.
+Copyright 2019 the ACT project <opensource@mnemonic.no>
 
+Permission to use, copy, modify, and/or distribute this software for any
+purpose with or without fee is hereby granted, provided that the above
+copyright notice and this permission notice appear in all copies.
+
+THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
+INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
+LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
+OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
+PERFORMANCE OF THIS SOFTWARE.
 """
 
 import argparse
-import functools
+import csv
+import io
+import json
+import os
+import re
 import sys
 import traceback
-from logging import error
-from typing import Dict, List, Text
+import zipfile
+from logging import error, warning
+from typing import Any, Dict, Optional, Text, Union, cast
 
 import act.api
-from act.api.helpers import Act, handle_facts
+import requests
+from act.api.helpers import handle_fact, handle_facts
 from act.api.libs import cli
-from pyattck import Attck
 
-from act.workers import worker_config
-from act.workers.libs import worker
+from act.workers.libs import urlcache, worker
+
+VERSION = "0.1"
+ISO_3166_FILE = (
+    "https://raw.githubusercontent.com/lukes/"
+    + "ISO-3166-Countries-with-Regional-Codes/master/all/all.json"
+)
+
+
+def get_cn_map(filename: Text) -> Dict:
+    """
+    Read file with county information (ISO 3166 from filename)
+    return map with country code (e.g. "NO") as key, and Country
+    Name (e.g. "Norway" as value)
+    """
+    cn_map = {}
 
+    for c_map in json.loads(open(filename, "r", encoding="utf8").read()):
+        cn_map[c_map["alpha-2"]] = c_map["name"]
 
-class VocabularyException(Exception):
-    pass
+    return cn_map
 
 
 def parseargs() -> argparse.ArgumentParser:
     """Parse arguments"""
-    parser = worker.parseargs("Threat Actor helper")
-    parser.add_argument("--ta", "--threat-actor", help="Threat Actor")
-    parser.add_argument("--ta-located-in", help="Threat Actor located in")
-    parser.add_argument("--campaign", help="Campaign")
+    parser = worker.parseargs("Shadowserver ASN enrichment")
     parser.add_argument(
-        "--techniques",
-        type=worker_config.string_list,
-        default=[],
-        help="Techniques (Commaseparated list)",
+        "--country-codes",
+        help="Should point to file downloaded from {}".format(ISO_3166_FILE),
     )
     parser.add_argument(
-        "--tools",
-        type=worker_config.string_list,
-        default=[],
-        help="Tools (Commaseparated list)",
+        "--veris-campaign", help="Read mapping of veris campaign from (CSV) file"
     )
     parser.add_argument(
-        "--sectors",
-        type=worker_config.string_list,
-        default=[],
-        help="Sectors (Commaseparated list)",
+        "--threat-actor-variety",
+        help="Varieties to use as Threat Actors",
+        default="Activist, Organized crime, Nation-state",
     )
     parser.add_argument(
-        "--target-countries",
-        type=worker_config.string_list,
-        default=[],
-        help="Target Countries (Commaseparated list)",
+        "--hash-url-matching",
+        help="Download and hash references matching regular expression",
+        default=r"^(.*pdf)$",
     )
     parser.add_argument(
-        "--country-region",
-        default="https://raw.githubusercontent.com/lukes/ISO-3166-Countries-with-Regional-Codes/master/all/all.json",
-        help="Country region in json format (HTTP URL or file)",
+        "--veris-prefix",
+        help='Prefix for incidents and campaign IDs. E.g use "VCDB" for Veris Community Database"',
     )
-
-    # Stix Vocabulary
+    parser.add_argument("--veris-url", help="Read veris incidents from URL.")
+    parser.add_argument("--veris-file", help="Read veris incidents from File.")
     parser.add_argument(
-        "--sector-vocabulary",
-        default="https://raw.githubusercontent.com/mnemonic-no/act-scio2/master/act/scio/etc/plugins/sectors.cfg",
-        help="Sector vocabulary (STIX2, in scio format). Fetched from URL or file",
+        "--stdin", action="store_true", help="Read veris incidents on stdin."
     )
-
     return parser
 
 
-def levenshtein(a: Text, b: Text) -> int:
-    "Calculates the Levenshtein distance between a and b."
-
-    n, m = len(a), len(b)
-    if n > m:
-        # Make sure n <= m, to use O(min(n,m)) space
-        a, b = b, a
-        n, m = m, n
-
-    current = list(range(n + 1))
-    for i in range(1, m + 1):
-        previous, current = current, [i] + [0] * n
-        for j in range(1, n + 1):
-            add, delete = previous[j] + 1, current[j - 1] + 1
-            change = previous[j - 1]
-            if a[j - 1] != b[i - 1]:
-                change = change + 1
-            current[j] = min(add, delete, change)
+def handle_reports(
+    config: Dict[Text, Any], incident: Dict[Text, Any], incident_id: Text
+) -> None:
+    """
+    Extract all references in incident. For each (URL-)reference, check whether we should
+    download the content and creaa a sha256 hash digest of it (must match config["hash_url_matching"]).
+    The sha256 hash is also cached locally.
+    """
 
-    return current[n]
+    # Split references by ";"
+    references = [
+        ref.strip() for ref in incident.get("reference", "").split(";") if ref.strip()
+    ]
+
+    if references:
+        for ref in references:
+            if not re.search(config["hash_url_matching"], ref):
+                continue
+
+            report_hash = config["db_cache"].query_download_update(ref)
+
+            if report_hash:
+                handle_fact(
+                    config["actapi"]
+                    .fact("mentions")
+                    .source("report", report_hash)
+                    .destination("incident", incident_id),
+                    output_format=config["output_format"],
+                )
 
 
-def find_levenshtein_candiates(value: Text, vocabulary: List, n_items: int = 3) -> List:
-    "Return top N list of possible levenshtein candidates"
+def handle_organizations(
+    config: Dict[Text, Any], incident: Dict[Text, Any], incident_id: Text
+) -> None:
+    """
+    Create facts:
+        * incident -targets-> organization
+        * organization -locatedIn-> country
+    """
+    victim = incident.get("victim", {}).get("victim_id")
 
-    possible_match = []
+    if not victim:
+        return
 
-    for entry in set(vocabulary):
-        possible_match.append([levenshtein(value, entry), entry])
+    handle_fact(
+        config["actapi"]
+        .fact("targets")
+        .source("incident", incident_id)
+        .destination("organization", victim),
+        output_format=config["output_format"],
+    )
 
-    return [x[1] for x in sorted(possible_match)[:n_items] if x[1]]
+    for country_code in incident.get("victim", {}).get("country", []):
+        country = config["cn_map"].get(country_code)
 
+        if country:
+            handle_fact(
+                config["actapi"]
+                .fact("locatedIn")
+                .source("organization", victim)
+                .destination("country", country),
+                output_format=config["output_format"],
+            )
 
-@functools.lru_cache(32)
-def fetch_country_regions(
-    country_region: Text, proxy_string: Text, http_timeout: int
-) -> Dict[Text, Text]:
-    "Fetch ISO-3166 list of country/regions"
 
-    vocabulary: Dict = {}
+def handle_threat_actor(
+    config: Dict[Text, Any], incident: Dict[Text, Any], incident_id: Text
+) -> None:
+    """
+    Creat facts from actor->external, where the variety includes at least on variety specified in config["threat_actor_variety"]
 
-    for c_map in worker.fetch_json(country_region, proxy_string, http_timeout):
-        country = c_map["name"]
-        vocabulary[country.lower()] = country
+    """
 
-    return vocabulary
+    external_actor = incident.get("actor", {}).get("external", {})
 
+    if not external_actor:
+        return  # No threat actors
 
-@functools.lru_cache(32)
-def fetch_sector(
-    sector_vocabulary: Text, proxy_string: Text, http_timeout: int
-) -> Dict[Text, Text]:
-    "Fetch STIX2 sector vocabulary"
+    # Varieties are "tags" on actors and we do not want to include all type of actors
+    # Make sure at least one of the varieties are in the list of the configured varieties to include
+    if any(
+        [
+            variety in config["threat_actor_variety"]
+            for variety in external_actor.get("variety", [])
+        ]
+    ):
+        threat_actors = [
+            ta.strip()
+            for ta in incident.get("actor", {}).get("external", {}).get("name", [])
+        ]
 
-    vocabulary: Dict = {}
+        for ta in threat_actors:
+            handle_fact(
+                config["actapi"]
+                .fact("attributedTo")
+                .source("incident", incident_id)
+                .destination("threatActor", ta),
+                output_format=config["output_format"],
+            )
 
-    # format=
-    # name: alias1,alias2,...aliasN
-    for line in worker.fetch(sector_vocabulary, proxy_string, http_timeout).split("\n"):
-        if not line.strip():
-            continue
 
-        name, aliases = line.split(":", 1)
+def handle_tool(
+    config: Dict[Text, Any], incident: Dict[Text, Any], incident_id: Text
+) -> None:
+    "Create content -classifiedAs-> tool, and fact chain from content to incident."
 
-        vocabulary[name] = name
+    # Both "," and ";" are used to separate tools :(
 
-        for alias in [a.strip() for a in aliases.split(",")]:
-            vocabulary[alias] = name
+    tools = [
+        malware.strip().lower()
+        for malware in re.split(
+            r";|,", incident.get("action", {}).get("malware", {}).get("name", "")
+        )
+        if malware
+    ]
 
-    return vocabulary
+    for tool in tools:
+        handle_facts(
+            act.api.fact.fact_chain(
+                config["actapi"]
+                .fact("classifiedAs")
+                .source("content", "*")
+                .destination("tool", tool),
+                config["actapi"]
+                .fact("observedIn")
+                .source("content", "*")
+                .destination("incident", incident_id),
+            ),
+            output_format=config["output_format"],
+        )
 
 
-@functools.lru_cache(32)
-def mitre_techniques() -> Dict[Text, Text]:
+def handle_campaign(
+    config: Dict[Text, Any], incident: Dict[Text, Any], incident_id: Text
+) -> None:
     """
-    Get list of all MITRE ATT&CK techniques and return map combined with
-    both technique IDs and (lowercased) name as key an name as value
+    Create incident -attributedTo-> campaign facts
+    If we have a mapping from campaign (UUID) to name, a campaign -name-> will also be created
     """
 
-    attack = Attck()
-    techniques = {}
-
-    for technique in attack.enterprise.techniques:
-        techniques[technique.id] = technique.name
-        techniques[technique.name.lower()] = technique.name
+    campaign = (
+        "{}-{}".format(config["veris_prefix"], incident["campaign_id"])
+        if incident.get("campaign_id")
+        else None
+    )
 
-    return techniques
+    if not campaign:
+        return
 
+    handle_fact(
+        config["actapi"]
+        .fact("attributedTo")
+        .source("incident", incident_id)
+        .destination("campaign", campaign),
+        output_format=config["output_format"],
+    )
 
-def technique_lookup(technique: Text) -> Text:
-    "Lookup technique and return name if exists, otherwise raise VocabularyException"
-    techniques = mitre_techniques()
+    name = config["campaign_map"].get(format(campaign))
 
-    try:
-        return techniques[technique]
-    except KeyError:
-        raise VocabularyException(
-            "Technique {} not found in MITRE ATT&CK. Nearest matches: {}".format(
-                technique,
-                ", ".join(find_levenshtein_candiates(technique, techniques.keys())),
-            )
+    if name:
+        handle_fact(
+            config["actapi"].fact("name", name).source("campaign", campaign),
+            output_format=config["output_format"],
         )
 
-
-def country_lookup(args: argparse.Namespace, country: Text) -> Text:
-    "Lookup country and return name if exists, otherwise raise VocabularyException"
-    vocabulary = fetch_country_regions(
-        args.country_region, args.proxy_string, args.http_timeout
-    )
-
-    try:
-        return vocabulary[country.lower()]
-    except KeyError:
-        raise VocabularyException(
-            "Country {} not found in ISO 3166 database. Nearest matches: {}".format(
-                country,
-                ", ".join(find_levenshtein_candiates(country, vocabulary.values())),
+    else:
+        warning(
+            "No name found for campaign {}. Make sure veris-campaign is provided and the ID is included in csv field (without prefix)".format(
+                campaign
             )
         )
 
 
-def sector_lookup(args: argparse.Namespace, sector: Text) -> Text:
-    "Lookup sector and return name if exists, otherwise raise VocabularyException"
+def handle_incident(config: Dict[Text, Any], incident: Dict[Text, Any]) -> None:
+    """handle veris incidents"""
 
-    vocabulary = fetch_sector(
-        args.sector_vocabulary, args.proxy_string, args.http_timeout
-    )
+    incident_id = "{}-{}".format(config["veris_prefix"], incident["incident_id"])
 
-    try:
-        return vocabulary[sector.lower()]
-    except KeyError:
-        raise VocabularyException(
-            "Sector {} not found in Stix vocabulary. Nearest matches: {}".format(
-                sector, ", ".join(find_levenshtein_candiates(sector, vocabulary))
-            )
-        )
+    handle_reports(config, incident, incident_id)
+    handle_organizations(config, incident, incident_id)
+    handle_tool(config, incident, incident_id)
+    handle_threat_actor(config, incident, incident_id)
+    handle_campaign(config, incident, incident_id)
 
 
-def add_ta_techniques(
-    client: Act, output_format: Text, threat_actor: Text, techniques: List[Text]
-) -> None:
-    """Threat Actor Techniques"""
+def handle_zip_file(config: Dict[Text, Any], zfile: Union[Text, io.BytesIO]) -> None:
+    "Read incident form all (json) files in zip file"
 
-    for technique in techniques:
-        handle_facts(
-            act.api.fact.fact_chain(
-                client.fact("attributedTo")
-                .source("incident", "*")
-                .destination("threatActor", threat_actor),
-                client.fact("observedIn")
-                .source("technique", technique)
-                .destination("incident", "*"),
-            ),
-            output_format=output_format,
-        )
+    # ZipFile accepts both file names (str) and file like objects
+    zf = zipfile.ZipFile(zfile, "r")
 
+    for fileinfo in zf.infolist():
+        for incident in json.loads(zf.read(fileinfo).decode("utf-8")):
+            handle_incident(config, incident)
 
-def add_ta_tools(
-    client: Act, output_format: Text, threat_actor: Text, tools: List[Text]
-) -> None:
-    """Threat Actor Tools"""
 
-    for tool in tools:
-        handle_facts(
-            act.api.fact.fact_chain(
-                client.fact("classifiedAs")
-                .source("content", "*")
-                .destination("tool", tool),
-                client.fact("observedIn")
-                .source("content", "*")
-                .destination("incident", "*"),
-                client.fact("attributedTo")
-                .source("incident", "*")
-                .destination("threatActor", threat_actor),
-            ),
-            output_format=output_format,
-        )
+def process(config: Dict[Text, Any]) -> None:
+    "Process inicdent from stdin, url or file. URL and File supports zipped files in zip-format."
 
+    # Read incident from stdin
+    if config["stdin"]:
+        for incident in sys.stdin.read().split("\n"):
+            handle_incident(config, json.loads(incident))
 
-def add_ta_sectors(
-    client: Act, output_format: Text, threat_actor: Text, sectors: List[Text]
-) -> None:
-    """Threat Actor Sectors"""
-    for sector in sectors:
-        handle_facts(
-            act.api.fact.fact_chain(
-                client.fact("targets")
-                .source("incident", "*")
-                .destination("organization", "*"),
-                client.fact("memberOf")
-                .source("organization", "*")
-                .destination("sector", sector),
-                client.fact("attributedTo")
-                .source("incident", "*")
-                .destination("threatActor", threat_actor),
-            ),
-            output_format=output_format,
-        )
+        return
 
-
-def add_ta_target_country(
-    client: Act, output_format: Text, threat_actor: Text, target_countries: List[Text]
-) -> None:
-    """Threat actor target countries"""
-    for target_country in target_countries:
-        handle_facts(
-            act.api.fact.fact_chain(
-                client.fact("targets")
-                .source("incident", "*")
-                .destination("organization", "*"),
-                client.fact("locatedIn")
-                .source("organization", "*")
-                .destination("country", target_country),
-                client.fact("attributedTo")
-                .source("incident", "*")
-                .destination("threatActor", threat_actor),
-            ),
-            output_format=output_format,
+    # Download incidents from URL
+    if config["veris_url"]:
+        req = requests.get(
+            config["veris_url"],
+            proxies=config["proxies"],
+            timeout=config["http_timeout"],
         )
+        if config["veris_url"].endswith(".zip"):
+            handle_zip_file(config, io.BytesIO(req.content))
+        else:
+            for incident in req.json():
+                handle_incident(config, cast(Dict, incident))
+        return
+
+    # Read incidents from file
+    if config["veris_file"]:
+        if config["veris_file"].endswith(".zip"):
+            handle_zip_file(config, config["veris_file"])
+        else:
+            with open(config["veris_file"]) as f:
+                for incident in json.loads(f.read()):
+                    handle_incident(config, cast(Dict, incident))
+        return
 
+    error("Must specifiy either --stdin, --veris-url or --veris-file")
 
-def add_ta_located_in(
-    client: Act, output_format: Text, threat_actor: Text, located_in: Text
-) -> None:
-    """Threat actor located in"""
-    handle_facts(
-        act.api.fact.fact_chain(
-            client.fact("locatedIn")
-            .source("organization", "*")
-            .destination("country", located_in),
-            client.fact("attributedTo")
-            .source("threatActor", threat_actor)
-            .destination("organization", "*"),
-        ),
-        output_format=output_format,
-    )
 
-
-def add_ta_campaign(
-    client: Act, output_format: Text, threat_actor: Text, campaign: Text
-) -> None:
-    """Threat Actor Campaign"""
-    handle_facts(
-        act.api.fact.fact_chain(
-            client.fact("attributedTo")
-            .source("incident", "*")
-            .destination("campaign", campaign),
-            client.fact("attributedTo")
-            .source("incident", "*")
-            .destination("threatActor", threat_actor),
-        ),
-        output_format=output_format,
-    )
+def get_campaigns(veris_prefix: Text, filename: Text) -> Optional[Dict[Text, Text]]:
+    """
+    Get mapping from campaign (UUID) to name
+    """
+    with open(filename) as csvfile:
+        return {
+            "{}-{}".format(veris_prefix, row[0]): row[1]
+            for row in csv.reader(csvfile, delimiter=",")
+        }
 
 
 def main() -> None:
-    """Main function"""
+    """main function"""
 
     # Look for default ini file in "/etc/actworkers.ini" and ~/config/actworkers/actworkers.ini
     # (or replace .config with $XDG_CONFIG_DIR if set)
     args = cli.handle_args(parseargs())
-
     actapi = worker.init_act(args)
 
-    if not args.ta:
-        sys.stderr.write("You must specify Threat Actor with --ta <THREAT ACTOR>\n")
-        sys.exit(1)
-
-    # Normalize and lookup country/technique/sectors
-    # Print error with suggested match if not found
-    ok = True
+    if not args.country_codes:
+        cli.fatal("You must specify --country-codes on command line or in config file")
 
-    try:
-        args.target_countries = [
-            country_lookup(args, country) for country in args.target_countries
-        ]
-    except (VocabularyException, FileNotFoundError, worker.UnsupportedScheme) as e:
-        sys.stderr.write(str(e))
-        ok = False
+    if not args.veris_prefix:
+        cli.fatal("You must specify --veris-prefix")
 
-    try:
-        args.techniques = [technique_lookup(tech) for tech in args.techniques]
-    except VocabularyException as e:
-        sys.stderr.write(str(e))
-        ok = False
+    if not (args.veris_url or args.veris_file or args.stdin):
+        cli.fatal("You must specify --veris-url, --veris-file or --stdin")
 
-    try:
-        if args.ta_located_in:
-            args.ta_located_in = country_lookup(args, args.ta_located_in)
-    except VocabularyException as e:
-        sys.stderr.write(str(e))
-        ok = False
+    args.veris_prefix = args.veris_prefix.upper()
 
-    try:
-        args.sectors = [sector_lookup(args, sector) for sector in args.sectors]
-    except VocabularyException as e:
-        sys.stderr.write(str(e))
-        ok = False
-
-    if not ok:
-        sys.exit(1)
-
-    if args.target_countries:
-        add_ta_target_country(
-            actapi, args.output_format, args.ta, args.target_countries
+    if not os.path.isfile(args.country_codes):
+        cli.fatal(
+            "Country/region file not found at specified location: {}".format(
+                args.country_codes
+            ),
+            2,
         )
 
-    if args.campaign:
-        add_ta_campaign(actapi, args.output_format, args.ta, args.campaign)
-
-    if args.tools:
-        add_ta_tools(actapi, args.output_format, args.ta, args.tools)
-
-    if args.techniques:
-        add_ta_techniques(actapi, args.output_format, args.ta, args.techniques)
+    args.threat_actor_variety = [
+        variety.strip() for variety in args.threat_actor_variety.split(",")
+    ]
+
+    # Configuration object that will be passed around to functions
+    config = {
+        # act API
+        "actapi": actapi,
+        # Map of CC -> Country Name
+        "cn_map": get_cn_map(args.country_codes),
+        # Map of CC -> Country Name
+        "campaign_map": get_campaigns(args.veris_prefix, args.veris_campaign)
+        if args.veris_campaign
+        else {},
+        # Cache of url > sha256
+        "db_cache": urlcache.URLCache(
+            requests_common_kwargs={
+                "proxies": {"http": args.proxy_string, "https": args.proxy_string},
+                "timeout": args.http_timeout,
+            }
+        ),
+        "proxies": {"http": args.proxy_string, "https": args.proxy_string}
+        if args.proxy_string
+        else None,
+    }
 
-    if args.sectors:
-        add_ta_sectors(actapi, args.output_format, args.ta, args.sectors)
+    # Add all arguments from args to config
+    config.update(vars(args))
 
-    if args.ta_located_in:
-        add_ta_located_in(actapi, args.output_format, args.ta, args.ta_located_in)
+    process(config)
 
 
 def main_log_error() -> None:
-    "Call main() and log all excetions  as errors"
+    "Main function. Log all exceptions to error"
     try:
         main()
     except Exception:
         error("Unhandled exception: {}".format(traceback.format_exc()))
         raise
```

### Comparing `act-workers-2.1.8/act/workers/template.py` & `act-workers-2.1.9/act/workers/template.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/thaicert.py` & `act-workers-2.1.9/act/workers/thaicert.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/tool_alias.py` & `act-workers-2.1.9/act/workers/tool_alias.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/update_ta_aliases_list.py` & `act-workers-2.1.9/act/workers/update_ta_aliases_list.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/url_shorter_unpack.py` & `act-workers-2.1.9/act/workers/url_shorter_unpack.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/vt.py` & `act-workers-2.1.9/act/workers/vt.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act/workers/worker_config.py` & `act-workers-2.1.9/act/workers/worker_config.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/act_workers.egg-info/PKG-INFO` & `act-workers-2.1.9/act_workers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: act-workers
-Version: 2.1.8
+Version: 2.1.9
 Summary: ACT workers
 Home-page: https://github.com/mnemonic-no/act-workers
 Author: mnemonic AS
 Author-email: opensource@mnemonic.no
 License: ISC
 Keywords: ACT,mnemonic
 Classifier: Development Status :: 4 - Beta
```

### Comparing `act-workers-2.1.8/act_workers.egg-info/SOURCES.txt` & `act-workers-2.1.9/act_workers.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 act/workers/country_regions.py
 act/workers/fact_chain_helper.py
 act/workers/generic_uploader.py
 act/workers/hybrid_analysis_feed.py
 act/workers/ip_asn_history.py
 act/workers/ip_filter.py
 act/workers/isight.py
+act/workers/mandiant_ti.py
 act/workers/misp_feeds.py
 act/workers/mnemonic_pdns.py
 act/workers/scio.py
 act/workers/search_graph.py
 act/workers/shadowserver_asn.py
 act/workers/shadowserver_enrich.py
 act/workers/ta_helper.py
@@ -29,14 +30,16 @@
 act/workers/veris.py
 act/workers/vt.py
 act/workers/worker_config.py
 act/workers/etc/act.ini
 act/workers/etc/search_jobs.ini
 act/workers/libs/__init__.py
 act/workers/libs/argus.py
+act/workers/libs/fact_chain.py
+act/workers/libs/mandiant_ti_v4.py
 act/workers/libs/misp.py
 act/workers/libs/mnemonic.py
 act/workers/libs/ta_list_methods.py
 act/workers/libs/urlcache.py
 act/workers/libs/worker.py
 act_workers.egg-info/PKG-INFO
 act_workers.egg-info/SOURCES.txt
```

### Comparing `act-workers-2.1.8/act_workers.egg-info/entry_points.txt` & `act-workers-2.1.9/act_workers.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 act-country-regions = act.workers.country_regions:main_log_error
 act-fact-chain-helper = act.workers.fact_chain_helper:main_log_error
 act-feed = act.workers.act_feed:main_log_error
 act-hybrid-analysis-feed = act.workers.hybrid_analysis_feed:main_log_error
 act-ip-asn-history = act.workers.ip_asn_history:main_log_error
 act-ip-filter = act.workers.ip_filter:main_log_error
 act-isight = act.workers.isight:main_log_error
+act-mandiat-ti = act.workers.mandiant_ti:main_log_error
 act-misp-feeds = act.workers.misp_feeds:main_log_error
 act-mnemonic-pdns = act.workers.mnemonic_pdns:main_log_error
 act-scio = act.workers.scio:main_log_error
 act-search-graph = act.workers.search_graph:main_log_error
 act-shadowserver-asn = act.workers.shadowserver_asn:main_log_error
 act-shadowserver-enrich = act.workers.shadowserver_enrich:main_log_error
 act-ta-helper = act.workers.ta_helper:main_log_error
```

### Comparing `act-workers-2.1.8/setup.py` & `act-workers-2.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), "rb") as f:
     long_description = f.read().decode("utf-8")
 
 setup(
     name="act-workers",
-    version="2.1.8",
+    version="2.1.9",
     author="mnemonic AS",
     zip_safe=True,
     author_email="opensource@mnemonic.no",
     description="ACT workers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="ISC",
@@ -27,14 +27,15 @@
             "act-country-regions = act.workers.country_regions:main_log_error",
             "act-fact-chain-helper = act.workers.fact_chain_helper:main_log_error",
             "act-feed = act.workers.act_feed:main_log_error",
             "act-hybrid-analysis-feed = act.workers.hybrid_analysis_feed:main_log_error",
             "act-ip-asn-history = act.workers.ip_asn_history:main_log_error",
             "act-ip-filter= act.workers.ip_filter:main_log_error",
             "act-isight = act.workers.isight:main_log_error",
+            "act-mandiat-ti = act.workers.mandiant_ti:main_log_error",
             "act-misp-feeds = act.workers.misp_feeds:main_log_error",
             "act-mnemonic-pdns = act.workers.mnemonic_pdns:main_log_error",
             "act-scio = act.workers.scio:main_log_error",
             "act-search-graph = act.workers.search_graph:main_log_error",
             "act-shadowserver-asn = act.workers.shadowserver_asn:main_log_error",
             "act-shadowserver-enrich = act.workers.shadowserver_enrich:main_log_error",
             "act-ta-helper = act.workers.ta_helper:main_log_error",
```

### Comparing `act-workers-2.1.8/test/test_argus_case.py` & `act-workers-2.1.9/test/test_argus_case.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/test/test_config.py` & `act-workers-2.1.9/test/test_config.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/test/test_misp.py` & `act-workers-2.1.9/test/test_misp.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/test/test_scio.py` & `act-workers-2.1.9/test/test_scio.py`

 * *Files identical despite different names*

### Comparing `act-workers-2.1.8/test/test_worker.py` & `act-workers-2.1.9/test/test_worker.py`

 * *Files identical despite different names*

