# Comparing `tmp/pytest-console-scripts-1.3.1.tar.gz` & `tmp/pytest-console-scripts-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-console-scripts-1.3.1.tar", last modified: Fri Mar 18 10:43:12 2022, max compression
+gzip compressed data, was "dist/pytest-console-scripts-1.4.0.tar", last modified: Mon May 22 15:17:21 2023, max compression
```

## Comparing `pytest-console-scripts-1.3.1.tar` & `pytest-console-scripts-1.4.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 kvas       (501) staff       (20)        0 2022-03-18 10:43:12.793721 pytest-console-scripts-1.3.1/
-drwxr-xr-x   0 kvas       (501) staff       (20)        0 2022-03-18 10:43:12.763429 pytest-console-scripts-1.3.1/.github/
-drwxr-xr-x   0 kvas       (501) staff       (20)        0 2022-03-18 10:43:12.778178 pytest-console-scripts-1.3.1/.github/workflows/
--rw-r--r--   0 kvas       (501) staff       (20)      525 2021-09-28 20:28:03.000000 pytest-console-scripts-1.3.1/.github/workflows/test.yml
--rw-r--r--   0 kvas       (501) staff       (20)      874 2019-01-11 19:15:43.000000 pytest-console-scripts-1.3.1/.gitignore
--rw-r--r--   0 kvas       (501) staff       (20)      417 2020-09-01 21:57:39.000000 pytest-console-scripts-1.3.1/CHANGELOG.md
--rw-r--r--   0 kvas       (501) staff       (20)     1082 2016-10-26 10:42:08.000000 pytest-console-scripts-1.3.1/LICENSE
--rw-r--r--   0 kvas       (501) staff       (20)       96 2020-11-19 19:53:12.000000 pytest-console-scripts-1.3.1/MANIFEST.in
--rw-r--r--   0 kvas       (501) staff       (20)    11373 2022-03-18 10:43:12.794209 pytest-console-scripts-1.3.1/PKG-INFO
--rw-r--r--   0 kvas       (501) staff       (20)     8591 2022-03-18 10:39:14.000000 pytest-console-scripts-1.3.1/README.md
-drwxr-xr-x   0 kvas       (501) staff       (20)        0 2022-03-18 10:43:12.782532 pytest-console-scripts-1.3.1/pytest_console_scripts.egg-info/
--rw-r--r--   0 kvas       (501) staff       (20)    11373 2022-03-18 10:43:12.000000 pytest-console-scripts-1.3.1/pytest_console_scripts.egg-info/PKG-INFO
--rw-r--r--   0 kvas       (501) staff       (20)      485 2022-03-18 10:43:12.000000 pytest-console-scripts-1.3.1/pytest_console_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 kvas       (501) staff       (20)        1 2022-03-18 10:43:12.000000 pytest-console-scripts-1.3.1/pytest_console_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 kvas       (501) staff       (20)       53 2022-03-18 10:43:12.000000 pytest-console-scripts-1.3.1/pytest_console_scripts.egg-info/entry_points.txt
--rw-r--r--   0 kvas       (501) staff       (20)       14 2022-03-18 10:43:12.000000 pytest-console-scripts-1.3.1/pytest_console_scripts.egg-info/requires.txt
--rw-r--r--   0 kvas       (501) staff       (20)       23 2022-03-18 10:43:12.000000 pytest-console-scripts-1.3.1/pytest_console_scripts.egg-info/top_level.txt
--rw-r--r--   0 kvas       (501) staff       (20)     9662 2022-03-18 10:39:14.000000 pytest-console-scripts-1.3.1/pytest_console_scripts.py
--rw-r--r--   0 kvas       (501) staff       (20)       63 2022-03-18 10:43:12.797971 pytest-console-scripts-1.3.1/setup.cfg
--rw-r--r--   0 kvas       (501) staff       (20)     1623 2022-03-18 10:39:14.000000 pytest-console-scripts-1.3.1/setup.py
-drwxr-xr-x   0 kvas       (501) staff       (20)        0 2022-03-18 10:43:12.790639 pytest-console-scripts-1.3.1/tests/
--rw-r--r--   0 kvas       (501) staff       (20)       28 2016-10-26 10:42:08.000000 pytest-console-scripts-1.3.1/tests/conftest.py
--rw-r--r--   0 kvas       (501) staff       (20)     3076 2020-11-20 17:09:54.000000 pytest-console-scripts-1.3.1/tests/test_console_scripts.py
--rw-r--r--   0 kvas       (501) staff       (20)    10326 2022-01-06 15:05:28.000000 pytest-console-scripts-1.3.1/tests/test_run_scripts.py
--rw-r--r--   0 kvas       (501) staff       (20)      658 2021-09-28 20:30:06.000000 pytest-console-scripts-1.3.1/tox.ini
+drwxr-xr-x   0 kvas       (501) staff       (20)        0 2023-05-22 15:17:21.910737 pytest-console-scripts-1.4.0/
+drwxr-xr-x   0 kvas       (501) staff       (20)        0 2023-05-22 15:17:21.883577 pytest-console-scripts-1.4.0/.github/
+drwxr-xr-x   0 kvas       (501) staff       (20)        0 2023-05-22 15:17:21.891069 pytest-console-scripts-1.4.0/.github/workflows/
+-rw-r--r--   0 kvas       (501) staff       (20)      735 2023-05-22 15:06:38.000000 pytest-console-scripts-1.4.0/.github/workflows/test.yml
+-rw-r--r--   0 kvas       (501) staff       (20)      874 2019-01-11 19:15:43.000000 pytest-console-scripts-1.4.0/.gitignore
+-rw-r--r--   0 kvas       (501) staff       (20)      417 2020-09-01 21:57:39.000000 pytest-console-scripts-1.4.0/CHANGELOG.md
+-rw-r--r--   0 kvas       (501) staff       (20)     1082 2016-10-26 10:42:08.000000 pytest-console-scripts-1.4.0/LICENSE
+-rw-r--r--   0 kvas       (501) staff       (20)       96 2020-11-19 19:53:12.000000 pytest-console-scripts-1.4.0/MANIFEST.in
+-rw-r--r--   0 kvas       (501) staff       (20)    12052 2023-05-22 15:17:21.913662 pytest-console-scripts-1.4.0/PKG-INFO
+-rw-r--r--   0 kvas       (501) staff       (20)     9056 2023-05-22 15:06:38.000000 pytest-console-scripts-1.4.0/README.md
+drwxr-xr-x   0 kvas       (501) staff       (20)        0 2023-05-22 15:17:21.892508 pytest-console-scripts-1.4.0/pytest_console_scripts/
+-rw-r--r--   0 kvas       (501) staff       (20)    14470 2023-05-22 15:06:38.000000 pytest-console-scripts-1.4.0/pytest_console_scripts/__init__.py
+-rw-r--r--   0 kvas       (501) staff       (20)        0 2023-05-22 15:06:38.000000 pytest-console-scripts-1.4.0/pytest_console_scripts/py.typed
+drwxr-xr-x   0 kvas       (501) staff       (20)        0 2023-05-22 15:17:21.896340 pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/
+-rw-r--r--   0 kvas       (501) staff       (20)    12052 2023-05-22 15:17:21.000000 pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 kvas       (501) staff       (20)      526 2023-05-22 15:17:21.000000 pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 kvas       (501) staff       (20)        1 2023-05-22 15:17:21.000000 pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 kvas       (501) staff       (20)       53 2023-05-22 15:17:21.000000 pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/entry_points.txt
+-rw-r--r--   0 kvas       (501) staff       (20)       66 2023-05-22 15:17:21.000000 pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/requires.txt
+-rw-r--r--   0 kvas       (501) staff       (20)       23 2023-05-22 15:17:21.000000 pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/top_level.txt
+-rw-r--r--   0 kvas       (501) staff       (20)       63 2023-05-22 15:17:21.917099 pytest-console-scripts-1.4.0/setup.cfg
+-rw-r--r--   0 kvas       (501) staff       (20)     1663 2023-05-22 15:06:38.000000 pytest-console-scripts-1.4.0/setup.py
+drwxr-xr-x   0 kvas       (501) staff       (20)        0 2023-05-22 15:17:21.906618 pytest-console-scripts-1.4.0/tests/
+-rw-r--r--   0 kvas       (501) staff       (20)       28 2016-10-26 10:42:08.000000 pytest-console-scripts-1.4.0/tests/conftest.py
+-rw-r--r--   0 kvas       (501) staff       (20)     3634 2023-05-15 20:16:04.000000 pytest-console-scripts-1.4.0/tests/test_console_scripts.py
+-rw-r--r--   0 kvas       (501) staff       (20)    14149 2023-05-22 15:06:38.000000 pytest-console-scripts-1.4.0/tests/test_run_scripts.py
+-rw-r--r--   0 kvas       (501) staff       (20)     1107 2023-05-22 15:06:38.000000 pytest-console-scripts-1.4.0/tox.ini
```

### Comparing `pytest-console-scripts-1.3.1/.gitignore` & `pytest-console-scripts-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-console-scripts-1.3.1/LICENSE` & `pytest-console-scripts-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-console-scripts-1.3.1/PKG-INFO` & `pytest-console-scripts-1.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-console-scripts
-Version: 1.3.1
+Version: 1.4.0
 Summary: Pytest plugin for testing console scripts
 Home-page: https://github.com/kvas-it/pytest-console-scripts
 Author: Vasily Kuznetsov
 Author-email: kvas.it@gmail.com
 Maintainer: Vasily Kuznetsov
 Maintainer-email: kvas.it@gmail.com
 License: MIT
