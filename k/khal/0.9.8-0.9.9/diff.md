# Comparing `tmp/khal-0.9.8.tar.gz` & `tmp/khal-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/khal-0.9.8.tar", last modified: Thu Oct  5 21:20:27 2017, max compression
+gzip compressed data, was "dist/khal-0.9.9.tar", last modified: Sat May 26 20:12:16 2018, max compression
```

## Comparing `khal-0.9.8.tar` & `khal-0.9.9.tar`

### file list

```diff
@@ -1,191 +1,192 @@
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/
--rw-rw-r--   0 cg        (1000) cg        (1000)       51 2016-09-07 22:40:53.000000 khal-0.9.8/CODE_OF_CONDUCT.rst
--rw-r--r--   0 cg        (1000) cg        (1000)       38 2017-10-05 21:20:27.000000 khal-0.9.8/setup.cfg
--rw-rw-r--   0 cg        (1000) cg        (1000)     3876 2017-03-29 23:16:15.000000 khal-0.9.8/README.rst
--rw-r--r--   0 cg        (1000) cg        (1000)     1813 2017-10-05 21:19:29.000000 khal-0.9.8/AUTHORS.txt
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/bin/
--rw-r--r--   0 cg        (1000) cg        (1000)       99 2017-07-01 17:31:33.000000 khal-0.9.8/bin/ikhal
--rw-r--r--   0 cg        (1000) cg        (1000)       97 2017-07-01 17:31:33.000000 khal-0.9.8/bin/khal
--rw-rw-r--   0 cg        (1000) cg        (1000)      179 2015-06-17 20:07:32.000000 khal-0.9.8/MANIFEST.in
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/khal/
--rw-r--r--   0 cg        (1000) cg        (1000)    24537 2017-10-05 21:19:29.000000 khal-0.9.8/khal/cli.py
--rw-r--r--   0 cg        (1000) cg        (1000)     8833 2017-10-05 21:19:29.000000 khal-0.9.8/khal/configwizard.py
--rw-r--r--   0 cg        (1000) cg        (1000)    23524 2017-10-05 21:19:29.000000 khal-0.9.8/khal/controllers.py
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/khal/settings/
--rw-rw-r--   0 cg        (1000) cg        (1000)     1342 2017-03-13 19:27:27.000000 khal-0.9.8/khal/settings/exceptions.py
--rw-r--r--   0 cg        (1000) cg        (1000)    13104 2017-10-05 21:19:29.000000 khal-0.9.8/khal/settings/khal.spec
--rw-rw-r--   0 cg        (1000) cg        (1000)       94 2017-01-30 23:30:33.000000 khal-0.9.8/khal/settings/__init__.py
--rw-r--r--   0 cg        (1000) cg        (1000)     7898 2017-10-05 21:19:29.000000 khal-0.9.8/khal/settings/utils.py
--rw-r--r--   0 cg        (1000) cg        (1000)     6883 2017-10-05 21:19:29.000000 khal-0.9.8/khal/settings/settings.py
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/khal/khalendar/
--rw-r--r--   0 cg        (1000) cg        (1000)     2175 2017-10-05 21:19:29.000000 khal-0.9.8/khal/khalendar/exceptions.py
--rw-r--r--   0 cg        (1000) cg        (1000)    26386 2017-10-05 21:19:29.000000 khal-0.9.8/khal/khalendar/backend.py
--rw-rw-r--   0 cg        (1000) cg        (1000)     1167 2017-03-13 19:27:27.000000 khal-0.9.8/khal/khalendar/__init__.py
--rw-r--r--   0 cg        (1000) cg        (1000)     8983 2017-10-05 21:19:29.000000 khal-0.9.8/khal/khalendar/vdir.py
--rw-r--r--   0 cg        (1000) cg        (1000)    13821 2017-10-05 21:19:29.000000 khal-0.9.8/khal/khalendar/khalendar.py
--rw-r--r--   0 cg        (1000) cg        (1000)    11816 2017-10-05 21:19:29.000000 khal-0.9.8/khal/khalendar/utils.py
--rw-r--r--   0 cg        (1000) cg        (1000)    30745 2017-10-05 21:19:29.000000 khal-0.9.8/khal/khalendar/event.py
--rw-rw-r--   0 cg        (1000) cg        (1000)     1184 2017-03-13 19:27:27.000000 khal-0.9.8/khal/__main__.py
--rw-r--r--   0 cg        (1000) cg        (1000)     1446 2017-10-05 21:19:29.000000 khal-0.9.8/khal/exceptions.py
--rw-rw-r--   0 cg        (1000) cg        (1000)      116 2017-10-05 21:20:26.000000 khal-0.9.8/khal/version.py
--rw-rw-r--   0 cg        (1000) cg        (1000)     1725 2017-03-13 19:27:27.000000 khal-0.9.8/khal/__init__.py
--rw-r--r--   0 cg        (1000) cg        (1000)     2184 2017-10-05 21:19:29.000000 khal-0.9.8/khal/log.py
--rw-r--r--   0 cg        (1000) cg        (1000)     7604 2017-10-05 21:19:29.000000 khal-0.9.8/khal/calendar_display.py
--rw-r--r--   0 cg        (1000) cg        (1000)    25482 2017-10-05 21:19:29.000000 khal-0.9.8/khal/utils.py
--rw-r--r--   0 cg        (1000) cg        (1000)     5598 2017-10-05 21:19:29.000000 khal-0.9.8/khal/terminal.py
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/khal/ui/
--rw-r--r--   0 cg        (1000) cg        (1000)    24359 2017-10-05 21:19:29.000000 khal-0.9.8/khal/ui/calendarwidget.py
--rw-r--r--   0 cg        (1000) cg        (1000)    47869 2017-10-05 21:19:29.000000 khal-0.9.8/khal/ui/__init__.py
--rw-r--r--   0 cg        (1000) cg        (1000)     3779 2017-10-05 21:19:29.000000 khal-0.9.8/khal/ui/colors.py
--rw-r--r--   0 cg        (1000) cg        (1000)    23895 2017-10-05 21:19:29.000000 khal-0.9.8/khal/ui/widgets.py
--rw-r--r--   0 cg        (1000) cg        (1000)     7218 2017-10-05 21:19:29.000000 khal-0.9.8/khal/ui/base.py
--rw-r--r--   0 cg        (1000) cg        (1000)    27553 2017-10-05 21:19:47.000000 khal-0.9.8/khal/ui/editor.py
--rw-r--r--   0 cg        (1000) cg        (1000)      583 2017-10-05 21:19:29.000000 khal-0.9.8/khal.conf.sample
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/khal.egg-info/
--rw-rw-r--   0 cg        (1000) cg        (1000)        1 2017-03-06 19:50:17.000000 khal-0.9.8/khal.egg-info/not-zip-safe
--rw-rw-r--   0 cg        (1000) cg        (1000)        1 2017-10-05 21:20:27.000000 khal-0.9.8/khal.egg-info/dependency_links.txt
--rw-rw-r--   0 cg        (1000) cg        (1000)       42 2017-10-05 21:20:27.000000 khal-0.9.8/khal.egg-info/top_level.txt
--rw-rw-r--   0 cg        (1000) cg        (1000)     4265 2017-10-05 21:20:27.000000 khal-0.9.8/khal.egg-info/SOURCES.txt
--rw-rw-r--   0 cg        (1000) cg        (1000)      123 2017-10-05 21:20:27.000000 khal-0.9.8/khal.egg-info/requires.txt
--rw-rw-r--   0 cg        (1000) cg        (1000)     5478 2017-10-05 21:20:27.000000 khal-0.9.8/khal.egg-info/PKG-INFO
--rw-rw-r--   0 cg        (1000) cg        (1000)       73 2017-10-05 21:20:27.000000 khal-0.9.8/khal.egg-info/entry_points.txt
--rw-r--r--   0 cg        (1000) cg        (1000)    19038 2017-10-05 21:19:47.000000 khal-0.9.8/CHANGELOG.rst
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/misc/
--rw-rw-r--   0 cg        (1000) cg        (1000)     1152 2016-02-28 16:43:59.000000 khal-0.9.8/misc/mutt2khal
--rw-rw-r--   0 cg        (1000) cg        (1000)     2906 2017-03-13 19:27:27.000000 khal-0.9.8/misc/__khal
--rw-rw-r--   0 cg        (1000) cg        (1000)      818 2017-04-07 23:18:22.000000 khal-0.9.8/tox.ini
--rw-rw-r--   0 cg        (1000) cg        (1000)      410 2017-04-07 23:18:22.000000 khal-0.9.8/.travis.yml
--rw-rw-r--   0 cg        (1000) cg        (1000)       71 2016-08-28 20:54:45.000000 khal-0.9.8/codecov.yml
--rwxr-xr-x   0 cg        (1000) cg        (1000)     2176 2017-10-05 21:19:29.000000 khal-0.9.8/setup.py
--rw-rw-r--   0 cg        (1000) cg        (1000)     1071 2017-03-13 19:27:27.000000 khal-0.9.8/COPYING
--rw-rw-r--   0 cg        (1000) cg        (1000)       21 2017-01-25 23:33:47.000000 khal-0.9.8/.coveragerc
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/doc/
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/doc/source/
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/doc/source/ystatic/
--rw-rw-r--   0 cg        (1000) cg        (1000)        0 2015-01-28 23:39:45.000000 khal-0.9.8/doc/source/ystatic/.gitignore
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/doc/source/ytemplates/
--rw-rw-r--   0 cg        (1000) cg        (1000)      197 2015-01-28 23:39:45.000000 khal-0.9.8/doc/source/ytemplates/layout.html
--rw-r--r--   0 cg        (1000) cg        (1000)     3278 2017-07-01 17:31:33.000000 khal-0.9.8/doc/source/install.rst
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/doc/source/images/
--rw-rw-r--   0 cg        (1000) cg        (1000)      896 2015-01-28 23:39:45.000000 khal-0.9.8/doc/source/images/rss.png
--rw-r--r--   0 cg        (1000) cg        (1000)    16648 2017-10-05 21:19:29.000000 khal-0.9.8/doc/source/configspec.rst
--rw-r--r--   0 cg        (1000) cg        (1000)    10515 2017-10-05 21:19:29.000000 khal-0.9.8/doc/source/hacking.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      354 2016-02-28 16:43:59.000000 khal-0.9.8/doc/source/man.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)     1220 2016-12-10 23:48:43.000000 khal-0.9.8/doc/source/index.rst
--rw-r--r--   0 cg        (1000) cg        (1000)     2377 2017-10-05 21:19:29.000000 khal-0.9.8/doc/source/feedback.rst
--rw-r--r--   0 cg        (1000) cg        (1000)     2085 2017-07-01 17:31:33.000000 khal-0.9.8/doc/source/configure.rst
--rw-r--r--   0 cg        (1000) cg        (1000)    15987 2017-10-05 21:19:29.000000 khal-0.9.8/doc/source/usage.rst
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/doc/source/news/
--rw-rw-r--   0 cg        (1000) cg        (1000)     1134 2017-03-13 19:27:27.000000 khal-0.9.8/doc/source/news/khal092.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)     1857 2016-12-10 23:48:43.000000 khal-0.9.8/doc/source/news/khal084.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)     1221 2017-03-29 23:16:15.000000 khal-0.9.8/doc/source/news/khal02.rst
--rw-r--r--   0 cg        (1000) cg        (1000)      681 2017-09-15 21:20:39.000000 khal-0.9.8/doc/source/news/khal097.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      560 2016-06-02 20:47:44.000000 khal-0.9.8/doc/source/news/khal082.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      627 2015-01-28 23:39:45.000000 khal-0.9.8/doc/source/news/khal031.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)     1030 2017-01-25 23:45:44.000000 khal-0.9.8/doc/source/news/khal091.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      967 2016-06-02 20:47:44.000000 khal-0.9.8/doc/source/news/khal08.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      453 2017-04-07 23:21:40.000000 khal-0.9.8/doc/source/news/khal095.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      413 2015-01-28 23:39:45.000000 khal-0.9.8/doc/source/news/30c3.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      873 2016-02-28 16:43:59.000000 khal-0.9.8/doc/source/news/khal07.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      355 2016-08-28 22:05:03.000000 khal-0.9.8/doc/source/news/khal083.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      754 2015-06-13 11:11:49.000000 khal-0.9.8/doc/source/news/khal05.rst
--rw-r--r--   0 cg        (1000) cg        (1000)      467 2017-07-01 17:31:33.000000 khal-0.9.8/doc/source/news/khal096.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      227 2015-01-28 23:39:45.000000 khal-0.9.8/doc/source/news/khal011.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      922 2016-12-10 23:48:43.000000 khal-0.9.8/doc/source/news/khal071.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      722 2017-03-29 23:16:15.000000 khal-0.9.8/doc/source/news/khal093.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      595 2015-01-28 23:39:45.000000 khal-0.9.8/doc/source/news/khal01.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      797 2015-02-20 16:45:41.000000 khal-0.9.8/doc/source/news/khal04.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)     1334 2015-01-28 23:39:45.000000 khal-0.9.8/doc/source/news/khal03.rst
--rw-r--r--   0 cg        (1000) cg        (1000)      693 2017-10-05 21:19:47.000000 khal-0.9.8/doc/source/news/khal098.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      599 2015-01-28 23:39:45.000000 khal-0.9.8/doc/source/news/callfortesting.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      416 2015-02-13 22:08:39.000000 khal-0.9.8/doc/source/news/31c3.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)     1077 2017-03-29 23:16:15.000000 khal-0.9.8/doc/source/news/khal09.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      760 2015-07-14 23:21:30.000000 khal-0.9.8/doc/source/news/khal06.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      362 2016-06-02 20:47:44.000000 khal-0.9.8/doc/source/news/khal081.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      866 2017-03-29 23:16:15.000000 khal-0.9.8/doc/source/news/khal094.rst
--rw-r--r--   0 cg        (1000) cg        (1000)     1097 2017-07-01 17:31:33.000000 khal-0.9.8/doc/source/faq.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)     1195 2017-03-13 19:27:27.000000 khal-0.9.8/doc/source/license.rst
--rw-r--r--   0 cg        (1000) cg        (1000)      793 2017-10-05 21:19:47.000000 khal-0.9.8/doc/source/news.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)       49 2015-06-01 21:39:03.000000 khal-0.9.8/doc/source/changelog.rst
--rw-r--r--   0 cg        (1000) cg        (1000)    11491 2017-10-05 21:19:29.000000 khal-0.9.8/doc/source/conf.py
--rw-r--r--   0 cg        (1000) cg        (1000)     4298 2017-07-01 17:31:33.000000 khal-0.9.8/doc/source/standards.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)     6771 2017-03-29 23:16:15.000000 khal-0.9.8/doc/Makefile
--rw-r--r--   0 cg        (1000) cg        (1000)       37 2017-07-01 17:31:33.000000 khal-0.9.8/doc/requirements.txt
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/doc/webpage/
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/doc/webpage/src/
--rw-rw-r--   0 cg        (1000) cg        (1000)      197 2015-01-28 23:39:45.000000 khal-0.9.8/doc/webpage/src/new_rss_url.rst
--rw-rw-r--   0 cg        (1000) cg        (1000)      124 2016-12-10 23:48:43.000000 khal-0.9.8/CONTRIBUTING.rst
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/tests/
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/tests/ics/
--rw-rw-r--   0 cg        (1000) cg        (1000)      293 2016-02-28 16:43:59.000000 khal-0.9.8/tests/ics/event_dt_two_rd.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      246 2016-02-28 16:43:59.000000 khal-0.9.8/tests/ics/event_dt_duration.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      312 2015-02-20 16:45:41.000000 khal-0.9.8/tests/ics/event_dtr_exdatez.ics
--rw-r--r--   0 cg        (1000) cg        (1000)     2807 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/cal_lots_of_timezones.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      209 2017-08-16 22:08:14.000000 khal-0.9.8/tests/ics/event_dt_floating.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      201 2016-04-12 21:07:42.000000 khal-0.9.8/tests/ics/event_dt_long.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      119 2016-02-28 16:43:59.000000 khal-0.9.8/tests/ics/event_d_no_value.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      105 2016-04-12 21:07:42.000000 khal-0.9.8/tests/ics/event_dt_no_end.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      335 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/event_dt_london.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      256 2016-02-28 16:43:59.000000 khal-0.9.8/tests/ics/event_d_rdate.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      208 2016-04-12 21:07:42.000000 khal-0.9.8/tests/ics/event_d_rr.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      177 2016-02-28 16:43:59.000000 khal-0.9.8/tests/ics/event_d.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      267 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/event_dt_simple_zulu.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      442 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/event_rrule_recuid_invalid_tzid.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      296 2015-02-20 16:45:41.000000 khal-0.9.8/tests/ics/event_dtr_notz_untilz.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      313 2016-08-28 20:54:45.000000 khal-0.9.8/tests/ics/event_invalid_exdate.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      306 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/event_dt_rrule_invalid_until.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      675 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/event_rrule_recuid_cancelled.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      211 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/event_dt_recuid_no_master.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      675 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/event_dt_simple_inkl_vtimezone.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      583 2016-04-12 21:07:42.000000 khal-0.9.8/tests/ics/event_dt_mixed_awareness.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      315 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/event_dt_local_missing_tz.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      182 2016-04-12 21:07:42.000000 khal-0.9.8/tests/ics/event_d_long.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      429 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/event_dt_multi_recuid_no_master.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      239 2016-04-12 21:07:42.000000 khal-0.9.8/tests/ics/event_dt_rd.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      375 2016-08-28 22:05:03.000000 khal-0.9.8/tests/ics/event_rdate_no_value.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      420 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/event_dt_simple_updated.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      578 2016-02-28 16:43:59.000000 khal-0.9.8/tests/ics/mult_uids_and_recuid_no_order.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      269 2015-06-22 13:19:43.000000 khal-0.9.8/tests/ics/event_rrule_recuid_update.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      335 2017-07-03 22:35:10.000000 khal-0.9.8/tests/ics/event_dt_simple.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      474 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/event_rrule_recuid.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      242 2016-04-12 21:07:42.000000 khal-0.9.8/tests/ics/event_dt_two_tz.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      177 2016-02-28 16:43:59.000000 khal-0.9.8/tests/ics/event_d_15.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      227 2016-04-12 21:07:42.000000 khal-0.9.8/tests/ics/event_dt_rr.ics
--rw-r--r--   0 cg        (1000) cg        (1000)     1020 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/cal_dt_two_tz.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      401 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/event_dt_simple_nocat.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      273 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/cal_d.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      478 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/cal_no_dst.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      360 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/event_dt_rrule_invalid_until2.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      218 2016-02-28 16:43:59.000000 khal-0.9.8/tests/ics/event_no_dst.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      182 2016-02-28 16:43:59.000000 khal-0.9.8/tests/ics/event_d_same_start_end.ics
--rw-r--r--   0 cg        (1000) cg        (1000)     2101 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/part1.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      177 2016-04-12 21:07:42.000000 khal-0.9.8/tests/ics/event_r_past.ics
--rw-r--r--   0 cg        (1000) cg        (1000)      628 2017-07-01 17:31:33.000000 khal-0.9.8/tests/ics/part0.ics
--rw-rw-r--   0 cg        (1000) cg        (1000)      337 2015-02-20 16:45:41.000000 khal-0.9.8/tests/ics/event_dtr_no_tz_exdatez.ics
--rw-r--r--   0 cg        (1000) cg        (1000)    28017 2017-10-05 21:19:29.000000 khal-0.9.8/tests/cli_test.py
--rw-rw-r--   0 cg        (1000) cg        (1000)        0 2017-01-30 23:30:33.000000 khal-0.9.8/tests/__init__.py
--rw-r--r--   0 cg        (1000) cg        (1000)     2917 2017-10-05 21:19:29.000000 khal-0.9.8/tests/conftest.py
--rw-r--r--   0 cg        (1000) cg        (1000)    16186 2017-10-05 21:19:29.000000 khal-0.9.8/tests/khalendar_test.py
--rw-r--r--   0 cg        (1000) cg        (1000)      288 2017-10-05 21:19:29.000000 khal-0.9.8/tests/configwizard_test.py
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/tests/configs/
--rw-rw-r--   0 cg        (1000) cg        (1000)      139 2015-02-13 22:08:39.000000 khal-0.9.8/tests/configs/small.conf
--rw-rw-r--   0 cg        (1000) cg        (1000)      281 2015-01-28 23:39:45.000000 khal-0.9.8/tests/configs/simple.conf
--rw-rw-r--   0 cg        (1000) cg        (1000)      197 2015-01-28 23:39:45.000000 khal-0.9.8/tests/configs/nocalendars.conf
--rw-r--r--   0 cg        (1000) cg        (1000)     7097 2017-10-05 21:19:29.000000 khal-0.9.8/tests/controller_test.py
--rw-r--r--   0 cg        (1000) cg        (1000)    11933 2017-10-05 21:19:29.000000 khal-0.9.8/tests/cal_display_test.py
--rw-r--r--   0 cg        (1000) cg        (1000)    24655 2017-10-05 21:19:29.000000 khal-0.9.8/tests/khalendar_utils_test.py
--rw-r--r--   0 cg        (1000) cg        (1000)     1414 2017-10-05 21:19:29.000000 khal-0.9.8/tests/terminal_test.py
--rw-r--r--   0 cg        (1000) cg        (1000)    26673 2017-10-05 21:19:29.000000 khal-0.9.8/tests/utils_test.py
--rw-r--r--   0 cg        (1000) cg        (1000)    31472 2017-10-05 21:19:29.000000 khal-0.9.8/tests/backend_test.py
--rw-r--r--   0 cg        (1000) cg        (1000)     3169 2017-10-05 21:19:29.000000 khal-0.9.8/tests/utils.py
--rw-r--r--   0 cg        (1000) cg        (1000)    20596 2017-10-05 21:19:29.000000 khal-0.9.8/tests/event_test.py
--rw-r--r--   0 cg        (1000) cg        (1000)     9493 2017-10-05 21:19:29.000000 khal-0.9.8/tests/settings_test.py
--rw-r--r--   0 cg        (1000) cg        (1000)     2295 2017-10-05 21:19:29.000000 khal-0.9.8/tests/vtimezone_test.py
-drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2017-10-05 21:20:27.000000 khal-0.9.8/tests/ui/
--rw-rw-r--   0 cg        (1000) cg        (1000)        0 2017-01-30 23:30:33.000000 khal-0.9.8/tests/ui/__init__.py
--rw-r--r--   0 cg        (1000) cg        (1000)     1641 2017-10-05 21:19:29.000000 khal-0.9.8/tests/ui/test_editor.py
--rw-rw-r--   0 cg        (1000) cg        (1000)      975 2017-01-30 23:30:33.000000 khal-0.9.8/tests/ui/test_widgets.py
--rw-r--r--   0 cg        (1000) cg        (1000)     2099 2017-10-05 21:19:29.000000 khal-0.9.8/tests/ui/test_calendarwidget.py
--rw-rw-r--   0 cg        (1000) cg        (1000)     2385 2017-03-13 19:27:27.000000 khal-0.9.8/tests/vdir_test.py
--rw-r--r--   0 cg        (1000) cg        (1000)     5478 2017-10-05 21:20:27.000000 khal-0.9.8/PKG-INFO
--rw-rw-r--   0 cg        (1000) cg        (1000)      131 2017-03-29 23:16:15.000000 khal-0.9.8/.gitignore
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/bin/
+-rw-r--r--   0 cg        (1000) cg        (1000)       99 2018-02-06 22:25:16.000000 khal-0.9.9/bin/ikhal
+-rw-r--r--   0 cg        (1000) cg        (1000)       97 2018-02-06 22:25:16.000000 khal-0.9.9/bin/khal
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/doc/
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/doc/source/
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/doc/source/images/
+-rw-r--r--   0 cg        (1000) cg        (1000)      896 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/images/rss.png
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/doc/source/news/
+-rw-r--r--   0 cg        (1000) cg        (1000)      413 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/30c3.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      416 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/31c3.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      599 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/callfortesting.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      595 2018-05-26 19:53:13.000000 khal-0.9.9/doc/source/news/khal01.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      227 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal011.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)     1221 2018-05-26 19:53:13.000000 khal-0.9.9/doc/source/news/khal02.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)     1334 2018-05-26 19:53:13.000000 khal-0.9.9/doc/source/news/khal03.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      627 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal031.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      797 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal04.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      754 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal05.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      760 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal06.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      873 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal07.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      922 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal071.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      967 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal08.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      362 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal081.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      560 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal082.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      355 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal083.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)     1857 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal084.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)     1077 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal09.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)     1030 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal091.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)     1134 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal092.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      722 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal093.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      866 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal094.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      453 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/news/khal095.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      467 2018-02-06 22:25:16.000000 khal-0.9.9/doc/source/news/khal096.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      681 2018-02-06 22:25:16.000000 khal-0.9.9/doc/source/news/khal097.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      693 2018-02-06 22:25:16.000000 khal-0.9.9/doc/source/news/khal098.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      645 2018-05-26 20:08:42.000000 khal-0.9.9/doc/source/news/khal099.rst
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/doc/source/ystatic/
+-rw-r--r--   0 cg        (1000) cg        (1000)        0 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/ystatic/.gitignore
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/doc/source/ytemplates/
+-rw-r--r--   0 cg        (1000) cg        (1000)      197 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/ytemplates/layout.html
+-rw-r--r--   0 cg        (1000) cg        (1000)       49 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/changelog.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)    11491 2018-05-26 19:53:13.000000 khal-0.9.9/doc/source/conf.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    16648 2018-05-26 20:10:00.000000 khal-0.9.9/doc/source/configspec.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)     2085 2018-05-26 19:53:13.000000 khal-0.9.9/doc/source/configure.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)     1097 2018-02-06 22:25:16.000000 khal-0.9.9/doc/source/faq.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)     2377 2018-05-26 19:53:13.000000 khal-0.9.9/doc/source/feedback.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)    10515 2018-05-26 19:53:13.000000 khal-0.9.9/doc/source/hacking.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)     1220 2018-05-26 19:53:13.000000 khal-0.9.9/doc/source/index.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)     3278 2018-05-26 19:53:13.000000 khal-0.9.9/doc/source/install.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)     1195 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/license.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      354 2017-12-29 19:04:53.000000 khal-0.9.9/doc/source/man.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      810 2018-05-26 19:59:40.000000 khal-0.9.9/doc/source/news.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)     4298 2018-02-06 22:25:16.000000 khal-0.9.9/doc/source/standards.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)    15987 2018-05-26 19:53:13.000000 khal-0.9.9/doc/source/usage.rst
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/doc/webpage/
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/doc/webpage/src/
+-rw-r--r--   0 cg        (1000) cg        (1000)      197 2017-12-29 19:04:53.000000 khal-0.9.9/doc/webpage/src/new_rss_url.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)     6771 2017-12-29 19:04:53.000000 khal-0.9.9/doc/Makefile
+-rw-r--r--   0 cg        (1000) cg        (1000)       37 2018-02-06 22:25:16.000000 khal-0.9.9/doc/requirements.txt
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/khal/
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/khal/khalendar/
+-rw-r--r--   0 cg        (1000) cg        (1000)     1167 2017-12-29 19:04:53.000000 khal-0.9.9/khal/khalendar/__init__.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    26386 2018-05-26 19:53:13.000000 khal-0.9.9/khal/khalendar/backend.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    30745 2018-05-26 19:53:13.000000 khal-0.9.9/khal/khalendar/event.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     2175 2018-05-26 19:53:13.000000 khal-0.9.9/khal/khalendar/exceptions.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    13821 2018-05-26 19:53:13.000000 khal-0.9.9/khal/khalendar/khalendar.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    11816 2018-05-26 19:53:13.000000 khal-0.9.9/khal/khalendar/utils.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     8983 2018-05-26 19:53:13.000000 khal-0.9.9/khal/khalendar/vdir.py
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/khal/settings/
+-rw-r--r--   0 cg        (1000) cg        (1000)       94 2017-12-29 19:04:53.000000 khal-0.9.9/khal/settings/__init__.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     1342 2017-12-29 19:04:53.000000 khal-0.9.9/khal/settings/exceptions.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    13104 2018-05-26 19:53:13.000000 khal-0.9.9/khal/settings/khal.spec
+-rw-r--r--   0 cg        (1000) cg        (1000)     6883 2018-05-26 19:53:13.000000 khal-0.9.9/khal/settings/settings.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     7898 2018-05-26 19:53:13.000000 khal-0.9.9/khal/settings/utils.py
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/khal/ui/
+-rw-r--r--   0 cg        (1000) cg        (1000)    47869 2018-05-26 19:53:13.000000 khal-0.9.9/khal/ui/__init__.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     7218 2018-05-26 19:53:13.000000 khal-0.9.9/khal/ui/base.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    24444 2018-05-26 19:53:13.000000 khal-0.9.9/khal/ui/calendarwidget.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     3779 2018-05-26 19:53:13.000000 khal-0.9.9/khal/ui/colors.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    27553 2018-05-26 19:53:13.000000 khal-0.9.9/khal/ui/editor.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    23895 2018-05-26 19:53:13.000000 khal-0.9.9/khal/ui/widgets.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     1725 2017-12-29 19:04:53.000000 khal-0.9.9/khal/__init__.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     1184 2017-12-29 19:04:53.000000 khal-0.9.9/khal/__main__.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     7604 2018-05-26 19:53:13.000000 khal-0.9.9/khal/calendar_display.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    24704 2018-05-26 19:53:13.000000 khal-0.9.9/khal/cli.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     8833 2018-05-26 19:53:13.000000 khal-0.9.9/khal/configwizard.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    23524 2018-05-26 19:53:13.000000 khal-0.9.9/khal/controllers.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     1446 2018-05-26 19:53:13.000000 khal-0.9.9/khal/exceptions.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     2184 2018-05-26 19:53:13.000000 khal-0.9.9/khal/log.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     5598 2018-05-26 19:53:13.000000 khal-0.9.9/khal/terminal.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    25482 2018-05-26 19:53:13.000000 khal-0.9.9/khal/utils.py
+-rw-r--r--   0 cg        (1000) cg        (1000)      116 2018-05-26 20:12:15.000000 khal-0.9.9/khal/version.py
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/khal.egg-info/
+-rw-r--r--   0 cg        (1000) cg        (1000)     5470 2018-05-26 20:12:15.000000 khal-0.9.9/khal.egg-info/PKG-INFO
+-rw-r--r--   0 cg        (1000) cg        (1000)     4293 2018-05-26 20:12:15.000000 khal-0.9.9/khal.egg-info/SOURCES.txt
+-rw-r--r--   0 cg        (1000) cg        (1000)        1 2018-05-26 20:12:15.000000 khal-0.9.9/khal.egg-info/dependency_links.txt
+-rw-r--r--   0 cg        (1000) cg        (1000)       73 2018-05-26 20:12:15.000000 khal-0.9.9/khal.egg-info/entry_points.txt
+-rw-r--r--   0 cg        (1000) cg        (1000)        1 2017-12-29 19:05:47.000000 khal-0.9.9/khal.egg-info/not-zip-safe
+-rw-r--r--   0 cg        (1000) cg        (1000)      130 2018-05-26 20:12:15.000000 khal-0.9.9/khal.egg-info/requires.txt
+-rw-r--r--   0 cg        (1000) cg        (1000)       42 2018-05-26 20:12:15.000000 khal-0.9.9/khal.egg-info/top_level.txt
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/misc/
+-rw-r--r--   0 cg        (1000) cg        (1000)     2906 2018-05-26 19:53:13.000000 khal-0.9.9/misc/__khal
+-rw-r--r--   0 cg        (1000) cg        (1000)     1152 2018-05-26 19:53:13.000000 khal-0.9.9/misc/mutt2khal
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/tests/
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/tests/configs/
+-rw-r--r--   0 cg        (1000) cg        (1000)      197 2017-12-29 19:04:53.000000 khal-0.9.9/tests/configs/nocalendars.conf
+-rw-r--r--   0 cg        (1000) cg        (1000)      281 2017-12-29 19:04:53.000000 khal-0.9.9/tests/configs/simple.conf
+-rw-r--r--   0 cg        (1000) cg        (1000)      139 2017-12-29 19:04:53.000000 khal-0.9.9/tests/configs/small.conf
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/tests/ics/
+-rw-r--r--   0 cg        (1000) cg        (1000)      273 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/cal_d.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)     1020 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/cal_dt_two_tz.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)     2807 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/cal_lots_of_timezones.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      478 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/cal_no_dst.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      177 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_d.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      177 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_d_15.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      182 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_d_long.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      119 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_d_no_value.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      256 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_d_rdate.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      208 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_d_rr.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      182 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_d_same_start_end.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      246 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_dt_duration.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      209 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/event_dt_floating.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      315 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/event_dt_local_missing_tz.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      335 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/event_dt_london.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      201 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_dt_long.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      583 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_dt_mixed_awareness.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      429 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/event_dt_multi_recuid_no_master.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      105 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_dt_no_end.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      239 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_dt_rd.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      211 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/event_dt_recuid_no_master.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      227 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_dt_rr.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      306 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/event_dt_rrule_invalid_until.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      360 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/event_dt_rrule_invalid_until2.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      335 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/event_dt_simple.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      675 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/event_dt_simple_inkl_vtimezone.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      401 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/event_dt_simple_nocat.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      420 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/event_dt_simple_updated.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      267 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/event_dt_simple_zulu.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      293 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_dt_two_rd.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      242 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_dt_two_tz.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      312 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_dtr_exdatez.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      337 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_dtr_no_tz_exdatez.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      296 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_dtr_notz_untilz.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      313 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_invalid_exdate.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      218 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_no_dst.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      177 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_r_past.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      375 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_rdate_no_value.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      474 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/event_rrule_recuid.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      675 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/event_rrule_recuid_cancelled.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      442 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/event_rrule_recuid_invalid_tzid.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      269 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/event_rrule_recuid_update.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      578 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ics/mult_uids_and_recuid_no_order.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)      628 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/part0.ics
+-rw-r--r--   0 cg        (1000) cg        (1000)     2101 2018-02-06 22:25:16.000000 khal-0.9.9/tests/ics/part1.ics
+drwxr-xr-x   0 cg        (1000) cg        (1000)        0 2018-05-26 20:12:16.000000 khal-0.9.9/tests/ui/
+-rw-r--r--   0 cg        (1000) cg        (1000)        0 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ui/__init__.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     2099 2018-05-26 19:53:13.000000 khal-0.9.9/tests/ui/test_calendarwidget.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     1641 2018-05-26 19:53:13.000000 khal-0.9.9/tests/ui/test_editor.py
+-rw-r--r--   0 cg        (1000) cg        (1000)      975 2017-12-29 19:04:53.000000 khal-0.9.9/tests/ui/test_widgets.py
+-rw-r--r--   0 cg        (1000) cg        (1000)        0 2017-12-29 19:04:53.000000 khal-0.9.9/tests/__init__.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    31472 2018-05-26 19:53:13.000000 khal-0.9.9/tests/backend_test.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    11933 2018-05-26 19:53:13.000000 khal-0.9.9/tests/cal_display_test.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    28017 2018-05-26 19:53:13.000000 khal-0.9.9/tests/cli_test.py
+-rw-r--r--   0 cg        (1000) cg        (1000)      288 2018-05-26 19:53:13.000000 khal-0.9.9/tests/configwizard_test.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     2917 2018-05-26 19:53:13.000000 khal-0.9.9/tests/conftest.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     7097 2018-05-26 19:53:13.000000 khal-0.9.9/tests/controller_test.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    20596 2018-05-26 19:53:13.000000 khal-0.9.9/tests/event_test.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    16186 2018-05-26 19:53:13.000000 khal-0.9.9/tests/khalendar_test.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    24655 2018-05-26 19:53:13.000000 khal-0.9.9/tests/khalendar_utils_test.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     9493 2018-05-26 19:53:13.000000 khal-0.9.9/tests/settings_test.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     1414 2018-05-26 19:53:13.000000 khal-0.9.9/tests/terminal_test.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     3169 2018-05-26 19:53:13.000000 khal-0.9.9/tests/utils.py
+-rw-r--r--   0 cg        (1000) cg        (1000)    26673 2018-05-26 19:53:13.000000 khal-0.9.9/tests/utils_test.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     2385 2017-12-29 19:04:53.000000 khal-0.9.9/tests/vdir_test.py
+-rw-r--r--   0 cg        (1000) cg        (1000)     2295 2018-05-26 19:53:13.000000 khal-0.9.9/tests/vtimezone_test.py
+-rw-r--r--   0 cg        (1000) cg        (1000)       21 2017-12-29 19:04:53.000000 khal-0.9.9/.coveragerc
+-rw-r--r--   0 cg        (1000) cg        (1000)      131 2018-05-26 19:53:13.000000 khal-0.9.9/.gitignore
+-rw-r--r--   0 cg        (1000) cg        (1000)      410 2018-05-26 19:53:13.000000 khal-0.9.9/.travis.yml
+-rw-r--r--   0 cg        (1000) cg        (1000)     1813 2018-05-26 19:53:13.000000 khal-0.9.9/AUTHORS.txt
+-rw-r--r--   0 cg        (1000) cg        (1000)    19143 2018-05-26 19:54:42.000000 khal-0.9.9/CHANGELOG.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)       51 2017-12-29 19:04:53.000000 khal-0.9.9/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)      124 2017-12-29 19:04:53.000000 khal-0.9.9/CONTRIBUTING.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)     1071 2017-12-29 19:04:53.000000 khal-0.9.9/COPYING
+-rw-r--r--   0 cg        (1000) cg        (1000)      179 2017-12-29 19:04:53.000000 khal-0.9.9/MANIFEST.in
+-rw-r--r--   0 cg        (1000) cg        (1000)     3876 2018-05-26 19:53:13.000000 khal-0.9.9/README.rst
+-rw-r--r--   0 cg        (1000) cg        (1000)       71 2017-12-29 19:04:53.000000 khal-0.9.9/codecov.yml
+-rw-r--r--   0 cg        (1000) cg        (1000)      583 2018-05-26 19:53:13.000000 khal-0.9.9/khal.conf.sample
+-rwxr-xr-x   0 cg        (1000) cg        (1000)     2183 2018-05-26 19:53:19.000000 khal-0.9.9/setup.py
+-rw-r--r--   0 cg        (1000) cg        (1000)      825 2018-05-26 19:53:13.000000 khal-0.9.9/tox.ini
+-rw-r--r--   0 cg        (1000) cg        (1000)     5470 2018-05-26 20:12:16.000000 khal-0.9.9/PKG-INFO
+-rw-r--r--   0 cg        (1000) cg        (1000)       38 2018-05-26 20:12:16.000000 khal-0.9.9/setup.cfg
```

### Comparing `khal-0.9.8/README.rst` & `khal-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/AUTHORS.txt` & `khal-0.9.9/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/cli.py` & `khal-0.9.9/khal/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 # LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 # WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 import logging
+import os
 import sys
 import textwrap
 from shutil import get_terminal_size
 import datetime
 
 try:
     from setproctitle import setproctitle
