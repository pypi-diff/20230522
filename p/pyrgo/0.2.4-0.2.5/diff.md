# Comparing `tmp/pyrgo-0.2.4.tar.gz` & `tmp/pyrgo-0.2.5.tar.gz`

## Comparing `pyrgo-0.2.4.tar` & `pyrgo-0.2.5.tar`

### file list

```diff
@@ -1,60 +1,76 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pyrgo-0.2.4/.tool-versions
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrgo-0.2.4/Makefile
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyrgo-0.2.4/mkdocs.yml
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 pyrgo-0.2.4/.github/workflows/release.yml
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyrgo-0.2.4/.github/workflows/test.yml
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pyrgo-0.2.4/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/__main__.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/cli.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/__init__.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/add.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/build.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/check.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/clean.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/fmt.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/init.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/lock.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/new.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/remove.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/sync.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/test.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/venv.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/docs/__init__.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/docs/build.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/docs/new.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/docs/root.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/cli/commands/docs/serve.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/contants.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/models/__init__.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/models/pyproject.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/ops/__init__.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/ops/add.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/ops/build.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/ops/check.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/ops/clean.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/ops/fmt.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/ops/lock.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/ops/sync.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/ops/test.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/ops/venv.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/ops/docs/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/ops/docs/build.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/ops/docs/new.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/ops/docs/serve.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/utilities/__init__.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/utilities/command.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyrgo/core/utilities/text.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrgo-0.2.4/requirements/core.lock
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pyrgo-0.2.4/scripts/new_release.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pyrgo-0.2.4/tests/unit/utilities/test_text.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pyrgo-0.2.4/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrgo-0.2.4/LICENSE
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 pyrgo-0.2.4/README.md
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 pyrgo-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 pyrgo-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pyrgo-0.2.5/.tool-versions
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrgo-0.2.5/Makefile
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyrgo-0.2.5/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pyrgo-0.2.5/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 pyrgo-0.2.5/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pyrgo-0.2.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pyrgo-0.2.5/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pyrgo-0.2.5/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/__init__.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/constants.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/__main__.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/__init__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/add.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/audit.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/build.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/check.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/clean.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/fmt.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/lock.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/remove.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/sync.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/test.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/venv.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/docs/__init__.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/docs/build.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/docs/new.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/docs/root.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/docs/serve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_new/__init__.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_new/__main__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_new/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/constants.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/models/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/models/command.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/models/config.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/__init__.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/audit.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/build.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/check.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/clean.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/fmt.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/lock.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/sync.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/test.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/venv.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/docs/__init__.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/docs/build.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/docs/new.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/docs/serve.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/resources/README.md
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/resources/__init__.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/resources/starter-project.zip
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/utilities/__init__.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/utilities/command.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/utilities/io.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/utilities/text.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 pyrgo-0.2.5/requirements/core.txt
+-rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 pyrgo-0.2.5/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pyrgo-0.2.5/scripts/new_release.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pyrgo-0.2.5/tests/test_errors.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 pyrgo-0.2.5/tests/models/test_command.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pyrgo-0.2.5/tests/utilities/test_command.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 pyrgo-0.2.5/tests/utilities/test_text.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pyrgo-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrgo-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 pyrgo-0.2.5/README.md
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 pyrgo-0.2.5/PKG-INFO
```

### Comparing `pyrgo-0.2.4/Makefile` & `pyrgo-0.2.5/Makefile`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.4/.github/workflows/release.yml` & `pyrgo-0.2.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.4/.github/workflows/test.yml` & `pyrgo-0.2.5/.github/workflows/test.yml`

 * *Files 17% similar despite different names*

```diff
@@ -29,14 +29,17 @@
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: "pip"
           cache-dependency-path: pyproject.toml
 
       - name: Install deps
-        run: pip install -U pip && pip install -e ".[dev]"
+        run: |
+          pip install -U pip
+          pip install -r requirements/dev.txt
+          pip install --no-deps -e .
 
       - name: Check code
         run: pyrgo check
 
       - name: Test code
         run: pyrgo test
```

### Comparing `pyrgo-0.2.4/pyrgo/cli/commands/check.py` & `pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/check.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """check command."""
+from __future__ import annotations
 
-
-import pathlib
 import sys
 
 import click
 from result import Ok
 
 from pyrgo.core import ops
