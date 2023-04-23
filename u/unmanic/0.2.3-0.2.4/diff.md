# Comparing `tmp/unmanic-0.2.3.tar.gz` & `tmp/unmanic-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unmanic-0.2.3.tar", last modified: Sat Jun  4 23:31:17 2022, max compression
+gzip compressed data, was "dist/unmanic-0.2.4.tar", last modified: Sun Apr 23 04:53:50 2023, max compression
```

## Comparing `unmanic-0.2.3.tar` & `unmanic-0.2.4.tar`

### file list

```diff
@@ -1,299 +1,306 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)    27920 2022-06-04 23:30:46.000000 unmanic-0.2.3/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     6766 2022-06-04 23:30:46.000000 unmanic-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    13036 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/api_v1/
--rw-r--r--   0 runner    (1001) docker     (121)     6476 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v1/history_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     5464 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v1/filebrowser_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7160 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v1/pending_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6005 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v1/session_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3733 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v1/base_api_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     8936 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v1/plugins_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6521 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     3006 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_request_router.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/api_v2/
--rw-r--r--   0 runner    (1001) docker     (121)    14004 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/history_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     7098 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/docs_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     5098 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/filebrowser_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30798 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/pending_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6840 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/session_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    10995 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/base_api_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)    17949 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/workers_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    46051 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/plugins_api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/api_v2/schema/
--rw-r--r--   0 runner    (1001) docker     (121)    41395 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/schema/schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3188 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/schema/unmanic.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4064 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/schema/swagger.py
--rw-r--r--   0 runner    (1001) docker     (121)    50039 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/settings_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     8980 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/upload_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     4275 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/api_v2/version_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2148 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     2655 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/docs/privacy_policy.md
--rw-r--r--   0 runner    (1001) docker     (121)   125703 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/docs/api_schema_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   249479 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/docs/api_schema_v2.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/frontend/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)      712 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/scripts/translate.sh
--rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/.eslintrc.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/frontend/public/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/frontend/public/icons/
--rw-r--r--   0 runner    (1001) docker     (121)    12280 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/public/icons/favicon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/public/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (121)     3603 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/public/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (121)     9370 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/public/icons/favicon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (121)     1406 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)   765115 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/.eslintignore
--rw-r--r--   0 runner    (1001) docker     (121)     7429 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/quasar.conf.js
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/package.json
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/babel.config.js
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/.postcssrc.js
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/jsconfig.json
--rwxr-xr-x   0 runner    (1001) docker     (121)     1474 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/css/
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/css/markdown-admonitions.css
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/css/quasar.variables.scss
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/css/app.scss
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/App.vue
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/pages/
--rw-r--r--   0 runner    (1001) docker     (121)    23846 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/pages/SettingsLink.vue
--rw-r--r--   0 runner    (1001) docker     (121)     3085 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/pages/DataPanels.vue
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/pages/SettingsPlugins.vue
--rw-r--r--   0 runner    (1001) docker     (121)    16027 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/pages/Dashboard.vue
--rw-r--r--   0 runner    (1001) docker     (121)      930 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/pages/Trigger.vue
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/pages/Error404.vue
--rw-r--r--   0 runner    (1001) docker     (121)    23867 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/pages/SettingsLibrary.vue
--rw-r--r--   0 runner    (1001) docker     (121)    12707 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/pages/SettingsWorkers.vue
--rw-r--r--   0 runner    (1001) docker     (121)    17461 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/pages/SettingsSupport.vue
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/language/
--rw-r--r--   0 runner    (1001) docker     (121)    17320 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/language/pl.json
--rw-r--r--   0 runner    (1001) docker     (121)    19922 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/language/ja.json
--rw-r--r--   0 runner    (1001) docker     (121)    17930 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/language/de.json
--rw-r--r--   0 runner    (1001) docker     (121)    17479 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/language/pt-br.json
--rw-r--r--   0 runner    (1001) docker     (121)    14643 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/language/zh.json
--rw-r--r--   0 runner    (1001) docker     (121)    17916 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/language/it.json
--rw-r--r--   0 runner    (1001) docker     (121)    24704 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/language/ru.json
--rw-r--r--   0 runner    (1001) docker     (121)    17200 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/language/nl.json
--rw-r--r--   0 runner    (1001) docker     (121)    16923 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/language/mi.json
--rw-r--r--   0 runner    (1001) docker     (121)    18515 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/language/fr.json
--rw-r--r--   0 runner    (1001) docker     (121)    16652 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/language/en.json
--rw-r--r--   0 runner    (1001) docker     (121)    17824 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/language/es.json
--rw-r--r--   0 runner    (1001) docker     (121)    16905 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/language/sv.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/
--rw-r--r--   0 runner    (1001) docker     (121)     2449 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/MarkdownDialog.vue
--rw-r--r--   0 runner    (1001) docker     (121)     4512 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/PendingTasks.vue
--rw-r--r--   0 runner    (1001) docker     (121)     8576 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/PluginInstallerManageRepos.vue
--rw-r--r--   0 runner    (1001) docker     (121)     6454 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/WorkerEventCreateDialog.vue
--rw-r--r--   0 runner    (1001) docker     (121)     2350 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/DrawerDataPanelsNav.vue
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/iframe-directive.js
--rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/LanguageSwitch.vue
--rw-r--r--   0 runner    (1001) docker     (121)     6754 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/WorkerProgress.vue
--rw-r--r--   0 runner    (1001) docker     (121)     2974 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/Avatar.vue
--rw-r--r--   0 runner    (1001) docker     (121)    16955 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/PluginsInstalledTable.vue
--rw-r--r--   0 runner    (1001) docker     (121)     8327 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/ReleaseNotesDialog.vue
--rw-r--r--   0 runner    (1001) docker     (121)    16362 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/PluginInstallerDialog.vue
--rw-r--r--   0 runner    (1001) docker     (121)     4168 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/CompletedTaskLogDialog.vue
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/MobileSettingsQuickNav.vue
--rw-r--r--   0 runner    (1001) docker     (121)    15456 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/WorkerGroupConfigureDialog.vue
--rw-r--r--   0 runner    (1001) docker     (121)    14192 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/LinkConfigureDialog.vue
--rw-r--r--   0 runner    (1001) docker     (121)    10522 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/PendingTasksTable.vue
--rw-r--r--   0 runner    (1001) docker     (121)     3929 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/JsonImportExportDialog.vue
--rw-r--r--   0 runner    (1001) docker     (121)     6253 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/PluginSelectorDialog.vue
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/WorkerProgressLog.vue
--rw-r--r--   0 runner    (1001) docker     (121)     4909 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/DrawerMainNav.vue
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/EssentialLink.vue
--rw-r--r--   0 runner    (1001) docker     (121)     4271 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/DrawerSettingsNav.vue
--rw-r--r--   0 runner    (1001) docker     (121)    25489 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/LibraryConfigureDialog.vue
--rw-r--r--   0 runner    (1001) docker     (121)     1713 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/FooterData.vue
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/LoginDialog.vue
--rw-r--r--   0 runner    (1001) docker     (121)    19828 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/PluginInfo.vue
--rw-r--r--   0 runner    (1001) docker     (121)    17019 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/CompletedTasksTable.vue
--rw-r--r--   0 runner    (1001) docker     (121)     6460 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/WorkerProgressStatus.vue
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/ThemeSwitch.vue
--rw-r--r--   0 runner    (1001) docker     (121)     5013 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/DirectoryBrowserDialog.vue
--rw-r--r--   0 runner    (1001) docker     (121)     8948 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/LibraryConfigurePluginFlowList.vue
--rw-r--r--   0 runner    (1001) docker     (121)     4511 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/components/CompletedTasks.vue
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/layouts/
--rw-r--r--   0 runner    (1001) docker     (121)     3998 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/layouts/MainLayout.vue
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/js/
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/js/markupParser.js
--rw-r--r--   0 runner    (1001) docker     (121)     8123 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/js/unmanicGlobals.js
--rw-r--r--   0 runner    (1001) docker     (121)    11389 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/js/unmanicWebsocket.js
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/js/dateTools.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/router/
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/router/routes.js
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/router/index.js
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/index.template.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/assets/
--rw-r--r--   0 runner    (1001) docker     (121)     3178 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    18218 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/assets/logo-lg.png
--rw-r--r--   0 runner    (1001) docker     (121)     4456 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/assets/quasar-logo-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (121)    37204 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/assets/unmanic-logo-white.png
--rw-r--r--   0 runner    (1001) docker     (121)   228094 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/assets/bg-md1.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    37547 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/assets/coffee-btn-image.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/boot/
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/boot/axios.js
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/frontend/src/boot/i18n.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/templates/global/
--rw-r--r--   0 runner    (1001) docker     (121)     2195 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/templates/global/login-popup.html
--rw-r--r--   0 runner    (1001) docker     (121)     2473 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/templates/global/support-future-development.html
--rw-r--r--   0 runner    (1001) docker     (121)     2326 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/templates/global/insufficient-permissions.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/webserver/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)     8214 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/helpers/completed_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17788 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/helpers/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     6213 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/helpers/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2439 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/helpers/documents.py
--rw-r--r--   0 runner    (1001) docker     (121)     5461 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/helpers/filebrowser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3008 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/helpers/workers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10260 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/helpers/pending_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/webserver/downloads.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/migrations_v1/
--rw-r--r--   0 runner    (1001) docker     (121)     2454 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/migrations_v1/001_rename_ffmpeg_log_to_log.py
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/migrations_v1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10923 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/service.py
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/version
--rw-r--r--   0 runner    (1001) docker     (121)    15518 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/libs/
--rw-r--r--   0 runner    (1001) docker     (121)    15035 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/uiserver.py
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/libs/unmodels/
--rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unmodels/installation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unmodels/completedtasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/libs/unmodels/lib/
--rw-r--r--   0 runner    (1001) docker     (121)     6012 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unmodels/lib/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1690 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unmodels/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unmodels/libraries.py
--rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unmodels/completedtaskscommandlogs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2389 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2144 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unmodels/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unmodels/enabledplugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     2204 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unmodels/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2059 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unmodels/librarypluginflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unmodels/workerschedules.py
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unmodels/workergroups.py
--rw-r--r--   0 runner    (1001) docker     (121)     1707 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unmodels/tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     1626 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unmodels/pluginrepos.py
--rw-r--r--   0 runner    (1001) docker     (121)     9890 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     9865 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/taskqueue.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20444 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/library.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/libs/unplugins/
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unplugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18939 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unplugins/pluginscli.py
--rw-r--r--   0 runner    (1001) docker     (121)    18151 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unplugins/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/library_management/
--rw-r--r--   0 runner    (1001) docker     (121)     3672 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/library_management/file_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/library_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3913 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3760 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/postprocessor/task_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     3916 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/postprocessor/file_move.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/frontend/
--rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3304 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/frontend/plugin_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2893 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/frontend/panel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/worker/
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/worker/process_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7526 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/plugin_type_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8593 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unplugins/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     7564 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/taskhandler.py
--rw-r--r--   0 runner    (1001) docker     (121)    13206 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/session.py
--rw-r--r--   0 runner    (1001) docker     (121)    30009 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)    37485 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/foreman.py
--rw-r--r--   0 runner    (1001) docker     (121)    12229 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/eventmonitor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/exceptions/ffprobe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1741 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/exceptions/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (121)     2251 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/base_codecs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/video_codecs/
--rw-r--r--   0 runner    (1001) docker     (121)     3526 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/video_codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/video_codecs/h264.py
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/video_codecs/hevc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/lib/
--rw-r--r--   0 runner    (1001) docker     (121)     5412 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/lib/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/lib/validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6562 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/audio_codec_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_codecs/
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_codecs/srt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1632 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_codecs/xsub.py
--rw-r--r--   0 runner    (1001) docker     (121)     3541 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_codecs/ssa.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_codecs/mov_text.py
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_codecs/ass.py
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_codecs/subrip.py
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2732 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/base_containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4774 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/video_codec_handle.py
--rw-r--r--   0 runner    (1001) docker     (121)    10828 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/info.py
--rw-r--r--   0 runner    (1001) docker     (121)     5016 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/containers/
--rw-r--r--   0 runner    (1001) docker     (121)     1656 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/containers/mpeg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/containers/vob.py
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/containers/ogv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1632 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/containers/mov.py
--rw-r--r--   0 runner    (1001) docker     (121)     3524 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1642 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/containers/avi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/containers/mp4.py
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/containers/flv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1607 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/containers/psp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1656 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/containers/mpegts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/containers/matroska.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/audio_codecs/
--rw-r--r--   0 runner    (1001) docker     (121)     1633 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/audio_codecs/aac.py
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/audio_codecs/ac3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/audio_codecs/mp3.py
--rw-r--r--   0 runner    (1001) docker     (121)     3526 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/audio_codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8625 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unffmpeg/hardware_acceleration_handle.py
--rw-r--r--   0 runner    (1001) docker     (121)    76048 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/installation_link.py
--rw-r--r--   0 runner    (1001) docker     (121)     9278 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/filetest.py
--rw-r--r--   0 runner    (1001) docker     (121)    16026 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/task.py
--rw-r--r--   0 runner    (1001) docker     (121)    21148 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (121)     7266 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/directoryinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)    10702 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/history.py
--rw-r--r--   0 runner    (1001) docker     (121)    14410 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/libraryscanner.py
--rw-r--r--   0 runner    (1001) docker     (121)     5363 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/unlogger.py
--rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/system.py
--rw-r--r--   0 runner    (1001) docker     (121)     3283 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/fileinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     9309 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)    10605 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/worker_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     6330 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/db_migrate.py
--rw-r--r--   0 runner    (1001) docker     (121)    31047 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/libs/workers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3627 2022-06-04 23:30:46.000000 unmanic-0.2.3/unmanic/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11147 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    49194 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-06-04 23:31:17.000000 unmanic-0.2.3/unmanic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-06-04 23:30:46.000000 unmanic-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-06-04 23:31:17.000000 unmanic-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6730 2022-06-04 23:30:46.000000 unmanic-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    49194 2022-06-04 23:31:17.000000 unmanic-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-04 23:30:46.000000 unmanic-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-06-04 23:30:46.000000 unmanic-0.2.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 04:53:32.000000 unmanic-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-23 04:53:32.000000 unmanic-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    49297 2023-04-23 04:53:50.000000 unmanic-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-23 04:53:32.000000 unmanic-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    27920 2023-04-23 04:53:32.000000 unmanic-0.2.4/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-23 04:53:32.000000 unmanic-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-23 04:53:50.000000 unmanic-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-04-23 04:53:32.000000 unmanic-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15518 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/db_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/directoryinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/eventmonitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/fileinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/filetest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37626 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/foreman.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76109 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/installation_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20446 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/libraryscanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32415 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21999 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16026 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/taskhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/taskqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15034 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/uiserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/audio_codec_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/audio_codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/audio_codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/audio_codecs/aac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/audio_codecs/ac3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/audio_codecs/mp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/base_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/base_containers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/containers/avi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/containers/flv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/containers/matroska.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/containers/mov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/containers/mp4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/containers/mpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/containers/mpegts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/containers/ogv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/containers/psp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/containers/vob.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/exceptions/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/exceptions/ffprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/hardware_acceleration_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/lib/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/lib/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_codecs/ass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_codecs/mov_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_codecs/srt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_codecs/ssa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_codecs/subrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_codecs/xsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/video_codec_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/video_codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/video_codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/video_codecs/h264.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unffmpeg/video_codecs/hevc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unlogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/libs/unmodels/
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unmodels/completedtasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unmodels/completedtaskscommandlogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unmodels/enabledplugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unmodels/installation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/libs/unmodels/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unmodels/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unmodels/lib/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unmodels/libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unmodels/librarypluginflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unmodels/pluginrepos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unmodels/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unmodels/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unmodels/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unmodels/workergroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unmodels/workerschedules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/libs/unplugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unplugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18496 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unplugins/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/frontend/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/frontend/plugin_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/library_management/
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/library_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/library_management/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/plugin_type_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/postprocessor/file_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/postprocessor/task_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/worker/process_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22384 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unplugins/pluginscli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/unplugins/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/worker_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31146 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/libs/workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/migrations_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/migrations_v1/001_rename_ffmpeg_log_to_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/migrations_v1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11104 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_request_router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/api_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v1/base_api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v1/filebrowser_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v1/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v1/pending_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v1/plugins_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v1/session_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/api_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/base_api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/docs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/filebrowser_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14004 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30798 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/pending_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46051 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/plugins_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/api_v2/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43658 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/schema/schemas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4064 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/schema/swagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/schema/unmanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/session_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50039 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/version_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17949 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/api_v2/workers_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   261856 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/docs/api_schema_v2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   132047 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/docs/api_schema_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/docs/privacy_policy.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/downloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/.eslintignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/.eslintrc.js
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/.postcssrc.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1474 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/babel.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/jsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)   765678 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/frontend/public/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/public/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/frontend/public/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/public/icons/favicon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/public/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/public/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/public/icons/favicon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/quasar.conf.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/frontend/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      712 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/scripts/translate.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/App.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   228094 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/assets/bg-md1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    37547 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/assets/coffee-btn-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/assets/logo-lg.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/assets/quasar-logo-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    37204 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/assets/unmanic-logo-white.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/boot/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/boot/axios.js
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/boot/global-event-bus.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/boot/i18n.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/Avatar.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/CompletedTaskLogDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/CompletedTasks.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/CompletedTasksTable.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/DirectoryBrowserDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/DrawerDataPanelsNav.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/DrawerMainNav.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/DrawerNotifications.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/DrawerSettingsNav.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/EssentialLink.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/FooterData.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/JsonImportExportDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/LanguageSwitch.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/LibraryConfigurePluginFlowList.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/LinkConfigureDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/LoginDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/MarkdownDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/MobileSettingsQuickNav.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/PendingTasks.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/PendingTasksTable.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/PluginInstallerManageRepos.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/PluginSelectorDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    19735 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/PluginsInstalledTable.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/ReleaseNotesDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/ThemeSwitch.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/WorkerEventCreateDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    15456 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/WorkerGroupConfigureDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/WorkerProgress.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/WorkerProgressLog.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/WorkerProgressStatus.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/dialogs/ConfigDrawerDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    23291 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/dialogs/PluginInfoDialog.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)    22212 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/forms/LibraryConfigForm.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/forms/PluginInstallerForm.vue
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/components/iframe-directive.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/css/app.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/css/markdown-admonitions.css
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/css/quasar.variables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/index.template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/js/dateTools.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/js/markupParser.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/js/unmanicGlobals.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/js/unmanicWebsocket.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/language/
+-rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/language/de.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/language/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18252 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/language/es.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18971 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/language/fr.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18307 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/language/it.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20438 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/language/ja.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17305 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/language/mi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17599 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/language/nl.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/language/pl.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17875 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/language/pt-br.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25260 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/language/ru.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17301 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/language/sv.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/language/zh.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/layouts/MainLayout.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    16027 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/pages/Dashboard.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/pages/DataPanels.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/pages/Error404.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    23948 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/pages/SettingsLibrary.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    23789 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/pages/SettingsLink.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/pages/SettingsPlugins.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    17461 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/pages/SettingsSupport.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/pages/SettingsWorkers.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/pages/Trigger.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/router/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/router/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-23 04:53:33.000000 unmanic-0.2.4/unmanic/webserver/frontend/src/router/routes.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/helpers/completed_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/helpers/documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/helpers/filebrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/helpers/pending_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18233 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/helpers/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/helpers/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/helpers/workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic/webserver/templates/global/
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/templates/global/insufficient-permissions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/templates/global/login-popup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/templates/global/support-future-development.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-04-23 04:53:32.000000 unmanic-0.2.4/unmanic/webserver/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49297 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 04:53:50.000000 unmanic-0.2.4/unmanic.egg-info/top_level.txt
```

### Comparing `unmanic-0.2.3/logo.png` & `unmanic-0.2.4/logo.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/setup.py` & `unmanic-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,19 @@
 module_author = versioninfo.author()
 module_email = versioninfo.email()
 module_url = versioninfo.url()
 module_classifiers = [
     versioninfo.dev_status(),
     'Intended Audience :: End Users/Desktop',
     'Intended Audience :: Developers',
-    'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Operating System :: POSIX :: Linux',
     'Operating System :: Unix',
     'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
     'Topic :: Multimedia :: Video :: Conversion',
     'Topic :: Internet :: WWW/HTTP',
 ]
```

### Comparing `unmanic-0.2.3/unmanic/webserver/package-lock.json` & `unmanic-0.2.4/unmanic/webserver/package-lock.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/websocket.py` & `unmanic-0.2.4/unmanic/webserver/websocket.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v1/history_api.py` & `unmanic-0.2.4/unmanic/webserver/api_v1/history_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v1/filebrowser_api.py` & `unmanic-0.2.4/unmanic/webserver/api_v1/filebrowser_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v1/__init__.py` & `unmanic-0.2.4/unmanic/webserver/api_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v1/pending_api.py` & `unmanic-0.2.4/unmanic/webserver/api_v1/pending_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v1/session_api.py` & `unmanic-0.2.4/unmanic/webserver/api_v1/session_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v1/base_api_handler.py` & `unmanic-0.2.4/unmanic/webserver/api_v1/base_api_handler.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v1/plugins_api.py` & `unmanic-0.2.4/unmanic/webserver/api_v1/plugins_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/__init__.py` & `unmanic-0.2.4/unmanic/webserver/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/plugins.py` & `unmanic-0.2.4/unmanic/webserver/plugins.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_request_router.py` & `unmanic-0.2.4/unmanic/webserver/api_request_router.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/history_api.py` & `unmanic-0.2.4/unmanic/webserver/api_v2/history_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/docs_api.py` & `unmanic-0.2.4/unmanic/webserver/api_v2/docs_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/filebrowser_api.py` & `unmanic-0.2.4/unmanic/webserver/api_v2/filebrowser_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/__init__.py` & `unmanic-0.2.4/unmanic/webserver/api_v2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,28 +32,30 @@
 
 from __future__ import absolute_import
 import warnings
 
 from .docs_api import ApiDocsHandler
 from .filebrowser_api import ApiFilebrowserHandler
 from .history_api import ApiHistoryHandler
+from .notifications_api import ApiNotificationsHandler
 from .pending_api import ApiPendingHandler
 from .plugins_api import ApiPluginsHandler
 from .session_api import ApiSessionHandler
 from .settings_api import ApiSettingsHandler
 from .upload_api import ApiUploadHandler
 from .version_api import ApiVersionHandler
 from .workers_api import ApiWorkersHandler
 
 __author__ = 'Josh.5 (jsunnex@gmail.com)'
 
 __all__ = (
     'ApiDocsHandler',
     'ApiFilebrowserHandler',
     'ApiHistoryHandler',
+    'ApiNotificationsHandler',
     'ApiPendingHandler',
     'ApiPluginsHandler',
     'ApiSessionHandler',
     'ApiSettingsHandler',
     'ApiUploadHandler',
     'ApiVersionHandler',
     'ApiWorkersHandler'
```

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/pending_api.py` & `unmanic-0.2.4/unmanic/webserver/api_v2/pending_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/session_api.py` & `unmanic-0.2.4/unmanic/webserver/api_v2/session_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/base_api_handler.py` & `unmanic-0.2.4/unmanic/webserver/api_v2/base_api_handler.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/workers_api.py` & `unmanic-0.2.4/unmanic/webserver/api_v2/workers_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/plugins_api.py` & `unmanic-0.2.4/unmanic/webserver/api_v2/plugins_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/schema/schemas.py` & `unmanic-0.2.4/unmanic/webserver/api_v2/schema/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,26 @@
         required=True,
         description="List of table IDs",
         example=[],
         validate=validate.Length(min=1),
     )
 
 
+class RequestTableUpdateByUuidList(BaseSchema):
+    """Schema for updating tables by UUID"""
+
+    uuid_list = fields.List(
+        cls_or_instance=fields.Str,
+        required=True,
+        description="List of table UUIDs",
+        example=[],
+        validate=validate.Length(min=1),
+    )
+
+
 class TableRecordsSuccessSchema(BaseSchema):
     """Schema for table results"""
 
     recordsTotal = fields.Int(
         required=False,
         description="Total number of records in this table",
         example=329,
@@ -377,14 +389,64 @@
     library_id = fields.Int(
         required=False,
         load_default=0,
         example=1,
     )
 
 
+# NOTIFICATIONS
+# =============
+
+class NotificationDataSchema(BaseSchema):
+    """Schema for notification data"""
+
+    uuid = fields.Str(
+        required=True,
+        description="Unique ID for this notification",
+        example="updateAvailable",
+    )
+    type = fields.Str(
+        required=True,
+        description="The type of notification",
+        example="info",
+    )
+    icon = fields.Str(
+        required=True,
+        description="The icon to display with the notification",
+        example="update",
+    )
+    label = fields.Str(
+        required=True,
+        description="The label of the notification. Can be a I18n key or a string",
+        example="updateAvailableLabel",
+    )
+    message = fields.Str(
+        required=True,
+        description="The message of the notification. Can be a I18n key or a string",
+        example="updateAvailableMessage",
+    )
+    navigation = fields.Dict(
+        required=True,
+        description="The navigation links of the notification",
+        example={'url': "https://docs.unmanic.app"},
+    )
+
+
+class RequestNotificationsDataSchema(BaseSchema):
+    """Schema for returning the current list of notifications"""
+
+    notifications = fields.Nested(
+        NotificationDataSchema,
+        required=True,
+        description="List of notifications",
+        many=True,
+        validate=validate.Length(min=0),
+    )
+
+
 # PENDING
 # =======
 
 class RequestPendingTableDataSchema(RequestTableDataSchema):
     """Schema for requesting pending tasks from the table"""
 
     order_by = fields.Str(
@@ -665,14 +727,26 @@
         example="checkbox",
     )
     label = fields.Str(
         required=True,
         description="The label used to define this config input",
         example="Downmix DTS-HD Master Audio (max 5.1 channels)?",
     )
+    description = fields.Str(
+        required=True,
+        description="Description of input field",
+        example="Will automatically downmix DTS-HD Master Audio to 5.1 channels ",
+        allow_none=True,
+    )
+    tooltip = fields.Str(
+        required=True,
+        description="Description of input field",
+        example="Will automatically downmix DTS-HD Master Audio to 5.1 channels ",
+        allow_none=True,
+    )
     select_options = fields.List(
         cls_or_instance=fields.Dict,
         required=True,
         description="Additional options if the input_type is set to 'select'",
         example=[
             {
                 'value': "first",
@@ -694,14 +768,19 @@
         },
     )
     display = fields.Str(
         required=True,
         description="Should the setting input be displayed (visible, hidden)",
         example="visible",
     )
+    sub_setting = fields.Boolean(
+        required=True,
+        description="Should the setting be a nested sub-setting field",
+        example=False,
+    )
 
 
 class PluginsInfoResultsSchema(PluginsMetadataResultsSchema):
     """Schema for pending task results returned by the table"""
 
     settings = fields.Nested(
         PluginsConfigInputItemSchema,
```

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/schema/__init__.py` & `unmanic-0.2.4/unmanic/webserver/api_v2/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/schema/unmanic.py` & `unmanic-0.2.4/unmanic/webserver/api_v2/schema/unmanic.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/schema/swagger.py` & `unmanic-0.2.4/unmanic/webserver/api_v2/schema/swagger.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/settings_api.py` & `unmanic-0.2.4/unmanic/webserver/api_v2/settings_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/upload_api.py` & `unmanic-0.2.4/unmanic/webserver/api_v2/upload_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -65,41 +65,49 @@
 
     routes = [
         {
             "path_pattern":      r"/upload/pending/file",
             "supported_methods": ["POST"],
             "call_method":       "upload_file_to_pending_tasks",
         },
+        {
+            "path_pattern":      r"/upload/plugin/file",
+            "supported_methods": ["POST"],
+            "call_method":       "upload_and_install_plugin",
+        },
     ]
 
     def initialize(self, **kwargs):
         self.session = session.Session()
         self.params = kwargs.get("params")
         self.config = config.Config()
         self.frontend_messages = FrontendPushMessages()
 
     def prepare(self):
         self.bytes_read = 0
         self.meta = dict()
-        self.receiver = self.get_receiver()
+        upload_type = "pending"
+        if "upload/plugin/file" in self.request.uri:
+            upload_type = "plugin"
+        self.receiver = self.get_receiver(upload_type)
 
         # If max_body_size is not set, you cannot upload files > 100MB
         self.request.connection.set_max_body_size(MAX_STREAMED_SIZE)
 
         # Set the output path to the cache directory
         out_folder = "unmanic_remote_pending_library-{}".format(time.time())
         if not self.cache_directory:
             self.cache_directory = os.path.join(self.config.get_cache_path(), 'remote_library', out_folder)
             if not os.path.exists(self.cache_directory):
                 os.makedirs(self.cache_directory)
 
     def data_received(self, chunk):
         self.receiver(chunk)
 
-    def get_receiver(self):
+    def get_receiver(self, upload_type):
         index = 0
         frontend_messages = self.frontend_messages
 
         def receiver(chunk):
             nonlocal index
             nonlocal frontend_messages
             if index == 0:
@@ -108,39 +116,40 @@
 
                 self.meta['boundary'] = SEPARATOR + split_chunk[0] + b'--' + SEPARATOR
                 self.meta['header'] = SEPARATOR.join(split_chunk[0:3])
                 self.meta['header'] += SEPARATOR * 2
                 self.meta['filename'] = split_chunk[1].split(b'=')[-1].replace(b'"', b'').decode()
 
                 if frontend_messages:
-                    frontend_messages.update(
-                        {
-                            'id':      'receivingRemoteFile',
-                            'type':    'status',
-                            'code':    'receivingRemoteFile',
-                            'message': self.meta['filename'],
-                            'timeout': 0
-                        }
-                    )
+                    if upload_type == 'pending':
+                        frontend_messages.update(
+                            {
+                                'id':      'receivingRemoteFile',
+                                'type':    'status',
+                                'code':    'receivingRemoteFile',
+                                'message': self.meta['filename'],
+                                'timeout': 0
+                            }
+                        )
 
                 chunk = chunk[len(self.meta['header']):]
                 self.fp = open(os.path.join(self.cache_directory, self.meta['filename']), "wb")
                 self.fp.write(chunk)
             else:
                 self.fp.write(chunk)
 
         return receiver
 
     def upload_file_to_pending_tasks(self):
         """
-        Pending - list tasks
+        Upload - upload a new pending task
         ---
-        description: Returns a list of pending tasks.
+        description: Uploads a file to the pending tasks list
         requestBody:
-            description: Returns a list of pending tasks.
+            description: Uploads a file to the pending tasks list
             required: True
             content:
                 multipart/form-data:
                     schema:
                         type: object
                         properties:
                             fileName:
@@ -228,11 +237,92 @@
             return
         except BaseApiError as bae:
             tornado.log.app_log.error("BaseApiError.{}: {}".format(self.route.get('call_method'), str(bae)))
             if self.frontend_messages:
                 self.frontend_messages.remove_item('receivingRemoteFile')
             return
         except Exception as e:
+            if self.frontend_messages:
+                self.frontend_messages.remove_item('receivingRemoteFile')
+            self.set_status(self.STATUS_ERROR_INTERNAL, reason=str(e))
+            self.write_error()
+
+    def upload_and_install_plugin(self):
+        """
+        Upload - upload a plugin and install it
+        ---
+        description: Uploads a plugin ZIP file and installs it
+        requestBody:
+            description: Uploads a plugin ZIP file and installs it
+            required: True
+            content:
+                multipart/form-data:
+                    schema:
+                        type: object
+                        properties:
+                            fileName:
+                                type: string
+                                format: binary
+        responses:
+            200:
+                description: 'Successful request; Returns success status'
+                content:
+                    application/json:
+                        schema:
+                            BaseSuccessSchema
+            400:
+                description: Bad request; Check `messages` for any validation errors
+                content:
+                    application/json:
+                        schema:
+                            BadRequestSchema
+            404:
+                description: Bad request; Requested endpoint not found
+                content:
+                    application/json:
+                        schema:
+                            BadEndpointSchema
+            405:
+                description: Bad request; Requested method is not allowed
+                content:
+                    application/json:
+                        schema:
+                            BadMethodSchema
+            500:
+                description: Internal error; Check `error` for exception
+                content:
+                    application/json:
+                        schema:
+                            InternalErrorSchema
+        """
+        try:
+            self.meta['content_length'] = int(self.request.headers.get('Content-Length')) - \
+                                          len(self.meta['header']) - \
+                                          len(self.meta['boundary'])
+
+            self.fp.seek(self.meta['content_length'], 0)
+            self.fp.truncate()
+            self.fp.close()
+
+            # Create task entry for the file
+            upload_path = os.path.join(self.cache_directory, self.meta['filename'])
+
+            # Install plugin from zip
+            from unmanic.libs.plugins import PluginsHandler
+            plugins = PluginsHandler()
+            if not plugins.install_plugin_from_path_on_disk(upload_path):
+                self.set_status(self.STATUS_ERROR_INTERNAL, reason="Failed to upload and install/update plugin")
+                self.write_error()
+                return
+
+            self.write_success()
+            return
+        except BaseApiError as bae:
+            tornado.log.app_log.error("BaseApiError.{}: {}".format(self.route.get('call_method'), str(bae)))
+            if self.frontend_messages:
+                self.frontend_messages.remove_item('receivingRemoteFile')
+            return
+        except Exception as e:
             if self.frontend_messages:
                 self.frontend_messages.remove_item('receivingRemoteFile')
             self.set_status(self.STATUS_ERROR_INTERNAL, reason=str(e))
             self.write_error()
```

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/README.md` & `unmanic-0.2.4/unmanic/webserver/api_v2/README.md`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/api_v2/version_api.py` & `unmanic-0.2.4/unmanic/webserver/api_v2/version_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/main.py` & `unmanic-0.2.4/unmanic/webserver/main.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/package.json` & `unmanic-0.2.4/unmanic/webserver/package.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/docs/privacy_policy.md` & `unmanic-0.2.4/unmanic/webserver/docs/privacy_policy.md`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/docs/api_schema_v2.yaml` & `unmanic-0.2.4/unmanic/webserver/docs/api_schema_v2.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,1430 +1,1519 @@
+info:
+  description: Documentation for the Unmanic application API
+  title: Unmanic API
+  version: '2'
+servers:
+- url: http://localhost:8888/unmanic/api/v2/
+  description: Local environment
 components:
+  securitySchemes:
+    BasicAuth:
+      type: http
+      scheme: basic
   schemas:
-    BadEndpoint:
-      properties:
-        error:
-          description: Return status code and reason
-          example: '404: Endpoint not found'
-          type: string
-      required:
-      - error
+    DocumentContentSuccess:
       type: object
-    BadMethod:
       properties:
-        error:
-          description: Return status code and reason
-          example: '405: Method ''GET'' not allowed'
-          type: string
+        content:
+          type: array
+          minItems: 1
+          description: Document contents read line-by-line into a list
+          example:
+          - 'First line
+
+            '
+          - 'Second line
+
+            '
+          - '
+
+            '
+          items:
+            type: string
       required:
-      - error
-      type: object
+      - content
     BadRequest:
+      type: object
       properties:
         error:
+          type: string
           description: Return status code and reason
           example: '400: Failed request schema validation'
-          type: string
         messages:
+          type: object
           description: Attached request body validation errors
           example: &id001
             name:
             - The thing that went wrong.
-          type: object
         traceback:
+          type: array
           description: Attached exception traceback (if developer mode is enabled)
           example: &id002
           - 'Traceback (most recent call last):
 
             '
           - '...'
           - 'json.decoder.JSONDecodeError: Expecting value: line 3 column 14 (char
             45)
 
             '
           items:
             type: string
+      required:
+      - error
+      - messages
+    BadEndpoint:
+      type: object
+      properties:
+        error:
+          type: string
+          description: Return status code and reason
+          example: '404: Endpoint not found'
+      required:
+      - error
+    BadMethod:
+      type: object
+      properties:
+        error:
+          type: string
+          description: Return status code and reason
+          example: '405: Method ''GET'' not allowed'
+      required:
+      - error
+    InternalError:
+      type: object
+      properties:
+        error:
+          type: string
+          description: Return status code and reason
+          example: '500: Caught exception message'
+        messages:
+          type: object
+          description: Attached request body validation errors
+          example: *id001
+        traceback:
           type: array
+          description: Attached exception traceback (if developer mode is enabled)
+          example: *id002
+          items:
+            type: string
       required:
       - error
       - messages
+    RequestDirectoryListingData:
       type: object
-    BaseSuccess:
       properties:
-        success:
-          description: This is always "True" when a request succeeds
-          example: true
-          type: boolean
+        current_path:
+          type: string
+          default: /
+          example: /
+        list_type:
+          type: string
+          default: all
+          example: directories
+    DirectoryListingResults:
+      type: object
+      properties:
+        directories:
+          type: array
+          minItems: 0
+          description: A list of directories in the given path
+          example:
+          - value: home
+            label: /home
+          - value: tmp
+            label: /tmp
+          items:
+            type: object
+        files:
+          type: array
+          minItems: 0
+          description: A list of files in the given path
+          example:
+          - value: file1.txt
+            label: /file1.txt
+          - value: file2.txt
+            label: /file2.txt
+          items:
+            type: object
       required:
-      - success
+      - directories
+      - files
+    RequestHistoryTableData:
+      type: object
+      properties:
+        start:
+          type: integer
+          default: 0
+          description: Start row number to select from
+          example: 0
+        length:
+          type: integer
+          default: 10
+          description: Number of rows to select
+          example: 10
+        search_value:
+          type: string
+          default: ''
+          description: String to filter search results by
+          example: items with this text in the value
+        status:
+          type: string
+          default: all
+          description: Filter on the status
+          example: all
+        after:
+          type: string
+          format: date-time
+          nullable: true
+          description: Filter entries since datetime
+          example: 2022-04-07 01:45
+        before:
+          type: string
+          format: date-time
+          nullable: true
+          description: Filter entries prior to datetime
+          example: 2022-04-07 01:55
+        order_by:
+          type: string
+          default: finish_time
+          example: finish_time
+        order_direction:
+          type: string
+          enum:
+          - asc
+          - desc
+          description: Order direction ('asc' or 'desc')
+          example: desc
+    CompletedTasksTableResults:
       type: object
+      properties:
+        id:
+          type: integer
+          description: Item ID
+          example: 1
+        task_label:
+          type: string
+          description: Item label
+          example: example.mp4
+        task_success:
+          type: boolean
+          description: Item success status
+          example: true
+        finish_time:
+          type: integer
+          description: Item finish time
+          example: 1627392616.6400812
+      required:
+      - finish_time
+      - id
+      - task_label
+      - task_success
     CompletedTasks:
+      type: object
       properties:
         recordsTotal:
+          type: integer
           description: Total number of records in this table
           example: 329
-          type: integer
         recordsFiltered:
+          type: integer
           default: 10
           description: Total number of records after filters have been applied
           example: 10
-          type: integer
         results:
+          minItems: 0
           description: Results
+          type: array
           items:
             $ref: '#/components/schemas/CompletedTasksTableResults'
-          minItems: 0
-          type: array
         successCount:
+          type: integer
           description: Total count of times with a success status in the results list
           example: 337
-          type: integer
         failedCount:
+          type: integer
           description: Total count of times with a failed status in the results list
           example: 2
-          type: integer
       required:
       - failedCount
       - results
       - successCount
+    RequestTableUpdateByIdList:
+      type: object
+      properties:
+        id_list:
+          type: array
+          minItems: 1
+          description: List of table IDs
+          example: &id003 []
+          items:
+            type: integer
+      required:
+      - id_list
+    BaseSuccess:
+      type: object
+      properties:
+        success:
+          type: boolean
+          description: This is always "True" when a request succeeds
+          example: true
+      required:
+      - success
+    RequestAddCompletedToPendingTasks:
       type: object
+      properties:
+        id_list:
+          type: array
+          minItems: 1
+          description: List of table IDs
+          example: *id003
+          items:
+            type: integer
+        library_id:
+          type: integer
+          default: 0
+          example: 1
+      required:
+      - id_list
+    CompletedTasksLogRequest:
+      type: object
+      properties:
+        task_id:
+          type: integer
+          description: The ID of the task
+          example: 1
+      required:
+      - task_id
     CompletedTasksLog:
+      type: object
       properties:
         command_log:
+          type: string
           description: Long string...
           example: Long string...
-          type: string
         command_log_lines:
+          type: array
           description: The long string broken up into an array of lines
           example:
           - ''
           - '<b>RUNNER: </b>'
           - 'Video Encoder H264 - libx264 [Pass #1]'
           - ''
           - <b>COMMAND:</b>
           - ''
           - '...'
           items:
             type: string
-          type: array
       required:
       - command_log
       - command_log_lines
+    NotificationData:
       type: object
-    CompletedTasksLogRequest:
-      properties:
-        task_id:
-          description: The ID of the task
-          example: 1
-          type: integer
-      required:
-      - task_id
-      type: object
-    CompletedTasksTableResults:
       properties:
-        id:
-          description: Item ID
-          example: 1
-          type: integer
-        task_label:
-          description: Item label
-          example: example.mp4
+        uuid:
           type: string
-        task_success:
-          description: Item success status
-          example: true
-          type: boolean
-        finish_time:
-          description: Item finish time
-          example: 1627392616.6400812
-          type: integer
+          description: Unique ID for this notification
+          example: updateAvailable
+        type:
+          type: string
+          description: The type of notification
+          example: info
+        icon:
+          type: string
+          description: The icon to display with the notification
+          example: update
+        label:
+          type: string
+          description: The label of the notification. Can be a I18n key or a string
+          example: updateAvailableLabel
+        message:
+          type: string
+          description: The message of the notification. Can be a I18n key or a string
+          example: updateAvailableMessage
+        navigation:
+          type: object
+          description: The navigation links of the notification
+          example:
+            url: https://docs.unmanic.app
       required:
-      - finish_time
-      - id
-      - task_label
-      - task_success
+      - icon
+      - label
+      - message
+      - navigation
+      - type
+      - uuid
+    RequestNotificationsData:
       type: object
-    DirectoryListingResults:
       properties:
-        directories:
-          description: A list of directories in the given path
-          example:
-          - label: /home
-            value: home
-          - label: /tmp
-            value: tmp
-          items:
-            type: object
+        notifications:
           minItems: 0
+          description: List of notifications
           type: array
-        files:
-          description: A list of files in the given path
-          example:
-          - label: /file1.txt
-            value: file1.txt
-          - label: /file2.txt
-            value: file2.txt
           items:
-            type: object
-          minItems: 0
-          type: array
+            $ref: '#/components/schemas/NotificationData'
       required:
-      - directories
-      - files
+      - notifications
+    RequestTableUpdateByUuidList:
       type: object
-    DocumentContentSuccess:
       properties:
-        content:
-          description: Document contents read line-by-line into a list
-          example:
-          - 'First line
-
-            '
-          - 'Second line
-
-            '
-          - '
-
-            '
-          items:
-            type: string
-          minItems: 1
+        uuid_list:
           type: array
-      required:
-      - content
-      type: object
-    InternalError:
-      properties:
-        error:
-          description: Return status code and reason
-          example: '500: Caught exception message'
-          type: string
-        messages:
-          description: Attached request body validation errors
-          example: *id001
-          type: object
-        traceback:
-          description: Attached exception traceback (if developer mode is enabled)
-          example: *id002
+          minItems: 1
+          description: List of table UUIDs
+          example: []
           items:
             type: string
-          type: array
       required:
-      - error
-      - messages
+      - uuid_list
+    RequestPendingTableData:
       type: object
-    LibraryResults:
       properties:
-        id:
-          description: ''
-          example: 1
+        start:
           type: integer
-        name:
-          description: The name of the library
-          example: Default
-          type: string
-        path:
-          description: The library path
-          example: /library
-          type: string
-        locked:
-          description: If the library is locked and cannot be deleted
-          example: false
-          type: boolean
-        enable_remote_only:
-          description: If the library is configured for remote files only
-          example: false
-          type: boolean
-        enable_scanner:
-          description: If the library is configured to execute library scans
-          example: false
-          type: boolean
-        enable_inotify:
-          description: If the library is configured to monitor for file changes
-          example: false
-          type: boolean
-        tags:
-          description: A list of tags associated with this library
-          example:
-          - GPU
-          - priority
-          items:
-            type: string
-          type: array
-      required:
-      - enable_inotify
-      - enable_remote_only
-      - enable_scanner
-      - id
-      - locked
-      - name
-      - path
-      - tags
-      type: object
-    PendingTasks:
-      properties:
-        recordsTotal:
-          description: Total number of records in this table
-          example: 329
+          default: 0
+          description: Start row number to select from
+          example: 0
+        length:
           type: integer
-        recordsFiltered:
           default: 10
-          description: Total number of records after filters have been applied
+          description: Number of rows to select
           example: 10
-          type: integer
-        results:
-          description: Results
-          items:
-            $ref: '#/components/schemas/PendingTasksTableResults'
-          minItems: 0
-          type: array
-      required:
-      - results
-      type: object
+        search_value:
+          type: string
+          default: ''
+          description: String to filter search results by
+          example: items with this text in the value
+        status:
+          type: string
+          default: all
+          description: Filter on the status
+          example: all
+        after:
+          type: string
+          format: date-time
+          nullable: true
+          description: Filter entries since datetime
+          example: 2022-04-07 01:45
+        before:
+          type: string
+          format: date-time
+          nullable: true
+          description: Filter entries prior to datetime
+          example: 2022-04-07 01:55
+        order_by:
+          type: string
+          default: priority
+          example: priority
+        order_direction:
+          type: string
+          enum:
+          - asc
+          - desc
+          description: Order direction ('asc' or 'desc')
+          example: desc
     PendingTasksTableResults:
+      type: object
       properties:
         id:
+          type: integer
           description: Item ID
           example: 1
-          type: integer
         abspath:
+          type: string
           description: File absolute path
           example: example.mp4
-          type: string
         priority:
+          type: integer
           description: The current priority (higher is greater)
           example: 100
-          type: integer
         type:
+          type: string
           description: The type of the pending task - local or remote
           example: local
-          type: string
         status:
+          type: string
           description: The current status of the pending task
           example: pending
-          type: string
         checksum:
+          type: string
           description: The uploaded file md5 checksum
           example: 5425ab3df5cdbad2e1099bb4cb963a4f
-          type: string
         library_id:
+          type: integer
           description: The ID of the library for which this task was created
           example: 1
-          type: integer
         library_name:
+          type: string
           description: The name of the library for which this task was created
           example: Default
-          type: string
       required:
       - abspath
       - id
       - priority
       - status
       - type
+    PendingTasks:
+      type: object
+      properties:
+        recordsTotal:
+          type: integer
+          description: Total number of records in this table
+          example: 329
+        recordsFiltered:
+          type: integer
+          default: 10
+          description: Total number of records after filters have been applied
+          example: 10
+        results:
+          minItems: 0
+          description: Results
+          type: array
+          items:
+            $ref: '#/components/schemas/PendingTasksTableResults'
+      required:
+      - results
+    RequestPendingTasksReorder:
+      type: object
+      properties:
+        id_list:
+          type: array
+          minItems: 1
+          description: List of table IDs
+          example: *id003
+          items:
+            type: integer
+        position:
+          type: string
+          enum:
+          - top
+          - bottom
+          description: Position to move given list of items to ('top' or 'bottom')
+          example: top
+      required:
+      - id_list
+      - position
+    RequestPendingTaskCreate:
+      type: object
+      properties:
+        path:
+          type: string
+          description: The absolute path to a file
+          example: /library/TEST_FILE.mkv
+        library_id:
+          type: integer
+          description: The ID of the library to append this task to
+          example: 1
+        library_name:
+          type: string
+          description: The name of the library to append this task to
+          example: Default
+        type:
+          type: string
+          description: The type of pending task to create (local/remote)
+          example: local
+        priority_score:
+          type: integer
+          description: Apply a priority score to the created task to either increase
+            or decrease its position in the queue
+          example: 1000
+      required:
+      - path
+    RequestPendingTasksLibraryUpdate:
+      type: object
+      properties:
+        id_list:
+          type: array
+          minItems: 1
+          description: List of table IDs
+          example: *id003
+          items:
+            type: integer
+        library_name:
+          type: string
+          example: Default
+      required:
+      - id_list
+      - library_name
+    TaskDownloadLink:
+      type: object
+      properties:
+        link_id:
+          type: string
+          description: The ID used to download the file /unmanic/downloads/{link_id}
+          example: 2960645c-a4e2-4b05-8866-7bd469ee9ef8
+      required:
+      - link_id
+    RequestPluginsTableData:
+      type: object
+      properties:
+        start:
+          type: integer
+          default: 0
+          description: Start row number to select from
+          example: 0
+        length:
+          type: integer
+          default: 10
+          description: Number of rows to select
+          example: 10
+        search_value:
+          type: string
+          default: ''
+          description: String to filter search results by
+          example: items with this text in the value
+        status:
+          type: string
+          default: all
+          description: Filter on the status
+          example: all
+        after:
+          type: string
+          format: date-time
+          nullable: true
+          description: Filter entries since datetime
+          example: 2022-04-07 01:45
+        before:
+          type: string
+          format: date-time
+          nullable: true
+          description: Filter entries prior to datetime
+          example: 2022-04-07 01:55
+        order_by:
+          type: string
+          default: name
+          example: name
+        order_direction:
+          type: string
+          enum:
+          - asc
+          - desc
+          description: Order direction ('asc' or 'desc')
+          example: desc
+    PluginStatus:
+      type: object
+      properties:
+        installed:
+          type: boolean
+          description: Is the plugin installed
+          example: true
+        update_available:
+          type: boolean
+          description: Does the plugin have an update available
+          example: true
+    PluginsTableResults:
       type: object
-    PluginFlowDataResults:
       properties:
         plugin_id:
+          type: string
           description: The plugin ID
           example: encoder_video_h264_nvenc
-          type: string
         name:
+          type: string
           description: The plugin name
           example: Video Encoder H264 - h264_nvenc
-          type: string
         author:
+          type: string
           description: The plugin author
           example: encoder_video_h264_nvenc
-          type: string
         description:
+          type: string
           description: The plugin description
           example: Ensure all video streams are encoded with the H264 codec using
             the h264_nvenc encoder.
-          type: string
         version:
+          type: string
           description: The plugin version
           example: Josh.5
-          type: string
         icon:
+          type: string
           description: The plugin icon
           example: https://raw.githubusercontent.com/Josh5/unmanic-plugins/master/source/encoder_video_h264_nvenc/icon.png
+        tags:
           type: string
+          description: The plugin tags
+          example: video,encoder,ffmpeg,worker,nvenc,nvdec,nvidia
+        status:
+          description: The plugin status
+          allOf:
+          - $ref: '#/components/schemas/PluginStatus'
+        changelog:
+          type: string
+          description: The plugin changelog
+          example: "[b][color=56adda]0.0.1[/color][/b]\u2022 initial version"
+        has_config:
+          type: boolean
+          description: The plugin has the ability to be configured
+          example: true
+        id:
+          type: integer
+          description: Item table ID
+          example: 1
       required:
       - author
       - description
       - icon
+      - id
       - name
       - plugin_id
+      - status
+      - tags
       - version
+    PluginsData:
       type: object
-    PluginReposListResults:
       properties:
-        repos:
-          description: Results
-          items:
-            $ref: '#/components/schemas/PluginReposMetadataResults'
+        recordsTotal:
+          type: integer
+          description: Total number of records in this table
+          example: 329
+        recordsFiltered:
+          type: integer
+          default: 10
+          description: Total number of records after filters have been applied
+          example: 10
+        results:
           minItems: 0
+          description: Results
           type: array
+          items:
+            $ref: '#/components/schemas/PluginsTableResults'
       required:
-      - repos
+      - results
+    RequestPluginsInfo:
       type: object
-    PluginReposMetadataResults:
       properties:
-        id:
-          description: The plugin repo ID
-          example: repository.josh5
-          type: string
-        name:
-          description: The plugin repo name
-          example: Josh.5 Development Plugins for Unmanic
-          type: string
-        icon:
-          description: The plugin repo icon
-          example: https://raw.githubusercontent.com/Josh5/unmanic-plugins/master/icon.png
+        plugin_id:
           type: string
-        path:
-          description: The plugin repo URL path
-          example: https://raw.githubusercontent.com/Josh5/unmanic-plugins/repo/repo.json
+          example: encoder_video_hevc_vaapi
+        repo_id:
           type: string
-      required:
-      - icon
-      - id
-      - name
-      - path
-      type: object
-    PluginStatus:
-      properties:
-        installed:
-          description: Is the plugin installed
-          example: true
+          description: The ID of the repository that this plugin is in
+          example: '158899500680826593283708490873332175078'
+        prefer_local:
           type: boolean
-        update_available:
-          description: Does the plugin have an update available
+          default: true
           example: true
-          type: boolean
-      type: object
-    PluginTypesResults:
-      properties:
-        results:
-          description: List of Plugin Type IDs supported by this installation
-          example:
-          - library_management.file_test
-          - postprocessor.file_move
-          - postprocessor.task_result
-          - worker.process_item
-          items:
-            type: string
-          type: array
+        library_id:
+          type: integer
+          default: 0
+          example: 1
       required:
-      - results
-      type: object
+      - plugin_id
     PluginsConfigInputItem:
+      type: object
       properties:
         key_id:
+          type: string
           description: The config input base64 encoded key (used for linking keys
             containing spaces, etc.)
           example: c8f122656ed2acabde9b57101a4c8ec7
-          type: string
         key:
+          type: string
           description: The config input key or name
           example: downmix_dts_hd_ma
-          type: string
         value:
           description: The current value of this config input
           example: false
         input_type:
+          type: string
           description: The config input type
           example: checkbox
-          type: string
         label:
+          type: string
           description: The label used to define this config input
           example: Downmix DTS-HD Master Audio (max 5.1 channels)?
+        description:
           type: string
+          nullable: true
+          description: Description of input field
+          example: 'Will automatically downmix DTS-HD Master Audio to 5.1 channels '
+        tooltip:
+          type: string
+          nullable: true
+          description: Description of input field
+          example: 'Will automatically downmix DTS-HD Master Audio to 5.1 channels '
         select_options:
+          type: array
           description: Additional options if the input_type is set to 'select'
           example:
-          - label: First Option
-            value: first
-          - label: Second Option
-            value: second
+          - value: first
+            label: First Option
+          - value: second
+            label: Second Option
           items:
             type: object
-          type: array
         slider_options:
+          type: object
           description: Additional options if the input_type is set to 'slider'
           example:
-            max: 8
             min: 1
+            max: 8
             suffix: M
-          type: object
         display:
+          type: string
           description: Should the setting input be displayed (visible, hidden)
           example: visible
-          type: string
+        sub_setting:
+          type: boolean
+          description: Should the setting be a nested sub-setting field
+          example: false
       required:
+      - description
       - display
       - input_type
       - key
       - key_id
       - label
       - select_options
       - slider_options
+      - sub_setting
+      - tooltip
       - value
-      type: object
-    PluginsData:
-      properties:
-        recordsTotal:
-          description: Total number of records in this table
-          example: 329
-          type: integer
-        recordsFiltered:
-          default: 10
-          description: Total number of records after filters have been applied
-          example: 10
-          type: integer
-        results:
-          description: Results
-          items:
-            $ref: '#/components/schemas/PluginsTableResults'
-          minItems: 0
-          type: array
-      required:
-      - results
-      type: object
-    PluginsDataPanelTypesData:
-      properties:
-        results:
-          description: Results
-          items:
-            $ref: '#/components/schemas/PluginFlowDataResults'
-          minItems: 0
-          type: array
-      required:
-      - results
-      type: object
     PluginsInfoResults:
+      type: object
       properties:
         plugin_id:
+          type: string
           description: The plugin ID
           example: encoder_video_h264_nvenc
-          type: string
         name:
+          type: string
           description: The plugin name
           example: Video Encoder H264 - h264_nvenc
-          type: string
         author:
+          type: string
           description: The plugin author
           example: encoder_video_h264_nvenc
-          type: string
         description:
+          type: string
           description: The plugin description
           example: Ensure all video streams are encoded with the H264 codec using
             the h264_nvenc encoder.
-          type: string
         version:
+          type: string
           description: The plugin version
           example: Josh.5
-          type: string
         icon:
+          type: string
           description: The plugin icon
           example: https://raw.githubusercontent.com/Josh5/unmanic-plugins/master/source/encoder_video_h264_nvenc/icon.png
-          type: string
         tags:
+          type: string
           description: The plugin tags
           example: video,encoder,ffmpeg,worker,nvenc,nvdec,nvidia
-          type: string
         status:
+          description: The plugin status
           allOf:
           - $ref: '#/components/schemas/PluginStatus'
-          description: The plugin status
         changelog:
+          type: string
           description: The plugin changelog
           example: "[b][color=56adda]0.0.1[/color][/b]\u2022 initial version"
-          type: string
         has_config:
+          type: boolean
           description: The plugin has the ability to be configured
           example: true
-          type: boolean
         settings:
           description: The plugin settings
+          type: array
           items:
             $ref: '#/components/schemas/PluginsConfigInputItem'
-          type: array
       required:
       - author
       - description
       - icon
       - name
       - plugin_id
       - status
       - tags
       - version
+    RequestPluginsSettingsSave:
       type: object
-    PluginsInstallableResults:
       properties:
-        plugins:
-          description: Results
-          items:
-            $ref: '#/components/schemas/PluginsMetadataInstallableResults'
-          minItems: 0
+        plugin_id:
+          type: string
+          example: encoder_video_hevc_vaapi
+        settings:
+          description: The plugin settings
           type: array
+          items:
+            $ref: '#/components/schemas/PluginsConfigInputItem'
+        library_id:
+          type: integer
+          default: 0
+          example: 1
       required:
-      - plugins
+      - plugin_id
+      - settings
+    RequestPluginsSettingsReset:
       type: object
+      properties:
+        plugin_id:
+          type: string
+          example: encoder_video_hevc_vaapi
+        library_id:
+          type: integer
+          default: 0
+          example: 1
+      required:
+      - plugin_id
     PluginsMetadataInstallableResults:
+      type: object
       properties:
         plugin_id:
+          type: string
           description: The plugin ID
           example: encoder_video_h264_nvenc
-          type: string
         name:
+          type: string
           description: The plugin name
           example: Video Encoder H264 - h264_nvenc
-          type: string
         author:
+          type: string
           description: The plugin author
           example: encoder_video_h264_nvenc
-          type: string
         description:
+          type: string
           description: The plugin description
           example: Ensure all video streams are encoded with the H264 codec using
             the h264_nvenc encoder.
-          type: string
         version:
+          type: string
           description: The plugin version
           example: Josh.5
-          type: string
         icon:
+          type: string
           description: The plugin icon
           example: https://raw.githubusercontent.com/Josh5/unmanic-plugins/master/source/encoder_video_h264_nvenc/icon.png
-          type: string
         tags:
+          type: string
           description: The plugin tags
           example: video,encoder,ffmpeg,worker,nvenc,nvdec,nvidia
-          type: string
         status:
+          description: The plugin status
           allOf:
           - $ref: '#/components/schemas/PluginStatus'
-          description: The plugin status
         changelog:
+          type: string
           description: The plugin changelog
           example: "[b][color=56adda]0.0.1[/color][/b]\u2022 initial version"
-          type: string
         has_config:
+          type: boolean
           description: The plugin has the ability to be configured
           example: true
-          type: boolean
         package_url:
+          type: string
           description: The plugin package download URL
           example: https://raw.githubusercontent.com/Unmanic/unmanic-plugins/repo/plugin_id/plugin_id-1.0.0.zip
-          type: string
         changelog_url:
+          type: string
           description: The plugin package download URL
           example: https://raw.githubusercontent.com/Unmanic/unmanic-plugins/repo/plugin_id/changelog.md
-          type: string
         repo_name:
+          type: string
           description: The name of the repository that this plugin is in
           example: Official Repo
-          type: string
         repo_id:
+          type: string
           description: The ID of the repository that this plugin is in
           example: '158899500680826593283708490873332175078'
-          type: string
       required:
       - author
       - description
       - icon
       - name
       - plugin_id
       - status
       - tags
       - version
+    PluginsInstallableResults:
+      type: object
+      properties:
+        plugins:
+          minItems: 0
+          description: Results
+          type: array
+          items:
+            $ref: '#/components/schemas/PluginsMetadataInstallableResults'
+      required:
+      - plugins
+    RequestPluginsById:
+      type: object
+      properties:
+        plugin_id:
+          type: string
+          example: encoder_video_hevc_vaapi
+        repo_id:
+          type: string
+          description: The ID of the repository that this plugin is in
+          example: '158899500680826593283708490873332175078'
+      required:
+      - plugin_id
+    RequestPluginsFlowByPluginType:
+      type: object
+      properties:
+        plugin_type:
+          type: string
+          example: library_management.file_test
+        library_id:
+          type: integer
+          default: 1
+          example: 1
+      required:
+      - plugin_type
+    PluginTypesResults:
+      type: object
+      properties:
+        results:
+          type: array
+          description: List of Plugin Type IDs supported by this installation
+          example:
+          - library_management.file_test
+          - postprocessor.file_move
+          - postprocessor.task_result
+          - worker.process_item
+          items:
+            type: string
+      required:
+      - results
+    PluginFlowDataResults:
       type: object
-    PluginsTableResults:
       properties:
         plugin_id:
+          type: string
           description: The plugin ID
           example: encoder_video_h264_nvenc
-          type: string
         name:
+          type: string
           description: The plugin name
           example: Video Encoder H264 - h264_nvenc
-          type: string
         author:
+          type: string
           description: The plugin author
           example: encoder_video_h264_nvenc
-          type: string
         description:
+          type: string
           description: The plugin description
           example: Ensure all video streams are encoded with the H264 codec using
             the h264_nvenc encoder.
-          type: string
         version:
+          type: string
           description: The plugin version
           example: Josh.5
-          type: string
         icon:
+          type: string
           description: The plugin icon
           example: https://raw.githubusercontent.com/Josh5/unmanic-plugins/master/source/encoder_video_h264_nvenc/icon.png
-          type: string
-        tags:
-          description: The plugin tags
-          example: video,encoder,ffmpeg,worker,nvenc,nvdec,nvidia
-          type: string
-        status:
-          allOf:
-          - $ref: '#/components/schemas/PluginStatus'
-          description: The plugin status
-        changelog:
-          description: The plugin changelog
-          example: "[b][color=56adda]0.0.1[/color][/b]\u2022 initial version"
-          type: string
-        has_config:
-          description: The plugin has the ability to be configured
-          example: true
-          type: boolean
-        id:
-          description: Item table ID
-          example: 1
-          type: integer
       required:
       - author
       - description
       - icon
-      - id
       - name
       - plugin_id
-      - status
-      - tags
       - version
+    RequestSavingPluginsFlowByPluginType:
       type: object
-    RequestAddCompletedToPendingTasks:
       properties:
-        id_list:
-          description: List of table IDs
-          example: &id003 []
-          items:
-            type: integer
-          minItems: 1
-          type: array
+        plugin_type:
+          type: string
+          example: library_management.file_test
         library_id:
-          default: 0
-          example: 1
           type: integer
-      required:
-      - id_list
-      type: object
-    RequestDatabaseItemById:
-      properties:
-        id:
-          description: The ID of the table item
+          default: 1
           example: 1
-          type: integer
+        plugin_flow:
+          minItems: 1
+          description: Saved flow
+          type: array
+          items:
+            $ref: '#/components/schemas/PluginFlowDataResults'
       required:
-      - id
-      type: object
-    RequestDirectoryListingData:
-      properties:
-        current_path:
-          default: /
-          example: /
-          type: string
-        list_type:
-          default: all
-          example: directories
-          type: string
-      type: object
-    RequestHistoryTableData:
-      properties:
-        start:
-          default: 0
-          description: Start row number to select from
-          example: 0
-          type: integer
-        length:
-          default: 10
-          description: Number of rows to select
-          example: 10
-          type: integer
-        search_value:
-          default: ''
-          description: String to filter search results by
-          example: items with this text in the value
-          type: string
-        status:
-          default: all
-          description: Filter on the status
-          example: all
-          type: string
-        after:
-          description: Filter entries since datetime
-          example: 2022-04-07 01:45
-          format: date-time
-          nullable: true
-          type: string
-        before:
-          description: Filter entries prior to datetime
-          example: 2022-04-07 01:55
-          format: date-time
-          nullable: true
-          type: string
-        order_by:
-          default: finish_time
-          example: finish_time
-          type: string
-        order_direction:
-          description: Order direction ('asc' or 'desc')
-          enum:
-          - asc
-          - desc
-          example: desc
-          type: string
+      - plugin_flow
+      - plugin_type
+    RequestUpdatePluginReposList:
       type: object
-    RequestLibraryById:
       properties:
-        id:
-          description: The ID of the library
-          example: 1
-          type: integer
+        repos_list:
+          type: array
+          minItems: 0
+          description: A list of repost to save
+          example:
+          - https://raw.githubusercontent.com/Josh5/unmanic-plugins/repo/repo.json
+          items:
+            type: string
       required:
-      - id
+      - repos_list
+    PluginReposMetadataResults:
       type: object
-    RequestPendingTableData:
       properties:
-        start:
-          default: 0
-          description: Start row number to select from
-          example: 0
-          type: integer
-        length:
-          default: 10
-          description: Number of rows to select
-          example: 10
-          type: integer
-        search_value:
-          default: ''
-          description: String to filter search results by
-          example: items with this text in the value
-          type: string
-        status:
-          default: all
-          description: Filter on the status
-          example: all
-          type: string
-        after:
-          description: Filter entries since datetime
-          example: 2022-04-07 01:45
-          format: date-time
-          nullable: true
-          type: string
-        before:
-          description: Filter entries prior to datetime
-          example: 2022-04-07 01:55
-          format: date-time
-          nullable: true
+        id:
           type: string
-        order_by:
-          default: priority
-          example: priority
+          description: The plugin repo ID
+          example: repository.josh5
+        name:
           type: string
-        order_direction:
-          description: Order direction ('asc' or 'desc')
-          enum:
-          - asc
-          - desc
-          example: desc
+          description: The plugin repo name
+          example: Josh.5 Development Plugins for Unmanic
+        icon:
           type: string
-      type: object
-    RequestPendingTaskCreate:
-      properties:
+          description: The plugin repo icon
+          example: https://raw.githubusercontent.com/Josh5/unmanic-plugins/master/icon.png
         path:
-          description: The absolute path to a file
-          example: /library/TEST_FILE.mkv
-          type: string
-        library_id:
-          description: The ID of the library to append this task to
-          example: 1
-          type: integer
-        library_name:
-          description: The name of the library to append this task to
-          example: Default
           type: string
-        type:
-          description: The type of pending task to create (local/remote)
-          example: local
-          type: string
-        priority_score:
-          description: Apply a priority score to the created task to either increase
-            or decrease its position in the queue
-          example: 1000
-          type: integer
+          description: The plugin repo URL path
+          example: https://raw.githubusercontent.com/Josh5/unmanic-plugins/repo/repo.json
       required:
+      - icon
+      - id
+      - name
       - path
+    PluginReposListResults:
       type: object
-    RequestPendingTasksLibraryUpdate:
       properties:
-        id_list:
-          description: List of table IDs
-          example: *id003
-          items:
-            type: integer
-          minItems: 1
+        repos:
+          minItems: 0
+          description: Results
           type: array
-        library_name:
-          example: Default
-          type: string
-      required:
-      - id_list
-      - library_name
-      type: object
-    RequestPendingTasksReorder:
-      properties:
-        id_list:
-          description: List of table IDs
-          example: *id003
           items:
-            type: integer
-          minItems: 1
-          type: array
-        position:
-          description: Position to move given list of items to ('top' or 'bottom')
-          enum:
-          - top
-          - bottom
-          example: top
-          type: string
-      required:
-      - id_list
-      - position
-      type: object
-    RequestPluginsById:
-      properties:
-        plugin_id:
-          example: encoder_video_hevc_vaapi
-          type: string
-        repo_id:
-          description: The ID of the repository that this plugin is in
-          example: '158899500680826593283708490873332175078'
-          type: string
-      required:
-      - plugin_id
-      type: object
-    RequestPluginsFlowByPluginType:
-      properties:
-        plugin_type:
-          example: library_management.file_test
-          type: string
-        library_id:
-          default: 1
-          example: 1
-          type: integer
-      required:
-      - plugin_type
-      type: object
-    RequestPluginsInfo:
-      properties:
-        plugin_id:
-          example: encoder_video_hevc_vaapi
-          type: string
-        repo_id:
-          description: The ID of the repository that this plugin is in
-          example: '158899500680826593283708490873332175078'
-          type: string
-        prefer_local:
-          default: true
-          example: true
-          type: boolean
-        library_id:
-          default: 0
-          example: 1
-          type: integer
-      required:
-      - plugin_id
-      type: object
-    RequestPluginsSettingsReset:
-      properties:
-        plugin_id:
-          example: encoder_video_hevc_vaapi
-          type: string
-        library_id:
-          default: 0
-          example: 1
-          type: integer
+            $ref: '#/components/schemas/PluginReposMetadataResults'
       required:
-      - plugin_id
+      - repos
+    PluginsDataPanelTypesData:
       type: object
-    RequestPluginsSettingsSave:
       properties:
-        plugin_id:
-          example: encoder_video_hevc_vaapi
-          type: string
-        settings:
-          description: The plugin settings
-          items:
-            $ref: '#/components/schemas/PluginsConfigInputItem'
+        results:
+          minItems: 0
+          description: Results
           type: array
-        library_id:
-          default: 0
-          example: 1
-          type: integer
+          items:
+            $ref: '#/components/schemas/PluginFlowDataResults'
       required:
-      - plugin_id
-      - settings
+      - results
+    SessionStateSuccess:
       type: object
-    RequestPluginsTableData:
       properties:
-        start:
-          default: 0
-          description: Start row number to select from
-          example: 0
-          type: integer
-        length:
-          default: 10
-          description: Number of rows to select
-          example: 10
+        level:
           type: integer
-        search_value:
-          default: ''
-          description: String to filter search results by
-          example: items with this text in the value
-          type: string
-        status:
-          default: all
-          description: Filter on the status
-          example: all
-          type: string
-        after:
-          description: Filter entries since datetime
-          example: 2022-04-07 01:45
-          format: date-time
-          nullable: true
-          type: string
-        before:
-          description: Filter entries prior to datetime
-          example: 2022-04-07 01:55
-          format: date-time
-          nullable: true
+          description: User level
+          example: 0
+        picture_uri:
           type: string
-        order_by:
-          default: name
-          example: name
+          description: User picture
+          example: https://c8.patreon.com/2/200/561356054
+        name:
           type: string
-        order_direction:
-          description: Order direction ('asc' or 'desc')
-          enum:
-          - asc
-          - desc
-          example: desc
+          description: User name
+          example: ExampleUsername123
+        email:
           type: string
-      type: object
-    RequestRemoteInstallationLinkConfig:
-      properties:
+          description: User email
+          example: example@gmail.com
+        created:
+          type: number
+          description: Session time created
+          example: 1627793093.676484
         uuid:
-          description: The uuid of the remote installation
-          example: 7cd35429-76ab-4a29-8649-8c91236b5f8b
           type: string
+          description: Installation uuid
+          example: b429fcc7-9ce1-bcb3-2b8a-b094747f226e
       required:
+      - level
       - uuid
+    SettingsReadAndWrite:
       type: object
-    RequestSavingPluginsFlowByPluginType:
       properties:
-        plugin_type:
-          example: library_management.file_test
-          type: string
-        library_id:
-          default: 1
-          example: 1
-          type: integer
-        plugin_flow:
-          description: Saved flow
-          items:
-            $ref: '#/components/schemas/PluginFlowDataResults'
-          minItems: 1
-          type: array
+        settings:
+          type: object
+          description: The current settings
+          example:
+            ui_port: 8888
+            debugging: false
+            library_path: /library
+            enable_library_scanner: false
+            schedule_full_scan_minutes: 1440
+            follow_symlinks: true
+            run_full_scan_on_start: false
+            cache_path: /tmp/unmanic
       required:
-      - plugin_flow
-      - plugin_type
+      - settings
+    SettingsSystemConfig:
       type: object
+      properties:
+        configuration:
+          type: object
+          description: The current system configuration
+          example: {}
+      required:
+      - configuration
     RequestSettingsRemoteInstallationAddressValidation:
+      type: object
       properties:
         address:
+          type: string
           description: The address of the remote installation
           example: 192.168.1.2:8888
-          type: string
         auth:
+          type: string
+          nullable: true
           description: Authentication type
           example: Basic
-          nullable: true
-          type: string
         username:
+          type: string
+          nullable: true
           description: An optional username
           example: foo
-          nullable: true
-          type: string
         password:
+          type: string
+          nullable: true
           description: An optional password
           example: bar
-          nullable: true
-          type: string
       required:
       - address
+    SettingsRemoteInstallationData:
       type: object
-    RequestTableUpdateByIdList:
       properties:
-        id_list:
-          description: List of table IDs
-          example: *id003
-          items:
-            type: integer
-          minItems: 1
-          type: array
+        installation:
+          type: object
+          description: The data from the remote installation
+          example: {}
       required:
-      - id_list
+      - installation
+    WorkerEventScheduleResults:
       type: object
-    RequestUpdatePluginReposList:
       properties:
-        repos_list:
-          description: A list of repost to save
+        repetition:
+          type: string
+          description: ''
+          example: daily
+        schedule_task:
+          type: string
+          description: The type of task. ['count', 'pause', 'resume']
+          example: count
+        schedule_time:
+          type: string
+          description: ''
+          example: The time when the task should be executed on
+        schedule_worker_count:
+          type: integer
+          description: The worker count to set (only valid if schedule_task is count)
+          example: 4
+      required:
+      - repetition
+      - schedule_task
+      - schedule_time
+    SettingsWorkerGroupConfig:
+      type: object
+      properties:
+        id:
+          type: integer
+          nullable: true
+          description: ''
+          example: 1
+        locked:
+          type: boolean
+          description: If the worker group is locked and cannot be deleted
+          example: false
+        name:
+          type: string
+          description: The name of the worker group
+          example: Default Group
+        number_of_workers:
+          type: integer
+          description: The number of workers in this group
+          example: 3
+        worker_event_schedules:
+          minItems: 0
+          description: Any scheduled evenets for this worker group
+          type: array
+          items:
+            $ref: '#/components/schemas/WorkerEventScheduleResults'
+        tags:
+          type: array
+          description: A list of tags associated with this worker
           example:
-          - https://raw.githubusercontent.com/Josh5/unmanic-plugins/repo/repo.json
+          - GPU
+          - priority
           items:
             type: string
+      required:
+      - id
+      - locked
+      - name
+      - number_of_workers
+      - tags
+      - worker_event_schedules
+    WorkerGroupsList:
+      type: object
+      properties:
+        worker_groups:
           minItems: 0
+          description: Results
           type: array
+          items:
+            $ref: '#/components/schemas/SettingsWorkerGroupConfig'
       required:
-      - repos_list
+      - worker_groups
+    RequestDatabaseItemById:
       type: object
-    RequestWorkerById:
       properties:
-        worker_id:
-          example: '1'
+        id:
+          type: integer
+          description: The ID of the table item
+          example: 1
+      required:
+      - id
+    RequestRemoteInstallationLinkConfig:
+      type: object
+      properties:
+        uuid:
           type: string
+          description: The uuid of the remote installation
+          example: 7cd35429-76ab-4a29-8649-8c91236b5f8b
       required:
-      - worker_id
+      - uuid
+    SettingsRemoteInstallationLinkConfig:
       type: object
-    SessionStateSuccess:
       properties:
-        level:
-          description: User level
-          example: 0
+        link_config:
+          type: object
+          description: The configuration for the remote installation link
+          example:
+            address: 10.0.0.2:8888
+            auth: None
+            username: ''
+            password: ''
+            available: true
+            name: API schema generated
+            version: 0.1.3
+            last_updated: 1636166593.013826
+            enable_receiving_tasks: false
+            enable_sending_tasks: false
+            enable_task_preloading: true
+            enable_distributed_worker_count: false
+            preloading_count: 2
+            enable_checksum_validation: false
+            enable_config_missing_libraries: false
+        distributed_worker_count_target:
           type: integer
-        picture_uri:
-          description: User picture
-          example: https://c8.patreon.com/2/200/561356054
-          type: string
+          description: The target count of workers to be distributed across any configured
+            linked installations
+          example: 4
+      required:
+      - link_config
+    LibraryResults:
+      type: object
+      properties:
+        id:
+          type: integer
+          description: ''
+          example: 1
         name:
-          description: User name
-          example: ExampleUsername123
           type: string
-        email:
-          description: User email
-          example: example@gmail.com
-          type: string
-        created:
-          description: Session time created
-          example: 1627793093.676484
-          type: number
-        uuid:
-          description: Installation uuid
-          example: b429fcc7-9ce1-bcb3-2b8a-b094747f226e
+          description: The name of the library
+          example: Default
+        path:
           type: string
+          description: The library path
+          example: /library
+        locked:
+          type: boolean
+          description: If the library is locked and cannot be deleted
+          example: false
+        enable_remote_only:
+          type: boolean
+          description: If the library is configured for remote files only
+          example: false
+        enable_scanner:
+          type: boolean
+          description: If the library is configured to execute library scans
+          example: false
+        enable_inotify:
+          type: boolean
+          description: If the library is configured to monitor for file changes
+          example: false
+        tags:
+          type: array
+          description: A list of tags associated with this library
+          example:
+          - GPU
+          - priority
+          items:
+            type: string
       required:
-      - level
-      - uuid
-      type: object
+      - enable_inotify
+      - enable_remote_only
+      - enable_scanner
+      - id
+      - locked
+      - name
+      - path
+      - tags
     SettingsLibrariesList:
+      type: object
       properties:
         libraries:
+          minItems: 1
           description: Results
+          type: array
           items:
             $ref: '#/components/schemas/LibraryResults'
-          minItems: 1
-          type: array
       required:
       - libraries
+    RequestLibraryById:
       type: object
+      properties:
+        id:
+          type: integer
+          description: The ID of the library
+          example: 1
+      required:
+      - id
     SettingsLibraryConfigReadAndWrite:
+      type: object
       properties:
         library_config:
+          type: object
           description: The library configuration
           example:
-            enable_inotify: false
-            enable_scanner: false
             id: 1
             name: Default
             path: /library
+            enable_scanner: false
+            enable_inotify: false
             priority_score: 0
             tags: []
-          type: object
         plugins:
+          type: object
           description: The library's enabled plugins
           example:
             enabled_plugins:
-            - description: Notify Plex on completion of a task.
-              icon: https://raw.githubusercontent.com/Josh5/unmanic.plugin.notify_plex/master/icon.png
-              library_id: 1
-              name: Notify Plex
+            - library_id: 1
               plugin_id: notify_plex
-          type: object
+              name: Notify Plex
+              description: Notify Plex on completion of a task.
+              icon: https://raw.githubusercontent.com/Josh5/unmanic.plugin.notify_plex/master/icon.png
       required:
       - library_config
-      type: object
     SettingsLibraryPluginConfigExport:
+      type: object
       properties:
         plugins:
+          type: object
           description: The library's enabled plugins
           example: &id004
             enabled_plugins:
-            - description: Ensure all audio streams are encoded with the AC3 codec
+            - library_id: 1
+              plugin_id: encoder_audio_ac3
+              name: Audio Encoder AC3
+              description: Ensure all audio streams are encoded with the AC3 codec
                 using the native FFmpeg ac3 encoder.
               icon: https://raw.githubusercontent.com/Josh5/unmanic.plugin.encoder_audio_ac3/master/icon.png
-              library_id: 1
-              name: Audio Encoder AC3
-              plugin_id: encoder_audio_ac3
             plugin_flow:
               library_management.file_test:
-              - author: Josh.5
+              - plugin_id: encoder_audio_ac3
+                name: Audio Encoder AC3
+                author: Josh.5
                 description: Ensure all audio streams are encoded with the AC3 codec
                   using the native FFmpeg ac3 encoder.
-                icon: https://raw.githubusercontent.com/Josh5/unmanic.plugin.encoder_audio_ac3/master/icon.png
-                name: Audio Encoder AC3
-                plugin_id: encoder_audio_ac3
                 version: 0.0.2
-              postprocessor.file_move: []
-              postprocessor.task_result: []
+                icon: https://raw.githubusercontent.com/Josh5/unmanic.plugin.encoder_audio_ac3/master/icon.png
               worker.process_item:
-              - author: Josh.5
+              - plugin_id: encoder_audio_ac3
+                name: Audio Encoder AC3
+                author: Josh.5
                 description: Ensure all audio streams are encoded with the AC3 codec
                   using the native FFmpeg ac3 encoder.
-                icon: https://raw.githubusercontent.com/Josh5/unmanic.plugin.encoder_audio_ac3/master/icon.png
-                name: Audio Encoder AC3
-                plugin_id: encoder_audio_ac3
                 version: 0.0.2
-          type: object
+                icon: https://raw.githubusercontent.com/Josh5/unmanic.plugin.encoder_audio_ac3/master/icon.png
+              postprocessor.file_move: []
+              postprocessor.task_result: []
         library_config:
+          type: object
           description: The library configuration
           example: &id005
-            enable_inotify: false
-            enable_scanner: false
             id: 1
             name: Default
             path: /library
+            enable_scanner: false
+            enable_inotify: false
             priority_score: 0
             tags: []
-          type: object
       required:
       - plugins
-      type: object
     SettingsLibraryPluginConfigImport:
+      type: object
       properties:
         plugins:
+          type: object
           description: The library's enabled plugins
           example: *id004
-          type: object
         library_config:
+          type: object
           description: The library configuration
           example: *id005
-          type: object
         library_id:
-          example: 1
           type: integer
+          example: 1
       required:
       - library_id
       - plugins
-      type: object
-    SettingsReadAndWrite:
-      properties:
-        settings:
-          description: The current settings
-          example:
-            cache_path: /tmp/unmanic
-            debugging: false
-            enable_library_scanner: false
-            follow_symlinks: true
-            library_path: /library
-            run_full_scan_on_start: false
-            schedule_full_scan_minutes: 1440
-            ui_port: 8888
-          type: object
-      required:
-      - settings
-      type: object
-    SettingsRemoteInstallationData:
-      properties:
-        installation:
-          description: The data from the remote installation
-          example: {}
-          type: object
-      required:
-      - installation
-      type: object
-    SettingsRemoteInstallationLinkConfig:
-      properties:
-        link_config:
-          description: The configuration for the remote installation link
-          example:
-            address: 10.0.0.2:8888
-            auth: None
-            available: true
-            enable_checksum_validation: false
-            enable_config_missing_libraries: false
-            enable_distributed_worker_count: false
-            enable_receiving_tasks: false
-            enable_sending_tasks: false
-            enable_task_preloading: true
-            last_updated: 1636166593.013826
-            name: API schema generated
-            password: ''
-            preloading_count: 2
-            username: ''
-            version: 0.1.3
-          type: object
-        distributed_worker_count_target:
-          description: The target count of workers to be distributed across any configured
-            linked installations
-          example: 4
-          type: integer
-      required:
-      - link_config
-      type: object
-    SettingsSystemConfig:
-      properties:
-        configuration:
-          description: The current system configuration
-          example: {}
-          type: object
-      required:
-      - configuration
-      type: object
-    SettingsWorkerGroupConfig:
-      properties:
-        id:
-          description: ''
-          example: 1
-          nullable: true
-          type: integer
-        locked:
-          description: If the worker group is locked and cannot be deleted
-          example: false
-          type: boolean
-        name:
-          description: The name of the worker group
-          example: Default Group
-          type: string
-        number_of_workers:
-          description: The number of workers in this group
-          example: 3
-          type: integer
-        worker_event_schedules:
-          description: Any scheduled evenets for this worker group
-          items:
-            $ref: '#/components/schemas/WorkerEventScheduleResults'
-          minItems: 0
-          type: array
-        tags:
-          description: A list of tags associated with this worker
-          example:
-          - GPU
-          - priority
-          items:
-            type: string
-          type: array
-      required:
-      - id
-      - locked
-      - name
-      - number_of_workers
-      - tags
-      - worker_event_schedules
-      type: object
-    TaskDownloadLink:
-      properties:
-        link_id:
-          description: The ID used to download the file /unmanic/downloads/{link_id}
-          example: 2960645c-a4e2-4b05-8866-7bd469ee9ef8
-          type: string
-      required:
-      - link_id
-      type: object
     VersionReadSuccess:
+      type: object
       properties:
         version:
+          type: string
           description: Application version
           example: 1.0.0
-          type: string
       required:
       - version
+    RequestWorkerById:
       type: object
-    WorkerEventScheduleResults:
       properties:
-        repetition:
-          description: ''
-          example: daily
-          type: string
-        schedule_task:
-          description: The type of task. ['count', 'pause', 'resume']
-          example: count
-          type: string
-        schedule_time:
-          description: ''
-          example: The time when the task should be executed on
+        worker_id:
           type: string
-        schedule_worker_count:
-          description: The worker count to set (only valid if schedule_task is count)
-          example: 4
-          type: integer
-      required:
-      - repetition
-      - schedule_task
-      - schedule_time
-      type: object
-    WorkerGroupsList:
-      properties:
-        worker_groups:
-          description: Results
-          items:
-            $ref: '#/components/schemas/SettingsWorkerGroupConfig'
-          minItems: 0
-          type: array
+          example: '1'
       required:
-      - worker_groups
-      type: object
+      - worker_id
     WorkerStatusResults:
+      type: object
       properties:
         id:
+          type: string
           description: ''
           example: W0
-          type: string
         name:
+          type: string
           description: ''
           example: Worker-W0
-          type: string
         idle:
+          type: boolean
           description: Flag - is worker idle
           example: true
-          type: boolean
         paused:
+          type: boolean
           description: Flag - is worker paused
           example: false
-          type: boolean
         start_time:
+          type: string
+          nullable: true
           description: The time when this worker started processing a task
           example: '1635746377.0021548'
-          nullable: true
-          type: string
         current_file:
+          type: string
           description: The basename of the file currently being processed
           example: file.mp4
-          type: string
         current_task:
+          type: integer
+          nullable: true
           description: The Task ID
           example: 1
-          nullable: true
-          type: integer
         worker_log_tail:
+          type: array
+          minItems: 0
           description: The log lines produced by the worker
           example:
           - "\n\nRUNNER: \nRemux Video Files [Pass #1]\n\n"
           - '
 
             Executing plugin runner... Please wait'
           - '
@@ -1432,2473 +1521,2580 @@
             Runner did not request to execute a command'
           - '
 
 
             No Plugin requested to run commands for this file ''/tmp/unmanic/unmanic_remote_pending_library-1635746225.3336523/file.mp4'''
           items:
             type: string
-          minItems: 0
-          type: array
         runners_info:
+          type: object
           description: The status of the plugin runner currently processing the file
           example:
             video_remuxer:
-              author: Josh.5
-              description: Remux a video file to the configured container
-              icon: https://raw.githubusercontent.com/Josh5/unmanic.plugin.video_remuxer/master/icon.png
-              name: Remux Video Files
               plugin_id: video_remuxer
               status: complete
-              success: true
+              name: Remux Video Files
+              author: Josh.5
               version: 0.0.5
-          type: object
+              icon: https://raw.githubusercontent.com/Josh5/unmanic.plugin.video_remuxer/master/icon.png
+              description: Remux a video file to the configured container
+              success: true
         subprocess:
+          type: object
           description: The status of the process currently being executed
           example:
-            elapsed: None
-            percent: None
             pid: 140408939493120
-          type: object
+            percent: None
+            elapsed: None
       required:
       - current_file
       - current_task
       - id
       - idle
       - name
       - paused
       - runners_info
       - start_time
       - subprocess
       - worker_log_tail
-      type: object
     WorkerStatusSuccess:
+      type: object
       properties:
         workers_status:
+          minItems: 0
           description: Results
+          type: array
           items:
             $ref: '#/components/schemas/WorkerStatusResults'
-          minItems: 0
-          type: array
       required:
       - workers_status
-      type: object
-  securitySchemes:
-    BasicAuth:
-      scheme: basic
-      type: http
-info:
-  description: Documentation for the Unmanic application API
-  title: Unmanic API
-  version: '2'
-openapi: 3.0.0
+security:
+- BasicAuth: []
 paths:
   /docs/privacypolicy:
     get:
       description: Returns the privacy policy.
       responses:
         '200':
+          description: 'Sample response: Returns the privacy policy.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/DocumentContentSuccess'
-          description: 'Sample response: Returns the privacy policy.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /docs/logs/zip:
     get:
       description: Returns the all log files as zip.
       responses:
         '200':
+          description: 'Sample response: Returns the all log files as zip.'
           content:
             application/octet-stream:
               schema:
-                format: binary
                 type: string
-          description: 'Sample response: Returns the all log files as zip.'
+                format: binary
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /filebrowser/list:
     post:
       description: Returns a list of files and/or subdirectories in a given directory.
       requestBody:
+        description: Requested a list of files and/or subdirectories in a given directory.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestDirectoryListingData'
-        description: Requested a list of files and/or subdirectories in a given directory.
-        required: true
       responses:
         '200':
+          description: 'Sample response: Returns a list of files and/or subdirectories
+            in a given directory.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/DirectoryListingResults'
-          description: 'Sample response: Returns a list of files and/or subdirectories
-            in a given directory.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /history/tasks:
     post:
       description: Returns a list of completed tasks.
       requestBody:
+        description: Returns a list of completed tasks.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestHistoryTableData'
-        description: Returns a list of completed tasks.
-        required: true
       responses:
         '200':
+          description: 'Sample response: Returns a list of completed tasks.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/CompletedTasks'
-          description: 'Sample response: Returns a list of completed tasks.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
     delete:
       description: Delete a list of completed tasks.
       requestBody:
+        description: Requested list of items to delete.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestTableUpdateByIdList'
-        description: Requested list of items to delete.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /history/reprocess:
     post:
       description: Add a list of completed tasks back to the Pending Tasks queue.
       requestBody:
+        description: Requested list of items to reprocess.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestAddCompletedToPendingTasks'
-        description: Requested list of items to reprocess.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /history/task/log:
     post:
       description: Request the details of a completed task.
       requestBody:
+        description: Requested the details of a completed task.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/CompletedTasksLogRequest'
-        description: Requested the details of a completed task.
-        required: true
       responses:
         '200':
+          description: 'Success: The details of a requested completed task.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/CompletedTasksLog'
-          description: 'Success: The details of a requested completed task.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
+        '500':
+          description: Internal error; Check `error` for exception
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/InternalError'
+  /notifications/read:
+    get:
+      description: Returns a list of notifications in reverse chronological order.
+      responses:
+        '200':
+          description: 'Sample response: A list of notifications in reverse chronological
+            order.'
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/RequestNotificationsData'
+        '400':
+          description: Bad request; Check `messages` for any validation errors
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/BadRequest'
+        '404':
+          description: Bad request; Requested endpoint not found
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/BadEndpoint'
+        '405':
           description: Bad request; Requested method is not allowed
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/BadMethod'
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
+  /notifications/remove:
+    delete:
+      description: Delete one or all notifications.
+      requestBody:
+        description: Requested list of items to delete.
+        required: true
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/RequestTableUpdateByUuidList'
+      responses:
+        '200':
+          description: Successful request; Returns success status
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/BaseSuccess'
+        '400':
+          description: Bad request; Check `messages` for any validation errors
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/BadRequest'
+        '404':
+          description: Bad request; Requested endpoint not found
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/BadEndpoint'
+        '405':
+          description: Bad request; Requested method is not allowed
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/BadMethod'
+        '500':
           description: Internal error; Check `error` for exception
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/InternalError'
   /pending/tasks:
     post:
       description: Returns a list of pending tasks.
       requestBody:
+        description: Returns a list of pending tasks.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestPendingTableData'
-        description: Returns a list of pending tasks.
-        required: true
       responses:
         '200':
+          description: 'Sample response: Returns a list of pending tasks.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/PendingTasks'
-          description: 'Sample response: Returns a list of pending tasks.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
     delete:
       description: Delete a list of pending tasks.
       requestBody:
+        description: Requested list of items to delete.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestTableUpdateByIdList'
-        description: Requested list of items to delete.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /pending/rescan:
     post:
       description: Triggers a library scan.
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /pending/reorder:
     post:
       description: Reorder a list of pending tasks.
       requestBody:
+        description: Requested list of items to reorder.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestPendingTasksReorder'
-        description: Requested list of items to reorder.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /pending/create:
     post:
       description: Create a new pending tasks from an absolute path
       requestBody:
+        description: Specify path and library to create a pending tasks from.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestPendingTaskCreate'
-        description: Specify path and library to create a pending tasks from.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns data for the generated task
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/PendingTasksTableResults'
-          description: Successful request; Returns data for the generated task
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /pending/library/update:
     post:
       description: Set the library of a list of created tasks who's status has not
         yet been updated.
       requestBody:
+        description: The ID list of the task to update and the Library Name to use.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestPendingTasksLibraryUpdate'
-        description: The ID list of the task to update and the Library Name to use.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /pending/status/get:
     post:
       description: Set the status of a list of pending tasks
       requestBody:
+        description: Set the status of a list of pending tasks.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestTableUpdateByIdList'
-        description: Set the status of a list of pending tasks.
-        required: true
       responses:
         '200':
+          description: 'Sample response: Returns a list of tasks with their status.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/PendingTasksTableResults'
-          description: 'Sample response: Returns a list of tasks with their status.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /pending/status/set/ready:
     post:
       description: Set the status of a list of created pending tasks as ready for
         processing
       requestBody:
+        description: Set the status of a list of created pending tasks as ready for
+          processing.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestTableUpdateByIdList'
-        description: Set the status of a list of created pending tasks as ready for
-          processing.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /pending/download/file/id/{task_id}:
     get:
       description: Request a link for downloading a task file
       responses:
         '200':
+          description: Successful request; Returns download link ID
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/TaskDownloadLink'
-          description: Successful request; Returns download link ID
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /pending/download/data/id/{task_id}:
     get:
       description: Request a link for downloading a task data
       responses:
         '200':
+          description: Successful request; Returns download link ID
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/TaskDownloadLink'
-          description: Successful request; Returns download link ID
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/installed:
     post:
       description: Returns a list of installed plugins.
       requestBody:
+        description: Requested a list of installed plugins.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestPluginsTableData'
-        description: Requested a list of installed plugins.
-        required: true
       responses:
         '200':
+          description: 'Sample response: Returns a list of installed plugins.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/PluginsData'
-          description: 'Sample response: Returns a list of installed plugins.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/enable:
     post:
       description: DEPRECATED! Enable a list of plugins.
       requestBody:
+        description: Requested list of plugins to enable.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestTableUpdateByIdList'
-        description: Requested list of plugins to enable.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/disable:
     post:
       description: DEPRECATED! Disable a list of plugins.
       requestBody:
+        description: Requested list of plugins to disable.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestTableUpdateByIdList'
-        description: Requested list of plugins to disable.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/update:
     post:
       description: Update a list of plugins given their DB table IDs.
       requestBody:
+        description: Requested list of plugins to update.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestTableUpdateByIdList'
-        description: Requested list of plugins to update.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/remove:
     delete:
       description: Remove a list of plugins given their DB table IDs.
       requestBody:
+        description: Requested list of plugins to remove.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestTableUpdateByIdList'
-        description: Requested list of plugins to remove.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/info:
     post:
       description: Returns a the metadata and settings of a requested plugin.
       requestBody:
+        description: Requested a single plugin's info.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestPluginsInfo'
-        description: Requested a single plugin's info.
-        required: true
       responses:
         '200':
+          description: 'Sample response: Returns a the metadata and settings of a
+            requested plugin.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/PluginsInfoResults'
-          description: 'Sample response: Returns a the metadata and settings of a
-            requested plugin.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/settings/update:
     post:
       description: Saves the settings of a single plugin.
       requestBody:
+        description: Requested a plugins settings be updated.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestPluginsSettingsSave'
-        description: Requested a plugins settings be updated.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/settings/reset:
     post:
       description: Reset the settings of a single plugin.
       requestBody:
+        description: Requested a plugins settings be reset.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestPluginsSettingsReset'
-        description: Requested a plugins settings be reset.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/installable:
     get:
       description: Returns a list of installable plugins.
       responses:
         '200':
+          description: 'Sample response: Returns a list of installable plugins.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/PluginsInstallableResults'
-          description: 'Sample response: Returns a list of installable plugins.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/install:
     post:
       description: Installs a plugin by its Plugin ID.
       requestBody:
+        description: Requested a plugin be installed by its Plugin ID.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestPluginsById'
-        description: Requested a plugin be installed by its Plugin ID.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/flow:
     post:
       description: Returns the plugin flow for a requested plugin type.
       requestBody:
+        description: Requests the plugin flow of a given plugin type.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestPluginsFlowByPluginType'
-        description: Requests the plugin flow of a given plugin type.
-        required: true
       responses:
         '200':
+          description: 'Sample response: Returns the plugin flow for a requested plugin
+            type.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/PluginsInstallableResults'
-          description: 'Sample response: Returns the plugin flow for a requested plugin
-            type.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/flow/types:
     get:
       description: Returns a list of all plugin types that have flows.
       responses:
         '200':
+          description: 'Sample response: Returns a list of all plugin types that have
+            flows.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/PluginTypesResults'
-          description: 'Sample response: Returns a list of all plugin types that have
-            flows.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/flow/save:
     post:
       description: Saves the plugin flow for a requested plugin type.
       requestBody:
+        description: Requests saving the plugin flow for a given plugin type.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestSavingPluginsFlowByPluginType'
-        description: Requests saving the plugin flow for a given plugin type.
-        required: true
       responses:
         '200':
+          description: 'Sample response: Save the plugin flow for a requested plugin
+            type.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/PluginsInstallableResults'
-          description: 'Sample response: Save the plugin flow for a requested plugin
-            type.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/repos/update:
     post:
       description: Updates the plugin repo list.
       requestBody:
+        description: Requested an update to the plugin repo list.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestUpdatePluginReposList'
-        description: Requested an update to the plugin repo list.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/repos/list:
     get:
       description: Returns a list of plugin repos.
       responses:
         '200':
+          description: 'Sample response: Returns a list of plugin repos.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/PluginReposListResults'
-          description: 'Sample response: Returns a list of plugin repos.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/repos/reload:
     post:
       description: Reload plugin repositories remote data.
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /plugins/panels/enabled:
     get:
       description: Returns a list of installed plugins.
       responses:
         '200':
+          description: 'Success: Returns a list of installed plugins.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/PluginsDataPanelTypesData'
-          description: 'Success: Returns a list of installed plugins.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /session/state:
     get:
       description: Returns the application session state.
       responses:
         '200':
+          description: 'Sample response: Returns the application session state.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/SessionStateSuccess'
-          description: 'Sample response: Returns the application session state.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /session/reload:
     post:
       description: Reload the current session.
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/read:
     get:
       description: Returns the application settings.
       responses:
         '200':
+          description: 'Sample response: Returns the application settings.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/SettingsReadAndWrite'
-          description: 'Sample response: Returns the application settings.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/write:
     post:
       description: Save a given dictionary of settings.
       requestBody:
+        description: Requested a dictionary of settings to save.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/SettingsReadAndWrite'
-        description: Requested a dictionary of settings to save.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/configuration:
     get:
       description: Returns the system configuration.
       responses:
         '200':
+          description: 'Sample response: Returns the system configuration.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/SettingsSystemConfig'
-          description: 'Sample response: Returns the system configuration.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/link/validate:
     post:
       description: Validate a remote installation address
       requestBody:
+        description: The details of the remote installation to validate
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestSettingsRemoteInstallationAddressValidation'
-        description: The details of the remote installation to validate
-        required: true
       responses:
         '200':
+          description: 'Sample response: Returns the remote installation data.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/SettingsRemoteInstallationData'
-          description: 'Sample response: Returns the remote installation data.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/worker_groups:
     get:
       description: Returns a list of all worker groups.
       responses:
         '200':
+          description: 'Sample response: Returns a list of all worker groups.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/WorkerGroupsList'
-          description: 'Sample response: Returns a list of all worker groups.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/worker_group/read:
     post:
       description: Read the configuration of a worker group
       requestBody:
+        description: The ID of the worker group
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestDatabaseItemById'
-        description: The ID of the worker group
-        required: true
       responses:
         '200':
+          description: 'Sample response: Returns the worker group configuration.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/SettingsWorkerGroupConfig'
-          description: 'Sample response: Returns the worker group configuration.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/worker_group/write:
     post:
       description: Write the configuration of a worker group
       requestBody:
+        description: The config of a worker group that is to be saved
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/SettingsWorkerGroupConfig'
-        description: The config of a worker group that is to be saved
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/worker_group/remove:
     delete:
       description: Remove a worker group
       requestBody:
+        description: Requested a worker group to remove.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestDatabaseItemById'
-        description: Requested a worker group to remove.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/link/read:
     post:
       description: Read the configuration of a remote installation link
       requestBody:
+        description: The UUID of the remote installation
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestRemoteInstallationLinkConfig'
-        description: The UUID of the remote installation
-        required: true
       responses:
         '200':
+          description: 'Sample response: Returns the remote installation link configuration.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/SettingsRemoteInstallationLinkConfig'
-          description: 'Sample response: Returns the remote installation link configuration.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/link/write:
     post:
       description: Write the configuration of a remote installation link
       requestBody:
+        description: The UUID of the remote installation and its configuration
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/SettingsRemoteInstallationLinkConfig'
-        description: The UUID of the remote installation and its configuration
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/link/remove:
     delete:
       description: Remove a configuration for a remote installation link
       requestBody:
+        description: Requested a remote installation link to remove.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestRemoteInstallationLinkConfig'
-        description: Requested a remote installation link to remove.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/libraries:
     get:
       description: Returns a list of all libraries.
       responses:
         '200':
+          description: 'Sample response: Returns a list of all libraries.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/SettingsLibrariesList'
-          description: 'Sample response: Returns a list of all libraries.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/library/read:
     post:
       description: Read the configuration of one library
       requestBody:
+        description: The ID of the library
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestLibraryById'
-        description: The ID of the library
-        required: true
       responses:
         '200':
+          description: 'Sample response: Returns the remote installation link configuration.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/SettingsLibraryConfigReadAndWrite'
-          description: 'Sample response: Returns the remote installation link configuration.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/library/write:
     post:
       description: Write the configuration of one library
       requestBody:
+        description: Requested a dictionary of settings to save.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/SettingsLibraryConfigReadAndWrite'
-        description: Requested a dictionary of settings to save.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/library/remove:
     delete:
       description: Remove a library
       requestBody:
+        description: Requested a library to remove.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestLibraryById'
-        description: Requested a library to remove.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/library/export:
     post:
       description: Export the plugin configuration of one library
       requestBody:
+        description: The ID of the library
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestLibraryById'
-        description: The ID of the library
-        required: true
       responses:
         '200':
+          description: 'Sample response: Returns the remote installation link configuration.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/SettingsLibraryPluginConfigExport'
-          description: 'Sample response: Returns the remote installation link configuration.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /settings/library/import:
     post:
       description: Import the configuration of one library
       requestBody:
+        description: Requested a dictionary of settings to save.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/SettingsLibraryPluginConfigImport'
-        description: Requested a dictionary of settings to save.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /upload/pending/file:
     post:
-      description: Returns a list of pending tasks.
+      description: Uploads a file to the pending tasks list
       requestBody:
+        description: Uploads a file to the pending tasks list
+        required: true
         content:
           multipart/form-data:
             schema:
+              type: object
               properties:
                 fileName:
-                  format: binary
                   type: string
-              type: object
-        description: Returns a list of pending tasks.
-        required: true
+                  format: binary
       responses:
         '200':
+          description: Successful request; Returns data for the generated task
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/PendingTasksTableResults'
-          description: Successful request; Returns data for the generated task
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
+  /upload/plugin/file:
+    post:
+      description: Uploads a plugin ZIP file and installs it
+      requestBody:
+        description: Uploads a plugin ZIP file and installs it
+        required: true
+        content:
+          multipart/form-data:
+            schema:
+              type: object
+              properties:
+                fileName:
+                  type: string
+                  format: binary
+      responses:
+        '200':
+          description: Successful request; Returns success status
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/BaseSuccess'
+        '400':
+          description: Bad request; Check `messages` for any validation errors
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/BadRequest'
+        '404':
+          description: Bad request; Requested endpoint not found
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/BadEndpoint'
+        '405':
+          description: Bad request; Requested method is not allowed
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/BadMethod'
+        '500':
           description: Internal error; Check `error` for exception
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/InternalError'
   /version/read:
     get:
       description: Returns the application version.
       responses:
         '200':
+          description: 'Sample response: Returns the application version.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/VersionReadSuccess'
-          description: 'Sample response: Returns the application version.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /workers/worker/pause:
     post:
       description: Pauses a worker by its ID.
       requestBody:
+        description: Requested a worker be paused by its ID.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestWorkerById'
-        description: Requested a worker be paused by its ID.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /workers/worker/pause/all:
     post:
       description: Pause all workers.
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /workers/worker/resume:
     post:
       description: Resumes a worker by its ID.
       requestBody:
+        description: Requested a worker be resumed by its ID.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestWorkerById'
-        description: Requested a worker be resumed by its ID.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /workers/worker/resume/all:
     post:
       description: Resumes all workers.
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /workers/worker/terminate:
     delete:
       description: Terminates a worker by its ID.
       requestBody:
+        description: Requested a worker be terminated by its ID.
+        required: true
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RequestWorkerById'
-        description: Requested a worker be terminated by its ID.
-        required: true
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /workers/worker/terminate/all:
     delete:
       description: Terminate all workers.
       responses:
         '200':
+          description: Successful request; Returns success status
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BaseSuccess'
-          description: Successful request; Returns success status
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
   /workers/status:
     get:
       description: Returns the status of all workers.
       responses:
         '200':
+          description: 'Sample response: Returns the status of all workers.'
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/WorkerStatusSuccess'
-          description: 'Sample response: Returns the status of all workers.'
         '400':
+          description: Bad request; Check `messages` for any validation errors
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadRequest'
-          description: Bad request; Check `messages` for any validation errors
         '404':
+          description: Bad request; Requested endpoint not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadEndpoint'
-          description: Bad request; Requested endpoint not found
         '405':
+          description: Bad request; Requested method is not allowed
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/BadMethod'
-          description: Bad request; Requested method is not allowed
         '500':
+          description: Internal error; Check `error` for exception
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/InternalError'
-          description: Internal error; Check `error` for exception
-security:
-- BasicAuth: []
-servers:
-- description: Local environment
-  url: http://localhost:8888/unmanic/api/v2/
+openapi: 3.0.0
```

### Comparing `unmanic-0.2.3/unmanic/webserver/docs/api_schema_v2.json` & `unmanic-0.2.4/unmanic/webserver/docs/api_schema_v2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950061278975421%*

 * *Differences: {"'components'": "{'schemas': {'PluginsConfigInputItem': {'properties': {'description': "*

 * *                 "OrderedDict([('type', 'string'), ('nullable', True), ('description', "*

 * *                 "'Description of input field'), ('example', 'Will automatically downmix DTS-HD "*

 * *                 "Master Audio to 5.1 channels ')]), 'tooltip': OrderedDict([('type', 'string'), "*

 * *                 "('nullable', True), ('description', 'Description of input field'), ('example', "*

 * *                 "'Will automatically […]*

```diff
@@ -346,14 +346,59 @@
                     "locked",
                     "name",
                     "path",
                     "tags"
                 ],
                 "type": "object"
             },
+            "NotificationData": {
+                "properties": {
+                    "icon": {
+                        "description": "The icon to display with the notification",
+                        "example": "update",
+                        "type": "string"
+                    },
+                    "label": {
+                        "description": "The label of the notification. Can be a I18n key or a string",
+                        "example": "updateAvailableLabel",
+                        "type": "string"
+                    },
+                    "message": {
+                        "description": "The message of the notification. Can be a I18n key or a string",
+                        "example": "updateAvailableMessage",
+                        "type": "string"
+                    },
+                    "navigation": {
+                        "description": "The navigation links of the notification",
+                        "example": {
+                            "url": "https://docs.unmanic.app"
+                        },
+                        "type": "object"
+                    },
+                    "type": {
+                        "description": "The type of notification",
+                        "example": "info",
+                        "type": "string"
+                    },
+                    "uuid": {
+                        "description": "Unique ID for this notification",
+                        "example": "updateAvailable",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "icon",
+                    "label",
+                    "message",
+                    "navigation",
+                    "type",
+                    "uuid"
+                ],
+                "type": "object"
+            },
             "PendingTasks": {
                 "properties": {
                     "recordsFiltered": {
                         "default": 10,
                         "description": "Total number of records after filters have been applied",
                         "example": 10,
                         "type": "integer"
@@ -553,14 +598,20 @@
                 "required": [
                     "results"
                 ],
                 "type": "object"
             },
             "PluginsConfigInputItem": {
                 "properties": {
+                    "description": {
+                        "description": "Description of input field",
+                        "example": "Will automatically downmix DTS-HD Master Audio to 5.1 channels ",
+                        "nullable": true,
+                        "type": "string"
+                    },
                     "display": {
                         "description": "Should the setting input be displayed (visible, hidden)",
                         "example": "visible",
                         "type": "string"
                     },
                     "input_type": {
                         "description": "The config input type",
@@ -604,27 +655,41 @@
                         "example": {
                             "max": 8,
                             "min": 1,
                             "suffix": "M"
                         },
                         "type": "object"
                     },
+                    "sub_setting": {
+                        "description": "Should the setting be a nested sub-setting field",
+                        "example": false,
+                        "type": "boolean"
+                    },
+                    "tooltip": {
+                        "description": "Description of input field",
+                        "example": "Will automatically downmix DTS-HD Master Audio to 5.1 channels ",
+                        "nullable": true,
+                        "type": "string"
+                    },
                     "value": {
                         "description": "The current value of this config input",
                         "example": false
                     }
                 },
                 "required": [
+                    "description",
                     "display",
                     "input_type",
                     "key",
                     "key_id",
                     "label",
                     "select_options",
                     "slider_options",
+                    "sub_setting",
+                    "tooltip",
                     "value"
                 ],
                 "type": "object"
             },
             "PluginsData": {
                 "properties": {
                     "recordsFiltered": {
@@ -1037,14 +1102,30 @@
                     }
                 },
                 "required": [
                     "id"
                 ],
                 "type": "object"
             },
+            "RequestNotificationsData": {
+                "properties": {
+                    "notifications": {
+                        "description": "List of notifications",
+                        "items": {
+                            "$ref": "#/components/schemas/NotificationData"
+                        },
+                        "minItems": 0,
+                        "type": "array"
+                    }
+                },
+                "required": [
+                    "notifications"
+                ],
+                "type": "object"
+            },
             "RequestPendingTableData": {
                 "properties": {
                     "after": {
                         "description": "Filter entries since datetime",
                         "example": "2022-04-07 01:45",
                         "format": "date-time",
                         "nullable": true,
@@ -1423,14 +1504,31 @@
                     }
                 },
                 "required": [
                     "id_list"
                 ],
                 "type": "object"
             },
+            "RequestTableUpdateByUuidList": {
+                "properties": {
+                    "uuid_list": {
+                        "description": "List of table UUIDs",
+                        "example": [],
+                        "items": {
+                            "type": "string"
+                        },
+                        "minItems": 1,
+                        "type": "array"
+                    }
+                },
+                "required": [
+                    "uuid_list"
+                ],
+                "type": "object"
+            },
             "RequestUpdatePluginReposList": {
                 "properties": {
                     "repos_list": {
                         "description": "A list of repost to save",
                         "example": [
                             "https://raw.githubusercontent.com/Josh5/unmanic-plugins/repo/repo.json"
                         ],
@@ -2454,14 +2552,139 @@
                             }
                         },
                         "description": "Internal error; Check `error` for exception"
                     }
                 }
             }
         },
+        "/notifications/read": {
+            "get": {
+                "description": "Returns a list of notifications in reverse chronological order.",
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/RequestNotificationsData"
+                                }
+                            }
+                        },
+                        "description": "Sample response: A list of notifications in reverse chronological order."
+                    },
+                    "400": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/BadRequest"
+                                }
+                            }
+                        },
+                        "description": "Bad request; Check `messages` for any validation errors"
+                    },
+                    "404": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/BadEndpoint"
+                                }
+                            }
+                        },
+                        "description": "Bad request; Requested endpoint not found"
+                    },
+                    "405": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/BadMethod"
+                                }
+                            }
+                        },
+                        "description": "Bad request; Requested method is not allowed"
+                    },
+                    "500": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/InternalError"
+                                }
+                            }
+                        },
+                        "description": "Internal error; Check `error` for exception"
+                    }
+                }
+            }
+        },
+        "/notifications/remove": {
+            "delete": {
+                "description": "Delete one or all notifications.",
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "$ref": "#/components/schemas/RequestTableUpdateByUuidList"
+                            }
+                        }
+                    },
+                    "description": "Requested list of items to delete.",
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/BaseSuccess"
+                                }
+                            }
+                        },
+                        "description": "Successful request; Returns success status"
+                    },
+                    "400": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/BadRequest"
+                                }
+                            }
+                        },
+                        "description": "Bad request; Check `messages` for any validation errors"
+                    },
+                    "404": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/BadEndpoint"
+                                }
+                            }
+                        },
+                        "description": "Bad request; Requested endpoint not found"
+                    },
+                    "405": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/BadMethod"
+                                }
+                            }
+                        },
+                        "description": "Bad request; Requested method is not allowed"
+                    },
+                    "500": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/InternalError"
+                                }
+                            }
+                        },
+                        "description": "Internal error; Check `error` for exception"
+                    }
+                }
+            }
+        },
         "/pending/create": {
             "post": {
                 "description": "Create a new pending tasks from an absolute path",
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
@@ -5428,30 +5651,30 @@
                         "description": "Internal error; Check `error` for exception"
                     }
                 }
             }
         },
         "/upload/pending/file": {
             "post": {
-                "description": "Returns a list of pending tasks.",
+                "description": "Uploads a file to the pending tasks list",
                 "requestBody": {
                     "content": {
                         "multipart/form-data": {
                             "schema": {
                                 "properties": {
                                     "fileName": {
                                         "format": "binary",
                                         "type": "string"
                                     }
                                 },
                                 "type": "object"
                             }
                         }
                     },
-                    "description": "Returns a list of pending tasks.",
+                    "description": "Uploads a file to the pending tasks list",
                     "required": true
                 },
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
@@ -5463,14 +5686,88 @@
                     },
                     "400": {
                         "content": {
                             "application/json": {
                                 "schema": {
                                     "$ref": "#/components/schemas/BadRequest"
                                 }
+                            }
+                        },
+                        "description": "Bad request; Check `messages` for any validation errors"
+                    },
+                    "404": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/BadEndpoint"
+                                }
+                            }
+                        },
+                        "description": "Bad request; Requested endpoint not found"
+                    },
+                    "405": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/BadMethod"
+                                }
+                            }
+                        },
+                        "description": "Bad request; Requested method is not allowed"
+                    },
+                    "500": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/InternalError"
+                                }
+                            }
+                        },
+                        "description": "Internal error; Check `error` for exception"
+                    }
+                }
+            }
+        },
+        "/upload/plugin/file": {
+            "post": {
+                "description": "Uploads a plugin ZIP file and installs it",
+                "requestBody": {
+                    "content": {
+                        "multipart/form-data": {
+                            "schema": {
+                                "properties": {
+                                    "fileName": {
+                                        "format": "binary",
+                                        "type": "string"
+                                    }
+                                },
+                                "type": "object"
+                            }
+                        }
+                    },
+                    "description": "Uploads a plugin ZIP file and installs it",
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/BaseSuccess"
+                                }
+                            }
+                        },
+                        "description": "Successful request; Returns success status"
+                    },
+                    "400": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/BadRequest"
+                                }
                             }
                         },
                         "description": "Bad request; Check `messages` for any validation errors"
                     },
                     "404": {
                         "content": {
                             "application/json": {
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/scripts/translate.sh` & `unmanic-0.2.4/unmanic/webserver/frontend/scripts/translate.sh`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/.eslintrc.js` & `unmanic-0.2.4/unmanic/webserver/frontend/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/public/icons/favicon-128x128.png` & `unmanic-0.2.4/unmanic/webserver/frontend/public/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/public/icons/favicon-16x16.png` & `unmanic-0.2.4/unmanic/webserver/frontend/public/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/public/icons/favicon-32x32.png` & `unmanic-0.2.4/unmanic/webserver/frontend/public/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/public/icons/favicon-96x96.png` & `unmanic-0.2.4/unmanic/webserver/frontend/public/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/public/favicon.ico` & `unmanic-0.2.4/unmanic/webserver/frontend/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/package-lock.json` & `unmanic-0.2.4/unmanic/webserver/frontend/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999796253988312%*

 * *Differences: {"'dependencies'": "{'tiny-emitter': OrderedDict([('version', '2.1.0'), ('resolved', "*

 * *                   "'https://registry.npmjs.org/tiny-emitter/-/tiny-emitter-2.1.0.tgz'), "*

 * *                   "('integrity', "*

 * *                   "'sha512-NB6Dk1A9xgQPMoGqC5CVXn123gWyte215ONT5Pp5a0yt4nlEoO1ZWeCwpncaekPHXO60i47ihFnZPiRPjRMq4Q==')])}",*

 * * "'packages'": "{'': {'dependencies': {'tiny-emitter': '^2.1.0'}}, 'node_modules/tiny-emitter': "*

 * *               "OrderedDict([('version', '2.1.0'), ('resolved', "*

 * *           […]*

```diff
@@ -7456,14 +7456,19 @@
         },
         "thunky": {
             "dev": true,
             "integrity": "sha512-eHY7nBftgThBqOyHGVN+l8gF0BucP09fMo0oO/Lb0w1OF80dJv+lDVpXG60WMQvkcxAkNybKsrEIE3ZtKGmPrA==",
             "resolved": "https://registry.npmjs.org/thunky/-/thunky-1.1.0.tgz",
             "version": "1.1.0"
         },
+        "tiny-emitter": {
+            "integrity": "sha512-NB6Dk1A9xgQPMoGqC5CVXn123gWyte215ONT5Pp5a0yt4nlEoO1ZWeCwpncaekPHXO60i47ihFnZPiRPjRMq4Q==",
+            "resolved": "https://registry.npmjs.org/tiny-emitter/-/tiny-emitter-2.1.0.tgz",
+            "version": "2.1.0"
+        },
         "tmp": {
             "dev": true,
             "integrity": "sha512-jRCJlojKnZ3addtTOjdIqoRuPEKBvNXcGYqzO6zWZX8KfKEpnGY5jfggJQ3EjKuu8D4bJRr0y+cYJFmYbImXGw==",
             "requires": {
                 "os-tmpdir": "~1.0.2"
             },
             "resolved": "https://registry.npmjs.org/tmp/-/tmp-0.0.33.tgz",
@@ -8409,14 +8414,15 @@
                 "@quasar/extras": "^1.13.5",
                 "axios": "^0.21.1",
                 "core-js": "^3.6.5",
                 "js-bbcode-parser": "^3.0.4",
                 "quasar": "^2.6.6",
                 "remarkable": "^2.0.1",
                 "remarkable-admonitions": "^0.2.2",
+                "tiny-emitter": "^2.1.0",
                 "vue-i18n": "^9.0.0-beta.0",
                 "vuedraggable": "^4.1.0",
                 "vuex": "^4.0.1",
                 "xbbcode-parser": "^0.1.0"
             },
             "devDependencies": {
                 "@babel/eslint-parser": "^7.13.14",
@@ -18490,14 +18496,19 @@
         },
         "node_modules/thunky": {
             "dev": true,
             "integrity": "sha512-eHY7nBftgThBqOyHGVN+l8gF0BucP09fMo0oO/Lb0w1OF80dJv+lDVpXG60WMQvkcxAkNybKsrEIE3ZtKGmPrA==",
             "resolved": "https://registry.npmjs.org/thunky/-/thunky-1.1.0.tgz",
             "version": "1.1.0"
         },
+        "node_modules/tiny-emitter": {
+            "integrity": "sha512-NB6Dk1A9xgQPMoGqC5CVXn123gWyte215ONT5Pp5a0yt4nlEoO1ZWeCwpncaekPHXO60i47ihFnZPiRPjRMq4Q==",
+            "resolved": "https://registry.npmjs.org/tiny-emitter/-/tiny-emitter-2.1.0.tgz",
+            "version": "2.1.0"
+        },
         "node_modules/tmp": {
             "dependencies": {
                 "os-tmpdir": "~1.0.2"
             },
             "dev": true,
             "engines": {
                 "node": ">=0.6.0"
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/quasar.conf.js` & `unmanic-0.2.4/unmanic/webserver/frontend/quasar.conf.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -22,14 +22,15 @@
 
         // app boot file (/src/boot)
         // --> boot files are part of "main.js"
         // https://v2.quasar.dev/quasar-cli/boot-files
         boot: [
             'axios',
             'i18n',
+            'global-event-bus',
         ],
 
         // https://v2.quasar.dev/quasar-cli/quasar-conf-js#Property%3A-css
         css: [
             'app.scss',
             'markdown-admonitions.css'
         ],
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/LICENSE` & `unmanic-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/package.json` & `unmanic-0.2.4/unmanic/webserver/frontend/package.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962121212121211%*

 * *Differences: {"'dependencies'": "{'tiny-emitter': '^2.1.0'}"}*

```diff
@@ -15,14 +15,15 @@
         "@quasar/extras": "^1.13.5",
         "axios": "^0.21.1",
         "core-js": "^3.6.5",
         "js-bbcode-parser": "^3.0.4",
         "quasar": "^2.6.6",
         "remarkable": "^2.0.1",
         "remarkable-admonitions": "^0.2.2",
+        "tiny-emitter": "^2.1.0",
         "vue-i18n": "^9.0.0-beta.0",
         "vuedraggable": "^4.1.0",
         "vuex": "^4.0.1",
         "xbbcode-parser": "^0.1.0"
     },
     "description": "A simple tool for optimising your video library to a single, uniform format",
     "devDependencies": {
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/jsconfig.json` & `unmanic-0.2.4/unmanic/webserver/frontend/jsconfig.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/README.md` & `unmanic-0.2.4/unmanic/webserver/frontend/README.md`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/css/markdown-admonitions.css` & `unmanic-0.2.4/unmanic/webserver/frontend/src/css/markdown-admonitions.css`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/css/quasar.variables.scss` & `unmanic-0.2.4/unmanic/webserver/frontend/src/css/quasar.variables.scss`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/App.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/App.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/pages/SettingsLink.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/pages/SettingsLink.vue`

 * *Files 1% similar despite different names*

```diff
@@ -396,15 +396,14 @@
           uuid: this.remoteInstallations[i].uuid,
           available: this.remoteInstallations[i].available,
         };
       }
       let data = {
         settings: {
           installation_name: this.installationName,
-          remote_installations: remoteInstallationsList,
         }
       }
       axios({
         method: 'post',
         url: getUnmanicApiUrl('v2', 'settings/write'),
         data: data
       }).then((response) => {
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/pages/DataPanels.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/pages/DataPanels.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/pages/SettingsPlugins.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/pages/SettingsPlugins.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/pages/Dashboard.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/pages/Dashboard.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/pages/Trigger.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/pages/Trigger.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/pages/Error404.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/pages/Error404.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/pages/SettingsLibrary.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/pages/SettingsLibrary.vue`

 * *Files 2% similar despite different names*

```diff
@@ -344,16 +344,16 @@
 import { UnmanicWebsocketHandler } from "src/js/unmanicWebsocket";
 import { onMounted, onUnmounted, ref } from "vue";
 import { useQuasar } from 'quasar'
 import { useI18n } from "vue-i18n";
 import DirectoryBrowserDialog from "components/DirectoryBrowserDialog";
 import axios from "axios";
 import { getUnmanicApiUrl } from "src/js/unmanicGlobals";
-import LibraryConfigureDialog from "components/LibraryConfigureDialog";
 import MobileSettingsQuickNav from "components/MobileSettingsQuickNav";
+import ConfigDrawerDialog from "components/dialogs/ConfigDrawerDialog";
 
 export default {
   name: 'SettingsLibrary',
   components: { MobileSettingsQuickNav },
   setup() {
     const $q = useQuasar()
     const { t: $t } = useI18n();
@@ -607,24 +607,27 @@
           actions: [{ icon: 'close', color: 'white' }]
         })
       });
     },
     configureLibraryPath: function (index) {
       let library = this.libraryPaths[index]
       this.$q.dialog({
-        component: LibraryConfigureDialog,
+        component: ConfigDrawerDialog,
         componentProps: {
-          dialogHeader: this.$t('headers.configureLibrary'),
-          libraryId: library.id
+          header: this.$t('headers.configureLibrary'),
+          componentName: "LibraryConfigForm",
+          componentProps: {
+            libraryId: library.id,
+          },
         },
       }).onOk((payload) => {
       }).onDismiss(() => {
         this.fetchSettings();
         this.fetchLibraryList();
-      })
+      });
     },
   },
   created() {
     this.fetchSettings();
     this.fetchLibraryList();
   }
 }
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/pages/SettingsWorkers.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/pages/SettingsWorkers.vue`

 * *Files 8% similar despite different names*

```diff
@@ -309,29 +309,17 @@
             actions: [{ icon: 'close', color: 'white' }]
           })
         });
       })
     },
     save: function () {
       // Save settings
-      let workerEventSchedule = []
-      for (let i = 0; i < this.schedules.length; i++) {
-        workerEventSchedule[workerEventSchedule.length] = {
-          repetition: this.schedules[i].repetition,
-          schedule_time: this.schedules[i].scheduleTime,
-          schedule_task: this.schedules[i].scheduleTask,
-          schedule_worker_count: this.schedules[i].scheduleWorkerCount,
-        };
-      }
       let data = {
         settings: {
-          worker_groups: this.workerGroups,
-          number_of_workers: this.workerCount,
           cache_path: this.cachePath,
-          worker_event_schedules: workerEventSchedule,
         }
       }
       axios({
         method: 'post',
         url: getUnmanicApiUrl('v2', 'settings/write'),
         data: data
       }).then((response) => {
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/pages/SettingsSupport.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/pages/SettingsSupport.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/language/pl.json` & `unmanic-0.2.4/unmanic/webserver/frontend/src/language/pl.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9702393162049654%*

 * *Differences: {"'buttons'": "{'dismissAll': 'Odrzucić wszystkie'}",*

 * * "'components'": "{'settings': {'library': {'name': 'Nazwa (musi być niepowtarzalna)', 'path': "*

 * *                 "'Ścieżka biblioteki'}, 'link': {'enableTaskPreloading': 'Wstępnie załaduj "*

 * *                 "niektóre zadania z kolejki zadań oczekujących na instalację zdalną', "*

 * *                 "'linkConfigChecksumValidationStatusLabel': 'Waliduj sumami kontrolnymi'}, "*

 * *                 "'support': {'appVersion': 'Wersja Unmanic'}}, 'plugins': {'errorSa […]*

```diff
@@ -1,10 +1,11 @@
 {
     "buttons": {
         "darkMode": "Tryb ciemny",
+        "dismissAll": "Odrzuci\u0107 wszystkie",
         "language": "J\u0119zyk"
     },
     "components": {
         "completedTasks": {
             "addToPendingTasksList": "Dodaj wybrane do listy zada\u0144 oczekuj\u0105cych",
             "before": "Zanim",
             "details": "Detale",
@@ -26,17 +27,21 @@
             "rescanLibrary": "Ponownie przeskanuj bibliotek\u0119 teraz"
         },
         "plugins": {
             "addRepository": "Dodaj repozytorium",
             "author": "Autor",
             "categoryFilter": "Filtr kategorii",
             "clickToUpdatePlugin": "Kliknij, aby zaktualizowa\u0107 wtyczk\u0119",
-            "errorSavingFlow": "Wyst\u0105pi\u0142 b\u0142\u0105d podczas zapisywania przep\u0142ywu wtyczki",
+            "errorSavingFlow": "Wyst\u0105pi\u0142 b\u0142\u0105d podczas zapisywania przep\u0142ywu wtyczek",
+            "failedToInstallPluginFromZip": "Nie uda\u0142o si\u0119 zainstalowa\u0107 wtyczki z przes\u0142anego pliku ZIP",
             "globalConfiguration": "Konfiguracja globalna",
-            "installPlugins": "Zainstaluj wtyczk\u0119",
+            "installPluginFromFile": "Zainstaluj wtyczk\u0119 z pliku",
+            "installPluginFromRepo": "Zainstaluj wtyczk\u0119 z repozytorium",
+            "installedPluginFromZip": "Zainstalowana wtyczka",
+            "invalidZipFile": "Plik nie jest prawid\u0142owym plikiem ZIP",
             "newRepository": "Nowe repozytorium",
             "pluginUpToDate": "Wtyczka jest aktualna",
             "refreshRepositories": "Od\u015bwie\u017c repozytoria",
             "removePlugin": "Usu\u0144 wtyczk\u0119",
             "repo": "Magazyn",
             "repoList": "Lista repozytori\u00f3w",
             "repoName": "Nazwa",
@@ -46,15 +51,15 @@
                 "libraryManagement": {
                     "fileTest": "Zarz\u0105dzanie bibliotek\u0105 - Test plik\u00f3w",
                     "fileTestCaption": "Te wtyczki s\u0105 wywo\u0142ywane w celu sprawdzenia, czy pliki powinny zosta\u0107 dodane do listy oczekuj\u0105cych zada\u0144"
                 },
                 "postprocessor": {
                     "fileMove": "Postprocesor \u2014 ruchy plik\u00f3w",
                     "fileMoveCaption": "Wtyczki te s\u0105 wywo\u0142ywane po zako\u0144czeniu zadania, aby doda\u0107 dodatkowe ruchy plik\u00f3w",
-                    "taskResult": "Postprocesor \u2014 oznaczanie sukcesu/pora\u017cki zadania",
+                    "taskResult": "Postprocesor \u2014 oznaczanie powodzenia/pora\u017cki zadania",
                     "taskResultCaption": "Te wtyczki s\u0105 wywo\u0142ywane po zako\u0144czeniu zadania, aby oznaczy\u0107 og\u00f3lny sukces lub pora\u017ck\u0119 tego zadania"
                 },
                 "worker": {
                     "processItem": "Pracownik \u2014 Przetwarzanie pliku",
                     "processItemCaption": "Wtyczki te s\u0105 wywo\u0142ywane przez pracownika i generuj\u0105 niestandardowe polecenie do wykonania i zarz\u0105dzania przez tego pracownika"
                 }
             },
@@ -90,17 +95,17 @@
                 "libraryRemoteOnlyStatus": "Tylko zdalne",
                 "libraryScanner": "Skaner biblioteczny",
                 "libraryScannerSchedule": "Harmonogram skanowania biblioteki w kilka minut",
                 "libraryScannerScheduleNotValid": "Harmonogram skanowania biblioteki jest nieprawid\u0142owy",
                 "libraryScannerStatusLabel": "Skaner biblioteczny",
                 "locked": "Biblioteki nie mo\u017cna usun\u0105\u0107",
                 "maxAgeOfCompletedTasks": "Maksymalna liczba dni do przechowywania uko\u0144czonych zada\u0144",
-                "name": "Imi\u0119 (musi by\u0107 niepowtarzalne)",
+                "name": "Nazwa (musi by\u0107 niepowtarzalna)",
                 "newLibrary": "Nowa Biblioteka",
-                "path": "\u015acie\u017cka do biblioteki",
+                "path": "\u015acie\u017cka biblioteki",
                 "pathConfiguration": "Biblioteki",
                 "pathDisabledReceiveRemoteFilesOnly": "Opcja wy\u0142\u0105czona, poniewa\u017c skonfigurowa\u0142e\u015b t\u0119 bibliotek\u0119 tylko do odbierania plik\u00f3w zdalnych",
                 "pendingTasks": "Zadania oczekuj\u0105ce",
                 "pluginFlow": "Przep\u0142yw wtyczek",
                 "plugins": "Wtyczki",
                 "priorityScore": "Ustaw modyfikator wyniku priorytetu dla zada\u0144 generowanych dla tej biblioteki",
                 "runLibraryScanOnStart": "Uruchom jednorazowe skanowanie biblioteki podczas uruchamiania",
@@ -114,16 +119,16 @@
                 "allowSendingTasks": "Wysy\u0142aj zadania do tej instalacji, gdy pracownicy s\u0105 dost\u0119pni",
                 "authentication": "Uwierzytelnianie",
                 "collectiveManagement": "Zarz\u0105dzanie zbiorowe",
                 "connection": "Po\u0142\u0105czenie",
                 "enableChecksumValidation": "Weryfikuj transfery plik\u00f3w za pomoc\u0105 sum kontrolnych (powoli)",
                 "enableConfigMissingLibraries": "Automatycznie skonfiguruj brakuj\u0105ce biblioteki podczas zdalnej instalacji",
                 "enableDistributedWorkerCount": "W\u0142\u0105cz rozproszon\u0105 liczb\u0119 pracownik\u00f3w dla tego \u0142\u0105cza",
-                "enableTaskPreloading": "Za\u0142aduj wst\u0119pnie niekt\u00f3re zadania z kolejki zada\u0144 oczekuj\u0105cych na instalacj\u0119 zdaln\u0105",
-                "linkConfigChecksumValidationStatusLabel": "Zatwierd\u017a sumami kontrolnymi",
+                "enableTaskPreloading": "Wst\u0119pnie za\u0142aduj niekt\u00f3re zadania z kolejki zada\u0144 oczekuj\u0105cych na instalacj\u0119 zdaln\u0105",
+                "linkConfigChecksumValidationStatusLabel": "Waliduj sumami kontrolnymi",
                 "linkConfigRemoteLibrariesStatusLabel": "Skonfiguruj brakuj\u0105ce biblioteki",
                 "linkDistributedWorkersStatusLabel": "Rozproszeni pracownicy",
                 "linkPreloadRemoteTasksStatusLabel": "Wst\u0119pne \u0142adowanie zada\u0144 zdalnych",
                 "linkReceivingTasksStatusLabel": "Odbieranie zada\u0144",
                 "linkSendingTasksStatusLabel": "Wysy\u0142anie zada\u0144",
                 "name": "Nazwa",
                 "nameThisInstall": "Nazwij t\u0119 instalacj\u0119",
@@ -135,15 +140,15 @@
                 "username": "Nazwa u\u017cytkownika",
                 "version": "Wersja",
                 "workerTarget": "Cel pracownika"
             },
             "pleaseEnterAValidNumber": "Prosz\u0119 wprowadzi\u0107 poprawny numer",
             "support": {
                 "apiSpec": "Specyfikacja API",
-                "appVersion": "Wersja niemaniakalna",
+                "appVersion": "Wersja Unmanic",
                 "applicationDocumentation": "Dokumentacja aplikacji",
                 "configPath": "\u015acie\u017cka konfiguracji",
                 "configuration": "Konfiguracja",
                 "currentSystemLogs": "Bie\u017c\u0105ce dzienniki systemowe",
                 "docs": "Dokumentacja",
                 "downloadSystemLogs": "Pobierz dzienniki systemowe",
                 "enableDebugging": "W\u0142\u0105cz debugowanie",
@@ -308,21 +313,24 @@
                 "error": "Na serwerze wyst\u0105pi\u0142 nieznany b\u0142\u0105d",
                 "info": "Nieznana wiadomo\u015b\u0107 z serwera",
                 "status": "Nieznana aktualizacja statusu z serwera",
                 "success": "Nieznana wiadomo\u015b\u0107 z serwera",
                 "warning": "Nieznane ostrze\u017cenie z serwera"
             },
             "incompatiblePlugin": "Unmanic przesta\u0142 przetwarza\u0107 zadania, poniewa\u017c wykry\u0142 niekompatybiln\u0105 wtyczk\u0119 w\u0142\u0105czon\u0105 w jednej z twoich bibliotek",
-            "libraryEnabledLimits": "Unmanic przesta\u0142 przetwarza\u0107 zadania, poniewa\u017c masz zbyt wiele bibliotek skonfigurowanych dla warstwy nieobs\u0142uguj\u0105cej. Rozwa\u017c sponsorowanie projektu, aby umo\u017cliwi\u0107 wi\u0119cej ni\u017c 2 bibliotekom.",
+            "libraryEnabledLimits": "Unmanic przesta\u0142 przetwarza\u0107 zadania, poniewa\u017c masz zbyt wiele bibliotek skonfigurowanych dla warstwy nieobs\u0142uguj\u0105cej. Rozwa\u017c sponsorowanie projektu, aby umo\u017cliwi\u0107 wi\u0119cej ni\u017c 2 biblioteki.",
             "libraryScanProgress": "Skanowanie biblioteki w toku",
             "linkedInstallationLimits": "Unmanic przesta\u0142 przetwarza\u0107 zadania, poniewa\u017c po\u0142\u0105czono zbyt wiele zdalnych instalacji dla warstwy nieobs\u0142uguj\u0105cej. Rozwa\u017c sponsorowanie projektu, aby po\u0142\u0105czy\u0107 wi\u0119cej ni\u017c jedn\u0105 instalacj\u0119 zdaln\u0105.",
             "pendingTaskHaltedPostProcessorQueueFull": "Kolejka postprocesora osi\u0105gn\u0119\u0142a sw\u00f3j limit",
             "pendingTaskHaltedPostProcessorQueueFullMessage": "Pracownicy nie otrzymaj\u0105 nowego oczekuj\u0105cego zadania, dop\u00f3ki kolejka postprocesora nie spadnie poni\u017cej aktualnie skonfigurowanej liczby pracownik\u00f3w",
-            "pluginSettingsChangeWorkersStopped": "Unmanic zatrzyma\u0142 wszystkich pracownik\u00f3w, poniewa\u017c wykry\u0142 zmian\u0119 w konfiguracji wtyczek. Kiedy b\u0119dziesz gotowy, wzn\u00f3w pracownik\u00f3w z pulpitu nawigacyjnego.",
+            "pluginSettingsChangeWorkersStopped": "Unmanic zatrzyma\u0142 wszystkich pracownik\u00f3w, poniewa\u017c wykry\u0142 zmian\u0119 w konfiguracji wtyczek. Gdy b\u0119dziesz gotowy, wzn\u00f3w pracownik\u00f3w z pulpitu nawigacyjnego.",
             "receivingRemoteFile": "Odbieranie zdalnego pliku"
+        },
+        "serverNotificationLabels": {
+            "failedTaskLabel": "Niepowodzenie zadania"
         }
     },
     "status": {
         "all": "Wszystko",
         "cannotLoadImage": "Nie mo\u017cna za\u0142adowa\u0107 obrazu",
         "disabled": "Wy\u0142\u0105czone",
         "enabled": "W\u0142\u0105czony",
@@ -333,15 +341,15 @@
     "tooltips": {
         "add": "Doda\u0107",
         "available": "Do dyspozycji",
         "back": "Z powrotem",
         "close": "Blisko",
         "configure": "Konfiguruj",
         "configureForThisLibrary": "Skonfiguruj dla tej biblioteki",
-        "defaultLibrary": "To jest biblioteka domy\u015blna. Nie mo\u017cna go usun\u0105\u0107.",
+        "defaultLibrary": "To jest domy\u015blna biblioteka. Nie mo\u017cna go usun\u0105\u0107.",
         "delete": "Usuwa\u0107",
         "etc": "Szacowany czas uko\u0144czenia",
         "install": "zainstalowa\u0107",
         "move": "Przenosi\u0107",
         "pluginInfo": "Informacje o wtyczce",
         "position": "Pozycja",
         "reinstall": "Zainstaluj ponownie",
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/language/ja.json` & `unmanic-0.2.4/unmanic/webserver/frontend/src/language/ja.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9095953363851745%*

 * *Differences: {"'buttons'": "{'dismissAll': 'すべて却下'}",*

 * * "'components'": "{'settings': {'library': {'name': '名前 (一意である必要があります)', 'path': 'ライブラリ パス', "*

 * *                 "'newLibrary': '新しい図書館', 'defaultLibrary': 'デフォルト ライブラリ', 'enableLibraryScanner': "*

 * *                 "'定期的なライブラリ スキャンを有効にする', 'libraryScannerSchedule': '数分でライブラリ スキャン スケジュール', "*

 * *                 "'libraryScannerScheduleNotValid': 'ライブラリ スキャン スケジュールが無効です', 'followSymlinks': "*

 * *                 "'ライブラリ スキャンでシンボリック リンクをたどる', 'runLibraryScanOnStart': '起動時に 1 回限り […]*

```diff
@@ -1,272 +1,277 @@
 {
     "buttons": {
         "darkMode": "\u30c0\u30fc\u30af\u30e2\u30fc\u30c9",
+        "dismissAll": "\u3059\u3079\u3066\u5374\u4e0b",
         "language": "\u8a00\u8a9e"
     },
     "components": {
         "completedTasks": {
-            "addToPendingTasksList": "\u9078\u629e\u3057\u305f\u3082\u306e\u3092[\u4fdd\u7559\u4e2d\u306e\u30bf\u30b9\u30af]\u30ea\u30b9\u30c8\u306b\u8ffd\u52a0",
+            "addToPendingTasksList": "\u9078\u629e\u3057\u305f\u30bf\u30b9\u30af\u3092\u4fdd\u7559\u4e2d\u306e\u30bf\u30b9\u30af \u30ea\u30b9\u30c8\u306b\u8ffd\u52a0",
             "before": "\u524d",
             "details": "\u8a73\u7d30",
             "errorGettingDetails": "\u3053\u306e\u30bf\u30b9\u30af\u306e\u8a73\u7d30\u3092\u53d6\u5f97\u4e2d\u306b\u30a8\u30e9\u30fc\u304c\u767a\u751f\u3057\u307e\u3057\u305f",
-            "removeSelected": "\u30ea\u30b9\u30c8\u304b\u3089\u9078\u629e\u3057\u305f\u3082\u306e\u3092\u524a\u9664",
-            "selectLibraryToAdd": "\u3053\u306e\u30bf\u30b9\u30af\u3092\u518d\u4f5c\u6210\u3059\u308b\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u9078\u629e\u3057\u307e\u3059",
+            "removeSelected": "\u9078\u629e\u3057\u305f\u3082\u306e\u3092\u30ea\u30b9\u30c8\u304b\u3089\u524a\u9664",
+            "selectLibraryToAdd": "\u3053\u306e\u30bf\u30b9\u30af\u3092\u518d\u4f5c\u6210\u3059\u308b\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u9078\u629e",
             "since": "\u4ee5\u6765"
         },
         "dataPanels": {
-            "noDataPanelsEnabled": "\u30c7\u30fc\u30bf\u30d1\u30cd\u30eb\u304c\u6709\u52b9\u306b\u306a\u3063\u3066\u3044\u307e\u305b\u3093\u3002\u30d7\u30e9\u30b0\u30a4\u30f3\u8a2d\u5b9a\u304b\u3089\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3057\u307e\u3059\u3002"
+            "noDataPanelsEnabled": "\u30c7\u30fc\u30bf \u30d1\u30cd\u30eb\u304c\u6709\u52b9\u306b\u306a\u3063\u3066\u3044\u307e\u305b\u3093\u3002\u30d7\u30e9\u30b0\u30a4\u30f3\u8a2d\u5b9a\u304b\u3089\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3057\u3066\u304f\u3060\u3055\u3044\u3002"
         },
         "footer": {
             "version": "\u30d0\u30fc\u30b8\u30e7\u30f3"
         },
         "pendingTasks": {
             "moveToBottom": "\u9078\u629e\u3057\u305f\u3082\u306e\u3092\u4e0b\u306b\u79fb\u52d5",
-            "moveToTop": "\u9078\u629e\u3057\u305f\u3082\u306e\u3092\u4e0a\u306b\u79fb\u52d5",
-            "removeSelected": "\u30ea\u30b9\u30c8\u304b\u3089\u9078\u629e\u3057\u305f\u3082\u306e\u3092\u524a\u9664",
-            "rescanLibrary": "\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u4eca\u3059\u3050\u518d\u30b9\u30ad\u30e3\u30f3"
+            "moveToTop": "\u9078\u629e\u3057\u305f\u3082\u306e\u3092\u4e00\u756a\u4e0a\u306b\u79fb\u52d5",
+            "removeSelected": "\u9078\u629e\u3057\u305f\u3082\u306e\u3092\u30ea\u30b9\u30c8\u304b\u3089\u524a\u9664",
+            "rescanLibrary": "\u4eca\u3059\u3050\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u518d\u30b9\u30ad\u30e3\u30f3"
         },
         "plugins": {
             "addRepository": "\u30ea\u30dd\u30b8\u30c8\u30ea\u3092\u8ffd\u52a0",
             "author": "\u8457\u8005",
-            "categoryFilter": "\u30ab\u30c6\u30b4\u30ea\u30d5\u30a3\u30eb\u30bf\u30fc",
-            "clickToUpdatePlugin": "\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u66f4\u65b0\u3059\u308b\u306b\u306f\u30af\u30ea\u30c3\u30af\u3057\u3066\u304f\u3060\u3055\u3044",
-            "errorSavingFlow": "\u30d7\u30e9\u30b0\u30a4\u30f3\u30d5\u30ed\u30fc\u306e\u4fdd\u5b58\u4e2d\u306b\u30a8\u30e9\u30fc\u304c\u767a\u751f\u3057\u307e\u3057\u305f",
+            "categoryFilter": "\u30ab\u30c6\u30b4\u30ea \u30d5\u30a3\u30eb\u30bf",
+            "clickToUpdatePlugin": "\u30af\u30ea\u30c3\u30af\u3057\u3066\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u66f4\u65b0",
+            "errorSavingFlow": "\u30d7\u30e9\u30b0\u30a4\u30f3 \u30d5\u30ed\u30fc\u306e\u4fdd\u5b58\u4e2d\u306b\u30a8\u30e9\u30fc\u304c\u767a\u751f\u3057\u307e\u3057\u305f",
+            "failedToInstallPluginFromZip": "\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u3055\u308c\u305f ZIP \u30d5\u30a1\u30a4\u30eb\u304b\u3089\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3067\u304d\u307e\u305b\u3093\u3067\u3057\u305f",
             "globalConfiguration": "\u30b0\u30ed\u30fc\u30d0\u30eb\u69cb\u6210",
-            "installPlugins": "\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3057\u307e\u3059",
+            "installPluginFromFile": "\u30d5\u30a1\u30a4\u30eb\u304b\u3089\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb",
+            "installPluginFromRepo": "\u30ec\u30dd\u304b\u3089\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb",
+            "installedPluginFromZip": "\u30d7\u30e9\u30b0\u30a4\u30f3\u304c\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3055\u308c\u3066\u3044\u307e\u3059",
+            "invalidZipFile": "\u30d5\u30a1\u30a4\u30eb\u306f\u6709\u52b9\u306a ZIP \u30d5\u30a1\u30a4\u30eb\u3067\u306f\u3042\u308a\u307e\u305b\u3093",
             "newRepository": "\u65b0\u3057\u3044\u30ea\u30dd\u30b8\u30c8\u30ea",
             "pluginUpToDate": "\u30d7\u30e9\u30b0\u30a4\u30f3\u306f\u6700\u65b0\u3067\u3059",
             "refreshRepositories": "\u30ea\u30dd\u30b8\u30c8\u30ea\u306e\u66f4\u65b0",
-            "removePlugin": "\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u524a\u9664\u3059\u308b",
+            "removePlugin": "\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u524a\u9664",
             "repo": "\u30ea\u30dd\u30b8\u30c8\u30ea",
-            "repoList": "\u30ea\u30dd\u30b8\u30c8\u30ea\u30ea\u30b9\u30c8",
+            "repoList": "\u30ea\u30dd\u30b8\u30c8\u30ea\u4e00\u89a7",
             "repoName": "\u540d\u524d",
-            "repoSource": "\u30ea\u30dd\u30b8\u30c8\u30ea\u306eURL",
-            "resetConfiguration": "\u69cb\u6210\u3092\u30ea\u30bb\u30c3\u30c8",
+            "repoSource": "\u30ea\u30dd\u30b8\u30c8\u30ea\u306e URL",
+            "resetConfiguration": "\u8a2d\u5b9a\u3092\u30ea\u30bb\u30c3\u30c8",
             "types": {
                 "libraryManagement": {
-                    "fileTest": "\u30e9\u30a4\u30d6\u30e9\u30ea\u7ba1\u7406-\u30d5\u30a1\u30a4\u30eb\u30c6\u30b9\u30c8",
-                    "fileTestCaption": "\u3053\u308c\u3089\u306e\u30d7\u30e9\u30b0\u30a4\u30f3\u306f\u3001\u30d5\u30a1\u30a4\u30eb\u3092\u4fdd\u7559\u4e2d\u306e\u30bf\u30b9\u30af\u30ea\u30b9\u30c8\u306b\u8ffd\u52a0\u3059\u308b\u5fc5\u8981\u304c\u3042\u308b\u304b\u3069\u3046\u304b\u3092\u30c6\u30b9\u30c8\u3059\u308b\u305f\u3081\u306b\u547c\u3073\u51fa\u3055\u308c\u307e\u3059"
+                    "fileTest": "\u30e9\u30a4\u30d6\u30e9\u30ea\u7ba1\u7406 - \u30d5\u30a1\u30a4\u30eb \u30c6\u30b9\u30c8",
+                    "fileTestCaption": "\u3053\u308c\u3089\u306e\u30d7\u30e9\u30b0\u30a4\u30f3\u306f\u3001\u4fdd\u7559\u4e2d\u306e\u30bf\u30b9\u30af \u30ea\u30b9\u30c8\u306b\u30d5\u30a1\u30a4\u30eb\u3092\u8ffd\u52a0\u3059\u308b\u5fc5\u8981\u304c\u3042\u308b\u304b\u3069\u3046\u304b\u3092\u30c6\u30b9\u30c8\u3059\u308b\u305f\u3081\u306b\u547c\u3073\u51fa\u3055\u308c\u307e\u3059\u3002"
                 },
                 "postprocessor": {
-                    "fileMove": "\u30dd\u30b9\u30c8\u30d7\u30ed\u30bb\u30c3\u30b5-\u30d5\u30a1\u30a4\u30eb\u306e\u79fb\u52d5",
-                    "fileMoveCaption": "\u3053\u308c\u3089\u306e\u30d7\u30e9\u30b0\u30a4\u30f3\u306f\u3001\u30bf\u30b9\u30af\u306e\u5b8c\u4e86\u6642\u306b\u547c\u3073\u51fa\u3055\u308c\u3001\u30d5\u30a1\u30a4\u30eb\u306e\u79fb\u52d5\u3092\u8ffd\u52a0\u3057\u307e\u3059",
-                    "taskResult": "\u30dd\u30b9\u30c8\u30d7\u30ed\u30bb\u30c3\u30b5-\u30bf\u30b9\u30af\u306e\u6210\u529f/\u5931\u6557\u306e\u30de\u30fc\u30ad\u30f3\u30b0",
+                    "fileMove": "\u30dd\u30b9\u30c8\u30d7\u30ed\u30bb\u30c3\u30b5\u30fc - \u30d5\u30a1\u30a4\u30eb\u79fb\u52d5",
+                    "fileMoveCaption": "\u3053\u308c\u3089\u306e\u30d7\u30e9\u30b0\u30a4\u30f3\u306f\u3001\u8ffd\u52a0\u306e\u30d5\u30a1\u30a4\u30eb\u79fb\u52d5\u3092\u8ffd\u52a0\u3059\u308b\u30bf\u30b9\u30af\u306e\u5b8c\u4e86\u6642\u306b\u547c\u3073\u51fa\u3055\u308c\u307e\u3059",
+                    "taskResult": "\u30dd\u30b9\u30c8\u30d7\u30ed\u30bb\u30c3\u30b5 - \u30bf\u30b9\u30af\u306e\u6210\u529f/\u5931\u6557\u306e\u30de\u30fc\u30ad\u30f3\u30b0",
                     "taskResultCaption": "\u3053\u308c\u3089\u306e\u30d7\u30e9\u30b0\u30a4\u30f3\u306f\u3001\u30bf\u30b9\u30af\u306e\u5b8c\u4e86\u6642\u306b\u547c\u3073\u51fa\u3055\u308c\u3001\u305d\u306e\u30bf\u30b9\u30af\u306e\u5168\u4f53\u7684\u306a\u6210\u529f\u307e\u305f\u306f\u5931\u6557\u3092\u30de\u30fc\u30af\u3057\u307e\u3059"
                 },
                 "worker": {
-                    "processItem": "\u30ef\u30fc\u30ab\u30fc-\u51e6\u7406\u30d5\u30a1\u30a4\u30eb",
-                    "processItemCaption": "\u3053\u308c\u3089\u306e\u30d7\u30e9\u30b0\u30a4\u30f3\u306f\u30ef\u30fc\u30ab\u30fc\u306b\u3088\u3063\u3066\u547c\u3073\u51fa\u3055\u308c\u3001\u305d\u306e\u30ef\u30fc\u30ab\u30fc\u306b\u3088\u3063\u3066\u5b9f\u884c\u304a\u3088\u3073\u7ba1\u7406\u3055\u308c\u308b\u30ab\u30b9\u30bf\u30e0\u30b3\u30de\u30f3\u30c9\u3092\u751f\u6210\u3057\u307e\u3059"
+                    "processItem": "\u30ef\u30fc\u30ab\u30fc - \u51e6\u7406\u4e2d\u306e\u30d5\u30a1\u30a4\u30eb",
+                    "processItemCaption": "\u3053\u308c\u3089\u306e\u30d7\u30e9\u30b0\u30a4\u30f3\u306f\u30ef\u30fc\u30ab\u30fc\u306b\u3088\u3063\u3066\u547c\u3073\u51fa\u3055\u308c\u3001\u305d\u306e\u30ef\u30fc\u30ab\u30fc\u306b\u3088\u3063\u3066\u5b9f\u884c\u304a\u3088\u3073\u7ba1\u7406\u3055\u308c\u308b\u30ab\u30b9\u30bf\u30e0 \u30b3\u30de\u30f3\u30c9\u3092\u751f\u6210\u3057\u307e\u3059\u3002"
                 }
             },
             "updateAvailable": "\u5229\u7528\u53ef\u80fd\u306a\u30a2\u30c3\u30d7\u30c7\u30fc\u30c8",
-            "updatePlugin": "\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u66f4\u65b0",
+            "updatePlugin": "\u30d7\u30e9\u30b0\u30a4\u30f3\u306e\u66f4\u65b0",
             "version": "\u30d0\u30fc\u30b8\u30e7\u30f3"
         },
         "settings": {
             "common": {
                 "configuration": "\u69cb\u6210",
                 "tags": "\u30bf\u30b0"
             },
             "library": {
-                "addPluginToThisLibrary": "\u3053\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u306b\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u8ffd\u52a0\u3057\u307e\u3059",
+                "addPluginToThisLibrary": "\u3053\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u306b\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u8ffd\u52a0",
                 "alwaysKeepFailedTasks": "\u5931\u6557\u3057\u305f\u30bf\u30b9\u30af\u3092\u5e38\u306b\u4fdd\u6301\u3059\u308b",
                 "autoManageCompletedTasks": "\u5b8c\u4e86\u3057\u305f\u30bf\u30b9\u30af\u3092\u81ea\u52d5\u7684\u306b\u7ba1\u7406\u3059\u308b",
-                "clearPendingTasksOnStart": "\u8d77\u52d5\u6642\u306b\u4fdd\u7559\u4e2d\u306e\u30bf\u30b9\u30af\u3092\u3059\u3079\u3066\u30af\u30ea\u30a2\u3059\u308b",
-                "cloneLibrary": "\u30af\u30ed\u30fc\u30f3\u30e9\u30a4\u30d6\u30e9\u30ea",
+                "clearPendingTasksOnStart": "\u8d77\u52d5\u6642\u306b\u3059\u3079\u3066\u306e\u4fdd\u7559\u4e2d\u306e\u30bf\u30b9\u30af\u3092\u30af\u30ea\u30a2\u3059\u308b",
+                "cloneLibrary": "\u30e9\u30a4\u30d6\u30e9\u30ea\u306e\u30af\u30ed\u30fc\u30f3",
                 "completedTasks": "\u5b8c\u4e86\u3057\u305f\u30bf\u30b9\u30af",
-                "concurrentFileTesters": "\u540c\u6642\u30d5\u30a1\u30a4\u30eb\u30c6\u30b9\u30bf\u30fc",
+                "concurrentFileTesters": "\u540c\u6642\u30d5\u30a1\u30a4\u30eb \u30c6\u30b9\u30bf\u30fc",
                 "confirmRemove": "\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u524a\u9664\u3059\u308b\u3068\u3001\u3053\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u306b\u95a2\u9023\u4ed8\u3051\u3089\u308c\u3066\u3044\u308b\u3059\u3079\u3066\u306e\u8a2d\u5b9a\u3082\u524a\u9664\u3055\u308c\u307e\u3059\u3002\u7d9a\u884c\u3057\u3066\u3082\u3088\u308d\u3057\u3044\u3067\u3059\u304b\uff1f",
-                "defaultLibrary": "\u30c7\u30d5\u30a9\u30eb\u30c8\u30e9\u30a4\u30d6\u30e9\u30ea",
-                "enableInotify": "\u3053\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u306e\u30d5\u30a1\u30a4\u30eb\u30e2\u30cb\u30bf\u30fc\u3092\u6709\u52b9\u306b\u3059\u308b",
-                "enableLibraryScanner": "\u5b9a\u671f\u7684\u306a\u30e9\u30a4\u30d6\u30e9\u30ea\u30b9\u30ad\u30e3\u30f3\u3092\u6709\u52b9\u306b\u3059\u308b",
-                "enableReceiveRemoteFilesOnly": "\u30ea\u30e2\u30fc\u30c8\u30d5\u30a1\u30a4\u30eb\u306e\u307f\u3092\u53d7\u4fe1\u3059\u308b\u3088\u3046\u306b\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u69cb\u6210\u3059\u308b",
-                "enableScanner": "\u3053\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u30b9\u30ad\u30e3\u30ca\u30fc\u3092\u6709\u52b9\u306b\u3059\u308b",
+                "defaultLibrary": "\u30c7\u30d5\u30a9\u30eb\u30c8 \u30e9\u30a4\u30d6\u30e9\u30ea",
+                "enableInotify": "\u3053\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u306e\u30d5\u30a1\u30a4\u30eb \u30e2\u30cb\u30bf\u30fc\u3092\u6709\u52b9\u306b\u3059\u308b",
+                "enableLibraryScanner": "\u5b9a\u671f\u7684\u306a\u30e9\u30a4\u30d6\u30e9\u30ea \u30b9\u30ad\u30e3\u30f3\u3092\u6709\u52b9\u306b\u3059\u308b",
+                "enableReceiveRemoteFilesOnly": "\u30ea\u30e2\u30fc\u30c8 \u30d5\u30a1\u30a4\u30eb\u306e\u307f\u3092\u53d7\u4fe1\u3059\u308b\u3088\u3046\u306b\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u69cb\u6210\u3059\u308b",
+                "enableScanner": "\u3053\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u306e\u30e9\u30a4\u30d6\u30e9\u30ea \u30b9\u30ad\u30e3\u30ca\u3092\u6709\u52b9\u306b\u3059\u308b",
                 "exportLibraryConfig": "\u69cb\u6210\u306e\u30a8\u30af\u30b9\u30dd\u30fc\u30c8",
-                "fileTesting": "\u30d5\u30a1\u30a4\u30eb\u30c6\u30b9\u30c8",
-                "followSymlinks": "\u30e9\u30a4\u30d6\u30e9\u30ea\u30b9\u30ad\u30e3\u30f3\u3067\u30b7\u30f3\u30dc\u30ea\u30c3\u30af\u30ea\u30f3\u30af\u3092\u305f\u3069\u308b",
+                "fileTesting": "\u30d5\u30a1\u30a4\u30eb\u306e\u30c6\u30b9\u30c8",
+                "followSymlinks": "\u30e9\u30a4\u30d6\u30e9\u30ea \u30b9\u30ad\u30e3\u30f3\u3067\u30b7\u30f3\u30dc\u30ea\u30c3\u30af \u30ea\u30f3\u30af\u3092\u305f\u3069\u308b",
                 "importLibraryConfig": "\u69cb\u6210\u306e\u30a4\u30f3\u30dd\u30fc\u30c8",
-                "importPluginConfigMessage": "\u30e9\u30a4\u30d6\u30e9\u30ea\u69cb\u6210\u306e\u30a4\u30f3\u30dd\u30fc\u30c8\u3002\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u304c\u5fc5\u8981\u306a\u30d7\u30e9\u30b0\u30a4\u30f3\u304c\u3042\u308b\u5834\u5408\u3001\u3053\u308c\u306b\u306f\u6642\u9593\u304c\u304b\u304b\u308b\u5834\u5408\u304c\u3042\u308a\u307e\u3059\u3002",
+                "importPluginConfigMessage": "\u30e9\u30a4\u30d6\u30e9\u30ea\u69cb\u6210\u3092\u30a4\u30f3\u30dd\u30fc\u30c8\u3057\u3066\u3044\u307e\u3059\u3002\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u304c\u5fc5\u8981\u306a\u30d7\u30e9\u30b0\u30a4\u30f3\u304c\u3042\u308b\u5834\u5408\u3001\u3053\u308c\u306b\u306f\u6642\u9593\u304c\u304b\u304b\u308b\u5834\u5408\u304c\u3042\u308a\u307e\u3059\u3002",
                 "libraryFileMonitorStatusLabel": "\u30d5\u30a1\u30a4\u30eb\u30e2\u30cb\u30bf\u30fc",
                 "libraryRemoteOnlyStatus": "\u30ea\u30e2\u30fc\u30c8\u306e\u307f",
                 "libraryScanner": "\u30e9\u30a4\u30d6\u30e9\u30ea\u30b9\u30ad\u30e3\u30ca\u30fc",
-                "libraryScannerSchedule": "\u6570\u5206\u3067\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u30b9\u30ad\u30e3\u30f3\u30b9\u30b1\u30b8\u30e5\u30fc\u30eb",
-                "libraryScannerScheduleNotValid": "\u30e9\u30a4\u30d6\u30e9\u30ea\u30b9\u30ad\u30e3\u30f3\u30b9\u30b1\u30b8\u30e5\u30fc\u30eb\u304c\u7121\u52b9\u3067\u3059",
+                "libraryScannerSchedule": "\u6570\u5206\u3067\u30e9\u30a4\u30d6\u30e9\u30ea \u30b9\u30ad\u30e3\u30f3 \u30b9\u30b1\u30b8\u30e5\u30fc\u30eb",
+                "libraryScannerScheduleNotValid": "\u30e9\u30a4\u30d6\u30e9\u30ea \u30b9\u30ad\u30e3\u30f3 \u30b9\u30b1\u30b8\u30e5\u30fc\u30eb\u304c\u7121\u52b9\u3067\u3059",
                 "libraryScannerStatusLabel": "\u30e9\u30a4\u30d6\u30e9\u30ea\u30b9\u30ad\u30e3\u30ca\u30fc",
-                "locked": "\u30e9\u30a4\u30d6\u30e9\u30ea\u306f\u524a\u9664\u3067\u304d\u307e\u305b\u3093",
+                "locked": "\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u524a\u9664\u3067\u304d\u307e\u305b\u3093",
                 "maxAgeOfCompletedTasks": "\u5b8c\u4e86\u3057\u305f\u30bf\u30b9\u30af\u3092\u4fdd\u6301\u3059\u308b\u6700\u5927\u65e5\u6570",
-                "name": "\u540d\u524d\uff08\u4e00\u610f\u3067\u3042\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\uff09",
-                "newLibrary": "\u65b0\u3057\u3044\u30e9\u30a4\u30d6\u30e9\u30ea",
-                "path": "\u30e9\u30a4\u30d6\u30e9\u30ea\u30d1\u30b9",
+                "name": "\u540d\u524d (\u4e00\u610f\u3067\u3042\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059)",
+                "newLibrary": "\u65b0\u3057\u3044\u56f3\u66f8\u9928",
+                "path": "\u30e9\u30a4\u30d6\u30e9\u30ea \u30d1\u30b9",
                 "pathConfiguration": "\u30e9\u30a4\u30d6\u30e9\u30ea",
-                "pathDisabledReceiveRemoteFilesOnly": "\u30ea\u30e2\u30fc\u30c8\u30d5\u30a1\u30a4\u30eb\u306e\u307f\u3092\u53d7\u4fe1\u3059\u308b\u3088\u3046\u306b\u3053\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u69cb\u6210\u3057\u305f\u305f\u3081\u3001\u30aa\u30d7\u30b7\u30e7\u30f3\u304c\u7121\u52b9\u306b\u306a\u308a\u307e\u3057\u305f",
+                "pathDisabledReceiveRemoteFilesOnly": "\u30ea\u30e2\u30fc\u30c8 \u30d5\u30a1\u30a4\u30eb\u306e\u307f\u3092\u53d7\u4fe1\u3059\u308b\u3088\u3046\u306b\u3053\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u69cb\u6210\u3057\u3066\u3044\u308b\u305f\u3081\u3001\u30aa\u30d7\u30b7\u30e7\u30f3\u306f\u7121\u52b9\u306b\u306a\u3063\u3066\u3044\u307e\u3059",
                 "pendingTasks": "\u4fdd\u7559\u4e2d\u306e\u30bf\u30b9\u30af",
-                "pluginFlow": "\u30d7\u30e9\u30b0\u30a4\u30f3\u30d5\u30ed\u30fc",
+                "pluginFlow": "\u30d7\u30e9\u30b0\u30a4\u30f3\u306e\u6d41\u308c",
                 "plugins": "\u30d7\u30e9\u30b0\u30a4\u30f3",
                 "priorityScore": "\u3053\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u7528\u306b\u751f\u6210\u3055\u308c\u305f\u30bf\u30b9\u30af\u306e\u512a\u5148\u5ea6\u30b9\u30b3\u30a2\u4fee\u98fe\u5b50\u3092\u8a2d\u5b9a\u3057\u307e\u3059",
-                "runLibraryScanOnStart": "\u8d77\u52d5\u6642\u306b1\u56de\u9650\u308a\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u30b9\u30ad\u30e3\u30f3\u3092\u5b9f\u884c\u3059\u308b",
-                "unlocked": "\u30e9\u30a4\u30d6\u30e9\u30ea\u306f\u524a\u9664\u3067\u304d\u307e\u3059"
+                "runLibraryScanOnStart": "\u8d77\u52d5\u6642\u306b 1 \u56de\u9650\u308a\u306e\u30e9\u30a4\u30d6\u30e9\u30ea \u30b9\u30ad\u30e3\u30f3\u3092\u5b9f\u884c\u3059\u308b",
+                "unlocked": "\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u524a\u9664\u3067\u304d\u307e\u3059"
             },
             "link": {
                 "add": "\u8ffd\u52a0",
-                "addRemoteInstallation": "\u30ea\u30e2\u30fc\u30c8\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3092\u8ffd\u52a0\u3059\u308b",
+                "addRemoteInstallation": "\u30ea\u30e2\u30fc\u30c8 \u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3092\u8ffd\u52a0\u3059\u308b",
                 "address": "\u4f4f\u6240",
-                "allowReceivingTasks": "\u30ef\u30fc\u30ab\u30fc\u304c\u5229\u7528\u53ef\u80fd\u306b\u306a\u3063\u305f\u3068\u304d\u306b\u3001\u3053\u306e\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u304b\u3089\u30bf\u30b9\u30af\u3092\u53d7\u3051\u53d6\u308a\u307e\u3059",
+                "allowReceivingTasks": "\u30ef\u30fc\u30ab\u30fc\u304c\u5229\u7528\u53ef\u80fd\u306a\u3068\u304d\u306b\u3001\u3053\u306e\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u304b\u3089\u30bf\u30b9\u30af\u3092\u53d7\u3051\u53d6\u308a\u307e\u3059",
                 "allowSendingTasks": "\u30ef\u30fc\u30ab\u30fc\u304c\u5229\u7528\u53ef\u80fd\u306b\u306a\u3063\u305f\u3089\u3001\u3053\u306e\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u306b\u30bf\u30b9\u30af\u3092\u9001\u4fe1\u3057\u307e\u3059",
                 "authentication": "\u8a8d\u8a3c",
-                "collectiveManagement": "\u96c6\u56e3\u7684\u7ba1\u7406",
+                "collectiveManagement": "\u4e00\u62ec\u7ba1\u7406",
                 "connection": "\u7e4b\u304c\u308a",
-                "enableChecksumValidation": "\u30c1\u30a7\u30c3\u30af\u30b5\u30e0\u3092\u4f7f\u7528\u3057\u3066\u30d5\u30a1\u30a4\u30eb\u8ee2\u9001\u3092\u691c\u8a3c\u3059\u308b\uff08\u9045\u3044\uff09",
-                "enableConfigMissingLibraries": "\u30ea\u30e2\u30fc\u30c8\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3067\u4e0d\u8db3\u3057\u3066\u3044\u308b\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u81ea\u52d5\u7684\u306b\u69cb\u6210\u3059\u308b",
+                "enableChecksumValidation": "\u30c1\u30a7\u30c3\u30af\u30b5\u30e0\u3092\u4f7f\u7528\u3057\u3066\u30d5\u30a1\u30a4\u30eb\u8ee2\u9001\u3092\u691c\u8a3c\u3059\u308b (\u9045\u3044)",
+                "enableConfigMissingLibraries": "\u30ea\u30e2\u30fc\u30c8 \u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3067\u4e0d\u8db3\u3057\u3066\u3044\u308b\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u81ea\u52d5\u7684\u306b\u69cb\u6210\u3059\u308b",
                 "enableDistributedWorkerCount": "\u3053\u306e\u30ea\u30f3\u30af\u306e\u5206\u6563\u30ef\u30fc\u30ab\u30fc\u6570\u3092\u6709\u52b9\u306b\u3059\u308b",
-                "enableTaskPreloading": "\u30ea\u30e2\u30fc\u30c8\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u306e\u4fdd\u7559\u4e2d\u306e\u30bf\u30b9\u30af\u30ad\u30e5\u30fc\u306b\u3044\u304f\u3064\u304b\u306e\u30bf\u30b9\u30af\u3092\u30d7\u30ea\u30ed\u30fc\u30c9\u3057\u307e\u3059",
+                "enableTaskPreloading": "\u30ea\u30e2\u30fc\u30c8 \u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u306e\u4fdd\u7559\u4e2d\u306e\u30bf\u30b9\u30af \u30ad\u30e5\u30fc\u306b\u3044\u304f\u3064\u304b\u306e\u30bf\u30b9\u30af\u3092\u30d7\u30ea\u30ed\u30fc\u30c9\u3057\u307e\u3059\u3002",
                 "linkConfigChecksumValidationStatusLabel": "\u30c1\u30a7\u30c3\u30af\u30b5\u30e0\u3067\u691c\u8a3c\u3059\u308b",
                 "linkConfigRemoteLibrariesStatusLabel": "\u4e0d\u8db3\u3057\u3066\u3044\u308b\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u69cb\u6210\u3059\u308b",
-                "linkDistributedWorkersStatusLabel": "\u5206\u6563\u578b\u30ef\u30fc\u30ab\u30fc",
-                "linkPreloadRemoteTasksStatusLabel": "\u30ea\u30e2\u30fc\u30c8\u30bf\u30b9\u30af\u3092\u30d7\u30ea\u30ed\u30fc\u30c9\u3059\u308b",
-                "linkReceivingTasksStatusLabel": "\u30bf\u30b9\u30af\u306e\u53d7\u4fe1",
+                "linkDistributedWorkersStatusLabel": "\u5206\u6563\u30ef\u30fc\u30ab\u30fc",
+                "linkPreloadRemoteTasksStatusLabel": "\u30ea\u30e2\u30fc\u30c8 \u30bf\u30b9\u30af\u3092\u30d7\u30ea\u30ed\u30fc\u30c9\u3059\u308b",
+                "linkReceivingTasksStatusLabel": "\u53d7\u4ed8\u696d\u52d9",
                 "linkSendingTasksStatusLabel": "\u30bf\u30b9\u30af\u306e\u9001\u4fe1",
                 "name": "\u540d\u524d",
                 "nameThisInstall": "\u3053\u306e\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u306b\u540d\u524d\u3092\u4ed8\u3051\u308b",
                 "password": "\u30d1\u30b9\u30ef\u30fc\u30c9",
                 "preloadingCount": "\u30d7\u30ea\u30ed\u30fc\u30c9\u3055\u308c\u305f\u4fdd\u7559\u4e2d\u306e\u30bf\u30b9\u30af\u6570",
                 "remoteInstallations": "\u30ea\u30e2\u30fc\u30c8\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb",
                 "remoteTaskProcessing": "\u30ea\u30e2\u30fc\u30c8\u30bf\u30b9\u30af\u51e6\u7406",
                 "thisInstallation": "\u30ed\u30fc\u30ab\u30eb",
                 "username": "\u30e6\u30fc\u30b6\u30fc\u540d",
                 "version": "\u30d0\u30fc\u30b8\u30e7\u30f3",
-                "workerTarget": "\u52b4\u50cd\u8005\u306e\u76ee\u6a19"
+                "workerTarget": "\u30ef\u30fc\u30ab\u30fc \u30bf\u30fc\u30b2\u30c3\u30c8"
             },
             "pleaseEnterAValidNumber": "\u6709\u52b9\u306a\u6570\u5024\u3092\u5165\u529b\u3057\u3066\u304f\u3060\u3055\u3044",
             "support": {
-                "apiSpec": "API\u4ed5\u69d8",
-                "appVersion": "Unmanic\u30d0\u30fc\u30b8\u30e7\u30f3",
-                "applicationDocumentation": "\u30a2\u30d7\u30ea\u30b1\u30fc\u30b7\u30e7\u30f3\u30c9\u30ad\u30e5\u30e1\u30f3\u30c8",
+                "apiSpec": "API \u4ed5\u69d8",
+                "appVersion": "\u30a2\u30f3\u30de\u30cb\u30c3\u30af\u30d0\u30fc\u30b8\u30e7\u30f3",
+                "applicationDocumentation": "\u30a2\u30d7\u30ea\u30b1\u30fc\u30b7\u30e7\u30f3 \u30c9\u30ad\u30e5\u30e1\u30f3\u30c8",
                 "configPath": "\u69cb\u6210\u30d1\u30b9",
                 "configuration": "\u69cb\u6210",
-                "currentSystemLogs": "\u73fe\u5728\u306e\u30b7\u30b9\u30c6\u30e0\u30ed\u30b0",
+                "currentSystemLogs": "\u73fe\u5728\u306e\u30b7\u30b9\u30c6\u30e0 \u30ed\u30b0",
                 "docs": "\u30c9\u30ad\u30e5\u30e1\u30f3\u30c6\u30fc\u30b7\u30e7\u30f3",
-                "downloadSystemLogs": "\u30b7\u30b9\u30c6\u30e0\u30ed\u30b0\u3092\u30c0\u30a6\u30f3\u30ed\u30fc\u30c9\u3059\u308b",
-                "enableDebugging": "EnableDebugging",
+                "downloadSystemLogs": "\u30b7\u30b9\u30c6\u30e0 \u30ed\u30b0\u306e\u30c0\u30a6\u30f3\u30ed\u30fc\u30c9",
+                "enableDebugging": "\u30c7\u30d0\u30c3\u30b0\u3092\u6709\u52b9\u306b\u3059\u308b",
                 "logs": "\u30ed\u30b0",
-                "logsPath": "\u30ed\u30b0\u30d1\u30b9",
-                "platform": "\u30d7\u30e9\u30c3\u30c8\u30d5\u30a9\u30fc\u30e0\uff08\u30aa\u30da\u30ec\u30fc\u30c6\u30a3\u30f3\u30b0\u30b7\u30b9\u30c6\u30e0\uff09",
-                "pythonVersion": "Python\u30d0\u30fc\u30b8\u30e7\u30f3",
+                "logsPath": "\u30ed\u30b0\u306e\u30d1\u30b9",
+                "platform": "\u30d7\u30e9\u30c3\u30c8\u30d5\u30a9\u30fc\u30e0 (\u30aa\u30da\u30ec\u30fc\u30c6\u30a3\u30f3\u30b0 \u30b7\u30b9\u30c6\u30e0)",
+                "pythonVersion": "Python \u30d0\u30fc\u30b8\u30e7\u30f3",
                 "support": "\u30b5\u30dd\u30fc\u30c8",
-                "unmanicAppSourceRequests": "Unmanic\u30a2\u30d7\u30ea\u30b1\u30fc\u30b7\u30e7\u30f3\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u6a5f\u80fd",
-                "unmanicFrontendSourceRequests": "Unmanic\u30d5\u30ed\u30f3\u30c8\u30a8\u30f3\u30c9\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u6a5f\u80fd",
-                "unmanicOfficialPluginRequests": "Unmanic\u306e\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u30ea\u30af\u30a8\u30b9\u30c8\u3059\u308b",
-                "userdataPath": "\u30e6\u30fc\u30b6\u30fc\u30c7\u30fc\u30bf\u30d1\u30b9"
+                "unmanicAppSourceRequests": "Unmanic Application \u306e\u30ea\u30af\u30a8\u30b9\u30c8\u6a5f\u80fd",
+                "unmanicFrontendSourceRequests": "Unmanic Frontend \u306e\u30ea\u30af\u30a8\u30b9\u30c8\u6a5f\u80fd",
+                "unmanicOfficialPluginRequests": "Unmanic \u306e\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u30ea\u30af\u30a8\u30b9\u30c8\u3059\u308b",
+                "userdataPath": "\u30e6\u30fc\u30b6\u30fc\u30c7\u30fc\u30bf \u30d1\u30b9"
             },
             "workers": {
                 "addEvent": "\u30a4\u30d9\u30f3\u30c8\u3092\u8ffd\u52a0",
-                "confirmRemove": "\u30ef\u30fc\u30ab\u30fc\u30b0\u30eb\u30fc\u30d7\u3092\u524a\u9664\u3059\u308b\u3068\u3001\u30b0\u30eb\u30fc\u30d7\u306b\u95a2\u9023\u4ed8\u3051\u3089\u308c\u3066\u3044\u308b\u3059\u3079\u3066\u306e\u8a2d\u5b9a\u3082\u524a\u9664\u3055\u308c\u307e\u3059\u3002\u7d9a\u884c\u3057\u3066\u3082\u3088\u308d\u3057\u3044\u3067\u3059\u304b\uff1f",
-                "locked": "\u30ef\u30fc\u30ab\u30fc\u30b0\u30eb\u30fc\u30d7\u306f\u524a\u9664\u3067\u304d\u307e\u305b\u3093",
-                "newScheduledEvent": "\u65b0\u3057\u3044\u30b9\u30b1\u30b8\u30e5\u30fc\u30eb\u3055\u308c\u305f\u30a4\u30d9\u30f3\u30c8",
-                "path": "\u30ad\u30e3\u30c3\u30b7\u30e5\u30d1\u30b9",
+                "confirmRemove": "\u30ef\u30fc\u30ab\u30fc \u30b0\u30eb\u30fc\u30d7\u3092\u524a\u9664\u3059\u308b\u3068\u3001\u30b0\u30eb\u30fc\u30d7\u306b\u95a2\u9023\u4ed8\u3051\u3089\u308c\u3066\u3044\u308b\u3059\u3079\u3066\u306e\u8a2d\u5b9a\u3082\u524a\u9664\u3055\u308c\u307e\u3059\u3002\u7d9a\u884c\u3057\u3066\u3082\u3088\u308d\u3057\u3044\u3067\u3059\u304b\uff1f",
+                "locked": "\u30ef\u30fc\u30ab\u30fc \u30b0\u30eb\u30fc\u30d7\u3092\u524a\u9664\u3067\u304d\u307e\u305b\u3093",
+                "newScheduledEvent": "\u65b0\u305f\u306b\u958b\u50ac\u4e88\u5b9a\u306e\u30a4\u30d9\u30f3\u30c8",
+                "path": "\u30ad\u30e3\u30c3\u30b7\u30e5 \u30d1\u30b9",
                 "repetition": "\u7e70\u308a\u8fd4\u3057",
-                "schedule": "\u52b4\u50cd\u8005\u306e\u30a4\u30d9\u30f3\u30c8\u30b9\u30b1\u30b8\u30e5\u30fc\u30eb",
+                "schedule": "\u30ef\u30fc\u30ab\u30fc \u30a4\u30d9\u30f3\u30c8 \u30b9\u30b1\u30b8\u30e5\u30fc\u30eb",
                 "scheduleLabels": {
-                    "count": "\u30ef\u30fc\u30ab\u30fc\u6570\u3092\u8a2d\u5b9a\u3059\u308b",
+                    "count": "\u30ef\u30fc\u30ab\u30fc\u6570\u306e\u8a2d\u5b9a",
                     "daily": "\u6bce\u65e5",
                     "friday": "\u6bce\u9031\u91d1\u66dc\u65e5",
                     "monday": "\u6bce\u9031\u6708\u66dc\u65e5",
-                    "pause": "\u3059\u3079\u3066\u306e\u52b4\u50cd\u8005\u3092\u4e00\u6642\u505c\u6b62\u3057\u307e\u3059",
-                    "resume": "\u3059\u3079\u3066\u306e\u52b4\u50cd\u8005\u3092\u518d\u958b\u3059\u308b",
+                    "pause": "\u3059\u3079\u3066\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u4e00\u6642\u505c\u6b62",
+                    "resume": "\u3059\u3079\u3066\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u518d\u958b\u3059\u308b",
                     "saturday": "\u6bce\u9031\u571f\u66dc\u65e5\u306b",
                     "sunday": "\u6bce\u9031\u65e5\u66dc\u65e5\u306b",
                     "thursday": "\u6bce\u9031\u6728\u66dc\u65e5\u306b",
                     "tuesday": "\u6bce\u9031\u706b\u66dc\u65e5",
                     "wednesday": "\u6bce\u9031\u6c34\u66dc\u65e5",
-                    "weekday": "\u6bce\u9031\u5e73\u65e5",
+                    "weekday": "\u5e73\u65e5",
                     "weekend": "\u6bce\u9031\u571f\u66dc\u65e5\u3068\u65e5\u66dc\u65e5"
                 },
                 "task": "\u4ed5\u4e8b",
-                "unlocked": "\u30ef\u30fc\u30ab\u30fc\u30b0\u30eb\u30fc\u30d7\u306f\u524a\u9664\u3067\u304d\u307e\u3059",
-                "workerCount": "\u52b4\u50cd\u8005\u6570",
+                "unlocked": "\u30ef\u30fc\u30ab\u30fc \u30b0\u30eb\u30fc\u30d7\u3092\u524a\u9664\u3067\u304d\u307e\u3059",
+                "workerCount": "\u30ef\u30fc\u30ab\u30fc\u6570",
                 "workerGroupName": "\u30b0\u30eb\u30fc\u30d7\u540d",
                 "workerGroups": "\u52b4\u50cd\u8005\u30b0\u30eb\u30fc\u30d7"
             }
         },
         "workers": {
             "currentRunner": {
                 "indeterminate": "\u4e0d\u5b9a",
                 "none": "\u306a\u3057"
             },
             "currentRunnerLabel": "\u73fe\u5728\u306e\u30e9\u30f3\u30ca\u30fc",
-            "listEmpty": "\u73fe\u5728\u5b9f\u884c\u4e2d\u306e\u30ef\u30fc\u30ab\u30fc\u306f\u3042\u308a\u307e\u305b\u3093\u3002 Unmanic\u306e\u8a2d\u5b9a\u3067\u30ef\u30fc\u30ab\u30fc\u6570\u3092\u5897\u3084\u3057\u3066\u3001\u30ef\u30fc\u30ab\u30fc\u3092\u751f\u6210\u3057\u307e\u3059\u3002",
-            "pauseAllWorkers": "\u3059\u3079\u3066\u306e\u52b4\u50cd\u8005\u3092\u4e00\u6642\u505c\u6b62\u3057\u307e\u3059",
-            "pauseWorker": "\u3053\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u4e00\u6642\u505c\u6b62\u3057\u307e\u3059",
-            "resumeAllWorkers": "\u3059\u3079\u3066\u306e\u52b4\u50cd\u8005\u3092\u518d\u958b\u3059\u308b",
-            "resumeWorker": "\u3053\u306e\u52b4\u50cd\u8005\u3092\u518d\u958b\u3059\u308b",
+            "listEmpty": "\u73fe\u5728\u5b9f\u884c\u4e2d\u306e\u30ef\u30fc\u30ab\u30fc\u306f\u3042\u308a\u307e\u305b\u3093\u3002 Unmanic \u306e\u8a2d\u5b9a\u3067\u30ef\u30fc\u30ab\u30fc\u6570\u3092\u5897\u3084\u3057\u3066\u3001\u30ef\u30fc\u30ab\u30fc\u3092\u30b9\u30dd\u30fc\u30f3\u3057\u307e\u3059\u3002",
+            "pauseAllWorkers": "\u3059\u3079\u3066\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u4e00\u6642\u505c\u6b62",
+            "pauseWorker": "\u3053\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u4e00\u6642\u505c\u6b62",
+            "resumeAllWorkers": "\u3059\u3079\u3066\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u518d\u958b\u3059\u308b",
+            "resumeWorker": "\u3053\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u518d\u958b\u3057\u307e\u3059",
             "startTimeLabel": "\u59cb\u307e\u308b\u6642\u9593",
             "state": {
-                "paused": "\u52b4\u50cd\u8005\u306f\u4e00\u6642\u505c\u6b62\u3057\u307e\u3057\u305f...",
-                "processing": "\u51e6\u7406\u30bf\u30b9\u30af...",
+                "paused": "\u30ef\u30fc\u30ab\u30fc\u304c\u4e00\u6642\u505c\u6b62\u3057\u307e\u3057\u305f...",
+                "processing": "\u30bf\u30b9\u30af\u3092\u51e6\u7406\u3057\u3066\u3044\u307e\u3059...",
                 "waiting": "\u5225\u306e\u30bf\u30b9\u30af\u3092\u5f85\u3063\u3066\u3044\u307e\u3059..."
             },
             "stateLabel": "\u5dde",
             "status": "\u72b6\u614b",
-            "terminateAllWorkers": "\u3059\u3079\u3066\u306e\u52b4\u50cd\u8005\u3092\u7d42\u4e86\u3059\u308b",
+            "terminateAllWorkers": "\u3059\u3079\u3066\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u7d42\u4e86\u3059\u308b",
             "terminateWorker": "\u3053\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u7d42\u4e86\u3057\u307e\u3059",
-            "terminateWorkerWarning": "\u3053\u306e\u30ef\u30fc\u30ab\u30fc\u3068\u305d\u306e\u73fe\u5728\u306e\u30bf\u30b9\u30af\u3092\u7d42\u4e86\u3057\u3066\u3082\u3088\u308d\u3057\u3044\u3067\u3059\u304b\uff1f\u73fe\u5728\u306e\u30bf\u30b9\u30af\u306f\u3001\u5b8c\u4e86\u3057\u305f\u30bf\u30b9\u30af\u30ea\u30b9\u30c8\u3067\u5931\u6557\u3068\u3057\u3066\u30de\u30fc\u30af\u3055\u308c\u307e\u3059\u3002",
-            "totalProcessingTimeLabel": "\u7dcf\u51e6\u7406\u6642\u9593",
-            "workerLog": "\u52b4\u50cd\u8005\u30ed\u30b0",
-            "workerPaused": "\u52b4\u50cd\u8005\u306f\u4e00\u6642\u505c\u6b62\u3055\u308c\u307e\u3057\u305f",
-            "workerPausedFailed": "Unmanic\u306f\u3001\u4f55\u3089\u304b\u306e\u7406\u7531\u3067\u3053\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u4e00\u6642\u505c\u6b62\u3067\u304d\u307e\u305b\u3093\u3067\u3057\u305f",
-            "workerResumed": "\u52b4\u50cd\u8005\u304c\u518d\u958b\u3055\u308c\u307e\u3057\u305f",
-            "workerResumedFailed": "Unmanic\u306f\u3001\u4f55\u3089\u304b\u306e\u7406\u7531\u3067\u3053\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u518d\u958b\u3067\u304d\u307e\u305b\u3093\u3067\u3057\u305f",
-            "workerTerminated": "\u52b4\u50cd\u8005\u306f\u89e3\u96c7\u3055\u308c\u307e\u3057\u305f",
-            "workerTerminationFailed": "Unmanic\u306f\u3001\u4f55\u3089\u304b\u306e\u7406\u7531\u3067\u3053\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u7d42\u4e86\u3067\u304d\u307e\u305b\u3093\u3067\u3057\u305f"
+            "terminateWorkerWarning": "\u3053\u306e\u30ef\u30fc\u30ab\u30fc\u3068\u305d\u306e\u73fe\u5728\u306e\u30bf\u30b9\u30af\u3092\u7d42\u4e86\u3057\u3066\u3082\u3088\u308d\u3057\u3044\u3067\u3059\u304b?\u73fe\u5728\u306e\u30bf\u30b9\u30af\u306f\u3001\u5b8c\u4e86\u3057\u305f\u30bf\u30b9\u30af \u30ea\u30b9\u30c8\u3067\u5931\u6557\u3068\u3057\u3066\u30de\u30fc\u30af\u3055\u308c\u307e\u3059\u3002",
+            "totalProcessingTimeLabel": "\u5408\u8a08\u51e6\u7406\u6642\u9593",
+            "workerLog": "\u30ef\u30fc\u30ab\u30fc\u30ed\u30b0",
+            "workerPaused": "\u30ef\u30fc\u30ab\u30fc\u304c\u4e00\u6642\u505c\u6b62\u3057\u307e\u3057\u305f",
+            "workerPausedFailed": "Unmanic \u306f\u4f55\u3089\u304b\u306e\u7406\u7531\u3067\u3053\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u4e00\u6642\u505c\u6b62\u3067\u304d\u307e\u305b\u3093\u3067\u3057\u305f",
+            "workerResumed": "\u30ef\u30fc\u30ab\u30fc\u304c\u518d\u958b\u3055\u308c\u307e\u3057\u305f",
+            "workerResumedFailed": "Unmanic \u306f\u4f55\u3089\u304b\u306e\u7406\u7531\u3067\u3053\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u518d\u958b\u3067\u304d\u307e\u305b\u3093\u3067\u3057\u305f",
+            "workerTerminated": "\u30ef\u30fc\u30ab\u30fc\u306f\u7d42\u4e86\u3057\u307e\u3057\u305f",
+            "workerTerminationFailed": "Unmanic \u306f\u4f55\u3089\u304b\u306e\u7406\u7531\u3067\u3053\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u7d42\u4e86\u3067\u304d\u307e\u305b\u3093\u3067\u3057\u305f"
         }
     },
     "headers": {
         "completedTaskDetails": "\u5b8c\u4e86\u3057\u305f\u30bf\u30b9\u30af\u306e\u8a73\u7d30",
         "completedTasks": "\u5b8c\u4e86\u3057\u305f\u30bf\u30b9\u30af",
-        "configureLibrary": "\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u69cb\u6210\u3059\u308b",
-        "configureRemoteInstallationLink": "\u30ea\u30e2\u30fc\u30c8\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u30ea\u30f3\u30af\u3092\u69cb\u6210\u3059\u308b",
-        "configureWorkerGroup": "\u30ef\u30fc\u30ab\u30fc\u30b0\u30eb\u30fc\u30d7\u3092\u69cb\u6210\u3059\u308b",
+        "configureLibrary": "\u30e9\u30a4\u30d6\u30e9\u30ea\u306e\u69cb\u6210",
+        "configureRemoteInstallationLink": "\u30ea\u30e2\u30fc\u30c8 \u30a4\u30f3\u30b9\u30c8\u30fc\u30eb \u30ea\u30f3\u30af\u306e\u69cb\u6210",
+        "configureWorkerGroup": "\u30ef\u30fc\u30ab\u30fc \u30b0\u30eb\u30fc\u30d7\u306e\u69cb\u6210",
         "confirm": "\u78ba\u8a8d",
-        "globalPluginConfig": "\u30b0\u30ed\u30fc\u30d0\u30eb\u30d7\u30e9\u30b0\u30a4\u30f3\u69cb\u6210",
+        "globalPluginConfig": "\u30b0\u30ed\u30fc\u30d0\u30eb \u30d7\u30e9\u30b0\u30a4\u30f3\u69cb\u6210",
         "information": "\u60c5\u5831",
-        "libraryPluginConfig": "\u30e9\u30a4\u30d6\u30e9\u30ea\u30d7\u30e9\u30b0\u30a4\u30f3\u306e\u69cb\u6210",
+        "libraryPluginConfig": "\u30e9\u30a4\u30d6\u30e9\u30ea \u30d7\u30e9\u30b0\u30a4\u30f3\u306e\u69cb\u6210",
         "librarySettings": "\u30e9\u30a4\u30d6\u30e9\u30ea\u8a2d\u5b9a",
-        "listEmpty": "\u3053\u306e\u30bf\u30b9\u30af\u30ea\u30b9\u30c8\u306f\u7a7a\u3067\u3059",
+        "listEmpty": "\u3053\u306e\u30bf\u30b9\u30af \u30ea\u30b9\u30c8\u306f\u7a7a\u3067\u3059",
         "login": "\u30ed\u30b0\u30a4\u30f3",
         "pendingTasks": "\u4fdd\u7559\u4e2d\u306e\u30bf\u30b9\u30af",
         "pluginInfo": "\u30d7\u30e9\u30b0\u30a4\u30f3\u60c5\u5831",
         "pluginInstaller": "\u30d7\u30e9\u30b0\u30a4\u30f3\u30a4\u30f3\u30b9\u30c8\u30fc\u30e9\u30fc",
         "pluginSettings": "\u30d7\u30e9\u30b0\u30a4\u30f3\u8a2d\u5b9a",
         "privacyPolicy": "\u30d7\u30e9\u30a4\u30d0\u30b7\u30fc\u30dd\u30ea\u30b7\u30fc",
         "releaseNotes": "\u30ea\u30ea\u30fc\u30b9\u30ce\u30fc\u30c8",
-        "selectDirectory": "\u30c7\u30a3\u30ec\u30af\u30c8\u30ea\u3092\u9078\u629e\u3057\u307e\u3059",
-        "selectLibrary": "\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u9078\u629e\u3057\u307e\u3059",
-        "selectPlugin": "\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u9078\u629e\u3057\u307e\u3059",
-        "supportFutureDevelopment": "\u5c06\u6765\u306e\u958b\u767a\u3092\u30b5\u30dd\u30fc\u30c8\u3059\u308b",
+        "selectDirectory": "\u30c7\u30a3\u30ec\u30af\u30c8\u30ea\u3092\u9078\u629e",
+        "selectLibrary": "\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u9078\u629e",
+        "selectPlugin": "\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u9078\u629e",
+        "supportFutureDevelopment": "\u5c06\u6765\u306e\u767a\u5c55\u3092\u30b5\u30dd\u30fc\u30c8",
         "workers": "\u52b4\u50cd\u8005"
     },
     "navigation": {
         "account": "\u30a2\u30ab\u30a6\u30f3\u30c8",
         "back": "\u623b\u308b",
         "backToDashboard": "\u30c0\u30c3\u30b7\u30e5\u30dc\u30fc\u30c9\u306b\u623b\u308b",
         "cancel": "\u30ad\u30e3\u30f3\u30bb\u30eb",
         "close": "\u8fd1\u3044",
-        "config": "\u69cb\u6210",
+        "config": "\u8a2d\u5b9a",
         "copy": "\u30b3\u30d4\u30fc",
         "dashboard": "\u30c0\u30c3\u30b7\u30e5\u30dc\u30fc\u30c9",
         "dataPanels": "\u30c7\u30fc\u30bf\u30d1\u30cd\u30eb",
         "documentation": "\u30c9\u30ad\u30e5\u30e1\u30f3\u30c6\u30fc\u30b7\u30e7\u30f3",
         "helpAndSupport": "\u30d8\u30eb\u30d7\u30b5\u30dd\u30fc\u30c8",
         "info": "\u60c5\u5831",
         "library": "\u3068\u3057\u3087\u3046\u304b\u3093",
         "link": "\u30ea\u30f3\u30af",
         "login": "\u30ed\u30b0\u30a4\u30f3",
         "loginWithDiscord": "Discord\u3067\u30ed\u30b0\u30a4\u30f3",
-        "loginWithGitHub": "GitHub\u3067\u30ed\u30b0\u30a4\u30f3",
-        "loginWithPatreon": "Patreon\u3067\u30ed\u30b0\u30a4\u30f3",
+        "loginWithGitHub": "GitHub \u3067\u30ed\u30b0\u30a4\u30f3",
+        "loginWithPatreon": "\u30d1\u30c8\u30ec\u30aa\u30f3\u3067\u30ed\u30b0\u30a4\u30f3",
         "logout": "\u30ed\u30b0\u30a2\u30a6\u30c8",
         "options": "\u30aa\u30d7\u30b7\u30e7\u30f3",
         "plugins": "\u30d7\u30e9\u30b0\u30a4\u30f3",
         "save": "\u4fdd\u5b58",
         "search": "\u63a2\u3059",
         "settings": "\u8a2d\u5b9a",
         "show": "\u898b\u305b\u308b",
@@ -274,55 +279,58 @@
         "submit": "\u9001\u4fe1",
         "workers": "\u52b4\u50cd\u8005",
         "yes": "\u306f\u3044"
     },
     "notifications": {
         "SavedPluginSettings": "\u30d7\u30e9\u30b0\u30a4\u30f3\u8a2d\u5b9a\u304c\u4fdd\u5b58\u3055\u308c\u307e\u3057\u305f\u3002",
         "allowPopups": "\u3053\u306e\u30a6\u30a7\u30d6\u30b5\u30a4\u30c8\u306e\u30dd\u30c3\u30d7\u30a2\u30c3\u30d7\u3092\u8a31\u53ef\u3057\u3066\u304f\u3060\u3055\u3044\u3002",
-        "backendConnectionWarning": "Unmanic\u30d0\u30c3\u30af\u30a8\u30f3\u30c9\u306b\u63a5\u7d9a\u3067\u304d\u307e\u305b\u3093\u3002\u52d5\u4f5c\u3057\u3066\u3044\u308b\u3053\u3068\u3092\u78ba\u8a8d\u3057\u3066\u304f\u3060\u3055\u3044\u3002",
+        "backendConnectionWarning": "Unmanic \u30d0\u30c3\u30af\u30a8\u30f3\u30c9\u306b\u63a5\u7d9a\u3067\u304d\u307e\u305b\u3093\u3002\u5b9f\u884c\u3055\u308c\u3066\u3044\u308b\u3053\u3068\u3092\u78ba\u8a8d\u3057\u3066\u304f\u3060\u3055\u3044\u3002",
         "cannotRemoveDefaultLibrary": "\u30c7\u30d5\u30a9\u30eb\u30c8\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u524a\u9664\u3067\u304d\u307e\u305b\u3093",
-        "copied": "\u30b3\u30d4\u30fc",
-        "failedToFetchEnabledDataPanelPlugins": "\u6709\u52b9\u306a\u30c7\u30fc\u30bf\u30d1\u30cd\u30eb\u30d7\u30e9\u30b0\u30a4\u30f3\u30ea\u30b9\u30c8\u306e\u53d6\u5f97\u306b\u5931\u6557\u3057\u307e\u3057\u305f",
-        "failedToFetchLibraryList": "Unmanic\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u30ea\u30b9\u30c8\u3092\u53d6\u5f97\u3067\u304d\u307e\u305b\u3093\u3067\u3057\u305f\u3002",
-        "failedToFetchLoginUrl": "\u30ed\u30b0\u30a4\u30f3URL\u306e\u53d6\u5f97\u306b\u5931\u6557\u3057\u307e\u3057\u305f\u3002",
-        "failedToFetchLogoutUrl": "\u30ed\u30b0\u30a2\u30a6\u30c8URL\u306e\u53d6\u5f97\u306b\u5931\u6557\u3057\u307e\u3057\u305f\u3002",
-        "failedToFetchSettings": "Unmanic\u306e\u73fe\u5728\u306e\u8a2d\u5b9a\u3092\u53d6\u5f97\u3067\u304d\u307e\u305b\u3093\u3067\u3057\u305f\u3002",
-        "failedToFetchSystemConfig": "Unmanic\u306e\u30b7\u30b9\u30c6\u30e0\u69cb\u6210\u3092\u30d5\u30a7\u30c3\u30c1\u3067\u304d\u307e\u305b\u3093\u3067\u3057\u305f\u3002",
-        "failedToInstallPlugin": "\u8981\u6c42\u3055\u308c\u305f\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3057\u3088\u3046\u3068\u3057\u305f\u3068\u304d\u306b\u30a8\u30e9\u30fc\u304c\u767a\u751f\u3057\u307e\u3057\u305f\u3002",
+        "copied": "\u30b3\u30d4\u30fc\u3057\u307e\u3057\u305f",
+        "failedToFetchEnabledDataPanelPlugins": "\u6709\u52b9\u306a\u30c7\u30fc\u30bf \u30d1\u30cd\u30eb \u30d7\u30e9\u30b0\u30a4\u30f3 \u30ea\u30b9\u30c8\u3092\u53d6\u5f97\u3067\u304d\u307e\u305b\u3093\u3067\u3057\u305f",
+        "failedToFetchLibraryList": "Unmanic \u306e\u30e9\u30a4\u30d6\u30e9\u30ea \u30ea\u30b9\u30c8\u306e\u53d6\u5f97\u306b\u5931\u6557\u3057\u307e\u3057\u305f\u3002",
+        "failedToFetchLoginUrl": "\u30ed\u30b0\u30a4\u30f3 URL \u306e\u53d6\u5f97\u306b\u5931\u6557\u3057\u307e\u3057\u305f\u3002",
+        "failedToFetchLogoutUrl": "\u30ed\u30b0\u30a2\u30a6\u30c8 URL \u306e\u53d6\u5f97\u306b\u5931\u6557\u3057\u307e\u3057\u305f\u3002",
+        "failedToFetchSettings": "Unmanic \u306e\u73fe\u5728\u306e\u8a2d\u5b9a\u3092\u53d6\u5f97\u3067\u304d\u307e\u305b\u3093\u3067\u3057\u305f\u3002",
+        "failedToFetchSystemConfig": "Unmanic \u306e\u30b7\u30b9\u30c6\u30e0\u69cb\u6210\u3092\u53d6\u5f97\u3067\u304d\u307e\u305b\u3093\u3067\u3057\u305f\u3002",
+        "failedToInstallPlugin": "\u8981\u6c42\u3055\u308c\u305f\u30d7\u30e9\u30b0\u30a4\u30f3\u306e\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u4e2d\u306b\u30a8\u30e9\u30fc\u304c\u767a\u751f\u3057\u307e\u3057\u305f\u3002",
         "failedToSavePluginSettings": "\u30d7\u30e9\u30b0\u30a4\u30f3\u8a2d\u5b9a\u306e\u4fdd\u5b58\u306b\u5931\u6557\u3057\u307e\u3057\u305f\u3002",
-        "failedToSaveSettings": "\u8a2d\u5b9a\u306e\u4fdd\u5b58\u306b\u5931\u6557\u3057\u307e\u3057\u305f\u3002",
-        "incompatibleRemoteInstallation": "\u8ffd\u52a0\u3057\u3088\u3046\u3068\u3057\u3066\u3044\u308b\u30ea\u30e2\u30fc\u30c8\u306eUnmanic\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u306f\u3001\u30ea\u30f3\u30af\u3068\u4e92\u63db\u6027\u304c\u3042\u308a\u307e\u305b\u3093\u3002\u6700\u521d\u306b\u66f4\u65b0\u3057\u3066\u307f\u3066\u304f\u3060\u3055\u3044\u3002",
-        "installed": "\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3055\u308c\u3066\u3044\u307e\u3059\u3002",
-        "invalidRemoteInstallationAddress": "\u5165\u529b\u3057\u305f\u30a2\u30c9\u30ec\u30b9\u306f\u3001\u6709\u52b9\u306aUnmanic\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3067\u306f\u3042\u308a\u307e\u305b\u3093\u3067\u3057\u305f\u3002",
-        "invalidWorkerEvent": "\u7121\u52b9\u306a\u30ef\u30fc\u30ab\u30fc\u30a4\u30d9\u30f3\u30c8\u3092\u8ffd\u52a0\u3067\u304d\u307e\u305b\u3093\u3002",
+        "failedToSaveSettings": "\u8a2d\u5b9a\u3092\u4fdd\u5b58\u3067\u304d\u307e\u305b\u3093\u3067\u3057\u305f\u3002",
+        "incompatibleRemoteInstallation": "\u8ffd\u52a0\u3057\u3088\u3046\u3068\u3057\u3066\u3044\u308b\u30ea\u30e2\u30fc\u30c8\u306e Unmanic \u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u306f\u3001\u30ea\u30f3\u30af\u306b\u5bfe\u5fdc\u3057\u3066\u3044\u307e\u305b\u3093\u3002\u307e\u305a\u306f\u66f4\u65b0\u3057\u3066\u307f\u3066\u304f\u3060\u3055\u3044\u3002",
+        "installed": "\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u6e08\u307f\u3002",
+        "invalidRemoteInstallationAddress": "\u5165\u529b\u3057\u305f\u30a2\u30c9\u30ec\u30b9\u306f\u3001\u6709\u52b9\u306a Unmanic \u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3067\u306f\u3042\u308a\u307e\u305b\u3093\u3067\u3057\u305f\u3002",
+        "invalidWorkerEvent": "\u7121\u52b9\u306a\u30ef\u30fc\u30ab\u30fc \u30a4\u30d9\u30f3\u30c8\u3092\u8ffd\u52a0\u3067\u304d\u307e\u305b\u3093\u3002",
         "newRepoAddFailed": "\u65b0\u3057\u3044\u30ea\u30dd\u30b8\u30c8\u30ea\u3092\u4fdd\u5b58\u3067\u304d\u307e\u305b\u3093\u3067\u3057\u305f\u3002",
-        "remoteInstallationAlreadyInList": "\u5165\u529b\u3057\u305f\u30a2\u30c9\u30ec\u30b9\u306f\u3001\u30ea\u30e2\u30fc\u30c8\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u306e\u30ea\u30b9\u30c8\u306b\u3059\u3067\u306b\u542b\u307e\u308c\u3066\u3044\u307e\u3059\u3002",
-        "repoAlreadyExists": "\u30ea\u30dd\u30b8\u30c8\u30ea\u306f\u3059\u3067\u306b\u5b58\u5728\u3057\u307e\u3059\u3002",
-        "repoRemovedFailed": "\u30ea\u30dd\u30b8\u30c8\u30ea\u3092\u524a\u9664\u3057\u3088\u3046\u3068\u3057\u305f\u3068\u304d\u306b\u554f\u984c\u304c\u767a\u751f\u3057\u307e\u3057\u305f\u3002",
+        "remoteInstallationAlreadyInList": "\u5165\u529b\u3057\u305f\u30a2\u30c9\u30ec\u30b9\u306f\u3001\u65e2\u306b\u30ea\u30e2\u30fc\u30c8 \u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u306e\u30ea\u30b9\u30c8\u306b\u542b\u307e\u308c\u3066\u3044\u307e\u3059\u3002",
+        "repoAlreadyExists": "\u30ea\u30dd\u30b8\u30c8\u30ea\u306f\u65e2\u306b\u5b58\u5728\u3057\u307e\u3059\u3002",
+        "repoRemovedFailed": "\u30ea\u30dd\u30b8\u30c8\u30ea\u306e\u524a\u9664\u4e2d\u306b\u554f\u984c\u304c\u767a\u751f\u3057\u307e\u3057\u305f\u3002",
         "repoRemovedSuccess": "\u30ea\u30dd\u30b8\u30c8\u30ea\u304c\u6b63\u5e38\u306b\u524a\u9664\u3055\u308c\u307e\u3057\u305f\u3002",
-        "reposRefreshFailure": "\u69cb\u6210\u3055\u308c\u305f\u30ea\u30dd\u30b8\u30c8\u30ea\u30fc\u3092\u66f4\u65b0\u3067\u304d\u307e\u305b\u3093\u3002\u304a\u305d\u3089\u304f\u3001URL\u306e1\u3064\u306b\u30a8\u30e9\u30fc\u304c\u3042\u308a\u307e\u3059\u304b\uff1f",
-        "reposRefreshSuccess": "\u3059\u3079\u3066\u306e\u30ea\u30dd\u30b8\u30c8\u30ea\u3092\u6b63\u5e38\u306b\u66f4\u65b0\u3057\u307e\u3057\u305f\u3002",
-        "rescanLibraryError": "\u30e9\u30a4\u30d6\u30e9\u30ea\u306e\u518d\u30b9\u30ad\u30e3\u30f3\u3092\u8981\u6c42\u3057\u3066\u3044\u308b\u3068\u304d\u306b\u30a8\u30e9\u30fc\u304c\u767a\u751f\u3057\u307e\u3057\u305f",
+        "reposRefreshFailure": "\u69cb\u6210\u6e08\u307f\u306e\u30ea\u30dd\u30b8\u30c8\u30ea\u3092\u66f4\u65b0\u3067\u304d\u307e\u305b\u3093\u3002\u304a\u305d\u3089\u304f\u3001\u3044\u305a\u308c\u304b\u306e URL \u306b\u30a8\u30e9\u30fc\u304c\u3042\u308a\u307e\u3059\u304b?",
+        "reposRefreshSuccess": "\u3059\u3079\u3066\u306e\u30ea\u30dd\u30b8\u30c8\u30ea\u304c\u6b63\u5e38\u306b\u66f4\u65b0\u3055\u308c\u307e\u3057\u305f\u3002",
+        "rescanLibraryError": "\u30e9\u30a4\u30d6\u30e9\u30ea\u306e\u518d\u30b9\u30ad\u30e3\u30f3\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u4e2d\u306b\u30a8\u30e9\u30fc\u304c\u767a\u751f\u3057\u307e\u3057\u305f",
         "saved": "\u4fdd\u5b58\u3057\u307e\u3057\u305f\u3002",
         "serverMessages": {
             "defaults": {
                 "error": "\u30b5\u30fc\u30d0\u30fc\u3067\u4e0d\u660e\u306a\u30a8\u30e9\u30fc\u304c\u767a\u751f\u3057\u307e\u3057\u305f",
                 "info": "\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u306e\u4e0d\u660e\u306a\u30e1\u30c3\u30bb\u30fc\u30b8",
-                "status": "\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u306e\u4e0d\u660e\u306a\u30b9\u30c6\u30fc\u30bf\u30b9\u306e\u66f4\u65b0",
+                "status": "\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u306e\u4e0d\u660e\u306a\u30b9\u30c6\u30fc\u30bf\u30b9\u66f4\u65b0",
                 "success": "\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u306e\u4e0d\u660e\u306a\u30e1\u30c3\u30bb\u30fc\u30b8",
                 "warning": "\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u306e\u4e0d\u660e\u306a\u8b66\u544a"
             },
-            "incompatiblePlugin": "Unmanic\u306f\u3001\u30e9\u30a4\u30d6\u30e9\u30ea\u306e1\u3064\u3067\u6709\u52b9\u306b\u306a\u3063\u3066\u3044\u308b\u4e92\u63db\u6027\u306e\u306a\u3044\u30d7\u30e9\u30b0\u30a4\u30f3\u3092\u691c\u51fa\u3057\u305f\u305f\u3081\u3001\u30bf\u30b9\u30af\u306e\u51e6\u7406\u3092\u505c\u6b62\u3057\u307e\u3057\u305f",
-            "libraryEnabledLimits": "\u975e\u30b5\u30dd\u30fc\u30bf\u30fc\u5c64\u7528\u306b\u69cb\u6210\u3055\u308c\u305f\u30e9\u30a4\u30d6\u30e9\u30ea\u30fc\u304c\u591a\u3059\u304e\u308b\u305f\u3081\u3001Unmanic\u306f\u30bf\u30b9\u30af\u306e\u51e6\u7406\u3092\u505c\u6b62\u3057\u307e\u3057\u305f\u3002 2\u3064\u4ee5\u4e0a\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u6709\u52b9\u306b\u3059\u308b\u305f\u3081\u306b\u30d7\u30ed\u30b8\u30a7\u30af\u30c8\u3092\u5f8c\u63f4\u3059\u308b\u3053\u3068\u3092\u691c\u8a0e\u3057\u3066\u304f\u3060\u3055\u3044\u3002",
-            "libraryScanProgress": "\u30e9\u30a4\u30d6\u30e9\u30ea\u30b9\u30ad\u30e3\u30f3\u306e\u5b9f\u884c",
-            "linkedInstallationLimits": "\u975e\u30b5\u30dd\u30fc\u30bf\u30fc\u5c64\u306b\u30ea\u30f3\u30af\u3057\u3066\u3044\u308b\u30ea\u30e2\u30fc\u30c8\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u304c\u591a\u3059\u304e\u308b\u305f\u3081\u3001Unmanic\u306f\u30bf\u30b9\u30af\u306e\u51e6\u7406\u3092\u505c\u6b62\u3057\u307e\u3057\u305f\u3002\u8907\u6570\u306e\u30ea\u30e2\u30fc\u30c8\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3092\u30ea\u30f3\u30af\u3059\u308b\u30d7\u30ed\u30b8\u30a7\u30af\u30c8\u3092\u5f8c\u63f4\u3059\u308b\u3053\u3068\u3092\u691c\u8a0e\u3057\u3066\u304f\u3060\u3055\u3044\u3002",
-            "pendingTaskHaltedPostProcessorQueueFull": "\u30dd\u30b9\u30c8\u30d7\u30ed\u30bb\u30c3\u30b5\u30ad\u30e5\u30fc\u304c\u5236\u9650\u306b\u9054\u3057\u307e\u3057\u305f",
-            "pendingTaskHaltedPostProcessorQueueFullMessage": "\u30dd\u30b9\u30c8\u30d7\u30ed\u30bb\u30c3\u30b5\u30ad\u30e5\u30fc\u304c\u73fe\u5728\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308b\u30ef\u30fc\u30ab\u30fc\u6570\u3092\u4e0b\u56de\u308b\u307e\u3067\u3001\u30ef\u30fc\u30ab\u30fc\u306f\u65b0\u3057\u3044\u4fdd\u7559\u4e2d\u306e\u30bf\u30b9\u30af\u3092\u53d7\u3051\u53d6\u308a\u307e\u305b\u3093\u3002",
-            "pluginSettingsChangeWorkersStopped": "Unmanic\u306f\u3001\u30d7\u30e9\u30b0\u30a4\u30f3\u69cb\u6210\u306e\u5909\u66f4\u3092\u691c\u51fa\u3057\u305f\u305f\u3081\u3001\u3059\u3079\u3066\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u505c\u6b62\u3057\u307e\u3057\u305f\u3002\u6e96\u5099\u304c\u3067\u304d\u305f\u3089\u3001\u30c0\u30c3\u30b7\u30e5\u30dc\u30fc\u30c9\u304b\u3089\u30ef\u30fc\u30ab\u30fc\u3092\u518d\u958b\u3057\u307e\u3059\u3002",
+            "incompatiblePlugin": "Unmanic \u306f\u3001\u30e9\u30a4\u30d6\u30e9\u30ea\u306e 1 \u3064\u3067\u4e92\u63db\u6027\u306e\u306a\u3044\u30d7\u30e9\u30b0\u30a4\u30f3\u304c\u6709\u52b9\u306b\u306a\u3063\u3066\u3044\u308b\u3053\u3068\u3092\u691c\u51fa\u3057\u305f\u305f\u3081\u3001\u30bf\u30b9\u30af\u306e\u51e6\u7406\u3092\u505c\u6b62\u3057\u307e\u3057\u305f",
+            "libraryEnabledLimits": "\u975e\u30b5\u30dd\u30fc\u30bf\u30fc\u968e\u5c64\u7528\u306b\u69cb\u6210\u3055\u308c\u305f\u30e9\u30a4\u30d6\u30e9\u30ea\u304c\u591a\u3059\u304e\u308b\u305f\u3081\u3001Unmanic \u306f\u30bf\u30b9\u30af\u306e\u51e6\u7406\u3092\u505c\u6b62\u3057\u307e\u3057\u305f\u3002\u30d7\u30ed\u30b8\u30a7\u30af\u30c8\u306e\u30b9\u30dd\u30f3\u30b5\u30fc\u306b\u306a\u3063\u3066\u30012 \u3064\u4ee5\u4e0a\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u3092\u6709\u52b9\u306b\u3059\u308b\u3053\u3068\u3092\u691c\u8a0e\u3057\u3066\u304f\u3060\u3055\u3044\u3002",
+            "libraryScanProgress": "\u30e9\u30a4\u30d6\u30e9\u30ea\u30b9\u30ad\u30e3\u30f3\u5b9f\u884c\u4e2d",
+            "linkedInstallationLimits": "\u975e\u30b5\u30dd\u30fc\u30bf\u30fc\u5c64\u306e\u30ea\u30e2\u30fc\u30c8 \u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3092\u30ea\u30f3\u30af\u3057\u3059\u304e\u305f\u305f\u3081\u3001Unmanic \u306f\u30bf\u30b9\u30af\u306e\u51e6\u7406\u3092\u505c\u6b62\u3057\u307e\u3057\u305f\u3002\u30d7\u30ed\u30b8\u30a7\u30af\u30c8\u306e\u30b9\u30dd\u30f3\u30b5\u30fc\u306b\u306a\u3063\u3066\u3001\u8907\u6570\u306e\u30ea\u30e2\u30fc\u30c8 \u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3092\u30ea\u30f3\u30af\u3059\u308b\u3053\u3068\u3092\u691c\u8a0e\u3057\u3066\u304f\u3060\u3055\u3044\u3002",
+            "pendingTaskHaltedPostProcessorQueueFull": "\u30dd\u30b9\u30c8\u30d7\u30ed\u30bb\u30c3\u30b5 \u30ad\u30e5\u30fc\u304c\u9650\u754c\u306b\u9054\u3057\u307e\u3057\u305f",
+            "pendingTaskHaltedPostProcessorQueueFullMessage": "\u30dd\u30b9\u30c8\u30d7\u30ed\u30bb\u30c3\u30b5\u30fc\u306e\u30ad\u30e5\u30fc\u304c\u73fe\u5728\u69cb\u6210\u3055\u308c\u3066\u3044\u308b\u30ef\u30fc\u30ab\u30fc\u6570\u3092\u4e0b\u56de\u308b\u307e\u3067\u3001\u30ef\u30fc\u30ab\u30fc\u306f\u65b0\u3057\u3044\u4fdd\u7559\u4e2d\u306e\u30bf\u30b9\u30af\u3092\u53d7\u3051\u53d6\u308a\u307e\u305b\u3093",
+            "pluginSettingsChangeWorkersStopped": "Unmanic \u306f\u3001\u30d7\u30e9\u30b0\u30a4\u30f3\u69cb\u6210\u306e\u5909\u66f4\u3092\u691c\u51fa\u3057\u305f\u305f\u3081\u3001\u3059\u3079\u3066\u306e\u30ef\u30fc\u30ab\u30fc\u3092\u505c\u6b62\u3057\u307e\u3057\u305f\u3002\u6e96\u5099\u304c\u3067\u304d\u305f\u3089\u3001\u30c0\u30c3\u30b7\u30e5\u30dc\u30fc\u30c9\u304b\u3089\u30ef\u30fc\u30ab\u30fc\u3092\u518d\u958b\u3057\u307e\u3059\u3002",
             "receivingRemoteFile": "\u30ea\u30e2\u30fc\u30c8\u30d5\u30a1\u30a4\u30eb\u306e\u53d7\u4fe1"
+        },
+        "serverNotificationLabels": {
+            "failedTaskLabel": "\u30bf\u30b9\u30af\u306e\u5931\u6557"
         }
     },
     "status": {
         "all": "\u5168\u3066",
         "cannotLoadImage": "\u753b\u50cf\u3092\u8aad\u307f\u8fbc\u3081\u307e\u305b\u3093",
         "disabled": "\u7121\u52b9",
         "enabled": "\u6709\u52b9",
@@ -332,22 +340,22 @@
     },
     "tooltips": {
         "add": "\u8ffd\u52a0",
         "available": "\u5229\u7528\u53ef\u80fd",
         "back": "\u623b\u308b",
         "close": "\u8fd1\u3044",
         "configure": "\u69cb\u6210\u3001\u8a2d\u5b9a",
-        "configureForThisLibrary": "\u3053\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u7528\u306b\u69cb\u6210\u3059\u308b",
-        "defaultLibrary": "\u3053\u308c\u306f\u30c7\u30d5\u30a9\u30eb\u30c8\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u3067\u3059\u3002\u524a\u9664\u3067\u304d\u307e\u305b\u3093\u3002",
+        "configureForThisLibrary": "\u3053\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u306e\u69cb\u6210",
+        "defaultLibrary": "\u3053\u308c\u304c\u30c7\u30d5\u30a9\u30eb\u30c8\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u3067\u3059\u3002\u524a\u9664\u3067\u304d\u307e\u305b\u3093\u3002",
         "delete": "\u6d88\u53bb",
-        "etc": "\u5b8c\u4e86\u4e88\u5b9a\u6642\u9593",
+        "etc": "\u5b8c\u6210\u4e88\u60f3\u6642\u9593",
         "install": "\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb",
         "move": "\u52d5\u304f",
         "pluginInfo": "\u30d7\u30e9\u30b0\u30a4\u30f3\u60c5\u5831",
         "position": "\u4f4d\u7f6e",
         "reinstall": "\u518d\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb",
         "remove": "\u524a\u9664\u3059\u308b",
-        "removeFromThisLibrary": "\u3053\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u304b\u3089\u524a\u9664\u3059\u308b",
-        "unavailable": "\u5229\u7528\u3067\u304d\u307e\u305b\u3093",
+        "removeFromThisLibrary": "\u3053\u306e\u30e9\u30a4\u30d6\u30e9\u30ea\u304b\u3089\u524a\u9664",
+        "unavailable": "\u5229\u7528\u4e0d\u53ef",
         "update": "\u30a2\u30c3\u30d7\u30c7\u30fc\u30c8"
     }
 }
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/language/de.json` & `unmanic-0.2.4/unmanic/webserver/frontend/src/language/de.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9724287684940395%*

 * *Differences: {"'buttons'": "{'dismissAll': 'Alle ablehnen'}",*

 * * "'components'": "{'settings': {'library': {'exportLibraryConfig': 'Konfig exportieren'}}, "*

 * *                 "'plugins': {'installPluginFromRepo': 'Installieren Sie das Plugin aus dem Repo', "*

 * *                 "'installPluginFromFile': 'Plugin aus Datei installieren', 'invalidZipFile': "*

 * *                 "'Datei ist keine gültige ZIP-Datei', 'failedToInstallPluginFromZip': 'Plug-in "*

 * *                 "konnte nicht aus der hochgeladenen ZIP-Datei installiert  […]*

```diff
@@ -1,10 +1,11 @@
 {
     "buttons": {
         "darkMode": "Dunkler Modus",
+        "dismissAll": "Alle ablehnen",
         "language": "Sprache"
     },
     "components": {
         "completedTasks": {
             "addToPendingTasksList": "Ausgew\u00e4hlte zur Liste der ausstehenden Aufgaben hinzuf\u00fcgen",
             "before": "Vor",
             "details": "Einzelheiten",
@@ -27,16 +28,20 @@
         },
         "plugins": {
             "addRepository": "Repository hinzuf\u00fcgen",
             "author": "Autor",
             "categoryFilter": "Kategoriefilter",
             "clickToUpdatePlugin": "Klicken Sie hier, um das Plugin zu aktualisieren",
             "errorSavingFlow": "Beim Speichern des Plugin-Flows ist ein Fehler aufgetreten",
+            "failedToInstallPluginFromZip": "Plug-in konnte nicht aus der hochgeladenen ZIP-Datei installiert werden",
             "globalConfiguration": "Globale Konfiguration",
-            "installPlugins": "PIugin installieren",
+            "installPluginFromFile": "Plugin aus Datei installieren",
+            "installPluginFromRepo": "Installieren Sie das Plugin aus dem Repo",
+            "installedPluginFromZip": "Plugin installiert",
+            "invalidZipFile": "Datei ist keine g\u00fcltige ZIP-Datei",
             "newRepository": "Neues Repository",
             "pluginUpToDate": "Plugin ist aktuell",
             "refreshRepositories": "Repositorys aktualisieren",
             "removePlugin": "Plugin entfernen",
             "repo": "Repository",
             "repoList": "Repository-Liste",
             "repoName": "Name",
@@ -77,15 +82,15 @@
                 "concurrentFileTesters": "Gleichzeitige Dateitester",
                 "confirmRemove": "Durch das Entfernen der Bibliothek werden auch alle dieser Bibliothek zugeordneten Einstellungen entfernt. M\u00f6chten Sie wirklich fortfahren?",
                 "defaultLibrary": "Standardbibliothek",
                 "enableInotify": "Aktivieren Sie die Datei\u00fcberwachung f\u00fcr diese Bibliothek",
                 "enableLibraryScanner": "Aktivieren Sie regelm\u00e4\u00dfige Bibliotheksscans",
                 "enableReceiveRemoteFilesOnly": "Konfigurieren Sie die Bibliothek nur f\u00fcr den Empfang von Remote-Dateien",
                 "enableScanner": "Aktivieren Sie den Bibliotheksscanner f\u00fcr diese Bibliothek",
-                "exportLibraryConfig": "Konfig. exportieren",
+                "exportLibraryConfig": "Konfig exportieren",
                 "fileTesting": "Dateipr\u00fcfung",
                 "followSymlinks": "Folgen Sie symbolischen Links bei Bibliotheksscans",
                 "importLibraryConfig": "Konfig importieren",
                 "importPluginConfigMessage": "Bibliothekskonfiguration importieren. Dies kann einige Zeit dauern, wenn Plugins installiert werden m\u00fcssen.",
                 "libraryFileMonitorStatusLabel": "Dateimonitor",
                 "libraryRemoteOnlyStatus": "Nur Fernbedienung",
                 "libraryScanner": "Bibliotheksscanner",
@@ -314,15 +319,18 @@
             "incompatiblePlugin": "Unmanic hat die Verarbeitung von Aufgaben gestoppt, da es ein inkompatibles Plug-in entdeckt hat, das in einer Ihrer Bibliotheken aktiviert ist",
             "libraryEnabledLimits": "Unmanic hat die Verarbeitung von Aufgaben eingestellt, da Sie zu viele Bibliotheken f\u00fcr eine Nicht-Supporter-Stufe konfiguriert haben. Erw\u00e4gen Sie, das Projekt zu sponsern, um mehr als zwei Bibliotheken zu erm\u00f6glichen.",
             "libraryScanProgress": "Bibliotheksscan l\u00e4uft",
             "linkedInstallationLimits": "Unmanic hat die Verarbeitung von Aufgaben eingestellt, da Sie zu viele Remote-Installationen f\u00fcr eine Nicht-Support-Stufe verkn\u00fcpft haben. Erw\u00e4gen Sie, das Projekt zu sponsern, um mehr als eine Remote-Installation zu verkn\u00fcpfen.",
             "pendingTaskHaltedPostProcessorQueueFull": "Die Postprozessorwarteschlange hat ihr Limit erreicht",
             "pendingTaskHaltedPostProcessorQueueFullMessage": "Worker erhalten keine neue ausstehende Aufgabe, bis die Postprozessor-Warteschlange unter die aktuell konfigurierte Worker-Anzahl f\u00e4llt",
             "pluginSettingsChangeWorkersStopped": "Unmanic hat alle Worker gestoppt, da es eine \u00c4nderung an der Plugin-Konfiguration festgestellt hat. Wenn Sie bereit sind, setzen Sie die Worker \u00fcber das Dashboard fort.",
-            "receivingRemoteFile": "Remote-Datei wird empfangen"
+            "receivingRemoteFile": "Entfernte Datei wird empfangen"
+        },
+        "serverNotificationLabels": {
+            "failedTaskLabel": "Aufgabenfehler"
         }
     },
     "status": {
         "all": "Alle",
         "cannotLoadImage": "Bild kann nicht geladen werden",
         "disabled": "Deaktiviert",
         "enabled": "Erm\u00f6glicht",
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/language/pt-br.json` & `unmanic-0.2.4/unmanic/webserver/frontend/src/language/pt-br.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9712692792634294%*

 * *Differences: {"'buttons'": "{'dismissAll': 'Recusar tudo'}",*

 * * "'components'": "{'plugins': {'types': {'postprocessor': {'fileMoveCaption': 'Esses plugins são "*

 * *                 'chamados na conclusão da tarefa para adicionar movimentos de arquivo '*

 * *                 "adicionais'}}, 'installPluginFromRepo': 'Instalar plug-in do repositório', "*

 * *                 "'installPluginFromFile': 'Instalar plug-in do arquivo', 'invalidZipFile': 'O "*

 * *                 "arquivo não é um arquivo ZIP válido', 'failedToInstallPluginFromZi […]*

```diff
@@ -1,10 +1,11 @@
 {
     "buttons": {
         "darkMode": "Modo escuro",
+        "dismissAll": "Recusar tudo",
         "language": "Linguagem"
     },
     "components": {
         "completedTasks": {
             "addToPendingTasksList": "Adicionar selecionado \u00e0 lista de tarefas pendentes",
             "before": "Antes da",
             "details": "Detalhes",
@@ -27,16 +28,20 @@
         },
         "plugins": {
             "addRepository": "Adicionar reposit\u00f3rio",
             "author": "Autor",
             "categoryFilter": "Filtro de categoria",
             "clickToUpdatePlugin": "Clique para atualizar o plug-in",
             "errorSavingFlow": "Foi encontrado um erro ao salvar o fluxo de plug-in",
+            "failedToInstallPluginFromZip": "Falha ao instalar o plug-in do arquivo ZIP carregado",
             "globalConfiguration": "Configura\u00e7\u00e3o global",
-            "installPlugins": "Instalar plugin",
+            "installPluginFromFile": "Instalar plug-in do arquivo",
+            "installPluginFromRepo": "Instalar plug-in do reposit\u00f3rio",
+            "installedPluginFromZip": "Plugin instalado",
+            "invalidZipFile": "O arquivo n\u00e3o \u00e9 um arquivo ZIP v\u00e1lido",
             "newRepository": "Novo reposit\u00f3rio",
             "pluginUpToDate": "O plug-in est\u00e1 atualizado",
             "refreshRepositories": "Atualizar reposit\u00f3rios",
             "removePlugin": "Remover plug-in",
             "repo": "Reposit\u00f3rio",
             "repoList": "Lista de reposit\u00f3rios",
             "repoName": "Nome",
@@ -45,15 +50,15 @@
             "types": {
                 "libraryManagement": {
                     "fileTest": "Gerenciamento de Biblioteca - Teste de arquivo",
                     "fileTestCaption": "Estes plugins s\u00e3o chamados para testar se os arquivos devem ser adicionados \u00e0 lista de tarefas pendentes"
                 },
                 "postprocessor": {
                     "fileMove": "P\u00f3s-processador - Movimentos de arquivos",
-                    "fileMoveCaption": "Esses plugins s\u00e3o chamados na conclus\u00e3o da tarefa para adicionar movimentos de arquivos adicionais",
+                    "fileMoveCaption": "Esses plugins s\u00e3o chamados na conclus\u00e3o da tarefa para adicionar movimentos de arquivo adicionais",
                     "taskResult": "P\u00f3s-processador - Marcando o sucesso/falha da tarefa",
                     "taskResultCaption": "Esses plugins s\u00e3o chamados na conclus\u00e3o de uma tarefa para marcar o sucesso ou falha geral dessa tarefa"
                 },
                 "worker": {
                     "processItem": "Trabalhador - Processando arquivo",
                     "processItemCaption": "Esses plugins s\u00e3o chamados por um trabalhador e produzem um comando personalizado para ser executado e gerenciado por esse trabalhador"
                 }
@@ -297,15 +302,15 @@
         "newRepoAddFailed": "Falha ao salvar o novo reposit\u00f3rio.",
         "remoteInstallationAlreadyInList": "O endere\u00e7o que voc\u00ea digitou j\u00e1 est\u00e1 na lista de instala\u00e7\u00f5es remotas.",
         "repoAlreadyExists": "O reposit\u00f3rio j\u00e1 existe.",
         "repoRemovedFailed": "Algo deu errado ao tentar remover o reposit\u00f3rio.",
         "repoRemovedSuccess": "Reposit\u00f3rio removido com sucesso.",
         "reposRefreshFailure": "N\u00e3o foi poss\u00edvel atualizar seus reposit\u00f3rios configurados. Talvez haja um erro em uma das URLs?",
         "reposRefreshSuccess": "Todos os reposit\u00f3rios atualizados com sucesso.",
-        "rescanLibraryError": "Foi encontrado um erro ao solicitar uma nova verifica\u00e7\u00e3o de biblioteca",
+        "rescanLibraryError": "Foi encontrado um erro ao solicitar uma nova verifica\u00e7\u00e3o da biblioteca",
         "saved": "Salvou.",
         "serverMessages": {
             "defaults": {
                 "error": "Ocorreu um erro desconhecido no servidor",
                 "info": "Mensagem desconhecida do servidor",
                 "status": "Atualiza\u00e7\u00e3o de status desconhecida do servidor",
                 "success": "Mensagem desconhecida do servidor",
@@ -315,14 +320,17 @@
             "libraryEnabledLimits": "Unmanic parou de processar tarefas porque voc\u00ea tem muitas bibliotecas configuradas para uma camada sem suporte. Considere patrocinar o projeto para habilitar mais de 2 bibliotecas.",
             "libraryScanProgress": "Verifica\u00e7\u00e3o da biblioteca em execu\u00e7\u00e3o",
             "linkedInstallationLimits": "O Unmanic parou de processar tarefas porque voc\u00ea vinculou muitas instala\u00e7\u00f5es remotas para uma camada sem suporte. Considere patrocinar o projeto para vincular mais de uma instala\u00e7\u00e3o remota.",
             "pendingTaskHaltedPostProcessorQueueFull": "A fila do p\u00f3s-processador atingiu seu limite",
             "pendingTaskHaltedPostProcessorQueueFullMessage": "Os trabalhadores n\u00e3o receber\u00e3o uma nova tarefa pendente at\u00e9 que a fila do p\u00f3s-processador caia abaixo da contagem de trabalhadores configurada atual",
             "pluginSettingsChangeWorkersStopped": "O Unmanic parou todos os trabalhadores, pois detectou uma altera\u00e7\u00e3o na configura\u00e7\u00e3o dos plugins. Quando estiver pronto, retome os trabalhadores do painel.",
             "receivingRemoteFile": "Recebendo arquivo remoto"
+        },
+        "serverNotificationLabels": {
+            "failedTaskLabel": "Falha na tarefa"
         }
     },
     "status": {
         "all": "Tudo",
         "cannotLoadImage": "N\u00e3o \u00e9 poss\u00edvel carregar a imagem",
         "disabled": "Desabilitado",
         "enabled": "Habilitado",
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/language/zh.json` & `unmanic-0.2.4/unmanic/webserver/frontend/src/language/zh.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9725029322073656%*

 * *Differences: {"'buttons'": "{'dismissAll': '关闭所有'}",*

 * * "'components'": "{'plugins': {'installPluginFromRepo': '从回购安装插件', 'installPluginFromFile': "*

 * *                 "'从文件安装插件', 'invalidZipFile': '文件不是有效的 ZIP 文件', 'failedToInstallPluginFromZip': "*

 * *                 "'从上传的 ZIP 文件安装插件失败', 'installedPluginFromZip': '已安装插件', delete: "*

 * *                 "['installPlugins']}}",*

 * * "'notifications'": "{'serverNotificationLabels': OrderedDict([('failedTaskLabel', '任务失败')])}"}*

```diff
@@ -1,10 +1,11 @@
 {
     "buttons": {
         "darkMode": "\u9ed1\u6697\u6a21\u5f0f",
+        "dismissAll": "\u5173\u95ed\u6240\u6709",
         "language": "\u8bed"
     },
     "components": {
         "completedTasks": {
             "addToPendingTasksList": "\u5c06\u6240\u9009\u5185\u5bb9\u6dfb\u52a0\u5230\u5f85\u5904\u7406\u4efb\u52a1\u5217\u8868",
             "before": "\u524d",
             "details": "\u7ec6\u8282",
@@ -27,16 +28,20 @@
         },
         "plugins": {
             "addRepository": "\u6dfb\u52a0\u5b58\u50a8\u5e93",
             "author": "\u4f5c\u8005",
             "categoryFilter": "\u7c7b\u522b\u8fc7\u6ee4\u5668",
             "clickToUpdatePlugin": "\u70b9\u51fb\u66f4\u65b0\u63d2\u4ef6",
             "errorSavingFlow": "\u4fdd\u5b58\u63d2\u4ef6\u6d41\u7a0b\u65f6\u9047\u5230\u9519\u8bef",
+            "failedToInstallPluginFromZip": "\u4ece\u4e0a\u4f20\u7684 ZIP \u6587\u4ef6\u5b89\u88c5\u63d2\u4ef6\u5931\u8d25",
             "globalConfiguration": "\u5168\u5c40\u914d\u7f6e",
-            "installPlugins": "\u5b89\u88c5\u63d2\u4ef6",
+            "installPluginFromFile": "\u4ece\u6587\u4ef6\u5b89\u88c5\u63d2\u4ef6",
+            "installPluginFromRepo": "\u4ece\u56de\u8d2d\u5b89\u88c5\u63d2\u4ef6",
+            "installedPluginFromZip": "\u5df2\u5b89\u88c5\u63d2\u4ef6",
+            "invalidZipFile": "\u6587\u4ef6\u4e0d\u662f\u6709\u6548\u7684 ZIP \u6587\u4ef6",
             "newRepository": "\u65b0\u5b58\u50a8\u5e93",
             "pluginUpToDate": "\u63d2\u4ef6\u662f\u6700\u65b0\u7684",
             "refreshRepositories": "\u5237\u65b0\u5b58\u50a8\u5e93",
             "removePlugin": "\u5220\u9664\u63d2\u4ef6",
             "repo": "\u5b58\u50a8\u5e93",
             "repoList": "\u5b58\u50a8\u5e93\u5217\u8868",
             "repoName": "\u59d3\u540d",
@@ -315,14 +320,17 @@
             "libraryEnabledLimits": "Unmanic \u5df2\u505c\u6b62\u5904\u7406\u4efb\u52a1\uff0c\u56e0\u4e3a\u60a8\u4e3a\u975e\u652f\u6301\u8005\u5c42\u914d\u7f6e\u4e86\u592a\u591a\u5e93\u3002\u8003\u8651\u8d5e\u52a9\u8be5\u9879\u76ee\u4ee5\u542f\u7528 2 \u4e2a\u4ee5\u4e0a\u7684\u5e93\u3002",
             "libraryScanProgress": "\u5e93\u626b\u63cf\u8fd0\u884c",
             "linkedInstallationLimits": "Unmanic \u5df2\u505c\u6b62\u5904\u7406\u4efb\u52a1\uff0c\u56e0\u4e3a\u60a8\u4e3a\u975e\u652f\u6301\u8005\u5c42\u94fe\u63a5\u4e86\u592a\u591a\u8fdc\u7a0b\u5b89\u88c5\u3002\u8003\u8651\u8d5e\u52a9\u8be5\u9879\u76ee\u4ee5\u94fe\u63a5\u591a\u4e2a\u8fdc\u7a0b\u5b89\u88c5\u3002",
             "pendingTaskHaltedPostProcessorQueueFull": "\u540e\u5904\u7406\u5668\u961f\u5217\u8fbe\u5230\u6781\u9650",
             "pendingTaskHaltedPostProcessorQueueFullMessage": "\u5728\u540e\u5904\u7406\u5668\u961f\u5217\u4f4e\u4e8e\u5f53\u524d\u914d\u7f6e\u7684\u5de5\u4f5c\u4eba\u5458\u8ba1\u6570\u4e4b\u524d\uff0c\u5de5\u4f5c\u4eba\u5458\u4e0d\u4f1a\u6536\u5230\u65b0\u7684\u5f85\u5904\u7406\u4efb\u52a1",
             "pluginSettingsChangeWorkersStopped": "Unmanic \u5df2\u505c\u6b62\u6240\u6709\u5de5\u4f5c\u4eba\u5458\uff0c\u56e0\u4e3a\u5b83\u68c0\u6d4b\u5230\u63d2\u4ef6\u914d\u7f6e\u53d1\u751f\u66f4\u6539\u3002\u51c6\u5907\u597d\u540e\uff0c\u4ece\u4eea\u8868\u677f\u6062\u590d\u5de5\u4f5c\u4eba\u5458\u3002",
             "receivingRemoteFile": "\u63a5\u6536\u8fdc\u7a0b\u6587\u4ef6"
+        },
+        "serverNotificationLabels": {
+            "failedTaskLabel": "\u4efb\u52a1\u5931\u8d25"
         }
     },
     "status": {
         "all": "\u5168\u90e8",
         "cannotLoadImage": "\u65e0\u6cd5\u52a0\u8f7d\u56fe\u7247",
         "disabled": "\u5df2\u7981\u7528",
         "enabled": "\u542f\u7528",
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/language/it.json` & `unmanic-0.2.4/unmanic/webserver/frontend/src/language/it.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9725029322073656%*

 * *Differences: {"'buttons'": "{'dismissAll': 'Ignora tutto'}",*

 * * "'components'": "{'plugins': {'installPluginFromRepo': 'Installa il plugin dal repository', "*

 * *                 "'installPluginFromFile': 'Installa plug-in da file', 'invalidZipFile': 'Il file "*

 * *                 "non è un file ZIP valido', 'failedToInstallPluginFromZip': 'Impossibile "*

 * *                 "installare il plug-in dal file ZIP caricato', 'installedPluginFromZip': 'Plugin "*

 * *                 "installato', delete: ['installPlugins']}}",*

 * * "'notification […]*

```diff
@@ -1,10 +1,11 @@
 {
     "buttons": {
         "darkMode": "Modalit\u00e0 scura",
+        "dismissAll": "Ignora tutto",
         "language": "Lingua"
     },
     "components": {
         "completedTasks": {
             "addToPendingTasksList": "Aggiungi selezionato all'elenco delle attivit\u00e0 in sospeso",
             "before": "Prima",
             "details": "Particolari",
@@ -27,16 +28,20 @@
         },
         "plugins": {
             "addRepository": "Aggiungi repository",
             "author": "Autore",
             "categoryFilter": "Filtro di categoria",
             "clickToUpdatePlugin": "Fare clic per aggiornare il plug-in",
             "errorSavingFlow": "Si \u00e8 verificato un errore durante il salvataggio del flusso di plug-in",
+            "failedToInstallPluginFromZip": "Impossibile installare il plug-in dal file ZIP caricato",
             "globalConfiguration": "Configurazione globale",
-            "installPlugins": "Installa plug-in",
+            "installPluginFromFile": "Installa plug-in da file",
+            "installPluginFromRepo": "Installa il plugin dal repository",
+            "installedPluginFromZip": "Plugin installato",
+            "invalidZipFile": "Il file non \u00e8 un file ZIP valido",
             "newRepository": "Nuovo archivio",
             "pluginUpToDate": "Il plugin \u00e8 aggiornato",
             "refreshRepositories": "Aggiorna repository",
             "removePlugin": "Rimuovi plug-in",
             "repo": "Repository",
             "repoList": "Elenco repository",
             "repoName": "Nome",
@@ -315,14 +320,17 @@
             "libraryEnabledLimits": "Unmanic ha interrotto l'elaborazione delle attivit\u00e0 perch\u00e9 hai troppe librerie configurate per un livello non supporter. Prendi in considerazione la possibilit\u00e0 di sponsorizzare il progetto per abilitare pi\u00f9 di 2 biblioteche.",
             "libraryScanProgress": "Scansione della libreria in esecuzione",
             "linkedInstallationLimits": "Unmanic ha interrotto l'elaborazione delle attivit\u00e0 poich\u00e9 hai collegato troppe installazioni remote per un livello non supporter. Prendi in considerazione la possibilit\u00e0 di sponsorizzare il progetto per collegare pi\u00f9 di un'installazione remota.",
             "pendingTaskHaltedPostProcessorQueueFull": "La coda del post-processore ha raggiunto il limite",
             "pendingTaskHaltedPostProcessorQueueFullMessage": "I lavoratori non riceveranno una nuova attivit\u00e0 in sospeso finch\u00e9 la coda del post-processore non scende al di sotto del conteggio dei lavoratori attualmente configurato",
             "pluginSettingsChangeWorkersStopped": "Unmanic ha fermato tutti i lavoratori poich\u00e9 ha rilevato una modifica alla configurazione dei plugin. Quando sei pronto, riprendi i lavoratori dalla dashboard.",
             "receivingRemoteFile": "Ricezione file remoto"
+        },
+        "serverNotificationLabels": {
+            "failedTaskLabel": "Compito fallito"
         }
     },
     "status": {
         "all": "Tutto",
         "cannotLoadImage": "Impossibile caricare l'immagine",
         "disabled": "Disabilitato",
         "enabled": "Abilitato",
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/language/ru.json` & `unmanic-0.2.4/unmanic/webserver/frontend/src/language/ru.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9708436294396885%*

 * *Differences: {"'buttons'": "{'dismissAll': 'Отклонить все'}",*

 * * "'components'": "{'settings': {'library': {'runLibraryScanOnStart': 'Запуск одноразового "*

 * *                 "сканирования библиотеки при запуске', 'pathDisabledReceiveRemoteFilesOnly': "*

 * *                 "'Опция отключена, так как вы настроили эту библиотеку только для получения "*

 * *                 "удаленных файлов.'}}, 'workers': {'workerPausedFailed': 'Unmanic не смог "*

 * *                 "приостановить этого воркера по какой-то причине', 'workerResumedFaile […]*

```diff
@@ -1,10 +1,11 @@
 {
     "buttons": {
         "darkMode": "\u0422\u0435\u043c\u043d\u044b\u0439 \u0440\u0435\u0436\u0438\u043c",
+        "dismissAll": "\u041e\u0442\u043a\u043b\u043e\u043d\u0438\u0442\u044c \u0432\u0441\u0435",
         "language": "\u042f\u0437\u044b\u043a"
     },
     "components": {
         "completedTasks": {
             "addToPendingTasksList": "\u0414\u043e\u0431\u0430\u0432\u0438\u0442\u044c \u0432\u044b\u0431\u0440\u0430\u043d\u043d\u043e\u0435 \u0432 \u0441\u043f\u0438\u0441\u043e\u043a \u043e\u0436\u0438\u0434\u0430\u044e\u0449\u0438\u0445 \u0432\u044b\u043f\u043e\u043b\u043d\u0435\u043d\u0438\u044f \u0437\u0430\u0434\u0430\u0447",
             "before": "\u0414\u043e",
             "details": "\u041f\u043e\u0434\u0440\u043e\u0431\u043d\u043e\u0441\u0442\u0438",
@@ -27,16 +28,20 @@
         },
         "plugins": {
             "addRepository": "\u0414\u043e\u0431\u0430\u0432\u0438\u0442\u044c \u0440\u0435\u043f\u043e\u0437\u0438\u0442\u043e\u0440\u0438\u0439",
             "author": "\u0410\u0432\u0442\u043e\u0440",
             "categoryFilter": "\u0424\u0438\u043b\u044c\u0442\u0440 \u043a\u0430\u0442\u0435\u0433\u043e\u0440\u0438\u0439",
             "clickToUpdatePlugin": "\u041d\u0430\u0436\u043c\u0438\u0442\u0435, \u0447\u0442\u043e\u0431\u044b \u043e\u0431\u043d\u043e\u0432\u0438\u0442\u044c \u043f\u043b\u0430\u0433\u0438\u043d",
             "errorSavingFlow": "\u041f\u0440\u043e\u0438\u0437\u043e\u0448\u043b\u0430 \u043e\u0448\u0438\u0431\u043a\u0430 \u043f\u0440\u0438 \u0441\u043e\u0445\u0440\u0430\u043d\u0435\u043d\u0438\u0438 \u043f\u043e\u0442\u043e\u043a\u0430 \u043f\u043b\u0430\u0433\u0438\u043d\u0430",
+            "failedToInstallPluginFromZip": "\u041d\u0435 \u0443\u0434\u0430\u043b\u043e\u0441\u044c \u0443\u0441\u0442\u0430\u043d\u043e\u0432\u0438\u0442\u044c \u043f\u043b\u0430\u0433\u0438\u043d \u0438\u0437 \u0437\u0430\u0433\u0440\u0443\u0436\u0435\u043d\u043d\u043e\u0433\u043e ZIP-\u0444\u0430\u0439\u043b\u0430",
             "globalConfiguration": "\u0413\u043b\u043e\u0431\u0430\u043b\u044c\u043d\u0430\u044f \u043a\u043e\u043d\u0444\u0438\u0433\u0443\u0440\u0430\u0446\u0438\u044f",
-            "installPlugins": "\u0423\u0441\u0442\u0430\u043d\u043e\u0432\u0438\u0442\u044c \u043f\u043b\u0430\u0433\u0438\u043d",
+            "installPluginFromFile": "\u0423\u0441\u0442\u0430\u043d\u043e\u0432\u0438\u0442\u044c \u043f\u043b\u0430\u0433\u0438\u043d \u0438\u0437 \u0444\u0430\u0439\u043b\u0430",
+            "installPluginFromRepo": "\u0423\u0441\u0442\u0430\u043d\u043e\u0432\u0438\u0442\u044c \u043f\u043b\u0430\u0433\u0438\u043d \u0438\u0437 \u0440\u0435\u043f\u043e\u0437\u0438\u0442\u043e\u0440\u0438\u044f",
+            "installedPluginFromZip": "\u041f\u043b\u0430\u0433\u0438\u043d \u0443\u0441\u0442\u0430\u043d\u043e\u0432\u043b\u0435\u043d",
+            "invalidZipFile": "\u0424\u0430\u0439\u043b \u043d\u0435 \u044f\u0432\u043b\u044f\u0435\u0442\u0441\u044f \u0434\u043e\u043f\u0443\u0441\u0442\u0438\u043c\u044b\u043c ZIP-\u0444\u0430\u0439\u043b\u043e\u043c",
             "newRepository": "\u041d\u043e\u0432\u044b\u0439 \u0440\u0435\u043f\u043e\u0437\u0438\u0442\u043e\u0440\u0438\u0439",
             "pluginUpToDate": "\u041f\u043b\u0430\u0433\u0438\u043d \u043e\u0431\u043d\u043e\u0432\u043b\u0435\u043d",
             "refreshRepositories": "\u041e\u0431\u043d\u043e\u0432\u0438\u0442\u044c \u0440\u0435\u043f\u043e\u0437\u0438\u0442\u043e\u0440\u0438\u0438",
             "removePlugin": "\u0423\u0434\u0430\u043b\u0438\u0442\u044c \u043f\u043b\u0430\u0433\u0438\u043d",
             "repo": "\u0420\u0435\u043f\u043e\u0437\u0438\u0442\u043e\u0440\u0438\u0439",
             "repoList": "\u0421\u043f\u0438\u0441\u043e\u043a \u0440\u0435\u043f\u043e\u0437\u0438\u0442\u043e\u0440\u0438\u0435\u0432",
             "repoName": "\u0418\u043c\u044f",
@@ -94,20 +99,20 @@
                 "libraryScannerStatusLabel": "\u0411\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u0447\u043d\u044b\u0439 \u0441\u043a\u0430\u043d\u0435\u0440",
                 "locked": "\u0411\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0443 \u043d\u0435\u043b\u044c\u0437\u044f \u0443\u0434\u0430\u043b\u0438\u0442\u044c",
                 "maxAgeOfCompletedTasks": "\u041c\u0430\u043a\u0441\u0438\u043c\u0430\u043b\u044c\u043d\u043e\u0435 \u043a\u043e\u043b\u0438\u0447\u0435\u0441\u0442\u0432\u043e \u0434\u043d\u0435\u0439 \u0434\u043b\u044f \u0445\u0440\u0430\u043d\u0435\u043d\u0438\u044f \u0432\u044b\u043f\u043e\u043b\u043d\u0435\u043d\u043d\u044b\u0445 \u0437\u0430\u0434\u0430\u0447",
                 "name": "\u0418\u043c\u044f (\u0434\u043e\u043b\u0436\u043d\u043e \u0431\u044b\u0442\u044c \u0443\u043d\u0438\u043a\u0430\u043b\u044c\u043d\u044b\u043c)",
                 "newLibrary": "\u041d\u043e\u0432\u0430\u044f \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0430",
                 "path": "\u041f\u0443\u0442\u044c \u043a \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0435",
                 "pathConfiguration": "\u0411\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0438",
-                "pathDisabledReceiveRemoteFilesOnly": "\u041e\u043f\u0446\u0438\u044f \u043e\u0442\u043a\u043b\u044e\u0447\u0435\u043d\u0430, \u0442\u0430\u043a \u043a\u0430\u043a \u0432\u044b \u043d\u0430\u0441\u0442\u0440\u043e\u0438\u043b\u0438 \u044d\u0442\u0443 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0443 \u0434\u043b\u044f \u043f\u043e\u043b\u0443\u0447\u0435\u043d\u0438\u044f \u0442\u043e\u043b\u044c\u043a\u043e \u0443\u0434\u0430\u043b\u0435\u043d\u043d\u044b\u0445 \u0444\u0430\u0439\u043b\u043e\u0432.",
+                "pathDisabledReceiveRemoteFilesOnly": "\u041e\u043f\u0446\u0438\u044f \u043e\u0442\u043a\u043b\u044e\u0447\u0435\u043d\u0430, \u0442\u0430\u043a \u043a\u0430\u043a \u0432\u044b \u043d\u0430\u0441\u0442\u0440\u043e\u0438\u043b\u0438 \u044d\u0442\u0443 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0443 \u0442\u043e\u043b\u044c\u043a\u043e \u0434\u043b\u044f \u043f\u043e\u043b\u0443\u0447\u0435\u043d\u0438\u044f \u0443\u0434\u0430\u043b\u0435\u043d\u043d\u044b\u0445 \u0444\u0430\u0439\u043b\u043e\u0432.",
                 "pendingTasks": "\u041d\u0435\u0437\u0430\u0432\u0435\u0440\u0448\u0435\u043d\u043d\u044b\u0435 \u0437\u0430\u0434\u0430\u0447\u0438",
                 "pluginFlow": "\u041f\u043e\u0442\u043e\u043a \u043f\u043b\u0430\u0433\u0438\u043d\u043e\u0432",
                 "plugins": "\u041f\u043b\u0430\u0433\u0438\u043d\u044b",
                 "priorityScore": "\u0423\u0441\u0442\u0430\u043d\u043e\u0432\u0438\u0442\u0435 \u043c\u043e\u0434\u0438\u0444\u0438\u043a\u0430\u0442\u043e\u0440 \u043e\u0446\u0435\u043d\u043a\u0438 \u043f\u0440\u0438\u043e\u0440\u0438\u0442\u0435\u0442\u0430 \u0434\u043b\u044f \u0437\u0430\u0434\u0430\u0447, \u0441\u043e\u0437\u0434\u0430\u043d\u043d\u044b\u0445 \u0434\u043b\u044f \u044d\u0442\u043e\u0439 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0438.",
-                "runLibraryScanOnStart": "\u0417\u0430\u043f\u0443\u0441\u043a \u043e\u0434\u043d\u043e\u043a\u0440\u0430\u0442\u043d\u043e\u0433\u043e \u0441\u043a\u0430\u043d\u0438\u0440\u043e\u0432\u0430\u043d\u0438\u044f \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0438 \u043f\u0440\u0438 \u0437\u0430\u043f\u0443\u0441\u043a\u0435",
+                "runLibraryScanOnStart": "\u0417\u0430\u043f\u0443\u0441\u043a \u043e\u0434\u043d\u043e\u0440\u0430\u0437\u043e\u0432\u043e\u0433\u043e \u0441\u043a\u0430\u043d\u0438\u0440\u043e\u0432\u0430\u043d\u0438\u044f \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0438 \u043f\u0440\u0438 \u0437\u0430\u043f\u0443\u0441\u043a\u0435",
                 "unlocked": "\u0411\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0443 \u043c\u043e\u0436\u043d\u043e \u0443\u0434\u0430\u043b\u0438\u0442\u044c"
             },
             "link": {
                 "add": "\u0414\u043e\u0431\u0430\u0432\u043b\u044f\u0442\u044c",
                 "addRemoteInstallation": "\u0414\u043e\u0431\u0430\u0432\u0438\u0442\u044c \u0443\u0434\u0430\u043b\u0435\u043d\u043d\u0443\u044e \u0443\u0441\u0442\u0430\u043d\u043e\u0432\u043a\u0443",
                 "address": "\u0410\u0434\u0440\u0435\u0441",
                 "allowReceivingTasks": "\u041f\u043e\u043b\u0443\u0447\u0430\u0442\u044c \u0437\u0430\u0434\u0430\u0447\u0438 \u0438\u0437 \u044d\u0442\u043e\u0439 \u0443\u0441\u0442\u0430\u043d\u043e\u0432\u043a\u0438, \u043a\u043e\u0433\u0434\u0430 \u0440\u0430\u0431\u043e\u0447\u0438\u0435 \u0434\u043e\u0441\u0442\u0443\u043f\u043d\u044b",
@@ -192,15 +197,15 @@
                 "indeterminate": "\u041d\u0435\u043e\u043f\u0440\u0435\u0434\u0435\u043b\u0435\u043d\u043d\u044b\u0439",
                 "none": "\u041d\u0438\u043a\u0442\u043e"
             },
             "currentRunnerLabel": "\u0422\u0435\u043a\u0443\u0449\u0438\u0439 \u0431\u0435\u0433\u0443\u043d",
             "listEmpty": "\u0412 \u043d\u0430\u0441\u0442\u043e\u044f\u0449\u0435\u0435 \u0432\u0440\u0435\u043c\u044f \u043d\u0435\u0442 \u0440\u0430\u0431\u043e\u0442\u0430\u044e\u0449\u0438\u0445 \u0440\u0430\u0431\u043e\u0447\u0438\u0445. \u0423\u0432\u0435\u043b\u0438\u0447\u044c\u0442\u0435 \u043a\u043e\u043b\u0438\u0447\u0435\u0441\u0442\u0432\u043e \u0440\u0430\u0431\u043e\u0447\u0438\u0445 \u0432 \u043d\u0430\u0441\u0442\u0440\u043e\u0439\u043a\u0430\u0445 Unmanic, \u0447\u0442\u043e\u0431\u044b \u0441\u043e\u0437\u0434\u0430\u0442\u044c \u0440\u0430\u0431\u043e\u0447\u0435\u0433\u043e.",
             "pauseAllWorkers": "\u041f\u0440\u0438\u043e\u0441\u0442\u0430\u043d\u043e\u0432\u0438\u0442\u044c \u0432\u0441\u0435\u0445 \u0440\u0430\u0431\u043e\u0447\u0438\u0445",
             "pauseWorker": "\u041f\u0440\u0438\u043e\u0441\u0442\u0430\u043d\u043e\u0432\u0438\u0442\u044c \u044d\u0442\u043e\u0433\u043e \u0440\u0430\u0431\u043e\u0442\u043d\u0438\u043a\u0430",
-            "resumeAllWorkers": "\u0412\u043e\u0437\u043e\u0431\u043d\u043e\u0432\u0438\u0442\u044c \u0432\u0441\u0435\u0445 \u0440\u0430\u0431\u043e\u0447\u0438\u0445",
+            "resumeAllWorkers": "\u0412\u043e\u0437\u043e\u0431\u043d\u043e\u0432\u0438\u0442\u044c \u0432\u0441\u0435\u0445 \u0440\u0430\u0431\u043e\u0442\u043d\u0438\u043a\u043e\u0432",
             "resumeWorker": "\u0412\u043e\u0437\u043e\u0431\u043d\u043e\u0432\u0438\u0442\u044c \u044d\u0442\u043e\u0433\u043e \u0440\u0430\u0431\u043e\u0442\u043d\u0438\u043a\u0430",
             "startTimeLabel": "\u0412\u0440\u0435\u043c\u044f \u043d\u0430\u0447\u0430\u043b\u0430",
             "state": {
                 "paused": "\u0420\u0430\u0431\u043e\u0447\u0438\u0439 \u043e\u0441\u0442\u0430\u043d\u043e\u0432\u0438\u043b\u0441\u044f...",
                 "processing": "\u041e\u0431\u0440\u0430\u0431\u043e\u0442\u043a\u0430 \u0437\u0430\u0434\u0430\u0447\u0438...",
                 "waiting": "\u0416\u0434\u0443 \u0434\u0440\u0443\u0433\u043e\u0433\u043e \u0437\u0430\u0434\u0430\u043d\u0438\u044f..."
             },
@@ -208,17 +213,17 @@
             "status": "\u0421\u0442\u0430\u0442\u0443\u0441",
             "terminateAllWorkers": "\u0423\u0432\u043e\u043b\u0438\u0442\u044c \u0432\u0441\u0435\u0445 \u0440\u0430\u0431\u043e\u0447\u0438\u0445",
             "terminateWorker": "\u0423\u0432\u043e\u043b\u0438\u0442\u044c \u044d\u0442\u043e\u0433\u043e \u0440\u0430\u0431\u043e\u0442\u043d\u0438\u043a\u0430",
             "terminateWorkerWarning": "\u0412\u044b \u0443\u0432\u0435\u0440\u0435\u043d\u044b, \u0447\u0442\u043e \u0445\u043e\u0442\u0438\u0442\u0435 \u0437\u0430\u0432\u0435\u0440\u0448\u0438\u0442\u044c \u044d\u0442\u043e\u0442 \u0440\u0430\u0431\u043e\u0447\u0438\u0439 \u043f\u0440\u043e\u0446\u0435\u0441\u0441 \u0438 \u0435\u0433\u043e \u0442\u0435\u043a\u0443\u0449\u0443\u044e \u0437\u0430\u0434\u0430\u0447\u0443? \u0422\u0435\u043a\u0443\u0449\u0430\u044f \u0437\u0430\u0434\u0430\u0447\u0430 \u0431\u0443\u0434\u0435\u0442 \u043f\u043e\u043c\u0435\u0447\u0435\u043d\u0430 \u043a\u0430\u043a \u043d\u0435\u0432\u044b\u043f\u043e\u043b\u043d\u0435\u043d\u043d\u0430\u044f \u0432 \u0441\u043f\u0438\u0441\u043a\u0435 \u0432\u044b\u043f\u043e\u043b\u043d\u0435\u043d\u043d\u044b\u0445 \u0437\u0430\u0434\u0430\u0447.",
             "totalProcessingTimeLabel": "\u041e\u0431\u0449\u0435\u0435 \u0432\u0440\u0435\u043c\u044f \u043e\u0431\u0440\u0430\u0431\u043e\u0442\u043a\u0438",
             "workerLog": "\u0420\u0430\u0431\u043e\u0447\u0438\u0439 \u0436\u0443\u0440\u043d\u0430\u043b",
             "workerPaused": "\u0420\u0430\u0431\u043e\u0447\u0438\u0439 \u0431\u044b\u043b \u043f\u0440\u0438\u043e\u0441\u0442\u0430\u043d\u043e\u0432\u043b\u0435\u043d",
-            "workerPausedFailed": "Unmanic \u043d\u0435 \u0441\u043c\u043e\u0433 \u043f\u0440\u0438\u043e\u0441\u0442\u0430\u043d\u043e\u0432\u0438\u0442\u044c \u044d\u0442\u043e\u0433\u043e \u0440\u0430\u0431\u043e\u0442\u043d\u0438\u043a\u0430 \u043f\u043e \u043a\u0430\u043a\u043e\u0439-\u0442\u043e \u043f\u0440\u0438\u0447\u0438\u043d\u0435",
+            "workerPausedFailed": "Unmanic \u043d\u0435 \u0441\u043c\u043e\u0433 \u043f\u0440\u0438\u043e\u0441\u0442\u0430\u043d\u043e\u0432\u0438\u0442\u044c \u044d\u0442\u043e\u0433\u043e \u0432\u043e\u0440\u043a\u0435\u0440\u0430 \u043f\u043e \u043a\u0430\u043a\u043e\u0439-\u0442\u043e \u043f\u0440\u0438\u0447\u0438\u043d\u0435",
             "workerResumed": "\u0420\u0430\u0431\u043e\u0442\u043d\u0438\u043a \u0431\u044b\u043b \u0432\u043e\u0437\u043e\u0431\u043d\u043e\u0432\u043b\u0435\u043d",
-            "workerResumedFailed": "Unmanic \u043d\u0435 \u0441\u043c\u043e\u0433 \u0432\u043e\u0437\u043e\u0431\u043d\u043e\u0432\u0438\u0442\u044c \u0440\u0430\u0431\u043e\u0442\u0443 \u044d\u0442\u043e\u0433\u043e \u0432\u043e\u0440\u043a\u0435\u0440\u0430 \u043f\u043e \u043a\u0430\u043a\u043e\u0439-\u0442\u043e \u043f\u0440\u0438\u0447\u0438\u043d\u0435",
+            "workerResumedFailed": "Unmanic \u043d\u0435 \u0441\u043c\u043e\u0433 \u0432\u043e\u0437\u043e\u0431\u043d\u043e\u0432\u0438\u0442\u044c \u0440\u0430\u0431\u043e\u0442\u0443 \u044d\u0442\u043e\u0433\u043e \u0440\u0430\u0431\u043e\u0442\u043d\u0438\u043a\u0430 \u043f\u043e \u043a\u0430\u043a\u043e\u0439-\u0442\u043e \u043f\u0440\u0438\u0447\u0438\u043d\u0435",
             "workerTerminated": "\u0420\u0430\u0431\u043e\u0447\u0438\u0439 \u0431\u044b\u043b \u0443\u0432\u043e\u043b\u0435\u043d",
             "workerTerminationFailed": "Unmanic \u043f\u043e \u043a\u0430\u043a\u043e\u0439-\u0442\u043e \u043f\u0440\u0438\u0447\u0438\u043d\u0435 \u043d\u0435 \u0441\u043c\u043e\u0433 \u0437\u0430\u0432\u0435\u0440\u0448\u0438\u0442\u044c \u0440\u0430\u0431\u043e\u0442\u0443 \u044d\u0442\u043e\u0433\u043e \u0440\u0430\u0431\u043e\u0442\u043d\u0438\u043a\u0430"
         }
     },
     "headers": {
         "completedTaskDetails": "\u0421\u0432\u0435\u0434\u0435\u043d\u0438\u044f \u043e \u0432\u044b\u043f\u043e\u043b\u043d\u0435\u043d\u043d\u043e\u0439 \u0437\u0430\u0434\u0430\u0447\u0435",
         "completedTasks": "\u0417\u0430\u0432\u0435\u0440\u0448\u0435\u043d\u043d\u044b\u0435 \u0437\u0430\u0434\u0430\u0447\u0438",
@@ -257,15 +262,15 @@
         "documentation": "\u0414\u043e\u043a\u0443\u043c\u0435\u043d\u0442\u0430\u0446\u0438\u044f",
         "helpAndSupport": "\u041f\u043e\u043c\u043e\u0449\u044c \u0438 \u043f\u043e\u0434\u0434\u0435\u0440\u0436\u043a\u0430",
         "info": "\u0418\u043d\u0444\u043e\u0440\u043c\u0430\u0446\u0438\u044f",
         "library": "\u0411\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0430",
         "link": "\u0421\u0441\u044b\u043b\u043a\u0430 \u043d\u0430 \u0441\u0430\u0439\u0442",
         "login": "\u0410\u0432\u0442\u043e\u0440\u0438\u0437\u043e\u0432\u0430\u0442\u044c\u0441\u044f",
         "loginWithDiscord": "\u0412\u043e\u0439\u0442\u0438 \u0447\u0435\u0440\u0435\u0437 \u0414\u0438\u0441\u043a\u043e\u0440\u0434",
-        "loginWithGitHub": "\u0412\u043e\u0439\u0442\u0438 \u0447\u0435\u0440\u0435\u0437 GitHub",
+        "loginWithGitHub": "\u0412\u043e\u0439\u0442\u0438 \u0441 \u043f\u043e\u043c\u043e\u0449\u044c\u044e GitHub",
         "loginWithPatreon": "\u0412\u043e\u0439\u0442\u0438 \u0447\u0435\u0440\u0435\u0437 \u041f\u0430\u0442\u0440\u0435\u043e\u043d",
         "logout": "\u0412\u044b\u0439\u0442\u0438",
         "options": "\u041e\u043f\u0446\u0438\u0438",
         "plugins": "\u041f\u043b\u0430\u0433\u0438\u043d\u044b",
         "save": "\u0421\u043e\u0445\u0440\u0430\u043d\u044f\u0442\u044c",
         "search": "\u041f\u043e\u0438\u0441\u043a",
         "settings": "\u041d\u0430\u0441\u0442\u0440\u043e\u0439\u043a\u0438",
@@ -312,17 +317,20 @@
                 "warning": "\u041d\u0435\u0438\u0437\u0432\u0435\u0441\u0442\u043d\u043e\u0435 \u043f\u0440\u0435\u0434\u0443\u043f\u0440\u0435\u0436\u0434\u0435\u043d\u0438\u0435 \u043e\u0442 \u0441\u0435\u0440\u0432\u0435\u0440\u0430"
             },
             "incompatiblePlugin": "Unmanic \u043f\u0440\u0435\u043a\u0440\u0430\u0442\u0438\u043b \u043e\u0431\u0440\u0430\u0431\u043e\u0442\u043a\u0443 \u0437\u0430\u0434\u0430\u0447, \u0442\u0430\u043a \u043a\u0430\u043a \u043e\u0431\u043d\u0430\u0440\u0443\u0436\u0438\u043b \u043d\u0435\u0441\u043e\u0432\u043c\u0435\u0441\u0442\u0438\u043c\u044b\u0439 \u043f\u043b\u0430\u0433\u0438\u043d, \u0432\u043a\u043b\u044e\u0447\u0435\u043d\u043d\u044b\u0439 \u0432 \u043e\u0434\u043d\u043e\u0439 \u0438\u0437 \u0432\u0430\u0448\u0438\u0445 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a.",
             "libraryEnabledLimits": "Unmanic \u043f\u0440\u0435\u043a\u0440\u0430\u0442\u0438\u043b \u043e\u0431\u0440\u0430\u0431\u043e\u0442\u043a\u0443 \u0437\u0430\u0434\u0430\u0447, \u0442\u0430\u043a \u043a\u0430\u043a \u0443 \u0432\u0430\u0441 \u0441\u043b\u0438\u0448\u043a\u043e\u043c \u043c\u043d\u043e\u0433\u043e \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a, \u043d\u0430\u0441\u0442\u0440\u043e\u0435\u043d\u043d\u044b\u0445 \u0434\u043b\u044f \u0443\u0440\u043e\u0432\u043d\u044f \u0431\u0435\u0437 \u043f\u043e\u0434\u0434\u0435\u0440\u0436\u043a\u0438. \u0420\u0430\u0441\u0441\u043c\u043e\u0442\u0440\u0438\u0442\u0435 \u0432\u043e\u0437\u043c\u043e\u0436\u043d\u043e\u0441\u0442\u044c \u0441\u043f\u043e\u043d\u0441\u0438\u0440\u043e\u0432\u0430\u043d\u0438\u044f \u043f\u0440\u043e\u0435\u043a\u0442\u0430, \u0447\u0442\u043e\u0431\u044b \u0432\u043a\u043b\u044e\u0447\u0438\u0442\u044c \u0431\u043e\u043b\u0435\u0435 2 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a.",
             "libraryScanProgress": "\u0412\u044b\u043f\u043e\u043b\u043d\u044f\u0435\u0442\u0441\u044f \u0441\u043a\u0430\u043d\u0438\u0440\u043e\u0432\u0430\u043d\u0438\u0435 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0438",
             "linkedInstallationLimits": "Unmanic \u043f\u0440\u0435\u043a\u0440\u0430\u0442\u0438\u043b \u043e\u0431\u0440\u0430\u0431\u043e\u0442\u043a\u0443 \u0437\u0430\u0434\u0430\u0447, \u0442\u0430\u043a \u043a\u0430\u043a \u0432\u044b \u0441\u0432\u044f\u0437\u0430\u043b\u0438 \u0441\u043b\u0438\u0448\u043a\u043e\u043c \u043c\u043d\u043e\u0433\u043e \u0443\u0434\u0430\u043b\u0435\u043d\u043d\u044b\u0445 \u0443\u0441\u0442\u0430\u043d\u043e\u0432\u043e\u043a \u0434\u043b\u044f \u0443\u0440\u043e\u0432\u043d\u044f \u0431\u0435\u0437 \u043f\u043e\u0434\u0434\u0435\u0440\u0436\u043a\u0438. \u0420\u0430\u0441\u0441\u043c\u043e\u0442\u0440\u0438\u0442\u0435 \u0432\u043e\u0437\u043c\u043e\u0436\u043d\u043e\u0441\u0442\u044c \u0441\u043f\u043e\u043d\u0441\u0438\u0440\u043e\u0432\u0430\u043d\u0438\u044f \u043f\u0440\u043e\u0435\u043a\u0442\u0430, \u0447\u0442\u043e\u0431\u044b \u0441\u0432\u044f\u0437\u0430\u0442\u044c \u0431\u043e\u043b\u0435\u0435 \u043e\u0434\u043d\u043e\u0439 \u0443\u0434\u0430\u043b\u0435\u043d\u043d\u043e\u0439 \u0443\u0441\u0442\u0430\u043d\u043e\u0432\u043a\u0438.",
             "pendingTaskHaltedPostProcessorQueueFull": "\u041e\u0447\u0435\u0440\u0435\u0434\u044c \u043f\u043e\u0441\u0442\u043f\u0440\u043e\u0446\u0435\u0441\u0441\u043e\u0440\u0430 \u0434\u043e\u0441\u0442\u0438\u0433\u043b\u0430 \u043f\u0440\u0435\u0434\u0435\u043b\u0430",
-            "pendingTaskHaltedPostProcessorQueueFullMessage": "\u0420\u0430\u0431\u043e\u0447\u0438\u0435 \u043d\u0435 \u043f\u043e\u043b\u0443\u0447\u0430\u0442 \u043d\u043e\u0432\u0443\u044e \u043e\u0436\u0438\u0434\u0430\u044e\u0449\u0443\u044e \u0437\u0430\u0434\u0430\u0447\u0443, \u043f\u043e\u043a\u0430 \u043e\u0447\u0435\u0440\u0435\u0434\u044c \u043f\u043e\u0441\u0442\u043f\u0440\u043e\u0446\u0435\u0441\u0441\u043e\u0440\u0430 \u043d\u0435 \u0443\u043f\u0430\u0434\u0435\u0442 \u043d\u0438\u0436\u0435 \u0442\u0435\u043a\u0443\u0449\u0435\u0433\u043e \u043d\u0430\u0441\u0442\u0440\u043e\u0435\u043d\u043d\u043e\u0433\u043e \u043a\u043e\u043b\u0438\u0447\u0435\u0441\u0442\u0432\u0430 \u0440\u0430\u0431\u043e\u0447\u0438\u0445",
+            "pendingTaskHaltedPostProcessorQueueFullMessage": "\u0420\u0430\u0431\u043e\u0447\u0438\u0435 \u043d\u0435 \u043f\u043e\u043b\u0443\u0447\u0430\u0442 \u043d\u043e\u0432\u0443\u044e \u043e\u0442\u043b\u043e\u0436\u0435\u043d\u043d\u0443\u044e \u0437\u0430\u0434\u0430\u0447\u0443, \u043f\u043e\u043a\u0430 \u043e\u0447\u0435\u0440\u0435\u0434\u044c \u043f\u043e\u0441\u0442\u043f\u0440\u043e\u0446\u0435\u0441\u0441\u043e\u0440\u0430 \u043d\u0435 \u0443\u043f\u0430\u0434\u0435\u0442 \u043d\u0438\u0436\u0435 \u0442\u0435\u043a\u0443\u0449\u0435\u0433\u043e \u043d\u0430\u0441\u0442\u0440\u043e\u0435\u043d\u043d\u043e\u0433\u043e \u043a\u043e\u043b\u0438\u0447\u0435\u0441\u0442\u0432\u0430 \u0440\u0430\u0431\u043e\u0447\u0438\u0445.",
             "pluginSettingsChangeWorkersStopped": "Unmanic \u043e\u0441\u0442\u0430\u043d\u043e\u0432\u0438\u043b \u0432\u0441\u0435\u0445 \u0440\u0430\u0431\u043e\u0447\u0438\u0445, \u0442\u0430\u043a \u043a\u0430\u043a \u043e\u0431\u043d\u0430\u0440\u0443\u0436\u0438\u043b \u0438\u0437\u043c\u0435\u043d\u0435\u043d\u0438\u0435 \u0432 \u043a\u043e\u043d\u0444\u0438\u0433\u0443\u0440\u0430\u0446\u0438\u0438 \u043f\u043b\u0430\u0433\u0438\u043d\u043e\u0432. \u041a\u043e\u0433\u0434\u0430 \u0431\u0443\u0434\u0435\u0442\u0435 \u0433\u043e\u0442\u043e\u0432\u044b, \u0432\u043e\u0437\u043e\u0431\u043d\u043e\u0432\u0438\u0442\u0435 \u0440\u0430\u0431\u043e\u0442\u0443 \u0432\u043e\u0440\u043a\u0435\u0440\u043e\u0432 \u0441 \u043f\u0430\u043d\u0435\u043b\u0438 \u0443\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u044f.",
             "receivingRemoteFile": "\u041f\u043e\u043b\u0443\u0447\u0435\u043d\u0438\u0435 \u0443\u0434\u0430\u043b\u0435\u043d\u043d\u043e\u0433\u043e \u0444\u0430\u0439\u043b\u0430"
+        },
+        "serverNotificationLabels": {
+            "failedTaskLabel": "\u0421\u0431\u043e\u0439 \u0437\u0430\u0434\u0430\u0447\u0438"
         }
     },
     "status": {
         "all": "\u0412\u0441\u0435",
         "cannotLoadImage": "\u041d\u0435 \u0443\u0434\u0430\u0435\u0442\u0441\u044f \u0437\u0430\u0433\u0440\u0443\u0437\u0438\u0442\u044c \u0438\u0437\u043e\u0431\u0440\u0430\u0436\u0435\u043d\u0438\u0435",
         "disabled": "\u041d\u0435\u043f\u043e\u043b\u043d\u043e\u0446\u0435\u043d\u043d\u044b\u0439",
         "enabled": "\u0412\u043a\u043b\u044e\u0447\u0435\u043d\u043e",
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/language/nl.json` & `unmanic-0.2.4/unmanic/webserver/frontend/src/language/nl.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9629847185718844%*

 * *Differences: {"'buttons'": "{'dismissAll': 'Alles afkeuren'}",*

 * * "'components'": "{'settings': {'library': {'pathConfiguration': 'Bibliotheken', "*

 * *                 "'libraryScannerSchedule': 'Scanschema bibliotheek in minuten', 'cloneLibrary': "*

 * *                 "'Bibliotheek klonen', 'importPluginConfigMessage': 'Bibliotheekconfiguratie "*

 * *                 'importeren. Dit kan even duren als er plug-ins zijn die moeten worden '*

 * *                 "geïnstalleerd.'}, 'workers': {'scheduleLabels': {'pause': 'Alle werkers "*

 * *   […]*

```diff
@@ -1,55 +1,60 @@
 {
     "buttons": {
         "darkMode": "Donkere modus",
+        "dismissAll": "Alles afkeuren",
         "language": "Taal"
     },
     "components": {
         "completedTasks": {
             "addToPendingTasksList": "Geselecteerde toevoegen aan lijst met lopende taken",
             "before": "Voordat",
             "details": "Details",
             "errorGettingDetails": "Er is een fout opgetreden bij het ophalen van de details voor deze taak",
             "removeSelected": "Geselecteerde uit lijst verwijderen",
             "selectLibraryToAdd": "Selecteer bibliotheek waarin u deze taak opnieuw wilt maken",
             "since": "Sinds"
         },
         "dataPanels": {
-            "noDataPanelsEnabled": "U heeft geen datapanelen ingeschakeld. Installeer er een vanuit uw plug-in-instellingen."
+            "noDataPanelsEnabled": "U hebt geen datapanelen ingeschakeld. Installeer er een vanuit uw plug-in-instellingen."
         },
         "footer": {
             "version": "Versie"
         },
         "pendingTasks": {
             "moveToBottom": "Geselecteerde naar beneden verplaatsen",
-            "moveToTop": "Verplaats geselecteerde naar boven",
+            "moveToTop": "Geselecteerde naar boven verplaatsen",
             "removeSelected": "Geselecteerde uit lijst verwijderen",
             "rescanLibrary": "Bibliotheek nu opnieuw scannen"
         },
         "plugins": {
             "addRepository": "Opslagplaats toevoegen",
             "author": "Auteur",
             "categoryFilter": "Categoriefilter",
             "clickToUpdatePlugin": "Klik om de plug-in bij te werken",
-            "errorSavingFlow": "Er is een fout opgetreden tijdens het opslaan van de plug-instroom",
+            "errorSavingFlow": "Er is een fout opgetreden tijdens het opslaan van de Plugin Flow",
+            "failedToInstallPluginFromZip": "Kan plug-in niet installeren vanuit het ge\u00fcploade ZIP-bestand",
             "globalConfiguration": "Algemene configuratie",
-            "installPlugins": "Installeer plugin",
+            "installPluginFromFile": "Plug-in installeren vanuit bestand",
+            "installPluginFromRepo": "Installeer plug-in van repo",
+            "installedPluginFromZip": "Plug-in ge\u00efnstalleerd",
+            "invalidZipFile": "Bestand is geen geldig ZIP-bestand",
             "newRepository": "Nieuwe opslagplaats",
             "pluginUpToDate": "Plug-in is up-to-date",
             "refreshRepositories": "Opslagplaatsen vernieuwen",
             "removePlugin": "Plug-in verwijderen",
             "repo": "Opslagplaats",
             "repoList": "Lijst met opslagplaatsen",
             "repoName": "Naam",
             "repoSource": "Repository-URL",
             "resetConfiguration": "Configuratie resetten",
             "types": {
                 "libraryManagement": {
                     "fileTest": "Bibliotheekbeheer - Bestandstest",
-                    "fileTestCaption": "Deze plug-ins worden aangeroepen om te testen of bestanden moeten worden toegevoegd aan de in behandeling zijnde takenlijst"
+                    "fileTestCaption": "Deze plug-ins worden aangeroepen om te testen of bestanden moeten worden toegevoegd aan de takenlijst in behandeling"
                 },
                 "postprocessor": {
                     "fileMove": "Postprocessor - Bestandsverplaatsingen",
                     "fileMoveCaption": "Deze plug-ins worden aangeroepen na voltooiing van de taak om extra bestandsverplaatsingen toe te voegen",
                     "taskResult": "Post-processor - Taak succes/mislukking markeren",
                     "taskResultCaption": "Deze plug-ins worden aangeroepen bij het voltooien van een taak om het algehele succes of falen van die taak te markeren"
                 },
@@ -68,61 +73,61 @@
                 "tags": "Tags"
             },
             "library": {
                 "addPluginToThisLibrary": "Voeg plug-in toe aan deze bibliotheek",
                 "alwaysKeepFailedTasks": "Bewaar mislukte taken altijd",
                 "autoManageCompletedTasks": "Beheer voltooide taken automatisch",
                 "clearPendingTasksOnStart": "Wis alle lopende taken bij het opstarten",
-                "cloneLibrary": "Kloon bibliotheek",
+                "cloneLibrary": "Bibliotheek klonen",
                 "completedTasks": "Voltooide taken",
                 "concurrentFileTesters": "Gelijktijdige bestandstesters",
                 "confirmRemove": "Als u de bibliotheek verwijdert, worden ook alle instellingen verwijderd die aan deze bibliotheek zijn gekoppeld. Weet je zeker dat je wilt doorgaan?",
                 "defaultLibrary": "Standaardbibliotheek",
                 "enableInotify": "Bestandsmonitor inschakelen voor deze bibliotheek",
                 "enableLibraryScanner": "Periodieke bibliotheekscans inschakelen",
                 "enableReceiveRemoteFilesOnly": "Bibliotheek configureren om alleen externe bestanden te ontvangen",
                 "enableScanner": "Bibliotheekscanner inschakelen voor deze bibliotheek",
                 "exportLibraryConfig": "Configuratie exporteren",
                 "fileTesting": "Bestand testen",
                 "followSymlinks": "Symlinks volgen op bibliotheekscans",
                 "importLibraryConfig": "Configuratie importeren",
-                "importPluginConfigMessage": "Bibliotheekconfiguratie importeren. Dit kan enige tijd duren als er plug-ins zijn die moeten worden ge\u00efnstalleerd.",
+                "importPluginConfigMessage": "Bibliotheekconfiguratie importeren. Dit kan even duren als er plug-ins zijn die moeten worden ge\u00efnstalleerd.",
                 "libraryFileMonitorStatusLabel": "Bestandsmonitor",
                 "libraryRemoteOnlyStatus": "Alleen op afstand",
                 "libraryScanner": "Bibliotheekscanner",
-                "libraryScannerSchedule": "Bibliotheekscanschema in minuten",
+                "libraryScannerSchedule": "Scanschema bibliotheek in minuten",
                 "libraryScannerScheduleNotValid": "Scanschema bibliotheek niet geldig",
                 "libraryScannerStatusLabel": "Bibliotheekscanner",
                 "locked": "De bibliotheek kan niet worden verwijderd",
                 "maxAgeOfCompletedTasks": "Maximaal aantal dagen om voltooide taken te bewaren",
                 "name": "Naam (moet uniek zijn)",
                 "newLibrary": "Nieuwe bibliotheek",
                 "path": "Bibliotheekpad",
-                "pathConfiguration": "bibliotheken",
+                "pathConfiguration": "Bibliotheken",
                 "pathDisabledReceiveRemoteFilesOnly": "Optie uitgeschakeld omdat u deze bibliotheek alleen hebt geconfigureerd voor het ontvangen van externe bestanden",
                 "pendingTasks": "Taken in behandeling",
                 "pluginFlow": "Plugin-stroom",
                 "plugins": "Plug-ins",
                 "priorityScore": "Stel een prioriteitsscore-modifier in voor taken die voor deze bibliotheek zijn gegenereerd",
                 "runLibraryScanOnStart": "Voer een eenmalige bibliotheekscan uit bij het opstarten",
                 "unlocked": "De bibliotheek kan worden verwijderd"
             },
             "link": {
                 "add": "Toevoegen",
                 "addRemoteInstallation": "Installatie op afstand toevoegen",
                 "address": "Adres",
-                "allowReceivingTasks": "Taken van deze installatie ontvangen wanneer werknemers beschikbaar zijn",
+                "allowReceivingTasks": "Taken van deze installatie ontvangen wanneer er werknemers beschikbaar zijn",
                 "allowSendingTasks": "Stuur taken naar deze installatie wanneer er werkers beschikbaar zijn",
                 "authentication": "authenticatie",
                 "collectiveManagement": "Collectief beheer",
                 "connection": "Verbinding",
                 "enableChecksumValidation": "Valideer bestandsoverdrachten met checksums (langzaam)",
                 "enableConfigMissingLibraries": "Configureer automatisch ontbrekende bibliotheken op de externe installatie",
                 "enableDistributedWorkerCount": "Gedistribueerd aantal werknemers inschakelen voor deze link",
-                "enableTaskPreloading": "Preload een aantal taken op de externe installatie Wachtende taken wachtrij",
+                "enableTaskPreloading": "Laad enkele taken vooraf in de wachtrij voor in behandeling zijnde taken op afstand",
                 "linkConfigChecksumValidationStatusLabel": "Valideren met checksums",
                 "linkConfigRemoteLibrariesStatusLabel": "Ontbrekende bibliotheken configureren",
                 "linkDistributedWorkersStatusLabel": "Gedistribueerde arbeiders",
                 "linkPreloadRemoteTasksStatusLabel": "Taken op afstand vooraf laden",
                 "linkReceivingTasksStatusLabel": "Taken ontvangen",
                 "linkSendingTasksStatusLabel": "Taken verzenden",
                 "name": "Naam",
@@ -166,15 +171,15 @@
                 "repetition": "Herhaling",
                 "schedule": "Werkrooster voor evenementen",
                 "scheduleLabels": {
                     "count": "Aantal werknemers instellen",
                     "daily": "Dagelijks",
                     "friday": "Elke vrijdag",
                     "monday": "Elke maandag",
-                    "pause": "Pauzeer alle werkers",
+                    "pause": "Alle werkers pauzeren",
                     "resume": "Alle werknemers hervatten",
                     "saturday": "Elke zaterdag",
                     "sunday": "Elke zondag",
                     "thursday": "Elke donderdag",
                     "tuesday": "Elke dinsdag",
                     "wednesday": "Elke woensdag",
                     "weekday": "Elke weekdag",
@@ -190,15 +195,15 @@
         "workers": {
             "currentRunner": {
                 "indeterminate": "onbepaald",
                 "none": "Geen"
             },
             "currentRunnerLabel": "Huidige Runner",
             "listEmpty": "Er zijn momenteel geen arbeiders actief. Verhoog het aantal werkers in de instellingen van Unmanic om een werker te spawnen.",
-            "pauseAllWorkers": "Pauzeer alle werkers",
+            "pauseAllWorkers": "Alle werkers pauzeren",
             "pauseWorker": "Deze werknemer onderbreken",
             "resumeAllWorkers": "Alle werknemers hervatten",
             "resumeWorker": "Deze werknemer hervatten",
             "startTimeLabel": "Starttijd",
             "state": {
                 "paused": "Werknemer gepauzeerd...",
                 "processing": "Taak verwerken...",
@@ -231,15 +236,15 @@
         "libraryPluginConfig": "Configuratie van bibliotheekplug-in",
         "librarySettings": "Bibliotheekinstellingen",
         "listEmpty": "Deze takenlijst is leeg",
         "login": "Log in",
         "pendingTasks": "Taken in behandeling",
         "pluginInfo": "Plugin-info",
         "pluginInstaller": "Installatieprogramma voor plug-ins",
-        "pluginSettings": "Instellingen voor plug-ins",
+        "pluginSettings": "Plugin-instellingen",
         "privacyPolicy": "Privacybeleid",
         "releaseNotes": "Release-opmerkingen",
         "selectDirectory": "Selecteer een map",
         "selectLibrary": "Selecteer een bibliotheek",
         "selectPlugin": "Selecteer een plug-in",
         "supportFutureDevelopment": "Ondersteuning toekomstige ontwikkeling",
         "workers": "arbeiders"
@@ -274,18 +279,18 @@
         "submit": "Indienen",
         "workers": "arbeiders",
         "yes": "Ja"
     },
     "notifications": {
         "SavedPluginSettings": "Plugin-instellingen opgeslagen.",
         "allowPopups": "Sta pop-ups voor deze website toe.",
-        "backendConnectionWarning": "Kan geen verbinding maken met de Unmanic-backend. Controleer of het actief is.",
+        "backendConnectionWarning": "Kan geen verbinding maken met Unmanic-backend. Controleer of het actief is.",
         "cannotRemoveDefaultLibrary": "Kan de standaardbibliotheek niet verwijderen",
         "copied": "gekopieerd",
-        "failedToFetchEnabledDataPanelPlugins": "Kan de lijst met ingeschakelde plug-ins van het gegevenspaneel niet ophalen",
+        "failedToFetchEnabledDataPanelPlugins": "Kan de lijst met ingeschakelde plug-ins voor het gegevenspaneel niet ophalen",
         "failedToFetchLibraryList": "Kan de bibliotheeklijst van Unmanic niet ophalen.",
         "failedToFetchLoginUrl": "Kan inlog-URL niet ophalen.",
         "failedToFetchLogoutUrl": "Kan uitlog-URL niet ophalen.",
         "failedToFetchSettings": "Kan de huidige instellingen van Unmanic niet ophalen.",
         "failedToFetchSystemConfig": "Kan de systeemconfiguratie van Unmanic niet ophalen.",
         "failedToInstallPlugin": "Er is een fout opgetreden bij het installeren van de gevraagde plug-in.",
         "failedToSavePluginSettings": "Kan plug-ininstellingen niet opslaan.",
@@ -310,19 +315,22 @@
                 "status": "Onbekende statusupdate van server",
                 "success": "Onbekend bericht van server",
                 "warning": "Onbekende waarschuwing van server"
             },
             "incompatiblePlugin": "Unmanic is gestopt met het verwerken van taken omdat het een incompatibele plug-in heeft gedetecteerd die is ingeschakeld in een van uw bibliotheken",
             "libraryEnabledLimits": "Unmanic is gestopt met het verwerken van taken omdat u te veel bibliotheken hebt geconfigureerd voor een niet-supporterlaag. Overweeg het project te sponsoren om meer dan 2 bibliotheken mogelijk te maken.",
             "libraryScanProgress": "Bibliotheekscan wordt uitgevoerd",
-            "linkedInstallationLimits": "Unmanic is gestopt met het verwerken van taken omdat u te veel externe installaties hebt gekoppeld voor een niet-supporterlaag. Overweeg het project te sponsoren om meer dan \u00e9\u00e9n installatie op afstand te koppelen.",
+            "linkedInstallationLimits": "Unmanic is gestopt met het verwerken van taken omdat u te veel externe installaties hebt gekoppeld voor een niet-supporterlaag. Overweeg het project te sponsoren om meer dan \u00e9\u00e9n externe installatie te koppelen.",
             "pendingTaskHaltedPostProcessorQueueFull": "De wachtrij van de postprocessor heeft zijn limiet bereikt",
             "pendingTaskHaltedPostProcessorQueueFullMessage": "Werknemers ontvangen geen nieuwe taak die in behandeling is totdat de wachtrij na de processor onder het huidige geconfigureerde aantal werknemers komt",
             "pluginSettingsChangeWorkersStopped": "Unmanic heeft alle werkers gestopt omdat het een wijziging in de configuratie van de plug-ins heeft gedetecteerd. Als u klaar bent, hervat u de werknemers vanaf het dashboard.",
             "receivingRemoteFile": "Bestand op afstand ontvangen"
+        },
+        "serverNotificationLabels": {
+            "failedTaskLabel": "Taak mislukt"
         }
     },
     "status": {
         "all": "Allemaal",
         "cannotLoadImage": "Kan afbeelding niet laden",
         "disabled": "Gehandicapt",
         "enabled": "Ingeschakeld",
@@ -335,15 +343,15 @@
         "available": "Verkrijgbaar",
         "back": "Rug",
         "close": "Dichtbij",
         "configure": "Configureren",
         "configureForThisLibrary": "Configureren voor deze bibliotheek",
         "defaultLibrary": "Dit is de standaardbibliotheek. Het kan niet worden verwijderd.",
         "delete": "Verwijderen",
-        "etc": "Geschatte voltooiingstijd",
+        "etc": "Geschatte tijd van voltooiing",
         "install": "Installeren",
         "move": "Beweging",
         "pluginInfo": "Plugin-info",
         "position": "Positie",
         "reinstall": "Opnieuw installeren",
         "remove": "Verwijderen",
         "removeFromThisLibrary": "Verwijderen uit deze bibliotheek",
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/language/mi.json` & `unmanic-0.2.4/unmanic/webserver/frontend/src/language/mi.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9523804060724153%*

 * *Differences: {"'buttons'": "{'dismissAll': 'Waiho Katoa'}",*

 * * "'components'": "{'settings': {'library': {'defaultLibrary': 'Puna Taunoa', "*

 * *                 "'libraryScannerSchedule': 'Te raarangi karapa whare pukapuka i roto i nga "*

 * *                 "meneti', 'libraryScannerScheduleNotValid': 'Kaore i te whaimana te raarangi "*

 * *                 "karapa whare pukapuka', 'fileTesting': 'Whakamatau kōnae', "*

 * *                 "'concurrentFileTesters': 'Kaiwhakamātau kōnae kotahi', "*

 * *                 "'enableReceiveRemoteFile […]*

```diff
@@ -1,128 +1,133 @@
 {
     "buttons": {
         "darkMode": "Aratau pouri",
+        "dismissAll": "Waiho Katoa",
         "language": "Reo"
     },
     "components": {
         "completedTasks": {
             "addToPendingTasksList": "T\u0101pirihia i t\u012bpakohia ki te r\u0101rangi T\u016bmahi T\u0101rewa",
             "before": "I mua",
             "details": "Nga korero",
             "errorGettingDetails": "I hapa i te tiki i nga korero mo tenei mahi",
             "removeSelected": "Tango kua tohua mai i te rarangi",
             "selectLibraryToAdd": "T\u012bpakohia te whare pukapuka hei waihanga an\u014d i t\u0113nei mahi",
             "since": "Mai"
         },
         "dataPanels": {
-            "noDataPanelsEnabled": "Karekau he Paewhiri Raraunga e whakahohea ana. T\u0101utahia t\u0113tahi mai i \u014d tautuhinga mono."
+            "noDataPanelsEnabled": "Karekau he Paewhiri Raraunga kua whakahohea. T\u0101utahia t\u0113tahi mai i \u014d tautuhinga mono."
         },
         "footer": {
             "version": "Putanga"
         },
         "pendingTasks": {
             "moveToBottom": "Nuku kua tohua ki raro",
             "moveToTop": "Nuku kua tohua ki runga",
             "removeSelected": "Tango kua tohua mai i te rarangi",
             "rescanLibrary": "Matawai ano te whare pukapuka inaianei"
         },
         "plugins": {
             "addRepository": "T\u0101piri Pupuri",
             "author": "Kaituhi",
             "categoryFilter": "T\u0101tari K\u0101wai",
-            "clickToUpdatePlugin": "Paatohia ki te whakahou i te mono",
-            "errorSavingFlow": "I puta he hapa i te tiaki i te Rere Monomai",
+            "clickToUpdatePlugin": "P\u0101whiri ki te whakahou i te mono",
+            "errorSavingFlow": "I puta he hapa i te wa e tiaki ana i te Rere Monomai",
+            "failedToInstallPluginFromZip": "I rahua te whakauru monomai i te konae ZIP kua tuku ake",
             "globalConfiguration": "Whirihoranga Ao",
-            "installPlugins": "T\u0101uta monomai",
+            "installPluginFromFile": "T\u0101uta Mono Mai i te K\u014dnae",
+            "installPluginFromRepo": "T\u0101uta monomai Mai Repo",
+            "installedPluginFromZip": "Kua whakauruhia te mono",
+            "invalidZipFile": "Ehara te k\u014dnae i te k\u014dnae ZIP whaimana",
             "newRepository": "Whare Pupuri Hou",
-            "pluginUpToDate": "Ko te monomai he mea hou",
-            "refreshRepositories": "T\u0101mata Pupuri",
+            "pluginUpToDate": "Kei te hou te monomai",
+            "refreshRepositories": "T\u0101mata Ng\u0101 Putunga",
             "removePlugin": "Tango monomai",
             "repo": "Putunga",
             "repoList": "Rarangi Putunga",
             "repoName": "Ingoa",
             "repoSource": "URL putunga",
             "resetConfiguration": "Tautuhi whirihoranga",
             "types": {
                 "libraryManagement": {
                     "fileTest": "Whakahaere Whare Pukapuka - Whakamatau K\u014dnae",
                     "fileTestCaption": "Ka karangahia enei mono ki te whakamatautau mena me taapiri nga konae ki te rarangi mahi e tatari ana"
                 },
                 "postprocessor": {
                     "fileMove": "Tukatuka-muri - Nga nekehanga k\u014dnae",
-                    "fileMoveCaption": "Ka karangahia enei mono ki te whakaotinga o nga mahi hei taapiri atu i nga nekehanga konae",
-                    "taskResult": "Tukatuka-muri - Tohu i te angitu/rahunga mahi",
-                    "taskResultCaption": "Ka karangahia enei mono i runga i te otinga o tetahi mahi hei tohu i te angitu katoa, i te kore ranei o taua mahi"
+                    "fileMoveCaption": "Ka karangahia enei mono ki te whakaoti i nga mahi hei taapiri atu i nga nekehanga konae",
+                    "taskResult": "Pou-tukatuka - Tohu i te angitu/rahunga mahi",
+                    "taskResultCaption": "Ka karangahia enei mono i te otinga o tetahi mahi hei tohu i te angitu katoa, i te kore ranei o taua mahi"
                 },
                 "worker": {
                     "processItem": "Kaimahi - Tukatuka k\u014dnae",
                     "processItemCaption": "Ko enei mono ka karangahia e tetahi kaimahi me te whakaputa i tetahi whakahau ritenga hei whakahaere me te whakahaere e taua kaimahi"
                 }
             },
             "updateAvailable": "Kei te waatea te whakahou",
-            "updatePlugin": "Whakah\u014du Monomai",
+            "updatePlugin": "Whakah\u014du monomai",
             "version": "Putanga"
         },
         "settings": {
             "common": {
                 "configuration": "Whirihoranga",
                 "tags": "Tohutohu"
             },
             "library": {
                 "addPluginToThisLibrary": "T\u0101piri mono ki t\u0113nei whare pukapuka",
                 "alwaysKeepFailedTasks": "Kia mau tonu nga mahi kua rahua",
                 "autoManageCompletedTasks": "Whakahaere aunoa i nga mahi kua oti",
                 "clearPendingTasksOnStart": "\u016akuia ng\u0101 mahi t\u0101rewa katoa i te t\u012bmatanga",
                 "cloneLibrary": "whare pukapuka Clone",
                 "completedTasks": "Kua oti nga mahi",
-                "concurrentFileTesters": "Kaiwhakamatautau konae",
+                "concurrentFileTesters": "Kaiwhakam\u0101tau k\u014dnae kotahi",
                 "confirmRemove": "Ma te tango i te whare pukapuka ka tangohia nga tautuhinga katoa e hono ana ki tenei puna. Kei te tino hiahia koe ki te haere tonu?",
-                "defaultLibrary": "Whare Pukapuka Taunoa",
+                "defaultLibrary": "Puna Taunoa",
                 "enableInotify": "Whakahohe te aroturuki k\u014dnae mo tenei puna",
                 "enableLibraryScanner": "Whakahohehia te tirotiro whare pukapuka i ia wa",
-                "enableReceiveRemoteFilesOnly": "Whirihorahia te Whare Pukapuka mo te tango i nga konae mamao anake",
+                "enableReceiveRemoteFilesOnly": "Whirihorahia te Puna mo te whiwhi i nga konae mamao anake",
                 "enableScanner": "Whakahohehia te matawai whare pukapuka mo tenei whare pukapuka",
                 "exportLibraryConfig": "Kaweake whirihora",
-                "fileTesting": "Te whakamatautau i nga konae",
+                "fileTesting": "Whakamatau k\u014dnae",
                 "followSymlinks": "Whaia nga hononga tohu mo nga karapa whare pukapuka",
                 "importLibraryConfig": "Kawemai whirihora",
-                "importPluginConfigMessage": "Te kawemai i te whirihoranga whare pukapuka. Ka roa pea tenei mena he mono kei te hiahia kia whakauruhia.",
+                "importPluginConfigMessage": "Te kawemai i te whirihoranga whare pukapuka. Ka roa pea tenei mena he monomai e hiahia ana kia whakauruhia.",
                 "libraryFileMonitorStatusLabel": "Aroturuki k\u014dnae",
                 "libraryRemoteOnlyStatus": "Mamao anake",
                 "libraryScanner": "Matawai whare pukapuka",
-                "libraryScannerSchedule": "Te rarangi karapa whare pukapuka i roto i nga meneti",
-                "libraryScannerScheduleNotValid": "Karekau i te mana te raarangi karapa whare pukapuka",
+                "libraryScannerSchedule": "Te raarangi karapa whare pukapuka i roto i nga meneti",
+                "libraryScannerScheduleNotValid": "Kaore i te whaimana te raarangi karapa whare pukapuka",
                 "libraryScannerStatusLabel": "Matawai whare pukapuka",
-                "locked": "Kaore e taea te whakakore i te whare pukapuka",
+                "locked": "Kaore e taea te muku te whare pukapuka",
                 "maxAgeOfCompletedTasks": "Te maha o nga ra hei pupuri i nga mahi kua oti",
                 "name": "Ingoa (me ahurei)",
                 "newLibrary": "Whare Pukapuka Hou",
                 "path": "Te ara whare pukapuka",
                 "pathConfiguration": "Whare Pukapuka",
                 "pathDisabledReceiveRemoteFilesOnly": "Kua monoa te whiringa i te mea kua whirihorahia e koe tenei puna mo te tango i nga konae mamao anake",
                 "pendingTasks": "Nga mahi e tatari ana",
                 "pluginFlow": "Rere monomai",
                 "plugins": "monomai",
-                "priorityScore": "Whakatakotoria he whakarereke kaute matua mo nga mahi kua mahia mo tenei puna",
+                "priorityScore": "Tautuhia he whakarereke kaute matua mo nga mahi i hangaia mo tenei puna",
                 "runLibraryScanOnStart": "Whakahaerehia he karapa whare pukapuka kotahi i te tiimatanga",
                 "unlocked": "Ka taea te whakakore i te whare pukapuka"
             },
             "link": {
                 "add": "T\u0101piri",
                 "addRemoteInstallation": "T\u0101piri t\u0101utanga mamao",
                 "address": "W\u0101hitau",
-                "allowReceivingTasks": "Whiwhi mahi mai i tenei whakaurunga ina waatea nga kaimahi",
+                "allowReceivingTasks": "Whiwhi mahi mai i tenei whakaurunga ina e waatea ana nga kaimahi",
                 "allowSendingTasks": "Tukua nga mahi ki tenei whakaurunga ina e waatea ana nga kaimahi",
                 "authentication": "Motuh\u0113h\u0113nga",
                 "collectiveManagement": "Whakahaere Huihuinga",
                 "connection": "Hononga",
                 "enableChecksumValidation": "Whakamana i nga whakawhitinga konae me nga arowhai (puturi)",
                 "enableConfigMissingLibraries": "Whirihora aunoa i nga whare pukapuka ngaro i runga i te whakaurunga mamao",
                 "enableDistributedWorkerCount": "Whakahohehia te tatau kaimahi toha mo tenei hononga",
-                "enableTaskPreloading": "Utaa mua etahi mahi i runga i te whakaurunga mamao e tatari ana i nga mahi e tatari ana",
+                "enableTaskPreloading": "Uta mua i etahi mahi i runga i te whakaurunga mamao e tatari ana i nga mahi e tatari ana",
                 "linkConfigChecksumValidationStatusLabel": "Whakamanahia me nga arowhai",
                 "linkConfigRemoteLibrariesStatusLabel": "Whirihorahia nga whare pukapuka e ngaro ana",
                 "linkDistributedWorkersStatusLabel": "Nga kaimahi kua tohatohahia",
                 "linkPreloadRemoteTasksStatusLabel": "Uta mua i nga mahi mamao",
                 "linkReceivingTasksStatusLabel": "Te whiwhi mahi",
                 "linkSendingTasksStatusLabel": "Te tuku mahi",
                 "name": "Ingoa",
@@ -149,15 +154,15 @@
                 "enableDebugging": "WhakahoheDebugging",
                 "logs": "Rangitaki",
                 "logsPath": "Ara Rangitaki",
                 "platform": "Papa (P\u016bnaha Whakahaere)",
                 "pythonVersion": "Putanga Python",
                 "support": "Tautoko",
                 "unmanicAppSourceRequests": "Tono te waahanga i roto i te Taup\u0101nga Unmanic",
-                "unmanicFrontendSourceRequests": "Tono tono i roto i te Unmanic Frontend",
+                "unmanicFrontendSourceRequests": "Tono te waahanga i roto i te Unmanic Frontend",
                 "unmanicOfficialPluginRequests": "Tonoa he mono mo Unmanic",
                 "userdataPath": "Ara Raraunga Kaiwhakamahi"
             },
             "workers": {
                 "addEvent": "T\u0101piri Takahanga",
                 "confirmRemove": "Ma te tango i te roopu kaimahi ka tango i nga tautuhinga katoa e hono ana ki te roopu. Kei te tino hiahia koe ki te haere tonu?",
                 "locked": "Kaore e taea te whakakore i te roopu kaimahi",
@@ -189,33 +194,33 @@
         },
         "workers": {
             "currentRunner": {
                 "indeterminate": "Karekau",
                 "none": "Karekau"
             },
             "currentRunnerLabel": "Kaiwhaiwhai o naianei",
-            "listEmpty": "Karekau he kaimahi e whakahaere ana i tenei wa. Whakanuia te tatauranga kaimahi i roto i nga tautuhinga a Unmanic ki te whanau he kaimahi.",
+            "listEmpty": "Karekau he kaimahi e whakahaere ana i tenei wa. Whakanuia te tatauranga kaimahi i roto i nga tautuhinga a Unmanic ki te whakaputa i tetahi kaimahi.",
             "pauseAllWorkers": "Tatari nga kaimahi katoa",
             "pauseWorker": "Tatari tenei kaimahi",
             "resumeAllWorkers": "Whakahokia nga kaimahi katoa",
             "resumeWorker": "Whakahokia tenei kaimahi",
             "startTimeLabel": "W\u0101 T\u012bmata",
             "state": {
-                "paused": "I okioki te kaimahi...",
+                "paused": "Ka okioki te kaimahi...",
                 "processing": "Tukatuka mahi...",
                 "waiting": "E tatari ana mo tetahi atu mahi..."
             },
             "stateLabel": "State",
             "status": "T\u016bnga",
             "terminateAllWorkers": "Whakamutua nga kaimahi katoa",
             "terminateWorker": "Whakamutua tenei kaimahi",
-            "terminateWorkerWarning": "Kei te tino hiahia koe ki te whakamutu i tenei kaimahi me tana mahi o naianei? Ko te mahi o naianei ka tohua i rahua i te rarangi mahi kua oti.",
+            "terminateWorkerWarning": "Kei te tino hiahia koe ki te whakamutu i tenei kaimahi me tana mahi o naianei? Ko te mahi o naianei ka tohua kua rahua i te rarangi mahi kua oti.",
             "totalProcessingTimeLabel": "W\u0101 Tukatuka Tapeke",
-            "workerLog": "Rangi Kaimahi",
-            "workerPaused": "Kua whakataa te kaimahi",
+            "workerLog": "Rangitaki Kaimahi",
+            "workerPaused": "Kua okioki te kaimahi",
             "workerPausedFailed": "Kaore i taea e Unmanic te whakataa tenei kaimahi mo etahi take",
             "workerResumed": "Kua mahi ano te kaimahi",
             "workerResumedFailed": "Kaore i taea e Unmanic te mahi ano i tenei kaimahi mo etahi take",
             "workerTerminated": "Kua whakamutua te kaimahi",
             "workerTerminationFailed": "Kaore i taea e Unmanic te whakamutu i tenei kaimahi mo etahi take"
         }
     },
@@ -229,16 +234,16 @@
         "globalPluginConfig": "Whirihoranga Mono Ao",
         "information": "Nga korero",
         "libraryPluginConfig": "Whirihoranga Mono Whare Pukapuka",
         "librarySettings": "Tautuhinga Whare Pukapuka",
         "listEmpty": "Kei te putua tenei rarangi mahi",
         "login": "Takiuru",
         "pendingTasks": "Nga Mahi Tarewa",
-        "pluginInfo": "Momo Moni",
-        "pluginInstaller": "Kaitautoko mono",
+        "pluginInfo": "Momo Mono",
+        "pluginInstaller": "Kaitautoko Mono",
         "pluginSettings": "Tautuhinga Monomai",
         "privacyPolicy": "Kaupapahere T\u016bmataiti",
         "releaseNotes": "Panui Panui",
         "selectDirectory": "T\u012bpakohia he whaiaronga",
         "selectLibrary": "T\u012bpakohia he whare pukapuka",
         "selectPlugin": "T\u012bpakohia he mono",
         "supportFutureDevelopment": "Tautoko i te whanaketanga a meake nei",
@@ -251,15 +256,15 @@
         "cancel": "Whakakore",
         "close": "Katia",
         "config": "Whirihora",
         "copy": "T\u0101rua",
         "dashboard": "Papatohu",
         "dataPanels": "Paewhiri Raraunga",
         "documentation": "Tuhinga",
-        "helpAndSupport": "Awhina & Tautoko",
+        "helpAndSupport": "\u0100whina & Tautoko",
         "info": "Nga korero",
         "library": "Whare Pukapuka",
         "link": "Hononga",
         "login": "Takiuru",
         "loginWithDiscord": "Takiuru me Discord",
         "loginWithGitHub": "Takiuru me GitHub",
         "loginWithPatreon": "Takiuru me Patreon",
@@ -274,15 +279,15 @@
         "submit": "Tukuna",
         "workers": "Kaimahi",
         "yes": "Ae"
     },
     "notifications": {
         "SavedPluginSettings": "Kua tiakina nga tautuhinga mono.",
         "allowPopups": "Whakaaetia nga pah\u016b-ake mo tenei paetukutuku.",
-        "backendConnectionWarning": "Kaore e taea te hono atu ki te tuara o Unmanic. Tena koa tirohia kei te rere.",
+        "backendConnectionWarning": "Kaore e taea te hono atu ki te tuara o Unmanic. Tirohia koa kei te rere.",
         "cannotRemoveDefaultLibrary": "Kaore e taea te tango i te Puna taunoa",
         "copied": "Kua kapea",
         "failedToFetchEnabledDataPanelPlugins": "I rahua te tiki i te rarangi monomai paewhiri raraunga kua whakahohea",
         "failedToFetchLibraryList": "I rahua te tiki i te rarangi whare pukapuka a Unmanic.",
         "failedToFetchLoginUrl": "I rahua te tiki URL takiuru.",
         "failedToFetchLogoutUrl": "I rahua te tiki URL takiputa.",
         "failedToFetchSettings": "I rahua te tiki i nga tautuhinga on\u0101ianei a Unmanic.",
@@ -292,42 +297,45 @@
         "failedToSaveSettings": "I rahua te tiaki i nga tautuhinga.",
         "incompatibleRemoteInstallation": "Ko te whakaurunga mamao Unmanic e ngana ana koe ki te taapiri kaore i te hototahi ki te hono. Ngana ki te whakahou i te tuatahi.",
         "installed": "Kua whakauruhia.",
         "invalidRemoteInstallationAddress": "Ko te wahitau i whakauruhia e koe ehara i te whakaurunga Unmanic tika.",
         "invalidWorkerEvent": "K\u0101ore e taea te t\u0101piri takahanga kaimahi muhu.",
         "newRepoAddFailed": "I rahua te penapena purongo hou.",
         "remoteInstallationAlreadyInList": "Ko te wahitau i whakauruhia e koe kei te rarangi o nga whakaurunga mamao.",
-        "repoAlreadyExists": "Kei te noho kee te putunga.",
-        "repoRemovedFailed": "I hapa i te wa e ngana ana ki te tango putunga.",
+        "repoAlreadyExists": "Kei te noho tonu te putunga.",
+        "repoRemovedFailed": "I raru tetahi i te wa e ngana ana ki te tango putunga.",
         "repoRemovedSuccess": "I momoho te tango putunga.",
         "reposRefreshFailure": "K\u0101ore e taea te whakah\u014du i \u014d putunga whirihora. Akene he hapa kei tetahi o nga URL?",
         "reposRefreshSuccess": "I momoho te whakahou i nga putunga katoa.",
-        "rescanLibraryError": "I puta he hapa i te wa e tono ana ki te tirotiro ano i te whare pukapuka",
+        "rescanLibraryError": "I puta he hapa i te wa e tono ana mo te tirotiro ano i te whare pukapuka",
         "saved": "Whakaorangia.",
         "serverMessages": {
             "defaults": {
                 "error": "I puta he hapa kore mohiotia i runga i te t\u016bmau",
                 "info": "Karere kore mohiotia mai i te t\u016bmau",
-                "status": "Whakahoutanga mana kore e mohiotia mai i te t\u016bmau",
+                "status": "Whakah\u014du t\u016bnga t\u0113 m\u014dhiotia mai i te t\u016bmau",
                 "success": "Karere kore mohiotia mai i te t\u016bmau",
                 "warning": "whakat\u016bpato t\u0113 m\u014dhiotia mai i te t\u016bmau"
             },
             "incompatiblePlugin": "Kua whakamutua e Unmanic nga mahi mahi na te mea kua kitea he mono hotokore kua whakahohea ki tetahi o o whare pukapuka",
-            "libraryEnabledLimits": "Kua whakamutua e Unmanic nga mahi mahi na te mea he maha rawa nga whare pukapuka kua whirihorahia mo te taumata-kore-tautoko. Whakaarohia te tautoko i te kaupapa kia taea ai te neke atu i te 2 whare pukapuka.",
+            "libraryEnabledLimits": "Kua whakamutua e Unmanic nga mahi mahi na te mea he maha rawa nga whare pukapuka kua whirihorahia mo te taumata-kore-tautoko. Whakaarohia te tautoko i te kaupapa kia kaha ake i te 2 whare pukapuka.",
             "libraryScanProgress": "E rere ana te karapa whare pukapuka",
             "linkedInstallationLimits": "Kua whakamutua e Unmanic nga mahi mahi na te mea kua honoa e koe te maha o nga whakaurunga mamao mo te taumata kore-tautoko. Whakaarohia te tautoko i te kaupapa ki te hono neke atu i te kotahi te whakaurunga mamao.",
             "pendingTaskHaltedPostProcessorQueueFull": "I tae te rarangi Pou-tukatuka ki tona rohe",
             "pendingTaskHaltedPostProcessorQueueFullMessage": "Karekau nga kaimahi e whiwhi mahi hou e tatari ana kia taka ra ano te rarangi Pou-tukatuka ki raro i te tatau kaimahi kua whirihorahia inaianei",
-            "pluginSettingsChangeWorkersStopped": "Kua whakamutua e Unmanic nga kaimahi katoa na te mea kua kitea he huringa ki te whirihoranga mono. Ina reri koe, haere ano nga kaimahi mai i te papatohu.",
+            "pluginSettingsChangeWorkersStopped": "Kua whakamutua e Unmanic nga kaimahi katoa na te mea kua kitea he huringa ki te whirihoranga mono. Kia reri koe, whakaara ano i nga kaimahi mai i te papatohu.",
             "receivingRemoteFile": "Te whiwhi k\u014dnae mamao"
+        },
+        "serverNotificationLabels": {
+            "failedTaskLabel": "Rahunga Mahi"
         }
     },
     "status": {
         "all": "Katoa",
-        "cannotLoadImage": "K\u0101ore e taea te uta atahanga",
+        "cannotLoadImage": "Kaore e taea te uta atahanga",
         "disabled": "Kua haua",
         "enabled": "Whakahohe",
         "failed": "I rahua",
         "none": "Karekau",
         "success": "Angitu"
     },
     "tooltips": {
@@ -338,15 +346,15 @@
         "configure": "Whirihora",
         "configureForThisLibrary": "Whirihorahia mo tenei whare pukapuka",
         "defaultLibrary": "Koinei te whare pukapuka taunoa. Kaore e taea te muku.",
         "delete": "Mukua",
         "etc": "W\u0101 Whakatau mo te Whakaoti",
         "install": "T\u0101uta",
         "move": "Nuku",
-        "pluginInfo": "Momo Moni",
+        "pluginInfo": "Momo Mono",
         "position": "Turanga",
         "reinstall": "T\u0101uta an\u014d",
         "remove": "Tango",
         "removeFromThisLibrary": "Tangohia mai i tenei whare pukapuka",
         "unavailable": "K\u0101ore i te w\u0101tea",
         "update": "Whakahou"
     }
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/language/fr.json` & `unmanic-0.2.4/unmanic/webserver/frontend/src/language/fr.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9725029322073656%*

 * *Differences: {"'buttons'": "{'dismissAll': 'Rejeter la totalité'}",*

 * * "'components'": "{'plugins': {'installPluginFromRepo': 'Installer le plugin à partir du "*

 * *                 "référentiel', 'installPluginFromFile': 'Installer le plugin à partir du "*

 * *                 'fichier\', \'invalidZipFile\': "Le fichier n\'est pas un fichier ZIP valide", '*

 * *                 '\'failedToInstallPluginFromZip\': "Échec de l\'installation du plug-in à partir '*

 * *                 'du fichier ZIP téléchargé", \'installedPluginFromZip\': \' […]*

```diff
@@ -1,10 +1,11 @@
 {
     "buttons": {
         "darkMode": "Mode sombre",
+        "dismissAll": "Rejeter la totalit\u00e9",
         "language": "Langue"
     },
     "components": {
         "completedTasks": {
             "addToPendingTasksList": "Ajouter la s\u00e9lection \u00e0 la liste des t\u00e2ches en attente",
             "before": "Avant de",
             "details": "D\u00e9tails",
@@ -27,16 +28,20 @@
         },
         "plugins": {
             "addRepository": "Ajouter un r\u00e9f\u00e9rentiel",
             "author": "Auteur",
             "categoryFilter": "Filtre de cat\u00e9gorie",
             "clickToUpdatePlugin": "Cliquez pour mettre \u00e0 jour le plugin",
             "errorSavingFlow": "Une erreur s'est produite lors de l'enregistrement du flux de plug-in",
+            "failedToInstallPluginFromZip": "\u00c9chec de l'installation du plug-in \u00e0 partir du fichier ZIP t\u00e9l\u00e9charg\u00e9",
             "globalConfiguration": "Configuration globale",
-            "installPlugins": "Installer le plugin",
+            "installPluginFromFile": "Installer le plugin \u00e0 partir du fichier",
+            "installPluginFromRepo": "Installer le plugin \u00e0 partir du r\u00e9f\u00e9rentiel",
+            "installedPluginFromZip": "Plugin install\u00e9",
+            "invalidZipFile": "Le fichier n'est pas un fichier ZIP valide",
             "newRepository": "Nouveau r\u00e9f\u00e9rentiel",
             "pluginUpToDate": "Le plugin est \u00e0 jour",
             "refreshRepositories": "Actualiser les r\u00e9f\u00e9rentiels",
             "removePlugin": "Supprimer le plug-in",
             "repo": "D\u00e9p\u00f4t",
             "repoList": "Liste des r\u00e9f\u00e9rentiels",
             "repoName": "Nom",
@@ -315,14 +320,17 @@
             "libraryEnabledLimits": "Unmanic a arr\u00eat\u00e9 de traiter les t\u00e2ches car vous avez trop de biblioth\u00e8ques configur\u00e9es pour un niveau non supporteur. Envisagez de parrainer le projet pour permettre \u00e0 plus de 2 biblioth\u00e8ques.",
             "libraryScanProgress": "Analyse de la biblioth\u00e8que en cours d'ex\u00e9cution",
             "linkedInstallationLimits": "Unmanic a arr\u00eat\u00e9 de traiter les t\u00e2ches car vous avez li\u00e9 trop d'installations \u00e0 distance pour un niveau non supporteur. Envisagez de parrainer le projet pour relier plus d'une installation \u00e0 distance.",
             "pendingTaskHaltedPostProcessorQueueFull": "La file d'attente du post-processeur a atteint sa limite",
             "pendingTaskHaltedPostProcessorQueueFullMessage": "Les travailleurs ne recevront pas de nouvelle t\u00e2che en attente tant que la file d'attente du post-processeur ne sera pas inf\u00e9rieure au nombre de travailleurs actuellement configur\u00e9",
             "pluginSettingsChangeWorkersStopped": "Unmanic a arr\u00eat\u00e9 tous les travailleurs car il a d\u00e9tect\u00e9 un changement dans la configuration des plugins. Lorsque vous \u00eates pr\u00eat, reprenez les ouvriers depuis le tableau de bord.",
             "receivingRemoteFile": "R\u00e9ception de fichier distant"
+        },
+        "serverNotificationLabels": {
+            "failedTaskLabel": "\u00c9chec de la t\u00e2che"
         }
     },
     "status": {
         "all": "Tout",
         "cannotLoadImage": "Impossible de charger l'image",
         "disabled": "Handicap\u00e9",
         "enabled": "Activ\u00e9",
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/language/en.json` & `unmanic-0.2.4/unmanic/webserver/frontend/src/language/en.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9725029322073656%*

 * *Differences: {"'buttons'": "{'dismissAll': 'Dismiss All'}",*

 * * "'components'": "{'plugins': {'installPluginFromRepo': 'Install Plugin From Repo', "*

 * *                 "'installPluginFromFile': 'Install Plugin From File', 'invalidZipFile': 'File is "*

 * *                 "not a valid ZIP file', 'failedToInstallPluginFromZip': 'Failed to install plugin "*

 * *                 "from the uploaded ZIP file', 'installedPluginFromZip': 'Plugin installed', "*

 * *                 "delete: ['installPlugins']}}",*

 * * "'notifications'": "{'serverNotif […]*

```diff
@@ -1,10 +1,11 @@
 {
     "buttons": {
         "darkMode": "Dark Mode",
+        "dismissAll": "Dismiss All",
         "language": "Language"
     },
     "components": {
         "completedTasks": {
             "addToPendingTasksList": "Add selected to Pending Tasks list",
             "before": "Before",
             "details": "Details",
@@ -27,16 +28,20 @@
         },
         "plugins": {
             "addRepository": "Add Repository",
             "author": "Author",
             "categoryFilter": "Category Filter",
             "clickToUpdatePlugin": "Click to update plugin",
             "errorSavingFlow": "An error was encountered while saving the Plugin Flow",
+            "failedToInstallPluginFromZip": "Failed to install plugin from the uploaded ZIP file",
             "globalConfiguration": "Global Configuration",
-            "installPlugins": "Install Plugin",
+            "installPluginFromFile": "Install Plugin From File",
+            "installPluginFromRepo": "Install Plugin From Repo",
+            "installedPluginFromZip": "Plugin installed",
+            "invalidZipFile": "File is not a valid ZIP file",
             "newRepository": "New Repository",
             "pluginUpToDate": "Plugin is up-to-date",
             "refreshRepositories": "Refresh Repositories",
             "removePlugin": "Remove Plugin",
             "repo": "Repository",
             "repoList": "Repository List",
             "repoName": "Name",
@@ -315,14 +320,17 @@
             "libraryEnabledLimits": "Unmanic has stopped processing tasks as you have too many libraries configured for a non-supporter tier. Consider sponsoring the project to enable more than 2 libraries.",
             "libraryScanProgress": "Library scan running",
             "linkedInstallationLimits": "Unmanic has stopped processing tasks as you have linked too many remote installations for a non-supporter tier. Consider sponsoring the project to link more than one remote installation.",
             "pendingTaskHaltedPostProcessorQueueFull": "The Post-processor queue reached its limit",
             "pendingTaskHaltedPostProcessorQueueFullMessage": "Workers will not receive a new pending task until the Post-processor queue drops below the current configured worker count",
             "pluginSettingsChangeWorkersStopped": "Unmanic has stopped all workers as it has detected a change to the plugins configuration. When you are ready, resume the workers from the dashboard.",
             "receivingRemoteFile": "Receiving remote file"
+        },
+        "serverNotificationLabels": {
+            "failedTaskLabel": "Task Failure"
         }
     },
     "status": {
         "all": "All",
         "cannotLoadImage": "Cannot load image",
         "disabled": "Disabled",
         "enabled": "Enabled",
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/language/es.json` & `unmanic-0.2.4/unmanic/webserver/frontend/src/language/es.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9724971866659058%*

 * *Differences: {"'buttons'": "{'dismissAll': 'Descartar todo'}",*

 * * "'components'": "{'settings': {'library': {'enableReceiveRemoteFilesOnly': 'Configurar la "*

 * *                 "biblioteca para recibir archivos remotos únicamente'}}, 'plugins': "*

 * *                 "{'installPluginFromRepo': 'Instalar complemento desde repositorio', "*

 * *                 "'installPluginFromFile': 'Instalar complemento desde archivo', 'invalidZipFile': "*

 * *                 "'El archivo no es un archivo ZIP válido', 'failedToInstallPluginFromZip': ' […]*

```diff
@@ -1,10 +1,11 @@
 {
     "buttons": {
         "darkMode": "Modo oscuro",
+        "dismissAll": "Descartar todo",
         "language": "Idioma"
     },
     "components": {
         "completedTasks": {
             "addToPendingTasksList": "Agregar seleccionado a la lista de tareas pendientes",
             "before": "Antes",
             "details": "Detalles",
@@ -27,16 +28,20 @@
         },
         "plugins": {
             "addRepository": "Agregar repositorio",
             "author": "Autor",
             "categoryFilter": "Filtro de categor\u00eda",
             "clickToUpdatePlugin": "Haga clic para actualizar el complemento",
             "errorSavingFlow": "Se encontr\u00f3 un error al guardar el flujo del complemento",
+            "failedToInstallPluginFromZip": "No se pudo instalar el complemento desde el archivo ZIP cargado",
             "globalConfiguration": "configuraci\u00f3n global",
-            "installPlugins": "Instalar complemento",
+            "installPluginFromFile": "Instalar complemento desde archivo",
+            "installPluginFromRepo": "Instalar complemento desde repositorio",
+            "installedPluginFromZip": "Complemento instalado",
+            "invalidZipFile": "El archivo no es un archivo ZIP v\u00e1lido",
             "newRepository": "Nuevo repositorio",
             "pluginUpToDate": "El complemento est\u00e1 actualizado",
             "refreshRepositories": "Actualizar repositorios",
             "removePlugin": "Eliminar complemento",
             "repo": "Repositorio",
             "repoList": "Lista de repositorios",
             "repoName": "Nombre",
@@ -75,15 +80,15 @@
                 "cloneLibrary": "Biblioteca de clones",
                 "completedTasks": "tareas completadas",
                 "concurrentFileTesters": "Comprobadores de archivos simult\u00e1neos",
                 "confirmRemove": "Al eliminar la biblioteca, tambi\u00e9n se eliminar\u00e1n todas las configuraciones asociadas con esta biblioteca. \u00bfSeguro que desea continuar?",
                 "defaultLibrary": "Biblioteca predeterminada",
                 "enableInotify": "Habilitar el monitor de archivos para esta biblioteca",
                 "enableLibraryScanner": "Habilitar escaneos peri\u00f3dicos de la biblioteca",
-                "enableReceiveRemoteFilesOnly": "Configurar la biblioteca para recibir solo archivos remotos",
+                "enableReceiveRemoteFilesOnly": "Configurar la biblioteca para recibir archivos remotos \u00fanicamente",
                 "enableScanner": "Habilitar esc\u00e1ner de biblioteca para esta biblioteca",
                 "exportLibraryConfig": "Exportar configuraci\u00f3n",
                 "fileTesting": "Prueba de archivos",
                 "followSymlinks": "Siga los enlaces simb\u00f3licos en los escaneos de la biblioteca",
                 "importLibraryConfig": "Importar configuraci\u00f3n",
                 "importPluginConfigMessage": "Importaci\u00f3n de la configuraci\u00f3n de la biblioteca. Esto puede llevar alg\u00fan tiempo si hay alg\u00fan complemento que requiera instalaci\u00f3n.",
                 "libraryFileMonitorStatusLabel": "supervisor de archivos",
@@ -315,14 +320,17 @@
             "libraryEnabledLimits": "Unmanic ha dejado de procesar tareas porque tiene demasiadas bibliotecas configuradas para un nivel que no es de soporte. Considere patrocinar el proyecto para habilitar m\u00e1s de 2 bibliotecas.",
             "libraryScanProgress": "Exploraci\u00f3n de biblioteca en ejecuci\u00f3n",
             "linkedInstallationLimits": "Unmanic ha dejado de procesar tareas porque ha vinculado demasiadas instalaciones remotas para un nivel que no es de soporte. Considere patrocinar el proyecto para vincular m\u00e1s de una instalaci\u00f3n remota.",
             "pendingTaskHaltedPostProcessorQueueFull": "La cola del posprocesador alcanz\u00f3 su l\u00edmite",
             "pendingTaskHaltedPostProcessorQueueFullMessage": "Los trabajadores no recibir\u00e1n una nueva tarea pendiente hasta que la cola del posprocesador caiga por debajo del recuento de trabajadores configurado actualmente.",
             "pluginSettingsChangeWorkersStopped": "Unmanic ha detenido a todos los trabajadores ya que ha detectado un cambio en la configuraci\u00f3n de los complementos. Cuando est\u00e9 listo, reanude a los trabajadores desde el tablero.",
             "receivingRemoteFile": "Recibir archivo remoto"
+        },
+        "serverNotificationLabels": {
+            "failedTaskLabel": "Error de tarea"
         }
     },
     "status": {
         "all": "Todos",
         "cannotLoadImage": "No se puede cargar la imagen",
         "disabled": "Desactivado",
         "enabled": "Activado",
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/language/sv.json` & `unmanic-0.2.4/unmanic/webserver/frontend/src/language/sv.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9658636397908918%*

 * *Differences: {"'buttons'": "{'dismissAll': 'Avfärda alla'}",*

 * * "'components'": "{'settings': {'link': {'allowReceivingTasks': 'Ta emot uppgifter från den här "*

 * *                 "installationen när arbetare är tillgängliga', 'enableDistributedWorkerCount': "*

 * *                 "'Aktivera distribuerat antal arbetare för den här länken'}}, 'completedTasks': "*

 * *                 "{'addToPendingTasksList': 'Lägg till valda i listan över väntande uppgifter'}, "*

 * *                 "'plugins': {'addRepository': 'Lägg till arkiv', 'ins […]*

```diff
@@ -1,15 +1,16 @@
 {
     "buttons": {
         "darkMode": "M\u00f6rkt l\u00e4ge",
+        "dismissAll": "Avf\u00e4rda alla",
         "language": "Spr\u00e5k"
     },
     "components": {
         "completedTasks": {
-            "addToPendingTasksList": "L\u00e4gg till markerade i listan \u00f6ver v\u00e4ntande uppgifter",
+            "addToPendingTasksList": "L\u00e4gg till valda i listan \u00f6ver v\u00e4ntande uppgifter",
             "before": "Innan",
             "details": "Detaljer",
             "errorGettingDetails": "Ett fel p\u00e5tr\u00e4ffades n\u00e4r detaljerna f\u00f6r denna uppgift skulle h\u00e4mtas",
             "removeSelected": "Ta bort markerade fr\u00e5n listan",
             "selectLibraryToAdd": "V\u00e4lj bibliotek d\u00e4r du vill \u00e5terskapa denna uppgift",
             "since": "Eftersom"
         },
@@ -22,21 +23,25 @@
         "pendingTasks": {
             "moveToBottom": "Flytta markerade till botten",
             "moveToTop": "Flytta markerade till toppen",
             "removeSelected": "Ta bort markerade fr\u00e5n listan",
             "rescanLibrary": "Skanna biblioteket igen nu"
         },
         "plugins": {
-            "addRepository": "L\u00e4gg till f\u00f6rr\u00e5d",
+            "addRepository": "L\u00e4gg till arkiv",
             "author": "F\u00f6rfattare",
             "categoryFilter": "Kategorifilter",
             "clickToUpdatePlugin": "Klicka f\u00f6r att uppdatera plugin",
             "errorSavingFlow": "Ett fel p\u00e5tr\u00e4ffades n\u00e4r pluginfl\u00f6det skulle sparas",
+            "failedToInstallPluginFromZip": "Det gick inte att installera plugin fr\u00e5n den uppladdade ZIP-filen",
             "globalConfiguration": "Global konfiguration",
-            "installPlugins": "Installera plugin",
+            "installPluginFromFile": "Installera plugin fr\u00e5n fil",
+            "installPluginFromRepo": "Installera plugin fr\u00e5n Repo",
+            "installedPluginFromZip": "Plugin installerad",
+            "invalidZipFile": "Filen \u00e4r inte en giltig ZIP-fil",
             "newRepository": "Nytt f\u00f6rr\u00e5d",
             "pluginUpToDate": "Plugin \u00e4r uppdaterad",
             "refreshRepositories": "Uppdatera f\u00f6rr\u00e5d",
             "removePlugin": "Ta bort plugin",
             "repo": "F\u00f6rvar",
             "repoList": "F\u00f6rvarslista",
             "repoName": "namn",
@@ -106,22 +111,22 @@
                 "runLibraryScanOnStart": "K\u00f6r en biblioteksskanning en g\u00e5ng vid start",
                 "unlocked": "Biblioteket kan raderas"
             },
             "link": {
                 "add": "L\u00e4gg till",
                 "addRemoteInstallation": "L\u00e4gg till fj\u00e4rrinstallation",
                 "address": "Adress",
-                "allowReceivingTasks": "Ta emot uppgifter fr\u00e5n denna installation n\u00e4r arbetare \u00e4r tillg\u00e4ngliga",
+                "allowReceivingTasks": "Ta emot uppgifter fr\u00e5n den h\u00e4r installationen n\u00e4r arbetare \u00e4r tillg\u00e4ngliga",
                 "allowSendingTasks": "Skicka uppgifter till den h\u00e4r installationen n\u00e4r arbetare \u00e4r tillg\u00e4ngliga",
                 "authentication": "Autentisering",
                 "collectiveManagement": "Kollektiv f\u00f6rvaltning",
                 "connection": "F\u00f6rbindelse",
                 "enableChecksumValidation": "Validera fil\u00f6verf\u00f6ringar med kontrollsummor (l\u00e5ngsamma)",
                 "enableConfigMissingLibraries": "Konfigurera saknade bibliotek automatiskt p\u00e5 fj\u00e4rrinstallationen",
-                "enableDistributedWorkerCount": "Aktivera distribuerat antal arbetare f\u00f6r denna l\u00e4nk",
+                "enableDistributedWorkerCount": "Aktivera distribuerat antal arbetare f\u00f6r den h\u00e4r l\u00e4nken",
                 "enableTaskPreloading": "F\u00f6rladda vissa uppgifter p\u00e5 fj\u00e4rrinstallationens k\u00f6n f\u00f6r v\u00e4ntande uppgifter",
                 "linkConfigChecksumValidationStatusLabel": "Validera med kontrollsummor",
                 "linkConfigRemoteLibrariesStatusLabel": "Konfigurera saknade bibliotek",
                 "linkDistributedWorkersStatusLabel": "Distribuerade arbetare",
                 "linkPreloadRemoteTasksStatusLabel": "F\u00f6rladda fj\u00e4rruppgifter",
                 "linkReceivingTasksStatusLabel": "Ta emot uppgifter",
                 "linkSendingTasksStatusLabel": "Skickar uppgifter",
@@ -280,32 +285,32 @@
         "allowPopups": "Till\u00e5t popup-f\u00f6nster f\u00f6r denna webbplats.",
         "backendConnectionWarning": "Det g\u00e5r inte att ansluta till Unmanic backend. Kontrollera att den \u00e4r ig\u00e5ng.",
         "cannotRemoveDefaultLibrary": "Det g\u00e5r inte att ta bort standardbiblioteket",
         "copied": "Kopierade",
         "failedToFetchEnabledDataPanelPlugins": "Det gick inte att h\u00e4mta listan \u00f6ver aktiverade datapanelpluginprogram",
         "failedToFetchLibraryList": "Det gick inte att h\u00e4mta Unmanics bibliotekslista.",
         "failedToFetchLoginUrl": "Det gick inte att h\u00e4mta inloggnings-URL.",
-        "failedToFetchLogoutUrl": "Det gick inte att h\u00e4mta webbadressen f\u00f6r utloggning.",
+        "failedToFetchLogoutUrl": "Det gick inte att h\u00e4mta utloggningsadressen.",
         "failedToFetchSettings": "Det gick inte att h\u00e4mta Unmanics nuvarande inst\u00e4llningar.",
         "failedToFetchSystemConfig": "Det gick inte att h\u00e4mta Unmanics systemkonfiguration.",
         "failedToInstallPlugin": "Ett fel p\u00e5tr\u00e4ffades vid f\u00f6rs\u00f6k att installera det beg\u00e4rda pluginprogrammet.",
-        "failedToSavePluginSettings": "Det gick inte att spara plugin-inst\u00e4llningarna.",
+        "failedToSavePluginSettings": "Det gick inte att spara plugininst\u00e4llningarna.",
         "failedToSaveSettings": "Det gick inte att spara inst\u00e4llningarna.",
         "incompatibleRemoteInstallation": "Fj\u00e4rrinstallationen av Unmanic som du f\u00f6rs\u00f6ker l\u00e4gga till \u00e4r inte kompatibel med l\u00e4nkning. F\u00f6rs\u00f6k att uppdatera den f\u00f6rst.",
         "installed": "Installerad.",
         "invalidRemoteInstallationAddress": "Adressen du angav var inte en giltig Unmanic-installation.",
         "invalidWorkerEvent": "Det gick inte att l\u00e4gga till ogiltig arbetsh\u00e4ndelse.",
         "newRepoAddFailed": "Det gick inte att spara det nya arkivet.",
         "remoteInstallationAlreadyInList": "Adressen du angav finns redan i listan \u00f6ver fj\u00e4rrinstallationer.",
         "repoAlreadyExists": "Lagret finns redan.",
         "repoRemovedFailed": "N\u00e5got gick fel n\u00e4r arkivet skulle tas bort.",
         "repoRemovedSuccess": "Repository har tagits bort.",
-        "reposRefreshFailure": "Det g\u00e5r inte att uppdatera dina konfigurerade arkiv. Kanske \u00e4r det ett fel i en av webbadresserna?",
-        "reposRefreshSuccess": "Alla arkiv har uppdaterats.",
-        "rescanLibraryError": "Ett fel p\u00e5tr\u00e4ffades vid beg\u00e4ran om en oms\u00f6kning av biblioteket",
+        "reposRefreshFailure": "Det g\u00e5r inte att uppdatera dina konfigurerade f\u00f6rr\u00e5d. Kanske \u00e4r det ett fel i en av webbadresserna?",
+        "reposRefreshSuccess": "Uppdaterade alla arkiv.",
+        "rescanLibraryError": "Ett fel p\u00e5tr\u00e4ffades n\u00e4r en oms\u00f6kning av biblioteket beg\u00e4rdes",
         "saved": "Sparad.",
         "serverMessages": {
             "defaults": {
                 "error": "Ok\u00e4nt fel uppstod p\u00e5 servern",
                 "info": "Ok\u00e4nt meddelande fr\u00e5n servern",
                 "status": "Ok\u00e4nd statusuppdatering fr\u00e5n servern",
                 "success": "Ok\u00e4nt meddelande fr\u00e5n servern",
@@ -315,14 +320,17 @@
             "libraryEnabledLimits": "Unmanic har slutat bearbeta uppgifter eftersom du har f\u00f6r m\u00e5nga bibliotek konfigurerade f\u00f6r en icke-supporterniv\u00e5. \u00d6verv\u00e4g att sponsra projektet f\u00f6r att m\u00f6jligg\u00f6ra fler \u00e4n 2 bibliotek.",
             "libraryScanProgress": "Bibliotekss\u00f6kning k\u00f6rs",
             "linkedInstallationLimits": "Unmanic har slutat bearbeta uppgifter eftersom du har l\u00e4nkat f\u00f6r m\u00e5nga fj\u00e4rrinstallationer f\u00f6r en icke-supporterniv\u00e5. \u00d6verv\u00e4g att sponsra projektet f\u00f6r att l\u00e4nka mer \u00e4n en fj\u00e4rrinstallation.",
             "pendingTaskHaltedPostProcessorQueueFull": "Efterbehandlingsk\u00f6n n\u00e5dde sin gr\u00e4ns",
             "pendingTaskHaltedPostProcessorQueueFullMessage": "Arbetare kommer inte att f\u00e5 en ny v\u00e4ntande uppgift f\u00f6rr\u00e4n efterbehandlark\u00f6n sjunker under det nuvarande konfigurerade antalet arbetare",
             "pluginSettingsChangeWorkersStopped": "Unmanic har stoppat alla arbetare eftersom de har uppt\u00e4ckt en \u00e4ndring av plugins-konfigurationen. N\u00e4r du \u00e4r redo, \u00e5teruppta arbetarna fr\u00e5n instrumentpanelen.",
             "receivingRemoteFile": "Tar emot fj\u00e4rrfil"
+        },
+        "serverNotificationLabels": {
+            "failedTaskLabel": "Uppgift misslyckande"
         }
     },
     "status": {
         "all": "Allt",
         "cannotLoadImage": "Det g\u00e5r inte att ladda bilden",
         "disabled": "Inaktiverad",
         "enabled": "Aktiverad",
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/MarkdownDialog.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/MarkdownDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/PendingTasks.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/PendingTasks.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/PluginInstallerManageRepos.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/PluginInstallerManageRepos.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/WorkerEventCreateDialog.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/WorkerEventCreateDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/DrawerDataPanelsNav.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/DrawerDataPanelsNav.vue`

 * *Files 11% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 
 
     </q-list>
   </q-scroll-area>
 
   <q-img
     v-if="$q.platform.is.mobile"
-    class="absolute-top bg-primary"
+    class="absolute-top header-background"
     style="height: 90px;">
-    <div class="absolute-center bg-primary">
+    <div class="absolute-center header-background">
       <q-avatar
         rounded
         clickable
         @click="$router.push('/ui/dashboard')"
         size="56px" class="q-mb-sm cursor-pointer">
         <q-img src="~assets/unmanic-logo-white.png"/>
       </q-avatar>
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/LanguageSwitch.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/LanguageSwitch.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/WorkerProgress.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/WorkerProgress.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/Avatar.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/Avatar.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/PluginsInstalledTable.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/PluginsInstalledTable.vue`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,44 @@
 <template>
 
 
   <q-card flat>
     <q-card-section :class="$q.platform.is.mobile ? 'q-px-none' : ''">
       <div class="row q-gutter-xs q-mt-xs justify-between">
         <div class="col-auto">
-          <q-btn
-            @click="openPluginInstaller"
-            class=""
-            color="secondary"
-            icon-right="add"
-            :label="$t('components.plugins.installPlugins')"/>
+          <q-btn-group>
+            <q-btn
+              @click="openPluginInstaller"
+              class=""
+              color="secondary"
+              icon-right="add"
+              :label="$t('components.plugins.installPluginFromRepo')"/>
+
+            <q-btn-dropdown
+              color="secondary"
+              :label="$t('components.plugins.installPluginFromFile')">
+              <div>
+                <div class="row no-wrap q-pa-md">
+                  <div class="column">
+                    <q-uploader
+                      style="max-width: 300px"
+                      :url="getUploadUrl()"
+                      label="Upload ZIP file..."
+                      color="secondary"
+                      accept=".zip, application/zip"
+                      auto-upload
+                      @rejected="onRejectedPluginUpload"
+                      @failed="onFailedPluginUploadAndInstall"
+                      @uploaded="onSuccessfulPluginUploadAndInstall"
+                    />
+                  </div>
+                </div>
+              </div>
+            </q-btn-dropdown>
+          </q-btn-group>
         </div>
         <div class="col-auto" style="max-width: 200px">
           <q-input
             filled dense
             class="shadow-1"
             debounce="300"
             color="primary"
@@ -206,33 +230,31 @@
           </q-item>
 
         </q-list>
       </div>
     </q-card-section>
   </q-card>
 
-  <PluginInfo v-bind:showPluginInfo="showPluginInfo"
-              v-bind:showPluginSettings="showPluginSettings"
-              v-on:hide="closePluginInfo"/>
-
 </template>
 
 <script>
 import { onMounted, watch, ref } from 'vue';
 import { getUnmanicApiUrl } from "src/js/unmanicGlobals";
 import { useQuasar } from "quasar";
 import axios from "axios";
-import PluginInfo from "components/PluginInfo";
 import { bbCodeToHTML } from "src/js/markupParser";
-import PluginInstallerDialog from "components/PluginInstallerDialog";
+import { useI18n } from "vue-i18n";
+import PluginInfoDialog from "components/dialogs/PluginInfoDialog";
+import ConfigDrawerDialog from "components/dialogs/ConfigDrawerDialog";
 
 export default {
-  components: { PluginInfo },
+  components: {},
   setup() {
     const $q = useQuasar();
+    const { t: $t } = useI18n();
     const rows = ref([]);
     const filter = ref('');
     const loading = ref(false);
     const pagination = ref({
       sortBy: 'name',
       descending: false,
       page: 1,
@@ -448,48 +470,112 @@
         })
       })
     }
 
     const showPluginInfo = ref('');
     const showPluginSettings = ref('');
 
-    function openPluginInfo(table_id, tab) {
-      showPluginInfo.value = '';
-      showPluginSettings.value = '';
+    function openPluginInfo(tableId, tab) {
+      // Fetch the details of the plugin info to be shown
+      let pluginId = '';
       for (let i = 0; i < listedPlugins.value.length; i++) {
         let plugin = listedPlugins.value[i];
-        if (plugin.id === table_id) {
-          if (tab === 'settings') {
-            showPluginSettings.value = plugin.plugin_id;
-          } else {
-            showPluginInfo.value = plugin.plugin_id;
-          }
+        if (plugin.id === tableId) {
+          pluginId = plugin.plugin_id;
         }
       }
+      // Ensure we have the info for the plugin to be displayed
+      if (pluginId === '') {
+        // Display error notification
+        $q.notify({
+          color: 'negative',
+          position: 'top',
+          message: 'An error was encountered while attempting to open plugin info',
+          icon: 'report_problem',
+          actions: [{ icon: 'close', color: 'white' }]
+        })
+        return
+      }
+      // Display the dialog
+      $q.dialog({
+        component: PluginInfoDialog,
+        componentProps: {
+          pluginId: pluginId,
+          startTab: (tab === 'settings') ? 'settings' : 'info',
+        },
+      }).onOk((payload) => {
+      }).onDismiss(() => {
+      })
     }
 
     function closePluginInfo() {
       showPluginInfo.value = '';
       showPluginSettings.value = '';
     }
 
     function openPluginInstaller() {
       $q.dialog({
-        component: PluginInstallerDialog,
-        // props forwarded to your custom component
-        componentProps: {},
+        component: ConfigDrawerDialog,
+        componentProps: {
+          header: $t('headers.pluginInstaller'),
+          componentName: "PluginInstallerForm",
+          width: "2000px",
+          componentProps: {},
+        },
       }).onOk((payload) => {
       }).onDismiss(() => {
         onRequest({
           pagination: pagination.value,
           filter: filter.value
         })
       })
     }
 
+    function getUploadUrl() {
+      return getUnmanicApiUrl('v2', 'upload/plugin/file')
+    }
+
+    function onRejectedPluginUpload(rejectedEntries) {
+      $q.notify({
+        color: 'negative',
+        position: 'top',
+        message: $t('components.plugins.invalidZipFile'),
+        icon: 'report_problem',
+        actions: [{ icon: 'close', color: 'white' }]
+      })
+    }
+
+    function onFailedPluginUploadAndInstall() {
+      $q.notify({
+        color: 'negative',
+        position: 'top',
+        message: $t('components.plugins.failedToInstallPluginFromZip'),
+        icon: 'check_circle',
+        actions: [{ icon: 'close', color: 'white' }]
+      })
+      onRequest({
+        pagination: pagination.value,
+        filter: undefined
+      })
+    }
+
+    function onSuccessfulPluginUploadAndInstall() {
+      $q.notify({
+        color: 'positive',
+        position: 'top',
+        message: $t('components.plugins.installedPluginFromZip'),
+        icon: 'check_circle',
+        actions: [{ icon: 'close', color: 'white' }]
+      })
+      onRequest({
+        pagination: pagination.value,
+        filter: undefined
+      })
+    }
+
     onMounted(() => {
       // get initial data from server (1st page)
       onRequest({
         pagination: pagination.value,
         filter: undefined
       })
     })
@@ -516,15 +602,19 @@
       disableSelected,
       updateSinglePlugin,
       removeSinglePlugin,
       openPluginInfo,
       showPluginInfo,
       showPluginSettings,
       closePluginInfo,
-      openPluginInstaller
+      openPluginInstaller,
+      getUploadUrl,
+      onRejectedPluginUpload,
+      onFailedPluginUploadAndInstall,
+      onSuccessfulPluginUploadAndInstall
     }
   }
 }
 </script>
 <style>
 .plugin-list-icon {
   display: block;
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/ReleaseNotesDialog.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/ReleaseNotesDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/PluginInstallerDialog.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/forms/PluginInstallerForm.vue`

 * *Files 13% similar despite different names*

```diff
@@ -1,373 +1,318 @@
 <template>
 
-  <!-- START DIALOG CONFIG
-  Right fullscreen pop-up
-  Note: Update template q-dialog ref="" value
-
-  All Platforms:
-   - Swipe right to dismiss
-  Desktop:
-   - Width 2000px
-   - Minimise button top-right
-  Mobile:
-   - Full screen
-   - Back button top-left
-  -->
-  <q-dialog
-    ref="dialogRef"
-    :maximized="$q.platform.is.mobile"
-    :transition-show="$q.platform.is.mobile ? 'jump-left' : 'slide-left'"
-    :transition-hide="$q.platform.is.mobile ? 'jump-right' : 'slide-right'"
-    full-height
-    position="right"
-    @hide="onDialogHide">
-
-    <q-card
-      v-touch-swipe.touch.left="hide"
-      :style="$q.platform.is.mobile ? 'max-width: 100vw;' : 'max-width: 95vw;'"
-      style="width:2000px;">
-
-      <q-card-section class="bg-card-head">
-        <div class="row items-center no-wrap">
-          <div
-            v-if="$q.platform.is.mobile"
-            class="col">
-            <q-btn
-              color="grey-7"
-              dense
-              round
-              flat
-              icon="arrow_back"
-              v-close-popup>
-            </q-btn>
-          </div>
-
-          <div class="col">
-            <div class="text-h6 text-blue-10">
-              {{ $t('headers.pluginInstaller') }}
-            </div>
-          </div>
-
-          <div
-            v-if="!$q.platform.is.mobile"
-            class="col-auto">
-            <q-btn
-              color="grey-7"
-              dense
-              round
-              flat
-              icon="arrow_forward"
-              v-close-popup>
-              <q-tooltip class="bg-white text-primary">{{ $t('tooltips.close') }}</q-tooltip>
-            </q-btn>
-          </div>
+  <div class="row q-col-gutter-none q-ma-none plugin-table-actions-bar">
+    <div class="col self-start">
+      <div class="row q-col-gutter-xs q-ma-xs">
+        <div
+          v-if="$q.platform.is.mobile"
+          class="col-auto">
+          <PluginInstallerManageRepos/>
         </div>
-      </q-card-section>
-      <!-- END DIALOG CONFIG -->
-
-      <q-card-section class="q-pa-none">
-        <div class="q-pa-md">
-
-          <q-table
-            grid
-            card-class="bg-primary text-white"
-            :rows="rows"
-            :columns="columns"
-            row-key="name"
-            :filter="filter"
-            hide-header
-            v-model:pagination="pagination"
-            hide-pagination
-          >
-            <template v-slot:top-left>
-              <div class="row q-col-gutter-xs q-ma-xs">
-                <div
-                  v-if="$q.platform.is.mobile"
-                  class="col-auto">
-                  <PluginInstallerManageRepos/>
-                </div>
-                <div class="col-auto">
-                  <q-input
-                    filled
-                    class="shadow-1"
-                    dense
-                    debounce="300"
-                    v-model="filter"
-                    :placeholder="$t('navigation.search')">
-                    <template v-slot:append>
-                      <q-icon name="search"/>
-                    </template>
-                  </q-input>
-                </div>
-                <div class="col-auto">
-                  <q-select
-                    filled
-                    class="shadow-1"
-                    @update:model-value="loadInstallablePlugins"
-                    dense
-                    :label="$t('components.plugins.categoryFilter')"
-                    v-model="tagFilter"
-                    :options="tags"
-                    style="min-width: 300px">
-                    <template v-slot:append>
-                      <q-icon name="style"/>
-                    </template>
-                  </q-select>
-                </div>
-              </div>
-            </template>
-
-            <template
-              v-if="!$q.platform.is.mobile"
-              v-slot:top-right>
-              <div class="row q-col-gutter-xs q-ma-xs">
-                <div class="col-auto">
-                  <PluginInstallerManageRepos v-on:repoReloaded="reloadPluginsPostRepoReloaded"/>
-                </div>
-              </div>
+        <div class="col-auto">
+          <q-input
+            filled
+            class="shadow-1"
+            dense
+            debounce="300"
+            v-model="filter"
+            :placeholder="$t('navigation.search')">
+            <template v-slot:append>
+              <q-icon name="search"/>
             </template>
-
-            <template v-slot:no-data>
-              <div class="full-width row flex-center text-accent q-gutter-sm">
-                <q-icon size="2em" name="sentiment_dissatisfied"/>
-                <q-item-label>{{ $t('headers.listEmpty') }}</q-item-label>
-                <q-icon size="2em" name="priority_high"/>
-              </div>
+          </q-input>
+        </div>
+        <div class="col-auto">
+          <q-select
+            filled
+            class="shadow-1"
+            @update:model-value="loadInstallablePlugins"
+            dense
+            :label="$t('components.plugins.categoryFilter')"
+            v-model="tagFilter"
+            :options="tags"
+            style="min-width: 300px">
+            <template v-slot:append>
+              <q-icon name="style"/>
             </template>
+          </q-select>
+        </div>
+      </div>
+    </div>
+    <div class="col self-end">
+      <div class="row q-col-gutter-xs q-ma-xs float-right">
+        <div class="col-auto">
+          <PluginInstallerManageRepos v-on:repoReloaded="reloadPluginsPostRepoReloaded"/>
+        </div>
+      </div>
+    </div>
+  </div>
+
+  <div :class="$q.platform.is.mobile ? 'q-px-none' : ''">
+
+    <q-table
+      grid
+      card-class="bg-primary text-white"
+      :rows="rows"
+      :columns="columns"
+      row-key="name"
+      :filter="filter"
+      hide-header
+      v-model:pagination="pagination"
+      hide-pagination
+      class="plugin-table"
+    >
+
+      <template v-slot:no-data>
+        <div class="full-width row flex-center text-accent q-gutter-sm">
+          <q-icon size="2em" name="sentiment_dissatisfied"/>
+          <q-item-label>{{ $t('headers.listEmpty') }}</q-item-label>
+          <q-icon size="2em" name="priority_high"/>
+        </div>
+      </template>
 
-            <template v-slot:item="props">
-              <div class="q-pa-xs col-xs-12 col-sm-6 col-md-4 col-lg-3 col-xl-2">
-                <q-card
-                  style="min-height: 220px;">
-                  <q-card-section
-                    style="min-height: 80px">
-                    <div class="row">
+      <template v-slot:item="props">
+        <div class="q-pa-xs col-xs-12 col-sm-6 col-md-4 col-lg-3 col-xl-2">
+          <q-card
+            style="min-height: 220px;">
+            <q-card-section
+              style="min-height: 50px">
+              <div class="row">
                       <span style="overflow: hidden;white-space: nowrap;">
                         <strong>{{ props.row.name }}</strong>
                       </span>
-                    </div>
-                    <div class="row float-right">
-                      <!--INSTALLED STATUS-->
-                      <q-btn
-                        v-if="props.row.update_available"
-                        color="warning"
-                        dense
-                        round
-                        flat
-                        icon="check_circle"> Update Available
-                      </q-btn>
-                      <q-btn
-                        v-else-if="props.row.installed"
-                        color="positive"
-                        dense
-                        round
-                        flat
-                        icon="check_circle"> Installed
-                      </q-btn>
-                    </div>
-                  </q-card-section>
+              </div>
+            </q-card-section>
 
-                  <q-separator
-                    v-if="props.row.update_available"
-                    color="warning"
-                  />
+            <q-separator
+              v-if="props.row.update_available"
+              color="warning"
+            />
 
-                  <q-separator
-                    v-else-if="props.row.installed"
-                    color="positive"
-                  />
+            <q-separator
+              v-else-if="props.row.installed"
+              color="positive"
+            />
 
-                  <q-separator
-                    v-else
-                  />
+            <q-separator
+              v-else
+            />
 
-                  <q-card-section>
-                    <div class="row q-col-gutter-md">
-                      <div class="col-auto">
-                        <q-skeleton v-if="!props.row.icon" width="100px" height="100px"/>
-                        <q-avatar
-                          v-else
-                          rounded
-                          size="100px">
-                          <q-img :src="props.row.icon" style="height:100%; max-width: 100px;">
-                            <template v-slot:error>
-                              <div class="absolute-full flex flex-center bg-negative text-white text-caption">
-                                {{ $t('status.cannotLoadImage') }}
-                              </div>
-                              <!--                            <img :src="props.row.icon">-->
-                            </template>
-                          </q-img>
-                        </q-avatar>
-                      </div>
-                      <div class="col">
-                        <div class="row q-col-gutter-md">
-                          <div class="col-4 self-start">{{ $t('components.plugins.author') }}</div>
-                          <div class="col self-end">{{ props.row.author }}</div>
-                        </div>
-                        <div class="row q-col-gutter-md">
-                          <div class="col-4 self-start">{{ $t('components.plugins.version') }}</div>
-                          <div class="col self-end">{{ props.row.version }}</div>
-                        </div>
-                        <div class="row q-col-gutter-md">
-                          <div class="col-4 self-start">{{ $t('components.plugins.repo') }}</div>
-                          <div class="col self-end">{{ props.row.repo_name }}</div>
+            <q-card-section>
+              <div class="row q-col-gutter-md">
+                <div class="col-auto">
+                  <q-skeleton v-if="!props.row.icon" width="100px" height="100px"/>
+                  <q-avatar
+                    v-else
+                    rounded
+                    size="100px">
+                    <q-img :src="props.row.icon" style="height:100%; max-width: 100px;">
+                      <template v-slot:error>
+                        <div class="absolute-full flex flex-center bg-negative text-white text-caption">
+                          {{ $t('status.cannotLoadImage') }}
                         </div>
-                      </div>
-                    </div>
-                  </q-card-section>
-
-                  <q-card-section>
-                    <div class="row">
-                      <div class="col-auto items-end">
-                        <!--INSTALL BUTTON-->
-                        <q-btn
-                          v-if="props.row.update_available"
-                          @click="installPlugin(props.row.plugin_id, props.row.repo_id)"
-                          color="accent"
-                          dense
-                          round
-                          flat
-                          icon="update">
-                          <q-tooltip class="bg-white text-primary">{{ $t('tooltips.update') }}</q-tooltip>
-                        </q-btn>
-                        <q-btn
-                          v-else-if="props.row.installed"
-                          @click="installPlugin(props.row.plugin_id, props.row.repo_id)"
-                          color="accent"
-                          dense
-                          round
-                          flat
-                          icon="download_for_offline">
-                          <q-tooltip class="bg-white text-primary">{{ $t('tooltips.reinstall') }}</q-tooltip>
-                        </q-btn>
-                        <q-btn
-                          v-else
-                          @click="installPlugin(props.row.plugin_id, props.row.repo_id)"
-                          color="accent"
-                          dense
-                          round
-                          flat
-                          icon="download_for_offline">
-                          <q-tooltip class="bg-white text-primary">{{ $t('tooltips.install') }}</q-tooltip>
-                        </q-btn>
-
-                        <!--DISPLAY INFORMATION BUTTON-->
-                        <q-btn
-                          @click="showPluginInfo = props.row.plugin_id"
-                          color="secondary"
-                          dense
-                          round
-                          flat
-                          icon="info">
-                          <q-tooltip class="bg-white text-primary">{{ $t('tooltips.pluginInfo') }}</q-tooltip>
-                        </q-btn>
-                      </div>
-                    </div>
-                  </q-card-section>
-
-                  <q-inner-loading :showing="pluginInstalling[props.row.repo_id + props.row.plugin_id]">
-                    <q-spinner size="100px" color="secondary"/>
-                  </q-inner-loading>
-
-                </q-card>
+                        <!--                            <img :src="props.row.icon">-->
+                      </template>
+                    </q-img>
+                  </q-avatar>
+                </div>
+                <div class="col">
+                  <div class="row q-col-gutter-md">
+                    <div class="col-4 self-start">{{ $t('components.plugins.author') }}</div>
+                    <div class="col self-end">{{ props.row.author }}</div>
+                  </div>
+                  <div class="row q-col-gutter-md">
+                    <div class="col-4 self-start">{{ $t('components.plugins.version') }}</div>
+                    <div class="col self-end">{{ props.row.version }}</div>
+                  </div>
+                  <div class="row q-col-gutter-md">
+                    <div class="col-4 self-start">{{ $t('components.plugins.repo') }}</div>
+                    <div class="col self-end">{{ props.row.repo_name }}</div>
+                  </div>
+                </div>
               </div>
-            </template>
+            </q-card-section>
 
-          </q-table>
+            <q-card-section class="q-pt-none">
+              <div class="row">
+                <div class="col self-start items-end">
+                  <!--INSTALL BUTTON-->
+                  <q-btn
+                    v-if="props.row.update_available"
+                    @click="installPlugin(props.row.plugin_id, props.row.repo_id)"
+                    color="accent"
+                    dense
+                    round
+                    flat
+                    icon="update">
+                    <q-tooltip class="bg-white text-primary">{{ $t('tooltips.update') }}</q-tooltip>
+                  </q-btn>
+                  <q-btn
+                    v-else-if="props.row.installed"
+                    @click="installPlugin(props.row.plugin_id, props.row.repo_id)"
+                    color="accent"
+                    dense
+                    round
+                    flat
+                    icon="download_for_offline">
+                    <q-tooltip class="bg-white text-primary">{{ $t('tooltips.reinstall') }}</q-tooltip>
+                  </q-btn>
+                  <q-btn
+                    v-else
+                    @click="installPlugin(props.row.plugin_id, props.row.repo_id)"
+                    color="accent"
+                    dense
+                    round
+                    flat
+                    icon="download_for_offline">
+                    <q-tooltip class="bg-white text-primary">{{ $t('tooltips.install') }}</q-tooltip>
+                  </q-btn>
+
+                  <!--DISPLAY INFORMATION BUTTON-->
+                  <q-btn
+                    @click="openPluginInfo(props.row.plugin_id, 'info')"
+                    color="secondary"
+                    dense
+                    round
+                    flat
+                    icon="info">
+                    <q-tooltip class="bg-white text-primary">{{ $t('tooltips.pluginInfo') }}</q-tooltip>
+                  </q-btn>
+                </div>
+                <div class="col self-end">
+                  <!--INSTALLED STATUS-->
+                  <q-btn
+                    v-if="props.row.update_available"
+                    color="warning"
+                    dense
+                    round
+                    flat
+                    class="float-right"
+                    icon="check_circle"> Update Available
+                  </q-btn>
+                  <q-btn
+                    v-else-if="props.row.installed"
+                    color="positive"
+                    dense
+                    round
+                    flat
+                    class="float-right"
+                    icon="check_circle"> Installed
+                  </q-btn>
+                </div>
+              </div>
+            </q-card-section>
 
-          <div class="row justify-center q-mt-md">
-            <q-pagination
-              v-model="pagination.page"
-              color="secondary"
-              :max="pagesNumber"
-              size="md"
-              direction-links
-              boundary-links
-            />
-          </div>
+            <q-inner-loading :showing="pluginInstalling[props.row.repo_id + props.row.plugin_id]">
+              <q-spinner size="100px" color="secondary"/>
+            </q-inner-loading>
 
+          </q-card>
         </div>
-      </q-card-section>
-    </q-card>
+      </template>
+
+    </q-table>
 
-    <PluginInfo v-bind:showPluginInfo="showPluginInfo"
-                v-bind:viewingRemoteInfo="viewingRemoteInfo"
-                v-on:hide="closePluginInfo"/>
+  </div>
 
-  </q-dialog>
 </template>
 
 <script>
 import axios from "axios";
 import { getUnmanicApiUrl } from "src/js/unmanicGlobals";
-import { computed, onMounted, ref } from "vue";
-import PluginInfo from "components/PluginInfo";
+import { computed, ref } from "vue";
+import PluginInfoDialog from "components/dialogs/PluginInfoDialog";
 import PluginInstallerManageRepos from "components/PluginInstallerManageRepos";
 
-const columns = [
-  {
-    name: 'icon',
-    required: true,
-    label: '',
-    align: 'left',
-    field: 'icon',
-    sortable: true
-  },
-  {
-    name: 'name',
-    required: true,
-    label: 'Name',
-    align: 'left',
-    field: 'name',
-    sortable: true
-  },
-  {
-    name: 'author',
-    align: 'center',
-    label: 'Author',
-    field: 'author',
-    sortable: false
-  },
-  {
-    name: 'version',
-    align: 'center',
-    label: 'Version',
-    field: 'version',
-    sortable: false
-  }
-]
-
 
 export default {
-  name: 'PluginInstallerDialog',
+  name: 'PluginInstallerForm',
+  components: { PluginInstallerManageRepos },
   props: {},
-  emits: [
-    // REQUIRED
-    'ok', 'hide', 'path'
-  ],
-  components: { PluginInstallerManageRepos, PluginInfo },
-  methods: {
-    // following method is REQUIRED
-    // (don't change its name --> "show")
-    show() {
-      this.$refs.dialogRef.show();
-    },
+  data: function () {
+    const filter = ref('')
+    const columns = ref([
+      {
+        name: 'icon',
+        required: true,
+        label: '',
+        align: 'left',
+        field: 'icon',
+        sortable: true
+      },
+      {
+        name: 'name',
+        required: true,
+        label: 'Name',
+        align: 'left',
+        field: 'name',
+        sortable: true
+      },
+      {
+        name: 'author',
+        align: 'center',
+        label: 'Author',
+        field: 'author',
+        sortable: false
+      },
+      {
+        name: 'version',
+        align: 'center',
+        label: 'Version',
+        field: 'version',
+        sortable: false
+      }
+    ])
+    const rows = ref([])
+    const pagination = ref({
+      page: 1,
+      rowsPerPage: 0
+    })
+    const tags = ref([])
+    const tagFilter = ref('All')
+
+    return {
+      /*
+      Required data:
+        - isLoading
+        - isSaved
+      */
+      isLoading: false,
+      isSaved: true,
+
+      pluginInstalling: ref({}),
 
-    // following method is REQUIRED
-    // (don't change its name --> "hide")
+      filter,
+      columns,
+      rows,
+      pagination,
+      tags,
+      tagFilter,
+    }
+  },
+  mounted() {
+    this.loadInstallablePlugins();
+  },
+  methods: {
+    /*
+    Required methods:
+      - hide()
+      - save()
+      - cancel()
+    */
     hide() {
-      this.$refs.dialogRef.hide();
+      return true;
     },
-
-    onDialogHide() {
-      // required to be emitted
-      // when QDialog emits "hide" event
-      this.$emit('hide')
+    save() {
+      return true;
+    },
+    cancel() {
+      return true;
     },
+
     installPlugin: function (plugin_id, repo_id) {
       console.debug('Installing plugin by Plugin ID: ' + plugin_id + 'from Repo ID - ' + repo_id)
 
       let data = {
         plugin_id: plugin_id,
         repo_id: repo_id,
       }
@@ -473,41 +418,60 @@
       // A repo refresh will reset a bunch of things.
       // This can mess up pagination. Best solution is to force us back to page one...
       this.pagination.page = 1;
 
       // Now trigger a reload of the installable plugins
       this.loadInstallablePlugins();
     },
-    closePluginInfo: function () {
-      this.showPluginInfo = '';
+    openPluginInfo: function (pluginId, tab) {
+      // Ensure we have the info for the plugin to be displayed
+      if (pluginId === '') {
+        // Display error notification
+        this.$q.notify({
+          color: 'negative',
+          position: 'top',
+          message: 'An error was encountered while attempting to open plugin info',
+          icon: 'report_problem',
+          actions: [{ icon: 'close', color: 'white' }]
+        })
+        return
+      }
+      // Display the dialog
+      this.$q.dialog({
+        component: PluginInfoDialog,
+        componentProps: {
+          pluginId: pluginId,
+          startTab: (tab === 'settings') ? 'settings' : 'info',
+          libraryId: this.currentID,
+          viewingRemoteInfo: true,
+        },
+      }).onOk((payload) => {
+      }).onDismiss(() => {
+      })
     }
   },
-  created() {
-    this.loadInstallablePlugins();
-  },
-  data: function () {
-    const tags = ref([])
-    const tagFilter = ref('All')
-
-    const rows = ref([])
-    const filter = ref('')
-    const pagination = ref({
-      page: 1,
-      rowsPerPage: 12
-    })
-
-    return {
-      filter,
-      columns,
-      rows,
-      pagination,
-      pagesNumber: computed(() => Math.ceil(rows.value.length / pagination.value.rowsPerPage)),
-      tags,
-      tagFilter,
-
-      viewingRemoteInfo: ref(true),
-      showPluginInfo: ref(''),
-      pluginInstalling: ref({}),
+  watch: {
+    libraryId(value) {
+      if (value.length > 0) {
+        this.currentID = this.libraryId;
+      }
     }
   }
 }
 </script>
+
+<style scoped>
+.plugin-table-actions-bar {
+  position: sticky;
+  top: 65px;
+  z-index: 90;
+  background: #fff;
+}
+
+.q-dark .plugin-table-actions-bar {
+  background: var(--q-dark) !important
+}
+
+.plugin-table {
+  margin-bottom: 220px;
+}
+</style>
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/CompletedTaskLogDialog.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/CompletedTaskLogDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/MobileSettingsQuickNav.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/MobileSettingsQuickNav.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/WorkerGroupConfigureDialog.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/WorkerGroupConfigureDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/LinkConfigureDialog.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/LinkConfigureDialog.vue`

 * *Files 1% similar despite different names*

```diff
@@ -327,25 +327,25 @@
       // required to be emitted
       // when QDialog emits "hide" event
       this.$emit('ok', {})
       this.$emit('hide')
     },
 
     fetchInstallationLinkConfig: function (uuid) {
-      this.currentUuid = uuid;
       // Fetch from server
       let data = {
-        uuid: this.currentUuid,
+        uuid: uuid,
       }
       axios({
         method: 'post',
         url: getUnmanicApiUrl('v2', 'settings/link/read'),
         data: data
       }).then((response) => {
         let link_config = response.data.link_config;
+        this.currentUuid = uuid;
         this.address = link_config.address;
         this.authType = link_config.auth;
         this.username = link_config.username;
         this.password = link_config.password;
         this.available = link_config.available;
         this.name = link_config.name;
         this.version = link_config.version;
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/PendingTasksTable.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/PendingTasksTable.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/JsonImportExportDialog.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/JsonImportExportDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/PluginSelectorDialog.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/PluginSelectorDialog.vue`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         <div class="row q-gutter-xs q-mt-xs justify-between">
           <div class="col-auto">
             <q-btn
               @click="openPluginInstaller"
               class=""
               color="secondary"
               icon-right="add"
-              :label="$t('components.plugins.installPlugins')"/>
+              :label="$t('components.plugins.installPluginFromRepo')"/>
           </div>
           <div class="col-auto" style="max-width: 200px">
             <q-input
               filled dense
               class="shadow-1"
               debounce="300"
               color="primary"
@@ -134,15 +134,15 @@
 </template>
 
 <script>
 
 import axios from "axios";
 import { getUnmanicApiUrl } from "src/js/unmanicGlobals";
 import { ref } from "vue";
-import PluginInstallerDialog from "components/PluginInstallerDialog";
+import ConfigDrawerDialog from "components/dialogs/ConfigDrawerDialog";
 
 export default {
   name: 'PluginSelectorDialog',
   props: {
     dialogHeader: {
       type: String,
       default: ' --- header --- '
@@ -216,17 +216,21 @@
     selectPlugin(plugin) {
       this.currentPlugin = plugin;
       this.hide();
     },
 
     openPluginInstaller() {
       this.$q.dialog({
-        component: PluginInstallerDialog,
-        // props forwarded to your custom component
-        componentProps: {},
+        component: ConfigDrawerDialog,
+        componentProps: {
+          header: this.$t('headers.pluginInstaller'),
+          componentName: "PluginInstallerForm",
+          width: "2000px",
+          componentProps: {},
+        },
       }).onOk((payload) => {
       }).onDismiss(() => {
         this.fetchPluginsList();
       })
     },
 
   },
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/WorkerProgressLog.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/WorkerProgressLog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/DrawerMainNav.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/DrawerMainNav.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/EssentialLink.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/EssentialLink.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/DrawerSettingsNav.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/DrawerSettingsNav.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/LibraryConfigureDialog.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/forms/LibraryConfigForm.vue`

 * *Files 3% similar despite different names*

```diff
@@ -1,465 +1,400 @@
 <template>
 
-  <!-- START DIALOG CONFIG
-  Right fullscreen pop-up
-  Note: Update template q-dialog ref="" value
-
-  All Platforms:
-   - Swipe right to dismiss
-  Desktop:
-   - Width 700px
-   - Minimise button top-right
-  Mobile:
-   - Full screen
-   - Back button top-left
-  -->
-  <q-dialog
-    ref="libraryConfigureDialogRef"
-    :maximized="$q.platform.is.mobile"
-    :transition-show="$q.platform.is.mobile ? 'jump-left' : 'slide-left'"
-    :transition-hide="$q.platform.is.mobile ? 'jump-right' : 'slide-right'"
-    full-height
-    position="right"
-    @before-hide="beforeDialogHide"
-    @hide="onDialogHide">
-
-    <q-card
-      v-touch-swipe.touch.right="hide"
-      :style="$q.platform.is.mobile ? 'max-width: 100vw;' : 'max-width: 95vw;'"
-      style="width:700px;">
-
-      <q-card-section class="bg-card-head">
-        <div class="row items-center no-wrap">
-          <div
-            v-if="$q.platform.is.mobile"
-            class="col">
-            <q-btn
-              color="grey-7"
-              dense
-              round
-              flat
-              icon="arrow_back"
-              v-close-popup>
-            </q-btn>
-          </div>
+  <div :class="$q.platform.is.mobile ? 'q-px-none' : ''">
+
+    <q-card flat>
+      <q-card-section :class="$q.platform.is.mobile ? 'q-px-none' : ''">
 
+        <div class="row items-center no-wrap q-mb-md">
           <div class="col">
-            <div class="text-h6 text-blue-10">
-              {{ dialogHeader }}
+            <div class="text-h5">
+              {{ $t('components.settings.common.configuration') }}
             </div>
           </div>
-
-          <div
-            v-if="!$q.platform.is.mobile"
-            class="col-auto">
+          <div class="col-auto">
+            <q-btn
+              round
+              flat
+              color="primary"
+              icon="download"
+              @click="exportPluginConfig">
+              <q-tooltip class="bg-white text-primary">{{
+                  $t('components.settings.library.exportLibraryConfig')
+                }}
+              </q-tooltip>
+            </q-btn>
+            <q-btn
+              round
+              flat
+              color="primary"
+              icon="publish"
+              @click="importPluginConfig">
+              <q-tooltip class="bg-white text-primary">{{
+                  $t('components.settings.library.importLibraryConfig')
+                }}
+              </q-tooltip>
+            </q-btn>
             <q-btn
-              color="grey-7"
-              dense
               round
               flat
-              icon="arrow_forward"
-              v-close-popup>
-              <q-tooltip class="bg-white text-primary">{{ $t('tooltips.close') }}</q-tooltip>
+              color="primary"
+              icon="content_copy"
+              @click="cloneLibrary">
+              <q-tooltip class="bg-white text-primary">{{
+                  $t('components.settings.library.cloneLibrary')
+                }}
+              </q-tooltip>
+            </q-btn>
+            <q-btn
+              v-if="locked"
+              round
+              flat
+              color="negative"
+              icon="lock"
+              @click="locked = false">
+              <q-tooltip class="bg-white text-primary">{{
+                  $t('components.settings.library.locked')
+                }}
+              </q-tooltip>
+            </q-btn>
+            <q-btn
+              v-else
+              round
+              flat
+              color="primary"
+              icon="lock_open"
+              @click="locked = true">
+              <q-tooltip class="bg-white text-primary">{{
+                  $t('components.settings.library.unlocked')
+                }}
+              </q-tooltip>
             </q-btn>
           </div>
         </div>
-      </q-card-section>
-      <!-- END DIALOG CONFIG -->
 
-      <q-card-section class="q-pt-none">
-
-        <div :class="$q.platform.is.mobile ? 'q-px-none' : ''">
-
-          <q-card flat>
-            <q-card-section :class="$q.platform.is.mobile ? 'q-px-none' : ''">
-
-              <div class="row items-center no-wrap q-mb-md">
-                <div class="col">
-                  <div class="text-h5">
-                    {{ $t('components.settings.common.configuration') }}
-                  </div>
-                </div>
-                <div class="col-auto">
-                  <q-btn
-                    round
-                    flat
-                    color="primary"
-                    icon="download"
-                    @click="exportPluginConfig">
-                    <q-tooltip class="bg-white text-primary">{{
-                        $t('components.settings.library.exportLibraryConfig')
-                      }}
-                    </q-tooltip>
-                  </q-btn>
-                  <q-btn
-                    round
-                    flat
-                    color="primary"
-                    icon="publish"
-                    @click="importPluginConfig">
-                    <q-tooltip class="bg-white text-primary">{{
-                        $t('components.settings.library.importLibraryConfig')
-                      }}
-                    </q-tooltip>
-                  </q-btn>
-                  <q-btn
-                    round
-                    flat
-                    color="primary"
-                    icon="content_copy"
-                    @click="cloneLibrary">
-                    <q-tooltip class="bg-white text-primary">{{
-                        $t('components.settings.library.cloneLibrary')
-                      }}
-                    </q-tooltip>
-                  </q-btn>
-                  <q-btn
-                    v-if="locked"
-                    round
-                    flat
-                    color="negative"
-                    icon="lock"
-                    @click="locked = false">
-                    <q-tooltip class="bg-white text-primary">{{
-                        $t('components.settings.library.locked')
-                      }}
-                    </q-tooltip>
-                  </q-btn>
-                  <q-btn
-                    v-else
-                    round
-                    flat
-                    color="primary"
-                    icon="lock_open"
-                    @click="locked = true">
-                    <q-tooltip class="bg-white text-primary">{{
-                        $t('components.settings.library.unlocked')
-                      }}
-                    </q-tooltip>
-                  </q-btn>
-                </div>
-              </div>
-
-              <div class="q-pb-sm">
-                <q-skeleton
-                  v-if="name === null"
-                  type="QInput"/>
-                <q-input
-                  v-if="name !== null"
-                  outlined
-                  color="primary"
-                  v-model="name"
-                  :label="$t('components.settings.library.name')"
-                  :placeholder="name">
-                </q-input>
-              </div>
-
-              <div
-                v-if="enableReceiveRemoteFilesOnly !== true"
-                class="q-pb-sm">
-                <q-skeleton
-                  v-if="path === null"
-                  type="QInput"/>
-                <q-input
-                  v-else
-                  readonly
-                  outlined
-                  color="primary"
-                  v-model="path"
-                  label-slot
-                  :placeholder="path"
-                  :disable="enableReceiveRemoteFilesOnly === true"
-                  @click="updateLibraryWithDirectoryBrowser">
-                  <template v-slot:label>
-                    <div class="row items-center all-pointer-events">
-                      {{ $t('components.settings.library.path') }}
-                    </div>
-                  </template>
-                  <template v-slot:append>
-                    <q-icon
-                      @click="updateLibraryWithDirectoryBrowser"
-                      class="cursor-pointer"
-                      name="folder_open"/>
-                  </template>
-                </q-input>
-                <q-tooltip
-                  v-if="enableReceiveRemoteFilesOnly === true"
-                  class="bg-white text-primary"
-                  anchor="bottom left"
-                  self="bottom left">
-                  {{ $t('components.settings.library.pathDisabledReceiveRemoteFilesOnly') }}
-                </q-tooltip>
-              </div>
+        <div class="q-pb-sm">
+          <q-skeleton
+            v-if="name === null"
+            type="QInput"/>
+          <q-input
+            v-if="name !== null"
+            outlined
+            color="primary"
+            v-model="name"
+            :label="$t('components.settings.library.name')"
+            :placeholder="name">
+          </q-input>
+        </div>
 
-              <div class="q-pb-sm">
-                <q-skeleton
-                  v-if="enableReceiveRemoteFilesOnly === null"
-                  type="QToggle"/>
-                <q-item
-                  v-else
-                  tag="label"
-                  class="border-hover"
-                  style="padding-left:12px">
-                  <q-item-section>
-                    <q-item-label>{{ $t('components.settings.library.enableReceiveRemoteFilesOnly') }}</q-item-label>
-                  </q-item-section>
-                  <q-item-section avatar>
-                    <q-toggle v-model="enableReceiveRemoteFilesOnly"/>
-                  </q-item-section>
-                </q-item>
-              </div>
-              <div
-                v-if="enableReceiveRemoteFilesOnly !== true"
-                class="q-pb-sm">
-                <q-skeleton
-                  v-if="enableScanner === null"
-                  type="QToggle"/>
-                <q-item
-                  v-else
-                  tag="label"
-                  class="border-hover"
-                  style="padding-left:12px"
-                  :disable="enableReceiveRemoteFilesOnly === true">
-                  <q-item-section>
-                    <q-item-label>{{ $t('components.settings.library.enableScanner') }}</q-item-label>
-                  </q-item-section>
-                  <q-item-section avatar>
-                    <q-toggle v-model="enableScanner" :disable="enableReceiveRemoteFilesOnly === true"/>
-                  </q-item-section>
-                </q-item>
-                <q-tooltip
-                  v-if="enableReceiveRemoteFilesOnly === true"
-                  class="bg-white text-primary"
-                  anchor="bottom left"
-                  self="bottom left">
-                  {{ $t('components.settings.library.pathDisabledReceiveRemoteFilesOnly') }}
-                </q-tooltip>
-              </div>
-              <div
-                v-if="enableReceiveRemoteFilesOnly !== true"
-                class="q-pb-sm">
-                <q-skeleton
-                  v-if="enableInotify === null"
-                  type="QToggle"/>
-                <q-item
-                  v-else
-                  tag="label"
-                  class="border-hover"
-                  style="padding-left:12px"
-                  :disable="enableReceiveRemoteFilesOnly === true">
-                  <q-item-section>
-                    <q-item-label>{{ $t('components.settings.library.enableInotify') }}</q-item-label>
-                  </q-item-section>
-                  <q-item-section avatar>
-                    <q-toggle v-model="enableInotify" :disable="enableReceiveRemoteFilesOnly === true"/>
-                  </q-item-section>
-                </q-item>
-                <q-tooltip
-                  v-if="enableReceiveRemoteFilesOnly === true"
-                  class="bg-white text-primary"
-                  anchor="bottom left"
-                  self="bottom left">
-                  {{ $t('components.settings.library.pathDisabledReceiveRemoteFilesOnly') }}
-                </q-tooltip>
-              </div>
+        <div
+          v-if="enableReceiveRemoteFilesOnly !== true"
+          class="q-pb-sm">
+          <q-skeleton
+            v-if="path === null"
+            type="QInput"/>
+          <q-input
+            v-else
+            readonly
+            outlined
+            color="primary"
+            v-model="path"
+            label-slot
+            :placeholder="path"
+            :disable="enableReceiveRemoteFilesOnly === true"
+            @click="updateLibraryWithDirectoryBrowser">
+            <template v-slot:label>
+              <div class="row items-center all-pointer-events">
+                {{ $t('components.settings.library.path') }}
+              </div>
+            </template>
+            <template v-slot:append>
+              <q-icon
+                @click="updateLibraryWithDirectoryBrowser"
+                class="cursor-pointer"
+                name="folder_open"/>
+            </template>
+          </q-input>
+          <q-tooltip
+            v-if="enableReceiveRemoteFilesOnly === true"
+            class="bg-white text-primary"
+            anchor="bottom left"
+            self="bottom left">
+            {{ $t('components.settings.library.pathDisabledReceiveRemoteFilesOnly') }}
+          </q-tooltip>
+        </div>
 
-              <div class="q-pb-sm">
-                <q-skeleton
-                  v-if="priorityScore === null"
-                  type="QInput"/>
-                <q-input
-                  v-if="priorityScore !== null"
-                  outlined
-                  color="primary"
-                  v-model.number="priorityScore"
-                  :label="$t('components.settings.library.priorityScore')"
-                  type="number"
-                />
-              </div>
+        <div class="q-pb-sm">
+          <q-skeleton
+            v-if="enableReceiveRemoteFilesOnly === null"
+            type="QToggle"/>
+          <q-item
+            v-else
+            tag="label"
+            class="border-hover"
+            style="padding-left:12px">
+            <q-item-section>
+              <q-item-label>{{ $t('components.settings.library.enableReceiveRemoteFilesOnly') }}</q-item-label>
+            </q-item-section>
+            <q-item-section avatar>
+              <q-toggle v-model="enableReceiveRemoteFilesOnly"/>
+            </q-item-section>
+          </q-item>
+        </div>
+        <div
+          v-if="enableReceiveRemoteFilesOnly !== true"
+          class="q-pb-sm">
+          <q-skeleton
+            v-if="enableScanner === null"
+            type="QToggle"/>
+          <q-item
+            v-else
+            tag="label"
+            class="border-hover"
+            style="padding-left:12px"
+            :disable="enableReceiveRemoteFilesOnly === true">
+            <q-item-section>
+              <q-item-label>{{ $t('components.settings.library.enableScanner') }}</q-item-label>
+            </q-item-section>
+            <q-item-section avatar>
+              <q-toggle v-model="enableScanner" :disable="enableReceiveRemoteFilesOnly === true"/>
+            </q-item-section>
+          </q-item>
+          <q-tooltip
+            v-if="enableReceiveRemoteFilesOnly === true"
+            class="bg-white text-primary"
+            anchor="bottom left"
+            self="bottom left">
+            {{ $t('components.settings.library.pathDisabledReceiveRemoteFilesOnly') }}
+          </q-tooltip>
+        </div>
+        <div
+          v-if="enableReceiveRemoteFilesOnly !== true"
+          class="q-pb-sm">
+          <q-skeleton
+            v-if="enableInotify === null"
+            type="QToggle"/>
+          <q-item
+            v-else
+            tag="label"
+            class="border-hover"
+            style="padding-left:12px"
+            :disable="enableReceiveRemoteFilesOnly === true">
+            <q-item-section>
+              <q-item-label>{{ $t('components.settings.library.enableInotify') }}</q-item-label>
+            </q-item-section>
+            <q-item-section avatar>
+              <q-toggle v-model="enableInotify" :disable="enableReceiveRemoteFilesOnly === true"/>
+            </q-item-section>
+          </q-item>
+          <q-tooltip
+            v-if="enableReceiveRemoteFilesOnly === true"
+            class="bg-white text-primary"
+            anchor="bottom left"
+            self="bottom left">
+            {{ $t('components.settings.library.pathDisabledReceiveRemoteFilesOnly') }}
+          </q-tooltip>
+        </div>
 
-              <div class="q-pb-sm">
-                <q-skeleton
-                  v-if="tags === null"
-                  type="QInput"/>
-                <q-select
-                  filled
-                  use-input
-                  use-chips
-                  multiple
-                  hide-dropdown-icon
-                  input-debounce="0"
-                  new-value-mode="add-unique"
-                  v-model="tags"
-                  :label="$t('components.settings.common.tags')"
-                  @keyup.tab="addTag"
-                />
-              </div>
-            </q-card-section>
+        <div class="q-pb-sm">
+          <q-skeleton
+            v-if="priorityScore === null"
+            type="QInput"/>
+          <q-input
+            v-if="priorityScore !== null"
+            outlined
+            color="primary"
+            v-model.number="priorityScore"
+            :label="$t('components.settings.library.priorityScore')"
+            type="number"
+          />
+        </div>
 
-            <q-separator/>
+        <div class="q-pb-sm">
+          <q-skeleton
+            v-if="tags === null"
+            type="QInput"/>
+          <q-select
+            filled
+            use-input
+            use-chips
+            multiple
+            hide-dropdown-icon
+            input-debounce="0"
+            new-value-mode="add-unique"
+            v-model="tags"
+            :label="$t('components.settings.common.tags')"
+            @keyup.tab="addTag"
+          />
+        </div>
+      </q-card-section>
 
-            <q-card-section :class="$q.platform.is.mobile ? 'q-px-none' : ''">
+      <q-separator/>
 
-              <div class="row items-center no-wrap q-mb-md">
-                <div class="col">
-                  <div class="text-h6">
-                    {{ $t('components.settings.library.plugins') }}
-                  </div>
-                </div>
-              </div>
+      <q-card-section :class="$q.platform.is.mobile ? 'q-px-none' : ''">
 
-              <div class="q-gutter-sm">
-                <q-skeleton
-                  v-if="enabledPlugins === null"
-                  type="text"/>
-
-                <q-list
-                  bordered
-                  separator
-                  class="rounded-borders">
-
-
-                  <div
-                    v-for="(plugin, index) in enabledPlugins"
-                    v-bind:key="index">
-                    <q-item>
-
-                      <q-item-section avatar>
-                        <q-img :src="plugin.icon"/>
-                      </q-item-section>
-
-                      <q-item-section>
-                        <q-item-label>{{ plugin.name }}</q-item-label>
-                        <q-item-label caption lines="2">{{ plugin.description }}</q-item-label>
-                      </q-item-section>
-
-                      <q-separator inset vertical class="q-mx-sm"/>
-
-                      <q-item-section center side>
-                        <div class="text-grey-8 q-gutter-xs">
-                          <q-btn
-                            flat dense round
-                            size="12px"
-                            color="grey-8"
-                            icon="tune"
-                            :disable="!plugin.has_config"
-                            @click="showPluginSettings = plugin.plugin_id">
-                            <q-tooltip class="bg-white text-primary">
-                              {{ $t('tooltips.configureForThisLibrary') }}
-                            </q-tooltip>
-                          </q-btn>
-                          <q-btn
-                            flat dense round
-                            size="12px"
-                            color="negative"
-                            icon="remove_circle_outline"
-                            @click="removePluginFromList(index)">
-                            <q-tooltip class="bg-white text-primary">
-                              {{ $t('tooltips.removeFromThisLibrary') }}
-                            </q-tooltip>
-                          </q-btn>
-                        </div>
-                      </q-item-section>
+        <div class="row items-center no-wrap q-mb-md">
+          <div class="col">
+            <div class="text-h6">
+              {{ $t('components.settings.library.plugins') }}
+            </div>
+          </div>
+        </div>
 
-                    </q-item>
+        <div class="q-gutter-sm">
+          <q-skeleton
+            v-if="enabledPlugins === null"
+            type="text"/>
+
+          <q-list
+            bordered
+            separator
+            class="rounded-borders">
+
+
+            <div
+              v-for="(plugin, index) in enabledPlugins"
+              v-bind:key="index">
+              <q-item>
+
+                <q-item-section avatar>
+                  <q-img :src="plugin.icon"/>
+                </q-item-section>
+
+                <q-item-section>
+                  <q-item-label>{{ plugin.name }}</q-item-label>
+                  <q-item-label caption lines="2">{{ plugin.description }}</q-item-label>
+                </q-item-section>
+
+                <q-separator inset vertical class="q-mx-sm"/>
+
+                <q-item-section center side>
+                  <div class="text-grey-8 q-gutter-xs">
+                    <q-btn
+                      flat dense round
+                      size="12px"
+                      color="grey-8"
+                      icon="tune"
+                      :disable="!plugin.has_config"
+                      @click="openPluginInfo(plugin.plugin_id, 'settings')">
+                      <q-tooltip class="bg-white text-primary">
+                        {{ $t('tooltips.configureForThisLibrary') }}
+                      </q-tooltip>
+                    </q-btn>
+                    <q-btn
+                      flat dense round
+                      size="12px"
+                      color="negative"
+                      icon="remove_circle_outline"
+                      @click="removePluginFromList(index)">
+                      <q-tooltip class="bg-white text-primary">
+                        {{ $t('tooltips.removeFromThisLibrary') }}
+                      </q-tooltip>
+                    </q-btn>
                   </div>
+                </q-item-section>
 
-                </q-list>
-
-                <q-bar class="bg-transparent q-mb-sm">
-                  <q-space/>
-                  <q-btn
-                    round
-                    flat
-                    color="primary"
-                    icon="add"
-                    @click="selectPluginFromList">
-                    <q-tooltip class="bg-white text-primary">{{
-                        $t('components.settings.library.addPluginToThisLibrary')
-                      }}
-                    </q-tooltip>
-                  </q-btn>
-                </q-bar>
-              </div>
-
-              <div class="text-h6">
-                {{ $t('components.settings.library.pluginFlow') }}
-              </div>
-
-              <LibraryConfigurePluginFlowList v-bind:libraryId="libraryId" :key="componentKey"/>
+              </q-item>
+            </div>
 
-            </q-card-section>
+          </q-list>
 
-          </q-card>
+          <q-bar class="bg-transparent q-mb-sm">
+            <q-space/>
+            <q-btn
+              round
+              flat
+              color="primary"
+              icon="add"
+              @click="selectPluginFromList">
+              <q-tooltip class="bg-white text-primary">{{
+                  $t('components.settings.library.addPluginToThisLibrary')
+                }}
+              </q-tooltip>
+            </q-btn>
+          </q-bar>
+        </div>
 
+        <div class="text-h6">
+          {{ $t('components.settings.library.pluginFlow') }}
         </div>
 
+        <LibraryConfigurePluginFlowList v-bind:libraryId="libraryId" :key="componentKey"/>
+
       </q-card-section>
 
     </q-card>
 
-    <PluginInfo v-bind:showPluginSettings="showPluginSettings"
-                v-bind:libraryId="libraryId"
-                v-on:hide="closePluginInfo"/>
+  </div>
 
-  </q-dialog>
 </template>
 
 <script>
 import axios from "axios";
 import { getUnmanicApiUrl } from "src/js/unmanicGlobals";
 import { ref } from "vue";
-import PluginInfo from "components/PluginInfo";
 import DirectoryBrowserDialog from "components/DirectoryBrowserDialog";
 import PluginSelectorDialog from "components/PluginSelectorDialog";
 import LibraryConfigurePluginFlowList from "components/LibraryConfigurePluginFlowList";
 import JsonImportExportDialog from "components/JsonImportExportDialog";
 import { Loading } from "quasar";
+import PluginInfoDialog from "components/dialogs/PluginInfoDialog";
 
 export default {
-  name: 'LibraryConfigureDialog',
-  components: { LibraryConfigurePluginFlowList, PluginInfo },
+  name: 'LibraryConfigForm',
+  components: { LibraryConfigurePluginFlowList },
   props: {
-    dialogHeader: {
-      type: String,
-      default: ' --- header --- '
-    },
     libraryId: {
       type: Number,
       default: 0
     }
   },
-  emits: [
-    // REQUIRED
-    'ok', 'hide', 'path'
-  ],
-  methods: {
-    // following method is REQUIRED
-    // (don't change its name --> "show")
-    show() {
-      this.$refs.libraryConfigureDialogRef.show();
-      this.fetchLibraryConfig(this.libraryId);
-    },
+  data: function () {
+    return {
+      /*
+      Required data:
+        - isLoading
+        - isSaved
+      */
+      isLoading: false,
+      isSaved: true,
 
-    // following method is REQUIRED
-    // (don't change its name --> "hide")
+      currentID: ref(null),
+      locked: ref(false),
+      name: ref(''),
+      path: ref(''),
+      enableReceiveRemoteFilesOnly: ref(false),
+      enableScanner: ref(false),
+      enableInotify: ref(false),
+      priorityScore: ref(0),
+      newTag: ref(''),
+      tags: ref([]),
+      enabledPlugins: ref([]),
+      componentKey: 1,
+      showLoading: ref(false),
+    }
+  },
+  mounted() {
+    this.fetchLibraryConfig(this.libraryId);
+  },
+  methods: {
+    /*
+    Required methods:
+      - hide()
+      - save()
+      - cancel()
+    */
     hide() {
-      this.$refs.libraryConfigureDialogRef.hide();
+      return true;
     },
-
-    onDialogHide() {
-      // required to be emitted
-      // when QDialog emits "hide" event
-      this.$emit('ok', {});
-      this.$emit('hide');
+    save() {
+      return this.saveLibraryConfig();
     },
-
-    beforeDialogHide() {
-      this.saveLibraryConfig();
+    cancel() {
+      return true;
     },
 
     fetchLibraryConfig: function (libraryId) {
       // Fetch from server
       let data = {
         id: libraryId,
       }
@@ -480,15 +415,15 @@
         this.priorityScore = libraryConfig.priority_score;
         this.tags = libraryConfig.tags;
 
         // Plugins
         this.enabledPlugins = response.data.plugins.enabled_plugins;
       });
     },
-    saveLibraryConfig: function () {
+    saveLibraryConfig: async function () {
       let data = {
         library_config: {
           id: this.currentID,
           locked: this.locked,
           name: this.name,
           path: this.path,
           enable_remote_only: this.enableReceiveRemoteFilesOnly,
@@ -497,36 +432,38 @@
           priority_score: this.priorityScore,
           tags: this.tags,
         },
         plugins: {
           enabled_plugins: this.enabledPlugins,
         }
       }
-      axios({
+      return await axios({
         method: 'post',
         url: getUnmanicApiUrl('v2', 'settings/library/write'),
         data: data
       }).then((response) => {
         // Save success, show feedback
         this.$q.notify({
           color: 'positive',
           position: 'top',
           icon: 'cloud_done',
           message: this.$t('notifications.saved'),
           timeout: 200
         })
         this.componentKey += 1;
+        return true;
       }).catch(() => {
         this.$q.notify({
           color: 'negative',
           position: 'top',
           message: this.$t('notifications.failedToSaveSettings'),
           icon: 'report_problem',
           actions: [{ icon: 'close', color: 'white' }]
         })
+        return false;
       });
     },
     addTag: function () {
       if (this.newTag) {
         this.tags[this.tags.length] = this.newTag;
         this.newTag = null;
       }
@@ -587,16 +524,38 @@
         }
       }
       this.enabledPlugins = enabledPluginList;
 
       // Save the current settings
       this.saveLibraryConfig()
     },
-    closePluginInfo: function () {
-      this.showPluginSettings = '';
+    openPluginInfo: function (pluginId, tab) {
+      // Ensure we have the info for the plugin to be displayed
+      if (pluginId === '') {
+        // Display error notification
+        this.$q.notify({
+          color: 'negative',
+          position: 'top',
+          message: 'An error was encountered while attempting to open plugin info',
+          icon: 'report_problem',
+          actions: [{ icon: 'close', color: 'white' }]
+        })
+        return
+      }
+      // Display the dialog
+      this.$q.dialog({
+        component: PluginInfoDialog,
+        componentProps: {
+          pluginId: pluginId,
+          startTab: (tab === 'settings') ? 'settings' : 'info',
+          libraryId: this.currentID,
+        },
+      }).onOk((payload) => {
+      }).onDismiss(() => {
+      })
     },
     exportPluginConfig: function () {
       let data = {
         id: this.currentID,
       }
       axios({
         method: 'post',
@@ -721,15 +680,16 @@
         let importString = JSON.stringify(configData, null, 2);
         // Setting the ID to 0 will create a new library
         this.currentID = 0;
         // Import the exported data
         this.importData(importString, true);
         // Reset the current ID and hide dialog
         this.currentID = this.libraryId;
-        this.hide();
+        // Hide dialog via the parent component
+        this.$emit('requestHide')
       }).catch(() => {
         this.$q.notify({
           color: 'negative',
           position: 'top',
           message: this.$t('notifications.failedToSaveSettings'),
           icon: 'report_problem',
           actions: [{ icon: 'close', color: 'white' }]
@@ -739,29 +699,14 @@
   },
   watch: {
     libraryId(value) {
       if (value.length > 0) {
         this.currentID = this.libraryId;
       }
     }
-  },
-  data: function () {
-    return {
-      maximizedToggle: true,
-      showPluginSettings: ref(''),
-      currentID: ref(null),
-      locked: ref(false),
-      name: ref(''),
-      path: ref(''),
-      enableReceiveRemoteFilesOnly: ref(false),
-      enableScanner: ref(false),
-      enableInotify: ref(false),
-      priorityScore: ref(0),
-      newTag: ref(''),
-      tags: ref([]),
-      enabledPlugins: ref([]),
-      componentKey: 1,
-      showLoading: ref(false),
-    }
   }
 }
 </script>
+
+<style scoped>
+
+</style>
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/FooterData.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/FooterData.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/LoginDialog.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/LoginDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/PluginInfo.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/dialogs/PluginInfoDialog.vue`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,79 @@
 <template>
-
+  <!--
+    TODO:
+      - Configure mobile view such that the form elements on the settings tab are not padded
+      - Fix header wrapping on mobile view
+    -->
+
+  <!-- START DIALOG CONFIG
+  Right fullscreen pop-up
+  Note: Update template q-dialog ref="" value
+
+  All Platforms:
+   - Swipe right to dismiss
+  Desktop:
+   - Width 700px
+   - Minimise button top-right
+  Mobile:
+   - Full screen
+   - Back button top-left
+  -->
   <q-dialog
-    v-model="pluginInfoShowDialog"
-    full-height
+    ref="pluginInfoDialogRef"
     :maximized="$q.platform.is.mobile"
-    :transition-show="($q.platform.is.mobile) ? 'slide-left' : 'scale'"
-    :transition-hide="($q.platform.is.mobile) ? 'slide-right' : 'scale'"
-    :position="($q.platform.is.mobile) ? 'right' : 'standard'"
+    :transition-show="$q.platform.is.mobile ? 'jump-left' : 'slide-left'"
+    :transition-hide="$q.platform.is.mobile ? 'jump-right' : 'slide-right'"
+    full-height
+    position="right"
     @before-hide="beforeDialogHide"
     @hide="onDialogHide">
 
     <q-card
-      style="width:1200px; max-width: 95vw;">
+      v-touch-swipe.touch.right="hide"
+      :style="$q.platform.is.mobile ? 'max-width: 100vw;' : 'max-width: 95vw;'"
+      style="width:2000px;">
+
       <q-card-section class="bg-card-head">
         <div class="row items-center no-wrap">
-          <div class="col">
-            <div class="text-h6 text-secondary">
-              <q-icon name="extension"/>
-              {{ header }}
-            </div>
-          </div>
-
-          <div class="col-auto">
+          <div
+            v-if="$q.platform.is.mobile"
+            class="col">
             <q-btn
-              v-if="!$q.platform.is.mobile"
               color="grey-7"
               dense
               round
               flat
-              icon="close_fullscreen" v-close-popup>
-              <q-tooltip class="bg-white text-primary">{{ $t('tooltips.close') }}</q-tooltip>
+              icon="arrow_back"
+              v-close-popup>
             </q-btn>
+          </div>
+
+          <div class="col">
+            <div class="text-h6 text-blue-10">
+              {{ dialogHeader }}
+            </div>
+          </div>
+
+          <div
+            v-if="!$q.platform.is.mobile"
+            class="col-auto">
             <q-btn
-              v-else
               color="grey-7"
               dense
               round
               flat
-              icon="arrow_forward" v-close-popup>
+              icon="arrow_forward"
+              v-close-popup>
               <q-tooltip class="bg-white text-primary">{{ $t('tooltips.close') }}</q-tooltip>
             </q-btn>
           </div>
         </div>
       </q-card-section>
+      <!-- END DIALOG CONFIG -->
 
       <q-tabs
         v-if="settings.length > 0"
         v-model="tab"
         align="left"
         class="text-primary">
         <q-tab
@@ -164,112 +191,156 @@
                   bordered
                   class="q-pa-sm"
                   style="width:100%">
 
                   <q-card-section class="q-pt-none">
 
                     <q-list
-                      v-if="settings.length > 0"
-                      separator>
+                      v-if="settings.length > 0">
                       <q-item
                         v-for="item in settings"
-                        :class="item.display"
+                        :class="item.sub_setting ? item.display + ' sub-setting': item.display"
                         :key="item.key_id"
-                        class="q-py-lg"
+                        class="q-py-sm"
                         v-bind="item">
 
                         <!-- Text input -->
                         <q-item-section
                           v-if="item.input_type === 'text'">
-                          <q-input filled v-model="item.value" :label="item.label" :placeholder="item.label"/>
+                          <q-input filled v-model="item.value"
+                                   :bottom-slots="item.description.length > 0"
+                                   :disable="item.display === 'disabled'"
+                                   :label="item.label"
+                                   :placeholder="item.label">
+                            <template v-slot:hint v-if="item.description.length > 0">
+                              {{ item.description }}
+                            </template>
+                          </q-input>
+                          <q-tooltip v-if="item.tooltip" anchor="bottom start" self="top start">
+                            {{ item.tooltip }}
+                          </q-tooltip>
                         </q-item-section>
 
                         <!-- Textarea input -->
                         <q-item-section
                           v-if="item.input_type === 'textarea'">
-                          <q-input filled type="textarea" v-model="item.value" :label="item.label"/>
+                          <q-input filled v-model="item.value"
+                                   type="textarea"
+                                   :bottom-slots="item.description.length > 0"
+                                   :disable="item.display === 'disabled'"
+                                   :label="item.label">
+                            <template v-slot:hint v-if="item.description.length > 0">
+                              {{ item.description }}
+                            </template>
+                          </q-input>
+                          <q-tooltip v-if="item.tooltip" anchor="bottom start" self="top start">
+                            {{ item.tooltip }}
+                          </q-tooltip>
                         </q-item-section>
 
                         <!-- Checkbox input -->
                         <q-item-section
-                          @click="item.value = !item.value"
                           v-if="item.input_type === 'checkbox'">
                           <div
+                            @click="item.value = !item.value"
                             :style="$q.dark.isActive ? 'background:rgba(255,255,255,.07)' : 'background:rgba(0, 0, 0, 0.05);'"
                             class="q-pa-sm rounded-borders">
                             <q-checkbox
                               @update:model-value="value=>{updateAndTriggerSave(item.key_id, value)}"
                               v-model="item.value"
+                              :disable="item.display === 'disabled'"
                               :label="item.label"/>
                           </div>
+                          <div v-if="item.description.length > 0"
+                               class="checkbox-hint">
+                            {{ item.description }}
+                          </div>
+                          <q-tooltip v-if="item.tooltip" anchor="bottom start" self="top start">
+                            {{ item.tooltip }}
+                          </q-tooltip>
                         </q-item-section>
 
                         <!-- Select input -->
                         <q-item-section
                           v-if="item.input_type === 'select'">
                           <q-select
                             @update:model-value="value=>{updateAndTriggerSave(item.key_id, value)}"
                             filled
                             v-model="item.value"
                             emit-value
                             map-options
+                            :bottom-slots="item.description.length > 0"
                             :options="item.select_options"
                             :option-value="opt => Object(opt) === opt && 'value' in opt ? opt.value : null"
                             :option-label="opt => Object(opt) === opt && 'label' in opt ? opt.label : '- Null -'"
-                            :label="item.label"/>
+                            :disable="item.display === 'disabled'"
+                            :label="item.label">
+                            <template v-slot:hint v-if="item.description.length > 0">
+                              {{ item.description }}
+                            </template>
+                          </q-select>
+                          <q-tooltip v-if="item.tooltip" anchor="bottom start" self="top start">
+                            {{ item.tooltip }}
+                          </q-tooltip>
                         </q-item-section>
 
                         <!-- Slider input -->
                         <q-item-section
-                          :class="item.display"
-                          avatar
-                          v-if="item.input_type === 'slider'">
-                          <q-icon color="primary" name="chevron_right"/>
-                        </q-item-section>
-                        <q-item-section
-                          :class="item.display"
                           v-if="item.input_type === 'slider'">
-                          <q-slider
-                            v-model="item.value"
-                            :min="Number(item.slider_options.min)"
-                            :max="Number(item.slider_options.max)"
-                            :step="Number(item.slider_options.step)"
-                            label
-                            :label-value="item.label + ': ' + item.value + item.slider_options.suffix"
-                            label-always
-                            color="primary"
-                          />
-                        </q-item-section>
-                        <q-item-section
-                          :class="item.display"
-                          avatar
-                          v-if="item.input_type === 'slider'">
-                          <q-icon color="primary" name="chevron_left"/>
+                          <q-item class="q-pa-none q-ma-none">
+                            <q-item-section :class="item.display" avatar>
+                              <q-icon color="primary" name="chevron_right"/>
+                            </q-item-section>
+                            <q-item-section class="q-pt-lg q-pb-none" :class="item.display">
+                              <q-slider
+                                v-model="item.value"
+                                :min="Number(item.slider_options.min)"
+                                :max="Number(item.slider_options.max)"
+                                :step="Number(item.slider_options.step)"
+                                :disable="item.display === 'disabled'"
+                                label
+                                :label-value="item.label + ': ' + item.value + item.slider_options.suffix"
+                                :hint="item.description"
+                                label-always
+                                color="primary"
+                              />
+                            </q-item-section>
+                            <q-item-section :class="item.display" avatar>
+                              <q-icon color="primary" name="chevron_left"/>
+                            </q-item-section>
+                          </q-item>
+                          <div v-if="item.description.length > 0"
+                               class="checkbox-hint">
+                            {{ item.description }}
+                          </div>
                         </q-item-section>
 
                         <!-- Directory browser input -->
                         <q-item-section
                           v-if="item.input_type === 'browse_directory'">
-
                           <q-input
                             readonly
                             filled
                             color="primary"
                             v-model="item.value"
+                            :disable="item.display === 'disabled'"
                             :label="item.label"
                             :placeholder="item.label"
+                            :hint="item.description"
                             @click="updateWithDirectoryBrowser(item)">
                             <template v-slot:append>
                               <q-icon
                                 @click="updateWithDirectoryBrowser(item)"
                                 class="cursor-pointer"
                                 name="folder_open"/>
                             </template>
                           </q-input>
-
+                          <q-tooltip v-if="item.tooltip" anchor="bottom start" self="top start">
+                            {{ item.tooltip }}
+                          </q-tooltip>
                         </q-item-section>
 
 
                       </q-item>
                     </q-list>
                   </q-card-section>
                 </q-card>
@@ -286,115 +357,146 @@
               </div>
             </div>
           </div>
         </q-tab-panel>
       </q-tab-panels>
 
     </q-card>
-  </q-dialog>
 
+  </q-dialog>
 </template>
 
 <script>
-import { ref } from "vue";
+/*
+tab          - The tab to display first ['info', 'settings']
+*/
+
 import axios from "axios";
 import { getUnmanicApiUrl } from "src/js/unmanicGlobals";
+import { useI18n } from "vue-i18n";
+import { ref } from "vue";
 import { markdownToHTML } from "src/js/markupParser";
 import DirectoryBrowserDialog from "components/DirectoryBrowserDialog";
 
 export default {
-  name: 'PluginInfo',
-  components: {},
-  data() {
-    return {
-      header: ref(''),
-      pluginInfoShowDialog: ref(false),
-      tab: ref('info'),
-      id: ref(null),
-      pluginId: ref(''),
-      icon: ref(null),
-      name: ref(null),
-      description: ref(null),
-      tags: ref(null),
-      author: ref(null),
-      version: ref(null),
-      changelog: ref(null),
-      status: ref(null),
-      settings: ref([]),
-      originalSettings: ref([]),
-    }
-  },
-  watch: {
-    showPluginInfo(value) {
-      if (value.length > 0) {
-        this.selectedPluginId = value;
-        this.setHeader('info');
-        this.fetchPluginInfo();
-        this.pluginInfoShowDialog = true;
-      } else {
-        this.pluginInfoShowDialog = false;
-        this.resetData();
-      }
+  name: 'LinkConfigureDialog',
+  props: {
+    pluginId: {
+      type: String
     },
-    showPluginSettings(value) {
-      if (value.length > 0) {
-        this.selectedPluginId = value;
-        this.tab = 'settings';
-        this.setHeader('settings');
-        this.fetchPluginInfo();
-        this.pluginInfoShowDialog = true;
-      } else {
-        this.pluginInfoShowDialog = false;
-        this.resetData();
-      }
+    startTab: {
+      type: String,
+      default: 'info'
+    },
+    viewingRemoteInfo: {
+      type: Boolean,
+      required: false,
+    },
+    libraryId: {
+      type: Number,
+      required: false,
     }
   },
+  emits: [
+    // REQUIRED
+    'ok', 'hide', 'path'
+  ],
   methods: {
-    resetData() {
-      this.selectedPluginId = '';
-      this.tab = 'info';
-      this.id = null;
-      this.pluginId = '';
-      this.icon = null;
-      this.name = null;
-      this.description = null;
-      this.tags = null;
-      this.author = null;
-      this.version = null;
-      this.changelog = null;
-      this.status = null;
-      this.settings = [];
-      this.currentSettings = [];
+    // following method is REQUIRED
+    // (don't change its name --> "show")
+    show() {
+      this.$refs.pluginInfoDialogRef.show();
+      this.tab = this.startTab;
+      this.setHeader(this.startTab);
+      this.fetchPluginData();
+    },
+
+    // following method is REQUIRED
+    // (don't change its name --> "hide")
+    hide() {
+      this.$refs.pluginInfoDialogRef.hide();
+    },
+
+    onDialogHide() {
+      // required to be emitted
+      // when QDialog emits "hide" event
+      this.$emit('ok', {})
+      this.$emit('hide')
+    },
+
+    beforeDialogHide: function () {
+      // Execute any functions prior to closing the dialog
+      this.ensurePluginSettingsAreSaved();
     },
+
     setHeader(tab) {
       if (tab === 'info') {
-        this.header = this.$t('headers.pluginInfo');
+        this.dialogHeader = this.$t('headers.pluginInfo');
       } else {
         if (this.libraryId) {
-          this.header = this.$t('headers.libraryPluginConfig');
+          this.dialogHeader = this.$t('headers.libraryPluginConfig');
         } else {
-          this.header = this.$t('headers.globalPluginConfig');
+          this.dialogHeader = this.$t('headers.globalPluginConfig');
         }
       }
     },
+
+    fetchPluginData: function () {
+      // Fetch from server
+      let postData = {
+        plugin_id: this.pluginId,
+        prefer_local: true,
+      }
+      if (this.viewingRemoteInfo) {
+        postData.prefer_local = false;
+      }
+      if (this.libraryId) {
+        postData.library_id = this.libraryId;
+      }
+      axios({
+        method: 'post',
+        url: getUnmanicApiUrl('v2', 'plugins/info'),
+        data: postData
+      }).then((response) => {
+        this.id = response.data.id
+        this.icon = response.data.icon
+        this.name = response.data.name
+        this.tags = response.data.tags
+        this.author = response.data.author
+        this.version = response.data.version
+        this.changelog = response.data.changelog
+        this.status = response.data.status
+        if (!this.viewingRemoteInfo) {
+          this.settings = response.data.settings
+          // Create a copy of the settings object for the "current settings".
+          // We will compare this later on.
+          this.currentSettings = JSON.parse(JSON.stringify(response.data.settings))
+        }
+        // Parse the changelog
+        this.changelog = markdownToHTML(response.data.changelog);
+        // Parse the description
+        this.description = markdownToHTML(response.data.description);
+      });
+    },
+
     resetPluginLibraryConfig() {
       let data = {
         plugin_id: this.pluginId
       }
       if (this.libraryId) {
         data.library_id = this.libraryId;
       }
       axios({
         method: 'post',
         url: getUnmanicApiUrl('v2', 'plugins/settings/reset'),
         data: data
       }).then((response) => {
         // Save success
-        // Refresh plugin info
-        this.fetchPluginInfo();
+        // Refresh plugin data
+        this.fetchPluginData();
         // Show feedback
         this.$q.notify({
           color: 'positive',
           position: 'top',
           message: this.$t('notifications.SavedPluginSettings'),
           icon: 'check_circle',
           timeout: 200,
@@ -408,59 +510,18 @@
           position: 'top',
           message: this.$t('notifications.failedToSavePluginSettings'),
           icon: 'report_problem',
           actions: [{ icon: 'close', color: 'white' }]
         })
       });
     },
-    fetchPluginInfo() {
-      console.debug('Fetching info for ' + this.selectedPluginId)
-      // Fetch from server
-      let data = {
-        plugin_id: this.selectedPluginId,
-        prefer_local: true,
-      }
-      if (this.viewingRemoteInfo) {
-        data.prefer_local = false;
-      }
-      if (this.libraryId) {
-        data.library_id = this.libraryId;
-      }
-      axios({
-        method: 'post',
-        url: getUnmanicApiUrl('v2', 'plugins/info'),
-        data: data
-      }).then((response) => {
-        this.id = response.data.id
-        this.pluginId = response.data.plugin_id
-        this.icon = response.data.icon
-        this.name = response.data.name
-        this.tags = response.data.tags
-        this.author = response.data.author
-        this.version = response.data.version
-        this.changelog = response.data.changelog
-        this.status = response.data.status
-        if (!this.viewingRemoteInfo) {
-          this.settings = response.data.settings
-          // Create a copy of the settings object for the "current settings".
-          // We will compare this later on.
-          this.currentSettings = JSON.parse(JSON.stringify(response.data.settings))
-        }
-
-        // Parse the changelog
-        this.changelog = markdownToHTML(response.data.changelog);
-
-        // Parse the description
-        this.description = markdownToHTML(response.data.description);
-      });
-    },
 
     settingsHaveBeenModified() {
       // This is a little complicated than it should be. Bot lists are just arrays.
-      // Therefore we need to loop over both and ensure the key value pairs in each are still the same
+      // Therefore, we need to loop over both and ensure the key value pairs in each are still the same
       // Extract values from settings
       let newSettings = {}
       for (let i = 0; i < this.settings.length; i++) {
         newSettings[this.settings[i].key_id] = this.settings[i].value;
       }
       // Loop over currently saved values and check they are the same
       for (let i = 0; i < this.currentSettings.length; i++) {
@@ -470,30 +531,25 @@
         }
       }
 
       // All parsed settings are the same
       return false;
     },
 
-    beforeDialogHide() {
+    ensurePluginSettingsAreSaved() {
       if (typeof this.currentSettings !== 'undefined') {
         if (this.currentSettings.length > 0) {
           // Only save if settings are different
           if (this.settingsHaveBeenModified()) {
             // Settings have changed since they were last saved... save them again.
             this.savePluginSettings();
           }
         }
       }
     },
-
-    onDialogHide() {
-      this.$emit('hide');
-    },
-
     savePluginSettings: function () {
       console.debug('Fetching info for ' + this.pluginId)
 
       let data = {
         plugin_id: this.pluginId,
         settings: this.settings
       }
@@ -502,16 +558,16 @@
       }
       axios({
         method: 'post',
         url: getUnmanicApiUrl('v2', 'plugins/settings/update'),
         data: data
       }).then((response) => {
         // Save success
-        // Refresh plugin info
-        this.fetchPluginInfo();
+        // Refresh plugin data
+        this.fetchPluginData();
         // Show feedback
         this.$q.notify({
           color: 'positive',
           position: 'top',
           message: this.$t('notifications.SavedPluginSettings'),
           icon: 'check_circle',
           timeout: 200,
@@ -523,23 +579,25 @@
           position: 'top',
           message: this.$t('notifications.failedToSavePluginSettings'),
           icon: 'report_problem',
           actions: [{ icon: 'close', color: 'white' }]
         })
       });
     },
+
     updateAndTriggerSave: function (key, value) {
       for (let i = 0; i < this.settings.length; i++) {
         if (this.settings[i].key_id === key) {
           this.settings[i].value = value;
           break
         }
       }
       this.savePluginSettings()
     },
+
     updateWithDirectoryBrowser: function (input) {
       this.$q.dialog({
         component: DirectoryBrowserDialog,
         // props forwarded to your custom component
         componentProps: {
           dialogHeader: this.$t('headers.selectDirectory'),
           initialPath: input.value,
@@ -548,41 +606,44 @@
       }).onOk((payload) => {
         if (typeof payload.selectedPath !== 'undefined' && payload.selectedPath !== null) {
           input.value = payload.selectedPath
         }
       }).onDismiss(() => {
       })
     }
-
   },
-  props: {
-    showPluginInfo: {
-      type: String,
-      required: false,
-    },
-    showPluginSettings: {
-      type: String,
-      required: false,
-    },
-    viewingRemoteInfo: {
-      type: Boolean,
-      required: false,
-    },
-    libraryId: {
-      type: Number,
-      required: false,
+  watch: {
+    uuid(value) {
+      if (value.length > 0) {
+        this.currentUuid = this.uuid;
+      }
     }
   },
-  setup() {
-    return {}
+  data: function () {
+    return {
+      dialogHeader: ref(''),
+      tab: ref('info'),
+      id: ref(null),
+      icon: ref(null),
+      name: ref(null),
+      description: ref(null),
+      tags: ref(null),
+      author: ref(null),
+      version: ref(null),
+      changelog: ref(null),
+      status: ref(null),
+      settings: ref([]),
+      originalSettings: ref([]),
+    }
   }
 }
 </script>
 
 <style>
+
 span.plugin-changelog * {
   margin-top: 0;
   margin-bottom: 0;
 }
 
 span.plugin-description {
   width: 100%;
@@ -619,8 +680,30 @@
   background: #222;
 }
 
 span.plugin-description hr {
   margin-top: 10px;
   margin-bottom: 10px;
 }
+
+.checkbox-hint {
+  line-height: 1;
+  font-size: 12px;
+  min-height: 20px;
+  color: rgba(0, 0, 0, 0.54);
+  padding: 8px 12px 0;
+  -webkit-backface-visibility: hidden;
+  backface-visibility: hidden;
+}
+
+.q-list--dark .checkbox-hint {
+  color: rgba(255, 255, 255, 0.7);
+}
+
+.sub-setting {
+  margin-left: 30px;
+  padding-top: 8px;
+  padding-left: 8px;
+  border-left: solid thin var(--q-primary);
+}
+
 </style>
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/CompletedTasksTable.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/CompletedTasksTable.vue`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
       title="Completed Tasks"
       :rows="rows"
       :columns="columns"
       row-key="id"
       v-model:pagination="pagination"
       :loading="loading"
       :filter="searchValue"
-      @request="onRequest"
+      @request="fetchCompletedTasks"
       binary-state-sort
       :selected-rows-label="getSelectedString"
       selection="multiple"
       v-model:selected="selected"
     >
       <template v-slot:top-left>
         <div class="row">
@@ -205,146 +205,77 @@
       </q-card-actions>
     </q-card>
   </q-dialog>
 
 </template>
 
 <script>
-import { onMounted, ref, watch } from 'vue';
+import { ref } from 'vue';
 import { getUnmanicApiUrl } from "src/js/unmanicGlobals";
-import { useQuasar } from "quasar";
 import dateTools from "src/js/dateTools";
 import axios from "axios";
 import CompletedTaskLogDialog from "components/CompletedTaskLogDialog";
-import { useI18n } from "vue-i18n";
-import { onUnmounted } from "@vue/runtime-core";
-
-const columns = [
-  {
-    name: 'task_label',
-    label: 'Name',
-    required: true,
-    align: 'left',
-    field: 'name',
-    sortable: true
-  },
-  {
-    name: 'finish_time',
-    label: 'Completed',
-    required: true,
-    align: 'left',
-    field: 'dateTimeCompleted',
-    sortable: true
-  },
-  {
-    name: 'task_success',
-    label: 'Status',
-    required: true,
-    align: 'left',
-    field: 'status',
-    sortable: true
-  },
-  {
-    name: 'details',
-    label: 'Details',
-    required: true,
-    align: 'left',
-    field: 'id',
-    sortable: false
-  }
-]
 
 export default {
-  setup() {
-    const $q = useQuasar();
-    const { t: $t } = useI18n();
-    const rows = ref([])
-    const searchValue = ref('')
-    const statusFilter = ref('all')
-    const statusFilterOptions = [
-      {
-        label: $t('status.all'),
-        value: 'all'
-      },
-      {
-        label: $t('status.success'),
-        value: 'success'
-      },
-      {
-        label: $t('status.failed'),
-        value: 'failed'
-      }
-    ]
-    const sinceDate = ref(null)
-    const beforeDate = ref(null)
-    const loading = ref(false)
-    const pagination = ref({
-      sortBy: 'finish_time',
-      descending: true,
-      page: 1,
-      rowsPerPage: 15,
-      rowsNumber: 10
-    })
-    const selected = ref([]);
-    const selectLibrary = ref(false)
-    const selectedLibraryId = ref(null)
-    const LibraryOptions = ref([])
-
-    let reloadInterval = null;
-
-    function getSelectedString() {
+  props: {
+    initStatusFilter: {
+      type: String,
+      default: 'all',
+      required: false
+    }
+  },
+  methods: {
+    getSelectedString: function () {
       let return_value = ''
-      if (selected.value.length !== 0) {
-        return_value = `${selected.value.length} record${selected.value.length > 1 ? 's' : ''} selected of ${rows.value.length}`
+      if (this.selected.length !== 0) {
+        return_value = `${this.selected.length} record${this.selected.length > 1 ? 's' : ''} selected of ${this.rows.length}`
       }
       return return_value
-    }
-
-    function deleteSelected() {
-      if (selected.value.length !== 0) {
+    },
+    deleteSelected: function () {
+      if (this.selected.length !== 0) {
         // Fetch the selected row IDs
         let id_list = []
-        for (let i = 0; i < selected.value.length; i++) {
-          let row = selected.value[i];
+        for (let i = 0; i < this.selected.length; i++) {
+          let row = this.selected[i];
           id_list[id_list.length] = row.id;
         }
         // Send those to the backend
         let data = {
           id_list: id_list,
         }
         axios({
           method: 'delete',
           url: getUnmanicApiUrl('v2', 'history/tasks'),
           data: data
         }).then((response) => {
-          onRequest({
-            pagination: pagination.value,
-            searchValue: searchValue.value
+          this.fetchCompletedTasks({
+            pagination: this.pagination,
+            searchValue: this.searchValue
           })
         }).catch(() => {
-          $q.notify({
+          this.$q.notify({
             color: 'negative',
             position: 'top',
             message: 'An error was encountered while requesting the selected tasks be deleted',
             icon: 'report_problem',
             actions: [{ icon: 'close', color: 'white' }]
           })
         })
       } else {
-        $q.notify({
+        this.$q.notify({
           color: 'warning',
           position: 'top',
           message: 'Nothing selected',
           icon: 'report_problem',
           actions: [{ icon: 'close', color: 'white' }]
         })
       }
-    }
-
-    function selectLibraryForRecreateTask() {
+    },
+    selectLibraryForRecreateTask: function () {
       // Fetch current settings
       axios({
         method: 'get',
         url: getUnmanicApiUrl('v2', 'settings/libraries')
       }).then((response) => {
         let libraryPathsList = []
         let defaultSelection;
@@ -354,219 +285,263 @@
             defaultSelection = libraryPath.id
           }
           libraryPathsList[libraryPathsList.length] = {
             label: libraryPath.name,
             value: libraryPath.id,
           }
         }
-        LibraryOptions.value = libraryPathsList;
+        this.LibraryOptions = libraryPathsList;
 
-        // If the list of libraries is only one, then dont bother showing this selector
-        selectedLibraryId.value = 1;
+        // If the list of libraries is only one, then don't bother showing this selector
+        this.selectedLibraryId = 1;
         if (libraryPathsList.length === 1) {
-          selectedLibraryId.value = defaultSelection;
-          addSelectedToPendingTaskList();
+          this.selectedLibraryId = defaultSelection;
+          this.addSelectedToPendingTaskList();
         } else {
-          selectLibrary.value = true;
+          this.selectLibrary = true;
         }
       }).catch(() => {
-        $q.notify({
+        this.$q.notify({
           color: 'negative',
           position: 'top',
-          message: $t('notifications.failedToFetchLibraryList'),
+          message: this.$t('notifications.failedToFetchLibraryList'),
           icon: 'report_problem',
           actions: [{ icon: 'close', color: 'white' }]
         })
       });
-    }
-
-    function addSelectedToPendingTaskList() {
-      if (selected.value.length !== 0) {
+    },
+    addSelectedToPendingTaskList: function () {
+      if (this.selected.length !== 0) {
         // Fetch the selected row IDs
         let id_list = []
-        for (let i = 0; i < selected.value.length; i++) {
-          let row = selected.value[i];
+        for (let i = 0; i < this.selected.length; i++) {
+          let row = this.selected[i];
           id_list[id_list.length] = row.id;
         }
         // Get library ID
-        let library_id = selectedLibraryId.value
+        let library_id = this.selectedLibraryId
         // Send those to the backend
         let data = {
           id_list: id_list,
           library_id: library_id,
         }
         axios({
           method: 'post',
           url: getUnmanicApiUrl('v2', 'history/reprocess'),
           data: data
         }).then((response) => {
-          onRequest({
-            pagination: pagination.value,
-            searchValue: searchValue.value
+          this.fetchCompletedTasks({
+            pagination: this.pagination,
+            searchValue: this.searchValue
           })
         }).catch(() => {
-          $q.notify({
+          this.$q.notify({
             color: 'negative',
             position: 'top',
             message: 'An error was encountered while requesting the selected tasks be added to the pending tasks list',
             icon: 'report_problem',
             actions: [{ icon: 'close', color: 'white' }]
           })
         })
       } else {
-        $q.notify({
+        this.$q.notify({
           color: 'warning',
           position: 'top',
           message: 'Nothing selected',
           icon: 'report_problem',
           actions: [{ icon: 'close', color: 'white' }]
         })
       }
-    }
-
-    function onRequest(props) {
+    },
+    openDetailsDialog: function (id) {
+      this.$q.dialog({
+        component: CompletedTaskLogDialog,
+        // props forwarded to your custom component
+        componentProps: {
+          completedTaskId: id
+        },
+      }).onOk((payload) => {
+      }).onDismiss(() => {
+      })
+    },
+    fetchCompletedTasks: function (props) {
       const { page, rowsPerPage, sortBy, descending } = props.pagination;
-      const searchValue = props.filter;
+      const searchValue = props.searchValue;
 
-      loading.value = true;
+      this.loading = true;
 
       // get all rows if "All" (0) is selected
-      const fetchCount = rowsPerPage === 0 ? pagination.value.rowsNumber : rowsPerPage;
+      const fetchCount = rowsPerPage === 0 ? this.pagination.rowsNumber : rowsPerPage;
 
       // calculate starting row of data
       const startRow = (page - 1) * rowsPerPage;
 
       // Fetch from server
       let data = {
         start: startRow,
         length: fetchCount,
         search_value: searchValue,
-        status: statusFilter.value,
-        after: sinceDate.value,
-        before: beforeDate.value,
+        status: this.statusFilter,
+        after: this.sinceDate,
+        before: this.beforeDate,
         order_by: sortBy,
         order_direction: descending ? 'desc' : 'asc',
       }
       axios({
         method: 'post',
         url: getUnmanicApiUrl('v2', 'history/tasks'),
         data: data
       }).then((response) => {
         // update rowsCount with appropriate value
-        pagination.value.rowsNumber = response.data.recordsFiltered;
+        this.pagination.rowsNumber = response.data.recordsFiltered;
 
         // Set returned data from server results
         const returnedData = [];
         for (let i = 0; i < response.data.results.length; i++) {
           let results = response.data.results[i];
           returnedData[i] = {
             id: results.id,
             name: results.task_label,
             dateTimeCompleted: dateTools.printDateTimeString(results.finish_time),
             status: results.task_success
           }
         }
 
         // clear out existing data and add new
-        rows.value.splice(0, rows.value.length, ...returnedData);
+        this.rows.splice(0, this.rows.length, ...returnedData);
 
         // don't forget to update local pagination object
-        pagination.value.page = page;
-        pagination.value.rowsPerPage = rowsPerPage;
-        pagination.value.sortBy = sortBy;
-        pagination.value.descending = descending;
+        this.pagination.page = page;
+        this.pagination.rowsPerPage = rowsPerPage;
+        this.pagination.sortBy = sortBy;
+        this.pagination.descending = descending;
 
         // ...and turn of loading indicator
-        loading.value = false;
+        this.loading = false;
       }).catch(() => {
-        $q.notify({
+        this.$q.notify({
           color: 'negative',
           position: 'top',
           message: 'An error was encountered while requesting the completed tasks list',
           icon: 'report_problem',
           actions: [{ icon: 'close', color: 'white' }]
         })
       })
     }
-
-    function openDetailsDialog(id) {
-      $q.dialog({
-        component: CompletedTaskLogDialog,
-        // props forwarded to your custom component
-        componentProps: {
-          completedTaskId: id
-        },
-      }).onOk((payload) => {
-      }).onDismiss(() => {
+  },
+  watch: {
+    statusFilter(value) {
+      this.fetchCompletedTasks({
+        pagination: this.pagination,
+        searchValue: this.searchValue
       })
-    }
-
-    onMounted(() => {
-      // get initial data from server (1st page)
-      onRequest({
-        pagination: pagination.value,
-        searchValue: undefined
+    },
+    sinceDate(value) {
+      this.fetchCompletedTasks({
+        pagination: this.pagination,
+        searchValue: this.searchValue
       })
-      reloadInterval = setInterval(() => {
-        onRequest({
-          pagination: pagination.value,
-          searchValue: searchValue.value
-        })
-      }, 10000);
-    })
-
-    onUnmounted(() => {
-      if (reloadInterval != null) {
-        clearInterval(reloadInterval);
-      }
-    })
-
-    // Monitor the status filter for changes
-    watch(statusFilter, (currentValue, oldValue) => {
-      onRequest({
-        pagination: pagination.value,
-        searchValue: searchValue.value
+    },
+    beforeDate(value) {
+      this.fetchCompletedTasks({
+        pagination: this.pagination,
+        searchValue: this.searchValue
       })
-    });
+    },
+  },
+  mounted() {
+    // Set default values
+    this.statusFilter = this.initStatusFilter;
+
+    // get initial data from server (1st page)
+    this.fetchCompletedTasks({
+      pagination: this.pagination,
+      searchValue: undefined
+    })
 
-    // Monitor the sinceDate date/time filter for changes
-    watch(sinceDate, (currentValue, oldValue) => {
-      onRequest({
-        pagination: pagination.value,
-        searchValue: searchValue.value
+    // TODO: Remove on unmount
+    this.reloadInterval = setInterval(() => {
+      this.fetchCompletedTasks({
+        pagination: this.pagination,
+        searchValue: this.searchValue
       })
-    });
+    }, 10000);
+  },
+  unmounted() {
+    if (this.reloadInterval != null) {
+      clearInterval(this.reloadInterval);
+    }
+  },
+  data: function () {
+    return {
+      reloadInterval: ref(null),
+      loading: ref(false),
 
-    // Monitor the beforeDate date/time filter for changes
-    watch(beforeDate, (currentValue, oldValue) => {
-      onRequest({
-        pagination: pagination.value,
-        searchValue: searchValue.value
-      })
-    });
+      columns: ref([
+        {
+          name: 'task_label',
+          label: 'Name',
+          required: true,
+          align: 'left',
+          field: 'name',
+          sortable: true
+        },
+        {
+          name: 'finish_time',
+          label: 'Completed',
+          required: true,
+          align: 'left',
+          field: 'dateTimeCompleted',
+          sortable: true
+        },
+        {
+          name: 'task_success',
+          label: 'Status',
+          required: true,
+          align: 'left',
+          field: 'status',
+          sortable: true
+        },
+        {
+          name: 'details',
+          label: 'Details',
+          required: true,
+          align: 'left',
+          field: 'id',
+          sortable: false
+        }
+      ]),
 
-    return {
-      selected,
-      searchValue,
-      statusFilter,
-      statusFilterOptions,
-      sinceDate,
-      beforeDate,
-      loading,
-      pagination,
-      columns,
-      rows,
-
-      selectLibrary,
-      selectedLibraryId,
-      LibraryOptions,
-
-      getSelectedString,
-      onRequest,
-      deleteSelected,
-      selectLibraryForRecreateTask,
-      addSelectedToPendingTaskList,
-      openDetailsDialog
+      rows: ref([]),
+      searchValue: ref(''),
+      statusFilter: ref('all'),
+      statusFilterOptions: [
+        {
+          label: this.$t('status.all'),
+          value: 'all'
+        },
+        {
+          label: this.$t('status.success'),
+          value: 'success'
+        },
+        {
+          label: this.$t('status.failed'),
+          value: 'failed'
+        }
+      ],
+      sinceDate: ref(null),
+      beforeDate: ref(null),
+      pagination: ref({
+        sortBy: 'finish_time',
+        descending: true,
+        page: 1,
+        rowsPerPage: 15,
+        rowsNumber: 10
+      }),
+      selected: ref([]),
+      selectLibrary: ref(false),
+      selectedLibraryId: ref(null),
+      LibraryOptions: ref([]),
     }
   }
 }
 </script>
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/WorkerProgressStatus.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/WorkerProgressStatus.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/ThemeSwitch.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/ThemeSwitch.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/DirectoryBrowserDialog.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/DirectoryBrowserDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/LibraryConfigurePluginFlowList.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/LibraryConfigurePluginFlowList.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/components/CompletedTasks.vue` & `unmanic-0.2.4/unmanic/webserver/frontend/src/components/CompletedTasks.vue`

 * *Files 7% similar despite different names*

```diff
@@ -125,15 +125,15 @@
               </div>
             </div>
           </q-card-section>
 
           <q-card-section class="q-pt-none">
 
             <div class="q-pa-md">
-              <CompletedTasksTable/>
+              <CompletedTasksTable :initStatusFilter="completedTasksPopupInitStatusFilter"/>
             </div>
 
           </q-card-section>
 
         </q-card>
       </q-dialog>
     </q-card-section>
@@ -144,17 +144,28 @@
 <script>
 import { defineComponent, ref } from "vue";
 import CompletedTasksTable from "components/CompletedTasksTable";
 
 export default defineComponent({
   name: 'CompletedTasks',
   components: { CompletedTasksTable },
+  mounted() {
+    // Add listeners
+    this.$global.$on(
+      'completedTasksShowFailed',
+      () => {
+        this.completedTasksPopupInitStatusFilter = 'failed'
+        this.completedTasksPopup = true
+      }
+    )
+  },
   data() {
     return {
       completedTasksPopup: ref(false),
+      completedTasksPopupInitStatusFilter: ref('all'),
     }
   },
   props: {
     taskList: {
       type: Array,
       required: true
     }
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/js/markupParser.js` & `unmanic-0.2.4/unmanic/webserver/frontend/src/js/markupParser.js`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/js/unmanicWebsocket.js` & `unmanic-0.2.4/unmanic/webserver/frontend/src/js/unmanicWebsocket.js`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/js/dateTools.js` & `unmanic-0.2.4/unmanic/webserver/frontend/src/js/dateTools.js`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/router/routes.js` & `unmanic-0.2.4/unmanic/webserver/frontend/src/router/routes.js`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/router/index.js` & `unmanic-0.2.4/unmanic/webserver/frontend/src/router/index.js`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/index.template.html` & `unmanic-0.2.4/unmanic/webserver/frontend/src/index.template.html`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/assets/logo.png` & `unmanic-0.2.4/unmanic/webserver/frontend/src/assets/logo.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/assets/logo-lg.png` & `unmanic-0.2.4/unmanic/webserver/frontend/src/assets/logo-lg.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/assets/quasar-logo-vertical.svg` & `unmanic-0.2.4/unmanic/webserver/frontend/src/assets/quasar-logo-vertical.svg`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/assets/unmanic-logo-white.png` & `unmanic-0.2.4/unmanic/webserver/frontend/src/assets/unmanic-logo-white.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/assets/bg-md1.jpg` & `unmanic-0.2.4/unmanic/webserver/frontend/src/assets/bg-md1.jpg`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/assets/coffee-btn-image.png` & `unmanic-0.2.4/unmanic/webserver/frontend/src/assets/coffee-btn-image.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/boot/axios.js` & `unmanic-0.2.4/unmanic/webserver/frontend/src/boot/axios.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -24,9 +24,10 @@
 
     app.config.globalProperties.$api = api
     // ^ ^ ^ this will allow you to use this.$api (for Vue Options API form)
     //       so you can easily perform requests against your app's API
 })
 
 export {
+    axios,
     api
 }
```

### Comparing `unmanic-0.2.3/unmanic/webserver/frontend/src/boot/i18n.js` & `unmanic-0.2.4/unmanic/webserver/frontend/src/boot/i18n.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
 import {
     createI18n
 } from 'vue-i18n'
 import {
     LocalStorage
 } from 'quasar'
 
-// Dont import messages from the directory... Read them from the JSON files in the language directory
+// Don't import messages from the directory... Read them from the JSON files in the language directory
 //import messages from 'src/i18n'
 
 function loadLocaleInfo() {
     const locales = require.context('src/language', true, /(^|\/)[A-Za-z0-9_,\s-]+\.json$/i)
     const messages = {}
     locales.keys().forEach(key => {
         const matched = key.match(/([A-Za-z0-9_-]+)\./i)
@@ -38,14 +38,15 @@
     // Default to English
     configuredLocale = 'en';
 }
 
 const i18n = createI18n({
     locale: configuredLocale,
     fallbackLocale: 'en',
+    silentTranslationWarn: true,
     messages
 })
 
 export default boot(({
     app
 }) => {
     // Set i18n instance on app
```

### Comparing `unmanic-0.2.3/unmanic/webserver/templates/global/login-popup.html` & `unmanic-0.2.4/unmanic/webserver/templates/global/login-popup.html`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/templates/global/support-future-development.html` & `unmanic-0.2.4/unmanic/webserver/templates/global/support-future-development.html`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/templates/global/insufficient-permissions.html` & `unmanic-0.2.4/unmanic/webserver/templates/global/insufficient-permissions.html`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/helpers/completed_tasks.py` & `unmanic-0.2.4/unmanic/webserver/helpers/completed_tasks.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/helpers/__init__.py` & `unmanic-0.2.4/unmanic/webserver/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/helpers/plugins.py` & `unmanic-0.2.4/unmanic/webserver/helpers/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,17 +222,20 @@
         for key in plugin_settings:
             form_input = {
                 "key_id":         hashlib.md5(key.encode('utf8')).hexdigest(),
                 "key":            key,
                 "value":          plugin_settings.get(key),
                 "input_type":     None,
                 "label":          None,
+                "description":    None,
+                "tooltip":        None,
                 "select_options": [],
                 "slider_options": {},
                 "display":        "visible",
+                "sub_setting":    False,
             }
 
             plugin_setting_meta = plugin_settings_meta.get(key, {})
 
             # Set input type for form
             form_input['input_type'] = plugin_setting_meta.get('input_type', None)
             if not form_input['input_type']:
@@ -250,20 +253,27 @@
                 "browse_directory",
             ]
             if form_input['input_type'] not in supported_input_types:
                 form_input['input_type'] = "text"
 
             # Set input display options
             form_input['display'] = plugin_setting_meta.get('display', 'visible')
+            form_input['sub_setting'] = plugin_setting_meta.get('sub_setting', False)
 
             # Set input label text
             form_input['label'] = plugin_setting_meta.get('label', None)
             if not form_input['label']:
                 form_input['label'] = key
 
+            # Set input description text
+            form_input['description'] = plugin_setting_meta.get('description', '')
+
+            # Set input tooltip text
+            form_input['tooltip'] = plugin_setting_meta.get('tooltip', '')
+
             # Set options if form input is select
             if form_input['input_type'] == 'select':
                 form_input['select_options'] = plugin_setting_meta.get('select_options', [])
                 if not form_input['select_options']:
                     # No options are given. Revert back to text input
                     form_input['input_type'] = 'text'
```

### Comparing `unmanic-0.2.3/unmanic/webserver/helpers/settings.py` & `unmanic-0.2.4/unmanic/webserver/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/helpers/documents.py` & `unmanic-0.2.4/unmanic/webserver/helpers/documents.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/helpers/filebrowser.py` & `unmanic-0.2.4/unmanic/webserver/helpers/filebrowser.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/helpers/workers.py` & `unmanic-0.2.4/unmanic/webserver/helpers/workers.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/helpers/pending_tasks.py` & `unmanic-0.2.4/unmanic/webserver/helpers/pending_tasks.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/webserver/downloads.py` & `unmanic-0.2.4/unmanic/webserver/downloads.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/migrations_v1/001_rename_ffmpeg_log_to_log.py` & `unmanic-0.2.4/unmanic/migrations_v1/001_rename_ffmpeg_log_to_log.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/__main__.py` & `unmanic-0.2.4/unmanic/__main__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/service.py` & `unmanic-0.2.4/unmanic/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 """
 import argparse
 import os
 import time
 import queue
 import signal
+import threading
 
 from unmanic import config, metadata
 from unmanic.libs import libraryscanner, unlogger, common, eventmonitor
 from unmanic.libs.db_migrate import Migrations
 from unmanic.libs.scheduler import ScheduledTasksManager
 from unmanic.libs.taskqueue import TaskQueue
 from unmanic.libs.postprocessor import PostProcessor
@@ -82,62 +83,64 @@
     def __init__(self):
         self.threads = []
         self.run_threads = True
         self.db_connection = None
 
         self.developer = None
 
+        self.event = threading.Event()
+
     def start_handler(self, data_queues, task_queue):
         main_logger.info("Starting TaskHandler")
-        handler = TaskHandler(data_queues, task_queue)
+        handler = TaskHandler(data_queues, task_queue, self.event)
         handler.daemon = True
         handler.start()
         self.threads.append({
             'name':   'TaskHandler',
             'thread': handler
         })
         return handler
 
     def start_post_processor(self, data_queues, task_queue):
         main_logger.info("Starting PostProcessor")
-        postprocessor = PostProcessor(data_queues, task_queue)
+        postprocessor = PostProcessor(data_queues, task_queue, self.event)
         postprocessor.daemon = True
         postprocessor.start()
         self.threads.append({
             'name':   'PostProcessor',
             'thread': postprocessor
         })
         return postprocessor
 
     def start_foreman(self, data_queues, settings, task_queue):
         main_logger.info("Starting Foreman")
-        foreman = Foreman(data_queues, settings, task_queue)
+        foreman = Foreman(data_queues, settings, task_queue, self.event)
         foreman.daemon = True
         foreman.start()
         self.threads.append({
             'name':   'Foreman',
             'thread': foreman
         })
         return foreman
 
     def start_library_scanner_manager(self, data_queues):
         main_logger.info("Starting LibraryScannerManager")
-        library_scanner_manager = libraryscanner.LibraryScannerManager(data_queues)
+        library_scanner_manager = libraryscanner.LibraryScannerManager(data_queues, self.event)
         library_scanner_manager.daemon = True
         library_scanner_manager.start()
         self.threads.append({
             'name':   'LibraryScannerManager',
             'thread': library_scanner_manager
         })
         return library_scanner_manager
 
     def start_inotify_watch_manager(self, data_queues, settings):
         if eventmonitor.event_monitor_module:
             main_logger.info("Starting EventMonitorManager")
-            event_monitor_manager = eventmonitor.EventMonitorManager(data_queues)
+            event_monitor_manager = eventmonitor.EventMonitorManager(data_queues, self.event)
             event_monitor_manager.daemon = True
             event_monitor_manager.start()
             self.threads.append({
                 'name':   'EventMonitorManager',
                 'thread': event_monitor_manager
             })
             return event_monitor_manager
@@ -153,15 +156,15 @@
             'name':   'UIServer',
             'thread': uiserver
         })
         return uiserver
 
     def start_scheduled_tasks_manager(self):
         main_logger.info("Starting ScheduledTasksManager")
-        scheduled_tasks_manager = ScheduledTasksManager()
+        scheduled_tasks_manager = ScheduledTasksManager(self.event)
         scheduled_tasks_manager.daemon = True
         scheduled_tasks_manager.start()
         self.threads.append({
             'name':   'ScheduledTasksManager',
             'thread': scheduled_tasks_manager
         })
         return scheduled_tasks_manager
@@ -214,14 +217,15 @@
         self.start_ui_server(data_queues, foreman)
 
         # Start new thread to run the scheduled tasks manager
         self.start_scheduled_tasks_manager()
 
     def stop_threads(self):
         main_logger.info("Stopping all threads")
+        self.event.set()
         for thread in self.threads:
             main_logger.info("Sending thread {} abort signal".format(thread['name']))
             thread['thread'].stop()
         for thread in self.threads:
             main_logger.info("Waiting for thread {} to stop".format(thread['name']))
             thread['thread'].join(10)
             main_logger.info("Thread {} has successfully stopped".format(thread['name']))
@@ -252,20 +256,21 @@
                 except (KeyboardInterrupt, SystemExit) as e:
                     break
         else:
             signal.signal(signal.SIGINT, self.sig_handle)
             signal.signal(signal.SIGTERM, self.sig_handle)
             while self.run_threads:
                 signal.pause()
+                time.sleep(.5)
 
         # Received term signal. Stop everything
         self.stop_threads()
         self.db_connection.stop()
         while not self.db_connection.is_stopped():
-            time.sleep(0.1)
+            time.sleep(.5)
             continue
         main_logger.info("Exit Unmanic")
 
 
 def main():
     parser = argparse.ArgumentParser(description='Unmanic')
     parser.add_argument('--version', action='version',
@@ -295,15 +300,15 @@
         from unmanic.libs.unplugins.pluginscli import PluginsCLI
         plugin_cli = PluginsCLI()
         plugin_cli.run()
 
         # Stop the DB connection
         db_connection.stop()
         while not db_connection.is_stopped():
-            time.sleep(0.1)
+            time.sleep(.2)
             continue
     else:
         # Run the main Unmanic service
         service = Service()
         service.developer = args.dev
         service.run()
```

### Comparing `unmanic-0.2.3/unmanic/__init__.py` & `unmanic-0.2.4/unmanic/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/config.py` & `unmanic-0.2.4/unmanic/config.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/uiserver.py` & `unmanic-0.2.4/unmanic/libs/uiserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 
 class FrontendPushMessages(Queue, metaclass=SingletonType):
     """
     Handles messages passed to the frontend.
 
     Messages are sent as objects. These objects require the following fields:
-        - 'id'          : A unique ID of the message. Prevents messages duplication
+        - 'id'          : A unique ID of the message. Prevent messages duplication
         - 'type'        : The type of message - 'error', 'warning', 'success', or 'info'
         - 'code'        : A code to represent an I18n string for the frontend to display
         - 'message'     : Additional message string that can be appended to the I18n string displayed on the frontend.
         - 'timeout'     : The timeout for this message. If set to 0, then the message will persist until manually dismissed.
 
     """
```

### Comparing `unmanic-0.2.3/unmanic/libs/singleton.py` & `unmanic-0.2.4/unmanic/libs/singleton.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unmodels/installation.py` & `unmanic-0.2.4/unmanic/libs/unmodels/installation.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unmodels/completedtasks.py` & `unmanic-0.2.4/unmanic/libs/unmodels/completedtasks.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unmodels/lib/basemodel.py` & `unmanic-0.2.4/unmanic/libs/unmodels/lib/basemodel.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unmodels/lib/__init__.py` & `unmanic-0.2.4/unmanic/libs/unmodels/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unmodels/libraries.py` & `unmanic-0.2.4/unmanic/libs/unmodels/libraries.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unmodels/completedtaskscommandlogs.py` & `unmanic-0.2.4/unmanic/libs/unmodels/completedtaskscommandlogs.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unmodels/plugins.py` & `unmanic-0.2.4/unmanic/libs/unmodels/plugins.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unmodels/enabledplugins.py` & `unmanic-0.2.4/unmanic/libs/unmodels/enabledplugins.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unmodels/tasks.py` & `unmanic-0.2.4/unmanic/libs/unmodels/tasks.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unmodels/librarypluginflow.py` & `unmanic-0.2.4/unmanic/libs/unmodels/librarypluginflow.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unmodels/workerschedules.py` & `unmanic-0.2.4/unmanic/libs/unmodels/workerschedules.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unmodels/workergroups.py` & `unmanic-0.2.4/unmanic/libs/unmodels/workergroups.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unmodels/tags.py` & `unmanic-0.2.4/unmanic/libs/unmodels/tags.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unmodels/pluginrepos.py` & `unmanic-0.2.4/unmanic/libs/unmodels/pluginrepos.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/common.py` & `unmanic-0.2.4/unmanic/libs/common.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/taskqueue.py` & `unmanic-0.2.4/unmanic/libs/taskqueue.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/__init__.py` & `unmanic-0.2.4/unmanic/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/library.py` & `unmanic-0.2.4/unmanic/libs/library.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         "Stiny Fane", "Driffin", "Andrers", "Beorhtio", "Balda", "Warder", "Bealdu", "Dene", "Andren", "Stephye", "Ealcar",
         "Richye Corby", "Ament Anes", "Tharry", "Germund", "Ralphye Payney"
     ]
     adjectives = [
         "awesome", "adorable", "abounding", "aspiring", "beloved", "blue", "blissful", "creamy", "cavernous", "content",
         "droopy", "excited", "enchanted", "enormous", "extroverted", "exciting", "gullible", "gaseous", "grumpy", "giant",
         "handsome", "hefty", "harmless", "happy", "hairy", "humdrum", "invincible", "illiterate", "inexperienced", "impolite",
-        "illustrious", "impartial", "innocent""jovial", "juvenile", "joyful", "jumpy", "jagged", "joyous", "kooky", "large",
+        "illustrious", "impartial", "innocent", "jovial", "juvenile", "joyful", "jumpy", "jagged", "joyous", "kooky", "large",
         "likeable", "mountainous", "momentous", "minty", "nocturnal", "nautical", "organic", "overcooked", "productive",
         "plush", "polished", "queasy", "quirky", "quintessential", "reminiscent", "remarkable", "ragged", "rowdy", "soggy",
         "sudden", "scandalous", "secretive", "spry", "squiggly", "smooth", "sulky", "scented", "spicy", "sticky", "slushy",
         "symptomatic", "tart", "turbulent", "tiresome", "typical", "xyloid", "xanthic", "zealous", "zany",
     ]
     return "{name}, the {adjective} library".format(name=random.choice(names), adjective=random.choice(adjectives))
```

### Comparing `unmanic-0.2.3/unmanic/libs/unplugins/__init__.py` & `unmanic-0.2.4/unmanic/libs/unplugins/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unplugins/pluginscli.py` & `unmanic-0.2.4/unmanic/libs/unplugins/pluginscli.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,36 +29,43 @@
            OR OTHER DEALINGS IN THE SOFTWARE.
 
 """
 import json
 import logging
 import os
 import re
+import shutil
 import subprocess
 
 import inquirer
+import requests
 
 from . import plugin_types
 
 from unmanic import config
 from unmanic.libs import unlogger, common
 from unmanic.libs.plugins import PluginsHandler
 from unmanic.libs.unplugins import PluginExecutor
 
+home_directory = common.get_home_dir()
+dev_cache_directory = os.path.join(home_directory, '.unmanic', 'dev', 'cache')
+dev_library_directory = os.path.join(home_directory, '.unmanic', 'dev', 'library')
+
 menus = {
     "main":          [
         inquirer.List(
             'cli_action',
             message="What would you like to do?",
             choices=[
                 'List all installed plugins',
                 'Test plugins',
                 'Create new plugin',
                 'Reload all plugins from disk',
                 'Remove plugin',
+                'Install test data',
                 'Exit',
             ],
         ),
     ],
     "create_plugin": [
         inquirer.Text('plugin_id', message="What's the plugin's id"),
         inquirer.Text('plugin_name', message="What's the plugin's name"),
@@ -148,14 +155,21 @@
                 '        - {}%(asctime)s:%(levelname)s:%(name)s - %(message)s{}'.format(BColours.RESULTS, BColours.ENDC),
                 datefmt='%Y-%m-%dT%H:%M:%S'
             )
         )
         unmanic_logging.enable_debugging()
         self.logger = unmanic_logging.get_logger(__class__.__name__)
 
+        self.test_data_modifiers = {
+            "{cache_path}":    dev_cache_directory,
+            "{library_path}":  dev_library_directory,
+            "{test_file_in}":  "Big_Buck_Bunny_1080_10s_30MB_h264.mkv",
+            "{test_file_out}": "Big_Buck_Bunny_1080_10s_30MB_h264-1616571944.7296877-WORKING-1.mkv"
+        }
+
     def _log(self, message, message2='', level="info"):
         message = common.format_message(message, message2)
         getattr(self.logger, level)(message)
 
     def create_new_plugins(self):
         plugin_details = inquirer.prompt(menus.get('create_plugin'))
 
@@ -390,15 +404,16 @@
             if not plugin_types_in_plugin:
                 error = "No runners found in plugin"
                 print("  -- {1}FAILED: {0}{2}".format(error, BColours.FAIL, BColours.ENDC))
                 print()
             else:
                 for plugin_type_in_plugin in plugin_types_in_plugin:
                     print("    {1}{0}{2}".format(plugin_type_in_plugin, BColours.SECTION, BColours.ENDC))
-                    errors = plugin_executor.test_plugin_runner(plugin_id, plugin_type_in_plugin)
+                    errors = plugin_executor.test_plugin_runner(plugin_id, plugin_type_in_plugin,
+                                                                test_data_modifiers=self.test_data_modifiers)
                     if errors:
                         for error in errors:
                             print("        -- {1}FAILED: {0}{2}".format(error, BColours.FAIL, BColours.ENDC))
                     else:
                         print("        -- {}PASSED{} --".format(BColours.OKGREEN, BColours.ENDC))
                     print()
 
@@ -418,15 +433,15 @@
             print()
 
     def test_plugins(self):
         plugin_results = self.__get_installed_plugins()
 
         # Generate menu choices
         all_plugin_details = {}
-        choices = ["Test All Plugins"]
+        choices = ["Configure Testdata", "Test All Plugins"]
         for plugin_details in plugin_results:
             choices.append(plugin_details.get('plugin_id'))
             all_plugin_details[plugin_details.get('plugin_id')] = plugin_details
         choices.append("Go Back")
 
         print()
         default_selection = None
@@ -439,32 +454,90 @@
             )
             selection = inquirer.prompt([plugin_test_inquirer])
 
             # If the 'Go Back' option was given, just return to previous menu
             if not selection or selection.get('selected_plugin') == "Go Back":
                 return
 
+            # Configure test file
+            if selection.get('selected_plugin') == "Configure Testdata":
+                self.configure_test_data()
+                continue
+
             # If 'Test All Plugins' was selected, then run tests against all plugins
             if selection.get('selected_plugin') == "Test All Plugins":
                 self.test_installed_plugins()
+                continue
 
             # Get the details for the selected plugin
             selected_plugin_details = all_plugin_details[selection.get('selected_plugin')]
             # Set that selection as the default for the next time
             default_selection = selection.get('selected_plugin')
             # Test that plugin
             self.test_installed_plugins(plugin_id=selected_plugin_details.get('plugin_id'))
 
+    def configure_test_data(self):
+
+        test_files = []
+        for (dir_path, dir_names, file_names) in os.walk(dev_library_directory):
+            test_files.extend(file_names)
+        print(test_files)
+
+        # Update test file
+        print()
+        print()
+        test_files_inquirer = inquirer.List(
+            'selected_file',
+            message="Which Plugin runner will be used?",
+            choices=test_files,
+        )
+        runner_selection = {}
+        runner_selection = {
+            **inquirer.prompt([test_files_inquirer]),
+            **runner_selection
+        }
+        self.test_data_modifiers['{test_file_in}'] = runner_selection.get('selected_file')
+        split_file_in = os.path.splitext(runner_selection.get('selected_file'))
+        self.test_data_modifiers['{test_file_out}'] = "{}-{}{}".format(split_file_in[0], "WORKING-1", split_file_in[1])
+
+    def install_test_data(self):
+        sample_files = {
+            "Big_Buck_Bunny_1080_10s_30MB_h264.mkv": "https://test-videos.co.uk/vids/bigbuckbunny/mkv/1080/Big_Buck_Bunny_1080_10s_30MB.mkv",
+            "Big_Buck_Bunny_1080_10s_30MB_h264.mp4": "https://test-videos.co.uk/vids/bigbuckbunny/mp4/h264/1080/Big_Buck_Bunny_1080_10s_30MB.mp4",
+            "Big_Buck_Bunny_1080_10s_30MB_av1.mp4":  "https://test-videos.co.uk/vids/bigbuckbunny/mp4/av1/1080/Big_Buck_Bunny_1080_10s_30MB.mp4",
+            "sample-12s.mp3":                        "https://download.samplelib.com/mp3/sample-12s.mp3",
+        }
+        if not os.path.exists(dev_cache_directory):
+            os.makedirs(dev_cache_directory)
+        if not os.path.exists(dev_library_directory):
+            os.makedirs(dev_library_directory)
+        for key in sample_files:
+            library_file = os.path.join(dev_library_directory, key)
+            file_url = sample_files.get(key)
+            print()
+            print("Downloading sample file: '{}'".format(file_url))
+            with requests.get(file_url, stream=True) as r:
+                r.raise_for_status()
+                with open(library_file, 'wb') as f:
+                    for chunk in r.iter_content(chunk_size=None):
+                        if chunk:
+                            f.write(chunk)
+
+            split_file_in = os.path.splitext(key)
+            cache_file = os.path.join(dev_cache_directory, "{}-{}{}".format(split_file_in[0], "WORKING-1", split_file_in[1]))
+            shutil.copyfile(library_file, cache_file)
+
     def main(self, arg):
         switcher = {
             'List all installed plugins':   'list_installed_plugins',
             'Test plugins':                 'test_plugins',
             'Create new plugin':            'create_new_plugins',
             'Reload all plugins from disk': 'reload_plugin_from_disk',
             'Remove plugin':                'remove_plugin',
+            'Install test data':            'install_test_data',
         }
         function = switcher.get(arg, None)
         if function:
             getattr(self, function)()
         else:
             self._log("Invalid selection")
             return
```

### Comparing `unmanic-0.2.3/unmanic/libs/unplugins/executor.py` & `unmanic-0.2.4/unmanic/libs/unplugins/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -458,24 +458,31 @@
         plugin_description = os.path.join(plugin_path, 'description.md')
         if os.path.exists(plugin_description):
             with open(plugin_description, 'r') as f:
                 description = f.readlines()
 
         return description
 
-    def test_plugin_runner(self, plugin_id, plugin_type, test_data=None):
+    def test_plugin_runner(self, plugin_id, plugin_type, test_data=None, test_data_modifiers=None):
+        if test_data is None:
+            test_data = {}
+        if test_data_modifiers is None:
+            test_data_modifiers = {}
         try:
             # Get the path for this plugin
             plugin_path = self.__get_plugin_directory(plugin_id)
 
             # Load this plugin module
             plugin_module = self.__load_plugin_module(plugin_id, plugin_path)
 
             # Get the called runner function for the given plugin type
             plugin_type_meta = self.get_plugin_type_meta(plugin_type)
+            if not test_data:
+                test_data = plugin_type_meta.get_test_data()
+                test_data = plugin_type_meta.modify_test_data(test_data, test_data_modifiers)
             errors = plugin_type_meta.run_data_schema_tests(plugin_id, plugin_module, test_data=test_data)
         except Exception as e:
             self._log("Exception while testing plugin runner for plugin '{}'".format(plugin_id), message2=str(e),
                       level="exception")
             errors = ["Exception encountered while testing runner - {}".format(str(e))]
 
         return errors
```

### Comparing `unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/library_management/file_test.py` & `unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/library_management/file_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,18 +74,18 @@
         "shared_info":               {
             "required": False,
             "type":     dict,
         },
     }
     test_data = {
         'library_id':                1,
-        'path':                      '/library/TEST_FILE.mkv',
+        'path':                      '{library_path}/{test_file_in}',
         'issues':                    [
             {
                 'id':      'format',
-                'message': "File is already in target format - '/library/TEST_FILE.mkv'"
+                'message': "File is already in target format - '{library_path}/{test_file_in}'"
             }
         ],
         'add_file_to_pending_tasks': True,
         'priority_score':            0,
         'shared_info':               {},
     }
```

### Comparing `unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/library_management/__init__.py` & `unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/library_management/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/__init__.py` & `unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/postprocessor/__init__.py` & `unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/postprocessor/task_result.py` & `unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/postprocessor/task_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,19 +73,19 @@
         },
         "source_data":                 {
             "required": False,
             "type":     dict,
         },
     }
     test_data = {
-        'final_cache_path':            '/tmp/unmanic/unmanic_file_conversion-diqxq-1651476950/TEST_FILE-UNMANIC-WORKING-2-1.mkv',
+        'final_cache_path':            '{cache_path}/{test_file_out}',
         'library_id':                  1,
         'task_processing_success':     True,
         'file_move_processes_success': True,
         'destination_files':           [
-            '/library/complete/library/TEST_FILE-UNMANIC.mkv',
+            '{library_path}/complete/library/{test_file_in}',
         ],
         'source_data':                 {
-            'abspath':  '/library/TEST_FILE.mkv',
-            'basename': 'TEST_FILE.mp4',
+            'abspath':  '{library_path}/{test_file_in}',
+            'basename': '{test_file_in}',
         },
     }
```

### Comparing `unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/postprocessor/file_move.py` & `unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/postprocessor/file_move.py`

 * *Files 9% similar despite different names*

```diff
@@ -80,16 +80,16 @@
             "required": True,
             "type":     bool,
         },
     }
     test_data = {
         'library_id':            1,
         'copy_file':             True,
-        'file_in':               '/tmp/unmanic/unmanic_file_conversion-diqxq-1651476950/TEST_FILE-UNMANIC-WORKING-2-1.mkv',
-        'file_out':              '/library/TEST_FILE.mkv',
+        'file_in':               '{cache_path}/{test_file_out}',
+        'file_out':              '{library_path}/{test_file_in}',
         'remove_source_file':    True,
         'run_default_file_copy': True,
         'source_data':           {
-            'abspath':  '/library/TEST_FILE.mkv',
-            'basename': 'TEST_FILE.mp4',
+            'abspath':  '{library_path}/{test_file_in}',
+            'basename': '{test_file_in}',
         }
     }
```

### Comparing `unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/frontend/__init__.py` & `unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/frontend/plugin_api.py` & `unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/frontend/plugin_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/frontend/panel.py` & `unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/frontend/panel.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/worker/process_item.py` & `unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/worker/process_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         },
         "exec_command":            {
             "required": True,
             "type":     [list, str],
         },
         "command_progress_parser": {
             "required": True,
-            "type":     'callable',
+            "type":     ['callable', None],
         },
         "file_in":                 {
             "required": True,
             "type":     str,
         },
         "file_out":                {
             "required": True,
@@ -86,13 +86,13 @@
             "type":     bool,
         },
     }
     test_data = {
         'worker_log':              [],
         'library_id':              1,
         'exec_command':            [],
-        'command_progress_parser': exec,
-        'file_in':                 '/library/TEST_FILE.mkv',
-        'file_out':                '/tmp/unmanic/unmanic_file_conversion-1616571944.7296784/TEST_FILE-1616571944.7296877-WORKING-1.mkv',
-        'original_file_path':      '/library/TEST_FILE.mkv',
+        'command_progress_parser': None,
+        'file_in':                 '{library_path}/{test_file_in}',
+        'file_out':                '{cache_path}/{test_file_out}',
+        'original_file_path':      '{library_path}/{test_file_in}',
         'repeat':                  False,
     }
```

### Comparing `unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/worker/__init__.py` & `unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unplugins/plugin_types/plugin_type_base.py` & `unmanic-0.2.4/unmanic/libs/unplugins/plugin_types/plugin_type_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,16 @@
            IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
            DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
            OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
            OR OTHER DEALINGS IN THE SOFTWARE.
 
 """
 import inspect
+import json
+from copy import deepcopy
 
 
 class PluginType(object):
     """
     PluginType
 
     Generic configuration and methods used across all plugin types
@@ -88,30 +90,40 @@
         """
         Return the plugin test data dictionary
 
         :return:
         """
         return self.test_data
 
+    @staticmethod
+    def modify_test_data(d: dict, v: dict):
+        dict_str = json.dumps(d)
+        for a, b in v.items():
+            dict_str = dict_str.replace(a, b)
+        return json.loads(dict_str)
+
     def __data_schema_test_data(self, plugin_id, plugin_runner, result_data, data_schema, data_tree="/"):
         """
         Ensure the test data returned is valid according to the schema
 
         :param plugin_id:
         :param plugin_runner:
         :param result_data:
         :param data_schema:
         :param data_tree:
         :return:
         """
 
         def test_data_type(provided_data, expected_data_type):
+            # Test for NoneType
             # Callable functions are best tested with the callable function
             # Everything else should be tested with the isinstance function
-            if expected_data_type == 'callable':
+            if provided_data is None and expected_data_type is None:
+                return True
+            elif expected_data_type == 'callable':
                 if callable(provided_data):
                     return True
             elif isinstance(provided_data, expected_data_type):
                 return True
             return False
 
         errors = []
@@ -160,29 +172,31 @@
                 if children_data_schema:
                     child_data_tree = "{}{}>".format(data_tree, key)
                     errors += self.__data_schema_test_data(plugin_id, plugin_runner, child_data, children_data_schema,
                                                            data_tree=child_data_tree)
 
         return errors
 
-    def run_data_schema_tests(self, plugin_id, plugin_module, test_data=None):
+    def run_data_schema_tests(self, plugin_id, plugin_module, test_data):
         """
         With a given set of test data, this method tests the provided
         plugin module's data output against the schema dictionary.
 
+        :param plugin_id:
         :param plugin_module:
+        :param test_data:
         :return:
         """
         plugin_runner = self.plugin_runner()
         plugin_runner_function = self.get_plugin_runner_function(plugin_module)
 
         # Get test data
         if not test_data:
             test_data = self.get_test_data()
-        test_data_copy = test_data.copy()
+        test_data_copy = deepcopy(test_data)
 
         # Get data schema
         data_schema = self.get_data_schema()
 
         # Execute plugin function
         run_count = 0
         while run_count < 2:
```

### Comparing `unmanic-0.2.3/unmanic/libs/unplugins/settings.py` & `unmanic-0.2.4/unmanic/libs/unplugins/settings.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/taskhandler.py` & `unmanic-0.2.4/unmanic/libs/taskhandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,17 +50,18 @@
             - Task Handler to monitor idle workers rather than idle workers looking for tasks in the TaskQueue object.
                 - When a worker thread is idle, the TaskHandler needs to read a select query on the database and add that
                     item to the TaskQueue
             - Workers should request a job from the TaskHandler rather than reading the TaskQueue directly ??
             -
     """
 
-    def __init__(self, data_queues, task_queue):
+    def __init__(self, data_queues, task_queue, event):
         super(TaskHandler, self).__init__(name='TaskHandler')
         self.settings = config.Config()
+        self.event = event
         self.data_queues = data_queues
         self.logger = data_queues["logging"].get_logger(self.name)
         self.task_queue = task_queue
         self.inotifytasks = data_queues["inotifytasks"]
         self.scheduledtasks = data_queues["scheduledtasks"]
         self.abort_flag = threading.Event()
         self.abort_flag.clear()
@@ -73,22 +74,23 @@
 
     def stop(self):
         self.abort_flag.set()
 
     def run(self):
         self._log("Starting TaskHandler Monitor loop")
         while not self.abort_flag.is_set():
+            self.event.wait(2)
             self.process_scheduledtasks_queue()
             self.process_inotifytasks_queue()
-            time.sleep(.2)
 
         self._log("Leaving TaskHandler Monitor loop...")
 
     def process_scheduledtasks_queue(self):
         while not self.abort_flag.is_set() and not self.scheduledtasks.empty():
+            # Do not sleep at all here. Process this loop as quick as possible
             try:
                 item = self.scheduledtasks.get_nowait()
                 pathname = item['pathname']
                 library_id = item['library_id']
                 priority_score = item.get('priority_score', 0)
                 if self.add_path_to_task_queue(pathname, library_id, priority_score=priority_score):
                     self._log("Adding file to task queue", pathname, level='info')
@@ -97,14 +99,15 @@
             except queue.Empty:
                 continue
             except Exception as e:
                 self._log("Exception in processing scheduledtasks", str(e), level='exception')
 
     def process_inotifytasks_queue(self):
         while not self.abort_flag.is_set() and not self.inotifytasks.empty():
+            # Do not sleep at all here. Process this loop as quick as possible
             try:
                 item = self.inotifytasks.get_nowait()
                 pathname = item['pathname']
                 library_id = item['library_id']
                 priority_score = item.get('priority_score', 0)
                 # TODO: Ensure the file is not still being modified at this point.
                 #  If it is still being modified here, it is ok to wait for that to finish (should not matter much)
```

### Comparing `unmanic-0.2.3/unmanic/libs/session.py` & `unmanic-0.2.4/unmanic/libs/session.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/plugins.py` & `unmanic-0.2.4/unmanic/libs/plugins.py`

 * *Files 5% similar despite different names*

```diff
@@ -339,18 +339,19 @@
         :param plugin_id:
         :param repo_id:
         :return:
         """
         plugin_list = self.get_installable_plugins_list(filter_repo_id=repo_id)
         for plugin in plugin_list:
             if plugin.get('plugin_id') == plugin_id:
-                success = self.install_plugin(plugin)
+                success = self.download_and_install_plugin(plugin)
 
                 if success:
                     try:
+                        # Write the plugin info to the DB
                         plugin_directory = self.get_plugin_path(plugin.get("plugin_id"))
                         result = self.write_plugin_data_to_db(plugin, plugin_directory)
                         if result:
                             self._log("Installed plugin '{}'".format(plugin_id), level="info")
 
                         # Ensure the plugin module is reloaded (if it was previously loaded)
                         plugin_executor = PluginExecutor()
@@ -358,38 +359,64 @@
 
                         return result
                     except Exception as e:
                         self._log("Exception while installing plugin '{}'.".format(plugin), str(e), level="exception")
 
         return False
 
-    def install_plugin(self, plugin):
+    def install_plugin_from_path_on_disk(self, abspath):
+        """
+        Install a plugin from a ZIP file on disk
+
+        :param abspath:
+        :return:
+        """
+        # TODO: Ensure that this is a zip file
+        try:
+            plugin_info = self.install_plugin(abspath)
+
+            # Set the plugin_id variable used when writing data to DB.
+            # The returned 'plugin_info' is just a readout of the info.json file which has this set to 'id'
+            plugin_info['plugin_id'] = plugin_info.get('id')
+
+            # Cleanup zip file
+            if os.path.isfile(abspath):
+                os.remove(abspath)
+
+            # Write the plugin info to the DB
+            plugin_directory = self.get_plugin_path(plugin_info.get("plugin_id"))
+            result = self.write_plugin_data_to_db(plugin_info, plugin_directory)
+            if result:
+                self._log("Installed plugin '{}'".format(plugin_info.get("plugin_id")), level="info")
+
+            # Ensure the plugin module is reloaded (if it was previously loaded)
+            plugin_executor = PluginExecutor()
+            plugin_executor.reload_plugin_module(plugin_info.get('plugin_id'))
+
+            return result
+        except Exception as e:
+            self._log("Exception while installing plugin from zip '{}'.".format(abspath), str(e), level="exception")
+
+        return False
+
+    def download_and_install_plugin(self, plugin):
         """
         Download and install a given plugin
 
         :param plugin:
         :return:
         """
         self._log("Installing plugin '{}'".format(plugin.get("name")), level='debug')
         # Try to fetch URL
         try:
             # Fetch remote zip file
-            destination = self.get_plugin_download_cache_path(plugin.get("plugin_id"), plugin.get("version"))
-            self._log("Downloading plugin '{}' to '{}'".format(plugin.get("package_url"), destination), level='debug')
-            with requests.get(plugin.get("package_url"), stream=True, allow_redirects=True) as r:
-                r.raise_for_status()
-                with open(destination, 'wb') as f:
-                    for chunk in r.iter_content(chunk_size=128):
-                        f.write(chunk)
-
-            # Extract zip file contents
-            plugin_directory = self.get_plugin_path(plugin.get("plugin_id"))
-            self._log("Extracting plugin to '{}'".format(plugin_directory), level='debug')
-            with zipfile.ZipFile(destination, "r") as zip_ref:
-                zip_ref.extractall(plugin_directory)
+            destination = self.download_plugin(plugin)
+
+            # Install downloaded plugin
+            self.install_plugin(destination, plugin.get("plugin_id"))
 
             # Cleanup zip file
             if os.path.isfile(destination):
                 os.remove(destination)
 
             self.notify_site_of_plugin_install(plugin)
 
@@ -397,14 +424,53 @@
 
         except Exception as e:
             success = False
             self._log("Exception while installing plugin '{}'.".format(plugin), str(e), level="exception")
 
         return False
 
+    def download_plugin(self, plugin):
+        """
+        Download a given plugin to a temp directory
+
+        :param plugin:
+        :return:
+        """
+        # Fetch remote zip file
+        destination = self.get_plugin_download_cache_path(plugin.get("plugin_id"), plugin.get("version"))
+        self._log("Downloading plugin '{}' to '{}'".format(plugin.get("package_url"), destination), level='debug')
+        with requests.get(plugin.get("package_url"), stream=True, allow_redirects=True) as r:
+            r.raise_for_status()
+            with open(destination, 'wb') as f:
+                for chunk in r.iter_content(chunk_size=128):
+                    f.write(chunk)
+        return destination
+
+    def install_plugin(self, zip_file, plugin_id=None):
+        """
+        Install a given plugin from a zip file
+
+        :param zip_file:
+        :param plugin_id:
+        :return:
+        """
+        # Read plugin ID from zip contents info.json if no plugin_id was provided
+        if not plugin_id:
+            with zipfile.ZipFile(zip_file, "r") as zip_ref:
+                plugin_info = json.loads(zip_ref.read('info.json'))
+            plugin_id = plugin_info.get('id')
+        # Create plugin destination directory based on plugin ID
+        plugin_directory = self.get_plugin_path(plugin_id)
+        # Extract zip file contents
+        self._log("Extracting plugin to '{}'".format(plugin_directory), level='debug')
+        with zipfile.ZipFile(zip_file, "r") as zip_ref:
+            zip_ref.extractall(plugin_directory)
+        # Return installed plugin info
+        return self.get_plugin_info(plugin_id)
+
     @staticmethod
     def write_plugin_data_to_db(plugin, plugin_directory):
         # Add installed plugin to database
         plugin_data = {
             Plugins.plugin_id:        plugin.get("plugin_id"),
             Plugins.name:             plugin.get("name"),
             Plugins.author:           plugin.get("author"),
```

### Comparing `unmanic-0.2.3/unmanic/libs/foreman.py` & `unmanic-0.2.4/unmanic/libs/foreman.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,18 @@
 from unmanic.libs.library import Library
 from unmanic.libs.plugins import PluginsHandler
 from unmanic.libs.worker_group import WorkerGroup
 from unmanic.libs.workers import Worker
 
 
 class Foreman(threading.Thread):
-    def __init__(self, data_queues, settings, task_queue):
+    def __init__(self, data_queues, settings, task_queue, event):
         super(Foreman, self).__init__(name='Foreman')
         self.settings = settings
+        self.event = event
         self.task_queue = task_queue
         self.data_queues = data_queues
         self.logger = data_queues["logging"].get_logger(self.name)
         self.workers_pending_task_queue = queue.Queue(maxsize=1)
         self.remote_workers_pending_task_queue = queue.Queue(maxsize=1)
         self.complete_queue = queue.Queue()
         self.worker_threads = {}
@@ -313,15 +314,16 @@
             return False
 
         # Startup a thread
         thread = installation_link.RemoteTaskManager(installation_id,
                                                      "RemoteTaskManager-{}".format(installation_id),
                                                      installation_info,
                                                      self.remote_workers_pending_task_queue,
-                                                     self.complete_queue)
+                                                     self.complete_queue,
+                                                     self.event)
         thread.daemon = True
         thread.start()
         self.remote_task_manager_threads[installation_id] = thread
         return True
 
     def remove_stale_available_remote_managers(self):
         """
@@ -411,15 +413,15 @@
                     'password':      remote_password,
                     'library_names': remote_library_names,
                     'created':       datetime.now(),
                 }
 
     def start_worker_thread(self, worker_id, worker_name, worker_group):
         thread = Worker(worker_id, worker_name, worker_group, self.workers_pending_task_queue,
-                        self.complete_queue)
+                        self.complete_queue, self.event)
         thread.daemon = True
         thread.start()
         self.worker_threads[worker_id] = thread
 
     def fetch_available_worker_ids(self):
         tread_ids = []
         for thread in self.worker_threads:
@@ -622,20 +624,20 @@
 
         # Flag to force checking for idle remote workers when set to False.
         # This will prevent always looping on idle local workers when the local worker's
         # tags prevent them from taking up tasks
         allow_local_idle_worker_check = True
 
         while not self.abort_flag.is_set():
-            time.sleep(1)
+            self.event.wait(2)
 
             try:
                 # Fetch all completed tasks from workers
                 while not self.abort_flag.is_set() and not self.complete_queue.empty():
-                    time.sleep(.2)
+                    self.event.wait(.5)
                     try:
                         task_item = self.complete_queue.get_nowait()
                         task_item.set_status('processed')
                     except queue.Empty:
                         continue
                     except Exception as e:
                         self._log("Exception when fetching completed task report from worker", message2=str(e),
@@ -686,20 +688,20 @@
                         # Remote workers are available
                         process_local = False
                         # For remote workers, only process local tasks. Don't hand remote tasks to another remote installation
                         get_local_pending_tasks_only = True
                     else:
                         allow_local_idle_worker_check = True
                         # All workers are currently busy
-                        time.sleep(1)
+                        self.event.wait(1)
                         continue
 
                     # Check if postprocessor task queue is full
                     if self.postprocessor_queue_full():
-                        time.sleep(3)
+                        self.event.wait(5)
                         continue
 
                     # Fetch the next item in the queue
                     available_worker_id = None
                     next_item_to_process = None
                     if process_local:
                         # For local processing, ensure tags match the available library and worker
@@ -716,29 +718,29 @@
                                 library_tags=library_tags)
                             if next_item_to_process:
                                 available_worker_id = worker_id
                                 break
                         # If no local worker ID was assigned to the given item, then try again in 2 seconds
                         if not available_worker_id:
                             allow_local_idle_worker_check = False
-                            time.sleep(1)
+                            self.event.wait(1)
                             continue
                     else:
                         # For remote items, run a search matching an available remote installation library
                         remote_library_names = self.get_available_remote_library_names()
                         next_item_to_process = self.task_queue.get_next_pending_tasks(local_only=get_local_pending_tasks_only,
                                                                                       library_names=remote_library_names)
 
                     if next_item_to_process:
                         try:
                             source_abspath = next_item_to_process.get_source_abspath()
                             task_library_name = next_item_to_process.get_task_library_name()
                         except Exception as e:
                             self._log("Exception in fetching task details", message2=str(e), level="exception")
-                            time.sleep(3)
+                            self.event.wait(3)
                             continue
 
                         self._log("Processing item - {}".format(source_abspath))
                         success = self.hand_task_to_workers(next_item_to_process, local=process_local,
                                                             library_name=task_library_name,
                                                             worker_id=available_worker_id)
                         if not success:
```

### Comparing `unmanic-0.2.3/unmanic/libs/eventmonitor.py` & `unmanic-0.2.4/unmanic/libs/eventmonitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,20 +111,21 @@
 
     Manage the EventProcessor thread.
     If the settings for enabling the EventProcessor changes, this manager
     class will stop or start the EventProcessor thread accordingly.
 
     """
 
-    def __init__(self, data_queues):
+    def __init__(self, data_queues, event):
         super(EventMonitorManager, self).__init__(name='EventMonitorManager')
         self.name = "EventMonitorManager"
         self.data_queues = data_queues
         self.settings = config.Config()
         self.logger = None
+        self.event = event
 
         # Create an event queue
         self.files_to_test = queue.Queue()
 
         self.abort_flag = threading.Event()
         self.abort_flag.clear()
 
@@ -138,21 +139,20 @@
         message = common.format_message(message, message2)
         getattr(self.logger, level)(message)
 
     def stop(self):
         self.abort_flag.set()
 
     def run(self):
-        # If we have a config set to run a schedule, then start the process.
-        # Otherwise close this thread now.
         self._log("Starting EventMonitorManager loop")
         while not self.abort_flag.is_set():
+            self.event.wait(.5)
 
             if not self.system_configuration_is_valid():
-                time.sleep(2)
+                self.event.wait(2)
                 continue
 
             if not self.files_to_test.empty():
                 item = self.files_to_test.get()
                 pathname = item.get('src_path')
                 library_id = item.get('library_id')
                 self.manage_event_queue(pathname, library_id)
@@ -180,15 +180,15 @@
                 if not self.event_observer_thread:
                     self.start_event_processor()
             else:
                 # If not enabled, ensure the EventProcessor is not running and stop it if it is
                 if self.event_observer_thread:
                     self.stop_event_processor()
             # Add delay
-            time.sleep(.5)
+            self.event.wait(2)
 
         self.stop_event_processor()
         self._log("Leaving EventMonitorManager loop...")
 
     def system_configuration_is_valid(self):
         """
         Check and ensure the system configuration is correct for running
@@ -209,28 +209,28 @@
 
         :return:
         """
         if not self.event_observer_thread:
             monitoring_path = False
             self.event_observer_thread = Observer()
             for lib_info in Library.get_all_libraries():
+                self.event.wait(.2)
                 try:
                     library = Library(lib_info['id'])
                 except Exception as e:
                     self._log("Unable to fetch library config for ID {}".format(lib_info['id']), level='exception')
                     continue
                 # Check if the library is configured for remote files only
                 if library.get_enable_remote_only():
                     # This library is configured to receive remote files only... Never enable the file monitor
                     continue
                 # Check if library scanner is enabled on any library
                 if library.get_enable_inotify():
                     library_path = library.get_path()
                     if not os.path.exists(library_path):
-                        time.sleep(.1)
                         continue
                     self._log("Adding library path to monitor '{}'".format(library_path))
                     event_handler = EventHandler(self.files_to_test, library.get_id())
                     self.event_observer_thread.schedule(event_handler, library_path, recursive=True)
                     monitoring_path = True
             # Only start observer if a path was added to be monitored
             if monitoring_path:
```

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/exceptions/__init__.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/exceptions/ffprobe.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/exceptions/ffprobe.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/exceptions/ffmpeg.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/exceptions/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/base_codecs.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/base_codecs.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/video_codecs/__init__.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/video_codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/video_codecs/h264.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/video_codecs/h264.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/video_codecs/hevc.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/video_codecs/hevc.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/lib/cli.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/lib/cli.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/lib/__init__.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/lib/validation.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/lib/validation.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/audio_codec_handle.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/audio_codec_handle.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_codecs/srt.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_codecs/srt.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_codecs/xsub.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_codecs/xsub.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_codecs/__init__.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_codecs/ssa.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_codecs/ssa.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_codecs/mov_text.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_codecs/mov_text.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_codecs/ass.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_codecs/ass.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_codecs/subrip.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_codecs/subrip.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/__init__.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/base_containers.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/base_containers.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/video_codec_handle.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/video_codec_handle.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/info.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/info.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/subtitle_handle.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/subtitle_handle.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/containers/mpeg.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/containers/mpeg.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/containers/vob.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/containers/vob.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/containers/ogv.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/containers/ogv.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/containers/mov.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/containers/mov.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/containers/__init__.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/containers/avi.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/containers/avi.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/containers/mp4.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/containers/mp4.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/containers/flv.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/containers/flv.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/containers/psp.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/containers/psp.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/containers/mpegts.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/containers/mpegts.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/containers/matroska.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/containers/matroska.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/audio_codecs/aac.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/audio_codecs/aac.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/audio_codecs/ac3.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/audio_codecs/ac3.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/audio_codecs/mp3.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/audio_codecs/mp3.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/audio_codecs/__init__.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/audio_codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/unffmpeg/hardware_acceleration_handle.py` & `unmanic-0.2.4/unmanic/libs/unffmpeg/hardware_acceleration_handle.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/installation_link.py` & `unmanic-0.2.4/unmanic/libs/installation_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -1184,18 +1184,19 @@
     finish_time = None
 
     worker_subprocess_percent = None
     worker_subprocess_elapsed = None
 
     worker_runners_info = {}
 
-    def __init__(self, thread_id, name, installation_info, pending_queue, complete_queue):
+    def __init__(self, thread_id, name, installation_info, pending_queue, complete_queue, event):
         super(RemoteTaskManager, self).__init__(name=name)
         self.thread_id = thread_id
         self.name = name
+        self.event = event
         self.installation_info = installation_info
         self.pending_queue = pending_queue
         self.complete_queue = complete_queue
 
         self.links = Links()
 
         # Create 'redundancy' flag. When this is set, the worker should die
@@ -1413,15 +1414,15 @@
                 # For files smaller than 100MB, just transfer them in parallel
                 # Smaller files add a lot of time overhead with the waiting in line and it slows the whole process down
                 # Larger files benefit from being transferred one at a time.
                 if initial_file_size > 100000000:
                     # Check for network transfer lock
                     lock_key = self.links.acquire_network_transfer_lock(address, transfer_limit=1, lock_type='send')
                     if not lock_key:
-                        time.sleep(1)
+                        self.event.wait(1)
                         continue
 
                 # Send a file to a remote installation.
                 self._log("Uploading file to remote installation '{}'".format(original_abspath), level='debug')
                 info = self.links.send_file_to_remote_installation(self.installation_info, original_abspath)
                 self.links.release_network_transfer_lock(lock_key)
                 if not info:
@@ -1448,15 +1449,15 @@
             return False
 
         # Set the library of the remote task using the library's name
         while not self.redundant_flag.is_set():
             result = self.links.set_the_remote_task_library(self.installation_info, remote_task_id, library_name)
             if result is None:
                 # Unable to reach remote installation
-                time.sleep(2)
+                self.event.wait(2)
                 continue
             if not result.get('success'):
                 self._log(
                     "Failed to match a remote library named '{}'. Remote installation will use the default library".format(
                         library_name), level='warning')
                 # Just log the warning for this. If no matching library name is found it will remain set as the default library
                 break
@@ -1464,15 +1465,15 @@
                 break
 
         # Start the remote task
         while not self.redundant_flag.is_set():
             result = self.links.start_the_remote_task_by_id(self.installation_info, remote_task_id)
             if not result:
                 # Unable to reach remote installation
-                time.sleep(2)
+                self.event.wait(2)
                 continue
             if not result.get('success'):
                 self._log("Failed to set initial remote pending task to status '{}'".format(original_abspath), level='error')
                 # Send request to terminate the remote worker then return
                 self.links.remove_task_from_remote_installation(self.installation_info, remote_task_id)
                 self.__write_failure_to_worker_log()
                 return False
@@ -1481,15 +1482,15 @@
 
         # Loop while redundant_flag not set (while true because of below)
         worker_id = None
         task_status = ''
         last_status_fetch = 0
         polling_delay = 5
         while task_status != 'complete':
-            time.sleep(1)
+            self.event.wait(1)
             if self.redundant_flag.is_set():
                 # Send request to terminate the remote worker then exit
                 if worker_id:
                     self.links.terminate_remote_worker(self.installation_info, worker_id)
                 break
 
             # Only fetch the status every 5 seconds
@@ -1585,15 +1586,15 @@
 
         if not data:
             self._log(
                 "Failed to retrieve remote task data for '{}'. NOTE: The cached files have not been removed from the remote host.".format(
                     original_abspath), level='error')
             self.__write_failure_to_worker_log()
             return False
-        self.worker_log = data.get('log')
+        self.worker_log = [data.get('log')]
 
         # Save the completed command log
         self.current_task.save_command_log(self.worker_log)
 
         # Fetch remote task file
         if data.get('task_success'):
             task_label = data.get('task_label')
@@ -1609,15 +1610,15 @@
             task_cache_path = self.current_task.get_cache_path()
 
             # Loop until we are able to upload the file to the remote installation
             while not self.redundant_flag.is_set():
                 # Check for network transfer lock
                 lock_key = self.links.acquire_network_transfer_lock(address, transfer_limit=2, lock_type='receive')
                 if not lock_key:
-                    time.sleep(1)
+                    self.event.wait(1)
                     continue
                 # Download the file
                 self._log("Downloading file from remote installation '{}'".format(task_label), level='debug')
                 success = self.links.fetch_remote_task_completed_file(self.installation_info, remote_task_id, task_cache_path)
                 self.links.release_network_transfer_lock(lock_key)
                 if not success:
                     self._log("Failed to download file '{}'".format(os.path.basename(data.get('abspath'))), level='error')
```

### Comparing `unmanic-0.2.3/unmanic/libs/filetest.py` & `unmanic-0.2.4/unmanic/libs/filetest.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
            OR OTHER DEALINGS IN THE SOFTWARE.
 
 """
 import os
 import queue
 import threading
 import time
+from copy import deepcopy
 
 from unmanic import config
 from unmanic.libs import history, common, unlogger
 from unmanic.libs.plugins import PluginsHandler
 
 
 class FileTest(object):
@@ -140,15 +141,15 @@
                 'priority_score': 0,
                 'shared_info':    {},
             }
             # Run tests against plugins
             for plugin_module in self.plugin_modules:
                 data['library_id'] = self.library_id
                 data['path'] = path
-                data['issues'] = file_issues.copy()
+                data['issues'] = deepcopy(file_issues)
                 data['add_file_to_pending_tasks'] = None
 
                 # Run plugin to update data
                 if not self.plugin_handler.exec_plugin_runner(data, plugin_module.get('plugin_id'),
                                                               'library_management.file_test'):
                     continue
 
@@ -164,18 +165,19 @@
             # Set the priority score modification
             priority_score_modification = data.get('priority_score', 0)
 
         return return_value, file_issues, priority_score_modification
 
 
 class FileTesterThread(threading.Thread):
-    def __init__(self, name, files_to_test, files_to_process, status_updates, library_id):
+    def __init__(self, name, files_to_test, files_to_process, status_updates, library_id, event):
         super(FileTesterThread, self).__init__(name=name)
         self.settings = config.Config()
         self.logger = None
+        self.event = event
         self.files_to_test = files_to_test
         self.files_to_process = files_to_process
         self.library_id = library_id
         self.status_updates = status_updates
         self.abort_flag = threading.Event()
         self.abort_flag.clear()
 
@@ -186,48 +188,46 @@
         message = common.format_message(message, message2)
         getattr(self.logger, level)(message)
 
     def stop(self):
         self.abort_flag.set()
 
     def run(self):
-        # If we have a config set to run a schedule, then start the process.
-        # Otherwise close this thread now.
         self._log("Starting {}".format(self.name))
         file_test = FileTest(self.library_id)
         while not self.abort_flag.is_set():
             try:
                 # Pending task queue has an item available. Fetch it.
                 next_file = self.files_to_test.get_nowait()
-
                 self.status_updates.put(next_file)
-
-                # Test file to be added to task list. Add it if required
-                try:
-                    result, issues, priority_score = file_test.should_file_be_added_to_task_list(next_file)
-                    # Log any error messages
-                    for issue in issues:
-                        if type(issue) is dict:
-                            self._log(issue.get('message'))
-                        else:
-                            self._log(issue)
-                    # If file needs to be added, then add it
-                    if result:
-                        self.add_path_to_queue({
-                            'path':           next_file,
-                            'priority_score': priority_score,
-                        })
-                except UnicodeEncodeError:
-                    self._log("File contains Unicode characters that cannot be processed. Ignoring.", level="warning")
-                except Exception as e:
-                    self._log("Exception testing file path in {}. Ignoring.".format(self.name), message2=str(e),
-                              level="exception")
             except queue.Empty:
-                time.sleep(.1)
+                self.event.wait(2)
                 continue
             except Exception as e:
-                self._log("Exception in checking library scan results with {}:".format(self.name), message2=str(e),
-                          level="exception")
+                self._log("Exception in fetching library scan result for path {}:".format(self.name), message2=str(e),
+                            level="exception")
+
+            # Test file to be added to task list. Add it if required
+            try:
+                result, issues, priority_score = file_test.should_file_be_added_to_task_list(next_file)
+                # Log any error messages
+                for issue in issues:
+                    if type(issue) is dict:
+                        self._log(issue.get('message'))
+                    else:
+                        self._log(issue)
+                # If file needs to be added, then add it
+                if result:
+                    self.add_path_to_queue({
+                        'path':           next_file,
+                        'priority_score': priority_score,
+                    })
+            except UnicodeEncodeError:
+                self._log("File contains Unicode characters that cannot be processed. Ignoring.", level="warning")
+            except Exception as e:
+                self._log("Exception testing file path in {}. Ignoring.".format(self.name), message2=str(e),
+                            level="exception")
+
         self._log("Exiting {}".format(self.name))
 
     def add_path_to_queue(self, item):
         self.files_to_process.put(item)
```

### Comparing `unmanic-0.2.3/unmanic/libs/task.py` & `unmanic-0.2.4/unmanic/libs/task.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/postprocessor.py` & `unmanic-0.2.4/unmanic/libs/postprocessor.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 import shutil
 import threading
 import time
 
 from unmanic import config
 from unmanic.libs import common, history
 from unmanic.libs.library import Library
+from unmanic.libs.notifications import Notifications
 from unmanic.libs.plugins import PluginsHandler
 
 """
 
 The post-processor handles all tasks carried out on completion of a workers task.
 This may be on either success or failure of the task.
 
@@ -60,17 +61,18 @@
 
 class PostProcessor(threading.Thread):
     """
     PostProcessor
 
     """
 
-    def __init__(self, data_queues, task_queue):
+    def __init__(self, data_queues, task_queue, event):
         super(PostProcessor, self).__init__(name='PostProcessor')
         self.logger = data_queues["logging"].get_logger(self.name)
+        self.event = event
         self.data_queues = data_queues
         self.settings = config.Config()
         self.task_queue = task_queue
         self.abort_flag = threading.Event()
         self.current_task = None
         self.ffmpeg = None
         self.abort_flag.clear()
@@ -81,22 +83,22 @@
 
     def stop(self):
         self.abort_flag.set()
 
     def run(self):
         self._log("Starting PostProcessor Monitor loop...")
         while not self.abort_flag.is_set():
-            time.sleep(1)
+            self.event.wait(1)
 
             if not self.system_configuration_is_valid():
-                time.sleep(2)
+                self.event.wait(2)
                 continue
 
             while not self.abort_flag.is_set() and not self.task_queue.task_list_processed_is_empty():
-                time.sleep(.2)
+                self.event.wait(.2)
                 self.current_task = self.task_queue.get_next_processed_tasks()
                 if self.current_task:
                     try:
                         self._log("Post-processing task - {}".format(self.current_task.get_source_abspath()))
                     except Exception as e:
                         self._log("Exception in fetching task absolute path", message2=str(e), level="exception")
                     if self.current_task.get_task_type() == 'local':
@@ -340,15 +342,15 @@
                 self._log("The file_in and file_out path are the same file. Nothing will be done! '{}'".format(file_in),
                           level="warning")
                 return False
 
             # Get a checksum prior to copy
             if not os.path.exists(file_in):
                 self._log("The file_in path does not exist! '{}'".format(file_in), level="warning")
-                time.sleep(1)
+                self.event.wait(1)
             self._log("Fetching checksum of source file '{}'.".format(file_in), level='debug')
 
             # Use a '.part' suffix for the file movement, then rename it after
             part_file_out = os.path.join("{}.unmanic.part".format(file_out))
 
             # Carry out the file movement
             if move:
@@ -385,14 +387,32 @@
 
         :return:
         """
         self._log("Writing task history log.", level='debug')
         history_logging = history.History()
         task_dump = self.current_task.task_dump()
 
+        # If task fails, the add a notification that a task has failed
+        if not self.current_task.task.success:
+            notifications = Notifications()
+            notifications.add(
+                {
+                    'uuid':       'newFailedTask',
+                    'type':       'error',
+                    'icon':       'report',
+                    'label':      'failedTaskLabel',
+                    'message':    'You have a new failed task in your completed tasks list',
+                    'navigation': {
+                        'push':   '/ui/dashboard',
+                        'events': [
+                            'completedTasksShowFailed',
+                        ],
+                    },
+                })
+
         history_logging.save_task_history(
             {
                 'task_label':          task_dump.get('task_label', ''),
                 'abspath':             task_dump.get('abspath', ''),
                 'task_success':        task_dump.get('task_success', ''),
                 'start_time':          task_dump.get('start_time', ''),
                 'finish_time':         task_dump.get('finish_time', ''),
```

### Comparing `unmanic-0.2.3/unmanic/libs/directoryinfo.py` & `unmanic-0.2.4/unmanic/libs/directoryinfo.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/history.py` & `unmanic-0.2.4/unmanic/libs/history.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/libraryscanner.py` & `unmanic-0.2.4/unmanic/libs/libraryscanner.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,21 +43,22 @@
 from unmanic.libs import common, unlogger
 from unmanic.libs.filetest import FileTesterThread
 from unmanic.libs.library import Library
 from unmanic.libs.plugins import PluginsHandler
 
 
 class LibraryScannerManager(threading.Thread):
-    def __init__(self, data_queues):
+    def __init__(self, data_queues, event):
         super(LibraryScannerManager, self).__init__(name='LibraryScannerManager')
         self.interval = 0
         self.firstrun = True
         self.data_queues = data_queues
         self.settings = config.Config()
         self.logger = None
+        self.event = event
         self.scheduledtasks = data_queues["scheduledtasks"]
         self.library_scanner_triggers = data_queues["library_scanner_triggers"]
         self.abort_flag = threading.Event()
         self.abort_flag.clear()
         self.scheduler = schedule.Scheduler()
 
         self.file_test_managers = {}
@@ -78,24 +79,22 @@
 
     def abort_is_set(self):
         # Check if the abort flag is set
         if self.abort_flag.is_set():
             # Return True straight away if it is
             return True
         # Sleep for a fraction of a second to prevent CPU pinning
-        time.sleep(.1)
+        self.event.wait(.1)
         # Return False
         return False
 
     def run(self):
-        # If we have a config set to run a schedule, then start the process.
-        # Otherwise close this thread now.
         self._log("Starting LibraryScanner Monitor loop")
         while not self.abort_is_set():
-            time.sleep(.2)
+            self.event.wait(1)
 
             # Main loop to configure the scheduler
             if int(self.settings.get_schedule_full_scan_minutes()) != self.interval:
                 self.interval = int(self.settings.get_schedule_full_scan_minutes())
             if self.interval and self.interval != 0:
                 self._log("Setting LibraryScanner schedule to scan every {} mins...".format(self.interval))
                 # Configure schedule
@@ -108,15 +107,15 @@
                     self._log("Running LibraryScanner on start")
                     self.scheduled_job()
                 self.firstrun = False
 
                 # Then loop and wait for the schedule
                 while not self.abort_is_set():
                     # Delay for 1 second before checking again.
-                    time.sleep(1)
+                    self.event.wait(1)
 
                     # Check if a manual library scan was triggered
                     try:
                         if not self.library_scanner_triggers.empty():
                             trigger = self.library_scanner_triggers.get_nowait()
                             if trigger == "library_scan":
                                 self.scheduled_job()
@@ -194,15 +193,15 @@
             'pathname':       pathname,
             'library_id':     library_id,
             'priority_score': priority_score,
         })
 
     def start_results_manager_thread(self, manager_id, status_updates, library_id):
         manager = FileTesterThread("FileTesterThread-{}".format(manager_id), self.files_to_test,
-                                   self.files_to_process, status_updates, library_id)
+                                   self.files_to_process, status_updates, library_id, self.event)
         manager.daemon = True
         manager.start()
         self.file_test_managers[manager_id] = manager
 
     def stop_all_file_test_managers(self):
         for manager_id in self.file_test_managers:
             self.file_test_managers[manager_id].abort_flag.set()
@@ -294,15 +293,15 @@
                 # This is used to ensure that the loop does not prematurely exit when the last file tests still
                 # progressing that have not yet made it to the "files_to_process" queue.
                 double_check += 1
                 if double_check > 5:
                     # There are not more files to test. Mark manager threads as completed
                     self.stop_all_file_test_managers()
                     break
-                time.sleep(1)
+                self.event.wait(1)
                 continue
 
             # Calculate percent of files tested
             if not self.files_to_test.empty():
                 current_queue_size = self.files_to_test.qsize()
                 if int(total_file_count) > 0 and int(current_queue_size) > 0:
                     percent_remaining = int((int(current_queue_size) / int(total_file_count)) * 100)
@@ -316,15 +315,15 @@
                 current_file = status_updates.get()
                 continue
             elif not self.files_to_process.empty():
                 item = self.files_to_process.get()
                 self.add_path_to_queue(item.get('path'), library_id, item.get('priority_score'))
                 continue
             else:
-                time.sleep(.1)
+                self.event.wait(.1)
 
         # Wait for threads to finish
         for manager_id in self.file_test_managers:
             self.file_test_managers[manager_id].abort_flag.set()
             self.file_test_managers[manager_id].join(2)
 
         self._log("Library scan completed in {} seconds".format((time.time() - start_time)), level="warning")
```

### Comparing `unmanic-0.2.3/unmanic/libs/unlogger.py` & `unmanic-0.2.4/unmanic/libs/unlogger.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/system.py` & `unmanic-0.2.4/unmanic/libs/system.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/fileinfo.py` & `unmanic-0.2.4/unmanic/libs/fileinfo.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/scheduler.py` & `unmanic-0.2.4/unmanic/libs/scheduler.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,17 +44,18 @@
 
 
 class ScheduledTasksManager(threading.Thread):
     """
     Manage any tasks that Unmanic needs to execute at regular intervals
     """
 
-    def __init__(self):
+    def __init__(self, event):
         super(ScheduledTasksManager, self).__init__(name='ScheduledTasksManager')
         self.logger = None
+        self.event = event
         self.abort_flag = threading.Event()
         self.abort_flag.clear()
         self.scheduler = schedule.Scheduler()
         self.force_local_worker_timer = 0
 
     def _log(self, message, message2='', level="info"):
         if not self.logger:
@@ -63,16 +64,14 @@
         message = common.format_message(message, message2)
         getattr(self.logger, level)(message)
 
     def stop(self):
         self.abort_flag.set()
 
     def run(self):
-        # If we have a config set to run a schedule, then start the process.
-        # Otherwise close this thread now.
         self._log("Starting ScheduledTasks Monitor loop")
 
         # Create scheduled tasks
         # Check the session every 60 minutes
         self.scheduler.every(60).minutes.do(self.register_unmanic)
         # Run the plugin repo update every 3 hours
         self.scheduler.every(3).hours.do(self.plugin_repo_update)
@@ -82,15 +81,15 @@
         self.scheduler.every(1).minutes.do(self.set_worker_count_based_on_remote_installation_links)
         # Run a completed task cleanup every 60 minutes and on startup
         self.scheduler.every(12).hours.do(self.manage_completed_tasks)
         self.manage_completed_tasks()
 
         # Loop every 2 seconds to check if a task is due to be run
         while not self.abort_flag.is_set():
-            time.sleep(1)
+            self.event.wait(2)
             # Check if scheduled task is due
             self.scheduler.run_pending()
 
         # Clear any tasks and exit
         self.scheduler.clear()
         self._log("Leaving ScheduledTasks Monitor loop...")
```

### Comparing `unmanic-0.2.3/unmanic/libs/worker_group.py` & `unmanic-0.2.4/unmanic/libs/worker_group.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic/libs/db_migrate.py` & `unmanic-0.2.4/unmanic/libs/db_migrate.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,20 +28,20 @@
            OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
            OR OTHER DEALINGS IN THE SOFTWARE.
 
 """
 import importlib
 import inspect
 import os
+import sys
 
 from peewee import Model, SqliteDatabase, Field
-from peewee_migrate import Router
+from peewee_migrate import Migrator, Router
 
 from unmanic.libs import unlogger
-from unmanic.libs.unmodels import list_all_models
 from unmanic.libs.unmodels.lib import BaseModel
 
 
 class Migrations(object):
     """
     Migrations
 
@@ -64,14 +64,16 @@
             self.database = SqliteDatabase(config['FILE'])
 
             self.router = Router(database=self.database,
                                  migrate_table='migratehistory_{}'.format(config.get('MIGRATIONS_HISTORY_VERSION')),
                                  migrate_dir=config.get('MIGRATIONS_DIR'),
                                  logger=self.logger)
 
+            self.migrator = Migrator(self.database)
+
     def __log(self, message, level='info'):
         if self.logger:
             getattr(self.logger, level)(message)
         else:
             print(message)
 
     def __run_all_migrations(self):
@@ -92,60 +94,49 @@
             - rename a column/field
             - delete a column/field
             - delete a table/model
 
         :return:
         """
         # Fetch all model classes
-        all_models = []
-        all_base_models = []
-        for model in list_all_models():
-            imported_model = getattr(importlib.import_module("unmanic.libs.unmodels"), model)
-            if inspect.isclass(imported_model) and issubclass(imported_model, BaseModel):
-                # Add this model to both the 'all_models' list and our list of base models
-                all_models.append(imported_model)
-                all_base_models.append(imported_model)
-            elif inspect.isclass(imported_model) and issubclass(imported_model, Model):
-                # If the model is not one of the base models, it is an in-build model from peewee.
-                # For, this list of models we will not run a migration, but we will still ensure that the
-                #   table is created in the DB
-                all_models.append(imported_model)
-                pass
+        discovered_models = inspect.getmembers(sys.modules["unmanic.libs.unmodels"], inspect.isclass)
+        all_models = [tup[1] for tup in discovered_models]
 
         # Start by creating all models
         self.__log("Initialising database tables")
         try:
             with self.database.transaction():
                 for model in all_models:
-                    self.router.migrator.create_table(model)
-                self.router.migrator.run()
+                    self.migrator.create_table(model)
+                self.migrator.run()
         except Exception:
             self.database.rollback()
             self.__log("Initialising tables failed", level='exception')
             raise
 
         # Migrations will only be used for removing obsolete columns
         self.__run_all_migrations()
 
         # Newly added fields can be auto added with this function... no need for a migration script
         # Ensure all files are also present for each of the model classes
         self.__log("Updating database fields")
-        for model in all_base_models:
-            # Fetch all peewee fields for the model class
-            # https://stackoverflow.com/questions/22573558/peewee-determining-meta-data-about-model-at-run-time
-            fields = model._meta.fields
-            # loop over the fields and ensure each on exists in the table
-            field_keys = [f for f in fields]
-            for fk in field_keys:
-                field = fields.get(fk)
-                if isinstance(field, Field):
-                    if not any(f for f in self.database.get_columns(model._meta.name) if f.name == field.name):
-                        # Field does not exist in DB table
-                        self.__log("Adding missing column")
-                        try:
-                            with self.database.transaction():
-                                self.router.migrator.add_columns(model, **{field.name: field})
-                                self.router.migrator.run()
-                        except Exception:
-                            self.database.rollback()
-                            self.__log("Update failed", level='exception')
-                            raise
+        for model in all_models:
+            if issubclass(model, BaseModel):
+                # Fetch all peewee fields for the model class
+                # https://stackoverflow.com/questions/22573558/peewee-determining-meta-data-about-model-at-run-time
+                fields = model._meta.fields
+                # loop over the fields and ensure each on exists in the table
+                field_keys = [f for f in fields]
+                for fk in field_keys:
+                    field = fields.get(fk)
+                    if isinstance(field, Field):
+                        if not any(f for f in self.database.get_columns(model._meta.name) if f.name == field.name):
+                            # Field does not exist in DB table
+                            self.__log("Adding missing column")
+                            try:
+                                with self.database.transaction():
+                                    self.migrator.add_columns(model, **{field.name: field})
+                                    self.migrator.run()
+                            except Exception:
+                                self.database.rollback()
+                                self.__log("Update failed", level='exception')
+                                raise
```

### Comparing `unmanic-0.2.3/unmanic/libs/workers.py` & `unmanic-0.2.4/unmanic/libs/workers.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,20 @@
     worker_subprocess = None
     worker_subprocess_pid = None
     worker_subprocess_percent = None
     worker_subprocess_elapsed = None
 
     worker_runners_info = {}
 
-    def __init__(self, thread_id, name, worker_group_id, pending_queue, complete_queue):
+    def __init__(self, thread_id, name, worker_group_id, pending_queue, complete_queue, event):
         super(Worker, self).__init__(name=name)
         self.thread_id = thread_id
         self.name = name
         self.worker_group_id = worker_group_id
+        self.event = event
 
         self.current_task = None
         self.pending_queue = pending_queue
         self.complete_queue = complete_queue
 
         # Create 'redundancy' flag. When this is set, the worker should die
         self.redundant_flag = threading.Event()
@@ -96,30 +97,30 @@
     def _log(self, message, message2='', level="info"):
         message = common.format_message(message, message2)
         getattr(self.logger, level)(message)
 
     def run(self):
         self._log("Starting worker")
         while not self.redundant_flag.is_set():
-            time.sleep(.2)  # Add delay for preventing loop maxing compute resources
+            self.event.wait(1)  # Add delay for preventing loop maxing compute resources
 
             # If the Foreman has paused this worker, then don't do anything
             if self.paused_flag.is_set():
                 self.paused = True
                 # If the worker is paused, wait for 5 seconds before continuing the loop
-                time.sleep(5)
+                self.event.wait(5)
                 continue
             self.paused = False
 
             # Set the worker as Idle - This will announce to the Foreman that it's ready for a task
             self.idle = True
 
             # Wait for task
             while not self.redundant_flag.is_set() and self.current_task:
-                time.sleep(.2)  # Add delay for preventing loop maxing compute resources
+                self.event.wait(.5)  # Add delay for preventing loop maxing compute resources
 
                 try:
                     # Process the set task
                     self.__process_task_queue_item()
                 except queue.Empty:
                     continue
                 except Exception as e:
@@ -345,15 +346,15 @@
                 data['exec_command'] = []
                 data['command_progress_parser'] = default_progress_parser
                 data['file_in'] = file_in
                 data['file_out'] = file_out
                 data['original_file_path'] = original_abspath
                 data['repeat'] = False
 
-                time.sleep(.2)  # Add delay for preventing loop maxing compute resources
+                self.event.wait(.2)  # Add delay for preventing loop maxing compute resources
                 self.worker_log.append("\n\nRUNNER: \n{} [Pass #{}]\n\n".format(plugin_module.get('name'), runner_pass_count))
                 self.worker_log.append("\nExecuting plugin runner... Please wait\n")
 
                 # Run plugin to update data
                 if not plugin_handler.exec_plugin_runner(data, plugin_module.get('plugin_id'), 'worker.process_item'):
                     # Skip this plugin module's loop
                     self.worker_runners_info[plugin_module.get('plugin_id')]['status'] = 'complete'
@@ -426,15 +427,15 @@
 
                         # Ensure the new 'file_in' is set to the previous runner's 'file_in' for the next loop
                         file_in = data.get("file_in")
                 else:
                     # Ensure the new 'file_in' is set to the previous runner's 'file_in' for the next loop
                     file_in = data.get("file_in")
                     # Log that this plugin did not request to execute anything
-                    self.worker_log.append("\nRunner did not request to execute a command")
+                    self.worker_log.append("\nRunner did not request for Unmanic to execute a command")
                     self._log(
                         "Worker process '{}' did not request to execute a command.".format(plugin_module.get('plugin_id')),
                         level='debug')
 
                 if os.path.exists(data.get('file_out')):
                     # Set the current file out to the most recently completed cache file
                     # If the file out does not exist, it is likely never used by the plugin.
@@ -451,16 +452,16 @@
 
             self.worker_runners_info[plugin_module.get('plugin_id')]['success'] = True
             self.worker_runners_info[plugin_module.get('plugin_id')]['status'] = 'complete'
 
         # Log if no command was run by any Plugins
         if no_exec_command_run:
             # If no jobs were carried out on this task
-            self._log("No Plugin requested to run commands for this file '{}'".format(original_abspath), level='warning')
-            self.worker_log.append("\n\nNo Plugin requested to run commands for this file '{}'".format(original_abspath))
+            self._log("No Plugin requested for Unmanic to run commands for this file '{}'".format(original_abspath), level='warning')
+            self.worker_log.append("\n\nNo Plugin requested for Unmanic to run commands for this file '{}'".format(original_abspath))
 
         # Save the completed command log
         self.current_task.save_command_log(self.worker_log)
 
         # If all plugins that were executed completed successfully, then this was overall a successful task.
         # At this point we need to move the final out file to the original task cache path so the postprocessor can collect it.
         if overall_success:
@@ -483,15 +484,15 @@
 
                 # There is a really odd intermittent bug with the shutil module that is causing it to
                 #   sometimes report that the file does not exist.
                 # This section adds a small pause and logs the error if that is the case.
                 # I have not yet figured out a solution as this is difficult to reproduce.
                 if not os.path.exists(current_file_out):
                     self._log("Error - current_file_out path does not exist! '{}'".format(file_in), level="error")
-                    time.sleep(1)
+                    self.event.wait(1)
 
                 # Ensure the cache directory exists
                 if not os.path.exists(cache_directory):
                     os.makedirs(cache_directory)
 
                 # Check that the current file out is not the original source file
                 if os.path.abspath(current_file_out) == os.path.abspath(original_abspath):
@@ -636,15 +637,15 @@
                 # Then resume it when the worker is resumed
                 if self.paused_flag.is_set():
                     self._log("Pausing PID {}".format(sub_proc.pid), level='debug')
                     proc.suspend()
                     self.paused = True
                     start_pause = time.time()
                     while not self.redundant_flag.is_set():
-                        time.sleep(1)
+                        self.event.wait(1)
                         if not self.paused_flag.is_set():
                             self._log("Resuming PID {}".format(sub_proc.pid), level='debug')
                             proc.resume()
                             self.paused = False
                             # Elapsed time is used for calculating etc.
                             # We account for this by counting the time we are paused also.
                             # This is then subtracted from the elapsed time in the calculation above.
```

### Comparing `unmanic-0.2.3/unmanic/metadata.py` & `unmanic-0.2.4/unmanic/metadata.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/unmanic.egg-info/SOURCES.txt` & `unmanic-0.2.4/unmanic.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 unmanic/libs/fileinfo.py
 unmanic/libs/filetest.py
 unmanic/libs/foreman.py
 unmanic/libs/history.py
 unmanic/libs/installation_link.py
 unmanic/libs/library.py
 unmanic/libs/libraryscanner.py
+unmanic/libs/notifications.py
 unmanic/libs/plugins.py
 unmanic/libs/postprocessor.py
 unmanic/libs/scheduler.py
 unmanic/libs/session.py
 unmanic/libs/singleton.py
 unmanic/libs/system.py
 unmanic/libs/task.py
@@ -133,14 +134,15 @@
 unmanic/webserver/api_v1/session_api.py
 unmanic/webserver/api_v2/README.md
 unmanic/webserver/api_v2/__init__.py
 unmanic/webserver/api_v2/base_api_handler.py
 unmanic/webserver/api_v2/docs_api.py
 unmanic/webserver/api_v2/filebrowser_api.py
 unmanic/webserver/api_v2/history_api.py
+unmanic/webserver/api_v2/notifications_api.py
 unmanic/webserver/api_v2/pending_api.py
 unmanic/webserver/api_v2/plugins_api.py
 unmanic/webserver/api_v2/session_api.py
 unmanic/webserver/api_v2/settings_api.py
 unmanic/webserver/api_v2/upload_api.py
 unmanic/webserver/api_v2/version_api.py
 unmanic/webserver/api_v2/workers_api.py
@@ -173,48 +175,51 @@
 unmanic/webserver/frontend/src/assets/bg-md1.jpg
 unmanic/webserver/frontend/src/assets/coffee-btn-image.png
 unmanic/webserver/frontend/src/assets/logo-lg.png
 unmanic/webserver/frontend/src/assets/logo.png
 unmanic/webserver/frontend/src/assets/quasar-logo-vertical.svg
 unmanic/webserver/frontend/src/assets/unmanic-logo-white.png
 unmanic/webserver/frontend/src/boot/axios.js
+unmanic/webserver/frontend/src/boot/global-event-bus.js
 unmanic/webserver/frontend/src/boot/i18n.js
 unmanic/webserver/frontend/src/components/Avatar.vue
 unmanic/webserver/frontend/src/components/CompletedTaskLogDialog.vue
 unmanic/webserver/frontend/src/components/CompletedTasks.vue
 unmanic/webserver/frontend/src/components/CompletedTasksTable.vue
 unmanic/webserver/frontend/src/components/DirectoryBrowserDialog.vue
 unmanic/webserver/frontend/src/components/DrawerDataPanelsNav.vue
 unmanic/webserver/frontend/src/components/DrawerMainNav.vue
+unmanic/webserver/frontend/src/components/DrawerNotifications.vue
 unmanic/webserver/frontend/src/components/DrawerSettingsNav.vue
 unmanic/webserver/frontend/src/components/EssentialLink.vue
 unmanic/webserver/frontend/src/components/FooterData.vue
 unmanic/webserver/frontend/src/components/JsonImportExportDialog.vue
 unmanic/webserver/frontend/src/components/LanguageSwitch.vue
-unmanic/webserver/frontend/src/components/LibraryConfigureDialog.vue
 unmanic/webserver/frontend/src/components/LibraryConfigurePluginFlowList.vue
 unmanic/webserver/frontend/src/components/LinkConfigureDialog.vue
 unmanic/webserver/frontend/src/components/LoginDialog.vue
 unmanic/webserver/frontend/src/components/MarkdownDialog.vue
 unmanic/webserver/frontend/src/components/MobileSettingsQuickNav.vue
 unmanic/webserver/frontend/src/components/PendingTasks.vue
 unmanic/webserver/frontend/src/components/PendingTasksTable.vue
-unmanic/webserver/frontend/src/components/PluginInfo.vue
-unmanic/webserver/frontend/src/components/PluginInstallerDialog.vue
 unmanic/webserver/frontend/src/components/PluginInstallerManageRepos.vue
 unmanic/webserver/frontend/src/components/PluginSelectorDialog.vue
 unmanic/webserver/frontend/src/components/PluginsInstalledTable.vue
 unmanic/webserver/frontend/src/components/ReleaseNotesDialog.vue
 unmanic/webserver/frontend/src/components/ThemeSwitch.vue
 unmanic/webserver/frontend/src/components/WorkerEventCreateDialog.vue
 unmanic/webserver/frontend/src/components/WorkerGroupConfigureDialog.vue
 unmanic/webserver/frontend/src/components/WorkerProgress.vue
 unmanic/webserver/frontend/src/components/WorkerProgressLog.vue
 unmanic/webserver/frontend/src/components/WorkerProgressStatus.vue
 unmanic/webserver/frontend/src/components/iframe-directive.js
+unmanic/webserver/frontend/src/components/dialogs/ConfigDrawerDialog.vue
+unmanic/webserver/frontend/src/components/dialogs/PluginInfoDialog.vue
+unmanic/webserver/frontend/src/components/forms/LibraryConfigForm.vue
+unmanic/webserver/frontend/src/components/forms/PluginInstallerForm.vue
 unmanic/webserver/frontend/src/css/app.scss
 unmanic/webserver/frontend/src/css/markdown-admonitions.css
 unmanic/webserver/frontend/src/css/quasar.variables.scss
 unmanic/webserver/frontend/src/js/dateTools.js
 unmanic/webserver/frontend/src/js/markupParser.js
 unmanic/webserver/frontend/src/js/unmanicGlobals.js
 unmanic/webserver/frontend/src/js/unmanicWebsocket.js
```

### Comparing `unmanic-0.2.3/unmanic.egg-info/PKG-INFO` & `unmanic-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unmanic
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple tool for optimising your video library to a single format
 Home-page: https://github.com/Josh5/unmanic
 Author: Josh.5
 Author-email: jsunnex@gmail.com
 Maintainer: Josh.5
 Maintainer-email: jsunnex@gmail.com
 License: GPLv3
@@ -90,15 +90,15 @@
         
         ## Install and Run
         
         For up-to-date installation instructions, follow the [Unmanic documentation](https://docs.unmanic.app/docs/)
         
         To run from source:
         
-        1) Install the Python dependencies listed above hen run:
+        1) Install the Python dependencies listed above then run:
         2) Run:
             ```
             # Ensure the submodules are checked out
             git submodule update --init --recursive
             
             # Build and install the project into your home directory
             python3 ./setup.py install --user
@@ -803,18 +803,20 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Multimedia :: Video :: Conversion
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unmanic Version: 0.2.3 Summary: A simple tool for
+Metadata-Version: 2.1 Name: unmanic Version: 0.2.4 Summary: A simple tool for
 optimising your video library to a single format Home-page: https://github.com/
 Josh5/unmanic Author: Josh.5 Author-email: jsunnex@gmail.com Maintainer: Josh.5
 Maintainer-email: jsunnex@gmail.com License: GPLv3 Description: Unmanic -
 Library Optimiser =========================== ![UNMANIC - Library Optimiser]
 (https://github.com/unmanic/unmanic/raw/master/logo.png) [Buy_Me_a_Coffee_at
 ko-fi.com] [![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/
 unmanic/
@@ -72,15 +72,15 @@
 required dependencies for those commands are installed. ## Screen-shots ####
 Dashboard: ![Screen-shot - Dashboard](./docs/images/unmanic-dashboard-
 processing-anime.png) #### File metrics: ![Screen-shot - Desktop](./docs/
 images/unmanic-file-size-data-panel-anime.png) #### Installed plugins: !
 [Screen-shot - Desktop](./docs/images/unmanic-list-installed-plugins.png) ##
 Install and Run For up-to-date installation instructions, follow the [Unmanic
 documentation](https://docs.unmanic.app/docs/) To run from source: 1) Install
-the Python dependencies listed above hen run: 2) Run: ``` # Ensure the
+the Python dependencies listed above then run: 2) Run: ``` # Ensure the
 submodules are checked out git submodule update --init --recursive # Build and
 install the project into your home directory python3 ./setup.py install --user
 # Run Unmanic unmanic ``` ## License and Contribution This projected is
 licensed under th GPL version 3. Copyright (C) Josh Sunnex - All Rights
 Reserved Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
@@ -540,14 +540,15 @@
 subroutine library, you may consider it more useful to permit linking
 proprietary applications with the library. If this is what you want to do, use
 the GNU Lesser General Public License instead of this License. But first,
 please read
 www.gnu.org/licenses/why-not-lgpl.html>. Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Operating System :: POSIX :: Linux Classifier: Operating System :: Unix
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Topic :: Multimedia :: Video :: Conversion Classifier: Topic ::
-Internet :: WWW/HTTP Requires-Python: >=3.6 Description-Content-Type: text/
-markdown Provides-Extra: dev
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Operating System :: POSIX :: Linux Classifier:
+Operating System :: Unix Classifier: License :: OSI Approved :: GNU General
+Public License v3 (GPLv3) Classifier: Topic :: Multimedia :: Video ::
+Conversion Classifier: Topic :: Internet :: WWW/HTTP Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: dev
```

### Comparing `unmanic-0.2.3/LICENSE` & `unmanic-0.2.4/unmanic/webserver/frontend/LICENSE`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.3/README.md` & `unmanic-0.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 ## Install and Run
 
 For up-to-date installation instructions, follow the [Unmanic documentation](https://docs.unmanic.app/docs/)
 
 To run from source:
 
-1) Install the Python dependencies listed above hen run:
+1) Install the Python dependencies listed above then run:
 2) Run:
     ```
     # Ensure the submodules are checked out
     git submodule update --init --recursive
     
     # Build and install the project into your home directory
     python3 ./setup.py install --user
```

#### html2text {}

```diff
@@ -68,15 +68,15 @@
 required dependencies for those commands are installed. ## Screen-shots ####
 Dashboard: ![Screen-shot - Dashboard](./docs/images/unmanic-dashboard-
 processing-anime.png) #### File metrics: ![Screen-shot - Desktop](./docs/
 images/unmanic-file-size-data-panel-anime.png) #### Installed plugins: !
 [Screen-shot - Desktop](./docs/images/unmanic-list-installed-plugins.png) ##
 Install and Run For up-to-date installation instructions, follow the [Unmanic
 documentation](https://docs.unmanic.app/docs/) To run from source: 1) Install
-the Python dependencies listed above hen run: 2) Run: ``` # Ensure the
+the Python dependencies listed above then run: 2) Run: ``` # Ensure the
 submodules are checked out git submodule update --init --recursive # Build and
 install the project into your home directory python3 ./setup.py install --user
 # Run Unmanic unmanic ``` ## License and Contribution This projected is
 licensed under th GPL version 3. Copyright (C) Josh Sunnex - All Rights
 Reserved Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
```

### Comparing `unmanic-0.2.3/PKG-INFO` & `unmanic-0.2.4/unmanic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unmanic
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple tool for optimising your video library to a single format
 Home-page: https://github.com/Josh5/unmanic
 Author: Josh.5
 Author-email: jsunnex@gmail.com
 Maintainer: Josh.5
 Maintainer-email: jsunnex@gmail.com
 License: GPLv3
@@ -90,15 +90,15 @@
         
         ## Install and Run
         
         For up-to-date installation instructions, follow the [Unmanic documentation](https://docs.unmanic.app/docs/)
         
         To run from source:
         
-        1) Install the Python dependencies listed above hen run:
+        1) Install the Python dependencies listed above then run:
         2) Run:
             ```
             # Ensure the submodules are checked out
             git submodule update --init --recursive
             
             # Build and install the project into your home directory
             python3 ./setup.py install --user
@@ -803,18 +803,20 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Multimedia :: Video :: Conversion
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unmanic Version: 0.2.3 Summary: A simple tool for
+Metadata-Version: 2.1 Name: unmanic Version: 0.2.4 Summary: A simple tool for
 optimising your video library to a single format Home-page: https://github.com/
 Josh5/unmanic Author: Josh.5 Author-email: jsunnex@gmail.com Maintainer: Josh.5
 Maintainer-email: jsunnex@gmail.com License: GPLv3 Description: Unmanic -
 Library Optimiser =========================== ![UNMANIC - Library Optimiser]
 (https://github.com/unmanic/unmanic/raw/master/logo.png) [Buy_Me_a_Coffee_at
 ko-fi.com] [![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/
 unmanic/
@@ -72,15 +72,15 @@
 required dependencies for those commands are installed. ## Screen-shots ####
 Dashboard: ![Screen-shot - Dashboard](./docs/images/unmanic-dashboard-
 processing-anime.png) #### File metrics: ![Screen-shot - Desktop](./docs/
 images/unmanic-file-size-data-panel-anime.png) #### Installed plugins: !
 [Screen-shot - Desktop](./docs/images/unmanic-list-installed-plugins.png) ##
 Install and Run For up-to-date installation instructions, follow the [Unmanic
 documentation](https://docs.unmanic.app/docs/) To run from source: 1) Install
-the Python dependencies listed above hen run: 2) Run: ``` # Ensure the
+the Python dependencies listed above then run: 2) Run: ``` # Ensure the
 submodules are checked out git submodule update --init --recursive # Build and
 install the project into your home directory python3 ./setup.py install --user
 # Run Unmanic unmanic ``` ## License and Contribution This projected is
 licensed under th GPL version 3. Copyright (C) Josh Sunnex - All Rights
 Reserved Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
@@ -540,14 +540,15 @@
 subroutine library, you may consider it more useful to permit linking
 proprietary applications with the library. If this is what you want to do, use
 the GNU Lesser General Public License instead of this License. But first,
 please read
 www.gnu.org/licenses/why-not-lgpl.html>. Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Operating System :: POSIX :: Linux Classifier: Operating System :: Unix
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Topic :: Multimedia :: Video :: Conversion Classifier: Topic ::
-Internet :: WWW/HTTP Requires-Python: >=3.6 Description-Content-Type: text/
-markdown Provides-Extra: dev
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Operating System :: POSIX :: Linux Classifier:
+Operating System :: Unix Classifier: License :: OSI Approved :: GNU General
+Public License v3 (GPLv3) Classifier: Topic :: Multimedia :: Video ::
+Conversion Classifier: Topic :: Internet :: WWW/HTTP Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: dev
```

### Comparing `unmanic-0.2.3/MANIFEST.in` & `unmanic-0.2.4/MANIFEST.in`

 * *Files identical despite different names*

