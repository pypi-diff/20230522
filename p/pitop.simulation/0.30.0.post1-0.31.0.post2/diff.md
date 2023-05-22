# Comparing `tmp/pitop.simulation-0.30.0.post1.tar.gz` & `tmp/pitop.simulation-0.31.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.simulation-0.30.0.post1.tar", last modified: Fri Dec 16 14:08:47 2022, max compression
+gzip compressed data, was "dist/pitop.simulation-0.31.0.post2.tar", last modified: Mon May 22 19:13:14 2023, max compression
```

## Comparing `pitop.simulation-0.30.0.post1.tar` & `pitop.simulation-0.31.0.post2.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:47.000000 pitop.simulation-0.30.0.post1/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1027 2022-12-16 14:08:47.000000 pitop.simulation-0.30.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      181 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:47.000000 pitop.simulation-0.30.0.post1/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:47.000000 pitop.simulation-0.30.0.post1/pitop/simulation/
--rw-r--r--   0 runner    (1001) docker     (122)      195 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      310 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/events.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:47.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/
--rw-r--r--   0 runner    (1001) docker     (122)     6176 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/Button.png
--rw-r--r--   0 runner    (1001) docker     (122)     6304 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/Button_pressed.png
--rw-r--r--   0 runner    (1001) docker     (122)     6353 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/Buzzer.png
--rw-r--r--   0 runner    (1001) docker     (122)     5809 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/LED_green_off.png
--rw-r--r--   0 runner    (1001) docker     (122)     6237 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/LED_green_on.png
--rw-r--r--   0 runner    (1001) docker     (122)     5669 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/LED_red_off.png
--rw-r--r--   0 runner    (1001) docker     (122)     5115 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/LED_red_on.png
--rw-r--r--   0 runner    (1001) docker     (122)     5749 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/LED_yellow_off.png
--rw-r--r--   0 runner    (1001) docker     (122)     5172 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/LED_yellow_on.png
--rw-r--r--   0 runner    (1001) docker     (122)     7143 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/LightSensor.png
--rw-r--r--   0 runner    (1001) docker     (122)   121264 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/Pitop.png
--rw-r--r--   0 runner    (1001) docker     (122)     7857 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/Potentiometer.png
--rw-r--r--   0 runner    (1001) docker     (122)     1866 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/Readme.md
--rw-r--r--   0 runner    (1001) docker     (122)     9412 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/SoundSensor.png
--rw-r--r--   0 runner    (1001) docker     (122)    14445 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/UltrasonicSensor.png
--rw-r--r--   0 runner    (1001) docker     (122)      936 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/angle_icon.png
--rw-r--r--   0 runner    (1001) docker     (122)     2352 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/buzzer_sound_icon.png
--rw-r--r--   0 runner    (1001) docker     (122)      655 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/distance_icon.png
--rw-r--r--   0 runner    (1001) docker     (122)     1128 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/lightbulb_icon.png
--rw-r--r--   0 runner    (1001) docker     (122)      685 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/images/speaker_icon.png
--rw-r--r--   0 runner    (1001) docker     (122)     4440 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/simsprite.py
--rw-r--r--   0 runner    (1001) docker     (122)     8061 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)    10131 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/sprites.py
--rw-r--r--   0 runner    (1001) docker     (122)       80 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:47.000000 pitop.simulation-0.30.0.post1/pitop/simulation/virtual_hardware/
--rw-r--r--   0 runner    (1001) docker     (122)      497 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/virtual_hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      863 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/virtual_hardware/fonts.py
--rw-r--r--   0 runner    (1001) docker     (122)     2610 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/virtual_hardware/pitop.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:47.000000 pitop.simulation-0.30.0.post1/pitop/simulation/virtual_hardware/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:47.000000 pitop.simulation-0.30.0.post1/pitop/simulation/virtual_hardware/vendor/Mock/
--rw-r--r--   0 runner    (1001) docker     (122)     8181 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/virtual_hardware/vendor/Mock/GPIO.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/virtual_hardware/vendor/Mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/virtual_hardware/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:47.000000 pitop.simulation-0.30.0.post1/pitop/simulation/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)       77 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/widgets/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     4969 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (122)     2123 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/pitop/simulation/widgets/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:47.000000 pitop.simulation-0.30.0.post1/pitop.simulation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1027 2022-12-16 14:08:47.000000 pitop.simulation-0.30.0.post1/pitop.simulation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1645 2022-12-16 14:08:47.000000 pitop.simulation-0.30.0.post1/pitop.simulation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-16 14:08:47.000000 pitop.simulation-0.30.0.post1/pitop.simulation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2022-12-16 14:08:47.000000 pitop.simulation-0.30.0.post1/pitop.simulation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-12-16 14:08:47.000000 pitop.simulation-0.30.0.post1/pitop.simulation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-16 14:08:47.000000 pitop.simulation-0.30.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1989 2022-12-16 14:07:48.000000 pitop.simulation-0.30.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop/simulation/
+-rw-r--r--   0 runner    (1001) docker     (122)      195 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/color.py
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/events.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/
+-rw-r--r--   0 runner    (1001) docker     (122)     6176 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/Button.png
+-rw-r--r--   0 runner    (1001) docker     (122)     6304 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/Button_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (122)     6353 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/Buzzer.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5809 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_green_off.png
+-rw-r--r--   0 runner    (1001) docker     (122)     6237 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_green_on.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5669 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_red_off.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5115 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_red_on.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_yellow_off.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5172 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_yellow_on.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7143 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/LightSensor.png
+-rw-r--r--   0 runner    (1001) docker     (122)   121264 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/Pitop.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7857 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/Potentiometer.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1866 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (122)     9412 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/SoundSensor.png
+-rw-r--r--   0 runner    (1001) docker     (122)    14445 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/UltrasonicSensor.png
+-rw-r--r--   0 runner    (1001) docker     (122)      936 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/angle_icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/buzzer_sound_icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/distance_icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1128 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/lightbulb_icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/speaker_icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1714 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/port_label.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4685 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/simsprite.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9453 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12342 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/sprites.py
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      863 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2610 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/pitop.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/vendor/Mock/
+-rw-r--r--   0 runner    (1001) docker     (122)     8181 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/vendor/Mock/GPIO.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/vendor/Mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop/simulation/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/widgets/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     4969 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2123 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/widgets/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop.simulation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop.simulation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop.simulation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop.simulation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop.simulation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop.simulation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1989 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/setup.py
```

### Comparing `pitop.simulation-0.30.0.post1/PKG-INFO` & `pitop.simulation-0.31.0.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.simulation
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Simulation
```

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/Button.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/Button.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/Button_pressed.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/Button_pressed.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/Buzzer.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/Buzzer.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/LED_green_off.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_green_off.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/LED_green_on.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_green_on.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/LED_red_off.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_red_off.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/LED_red_on.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_red_on.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/LED_yellow_off.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_yellow_off.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/LED_yellow_on.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_yellow_on.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/LightSensor.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/LightSensor.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/Pitop.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/Pitop.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/Potentiometer.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/Potentiometer.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/Readme.md` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/Readme.md`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/SoundSensor.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/SoundSensor.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/UltrasonicSensor.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/UltrasonicSensor.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/__init__.py` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/__init__.py`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/angle_icon.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/angle_icon.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/buzzer_sound_icon.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/buzzer_sound_icon.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/distance_icon.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/distance_icon.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/lightbulb_icon.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/lightbulb_icon.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/images/speaker_icon.png` & `pitop.simulation-0.31.0.post2/pitop/simulation/images/speaker_icon.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/simsprite.py` & `pitop.simulation-0.31.0.post2/pitop/simulation/simsprite.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         center = int(sim_size[0] / 2), int(sim_size[1] / 2)
         sprite.set_pos(
             center[0] - int(sprite.rect.width / 2),
             center[1] - int(sprite.rect.height / 2),
         )
 
         sprite_group.add(sprite)
-        return sprite_group
+        return sprite_group, sprite
 
     @staticmethod
     def handle_sim_event(e: SimEvent, component):
         pass
 
     def handle_pygame_event(self, e: pygame.event.Event):
         pass
@@ -64,41 +64,48 @@
 
 
 class ComponentableSimSprite(SimSprite):
     Size = PITOP_SIM_SIZE
 
     @classmethod
     def create_sprite_group(cls, sim_size, config, scale):
-        sprite_group = super().create_sprite_group(sim_size, config, scale)
+        sprite_group, main_sprite = super().create_sprite_group(sim_size, config, scale)
 
-        main_sprite_rect = sprite_group.sprites()[0].rect
-        sprite_centres = cls._generate_sprite_centres(sim_size, main_sprite_rect)
+        sprite_centres = cls._generate_sprite_centres(sim_size, main_sprite.rect)
+        main_sprite.sprite_centres = sprite_centres
 
         components = config.get("components", {})
         for component in components.values():
-            sprite_class = getattr(Sprites, component.get("classname"), None)
+            component_sprite = main_sprite.create_child_sprite(component, scale)
+            if component_sprite is not None:
+                sprite_group.add(component_sprite)
 
-            if not sprite_class:
-                continue
+        return sprite_group, main_sprite
 
-            sprite = sprite_class(component, scale)
-            if not sprite:
-                continue
+    def create_child_sprite(self, component, scale):
+        sprite_class = getattr(Sprites, component.get("classname"), None)
 
-            sprite_centre = sprite_centres.get(component.get("port_name", None), (0, 0))
+        if not sprite_class:
+            return None
 
-            sprite.set_pos(
-                sprite_centre[0] - int(sprite.rect.width / 2),
-                sprite_centre[1] - int(sprite.rect.height / 2),
-            )
+        sprite = sprite_class(component, scale, draw_port=True)
+        if not sprite:
+            return None
 
-            sprite.name = component.get("name")
-            sprite_group.add(sprite)
+        sprite_centre = self.sprite_centres.get(
+            component.get("port_name", None), (0, 0)
+        )
+
+        sprite.set_pos(
+            sprite_centre[0] - int(sprite.rect.width / 2),
+            sprite_centre[1] - int(sprite.rect.height / 2),
+        )
 
-        return sprite_group
+        sprite.name = component.get("name")
+        return sprite
 
     @staticmethod
     def handle_sim_event(e: SimEvent, component):
         for _, child in component.children_gen():
             sprite_class = getattr(Sprites, child.config.get("classname"), None)
             if not sprite_class:
                 continue
```

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/simulation.py` & `pitop.simulation-0.31.0.post2/pitop/simulation/simulation.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
         self.component = component
         self.scale = scale or 1  # full scale is approx life size
         self.size = size
 
         # communication channels between main process and sim
         self._stop_ev = Event()  # stopping this simulation
