# Comparing `tmp/gitlab_changelog_tool-1.0.0-py3-none-any.whl.zip` & `tmp/gitlab_changelog_tool-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 7357 bytes, number of entries: 11
--rw-r--r--  2.0 unx       71 b- defN 23-May-22 11:37 gitlab_changelog_tool/__init__.py
--rw-r--r--  2.0 unx      140 b- defN 23-May-22 11:37 gitlab_changelog_tool/__main__.py
--rw-r--r--  2.0 unx     4574 b- defN 23-May-22 11:37 gitlab_changelog_tool/api.py
--rw-r--r--  2.0 unx     1989 b- defN 23-May-22 11:37 gitlab_changelog_tool/cli.py
--rw-r--r--  2.0 unx      614 b- defN 23-May-22 11:37 gitlab_changelog_tool/package.py
--rw-r--r--  2.0 unx     1502 b- defN 23-May-22 11:37 gitlab_changelog_tool-1.0.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     4623 b- defN 23-May-22 11:37 gitlab_changelog_tool-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 11:37 gitlab_changelog_tool-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       77 b- defN 23-May-22 11:37 gitlab_changelog_tool-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-May-22 11:37 gitlab_changelog_tool-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1003 b- defN 23-May-22 11:37 gitlab_changelog_tool-1.0.0.dist-info/RECORD
-11 files, 14707 bytes uncompressed, 5619 bytes compressed:  61.8%
+Zip file size: 7760 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       71 b- defN 23-May-22 12:10 gitlab_changelog_tool/__init__.py
+-rw-r--r--  2.0 unx      140 b- defN 23-May-22 12:10 gitlab_changelog_tool/__main__.py
+-rw-r--r--  2.0 unx     4574 b- defN 23-May-22 12:10 gitlab_changelog_tool/api.py
+-rw-r--r--  2.0 unx     1989 b- defN 23-May-22 12:10 gitlab_changelog_tool/cli.py
+-rw-r--r--  2.0 unx      614 b- defN 23-May-22 12:10 gitlab_changelog_tool/package.py
+-rw-r--r--  2.0 unx      430 b- defN 23-May-22 12:10 gitlab_changelog_tool/templates/CHANGELOG.md
+-rw-r--r--  2.0 unx     1502 b- defN 23-May-22 12:10 gitlab_changelog_tool-1.0.1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     4623 b- defN 23-May-22 12:10 gitlab_changelog_tool-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-22 12:10 gitlab_changelog_tool-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       77 b- defN 23-May-22 12:10 gitlab_changelog_tool-1.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-May-22 12:10 gitlab_changelog_tool-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1103 b- defN 23-May-22 12:10 gitlab_changelog_tool-1.0.1.dist-info/RECORD
+12 files, 15237 bytes uncompressed, 5858 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -9,26 +9,29 @@
 
 Filename: gitlab_changelog_tool/cli.py
 Comment: 
 
 Filename: gitlab_changelog_tool/package.py
 Comment: 
 
-Filename: gitlab_changelog_tool-1.0.0.dist-info/LICENSE.md
+Filename: gitlab_changelog_tool/templates/CHANGELOG.md
 Comment: 
 
-Filename: gitlab_changelog_tool-1.0.0.dist-info/METADATA
+Filename: gitlab_changelog_tool-1.0.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: gitlab_changelog_tool-1.0.0.dist-info/WHEEL
+Filename: gitlab_changelog_tool-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: gitlab_changelog_tool-1.0.0.dist-info/entry_points.txt
+Filename: gitlab_changelog_tool-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: gitlab_changelog_tool-1.0.0.dist-info/top_level.txt
+Filename: gitlab_changelog_tool-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: gitlab_changelog_tool-1.0.0.dist-info/RECORD
+Filename: gitlab_changelog_tool-1.0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: gitlab_changelog_tool-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gitlab_changelog_tool/package.py

```diff
@@ -2,15 +2,15 @@
 Package description information.
 '''
 
 #: Package display name.
 __title__ = 'GitLab Changelog Tool'
 
 #: Package version.
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 #: Package description.
 __description__ = 'Automatically generate changelogs from merge requests on GitLab.'
 
 #: Package author name.
 __author__ = 'Danilo Peixoto Ferreira'
```

## Comparing `gitlab_changelog_tool-1.0.0.dist-info/LICENSE.md` & `gitlab_changelog_tool-1.0.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `gitlab_changelog_tool-1.0.0.dist-info/METADATA` & `gitlab_changelog_tool-1.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-changelog-tool
-Version: 1.0.0
+Version: 1.0.1
 Summary: Automatically generate changelogs from merge requests on GitLab.
 Home-page: https://github.com/danilopeixoto/gitlab-changelog-tool
 Download-URL: https://pypi.org/project/gitlab-changelog-tool
 Author: Danilo Peixoto Ferreira
 License: BSD-3-Clause
 Project-URL: Code, https://github.com/danilopeixoto/gitlab-changelog-tool
 Project-URL: Issue tracker, https://github.com/danilopeixoto/gitlab-changelog-tool/issues
```

