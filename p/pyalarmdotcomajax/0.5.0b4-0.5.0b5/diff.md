# Comparing `tmp/pyalarmdotcomajax-0.5.0b4.tar.gz` & `tmp/pyalarmdotcomajax-0.5.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalarmdotcomajax-0.5.0b4.tar", last modified: Sat May 20 18:25:04 2023, max compression
+gzip compressed data, was "pyalarmdotcomajax-0.5.0b5.tar", last modified: Mon May 22 20:21:26 2023, max compression
```

## Comparing `pyalarmdotcomajax-0.5.0b4.tar` & `pyalarmdotcomajax-0.5.0b5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:25:04.517009 pyalarmdotcomajax-0.5.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-05-20 18:25:04.517009 pyalarmdotcomajax-0.5.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:25:04.501009 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/
--rw-r--r--   0 runner    (1001) docker     (123)    41492 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20518 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:25:04.509009 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/image_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14474 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:25:04.509009 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:25:04.513009 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:25:04.505009 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-05-20 18:25:04.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-20 18:25:04.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:25:04.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 18:25:04.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-20 18:25:04.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-20 18:25:04.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:25:04.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-20 18:25:04.517009 pyalarmdotcomajax-0.5.0b4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:25:04.513009 pyalarmdotcomajax-0.5.0b4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:25:04.517009 pyalarmdotcomajax-0.5.0b4/tests/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/tests/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/tests/test_device_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/tests/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/tests/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/tests/test_thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:21:26.834513 pyalarmdotcomajax-0.5.0b5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-05-22 20:21:26.834513 pyalarmdotcomajax-0.5.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:21:26.826513 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/
+-rw-r--r--   0 runner    (1001) docker     (123)    47148 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20770 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:21:26.830513 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/image_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14474 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:21:26.830513 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:21:26.834513 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:21:26.826513 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-05-22 20:21:26.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-22 20:21:26.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:21:26.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-22 20:21:26.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 20:21:26.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-22 20:21:26.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:21:26.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-22 20:21:26.834513 pyalarmdotcomajax-0.5.0b5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:21:26.834513 pyalarmdotcomajax-0.5.0b5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:21:26.834513 pyalarmdotcomajax-0.5.0b5/tests/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/tests/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/tests/test_device_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/tests/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/tests/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/tests/test_thermostat.py
```

### Comparing `pyalarmdotcomajax-0.5.0b4/LICENSE` & `pyalarmdotcomajax-0.5.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/PKG-INFO` & `pyalarmdotcomajax-0.5.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.5.0b4
+Version: 0.5.0b5
 Summary: Python Interface for Alarm.com
 Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
 Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b4 Summary: Python
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b5 Summary: Python
 Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
 46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
 System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: Environment :: Web