+        self._config_q = Queue()  # sending component config updates into sim
         self._state_q = Queue()  # sending component state updates into sim
         self._out_event_q = Queue()  # sending sim events to components
         self._in_event_q = Queue()  # artificially firing pygame events (tests)
         self._snapshot_ev = Event()  # requesting sim snapshot images
         self._snapshot_q = Queue()  # returning snapshot images
 
         # pygame must be run in another process as it is designed to use the
@@ -55,14 +56,15 @@
         self._process = Process(
             target=_run,
             args=(
                 self.component.config,
                 self.scale,
                 self.size,
                 self._stop_ev,
+                self._config_q,
                 self._state_q,
                 self._out_event_q,
                 self._in_event_q,
                 self._snapshot_ev,
                 self._snapshot_q,
             ),
         )
@@ -86,33 +88,42 @@
         return self._snapshot_q.get()
 
     def event(self, type, target):
         # send a pygame event into the sim to simulate interactions for tests
         self._in_event_q.put((type, target))
 
     def __communicate(self):
+        # store config as a string (not reference) to easily check if it's changed
+        str_config = str(self.component.config)
+
         while True:
             if self._stop_ev.is_set():
                 break
 
             if self._process is None or not self._process.is_alive():
                 break
 
-            # update the sim with the current state of the simulated component
+            # update sim with current state of simulated component
             self._state_q.put(self.component.state)
 
