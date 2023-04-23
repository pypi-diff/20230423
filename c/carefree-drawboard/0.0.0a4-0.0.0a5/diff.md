# Comparing `tmp/carefree-drawboard-0.0.0a4.tar.gz` & `tmp/carefree-drawboard-0.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-drawboard-0.0.0a4.tar", last modified: Tue Apr 18 10:07:58 2023, max compression
+gzip compressed data, was "carefree-drawboard-0.0.0a5.tar", last modified: Sun Apr 23 09:52:59 2023, max compression
```

## Comparing `carefree-drawboard-0.0.0a4.tar` & `carefree-drawboard-0.0.0a5.tar`

### file list

```diff
@@ -1,192 +1,196 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.854997 carefree-drawboard-0.0.0a4/
--rw-rw-rw-   0        0        0    11557 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a4/LICENSE
--rw-rw-rw-   0        0        0      121 2023-04-18 10:04:06.000000 carefree-drawboard-0.0.0a4/MANIFEST.in
--rw-rw-rw-   0        0        0     9076 2023-04-18 10:07:58.854997 carefree-drawboard-0.0.0a4/PKG-INFO
--rw-rw-rw-   0        0        0     8793 2023-04-18 02:22:15.000000 carefree-drawboard-0.0.0a4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.781726 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/
--rw-rw-rw-   0        0        0     9076 2023-04-18 10:07:57.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5363 2023-04-18 10:07:58.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 10:07:57.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 10:07:57.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      155 2023-04-18 10:07:57.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 10:07:57.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.783719 carefree-drawboard-0.0.0a4/cfdraw/
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.786709 carefree-drawboard-0.0.0a4/cfdraw/.web/
--rw-rw-rw-   0        0        0      121 2023-04-18 05:54:36.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/.env
--rw-rw-rw-   0        0        0      143 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/.prettierrc
--rw-rw-rw-   0        0        0      323 2023-04-13 08:34:20.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/index.html
--rw-rw-rw-   0        0        0     1628 2023-04-18 02:10:06.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/package.json
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.789699 carefree-drawboard-0.0.0a4/cfdraw/.web/src/
--rw-rw-rw-   0        0        0      895 2023-04-18 10:06:42.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/App.tsx
--rw-rw-rw-   0        0        0     1453 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/BoardPanel.tsx
--rw-rw-rw-   0        0        0     5434 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/_settings.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.794683 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/
--rw-rw-rw-   0        0        0     2263 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/addImage.ts
--rw-rw-rw-   0        0        0      960 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/addText.ts
--rw-rw-rw-   0        0        0     9573 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/arrange.ts
--rw-rw-rw-   0        0        0     1930 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/download.ts
--rw-rw-rw-   0        0        0     2174 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/export.ts
--rw-rw-rw-   0        0        0     5947 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/importMeta.ts
--rw-rw-rw-   0        0        0     1286 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/managePlugins.ts
--rw-rw-rw-   0        0        0     3528 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/manageProjects.ts
--rw-rw-rw-   0        0        0      272 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/update.ts
--rw-rw-rw-   0        0        0     1175 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/uploadImage.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.750433 carefree-drawboard-0.0.0a4/cfdraw/.web/src/assets/
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.794683 carefree-drawboard-0.0.0a4/cfdraw/.web/src/assets/icons/
--rw-rw-rw-   0        0        0      257 2022-10-23 15:19:01.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/assets/icons/arrow-down.svg
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.798669 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/
--rw-rw-rw-   0        0        0      353 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFButton.tsx
--rw-rw-rw-   0        0        0      359 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFDivider.tsx
--rw-rw-rw-   0        0        0      243 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFHeading.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.799667 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFIcon/
--rw-rw-rw-   0        0        0      546 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFIcon/index.scss
--rw-rw-rw-   0        0        0     1568 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFIcon/index.tsx
--rw-rw-rw-   0        0        0     1568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFImageUploader.tsx
--rw-rw-rw-   0        0        0      346 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFInput.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.800663 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSelect/
--rw-rw-rw-   0        0        0       70 2023-04-07 06:01:04.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSelect/index.scss
--rw-rw-rw-   0        0        0     3483 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSelect/index.tsx
--rw-rw-rw-   0        0        0     4606 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSlider.tsx
--rw-rw-rw-   0        0        0     1644 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSwitch.tsx
--rw-rw-rw-   0        0        0      324 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFText.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.802656 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/
--rw-rw-rw-   0        0        0     3110 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useFileDropper.ts
--rw-rw-rw-   0        0        0     4289 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useGridLines.ts
--rw-rw-rw-   0        0        0     2940 2023-04-17 06:33:19.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useInitBoard.ts
--rw-rw-rw-   0        0        0      445 2023-04-11 05:03:17.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/usePreventDefaults.ts
--rw-rw-rw-   0        0        0     5003 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/usePython.ts
--rw-rw-rw-   0        0        0      394 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useUndoRedo.ts
--rw-rw-rw-   0        0        0      131 2023-04-07 08:12:13.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/index.scss
--rw-rw-rw-   0        0        0      345 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/index.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.806643 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/
--rw-rw-rw-   0        0        0      792 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/add.ts
--rw-rw-rw-   0        0        0      849 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/brush.ts
--rw-rw-rw-   0        0        0     1148 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/download.ts
--rw-rw-rw-   0        0        0     1436 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/index.ts
--rw-rw-rw-   0        0        0      404 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/nodeEditor.ts
--rw-rw-rw-   0        0        0     2283 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/plugins.ts
--rw-rw-rw-   0        0        0     1746 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/projects.ts
--rw-rw-rw-   0        0        0      896 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/settings.ts
--rw-rw-rw-   0        0        0     6568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/toast.ts
--rw-rw-rw-   0        0        0     1472 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/ui.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.810629 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/
--rw-rw-rw-   0        0        0     2839 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/AddPlugin.tsx
--rw-rw-rw-   0        0        0      870 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/ArrangePlugin.tsx
--rw-rw-rw-   0        0        0     4801 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/BrushPlugin.tsx
--rw-rw-rw-   0        0        0      879 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/DeletePlugin.tsx
--rw-rw-rw-   0        0        0     3545 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/DownloadPlugin.tsx
--rw-rw-rw-   0        0        0     1067 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/GroupPlugin.tsx
--rw-rw-rw-   0        0        0     1101 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/LinksPlugin.tsx
--rw-rw-rw-   0        0        0     6511 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/ProjectPlugin.tsx
--rw-rw-rw-   0        0        0     5093 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/SettingsPlugin.tsx
--rw-rw-rw-   0        0        0     2366 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/TextEditorPlugin.tsx
--rw-rw-rw-   0        0        0      906 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.813619 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/
--rw-rw-rw-   0        0        0     3607 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpFieldsPlugin.tsx
--rw-rw-rw-   0        0        0     2064 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpPluginWithSubmit.tsx
--rw-rw-rw-   0        0        0     1951 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpQAPlugin.tsx
--rw-rw-rw-   0        0        0     1602 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpTextAreaPlugin.tsx
--rw-rw-rw-   0        0        0      258 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.814615 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.817607 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/
--rw-rw-rw-   0        0        0     1411 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
--rw-rw-rw-   0        0        0      693 2023-04-13 06:08:57.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
--rw-rw-rw-   0        0        0      854 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
--rw-rw-rw-   0        0        0     1133 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/index.tsx
--rw-rw-rw-   0        0        0      614 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/utils.ts
--rw-rw-rw-   0        0        0     7481 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Floating.tsx
--rw-rw-rw-   0        0        0      307 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Link.tsx
--rw-rw-rw-   0        0        0     7048 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Render.tsx
--rw-rw-rw-   0        0        0     2318 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/index.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.818604 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/utils/
--rw-rw-rw-   0        0        0     1575 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/utils/factory.ts
--rw-rw-rw-   0        0        0      583 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/utils/renderFilters.ts
--rw-rw-rw-   0        0        0      841 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/react-app-env.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.819600 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/
--rw-rw-rw-   0        0        0      922 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/actions.ts
--rw-rw-rw-   0        0        0     3555 2023-04-17 15:25:00.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.821593 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/interceptors/
--rw-rw-rw-   0        0        0      880 2023-04-17 14:19:55.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/interceptors/_python.ts
--rw-rw-rw-   0        0        0      752 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/interceptors/index.ts
--rw-rw-rw-   0        0        0       38 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/reset.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.826578 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/
--rw-rw-rw-   0        0        0     3348 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/_python.ts
--rw-rw-rw-   0        0        0     1607 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/meta.ts
--rw-rw-rw-   0        0        0     1169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/metaFields.ts
--rw-rw-rw-   0        0        0      289 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/misc.ts
--rw-rw-rw-   0        0        0     3169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/plugins.ts
--rw-rw-rw-   0        0        0      850 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/requests.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.832561 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/
--rw-rw-rw-   0        0        0     1431 2023-04-17 09:56:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/_python.ts
--rw-rw-rw-   0        0        0     1495 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/gridLines.ts
--rw-rw-rw-   0        0        0      578 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/hooks.ts
--rw-rw-rw-   0        0        0      468 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/init.ts
--rw-rw-rw-   0        0        0     1107 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/meta.ts
--rw-rw-rw-   0        0        0     1561 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/plugins.ts
--rw-rw-rw-   0        0        0     1704 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/projects.ts
--rw-rw-rw-   0        0        0     3285 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/theme.ts
--rw-rw-rw-   0        0        0     2025 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/ui.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.835551 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/
--rw-rw-rw-   0        0        0      467 2023-04-07 05:25:36.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/bem.ts
--rw-rw-rw-   0        0        0      466 2023-04-17 06:32:01.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/constants.ts
--rw-rw-rw-   0        0        0      934 2023-04-06 06:11:04.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/event.ts
--rw-rw-rw-   0        0        0     1025 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/misc.ts
--rw-rw-rw-   0        0        0      633 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/toast.ts
--rw-rw-rw-   0        0        0       39 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/vite-env.d.ts
--rw-rw-rw-   0        0        0      656 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/tsconfig.json
--rw-rw-rw-   0        0        0      193 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/tsconfig.node.json
--rw-rw-rw-   0        0        0      103 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/tsconfig.paths.json
--rw-rw-rw-   0        0        0     1849 2023-04-18 03:53:52.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/vite.config.ts
--rw-rw-rw-   0        0        0   214083 2023-04-18 03:11:54.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/yarn.lock
--rw-rw-rw-   0        0        0      405 2023-04-13 06:43:12.000000 carefree-drawboard-0.0.0a4/cfdraw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.837544 carefree-drawboard-0.0.0a4/cfdraw/app/
--rw-rw-rw-   0        0        0       20 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/app/__init__.py
--rw-rw-rw-   0        0        0     3022 2023-04-18 07:46:59.000000 carefree-drawboard-0.0.0a4/cfdraw/app/app.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.840534 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/
--rw-rw-rw-   0        0        0      118 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/__init__.py
--rw-rw-rw-   0        0        0      493 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/base.py
--rw-rw-rw-   0        0        0     1944 2023-04-18 06:33:13.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/plugins.py
--rw-rw-rw-   0        0        0     5713 2023-04-17 13:23:53.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/project.py
--rw-rw-rw-   0        0        0     1813 2023-04-18 02:06:49.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/upload.py
--rw-rw-rw-   0        0        0     2974 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/websocket.py
--rw-rw-rw-   0        0        0      519 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/app/schema.py
--rw-rw-rw-   0        0        0     3485 2023-04-18 08:00:45.000000 carefree-drawboard-0.0.0a4/cfdraw/cli.py
--rw-rw-rw-   0        0        0     2226 2023-04-18 07:55:50.000000 carefree-drawboard-0.0.0a4/cfdraw/config.py
--rw-rw-rw-   0        0        0     1479 2023-04-18 07:48:42.000000 carefree-drawboard-0.0.0a4/cfdraw/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.841530 carefree-drawboard-0.0.0a4/cfdraw/parsers/
--rw-rw-rw-   0        0        0       44 2023-04-09 01:57:56.000000 carefree-drawboard-0.0.0a4/cfdraw/parsers/__init__.py
--rw-rw-rw-   0        0        0      609 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a4/cfdraw/parsers/chakra.py
--rw-rw-rw-   0        0        0     6203 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/parsers/noli.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.843524 carefree-drawboard-0.0.0a4/cfdraw/plugins/
--rw-rw-rw-   0        0        0      113 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/__init__.py
--rw-rw-rw-   0        0        0     4367 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/base.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.843524 carefree-drawboard-0.0.0a4/cfdraw/plugins/community/
--rw-rw-rw-   0        0        0        0 2023-04-14 05:16:37.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/community/__init__.py
--rw-rw-rw-   0        0        0     2407 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/factory.py
--rw-rw-rw-   0        0        0     1956 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/meta.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.845027 carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/
--rw-rw-rw-   0        0        0       71 2023-04-13 03:23:59.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/__init__.py
--rw-rw-rw-   0        0        0     1167 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/fields.py
--rw-rw-rw-   0        0        0      671 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/text_area.py
--rw-rw-rw-   0        0        0      795 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/timer.py
--rw-rw-rw-   0        0        0     1090 2023-04-17 09:56:46.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/sync.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.847024 carefree-drawboard-0.0.0a4/cfdraw/schema/
--rw-rw-rw-   0        0        0       47 2023-04-13 15:19:11.000000 carefree-drawboard-0.0.0a4/cfdraw/schema/__init__.py
--rw-rw-rw-   0        0        0     3157 2023-04-13 06:12:19.000000 carefree-drawboard-0.0.0a4/cfdraw/schema/fields.py
--rw-rw-rw-   0        0        0     9673 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/schema/plugins.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.849017 carefree-drawboard-0.0.0a4/cfdraw/server/
--rw-rw-rw-   0        0        0     1194 2023-04-18 09:42:33.000000 carefree-drawboard-0.0.0a4/cfdraw/server/__init__.py
--rw-rw-rw-   0        0        0     1185 2023-04-18 07:04:07.000000 carefree-drawboard-0.0.0a4/cfdraw/server/http.py
--rw-rw-rw-   0        0        0      381 2023-04-18 07:40:33.000000 carefree-drawboard-0.0.0a4/cfdraw/server/index.py
--rw-rw-rw-   0        0        0     1459 2023-04-18 07:40:19.000000 carefree-drawboard-0.0.0a4/cfdraw/server/socket.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.854001 carefree-drawboard-0.0.0a4/cfdraw/utils/
--rw-rw-rw-   0        0        0        0 2023-04-08 03:23:05.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/cache.py
--rw-rw-rw-   0        0        0      875 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/console.py
--rw-rw-rw-   0        0        0     2781 2023-04-18 07:55:53.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/exec.py
--rw-rw-rw-   0        0        0      638 2023-04-17 03:07:08.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/prerequisites.py
--rw-rw-rw-   0        0        0     1766 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/processes.py
--rw-rw-rw-   0        0        0     3667 2023-04-17 13:24:23.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/server.py
--rw-rw-rw-   0        0        0     2733 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/template.py
--rw-rw-rw-   0        0        0      113 2023-04-18 10:07:58.855994 carefree-drawboard-0.0.0a4/setup.cfg
--rw-rw-rw-   0        0        0     1054 2023-04-18 10:07:27.000000 carefree-drawboard-0.0.0a4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.377564 carefree-drawboard-0.0.0a5/
+-rw-rw-rw-   0        0        0    11557 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a5/LICENSE
+-rw-rw-rw-   0        0        0      121 2023-04-18 10:04:06.000000 carefree-drawboard-0.0.0a5/MANIFEST.in
+-rw-rw-rw-   0        0        0     9026 2023-04-23 09:52:59.378564 carefree-drawboard-0.0.0a5/PKG-INFO
+-rw-rw-rw-   0        0        0     8743 2023-04-21 04:33:50.000000 carefree-drawboard-0.0.0a5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.299776 carefree-drawboard-0.0.0a5/carefree_drawboard.egg-info/
+-rw-rw-rw-   0        0        0     9026 2023-04-23 09:52:57.000000 carefree-drawboard-0.0.0a5/carefree_drawboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5586 2023-04-23 09:52:59.000000 carefree-drawboard-0.0.0a5/carefree_drawboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 09:52:57.000000 carefree-drawboard-0.0.0a5/carefree_drawboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 09:52:57.000000 carefree-drawboard-0.0.0a5/carefree_drawboard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      164 2023-04-23 09:52:57.000000 carefree-drawboard-0.0.0a5/carefree_drawboard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-23 09:52:57.000000 carefree-drawboard-0.0.0a5/carefree_drawboard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.301926 carefree-drawboard-0.0.0a5/cfdraw/
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.304926 carefree-drawboard-0.0.0a5/cfdraw/.web/
+-rw-rw-rw-   0        0        0      121 2023-04-18 05:54:36.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/.env
+-rw-rw-rw-   0        0        0      143 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/.prettierrc
+-rw-rw-rw-   0        0        0      323 2023-04-13 08:34:20.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/index.html
+-rw-rw-rw-   0        0        0     1628 2023-04-18 02:10:06.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/package.json
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.308926 carefree-drawboard-0.0.0a5/cfdraw/.web/src/
+-rw-rw-rw-   0        0        0      963 2023-04-22 16:41:47.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/App.tsx
+-rw-rw-rw-   0        0        0     1453 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/BoardPanel.tsx
+-rw-rw-rw-   0        0        0     5781 2023-04-23 04:23:21.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/_settings.ts
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.313926 carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/
+-rw-rw-rw-   0        0        0     2263 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/addImage.ts
+-rw-rw-rw-   0        0        0      960 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/addText.ts
+-rw-rw-rw-   0        0        0     9573 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/arrange.ts
+-rw-rw-rw-   0        0        0     1930 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/download.ts
+-rw-rw-rw-   0        0        0     2249 2023-04-19 04:21:39.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/export.ts
+-rw-rw-rw-   0        0        0     5952 2023-04-23 08:04:37.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/importMeta.ts
+-rw-rw-rw-   0        0        0     1286 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/managePlugins.ts
+-rw-rw-rw-   0        0        0     3528 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/manageProjects.ts
+-rw-rw-rw-   0        0        0      272 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/update.ts
+-rw-rw-rw-   0        0        0     1175 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/uploadImage.ts
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.273936 carefree-drawboard-0.0.0a5/cfdraw/.web/src/assets/
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.313926 carefree-drawboard-0.0.0a5/cfdraw/.web/src/assets/icons/
+-rw-rw-rw-   0        0        0      257 2022-10-23 15:19:01.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/assets/icons/arrow-down.svg
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.319926 carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/
+-rw-rw-rw-   0        0        0      723 2023-04-22 13:46:05.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFButton.tsx
+-rw-rw-rw-   0        0        0      359 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFDivider.tsx
+-rw-rw-rw-   0        0        0      243 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFHeading.tsx
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.321926 carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFIcon/
+-rw-rw-rw-   0        0        0      546 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFIcon/index.scss
+-rw-rw-rw-   0        0        0     1568 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFIcon/index.tsx
+-rw-rw-rw-   0        0        0     1568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFImageUploader.tsx
+-rw-rw-rw-   0        0        0      346 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFInput.tsx
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.322926 carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFSelect/
+-rw-rw-rw-   0        0        0       70 2023-04-07 06:01:04.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFSelect/index.scss
+-rw-rw-rw-   0        0        0     3483 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFSelect/index.tsx
+-rw-rw-rw-   0        0        0     4606 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFSlider.tsx
+-rw-rw-rw-   0        0        0     1644 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFSwitch.tsx
+-rw-rw-rw-   0        0        0      324 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFText.tsx
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.327927 carefree-drawboard-0.0.0a5/cfdraw/.web/src/hooks/
+-rw-rw-rw-   0        0        0     3110 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/hooks/useFileDropper.ts
+-rw-rw-rw-   0        0        0     4289 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/hooks/useGridLines.ts
+-rw-rw-rw-   0        0        0     2940 2023-04-17 06:33:19.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/hooks/useInitBoard.ts
+-rw-rw-rw-   0        0        0      445 2023-04-11 05:03:17.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/hooks/usePreventDefaults.ts
+-rw-rw-rw-   0        0        0     5241 2023-04-23 08:46:49.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/hooks/usePython.ts
+-rw-rw-rw-   0        0        0      394 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/hooks/useUndoRedo.ts
+-rw-rw-rw-   0        0        0      131 2023-04-07 08:12:13.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/index.scss
+-rw-rw-rw-   0        0        0      345 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/index.tsx
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.332926 carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/
+-rw-rw-rw-   0        0        0      792 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/add.ts
+-rw-rw-rw-   0        0        0      849 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/brush.ts
+-rw-rw-rw-   0        0        0     1148 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/download.ts
+-rw-rw-rw-   0        0        0     1436 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/index.ts
+-rw-rw-rw-   0        0        0      404 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/nodeEditor.ts
+-rw-rw-rw-   0        0        0     2302 2023-04-23 08:04:44.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/plugins.ts
+-rw-rw-rw-   0        0        0     1746 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/projects.ts
+-rw-rw-rw-   0        0        0      896 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/settings.ts
+-rw-rw-rw-   0        0        0     7075 2023-04-21 10:12:04.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/toast.ts
+-rw-rw-rw-   0        0        0     1472 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/ui.ts
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.341925 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/
+-rw-rw-rw-   0        0        0     2806 2023-04-23 04:26:50.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/AddPlugin.tsx
+-rw-rw-rw-   0        0        0      876 2023-04-23 04:26:57.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/ArrangePlugin.tsx
+-rw-rw-rw-   0        0        0     4807 2023-04-23 04:27:02.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/BrushPlugin.tsx
+-rw-rw-rw-   0        0        0      852 2023-04-23 04:27:13.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/DeletePlugin.tsx
+-rw-rw-rw-   0        0        0     3471 2023-04-23 04:27:24.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/DownloadPlugin.tsx
+-rw-rw-rw-   0        0        0     1081 2023-04-23 04:27:32.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/GroupPlugin.tsx
+-rw-rw-rw-   0        0        0     1121 2023-04-23 04:21:09.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/LinksPlugin.tsx
+-rw-rw-rw-   0        0        0     1211 2023-04-23 07:58:28.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/MetaPlugin.tsx
+-rw-rw-rw-   0        0        0     6478 2023-04-23 04:27:51.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/ProjectPlugin.tsx
+-rw-rw-rw-   0        0        0     5066 2023-04-23 04:28:03.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/SettingsPlugin.tsx
+-rw-rw-rw-   0        0        0     2372 2023-04-23 04:28:10.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/TextEditorPlugin.tsx
+-rw-rw-rw-   0        0        0      920 2023-04-23 04:28:16.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.344926 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/_python/
+-rw-rw-rw-   0        0        0      685 2023-04-21 06:07:38.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/_python/DefinitionFields.tsx
+-rw-rw-rw-   0        0        0     3578 2023-04-23 08:46:18.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
+-rw-rw-rw-   0        0        0     2820 2023-04-23 08:17:14.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
+-rw-rw-rw-   0        0        0     2076 2023-04-23 08:47:06.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/_python/QAPlugin.tsx
+-rw-rw-rw-   0        0        0     1840 2023-04-23 08:47:14.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
+-rw-rw-rw-   0        0        0     1353 2023-04-21 09:49:07.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/_python/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.347926 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.351564 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/Fields/
+-rw-rw-rw-   0        0        0     1411 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
+-rw-rw-rw-   0        0        0      693 2023-04-13 06:08:57.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
+-rw-rw-rw-   0        0        0      854 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
+-rw-rw-rw-   0        0        0     1133 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/Fields/index.tsx
+-rw-rw-rw-   0        0        0      614 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/Fields/utils.ts
+-rw-rw-rw-   0        0        0     7481 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/Floating.tsx
+-rw-rw-rw-   0        0        0      307 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/Link.tsx
+-rw-rw-rw-   0        0        0     7048 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/Render.tsx
+-rw-rw-rw-   0        0        0      225 2023-04-21 05:52:53.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/hooks.ts
+-rw-rw-rw-   0        0        0     2337 2023-04-23 08:05:02.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/index.tsx
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.352564 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/utils/
+-rw-rw-rw-   0        0        0     1575 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/utils/factory.ts
+-rw-rw-rw-   0        0        0      583 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/utils/renderFilters.ts
+-rw-rw-rw-   0        0        0      841 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/react-app-env.d.ts
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.352564 carefree-drawboard-0.0.0a5/cfdraw/.web/src/requests/
+-rw-rw-rw-   0        0        0     1028 2023-04-19 04:57:46.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/requests/actions.ts
+-rw-rw-rw-   0        0        0     2545 2023-04-23 09:26:16.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/requests/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.353563 carefree-drawboard-0.0.0a5/cfdraw/.web/src/requests/interceptors/
+-rw-rw-rw-   0        0        0      880 2023-04-17 14:19:55.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/requests/interceptors/_python.ts
+-rw-rw-rw-   0        0        0      752 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/requests/interceptors/index.ts
+-rw-rw-rw-   0        0        0       38 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/reset.d.ts
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.356563 carefree-drawboard-0.0.0a5/cfdraw/.web/src/schema/
+-rw-rw-rw-   0        0        0     3871 2023-04-23 08:46:09.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/schema/_python.ts
+-rw-rw-rw-   0        0        0     1772 2023-04-23 08:05:20.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/schema/meta.ts
+-rw-rw-rw-   0        0        0     1169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/schema/metaFields.ts
+-rw-rw-rw-   0        0        0      289 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/schema/misc.ts
+-rw-rw-rw-   0        0        0     3125 2023-04-23 08:05:25.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/schema/plugins.ts
+-rw-rw-rw-   0        0        0      850 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/schema/requests.ts
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.361564 carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/
+-rw-rw-rw-   0        0        0     1431 2023-04-17 09:56:35.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/_python.ts
+-rw-rw-rw-   0        0        0      586 2023-04-23 09:28:17.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/debug.ts
+-rw-rw-rw-   0        0        0     1495 2023-04-21 10:35:17.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/gridLines.ts
+-rw-rw-rw-   0        0        0      578 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/hooks.ts
+-rw-rw-rw-   0        0        0      468 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/init.ts
+-rw-rw-rw-   0        0        0     1107 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/meta.ts
+-rw-rw-rw-   0        0        0     1561 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/plugins.ts
+-rw-rw-rw-   0        0        0     1704 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/projects.ts
+-rw-rw-rw-   0        0        0     5727 2023-04-23 08:46:40.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/socket.ts
+-rw-rw-rw-   0        0        0     3285 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/theme.ts
+-rw-rw-rw-   0        0        0     2025 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/ui.ts
+-rw-rw-rw-   0        0        0      703 2023-04-23 07:27:21.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/user.ts
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.363564 carefree-drawboard-0.0.0a5/cfdraw/.web/src/utils/
+-rw-rw-rw-   0        0        0      467 2023-04-07 05:25:36.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/utils/bem.ts
+-rw-rw-rw-   0        0        0      466 2023-04-17 06:32:01.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/utils/constants.ts
+-rw-rw-rw-   0        0        0      934 2023-04-06 06:11:04.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/utils/event.ts
+-rw-rw-rw-   0        0        0     1025 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/utils/misc.ts
+-rw-rw-rw-   0        0        0      633 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/utils/toast.ts
+-rw-rw-rw-   0        0        0       39 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/src/vite-env.d.ts
+-rw-rw-rw-   0        0        0      656 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/tsconfig.json
+-rw-rw-rw-   0        0        0      193 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/tsconfig.node.json
+-rw-rw-rw-   0        0        0      103 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/tsconfig.paths.json
+-rw-rw-rw-   0        0        0     1849 2023-04-18 03:53:52.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/vite.config.ts
+-rw-rw-rw-   0        0        0   214083 2023-04-18 03:11:54.000000 carefree-drawboard-0.0.0a5/cfdraw/.web/yarn.lock
+-rw-rw-rw-   0        0        0      405 2023-04-13 06:43:12.000000 carefree-drawboard-0.0.0a5/cfdraw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.364564 carefree-drawboard-0.0.0a5/cfdraw/app/
+-rw-rw-rw-   0        0        0       20 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a5/cfdraw/app/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-23 08:15:58.000000 carefree-drawboard-0.0.0a5/cfdraw/app/app.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.367564 carefree-drawboard-0.0.0a5/cfdraw/app/endpoints/
+-rw-rw-rw-   0        0        0      139 2023-04-23 08:15:42.000000 carefree-drawboard-0.0.0a5/cfdraw/app/endpoints/__init__.py
+-rw-rw-rw-   0        0        0      745 2023-04-21 12:01:39.000000 carefree-drawboard-0.0.0a5/cfdraw/app/endpoints/assets.py
+-rw-rw-rw-   0        0        0      493 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a5/cfdraw/app/endpoints/base.py
+-rw-rw-rw-   0        0        0     5713 2023-04-19 04:49:15.000000 carefree-drawboard-0.0.0a5/cfdraw/app/endpoints/project.py
+-rw-rw-rw-   0        0        0     6797 2023-04-23 08:57:07.000000 carefree-drawboard-0.0.0a5/cfdraw/app/endpoints/queue.py
+-rw-rw-rw-   0        0        0     2158 2023-04-19 04:21:46.000000 carefree-drawboard-0.0.0a5/cfdraw/app/endpoints/upload.py
+-rw-rw-rw-   0        0        0     3112 2023-04-23 08:59:01.000000 carefree-drawboard-0.0.0a5/cfdraw/app/endpoints/websocket.py
+-rw-rw-rw-   0        0        0     1389 2023-04-23 08:48:13.000000 carefree-drawboard-0.0.0a5/cfdraw/app/schema.py
+-rw-rw-rw-   0        0        0     3333 2023-04-22 02:31:01.000000 carefree-drawboard-0.0.0a5/cfdraw/cli.py
+-rw-rw-rw-   0        0        0     2245 2023-04-21 12:04:53.000000 carefree-drawboard-0.0.0a5/cfdraw/config.py
+-rw-rw-rw-   0        0        0     1456 2023-04-21 11:42:04.000000 carefree-drawboard-0.0.0a5/cfdraw/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.368564 carefree-drawboard-0.0.0a5/cfdraw/parsers/
+-rw-rw-rw-   0        0        0       44 2023-04-09 01:57:56.000000 carefree-drawboard-0.0.0a5/cfdraw/parsers/__init__.py
+-rw-rw-rw-   0        0        0      609 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a5/cfdraw/parsers/chakra.py
+-rw-rw-rw-   0        0        0     6692 2023-04-19 02:34:15.000000 carefree-drawboard-0.0.0a5/cfdraw/parsers/noli.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.370563 carefree-drawboard-0.0.0a5/cfdraw/plugins/
+-rw-rw-rw-   0        0        0       92 2023-04-23 04:40:40.000000 carefree-drawboard-0.0.0a5/cfdraw/plugins/__init__.py
+-rw-rw-rw-   0        0        0     4756 2023-04-23 09:35:11.000000 carefree-drawboard-0.0.0a5/cfdraw/plugins/base.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.370563 carefree-drawboard-0.0.0a5/cfdraw/plugins/community/
+-rw-rw-rw-   0        0        0        0 2023-04-14 05:16:37.000000 carefree-drawboard-0.0.0a5/cfdraw/plugins/community/__init__.py
+-rw-rw-rw-   0        0        0     2472 2023-04-22 12:17:12.000000 carefree-drawboard-0.0.0a5/cfdraw/plugins/factory.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.372563 carefree-drawboard-0.0.0a5/cfdraw/plugins/middlewares/
+-rw-rw-rw-   0        0        0      100 2023-04-23 09:08:34.000000 carefree-drawboard-0.0.0a5/cfdraw/plugins/middlewares/__init__.py
+-rw-rw-rw-   0        0        0      908 2023-04-23 09:30:55.000000 carefree-drawboard-0.0.0a5/cfdraw/plugins/middlewares/fields.py
+-rw-rw-rw-   0        0        0      725 2023-04-23 09:31:04.000000 carefree-drawboard-0.0.0a5/cfdraw/plugins/middlewares/send_message.py
+-rw-rw-rw-   0        0        0      500 2023-04-23 09:31:13.000000 carefree-drawboard-0.0.0a5/cfdraw/plugins/middlewares/text_area.py
+-rw-rw-rw-   0        0        0      962 2023-04-23 09:31:28.000000 carefree-drawboard-0.0.0a5/cfdraw/plugins/middlewares/timer.py
+-rw-rw-rw-   0        0        0      920 2023-04-23 09:20:38.000000 carefree-drawboard-0.0.0a5/cfdraw/plugins/sync.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.373563 carefree-drawboard-0.0.0a5/cfdraw/schema/
+-rw-rw-rw-   0        0        0       47 2023-04-13 15:19:11.000000 carefree-drawboard-0.0.0a5/cfdraw/schema/__init__.py
+-rw-rw-rw-   0        0        0     3157 2023-04-13 06:12:19.000000 carefree-drawboard-0.0.0a5/cfdraw/schema/fields.py
+-rw-rw-rw-   0        0        0    12365 2023-04-23 09:33:56.000000 carefree-drawboard-0.0.0a5/cfdraw/schema/plugins.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.377564 carefree-drawboard-0.0.0a5/cfdraw/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-08 03:23:05.000000 carefree-drawboard-0.0.0a5/cfdraw/utils/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a5/cfdraw/utils/cache.py
+-rw-rw-rw-   0        0        0      875 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a5/cfdraw/utils/console.py
+-rw-rw-rw-   0        0        0     6414 2023-04-23 02:50:50.000000 carefree-drawboard-0.0.0a5/cfdraw/utils/data_structures.py
+-rw-rw-rw-   0        0        0     2622 2023-04-22 02:30:59.000000 carefree-drawboard-0.0.0a5/cfdraw/utils/exec.py
+-rw-rw-rw-   0        0        0      713 2023-04-23 07:36:56.000000 carefree-drawboard-0.0.0a5/cfdraw/utils/misc.py
+-rw-rw-rw-   0        0        0      638 2023-04-17 03:07:08.000000 carefree-drawboard-0.0.0a5/cfdraw/utils/prerequisites.py
+-rw-rw-rw-   0        0        0     1766 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a5/cfdraw/utils/processes.py
+-rw-rw-rw-   0        0        0     3667 2023-04-17 13:24:23.000000 carefree-drawboard-0.0.0a5/cfdraw/utils/server.py
+-rw-rw-rw-   0        0        0     2691 2023-04-23 08:40:14.000000 carefree-drawboard-0.0.0a5/cfdraw/utils/template.py
+-rw-rw-rw-   0        0        0      113 2023-04-23 09:52:59.381565 carefree-drawboard-0.0.0a5/setup.cfg
+-rw-rw-rw-   0        0        0     1063 2023-04-23 09:52:39.000000 carefree-drawboard-0.0.0a5/setup.py
```

### Comparing `carefree-drawboard-0.0.0a4/LICENSE` & `carefree-drawboard-0.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/PKG-INFO` & `carefree-drawboard-0.0.0a5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-drawboard
-Version: 0.0.0a4
+Version: 0.0.0a5
 Summary: 🎨 Infinite Drawboard in Python
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn drawboard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -12,20 +12,20 @@
 
 ![Stable Diffusion](examples/assets/stable-diffusion.png)
 
 > This is the screenshot I used for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example and I don't know what should be the proper banner, help!
 
 <div align="center">
 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 [![PyPI version](https://badge.fury.io/py/carefree-drawboard.svg)](https://badge.fury.io/py/carefree-drawboard.svg)
 ![Checks](https://github.com/carefree0910/carefree-drawboard/actions/workflows/checks.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 
-### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting)
+### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet)
 
 <div align="left">
 
 ## Installation
 
 `carefree-drawboard` 🎨 requires the following to get started:
 
@@ -57,34 +57,34 @@
 
 Create a folder (e.g., `my_fancy_app`) wherever you like, get into it, and run
 
 ```bash
 cfdraw init
 ```
 
-> When you run this command for the first time, we will use `yarn` to install the JavaScript dependencies for you, which may be quite slow!
-
 This command will write two files to your folder (`my_fancy_app`). After which you can run the app in development mode:
 
 ```bash
 cfdraw run
 ```
 
+> When you run this command for the first time and have not called `cfdraw install` before, we will use `yarn` to install the JavaScript dependencies for you, which may be quite slow!
+
 And you should see your app running at http://localhost:5123. Now you can play with the generated `app.py` file and see warm reload (yeah, not hot enough because we rely on the `reload` provided by `uvicorn` 🤣).
 
-> Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dropping on directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
+> Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dragging it directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
 
 [Demo Video](https://user-images.githubusercontent.com/15677328/232184463-627c2cd7-728a-49ce-93c6-7c878edc27b9.mp4)
 
 ## Examples
 
-* [Getting Started](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
+* [**Getting Started**](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
 * [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins with `carefree-drawboard` 🎨.
 * [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common Stable Diffusion plugins with `carefree-drawboard` 🎨.
-* [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
+* [**Caption & Diffusion**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
 * [Stable Diffusion Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting), which shows how can we implement complicated plugins like `StableDiffusionInpainting` very easily with `carefree-drawboard` 🎨.
 * [Stable Diffusion ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet), which shows how can we decouple complicated workflows like `ControlNet` into separate, lightweight, and reusable plugins very easily with `carefree-drawboard` 🎨.
 
 ## Documentation
 
 Check the [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) page for documentation!
 
@@ -98,18 +98,16 @@
 
 Contributions are truly welcomed! Here are some good (common) ways to get started:
 
 * **GitHub Discussions**: Currently the best way to chat around.
 * **GitHub Issues**: Bugs! Fixes! PRs!.
 
 Apart from these:
+* It might be the best to start from the [Contributing](https://github.com/carefree0910/carefree-drawboard/wiki/Contributing) Wiki page.
 * If you are truly an enthusiast, you may check out our [Roadmap](https://github.com/carefree0910/carefree-drawboard/wiki/Roadmap), pick up what you are interested, and create the corresponding PR!
-* If you are familiar with `React`, you may check out the [Customizations](https://github.com/carefree0910/carefree-drawboard/wiki/Customizations) documentation and try to customize your own plugins and have fun!
-
-> It is also recommended to start from the [Development Guide](https://github.com/carefree0910/carefree-drawboard/wiki/Development-Guide)!
 
 ### Style Guide
 
 If you are still interested: `carefree-drawboard` 🎨 adopted [`black`](https://github.com/psf/black) and [`mypy`](https://github.com/python/mypy) to stylize its codes, so you may need to check the format, coding style and type hint with them before your codes could actually be merged.
 
 ## Q&A
```

### Comparing `carefree-drawboard-0.0.0a4/README.md` & `carefree-drawboard-0.0.0a5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 ![Stable Diffusion](examples/assets/stable-diffusion.png)
 
 > This is the screenshot I used for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example and I don't know what should be the proper banner, help!
 
 <div align="center">
 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 [![PyPI version](https://badge.fury.io/py/carefree-drawboard.svg)](https://badge.fury.io/py/carefree-drawboard.svg)
 ![Checks](https://github.com/carefree0910/carefree-drawboard/actions/workflows/checks.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 
-### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting)
+### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet)
 
 <div align="left">
 
 ## Installation
 
 `carefree-drawboard` 🎨 requires the following to get started:
 
@@ -47,34 +47,34 @@
 
 Create a folder (e.g., `my_fancy_app`) wherever you like, get into it, and run
 
 ```bash
 cfdraw init
 ```
 
-> When you run this command for the first time, we will use `yarn` to install the JavaScript dependencies for you, which may be quite slow!
-
 This command will write two files to your folder (`my_fancy_app`). After which you can run the app in development mode:
 
 ```bash
 cfdraw run
 ```
 
+> When you run this command for the first time and have not called `cfdraw install` before, we will use `yarn` to install the JavaScript dependencies for you, which may be quite slow!
+
 And you should see your app running at http://localhost:5123. Now you can play with the generated `app.py` file and see warm reload (yeah, not hot enough because we rely on the `reload` provided by `uvicorn` 🤣).
 
-> Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dropping on directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
+> Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dragging it directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
 
 [Demo Video](https://user-images.githubusercontent.com/15677328/232184463-627c2cd7-728a-49ce-93c6-7c878edc27b9.mp4)
 
 ## Examples
 
-* [Getting Started](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
+* [**Getting Started**](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
 * [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins with `carefree-drawboard` 🎨.
 * [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common Stable Diffusion plugins with `carefree-drawboard` 🎨.
-* [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
+* [**Caption & Diffusion**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
 * [Stable Diffusion Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting), which shows how can we implement complicated plugins like `StableDiffusionInpainting` very easily with `carefree-drawboard` 🎨.
 * [Stable Diffusion ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet), which shows how can we decouple complicated workflows like `ControlNet` into separate, lightweight, and reusable plugins very easily with `carefree-drawboard` 🎨.
 
 ## Documentation
 
 Check the [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) page for documentation!
 
@@ -88,18 +88,16 @@
 
 Contributions are truly welcomed! Here are some good (common) ways to get started:
 
 * **GitHub Discussions**: Currently the best way to chat around.
 * **GitHub Issues**: Bugs! Fixes! PRs!.
 
 Apart from these:
+* It might be the best to start from the [Contributing](https://github.com/carefree0910/carefree-drawboard/wiki/Contributing) Wiki page.
 * If you are truly an enthusiast, you may check out our [Roadmap](https://github.com/carefree0910/carefree-drawboard/wiki/Roadmap), pick up what you are interested, and create the corresponding PR!
-* If you are familiar with `React`, you may check out the [Customizations](https://github.com/carefree0910/carefree-drawboard/wiki/Customizations) documentation and try to customize your own plugins and have fun!
-
-> It is also recommended to start from the [Development Guide](https://github.com/carefree0910/carefree-drawboard/wiki/Development-Guide)!
 
 ### Style Guide
 
 If you are still interested: `carefree-drawboard` 🎨 adopted [`black`](https://github.com/psf/black) and [`mypy`](https://github.com/python/mypy) to stylize its codes, so you may need to check the format, coding style and type hint with them before your codes could actually be merged.
 
 ## Q&A
```

### Comparing `carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/PKG-INFO` & `carefree-drawboard-0.0.0a5/carefree_drawboard.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-drawboard
-Version: 0.0.0a4
+Version: 0.0.0a5
 Summary: 🎨 Infinite Drawboard in Python
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn drawboard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -12,20 +12,20 @@
 
 ![Stable Diffusion](examples/assets/stable-diffusion.png)
 
 > This is the screenshot I used for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example and I don't know what should be the proper banner, help!
 
 <div align="center">
 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 [![PyPI version](https://badge.fury.io/py/carefree-drawboard.svg)](https://badge.fury.io/py/carefree-drawboard.svg)
 ![Checks](https://github.com/carefree0910/carefree-drawboard/actions/workflows/checks.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 
-### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting)
+### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet)
 
 <div align="left">
 
 ## Installation
 
 `carefree-drawboard` 🎨 requires the following to get started:
 
@@ -57,34 +57,34 @@
 
 Create a folder (e.g., `my_fancy_app`) wherever you like, get into it, and run
 
 ```bash
 cfdraw init
 ```
 
-> When you run this command for the first time, we will use `yarn` to install the JavaScript dependencies for you, which may be quite slow!
-
 This command will write two files to your folder (`my_fancy_app`). After which you can run the app in development mode:
 
 ```bash
 cfdraw run
 ```
 
+> When you run this command for the first time and have not called `cfdraw install` before, we will use `yarn` to install the JavaScript dependencies for you, which may be quite slow!
+
 And you should see your app running at http://localhost:5123. Now you can play with the generated `app.py` file and see warm reload (yeah, not hot enough because we rely on the `reload` provided by `uvicorn` 🤣).
 
-> Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dropping on directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
+> Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dragging it directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
 
 [Demo Video](https://user-images.githubusercontent.com/15677328/232184463-627c2cd7-728a-49ce-93c6-7c878edc27b9.mp4)
 
 ## Examples
 
-* [Getting Started](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
+* [**Getting Started**](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
 * [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins with `carefree-drawboard` 🎨.
 * [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common Stable Diffusion plugins with `carefree-drawboard` 🎨.
-* [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
+* [**Caption & Diffusion**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
 * [Stable Diffusion Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting), which shows how can we implement complicated plugins like `StableDiffusionInpainting` very easily with `carefree-drawboard` 🎨.
 * [Stable Diffusion ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet), which shows how can we decouple complicated workflows like `ControlNet` into separate, lightweight, and reusable plugins very easily with `carefree-drawboard` 🎨.
 
 ## Documentation
 
 Check the [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) page for documentation!
 
@@ -98,18 +98,16 @@
 
 Contributions are truly welcomed! Here are some good (common) ways to get started:
 
 * **GitHub Discussions**: Currently the best way to chat around.
 * **GitHub Issues**: Bugs! Fixes! PRs!.
 
 Apart from these:
+* It might be the best to start from the [Contributing](https://github.com/carefree0910/carefree-drawboard/wiki/Contributing) Wiki page.
 * If you are truly an enthusiast, you may check out our [Roadmap](https://github.com/carefree0910/carefree-drawboard/wiki/Roadmap), pick up what you are interested, and create the corresponding PR!
-* If you are familiar with `React`, you may check out the [Customizations](https://github.com/carefree0910/carefree-drawboard/wiki/Customizations) documentation and try to customize your own plugins and have fun!
-
-> It is also recommended to start from the [Development Guide](https://github.com/carefree0910/carefree-drawboard/wiki/Development-Guide)!
 
 ### Style Guide
 
 If you are still interested: `carefree-drawboard` 🎨 adopted [`black`](https://github.com/psf/black) and [`mypy`](https://github.com/python/mypy) to stylize its codes, so you may need to check the format, coding style and type hint with them before your codes could actually be merged.
 
 ## Q&A
```

### Comparing `carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/SOURCES.txt` & `carefree-drawboard-0.0.0a5/carefree_drawboard.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -72,27 +72,30 @@
 cfdraw/.web/src/plugins/AddPlugin.tsx
 cfdraw/.web/src/plugins/ArrangePlugin.tsx
 cfdraw/.web/src/plugins/BrushPlugin.tsx
 cfdraw/.web/src/plugins/DeletePlugin.tsx
 cfdraw/.web/src/plugins/DownloadPlugin.tsx
 cfdraw/.web/src/plugins/GroupPlugin.tsx
 cfdraw/.web/src/plugins/LinksPlugin.tsx
+cfdraw/.web/src/plugins/MetaPlugin.tsx
 cfdraw/.web/src/plugins/ProjectPlugin.tsx
 cfdraw/.web/src/plugins/SettingsPlugin.tsx
 cfdraw/.web/src/plugins/TextEditorPlugin.tsx
 cfdraw/.web/src/plugins/UndoRedoPlugin.tsx
 cfdraw/.web/src/plugins/index.tsx
-cfdraw/.web/src/plugins/_python/HttpFieldsPlugin.tsx
-cfdraw/.web/src/plugins/_python/HttpPluginWithSubmit.tsx
-cfdraw/.web/src/plugins/_python/HttpQAPlugin.tsx
-cfdraw/.web/src/plugins/_python/HttpTextAreaPlugin.tsx
+cfdraw/.web/src/plugins/_python/DefinitionFields.tsx
+cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
+cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
+cfdraw/.web/src/plugins/_python/QAPlugin.tsx
+cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
 cfdraw/.web/src/plugins/_python/hooks.ts
 cfdraw/.web/src/plugins/components/Floating.tsx
 cfdraw/.web/src/plugins/components/Link.tsx
 cfdraw/.web/src/plugins/components/Render.tsx
+cfdraw/.web/src/plugins/components/hooks.ts
 cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
 cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
 cfdraw/.web/src/plugins/components/Fields/TextField.tsx
 cfdraw/.web/src/plugins/components/Fields/index.tsx
 cfdraw/.web/src/plugins/components/Fields/utils.ts
 cfdraw/.web/src/plugins/utils/factory.ts
 cfdraw/.web/src/plugins/utils/renderFilters.ts
@@ -103,57 +106,59 @@
 cfdraw/.web/src/schema/_python.ts
 cfdraw/.web/src/schema/meta.ts
 cfdraw/.web/src/schema/metaFields.ts
 cfdraw/.web/src/schema/misc.ts
 cfdraw/.web/src/schema/plugins.ts
 cfdraw/.web/src/schema/requests.ts
 cfdraw/.web/src/stores/_python.ts
+cfdraw/.web/src/stores/debug.ts
 cfdraw/.web/src/stores/gridLines.ts
 cfdraw/.web/src/stores/hooks.ts
 cfdraw/.web/src/stores/init.ts
 cfdraw/.web/src/stores/meta.ts
 cfdraw/.web/src/stores/plugins.ts
 cfdraw/.web/src/stores/projects.ts
+cfdraw/.web/src/stores/socket.ts
 cfdraw/.web/src/stores/theme.ts
 cfdraw/.web/src/stores/ui.ts
+cfdraw/.web/src/stores/user.ts
 cfdraw/.web/src/utils/bem.ts
 cfdraw/.web/src/utils/constants.ts
 cfdraw/.web/src/utils/event.ts
 cfdraw/.web/src/utils/misc.ts
 cfdraw/.web/src/utils/toast.ts
 cfdraw/app/__init__.py
 cfdraw/app/app.py
 cfdraw/app/schema.py
 cfdraw/app/endpoints/__init__.py
+cfdraw/app/endpoints/assets.py
 cfdraw/app/endpoints/base.py
-cfdraw/app/endpoints/plugins.py
 cfdraw/app/endpoints/project.py
+cfdraw/app/endpoints/queue.py
 cfdraw/app/endpoints/upload.py
 cfdraw/app/endpoints/websocket.py
 cfdraw/parsers/__init__.py
 cfdraw/parsers/chakra.py
 cfdraw/parsers/noli.py
 cfdraw/plugins/__init__.py
 cfdraw/plugins/base.py
 cfdraw/plugins/factory.py
-cfdraw/plugins/meta.py
 cfdraw/plugins/sync.py
 cfdraw/plugins/community/__init__.py
 cfdraw/plugins/middlewares/__init__.py
 cfdraw/plugins/middlewares/fields.py
+cfdraw/plugins/middlewares/send_message.py
 cfdraw/plugins/middlewares/text_area.py
 cfdraw/plugins/middlewares/timer.py
 cfdraw/schema/__init__.py
 cfdraw/schema/fields.py
 cfdraw/schema/plugins.py
-cfdraw/server/__init__.py
-cfdraw/server/http.py
-cfdraw/server/index.py
-cfdraw/server/socket.py
 cfdraw/utils/__init__.py
 cfdraw/utils/cache.py
 cfdraw/utils/console.py
+cfdraw/utils/data_structures.py
 cfdraw/utils/exec.py
+cfdraw/utils/misc.py
 cfdraw/utils/prerequisites.py
 cfdraw/utils/processes.py
 cfdraw/utils/server.py
 cfdraw/utils/template.py
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/package.json` & `carefree-drawboard-0.0.0a5/cfdraw/.web/package.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/App.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/App.tsx`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import { Flex } from "@chakra-ui/react";
 import { observer } from "mobx-react-lite";
 
 import { langStore } from "@carefree0910/business";
 
+import { useWebSocket } from "./stores/socket";
 import { useInitBoard } from "./hooks/useInitBoard";
 import { useFileDropper } from "./hooks/useFileDropper";
 import { useGridLines } from "./hooks/useGridLines";
 import { usePreventDefaults } from "./hooks/usePreventDefaults";
 import { useUndoRedo } from "./hooks/useUndoRedo";
 import { useSyncPython } from "./hooks/usePython";
 import BoardPanel from "./BoardPanel";
 
 function App() {
+  useWebSocket();
   useSyncPython();
   useInitBoard();
   useFileDropper(langStore.tgt);
   useGridLines();
   useUndoRedo();
   usePreventDefaults();
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/BoardPanel.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/BoardPanel.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/_settings.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/_settings.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 import type { AvailablePlugins, IMakePlugin } from "@/schema/plugins";
 
 export const reactPluginSettings: IMakePlugin<AvailablePlugins>[] = [
   {
+    type: "meta",
+    props: {
+      offsetY: 48,
+      nodeConstraint: "singleNode",
+      renderInfo: {
+        w: 400,
+        h: 400,
+        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/0ec1b08f9c3e4ef4813ecb80bebf3b42.png",
+        pivot: "rt",
+        follow: true,
+      },
+      pluginInfo: {},
+    },
+  },
+  {
     type: "settings",
     props: {
       nodeConstraint: "none",
       renderInfo: {
         w: 300,
         h: 400,
         src: "https://ailab-huawei-cdn.nolibox.com/upload/images/49223052f17f4f249c56ba00f43b3043.png",
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/addImage.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/addImage.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/addText.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/addText.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/arrange.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/arrange.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/download.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/export.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/export.ts`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import { INode, ISingleNode, Lang, toJsonBlob } from "@carefree0910/core";
 import { ExportBlobOptions, exportBlob, exportNodes } from "@carefree0910/svg";
 import { translate } from "@carefree0910/business";
 
 import type { DownloadFormat, IToast, ImageFormat } from "@/schema/misc";
 import { toast } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
+import { Requests } from "@/requests/actions";
 import { uploadImage } from "./uploadImage";
 
 const isImage = (format: DownloadFormat) => format === "JPG" || format === "PNG";
-const toJpegUrl = (url: string) => `${url}?jpeg=True`;
+
+function fetchImage(data: { url: string; jpeg: boolean }): Promise<Blob> {
+  return Requests.postJson<Blob>("_python", "/fetch_image", data, "blob");
+}
 
 export type IExportBlob = ExportBlobOptions & { t: IToast; lang: Lang };
 export class Exporter {
   static async exportBlob(
     nodes: ISingleNode[],
     { t, lang, ...others }: IExportBlob,
   ): Promise<Blob | void> {
@@ -26,33 +30,30 @@
   static async exportOne(
     t: IToast,
     lang: Lang,
     node: INode,
     format: ImageFormat,
     exportOriginalSize: boolean,
   ): Promise<Blob | void> {
+    const jpeg = format === "JPG";
     if (isImage(format) && node.type === "image" && exportOriginalSize) {
-      let url = node.renderParams.src;
-      if (format === "JPG") {
-        url = toJpegUrl(url);
-      }
-      return fetch(url).then((res) => res.blob());
+      return fetchImage({ url: node.renderParams.src, jpeg });
     }
     const bounding = node.bbox.bounding.toAABB();
     const targetNodes = node.type === "group" ? node.allChildrenNodes : [node];
     if (isImage(format)) {
       const blob = await Exporter.exportBlob(targetNodes, {
         t,
         lang,
         exportOptions: { exportBox: bounding },
       });
       if (!blob || format !== "JPG") return blob;
       const res = await uploadImage(t, lang, blob, { failed: async () => void 0 });
       if (!res) return;
-      return fetch(toJpegUrl(res.url)).then((res) => res.blob());
+      return fetchImage({ url: res.url, jpeg: true });
     }
     const res = await exportNodes(targetNodes, { exportBox: bounding });
     if (!res) {
       toast(t, "error", translate(Toast_Words["export-blob-error-message"], lang));
       return;
     }
     return toJsonBlob(res.svg.svg());
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/importMeta.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/importMeta.ts`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import { Dictionary, RectangleShapeNode, getRandomHash, shallowCopy } from "@carefree0910/core";
 import { BoardStore, translate, useAddNode } from "@carefree0910/business";
 
-import type { IMetaData, MetaType } from "@/schema/meta";
+import type { IMetaData, IPythonFieldsMetaData, MetaType } from "@/schema/meta";
 import type { IImportMeta } from "@/schema/meta";
 import { toast } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
 import { themeStore } from "@/stores/theme";
 import { updateMeta } from "./update";
 import { addNewText } from "./addText";
 import { addNewImage, getNewRectangle, INewRectangle, NewImageInfo } from "./addImage";
@@ -24,27 +24,28 @@
   updateMeta(alias, node.params.meta);
 }
 
 const consumers: Record<MetaType, (input: IImportMeta<any>) => void> = {
   upload: consumeUpload,
   "add.text": consumeAddText,
   "add.sketch.path": consumeAddSketchPath,
-  "python.httpFields": consumePythonHttpFields,
+  "python.fields": consumePythonFields,
 };
 function consumeUpload({ t, lang, type, metaData }: IImportMeta<"upload">): void {
   const success = async () => {
     toast(t, "success", translate(Toast_Words["upload-image-success-message"], lang));
     updateTimestamps(newAlias);
   };
   const failed = async () => {
     toast(t, "error", translate(Toast_Words["upload-image-error-message"], lang));
   };
   const { w, h, url, isDrag } = metaData;
   const prefix = isDrag ? "drag-" : "";
   const newAlias = `${prefix}upload.${getRandomHash()}`;
+  metaData.alias = newAlias;
   const bboxInfo: NewImageInfo = { w, h };
   addNewImage(newAlias, url, {
     info: bboxInfo,
     meta: { type, data: metaData },
     callbacks: { success, failed },
     noSelect: false,
   });
@@ -57,63 +58,56 @@
     toast(t, "success", translate(Toast_Words["add-text-success-message"], lang));
     updateTimestamps(newAlias);
   };
   const failed = async () => {
     toast(t, "error", translate(Toast_Words["add-text-error-message"], lang));
   };
   const { addText } = useAddNode({ success, failed });
+  metaData.alias = newAlias;
   addText({ trace: true })({
     alias: newAlias,
     initColor: textColor,
     lang,
     autoFit: true,
     meta: { type, data: metaData },
   });
 }
 function consumeAddSketchPath(): void {
   throw Error("Add sketch path by `importMeta` is not supported yet.");
 }
-function consumePythonHttpFields({
-  t,
-  lang,
-  type,
-  metaData,
-}: IImportMeta<"python.httpFields">): void {
+function consumePythonFields({ t, lang, type, metaData }: IImportMeta<"python.fields">): void {
   const success = async () => {
     toast(t, "success", translate(Toast_Words["generate-image-success-message"], lang));
   };
   const failed = async (err: any) => {
     toast(
       t,
       "error",
       `${translate(Toast_Words["post-python-http-fields-plugin-error-message"], lang)} (${err})`,
     );
   };
-  const getNewAlias = () => `python.httpFields.${metaData.identifier}.${getRandomHash()}`;
+  const getNewAlias = () => `${type}.${metaData.identifier}.${getRandomHash()}`;
+  interface IPack<R> {
+    data: R;
+    alias: string;
+    rectangle: RectangleShapeNode;
+    metaData: IPythonFieldsMetaData;
+  }
   function gatherPacks<T, R>(
     responses: T[],
     getRectangleInfo: (res: T) => INewRectangle,
     getData: (res: T) => R,
-  ): {
-    data: R;
-    alias: string;
-    rectangle: RectangleShapeNode;
-    metaData: Dictionary<any>;
-  }[] {
-    const packs: {
-      data: R;
-      alias: string;
-      rectangle: RectangleShapeNode;
-      metaData: Dictionary<any>;
-    }[] = [];
+  ): IPack<R>[] {
+    const packs: IPack<R>[] = [];
     responses.forEach((res, i) => {
       const newAlias = getNewAlias();
       const rectangle = getNewRectangle(`${i}.${getRandomHash()}`, getRectangleInfo(res));
       const iMetaData = shallowCopy(metaData);
       iMetaData.response.value = metaData.response.value[i] as any;
+      iMetaData.alias = newAlias;
       iMetaData.timestamp = Date.now();
       packs.push({ data: getData(res), alias: newAlias, rectangle, metaData: iMetaData });
     });
     return packs;
   }
   function getCallbacks(isLast: boolean) {
     return { success: isLast ? success : async () => void 0, failed };
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/managePlugins.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/managePlugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/manageProjects.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/manageProjects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/uploadImage.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/actions/uploadImage.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFIcon/index.scss` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFIcon/index.scss`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFIcon/index.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFIcon/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFImageUploader.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFImageUploader.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSelect/index.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFSelect/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSlider.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFSlider.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSwitch.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/components/CFSwitch.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useFileDropper.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/hooks/useFileDropper.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useGridLines.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/hooks/useGridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useInitBoard.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/hooks/useInitBoard.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/usePython.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/hooks/usePython.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import { useCallback, useEffect } from "react";
+import { useCallback } from "react";
 
 import { BBox, INode, INodes, Logger } from "@carefree0910/core";
 
 import type { IMeta } from "@/schema/meta";
 import type {
   INodeData,
-  IPythonResponse,
-  IPythonRequest,
-  IUseHttpPython,
+  IPythonSocketRequest,
   IUsePythonInfo,
+  IUseSocketPython,
+  IPythonOnSocketMessage,
 } from "@/schema/_python";
+import { userStore } from "@/stores/user";
+import { debugStore } from "@/stores/debug";
 import { IPythonStore, updatePythonStore } from "@/stores/_python";
-import { Requests } from "@/requests/actions";
-import { useWebSocket } from "@/requests/hooks";
+import { useWebSocketHook } from "@/requests/hooks";
 import { uploadImage } from "@/actions/uploadImage";
 import { Exporter, IExportBlob } from "@/actions/export";
 
 type IGetNodeData = IExportBlob & { exportBox: BBox };
 async function getNodeData(node: INode | null, opt: IGetNodeData): Promise<INodeData> {
   if (!node) return {};
   const { x, y } = node.position;
@@ -50,112 +51,122 @@
 async function getPythonRequest({
   node,
   nodes,
   identifier,
   getExtraRequestData,
   opt,
 }: Omit<IUsePythonInfo, "endpoint" | "isInvisible"> & {
-  opt: IGetNodeData;
-}): Promise<IPythonRequest> {
-  const nodeData = await getNodeData(node, opt);
-  const nodeDataList = nodes.length <= 1 ? [] : await getNodeDataList(nodes, opt);
+  opt: IExportBlob;
+}): Promise<Omit<IPythonSocketRequest, "hash">> {
+  const exportBox = new INodes(nodes).bbox;
+  const getNodeDataOpt: IGetNodeData = { exportBox, ...opt };
+  const nodeData = await getNodeData(node, getNodeDataOpt);
+  const nodeDataList = nodes.length <= 1 ? [] : await getNodeDataList(nodes, getNodeDataOpt);
   return {
+    userId: userStore.userId,
     identifier,
     nodeData,
     nodeDataList,
     extraData: getExtraRequestData ? getExtraRequestData() : {},
   };
 }
 
-export function useHttpPython<R>({
+/**
+ * this function will integrate a simple but useful retry mechanism, so we only need to
+ * focus on the core logics in `onMessage` function.
+ */
+export function useSocketPython<R>({
   t,
   lang,
+  hash,
   node,
   nodes,
   endpoint,
   identifier,
   isInvisible,
   updateInterval,
-  forceNotSend,
-  onUseHttpPythonSuccess,
-  onUseHttpPythonError,
-  beforeRequest,
   getExtraRequestData,
-}: IUseHttpPython<R>) {
+  onMessage,
+  onSocketError,
+}: IUseSocketPython<R>) {
   const deps = [
+    t,
+    lang,
+    hash,
     node?.alias,
     nodes.map((n) => n.alias).join("_"),
     endpoint,
     identifier,
     updateInterval,
     isInvisible,
-    forceNotSend,
+    getExtraRequestData,
   ];
+
+  const getMessage = useCallback(
+    () =>
+      getPythonRequest({
+        node,
+        nodes,
+        identifier,
+        getExtraRequestData,
+        opt: { t, lang },
+      }).then((req) => ({ hash: hash!, ...req })),
+    [deps],
+  );
+
   const requestFn = useCallback(() => {
-    if (isInvisible || forceNotSend) return Promise.resolve();
-    const exportBox = new INodes(nodes).bbox;
-    const preprocess = beforeRequest ? beforeRequest() : Promise.resolve();
-    return preprocess
-      .then(() =>
-        getPythonRequest({
-          node,
-          nodes,
-          identifier,
-          getExtraRequestData,
-          opt: { t, lang, exportBox },
-        }),
-      )
-      .then((req) => Requests.postJson<IPythonResponse<R>>("_python", endpoint, req))
-      .then((res) => {
-        if (res.success) return onUseHttpPythonSuccess(res);
-        throw Error(res.message);
-      })
-      .catch((err) => {
-        if (onUseHttpPythonError) return onUseHttpPythonError(err);
-        Logger.error(err);
-      });
-  }, deps);
+    useWebSocketHook({
+      isInvisible,
+      hash,
+      getMessage,
+      onMessage,
+      onSocketError,
+      updateInterval,
+    });
+  }, [getMessage, onMessage, onSocketError]);
 
-  useEffect(() => {
-    let timer: any;
-    let shouldIgnore = false; // IMPORTANT!
-    function requestWithTimeout() {
-      if (isInvisible || shouldIgnore) return;
-      requestFn().then(() => (timer = setTimeout(requestWithTimeout, updateInterval)));
-    }
-    if (!updateInterval) requestFn();
-    else requestWithTimeout();
-
-    return () => {
-      shouldIgnore = true;
-      clearTimeout(timer);
-    };
-  }, deps);
+  requestFn();
 }
 
 export function useSyncPython() {
-  const getMessage = () => ({
-    identifier: "sync",
-    nodeData: {},
-    nodeDataList: [],
-    extraData: {},
-    isInternal: true,
-  });
-
-  useWebSocket<IPythonStore>({
-    getMessage,
-    onMessage: async ({ success, message, data: { status, data } }) => {
-      if (!success) {
-        Logger.warn(`sync python settings failed: ${message}`);
-        return { newMessage: getMessage };
-      }
+  const hash = "0";
+  const getMessage = useCallback(
+    (): Promise<IPythonSocketRequest> =>
+      Promise.resolve({
+        hash,
+        userId: userStore.userId,
+        identifier: "sync",
+        nodeData: {},
+        nodeDataList: [],
+        extraData: {},
+        isInternal: true,
+      }),
+    [],
+  );
+  const onMessage = useCallback<IPythonOnSocketMessage<IPythonStore>>(
+    async ({ status, total, pending, message, data: { progress, final } }) => {
       if (status !== "finished") {
-        Logger.warn(`sync in progress: ${JSON.stringify(data)}`);
+        if (status === "pending") {
+          Logger.warn(`sync pending: ${pending} / ${total}`);
+        } else if (status === "working") {
+          // Logger.warn(`sync in progress: ${progress}`);
+        } else {
+          Logger.warn(`sync failed: ${message}`);
+          return { newMessage: getMessage };
+        }
+        return {};
       } else {
-        if (updatePythonStore(data)) {
-          Logger.log(`sync successfully: ${JSON.stringify(data)}, rerendering`);
+        if (!final) {
+          Logger.warn("sync data not found");
+          return { newMessage: getMessage };
         }
-        return { newMessage: getMessage };
+        if (updatePythonStore(final)) {
+          Logger.log(`sync successfully: ${JSON.stringify(final)}, rerendering`);
+        }
+        return debugStore.pollSync ? { newMessage: getMessage } : {};
       }
     },
-  });
+    [],
+  );
+
+  useWebSocketHook<IPythonStore>({ isInvisible: false, hash, getMessage, onMessage });
 }
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/add.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/add.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/brush.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/brush.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/download.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/index.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/plugins.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/plugins.ts`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
   allAvailablePlugins,
   allAvailablePythonPlugins,
   AvailablePluginsAndPythonPlugins,
 } from "@/schema/plugins";
 
 const _pluginsLangRecords: Record<Lang, Record<AvailablePluginsAndPythonPlugins, string>> = {
   zh: {
+    meta: "元数据",
     settings: "设置",
     project: "项目",
     add: "添加",
     arrange: "智能整理",
     undo: "撤销",
     redo: "重做",
     download: "下载",
@@ -19,19 +20,20 @@
     wiki: "文档",
     github: "Github",
     email: "邮件",
     textEditor: "编辑文本",
     groupEditor: "编辑组",
     multiEditor: "编辑多节点",
     brush: "画笔",
-    "_python.httpTextArea": "Python 文本框",
-    "_python.httpQA": "Python 问答",
-    "_python.httpFields": "Python 插件",
+    "_python.textArea": "Python 文本框",
+    "_python.QA": "Python 问答",
+    "_python.fields": "Python 插件",
   },
   en: {
+    meta: "Meta",
     settings: "Settings",
     project: "Project",
     add: "Add",
     arrange: "Auto Arrange",
     undo: "Undo",
     redo: "Redo",
     download: "Download",
@@ -39,17 +41,17 @@
     wiki: "Wiki",
     github: "Github",
     email: "Email",
     textEditor: "Edit Text",
     groupEditor: "Edit Group",
     multiEditor: "Edit Multi Nodes",
     brush: "Brush",
-    "_python.httpTextArea": "Python TextArea",
-    "_python.httpQA": "Python Q & A",
-    "_python.httpFields": "Python Plugin",
+    "_python.textArea": "Python TextArea",
+    "_python.QA": "Python Q & A",
+    "_python.fields": "Python Plugin",
   },
 };
 
 export const Plugins_Words: Record<AvailablePluginsAndPythonPlugins, string> = {} as any;
 export const pluginsLangRecords: Dictionary<Dictionary<string>> = {};
 
 function injectScope(scope: string, data: Dictionary<string>) {
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/projects.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/settings.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/settings.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/toast.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/toast.ts`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,18 @@
   "downloading-project-message" = "downloading-project-message",
   "importing-local-project-message" = "importing-local-project-message",
   "import-local-project-success-message" = "import-local-project-success-message",
   "import-local-project-error-message" = "import-local-project-error-message",
   "add-text-success-message" = "add-text-success-message",
   "add-text-error-message" = "add-text-error-message",
   "auto-arrange-no-need-message" = "auto-arrange-no-need-message",
+  "submit-task-busy-message" = "submit-task-busy-message",
   "submit-task-success-message" = "submit-task-success-message",
   "submit-task-error-message" = "submit-task-error-message",
+  "submit-task-finished-message" = "submit-task-finished-message",
   "downloading-nodes-message" = "downloading-nodes-message",
   "export-blob-error-message" = "export-blob-error-message",
   "enter-brush-mode-message" = "enter-brush-mode-message",
   "exit-brush-mode-message" = "exit-brush-mode-message",
 }
 
 export const toastLangRecords: Record<Lang, Record<Toast_Words, string>> = {
@@ -53,16 +55,18 @@
     [Toast_Words["downloading-project-message"]]: "下载项目中",
     [Toast_Words["importing-local-project-message"]]: "导入中",
     [Toast_Words["import-local-project-success-message"]]: "导入成功",
     [Toast_Words["import-local-project-error-message"]]: "导入失败",
     [Toast_Words["add-text-success-message"]]: "添加文字成功",
     [Toast_Words["add-text-error-message"]]: "添加文字时出了些问题",
     [Toast_Words["auto-arrange-no-need-message"]]: "当前节点无需整理",
+    [Toast_Words["submit-task-busy-message"]]: "当前任务正在执行中，请稍候...",
     [Toast_Words["submit-task-success-message"]]: "任务提交成功",
     [Toast_Words["submit-task-error-message"]]: "执行任务时出了些问题",
+    [Toast_Words["submit-task-finished-message"]]: "任务已执行完成",
     [Toast_Words["downloading-nodes-message"]]: "下载中",
     [Toast_Words["export-blob-error-message"]]: "导出节点时出了些问题",
     [Toast_Words["enter-brush-mode-message"]]: "已进入涂鸦模式",
     [Toast_Words["exit-brush-mode-message"]]: "已退出涂鸦模式",
   },
   en: {
     [Toast_Words["dropping-message"]]: "Detecting",
@@ -84,15 +88,18 @@
     [Toast_Words["downloading-project-message"]]: "Downloading",
     [Toast_Words["importing-local-project-message"]]: "Importing",
     [Toast_Words["import-local-project-success-message"]]: "Imported successfully!",
     [Toast_Words["import-local-project-error-message"]]: "Import failed",
     [Toast_Words["add-text-success-message"]]: "Text added successfully",
     [Toast_Words["add-text-error-message"]]: "Something is wrong when adding Text Node",
     [Toast_Words["auto-arrange-no-need-message"]]: "There is no need to arrange the Nodes",
+    [Toast_Words["submit-task-busy-message"]]:
+      "Current task is being executed, please wait for a while...",
     [Toast_Words["submit-task-success-message"]]: "Task submitted successfully!",
     [Toast_Words["submit-task-error-message"]]: "Something is wrong when executing the task",
+    [Toast_Words["submit-task-finished-message"]]: "Task has been executed successfully",
     [Toast_Words["downloading-nodes-message"]]: "Downloading",
     [Toast_Words["export-blob-error-message"]]: "Something is wrong when exporting Node",
     [Toast_Words["enter-brush-mode-message"]]: "Entered sketch mode",
     [Toast_Words["exit-brush-mode-message"]]: "Exited sketch mode",
   },
 };
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/ui.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/lang/ui.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/AddPlugin.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/AddPlugin.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 import { loadLocalProject, saveProject } from "@/actions/manageProjects";
 import { getNewProject } from "@/stores/projects";
 import CFButton from "@/components/CFButton";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import CFImageUploader from "@/components/CFImageUploader";
 import { drawboardPluginFactory } from "./utils/factory";
-import { floatingControlEvent, floatingEvent } from "./components/Floating";
+import { floatingEvent } from "./components/Floating";
 import Render from "./components/Render";
+import { useClosePanel } from "./components/hooks";
 
 const AddPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `add_${getRandomHash()}`, []);
   const t = useToast();
   const lang = langStore.tgt;
 
-  const closePanel = () => floatingControlEvent.emit({ id, expand: false });
+  const closePanel = useClosePanel(id);
   const onNewProject = () => {
     toast(t, "info", translate(Toast_Words["adding-project-message"], lang));
     saveProject(
       t,
       lang,
       async () =>
         loadLocalProject(
@@ -70,10 +71,8 @@
           {translate(Add_Words["add-text-button"], lang)}
         </CFButton>
       </Flex>
     </Render>
   );
 };
 
-const _ = observer(AddPlugin);
-drawboardPluginFactory.register("add")(_);
-export default _;
+drawboardPluginFactory.register("add", true)(observer(AddPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/ArrangePlugin.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/ArrangePlugin.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     <Render
       id={id}
       onFloatingButtonClick={async () => onArrange(t, lang, { type: "multiple", nodes })}
       {...props}
     />
   );
 };
-drawboardPluginFactory.register("arrange")(observer(ArrangePlugin));
+drawboardPluginFactory.register("arrange", true)(observer(ArrangePlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/BrushPlugin.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/BrushPlugin.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -137,8 +137,8 @@
           switchBrushMode();
         }}>
         {translate(Brush_Words["finish-brush-message"], lang)}
       </CFButton>
     </Render>
   );
 };
-drawboardPluginFactory.register("brush")(observer(BrushPlugin));
+drawboardPluginFactory.register("brush", true)(observer(BrushPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/DeletePlugin.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/DeletePlugin.tsx`

 * *Files 13% similar despite different names*

```diff
@@ -14,10 +14,8 @@
   if (type === "none") return null;
   function onDelete(): void {
     useSafeExecute("remove", null, true)(nodes.map((node) => node.alias));
   }
   return <Render id={id} onFloatingButtonClick={async () => onDelete()} {...props} />;
 };
 
-const _ = observer(DeletePlugin);
-drawboardPluginFactory.register("delete")(_);
-export default _;
+drawboardPluginFactory.register("delete", true)(observer(DeletePlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/DownloadPlugin.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/DownloadPlugin.tsx`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import { downloadNodes } from "@/actions/download";
 import CFSelect, { CFSrollableSelect } from "@/components/CFSelect";
 import CFText from "@/components/CFText";
 import CFButton from "@/components/CFButton";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import { drawboardPluginFactory } from "./utils/factory";
-import { floatingControlEvent } from "./components/Floating";
 import Render from "./components/Render";
+import { useClosePanel } from "./components/hooks";
 
 const DownloadPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `download_${getRandomHash()}`, []);
   const t = useToast();
   const lang = langStore.tgt;
   const { type, nodes } = useSelecting("raw");
   const { w, h, imgWH } = useSelecting("basic")({ fixed: 0 }) ?? {};
@@ -41,15 +41,15 @@
   const getWord = (keepOriginal: string) =>
     translate(
       keepOriginal === "true"
         ? Download_Words["download-image-size-original"]
         : Download_Words["download-image-size-drawboard"],
       lang,
     );
-  const closePanel = () => floatingControlEvent.emit({ id, expand: false });
+  const closePanel = useClosePanel(id);
   const onDownload = () => {
     downloadNodes(t, lang, nodes, format, keepOriginal);
     closePanel();
   };
 
   return (
     <Render id={id} {...props}>
@@ -83,10 +83,8 @@
           {translate(Download_Words["download-button"], lang)}
         </CFButton>
       </Flex>
     </Render>
   );
 };
 
-const _ = observer(DownloadPlugin);
-drawboardPluginFactory.register("download")(_);
-export default _;
+drawboardPluginFactory.register("download", true)(observer(DownloadPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/GroupPlugin.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/GroupPlugin.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -14,9 +14,10 @@
   return <Render id={id} onFloatingButtonClick={async () => unGroup?.()} {...props} />;
 };
 const MultiEditorPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `multiEditor_${getRandomHash()}`, []);
   const { setGroup } = useSelecting("multiple") ?? {};
   return <Render id={id} onFloatingButtonClick={async () => setGroup?.()} {...props} />;
 };
-drawboardPluginFactory.register("groupEditor")(observer(GroupEditorPlugin));
-drawboardPluginFactory.register("multiEditor")(observer(MultiEditorPlugin));
+
+drawboardPluginFactory.register("groupEditor", true)(observer(GroupEditorPlugin));
+drawboardPluginFactory.register("multiEditor", true)(observer(MultiEditorPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/LinksPlugin.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/LinksPlugin.tsx`

 * *Files 10% similar despite different names*

```diff
@@ -15,10 +15,11 @@
   const id = useMemo(() => `emailLink_${getRandomHash()}`, []);
   return <Link id={id} href="mailto: syameimaru.saki@gmail.com" {...props} />;
 };
 const GitHubPlugin = (props: IPlugin) => {
   const id = useMemo(() => `githubLink_${getRandomHash()}`, []);
   return <Link id={id} url="https://github.com/carefree0910/carefree-drawboard" {...props} />;
 };
-drawboardPluginFactory.register("wiki")(observer(WikiPlugin));
-drawboardPluginFactory.register("email")(observer(EmailPlugin));
-drawboardPluginFactory.register("github")(observer(GitHubPlugin));
+
+drawboardPluginFactory.register("wiki", true)(observer(WikiPlugin));
+drawboardPluginFactory.register("email", true)(observer(EmailPlugin));
+drawboardPluginFactory.register("github", true)(observer(GitHubPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/ProjectPlugin.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/ProjectPlugin.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,25 @@
 import { setCurrentProjectName, useCurrentProject } from "@/stores/projects";
 import {
   ILoadedProject,
   fetchAllProjects,
   loadProject,
   saveProject,
 } from "@/actions/manageProjects";
+import { downloadCurrentFullProject } from "@/actions/download";
 import CFText from "@/components/CFText";
 import CFInput from "@/components/CFInput";
 import CFButton from "@/components/CFButton";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import { CFSrollableSelect } from "@/components/CFSelect";
 import { drawboardPluginFactory } from "./utils/factory";
 import Render from "./components/Render";
-import { floatingControlEvent, floatingEvent, floatingRenderEvent } from "./components/Floating";
-import { downloadCurrentFullProject } from "@/actions/download";
+import { floatingEvent, floatingRenderEvent } from "./components/Floating";
+import { useClosePanel } from "./components/hooks";
 
 type IImportLocal = ILoadedProject | INodePack[];
 const ProjectPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `project_${getRandomHash()}`, []);
   const t = useToast();
   const lang = langStore.tgt;
   const { uid, name } = useCurrentProject();
@@ -68,15 +69,15 @@
 
     return () => {
       floatingDispose();
       floatingRenderDispose();
     };
   }, [id]);
 
-  const closePanel = () => floatingControlEvent.emit({ id, expand: false });
+  const closePanel = useClosePanel(id);
   function updateProjectStates(uid: string, name: string) {
     setSelectedUid(uid);
     setUserInputName(name);
   }
 
   function onRenameProject() {
     setCurrentProjectName(userInputName);
@@ -168,10 +169,8 @@
           </CFButton>
         </Upload>
       </Flex>
     </Render>
   );
 };
 
-const _ = observer(ProjectPlugin);
-drawboardPluginFactory.register("project")(_);
-export default _;
+drawboardPluginFactory.register("project", true)(observer(ProjectPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/SettingsPlugin.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/SettingsPlugin.tsx`

 * *Files 5% similar despite different names*

```diff
@@ -118,10 +118,8 @@
           </Flex>
         </Box>
       </Flex>
     </Render>
   );
 };
 
-const _ = observer(SettingsPlugin);
-drawboardPluginFactory.register("settings")(_);
-export default _;
+drawboardPluginFactory.register("settings", true)(observer(SettingsPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/TextEditorPlugin.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/TextEditorPlugin.tsx`

 * *Files 0% similar despite different names*

```diff
@@ -60,8 +60,8 @@
           }}
           onBlur={() => editContent({ trace: true })(content)}
         />
       </Flex>
     </Render>
   );
 };
-drawboardPluginFactory.register("textEditor")(observer(TextEditorPlugin));
+drawboardPluginFactory.register("textEditor", true)(observer(TextEditorPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -12,9 +12,10 @@
   const id = useMemo(() => `undo_${getRandomHash()}`, []);
   return <Render id={id} onFloatingButtonClick={async () => safeUndo()} {...props} />;
 };
 const RedoPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `redo_${getRandomHash()}`, []);
   return <Render id={id} onFloatingButtonClick={async () => safeRedo()} {...props} />;
 };
-drawboardPluginFactory.register("undo")(observer(UndoPlugin));
-drawboardPluginFactory.register("redo")(observer(RedoPlugin));
+
+drawboardPluginFactory.register("undo", true)(observer(UndoPlugin));
+drawboardPluginFactory.register("redo", true)(observer(RedoPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpFieldsPlugin.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx`

 * *Files 17% similar despite different names*

```diff
@@ -1,96 +1,93 @@
-import { useMemo, useCallback } from "react";
+import { useCallback } from "react";
 import { observer } from "mobx-react-lite";
 import { CloseIcon } from "@chakra-ui/icons";
 import { Flex, Spacer, useToast } from "@chakra-ui/react";
 
-import { Dictionary, getRandomHash } from "@carefree0910/core";
 import { langStore, translate } from "@carefree0910/business";
 
-import type { IMeta, IPythonHttpFieldsResponse } from "@/schema/meta";
-import type { IPythonHttpFieldsPlugin, IPythonResponse } from "@/schema/_python";
+import type { IPythonFieldsResponse } from "@/schema/meta";
+import type { IPythonFieldsPlugin, IPythonOnSocketMessage } from "@/schema/_python";
 import { UI_Words } from "@/lang/ui";
 import { Toast_Words } from "@/lang/toast";
 import { toast } from "@/utils/toast";
 import { titleCaseWord } from "@/utils/misc";
+import { removeSocketHook, socketLog } from "@/stores/socket";
 import { importMeta } from "@/actions/importMeta";
-import { getMetaField } from "@/stores/meta";
-import { drawboardPluginFactory } from "@/plugins/utils/factory";
 import CFHeading from "@/components/CFHeading";
-import { useDefinitions } from "../components/Fields";
-import { floatingControlEvent } from "../components/Floating";
-import { useIdentifierId } from "./hooks";
-import PythonHttpPluginWithSubmit from "./HttpPluginWithSubmit";
-
-const PythonHttpFieldsPlugin = ({ pluginInfo, ...props }: IPythonHttpFieldsPlugin) => {
-  const identifierId = useIdentifierId(pluginInfo.identifier);
-  const id = useMemo(() => `${identifierId}_${getRandomHash()}`, [identifierId]);
+import { drawboardPluginFactory } from "@/plugins/utils/factory";
+import { useClosePanel } from "../components/hooks";
+import { useCurrentMeta, useDefinitionsRequestDataFn, useFieldsPluginIds } from "./hooks";
+import PythonPluginWithSubmit, { socketFinishedEvent } from "./PluginWithSubmit";
+import DefinitionFields from "./DefinitionFields";
+
+const PythonFieldsPlugin = ({ pluginInfo, ...props }: IPythonFieldsPlugin) => {
+  const { id, identifierId } = useFieldsPluginIds(pluginInfo.identifier);
   const t = useToast();
   const lang = langStore.tgt;
   const definitions = pluginInfo.definitions;
-  const getExtraRequestData = useMemo(
-    () => () => {
-      const data: Dictionary<any> = {};
-      Object.keys(definitions).forEach((field) => {
-        data[field] = getMetaField(field);
-      });
-      return data;
+  const getExtraRequestData = useDefinitionsRequestDataFn(definitions);
+  const currentMeta = useCurrentMeta(pluginInfo.node);
+  const emitClose = useClosePanel(id);
+
+  const onMessage = useCallback<IPythonOnSocketMessage<IPythonFieldsResponse>>(
+    async ({ hash, status, total, pending, data: { progress, intermediate, final } }) => {
+      switch (status) {
+        case "finished": {
+          socketFinishedEvent.emit({ id });
+          if (!final) {
+            toast(
+              t,
+              "success",
+              `${translate(Toast_Words["submit-task-finished-message"], lang)} (${identifierId})`,
+            );
+          } else {
+            const { _duration, ...response } = final;
+            importMeta({
+              t,
+              lang,
+              type: "python.fields",
+              metaData: {
+                identifier: identifierId,
+                parameters: getExtraRequestData(),
+                response,
+                duration: _duration,
+                from: currentMeta,
+              },
+            });
+          }
+          socketLog(`> remove hook (${hash})`);
+          removeSocketHook(hash);
+        }
+      }
+      return {};
+    },
+    [id, lang, identifierId, currentMeta, getExtraRequestData],
+  );
+  const onSocketError = useCallback(
+    async (err: any) => {
+      toast(t, "error", `${translate(Toast_Words["submit-task-error-message"], lang)} - ${err}`);
     },
-    [definitions],
+    [t, lang],
   );
-  const currentMeta = useMemo(() => {
-    const node = pluginInfo.node;
-    let currentMeta: IMeta | undefined;
-    if (node && node.type !== "group") {
-      currentMeta = node.params.meta as IMeta;
-    }
-    return currentMeta;
-  }, [pluginInfo.node]);
-  const emitClose = useCallback(() => floatingControlEvent.emit({ id, expand: false }), [id]);
-
-  async function onUseHttpPythonSuccess({
-    data: { _duration, ...response },
-  }: IPythonResponse<IPythonHttpFieldsResponse>) {
-    importMeta({
-      t,
-      lang,
-      type: "python.httpFields",
-      metaData: {
-        identifier: identifierId,
-        parameters: getExtraRequestData(),
-        response,
-        duration: _duration,
-        from: currentMeta,
-      },
-    });
-  }
-  async function onUseHttpPythonError(err: any) {
-    toast(t, "error", `${translate(Toast_Words["submit-task-error-message"], lang)} - ${err}`);
-  }
 
   const header = pluginInfo.header ?? titleCaseWord(identifierId);
   return (
-    <PythonHttpPluginWithSubmit
+    <PythonPluginWithSubmit
       id={id}
       buttonText={translate(UI_Words["submit-task"], lang)}
       getExtraRequestData={getExtraRequestData}
-      onUseHttpPythonSuccess={onUseHttpPythonSuccess}
-      onUseHttpPythonError={onUseHttpPythonError}
+      onMessage={onMessage}
+      onSocketError={onSocketError}
       pluginInfo={pluginInfo}
       {...props}>
       <Flex>
         <CFHeading>{header}</CFHeading>
         <Spacer />
         <CloseIcon w="12px" cursor="pointer" onClick={emitClose} />
       </Flex>
-      {Object.keys(definitions).length > 0 && (
-        <Flex p="12px" gap="12px" flexWrap="wrap" alignItems="center" justifyContent="space-around">
-          {useDefinitions(definitions, pluginInfo.numColumns)}
-        </Flex>
-      )}
-    </PythonHttpPluginWithSubmit>
+      <DefinitionFields definitions={definitions} numColumns={pluginInfo.numColumns} />
+    </PythonPluginWithSubmit>
   );
 };
 
-const _ = observer(PythonHttpFieldsPlugin);
-drawboardPluginFactory.registerPython("_python.httpFields", true)(_);
-export default _;
+drawboardPluginFactory.registerPython("_python.fields", true)(observer(PythonFieldsPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpPluginWithSubmit.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,100 @@
-import { useState } from "react";
+import { useCallback, useEffect, useState } from "react";
 import { observer } from "mobx-react-lite";
 import { useToast } from "@chakra-ui/react";
 
+import { getRandomHash } from "@carefree0910/core";
 import { langStore, translate } from "@carefree0910/business";
 
-import type { IPythonHttpPluginWithSubmit } from "@/schema/_python";
+import type { IPythonSocketPluginWithSubmit } from "@/schema/_python";
+import { Event } from "@/utils/event";
 import { toast } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
-import { useHttpPython } from "@/hooks/usePython";
-import CFButton from "@/components/CFButton";
+import { userStore } from "@/stores/user";
+import { useSocketPython } from "@/hooks/usePython";
+import { CFButtonWithBusyTooltip } from "@/components/CFButton";
 import CFDivider from "@/components/CFDivider";
 import Render from "../components/Render";
 import { floatingControlEvent } from "../components/Floating";
 
-const PythonHttpPluginWithSubmit = ({
+export const socketFinishedEvent = new Event<{ id: string }>();
+function PythonPluginWithSubmit<R>({
   id,
   pluginInfo: {
     node,
     nodes,
     endpoint,
     identifier,
     updateInterval,
     closeOnSubmit = true,
     toastOnSubmit = true,
-    submitToastMessage,
+    toastMessageOnSubmit,
   },
   buttonText,
-  onUseHttpPythonError,
-  onUseHttpPythonSuccess,
-  beforeRequest,
+  onMessage,
+  onSocketError,
   getExtraRequestData,
   children,
   ...props
-}: IPythonHttpPluginWithSubmit<any>) => {
+}: IPythonSocketPluginWithSubmit<R>) {
   const t = useToast();
   const lang = langStore.tgt;
-  const [send, setSend] = useState(false);
+  const [hash, setHash] = useState<number | undefined>(undefined);
+  const [busy, setBusy] = useState(false);
+  const onClick = useCallback(() => {
+    if (busy) return;
+    if (!userStore.canAlwaysSubmit) {
+      setBusy(true);
+    }
+    setHash(getRandomHash());
+    if (closeOnSubmit) {
+      floatingControlEvent.emit({ id, expand: false });
+    }
+    if (toastOnSubmit) {
+      toastMessageOnSubmit ??= translate(Toast_Words["submit-task-success-message"], lang);
+      toast(t, "info", toastMessageOnSubmit);
+    }
+  }, [id, t, lang, closeOnSubmit, toastOnSubmit, toastMessageOnSubmit, busy]);
 
-  useHttpPython<{ text: string }>({
+  useSocketPython<R>({
     t,
     lang,
+    hash: hash?.toString(),
     node,
     nodes,
     endpoint,
     identifier,
     isInvisible: props.renderInfo.isInvisible ?? false,
     updateInterval,
-    forceNotSend: !send,
-    onUseHttpPythonError,
-    onUseHttpPythonSuccess,
-    beforeRequest: async () => {
-      setSend(false);
-      beforeRequest && (await beforeRequest());
-    },
+    onMessage,
+    onSocketError,
     getExtraRequestData,
   });
 
-  function onClick() {
-    setSend(true);
-    if (closeOnSubmit) {
-      floatingControlEvent.emit({ id, expand: false });
-    }
-    if (toastOnSubmit) {
-      submitToastMessage ??= translate(Toast_Words["submit-task-success-message"], lang);
-      toast(t, "info", submitToastMessage);
-    }
-  }
+  useEffect(() => {
+    const { dispose } = socketFinishedEvent.on(({ id: incomingId }) => {
+      if (incomingId === id) {
+        setBusy(false);
+        setHash(undefined);
+      }
+    });
+
+    return () => {
+      dispose();
+    };
+  }, [id, setBusy, setHash]);
 
   return (
     <Render id={id} {...props}>
       {children}
       <CFDivider />
-      <CFButton onClick={onClick}>{buttonText}</CFButton>
+      <CFButtonWithBusyTooltip
+        busy={busy}
+        tooltip={translate(Toast_Words["submit-task-busy-message"], lang)}
+        onClick={onClick}>
+        {buttonText}
+      </CFButtonWithBusyTooltip>
     </Render>
   );
-};
+}
 
-export default observer(PythonHttpPluginWithSubmit);
+export default observer(PythonPluginWithSubmit);
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpQAPlugin.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/_python/QAPlugin.tsx`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,55 @@
-import { useMemo, useState } from "react";
+import { useCallback, useMemo, useState } from "react";
 import { observer } from "mobx-react-lite";
 import { Textarea } from "@chakra-ui/react";
 
 import { getRandomHash } from "@carefree0910/core";
 import { langStore, translate } from "@carefree0910/business";
 
-import type { IPythonHttpQAPlugin, IPythonResponse } from "@/schema/_python";
+import type { IPythonOnSocketMessage, IPythonQAPlugin } from "@/schema/_python";
 import { UI_Words } from "@/lang/ui";
 import CFInput from "@/components/CFInput";
 import { drawboardPluginFactory } from "@/plugins/utils/factory";
 import { useIdentifierId } from "./hooks";
-import PythonHttpPluginWithSubmit from "./HttpPluginWithSubmit";
+import PythonPluginWithSubmit from "./PluginWithSubmit";
 
-const PythonHttpQAPlugin = ({ pluginInfo, ...props }: IPythonHttpQAPlugin) => {
+const PythonQAPlugin = ({ pluginInfo, ...props }: IPythonQAPlugin) => {
   const identifierId = useIdentifierId(pluginInfo.identifier);
   const id = useMemo(() => `${identifierId}_QA_${getRandomHash()}`, []);
   const [userInput, setUserInput] = useState("");
   const [serverText, setServerText] = useState(pluginInfo.initialText);
   const lang = langStore.tgt;
-
-  function getExtraRequestData() {
-    return { text: userInput };
-  }
-  async function onUseHttpPythonSuccess(res: IPythonResponse<{ text: string }>) {
-    setServerText(res.data.text);
-  }
+  const getExtraRequestData = useCallback(() => ({ text: userInput }), [userInput]);
+  const onMessage = useCallback<IPythonOnSocketMessage<{ text: string }>>(
+    async ({ status, data }) => {
+      if (status === "finished") {
+        setServerText(data.final?.text ?? "");
+      } else {
+        setServerText("Thinking...");
+      }
+      return {};
+    },
+    [setServerText],
+  );
 
   return (
-    <PythonHttpPluginWithSubmit
+    <PythonPluginWithSubmit
       id={id}
       buttonText={translate(UI_Words["submit-task"], lang)}
       getExtraRequestData={getExtraRequestData}
-      onUseHttpPythonSuccess={onUseHttpPythonSuccess}
+      onMessage={onMessage}
       pluginInfo={pluginInfo}
       {...props}>
       <Textarea w="100%" h="40%" minH="0px" value={serverText} readOnly />
       <CFInput
         w="100%"
         h="30%"
         mt="16px"
         value={userInput}
         onChange={(event) => setUserInput(event.target.value)}
         placeholder={translate(UI_Words["qa-field-placeholder"], langStore.tgt)}
       />
-    </PythonHttpPluginWithSubmit>
+    </PythonPluginWithSubmit>
   );
 };
 
-const _ = observer(PythonHttpQAPlugin);
-drawboardPluginFactory.registerPython("_python.httpQA", true)(_);
-export default _;
+drawboardPluginFactory.registerPython("_python.QA", true)(observer(PythonQAPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpTextAreaPlugin.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,56 @@
-import { useMemo, useState } from "react";
+import { useCallback, useMemo, useState } from "react";
 import { observer } from "mobx-react-lite";
 import { Textarea, useToast } from "@chakra-ui/react";
 
 import { getRandomHash } from "@carefree0910/core";
 import { langStore } from "@carefree0910/business";
 
-import type { IPythonHttpTextAreaPlugin } from "@/schema/_python";
-import { useHttpPython } from "@/hooks/usePython";
+import type { IPythonTextAreaPlugin, IPythonOnSocketMessage } from "@/schema/_python";
+import { useSocketPython } from "@/hooks/usePython";
 import { drawboardPluginFactory } from "@/plugins/utils/factory";
 import Render from "@/plugins/components/Render";
 import { useIdentifierId } from "./hooks";
 
-const PythonHttpTextAreaPlugin = ({
+const PythonTextAreaPlugin = ({
   pluginInfo: { node, nodes, endpoint, identifier, updateInterval, noLoading, textAlign },
   ...props
-}: IPythonHttpTextAreaPlugin) => {
+}: IPythonTextAreaPlugin) => {
   const t = useToast();
   const lang = langStore.tgt;
   const identifierId = useIdentifierId(identifier);
-  const id = useMemo(() => `${identifierId}_textArea_${getRandomHash()}`, []);
+  const id = useMemo(() => `${identifierId}_textArea_${getRandomHash()}`, [identifierId]);
+  const hash = useMemo(() => getRandomHash().toString(), [id]);
   const [value, setValue] = useState("");
+  const onMessage = useCallback<IPythonOnSocketMessage<{ text: string }>>(
+    async ({ status, data }) => {
+      if (status === "finished") {
+        setValue(data.final?.text ?? "");
+      } else if (!noLoading) {
+        setValue("Loading...");
+      }
+      return {};
+    },
+    [setValue],
+  );
 
-  useHttpPython<{ text: string }>({
+  useSocketPython({
     t,
     lang,
+    hash,
     node,
     nodes,
     endpoint,
     identifier,
     isInvisible: props.renderInfo.isInvisible ?? false,
     updateInterval,
-    onUseHttpPythonSuccess: async (res) => setValue(res.data.text),
-    beforeRequest: noLoading ? undefined : async () => setValue("Loading..."),
+    onMessage,
   });
 
   return (
     <Render id={id} {...props}>
       <Textarea w="100%" h="100%" minH="0px" value={value} textAlign={textAlign} readOnly />
     </Render>
   );
 };
 
-const _ = observer(PythonHttpTextAreaPlugin);
-drawboardPluginFactory.registerPython("_python.httpTextArea", true)(_);
-export default _;
+drawboardPluginFactory.registerPython("_python.textArea", true)(observer(PythonTextAreaPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/TextField.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/Fields/TextField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/index.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/Fields/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/utils.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/Fields/utils.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Floating.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/Floating.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Render.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/components/Render.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/index.tsx` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/index.tsx`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 
 import type { AvailablePluginsAndPythonPlugins, IMakePlugin } from "@/schema/plugins";
 import { pluginIsVisible, pythonPluginIsVisible } from "@/stores/plugins";
 import { drawboardPluginFactory } from "./utils/factory";
 import { getNodeFilter } from "./utils/renderFilters";
 
 // these lines are needed to make sure the plugins are registered
+export * from "./MetaPlugin";
 export * from "./SettingsPlugin";
 export * from "./ProjectPlugin";
 export * from "./AddPlugin";
 export * from "./ArrangePlugin";
 export * from "./UndoRedoPlugin";
 export * from "./DownloadPlugin";
 export * from "./DeletePlugin";
 export * from "./TextEditorPlugin";
 export * from "./GroupPlugin";
 export * from "./LinksPlugin";
 export * from "./BrushPlugin";
-export * from "./_python/HttpTextAreaPlugin";
-export * from "./_python/HttpQAPlugin";
-export * from "./_python/HttpFieldsPlugin";
+export * from "./_python/TextAreaPlugin";
+export * from "./_python/QAPlugin";
+export * from "./_python/FieldsPlugin";
 
 export function makePlugin<T extends AvailablePluginsAndPythonPlugins>({
   key,
   type,
   containerRef,
   props: { renderInfo, pluginInfo, ...props },
 }: IMakePlugin<T> & { key: string }) {
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/utils/factory.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/utils/factory.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/utils/renderFilters.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/plugins/utils/renderFilters.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/react-app-env.d.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/react-app-env.d.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/interceptors/_python.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/requests/interceptors/_python.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/interceptors/index.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/requests/interceptors/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/meta.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/schema/meta.ts`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import type { Dictionary, Lang } from "@carefree0910/core";
 
 import type { IToast } from "./misc";
 
 // general
 
-export const allMetaTypes = ["upload", "python.httpFields", "add.text", "add.sketch.path"] as const;
-export type MetaType = typeof allMetaTypes[number];
+export const allMetaTypes = ["upload", "add.text", "add.sketch.path", "python.fields"] as const;
+export type MetaType = (typeof allMetaTypes)[number];
 export interface ICommonMetaData<T extends _IMetaData = _IMetaData> {
+  alias?: string;
   timestamp?: number;
   duration?: number;
   from?: IMeta<T>;
 }
 type _IMetaData = ICommonMetaData & Dictionary<any>;
 export interface IMeta<T extends _IMetaData = _IMetaData> {
   type: MetaType;
@@ -21,29 +22,29 @@
 
 interface IUploadMetaData extends ICommonMetaData {
   w: number;
   h: number;
   url: string;
   isDrag: boolean;
 }
-export type IPythonHttpFieldsResponse = { _duration?: number } & (
+export type IPythonFieldsResponse = { _duration?: number } & (
   | { type: "text"; value: string[] }
   | { type: "image"; value: { w: number; h: number; url: string }[] }
 );
-export type IPythonHttpFieldsMetaData = ICommonMetaData & {
+export type IPythonFieldsMetaData = ICommonMetaData & {
   identifier: string;
   parameters: Dictionary<any>;
-  response: IPythonHttpFieldsResponse;
+  response: IPythonFieldsResponse;
 };
 
 export interface IMetaData {
   upload: IUploadMetaData;
   "add.text": ICommonMetaData;
   "add.sketch.path": ICommonMetaData;
-  "python.httpFields": IPythonHttpFieldsMetaData;
+  "python.fields": IPythonFieldsMetaData;
 }
 
 export interface IImportMeta<T extends MetaType> {
   t: IToast;
   lang: Lang;
   type: T;
   metaData: IMetaData[T];
@@ -54,7 +55,11 @@
 export function checkMeta(meta: any): meta is IMeta {
   return allMetaTypes.includes(meta?.type);
 }
 export function getOriginMeta(meta: any): IMeta | undefined {
   if (!checkMeta(meta)) return;
   return getOriginMeta(meta.data.from);
 }
+export function getMetaTrace(meta: IMeta): IMeta[] {
+  if (!checkMeta(meta)) return [];
+  return [meta, ...(meta.data.from ? getMetaTrace(meta.data.from) : [])];
+}
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/metaFields.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/schema/metaFields.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/plugins.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/schema/plugins.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import type { RefObject } from "react";
 import type { FlexProps } from "@chakra-ui/react";
 
 import type { INode, NodeType, PivotType } from "@carefree0910/core";
 import type { IResponse } from "@carefree0910/business";
 
 import type { IFieldDefinition, _IFieldDefinition } from "./metaFields";
-import type {
-  IPythonHttpFieldsPlugin,
-  IPythonHttpQAPlugin,
-  IPythonHttpTextAreaPlugin,
-} from "./_python";
+import type { IPythonFieldsPlugin, IPythonQAPlugin, IPythonTextAreaPlugin } from "./_python";
 
 // general
 
 export type NodeConstraints = NodeType | "none" | "anyNode" | "singleNode" | "multiNode";
 export interface IPositionInfo {
   w: number;
   h: number;
@@ -61,14 +57,15 @@
   field: string;
   definition: IFieldDefinition<T>;
 }
 
 // factory
 
 export const allAvailablePlugins = [
+  "meta",
   "settings",
   "project",
   "add",
   "arrange",
   "undo",
   "redo",
   "download",
@@ -78,20 +75,20 @@
   "email",
   "textEditor",
   "groupEditor",
   "multiEditor",
   "brush",
 ] as const;
 export const allAvailablePythonPlugins = [
-  "_python.httpTextArea",
-  "_python.httpQA",
-  "_python.httpFields",
+  "_python.textArea",
+  "_python.QA",
+  "_python.fields",
 ] as const;
-export type AvailablePlugins = typeof allAvailablePlugins[number];
-export type AvailablePythonPlugins = typeof allAvailablePythonPlugins[number];
+export type AvailablePlugins = (typeof allAvailablePlugins)[number];
+export type AvailablePythonPlugins = (typeof allAvailablePythonPlugins)[number];
 export type AvailablePluginsAndPythonPlugins = AvailablePlugins | AvailablePythonPlugins;
 
 export interface IPluginProps {
   // react plugins
   meta: IPlugin;
   settings: IPlugin;
   project: IPlugin;
@@ -105,17 +102,17 @@
   github: IPlugin;
   email: IPlugin;
   textEditor: IPlugin;
   groupEditor: IPlugin;
   multiEditor: IPlugin;
   brush: IPlugin;
   // python plugins
-  "_python.httpTextArea": IPythonHttpTextAreaPlugin;
-  "_python.httpQA": IPythonHttpQAPlugin;
-  "_python.httpFields": IPythonHttpFieldsPlugin;
+  "_python.textArea": IPythonTextAreaPlugin;
+  "_python.QA": IPythonQAPlugin;
+  "_python.fields": IPythonFieldsPlugin;
 }
 
 export interface IMakePlugin<T extends AvailablePluginsAndPythonPlugins> {
   type: T;
   props: Omit<IPluginProps[T], "containerRef" | "pluginInfo"> & {
     pluginInfo: Omit<IPluginProps[T]["pluginInfo"], "node" | "nodes">;
   };
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/requests.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/schema/requests.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/_python.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/_python.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/gridLines.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/gridLines.ts`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 }
 class GridLinesStore extends ABCStore<IGridLinesStore> implements IGridLinesStore {
   enable = true;
   lineWidth = 1;
   lineColor = "208,208,208";
   maxOpacity = 0.8;
   maxGridSize = 250;
-  span = 5;
+  span = 4;
   startSubGridsFraction = 0.45;
 
   constructor() {
     super();
     makeObservable(this, {
       enable: observable,
       lineWidth: observable,
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/hooks.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/hooks.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/meta.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/meta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/plugins.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/plugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/projects.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/theme.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/theme.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/ui.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/stores/ui.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/event.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/utils/event.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/misc.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/utils/misc.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/toast.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/src/utils/toast.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/tsconfig.json` & `carefree-drawboard-0.0.0a5/cfdraw/.web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/vite.config.ts` & `carefree-drawboard-0.0.0a5/cfdraw/.web/vite.config.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/yarn.lock` & `carefree-drawboard-0.0.0a5/cfdraw/.web/yarn.lock`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/app/app.py` & `carefree-drawboard-0.0.0a5/cfdraw/app/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,98 +1,106 @@
 from typing import Dict
 from typing import List
+from typing import AsyncGenerator
 from aiohttp import ClientSession
 from fastapi import FastAPI
+from contextlib import asynccontextmanager
 from cftool.misc import print_info
 from cftool.misc import random_hash
 from fastapi.middleware import cors
 
 from cfdraw import constants
 from cfdraw.config import get_config
 from cfdraw.app.schema import IApp
 from cfdraw.app.endpoints import *
-from cfdraw.schema.plugins import IPlugin
+from cfdraw.plugins.factory import Plugins
 from cfdraw.plugins.factory import PluginFactory
 
 
 async def ping() -> str:
     return "pong"
 
 
 class App(IApp):
     def __init__(self) -> None:
+        # FastAPI lifspan
+
+        @asynccontextmanager
+        async def lifespan(api: FastAPI) -> AsyncGenerator:
+            # startup
+
+            def info(msg: str) -> None:
+                print_info(msg)
+
+            self.hash = random_hash()
+            info(f"🚀 Starting Backend Server at {self.config.api_url} ...")
+            info("🔨 Compiling Plugins & Endpoints...")
+            for plugin_type in self.plugins.values():
+                plugin_type.hash = self.hash
+                plugin_type.http_session = self.http_session
+            for endpoint in self.endpoints:
+                await endpoint.on_startup()
+            upload_root_path = self.config.upload_root_path
+            info(f"🔔 Your files will be saved to '{upload_root_path}'")
+            info("🎉 Backend Server is Ready!")
+
+            yield
+
+            # shutdown
+
+            await self.http_session.close()
+            for plugin_type in self.plugins.values():
+                plugin_type.http_session = None
+            for endpoint in self.endpoints:
+                await endpoint.on_shutdown()
+            self.http_session = None
+
         # config
         self.config = get_config()
         # clients
         self.http_session = ClientSession()
+        # queue
+        self.request_queue = RequestQueue()
         # fastapi
-        self.api = FastAPI()
+        self.api = FastAPI(lifespan=lifespan)
         self.add_cors()
         self.add_default_endpoints()
-        self.add_events()
         self.endpoints: List[IEndpoint] = [
             UploadEndpoint(self),
             ProjectEndpoint(self),
-            PluginsEndpoint(self),
             WebsocketEndpoint(self),
         ]
+        if self.config.use_unified:
+            self.endpoints.append(AssetsEndpoint(self))
         for endpoint in self.endpoints:
             endpoint.register()
         self.hash = random_hash()
 
     def __str__(self) -> str:
         return "<App />"
 
     __repr__ = __str__
 
     @property
-    def plugins(self) -> Dict[str, IPlugin]:
+    def plugins(self) -> Plugins:
         return PluginFactory.plugins
 
     @property
-    def internal_plugins(self) -> Dict[str, IPlugin]:
+    def internal_plugins(self) -> Plugins:
         return PluginFactory.internal_plugins
 
     def add_cors(self) -> None:
         self.api.add_middleware(
             cors.CORSMiddleware,
             allow_credentials=True,
             allow_methods=["*"],
             allow_headers=["*"],
             allow_origins=["*"],
         )
 
-    def add_events(self) -> None:
-        @self.api.on_event("startup")
-        async def startup() -> None:
-            def info(msg: str) -> None:
-                if not self.config.use_tornado:
-                    print_info(msg)
-
-            self.hash = random_hash()
-            info(f"🚀 Starting Backend Server at {self.config.api_url} ...")
-            info("🔨 Compiling Plugins & Endpoints...")
-            for plugin in self.plugins.values():
-                plugin.hash = self.hash
-                plugin.http_session = self.http_session
-            for endpoint in self.endpoints:
-                await endpoint.on_startup()
-            upload_root_path = self.config.upload_root_path
-            info(f"🔔 Your files will be saved to '{upload_root_path}'")
-            info("🎉 Backend Server is Ready!")
-
-        @self.api.on_event("shutdown")
-        async def shutdown() -> None:
-            await self.http_session.close()
-            for plugin in self.plugins.values():
-                plugin.http_session = None
-            for endpoint in self.endpoints:
-                await endpoint.on_shutdown()
-            self.http_session = None
-
     def add_default_endpoints(self) -> None:
         self.api.get(str(constants.Endpoint.PING))(ping)
 
 
 __all__ = [
     "App",
 ]
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/plugins.py` & `carefree-drawboard-0.0.0a5/cfdraw/app/endpoints/upload.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,73 @@
-from cftool.misc import print_info
+from io import BytesIO
+from PIL import Image
+from typing import Optional
+from fastapi import File
+from fastapi import Response
+from fastapi import UploadFile
+from pydantic import BaseModel
 
+from cfdraw import constants
+from cfdraw.utils import server
 from cfdraw.app.schema import IApp
 from cfdraw.utils.server import get_err_msg
 from cfdraw.utils.server import get_responses
-from cfdraw.schema.plugins import IPluginRequest
-from cfdraw.schema.plugins import IPluginResponse
-from cfdraw.plugins.base import IHttpPlugin
-from cfdraw.plugins.base import ISocketPlugin
+from cfdraw.utils.server import get_image_response_kwargs
 from cfdraw.app.endpoints.base import IEndpoint
 
 
-def add_plugins(app: IApp) -> None:
-    for identifier, plugin in app.plugins.items():
-        if not isinstance(plugin, IHttpPlugin):
-            continue
-        endpoint = f"/{identifier}"
-        if not app.config.prod:
-            print_info(f"registering endpoint '{endpoint}'")
-
-        def _register(_id: str, _p: IHttpPlugin) -> None:
-            @app.api.post(
-                endpoint,
-                name=endpoint[1:].replace("/", "_"),
-                responses=get_responses(IPluginResponse),
-            )
-            async def fn(data: IPluginRequest) -> IPluginResponse:
-                if _p.hash_identifier(_id) != data.identifier:
-                    return IPluginResponse(
-                        success=False,
-                        message=(
-                            f"internal error occurred: identifier mismatch, "
-                            f"current hash is {_p.hash_identifier(_id)} "
-                            f"but incoming identifier is {data.identifier}"
-                        ),
-                        data={},
-                    )
-                try:
-                    return await _p(data)
-                except Exception as err:
-                    err_msg = get_err_msg(err)
-                    return IPluginResponse(success=False, message=err_msg, data={})
+class ImageDataModel(BaseModel):
+    w: int
+    h: int
+    url: str
+
+
+class UploadImageResponse(BaseModel):
+    success: bool
+    message: str
+    data: Optional[ImageDataModel]
+
+
+class FetchImageModel(BaseModel):
+    url: str
+    jpeg: bool
+
+
+def add_upload_image(app: IApp) -> None:
+    @app.api.post("/upload_image", responses=get_responses(UploadImageResponse))
+    def upload_image(image: UploadFile = File(...)) -> UploadImageResponse:
+        try:
+            contents = image.file.read()
+            loaded_image = Image.open(BytesIO(contents))
+            res = server.upload_image(loaded_image)
+        except Exception as err:
+            err_msg = get_err_msg(err)
+            return UploadImageResponse(success=False, message=err_msg, data=None)
+        finally:
+            image.file.close()
+        return UploadImageResponse(
+            success=True,
+            message="",
+            data=ImageDataModel(**res),
+        )
+
+    @app.api.post("/fetch_image", **get_image_response_kwargs())
+    async def fetch_image(data: FetchImageModel) -> Response:
+        file = data.url.split(constants.UPLOAD_IMAGE_FOLDER_NAME)[1][1:]  # remove '/'
+        return server.get_image_response(file, data.jpeg)
+
+    @app.api.get(
+        f"/{constants.UPLOAD_IMAGE_FOLDER_NAME}/{{file}}/",
+        **get_image_response_kwargs(),
+    )
+    async def get_image(file: str, jpeg: bool = False) -> Response:
+        return server.get_image_response(file, jpeg)
 
-        _register(identifier, plugin)
 
-
-class PluginsEndpoint(IEndpoint):
+class UploadEndpoint(IEndpoint):
     def register(self) -> None:
-        add_plugins(self.app)
+        add_upload_image(self.app)
 
 
 __all__ = [
-    "PluginsEndpoint",
+    "UploadEndpoint",
 ]
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/project.py` & `carefree-drawboard-0.0.0a5/cfdraw/app/endpoints/project.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/upload.py` & `carefree-drawboard-0.0.0a5/cfdraw/plugins/middlewares/fields.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,30 @@
-from io import BytesIO
-from PIL import Image
-from typing import Optional
-from fastapi import File
-from fastapi import Response
-from fastapi import UploadFile
-from pydantic import BaseModel
-
-from cfdraw import constants
-from cfdraw.utils import server
-from cfdraw.app.schema import IApp
-from cfdraw.utils.server import get_err_msg
-from cfdraw.utils.server import get_responses
-from cfdraw.utils.server import get_image_response_kwargs
-from cfdraw.app.endpoints.base import IEndpoint
-
-
-class ImageDataModel(BaseModel):
-    w: int
-    h: int
-    url: str
-
-
-class UploadImageResponse(BaseModel):
-    success: bool
-    message: str
-    data: Optional[ImageDataModel]
-
-
-def add_upload_image(app: IApp) -> None:
-    @app.api.post("/upload_image", responses=get_responses(UploadImageResponse))
-    def upload_image(image: UploadFile = File(...)) -> UploadImageResponse:
-        try:
-            contents = image.file.read()
-            loaded_image = Image.open(BytesIO(contents))
-            res = server.upload_image(loaded_image)
-        except Exception as err:
-            err_msg = get_err_msg(err)
-            return UploadImageResponse(success=False, message=err_msg, data=None)
-        finally:
-            image.file.close()
-        return UploadImageResponse(
-            success=True,
-            message="",
-            data=ImageDataModel(**res),
-        )
-
-    @app.api.get(
-        f"/{constants.UPLOAD_IMAGE_FOLDER_NAME}/{{file}}/",
-        **get_image_response_kwargs(),
-    )
-    async def fetch_image(file: str, jpeg: bool = False) -> Response:
-        return server.get_image_response(file, jpeg)
-
-
-class UploadEndpoint(IEndpoint):
-    def register(self) -> None:
-        add_upload_image(self.app)
+from typing import List
+from typing import Union
+from PIL.Image import Image
+
+from cfdraw.utils.server import upload_image
+from cfdraw.schema.plugins import PluginType
+from cfdraw.schema.plugins import IMiddleWare
+from cfdraw.schema.plugins import ISocketMessage
+
+
+class FieldsMiddleWare(IMiddleWare):
+    @property
+    def subscriptions(self) -> List[PluginType]:
+        return [PluginType.FIELDS]
+
+    async def process(
+        self,
+        response: Union[str, List[str], Image, List[Image]],
+    ) -> ISocketMessage:
+        if not isinstance(response, list):
+            response = [response]
+        if isinstance(response[0], str):
+            return self.make_success(dict(type="text", value=response))
+        urls = [upload_image(image) for image in response]
+        return self.make_success(dict(type="image", value=urls))
 
 
 __all__ = [
-    "UploadEndpoint",
+    "FieldsMiddleWare",
 ]
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/cli.py` & `carefree-drawboard-0.0.0a5/cfdraw/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,55 +23,53 @@
     no_frontend: bool = typer.Option(False, help="Whether not to run the frontend."),
     no_backend: bool = typer.Option(False, help="Whether not to run the backend."),
     log_level: constants.LogLevel = typer.Option(
         constants.LogLevel.ERROR,
         help="The log level to use.",
     ),
     prod: bool = typer.Option(False, help="Whether to run in production mode."),
-    tornado: bool = typer.Option(False, help="Whether use tornado to unify servers."),
+    unified: bool = typer.Option(False, help="Whether use unified servers."),
+    host: bool = typer.Option(False, help="Whether use `--host` in development mode."),
 ) -> None:
     sys.path.insert(0, os.getcwd())
-    if tornado:
+    if unified:
         if not prod:
             console.print(
-                "[bold orange1]Tornado is only available in production mode, "
+                "[bold orange1]`--unified` is only available in production mode, "
                 "so `--prod` flag will be forced."
             )
             prod = True
     constants.set_env(constants.Env.PROD if prod else constants.Env.DEV)
-    constants.set_tornado(tornado)
+    constants.set_unified(unified)
     # fetch config
     config = get_config()
     # fetch module
     if module is None:
         module = constants.DEFAULT_MODULE
     if module.endswith(".py"):
         module = module[:-3]
     path_prefix = f".{os.path.sep}"
     if module.startswith(path_prefix):
         module = module[len(path_prefix) :]
     console.rule(f"[bold green]Running {module}")
     # execute
     frontend_port = config.frontend_port
     backend_port = config.backend_port
-    tornado_port = config.tornado_port
     if not no_frontend and processes.is_process_on_port(frontend_port):
         frontend_port = processes.change_or_terminate_port(frontend_port, "frontend")
     if not no_backend and processes.is_process_on_port(backend_port):
         backend_port = processes.change_or_terminate_port(backend_port, "backend")
-    if tornado and not no_backend and processes.is_process_on_port(tornado_port):
-        tornado_port = processes.change_or_terminate_port(tornado_port, "tornado")
     config.frontend_port = frontend_port
     config.backend_port = backend_port
-    config.tornado_port = tornado_port
     if not prod:
-        frontend_fn, backend_fn = exec.run_frontend, exec.run_backend
+        frontend_fn = lambda: exec.run_frontend(host)
+        backend_fn = exec.run_backend
     else:
         frontend_fn = exec.run_frontend_prod
-        backend_fn = exec.run_tornado if tornado else exec.run_backend
+        backend_fn = exec.run_backend_prod  # type: ignore
     try:
         if not no_frontend:
             frontend_fn()
         if not no_backend:
             backend_fn(module, log_level=log_level)
     finally:
         console.rule("[bold]Shutting down")
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/config.py` & `carefree-drawboard-0.0.0a5/cfdraw/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,46 +13,49 @@
 class Config:
     # app
     entry: str = constants.DEFAULT_ENTRY
     # frontend
     frontend_port: str = constants.FRONTEND_PORT
     # api
     backend_port: str = constants.BACKEND_PORT
-    tornado_port: str = constants.TORNADO_PORT
     backend_hosting_url: Optional[str] = None  # this must be provided for hosting
     # upload
     upload_root: str = str(constants.UPLOAD_ROOT)
     # misc
     use_react_strict_mode: bool = False
 
     @property
     def prod(self) -> bool:
         return constants.get_env() == constants.Env.PROD
 
     @property
-    def use_tornado(self) -> bool:
-        return constants.use_tornado()
+    def use_unified(self) -> bool:
+        return constants.use_unified()
 
     @property
     def api_port(self) -> str:
-        return self.tornado_port if self.use_tornado else self.backend_port
+        return self.backend_port
 
     @property
     def api_url(self) -> str:
         if self.backend_hosting_url is not None:
             api_url = self.backend_hosting_url
         else:
             env_api_url = os.environ.get(constants.API_URL_KEY)
             if env_api_url is not None:
                 api_url = env_api_url
             else:
                 api_url = f"http://localhost:{self.api_port}"
         return api_url.rstrip("/").rstrip("\\")
 
     @property
+    def frontend_url(self) -> str:
+        return f"http://localhost:{self.frontend_port}"
+
+    @property
     def upload_root_path(self) -> Path:
         return Path(self.upload_root).absolute()
 
     @property
     def upload_image_folder(self) -> Path:
         folder = self.upload_root_path / constants.UPLOAD_IMAGE_FOLDER_NAME
         folder.mkdir(parents=True, exist_ok=True)
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/constants.py` & `carefree-drawboard-0.0.0a5/cfdraw/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 # frontend
 FRONTEND_PORT = "5123"
 
 # api
 ERR_CODE = 406
 BACKEND_PORT = "8123"
-TORNADO_PORT = "8234"
 DEV_BACKEND_HOST = "0.0.0.0"
 API_URL_KEY = "CFDRAW_API_URL"
 
 
 class Endpoint(Enum):
     PING = "ping"
     WEBSOCKET = "ws"
@@ -29,15 +28,15 @@
         return f"/{self.value}"
 
     __repr__ = __str__
 
 
 # misc
 ENV_KEY = "CFDRAW_ENV"
-TORNADO_KEY = "CFDRAW_TORNADO"
+UNIFIED_KEY = "CFDRAW_UNIFIED"
 
 
 class Env(str, Enum):
     DEV = "development"
     PROD = "production"
 
 
@@ -45,20 +44,20 @@
     return os.environ.get(ENV_KEY, Env.DEV)  # type: ignore
 
 
 def set_env(env: Env) -> None:
     os.environ[ENV_KEY] = env.value
 
 
-def use_tornado() -> bool:
-    return os.environ.get(TORNADO_KEY, None) == "enabled"
+def use_unified() -> bool:
+    return os.environ.get(UNIFIED_KEY, None) == "enabled"
 
 
-def set_tornado(enable: bool) -> None:
-    os.environ[TORNADO_KEY] = "enabled" if enable else "disabled"
+def set_unified(enable: bool) -> None:
+    os.environ[UNIFIED_KEY] = "enabled" if enable else "disabled"
 
 
 class LogLevel(str, Enum):
     DEBUG = "debug"
     INFO = "info"
     WARNING = "warning"
     ERROR = "error"
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/parsers/chakra.py` & `carefree-drawboard-0.0.0a5/cfdraw/parsers/chakra.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/parsers/noli.py` & `carefree-drawboard-0.0.0a5/cfdraw/parsers/noli.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Dict
 from typing import List
 from typing import Tuple
 from typing import Union
 from typing import Optional
 from typing import Generator
 from pydantic import BaseModel
+from dataclasses import dataclass
 
 
 class PivotType(str, Enum):
     LT = "lt"
     TOP = "top"
     RT = "rt"
     LEFT = "left"
@@ -45,22 +46,40 @@
     SINGLE_NODE = "singleNode"
     MULTI_NODE = "multiNode"
 
 
 # data structures
 
 
+@dataclass
+class Point:
+    x: float
+    y: float
+
+    @property
+    def tuple(self) -> Tuple[float, float]:
+        return self.x, self.y
+
+    def __rmatmul__(self, other: "Matrix2D") -> "Point":
+        a, b, c, d, e, f = [pair[1] for pair in other]
+        x, y = self.x, self.y
+        return Point(x=a * x + c * y + e, y=b * x + d * y + f)
+
+
 class Matrix2D(BaseModel):
     a: float
     b: float
     c: float
     d: float
     e: float
     f: float
 
+    def __matmul__(self, other: Point) -> Point:
+        return other.__rmatmul__(self)
+
     @property
     def w(self) -> float:
         return math.sqrt(self.a**2 + self.b**2)
 
     @property
     def h(self) -> float:
         return (self.a * self.d - self.b * self.c) / max(self.w, 1.0e-12)
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/plugins/base.py` & `carefree-drawboard-0.0.0a5/cfdraw/plugins/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 from io import BytesIO
 from abc import abstractmethod
 from abc import ABCMeta
 from PIL import Image
 from typing import Any
 from typing import Dict
 from typing import List
-from typing import Callable
-from typing import Coroutine
 
 from cfdraw import constants
 from cfdraw.utils import server
+from cfdraw.utils.misc import deprecated
 from cfdraw.schema.plugins import *
 from cfdraw.plugins.middlewares import *
 from cfdraw.parsers.noli import SingleNodeType
 from cfdraw.parsers.noli import NodeConstraints
 from cfdraw.parsers.chakra import IChakra
 
 
-class IBasePlugin(IPlugin, metaclass=ABCMeta):
+class ISocketPlugin(IPlugin, metaclass=ABCMeta):
     @abstractmethod
-    async def process(self, data: IPluginRequest) -> Any:
+    async def process(self, data: ISocketRequest) -> Any:
         pass
 
     @property
     def middlewares(self) -> List[IMiddleWare]:
-        return []
+        common_middlewares: List[IMiddleWare] = [
+            TextAreaMiddleWare(self.send_text),
+            FieldsMiddleWare(self.send_text),
+            TimerMiddleWare(self.send_text),
+        ]
+        send_message_middleware = SendSocketMessageMiddleWare(self.send_text)
+        return common_middlewares + [send_message_middleware]
 
-    async def __call__(self, data: IPluginRequest) -> IPluginResponse:
+    async def __call__(self, data: ISocketRequest) -> ISocketMessage:
         middlewares = self.middlewares
         for middleware in middlewares:
             await middleware.before(data)
         response = await self.process(data)
         for middleware in middlewares:
             response = await middleware(self, response)
         return response
@@ -77,60 +82,73 @@
         if src.startswith("http://") and constants.UPLOAD_IMAGE_FOLDER_NAME in src:
             file = src.split(constants.UPLOAD_IMAGE_FOLDER_NAME)[1][1:]  # remove '/'
             return server.get_image(file)
         async with self.http_session.get(src) as res:
             return Image.open(BytesIO(await res.read()))
 
 
-class IHttpPlugin(IBasePlugin, metaclass=ABCMeta):
-    @property
-    def middlewares(self) -> List[IMiddleWare]:
-        return [TextAreaMiddleWare(), FieldsMiddleWare(), TimerMiddleWare()]
-
-
-class ISocketPlugin(IBasePlugin, metaclass=ABCMeta):
-    send_text: Callable[[ISocketMessage], Coroutine[Any, Any, None]]
-
-    @abstractmethod
-    async def process(self, data: IPluginRequest) -> ISocketMessage:
-        pass
-
-
 class IInternalSocketPlugin(ISocketPlugin, metaclass=ABCMeta):
     @property
     def type(self) -> PluginType:
         return PluginType._INTERNAL
 
     @property
     def settings(self) -> IPluginSettings:
         return IPluginSettings(w=1, h=1, nodeConstraint=NodeConstraints.NONE)
 
 
 # bindings
 
 
-class IHttpTextAreaPlugin(IHttpPlugin):
+class ITextAreaPlugin(ISocketPlugin):
     @property
     def type(self) -> PluginType:
-        return PluginType.HTTP_TEXT_AREA
+        return PluginType.TEXT_AREA
 
 
-class IHttpQAPlugin(IHttpPlugin):
+class IQAPlugin(ISocketPlugin):
     @property
     def type(self) -> PluginType:
-        return PluginType.HTTP_QA
+        return PluginType.QA
 
 
-class IHttpFieldsPlugin(IHttpPlugin):
+class IFieldsPlugin(ISocketPlugin):
     @property
     def type(self) -> PluginType:
-        return PluginType.HTTP_FIELDS
+        return PluginType.FIELDS
+
+
+## deprecated
+
+
+@deprecated("please use `ISocketPlugin` instead")
+class IHttpPlugin(ISocketPlugin, metaclass=ABCMeta):
+    pass
+
+
+@deprecated("please use `ITextAreaPlugin` instead")
+class IHttpTextAreaPlugin(ITextAreaPlugin):
+    pass
+
+
+@deprecated("please use `IQAPlugin` instead")
+class IHttpQAPlugin(IQAPlugin):
+    pass
+
+
+@deprecated("please use `IFieldsPlugin` instead")
+class IHttpFieldsPlugin(IFieldsPlugin):
+    pass
 
 
 __all__ = [
-    "IHttpPlugin",
     "ISocketPlugin",
     "IInternalSocketPlugin",
+    "ITextAreaPlugin",
+    "IQAPlugin",
+    "IFieldsPlugin",
+    # deprecated
+    "IHttpPlugin",
     "IHttpTextAreaPlugin",
     "IHttpQAPlugin",
     "IHttpFieldsPlugin",
 ]
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/plugins/factory.py` & `carefree-drawboard-0.0.0a5/cfdraw/plugins/factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from typing import Dict
 from typing import Type
 from typing import Callable
 from typing import NamedTuple
 
+from cfdraw.utils.data_structures import Types
 from cfdraw.schema.plugins import IPlugin
 from cfdraw.schema.plugins import IPluginSettings
 
+
 TPlugin = Type[IPlugin]
 
 
+class Plugins(Types[IPlugin]):
+    pass
+
+
 class PluginInfo(NamedTuple):
     name: str
     settings: IPluginSettings
     plugin_type: Type[IPlugin]
 
 
 class PluginFactory:
@@ -22,31 +28,27 @@
     > `recorded` stores all plugins that are recorded, and can be accessed via `available`
     >> You can record a plugin by using the `record` decorator
     >> After which you can decide which plugins to use with the `register` method!
     > Notice that we don't need to guarantee that the plugin's name is identical to the plugin's identifier
     >> `plugins` use 'identifier' as the key, and `recorded` use 'name' as the key
     """
 
-    plugins: Dict[str, IPlugin] = {}
-    recorded: Dict[str, IPlugin] = {}
-    internal_plugins: Dict[str, IPlugin] = {}
+    plugins = Plugins()
+    recorded = Plugins()
+    internal_plugins = Plugins()
 
     @classmethod
-    def _register(
-        cls,
-        d: Dict[str, IPlugin],
-        identifier: str,
-    ) -> Callable[[TPlugin], TPlugin]:
+    def _register(cls, d: Plugins, identifier: str) -> Callable[[TPlugin], TPlugin]:
         if identifier in d:
             raise ValueError(f"plugin {identifier} already exists")
 
-        def _fn(plugin: TPlugin) -> TPlugin:
-            plugin.identifier = identifier
-            d[identifier] = plugin()
-            return plugin
+        def _fn(plugin_type: TPlugin) -> TPlugin:
+            plugin_type.identifier = identifier
+            d[identifier] = plugin_type
+            return plugin_type
 
         return _fn
 
     @classmethod
     def register(cls, identifier: str) -> Callable[[TPlugin], TPlugin]:
         return cls._register(cls.plugins, identifier)
 
@@ -55,25 +57,26 @@
         return cls._register(cls.internal_plugins, identifier)
 
     @classmethod
     def record(cls, name: str) -> Callable[[TPlugin], TPlugin]:
         if name in cls.recorded:
             raise ValueError(f"plugin {name} already recorded")
 
-        def _record(plugin: TPlugin) -> TPlugin:
-            cls.recorded[name] = plugin()
-            return plugin
+        def _record(plugin_type: TPlugin) -> TPlugin:
+            cls.recorded[name] = plugin_type
+            return plugin_type
 
         return _record
 
     @classmethod
     def available(cls) -> Dict[str, PluginInfo]:
         return {
-            name: PluginInfo(name, plugin.settings, plugin.__class__)
-            for name, plugin in cls.recorded.items()
+            name: PluginInfo(name, plugin_type().settings, plugin_type)
+            for name, plugin_type in cls.recorded.items()
         }
 
 
 __all__ = [
+    "Plugins",
     "PluginInfo",
     "PluginFactory",
 ]
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/plugins/sync.py` & `carefree-drawboard-0.0.0a5/cfdraw/plugins/sync.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,31 +3,26 @@
 from cfdraw.schema.plugins import *
 from cfdraw.plugins.base import *
 from cfdraw.plugins.factory import PluginFactory
 
 
 @PluginFactory.register_internal("sync")
 class SyncSocketPlugin(IInternalSocketPlugin):
-    async def process(self, data: IPluginRequest) -> ISocketMessage:
+    async def process(self, data: ISocketRequest) -> ISocketMessage:
         config = get_config()
-        return ISocketMessage(
-            success=True,
-            message="",
-            data=ISocketData(
-                status=SocketStatus.FINISHED,
-                pending=0,
-                data=dict(
-                    pluginSettings=[
-                        plugin.to_plugin_settings()
-                        for plugin in PluginFactory.plugins.values()
-                    ],
-                    globalSettings=dict(
-                        useStrictMode=config.use_react_strict_mode,
-                        sockenEndpoint=str(constants.Endpoint.WEBSOCKET),
-                    ),
+        return ISocketMessage.make_success(
+            data.hash,
+            dict(
+                pluginSettings=[
+                    plugin_type().to_plugin_settings()
+                    for plugin_type in PluginFactory.plugins.values()
+                ],
+                globalSettings=dict(
+                    useStrictMode=config.use_react_strict_mode,
+                    sockenEndpoint=str(constants.Endpoint.WEBSOCKET),
                 ),
             ),
         )
 
 
 __all__ = [
     "SyncSocketPlugin",
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/schema/fields.py` & `carefree-drawboard-0.0.0a5/cfdraw/schema/fields.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/schema/plugins.py` & `carefree-drawboard-0.0.0a5/cfdraw/schema/plugins.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 from abc import abstractmethod
 from abc import ABC
+from abc import ABCMeta
 from PIL import Image
 from enum import Enum
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import TypeVar
+from typing import Callable
 from typing import Optional
+from typing import Coroutine
 from aiohttp import ClientSession
 from pydantic import Field
 from pydantic import BaseModel
 
+from cfdraw.utils.misc import deprecated
 from cfdraw.schema.fields import IFieldDefinition
 from cfdraw.parsers.noli import Matrix2D
 from cfdraw.parsers.noli import INodeType
 from cfdraw.parsers.noli import PivotType
 from cfdraw.parsers.noli import NodeConstraints
 from cfdraw.parsers.chakra import IChakra
 from cfdraw.parsers.chakra import TextAlign
 
 
 TPluginModel = TypeVar("TPluginModel")
+ISendSocketText = Callable[["ISocketMessage"], Coroutine[Any, Any, None]]
 
 
 class PluginType(str, Enum):
-    HTTP_TEXT_AREA = "httpTextArea"
-    HTTP_QA = "httpQA"
-    HTTP_FIELDS = "httpFields"
+    # These types should align with the `allAvailablePythonPlugins` locates at
+    # `cfdraw/.web/src/schema/plugins.ts` (without the `_python.` prefix)
+    TEXT_AREA = "textArea"
+    QA = "QA"
+    FIELDS = "fields"
     # this type of plugins will not be rendered on the drawboard 🎨
     _INTERNAL = "_internal"
 
 
 # general
 
 
@@ -46,15 +53,15 @@
         None,
         description="Whether close the expanded panel when the submit button is clicked",
     )
     toastOnSubmit: Optional[bool] = Field(
         None,
         description="Whether trigger a toast message when the submit button is clicked",
     )
-    submitToastMessage: Optional[str] = Field(
+    toastMessageOnSubmit: Optional[str] = Field(
         None,
         description="The message of the toast, only take effect when `toastOnSubmit` is `True`",
     )
 
 
 class IPluginSettings(IChakra):
     # required fields
@@ -146,17 +153,19 @@
         description=(
             "Will be a list of `INodeData` if and only if "
             "the node is a `Group` (i.e. `type` == 'group')"
         ),
     )
 
 
-class IPluginRequest(BaseModel):
-    """This should align with `IPythonRequest` at `src/schema/_python.ts`"""
+class ISocketRequest(BaseModel):
+    """This should align with `IPythonSocketRequest` at `src/schema/_python.ts`"""
 
+    hash: str = Field(..., description="The hash of the request")
+    userId: str = Field(..., description="The id of the user")
     identifier: str = Field(..., description="The identifier of the plugin")
     nodeData: INodeData = Field(
         ...,
         description="""
 Data extracted from `node`.
 > If multiple nodes are selected, this field will be empty and please use `nodeDataList` instead.
 """,
@@ -168,146 +177,220 @@
 > If only one node is selected, this field will be empty and please use `nodeData` instead.
 """,
     )
     extraData: Dict[str, Any] = Field(..., description="Extra data of each plugin")
     isInternal: bool = Field(False, description="Whether the request is internal")
 
 
-class IPluginResponse(BaseModel):
-    """This should align with `IPythonResponse` at `src/schema/_python.ts`"""
-
-    success: bool = Field(..., description="Whether returned successfully")
-    message: str = Field(..., description="The message of the response")
-    data: Dict[str, Any] = Field(..., description="The data of the response")
-
-
 class SocketStatus(str, Enum):
     """This should align with `PythonSocketStatus` at `src/schema/_python.ts`"""
 
     PENDING = "pending"
     WORKING = "working"
     FINISHED = "finished"
     EXCEPTION = "exception"
 
 
-class ISocketData(BaseModel):
-    """This should align with `IPythonSocketData` at `src/schema/_python.ts`"""
+class ISocketIntermediate(BaseModel):
+    """This should align with `IPythonSocketIntermediate` at `src/schema/_python.ts`"""
+
+    imageList: Optional[List[str]] = Field(
+        None,
+        description="Intermediate images, if any",
+    )
+    textList: Optional[List[str]] = Field(
+        None,
+        description="Intermediate texts, if any",
+    )
+
+
+class ISocketResponse(BaseModel):
+    """This should align with `IPythonSocketResponse` at `src/schema/_python.ts`"""
+
+    progress: Optional[float] = Field(
+        None,
+        ge=0.0,
+        le=1.0,
+        description="Progress of current task, if any",
+    )
+    intermediate: Optional[ISocketIntermediate] = Field(
+        None,
+        description="Intermediate responses, if any",
+    )
+    final: Optional[Dict[str, Any]] = Field(None, description="Final response, if any")
+
+
+class ISocketMessage(BaseModel):
+    """This should align with `IPythonSocketMessage` at `src/schema/_python.ts`"""
 
+    hash: str = Field(..., description="Hash of the current task")
     status: SocketStatus = Field(..., description="Status of the current task")
+    total: int = Field(..., description="Number of tasks")
     pending: int = Field(..., description="Number of pending tasks")
-    data: Optional[Dict[str, Any]] = Field(None, description="Response data, if any")
+    message: str = Field(..., description="Message of the current status")
+    data: ISocketResponse = Field(ISocketResponse(), description="Response data")
 
-
-class ISocketMessage(IPluginResponse):
-    data: ISocketData = Field(..., description="Socket data of the current task")
+    @classmethod
+    def make_success(cls, hash: str, final: Dict[str, Any]) -> "ISocketMessage":
+        return cls(
+            hash=hash,
+            status=SocketStatus.FINISHED,
+            total=0,
+            pending=0,
+            message="",
+            data=ISocketResponse(final=final),
+        )
+
+    @classmethod
+    def make_exception(cls, hash: str, message: str) -> "ISocketMessage":
+        return cls(
+            hash=hash,
+            status=SocketStatus.EXCEPTION,
+            total=0,
+            pending=0,
+            message=message,
+        )
 
 
 # plugin interface
 
 
 class IPlugin(ABC):
     hash: str
     identifier: str
     http_session: ClientSession
+    send_text: ISendSocketText
 
     @property
     @abstractmethod
     def type(self) -> PluginType:
         pass
 
     @property
     @abstractmethod
     def settings(self) -> IPluginSettings:
         pass
 
     @abstractmethod
-    async def __call__(self, data: IPluginRequest) -> IPluginResponse:
+    async def __call__(self, data: ISocketRequest) -> ISocketMessage:
         pass
 
     @abstractmethod
     def to_plugin_settings(self) -> Dict[str, Any]:
         pass
 
     @abstractmethod
     async def load_image(self, src: str) -> Image.Image:
         pass
 
 
 class IMiddleWare(ABC):
+    hash: str
+    send_text: ISendSocketText
+
     # abstract
 
     @property
     @abstractmethod
     def subscriptions(self) -> List[PluginType]:
         pass
 
     @abstractmethod
-    async def process(self, response: Any) -> IPluginResponse:
-        pass
+    async def process(self, response: Any) -> ISocketMessage:
+        """
+        If `can_handle_message` is `False`, the `response` here could be anything except
+        `ISocketMessage`, because in this case if `response` is already an `ISocketMessage`,
+        it will be returned directly in the `__call__` method.
+        """
 
     # optional callbacks
 
-    async def before(self, request: IPluginRequest) -> None:
-        pass
+    @property
+    def can_handle_message(self) -> bool:
+        return False
+
+    async def before(self, request: ISocketRequest) -> None:
+        self.hash = request.hash
 
     # api
 
-    async def __call__(self, plugin: IPlugin, response: Any) -> IPluginResponse:
+    def __init__(self, send_text: ISendSocketText) -> None:
+        self.send_text = send_text
+
+    async def __call__(self, plugin: IPlugin, response: Any) -> ISocketMessage:
         if plugin.type not in self.subscriptions:
             return response
+        if isinstance(response, ISocketMessage) and not self.can_handle_message:
+            return response
         return await self.process(response)
 
+    def make_success(self, final: Dict[str, Any]) -> ISocketMessage:
+        return ISocketMessage.make_success(self.hash, final)
+
 
 # (react) bindings
 
-## (http) text area
+
+class IFieldsPluginInfo(IPluginInfo):
+    header: Optional[str] = Field(None, description="Header of the plugin")
+    definitions: Dict[str, IFieldDefinition] = Field(
+        ...,
+        description="Field definitions",
+    )
+    numColumns: Optional[int] = Field(None, description="Number of columns")
+
+
+## text area
 
 
-class IHttpTextAreaPluginInfo(IPluginInfo):
+class ITextAreaPluginInfo(IPluginInfo):
     noLoading: bool = Field(
         False, description="Whether to show the 'Loading...' text or not"
     )
     textAlign: Optional[TextAlign] = Field(None, description="Text align")
 
 
-## (http) qa
+## qa
 
 
-class IHttpQAPluginInfo(IPluginInfo):
+class IQAPluginInfo(IPluginInfo):
     initialText: str = Field(
         ...,
         description="The initial text to be displayed in the text area",
     )
 
 
-## (http) fields
+## deprecated
 
 
-class IHttpFieldsPluginInfo(IPluginInfo):
-    header: Optional[str] = Field(None, description="Header of the plugin")
-    definitions: Dict[str, IFieldDefinition] = Field(
-        ...,
-        description="Field definitions",
-    )
-    numColumns: Optional[int] = Field(None, description="Number of columns")
+@deprecated("please use `ITextAreaPluginInfo` instead")
+class IHttpTextAreaPluginInfo(ITextAreaPluginInfo):
+    pass
+
+
+@deprecated("please use `IQAPluginInfo` instead")
+class IHttpQAPluginInfo(IQAPluginInfo):
+    pass
 
 
 __all__ = [
+    "ISendSocketText",
     "PluginType",
     # general
     "IPluginInfo",
     "IPluginSettings",
     # web
     "INodeData",
-    "IPluginRequest",
-    "IPluginResponse",
+    "ISocketRequest",
     "SocketStatus",
-    "ISocketData",
     "ISocketMessage",
     # plugin interface
     "IPlugin",
     "IMiddleWare",
+    "IFieldsPluginInfo",
     # bindings
+    "ITextAreaPluginInfo",
+    "IQAPluginInfo",
+    # deprecated
     "IHttpTextAreaPluginInfo",
     "IHttpQAPluginInfo",
-    "IHttpFieldsPluginInfo",
 ]
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/utils/cache.py` & `carefree-drawboard-0.0.0a5/cfdraw/utils/cache.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/utils/console.py` & `carefree-drawboard-0.0.0a5/cfdraw/utils/console.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/utils/exec.py` & `carefree-drawboard-0.0.0a5/cfdraw/utils/exec.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,45 +4,45 @@
 
 from cftool.misc import print_info
 
 from cfdraw import constants
 from cfdraw.utils import console
 from cfdraw.utils import prerequisites
 from cfdraw.config import get_config
-from cfdraw.config import Config
-from cfdraw.server import launch_server
 
 
 def setup_frontend() -> None:
     config = get_config()
     prerequisites.install_frontend_packages()
     console.rule("[bold green]Launching App")
     os.environ["CFDRAW_FE_PORT"] = config.frontend_port
     os.environ["CFDRAW_BE_PORT"] = config.api_port
     if config.backend_hosting_url is not None:
         os.environ[constants.API_URL_KEY] = config.api_url
 
 
-def run_frontend() -> None:
+def run_frontend(host: bool) -> None:
     setup_frontend()
+    cmd = [prerequisites.get_yarn(), "dev", "--force"]
+    if host:
+        cmd.append("--host")
     subprocess.Popen(
-        [prerequisites.get_yarn(), "dev", "--force"],
+        cmd,
         cwd=constants.WEB_ROOT,
         env=os.environ,
         stdout=subprocess.DEVNULL,
         stderr=subprocess.STDOUT,
     )
-    frontend_url = f"http://localhost:{get_config().frontend_port}"
-    print_info(f"👌 Your app will be ready at {frontend_url} soon...")
+    print_info(f"👌 Your app will be ready at {get_config().frontend_url} soon...")
 
 
 def run_frontend_prod() -> None:
     setup_frontend()
     config = get_config()
-    if config.use_tornado:
+    if config.use_unified:
         print_info(f"👀 Your app codes are being compiled, please wait for a while...")
         subprocess.run(
             [prerequisites.get_yarn(), "build"],
             cwd=constants.WEB_ROOT,
             env=os.environ,
         )
     else:
@@ -53,34 +53,33 @@
         )
         print_info(
             f"👀 Your app codes are being compiled, "
             "please wait until a bunch of urls appear..."
         )
 
 
-def run_backend(module: str, *, log_level: constants.LogLevel) -> None:
-    console.rule("[bold green]Launching Backend")
+def run_backend(
+    module: str,
+    *,
+    log_level: constants.LogLevel,
+    verbose: bool = True,
+) -> None:
+    if verbose:
+        console.rule("[bold green]Launching Backend")
     config = get_config()
     # I'm not familiar with production stuffs of `uvicorn`, so currently
     # only the `reload` flag is different.
     uvicorn.run(
         f"{module}:{config.entry}.{constants.API_VAR}",
         host=constants.DEV_BACKEND_HOST,
         port=int(config.backend_port),
         log_level=log_level,
         reload=not config.prod,
     )
 
 
-def run_tornado(module: str, *, log_level: constants.LogLevel) -> None:
-    def before_launch(config: Config) -> None:
-        cmd = [
-            "uvicorn",
-            f"{module}:{config.entry}.{constants.API_VAR}",
-            f"--host={constants.DEV_BACKEND_HOST}",
-            f"--port={config.backend_port}",
-            f"--log-level={log_level}",
-        ]
-        subprocess.Popen(cmd)
-
-    console.rule("[bold green]Launching Tornado Backend")
-    launch_server(before_launch)
+def run_backend_prod(module: str, *, log_level: constants.LogLevel) -> None:
+    console.rule("[bold green]Launching Production Backend")
+    config = get_config()
+    if config.use_unified:
+        print_info(f"👌 Your app will be ready at {config.api_url} soon...")
+    run_backend(module, log_level=log_level, verbose=False)
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/utils/prerequisites.py` & `carefree-drawboard-0.0.0a5/cfdraw/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/utils/processes.py` & `carefree-drawboard-0.0.0a5/cfdraw/utils/processes.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/utils/server.py` & `carefree-drawboard-0.0.0a5/cfdraw/utils/server.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/utils/template.py` & `carefree-drawboard-0.0.0a5/cfdraw/utils/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,44 +8,43 @@
 
 IMAGE_APP_TEMPLATE = f"""
 from PIL import Image
 from PIL import ImageFilter
 from cfdraw import *
 
 # This will perform a Gaussian blur on the image
-class Plugin(IHttpFieldsPlugin):
+class Plugin(IFieldsPlugin):
     @property
     def settings(self) -> IPluginSettings:
         return IPluginSettings(
             w=300,
             h=180,
             nodeConstraint=NodeConstraints.IMAGE,
             pivot=PivotType.RT,
             follow=True,
-            pluginInfo=IHttpFieldsPluginInfo(
+            pluginInfo=IFieldsPluginInfo(
                 definitions=dict(
                     size=INumberField(
                         default=3,
                         min=1,
                         max=10,
                         step=1,
                         isInt=True,
                         label="Size",
                     )
                 ),
             ),
         )
 
-    async def process(self, data: IPluginRequest) -> Image.Image:
+    async def process(self, data: ISocketRequest) -> Image.Image:
         image = await self.load_image(data.nodeData.src)
         return image.filter(ImageFilter.GaussianBlur(data.extraData["size"]))
 
 
 register_plugin("blur")(Plugin)
-register_all_available_plugins()
 {constants.DEFAULT_ENTRY} = App()
 """
 
 CONFIG_TEMPLATE = f"""
 from cfdraw.config import Config
 
 {constants.DEFAULT_CONFIG_ENTRY} = Config(
```

### Comparing `carefree-drawboard-0.0.0a4/setup.py` & `carefree-drawboard-0.0.0a5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.0-alpha.4"
+VERSION = "0.0.0-alpha.5"
 PACKAGE_NAME = "carefree-drawboard"
 
 DESCRIPTION = "🎨 Infinite Drawboard in Python"
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
@@ -12,26 +12,26 @@
     version=VERSION,
     packages=find_packages(exclude=("tests",)),
     include_package_data=True,
     entry_points={"console_scripts": ["cfdraw = cfdraw.cli:cli"]},
     install_requires=[
         "rich",
         "typer",
-        "fastapi",
+        "fastapi>=0.95.1",
         "gunicorn",
         "pydantic",
         "uvicorn",
         "websockets",
         "watchdog",
         "python-multipart",
         "carefree-toolkit>=0.3.4",
         "pillow",
         "aiohttp",
         "charset-normalizer==2.1.0",
-        "tornado",
+        "aiofiles",
     ],
     author="carefree0910",
     author_email="syameimaru.saki@gmail.com",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     keywords="python carefree-learn drawboard",
```

