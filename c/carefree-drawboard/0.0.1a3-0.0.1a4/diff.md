# Comparing `tmp/carefree-drawboard-0.0.1a3.tar.gz` & `tmp/carefree-drawboard-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-drawboard-0.0.1a3.tar", last modified: Mon May 15 19:46:13 2023, max compression
+gzip compressed data, was "carefree-drawboard-0.0.1a4.tar", last modified: Mon May 22 14:54:00 2023, max compression
```

## Comparing `carefree-drawboard-0.0.1a3.tar` & `carefree-drawboard-0.0.1a4.tar`

### file list

```diff
@@ -1,215 +1,245 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:13.126598 carefree-drawboard-0.0.1a3/
--rw-rw-rw-   0        0        0    11557 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a3/LICENSE
--rw-rw-rw-   0        0        0      121 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a3/MANIFEST.in
--rw-rw-rw-   0        0        0     9102 2023-05-15 19:46:13.127595 carefree-drawboard-0.0.1a3/PKG-INFO
--rw-rw-rw-   0        0        0     8819 2023-05-15 01:06:24.000000 carefree-drawboard-0.0.1a3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.725888 carefree-drawboard-0.0.1a3/carefree_drawboard.egg-info/
--rw-rw-rw-   0        0        0     9102 2023-05-15 19:46:08.000000 carefree-drawboard-0.0.1a3/carefree_drawboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6362 2023-05-15 19:46:12.000000 carefree-drawboard-0.0.1a3/carefree_drawboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 19:46:08.000000 carefree-drawboard-0.0.1a3/carefree_drawboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 19:46:08.000000 carefree-drawboard-0.0.1a3/carefree_drawboard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      164 2023-05-15 19:46:08.000000 carefree-drawboard-0.0.1a3/carefree_drawboard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-15 19:46:08.000000 carefree-drawboard-0.0.1a3/carefree_drawboard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.734872 carefree-drawboard-0.0.1a3/cfdraw/
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.752337 carefree-drawboard-0.0.1a3/cfdraw/.web/
--rw-rw-rw-   0        0        0      137 2023-05-12 19:54:40.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/.env
--rw-rw-rw-   0        0        0      143 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/.prettierrc
--rw-rw-rw-   0        0        0      548 2023-05-14 15:52:46.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/index.html
--rw-rw-rw-   0        0        0     1669 2023-05-15 16:16:52.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/package.json
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.772284 carefree-drawboard-0.0.1a3/cfdraw/.web/src/
--rw-rw-rw-   0        0        0     1012 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/App.tsx
--rw-rw-rw-   0        0        0     1470 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/BoardPanel.tsx
--rw-rw-rw-   0        0        0     5509 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/_settings.ts
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.798992 carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/
--rw-rw-rw-   0        0        0     2316 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/addImage.ts
--rw-rw-rw-   0        0        0      919 2023-05-15 16:16:52.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/addText.ts
--rw-rw-rw-   0        0        0     9398 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/arrange.ts
--rw-rw-rw-   0        0        0     1806 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/download.ts
--rw-rw-rw-   0        0        0     1979 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/export.ts
--rw-rw-rw-   0        0        0      236 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/i18n.ts
--rw-rw-rw-   0        0        0     8268 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/importMeta.ts
--rw-rw-rw-   0        0        0     1448 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/managePlugins.ts
--rw-rw-rw-   0        0        0     5032 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/manageProjects.ts
--rw-rw-rw-   0        0        0      272 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/update.ts
--rw-rw-rw-   0        0        0     1118 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/uploadImage.ts
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.801983 carefree-drawboard-0.0.1a3/cfdraw/.web/src/assets/
--rw-rw-rw-   0        0        0     6591 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/assets/icon-loading.json
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.805973 carefree-drawboard-0.0.1a3/cfdraw/.web/src/assets/icons/
--rw-rw-rw-   0        0        0      257 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/assets/icons/arrow-down.svg
--rw-rw-rw-   0        0        0      925 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/assets/icons/delete.svg
--rw-rw-rw-   0        0        0     6681 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/assets/loading-page.json
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.835301 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/
--rw-rw-rw-   0        0        0     2740 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFButton.tsx
--rw-rw-rw-   0        0        0      640 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFCircularProgress.tsx
--rw-rw-rw-   0        0        0      359 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFDivider.tsx
--rw-rw-rw-   0        0        0      235 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFHeading.tsx
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.839292 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFIcon/
--rw-rw-rw-   0        0        0      546 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFIcon/index.scss
--rw-rw-rw-   0        0        0     1568 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFIcon/index.tsx
--rw-rw-rw-   0        0        0     1484 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFImageUploader.tsx
--rw-rw-rw-   0        0        0      522 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFInput.tsx
--rw-rw-rw-   0        0        0     1382 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFLoadingPage.tsx
--rw-rw-rw-   0        0        0      984 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFLottie.tsx
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.844278 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFSelect/
--rw-rw-rw-   0        0        0       70 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFSelect/index.scss
--rw-rw-rw-   0        0        0     3514 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFSelect/index.tsx
--rw-rw-rw-   0        0        0     5223 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFSlider.tsx
--rw-rw-rw-   0        0        0     1738 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFSwitch.tsx
--rw-rw-rw-   0        0        0      740 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFText.tsx
--rw-rw-rw-   0        0        0      531 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFTextarea.tsx
--rw-rw-rw-   0        0        0      417 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFTooltip.tsx
--rw-rw-rw-   0        0        0      185 2023-05-14 15:52:46.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/env.d.ts
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.864911 carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/
--rw-rw-rw-   0        0        0     1316 2023-05-14 15:52:46.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/useAuth.ts
--rw-rw-rw-   0        0        0     2976 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/useDocumentEvents.ts
--rw-rw-rw-   0        0        0     3077 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/useFileDropper.ts
--rw-rw-rw-   0        0        0     4410 2023-05-12 14:52:45.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/useGridLines.ts
--rw-rw-rw-   0        0        0     3943 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/useInitBoard.ts
--rw-rw-rw-   0        0        0      669 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/usePreventDefaults.ts
--rw-rw-rw-   0        0        0     5914 2023-05-12 20:46:03.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/usePython.ts
--rw-rw-rw-   0        0        0    10902 2023-05-14 10:39:38.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/useSetup.ts
--rw-rw-rw-   0        0        0      163 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/index.scss
--rw-rw-rw-   0        0        0      345 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/index.tsx
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.891800 carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/
--rw-rw-rw-   0        0        0      954 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/add.ts
--rw-rw-rw-   0        0        0      849 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/brush.ts
--rw-rw-rw-   0        0        0     1148 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/download.ts
--rw-rw-rw-   0        0        0     1466 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/index.ts
--rw-rw-rw-   0        0        0      404 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/nodeEditor.ts
--rw-rw-rw-   0        0        0     2372 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/plugins.ts
--rw-rw-rw-   0        0        0     1746 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/projects.ts
--rw-rw-rw-   0        0        0      896 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/settings.ts
--rw-rw-rw-   0        0        0    10105 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/toast.ts
--rw-rw-rw-   0        0        0     2343 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/tooltip.ts
--rw-rw-rw-   0        0        0      976 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/ui.ts
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.894792 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.914858 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_python/
--rw-rw-rw-   0        0        0     2196 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_python/ChatPlugin.tsx
--rw-rw-rw-   0        0        0     3027 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
--rw-rw-rw-   0        0        0     2920 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_python/PluginGroup.tsx
--rw-rw-rw-   0        0        0     3394 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
--rw-rw-rw-   0        0        0     1909 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_python/QAPlugin.tsx
--rw-rw-rw-   0        0        0     2127 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
--rw-rw-rw-   0        0        0     2621 2023-05-12 14:52:45.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_python/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.942557 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/
--rw-rw-rw-   0        0        0     3760 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/AddPlugin.tsx
--rw-rw-rw-   0        0        0      714 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx
--rw-rw-rw-   0        0        0     4598 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx
--rw-rw-rw-   0        0        0      854 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/DeletePlugin.tsx
--rw-rw-rw-   0        0        0     3546 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx
--rw-rw-rw-   0        0        0     1083 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx
--rw-rw-rw-   0        0        0     1123 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/LinksPlugin.tsx
--rw-rw-rw-   0        0        0     1352 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/MetaPlugin.tsx
--rw-rw-rw-   0        0        0     8594 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx
--rw-rw-rw-   0        0        0     4927 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx
--rw-rw-rw-   0        0        0     2204 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx
--rw-rw-rw-   0        0        0     1266 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.952279 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.968016 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Fields/
--rw-rw-rw-   0        0        0     1116 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Fields/BooleanField.tsx
--rw-rw-rw-   0        0        0     2043 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
--rw-rw-rw-   0        0        0     2565 2023-05-12 20:46:03.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
--rw-rw-rw-   0        0        0     2291 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
--rw-rw-rw-   0        0        0     2620 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Fields/index.tsx
--rw-rw-rw-   0        0        0      720 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Fields/utils.ts
--rw-rw-rw-   0        0        0     7862 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Floating.tsx
--rw-rw-rw-   0        0        0      307 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Link.tsx
--rw-rw-rw-   0        0        0    10883 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Render.tsx
--rw-rw-rw-   0        0        0      214 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/hooks.ts
--rw-rw-rw-   0        0        0     2295 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/index.tsx
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.974002 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/utils/
--rw-rw-rw-   0        0        0     1960 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/utils/cleanup.ts
--rw-rw-rw-   0        0        0     1450 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/utils/factory.ts
--rw-rw-rw-   0        0        0     4048 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/utils/renderFilters.ts
--rw-rw-rw-   0        0        0      841 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/react-app-env.d.ts
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.979517 carefree-drawboard-0.0.1a3/cfdraw/.web/src/requests/
--rw-rw-rw-   0        0        0     1290 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/requests/actions.ts
--rw-rw-rw-   0        0        0     2921 2023-05-12 20:35:16.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/requests/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.983131 carefree-drawboard-0.0.1a3/cfdraw/.web/src/requests/interceptors/
--rw-rw-rw-   0        0        0      880 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/requests/interceptors/_python.ts
--rw-rw-rw-   0        0        0      752 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/requests/interceptors/index.ts
--rw-rw-rw-   0        0        0       38 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/reset.d.ts
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:12.997095 carefree-drawboard-0.0.1a3/cfdraw/.web/src/schema/
--rw-rw-rw-   0        0        0     5025 2023-05-12 20:35:16.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/schema/_python.ts
--rw-rw-rw-   0        0        0     1804 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/schema/fields.ts
--rw-rw-rw-   0        0        0     2076 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/schema/meta.ts
--rw-rw-rw-   0        0        0      313 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/schema/misc.ts
--rw-rw-rw-   0        0        0     3514 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/schema/plugins.ts
--rw-rw-rw-   0        0        0      850 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/schema/requests.ts
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:13.025819 carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/
--rw-rw-rw-   0        0        0      792 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/debug.ts
--rw-rw-rw-   0        0        0     1495 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/gridLines.ts
--rw-rw-rw-   0        0        0      578 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/hooks.ts
--rw-rw-rw-   0        0        0     1107 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/meta.ts
--rw-rw-rw-   0        0        0     7527 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/pluginsInfo.ts
--rw-rw-rw-   0        0        0     1968 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/projects.ts
--rw-rw-rw-   0        0        0     1716 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/settings.ts
--rw-rw-rw-   0        0        0     9316 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/socket.ts
--rw-rw-rw-   0        0        0     4852 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/theme.ts
--rw-rw-rw-   0        0        0     2054 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/ui.ts
--rw-rw-rw-   0        0        0      501 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/user.ts
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:13.040819 carefree-drawboard-0.0.1a3/cfdraw/.web/src/utils/
--rw-rw-rw-   0        0        0      467 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/utils/bem.ts
--rw-rw-rw-   0        0        0     3876 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/utils/constants.ts
--rw-rw-rw-   0        0        0     1266 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/utils/event.ts
--rw-rw-rw-   0        0        0     1822 2023-05-15 16:16:52.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/utils/misc.ts
--rw-rw-rw-   0        0        0     2053 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/utils/toast.ts
--rw-rw-rw-   0        0        0       39 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/src/vite-env.d.ts
--rw-rw-rw-   0        0        0      656 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/tsconfig.json
--rw-rw-rw-   0        0        0      193 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/tsconfig.node.json
--rw-rw-rw-   0        0        0      103 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/tsconfig.paths.json
--rw-rw-rw-   0        0        0     2069 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/vite.config.ts
--rw-rw-rw-   0        0        0   224022 2023-05-15 16:16:52.000000 carefree-drawboard-0.0.1a3/cfdraw/.web/yarn.lock
--rw-rw-rw-   0        0        0      475 2023-05-08 16:30:47.000000 carefree-drawboard-0.0.1a3/cfdraw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:13.046800 carefree-drawboard-0.0.1a3/cfdraw/app/
--rw-rw-rw-   0        0        0       20 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/app/__init__.py
--rw-rw-rw-   0        0        0     4826 2023-05-14 11:08:54.000000 carefree-drawboard-0.0.1a3/cfdraw/app/app.py
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:13.062272 carefree-drawboard-0.0.1a3/cfdraw/app/endpoints/
--rw-rw-rw-   0        0        0      139 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/app/endpoints/__init__.py
--rw-rw-rw-   0        0        0     1273 2023-05-14 15:52:46.000000 carefree-drawboard-0.0.1a3/cfdraw/app/endpoints/assets.py
--rw-rw-rw-   0        0        0      493 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/app/endpoints/base.py
--rw-rw-rw-   0        0        0     7363 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a3/cfdraw/app/endpoints/project.py
--rw-rw-rw-   0        0        0     6918 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/app/endpoints/queue.py
--rw-rw-rw-   0        0        0     3577 2023-05-14 11:08:54.000000 carefree-drawboard-0.0.1a3/cfdraw/app/endpoints/upload.py
--rw-rw-rw-   0        0        0     3991 2023-05-14 10:39:38.000000 carefree-drawboard-0.0.1a3/cfdraw/app/endpoints/websocket.py
--rw-rw-rw-   0        0        0     1277 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/app/schema.py
--rw-rw-rw-   0        0        0     3518 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/cli.py
--rw-rw-rw-   0        0        0     2430 2023-05-12 20:35:16.000000 carefree-drawboard-0.0.1a3/cfdraw/config.py
--rw-rw-rw-   0        0        0     3045 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a3/cfdraw/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:13.068280 carefree-drawboard-0.0.1a3/cfdraw/parsers/
--rw-rw-rw-   0        0        0       44 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/parsers/__init__.py
--rw-rw-rw-   0        0        0      710 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/parsers/chakra.py
--rw-rw-rw-   0        0        0    13291 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/parsers/noli.py
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:13.075236 carefree-drawboard-0.0.1a3/cfdraw/plugins/
--rw-rw-rw-   0        0        0       97 2023-05-08 01:07:56.000000 carefree-drawboard-0.0.1a3/cfdraw/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:13.081219 carefree-drawboard-0.0.1a3/cfdraw/plugins/_internal/
--rw-rw-rw-   0        0        0       52 2023-05-08 01:08:15.000000 carefree-drawboard-0.0.1a3/cfdraw/plugins/_internal/__init__.py
--rw-rw-rw-   0        0        0     1399 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/plugins/_internal/node_validator.py
--rw-rw-rw-   0        0        0     1457 2023-05-08 01:08:43.000000 carefree-drawboard-0.0.1a3/cfdraw/plugins/_internal/sync.py
--rw-rw-rw-   0        0        0     6755 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/plugins/base.py
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:13.083213 carefree-drawboard-0.0.1a3/cfdraw/plugins/community/
--rw-rw-rw-   0        0        0        0 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/plugins/community/__init__.py
--rw-rw-rw-   0        0        0     1918 2023-05-08 01:06:37.000000 carefree-drawboard-0.0.1a3/cfdraw/plugins/factory.py
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:13.091194 carefree-drawboard-0.0.1a3/cfdraw/plugins/middlewares/
--rw-rw-rw-   0        0        0       76 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/plugins/middlewares/__init__.py
--rw-rw-rw-   0        0        0     1696 2023-05-14 11:08:54.000000 carefree-drawboard-0.0.1a3/cfdraw/plugins/middlewares/response.py
--rw-rw-rw-   0        0        0      904 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/plugins/middlewares/send_message.py
--rw-rw-rw-   0        0        0      643 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/plugins/middlewares/timer.py
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:13.099695 carefree-drawboard-0.0.1a3/cfdraw/schema/
--rw-rw-rw-   0        0        0       72 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/schema/__init__.py
--rw-rw-rw-   0        0        0     5950 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/schema/fields.py
--rw-rw-rw-   0        0        0    18207 2023-05-12 20:35:16.000000 carefree-drawboard-0.0.1a3/cfdraw/schema/plugins.py
--rw-rw-rw-   0        0        0     1615 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/schema/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-15 19:46:13.124604 carefree-drawboard-0.0.1a3/cfdraw/utils/
--rw-rw-rw-   0        0        0        0 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/utils/__init__.py
--rw-rw-rw-   0        0        0      833 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/utils/cache.py
--rw-rw-rw-   0        0        0      875 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/utils/console.py
--rw-rw-rw-   0        0        0     6551 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/utils/data_structures.py
--rw-rw-rw-   0        0        0     2622 2023-05-12 20:16:11.000000 carefree-drawboard-0.0.1a3/cfdraw/utils/exec.py
--rw-rw-rw-   0        0        0     2415 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/utils/misc.py
--rw-rw-rw-   0        0        0      638 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/utils/prerequisites.py
--rw-rw-rw-   0        0        0     1766 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/utils/processes.py
--rw-rw-rw-   0        0        0     4036 2023-05-12 20:35:16.000000 carefree-drawboard-0.0.1a3/cfdraw/utils/server.py
--rw-rw-rw-   0        0        0     2732 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a3/cfdraw/utils/template.py
--rw-rw-rw-   0        0        0      113 2023-05-15 19:46:13.129589 carefree-drawboard-0.0.1a3/setup.cfg
--rw-rw-rw-   0        0        0     1063 2023-05-15 19:45:53.000000 carefree-drawboard-0.0.1a3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.838981 carefree-drawboard-0.0.1a4/
+-rw-rw-rw-   0        0        0    11557 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.1a4/LICENSE
+-rw-rw-rw-   0        0        0      121 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/MANIFEST.in
+-rw-rw-rw-   0        0        0     9469 2023-05-22 14:54:00.839977 carefree-drawboard-0.0.1a4/PKG-INFO
+-rw-rw-rw-   0        0        0     9186 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.736814 carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/
+-rw-rw-rw-   0        0        0     9469 2023-05-22 14:53:57.000000 carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7667 2023-05-22 14:54:00.000000 carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 14:53:57.000000 carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 14:53:57.000000 carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      179 2023-05-22 14:53:57.000000 carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-22 14:53:57.000000 carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.738808 carefree-drawboard-0.0.1a4/cfdraw/
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.742795 carefree-drawboard-0.0.1a4/cfdraw/.web/
+-rw-rw-rw-   0        0        0      137 2023-05-13 11:08:39.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/.env
+-rw-rw-rw-   0        0        0      143 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/.prettierrc
+-rw-rw-rw-   0        0        0      548 2023-05-15 11:41:37.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/index.html
+-rw-rw-rw-   0        0        0     1967 2023-05-22 14:36:20.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/package.json
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.747778 carefree-drawboard-0.0.1a4/cfdraw/.web/src/
+-rw-rw-rw-   0        0        0     1012 2023-05-14 06:28:56.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/App.tsx
+-rw-rw-rw-   0        0        0     1470 2023-05-14 03:25:05.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/BoardPanel.tsx
+-rw-rw-rw-   0        0        0     6602 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/_settings.ts
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.752761 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/
+-rw-rw-rw-   0        0        0     2316 2023-05-13 11:08:39.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/addImage.ts
+-rw-rw-rw-   0        0        0      919 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/addText.ts
+-rw-rw-rw-   0        0        0     9398 2023-05-13 11:08:39.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/arrange.ts
+-rw-rw-rw-   0        0        0     1806 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/download.ts
+-rw-rw-rw-   0        0        0     1979 2023-05-13 11:08:39.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/export.ts
+-rw-rw-rw-   0        0        0      236 2023-05-04 12:54:31.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/i18n.ts
+-rw-rw-rw-   0        0        0     8257 2023-05-22 09:35:32.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/importMeta.ts
+-rw-rw-rw-   0        0        0     1838 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/managePlugins.ts
+-rw-rw-rw-   0        0        0     5032 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/manageProjects.ts
+-rw-rw-rw-   0        0        0      272 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/update.ts
+-rw-rw-rw-   0        0        0     1118 2023-05-06 09:50:20.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/uploadImage.ts
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.753757 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.764721 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/
+-rw-rw-rw-   0        0        0      504 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/add-blank.svg
+-rw-rw-rw-   0        0        0      615 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/add-frame.svg
+-rw-rw-rw-   0        0        0     1243 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/add-image.svg
+-rw-rw-rw-   0        0        0      837 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/add-project.svg
+-rw-rw-rw-   0        0        0      414 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/add-text.svg
+-rw-rw-rw-   0        0        0      307 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/add.svg
+-rw-rw-rw-   0        0        0      557 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/arrange.svg
+-rw-rw-rw-   0        0        0      257 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/arrow-down.svg
+-rw-rw-rw-   0        0        0     1378 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/brush.svg
+-rw-rw-rw-   0        0        0      927 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/delete.svg
+-rw-rw-rw-   0        0        0      574 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/download.svg
+-rw-rw-rw-   0        0        0      770 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/editor.svg
+-rw-rw-rw-   0        0        0      711 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/email.svg
+-rw-rw-rw-   0        0        0     1346 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/github.svg
+-rw-rw-rw-   0        0        0     1270 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/group-editor.svg
+-rw-rw-rw-   0        0        0      718 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/meta.svg
+-rw-rw-rw-   0        0        0      930 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/multi-editor.svg
+-rw-rw-rw-   0        0        0      914 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/project.svg
+-rw-rw-rw-   0        0        0      465 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/redo.svg
+-rw-rw-rw-   0        0        0     1420 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/settings.svg
+-rw-rw-rw-   0        0        0     1104 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/shortcuts.svg
+-rw-rw-rw-   0        0        0      466 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/undo.svg
+-rw-rw-rw-   0        0        0      464 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/wiki.svg
+-rw-rw-rw-   0        0        0     3284 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/image-placeholder.svg
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.765718 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/lottie/
+-rw-rw-rw-   0        0        0     6591 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/lottie/icon-loading.json
+-rw-rw-rw-   0        0        0     6681 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/lottie/loading-page.json
+-rw-rw-rw-   0        0        0     5930 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/nsfw-placeholder.svg
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.772694 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/
+-rw-rw-rw-   0        0        0     2796 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFButton.tsx
+-rw-rw-rw-   0        0        0      640 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFCircularProgress.tsx
+-rw-rw-rw-   0        0        0     2202 2023-05-18 14:43:58.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFColorPicker.tsx
+-rw-rw-rw-   0        0        0      359 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFDivider.tsx
+-rw-rw-rw-   0        0        0      235 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFHeading.tsx
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.773694 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFIcon/
+-rw-rw-rw-   0        0        0      546 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFIcon/index.scss
+-rw-rw-rw-   0        0        0     1568 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFIcon/index.tsx
+-rw-rw-rw-   0        0        0     1484 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFImageUploader.tsx
+-rw-rw-rw-   0        0        0      794 2023-05-22 14:32:05.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFInput.tsx
+-rw-rw-rw-   0        0        0     1330 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFLoadingPage.tsx
+-rw-rw-rw-   0        0        0      984 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFLottie.tsx
+-rw-rw-rw-   0        0        0     1441 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFMarkdown.tsx
+-rw-rw-rw-   0        0        0     3386 2023-05-22 14:28:24.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFSelect.tsx
+-rw-rw-rw-   0        0        0     5270 2023-05-18 14:43:58.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFSlider.tsx
+-rw-rw-rw-   0        0        0     1600 2023-05-18 14:43:58.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFSwitch.tsx
+-rw-rw-rw-   0        0        0      738 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFText.tsx
+-rw-rw-rw-   0        0        0      491 2023-05-22 14:28:24.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFTextarea.tsx
+-rw-rw-rw-   0        0        0     1007 2023-05-18 14:43:58.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFTooltip.tsx
+-rw-rw-rw-   0        0        0      185 2023-05-15 08:54:13.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/env.d.ts
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.776683 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/
+-rw-rw-rw-   0        0        0     1316 2023-05-14 13:38:46.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useAuth.ts
+-rw-rw-rw-   0        0        0     3471 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useDocumentEvents.ts
+-rw-rw-rw-   0        0        0     3077 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useFileDropper.ts
+-rw-rw-rw-   0        0        0     4410 2023-05-12 10:15:34.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useGridLines.ts
+-rw-rw-rw-   0        0        0     3943 2023-05-14 03:25:05.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useInitBoard.ts
+-rw-rw-rw-   0        0        0      669 2023-05-12 12:36:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/usePreventDefaults.ts
+-rw-rw-rw-   0        0        0     6043 2023-05-19 13:14:54.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/usePython.ts
+-rw-rw-rw-   0        0        0    11019 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useSetup.ts
+-rw-rw-rw-   0        0        0      163 2023-05-12 12:36:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/index.scss
+-rw-rw-rw-   0        0        0      345 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/index.tsx
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.781668 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/
+-rw-rw-rw-   0        0        0     1103 2023-05-22 01:50:13.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/add.ts
+-rw-rw-rw-   0        0        0      849 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/brush.ts
+-rw-rw-rw-   0        0        0     1148 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/download.ts
+-rw-rw-rw-   0        0        0     1466 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/index.ts
+-rw-rw-rw-   0        0        0      404 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/nodeEditor.ts
+-rw-rw-rw-   0        0        0     2556 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/plugins.ts
+-rw-rw-rw-   0        0        0     1746 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/projects.ts
+-rw-rw-rw-   0        0        0      896 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/settings.ts
+-rw-rw-rw-   0        0        0    10266 2023-05-22 01:50:13.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/toast.ts
+-rw-rw-rw-   0        0        0     2501 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/tooltip.ts
+-rw-rw-rw-   0        0        0     1488 2023-05-21 12:53:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/ui.ts
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.782663 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.785653 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/
+-rw-rw-rw-   0        0        0     2195 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/ChatPlugin.tsx
+-rw-rw-rw-   0        0        0     2996 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
+-rw-rw-rw-   0        0        0      701 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/MarkdownPlugin.tsx
+-rw-rw-rw-   0        0        0     2920 2023-05-04 12:54:31.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/PluginGroup.tsx
+-rw-rw-rw-   0        0        0     3576 2023-05-19 13:14:54.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
+-rw-rw-rw-   0        0        0     1908 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/QAPlugin.tsx
+-rw-rw-rw-   0        0        0      804 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
+-rw-rw-rw-   0        0        0     4365 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.791141 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/
+-rw-rw-rw-   0        0        0     5887 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/AddPlugin.tsx
+-rw-rw-rw-   0        0        0      658 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx
+-rw-rw-rw-   0        0        0     4581 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx
+-rw-rw-rw-   0        0        0      800 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/DeletePlugin.tsx
+-rw-rw-rw-   0        0        0     4152 2023-05-22 14:28:24.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx
+-rw-rw-rw-   0        0        0     1008 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx
+-rw-rw-rw-   0        0        0     1259 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/LinksPlugin.tsx
+-rw-rw-rw-   0        0        0     1375 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/MetaPlugin.tsx
+-rw-rw-rw-   0        0        0     8878 2023-05-22 14:33:43.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx
+-rw-rw-rw-   0        0        0     5152 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx
+-rw-rw-rw-   0        0        0     1909 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/ShortcutsPlugin.tsx
+-rw-rw-rw-   0        0        0     4271 2023-05-22 14:28:24.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx
+-rw-rw-rw-   0        0        0     1176 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.793134 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.797121 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/
+-rw-rw-rw-   0        0        0     1083 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/BooleanField.tsx
+-rw-rw-rw-   0        0        0     1262 2023-05-18 14:43:58.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/ColorField.tsx
+-rw-rw-rw-   0        0        0      881 2023-05-18 14:43:58.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/Field.tsx
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.798117 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/ListField/
+-rw-rw-rw-   0        0        0      367 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/ListField/index.scss
+-rw-rw-rw-   0        0        0     5940 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/ListField/index.tsx
+-rw-rw-rw-   0        0        0     2013 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
+-rw-rw-rw-   0        0        0     2516 2023-05-22 14:28:24.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
+-rw-rw-rw-   0        0        0     2276 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
+-rw-rw-rw-   0        0        0     1915 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/index.tsx
+-rw-rw-rw-   0        0        0     1763 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/utils.ts
+-rw-rw-rw-   0        0        0     7706 2023-05-18 14:43:58.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Floating.tsx
+-rw-rw-rw-   0        0        0      410 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Link.tsx
+-rw-rw-rw-   0        0        0    10883 2023-05-22 03:10:27.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Render.tsx
+-rw-rw-rw-   0        0        0      214 2023-05-04 12:54:31.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/hooks.ts
+-rw-rw-rw-   0        0        0     2381 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/index.tsx
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.801108 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/utils/
+-rw-rw-rw-   0        0        0     1960 2023-05-06 06:34:44.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/utils/cleanup.ts
+-rw-rw-rw-   0        0        0     1450 2023-05-04 12:54:31.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/utils/factory.ts
+-rw-rw-rw-   0        0        0     4081 2023-05-19 13:14:54.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/utils/renderFilters.ts
+-rw-rw-rw-   0        0        0      841 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/react-app-env.d.ts
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.803101 carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/
+-rw-rw-rw-   0        0        0     1290 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/actions.ts
+-rw-rw-rw-   0        0        0     2921 2023-05-14 03:25:05.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.804098 carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/interceptors/
+-rw-rw-rw-   0        0        0      880 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/interceptors/_python.ts
+-rw-rw-rw-   0        0        0      752 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/interceptors/index.ts
+-rw-rw-rw-   0        0        0       38 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/reset.d.ts
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.809081 carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/
+-rw-rw-rw-   0        0        0     5031 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/_python.ts
+-rw-rw-rw-   0        0        0     1854 2023-05-21 04:22:06.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/fields.ts
+-rw-rw-rw-   0        0        0     2076 2023-05-06 09:11:52.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/meta.ts
+-rw-rw-rw-   0        0        0      313 2023-05-04 12:54:31.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/misc.ts
+-rw-rw-rw-   0        0        0     3910 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/plugins.ts
+-rw-rw-rw-   0        0        0      850 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/requests.ts
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.818051 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/
+-rw-rw-rw-   0        0        0      792 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/debug.ts
+-rw-rw-rw-   0        0        0     1495 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/gridLines.ts
+-rw-rw-rw-   0        0        0      578 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/hooks.ts
+-rw-rw-rw-   0        0        0     2162 2023-05-17 16:39:19.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/meta.ts
+-rw-rw-rw-   0        0        0     7774 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/pluginsInfo.ts
+-rw-rw-rw-   0        0        0     1968 2023-05-14 06:28:56.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/projects.ts
+-rw-rw-rw-   0        0        0     1888 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/settings.ts
+-rw-rw-rw-   0        0        0     9316 2023-05-14 06:28:56.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/socket.ts
+-rw-rw-rw-   0        0        0     5090 2023-05-22 14:28:24.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/theme.ts
+-rw-rw-rw-   0        0        0     2054 2023-05-04 12:54:31.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/ui.ts
+-rw-rw-rw-   0        0        0      501 2023-05-04 12:54:31.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/user.ts
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.820044 carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/
+-rw-rw-rw-   0        0        0      467 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/bem.ts
+-rw-rw-rw-   0        0        0     1921 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/constants.ts
+-rw-rw-rw-   0        0        0     1266 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/event.ts
+-rw-rw-rw-   0        0        0     1822 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/misc.ts
+-rw-rw-rw-   0        0        0     2053 2023-05-14 06:28:56.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/toast.ts
+-rw-rw-rw-   0        0        0       39 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/vite-env.d.ts
+-rw-rw-rw-   0        0        0      656 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/tsconfig.json
+-rw-rw-rw-   0        0        0      193 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/tsconfig.node.json
+-rw-rw-rw-   0        0        0      103 2023-05-14 02:56:39.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/tsconfig.paths.json
+-rw-rw-rw-   0        0        0     2165 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/vite.config.ts
+-rw-rw-rw-   0        0        0   272589 2023-05-22 14:39:55.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/yarn.lock
+-rw-rw-rw-   0        0        0      475 2023-05-08 06:29:38.000000 carefree-drawboard-0.0.1a4/cfdraw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.821041 carefree-drawboard-0.0.1a4/cfdraw/app/
+-rw-rw-rw-   0        0        0       20 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.1a4/cfdraw/app/__init__.py
+-rw-rw-rw-   0        0        0     4826 2023-05-22 14:28:31.000000 carefree-drawboard-0.0.1a4/cfdraw/app/app.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.825027 carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/
+-rw-rw-rw-   0        0        0      139 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     1273 2023-05-15 11:41:37.000000 carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/assets.py
+-rw-rw-rw-   0        0        0      493 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/base.py
+-rw-rw-rw-   0        0        0     7161 2023-05-19 13:15:29.000000 carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/project.py
+-rw-rw-rw-   0        0        0     6900 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/queue.py
+-rw-rw-rw-   0        0        0     3617 2023-05-22 14:28:17.000000 carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/upload.py
+-rw-rw-rw-   0        0        0     3985 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/websocket.py
+-rw-rw-rw-   0        0        0     1277 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/app/schema.py
+-rw-rw-rw-   0        0        0     3518 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/cli.py
+-rw-rw-rw-   0        0        0     2550 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/config.py
+-rw-rw-rw-   0        0        0     2930 2023-05-22 11:26:26.000000 carefree-drawboard-0.0.1a4/cfdraw/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.827020 carefree-drawboard-0.0.1a4/cfdraw/parsers/
+-rw-rw-rw-   0        0        0       44 2023-04-09 01:57:56.000000 carefree-drawboard-0.0.1a4/cfdraw/parsers/__init__.py
+-rw-rw-rw-   0        0        0      710 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/parsers/chakra.py
+-rw-rw-rw-   0        0        0    13291 2023-05-06 05:18:28.000000 carefree-drawboard-0.0.1a4/cfdraw/parsers/noli.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.829014 carefree-drawboard-0.0.1a4/cfdraw/plugins/
+-rw-rw-rw-   0        0        0       97 2023-05-08 06:29:38.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.831008 carefree-drawboard-0.0.1a4/cfdraw/plugins/_internal/
+-rw-rw-rw-   0        0        0       52 2023-05-08 06:29:38.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/_internal/__init__.py
+-rw-rw-rw-   0        0        0     1399 2023-05-08 06:29:38.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/_internal/node_validator.py
+-rw-rw-rw-   0        0        0     1510 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/_internal/sync.py
+-rw-rw-rw-   0        0        0     4250 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/base.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.831008 carefree-drawboard-0.0.1a4/cfdraw/plugins/community/
+-rw-rw-rw-   0        0        0        0 2023-04-14 05:16:37.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/community/__init__.py
+-rw-rw-rw-   0        0        0     1887 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.833001 carefree-drawboard-0.0.1a4/cfdraw/plugins/middlewares/
+-rw-rw-rw-   0        0        0       76 2023-05-05 11:49:30.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     1776 2023-05-19 13:15:22.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/middlewares/response.py
+-rw-rw-rw-   0        0        0      904 2023-05-05 11:49:30.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/middlewares/send_message.py
+-rw-rw-rw-   0        0        0      643 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/middlewares/timer.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.834994 carefree-drawboard-0.0.1a4/cfdraw/schema/
+-rw-rw-rw-   0        0        0       72 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/schema/__init__.py
+-rw-rw-rw-   0        0        0     6566 2023-05-18 14:43:58.000000 carefree-drawboard-0.0.1a4/cfdraw/schema/fields.py
+-rw-rw-rw-   0        0        0    22856 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/schema/plugins.py
+-rw-rw-rw-   0        0        0     2355 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/schema/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.838981 carefree-drawboard-0.0.1a4/cfdraw/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-08 03:23:05.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/cache.py
+-rw-rw-rw-   0        0        0      875 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/console.py
+-rw-rw-rw-   0        0        0     2622 2023-05-14 02:59:27.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/exec.py
+-rw-rw-rw-   0        0        0     2327 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/misc.py
+-rw-rw-rw-   0        0        0      638 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/prerequisites.py
+-rw-rw-rw-   0        0        0     1766 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/processes.py
+-rw-rw-rw-   0        0        0     2140 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/server.py
+-rw-rw-rw-   0        0        0     2732 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/template.py
+-rw-rw-rw-   0        0        0      113 2023-05-22 14:54:00.840974 carefree-drawboard-0.0.1a4/setup.cfg
+-rw-rw-rw-   0        0        0     1102 2023-05-22 14:51:54.000000 carefree-drawboard-0.0.1a4/setup.py
```

### Comparing `carefree-drawboard-0.0.1a3/LICENSE` & `carefree-drawboard-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/PKG-INFO` & `carefree-drawboard-0.0.1a4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-drawboard
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: 🎨 Infinite Drawboard in Python
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn drawboard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -85,14 +85,15 @@
 
 * [**Getting Started**](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
 * [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins. It also shows how to use the `IPluginGroup` in `carefree-drawboard` 🎨 to group the plugins together and make the UI cleaner.
 * [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common SD plugins.
 * [**Caption & Diffusion**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
 * [Stable Diffusion Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting), which shows how can we implement complicated plugins like `StableDiffusionInpainting` very easily.
 * [Stable Diffusion ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet), which shows how can we decouple complicated workflows like `ControlNet` into separate, lightweight, and reusable plugins very easily.
+* [**Carefree Creator**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/carefree_creator), which contains a free, public-available [demo](https://drawboard-demo.nolibox.com/) of the real world business ready product we are selling. It is a web app with tons of AI magics, but still remains easy for `carefree-drawboard` 🎨 to implement them.
 
 ## Documentation
 
 Check the [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) page for documentation!
 
 ## Status
```

### Comparing `carefree-drawboard-0.0.1a3/README.md` & `carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: carefree-drawboard
+Version: 0.0.1a4
+Summary: 🎨 Infinite Drawboard in Python
+Author: carefree0910
+Author-email: syameimaru.saki@gmail.com
+Keywords: python carefree-learn drawboard
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # carefree-drawboard 🎨
 
 ![Stable Diffusion](examples/assets/stable-diffusion.png)
 
 <div align="center">
 
 <br>
@@ -75,14 +85,15 @@
 
 * [**Getting Started**](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
 * [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins. It also shows how to use the `IPluginGroup` in `carefree-drawboard` 🎨 to group the plugins together and make the UI cleaner.
 * [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common SD plugins.
 * [**Caption & Diffusion**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
 * [Stable Diffusion Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting), which shows how can we implement complicated plugins like `StableDiffusionInpainting` very easily.
 * [Stable Diffusion ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet), which shows how can we decouple complicated workflows like `ControlNet` into separate, lightweight, and reusable plugins very easily.
+* [**Carefree Creator**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/carefree_creator), which contains a free, public-available [demo](https://drawboard-demo.nolibox.com/) of the real world business ready product we are selling. It is a web app with tons of AI magics, but still remains easy for `carefree-drawboard` 🎨 to implement them.
 
 ## Documentation
 
 Check the [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) page for documentation!
 
 ## Status
```

### Comparing `carefree-drawboard-0.0.1a3/carefree_drawboard.egg-info/PKG-INFO` & `carefree-drawboard-0.0.1a4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: carefree-drawboard
-Version: 0.0.1a3
-Summary: 🎨 Infinite Drawboard in Python
-Author: carefree0910
-Author-email: syameimaru.saki@gmail.com
-Keywords: python carefree-learn drawboard
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # carefree-drawboard 🎨
 
 ![Stable Diffusion](examples/assets/stable-diffusion.png)
 
 <div align="center">
 
 <br>
@@ -85,14 +75,15 @@
 
 * [**Getting Started**](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
 * [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins. It also shows how to use the `IPluginGroup` in `carefree-drawboard` 🎨 to group the plugins together and make the UI cleaner.
 * [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common SD plugins.
 * [**Caption & Diffusion**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
 * [Stable Diffusion Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting), which shows how can we implement complicated plugins like `StableDiffusionInpainting` very easily.
 * [Stable Diffusion ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet), which shows how can we decouple complicated workflows like `ControlNet` into separate, lightweight, and reusable plugins very easily.
+* [**Carefree Creator**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/carefree_creator), which contains a free, public-available [demo](https://drawboard-demo.nolibox.com/) of the real world business ready product we are selling. It is a web app with tons of AI magics, but still remains easy for `carefree-drawboard` 🎨 to implement them.
 
 ## Documentation
 
 Check the [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) page for documentation!
 
 ## Status
```

### Comparing `carefree-drawboard-0.0.1a3/carefree_drawboard.egg-info/SOURCES.txt` & `carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -38,35 +38,59 @@
 cfdraw/.web/src/actions/export.ts
 cfdraw/.web/src/actions/i18n.ts
 cfdraw/.web/src/actions/importMeta.ts
 cfdraw/.web/src/actions/managePlugins.ts
 cfdraw/.web/src/actions/manageProjects.ts
 cfdraw/.web/src/actions/update.ts
 cfdraw/.web/src/actions/uploadImage.ts
-cfdraw/.web/src/assets/icon-loading.json
-cfdraw/.web/src/assets/loading-page.json
+cfdraw/.web/src/assets/image-placeholder.svg
+cfdraw/.web/src/assets/nsfw-placeholder.svg
+cfdraw/.web/src/assets/icons/add-blank.svg
+cfdraw/.web/src/assets/icons/add-frame.svg
+cfdraw/.web/src/assets/icons/add-image.svg
+cfdraw/.web/src/assets/icons/add-project.svg
+cfdraw/.web/src/assets/icons/add-text.svg
+cfdraw/.web/src/assets/icons/add.svg
+cfdraw/.web/src/assets/icons/arrange.svg
 cfdraw/.web/src/assets/icons/arrow-down.svg
+cfdraw/.web/src/assets/icons/brush.svg
 cfdraw/.web/src/assets/icons/delete.svg
+cfdraw/.web/src/assets/icons/download.svg
+cfdraw/.web/src/assets/icons/editor.svg
+cfdraw/.web/src/assets/icons/email.svg
+cfdraw/.web/src/assets/icons/github.svg
+cfdraw/.web/src/assets/icons/group-editor.svg
+cfdraw/.web/src/assets/icons/meta.svg
+cfdraw/.web/src/assets/icons/multi-editor.svg
+cfdraw/.web/src/assets/icons/project.svg
+cfdraw/.web/src/assets/icons/redo.svg
+cfdraw/.web/src/assets/icons/settings.svg
+cfdraw/.web/src/assets/icons/shortcuts.svg
+cfdraw/.web/src/assets/icons/undo.svg
+cfdraw/.web/src/assets/icons/wiki.svg
+cfdraw/.web/src/assets/lottie/icon-loading.json
+cfdraw/.web/src/assets/lottie/loading-page.json
 cfdraw/.web/src/components/CFButton.tsx
 cfdraw/.web/src/components/CFCircularProgress.tsx
+cfdraw/.web/src/components/CFColorPicker.tsx
 cfdraw/.web/src/components/CFDivider.tsx
 cfdraw/.web/src/components/CFHeading.tsx
 cfdraw/.web/src/components/CFImageUploader.tsx
 cfdraw/.web/src/components/CFInput.tsx
 cfdraw/.web/src/components/CFLoadingPage.tsx
 cfdraw/.web/src/components/CFLottie.tsx
+cfdraw/.web/src/components/CFMarkdown.tsx
+cfdraw/.web/src/components/CFSelect.tsx
 cfdraw/.web/src/components/CFSlider.tsx
 cfdraw/.web/src/components/CFSwitch.tsx
 cfdraw/.web/src/components/CFText.tsx
 cfdraw/.web/src/components/CFTextarea.tsx
 cfdraw/.web/src/components/CFTooltip.tsx
 cfdraw/.web/src/components/CFIcon/index.scss
 cfdraw/.web/src/components/CFIcon/index.tsx
-cfdraw/.web/src/components/CFSelect/index.scss
-cfdraw/.web/src/components/CFSelect/index.tsx
 cfdraw/.web/src/hooks/useAuth.ts
 cfdraw/.web/src/hooks/useDocumentEvents.ts
 cfdraw/.web/src/hooks/useFileDropper.ts
 cfdraw/.web/src/hooks/useGridLines.ts
 cfdraw/.web/src/hooks/useInitBoard.ts
 cfdraw/.web/src/hooks/usePreventDefaults.ts
 cfdraw/.web/src/hooks/usePython.ts
@@ -81,14 +105,15 @@
 cfdraw/.web/src/lang/settings.ts
 cfdraw/.web/src/lang/toast.ts
 cfdraw/.web/src/lang/tooltip.ts
 cfdraw/.web/src/lang/ui.ts
 cfdraw/.web/src/plugins/index.tsx
 cfdraw/.web/src/plugins/_python/ChatPlugin.tsx
 cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
+cfdraw/.web/src/plugins/_python/MarkdownPlugin.tsx
 cfdraw/.web/src/plugins/_python/PluginGroup.tsx
 cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
 cfdraw/.web/src/plugins/_python/QAPlugin.tsx
 cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
 cfdraw/.web/src/plugins/_python/hooks.ts
 cfdraw/.web/src/plugins/_react/AddPlugin.tsx
 cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx
@@ -96,26 +121,31 @@
 cfdraw/.web/src/plugins/_react/DeletePlugin.tsx
 cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx
 cfdraw/.web/src/plugins/_react/GroupPlugin.tsx
 cfdraw/.web/src/plugins/_react/LinksPlugin.tsx
 cfdraw/.web/src/plugins/_react/MetaPlugin.tsx
 cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx
 cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx
+cfdraw/.web/src/plugins/_react/ShortcutsPlugin.tsx
 cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx
 cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx
 cfdraw/.web/src/plugins/components/Floating.tsx
 cfdraw/.web/src/plugins/components/Link.tsx
 cfdraw/.web/src/plugins/components/Render.tsx
 cfdraw/.web/src/plugins/components/hooks.ts
 cfdraw/.web/src/plugins/components/Fields/BooleanField.tsx
+cfdraw/.web/src/plugins/components/Fields/ColorField.tsx
+cfdraw/.web/src/plugins/components/Fields/Field.tsx
 cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
 cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
 cfdraw/.web/src/plugins/components/Fields/TextField.tsx
 cfdraw/.web/src/plugins/components/Fields/index.tsx
 cfdraw/.web/src/plugins/components/Fields/utils.ts
+cfdraw/.web/src/plugins/components/Fields/ListField/index.scss
+cfdraw/.web/src/plugins/components/Fields/ListField/index.tsx
 cfdraw/.web/src/plugins/utils/cleanup.ts
 cfdraw/.web/src/plugins/utils/factory.ts
 cfdraw/.web/src/plugins/utils/renderFilters.ts
 cfdraw/.web/src/requests/actions.ts
 cfdraw/.web/src/requests/hooks.ts
 cfdraw/.web/src/requests/interceptors/_python.ts
 cfdraw/.web/src/requests/interceptors/index.ts
@@ -168,14 +198,13 @@
 cfdraw/schema/__init__.py
 cfdraw/schema/fields.py
 cfdraw/schema/plugins.py
 cfdraw/schema/settings.py
 cfdraw/utils/__init__.py
 cfdraw/utils/cache.py
 cfdraw/utils/console.py
-cfdraw/utils/data_structures.py
 cfdraw/utils/exec.py
 cfdraw/utils/misc.py
 cfdraw/utils/prerequisites.py
 cfdraw/utils/processes.py
 cfdraw/utils/server.py
 cfdraw/utils/template.py
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/index.html` & `carefree-drawboard-0.0.1a4/cfdraw/.web/index.html`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/package.json` & `carefree-drawboard-0.0.1a4/cfdraw/.web/package.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9734693877551022%*

 * *Differences: {"'dependencies'": "{'@carefree0910/business': '~0.5.1-alpha.12', '@carefree0910/core': "*

 * *                   "'~0.5.1-alpha.12', '@carefree0910/native': '~0.5.1-alpha.12', "*

 * *                   "'@carefree0910/svg': '~0.5.1-alpha.12', 'chakra-react-select': '^4.6.0', "*

 * *                   "'react-color': '^2.19.3', 'react-markdown': '^8.0.7', 'react-select': "*

 * *                   "'^5.7.3', 'react-syntax-highlighter': '^15.5.0', 'remark-gfm': '^3.0.1'}",*

 * * "'devDependencies'": "{'@types/react-color': '^3.0.6',  […]*

```diff
@@ -1,44 +1,52 @@
 {
     "dependencies": {
-        "@carefree0910/business": "~0.5.1-alpha.8",
-        "@carefree0910/core": "~0.5.1-alpha.8",
-        "@carefree0910/native": "~0.5.1-alpha.8",
-        "@carefree0910/svg": "~0.5.1-alpha.8",
+        "@carefree0910/business": "~0.5.1-alpha.12",
+        "@carefree0910/core": "~0.5.1-alpha.12",
+        "@carefree0910/native": "~0.5.1-alpha.12",
+        "@carefree0910/svg": "~0.5.1-alpha.12",
         "@chakra-ui/icons": "^2.0.4",
         "@chakra-ui/react": "^2.2.4",
         "@emotion/react": "^11.9.3",
         "@emotion/styled": "^11.9.3",
         "@svgdotjs/svg.filter.js": "^3.0.8",
         "@svgdotjs/svg.js": "^3.1.1",
         "@svgdotjs/svg.topath.js": "^2.0.3",
         "@svgdotjs/svg.topoly.js": "^1.0.3",
         "ahooks": "^3.7.6",
         "axios": "^1.3.4",
+        "chakra-react-select": "^4.6.0",
         "classnames": "^2.3.2",
         "eslint": "8.37.0",
         "eslint-config-next": "13.2.4",
         "framer-motion": "^10.10.0",
         "jszip": "^3.7.1",
         "lottie-web": "^5.11.0",
         "ml-matrix": "^6.10.0",
         "mobx": "6.6.1",
         "mobx-react-lite": "^3.4.0",
         "next": "13.2.4",
         "platform": "^1.3.6",
         "rc-upload": "^4.3.4",
         "react": "18.2.0",
+        "react-color": "^2.19.3",
         "react-dom": "18.2.0",
+        "react-markdown": "^8.0.7",
+        "react-select": "^5.7.3",
+        "react-syntax-highlighter": "^15.5.0",
+        "remark-gfm": "^3.0.1",
         "uuid": "^9.0.0"
     },
     "devDependencies": {
         "@total-typescript/ts-reset": "^0.4.2",
         "@types/node": "18.15.11",
         "@types/react": "18.0.33",
+        "@types/react-color": "^3.0.6",
         "@types/react-dom": "18.0.11",
+        "@types/react-syntax-highlighter": "^15.5.6",
         "@types/uuid": "^9.0.1",
         "@vitejs/plugin-react": "^3.1.0",
         "rollup-plugin-visualizer": "^5.9.0",
         "sass": "^1.60.0",
         "typescript": "^5.0.3",
         "vite": "^4.2.0",
         "vite-plugin-svgr": "^2.4.0",
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/App.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/App.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/BoardPanel.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/BoardPanel.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/addImage.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/addImage.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/addText.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/addText.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/arrange.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/arrange.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/download.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/export.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/export.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/importMeta.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/importMeta.ts`

 * *Files 0% similar despite different names*

```diff
@@ -134,18 +134,18 @@
   res: R;
   alias: string;
   rectangle: RectangleShapeNode;
   metaData: IPythonFieldsMetaData;
 }
 function consumePythonFields({ type, metaData }: IImportMeta<"python.fields">): void {
   const success = async () => {
-    toastWord("success", Toast_Words["generate-image-success-message"]);
+    toastWord("success", Toast_Words["generate-success-message"]);
   };
   const failed = async (err: any) => {
-    toastWord("error", Toast_Words["post-python-http-fields-plugin-error-message"], {
+    toastWord("error", Toast_Words["post-python-fields-plugin-error-message"], {
       appendix: ` (${err})`,
     });
   };
   const getNewAlias = () => `${type}.${metaData.identifier}.${getRandomHash()}`;
   function gatherPacks<T extends IPythonResults>(
     results: T,
     getRectangleInfo: (res: T["value"][number]) => INewRectangle,
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/managePlugins.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/managePlugins.ts`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,63 @@
 import { runInAction } from "mobx";
 
-import type { AllPlugins } from "@/schema/plugins";
+import type { ReactPlugins } from "@/schema/plugins";
 import { reactPluginSettings } from "@/_settings";
 import { usePythonPluginSettings } from "@/stores/settings";
 import {
   setPluginExpanded,
   usePluginsExpanded,
   setReactPluginVisible,
   setPythonPluginVisible,
+  usePluginIds,
 } from "@/stores/pluginsInfo";
 
-function setAllPluginVisible(visible: boolean, except?: AllPlugins[]) {
+interface IExcepts {
+  exceptReactPlugins?: ReactPlugins[];
+  exceptIdentifiers?: string[];
+}
+
+function setAllPluginVisible(visible: boolean, opt?: IExcepts) {
+  opt ??= {};
   runInAction(() => {
     reactPluginSettings.forEach(({ type }) => {
-      if (except?.includes(type)) return;
+      if (opt?.exceptReactPlugins?.includes(type)) return;
       if (!["settings", "undo", "redo"].includes(type)) {
         setReactPluginVisible(type, visible);
       }
     });
     usePythonPluginSettings().forEach(({ props }) => {
       const identifier = props.pluginInfo.identifier;
-      if (except?.includes(identifier)) return;
+      if (opt?.exceptIdentifiers?.includes(identifier)) return;
       setPythonPluginVisible(identifier, visible);
     });
   });
 }
 
-export function collapseAllPlugins(opt?: { except?: AllPlugins[] }) {
+export function collapseAllPlugins(opt?: IExcepts) {
   runInAction(() => {
     Object.keys(usePluginsExpanded()).forEach((id) => {
-      if (opt?.except && opt.except.some((e) => id.startsWith(e))) return;
+      if (
+        opt?.exceptReactPlugins &&
+        opt.exceptReactPlugins.some((type) => usePluginIds(type, false).id === id)
+      ) {
+        return;
+      }
+      if (
+        opt?.exceptIdentifiers &&
+        opt.exceptIdentifiers.some((identifier) => usePluginIds(identifier, false).id === id)
+      ) {
+        return;
+      }
       setPluginExpanded(id, false);
     });
   });
 }
-export function hideAllPlugins(opt?: { except?: AllPlugins[] }) {
+export function hideAllPlugins(opt?: IExcepts) {
   // collapse all plugins first
   collapseAllPlugins(opt);
   // then hide all plugins
-  setAllPluginVisible(false, opt?.except);
+  setAllPluginVisible(false, opt);
 }
 export function showAllPlugins() {
   setAllPluginVisible(true);
 }
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/manageProjects.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/manageProjects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/actions/uploadImage.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/uploadImage.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/assets/icon-loading.json` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/lottie/icon-loading.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/assets/icons/delete.svg` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/delete.svg`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-00000000: 3c73 7667 2078 6d6c 6e73 3d22 6874 7470  <svg xmlns="http
-00000010: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
-00000020: 3030 2f73 7667 2220 7769 6474 683d 2233  00/svg" width="3
-00000030: 3222 2068 6569 6768 743d 2233 3222 2076  2" height="32" v
-00000040: 6965 7742 6f78 3d22 3020 3020 3332 2033  iewBox="0 0 32 3
-00000050: 3222 2066 696c 6c3d 226e 6f6e 6522 3e0d  2" fill="none">.
+00000000: 3c73 7667 2077 6964 7468 3d22 3332 2220  <svg width="32" 
+00000010: 6865 6967 6874 3d22 3332 2220 7669 6577  height="32" view
+00000020: 426f 783d 2230 2030 2033 3220 3332 2220  Box="0 0 32 32" 
+00000030: 6669 6c6c 3d22 6e6f 6e65 2220 786d 6c6e  fill="none" xmln
+00000040: 733d 2268 7474 703a 2f2f 7777 772e 7733  s="http://www.w3
+00000050: 2e6f 7267 2f32 3030 302f 7376 6722 3e0d  .org/2000/svg">.
 00000060: 0a3c 7061 7468 2064 3d22 4d32 3720 3748  .<path d="M27 7H
 00000070: 3522 2073 7472 6f6b 653d 2223 4535 3137  5" stroke="#E517
 00000080: 3137 2220 7374 726f 6b65 2d77 6964 7468  17" stroke-width
 00000090: 3d22 3222 2073 7472 6f6b 652d 6c69 6e65  ="2" stroke-line
 000000a0: 6361 703d 2272 6f75 6e64 2220 7374 726f  cap="round" stro
 000000b0: 6b65 2d6c 696e 656a 6f69 6e3d 2272 6f75  ke-linejoin="rou
 000000c0: 6e64 222f 3e0d 0a3c 7061 7468 2064 3d22  nd"/>..<path d="
@@ -51,8 +51,8 @@
 00000320: 3131 2e32 3130 3720 332e 3936 3038 3620  11.2107 3.96086 
 00000330: 3131 2034 2e34 3639 3537 2031 3120 3556  11 4.46957 11 5V
 00000340: 3722 2073 7472 6f6b 653d 2223 4535 3137  7" stroke="#E517
 00000350: 3137 2220 7374 726f 6b65 2d77 6964 7468  17" stroke-width
 00000360: 3d22 3222 2073 7472 6f6b 652d 6c69 6e65  ="2" stroke-line
 00000370: 6361 703d 2272 6f75 6e64 2220 7374 726f  cap="round" stro
 00000380: 6b65 2d6c 696e 656a 6f69 6e3d 2272 6f75  ke-linejoin="rou
-00000390: 6e64 222f 3e0d 0a3c 2f73 7667 3e         nd"/>..</svg>
+00000390: 6e64 222f 3e0d 0a3c 2f73 7667 3e0d 0a    nd"/>..</svg>..
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/assets/loading-page.json` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/lottie/loading-page.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFButton.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFButton.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import { observer } from "mobx-react-lite";
 import { useState, useCallback } from "react";
 import { Box, Button, ButtonProps, Image, ImageProps } from "@chakra-ui/react";
 
-import iconLoading from "@/assets/icon-loading.json";
+import iconLoading from "@/assets/lottie/icon-loading.json";
+
 import { Event } from "@/utils/event";
-import { VISIBILITY_TRANSITION } from "@/utils/constants";
+import { makeVisibilityTransitionProps } from "@/utils/constants";
 import { themeStore } from "@/stores/theme";
 import { settingsStore } from "@/stores/settings";
 import CFLottie from "./CFLottie";
 import CFTooltip from "./CFTooltip";
 
 function CFButton(props: ButtonProps) {
   const { textColor } = themeStore.styles;
@@ -59,18 +60,20 @@
       <CFTooltip label={tooltip}>
         <Box as="button" id={id} {...others}>
           <Image
             src={src}
             w="100%"
             h="100%"
             draggable={false}
-            visibility={iconLoaded ? "visible" : "hidden"}
-            transition={VISIBILITY_TRANSITION}
             onLoad={onIconLoaded}
             {...imageProps}
+            {...makeVisibilityTransitionProps({
+              visible: iconLoaded,
+              opacity: imageProps?.opacity,
+            })}
           />
           {children}
           <CFLottie
             w="100%"
             h="100%"
             position="absolute"
             left="0px"
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFCircularProgress.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFCircularProgress.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFIcon/index.scss` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFIcon/index.scss`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFIcon/index.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFIcon/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFImageUploader.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFImageUploader.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFLoadingPage.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFLoadingPage.tsx`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import React, { PropsWithChildren } from "react";
 import { observer } from "mobx-react-lite";
 import { Center, Flex, Spacer } from "@chakra-ui/react";
 
 import { useIsReady } from "@carefree0910/business";
 
-import loadingPage from "@/assets/loading-page.json";
-import { makeVisiblilityTransition } from "@/utils/constants";
+import loadingPage from "@/assets/lottie/loading-page.json";
+
+import { makeVisibilityTransitionProps } from "@/utils/constants";
 import { useSettingsSynced } from "@/stores/settings";
 import { themeStore } from "@/stores/theme";
 import { useIsAllReady } from "@/hooks/useSetup";
 import CFLottie from "./CFLottie";
 
 const CFLoadingPage: React.FC<PropsWithChildren> = ({ children }) => {
   const isReady = useIsReady() && useIsAllReady();
@@ -24,17 +25,15 @@
           w="100%"
           h="100%"
           bg={boardBg}
           zIndex="1000"
           position="absolute"
           direction="column"
           alignContent="center"
-          opacity={isReady ? 0 : 1}
-          visibility={isReady ? "hidden" : "visible"}
-          transition={makeVisiblilityTransition(0.5)}>
+          {...makeVisibilityTransitionProps({ visible: !isReady, second: 0.5 })}>
           <Spacer />
           <Center>
             <CFLottie hide={!isSynced} animationData={loadingPage} />
           </Center>
           <Spacer />
         </Flex>
       )}
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFLottie.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFLottie.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFSlider.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFSlider.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import { observer } from "mobx-react-lite";
 import { useUnmount } from "ahooks";
 import React, { useCallback, useEffect, useState } from "react";
 
 import { BoardStore, useGlobalTransform, useIsReady } from "@carefree0910/business";
 
 import { themeStore } from "@/stores/theme";
-import { CFCaption } from "./CFText";
+import { CFLabel } from "./CFText";
 import CFInput from "./CFInput";
 import CFTooltip from "./CFTooltip";
 
 export interface ICFSlider extends FlexProps {
   className?: string;
   min: number;
   max: number;
@@ -119,26 +119,28 @@
       if (value.toString() !== inputVal) {
         setInputVal(value.toFixed(precision).toString());
       }
     }
   }, [value]);
 
   useUnmount(() => {
-    handleInputBlur(+inputVal);
+    if (value.toString() !== inputVal) {
+      handleInputBlur(+inputVal);
+    }
   });
 
   const {
     textColor,
     sliderColors: { sliderTrackColor, sliderThumbBorderColor, inputBgColor },
   } = themeStore.styles;
 
   return (
     <Flex className={className} align="center" color={textColor} {...props}>
       <CFTooltip label={tooltip}>
-        <CFCaption label={label} />
+        <CFLabel label={label} />
       </CFTooltip>
       <Slider
         focusThumbOnChange={!iptFocused}
         flex={1}
         h="32px"
         mx="1em"
         value={scale === "linear" ? val : Math.log(val + offset)}
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFSwitch.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFSwitch.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import { observer } from "mobx-react-lite";
 import { useMemo, ReactElement } from "react";
 import {
-  FlexProps,
   FormControl,
+  FormControlProps,
   FormLabel,
   FormLabelProps,
   Spacer,
   Switch,
 } from "@chakra-ui/react";
 
 import { getRandomHash } from "@carefree0910/core";
 
 import { themeStore } from "@/stores/theme";
-import CFTooltip from "./CFTooltip";
+import CFTooltip, { CFFormLabel } from "./CFTooltip";
 
-interface ICFSwitch extends FlexProps {
+interface ICFSwitch extends FormControlProps {
   label: string;
   value: boolean;
   setValue: (value: boolean) => void;
   tooltip?: ReactElement;
   disableSwitch?: boolean;
   formLabelProps?: FormLabelProps;
 }
@@ -29,31 +29,25 @@
   tooltip,
   disableSwitch,
   formLabelProps,
   ...props
 }: ICFSwitch) {
   const hashId = useMemo(() => getRandomHash().toString(), []);
   const {
-    textColor,
     switchColors: { checkedBgColor, uncheckedBgColor },
   } = themeStore.styles;
 
   return (
     <FormControl display="flex" alignItems="center" {...props}>
-      <CFTooltip label={tooltip}>
-        <FormLabel
-          mb="0"
-          color={textColor}
-          fontSize={props.fontSize ?? "14px"}
-          htmlFor={hashId}
-          userSelect="none"
-          {...formLabelProps}>
-          {label}
-        </FormLabel>
-      </CFTooltip>
+      <CFFormLabel
+        label={label}
+        tooltip={{ label: tooltip }}
+        {...formLabelProps}
+        htmlFor={hashId}
+      />
       <Spacer />
       <Switch
         id={hashId}
         sx={{
           "span.chakra-switch__track": { backgroundColor: checkedBgColor },
           "span.chakra-switch__track:not([data-checked])": { backgroundColor: uncheckedBgColor },
         }}
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/components/CFText.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFText.tsx`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import { themeStore } from "@/stores/theme";
 
 const CFText = forwardRef(function (props: TextProps, ref) {
   const { textColor } = themeStore.styles;
 
   return <Text ref={ref} color={textColor} {...props} />;
 });
-export const CFCaption = observer(
+export const CFLabel = observer(
   forwardRef(function ({ label, ...props }: TextProps & { label?: string }, ref) {
     return (
       <>
         {label && (
           <CFText minW="20%" align="center" fontSize="14px" flexShrink={0} {...props} ref={ref}>
             {label}
           </CFText>
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/useAuth.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useAuth.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/useDocumentEvents.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useDocumentEvents.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 import { useEffect } from "react";
 import { makeObservable, observable } from "mobx";
 
 import { isUndefined } from "@carefree0910/core";
 import { ABCStore, BoardStore, useIsReady } from "@carefree0910/business";
 
+import type { ReactPlugins } from "@/schema/plugins";
+import { useReactPluginSettings } from "@/_settings";
+import { usePythonPluginSettings } from "@/stores/settings";
 import { setPluginExpanded, usePluginParent, usePluginsExpanded } from "@/stores/pluginsInfo";
 import { collapseAllPlugins } from "@/actions/managePlugins";
 
 // helpers
 
 function smartCollapse(): void {
   const currentExpanded = usePluginsExpanded();
   const expanding = Object.keys(currentExpanded).find((key) => currentExpanded[key]);
-  collapseAllPlugins({ except: ["brush"] });
+  collapseAllPlugins({
+    exceptReactPlugins: (["brush"] as ReactPlugins[]).concat(
+      useReactPluginSettings()
+        .filter((s) => s.props.renderInfo.keepOpen)
+        .map((s) => s.type),
+    ),
+    exceptIdentifiers: usePythonPluginSettings()
+      .filter((s) => s.props.renderInfo.keepOpen)
+      .map((s) => s.props.pluginInfo.identifier),
+  });
   if (!isUndefined(expanding)) {
     const parent = usePluginParent(expanding);
     if (!isUndefined(parent)) {
       setPluginExpanded(parent, true);
     }
   }
 }
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/useFileDropper.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useFileDropper.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/useGridLines.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useGridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/useInitBoard.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useInitBoard.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/usePreventDefaults.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/usePreventDefaults.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/usePython.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/usePython.ts`

 * *Files 7% similar despite different names*

```diff
@@ -99,29 +99,31 @@
 }
 export async function getPythonRequest({
   node,
   nodes,
   identifier,
   getExtraRequestData,
   opt = {},
+  needExportNodeData,
 }: Omit<IUsePythonInfo, "isInvisible"> & {
   opt?: IGetPythonRequest;
 }): Promise<Omit<IPythonSocketRequest, "hash">> {
   let exportBox: BBox | undefined;
   if (!opt.noExport) {
     exportBox =
       nodes.length === 0
         ? node?.bbox ?? BBox.unit()
         : nodes.length === 1
         ? nodes[0].bbox
         : nodes[argMax(nodes.map((n) => n.bbox.area))].bbox;
   }
   const getNodeDataOpt: IGetNodeData = { exportBox, ...opt };
-  const nodeData = await getNodeData(node, getNodeDataOpt);
-  const nodeDataList = nodes.length <= 1 ? [] : await getNodeDataList(nodes, getNodeDataOpt);
+  const nodeData = needExportNodeData ? await getNodeData(node, getNodeDataOpt) : {};
+  const nodeDataList =
+    !needExportNodeData || nodes.length <= 1 ? [] : await getNodeDataList(nodes, getNodeDataOpt);
   return {
     userId: userStore.userId,
     baseURL: getBaseURL(),
     identifier,
     nodeData,
     nodeDataList,
     extraData: getExtraRequestData ? getExtraRequestData() : {},
@@ -140,14 +142,15 @@
   identifier,
   isInvisible,
   retryInterval,
   updateInterval,
   getExtraRequestData,
   onMessage,
   onSocketError,
+  needExportNodeData,
 }: IUseSocketPython<R>) {
   const deps = [
     hash,
     node?.alias,
     nodes.map((n) => n.alias).join("_"),
     identifier,
     retryInterval,
@@ -159,14 +162,15 @@
   const getMessage = useCallback(
     () =>
       getPythonRequest({
         node,
         nodes,
         identifier,
         getExtraRequestData,
+        needExportNodeData,
       }).then((req) => ({ hash: hash!, ...req })),
     [deps],
   );
 
   const requestFn = useCallback(() => {
     useWebSocketHook({
       isInvisible,
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/hooks/useSetup.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useSetup.ts`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,16 @@
 //// update settings, return `true` if settings hash is changed (which means rerendering is needed)
 const updateSettings = (data: ISettingsStore): boolean => {
   const incomingHash = getHash(JSON.stringify(data)).toString();
   if (settingsStore.hash === incomingHash) return false;
   runInAction(async () => {
     settingsStore.hash = incomingHash;
     settingsStore.pluginSettings = data.pluginSettings;
+    // `extraPlugins` should be updated every time to enable hot reload.
+    settingsStore.extraPlugins = data.extraPlugins;
     // `internalSettings` should only be updated once.
     if (!settingsStore.internalSettings) {
       settingsStore.internalSettings = data.internalSettings;
     }
     // `boardSettings` should only be updated once.
     if (!settingsStore.boardSettings) {
       if (!data.boardSettings) return;
@@ -202,15 +204,15 @@
         nodeDataList: [],
         extraData: {},
         isInternal: true,
       }),
     [],
   );
   const onMessage = useCallback<IPythonOnSocketMessage<ISettingsStore>>(
-    async ({ status, total, pending, message, data: { progress, final } }) => {
+    async ({ status, total, pending, message, data: { final } }) => {
       collapseAllPlugins();
       if (status !== "finished") {
         if (status === "pending") {
           Logger.warn(`sync pending: ${pending} / ${total}`);
         } else if (status === "working") {
           // Logger.warn(`sync in progress: ${progress}`);
         } else {
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/add.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/add.ts`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 
 export enum Add_Words {
   "add-plugin-header" = "add-plugin-header",
   "new-project-button" = "new-project-button",
   "upload-image-button" = "upload-image-button",
   "add-text-button" = "add-text-button",
   "add-blank-button" = "add-blank-button",
+  "add-frame-button" = "add-frame-button",
 }
 
 export const addLangRecords: Record<Lang, Record<Add_Words, string>> = {
   zh: {
     [Add_Words["add-plugin-header"]]: "添加",
     [Add_Words["new-project-button"]]: "新建项目",
     [Add_Words["upload-image-button"]]: "上传图片",
     [Add_Words["add-text-button"]]: "添加文字",
     [Add_Words["add-blank-button"]]: "添加空白画布",
+    [Add_Words["add-frame-button"]]: "添加画框",
   },
   en: {
     [Add_Words["add-plugin-header"]]: "Add",
     [Add_Words["new-project-button"]]: "New Project",
     [Add_Words["upload-image-button"]]: "Upload Image",
     [Add_Words["add-text-button"]]: "Add Text",
     [Add_Words["add-blank-button"]]: "Add Blank Canvas",
+    [Add_Words["add-frame-button"]]: "Add Frame",
   },
 };
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/brush.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/brush.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/download.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/index.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/plugins.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/plugins.ts`

 * *Files 6% similar despite different names*

```diff
@@ -10,48 +10,54 @@
     add: "添加",
     arrange: "智能整理",
     undo: "撤销",
     redo: "重做",
     download: "下载",
     delete: "删除",
     wiki: "文档",
-    github: "Github",
     email: "邮件",
+    github: "Github",
+    shortcuts: "快捷键",
+    logo: "Logo",
     textEditor: "编辑文本",
     groupEditor: "编辑组",
     multiEditor: "编辑多节点",
     brush: "画笔",
+    "_python.pluginGroup": "Python 插件组",
     "_python.fields": "Python 插件",
     "_python.textArea": "Python 文本框",
     "_python.QA": "Python 问答",
     "_python.chat": "Python 对话",
-    "_python.pluginGroup": "Python 插件组",
+    "_python.markdown": "Python Markdown",
   },
   en: {
     meta: "Meta",
     settings: "Settings",
     project: "Project",
     add: "Add",
     arrange: "Auto Arrange",
     undo: "Undo",
     redo: "Redo",
     download: "Download",
     delete: "Delete",
     wiki: "Wiki",
-    github: "Github",
     email: "Email",
+    github: "Github",
+    shortcuts: "Shortcuts",
+    logo: "Logo",
     textEditor: "Edit Text",
     groupEditor: "Edit Group",
     multiEditor: "Edit Multi Nodes",
     brush: "Brush",
+    "_python.pluginGroup": "Python Plugin Group",
     "_python.fields": "Python Plugin",
     "_python.textArea": "Python TextArea",
     "_python.QA": "Python Q & A",
     "_python.chat": "Python Chat",
-    "_python.pluginGroup": "Python Plugin Group",
+    "_python.markdown": "Python Markdown",
   },
 };
 
 export const Plugins_Words: Record<AllPlugins, string> = {} as any;
 export const pluginsLangRecords: Dictionary<Dictionary<string>> = {};
 
 function injectScope(scope: string, data: Dictionary<string>) {
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/projects.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/settings.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/settings.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/toast.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/toast.ts`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 
 export enum Toast_Words {
   "dropping-message" = "dropping-message",
   "uploading-image-message" = "uploading-image-message",
   "upload-image-success-message" = "upload-image-success-message",
   "upload-image-error-message" = "upload-image-error-message",
   "strange-image-error-message" = "strange-image-error-message",
-  "generate-image-success-message" = "generate-image-success-message",
-  "generate-image-error-message" = "generate-image-error-message",
-  "post-python-http-fields-plugin-error-message" = "post-python-http-fields-plugin-error-message",
+  "generate-success-message" = "generate-success-message",
+  "post-python-fields-plugin-error-message" = "post-python-fields-plugin-error-message",
   "uploading-project-message" = "uploading-project-message",
   "adding-project-message" = "adding-project-message",
   "add-project-success-message" = "add-project-success-message",
   "save-project-success-message" = "save-project-success-message",
   "save-project-error-message" = "save-project-error-message",
   "loading-project-message" = "loading-project-message",
   "load-project-success-message" = "load-project-success-message",
@@ -27,14 +26,16 @@
   "import-local-project-error-message" = "import-local-project-error-message",
   "delete-project-success-message" = "delete-project-success-message",
   "delete-project-error-message" = "delete-project-error-message",
   "add-text-success-message" = "add-text-success-message",
   "add-text-error-message" = "add-text-error-message",
   "add-blank-success-message" = "add-blank-success-message",
   "add-blank-error-message" = "add-blank-error-message",
+  "add-frame-success-message" = "add-frame-success-message",
+  "add-frame-error-message" = "add-frame-error-message",
   "auto-arrange-no-need-message" = "auto-arrange-no-need-message",
   "submit-task-busy-message" = "submit-task-busy-message",
   "submit-task-success-message" = "submit-task-success-message",
   "submit-task-error-message" = "submit-task-error-message",
   "submit-task-interrupted-message" = "submit-task-interrupted-message",
   "submit-task-finished-message" = "submit-task-finished-message",
   "downloading-nodes-message" = "downloading-nodes-message",
@@ -49,17 +50,16 @@
 export const toastLangRecords: Record<Lang, Record<Toast_Words, string>> = {
   zh: {
     [Toast_Words["dropping-message"]]: "识别中",
     [Toast_Words["uploading-image-message"]]: "上传中，请稍候",
     [Toast_Words["upload-image-success-message"]]: "上传图片成功",
     [Toast_Words["upload-image-error-message"]]: "上传图片失败",
     [Toast_Words["strange-image-error-message"]]: "图片类型错误，当前仅支持上传 jpg/png 图片",
-    [Toast_Words["generate-image-success-message"]]: "生成图片成功",
-    [Toast_Words["generate-image-error-message"]]: "生成图片失败",
-    [Toast_Words["post-python-http-fields-plugin-error-message"]]: "请求 Python 服务时失败",
+    [Toast_Words["generate-success-message"]]: "生成成功",
+    [Toast_Words["post-python-fields-plugin-error-message"]]: "请求 Python 服务时失败",
     [Toast_Words["uploading-project-message"]]: "保存项目中",
     [Toast_Words["adding-project-message"]]: "新建项目中",
     [Toast_Words["add-project-success-message"]]: "新建项目成功",
     [Toast_Words["save-project-success-message"]]: "保存项目成功",
     [Toast_Words["save-project-error-message"]]: "保存项目失败",
     [Toast_Words["loading-project-message"]]: "加载项目中，请稍候",
     [Toast_Words["load-project-success-message"]]: "加载项目成功",
@@ -74,14 +74,16 @@
     [Toast_Words["import-local-project-error-message"]]: "导入失败",
     [Toast_Words["delete-project-success-message"]]: "删除项目成功",
     [Toast_Words["delete-project-error-message"]]: "删除项目失败",
     [Toast_Words["add-text-success-message"]]: "添加文字成功",
     [Toast_Words["add-text-error-message"]]: "添加文字时出了些问题",
     [Toast_Words["add-blank-success-message"]]: "添加空白画布成功",
     [Toast_Words["add-blank-error-message"]]: "添加空白画布时出了些问题",
+    [Toast_Words["add-frame-success-message"]]: "添加画框成功",
+    [Toast_Words["add-frame-error-message"]]: "添加画框时出了些问题",
     [Toast_Words["auto-arrange-no-need-message"]]: "当前节点无需整理",
     [Toast_Words["submit-task-busy-message"]]: "当前任务正在执行中，请稍候...",
     [Toast_Words["submit-task-success-message"]]: "任务提交成功",
     [Toast_Words["submit-task-error-message"]]: "执行任务时出了些问题",
     [Toast_Words["submit-task-interrupted-message"]]: "任务执行被中断",
     [Toast_Words["submit-task-finished-message"]]: "任务已执行完成",
     [Toast_Words["downloading-nodes-message"]]: "下载中",
@@ -94,17 +96,16 @@
   },
   en: {
     [Toast_Words["dropping-message"]]: "Detecting",
     [Toast_Words["uploading-image-message"]]: "Uploading, please wait for a while",
     [Toast_Words["upload-image-success-message"]]: "Image uploaded successfully!",
     [Toast_Words["upload-image-error-message"]]: "Upload image failed",
     [Toast_Words["strange-image-error-message"]]: "Only jpg/png images are supported",
-    [Toast_Words["generate-image-success-message"]]: "Image generated successfully!",
-    [Toast_Words["generate-image-error-message"]]: "Generate image failed",
-    [Toast_Words["post-python-http-fields-plugin-error-message"]]: "Request Python service failed",
+    [Toast_Words["generate-success-message"]]: "Generated successfully!",
+    [Toast_Words["post-python-fields-plugin-error-message"]]: "Request Python service failed",
     [Toast_Words["uploading-project-message"]]: "Saving",
     [Toast_Words["adding-project-message"]]: "Creating new project",
     [Toast_Words["add-project-success-message"]]: "Project created successfully!",
     [Toast_Words["save-project-success-message"]]: "Project saved successfully!",
     [Toast_Words["save-project-error-message"]]: "Save project failed",
     [Toast_Words["loading-project-message"]]: "Loading",
     [Toast_Words["load-project-success-message"]]: "Project loaded successfully!",
@@ -120,14 +121,16 @@
     [Toast_Words["import-local-project-error-message"]]: "Import failed",
     [Toast_Words["delete-project-success-message"]]: "Project deleted successfully!",
     [Toast_Words["delete-project-error-message"]]: "Delete project failed",
     [Toast_Words["add-text-success-message"]]: "Text added successfully",
     [Toast_Words["add-text-error-message"]]: "Something is wrong when adding Text Node",
     [Toast_Words["add-blank-success-message"]]: "Blank Canvas added successfully",
     [Toast_Words["add-blank-error-message"]]: "Something is wrong when adding Blank Canvas",
+    [Toast_Words["add-frame-success-message"]]: "Frame added successfully",
+    [Toast_Words["add-frame-error-message"]]: "Something is wrong when adding Frame",
     [Toast_Words["auto-arrange-no-need-message"]]: "There is no need to arrange the Nodes",
     [Toast_Words["submit-task-busy-message"]]:
       "Current task is being executed, please wait for a while...",
     [Toast_Words["submit-task-success-message"]]: "Task submitted successfully!",
     [Toast_Words["submit-task-error-message"]]: "Something is wrong when executing the task",
     [Toast_Words["submit-task-interrupted-message"]]: "Task submission is interrupted",
     [Toast_Words["submit-task-finished-message"]]: "Task has been executed successfully",
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/lang/tooltip.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/tooltip.ts`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,17 @@
   "undo-tooltip" = "undo-tooltip",
   "redo-tooltip" = "redo-tooltip",
   "text-editor-tooltip" = "text-editor-tooltip",
   "ungroup-the-nodes-tooltip" = "ungroup-the-nodes-tooltip",
   "group-the-nodes-tooltip" = "group-the-nodes-tooltip",
   "auto-arrange-tooltip" = "auto-arrange-tooltip",
   "wiki-tooltip" = "wiki-tooltip",
-  "github-tooltip" = "github-tooltip",
   "email-tooltip" = "email-tooltip",
+  "github-tooltip" = "github-tooltip",
+  "shortcuts-tooltip" = "shortcuts-tooltip",
 }
 
 export const tooltipLangRecords: Record<Lang, Record<Tooltip_Words, string>> = {
   zh: {
     [Tooltip_Words["settings-tooltip"]]: "设置",
     [Tooltip_Words["project-management-tooltip"]]: "项目管理",
     [Tooltip_Words["add-new-stuff-tooltip"]]: "添加新的元素",
@@ -25,26 +26,28 @@
     [Tooltip_Words["undo-tooltip"]]: "撤销",
     [Tooltip_Words["redo-tooltip"]]: "重做",
     [Tooltip_Words["text-editor-tooltip"]]: "文本编辑器",
     [Tooltip_Words["ungroup-the-nodes-tooltip"]]: "解组",
     [Tooltip_Words["group-the-nodes-tooltip"]]: "打组",
     [Tooltip_Words["auto-arrange-tooltip"]]: "自动排列",
     [Tooltip_Words["wiki-tooltip"]]: "Wiki",
-    [Tooltip_Words["github-tooltip"]]: "Github",
     [Tooltip_Words["email-tooltip"]]: "Email",
+    [Tooltip_Words["github-tooltip"]]: "Github",
+    [Tooltip_Words["shortcuts-tooltip"]]: "快捷键",
   },
   en: {
     [Tooltip_Words["settings-tooltip"]]: "Settings",
     [Tooltip_Words["project-management-tooltip"]]: "Project Management",
     [Tooltip_Words["add-new-stuff-tooltip"]]: "Add new stuff",
     [Tooltip_Words["enter-sketch-mode-tooltip"]]: "Enter Sketch Mode",
     [Tooltip_Words["undo-tooltip"]]: "Undo",
     [Tooltip_Words["redo-tooltip"]]: "Redo",
     [Tooltip_Words["text-editor-tooltip"]]: "Text Editor",
     [Tooltip_Words["ungroup-the-nodes-tooltip"]]: "Ungroup the Nodes",
     [Tooltip_Words["group-the-nodes-tooltip"]]: "Group the Nodes",
     [Tooltip_Words["auto-arrange-tooltip"]]: "Auto Arrange",
     [Tooltip_Words["wiki-tooltip"]]: "Wiki",
-    [Tooltip_Words["github-tooltip"]]: "Github",
     [Tooltip_Words["email-tooltip"]]: "Email",
+    [Tooltip_Words["github-tooltip"]]: "Github",
+    [Tooltip_Words["shortcuts-tooltip"]]: "Shortcuts",
   },
 };
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_python/ChatPlugin.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/ChatPlugin.tsx`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import { usePluginIds } from "@/stores/pluginsInfo";
 import { parseIStr } from "@/actions/i18n";
 import CFInput from "@/components/CFInput";
 import { drawboardPluginFactory } from "@/plugins/utils/factory";
 import PythonPluginWithSubmit from "./PluginWithSubmit";
 
 const PythonChatPlugin = ({ pluginInfo, ...props }: IPythonQAPlugin) => {
-  const { id } = usePluginIds(`Chat_${pluginInfo.identifier}`);
+  const id = usePluginIds(`Chat_${pluginInfo.identifier}`).id;
   const [context, setContext] = useState(parseIStr(pluginInfo.initialText));
   const [userInput, setUserInput] = useState("");
   const lang = langStore.tgt;
   const getExtraRequestData = useCallback(() => ({ context, userInput }), [context, userInput]);
   const onIntermediate = useCallback<OnPythonPluginMessage>(
     async ({ data: { intermediate } }) => {
       if (intermediate?.textList?.length) {
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import { titleCaseWord } from "@/utils/misc";
 import { usePluginIds, usePluginTaskCache } from "@/stores/pluginsInfo";
 import { parseIStr } from "@/actions/i18n";
 import { importMeta } from "@/actions/importMeta";
 import CFHeading from "@/components/CFHeading";
 import { drawboardPluginFactory } from "@/plugins/utils/factory";
 import { useClosePanel } from "../components/hooks";
-import { useDefinitions } from "../components/Fields";
+import { Definitions } from "../components/Fields";
 import { useDefinitionsRequestDataFn } from "./hooks";
 import PythonPluginWithSubmit from "./PluginWithSubmit";
 
 const PythonFieldsPlugin = ({ pluginInfo, ...props }: IPythonFieldsPlugin) => {
   const { id, pureIdentifier } = usePluginIds(pluginInfo.identifier);
   const lang = langStore.tgt;
   const { definitions } = pluginInfo;
@@ -54,28 +54,27 @@
     async (err: any) => {
       toastWord("error", Toast_Words["submit-task-error-message"], { appendix: ` - ${err}` });
     },
     [lang],
   );
 
   const header = parseIStr(pluginInfo.header ?? titleCaseWord(pureIdentifier));
-  const Definitions = useDefinitions({ definitions, numColumns: pluginInfo.numColumns });
   return (
     <PythonPluginWithSubmit
       id={id}
       buttonText={translate(UI_Words["submit-task"], lang)}
       getExtraRequestData={getExtraRequestData}
       onFinished={onFinished}
       onSocketError={onSocketError}
       pluginInfo={pluginInfo}
       {...props}>
       <Flex>
         <CFHeading>{header}</CFHeading>
         <Spacer />
         <CloseIcon w="12px" cursor="pointer" onClick={emitClose} />
       </Flex>
-      {Definitions}
+      <Definitions definitions={definitions} numColumns={pluginInfo.numColumns} />
     </PythonPluginWithSubmit>
   );
 };
 
 drawboardPluginFactory.registerPython("_python.fields", true)(observer(PythonFieldsPlugin));
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_python/PluginGroup.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/PluginGroup.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
   setPluginTaskCache,
 } from "@/stores/pluginsInfo";
 import { useSocketPython } from "@/hooks/usePython";
 import { parseIStr } from "@/actions/i18n";
 import { CFButtonWithBusyTooltip } from "@/components/CFButton";
 import CFDivider from "@/components/CFDivider";
 import Render from "../components/Render";
+import { checkHasConstraint } from "../utils/renderFilters";
 import { useCurrentMeta, useOnMessage } from "./hooks";
 
 export const socketFinishedEvent = new Event<{ id: string }>();
 function PythonPluginWithSubmit({
   id,
   pluginInfo,
   buttonText,
@@ -45,15 +46,16 @@
     toastOnSubmit = true,
     toastMessageOnSubmit,
   } = pluginInfo;
   const lang = langStore.tgt;
   const [hash, setHash] = useState<string | undefined>(undefined);
   const [busy, setBusy] = useState(false);
   const taskCache = usePluginTaskCache(id);
-  const currentMeta = useCurrentMeta(node, nodes);
+  const hasConstraint = checkHasConstraint(props);
+  const currentMeta = hasConstraint ? useCurrentMeta(node, nodes) : undefined;
   const onClick = useCallback(() => {
     if (busy) return;
     beforeSubmit?.();
     setBusy(true);
     setHash(usePluginHash(id));
     if (!taskCache) {
       setPluginTaskCache(id, { currentMeta, parameters: getExtraRequestData?.() ?? {} });
@@ -93,14 +95,15 @@
     identifier,
     isInvisible: props.renderInfo.isInvisible ?? false,
     retryInterval,
     updateInterval,
     onMessage,
     onSocketError,
     getExtraRequestData,
+    needExportNodeData: hasConstraint,
   });
 
   useEffect(() => {
     const { dispose } = socketFinishedEvent.on(({ id: incomingId }) => {
       if (incomingId === id) {
         setBusy(false);
         setHash(undefined);
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_python/QAPlugin.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/QAPlugin.tsx`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import { usePluginIds } from "@/stores/pluginsInfo";
 import { parseIStr } from "@/actions/i18n";
 import CFInput from "@/components/CFInput";
 import { drawboardPluginFactory } from "@/plugins/utils/factory";
 import PythonPluginWithSubmit from "./PluginWithSubmit";
 
 const PythonQAPlugin = ({ pluginInfo, ...props }: IPythonQAPlugin) => {
-  const { id } = usePluginIds(`QA_${pluginInfo.identifier}`);
+  const id = usePluginIds(`QA_${pluginInfo.identifier}`).id;
   const [userInput, setUserInput] = useState("");
   const [serverText, setServerText] = useState(parseIStr(pluginInfo.initialText));
   const lang = langStore.tgt;
   const getExtraRequestData = useCallback(() => ({ text: userInput }), [userInput]);
   const onFinished = useCallback<OnPythonPluginMessage>(
     async ({ data: { final } }) => {
       if (final?.type === "text") {
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_python/hooks.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/hooks.ts`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,32 @@
-import { useCallback, useMemo } from "react";
+import { useCallback, useEffect, useMemo, useState } from "react";
 
-import { Dictionary, INode, isSingleNode, shallowCopy } from "@carefree0910/core";
+import { Dictionary, INode, getRandomHash, isSingleNode, shallowCopy } from "@carefree0910/core";
 import { langStore } from "@carefree0910/business";
 
 import type { IMeta } from "@/schema/meta";
 import type { IDefinitions } from "@/schema/fields";
-import type { IPythonOnPluginMessage, IUseOnPythonPluginMessage } from "@/schema/_python";
+import type {
+  IPythonOnPluginMessage,
+  IPythonPlugin,
+  IUseOnPythonPluginMessage,
+  OnPythonPluginMessage,
+} from "@/schema/_python";
 import { getMetaField } from "@/stores/meta";
-import { setPluginMessage } from "@/stores/pluginsInfo";
+import { setPluginMessage, usePluginIds, usePluginNeedRender } from "@/stores/pluginsInfo";
+import { useSocketPython } from "@/hooks/usePython";
 import { cleanupException, cleanupFinished, cleanupInterrupted } from "../utils/cleanup";
+import { socketFinishedEvent } from "./PluginWithSubmit";
+import { checkHasConstraint } from "../utils/renderFilters";
 
 export function useDefinitionsRequestDataFn(definitions: IDefinitions): () => Dictionary<any> {
   return useCallback(() => {
     const data: Dictionary<any> = {};
     Object.keys(definitions).forEach((field) => {
-      data[field] = getMetaField(field);
+      data[field] = getMetaField({ field });
     });
     return data;
   }, [definitions]);
 }
 export function useCurrentMeta(node: INode | null, nodes: INode[]): IMeta | undefined {
   return useMemo(() => {
     let currentMeta: IMeta | undefined;
@@ -74,7 +82,59 @@
         }
       }
       return {};
     },
     [id, lang, retryInterval, noErrorToast, onFinished],
   );
 }
+
+interface IUseTextTransfer {
+  key: string;
+  plugin: IPythonPlugin;
+}
+export function useTextTransfer({ key, plugin: { pluginInfo, ...props } }: IUseTextTransfer): {
+  id: string;
+  text: string;
+} {
+  const { node, nodes, identifier, retryInterval, updateInterval } = pluginInfo;
+  const id = usePluginIds(`${key}_${identifier}`).id;
+  const needRender = usePluginNeedRender(id);
+  const [hash, setHash] = useState<string | undefined>(undefined);
+  useEffect(() => {
+    if (needRender) {
+      setHash(getRandomHash().toString());
+    }
+  }, [needRender]);
+  useEffect(() => {
+    const { dispose } = socketFinishedEvent.on(({ id: incomingId }) => {
+      if (incomingId === id) {
+        setHash(undefined);
+      }
+    });
+    return dispose;
+  }, [id, setHash]);
+  const [value, setValue] = useState("");
+  const onFinished = useCallback<OnPythonPluginMessage>(
+    async ({ data: { final } }) => {
+      if (final?.type === "text") {
+        setValue(final.value[0].text);
+      }
+    },
+    [setValue],
+  );
+  const onMessage = useOnMessage({ id, pluginInfo, onFinished });
+  const hasConstraint = checkHasConstraint(props);
+
+  useSocketPython({
+    hash,
+    node,
+    nodes,
+    identifier,
+    isInvisible: props.renderInfo.isInvisible ?? false,
+    retryInterval,
+    updateInterval,
+    onMessage,
+    needExportNodeData: hasConstraint,
+  });
+
+  return { id, text: value };
+}
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import { useEffect, useMemo } from "react";
+import { useEffect } from "react";
 import { observer } from "mobx-react-lite";
 import { runInAction } from "mobx";
 
-import { IPathOptions, getRandomHash } from "@carefree0910/core";
+import { IPathOptions } from "@carefree0910/core";
 import {
   BoardStore,
   langStore,
   toolbarStore,
   translate,
   updateBrushOptions,
 } from "@carefree0910/business";
@@ -14,15 +14,15 @@
 import type { ICommonMetaData, IMeta } from "@/schema/meta";
 import type { IPlugin } from "@/schema/plugins";
 import { toastWord } from "@/utils/toast";
 import { Brush_Words } from "@/lang/brush";
 import { Toast_Words } from "@/lang/toast";
 import { themeStore } from "@/stores/theme";
 import { VisibleManager, uiStore } from "@/stores/ui";
-import { setPluginExpanded } from "@/stores/pluginsInfo";
+import { setPluginExpanded, usePluginIds } from "@/stores/pluginsInfo";
 import { hideAllPlugins } from "@/actions/managePlugins";
 import CFButton from "@/components/CFButton";
 import CFSlider from "@/components/CFSlider";
 import CFSwitch from "@/components/CFSwitch";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import { drawboardPluginFactory } from "../utils/factory";
@@ -49,15 +49,15 @@
   }
   // handle plugin visibilities
   runInAction(() => {
     const inBrushMode = !previousInBrushMode;
     if (inBrushMode) {
       uiStore.disablePluginSettings = true;
       VisibleManager.updateVisibleBackup();
-      hideAllPlugins({ except: ["brush"] });
+      hideAllPlugins({ exceptReactPlugins: ["brush"] });
     } else {
       uiStore.disablePluginSettings = false;
       VisibleManager.restoreVisibleBackup();
     }
   });
 };
 
@@ -96,15 +96,16 @@
         formLabelProps={{ ml: "6px" }}
       />
     </>
   );
 }
 
 const BrushPlugin = ({ pluginInfo, ...props }: IPlugin) => {
-  const id = useMemo(() => `brush_${getRandomHash()}`, []);
+  const id = usePluginIds("brush").id;
+
   const lang = langStore.tgt;
   const options = toolbarStore.allBrushOptions;
   const inBrushMode = toolbarStore.inBrushMode;
   const switchBrushMode = useSwitchBrushMode();
   const optionsList = !options ? [] : Array.isArray(options) ? options : [options];
 
   useEffect(() => {
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,105 @@
 import { useCallback, useMemo, useState } from "react";
 import { observer } from "mobx-react-lite";
 import { Flex, Spacer } from "@chakra-ui/react";
 
-import { getRandomHash } from "@carefree0910/core";
 import { langStore, translate, useSelecting } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
 import { DownloadFormat, allDownloadFormat } from "@/schema/misc";
 import { Download_Words } from "@/lang/download";
 import { themeStore } from "@/stores/theme";
+import { usePluginIds } from "@/stores/pluginsInfo";
 import { downloadNodes } from "@/actions/download";
 import CFSelect, { CFSrollableSelect } from "@/components/CFSelect";
 import CFText from "@/components/CFText";
 import CFButton from "@/components/CFButton";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import { drawboardPluginFactory } from "../utils/factory";
 import { useClosePanel } from "../components/hooks";
 import Render from "../components/Render";
 
 const DownloadPlugin = ({ pluginInfo, ...props }: IPlugin) => {
-  const id = useMemo(() => `download_${getRandomHash()}`, []);
+  const id = usePluginIds("download").id;
   const lang = langStore.tgt;
   const { type, nodes } = useSelecting("raw");
   const { w, h, imgWH } = useSelecting("basic")({ fixed: 0 }) ?? {};
   const { captionColor } = themeStore.styles;
   const [format, setFormat] = useState<DownloadFormat>("PNG");
   const [keepOriginal, setKeepOriginal] = useState(true);
   const sizeString = useMemo(() => {
     if (!type || type === "none") return null;
     if (type === "multiple") return translate(Download_Words["download-multiple-caption"], lang);
     if (!keepOriginal || type !== "image") return `${w} x ${Math.abs(h!)}`;
     if (!imgWH) return "Loading...";
     return `${imgWH.w} x ${imgWH.h}`;
   }, [type, lang, w, h, imgWH, keepOriginal]);
   const getWord = useCallback(
-    (keepOriginal: string) =>
+    (keepOriginal: boolean) =>
       translate(
-        keepOriginal === "true"
+        keepOriginal
           ? Download_Words["download-image-size-original"]
           : Download_Words["download-image-size-drawboard"],
         lang,
       ),
     [lang],
   );
   const closePanel = useClosePanel(id);
   const onDownload = useCallback(() => {
     downloadNodes(nodes, format, keepOriginal);
     closePanel();
   }, [nodes, format, keepOriginal, closePanel]);
 
+  const selectedDownloadFormat = { value: format, label: format };
+  const downloadFormatOptions = allDownloadFormat.map((format) => ({
+    value: format,
+    label: format,
+  }));
+
+  const selectedKeepOriginal = { value: keepOriginal, label: getWord(keepOriginal) };
+  const keepOriginalOptions = [true, false].map((keepOriginal) => ({
+    value: keepOriginal,
+    label: getWord(keepOriginal),
+  }));
+
   if (!nodes) return null;
 
   return (
     <Render id={id} {...props}>
       <Flex w="100%" h="100%" direction="column">
         <Flex align="center">
           <CFHeading>{translate(Download_Words["download-plugin-header"], lang)}</CFHeading>
           <CFText ml="4px" fontSize="sm">
             ({nodes.length})
           </CFText>
         </Flex>
         <CFDivider />
-        <CFSrollableSelect
-          value={format}
-          options={allDownloadFormat as any}
-          onOptionClick={(option) => setFormat(option as DownloadFormat)}
+        <CFSrollableSelect<DownloadFormat, false>
+          height="32px"
+          fontSize="14px"
+          value={selectedDownloadFormat}
+          options={downloadFormatOptions}
+          onChange={(e) => {
+            if (!!e) {
+              setFormat(e.value);
+            }
+          }}
         />
-        <CFSelect
-          mt="4px"
-          value={keepOriginal ? "true" : "false"}
-          options={["true", "false"]}
-          optionConverter={getWord}
-          onOptionClick={(option) => setKeepOriginal(option === "true")}
+        <CFSelect<boolean, false>
+          height="32px"
+          fontSize="14px"
+          boxProps={{ mt: "10px" }}
+          value={selectedKeepOriginal}
+          options={keepOriginalOptions}
+          onChange={(e) => {
+            if (!!e) {
+              setKeepOriginal(e.value);
+            }
+          }}
         />
         <Flex mt="8px" pr="6px">
           <Spacer />
           <CFText color={captionColor} fontSize="sm">
             {sizeString}
           </CFText>
         </Flex>
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-import { useMemo } from "react";
 import { observer } from "mobx-react-lite";
 
-import { getRandomHash } from "@carefree0910/core";
 import { useSelecting } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
+import { usePluginIds } from "@/stores/pluginsInfo";
 import Render from "../components/Render";
 import { drawboardPluginFactory } from "../utils/factory";
 
 const GroupEditorPlugin = ({ pluginInfo, ...props }: IPlugin) => {
-  const id = useMemo(() => `groupEditor_${getRandomHash()}`, []);
+  const id = usePluginIds("groupEditor").id;
   const { unGroup } = useSelecting("group") ?? {};
   return <Render id={id} onFloatingButtonClick={async () => unGroup?.()} {...props} />;
 };
 const MultiEditorPlugin = ({ pluginInfo, ...props }: IPlugin) => {
-  const id = useMemo(() => `multiEditor_${getRandomHash()}`, []);
+  const id = usePluginIds("multiEditor").id;
   const { setGroup } = useSelecting("multiple") ?? {};
   return <Render id={id} onFloatingButtonClick={async () => setGroup?.()} {...props} />;
 };
 
 drawboardPluginFactory.register("groupEditor", true)(observer(GroupEditorPlugin));
 drawboardPluginFactory.register("multiEditor", true)(observer(MultiEditorPlugin));
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/MetaPlugin.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/MetaPlugin.tsx`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import { observer } from "mobx-react-lite";
-import { Textarea } from "@chakra-ui/react";
 
 import { useSelecting } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
 import { IMeta, getMetaTrace } from "@/schema/meta";
 import { usePluginIds } from "@/stores/pluginsInfo";
+import CFMarkdown from "@/components/CFMarkdown";
 import { drawboardPluginFactory } from "../utils/factory";
 import Render from "../components/Render";
 
 function getMetaRepresentation(meta: IMeta): string {
   const { type, data } = meta;
   if (type.startsWith("python.")) {
     return data.identifier ?? "unknown";
   }
   return type;
 }
 
 const MetaPlugin = ({ pluginInfo, ...others }: IPlugin) => {
-  const { id } = usePluginIds("meta");
+  const id = usePluginIds("meta").id;
   const info = useSelecting("raw");
   if (!info || info.type === "group" || info.type === "frame" || info.type === "multiple") {
     return null;
   }
   const _meta = info.displayNode?.params.meta;
   if (!_meta) return null;
   const meta = _meta as IMeta;
   const history = getMetaTrace(meta).reverse().map(getMetaRepresentation).join(" -> ");
+  const jsonString = JSON.stringify(meta, null, 2);
+  const markdown = `**${history}**
+
+~~~json
+${jsonString}
+~~~
+`;
 
   return (
     <Render id={id} {...others}>
-      <Textarea
-        w="100%"
-        h="100%"
-        value={`${history}\n\n${JSON.stringify(meta, null, 4)}`}
-        readOnly
-      />
+      <CFMarkdown markdown={markdown} />
     </Render>
   );
 };
 
 drawboardPluginFactory.register("meta", true)(observer(MetaPlugin));
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import Upload from "rc-upload";
 import { observer } from "mobx-react-lite";
 import { useMemo, useState, useEffect, useCallback } from "react";
 import { Box, Flex, Image } from "@chakra-ui/react";
 
-import { Dictionary, Graph, INodePack, Logger, getRandomHash } from "@carefree0910/core";
-import { langStore, translate, useSafeExecute } from "@carefree0910/business";
+import { Dictionary, Graph, INodePack, Logger } from "@carefree0910/core";
+import { BoardStore, langStore, translate, useSafeExecute } from "@carefree0910/business";
 
-import type { IPlugin } from "@/schema/plugins";
 import DeleteIcon from "@/assets/icons/delete.svg";
+
+import type { IPlugin } from "@/schema/plugins";
 import { toastWord } from "@/utils/toast";
 import { globalEvent } from "@/utils/event";
 import { Toast_Words } from "@/lang/toast";
 import { Projects_Words } from "@/lang/projects";
 import { userStore } from "@/stores/user";
 import {
   IProjectsStore,
   getNewProjectInfo,
   getTimeString,
   setCurrentProjectName,
   updateCurrentProjectInfo,
   useCurrentProjectInfo,
 } from "@/stores/projects";
-import { usePluginIsExpanded } from "@/stores/pluginsInfo";
+import { usePluginIds, usePluginIsExpanded } from "@/stores/pluginsInfo";
 import {
   AUTO_SAVE_PREFIX,
   IProject,
   deleteProject,
   getAllProjectInfo,
   getProject,
   loadProject,
@@ -42,15 +43,15 @@
 import { drawboardPluginFactory } from "../utils/factory";
 import { useClosePanel } from "../components/hooks";
 import Render from "../components/Render";
 
 type IImportLocal = IProject | INodePack[];
 
 const ProjectPlugin = ({ pluginInfo, ...props }: IPlugin) => {
-  const id = useMemo(() => `project_${getRandomHash()}`, []);
+  const id = usePluginIds("project").id;
   const lang = langStore.tgt;
   const userId = userStore.userId;
   const expand = usePluginIsExpanded(id);
   const { uid, name } = useCurrentProjectInfo();
   const [selectedUid, setSelectedUid] = useState("");
   const [userInputName, setUserInputName] = useState(name);
   const [allUid2Name, setAllUid2Name] = useState<Dictionary<string> | undefined>();
@@ -140,14 +141,18 @@
       return;
     }
     if (selectedUid === uid) {
       toastWord("info", Toast_Words["already-selected-project-message"]);
       return;
     }
     getLoadUid()
+      .then(async (uid) => {
+        await BoardStore.board.selectorPluginNullable?.destroyAll();
+        return uid;
+      })
       .then((uid) => loadProject(uid, onLoadProjectSuccess))
       .catch((err) =>
         toastWord("error", Toast_Words["load-project-error-message"], { appendix: ` - ${err}` }),
       );
   }
   function onDownloadProject(): void {
     downloadCurrentFullProject();
@@ -197,20 +202,23 @@
         <CFButton mt="12px" onClick={onRenameProject}>
           {translate(Projects_Words["save-project"], lang)}
         </CFButton>
         <CFDivider />
         {allUid2Name ? (
           allProjectUids.length > 0 ? (
             <Flex w="100%">
-              <CFSrollableSelect
-                flex={1}
-                value={selectedUid}
-                options={allProjectUids}
-                onOptionClick={(uid) => setSelectedUid(uid)}
-                optionConverter={(uid) => allUid2Name[uid]}
+              <CFSrollableSelect<string, false>
+                boxProps={{ flex: 1 }}
+                value={{ value: selectedUid, label: allUid2Name?.[selectedUid] }}
+                options={allProjectUids.map((uid) => ({ value: uid, label: allUid2Name[uid] }))}
+                onChange={(e) => {
+                  if (!!e) {
+                    setSelectedUid(e.value);
+                  }
+                }}
               />
               <Box as="button" w="32px" h="100%" p="4px" mx="4px" onClick={onDeleteProject}>
                 <Image src={DeleteIcon} />
               </Box>
             </Flex>
           ) : (
             <CFText>{translate(Projects_Words["no-projects-available"], lang)}</CFText>
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import { useMemo } from "react";
 import { observer } from "mobx-react-lite";
 import { Box, Checkbox, Flex } from "@chakra-ui/react";
 
-import { getRandomHash, Lang } from "@carefree0910/core";
+import { Lang } from "@carefree0910/core";
 import {
   langDescriptions,
   langStore,
   switchLangTo,
   translate,
   useIsReady,
 } from "@carefree0910/business";
@@ -18,44 +17,58 @@
 import { uiStore } from "@/stores/ui";
 import { usePythonPluginSettings } from "@/stores/settings";
 import {
   useReactPluginIsVisible,
   usePythonPluginIsVisible,
   setPythonPluginVisible,
   setReactPluginVisible,
+  usePluginIds,
 } from "@/stores/pluginsInfo";
 import { parseIStr } from "@/actions/i18n";
 import { hideAllPlugins, showAllPlugins } from "@/actions/managePlugins";
 import CFButton from "@/components/CFButton";
 import CFSelect from "@/components/CFSelect";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import { CFGlobalScaleSlider } from "@/components/CFSlider";
 import { drawboardPluginFactory } from "../utils/factory";
 import Render from "../components/Render";
 
+interface LangOption {
+  value: Lang;
+  label: string;
+}
 const SettingsPlugin = ({ pluginInfo, ...props }: IPlugin) => {
-  const id = useMemo(() => `settings_${getRandomHash()}`, []);
+  const id = usePluginIds("settings").id;
   const lang = langStore.tgt;
   const commonProps = { fontWeight: 400, size: "md" };
   const disablePluginSettings = uiStore.disablePluginSettings;
 
+  const selected = { value: lang, label: langDescriptions[lang] };
+  const options: LangOption[] = Object.keys(langDescriptions).map((lang) => ({
+    value: lang as Lang,
+    label: langDescriptions[lang as Lang],
+  }));
+
   return (
     <Render id={id} {...props}>
       <Flex w="100%" h="100%" direction="column">
         {/* language settings */}
         <Box mt="12px">
           <CFHeading>语言 / Language</CFHeading>
           <CFDivider />
-          <CFSelect
-            flex={1}
-            value={lang}
-            options={Object.keys(langDescriptions)}
-            optionConverter={(lang: string) => langDescriptions[lang as Lang]}
-            onOptionClick={(lang: string) => switchLangTo(lang as Lang)}
+          <CFSelect<Lang, false>
+            boxProps={{ mt: "16px" }}
+            value={selected}
+            options={options}
+            onChange={(e) => {
+              if (!!e) {
+                switchLangTo(e.value);
+              }
+            }}
           />
         </Box>
         {/* globalScale settings */}
         {useIsReady() && (
           <Box mt="24px">
             <CFHeading>{translate(Settings_Words["global-scale-header"], lang)}</CFHeading>
             <CFDivider />
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-import { useEffect, useMemo } from "react";
+import { useEffect } from "react";
 import { observer } from "mobx-react-lite";
 
-import { getRandomHash } from "@carefree0910/core";
 import { safeRedo, safeUndo, useUndoRedoSteps } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
-import { setReactPluginVisible } from "@/stores/pluginsInfo";
+import { setReactPluginVisible, usePluginIds } from "@/stores/pluginsInfo";
 import { drawboardPluginFactory } from "../utils/factory";
 import Render from "../components/Render";
 
 const UndoPlugin = ({ pluginInfo, ...props }: IPlugin) => {
-  const id = useMemo(() => `undo_${getRandomHash()}`, []);
+  const id = usePluginIds("undo").id;
   const { undoSteps } = useUndoRedoSteps();
   useEffect(() => setReactPluginVisible("undo", undoSteps > 0), [undoSteps]);
 
   return <Render id={id} onFloatingButtonClick={async () => safeUndo()} {...props} />;
 };
 const RedoPlugin = ({ pluginInfo, ...props }: IPlugin) => {
-  const id = useMemo(() => `redo_${getRandomHash()}`, []);
+  const id = usePluginIds("redo").id;
   const { redoSteps } = useUndoRedoSteps();
   useEffect(() => setReactPluginVisible("redo", redoSteps > 0), [redoSteps]);
 
   return <Render id={id} onFloatingButtonClick={async () => safeRedo()} {...props} />;
 };
 
 drawboardPluginFactory.register("undo", true)(observer(UndoPlugin));
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Fields/BooleanField.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/BooleanField.tsx`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,27 @@
 import type { IBooleanField } from "@/schema/fields";
 import { titleCaseWord } from "@/utils/misc";
 import { getMetaField, setMetaField } from "@/stores/meta";
 import { parseIStr } from "@/actions/i18n";
 import CFSwitch from "@/components/CFSwitch";
 import { useDefaultFieldValue } from "./utils";
 
-export interface BooleanFieldProps extends IField<IBooleanField> {}
-function BooleanField({ field, definition }: BooleanFieldProps) {
-  useDefaultFieldValue({ field, definition });
-  const label = parseIStr(definition.label ?? titleCaseWord(field));
+function BooleanField({ definition, ...fieldKeys }: IField<IBooleanField>) {
+  useDefaultFieldValue({ definition, ...fieldKeys });
+  const label = parseIStr(definition.label ?? titleCaseWord(fieldKeys.field));
   const tooltip = parseIStr(definition.tooltip ?? "");
-  const [value, setValue] = useState(getMetaField(field) ?? definition.default);
+  const [value, setValue] = useState(getMetaField(fieldKeys) ?? definition.default);
 
   return (
     <CFSwitch
       label={label}
       value={value}
       setValue={(value) => {
         setValue(value);
-        setMetaField(field, value);
+        setMetaField(fieldKeys, value);
       }}
       tooltip={tooltip}
       {...definition.props}
     />
   );
 }
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx`

 * *Files 23% similar despite different names*

```diff
@@ -8,37 +8,36 @@
 import { titleCaseWord } from "@/utils/misc";
 import { getMetaField, setMetaField } from "@/stores/meta";
 import { parseIStr } from "@/actions/i18n";
 import CFSlider from "@/components/CFSlider";
 import TextField from "./TextField";
 import { useDefaultFieldValue } from "./utils";
 
-export interface NumberFieldProps extends IField<INumberField> {}
-function NumberField({ field, definition }: NumberFieldProps) {
-  useDefaultFieldValue({ field, definition });
-  const label = parseIStr(definition.label ?? titleCaseWord(field));
-  const [value, setValue] = useState(getMetaField(field) ?? definition.default);
+function NumberField({ definition, ...fieldKeys }: IField<INumberField>) {
+  useDefaultFieldValue({ definition, ...fieldKeys });
+  const label = parseIStr(definition.label ?? titleCaseWord(fieldKeys.field));
+  const [value, setValue] = useState(getMetaField(fieldKeys) ?? definition.default);
 
   if (isUndefined(definition.min) || isUndefined(definition.max)) {
     const tooltip = parseIStr(definition.tooltip ?? label);
     return (
       <TextField
-        field={field}
         definition={{
           type: "text",
           default: definition.default.toString(),
           label: definition.label,
           tooltip,
           props: definition.props,
           numberOptions: {
             min: definition.min,
             max: definition.max,
             isInt: definition.isInt,
           },
         }}
+        {...fieldKeys}
       />
     );
   }
 
   let step = definition.step;
   if (!isUndefined(step) && definition.isInt) step = Math.round(step);
   const tooltip = parseIStr(definition.tooltip ?? "");
@@ -47,15 +46,15 @@
     <CFSlider
       min={definition.min}
       max={definition.max}
       step={step}
       value={value}
       onSliderChange={(value) => {
         setValue(value);
-        setMetaField(field, value);
+        setMetaField(fieldKeys, value);
       }}
       scale={definition.scale}
       label={label}
       tooltip={tooltip}
       precision={definition.isInt ? 0 : definition.precision}
       {...definition.props}
     />
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 import { useCallback, useState } from "react";
 import { observer } from "mobx-react-lite";
-import { Box, Flex } from "@chakra-ui/react";
 
 import { getHash } from "@carefree0910/core";
 
+import type { IStr } from "@/schema/misc";
 import type { IField } from "@/schema/plugins";
 import type { ISelectField } from "@/schema/fields";
 import { getBaseURL, titleCaseWord } from "@/utils/misc";
 import { userStore } from "@/stores/user";
 import { runOneTimeSocketHook } from "@/stores/socket";
 import { getMetaField, setMetaField } from "@/stores/meta";
 import { parseIStr } from "@/actions/i18n";
-import CFTooltip from "@/components/CFTooltip";
-import { CFCaption } from "@/components/CFText";
 import { CFSrollableSelect } from "@/components/CFSelect";
 import { useDefaultFieldValue } from "./utils";
 
-export interface SelectFieldProps extends IField<ISelectField<string>> {}
-function SelectField({ field, definition }: SelectFieldProps) {
-  useDefaultFieldValue({ field, definition });
+function SelectField({ definition, ...fieldKeys }: IField<ISelectField>) {
+  useDefaultFieldValue({ definition, ...fieldKeys });
   const userId = userStore.userId;
-  const label = parseIStr(definition.label ?? titleCaseWord(field));
+  const label = parseIStr(definition.label ?? titleCaseWord(fieldKeys.field));
   const tooltip = parseIStr(definition.tooltip ?? "");
-  const [value, setValue] = useState(getMetaField(field) ?? definition.default);
-  const [options, setOptions] = useState(definition.values as string[]);
-  const onClick = useCallback(() => {
+  const [value, setValue] = useState(getMetaField(fieldKeys) ?? definition.default);
+  const [options, setOptions] = useState(definition.values as IStr[]);
+  const onMenuOpen = useCallback(() => {
     if (definition.localProperties) {
       const extraData = definition.localProperties;
       const hash = getHash(JSON.stringify(extraData)).toString();
-      runOneTimeSocketHook<{ values: string[] }>({
+      runOneTimeSocketHook<{ options: string[] }>({
         key: "selectField",
         hook: {
           key: hash,
           getMessage: async () => ({
             hash,
             userId,
             baseURL: getBaseURL(),
@@ -41,35 +38,37 @@
             nodeDataList: [],
             extraData,
             isInternal: true,
           }),
         },
       }).then((res) => {
         if (res) {
-          setOptions(res.values);
+          setOptions(res.options);
         }
       });
     }
   }, [definition.localProperties]);
 
+  const selected = { value, label: parseIStr(value) };
+  const selectOptions = options.map((value) => ({ value, label: parseIStr(value) }));
+
   return (
-    <Flex w="100%" h="100%" align="center" {...definition.props}>
-      <CFTooltip label={tooltip}>
-        <CFCaption label={label} />
-      </CFTooltip>
-      <Box w="8px" />
-      <CFSrollableSelect
-        flex={1}
-        h="100%"
-        value={value}
-        options={options}
-        onOptionClick={(value) => {
-          setValue(value);
-          setMetaField(field, value);
-        }}
-        onClick={onClick}
-      />
-    </Flex>
+    <CFSrollableSelect<IStr, false>
+      fontSize="14px"
+      label={label}
+      tooltip={tooltip}
+      flexProps={definition.props}
+      boxProps={{ flex: 1 }}
+      value={selected}
+      options={selectOptions}
+      onMenuOpen={onMenuOpen}
+      onChange={(e) => {
+        if (!!e) {
+          setValue(e.value);
+          setMetaField(fieldKeys, e.value);
+        }
+      }}
+    />
   );
 }
 
 export default observer(SelectField);
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Fields/TextField.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/TextField.tsx`

 * *Files 11% similar despite different names*

```diff
@@ -8,33 +8,32 @@
 import { titleCaseWord } from "@/utils/misc";
 import { getMetaField, setMetaField } from "@/stores/meta";
 import { parseIStr } from "@/actions/i18n";
 import CFInput from "@/components/CFInput";
 import CFTextarea from "@/components/CFTextarea";
 import { useDefaultFieldValue } from "./utils";
 
-export interface TextFieldProps extends IField<ITextField> {}
-function TextField({ field, definition }: TextFieldProps) {
-  useDefaultFieldValue({ field, definition });
-  const label = parseIStr(definition.label ?? titleCaseWord(field));
+function TextField({ definition, ...fieldKeys }: IField<ITextField>) {
+  useDefaultFieldValue({ definition, ...fieldKeys });
+  const label = parseIStr(definition.label ?? titleCaseWord(fieldKeys.field));
   const tooltip = parseIStr(definition.tooltip ?? "");
   const defaultText = parseIStr(definition.default ?? "");
-  const [value, setValue] = useState(getMetaField(field) ?? defaultText);
+  const [value, setValue] = useState(getMetaField(fieldKeys) ?? defaultText);
   const isNumber = useMemo(() => !!definition.numberOptions, [definition.numberOptions]);
   const Input = definition.numRows && definition.numRows > 1 ? CFTextarea : CFInput;
 
   const onChange = useCallback(
     (event: ChangeEvent<HTMLInputElement | HTMLTextAreaElement>) => {
       const v = event.target.value;
       setValue(v);
       if (!isNumber) {
-        setMetaField(field, v);
+        setMetaField(fieldKeys, v);
       }
     },
-    [isNumber, field, setValue],
+    [isNumber, fieldKeys, setValue],
   );
   const onBlur = useCallback(() => {
     if (definition.numberOptions) {
       let number = +value;
       const options = definition.numberOptions;
       if (isNaN(number)) number = 0;
       if (!isUndefined(options.min)) {
@@ -43,17 +42,17 @@
       if (!isUndefined(options.max)) {
         number = Math.min(number, options.max);
       }
       if (options.isInt) {
         number = Math.round(number);
       }
       setValue(number.toString());
-      setMetaField(field, number);
+      setMetaField(fieldKeys, number);
     }
-  }, [field, value, setValue, definition.numberOptions]);
+  }, [fieldKeys, value, setValue, definition.numberOptions]);
 
   return (
     <Input
       value={value}
       onChange={onChange}
       onBlur={onBlur}
       tooltip={tooltip}
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Fields/index.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/index.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,47 @@
 import { ReactElement, useMemo } from "react";
 import { Flex, FlexProps } from "@chakra-ui/react";
 
-import { argMin, isUndefined, range, shallowCopy } from "@carefree0910/core";
+import { argMin, range, shallowCopy } from "@carefree0910/core";
 
 import type { IDefinitions } from "@/schema/fields";
-import TextField from "./TextField";
-import NumberField from "./NumberField";
-import SelectField from "./SelectField";
-import BooleanField from "./BooleanField";
+import { getFieldH } from "./utils";
+import { Field } from "./Field";
+import ListField from "./ListField";
 
-interface IUseDefinitions extends FlexProps {
+interface IDefinitionsComponent extends FlexProps {
   definitions: IDefinitions;
   numColumns?: number;
   rowGap?: number;
 }
-export function useDefinitions({ definitions, numColumns, rowGap, ...others }: IUseDefinitions) {
+export function Definitions({ definitions, numColumns, rowGap, ...others }: IDefinitionsComponent) {
   const nc = numColumns ?? 1;
   const gap = rowGap ?? 12;
-  const defaultH = 42;
+
   const columnW = useMemo(
     () => (numColumns === 1 ? "100%" : `${(100 - 5 * (nc - 1)) / nc}%`),
     [nc],
   );
 
   const entries = Object.entries(shallowCopy(definitions));
   if (entries.length === 0) return null;
 
   const columns: ReactElement[][] = range(0, nc).map(() => []);
   const heights = columns.map(() => 0);
   entries.forEach(([field, definition]) => {
-    let Field: any;
-    if (definition.type === "text") {
-      Field = TextField;
-    } else if (definition.type === "number") {
-      Field = NumberField;
-    } else if (definition.type === "select") {
-      Field = SelectField;
-    } else if (definition.type === "boolean") {
-      Field = BooleanField;
-    }
-    if (!Field) return;
-    const props = definition.props ?? {};
-    if (isUndefined(props.w)) props.w = "100%";
-    // calculate height, in order to place the field in the shortest column
-    let FieldH;
-    if (!isUndefined(props.h)) {
-      if (!props.h.endsWith("px")) {
-        throw Error(`Field '${field}' height must be in px`);
-      }
-      FieldH = parseInt(props.h.slice(0, -2));
+    let FieldComponent;
+    if (definition.type !== "list") {
+      FieldComponent = <Field key={field} field={field} definition={definition} gap={gap} />;
     } else {
-      const numRows = definition.numRows ?? 1;
-      FieldH = defaultH * numRows + gap * (numRows - 1);
-      props.h = `${FieldH}px`;
+      FieldComponent = <ListField key={field} field={field} definition={definition} gap={gap} />;
     }
-    definition.props = props;
+    const fieldH = getFieldH({ gap, definition, field });
     const columnIdx = argMin(heights);
-    heights[columnIdx] += FieldH + gap;
-    columns[columnIdx].push(<Field key={field} field={field} definition={definition} />);
+    heights[columnIdx] += fieldH + gap;
+    columns[columnIdx].push(FieldComponent);
   });
 
   return (
     <Flex p="12px" flexWrap="wrap" alignItems="center" justifyContent="space-around" {...others}>
       {columns.map((column, idx) => (
         <Flex
           key={idx}
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Floating.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Floating.tsx`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,19 @@
   TextProps,
 } from "@chakra-ui/react";
 
 import { isUndefined } from "@carefree0910/core";
 import { langStore, translate } from "@carefree0910/business";
 
 import type { IFloating } from "@/schema/plugins";
-import { BG_TRANSITION, DEFAULT_PLUGIN_SETTINGS, VISIBILITY_TRANSITION } from "@/utils/constants";
+import {
+  BG_TRANSITION,
+  DEFAULT_PLUGIN_SETTINGS,
+  makeVisibilityTransitionProps,
+} from "@/utils/constants";
 import { UI_Words } from "@/lang/ui";
 import { themeStore, useScrollBarSx } from "@/stores/theme";
 import {
   usePluginMessage,
   usePluginIsExpanded,
   setPluginExpanded,
   usePluginGroupIsExpanded,
@@ -85,26 +89,26 @@
   bgOpacity ??= DEFAULT_PLUGIN_SETTINGS.bgOpacity;
   const bgOpacityHex = Math.round(bgOpacity * 255).toString(16);
   const getCommonProps = useCallback(
     <T extends boolean>(isExpand: T): T extends true ? FlexProps : ButtonProps => ({
       p: isExpand ? "12px" : "8px",
       bg: `${isBusy ? busyColor : panelBg}${bgOpacityHex}`,
       position: "absolute",
-      // boxShadow: "2px 2px 4px rgba(0, 0, 0, 0.25)",
       borderRadius: "4px",
       /**
        * if
        *   1. `interactingWithBoard` is `true`
-       * or this floating belongs to a group, and:
-       *   2. we are focusing on the plugin button (isExpand=false) and the group is not expanded
-       *   3. we are focusing on the expanded panel (isExpand=true) but the floating is not expanded
+       *   2. we are focusing on the expanded panel (isExpand=true) but the floating is not expanded
+       *   3. we are focusing on the plugin icon (isExpand=false), but the icon is not activated
        * then this floating should not be interactive
        */
       pointerEvents:
-        interactingWithBoard || (!iconActivated && (!isExpand || !expand)) ? "none" : "auto",
+        interactingWithBoard || (isExpand && !expand) || (!isExpand && !iconActivated)
+          ? "none"
+          : "auto",
     }),
     [panelBg, busyColor, bgOpacityHex, expand, isBusy, iconActivated, interactingWithBoard],
   );
   //// progress bar props
   const progressProps = useMemo<CircularProgressProps>(() => {
     const size = Math.floor(Math.min(iconW, iconH) * 0.8);
     return {
@@ -181,17 +185,18 @@
         h={`${iconH}px`}
         onClick={() => {
           if (!noExpand) {
             setPluginExpanded(id, !expand);
           }
           onFloatingButtonClick?.();
         }}
-        opacity={isInvisible ? 0 : 1}
-        visibility={isInvisible ? "hidden" : "visible"}
-        transition={`${VISIBILITY_TRANSITION}, ${BG_TRANSITION}`}
+        {...makeVisibilityTransitionProps({
+          visible: !isInvisible,
+          extraTransitions: BG_TRANSITION,
+        })}
         _focus={{ outline: "none" }}
         {...getCommonProps(false)}
         {...props}
         imageProps={{ opacity: iconOpacity }}>
         {taskMessage && isBusy && (
           <Box w={`${iconW}px`} h={`${iconH}px`} position="absolute" left="0px" top="0px">
             {taskMessage.status === "pending" ? (
@@ -222,17 +227,15 @@
         <Portal containerRef={ref as any}>
           <Flex
             id={expandId}
             w={`${w}px`}
             h={`${h}px`}
             overflowX="hidden"
             direction="column"
-            opacity={expand ? 1 : 0}
-            visibility={expand ? "visible" : "hidden"}
-            transition={VISIBILITY_TRANSITION}
+            {...makeVisibilityTransitionProps({ visible: expand })}
             {...getCommonProps(true)}
             bg={expandBg}
             sx={useScrollBarSx()}
             {...parsedExpandProps}>
             {children}
           </Flex>
         </Portal>
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/components/Render.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Render.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/index.tsx` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/index.tsx`

 * *Files 5% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 export * from "./_react/ArrangePlugin";
 export * from "./_react/UndoRedoPlugin";
 export * from "./_react/DownloadPlugin";
 export * from "./_react/DeletePlugin";
 export * from "./_react/TextEditorPlugin";
 export * from "./_react/GroupPlugin";
 export * from "./_react/LinksPlugin";
+export * from "./_react/ShortcutsPlugin";
 export * from "./_react/BrushPlugin";
+export * from "./_python/PluginGroup";
 export * from "./_python/FieldsPlugin";
 export * from "./_python/TextAreaPlugin";
 export * from "./_python/QAPlugin";
 export * from "./_python/ChatPlugin";
-export * from "./_python/PluginGroup";
+export * from "./_python/MarkdownPlugin";
 
 function MakePlugin<T extends AllPlugins>({
   type,
   containerRef,
   props: { renderInfo, pluginInfo, ...props },
 }: IMakePlugin<T>) {
   renderInfo = shallowCopy(renderInfo);
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/utils/cleanup.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/utils/cleanup.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/utils/factory.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/utils/factory.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/plugins/utils/renderFilters.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/utils/renderFilters.ts`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
   const hash = hashInfo(info);
   const getMessage = (): Promise<IPythonSocketRequest> => {
     return getPythonRequest({
       node: info?.displayNode ?? null,
       nodes: info?.nodes ?? [],
       identifier: "node_validator",
       opt: { noExport: true },
+      needExportNodeData: true,
     }).then((data) => ({
       ...data,
       hash,
       extraData: { key: validator },
       isInternal: true,
     }));
   };
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/react-app-env.d.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/react-app-env.d.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/requests/actions.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/actions.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/requests/hooks.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/hooks.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/requests/interceptors/_python.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/interceptors/_python.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/requests/interceptors/index.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/interceptors/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/schema/_python.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/_python.ts`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
   pluginInfo: IPythonPluginInfo;
 }
 interface IPythonCallbacks {
   getExtraRequestData?: () => Dictionary<any>;
 }
 export interface IUsePythonInfo extends IPythonPluginInfo, IPythonCallbacks {
   isInvisible: boolean;
+  needExportNodeData: boolean;
 }
 export interface INodeData {
   type?: INode["type"];
   // transform info
   x?: number;
   y?: number;
   w?: number;
@@ -40,14 +41,38 @@
   meta?: IMeta;
   // children, in case this is a `Group`
   children?: INodeData[];
 }
 
 // plugin
 
+export interface IPythonPluginGroup extends IPythonPlugin {
+  pluginInfo: IPythonPluginInfo & {
+    header?: IStr;
+    plugins: IMakePlugin<PythonPlugins>[];
+  };
+}
+
+export interface IUseOnPythonPluginMessage {
+  id: string;
+  pluginInfo: IPythonPluginInfo & IPythonPluginWithSubmitPluginInfo;
+  onIntermediate?: OnPythonPluginMessage;
+  onFinished: OnPythonPluginMessage;
+}
+export type OnPythonPluginMessage = (message: IPythonPluginMessage) => void;
+export interface IPythonSocketPluginWithSubmit
+  extends Omit<IPythonPlugin, "id" | "pluginInfo">,
+    Omit<IPythonSocketCallbacks<IPythonResults>, "getMessage" | "onMessage">,
+    IUseOnPythonPluginMessage {
+  id: string;
+  buttonText: string;
+  beforeSubmit?: () => void;
+  afterSubmit?: () => void;
+}
+
 interface IPythonPluginWithSubmitPluginInfo {
   closeOnSubmit?: boolean;
   toastOnSubmit?: boolean;
   toastMessageOnSubmit?: IStr;
 }
 export interface IPythonFieldsPlugin extends IPythonPlugin {
   pluginInfo: IPythonPluginInfo &
@@ -56,53 +81,28 @@
       definitions: IDefinitions;
       numColumns?: number;
     };
 }
 
 export interface IPythonTextAreaPlugin extends IPythonPlugin {
   pluginInfo: IPythonPluginInfo & {
-    noLoading?: boolean;
     textAlign?: TextareaProps["textAlign"];
   };
 }
 export interface IPythonQAPlugin extends IPythonPlugin {
   pluginInfo: IPythonPluginInfo & {
     initialText: IStr;
   };
 }
 export interface IPythonChatPlugin extends IPythonPlugin {
   pluginInfo: IPythonPluginInfo & {
     initialText: IStr;
   };
 }
 
-export interface IPythonPluginGroup extends IPythonPlugin {
-  pluginInfo: IPythonPluginInfo & {
-    header?: IStr;
-    plugins: IMakePlugin<PythonPlugins>[];
-  };
-}
-
-export interface IUseOnPythonPluginMessage {
-  id: string;
-  pluginInfo: IPythonPluginInfo & IPythonPluginWithSubmitPluginInfo;
-  onIntermediate?: OnPythonPluginMessage;
-  onFinished: OnPythonPluginMessage;
-}
-export type OnPythonPluginMessage = (message: IPythonPluginMessage) => void;
-export interface IPythonSocketPluginWithSubmit
-  extends Omit<IPythonPlugin, "id" | "pluginInfo">,
-    Omit<IPythonSocketCallbacks<IPythonResults>, "getMessage" | "onMessage">,
-    IUseOnPythonPluginMessage {
-  id: string;
-  buttonText: string;
-  beforeSubmit?: () => void;
-  afterSubmit?: () => void;
-}
-
 // web
 
 export interface IPythonSocketRequest {
   hash: string;
   userId: string;
   baseURL: string;
   identifier: string;
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/schema/fields.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/fields.ts`

 * *Files 9% similar despite different names*

```diff
@@ -34,45 +34,47 @@
   precision?: number;
 }
 interface ISelectLocalProperties {
   path: string;
   regex?: string;
   noExt: boolean;
   onlyFiles: boolean;
+  defaultPlaceholder?: string;
 }
-export interface ISelectField<T> extends IBaseFields {
+export interface ISelectField extends IBaseFields {
   type: "select";
-  values: readonly T[];
-  default: T;
+  values: readonly IStr[];
+  default: IStr;
   isMulti?: boolean;
   localProperties?: ISelectLocalProperties;
 }
 export interface IBooleanField extends IBaseFields {
   type: "boolean";
   default: boolean;
 }
 export interface IColorField extends IBaseFields {
   type: "color";
   default: IStr;
 }
 export interface IListField extends IBaseFields {
   type: "list";
-  item: IFieldDefinition;
+  item: IDefinitions;
   default: any[];
+  maxNumRows?: number;
 }
 export interface IObjectField extends IBaseFields {
   type: "object";
   items: IDefinitions;
   default: Dictionary<any>;
 }
 
 export type IFieldDefinition =
   | ITextField
   | IImageField
   | INumberField
-  | ISelectField<any>
+  | ISelectField
   | IBooleanField
   | IColorField
   | IListField
   | IObjectField;
 export type IFieldType = IFieldDefinition["type"];
 export type IDefinitions = Dictionary<IFieldDefinition>;
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/schema/meta.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/meta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/schema/plugins.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/plugins.ts`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import type { INode, NodeType, PivotType } from "@carefree0910/core";
 
 import type { IStr } from "./misc";
 import type { IFieldDefinition } from "./fields";
 import type {
   IPythonChatPlugin,
   IPythonFieldsPlugin,
+  IPythonPlugin,
   IPythonPluginGroup,
   IPythonQAPlugin,
   IPythonTextAreaPlugin,
 } from "./_python";
 
 // general
 
@@ -39,43 +40,52 @@
 export interface IRenderInfo extends IExpandPositionInfo {
   src: IStr;
   tooltip?: IStr;
   offsetX?: number;
   offsetY?: number;
   bgOpacity?: number;
   useModal?: boolean;
+  keepOpen?: boolean;
   modalOpacity?: number;
   expandProps?: FlexProps;
   isInvisible?: boolean;
 }
 export interface IFloating extends ButtonProps {
   id: string;
   groupId?: string; // the id of the group this floating belongs to
   renderInfo: IRenderInfo;
   noExpand?: boolean;
   onFloatingButtonClick?: () => Promise<void>;
 }
 export interface IRender extends Omit<IFloating, "id" | "renderInfo">, NodeConstraintSettings {
   id?: string;
-  renderInfo: Partial<Omit<IRenderInfo, "src">> & { w: number; h: number; src: string };
+  renderInfo: Partial<Omit<IRenderInfo, "src">> & { w: number; h: number; src: IStr };
   containerRef?: RefObject<HTMLDivElement>;
 }
 export interface IPluginInfo {
   node: INode | null;
   nodes: INode[];
 }
 export interface IPlugin extends IRender {
   pluginInfo: IPluginInfo;
 }
+export interface ILogoPlugin extends IPlugin {
+  pluginInfo: IPluginInfo & { redirectUrl?: string };
+}
 
 // specific
 
+export interface IListProperties {
+  listKey: string;
+  listIndex: number;
+}
 export interface IField<T extends IFieldDefinition> {
   field: string;
   definition: T;
+  listProperties?: IListProperties;
 }
 
 // factory
 
 export const allReactPlugins = [
   "meta",
   "settings",
@@ -83,27 +93,30 @@
   "add",
   "arrange",
   "undo",
   "redo",
   "download",
   "delete",
   "wiki",
-  "github",
   "email",
+  "github",
+  "shortcuts",
+  "logo",
   "textEditor",
   "groupEditor",
   "multiEditor",
   "brush",
 ] as const;
 export const allPythonPlugins = [
+  "_python.pluginGroup",
   "_python.fields",
   "_python.textArea",
   "_python.QA",
   "_python.chat",
-  "_python.pluginGroup",
+  "_python.markdown",
 ] as const;
 export type ReactPlugins = (typeof allReactPlugins)[number];
 export type PythonPlugins = (typeof allPythonPlugins)[number];
 export type AllPlugins = ReactPlugins | PythonPlugins;
 
 export interface IPluginProps {
   // react plugins
@@ -113,26 +126,29 @@
   add: IPlugin;
   arrange: IPlugin;
   undo: IPlugin;
   redo: IPlugin;
   download: IPlugin;
   delete: IPlugin;
   wiki: IPlugin;
-  github: IPlugin;
   email: IPlugin;
+  github: IPlugin;
+  shortcuts: IPlugin;
+  logo: ILogoPlugin;
   textEditor: IPlugin;
   groupEditor: IPlugin;
   multiEditor: IPlugin;
   brush: IPlugin;
   // python plugins
+  "_python.pluginGroup": IPythonPluginGroup;
   "_python.fields": IPythonFieldsPlugin;
   "_python.textArea": IPythonTextAreaPlugin;
   "_python.QA": IPythonQAPlugin;
   "_python.chat": IPythonChatPlugin;
-  "_python.pluginGroup": IPythonPluginGroup;
+  "_python.markdown": IPythonPlugin;
 }
 
 export interface IMakePlugin<T extends AllPlugins> {
   type: T;
   props: Omit<IPluginProps[T], "containerRef" | "pluginInfo"> & {
     pluginInfo: Omit<IPluginProps[T]["pluginInfo"], "node" | "nodes">;
   };
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/schema/requests.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/requests.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/debug.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/debug.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/gridLines.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/gridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/hooks.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/hooks.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/pluginsInfo.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/pluginsInfo.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import { useCallback, useEffect } from "react";
 import { action, makeObservable, observable, runInAction } from "mobx";
 
 import { Dictionary, getRandomHash, isUndefined } from "@carefree0910/core";
 import { ABCStore, useIsReady } from "@carefree0910/business";
 
 import type { IMeta } from "@/schema/meta";
-import type { ReactPlugins } from "@/schema/plugins";
+import { allReactPlugins, type ReactPlugins } from "@/schema/plugins";
 import type { IPythonPluginMessage } from "@/schema/_python";
 import { stripHashFromIdentifier } from "@/utils/misc";
 
 interface IDs {
   id: string;
   pureIdentifier: string;
 }
@@ -101,22 +101,26 @@
   remove<T extends IPluginCollection>(collection: T, key: string) {
     delete this[collection][key];
   }
 }
 
 const pluginsInfoStore = new PluginsInfoStore();
 // ids
-export const usePluginIds = (identifier: string): IDs => {
-  const pureIdentifier = stripHashFromIdentifier(identifier).replaceAll(".", "_");
+export function usePluginIds(plugin: ReactPlugins, hasEffect?: boolean): IDs;
+export function usePluginIds(identifier: string, hasEffect?: boolean): IDs;
+export function usePluginIds(input: ReactPlugins | string, hasEffect: boolean = true): IDs {
+  const pureIdentifier = allReactPlugins.includes(input)
+    ? input
+    : stripHashFromIdentifier(input).replaceAll(".", "_");
   return pluginsInfoStore.setDefault("ids", {
     key: pureIdentifier,
-    hasEffect: true,
+    hasEffect,
     getDefault: () => ({ id: `${pureIdentifier}_${getRandomHash()}`, pureIdentifier }),
   });
-};
+}
 // hashes
 export const usePluginHash = (id: string): string => {
   return pluginsInfoStore.setDefault("hashes", {
     key: id,
     hasEffect: false,
     getDefault: () => getRandomHash().toString(),
   });
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/projects.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/socket.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/socket.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/theme.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/theme.ts`

 * *Files 9% similar despite different names*

```diff
@@ -12,21 +12,20 @@
   panelBg: string;
   // color of the text
   textColor: string;
   // color of the caption
   captionColor: string;
   // color of the divider
   dividerColor: string;
+  // colors of the `CFInput` component
+  inputColors: {
+    activeBorderColor: string;
+  };
   // colors of the `CFSelect` component
   selectColors: {
-    color: string;
-    bgColor: string;
-    hoverBgColor: string;
-    checkedColor: string;
-    hoverBorderColor: string;
     activeBorderColor: string;
   };
   // colors of the `CFSlider` component
   sliderColors: {
     sliderTrackColor: string;
     sliderThumbBorderColor: string;
     inputBgColor: string;
@@ -60,21 +59,19 @@
 export const allThemes: Record<ThemeType, ThemeStyles> = {
   light: {
     boardBg: "#f7f7f7",
     panelBg: "#f9f9f9",
     textColor: "#333333",
     captionColor: "#888888",
     dividerColor: "#cccccc",
+    inputColors: {
+      activeBorderColor: "#3fc9a8",
+    },
     selectColors: {
-      color: "#333333",
-      bgColor: "#f0f0f0",
-      hoverBgColor: "#f9f9f9",
-      checkedColor: "#3ad822",
-      hoverBorderColor: "#bbbbbb",
-      activeBorderColor: "#999999",
+      activeBorderColor: "#3fc9a8",
     },
     sliderColors: {
       sliderTrackColor: "#3ad822",
       sliderThumbBorderColor: "#3fc9a8",
       inputBgColor: "#eeeeee",
     },
     switchColors: {
@@ -103,21 +100,19 @@
   // currently dark mode is just a placeholder
   dark: {
     boardBg: "#242424",
     panelBg: "#f9f9f9",
     textColor: "#333333",
     captionColor: "#888888",
     dividerColor: "#cccccc",
+    inputColors: {
+      activeBorderColor: "#3fc9a8",
+    },
     selectColors: {
-      color: "#333333",
-      bgColor: "#f0f0f0",
-      hoverBgColor: "#f9f9f9",
-      checkedColor: "#3ad822",
-      hoverBorderColor: "#bbbbbb",
-      activeBorderColor: "#999999",
+      activeBorderColor: "#3fc9a8",
     },
     sliderColors: {
       sliderTrackColor: "#3ad822",
       sliderThumbBorderColor: "#3fc9a8",
       inputBgColor: "#eeeeee",
     },
     switchColors: {
@@ -188,7 +183,26 @@
       borderRadius: "8px",
     },
     "&::-webkit-scrollbar-corner": {
       backgroundColor: "transparent",
     },
   };
 }
+export function useInputProps(): ChakraProps {
+  const {
+    textColor,
+    captionColor,
+    inputColors: { activeBorderColor },
+  } = themeStore.styles;
+
+  return {
+    color: textColor,
+    borderWidth: "1px",
+    borderRadius: "0px",
+    flexShrink: 0,
+    _placeholder: { color: captionColor },
+    _focusVisible: {
+      borderColor: activeBorderColor,
+      boxShadow: `0 0 0 1px ${activeBorderColor}`,
+    },
+  };
+}
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/stores/ui.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/ui.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/utils/event.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/event.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/utils/misc.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/misc.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/src/utils/toast.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/toast.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/tsconfig.json` & `carefree-drawboard-0.0.1a4/cfdraw/.web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/vite.config.ts` & `carefree-drawboard-0.0.1a4/cfdraw/.web/vite.config.ts`

 * *Files 7% similar despite different names*

```diff
@@ -46,28 +46,29 @@
   },
   esbuild: {
     keepNames: true,
   },
   build: {
     rollupOptions: {
       output: {
-        entryFileNames: "assets/[name].js",
-        chunkFileNames: "assets/[name].js",
-        assetFileNames: "assets/[name].[ext]",
         manualChunks: {
           axios: ["axios"],
           jszip: ["jszip"],
           react: ["react", "react-dom"],
           "chakra-ui": ["@chakra-ui/react", "@chakra-ui/icons"],
           svgdotjs: [
             "@svgdotjs/svg.js",
             "@svgdotjs/svg.filter.js",
             "@svgdotjs/svg.topath.js",
             "@svgdotjs/svg.topoly.js",
           ],
+          "lottie-web": ["lottie-web"],
+          "react-color": ["react-color"],
+          "chakra-react-select": ["chakra-react-select"],
+          "react-markdown": ["react-markdown", "remark-gfm", "react-syntax-highlighter"],
           "@carefree0910/core": ["@carefree0910/core"],
           "@carefree0910/svg": ["@carefree0910/svg"],
           "@carefree0910/business": ["@carefree0910/business"],
           "@carefree0910/native": ["@carefree0910/native"],
         },
       },
     },
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/.web/yarn.lock` & `carefree-drawboard-0.0.1a4/cfdraw/.web/yarn.lock`

 * *Files 11% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 "@babel/plugin-transform-react-jsx-source@^7.19.6":
   version "7.19.6"
   resolved "https://registry.npmmirror.com/@babel/plugin-transform-react-jsx-source/-/plugin-transform-react-jsx-source-7.19.6.tgz#88578ae8331e5887e8ce28e4c9dc83fb29da0b86"
   integrity sha512-RpAi004QyMNisst/pvSanoRdJ4q+jMCWyk9zdw/CyLB9j8RXEahodR6l2GyttDRyEVWZtbN+TpLiHJ3t34LbsQ==
   dependencies:
     "@babel/helper-plugin-utils" "^7.19.0"
 
-"@babel/runtime@^7.0.0", "@babel/runtime@^7.12.13", "@babel/runtime@^7.12.5", "@babel/runtime@^7.18.3", "@babel/runtime@^7.20.7", "@babel/runtime@^7.21.0":
+"@babel/runtime@^7.0.0", "@babel/runtime@^7.12.0", "@babel/runtime@^7.12.13", "@babel/runtime@^7.12.5", "@babel/runtime@^7.18.3", "@babel/runtime@^7.20.7", "@babel/runtime@^7.21.0", "@babel/runtime@^7.3.1", "@babel/runtime@^7.5.5", "@babel/runtime@^7.8.7":
   version "7.21.5"
   resolved "https://registry.npmmirror.com/@babel/runtime/-/runtime-7.21.5.tgz#8492dddda9644ae3bda3b45eabe87382caee7200"
   integrity sha512-8jI69toZqqcsnqGGqwGS4Qb1VwLOEp4hz+CXPywcvjs60u3B4Pom/U/7rm4W8tMOYEB+E9wgD0mW1l3r8qlI9Q==
   dependencies:
     regenerator-runtime "^0.13.11"
 
 "@babel/template@^7.20.7":
@@ -213,41 +213,41 @@
   resolved "https://registry.npmmirror.com/@babel/types/-/types-7.21.5.tgz#18dfbd47c39d3904d5db3d3dc2cc80bedb60e5b6"
   integrity sha512-m4AfNvVF2mVC/F7fDEdH2El3HzUg9It/XsCxZiOTTA3m3qYfcSVSbTfM6Q9xG+hYDniZssYhlXKKUMD5m8tF4Q==
   dependencies:
     "@babel/helper-string-parser" "^7.21.5"
     "@babel/helper-validator-identifier" "^7.19.1"
     to-fast-properties "^2.0.0"
 
-"@carefree0910/business@~0.5.1-alpha.8":
-  version "0.5.1-alpha.8"
-  resolved "https://registry.npmmirror.com/@carefree0910/business/-/business-0.5.1-alpha.8.tgz#a493b93d3340a38abd3994cb5f07eea21e3107ac"
-  integrity sha512-gbC3JUhi05SixMpCwFlAu+zNPbcJeHkYeyyfVbfqk3vXHzl6RL5kwV+77T/iJcQVVFkq7nIZBZg0Y6YIq9euBA==
-  dependencies:
-    "@carefree0910/core" "^0.5.1-alpha.8"
-    "@carefree0910/svg" "^0.5.1-alpha.8"
-
-"@carefree0910/core@^0.5.1-alpha.8", "@carefree0910/core@~0.5.1-alpha.8":
-  version "0.5.1-alpha.8"
-  resolved "https://registry.npmmirror.com/@carefree0910/core/-/core-0.5.1-alpha.8.tgz#7a3568e703cc7b50fef9d630e504a7266e052d63"
-  integrity sha512-pMpt1FTpJHAsUrX/1QpxhCFYeXjSnhvCr89mBOJEvLDdpgyHS8ONtJFiqfHuuWTdisFXDEE4VRGlghmgkOQnZg==
-
-"@carefree0910/native@~0.5.1-alpha.8":
-  version "0.5.1-alpha.8"
-  resolved "https://registry.npmmirror.com/@carefree0910/native/-/native-0.5.1-alpha.8.tgz#e33c982a1c41c8c3e31195dad440655871ffc46b"
-  integrity sha512-pnwnGhdoQUG+JLfLvuk6IhUHO/2FJKIFSfqbpxdkO0Q8zVoXZeqmrFsHEHq7WbCiWwcrmXI11nsc+g6/5z+uog==
-  dependencies:
-    "@carefree0910/core" "^0.5.1-alpha.8"
-    "@carefree0910/svg" "^0.5.1-alpha.8"
-
-"@carefree0910/svg@^0.5.1-alpha.8", "@carefree0910/svg@~0.5.1-alpha.8":
-  version "0.5.1-alpha.8"
-  resolved "https://registry.npmmirror.com/@carefree0910/svg/-/svg-0.5.1-alpha.8.tgz#6a80dd8f09099339fbcb90e344913b106a6fc93a"
-  integrity sha512-GYOpRxea5rXKlNfp1Xa5zIGZ8hkKsrQWLbJnDqmGu0UIjh+wzGNqiTJGDMc+LkGAPpaZ/nOHFMCLxeOSzimO9w==
+"@carefree0910/business@~0.5.1-alpha.12":
+  version "0.5.1-alpha.12"
+  resolved "https://registry.npmmirror.com/@carefree0910/business/-/business-0.5.1-alpha.12.tgz#fe2c14e8a590ca110b7c43e7376a25ac3e9ed9a9"
+  integrity sha512-jNGSnyee48ReFQpQumPRO4ybD1WoZEsyUb6O6I6tjOhFY8VOYPOv7KlsTRybf5zMsyvufhQT/NnnPwmbubQW4Q==
+  dependencies:
+    "@carefree0910/core" "^0.5.1-alpha.12"
+    "@carefree0910/svg" "^0.5.1-alpha.12"
+
+"@carefree0910/core@^0.5.1-alpha.12", "@carefree0910/core@~0.5.1-alpha.12":
+  version "0.5.1-alpha.12"
+  resolved "https://registry.npmmirror.com/@carefree0910/core/-/core-0.5.1-alpha.12.tgz#9cbcd6387904fc6684ed9dd1e3977f21fa72337d"
+  integrity sha512-vcHr4avN6YAovMocPuhKUR9revZ0qWDGY0SoE9bI9MRHGEVN9XkjELk0USYcpUKRdWNAxejzeCJenPRXdWIvLQ==
+
+"@carefree0910/native@~0.5.1-alpha.12":
+  version "0.5.1-alpha.12"
+  resolved "https://registry.npmmirror.com/@carefree0910/native/-/native-0.5.1-alpha.12.tgz#560905a39f452ae0910115d3f772fbb306a098b6"
+  integrity sha512-Nnbg+5LIODPjYfDx3Oa5TuW4w5tw4VIyIGJJr0mC/JDys/xiSULKzPMJ2cAaaHfQES2TXyO+Ufru9yZRjWrBmA==
+  dependencies:
+    "@carefree0910/core" "^0.5.1-alpha.12"
+    "@carefree0910/svg" "^0.5.1-alpha.12"
+
+"@carefree0910/svg@^0.5.1-alpha.12", "@carefree0910/svg@~0.5.1-alpha.12":
+  version "0.5.1-alpha.12"
+  resolved "https://registry.npmmirror.com/@carefree0910/svg/-/svg-0.5.1-alpha.12.tgz#31d5fbb2b93b66c0995ea8df45bed69806008e18"
+  integrity sha512-7QNGWuu8r02HjwiHEAdGF5dh9lO8Mg+60X9AhvnTcWtftwPDRucXQBZEm02gutF8Anb3Rc4RYtjwxxqI8qwAHw==
   dependencies:
-    "@carefree0910/core" "^0.5.1-alpha.8"
+    "@carefree0910/core" "^0.5.1-alpha.12"
 
 "@chakra-ui/accordion@2.1.11":
   version "2.1.11"
   resolved "https://registry.npmmirror.com/@chakra-ui/accordion/-/accordion-2.1.11.tgz#c6df0100c543645d0631df3aefde2ea2b8ed6313"
   integrity sha512-mfVPmqETp9pyRDHJ33AdF19oHv/LyxVzQJtlxUByuvs8Cj9QQZ2LQLg5kejm+b3mj03A7A6yfbuo3RNaI4Bhsg==
   dependencies:
     "@chakra-ui/descendant" "3.0.14"
@@ -1064,15 +1064,15 @@
     babel-plugin-macros "^3.1.0"
     convert-source-map "^1.5.0"
     escape-string-regexp "^4.0.0"
     find-root "^1.1.0"
     source-map "^0.5.7"
     stylis "4.2.0"
 
-"@emotion/cache@^11.11.0":
+"@emotion/cache@^11.11.0", "@emotion/cache@^11.4.0":
   version "11.11.0"
   resolved "https://registry.npmmirror.com/@emotion/cache/-/cache-11.11.0.tgz#809b33ee6b1cb1a625fef7a45bc568ccd9b8f3ff"
   integrity sha512-P34z9ssTCBi3e9EI1ZsWpNHcfY1r09ZO0rZbRO2ob3ZQMnFI35jB536qoXbkdesr5EUhYi22anuEJuyxifaqAQ==
   dependencies:
     "@emotion/memoize" "^0.8.1"
     "@emotion/sheet" "^1.2.2"
     "@emotion/utils" "^1.2.1"
@@ -1104,15 +1104,15 @@
   integrity sha512-Ja/Vfqe3HpuzRsG1oBtWTHk2PGZ7GR+2Vz5iYGelAw8dx32K0y7PjVuxK6z1nMpZOqAFsRUPCkK1YjJ56qJlgw==
 
 "@emotion/memoize@^0.8.1":
   version "0.8.1"
   resolved "https://registry.npmmirror.com/@emotion/memoize/-/memoize-0.8.1.tgz#c1ddb040429c6d21d38cc945fe75c818cfb68e17"
   integrity sha512-W2P2c/VRW1/1tLox0mVUalvnWXxavmv/Oum2aPsRcoDJuob75FC3Y8FbpfLwUegRcxINtGUMPq0tFCvYNTBXNA==
 
-"@emotion/react@^11.9.3":
+"@emotion/react@^11.8.1", "@emotion/react@^11.9.3":
   version "11.11.0"
   resolved "https://registry.npmmirror.com/@emotion/react/-/react-11.11.0.tgz#408196b7ef8729d8ad08fc061b03b046d1460e02"
   integrity sha512-ZSK3ZJsNkwfjT3JpDAWJZlrGD81Z3ytNDsxw1LKq1o+xkmO5pnWfr6gmCC8gHEFf3nSSX/09YrG67jybNPxSUw==
   dependencies:
     "@babel/runtime" "^7.18.3"
     "@emotion/babel-plugin" "^11.11.0"
     "@emotion/cache" "^11.11.0"
@@ -1308,14 +1308,26 @@
     strip-json-comments "^3.1.1"
 
 "@eslint/js@8.37.0":
   version "8.37.0"
   resolved "https://registry.npmmirror.com/@eslint/js/-/js-8.37.0.tgz#cf1b5fa24217fe007f6487a26d765274925efa7d"
   integrity sha512-x5vzdtOOGgFVDCUs81QRB2+liax8rFg3+7hqM+QhBG0/G3F1ZsoYl97UrqgHgQ9KKT7G6c4V+aTUCgu/n22v1A==
 
+"@floating-ui/core@^1.2.6":
+  version "1.2.6"
+  resolved "https://registry.npmmirror.com/@floating-ui/core/-/core-1.2.6.tgz#d21ace437cc919cdd8f1640302fa8851e65e75c0"
+  integrity sha512-EvYTiXet5XqweYGClEmpu3BoxmsQ4hkj3QaYA6qEnigCWffTP3vNRwBReTdrwDwo7OoJ3wM8Uoe9Uk4n+d4hfg==
+
+"@floating-ui/dom@^1.0.1":
+  version "1.2.8"
+  resolved "https://registry.npmmirror.com/@floating-ui/dom/-/dom-1.2.8.tgz#aee0f6ccc0787ab8fe741487a6e5e95b7b125375"
+  integrity sha512-XLwhYV90MxiHDq6S0rzFZj00fnDM+A1R9jhSioZoMsa7G0Q0i+Q4x40ajR8FHSdYDE1bgjG45mIWe6jtv9UPmg==
+  dependencies:
+    "@floating-ui/core" "^1.2.6"
+
 "@humanwhocodes/config-array@^0.11.8":
   version "0.11.8"
   resolved "https://registry.npmmirror.com/@humanwhocodes/config-array/-/config-array-0.11.8.tgz#03595ac2075a4dc0f191cc2131de14fbd7d410b9"
   integrity sha512-UybHIJzJnR5Qc/MsD9Kr+RpO2h+/P1GhOwdiLPXK5TWk5sgTdu88bTD9UP+CKbPPh5Rni1u0GjAdYQLemG8g+g==
   dependencies:
     "@humanwhocodes/object-schema" "^1.2.1"
     debug "^4.1.1"
@@ -1327,14 +1339,19 @@
   integrity sha512-bxveV4V8v5Yb4ncFTT3rPSgZBOpCkjfK0y4oVVVJwIuDVBRMDXrPyXRL988i5ap9m9bnyEEjWfm5WkBmtffLfA==
 
 "@humanwhocodes/object-schema@^1.2.1":
   version "1.2.1"
   resolved "https://registry.npmmirror.com/@humanwhocodes/object-schema/-/object-schema-1.2.1.tgz#b520529ec21d8e5945a1851dfd1c32e94e39ff45"
   integrity sha512-ZnQMnLV4e7hDlUvw8H+U8ASL02SS2Gn6+9Ac3wGGLIe7+je2AeAOxPY+izIPJDfFDb7eDjev0Us8MO1iFRN8hA==
 
+"@icons/material@^0.2.4":
+  version "0.2.4"
+  resolved "https://registry.npmmirror.com/@icons/material/-/material-0.2.4.tgz#e90c9f71768b3736e76d7dd6783fc6c2afa88bc8"
+  integrity sha512-QPcGmICAPbGLGb6F/yNf/KzKqvFx8z5qx3D1yFqVAjoFmXK35EgyW+cJ57Te3CNsmzblwtzakLGFqHPqrfb4Tw==
+
 "@jridgewell/gen-mapping@^0.3.0", "@jridgewell/gen-mapping@^0.3.2":
   version "0.3.3"
   resolved "https://registry.npmmirror.com/@jridgewell/gen-mapping/-/gen-mapping-0.3.3.tgz#7e02e6eb5df901aaedb08514203b096614024098"
   integrity sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==
   dependencies:
     "@jridgewell/set-array" "^1.0.1"
     "@jridgewell/sourcemap-codec" "^1.4.10"
@@ -1614,19 +1631,33 @@
     tslib "^2.4.0"
 
 "@total-typescript/ts-reset@^0.4.2":
   version "0.4.2"
   resolved "https://registry.npmmirror.com/@total-typescript/ts-reset/-/ts-reset-0.4.2.tgz#c564c173ba09973968e1046c93965b7a257878a4"
   integrity sha512-vqd7ZUDSrXFVT1n8b2kc3LnklncDQFPvR58yUS1kEP23/nHPAO9l1lMjUfnPrXYYk4Hj54rrLKMW5ipwk7k09A==
 
+"@types/debug@^4.0.0":
+  version "4.1.7"
+  resolved "https://registry.npmmirror.com/@types/debug/-/debug-4.1.7.tgz#7cc0ea761509124709b8b2d1090d8f6c17aadb82"
+  integrity sha512-9AonUzyTjXXhEOa0DnqpzZi6VHlqKMswga9EXjpXnnqxwLtdvPPtlO8evrI5D9S6asFRCQ6v+wpiUKbw+vKqyg==
+  dependencies:
+    "@types/ms" "*"
+
 "@types/estree@^1.0.0":
   version "1.0.1"
   resolved "https://registry.npmmirror.com/@types/estree/-/estree-1.0.1.tgz#aa22750962f3bf0e79d753d3cc067f010c95f194"
   integrity sha512-LG4opVs2ANWZ1TJoKc937iMmNstM/d0ae1vNbnBvBhqCSezgVUOzcLCqbI5elV8Vy6WKwKjaqR+zO9VKirBBCA==
 
+"@types/hast@^2.0.0":
+  version "2.3.4"
+  resolved "https://registry.npmmirror.com/@types/hast/-/hast-2.3.4.tgz#8aa5ef92c117d20d974a82bdfb6a648b08c0bafc"
+  integrity sha512-wLEm0QvaoawEDoTRwzTXp4b4jpwiJDvR5KMnFnVodm3scufTlBOWRD6N1OBf9TZMhjlNsSfcO5V+7AF4+Vy+9g==
+  dependencies:
+    "@types/unist" "*"
+
 "@types/js-cookie@^2.x.x":
   version "2.2.7"
   resolved "https://registry.npmmirror.com/@types/js-cookie/-/js-cookie-2.2.7.tgz#226a9e31680835a6188e887f3988e60c04d3f6a3"
   integrity sha512-aLkWa0C0vO5b4Sr798E26QgOkss68Un0bLjs7u9qxzPT5CG+8DuNTffWES58YzJs3hrVAOs1wonycqEBqNJubA==
 
 "@types/json5@^0.0.29":
   version "0.0.29"
@@ -1641,36 +1672,70 @@
     "@types/lodash" "*"
 
 "@types/lodash@*":
   version "4.14.194"
   resolved "https://registry.npmmirror.com/@types/lodash/-/lodash-4.14.194.tgz#b71eb6f7a0ff11bff59fc987134a093029258a76"
   integrity sha512-r22s9tAS7imvBt2lyHC9B8AGwWnXaYb1tY09oyLkXDs4vArpYJzw09nj8MLx5VfciBPGIb+ZwG0ssYnEPJxn/g==
 
+"@types/mdast@^3.0.0":
+  version "3.0.11"
+  resolved "https://registry.npmmirror.com/@types/mdast/-/mdast-3.0.11.tgz#dc130f7e7d9306124286f6d6cee40cf4d14a3dc0"
+  integrity sha512-Y/uImid8aAwrEA24/1tcRZwpxX3pIFTSilcNDKSPn+Y2iDywSEachzRuvgAYYLR3wpGXAsMbv5lvKLDZLeYPAw==
+  dependencies:
+    "@types/unist" "*"
+
+"@types/ms@*":
+  version "0.7.31"
+  resolved "https://registry.npmmirror.com/@types/ms/-/ms-0.7.31.tgz#31b7ca6407128a3d2bbc27fe2d21b345397f6197"
+  integrity sha512-iiUgKzV9AuaEkZqkOLDIvlQiL6ltuZd9tGcW3gwpnX8JbuiuhFlEGmmFXEXkN50Cvq7Os88IY2v0dkDqXYWVgA==
+
 "@types/node@18.15.11":
   version "18.15.11"
   resolved "https://registry.npmmirror.com/@types/node/-/node-18.15.11.tgz#b3b790f09cb1696cffcec605de025b088fa4225f"
   integrity sha512-E5Kwq2n4SbMzQOn6wnmBjuK9ouqlURrcZDVfbo9ftDDTFt3nk7ZKK4GMOzoYgnpQJKcxwQw+lGaBvvlMo0qN/Q==
 
 "@types/parse-json@^4.0.0":
   version "4.0.0"
   resolved "https://registry.npmmirror.com/@types/parse-json/-/parse-json-4.0.0.tgz#2f8bb441434d163b35fb8ffdccd7138927ffb8c0"
   integrity sha512-//oorEZjL6sbPcKUaCdIGlIUeH26mgzimjBB77G6XRgnDl/L5wOnpyBGRe/Mmf5CVW3PwEBE1NjiMZ/ssFh4wA==
 
-"@types/prop-types@*":
+"@types/prop-types@*", "@types/prop-types@^15.0.0":
   version "15.7.5"
   resolved "https://registry.npmmirror.com/@types/prop-types/-/prop-types-15.7.5.tgz#5f19d2b85a98e9558036f6a3cacc8819420f05cf"
   integrity sha512-JCB8C6SnDoQf0cNycqd/35A7MjcnK+ZTqE7judS6o7utxUCg6imJg3QK2qzHKszlTjcj2cn+NwMB2i96ubpj7w==
 
+"@types/react-color@^3.0.6":
+  version "3.0.6"
+  resolved "https://registry.npmmirror.com/@types/react-color/-/react-color-3.0.6.tgz#602fed023802b2424e7cd6ff3594ccd3d5055f9a"
+  integrity sha512-OzPIO5AyRmLA7PlOyISlgabpYUa3En74LP8mTMa0veCA719SvYQov4WLMsHvCgXP+L+KI9yGhYnqZafVGG0P4w==
+  dependencies:
+    "@types/react" "*"
+    "@types/reactcss" "*"
+
 "@types/react-dom@18.0.11":
   version "18.0.11"
   resolved "https://registry.npmmirror.com/@types/react-dom/-/react-dom-18.0.11.tgz#321351c1459bc9ca3d216aefc8a167beec334e33"
   integrity sha512-O38bPbI2CWtgw/OoQoY+BRelw7uysmXbWvw3nLWO21H1HSh+GOlqPuXshJfjmpNlKiiSDG9cc1JZAaMmVdcTlw==
   dependencies:
     "@types/react" "*"
 
+"@types/react-syntax-highlighter@^15.5.6":
+  version "15.5.6"
+  resolved "https://registry.npmmirror.com/@types/react-syntax-highlighter/-/react-syntax-highlighter-15.5.6.tgz#77c95e6b74d2be23208fcdcf187b93b47025f1b1"
+  integrity sha512-i7wFuLbIAFlabTeD2I1cLjEOrG/xdMa/rpx2zwzAoGHuXJDhSqp9BSfDlMHSh9JSuNfxHk9eEmMX6D55GiyjGg==
+  dependencies:
+    "@types/react" "*"
+
+"@types/react-transition-group@^4.4.0":
+  version "4.4.6"
+  resolved "https://registry.npmmirror.com/@types/react-transition-group/-/react-transition-group-4.4.6.tgz#18187bcda5281f8e10dfc48f0943e2fdf4f75e2e"
+  integrity sha512-VnCdSxfcm08KjsJVQcfBmhEQAPnLB8G08hAxn39azX1qYBQ/5RVQuoHuKIcfKOdncuaUvEpFKFzEvbtIMsfVew==
+  dependencies:
+    "@types/react" "*"
+
 "@types/react@*":
   version "18.2.6"
   resolved "https://registry.npmmirror.com/@types/react/-/react-18.2.6.tgz#5cd53ee0d30ffc193b159d3516c8c8ad2f19d571"
   integrity sha512-wRZClXn//zxCFW+ye/D2qY65UsYP1Fpex2YXorHc8awoNamkMZSvBxwxdYVInsHOZZd2Ppq8isnSzJL5Mpf8OA==
   dependencies:
     "@types/prop-types" "*"
     "@types/scheduler" "*"
@@ -1681,19 +1746,31 @@
   resolved "https://registry.npmmirror.com/@types/react/-/react-18.0.33.tgz#a1575160cb4376787c2f5fe0312302f824baa61e"
   integrity sha512-sHxzVxeanvQyQ1lr8NSHaj0kDzcNiGpILEVt69g9S31/7PfMvNCKLKcsHw4lYKjs3cGNJjXSP4mYzX43QlnjNA==
   dependencies:
     "@types/prop-types" "*"
     "@types/scheduler" "*"
     csstype "^3.0.2"
 
+"@types/reactcss@*":
+  version "1.2.6"
+  resolved "https://registry.npmmirror.com/@types/reactcss/-/reactcss-1.2.6.tgz#133c1e7e896f2726370d1d5a26bf06a30a038bcc"
+  integrity sha512-qaIzpCuXNWomGR1Xq8SCFTtF4v8V27Y6f+b9+bzHiv087MylI/nTCqqdChNeWS7tslgROmYB7yeiruWX7WnqNg==
+  dependencies:
+    "@types/react" "*"
+
 "@types/scheduler@*":
   version "0.16.3"
   resolved "https://registry.npmmirror.com/@types/scheduler/-/scheduler-0.16.3.tgz#cef09e3ec9af1d63d2a6cc5b383a737e24e6dcf5"
   integrity sha512-5cJ8CB4yAx7BH1oMvdU0Jh9lrEXyPkar6F9G/ERswkCuvP4KQZfZkSjcMbAICCpQTN4OuZn8tz0HiKv9TGZgrQ==
 
+"@types/unist@*", "@types/unist@^2.0.0":
+  version "2.0.6"
+  resolved "https://registry.npmmirror.com/@types/unist/-/unist-2.0.6.tgz#250a7b16c3b91f672a24552ec64678eeb1d3a08d"
+  integrity sha512-PBjIUxZHOuj0R15/xuwJYjFi+KZdNFrehocChv4g5hu6aFroHue8m0lBP0POdK2nKzbw0cgV1mws8+V/JAcEkQ==
+
 "@types/uuid@^9.0.1":
   version "9.0.1"
   resolved "https://registry.npmmirror.com/@types/uuid/-/uuid-9.0.1.tgz#98586dc36aee8dacc98cc396dbca8d0429647aa6"
   integrity sha512-rFT3ak0/2trgvp4yYZo5iKFEPsET7vKydKF+VRCxlQ9bpheehyAJH89dAkaLEq/j/RZXJIqcgsmPJKUP1Z28HA==
 
 "@typescript-eslint/parser@^5.42.0":
   version "5.59.5"
@@ -1943,14 +2020,19 @@
   resolved "https://registry.npmmirror.com/babel-plugin-macros/-/babel-plugin-macros-3.1.0.tgz#9ef6dc74deb934b4db344dc973ee851d148c50c1"
   integrity sha512-Cg7TFGpIr01vOQNODXOOaGz2NpCU5gl8x1qJFbb6hbZxR7XrcE2vtbAsTAbJ7/xwJtUuJEw8K8Zr/AE0LHlesg==
   dependencies:
     "@babel/runtime" "^7.12.5"
     cosmiconfig "^7.0.0"
     resolve "^1.19.0"
 
+bail@^2.0.0:
+  version "2.0.2"
+  resolved "https://registry.npmmirror.com/bail/-/bail-2.0.2.tgz#d26f5cd8fe5d6f832a31517b9f7c356040ba6d5d"
+  integrity sha512-0xO6mYd7JB2YesxDKplafRpsiOzPt9V02ddPCLbY1xYGPOX24NTyN50qnUxgCPcSoYMhKpAuBTjQoRZCAkUDRw==
+
 balanced-match@^1.0.0:
   version "1.0.2"
   resolved "https://registry.npmmirror.com/balanced-match/-/balanced-match-1.0.2.tgz#e83e3a7e3f300b34cb9d87f615fa0cbf357690ee"
   integrity sha512-3oSeUO0TMV67hN1AmbXsK4yaqU7tjiHlbxRDZOpH0KW9+CeX4bRAaX0Anxt0tx2MrpRpWwQaPwIlISEJhYU5Pw==
 
 big-integer@^1.6.44:
   version "1.6.51"
@@ -2020,14 +2102,26 @@
   integrity sha512-Gmy6FhYlCY7uOElZUSbxo2UCDH8owEk996gkbrpsgGtrJLM3J7jGxl9Ic7Qwwj4ivOE5AWZWRMecDdF7hqGjFA==
 
 caniuse-lite@^1.0.30001406, caniuse-lite@^1.0.30001449:
   version "1.0.30001486"
   resolved "https://registry.npmmirror.com/caniuse-lite/-/caniuse-lite-1.0.30001486.tgz#56a08885228edf62cbe1ac8980f2b5dae159997e"
   integrity sha512-uv7/gXuHi10Whlj0pp5q/tsK/32J2QSqVRKQhs2j8VsDCjgyruAh/eEXHF822VqO9yT6iZKw3nRwZRSPBE9OQg==
 
+ccount@^2.0.0:
+  version "2.0.1"
+  resolved "https://registry.npmmirror.com/ccount/-/ccount-2.0.1.tgz#17a3bf82302e0870d6da43a01311a8bc02a3ecf5"
+  integrity sha512-eyrF0jiFpY+3drT6383f1qhkbGsLSifNAjA61IUjZjmLCWjItY6LB9ft9YhoDgwfmclB2zhu51Lc7+95b8NRAg==
+
+chakra-react-select@^4.6.0:
+  version "4.6.0"
+  resolved "https://registry.npmmirror.com/chakra-react-select/-/chakra-react-select-4.6.0.tgz#a1a35ee7c531db47ac9c8bd412fb0a3745e77321"
+  integrity sha512-Ckcs+ofX5LxCc0oOz4SorDIRqF/afd5tAQOa694JVJiIckYorUmZASEUSSDdXaZltsUAtJE11CUmEZgVVsk9Eg==
+  dependencies:
+    react-select "5.7.0"
+
 chalk@^2.0.0:
   version "2.4.2"
   resolved "https://registry.npmmirror.com/chalk/-/chalk-2.4.2.tgz#cd42541677a54333cf541a49108c1432b44c9424"
   integrity sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==
   dependencies:
     ansi-styles "^3.2.1"
     escape-string-regexp "^1.0.5"
@@ -2037,14 +2131,34 @@
   version "4.1.2"
   resolved "https://registry.npmmirror.com/chalk/-/chalk-4.1.2.tgz#aac4e2b7734a740867aeb16bf02aad556a1e7a01"
   integrity sha512-oKnbhFyRIXpUuez8iBMmyEa4nbj4IOQyuhc/wy9kY7/WVPcwIO9VA668Pu8RkO7+0G76SLROeyw9CpQ061i4mA==
   dependencies:
     ansi-styles "^4.1.0"
     supports-color "^7.1.0"
 
+character-entities-legacy@^1.0.0:
+  version "1.1.4"
+  resolved "https://registry.npmmirror.com/character-entities-legacy/-/character-entities-legacy-1.1.4.tgz#94bc1845dce70a5bb9d2ecc748725661293d8fc1"
+  integrity sha512-3Xnr+7ZFS1uxeiUDvV02wQ+QDbc55o97tIV5zHScSPJpcLm/r0DFPcoY3tYRp+VZukxuMeKgXYmsXQHO05zQeA==
+
+character-entities@^1.0.0:
+  version "1.2.4"
+  resolved "https://registry.npmmirror.com/character-entities/-/character-entities-1.2.4.tgz#e12c3939b7eaf4e5b15e7ad4c5e28e1d48c5b16b"
+  integrity sha512-iBMyeEHxfVnIakwOuDXpVkc54HijNgCyQB2w0VfGQThle6NXn50zU6V/u+LDhxHcDUPojn6Kpga3PTAD8W1bQw==
+
+character-entities@^2.0.0:
+  version "2.0.2"
+  resolved "https://registry.npmmirror.com/character-entities/-/character-entities-2.0.2.tgz#2d09c2e72cd9523076ccb21157dff66ad43fcc22"
+  integrity sha512-shx7oQ0Awen/BRIdkjkvz54PnEEI/EjwXDSIZp86/KKdbafHh1Df/RYGBhn4hbe2+uKC9FnT5UCEdyPz3ai9hQ==
+
+character-reference-invalid@^1.0.0:
+  version "1.1.4"
+  resolved "https://registry.npmmirror.com/character-reference-invalid/-/character-reference-invalid-1.1.4.tgz#083329cda0eae272ab3dbbf37e9a382c13af1560"
+  integrity sha512-mKKUkUbhPpQlCOfIuZkvSEgktjPFIsZKRRbC6KWVEMvlzblj3i3asQv5ODsrwt0N3pHAEvjP8KTQPHkp0+6jOg==
+
 "chokidar@>=3.0.0 <4.0.0":
   version "3.5.3"
   resolved "https://registry.npmmirror.com/chokidar/-/chokidar-3.5.3.tgz#1cf37c8707b932bd1af1ae22c0432e2acd1903bd"
   integrity sha512-Dr3sfKRP6oTcjf2JmUmFJfeVMvXBdegxB0iVQ5eb2V10uFJUCAS8OByZdVAyVb8xXNz3GjjTgj9kLWsZTqE6kw==
   dependencies:
     anymatch "~3.1.2"
     braces "~3.0.2"
@@ -2107,14 +2221,24 @@
 combined-stream@^1.0.8:
   version "1.0.8"
   resolved "https://registry.npmmirror.com/combined-stream/-/combined-stream-1.0.8.tgz#c3d45a8b34fd730631a110a8a2520682b31d5a7f"
   integrity sha512-FQN4MRfuJeHf7cBbBMJFXhKSDq+2kAArBlmRBvcvFE5BB1HZKXtSFASDhdlz9zOYwxh8lDdnvmMOe/+5cdoEdg==
   dependencies:
     delayed-stream "~1.0.0"
 
+comma-separated-tokens@^1.0.0:
+  version "1.0.8"
+  resolved "https://registry.npmmirror.com/comma-separated-tokens/-/comma-separated-tokens-1.0.8.tgz#632b80b6117867a158f1080ad498b2fbe7e3f5ea"
+  integrity sha512-GHuDRO12Sypu2cV70d1dkA2EUmXHgntrzbpvOB+Qy+49ypNfGgFQIC2fhhXbnyrJRynDCAARsT7Ou0M6hirpfw==
+
+comma-separated-tokens@^2.0.0:
+  version "2.0.3"
+  resolved "https://registry.npmmirror.com/comma-separated-tokens/-/comma-separated-tokens-2.0.3.tgz#4e89c9458acb61bc8fef19f4529973b2392839ee"
+  integrity sha512-Fu4hJdvzeylCfQPp9SGWidpzrMs7tTrlu6Vb8XGaRGck8QSNZJJp538Wrb60Lax4fPwR64ViY468OIUTbRlGZg==
+
 compute-scroll-into-view@1.0.20:
   version "1.0.20"
   resolved "https://registry.npmmirror.com/compute-scroll-into-view/-/compute-scroll-into-view-1.0.20.tgz#1768b5522d1172754f5d0c9b02de3af6be506a43"
   integrity sha512-UCB0ioiyj8CRjtrvaceBLqqhZCVP+1B8+NWQhmdsm0VXOJtobBCf1dBQmebCCo34qZmUwZfIH2MZLqNHazrfjg==
 
 concat-map@0.0.1:
   version "0.0.1"
@@ -2183,21 +2307,28 @@
 debug@^3.2.7:
   version "3.2.7"
   resolved "https://registry.npmmirror.com/debug/-/debug-3.2.7.tgz#72580b7e9145fb39b6676f9c5e5fb100b934179a"
   integrity sha512-CFjzYYAi4ThfiQvizrFQevTTXHtnCqWfe7x1AhgEscTz6ZbLbfoLRLPugTQyBth6f8ZERVUSyWHFD/7Wu4t1XQ==
   dependencies:
     ms "^2.1.1"
 
-debug@^4.1.0, debug@^4.1.1, debug@^4.3.2, debug@^4.3.4:
+debug@^4.0.0, debug@^4.1.0, debug@^4.1.1, debug@^4.3.2, debug@^4.3.4:
   version "4.3.4"
   resolved "https://registry.npmmirror.com/debug/-/debug-4.3.4.tgz#1319f6579357f2338d3337d2cdd4914bb5dcc865"
   integrity sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==
   dependencies:
     ms "2.1.2"
 
+decode-named-character-reference@^1.0.0:
+  version "1.0.2"
+  resolved "https://registry.npmmirror.com/decode-named-character-reference/-/decode-named-character-reference-1.0.2.tgz#daabac9690874c394c81e4162a0304b35d824f0e"
+  integrity sha512-O8x12RzrUF8xyVcY0KJowWsmaJxQbmy0/EtnNtHRpsOcT7dFk5W598coHqBVpmWo1oQQfsCqfCmkZN5DJrZVdg==
+  dependencies:
+    character-entities "^2.0.0"
+
 deep-equal@^2.0.5:
   version "2.2.1"
   resolved "https://registry.npmmirror.com/deep-equal/-/deep-equal-2.2.1.tgz#c72ab22f3a7d3503a4ca87dde976fe9978816739"
   integrity sha512-lKdkdV6EOGoVn65XaOsPdH4rMxTZOnmFyuIkMjM1i5HHCbfjC97dawgTAy0deYNfuqUqW+Q5VrVaQYtUpSd6yQ==
   dependencies:
     array-buffer-byte-length "^1.0.0"
     call-bind "^1.0.2"
@@ -2260,19 +2391,29 @@
     object-keys "^1.1.1"
 
 delayed-stream@~1.0.0:
   version "1.0.0"
   resolved "https://registry.npmmirror.com/delayed-stream/-/delayed-stream-1.0.0.tgz#df3ae199acadfb7d440aaae0b29e2272b24ec619"
   integrity sha512-ZySD7Nf91aLB0RxL4KGrKHBXl7Eds1DAmEdcoVawXnLD7SDhpNgtuII2aAkg7a7QS41jxPSZ17p4VdGnMHk3MQ==
 
+dequal@^2.0.0:
+  version "2.0.3"
+  resolved "https://registry.npmmirror.com/dequal/-/dequal-2.0.3.tgz#2644214f1997d39ed0ee0ece72335490a7ac67be"
+  integrity sha512-0je+qPKHEMohvfRTCEo3CrPG6cAzAYgmzKyxRiYSSDkS6eGJdyVJm7WaYA5ECaAD9wLB2T4EEeymA5aFVcYXCA==
+
 detect-node-es@^1.1.0:
   version "1.1.0"
   resolved "https://registry.npmmirror.com/detect-node-es/-/detect-node-es-1.1.0.tgz#163acdf643330caa0b4cd7c21e7ee7755d6fa493"
   integrity sha512-ypdmJU/TbBby2Dxibuv7ZLW3Bs1QEmM7nHjEANfohJLvE0XVujisn1qPJcZxg+qDucsr+bP6fLD1rPS3AhJ7EQ==
 
+diff@^5.0.0:
+  version "5.1.0"
+  resolved "https://registry.npmmirror.com/diff/-/diff-5.1.0.tgz#bc52d298c5ea8df9194800224445ed43ffc87e40"
+  integrity sha512-D+mk+qE8VC/PAUrlAU34N+VfXev0ghe5ywmpqrawphmVZc1bEfn56uo9qpyGp1p4xpzOHkSW4ztBd6L7Xx4ACw==
+
 dir-glob@^3.0.1:
   version "3.0.1"
   resolved "https://registry.npmmirror.com/dir-glob/-/dir-glob-3.0.1.tgz#56dbf73d992a4a93ba1584f4534063fd2e41717f"
   integrity sha512-WkrWp9GR4KXfKGYzOLmTuGVi1UWFfws377n9cc55/tb6DuqyF6pcQ5AbiHEshaDpY9v6oaSr2XCDidGmMwdzIA==
   dependencies:
     path-type "^4.0.0"
 
@@ -2286,14 +2427,22 @@
 doctrine@^3.0.0:
   version "3.0.0"
   resolved "https://registry.npmmirror.com/doctrine/-/doctrine-3.0.0.tgz#addebead72a6574db783639dc87a121773973961"
   integrity sha512-yS+Q5i3hBf7GBkd4KG8a7eBNNWNGLTaEwwYWUijIYM7zrlYDM0BFXHjjPWlWZ1Rg7UaddZeIDmi9jF3HmqiQ2w==
   dependencies:
     esutils "^2.0.2"
 
+dom-helpers@^5.0.1:
+  version "5.2.1"
+  resolved "https://registry.npmmirror.com/dom-helpers/-/dom-helpers-5.2.1.tgz#d9400536b2bf8225ad98fe052e029451ac40e902"
+  integrity sha512-nRCa7CK3VTrM2NmGkIy4cbK7IZlgBE/PYMn55rrXefr5xXDP0LdtfPnblFDoVdcAfslJ7or6iqAUnx0CCGIWQA==
+  dependencies:
+    "@babel/runtime" "^7.8.7"
+    csstype "^3.0.2"
+
 electron-to-chromium@^1.4.284:
   version "1.4.393"
   resolved "https://registry.npmmirror.com/electron-to-chromium/-/electron-to-chromium-1.4.393.tgz#82a2dcd50dc7ea392d5875e10be81c3667ff8133"
   integrity sha512-Yl1E9pu+7PBKSVHZsuw79QVa8ZonpyxBGI/MnuBumiXpxNuNwFo9iZLAAhQGla/LTAt1A7zR4PwgysukxJc0qA==
 
 emoji-regex@^8.0.0:
   version "8.0.0"
@@ -2444,14 +2593,19 @@
   integrity sha512-vbRorB5FUQWvla16U8R/qgaFIya2qGzwDrNmCZuYKrbdSUMG6I1ZCGQRefkRVhuOkIGVne7BQ35DSfo1qvJqFg==
 
 escape-string-regexp@^4.0.0:
   version "4.0.0"
   resolved "https://registry.npmmirror.com/escape-string-regexp/-/escape-string-regexp-4.0.0.tgz#14ba83a5d373e3d311e5afca29cf5bfad965bf34"
   integrity sha512-TtpcNJ3XAzx3Gq8sWRzJaVajRs0uVxA2YAkdb1jm2YkPz4G6egUFAyA3n5vtEIZefPk5Wa4UXbKuS5fKkJWdgA==
 
+escape-string-regexp@^5.0.0:
+  version "5.0.0"
+  resolved "https://registry.npmmirror.com/escape-string-regexp/-/escape-string-regexp-5.0.0.tgz#4683126b500b61762f2dbebace1806e8be31b1c8"
+  integrity sha512-/veY75JbMK4j1yjvuUxuVsiS/hr/4iHs9FTT6cgTexxdE0Ly/glccBAkloH/DofkjRbZU3bnoj38mOmhkZ0lHw==
+
 eslint-config-next@13.2.4:
   version "13.2.4"
   resolved "https://registry.npmmirror.com/eslint-config-next/-/eslint-config-next-13.2.4.tgz#8aa4d42da3a575a814634ba9c88c8d25266c5fdd"
   integrity sha512-lunIBhsoeqw6/Lfkd6zPt25w1bn0znLA/JCL+au1HoEpSb4/PpsOYsYtgV/q+YPsoKIOzFyU5xnb04iZnXjUvg==
   dependencies:
     "@next/eslint-plugin-next" "13.2.4"
     "@rushstack/eslint-patch" "^1.1.3"
@@ -2685,14 +2839,19 @@
     is-stream "^3.0.0"
     merge-stream "^2.0.0"
     npm-run-path "^5.1.0"
     onetime "^6.0.0"
     signal-exit "^3.0.7"
     strip-final-newline "^3.0.0"
 
+extend@^3.0.0:
+  version "3.0.2"
+  resolved "https://registry.npmmirror.com/extend/-/extend-3.0.2.tgz#f8b1136b4071fbd8eb140aff858b1019ec2915fa"
+  integrity sha512-fjquC59cD7CyW6urNXK0FBufkZcoiGG80wTuPujX590cB5Ttln20E2UB4S/WARVqhXffZl2LNgS+gQdPIIim/g==
+
 fast-deep-equal@^3.1.1, fast-deep-equal@^3.1.3:
   version "3.1.3"
   resolved "https://registry.npmmirror.com/fast-deep-equal/-/fast-deep-equal-3.1.3.tgz#3a7d56b559d6cbc3eb512325244e619a65c6c525"
   integrity sha512-f3qQ9oQy9j2AhBe/H9VC91wLmKBCCU/gDOnKNAYG5hswO7BLKj09Hc5HYNz9cGI++xlpDCIgDaitVs03ATR84Q==
 
 fast-glob@^3.2.11, fast-glob@^3.2.12, fast-glob@^3.2.9:
   version "3.2.12"
@@ -2718,14 +2877,21 @@
 fastq@^1.6.0:
   version "1.15.0"
   resolved "https://registry.npmmirror.com/fastq/-/fastq-1.15.0.tgz#d04d07c6a2a68fe4599fea8d2e103a937fae6b3a"
   integrity sha512-wBrocU2LCXXa+lWBt8RoIRD89Fi8OdABODa/kEnyeyjS5aZO5/GNvI5sEINADqP/h8M29UHTHUb53sUu5Ihqdw==
   dependencies:
     reusify "^1.0.4"
 
+fault@^1.0.0:
+  version "1.0.4"
+  resolved "https://registry.npmmirror.com/fault/-/fault-1.0.4.tgz#eafcfc0a6d214fc94601e170df29954a4f842f13"
+  integrity sha512-CJ0HCB5tL5fYTEA7ToAq5+kTwd++Borf1/bifxd9iT70QcXr4MRrO3Llf8Ifs70q+SJcGHFtnIE/Nw6giCtECA==
+  dependencies:
+    format "^0.2.0"
+
 file-entry-cache@^6.0.1:
   version "6.0.1"
   resolved "https://registry.npmmirror.com/file-entry-cache/-/file-entry-cache-6.0.1.tgz#211b2dd9659cb0394b073e7323ac3c933d522027"
   integrity sha512-7Gps/XWymbLk2QLYK4NzpMOrYjMhdIxXuIvy2QBsLE6ljuodKvdkWs/cpyJJ3CVIVpH0Oi1Hvg1ovbMzLdFBBg==
   dependencies:
     flat-cache "^3.0.4"
 
@@ -2786,14 +2952,19 @@
   resolved "https://registry.npmmirror.com/form-data/-/form-data-4.0.0.tgz#93919daeaf361ee529584b9b31664dc12c9fa452"
   integrity sha512-ETEklSGi5t0QMZuiXoA/Q6vcnxcLQP5vdugSpuAyi6SVGi2clPPp+xgEhuMaHC+zGgn31Kd235W35f7Hykkaww==
   dependencies:
     asynckit "^0.4.0"
     combined-stream "^1.0.8"
     mime-types "^2.1.12"
 
+format@^0.2.0:
+  version "0.2.2"
+  resolved "https://registry.npmmirror.com/format/-/format-0.2.2.tgz#d6170107e9efdc4ed30c9dc39016df942b5cb58b"
+  integrity sha512-wzsgA6WOq+09wrU1tsJ09udeR/YZRaeArL9e1wPbFg3GG2yDnC2ldKpxs4xunpFF9DgqCqOIra3bc1HWrJ37Ww==
+
 framer-motion@^10.10.0:
   version "10.12.10"
   resolved "https://registry.npmmirror.com/framer-motion/-/framer-motion-10.12.10.tgz#39aff293d8c520f6d9a4a34bf25121a8f1a12d6d"
   integrity sha512-f/VkrpxfG4xSmBi105/NCfcTt219IgglQEUR0BsuFZAg+be6N3QAcujFyBEvBvbDOSP9Ccv6OMiaY0HFMnBoMA==
   dependencies:
     tslib "^2.4.0"
   optionalDependencies:
@@ -3022,14 +3193,40 @@
 has@^1.0.3:
   version "1.0.3"
   resolved "https://registry.npmmirror.com/has/-/has-1.0.3.tgz#722d7cbfc1f6aa8241f16dd814e011e1f41e8796"
   integrity sha512-f2dvO0VU6Oej7RkWJGrehjbzMAjFp5/VKPp5tTpWIV4JHHZK1/BxbFRtf/siA2SWTe09caDmVtYYzWEIbBS4zw==
   dependencies:
     function-bind "^1.1.1"
 
+hast-util-parse-selector@^2.0.0:
+  version "2.2.5"
+  resolved "https://registry.npmmirror.com/hast-util-parse-selector/-/hast-util-parse-selector-2.2.5.tgz#d57c23f4da16ae3c63b3b6ca4616683313499c3a"
+  integrity sha512-7j6mrk/qqkSehsM92wQjdIgWM2/BW61u/53G6xmC8i1OmEdKLHbk419QKQUjz6LglWsfqoiHmyMRkP1BGjecNQ==
+
+hast-util-whitespace@^2.0.0:
+  version "2.0.1"
+  resolved "https://registry.npmmirror.com/hast-util-whitespace/-/hast-util-whitespace-2.0.1.tgz#0ec64e257e6fc216c7d14c8a1b74d27d650b4557"
+  integrity sha512-nAxA0v8+vXSBDt3AnRUNjyRIQ0rD+ntpbAp4LnPkumc5M9yUbSMa4XDU9Q6etY4f1Wp4bNgvc1yjiZtsTTrSng==
+
+hastscript@^6.0.0:
+  version "6.0.0"
+  resolved "https://registry.npmmirror.com/hastscript/-/hastscript-6.0.0.tgz#e8768d7eac56c3fdeac8a92830d58e811e5bf640"
+  integrity sha512-nDM6bvd7lIqDUiYEiu5Sl/+6ReP0BMk/2f4U/Rooccxkj0P5nm+acM5PrGJ/t5I8qPGiqZSE6hVAwZEdZIvP4w==
+  dependencies:
+    "@types/hast" "^2.0.0"
+    comma-separated-tokens "^1.0.0"
+    hast-util-parse-selector "^2.0.0"
+    property-information "^5.0.0"
+    space-separated-tokens "^1.0.0"
+
+highlight.js@^10.4.1, highlight.js@~10.7.0:
+  version "10.7.3"
+  resolved "https://registry.npmmirror.com/highlight.js/-/highlight.js-10.7.3.tgz#697272e3991356e40c3cac566a74eef681756531"
+  integrity sha512-tzcUFauisWKNHaRkN4Wjl/ZA07gENAjFl3J/c480dprkGTg5EQstgaNFqBfUqCq54kZRIEcreTsAgF/m2quD7A==
+
 hoist-non-react-statics@^3.3.1:
   version "3.3.2"
   resolved "https://registry.npmmirror.com/hoist-non-react-statics/-/hoist-non-react-statics-3.3.2.tgz#ece0acaf71d62c2969c2ec59feff42a4b1a85b45"
   integrity sha512-/gGivxi8JPKWNm/W0jSmzcMPpfpPLc3dY/6GxhX2hQ9iGj3aDfklV4ET7NjKpSinLpJ5vafa9iiGIEZg10SfBw==
   dependencies:
     react-is "^16.7.0"
 
@@ -3080,14 +3277,19 @@
     wrappy "1"
 
 inherits@2, inherits@~2.0.3:
   version "2.0.4"
   resolved "https://registry.npmmirror.com/inherits/-/inherits-2.0.4.tgz#0fa2c64f932917c3433a0ded55363aae37416b7c"
   integrity sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==
 
+inline-style-parser@0.1.1:
+  version "0.1.1"
+  resolved "https://registry.npmmirror.com/inline-style-parser/-/inline-style-parser-0.1.1.tgz#ec8a3b429274e9c0a1f1c4ffa9453a7fef72cea1"
+  integrity sha512-7NXolsK4CAS5+xvdj5OMMbI962hU/wvwoxk+LWR9Ek9bVtyuuYScDN6eS0rUm6TxApFpw7CX1o4uJzcd4AyD3Q==
+
 internal-slot@^1.0.3, internal-slot@^1.0.4, internal-slot@^1.0.5:
   version "1.0.5"
   resolved "https://registry.npmmirror.com/internal-slot/-/internal-slot-1.0.5.tgz#f2a2ee21f668f8627a4667f309dc0f4fb6674986"
   integrity sha512-Y+R5hJrzs52QCG2laLn4udYVnxsfny9CpOhNhUvk/SSSVyF6T27FzRbF0sroPidSu3X8oEAkOn2K804mjpt6UQ==
   dependencies:
     get-intrinsic "^1.2.0"
     has "^1.0.3"
@@ -3101,14 +3303,27 @@
 invariant@^2.2.4:
   version "2.2.4"
   resolved "https://registry.npmmirror.com/invariant/-/invariant-2.2.4.tgz#610f3c92c9359ce1db616e538008d23ff35158e6"
   integrity sha512-phJfQVBuaJM5raOpJjSfkiD6BpbCE4Ns//LaXl6wGYtUBY83nWS6Rf9tXm2e8VaK60JEjYldbPif/A2B1C2gNA==
   dependencies:
     loose-envify "^1.0.0"
 
+is-alphabetical@^1.0.0:
+  version "1.0.4"
+  resolved "https://registry.npmmirror.com/is-alphabetical/-/is-alphabetical-1.0.4.tgz#9e7d6b94916be22153745d184c298cbf986a686d"
+  integrity sha512-DwzsA04LQ10FHTZuL0/grVDk4rFoVH1pjAToYwBrHSxcrBIGQuXrQMtD5U1b0U2XVgKZCTLLP8u2Qxqhy3l2Vg==
+
+is-alphanumerical@^1.0.0:
+  version "1.0.4"
+  resolved "https://registry.npmmirror.com/is-alphanumerical/-/is-alphanumerical-1.0.4.tgz#7eb9a2431f855f6b1ef1a78e326df515696c4dbf"
+  integrity sha512-UzoZUr+XfVz3t3v4KyGEniVL9BDRoQtY7tOyrRybkVNjDFWyo1yhXNGrrBTQxp3ib9BLAWs7k2YKBQsFRkZG9A==
+  dependencies:
+    is-alphabetical "^1.0.0"
+    is-decimal "^1.0.0"
+
 is-any-array@^2.0.0:
   version "2.0.1"
   resolved "https://registry.npmmirror.com/is-any-array/-/is-any-array-2.0.1.tgz#9233242a9c098220290aa2ec28f82ca7fa79899e"
   integrity sha512-UtilS7hLRu++wb/WBAw9bNuP1Eg04Ivn1vERJck8zJthEvXCBEBpGR/33u/xLKWEQf95803oalHrVDptcAvFdQ==
 
 is-arguments@^1.1.1:
   version "1.1.1"
@@ -3150,14 +3365,19 @@
   version "1.1.2"
   resolved "https://registry.npmmirror.com/is-boolean-object/-/is-boolean-object-1.1.2.tgz#5c6dc200246dd9321ae4b885a114bb1f75f63719"
   integrity sha512-gDYaKHJmnj4aWxyj6YHyXVpdQawtVLHU5cb+eztPGczf6cjuTdwve5ZIEfgXqH4e57An1D1AKf8CZ3kYrQRqYA==
   dependencies:
     call-bind "^1.0.2"
     has-tostringtag "^1.0.0"
 
+is-buffer@^2.0.0:
+  version "2.0.5"
+  resolved "https://registry.npmmirror.com/is-buffer/-/is-buffer-2.0.5.tgz#ebc252e400d22ff8d77fa09888821a24a658c191"
+  integrity sha512-i2R6zNFDwgEHJyQUtJEk0XFi1i0dPFn/oqjK3/vPCcDeJvW5NQ83V8QbicfF1SupOaB0h8ntgBC2YiE7dfyctQ==
+
 is-callable@^1.1.3, is-callable@^1.1.4, is-callable@^1.2.7:
   version "1.2.7"
   resolved "https://registry.npmmirror.com/is-callable/-/is-callable-1.2.7.tgz#3bc2a85ea742d9e36205dcacdd72ca1fdc51b055"
   integrity sha512-1BC0BVFhS/p0qtw6enp8e+8OD0UrK0oFLztSjNzhcKA3WDuJxxAPXzPuPtKkjEY9UUoEWlX/8fgKeu2S8i9JTA==
 
 is-core-module@^2.11.0, is-core-module@^2.9.0:
   version "2.12.0"
@@ -3169,14 +3389,19 @@
 is-date-object@^1.0.1, is-date-object@^1.0.5:
   version "1.0.5"
   resolved "https://registry.npmmirror.com/is-date-object/-/is-date-object-1.0.5.tgz#0841d5536e724c25597bf6ea62e1bd38298df31f"
   integrity sha512-9YQaSxsAiSwcvS33MBk3wTCVnWK+HhF8VZR2jRxehM16QcVOdHqPn4VPHmRK4lSr38n9JriurInLcP90xsYNfQ==
   dependencies:
     has-tostringtag "^1.0.0"
 
+is-decimal@^1.0.0:
+  version "1.0.4"
+  resolved "https://registry.npmmirror.com/is-decimal/-/is-decimal-1.0.4.tgz#65a3a5958a1c5b63a706e1b333d7cd9f630d3fa5"
+  integrity sha512-RGdriMmQQvZ2aqaQq3awNA6dCGtKpiDFcOzrTWrDAT2MiWrKQVPmxLGHl7Y2nNu6led0kEyoX0enY0qXYsv9zw==
+
 is-docker@^2.0.0, is-docker@^2.1.1:
   version "2.2.1"
   resolved "https://registry.npmmirror.com/is-docker/-/is-docker-2.2.1.tgz#33eeabe23cfe86f14bde4408a02c0cfb853acdaa"
   integrity sha512-F+i2BKsFrH66iaUFc0woD8sLy8getkwTwtOBjvs56Cx4CgJDeKQeqfz8wAYiSb8JOprWhHH5p77PbmYCvvUuXQ==
 
 is-docker@^3.0.0:
   version "3.0.0"
@@ -3196,14 +3421,19 @@
 is-glob@^4.0.0, is-glob@^4.0.1, is-glob@^4.0.3, is-glob@~4.0.1:
   version "4.0.3"
   resolved "https://registry.npmmirror.com/is-glob/-/is-glob-4.0.3.tgz#64f61e42cbbb2eec2071a9dac0b28ba1e65d5084"
   integrity sha512-xelSayHH36ZgE7ZWhli7pW34hNbNl8Ojv5KVmkJD4hBdD3th8Tfk9vYasLM+mXWOZhFkgZfxhLSnrwRr4elSSg==
   dependencies:
     is-extglob "^2.1.1"
 
+is-hexadecimal@^1.0.0:
+  version "1.0.4"
+  resolved "https://registry.npmmirror.com/is-hexadecimal/-/is-hexadecimal-1.0.4.tgz#cc35c97588da4bd49a8eedd6bc4082d44dcb23a7"
+  integrity sha512-gyPJuv83bHMpocVYoqof5VDiZveEoGoFL8m3BXNb2VW8Xs+rz9kqO8LOQ5DH6EsuvilT1ApazU0pyl+ytbPtlw==
+
 is-inside-container@^1.0.0:
   version "1.0.0"
   resolved "https://registry.npmmirror.com/is-inside-container/-/is-inside-container-1.0.0.tgz#e81fba699662eb31dbdaf26766a61d4814717ea4"
   integrity sha512-KIYLCCJghfHZxqjYBE7rEy0OBuTd5xCHS7tHVgvCLkx7StIoaxwNW3hCALgEUjFfeRk+MG/Qxmp/vtETEF3tRA==
   dependencies:
     is-docker "^3.0.0"
 
@@ -3230,14 +3460,19 @@
   integrity sha512-41Cifkg6e8TylSpdtTpeLVMqvSBEVzTttHvERD741+pnZ8ANv0004MRL43QKPDlK9cGvNp6NZWZUBlbGXYxxng==
 
 is-path-inside@^3.0.3:
   version "3.0.3"
   resolved "https://registry.npmmirror.com/is-path-inside/-/is-path-inside-3.0.3.tgz#d231362e53a07ff2b0e0ea7fed049161ffd16283"
   integrity sha512-Fd4gABb+ycGAmKou8eMftCupSir5lRxqf4aD/vd0cD2qc4HL07OjCeuHMr8Ro4CoMaeCKDB0/ECBOVWjTwUvPQ==
 
+is-plain-obj@^4.0.0:
+  version "4.1.0"
+  resolved "https://registry.npmmirror.com/is-plain-obj/-/is-plain-obj-4.1.0.tgz#d65025edec3657ce032fd7db63c97883eaed71f0"
+  integrity sha512-+Pgi+vMuUNkJyExiMBt5IlFoMyKnr5zhJ4Uspz58WOhBF5QoIZkFyNHIbBAtHwzVAgk5RtndVNsDRN61/mmDqg==
+
 is-regex@^1.1.4:
   version "1.1.4"
   resolved "https://registry.npmmirror.com/is-regex/-/is-regex-1.1.4.tgz#eef5663cd59fa4c0ae339505323df6854bb15958"
   integrity sha512-kvRdxDsxZjhzUX07ZnLydzS1TU/TJlTUHHY4YLL87e37oUA49DfkLqgy+VjFocowy29cKvcSiu+kIv728jTTVg==
   dependencies:
     call-bind "^1.0.2"
     has-tostringtag "^1.0.0"
@@ -3399,14 +3634,19 @@
   integrity sha512-xXDvecyTpGLrqFrvkrUSoxxfJI5AH7U8zxxtVclpsUtMCq4JQ290LY8AW5c7Ggnr/Y/oK+bQMbqK2qmtk3pN4g==
   dependencies:
     lie "~3.3.0"
     pako "~1.0.2"
     readable-stream "~2.3.6"
     setimmediate "^1.0.5"
 
+kleur@^4.0.3:
+  version "4.1.5"
+  resolved "https://registry.npmmirror.com/kleur/-/kleur-4.1.5.tgz#95106101795f7050c6c650f350c683febddb1780"
+  integrity sha512-o+NO+8WrRiQEE4/7nwRJhN1HWpVmJm511pBHUxPLtp0BUISzlBplORYSmTclCnJvQq2tKu/sgl3xVpkc7ZWuQQ==
+
 language-subtag-registry@~0.3.2:
   version "0.3.22"
   resolved "https://registry.npmmirror.com/language-subtag-registry/-/language-subtag-registry-0.3.22.tgz#2e1500861b2e457eba7e7ae86877cbd08fa1fd1d"
   integrity sha512-tN0MCzyWnoz/4nHS6uxdlFWoUZT7ABptwKPQ52Ea7URk6vll88bWBVhodtnlfEuCcKWNGoc+uGbw1cwa9IKh/w==
 
 language-tags@=1.0.5:
   version "1.0.5"
@@ -3438,41 +3678,59 @@
 locate-path@^6.0.0:
   version "6.0.0"
   resolved "https://registry.npmmirror.com/locate-path/-/locate-path-6.0.0.tgz#55321eb309febbc59c4801d931a72452a681d286"
   integrity sha512-iPZK6eYjbxRu3uB4/WZ3EsEIMJFMqAoopl3R+zuq0UjcAm/MO6KCweDgPfP3elTztoKP3KtnVHxTn2NHBSDVUw==
   dependencies:
     p-locate "^5.0.0"
 
+lodash-es@^4.17.15:
+  version "4.17.21"
+  resolved "https://registry.npmmirror.com/lodash-es/-/lodash-es-4.17.21.tgz#43e626c46e6591b7750beb2b50117390c609e3ee"
+  integrity sha512-mKnC+QJ9pWVzv+C4/U3rRsHapFfHvQFoFB92e52xeyGMcX6/OlIl78je1u8vePzYZSkkogMPJ2yjxxsb89cxyw==
+
 lodash.merge@^4.6.2:
   version "4.6.2"
   resolved "https://registry.npmmirror.com/lodash.merge/-/lodash.merge-4.6.2.tgz#558aa53b43b661e1925a0afdfa36a9a1085fe57a"
   integrity sha512-0KpjqXRVvrYyCsX1swR/XTK0va6VQkQM6MNo7PqW77ByjAhoARA8EfrP1N4+KlKj8YS0ZUCtRT/YUuhyYDujIQ==
 
 lodash.mergewith@4.6.2:
   version "4.6.2"
   resolved "https://registry.npmmirror.com/lodash.mergewith/-/lodash.mergewith-4.6.2.tgz#617121f89ac55f59047c7aec1ccd6654c6590f55"
   integrity sha512-GK3g5RPZWTRSeLSpgP8Xhra+pnjBC56q9FZYe1d5RN3TJ35dbkGy3YqBSMbyCrlbi+CM9Z3Jk5yTL7RCsqboyQ==
 
-lodash@^4.17.21:
+lodash@^4.0.1, lodash@^4.17.15, lodash@^4.17.21:
   version "4.17.21"
   resolved "https://registry.npmmirror.com/lodash/-/lodash-4.17.21.tgz#679591c564c3bffaae8454cf0b3df370c3d6911c"
   integrity sha512-v2kDEe57lecTulaDIuNTPy3Ry4gLGJ6Z1O3vE1krgXZNrsQ+LFTGHVxVjcXPs17LhbZVGedAJv8XZ1tvj5FvSg==
 
+longest-streak@^3.0.0:
+  version "3.1.0"
+  resolved "https://registry.npmmirror.com/longest-streak/-/longest-streak-3.1.0.tgz#62fa67cd958742a1574af9f39866364102d90cd4"
+  integrity sha512-9Ri+o0JYgehTaVBBDoMqIl8GXtbWg711O3srftcHhZ0dqnETqLaoIK0x17fUw9rFSlK/0NlsKe0Ahhyl5pXE2g==
+
 loose-envify@^1.0.0, loose-envify@^1.1.0, loose-envify@^1.4.0:
   version "1.4.0"
   resolved "https://registry.npmmirror.com/loose-envify/-/loose-envify-1.4.0.tgz#71ee51fa7be4caec1a63839f7e682d8132d30caf"
   integrity sha512-lyuxPGr/Wfhrlem2CL/UcnUc1zcqKAImBDzukY7Y5F/yQiNdko6+fRLevlw1HgMySw7f611UIY408EtxRSoK3Q==
   dependencies:
     js-tokens "^3.0.0 || ^4.0.0"
 
 lottie-web@^5.11.0:
   version "5.11.0"
   resolved "https://registry.npmmirror.com/lottie-web/-/lottie-web-5.11.0.tgz#04bb9fd6cdfbb10e586985dd666de6c727619d95"
   integrity sha512-9vSt0AtdOH98GKDXwD5LPfFg9Pcmxt5+1BllAbudKM5iqPxpJnJUfuGaP45OyudDrESCOBgsjnntVUTygBNlzw==
 
+lowlight@^1.17.0:
+  version "1.20.0"
+  resolved "https://registry.npmmirror.com/lowlight/-/lowlight-1.20.0.tgz#ddb197d33462ad0d93bf19d17b6c301aa3941888"
+  integrity sha512-8Ktj+prEb1RoCPkEOrPMYUN/nCggB7qAWe3a7OpMjWQkh3l2RD5wKRQ+o8Q8YuI9RG/xs95waaI/E6ym/7NsTw==
+  dependencies:
+    fault "^1.0.0"
+    highlight.js "~10.7.0"
+
 lru-cache@^5.1.1:
   version "5.1.1"
   resolved "https://registry.npmmirror.com/lru-cache/-/lru-cache-5.1.1.tgz#1da27e6710271947695daf6848e847f01d84b920"
   integrity sha512-KpNARQA3Iwv+jTA0utUVVbrh+Jlrr1Fv0e56GGzAFOXN7dk/FviaDW8LHmK52DlcH4WP2n6gI8vN1aesBFgo9w==
   dependencies:
     yallist "^3.0.2"
 
@@ -3486,24 +3744,451 @@
 magic-string@^0.27.0:
   version "0.27.0"
   resolved "https://registry.npmmirror.com/magic-string/-/magic-string-0.27.0.tgz#e4a3413b4bab6d98d2becffd48b4a257effdbbf3"
   integrity sha512-8UnnX2PeRAPZuN12svgR9j7M1uWMovg/CEnIwIG0LFkXSJJe4PdfUGiTGl8V9bsBHFUtfVINcSyYxd7q+kx9fA==
   dependencies:
     "@jridgewell/sourcemap-codec" "^1.4.13"
 
+markdown-table@^3.0.0:
+  version "3.0.3"
+  resolved "https://registry.npmmirror.com/markdown-table/-/markdown-table-3.0.3.tgz#e6331d30e493127e031dd385488b5bd326e4a6bd"
+  integrity sha512-Z1NL3Tb1M9wH4XESsCDEksWoKTdlUafKc4pt0GRwjUyXaCFZ+dc3g2erqB6zm3szA2IUSi7VnPI+o/9jnxh9hw==
+
+material-colors@^1.2.1:
+  version "1.2.6"
+  resolved "https://registry.npmmirror.com/material-colors/-/material-colors-1.2.6.tgz#6d1958871126992ceecc72f4bcc4d8f010865f46"
+  integrity sha512-6qE4B9deFBIa9YSpOc9O0Sgc43zTeVYbgDT5veRKSlB2+ZuHNoVVxA1L/ckMUayV9Ay9y7Z/SZCLcGteW9i7bg==
+
+mdast-util-definitions@^5.0.0:
+  version "5.1.2"
+  resolved "https://registry.npmmirror.com/mdast-util-definitions/-/mdast-util-definitions-5.1.2.tgz#9910abb60ac5d7115d6819b57ae0bcef07a3f7a7"
+  integrity sha512-8SVPMuHqlPME/z3gqVwWY4zVXn8lqKv/pAhC57FuJ40ImXyBpmO5ukh98zB2v7Blql2FiHjHv9LVztSIqjY+MA==
+  dependencies:
+    "@types/mdast" "^3.0.0"
+    "@types/unist" "^2.0.0"
+    unist-util-visit "^4.0.0"
+
+mdast-util-find-and-replace@^2.0.0:
+  version "2.2.2"
+  resolved "https://registry.npmmirror.com/mdast-util-find-and-replace/-/mdast-util-find-and-replace-2.2.2.tgz#cc2b774f7f3630da4bd592f61966fecade8b99b1"
+  integrity sha512-MTtdFRz/eMDHXzeK6W3dO7mXUlF82Gom4y0oOgvHhh/HXZAGvIQDUvQ0SuUx+j2tv44b8xTHOm8K/9OoRFnXKw==
+  dependencies:
+    "@types/mdast" "^3.0.0"
+    escape-string-regexp "^5.0.0"
+    unist-util-is "^5.0.0"
+    unist-util-visit-parents "^5.0.0"
+
+mdast-util-from-markdown@^1.0.0:
+  version "1.3.0"
+  resolved "https://registry.npmmirror.com/mdast-util-from-markdown/-/mdast-util-from-markdown-1.3.0.tgz#0214124154f26154a2b3f9d401155509be45e894"
+  integrity sha512-HN3W1gRIuN/ZW295c7zi7g9lVBllMgZE40RxCX37wrTPWXCWtpvOZdfnuK+1WNpvZje6XuJeI3Wnb4TJEUem+g==
+  dependencies:
+    "@types/mdast" "^3.0.0"
+    "@types/unist" "^2.0.0"
+    decode-named-character-reference "^1.0.0"
+    mdast-util-to-string "^3.1.0"
+    micromark "^3.0.0"
+    micromark-util-decode-numeric-character-reference "^1.0.0"
+    micromark-util-decode-string "^1.0.0"
+    micromark-util-normalize-identifier "^1.0.0"
+    micromark-util-symbol "^1.0.0"
+    micromark-util-types "^1.0.0"
+    unist-util-stringify-position "^3.0.0"
+    uvu "^0.5.0"
+
+mdast-util-gfm-autolink-literal@^1.0.0:
+  version "1.0.3"
+  resolved "https://registry.npmmirror.com/mdast-util-gfm-autolink-literal/-/mdast-util-gfm-autolink-literal-1.0.3.tgz#67a13abe813d7eba350453a5333ae1bc0ec05c06"
+  integrity sha512-My8KJ57FYEy2W2LyNom4n3E7hKTuQk/0SES0u16tjA9Z3oFkF4RrC/hPAPgjlSpezsOvI8ObcXcElo92wn5IGA==
+  dependencies:
+    "@types/mdast" "^3.0.0"
+    ccount "^2.0.0"
+    mdast-util-find-and-replace "^2.0.0"
+    micromark-util-character "^1.0.0"
+
+mdast-util-gfm-footnote@^1.0.0:
+  version "1.0.2"
+  resolved "https://registry.npmmirror.com/mdast-util-gfm-footnote/-/mdast-util-gfm-footnote-1.0.2.tgz#ce5e49b639c44de68d5bf5399877a14d5020424e"
+  integrity sha512-56D19KOGbE00uKVj3sgIykpwKL179QsVFwx/DCW0u/0+URsryacI4MAdNJl0dh+u2PSsD9FtxPFbHCzJ78qJFQ==
+  dependencies:
+    "@types/mdast" "^3.0.0"
+    mdast-util-to-markdown "^1.3.0"
+    micromark-util-normalize-identifier "^1.0.0"
+
+mdast-util-gfm-strikethrough@^1.0.0:
+  version "1.0.3"
+  resolved "https://registry.npmmirror.com/mdast-util-gfm-strikethrough/-/mdast-util-gfm-strikethrough-1.0.3.tgz#5470eb105b483f7746b8805b9b989342085795b7"
+  integrity sha512-DAPhYzTYrRcXdMjUtUjKvW9z/FNAMTdU0ORyMcbmkwYNbKocDpdk+PX1L1dQgOID/+vVs1uBQ7ElrBQfZ0cuiQ==
+  dependencies:
+    "@types/mdast" "^3.0.0"
+    mdast-util-to-markdown "^1.3.0"
+
+mdast-util-gfm-table@^1.0.0:
+  version "1.0.7"
+  resolved "https://registry.npmmirror.com/mdast-util-gfm-table/-/mdast-util-gfm-table-1.0.7.tgz#3552153a146379f0f9c4c1101b071d70bbed1a46"
+  integrity sha512-jjcpmNnQvrmN5Vx7y7lEc2iIOEytYv7rTvu+MeyAsSHTASGCCRA79Igg2uKssgOs1i1po8s3plW0sTu1wkkLGg==
+  dependencies:
+    "@types/mdast" "^3.0.0"
+    markdown-table "^3.0.0"
+    mdast-util-from-markdown "^1.0.0"
+    mdast-util-to-markdown "^1.3.0"
+
+mdast-util-gfm-task-list-item@^1.0.0:
+  version "1.0.2"
+  resolved "https://registry.npmmirror.com/mdast-util-gfm-task-list-item/-/mdast-util-gfm-task-list-item-1.0.2.tgz#b280fcf3b7be6fd0cc012bbe67a59831eb34097b"
+  integrity sha512-PFTA1gzfp1B1UaiJVyhJZA1rm0+Tzn690frc/L8vNX1Jop4STZgOE6bxUhnzdVSB+vm2GU1tIsuQcA9bxTQpMQ==
+  dependencies:
+    "@types/mdast" "^3.0.0"
+    mdast-util-to-markdown "^1.3.0"
+
+mdast-util-gfm@^2.0.0:
+  version "2.0.2"
+  resolved "https://registry.npmmirror.com/mdast-util-gfm/-/mdast-util-gfm-2.0.2.tgz#e92f4d8717d74bdba6de57ed21cc8b9552e2d0b6"
+  integrity sha512-qvZ608nBppZ4icQlhQQIAdc6S3Ffj9RGmzwUKUWuEICFnd1LVkN3EktF7ZHAgfcEdvZB5owU9tQgt99e2TlLjg==
+  dependencies:
+    mdast-util-from-markdown "^1.0.0"
+    mdast-util-gfm-autolink-literal "^1.0.0"
+    mdast-util-gfm-footnote "^1.0.0"
+    mdast-util-gfm-strikethrough "^1.0.0"
+    mdast-util-gfm-table "^1.0.0"
+    mdast-util-gfm-task-list-item "^1.0.0"
+    mdast-util-to-markdown "^1.0.0"
+
+mdast-util-phrasing@^3.0.0:
+  version "3.0.1"
+  resolved "https://registry.npmmirror.com/mdast-util-phrasing/-/mdast-util-phrasing-3.0.1.tgz#c7c21d0d435d7fb90956038f02e8702781f95463"
+  integrity sha512-WmI1gTXUBJo4/ZmSk79Wcb2HcjPJBzM1nlI/OUWA8yk2X9ik3ffNbBGsU+09BFmXaL1IBb9fiuvq6/KMiNycSg==
+  dependencies:
+    "@types/mdast" "^3.0.0"
+    unist-util-is "^5.0.0"
+
+mdast-util-to-hast@^12.1.0:
+  version "12.3.0"
+  resolved "https://registry.npmmirror.com/mdast-util-to-hast/-/mdast-util-to-hast-12.3.0.tgz#045d2825fb04374e59970f5b3f279b5700f6fb49"
+  integrity sha512-pits93r8PhnIoU4Vy9bjW39M2jJ6/tdHyja9rrot9uujkN7UTU9SDnE6WNJz/IGyQk3XHX6yNNtrBH6cQzm8Hw==
+  dependencies:
+    "@types/hast" "^2.0.0"
+    "@types/mdast" "^3.0.0"
+    mdast-util-definitions "^5.0.0"
+    micromark-util-sanitize-uri "^1.1.0"
+    trim-lines "^3.0.0"
+    unist-util-generated "^2.0.0"
+    unist-util-position "^4.0.0"
+    unist-util-visit "^4.0.0"
+
+mdast-util-to-markdown@^1.0.0, mdast-util-to-markdown@^1.3.0:
+  version "1.5.0"
+  resolved "https://registry.npmmirror.com/mdast-util-to-markdown/-/mdast-util-to-markdown-1.5.0.tgz#c13343cb3fc98621911d33b5cd42e7d0731171c6"
+  integrity sha512-bbv7TPv/WC49thZPg3jXuqzuvI45IL2EVAr/KxF0BSdHsU0ceFHOmwQn6evxAh1GaoK/6GQ1wp4R4oW2+LFL/A==
+  dependencies:
+    "@types/mdast" "^3.0.0"
+    "@types/unist" "^2.0.0"
+    longest-streak "^3.0.0"
+    mdast-util-phrasing "^3.0.0"
+    mdast-util-to-string "^3.0.0"
+    micromark-util-decode-string "^1.0.0"
+    unist-util-visit "^4.0.0"
+    zwitch "^2.0.0"
+
+mdast-util-to-string@^3.0.0, mdast-util-to-string@^3.1.0:
+  version "3.2.0"
+  resolved "https://registry.npmmirror.com/mdast-util-to-string/-/mdast-util-to-string-3.2.0.tgz#66f7bb6324756741c5f47a53557f0cbf16b6f789"
+  integrity sha512-V4Zn/ncyN1QNSqSBxTrMOLpjr+IKdHl2v3KVLoWmDPscP4r9GcCi71gjgvUV1SFSKh92AjAG4peFuBl2/YgCJg==
+  dependencies:
+    "@types/mdast" "^3.0.0"
+
+memoize-one@^6.0.0:
+  version "6.0.0"
+  resolved "https://registry.npmmirror.com/memoize-one/-/memoize-one-6.0.0.tgz#b2591b871ed82948aee4727dc6abceeeac8c1045"
+  integrity sha512-rkpe71W0N0c0Xz6QD0eJETuWAJGnJ9afsl1srmwPrI+yBCkge5EycXXbYRyvL29zZVUWQCY7InPRCv3GDXuZNw==
+
 merge-stream@^2.0.0:
   version "2.0.0"
   resolved "https://registry.npmmirror.com/merge-stream/-/merge-stream-2.0.0.tgz#52823629a14dd00c9770fb6ad47dc6310f2c1f60"
   integrity sha512-abv/qOcuPfk3URPfDzmZU1LKmuw8kT+0nIHvKrKgFrwifol/doWcdA4ZqsWQ8ENrFKkd67Mfpo/LovbIUsbt3w==
 
 merge2@^1.3.0, merge2@^1.4.1:
   version "1.4.1"
   resolved "https://registry.npmmirror.com/merge2/-/merge2-1.4.1.tgz#4368892f885e907455a6fd7dc55c0c9d404990ae"
   integrity sha512-8q7VEgMJW4J8tcfVPy8g09NcQwZdbwFEqhe/WZkoIzjn/3TGDwtOCYtXGxA3O8tPzpczCCDgv+P2P5y00ZJOOg==
 
+micromark-core-commonmark@^1.0.0, micromark-core-commonmark@^1.0.1:
+  version "1.0.6"
+  resolved "https://registry.npmmirror.com/micromark-core-commonmark/-/micromark-core-commonmark-1.0.6.tgz#edff4c72e5993d93724a3c206970f5a15b0585ad"
+  integrity sha512-K+PkJTxqjFfSNkfAhp4GB+cZPfQd6dxtTXnf+RjZOV7T4EEXnvgzOcnp+eSTmpGk9d1S9sL6/lqrgSNn/s0HZA==
+  dependencies:
+    decode-named-character-reference "^1.0.0"
+    micromark-factory-destination "^1.0.0"
+    micromark-factory-label "^1.0.0"
+    micromark-factory-space "^1.0.0"
+    micromark-factory-title "^1.0.0"
+    micromark-factory-whitespace "^1.0.0"
+    micromark-util-character "^1.0.0"
+    micromark-util-chunked "^1.0.0"
+    micromark-util-classify-character "^1.0.0"
+    micromark-util-html-tag-name "^1.0.0"
+    micromark-util-normalize-identifier "^1.0.0"
+    micromark-util-resolve-all "^1.0.0"
+    micromark-util-subtokenize "^1.0.0"
+    micromark-util-symbol "^1.0.0"
+    micromark-util-types "^1.0.1"
+    uvu "^0.5.0"
+
+micromark-extension-gfm-autolink-literal@^1.0.0:
+  version "1.0.4"
+  resolved "https://registry.npmmirror.com/micromark-extension-gfm-autolink-literal/-/micromark-extension-gfm-autolink-literal-1.0.4.tgz#3a8af48264be47138654ab0b8700a8e22785ef07"
+  integrity sha512-WCssN+M9rUyfHN5zPBn3/f0mIA7tqArHL/EKbv3CZK+LT2rG77FEikIQEqBkv46fOqXQK4NEW/Pc7Z27gshpeg==
+  dependencies:
+    micromark-util-character "^1.0.0"
+    micromark-util-sanitize-uri "^1.0.0"
+    micromark-util-symbol "^1.0.0"
+    micromark-util-types "^1.0.0"
+
+micromark-extension-gfm-footnote@^1.0.0:
+  version "1.1.0"
+  resolved "https://registry.npmmirror.com/micromark-extension-gfm-footnote/-/micromark-extension-gfm-footnote-1.1.0.tgz#73e3db823db9defef25f68074cb4cf4bb9cf6a8c"
+  integrity sha512-RWYce7j8+c0n7Djzv5NzGEGitNNYO3uj+h/XYMdS/JinH1Go+/Qkomg/rfxExFzYTiydaV6GLeffGO5qcJbMPA==
+  dependencies:
+    micromark-core-commonmark "^1.0.0"
+    micromark-factory-space "^1.0.0"
+    micromark-util-character "^1.0.0"
+    micromark-util-normalize-identifier "^1.0.0"
+    micromark-util-sanitize-uri "^1.0.0"
+    micromark-util-symbol "^1.0.0"
+    micromark-util-types "^1.0.0"
+    uvu "^0.5.0"
+
+micromark-extension-gfm-strikethrough@^1.0.0:
+  version "1.0.5"
+  resolved "https://registry.npmmirror.com/micromark-extension-gfm-strikethrough/-/micromark-extension-gfm-strikethrough-1.0.5.tgz#4db40b87d674a6fe1d00d59ac91118e4f5960f12"
+  integrity sha512-X0oI5eYYQVARhiNfbETy7BfLSmSilzN1eOuoRnrf9oUNsPRrWOAe9UqSizgw1vNxQBfOwL+n2610S3bYjVNi7w==
+  dependencies:
+    micromark-util-chunked "^1.0.0"
+    micromark-util-classify-character "^1.0.0"
+    micromark-util-resolve-all "^1.0.0"
+    micromark-util-symbol "^1.0.0"
+    micromark-util-types "^1.0.0"
+    uvu "^0.5.0"
+
+micromark-extension-gfm-table@^1.0.0:
+  version "1.0.6"
+  resolved "https://registry.npmmirror.com/micromark-extension-gfm-table/-/micromark-extension-gfm-table-1.0.6.tgz#22b2b18dff9db39bdb29d6017e53bdd370672c8e"
+  integrity sha512-92pq7Q+T+4kXH4M6kL+pc8WU23Z9iuhcqmtYFWdFWjm73ZscFpH2xE28+XFpGWlvgq3LUwcN0XC0PGCicYFpgA==
+  dependencies:
+    micromark-factory-space "^1.0.0"
+    micromark-util-character "^1.0.0"
+    micromark-util-symbol "^1.0.0"
+    micromark-util-types "^1.0.0"
+    uvu "^0.5.0"
+
+micromark-extension-gfm-tagfilter@^1.0.0:
+  version "1.0.2"
+  resolved "https://registry.npmmirror.com/micromark-extension-gfm-tagfilter/-/micromark-extension-gfm-tagfilter-1.0.2.tgz#aa7c4dd92dabbcb80f313ebaaa8eb3dac05f13a7"
+  integrity sha512-5XWB9GbAUSHTn8VPU8/1DBXMuKYT5uOgEjJb8gN3mW0PNW5OPHpSdojoqf+iq1xo7vWzw/P8bAHY0n6ijpXF7g==
+  dependencies:
+    micromark-util-types "^1.0.0"
+
+micromark-extension-gfm-task-list-item@^1.0.0:
+  version "1.0.4"
+  resolved "https://registry.npmmirror.com/micromark-extension-gfm-task-list-item/-/micromark-extension-gfm-task-list-item-1.0.4.tgz#4b66d87847de40cef2b5ceddb9f9629a6dfe7472"
+  integrity sha512-9XlIUUVnYXHsFF2HZ9jby4h3npfX10S1coXTnV035QGPgrtNYQq3J6IfIvcCIUAJrrqBVi5BqA/LmaOMJqPwMQ==
+  dependencies:
+    micromark-factory-space "^1.0.0"
+    micromark-util-character "^1.0.0"
+    micromark-util-symbol "^1.0.0"
+    micromark-util-types "^1.0.0"
+    uvu "^0.5.0"
+
+micromark-extension-gfm@^2.0.0:
+  version "2.0.3"
+  resolved "https://registry.npmmirror.com/micromark-extension-gfm/-/micromark-extension-gfm-2.0.3.tgz#e517e8579949a5024a493e49204e884aa74f5acf"
+  integrity sha512-vb9OoHqrhCmbRidQv/2+Bc6pkP0FrtlhurxZofvOEy5o8RtuuvTq+RQ1Vw5ZDNrVraQZu3HixESqbG+0iKk/MQ==
+  dependencies:
+    micromark-extension-gfm-autolink-literal "^1.0.0"
+    micromark-extension-gfm-footnote "^1.0.0"
+    micromark-extension-gfm-strikethrough "^1.0.0"
+    micromark-extension-gfm-table "^1.0.0"
+    micromark-extension-gfm-tagfilter "^1.0.0"
+    micromark-extension-gfm-task-list-item "^1.0.0"
+    micromark-util-combine-extensions "^1.0.0"
+    micromark-util-types "^1.0.0"
+
+micromark-factory-destination@^1.0.0:
+  version "1.0.0"
+  resolved "https://registry.npmmirror.com/micromark-factory-destination/-/micromark-factory-destination-1.0.0.tgz#fef1cb59ad4997c496f887b6977aa3034a5a277e"
+  integrity sha512-eUBA7Rs1/xtTVun9TmV3gjfPz2wEwgK5R5xcbIM5ZYAtvGF6JkyaDsj0agx8urXnO31tEO6Ug83iVH3tdedLnw==
+  dependencies:
+    micromark-util-character "^1.0.0"
+    micromark-util-symbol "^1.0.0"
+    micromark-util-types "^1.0.0"
+
+micromark-factory-label@^1.0.0:
+  version "1.0.2"
+  resolved "https://registry.npmmirror.com/micromark-factory-label/-/micromark-factory-label-1.0.2.tgz#6be2551fa8d13542fcbbac478258fb7a20047137"
+  integrity sha512-CTIwxlOnU7dEshXDQ+dsr2n+yxpP0+fn271pu0bwDIS8uqfFcumXpj5mLn3hSC8iw2MUr6Gx8EcKng1dD7i6hg==
+  dependencies:
+    micromark-util-character "^1.0.0"
+    micromark-util-symbol "^1.0.0"
+    micromark-util-types "^1.0.0"
+    uvu "^0.5.0"
+
+micromark-factory-space@^1.0.0:
+  version "1.0.0"
+  resolved "https://registry.npmmirror.com/micromark-factory-space/-/micromark-factory-space-1.0.0.tgz#cebff49968f2b9616c0fcb239e96685cb9497633"
+  integrity sha512-qUmqs4kj9a5yBnk3JMLyjtWYN6Mzfcx8uJfi5XAveBniDevmZasdGBba5b4QsvRcAkmvGo5ACmSUmyGiKTLZew==
+  dependencies:
+    micromark-util-character "^1.0.0"
+    micromark-util-types "^1.0.0"
+
+micromark-factory-title@^1.0.0:
+  version "1.0.2"
+  resolved "https://registry.npmmirror.com/micromark-factory-title/-/micromark-factory-title-1.0.2.tgz#7e09287c3748ff1693930f176e1c4a328382494f"
+  integrity sha512-zily+Nr4yFqgMGRKLpTVsNl5L4PMu485fGFDOQJQBl2NFpjGte1e86zC0da93wf97jrc4+2G2GQudFMHn3IX+A==
+  dependencies:
+    micromark-factory-space "^1.0.0"
+    micromark-util-character "^1.0.0"
+    micromark-util-symbol "^1.0.0"
+    micromark-util-types "^1.0.0"
+    uvu "^0.5.0"
+
+micromark-factory-whitespace@^1.0.0:
+  version "1.0.0"
+  resolved "https://registry.npmmirror.com/micromark-factory-whitespace/-/micromark-factory-whitespace-1.0.0.tgz#e991e043ad376c1ba52f4e49858ce0794678621c"
+  integrity sha512-Qx7uEyahU1lt1RnsECBiuEbfr9INjQTGa6Err+gF3g0Tx4YEviPbqqGKNv/NrBaE7dVHdn1bVZKM/n5I/Bak7A==
+  dependencies:
+    micromark-factory-space "^1.0.0"
+    micromark-util-character "^1.0.0"
+    micromark-util-symbol "^1.0.0"
+    micromark-util-types "^1.0.0"
+
+micromark-util-character@^1.0.0:
+  version "1.1.0"
+  resolved "https://registry.npmmirror.com/micromark-util-character/-/micromark-util-character-1.1.0.tgz#d97c54d5742a0d9611a68ca0cd4124331f264d86"
+  integrity sha512-agJ5B3unGNJ9rJvADMJ5ZiYjBRyDpzKAOk01Kpi1TKhlT1APx3XZk6eN7RtSz1erbWHC2L8T3xLZ81wdtGRZzg==
+  dependencies:
+    micromark-util-symbol "^1.0.0"
+    micromark-util-types "^1.0.0"
+
+micromark-util-chunked@^1.0.0:
+  version "1.0.0"
+  resolved "https://registry.npmmirror.com/micromark-util-chunked/-/micromark-util-chunked-1.0.0.tgz#5b40d83f3d53b84c4c6bce30ed4257e9a4c79d06"
+  integrity sha512-5e8xTis5tEZKgesfbQMKRCyzvffRRUX+lK/y+DvsMFdabAicPkkZV6gO+FEWi9RfuKKoxxPwNL+dFF0SMImc1g==
+  dependencies:
+    micromark-util-symbol "^1.0.0"
+
+micromark-util-classify-character@^1.0.0:
+  version "1.0.0"
+  resolved "https://registry.npmmirror.com/micromark-util-classify-character/-/micromark-util-classify-character-1.0.0.tgz#cbd7b447cb79ee6997dd274a46fc4eb806460a20"
+  integrity sha512-F8oW2KKrQRb3vS5ud5HIqBVkCqQi224Nm55o5wYLzY/9PwHGXC01tr3d7+TqHHz6zrKQ72Okwtvm/xQm6OVNZA==
+  dependencies:
+    micromark-util-character "^1.0.0"
+    micromark-util-symbol "^1.0.0"
+    micromark-util-types "^1.0.0"
+
+micromark-util-combine-extensions@^1.0.0:
+  version "1.0.0"
+  resolved "https://registry.npmmirror.com/micromark-util-combine-extensions/-/micromark-util-combine-extensions-1.0.0.tgz#91418e1e74fb893e3628b8d496085639124ff3d5"
+  integrity sha512-J8H058vFBdo/6+AsjHp2NF7AJ02SZtWaVUjsayNFeAiydTxUwViQPxN0Hf8dp4FmCQi0UUFovFsEyRSUmFH3MA==
+  dependencies:
+    micromark-util-chunked "^1.0.0"
+    micromark-util-types "^1.0.0"
+
+micromark-util-decode-numeric-character-reference@^1.0.0:
+  version "1.0.0"
+  resolved "https://registry.npmmirror.com/micromark-util-decode-numeric-character-reference/-/micromark-util-decode-numeric-character-reference-1.0.0.tgz#dcc85f13b5bd93ff8d2868c3dba28039d490b946"
+  integrity sha512-OzO9AI5VUtrTD7KSdagf4MWgHMtET17Ua1fIpXTpuhclCqD8egFWo85GxSGvxgkGS74bEahvtM0WP0HjvV0e4w==
+  dependencies:
+    micromark-util-symbol "^1.0.0"
+
+micromark-util-decode-string@^1.0.0:
+  version "1.0.2"
+  resolved "https://registry.npmmirror.com/micromark-util-decode-string/-/micromark-util-decode-string-1.0.2.tgz#942252ab7a76dec2dbf089cc32505ee2bc3acf02"
+  integrity sha512-DLT5Ho02qr6QWVNYbRZ3RYOSSWWFuH3tJexd3dgN1odEuPNxCngTCXJum7+ViRAd9BbdxCvMToPOD/IvVhzG6Q==
+  dependencies:
+    decode-named-character-reference "^1.0.0"
+    micromark-util-character "^1.0.0"
+    micromark-util-decode-numeric-character-reference "^1.0.0"
+    micromark-util-symbol "^1.0.0"
+
+micromark-util-encode@^1.0.0:
+  version "1.0.1"
+  resolved "https://registry.npmmirror.com/micromark-util-encode/-/micromark-util-encode-1.0.1.tgz#2c1c22d3800870ad770ece5686ebca5920353383"
+  integrity sha512-U2s5YdnAYexjKDel31SVMPbfi+eF8y1U4pfiRW/Y8EFVCy/vgxk/2wWTxzcqE71LHtCuCzlBDRU2a5CQ5j+mQA==
+
+micromark-util-html-tag-name@^1.0.0:
+  version "1.1.0"
+  resolved "https://registry.npmmirror.com/micromark-util-html-tag-name/-/micromark-util-html-tag-name-1.1.0.tgz#eb227118befd51f48858e879b7a419fc0df20497"
+  integrity sha512-BKlClMmYROy9UiV03SwNmckkjn8QHVaWkqoAqzivabvdGcwNGMMMH/5szAnywmsTBUzDsU57/mFi0sp4BQO6dA==
+
+micromark-util-normalize-identifier@^1.0.0:
+  version "1.0.0"
+  resolved "https://registry.npmmirror.com/micromark-util-normalize-identifier/-/micromark-util-normalize-identifier-1.0.0.tgz#4a3539cb8db954bbec5203952bfe8cedadae7828"
+  integrity sha512-yg+zrL14bBTFrQ7n35CmByWUTFsgst5JhA4gJYoty4Dqzj4Z4Fr/DHekSS5aLfH9bdlfnSvKAWsAgJhIbogyBg==
+  dependencies:
+    micromark-util-symbol "^1.0.0"
+
+micromark-util-resolve-all@^1.0.0:
+  version "1.0.0"
+  resolved "https://registry.npmmirror.com/micromark-util-resolve-all/-/micromark-util-resolve-all-1.0.0.tgz#a7c363f49a0162e931960c44f3127ab58f031d88"
+  integrity sha512-CB/AGk98u50k42kvgaMM94wzBqozSzDDaonKU7P7jwQIuH2RU0TeBqGYJz2WY1UdihhjweivStrJ2JdkdEmcfw==
+  dependencies:
+    micromark-util-types "^1.0.0"
+
+micromark-util-sanitize-uri@^1.0.0, micromark-util-sanitize-uri@^1.1.0:
+  version "1.1.0"
+  resolved "https://registry.npmmirror.com/micromark-util-sanitize-uri/-/micromark-util-sanitize-uri-1.1.0.tgz#f12e07a85106b902645e0364feb07cf253a85aee"
+  integrity sha512-RoxtuSCX6sUNtxhbmsEFQfWzs8VN7cTctmBPvYivo98xb/kDEoTCtJQX5wyzIYEmk/lvNFTat4hL8oW0KndFpg==
+  dependencies:
+    micromark-util-character "^1.0.0"
+    micromark-util-encode "^1.0.0"
+    micromark-util-symbol "^1.0.0"
+
+micromark-util-subtokenize@^1.0.0:
+  version "1.0.2"
+  resolved "https://registry.npmmirror.com/micromark-util-subtokenize/-/micromark-util-subtokenize-1.0.2.tgz#ff6f1af6ac836f8bfdbf9b02f40431760ad89105"
+  integrity sha512-d90uqCnXp/cy4G881Ub4psE57Sf8YD0pim9QdjCRNjfas2M1u6Lbt+XZK9gnHL2XFhnozZiEdCa9CNfXSfQ6xA==
+  dependencies:
+    micromark-util-chunked "^1.0.0"
+    micromark-util-symbol "^1.0.0"
+    micromark-util-types "^1.0.0"
+    uvu "^0.5.0"
+
+micromark-util-symbol@^1.0.0:
+  version "1.0.1"
+  resolved "https://registry.npmmirror.com/micromark-util-symbol/-/micromark-util-symbol-1.0.1.tgz#b90344db62042ce454f351cf0bebcc0a6da4920e"
+  integrity sha512-oKDEMK2u5qqAptasDAwWDXq0tG9AssVwAx3E9bBF3t/shRIGsWIRG+cGafs2p/SnDSOecnt6hZPCE2o6lHfFmQ==
+
+micromark-util-types@^1.0.0, micromark-util-types@^1.0.1:
+  version "1.0.2"
+  resolved "https://registry.npmmirror.com/micromark-util-types/-/micromark-util-types-1.0.2.tgz#f4220fdb319205812f99c40f8c87a9be83eded20"
+  integrity sha512-DCfg/T8fcrhrRKTPjRrw/5LLvdGV7BHySf/1LOZx7TzWZdYRjogNtyNq885z3nNallwr3QUKARjqvHqX1/7t+w==
+
+micromark@^3.0.0:
+  version "3.1.0"
+  resolved "https://registry.npmmirror.com/micromark/-/micromark-3.1.0.tgz#eeba0fe0ac1c9aaef675157b52c166f125e89f62"
+  integrity sha512-6Mj0yHLdUZjHnOPgr5xfWIMqMWS12zDN6iws9SLuSz76W8jTtAv24MN4/CL7gJrl5vtxGInkkqDv/JIoRsQOvA==
+  dependencies:
+    "@types/debug" "^4.0.0"
+    debug "^4.0.0"
+    decode-named-character-reference "^1.0.0"
+    micromark-core-commonmark "^1.0.1"
+    micromark-factory-space "^1.0.0"
+    micromark-util-character "^1.0.0"
+    micromark-util-chunked "^1.0.0"
+    micromark-util-combine-extensions "^1.0.0"
+    micromark-util-decode-numeric-character-reference "^1.0.0"
+    micromark-util-encode "^1.0.0"
+    micromark-util-normalize-identifier "^1.0.0"
+    micromark-util-resolve-all "^1.0.0"
+    micromark-util-sanitize-uri "^1.0.0"
+    micromark-util-subtokenize "^1.0.0"
+    micromark-util-symbol "^1.0.0"
+    micromark-util-types "^1.0.1"
+    uvu "^0.5.0"
+
 micromatch@^4.0.4:
   version "4.0.5"
   resolved "https://registry.npmmirror.com/micromatch/-/micromatch-4.0.5.tgz#bc8999a7cbbf77cdc89f132f6e467051b49090c6"
   integrity sha512-DMy+ERcEW2q8Z2Po+WNXuw3c5YaUSFjAO5GsJqfEl7UjvtIuFKO6ZrKvcItdy98dwFI2N1tg3zNIdKaQT+aNdA==
   dependencies:
     braces "^3.0.2"
     picomatch "^2.3.1"
@@ -3579,14 +4264,19 @@
   integrity sha512-NkJREyFTSUXR772Qaai51BnE1voWx56LOL80xG7qkZr6vo8vEaLF3sz1JNUVh+rxmUzxYaqOhfuxTfqUh0FXUg==
 
 mobx@6.6.1:
   version "6.6.1"
   resolved "https://registry.npmmirror.com/mobx/-/mobx-6.6.1.tgz#70ee6aa82f25aeb7e7d522bd621207434e509318"
   integrity sha512-7su3UZv5JF+ohLr2opabjbUAERfXstMY+wiBtey8yNAPoB8H187RaQXuhFjNkH8aE4iHbDWnhDFZw0+5ic4nGQ==
 
+mri@^1.1.0:
+  version "1.2.0"
+  resolved "https://registry.npmmirror.com/mri/-/mri-1.2.0.tgz#6721480fec2a11a4889861115a48b6cbe7cc8f0b"
+  integrity sha512-tzzskb3bG8LvYGFF/mDTpq3jpI6Q9wc3LEmBaghu+DdCssd1FakN7Bc0hVNmEyGq1bq3RgfkCb3cmQLpNPOroA==
+
 ms@2.1.2:
   version "2.1.2"
   resolved "https://registry.npmmirror.com/ms/-/ms-2.1.2.tgz#d09d1f357b443f493382a8eb3ccd183872ae6009"
   integrity sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==
 
 ms@^2.1.1:
   version "2.1.3"
@@ -3794,14 +4484,26 @@
 parent-module@^1.0.0:
   version "1.0.1"
   resolved "https://registry.npmmirror.com/parent-module/-/parent-module-1.0.1.tgz#691d2709e78c79fae3a156622452d00762caaaa2"
   integrity sha512-GQ2EWRpQV8/o+Aw8YqtfZZPfNRWZYkbidE9k5rpl/hC3vtHHBfGm2Ifi6qWV+coDGkrUKZAxE3Lot5kcsRlh+g==
   dependencies:
     callsites "^3.0.0"
 
+parse-entities@^2.0.0:
+  version "2.0.0"
+  resolved "https://registry.npmmirror.com/parse-entities/-/parse-entities-2.0.0.tgz#53c6eb5b9314a1f4ec99fa0fdf7ce01ecda0cbe8"
+  integrity sha512-kkywGpCcRYhqQIchaWqZ875wzpS/bMKhz5HnN3p7wveJTkTtyAB/AlnS0f8DFSqYW1T82t6yEAkEcB+A1I3MbQ==
+  dependencies:
+    character-entities "^1.0.0"
+    character-entities-legacy "^1.0.0"
+    character-reference-invalid "^1.0.0"
+    is-alphanumerical "^1.0.0"
+    is-decimal "^1.0.0"
+    is-hexadecimal "^1.0.0"
+
 parse-json@^5.0.0:
   version "5.2.0"
   resolved "https://registry.npmmirror.com/parse-json/-/parse-json-5.2.0.tgz#c76fc66dee54231c962b22bcc8a72cf2f99753cd"
   integrity sha512-ayCKvm/phCGxOkYRSCM82iDwct8/EonSEgCSxWxD7ve6jHggsFl4fZVQBPRNgQoKiuV/odhFrGzQXZwbifC8Rg==
   dependencies:
     "@babel/code-frame" "^7.0.0"
     error-ex "^1.3.1"
@@ -3872,28 +4574,50 @@
     source-map-js "^1.0.2"
 
 prelude-ls@^1.2.1:
   version "1.2.1"
   resolved "https://registry.npmmirror.com/prelude-ls/-/prelude-ls-1.2.1.tgz#debc6489d7a6e6b0e7611888cec880337d316396"
   integrity sha512-vkcDPrRZo1QZLbn5RLGPpg/WmIQ65qoWWhcGKf/b5eplkkarX0m9z8ppCat4mlOqUsWpyNuYgO3VRyrYHSzX5g==
 
+prismjs@^1.27.0:
+  version "1.29.0"
+  resolved "https://registry.npmmirror.com/prismjs/-/prismjs-1.29.0.tgz#f113555a8fa9b57c35e637bba27509dcf802dd12"
+  integrity sha512-Kx/1w86q/epKcmte75LNrEoT+lX8pBpavuAbvJWRXar7Hz8jrtF+e3vY751p0R8H9HdArwaCTNDDzHg/ScJK1Q==
+
+prismjs@~1.27.0:
+  version "1.27.0"
+  resolved "https://registry.npmmirror.com/prismjs/-/prismjs-1.27.0.tgz#bb6ee3138a0b438a3653dd4d6ce0cc6510a45057"
+  integrity sha512-t13BGPUlFDR7wRB5kQDG4jjl7XeuH6jbJGt11JHPL96qwsEHNX2+68tFXqc1/k+/jALsbSWJKUOT/hcYAZ5LkA==
+
 process-nextick-args@~2.0.0:
   version "2.0.1"
   resolved "https://registry.npmmirror.com/process-nextick-args/-/process-nextick-args-2.0.1.tgz#7820d9b16120cc55ca9ae7792680ae7dba6d7fe2"
   integrity sha512-3ouUOpQhtgrbOa17J7+uxOTpITYWaGP7/AhoR3+A+/1e9skrzelGi/dXzEYyvbxubEF6Wn2ypscTKiKJFFn1ag==
 
-prop-types@^15.6.2, prop-types@^15.8.1:
+prop-types@^15.0.0, prop-types@^15.5.10, prop-types@^15.6.0, prop-types@^15.6.2, prop-types@^15.8.1:
   version "15.8.1"
   resolved "https://registry.npmmirror.com/prop-types/-/prop-types-15.8.1.tgz#67d87bf1a694f48435cf332c24af10214a3140b5"
   integrity sha512-oj87CgZICdulUohogVAR7AjlC0327U4el4L6eAvOqCeudMDVU0NThNaV+b9Df4dXgSP1gXMTnPdhfe/2qDH5cg==
   dependencies:
     loose-envify "^1.4.0"
     object-assign "^4.1.1"
     react-is "^16.13.1"
 
+property-information@^5.0.0:
+  version "5.6.0"
+  resolved "https://registry.npmmirror.com/property-information/-/property-information-5.6.0.tgz#61675545fb23002f245c6540ec46077d4da3ed69"
+  integrity sha512-YUHSPk+A30YPv+0Qf8i9Mbfe/C0hdPXk1s1jPVToV8pk8BQtpw10ct89Eo7OWkutrwqvT0eicAxlOg3dOAu8JA==
+  dependencies:
+    xtend "^4.0.0"
+
+property-information@^6.0.0:
+  version "6.2.0"
+  resolved "https://registry.npmmirror.com/property-information/-/property-information-6.2.0.tgz#b74f522c31c097b5149e3c3cb8d7f3defd986a1d"
+  integrity sha512-kma4U7AFCTwpqq5twzC1YVIDXSqg6qQK6JN0smOw8fgRy1OkMi0CYSzFmsy6dnqSenamAtj0CyXMUJ1Mf6oROg==
+
 proxy-from-env@^1.1.0:
   version "1.1.0"
   resolved "https://registry.npmmirror.com/proxy-from-env/-/proxy-from-env-1.1.0.tgz#e102f16ca355424865755d2c9e8ea4f24d58c3e2"
   integrity sha512-D+zkORCbA9f1tdWRK0RaCR3GPv50cMxcrz4X8k5LTSUD1Dkw47mKJEZQNunItRTkWwgtaUSo1RVFRIG9ZXiFYg==
 
 punycode@^2.1.0:
   version "2.3.0"
@@ -3925,14 +4649,27 @@
 react-clientside-effect@^1.2.6:
   version "1.2.6"
   resolved "https://registry.npmmirror.com/react-clientside-effect/-/react-clientside-effect-1.2.6.tgz#29f9b14e944a376b03fb650eed2a754dd128ea3a"
   integrity sha512-XGGGRQAKY+q25Lz9a/4EPqom7WRjz3z9R2k4jhVKA/puQFH/5Nt27vFZYql4m4NVNdUvX8PS3O7r/Zzm7cjUlg==
   dependencies:
     "@babel/runtime" "^7.12.13"
 
+react-color@^2.19.3:
+  version "2.19.3"
+  resolved "https://registry.npmmirror.com/react-color/-/react-color-2.19.3.tgz#ec6c6b4568312a3c6a18420ab0472e146aa5683d"
+  integrity sha512-LEeGE/ZzNLIsFWa1TMe8y5VYqr7bibneWmvJwm1pCn/eNmrabWDh659JSPn9BuaMpEfU83WTOJfnCcjDZwNQTA==
+  dependencies:
+    "@icons/material" "^0.2.4"
+    lodash "^4.17.15"
+    lodash-es "^4.17.15"
+    material-colors "^1.2.1"
+    prop-types "^15.5.10"
+    reactcss "^1.2.0"
+    tinycolor2 "^1.4.1"
+
 react-dom@18.2.0:
   version "18.2.0"
   resolved "https://registry.npmmirror.com/react-dom/-/react-dom-18.2.0.tgz#22aaf38708db2674ed9ada224ca4aa708d821e3d"
   integrity sha512-6IMTriUmvsjHUjNtEDudZfuDQUoWXVxKHhlEGSk81n4YFS+r/Kl99wXiwlVXtPBtJenozv2P+hxDsw9eA7Xo6g==
   dependencies:
     loose-envify "^1.1.0"
     scheduler "^0.23.0"
@@ -3955,14 +4692,40 @@
     use-sidecar "^1.1.2"
 
 react-is@^16.12.0, react-is@^16.13.1, react-is@^16.7.0:
   version "16.13.1"
   resolved "https://registry.npmmirror.com/react-is/-/react-is-16.13.1.tgz#789729a4dc36de2999dc156dd6c1d9c18cea56a4"
   integrity sha512-24e6ynE2H+OKt4kqsOvNd8kBpV65zoxbA4BVsEOB3ARVWQki/DHzaUoC5KuON/BiccDaCCTZBuOcfZs70kR8bQ==
 
+react-is@^18.0.0:
+  version "18.2.0"
+  resolved "https://registry.npmmirror.com/react-is/-/react-is-18.2.0.tgz#199431eeaaa2e09f86427efbb4f1473edb47609b"
+  integrity sha512-xWGDIW6x921xtzPkhiULtthJHoJvBbF3q26fzloPCK0hsvxtPVelvftw3zjbHWSkR2km9Z+4uxbDDK/6Zw9B8w==
+
+react-markdown@^8.0.7:
+  version "8.0.7"
+  resolved "https://registry.npmmirror.com/react-markdown/-/react-markdown-8.0.7.tgz#c8dbd1b9ba5f1c5e7e5f2a44de465a3caafdf89b"
+  integrity sha512-bvWbzG4MtOU62XqBx3Xx+zB2raaFFsq4mYiAzfjXJMEz2sixgeAfraA3tvzULF02ZdOMUOKTBFFaZJDDrq+BJQ==
+  dependencies:
+    "@types/hast" "^2.0.0"
+    "@types/prop-types" "^15.0.0"
+    "@types/unist" "^2.0.0"
+    comma-separated-tokens "^2.0.0"
+    hast-util-whitespace "^2.0.0"
+    prop-types "^15.0.0"
+    property-information "^6.0.0"
+    react-is "^18.0.0"
+    remark-parse "^10.0.0"
+    remark-rehype "^10.0.0"
+    space-separated-tokens "^2.0.0"
+    style-to-object "^0.4.0"
+    unified "^10.0.0"
+    unist-util-visit "^4.0.0"
+    vfile "^5.0.0"
+
 react-refresh@^0.14.0:
   version "0.14.0"
   resolved "https://registry.npmmirror.com/react-refresh/-/react-refresh-0.14.0.tgz#4e02825378a5f227079554d4284889354e5f553e"
   integrity sha512-wViHqhAd8OHeLS/IRMJjTSDHF3U9eWi62F/MledQGPdJGDhodXJ9PBLNGr6WWL7qlH12Mt3TyTpbS+hGXMjCzQ==
 
 react-remove-scroll-bar@^2.3.4:
   version "2.3.4"
@@ -3979,30 +4742,88 @@
   dependencies:
     react-remove-scroll-bar "^2.3.4"
     react-style-singleton "^2.2.1"
     tslib "^2.1.0"
     use-callback-ref "^1.3.0"
     use-sidecar "^1.1.2"
 
+react-select@5.7.0:
+  version "5.7.0"
+  resolved "https://registry.npmmirror.com/react-select/-/react-select-5.7.0.tgz#82921b38f1fcf1471a0b62304da01f2896cd8ce6"
+  integrity sha512-lJGiMxCa3cqnUr2Jjtg9YHsaytiZqeNOKeibv6WF5zbK/fPegZ1hg3y/9P1RZVLhqBTs0PfqQLKuAACednYGhQ==
+  dependencies:
+    "@babel/runtime" "^7.12.0"
+    "@emotion/cache" "^11.4.0"
+    "@emotion/react" "^11.8.1"
+    "@floating-ui/dom" "^1.0.1"
+    "@types/react-transition-group" "^4.4.0"
+    memoize-one "^6.0.0"
+    prop-types "^15.6.0"
+    react-transition-group "^4.3.0"
+    use-isomorphic-layout-effect "^1.1.2"
+
+react-select@^5.7.3:
+  version "5.7.3"
+  resolved "https://registry.npmmirror.com/react-select/-/react-select-5.7.3.tgz#fa0dc9a23cad6ff3871ad3829f6083a4b54961a2"
+  integrity sha512-z8i3NCuFFWL3w27xq92rBkVI2onT0jzIIPe480HlBjXJ3b5o6Q+Clp4ydyeKrj9DZZ3lrjawwLC5NGl0FSvUDg==
+  dependencies:
+    "@babel/runtime" "^7.12.0"
+    "@emotion/cache" "^11.4.0"
+    "@emotion/react" "^11.8.1"
+    "@floating-ui/dom" "^1.0.1"
+    "@types/react-transition-group" "^4.4.0"
+    memoize-one "^6.0.0"
+    prop-types "^15.6.0"
+    react-transition-group "^4.3.0"
+    use-isomorphic-layout-effect "^1.1.2"
+
 react-style-singleton@^2.2.1:
   version "2.2.1"
   resolved "https://registry.npmmirror.com/react-style-singleton/-/react-style-singleton-2.2.1.tgz#f99e420492b2d8f34d38308ff660b60d0b1205b4"
   integrity sha512-ZWj0fHEMyWkHzKYUr2Bs/4zU6XLmq9HsgBURm7g5pAVfyn49DgUiNgY2d4lXRlYSiCif9YBGpQleewkcqddc7g==
   dependencies:
     get-nonce "^1.0.0"
     invariant "^2.2.4"
     tslib "^2.0.0"
 
+react-syntax-highlighter@^15.5.0:
+  version "15.5.0"
+  resolved "https://registry.npmmirror.com/react-syntax-highlighter/-/react-syntax-highlighter-15.5.0.tgz#4b3eccc2325fa2ec8eff1e2d6c18fa4a9e07ab20"
+  integrity sha512-+zq2myprEnQmH5yw6Gqc8lD55QHnpKaU8TOcFeC/Lg/MQSs8UknEA0JC4nTZGFAXC2J2Hyj/ijJ7NlabyPi2gg==
+  dependencies:
+    "@babel/runtime" "^7.3.1"
+    highlight.js "^10.4.1"
+    lowlight "^1.17.0"
+    prismjs "^1.27.0"
+    refractor "^3.6.0"
+
+react-transition-group@^4.3.0:
+  version "4.4.5"
+  resolved "https://registry.npmmirror.com/react-transition-group/-/react-transition-group-4.4.5.tgz#e53d4e3f3344da8521489fbef8f2581d42becdd1"
+  integrity sha512-pZcd1MCJoiKiBR2NRxeCRg13uCXbydPnmB4EOeRrY7480qNWO8IIgQG6zlDkm6uRMsURXPuKq0GWtiM59a5Q6g==
+  dependencies:
+    "@babel/runtime" "^7.5.5"
+    dom-helpers "^5.0.1"
+    loose-envify "^1.4.0"
+    prop-types "^15.6.2"
+
 react@18.2.0:
   version "18.2.0"
   resolved "https://registry.npmmirror.com/react/-/react-18.2.0.tgz#555bd98592883255fa00de14f1151a917b5d77d5"
   integrity sha512-/3IjMdb2L9QbBdWiW5e3P2/npwMBaU9mHCSCUzNln0ZCYbcfTsGbTJrU/kGemdH2IWmB2ioZ+zkxtmq6g09fGQ==
   dependencies:
     loose-envify "^1.1.0"
 
+reactcss@^1.2.0:
+  version "1.2.3"
+  resolved "https://registry.npmmirror.com/reactcss/-/reactcss-1.2.3.tgz#c00013875e557b1cf0dfd9a368a1c3dab3b548dd"
+  integrity sha512-KiwVUcFu1RErkI97ywr8nvx8dNOpT03rbnma0SSalTYjkrPYaEajR4a/MRt6DZ46K6arDRbWMNHF+xH7G7n/8A==
+  dependencies:
+    lodash "^4.0.1"
+
 readable-stream@~2.3.6:
   version "2.3.8"
   resolved "https://registry.npmmirror.com/readable-stream/-/readable-stream-2.3.8.tgz#91125e8042bba1b9887f49345f6277027ce8be9b"
   integrity sha512-8p0AUk4XODgIewSi0l8Epjs+EVnWiK7NoDIEGU0HhE7+ZyY8D1IMY7odu5lRrFXGg71L15KG8QrPmum45RTtdA==
   dependencies:
     core-util-is "~1.0.0"
     inherits "~2.0.3"
@@ -4015,28 +4836,66 @@
 readdirp@~3.6.0:
   version "3.6.0"
   resolved "https://registry.npmmirror.com/readdirp/-/readdirp-3.6.0.tgz#74a370bd857116e245b29cc97340cd431a02a6c7"
   integrity sha512-hOS089on8RduqdbhvQ5Z37A0ESjsqz6qnRcffsMU3495FuTdqSm+7bhJ29JvIOsBDEEnan5DPu9t3To9VRlMzA==
   dependencies:
     picomatch "^2.2.1"
 
+refractor@^3.6.0:
+  version "3.6.0"
+  resolved "https://registry.npmmirror.com/refractor/-/refractor-3.6.0.tgz#ac318f5a0715ead790fcfb0c71f4dd83d977935a"
+  integrity sha512-MY9W41IOWxxk31o+YvFCNyNzdkc9M20NoZK5vq6jkv4I/uh2zkWcfudj0Q1fovjUQJrNewS9NMzeTtqPf+n5EA==
+  dependencies:
+    hastscript "^6.0.0"
+    parse-entities "^2.0.0"
+    prismjs "~1.27.0"
+
 regenerator-runtime@^0.13.11:
   version "0.13.11"
   resolved "https://registry.npmmirror.com/regenerator-runtime/-/regenerator-runtime-0.13.11.tgz#f6dca3e7ceec20590d07ada785636a90cdca17f9"
   integrity sha512-kY1AZVr2Ra+t+piVaJ4gxaFaReZVH40AKNo7UCX6W+dEwBo/2oZJzqfuN1qLq1oL45o56cPaTXELwrTh8Fpggg==
 
 regexp.prototype.flags@^1.4.3, regexp.prototype.flags@^1.5.0:
   version "1.5.0"
   resolved "https://registry.npmmirror.com/regexp.prototype.flags/-/regexp.prototype.flags-1.5.0.tgz#fe7ce25e7e4cca8db37b6634c8a2c7009199b9cb"
   integrity sha512-0SutC3pNudRKgquxGoRGIz946MZVHqbNfPjBdxeOhBrdgDKlRoXmYLQN9xRbrR09ZXWeGAdPuif7egofn6v5LA==
   dependencies:
     call-bind "^1.0.2"
     define-properties "^1.2.0"
     functions-have-names "^1.2.3"
 
+remark-gfm@^3.0.1:
+  version "3.0.1"
+  resolved "https://registry.npmmirror.com/remark-gfm/-/remark-gfm-3.0.1.tgz#0b180f095e3036545e9dddac0e8df3fa5cfee54f"
+  integrity sha512-lEFDoi2PICJyNrACFOfDD3JlLkuSbOa5Wd8EPt06HUdptv8Gn0bxYTdbU/XXQ3swAPkEaGxxPN9cbnMHvVu1Ig==
+  dependencies:
+    "@types/mdast" "^3.0.0"
+    mdast-util-gfm "^2.0.0"
+    micromark-extension-gfm "^2.0.0"
+    unified "^10.0.0"
+
+remark-parse@^10.0.0:
+  version "10.0.2"
+  resolved "https://registry.npmmirror.com/remark-parse/-/remark-parse-10.0.2.tgz#ca241fde8751c2158933f031a4e3efbaeb8bc262"
+  integrity sha512-3ydxgHa/ZQzG8LvC7jTXccARYDcRld3VfcgIIFs7bI6vbRSxJJmzgLEIIoYKyrfhaY+ujuWaf/PJiMZXoiCXgw==
+  dependencies:
+    "@types/mdast" "^3.0.0"
+    mdast-util-from-markdown "^1.0.0"
+    unified "^10.0.0"
+
+remark-rehype@^10.0.0:
+  version "10.1.0"
+  resolved "https://registry.npmmirror.com/remark-rehype/-/remark-rehype-10.1.0.tgz#32dc99d2034c27ecaf2e0150d22a6dcccd9a6279"
+  integrity sha512-EFmR5zppdBp0WQeDVZ/b66CWJipB2q2VLNFMabzDSGR66Z2fQii83G5gTBbgGEnEEA0QRussvrFHxk1HWGJskw==
+  dependencies:
+    "@types/hast" "^2.0.0"
+    "@types/mdast" "^3.0.0"
+    mdast-util-to-hast "^12.1.0"
+    unified "^10.0.0"
+
 require-directory@^2.1.1:
   version "2.1.1"
   resolved "https://registry.npmmirror.com/require-directory/-/require-directory-2.1.1.tgz#8c64ad5fd30dab1c976e2344ffe7f792a6a6df42"
   integrity sha512-fGxEI7+wsG9xrvdjsrlmL22OMTTiHRwAMroiEeMgq8gzoLC/PQr7RsRDSTLUg/bZAZtF+TVIkHc6/4RIKrui+Q==
 
 resize-observer-polyfill@^1.5.1:
   version "1.5.1"
@@ -4105,14 +4964,21 @@
 run-parallel@^1.1.9:
   version "1.2.0"
   resolved "https://registry.npmmirror.com/run-parallel/-/run-parallel-1.2.0.tgz#66d1368da7bdf921eb9d95bd1a9229e7f21a43ee"
   integrity sha512-5l4VyZR86LZ/lDxZTR6jqL8AFE2S0IFLMP26AbjsLVADxHdhB/c0GUsH+y39UfCi3dzz8OlQuPmnaJOMoDHQBA==
   dependencies:
     queue-microtask "^1.2.2"
 
+sade@^1.7.3:
+  version "1.8.1"
+  resolved "https://registry.npmmirror.com/sade/-/sade-1.8.1.tgz#0a78e81d658d394887be57d2a409bf703a3b2701"
+  integrity sha512-xal3CZX1Xlo/k4ApwCFrHVACi9fBqJ7V+mwhBsuf/1IOKbBy098Fex+Wa/5QMubw09pSZ/u8EY8PWgevJsXp1A==
+  dependencies:
+    mri "^1.1.0"
+
 safe-buffer@~5.1.0, safe-buffer@~5.1.1:
   version "5.1.2"
   resolved "https://registry.npmmirror.com/safe-buffer/-/safe-buffer-5.1.2.tgz#991ec69d296e0313747d59bdfd2b745c35f8828d"
   integrity sha512-Gd2UZBJDkXlY7GbJxfsE8/nvKkUEU1G38c1siN6QP6a9PT9MmHB8GnpscSmMJSoF8LOIrt8ud/wPtojys4G6+g==
 
 safe-regex-test@^1.0.0:
   version "1.0.0"
@@ -4208,14 +5074,24 @@
   integrity sha512-LbrmJOMUSdEVxIKvdcJzQC+nQhe8FUZQTXQy6+I75skNgn3OoQ0DZA8YnFa7gp8tqtL3KPf1kmo0R5DoApeSGQ==
 
 source-map@^0.7.4:
   version "0.7.4"
   resolved "https://registry.npmmirror.com/source-map/-/source-map-0.7.4.tgz#a9bbe705c9d8846f4e08ff6765acf0f1b0898656"
   integrity sha512-l3BikUxvPOcn5E74dZiq5BGsTb5yEwhaTSzccU6t4sDOH8NWJCstKO5QT2CvtFoK6F0saL7p9xHAqHOlCPJygA==
 
+space-separated-tokens@^1.0.0:
+  version "1.1.5"
+  resolved "https://registry.npmmirror.com/space-separated-tokens/-/space-separated-tokens-1.1.5.tgz#85f32c3d10d9682007e917414ddc5c26d1aa6899"
+  integrity sha512-q/JSVd1Lptzhf5bkYm4ob4iWPjx0KiRe3sRFBNrVqbJkFaBm5vbbowy1mymoPNLRa52+oadOhJ+K49wsSeSjTA==
+
+space-separated-tokens@^2.0.0:
+  version "2.0.2"
+  resolved "https://registry.npmmirror.com/space-separated-tokens/-/space-separated-tokens-2.0.2.tgz#1ecd9d2350a3844572c3f4a312bceb018348859f"
+  integrity sha512-PEGlAwrG8yXGXRjW32fGbg66JAlOAwbObuqVoJpv/mRgoWDQfgH1wDPvtzWyUSNAXBGSk8h755YDbbcEy3SH2Q==
+
 stop-iteration-iterator@^1.0.0:
   version "1.0.0"
   resolved "https://registry.npmmirror.com/stop-iteration-iterator/-/stop-iteration-iterator-1.0.0.tgz#6a60be0b4ee757d1ed5254858ec66b10c49285e4"
   integrity sha512-iCGQj+0l0HOdZ2AEeBADlsRC+vsnDsZsbdSiH1yNSjcfKM7fdpCMfqAL/dwF5BLiw/XhRft/Wax6zQbhq2BcjQ==
   dependencies:
     internal-slot "^1.0.4"
 
@@ -4299,14 +5175,21 @@
   integrity sha512-dOESqjYr96iWYylGObzd39EuNTa5VJxyvVAEm5Jnh7KGo75V43Hk1odPQkNDyXNmUR6k+gEiDVXnjB8HJ3crXw==
 
 strip-json-comments@^3.1.0, strip-json-comments@^3.1.1:
   version "3.1.1"
   resolved "https://registry.npmmirror.com/strip-json-comments/-/strip-json-comments-3.1.1.tgz#31f1281b3832630434831c310c01cccda8cbe006"
   integrity sha512-6fPc+R4ihwqP6N/aIv2f1gMH8lOVtWQHoqC4yK6oSDVVocumAsfCqjkXnqiYMhmMwS/mEHLp7Vehlt3ql6lEig==
 
+style-to-object@^0.4.0:
+  version "0.4.1"
+  resolved "https://registry.npmmirror.com/style-to-object/-/style-to-object-0.4.1.tgz#53cf856f7cf7f172d72939d9679556469ba5de37"
+  integrity sha512-HFpbb5gr2ypci7Qw+IOhnP2zOU7e77b+rzM+wTzXzfi1PrtBCX0E7Pk4wL4iTLnhzZ+JgEGAhX81ebTg/aYjQw==
+  dependencies:
+    inline-style-parser "0.1.1"
+
 styled-jsx@5.1.1:
   version "5.1.1"
   resolved "https://registry.npmmirror.com/styled-jsx/-/styled-jsx-5.1.1.tgz#839a1c3aaacc4e735fed0781b8619ea5d0009d1f"
   integrity sha512-pW7uC1l4mBZ8ugbiZrcIsiIvVx1UmTfw7UkC3Um2tmfUq9Bhk8IiyEIPl6F8agHgjzku6j0xQEZbfA5uSgSaCw==
   dependencies:
     client-only "0.0.1"
 
@@ -4358,14 +5241,19 @@
   integrity sha512-N+8UisAXDGk8PFXP4HAzVR9nbfmVJ3zYLAWiTIoqC5v5isinhr+r5uaO8+7r3BMfuNIufIsA7RdpVgacC2cSpw==
 
 tiny-invariant@^1.0.6:
   version "1.3.1"
   resolved "https://registry.npmmirror.com/tiny-invariant/-/tiny-invariant-1.3.1.tgz#8560808c916ef02ecfd55e66090df23a4b7aa642"
   integrity sha512-AD5ih2NlSssTCwsMznbvwMZpJ1cbhkGd2uueNxzv2jDlEeZdU04JQfRnggJQ8DrcVBGjAsCKwFBbDlVNtEMlzw==
 
+tinycolor2@^1.4.1:
+  version "1.6.0"
+  resolved "https://registry.npmmirror.com/tinycolor2/-/tinycolor2-1.6.0.tgz#f98007460169b0263b97072c5ae92484ce02d09e"
+  integrity sha512-XPaBkWQJdsf3pLKJV9p4qN/S+fm2Oj8AIPo1BTUhg5oxkvm9+SVEGFdhyOz7tTdUTfvxMiAs4sp6/eZO2Ew+pw==
+
 titleize@^3.0.0:
   version "3.0.0"
   resolved "https://registry.npmmirror.com/titleize/-/titleize-3.0.0.tgz#71c12eb7fdd2558aa8a44b0be83b8a76694acd53"
   integrity sha512-KxVu8EYHDPBdUYdKZdKtU2aj2XfEx9AfjXxE/Aj0vT06w2icA09Vus1rh6eSu1y01akYg6BjIK/hxyLJINoMLQ==
 
 to-fast-properties@^2.0.0:
   version "2.0.0"
@@ -4380,14 +5268,24 @@
     is-number "^7.0.0"
 
 toggle-selection@^1.0.6:
   version "1.0.6"
   resolved "https://registry.npmmirror.com/toggle-selection/-/toggle-selection-1.0.6.tgz#6e45b1263f2017fa0acc7d89d78b15b8bf77da32"
   integrity sha512-BiZS+C1OS8g/q2RRbJmy59xpyghNBqrr6k5L/uKBGRsTfxmu3ffiRnd8mlGPUVayg8pvfi5urfnu8TU7DVOkLQ==
 
+trim-lines@^3.0.0:
+  version "3.0.1"
+  resolved "https://registry.npmmirror.com/trim-lines/-/trim-lines-3.0.1.tgz#d802e332a07df861c48802c04321017b1bd87338"
+  integrity sha512-kRj8B+YHZCc9kQYdWfJB2/oUl9rA99qbowYYBtr4ui4mZyAQ2JpvVBd/6U2YloATfqBhBTSMhTpgBHtU0Mf3Rg==
+
+trough@^2.0.0:
+  version "2.1.0"
+  resolved "https://registry.npmmirror.com/trough/-/trough-2.1.0.tgz#0f7b511a4fde65a46f18477ab38849b22c554876"
+  integrity sha512-AqTiAOLcj85xS7vQ8QkAV41hPDIJ71XJB4RCUrzo/1GM2CQwhkJGaf9Hgr7BOugMRpgGUrqRg/DrBDl4H40+8g==
+
 tsconfck@^2.1.0:
   version "2.1.1"
   resolved "https://registry.npmmirror.com/tsconfck/-/tsconfck-2.1.1.tgz#9b51603d2712d1f4740fa14748ca886a2e1893e5"
   integrity sha512-ZPCkJBKASZBmBUNqGHmRhdhM8pJYDdOXp4nRgj/O0JwUwsMq50lCDRQP/M5GBNAA0elPrq4gAeu4dkaVCuKWww==
 
 tsconfig-paths@^3.14.1:
   version "3.14.2"
@@ -4453,14 +5351,70 @@
   integrity sha512-61pPlCD9h51VoreyJ0BReideM3MDKMKnh6+V9L08331ipq6Q8OFXZYiqP6n/tbHx4s5I9uRhcye6BrbkizkBDw==
   dependencies:
     call-bind "^1.0.2"
     has-bigints "^1.0.2"
     has-symbols "^1.0.3"
     which-boxed-primitive "^1.0.2"
 
+unified@^10.0.0:
+  version "10.1.2"
+  resolved "https://registry.npmmirror.com/unified/-/unified-10.1.2.tgz#b1d64e55dafe1f0b98bb6c719881103ecf6c86df"
+  integrity sha512-pUSWAi/RAnVy1Pif2kAoeWNBa3JVrx0MId2LASj8G+7AiHWoKZNTomq6LG326T68U7/e263X6fTdcXIy7XnF7Q==
+  dependencies:
+    "@types/unist" "^2.0.0"
+    bail "^2.0.0"
+    extend "^3.0.0"
+    is-buffer "^2.0.0"
+    is-plain-obj "^4.0.0"
+    trough "^2.0.0"
+    vfile "^5.0.0"
+
+unist-util-generated@^2.0.0:
+  version "2.0.1"
+  resolved "https://registry.npmmirror.com/unist-util-generated/-/unist-util-generated-2.0.1.tgz#e37c50af35d3ed185ac6ceacb6ca0afb28a85cae"
+  integrity sha512-qF72kLmPxAw0oN2fwpWIqbXAVyEqUzDHMsbtPvOudIlUzXYFIeQIuxXQCRCFh22B7cixvU0MG7m3MW8FTq/S+A==
+
+unist-util-is@^5.0.0:
+  version "5.2.1"
+  resolved "https://registry.npmmirror.com/unist-util-is/-/unist-util-is-5.2.1.tgz#b74960e145c18dcb6226bc57933597f5486deae9"
+  integrity sha512-u9njyyfEh43npf1M+yGKDGVPbY/JWEemg5nH05ncKPfi+kBbKBJoTdsogMu33uhytuLlv9y0O7GH7fEdwLdLQw==
+  dependencies:
+    "@types/unist" "^2.0.0"
+
+unist-util-position@^4.0.0:
+  version "4.0.4"
+  resolved "https://registry.npmmirror.com/unist-util-position/-/unist-util-position-4.0.4.tgz#93f6d8c7d6b373d9b825844645877c127455f037"
+  integrity sha512-kUBE91efOWfIVBo8xzh/uZQ7p9ffYRtUbMRZBNFYwf0RK8koUMx6dGUfwylLOKmaT2cs4wSW96QoYUSXAyEtpg==
+  dependencies:
+    "@types/unist" "^2.0.0"
+
+unist-util-stringify-position@^3.0.0:
+  version "3.0.3"
+  resolved "https://registry.npmmirror.com/unist-util-stringify-position/-/unist-util-stringify-position-3.0.3.tgz#03ad3348210c2d930772d64b489580c13a7db39d"
+  integrity sha512-k5GzIBZ/QatR8N5X2y+drfpWG8IDBzdnVj6OInRNWm1oXrzydiaAT2OQiA8DPRRZyAKb9b6I2a6PxYklZD0gKg==
+  dependencies:
+    "@types/unist" "^2.0.0"
+
+unist-util-visit-parents@^5.0.0, unist-util-visit-parents@^5.1.1:
+  version "5.1.3"
+  resolved "https://registry.npmmirror.com/unist-util-visit-parents/-/unist-util-visit-parents-5.1.3.tgz#b4520811b0ca34285633785045df7a8d6776cfeb"
+  integrity sha512-x6+y8g7wWMyQhL1iZfhIPhDAs7Xwbn9nRosDXl7qoPTSCy0yNxnKc+hWokFifWQIDGi154rdUqKvbCa4+1kLhg==
+  dependencies:
+    "@types/unist" "^2.0.0"
+    unist-util-is "^5.0.0"
+
+unist-util-visit@^4.0.0:
+  version "4.1.2"
+  resolved "https://registry.npmmirror.com/unist-util-visit/-/unist-util-visit-4.1.2.tgz#125a42d1eb876283715a3cb5cceaa531828c72e2"
+  integrity sha512-MSd8OUGISqHdVvfY9TPhyK2VdUrPgxkUtWSuMHF6XAAFuL4LokseigBnZtPnJMu+FbynTkFNnFlyjxpVKujMRg==
+  dependencies:
+    "@types/unist" "^2.0.0"
+    unist-util-is "^5.0.0"
+    unist-util-visit-parents "^5.1.1"
+
 untildify@^4.0.0:
   version "4.0.0"
   resolved "https://registry.npmmirror.com/untildify/-/untildify-4.0.0.tgz#2bc947b953652487e4600949fb091e3ae8cd919b"
   integrity sha512-KK8xQ1mkzZeg9inewmFVDNkg3l5LUhoq9kN6iWYB/CC9YMG8HA+c1Q8HwDe6dEX7kErrEVNVBO3fWsVq5iDgtw==
 
 update-browserslist-db@^1.0.10:
   version "1.0.11"
@@ -4480,14 +5434,19 @@
 use-callback-ref@^1.3.0:
   version "1.3.0"
   resolved "https://registry.npmmirror.com/use-callback-ref/-/use-callback-ref-1.3.0.tgz#772199899b9c9a50526fedc4993fc7fa1f7e32d5"
   integrity sha512-3FT9PRuRdbB9HfXhEq35u4oZkvpJ5kuYbpqhCfmiZyReuRgpnhDlbr2ZEnnuS0RrJAPn6l23xjFg9kpDM+Ms7w==
   dependencies:
     tslib "^2.0.0"
 
+use-isomorphic-layout-effect@^1.1.2:
+  version "1.1.2"
+  resolved "https://registry.npmmirror.com/use-isomorphic-layout-effect/-/use-isomorphic-layout-effect-1.1.2.tgz#497cefb13d863d687b08477d9e5a164ad8c1a6fb"
+  integrity sha512-49L8yCO3iGT/ZF9QttjwLF/ZD9Iwto5LnH5LmEdk/6cFmXddqi2ulF0edxTwjj+7mqvpVVGQWvbXZdn32wRSHA==
+
 use-sidecar@^1.1.2:
   version "1.1.2"
   resolved "https://registry.npmmirror.com/use-sidecar/-/use-sidecar-1.1.2.tgz#2f43126ba2d7d7e117aa5855e5d8f0276dfe73c2"
   integrity sha512-epTbsLuzZ7lPClpz2TyryBfztm7m+28DlEv2ZCQ3MDr5ssiwyOwGH/e5F9CkfWjJ1t4clvI58yF822/GUkjjhw==
   dependencies:
     detect-node-es "^1.1.0"
     tslib "^2.0.0"
@@ -4498,14 +5457,42 @@
   integrity sha512-EPD5q1uXyFxJpCrLnCc1nHnq3gOa6DZBocAIiI2TaSCA7VCJ1UJDMagCzIkXNsUYfD1daK//LTEQ8xiIbrHtcw==
 
 uuid@^9.0.0:
   version "9.0.0"
   resolved "https://registry.npmmirror.com/uuid/-/uuid-9.0.0.tgz#592f550650024a38ceb0c562f2f6aa435761efb5"
   integrity sha512-MXcSTerfPa4uqyzStbRoTgt5XIe3x5+42+q1sDuy3R5MDk66URdLMOZe5aPX/SQd+kuYAh0FdP/pO28IkQyTeg==
 
+uvu@^0.5.0:
+  version "0.5.6"
+  resolved "https://registry.npmmirror.com/uvu/-/uvu-0.5.6.tgz#2754ca20bcb0bb59b64e9985e84d2e81058502df"
+  integrity sha512-+g8ENReyr8YsOc6fv/NVJs2vFdHBnBNdfE49rshrTzDWOlUx4Gq7KOS2GD8eqhy2j+Ejq29+SbKH8yjkAqXqoA==
+  dependencies:
+    dequal "^2.0.0"
+    diff "^5.0.0"
+    kleur "^4.0.3"
+    sade "^1.7.3"
+
+vfile-message@^3.0.0:
+  version "3.1.4"
+  resolved "https://registry.npmmirror.com/vfile-message/-/vfile-message-3.1.4.tgz#15a50816ae7d7c2d1fa87090a7f9f96612b59dea"
+  integrity sha512-fa0Z6P8HUrQN4BZaX05SIVXic+7kE3b05PWAtPuYP9QLHsLKYR7/AlLW3NtOrpXRLeawpDLMsVkmk5DG0NXgWw==
+  dependencies:
+    "@types/unist" "^2.0.0"
+    unist-util-stringify-position "^3.0.0"
+
+vfile@^5.0.0:
+  version "5.3.7"
+  resolved "https://registry.npmmirror.com/vfile/-/vfile-5.3.7.tgz#de0677e6683e3380fafc46544cfe603118826ab7"
+  integrity sha512-r7qlzkgErKjobAmyNIkkSpizsFPYiUPuJb5pNW1RB4JcYVZhs4lIbVqk8XPk033CV/1z8ss5pkax8SuhGpcG8g==
+  dependencies:
+    "@types/unist" "^2.0.0"
+    is-buffer "^2.0.0"
+    unist-util-stringify-position "^3.0.0"
+    vfile-message "^3.0.0"
+
 vite-plugin-svgr@^2.4.0:
   version "2.4.0"
   resolved "https://registry.npmmirror.com/vite-plugin-svgr/-/vite-plugin-svgr-2.4.0.tgz#9b14953955e79893ea7718089b9777a494e38fc6"
   integrity sha512-q+mJJol6ThvqkkJvvVFEndI4EaKIjSI0I3jNFgSoC9fXAz1M7kYTVUin8fhUsFojFDKZ9VHKtX6NXNaOLpbsHA==
   dependencies:
     "@rollup/pluginutils" "^5.0.2"
     "@svgr/core" "^6.5.1"
@@ -4585,14 +5572,19 @@
     strip-ansi "^6.0.0"
 
 wrappy@1:
   version "1.0.2"
   resolved "https://registry.npmmirror.com/wrappy/-/wrappy-1.0.2.tgz#b5243d8f3ec1aa35f1364605bc0d1036e30ab69f"
   integrity sha512-l4Sp/DRseor9wL6EvV2+TuQn63dMkPjZ/sp9XkghTEbV9KlPS1xUsZ3u7/IQO4wxtcFB4bgpQPRcR3QCvezPcQ==
 
+xtend@^4.0.0:
+  version "4.0.2"
+  resolved "https://registry.npmmirror.com/xtend/-/xtend-4.0.2.tgz#bb72779f5fa465186b1f438f674fa347fdb5db54"
+  integrity sha512-LKYU1iAXJXUgAXn9URjiu+MWhyUXHsvfp7mcuYm9dSUKK0/CjtrUwFAxD82/mCWbtLsGjFIad0wIsod4zrTAEQ==
+
 y18n@^5.0.5:
   version "5.0.8"
   resolved "https://registry.npmmirror.com/y18n/-/y18n-5.0.8.tgz#7f4934d0f7ca8c56f95314939ddcd2dd91ce1d55"
   integrity sha512-0pfFzegeDWJHJIAmTLRP2DwHjdF5s7jo9tuztdQxAhINCdvS+3nGINqPd00AphqJR/0LhANUS6/+7SCb98YOfA==
 
 yallist@^3.0.2:
   version "3.1.1"
@@ -4627,7 +5619,12 @@
     y18n "^5.0.5"
     yargs-parser "^21.1.1"
 
 yocto-queue@^0.1.0:
   version "0.1.0"
   resolved "https://registry.npmmirror.com/yocto-queue/-/yocto-queue-0.1.0.tgz#0294eb3dee05028d31ee1a5fa2c556a6aaf10a1b"
   integrity sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==
+
+zwitch@^2.0.0:
+  version "2.0.4"
+  resolved "https://registry.npmmirror.com/zwitch/-/zwitch-2.0.4.tgz#c827d4b0acb76fc3e685a4c6ec2902d51070e9d7"
+  integrity sha512-bXE4cR/kVZhKZX/RjPEflHaKVhUVl85noU3v6b8apfQEc1x4A+zBxjZ4lN8LqGd6WZ3dl98pY4o717VFmoPp+A==
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/app/app.py` & `carefree-drawboard-0.0.1a4/cfdraw/app/app.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/app/endpoints/assets.py` & `carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/assets.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/app/endpoints/project.py` & `carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/project.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # A simple file system based project manager
 # Should be easy to replace with a database based one
 
 import json
 
 from typing import Any
 from typing import List
+from pathlib import Path
+from filelock import FileLock
 from pydantic import BaseModel
+from cftool.web import raise_err
+from cftool.web import get_responses
+from cftool.misc import get_err_msg
 from cftool.misc import print_warning
 
 from cfdraw import constants
+from cfdraw.config import get_config
 from cfdraw.parsers import noli
 from cfdraw.app.schema import IApp
-from cfdraw.utils.misc import get_err_msg
-from cfdraw.utils.server import raise_err
-from cfdraw.utils.server import get_responses
 from cfdraw.app.endpoints.base import IEndpoint
 
 
 suffix = ".cfdraw"
 
 
 class ProjectMeta(BaseModel):
@@ -34,104 +37,103 @@
 
 
 class SaveProjectResponse(BaseModel):
     success: bool
     message: str
 
 
+def get_project_folder(userId: str) -> Path:
+    folder = get_config().upload_project_folder / userId
+    if not folder.exists():
+        folder.mkdir(parents=True)
+    return folder
+
+
+def get_meta_lock(userId: str) -> FileLock:
+    return FileLock(get_project_folder(userId) / "maintain_meta.lock")
+
+
+def get_save_project_lock(userId: str) -> FileLock:
+    return FileLock(get_project_folder(userId) / "save_project.lock")
+
+
+def get_delete_project_lock(userId: str) -> FileLock:
+    return FileLock(get_project_folder(userId) / "delete_project.lock")
+
+
+def move_to_buggy(path: Path, userId: str, err: Exception) -> None:
+    buggy_folder = get_project_folder(userId) / constants.BUGGY_PROJECT_FOLDER
+    buggy_folder.mkdir(parents=True, exist_ok=True)
+    lock = FileLock(buggy_folder / "move_to_buggy.lock")
+    with lock:
+        backup_path = buggy_folder / path.name
+        print_warning(
+            f"failed to load project '{path}', it will be moved to '{backup_path}'"
+            f" ({get_err_msg(err)})"
+        )
+        path.rename(buggy_folder / path.name)
+
+
 def maintain_meta(app: IApp, userId: str) -> None:
-    upload_project_folder = app.config.upload_project_folder / userId
-    if not upload_project_folder.exists():
-        upload_project_folder.mkdir(parents=True)
-    existing_projects = [
-        path.absolute()
-        for path in upload_project_folder.iterdir()
-        if path.is_file() and path.suffix == suffix
-    ]
-    meta_path = upload_project_folder / constants.PROJECT_META_FILE
-    checked = False
-    if meta_path.is_file():
-        try:
-            with open(meta_path, "r") as f:
-                project_meta = json.load(f)
-            if len(project_meta) == len(existing_projects):
-                checked = True
-            else:
-                print_warning("project meta file is not up-to-date")
-        except Exception as err:
-            print_warning(f"failed to check project meta file: {get_err_msg(err)}")
-    if checked:
-        return
-    project_meta = {}
-    for path in existing_projects:
-        try:
-            with open(path, "r") as f:
-                d = json.load(f)
-            project_meta[d["uid"]] = dict(
-                uid=d["uid"],
-                name=d["name"],
-                createTime=d["createTime"],
-                updateTime=d["updateTime"],
-            )
-        except Exception as err:
-            buggy_folder = upload_project_folder / constants.BUGGY_PROJECT_FOLDER
-            buggy_folder.mkdir(parents=True, exist_ok=True)
-            backup_path = buggy_folder / path.name
-            print_warning(
-                f"failed to load project '{path}', it will be moved to '{backup_path}'"
-                f" ({get_err_msg(err)})"
-            )
-            path.rename(buggy_folder / path.name)
-    with open(meta_path, "w") as f:
-        json.dump(project_meta, f)
+    with get_meta_lock(userId):
+        upload_project_folder = get_project_folder(userId)
+        existing_projects = [
+            path.absolute()
+            for path in upload_project_folder.iterdir()
+            if path.is_file() and path.suffix == suffix
+        ]
+        project_meta = {}
+        for path in existing_projects:
+            try:
+                with open(path, "r") as f:
+                    d = json.load(f)
+                project_meta[d["uid"]] = dict(
+                    uid=d["uid"],
+                    name=d["name"],
+                    createTime=d["createTime"],
+                    updateTime=d["updateTime"],
+                )
+            except Exception as err:
+                move_to_buggy(path, userId, err)
+        with open(upload_project_folder / constants.PROJECT_META_FILE, "w") as f:
+            json.dump(project_meta, f)
 
 
 def maintain_all_meta(app: IApp) -> None:
     for user_folder in app.config.upload_project_folder.iterdir():
         if user_folder.is_dir():
             maintain_meta(app, user_folder.name)
 
 
 def add_project_managements(app: IApp) -> None:
     @app.api.post("/save_project", responses=get_responses(SaveProjectResponse))
     def save_project(data: ProjectModel) -> SaveProjectResponse:
-        upload_project_folder = app.config.upload_project_folder / data.userId
-        if not upload_project_folder.exists():
-            upload_project_folder.mkdir(parents=True)
-        try:
-            file = f"{data.uid}{suffix}"
-            with open(upload_project_folder / file, "w") as f:
-                json.dump(data.dict(), f)
-            # maintain meta
-            meta_path = upload_project_folder / constants.PROJECT_META_FILE
-            if not meta_path.is_file():
+        with get_save_project_lock(data.userId):
+            try:
+                upload_project_folder = get_project_folder(data.userId)
+                with open(upload_project_folder / f"{data.uid}{suffix}", "w") as f:
+                    json.dump(data.dict(), f)
                 maintain_meta(app, data.userId)
-            else:
-                with open(meta_path, "r") as f:
-                    meta = json.load(f)
-                meta[data.uid] = dict(
-                    uid=data.uid,
-                    name=data.name,
-                    createTime=data.createTime,
-                    updateTime=data.updateTime,
-                )
-                with open(meta_path, "w") as f:
-                    json.dump(meta, f)
-        except Exception as err:
-            err_msg = get_err_msg(err)
-            return SaveProjectResponse(success=False, message=err_msg)
+            except Exception as err:
+                err_msg = get_err_msg(err)
+                return SaveProjectResponse(success=False, message=err_msg)
         return SaveProjectResponse(success=True, message="")
 
     @app.api.get("/get_project/", responses=get_responses(ProjectModel))
     async def fetch_project(userId: str, uid: str) -> ProjectModel:  # type: ignore
         try:
-            upload_project_folder = app.config.upload_project_folder / userId
-            file = f"{uid}{suffix}"
-            with open(upload_project_folder / file, "r") as f:
-                d = json.load(f)
+            with get_save_project_lock(userId):
+                with get_delete_project_lock(userId):
+                    upload_project_folder = get_project_folder(userId)
+                    path = upload_project_folder / f"{uid}{suffix}"
+                    try:
+                        with open(path, "r") as f:
+                            d = json.load(f)
+                    except Exception as err:
+                        move_to_buggy(path, userId, err)
 
             # TODO: this kind of transformation should be included in the
             # migration stage, not runtime stage. Will be fixed in the future
 
             # # replace url if needed
             # graph = noli.parse_graph(d["graphInfo"])
             # for node in graph.all_single_nodes:
@@ -148,45 +150,41 @@
 
             return ProjectModel(**d)
         except Exception as err:
             raise_err(err)
 
     @app.api.get("/all_projects/")
     async def fetch_all_projects(userId: str) -> List[ProjectMeta]:
-        upload_project_folder = app.config.upload_project_folder / userId
+        upload_project_folder = get_project_folder(userId)
         if not upload_project_folder.exists():
             return []
         meta_path = upload_project_folder / constants.PROJECT_META_FILE
         if not meta_path.is_file():
             maintain_meta(app, userId)
-        with open(meta_path, "r") as f:
-            meta = json.load(f)
+        try:
+            with get_meta_lock(userId):
+                with open(meta_path, "r") as f:
+                    meta = json.load(f)
+        except Exception as err:
+            print_warning(
+                f"failed to load project meta file '{meta_path}', "
+                f"will regenerate it ({get_err_msg(err)})"
+            )
+            maintain_meta(app, userId)
         s = sorted([(v["updateTime"], k) for k, v in meta.items()], reverse=True)
         return [ProjectMeta(**meta[k]) for _, k in s]
 
     @app.api.delete("/projects/")
     async def delete_project(userId: str, uid: str) -> None:
-        upload_project_folder = app.config.upload_project_folder / userId
-        if not upload_project_folder.exists():
-            return
-        file = f"{uid}{suffix}"
-        path = upload_project_folder / file
-        if path.is_file():
-            path.unlink()
-        # maintain meta
-        meta_path = upload_project_folder / constants.PROJECT_META_FILE
-        if not meta_path.is_file():
+        with get_delete_project_lock(userId):
+            upload_project_folder = get_project_folder(userId)
+            path = upload_project_folder / f"{uid}{suffix}"
+            if path.is_file():
+                path.unlink()
             maintain_meta(app, userId)
-        else:
-            with open(meta_path, "r") as f:
-                meta = json.load(f)
-            if uid in meta:
-                meta.pop(uid)
-                with open(meta_path, "w") as f:
-                    json.dump(meta, f)
 
 
 class ProjectEndpoint(IEndpoint):
     def register(self) -> None:
         add_project_managements(self.app)
 
     async def on_startup(self) -> None:
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/app/endpoints/queue.py` & `carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import asyncio
 
 from typing import Dict
 from typing import Tuple
 from typing import Optional
+from cftool.misc import get_err_msg
 from cftool.misc import print_error
 from cftool.misc import random_hash
 from cftool.misc import print_warning
+from cftool.data_structures import Item
+from cftool.data_structures import QueuesInQueue
 
 from cfdraw.app.schema import IRequestQueue
 from cfdraw.app.schema import IRequestQueueData
 from cfdraw.utils.misc import offload
-from cfdraw.utils.misc import get_err_msg
-from cfdraw.utils.data_structures import Item
-from cfdraw.utils.data_structures import QueuesInQueue
 from cfdraw.schema.plugins import ISend
 from cfdraw.schema.plugins import SocketStatus
 from cfdraw.schema.plugins import ISocketMessage
 
 
 DEBUG = False
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/app/endpoints/upload.py` & `carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from fastapi import File
 from fastapi import Form
 from fastapi import Request
 from fastapi import Response
 from fastapi import UploadFile
 from pydantic import BaseModel
 from PIL.PngImagePlugin import PngInfo
+from cftool.web import get_responses
+from cftool.web import get_image_response_kwargs
+from cftool.misc import get_err_msg
 
 from cfdraw import constants
 from cfdraw.app.schema import IApp
-from cfdraw.utils.misc import get_err_msg
 from cfdraw.utils.server import save_image
-from cfdraw.utils.server import get_responses
 from cfdraw.utils.server import get_image_response
-from cfdraw.utils.server import get_image_response_kwargs
 from cfdraw.app.endpoints.base import IEndpoint
 
 
 class ImageDataModel(BaseModel):
     w: int
     h: int
     url: str
@@ -48,14 +48,15 @@
     """
 
     @staticmethod
     async def upload_image(
         contents: Union[bytes, Image.Image],
         meta: PngInfo,
         base_url: str,
+        audit: bool,
     ) -> ImageDataModel:
         """
         When this method is used in the:
         * `upload_image` endpoint, `contents` will be a `bytes` object.
         * `FieldsMiddleWare`, `contents` will be an `Image.Image` object.
         """
 
@@ -72,23 +73,24 @@
 
 
 def add_upload_image(app: IApp) -> None:
     @app.api.post("/upload_image", responses=get_responses(UploadImageResponse))
     async def upload_image(
         image: UploadFile = File(),
         userId: str = Form(),
+        audit: bool = Form(True),
         *,
         request: Request,
     ) -> UploadImageResponse:
         try:
             base_url = str(request.base_url)
             contents = image.file.read()
             meta = PngInfo()
             meta.add_text("userId", userId)
-            data = await ImageUploader.upload_image(contents, meta, base_url)
+            data = await ImageUploader.upload_image(contents, meta, base_url, audit)
         except Exception as err:
             err_msg = get_err_msg(err)
             return UploadImageResponse(success=False, message=err_msg, data=None)
         finally:
             image.file.close()
         return UploadImageResponse(success=True, message="", data=data)
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/app/endpoints/websocket.py` & `carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
 import asyncio
 import logging
 
 from fastapi import WebSocket
 from fastapi import WebSocketDisconnect
+from cftool.misc import get_err_msg
 from cftool.misc import print_error
 from starlette.websockets import WebSocketState
 
 from cfdraw import constants
 from cfdraw.app.schema import IApp
 from cfdraw.app.schema import IRequestQueueData
 from cfdraw.utils.misc import offload
-from cfdraw.utils.misc import get_err_msg
 from cfdraw.schema.plugins import ElapsedTimes
 from cfdraw.schema.plugins import ISocketRequest
 from cfdraw.schema.plugins import ISocketMessage
 from cfdraw.app.endpoints.base import IEndpoint
 
 
 def add_websocket(app: IApp) -> None:
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/app/schema.py` & `carefree-drawboard-0.0.1a4/cfdraw/app/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/cli.py` & `carefree-drawboard-0.0.1a4/cfdraw/cli.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/config.py` & `carefree-drawboard-0.0.1a4/cfdraw/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 from importlib import import_module
 from dataclasses import field
 from dataclasses import dataclass
 
 from cfdraw import constants
 from cfdraw.utils.cache import cache_resource
+from cfdraw.schema.settings import ExtraPlugins
 from cfdraw.schema.settings import BoardSettings
 
 
 @dataclass
 class Config:
     # app
     entry: str = constants.DEFAULT_ENTRY
@@ -21,14 +22,16 @@
     backend_port: str = constants.BACKEND_PORT
     ## if provided, will be set as `CFDRAW_API_URL`
     backend_hosting_url: Optional[str] = None
     # upload
     upload_root: str = field(default_factory=constants.get_upload_root)
     # board
     board_settings: BoardSettings = BoardSettings()
+    # extra plugins
+    extra_plugins: ExtraPlugins = ExtraPlugins()
     # misc
     use_react_strict_mode: bool = False
 
     @property
     def prod(self) -> bool:
         return constants.get_env() == constants.Env.PROD
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/parsers/chakra.py` & `carefree-drawboard-0.0.1a4/cfdraw/parsers/chakra.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/parsers/noli.py` & `carefree-drawboard-0.0.1a4/cfdraw/parsers/noli.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/plugins/_internal/node_validator.py` & `carefree-drawboard-0.0.1a4/cfdraw/plugins/_internal/node_validator.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/plugins/_internal/sync.py` & `carefree-drawboard-0.0.1a4/cfdraw/plugins/_internal/sync.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,31 +10,32 @@
 class SyncSocketPlugin(IInternalSocketPlugin):
     async def process(self, data: ISocketRequest) -> ISocketMessage:
         config = get_config()
         return ISocketMessage.make_success(
             data.hash,
             dict(
                 pluginSettings=[
-                    plugin_type().to_plugin_settings()
+                    plugin_type().to_react()
                     for plugin_type in PluginFactory.plugins.values()
                     if not plugin_type._in_group
                 ],
                 internalSettings=dict(
                     useStrictMode=config.use_react_strict_mode,
                     sockenEndpoint=str(constants.Endpoint.WEBSOCKET),
                 ),
                 boardSettings=config.board_settings.to_filtered(),
+                extraPlugins=config.extra_plugins.dict(),
             ),
         )
 
 
 @PluginFactory.register_internal("sync_local_select")
 class SyncLocalSelectSocketPlugin(IInternalSocketPlugin):
     async def process(self, data: ISocketRequest) -> ISocketMessage:
-        values = ISelectLocalField.get_values(**data.extraData)
-        return ISocketMessage.make_success(data.hash, dict(values=values))
+        options = ISelectLocalField.get_options(**data.extraData)
+        return ISocketMessage.make_success(data.hash, dict(options=options))
 
 
 __all__ = [
     "SyncSocketPlugin",
     "SyncLocalSelectSocketPlugin",
 ]
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/plugins/factory.py` & `carefree-drawboard-0.0.1a4/cfdraw/plugins/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import Dict
 from typing import Type
 from typing import Callable
 from typing import NamedTuple
+from cftool.data_structures import Types
 
-from cfdraw.utils.data_structures import Types
 from cfdraw.schema.plugins import IPlugin
 from cfdraw.schema.plugins import IPluginSettings
 from cfdraw.schema.plugins import IPluginGroupInfo
 
 
 TPlugin = Type[IPlugin]
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/plugins/middlewares/response.py` & `carefree-drawboard-0.0.1a4/cfdraw/plugins/middlewares/response.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,16 +35,18 @@
                     type="text",
                     value=[dict(text=text, safe=True, reason="") for text in response],
                 )
             )
         meta = PngInfo()
         meta.add_text("request", self.request.json())
         t = time.time()
+        audit = self.plugin.image_should_audit
+        upload = ImageUploader.upload_image
         base_url = self.request.baseURL
-        futures = [ImageUploader.upload_image(im, meta, base_url) for im in response]
+        futures = [upload(im, meta, base_url, audit) for im in response]
         urls = [data.dict() for data in await asyncio.gather(*futures)]
         self.plugin.elapsed_times.upload = time.time() - t
         return self.make_success(dict(type="image", value=urls))
 
 
 __all__ = [
     "ResponseMiddleWare",
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/plugins/middlewares/send_message.py` & `carefree-drawboard-0.0.1a4/cfdraw/plugins/middlewares/send_message.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/plugins/middlewares/timer.py` & `carefree-drawboard-0.0.1a4/cfdraw/plugins/middlewares/timer.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/schema/fields.py` & `carefree-drawboard-0.0.1a4/cfdraw/schema/fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,67 +79,79 @@
 
 class ISelectLocalField(IBaseField):
     path: str = Field(..., description="The local path you want to read")
     default: Optional[str] = Field(None, description="The default value of the field")
     regex: Optional[str] = Field(None, description="The regex to filter the files")
     noExt: bool = Field(False, description="Whether to remove the extension")
     onlyFiles: bool = Field(True, description="Whether only consider files")
+    defaultPlaceholder: Optional[str] = Field(
+        None,
+        description="If provided, it will be inserted to the first of the options and serve as the default value",
+    )
     isMulti: Optional[bool] = Field(None, description="Whether use multi-select")
     type: FieldType = Field(FieldType.SELECT_LOCAL, description="Type", const=True)
 
     @staticmethod
-    def get_values(
+    def get_options(
         *,
         path: str,
-        regex: Optional[str],
+        regex: Optional[str] = None,
         noExt: bool,
         onlyFiles: bool,
+        defaultPlaceholder: Optional[str] = None,
     ) -> List[str]:
         p = Path(path)
+        if not p.is_dir():
+            return [] if defaultPlaceholder is None else [defaultPlaceholder]
         paths = [f for f in p.iterdir() if f]
         if onlyFiles:
             paths = [f for f in paths if f.is_file()]
         if regex:
             paths = [f for f in paths if re.search(regex, f.name)]
-        return sorted([f.stem if noExt else f.name for f in paths])
+        sorted_paths = sorted([f.stem if noExt else f.name for f in paths])
+        if defaultPlaceholder is None:
+            return sorted_paths
+        return [defaultPlaceholder] + sorted_paths
 
     def dict(self, **kwargs: Any) -> Dict[str, Any]:
         d = super().dict(**kwargs)
         d["type"] = FieldType.SELECT.value
         kw = dict(
             path=d.pop("path"),
             regex=d.pop("regex"),
             noExt=d.pop("noExt"),
             onlyFiles=d.pop("onlyFiles"),
+            defaultPlaceholder=d.pop("defaultPlaceholder"),
         )
-        values = self.get_values(**kw)
+        values = self.get_options(**kw)
         d["values"] = values
         if d["default"] is None:
-            d["default"] = "" if not values else values[0]
+            d["default"] = values[0]
         d["isLocal"] = True
         d["localProperties"] = kw
         return d
 
 
 class IBooleanField(IBaseField):
     default: bool = Field(..., description="The default value of the field")
     type: FieldType = Field(FieldType.BOOLEAN, description="Type", const=True)
 
 
 class IColorField(IBaseField):
-    default: IStr = Field("", description="The default value of the field")
+    default: IStr = Field("#ffffff", description="The default value of the field")
     type: FieldType = Field(FieldType.COLOR, description="Type", const=True)
 
 
 class IListField(IBaseField):
-    item: "IFieldDefinition" = Field(..., description="The item of the field")
+    item: Dict[str, "IFieldDefinition"] = Field(..., description="Definitions")
     default: List[Any] = Field(
         default_factory=lambda: [],
         description="The default items of the field",
     )
+    maxNumRows: Optional[int] = Field(None, description="Maximum number of rows")
     type: FieldType = Field(FieldType.LIST, description="Type", const=True)
 
 
 class IObjectField(IBaseField):
     fields: Dict[str, "IFieldDefinition"] = Field(..., description="Sub fields")
     default: Dict[str, Any] = Field(
         default_factory=lambda: {},
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/schema/plugins.py` & `carefree-drawboard-0.0.1a4/cfdraw/schema/plugins.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from typing import Callable
 from typing import Optional
 from typing import Coroutine
 from aiohttp import ClientSession
 from pydantic import Field
 from pydantic import BaseModel
 
+from cfdraw import constants
 from cfdraw.utils.misc import deprecated
 from cfdraw.schema.fields import IFieldDefinition
 from cfdraw.parsers.noli import IStr
 from cfdraw.parsers.noli import Matrix2D
 from cfdraw.parsers.noli import INodeType
 from cfdraw.parsers.noli import PivotType
 from cfdraw.parsers.noli import SingleNodeType
@@ -36,19 +37,20 @@
 
 class PluginType(str, Enum):
     """
     These types should align with the `allPythonPlugins` locates at
     `cfdraw/.web/src/schema/plugins.ts`
     """
 
+    PLUGIN_GROUP = "_python.pluginGroup"
     FIELDS = "_python.fields"
     TEXT_AREA = "_python.textArea"
     QA = "_python.QA"
     CHAT = "_python.chat"
-    PLUGIN_GROUP = "_python.pluginGroup"
+    MARKDOWN = "_python.markdown"
 
     # this type of plugins will not be rendered on the drawboard 🎨
     _INTERNAL = "_internal"
 
 
 class ReactPluginType(str, Enum):
     """
@@ -62,25 +64,30 @@
     ADD = "add"
     ARRANGE = "arrange"
     UNDO = "undo"
     REDO = "redo"
     DOWNLOAD = "download"
     DELETE = "delete"
     WIKI = "wiki"
-    GITHUB = "github"
     EMAIL = "email"
+    GITHUB = "github"
+    LOGO = "logo"
     TEXT_EDITOR = "textEditor"
     GROUP_EDITOR = "groupEditor"
     MULTI_EDITOR = "multiEditor"
     BRUSH = "brush"
 
 
 # general
 
 
+def hash_identifier(hash: str, identifier: str) -> str:
+    return f"{identifier}.{hash}"
+
+
 class IPluginInfo(BaseModel):
     """
     This should align with the following interfaces locate at `cfdraw/.web/src/schema/_python.ts`:
     * `IPythonPluginInfo`: `name`
     * `IPythonSocketIntervals`: `retryInterval`, `updateInterval`
     * `IPythonPluginWithSubmitPluginInfo`: `closeOnSubmit`, `toastOnSubmit`, `toastMessageOnSubmit`
     """
@@ -107,14 +114,52 @@
     toastMessageOnSubmit: Optional[IStr] = Field(
         None,
         description="The message of the toast, only take effect when `toastOnSubmit` is `True`",
     )
 
 
 class IPluginSettings(IChakra):
+    """
+    This should align with the `IPythonPlugin` locate at `cfdraw/.web/src/schema/_python.ts`,
+    but for the sake of accessibility, we 'flattened' the fields. Here's a detailed explanation:
+
+    --- IChakra --
+
+    > Fields of `IChakra`, except `w` & `h`, will be injected to the `buttonProps`.
+    >> `w` & `h` has special meanings so we need to skip them.
+    > Documents of `charaProps` is listed below (the --- React fields --- section).
+
+    --- required fields ---
+
+    * `w` and `h` are the width and height of the expanded plugin, respectively.
+    > Sometimes a plugin need not to be expanded, in this case, you can set `w` and `h` to `0`.
+    > These two fields will go to the `renderInfo` part of the `IRender`, locates at
+    `cfdraw/.web/src/schema/plugins.ts`.
+
+    --- node constraints ---
+
+    > These fields will go to the `NodeConstraintSettings` part of the `IRender`, locates at
+    `cfdraw/.web/src/schema/plugins.ts`.
+    > See Plugin Positioning (https://github.com/carefree0910/carefree-drawboard/wiki/Details#plugin-positioning)
+    for detailed explanations of these fields.
+
+    --- style fields ---
+
+    > These fields will go to the `renderInfo` part of the `IRender`, locates at
+    `cfdraw/.web/src/schema/plugins.ts`.
+    > Which means they should align with the `IRenderInfo` locates at the same file.
+
+    --- React fields ---
+
+    * the `pluginInfo` maps to `IPythonPluginInfo`, but the `identifier` is injected on the fly.
+    * the `buttonProps` is the universal fallback for you to inject any `ButtonProps` to the
+    plugin button. (see `cfdraw/.web/src/schema/plugins.ts`, where you can see
+    `export interface IFloating extends ButtonProps`)
+    """
+
     # required fields
     w: int = Field(..., gt=0, description="Width of the expanded plugin")  # type: ignore
     h: int = Field(..., gt=0, description="Height of the expanded plugin")  # type: ignore
     # node constraints
     nodeConstraint: Optional[NodeConstraints] = Field(
         None,
         description="""
@@ -179,21 +224,72 @@
     )
     iconW: Optional[int] = Field(None, description="Width of the plugin button")
     iconH: Optional[int] = Field(None, description="Height of the plugin button")
     offsetX: Optional[int] = Field(None, description="X offset of the plugin button")
     offsetY: Optional[int] = Field(None, description="Y offset of the plugin button")
     bgOpacity: Optional[float] = Field(None, description="Opacity of the plugin button")
     useModal: bool = Field(False, description="Whether popup a modal for the plugin")
+    keepOpen: bool = Field(
+        False,
+        description="Whether should we keep the expanded panel of the plugin open, even when users already clicked on the drawboard.",
+    )
     modalOpacity: Optional[float] = Field(None, description="Opacity of the modal")
     expandProps: Optional[IChakra] = Field(
         None,
         description="Extra (chakra) props of the plugin's expanded panel",
     )
     # React fields
     pluginInfo: IPluginInfo = Field(IPluginInfo(), description="Plugin info")
+    buttonProps: Optional[Dict[str, Any]] = Field(
+        None,
+        description="Extra (chakra) props of the plugin button",
+    )
+
+    def to_react(self, type: str, hash: str, identifier: str) -> Dict[str, Any]:
+        d = self.dict(exclude={"pluginInfo"})
+        pI = self.pluginInfo
+        kw = dict(exclude={"plugins"}) if isinstance(pI, IPluginGroupInfo) else {}
+        plugin_info = self.pluginInfo.dict(**kw)
+        plugin_info["identifier"] = identifier
+        if isinstance(pI, IPluginGroupInfo):
+            plugins: List[Dict[str, Any]] = []
+            for p_identifier, p_base in pI.plugins.items():
+                p_base.hash = hash
+                p = p_base()
+                p.identifier = p_identifier
+                plugins.append(p.to_react())
+            plugin_info["plugins"] = plugins
+        node_constraint = d.pop("nodeConstraint")
+        node_constraint_rules = d.pop("nodeConstraintRules")
+        node_constraint_validator = d.pop("nodeConstraintValidator")
+        button_props = d.pop("buttonProps", None) or {}
+        for field in IChakra.__fields__:
+            # `w` and `h` are special fields, should not be included in `chakra_props`
+            if field in ["w", "h"]:
+                continue
+            chakra_value = d.pop(field)
+            if chakra_value is not None:
+                button_props[field] = chakra_value
+        for k, v in list(d.items()):
+            if v is None:
+                d.pop(k)
+        # src
+        if not isinstance(pI, IPluginGroupInfo):
+            d.setdefault("src", constants.DEFAULT_PLUGIN_ICON)
+        else:
+            d.setdefault("src", constants.DEFAULT_PLUGIN_GROUP_ICON)
+        # gather
+        props = dict(pluginInfo=plugin_info, renderInfo=d, **button_props)
+        if node_constraint is not None:
+            props["nodeConstraint"] = node_constraint
+        if node_constraint_rules is not None:
+            props["nodeConstraintRules"] = node_constraint_rules
+        if node_constraint_validator is not None:
+            props["nodeConstraintValidator"] = node_constraint_validator
+        return dict(type=type, props=props)
 
 
 class ElapsedTimes(BaseModel):
     """This should align with `IElapsedTimes` at `cfdraw/.web/src/schema/meta.ts`"""
 
     createTime: Optional[float]
     startTime: Optional[float]
@@ -402,15 +498,15 @@
         pass
 
     @abstractmethod
     async def __call__(self, data: ISocketRequest) -> ISocketMessage:
         pass
 
     @abstractmethod
-    def to_plugin_settings(self) -> Dict[str, Any]:
+    def to_react(self) -> Dict[str, Any]:
         pass
 
     @abstractmethod
     def filter(self, nodes: List[INodeData], target: SingleNodeType) -> List[INodeData]:
         pass
 
     @abstractmethod
@@ -425,14 +521,16 @@
         textList: Optional[List[str]] = None,
         imageList: Optional[List[str]] = None,
     ) -> bool:
         pass
 
     # optional
 
+    ## Whether the images generated by this plugin should be audited
+    image_should_audit: bool = True
     ## List of python package requirements of the plugin
     requirements: Optional[List[str]] = None
     ## The notification (introductions, hardware requirements, etc.) you want to print out
     notification: Optional[str] = None
 
 
 class Subscription(str, Enum):
@@ -485,14 +583,33 @@
     def make_success(self, final: Dict[str, Any]) -> ISocketMessage:
         return ISocketMessage.make_success(self.hash, final)
 
 
 # (react) bindings
 
 
+class ILogoPluginInfo(IPluginInfo):
+    """This should align with `ILogoPlugin` at `cfdraw/.web/src/schema/plugins.ts`"""
+
+    redirectUrl: Optional[IStr] = Field(
+        None,
+        description="Redirection target when clicking the logo, `None` means no redirection",
+    )
+
+
+class ILogoSettings(IPluginSettings):
+    w: int = Field(0, gt=0, description="Width of the expanded plugin")  # type: ignore
+    h: int = Field(0, gt=0, description="Height of the expanded plugin")  # type: ignore
+
+
+class IPluginGroupInfo(IPluginInfo):
+    header: Optional[IStr] = Field(None, description="Header of the plugin group")
+    plugins: Dict[str, Type[IPlugin]] = Field(..., description="Plugins in the group")
+
+
 class IFieldsPluginInfo(IPluginInfo):
     """This should align with `IPythonFieldsPlugin` at `cfdraw/.web/src/schema/_python.ts`"""
 
     header: Optional[IStr] = Field(None, description="Header of the plugin")
     definitions: Dict[str, IFieldDefinition] = Field(
         ...,
         description="Field definitions",
@@ -524,52 +641,34 @@
 
     initialText: IStr = Field(
         "",
         description="The initial text to be displayed in the text area",
     )
 
 
-class IPluginGroupInfo(IPluginInfo):
-    header: Optional[IStr] = Field(None, description="Header of the plugin group")
-    plugins: Dict[str, Type[IPlugin]] = Field(..., description="Plugins in the group")
-
-
-## deprecated
-
-
-@deprecated("please use `ITextAreaPluginInfo` instead")
-class IHttpTextAreaPluginInfo(ITextAreaPluginInfo):
-    pass
-
-
-@deprecated("please use `IQAPluginInfo` instead")
-class IHttpQAPluginInfo(IQAPluginInfo):
-    pass
-
-
 __all__ = [
     "ISend",
     "PluginType",
     "ReactPluginType",
     # general
+    "hash_identifier",
     "IPluginInfo",
     "IPluginSettings",
     # web
     "INodeData",
     "ISocketRequest",
     "SocketStatus",
     "ISocketIntermediate",
     "ISocketResponse",
     "ISocketMessage",
     # plugin interface
     "IPlugin",
     "IMiddleWare",
     "IFieldsPluginInfo",
     # bindings
+    "ILogoPluginInfo",
+    "ILogoSettings",
+    "IPluginGroupInfo",
     "ITextAreaPluginInfo",
     "IQAPluginInfo",
     "IChatPluginInfo",
-    "IPluginGroupInfo",
-    # deprecated
-    "IHttpTextAreaPluginInfo",
-    "IHttpQAPluginInfo",
 ]
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/utils/cache.py` & `carefree-drawboard-0.0.1a4/cfdraw/utils/cache.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/utils/console.py` & `carefree-drawboard-0.0.1a4/cfdraw/utils/console.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/utils/exec.py` & `carefree-drawboard-0.0.1a4/cfdraw/utils/exec.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/utils/misc.py` & `carefree-drawboard-0.0.1a4/cfdraw/utils/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-import sys
 import asyncio
 import threading
 
 from typing import Any
 from typing import TypeVar
 from typing import Callable
 from typing import Coroutine
+from cftool.misc import get_err_msg
 from cftool.misc import print_error
 from cftool.misc import print_warning
 from concurrent.futures import ThreadPoolExecutor
 
 
 TFutureResponse = TypeVar("TFutureResponse")
 
 
-def get_err_msg(err: Exception) -> str:
-    return " | ".join(map(repr, sys.exc_info()[:2] + (str(err),)))
-
-
 def deprecated(message: str) -> Callable[[type], type]:
     def _deprecated(cls: type) -> type:
         def init(self: Any, *args: Any, **kwargs: Any) -> None:
             if not cls._warned_deprecation:  # type: ignore
                 print_warning(f"{cls.__name__} is deprecated, {message}")
                 cls._warned_deprecation = True  # type: ignore
             original_init(self, *args, **kwargs)
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/utils/prerequisites.py` & `carefree-drawboard-0.0.1a4/cfdraw/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/utils/processes.py` & `carefree-drawboard-0.0.1a4/cfdraw/utils/processes.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/utils/server.py` & `carefree-drawboard-0.0.1a4/cfdraw/utils/server.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,25 @@
 import random
-import socket
-import logging
 
 import numpy as np
 
 from io import BytesIO
 from PIL import Image
 from typing import Any
 from typing import Dict
-from typing import Type
 from typing import Union
-from typing import Optional
 from fastapi import Response
-from fastapi import HTTPException
-from pydantic import BaseModel
 from PIL.PngImagePlugin import PngInfo
 from cftool.cv import to_rgb
 from cftool.cv import np_to_bytes
+from cftool.web import raise_err
 from cftool.misc import random_hash
 
 from cfdraw import constants
 from cfdraw.config import get_config
-from cfdraw.utils.misc import get_err_msg
-
-
-class RuntimeError(BaseModel):
-    detail: str
-
-    class Config:
-        schema_extra = {
-            "example": {"detail": "RuntimeError occurred."},
-        }
-
-
-def get_ip() -> str:
-    return socket.gethostbyname(socket.gethostname())
-
-
-def get_responses(
-    success_model: Type[BaseModel],
-    *,
-    json_example: Optional[Dict[str, Any]] = None,
-) -> Dict[int, Dict[str, Type]]:
-    success_response: Dict[str, Any] = {"model": success_model}
-    if json_example is not None:
-        content = success_response["content"] = {}
-        json_field = content["application/json"] = {}
-        json_field["example"] = json_example
-    return {
-        200: success_response,
-        constants.ERR_CODE: {"model": RuntimeError},
-    }
-
-
-def get_image_response_kwargs() -> Dict[str, Any]:
-    example = "\\x89PNG\\r\\n\\x1a\\n\\x00\\x00\\x00\\rIHDR\\x00\\x00\\x00\\x01\\x00\\x00\\x00\\x01\\x08\\x00\\x00\\x00\\x00:~\\x9bU\\x00\\x00\\x00\\nIDATx\\x9cc`\\x00\\x00\\x00\\x02\\x00\\x01H\\xaf\\xa4q\\x00\\x00\\x00\\x00IEND\\xaeB`\\x82"
-    responses = {
-        200: {"content": {"image/png": {"example": example}}},
-        constants.ERR_CODE: {"model": RuntimeError},
-    }
-    description = """
-Bytes of the output image.
-+ When using `requests` in `Python`, you can get the `bytes` with `res.content`.
-+ When using `fetch` in `JavaScript`, you can get the `Blob` with `await res.blob()`.
-"""
-    return dict(
-        responses=responses,
-        response_class=Response(content=b""),
-        response_description=description,
-    )
-
-
-def raise_err(err: Exception) -> None:
-    logging.exception(err)
-    raise HTTPException(status_code=constants.ERR_CODE, detail=get_err_msg(err))
 
 
 def save_image(image: Image.Image, meta: PngInfo, base_url: str) -> Dict[str, Any]:
     w, h = image.size
     config = get_config()
     state = random.getstate()
     random.seed()
```

### Comparing `carefree-drawboard-0.0.1a3/cfdraw/utils/template.py` & `carefree-drawboard-0.0.1a4/cfdraw/utils/template.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a3/setup.py` & `carefree-drawboard-0.0.1a4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.1-alpha.3"
+VERSION = "0.0.1-alpha.4"
 PACKAGE_NAME = "carefree-drawboard"
 
 DESCRIPTION = "🎨 Infinite Drawboard in Python"
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
@@ -19,19 +19,21 @@
         "fastapi>=0.95.1",
         "gunicorn",
         "pydantic",
         "uvicorn",
         "websockets",
         "watchdog",
         "python-multipart",
-        "carefree-toolkit>=0.3.4",
+        "carefree-toolkit>=0.3.5",
         "pillow",
         "aiohttp",
         "charset-normalizer==2.1.0",
         "aiofiles",
+        "regex",
+        "filelock",
     ],
     author="carefree0910",
     author_email="syameimaru.saki@gmail.com",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     keywords="python carefree-learn drawboard",
```