+            # update sim with current config only if it's changed
+            if str(self.component.config) != str_config:
+                str_config = str(self.component.config)
+                self._config_q.put(self.component.config)
+
             # handle events produced by the sim which affect our simulated
             # component (eg PMA Button presses, sensor slider updates)
             while not self._out_event_q.empty():
                 sim_event = self._out_event_q.get_nowait()
                 self._main_sprite_class.handle_sim_event(
                     sim_event,
                     self.component,
                 )
 
+            # sleep - timed to match pygame loop
             sleep(0.05)
 
         self.stop()
 
 
 def to_bytes(surface):
     image_string = pygame.image.tostring(surface, "RGB")
@@ -123,14 +134,15 @@
 
 
 def _run(
     config,
     scale,
     size,
     stop_ev,
+    config_q,
     state_q,
     out_event_q,
     in_event_q,
     snapshot_ev,
     snapshot_q,
 ):
     # the pygame application - this should be a separate python process
@@ -141,17 +153,18 @@
     sprite_class = getattr(Sprites, config.get("classname"))
     size = size or multiply_scalar(scale, sprite_class.Size)
 
     screen = pygame.display.set_mode(size)
     screen.fill((255, 255, 255))
 
     # create our sprites based on the simulated component's config
-    sprite_group = sprite_class.create_sprite_group(size, config, scale)
+    sprite_group, main_sprite = sprite_class.create_sprite_group(size, config, scale)
 
     while not stop_ev.is_set():