+from pyrgo.core.constants import app_config
 
 
 @click.command()
 @click.option(
     "--add-noqa",
     "add_noqa",
     is_flag=True,
@@ -26,16 +26,14 @@
     default=False,
     type=bool,
     help="Ignore any `# noqa` comments",
 )
 def check(*, add_noqa: bool, ignore_noqa: bool) -> None:
     """Analyze the current package with `ruff` and `mypy`."""
     executed = ops.check.execute(
-        cwd=pathlib.Path().cwd(),
         add_noqa=add_noqa,
         ignore_noqa=ignore_noqa,
+        app_config=app_config,
     )
     if not isinstance(executed, Ok):
-        click.echo(message=executed.err())
         sys.exit(1)
-
     sys.exit(0)
```

### Comparing `pyrgo-0.2.4/pyrgo/cli/commands/test.py` & `pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,35 @@
 """test command."""
+from __future__ import annotations
 
-import pathlib
 import sys
-from typing import List, Optional
 
 import click
 from result import Ok
 
 from pyrgo.core import ops
-from pyrgo.core.models.pyproject import Pyproject
-
-
-def dynamic_marker_choices() -> List[str]:
-    """Dynamic markers for options."""
-    pyproject = Pyproject(cwd=pathlib.Path().cwd())
-    pyproject.read_pyproject_toml()
-    return pyproject.list_pytest_markers()
+from pyrgo.core.constants import app_config
 
 
 @click.command()
 @click.option(
     "-m",
     "--marked",
     "marker",
     type=click.Choice(
-        choices=dynamic_marker_choices(),
+        choices=app_config.pytest_makers,
     ),
     default=None,
     help="Run tests based on marks. By default all tests are executed.",
 )
 def test(
     *,
-    marker: Optional[str],
+    marker: str | None,
 ) -> None:
     """Execute tests using `pytest`."""
-    executed = ops.test.execute(marker=marker)
-
+    executed = ops.test.execute(
+        marker=marker,
+        app_config=app_config,
+    )
     if not isinstance(executed, Ok):
-        click.echo(message=executed.err())
         sys.exit(1)
-
     sys.exit(0)
```

### Comparing `pyrgo-0.2.4/pyrgo/cli/commands/docs/build.py` & `pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/docs/build.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """docs build documentation."""
+from __future__ import annotations
+
 import sys
+from typing import TYPE_CHECKING
 
-if sys.version_info >= (3, 9):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
+if TYPE_CHECKING:
+    if sys.version_info >= (3, 9):
+        from typing import Literal
+    else:
+        from typing_extensions import Literal
 
 import click
 from result import Ok
 
 from pyrgo.core import ops
 
 
@@ -35,13 +39,15 @@
         "material",
         "mkdocs",
         "readthedocs",
     ],
     strict: bool,
 ) -> None:
     """Build project documentation."""
-    executed = ops.docs.build.execute(theme=theme, strict=strict)
+    executed = ops.docs.build.execute(
+        theme=theme,
+        strict=strict,
+    )
     if not isinstance(executed, Ok):
-        click.echo(message=executed.err())
         sys.exit(1)
 
     sys.exit(0)
```

### Comparing `pyrgo-0.2.4/pyrgo/cli/commands/docs/serve.py` & `pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/docs/serve.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """docs serve command."""
+from __future__ import annotations
+
 import sys
+from typing import TYPE_CHECKING
 
 from result import Ok
 
-if sys.version_info >= (3, 9):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
+if TYPE_CHECKING:
+    if sys.version_info >= (3, 9):
+        from typing import Literal
+    else:
+        from typing_extensions import Literal
 
 
 import click
 
 from pyrgo.core import ops
 
 
@@ -53,11 +57,10 @@
     """Serve project documentation."""
     executed = ops.docs.serve.execute(
         dev_address=dev_addr,
         theme=theme,
         strict=strict,
     )
     if not isinstance(executed, Ok):
-        click.echo(message=executed.err())
         sys.exit(1)
 
     sys.exit(0)