```

### Comparing `pyalarmdotcomajax-0.5.0b4/README.md` & `pyalarmdotcomajax-0.5.0b5/README.md`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/__init__.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import json
 import logging
 import re
-from collections.abc import Callable
-from datetime import datetime
+from collections.abc import Callable, Coroutine
+from contextlib import suppress
+from datetime import datetime, timedelta
 from enum import Enum
-from typing import TypedDict
+from typing import Any, TypedDict
 
 import aiohttp
 from bs4 import BeautifulSoup
 
 from pyalarmdotcomajax import const as c
 from pyalarmdotcomajax.devices import (
     BaseDevice,
@@ -26,32 +27,32 @@
     AttributeRegistry,
     DeviceRegistry,
     DeviceType,
 )
 from pyalarmdotcomajax.errors import (
     AuthenticationFailed,
     DataFetchFailed,
+    SessionTimeout,
     TryAgain,
     TwoFactor_ConfigurationRequired,
-    TwoFactor_OtpRequired,
     UnexpectedDataStructure,
     UnsupportedDevice,
 )
 from pyalarmdotcomajax.extensions import (
     CameraSkybellControllerExtension,
     ConfigurationOption,
     ControllerExtensions_t,
     ExtendedProperties,
 )
 from pyalarmdotcomajax.websockets.client import WebSocketClient, WebSocketState
 
 # TODO: Use error handler and exception handlers in _async_get_system_devices on other request functions.
 # TODO: Fix get raw server response function.
 
-__version__ = "0.5.0-beta.4"
+__version__ = "0.5.0-beta.5"
 
 log = logging.getLogger(__name__)
 
 
 class ExtensionResults(TypedDict):
     """Results of multi-device extension calls."""
 
@@ -85,14 +86,15 @@
     ALL_SYSTEMS_URL_TEMPLATE = "{}web/api/systems/availableSystemItems?searchString="
     ALL_RECENT_IMAGES_TEMPLATE = "{}web/api/imageSensor/imageSensorImages/getRecentImages"
 
     # LOGIN & SESSION: BEGIN
     LOGIN_TWO_FACTOR_COOKIE_NAME = "twoFactorAuthenticationId"
     LOGIN_USERNAME_FIELD = "ctl00$ContentPlaceHolder1$loginform$txtUserName"
     LOGIN_PASSWORD_FIELD = "txtPassword"  # noqa: S105
+    LOGIN_REMEMBERME_FIELD = "ctl00$ContentPlaceHolder1$loginform$chkRememberMe"
 
     LOGIN_URL = "https://www.alarm.com/login"
     LOGIN_POST_URL = "https://www.alarm.com/web/Default.aspx"
     LOGIN_2FA_POST_URL_TEMPLATE = (
         "{}web/api/engines/twoFactorAuthentication/twoFactorAuthentications/{}/verifyTwoFactorCode"
     )
     LOGIN_2FA_DETAIL_URL_TEMPLATE = "{}web/api/engines/twoFactorAuthentication/twoFactorAuthentications/{}"
@@ -103,17 +105,20 @@
     LOGIN_2FA_REQUEST_OTP_EMAIL_URL_TEMPLATE = "{}web/api/engines/twoFactorAuthentication/twoFactorAuthentications/{}/sendTwoFactorAuthenticationCodeViaEmail"
 
     VIEWSTATE_FIELD = "__VIEWSTATE"
     VIEWSTATEGENERATOR_FIELD = "__VIEWSTATEGENERATOR"
     EVENTVALIDATION_FIELD = "__EVENTVALIDATION"
     PREVIOUSPAGE_FIELD = "__PREVIOUSPAGE"
 
-    KEEP_ALIVE_CHECK_URL_TEMPLATE = "{}web/KeepAlive.aspx?timestamp={}"
-    KEEP_ALIVE_CHECK_RESPONSE = '{"status":"Keep Alive"}'
-    KEEP_ALIVE_URL = "{}web/api/identities/{}/reloadContext"
+    KEEP_ALIVE_DEFAULT_URL = "/web/KeepAlive.aspx"
+    KEEP_ALIVE_URL_PARAM_TEMPLATE = "?timestamp={}"
+    KEEP_ALIVE_RENEW_SESSION_URL_TEMPLATE = "{}web/api/identities/{}/reloadContext"
+    KEEP_ALIVE_SIGNAL_INTERVAL_S = 60
+    SESSION_REFRESH_DEFAULT_INTERVAL_MS = 780000  # 13 minutes. Sessions expire at 15.
+
     # LOGIN & SESSION: END
 
     def __init__(
         self,
         username: str,
         password: str,
         websession: aiohttp.ClientSession,
@@ -135,30 +140,43 @@
 
         self._provider_name: str | None = None
         self._user_id: str | None = None
         self._user_email: str | None = None
         self._active_system_id: str | None = None
         self._ajax_headers: dict = self.AJAX_HEADERS_TEMPLATE
 
-        self._ws_state_callback: Callable[[WebSocketState], None] | None = None
-        self._websocket: WebSocketClient | None = None
-
         self._partition_map: dict = (
             {}
         )  # Individual devices don't list their associated partitions. This map is used to retrieve partition id when each device is created.
 
         self._installed_device_types: set[DeviceType] = (
             set()
         )  # List of device types that are present in a user's environment. We'll use this to cut down on the number of API calls made.
 
         self._trouble_conditions: dict = {}
 
         self.devices: DeviceRegistry = DeviceRegistry()
 
         #
+        # WEBSOCKET ATTRIBUTES
+        #
+
+        self._ws_state_callback: Callable[[WebSocketState], None] | None = None
+        self._websocket: WebSocketClient | None = None
+
+        #
+        # SESSION ATTRIBUTES
+        #
+
+        self._session_refresh_interval_ms: int = self.SESSION_REFRESH_DEFAULT_INTERVAL_MS
+        self._keep_alive_url: str = self.KEEP_ALIVE_DEFAULT_URL
+        self._last_session_refresh: datetime = datetime.now()
+        self._session_timer: SessionTimer | None = None
+
+        #
         # CLI ATTRIBUTES
         #
         self.raw_catalog: dict = {}
         self.raw_system: dict = {}
         self.raw_image_sensors: dict = {}
         self.raw_recent_images: dict = {}
 
@@ -344,37 +362,48 @@
                             device_type=device_type,
                             event=event,
                             device_id=device_id,
                             msg_body=msg_body,
                         )
 
                 case "403":
-                    # May have been logged out, try again
+                    # Session may have expired. Log back in and try again.
                     log.warning(
-                        "Error executing %s, NOT logging in and trying again...",
+                        "Error executing %s. Session. probably expired. Logging in and trying again...",
                         event.value,
                     )
 
-                    return False
-                    # if retry_on_failure:
-                    #     await self.async_login()
-                    #     return await self.async_send_command(
-                    #         device_type,
-                    #         event,
-                    #         device_id,
-                    #         msg_body,
-                    #         False,
-                    #     )
+                    if retry_on_failure:
+                        await self.async_login()
+                        return await self.async_send_command(
+                            device_type,
+                            event,
+                            device_id,
+                            msg_body,
+                            False,
+                        )
 
         log.error(
             f"{event.value} failed with HTTP code {resp.status}. URL: {url}\nJSON: {msg_body}\nHeaders:"
             f" {self._ajax_headers}"
         )
         raise ConnectionError
 
+    async def start_session_nudger(self) -> None:
+        """Start task to nudge user sessions to keep from timing out."""
+
+        self._session_timer = SessionTimer(self.keep_alive, self.KEEP_ALIVE_SIGNAL_INTERVAL_S)
+        await self._session_timer.start()
+
+    async def stop_session_nudger(self) -> None:
+        """Stop session nudger."""
+
+        if self._session_timer:
+            await self._session_timer.stop()
+
     #
     # WEBSOCKET FUNCTIONS
     #
 
     def start_websocket(self, ws_state_callback: Callable[[WebSocketState], None] | None = None) -> None:
         """Construct and return a websocket client."""
 
@@ -393,61 +422,57 @@
 
     #
     # AUTHENTICATION FUNCTIONS
     #
 
     async def async_login(
         self,
-    ) -> None:
+    ) -> list[OtpType] | None:
         """Login to Alarm.com."""
         log.debug("Attempting to log in to Alarm.com")
 
-        # TODO: Prevent login from making a ton of saved devices in ADC.
-
         try:
             await self._async_login_and_get_key()
             await self._async_get_identity_info()
 
-            # Check whether two factor authentication is required.
-            if not self._two_factor_cookie:
-                async with self._websession.get(
-                    url=AttributeRegistry.get_endpoints(DeviceType.SYSTEM)["primary"].format(c.URL_BASE, ""),
-                    headers=self._ajax_headers,
-                ) as resp:
-                    json_rsp = await resp.json()
-
-                    log.debug(f"Response from Alarm.com login: {resp.status} {resp.json()}")
+            log.info("Logged in successfully.")
 
-                for error in (errors := json_rsp.get("errors", {})):
-                    if error.get("status") == "409" and error.get("detail") == "TwoFactorAuthenticationRequired":
-                        log.debug("Two factor authentication code or cookie required.")
-                        raise TwoFactor_OtpRequired
+            return await self._get_2fa_requirements()
 
         except (DataFetchFailed, UnexpectedDataStructure) as err:
             raise ConnectionError from err
         except (AuthenticationFailed, PermissionError) as err:
             raise AuthenticationFailed from err
-        except TwoFactor_ConfigurationRequired as err:
-            raise err
-
-        log.info("Logged in successfully.")
-        return None
 
-    async def async_get_enabled_2fa_methods(self) -> list[OtpType]:
+    async def _get_2fa_requirements(self) -> list[OtpType] | None:
         """Get list of two factor authentication methods enabled on account."""
 
         async with self._websession.get(
             url=self.LOGIN_2FA_DETAIL_URL_TEMPLATE.format(c.URL_BASE, self._user_id),
             headers=self._ajax_headers,
         ) as resp:
             json_rsp = await resp.json()
+
+            if not (data := json_rsp.get("data", {})):
+                raise UnexpectedDataStructure("Could not find expected data in two-factor authentication details.")
+
+            if data.get("showSuggestedSetup") is True:
+                raise TwoFactor_ConfigurationRequired(
+                    "Got 2FA nag screen. 2FA must be configured on this account before proceeding."
+                )
+
             enabled_otp_types_bitmask = json_rsp.get("data", {}).get("attributes", {}).get("enabledTwoFactorTypes")
             enabled_2fa_methods = [
                 otp_type for otp_type in OtpType if bool(enabled_otp_types_bitmask & otp_type.value)
             ]
+
+            if OtpType.disabled in enabled_2fa_methods or data.get("isCurrentDeviceTrusted") is True:
+                # 2FA is disabled, we can skip 2FA altogether.
+                return None
+
             log.info(f"Requires two-factor authentication. Enabled methods are {enabled_2fa_methods}")
             return enabled_2fa_methods
 
     async def async_request_otp(self, method: OtpType | None) -> None:
         """Request SMS/email OTP code from Alarm.com."""
 
         if method not in (OtpType.email, OtpType.sms):
@@ -471,15 +496,17 @@
 
         except (asyncio.TimeoutError, aiohttp.ClientError) as err:
             log.error("Can not load 2FA submission page from Alarm.com")
             raise DataFetchFailed from err
 
         return None
 
-    async def async_submit_otp(self, code: str, method: OtpType, device_name: str | None = None) -> str | None:
+    async def async_submit_otp(
+        self, code: str, method: OtpType, device_name: str | None = None, remember_me: bool = False
+    ) -> str | None:
         """Submit two factor authentication code.
 
         Register device and return 2FA code if device_name is not None.
         """
 
         # Submit code
         try:
@@ -507,27 +534,27 @@
                 resp.status,
                 await resp.text(),
             )
             raise DataFetchFailed("Unknown error.")
 
         log.debug("Submitted OTP code.")
 
-        if not device_name:
+        if not device_name and not remember_me:
             log.debug('Skipping "Remember Me".')
             return None
 
         # Submit device name for "remember me" function.
-        if json_rsp.get("value", {}).get("deviceName"):
+        if suggested_device_name := json_rsp.get("value", {}).get("deviceName"):
             try:
                 log.debug("Registering device...")
 
                 async with self._websession.post(
                     url=self.LOGIN_2FA_TRUST_URL_TEMPLATE.format(c.URL_BASE, self._user_id),
                     headers=self._ajax_headers,
-                    json={"deviceName": device_name},
+                    json={"deviceName": device_name if device_name else suggested_device_name},
                 ) as resp:
                     json_rsp = await resp.json()
             except (asyncio.TimeoutError, aiohttp.ClientError) as err:
                 log.error("Can not load device trust page from Alarm.com")
                 raise DataFetchFailed from err
 
             log.debug("Registered device.")
@@ -538,32 +565,91 @@
                 log.debug("Found two-factor authentication cookie: %s", cookie.value)
                 self._two_factor_cookie = {"twoFactorAuthenticationId": cookie.value} if cookie.value else {}
                 return str(cookie.value)
 
         log.error("Failed to find two-factor authentication cookie.")
         return None
 
+    async def is_logged_in(self, throw: bool = False) -> bool:
+        """Check if we are still logged in."""
+
+        url = f"{c.URL_BASE[:-1]}{self._keep_alive_url}{self.KEEP_ALIVE_URL_PARAM_TEMPLATE.format(int(round(datetime.now().timestamp())))}"
+
+        async with self._websession.get(
+            url=url,
+            headers=self._ajax_headers,
+        ) as resp:
+            text_rsp = await resp.text()
+
+        if resp.status == 403:
+            log.debug("Session expired.")
+
+            if throw:
+                raise SessionTimeout
+
+            return False
+
+        elif resp.status >= 400:
+            raise DataFetchFailed(f"Failed to send keep alive signal. Response: {text_rsp}")
+
+        return True
+
+    async def keep_alive(self) -> None:
+        """Keep session alive. Handle if not (optionally).
+
+        Should be called once per minute to keep session alive.
+        """
+
+        reload_context_now = (
+            self._last_session_refresh + timedelta(milliseconds=self._session_refresh_interval_ms)
+        ) < datetime.now()
+
+        seconds_remaining = (
+            self._last_session_refresh
+            + (timedelta(milliseconds=self._session_refresh_interval_ms))
+            - datetime.now()
+        ).total_seconds()
+
+        debug_message = "Sending keep alive signal. Time until session context refresh: {}".format(
+            "imminent" if reload_context_now else f"~ {round((seconds_remaining % 3600) // 60)} minutes."
+        )
+        log.debug(debug_message)
+
+        try:
+            if await self.is_logged_in(throw=True) and reload_context_now:
+                await self._reload_session_context()
+        except SessionTimeout:
+            log.info("User session expired. Logging back in.")
+            await self.async_login()
+
     #
     #
     #####################
     # PRIVATE FUNCTIONS #
     #####################
     #
-    # Communicate directly with the ADC API
 
-    async def _async_keep_alive_login_check(self) -> bool:
-        """Check if we are logged in."""
+    async def _reload_session_context(self) -> None:
+        """Check if we are still logged in."""
 
-        async with self._websession.get(
-            url=self.KEEP_ALIVE_CHECK_URL_TEMPLATE.format(c.URL_BASE, int(round(datetime.now().timestamp()))),
+        log.debug("Reloading session context.")
+
+        async with self._websession.post(
+            url=self.KEEP_ALIVE_RENEW_SESSION_URL_TEMPLATE.format(c.URL_BASE, self._user_id),
             headers=self._ajax_headers,
+            data=json.dumps({"included": [], "meta": {"transformer_version": "1.1"}}),
         ) as resp:
-            text_rsp = await resp.text()
+            json_rsp = await resp.json()
+
+            if resp.status >= 400:
+                raise DataFetchFailed(f"Failed to reload session context. Response: {json_rsp}")
 
-        return bool(text_rsp == self.KEEP_ALIVE_CHECK_RESPONSE)
+            self._last_session_refresh = datetime.now()
+
+        return None
 
     async def _async_update__build_device(
         self,
         raw_device: dict,
         device_type_specific_data: dict[str, DeviceTypeSpecificData],
         extension_results: dict[str, ExtensionResults],
     ) -> AllDevices_t:
@@ -691,34 +777,40 @@
                     results[device_id] = {
                         "settings": device_properties.settings,
                         "controller": extension_controller,
                     }
 
         return results
 
-    async def _async_get_active_system(self) -> str:
+    async def _async_get_active_system(self, retry_on_failure: bool = True) -> str:
         """Get active system for user account."""
 
         try:
             log.info("Getting active system.")
 
             async with self._websession.get(
                 url=self.ALL_SYSTEMS_URL_TEMPLATE.format(c.URL_BASE),
                 headers=self._ajax_headers,
-                raise_for_status=True,
             ) as resp:
                 json_rsp = await resp.json()
 
+                await self._async_handle_server_errors(json_rsp, "active system", retry_on_failure)
+
                 return str(
                     [system["id"] for system in json_rsp.get("data", []) if system["attributes"]["isSelected"]][0]
                 )
 
         except (asyncio.TimeoutError, aiohttp.ClientError, aiohttp.ClientResponseError, KeyError) as err:
             log.error("Failed to get available systems.")
             raise DataFetchFailed from err
+        except TryAgain as err:
+            if retry_on_failure:
+                return await self._async_get_active_system(retry_on_failure=False)
+            else:
+                raise err
 
     async def _async_get_recent_images(self) -> dict[str, DeviceTypeSpecificData]:
         """Get recent images."""
 
         try:
             log.info("Getting recent images.")
 
@@ -759,36 +851,39 @@
             log.info(f"Checking system {system_id} for image sensors.")
 
             # Find image sensors.
 
             async with self._websession.get(
                 url=AttributeRegistry.get_endpoints(DeviceType.SYSTEM)["primary"].format(c.URL_BASE, system_id),
                 headers=self._ajax_headers,
-                raise_for_status=True,
             ) as resp:
                 json_rsp = await resp.json()
 
                 await self._async_handle_server_errors(json_rsp, "image sensors", retry_on_failure)
 
                 return len(json_rsp["data"].get("relationships", {}).get("imageSensors", {}).get("data", [])) > 0
 
         except (asyncio.TimeoutError, aiohttp.ClientError, aiohttp.ClientResponseError, KeyError) as err:
             log.error("Failed to get image sensors.")
             raise DataFetchFailed from err
+        except TryAgain as err:
+            if retry_on_failure:
+                return await self._async_has_image_sensors(system_id, retry_on_failure=False)
+            else:
+                raise err
 
     async def _async_get_system(self, system_id: str, retry_on_failure: bool = True) -> list[dict]:
         """Get all devices present in system."""
 
         try:
             log.info(f"Getting system data for {system_id}.")
 
             async with self._websession.get(
                 url=AttributeRegistry.get_endpoints(DeviceType.SYSTEM)["primary"].format(c.URL_BASE, system_id),
                 headers=self._ajax_headers,
-                raise_for_status=True,
             ) as resp:
                 json_rsp = await resp.json()
 
                 # Used by adc CLI.
                 self.raw_system = json_rsp
 
                 await self._async_handle_server_errors(json_rsp, "system", retry_on_failure)
@@ -806,15 +901,14 @@
 
         try:
             log.info(f"Getting all devices in {system_id}.")
 
             async with self._websession.get(
                 url=self.ALL_DEVICES_URL_TEMPLATE.format(c.URL_BASE, system_id),
                 headers=self._ajax_headers,
-                raise_for_status=True,
             ) as resp:
                 json_rsp = await resp.json()
 
                 # Used by adc CLI.
                 self.raw_catalog = json_rsp
 
                 await self._async_handle_server_errors(json_rsp, "system devices", retry_on_failure)
@@ -838,15 +932,14 @@
 
         try:
             log.info(f"Getting all {device_type.value}.")
 
             async with self._websession.get(
                 url=AttributeRegistry.get_endpoints(device_type)["primary"].format(c.URL_BASE, ""),
                 headers=self._ajax_headers,
-                raise_for_status=True,
             ) as resp:
                 json_rsp = await resp.json()
 
                 # Used by adc CLI.
                 if device_type == DeviceType.IMAGE_SENSOR:
                     self.raw_image_sensors = json_rsp
 
@@ -858,53 +951,82 @@
             log.error(f"Failed to get {device_type.value}.")
             raise DataFetchFailed from err
         except TryAgain:
             return await self._async_get_devices_by_device_type(device_type=device_type, retry_on_failure=False)
 
     async def _async_get_identity_info(self) -> None:
         """Get user id, email address, provider name, etc."""
-        try:
-            async with self._websession.get(
-                url=c.IDENTITIES_URL_TEMPLATE.format(c.URL_BASE, ""),
-                headers=self._ajax_headers,
-                cookies=self._two_factor_cookie,
-            ) as resp:
-                json_rsp = await resp.json()
 
+        async with self._websession.get(
+            url=c.IDENTITIES_URL_TEMPLATE.format(c.URL_BASE, ""),
+            headers=self._ajax_headers,
+            cookies=self._two_factor_cookie,
+        ) as resp:
+            json_rsp = await resp.json()
+
+            try:
                 self._user_id = json_rsp["data"][0]["id"]
                 self._provider_name = json_rsp["data"][0]["attributes"]["logoName"]
+                self._provider_name = json_rsp["data"][0]["attributes"]["logoName"]
 
                 for inclusion in json_rsp["included"]:
                     if inclusion["id"] == self._user_id and inclusion["type"] == "profile/profile":
                         self._user_email = inclusion["attributes"]["loginEmailAddress"]
 
-            if self._user_email is None:
-                raise AuthenticationFailed("Could not find user email address.")
+                if not self._user_email:
+                    raise KeyError("Failed to get user's email address.")
+            except KeyError as err:
+                log.error(f"{__name__} _async_get_identity_info: Failed to get user's identity info.")
+                log.debug(
+                    f"{__name__} _async_get_identity_info: Server Response:\n{json.dumps(json_rsp, indent=4)}"
+                )
+                raise AuthenticationFailed from err
 
-            log.debug("Got Provider: %s, User ID: %s", self._provider_name, self._user_id)
+            try:
+                self._session_refresh_interval_ms = json_rsp["data"][0]["attributes"][
+                    "applicationSessionProperties"
+                ]["inactivityWarningTimeoutMs"]
+
+                if not self._session_refresh_interval_ms:
+                    raise KeyError
+            except KeyError:
+                self._session_refresh_interval_ms = self.SESSION_REFRESH_DEFAULT_INTERVAL_MS
 
-        except KeyError as err:
-            log.error(f"{__name__} _async_get_identity_info: Failed to get user's identity info.")
-            log.debug(f"{__name__} _async_get_identity_info: Server Response:\n{json.dumps(json_rsp, indent=4)}")
-            raise AuthenticationFailed from err
+            try:
+                self._keep_alive_url = json_rsp["data"][0]["attributes"]["applicationSessionProperties"][
+                    "keepAliveUrl"
+                ]
+                if not self._keep_alive_url:
+                    raise KeyError
+            except KeyError:
+                self._keep_alive_url = self.KEEP_ALIVE_DEFAULT_URL
+
+            log.debug("*** START IDENTITY INFO ***")
+            log.debug(f"Provider: {self._provider_name}")
+            log.debug(f"User: {self._user_id} {self._user_email}")
+            log.debug(f"Keep Alive Interval: {self._session_refresh_interval_ms}")
+            log.debug(f"Keep Alive URL: {self._keep_alive_url}")
+            log.debug("*** END IDENTITY INFO ***")
 
-    async def _async_get_trouble_conditions(self) -> None:
+    async def _async_get_trouble_conditions(self, retry_on_failure: bool = True) -> None:
         """Get trouble conditions for all devices."""
 
         # TODO: Trouble condition dict should be flagged, not None, when library encounters an error retrieving trouble conditions.
 
         try:
             async with self._websession.get(
                 url=c.TROUBLECONDITIONS_URL_TEMPLATE.format(c.URL_BASE, ""),
                 headers=self._ajax_headers,
             ) as resp:
                 json_rsp = await resp.json()
 
                 log.debug("Trouble condition response:\n%s", json_rsp)
 
+                await self._async_handle_server_errors(json_rsp, "active system", retry_on_failure)
+
                 trouble_all_devices: dict = {}
                 for condition in json_rsp.get("data", []):
                     device_id = condition.get("attributes", {}).get("emberDeviceId")
                     new_trouble: TroubleCondition = {
                         "message_id": condition.get("id"),
                         "title": condition.get("attributes", {}).get("description"),
                         "body": condition.get("attributes", {}).get("extraData", {}).get("description"),
@@ -932,14 +1054,20 @@
             raise DataFetchFailed from err
 
         except KeyError as err:
             self._trouble_conditions = {}
             log.error("Failed processing trouble conditions.")
             raise UnexpectedDataStructure from err
 
+        except TryAgain as err:
+            if retry_on_failure:
+                return await self._async_get_trouble_conditions(retry_on_failure=False)
+            else:
+                raise err
+
     async def _async_handle_server_errors(
         self, json_rsp: dict, request_name: str, retry_on_failure: bool = False
     ) -> None:
         """Handle errors returned by the server."""
 
         log.debug(
             f"\n==============================\nServer Response:\n{json_rsp}\n=============================="
@@ -971,15 +1099,15 @@
                     log.error(
                         "Error fetching data from Alarm.com. Got 403 status when"
                         f" fetching {request_name}. Logging in"
                         " again didn't help. Giving up on device type."
                     )
                     raise DataFetchFailed(error_msg)
 
-                if not self._async_keep_alive_login_check():
+                if not self.is_logged_in():
                     log.debug(
                         "Error fetching data from Alarm.com. Got 403 status"
                         f" when requesting {request_name}. Trying to"
                         " refresh auth tokens by logging in again."
                     )
 
                     await self.async_login()
@@ -1035,32 +1163,67 @@
                 data={
                     self.LOGIN_USERNAME_FIELD: self._username,
                     self.LOGIN_PASSWORD_FIELD: self._password,
                     self.VIEWSTATE_FIELD: login_info[self.VIEWSTATE_FIELD],
                     self.VIEWSTATEGENERATOR_FIELD: login_info[self.VIEWSTATEGENERATOR_FIELD],
                     self.EVENTVALIDATION_FIELD: login_info[self.EVENTVALIDATION_FIELD],
                     self.PREVIOUSPAGE_FIELD: login_info[self.PREVIOUSPAGE_FIELD],
+                    self.LOGIN_REMEMBERME_FIELD: "on",
                     "IsFromNewSite": "1",
                 },
                 cookies=self._two_factor_cookie,
             ) as resp:
                 if re.search("m=login_fail", str(resp.url)) is not None:
                     log.error("Login failed.")
                     log.error("\nResponse URL:\n%s\n", str(resp.url))
                     log.error("\nRequest Headers:\n%s\n", str(resp.request_info.headers))
                     raise AuthenticationFailed("Invalid username and password.")
 
-                # If Alarm.com is warning us that we'll have to set up two factor authentication soon, alert caller.
-                if re.search("concurrent-two-factor-authentication", str(resp.url)) is not None:
-                    raise TwoFactor_ConfigurationRequired("Encountered 2FA nag screen.")
-
                 # Update anti-forgery cookie
                 self._ajax_headers["ajaxrequestuniquekey"] = resp.cookies["afg"].value
 
         except (asyncio.TimeoutError, aiohttp.ClientError) as err:
             log.error("Can not login to Alarm.com")
             raise DataFetchFailed from err
         except KeyError as err:
             log.error("Unable to extract ajax key from Alarm.com. Response:\n%s", resp)
             raise DataFetchFailed from err
 
+        self._last_session_refresh = datetime.now()
+
         log.debug("Logged in to Alarm.com.")
+
+
+class SessionTimer:
+    """Run keep_alive function periodically to keep session alive."""
+
+    # https://stackoverflow.com/a/37514633
+
+    def __init__(self, func: Callable[[], Coroutine[Any, Any, Any]], time: float) -> None:
+        """Initialize SessionTimer. Takes time in seconds."""
+        self.func = func
+        self.time: float = time
+        self.is_started: bool = False
+        self._task: asyncio.Task | None = None
+
+    async def start(self) -> None:
+        """Start SessionTimer."""
+        if not self.is_started:
+            self.is_started = True
+            # Start task to call func periodically:
+            self._task = asyncio.ensure_future(self._run())
+
+    async def stop(self) -> None:
+        """Stop SessionTimer."""
+        if self.is_started:
+            self.is_started = False
+            # Stop task and await it stopped:
+            if self._task:
+                self._task.cancel()
+                with suppress(asyncio.CancelledError):
+                    await self._task
+
+    async def _run(self) -> None:
+        """Run task and sleep."""
+        while True:
+            await asyncio.sleep(self.time)
+            await self.func()
```

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/cli.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from . import AlarmController, OtpType
 from .devices import BaseDevice, DeviceType
 from .devices.light import Light
 from .devices.sensor import Sensor
 from .errors import (
     InvalidConfigurationOption,
     TwoFactor_ConfigurationRequired,
-    TwoFactor_OtpRequired,
     UnexpectedDataStructure,
 )
 from .extensions import ConfigurationOption
 from .helpers import ExtendedEnumMixin, slug_to_title
 from .websockets.client import WebSocketState
 
 CLI_CARD_BREAK = ""  # "--------"