+        # handle pygame events eg UI
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
                 stop_ev.set()
                 break
 
             # mouse events are dispatched to our sprite.handle_pygame_event
             # methods for UI uses, such as activating slider inputs...
@@ -174,51 +187,69 @@
                     if (
                         rect.x <= pos[0] <= rect.x + rect.width
                         and rect.y <= pos[1] <= rect.y + rect.height
                     ):
                         sprite.handle_pygame_event(event)
                         out_event_q.put(SimEvent(SimEventTypes.MOUSE_DOWN, sprite.name))
 
+        # send out postion update events for selected sliders
         for sprite in sprite_group.sprites():
             if hasattr(sprite, "slider") and sprite.slider.selected:
                 out_event_q.put(
                     SimEvent(
                         SimEventTypes.SLIDER_UPDATE,
                         sprite.name,
                         sprite.slider.value,
                     )
                 )
 
+        # handle incoming simulated ui events
         while not in_event_q.empty():
             # find which sprite matches the target_name and translate to target
             # the event at that sprite's position in the simulation
             type, target_name = in_event_q.get_nowait()
             target = [s for s in sprite_group.sprites() if s.name == target_name]
             if not len(target):
                 continue
             pos = (target[0].rect.x, target[0].rect.y)
             event = pygame.event.Event(
                 type, {"pos": pos, "button": 1, "touch": False, "window": None}
             )
             pygame.event.post(event)
 
+        # respond to screenshot requests
         if snapshot_ev.is_set():
             snapshot_q.put(to_bytes(screen))
             snapshot_ev.clear()
 