```

### Comparing `pyrgo-0.2.4/requirements/core.lock` & `pyrgo-0.2.5/requirements/core.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,125 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
-#    pip-compile --output-file=requirements/core.lock --resolver=backtracking pyproject.toml
+#    pip-compile --output-file=requirements/core.txt --resolver=backtracking pyproject.toml
 #
 --trusted-host pypi.python.org
 --trusted-host pypi.org
 --trusted-host files.pythonhosted.org
 
 black==23.3.0
     # via pyrgo (pyproject.toml)
 build==0.10.0
     # via
     #   pip-tools
     #   pyrgo (pyproject.toml)
+cachecontrol[filecache]==0.12.11
+    # via pip-audit
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   mkdocs
     #   pip-tools
     #   pyrgo (pyproject.toml)
 colorama==0.4.6
     # via mkdocs-material
+cyclonedx-python-lib==2.7.1
+    # via pip-audit
 exceptiongroup==1.1.1
     # via pytest
 ghp-import==2.1.0
     # via mkdocs
+html5lib==1.1
+    # via pip-audit
 idna==3.4
     # via requests
+importlib-metadata==6.6.0
+    # via
+    #   build
+    #   click
+    #   cyclonedx-python-lib
+    #   markdown
+    #   mkdocs
+    #   pluggy
+    #   pytest
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via
     #   mkdocs
     #   mkdocs-material
+lockfile==0.12.2
+    # via cachecontrol
+loguru==0.7.0
+    # via pyrgo (pyproject.toml)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-material
     #   pymdown-extensions
+markdown-it-py==2.2.0
+    # via rich
 markupsafe==2.1.2
     # via jinja2
+mdurl==0.1.2
+    # via markdown-it-py
 mergedeep==1.3.4
     # via mkdocs
 mkdocs==1.4.3
     # via mkdocs-material
-mkdocs-material==9.1.12
+mkdocs-material==9.1.13
     # via pyrgo (pyproject.toml)
 mkdocs-material-extensions==1.1.1
     # via mkdocs-material
+msgpack==1.0.5
+    # via cachecontrol
 mypy==1.3.0
     # via pyrgo (pyproject.toml)
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
+packageurl-python==0.11.1
+    # via cyclonedx-python-lib
 packaging==23.1
     # via
     #   black
     #   build
     #   mkdocs
+    #   pip-audit
+    #   pip-requirements-parser
     #   pytest
 pathspec==0.11.1
     # via black
+pip-api==0.0.30
+    # via pip-audit
+pip-audit==2.5.5
+    # via pyrgo (pyproject.toml)
+pip-requirements-parser==32.0.1
+    # via pip-audit
 pip-tools==6.13.0
     # via pyrgo (pyproject.toml)
 platformdirs==3.5.1
     # via black
 pluggy==1.0.0
     # via pytest
 pygments==2.15.1
+    # via
+    #   mkdocs-material
+    #   rich
+pymdown-extensions==10.0.1
     # via mkdocs-material
-pymdown-extensions==10.0
-    # via mkdocs-material
+pyparsing==3.0.9
+    # via pip-requirements-parser
 pyproject-hooks==1.0.0
     # via build
 pytest==7.3.1
     # via pyrgo (pyproject.toml)
 python-dateutil==2.8.2
     # via ghp-import
 pyyaml==6.0
@@ -88,37 +127,63 @@
     #   mkdocs
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 regex==2023.5.5
     # via mkdocs-material
-requests==2.30.0
-    # via mkdocs-material
+requests==2.29.0
+    # via
+    #   cachecontrol
+    #   mkdocs-material
+    #   pip-audit
 result==0.10.0
     # via pyrgo (pyproject.toml)
+rich==13.3.5
+    # via pip-audit
 ruff==0.0.267
     # via pyrgo (pyproject.toml)
 six==1.16.0
-    # via python-dateutil
+    # via
+    #   html5lib
+    #   python-dateutil
+sortedcontainers==2.4.0
+    # via cyclonedx-python-lib
+toml==0.10.2
+    # via
+    #   cyclonedx-python-lib
+    #   pip-audit
 tomli==2.0.1
     # via
     #   black
     #   build
     #   mypy
     #   pyproject-hooks
-    #   pyrgo (pyproject.toml)
     #   pytest
-tomlkit==0.11.8
-    # via pyrgo (pyproject.toml)
+typed-ast==1.5.4
+    # via
+    #   black
+    #   mypy
 typing-extensions==4.5.0