@@ -217,25 +216,23 @@
             username=args.get("username", ""),
             password=args.get("password", ""),
             websession=session,
             twofactorcookie=args.get("cookie"),
         )
 
         try:
-            await alarm.async_login()
+            if enabled_2fa_methods := await alarm.async_login():
+                await async_handle_otp_workflow(alarm, args, enabled_2fa_methods)
         except TwoFactor_ConfigurationRequired:
             cprint(
                 "Unable to log in. Please set up two-factor authentication for this account.",
                 "red",
             )
             sys.exit()
 
-        except TwoFactor_OtpRequired:
-            await async_handle_otp_workflow(alarm, args)
-
         #######################
         # REFRESH DEVICE DATA #
         #######################
 
         await alarm.async_update()
 
         device_type_output: dict = {}
@@ -398,42 +395,52 @@
                 "on_yellow",
                 attrs=["bold"],
             )
             cprint(
                 "(Press Ctrl+C or Cmd+C to exit.)",
                 attrs=["bold"],
             )
+
             await _async_stream_realtime(alarm)
 
 
 #############
 # FUNCTIONS #
 #############
 
 
 async def _async_stream_realtime(alarm: AlarmController) -> None:
     """Stream real-time updates via WebSockets."""
 
+    # Keep user session alive.
+    await alarm.start_session_nudger()
+
     def ws_state_handler(state: WebSocketState) -> None:
         """Handle websocket connection state changes."""
 
