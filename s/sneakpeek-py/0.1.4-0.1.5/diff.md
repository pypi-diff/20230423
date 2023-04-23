# Comparing `tmp/sneakpeek_py-0.1.4.tar.gz` & `tmp/sneakpeek_py-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneakpeek_py-0.1.4.tar", max compression
+gzip compressed data, was "sneakpeek_py-0.1.5.tar", max compression
```

## Comparing `sneakpeek_py-0.1.4.tar` & `sneakpeek_py-0.1.5.tar`

### file list

```diff
@@ -1,57 +1,167 @@
--rw-r--r--   0        0        0       85 2023-04-02 10:58:33.945002 sneakpeek_py-0.1.4/README.md
--rw-r--r--   0        0        0     1753 2023-04-22 18:46:45.441340 sneakpeek_py-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3483 2023-04-22 18:35:18.037503 sneakpeek_py-0.1.4/sneakpeek/api.py
--rw-r--r--   0        0        0      726 2023-04-10 11:41:30.863384 sneakpeek_py-0.1.4/sneakpeek/lib/errors.py
--rw-r--r--   0        0        0     1325 2023-04-14 20:40:35.860617 sneakpeek_py-0.1.4/sneakpeek/lib/models.py
--rw-r--r--   0        0        0     4637 2023-04-16 16:40:10.652490 sneakpeek_py-0.1.4/sneakpeek/lib/queue.py
--rw-r--r--   0        0        0     2141 2023-04-22 17:36:34.069286 sneakpeek_py-0.1.4/sneakpeek/lib/storage/base.py
--rw-r--r--   0        0        0     9527 2023-04-22 17:37:37.160714 sneakpeek_py-0.1.4/sneakpeek/lib/storage/in_memory_storage.py
--rw-r--r--   0        0        0     9153 2023-04-22 17:38:03.913301 sneakpeek_py-0.1.4/sneakpeek/lib/storage/redis_storage.py
--rw-r--r--   0        0        0     1535 2023-04-15 08:35:07.840371 sneakpeek_py-0.1.4/sneakpeek/logging.py
--rw-r--r--   0        0        0     3291 2023-04-15 13:15:52.422916 sneakpeek_py-0.1.4/sneakpeek/metrics.py
--rw-r--r--   0        0        0     1338 2023-04-15 14:28:45.826848 sneakpeek_py-0.1.4/sneakpeek/plugins/proxy_plugin.py
--rw-r--r--   0        0        0     4209 2023-04-15 10:43:26.332501 sneakpeek_py-0.1.4/sneakpeek/plugins/rate_limiter_plugin.py
--rw-r--r--   0        0        0     2062 2023-04-15 10:43:18.016302 sneakpeek_py-0.1.4/sneakpeek/plugins/requests_logging_plugin.py
--rw-r--r--   0        0        0     3747 2023-04-15 10:43:12.817939 sneakpeek_py-0.1.4/sneakpeek/plugins/robots_txt_plugin.py
--rw-r--r--   0        0        0     1391 2023-04-15 14:24:15.543165 sneakpeek_py-0.1.4/sneakpeek/plugins/user_agent_injecter_plugin.py
--rw-r--r--   0        0        0      659 2023-04-15 07:08:31.686879 sneakpeek_py-0.1.4/sneakpeek/plugins/utils.py
--rw-r--r--   0        0        0     3344 2023-04-16 16:37:19.181274 sneakpeek_py-0.1.4/sneakpeek/runner.py
--rw-r--r--   0        0        0    11264 2023-04-16 16:40:24.540096 sneakpeek_py-0.1.4/sneakpeek/scheduler.py
--rw-r--r--   0        0        0      172 2023-04-14 20:22:32.213615 sneakpeek_py-0.1.4/sneakpeek/scraper_config.py
--rw-r--r--   0        0        0     6956 2023-04-16 16:36:12.560412 sneakpeek_py-0.1.4/sneakpeek/scraper_context.py
--rw-r--r--   0        0        0      282 2023-04-14 20:58:00.201559 sneakpeek_py-0.1.4/sneakpeek/scraper_handler.py
--rw-r--r--   0        0        0     3682 2023-04-22 18:44:30.263917 sneakpeek_py-0.1.4/sneakpeek/server.py
--rw-r--r--   0        0        0      550 2023-04-22 18:35:47.148387 sneakpeek_py-0.1.4/sneakpeek/static/assets/ErrorNotFound.9617f9a7.js
--rw-r--r--   0        0        0    20436 2023-04-22 18:35:47.145054 sneakpeek_py-0.1.4/sneakpeek/static/assets/KFOkCnqEu92Fr1MmgVxIIzQ.34e9582c.woff
--rw-r--r--   0        0        0    20544 2023-04-22 18:35:47.146248 sneakpeek_py-0.1.4/sneakpeek/static/assets/KFOlCnqEu92Fr1MmEU9fBBc-.9ce7f3ac.woff
--rw-r--r--   0        0        0    20416 2023-04-22 18:35:47.146208 sneakpeek_py-0.1.4/sneakpeek/static/assets/KFOlCnqEu92Fr1MmSU5fBBc-.bf14c7d7.woff
--rw-r--r--   0        0        0    20408 2023-04-22 18:35:47.146455 sneakpeek_py-0.1.4/sneakpeek/static/assets/KFOlCnqEu92Fr1MmWUlfBBc-.e0fd57c0.woff
--rw-r--r--   0        0        0    20424 2023-04-22 18:35:47.146125 sneakpeek_py-0.1.4/sneakpeek/static/assets/KFOlCnqEu92Fr1MmYUtfBBc-.f6537e32.woff
--rw-r--r--   0        0        0    20344 2023-04-22 18:35:47.146188 sneakpeek_py-0.1.4/sneakpeek/static/assets/KFOmCnqEu92Fr1Mu4mxM.f2abf7fb.woff
--rw-r--r--   0        0        0    24866 2023-04-22 18:35:47.146431 sneakpeek_py-0.1.4/sneakpeek/static/assets/MainLayout.06dc30a3.js
--rw-r--r--   0        0        0      538 2023-04-22 18:35:47.148607 sneakpeek_py-0.1.4/sneakpeek/static/assets/NewScraperPage.abf42128.js
--rw-r--r--   0        0        0    30651 2023-04-22 18:35:47.148410 sneakpeek_py-0.1.4/sneakpeek/static/assets/PriorityChip.61343a15.js
--rw-r--r--   0        0        0      655 2023-04-22 18:35:47.146487 sneakpeek_py-0.1.4/sneakpeek/static/assets/QList.7f24c43e.js
--rw-r--r--   0        0        0    76403 2023-04-22 18:35:47.148351 sneakpeek_py-0.1.4/sneakpeek/static/assets/QPage.6206ab40.js
--rw-r--r--   0        0        0  1333182 2023-04-22 18:35:47.148573 sneakpeek_py-0.1.4/sneakpeek/static/assets/ScraperEditForm.197dd68f.js
--rw-r--r--   0        0        0     3323 2023-04-22 18:35:47.148364 sneakpeek_py-0.1.4/sneakpeek/static/assets/ScraperEditForm.640de0df.css
--rw-r--r--   0        0        0    26587 2023-04-22 18:35:47.148377 sneakpeek_py-0.1.4/sneakpeek/static/assets/ScraperPage.732b3035.js
--rw-r--r--   0        0        0     2479 2023-04-22 18:35:47.148321 sneakpeek_py-0.1.4/sneakpeek/static/assets/ScrapersPage.06097019.js
--rw-r--r--   0        0        0    11097 2023-04-22 18:35:47.146471 sneakpeek_py-0.1.4/sneakpeek/static/assets/api.8025d512.js
--rw-r--r--   0        0        0   187208 2023-04-22 18:35:47.146352 sneakpeek_py-0.1.4/sneakpeek/static/assets/fa-brands-400.20c4a58b.ttf
--rw-r--r--   0        0        0   108020 2023-04-22 18:35:47.146608 sneakpeek_py-0.1.4/sneakpeek/static/assets/fa-brands-400.74833209.woff2
--rw-r--r--   0        0        0    63952 2023-04-22 18:35:47.146236 sneakpeek_py-0.1.4/sneakpeek/static/assets/fa-regular-400.528d022d.ttf
--rw-r--r--   0        0        0    24948 2023-04-22 18:35:47.146154 sneakpeek_py-0.1.4/sneakpeek/static/assets/fa-regular-400.8e7e5ea1.woff2
--rw-r--r--   0        0        0   394628 2023-04-22 18:35:47.146414 sneakpeek_py-0.1.4/sneakpeek/static/assets/fa-solid-900.67a65763.ttf
--rw-r--r--   0        0        0   150124 2023-04-22 18:35:47.146277 sneakpeek_py-0.1.4/sneakpeek/static/assets/fa-solid-900.7152a693.woff2
--rw-r--r--   0        0        0    10172 2023-04-22 18:35:47.146502 sneakpeek_py-0.1.4/sneakpeek/static/assets/fa-v4compatibility.0515a423.ttf
--rw-r--r--   0        0        0     4564 2023-04-22 18:35:47.146294 sneakpeek_py-0.1.4/sneakpeek/static/assets/fa-v4compatibility.694a17c3.woff2
--rw-r--r--   0        0        0   164912 2023-04-22 18:35:47.146665 sneakpeek_py-0.1.4/sneakpeek/static/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.fd84f88b.woff
--rw-r--r--   0        0        0   128616 2023-04-22 18:35:47.146319 sneakpeek_py-0.1.4/sneakpeek/static/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.4a4dbc62.woff2
--rw-r--r--   0        0        0   132320 2023-04-22 18:35:47.146538 sneakpeek_py-0.1.4/sneakpeek/static/assets/index.422cc3a0.js
--rw-r--r--   0        0        0   307194 2023-04-22 18:35:47.148448 sneakpeek_py-0.1.4/sneakpeek/static/assets/index.99b1d043.css
--rw-r--r--   0        0        0    64483 2023-04-22 18:35:46.776382 sneakpeek_py-0.1.4/sneakpeek/static/favicon.ico
--rw-r--r--   0        0        0     2359 2023-04-22 18:35:46.776784 sneakpeek_py-0.1.4/sneakpeek/static/icons/favicon.png
--rw-r--r--   0        0        0      659 2023-04-22 18:35:47.148589 sneakpeek_py-0.1.4/sneakpeek/static/index.html
--rw-r--r--   0        0        0     3444 2023-04-16 14:06:00.425497 sneakpeek_py-0.1.4/sneakpeek/worker.py
--rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 sneakpeek_py-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     5422 2023-04-23 21:11:03.986542 sneakpeek_py-0.1.5/README.md
+-rw-r--r--   0        0        0     2164 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4660 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/api.py
+-rw-r--r--   0        0        0      715 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/lib/errors.py
+-rw-r--r--   0        0        0     3226 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/lib/models.py
+-rw-r--r--   0        0        0     6988 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/lib/queue.py
+-rw-r--r--   0        0        0     6083 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/lib/storage/base.py
+-rw-r--r--   0        0        0    10242 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/lib/storage/in_memory_storage.py
+-rw-r--r--   0        0        0    10439 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/lib/storage/redis_storage.py
+-rw-r--r--   0        0        0     2918 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/logging.py
+-rw-r--r--   0        0        0     4750 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/metrics.py
+-rw-r--r--   0        0        0     1560 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/plugins/proxy_plugin.py
+-rw-r--r--   0        0        0     4969 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/plugins/rate_limiter_plugin.py
+-rw-r--r--   0        0        0     2273 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/plugins/requests_logging_plugin.py
+-rw-r--r--   0        0        0     4120 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/plugins/robots_txt_plugin.py
+-rw-r--r--   0        0        0     1755 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/plugins/user_agent_injecter_plugin.py
+-rw-r--r--   0        0        0      659 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/plugins/utils.py
+-rw-r--r--   0        0        0     4453 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/runner.py
+-rw-r--r--   0        0        0    13593 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/scheduler.py
+-rw-r--r--   0        0        0      527 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/scraper_config.py
+-rw-r--r--   0        0        0    10263 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/scraper_context.py
+-rw-r--r--   0        0        0      655 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/scraper_handler.py
+-rw-r--r--   0        0        0     7650 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/server.py
+-rw-r--r--   0        0        0      550 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/static/assets/ErrorNotFound.9617f9a7.js
+-rw-r--r--   0        0        0    20436 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/static/assets/KFOkCnqEu92Fr1MmgVxIIzQ.34e9582c.woff
+-rw-r--r--   0        0        0    20544 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/static/assets/KFOlCnqEu92Fr1MmEU9fBBc-.9ce7f3ac.woff
+-rw-r--r--   0        0        0    20416 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/static/assets/KFOlCnqEu92Fr1MmSU5fBBc-.bf14c7d7.woff
+-rw-r--r--   0        0        0    20408 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/static/assets/KFOlCnqEu92Fr1MmWUlfBBc-.e0fd57c0.woff
+-rw-r--r--   0        0        0    20424 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/static/assets/KFOlCnqEu92Fr1MmYUtfBBc-.f6537e32.woff
+-rw-r--r--   0        0        0    20344 2023-04-23 21:11:03.994542 sneakpeek_py-0.1.5/sneakpeek/static/assets/KFOmCnqEu92Fr1Mu4mxM.f2abf7fb.woff
+-rw-r--r--   0        0        0    24866 2023-04-23 21:11:03.998542 sneakpeek_py-0.1.5/sneakpeek/static/assets/MainLayout.06dc30a3.js
+-rw-r--r--   0        0        0      538 2023-04-23 21:11:03.998542 sneakpeek_py-0.1.5/sneakpeek/static/assets/NewScraperPage.abf42128.js
+-rw-r--r--   0        0        0    30651 2023-04-23 21:11:03.998542 sneakpeek_py-0.1.5/sneakpeek/static/assets/PriorityChip.61343a15.js
+-rw-r--r--   0        0        0      655 2023-04-23 21:11:03.998542 sneakpeek_py-0.1.5/sneakpeek/static/assets/QList.7f24c43e.js
+-rw-r--r--   0        0        0    76403 2023-04-23 21:11:03.998542 sneakpeek_py-0.1.5/sneakpeek/static/assets/QPage.6206ab40.js
+-rw-r--r--   0        0        0  1333182 2023-04-23 21:11:04.006543 sneakpeek_py-0.1.5/sneakpeek/static/assets/ScraperEditForm.197dd68f.js
+-rw-r--r--   0        0        0     3323 2023-04-23 21:11:04.006543 sneakpeek_py-0.1.5/sneakpeek/static/assets/ScraperEditForm.640de0df.css
+-rw-r--r--   0        0        0    26587 2023-04-23 21:11:04.006543 sneakpeek_py-0.1.5/sneakpeek/static/assets/ScraperPage.732b3035.js
+-rw-r--r--   0        0        0     2479 2023-04-23 21:11:04.006543 sneakpeek_py-0.1.5/sneakpeek/static/assets/ScrapersPage.06097019.js
+-rw-r--r--   0        0        0    11097 2023-04-23 21:11:04.006543 sneakpeek_py-0.1.5/sneakpeek/static/assets/api.8025d512.js
+-rw-r--r--   0        0        0   187208 2023-04-23 21:11:04.006543 sneakpeek_py-0.1.5/sneakpeek/static/assets/fa-brands-400.20c4a58b.ttf
+-rw-r--r--   0        0        0   108020 2023-04-23 21:11:04.006543 sneakpeek_py-0.1.5/sneakpeek/static/assets/fa-brands-400.74833209.woff2
+-rw-r--r--   0        0        0    63952 2023-04-23 21:11:04.006543 sneakpeek_py-0.1.5/sneakpeek/static/assets/fa-regular-400.528d022d.ttf
+-rw-r--r--   0        0        0    24948 2023-04-23 21:11:04.006543 sneakpeek_py-0.1.5/sneakpeek/static/assets/fa-regular-400.8e7e5ea1.woff2
+-rw-r--r--   0        0        0   394628 2023-04-23 21:11:04.010542 sneakpeek_py-0.1.5/sneakpeek/static/assets/fa-solid-900.67a65763.ttf
+-rw-r--r--   0        0        0   150124 2023-04-23 21:11:04.010542 sneakpeek_py-0.1.5/sneakpeek/static/assets/fa-solid-900.7152a693.woff2
+-rw-r--r--   0        0        0    10172 2023-04-23 21:11:04.010542 sneakpeek_py-0.1.5/sneakpeek/static/assets/fa-v4compatibility.0515a423.ttf
+-rw-r--r--   0        0        0     4564 2023-04-23 21:11:04.010542 sneakpeek_py-0.1.5/sneakpeek/static/assets/fa-v4compatibility.694a17c3.woff2
+-rw-r--r--   0        0        0   164912 2023-04-23 21:11:04.010542 sneakpeek_py-0.1.5/sneakpeek/static/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.fd84f88b.woff
+-rw-r--r--   0        0        0   128616 2023-04-23 21:11:04.010542 sneakpeek_py-0.1.5/sneakpeek/static/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.4a4dbc62.woff2
+-rw-r--r--   0        0        0   132320 2023-04-23 21:11:04.014543 sneakpeek_py-0.1.5/sneakpeek/static/assets/index.422cc3a0.js
+-rw-r--r--   0        0        0   307194 2023-04-23 21:11:04.014543 sneakpeek_py-0.1.5/sneakpeek/static/assets/index.99b1d043.css
+-rw-r--r--   0        0        0      230 2023-04-23 21:12:03.378871 sneakpeek_py-0.1.5/sneakpeek/static/docs/.buildinfo
+-rw-r--r--   0        0        0   961226 2023-04-23 21:12:02.278866 sneakpeek_py-0.1.5/sneakpeek/static/docs/.doctrees/api.doctree
+-rw-r--r--   0        0        0     8116 2023-04-23 21:12:02.290866 sneakpeek_py-0.1.5/sneakpeek/static/docs/.doctrees/deployment.doctree
+-rw-r--r--   0        0        0    40371 2023-04-23 21:12:02.326866 sneakpeek_py-0.1.5/sneakpeek/static/docs/.doctrees/design.doctree
+-rw-r--r--   0        0        0    76082 2023-04-23 21:12:02.390867 sneakpeek_py-0.1.5/sneakpeek/static/docs/.doctrees/environment.pickle
+-rw-r--r--   0        0        0     5405 2023-04-23 21:12:02.334866 sneakpeek_py-0.1.5/sneakpeek/static/docs/.doctrees/index.doctree
+-rw-r--r--   0        0        0     3823 2023-04-23 21:12:02.338866 sneakpeek_py-0.1.5/sneakpeek/static/docs/.doctrees/plugins/index.doctree
+-rw-r--r--   0        0        0    13997 2023-04-23 21:12:02.350866 sneakpeek_py-0.1.5/sneakpeek/static/docs/.doctrees/plugins/new_plugin.doctree
+-rw-r--r--   0        0        0     6215 2023-04-23 21:12:02.354866 sneakpeek_py-0.1.5/sneakpeek/static/docs/.doctrees/plugins/proxy_plugin.doctree
+-rw-r--r--   0        0        0     8218 2023-04-23 21:12:02.362866 sneakpeek_py-0.1.5/sneakpeek/static/docs/.doctrees/plugins/rate_limiter_plugin.doctree
+-rw-r--r--   0        0        0     6215 2023-04-23 21:12:02.366866 sneakpeek_py-0.1.5/sneakpeek/static/docs/.doctrees/plugins/requests_logging_plugin.doctree
+-rw-r--r--   0        0        0     6235 2023-04-23 21:12:02.374867 sneakpeek_py-0.1.5/sneakpeek/static/docs/.doctrees/plugins/robots_txt_plugin.doctree
+-rw-r--r--   0        0        0     7249 2023-04-23 21:12:02.378867 sneakpeek_py-0.1.5/sneakpeek/static/docs/.doctrees/plugins/user_agent_injecter_plugin.doctree
+-rw-r--r--   0        0        0    13715 2023-04-23 21:12:02.386867 sneakpeek_py-0.1.5/sneakpeek/static/docs/.doctrees/quick_start.doctree
+-rw-r--r--   0        0        0      971 2023-04-23 21:11:03.986542 sneakpeek_py-0.1.5/sneakpeek/static/docs/_sources/api.rst.txt
+-rw-r--r--   0        0        0     1335 2023-04-23 21:11:03.986542 sneakpeek_py-0.1.5/sneakpeek/static/docs/_sources/deployment.rst.txt
+-rw-r--r--   0        0        0     5920 2023-04-23 21:11:03.986542 sneakpeek_py-0.1.5/sneakpeek/static/docs/_sources/design.rst.txt
+-rw-r--r--   0        0        0      477 2023-04-23 21:11:03.986542 sneakpeek_py-0.1.5/sneakpeek/static/docs/_sources/index.rst.txt
+-rw-r--r--   0        0        0      457 2023-04-23 21:11:03.986542 sneakpeek_py-0.1.5/sneakpeek/static/docs/_sources/plugins/index.rst.txt
+-rw-r--r--   0        0        0     4271 2023-04-23 21:11:03.986542 sneakpeek_py-0.1.5/sneakpeek/static/docs/_sources/plugins/new_plugin.rst.txt
+-rw-r--r--   0        0        0     1389 2023-04-23 21:11:03.986542 sneakpeek_py-0.1.5/sneakpeek/static/docs/_sources/plugins/proxy_plugin.rst.txt
+-rw-r--r--   0        0        0     2053 2023-04-23 21:11:03.986542 sneakpeek_py-0.1.5/sneakpeek/static/docs/_sources/plugins/rate_limiter_plugin.rst.txt
+-rw-r--r--   0        0        0     1338 2023-04-23 21:11:03.986542 sneakpeek_py-0.1.5/sneakpeek/static/docs/_sources/plugins/requests_logging_plugin.rst.txt
+-rw-r--r--   0        0        0     1367 2023-04-23 21:11:03.986542 sneakpeek_py-0.1.5/sneakpeek/static/docs/_sources/plugins/robots_txt_plugin.rst.txt
+-rw-r--r--   0        0        0     1507 2023-04-23 21:11:03.986542 sneakpeek_py-0.1.5/sneakpeek/static/docs/_sources/plugins/user_agent_injecter_plugin.rst.txt
+-rw-r--r--   0        0        0     5412 2023-04-23 21:11:03.986542 sneakpeek_py-0.1.5/sneakpeek/static/docs/_sources/quick_start.rst.txt
+-rw-r--r--   0        0        0    14638 2023-04-23 21:12:03.370871 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/basic.css
+-rw-r--r--   0        0        0     3275 2023-04-23 21:11:22.774668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/badge_only.css
+-rw-r--r--   0        0        0    87624 2023-04-23 21:11:22.774668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2023-04-23 21:11:22.774668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2023-04-23 21:11:22.774668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2023-04-23 21:11:22.778668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2023-04-23 21:11:22.778668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2023-04-23 21:11:22.782668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2023-04-23 21:11:22.786668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2023-04-23 21:11:22.786668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2023-04-23 21:11:22.786668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2023-04-23 21:11:22.790668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2023-04-23 21:11:22.790668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2023-04-23 21:11:22.794668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2023-04-23 21:11:22.798668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2023-04-23 21:11:22.798668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2023-04-23 21:11:22.802668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2023-04-23 21:11:22.802668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2023-04-23 21:11:22.806668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0   129674 2023-04-23 21:11:22.774668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/css/theme.css
+-rw-r--r--   0        0        0     9630 2023-04-23 21:11:22.258665 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/doctools.js
+-rw-r--r--   0        0        0      353 2023-04-23 21:12:03.370871 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2023-04-23 21:11:22.258665 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/file.png
+-rw-r--r--   0        0        0   287630 2023-04-23 21:11:22.262665 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/jquery-3.5.1.js
+-rw-r--r--   0        0        0    89476 2023-04-23 21:11:22.262665 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/jquery.js
+-rw-r--r--   0        0        0      934 2023-04-23 21:11:22.806668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2023-04-23 21:11:22.806668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2023-04-23 21:11:22.806668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2023-04-23 21:11:22.806668 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/js/theme.js
+-rw-r--r--   0        0        0    10854 2023-04-23 21:12:03.366871 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/language_data.js
+-rw-r--r--   0        0        0       90 2023-04-23 21:11:22.262665 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/minus.png
+-rw-r--r--   0        0        0       90 2023-04-23 21:11:22.262665 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/plus.png
+-rw-r--r--   0        0        0     4846 2023-04-23 21:12:03.362871 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/pygments.css
+-rw-r--r--   0        0        0    16733 2023-04-23 21:11:22.262665 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/searchtools.js
+-rw-r--r--   0        0        0    68420 2023-04-23 21:11:22.262665 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/underscore-1.13.1.js
+-rw-r--r--   0        0        0    19530 2023-04-23 21:11:22.266665 sneakpeek_py-0.1.5/sneakpeek/static/docs/_static/underscore.js
+-rw-r--r--   0        0        0   296498 2023-04-23 21:12:02.966869 sneakpeek_py-0.1.5/sneakpeek/static/docs/api.html
+-rw-r--r--   0        0        0     7429 2023-04-23 21:12:02.986869 sneakpeek_py-0.1.5/sneakpeek/static/docs/deployment.html
+-rw-r--r--   0        0        0    19360 2023-04-23 21:12:03.014869 sneakpeek_py-0.1.5/sneakpeek/static/docs/design.html
+-rw-r--r--   0        0        0    46781 2023-04-23 21:12:03.334871 sneakpeek_py-0.1.5/sneakpeek/static/docs/genindex.html
+-rw-r--r--   0        0        0     8498 2023-04-23 21:12:03.030869 sneakpeek_py-0.1.5/sneakpeek/static/docs/index.html
+-rw-r--r--   0        0        0     2035 2023-04-23 21:12:03.386871 sneakpeek_py-0.1.5/sneakpeek/static/docs/objects.inv
+-rw-r--r--   0        0        0     6989 2023-04-23 21:12:03.050869 sneakpeek_py-0.1.5/sneakpeek/static/docs/plugins/index.html
+-rw-r--r--   0        0        0    19629 2023-04-23 21:12:03.078869 sneakpeek_py-0.1.5/sneakpeek/static/docs/plugins/new_plugin.html
+-rw-r--r--   0        0        0     9726 2023-04-23 21:12:03.190870 sneakpeek_py-0.1.5/sneakpeek/static/docs/plugins/proxy_plugin.html
+-rw-r--r--   0        0        0    10251 2023-04-23 21:12:03.210870 sneakpeek_py-0.1.5/sneakpeek/static/docs/plugins/rate_limiter_plugin.html
+-rw-r--r--   0        0        0     9062 2023-04-23 21:12:03.230870 sneakpeek_py-0.1.5/sneakpeek/static/docs/plugins/requests_logging_plugin.html
+-rw-r--r--   0        0        0     9063 2023-04-23 21:12:03.250870 sneakpeek_py-0.1.5/sneakpeek/static/docs/plugins/robots_txt_plugin.html
+-rw-r--r--   0        0        0     9492 2023-04-23 21:12:03.270870 sneakpeek_py-0.1.5/sneakpeek/static/docs/plugins/user_agent_injecter_plugin.html
+-rw-r--r--   0        0        0    10148 2023-04-23 21:12:03.350871 sneakpeek_py-0.1.5/sneakpeek/static/docs/py-modindex.html
+-rw-r--r--   0        0        0    18514 2023-04-23 21:12:03.310871 sneakpeek_py-0.1.5/sneakpeek/static/docs/quick_start.html
+-rw-r--r--   0        0        0     5143 2023-04-23 21:12:03.362871 sneakpeek_py-0.1.5/sneakpeek/static/docs/search.html
+-rw-r--r--   0        0        0    19667 2023-04-23 21:12:03.382871 sneakpeek_py-0.1.5/sneakpeek/static/docs/searchindex.js
+-rw-r--r--   0        0        0    64483 2023-04-23 21:11:04.034543 sneakpeek_py-0.1.5/sneakpeek/static/favicon.ico
+-rw-r--r--   0        0        0     2359 2023-04-23 21:11:04.034543 sneakpeek_py-0.1.5/sneakpeek/static/icons/favicon.png
+-rw-r--r--   0        0        0      659 2023-04-23 21:11:04.034543 sneakpeek_py-0.1.5/sneakpeek/static/index.html
+-rw-r--r--   0        0        0      550 2023-04-23 21:11:55.894838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/ErrorNotFound.fa2e6ce5.js
+-rw-r--r--   0        0        0    20436 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/KFOkCnqEu92Fr1MmgVxIIzQ.34e9582c.woff
+-rw-r--r--   0        0        0    20544 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/KFOlCnqEu92Fr1MmEU9fBBc-.9ce7f3ac.woff
+-rw-r--r--   0        0        0    20416 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/KFOlCnqEu92Fr1MmSU5fBBc-.bf14c7d7.woff
+-rw-r--r--   0        0        0    20408 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/KFOlCnqEu92Fr1MmWUlfBBc-.e0fd57c0.woff
+-rw-r--r--   0        0        0    20424 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/KFOlCnqEu92Fr1MmYUtfBBc-.f6537e32.woff
+-rw-r--r--   0        0        0    20344 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/KFOmCnqEu92Fr1Mu4mxM.f2abf7fb.woff
+-rw-r--r--   0        0        0    24866 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/MainLayout.9793f7d2.js
+-rw-r--r--   0        0        0      538 2023-04-23 21:11:55.894838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/NewScraperPage.b1dbe3a9.js
+-rw-r--r--   0        0        0    30651 2023-04-23 21:11:55.894838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/PriorityChip.5a9183b4.js
+-rw-r--r--   0        0        0      655 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/QList.f8f850db.js
+-rw-r--r--   0        0        0    76403 2023-04-23 21:11:55.894838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/QPage.6b285e46.js
+-rw-r--r--   0        0        0     3323 2023-04-23 21:11:55.894838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/ScraperEditForm.640de0df.css
+-rw-r--r--   0        0        0  1333099 2023-04-23 21:11:55.894838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/ScraperEditForm.ca0cf7b2.js
+-rw-r--r--   0        0        0    26587 2023-04-23 21:11:55.894838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/ScraperPage.55442f56.js
+-rw-r--r--   0        0        0     2479 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/ScrapersPage.c93a5603.js
+-rw-r--r--   0        0        0    11097 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/api.94e9d625.js
+-rw-r--r--   0        0        0   187208 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/fa-brands-400.20c4a58b.ttf
+-rw-r--r--   0        0        0   108020 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/fa-brands-400.74833209.woff2
+-rw-r--r--   0        0        0    63952 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/fa-regular-400.528d022d.ttf
+-rw-r--r--   0        0        0    24948 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/fa-regular-400.8e7e5ea1.woff2
+-rw-r--r--   0        0        0   394628 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/fa-solid-900.67a65763.ttf
+-rw-r--r--   0        0        0   150124 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/fa-solid-900.7152a693.woff2
+-rw-r--r--   0        0        0    10172 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/fa-v4compatibility.0515a423.ttf
+-rw-r--r--   0        0        0     4564 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/fa-v4compatibility.694a17c3.woff2
+-rw-r--r--   0        0        0   164912 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.fd84f88b.woff
+-rw-r--r--   0        0        0   128616 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.4a4dbc62.woff2
+-rw-r--r--   0        0        0   132320 2023-04-23 21:11:55.890838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/index.7e99b1bd.js
+-rw-r--r--   0        0        0   307194 2023-04-23 21:11:55.894838 sneakpeek_py-0.1.5/sneakpeek/static/ui/assets/index.99b1d043.css
+-rw-r--r--   0        0        0     2359 2023-04-23 21:11:54.922833 sneakpeek_py-0.1.5/sneakpeek/static/ui/icons/favicon.png
+-rw-r--r--   0        0        0      659 2023-04-23 21:11:55.894838 sneakpeek_py-0.1.5/sneakpeek/static/ui/index.html
+-rw-r--r--   0        0        0     4174 2023-04-23 21:11:04.054543 sneakpeek_py-0.1.5/sneakpeek/worker.py
+-rw-r--r--   0        0        0     7515 1970-01-01 00:00:00.000000 sneakpeek_py-0.1.5/PKG-INFO
```

### Comparing `sneakpeek_py-0.1.4/pyproject.toml` & `sneakpeek_py-0.1.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "sneakpeek-py"
 packages = [{ include = "sneakpeek" }]