-    # via mypy
-urllib3==2.0.2
+    # via
+    #   black
+    #   importlib-metadata
+    #   markdown-it-py
+    #   mkdocs
+    #   mypy
+    #   platformdirs
+    #   result
+    #   rich
+urllib3==1.26.15
     # via requests
 watchdog==3.0.0
     # via mkdocs
+webencodings==0.5.1
+    # via html5lib
 wheel==0.40.0
     # via pip-tools
+zipp==3.15.0
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `pyrgo-0.2.4/scripts/new_release.py` & `pyrgo-0.2.5/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.4/.gitignore` & `pyrgo-0.2.5/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,12 @@
 
 # Sphinx documentation
 docs/_build/
 
 # PyCharm
 .idea/
 
-# VSCode
-.vscode/
-
 # Pyenv
 .python-version
 
 # Mkdocs
 site/
```

### Comparing `pyrgo-0.2.4/LICENSE` & `pyrgo-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.4/README.md` & `pyrgo-0.2.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,20 @@
   - [black](https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html)
 - Code checking:
   - [ruff](https://beta.ruff.rs/docs/)
   - [mypy](https://mypy.readthedocs.io/en/stable/config_file.html)
 - Artifacts building:
   - [build](https://pypa-build.readthedocs.io/en/stable/)
 - Package management:
+  - [pip](https://pip.pypa.io/en/stable/)
   - [pip-tools](https://pip-tools.readthedocs.io/en/latest/)
 - Code documentation:
   - [mkdocs-material](https://squidfunk.github.io/mkdocs-material/)
+- Virtual enviroment:
+  - [venv](https://virtualenv.pypa.io/en/latest/)
 
 All behind a unified API.
 
 ```bash
 pyrgo -h
 
 # Usage: pyrgo [OPTIONS] COMMAND [ARGS]...
@@ -33,17 +36,17 @@
 #   -h, --help  Show this message and exit.
 
 # Commands:
 #   add     Add dependencies to a pyproject.toml manifest file and install.
 #   build   Build project.
 #   check   Analyze the current package with `ruff` and `mypy`.
 #   clean   Remove artifacts that pyrgo has generated in the past.
-#   docs    Document you project.
+#   docs    Document you project with `mkdocs-material`.
 #   fmt     Format all files of the current project using `black` and `ruff`.
 #   init    Create a new pyrgo project in an existing directory.
 #   lock    Lock dependencies using `piptools`.
 #   new     Create a new pyrgo project.
 #   remove  Remove dependencies from the manifest file.
 #   sync    Synchronize virtual environment with requirements.txt.
 #   test    Execute tests using `pytest`.
 #   venv    Create project virtual environment.
-```
+```
```

### Comparing `pyrgo-0.2.4/pyproject.toml` & `pyrgo-0.2.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyrgo"
-version = "0.2.4"
+version = "0.2.5"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
+authors = [
+    { name = "Tomas Perez Alvarez", email = "tomasperezalvarez@gmail.com"}
+]
 dependencies = [
     "click",
     "ruff",
     "mypy",
     "black",
     "pip-tools",
     "pytest",
     "mkdocs-material",
-    "tomli",
     "result",
     "build",
-    "tomlkit"
+    "loguru",
+    "pip-audit>=2.5.5",
 ]
 
-[[project.authors]]
-name = "Tomas Perez Alvarez"
-email = "tomasperezalvarez@gmail.com"
-
 [project.optional-dependencies]
-
+dev = [
+    "pytest-cov"
+]
 
 [project.scripts]
-pyrgo = "pyrgo.cli.__main__:cli"
+pyrgo = "pyrgo.cli.pyrgo_core.cli:root"
+pyrgo-new = "pyrgo.cli.pyrgo_new.cli:new"
 
 [project.urls]
 Documentation = "https://github.com/Tomperez98/pyrgo#readme"
 Issues = "https://github.com/Tomperez98/pyrgo/issues"
 Source = "https://github.com/Tomperez98/pyrgo"
 
 [tool.ruff]
@@ -71,39 +73,68 @@
     "node_modules",
     "venv",
 ]
 
 [tool.ruff.per-file-ignores]
 "scripts/*.py" = ["INP001"]
 "__init__.py" = ["D104"]
-"tests/*.py" = ["INP001"]
+"tests/*.py" = ["INP001", "S101"]
 
 [tool.ruff.isort]
+known-first-party = ["pyrgo"]
 force-wrap-aliases = true
 combine-as-imports = true
+required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
+[tool.ruff.flake8-quotes]
+inline-quotes = "double"
+
 
 [tool.black]
 line-length = 88
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 xfail_strict = true
 addopts = [
     "--import-mode=importlib",
+    "--strict-markers",
+    "--cov-fail-under=5",
+    "--cov-report=term-missing:skip-covered",
+    "--cov-config=pyproject.toml",
+    "--cov=pyrgo",
 ]
 markers = [
     "integration: mark integration tests.",
     "unit: mark unittest.",
 ]
 
+[tool.coverage.run]
+branch = true
+parallel = true
+omit = [
+    "pyrgo/logging.py",
+    "pyrgo/cli/**",
+    "pyrgo/**/__init__.py"
+]
+relative_files = true
+
+[tool.coverage.report]
+precision = 1
+exclude_lines = [
+    "if __name__ == .__main__.:",
+    "if TYPE_CHECKING:",
+    "@overload",
+    "raise NotImplementedError",
+]
+
 [tool.mypy]
 show_error_codes = true
 follow_imports = "normal"
 strict_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 disallow_any_generics = true
```

### Comparing `pyrgo-0.2.4/PKG-INFO` & `pyrgo-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: pyrgo
-Version: 0.2.4
+Version: 0.2.5
 Project-URL: Documentation, https://github.com/Tomperez98/pyrgo#readme
 Project-URL: Issues, https://github.com/Tomperez98/pyrgo/issues
 Project-URL: Source, https://github.com/Tomperez98/pyrgo
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Rust
 Requires-Python: >=3.7
 Requires-Dist: black
 Requires-Dist: build
 Requires-Dist: click
+Requires-Dist: loguru
 Requires-Dist: mkdocs-material
 Requires-Dist: mypy
+Requires-Dist: pip-audit>=2.5.5
 Requires-Dist: pip-tools
 Requires-Dist: pytest
 Requires-Dist: result
 Requires-Dist: ruff
-Requires-Dist: tomli
-Requires-Dist: tomlkit
+Provides-Extra: dev
+Requires-Dist: pytest-cov; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # pyrgo
 
 Python project manager inspired in [Cargo](https://doc.rust-lang.org/cargo/).
 
 `Pyrgo` does not reinvent the wheel. It's just a unified API that leverages popular libraries to improve your development experience.
@@ -36,17 +38,20 @@
   - [black](https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html)
 - Code checking:
   - [ruff](https://beta.ruff.rs/docs/)
   - [mypy](https://mypy.readthedocs.io/en/stable/config_file.html)
 - Artifacts building:
   - [build](https://pypa-build.readthedocs.io/en/stable/)
 - Package management:
+  - [pip](https://pip.pypa.io/en/stable/)
   - [pip-tools](https://pip-tools.readthedocs.io/en/latest/)
 - Code documentation:
   - [mkdocs-material](https://squidfunk.github.io/mkdocs-material/)
+- Virtual enviroment:
+  - [venv](https://virtualenv.pypa.io/en/latest/)
 
 All behind a unified API.
 
 ```bash
 pyrgo -h
 
 # Usage: pyrgo [OPTIONS] COMMAND [ARGS]...
@@ -58,17 +63,17 @@
 #   -h, --help  Show this message and exit.
 
 # Commands:
 #   add     Add dependencies to a pyproject.toml manifest file and install.
 #   build   Build project.
 #   check   Analyze the current package with `ruff` and `mypy`.
 #   clean   Remove artifacts that pyrgo has generated in the past.
-#   docs    Document you project.
+#   docs    Document you project with `mkdocs-material`.
 #   fmt     Format all files of the current project using `black` and `ruff`.
 #   init    Create a new pyrgo project in an existing directory.
 #   lock    Lock dependencies using `piptools`.
 #   new     Create a new pyrgo project.
 #   remove  Remove dependencies from the manifest file.
 #   sync    Synchronize virtual environment with requirements.txt.
 #   test    Execute tests using `pytest`.
 #   venv    Create project virtual environment.
-```
+```
```

