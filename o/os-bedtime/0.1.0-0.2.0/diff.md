# Comparing `tmp/os_bedtime-0.1.0.tar.gz` & `tmp/os_bedtime-0.2.0.tar.gz`

## Comparing `os_bedtime-0.1.0.tar` & `os_bedtime-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 os_bedtime-0.1.0/src/os_bedtime/__init__.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 os_bedtime-0.1.0/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 os_bedtime-0.1.0/LICENSE
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 os_bedtime-0.1.0/README.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 os_bedtime-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 os_bedtime-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 os_bedtime-0.2.0/.vscode/tasks.json
+-rw-r--r--   0        0        0     8893 2020-02-02 00:00:00.000000 os_bedtime-0.2.0/src/os_bedtime/__init__.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 os_bedtime-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 os_bedtime-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 os_bedtime-0.2.0/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 os_bedtime-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 os_bedtime-0.2.0/PKG-INFO
```

### Comparing `os_bedtime-0.1.0/.gitignore` & `os_bedtime-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `os_bedtime-0.1.0/LICENSE` & `os_bedtime-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `os_bedtime-0.1.0/README.md` & `os_bedtime-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,36 +9,36 @@
 Currently this module is yet in the major version **0.x.x** and with that in mind the interface might change at any time.  
 It is kept in mind to make changes as little as possible, but it is not out of question that things might brake during early access.  
 
 If you feel like contributing. (OSX or Linux or improvements for Windows even) Let me know in an issue.  
 
 ## How to install
 
-TBA
+`pip install os-bedtime`  
 
 ## **Issue:** Sleep issues
 
 Your computer might be waking from sleep mode because certain peripheral devices, such as a mouse, a keyboard, or headphones are plugged into a USB port or connected via Bluetooth. It might also be caused by an app or a wake timer.
 
 ### **Windows:** Turn off wake-timers
 
-> Wake timers are timers that may wake your computer on a set time. Disabling this make this impossible until you re-enable > it.  
+> Wake timers are timers that may wake your computer on a set time. Disabling this make this impossible until you re-enable it.  
 > *If you use wake-timers to automatically wake your computer at 7 am or something, this will not work anymore.*
 > 
 > 1. Right-click Windows button. Select `Energy-management`  
 > 2. Scroll down and click the link for `Extra energy-settings`  
 > 3. Click the `Change power-plan` to the right of the currently selected power-plan  
 > 4. Click the `Change advanced energy-settings` link  
 > 5. Scroll and find `Sleep` -> `Allow activation timers`  
 > 6. Set it to `No` or `Disabled`  
 
 ### **Windows:** Turn off peripheral-devices access to wake your pc
 
 > Peripheral-devices (like for example your keyboard) have access to wake your computer out of sleep-mode.
-> For something like a keyboard this makes sense. You press the spacebar and the computer wakes up, but there are other devices where this might make less sense. For example a network device may wake your computer?
+> For something like a keyboard this makes sense. You press the space-bar and the computer wakes up, but there are other devices where this might make less sense. For example a network device may wake your computer?
 > 
 > 1. left-click the windows button. Type `CMD` and choose `Run as administrator`  
 > 2. It will prompt you if you did this and allow this... Allow  
 > 3. Type in the console `powercfg -devicequery wake_armed` and press enter  
 > 4. It gives you a list of all your peripheral devices that may wake up your computer out of sleep mode  
 > 5. Right-click Windows button. Select `Device-management`  
 > 6. Find all the devices (or the onces you want to disable), in the list and double-click them
```

### Comparing `os_bedtime-0.1.0/pyproject.toml` & `os_bedtime-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
-requires = ["hatchling","psutil"]
+requires = ["hatchling","psutil","pynput"]
 build-backend = "hatchling.build"
 [project]
 name = "os_bedtime"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Holandsoest", email="holandsoest@gmail.com" },
 ]
 description = "Put your computer to sleep, etc."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `os_bedtime-0.1.0/PKG-INFO` & `os_bedtime-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os_bedtime
-Version: 0.1.0
+Version: 0.2.0
 Summary: Put your computer to sleep, etc.
 Project-URL: Homepage, https://github.com/Holandsoest/os_bedtime
 Project-URL: Bug Tracker, https://github.com/Holandsoest/os_bedtime/issues
 Author-email: Holandsoest <holandsoest@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,36 +23,36 @@
 Currently this module is yet in the major version **0.x.x** and with that in mind the interface might change at any time.  
 It is kept in mind to make changes as little as possible, but it is not out of question that things might brake during early access.  
 
 If you feel like contributing. (OSX or Linux or improvements for Windows even) Let me know in an issue.  
 
 ## How to install
 
-TBA
+`pip install os-bedtime`  
 
 ## **Issue:** Sleep issues
 
 Your computer might be waking from sleep mode because certain peripheral devices, such as a mouse, a keyboard, or headphones are plugged into a USB port or connected via Bluetooth. It might also be caused by an app or a wake timer.
 
 ### **Windows:** Turn off wake-timers
 
-> Wake timers are timers that may wake your computer on a set time. Disabling this make this impossible until you re-enable > it.  
+> Wake timers are timers that may wake your computer on a set time. Disabling this make this impossible until you re-enable it.  
 > *If you use wake-timers to automatically wake your computer at 7 am or something, this will not work anymore.*
 > 
 > 1. Right-click Windows button. Select `Energy-management`  
 > 2. Scroll down and click the link for `Extra energy-settings`  
 > 3. Click the `Change power-plan` to the right of the currently selected power-plan  
 > 4. Click the `Change advanced energy-settings` link  
 > 5. Scroll and find `Sleep` -> `Allow activation timers`  
 > 6. Set it to `No` or `Disabled`  
 
 ### **Windows:** Turn off peripheral-devices access to wake your pc
 
 > Peripheral-devices (like for example your keyboard) have access to wake your computer out of sleep-mode.
-> For something like a keyboard this makes sense. You press the spacebar and the computer wakes up, but there are other devices where this might make less sense. For example a network device may wake your computer?
+> For something like a keyboard this makes sense. You press the space-bar and the computer wakes up, but there are other devices where this might make less sense. For example a network device may wake your computer?
 > 
 > 1. left-click the windows button. Type `CMD` and choose `Run as administrator`  
 > 2. It will prompt you if you did this and allow this... Allow  
 > 3. Type in the console `powercfg -devicequery wake_armed` and press enter  
 > 4. It gives you a list of all your peripheral devices that may wake up your computer out of sleep mode  
 > 5. Right-click Windows button. Select `Device-management`  
 > 6. Find all the devices (or the onces you want to disable), in the list and double-click them
```