@@ -20,23 +20,25 @@
         run many external scripts. This is speeds up development. In the CI environment
         subprocess mode can be used to make sure the scripts also work (and behave the
         same) when run by a fresh interpreter.
         
         Requirements
         ------------
         
-        - Python 3.6+, or PyPy3,
+        - Python 3.7+, or PyPy3,
         - Pytest 4.0 or newer.
         
         Installation
         ------------
         
         You can install "pytest-console-scripts" via [pip][2] from [PyPI][3]:
         
-            $ pip install pytest-console-scripts
+        ```sh
+        $ pip install pytest-console-scripts
+        ```
         
         Normally you would add it as a test dependency in `tox.ini` (see [tox
         documentation][9]).
         
         Usage
         -----
         
@@ -46,67 +48,92 @@
         executables that are not Python scripts, but only in subprocess mode (there's
         no benefit in using `pytest-console-scripts` for this, you should just use
         `subprocess.run`).
         
         Here's an example with `console_scripts` entry point. Imagine we have a python
         package `foo` with the following `setup.py`:
         
-            setup(
-                name='foo',
-                version='0.0.1',
-                py_modules=['foo'],
-                entry_points={
-                    'console_scripts': ['foobar=foo:bar']
-                },
-            )
+        ```py
+        setup(
+            name='foo',
+            version='0.0.1',
+            py_modules=['foo'],
+            entry_points={
+                'console_scripts': ['foobar=foo:bar']
+            },
+        )
+        ```
         
         We could use pytest-console-scripts to test the `foobar` script:
         
-            def test_foo_bar(script_runner):
-                ret = script_runner.run('foobar', '--version')
-                assert ret.success
-                assert ret.stdout == '3.2.1\n'
-                assert ret.stderr == ''
+        ```py
+        def test_foo_bar(script_runner):
+            result = script_runner.run(['foobar', '--version'])
+            assert result.returncode == 0
+            assert result.stdout == '3.2.1\n'
+            assert result.stderr == ''
+        
+            script_runner.run('foobar --version', shell=True, check=True)
+        ```
         
         This would use the `script_runner` fixture provided by the plugin to
         run the script and capture its output.
         
         The arguments of `script_runner.run` are the command name of the script and
         any command line arguments that should be passed to it. Additionally the
         following keyword arguments can be used:
         
         - `cwd` - set the working directory of the script under test.
         - `env` - a dictionary with environment variables to use instead of the current
           environment.
         - `stdin` - a file-like object that will be piped to standard input of the
           script.
+        - `check` - raises an exception if `returncode != 0`, defaults to False.
+        - `shell` - mimic shell execution, this should work well for simple cases,
+          defaults to False.
+        
+        Type-hinting is also supported.
+        You may type-hint the fixture with the following code:
+        
+        ```py
+        from pytest_console_scripts import ScriptRunner
+        
+        def test_foo_bar(script_runner: ScriptRunner) -> None:
+            ...
+        ```
         
         Configuring script execution mode
         ---------------------------------
         
         In the example above the `foobar` script would run in in-process mode (which is
         the default). This is fast and good for quick iteration during development.
         After we're happy with the functionality, it's time to run the script in
         subprocess mode to simulate real invocation more closely. There are several
         ways to do this. We can configure it via pytest configuration (for example in
         `tox.ini`):
         
-             [pytest]
-             script_launch_mode = subprocess
+        ```ini
+        [pytest]
+        script_launch_mode = subprocess
+        ```
         
         We can give a command line option to pytest (this will override the
         configuration file):
         
-            $ pytest --script-launch-mode=subprocess test_foobar.py
+        ```sh
+        $ pytest --script-launch-mode=subprocess test_foobar.py
+        ```
         
         We can also mark individual tests to run in a specific mode:
         
-            @pytest.mark.script_launch_mode('subprocess')
-            def test_foobar(script_runner):
-                ...
+        ```py
+        @pytest.mark.script_launch_mode('subprocess')
+        def test_foobar(script_runner):
+            ...
+        ```
         
         Between these three methods the marking of the tests has priority before the
         command line option that in turn overrides the configuration setting. All three
         can take three possible values: "inprocess", "subprocess", and "both" (which
         will cause the test to be run twice: in in-process and in subprocess modes).
         
         Interaction with mocking
@@ -140,27 +167,33 @@
         
         However, in some cases it might be useful to disable the output capturing and
         PyTest provides [ways to do it][13]. When capturing is disabled, all test run
         results will be printed out and this might make it harder to inspect the other
         output of the tests. To deal with this, `pytest-console-scripts` has an option
         to disable the printing of script run results:
         
-            $ pytest --hide-run-results test_foobar.py
+        ```sh
+        $ pytest --hide-run-results test_foobar.py
+        ```
         
         It's also possible to disable it just for one script run:
         
-            result = script_runner.run('foobar', print_result=False)
+        ```py
+        result = script_runner.run('foobar', print_result=False)
+        ```
         
         When printing of script run results is disabled, script output won't be
-        visisble even when the test fails. Unfortunately there's no automatic way to
+        visible even when the test fails. Unfortunately there's no automatic way to
         print it only if the test fails because by the time a script run completes we
         don't know whether the test will fail or not. It's possible to do it manually
         from the test by using:
         
-            result.print()
+        ```py
+        result.print()
+        ```
         
         This, combined with `--hide-run-results` or `print_result=False` can be used to
         only print interesting run results when capturing is off.
         
         Package installation and testing during development
         ---------------------------------------------------
         
@@ -221,17 +254,16 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pytest-console-scripts-1.3.1/README.md` & `pytest-console-scripts-1.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -10,23 +10,25 @@
 run many external scripts. This is speeds up development. In the CI environment
 subprocess mode can be used to make sure the scripts also work (and behave the
 same) when run by a fresh interpreter.
 
 Requirements
 ------------
 
-- Python 3.6+, or PyPy3,
+- Python 3.7+, or PyPy3,
 - Pytest 4.0 or newer.
 
 Installation
 ------------
 
 You can install "pytest-console-scripts" via [pip][2] from [PyPI][3]:
 
-    $ pip install pytest-console-scripts
+```sh
+$ pip install pytest-console-scripts
+```
 
 Normally you would add it as a test dependency in `tox.ini` (see [tox
 documentation][9]).
 
 Usage
 -----
 
@@ -36,67 +38,92 @@
 executables that are not Python scripts, but only in subprocess mode (there's
 no benefit in using `pytest-console-scripts` for this, you should just use
 `subprocess.run`).
 
 Here's an example with `console_scripts` entry point. Imagine we have a python
 package `foo` with the following `setup.py`:
 