-version = "0.1.4"
-description = "Tool box for creating scrapers, so that you only focus on scraping logic"
+version = "0.1.5"
+description = "Sneakpeek is a framework that helps to quickly and conviniently develop scrapers. It's the best choice for scrapers that have some specific complex scraping logic that needs to be run on a constant basis."
 authors = ["Dan Yazovsky <daniil.yazovsky@gmail.com>"]
 maintainers = ["Dan Yazovsky <daniil.yazovsky@gmail.com>"]
 repository = "https://github.com/flulemon/sneakpeek"
-documentation = "https://github.com/flulemon/sneakpeek"
+documentation = "https://sneakpeek-py.readthedocs.io/en/latest/"
 homepage = "https://github.com/flulemon/sneakpeek"
 license = "BSD-3-Clause"
 readme = "README.md"
 classifiers = [
     "Operating System :: OS Independent",
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: BSD License",
@@ -33,14 +33,18 @@
 redis = "^4.5.4"
 apscheduler = "^3.10.1"
 aiohttp = "^3.8.4"
 uvicorn = "^0.21.1"
 cachetools = "^5.3.0"
 prometheus-client = "^0.16.0"
 fake-useragent = "^1.1.3"
+Sphinx = { version = "4.2.0", optional = true }
+sphinx-rtd-theme = { version = "1.0.0", optional = true }
+sphinxcontrib-napoleon = { version = "0.7", optional = true }
+yarl = "^1.9.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 fakeredis = "^2.10.3"
 black = "^23.3.0"
 pytest-lazy-fixture = "^0.6.3"
 pytest-asyncio = "^0.21.0"
@@ -49,8 +53,11 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
-log_cli_date_format = "%Y-%m-%d %H:%M:%S"
+log_cli_date_format = "%Y-%m-%d %H:%M:%S"
+
+[tool.poetry.extras]
+docs = ["Sphinx", "sphinx-rtd-theme", "sphinxcontrib-napoleon"]
```

### Comparing `sneakpeek_py-0.1.4/sneakpeek/lib/errors.py` & `sneakpeek_py-0.1.5/sneakpeek/lib/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 
 class ScraperNotFoundError(jsonrpc.BaseError):
     CODE = 5000
     MESSAGE = "Scraper not found"
 
 
-class ScraperRunNotFoundError(jsonrpc.BaseError):
+class ScraperJobNotFoundError(jsonrpc.BaseError):
     CODE = 5001
-    MESSAGE = "Scraper run not found"
+    MESSAGE = "Scraper job not found"
 
 
 class ScraperHasActiveRunError(jsonrpc.BaseError):
     CODE = 10000
-    MESSAGE = "Scraper has active runs"
+    MESSAGE = "Scraper has active jobs"
 
 
-class ScraperRunPingNotStartedError(jsonrpc.BaseError):
+class ScraperJobPingNotStartedError(jsonrpc.BaseError):
     CODE = 10001
-    MESSAGE = "Failed to ping not started scraper run"
+    MESSAGE = "Failed to ping not started scraper job"
 
 
-class ScraperRunPingFinishedError(jsonrpc.BaseError):
+class ScraperJobPingFinishedError(jsonrpc.BaseError):
     CODE = 10002
-    MESSAGE = "Tried to ping finished scraper run"
+    MESSAGE = "Tried to ping finished scraper job"
 
 
 class UnknownScraperHandlerError(jsonrpc.BaseError):
     CODE = 10002
-    MESSAGE = "Tried to ping finished scraper run"
+    MESSAGE = "Unknown scraper handler"
```

### Comparing `sneakpeek_py-0.1.4/sneakpeek/lib/storage/in_memory_storage.py` & `sneakpeek_py-0.1.5/sneakpeek/lib/storage/in_memory_storage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 import logging
 from asyncio import Lock
 from datetime import datetime, timedelta
 from itertools import count
 from typing import Iterator
 
-from sneakpeek.lib.errors import ScraperNotFoundError, ScraperRunNotFoundError
-from sneakpeek.lib.models import Lease, Scraper, ScraperRun, ScraperRunPriority
+from sneakpeek.lib.errors import ScraperJobNotFoundError, ScraperNotFoundError
+from sneakpeek.lib.models import Lease, Scraper, ScraperJob, ScraperJobPriority
 from sneakpeek.metrics import count_invocations, measure_latency
 
-from .base import Storage
+from .base import LeaseStorage, ScraperJobsStorage, ScrapersStorage
 
 
-class InMemoryStorage(Storage):
+class InMemoryScrapersStorage(ScrapersStorage):
+    """In-memory storage implementation"""
+
     def __init__(
         self,
         scrapers: list[Scraper] | None = None,
-        is_read_only: bool = False,
+        is_read_only: bool = True,
     ) -> None:
+        """
+        Args:
+            scrapers (list[Scraper] | None, optional): List of pre-defined scrapers. Defaults to None.
+            is_read_only (bool, optional): Whether to allow modifications of the scrapers list. Set to true only for development. Defaults to True.
+        """
         self._logger = logging.getLogger(__name__)
         self._scrapers: dict[int, Scraper] = {
             scraper.id: scraper for scraper in scrapers or []
         }
-        self._scraper_runs: dict[int, dict[int, ScraperRun]] = {}
-        self._queues: dict[ScraperRunPriority, list[ScraperRun]] = {}
         self._id_generator: Iterator[int] = count(1)
         self._lock = Lock()
-        self._leases: dict[str, Lease] = {}
         self._is_read_only = is_read_only
 
     def _generate_id(self) -> int:
         for id in self._id_generator:
-            if id not in self._scrapers and id not in self._scraper_runs:
+            if id not in self._scrapers:
                 return id
 
     @count_invocations(subsystem="storage")
     @measure_latency(subsystem="storage")
+    async def is_read_only(self) -> bool:
+        return self._is_read_only
+
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def search_scrapers(
         self,
         name_filter: str | None = None,
         max_items: int | None = None,
         offset: int | None = None,
     ) -> list[Scraper]:
         offset = offset or 0
@@ -100,114 +109,133 @@
         async with self._lock:
             if id not in self._scrapers:
                 raise ScraperNotFoundError(id)
             scraper_to_delete = self._scrapers[id]
             del self._scrapers[id]
             return scraper_to_delete
 
+
+class InMemoryScraperJobsStorage(ScraperJobsStorage):
+    """In memory storage for scraper jobs. Should only be used for development purposes"""
+
+    def __init__(self) -> None:
+        self._logger = logging.getLogger(__name__)
+        self._scraper_jobs: dict[int, dict[int, ScraperJob]] = {}
+        self._queues: dict[ScraperJobPriority, list[ScraperJob]] = {}
+        self._id_generator: Iterator[int] = count(1)
+        self._lock = Lock()
+
+    def _generate_id(self) -> int:
+        for id in self._id_generator:
+            for scraper_id, scraper_jobs in self._scraper_jobs.items():
+                if id == scraper_id or id in scraper_jobs:
+                    continue
+            return id
+
     @count_invocations(subsystem="storage")
     @measure_latency(subsystem="storage")
-    async def get_scraper_runs(self, id: int) -> list[ScraperRun]:
+    async def get_scraper_jobs(self, id: int) -> list[ScraperJob]:
         async with self._lock:
-            if id not in self._scrapers:
-                raise ScraperNotFoundError(id)
             return list(
                 sorted(
-                    self._scraper_runs.get(id, {}).values(),
+                    self._scraper_jobs.get(id, {}).values(),
                     key=lambda x: x.id,
                     reverse=True,
                 )
             )
 
     @count_invocations(subsystem="storage")
     @measure_latency(subsystem="storage")
-    async def add_scraper_run(self, scraper_run: ScraperRun) -> ScraperRun:
+    async def add_scraper_job(self, scraper_job: ScraperJob) -> ScraperJob:
         async with self._lock:
-            scraper_run.id = (
-                scraper_run.id
-                if scraper_run.id and scraper_run.id > 0
+            scraper_job.id = (
+                scraper_job.id
+                if scraper_job.id and scraper_job.id > 0
                 else self._generate_id()
             )
-            if scraper_run.scraper.id not in self._scrapers:
-                raise ScraperRunNotFoundError(scraper_run.scraper.id)
 
-            if scraper_run.scraper.id not in self._scraper_runs:
-                self._scraper_runs[scraper_run.scraper.id] = {}
+            if scraper_job.scraper.id not in self._scraper_jobs:
+                self._scraper_jobs[scraper_job.scraper.id] = {}
 
-            if scraper_run.id in self._scraper_runs[scraper_run.scraper.id]:
+            if scraper_job.id in self._scraper_jobs[scraper_job.scraper.id]:
                 self._logger.warning(
-                    f"Will rewrite existing scraper run: {self._scraper_runs[scraper_run.scraper.id][scraper_run.id]} with {scraper_run}"
+                    f"Will rewrite existing scraper run: {self._scraper_jobs[scraper_job.scraper.id][scraper_job.id]} with {scraper_job}"
                 )
 
-            self._scraper_runs[scraper_run.scraper.id][scraper_run.id] = scraper_run
-            if scraper_run.priority not in self._queues:
-                self._queues[scraper_run.priority] = []
-            self._queues[scraper_run.priority].append(scraper_run)
-            return scraper_run
+            self._scraper_jobs[scraper_job.scraper.id][scraper_job.id] = scraper_job
+            if scraper_job.priority not in self._queues:
+                self._queues[scraper_job.priority] = []
+            self._queues[scraper_job.priority].append(scraper_job)
+            return scraper_job
 
     @count_invocations(subsystem="storage")
     @measure_latency(subsystem="storage")
-    async def update_scraper_run(self, scraper_run: ScraperRun) -> ScraperRun:
+    async def update_scraper_job(self, scraper_job: ScraperJob) -> ScraperJob:
         async with self._lock:
-            if scraper_run.scraper.id not in self._scrapers:
-                raise ScraperNotFoundError(scraper_run.scraper.id)
             if (
-                not self._scraper_runs.get(scraper_run.scraper.id)
-                or scraper_run.id not in self._scraper_runs[scraper_run.scraper.id]
+                not self._scraper_jobs.get(scraper_job.scraper.id)
+                or scraper_job.id not in self._scraper_jobs[scraper_job.scraper.id]
             ):
-                raise ScraperRunNotFoundError(scraper_run.id)
+                raise ScraperJobNotFoundError(scraper_job.id)
 
-            self._scraper_runs[scraper_run.scraper.id][scraper_run.id] = scraper_run
-            return scraper_run
+            self._scraper_jobs[scraper_job.scraper.id][scraper_job.id] = scraper_job
+            return scraper_job
 
     @count_invocations(subsystem="storage")
     @measure_latency(subsystem="storage")
-    async def get_scraper_run(self, scraper_id: int, scraper_run_id: int) -> ScraperRun:
+    async def get_scraper_job(self, scraper_id: int, scraper_job_id: int) -> ScraperJob:
         async with self._lock:
-            if scraper_id not in self._scrapers:
-                raise ScraperNotFoundError(scraper_id)
             if (
-                not self._scraper_runs.get(scraper_id)
-                or scraper_run_id not in self._scraper_runs[scraper_id]
+                not self._scraper_jobs.get(scraper_id)
+                or scraper_job_id not in self._scraper_jobs[scraper_id]
             ):
-                raise ScraperRunNotFoundError(scraper_run_id)
-            return self._scraper_runs[scraper_id][scraper_run_id]
+                raise ScraperJobNotFoundError(scraper_job_id)
+            return self._scraper_jobs[scraper_id][scraper_job_id]
 
     @count_invocations(subsystem="storage")
     @measure_latency(subsystem="storage")
-    async def dequeue_scraper_run(
+    async def dequeue_scraper_job(
         self,
-        priority: ScraperRunPriority,
-    ) -> ScraperRun | None:
+        priority: ScraperJobPriority,
+    ) -> ScraperJob | None:
         async with self._lock:
             if not self._queues.get(priority):
                 return None
             return self._queues[priority].pop(0)
 
     @count_invocations(subsystem="storage")
     @measure_latency(subsystem="storage")
-    async def get_queue_len(self, priority: ScraperRunPriority) -> int:
+    async def get_queue_len(self, priority: ScraperJobPriority) -> int:
         return len(self._queues.get(priority) or [])
 
     @count_invocations(subsystem="storage")
     @measure_latency(subsystem="storage")
-    async def delete_old_scraper_runs(self, keep_last: int = 50) -> None:
+    async def delete_old_scraper_jobs(self, keep_last: int = 50) -> None:
         async with self._lock:
-            self._scraper_runs = {
+            self._scraper_jobs = {
                 scraper_id: {
-                    scraper_run.id: scraper_run
-                    for scraper_run in sorted(
-                        scraper_runs.values(),
+                    scraper_job.id: scraper_job
+                    for scraper_job in sorted(
+                        scraper_jobs.values(),
                         key=lambda item: item.id,
                         reverse=True,
                     )[:keep_last]
                 }
-                for scraper_id, scraper_runs in self._scraper_runs.items()
+                for scraper_id, scraper_jobs in self._scraper_jobs.items()
             }
 
+
+class InMemoryLeaseStorage(LeaseStorage):
+    """In memory storage for leases. Should only be used for development purposes"""
+
+    def __init__(self) -> None:
+        self._logger = logging.getLogger(__name__)
+        self._lock = Lock()
+        self._leases: dict[str, Lease] = {}
+
     def _can_acquire_lease(self, lease_name: str, owner_id: str) -> bool:
         existing_lease = self._leases.get(lease_name)
         return (
             not existing_lease
             or existing_lease.acquired_until < datetime.utcnow()
             or existing_lease.owner_id == owner_id
         )
@@ -235,12 +263,7 @@
     @measure_latency(subsystem="storage")
     async def release_lease(self, lease_name: str, owner_id: str) -> None:
         async with self._lock:
             if lease_name not in self._leases:
                 return
             if self._can_acquire_lease(lease_name, owner_id):
                 del self._leases[lease_name]
-
-    @count_invocations(subsystem="storage")
-    @measure_latency(subsystem="storage")
-    async def is_read_only(self) -> bool:
-        return self._is_read_only
```

### Comparing `sneakpeek_py-0.1.4/sneakpeek/metrics.py` & `sneakpeek_py-0.1.5/sneakpeek/metrics.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,14 +26,35 @@
     documentation="Number of active subsytem replicas",
     namespace="sneakpeek",
     labelnames=["type"],
 )
 
 
 def measure_latency(subsystem: str):
+    """
+    Decorator for measuring latency of the function (works for both sync and async functions).
+
+    .. code-block:: python3
+
+        @measure_latency(subsytem="my subsystem")
+        def my_awesome_func():
+            ...
+
+
+    This will export following Prometheus histogram metric:
+
+
+    .. code-block::
+
+        sneakpeek_latency{subsystem="my subsystem", method="my_awesome_func"}
+
+    Args:
+        subsystem (str): Subsystem name to be used in the metric annotation
+    """
+
     def wrapper(func):
         @wraps(func)
         def sync_wrapper(*args, **kwargs):
             with latency_histogram.labels(
                 subsystem=subsystem, method=func.__name__
             ).time():
                 return func(*args, **kwargs)
@@ -47,14 +68,40 @@
 
         return async_wrapper if asyncio.iscoroutinefunction(func) else sync_wrapper
 
     return wrapper
 
 
 def count_invocations(subsystem: str):
+    """
+    Decorator for measuring number of function invocations (works for both sync and async functions).
+
+    .. code-block:: python3
+
+        @count_invocations(subsytem="my subsystem")
+        def my_awesome_func():
+            ...
+
+
+    This will export following Prometheus counter metrics:
+
+
+    .. code-block::
+
+        # Total number of invocations
+        sneakpeek_invocations{subsystem="my subsystem", method="my_awesome_func", type="total", error=""}
+        # Total number of successful invocations (ones that haven't thrown an exception)
+        sneakpeek_invocations{subsystem="my subsystem", method="my_awesome_func", type="success", error=""}
+        # Total number of failed invocations (ones that have thrown an exception)
+        sneakpeek_invocations{subsystem="my subsystem", method="my_awesome_func", type="error", error="<Exception class name>"}
+
+    Args:
+        subsystem (str): Subsystem name to be used in the metric annotation
+    """
+
     def wrapper(func):
         @wraps(func)
         def sync_wrapper(*args, **kwargs):
             invocations_counter.labels(
                 subsystem=subsystem,
                 method=func.__name__,
                 type="total",
```

### Comparing `sneakpeek_py-0.1.4/sneakpeek/plugins/rate_limiter_plugin.py` & `sneakpeek_py-0.1.5/sneakpeek/plugins/robots_txt_plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,137 +1,118 @@
-import asyncio
 import logging
-from asyncio import Lock
-from datetime import datetime, timedelta
+import sys
+from datetime import timedelta
 from enum import Enum, auto
-from random import randint
+from traceback import format_exc
 from typing import Any
 from urllib.parse import urlparse
+from urllib.robotparser import RobotFileParser
 
-from cachetools.func import ttl_cache
-from pydantic import BaseModel, validator
+import aiohttp
+from cachetools import TTLCache
+from pydantic import BaseModel
 
 from sneakpeek.plugins.utils import parse_config_from_obj
 from sneakpeek.scraper_context import BeforeRequestPlugin, Request
 
-DEFAULT_BUCKET_TIME_WINDOW = timedelta(minutes=1)
 
+class RobotsTxtViolationException(Exception):
+    """Exception which is raised if request is disallowed by website robots.txt"""
 
-def rate_limited_delay_jitter() -> timedelta:
-    return timedelta(milliseconds=randint(0, 500))
+    pass
 
 
-class _LeakyBucket:
-    def __init__(
-        self, size: int, time_window: timedelta = DEFAULT_BUCKET_TIME_WINDOW
-    ) -> None:
-        self.size = size
-        self.time_window = time_window
-        self.queue: list[datetime] = []
-        self.lock = Lock()
-
-    def last_used(self) -> datetime | None:
-        if not self.queue:
-            return None
-        return self.queue[0]
-
-    async def add(self) -> datetime | None:
-        async with self.lock:
-            now = datetime.utcnow()
-            while self.queue and self.queue[0] <= now - self.time_window:
-                self.queue.pop(0)
-            if not self.size:
-                raise ValueError("Queue size is 0")
-            if len(self.queue) >= self.size:
-                return self.queue[0] + self.time_window
+class RobotsTxtViolationStrategy(Enum):
+    """What to do if the request is disallowed by website robots.txt"""
 
-            self.queue.append(now)
-            return None
+    LOG = auto()  #: Only log violation
+    THROW = auto()  #: Raise an exception on vioalation
 
 
-class RateLimitedException(Exception):
-    pass
+class RobotsTxtPluginConfig(BaseModel):
+    """robots.txt plugin configuration"""
 
+    violation_strategy: RobotsTxtViolationStrategy = RobotsTxtViolationStrategy.LOG
 
-class RateLimitedStrategy(Enum):
-    THROW = auto()
-    WAIT = auto()
-
-
-class RateLimiterPluginConfig(BaseModel):
-    max_rpm: int = 60
-    rate_limited_strategy: RateLimitedStrategy = RateLimitedStrategy.WAIT
-    time_window: timedelta = DEFAULT_BUCKET_TIME_WINDOW
-
-    @validator("max_rpm")
-    def check_max_rpm(cls, v: int) -> int:
-        if v <= 0:
-            raise ValueError(f"`max_rpm` must be a positive integer. Received: {v}")
-        return v
-
-    def __hash__(self):
-        return hash(
-            (
-                self.max_rpm,
-                self.rate_limited_strategy,
-                self.time_window,
-            )
-        )
 
+class RobotsTxtPlugin(BeforeRequestPlugin):
+    """Robots.txt plugin can log and optionally block requests if they are disallowed by website robots.txt."""
 
-class RateLimiterPlugin(BeforeRequestPlugin):
-    def __init__(self, default_config: RateLimiterPluginConfig | None = None) -> None:
-        self._default_config = default_config or RateLimiterPluginConfig()
+    def __init__(self, default_config: RobotsTxtPluginConfig | None = None) -> None:
+        self._default_config = default_config or RobotsTxtPluginConfig()
         self._logger = logging.getLogger(__name__)
+        self._cache = TTLCache(
+            maxsize=sys.maxsize,
+            ttl=timedelta(hours=1).total_seconds(),
+        )
 
     @property
     def name(self) -> str:
-        return "rate_limiter"
-
-    def _extract_key(self, url: str) -> str:
-        return urlparse(url).hostname
-
-    @ttl_cache(maxsize=None, ttl=timedelta(minutes=5).total_seconds())
-    def _get_bucket(self, key: str, config: RateLimiterPluginConfig) -> _LeakyBucket:
-        return _LeakyBucket(
-            size=config.max_rpm,
-            time_window=config.time_window,
-        )
+        return "robots_txt"
 
-    async def _wait_for_admission(
-        self,
-        url: str,
-        config: RateLimiterPluginConfig,
-    ) -> None:
-        key = self._extract_key(url)
-        bucket = self._get_bucket(key, config)
-        while True:
-            next_attempt_dt = await bucket.add()
-            if not next_attempt_dt:
-                return
-            error_message = (
-                f"Rate limited request to '{url}' because there were "
-                f"more than {bucket.size} calls in the last {int(bucket.time_window.total_seconds())}s "
-                f"to the domain {key}. "
-                f"Next available call will be permitted at {next_attempt_dt}."
-            )
+    def _extract_host(self, url: str) -> str:
+        return urlparse(url).hostname.replace("www.", "")
 
-            if config.rate_limited_strategy == RateLimitedStrategy.THROW:
-                raise RateLimitedException(error_message)
-            self._logger.info(error_message)
-            attempt_delay = next_attempt_dt - datetime.utcnow()
-            attempt_delay += rate_limited_delay_jitter()
-            await asyncio.sleep(attempt_delay.total_seconds())
+    async def _get_robots_txt_by_url(self, url: str) -> RobotFileParser | None:
+        async with aiohttp.ClientSession() as session:
+            response = await session.get(url)
+            if response.status != 200:
+                return None
+            contents = await response.text()
+            rfp = RobotFileParser()
+            rfp.parse(contents.split("\n"))
+            return rfp
+
+    async def _load_robots_txt(self, host: str) -> RobotFileParser | None:
+        if cached := self._cache.get(host):
+            return cached
+        for scheme in ["http", "https"]:
+            for host_prefix in ["", "www."]:
+                try:
+                    robots_txt = await self._get_robots_txt_by_url(
+                        f"{scheme}://{host_prefix}{host}/robots.txt"
+                    )
+                    self._cache[host] = robots_txt
+                    if robots_txt:
+                        return robots_txt
+                except Exception as e:
+                    self._logger.error(f"Failed to get robots.txt for {host}: {e}")
+                    self._logger.debug(
+                        f"Failed to get robots.txt for {host}. Traceback: {format_exc()}"
+                    )
+        return None
 
     async def before_request(
         self,
         request: Request,
         config: Any | None,
     ) -> Request:
         config = parse_config_from_obj(
             config,
             self.name,
-            RateLimiterPluginConfig,
+            RobotsTxtPluginConfig,
             self._default_config,
         )
-        await self._wait_for_admission(request.url, config)
+        host = self._extract_host(request.url)
+        robots_txt = await self._load_robots_txt(host)
+        if not robots_txt:
+            self._logger.debug(
+                f"No robots.txt was retrieved for {request.url}. Defaulting to allow"
+            )
+            return request
+
+        user_agent = (request.headers or {}).get("User-Agent")
+        if not user_agent:
+            self._logger.debug(
+                f"User-Agent is empty while requesting {request.url}. Defaulting to '*'"
+            )
+            user_agent = "*"
+
+        if not robots_txt.can_fetch(user_agent, request.url):
+            error_message = f"robots.txt prohibits requesting {request.url}"
+            if config.violation_strategy == RobotsTxtViolationStrategy.THROW:
+                raise RobotsTxtViolationException(error_message)
+            self._logger.error(
+                f"{error_message}. Proceeding because strategy is {config.violation_strategy}"
+            )
+
         return request
```

### Comparing `sneakpeek_py-0.1.4/sneakpeek/plugins/requests_logging_plugin.py` & `sneakpeek_py-0.1.5/sneakpeek/plugins/requests_logging_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,19 +5,23 @@
 from pydantic import BaseModel
 
 from sneakpeek.plugins.utils import parse_config_from_obj
 from sneakpeek.scraper_context import AfterResponsePlugin, BeforeRequestPlugin, Request
 
 
 class RequestsLoggingPluginConfig(BaseModel):
-    log_request: bool = True
-    log_response: bool = True
+    """Requests logging plugin config"""
+
+    log_request: bool = True  #: Whether to log request being made
+    log_response: bool = True  #: Whether to log response being made
 
 
 class RequestsLoggingPlugin(BeforeRequestPlugin, AfterResponsePlugin):
+    """Requests logging middleware logs all requests being made and received responses."""
+
     def __init__(
         self, default_config: RequestsLoggingPluginConfig | None = None
     ) -> None:
         self._default_config = default_config or RequestsLoggingPluginConfig()
         self._logger = logging.getLogger(__name__)
 
     @property
```

### Comparing `sneakpeek_py-0.1.4/sneakpeek/plugins/user_agent_injecter_plugin.py` & `sneakpeek_py-0.1.5/sneakpeek/plugins/proxy_plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 from typing import Any
 
+from aiohttp import BasicAuth
 from fake_useragent import UserAgent
 from pydantic import BaseModel
+from yarl import URL
 
 from sneakpeek.plugins.utils import parse_config_from_obj
 from sneakpeek.scraper_context import BeforeRequestPlugin, Request
 
 
-class UserAgentInjecterPluginConfig(BaseModel):
-    use_external_data: bool = True
-    browsers: list[str] = ["chrome", "edge", "firefox", "safari", "opera"]
+class ProxyPluginConfig(BaseModel):
+    """Proxy plugin config"""
 
+    proxy: str | URL | None = None  #: Proxy URL
+    proxy_auth: BasicAuth | None = None  #: Proxy authentication info to use
 
-class UserAgentInjecterPlugin(BeforeRequestPlugin):
-    def __init__(
-        self, default_config: UserAgentInjecterPluginConfig | None = None
-    ) -> None:
-        self._default_config = default_config or UserAgentInjecterPluginConfig()
+    class Config:
+        arbitrary_types_allowed = True
+
+
+class ProxyPlugin(BeforeRequestPlugin):
+    """Proxy plugin automatically sets proxy arguments for all HTTP requests."""
+
+    def __init__(self, default_config: ProxyPluginConfig | None = None) -> None:
+        self._default_config = default_config or ProxyPluginConfig()
         self._user_agents = UserAgent(
             use_external_data=self._default_config.use_external_data,
             browsers=self._default_config.browsers,
         )
 
     @property
     def name(self) -> str:
-        return "user_agent_injecter"
+        return "proxy"
 
     async def before_request(
         self,
         request: Request,
         config: Any | None,
     ) -> Request:
         config = parse_config_from_obj(
             config,
             self.name,
-            UserAgentInjecterPluginConfig,
+            ProxyPluginConfig,
             self._default_config,
         )
-        if (request.headers or {}).get("User-Agent"):
-            return request
-        if not request.headers:
-            request.headers = {}
-        request.headers["User-Agent"] = self._user_agents.random
+        if not request.kwargs:
+            request.kwargs = {}
+        if config.proxy:
+            request.kwargs["proxy"] = config.proxy
+        if config.proxy_auth:
+            request.kwargs["proxy_auth"] = config.proxy_auth
         return request
```

### Comparing `sneakpeek_py-0.1.4/sneakpeek/plugins/utils.py` & `sneakpeek_py-0.1.5/sneakpeek/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/scheduler.py` & `sneakpeek_py-0.1.5/sneakpeek/scheduler.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
 from apscheduler.triggers.base import BaseTrigger
 from apscheduler.triggers.cron import CronTrigger
 from apscheduler.triggers.interval import IntervalTrigger
 from prometheus_client import Gauge
 
 from sneakpeek.lib.errors import ScraperHasActiveRunError
-from sneakpeek.lib.models import Lease, Scraper, ScraperRunPriority, ScraperSchedule
+from sneakpeek.lib.models import Lease, Scraper, ScraperJobPriority, ScraperSchedule
 from sneakpeek.lib.queue import QueueABC
-from sneakpeek.lib.storage.base import Storage
+from sneakpeek.lib.storage.base import LeaseStorage, ScraperJobsStorage, ScrapersStorage
 from sneakpeek.metrics import count_invocations, measure_latency, replicas_gauge
 
 DEFAULT_LEASE_DURATION = timedelta(minutes=1)
 DEFAULT_STORAGE_POLL_DELAY = timedelta(seconds=5)
 DEFAULT_RUNS_TO_KEEP = 100
 
 
 queue_length_gauge = Gauge(
     name="queue_length",
-    documentation="Number of pending scraper runs",
+    documentation="Number of pending scraper jobs",
     namespace="sneakpeek",
     labelnames=["priority"],
 )
 
 
 class SchedulerABC(ABC):
     @abstractmethod
@@ -39,99 +39,124 @@
 
     @abstractmethod
     async def stop(self) -> None:
         ...
 
 
 class Scheduler(SchedulerABC):
+    """Sneakpeeker scheduler - schedules scrapers and performs maintenance jobs. Uses APScheduler under the hood."""
+
     def __init__(
         self,
-        storage: Storage,
+        scrapers_storage: ScrapersStorage,
+        jobs_storage: ScraperJobsStorage,
+        lease_storage: LeaseStorage,
         queue: QueueABC,
         storage_poll_frequency: timedelta = DEFAULT_STORAGE_POLL_DELAY,
         lease_duration: timedelta = DEFAULT_LEASE_DURATION,
-        runs_to_keep: int = 3,
+        jobs_to_keep: int = 100,
     ) -> None:
+        """Initialize scheduler
+
+        Args:
+            scrapers_storage (ScrapersStorage): Scrapers storage
+            jobs_storage (ScraperJobsStorage): Jobs storage
+            lease_storage (LeaseStorage): Lease storage
+            queue (Queue): Sneakpeek queue implementation
+            storage_poll_frequency (timedelta, optional): How much scheduler wait before polling storage for scrapers updates. Defaults to 5 seconds.
+            lease_duration (timedelta, optional): How long scheduler lease lasts. Lease is required for scheduler to be able to create new scraper jobs. This is needed so at any point of time there's only one active scheduler instance. Defaults to 1 minute.
+            jobs_to_keep (int, optional): Maximum number of historical scraper jobs to keep in the storage. Storage is cleaned up every 10 minutes. Defaults to 100.
+        """
         self._lease_name = "sneakpeek:scheduler"
         self._owner_id = str(uuid4())
         self._lease_duration = lease_duration
-        self._storage = storage
+        self._scrapers_storage = scrapers_storage
+        self._jobs_storage = jobs_storage
+        self._lease_storage = lease_storage
         self._queue = queue
         self._scheduler = AsyncIOScheduler()
         self._lease: Lease | None = None
         self._lock = Lock()
         self._scrapers: Dict[int, Scraper] = {}
         self._logger = logging.getLogger(__name__)
         self._scheduler.add_job(
             self._on_tick,
             trigger="interval",
             seconds=int(storage_poll_frequency.total_seconds()),
             id="scheduler:internal:on_tick",
             max_instances=1,
         )
-        self._max_kill_dead_runs_concurrency = 10
+        self._max_kill_dead_jobs_concurrency = 10
         self._scheduler.add_job(
-            self._kill_dead_scraper_runs,
+            self._kill_dead_scraper_jobs,
             trigger="interval",
             seconds=int(timedelta(minutes=1).total_seconds()),
-            id="scheduler:internal:kill_dead_runs",
+            id="scheduler:internal:kill_dead_jobs",
             max_instances=1,
         )
         self._scheduler.add_job(
             self._export_queue_len,
             trigger="interval",
             seconds=int(timedelta(seconds=5).total_seconds()),
             id="scheduler:internal:export_queue_len",
             max_instances=1,
         )
-        self._runs_to_keep = runs_to_keep
+        self._jobs_to_keep = jobs_to_keep
         self._scheduler.add_job(
-            self._delete_old_scraper_runs,
+            self._delete_old_scraper_jobs,
             trigger="interval",
             seconds=int(timedelta(minutes=10).total_seconds()),
-            id="scheduler:internal:delete_old_runs",
+            id="scheduler:internal:delete_old_jobs",
             max_instances=1,
         )
 
+    @property
+    def _is_lease_acquired(self) -> bool:
+        return (
+            self._lease
+            and self._lease.acquired
+            and datetime.utcnow() < self._lease.acquired_until
+        )
+
     @measure_latency(subsystem="scheduler")
     @count_invocations(subsystem="scheduler")
     async def _enqueue_scraper(self, scraper_id: int) -> None:
+        if not self._is_lease_acquired:
+            self._logger.debug(
+                f"Couldn't enqueue scraper id={scraper_id} because lease is not acquired"
+            )
+            return
         scraper = self._scrapers.get(scraper_id)
         if not scraper:
             self._logger.warning(f"Tried to enqueue unknown scraper: {scraper_id}")
             return
 
         scraper_human_id = f"'{scraper.name}'::{scraper.id}"
         self._logger.debug(f"Trying to enqueue scraper {scraper_human_id}")
-        if not self._lease:
-            self._logger.debug(
-                f"Couldn't enqueue scraper {scraper_human_id} because lease is not acquired"
-            )
-            return
         try:
-            scraper_run = await self._queue.enqueue(
+            scraper_job = await self._queue.enqueue(
                 scraper.id,
                 scraper.schedule_priority,
             )
             self._logger.info(
-                f"Successfully enqueued scraper {scraper_human_id}::{scraper_run.id}"
+                f"Successfully enqueued scraper {scraper_human_id}::{scraper_job.id}"
             )
         except ScraperHasActiveRunError as e:
             self._logger.debug(f"Failed to enqueue {scraper_human_id}: {e}")
         except Exception as e:
             self._logger.error(f"Failed to enqueue {scraper_human_id}: {e}")
             self._logger.debug(
                 f"Failed to enqueue {scraper_human_id}. Traceback: {format_exc()}"
             )
 
     async def _get_scraper_trigger(self, scraper: Scraper) -> BaseTrigger:
         start_date = datetime.min
-        scraper_runs = await self._storage.get_scraper_runs(scraper.id)
-        if scraper_runs:
-            last_run = sorted(scraper_runs, key=lambda x: x.id, reverse=True)[0]
+        scraper_jobs = await self._jobs_storage.get_scraper_jobs(scraper.id)
+        if scraper_jobs:
+            last_run = sorted(scraper_jobs, key=lambda x: x.id, reverse=True)[0]
             start_date = last_run.finished_at
         match scraper.schedule:
             case ScraperSchedule.CRONTAB:
                 return CronTrigger.from_crontab(scraper.schedule_crontab)
             case ScraperSchedule.EVERY_HOUR:
                 return IntervalTrigger(hours=1, start_date=start_date)
             case ScraperSchedule.EVERY_DAY:
@@ -151,14 +176,20 @@
         del self._scrapers[scraper.id]
 
     @measure_latency(subsystem="scheduler")
     @count_invocations(subsystem="scheduler")
     async def _update_scraper_job(
         self, scraper: Scraper, remove_existing: bool
     ) -> None:
+        """Add or update internal scheduler job for the scraper.
+
+        Args:
+            scraper (Scraper): Scraper metadata
+            remove_existing (bool): If True will remove internal scheduler job before adding a new one.
+        """
         logging.info(
             f"{'Updating' if remove_existing else 'Adding'} scraper enqueue job: '{scraper.name}'::{scraper.id}"
         )
         job_id = f"scheduler:scraper:{scraper.id}"
         trigger = await self._get_scraper_trigger(scraper)
         self._scrapers[scraper.id] = scraper
         if remove_existing:
@@ -169,34 +200,40 @@
             id=job_id,
             args=(scraper.id,),
         )
 
     @measure_latency(subsystem="scheduler")
     @count_invocations(subsystem="scheduler")
     async def _update_scrapers_jobs(self) -> None:
-        scrapers = await self._storage.get_scrapers()
+        """Poll storage for all existing scrapers and update corresponding scheduler jobs"""
+        scrapers = await self._scrapers_storage.get_scrapers()
         index = {scraper.id: scraper for scraper in scrapers}
         for existing in self._scrapers.values():
             if existing.id not in index:
                 self._remove_scraper_job(existing)
             elif self._scrapers[existing.id] != index[existing.id]:
                 await self._update_scraper_job(existing, remove_existing=True)
 
         for scraper in index.values():
             if scraper.id not in self._scrapers:
                 await self._update_scraper_job(scraper, remove_existing=False)
 
     @measure_latency(subsystem="scheduler")
     @count_invocations(subsystem="scheduler")
     async def _on_tick(self) -> None:
+        """Periodic job that:
+
+        * Tries to acquire lease to ensure that there's only single active scheduler replica that can enqueue jobs
+        * Updates internal (APScheduler) jobs that enqueue scrapers
+        """
         replicas_gauge.labels(type="total_scheduler").set(1)
         try:
             self._logger.debug("Starting scheduler update cycle")
             self._logger.debug("Trying to acquire lease")
-            self._lease = await self._storage.maybe_acquire_lease(
+            self._lease = await self._lease_storage.maybe_acquire_lease(
                 self._lease_name,
                 self._owner_id,
                 self._lease_duration,
             )
             if self._lease:
                 replicas_gauge.labels(type="active_scheduler").set(1)
                 self._logger.info(
@@ -209,68 +246,71 @@
             self._logger.error(f"Scheduler on tick function failed: {e}")
             self._logger.debug(
                 f"Scheduler on tick function failed. Traceback: {format_exc()}"
             )
 
     @measure_latency(subsystem="scheduler")
     @count_invocations(subsystem="scheduler")
-    async def _kill_dead_scraper_runs(self):
-        if not self._lease:
+    async def _kill_dead_scraper_jobs(self) -> None:
+        """Periodic job that kills scraper jobs that are active but haven't been pinged for a while"""
+        if not self._is_lease_acquired:
             return
         try:
-            semaphore = asyncio.Semaphore(self._max_kill_dead_runs_concurrency)
+            semaphore = asyncio.Semaphore(self._max_kill_dead_jobs_concurrency)
 
-            async def kill_dead_runs(scraper_id):
+            async def kill_dead_jobs(scraper_id):
                 async with semaphore:
-                    return await self._queue.kill_dead_scraper_runs(scraper_id)
+                    return await self._queue.kill_dead_scraper_jobs(scraper_id)
 
             scrapers = list(self._scrapers.keys())
-            self._logger.info(f"Killing dead runs for {len(scrapers)} scrapers")
-            kill_jobs = [kill_dead_runs(scraper) for scraper in scrapers]
+            self._logger.info(f"Killing dead jobs for {len(scrapers)} scrapers")
+            kill_jobs = [kill_dead_jobs(scraper) for scraper in scrapers]
             results = await asyncio.gather(*kill_jobs, return_exceptions=True)
             killed = sum(
                 [len(item) for item in results if not isinstance(item, Exception)]
             )
             failed = [item for item in results if isinstance(item, Exception)]
             if failed:
                 self._logger.error(
-                    f"Failed to kill dead runs for {len(failed)} scrapers: {failed}"
+                    f"Failed to kill dead jobs for {len(failed)} scrapers: {failed}"
                 )
             if killed > 0:
-                self._logger.info(f"Successfully killed {killed} dead runs")
+                self._logger.info(f"Successfully killed {killed} dead jobs")
         except Exception as e:
-            self._logger.error(f"Scheduler kill dead runs failed: {e}")
+            self._logger.error(f"Scheduler kill dead jobs failed: {e}")
             self._logger.debug(
-                f"Scheduler kill dead runs failed. Traceback: {format_exc()}"
+                f"Scheduler kill dead jobs failed. Traceback: {format_exc()}"
             )
 
     @measure_latency(subsystem="scheduler")
     @count_invocations(subsystem="scheduler")
-    async def _delete_old_scraper_runs(self):
-        if not self._lease:
+    async def _delete_old_scraper_jobs(self):
+        """Periodic job that cleans up storage from old historical scraper jobs"""
+        if not self._is_lease_acquired:
             return
         try:
-            self._logger.info("Removing old scraper runs")
-            await self._storage.delete_old_scraper_runs(self._runs_to_keep)
-            self._logger.info("Successfully removed old scraper runs")
+            self._logger.info("Removing old scraper jobs")
+            await self._jobs_storage.delete_old_scraper_jobs(self._jobs_to_keep)
+            self._logger.info("Successfully removed old scraper jobs")
         except Exception as e:
-            self._logger.error(f"Removing old scraper runs failed: {e}")
+            self._logger.error(f"Removing old scraper jobs failed: {e}")
             self._logger.debug(
-                f"Removing old scraper runs failed. Traceback: {format_exc()}"
+                f"Removing old scraper jobs failed. Traceback: {format_exc()}"
             )
 
     @measure_latency(subsystem="scheduler")
     @count_invocations(subsystem="scheduler")
     async def _export_queue_len(self):
-        if not self._lease:
+        """Periodic job that exports queue length metrics"""
+        if not self._is_lease_acquired:
             return
         try:
-            for priority in ScraperRunPriority:
-                pending_runs = await self._queue.get_queue_len(priority)
-                queue_length_gauge.labels(priority=priority.name).set(pending_runs)
+            for priority in ScraperJobPriority:
+                pending_jobs = await self._queue.get_queue_len(priority)
+                queue_length_gauge.labels(priority=priority.name).set(pending_jobs)
         except Exception as e:
             self._logger.error(f"Scheduler export queue length failed: {e}")
             self._logger.debug(
                 f"Scheduler export queue length failed. Traceback: {format_exc()}"
             )
 
     async def start(self) -> None:
```

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/ErrorNotFound.9617f9a7.js` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/ErrorNotFound.9617f9a7.js`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/KFOkCnqEu92Fr1MmgVxIIzQ.34e9582c.woff` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/KFOkCnqEu92Fr1MmgVxIIzQ.34e9582c.woff`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/KFOlCnqEu92Fr1MmEU9fBBc-.9ce7f3ac.woff` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/KFOlCnqEu92Fr1MmEU9fBBc-.9ce7f3ac.woff`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/KFOlCnqEu92Fr1MmSU5fBBc-.bf14c7d7.woff` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/KFOlCnqEu92Fr1MmSU5fBBc-.bf14c7d7.woff`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/KFOlCnqEu92Fr1MmWUlfBBc-.e0fd57c0.woff` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/KFOlCnqEu92Fr1MmWUlfBBc-.e0fd57c0.woff`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/KFOlCnqEu92Fr1MmYUtfBBc-.f6537e32.woff` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/KFOlCnqEu92Fr1MmYUtfBBc-.f6537e32.woff`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/KFOmCnqEu92Fr1Mu4mxM.f2abf7fb.woff` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/KFOmCnqEu92Fr1Mu4mxM.f2abf7fb.woff`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/MainLayout.06dc30a3.js` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/MainLayout.06dc30a3.js`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/NewScraperPage.abf42128.js` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/NewScraperPage.abf42128.js`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/PriorityChip.61343a15.js` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/PriorityChip.61343a15.js`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/QList.7f24c43e.js` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/QList.7f24c43e.js`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/QPage.6206ab40.js` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/QPage.6206ab40.js`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/ScraperEditForm.197dd68f.js` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/ScraperEditForm.197dd68f.js`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/ScraperEditForm.640de0df.css` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/ScraperEditForm.640de0df.css`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/ScraperPage.732b3035.js` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/ScraperPage.732b3035.js`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/ScrapersPage.06097019.js` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/ScrapersPage.06097019.js`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/api.8025d512.js` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/api.8025d512.js`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/fa-brands-400.20c4a58b.ttf` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/fa-brands-400.20c4a58b.ttf`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/fa-brands-400.74833209.woff2` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/fa-brands-400.74833209.woff2`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/fa-regular-400.528d022d.ttf` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/fa-regular-400.528d022d.ttf`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/fa-regular-400.8e7e5ea1.woff2` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/fa-regular-400.8e7e5ea1.woff2`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/fa-solid-900.67a65763.ttf` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/fa-solid-900.67a65763.ttf`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/fa-solid-900.7152a693.woff2` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/fa-solid-900.7152a693.woff2`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/fa-v4compatibility.0515a423.ttf` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/fa-v4compatibility.0515a423.ttf`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/fa-v4compatibility.694a17c3.woff2` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/fa-v4compatibility.694a17c3.woff2`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.fd84f88b.woff` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.fd84f88b.woff`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.4a4dbc62.woff2` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.4a4dbc62.woff2`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/index.422cc3a0.js` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/index.422cc3a0.js`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/assets/index.99b1d043.css` & `sneakpeek_py-0.1.5/sneakpeek/static/assets/index.99b1d043.css`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/favicon.ico` & `sneakpeek_py-0.1.5/sneakpeek/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/icons/favicon.png` & `sneakpeek_py-0.1.5/sneakpeek/static/icons/favicon.png`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.4/sneakpeek/static/index.html` & `sneakpeek_py-0.1.5/sneakpeek/static/index.html`

 * *Files identical despite different names*