-        print(f"Websocket state changed to: {state.name}")
+        if state in [WebSocketState.DISCONNECTED]:
+            # asyncio.create_task(alarm.async_connect())
+            cprint("Lost streaming connection to Alarm.com.", "red")
+            sys.exit()
 
     alarm.start_websocket(ws_state_handler)
 
     try:
         # Keep event loop alive until cancelled.
         while True:
             await asyncio.sleep(1)
 
     except asyncio.CancelledError:
         pass
 
     finally:
-        # Close connection when cancelled.
+        # Close connections & stop tasks when cancelled.
+
+        await alarm.stop_session_nudger()
+
         alarm.stop_websocket()
 
 
 def _human_output(alarm: AlarmController) -> dict:
     """Output user-friendly list of devices and statuses."""
 
     output = {}
@@ -533,15 +540,17 @@
             output_str += f"""[TITLE: {condition["title"]}] [MESSAGE ID: {condition["message_id"]}] [MESSAGE: {condition["body"]}] """
 
         output_str += "\n"
 
     return output_str
 
 
-async def async_handle_otp_workflow(alarm: AlarmController, args: dict[str, Any]) -> None:
+async def async_handle_otp_workflow(
+    alarm: AlarmController, args: dict[str, Any], enabled_2fa_methods: list[OtpType]
+) -> None:
     """Handle two-factor authentication workflow."""
 
     #
     # Determine which OTP method to use
     #
 
     code: str | None
