# Comparing `tmp/mkdocs-git-authors-plugin-0.7.0.tar.gz` & `tmp/mkdocs-git-authors-plugin-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-git-authors-plugin-0.7.0.tar", last modified: Wed Nov  2 20:17:28 2022, max compression
+gzip compressed data, was "mkdocs-git-authors-plugin-0.7.1.tar", last modified: Mon May 22 18:11:49 2023, max compression
```

## Comparing `mkdocs-git-authors-plugin-0.7.0.tar` & `mkdocs-git-authors-plugin-0.7.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 20:17:28.671512 mkdocs-git-authors-plugin-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-11-02 20:16:27.000000 mkdocs-git-authors-plugin-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3904 2022-11-02 20:17:28.671512 mkdocs-git-authors-plugin-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2989 2022-11-02 20:16:27.000000 mkdocs-git-authors-plugin-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 20:17:28.667512 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 20:16:27.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3539 2022-11-02 20:16:27.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/ci.py
--rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-11-02 20:16:27.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/exclude.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 20:17:28.667512 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/git/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 20:16:27.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4777 2022-11-02 20:16:27.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/git/author.py
--rw-r--r--   0 runner    (1001) docker     (121)     3377 2022-11-02 20:16:27.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/git/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1947 2022-11-02 20:16:27.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/git/commit.py
--rw-r--r--   0 runner    (1001) docker     (121)     6633 2022-11-02 20:16:27.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/git/page.py
--rw-r--r--   0 runner    (1001) docker     (121)     5000 2022-11-02 20:16:27.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/git/repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     8580 2022-11-02 20:16:27.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     4192 2022-11-02 20:16:27.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 20:17:28.667512 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3904 2022-11-02 20:17:28.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-11-02 20:17:28.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 20:17:28.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-02 20:17:28.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-02 20:17:28.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-02 20:17:28.000000 mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-02 20:17:28.671512 mkdocs-git-authors-plugin-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2022-11-02 20:16:27.000000 mkdocs-git-authors-plugin-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:11:49.851965 mkdocs-git-authors-plugin-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-22 18:11:49.851965 mkdocs-git-authors-plugin-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:11:49.851965 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/exclude.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:11:49.851965 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/author.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:11:49.851965 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-22 18:11:49.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-22 18:11:49.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:11:49.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-22 18:11:49.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 18:11:49.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 18:11:49.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 18:11:49.851965 mkdocs-git-authors-plugin-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/setup.py
```

### Comparing `mkdocs-git-authors-plugin-0.7.0/LICENSE` & `mkdocs-git-authors-plugin-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.7.0/PKG-INFO` & `mkdocs-git-authors-plugin-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-git-authors-plugin
-Version: 0.7.0
+Version: 0.7.1
 Summary: Mkdocs plugin to display git authors of a page
 Home-page: https://github.com/timvink/mkdocs-git-authors-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs git contributors committers authors plugin
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Documentation
 Classifier: Topic :: Text Processing
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Actions Status](https://github.com/timvink/mkdocs-git-authors-plugin/workflows/pytest/badge.svg)](https://github.com/timvink/mkdocs-git-authors-plugin/actions)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-git-authors-plugin)
 ![PyPI](https://img.shields.io/pypi/v/mkdocs-git-authors-plugin)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mkdocs-git-authors-plugin)
```

### Comparing `mkdocs-git-authors-plugin-0.7.0/README.md` & `mkdocs-git-authors-plugin-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/ci.py` & `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/ci.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,34 +3,56 @@
 
 This is because often CI runners do not have access to full git history.
 
 Taken from https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/blob/master/mkdocs_git_revision_date_localized_plugin/ci.py
 """
 
 import os
+from contextlib import contextmanager
 import logging
-
 from pathlib import Path
+from typing import Union
 from mkdocs_git_authors_plugin.git.command import GitCommand
 
 
+@contextmanager
+def working_directory(path: Union[str, Path]):
+    """
+    Temporarily change working directory.
+    A context manager which changes the working directory to the given
+    path, and then changes it back to its previous value on exit.
+    Usage:
+    ```python
+    # Do something in original directory
+    with working_directory('/my/new/path'):
+        # Do something in new directory
+    # Back to old directory
+    ```
+    """    
+    origin = Path().absolute()
+    try:
+        os.chdir(path)
+        yield
+    finally:
+        os.chdir(origin)
+
+
 def raise_ci_warnings(path: str) -> None:
     """
     Raise warnings when users use plugin on CI build runners.
 
     Args:
         path (str): path to the root of the git repo
     """
-    with Path(path):
+    with working_directory(path):
         if not is_shallow_clone():
             return None
 
         n_commits = commit_count()
 
-
     # Gitlab Runners
     if os.getenv("GITLAB_CI") is not None and n_commits < 50:
         # Default is GIT_DEPTH of 50 for gitlab
         logging.warning(
             """
                 [git-authors] Running on a GitLab runner might lead to wrong
                 Git revision dates due to a shallow git fetch depth.
@@ -84,17 +106,17 @@
 def commit_count() -> int:
     """
     Determine the number of commits in a repository.
 
     Returns:
         count (int): Number of commits.
     """
-    gc = GitCommand('rev-list',['--count','HEAD'])
+    gc = GitCommand("rev-list", ["--count", "HEAD"])
     gc.run()
-    n_commits = int(gc._stdout[0])
+    n_commits = int(gc._stdout[0])  # type: ignore
     assert n_commits >= 0
     return n_commits
 
 
 def is_shallow_clone() -> bool:
     """
     Determine if repository is a shallow clone.
```

### Comparing `mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/exclude.py` & `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/exclude.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/git/author.py` & `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/author.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from .repo import AbstractRepoObject, Repo
 from .page import Page
 from .commit import Commit
 
+from typing import Dict
+
 
 class Author(AbstractRepoObject):
     """
     Abstraction of an author in the Git repository.
     """
 
     def __init__(self, repo: Repo, name: str, email: str):
@@ -16,15 +18,15 @@
             repo: reference to the global Repo instance
             name: author's full name
             email: author's email
         """
         super().__init__(repo)
         self._name = name
         self._email = email
-        self._pages = {}
+        self._pages: Dict[str, dict] = dict()
 
     def add_lines(self, page: Page, commit: Commit, lines: int = 1):
         """
         Add line(s) in a given page/commit to the author's data.
 
         Args:
             page: Page object referencing the markdown file
```

### Comparing `mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/git/command.py` & `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/command.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/git/commit.py` & `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/commit.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             sha: 40-byte SHA string
         """
 
         super().__init__(repo)
 
         # Replace <>
         # from '<email@domain.com>'
-        # to   'email@domain.com'        
+        # to   'email@domain.com'
         author_email = re.sub(r"\<|\>", "", author_email)
         # Lowercase, as emails are not case sensitive.
         # See https://github.com/timvink/mkdocs-git-authors-plugin/issues/59
         author_email = author_email.lower()
 
         self._author = self.repo().author(author_name, author_email)
         self._datetime = util.commit_datetime(author_time, author_tz)
```

### Comparing `mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/git/page.py` & `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/page.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from pathlib import Path
 import re
 import logging
 from .repo import Repo, AbstractRepoObject
 from .command import GitCommand, GitCommandError
 
+from typing import List
+
 logger = logging.getLogger("mkdocs.plugins")
 
 
 class Page(AbstractRepoObject):
     """
     Results of git blame for a given file.
 
@@ -24,15 +26,15 @@
             repo: Reference to the global Repo instance
             path: Absolute path to the page's Markdown file
         """
         super().__init__(repo)
         self._path = path
         self._sorted = False
         self._total_lines = 0
-        self._authors = []
+        self._authors: List[dict] = list()
         try:
             self._process_git_blame()
         except GitCommandError:
             logger.warning(
                 "[git-authors-plugin] %s has not been committed yet. Lines are not counted"
                 % path
             )
@@ -56,20 +58,28 @@
         Args:
 
         Returns:
             sorted list with Author objects
         """
         if not self._sorted:
             repo = self.repo()
-            reverse = repo.config("show_line_count") or repo.config("show_contribution") or repo.config("sort_authors_by") == "contribution"
+            reverse = (
+                repo.config("show_line_count")
+                or repo.config("show_contribution")
+                or repo.config("sort_authors_by") == "contribution"
+            )
             self._authors = sorted(self._authors, key=repo._sort_key, reverse=reverse)
             self._sorted = True
             author_threshold = repo.config("authorship_threshold_percent")
             if author_threshold > 0 and len(self._authors) > 1:
-                self._authors = [a for a in self._authors if a.contribution()*100 > author_threshold]
+                self._authors = [
+                    a
+                    for a in self._authors
+                    if a.contribution() * 100 > author_threshold
+                ]
         return self._authors
 
     def _process_git_blame(self):
         """
         Execute git blame and parse the results.
 
         This retrieves all data we need, also for the Commit object.
```

### Comparing `mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/git/repo.py` & `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             self._authors[email] = Author(self, name, email)
         return self._authors[email]
 
     def get_authors(self):
         """
         Sorted list of authors in the repository.
 
-        Default sort order is by ascending names, 
+        Default sort order is by ascending names,
         and decending when contribution or line count is shown
 
         Args:
 
         Returns:
             List of Author objects
         """
@@ -148,15 +148,19 @@
 
         Args:
             author: an Author object
 
         Returns:
             comparison key for the sorted() function,
         """
-        if self.config("show_line_count") or self.config("show_contribution") or self.config("sort_authors_by") == "contribution":
+        if (
+            self.config("show_line_count")
+            or self.config("show_contribution")
+            or self.config("sort_authors_by") == "contribution"
+        ):
             key = "contribution"
         else:
             key = "name"
 
         func = getattr(author, key)
         return func()
```

### Comparing `mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/plugin.py` & `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from . import util
 from .git.repo import Repo
 from mkdocs_git_authors_plugin.ci import raise_ci_warnings
 from mkdocs_git_authors_plugin.exclude import exclude
 
 logger = logging.getLogger("mkdocs.plugins")
 
+
 class GitAuthorsPlugin(BasePlugin):
     config_scheme = (
         ("show_contribution", config_options.Type(bool, default=False)),
         ("show_line_count", config_options.Type(bool, default=False)),
         ("show_email_address", config_options.Type(bool, default=True)),
         ("count_empty_lines", config_options.Type(bool, default=True)),
         ("fallback_to_empty", config_options.Type(bool, default=False)),
@@ -45,25 +46,25 @@
 
         Args:
             config: global configuration object
 
         Returns:
             (updated) configuration object
         """
-        if not self.config.get('enabled'):
+        if not self.config.get("enabled"):
             return config
-        
-        assert self.config['authorship_threshold_percent'] >= 0
-        assert self.config['authorship_threshold_percent'] <= 100
+
+        assert self.config["authorship_threshold_percent"] >= 0
+        assert self.config["authorship_threshold_percent"] <= 100
 
         try:
             self._repo = Repo()
             self._fallback = False
             self.repo().set_config(self.config)
-            raise_ci_warnings(path = self.repo()._root)
+            raise_ci_warnings(path=self.repo()._root)
         except GitCommandError:
             if self.config["fallback_to_empty"]:
                 self._fallback = True
                 logger.warning(
                     "[git-authors-plugin] Unable to find a git directory and/or git is not installed."
                     " Option 'fallback_to_empty' set to 'true': Falling back to empty authors list"
                 )
@@ -93,26 +94,26 @@
         Args:
             files: global files collection
             config: global configuration object
 
         Returns:
             global files collection
         """
-        if not self.config.get('enabled'):
+        if not self.config.get("enabled"):
             return
         if self._fallback:
             return
-        
+
         for file in files:
 
             # Exclude pages specified in config
             excluded_pages = self.config.get("exclude", [])
             if exclude(file.src_path, excluded_pages):
                 continue
-            
+
             path = file.abs_src_path
             if path.endswith(".md"):
                 _ = self.repo().page(path)
 
     def on_page_content(self, html, page, config, files, **kwargs):
         """
         Replace jinja tag {{ git_site_authors }} in HTML.
@@ -132,30 +133,32 @@
             page: mkdocs.nav.Page instance
             config: global configuration object
             site_navigation: global navigation object
 
         Returns:
             str: HTML text of page as string
         """
-        if not self.config.get('enabled'):
+        if not self.config.get("enabled"):
             return html
-        
+
         # Exclude pages specified in config
         excluded_pages = self.config.get("exclude", [])
         if exclude(page.file.src_path, excluded_pages):
             return html
 
         # Replace {{ git_site_authors }}
         list_pattern = re.compile(
             r"\{\{\s*git_site_authors\s*\}\}", flags=re.IGNORECASE
         )
         if list_pattern.search(html):
             html = list_pattern.sub(
-                "" if self._fallback else
-                util.site_authors_summary(self.repo().get_authors(), self.config), html
+                ""
+                if self._fallback
+                else util.site_authors_summary(self.repo().get_authors(), self.config),
+                html,
             )
 
         # Replace {{ git_page_authors }}
         if self._fallback:
             page_authors = ""
         else:
             page_obj = self.repo().page(page.file.abs_src_path)
@@ -187,15 +190,15 @@
             page (class): mkdocs.nav.Page instance
             config: global configuration object
             nav: global navigation object
 
         Returns:
             dict: template context variables
         """
-        if not self.config.get('enabled'):
+        if not self.config.get("enabled"):
             return context
         if self._fallback:
             return context
 
         # Exclude pages specified in config
         excluded_pages = self.config.get("exclude", [])
         if exclude(page.file.src_path, excluded_pages):
```

### Comparing `mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin/util.py` & `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,19 +35,19 @@
     """
     return dt.strftime("%c %z")
 
 
 def page_authors_summary(page, config: dict):
     """
     A summary of the authors' contributions on a page level
-    
+
     Args:
         page (Page): Page class
         config (dict): plugin's config dict
-    
+
     Returns:
         str: HTML text with authors
     """
 
     authors = page.get_authors()
     authors_summary = []
     author_name = ""
@@ -60,16 +60,16 @@
         )
         if page.repo().config("show_email_address"):
             author_name = "<a href='mailto:%s'>%s</a>" % (author.email(), author.name())
         else:
             author_name = author.name()
         authors_summary.append("%s%s" % (author_name, contrib))
 
-    authors_summary = ", ".join(authors_summary)
-    return "<span class='git-page-authors git-authors'>%s</span>" % authors_summary
+    authors_summary_str = ", ".join(authors_summary)
+    return "<span class='git-page-authors git-authors'>%s</span>" % authors_summary_str
 
 
 def site_authors_summary(authors, config: dict):
     """
     A summary list of the authors' contributions on repo level.
 
     Iterates over all authors and produces an HTML <ul> list with
@@ -120,15 +120,15 @@
 </ul>
     """
     return result
 
 
 def page_authors(authors, path):
     """List of dicts with info on page authors
-    # TODO: rename to something more representative like 'authors_to_dict()' 
+    # TODO: rename to something more representative like 'authors_to_dict()'
     Args:
         authors (list): list with Author classes
         path (str): path to page
     """
     if type(path) == str:
         path = Path(path)
     return [
```

### Comparing `mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin.egg-info/PKG-INFO` & `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-git-authors-plugin
-Version: 0.7.0
+Version: 0.7.1
 Summary: Mkdocs plugin to display git authors of a page
 Home-page: https://github.com/timvink/mkdocs-git-authors-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs git contributors committers authors plugin
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Documentation
 Classifier: Topic :: Text Processing
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Actions Status](https://github.com/timvink/mkdocs-git-authors-plugin/workflows/pytest/badge.svg)](https://github.com/timvink/mkdocs-git-authors-plugin/actions)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-git-authors-plugin)
 ![PyPI](https://img.shields.io/pypi/v/mkdocs-git-authors-plugin)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mkdocs-git-authors-plugin)
```

### Comparing `mkdocs-git-authors-plugin-0.7.0/mkdocs_git_authors_plugin.egg-info/SOURCES.txt` & `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.7.0/setup.py` & `mkdocs-git-authors-plugin-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mkdocs-git-authors-plugin",
-    version="0.7.0",
+    version="0.7.1",
     description="Mkdocs plugin to display git authors of a page",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs git contributors committers authors plugin",
     url="https://github.com/timvink/mkdocs-git-authors-plugin",
     author="Tim Vink",
     author_email="vinktim@gmail.com",
     license="MIT",
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     classifiers=[
         "Operating System :: OS Independent",
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

