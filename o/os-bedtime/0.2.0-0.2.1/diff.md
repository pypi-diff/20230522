# Comparing `tmp/os_bedtime-0.2.0.tar.gz` & `tmp/os_bedtime-0.2.1.tar.gz`

## Comparing `os_bedtime-0.2.0.tar` & `os_bedtime-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 os_bedtime-0.2.0/.vscode/tasks.json
--rw-r--r--   0        0        0     8893 2020-02-02 00:00:00.000000 os_bedtime-0.2.0/src/os_bedtime/__init__.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 os_bedtime-0.2.0/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 os_bedtime-0.2.0/LICENSE
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 os_bedtime-0.2.0/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 os_bedtime-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 os_bedtime-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 os_bedtime-0.2.1/.vscode/tasks.json
+-rw-r--r--   0        0        0     8992 2020-02-02 00:00:00.000000 os_bedtime-0.2.1/src/os_bedtime/__init__.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 os_bedtime-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 os_bedtime-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 os_bedtime-0.2.1/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 os_bedtime-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 os_bedtime-0.2.1/PKG-INFO
```

### Comparing `os_bedtime-0.2.0/src/os_bedtime/__init__.py` & `os_bedtime-0.2.1/src/os_bedtime/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         if force: command += " --force"
         if message != "": command+=f' --message={message}'
     elif psutil.WINDOWS:
         command = "shutdown"
         command += " /r" if reboot else " /s"
         if force: command += " /f"
         if seconds_delay > 0: command += f" /t {int(seconds_delay)}"
-        if message != "": command += f' /c {message}'
+        if message != '': command += f' /c "{message}"'
         os.system(command)
     else:
         raise RuntimeError("I have no implementation for that operating system :'(")
 def computer_lock() -> None:
     """Locks your computer.
     
     Implemented for WINDOWS.
@@ -208,9 +208,10 @@
     for listener in listeners:
         listener.stop_thread()
     for listener in listeners:
         listener.join()
 
     # Returns True if listener triggered
     return did_trigger
-# if __name__ == '__main__':
+if __name__ == '__main__':
+    computer_shutdown(seconds_delay=60, message='Whoa! You scared me! What is wrong with you???')
 #     print(computer_hostage(lambda:print('Payload trigger example'), timeout_seconds=5, verbose=True))
```

### Comparing `os_bedtime-0.2.0/.gitignore` & `os_bedtime-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `os_bedtime-0.2.0/LICENSE` & `os_bedtime-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `os_bedtime-0.2.0/README.md` & `os_bedtime-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `os_bedtime-0.2.0/pyproject.toml` & `os_bedtime-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling","psutil","pynput"]
 build-backend = "hatchling.build"
 [project]
 name = "os_bedtime"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Holandsoest", email="holandsoest@gmail.com" },
 ]
 description = "Put your computer to sleep, etc."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `os_bedtime-0.2.0/PKG-INFO` & `os_bedtime-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os_bedtime
-Version: 0.2.0
+Version: 0.2.1
 Summary: Put your computer to sleep, etc.
 Project-URL: Homepage, https://github.com/Holandsoest/os_bedtime
 Project-URL: Bug Tracker, https://github.com/Holandsoest/os_bedtime/issues
 Author-email: Holandsoest <holandsoest@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