-    setup(
-        name='foo',
-        version='0.0.1',
-        py_modules=['foo'],
-        entry_points={
-            'console_scripts': ['foobar=foo:bar']
-        },
-    )
+```py
+setup(
+    name='foo',
+    version='0.0.1',
+    py_modules=['foo'],
+    entry_points={
+        'console_scripts': ['foobar=foo:bar']
+    },
+)
+```
 
 We could use pytest-console-scripts to test the `foobar` script:
 
-    def test_foo_bar(script_runner):
-        ret = script_runner.run('foobar', '--version')
-        assert ret.success
-        assert ret.stdout == '3.2.1\n'
-        assert ret.stderr == ''
+```py
+def test_foo_bar(script_runner):
+    result = script_runner.run(['foobar', '--version'])
+    assert result.returncode == 0
+    assert result.stdout == '3.2.1\n'
+    assert result.stderr == ''
+
+    script_runner.run('foobar --version', shell=True, check=True)
+```
 
 This would use the `script_runner` fixture provided by the plugin to
 run the script and capture its output.
 
 The arguments of `script_runner.run` are the command name of the script and
 any command line arguments that should be passed to it. Additionally the
 following keyword arguments can be used:
 
 - `cwd` - set the working directory of the script under test.
 - `env` - a dictionary with environment variables to use instead of the current
   environment.
 - `stdin` - a file-like object that will be piped to standard input of the
   script.
+- `check` - raises an exception if `returncode != 0`, defaults to False.
+- `shell` - mimic shell execution, this should work well for simple cases,
+  defaults to False.
+
+Type-hinting is also supported.
+You may type-hint the fixture with the following code:
+
+```py
+from pytest_console_scripts import ScriptRunner
+
+def test_foo_bar(script_runner: ScriptRunner) -> None:
+    ...
+```
 
 Configuring script execution mode
 ---------------------------------
 
 In the example above the `foobar` script would run in in-process mode (which is
 the default). This is fast and good for quick iteration during development.
 After we're happy with the functionality, it's time to run the script in
 subprocess mode to simulate real invocation more closely. There are several
 ways to do this. We can configure it via pytest configuration (for example in
 `tox.ini`):
 
-     [pytest]
-     script_launch_mode = subprocess
+```ini
+[pytest]
+script_launch_mode = subprocess
+```
 
 We can give a command line option to pytest (this will override the
 configuration file):
 
-    $ pytest --script-launch-mode=subprocess test_foobar.py
+```sh
+$ pytest --script-launch-mode=subprocess test_foobar.py
+```
 
 We can also mark individual tests to run in a specific mode:
 
-    @pytest.mark.script_launch_mode('subprocess')
-    def test_foobar(script_runner):
-        ...
+```py
+@pytest.mark.script_launch_mode('subprocess')
+def test_foobar(script_runner):
+    ...
+```
 
 Between these three methods the marking of the tests has priority before the
 command line option that in turn overrides the configuration setting. All three
 can take three possible values: "inprocess", "subprocess", and "both" (which
 will cause the test to be run twice: in in-process and in subprocess modes).
 
 Interaction with mocking
@@ -130,27 +157,33 @@
 
 However, in some cases it might be useful to disable the output capturing and
 PyTest provides [ways to do it][13]. When capturing is disabled, all test run
 results will be printed out and this might make it harder to inspect the other
 output of the tests. To deal with this, `pytest-console-scripts` has an option
 to disable the printing of script run results:
 
-    $ pytest --hide-run-results test_foobar.py
+```sh
+$ pytest --hide-run-results test_foobar.py
+```
 
 It's also possible to disable it just for one script run:
 
-    result = script_runner.run('foobar', print_result=False)
+```py
+result = script_runner.run('foobar', print_result=False)
+```
 
 When printing of script run results is disabled, script output won't be
-visisble even when the test fails. Unfortunately there's no automatic way to
+visible even when the test fails. Unfortunately there's no automatic way to
 print it only if the test fails because by the time a script run completes we
 don't know whether the test will fail or not. It's possible to do it manually
 from the test by using:
 
-    result.print()
+```py
+result.print()
+```
 
 This, combined with `--hide-run-results` or `print_result=False` can be used to
 only print interesting run results when capturing is off.
 
 Package installation and testing during development
 ---------------------------------------------------
```

### Comparing `pytest-console-scripts-1.3.1/pytest_console_scripts.egg-info/PKG-INFO` & `pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-console-scripts
-Version: 1.3.1
+Version: 1.4.0
 Summary: Pytest plugin for testing console scripts
 Home-page: https://github.com/kvas-it/pytest-console-scripts
 Author: Vasily Kuznetsov
 Author-email: kvas.it@gmail.com
 Maintainer: Vasily Kuznetsov
 Maintainer-email: kvas.it@gmail.com
 License: MIT
@@ -20,23 +20,25 @@
         run many external scripts. This is speeds up development. In the CI environment
         subprocess mode can be used to make sure the scripts also work (and behave the
         same) when run by a fresh interpreter.
         
         Requirements
         ------------
         
-        - Python 3.6+, or PyPy3,
+        - Python 3.7+, or PyPy3,
         - Pytest 4.0 or newer.
         
         Installation
         ------------
         
         You can install "pytest-console-scripts" via [pip][2] from [PyPI][3]:
         
-            $ pip install pytest-console-scripts
+        ```sh
+        $ pip install pytest-console-scripts
+        ```
         
         Normally you would add it as a test dependency in `tox.ini` (see [tox
         documentation][9]).
         
         Usage
         -----
         
@@ -46,67 +48,92 @@
         executables that are not Python scripts, but only in subprocess mode (there's
         no benefit in using `pytest-console-scripts` for this, you should just use
         `subprocess.run`).
         
         Here's an example with `console_scripts` entry point. Imagine we have a python
         package `foo` with the following `setup.py`:
         
-            setup(
-                name='foo',
-                version='0.0.1',
-                py_modules=['foo'],
-                entry_points={
-                    'console_scripts': ['foobar=foo:bar']
-                },
-            )
+        ```py
+        setup(
+            name='foo',
+            version='0.0.1',
+            py_modules=['foo'],
+            entry_points={
+                'console_scripts': ['foobar=foo:bar']
+            },
+        )
+        ```
         
         We could use pytest-console-scripts to test the `foobar` script:
         
-            def test_foo_bar(script_runner):
-                ret = script_runner.run('foobar', '--version')
-                assert ret.success
-                assert ret.stdout == '3.2.1\n'
-                assert ret.stderr == ''
+        ```py
+        def test_foo_bar(script_runner):
+            result = script_runner.run(['foobar', '--version'])
+            assert result.returncode == 0
+            assert result.stdout == '3.2.1\n'
+            assert result.stderr == ''
+        
+            script_runner.run('foobar --version', shell=True, check=True)
+        ```
         
         This would use the `script_runner` fixture provided by the plugin to
         run the script and capture its output.
         
         The arguments of `script_runner.run` are the command name of the script and
         any command line arguments that should be passed to it. Additionally the
         following keyword arguments can be used:
         
         - `cwd` - set the working directory of the script under test.
         - `env` - a dictionary with environment variables to use instead of the current
           environment.
         - `stdin` - a file-like object that will be piped to standard input of the
           script.
+        - `check` - raises an exception if `returncode != 0`, defaults to False.
+        - `shell` - mimic shell execution, this should work well for simple cases,
+          defaults to False.
+        
+        Type-hinting is also supported.
+        You may type-hint the fixture with the following code:
+        
+        ```py
+        from pytest_console_scripts import ScriptRunner
+        
+        def test_foo_bar(script_runner: ScriptRunner) -> None:
+            ...
+        ```
         
         Configuring script execution mode
         ---------------------------------
         
         In the example above the `foobar` script would run in in-process mode (which is
         the default). This is fast and good for quick iteration during development.
         After we're happy with the functionality, it's time to run the script in
         subprocess mode to simulate real invocation more closely. There are several
         ways to do this. We can configure it via pytest configuration (for example in
         `tox.ini`):
         