@@ -431,15 +432,19 @@
                 'When using batch import, please specify a calendar to import '
                 'into or set the `default_calendar` in the config file.')
 
         try:
             # Default to stdin:
             if not ics:
                 ics_strs = (sys.stdin.read(),)
-                sys.stdin = open('/dev/tty', 'r')
+                if not batch:
+                    if os.path.isfile('/dev/tty'):
+                        sys.stdin = open('/dev/tty', 'r')
+                    else:
+                        logger.warning('/dev/tty does not exist, importing might not work')
             else:
                 ics_strs = (ics_file.read() for ics_file in ics)
 
             for ics_str in ics_strs:
                 controllers.import_ics(
                     collection,
                     ctx.obj['conf'],
@@ -519,15 +524,14 @@
         try:
             if ics:
                 ics_str = ics.read()
                 name = ics.name
             else:
                 ics_str = sys.stdin.read()
                 name = 'stdin input'
-                sys.stdin = open('/dev/tty', 'r')
             controllers.print_ics(ctx.obj['conf'], name, ics_str, format)
         except FatalError as error:
             logger.fatal(error)
             sys.exit(1)
 
     @cli.command()
     @multi_calendar_option
```

### Comparing `khal-0.9.8/khal/configwizard.py` & `khal-0.9.9/khal/configwizard.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/controllers.py` & `khal-0.9.9/khal/controllers.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/settings/exceptions.py` & `khal-0.9.9/khal/settings/exceptions.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/settings/khal.spec` & `khal-0.9.9/khal/settings/khal.spec`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/settings/utils.py` & `khal-0.9.9/khal/settings/utils.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/settings/settings.py` & `khal-0.9.9/khal/settings/settings.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/khalendar/exceptions.py` & `khal-0.9.9/khal/khalendar/exceptions.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/khalendar/backend.py` & `khal-0.9.9/khal/khalendar/backend.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/khalendar/__init__.py` & `khal-0.9.9/khal/khalendar/__init__.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/khalendar/vdir.py` & `khal-0.9.9/khal/khalendar/vdir.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/khalendar/khalendar.py` & `khal-0.9.9/khal/khalendar/khalendar.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/khalendar/utils.py` & `khal-0.9.9/khal/khalendar/utils.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/khalendar/event.py` & `khal-0.9.9/khal/khalendar/event.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/__main__.py` & `khal-0.9.9/khal/__main__.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/exceptions.py` & `khal-0.9.9/khal/exceptions.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/__init__.py` & `khal-0.9.9/khal/__init__.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/log.py` & `khal-0.9.9/khal/log.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/calendar_display.py` & `khal-0.9.9/khal/calendar_display.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/utils.py` & `khal-0.9.9/khal/utils.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/terminal.py` & `khal-0.9.9/khal/terminal.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/ui/calendarwidget.py` & `khal-0.9.9/khal/ui/calendarwidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -615,16 +615,17 @@
                 else:
                     return None
         if get_styles is None:
             get_styles = _get_styles
 
         if weeknumbers == 'right':
             dnames.append('#w')
+        month_names_length = get_month_abbr_len()
         dnames = urwid.Columns(
-            [(4, urwid.Text('    '))] +
+            [(month_names_length, urwid.Text(' ' * month_names_length))] +
             [(2, urwid.AttrMap(urwid.Text(name), 'dayname')) for name in dnames],
             dividechars=1)
         self.walker = CalendarWalker(
             on_date_change, on_press, default_keybindings, firstweekday, weeknumbers,
             get_styles, initial=self._initial)
         self.box = CListBox(self.walker)
         frame = urwid.Frame(self.box, header=dnames)
```

### Comparing `khal-0.9.8/khal/ui/__init__.py` & `khal-0.9.9/khal/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/ui/colors.py` & `khal-0.9.9/khal/ui/colors.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/ui/widgets.py` & `khal-0.9.9/khal/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/ui/base.py` & `khal-0.9.9/khal/ui/base.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal/ui/editor.py` & `khal-0.9.9/khal/ui/editor.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal.conf.sample` & `khal-0.9.9/khal.conf.sample`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/khal.egg-info/SOURCES.txt` & `khal-0.9.9/khal.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 doc/source/news/khal092.rst
 doc/source/news/khal093.rst
 doc/source/news/khal094.rst
 doc/source/news/khal095.rst
 doc/source/news/khal096.rst
 doc/source/news/khal097.rst
 doc/source/news/khal098.rst
+doc/source/news/khal099.rst
 doc/source/ystatic/.gitignore
 doc/source/ytemplates/layout.html
 doc/webpage/src/new_rss_url.rst
 khal/__init__.py
 khal/__main__.py
 khal/calendar_display.py
 khal/cli.py
```

### Comparing `khal-0.9.8/khal.egg-info/PKG-INFO` & `khal-0.9.9/khal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: khal
-Version: 0.9.8
+Version: 0.9.9
 Summary: A standards based terminal calendar
 Home-page: http://lostpackets.de/khal/
 Author: Christian Geier et. al.
 Author-email: khal@lostpackets.de
 License: Expat/MIT
-Description-Content-Type: UNKNOWN
 Description: khal
         ====
         .. image:: https://travis-ci.org/pimutils/khal.svg?branch=master
             :target: https://travis-ci.org/pimutils/khal
         
         .. image:: https://codecov.io/github/pimutils/khal/coverage.svg?branch=master
           :target: https://codecov.io/github/pimutils/khal?branch=master
@@ -113,7 +112,8 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Classifier: Topic :: Communications
+Provides-Extra: proctitle
```

### Comparing `khal-0.9.8/CHANGELOG.rst` & `khal-0.9.9/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project should be documented here.
 For more detailed information have a look at the git log.
 
 Package maintainers and users who have to manually update their installation
 may want to subscribe to `GitHub's tag feed
 <https://github.com/geier/khal/tags.atom>`_.
 
+0.9.9
+=====
+released 2018-05-26
+
+* Dependencies: only dateutil < 2.7 is supported (and always has been)
+
 0.9.8
 =====
 released 2017-10-05
 
 * FIX a bug in ikhal: when editing events and not editing the dates, the end
   time could erroneously be moved to the start time + 1h
```

### Comparing `khal-0.9.8/misc/mutt2khal` & `khal-0.9.9/misc/mutt2khal`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/misc/__khal` & `khal-0.9.9/misc/__khal`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tox.ini` & `khal-0.9.9/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   TRAVIS_REPO_SLUG
 deps =
     codecov
     pytest
     pytest-cov
     pytest-capturelog
     freezegun
-    vdirsyncer
+    vdirsyncer<0.17.0
     pytz201702: pytz==2017.2
     pytz201610: pytz==2016.10
 
 commands =
     py.test --cov khal {posargs}
     codecov -e TOXENV
```

### Comparing `khal-0.9.8/setup.py` & `khal-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 requirements = [
     'click>=3.2',
     'icalendar',
     'urwid',
     'pyxdg',
     'pytz',
-    'python-dateutil',
+    'python-dateutil<=2.6.1',
     'configobj',
     # https://github.com/untitaker/python-atomicwrites/commit/4d12f23227b6a944ab1d99c507a69fdbc7c9ed6d  # noqa
     'atomicwrites>=0.1.7',
     'tzlocal>=1.0',
 ]
 
 test_requirements = [
```

### Comparing `khal-0.9.8/COPYING` & `khal-0.9.9/COPYING`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/install.rst` & `khal-0.9.9/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/images/rss.png` & `khal-0.9.9/doc/source/images/rss.png`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/configspec.rst` & `khal-0.9.9/doc/source/configspec.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/hacking.rst` & `khal-0.9.9/doc/source/hacking.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/index.rst` & `khal-0.9.9/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/feedback.rst` & `khal-0.9.9/doc/source/feedback.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/configure.rst` & `khal-0.9.9/doc/source/configure.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/usage.rst` & `khal-0.9.9/doc/source/usage.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal092.rst` & `khal-0.9.9/doc/source/news/khal092.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal084.rst` & `khal-0.9.9/doc/source/news/khal084.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal02.rst` & `khal-0.9.9/doc/source/news/khal02.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal097.rst` & `khal-0.9.9/doc/source/news/khal097.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal082.rst` & `khal-0.9.9/doc/source/news/khal082.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal031.rst` & `khal-0.9.9/doc/source/news/khal031.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal091.rst` & `khal-0.9.9/doc/source/news/khal091.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal08.rst` & `khal-0.9.9/doc/source/news/khal08.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal07.rst` & `khal-0.9.9/doc/source/news/khal07.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal05.rst` & `khal-0.9.9/doc/source/news/khal05.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal071.rst` & `khal-0.9.9/doc/source/news/khal071.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal093.rst` & `khal-0.9.9/doc/source/news/khal093.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal01.rst` & `khal-0.9.9/doc/source/news/khal01.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal04.rst` & `khal-0.9.9/doc/source/news/khal04.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal03.rst` & `khal-0.9.9/doc/source/news/khal03.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal098.rst` & `khal-0.9.9/doc/source/news/khal098.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/callfortesting.rst` & `khal-0.9.9/doc/source/news/callfortesting.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal09.rst` & `khal-0.9.9/doc/source/news/khal09.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal06.rst` & `khal-0.9.9/doc/source/news/khal06.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news/khal094.rst` & `khal-0.9.9/doc/source/news/khal094.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/faq.rst` & `khal-0.9.9/doc/source/faq.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/license.rst` & `khal-0.9.9/doc/source/license.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/news.rst` & `khal-0.9.9/doc/source/news.rst`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
         :target: https://lostpackets.de/khal/index.rss
 
 .. feed::
     :rss: index.rss
     :title: khal news
     :link: http://lostpackets.de/khal/
 
+    news/khal099
     news/khal098
     news/khal097
     news/khal096
     news/khal095
     news/khal094
     news/khal093
     news/khal092
```

### Comparing `khal-0.9.8/doc/source/conf.py` & `khal-0.9.9/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/source/standards.rst` & `khal-0.9.9/doc/source/standards.rst`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/doc/Makefile` & `khal-0.9.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/ics/cal_lots_of_timezones.ics` & `khal-0.9.9/tests/ics/cal_lots_of_timezones.ics`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/ics/event_rrule_recuid_cancelled.ics` & `khal-0.9.9/tests/ics/event_rrule_recuid_cancelled.ics`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/ics/event_dt_simple_inkl_vtimezone.ics` & `khal-0.9.9/tests/ics/event_dt_simple_inkl_vtimezone.ics`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/ics/event_dt_mixed_awareness.ics` & `khal-0.9.9/tests/ics/event_dt_mixed_awareness.ics`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/ics/mult_uids_and_recuid_no_order.ics` & `khal-0.9.9/tests/ics/mult_uids_and_recuid_no_order.ics`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/ics/cal_dt_two_tz.ics` & `khal-0.9.9/tests/ics/cal_dt_two_tz.ics`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/ics/part1.ics` & `khal-0.9.9/tests/ics/part1.ics`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/ics/part0.ics` & `khal-0.9.9/tests/ics/part0.ics`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/cli_test.py` & `khal-0.9.9/tests/cli_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -677,15 +677,15 @@
     assert 24 == len(result.output.split('\t'))
 
 
 def test_printics_read_from_stdin(runner):
     runner = runner(command='printics')
     result = runner.invoke(main_khal, ['printics'], input=_get_text('cal_d'))
     assert not result.exception
-    assert result.output == '1 events found in stdin input\n An Event\n'
+    assert '1 events found in stdin input\n An Event\n' in result.output
 
 
 def test_configure_command_config_exists(runner):
     runner = runner()
     result = runner.invoke(main_khal, ['configure'], input=choices())
     assert 'Found an existing' in result.output
     assert result.exit_code == 1
```

### Comparing `khal-0.9.8/tests/conftest.py` & `khal-0.9.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/khalendar_test.py` & `khal-0.9.9/tests/khalendar_test.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/controller_test.py` & `khal-0.9.9/tests/controller_test.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/cal_display_test.py` & `khal-0.9.9/tests/cal_display_test.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/khalendar_utils_test.py` & `khal-0.9.9/tests/khalendar_utils_test.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/terminal_test.py` & `khal-0.9.9/tests/terminal_test.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/utils_test.py` & `khal-0.9.9/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/backend_test.py` & `khal-0.9.9/tests/backend_test.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/utils.py` & `khal-0.9.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/event_test.py` & `khal-0.9.9/tests/event_test.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/settings_test.py` & `khal-0.9.9/tests/settings_test.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/vtimezone_test.py` & `khal-0.9.9/tests/vtimezone_test.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/ui/test_editor.py` & `khal-0.9.9/tests/ui/test_editor.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/ui/test_widgets.py` & `khal-0.9.9/tests/ui/test_widgets.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/ui/test_calendarwidget.py` & `khal-0.9.9/tests/ui/test_calendarwidget.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/tests/vdir_test.py` & `khal-0.9.9/tests/vdir_test.py`

 * *Files identical despite different names*

### Comparing `khal-0.9.8/PKG-INFO` & `khal-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: khal
-Version: 0.9.8
+Version: 0.9.9
 Summary: A standards based terminal calendar
 Home-page: http://lostpackets.de/khal/
 Author: Christian Geier et. al.
 Author-email: khal@lostpackets.de
 License: Expat/MIT
-Description-Content-Type: UNKNOWN
 Description: khal
         ====
         .. image:: https://travis-ci.org/pimutils/khal.svg?branch=master
             :target: https://travis-ci.org/pimutils/khal
         
         .. image:: https://codecov.io/github/pimutils/khal/coverage.svg?branch=master
           :target: https://codecov.io/github/pimutils/khal?branch=master
@@ -113,7 +112,8 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Classifier: Topic :: Communications
+Provides-Extra: proctitle
```

