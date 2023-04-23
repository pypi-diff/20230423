# Comparing `tmp/aa-timezones-1.8.0.tar.gz` & `tmp/aa_timezones-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-timezones-1.8.0.tar", last modified: Mon Feb 28 11:15:43 2022, max compression
+gzip compressed data, was "aa_timezones-1.9.0.tar", last modified: Thu Mar  3 01:08:44 2022, max compression
```

## Comparing `aa-timezones-1.8.0.tar` & `aa_timezones-1.9.0.tar`

### file list

```diff
@@ -1,154 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.146108 aa-timezones-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7247 2022-02-28 11:15:43.146108 aa-timezones-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4839 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.134107 aa-timezones-1.8.0/aa_timezones.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7247 2022-02-28 11:15:42.000000 aa-timezones-1.8.0/aa_timezones.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7778 2022-02-28 11:15:43.000000 aa-timezones-1.8.0/aa_timezones.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-28 11:15:42.000000 aa-timezones-1.8.0/aa_timezones.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-02-28 11:15:42.000000 aa-timezones-1.8.0/aa_timezones.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-02-28 11:15:42.000000 aa-timezones-1.8.0/aa_timezones.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-28 11:15:43.146108 aa-timezones-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2500 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.134107 aa-timezones-1.8.0/testauth/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/testauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/testauth/celery.py
--rw-r--r--   0 runner    (1001) docker     (121)     9416 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/testauth/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/testauth/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/testauth/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.134107 aa-timezones-1.8.0/timezones/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1849 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.130107 aa-timezones-1.8.0/timezones/management/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.134107 aa-timezones-1.8.0/timezones/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     3353 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/management/commands/timezones_load_tz_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.134107 aa-timezones-1.8.0/timezones/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     2925 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/migrations/0002_timezonedata_timezones.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/migrations/0003_auto_20201003_1748.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.130107 aa-timezones-1.8.0/timezones/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.130107 aa-timezones-1.8.0/timezones/static/timezones/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.134107 aa-timezones-1.8.0/timezones/static/timezones/css/
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/timezones.css
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/timezones.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.130107 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.138107 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/css/
--rw-r--r--   0 runner    (1001) docker     (121)   152810 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/css/weather-icons-wind.css
--rw-r--r--   0 runner    (1001) docker     (121)   126943 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/css/weather-icons-wind.min.css
--rw-r--r--   0 runner    (1001) docker     (121)    31970 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/css/weather-icons.css
--rw-r--r--   0 runner    (1001) docker     (121)    25872 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/css/weather-icons.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.138107 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/font/
--rwxr-xr-x   0 runner    (1001) docker     (121)    99774 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.eot
--rwxr-xr-x   0 runner    (1001) docker     (121)   184969 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.svg
--rwxr-xr-x   0 runner    (1001) docker     (121)    99564 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.ttf
--rwxr-xr-x   0 runner    (1001) docker     (121)    56468 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.woff
--rwxr-xr-x   0 runner    (1001) docker     (121)    44720 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.138107 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.138107 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-beaufort.less
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-day.less
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-direction.less
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-misc.less
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-moon-aliases.less
--rw-r--r--   0 runner    (1001) docker     (121)     3956 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-moon.less
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-neutral.less
--rw-r--r--   0 runner    (1001) docker     (121)     2574 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-night.less
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-time.less
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-wind-aliases.less
--rw-r--r--   0 runner    (1001) docker     (121)    30270 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-wind-degrees.less
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-wind.less
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.142107 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-variables/
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-beaufort.less
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-day.less
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-direction.less
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-misc.less
--rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-moon.less
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-neutral.less
--rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-night.less
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-time.less
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-wind-names.less
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.142107 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/mappings/
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-forecast-io.less
--rw-r--r--   0 runner    (1001) docker     (121)    19149 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-owm.less
--rw-r--r--   0 runner    (1001) docker     (121)     6536 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-wmo4680.less
--rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-wunderground.less
--rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-yahoo.less
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/weather-icons-classes.less
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/weather-icons-core.less
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/weather-icons-variables.less
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/weather-icons-wind.less
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/weather-icons-wind.min.less
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/weather-icons.less
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/weather-icons.min.less
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.142107 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.142107 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-beaufort.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-day.scss
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-direction.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-misc.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-moon-aliases.scss
--rw-r--r--   0 runner    (1001) docker     (121)     3956 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-moon.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-neutral.scss
--rw-r--r--   0 runner    (1001) docker     (121)     2574 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-night.scss
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-time.scss
--rw-r--r--   0 runner    (1001) docker     (121)     2013 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-wind-aliases.scss
--rw-r--r--   0 runner    (1001) docker     (121)    36108 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-wind-degrees.scss
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-wind.scss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.142107 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-beaufort.scss
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-day.scss
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-direction.scss
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-misc.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-moon.scss
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-neutral.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-night.scss
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-time.scss
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-wind-names.scss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.146108 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/mappings/
--rw-r--r--   0 runner    (1001) docker     (121)     1157 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-forecast-io.scss
--rw-r--r--   0 runner    (1001) docker     (121)    19326 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-owm.scss
--rw-r--r--   0 runner    (1001) docker     (121)     6621 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-wmo4680.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-wunderground.scss
--rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-yahoo.scss
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/weather-icons-classes.scss
--rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/weather-icons-core.scss
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/weather-icons-variables.scss
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/weather-icons-wind.min.scss
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/weather-icons-wind.scss
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/weather-icons.min.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/weather-icons.scss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.146108 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/values/
--rw-r--r--   0 runner    (1001) docker     (121)    31475 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/values/weathericons.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.146108 aa-timezones-1.8.0/timezones/static/timezones/js/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.146108 aa-timezones-1.8.0/timezones/static/timezones/js/moment/
--rw-r--r--   0 runner    (1001) docker     (121)   163718 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/js/moment/moment-timezone-with-data-1970-2030.js
--rw-r--r--   0 runner    (1001) docker     (121)   144023 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/js/moment/moment-timezone-with-data-1970-2030.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.146108 aa-timezones-1.8.0/timezones/static/timezones/js/timeago/
--rw-r--r--   0 runner    (1001) docker     (121)     8503 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/js/timeago/jquery.timeago.js
--rw-r--r--   0 runner    (1001) docker     (121)     4765 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/js/timeago/jquery.timeago.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     6915 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/js/timezones.js
--rw-r--r--   0 runner    (1001) docker     (121)     4248 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/static/timezones/js/timezones.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.134107 aa-timezones-1.8.0/timezones/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.146108 aa-timezones-1.8.0/timezones/templates/timezones/
--rw-r--r--   0 runner    (1001) docker     (121)    13969 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/templates/timezones/adjust-time.html
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/templates/timezones/base.html
--rw-r--r--   0 runner    (1001) docker     (121)     4121 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/templates/timezones/index.html
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/templates/timezones/time-until.html
--rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/templates/timezones/timezone-panel.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.146108 aa-timezones-1.8.0/timezones/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/templatetags/timezones_versioned_static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 11:15:43.146108 aa-timezones-1.8.0/timezones/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/tests/test_access.py
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/tests/test_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-02-28 11:15:35.000000 aa-timezones-1.8.0/timezones/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.806945 aa_timezones-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6232 2022-03-03 01:08:44.810945 aa_timezones-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4839 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.786945 aa_timezones-1.9.0/aa_timezones.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6232 2022-03-03 01:08:44.000000 aa_timezones-1.9.0/aa_timezones.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7734 2022-03-03 01:08:44.000000 aa_timezones-1.9.0/aa_timezones.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-03 01:08:44.000000 aa_timezones-1.9.0/aa_timezones.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-03 01:08:43.000000 aa_timezones-1.9.0/aa_timezones.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-03-03 01:08:44.000000 aa_timezones-1.9.0/aa_timezones.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-03-03 01:08:44.000000 aa_timezones-1.9.0/aa_timezones.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-03-03 01:08:44.810945 aa_timezones-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.786945 aa_timezones-1.9.0/timezones/
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1849 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.782945 aa_timezones-1.9.0/timezones/management/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.786945 aa_timezones-1.9.0/timezones/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)     3353 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/management/commands/timezones_load_tz_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.790945 aa_timezones-1.9.0/timezones/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)      802 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2925 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/migrations/0002_timezonedata_timezones.py
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/migrations/0003_auto_20201003_1748.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2125 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.782945 aa_timezones-1.9.0/timezones/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.786945 aa_timezones-1.9.0/timezones/static/timezones/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.790945 aa_timezones-1.9.0/timezones/static/timezones/css/
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/timezones.css
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/timezones.min.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.786945 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.790945 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/css/
+-rw-r--r--   0 runner    (1001) docker     (121)   152810 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/css/weather-icons-wind.css
+-rw-r--r--   0 runner    (1001) docker     (121)   126943 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/css/weather-icons-wind.min.css
+-rw-r--r--   0 runner    (1001) docker     (121)    31970 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/css/weather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (121)    25872 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/css/weather-icons.min.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.794946 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/font/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    99774 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.eot
+-rwxr-xr-x   0 runner    (1001) docker     (121)   184969 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.svg
+-rwxr-xr-x   0 runner    (1001) docker     (121)    99564 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (121)    56468 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.woff
+-rwxr-xr-x   0 runner    (1001) docker     (121)    44720 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.794946 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.798946 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-beaufort.less
+-rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-day.less
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-direction.less
+-rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-misc.less
+-rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-moon-aliases.less
+-rw-r--r--   0 runner    (1001) docker     (121)     3956 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-moon.less
+-rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-neutral.less
+-rw-r--r--   0 runner    (1001) docker     (121)     2574 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-night.less
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-time.less
+-rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-wind-aliases.less
+-rw-r--r--   0 runner    (1001) docker     (121)    30270 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-wind-degrees.less
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-wind.less
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.798946 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-variables/
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-beaufort.less
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-day.less
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-direction.less
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-misc.less
+-rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-moon.less
+-rw-r--r--   0 runner    (1001) docker     (121)      814 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-neutral.less
+-rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-night.less
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-time.less
+-rw-r--r--   0 runner    (1001) docker     (121)      456 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-wind-names.less
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.802945 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/mappings/
+-rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-forecast-io.less
+-rw-r--r--   0 runner    (1001) docker     (121)    19149 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-owm.less
+-rw-r--r--   0 runner    (1001) docker     (121)     6536 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-wmo4680.less
+-rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-wunderground.less
+-rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-yahoo.less
+-rw-r--r--   0 runner    (1001) docker     (121)      398 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/weather-icons-classes.less
+-rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/weather-icons-core.less
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/weather-icons-variables.less
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/weather-icons-wind.less
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/weather-icons-wind.min.less
+-rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/weather-icons.less
+-rw-r--r--   0 runner    (1001) docker     (121)      894 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/weather-icons.min.less
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.802945 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.802945 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-beaufort.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-day.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-direction.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-misc.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-moon-aliases.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     3956 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-moon.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-neutral.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     2574 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-night.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-time.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     2013 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-wind-aliases.scss
+-rw-r--r--   0 runner    (1001) docker     (121)    36108 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-wind-degrees.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      322 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-wind.scss
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.806945 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-beaufort.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-day.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-direction.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-misc.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-moon.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      814 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-neutral.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-night.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-time.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      456 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-wind-names.scss
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.806945 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/mappings/
+-rw-r--r--   0 runner    (1001) docker     (121)     1157 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-forecast-io.scss
+-rw-r--r--   0 runner    (1001) docker     (121)    19326 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-owm.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     6621 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-wmo4680.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-wunderground.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-yahoo.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      398 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/weather-icons-classes.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/weather-icons-core.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/weather-icons-variables.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/weather-icons-wind.min.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/weather-icons-wind.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/weather-icons.min.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/weather-icons.scss
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.806945 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/values/
+-rw-r--r--   0 runner    (1001) docker     (121)    31475 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/values/weathericons.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.806945 aa_timezones-1.9.0/timezones/static/timezones/js/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.806945 aa_timezones-1.9.0/timezones/static/timezones/js/moment/
+-rw-r--r--   0 runner    (1001) docker     (121)   163718 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/js/moment/moment-timezone-with-data-1970-2030.js
+-rw-r--r--   0 runner    (1001) docker     (121)   144023 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/js/moment/moment-timezone-with-data-1970-2030.min.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.806945 aa_timezones-1.9.0/timezones/static/timezones/js/timeago/
+-rw-r--r--   0 runner    (1001) docker     (121)     8503 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/js/timeago/jquery.timeago.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4765 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/js/timeago/jquery.timeago.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)     6915 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/js/timezones.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4248 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/static/timezones/js/timezones.min.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.786945 aa_timezones-1.9.0/timezones/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.806945 aa_timezones-1.9.0/timezones/templates/timezones/
+-rw-r--r--   0 runner    (1001) docker     (121)    13969 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/templates/timezones/adjust-time.html
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/templates/timezones/base.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4121 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/templates/timezones/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/templates/timezones/time-until.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/templates/timezones/timezone-panel.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.806945 aa_timezones-1.9.0/timezones/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      512 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/templatetags/timezones_versioned_static.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 01:08:44.806945 aa_timezones-1.9.0/timezones/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/tests/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (121)      736 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/tests/test_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)      843 2022-03-03 01:08:27.000000 aa_timezones-1.9.0/timezones/views.py
```

### Comparing `aa-timezones-1.8.0/LICENSE` & `aa_timezones-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/PKG-INFO` & `aa_timezones-1.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,159 +1,164 @@
 Metadata-Version: 2.1