-             [pytest]
-             script_launch_mode = subprocess
+        ```ini
+        [pytest]
+        script_launch_mode = subprocess
+        ```
         
         We can give a command line option to pytest (this will override the
         configuration file):
         
-            $ pytest --script-launch-mode=subprocess test_foobar.py
+        ```sh
+        $ pytest --script-launch-mode=subprocess test_foobar.py
+        ```
         
         We can also mark individual tests to run in a specific mode:
         
-            @pytest.mark.script_launch_mode('subprocess')
-            def test_foobar(script_runner):
-                ...
+        ```py
+        @pytest.mark.script_launch_mode('subprocess')
+        def test_foobar(script_runner):
+            ...
+        ```
         
         Between these three methods the marking of the tests has priority before the
         command line option that in turn overrides the configuration setting. All three
         can take three possible values: "inprocess", "subprocess", and "both" (which
         will cause the test to be run twice: in in-process and in subprocess modes).
         
         Interaction with mocking
@@ -140,27 +167,33 @@
         
         However, in some cases it might be useful to disable the output capturing and
         PyTest provides [ways to do it][13]. When capturing is disabled, all test run
         results will be printed out and this might make it harder to inspect the other
         output of the tests. To deal with this, `pytest-console-scripts` has an option
         to disable the printing of script run results:
         
-            $ pytest --hide-run-results test_foobar.py
+        ```sh
+        $ pytest --hide-run-results test_foobar.py
+        ```
         
         It's also possible to disable it just for one script run:
         
-            result = script_runner.run('foobar', print_result=False)
+        ```py
+        result = script_runner.run('foobar', print_result=False)
+        ```
         
         When printing of script run results is disabled, script output won't be
-        visisble even when the test fails. Unfortunately there's no automatic way to
+        visible even when the test fails. Unfortunately there's no automatic way to
         print it only if the test fails because by the time a script run completes we
         don't know whether the test will fail or not. It's possible to do it manually
         from the test by using:
         
-            result.print()
+        ```py
+        result.print()
+        ```
         
         This, combined with `--hide-run-results` or `print_result=False` can be used to
         only print interesting run results when capturing is off.
         
         Package installation and testing during development
         ---------------------------------------------------
         
@@ -221,17 +254,16 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pytest-console-scripts-1.3.1/pytest_console_scripts.py` & `pytest-console-scripts-1.4.0/pytest_console_scripts/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,40 @@
-from __future__ import unicode_literals, print_function
+from __future__ import annotations
 
+import contextlib
 import io
 import logging
 import os
-import pkg_resources
+import shlex
 import shutil
 import subprocess
 import sys
 import traceback
-
+import warnings
+from pathlib import Path
+from typing import Any, Callable, Iterator, Sequence, Union
 from unittest import mock
+
 import pytest
 
+if sys.version_info < (3, 10):
+    import importlib_metadata
+else:
+    import importlib.metadata as importlib_metadata
+
+_StrOrPath = Union[str, os.PathLike]
+"""A command line argument type as a str or path."""
+
+_Command = Union[_StrOrPath, Sequence[_StrOrPath]]
+"""A command-like type compatible with subprocess.run."""
+
 StreamMock = io.StringIO
 
 
-def pytest_addoption(parser):
+def pytest_addoption(parser: pytest.Parser) -> None:
     group = parser.getgroup('console-scripts')
     group.addoption(
         '--script-launch-mode',
         metavar='inprocess|subprocess|both',
         action='store',
         dest='script_launch_mode',
         default=None,
@@ -27,46 +42,48 @@
     )
     group.addoption(
         '--hide-run-results',
         action='store_true',
         dest='hide_run_results',
         default=False,
         help="don't print out script run results on failures or when "
-             "output capturing is disabled"
+             'output capturing is disabled'
     )
     parser.addini(
         'script_launch_mode',
         'how to run python scripts under test (inprocess|subprocess|both)'
     )
 
 
-def pytest_configure(config):
+def pytest_configure(config: pytest.Config) -> None:
     config.addinivalue_line(
         'markers',
         'script_launch_mode: how to run python scripts under test '
         '(inprocess|subprocess|both)',
     )
 
 
-def _get_mark_mode(metafunc):
+def _get_mark_mode(metafunc: pytest.Metafunc) -> str | None:
     """Return launch mode as indicated by test function marker or None."""
     marker = metafunc.definition.get_closest_marker('script_launch_mode')
     if marker:
-        return marker.args[0]
+        return str(marker.args[0])
+    return None
 
 
-def _is_nonexecutable_python_file(command):
+def _is_nonexecutable_python_file(command: _StrOrPath) -> bool:
     """Check if `command` is a Python file with no executable mode set."""
-    mode = os.stat(command).st_mode
+    command = Path(command)
+    mode = command.stat().st_mode
     if mode & os.X_OK:
         return False
