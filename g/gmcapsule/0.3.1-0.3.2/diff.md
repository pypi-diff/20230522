# Comparing `tmp/gmcapsule-0.3.1.tar.gz` & `tmp/gmcapsule-0.3.2.tar.gz`

## Comparing `gmcapsule-0.3.1.tar` & `gmcapsule-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 gmcapsule-0.3.1/example.ini
--rw-r--r--   0        0        0    22960 2020-02-02 00:00:00.000000 gmcapsule-0.3.1/gmcapsule/__init__.py
--rw-r--r--   0        0        0    24276 2020-02-02 00:00:00.000000 gmcapsule-0.3.1/gmcapsule/gemini.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 gmcapsule-0.3.1/gmcapsule/markdown.py
--rwxr-xr-x   0        0        0    18475 2020-02-02 00:00:00.000000 gmcapsule-0.3.1/gmcapsule/modules/80_gitview.py
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 gmcapsule-0.3.1/gmcapsule/modules/90_cgi.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 gmcapsule-0.3.1/gmcapsule/modules/99_static.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 gmcapsule-0.3.1/.gitignore
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 gmcapsule-0.3.1/README.md
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gmcapsule-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 gmcapsule-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/example.ini
+-rw-r--r--   0        0        0    22960 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/gmcapsule/__init__.py
+-rw-r--r--   0        0        0    24276 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/gmcapsule/gemini.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/gmcapsule/markdown.py
+-rwxr-xr-x   0        0        0    18589 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/gmcapsule/modules/80_gitview.py
+-rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/gmcapsule/modules/90_cgi.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/gmcapsule/modules/99_static.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/.gitignore
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/README.md
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/PKG-INFO
```

### Comparing `gmcapsule-0.3.1/example.ini` & `gmcapsule-0.3.2/example.ini`

 * *Files 20% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 
 [cgi.printenv]
 path            = /cgienv
 command         = printenv
 
 ;--------------------------------------------------------------------------
 
-;[gitview]
-;git             = /usr/bin/git
-;cache_path      = /Users/jaakko/Library/Caches/gmgitview
+[gitview]
+git             = /usr/bin/git
+cache_path      = /Users/jaakko/Library/Caches/gmgitview
 
 [gitview.lagrange]
 title           = Lagrange
 brief           = A Beautiful Gemini Client
 clone_url       = https://git.skyjake.fi/gemini/lagrange.git
 tag_url         = https://git.skyjake.fi/gemini/lagrange/releases/tag/{tag}
 path            = /Users/jaakko/src/lagrange
@@ -43,7 +43,16 @@
 [gitview.gitview]
 title           = GmGitView
 brief           = Git Repository Viewer for Gemini
 clone_url       = https://git.skyjake.fi/gemini/gitview.git
 path            = /Users/jaakko/src/gmgitview
 url_root        = gmgitview
 default_branch  = main
+
+[gitview.bubble]
+title = Bubble
+brief = Bulletin Boards for Gemini
+clone_url = https://git.skyjake.fi/gemini/bubble.git
+path = /Users/jaakko/src/bubble
+url_root = bubble
+default_branch = main
+
```

### Comparing `gmcapsule-0.3.1/gmcapsule/__init__.py` & `gmcapsule-0.3.2/gmcapsule/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
 import subprocess
 from pathlib import Path
 
 from .gemini import Server, Cache
 from .markdown import to_gemtext as markdown_to_gemtext
 
 
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 __all__ = [
     'Config', 'Capsule', 'Cache',
     'get_mime_type', 'markdown_to_gemtext'
 ]
 
 
 class Config:
```

### Comparing `gmcapsule-0.3.1/gmcapsule/gemini.py` & `gmcapsule-0.3.2/gmcapsule/gemini.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.3.1/gmcapsule/markdown.py` & `gmcapsule-0.3.2/gmcapsule/markdown.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.3.1/gmcapsule/modules/80_gitview.py` & `gmcapsule-0.3.2/gmcapsule/modules/80_gitview.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,19 @@
             out = self.git([
                 'log',
                 f'-n{count}',
                 f'--skip={skip}',
                 "--pretty=format:{^@^hash^@^:^@^%h^@^,^@^fullHash^@^:^@^%H^@^,^@^parent^@^:^@^%p^@^,^@^refs^@^:^@^%D^@^,^@^author^@^:^@^%an^@^,^@^date^@^:^@^%ad^@^,^@^email^@^:^@^%aE^@^,^@^message^@^:^@^%s^@^,^@^body^@^:^@^%b^@^,^@^commitDate^@^:^@^%ai^@^,^@^age^@^:^@^%cr^@^},^@&@^",
                 commit_hash if commit_hash else self.branch])
             out = out.replace('^@&@^\n', '').replace(',^@&@^', '') \
-                    .replace('\n', '\\n').replace('\t', '    ').replace('"', '\\"').replace('^@^', '"') \
+                    .replace('\\', '\\\\') \
+                    .replace('\n', '\\n') \
+                    .replace('\t', '    ') \
+                    .replace('"', '\\"') \
+                    .replace('^@^', '"') \
                     .replace('\\n#', '\\n') \
                     .replace('"body":"#', '"body":"')
             out = '[' + out + ']'
             #print(out)
             return json.loads(out)
         except:
             return []
```

### Comparing `gmcapsule-0.3.1/gmcapsule/modules/90_cgi.py` & `gmcapsule-0.3.2/gmcapsule/modules/90_cgi.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.3.1/gmcapsule/modules/99_static.py` & `gmcapsule-0.3.2/gmcapsule/modules/99_static.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.3.1/README.md` & `gmcapsule-0.3.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -51,14 +51,18 @@
 * Added a shutdown event for custom background workers.
 * `Request.query` is None if there is no query string present. Previously, the query string was an empty string in this case. This allows making a distinction between empty and absent query strings.
 
 v0.3.1:
 
 * CGI: Fixed handling of a missing query string.
 
+v0.3.2:
+
+* GitView: Fixed processing of Git commit history when a message contains backslashes.
+
 ### v0.2
 
 * Added `[cgi] bin_root` configuration option for automatically and dynamically mapping all executables in a directory tree to URL entry points.
 * Minor documentation updates.
 * Published on PyPi as "gmcapsule".
 
 v0.2.1:
```

### Comparing `gmcapsule-0.3.1/pyproject.toml` & `gmcapsule-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.3.1/PKG-INFO` & `gmcapsule-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmcapsule
-Version: 0.3.1
+Version: 0.3.2
 Summary: Extensible Gemini/Titan server
 Project-URL: Home-page, https://geminispace.org/gmcapsule/
 Project-URL: Documentation, https://geminispace.org/gmcapsule/gmcapsule.html
 Project-URL: Source, https://codeberg.org/skyjake/gmcapsule
 Project-URL: Issues, https://codeberg.org/skyjake/gmcapsule/issues
 Author-email: Jaakko Keränen <jaakko.keranen@iki.fi>
 Keywords: gemini,internet,server,titan
@@ -73,14 +73,18 @@
 * Added a shutdown event for custom background workers.
 * `Request.query` is None if there is no query string present. Previously, the query string was an empty string in this case. This allows making a distinction between empty and absent query strings.
 
 v0.3.1:
 
 * CGI: Fixed handling of a missing query string.
 
+v0.3.2:
+
+* GitView: Fixed processing of Git commit history when a message contains backslashes.
+
 ### v0.2
 
 * Added `[cgi] bin_root` configuration option for automatically and dynamically mapping all executables in a directory tree to URL entry points.
 * Minor documentation updates.
 * Published on PyPi as "gmcapsule".
 
 v0.2.1:
```

