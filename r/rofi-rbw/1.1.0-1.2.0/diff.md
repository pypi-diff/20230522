# Comparing `tmp/rofi_rbw-1.1.0.tar.gz` & `tmp/rofi_rbw-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rofi_rbw-1.1.0.tar", max compression
+gzip compressed data, was "rofi_rbw-1.2.0.tar", max compression
```

## Comparing `rofi_rbw-1.1.0.tar` & `rofi_rbw-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,17 @@
--rw-r--r--   0        0        0     1075 2023-01-03 08:16:30.965044 rofi_rbw-1.1.0/LICENSE
--rw-r--r--   0        0        0     7074 2023-01-03 08:18:12.464845 rofi_rbw-1.1.0/README.md
--rw-r--r--   0        0        0      713 2023-01-03 08:23:47.379598 rofi_rbw-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      206 2022-12-22 13:31:28.675750 rofi_rbw-1.1.0/src/rofi_rbw/__init__.py
--rw-r--r--   0        0        0      105 2022-12-22 13:31:28.675750 rofi_rbw-1.1.0/src/rofi_rbw/__main__.py
--rw-r--r--   0        0        0      197 2022-12-22 13:31:28.675750 rofi_rbw-1.1.0/src/rofi_rbw/abstractionhelper.py
--rw-r--r--   0        0        0     3586 2022-12-22 13:31:28.675750 rofi_rbw-1.1.0/src/rofi_rbw/clipboarder.py
--rw-r--r--   0        0        0     1198 2022-12-22 13:31:28.675750 rofi_rbw-1.1.0/src/rofi_rbw/credentials.py
--rw-r--r--   0        0        0     4168 2023-01-03 08:26:47.361965 rofi_rbw-1.1.0/src/rofi_rbw/docs/rofi-rbw.1
--rw-r--r--   0        0        0     3428 2023-01-03 08:26:46.625301 rofi_rbw-1.1.0/src/rofi_rbw/docs/rofi-rbw.1.md
--rw-r--r--   0        0        0      186 2023-01-03 08:18:12.464845 rofi_rbw-1.1.0/src/rofi_rbw/entry.py
--rw-r--r--   0        0        0     1233 2022-12-22 13:31:28.675750 rofi_rbw-1.1.0/src/rofi_rbw/models.py
--rw-r--r--   0        0        0      457 2022-12-22 13:31:28.675750 rofi_rbw-1.1.0/src/rofi_rbw/paths.py
--rw-r--r--   0        0        0     2325 2023-01-03 08:18:12.464845 rofi_rbw-1.1.0/src/rofi_rbw/rbw.py
--rwxr-xr-x   0        0        0     8260 2023-01-03 08:27:35.101739 rofi_rbw-1.1.0/src/rofi_rbw/rofi_rbw.py
--rw-r--r--   0        0        0     9835 2023-01-03 08:18:12.464845 rofi_rbw-1.1.0/src/rofi_rbw/selector.py
--rw-r--r--   0        0        0     2696 2022-12-22 13:31:28.675750 rofi_rbw-1.1.0/src/rofi_rbw/typer.py
--rw-r--r--   0        0        0     7996 1970-01-01 00:00:00.000000 rofi_rbw-1.1.0/setup.py
--rw-r--r--   0        0        0     7765 1970-01-01 00:00:00.000000 rofi_rbw-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-01-03 08:16:30.965044 rofi_rbw-1.2.0/LICENSE
+-rw-r--r--   0        0        0     7084 2023-02-15 20:30:16.093877 rofi_rbw-1.2.0/README.md
+-rw-r--r--   0        0        0     4180 2023-05-22 15:59:25.002029 rofi_rbw-1.2.0/docs/rofi-rbw.1
+-rw-r--r--   0        0        0      749 2023-05-22 15:59:25.002029 rofi_rbw-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      206 2022-12-22 13:31:28.675750 rofi_rbw-1.2.0/src/rofi_rbw/__init__.py
+-rw-r--r--   0        0        0      105 2022-12-22 13:31:28.675750 rofi_rbw-1.2.0/src/rofi_rbw/__main__.py
+-rw-r--r--   0        0        0      197 2022-12-22 13:31:28.675750 rofi_rbw-1.2.0/src/rofi_rbw/abstractionhelper.py
+-rw-r--r--   0        0        0     3586 2022-12-22 13:31:28.675750 rofi_rbw-1.2.0/src/rofi_rbw/clipboarder.py
+-rw-r--r--   0        0        0     1198 2022-12-22 13:31:28.675750 rofi_rbw-1.2.0/src/rofi_rbw/credentials.py
+-rw-r--r--   0        0        0      186 2023-01-03 08:18:12.464845 rofi_rbw-1.2.0/src/rofi_rbw/entry.py
+-rw-r--r--   0        0        0     1233 2022-12-22 13:31:28.675750 rofi_rbw-1.2.0/src/rofi_rbw/models.py
+-rw-r--r--   0        0        0      457 2022-12-22 13:31:28.675750 rofi_rbw-1.2.0/src/rofi_rbw/paths.py
+-rw-r--r--   0        0        0     2432 2023-05-22 15:58:58.192103 rofi_rbw-1.2.0/src/rofi_rbw/rbw.py
+-rwxr-xr-x   0        0        0     8270 2023-02-15 20:30:16.093877 rofi_rbw-1.2.0/src/rofi_rbw/rofi_rbw.py
+-rw-r--r--   0        0        0     9835 2023-01-03 08:18:12.464845 rofi_rbw-1.2.0/src/rofi_rbw/selector.py
+-rw-r--r--   0        0        0     3098 2023-05-22 15:58:58.192103 rofi_rbw-1.2.0/src/rofi_rbw/typer.py
+-rw-r--r--   0        0        0     7775 1970-01-01 00:00:00.000000 rofi_rbw-1.2.0/PKG-INFO
```

### Comparing `rofi_rbw-1.1.0/LICENSE` & `rofi_rbw-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.1.0/README.md` & `rofi_rbw-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 |----------------------|--------------|------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `--action`           | `-a`         | `type` (default), `copy`, `print`                    | Choose what `rofi-rbw` should do.                                                                                                                                                                                                                                           |
 | `--target`           | `-t`         | `username`, `password`, `totp` (or any custom field) | Choose which components of the selected entry are interesting. Can be passed multiple times to type/copy/print several components. Default is `username` and `password`.                                                                                                    |
 | `--prompt`           | `-r`         | any string                                           | Define the text of the prompt.                                                                                                                                                                                                                                              |
 | `--selector-args`    |              |                                                      | Define arguments that will be passed through to `rofi` or `wofi`.<br/>Please note that you need to specify it as `--selector-args="<args>"` or `--selector-args " <args>"` because of a [bug in argparse](https://github.com/python/cpython/issues/53580)                   |
 | `--selector`         |              | `rofi`, `wofi`                                       | Show the selection dialog with this application. Chosen automatically by default.                                                                                                                                                                                           |
 | `--clipboarder`      |              | `xsel`, `xclip`, `wl-copy`                           | Access the clipboard with this application. Chosen automatically by default.                                                                                                                                                                                                |
-| `--typer`            |              | `xdotool`, `wtype`, `ydotool`                        | Type the characters using this application. Chosen automatically by default.                                                                                                                                                                                                |
+| `--typer`            |              | `xdotool`, `wtype`, `ydotool`, `dotool`              | Type the characters using this application. Chosen automatically by default.                                                                                                                                                                                                |
 | `--clear-after`      |              | integer number >= 0 (default is `0`)                 | Limit the duration in seconds passwords stay in your clipboard (unless overwritten). When set to 0, passwords will be kept indefinitely.                                                                                                                                    |
 | `--no-help`          |              |                                                      | Don't show the help message about the available shortcuts.                                                                                                                                                                                                                  |
 | `--no-folder`        |              |                                                      | Don't show the entry's folder in the list.                                                                                                                                                                                                                                  |
 | `--keybindings`      |              |                                                      | Define custom keybindings in the format `<shortcut>:<action>:<target>`, for example `Alt+n:copy:username`. Multiple keybindings can be concatenated with `,`; multiple targets for one shortcut can be concatenated with `:`. Note that `wofi` doesn't support keybindings. |
 | `--menu-keybindings` |              |                                                      | Define custom keybindings for the target menu in the format `<shortcut>:<action>`, similar to `--keybindings`. Note that `wofi` doesn't support keybindings.                                                                                                                |
 
 # Installation
@@ -45,9 +45,9 @@
 Download the wheel file from releases and install it with  `sudo pip install $filename` (or you can use `pip install --user $filename` to only install it for the local user).
 Note that it needs `configargparse` to work.
 
 ## Dependencies
 You also need:
 - Python 3.7 or higher
 - `rofi` or `wofi`
-- Something to programmatically type characters into other applications. Depending on your display server, it's `xdotool`, `wtype` or `ydotool`.
+- Something to programmatically type characters into other applications. Depending on your display server, it's `xdotool`, `wtype`, `ydotool` or `dotool`.
 - Something to copy text to the clipboard. Again, depending on the display server, you want `xclip`, `xsel` or `wl-copy`.
```

### Comparing `rofi_rbw-1.1.0/pyproject.toml` & `rofi_rbw-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 [tool.poetry]
 name = "rofi-rbw"
-version = "1.1.0"
+version = "1.2.0"
 description = "Rofi frontend for Bitwarden"
 authors = ["Fabian Winter <5821180+fdw@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fdw/rofi-rbw"
 repository = "https://github.com/fdw/rofi-rbw"
 packages =[
     { include = "rofi_rbw", from = "src" }
 ]
+include = [
+    "docs/rofi-rbw.1"
+]
 
 [tool.poetry.scripts]
 rofi-rbw = 'rofi_rbw.__main__:main'
 
 [tool.poetry.dependencies]
 python = "^3.8"
 ConfigArgParse = ">0.15,<2.0.0"
```

### Comparing `rofi_rbw-1.1.0/src/rofi_rbw/clipboarder.py` & `rofi_rbw-1.2.0/src/rofi_rbw/clipboarder.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.1.0/src/rofi_rbw/credentials.py` & `rofi_rbw-1.2.0/src/rofi_rbw/credentials.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.1.0/src/rofi_rbw/docs/rofi-rbw.1` & `rofi_rbw-1.2.0/docs/rofi-rbw.1`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.\" Automatically generated by Pandoc 2.19.2
+.\" Automatically generated by Pandoc 3.1.2
 .\"
 .\" Define V font for inline verbatim, using C font in formats
 .\" that render this, and otherwise B font.
 .ie "\f[CB]x\f[]"x" \{\
 . ftr V B
 . ftr VI BI
 . ftr VB B
@@ -10,15 +10,15 @@
 .\}
 .el \{\
 . ftr V CR
 . ftr VI CI
 . ftr VB CB
 . ftr VBI CBI
 .\}
-.TH "ROFI-RBW" "1" "January 03, 2023" "Version 1.1.0" "Rofi Third-party Add-on Documentation"
+.TH "ROFI-RBW" "1" "May 13, 2023" "Version 1.2.0" "Rofi Third-party Add-on Documentation"
 .hy
 .SH NAME
 .PP
 \f[B]rofi-rbw\f[R] - A rofi frontend for the alternative Bitwarden
 client rbw
 .SH SYNOPSIS
 .PP
@@ -71,15 +71,15 @@
 Possible values: xsel, xclip, wl-copy
 .RS
 .PP
 Choose the application to access the clipboard with manually.
 .RE
 .TP
 --typer \f[I]TYPER\f[R]
-Possible values: xdotool, wtype
+Possible values: xdotool, wtype, ydotool, dotool
 .RS
 .PP
 Choose the application to type with manually.
 .RE
 .TP
 --selector \f[I]SELECTOR\f[R]
 Possible values: rofi, wofi
```

### Comparing `rofi_rbw-1.1.0/src/rofi_rbw/models.py` & `rofi_rbw-1.2.0/src/rofi_rbw/models.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.1.0/src/rofi_rbw/rbw.py` & `rofi_rbw-1.2.0/src/rofi_rbw/rbw.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import json
+from json import JSONDecodeError
 from subprocess import run
 from typing import List, Optional
 
 from .credentials import Credentials
 from .entry import Entry
 
 
 class Rbw:
     def list_entries(self) -> List[Entry]:
-        rbw = run(["rbw", "ls", "--fields", "folder,name,user"], encoding="utf-8", capture_output=True)
+        rbw = run(["rbw", "list", "--fields", "folder,name,user"], encoding="utf-8", capture_output=True)
 
         if rbw.returncode != 0:
             print("There was a problem calling rbw. Is it correctly configured?")
             print(rbw.stderr)
             exit(2)
 
         return sorted(
@@ -24,43 +26,42 @@
 
         try:
             return Entry(fields[1], fields[0], fields[2] if len(fields) > 2 else "")
         except IndexError:
             raise Exception("Entry is incorrectly formatted and cannot be parsed")
 
     def fetch_credentials(self, entry: Entry) -> "Credentials":
-        password = ""
-        has_totp = False
-        uris = []
-        further = {}
-
-        line, *rest = self.__load_from_rbw(entry.name, entry.username, entry.folder).strip().split("\n")
-        if len(line.split(": ", 1)) == 2:
-            # First line contains ': ' and thus there is no password
-            rest = [line] + rest
-        else:
-            password = line
-
-        for line in rest:
-            try:
-                key, value = line.split(": ", 1)
-                if key == "URI":
-                    uris.append(value)
-                elif key == "TOTP Secret":
-                    has_totp = True
-                elif key == "Match type" or key == "username":
-                    pass
-                else:
-                    further[key] = value
-            except ValueError:
-                pass
-        return Credentials(entry.name, entry.folder, entry.username, password, has_totp, uris, further)
+        try:
+            data = json.loads(self.__load_from_rbw(entry.name, entry.username, entry.folder).strip())
+
+            if data["data"] is None or "password" not in data["data"]:
+                print('rofi-rbw only supports logins')
+                return Credentials(
+                    entry.name,
+                    entry.folder,
+                    entry.username,
+                    further={item["name"]: item["value"] for item in data["fields"]},
+                )
+
+            return Credentials(
+                entry.name,
+                entry.folder,
+                entry.username,
+                data["data"]["password"] or "",
+                data["data"]["totp"] is not None,
+                [item["uri"] for item in data["data"]["uris"]],
+                {item["name"]: item["value"] for item in data["fields"]},
+            )
+
+        except JSONDecodeError as exception:
+            print(f"Could not parse the output: {exception.msg}")
+            exit(12)
 
     def __load_from_rbw(self, name: str, username: str, folder: Optional[str]) -> str:
-        command = ["rbw", "get", "--full", name]
+        command = ["rbw", "get", "--raw", name]
         if username:
             command.append(username)
 
         if folder:
             command.extend(["--folder", folder])
 
         return run(command, capture_output=True, encoding="utf-8").stdout
```

### Comparing `rofi_rbw-1.1.0/src/rofi_rbw/rofi_rbw.py` & `rofi_rbw-1.2.0/src/rofi_rbw/rofi_rbw.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             help="Choose the application to access the clipboard with",
         )
         parser.add_argument(
             "--typer",
             dest="typer",
             action="store",
             type=str,
-            choices=["xdotool", "wtype", "ydotool"],
+            choices=["xdotool", "wtype", "ydotool", "dotool"],
             default=None,
             help="Choose the application to type with",
         )
         parser.add_argument(
             "--clear-after",
             dest="clear",
             action="store",
```

### Comparing `rofi_rbw-1.1.0/src/rofi_rbw/selector.py` & `rofi_rbw-1.2.0/src/rofi_rbw/selector.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.1.0/src/rofi_rbw/typer.py` & `rofi_rbw-1.2.0/src/rofi_rbw/typer.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,10 +89,26 @@
         return "not possible with ydotool"
 
     def type_characters(self, characters: str, active_window: str) -> None:
         time.sleep(0.05)
         run(["ydotool", "type", "--key-delay", "0", characters])
 
 
+class DotoolTyper(Typer):
+    @staticmethod
+    def supported() -> bool:
+        return is_installed("dotool")
+
+    @staticmethod
+    def name() -> str:
+        return "dotool"
+
+    def get_active_window(self) -> str:
+        return "not possible with dotool"
+
+    def type_characters(self, characters: str, active_window: str) -> None:
+        run(["dotool"], text=True, input=f"type {characters}")
+
+
 class NoTyperFoundException(Exception):
     def __str__(self) -> str:
         return "Could not find a valid way to type characters. Please check the required dependencies."
```

### Comparing `rofi_rbw-1.1.0/setup.py` & `rofi_rbw-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,73 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: rofi-rbw
+Version: 1.2.0
+Summary: Rofi frontend for Bitwarden
+Home-page: https://github.com/fdw/rofi-rbw
+License: MIT
+Author: Fabian Winter
+Author-email: 5821180+fdw@users.noreply.github.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: ConfigArgParse (>0.15,<2.0.0)
+Project-URL: Repository, https://github.com/fdw/rofi-rbw
+Description-Content-Type: text/markdown
+
+# rbw-rofi
+## A rofi frontend for Bitwarden
+
+Based on the alternative [Bitwarden](https://bitwarden.com/) CLI [rbw](https://github.com/doy/rbw/) and inspired by [rofi-pass](https://github.com/carnager/rofi-pass), `rbw-rofi` is a simplistic password typer/copier using [rofi](https://github.com/davatorium/rofi) and [wofi](https://hg.sr.ht/~scoopta/wofi).
+
+## Features
+- Autotype password or username (`Enter`/`Alt+3` and `Alt+2`, respectively)
+- Autotype username and password (with a `tab` character in between) with `Alt+1` (and copy TOTP to clipboard)
+- Copy username, password or TOTP to the clipboard (`Alt+u`, `Alt+p` and `Alt+t`, respectively)
+- Show an autotype menu with all fields
+
+## Usage
+First, you need to configure `rbw`. See its documentation for that.
+Then, you can start `rofi-rbw`. It is *not* available as a rofi mode.
+
+# Configuration
+You can configure `rofi-rbw` either with cli arguments or with a config file called `$XDG_CONFIG_HOME/rofi-rbw.rc`. In the file, use the long option names without double dashes.
+
+## Options
+
+| long option          | short option | possible values                                      | description                                                                                                                                                                                                                                                                 |
+|----------------------|--------------|------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `--action`           | `-a`         | `type` (default), `copy`, `print`                    | Choose what `rofi-rbw` should do.                                                                                                                                                                                                                                           |
+| `--target`           | `-t`         | `username`, `password`, `totp` (or any custom field) | Choose which components of the selected entry are interesting. Can be passed multiple times to type/copy/print several components. Default is `username` and `password`.                                                                                                    |
+| `--prompt`           | `-r`         | any string                                           | Define the text of the prompt.                                                                                                                                                                                                                                              |
+| `--selector-args`    |              |                                                      | Define arguments that will be passed through to `rofi` or `wofi`.<br/>Please note that you need to specify it as `--selector-args="<args>"` or `--selector-args " <args>"` because of a [bug in argparse](https://github.com/python/cpython/issues/53580)                   |
+| `--selector`         |              | `rofi`, `wofi`                                       | Show the selection dialog with this application. Chosen automatically by default.                                                                                                                                                                                           |
+| `--clipboarder`      |              | `xsel`, `xclip`, `wl-copy`                           | Access the clipboard with this application. Chosen automatically by default.                                                                                                                                                                                                |
+| `--typer`            |              | `xdotool`, `wtype`, `ydotool`, `dotool`              | Type the characters using this application. Chosen automatically by default.                                                                                                                                                                                                |
+| `--clear-after`      |              | integer number >= 0 (default is `0`)                 | Limit the duration in seconds passwords stay in your clipboard (unless overwritten). When set to 0, passwords will be kept indefinitely.                                                                                                                                    |
+| `--no-help`          |              |                                                      | Don't show the help message about the available shortcuts.                                                                                                                                                                                                                  |
+| `--no-folder`        |              |                                                      | Don't show the entry's folder in the list.                                                                                                                                                                                                                                  |
+| `--keybindings`      |              |                                                      | Define custom keybindings in the format `<shortcut>:<action>:<target>`, for example `Alt+n:copy:username`. Multiple keybindings can be concatenated with `,`; multiple targets for one shortcut can be concatenated with `:`. Note that `wofi` doesn't support keybindings. |
+| `--menu-keybindings` |              |                                                      | Define custom keybindings for the target menu in the format `<shortcut>:<action>`, similar to `--keybindings`. Note that `wofi` doesn't support keybindings.                                                                                                                |
+
+# Installation
+
+## From distribution repositories
+[![Packaging status](https://repology.org/badge/vertical-allrepos/rofi-rbw.svg)](https://repology.org/project/rofi-rbw/versions)
+
+## From PyPI
+`rofi-rbw` is on [PyPI](https://pypi.org/project/rofi-rbw/). You can install it with `pip install --user rofi-rbw` (or `sudo pip install rofi-rbw`).
+
+## Manually
+Download the wheel file from releases and install it with  `sudo pip install $filename` (or you can use `pip install --user $filename` to only install it for the local user).
+Note that it needs `configargparse` to work.
+
+## Dependencies
+You also need:
+- Python 3.7 or higher
+- `rofi` or `wofi`
+- Something to programmatically type characters into other applications. Depending on your display server, it's `xdotool`, `wtype`, `ydotool` or `dotool`.
+- Something to copy text to the clipboard. Again, depending on the display server, you want `xclip`, `xsel` or `wl-copy`.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['rofi_rbw']
-
-package_data = \
-{'': ['*'], 'rofi_rbw': ['docs/*']}
-
-install_requires = \
-['ConfigArgParse>0.15,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['rofi-rbw = rofi_rbw.__main__:main']}
-
-setup_kwargs = {
-    'name': 'rofi-rbw',
-    'version': '1.1.0',
-    'description': 'Rofi frontend for Bitwarden',
-    'long_description': '# rbw-rofi\n## A rofi frontend for Bitwarden\n\nBased on the alternative [Bitwarden](https://bitwarden.com/) CLI [rbw](https://github.com/doy/rbw/) and inspired by [rofi-pass](https://github.com/carnager/rofi-pass), `rbw-rofi` is a simplistic password typer/copier using [rofi](https://github.com/davatorium/rofi) and [wofi](https://hg.sr.ht/~scoopta/wofi).\n\n## Features\n- Autotype password or username (`Enter`/`Alt+3` and `Alt+2`, respectively)\n- Autotype username and password (with a `tab` character in between) with `Alt+1` (and copy TOTP to clipboard)\n- Copy username, password or TOTP to the clipboard (`Alt+u`, `Alt+p` and `Alt+t`, respectively)\n- Show an autotype menu with all fields\n\n## Usage\nFirst, you need to configure `rbw`. See its documentation for that.\nThen, you can start `rofi-rbw`. It is *not* available as a rofi mode.\n\n# Configuration\nYou can configure `rofi-rbw` either with cli arguments or with a config file called `$XDG_CONFIG_HOME/rofi-rbw.rc`. In the file, use the long option names without double dashes.\n\n## Options\n\n| long option          | short option | possible values                                      | description                                                                                                                                                                                                                                                                 |\n|----------------------|--------------|------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|\n| `--action`           | `-a`         | `type` (default), `copy`, `print`                    | Choose what `rofi-rbw` should do.                                                                                                                                                                                                                                           |\n| `--target`           | `-t`         | `username`, `password`, `totp` (or any custom field) | Choose which components of the selected entry are interesting. Can be passed multiple times to type/copy/print several components. Default is `username` and `password`.                                                                                                    |\n| `--prompt`           | `-r`         | any string                                           | Define the text of the prompt.                                                                                                                                                                                                                                              |\n| `--selector-args`    |              |                                                      | Define arguments that will be passed through to `rofi` or `wofi`.<br/>Please note that you need to specify it as `--selector-args="<args>"` or `--selector-args " <args>"` because of a [bug in argparse](https://github.com/python/cpython/issues/53580)                   |\n| `--selector`         |              | `rofi`, `wofi`                                       | Show the selection dialog with this application. Chosen automatically by default.                                                                                                                                                                                           |\n| `--clipboarder`      |              | `xsel`, `xclip`, `wl-copy`                           | Access the clipboard with this application. Chosen automatically by default.                                                                                                                                                                                                |\n| `--typer`            |              | `xdotool`, `wtype`, `ydotool`                        | Type the characters using this application. Chosen automatically by default.                                                                                                                                                                                                |\n| `--clear-after`      |              | integer number >= 0 (default is `0`)                 | Limit the duration in seconds passwords stay in your clipboard (unless overwritten). When set to 0, passwords will be kept indefinitely.                                                                                                                                    |\n| `--no-help`          |              |                                                      | Don\'t show the help message about the available shortcuts.                                                                                                                                                                                                                  |\n| `--no-folder`        |              |                                                      | Don\'t show the entry\'s folder in the list.                                                                                                                                                                                                                                  |\n| `--keybindings`      |              |                                                      | Define custom keybindings in the format `<shortcut>:<action>:<target>`, for example `Alt+n:copy:username`. Multiple keybindings can be concatenated with `,`; multiple targets for one shortcut can be concatenated with `:`. Note that `wofi` doesn\'t support keybindings. |\n| `--menu-keybindings` |              |                                                      | Define custom keybindings for the target menu in the format `<shortcut>:<action>`, similar to `--keybindings`. Note that `wofi` doesn\'t support keybindings.                                                                                                                |\n\n# Installation\n\n## From distribution repositories\n[![Packaging status](https://repology.org/badge/vertical-allrepos/rofi-rbw.svg)](https://repology.org/project/rofi-rbw/versions)\n\n## From PyPI\n`rofi-rbw` is on [PyPI](https://pypi.org/project/rofi-rbw/). You can install it with `pip install --user rofi-rbw` (or `sudo pip install rofi-rbw`).\n\n## Manually\nDownload the wheel file from releases and install it with  `sudo pip install $filename` (or you can use `pip install --user $filename` to only install it for the local user).\nNote that it needs `configargparse` to work.\n\n## Dependencies\nYou also need:\n- Python 3.7 or higher\n- `rofi` or `wofi`\n- Something to programmatically type characters into other applications. Depending on your display server, it\'s `xdotool`, `wtype` or `ydotool`.\n- Something to copy text to the clipboard. Again, depending on the display server, you want `xclip`, `xsel` or `wl-copy`.\n',
-    'author': 'Fabian Winter',
-    'author_email': '5821180+fdw@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/fdw/rofi-rbw',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