-Name: aa-timezones
-Version: 1.8.0
+Name: aa_timezones
+Version: 1.9.0
 Summary: Time Zones Overview for Alliance Auth
 Home-page: https://github.com/ppfeufer/aa-timezones
 Author: Peter Pfeufer
 Author-email: development@ppfeufer.de
-License: GPLv3
+Maintainer: Peter Pfeufer
+Maintainer-email: development@ppfeufer.de
+License: GPL-3.0
 Project-URL: Issue / Bug Reports, https://github.com/ppfeufer/aa-timezones/issues
 Project-URL: Changelog, https://github.com/ppfeufer/aa-timezones/blob/master/CHANGELOG.md
-Project-URL: Release Notes, https://github.com/ppfeufer/aa-timezones/releases/tag/v1.8.0
-Project-URL: Git Repository, https://github.com/ppfeufer/aa-timezones
-Description: # AA Time Zones
-        
-        [![Version](https://img.shields.io/pypi/v/aa-timezones?label=release)](https://pypi.org/project/aa-timezones/)
-        [![License](https://img.shields.io/github/license/ppfeufer/aa-timezones)](https://github.com/ppfeufer/aa-timezones/blob/master/LICENSE)
-        [![Python](https://img.shields.io/pypi/pyversions/aa-timezones)](https://pypi.org/project/aa-timezones/)
-        [![Django](https://img.shields.io/pypi/djversions/aa-timezones?label=django)](https://pypi.org/project/aa-timezones/)
-        ![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
-        [![Code Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](http://black.readthedocs.io/en/latest/)
-        [![Discord](https://img.shields.io/discord/790364535294132234?label=discord)](https://discord.gg/zmh52wnfvM)
-        [![Checks](https://github.com/ppfeufer/aa-timezones/actions/workflows/automated-checks.yml/badge.svg)](https://github.com/ppfeufer/aa-timezones/actions/workflows/automated-checks.yml)
-        [![codecov](https://codecov.io/gh/ppfeufer/aa-timezones/branch/master/graph/badge.svg?token=ZSRTW5FR4C)](https://codecov.io/gh/ppfeufer/aa-timezones)
-        [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/ppfeufer/aa-timezones/blob/master/CODE_OF_CONDUCT.md)
-        
-        
-        App for displaying different time zones with Alliance Auth
-        
-        ![Time Zones](https://raw.githubusercontent.com/ppfeufer/aa-timezones/master/timezones/docs/time-zones.jpg)
-        
-        
-        ## Contents
-        
-        - [Installation](#installation)
-        - [Updating](#updating)
-        - [Configure Timezone Panels](#configure-timezone-panels)
-        - [Adjusting Time](#adjusting-time)
-        - [Change Log](CHANGELOG.md)
-        
-        
-        ## Installation
-        
-        **Important**: This app is a plugin for Alliance Auth.
-        If you don't have Alliance Auth running already, please install it first before proceeding.
-        (see the official [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html)
-        for details)
-        
-        
-        ### Step 1 - Install app
-        
-        Make sure you are in the virtual environment (venv) of your Alliance Auth installation.
-        Then install the latest version:
-        
-        ```bash
-        pip install aa-timezones
-        ```
-        
-        
-        ### Step 2 - Update your AA settings
-        
-        Configure your AA settings (`local.py`) as follows:
-        
-        - Add `'timezones',` to `INSTALLED_APPS`
-        
-        
-        ### Step 3 - Finalize the installation
-        
-        Run migrations & copy static files
-        
-        ```bash
-        python manage.py collectstatic
-        python manage.py migrate
-        ```
-        
-        Restart your supervisor services for AA
-        
-        Once done, it's time to add all the time zone informations, so you can define your
-        own set of panels later. To do so, simply run:
-        
-        ```bash
-        python manage.py timezones_load_tz_data
-        ```
-        
-        
-        ### Step 4 - Setup permissions
-        
-        Now you can setup permissions in Alliance Auth for your users.
-        Add ``timezones|aa timezones|Can access ths app`` to the states and/or groups you would
-        like to have access.
-        
-        
-        ## Updating
-        
-        To update your existing installation of AA Time Zones first enable your virtual environment.
-        
-        Then run the following commands from your AA project directory (the one that contains `manage.py`).
-        
-        ```bash
-        pip install -U aa-timezones
-        ```
-        
-        ```bash
-        python manage.py collectstatic
-        ```
-        
-        ```bash
-        python manage.py migrate
-        ```
-        
-        Now restart your AA supervisor services.
-        
-        
-        ## Configure Timezone Panels
-        Per default there are 10 additional time zone panels that are displayed (see first image).
-        If you want to change those, you can create your own set of panels in your admin backend.
-        
-        **NOTE:** "Local Time" and "EVE Time" will always be displayed as the first two panels,
-        no matter what.
-        
-        
-        ## Adjusting Time
-        
-        You can easiely adjust the time that is displayed for all timezones.
-        This is useful for reinforcement timers or pre-planned fleets. To do so,
-        click on the "Adjust Time" button below the time zone panels and you will see 2 different ways to set a new time.
-        
-        ![Adjusting Time](https://raw.githubusercontent.com/ppfeufer/aa-timezones/master/timezones/docs/adjust-time.jpg)
-        
-        The first one is meant for timers, like reinforcement timers, anchoring timers or the like.
-        It's maximum is 7 day, 59 minutes and 59 seconds into the future. That should cover pretty much all
-        timers you can find in Eve Online.
-        
-        The second one is best suited for pre-planned fleets. Here you can set a fixed date and time based
-        on the selected time zone. The default selected time zone is "EVE Time" but you can change it
-        to all the available options. Keep in mind, the selected time zone is the one the time and date will be adjusted to.
-        So if you are going to use it to plan fleets it is recommanded to keep this set to "EVE Time".
-        
-        To set the adjusted time, simply click on "Set Time" in the row you altered. This will than adjust all
-        time zone panels to the time you selected and will also alter the link in your browser, so you can share it
-        with others directly.
-        
+Keywords: allianceauth,eveonline,time,timezones
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# AA Time Zones
+
+[![Version](https://img.shields.io/pypi/v/aa-timezones?label=release)](https://pypi.org/project/aa-timezones/)
+[![License](https://img.shields.io/github/license/ppfeufer/aa-timezones)](https://github.com/ppfeufer/aa-timezones/blob/master/LICENSE)
+[![Python](https://img.shields.io/pypi/pyversions/aa-timezones)](https://pypi.org/project/aa-timezones/)
+[![Django](https://img.shields.io/pypi/djversions/aa-timezones?label=django)](https://pypi.org/project/aa-timezones/)
+![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
+[![Code Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](http://black.readthedocs.io/en/latest/)
+[![Discord](https://img.shields.io/discord/790364535294132234?label=discord)](https://discord.gg/zmh52wnfvM)
+[![Checks](https://github.com/ppfeufer/aa-timezones/actions/workflows/automated-checks.yml/badge.svg)](https://github.com/ppfeufer/aa-timezones/actions/workflows/automated-checks.yml)
+[![codecov](https://codecov.io/gh/ppfeufer/aa-timezones/branch/master/graph/badge.svg?token=ZSRTW5FR4C)](https://codecov.io/gh/ppfeufer/aa-timezones)
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/ppfeufer/aa-timezones/blob/master/CODE_OF_CONDUCT.md)
+
+
+App for displaying different time zones with Alliance Auth
+
+![Time Zones](https://raw.githubusercontent.com/ppfeufer/aa-timezones/master/timezones/docs/time-zones.jpg)
+
+
+## Contents
+
+- [Installation](#installation)
+- [Updating](#updating)
+- [Configure Timezone Panels](#configure-timezone-panels)
+- [Adjusting Time](#adjusting-time)
+- [Change Log](CHANGELOG.md)
+
+
+## Installation
+
+**Important**: This app is a plugin for Alliance Auth.
+If you don't have Alliance Auth running already, please install it first before proceeding.
+(see the official [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html)
+for details)
+
+
+### Step 1 - Install app
+
+Make sure you are in the virtual environment (venv) of your Alliance Auth installation.
+Then install the latest version:
+
+```bash
+pip install aa-timezones
+```
+
+
+### Step 2 - Update your AA settings
+
+Configure your AA settings (`local.py`) as follows:
+
+- Add `'timezones',` to `INSTALLED_APPS`
+
+
+### Step 3 - Finalize the installation
+
+Run migrations & copy static files
+
+```bash
+python manage.py collectstatic
+python manage.py migrate
+```
+
+Restart your supervisor services for AA
+
+Once done, it's time to add all the time zone informations, so you can define your
+own set of panels later. To do so, simply run:
+
+```bash
+python manage.py timezones_load_tz_data
+```
+
+
+### Step 4 - Setup permissions
+
+Now you can setup permissions in Alliance Auth for your users.
+Add ``timezones|aa timezones|Can access ths app`` to the states and/or groups you would
+like to have access.
+
+
+## Updating
+
+To update your existing installation of AA Time Zones first enable your virtual environment.
+
+Then run the following commands from your AA project directory (the one that contains `manage.py`).
+
+```bash
+pip install -U aa-timezones
+```
+
+```bash
+python manage.py collectstatic
+```
+
+```bash
+python manage.py migrate
+```
+
+Now restart your AA supervisor services.
+
+
+## Configure Timezone Panels
+Per default there are 10 additional time zone panels that are displayed (see first image).
+If you want to change those, you can create your own set of panels in your admin backend.
+
+**NOTE:** "Local Time" and "EVE Time" will always be displayed as the first two panels,
+no matter what.
+
+
+## Adjusting Time
+
+You can easiely adjust the time that is displayed for all timezones.
+This is useful for reinforcement timers or pre-planned fleets. To do so,
+click on the "Adjust Time" button below the time zone panels and you will see 2 different ways to set a new time.
+
+![Adjusting Time](https://raw.githubusercontent.com/ppfeufer/aa-timezones/master/timezones/docs/adjust-time.jpg)
+
+The first one is meant for timers, like reinforcement timers, anchoring timers or the like.
+It's maximum is 7 day, 59 minutes and 59 seconds into the future. That should cover pretty much all
+timers you can find in Eve Online.
+
+The second one is best suited for pre-planned fleets. Here you can set a fixed date and time based
+on the selected time zone. The default selected time zone is "EVE Time" but you can change it
+to all the available options. Keep in mind, the selected time zone is the one the time and date will be adjusted to.
+So if you are going to use it to plan fleets it is recommanded to keep this set to "EVE Time".
+
+To set the adjusted time, simply click on "Set Time" in the row you altered. This will than adjust all
+time zone panels to the time you selected and will also alter the link in your browser, so you can share it
+with others directly.
+
+
```

### Comparing `aa-timezones-1.8.0/README.md` & `aa_timezones-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/aa_timezones.egg-info/PKG-INFO` & `aa_timezones-1.9.0/aa_timezones.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,159 +1,164 @@
 Metadata-Version: 2.1
 Name: aa-timezones
-Version: 1.8.0
+Version: 1.9.0
 Summary: Time Zones Overview for Alliance Auth
 Home-page: https://github.com/ppfeufer/aa-timezones
 Author: Peter Pfeufer
 Author-email: development@ppfeufer.de
-License: GPLv3
+Maintainer: Peter Pfeufer
+Maintainer-email: development@ppfeufer.de
+License: GPL-3.0
 Project-URL: Issue / Bug Reports, https://github.com/ppfeufer/aa-timezones/issues
 Project-URL: Changelog, https://github.com/ppfeufer/aa-timezones/blob/master/CHANGELOG.md
-Project-URL: Release Notes, https://github.com/ppfeufer/aa-timezones/releases/tag/v1.8.0
-Project-URL: Git Repository, https://github.com/ppfeufer/aa-timezones
-Description: # AA Time Zones
-        
-        [![Version](https://img.shields.io/pypi/v/aa-timezones?label=release)](https://pypi.org/project/aa-timezones/)
-        [![License](https://img.shields.io/github/license/ppfeufer/aa-timezones)](https://github.com/ppfeufer/aa-timezones/blob/master/LICENSE)
-        [![Python](https://img.shields.io/pypi/pyversions/aa-timezones)](https://pypi.org/project/aa-timezones/)
-        [![Django](https://img.shields.io/pypi/djversions/aa-timezones?label=django)](https://pypi.org/project/aa-timezones/)
-        ![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
-        [![Code Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](http://black.readthedocs.io/en/latest/)
-        [![Discord](https://img.shields.io/discord/790364535294132234?label=discord)](https://discord.gg/zmh52wnfvM)
-        [![Checks](https://github.com/ppfeufer/aa-timezones/actions/workflows/automated-checks.yml/badge.svg)](https://github.com/ppfeufer/aa-timezones/actions/workflows/automated-checks.yml)
-        [![codecov](https://codecov.io/gh/ppfeufer/aa-timezones/branch/master/graph/badge.svg?token=ZSRTW5FR4C)](https://codecov.io/gh/ppfeufer/aa-timezones)
-        [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/ppfeufer/aa-timezones/blob/master/CODE_OF_CONDUCT.md)
-        
-        
-        App for displaying different time zones with Alliance Auth
-        
-        ![Time Zones](https://raw.githubusercontent.com/ppfeufer/aa-timezones/master/timezones/docs/time-zones.jpg)
-        
-        
-        ## Contents
-        
-        - [Installation](#installation)
-        - [Updating](#updating)
-        - [Configure Timezone Panels](#configure-timezone-panels)
-        - [Adjusting Time](#adjusting-time)
-        - [Change Log](CHANGELOG.md)
-        
-        
-        ## Installation
-        
-        **Important**: This app is a plugin for Alliance Auth.
-        If you don't have Alliance Auth running already, please install it first before proceeding.
-        (see the official [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html)
-        for details)
-        
-        
-        ### Step 1 - Install app
-        
-        Make sure you are in the virtual environment (venv) of your Alliance Auth installation.
-        Then install the latest version:
-        
-        ```bash
-        pip install aa-timezones
-        ```
-        
-        
-        ### Step 2 - Update your AA settings
-        
-        Configure your AA settings (`local.py`) as follows:
-        
-        - Add `'timezones',` to `INSTALLED_APPS`
-        
-        
-        ### Step 3 - Finalize the installation
-        
-        Run migrations & copy static files
-        
-        ```bash
-        python manage.py collectstatic
-        python manage.py migrate
-        ```
-        
-        Restart your supervisor services for AA
-        
-        Once done, it's time to add all the time zone informations, so you can define your
-        own set of panels later. To do so, simply run:
-        
-        ```bash
-        python manage.py timezones_load_tz_data
-        ```
-        
-        
-        ### Step 4 - Setup permissions
-        
-        Now you can setup permissions in Alliance Auth for your users.
-        Add ``timezones|aa timezones|Can access ths app`` to the states and/or groups you would
-        like to have access.
-        
-        
-        ## Updating
-        
-        To update your existing installation of AA Time Zones first enable your virtual environment.
-        
-        Then run the following commands from your AA project directory (the one that contains `manage.py`).
-        
-        ```bash
-        pip install -U aa-timezones
-        ```
-        
-        ```bash
-        python manage.py collectstatic
-        ```
-        
-        ```bash
-        python manage.py migrate
-        ```
-        
-        Now restart your AA supervisor services.
-        
-        
-        ## Configure Timezone Panels
-        Per default there are 10 additional time zone panels that are displayed (see first image).
-        If you want to change those, you can create your own set of panels in your admin backend.
-        
-        **NOTE:** "Local Time" and "EVE Time" will always be displayed as the first two panels,
-        no matter what.
-        
-        
-        ## Adjusting Time
-        
-        You can easiely adjust the time that is displayed for all timezones.
-        This is useful for reinforcement timers or pre-planned fleets. To do so,
-        click on the "Adjust Time" button below the time zone panels and you will see 2 different ways to set a new time.
-        
-        ![Adjusting Time](https://raw.githubusercontent.com/ppfeufer/aa-timezones/master/timezones/docs/adjust-time.jpg)
-        
-        The first one is meant for timers, like reinforcement timers, anchoring timers or the like.
-        It's maximum is 7 day, 59 minutes and 59 seconds into the future. That should cover pretty much all
-        timers you can find in Eve Online.
-        
-        The second one is best suited for pre-planned fleets. Here you can set a fixed date and time based
-        on the selected time zone. The default selected time zone is "EVE Time" but you can change it
-        to all the available options. Keep in mind, the selected time zone is the one the time and date will be adjusted to.
-        So if you are going to use it to plan fleets it is recommanded to keep this set to "EVE Time".
-        
-        To set the adjusted time, simply click on "Set Time" in the row you altered. This will than adjust all
-        time zone panels to the time you selected and will also alter the link in your browser, so you can share it
-        with others directly.
-        
+Keywords: allianceauth,eveonline,time,timezones
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# AA Time Zones
+
+[![Version](https://img.shields.io/pypi/v/aa-timezones?label=release)](https://pypi.org/project/aa-timezones/)
+[![License](https://img.shields.io/github/license/ppfeufer/aa-timezones)](https://github.com/ppfeufer/aa-timezones/blob/master/LICENSE)
+[![Python](https://img.shields.io/pypi/pyversions/aa-timezones)](https://pypi.org/project/aa-timezones/)
+[![Django](https://img.shields.io/pypi/djversions/aa-timezones?label=django)](https://pypi.org/project/aa-timezones/)
+![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
+[![Code Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](http://black.readthedocs.io/en/latest/)
+[![Discord](https://img.shields.io/discord/790364535294132234?label=discord)](https://discord.gg/zmh52wnfvM)
+[![Checks](https://github.com/ppfeufer/aa-timezones/actions/workflows/automated-checks.yml/badge.svg)](https://github.com/ppfeufer/aa-timezones/actions/workflows/automated-checks.yml)
+[![codecov](https://codecov.io/gh/ppfeufer/aa-timezones/branch/master/graph/badge.svg?token=ZSRTW5FR4C)](https://codecov.io/gh/ppfeufer/aa-timezones)
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/ppfeufer/aa-timezones/blob/master/CODE_OF_CONDUCT.md)
+
+
+App for displaying different time zones with Alliance Auth
+
+![Time Zones](https://raw.githubusercontent.com/ppfeufer/aa-timezones/master/timezones/docs/time-zones.jpg)
+
+
+## Contents
+
+- [Installation](#installation)
+- [Updating](#updating)
+- [Configure Timezone Panels](#configure-timezone-panels)
+- [Adjusting Time](#adjusting-time)
+- [Change Log](CHANGELOG.md)
+
+
+## Installation
+
+**Important**: This app is a plugin for Alliance Auth.
+If you don't have Alliance Auth running already, please install it first before proceeding.
+(see the official [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html)
+for details)
+
+
+### Step 1 - Install app
+
+Make sure you are in the virtual environment (venv) of your Alliance Auth installation.
+Then install the latest version:
+
+```bash
+pip install aa-timezones
+```
+
+
+### Step 2 - Update your AA settings
+
+Configure your AA settings (`local.py`) as follows:
+
+- Add `'timezones',` to `INSTALLED_APPS`
+
+
+### Step 3 - Finalize the installation
+
+Run migrations & copy static files
+
+```bash
+python manage.py collectstatic
+python manage.py migrate
+```
+
+Restart your supervisor services for AA
+
+Once done, it's time to add all the time zone informations, so you can define your
+own set of panels later. To do so, simply run:
+
+```bash
+python manage.py timezones_load_tz_data
+```
+
+
+### Step 4 - Setup permissions
+
+Now you can setup permissions in Alliance Auth for your users.
+Add ``timezones|aa timezones|Can access ths app`` to the states and/or groups you would
+like to have access.
+
+
+## Updating
+
+To update your existing installation of AA Time Zones first enable your virtual environment.
+
+Then run the following commands from your AA project directory (the one that contains `manage.py`).
+
+```bash
+pip install -U aa-timezones
+```
+
+```bash
+python manage.py collectstatic
+```
+
+```bash
+python manage.py migrate
+```
+
+Now restart your AA supervisor services.
+
+
+## Configure Timezone Panels
+Per default there are 10 additional time zone panels that are displayed (see first image).
+If you want to change those, you can create your own set of panels in your admin backend.
+
+**NOTE:** "Local Time" and "EVE Time" will always be displayed as the first two panels,
+no matter what.
+
+
+## Adjusting Time
+
+You can easiely adjust the time that is displayed for all timezones.
+This is useful for reinforcement timers or pre-planned fleets. To do so,
+click on the "Adjust Time" button below the time zone panels and you will see 2 different ways to set a new time.
+
+![Adjusting Time](https://raw.githubusercontent.com/ppfeufer/aa-timezones/master/timezones/docs/adjust-time.jpg)
+
+The first one is meant for timers, like reinforcement timers, anchoring timers or the like.
+It's maximum is 7 day, 59 minutes and 59 seconds into the future. That should cover pretty much all
+timers you can find in Eve Online.
+
+The second one is best suited for pre-planned fleets. Here you can set a fixed date and time based
+on the selected time zone. The default selected time zone is "EVE Time" but you can change it
+to all the available options. Keep in mind, the selected time zone is the one the time and date will be adjusted to.
+So if you are going to use it to plan fleets it is recommanded to keep this set to "EVE Time".
+
+To set the adjusted time, simply click on "Set Time" in the row you altered. This will than adjust all
+time zone panels to the time you selected and will also alter the link in your browser, so you can share it
+with others directly.
+
+
```

### Comparing `aa-timezones-1.8.0/aa_timezones.egg-info/SOURCES.txt` & `aa_timezones-1.9.0/aa_timezones.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
+setup.cfg
 aa_timezones.egg-info/PKG-INFO
 aa_timezones.egg-info/SOURCES.txt
 aa_timezones.egg-info/dependency_links.txt
+aa_timezones.egg-info/not-zip-safe
 aa_timezones.egg-info/requires.txt
 aa_timezones.egg-info/top_level.txt
-testauth/__init__.py
-testauth/celery.py
-testauth/settings.py
-testauth/urls.py
-testauth/wsgi.py
 timezones/__init__.py
 timezones/admin.py
 timezones/apps.py
 timezones/auth_hooks.py
 timezones/constants.py
 timezones/models.py
 timezones/urls.py
```

### Comparing `aa-timezones-1.8.0/timezones/admin.py` & `aa_timezones-1.9.0/timezones/admin.py`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/auth_hooks.py` & `aa_timezones-1.9.0/timezones/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/constants.py` & `aa_timezones-1.9.0/timezones/constants.py`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/management/commands/timezones_load_tz_data.py` & `aa_timezones-1.9.0/timezones/management/commands/timezones_load_tz_data.py`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/migrations/0001_initial.py` & `aa_timezones-1.9.0/timezones/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/migrations/0002_timezonedata_timezones.py` & `aa_timezones-1.9.0/timezones/migrations/0002_timezonedata_timezones.py`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/models.py` & `aa_timezones-1.9.0/timezones/models.py`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/css/weather-icons-wind.css` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/css/weather-icons-wind.css`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/css/weather-icons-wind.min.css` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/css/weather-icons-wind.min.css`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/css/weather-icons.css` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/css/weather-icons.css`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/css/weather-icons.min.css` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/css/weather-icons.min.css`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.eot` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.svg` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.ttf` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.woff` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.woff2` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/font/weathericons-regular-webfont.woff2`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-beaufort.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-beaufort.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-day.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-day.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-misc.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-misc.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-moon-aliases.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-moon-aliases.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-moon.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-moon.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-neutral.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-neutral.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-night.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-night.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-wind-aliases.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-wind-aliases.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-wind-degrees.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-classes/classes-wind-degrees.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-day.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-day.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-moon.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-moon.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-neutral.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-neutral.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-night.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/icon-variables/variables-night.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-forecast-io.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-forecast-io.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-owm.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-owm.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-wmo4680.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-wmo4680.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-wunderground.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-wunderground.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-yahoo.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/mappings/wi-yahoo.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/weather-icons-core.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/weather-icons-core.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/weather-icons.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/weather-icons.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/less/weather-icons.min.less` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/less/weather-icons.min.less`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-beaufort.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-beaufort.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-day.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-day.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-misc.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-misc.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-moon-aliases.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-moon-aliases.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-moon.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-moon.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-neutral.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-neutral.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-night.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-night.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-wind-aliases.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-wind-aliases.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-wind-degrees.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-classes/classes-wind-degrees.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-day.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-day.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-moon.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-moon.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-neutral.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-neutral.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-night.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/icon-variables/variables-night.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-forecast-io.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-forecast-io.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-owm.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-owm.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-wmo4680.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-wmo4680.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-wunderground.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-wunderground.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-yahoo.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/mappings/wi-yahoo.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/weather-icons-core.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/weather-icons-core.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/weather-icons.min.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/weather-icons.min.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/sass/weather-icons.scss` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/sass/weather-icons.scss`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/css/weather-icons/values/weathericons.xml` & `aa_timezones-1.9.0/timezones/static/timezones/css/weather-icons/values/weathericons.xml`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/js/moment/moment-timezone-with-data-1970-2030.js` & `aa_timezones-1.9.0/timezones/static/timezones/js/moment/moment-timezone-with-data-1970-2030.js`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/js/moment/moment-timezone-with-data-1970-2030.min.js` & `aa_timezones-1.9.0/timezones/static/timezones/js/moment/moment-timezone-with-data-1970-2030.min.js`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/js/timeago/jquery.timeago.js` & `aa_timezones-1.9.0/timezones/static/timezones/js/timeago/jquery.timeago.js`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/js/timeago/jquery.timeago.min.js` & `aa_timezones-1.9.0/timezones/static/timezones/js/timeago/jquery.timeago.min.js`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/js/timezones.js` & `aa_timezones-1.9.0/timezones/static/timezones/js/timezones.js`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/static/timezones/js/timezones.min.js` & `aa_timezones-1.9.0/timezones/static/timezones/js/timezones.min.js`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/templates/timezones/adjust-time.html` & `aa_timezones-1.9.0/timezones/templates/timezones/adjust-time.html`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/templates/timezones/index.html` & `aa_timezones-1.9.0/timezones/templates/timezones/index.html`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/templates/timezones/timezone-panel.html` & `aa_timezones-1.9.0/timezones/templates/timezones/timezone-panel.html`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/templatetags/timezones_versioned_static.py` & `aa_timezones-1.9.0/timezones/templatetags/timezones_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/tests/test_access.py` & `aa_timezones-1.9.0/timezones/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/tests/test_templatetags.py` & `aa_timezones-1.9.0/timezones/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/tests/test_view.py` & `aa_timezones-1.9.0/timezones/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/tests/utils.py` & `aa_timezones-1.9.0/timezones/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa-timezones-1.8.0/timezones/views.py` & `aa_timezones-1.9.0/timezones/views.py`

 * *Files identical despite different names*