+        # check changes to component config eg newly added sprites
+        while not config_q.empty():
+            new_config = config_q.get_nowait()
+            components = new_config.get("components", {})
+
+            sprite_names = [sprite.name for sprite in sprite_group.sprites()]
+
+            for component in components.values():
+                if component.get("name") not in sprite_names:
+                    component_sprite = main_sprite.create_child_sprite(component, scale)
+                    sprite_group.add(component_sprite)
+
+        # forward inbound component state updates
         while not state_q.empty():
             # provide sprites with relevant part of the component state tree
             state = state_q.get_nowait()
             for sprite in sprite_group.sprites():
                 if sprite.name == "main":
                     sprite.state = state
                 else:
                     sprite.state = state.get(sprite.name)
 
+        # draw
         sprite_group.update()
         sprite_group.draw(screen)
         pygame.display.flip()
 
+        # sleep - timed to match controlling thread
         clock.tick(20)
 
     # Don't pygame.quit() - isn't needed and can cause X server to crash
     sys.exit()
```

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/sprites.py` & `pitop.simulation-0.31.0.post2/pitop/simulation/sprites.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from dataclasses import dataclass
 from typing import Any, Tuple
 
 import pygame
 
 from . import images as Images
+from .color import PitopColorScheme
 from .events import SimEvent, SimEventTypes
 from .images import PMA_CUBE_SIZE
+from .port_label import PortLabel
 from .simsprite import ComponentableSimSprite, SimSprite
 from .utils import multiply_scalar
 from .virtual_hardware import is_virtual_hardware
 from .widgets.slider import Slider
 
 MARGIN = 10
 SLIDER_WIDTH = 85
-SLIDER_HORIZONTAL_OFFSET = int((PMA_CUBE_SIZE[0] - SLIDER_WIDTH) / 2)
 SLIDER_HEIGHT = 8
 SLIDER_HANDLE_RADIUS = 8
 FONT_SIZE = 22
 TEXT_OFFSET = (-13, 8)
 
 
 class Pitop(pygame.sprite.Sprite, ComponentableSimSprite):
@@ -42,45 +43,67 @@
             )
             size = multiply_scalar(self.scale, rgb.size)
             image = pygame.transform.scale(miniscreen_surface, size)
             self.image.blit(image, self.miniscreen_pos)
 
 
 class LED(pygame.sprite.Sprite, SimSprite):
-    def __init__(self, config, scale):
+    def __init__(self, config, scale, draw_port=False):
         pygame.sprite.Sprite.__init__(self)
 
         self.color = config.get("color", "red")
         self.off_image = SimSprite._load_image(
             getattr(Images, f"LED_{self.color}_off"), scale
         )
         self.on_image = SimSprite._load_image(
             getattr(Images, f"LED_{self.color}_on"), scale
         )
 
+        if draw_port:
+            self.Size = (self.Size[0], self.Size[1] + PortLabel.height + MARGIN)
+            port_label = PortLabel(
+                config.get("port_name"),
+                self.Size,
+                scale,
+                pos=(int(self.Size[0]) / 2 - 40, PortLabel.height),
+            )
+            self.on_image = port_label.render(self.on_image)
+            self.off_image = port_label.render(self.off_image)
+
         self.image = self.off_image
         self.rect = self.image.get_rect()
 
     def update(self):
         if not hasattr(self, "state"):
             return
 
         if self.state.get("value", False):
             self.image = self.on_image
         else:
             self.image = self.off_image
 
 
 class Button(pygame.sprite.Sprite, SimSprite):
-    def __init__(self, config, scale):
+    def __init__(self, config, scale, draw_port=False):
         pygame.sprite.Sprite.__init__(self)
 
         self.released_image = SimSprite._load_image(Images.Button, scale)
         self.pressed_image = SimSprite._load_image(Images.Button_pressed, scale)
 
+        if draw_port:
+            self.Size = (self.Size[0], self.Size[1] + PortLabel.height + MARGIN)
+            port_label = PortLabel(
+                config.get("port_name"),
+                self.Size,
+                scale,
+                pos=(int(self.Size[0]) / 2 - 40, PortLabel.height),
+            )
+            self.released_image = port_label.render(self.released_image)
+            self.pressed_image = port_label.render(self.pressed_image)
+
         self.image = self.released_image
         self.rect = self.image.get_rect()
 
     def update(self):
         if not hasattr(self, "state"):
             return
 
@@ -99,17 +122,17 @@
             component.pin.drive_low()
 
         elif e.type == SimEventTypes.MOUSE_UP:
             component.pin.drive_high()
 
 
 class Buzzer(pygame.sprite.Sprite, SimSprite):
-    Size = ((PMA_CUBE_SIZE[0] + 2 * MARGIN) * 2, PMA_CUBE_SIZE[0] + 2 * MARGIN)
+    Size = ((PMA_CUBE_SIZE[0]) * 2, PMA_CUBE_SIZE[0])
 
-    def __init__(self, config, scale):
+    def __init__(self, config, scale, draw_port=False):
         pygame.sprite.Sprite.__init__(self)
 
         def get_pos(image):
             return (
                 int((self.Size[0] * scale - image.get_width()) / 2),
                 int((self.Size[1] * scale - image.get_height()) / 2),
             )
@@ -118,26 +141,47 @@
         self.component_pos = get_pos(self.component_image)
 
         self.buzzer_sound_image = SimSprite._load_image(Images.buzzer_sound_icon, scale)
         self.buzzer_sound_image_pos = get_pos(self.buzzer_sound_image)
 
         self.base_image = pygame.Surface(multiply_scalar(scale, self.Size))
         self.base_image.fill(pygame.Color("WHITE"))
+
+        if draw_port:
+            label_height = PortLabel.height + MARGIN
+            self.Size = (self.Size[0], self.Size[1] + label_height)
+            port_label = PortLabel(
+                config.get("port_name"),
+                self.Size,
+                scale,
+                pos=(int(self.Size[0]) / 2 - 30, PortLabel.height),
+            )
+            self.base_image = port_label.render(self.base_image)
+            self.component_pos = (
+                self.component_pos[0],
+                self.component_pos[1] + scale * label_height,
+            )
+            self.buzzer_sound_image_pos = (
+                self.buzzer_sound_image_pos[0],
+                self.buzzer_sound_image_pos[1] + scale * label_height,
+            )
+
         self.rect = self.base_image.get_rect()
 
     def render(self):
         value = False
         if hasattr(self, "state"):
             value = self.state.get("value", False)
 
         image = self.base_image.copy()
         if value:
             image.blit(self.buzzer_sound_image, self.buzzer_sound_image_pos)
 
         image.blit(self.component_image, self.component_pos)
+
         return image
 
     def update(self):
         if not hasattr(self, "state"):
             return
 
         self.image = self.render()
@@ -149,109 +193,131 @@
     obj: Any
 
 
 class SliderSensorSprite(pygame.sprite.Sprite, SimSprite):
     slider: Slider
     font: Component
     icon: Component
+    img: Component
     scale: float
 
     image: str
     icon: str
     measurement_key_in_state: str
     min_value: int = 0
     max_value: int = 999
     slider_step: int = 1
 
-    def __init__(self, config, scale):
+    def __init__(self, config, scale, draw_port=False):
         pygame.sprite.Sprite.__init__(self)
         self.scale = scale
 
-        self.create_components()
+        self.port_label = None
+        if draw_port:
+            self.Size = (self.Size[0], self.Size[1] + PortLabel.height + MARGIN)
+            self.port_label = PortLabel(config.get("port_name"), self.Size, scale)
 
+        self.create_components()
         assert self.slider is not None
         assert self.font is not None
         assert self.icon is not None
+        assert self.img is not None
 
         self.base_image = self.draw_base_image()
 
         if not is_virtual_hardware():
             self.slider.disable()
 
         self.image = self.render()
         self.rect = self.image.get_rect()
 
     def create_components(self):
-        right_hand_side_x_start = self.Size[0] - MARGIN - PMA_CUBE_SIZE[0]
+        label_height = (
+            self.scale * (PortLabel.height + MARGIN) if self.port_label else 0
+        )
+        right_hand_side_x_start = self.Size[0] - SLIDER_WIDTH - SLIDER_HANDLE_RADIUS - 1
 
         slider_pos = (
-            right_hand_side_x_start + SLIDER_HORIZONTAL_OFFSET,
-            self.Size[1] - 2 * MARGIN - SLIDER_HEIGHT,
+            right_hand_side_x_start,
+            self.Size[1] - MARGIN - SLIDER_HEIGHT,
         )
         slider_pos = multiply_scalar(self.scale, slider_pos)
 
         self.slider = Slider(
             x=slider_pos[0],
             y=slider_pos[1],
             width=int(SLIDER_WIDTH * self.scale),
             height=int(SLIDER_HEIGHT * self.scale),
             min=self.min_value,
             max=self.max_value,
             step=self.slider_step,
             initial=0,
             handleRadius=int(SLIDER_HANDLE_RADIUS * self.scale),
-            handleColour=pygame.Color("#505050"),
-            colour=pygame.Color("#DBDEE0"),
+            handleColour=pygame.Color(PitopColorScheme.CHARCOAL),
+            colour=pygame.Color(PitopColorScheme.GRAY),
         )
 
         text_pos = (
             slider_pos[0] + self.slider.width / 2 + TEXT_OFFSET[0] * self.scale,
             slider_pos[1] - MARGIN * 2 * self.scale,
         )
 
         self.font = Component(
             text_pos, pygame.font.SysFont(None, int(FONT_SIZE * self.scale))
         )
 
         icon_image = SimSprite._load_image(self.icon, self.scale)
         icon_pos = (
             slider_pos[0] + self.slider.width / 2 - icon_image.get_width() / 2,
-            text_pos[1] - icon_image.get_height() - self.scale * MARGIN / 2,
+            text_pos[1]
+            - icon_image.get_height()
+            - self.scale * MARGIN / 2
+            - label_height,
         )
         self.icon = Component(icon_pos, icon_image)
 
-    def draw_base_image(self):
-        component_image = SimSprite._load_image(self.image, self.scale)
+        self.img = Component(
+            (0, 0),
+            SimSprite._load_image(self.image, self.scale),
+        )
 
+    def draw_base_image(self):
         base_image = pygame.Surface(multiply_scalar(self.scale, self.Size))
         base_image.fill(pygame.Color("WHITE"))
-        base_image.blit(component_image, multiply_scalar(self.scale, (MARGIN, MARGIN)))
+        base_image.blit(self.img.obj, self.img.pos)
         base_image.blit(self.icon.obj, self.icon.pos)
+
+        if self.port_label:
+            base_image = self.port_label.render(base_image)
+
         return base_image
 
     def set_pos(self, x, y):
         super().set_pos(x, y)
         self.slider.parent_x = x
         self.slider.parent_y = y
 
     def render(self):
         value = 0
         if hasattr(self, "state"):
             value = self.state.get(self.measurement_key_in_state, 0)
 
         image = self.base_image.copy()
         image.blit(
-            self.font.obj.render(str(value), True, pygame.Color("#505050")),
+            self.font.obj.render(
+                str(value), True, pygame.Color(PitopColorScheme.CHARCOAL)
+            ),
             self.font.pos,
         )
 
         if not self.slider.selected:
             self.slider.value = value
 
         self.slider.draw(image)
+
         return image
 
     def update(self):
         if not hasattr(self, "state"):
             return
 
         self.slider.update()
@@ -269,22 +335,22 @@
             component.read.return_value = e.value
 
     def handle_pygame_event(self, e: pygame.event.Event):
         self.slider.handle_event(e)
 
 
 class LightSensor(SliderSensorSprite):
-    Size = (PMA_CUBE_SIZE[0] * 2 + MARGIN * 3, PMA_CUBE_SIZE[1] + 2 * MARGIN)
+    Size = (PMA_CUBE_SIZE[0] * 2 + MARGIN, PMA_CUBE_SIZE[1])
     image = Images.LightSensor
     measurement_key_in_state = "reading"
     icon = Images.lightbulb_icon
 
 
 class SoundSensor(SliderSensorSprite):
-    Size = (PMA_CUBE_SIZE[0] * 2 + MARGIN * 3, PMA_CUBE_SIZE[1] + 2 * MARGIN)
+    Size = (PMA_CUBE_SIZE[0] * 2 + MARGIN, PMA_CUBE_SIZE[1])
     image = Images.SoundSensor
     max_value = 500
     measurement_key_in_state = "reading"
     icon = Images.speaker_icon
 
     @staticmethod
     def handle_sim_event(e: SimEvent, component):
@@ -298,22 +364,22 @@
             # since 'reading' is a property of SoundSensor, it's treated differently
             # see 'mock_pitop()' in pitop.py
             reading_mock = component._mock.get("reading")
             reading_mock.return_value = e.value
 
 
 class Potentiometer(SliderSensorSprite):
-    Size = (PMA_CUBE_SIZE[0] * 2 + MARGIN * 3, PMA_CUBE_SIZE[1] + 2 * MARGIN)
+    Size = (PMA_CUBE_SIZE[0] * 2 + MARGIN, PMA_CUBE_SIZE[1])
     image = Images.Potentiometer
     measurement_key_in_state = "position"
     icon = Images.angle_icon
 
 
 class UltrasonicSensor(SliderSensorSprite):
-    Size = (PMA_CUBE_SIZE[0] * 3 + MARGIN * 3, PMA_CUBE_SIZE[1] + 2 * MARGIN)
+    Size = (PMA_CUBE_SIZE[0] * 3 + MARGIN, PMA_CUBE_SIZE[1])
     image = Images.UltrasonicSensor
     max_value = 3
     measurement_key_in_state = "distance"
     icon = Images.distance_icon
     slider_step = 0.1
 
     @staticmethod
```

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/virtual_hardware/fonts.py` & `pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/fonts.py`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/virtual_hardware/pitop.py` & `pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/pitop.py`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/virtual_hardware/vendor/Mock/GPIO.py` & `pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/vendor/Mock/GPIO.py`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/widgets/slider.py` & `pitop.simulation-0.31.0.post2/pitop/simulation/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop/simulation/widgets/widget.py` & `pitop.simulation-0.31.0.post2/pitop/simulation/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.30.0.post1/pitop.simulation.egg-info/PKG-INFO` & `pitop.simulation-0.31.0.post2/pitop.simulation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.simulation
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Simulation
```

### Comparing `pitop.simulation-0.30.0.post1/pitop.simulation.egg-info/SOURCES.txt` & `pitop.simulation-0.31.0.post2/pitop.simulation.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 setup.py
 pitop.simulation.egg-info/PKG-INFO
 pitop.simulation.egg-info/SOURCES.txt
 pitop.simulation.egg-info/dependency_links.txt
 pitop.simulation.egg-info/requires.txt
 pitop.simulation.egg-info/top_level.txt
 pitop/simulation/__init__.py
+pitop/simulation/color.py
 pitop/simulation/events.py
+pitop/simulation/port_label.py
 pitop/simulation/simsprite.py
 pitop/simulation/simulation.py
 pitop/simulation/sprites.py
 pitop/simulation/utils.py
 pitop/simulation/images/Button.png
 pitop/simulation/images/Button_pressed.png
 pitop/simulation/images/Buzzer.png
```

### Comparing `pitop.simulation-0.30.0.post1/setup.py` & `pitop.simulation-0.31.0.post2/setup.py`

 * *Files identical despite different names*