@@ -552,15 +561,15 @@
     else:
         cprint(
             "Two factor authentication is enabled for this user.",
             attrs=["bold"],
         )
 
         # Get list of enabled OTP methods.
-        if len(enabled_2fa_methods := await alarm.async_get_enabled_2fa_methods()) == 1:
+        if len(enabled_2fa_methods) == 1:
             # If only one OTP method is enabled, use it without prompting user.
             selected_otp_method = enabled_2fa_methods[0]
             cprint(f"Using {selected_otp_method.name} for One-Time Password.")
         elif cli_otp_method := args.get("otp_method"):
             # If multiple OTP methods are enabled, but the user provided one via CLI, use it.
             selected_otp_method = OtpType(cli_otp_method)
             cprint(f"Using {selected_otp_method.name} for One-Time Password.")
```

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/__init__.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/garage_door.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/garage_door.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/gate.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/gate.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/image_sensor.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/image_sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/light.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/light.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/lock.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/lock.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/partition.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/registry.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/registry.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/sensor.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/system.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/system.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/thermostat.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/thermostat.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/errors.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,7 +44,11 @@
 
 class UnsupportedAction(Exception):
     """Device does not support requested action."""
 
 
 class TryAgain(Exception):
     """Request that caller tries again after session has been fixed."""
+
+
+class SessionTimeout(Exception):
+    """Session has timed out and needs to be re-established."""
```

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/extensions.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/extensions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/helpers.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/helpers.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/client.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/client.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/const.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/const.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/__init__.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/garage_door.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/garage_door.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/gate.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/gate.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/light.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/light.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/lock.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/lock.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/partition.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/sensor.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/thermostat.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/thermostat.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/water_sensor.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/water_sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/messages.py` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/messages.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/PKG-INFO` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.5.0b4
+Version: 0.5.0b5
 Summary: Python Interface for Alarm.com
 Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
 Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b4 Summary: Python
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b5 Summary: Python
 Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
 46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
 System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: Environment :: Web
```

### Comparing `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/SOURCES.txt` & `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/pyproject.toml` & `pyalarmdotcomajax-0.5.0b5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/setup.cfg` & `pyalarmdotcomajax-0.5.0b5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/tests/__init__.py` & `pyalarmdotcomajax-0.5.0b5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/tests/conftest.py` & `pyalarmdotcomajax-0.5.0b5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/tests/test_controller.py` & `pyalarmdotcomajax-0.5.0b5/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/tests/test_device_extensions.py` & `pyalarmdotcomajax-0.5.0b5/tests/test_device_extensions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/tests/test_partition.py` & `pyalarmdotcomajax-0.5.0b5/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/tests/test_sensors.py` & `pyalarmdotcomajax-0.5.0b5/tests/test_sensors.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b4/tests/test_thermostat.py` & `pyalarmdotcomajax-0.5.0b5/tests/test_thermostat.py`

 * *Files identical despite different names*