-    return os.path.splitext(command)[1] == '.py'
+    return command.suffix == '.py'
 
 
-def pytest_generate_tests(metafunc):
+def pytest_generate_tests(metafunc: pytest.Metafunc) -> None:
     """Parametrize script_launch_mode fixture.
 
     Checks the configuration sources in this order:
     - `script_launch_mode` mark on the test,
     - `--script-launch-mode` option,
     - `script_launch_mode` configuration option in [pytest] section of the
       pyest config file.
@@ -90,200 +107,350 @@
 
     if mode in {'inprocess', 'subprocess'}:
         metafunc.parametrize('script_launch_mode', [mode], indirect=True)
     elif mode == 'both':
         metafunc.parametrize('script_launch_mode', ['inprocess', 'subprocess'],
                              indirect=True)
     else:
-        raise ValueError('Invalid script launch mode: {}'.format(mode))
+        raise ValueError(f'Invalid script launch mode: {mode}')
 
 
-class RunResult(object):
+class RunResult:
     """Result of running a script."""
 
-    def __init__(self, returncode, stdout, stderr, print_result):
+    def __init__(
+        self, returncode: int, stdout: str, stderr: str, print_result: bool
+    ) -> None:
         self.success = returncode == 0
         self.returncode = returncode
         self.stdout = stdout
         self.stderr = stderr
         if print_result:
             self.print()
 
-    def print(self):
+    def print(self) -> None:
         print('# Script return code:', self.returncode)
         print('# Script stdout:', self.stdout, sep='\n')
         print('# Script stderr:', self.stderr, sep='\n')
 
 
-class ScriptRunner(object):
+def _handle_command_args(
+    command: _Command,
+    *args: _StrOrPath,
+    shell: bool = False,
+) -> Sequence[_StrOrPath]:
+    """Return command arguments in a consistent list format.
+
+    If shell=True then this function tries to mimic local shell execution.
+    """
+    if shell:
+        if args or not isinstance(command, (str, os.PathLike)):
+            command = subprocess.list2cmdline(
+                str(arg)
+                for arg in _handle_command_args(command, *args, shell=False)
+            )
+        command = shlex.split(str(command), posix=os.name == 'posix')
+        args = ()
+
+    if args:
+        warnings.warn(
+            'script_runner commands should be passed as a single sequence,'
+            ' not as multiple arguments.'
+            '\nReplace `script_runner.run(a, b, c)` calls with'
+            ' `script_runner.run([a, b, c])`',
+            DeprecationWarning,
+        )
+        if not isinstance(command, (str, os.PathLike)):
+            return [*command, *args]
+        return [command, *args]
+    if isinstance(command, (str, os.PathLike)):
+        return [command]
+    return command
+
+
+@contextlib.contextmanager
+def _patch_environ(new_environ: dict[str, str] | None) -> Iterator[None]:
+    """Replace the environment for the duration of a context."""
+    if new_environ is None:
+        yield
+        return
+    old_environ = os.environ.copy()
+    os.environ.clear()
+    os.environ.update(new_environ)
+    yield
+    os.environ.clear()
+    os.environ.update(old_environ)
+
+
+@contextlib.contextmanager
+def _chdir_context(new_dir: _StrOrPath | None) -> Iterator[None]:
+    """Replace the current directory for the duration of a context."""
+    if new_dir is None:
+        yield
+        return
+    old_cwd = os.getcwd()
+    os.chdir(new_dir)
+    yield
+    os.chdir(old_cwd)
+
+
+@contextlib.contextmanager
+def _push_and_reset_logger() -> Iterator[None]:
+    """Do a very basic reset of the root logger and restore its config on exit.
+
+    This allows scripts to call logging.basicConfig(...) and have
+    it work as expected. It might not work for more sophisticated logging
+    setups but it's simple and covers the basic usage whereas implementing
+    a comprehensive fix is impossible in a compatible way.
+    """
+    logger = logging.getLogger()
+    old_handlers = logger.handlers
+    old_disabled = logger.disabled
+    old_level = logger.level
+    logger.handlers = []
+    logger.disabled = False
+    logger.setLevel(logging.NOTSET)
+    yield
+    # Restore logger to previous configuration
+    logger.handlers = old_handlers
+    logger.disabled = old_disabled
+    logger.setLevel(old_level)
+
+
+class ScriptRunner:
     """Fixture for running python scripts under test."""
 
-    def __init__(self, launch_mode, rootdir, print_result=True):
+    def __init__(
+        self, launch_mode: str,
+        rootdir: _StrOrPath,
+        print_result: bool = True
+    ) -> None:
         assert launch_mode in {'inprocess', 'subprocess'}
         self.launch_mode = launch_mode
         self.print_result = print_result
         self.rootdir = rootdir
 
-    def __repr__(self):
-        return '<ScriptRunner {}>'.format(self.launch_mode)
+    def __repr__(self) -> str:
+        return f'<ScriptRunner {self.launch_mode}>'
+
+    def run(
+        self,
+        command: _Command,
+        *arguments: _StrOrPath,
+        print_result: bool | None = None,
+        shell: bool = False,
+        cwd: _StrOrPath | None = None,
+        env: dict[str, str] | None = None,
+        stdin: io.IOBase | None = None,
+        check: bool = False,
+        **options: Any,
+    ) -> RunResult:
+        if print_result is None:
+            print_result = self.print_result
 
-    def run(self, command, *arguments, **options):
-        options.setdefault('print_result', self.print_result)
-        if options['print_result']:
+        if print_result:
             print('# Running console script:', command, *arguments)
 
         if self.launch_mode == 'inprocess':
-            return self.run_inprocess(command, *arguments, **options)
-        return self.run_subprocess(command, *arguments, **options)
-
-    def _save_and_reset_logger(self):
-        """Do a very basic reset of the root logger and return its config.
-
-        This allows scripts to call logging.basicConfig(...) and have
-        it work as expected. It might not work for more sophisticated logging
-        setups but it's simple and covers the basic usage whereas implementing
-        a comprehensive fix is impossible in a compatible way.
-
-        """
-        logger = logging.getLogger()
-        config = {
-            'level': logger.level,
-            'handlers': logger.handlers,
-            'disabled': logger.disabled,
-        }
-        logger.handlers = []
-        logger.disabled = False
-        logger.setLevel(logging.NOTSET)
-        return config
-
-    def _restore_logger(self, config):
-        """Restore logger to previous configuration."""
-        logger = logging.getLogger()
-        logger.handlers = config['handlers']
-        logger.disabled = config['disabled']
-        logger.setLevel(config['level'])
+            run_function = self.run_inprocess
+        else:
+            run_function = self.run_subprocess
+        return run_function(
+            command,
+            *arguments,
+            print_result=print_result,
+            shell=shell,
+            cwd=cwd,
+            env=env,
+            stdin=stdin,
+            check=check,
+            **options,
+        )
 
-    def _locate_script(self, command, **options):
+    @staticmethod
+    def _locate_script(
+        command: _StrOrPath,
+        *,
+        cwd: _StrOrPath | None,
+        env: dict[str, str] | None,
+    ) -> Path:
         """Locate script in PATH or in current directory."""
         script_path = shutil.which(
             command,
-            path=options.get('env', {}).get('PATH', None),
+            path=env.get('PATH', None) if env is not None else None,
         )
         if script_path is not None:
-            return script_path
-
-        cwd = options.get('cwd', os.getcwd())
-        script_path = os.path.join(cwd, command)
-        if os.path.exists(script_path):
-            return script_path
+            return Path(script_path)
 
-        raise FileNotFoundError('Cannot find ' + command)
+        cwd = cwd if cwd is not None else os.getcwd()
+        return Path(cwd, command).resolve(strict=True)
 
-    def _load_script(self, command, **options):
+    @classmethod
+    def _load_script(
+        cls,
+        command: _StrOrPath,
+        *,
+        cwd: _StrOrPath | None,
+        env: dict[str, str] | None,
+    ) -> Callable[[], int | None]:
         """Load target script via entry points or compile/exec."""
-        entry_points = list(pkg_resources.iter_entry_points('console_scripts',
-                                                            command))
-        if entry_points:
-            def console_script():
-                s = entry_points[0].load()
-                return s()
-            return console_script
+        if isinstance(command, str):
+            entry_points = tuple(
+                importlib_metadata.entry_points(
+                    group='console_scripts', name=command
+                )
+            )
+            if entry_points:
+                def console_script() -> int | None:
+                    s: Callable[[], int | None] = entry_points[0].load()
+                    return s()
+                return console_script
 
-        script_path = self._locate_script(command, **options)
+        script_path = cls._locate_script(command, cwd=cwd, env=env)
 
-        def exec_script():
+        def exec_script() -> int:
             with open(script_path, 'rt', encoding='utf-8') as script:
                 compiled = compile(script.read(), str(script), 'exec', flags=0)
                 exec(compiled, {'__name__': '__main__'})
             return 0
 
         return exec_script
 
-    def run_inprocess(self, command, *arguments, **options):
-        cmdargs = [command] + list(arguments)
-        script = self._load_script(command, **options)
-        stdin = options.get('stdin', StreamMock())
-        stdout = StreamMock()
-        stderr = StreamMock()
-        stdin_patch = mock.patch('sys.stdin', new=stdin)
-        stdout_patch = mock.patch('sys.stdout', new=stdout)
-        stderr_patch = mock.patch('sys.stderr', new=stderr)
-        argv_patch = mock.patch('sys.argv', new=cmdargs)
-        saved_dir = os.getcwd()
-        logger_conf = self._save_and_reset_logger()
-
-        if 'env' in options:
-            old_env = os.environ
-            os.environ = options.get('env')
+    @classmethod
+    def run_inprocess(
+        cls,
+        command: _Command,
+        *arguments: _StrOrPath,
+        shell: bool = False,
+        cwd: _StrOrPath | None = None,
+        env: dict[str, str] | None = None,
+        print_result: bool = True,
+        stdin: io.IOBase | None = None,
+        check: bool = False,
+        **options: Any,
+    ) -> RunResult:
+        for key in options:
+            warnings.warn(
+                f'Keyword argument {key!r} was ignored.'
+                '\nConsider using subprocess mode or raising an issue.'
+            )
+        cmd_args = _handle_command_args(command, *arguments, shell=shell)
+        script = cls._load_script(cmd_args[0], cwd=cwd, env=env)
+        cmd_args = [str(cmd) for cmd in cmd_args]
+        stdin_stream = stdin if stdin is not None else StreamMock()
+        stdout_stream = StreamMock()
+        stderr_stream = StreamMock()
+        with contextlib.ExitStack() as stack:
+            stack.enter_context(mock.patch('sys.stdin', new=stdin_stream))
+            stack.enter_context(contextlib.redirect_stdout(stdout_stream))
+            stack.enter_context(contextlib.redirect_stderr(stderr_stream))
+            stack.enter_context(mock.patch('sys.argv', new=cmd_args))
+            stack.enter_context(_push_and_reset_logger())
+            stack.enter_context(_patch_environ(env))
+            stack.enter_context(_chdir_context(cwd))
 
-        if 'cwd' in options:
-            os.chdir(options['cwd'])
-
-        print_result = options.pop('print_result')
-
-        with stdin_patch, stdout_patch, stderr_patch, argv_patch:
             try:
                 returncode = script()
-                if returncode is None:
-                    returncode = 0  # None also means success.
             except SystemExit as exc:
-                returncode = exc.code
-                if isinstance(returncode, str):
-                    stderr.write('{}\n'.format(exc))
+                returncode = 1
+                if isinstance(exc.code, str):
+                    stderr_stream.write(f'{exc}\n')
                     returncode = 1
-                elif returncode is None:
-                    returncode = 0
+                else:
+                    returncode = exc.code
             except Exception:
                 returncode = 1
                 try:
                     et, ev, tb = sys.exc_info()
+                    assert tb
                     # Hide current frame from the stack trace.
                     traceback.print_exception(et, ev, tb.tb_next)
                 finally:
                     del tb
 
-        self._restore_logger(logger_conf)
-        os.chdir(saved_dir)
-
-        if 'env' in options:
-            os.environ = old_env
-
-        return RunResult(returncode, stdout.getvalue(), stderr.getvalue(),
-                         print_result)
+        result = RunResult(
+            returncode or 0,  # None also means success
+            stdout_stream.getvalue(),
+            stderr_stream.getvalue(),
+            print_result,
+        )
 
-    def run_subprocess(self, command, *arguments, **options):
-        stdin_input = None
-        if 'stdin' in options:
-            stdin_input = options.pop('stdin').read()
+        if check and returncode:
+            raise subprocess.CalledProcessError(
+                returncode,
+                cmd_args,
+                result.stdout,
+                result.stderr,
+            )
+
+        return result
+
+    @classmethod
+    def run_subprocess(
+        cls,
+        command: _Command,
+        *arguments: _StrOrPath,
+        print_result: bool = True,
+        shell: bool = False,
+        cwd: _StrOrPath | None = None,
+        env: dict[str, str] | None = None,
+        stdin: io.IOBase | None = None,
+        check: bool = False,
+        universal_newlines: bool = True,
+        **options: Any,
+    ) -> RunResult:
+        stdin_input: str | bytes | None = None
+        if stdin is not None:
+            stdin_input = stdin.read()
 
-        options.setdefault('universal_newlines', True)
-        print_result = options.pop('print_result')
+        script_path = cls._locate_script(_handle_command_args(
+            command, *arguments, shell=shell)[0], cwd=cwd, env=env
+        )
+        if arguments:
+            command = _handle_command_args(command, *arguments, shell=shell)
 
-        cmd_args = [command] + list(arguments)
-        script_path = self._locate_script(command, **options)
         if _is_nonexecutable_python_file(script_path):
-            cmd_args = [sys.executable or 'python'] + cmd_args
+            command = _handle_command_args(command, shell=shell)
+            command = [sys.executable or 'python', *command]
+
+        if sys.version_info < (3, 8):
+            if isinstance(command, os.PathLike):
+                command = [command]
+            if not isinstance(command, str):
+                command = [
+                    str(Path(arg)) if isinstance(arg, os.PathLike) else arg
+                    for arg in command
+                ]
 
         cp = subprocess.run(
-            cmd_args,
+            command,
             input=stdin_input,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
+            shell=shell,
+            cwd=cwd,
+            env=env,
+            check=check,
+            universal_newlines=universal_newlines,
             **options,
         )
         return RunResult(cp.returncode, cp.stdout, cp.stderr, print_result)
 
 
 @pytest.fixture
-def script_launch_mode(request):
-    return request.param
+def script_launch_mode(request: pytest.FixtureRequest) -> str:
+    return str(request.param)
 
 
 @pytest.fixture
-def script_cwd(tmpdir):
-    return tmpdir.mkdir('script-cwd')
+def script_cwd(tmp_path: Path) -> Path:
+    work_dir = tmp_path / 'script-cwd'
+    work_dir.mkdir()
+    return work_dir
 
 
 @pytest.fixture
-def script_runner(request, script_cwd, script_launch_mode):
-    print_result = not request.config.getoption("--hide-run-results")
+def script_runner(
+    request: pytest.FixtureRequest, script_cwd: Path, script_launch_mode: str
+) -> ScriptRunner:
+    print_result = not request.config.getoption('--hide-run-results')
     return ScriptRunner(script_launch_mode, script_cwd, print_result)
```

### Comparing `pytest-console-scripts-1.3.1/setup.py` & `pytest-console-scripts-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import os
+from pathlib import Path
 from setuptools import setup
 
-
-def read(fname):
-    file_path = os.path.join(os.path.dirname(__file__), fname)
-    with open(file_path, encoding='utf-8') as f:
-        return f.read()
+THIS_DIR = Path(__file__).parent
+README_TEXT = (THIS_DIR / 'README.md').read_text(encoding='utf-8')
 
 
 setup(
     name='pytest-console-scripts',
     use_scm_version=True,
     author='Vasily Kuznetsov',
     author_email='kvas.it@gmail.com',
     maintainer='Vasily Kuznetsov',
     maintainer_email='kvas.it@gmail.com',
     license='MIT',
     url='https://github.com/kvas-it/pytest-console-scripts',
     description='Pytest plugin for testing console scripts',
-    long_description=read('README.md'),
+    long_description=README_TEXT,
     long_description_content_type='text/markdown',
-    py_modules=['pytest_console_scripts'],
-    install_requires=['pytest>=4.0.0'],
-    python_requires='>=3.6',
+    packages=['pytest_console_scripts'],
+    package_data={'pytest_console_scripts': ['py.typed']},
+    install_requires=[
+        'pytest >=4.0.0',
+        "importlib_metadata >=3.6; python_version < '3.10'",
+    ],
+    python_requires='>=3.7',
     setup_requires=['setuptools-scm'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Framework :: Pytest',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Testing',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Operating System :: OS Independent',
         'License :: OSI Approved :: MIT License',
```

### Comparing `pytest-console-scripts-1.3.1/tests/test_run_scripts.py` & `pytest-console-scripts-1.4.0/tests/test_run_scripts.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,85 @@
 """Test running of scripts with various modes and options."""
+from __future__ import annotations
 
 import importlib
 import io
 import os
 import sys
+from pathlib import Path
+from subprocess import CalledProcessError
+from types import ModuleType
+from typing import Any
 from unittest import mock
 
 import pytest
 
+from pytest_console_scripts import ScriptRunner
+
 
 @pytest.fixture(params=['inprocess', 'subprocess'])
-def launch_mode(request):
+def launch_mode(request: pytest.FixtureRequest) -> str:
     """Launch mode: inprocess|subprocess."""
-    return request.param
+    return str(request.param)
 
 
 @pytest.fixture()
-def console_script(tmpdir):
+def console_script(tmp_path: Path) -> Path:
     """Python script to use in tests."""
-    script = tmpdir.join('script.py')
-    script.write('#!/usr/bin/env python\nprint("foo")')
+    script = tmp_path / 'script.py'
+    script.write_text('#!/usr/bin/env python\nprint("foo")')
     return script
 
 
 @pytest.mark.script_launch_mode('both')
-def test_not_installed(console_script, script_runner):
+def test_not_installed(
+    console_script: Path, script_runner: ScriptRunner
+) -> None:
     result = script_runner.run(str(console_script))
     assert result.success
     assert result.stdout == 'foo\n'
     assert result.stderr == ''
 
 
+@pytest.mark.xfail(
+    sys.platform == "win32",
+    reason="Windows does not treat Python scripts as executables."
+)
 @pytest.mark.script_launch_mode('both')
-def test_elsewhere_in_the_path(console_script, script_runner):
+def test_elsewhere_in_the_path(
+    console_script: Path, script_runner: ScriptRunner
+) -> None:
     console_script.chmod(0o777)
-    env = {'PATH': str(console_script.dirpath() + ':' + os.environ['PATH'])}
-    result = script_runner.run(console_script.basename, env=env)
+    env = os.environ.copy()
+    env["PATH"] = f"{console_script.parent}{os.pathsep}{env['PATH']}"
+    result = script_runner.run(console_script.name, env=env)
     assert result.success
     assert result.stdout == 'foo\n'
     assert result.stderr == ''
 
 
 @pytest.mark.script_launch_mode('both')
-def test_run_pytest(tmpdir, console_script, script_runner, launch_mode):
-    console_script.write('import os;print(os.getpid())')
-    test = tmpdir.join('test_{}.py'.format(launch_mode))
+def test_run_pytest(
+    tmp_path: Path,
+    console_script: Path,
+    script_runner: ScriptRunner,
+    launch_mode: str
+) -> None:
+    console_script.write_text('import os;print(os.getpid())')
+    test = tmp_path / f'test_{launch_mode}.py'
     compare = '==' if launch_mode == 'inprocess' else '!='
-    test.write(
-        """
+    test.write_text(
+        f"""
 import os
 def test_script(script_runner):
-    result = script_runner.run('{}')
+    result = script_runner.run(R'''{console_script}''')
     assert result.success
-    assert result.stdout {} str(os.getpid()) + '\\n'
+    assert result.stdout {compare} str(os.getpid()) + '\\n'
     assert result.stderr == ''
-        """.format(console_script, compare)
+        """
     )
 
     # Here we're testing two things:
     #
     # - pytest is a Python script that's installed in the test environment, so
     #   we'll use `script_runner` fixture to run it -- this tests execution of
     #   installed scripts from the path.
@@ -75,249 +96,374 @@
         str(test),
         '--script-launch-mode=' + launch_mode,
     )
     assert result.success
 
 
 @pytest.mark.script_launch_mode('inprocess')
-def test_return_None(script_runner):
+def test_return_None(
+    console_script: Path, script_runner: ScriptRunner
+) -> None:
     """Check that entry point function returning None is counted as success."""
-
     # Many console_scripts entry point functions return 0 on success but not
     # all of them do. Returning `None` is also allowed and would be translated
     # to return code 0 when run normally via wrapper. This test checks that we
     # handle this case properly in inprocess mode.
-    #
-    # One commonly available script that returns None from the entry point
-    # function is easy_install so we use it here.
+    console_script.write_text(
+        """
+import sys
+print("Foo")
+sys.exit(None)
+"""
+    )
+    result = script_runner.run(str(console_script))
+    assert result.success
+    assert 'Foo' in result.stdout
 
-    try:
-        path = script_runner._locate_script('easy_install')
-        if os.path.join('.pyenv', 'shims') in path:
-            # We have a shell wrapper from pyenv instead of real easy_install.
-            return
-    except FileNotFoundError:
-        # No easy_install. We skip the test.
-        return
 
-    result = script_runner.run('easy_install', '-h')
-    assert result.success
-    assert '--verbose' in result.stdout
+@pytest.mark.script_launch_mode('inprocess')
+def test_return_code_uncommon(
+    console_script: Path, script_runner: ScriptRunner
+) -> None:
+    """Check uncommon return codes."""
+    console_script.write_text(
+        """
+import sys
+sys.exit(2)
+"""
+    )
+    assert script_runner.run(str(console_script)).returncode == 2
 
 
 @pytest.mark.script_launch_mode('both')
-def test_abnormal_exit(console_script, script_runner):
-    console_script.write('import sys;sys.exit("boom")')
+def test_abnormal_exit(
+    console_script: Path, script_runner: ScriptRunner
+) -> None:
+    console_script.write_text('import sys;sys.exit("boom")')
     result = script_runner.run(str(console_script))
     assert not result.success
     assert result.stdout == ''
     assert result.stderr == 'boom\n'
 
 
 @pytest.mark.script_launch_mode('both')
-def test_exception(console_script, script_runner):
-    console_script.write('raise TypeError("boom")')
+def test_exception(console_script: Path, script_runner: ScriptRunner) -> None:
+    console_script.write_text('raise TypeError("boom")')
     result = script_runner.run(str(console_script))
     assert not result.success
     assert result.stdout == ''
     assert 'TypeError: boom' in result.stderr
 
 
-def test_cwd(console_script, script_runner, tmpdir):
+def test_cwd(
+    console_script: Path,
+    script_runner: ScriptRunner,
+    tmp_path: Path,
+) -> None:
     """Script starts in dir given by cwd arg and cwd changes are contained."""
-    dir1 = tmpdir.mkdir('dir1')
-    dir2 = tmpdir.mkdir('dir2')
-    console_script.write(
-        """
+    dir1 = tmp_path / 'dir1'
+    dir1.mkdir()
+    dir2 = tmp_path / 'dir2'
+    dir2.mkdir()
+    console_script.write_text(
+        f"""
 import os
 print(os.getcwd())
-os.chdir('{}')
+os.chdir(R'''{dir2}''')
 print(os.getcwd())
-        """.format(dir2)
+        """
     )
     mydir = os.getcwd()
     result = script_runner.run(str(console_script), cwd=str(dir1))
     assert result.success
-    assert result.stdout == '{}\n{}\n'.format(dir1, dir2)
+    assert result.stdout == f'{dir1}\n{dir2}\n'
     assert os.getcwd() == mydir
 
 
 @pytest.mark.script_launch_mode('both')
-def test_env(console_script, script_runner):
+def test_env(console_script: Path, script_runner: ScriptRunner) -> None:
     """Script receives environment and env changes don't escape to test."""
-    console_script.write(
+    console_script.write_text(
         """
 import os
 print(os.environ['FOO'])
 os.environ['FOO'] = 'baz'
         """
     )
-    result = script_runner.run(str(console_script), env={'FOO': 'bar'})
+    env = os.environ.copy()
+    env['FOO'] = 'bar'
+    result = script_runner.run(str(console_script), env=env)
     assert result.success
     assert result.stdout == 'bar\n'
     assert 'FOO' not in os.environ
 
 
 @pytest.mark.script_launch_mode('both')
-def test_stdin(console_script, script_runner):
-    console_script.write(
+def test_stdin(console_script: Path, script_runner: ScriptRunner) -> None:
+    console_script.write_text(
         """
 import sys
 for line in sys.stdin:
     sys.stdout.write('simon says ' + line)
     sys.stderr.write('error says ' + line)
         """
     )
     stdin = io.StringIO('foo\nbar')
     result = script_runner.run(str(console_script), stdin=stdin)
     assert result.success
     assert result.stdout == 'simon says foo\nsimon says bar'
     assert result.stderr == 'error says foo\nerror says bar'
 
 
-def test_logging(console_script, script_runner):
+def test_logging(console_script: Path, script_runner: ScriptRunner) -> None:
     """Test that the script can perform logging initialization."""
-    console_script.write(
+    console_script.write_text(
         """
 import logging, sys
 logging.basicConfig(stream=sys.stderr, level=logging.INFO)
 logging.debug('hidden')
 logging.info('shown')
         """
     )
     result = script_runner.run(str(console_script))
     assert result.success
     assert result.stderr == 'INFO:root:shown\n'
 
 
 @pytest.mark.parametrize('fail', [True, False])
-def test_print_stdio_on_error(console_script, script_runner, tmpdir, fail,
-                              launch_mode):
+def test_print_stdio_on_error(
+    console_script: Path,
+    script_runner: ScriptRunner,
+    tmp_path: Path,
+    fail: bool,
+    launch_mode: str,
+) -> None:
     """Output of the script is printed when the test fails."""
-    console_script.write('print("12345")\nraise Exception("54321")')
-    test = tmpdir.join('test_{}_{}.py'.format(fail, launch_mode))
-    test.write(
-        """
+    console_script.write_text('print("12345")\nraise Exception("54321")')
+    test = tmp_path / f'test_{fail}_{launch_mode}.py'
+    test.write_text(
+        f"""
 def test_fail(script_runner):
-    ret = script_runner.run('{}', 'arg')
-    assert ret.success is {}
-        """.format(console_script, fail)
+    ret = script_runner.run(R'''{console_script}''', 'arg')
+    assert ret.success is {fail}
+        """
     )
     result = script_runner.run(
         'pytest',
         str(test),
         '--script-launch-mode=' + launch_mode,
     )
     assert result.success != fail
     if fail:
-        assert ('# Running console script: {} arg\n'.format(console_script)
+        assert (f'# Running console script: {console_script} arg\n'
                 in result.stdout)
         assert '# Script return code: 1\n' in result.stdout
         assert '# Script stdout:\n12345\n' in result.stdout
         assert '# Script stderr:\nTraceback' in result.stdout
         assert 'Exception: 54321' in result.stdout
     else:
         assert '# Running console script' not in result.stdout
         assert '12345' not in result.stdout
         assert '54321' not in result.stdout
 
 
 @pytest.mark.script_launch_mode('inprocess')
-def test_mocking(console_script, script_runner, monkeypatch):
+def test_mocking(
+    console_script: Path,
+    script_runner: ScriptRunner,
+    monkeypatch: pytest.MonkeyPatch
+) -> None:
     """Test mocking in of console scripts (in-process mode only).
 
     Note: we can't mock objects in the script itself because it will not be
     imported via normal import system but we can mock anything in the modules
     that the script imports.
 
     """
-    console_script.write(
+    console_script.write_text(
         """
 import os
 print(os.path.basename('foo'))
         """
     )
     monkeypatch.setattr(os.path, 'basename', lambda foo: 'bar')
     result = script_runner.run(str(console_script))
     assert result.success
     assert result.stdout == 'bar\n'
 
 
-def test_hide_run_result_arg(tmpdir, console_script, script_runner):
+def test_hide_run_result_arg(
+    tmp_path: Path, console_script: Path, script_runner: ScriptRunner
+) -> None:
     """Disable printing of the RunResult to stdout with print_result=False."""
-    console_script.write('print("the answer is 42")')
-    test = tmpdir.join('test_hrra.py')
-    test.write(
-        """
+    console_script.write_text('print("the answer is 42")')
+    test = tmp_path / 'test_hrra.py'
+    test.write_text(
+        f"""
 import pytest
 
 @pytest.mark.script_launch_mode('both')
 def test_script(script_runner):
-    script_runner.run('{}', print_result=False)
-        """.format(console_script)
+    script_runner.run(R'''{console_script}''', print_result=False)
+        """
     )
     result = script_runner.run('pytest', '-s', str(test))
     assert result.success
     assert 'the answer is 42' not in result.stdout
     assert 'Running console script' not in result.stdout
 
 
-def test_hide_run_result_opt(tmpdir, console_script, script_runner):
+def test_hide_run_result_opt(
+    tmp_path: Path, console_script: Path, script_runner: ScriptRunner
+) -> None:
     """Disable printing of the RunResult to stdout with print_result=False."""
-    console_script.write('print("the answer is 42")')
-    test = tmpdir.join('test_hrro.py')
-    test.write(
-        """
+    console_script.write_text('print("the answer is 42")')
+    test = tmp_path / 'test_hrro.py'
+    test.write_text(
+        f"""
 import pytest
 
 @pytest.mark.script_launch_mode('both')
 def test_script(script_runner):
-    script_runner.run('{}')
-        """.format(console_script)
+    script_runner.run(R'''{console_script}''')
+        """
     )
     result = script_runner.run('pytest', '-s', '--hide-run-results', str(test))
     assert result.success
     assert 'the answer is 42' not in result.stdout
     assert 'Running console script' not in result.stdout
 
 
 class MockEntryPoint:
-    def __init__(self, exec_path):
+    module: ModuleType
+
+    def __init__(self, exec_path: str | Path):
         self.exec_path = exec_path
-        self.module = None
 
-    def load(self):
+    def load(self) -> Any:
         base, module = os.path.split(self.exec_path)
         module_name, _ = os.path.splitext(module)
         sys.path.append(base)
         self.module = importlib.import_module(module_name)
         sys.path.pop(-1)
         return self.module.run
 
 
 @pytest.mark.script_launch_mode('inprocess')
-def test_global_logging(tmpdir, console_script, script_runner):
-    """Load global values when executing from pkg_resources"""
-    test = tmpdir.join('test_entry_point.py')
-    test.write(
+def test_global_logging(
+    tmp_path: Path, console_script: Path, script_runner: ScriptRunner
+) -> None:
+    """Load global values when executing from importlib.metadata"""
+    test = tmp_path / 'test_entry_point.py'
+    test.write_text(
         """
 import logging
 
 logging.basicConfig(level=logging.INFO)
 LOGGER = logging.getLogger(__name__)
 
 
-def run():
+def run() -> None:
     LOGGER.debug('DEBUG')
     LOGGER.info('INFO')
     LOGGER.warning('WARNING')
         """
     )
 
+    if sys.version_info < (3, 10):
+        patched_func = 'importlib_metadata.entry_points'
+    else:
+        patched_func = 'importlib.metadata.entry_points'
+
     with mock.patch(
-        'pkg_resources.iter_entry_points',
+        patched_func,
         mock.MagicMock(return_value=[MockEntryPoint(str(test))]),
     ):
         result = script_runner.run(str(console_script))
         assert result.success
         assert 'INFO:test_entry_point:INFO\n' in result.stderr
         assert 'DEBUG\n' not in result.stderr
+
+
+@pytest.mark.script_launch_mode('both')
+def test_shell(
+    console_script: Path, script_runner: ScriptRunner
+) -> None:
+    console_script.chmod(0o777)
+    result = script_runner.run(
+        f"{console_script} --test", shell=True, check=True
+    )
+    assert result.stdout == 'foo\n'
+    assert result.stderr == ''
+    result = script_runner.run(
+        [str(console_script), "--test"], shell=True, check=True
+    )
+    assert result.stdout == 'foo\n'
+    assert result.stderr == ''
+
+
+@pytest.mark.script_launch_mode('both')
+def test_deprecated_args(
+    console_script: Path, script_runner: ScriptRunner
+) -> None:
+    if (
+        script_runner.launch_mode == 'subprocess'
+        and sys.platform == 'win32'
+        and sys.version_info < (3, 8)
+    ):
+        pytest.xfail("PathLike's might not be supported this far back")
+    console_script.write_text(
+        """
+import sys
+print(sys.argv[1:])
+        """
+    )
+    result = script_runner.run(console_script, 'A', 'B', check=True)
+    assert result.stdout == "['A', 'B']\n"
+    result = script_runner.run([console_script, 'C'], 'D', check=True)
+    assert result.stdout == "['C', 'D']\n"
+
+
+@pytest.mark.script_launch_mode('both')
+def test_check(
+    console_script: Path, script_runner: ScriptRunner
+) -> None:
+    console_script.write_text("""import sys; sys.exit(1)""")
+    with pytest.raises(CalledProcessError, match='.*non-zero exit status 1'):
+        script_runner.run(str(console_script), check=True)
+
+
+@pytest.mark.script_launch_mode('both')
+def test_ignore_universal_newlines(
+    console_script: Path, script_runner: ScriptRunner
+) -> None:
+    result = script_runner.run(
+        str(console_script), check=True, universal_newlines=True
+    )
+    assert result.stdout == 'foo\n'
+    assert result.stderr == ''
+
+
+@pytest.mark.script_launch_mode('subprocess')
+def test_disable_universal_newlines(
+    console_script: Path, script_runner: ScriptRunner
+) -> None:
+    result = script_runner.run(
+        str(console_script), check=True, universal_newlines=False
+    )
+    assert isinstance(result.stdout, bytes)
+    assert isinstance(result.stderr, bytes)
+    assert result.stdout.strip() == b'foo'
+    assert result.stderr == b''
+
+
+@pytest.mark.script_launch_mode('both')
+def test_run_path(
+    console_script: Path, script_runner: ScriptRunner
+) -> None:
+    result = script_runner.run(console_script, check=True)
+    assert result.stdout == 'foo\n'
+    assert result.stderr == ''
+    console_script.chmod(0o777)
+    result = script_runner.run(console_script, check=True)
+    assert result.stdout == 'foo\n'
+    assert result.stderr == ''
```

