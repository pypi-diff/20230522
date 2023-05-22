# Comparing `tmp/robodyno-1.6.0.tar.gz` & `tmp/robodyno-1.6.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robodyno-1.6.0.tar", last modified: Fri May  5 05:39:23 2023, max compression
+gzip compressed data, was "robodyno-1.6.1b0.tar", last modified: Fri May 19 05:49:23 2023, max compression
```

## Comparing `robodyno-1.6.0.tar` & `robodyno-1.6.1b0.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.946601 robodyno-1.6.0/
--rw-r--r--   0 root         (0) root         (0)    10483 2023-05-05 05:39:23.946601 robodyno-1.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6259 2023-05-05 05:39:15.000000 robodyno-1.6.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 05:39:23.946601 robodyno-1.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4004 2023-05-05 05:39:15.000000 robodyno-1.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.918601 robodyno-1.6.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.922601 robodyno-1.6.0/src/robodyno/
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.922601 robodyno-1.6.0/src/robodyno/components/
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.926601 robodyno-1.6.0/src/robodyno/components/brands/
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/brands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2404 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/brands/robodyno.py
--rw-rw-rw-   0 root         (0) root         (0)      801 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/brands/uuid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.930601 robodyno-1.6.0/src/robodyno/components/can_bus/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/can_bus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/can_bus/adaptive_gripper.py
--rw-rw-rw-   0 root         (0) root         (0)     1571 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/can_bus/can_bus_device.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/can_bus/gps_sensor.py
--rw-rw-rw-   0 root         (0) root         (0)     5136 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/can_bus/imu_sensor.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/can_bus/led_driver.py
--rw-rw-rw-   0 root         (0) root         (0)    22429 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/can_bus/motor.py
--rw-rw-rw-   0 root         (0) root         (0)     1997 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/can_bus/pwm_driver.py
--rw-rw-rw-   0 root         (0) root         (0)     3490 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/can_bus/slider_module.py
--rw-rw-rw-   0 root         (0) root         (0)     4449 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/can_bus/stepper_driver.py
--rw-rw-rw-   0 root         (0) root         (0)     2185 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/can_bus/vacuum_gripper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.934601 robodyno-1.6.0/src/robodyno/components/webots/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/webots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19379 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/webots/motor.py
--rw-rw-rw-   0 root         (0) root         (0)     3346 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/webots/slider_module.py
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/components/webots/webots_device.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.934601 robodyno-1.6.0/src/robodyno/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8575 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/interfaces/can_bus.py
--rw-rw-rw-   0 root         (0) root         (0)     2957 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/interfaces/webots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.934601 robodyno-1.6.0/src/robodyno/robots/
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/robots/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.934601 robodyno-1.6.0/src/robodyno/robots/four_dof_palletizing_robot/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/robots/four_dof_palletizing_robot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7717 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/robots/four_dof_palletizing_robot/four_dof_pallet_robot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.938601 robodyno-1.6.0/src/robodyno/robots/four_dof_scara_robot/
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/robots/four_dof_scara_robot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8172 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/robots/four_dof_scara_robot/four_dof_scara_robot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.938601 robodyno-1.6.0/src/robodyno/robots/six_dof_collaborative_robot/
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/robots/six_dof_collaborative_robot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10347 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/robots/six_dof_collaborative_robot/six_dof_collab_robot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.938601 robodyno-1.6.0/src/robodyno/robots/three_dof_delta_robot/
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/robots/three_dof_delta_robot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9508 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/robots/three_dof_delta_robot/three_dof_delta_robot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.942601 robodyno-1.6.0/src/robodyno/robots/three_dof_palletizing_robot/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/robots/three_dof_palletizing_robot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7287 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/robots/three_dof_palletizing_robot/three_dof_pallet_robot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.942601 robodyno-1.6.0/src/robodyno/robots/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/robots/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      602 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/robots/utils/interpolations.py
--rw-rw-rw-   0 root         (0) root         (0)    57825 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/robots/utils/transformations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.946601 robodyno-1.6.0/src/robodyno/tools/
--rw-rw-rw-   0 root         (0) root         (0)    10000 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1460 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/tools/list_devices.py
--rw-rw-rw-   0 root         (0) root         (0)     1828 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/tools/monitor.py
--rw-rw-rw-   0 root         (0) root         (0)      724 2023-05-05 05:39:15.000000 robodyno-1.6.0/src/robodyno/tools/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:39:23.922601 robodyno-1.6.0/src/robodyno.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10483 2023-05-05 05:39:23.000000 robodyno-1.6.0/src/robodyno.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2145 2023-05-05 05:39:23.000000 robodyno-1.6.0/src/robodyno.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 05:39:23.000000 robodyno-1.6.0/src/robodyno.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1133 2023-05-05 05:39:23.000000 robodyno-1.6.0/src/robodyno.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-05 05:39:23.000000 robodyno-1.6.0/src/robodyno.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-05 05:39:23.000000 robodyno-1.6.0/src/robodyno.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.532642 robodyno-1.6.1b0/
+-rw-rw-rw-   0        0        0    11028 2023-05-19 05:49:23.531642 robodyno-1.6.1b0/PKG-INFO
+-rw-rw-rw-   0        0        0      126 2023-05-19 05:43:33.000000 robodyno-1.6.1b0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 05:49:23.532642 robodyno-1.6.1b0/setup.cfg
+-rw-rw-rw-   0        0        0     4940 2023-05-19 05:49:15.000000 robodyno-1.6.1b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.459128 robodyno-1.6.1b0/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.468128 robodyno-1.6.1b0/src/robodyno/
+-rw-rw-rw-   0        0        0     1606 2023-05-17 09:30:59.000000 robodyno-1.6.1b0/src/robodyno/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.486643 robodyno-1.6.1b0/src/robodyno/components/
+-rw-rw-rw-   0        0        0     2999 2023-05-18 03:40:55.000000 robodyno-1.6.1b0/src/robodyno/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.497642 robodyno-1.6.1b0/src/robodyno/components/can_bus/
+-rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/adaptive_gripper.py
+-rw-rw-rw-   0        0        0     3772 2023-05-17 02:08:48.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/can_bus_device.py
+-rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/gps_sensor.py
+-rw-rw-rw-   0        0        0     9038 2023-05-18 03:30:30.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/imu_sensor.py
+-rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/led_driver.py
+-rw-rw-rw-   0        0        0    32976 2023-05-19 04:18:34.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/motor.py
+-rw-rw-rw-   0        0        0     4768 2023-05-18 03:30:47.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/pwm_driver.py
+-rw-rw-rw-   0        0        0     5720 2023-05-17 04:06:44.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/slider_module.py
+-rw-rw-rw-   0        0        0     6833 2023-05-18 03:31:00.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/stepper_driver.py
+-rw-rw-rw-   0        0        0        0 2023-05-16 14:51:18.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/vacuum_gripper.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.500643 robodyno-1.6.1b0/src/robodyno/components/config/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:59:20.000000 robodyno-1.6.1b0/src/robodyno/components/config/__init__.py
+-rw-rw-rw-   0        0        0     2149 2023-05-17 05:24:55.000000 robodyno-1.6.1b0/src/robodyno/components/config/model.py
+-rw-rw-rw-   0        0        0     5980 2023-05-19 03:28:35.000000 robodyno-1.6.1b0/src/robodyno/components/config/robottime_config.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.505643 robodyno-1.6.1b0/src/robodyno/components/webots/
+-rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/components/webots/__init__.py
+-rw-rw-rw-   0        0        0    19697 2023-05-16 03:47:38.000000 robodyno-1.6.1b0/src/robodyno/components/webots/motor.py
+-rw-rw-rw-   0        0        0     3456 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/components/webots/slider_module.py
+-rw-rw-rw-   0        0        0     1543 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/components/webots/webots_device.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.508642 robodyno-1.6.1b0/src/robodyno/interfaces/
+-rw-rw-rw-   0        0        0      533 2023-05-18 03:40:10.000000 robodyno-1.6.1b0/src/robodyno/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     9768 2023-05-19 05:14:39.000000 robodyno-1.6.1b0/src/robodyno/interfaces/can_bus.py
+-rw-rw-rw-   0        0        0     3069 2023-05-16 05:58:37.000000 robodyno-1.6.1b0/src/robodyno/interfaces/webots.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.509642 robodyno-1.6.1b0/src/robodyno/robots/
+-rw-rw-rw-   0        0        0      309 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.511642 robodyno-1.6.1b0/src/robodyno/robots/four_dof_palletizing_robot/
+-rw-rw-rw-   0        0        0       50 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/four_dof_palletizing_robot/__init__.py
+-rw-rw-rw-   0        0        0     7949 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/four_dof_palletizing_robot/four_dof_pallet_robot.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.513642 robodyno-1.6.1b0/src/robodyno/robots/four_dof_scara_robot/
+-rw-rw-rw-   0        0        0       46 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/four_dof_scara_robot/__init__.py
+-rw-rw-rw-   0        0        0     8412 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/four_dof_scara_robot/four_dof_scara_robot.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.516642 robodyno-1.6.1b0/src/robodyno/robots/six_dof_collaborative_robot/
+-rw-rw-rw-   0        0        0       51 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/six_dof_collaborative_robot/__init__.py
+-rw-rw-rw-   0        0        0    10624 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/six_dof_collaborative_robot/six_dof_collab_robot.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.518651 robodyno-1.6.1b0/src/robodyno/robots/three_dof_delta_robot/
+-rw-rw-rw-   0        0        0       48 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/three_dof_delta_robot/__init__.py
+-rw-rw-rw-   0        0        0     9792 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/three_dof_delta_robot/three_dof_delta_robot.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.521643 robodyno-1.6.1b0/src/robodyno/robots/three_dof_palletizing_robot/
+-rw-rw-rw-   0        0        0       50 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/three_dof_palletizing_robot/__init__.py
+-rw-rw-rw-   0        0        0     7512 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/three_dof_palletizing_robot/three_dof_pallet_robot.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.524643 robodyno-1.6.1b0/src/robodyno/robots/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/utils/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/utils/interpolations.py
+-rw-rw-rw-   0        0        0    59522 2023-05-19 05:16:51.000000 robodyno-1.6.1b0/src/robodyno/robots/utils/transformations.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.530645 robodyno-1.6.1b0/src/robodyno/tools/
+-rw-rw-rw-   0        0        0        0 2023-05-18 09:35:59.000000 robodyno-1.6.1b0/src/robodyno/tools/__init__.py
+-rw-rw-rw-   0        0        0     4183 2023-05-18 04:13:40.000000 robodyno-1.6.1b0/src/robodyno/tools/can_bus_monitor.py
+-rw-rw-rw-   0        0        0    16396 2023-05-19 05:11:28.000000 robodyno-1.6.1b0/src/robodyno/tools/cli.py
+-rw-rw-rw-   0        0        0     3407 2023-05-19 03:16:35.000000 robodyno-1.6.1b0/src/robodyno/tools/cli_param_types.py
+-rw-rw-rw-   0        0        0     3992 2023-05-18 07:23:21.000000 robodyno-1.6.1b0/src/robodyno/tools/motor_info_table.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.484644 robodyno-1.6.1b0/src/robodyno.egg-info/
+-rw-rw-rw-   0        0        0    11028 2023-05-19 05:49:23.000000 robodyno-1.6.1b0/src/robodyno.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2202 2023-05-19 05:49:23.000000 robodyno-1.6.1b0/src/robodyno.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 05:49:23.000000 robodyno-1.6.1b0/src/robodyno.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1039 2023-05-19 05:49:23.000000 robodyno-1.6.1b0/src/robodyno.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      121 2023-05-19 05:49:23.000000 robodyno-1.6.1b0/src/robodyno.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 05:49:23.000000 robodyno-1.6.1b0/src/robodyno.egg-info/top_level.txt
```

### Comparing `robodyno-1.6.0/PKG-INFO` & `robodyno-1.6.1b0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,535 +1,535 @@
-Metadata-Version: 2.1
-Name: robodyno
-Version: 1.6.0
-Summary: The Robodyno Robot SDK for Python 3
-Home-page: http://101.42.250.169/
-Author: song
-Author-email: zhaosongy@126.com
-Maintainer: robottime
-Maintainer-email: lab@robottime.cn
-License: MIT License
-Keywords: robodyno,robot,robot module
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Framework :: Robot Framework
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# Robodyno
-
-## 安装
-[安装Python(>=3.7)](https://www.python.org/downloads/)
-
-使用pip安装robodyno库
-
-```
-pip install robodyno
-````
-
-## Python API
-
-### 1. 初始化电机对象
-
-```python
-from robodyno.components import Motor
-from robodyno.interfaces import CanBus
-can = CanBus()
-motor = Motor(can, 0x10)
-```
-`Motor(iface, id, type)`  
-参数 ：
-- iface : robodyno 接口对象
-- id : 电机ID（ 范围从 0x01 到 0x3F ）
-- type : 电机的类型，默认自动识别
-    - ROBODYNO_PRO_44
-    - ROBODYNO_PRO_12
-    - ROBODYNO_PRO_50
-    - ROBODYNO_PRO_100
-
-### 2. 读取电机状态
-
-```python
-motor.state
-```
-`state`  
-返回值 ：
-- 电机状态 （1-空闲，8-使能）
-
-### 3. 读取电机错误
-
-```python
-motor.error
-```
-`error`  
-返回值 :  
-- 电机错误 dict  
-    - error : 错误码（1-电压不足，14-急停）  
-    - motor : 电机相关错误码  
-    - encoder_err : 编码器相关错误码  
-    - controller_err : 控制器相关错误码  
-
-
-
-### 4. 读取电机模式
-
-```python
-motor.mode
-```
-`mode`  
-返回值：  
-- 电机模式 dict （control_mode，input_mode）  
-- control_mode : 控制模式（ 1-力矩模式，2-速度模式，3-位置模式 ）  
-- input_mode : 输入模式（ 1-直接值，2-带加速度，3-带滤波，5-梯形轨迹 )  
-
-### 5. 读取电机版本
-
-```python
-motor.get_version(1)
-```
-`get_api_version(timeout = 0)`  
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值 ：
-- API版本dict
-    - device_uuid : 设备uuid
-    - main_version : 主版本号
-    - sub_version : 副版本号
-
-### 6. 电机软急停
-
-```python
-motor.estop()
-```
-
-`estop()`  
-
-### 7. 电机重启
-
-```python
-motor.reboot()
-```
-
-`reboot()`  
-
-### 8. 清除错误
-
-```python
-motor.clear_errors()
-```
-
-`clear_errors()`
-
-### 9. 保存设置
-```python
-motor.save_configuration()
-```
-
-`save_configuration()`
-
-设置参数后默认不会保存，直到调用此函数
-
-### 10. 设置电机CAN_ID
-
-```python
-motor.config_can_bus(id = 0x10, heartbeat = 1)
-```
-
-`config_can_bus(new_id, heartbeat = 1, bitrate = 'CAN_1M')`
-
-参数 ：
-- new_id ：电机新CAN_ID (0x01~0x3F)
-- heartbeat : 心跳包发送周期 （ s ）
-
-### 11. 电机使能
-```python
-motor.enable()
-```
-
-`enable()`
-
-### 12. 电机失能
-
-```python
-motor.disable()
-```
-
-`disable()`
-
-### 13. 电机校准
-```python
-motor.calibrate()
-```
-
-`calibrate()`
-
-校准后需保存参数
-
-### 14. 读取总线电压
-```python
-motor.get_voltage(1)
-```
-
-`get_voltage(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值 ：
-- 总线电压值 ( V ) ，超时则不返回
-
-### 15. 读取电机温度
-```python
-motor.get_temperature(1)
-```
-
-`get_temperature(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 电机温度 ( °C ) ，超时则不返回
-
-### 16. 读取电机状态参数
-```python
-motor.get_feedback(1)
-```
-
-`get_feedback(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值 ：
-- 电机状态参数(位置rad, 速度rad/s, 力矩Nm)，超时则不返回
-
-
-### 17. 读取电机位置
-```python
-motor.get_pos(1)
-```
-
-`get_pos(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 位置(rad)，超时则不返回
-
-### 18. 读取电机绝对位置
-```python
-motor.get_abs_pos(1)
-```
-
-`get_abs_pos(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 绝对位置(rad)，断电不丢失，超时则不返回
-
-### 19. 读取电机速度
-```python
-motor.get_vel(1)
-```
-
-`get_vel(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 速度(rad/s)，超时则不返回
-
-### 20. 读取电机力矩
-```python
-motor.get_torque(1)
-```
-
-`get_torque(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 力矩(Nm)，超时则不返回
-
-### 21. 读取电机控制模式
-```python
-motor.get_mode(1)
-```
-`get_mode(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 控制模式(control_mode, input_mode)
-    - control_mode: 控制模式（1：力矩控制，2：速度控制，3：位置控制）
-    - input_mode: 输入模式（1：直接值，2：带加速度，3：带滤波，5：梯形轨迹)
-
-### 22. 进入直接位置模式
-```python
-motor.position_mode()
-```
-`position_mode()`
-
-直接PID控制位置
-
-### 23. 进入滤波位置模式
-```python
-motor.position_filter_mode(4)
-```
-`position_filter_mode(bandwidth)`
-
-参数：
-- bandwidth: 滤波带宽 / 控制频率(Hz)
-
-### 24. 进入轨迹位置模式
-```python
-motor.position_track_mode(10,5,5)
-```
-`position_track_mode(vel, acc, dec)`
-
-参数:
-- vel: 运动最高速度 ( rad/s ) 
-- acc: 运动加速度 ( rad/s^2 ) 
-- dec: 运动减速度 ( rad/s^2 ) 
-
-### 25. 进入直接速度模式
-```python
-motor.velocity_mode()
-```
-`velocity_mode()`
-
-速度PID控制
-
-### 26. 进入匀加减速速度模式
-```python
-motor.velocity_ramp_mode(1.414)
-```
-`velocity_ramp_mode(ramp)`
-
-参数:
-- ramp: 加速度(rad/s^2)
-
-### 27. 进入力矩控制模式
-```python
-motor.torque_mode()
-```
-`torque_mode()`
-
-### 28. 读取电机PID参数
-```python
-motor.get_pid(1)
-```
-`get_pid(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 电机PID
-    - pos_kp : 位置环P
-    - vel_kp : 速度环P
-    - vel_ki : 速度环I
-
-### 29. 设置电机PID参数
-```python
-motor.set_pid(100,0.02,0.005)
-```
-`set_pid(pos_kp, vel_kp, vel_ki)`
-
-参数:
-- pos_kp: 位置环比例系数
-- vel_kp: 速度环比例系数
-- vel_ki: 速度环积分系数
-
-### 30. 读取电机速度限制
-```python
-motor.get_vel_limit()
-```
-`get_vel_limit(timeout = 0)`
-
-参数:
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 输出端最大速度(rad/s)，超时则不返回
-
-### 31. 读取电机电流限制
-```python
-motor.get_current_limit()
-```
-
-`get_current_limit(timeout = 0)`
-
-参数:
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 最大电流(A)，超时则不返回
-
-### 32. 设置电机速度限制
-```python
-motor.set_vel_limit(3.14)
-```
-
-`set_vel_limit(vel_lim)`
-
-参数：
-- vel_lim: 输出端最大速度(rad/s)
-
-### 33. 设置电机电流限制
-```python
-motor.set_current_limit(10)
-```
-`set_current_limit(current_lim)`
-
-参数:
-- current_lim : 最大电流(A)
-
-### 34. 设置位置
-```python
-motor.set_pos(-1.57)
-```
-`set_pos(pos)`
-
-参数:
-- pos: 目标位置(rad)
-
-### 35. 设置绝对位置
-```python
-motor.set_abs_pos(-1.57)
-```
-`set_abs_pos(pos)`
-
-参数:
-- pos: 目标绝对位置(rad)
-
-### 36. 设置速度
-```python
-motor.set_vel(-0.5)
-```
-`set_vel(velocity)`
-
-参数：
-- velocity: 目标速度(rad/s)
-
-### 37. 设置力矩
-```python
-motor.set_torque(0.0)
-```
-`set_torque(torque)`
-
-参数：
-- torque: 目标力矩(Nm)
-
-### 38. 恢复出厂设置
-```python
-motor.reset()
-```
-`reset()`
-
-## 命令行工具
-
-1. robodyno
-- -c, --channel: CAN总线通道选项（可选，默认can0）
-- -b, --bitrate: CAN总线速率选项（可选，默认CAN_1M）
-- -h, --help: 显示帮助信息
-
-    `robodyno -h`
-
-- list: 列举总线上所有robodyno设备
-
-    -   例：当前CAN总线速率为1000K，通道为can0，列举所有robodyno设备
-
-        `robodyno list`
-
-- monitor: 监听总线上所有消息
-
-    - 例：当前CAN总线速率为500K，监听CAN总线上的实时消息
-
-        `robodyno monitor -b CAN_500K`
-
-2. robodyno-motor
-- -c, --channel: CAN总线通道选项（可选，默认can0）
-- -b, --bitrate: CAN总线速率选项（可选，默认CAN_1M）
-- --id: 需要操作的电机ID（可选，可传多个，默认0x10）
-- -h, --help: 显示帮助信息
-
-    `robodyno-motor -h`
-
-- enable: 电机使能
-
-    - 例：将ID为0x10的电机使能
-
-        `robodyno-motor enable`
-
-- disable: 电机失能
-
-    - 例：将ID为0x11的电机失能
-
-        `robodyno-motor disable --id 0x11`
-
-- info: 显示电机状态信息
-
-    - 例：显示ID为0x12、0x13及0x14的电机信息
-
-        `robodyno-motor info --id 0x12 0x13 0x14`
-
-- control: 控制电机运动
-
-    - -p, --pos: 指定电机运动位置(rad)
-
-    - 例：将电机转动到相对开机初始位置180°的位置
-
-        `robodyno-motor control -p 3.14`
-
-    - -ap, --abs-pos: 指定电机绝对位置（仅支持部分型号）(rad)
-
-    - 例：将ID为0x10的电机转动到相对复位位置180°的位置
-
-        `robodyno-motor control -ap 3.14`
-
-    - -v, --vel: 指定电机运动速度(rad/s)
-
-    - 例：操作ID为0x11的电机以15rpm的速度转动
-
-        `robodyno-motor control --id 0x11 -v 1.57`
-
-    - -t, --torque: 指定电机输出力矩(Nm)
-
-    - 例：操作ID为0x12, 0x13及0x14的电机输出0.1Nm的扭矩
-
-        `robodyno-motor control --id 0x12 0x13 0x14 -t 0.1`
-
-- config --new-id [-s, --save]: 修改电机ID，只能同时操作一个电机，-s 保存设置
-
-    - 例：将原ID为0x10的电机ID更改为0x11并保存
-
-        `robodyno-motor config --new-id 0x11 -s`
-    
-    - 例：将原ID为0x11的电机ID临时更改为0x10（断电后ID仍为0x11）
-
-        `robodyno-motor config --id 0x11 --new-id 0x10`
-
-- reset: 将电机恢复出厂设置（重新校准，ID复原为0x10）
-    
-    - 例：将ID为0x11的电机恢复出厂设置
-
-        `robodyno-motor reset --id 0x11`
+Metadata-Version: 2.1
+Name: robodyno
+Version: 1.6.1b0
+Summary: The Robodyno Robot SDK for Python 3
+Home-page: http://101.42.250.169/
+Author: song
+Author-email: zhaosongy@126.com
+Maintainer: robottime
+Maintainer-email: lab@robottime.cn
+License: MIT License
+Keywords: robodyno,robot,robot module
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Framework :: Robot Framework
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# Robodyno
+
+## 安装
+[安装Python(>=3.7)](https://www.python.org/downloads/)
+
+使用pip安装robodyno库
+
+```
+pip install robodyno
+````
+
+## Python API
+
+### 1. 初始化电机对象
+
+```python
+from robodyno.components import Motor
+from robodyno.interfaces import CanBus
+can = CanBus()
+motor = Motor(can, 0x10)
+```
+`Motor(iface, id, type)`  
+参数 ：
+- iface : robodyno 接口对象
+- id : 电机ID（ 范围从 0x01 到 0x3F ）
+- type : 电机的类型，默认自动识别
+    - ROBODYNO_PRO_44
+    - ROBODYNO_PRO_12
+    - ROBODYNO_PRO_50
+    - ROBODYNO_PRO_100
+
+### 2. 读取电机状态
+
+```python
+motor.state
+```
+`state`  
+返回值 ：
+- 电机状态 （1-空闲，8-使能）
+
+### 3. 读取电机错误
+
+```python
+motor.error
+```
+`error`  
+返回值 :  
+- 电机错误 dict  
+    - error : 错误码（1-电压不足，14-急停）  
+    - motor : 电机相关错误码  
+    - encoder_err : 编码器相关错误码  
+    - controller_err : 控制器相关错误码  
+
+
+
+### 4. 读取电机模式
+
+```python
+motor.mode
+```
+`mode`  
+返回值：  
+- 电机模式 dict （control_mode，input_mode）  
+- control_mode : 控制模式（ 1-力矩模式，2-速度模式，3-位置模式 ）  
+- input_mode : 输入模式（ 1-直接值，2-带加速度，3-带滤波，5-梯形轨迹 )  
+
+### 5. 读取电机版本
+
+```python
+motor.get_version(1)
+```
+`get_api_version(timeout = 0)`  
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值 ：
+- API版本dict
+    - device_uuid : 设备uuid
+    - main_version : 主版本号
+    - sub_version : 副版本号
+
+### 6. 电机软急停
+
+```python
+motor.estop()
+```
+
+`estop()`  
+
+### 7. 电机重启
+
+```python
+motor.reboot()
+```
+
+`reboot()`  
+
+### 8. 清除错误
+
+```python
+motor.clear_errors()
+```
+
+`clear_errors()`
+
+### 9. 保存设置
+```python
+motor.save() # or motor.save_configuration()
+```
+
+`save()`
+
+设置参数后默认不会保存，直到调用此函数
+
+### 10. 设置电机CAN_ID
+
+```python
+motor.config_can_bus(new_id = 0x11, heartbeat = 1)
+```
+
+`config_can_bus(new_id, heartbeat = 1, bitrate = 'CAN_1M')`
+
+参数 ：
+- new_id ：电机新CAN_ID (0x01~0x3F)
+- heartbeat : 心跳包发送周期 （ s ）
+
+### 11. 电机使能
+```python
+motor.enable()
+```
+
+`enable()`
+
+### 12. 电机失能
+
+```python
+motor.disable()
+```
+
+`disable()`
+
+### 13. 电机校准
+```python
+motor.calibrate()
+```
+
+`calibrate()`
+
+校准后需保存参数
+
+### 14. 读取总线电压
+```python
+motor.get_voltage(1)
+```
+
+`get_voltage(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值 ：
+- 总线电压值 ( V ) ，超时则不返回
+
+### 15. 读取电机温度
+```python
+motor.get_temperature(1)
+```
+
+`get_temperature(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 电机温度 ( °C ) ，超时则不返回
+
+### 16. 读取电机状态参数
+```python
+motor.get_feedback(1)
+```
+
+`get_feedback(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值 ：
+- 电机状态参数(位置rad, 速度rad/s, 力矩Nm)，超时则不返回
+
+
+### 17. 读取电机位置
+```python
+motor.get_pos(1)
+```
+
+`get_pos(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 位置(rad)，超时则不返回
+
+### 18. 读取电机绝对位置
+```python
+motor.get_abs_pos(1)
+```
+
+`get_abs_pos(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 绝对位置(rad)，断电不丢失，超时则不返回
+
+### 19. 读取电机速度
+```python
+motor.get_vel(1)
+```
+
+`get_vel(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 速度(rad/s)，超时则不返回
+
+### 20. 读取电机力矩
+```python
+motor.get_torque(1)
+```
+
+`get_torque(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 力矩(Nm)，超时则不返回
+
+### 21. 读取电机控制模式
+```python
+motor.get_mode(1)
+```
+`get_mode(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 控制模式(control_mode, input_mode)
+    - control_mode: 控制模式（1：力矩控制，2：速度控制，3：位置控制）
+    - input_mode: 输入模式（1：直接值，2：带加速度，3：带滤波，5：梯形轨迹)
+
+### 22. 进入直接位置模式
+```python
+motor.position_mode()
+```
+`position_mode()`
+
+直接PID控制位置
+
+### 23. 进入滤波位置模式
+```python
+motor.position_filter_mode(4)
+```
+`position_filter_mode(bandwidth)`
+
+参数：
+- bandwidth: 滤波带宽 / 控制频率(Hz)
+
+### 24. 进入轨迹位置模式
+```python
+motor.position_track_mode(10,5,5)
+```
+`position_track_mode(vel, acc, dec)`
+
+参数:
+- vel: 运动最高速度 ( rad/s ) 
+- acc: 运动加速度 ( rad/s^2 ) 
+- dec: 运动减速度 ( rad/s^2 ) 
+
+### 25. 进入直接速度模式
+```python
+motor.velocity_mode()
+```
+`velocity_mode()`
+
+速度PID控制
+
+### 26. 进入匀加减速速度模式
+```python
+motor.velocity_ramp_mode(1.414)
+```
+`velocity_ramp_mode(ramp)`
+
+参数:
+- ramp: 加速度(rad/s^2)
+
+### 27. 进入力矩控制模式
+```python
+motor.torque_mode()
+```
+`torque_mode()`
+
+### 28. 读取电机PID参数
+```python
+motor.get_pid(1)
+```
+`get_pid(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 电机PID
+    - pos_kp : 位置环P
+    - vel_kp : 速度环P
+    - vel_ki : 速度环I
+
+### 29. 设置电机PID参数
+```python
+motor.set_pid(100,0.02,0.005)
+```
+`set_pid(pos_kp, vel_kp, vel_ki)`
+
+参数:
+- pos_kp: 位置环比例系数
+- vel_kp: 速度环比例系数
+- vel_ki: 速度环积分系数
+
+### 30. 读取电机速度限制
+```python
+motor.get_vel_limit()
+```
+`get_vel_limit(timeout = 0)`
+
+参数:
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 输出端最大速度(rad/s)，超时则不返回
+
+### 31. 读取电机电流限制
+```python
+motor.get_current_limit()
+```
+
+`get_current_limit(timeout = 0)`
+
+参数:
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 最大电流(A)，超时则不返回
+
+### 32. 设置电机速度限制
+```python
+motor.set_vel_limit(3.14)
+```
+
+`set_vel_limit(vel_lim)`
+
+参数：
+- vel_lim: 输出端最大速度(rad/s)
+
+### 33. 设置电机电流限制
+```python
+motor.set_current_limit(10)
+```
+`set_current_limit(current_lim)`
+
+参数:
+- current_lim : 最大电流(A)
+
+### 34. 设置位置
+```python
+motor.set_pos(-1.57)
+```
+`set_pos(pos)`
+
+参数:
+- pos: 目标位置(rad)
+
+### 35. 设置绝对位置
+```python
+motor.set_abs_pos(-1.57)
+```
+`set_abs_pos(pos)`
+
+参数:
+- pos: 目标绝对位置(rad)
+
+### 36. 设置速度
+```python
+motor.set_vel(-0.5)
+```
+`set_vel(velocity)`
+
+参数：
+- velocity: 目标速度(rad/s)
+
+### 37. 设置力矩
+```python
+motor.set_torque(0.0)
+```
+`set_torque(torque)`
+
+参数：
+- torque: 目标力矩(Nm)
+
+### 38. 恢复出厂设置
+```python
+motor.reset()
+```
+`reset()`
+
+## 命令行工具
+
+1. robodyno
+- -c, --channel: CAN总线通道选项（可选，默认can0）
+- -b, --bitrate: CAN总线速率选项（可选，默认CAN_1M）
+- -h, --help: 显示帮助信息
+
+    `robodyno -h`
+
+- list: 列举总线上所有robodyno设备
+
+    -   例：当前CAN总线速率为1000K，通道为can0，列举所有robodyno设备
+
+        `robodyno list`
+
+- monitor: 监听总线上所有消息
+
+    - 例：当前CAN总线速率为500K，监听CAN总线上的实时消息
+
+        `robodyno monitor -b CAN_500K`
+
+2. robodyno-motor
+- -c, --channel: CAN总线通道选项（可选，默认can0）
+- -b, --bitrate: CAN总线速率选项（可选，默认CAN_1M）
+- --id: 需要操作的电机ID（可选，可传多个，默认0x10）
+- -h, --help: 显示帮助信息
+
+    `robodyno-motor -h`
+
+- enable: 电机使能
+
+    - 例：将ID为0x10的电机使能
+
+        `robodyno-motor enable`
+
+- disable: 电机失能
+
+    - 例：将ID为0x11的电机失能
+
+        `robodyno-motor disable --id 0x11`
+
+- info: 显示电机状态信息
+
+    - 例：显示ID为0x12、0x13及0x14的电机信息
+
+        `robodyno-motor info --id 0x12 0x13 0x14`
+
+- control: 控制电机运动
+
+    - -p, --pos: 指定电机运动位置(rad)
+
+    - 例：将电机转动到相对开机初始位置180°的位置
+
+        `robodyno-motor control -p 3.14`
+
+    - -ap, --abs-pos: 指定电机绝对位置（仅支持部分型号）(rad)
+
+    - 例：将ID为0x10的电机转动到相对复位位置180°的位置
+
+        `robodyno-motor control -ap 3.14`
+
+    - -v, --vel: 指定电机运动速度(rad/s)
+
+    - 例：操作ID为0x11的电机以15rpm的速度转动
+
+        `robodyno-motor control --id 0x11 -v 1.57`
+
+    - -t, --torque: 指定电机输出力矩(Nm)
+
+    - 例：操作ID为0x12, 0x13及0x14的电机输出0.1Nm的扭矩
+
+        `robodyno-motor control --id 0x12 0x13 0x14 -t 0.1`
+
+- config --new-id [-s, --save]: 修改电机ID，只能同时操作一个电机，-s 保存设置
+
+    - 例：将原ID为0x10的电机ID更改为0x11并保存
+
+        `robodyno-motor config --new-id 0x11 -s`
+    
+    - 例：将原ID为0x11的电机ID临时更改为0x10（断电后ID仍为0x11）
+
+        `robodyno-motor config --id 0x11 --new-id 0x10`
+
+- reset: 将电机恢复出厂设置（重新校准，ID复原为0x10）
+    
+    - 例：将ID为0x11的电机恢复出厂设置
+
+        `robodyno-motor reset --id 0x11`
```

### Comparing `robodyno-1.6.0/src/robodyno/components/can_bus/motor.py` & `robodyno-1.6.1b0/src/robodyno/components/webots/motor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,711 +1,550 @@
-#!/usr/bin/env python
-# -*-coding:utf-8 -*-
-"""motor.py
-Time    :   2023/01/03
-Author  :   song 
-Version :   1.0
-Contact :   zhaosongy@CanBus.126.com
-License :   (C)Copyright 2022, robottime / robodyno
-
-Robodyno motor can bus driver
-
-  Typical usage example:
-
-  from robodyno.interfaces import CanBus, Webots
-  from robodyno.components import Motor
-
-  can = CanBus()
-  webots = Webots()
-  
-  motor_can = Motor(iface = can, id = 0x10, type = 'ROBODYNO_PRO_44')
-  motor_webots = Motor(iface = webots, id = 0x11, type = 'ROBODYNO_PRO_12')
-
-  can.disconnect()
-"""
-
-import time
-from math import pi, fabs
-from enum import Enum
-import struct
-
-from robodyno.interfaces import CanBus
-from robodyno.components import DeviceType, ROBODYNO_MOTOR_SPECS, CanBusDevice
-
-class Motor(CanBusDevice):
-    """Robodyno Motor
-    
-    Attributes:
-        id: correspond with motor id in real world or simulation.
-        type: motor type enum
-        reduction: motor reduction
-        available_velocity: theoretical max velocity(rad/s)
-        available_torque: theoretical max torque(Nm)
-        available_current: theoretical max phase current(A)
-        torque_constant: theoretical torque provided by unit current(Nm/A)
-        with_brake: is motor has a brake(bool)
-        state: motor state read from heartbeat pack
-        error: motor error read from heartbeat pack
-        mode: motor mode read from heartbeat pack
-        sync_time: last timestamp when receive heartbeat pack
-    """
-
-    class MotorApiRuntimeError(RuntimeError):
-        def __init__(self):
-            super().__init__('Failed to invoke motor api from interface.')
-
-    class MotorState(Enum):
-        UNKNOWN = -1
-        DISABLED = 1
-        CALIBRATE = 3
-        MOTOR_CALIBRATING = 4
-        OFFSET_CALIBRATING = 7
-        ENABLED = 8
-
-    class MotorError(Enum):
-        NONE = 0
-        INVALID_STATE = 1
-        UNDER_VOLTAGE = 2
-        OVER_VOLTAGE = 3
-        CURRENT_MEASUREMENT_TIMEOUT = 4
-        BRAKE_RESISTOR_DISARMED = 5
-        MOTOR_DISARMED = 6
-        MOTOR_FAILED = 7
-        SENSORLESS_ESTIMATOR_FAILED = 8
-        ENCODER_FAILED = 9
-        CONTROLLER_FAILED = 10
-        POS_CTRL_DURING_SENSORLESS = 11
-        WATCHDOG_TIMER_EXPIRED = 12
-        MIN_ENDSTOP_PRESSED = 13
-        MAX_ENDSTOP_PRESSED = 14
-        ESTOP_REQUESTED = 15
-        HOMING_WITHOUT_ENDSTOP = 16
-        OVER_TEMP = 17
-
-    class MotorMotorError(Enum):
-        NONE = 0
-        PHASE_RESISTANCE_OUT_OF_RANGE = 1
-        PHASE_INDUCTANCE_OUT_OF_RANGE = 2
-        ADC_FAILED = 3
-        DRV_FAULT = 4
-        CONTROL_DEADLINE_MISSED = 5
-        NOT_IMPLEMENTED_MOTOR_TYPE = 6
-        BRAKE_CURRENT_OUT_OF_RANGE = 7
-        MODULATION_MAGNITUDE = 8
-        BRAKE_DEADTIME_VIOLATION = 9
-        UNEXPECTED_TIMER_CALLBACK = 10
-        CURRENT_SENSE_SATURATION = 11
-        CURRENT_LIMIT_VIOLATION = 13
-        BRAKE_DUTY_CYCLE_NAN = 14
-        DC_BUS_OVER_REGEN_CURRENT = 15
-        DC_BUS_OVER_CURRENT = 16
-
-    class MotorEncoderError(Enum):
-        NONE = 0
-        UNSTABLE_GAIN = 1
-        CPR_POLEPAIRS_MISMATCH = 2
-        NO_RESPONSE = 3
-        UNSUPPORTED_ENCODER_MODE = 4
-        ILLEGAL_HALL_STATE = 5
-        INDEX_NOT_FOUND_YET = 6
-        ABS_SPI_TIMEOUT = 7
-        ABS_SPI_COM_FAIL = 8
-        ABS_SPI_NOT_READY = 9
-        
-    class MotorControllerError(Enum):
-        NONE = 0
-        OVERSPEED = 1
-        INVALID_INPUT_MODE = 2
-        UNSTABLE_GAIN = 3
-        INVALID_MIRROR_AXIS = 4
-        INVALID_LOAD_ENCODER = 5
-        INVALID_ESTIMATE = 6
-
-    class MotorControlMode(Enum):
-        UNKNOWN = -1
-        POSITION_MODE = 0
-        POSITION_FILTER_MODE = 1
-        POSITION_TRACK_MODE = 2
-        VELOCITY_MODE = 3
-        VELOCITY_RAMP_MODE = 4
-        TORQUE_MODE = 5
-
-    CMD_HEARTBEAT = 0x02
-    CMD_ESTOP = 0x03
-    CMD_REBOOT = 0x04
-    CMD_CLEAR_ERRORS = 0x05
-    CMD_SAVE = 0x06
-    CMD_CONFIG_CAN = 0x07
-    CMD_SET_STATE = 0x08
-    CMD_GET_HARDWARE_STATUS = 0x09
-    CMD_GET_MOTOR_FEEDBACK = 0x0A
-    CMD_GET_MODE = 0x0B
-    CMD_SET_MODE = 0x0C
-    CMD_GET_PID = 0x0D
-    CMD_SET_PID = 0x0E
-    CMD_GET_LIMITS = 0x0F
-    CMD_SET_LIMITS = 0x10
-    CMD_SET_POS = 0x11
-    CMD_SET_VEL = 0x12
-    CMD_SET_TORQUE = 0x13
-    CMD_RESET = 0x14
-    CMD_UNLOCK = 0x15
-    CMD_GET_ABS_POS = 0x16
-    CMD_SET_ABS_POS = 0x17
-    CMD_INIT_POS = 0x18
-    CMD_INIT_ABS_POS = 0x19
-    CMD_GET_STATE = 0x20
-
-    def __init__(self, iface, id = 0x10, type = None):
-        """Init motor from interface, id and type.
-        
-        Args:
-            iface: robodyno interface object
-            id: range from 0x01 to 0x40
-            type: Motor type string
-        """
-        super().__init__(iface, id)
-        valid_motor_types = [
-            DeviceType.ROBODYNO_PRO_44,
-            DeviceType.ROBODYNO_PRO_12,
-            DeviceType.ROBODYNO_PRO_50 ,
-            DeviceType.ROBODYNO_PRO_100,
-            DeviceType.ROBODYNO_PRO_DIRECT,
-            DeviceType.ROBODYNO_PLUS_50 ,
-            DeviceType.ROBODYNO_PLUS_100,
-            DeviceType.ROBODYNO_PLUS_12 ,
-            DeviceType.ROBODYNO_PLUS_DIRECT,
-            DeviceType.ROBODYNO_NANO_100,
-        ]
-        self.get_version(timeout=0.15)
-        if type:
-            self.type = DeviceType[type]
-        if self.type not in valid_motor_types:
-            raise ValueError('Motor type is invalid and can not distinguish automatically.')
-
-        self.__dict__.update(ROBODYNO_MOTOR_SPECS.get(self.type, None))
-        
-        self.state = self.MotorState.UNKNOWN
-        self.error = {
-            'error': self.MotorError.NONE,
-            'motor_err': self.MotorMotorError.NONE,
-            'encoder_err': self.MotorEncoderError.NONE,
-            'controller_err': self.MotorControllerError.NONE,
-        }
-        self.mode = self.MotorControlMode.UNKNOWN
-        self.sync_time = 0
-        if self.fw_ver >= 1:
-            self.get_state(1.5)
-
-        self._rot_factor = -self.reduction / 2.0 / pi
-        if self.fw_ver <= 0.3:
-            self._rot_factor = -self._rot_factor
-        self._iface.subscribe(
-            device_id = self.id, 
-            command_id = self.CMD_HEARTBEAT, 
-            callback = self._heartbeat_callback
-        )
-    
-    def __del__(self):
-        """Collect node from memory."""
-        self._iface.unsubscribe(
-            device_id = self.id, 
-            command_id = self.CMD_HEARTBEAT, 
-            callback = self._heartbeat_callback
-        )
-
-    def _heartbeat_callback(self, device_id, command_id, data, timestamp):
-        """Update motor attributes from heartbeat."""
-        state, err, merr, eerr, cerr, cm, im, _ = struct.unpack('<BBBBBBBB', data)
-        self.state = self.MotorState(state)
-        if self.fw_ver < 1:
-            self.error.update({
-                'error': self.MotorError(err+1 if err > 0 else 0),
-                'motor_err': self.MotorMotorError(merr+1 if merr > 0 else 0),
-                'encoder_err': self.MotorEncoderError(eerr+1 if eerr > 0 else 0),
-                'controller_err': self.MotorControllerError(cerr+1 if cerr > 0 else 0),
-            })
-        else:
-            self.error.update({
-                'error': self.MotorError(err),
-                'motor_err': self.MotorMotorError(merr),
-                'encoder_err': self.MotorEncoderError(eerr),
-                'controller_err': self.MotorControllerError(cerr),
-            })
-        self.mode = self._ctrl_mode_from_raw(cm, im)
-        self.sync_time = timestamp
-    
-    @CanBus.get_from_bus(CMD_GET_STATE, '<BBBBBBBB')
-    def get_state(self, state, err, merr, eerr, cerr, cm, im, type):
-        """Get motor state.
-        
-        Args:
-            timeout: 0 indicates unlimited timeout(s)
-        
-        Returns:
-            (state, error, mode)
-            None if timeout
-        """
-        self.state = self.MotorState(state)
-        if self.fw_ver < 1:
-            self.error.update({
-                'error': self.MotorError(err+1 if err > 0 else 0),
-                'motor_err': self.MotorMotorError(merr+1 if merr > 0 else 0),
-                'encoder_err': self.MotorEncoderError(eerr+1 if eerr > 0 else 0),
-                'controller_err': self.MotorControllerError(cerr+1 if cerr > 0 else 0),
-            })
-        else:
-            self.error.update({
-                'error': self.MotorError(err),
-                'motor_err': self.MotorMotorError(merr),
-                'encoder_err': self.MotorEncoderError(eerr),
-                'controller_err': self.MotorControllerError(cerr),
-            })
-        self.mode = self._ctrl_mode_from_raw(cm, im)
-        return (self.state, self.error, self.mode)
-
-    def _ctrl_mode_to_raw(self, mode):
-        """Translate from control mode enum to control mode raw msg
-        
-        Args:
-            mode: control mode enum
-        
-        Returns:
-            tuple of raw msg: (control mode, input mode)
-            None when mode not recognized
-        """
-        if mode == self.MotorControlMode.POSITION_MODE:
-            return (3, 1)
-        elif mode == self.MotorControlMode.POSITION_FILTER_MODE:
-            return (3, 3)
-        elif mode == self.MotorControlMode.POSITION_TRACK_MODE:
-            return (3, 5)
-        elif mode == self.MotorControlMode.VELOCITY_MODE:
-            return (2, 1)
-        elif mode == self.MotorControlMode.VELOCITY_RAMP_MODE:
-            return (2, 2)
-        elif mode == self.MotorControlMode.TORQUE_MODE:
-            return (1, 1)
-        else:
-            return None
-
-    def _ctrl_mode_from_raw(self, cmode, imode):
-        """Translate from control mode raw msg to control mode enum
-        
-        Args:
-            cmode: raw control mode
-            imode: raw input mode
-        
-        Returns:
-            control mode enum
-        """
-        if cmode == 3:
-            if imode == 1:
-                return self.MotorControlMode.POSITION_MODE
-            elif imode == 3:
-                return self.MotorControlMode.POSITION_FILTER_MODE
-            elif imode == 5:
-                return self.MotorControlMode.POSITION_TRACK_MODE
-        if cmode == 2:
-            if imode == 1:
-                return self.MotorControlMode.VELOCITY_MODE
-            elif imode == 2:
-                return self.MotorControlMode.VELOCITY_RAMP_MODE
-        if cmode == 1 and imode == 1:
-            return self.MotorControlMode.TORQUE_MODE
-        return self.MotorControlMode.UNKNOWN
-    
-    @CanBus.send_to_bus(CMD_ESTOP)
-    def estop(self):
-        """Emergency stop motor."""
-        pass
-
-    @CanBus.send_to_bus(CMD_REBOOT)
-    def reboot(self):
-        """Reboot motor."""
-        pass
-
-    @CanBus.send_to_bus(CMD_CLEAR_ERRORS)
-    def clear_errors(self):
-        """Try to clear motor errors."""
-        pass
-
-    @CanBus.send_to_bus(CMD_SAVE)
-    def _save(self):
-        """Save configurations to hardware."""
-        pass
-
-    def save_configuration(self):
-        """Save configurations to hardware."""
-        self._save()
-        self.clear_errors()
-
-    @CanBus.send_to_bus(CMD_CONFIG_CAN, '<HHI')
-    def config_can_bus(self, new_id, heartbeat = 1000, bitrate = 'CAN_1M'):
-        """Configure motor can bus settings.
-        
-        Args:
-            new_id: motor device id(0x01-0x3f)
-            heartbeat: heartbeat period(ms)
-            bitrate: choose from 'CAN_1000K', 'CAN_500K', 'CAN_250K',
-                     (save and reboot to take effect)
-        """
-        if new_id < 0x01 or new_id > 0x3f:
-            raise ValueError('Unavailable can id. Choose from 0x01-0x3f')
-
-        bitrate = CanBus.CanSpeed[bitrate].value
-        if bitrate == 250000:
-            bitrate_id = 0
-        elif bitrate == 500000:
-            bitrate_id = 1
-        else:
-            bitrate_id = 2
-        return (new_id, bitrate_id, int(heartbeat))
-
-    @CanBus.send_to_bus(CMD_SET_STATE, '<I')
-    def set_state(self, state):
-        """Cange motor state.
-        
-        Args:
-            state: motor state(MotorState)
-        """
-        return (state.value,)
-
-    def enable(self):
-        """Enable motor. Set motor state to CLOSED_LOOP."""
-        try:
-            self.set_state(self.MotorState.ENABLED)
-            time.sleep(0.02)
-        except:
-            raise self.MotorApiRuntimeError
-    
-    def calibrate(self):
-        """Calibrate motor. Set motor state to CALIBRATE."""
-        try:
-            self.set_state(self.MotorState.CALIBRATE)
-        except:
-            raise self.MotorApiRuntimeError
-    
-    def disable(self):
-        """Disable motor. Set motor state to IDLE."""
-        try:
-            self.set_state(self.MotorState.DISABLED)
-        except:
-            raise self.MotorApiRuntimeError
-
-    @CanBus.get_from_bus(CMD_GET_HARDWARE_STATUS, '<ff')
-    def get_voltage(self, vbus, temperature):
-        """Get motor vbus voltage.
-        
-        Args:
-            timeout: 0 indicates unlimited timeout(s)
-        
-        Returns:
-            voltage(V)
-            None if timeout
-        """
-        return vbus
-    
-    @CanBus.get_from_bus(CMD_GET_HARDWARE_STATUS, '<ff')
-    def get_temperature(self, vbus, temperature):
-        """Get motor temperature.
-        
-        Args:
-            timeout: 0 indicates unlimited timeout(s)
-        
-        Returns:
-            temperature(°C)
-            None if timeout
-        """
-        return temperature
-    
-    @CanBus.get_from_bus(CMD_GET_MOTOR_FEEDBACK, '<fee')
-    def get_feedback(self, pos, vel, torque):
-        """Get motor position, velocity and torque feedback.
-        
-        Args:
-            timeout: 0 indicates unlimited timeout(s)
-        
-        Returns:
-            position(rad), velocity(rad/s), torque(Nm)
-            None if timeout
-        """
-        return pos / self._rot_factor, vel / self._rot_factor, torque * self.reduction
-
-    def get_pos(self, timeout = 0):
-        """Get motor position.
-        
-        Args:
-            timeout: 0 indicates unlimited timeout(s)
-        
-        Returns:
-            position(rad)
-            None if timeout
-        """
-        try:
-            return self.get_feedback(timeout)[0]
-        except:
-            raise self.MotorApiRuntimeError
-
-    @CanBus.get_from_bus(CMD_GET_ABS_POS, '<f')
-    def get_abs_pos(self, pos):
-        """Get motor absolute position.
-        
-        Args:
-            timeout: 0 indicates unlimited timeout(s)
-        
-        Returns:
-            position(rad)
-            None if timeout
-        """
-        return pos / self._rot_factor
-    
-    def get_vel(self, timeout = 0):
-        """Get motor velocity.
-        
-        Args:
-            timeout: 0 indicates unlimited timeout(s)
-        
-        Returns:
-            velocity(rad/s)
-            None if timeout
-        """
-        try:
-            return self.get_feedback(timeout)[1]
-        except:
-            raise self.MotorApiRuntimeError
-    
-    def get_torque(self, timeout = 0):
-        """Get motor torque.
-        
-        Args:
-            timeout: 0 indicates unlimited timeout(s)
-        
-        Returns:
-            torque(Nm)
-            None if timeout
-        """
-        try:
-            return self.get_feedback(timeout)[2]
-        except:
-            raise self.MotorApiRuntimeError
-    
-    @CanBus.get_from_bus(CMD_GET_MODE, '8s')
-    def get_mode(self, payload):
-        """Get motor control mode and params.
-        
-        Args:
-            timeout: 0 indicates unlimited timeout(s)
-        
-        Returns:
-            control mode(MotorControlMode), control params dict
-            None if timeout
-        """
-        control_mode, input_mode = struct.unpack('<BB', payload[:2])
-        mode = self._ctrl_mode_from_raw(control_mode, input_mode)
-        self.mode = mode
-        if mode == self.MotorControlMode.POSITION_FILTER_MODE:
-            bandwidth, = struct.unpack('<f', payload[2:6])
-            return (mode, {'bandwidth': bandwidth})
-        elif mode == self.MotorControlMode.POSITION_TRACK_MODE:
-            vel, acc, dec = struct.unpack('<eee', payload[2:8])
-            return (mode, {
-                'vel': fabs(vel / self._rot_factor),
-                'acc': fabs(acc / self._rot_factor),
-                'dec': fabs(dec / self._rot_factor),
-            })
-        elif mode == self.MotorControlMode.VELOCITY_RAMP_MODE:
-            ramp, = struct.unpack('<f', payload[2:6])
-            return (mode, {'ramp': fabs(ramp / self._rot_factor)})
-        else:
-            return (mode, )
-    
-    @CanBus.send_to_bus(CMD_SET_MODE, '<BB')
-    def position_mode(self):
-        """Enter position pid mode."""
-        return self._ctrl_mode_to_raw(self.MotorControlMode.POSITION_MODE)
-
-    @CanBus.send_to_bus(CMD_SET_MODE, '<BBf')
-    def position_filter_mode(self, bandwidth):
-        """Enter position filter mode.
-        
-        Args:
-            bandwidth: filter bandwith, equals to control frequency(Hz)
-        """
-        cmode, imode = self._ctrl_mode_to_raw(self.MotorControlMode.POSITION_FILTER_MODE)
-        return (cmode, imode, bandwidth)
-    
-    @CanBus.send_to_bus(CMD_SET_MODE, '<BBeee')
-    def position_track_mode(self, vel, acc, dec):
-        """Enter position track mode.
-        
-        Args:
-            vel: motion max vel(rad/s)
-            acc: motion acceleration(rad/s^2)
-            dec: motion deceleration(rad/s^2)
-        """
-        cmode, imode = self._ctrl_mode_to_raw(self.MotorControlMode.POSITION_TRACK_MODE)
-        return (
-            cmode, 
-            imode, 
-            fabs(vel * self._rot_factor), 
-            fabs(acc * self._rot_factor), 
-            fabs(dec * self._rot_factor)
-        )
-    
-    @CanBus.send_to_bus(CMD_SET_MODE, '<BB')
-    def velocity_mode(self):
-        """Enter velocity mode."""
-        return self._ctrl_mode_to_raw(self.MotorControlMode.VELOCITY_MODE)
-    
-    @CanBus.send_to_bus(CMD_SET_MODE, '<BBf')
-    def velocity_ramp_mode(self, ramp):
-        """Enter velocity ramp mode.
-        
-        Args:
-            ramp: motion acceleration(rad/s^2)
-        """
-        cmode, imode = self._ctrl_mode_to_raw(self.MotorControlMode.VELOCITY_RAMP_MODE)
-        return (cmode, imode, fabs(ramp * self._rot_factor))
-    
-    @CanBus.send_to_bus(CMD_SET_MODE, '<BB')
-    def torque_mode(self):
-        """Enter torque mode"""
-        return self._ctrl_mode_to_raw(self.MotorControlMode.TORQUE_MODE)
-    
-    @CanBus.get_from_bus(CMD_GET_PID, '<fee')
-    def get_pid(self, pos_kp, vel_kp, vel_ki):
-        """Get motor pid params.
-        
-        Args:
-            timeout: 0 indicates unlimited timeout(s)
-        
-        Returns:
-            pos_kp, vel_kp, vel_ki
-            None if timeout
-        """
-        return (pos_kp, vel_kp, vel_ki)
-    
-    @CanBus.send_to_bus(CMD_SET_PID, '<fee')
-    def set_pid(self, pos_kp, vel_kp, vel_ki):
-        """Set motor pid params.
-        
-        Args:
-            pos_kp: kp of position control
-            vel_kp: kp of velocity control
-            vel_ki: ki of velocity control
-        """
-        return (pos_kp, vel_kp, vel_ki)
-
-    @CanBus.get_from_bus(CMD_GET_LIMITS, '<ff')
-    def get_vel_limit(self, vel_limit, current_limit):
-        """Get motor volocity limit.
-        
-        Args:
-            timeout: 0 indicates unlimited timeout(s)
-        
-        Returns:
-            velocity limit(rad/s)
-            None if timeout
-        """
-        return vel_limit / fabs(self._rot_factor)
-    
-    @CanBus.get_from_bus(CMD_GET_LIMITS, '<ff')
-    def get_current_limit(self, vel_limit, current_limit):
-        """Get motor current limit.
-        
-        Args:
-            timeout: 0 indicates unlimited timeout(s)
-        
-        Returns:
-            current limit(A)
-            None if timeout
-        """
-        return current_limit
-
-    @CanBus.send_to_bus(CMD_SET_LIMITS, '<ff')
-    def set_vel_limit(self, vel_lim):
-        """Set motor velocity limit.
-        
-        Args:
-            vel_lim: velocity limit(rad/s)
-        """
-        return (fabs(vel_lim * self._rot_factor), 0)
-    
-    @CanBus.send_to_bus(CMD_SET_LIMITS, '<ff')
-    def set_current_limit(self, current_lim):
-        """Set motor current limit.
-        
-        Args:
-            current_lim: current limit(A)
-        """
-        return (0, current_lim)
-    
-    @CanBus.send_to_bus(CMD_SET_POS, '<fee')
-    def set_pos(self, pos, vel_ff = 0, torque_ff = 0):
-        """Set motor target position.
-        
-        Args:
-            pos: target position(rad)
-            vel_ff: velocity feed forward(rad/s)
-            torque_ff:torque feed forward(Nm)
-        """
-        return (pos * self._rot_factor, vel_ff * self._rot_factor, torque_ff / self.reduction)
-    
-    @CanBus.send_to_bus(CMD_SET_ABS_POS, '<fee')
-    def set_abs_pos(self, pos, vel_ff = 0, torque_ff = 0):
-        """Set motor target absolute position.
-        
-        Args:
-            pos: target absolute position(rad)
-            vel_ff: velocity feed forward(rad/s)
-            torque_ff:torque feed forward(Nm)
-        """
-        return (pos * self._rot_factor, vel_ff * self._rot_factor, torque_ff / self.reduction)
-
-    @CanBus.send_to_bus(CMD_INIT_POS, '<f')
-    def init_pos(self, offset = 0):
-        """Init motor pos with current position.
-        
-        Args:
-            offset: current position(rad)
-        """
-        return (offset * self._rot_factor, )
-
-    @CanBus.send_to_bus(CMD_INIT_ABS_POS, '<f')
-    def init_abs_pos(self, offset = 0):
-        """Init motor absolute pos with current position.
-        
-        Args:
-            offset: current absolute position(rad)
-        """
-        return (offset * self._rot_factor, )
-
-    @CanBus.send_to_bus(CMD_SET_VEL, '<ff')
-    def set_vel(self, vel, torque_ff = 0):
-        """Set motor velocity.
-        
-        Args:
-            vel: target velocity(rad)
-            torque_ff: torque feed forward(Nm)
-        """
-        return (vel * self._rot_factor, torque_ff / self.reduction)
-    
-    @CanBus.send_to_bus(CMD_SET_TORQUE, '<f')
-    def set_torque(self, torque):
-        """Set motor torque.
-        
-        Args:
-            torque: target torque(Nm)
-        """
-        return (torque / self.reduction, )
-
-    @CanBus.send_to_bus(CMD_RESET)
-    def reset(self):
-        """Reset motor with factory configurations."""
-        pass
-
-    @CanBus.send_to_bus(CMD_UNLOCK)
-    def unlock(self):
-        """Unlock motor brake if motor has one."""
-        if not self.with_brake:
-            raise RuntimeError('Motor do not have a brake.')
+#!/usr/bin/env python
+# -*-coding:utf-8 -*-
+"""motor.py
+Time    :   2023/01/05
+Author  :   song 
+Version :   1.0
+Contact :   zhaosongy@126.com
+License :   (C)Copyright 2022, robottime / robodyno
+
+Robodyno motor webots bridge
+
+  Typical usage example:
+
+  from robodyno.interfaces import CanBus, Webots
+  from robodyno.components import Motor
+
+  can = CanBus()
+  webots = Webots()
+  
+  motor_can = Motor(iface = can, id = 0x10, type = 'ROBODYNO_PRO_44')
+  motor_webots = Motor(iface = webots, id = 0x11, type = 'ROBODYNO_PRO_12')
+
+  can.disconnect()
+"""
+
+from math import pi, fabs, copysign, sqrt
+from enum import Enum
+from robodyno.components import DeviceType, ROBODYNO_MOTOR_SPECS, WebotsDevice
+from robodyno.components.can_bus.motor import Motor as CanMotor
+from robodyno.interfaces import InterfaceType, GET_IFACE_TYPE
+
+class MotorPositionTrackController(object):
+    def __init__(self, max_vel, max_acc, max_dec):
+        self.max_vel = max_vel
+        self.max_acc = max_acc
+        self.max_dec = max_dec
+        self.target = 0
+        self.pos = 0
+        self.vel = 0
+        self.top_vel = 0
+        self.acc = 0
+        self.dec = 0
+        self.t = 0
+        self.t_acc = 0
+        self.t_dec = 0
+        self.t_vel = 0
+    
+    def set_pos(self, target_pos, pos, vel):
+        self.t = 0
+        self.target = target_pos
+        self.pos = pos
+        self.vel = vel
+
+        dx = self.target - self.pos
+        self.top_vel = self.max_vel if dx >= 0 else -self.max_vel
+        dx_stop = self.vel * fabs(self.vel) / (2.0 * self.max_dec)
+        s = copysign(1, dx - dx_stop)
+        self.top_vel = s * self.max_vel
+        self.acc = s * self.max_acc
+        self.dec = -s * self.max_dec
+        if s * self.vel > s * self.top_vel:
+            self.acc = -self.acc
+        self.t_acc = (self.top_vel - self.vel) / self.acc
+        self.t_dec = -self.top_vel / self.dec
+        dx_min = 0.5 * self.t_acc * (self.top_vel + self.vel) + 0.5 * self.t_dec * self.top_vel
+        if s * dx < s * dx_min:
+            self.top_vel = s * sqrt(max((self.dec*self.vel*self.vel + 2*self.acc*self.dec*dx) / (self.dec-self.acc), 0))
+            self.t_acc = max(0, (self.top_vel - self.vel) / self.acc)
+            self.t_dec = max(0, -self.top_vel / self.dec)
+            self.t_vel = 0
+        else:
+            self.t_vel = (dx - dx_min) / self.top_vel
+        
+    def update(self, dt):
+        self.t += dt
+        if self.t < 0:
+            return (self.pos, self.vel)
+        if self.t < self.t_acc:
+            return (
+                self.pos + self.vel * self.t + 0.5 * self.acc * self.t * self.t,
+                self.vel + self.acc * self.t
+            )
+        if self.t < self.t_acc + self.t_vel:
+            return (
+                self.pos + self.vel*self.t_acc + 0.5*self.acc*self.t_acc*self.t_acc + self.top_vel*(self.t - self.t_acc),
+                self.top_vel
+            )
+        if self.t < self.t_acc + self.t_vel + self.t_dec:
+            td = self.t - (self.t_acc + self.t_vel + self.t_dec)
+            return (
+                self.target + 0.5 * self.dec * td * td,
+                self.dec * td
+            )
+        else:
+            return (self.target, self.max_vel)
+
+class MotorPositionFilterController(object):
+    def __init__(self, bandwidth):
+        self.bandwidth = bandwidth
+        self.target = 0
+    
+    def set_pos(self, target_pos):
+        self.target = target_pos
+    
+    def update(self, dt, pos, vel):
+        bandwidth = min(self.bandwidth, 0.25 / dt)
+        input_filter_ki = 2.0 * bandwidth
+        input_filter_kp = 0.25 * (input_filter_ki * input_filter_ki)
+        delta_pos = self.target - pos
+        delta_vel = -vel
+        accel = input_filter_kp * delta_pos + input_filter_ki * delta_vel
+        new_vel = vel + dt * accel
+        new_pos = pos + dt * new_vel
+        return (new_pos, new_vel)
+
+class Motor(WebotsDevice):
+    """Robodyno Motor
+    
+    Attributes:
+        id: correspond with motor id in real world or simulation.
+        type: motor type enum
+        reduction: motor reduction
+        available_velocity: theoretical max velocity(rad/s)
+        available_torque: theoretical max torque(Nm)
+        available_current: theoretical max phase current(A)
+        torque_constant: theoretical torque provided by unit current(Nm/A)
+        with_brake: is motor has a brake(bool)
+        state: motor state
+        mode: motor mode
+    """
+
+    class MotorState(Enum):
+        UNKNOWN = -1
+        DISABLED = 1
+        CALIBRATE = 3
+        MOTOR_CALIBRATING = 4
+        OFFSET_CALIBRATING = 7
+        ENABLED = 8
+
+    class MotorControlMode(Enum):
+        UNKNOWN = -1
+        POSITION_MODE = 0
+        POSITION_FILTER_MODE = 1
+        POSITION_TRACK_MODE = 2
+        VELOCITY_MODE = 3
+        VELOCITY_RAMP_MODE = 4
+        TORQUE_MODE = 5
+        TWIN_MODE = 255
+    
+    def __init__(self, iface, id = 0x10, type = None, twin = None):
+        """Init motor from interface, id and type.
+        
+        Args:
+            iface: robodyno interface object
+            id: range from 0x01 to 0x40 or motor name in webots
+            type: Motor type string
+        """
+        iface._mutex.acquire()
+        super().__init__(iface, id, auto_register=False)
+        valid_motor_types = [
+            DeviceType.ROBODYNO_PRO_44,
+            DeviceType.ROBODYNO_PRO_12,
+            DeviceType.ROBODYNO_PRO_50 ,
+            DeviceType.ROBODYNO_PRO_100,
+            DeviceType.ROBODYNO_PRO_DIRECT,
+            DeviceType.ROBODYNO_PLUS_50 ,
+            DeviceType.ROBODYNO_PLUS_100,
+            DeviceType.ROBODYNO_PLUS_12 ,
+            DeviceType.ROBODYNO_PLUS_DIRECT,
+            DeviceType.ROBODYNO_NANO_100,
+        ]
+        try:
+            self.name = '0x{:02X}::motor'.format(id)
+        except:
+            self.name = id
+        self._motor = self._iface.robot.getDevice(self.name)
+        self._pos_sensor = self._motor.getPositionSensor()
+        self._twin_motor = None
+        if twin and GET_IFACE_TYPE(twin) == InterfaceType.CanBus:
+            self._twin_motor = CanMotor(twin, id, type)
+            self.init_twin_offset()
+            self.type = self._twin_motor.type
+        elif type:
+            self.type = DeviceType[type]
+        else:
+            self.type = DeviceType[self._pos_sensor.getName()]
+        if self.type not in valid_motor_types:
+            raise ValueError('Motor type is invalid')
+        self.mode = self.MotorControlMode.UNKNOWN
+        self.__dict__.update(ROBODYNO_MOTOR_SPECS.get(self.type, None))
+        self.state = self.MotorState.DISABLED
+        self._rot_factor = self.reduction / 2.0 / pi
+
+        self._motor.enableTorqueFeedback(int(self._iface.time_step))
+        self._pos_sensor.enable(int(self._iface.time_step))
+
+        self._track_controller = MotorPositionTrackController(
+            fabs(4 * 2 * pi / self.reduction),
+            fabs(10 * 2 * pi / self.reduction),
+            fabs(10 * 2 * pi / self.reduction)
+        )
+        self._filter_controller = MotorPositionFilterController(10)
+
+        self._input_pos = 0
+        self._input_vel = 0
+        self._input_torque = 0
+        self._max_vel = self.available_velocity
+        self._pos_feedback = 0
+        self._vel_feedback = 0
+        self._torque_feedback = 0
+        self._prev_pos_feedback = 0
+        self._prev_update_time = self._iface.time()
+        self._iface.register(self)
+        iface._mutex.release()
+        if self._twin_motor:
+            self.twin_mode()
+        else:
+            self.position_mode()
+
+    def init_twin_offset(self):
+        """Read twin motor position set set it as an offset.
+
+        Returns:
+            True if success else False.
+        """
+        self._twin_offset = 0
+        if self._twin_motor:
+            if self._twin_motor.fw_ver >= 1:
+                abs_pos = self._twin_motor.get_abs_pos(0.5)
+                if abs_pos:
+                    self._twin_offset = abs_pos
+                    return True
+                else:
+                    return False
+            else:
+                pos = self._twin_motor.get_pos(0.5)
+                if pos:
+                    self._twin_offset = pos
+                    return True
+                else:
+                    return False
+
+    def parallel_update(self):
+        """Update parallel with simulation step."""
+        if self.mode == self.MotorControlMode.TWIN_MODE:
+            feedback = self._twin_motor.get_feedback(0.1)
+            if feedback is not None:
+                self._pos_feedback, self._vel_feedback, self._torque_feedback = feedback
+                self._pos_feedback -= self._twin_offset
+            if self._twin_motor.fw_ver >= 1:
+                abs_pos = self._twin_motor.get_abs_pos(0.1)
+                if abs_pos:
+                    self._pos_feedback = abs_pos - self._twin_offset
+
+    def update(self):
+        """Simulation update callback."""
+        if self.mode == self.MotorControlMode.TWIN_MODE:
+            self._motor.setPosition(self._pos_feedback)
+            return
+
+        t = self._iface.time()
+        dt = t - self._prev_update_time
+        self._prev_update_time = t
+        if dt == 0:
+            return
+        self._pos_feedback = self._pos_sensor.getValue()
+        self._vel_feedback = (self._pos_feedback - self._prev_pos_feedback) / dt
+        self._prev_pos_feedback = self._pos_feedback
+        self._torque_feedback = self._motor.getTorqueFeedback()
+        if self.state == self.MotorState.DISABLED:
+            self._motor.setTorque(0)
+        elif self.state == self.MotorState.ENABLED:
+            if self.mode == self.MotorControlMode.TORQUE_MODE:
+                self._motor.setTorque(self._input_torque)
+            elif self.mode == self.MotorControlMode.VELOCITY_MODE or self.mode == self.MotorControlMode.VELOCITY_RAMP_MODE:
+                self._motor.setVelocity(self._input_vel)
+            elif self.mode == self.MotorControlMode.POSITION_MODE:
+                self._motor.setPosition(self._input_pos)
+            elif self.mode == self.MotorControlMode.POSITION_FILTER_MODE:
+                p, v = self._filter_controller.update(dt, self._pos_feedback, self._vel_feedback)
+                self._motor.setPosition(p)
+                self._motor.setVelocity(fabs(v))
+            elif self.mode == self.MotorControlMode.POSITION_TRACK_MODE:
+                p, v = self._track_controller.update(dt)
+                self._motor.setPosition(p)
+                self._motor.setVelocity(fabs(v))
+
+    def enable(self):
+        """Enable motor. Set motor state to CLOSED_LOOP."""
+        self._iface._mutex.acquire()
+        self.state = self.MotorState.ENABLED
+        self._iface._mutex.release()
+    
+    def disable(self):
+        """Disable motor. Set motor state to IDLE."""
+        self._iface._mutex.acquire()
+        self.state = self.MotorState.DISABLED
+        self._iface._mutex.release()
+
+    def get_pos(self, timeout = 0):
+        """Get motor position.
+        
+        Args:
+            timeout: 0 indicates unlimited timeout(s)
+        
+        Returns:
+            position(rad)
+            None if timeout
+        """
+        return self._pos_feedback 
+
+    def get_abs_pos(self, timeout = 0):
+        """Get motor absolute position.
+        
+        Args:
+            timeout: 0 indicates unlimited timeout(s)
+        
+        Returns:
+            position(rad)
+            None if timeout
+        """
+        return self._pos_feedback 
+
+
+    def get_vel(self, timeout = 0):
+        """Get motor velocity.
+        
+        Args:
+            timeout: 0 indicates unlimited timeout(s)
+        
+        Returns:
+            velocity(rad/s)
+            None if timeout
+        """
+        return self._vel_feedback 
+
+    def get_torque(self, timeout = 0):
+        """Get motor torque.
+        
+        Args:
+            timeout: 0 indicates unlimited timeout(s)
+        
+        Returns:
+            torque(Nm)
+            None if timeout
+        """
+        return self._torque_feedback 
+
+    def get_mode(self, payload):
+        """Get motor control mode and params.
+        
+        Args:
+            timeout: 0 indicates unlimited timeout(s)
+        
+        Returns:
+            control mode(MotorControlMode), control params dict
+            None if timeout
+        """
+        ret = None
+        if self.mode == self.MotorControlMode.POSITION_FILTER_MODE:
+            ret = (self.mode, {'bandwidth': self._filter_controller.bandwidth})
+        elif self.mode == self.MotorControlMode.POSITION_TRACK_MODE:
+            ret = (self.mode, {
+                'vel': fabs(self._track_controller.max_vel / self._rot_factor),
+                'acc': fabs(self._track_controller.max_acc / self._rot_factor),
+                'dec': fabs(self._track_controller.max_dec / self._rot_factor),
+            })
+        elif self.mode == self.MotorControlMode.VELOCITY_RAMP_MODE:
+            ret = (self.mode, {'ramp': self._motor.getAcceleration()})
+        else:
+            ret = (self.mode, )
+        return ret
+    
+    def twin_mode(self):
+        self._iface._mutex.acquire()
+        self._motor.setPosition(self._pos_feedback)
+        self._motor.setVelocity(self._max_vel)
+        self._motor.setAcceleration(-1)
+        self.mode = self.MotorControlMode.TWIN_MODE
+        self.state = self.MotorState.ENABLED
+        self._iface._mutex.release()
+
+    def position_mode(self):
+        """Enter position pid mode."""
+        self._iface._mutex.acquire()
+        self._motor.setPosition(self._pos_feedback)
+        self._motor.setVelocity(self._max_vel)
+        self._motor.setAcceleration(-1)
+        self.mode = self.MotorControlMode.POSITION_MODE
+        self._iface._mutex.release()
+
+    def position_filter_mode(self, bandwidth):
+        """Enter position filter mode.
+        
+        Args:
+            bandwidth: filter bandwith, equals to control frequency(Hz)
+        """
+        self._iface._mutex.acquire()
+        self._filter_controller = MotorPositionFilterController(bandwidth)
+        self._filter_controller.set_pos(self._pos_feedback)
+        self._motor.setAcceleration(-1)
+        self.mode = self.MotorControlMode.POSITION_FILTER_MODE
+        self._iface._mutex.release()
+
+    def position_track_mode(self, vel, acc, dec):
+        """Enter position track mode.
+        
+        Args:
+            vel: motion max vel(rad/s)
+            acc: motion acceleration(rad/s^2)
+            dec: motion deceleration(rad/s^2)
+        """
+        self._iface._mutex.acquire()
+        self._track_controller = MotorPositionTrackController(vel, acc, dec)
+        self._track_controller.set_pos(self._pos_feedback, self._pos_feedback, self._vel_feedback)
+        self._motor.setAcceleration(-1)
+        self.mode = self.MotorControlMode.POSITION_TRACK_MODE
+        self._iface._mutex.release()
+    
+    def velocity_mode(self):
+        """Enter velocity mode."""
+        self._iface._mutex.acquire()
+        self._motor.setPosition(float('+inf'))
+        self._motor.setVelocity(self._input_vel)
+        self._motor.setAcceleration(-1)
+        self.mode = self.MotorControlMode.VELOCITY_MODE
+        self._iface._mutex.release()
+
+    def velocity_ramp_mode(self, ramp):
+        """Enter velocity ramp mode.
+        
+        Args:
+            ramp: motion acceleration(rad/s^2)
+        """
+        self._iface._mutex.acquire()
+        self._motor.setPosition(float('+inf'))
+        self._motor.setVelocity(self._input_vel)
+        self._motor.setAcceleration(ramp)
+        self.mode = self.MotorControlMode.VELOCITY_RAMP_MODE
+        self._iface._mutex.release()
+
+    def torque_mode(self):
+        """Enter torque mode"""
+        self._iface._mutex.acquire()
+        self._motor.setTorque(self._input_torque)
+        self.mode = self.MotorControlMode.TORQUE_MODE
+        self._iface._mutex.release()
+    
+    def get_vel_limit(self, vel_limit, current_limit):
+        """Get motor volocity limit.
+        
+        Args:
+            timeout: 0 indicates unlimited timeout(s)
+        
+        Returns:
+            velocity limit(rad/s)
+            None if timeout
+        """
+        return self._max_vel
+    
+    def get_current_limit(self, vel_limit, current_limit):
+        """Get motor current limit.
+        
+        Args:
+            timeout: 0 indicates unlimited timeout(s)
+        
+        Returns:
+            current limit(A)
+            None if timeout
+        """
+        return self._motor.getAvailableTorque() / self.torque_constant
+    
+    def set_vel_limit(self, vel_lim):
+        """Set motor velocity limit.
+        
+        Args:
+            vel_lim: velocity limit(rad/s)
+        """
+        self._iface._mutex.acquire()
+        if (fabs(vel_lim) > self.available_velocity):
+            raise ValueError('Velocity limit exceeded available value.')
+        self._max_vel = fabs(vel_lim)
+        if self.mode in [self.MotorControlMode.POSITION_MODE, self.MotorControlMode.POSITION_FILTER_MODE, self.MotorControlMode.POSITION_TRACK_MODE]:
+            self._motor.setVelocity(fabs(vel_lim))
+        self._iface._mutex.release()
+    
+    def set_current_limit(self, current_lim):
+        """Set motor current limit.
+        
+        Args:
+            current_lim: current limit(A)
+        """
+        self._iface._mutex.acquire()
+        if fabs(current_lim) * self.torque_constant > self.available_current:
+            raise ValueError('Current limit exceed available value.')
+        self._motor.setAvailableTorque(fabs(current_lim) * self.torque_constant)
+        self._iface._mutex.release()
+
+    def set_pos(self, pos, vel_ff = 0, torque_ff = 0):
+        """Set motor target position.
+        
+        Args:
+            pos: target position(rad)
+            vel_ff: velocity feed forward(rad/s)
+            torque_ff:torque feed forward(Nm)
+        """
+        self._iface._mutex.acquire()
+        pos = pos 
+        self._input_pos = pos
+        self._filter_controller.set_pos(pos)
+        self._track_controller.set_pos(pos, self._pos_feedback, self._vel_feedback)
+        self._iface._mutex.release()
+    
+    def set_abs_pos(self, pos, vel_ff = 0, torque_ff = 0):
+        """Set motor target absolute position.
+        
+        Args:
+            pos: target position(rad)
+            vel_ff: velocity feed forward(rad/s)
+            torque_ff:torque feed forward(Nm)
+        """
+        self._iface._mutex.acquire()
+        pos = pos 
+        self._input_pos = pos
+        self._filter_controller.set_pos(pos)
+        self._track_controller.set_pos(pos, self._pos_feedback, self._vel_feedback)
+        self._iface._mutex.release()
+    
+    def set_vel(self, vel, torque_ff = 0):
+        """Set motor velocity.
+        
+        Args:
+            vel: target velocity(rad)
+            torque_ff: torque feed forward(Nm)
+        """
+        self._iface._mutex.acquire()
+        vel = vel 
+        self._input_vel = vel
+        self._iface._mutex.release()
+    
+    def set_torque(self, torque):
+        """Set motor torque.
+        
+        Args:
+            torque: target torque(Nm)
+        """
+        self._iface._mutex.acquire()
+        torque = torque 
+        self._input_torque = torque
+        self._iface._mutex.release()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `robodyno-1.6.0/src/robodyno/components/can_bus/slider_module.py` & `robodyno-1.6.1b0/src/robodyno/components/webots/slider_module.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,125 +1,110 @@
-#!/usr/bin/env python
-# -*-coding:utf-8 -*-
-"""slider_module.py
-Time    :   2023/01/30
-Author  :   song 
-Version :   1.0
-Contact :   zhaosongy@126.com
-License :   (C)Copyright 2022, robottime / robodyno
-
-Robodyno slider module can bus driver
-
-  Typical usage example:
-
-  from robodyno.interfaces import CanBus
-  from robodyno.components import SliderModule
-
-  can = CanBus()
-  
-  slider = SliderModule(can, id = 0x10, type = 'ROBODYNO_PRO_44', max_vel = 0.02)
-
-  can.disconnect()
-"""
-
-import time
-from math import fabs, pi
-from robodyno.components.can_bus.motor import Motor
-
-class SliderModule():
-    """Robodyno slider module driver.
-    
-    Attributes:
-        motor: robodyno motor integrated in module
-        max_vel: slider's max velocity (m/s)
-        LEAD: linear travel the nut makes per one screw revolution (m)
-    """
-
-    def __init__(self, iface, id = 0x10, type = None, max_vel = 0.02, *args, **kwargs):
-        """Init slider module from interface, motor id, motor type, slider's max vel
-        
-        Args:
-            iface: robodyno interface
-            id: robodyno motor id
-            type: robodyno motor type
-            max_vel: slider
-        """
-        self.LEAD = 0.01
-        self.motor = Motor(iface, id, type)
-        self._reduction = self.LEAD / 2 / pi # mm/rad
-        self.set_max_vel(max_vel)
-    
-    def set_max_vel(self, max_vel):
-        """Change slider's max velocity.
-        
-        Args:
-            max_vel: slider's max velocity, should be always positive (m/s)
-        """
-        self.max_vel = fabs(max_vel)
-        self.motor.position_track_mode(self.max_vel / self._reduction, 40, 40)
-    
-    def enable(self):
-        """Enable slider module."""
-        self.motor.enable()
-
-    def disable(self):
-        """Disable slider module."""
-        self.motor.disable()
-
-    def set_pos(self, pos):
-        """Set slider's position.
-        
-        Args:
-            pos: slider's position (m)
-        """
-        self.motor.set_pos(pos / self._reduction)
-        
-    def set_abs_pos(self, pos):
-        """Set slider's absolute position.
-        
-        Args:
-            pos: slider's absolute position (m)
-        """
-        self.motor.set_abs_pos(pos / self._reduction)
-
-    def get_pos(self, timeout = 0):
-        """Read slider's position.
-        
-        Args:
-            timeout: 0 indicates unlimited timeout (s)
-        
-        Returns:
-            position (m) / None if timeout
-        """
-        pos = self.motor.get_pos(timeout)
-        return None if pos is None else pos * self._reduction
-
-    def get_abs_pos(self, timeout = 0):
-        """Read slider's absolute position.
-        
-        Args:
-            timeout: 0 indicates unlimited timeout (s)
-        
-        Returns:
-            absolute position (m) / None if timeout
-        """
-        pos = self.motor.get_abs_pos(timeout)
-        return None if pos is None else pos * self._reduction
-
-    def init_pos(self, offset = 0):
-        """Init slider pos with current position
-        
-        Args:
-            offset: current position (m)
-        """
-        self.motor.init_pos(offset / self._reduction)
-
-    def init_abs_pos(self, offset = 0, save = True):
-        """Init slider absolute pos with current position
-        
-        Args:
-            offset: current absolute position (m)
-        """
-        self.motor.init_abs_pos(offset / self._reduction)
-        if save:
-            self.motor.save_configuration()
-            time.sleep(0.1)
+#!/usr/bin/env python
+# -*-coding:utf-8 -*-
+"""slider_module.py
+Time    :   2023/04/02
+Author  :   song 
+Version :   1.0
+Contact :   zhaosongy@126.com
+License :   (C)Copyright 2022, robottime / robodyno
+
+Robodyno slider module can bus driver
+
+  Typical usage example:
+
+  from robodyno.interfaces import Webots
+  from robodyno.components import SliderModule
+
+  webots = Webots()
+  
+  slider = SliderModule(webots, id = 0x10, max_vel = 0.02)
+"""
+
+import time
+from math import fabs, pi
+from robodyno.components.webots.motor import Motor
+
+class SliderModule():
+    """Robodyno slider module driver.
+    
+    Attributes:
+        motor: robodyno motor integrated in module
+        max_vel: slider's max velocity (m/s)
+        LEAD: linear travel the nut makes per one screw revolution (m)
+    """
+
+    def __init__(self, iface, id = 0x10, type = None, max_vel = 0.02, twin = None, *args, **kwargs):
+        """Init slider module from interface, motor id, motor type, slider's max vel
+        
+        Args:
+            iface: robodyno interface
+            id: robodyno motor id
+            type: robodyno motor type
+            max_vel: slider
+        """
+        self.LEAD = 0.01
+        self.motor = Motor(iface, id, type, twin)
+        self._reduction = self.LEAD / 2 / pi # mm/rad
+        if self.motor.mode != self.motor.MotorControlMode.TWIN_MODE:
+            self.set_max_vel(max_vel)
+    
+    def set_max_vel(self, max_vel):
+        """Change slider's max velocity.
+        
+        Args:
+            max_vel: slider's max velocity, should be always positive (m/s)
+        """
+        self.max_vel = fabs(max_vel)
+        if self.motor.mode != self.motor.MotorControlMode.TWIN_MODE:
+            self.motor.position_track_mode(self.max_vel / self._reduction, 40, 40)
+    
+    def enable(self):
+        """Enable slider module."""
+        if self.motor.mode != self.motor.MotorControlMode.TWIN_MODE:
+            self.motor.enable()
+
+    def disable(self):
+        """Disable slider module."""
+        if self.motor.mode != self.motor.MotorControlMode.TWIN_MODE:
+            self.motor.disable()
+
+    def set_pos(self, pos):
+        """Set slider's position.
+        
+        Args:
+            pos: slider's position (m)
+        """
+        if self.motor.mode != self.motor.MotorControlMode.TWIN_MODE:
+            self.motor.set_pos(pos / self._reduction)
+        
+    def set_abs_pos(self, pos):
+        """Set slider's absolute position.
+        
+        Args:
+            pos: slider's absolute position (m)
+        """
+        if self.motor.mode != self.motor.MotorControlMode.TWIN_MODE:
+            self.motor.set_abs_pos(pos / self._reduction)
+
+    def get_pos(self, timeout = 0):
+        """Read slider's position.
+        
+        Args:
+            timeout: 0 indicates unlimited timeout (s)
+        
+        Returns:
+            position (m) / None if timeout
+        """
+        pos = self.motor.get_pos(timeout)
+        return None if pos is None else pos * self._reduction
+
+    def get_abs_pos(self, timeout = 0):
+        """Read slider's absolute position.
+        
+        Args:
+            timeout: 0 indicates unlimited timeout (s)
+        
+        Returns:
+            absolute position (m) / None if timeout
+        """
+        pos = self.motor.get_abs_pos(timeout)
+        return None if pos is None else pos * self._reduction
```

### Comparing `robodyno-1.6.0/src/robodyno/components/webots/webots_device.py` & `robodyno-1.6.1b0/src/robodyno/components/webots/webots_device.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-#!/usr/bin/env python
-# -*-coding:utf-8 -*-
-"""webots_device.py
-Time    :   2023/01/05
-Author  :   song 
-Version :   1.0
-Contact :   zhaosongy@126.com
-License :   (C)Copyright 2022, robottime / robodyno
-
-Webots device node base class.
-"""
-
-from enum import Enum
-from robodyno.interfaces import Webots
-
-class WebotsDevice(object):
-    """Webots common device node."""
-    
-    def __init__(self, iface, id = 0x10, auto_register = True):
-        """Init node with webots interface and id.
-        
-        Args:
-            iface: webots interface
-            id: node id
-            type: robodyno device type name
-            auto_register: auto register self to webots interface
-        """
-        self.id = id
-        if not isinstance(iface, Webots):
-            raise ValueError('Use a webots interface to init a webots device.')
-        self._iface = iface
-        if auto_register:
-            iface.register(self)
-    
-    def __del__(self):
-        """Collect node from memory."""
-        self._iface.deregister(self)
-    
-    def get_version(self):
-        """Get device simulation version.
-        
-        Returns:
-            dictionary of device version
-        """
-        return {
-            'main_version': 4,
-            'sub_version': 0,
-            'type': self.type
-        }
-    
-    def parallel_update(self):
-        """Update parallel with simulation step."""
-        pass
-
-    def update(self):
-        """after simulation step update callback."""
+#!/usr/bin/env python
+# -*-coding:utf-8 -*-
+"""webots_device.py
+Time    :   2023/01/05
+Author  :   song 
+Version :   1.0
+Contact :   zhaosongy@126.com
+License :   (C)Copyright 2022, robottime / robodyno
+
+Webots device node base class.
+"""
+
+from enum import Enum
+from robodyno.interfaces import Webots
+
+class WebotsDevice(object):
+    """Webots common device node."""
+    
+    def __init__(self, iface, id = 0x10, auto_register = True):
+        """Init node with webots interface and id.
+        
+        Args:
+            iface: webots interface
+            id: node id
+            type: robodyno device type name
+            auto_register: auto register self to webots interface
+        """
+        self.id = id
+        if not isinstance(iface, Webots):
+            raise ValueError('Use a webots interface to init a webots device.')
+        self._iface = iface
+        if auto_register:
+            iface.register(self)
+    
+    def __del__(self):
+        """Collect node from memory."""
+        self._iface.deregister(self)
+    
+    def get_version(self):
+        """Get device simulation version.
+        
+        Returns:
+            dictionary of device version
+        """
+        return {
+            'main_version': 4,
+            'sub_version': 0,
+            'type': self.type
+        }
+    
+    def parallel_update(self):
+        """Update parallel with simulation step."""
+        pass
+
+    def update(self):
+        """after simulation step update callback."""
         pass
```

### Comparing `robodyno-1.6.0/src/robodyno/interfaces/webots.py` & `robodyno-1.6.1b0/src/robodyno/interfaces/webots.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-#!/usr/bin/env python
-# -*-coding:utf-8 -*-
-"""webots.py
-Time    :   2023/01/05
-Author  :   song 
-Version :   1.0
-Contact :   zhaosongy@126.com
-License :   (C)Copyright 2022, robottime / robodyno
-
-Robodyno webots interface
-
-  Typical usage example:
-
-  webots = Webots(time_step = 0)
-"""
-
-import threading
-from threading import Lock
-import time
-
-try:
-    from controller import Robot
-except:
-    raise RuntimeError('Only work with Webots environment.')
-
-class Webots(object):
-    """Webots interface holds global robot instance, update nodes automaticly.
-    
-    Attributes:
-        robot: Webots robot instance
-        time_step: Webots simulate timestep
-    """
-    
-    def __init__(self, time_step = 0, step_callback = None):
-        """Init Webots interface.
-        
-        Args:
-            time_step: time step to update simulation
-                       set it to 0 to use value of the basicTimeStep field of the WorldInfo node
-            step_callback: called after each simulation step
-        """
-        self.robot = Robot()
-        if time_step == 0:
-            self.time_step = self.robot.getBasicTimeStep()
-        else:
-            self.time_step = time_step
-
-        self._nodes = []
-        
-        self._step_cb = step_callback
-        
-        self._wb_thread = threading.Thread(
-            target = self._wb_thread_callback,
-            name = 'webots.step',
-            daemon= True
-        )
-        self._mutex = Lock()
-        self.robot.step(int(self.time_step))
-        self._wb_thread.start()
-    
-    def time(self):
-        """Get time in simulation world.
-        
-        Returns:
-            current time in seconds
-        """
-        return self.robot.getTime()
-
-    def sleep(self, seconds):
-        """Time sleep.
-        
-        Args:
-            seconds: sleep duration in seconds
-        """
-        s = self.time()
-        while self.time() - s < seconds:
-            pass
-
-    def register(self, node):
-        """Simulation will update all nodes registered to interface.
-        
-        Args:
-            node: node with update function
-        """
-        self._nodes.append(node)
-    
-    def deregister(self, node):
-        """Deregister a registered node.
-        
-        Args:
-            node: node registered
-        """
-        self._nodes.remove(node)
-    
-    def _wb_thread_callback(self):
-        """Step webots simulation thread callback"""
-        while(True):
-            self._mutex.acquire()
-            if self.robot.stepBegin(int(self.time_step)) == -1:
-                self._mutex.release()
-                break
-            for node in self._nodes:
-                node.parallel_update()
-            if self.robot.stepEnd() == -1:
-                self._mutex.release()
-                break
-            for node in self._nodes:
-                node.update()
-            self._mutex.release()
-            if self._step_cb:
-                self._step_cb()
-            time.sleep(0.001)
+#!/usr/bin/env python
+# -*-coding:utf-8 -*-
+"""webots.py
+Time    :   2023/01/05
+Author  :   song 
+Version :   1.0
+Contact :   zhaosongy@126.com
+License :   (C)Copyright 2022, robottime / robodyno
+
+Robodyno webots interface
+
+  Typical usage example:
+
+  webots = Webots(time_step = 0)
+"""
+
+import threading
+from threading import Lock
+import time
+
+try:
+    from controller import Robot
+except:
+    raise RuntimeError('Only work with Webots environment.')
+
+class Webots(object):
+    """Webots interface holds global robot instance, update nodes automaticly.
+    
+    Attributes:
+        robot: Webots robot instance
+        time_step: Webots simulate timestep
+    """
+    
+    def __init__(self, time_step = 0, step_callback = None):
+        """Init Webots interface.
+        
+        Args:
+            time_step: time step to update simulation
+                       set it to 0 to use value of the basicTimeStep field of the WorldInfo node
+            step_callback: called after each simulation step
+        """
+        self.robot = Robot()
+        if time_step == 0:
+            self.time_step = self.robot.getBasicTimeStep()
+        else:
+            self.time_step = time_step
+
+        self._nodes = []
+        
+        self._step_cb = step_callback
+        
+        self._wb_thread = threading.Thread(
+            target = self._wb_thread_callback,
+            name = 'webots.step',
+            daemon= True
+        )
+        self._mutex = Lock()
+        self.robot.step(int(self.time_step))
+        self._wb_thread.start()
+    
+    def time(self):
+        """Get time in simulation world.
+        
+        Returns:
+            current time in seconds
+        """
+        return self.robot.getTime()
+
+    def sleep(self, seconds):
+        """Time sleep.
+        
+        Args:
+            seconds: sleep duration in seconds
+        """
+        s = self.time()
+        while self.time() - s < seconds:
+            pass
+
+    def register(self, node):
+        """Simulation will update all nodes registered to interface.
+        
+        Args:
+            node: node with update function
+        """
+        self._nodes.append(node)
+    
+    def deregister(self, node):
+        """Deregister a registered node.
+        
+        Args:
+            node: node registered
+        """
+        self._nodes.remove(node)
+    
+    def _wb_thread_callback(self):
+        """Step webots simulation thread callback"""
+        while(True):
+            self._mutex.acquire()
+            if self.robot.stepBegin(int(self.time_step)) == -1:
+                self._mutex.release()
+                break
+            for node in self._nodes:
+                node.parallel_update()
+            if self.robot.stepEnd() == -1:
+                self._mutex.release()
+                break
+            for node in self._nodes:
+                node.update()
+            self._mutex.release()
+            if self._step_cb:
+                self._step_cb()
+            time.sleep(0.001)
```

### Comparing `robodyno-1.6.0/src/robodyno/robots/four_dof_palletizing_robot/four_dof_pallet_robot.py` & `robodyno-1.6.1b0/src/robodyno/robots/four_dof_palletizing_robot/four_dof_pallet_robot.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,232 +1,232 @@
-#!/usr/bin/env python
-# -*-coding:utf-8 -*-
-"""four_dof_pallet_robot.py
-Time    :   2022/10/17
-Author  :   ryan 
-Version :   1.0
-Contact :   ryanzhang@163.com
-License :   (C)Copyright 2022, robottime / robodyno
-
-4DoF Pallet Robot Drive
-
-  Typical usage example:
-
-  from robodyno.robots.four_dof_pallet_robot import FourDoFPallet
-  robot = FourDoFPallet(
-    j1 = base_motor,
-    j2 = upperarm_motor,
-    j3 = forearm_motor,
-    j4 = hand_motor,
-    l01 = 0.0794,
-    l23 = 0.190,
-    l34 = 0.190,
-    l45 = 0.010,
-    end_effector = None
-  )
-"""
-import time
-from math import pi, cos, sin, sqrt, atan2, acos
-from ..utils.interpolations import linear_interpolation
-
-class FourDoFPallet(object):
-    """4 DoF pallet robot driver
-    
-    Attributes:
-        joints: list of 4 joint motors
-        l01: link from world to joint 1 (m)
-        l23: link from joint 2 to joint 3 transverse distance (m)
-        l34: link from joint 3 to joint 4 longitudinal distance (m)
-        l45: link from joint 4 to joint 5 transverse distance (m)
-        end_effector: end effector object
-    """
-    def __init__(self, j1, j2, j3, j4, l01, l23, l34, l45, end_effector = None):
-        self.joints = [j1, j2, j3, j4]
-        self.l01 = l01
-        self.l23 = l23
-        self.l34 = l34
-        self.l45 = l45
-        self.end_effector = end_effector
-
-        for m in self.joints:
-          m.position_filter_mode(8)
-        self._axes_poses = [0 for i in range(4)]
-        self._axes_zeros = [0 for i in range(4)]
-
-    def get_joints_pose(self):
-        """Read joints position to a list.
-        
-        Returns:
-            a list of 4 joint positions
-        """
-        poses = []
-        for i in range(4):
-            pos = None
-            count = 0
-            while not pos:
-                if count > 5:
-                    raise RuntimeError('Filed to get position of Joint {}'.format(i+1))
-                count += 1
-                pos = self.joints[i].get_pos(0.2)
-            poses.append(pos - self._axes_zeros[i])
-        return poses
-
-    def enable(self):
-        """enable joints motors"""
-        for i in range(4):
-            self.joints[i].enable()
-
-    def disable(self):
-        """disable joints motors"""
-        for i in range(4):
-            self.joints[i].disable()
-
-    def init (self, axes_poses = [0 for i in range(4)]):
-        """Calibrate robot motors with given axes poses.
-        
-        Args:
-            axes_poses: list of 4 axes poses(rad)
-        """
-        self._axes_poses = axes_poses.copy()
-        self._axes_zeros = [0 for i in range(4)]
-        cur_poses = self.get_joints_pose()
-        for i in range(4):
-            self._axes_zeros[i] = cur_poses[i] - self._axes_poses[i]
-            self._axes_poses[i] = 0
-
-    def set_joint_pos(self, id, pos):
-        """Set joint angle with joint and position.
-        
-        Args:
-            id: joint id (0-3)
-            pos: joint target position(red)
-        """
-        self.joints[id].set_pos(pos + self._axes_zeros[id])
-        self._axes_poses[id] = pos        
-        
-    def joint_space_interpolated_motion(self, target, speeds = [0 for i in range(4)], duration = 0):
-        """Robot interpolated motion in joint space.
-        
-        Args:
-            target: iterable of 4 joints target angle(rad)
-            speeds: iterable of 4 joints motion speed(rad/s)
-            duration: default motion duration(s)
-        """
-        interpolation = []
-        joint_poses = self._axes_poses.copy()
-        for i in range(4):
-            interpolation.append(linear_interpolation(joint_poses[i], target[i], speed=speeds[i], duration=duration))
-        update_flag = True
-        while update_flag:
-            update_flag = False
-            for i in range(4):
-                pos = next(interpolation[i], None)
-                if pos is not None:
-                    self.set_joint_pos(i, pos)
-                    update_flag = True
-            time.sleep(0.05)
-
-    def home(self, duration = 5):
-        """Move back to zero position.
-        
-        Args:
-            duration: motion duration(s)
-        """
-        self.joint_space_interpolated_motion((0,0,0,0), duration = duration)
-
-    def cartesian_space_interpolated_motion(self, x, y, z, yaw, x_speed = None, y_speed = None, z_speed = None, yaw_speed = None, duration = 0):
-        """Robot Interpolated motion in cartesian space.
-        
-        Args:
-            x: target robot end x
-            y: target robot end y
-            z: target robot end z
-            yaw: target robot end yaw
-            x_speed: speed alone X dimension(m/s)
-            y_speed: speed alone Y dimension(m/s)
-            z_speed: speed alone Z dimension(m/s)
-            yaw_speed: rotation speed on Z axis(rad/s)
-            duration: default motion duration(s)
-        """
-        current_pose = self.forward_kinematics(self._axes_poses.copy())
-        current_x = current_pose[0]
-        current_y = current_pose[1]
-        current_z = current_pose[2]
-        current_yaw = current_pose[3]
-
-        x_interpolation = linear_interpolation(current_x, x, x_speed, duration)
-        y_interpolation = linear_interpolation(current_y, y, y_speed, duration)
-        z_interpolation = linear_interpolation(current_z, z, z_speed, duration)
-        yaw_interpolation = linear_interpolation(current_yaw, yaw, yaw_speed, duration)
-        
-        while True:
-            temp_x = next(x_interpolation, x)
-            temp_y = next(y_interpolation, y)
-            temp_z = next(z_interpolation, z)
-            temp_yaw = next(yaw_interpolation, yaw)
-
-            axes = self.inverse_kinematics(temp_x, temp_y, temp_z, temp_yaw)
-            for i in range(4):
-                self.set_joint_pos(i, axes[i])
-            if temp_x == x and temp_y == y and temp_z == z and temp_yaw == yaw:
-                break
-            time.sleep(0.05)
-
-    def forward_kinematics(self, angles):
-        """Forward kinematics algorism
-        
-        Args:
-            angles: list of 4 joint angles(rad)
-        
-        Returns:
-            (x, y, z, yaw): tuples of 3 axis position and 1 axis posture
-        """
-        a_2 = self.l23 * self.l23 + self.l34 * self.l34 - 2 * self.l23 * self.l34 * cos(pi/2 + angles[2])
-        a = sqrt(a_2)
-        cos_alpha = (self.l23 * self.l23 + a_2 - self.l34 * self.l34) / (2 * a * self.l23)
-        alpha = acos(cos_alpha)
-        
-        b = a * sin(alpha + angles[1])
-        
-        x = b * cos(angles[0])
-        y = b * sin(angles[0])
-        z = a * cos(alpha + angles[1]) + self.l01 - self.l45
-        yaw = -angles[0] + angles[3]
-
-        return (x, y, z, yaw)
-        
-
-    def inverse_kinematics(self, x, y, z, yaw):
-        """inverse kinematics algorism
-        
-        Args:
-            x: robot end x
-            y: robot end y
-            z: robot end z
-            yaw: robot end yaw
-        
-        Returns:
-            list of joint angles
-        """
-        z -= self.l01 - self.l45
-        angle = [0, 0, 0, 0]
-        
-        a = sqrt(x * x + y * y)
-        # beta = atan2(z, a)
-        b = sqrt(a * a + z * z)
-        cos_alpha = (b * b + self.l23 * self.l23 - self.l34 * self.l34) / (2 * b * self.l23)
-        
-        # cos_c = (self.l23 * self.l23 + self.l34 * self.l34 - b * b) / (2 * self.l34 * self.l23)
-        # theta_31 = acos(cos_c) - pi/2
-        
-        try:
-            alpha = acos(cos_alpha)
-        except ValueError:
-            print("Pose not in range! Choose other Pose that is not a singularity")
-            return self.get_joints_poses()
-
-        angle[0] = atan2(y, x)
-        angle[1] = atan2(a,z) -alpha
-        angle[2] = pi - pi/2 - alpha*2
-        angle[3] = yaw + angle[0]
-
-        return angle
+#!/usr/bin/env python
+# -*-coding:utf-8 -*-
+"""four_dof_pallet_robot.py
+Time    :   2022/10/17
+Author  :   ryan 
+Version :   1.0
+Contact :   ryanzhang@163.com
+License :   (C)Copyright 2022, robottime / robodyno
+
+4DoF Pallet Robot Drive
+
+  Typical usage example:
+
+  from robodyno.robots.four_dof_pallet_robot import FourDoFPallet
+  robot = FourDoFPallet(
+    j1 = base_motor,
+    j2 = upperarm_motor,
+    j3 = forearm_motor,
+    j4 = hand_motor,
+    l01 = 0.0794,
+    l23 = 0.190,
+    l34 = 0.190,
+    l45 = 0.010,
+    end_effector = None
+  )
+"""
+import time
+from math import pi, cos, sin, sqrt, atan2, acos
+from ..utils.interpolations import linear_interpolation
+
+class FourDoFPallet(object):
+    """4 DoF pallet robot driver
+    
+    Attributes:
+        joints: list of 4 joint motors
+        l01: link from world to joint 1 (m)
+        l23: link from joint 2 to joint 3 transverse distance (m)
+        l34: link from joint 3 to joint 4 longitudinal distance (m)
+        l45: link from joint 4 to joint 5 transverse distance (m)
+        end_effector: end effector object
+    """
+    def __init__(self, j1, j2, j3, j4, l01, l23, l34, l45, end_effector = None):
+        self.joints = [j1, j2, j3, j4]
+        self.l01 = l01
+        self.l23 = l23
+        self.l34 = l34
+        self.l45 = l45
+        self.end_effector = end_effector
+
+        for m in self.joints:
+          m.position_filter_mode(8)
+        self._axes_poses = [0 for i in range(4)]
+        self._axes_zeros = [0 for i in range(4)]
+
+    def get_joints_pose(self):
+        """Read joints position to a list.
+        
+        Returns:
+            a list of 4 joint positions
+        """
+        poses = []
+        for i in range(4):
+            pos = None
+            count = 0
+            while not pos:
+                if count > 5:
+                    raise RuntimeError('Filed to get position of Joint {}'.format(i+1))
+                count += 1
+                pos = self.joints[i].get_pos(0.2)
+            poses.append(pos - self._axes_zeros[i])
+        return poses
+
+    def enable(self):
+        """enable joints motors"""
+        for i in range(4):
+            self.joints[i].enable()
+
+    def disable(self):
+        """disable joints motors"""
+        for i in range(4):
+            self.joints[i].disable()
+
+    def init (self, axes_poses = [0 for i in range(4)]):
+        """Calibrate robot motors with given axes poses.
+        
+        Args:
+            axes_poses: list of 4 axes poses(rad)
+        """
+        self._axes_poses = axes_poses.copy()
+        self._axes_zeros = [0 for i in range(4)]
+        cur_poses = self.get_joints_pose()
+        for i in range(4):
+            self._axes_zeros[i] = cur_poses[i] - self._axes_poses[i]
+            self._axes_poses[i] = 0
+
+    def set_joint_pos(self, id, pos):
+        """Set joint angle with joint and position.
+        
+        Args:
+            id: joint id (0-3)
+            pos: joint target position(red)
+        """
+        self.joints[id].set_pos(pos + self._axes_zeros[id])
+        self._axes_poses[id] = pos        
+        
+    def joint_space_interpolated_motion(self, target, speeds = [0 for i in range(4)], duration = 0):
+        """Robot interpolated motion in joint space.
+        
+        Args:
+            target: iterable of 4 joints target angle(rad)
+            speeds: iterable of 4 joints motion speed(rad/s)
+            duration: default motion duration(s)
+        """
+        interpolation = []
+        joint_poses = self._axes_poses.copy()
+        for i in range(4):
+            interpolation.append(linear_interpolation(joint_poses[i], target[i], speed=speeds[i], duration=duration))
+        update_flag = True
+        while update_flag:
+            update_flag = False
+            for i in range(4):
+                pos = next(interpolation[i], None)
+                if pos is not None:
+                    self.set_joint_pos(i, pos)
+                    update_flag = True
+            time.sleep(0.05)
+
+    def home(self, duration = 5):
+        """Move back to zero position.
+        
+        Args:
+            duration: motion duration(s)
+        """
+        self.joint_space_interpolated_motion((0,0,0,0), duration = duration)
+
+    def cartesian_space_interpolated_motion(self, x, y, z, yaw, x_speed = None, y_speed = None, z_speed = None, yaw_speed = None, duration = 0):
+        """Robot Interpolated motion in cartesian space.
+        
+        Args:
+            x: target robot end x
+            y: target robot end y
+            z: target robot end z
+            yaw: target robot end yaw
+            x_speed: speed alone X dimension(m/s)
+            y_speed: speed alone Y dimension(m/s)
+            z_speed: speed alone Z dimension(m/s)
+            yaw_speed: rotation speed on Z axis(rad/s)
+            duration: default motion duration(s)
+        """
+        current_pose = self.forward_kinematics(self._axes_poses.copy())
+        current_x = current_pose[0]
+        current_y = current_pose[1]
+        current_z = current_pose[2]
+        current_yaw = current_pose[3]
+
+        x_interpolation = linear_interpolation(current_x, x, x_speed, duration)
+        y_interpolation = linear_interpolation(current_y, y, y_speed, duration)
+        z_interpolation = linear_interpolation(current_z, z, z_speed, duration)
+        yaw_interpolation = linear_interpolation(current_yaw, yaw, yaw_speed, duration)
+        
+        while True:
+            temp_x = next(x_interpolation, x)
+            temp_y = next(y_interpolation, y)
+            temp_z = next(z_interpolation, z)
+            temp_yaw = next(yaw_interpolation, yaw)
+
+            axes = self.inverse_kinematics(temp_x, temp_y, temp_z, temp_yaw)
+            for i in range(4):
+                self.set_joint_pos(i, axes[i])
+            if temp_x == x and temp_y == y and temp_z == z and temp_yaw == yaw:
+                break
+            time.sleep(0.05)
+
+    def forward_kinematics(self, angles):
+        """Forward kinematics algorism
+        
+        Args:
+            angles: list of 4 joint angles(rad)
+        
+        Returns:
+            (x, y, z, yaw): tuples of 3 axis position and 1 axis posture
+        """
+        a_2 = self.l23 * self.l23 + self.l34 * self.l34 - 2 * self.l23 * self.l34 * cos(pi/2 + angles[2])
+        a = sqrt(a_2)
+        cos_alpha = (self.l23 * self.l23 + a_2 - self.l34 * self.l34) / (2 * a * self.l23)
+        alpha = acos(cos_alpha)
+        
+        b = a * sin(alpha + angles[1])
+        
+        x = b * cos(angles[0])
+        y = b * sin(angles[0])
+        z = a * cos(alpha + angles[1]) + self.l01 - self.l45
+        yaw = -angles[0] + angles[3]
+
+        return (x, y, z, yaw)
+        
+
+    def inverse_kinematics(self, x, y, z, yaw):
+        """inverse kinematics algorism
+        
+        Args:
+            x: robot end x
+            y: robot end y
+            z: robot end z
+            yaw: robot end yaw
+        
+        Returns:
+            list of joint angles
+        """
+        z -= self.l01 - self.l45
+        angle = [0, 0, 0, 0]
+        
+        a = sqrt(x * x + y * y)
+        # beta = atan2(z, a)
+        b = sqrt(a * a + z * z)
+        cos_alpha = (b * b + self.l23 * self.l23 - self.l34 * self.l34) / (2 * b * self.l23)
+        
+        # cos_c = (self.l23 * self.l23 + self.l34 * self.l34 - b * b) / (2 * self.l34 * self.l23)
+        # theta_31 = acos(cos_c) - pi/2
+        
+        try:
+            alpha = acos(cos_alpha)
+        except ValueError:
+            print("Pose not in range! Choose other Pose that is not a singularity")
+            return self.get_joints_poses()
+
+        angle[0] = atan2(y, x)
+        angle[1] = atan2(a,z) -alpha
+        angle[2] = pi - pi/2 - alpha*2
+        angle[3] = yaw + angle[0]
+
+        return angle
```

### Comparing `robodyno-1.6.0/src/robodyno/robots/four_dof_scara_robot/four_dof_scara_robot.py` & `robodyno-1.6.1b0/src/robodyno/robots/three_dof_palletizing_robot/three_dof_pallet_robot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,240 +1,225 @@
-#!/usr/bin/env python
-# -*-coding:utf-8 -*-
-"""four_dof_scara_robot.py
-Time    :   2022/10/17
-Author  :   ryan 
-Version :   1.0
-Contact :   ryanzhang@163.com
-License :   (C)Copyright 2022, robottime / robodyno
-
-4DoF Scara robot Driver
-
-  Typical usage example:
-
-  from robodyno.robots.four_dof_scara_robot import FourDoFScara
-  robot = FourDoFScara(
-    j1 = shoulder_motor,
-    j2 = upperarm_motor,
-    j3 = forearm_motor,
-    j4 = hand_motor,
-    l12 = 0.100,
-    l23 = 0.185,
-    l34 = 0.185,
-    l04 = 0.255
-    screw_lead = 0.0102,
-    end_effector = None
-  )
-"""
-import time
-from math import pi, cos, sin, sqrt, atan2
-from ..utils.interpolations import linear_interpolation
-
-class FourDoFScara(object):
-    """4 DoF scara robot driver
-    
-    Attributes:
-        joints: list of 4 joint motors
-        l12: link from joint 1 to joint 2  (m)
-        l23: link from joint 2 to joint 3  (m)
-        l34: link from joint 3 to joint 4  (m)
-        l04: link from world to joint 4 longitudinal distance (m)
-        screw_lead: screw lead (m)
-        end_effector: end effector object
-
-    """
-    def __init__(self, j1, j2, j3, j4, l12, l23, l34, l04, screw_lead, end_effector = None):
-        """init robot with joints and links"""
-        self.joints = [j1, j2, j3, j4]
-        self.l12 = l12
-        self.l23 = l23
-        self.l34 = l34
-        self.l04 = l04
-        self.screw_lead = screw_lead
-        self.end_effector = end_effector
-
-        for m in self.joints:
-            m.position_filter_mode(8)
-        # self.motors[0].position_traj_mode(10,5,5)
-        self._axes_poses = [0 for i in range(4)]
-        self._axes_zeros = [0 for i in range(4)]
-
-    def get_joints_poses(self):
-        """Read joints positions to a list.
-        
-        Returns:
-            a list of 4 joint positions
-        """
-        poses = []
-        for i in range(4):
-            pos = None
-            count = 0
-            while not pos:
-                if count > 5:
-                    raise RuntimeError('Filed to get position of Joint {}'.format(i+1))
-                count += 1
-                pos = self.joints[i].get_pos(0.2)
-            poses.append(pos - self._axes_zeros[i])
-        return poses
-
-    def enable(self):
-        """enable joints motors"""
-        for i in range(4):
-            self.joints[i].enable()
-
-    def disable(self):
-        """disable joints motors"""
-        for i in range(4):
-            self.joints[i].disable()
-
-    def init(self, axes_poses = [0 for i in range(4)]):
-        """Calibrate robot motors with given axes poses.
-        
-        Args:
-            axes_poses: list of 4 axes poses(rad)
-        """
-        self._axes_poses = axes_poses.copy()
-        self._axes_zeros = [0 for i in range(4)]
-        cur_poses = self.get_joints_poses()
-        for i in range(4):
-            self._axes_zeros[i] = cur_poses[i] - self._axes_poses[i]
-            self._axes_poses[i] = 0
-
-    def set_joint_pos(self, id, pos):
-        """Set joint angle with joint id and position
-        
-        Args:
-            id: joint id (0-3)
-            pos: joint target position(rad)
-        """
-        self.joints[id].set_pos(pos + self._axes_zeros[id])
-        self._axes_poses[id] = pos
-
-    def joint_space_interpolated_motion(self, target, speeds = [None for i in range(4)], duration = 0):
-        """Robot interpolated motion in joint space.
-        
-        Args:
-            target: iterable of 4 joints target angle(rad)
-            speeds: iterable of 4 joints motion speed(rad/s)
-            duration: default motion duration(s)
-        """
-        interpolation = []
-        joint_poses = self._axes_poses.copy()
-        for i in range(4):
-            interpolation.append(linear_interpolation(joint_poses[i], target[i], speed=speeds[i], duration=duration))
-        update_flag = True
-        while update_flag:
-            update_flag = False
-            for i in range(4):
-                pos = next(interpolation[i], None)
-                if pos is not None:
-                    self.set_joint_pos(i, pos)
-                    update_flag = True
-            time.sleep(0.05)
-
-    def home(self, duration = 5):
-        """Move back to zero position.
-        
-        Args:
-            duration: motion duration(s)
-        """
-        self.joint_space_interpolated_motion((0,0,0,0), duration = duration)
-
-    def cartesian_space_interpolated_motion(self, x, y, z, yaw, x_speed = None, y_speed = None, z_speed = None, yaw_speed = None, hand_coordinate = 1, duration = 0):
-        """Robot Interpolated motion in cartesian space.
-        
-        Args:
-            x: target robot end x
-            y: target robot end y
-            z: target robot end z
-            yaw: target robot end yaw
-            x_speed: speed alone X dimension(m/s)
-            y_speed: speed alone Y dimension(m/s)
-            z_speed: speed alone Z dimension(m/s)
-            yaw_speed: rotation speed on Z axis(rad/s)
-            hand_coordinate: 0 is left hand coordinate system
-                             1 is right hand coordinate system
-            duration: default motion duration(s)
-        """
-        current_pose = self.forward_kinematics(self._axes_poses.copy())
-        current_x = current_pose[0]
-        current_y = current_pose[1]
-        current_z = current_pose[2]
-        current_yaw = current_pose[3]
-
-        x_interpolation = linear_interpolation(current_x, x, x_speed, duration)
-        y_interpolation = linear_interpolation(current_y, y, y_speed, duration)
-        z_interpolation = linear_interpolation(current_z, z, z_speed, duration)
-        yaw_interpolation = linear_interpolation(current_yaw, yaw, yaw_speed, duration)
-        
-        while True:
-            temp_x = next(x_interpolation, x)
-            temp_y = next(y_interpolation, y)
-            temp_z = next(z_interpolation, z)
-            temp_yaw = next(yaw_interpolation, yaw)
-
-            axes = self.inverse_kinematics(temp_x, temp_y, temp_z, temp_yaw , hand_coordinate)
-            for i in range(4):
-                self.set_joint_pos(i, axes[i])
-            if temp_x == x and temp_y == y and temp_z == z and temp_yaw == yaw:
-                break
-            time.sleep(0.05)
-
-    def forward_kinematics(self, angles):
-        """Forward kinematics algorism
-        
-        Args:
-            angles: list of 4 joint angles(rad)
-        
-        Returns:
-            (x, y, z, yaw): tuples of 3 axis position and 1 axis posture
-        """
-        x = self.l23 * cos(angles[1]) + self.l34 * cos(angles[1] + angles[2]) + self.l12
-        y = self.l23 * sin(angles[1]) + self.l34 * sin(angles[1] + angles[2])
-        z = angles[0] * self.screw_lead / (2 * pi) + self.l04
-        yaw = -angles[3] + angles[1] + angles[2]
-
-        return (x, y, z, yaw)
-    
-    def inverse_kinematics(self, x, y, z, yaw, hand_coordinate = 1):
-        """inverse kinematics algorism
-        
-        Args:
-            x: robot end x
-            y: robot end y
-            z: robot end z
-            yaw: robot end yaw
-            hand_coordinate: 0 is left hand coordinate system
-                             1 is right hand coordinate system
-        
-        Returns:
-            list of 4 joint angles
-        """
-        angle = [0, 0, 0, 0]
-        x -= self.l12
-        z -= self.l04
-        
-        c3 = (x*x + y*y - self.l23*self.l23 - self.l34*self.l34) / (2.0 * self.l23 * self.l34)
-        temp = 1 - c3 * c3
-        try:
-            if(hand_coordinate == 1):
-                s3 = sqrt(temp)  # right
-            elif(hand_coordinate == 0):
-                s3 = -sqrt(temp) # left
-        except ValueError:
-            print("Pose not in range! Choose other Pose that is not a singularity")
-            return self.get_joints_poses()
-         
-        angle[2] = atan2(s3, c3)
-         
-        alpha = atan2(y, x)
-        r = sqrt(x*x + y*y)
-        sin_beta = self.l34 * sin(angle[2]) / r
-        cos_beta = (self.l23 + self.l34 * cos(angle[2])) / r
-        beta = atan2(sin_beta, cos_beta)
-        angle[1] = alpha - beta
-        
-        angle[0] = (2*pi * z) / self.screw_lead
-        angle[3] = angle[1] + angle[2] - yaw
-         
-        return angle
-        
+#!/usr/bin/env python
+# -*-coding:utf-8 -*-
+"""three_dof_pallet_robot.py
+Time    :   2022/10/17
+Author  :   ryan 
+Version :   1.0
+Contact :   ryanzhang@163.com
+License :   (C)Copyright 2022, robottime / robodyno
+
+3DoF Pallet Robot Drive
+
+  Typical usage example:
+
+  from robodyno.robots.three_dof_pallet_robot import ThreeDoFPallet
+  robot = ThreeDoFPallet(
+    j1 = base_motor,
+    j2 = upperarm_motor,
+    j3 = forearm_motor,
+    l01 = 0.0794,
+    l23 = 0.190,
+    l34 = 0.190,
+    l45 = 0.010,
+    end_effector = None
+  )
+"""
+import time
+from math import pi, cos, sin, sqrt, atan2, acos
+from ..utils.interpolations import linear_interpolation
+
+class ThreeDoFPallet(object):
+    """3 DoF pallet robot driver
+    
+    Attributes:
+        joints: list of 3 joint motors
+        l01: link from world to joint 1 (m)
+        l23: link from joint 2 to joint 3 transverse distance (m)
+        l34: link from joint 3 to joint 4 longitudinal distance (m)
+        l45: link from joint 4 to joint 5 transverse distance (m)
+        end_effector: end effector object
+    """
+    def __init__(self, j1, j2, j3, l01, l23, l34, l45, end_effector = None):
+        self.joints = [j1, j2, j3]
+        self.l01 = l01
+        self.l23 = l23
+        self.l34 = l34
+        self.l45 = l45
+        self.end_effector = end_effector
+
+        for m in self.joints:
+          m.position_filter_mode(8)
+        self._axes_poses = [0 for i in range(3)]
+        self._axes_zeros = [0 for i in range(3)]
+
+    def get_joints_pose(self):
+        """Read joints position to a list.
+        
+        Returns:
+            a list of 3 joint positions
+        """
+        poses = []
+        for i in range(3):
+            pos = None
+            count = 0
+            while not pos:
+                if count > 5:
+                    raise RuntimeError('Filed to get position of Joint {}'.format(i+1))
+                count += 1
+                pos = self.joints[i].get_pos(0.2)
+            poses.append(pos - self._axes_zeros[i])
+        return poses
+
+    def enable(self):
+        """enable joints motors"""
+        for i in range(3):
+            self.joints[i].enable()
+
+    def disable(self):
+        """disable joints motors"""
+        for i in range(3):
+            self.joints[i].disable()
+
+    def init (self, axes_poses = [0 for i in range(3)]):
+        """Calibrate robot motors with given axes poses.
+        
+        Args:
+            axes_poses: list of 3 axes poses(rad)
+        """
+        self._axes_poses = axes_poses.copy()
+        self._axes_zeros = [0 for i in range(3)]
+        cur_poses = self.get_joints_pose()
+        for i in range(3):
+            self._axes_zeros[i] = cur_poses[i] - self._axes_poses[i]
+            self._axes_poses[i] = 0
+
+    def set_joint_pos(self, id, pos):
+        """Set joint angle with joint and position.
+        
+        Args:
+            id: joint id (0-2)
+            pos: joint target position(red)
+        """
+        self.joints[id].set_pos(pos + self._axes_zeros[id])
+        self._axes_poses[id] = pos        
+        
+    def joint_space_interpolated_motion(self, target, speeds = [0 for i in range(3)], duration = 0):
+        """Robot interpolated motion in joint space.
+        
+        Args:
+            target: iterable of 3 joints target angle(rad)
+            speeds: iterable of 3 joints motion speed(rad/s)
+            duration: default motion duration(s)
+        """
+        interpolation = []
+        joint_poses = self._axes_poses.copy()
+        for i in range(3):
+            interpolation.append(linear_interpolation(joint_poses[i], target[i], speed=speeds[i], duration=duration))
+        update_flag = True
+        while update_flag:
+            update_flag = False
+            for i in range(3):
+                pos = next(interpolation[i], None)
+                if pos is not None:
+                    self.set_joint_pos(i, pos)
+                    update_flag = True
+            time.sleep(0.05)
+
+    def home(self, duration = 5):
+        """Move back to zero position.
+        
+        Args:
+            duration: motion duration(s)
+        """
+        self.joint_space_interpolated_motion((0,0,0), duration = duration)
+
+    def cartesian_space_interpolated_motion(self, x, y, z, x_speed = None, y_speed = None, z_speed = None, duration = 0):
+        """Robot Interpolated motion in cartesian space.
+        
+        Args:
+            x: target robot end x
+            y: target robot end y
+            z: target robot end z
+            x_speed: speed alone X dimension(m/s)
+            y_speed: speed alone Y dimension(m/s)
+            z_speed: speed alone Z dimension(m/s)
+            duration: default motion duration(s)
+        """
+        current_pose = self.forward_kinematics(self._axes_poses.copy())
+        current_x = current_pose[0]
+        current_y = current_pose[1]
+        current_z = current_pose[2]
+
+        x_interpolation = linear_interpolation(current_x, x, x_speed, duration)
+        y_interpolation = linear_interpolation(current_y, y, y_speed, duration)
+        z_interpolation = linear_interpolation(current_z, z, z_speed, duration)
+        
+        while True:
+            temp_x = next(x_interpolation, x)
+            temp_y = next(y_interpolation, y)
+            temp_z = next(z_interpolation, z)
+
+            axes = self.inverse_kinematics(temp_x, temp_y, temp_z)
+            for i in range(4):
+                self.set_joint_pos(i, axes[i])
+            if temp_x == x and temp_y == y and temp_z == z:
+                break
+            time.sleep(0.05)
+
+    def forward_kinematics(self, angles):
+        """Forward kinematics algorism
+        
+        Args:
+            angles: list of 3 joint angles(rad)
+        
+        Returns:
+            (x, y, z): tuples of 3 axis position
+        """
+        a_2 = self.l23 * self.l23 + self.l34 * self.l34 - 2 * self.l23 * self.l34 * cos(pi/2 + angles[2])
+        a = sqrt(a_2)
+        # alpha = (pi-pi/2-theta3) / 2
+        cos_alpha = (self.l23 * self.l23 + a_2 - self.l34 * self.l34) / (2 * a * self.l23)
+        alpha = acos(cos_alpha)
+        # print(alpha)
+        
+        b = a * sin(alpha + angles[1])
+        
+        x = b * cos(angles[0])
+        y = b * sin(angles[0])
+        z = a * cos(alpha + angles[1]) + self.l01 - self.l45
+        return (x, y, z)
+        
+
+    def inverse_kinematics(self, x, y, z):
+        """inverse kinematics algorism
+        
+        Args:
+            x: robot end x
+            y: robot end y
+            z: robot end z
+        
+        Returns:
+            list of joint angles
+        """
+        cf = z - self.l01 + self.l45
+        angle = [0, 0, 0]
+        
+        a = sqrt(x * x + y * y)
+        # beta = atan2(z, a)
+        r = sqrt(a * a + cf * cf)
+        cos_alpha = (r * r + self.l23 * self.l23 - self.l34 * self.l34) / (2 * r * self.l23)
+        
+        cos_abc = (self.l23 * self.l23 + self.l34 * self.l34 - r * r) / (2 * self.l34 * self.l23)
+        
+        try:
+            alpha = acos(cos_alpha)
+            abc = acos(cos_abc)
+        except ValueError:
+            print("Pose not in range! Choose other Pose that is not a singularity")
+            return self.get_joints_poses()
+
+        angle[0] = atan2(y, x)
+        angle[1] = atan2(a,z) -alpha
+        angle[2] = abc - pi/2
+
+        return angle
+
```

### Comparing `robodyno-1.6.0/src/robodyno/robots/three_dof_delta_robot/three_dof_delta_robot.py` & `robodyno-1.6.1b0/src/robodyno/robots/three_dof_delta_robot/three_dof_delta_robot.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,284 +1,284 @@
-#!/usr/bin/env python
-# -*-coding:utf-8 -*-
-"""three_dof_delta_robot.py
-Time    :   2022/10/09
-Author  :   ryan 
-Version :   1.0
-Contact :   ryanzhang@163.com
-License :   (C)Copyright 2022, robottime / robodyno
-
-3DoF Delta Robot Drive
-
-  Typical usage example:
-
-  from robodyno.robots.three_dof_delta_robot import ThreeDoFDelta
-  robot = ThreeDoFDelta(
-    j1 = delta_motor1,
-    j2 = delta_motor2,
-    j3 = delta_motor3,
-    l1 = 0.12864,
-    l2 = 0.3,
-    r1 = 0.13856,
-    r2 = 0.025,
-    end_effector = None
-  )
-  
-"""
-import time
-import numpy as np
-from math import pi, cos, sin, sqrt, atan
-from ..utils.interpolations import linear_interpolation
-
-
-class ThreeDoFDelta(object):
-    """3 DoF delta robot driver
-    
-    Attributes:
-        joints: list of 3 joint motors
-        l1: link is the active arm (m)
-        l2: link is the slave arm (m) 
-        r1: fixed platform radius (m)
-        r2: motion platform radius (m)
-        end_effector: end effector object
-    """
-    def __init__(self, j1, j2, j3, l1, l2, r1, r2, end_effector = None):
-        """init robot with joints and links"""
-        self.joints = [j1, j2, j3]
-        self.l1 = l1
-        self.l2 = l2
-        self.r1 = r1
-        self.r2 = r2
-        self.end_effector = end_effector
-
-        for m in self.joints:
-            m.position_filter_mode(8)
-        self._axes_poses = [0 for i in range(3)]
-        self._axes_zeros = [0 for i in range(3)]
-        self._link_deviation = 0.08 # 4.63°
-
-    def get_joints_poses(self):
-        """Read joints positions to a list.
-
-        Returns:
-            a list of 3 joint positions
-        """
-        poses = []
-        for i in range(3):
-            pos = None
-            count = 0
-            while not pos:
-                if count > 5:
-                    raise RuntimeError('Filed to get position of Joint {}'.format(i+1))
-                count += 1
-                pos = self.joints[i].get_pos(0.2)
-            poses.append(pos - self._axes_zeros[i])
-        return poses
-
-    def enable(self):
-        """enable joints motors"""
-        for i in range(3):
-            self.joints[i].enable()
-
-    def disable(self):
-        """disable joints motors"""
-        for i in range(3):
-            self.joints[i].disable()
-
-    def init(self, axes_poses = [0 for i in range(3)]):
-        """Calibrate robot motors with given axes poses.
-        
-        Args:
-            axes_poses: list of 3 axes poses(rad)
-        """
-        self._axes_poses = axes_poses.copy()
-        self._axes_zeros = [0 for i in range(3)]
-        cur_poses = self.get_joints_poses()
-        for i in range(3):
-            self._axes_zeros[i] = cur_poses[i] - self._axes_poses[i]
-            self._axes_poses[i] = 0
-
-    def set_joint_pos(self, id, pos):
-        """Set joint angle with joint id and position
-        
-        Args:
-            id: joint id (0-2)
-            pos: joint target position(rad)
-        """
-        self.joints[id].set_pos(pos + self._axes_zeros[id])
-        self._axes_poses[id] = pos
-
-    def joint_space_interpolated_motion(self, target, speeds = [None for i in range(3)], duration = 0):
-        """Robot interpolated motion in joint space.
-        
-        Args:
-            target: iterable of 3 joints target angle(rad)
-            speeds: iterable of 3 joints motion speed(rad/s)
-            duration: default motion duration(s)
-        """
-        interpolation = []
-        joint_poses = self._axes_poses.copy()
-        for i in range(3):
-            interpolation.append(linear_interpolation(joint_poses[i], target[i], speed=speeds[i], duration=duration))
-        update_flag = True
-        while update_flag:
-            update_flag = False
-            for i in range(3):
-                pos = next(interpolation[i], None)
-                if pos is not None:
-                    self.set_joint_pos(i, pos)
-                    update_flag = True
-            time.sleep(0.05)
-    
-    def home(self, duration = 5):
-        """Move back to zero position.
-        
-        Args:
-            duration: motion duration(s)
-        """
-        self.joint_space_interpolated_motion((0,0,0), duration = duration)
-
-    def cartesian_space_interpolated_motion(self, x, y, z, x_speed = None, y_speed = None, z_speed = None, duration = 0):
-        """Robot Interpolated motion in cartesian space.
-        
-        Args:
-            x: target robot end x
-            y: target robot end y
-            z: target robot end z
-            x_speed: speed alone X dimension(m/s)
-            y_speed: speed alone Y dimension(m/s)
-            z_speed: speed alone Z dimension(m/s)
-            duration: default motion duration(s)
-        """
-        current_pose = self.forward_kinematics(self._axes_poses.copy())
-        current_x = current_pose[0]
-        current_y = current_pose[1]
-        current_z = current_pose[2]
-
-        x_interpolation = linear_interpolation(current_x, x, x_speed, duration)
-        y_interpolation = linear_interpolation(current_y, y, y_speed, duration)
-        z_interpolation = linear_interpolation(current_z, z, z_speed, duration)
-        
-        while True:
-            temp_x = next(x_interpolation, x)
-            temp_y = next(y_interpolation, y)
-            temp_z = next(z_interpolation, z)
-
-            axes = self.inverse_kinematics(temp_x, temp_y, temp_z)
-            for i in range(3):
-                self.set_joint_pos(i, axes[i])
-            if temp_x == x and temp_y == y and temp_z == z:
-                break
-            time.sleep(0.05)
-
-    def forward_kinematics(self, angles):
-        """Forward kinematics algorism
-        
-        Args:
-            angles: list of 3 joint angles(rad)
-        
-        Returns:
-            (x, y, z): tuples of 3 axis position
-        """
-        cos_0 = cos(0) # 0°
-        sin_0 = sin(0)
-        cos_120 = cos(2 * pi / 3) # 120°
-        sin_120 = sin(2 * pi / 3)
-        cos_240 = cos(4 * pi / 3) # 240°
-        sin_240 = sin(4 * pi / 3)
-        
-        theta1 = angles[0] + self._link_deviation  
-        theta2 = angles[1] + self._link_deviation 
-        theta3 = angles[2] + self._link_deviation 
-
-        O_C1 = np.array([self.r1 * cos_0  , self.r1 * sin_0  , 0])
-        O_C2 = np.array([self.r1 * cos_120, self.r1 * sin_120, 0])
-        O_C3 = np.array([self.r1 * cos_240, self.r1 * sin_240, 0])
-
-        C1_B1 = np.array([-self.l1*sin(theta1)*cos_0  , -self.l1*sin(theta1)*sin_0  , -self.l1*cos(theta1)])
-        C2_B2 = np.array([-self.l1*sin(theta2)*cos_120, -self.l1*sin(theta2)*sin_120, -self.l1*cos(theta2)])
-        C3_B3 = np.array([-self.l1*sin(theta3)*cos_240, -self.l1*sin(theta3)*sin_240, -self.l1*cos(theta3)])
-
-        A1_P = np.array([-self.r2*cos_0  , -self.r2*sin_0  , 0])
-        A2_P = np.array([-self.r2*cos_120, -self.r2*sin_120, 0])
-        A3_P = np.array([-self.r2*cos_240, -self.r2*sin_240, 0])
-
-        O_D1 = O_C1 + C1_B1 + A1_P
-        O_D2 = O_C2 + C2_B2 + A2_P
-        O_D3 = O_C3 + C3_B3 + A3_P
-        
-        D2_D1 = O_D1 - O_D2
-        D2_D3 = O_D3 - O_D2
-        D3_D1 = O_D1 - O_D3
-        D3_D2 = O_D2 - O_D3
-
-        a = np.linalg.norm(D2_D1)
-        b = np.linalg.norm(D2_D3)
-        c = np.linalg.norm(D3_D1)
-
-        p = (a + b + c) / 2
-        S = sqrt(p * (p-a) * (p-b) * (p-c))
-        D2_E_norm = a * b * c / (4 * S)
-
-        D2_F_norm = b / 2
-        FE_norm = np.linalg.norm(sqrt(D2_E_norm * D2_E_norm - D2_F_norm * D2_F_norm))
-
-        nF_E1 = np.cross(np.cross(D2_D1, D2_D3), D3_D2) / (a * b * b)
-        nF_E = nF_E1 / np.linalg.norm(nF_E1)
-
-        nE_P1 = np.cross(D2_D1, D2_D3) / (a * b)
-        nE_P = nE_P1 / np.linalg.norm(nE_P1)
-
-        D1_P_norm = self.l2
-        D1_E_norm = a * b * c / (4 * S)
-
-        EP_norm = sqrt(D1_P_norm * D1_P_norm - D1_E_norm * D1_E_norm)
-        EP = EP_norm * nE_P
-
-        OF = (O_D2 + O_D3) / 2
-        FE = FE_norm *nF_E
-        OE = OF + FE
-
-        OP = OE + EP
-
-        x = OP[0]
-        y = OP[1]
-        z = OP[2]
-
-        return (x, y, z)
-
-    def inverse_kinematics(self, x, y, z):
-        """inverse kinematics algorism
-        
-        Args:
-            x: robot end x
-            y: robot end y
-            z: robot end z
-        
-        Returns:
-            list of joint angles
-        """
-        angles = [0, 0, 0]
-        m = x*x + y*y + z*z + (self.r1-self.r2)*(self.r1-self.r2) + self.l1*self.l1 - self.l2*self.l2 
-        A = [(m - 2 * x * (self.r1 - self.r2)) / (2 * self.l1) - (self.r1 - self.r2 - x),
-             (m + (self.r1 - self.r2) * (x - sqrt(3) * y)) / (self.l1) - 2 * (self.r1 - self.r2) - (x - sqrt(3) * y),
-             (m + (self.r1 - self.r2) * (x + sqrt(3) * y)) / (self.l1) - 2 * (self.r1 - self.r2) - (x + sqrt(3) * y)]
-
-        B = [2 * z,
-             4 * z,
-             4 * z]
-        C = [(m - 2 * x * (self.r1 - self.r2)) / (2 * self.l1) + (self.r1 - self.r2 - x),
-             (m + (self.r1 - self.r2) * (x - sqrt(3) * y)) / (self.l1) + 2 * (self.r1 - self.r2) + (x - sqrt(3) * y),
-             (m + (self.r1 - self.r2) * (x + sqrt(3) * y)) / (self.l1) + 2 * (self.r1 - self.r2) + (x + sqrt(3) * y)]
-        
-        delta = [0,0,0]
-        for i in range(3):
-            delta[i] = B[i] * B[i] - 4 * A[i] * C[i]
-            try:
-                t = (-B[i] - sqrt(delta[i])) / (2 * A[i])
-                angles[i] = 2 * atan(t) - (pi/2 + self._link_deviation)
-            except ValueError:
-                print('Pose not in range! Choose other Pose that is not a singularity')
-                return self.get_joints_poses()
-
-        return angles
-
+#!/usr/bin/env python
+# -*-coding:utf-8 -*-
+"""three_dof_delta_robot.py
+Time    :   2022/10/09
+Author  :   ryan 
+Version :   1.0
+Contact :   ryanzhang@163.com
+License :   (C)Copyright 2022, robottime / robodyno
+
+3DoF Delta Robot Drive
+
+  Typical usage example:
+
+  from robodyno.robots.three_dof_delta_robot import ThreeDoFDelta
+  robot = ThreeDoFDelta(
+    j1 = delta_motor1,
+    j2 = delta_motor2,
+    j3 = delta_motor3,
+    l1 = 0.12864,
+    l2 = 0.3,
+    r1 = 0.13856,
+    r2 = 0.025,
+    end_effector = None
+  )
+  
+"""
+import time
+import numpy as np
+from math import pi, cos, sin, sqrt, atan
+from ..utils.interpolations import linear_interpolation
+
+
+class ThreeDoFDelta(object):
+    """3 DoF delta robot driver
+    
+    Attributes:
+        joints: list of 3 joint motors
+        l1: link is the active arm (m)
+        l2: link is the slave arm (m) 
+        r1: fixed platform radius (m)
+        r2: motion platform radius (m)
+        end_effector: end effector object
+    """
+    def __init__(self, j1, j2, j3, l1, l2, r1, r2, end_effector = None):
+        """init robot with joints and links"""
+        self.joints = [j1, j2, j3]
+        self.l1 = l1
+        self.l2 = l2
+        self.r1 = r1
+        self.r2 = r2
+        self.end_effector = end_effector
+
+        for m in self.joints:
+            m.position_filter_mode(8)
+        self._axes_poses = [0 for i in range(3)]
+        self._axes_zeros = [0 for i in range(3)]
+        self._link_deviation = 0.08 # 4.63°
+
+    def get_joints_poses(self):
+        """Read joints positions to a list.
+
+        Returns:
+            a list of 3 joint positions
+        """
+        poses = []
+        for i in range(3):
+            pos = None
+            count = 0
+            while not pos:
+                if count > 5:
+                    raise RuntimeError('Filed to get position of Joint {}'.format(i+1))
+                count += 1
+                pos = self.joints[i].get_pos(0.2)
+            poses.append(pos - self._axes_zeros[i])
+        return poses
+
+    def enable(self):
+        """enable joints motors"""
+        for i in range(3):
+            self.joints[i].enable()
+
+    def disable(self):
+        """disable joints motors"""
+        for i in range(3):
+            self.joints[i].disable()
+
+    def init(self, axes_poses = [0 for i in range(3)]):
+        """Calibrate robot motors with given axes poses.
+        
+        Args:
+            axes_poses: list of 3 axes poses(rad)
+        """
+        self._axes_poses = axes_poses.copy()
+        self._axes_zeros = [0 for i in range(3)]
+        cur_poses = self.get_joints_poses()
+        for i in range(3):
+            self._axes_zeros[i] = cur_poses[i] - self._axes_poses[i]
+            self._axes_poses[i] = 0
+
+    def set_joint_pos(self, id, pos):
+        """Set joint angle with joint id and position
+        
+        Args:
+            id: joint id (0-2)
+            pos: joint target position(rad)
+        """
+        self.joints[id].set_pos(pos + self._axes_zeros[id])
+        self._axes_poses[id] = pos
+
+    def joint_space_interpolated_motion(self, target, speeds = [None for i in range(3)], duration = 0):
+        """Robot interpolated motion in joint space.
+        
+        Args:
+            target: iterable of 3 joints target angle(rad)
+            speeds: iterable of 3 joints motion speed(rad/s)
+            duration: default motion duration(s)
+        """
+        interpolation = []
+        joint_poses = self._axes_poses.copy()
+        for i in range(3):
+            interpolation.append(linear_interpolation(joint_poses[i], target[i], speed=speeds[i], duration=duration))
+        update_flag = True
+        while update_flag:
+            update_flag = False
+            for i in range(3):
+                pos = next(interpolation[i], None)
+                if pos is not None:
+                    self.set_joint_pos(i, pos)
+                    update_flag = True
+            time.sleep(0.05)
+    
+    def home(self, duration = 5):
+        """Move back to zero position.
+        
+        Args:
+            duration: motion duration(s)
+        """
+        self.joint_space_interpolated_motion((0,0,0), duration = duration)
+
+    def cartesian_space_interpolated_motion(self, x, y, z, x_speed = None, y_speed = None, z_speed = None, duration = 0):
+        """Robot Interpolated motion in cartesian space.
+        
+        Args:
+            x: target robot end x
+            y: target robot end y
+            z: target robot end z
+            x_speed: speed alone X dimension(m/s)
+            y_speed: speed alone Y dimension(m/s)
+            z_speed: speed alone Z dimension(m/s)
+            duration: default motion duration(s)
+        """
+        current_pose = self.forward_kinematics(self._axes_poses.copy())
+        current_x = current_pose[0]
+        current_y = current_pose[1]
+        current_z = current_pose[2]
+
+        x_interpolation = linear_interpolation(current_x, x, x_speed, duration)
+        y_interpolation = linear_interpolation(current_y, y, y_speed, duration)
+        z_interpolation = linear_interpolation(current_z, z, z_speed, duration)
+        
+        while True:
+            temp_x = next(x_interpolation, x)
+            temp_y = next(y_interpolation, y)
+            temp_z = next(z_interpolation, z)
+
+            axes = self.inverse_kinematics(temp_x, temp_y, temp_z)
+            for i in range(3):
+                self.set_joint_pos(i, axes[i])
+            if temp_x == x and temp_y == y and temp_z == z:
+                break
+            time.sleep(0.05)
+
+    def forward_kinematics(self, angles):
+        """Forward kinematics algorism
+        
+        Args:
+            angles: list of 3 joint angles(rad)
+        
+        Returns:
+            (x, y, z): tuples of 3 axis position
+        """
+        cos_0 = cos(0) # 0°
+        sin_0 = sin(0)
+        cos_120 = cos(2 * pi / 3) # 120°
+        sin_120 = sin(2 * pi / 3)
+        cos_240 = cos(4 * pi / 3) # 240°
+        sin_240 = sin(4 * pi / 3)
+        
+        theta1 = angles[0] + self._link_deviation  
+        theta2 = angles[1] + self._link_deviation 
+        theta3 = angles[2] + self._link_deviation 
+
+        O_C1 = np.array([self.r1 * cos_0  , self.r1 * sin_0  , 0])
+        O_C2 = np.array([self.r1 * cos_120, self.r1 * sin_120, 0])
+        O_C3 = np.array([self.r1 * cos_240, self.r1 * sin_240, 0])
+
+        C1_B1 = np.array([-self.l1*sin(theta1)*cos_0  , -self.l1*sin(theta1)*sin_0  , -self.l1*cos(theta1)])
+        C2_B2 = np.array([-self.l1*sin(theta2)*cos_120, -self.l1*sin(theta2)*sin_120, -self.l1*cos(theta2)])
+        C3_B3 = np.array([-self.l1*sin(theta3)*cos_240, -self.l1*sin(theta3)*sin_240, -self.l1*cos(theta3)])
+
+        A1_P = np.array([-self.r2*cos_0  , -self.r2*sin_0  , 0])
+        A2_P = np.array([-self.r2*cos_120, -self.r2*sin_120, 0])
+        A3_P = np.array([-self.r2*cos_240, -self.r2*sin_240, 0])
+
+        O_D1 = O_C1 + C1_B1 + A1_P
+        O_D2 = O_C2 + C2_B2 + A2_P
+        O_D3 = O_C3 + C3_B3 + A3_P
+        
+        D2_D1 = O_D1 - O_D2
+        D2_D3 = O_D3 - O_D2
+        D3_D1 = O_D1 - O_D3
+        D3_D2 = O_D2 - O_D3
+
+        a = np.linalg.norm(D2_D1)
+        b = np.linalg.norm(D2_D3)
+        c = np.linalg.norm(D3_D1)
+
+        p = (a + b + c) / 2
+        S = sqrt(p * (p-a) * (p-b) * (p-c))
+        D2_E_norm = a * b * c / (4 * S)
+
+        D2_F_norm = b / 2
+        FE_norm = np.linalg.norm(sqrt(D2_E_norm * D2_E_norm - D2_F_norm * D2_F_norm))
+
+        nF_E1 = np.cross(np.cross(D2_D1, D2_D3), D3_D2) / (a * b * b)
+        nF_E = nF_E1 / np.linalg.norm(nF_E1)
+
+        nE_P1 = np.cross(D2_D1, D2_D3) / (a * b)
+        nE_P = nE_P1 / np.linalg.norm(nE_P1)
+
+        D1_P_norm = self.l2
+        D1_E_norm = a * b * c / (4 * S)
+
+        EP_norm = sqrt(D1_P_norm * D1_P_norm - D1_E_norm * D1_E_norm)
+        EP = EP_norm * nE_P
+
+        OF = (O_D2 + O_D3) / 2
+        FE = FE_norm *nF_E
+        OE = OF + FE
+
+        OP = OE + EP
+
+        x = OP[0]
+        y = OP[1]
+        z = OP[2]
+
+        return (x, y, z)
+
+    def inverse_kinematics(self, x, y, z):
+        """inverse kinematics algorism
+        
+        Args:
+            x: robot end x
+            y: robot end y
+            z: robot end z
+        
+        Returns:
+            list of joint angles
+        """
+        angles = [0, 0, 0]
+        m = x*x + y*y + z*z + (self.r1-self.r2)*(self.r1-self.r2) + self.l1*self.l1 - self.l2*self.l2 
+        A = [(m - 2 * x * (self.r1 - self.r2)) / (2 * self.l1) - (self.r1 - self.r2 - x),
+             (m + (self.r1 - self.r2) * (x - sqrt(3) * y)) / (self.l1) - 2 * (self.r1 - self.r2) - (x - sqrt(3) * y),
+             (m + (self.r1 - self.r2) * (x + sqrt(3) * y)) / (self.l1) - 2 * (self.r1 - self.r2) - (x + sqrt(3) * y)]
+
+        B = [2 * z,
+             4 * z,
+             4 * z]
+        C = [(m - 2 * x * (self.r1 - self.r2)) / (2 * self.l1) + (self.r1 - self.r2 - x),
+             (m + (self.r1 - self.r2) * (x - sqrt(3) * y)) / (self.l1) + 2 * (self.r1 - self.r2) + (x - sqrt(3) * y),
+             (m + (self.r1 - self.r2) * (x + sqrt(3) * y)) / (self.l1) + 2 * (self.r1 - self.r2) + (x + sqrt(3) * y)]
+        
+        delta = [0,0,0]
+        for i in range(3):
+            delta[i] = B[i] * B[i] - 4 * A[i] * C[i]
+            try:
+                t = (-B[i] - sqrt(delta[i])) / (2 * A[i])
+                angles[i] = 2 * atan(t) - (pi/2 + self._link_deviation)
+            except ValueError:
+                print('Pose not in range! Choose other Pose that is not a singularity')
+                return self.get_joints_poses()
+
+        return angles
+
```

### Comparing `robodyno-1.6.0/src/robodyno/robots/utils/transformations.py` & `robodyno-1.6.1b0/src/robodyno/robots/utils/transformations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1701 +1,1701 @@
-# -*- coding: utf-8 -*-
-# transformations.py
-
-# Copyright (c) 2006, Christoph Gohlke
-# Copyright (c) 2006-2009, The Regents of the University of California
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without
-# modification, are permitted provided that the following conditions are met:
-#
-# * Redistributions of source code must retain the above copyright
-#   notice, this list of conditions and the following disclaimer.
-# * Redistributions in binary form must reproduce the above copyright
-#   notice, this list of conditions and the following disclaimer in the
-#   documentation and/or other materials provided with the distribution.
-# * Neither the name of the copyright holders nor the names of any
-#   contributors may be used to endorse or promote products derived
-#   from this software without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-# ARE DISCLAIMED.  IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE
-# LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-# CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
-# SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-# INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-# ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-# POSSIBILITY OF SUCH DAMAGE.
-
-"""Homogeneous Transformation Matrices and Quaternions.
-
-A library for calculating 4x4 matrices for translating, rotating, reflecting,
-scaling, shearing, projecting, orthogonalizing, and superimposing arrays of
-3D homogeneous coordinates as well as for converting between rotation matrices,
-Euler angles, and quaternions. Also includes an Arcball control object and
-functions to decompose transformation matrices.
-
-:Authors:
-  `Christoph Gohlke <http://www.lfd.uci.edu/~gohlke/>`__,
-  Laboratory for Fluorescence Dynamics, University of California, Irvine
-
-:Version: 20090418
-
-Requirements
-------------
-
-* `Python 2.6 <http://www.python.org>`__
-* `Numpy 1.3 <http://numpy.scipy.org>`__
-* `transformations.c 20090418 <http://www.lfd.uci.edu/~gohlke/>`__
-  (optional implementation of some functions in C)
-
-Notes
------
-
-Matrices (M) can be inverted using numpy.linalg.inv(M), concatenated using
-numpy.dot(M0, M1), or used to transform homogeneous coordinates (v) using
-numpy.dot(M, v) for shape (4, \*) "point of arrays", respectively
-numpy.dot(v, M.T) for shape (\*, 4) "array of points".
-
-Calculations are carried out with numpy.float64 precision.
-
-This Python implementation is not optimized for speed.
-
-Vector, point, quaternion, and matrix function arguments are expected to be
-"array like", i.e. tuple, list, or numpy arrays.
-
-Return types are numpy arrays unless specified otherwise.
-
-Angles are in radians unless specified otherwise.
-
-Quaternions ix+jy+kz+w are represented as [x, y, z, w].
-
-Use the transpose of transformation matrices for OpenGL glMultMatrixd().
-
-A triple of Euler angles can be applied/interpreted in 24 ways, which can
-be specified using a 4 character string or encoded 4-tuple:
-
-  *Axes 4-string*: e.g. 'sxyz' or 'ryxy'
-
-  - first character : rotations are applied to 's'tatic or 'r'otating frame
-  - remaining characters : successive rotation axis 'x', 'y', or 'z'
-
-  *Axes 4-tuple*: e.g. (0, 0, 0, 0) or (1, 1, 1, 1)
-
-  - inner axis: code of axis ('x':0, 'y':1, 'z':2) of rightmost matrix.
-  - parity : even (0) if inner axis 'x' is followed by 'y', 'y' is followed
-    by 'z', or 'z' is followed by 'x'. Otherwise odd (1).
-  - repetition : first and last axis are same (1) or different (0).
-  - frame : rotations are applied to static (0) or rotating (1) frame.
-
-References
-----------
-
-(1)  Matrices and transformations. Ronald Goldman.
-     In "Graphics Gems I", pp 472-475. Morgan Kaufmann, 1990.
-(2)  More matrices and transformations: shear and pseudo-perspective.
-     Ronald Goldman. In "Graphics Gems II", pp 320-323. Morgan Kaufmann, 1991.
-(3)  Decomposing a matrix into simple transformations. Spencer Thomas.
-     In "Graphics Gems II", pp 320-323. Morgan Kaufmann, 1991.
-(4)  Recovering the data from the transformation matrix. Ronald Goldman.
-     In "Graphics Gems II", pp 324-331. Morgan Kaufmann, 1991.
-(5)  Euler angle conversion. Ken Shoemake.
-     In "Graphics Gems IV", pp 222-229. Morgan Kaufmann, 1994.
-(6)  Arcball rotation control. Ken Shoemake.
-     In "Graphics Gems IV", pp 175-192. Morgan Kaufmann, 1994.
-(7)  Representing attitude: Euler angles, unit quaternions, and rotation
-     vectors. James Diebel. 2006.
-(8)  A discussion of the solution for the best rotation to relate two sets
-     of vectors. W Kabsch. Acta Cryst. 1978. A34, 827-828.
-(9)  Closed-form solution of absolute orientation using unit quaternions.
-     BKP Horn. J Opt Soc Am A. 1987. 4(4), 629-642.
-(10) Quaternions. Ken Shoemake.
-     http://www.sfu.ca/~jwa3/cmpt461/files/quatut.pdf
-(11) From quaternion to matrix and back. JMP van Waveren. 2005.
-     http://www.intel.com/cd/ids/developer/asmo-na/eng/293748.htm
-(12) Uniform random rotations. Ken Shoemake.
-     In "Graphics Gems III", pp 124-132. Morgan Kaufmann, 1992.
-
-
-Examples
---------
-
->>> alpha, beta, gamma = 0.123, -1.234, 2.345
->>> origin, xaxis, yaxis, zaxis = (0, 0, 0), (1, 0, 0), (0, 1, 0), (0, 0, 1)
->>> I = identity_matrix()
->>> Rx = rotation_matrix(alpha, xaxis)
->>> Ry = rotation_matrix(beta, yaxis)
->>> Rz = rotation_matrix(gamma, zaxis)
->>> R = concatenate_matrices(Rx, Ry, Rz)
->>> euler = euler_from_matrix(R, 'rxyz')
->>> numpy.allclose([alpha, beta, gamma], euler)
-True
->>> Re = euler_matrix(alpha, beta, gamma, 'rxyz')
->>> is_same_transform(R, Re)
-True
->>> al, be, ga = euler_from_matrix(Re, 'rxyz')
->>> is_same_transform(Re, euler_matrix(al, be, ga, 'rxyz'))
-True
->>> qx = quaternion_about_axis(alpha, xaxis)
->>> qy = quaternion_about_axis(beta, yaxis)
->>> qz = quaternion_about_axis(gamma, zaxis)
->>> q = quaternion_multiply(qx, qy)
->>> q = quaternion_multiply(q, qz)
->>> Rq = quaternion_matrix(q)
->>> is_same_transform(R, Rq)
-True
->>> S = scale_matrix(1.23, origin)
->>> T = translation_matrix((1, 2, 3))
->>> Z = shear_matrix(beta, xaxis, origin, zaxis)
->>> R = random_rotation_matrix(numpy.random.rand(3))
->>> M = concatenate_matrices(T, R, Z, S)
->>> scale, shear, angles, trans, persp = decompose_matrix(M)
->>> numpy.allclose(scale, 1.23)
-True
->>> numpy.allclose(trans, (1, 2, 3))
-True
->>> numpy.allclose(shear, (0, math.tan(beta), 0))
-True
->>> is_same_transform(R, euler_matrix(axes='sxyz', *angles))
-True
->>> M1 = compose_matrix(scale, shear, angles, trans, persp)
->>> is_same_transform(M, M1)
-True
-
-"""
-
-from __future__ import division
-
-import warnings
-import math
-
-import numpy
-
-# Documentation in HTML format can be generated with Epydoc
-__docformat__ = "restructuredtext en"
-
-
-def identity_matrix():
-    """Return 4x4 identity/unit matrix.
-
-    >>> I = identity_matrix()
-    >>> numpy.allclose(I, numpy.dot(I, I))
-    True
-    >>> numpy.sum(I), numpy.trace(I)
-    (4.0, 4.0)
-    >>> numpy.allclose(I, numpy.identity(4, dtype=numpy.float64))
-    True
-
-    """
-    return numpy.identity(4, dtype=numpy.float64)
-
-def dh_matrix(alpha, a, d, theta, dh_mode = "SDH"):
-    """Return DH matrix by params.
-    
-    Args:
-        alpha,a,d,theta: DH parameters
-        dh_mode: "SDH" -> Standard DH
-                 "MDH" -> Modified DH
-    """
-    sinth = math.sin(theta)
-    costh = math.cos(theta)
-    sina = math.sin(alpha)
-    cosa = math.cos(alpha)
-    if (dh_mode == "SDH"):
-        M = numpy.array(((costh, -sinth * cosa,  sinth * sina, a * costh),
-                        (sinth,  costh * cosa, -costh * sina, a * sinth),
-                        (0.0  ,  sina        ,  cosa        , d        ),
-                        (0.0  ,  0.0         ,  0.0         , 1.0      )), dtype=numpy.float64)
-    if (dh_mode == "MDH"):
-        M = numpy.array(((costh       , -sinth      ,  0   ,  a       ),
-                        (sinth * cosa, costh * cosa, -sina, -sina * d),
-                        (sinth * sina, costh * sina,  cosa,  cosa * d),
-                        (0.0         , 0.0,           0.0,   1.0     )), dtype=numpy.float64)
-    return M
-
-def translation_matrix(direction):
-    """Return matrix to translate by direction vector.
-
-    >>> v = numpy.random.random(3) - 0.5
-    >>> numpy.allclose(v, translation_matrix(v)[:3, 3])
-    True
-
-    """
-    M = numpy.identity(4)
-    M[:3, 3] = direction[:3]
-    return M
-
-
-def translation_from_matrix(matrix):
-    """Return translation vector from translation matrix.
-
-    >>> v0 = numpy.random.random(3) - 0.5
-    >>> v1 = translation_from_matrix(translation_matrix(v0))
-    >>> numpy.allclose(v0, v1)
-    True
-
-    """
-    return numpy.array(matrix, copy=False)[:3, 3].copy()
-
-
-def reflection_matrix(point, normal):
-    """Return matrix to mirror at plane defined by point and normal vector.
-
-    >>> v0 = numpy.random.random(4) - 0.5
-    >>> v0[3] = 1.0
-    >>> v1 = numpy.random.random(3) - 0.5
-    >>> R = reflection_matrix(v0, v1)
-    >>> numpy.allclose(2., numpy.trace(R))
-    True
-    >>> numpy.allclose(v0, numpy.dot(R, v0))
-    True
-    >>> v2 = v0.copy()
-    >>> v2[:3] += v1
-    >>> v3 = v0.copy()
-    >>> v2[:3] -= v1
-    >>> numpy.allclose(v2, numpy.dot(R, v3))
-    True
-
-    """
-    normal = unit_vector(normal[:3])
-    M = numpy.identity(4)
-    M[:3, :3] -= 2.0 * numpy.outer(normal, normal)
-    M[:3, 3] = (2.0 * numpy.dot(point[:3], normal)) * normal
-    return M
-
-
-def reflection_from_matrix(matrix):
-    """Return mirror plane point and normal vector from reflection matrix.
-
-    >>> v0 = numpy.random.random(3) - 0.5
-    >>> v1 = numpy.random.random(3) - 0.5
-    >>> M0 = reflection_matrix(v0, v1)
-    >>> point, normal = reflection_from_matrix(M0)
-    >>> M1 = reflection_matrix(point, normal)
-    >>> is_same_transform(M0, M1)
-    True
-
-    """
-    M = numpy.array(matrix, dtype=numpy.float64, copy=False)
-    # normal: unit eigenvector corresponding to eigenvalue -1
-    l, V = numpy.linalg.eig(M[:3, :3])
-    i = numpy.where(abs(numpy.real(l) + 1.0) < 1e-8)[0]
-    if not len(i):
-        raise ValueError("no unit eigenvector corresponding to eigenvalue -1")
-    normal = numpy.real(V[:, i[0]]).squeeze()
-    # point: any unit eigenvector corresponding to eigenvalue 1
-    l, V = numpy.linalg.eig(M)
-    i = numpy.where(abs(numpy.real(l) - 1.0) < 1e-8)[0]
-    if not len(i):
-        raise ValueError("no unit eigenvector corresponding to eigenvalue 1")
-    point = numpy.real(V[:, i[-1]]).squeeze()
-    point /= point[3]
-    return point, normal
-
-
-def rotation_matrix(angle, direction, point=None):
-    """Return matrix to rotate about axis defined by point and direction.
-
-    >>> angle = (random.random() - 0.5) * (2*math.pi)
-    >>> direc = numpy.random.random(3) - 0.5
-    >>> point = numpy.random.random(3) - 0.5
-    >>> R0 = rotation_matrix(angle, direc, point)
-    >>> R1 = rotation_matrix(angle-2*math.pi, direc, point)
-    >>> is_same_transform(R0, R1)
-    True
-    >>> R0 = rotation_matrix(angle, direc, point)
-    >>> R1 = rotation_matrix(-angle, -direc, point)
-    >>> is_same_transform(R0, R1)
-    True
-    >>> I = numpy.identity(4, numpy.float64)
-    >>> numpy.allclose(I, rotation_matrix(math.pi*2, direc))
-    True
-    >>> numpy.allclose(2., numpy.trace(rotation_matrix(math.pi/2,
-    ...                                                direc, point)))
-    True
-
-    """
-    sina = math.sin(angle)
-    cosa = math.cos(angle)
-    direction = unit_vector(direction[:3])
-    # rotation matrix around unit vector
-    R = numpy.array(((cosa, 0.0,  0.0),
-                     (0.0,  cosa, 0.0),
-                     (0.0,  0.0,  cosa)), dtype=numpy.float64)
-    R += numpy.outer(direction, direction) * (1.0 - cosa)
-    direction *= sina
-    R += numpy.array((( 0.0,         -direction[2],  direction[1]),
-                      ( direction[2], 0.0,          -direction[0]),
-                      (-direction[1], direction[0],  0.0)),
-                     dtype=numpy.float64)
-    M = numpy.identity(4)
-    M[:3, :3] = R
-    if point is not None:
-        # rotation not around origin
-        point = numpy.array(point[:3], dtype=numpy.float64, copy=False)
-        M[:3, 3] = point - numpy.dot(R, point)
-    return M
-
-
-def rotation_from_matrix(matrix):
-    """Return rotation angle and axis from rotation matrix.
-
-    >>> angle = (random.random() - 0.5) * (2*math.pi)
-    >>> direc = numpy.random.random(3) - 0.5
-    >>> point = numpy.random.random(3) - 0.5
-    >>> R0 = rotation_matrix(angle, direc, point)
-    >>> angle, direc, point = rotation_from_matrix(R0)
-    >>> R1 = rotation_matrix(angle, direc, point)
-    >>> is_same_transform(R0, R1)
-    True
-
-    """
-    R = numpy.array(matrix, dtype=numpy.float64, copy=False)
-    R33 = R[:3, :3]
-    # direction: unit eigenvector of R33 corresponding to eigenvalue of 1
-    l, W = numpy.linalg.eig(R33.T)
-    i = numpy.where(abs(numpy.real(l) - 1.0) < 1e-8)[0]
-    if not len(i):
-        raise ValueError("no unit eigenvector corresponding to eigenvalue 1")
-    direction = numpy.real(W[:, i[-1]]).squeeze()
-    # point: unit eigenvector of R33 corresponding to eigenvalue of 1
-    l, Q = numpy.linalg.eig(R)
-    i = numpy.where(abs(numpy.real(l) - 1.0) < 1e-8)[0]
-    if not len(i):
-        raise ValueError("no unit eigenvector corresponding to eigenvalue 1")
-    point = numpy.real(Q[:, i[-1]]).squeeze()
-    point /= point[3]
-    # rotation angle depending on direction
-    cosa = (numpy.trace(R33) - 1.0) / 2.0
-    if abs(direction[2]) > 1e-8:
-        sina = (R[1, 0] + (cosa-1.0)*direction[0]*direction[1]) / direction[2]
-    elif abs(direction[1]) > 1e-8:
-        sina = (R[0, 2] + (cosa-1.0)*direction[0]*direction[2]) / direction[1]
-    else:
-        sina = (R[2, 1] + (cosa-1.0)*direction[1]*direction[2]) / direction[0]
-    angle = math.atan2(sina, cosa)
-    return angle, direction, point
-
-
-def scale_matrix(factor, origin=None, direction=None):
-    """Return matrix to scale by factor around origin in direction.
-
-    Use factor -1 for point symmetry.
-
-    >>> v = (numpy.random.rand(4, 5) - 0.5) * 20.0
-    >>> v[3] = 1.0
-    >>> S = scale_matrix(-1.234)
-    >>> numpy.allclose(numpy.dot(S, v)[:3], -1.234*v[:3])
-    True
-    >>> factor = random.random() * 10 - 5
-    >>> origin = numpy.random.random(3) - 0.5
-    >>> direct = numpy.random.random(3) - 0.5
-    >>> S = scale_matrix(factor, origin)
-    >>> S = scale_matrix(factor, origin, direct)
-
-    """
-    if direction is None:
-        # uniform scaling
-        M = numpy.array(((factor, 0.0,    0.0,    0.0),
-                         (0.0,    factor, 0.0,    0.0),
-                         (0.0,    0.0,    factor, 0.0),
-                         (0.0,    0.0,    0.0,    1.0)), dtype=numpy.float64)
-        if origin is not None:
-            M[:3, 3] = origin[:3]
-            M[:3, 3] *= 1.0 - factor
-    else:
-        # nonuniform scaling
-        direction = unit_vector(direction[:3])
-        factor = 1.0 - factor
-        M = numpy.identity(4)
-        M[:3, :3] -= factor * numpy.outer(direction, direction)
-        if origin is not None:
-            M[:3, 3] = (factor * numpy.dot(origin[:3], direction)) * direction
-    return M
-
-
-def scale_from_matrix(matrix):
-    """Return scaling factor, origin and direction from scaling matrix.
-
-    >>> factor = random.random() * 10 - 5
-    >>> origin = numpy.random.random(3) - 0.5
-    >>> direct = numpy.random.random(3) - 0.5
-    >>> S0 = scale_matrix(factor, origin)
-    >>> factor, origin, direction = scale_from_matrix(S0)
-    >>> S1 = scale_matrix(factor, origin, direction)
-    >>> is_same_transform(S0, S1)
-    True
-    >>> S0 = scale_matrix(factor, origin, direct)
-    >>> factor, origin, direction = scale_from_matrix(S0)
-    >>> S1 = scale_matrix(factor, origin, direction)
-    >>> is_same_transform(S0, S1)
-    True
-
-    """
-    M = numpy.array(matrix, dtype=numpy.float64, copy=False)
-    M33 = M[:3, :3]
-    factor = numpy.trace(M33) - 2.0
-    try:
-        # direction: unit eigenvector corresponding to eigenvalue factor
-        l, V = numpy.linalg.eig(M33)
-        i = numpy.where(abs(numpy.real(l) - factor) < 1e-8)[0][0]
-        direction = numpy.real(V[:, i]).squeeze()
-        direction /= vector_norm(direction)
-    except IndexError:
-        # uniform scaling
-        factor = (factor + 2.0) / 3.0
-        direction = None
-    # origin: any eigenvector corresponding to eigenvalue 1
-    l, V = numpy.linalg.eig(M)
-    i = numpy.where(abs(numpy.real(l) - 1.0) < 1e-8)[0]
-    if not len(i):
-        raise ValueError("no eigenvector corresponding to eigenvalue 1")
-    origin = numpy.real(V[:, i[-1]]).squeeze()
-    origin /= origin[3]
-    return factor, origin, direction
-
-
-def projection_matrix(point, normal, direction=None,
-                      perspective=None, pseudo=False):
-    """Return matrix to project onto plane defined by point and normal.
-
-    Using either perspective point, projection direction, or none of both.
-
-    If pseudo is True, perspective projections will preserve relative depth
-    such that Perspective = dot(Orthogonal, PseudoPerspective).
-
-    >>> P = projection_matrix((0, 0, 0), (1, 0, 0))
-    >>> numpy.allclose(P[1:, 1:], numpy.identity(4)[1:, 1:])
-    True
-    >>> point = numpy.random.random(3) - 0.5
-    >>> normal = numpy.random.random(3) - 0.5
-    >>> direct = numpy.random.random(3) - 0.5
-    >>> persp = numpy.random.random(3) - 0.5
-    >>> P0 = projection_matrix(point, normal)
-    >>> P1 = projection_matrix(point, normal, direction=direct)
-    >>> P2 = projection_matrix(point, normal, perspective=persp)
-    >>> P3 = projection_matrix(point, normal, perspective=persp, pseudo=True)
-    >>> is_same_transform(P2, numpy.dot(P0, P3))
-    True
-    >>> P = projection_matrix((3, 0, 0), (1, 1, 0), (1, 0, 0))
-    >>> v0 = (numpy.random.rand(4, 5) - 0.5) * 20.0
-    >>> v0[3] = 1.0
-    >>> v1 = numpy.dot(P, v0)
-    >>> numpy.allclose(v1[1], v0[1])
-    True
-    >>> numpy.allclose(v1[0], 3.0-v1[1])
-    True
-
-    """
-    M = numpy.identity(4)
-    point = numpy.array(point[:3], dtype=numpy.float64, copy=False)
-    normal = unit_vector(normal[:3])
-    if perspective is not None:
-        # perspective projection
-        perspective = numpy.array(perspective[:3], dtype=numpy.float64,
-                                  copy=False)
-        M[0, 0] = M[1, 1] = M[2, 2] = numpy.dot(perspective-point, normal)
-        M[:3, :3] -= numpy.outer(perspective, normal)
-        if pseudo:
-            # preserve relative depth
-            M[:3, :3] -= numpy.outer(normal, normal)
-            M[:3, 3] = numpy.dot(point, normal) * (perspective+normal)
-        else:
-            M[:3, 3] = numpy.dot(point, normal) * perspective
-        M[3, :3] = -normal
-        M[3, 3] = numpy.dot(perspective, normal)
-    elif direction is not None:
-        # parallel projection
-        direction = numpy.array(direction[:3], dtype=numpy.float64, copy=False)
-        scale = numpy.dot(direction, normal)
-        M[:3, :3] -= numpy.outer(direction, normal) / scale
-        M[:3, 3] = direction * (numpy.dot(point, normal) / scale)
-    else:
-        # orthogonal projection
-        M[:3, :3] -= numpy.outer(normal, normal)
-        M[:3, 3] = numpy.dot(point, normal) * normal
-    return M
-
-
-def projection_from_matrix(matrix, pseudo=False):
-    """Return projection plane and perspective point from projection matrix.
-
-    Return values are same as arguments for projection_matrix function:
-    point, normal, direction, perspective, and pseudo.
-
-    >>> point = numpy.random.random(3) - 0.5
-    >>> normal = numpy.random.random(3) - 0.5
-    >>> direct = numpy.random.random(3) - 0.5
-    >>> persp = numpy.random.random(3) - 0.5
-    >>> P0 = projection_matrix(point, normal)
-    >>> result = projection_from_matrix(P0)
-    >>> P1 = projection_matrix(*result)
-    >>> is_same_transform(P0, P1)
-    True
-    >>> P0 = projection_matrix(point, normal, direct)
-    >>> result = projection_from_matrix(P0)
-    >>> P1 = projection_matrix(*result)
-    >>> is_same_transform(P0, P1)
-    True
-    >>> P0 = projection_matrix(point, normal, perspective=persp, pseudo=False)
-    >>> result = projection_from_matrix(P0, pseudo=False)
-    >>> P1 = projection_matrix(*result)
-    >>> is_same_transform(P0, P1)
-    True
-    >>> P0 = projection_matrix(point, normal, perspective=persp, pseudo=True)
-    >>> result = projection_from_matrix(P0, pseudo=True)
-    >>> P1 = projection_matrix(*result)
-    >>> is_same_transform(P0, P1)
-    True
-
-    """
-    M = numpy.array(matrix, dtype=numpy.float64, copy=False)
-    M33 = M[:3, :3]
-    l, V = numpy.linalg.eig(M)
-    i = numpy.where(abs(numpy.real(l) - 1.0) < 1e-8)[0]
-    if not pseudo and len(i):
-        # point: any eigenvector corresponding to eigenvalue 1
-        point = numpy.real(V[:, i[-1]]).squeeze()
-        point /= point[3]
-        # direction: unit eigenvector corresponding to eigenvalue 0
-        l, V = numpy.linalg.eig(M33)
-        i = numpy.where(abs(numpy.real(l)) < 1e-8)[0]
-        if not len(i):
-            raise ValueError("no eigenvector corresponding to eigenvalue 0")
-        direction = numpy.real(V[:, i[0]]).squeeze()
-        direction /= vector_norm(direction)
-        # normal: unit eigenvector of M33.T corresponding to eigenvalue 0
-        l, V = numpy.linalg.eig(M33.T)
-        i = numpy.where(abs(numpy.real(l)) < 1e-8)[0]
-        if len(i):
-            # parallel projection
-            normal = numpy.real(V[:, i[0]]).squeeze()
-            normal /= vector_norm(normal)
-            return point, normal, direction, None, False
-        else:
-            # orthogonal projection, where normal equals direction vector
-            return point, direction, None, None, False
-    else:
-        # perspective projection
-        i = numpy.where(abs(numpy.real(l)) > 1e-8)[0]
-        if not len(i):
-            raise ValueError(
-                "no eigenvector not corresponding to eigenvalue 0")
-        point = numpy.real(V[:, i[-1]]).squeeze()
-        point /= point[3]
-        normal = - M[3, :3]
-        perspective = M[:3, 3] / numpy.dot(point[:3], normal)
-        if pseudo:
-            perspective -= normal
-        return point, normal, None, perspective, pseudo
-
-
-def clip_matrix(left, right, bottom, top, near, far, perspective=False):
-    """Return matrix to obtain normalized device coordinates from frustrum.
-
-    The frustrum bounds are axis-aligned along x (left, right),
-    y (bottom, top) and z (near, far).
-
-    Normalized device coordinates are in range [-1, 1] if coordinates are
-    inside the frustrum.
-
-    If perspective is True the frustrum is a truncated pyramid with the
-    perspective point at origin and direction along z axis, otherwise an
-    orthographic canonical view volume (a box).
-
-    Homogeneous coordinates transformed by the perspective clip matrix
-    need to be dehomogenized (devided by w coordinate).
-
-    >>> frustrum = numpy.random.rand(6)
-    >>> frustrum[1] += frustrum[0]
-    >>> frustrum[3] += frustrum[2]
-    >>> frustrum[5] += frustrum[4]
-    >>> M = clip_matrix(*frustrum, perspective=False)
-    >>> numpy.dot(M, [frustrum[0], frustrum[2], frustrum[4], 1.0])
-    array([-1., -1., -1.,  1.])
-    >>> numpy.dot(M, [frustrum[1], frustrum[3], frustrum[5], 1.0])
-    array([ 1.,  1.,  1.,  1.])
-    >>> M = clip_matrix(*frustrum, perspective=True)
-    >>> v = numpy.dot(M, [frustrum[0], frustrum[2], frustrum[4], 1.0])
-    >>> v / v[3]
-    array([-1., -1., -1.,  1.])
-    >>> v = numpy.dot(M, [frustrum[1], frustrum[3], frustrum[4], 1.0])
-    >>> v / v[3]
-    array([ 1.,  1., -1.,  1.])
-
-    """
-    if left >= right or bottom >= top or near >= far:
-        raise ValueError("invalid frustrum")
-    if perspective:
-        if near <= _EPS:
-            raise ValueError("invalid frustrum: near <= 0")
-        t = 2.0 * near
-        M = ((-t/(right-left), 0.0, (right+left)/(right-left), 0.0),
-             (0.0, -t/(top-bottom), (top+bottom)/(top-bottom), 0.0),
-             (0.0, 0.0, -(far+near)/(far-near), t*far/(far-near)),
-             (0.0, 0.0, -1.0, 0.0))
-    else:
-        M = ((2.0/(right-left), 0.0, 0.0, (right+left)/(left-right)),
-             (0.0, 2.0/(top-bottom), 0.0, (top+bottom)/(bottom-top)),
-             (0.0, 0.0, 2.0/(far-near), (far+near)/(near-far)),
-             (0.0, 0.0, 0.0, 1.0))
-    return numpy.array(M, dtype=numpy.float64)
-
-
-def shear_matrix(angle, direction, point, normal):
-    """Return matrix to shear by angle along direction vector on shear plane.
-
-    The shear plane is defined by a point and normal vector. The direction
-    vector must be orthogonal to the plane's normal vector.
-
-    A point P is transformed by the shear matrix into P" such that
-    the vector P-P" is parallel to the direction vector and its extent is
-    given by the angle of P-P'-P", where P' is the orthogonal projection
-    of P onto the shear plane.
-
-    >>> angle = (random.random() - 0.5) * 4*math.pi
-    >>> direct = numpy.random.random(3) - 0.5
-    >>> point = numpy.random.random(3) - 0.5
-    >>> normal = numpy.cross(direct, numpy.random.random(3))
-    >>> S = shear_matrix(angle, direct, point, normal)
-    >>> numpy.allclose(1.0, numpy.linalg.det(S))
-    True
-
-    """
-    normal = unit_vector(normal[:3])
-    direction = unit_vector(direction[:3])
-    if abs(numpy.dot(normal, direction)) > 1e-6:
-        raise ValueError("direction and normal vectors are not orthogonal")
-    angle = math.tan(angle)
-    M = numpy.identity(4)
-    M[:3, :3] += angle * numpy.outer(direction, normal)
-    M[:3, 3] = -angle * numpy.dot(point[:3], normal) * direction
-    return M
-
-
-def shear_from_matrix(matrix):
-    """Return shear angle, direction and plane from shear matrix.
-
-    >>> angle = (random.random() - 0.5) * 4*math.pi
-    >>> direct = numpy.random.random(3) - 0.5
-    >>> point = numpy.random.random(3) - 0.5
-    >>> normal = numpy.cross(direct, numpy.random.random(3))
-    >>> S0 = shear_matrix(angle, direct, point, normal)
-    >>> angle, direct, point, normal = shear_from_matrix(S0)
-    >>> S1 = shear_matrix(angle, direct, point, normal)
-    >>> is_same_transform(S0, S1)
-    True
-
-    """
-    M = numpy.array(matrix, dtype=numpy.float64, copy=False)
-    M33 = M[:3, :3]
-    # normal: cross independent eigenvectors corresponding to the eigenvalue 1
-    l, V = numpy.linalg.eig(M33)
-    i = numpy.where(abs(numpy.real(l) - 1.0) < 1e-4)[0]
-    if len(i) < 2:
-        raise ValueError("No two linear independent eigenvectors found %s" % l)
-    V = numpy.real(V[:, i]).squeeze().T
-    lenorm = -1.0
-    for i0, i1 in ((0, 1), (0, 2), (1, 2)):
-        n = numpy.cross(V[i0], V[i1])
-        l = vector_norm(n)
-        if l > lenorm:
-            lenorm = l
-            normal = n
-    normal /= lenorm
-    # direction and angle
-    direction = numpy.dot(M33 - numpy.identity(3), normal)
-    angle = vector_norm(direction)
-    direction /= angle
-    angle = math.atan(angle)
-    # point: eigenvector corresponding to eigenvalue 1
-    l, V = numpy.linalg.eig(M)
-    i = numpy.where(abs(numpy.real(l) - 1.0) < 1e-8)[0]
-    if not len(i):
-        raise ValueError("no eigenvector corresponding to eigenvalue 1")
-    point = numpy.real(V[:, i[-1]]).squeeze()
-    point /= point[3]
-    return angle, direction, point, normal
-
-
-def decompose_matrix(matrix):
-    """Return sequence of transformations from transformation matrix.
-
-    matrix : array_like
-        Non-degenerative homogeneous transformation matrix
-
-    Return tuple of:
-        scale : vector of 3 scaling factors
-        shear : list of shear factors for x-y, x-z, y-z axes
-        angles : list of Euler angles about static x, y, z axes
-        translate : translation vector along x, y, z axes
-        perspective : perspective partition of matrix
-
-    Raise ValueError if matrix is of wrong type or degenerative.
-
-    >>> T0 = translation_matrix((1, 2, 3))
-    >>> scale, shear, angles, trans, persp = decompose_matrix(T0)
-    >>> T1 = translation_matrix(trans)
-    >>> numpy.allclose(T0, T1)
-    True
-    >>> S = scale_matrix(0.123)
-    >>> scale, shear, angles, trans, persp = decompose_matrix(S)
-    >>> scale[0]
-    0.123
-    >>> R0 = euler_matrix(1, 2, 3)
-    >>> scale, shear, angles, trans, persp = decompose_matrix(R0)
-    >>> R1 = euler_matrix(*angles)
-    >>> numpy.allclose(R0, R1)
-    True
-
-    """
-    M = numpy.array(matrix, dtype=numpy.float64, copy=True).T
-    if abs(M[3, 3]) < _EPS:
-        raise ValueError("M[3, 3] is zero")
-    M /= M[3, 3]
-    P = M.copy()
-    P[:, 3] = 0, 0, 0, 1
-    if not numpy.linalg.det(P):
-        raise ValueError("Matrix is singular")
-
-    scale = numpy.zeros((3, ), dtype=numpy.float64)
-    shear = [0, 0, 0]
-    angles = [0, 0, 0]
-
-    if any(abs(M[:3, 3]) > _EPS):
-        perspective = numpy.dot(M[:, 3], numpy.linalg.inv(P.T))
-        M[:, 3] = 0, 0, 0, 1
-    else:
-        perspective = numpy.array((0, 0, 0, 1), dtype=numpy.float64)
-
-    translate = M[3, :3].copy()
-    M[3, :3] = 0
-
-    row = M[:3, :3].copy()
-    scale[0] = vector_norm(row[0])
-    row[0] /= scale[0]
-    shear[0] = numpy.dot(row[0], row[1])
-    row[1] -= row[0] * shear[0]
-    scale[1] = vector_norm(row[1])
-    row[1] /= scale[1]
-    shear[0] /= scale[1]
-    shear[1] = numpy.dot(row[0], row[2])
-    row[2] -= row[0] * shear[1]
-    shear[2] = numpy.dot(row[1], row[2])
-    row[2] -= row[1] * shear[2]
-    scale[2] = vector_norm(row[2])
-    row[2] /= scale[2]
-    shear[1:] /= scale[2]
-
-    if numpy.dot(row[0], numpy.cross(row[1], row[2])) < 0:
-        scale *= -1
-        row *= -1
-
-    angles[1] = math.asin(-row[0, 2])
-    if math.cos(angles[1]):
-        angles[0] = math.atan2(row[1, 2], row[2, 2])
-        angles[2] = math.atan2(row[0, 1], row[0, 0])
-    else:
-        #angles[0] = math.atan2(row[1, 0], row[1, 1])
-        angles[0] = math.atan2(-row[2, 1], row[1, 1])
-        angles[2] = 0.0
-
-    return scale, shear, angles, translate, perspective
-
-
-def compose_matrix(scale=None, shear=None, angles=None, translate=None,
-                   perspective=None):
-    """Return transformation matrix from sequence of transformations.
-
-    This is the inverse of the decompose_matrix function.
-
-    Sequence of transformations:
-        scale : vector of 3 scaling factors
-        shear : list of shear factors for x-y, x-z, y-z axes
-        angles : list of Euler angles about static x, y, z axes
-        translate : translation vector along x, y, z axes
-        perspective : perspective partition of matrix
-
-    >>> scale = numpy.random.random(3) - 0.5
-    >>> shear = numpy.random.random(3) - 0.5
-    >>> angles = (numpy.random.random(3) - 0.5) * (2*math.pi)
-    >>> trans = numpy.random.random(3) - 0.5
-    >>> persp = numpy.random.random(4) - 0.5
-    >>> M0 = compose_matrix(scale, shear, angles, trans, persp)
-    >>> result = decompose_matrix(M0)
-    >>> M1 = compose_matrix(*result)
-    >>> is_same_transform(M0, M1)
-    True
-
-    """
-    M = numpy.identity(4)
-    if perspective is not None:
-        P = numpy.identity(4)
-        P[3, :] = perspective[:4]
-        M = numpy.dot(M, P)
-    if translate is not None:
-        T = numpy.identity(4)
-        T[:3, 3] = translate[:3]
-        M = numpy.dot(M, T)
-    if angles is not None:
-        R = euler_matrix(angles[0], angles[1], angles[2], 'sxyz')
-        M = numpy.dot(M, R)
-    if shear is not None:
-        Z = numpy.identity(4)
-        Z[1, 2] = shear[2]
-        Z[0, 2] = shear[1]
-        Z[0, 1] = shear[0]
-        M = numpy.dot(M, Z)
-    if scale is not None:
-        S = numpy.identity(4)
-        S[0, 0] = scale[0]
-        S[1, 1] = scale[1]
-        S[2, 2] = scale[2]
-        M = numpy.dot(M, S)
-    M /= M[3, 3]
-    return M
-
-
-def orthogonalization_matrix(lengths, angles):
-    """Return orthogonalization matrix for crystallographic cell coordinates.
-
-    Angles are expected in degrees.
-
-    The de-orthogonalization matrix is the inverse.
-
-    >>> O = orthogonalization_matrix((10., 10., 10.), (90., 90., 90.))
-    >>> numpy.allclose(O[:3, :3], numpy.identity(3, float) * 10)
-    True
-    >>> O = orthogonalization_matrix([9.8, 12.0, 15.5], [87.2, 80.7, 69.7])
-    >>> numpy.allclose(numpy.sum(O), 43.063229)
-    True
-
-    """
-    a, b, c = lengths
-    angles = numpy.radians(angles)
-    sina, sinb, _ = numpy.sin(angles)
-    cosa, cosb, cosg = numpy.cos(angles)
-    co = (cosa * cosb - cosg) / (sina * sinb)
-    return numpy.array((
-        ( a*sinb*math.sqrt(1.0-co*co),  0.0,    0.0, 0.0),
-        (-a*sinb*co,                    b*sina, 0.0, 0.0),
-        ( a*cosb,                       b*cosa, c,   0.0),
-        ( 0.0,                          0.0,    0.0, 1.0)),
-        dtype=numpy.float64)
-
-
-def superimposition_matrix(v0, v1, scaling=False, usesvd=True):
-    """Return matrix to transform given vector set into second vector set.
-
-    v0 and v1 are shape (3, \*) or (4, \*) arrays of at least 3 vectors.
-
-    If usesvd is True, the weighted sum of squared deviations (RMSD) is
-    minimized according to the algorithm by W. Kabsch [8]. Otherwise the
-    quaternion based algorithm by B. Horn [9] is used (slower when using
-    this Python implementation).
-
-    The returned matrix performs rotation, translation and uniform scaling
-    (if specified).
-
-    >>> v0 = numpy.random.rand(3, 10)
-    >>> M = superimposition_matrix(v0, v0)
-    >>> numpy.allclose(M, numpy.identity(4))
-    True
-    >>> R = random_rotation_matrix(numpy.random.random(3))
-    >>> v0 = ((1,0,0), (0,1,0), (0,0,1), (1,1,1))
-    >>> v1 = numpy.dot(R, v0)
-    >>> M = superimposition_matrix(v0, v1)
-    >>> numpy.allclose(v1, numpy.dot(M, v0))
-    True
-    >>> v0 = (numpy.random.rand(4, 100) - 0.5) * 20.0
-    >>> v0[3] = 1.0
-    >>> v1 = numpy.dot(R, v0)
-    >>> M = superimposition_matrix(v0, v1)
-    >>> numpy.allclose(v1, numpy.dot(M, v0))
-    True
-    >>> S = scale_matrix(random.random())
-    >>> T = translation_matrix(numpy.random.random(3)-0.5)
-    >>> M = concatenate_matrices(T, R, S)
-    >>> v1 = numpy.dot(M, v0)
-    >>> v0[:3] += numpy.random.normal(0.0, 1e-9, 300).reshape(3, -1)
-    >>> M = superimposition_matrix(v0, v1, scaling=True)
-    >>> numpy.allclose(v1, numpy.dot(M, v0))
-    True
-    >>> M = superimposition_matrix(v0, v1, scaling=True, usesvd=False)
-    >>> numpy.allclose(v1, numpy.dot(M, v0))
-    True
-    >>> v = numpy.empty((4, 100, 3), dtype=numpy.float64)
-    >>> v[:, :, 0] = v0
-    >>> M = superimposition_matrix(v0, v1, scaling=True, usesvd=False)
-    >>> numpy.allclose(v1, numpy.dot(M, v[:, :, 0]))
-    True
-
-    """
-    v0 = numpy.array(v0, dtype=numpy.float64, copy=False)[:3]
-    v1 = numpy.array(v1, dtype=numpy.float64, copy=False)[:3]
-
-    if v0.shape != v1.shape or v0.shape[1] < 3:
-        raise ValueError("Vector sets are of wrong shape or type.")
-
-    # move centroids to origin
-    t0 = numpy.mean(v0, axis=1)
-    t1 = numpy.mean(v1, axis=1)
-    v0 = v0 - t0.reshape(3, 1)
-    v1 = v1 - t1.reshape(3, 1)
-
-    if usesvd:
-        # Singular Value Decomposition of covariance matrix
-        u, s, vh = numpy.linalg.svd(numpy.dot(v1, v0.T))
-        # rotation matrix from SVD orthonormal bases
-        R = numpy.dot(u, vh)
-        if numpy.linalg.det(R) < 0.0:
-            # R does not constitute right handed system
-            R -= numpy.outer(u[:, 2], vh[2, :]*2.0)
-            s[-1] *= -1.0
-        # homogeneous transformation matrix
-        M = numpy.identity(4)
-        M[:3, :3] = R
-    else:
-        # compute symmetric matrix N
-        xx, yy, zz = numpy.sum(v0 * v1, axis=1)
-        xy, yz, zx = numpy.sum(v0 * numpy.roll(v1, -1, axis=0), axis=1)
-        xz, yx, zy = numpy.sum(v0 * numpy.roll(v1, -2, axis=0), axis=1)
-        N = ((xx+yy+zz, yz-zy,    zx-xz,    xy-yx),
-             (yz-zy,    xx-yy-zz, xy+yx,    zx+xz),
-             (zx-xz,    xy+yx,   -xx+yy-zz, yz+zy),
-             (xy-yx,    zx+xz,    yz+zy,   -xx-yy+zz))
-        # quaternion: eigenvector corresponding to most positive eigenvalue
-        l, V = numpy.linalg.eig(N)
-        q = V[:, numpy.argmax(l)]
-        q /= vector_norm(q) # unit quaternion
-        q = numpy.roll(q, -1) # move w component to end
-        # homogeneous transformation matrix
-        M = quaternion_matrix(q)
-
-    # scale: ratio of rms deviations from centroid
-    if scaling:
-        v0 *= v0
-        v1 *= v1
-        M[:3, :3] *= math.sqrt(numpy.sum(v1) / numpy.sum(v0))
-
-    # translation
-    M[:3, 3] = t1
-    T = numpy.identity(4)
-    T[:3, 3] = -t0
-    M = numpy.dot(M, T)
-    return M
-
-
-def euler_matrix(ai, aj, ak, axes='sxyz'):
-    """Return homogeneous rotation matrix from Euler angles and axis sequence.
-
-    ai, aj, ak : Euler's roll, pitch and yaw angles
-    axes : One of 24 axis sequences as string or encoded tuple
-
-    >>> R = euler_matrix(1, 2, 3, 'syxz')
-    >>> numpy.allclose(numpy.sum(R[0]), -1.34786452)
-    True
-    >>> R = euler_matrix(1, 2, 3, (0, 1, 0, 1))
-    >>> numpy.allclose(numpy.sum(R[0]), -0.383436184)
-    True
-    >>> ai, aj, ak = (4.0*math.pi) * (numpy.random.random(3) - 0.5)
-    >>> for axes in _AXES2TUPLE.keys():
-    ...    R = euler_matrix(ai, aj, ak, axes)
-    >>> for axes in _TUPLE2AXES.keys():
-    ...    R = euler_matrix(ai, aj, ak, axes)
-
-    """
-    try:
-        firstaxis, parity, repetition, frame = _AXES2TUPLE[axes]
-    except (AttributeError, KeyError):
-        _ = _TUPLE2AXES[axes]
-        firstaxis, parity, repetition, frame = axes
-
-    i = firstaxis
-    j = _NEXT_AXIS[i+parity]
-    k = _NEXT_AXIS[i-parity+1]
-
-    if frame:
-        ai, ak = ak, ai
-    if parity:
-        ai, aj, ak = -ai, -aj, -ak
-
-    si, sj, sk = math.sin(ai), math.sin(aj), math.sin(ak)
-    ci, cj, ck = math.cos(ai), math.cos(aj), math.cos(ak)
-    cc, cs = ci*ck, ci*sk
-    sc, ss = si*ck, si*sk
-
-    M = numpy.identity(4)
-    if repetition:
-        M[i, i] = cj
-        M[i, j] = sj*si
-        M[i, k] = sj*ci
-        M[j, i] = sj*sk
-        M[j, j] = -cj*ss+cc
-        M[j, k] = -cj*cs-sc
-        M[k, i] = -sj*ck
-        M[k, j] = cj*sc+cs
-        M[k, k] = cj*cc-ss
-    else:
-        M[i, i] = cj*ck
-        M[i, j] = sj*sc-cs
-        M[i, k] = sj*cc+ss
-        M[j, i] = cj*sk
-        M[j, j] = sj*ss+cc
-        M[j, k] = sj*cs-sc
-        M[k, i] = -sj
-        M[k, j] = cj*si
-        M[k, k] = cj*ci
-    return M
-
-
-def euler_from_matrix(matrix, axes='sxyz'):
-    """Return Euler angles from rotation matrix for specified axis sequence.
-
-    axes : One of 24 axis sequences as string or encoded tuple
-
-    Note that many Euler angle triplets can describe one matrix.
-
-    >>> R0 = euler_matrix(1, 2, 3, 'syxz')
-    >>> al, be, ga = euler_from_matrix(R0, 'syxz')
-    >>> R1 = euler_matrix(al, be, ga, 'syxz')
-    >>> numpy.allclose(R0, R1)
-    True
-    >>> angles = (4.0*math.pi) * (numpy.random.random(3) - 0.5)
-    >>> for axes in _AXES2TUPLE.keys():
-    ...    R0 = euler_matrix(axes=axes, *angles)
-    ...    R1 = euler_matrix(axes=axes, *euler_from_matrix(R0, axes))
-    ...    if not numpy.allclose(R0, R1): print axes, "failed"
-
-    """
-    try:
-        firstaxis, parity, repetition, frame = _AXES2TUPLE[axes.lower()]
-    except (AttributeError, KeyError):
-        _ = _TUPLE2AXES[axes]
-        firstaxis, parity, repetition, frame = axes
-
-    i = firstaxis
-    j = _NEXT_AXIS[i+parity]
-    k = _NEXT_AXIS[i-parity+1]
-
-    M = numpy.array(matrix, dtype=numpy.float64, copy=False)[:3, :3]
-    if repetition:
-        sy = math.sqrt(M[i, j]*M[i, j] + M[i, k]*M[i, k])
-        if sy > _EPS:
-            ax = math.atan2( M[i, j],  M[i, k])
-            ay = math.atan2( sy,       M[i, i])
-            az = math.atan2( M[j, i], -M[k, i])
-        else:
-            ax = math.atan2(-M[j, k],  M[j, j])
-            ay = math.atan2( sy,       M[i, i])
-            az = 0.0
-    else:
-        cy = math.sqrt(M[i, i]*M[i, i] + M[j, i]*M[j, i])
-        if cy > _EPS:
-            ax = math.atan2( M[k, j],  M[k, k])
-            ay = math.atan2(-M[k, i],  cy)
-            az = math.atan2( M[j, i],  M[i, i])
-        else:
-            ax = math.atan2(-M[j, k],  M[j, j])
-            ay = math.atan2(-M[k, i],  cy)
-            az = 0.0
-
-    if parity:
-        ax, ay, az = -ax, -ay, -az
-    if frame:
-        ax, az = az, ax
-    return ax, ay, az
-
-
-def euler_from_quaternion(quaternion, axes='sxyz'):
-    """Return Euler angles from quaternion for specified axis sequence.
-
-    >>> angles = euler_from_quaternion([0.06146124, 0, 0, 0.99810947])
-    >>> numpy.allclose(angles, [0.123, 0, 0])
-    True
-
-    """
-    return euler_from_matrix(quaternion_matrix(quaternion), axes)
-
-
-def quaternion_from_euler(ai, aj, ak, axes='sxyz'):
-    """Return quaternion from Euler angles and axis sequence.
-
-    ai, aj, ak : Euler's roll, pitch and yaw angles
-    axes : One of 24 axis sequences as string or encoded tuple
-
-    >>> q = quaternion_from_euler(1, 2, 3, 'ryxz')
-    >>> numpy.allclose(q, [0.310622, -0.718287, 0.444435, 0.435953])
-    True
-
-    """
-    try:
-        firstaxis, parity, repetition, frame = _AXES2TUPLE[axes.lower()]
-    except (AttributeError, KeyError):
-        _ = _TUPLE2AXES[axes]
-        firstaxis, parity, repetition, frame = axes
-
-    i = firstaxis
-    j = _NEXT_AXIS[i+parity]
-    k = _NEXT_AXIS[i-parity+1]
-
-    if frame:
-        ai, ak = ak, ai
-    if parity:
-        aj = -aj
-
-    ai /= 2.0
-    aj /= 2.0
-    ak /= 2.0
-    ci = math.cos(ai)
-    si = math.sin(ai)
-    cj = math.cos(aj)
-    sj = math.sin(aj)
-    ck = math.cos(ak)
-    sk = math.sin(ak)
-    cc = ci*ck
-    cs = ci*sk
-    sc = si*ck
-    ss = si*sk
-
-    quaternion = numpy.empty((4, ), dtype=numpy.float64)
-    if repetition:
-        quaternion[i] = cj*(cs + sc)
-        quaternion[j] = sj*(cc + ss)
-        quaternion[k] = sj*(cs - sc)
-        quaternion[3] = cj*(cc - ss)
-    else:
-        quaternion[i] = cj*sc - sj*cs
-        quaternion[j] = cj*ss + sj*cc
-        quaternion[k] = cj*cs - sj*sc
-        quaternion[3] = cj*cc + sj*ss
-    if parity:
-        quaternion[j] *= -1
-
-    return quaternion
-
-
-def quaternion_about_axis(angle, axis):
-    """Return quaternion for rotation about axis.
-
-    >>> q = quaternion_about_axis(0.123, (1, 0, 0))
-    >>> numpy.allclose(q, [0.06146124, 0, 0, 0.99810947])
-    True
-
-    """
-    quaternion = numpy.zeros((4, ), dtype=numpy.float64)
-    quaternion[:3] = axis[:3]
-    qlen = vector_norm(quaternion)
-    if qlen > _EPS:
-        quaternion *= math.sin(angle/2.0) / qlen
-    quaternion[3] = math.cos(angle/2.0)
-    return quaternion
-
-
-def quaternion_matrix(quaternion):
-    """Return homogeneous rotation matrix from quaternion.
-
-    >>> R = quaternion_matrix([0.06146124, 0, 0, 0.99810947])
-    >>> numpy.allclose(R, rotation_matrix(0.123, (1, 0, 0)))
-    True
-
-    """
-    q = numpy.array(quaternion[:4], dtype=numpy.float64, copy=True)
-    nq = numpy.dot(q, q)
-    if nq < _EPS:
-        return numpy.identity(4)
-    q *= math.sqrt(2.0 / nq)
-    q = numpy.outer(q, q)
-    return numpy.array((
-        (1.0-q[1, 1]-q[2, 2],     q[0, 1]-q[2, 3],     q[0, 2]+q[1, 3], 0.0),
-        (    q[0, 1]+q[2, 3], 1.0-q[0, 0]-q[2, 2],     q[1, 2]-q[0, 3], 0.0),
-        (    q[0, 2]-q[1, 3],     q[1, 2]+q[0, 3], 1.0-q[0, 0]-q[1, 1], 0.0),
-        (                0.0,                 0.0,                 0.0, 1.0)
-        ), dtype=numpy.float64)
-
-
-def quaternion_from_matrix(matrix):
-    """Return quaternion from rotation matrix.
-
-    >>> R = rotation_matrix(0.123, (1, 2, 3))
-    >>> q = quaternion_from_matrix(R)
-    >>> numpy.allclose(q, [0.0164262, 0.0328524, 0.0492786, 0.9981095])
-    True
-
-    """
-    q = numpy.empty((4, ), dtype=numpy.float64)
-    M = numpy.array(matrix, dtype=numpy.float64, copy=False)[:4, :4]
-    t = numpy.trace(M)
-    if t > M[3, 3]:
-        q[3] = t
-        q[2] = M[1, 0] - M[0, 1]
-        q[1] = M[0, 2] - M[2, 0]
-        q[0] = M[2, 1] - M[1, 2]
-    else:
-        i, j, k = 0, 1, 2
-        if M[1, 1] > M[0, 0]:
-            i, j, k = 1, 2, 0
-        if M[2, 2] > M[i, i]:
-            i, j, k = 2, 0, 1
-        t = M[i, i] - (M[j, j] + M[k, k]) + M[3, 3]
-        q[i] = t
-        q[j] = M[i, j] + M[j, i]
-        q[k] = M[k, i] + M[i, k]
-        q[3] = M[k, j] - M[j, k]
-    q *= 0.5 / math.sqrt(t * M[3, 3])
-    return q
-
-
-def quaternion_multiply(quaternion1, quaternion0):
-    """Return multiplication of two quaternions.
-
-    >>> q = quaternion_multiply([1, -2, 3, 4], [-5, 6, 7, 8])
-    >>> numpy.allclose(q, [-44, -14, 48, 28])
-    True
-
-    """
-    x0, y0, z0, w0 = quaternion0
-    x1, y1, z1, w1 = quaternion1
-    return numpy.array((
-         x1*w0 + y1*z0 - z1*y0 + w1*x0,
-        -x1*z0 + y1*w0 + z1*x0 + w1*y0,
-         x1*y0 - y1*x0 + z1*w0 + w1*z0,
-        -x1*x0 - y1*y0 - z1*z0 + w1*w0), dtype=numpy.float64)
-
-
-def quaternion_conjugate(quaternion):
-    """Return conjugate of quaternion.
-
-    >>> q0 = random_quaternion()
-    >>> q1 = quaternion_conjugate(q0)
-    >>> q1[3] == q0[3] and all(q1[:3] == -q0[:3])
-    True
-
-    """
-    return numpy.array((-quaternion[0], -quaternion[1],
-                        -quaternion[2], quaternion[3]), dtype=numpy.float64)
-
-
-def quaternion_inverse(quaternion):
-    """Return inverse of quaternion.
-
-    >>> q0 = random_quaternion()
-    >>> q1 = quaternion_inverse(q0)
-    >>> numpy.allclose(quaternion_multiply(q0, q1), [0, 0, 0, 1])
-    True
-
-    """
-    return quaternion_conjugate(quaternion) / numpy.dot(quaternion, quaternion)
-
-
-def quaternion_slerp(quat0, quat1, fraction, spin=0, shortestpath=True):
-    """Return spherical linear interpolation between two quaternions.
-
-    >>> q0 = random_quaternion()
-    >>> q1 = random_quaternion()
-    >>> q = quaternion_slerp(q0, q1, 0.0)
-    >>> numpy.allclose(q, q0)
-    True
-    >>> q = quaternion_slerp(q0, q1, 1.0, 1)
-    >>> numpy.allclose(q, q1)
-    True
-    >>> q = quaternion_slerp(q0, q1, 0.5)
-    >>> angle = math.acos(numpy.dot(q0, q))
-    >>> numpy.allclose(2.0, math.acos(numpy.dot(q0, q1)) / angle) or \
-        numpy.allclose(2.0, math.acos(-numpy.dot(q0, q1)) / angle)
-    True
-
-    """
-    q0 = unit_vector(quat0[:4])
-    q1 = unit_vector(quat1[:4])
-    if fraction == 0.0:
-        return q0
-    elif fraction == 1.0:
-        return q1
-    d = numpy.dot(q0, q1)
-    if abs(abs(d) - 1.0) < _EPS:
-        return q0
-    if shortestpath and d < 0.0:
-        # invert rotation
-        d = -d
-        q1 *= -1.0
-    angle = math.acos(d) + spin * math.pi
-    if abs(angle) < _EPS:
-        return q0
-    isin = 1.0 / math.sin(angle)
-    q0 *= math.sin((1.0 - fraction) * angle) * isin
-    q1 *= math.sin(fraction * angle) * isin
-    q0 += q1
-    return q0
-
-
-def random_quaternion(rand=None):
-    """Return uniform random unit quaternion.
-
-    rand: array like or None
-        Three independent random variables that are uniformly distributed
-        between 0 and 1.
-
-    >>> q = random_quaternion()
-    >>> numpy.allclose(1.0, vector_norm(q))
-    True
-    >>> q = random_quaternion(numpy.random.random(3))
-    >>> q.shape
-    (4,)
-
-    """
-    if rand is None:
-        rand = numpy.random.rand(3)
-    else:
-        assert len(rand) == 3
-    r1 = numpy.sqrt(1.0 - rand[0])
-    r2 = numpy.sqrt(rand[0])
-    pi2 = math.pi * 2.0
-    t1 = pi2 * rand[1]
-    t2 = pi2 * rand[2]
-    return numpy.array((numpy.sin(t1)*r1,
-                        numpy.cos(t1)*r1,
-                        numpy.sin(t2)*r2,
-                        numpy.cos(t2)*r2), dtype=numpy.float64)
-
-
-def random_rotation_matrix(rand=None):
-    """Return uniform random rotation matrix.
-
-    rnd: array like
-        Three independent random variables that are uniformly distributed
-        between 0 and 1 for each returned quaternion.
-
-    >>> R = random_rotation_matrix()
-    >>> numpy.allclose(numpy.dot(R.T, R), numpy.identity(4))
-    True
-
-    """
-    return quaternion_matrix(random_quaternion(rand))
-
-
-class Arcball(object):
-    """Virtual Trackball Control.
-
-    >>> ball = Arcball()
-    >>> ball = Arcball(initial=numpy.identity(4))
-    >>> ball.place([320, 320], 320)
-    >>> ball.down([500, 250])
-    >>> ball.drag([475, 275])
-    >>> R = ball.matrix()
-    >>> numpy.allclose(numpy.sum(R), 3.90583455)
-    True
-    >>> ball = Arcball(initial=[0, 0, 0, 1])
-    >>> ball.place([320, 320], 320)
-    >>> ball.setaxes([1,1,0], [-1, 1, 0])
-    >>> ball.setconstrain(True)
-    >>> ball.down([400, 200])
-    >>> ball.drag([200, 400])
-    >>> R = ball.matrix()
-    >>> numpy.allclose(numpy.sum(R), 0.2055924)
-    True
-    >>> ball.next()
-
-    """
-
-    def __init__(self, initial=None):
-        """Initialize virtual trackball control.
-
-        initial : quaternion or rotation matrix
-
-        """
-        self._axis = None
-        self._axes = None
-        self._radius = 1.0
-        self._center = [0.0, 0.0]
-        self._vdown = numpy.array([0, 0, 1], dtype=numpy.float64)
-        self._constrain = False
-
-        if initial is None:
-            self._qdown = numpy.array([0, 0, 0, 1], dtype=numpy.float64)
-        else:
-            initial = numpy.array(initial, dtype=numpy.float64)
-            if initial.shape == (4, 4):
-                self._qdown = quaternion_from_matrix(initial)
-            elif initial.shape == (4, ):
-                initial /= vector_norm(initial)
-                self._qdown = initial
-            else:
-                raise ValueError("initial not a quaternion or matrix.")
-
-        self._qnow = self._qpre = self._qdown
-
-    def place(self, center, radius):
-        """Place Arcball, e.g. when window size changes.
-
-        center : sequence[2]
-            Window coordinates of trackball center.
-        radius : float
-            Radius of trackball in window coordinates.
-
-        """
-        self._radius = float(radius)
-        self._center[0] = center[0]
-        self._center[1] = center[1]
-
-    def setaxes(self, *axes):
-        """Set axes to constrain rotations."""
-        if axes is None:
-            self._axes = None
-        else:
-            self._axes = [unit_vector(axis) for axis in axes]
-
-    def setconstrain(self, constrain):
-        """Set state of constrain to axis mode."""
-        self._constrain = constrain == True
-
-    def getconstrain(self):
-        """Return state of constrain to axis mode."""
-        return self._constrain
-
-    def down(self, point):
-        """Set initial cursor window coordinates and pick constrain-axis."""
-        self._vdown = arcball_map_to_sphere(point, self._center, self._radius)
-        self._qdown = self._qpre = self._qnow
-
-        if self._constrain and self._axes is not None:
-            self._axis = arcball_nearest_axis(self._vdown, self._axes)
-            self._vdown = arcball_constrain_to_axis(self._vdown, self._axis)
-        else:
-            self._axis = None
-
-    def drag(self, point):
-        """Update current cursor window coordinates."""
-        vnow = arcball_map_to_sphere(point, self._center, self._radius)
-
-        if self._axis is not None:
-            vnow = arcball_constrain_to_axis(vnow, self._axis)
-
-        self._qpre = self._qnow
-
-        t = numpy.cross(self._vdown, vnow)
-        if numpy.dot(t, t) < _EPS:
-            self._qnow = self._qdown
-        else:
-            q = [t[0], t[1], t[2], numpy.dot(self._vdown, vnow)]
-            self._qnow = quaternion_multiply(q, self._qdown)
-
-    def next(self, acceleration=0.0):
-        """Continue rotation in direction of last drag."""
-        q = quaternion_slerp(self._qpre, self._qnow, 2.0+acceleration, False)
-        self._qpre, self._qnow = self._qnow, q
-
-    def matrix(self):
-        """Return homogeneous rotation matrix."""
-        return quaternion_matrix(self._qnow)
-
-
-def arcball_map_to_sphere(point, center, radius):
-    """Return unit sphere coordinates from window coordinates."""
-    v = numpy.array(((point[0] - center[0]) / radius,
-                     (center[1] - point[1]) / radius,
-                     0.0), dtype=numpy.float64)
-    n = v[0]*v[0] + v[1]*v[1]
-    if n > 1.0:
-        v /= math.sqrt(n) # position outside of sphere
-    else:
-        v[2] = math.sqrt(1.0 - n)
-    return v
-
-
-def arcball_constrain_to_axis(point, axis):
-    """Return sphere point perpendicular to axis."""
-    v = numpy.array(point, dtype=numpy.float64, copy=True)
-    a = numpy.array(axis, dtype=numpy.float64, copy=True)
-    v -= a * numpy.dot(a, v) # on plane
-    n = vector_norm(v)
-    if n > _EPS:
-        if v[2] < 0.0:
-            v *= -1.0
-        v /= n
-        return v
-    if a[2] == 1.0:
-        return numpy.array([1, 0, 0], dtype=numpy.float64)
-    return unit_vector([-a[1], a[0], 0])
-
-
-def arcball_nearest_axis(point, axes):
-    """Return axis, which arc is nearest to point."""
-    point = numpy.array(point, dtype=numpy.float64, copy=False)
-    nearest = None
-    mx = -1.0
-    for axis in axes:
-        t = numpy.dot(arcball_constrain_to_axis(point, axis), point)
-        if t > mx:
-            nearest = axis
-            mx = t
-    return nearest
-
-
-# epsilon for testing whether a number is close to zero
-_EPS = numpy.finfo(float).eps * 4.0
-
-# axis sequences for Euler angles
-_NEXT_AXIS = [1, 2, 0, 1]
-
-# map axes strings to/from tuples of inner axis, parity, repetition, frame
-_AXES2TUPLE = {
-    'sxyz': (0, 0, 0, 0), 'sxyx': (0, 0, 1, 0), 'sxzy': (0, 1, 0, 0),
-    'sxzx': (0, 1, 1, 0), 'syzx': (1, 0, 0, 0), 'syzy': (1, 0, 1, 0),
-    'syxz': (1, 1, 0, 0), 'syxy': (1, 1, 1, 0), 'szxy': (2, 0, 0, 0),
-    'szxz': (2, 0, 1, 0), 'szyx': (2, 1, 0, 0), 'szyz': (2, 1, 1, 0),
-    'rzyx': (0, 0, 0, 1), 'rxyx': (0, 0, 1, 1), 'ryzx': (0, 1, 0, 1),
-    'rxzx': (0, 1, 1, 1), 'rxzy': (1, 0, 0, 1), 'ryzy': (1, 0, 1, 1),
-    'rzxy': (1, 1, 0, 1), 'ryxy': (1, 1, 1, 1), 'ryxz': (2, 0, 0, 1),
-    'rzxz': (2, 0, 1, 1), 'rxyz': (2, 1, 0, 1), 'rzyz': (2, 1, 1, 1)}
-
-_TUPLE2AXES = dict((v, k) for k, v in _AXES2TUPLE.items())
-
-# helper functions
-
-def vector_norm(data, axis=None, out=None):
-    """Return length, i.e. eucledian norm, of ndarray along axis.
-
-    >>> v = numpy.random.random(3)
-    >>> n = vector_norm(v)
-    >>> numpy.allclose(n, numpy.linalg.norm(v))
-    True
-    >>> v = numpy.random.rand(6, 5, 3)
-    >>> n = vector_norm(v, axis=-1)
-    >>> numpy.allclose(n, numpy.sqrt(numpy.sum(v*v, axis=2)))
-    True
-    >>> n = vector_norm(v, axis=1)
-    >>> numpy.allclose(n, numpy.sqrt(numpy.sum(v*v, axis=1)))
-    True
-    >>> v = numpy.random.rand(5, 4, 3)
-    >>> n = numpy.empty((5, 3), dtype=numpy.float64)
-    >>> vector_norm(v, axis=1, out=n)
-    >>> numpy.allclose(n, numpy.sqrt(numpy.sum(v*v, axis=1)))
-    True
-    >>> vector_norm([])
-    0.0
-    >>> vector_norm([1.0])
-    1.0
-
-    """
-    data = numpy.array(data, dtype=numpy.float64, copy=True)
-    if out is None:
-        if data.ndim == 1:
-            return math.sqrt(numpy.dot(data, data))
-        data *= data
-        out = numpy.atleast_1d(numpy.sum(data, axis=axis))
-        numpy.sqrt(out, out)
-        return out
-    else:
-        data *= data
-        numpy.sum(data, axis=axis, out=out)
-        numpy.sqrt(out, out)
-
-
-def unit_vector(data, axis=None, out=None):
-    """Return ndarray normalized by length, i.e. eucledian norm, along axis.
-
-    >>> v0 = numpy.random.random(3)
-    >>> v1 = unit_vector(v0)
-    >>> numpy.allclose(v1, v0 / numpy.linalg.norm(v0))
-    True
-    >>> v0 = numpy.random.rand(5, 4, 3)
-    >>> v1 = unit_vector(v0, axis=-1)
-    >>> v2 = v0 / numpy.expand_dims(numpy.sqrt(numpy.sum(v0*v0, axis=2)), 2)
-    >>> numpy.allclose(v1, v2)
-    True
-    >>> v1 = unit_vector(v0, axis=1)
-    >>> v2 = v0 / numpy.expand_dims(numpy.sqrt(numpy.sum(v0*v0, axis=1)), 1)
-    >>> numpy.allclose(v1, v2)
-    True
-    >>> v1 = numpy.empty((5, 4, 3), dtype=numpy.float64)
-    >>> unit_vector(v0, axis=1, out=v1)
-    >>> numpy.allclose(v1, v2)
-    True
-    >>> list(unit_vector([]))
-    []
-    >>> list(unit_vector([1.0]))
-    [1.0]
-
-    """
-    if out is None:
-        data = numpy.array(data, dtype=numpy.float64, copy=True)
-        if data.ndim == 1:
-            data /= math.sqrt(numpy.dot(data, data))
-            return data
-    else:
-        if out is not data:
-            out[:] = numpy.array(data, copy=False)
-        data = out
-    length = numpy.atleast_1d(numpy.sum(data*data, axis))
-    numpy.sqrt(length, length)
-    if axis is not None:
-        length = numpy.expand_dims(length, axis)
-    data /= length
-    if out is None:
-        return data
-
-
-def random_vector(size):
-    """Return array of random doubles in the half-open interval [0.0, 1.0).
-
-    >>> v = random_vector(10000)
-    >>> numpy.all(v >= 0.0) and numpy.all(v < 1.0)
-    True
-    >>> v0 = random_vector(10)
-    >>> v1 = random_vector(10)
-    >>> numpy.any(v0 == v1)
-    False
-
-    """
-    return numpy.random.random(size)
-
-
-def inverse_matrix(matrix):
-    """Return inverse of square transformation matrix.
-
-    >>> M0 = random_rotation_matrix()
-    >>> M1 = inverse_matrix(M0.T)
-    >>> numpy.allclose(M1, numpy.linalg.inv(M0.T))
-    True
-    >>> for size in range(1, 7):
-    ...     M0 = numpy.random.rand(size, size)
-    ...     M1 = inverse_matrix(M0)
-    ...     if not numpy.allclose(M1, numpy.linalg.inv(M0)): print size
-
-    """
-    return numpy.linalg.inv(matrix)
-
-
-def concatenate_matrices(*matrices):
-    """Return concatenation of series of transformation matrices.
-
-    >>> M = numpy.random.rand(16).reshape((4, 4)) - 0.5
-    >>> numpy.allclose(M, concatenate_matrices(M))
-    True
-    >>> numpy.allclose(numpy.dot(M, M.T), concatenate_matrices(M, M.T))
-    True
-
-    """
-    M = numpy.identity(4)
-    for i in matrices:
-        M = numpy.dot(M, i)
-    return M
-
-
-def is_same_transform(matrix0, matrix1):
-    """Return True if two matrices perform same transformation.
-
-    >>> is_same_transform(numpy.identity(4), numpy.identity(4))
-    True
-    >>> is_same_transform(numpy.identity(4), random_rotation_matrix())
-    False
-
-    """
-    matrix0 = numpy.array(matrix0, dtype=numpy.float64, copy=True)
-    matrix0 /= matrix0[3, 3]
-    matrix1 = numpy.array(matrix1, dtype=numpy.float64, copy=True)
-    matrix1 /= matrix1[3, 3]
-    return numpy.allclose(matrix0, matrix1)
+# -*- coding: utf-8 -*-
+# transformations.py
+
+# Copyright (c) 2006, Christoph Gohlke
+# Copyright (c) 2006-2009, The Regents of the University of California
+# All rights reserved.
+#
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted provided that the following conditions are met:
+#
+# * Redistributions of source code must retain the above copyright
+#   notice, this list of conditions and the following disclaimer.
+# * Redistributions in binary form must reproduce the above copyright
+#   notice, this list of conditions and the following disclaimer in the
+#   documentation and/or other materials provided with the distribution.
+# * Neither the name of the copyright holders nor the names of any
+#   contributors may be used to endorse or promote products derived
+#   from this software without specific prior written permission.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+# ARE DISCLAIMED.  IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE
+# LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+# CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+# SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+# INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+# ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+# POSSIBILITY OF SUCH DAMAGE.
+
+"""Homogeneous Transformation Matrices and Quaternions.
+
+A library for calculating 4x4 matrices for translating, rotating, reflecting,
+scaling, shearing, projecting, orthogonalizing, and superimposing arrays of
+3D homogeneous coordinates as well as for converting between rotation matrices,
+Euler angles, and quaternions. Also includes an Arcball control object and
+functions to decompose transformation matrices.
+
+:Authors:
+  `Christoph Gohlke <http://www.lfd.uci.edu/~gohlke/>`__,
+  Laboratory for Fluorescence Dynamics, University of California, Irvine
+
+:Version: 20090418
+
+Requirements
+------------
+
+* `Python 2.6 <http://www.python.org>`__
+* `Numpy 1.3 <http://numpy.scipy.org>`__
+* `transformations.c 20090418 <http://www.lfd.uci.edu/~gohlke/>`__
+  (optional implementation of some functions in C)
+
+Notes
+-----
+
+Matrices (M) can be inverted using numpy.linalg.inv(M), concatenated using
+numpy.dot(M0, M1), or used to transform homogeneous coordinates (v) using
+numpy.dot(M, v) for shape (4, *) "point of arrays", respectively
+numpy.dot(v, M.T) for shape (*, 4) "array of points".
+
+Calculations are carried out with numpy.float64 precision.
+
+This Python implementation is not optimized for speed.
+
+Vector, point, quaternion, and matrix function arguments are expected to be
+"array like", i.e. tuple, list, or numpy arrays.
+
+Return types are numpy arrays unless specified otherwise.
+
+Angles are in radians unless specified otherwise.
+
+Quaternions ix+jy+kz+w are represented as [x, y, z, w].
+
+Use the transpose of transformation matrices for OpenGL glMultMatrixd().
+
+A triple of Euler angles can be applied/interpreted in 24 ways, which can
+be specified using a 4 character string or encoded 4-tuple:
+
+  *Axes 4-string*: e.g. 'sxyz' or 'ryxy'
+
+  - first character : rotations are applied to 's'tatic or 'r'otating frame
+  - remaining characters : successive rotation axis 'x', 'y', or 'z'
+
+  *Axes 4-tuple*: e.g. (0, 0, 0, 0) or (1, 1, 1, 1)
+
+  - inner axis: code of axis ('x':0, 'y':1, 'z':2) of rightmost matrix.
+  - parity : even (0) if inner axis 'x' is followed by 'y', 'y' is followed
+    by 'z', or 'z' is followed by 'x'. Otherwise odd (1).
+  - repetition : first and last axis are same (1) or different (0).
+  - frame : rotations are applied to static (0) or rotating (1) frame.
+
+References
+----------
+
+(1)  Matrices and transformations. Ronald Goldman.
+     In "Graphics Gems I", pp 472-475. Morgan Kaufmann, 1990.
+(2)  More matrices and transformations: shear and pseudo-perspective.
+     Ronald Goldman. In "Graphics Gems II", pp 320-323. Morgan Kaufmann, 1991.
+(3)  Decomposing a matrix into simple transformations. Spencer Thomas.
+     In "Graphics Gems II", pp 320-323. Morgan Kaufmann, 1991.
+(4)  Recovering the data from the transformation matrix. Ronald Goldman.
+     In "Graphics Gems II", pp 324-331. Morgan Kaufmann, 1991.
+(5)  Euler angle conversion. Ken Shoemake.
+     In "Graphics Gems IV", pp 222-229. Morgan Kaufmann, 1994.
+(6)  Arcball rotation control. Ken Shoemake.
+     In "Graphics Gems IV", pp 175-192. Morgan Kaufmann, 1994.
+(7)  Representing attitude: Euler angles, unit quaternions, and rotation
+     vectors. James Diebel. 2006.
+(8)  A discussion of the solution for the best rotation to relate two sets
+     of vectors. W Kabsch. Acta Cryst. 1978. A34, 827-828.
+(9)  Closed-form solution of absolute orientation using unit quaternions.
+     BKP Horn. J Opt Soc Am A. 1987. 4(4), 629-642.
+(10) Quaternions. Ken Shoemake.
+     http://www.sfu.ca/~jwa3/cmpt461/files/quatut.pdf
+(11) From quaternion to matrix and back. JMP van Waveren. 2005.
+     http://www.intel.com/cd/ids/developer/asmo-na/eng/293748.htm
+(12) Uniform random rotations. Ken Shoemake.
+     In "Graphics Gems III", pp 124-132. Morgan Kaufmann, 1992.
+
+
+Examples
+--------
+
+>>> alpha, beta, gamma = 0.123, -1.234, 2.345
+>>> origin, xaxis, yaxis, zaxis = (0, 0, 0), (1, 0, 0), (0, 1, 0), (0, 0, 1)
+>>> I = identity_matrix()
+>>> Rx = rotation_matrix(alpha, xaxis)
+>>> Ry = rotation_matrix(beta, yaxis)
+>>> Rz = rotation_matrix(gamma, zaxis)
+>>> R = concatenate_matrices(Rx, Ry, Rz)
+>>> euler = euler_from_matrix(R, 'rxyz')
+>>> numpy.allclose([alpha, beta, gamma], euler)
+True
+>>> Re = euler_matrix(alpha, beta, gamma, 'rxyz')
+>>> is_same_transform(R, Re)
+True
+>>> al, be, ga = euler_from_matrix(Re, 'rxyz')
+>>> is_same_transform(Re, euler_matrix(al, be, ga, 'rxyz'))
+True
+>>> qx = quaternion_about_axis(alpha, xaxis)
+>>> qy = quaternion_about_axis(beta, yaxis)
+>>> qz = quaternion_about_axis(gamma, zaxis)
+>>> q = quaternion_multiply(qx, qy)
+>>> q = quaternion_multiply(q, qz)
+>>> Rq = quaternion_matrix(q)
+>>> is_same_transform(R, Rq)
+True
+>>> S = scale_matrix(1.23, origin)
+>>> T = translation_matrix((1, 2, 3))
+>>> Z = shear_matrix(beta, xaxis, origin, zaxis)
+>>> R = random_rotation_matrix(numpy.random.rand(3))
+>>> M = concatenate_matrices(T, R, Z, S)
+>>> scale, shear, angles, trans, persp = decompose_matrix(M)
+>>> numpy.allclose(scale, 1.23)
+True
+>>> numpy.allclose(trans, (1, 2, 3))
+True
+>>> numpy.allclose(shear, (0, math.tan(beta), 0))
+True
+>>> is_same_transform(R, euler_matrix(axes='sxyz', *angles))
+True
+>>> M1 = compose_matrix(scale, shear, angles, trans, persp)
+>>> is_same_transform(M, M1)
+True
+
+"""
+
+from __future__ import division
+
+import warnings
+import math
+
+import numpy
+
+# Documentation in HTML format can be generated with Epydoc
+__docformat__ = "restructuredtext en"
+
+
+def identity_matrix():
+    """Return 4x4 identity/unit matrix.
+
+    >>> I = identity_matrix()
+    >>> numpy.allclose(I, numpy.dot(I, I))
+    True
+    >>> numpy.sum(I), numpy.trace(I)
+    (4.0, 4.0)
+    >>> numpy.allclose(I, numpy.identity(4, dtype=numpy.float64))
+    True
+
+    """
+    return numpy.identity(4, dtype=numpy.float64)
+
+def dh_matrix(alpha, a, d, theta, dh_mode = "SDH"):
+    """Return DH matrix by params.
+    
+    Args:
+        alpha,a,d,theta: DH parameters
+        dh_mode: "SDH" -> Standard DH
+                 "MDH" -> Modified DH
+    """
+    sinth = math.sin(theta)
+    costh = math.cos(theta)
+    sina = math.sin(alpha)
+    cosa = math.cos(alpha)
+    if (dh_mode == "SDH"):
+        M = numpy.array(((costh, -sinth * cosa,  sinth * sina, a * costh),
+                        (sinth,  costh * cosa, -costh * sina, a * sinth),
+                        (0.0  ,  sina        ,  cosa        , d        ),
+                        (0.0  ,  0.0         ,  0.0         , 1.0      )), dtype=numpy.float64)
+    if (dh_mode == "MDH"):
+        M = numpy.array(((costh       , -sinth      ,  0   ,  a       ),
+                        (sinth * cosa, costh * cosa, -sina, -sina * d),
+                        (sinth * sina, costh * sina,  cosa,  cosa * d),
+                        (0.0         , 0.0,           0.0,   1.0     )), dtype=numpy.float64)
+    return M
+
+def translation_matrix(direction):
+    """Return matrix to translate by direction vector.
+
+    >>> v = numpy.random.random(3) - 0.5
+    >>> numpy.allclose(v, translation_matrix(v)[:3, 3])
+    True
+
+    """
+    M = numpy.identity(4)
+    M[:3, 3] = direction[:3]
+    return M
+
+
+def translation_from_matrix(matrix):
+    """Return translation vector from translation matrix.
+
+    >>> v0 = numpy.random.random(3) - 0.5
+    >>> v1 = translation_from_matrix(translation_matrix(v0))
+    >>> numpy.allclose(v0, v1)
+    True
+
+    """
+    return numpy.array(matrix, copy=False)[:3, 3].copy()
+
+
+def reflection_matrix(point, normal):
+    """Return matrix to mirror at plane defined by point and normal vector.
+
+    >>> v0 = numpy.random.random(4) - 0.5
+    >>> v0[3] = 1.0
+    >>> v1 = numpy.random.random(3) - 0.5
+    >>> R = reflection_matrix(v0, v1)
+    >>> numpy.allclose(2., numpy.trace(R))
+    True
+    >>> numpy.allclose(v0, numpy.dot(R, v0))
+    True
+    >>> v2 = v0.copy()
+    >>> v2[:3] += v1
+    >>> v3 = v0.copy()
+    >>> v2[:3] -= v1
+    >>> numpy.allclose(v2, numpy.dot(R, v3))
+    True
+
+    """
+    normal = unit_vector(normal[:3])
+    M = numpy.identity(4)
+    M[:3, :3] -= 2.0 * numpy.outer(normal, normal)
+    M[:3, 3] = (2.0 * numpy.dot(point[:3], normal)) * normal
+    return M
+
+
+def reflection_from_matrix(matrix):
+    """Return mirror plane point and normal vector from reflection matrix.
+
+    >>> v0 = numpy.random.random(3) - 0.5
+    >>> v1 = numpy.random.random(3) - 0.5
+    >>> M0 = reflection_matrix(v0, v1)
+    >>> point, normal = reflection_from_matrix(M0)
+    >>> M1 = reflection_matrix(point, normal)
+    >>> is_same_transform(M0, M1)
+    True
+
+    """
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)
+    # normal: unit eigenvector corresponding to eigenvalue -1
+    l, V = numpy.linalg.eig(M[:3, :3])
+    i = numpy.where(abs(numpy.real(l) + 1.0) < 1e-8)[0]
+    if not len(i):
+        raise ValueError("no unit eigenvector corresponding to eigenvalue -1")
+    normal = numpy.real(V[:, i[0]]).squeeze()
+    # point: any unit eigenvector corresponding to eigenvalue 1
+    l, V = numpy.linalg.eig(M)
+    i = numpy.where(abs(numpy.real(l) - 1.0) < 1e-8)[0]
+    if not len(i):
+        raise ValueError("no unit eigenvector corresponding to eigenvalue 1")
+    point = numpy.real(V[:, i[-1]]).squeeze()
+    point /= point[3]
+    return point, normal
+
+
+def rotation_matrix(angle, direction, point=None):
+    """Return matrix to rotate about axis defined by point and direction.
+
+    >>> angle = (random.random() - 0.5) * (2*math.pi)
+    >>> direc = numpy.random.random(3) - 0.5
+    >>> point = numpy.random.random(3) - 0.5
+    >>> R0 = rotation_matrix(angle, direc, point)
+    >>> R1 = rotation_matrix(angle-2*math.pi, direc, point)
+    >>> is_same_transform(R0, R1)
+    True
+    >>> R0 = rotation_matrix(angle, direc, point)
+    >>> R1 = rotation_matrix(-angle, -direc, point)
+    >>> is_same_transform(R0, R1)
+    True
+    >>> I = numpy.identity(4, numpy.float64)
+    >>> numpy.allclose(I, rotation_matrix(math.pi*2, direc))
+    True
+    >>> numpy.allclose(2., numpy.trace(rotation_matrix(math.pi/2,
+    ...                                                direc, point)))
+    True
+
+    """
+    sina = math.sin(angle)
+    cosa = math.cos(angle)
+    direction = unit_vector(direction[:3])
+    # rotation matrix around unit vector
+    R = numpy.array(((cosa, 0.0,  0.0),
+                     (0.0,  cosa, 0.0),
+                     (0.0,  0.0,  cosa)), dtype=numpy.float64)
+    R += numpy.outer(direction, direction) * (1.0 - cosa)
+    direction *= sina
+    R += numpy.array((( 0.0,         -direction[2],  direction[1]),
+                      ( direction[2], 0.0,          -direction[0]),
+                      (-direction[1], direction[0],  0.0)),
+                     dtype=numpy.float64)
+    M = numpy.identity(4)
+    M[:3, :3] = R
+    if point is not None:
+        # rotation not around origin
+        point = numpy.array(point[:3], dtype=numpy.float64, copy=False)
+        M[:3, 3] = point - numpy.dot(R, point)
+    return M
+
+
+def rotation_from_matrix(matrix):
+    """Return rotation angle and axis from rotation matrix.
+
+    >>> angle = (random.random() - 0.5) * (2*math.pi)
+    >>> direc = numpy.random.random(3) - 0.5
+    >>> point = numpy.random.random(3) - 0.5
+    >>> R0 = rotation_matrix(angle, direc, point)
+    >>> angle, direc, point = rotation_from_matrix(R0)
+    >>> R1 = rotation_matrix(angle, direc, point)
+    >>> is_same_transform(R0, R1)
+    True
+
+    """
+    R = numpy.array(matrix, dtype=numpy.float64, copy=False)
+    R33 = R[:3, :3]
+    # direction: unit eigenvector of R33 corresponding to eigenvalue of 1
+    l, W = numpy.linalg.eig(R33.T)
+    i = numpy.where(abs(numpy.real(l) - 1.0) < 1e-8)[0]
+    if not len(i):
+        raise ValueError("no unit eigenvector corresponding to eigenvalue 1")
+    direction = numpy.real(W[:, i[-1]]).squeeze()
+    # point: unit eigenvector of R33 corresponding to eigenvalue of 1
+    l, Q = numpy.linalg.eig(R)
+    i = numpy.where(abs(numpy.real(l) - 1.0) < 1e-8)[0]
+    if not len(i):
+        raise ValueError("no unit eigenvector corresponding to eigenvalue 1")
+    point = numpy.real(Q[:, i[-1]]).squeeze()
+    point /= point[3]
+    # rotation angle depending on direction
+    cosa = (numpy.trace(R33) - 1.0) / 2.0
+    if abs(direction[2]) > 1e-8:
+        sina = (R[1, 0] + (cosa-1.0)*direction[0]*direction[1]) / direction[2]
+    elif abs(direction[1]) > 1e-8:
+        sina = (R[0, 2] + (cosa-1.0)*direction[0]*direction[2]) / direction[1]
+    else:
+        sina = (R[2, 1] + (cosa-1.0)*direction[1]*direction[2]) / direction[0]
+    angle = math.atan2(sina, cosa)
+    return angle, direction, point
+
+
+def scale_matrix(factor, origin=None, direction=None):
+    """Return matrix to scale by factor around origin in direction.
+
+    Use factor -1 for point symmetry.
+
+    >>> v = (numpy.random.rand(4, 5) - 0.5) * 20.0
+    >>> v[3] = 1.0
+    >>> S = scale_matrix(-1.234)
+    >>> numpy.allclose(numpy.dot(S, v)[:3], -1.234*v[:3])
+    True
+    >>> factor = random.random() * 10 - 5
+    >>> origin = numpy.random.random(3) - 0.5
+    >>> direct = numpy.random.random(3) - 0.5
+    >>> S = scale_matrix(factor, origin)
+    >>> S = scale_matrix(factor, origin, direct)
+
+    """
+    if direction is None:
+        # uniform scaling
+        M = numpy.array(((factor, 0.0,    0.0,    0.0),
+                         (0.0,    factor, 0.0,    0.0),
+                         (0.0,    0.0,    factor, 0.0),
+                         (0.0,    0.0,    0.0,    1.0)), dtype=numpy.float64)
+        if origin is not None:
+            M[:3, 3] = origin[:3]
+            M[:3, 3] *= 1.0 - factor
+    else:
+        # nonuniform scaling
+        direction = unit_vector(direction[:3])
+        factor = 1.0 - factor
+        M = numpy.identity(4)
+        M[:3, :3] -= factor * numpy.outer(direction, direction)
+        if origin is not None:
+            M[:3, 3] = (factor * numpy.dot(origin[:3], direction)) * direction
+    return M
+
+
+def scale_from_matrix(matrix):
+    """Return scaling factor, origin and direction from scaling matrix.
+
+    >>> factor = random.random() * 10 - 5
+    >>> origin = numpy.random.random(3) - 0.5
+    >>> direct = numpy.random.random(3) - 0.5
+    >>> S0 = scale_matrix(factor, origin)
+    >>> factor, origin, direction = scale_from_matrix(S0)
+    >>> S1 = scale_matrix(factor, origin, direction)
+    >>> is_same_transform(S0, S1)
+    True
+    >>> S0 = scale_matrix(factor, origin, direct)
+    >>> factor, origin, direction = scale_from_matrix(S0)
+    >>> S1 = scale_matrix(factor, origin, direction)
+    >>> is_same_transform(S0, S1)
+    True
+
+    """
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)
+    M33 = M[:3, :3]
+    factor = numpy.trace(M33) - 2.0
+    try:
+        # direction: unit eigenvector corresponding to eigenvalue factor
+        l, V = numpy.linalg.eig(M33)
+        i = numpy.where(abs(numpy.real(l) - factor) < 1e-8)[0][0]
+        direction = numpy.real(V[:, i]).squeeze()
+        direction /= vector_norm(direction)
+    except IndexError:
+        # uniform scaling
+        factor = (factor + 2.0) / 3.0
+        direction = None
+    # origin: any eigenvector corresponding to eigenvalue 1
+    l, V = numpy.linalg.eig(M)
+    i = numpy.where(abs(numpy.real(l) - 1.0) < 1e-8)[0]
+    if not len(i):
+        raise ValueError("no eigenvector corresponding to eigenvalue 1")
+    origin = numpy.real(V[:, i[-1]]).squeeze()
+    origin /= origin[3]
+    return factor, origin, direction
+
+
+def projection_matrix(point, normal, direction=None,
+                      perspective=None, pseudo=False):
+    """Return matrix to project onto plane defined by point and normal.
+
+    Using either perspective point, projection direction, or none of both.
+
+    If pseudo is True, perspective projections will preserve relative depth
+    such that Perspective = dot(Orthogonal, PseudoPerspective).
+
+    >>> P = projection_matrix((0, 0, 0), (1, 0, 0))
+    >>> numpy.allclose(P[1:, 1:], numpy.identity(4)[1:, 1:])
+    True
+    >>> point = numpy.random.random(3) - 0.5
+    >>> normal = numpy.random.random(3) - 0.5
+    >>> direct = numpy.random.random(3) - 0.5
+    >>> persp = numpy.random.random(3) - 0.5
+    >>> P0 = projection_matrix(point, normal)
+    >>> P1 = projection_matrix(point, normal, direction=direct)
+    >>> P2 = projection_matrix(point, normal, perspective=persp)
+    >>> P3 = projection_matrix(point, normal, perspective=persp, pseudo=True)
+    >>> is_same_transform(P2, numpy.dot(P0, P3))
+    True
+    >>> P = projection_matrix((3, 0, 0), (1, 1, 0), (1, 0, 0))
+    >>> v0 = (numpy.random.rand(4, 5) - 0.5) * 20.0
+    >>> v0[3] = 1.0
+    >>> v1 = numpy.dot(P, v0)
+    >>> numpy.allclose(v1[1], v0[1])
+    True
+    >>> numpy.allclose(v1[0], 3.0-v1[1])
+    True
+
+    """
+    M = numpy.identity(4)
+    point = numpy.array(point[:3], dtype=numpy.float64, copy=False)
+    normal = unit_vector(normal[:3])
+    if perspective is not None:
+        # perspective projection
+        perspective = numpy.array(perspective[:3], dtype=numpy.float64,
+                                  copy=False)
+        M[0, 0] = M[1, 1] = M[2, 2] = numpy.dot(perspective-point, normal)
+        M[:3, :3] -= numpy.outer(perspective, normal)
+        if pseudo:
+            # preserve relative depth
+            M[:3, :3] -= numpy.outer(normal, normal)
+            M[:3, 3] = numpy.dot(point, normal) * (perspective+normal)
+        else:
+            M[:3, 3] = numpy.dot(point, normal) * perspective
+        M[3, :3] = -normal
+        M[3, 3] = numpy.dot(perspective, normal)
+    elif direction is not None:
+        # parallel projection
+        direction = numpy.array(direction[:3], dtype=numpy.float64, copy=False)
+        scale = numpy.dot(direction, normal)
+        M[:3, :3] -= numpy.outer(direction, normal) / scale
+        M[:3, 3] = direction * (numpy.dot(point, normal) / scale)
+    else:
+        # orthogonal projection
+        M[:3, :3] -= numpy.outer(normal, normal)
+        M[:3, 3] = numpy.dot(point, normal) * normal
+    return M
+
+
+def projection_from_matrix(matrix, pseudo=False):
+    """Return projection plane and perspective point from projection matrix.
+
+    Return values are same as arguments for projection_matrix function:
+    point, normal, direction, perspective, and pseudo.
+
+    >>> point = numpy.random.random(3) - 0.5
+    >>> normal = numpy.random.random(3) - 0.5
+    >>> direct = numpy.random.random(3) - 0.5
+    >>> persp = numpy.random.random(3) - 0.5
+    >>> P0 = projection_matrix(point, normal)
+    >>> result = projection_from_matrix(P0)
+    >>> P1 = projection_matrix(*result)
+    >>> is_same_transform(P0, P1)
+    True
+    >>> P0 = projection_matrix(point, normal, direct)
+    >>> result = projection_from_matrix(P0)
+    >>> P1 = projection_matrix(*result)
+    >>> is_same_transform(P0, P1)
+    True
+    >>> P0 = projection_matrix(point, normal, perspective=persp, pseudo=False)
+    >>> result = projection_from_matrix(P0, pseudo=False)
+    >>> P1 = projection_matrix(*result)
+    >>> is_same_transform(P0, P1)
+    True
+    >>> P0 = projection_matrix(point, normal, perspective=persp, pseudo=True)
+    >>> result = projection_from_matrix(P0, pseudo=True)
+    >>> P1 = projection_matrix(*result)
+    >>> is_same_transform(P0, P1)
+    True
+
+    """
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)
+    M33 = M[:3, :3]
+    l, V = numpy.linalg.eig(M)
+    i = numpy.where(abs(numpy.real(l) - 1.0) < 1e-8)[0]
+    if not pseudo and len(i):
+        # point: any eigenvector corresponding to eigenvalue 1
+        point = numpy.real(V[:, i[-1]]).squeeze()
+        point /= point[3]
+        # direction: unit eigenvector corresponding to eigenvalue 0
+        l, V = numpy.linalg.eig(M33)
+        i = numpy.where(abs(numpy.real(l)) < 1e-8)[0]
+        if not len(i):
+            raise ValueError("no eigenvector corresponding to eigenvalue 0")
+        direction = numpy.real(V[:, i[0]]).squeeze()
+        direction /= vector_norm(direction)
+        # normal: unit eigenvector of M33.T corresponding to eigenvalue 0
+        l, V = numpy.linalg.eig(M33.T)
+        i = numpy.where(abs(numpy.real(l)) < 1e-8)[0]
+        if len(i):
+            # parallel projection
+            normal = numpy.real(V[:, i[0]]).squeeze()
+            normal /= vector_norm(normal)
+            return point, normal, direction, None, False
+        else:
+            # orthogonal projection, where normal equals direction vector
+            return point, direction, None, None, False
+    else:
+        # perspective projection
+        i = numpy.where(abs(numpy.real(l)) > 1e-8)[0]
+        if not len(i):
+            raise ValueError(
+                "no eigenvector not corresponding to eigenvalue 0")
+        point = numpy.real(V[:, i[-1]]).squeeze()
+        point /= point[3]
+        normal = - M[3, :3]
+        perspective = M[:3, 3] / numpy.dot(point[:3], normal)
+        if pseudo:
+            perspective -= normal
+        return point, normal, None, perspective, pseudo
+
+
+def clip_matrix(left, right, bottom, top, near, far, perspective=False):
+    """Return matrix to obtain normalized device coordinates from frustrum.
+
+    The frustrum bounds are axis-aligned along x (left, right),
+    y (bottom, top) and z (near, far).
+
+    Normalized device coordinates are in range [-1, 1] if coordinates are
+    inside the frustrum.
+
+    If perspective is True the frustrum is a truncated pyramid with the
+    perspective point at origin and direction along z axis, otherwise an
+    orthographic canonical view volume (a box).
+
+    Homogeneous coordinates transformed by the perspective clip matrix
+    need to be dehomogenized (devided by w coordinate).
+
+    >>> frustrum = numpy.random.rand(6)
+    >>> frustrum[1] += frustrum[0]
+    >>> frustrum[3] += frustrum[2]
+    >>> frustrum[5] += frustrum[4]
+    >>> M = clip_matrix(*frustrum, perspective=False)
+    >>> numpy.dot(M, [frustrum[0], frustrum[2], frustrum[4], 1.0])
+    array([-1., -1., -1.,  1.])
+    >>> numpy.dot(M, [frustrum[1], frustrum[3], frustrum[5], 1.0])
+    array([ 1.,  1.,  1.,  1.])
+    >>> M = clip_matrix(*frustrum, perspective=True)
+    >>> v = numpy.dot(M, [frustrum[0], frustrum[2], frustrum[4], 1.0])
+    >>> v / v[3]
+    array([-1., -1., -1.,  1.])
+    >>> v = numpy.dot(M, [frustrum[1], frustrum[3], frustrum[4], 1.0])
+    >>> v / v[3]
+    array([ 1.,  1., -1.,  1.])
+
+    """
+    if left >= right or bottom >= top or near >= far:
+        raise ValueError("invalid frustrum")
+    if perspective:
+        if near <= _EPS:
+            raise ValueError("invalid frustrum: near <= 0")
+        t = 2.0 * near
+        M = ((-t/(right-left), 0.0, (right+left)/(right-left), 0.0),
+             (0.0, -t/(top-bottom), (top+bottom)/(top-bottom), 0.0),
+             (0.0, 0.0, -(far+near)/(far-near), t*far/(far-near)),
+             (0.0, 0.0, -1.0, 0.0))
+    else:
+        M = ((2.0/(right-left), 0.0, 0.0, (right+left)/(left-right)),
+             (0.0, 2.0/(top-bottom), 0.0, (top+bottom)/(bottom-top)),
+             (0.0, 0.0, 2.0/(far-near), (far+near)/(near-far)),
+             (0.0, 0.0, 0.0, 1.0))
+    return numpy.array(M, dtype=numpy.float64)
+
+
+def shear_matrix(angle, direction, point, normal):
+    """Return matrix to shear by angle along direction vector on shear plane.
+
+    The shear plane is defined by a point and normal vector. The direction
+    vector must be orthogonal to the plane's normal vector.
+
+    A point P is transformed by the shear matrix into P" such that
+    the vector P-P" is parallel to the direction vector and its extent is
+    given by the angle of P-P'-P", where P' is the orthogonal projection
+    of P onto the shear plane.
+
+    >>> angle = (random.random() - 0.5) * 4*math.pi
+    >>> direct = numpy.random.random(3) - 0.5
+    >>> point = numpy.random.random(3) - 0.5
+    >>> normal = numpy.cross(direct, numpy.random.random(3))
+    >>> S = shear_matrix(angle, direct, point, normal)
+    >>> numpy.allclose(1.0, numpy.linalg.det(S))
+    True
+
+    """
+    normal = unit_vector(normal[:3])
+    direction = unit_vector(direction[:3])
+    if abs(numpy.dot(normal, direction)) > 1e-6:
+        raise ValueError("direction and normal vectors are not orthogonal")
+    angle = math.tan(angle)
+    M = numpy.identity(4)
+    M[:3, :3] += angle * numpy.outer(direction, normal)
+    M[:3, 3] = -angle * numpy.dot(point[:3], normal) * direction
+    return M
+
+
+def shear_from_matrix(matrix):
+    """Return shear angle, direction and plane from shear matrix.
+
+    >>> angle = (random.random() - 0.5) * 4*math.pi
+    >>> direct = numpy.random.random(3) - 0.5
+    >>> point = numpy.random.random(3) - 0.5
+    >>> normal = numpy.cross(direct, numpy.random.random(3))
+    >>> S0 = shear_matrix(angle, direct, point, normal)
+    >>> angle, direct, point, normal = shear_from_matrix(S0)
+    >>> S1 = shear_matrix(angle, direct, point, normal)
+    >>> is_same_transform(S0, S1)
+    True
+
+    """
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)
+    M33 = M[:3, :3]
+    # normal: cross independent eigenvectors corresponding to the eigenvalue 1
+    l, V = numpy.linalg.eig(M33)
+    i = numpy.where(abs(numpy.real(l) - 1.0) < 1e-4)[0]
+    if len(i) < 2:
+        raise ValueError("No two linear independent eigenvectors found %s" % l)
+    V = numpy.real(V[:, i]).squeeze().T
+    lenorm = -1.0
+    for i0, i1 in ((0, 1), (0, 2), (1, 2)):
+        n = numpy.cross(V[i0], V[i1])
+        l = vector_norm(n)
+        if l > lenorm:
+            lenorm = l
+            normal = n
+    normal /= lenorm
+    # direction and angle
+    direction = numpy.dot(M33 - numpy.identity(3), normal)
+    angle = vector_norm(direction)
+    direction /= angle
+    angle = math.atan(angle)
+    # point: eigenvector corresponding to eigenvalue 1
+    l, V = numpy.linalg.eig(M)
+    i = numpy.where(abs(numpy.real(l) - 1.0) < 1e-8)[0]
+    if not len(i):
+        raise ValueError("no eigenvector corresponding to eigenvalue 1")
+    point = numpy.real(V[:, i[-1]]).squeeze()
+    point /= point[3]
+    return angle, direction, point, normal
+
+
+def decompose_matrix(matrix):
+    """Return sequence of transformations from transformation matrix.
+
+    matrix : array_like
+        Non-degenerative homogeneous transformation matrix
+
+    Return tuple of:
+        scale : vector of 3 scaling factors
+        shear : list of shear factors for x-y, x-z, y-z axes
+        angles : list of Euler angles about static x, y, z axes
+        translate : translation vector along x, y, z axes
+        perspective : perspective partition of matrix
+
+    Raise ValueError if matrix is of wrong type or degenerative.
+
+    >>> T0 = translation_matrix((1, 2, 3))
+    >>> scale, shear, angles, trans, persp = decompose_matrix(T0)
+    >>> T1 = translation_matrix(trans)
+    >>> numpy.allclose(T0, T1)
+    True
+    >>> S = scale_matrix(0.123)
+    >>> scale, shear, angles, trans, persp = decompose_matrix(S)
+    >>> scale[0]
+    0.123
+    >>> R0 = euler_matrix(1, 2, 3)
+    >>> scale, shear, angles, trans, persp = decompose_matrix(R0)
+    >>> R1 = euler_matrix(*angles)
+    >>> numpy.allclose(R0, R1)
+    True
+
+    """
+    M = numpy.array(matrix, dtype=numpy.float64, copy=True).T
+    if abs(M[3, 3]) < _EPS:
+        raise ValueError("M[3, 3] is zero")
+    M /= M[3, 3]
+    P = M.copy()
+    P[:, 3] = 0, 0, 0, 1
+    if not numpy.linalg.det(P):
+        raise ValueError("Matrix is singular")
+
+    scale = numpy.zeros((3, ), dtype=numpy.float64)
+    shear = [0, 0, 0]
+    angles = [0, 0, 0]
+
+    if any(abs(M[:3, 3]) > _EPS):
+        perspective = numpy.dot(M[:, 3], numpy.linalg.inv(P.T))
+        M[:, 3] = 0, 0, 0, 1
+    else:
+        perspective = numpy.array((0, 0, 0, 1), dtype=numpy.float64)
+
+    translate = M[3, :3].copy()
+    M[3, :3] = 0
+
+    row = M[:3, :3].copy()
+    scale[0] = vector_norm(row[0])
+    row[0] /= scale[0]
+    shear[0] = numpy.dot(row[0], row[1])
+    row[1] -= row[0] * shear[0]
+    scale[1] = vector_norm(row[1])
+    row[1] /= scale[1]
+    shear[0] /= scale[1]
+    shear[1] = numpy.dot(row[0], row[2])
+    row[2] -= row[0] * shear[1]
+    shear[2] = numpy.dot(row[1], row[2])
+    row[2] -= row[1] * shear[2]
+    scale[2] = vector_norm(row[2])
+    row[2] /= scale[2]
+    shear[1:] /= scale[2]
+
+    if numpy.dot(row[0], numpy.cross(row[1], row[2])) < 0:
+        scale *= -1
+        row *= -1
+
+    angles[1] = math.asin(-row[0, 2])
+    if math.cos(angles[1]):
+        angles[0] = math.atan2(row[1, 2], row[2, 2])
+        angles[2] = math.atan2(row[0, 1], row[0, 0])
+    else:
+        #angles[0] = math.atan2(row[1, 0], row[1, 1])
+        angles[0] = math.atan2(-row[2, 1], row[1, 1])
+        angles[2] = 0.0
+
+    return scale, shear, angles, translate, perspective
+
+
+def compose_matrix(scale=None, shear=None, angles=None, translate=None,
+                   perspective=None):
+    """Return transformation matrix from sequence of transformations.
+
+    This is the inverse of the decompose_matrix function.
+
+    Sequence of transformations:
+        scale : vector of 3 scaling factors
+        shear : list of shear factors for x-y, x-z, y-z axes
+        angles : list of Euler angles about static x, y, z axes
+        translate : translation vector along x, y, z axes
+        perspective : perspective partition of matrix
+
+    >>> scale = numpy.random.random(3) - 0.5
+    >>> shear = numpy.random.random(3) - 0.5
+    >>> angles = (numpy.random.random(3) - 0.5) * (2*math.pi)
+    >>> trans = numpy.random.random(3) - 0.5
+    >>> persp = numpy.random.random(4) - 0.5
+    >>> M0 = compose_matrix(scale, shear, angles, trans, persp)
+    >>> result = decompose_matrix(M0)
+    >>> M1 = compose_matrix(*result)
+    >>> is_same_transform(M0, M1)
+    True
+
+    """
+    M = numpy.identity(4)
+    if perspective is not None:
+        P = numpy.identity(4)
+        P[3, :] = perspective[:4]
+        M = numpy.dot(M, P)
+    if translate is not None:
+        T = numpy.identity(4)
+        T[:3, 3] = translate[:3]
+        M = numpy.dot(M, T)
+    if angles is not None:
+        R = euler_matrix(angles[0], angles[1], angles[2], 'sxyz')
+        M = numpy.dot(M, R)
+    if shear is not None:
+        Z = numpy.identity(4)
+        Z[1, 2] = shear[2]
+        Z[0, 2] = shear[1]
+        Z[0, 1] = shear[0]
+        M = numpy.dot(M, Z)
+    if scale is not None:
+        S = numpy.identity(4)
+        S[0, 0] = scale[0]
+        S[1, 1] = scale[1]
+        S[2, 2] = scale[2]
+        M = numpy.dot(M, S)
+    M /= M[3, 3]
+    return M
+
+
+def orthogonalization_matrix(lengths, angles):
+    """Return orthogonalization matrix for crystallographic cell coordinates.
+
+    Angles are expected in degrees.
+
+    The de-orthogonalization matrix is the inverse.
+
+    >>> O = orthogonalization_matrix((10., 10., 10.), (90., 90., 90.))
+    >>> numpy.allclose(O[:3, :3], numpy.identity(3, float) * 10)
+    True
+    >>> O = orthogonalization_matrix([9.8, 12.0, 15.5], [87.2, 80.7, 69.7])
+    >>> numpy.allclose(numpy.sum(O), 43.063229)
+    True
+
+    """
+    a, b, c = lengths
+    angles = numpy.radians(angles)
+    sina, sinb, _ = numpy.sin(angles)
+    cosa, cosb, cosg = numpy.cos(angles)
+    co = (cosa * cosb - cosg) / (sina * sinb)
+    return numpy.array((
+        ( a*sinb*math.sqrt(1.0-co*co),  0.0,    0.0, 0.0),
+        (-a*sinb*co,                    b*sina, 0.0, 0.0),
+        ( a*cosb,                       b*cosa, c,   0.0),
+        ( 0.0,                          0.0,    0.0, 1.0)),
+        dtype=numpy.float64)
+
+
+def superimposition_matrix(v0, v1, scaling=False, usesvd=True):
+    """Return matrix to transform given vector set into second vector set.
+
+    v0 and v1 are shape (3, *) or (4, *) arrays of at least 3 vectors.
+
+    If usesvd is True, the weighted sum of squared deviations (RMSD) is
+    minimized according to the algorithm by W. Kabsch [8]. Otherwise the
+    quaternion based algorithm by B. Horn [9] is used (slower when using
+    this Python implementation).
+
+    The returned matrix performs rotation, translation and uniform scaling
+    (if specified).
+
+    >>> v0 = numpy.random.rand(3, 10)
+    >>> M = superimposition_matrix(v0, v0)
+    >>> numpy.allclose(M, numpy.identity(4))
+    True
+    >>> R = random_rotation_matrix(numpy.random.random(3))
+    >>> v0 = ((1,0,0), (0,1,0), (0,0,1), (1,1,1))
+    >>> v1 = numpy.dot(R, v0)
+    >>> M = superimposition_matrix(v0, v1)
+    >>> numpy.allclose(v1, numpy.dot(M, v0))
+    True
+    >>> v0 = (numpy.random.rand(4, 100) - 0.5) * 20.0
+    >>> v0[3] = 1.0
+    >>> v1 = numpy.dot(R, v0)
+    >>> M = superimposition_matrix(v0, v1)
+    >>> numpy.allclose(v1, numpy.dot(M, v0))
+    True
+    >>> S = scale_matrix(random.random())
+    >>> T = translation_matrix(numpy.random.random(3)-0.5)
+    >>> M = concatenate_matrices(T, R, S)
+    >>> v1 = numpy.dot(M, v0)
+    >>> v0[:3] += numpy.random.normal(0.0, 1e-9, 300).reshape(3, -1)
+    >>> M = superimposition_matrix(v0, v1, scaling=True)
+    >>> numpy.allclose(v1, numpy.dot(M, v0))
+    True
+    >>> M = superimposition_matrix(v0, v1, scaling=True, usesvd=False)
+    >>> numpy.allclose(v1, numpy.dot(M, v0))
+    True
+    >>> v = numpy.empty((4, 100, 3), dtype=numpy.float64)
+    >>> v[:, :, 0] = v0
+    >>> M = superimposition_matrix(v0, v1, scaling=True, usesvd=False)
+    >>> numpy.allclose(v1, numpy.dot(M, v[:, :, 0]))
+    True
+
+    """
+    v0 = numpy.array(v0, dtype=numpy.float64, copy=False)[:3]
+    v1 = numpy.array(v1, dtype=numpy.float64, copy=False)[:3]
+
+    if v0.shape != v1.shape or v0.shape[1] < 3:
+        raise ValueError("Vector sets are of wrong shape or type.")
+
+    # move centroids to origin
+    t0 = numpy.mean(v0, axis=1)
+    t1 = numpy.mean(v1, axis=1)
+    v0 = v0 - t0.reshape(3, 1)
+    v1 = v1 - t1.reshape(3, 1)
+
+    if usesvd:
+        # Singular Value Decomposition of covariance matrix
+        u, s, vh = numpy.linalg.svd(numpy.dot(v1, v0.T))
+        # rotation matrix from SVD orthonormal bases
+        R = numpy.dot(u, vh)
+        if numpy.linalg.det(R) < 0.0:
+            # R does not constitute right handed system
+            R -= numpy.outer(u[:, 2], vh[2, :]*2.0)
+            s[-1] *= -1.0
+        # homogeneous transformation matrix
+        M = numpy.identity(4)
+        M[:3, :3] = R
+    else:
+        # compute symmetric matrix N
+        xx, yy, zz = numpy.sum(v0 * v1, axis=1)
+        xy, yz, zx = numpy.sum(v0 * numpy.roll(v1, -1, axis=0), axis=1)
+        xz, yx, zy = numpy.sum(v0 * numpy.roll(v1, -2, axis=0), axis=1)
+        N = ((xx+yy+zz, yz-zy,    zx-xz,    xy-yx),
+             (yz-zy,    xx-yy-zz, xy+yx,    zx+xz),
+             (zx-xz,    xy+yx,   -xx+yy-zz, yz+zy),
+             (xy-yx,    zx+xz,    yz+zy,   -xx-yy+zz))
+        # quaternion: eigenvector corresponding to most positive eigenvalue
+        l, V = numpy.linalg.eig(N)
+        q = V[:, numpy.argmax(l)]
+        q /= vector_norm(q) # unit quaternion
+        q = numpy.roll(q, -1) # move w component to end
+        # homogeneous transformation matrix
+        M = quaternion_matrix(q)
+
+    # scale: ratio of rms deviations from centroid
+    if scaling:
+        v0 *= v0
+        v1 *= v1
+        M[:3, :3] *= math.sqrt(numpy.sum(v1) / numpy.sum(v0))
+
+    # translation
+    M[:3, 3] = t1
+    T = numpy.identity(4)
+    T[:3, 3] = -t0
+    M = numpy.dot(M, T)
+    return M
+
+
+def euler_matrix(ai, aj, ak, axes='sxyz'):
+    """Return homogeneous rotation matrix from Euler angles and axis sequence.
+
+    ai, aj, ak : Euler's roll, pitch and yaw angles
+    axes : One of 24 axis sequences as string or encoded tuple
+
+    >>> R = euler_matrix(1, 2, 3, 'syxz')
+    >>> numpy.allclose(numpy.sum(R[0]), -1.34786452)
+    True
+    >>> R = euler_matrix(1, 2, 3, (0, 1, 0, 1))
+    >>> numpy.allclose(numpy.sum(R[0]), -0.383436184)
+    True
+    >>> ai, aj, ak = (4.0*math.pi) * (numpy.random.random(3) - 0.5)
+    >>> for axes in _AXES2TUPLE.keys():
+    ...    R = euler_matrix(ai, aj, ak, axes)
+    >>> for axes in _TUPLE2AXES.keys():
+    ...    R = euler_matrix(ai, aj, ak, axes)
+
+    """
+    try:
+        firstaxis, parity, repetition, frame = _AXES2TUPLE[axes]
+    except (AttributeError, KeyError):
+        _ = _TUPLE2AXES[axes]
+        firstaxis, parity, repetition, frame = axes
+
+    i = firstaxis
+    j = _NEXT_AXIS[i+parity]
+    k = _NEXT_AXIS[i-parity+1]
+
+    if frame:
+        ai, ak = ak, ai
+    if parity:
+        ai, aj, ak = -ai, -aj, -ak
+
+    si, sj, sk = math.sin(ai), math.sin(aj), math.sin(ak)
+    ci, cj, ck = math.cos(ai), math.cos(aj), math.cos(ak)
+    cc, cs = ci*ck, ci*sk
+    sc, ss = si*ck, si*sk
+
+    M = numpy.identity(4)
+    if repetition:
+        M[i, i] = cj
+        M[i, j] = sj*si
+        M[i, k] = sj*ci
+        M[j, i] = sj*sk
+        M[j, j] = -cj*ss+cc
+        M[j, k] = -cj*cs-sc
+        M[k, i] = -sj*ck
+        M[k, j] = cj*sc+cs
+        M[k, k] = cj*cc-ss
+    else:
+        M[i, i] = cj*ck
+        M[i, j] = sj*sc-cs
+        M[i, k] = sj*cc+ss
+        M[j, i] = cj*sk
+        M[j, j] = sj*ss+cc
+        M[j, k] = sj*cs-sc
+        M[k, i] = -sj
+        M[k, j] = cj*si
+        M[k, k] = cj*ci
+    return M
+
+
+def euler_from_matrix(matrix, axes='sxyz'):
+    """Return Euler angles from rotation matrix for specified axis sequence.
+
+    axes : One of 24 axis sequences as string or encoded tuple
+
+    Note that many Euler angle triplets can describe one matrix.
+
+    >>> R0 = euler_matrix(1, 2, 3, 'syxz')
+    >>> al, be, ga = euler_from_matrix(R0, 'syxz')
+    >>> R1 = euler_matrix(al, be, ga, 'syxz')
+    >>> numpy.allclose(R0, R1)
+    True
+    >>> angles = (4.0*math.pi) * (numpy.random.random(3) - 0.5)
+    >>> for axes in _AXES2TUPLE.keys():
+    ...    R0 = euler_matrix(axes=axes, *angles)
+    ...    R1 = euler_matrix(axes=axes, *euler_from_matrix(R0, axes))
+    ...    if not numpy.allclose(R0, R1): print axes, "failed"
+
+    """
+    try:
+        firstaxis, parity, repetition, frame = _AXES2TUPLE[axes.lower()]
+    except (AttributeError, KeyError):
+        _ = _TUPLE2AXES[axes]
+        firstaxis, parity, repetition, frame = axes
+
+    i = firstaxis
+    j = _NEXT_AXIS[i+parity]
+    k = _NEXT_AXIS[i-parity+1]
+
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)[:3, :3]
+    if repetition:
+        sy = math.sqrt(M[i, j]*M[i, j] + M[i, k]*M[i, k])
+        if sy > _EPS:
+            ax = math.atan2( M[i, j],  M[i, k])
+            ay = math.atan2( sy,       M[i, i])
+            az = math.atan2( M[j, i], -M[k, i])
+        else:
+            ax = math.atan2(-M[j, k],  M[j, j])
+            ay = math.atan2( sy,       M[i, i])
+            az = 0.0
+    else:
+        cy = math.sqrt(M[i, i]*M[i, i] + M[j, i]*M[j, i])
+        if cy > _EPS:
+            ax = math.atan2( M[k, j],  M[k, k])
+            ay = math.atan2(-M[k, i],  cy)
+            az = math.atan2( M[j, i],  M[i, i])
+        else:
+            ax = math.atan2(-M[j, k],  M[j, j])
+            ay = math.atan2(-M[k, i],  cy)
+            az = 0.0
+
+    if parity:
+        ax, ay, az = -ax, -ay, -az
+    if frame:
+        ax, az = az, ax
+    return ax, ay, az
+
+
+def euler_from_quaternion(quaternion, axes='sxyz'):
+    """Return Euler angles from quaternion for specified axis sequence.
+
+    >>> angles = euler_from_quaternion([0.06146124, 0, 0, 0.99810947])
+    >>> numpy.allclose(angles, [0.123, 0, 0])
+    True
+
+    """
+    return euler_from_matrix(quaternion_matrix(quaternion), axes)
+
+
+def quaternion_from_euler(ai, aj, ak, axes='sxyz'):
+    """Return quaternion from Euler angles and axis sequence.
+
+    ai, aj, ak : Euler's roll, pitch and yaw angles
+    axes : One of 24 axis sequences as string or encoded tuple
+
+    >>> q = quaternion_from_euler(1, 2, 3, 'ryxz')
+    >>> numpy.allclose(q, [0.310622, -0.718287, 0.444435, 0.435953])
+    True
+
+    """
+    try:
+        firstaxis, parity, repetition, frame = _AXES2TUPLE[axes.lower()]
+    except (AttributeError, KeyError):
+        _ = _TUPLE2AXES[axes]
+        firstaxis, parity, repetition, frame = axes
+
+    i = firstaxis
+    j = _NEXT_AXIS[i+parity]
+    k = _NEXT_AXIS[i-parity+1]
+
+    if frame:
+        ai, ak = ak, ai
+    if parity:
+        aj = -aj
+
+    ai /= 2.0
+    aj /= 2.0
+    ak /= 2.0
+    ci = math.cos(ai)
+    si = math.sin(ai)
+    cj = math.cos(aj)
+    sj = math.sin(aj)
+    ck = math.cos(ak)
+    sk = math.sin(ak)
+    cc = ci*ck
+    cs = ci*sk
+    sc = si*ck
+    ss = si*sk
+
+    quaternion = numpy.empty((4, ), dtype=numpy.float64)
+    if repetition:
+        quaternion[i] = cj*(cs + sc)
+        quaternion[j] = sj*(cc + ss)
+        quaternion[k] = sj*(cs - sc)
+        quaternion[3] = cj*(cc - ss)
+    else:
+        quaternion[i] = cj*sc - sj*cs
+        quaternion[j] = cj*ss + sj*cc
+        quaternion[k] = cj*cs - sj*sc
+        quaternion[3] = cj*cc + sj*ss
+    if parity:
+        quaternion[j] *= -1
+
+    return quaternion
+
+
+def quaternion_about_axis(angle, axis):
+    """Return quaternion for rotation about axis.
+
+    >>> q = quaternion_about_axis(0.123, (1, 0, 0))
+    >>> numpy.allclose(q, [0.06146124, 0, 0, 0.99810947])
+    True
+
+    """
+    quaternion = numpy.zeros((4, ), dtype=numpy.float64)
+    quaternion[:3] = axis[:3]
+    qlen = vector_norm(quaternion)
+    if qlen > _EPS:
+        quaternion *= math.sin(angle/2.0) / qlen
+    quaternion[3] = math.cos(angle/2.0)
+    return quaternion
+
+
+def quaternion_matrix(quaternion):
+    """Return homogeneous rotation matrix from quaternion.
+
+    >>> R = quaternion_matrix([0.06146124, 0, 0, 0.99810947])
+    >>> numpy.allclose(R, rotation_matrix(0.123, (1, 0, 0)))
+    True
+
+    """
+    q = numpy.array(quaternion[:4], dtype=numpy.float64, copy=True)
+    nq = numpy.dot(q, q)
+    if nq < _EPS:
+        return numpy.identity(4)
+    q *= math.sqrt(2.0 / nq)
+    q = numpy.outer(q, q)
+    return numpy.array((
+        (1.0-q[1, 1]-q[2, 2],     q[0, 1]-q[2, 3],     q[0, 2]+q[1, 3], 0.0),
+        (    q[0, 1]+q[2, 3], 1.0-q[0, 0]-q[2, 2],     q[1, 2]-q[0, 3], 0.0),
+        (    q[0, 2]-q[1, 3],     q[1, 2]+q[0, 3], 1.0-q[0, 0]-q[1, 1], 0.0),
+        (                0.0,                 0.0,                 0.0, 1.0)
+        ), dtype=numpy.float64)
+
+
+def quaternion_from_matrix(matrix):
+    """Return quaternion from rotation matrix.
+
+    >>> R = rotation_matrix(0.123, (1, 2, 3))
+    >>> q = quaternion_from_matrix(R)
+    >>> numpy.allclose(q, [0.0164262, 0.0328524, 0.0492786, 0.9981095])
+    True
+
+    """
+    q = numpy.empty((4, ), dtype=numpy.float64)
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)[:4, :4]
+    t = numpy.trace(M)
+    if t > M[3, 3]:
+        q[3] = t
+        q[2] = M[1, 0] - M[0, 1]
+        q[1] = M[0, 2] - M[2, 0]
+        q[0] = M[2, 1] - M[1, 2]
+    else:
+        i, j, k = 0, 1, 2
+        if M[1, 1] > M[0, 0]:
+            i, j, k = 1, 2, 0
+        if M[2, 2] > M[i, i]:
+            i, j, k = 2, 0, 1
+        t = M[i, i] - (M[j, j] + M[k, k]) + M[3, 3]
+        q[i] = t
+        q[j] = M[i, j] + M[j, i]
+        q[k] = M[k, i] + M[i, k]
+        q[3] = M[k, j] - M[j, k]
+    q *= 0.5 / math.sqrt(t * M[3, 3])
+    return q
+
+
+def quaternion_multiply(quaternion1, quaternion0):
+    """Return multiplication of two quaternions.
+
+    >>> q = quaternion_multiply([1, -2, 3, 4], [-5, 6, 7, 8])
+    >>> numpy.allclose(q, [-44, -14, 48, 28])
+    True
+
+    """
+    x0, y0, z0, w0 = quaternion0
+    x1, y1, z1, w1 = quaternion1
+    return numpy.array((
+         x1*w0 + y1*z0 - z1*y0 + w1*x0,
+        -x1*z0 + y1*w0 + z1*x0 + w1*y0,
+         x1*y0 - y1*x0 + z1*w0 + w1*z0,
+        -x1*x0 - y1*y0 - z1*z0 + w1*w0), dtype=numpy.float64)
+
+
+def quaternion_conjugate(quaternion):
+    """Return conjugate of quaternion.
+
+    >>> q0 = random_quaternion()
+    >>> q1 = quaternion_conjugate(q0)
+    >>> q1[3] == q0[3] and all(q1[:3] == -q0[:3])
+    True
+
+    """
+    return numpy.array((-quaternion[0], -quaternion[1],
+                        -quaternion[2], quaternion[3]), dtype=numpy.float64)
+
+
+def quaternion_inverse(quaternion):
+    """Return inverse of quaternion.
+
+    >>> q0 = random_quaternion()
+    >>> q1 = quaternion_inverse(q0)
+    >>> numpy.allclose(quaternion_multiply(q0, q1), [0, 0, 0, 1])
+    True
+
+    """
+    return quaternion_conjugate(quaternion) / numpy.dot(quaternion, quaternion)
+
+
+def quaternion_slerp(quat0, quat1, fraction, spin=0, shortestpath=True):
+    """Return spherical linear interpolation between two quaternions.
+
+    >>> q0 = random_quaternion()
+    >>> q1 = random_quaternion()
+    >>> q = quaternion_slerp(q0, q1, 0.0)
+    >>> numpy.allclose(q, q0)
+    True
+    >>> q = quaternion_slerp(q0, q1, 1.0, 1)
+    >>> numpy.allclose(q, q1)
+    True
+    >>> q = quaternion_slerp(q0, q1, 0.5)
+    >>> angle = math.acos(numpy.dot(q0, q))
+    >>> numpy.allclose(2.0, math.acos(numpy.dot(q0, q1)) / angle) or \
+        numpy.allclose(2.0, math.acos(-numpy.dot(q0, q1)) / angle)
+    True
+
+    """
+    q0 = unit_vector(quat0[:4])
+    q1 = unit_vector(quat1[:4])
+    if fraction == 0.0:
+        return q0
+    elif fraction == 1.0:
+        return q1
+    d = numpy.dot(q0, q1)
+    if abs(abs(d) - 1.0) < _EPS:
+        return q0
+    if shortestpath and d < 0.0:
+        # invert rotation
+        d = -d
+        q1 *= -1.0
+    angle = math.acos(d) + spin * math.pi
+    if abs(angle) < _EPS:
+        return q0
+    isin = 1.0 / math.sin(angle)
+    q0 *= math.sin((1.0 - fraction) * angle) * isin
+    q1 *= math.sin(fraction * angle) * isin
+    q0 += q1
+    return q0
+
+
+def random_quaternion(rand=None):
+    """Return uniform random unit quaternion.
+
+    rand: array like or None
+        Three independent random variables that are uniformly distributed
+        between 0 and 1.
+
+    >>> q = random_quaternion()
+    >>> numpy.allclose(1.0, vector_norm(q))
+    True
+    >>> q = random_quaternion(numpy.random.random(3))
+    >>> q.shape
+    (4,)
+
+    """
+    if rand is None:
+        rand = numpy.random.rand(3)
+    else:
+        assert len(rand) == 3
+    r1 = numpy.sqrt(1.0 - rand[0])
+    r2 = numpy.sqrt(rand[0])
+    pi2 = math.pi * 2.0
+    t1 = pi2 * rand[1]
+    t2 = pi2 * rand[2]
+    return numpy.array((numpy.sin(t1)*r1,
+                        numpy.cos(t1)*r1,
+                        numpy.sin(t2)*r2,
+                        numpy.cos(t2)*r2), dtype=numpy.float64)
+
+
+def random_rotation_matrix(rand=None):
+    """Return uniform random rotation matrix.
+
+    rnd: array like
+        Three independent random variables that are uniformly distributed
+        between 0 and 1 for each returned quaternion.
+
+    >>> R = random_rotation_matrix()
+    >>> numpy.allclose(numpy.dot(R.T, R), numpy.identity(4))
+    True
+
+    """
+    return quaternion_matrix(random_quaternion(rand))
+
+
+class Arcball(object):
+    """Virtual Trackball Control.
+
+    >>> ball = Arcball()
+    >>> ball = Arcball(initial=numpy.identity(4))
+    >>> ball.place([320, 320], 320)
+    >>> ball.down([500, 250])
+    >>> ball.drag([475, 275])
+    >>> R = ball.matrix()
+    >>> numpy.allclose(numpy.sum(R), 3.90583455)
+    True
+    >>> ball = Arcball(initial=[0, 0, 0, 1])
+    >>> ball.place([320, 320], 320)
+    >>> ball.setaxes([1,1,0], [-1, 1, 0])
+    >>> ball.setconstrain(True)
+    >>> ball.down([400, 200])
+    >>> ball.drag([200, 400])
+    >>> R = ball.matrix()
+    >>> numpy.allclose(numpy.sum(R), 0.2055924)
+    True
+    >>> ball.next()
+
+    """
+
+    def __init__(self, initial=None):
+        """Initialize virtual trackball control.
+
+        initial : quaternion or rotation matrix
+
+        """
+        self._axis = None
+        self._axes = None
+        self._radius = 1.0
+        self._center = [0.0, 0.0]
+        self._vdown = numpy.array([0, 0, 1], dtype=numpy.float64)
+        self._constrain = False
+
+        if initial is None:
+            self._qdown = numpy.array([0, 0, 0, 1], dtype=numpy.float64)
+        else:
+            initial = numpy.array(initial, dtype=numpy.float64)
+            if initial.shape == (4, 4):
+                self._qdown = quaternion_from_matrix(initial)
+            elif initial.shape == (4, ):
+                initial /= vector_norm(initial)
+                self._qdown = initial
+            else:
+                raise ValueError("initial not a quaternion or matrix.")
+
+        self._qnow = self._qpre = self._qdown
+
+    def place(self, center, radius):
+        """Place Arcball, e.g. when window size changes.
+
+        center : sequence[2]
+            Window coordinates of trackball center.
+        radius : float
+            Radius of trackball in window coordinates.
+
+        """
+        self._radius = float(radius)
+        self._center[0] = center[0]
+        self._center[1] = center[1]
+
+    def setaxes(self, *axes):
+        """Set axes to constrain rotations."""
+        if axes is None:
+            self._axes = None
+        else:
+            self._axes = [unit_vector(axis) for axis in axes]
+
+    def setconstrain(self, constrain):
+        """Set state of constrain to axis mode."""
+        self._constrain = constrain == True
+
+    def getconstrain(self):
+        """Return state of constrain to axis mode."""
+        return self._constrain
+
+    def down(self, point):
+        """Set initial cursor window coordinates and pick constrain-axis."""
+        self._vdown = arcball_map_to_sphere(point, self._center, self._radius)
+        self._qdown = self._qpre = self._qnow
+
+        if self._constrain and self._axes is not None:
+            self._axis = arcball_nearest_axis(self._vdown, self._axes)
+            self._vdown = arcball_constrain_to_axis(self._vdown, self._axis)
+        else:
+            self._axis = None
+
+    def drag(self, point):
+        """Update current cursor window coordinates."""
+        vnow = arcball_map_to_sphere(point, self._center, self._radius)
+
+        if self._axis is not None:
+            vnow = arcball_constrain_to_axis(vnow, self._axis)
+
+        self._qpre = self._qnow
+
+        t = numpy.cross(self._vdown, vnow)
+        if numpy.dot(t, t) < _EPS:
+            self._qnow = self._qdown
+        else:
+            q = [t[0], t[1], t[2], numpy.dot(self._vdown, vnow)]
+            self._qnow = quaternion_multiply(q, self._qdown)
+
+    def next(self, acceleration=0.0):
+        """Continue rotation in direction of last drag."""
+        q = quaternion_slerp(self._qpre, self._qnow, 2.0+acceleration, False)
+        self._qpre, self._qnow = self._qnow, q
+
+    def matrix(self):
+        """Return homogeneous rotation matrix."""
+        return quaternion_matrix(self._qnow)
+
+
+def arcball_map_to_sphere(point, center, radius):
+    """Return unit sphere coordinates from window coordinates."""
+    v = numpy.array(((point[0] - center[0]) / radius,
+                     (center[1] - point[1]) / radius,
+                     0.0), dtype=numpy.float64)
+    n = v[0]*v[0] + v[1]*v[1]
+    if n > 1.0:
+        v /= math.sqrt(n) # position outside of sphere
+    else:
+        v[2] = math.sqrt(1.0 - n)
+    return v
+
+
+def arcball_constrain_to_axis(point, axis):
+    """Return sphere point perpendicular to axis."""
+    v = numpy.array(point, dtype=numpy.float64, copy=True)
+    a = numpy.array(axis, dtype=numpy.float64, copy=True)
+    v -= a * numpy.dot(a, v) # on plane
+    n = vector_norm(v)
+    if n > _EPS:
+        if v[2] < 0.0:
+            v *= -1.0
+        v /= n
+        return v
+    if a[2] == 1.0:
+        return numpy.array([1, 0, 0], dtype=numpy.float64)
+    return unit_vector([-a[1], a[0], 0])
+
+
+def arcball_nearest_axis(point, axes):
+    """Return axis, which arc is nearest to point."""
+    point = numpy.array(point, dtype=numpy.float64, copy=False)
+    nearest = None
+    mx = -1.0
+    for axis in axes:
+        t = numpy.dot(arcball_constrain_to_axis(point, axis), point)
+        if t > mx:
+            nearest = axis
+            mx = t
+    return nearest
+
+
+# epsilon for testing whether a number is close to zero
+_EPS = numpy.finfo(float).eps * 4.0
+
+# axis sequences for Euler angles
+_NEXT_AXIS = [1, 2, 0, 1]
+
+# map axes strings to/from tuples of inner axis, parity, repetition, frame
+_AXES2TUPLE = {
+    'sxyz': (0, 0, 0, 0), 'sxyx': (0, 0, 1, 0), 'sxzy': (0, 1, 0, 0),
+    'sxzx': (0, 1, 1, 0), 'syzx': (1, 0, 0, 0), 'syzy': (1, 0, 1, 0),
+    'syxz': (1, 1, 0, 0), 'syxy': (1, 1, 1, 0), 'szxy': (2, 0, 0, 0),
+    'szxz': (2, 0, 1, 0), 'szyx': (2, 1, 0, 0), 'szyz': (2, 1, 1, 0),
+    'rzyx': (0, 0, 0, 1), 'rxyx': (0, 0, 1, 1), 'ryzx': (0, 1, 0, 1),
+    'rxzx': (0, 1, 1, 1), 'rxzy': (1, 0, 0, 1), 'ryzy': (1, 0, 1, 1),
+    'rzxy': (1, 1, 0, 1), 'ryxy': (1, 1, 1, 1), 'ryxz': (2, 0, 0, 1),
+    'rzxz': (2, 0, 1, 1), 'rxyz': (2, 1, 0, 1), 'rzyz': (2, 1, 1, 1)}
+
+_TUPLE2AXES = dict((v, k) for k, v in _AXES2TUPLE.items())
+
+# helper functions
+
+def vector_norm(data, axis=None, out=None):
+    """Return length, i.e. eucledian norm, of ndarray along axis.
+
+    >>> v = numpy.random.random(3)
+    >>> n = vector_norm(v)
+    >>> numpy.allclose(n, numpy.linalg.norm(v))
+    True
+    >>> v = numpy.random.rand(6, 5, 3)
+    >>> n = vector_norm(v, axis=-1)
+    >>> numpy.allclose(n, numpy.sqrt(numpy.sum(v*v, axis=2)))
+    True
+    >>> n = vector_norm(v, axis=1)
+    >>> numpy.allclose(n, numpy.sqrt(numpy.sum(v*v, axis=1)))
+    True
+    >>> v = numpy.random.rand(5, 4, 3)
+    >>> n = numpy.empty((5, 3), dtype=numpy.float64)
+    >>> vector_norm(v, axis=1, out=n)
+    >>> numpy.allclose(n, numpy.sqrt(numpy.sum(v*v, axis=1)))
+    True
+    >>> vector_norm([])
+    0.0
+    >>> vector_norm([1.0])
+    1.0
+
+    """
+    data = numpy.array(data, dtype=numpy.float64, copy=True)
+    if out is None:
+        if data.ndim == 1:
+            return math.sqrt(numpy.dot(data, data))
+        data *= data
+        out = numpy.atleast_1d(numpy.sum(data, axis=axis))
+        numpy.sqrt(out, out)
+        return out
+    else:
+        data *= data
+        numpy.sum(data, axis=axis, out=out)
+        numpy.sqrt(out, out)
+
+
+def unit_vector(data, axis=None, out=None):
+    """Return ndarray normalized by length, i.e. eucledian norm, along axis.
+
+    >>> v0 = numpy.random.random(3)
+    >>> v1 = unit_vector(v0)
+    >>> numpy.allclose(v1, v0 / numpy.linalg.norm(v0))
+    True
+    >>> v0 = numpy.random.rand(5, 4, 3)
+    >>> v1 = unit_vector(v0, axis=-1)
+    >>> v2 = v0 / numpy.expand_dims(numpy.sqrt(numpy.sum(v0*v0, axis=2)), 2)
+    >>> numpy.allclose(v1, v2)
+    True
+    >>> v1 = unit_vector(v0, axis=1)
+    >>> v2 = v0 / numpy.expand_dims(numpy.sqrt(numpy.sum(v0*v0, axis=1)), 1)
+    >>> numpy.allclose(v1, v2)
+    True
+    >>> v1 = numpy.empty((5, 4, 3), dtype=numpy.float64)
+    >>> unit_vector(v0, axis=1, out=v1)
+    >>> numpy.allclose(v1, v2)
+    True
+    >>> list(unit_vector([]))
+    []
+    >>> list(unit_vector([1.0]))
+    [1.0]
+
+    """
+    if out is None:
+        data = numpy.array(data, dtype=numpy.float64, copy=True)
+        if data.ndim == 1:
+            data /= math.sqrt(numpy.dot(data, data))
+            return data
+    else:
+        if out is not data:
+            out[:] = numpy.array(data, copy=False)
+        data = out
+    length = numpy.atleast_1d(numpy.sum(data*data, axis))
+    numpy.sqrt(length, length)
+    if axis is not None:
+        length = numpy.expand_dims(length, axis)
+    data /= length
+    if out is None:
+        return data
+
+
+def random_vector(size):
+    """Return array of random doubles in the half-open interval [0.0, 1.0).
+
+    >>> v = random_vector(10000)
+    >>> numpy.all(v >= 0.0) and numpy.all(v < 1.0)
+    True
+    >>> v0 = random_vector(10)
+    >>> v1 = random_vector(10)
+    >>> numpy.any(v0 == v1)
+    False
+
+    """
+    return numpy.random.random(size)
+
+
+def inverse_matrix(matrix):
+    """Return inverse of square transformation matrix.
+
+    >>> M0 = random_rotation_matrix()
+    >>> M1 = inverse_matrix(M0.T)
+    >>> numpy.allclose(M1, numpy.linalg.inv(M0.T))
+    True
+    >>> for size in range(1, 7):
+    ...     M0 = numpy.random.rand(size, size)
+    ...     M1 = inverse_matrix(M0)
+    ...     if not numpy.allclose(M1, numpy.linalg.inv(M0)): print size
+
+    """
+    return numpy.linalg.inv(matrix)
+
+
+def concatenate_matrices(*matrices):
+    """Return concatenation of series of transformation matrices.
+
+    >>> M = numpy.random.rand(16).reshape((4, 4)) - 0.5
+    >>> numpy.allclose(M, concatenate_matrices(M))
+    True
+    >>> numpy.allclose(numpy.dot(M, M.T), concatenate_matrices(M, M.T))
+    True
+
+    """
+    M = numpy.identity(4)
+    for i in matrices:
+        M = numpy.dot(M, i)
+    return M
+
+
+def is_same_transform(matrix0, matrix1):
+    """Return True if two matrices perform same transformation.
+
+    >>> is_same_transform(numpy.identity(4), numpy.identity(4))
+    True
+    >>> is_same_transform(numpy.identity(4), random_rotation_matrix())
+    False
+
+    """
+    matrix0 = numpy.array(matrix0, dtype=numpy.float64, copy=True)
+    matrix0 /= matrix0[3, 3]
+    matrix1 = numpy.array(matrix1, dtype=numpy.float64, copy=True)
+    matrix1 /= matrix1[3, 3]
+    return numpy.allclose(matrix0, matrix1)
```

### Comparing `robodyno-1.6.0/src/robodyno.egg-info/PKG-INFO` & `robodyno-1.6.1b0/src/robodyno.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,535 +1,535 @@
-Metadata-Version: 2.1
-Name: robodyno
-Version: 1.6.0
-Summary: The Robodyno Robot SDK for Python 3
-Home-page: http://101.42.250.169/
-Author: song
-Author-email: zhaosongy@126.com
-Maintainer: robottime
-Maintainer-email: lab@robottime.cn
-License: MIT License
-Keywords: robodyno,robot,robot module
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Framework :: Robot Framework
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# Robodyno
-
-## 安装
-[安装Python(>=3.7)](https://www.python.org/downloads/)
-
-使用pip安装robodyno库
-
-```
-pip install robodyno
-````
-
-## Python API
-
-### 1. 初始化电机对象
-
-```python
-from robodyno.components import Motor
-from robodyno.interfaces import CanBus
-can = CanBus()
-motor = Motor(can, 0x10)
-```
-`Motor(iface, id, type)`  
-参数 ：
-- iface : robodyno 接口对象
-- id : 电机ID（ 范围从 0x01 到 0x3F ）
-- type : 电机的类型，默认自动识别
-    - ROBODYNO_PRO_44
-    - ROBODYNO_PRO_12
-    - ROBODYNO_PRO_50
-    - ROBODYNO_PRO_100
-
-### 2. 读取电机状态
-
-```python
-motor.state
-```
-`state`  
-返回值 ：
-- 电机状态 （1-空闲，8-使能）
-
-### 3. 读取电机错误
-
-```python
-motor.error
-```
-`error`  
-返回值 :  
-- 电机错误 dict  
-    - error : 错误码（1-电压不足，14-急停）  
-    - motor : 电机相关错误码  
-    - encoder_err : 编码器相关错误码  
-    - controller_err : 控制器相关错误码  
-
-
-
-### 4. 读取电机模式
-
-```python
-motor.mode
-```
-`mode`  
-返回值：  
-- 电机模式 dict （control_mode，input_mode）  
-- control_mode : 控制模式（ 1-力矩模式，2-速度模式，3-位置模式 ）  
-- input_mode : 输入模式（ 1-直接值，2-带加速度，3-带滤波，5-梯形轨迹 )  
-
-### 5. 读取电机版本
-
-```python
-motor.get_version(1)
-```
-`get_api_version(timeout = 0)`  
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值 ：
-- API版本dict
-    - device_uuid : 设备uuid
-    - main_version : 主版本号
-    - sub_version : 副版本号
-
-### 6. 电机软急停
-
-```python
-motor.estop()
-```
-
-`estop()`  
-
-### 7. 电机重启
-
-```python
-motor.reboot()
-```
-
-`reboot()`  
-
-### 8. 清除错误
-
-```python
-motor.clear_errors()
-```
-
-`clear_errors()`
-
-### 9. 保存设置
-```python
-motor.save_configuration()
-```
-
-`save_configuration()`
-
-设置参数后默认不会保存，直到调用此函数
-
-### 10. 设置电机CAN_ID
-
-```python
-motor.config_can_bus(id = 0x10, heartbeat = 1)
-```
-
-`config_can_bus(new_id, heartbeat = 1, bitrate = 'CAN_1M')`
-
-参数 ：
-- new_id ：电机新CAN_ID (0x01~0x3F)
-- heartbeat : 心跳包发送周期 （ s ）
-
-### 11. 电机使能
-```python
-motor.enable()
-```
-
-`enable()`
-
-### 12. 电机失能
-
-```python
-motor.disable()
-```
-
-`disable()`
-
-### 13. 电机校准
-```python
-motor.calibrate()
-```
-
-`calibrate()`
-
-校准后需保存参数
-
-### 14. 读取总线电压
-```python
-motor.get_voltage(1)
-```
-
-`get_voltage(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值 ：
-- 总线电压值 ( V ) ，超时则不返回
-
-### 15. 读取电机温度
-```python
-motor.get_temperature(1)
-```
-
-`get_temperature(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 电机温度 ( °C ) ，超时则不返回
-
-### 16. 读取电机状态参数
-```python
-motor.get_feedback(1)
-```
-
-`get_feedback(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值 ：
-- 电机状态参数(位置rad, 速度rad/s, 力矩Nm)，超时则不返回
-
-
-### 17. 读取电机位置
-```python
-motor.get_pos(1)
-```
-
-`get_pos(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 位置(rad)，超时则不返回
-
-### 18. 读取电机绝对位置
-```python
-motor.get_abs_pos(1)
-```
-
-`get_abs_pos(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 绝对位置(rad)，断电不丢失，超时则不返回
-
-### 19. 读取电机速度
-```python
-motor.get_vel(1)
-```
-
-`get_vel(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 速度(rad/s)，超时则不返回
-
-### 20. 读取电机力矩
-```python
-motor.get_torque(1)
-```
-
-`get_torque(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 力矩(Nm)，超时则不返回
-
-### 21. 读取电机控制模式
-```python
-motor.get_mode(1)
-```
-`get_mode(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 控制模式(control_mode, input_mode)
-    - control_mode: 控制模式（1：力矩控制，2：速度控制，3：位置控制）
-    - input_mode: 输入模式（1：直接值，2：带加速度，3：带滤波，5：梯形轨迹)
-
-### 22. 进入直接位置模式
-```python
-motor.position_mode()
-```
-`position_mode()`
-
-直接PID控制位置
-
-### 23. 进入滤波位置模式
-```python
-motor.position_filter_mode(4)
-```
-`position_filter_mode(bandwidth)`
-
-参数：
-- bandwidth: 滤波带宽 / 控制频率(Hz)
-
-### 24. 进入轨迹位置模式
-```python
-motor.position_track_mode(10,5,5)
-```
-`position_track_mode(vel, acc, dec)`
-
-参数:
-- vel: 运动最高速度 ( rad/s ) 
-- acc: 运动加速度 ( rad/s^2 ) 
-- dec: 运动减速度 ( rad/s^2 ) 
-
-### 25. 进入直接速度模式
-```python
-motor.velocity_mode()
-```
-`velocity_mode()`
-
-速度PID控制
-
-### 26. 进入匀加减速速度模式
-```python
-motor.velocity_ramp_mode(1.414)
-```
-`velocity_ramp_mode(ramp)`
-
-参数:
-- ramp: 加速度(rad/s^2)
-
-### 27. 进入力矩控制模式
-```python
-motor.torque_mode()
-```
-`torque_mode()`
-
-### 28. 读取电机PID参数
-```python
-motor.get_pid(1)
-```
-`get_pid(timeout = 0)`
-
-参数：
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 电机PID
-    - pos_kp : 位置环P
-    - vel_kp : 速度环P
-    - vel_ki : 速度环I
-
-### 29. 设置电机PID参数
-```python
-motor.set_pid(100,0.02,0.005)
-```
-`set_pid(pos_kp, vel_kp, vel_ki)`
-
-参数:
-- pos_kp: 位置环比例系数
-- vel_kp: 速度环比例系数
-- vel_ki: 速度环积分系数
-
-### 30. 读取电机速度限制
-```python
-motor.get_vel_limit()
-```
-`get_vel_limit(timeout = 0)`
-
-参数:
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 输出端最大速度(rad/s)，超时则不返回
-
-### 31. 读取电机电流限制
-```python
-motor.get_current_limit()
-```
-
-`get_current_limit(timeout = 0)`
-
-参数:
-- timeout : 请求超时时间(s)，0代表无超时时间
-
-返回值：
-- 最大电流(A)，超时则不返回
-
-### 32. 设置电机速度限制
-```python
-motor.set_vel_limit(3.14)
-```
-
-`set_vel_limit(vel_lim)`
-
-参数：
-- vel_lim: 输出端最大速度(rad/s)
-
-### 33. 设置电机电流限制
-```python
-motor.set_current_limit(10)
-```
-`set_current_limit(current_lim)`
-
-参数:
-- current_lim : 最大电流(A)
-
-### 34. 设置位置
-```python
-motor.set_pos(-1.57)
-```
-`set_pos(pos)`
-
-参数:
-- pos: 目标位置(rad)
-
-### 35. 设置绝对位置
-```python
-motor.set_abs_pos(-1.57)
-```
-`set_abs_pos(pos)`
-
-参数:
-- pos: 目标绝对位置(rad)
-
-### 36. 设置速度
-```python
-motor.set_vel(-0.5)
-```
-`set_vel(velocity)`
-
-参数：
-- velocity: 目标速度(rad/s)
-
-### 37. 设置力矩
-```python
-motor.set_torque(0.0)
-```
-`set_torque(torque)`
-
-参数：
-- torque: 目标力矩(Nm)
-
-### 38. 恢复出厂设置
-```python
-motor.reset()
-```
-`reset()`
-
-## 命令行工具
-
-1. robodyno
-- -c, --channel: CAN总线通道选项（可选，默认can0）
-- -b, --bitrate: CAN总线速率选项（可选，默认CAN_1M）
-- -h, --help: 显示帮助信息
-
-    `robodyno -h`
-
-- list: 列举总线上所有robodyno设备
-
-    -   例：当前CAN总线速率为1000K，通道为can0，列举所有robodyno设备
-
-        `robodyno list`
-
-- monitor: 监听总线上所有消息
-
-    - 例：当前CAN总线速率为500K，监听CAN总线上的实时消息
-
-        `robodyno monitor -b CAN_500K`
-
-2. robodyno-motor
-- -c, --channel: CAN总线通道选项（可选，默认can0）
-- -b, --bitrate: CAN总线速率选项（可选，默认CAN_1M）
-- --id: 需要操作的电机ID（可选，可传多个，默认0x10）
-- -h, --help: 显示帮助信息
-
-    `robodyno-motor -h`
-
-- enable: 电机使能
-
-    - 例：将ID为0x10的电机使能
-
-        `robodyno-motor enable`
-
-- disable: 电机失能
-
-    - 例：将ID为0x11的电机失能
-
-        `robodyno-motor disable --id 0x11`
-
-- info: 显示电机状态信息
-
-    - 例：显示ID为0x12、0x13及0x14的电机信息
-
-        `robodyno-motor info --id 0x12 0x13 0x14`
-
-- control: 控制电机运动
-
-    - -p, --pos: 指定电机运动位置(rad)
-
-    - 例：将电机转动到相对开机初始位置180°的位置
-
-        `robodyno-motor control -p 3.14`
-
-    - -ap, --abs-pos: 指定电机绝对位置（仅支持部分型号）(rad)
-
-    - 例：将ID为0x10的电机转动到相对复位位置180°的位置
-
-        `robodyno-motor control -ap 3.14`
-
-    - -v, --vel: 指定电机运动速度(rad/s)
-
-    - 例：操作ID为0x11的电机以15rpm的速度转动
-
-        `robodyno-motor control --id 0x11 -v 1.57`
-
-    - -t, --torque: 指定电机输出力矩(Nm)
-
-    - 例：操作ID为0x12, 0x13及0x14的电机输出0.1Nm的扭矩
-
-        `robodyno-motor control --id 0x12 0x13 0x14 -t 0.1`
-
-- config --new-id [-s, --save]: 修改电机ID，只能同时操作一个电机，-s 保存设置
-
-    - 例：将原ID为0x10的电机ID更改为0x11并保存
-
-        `robodyno-motor config --new-id 0x11 -s`
-    
-    - 例：将原ID为0x11的电机ID临时更改为0x10（断电后ID仍为0x11）
-
-        `robodyno-motor config --id 0x11 --new-id 0x10`
-
-- reset: 将电机恢复出厂设置（重新校准，ID复原为0x10）
-    
-    - 例：将ID为0x11的电机恢复出厂设置
-
-        `robodyno-motor reset --id 0x11`
+Metadata-Version: 2.1
+Name: robodyno
+Version: 1.6.1b0
+Summary: The Robodyno Robot SDK for Python 3
+Home-page: http://101.42.250.169/
+Author: song
+Author-email: zhaosongy@126.com
+Maintainer: robottime
+Maintainer-email: lab@robottime.cn
+License: MIT License
+Keywords: robodyno,robot,robot module
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Framework :: Robot Framework
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# Robodyno
+
+## 安装
+[安装Python(>=3.7)](https://www.python.org/downloads/)
+
+使用pip安装robodyno库
+
+```
+pip install robodyno
+````
+
+## Python API
+
+### 1. 初始化电机对象
+
+```python
+from robodyno.components import Motor
+from robodyno.interfaces import CanBus
+can = CanBus()
+motor = Motor(can, 0x10)
+```
+`Motor(iface, id, type)`  
+参数 ：
+- iface : robodyno 接口对象
+- id : 电机ID（ 范围从 0x01 到 0x3F ）
+- type : 电机的类型，默认自动识别
+    - ROBODYNO_PRO_44
+    - ROBODYNO_PRO_12
+    - ROBODYNO_PRO_50
+    - ROBODYNO_PRO_100
+
+### 2. 读取电机状态
+
+```python
+motor.state
+```
+`state`  
+返回值 ：
+- 电机状态 （1-空闲，8-使能）
+
+### 3. 读取电机错误
+
+```python
+motor.error
+```
+`error`  
+返回值 :  
+- 电机错误 dict  
+    - error : 错误码（1-电压不足，14-急停）  
+    - motor : 电机相关错误码  
+    - encoder_err : 编码器相关错误码  
+    - controller_err : 控制器相关错误码  
+
+
+
+### 4. 读取电机模式
+
+```python
+motor.mode
+```
+`mode`  
+返回值：  
+- 电机模式 dict （control_mode，input_mode）  
+- control_mode : 控制模式（ 1-力矩模式，2-速度模式，3-位置模式 ）  
+- input_mode : 输入模式（ 1-直接值，2-带加速度，3-带滤波，5-梯形轨迹 )  
+
+### 5. 读取电机版本
+
+```python
+motor.get_version(1)
+```
+`get_api_version(timeout = 0)`  
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值 ：
+- API版本dict
+    - device_uuid : 设备uuid
+    - main_version : 主版本号
+    - sub_version : 副版本号
+
+### 6. 电机软急停
+
+```python
+motor.estop()
+```
+
+`estop()`  
+
+### 7. 电机重启
+
+```python
+motor.reboot()
+```
+
+`reboot()`  
+
+### 8. 清除错误
+
+```python
+motor.clear_errors()
+```
+
+`clear_errors()`
+
+### 9. 保存设置
+```python
+motor.save() # or motor.save_configuration()
+```
+
+`save()`
+
+设置参数后默认不会保存，直到调用此函数
+
+### 10. 设置电机CAN_ID
+
+```python
+motor.config_can_bus(new_id = 0x11, heartbeat = 1)
+```
+
+`config_can_bus(new_id, heartbeat = 1, bitrate = 'CAN_1M')`
+
+参数 ：
+- new_id ：电机新CAN_ID (0x01~0x3F)
+- heartbeat : 心跳包发送周期 （ s ）
+
+### 11. 电机使能
+```python
+motor.enable()
+```
+
+`enable()`
+
+### 12. 电机失能
+
+```python
+motor.disable()
+```
+
+`disable()`
+
+### 13. 电机校准
+```python
+motor.calibrate()
+```
+
+`calibrate()`
+
+校准后需保存参数
+
+### 14. 读取总线电压
+```python
+motor.get_voltage(1)
+```
+
+`get_voltage(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值 ：
+- 总线电压值 ( V ) ，超时则不返回
+
+### 15. 读取电机温度
+```python
+motor.get_temperature(1)
+```
+
+`get_temperature(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 电机温度 ( °C ) ，超时则不返回
+
+### 16. 读取电机状态参数
+```python
+motor.get_feedback(1)
+```
+
+`get_feedback(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值 ：
+- 电机状态参数(位置rad, 速度rad/s, 力矩Nm)，超时则不返回
+
+
+### 17. 读取电机位置
+```python
+motor.get_pos(1)
+```
+
+`get_pos(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 位置(rad)，超时则不返回
+
+### 18. 读取电机绝对位置
+```python
+motor.get_abs_pos(1)
+```
+
+`get_abs_pos(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 绝对位置(rad)，断电不丢失，超时则不返回
+
+### 19. 读取电机速度
+```python
+motor.get_vel(1)
+```
+
+`get_vel(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 速度(rad/s)，超时则不返回
+
+### 20. 读取电机力矩
+```python
+motor.get_torque(1)
+```
+
+`get_torque(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 力矩(Nm)，超时则不返回
+
+### 21. 读取电机控制模式
+```python
+motor.get_mode(1)
+```
+`get_mode(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 控制模式(control_mode, input_mode)
+    - control_mode: 控制模式（1：力矩控制，2：速度控制，3：位置控制）
+    - input_mode: 输入模式（1：直接值，2：带加速度，3：带滤波，5：梯形轨迹)
+
+### 22. 进入直接位置模式
+```python
+motor.position_mode()
+```
+`position_mode()`
+
+直接PID控制位置
+
+### 23. 进入滤波位置模式
+```python
+motor.position_filter_mode(4)
+```
+`position_filter_mode(bandwidth)`
+
+参数：
+- bandwidth: 滤波带宽 / 控制频率(Hz)
+
+### 24. 进入轨迹位置模式
+```python
+motor.position_track_mode(10,5,5)
+```
+`position_track_mode(vel, acc, dec)`
+
+参数:
+- vel: 运动最高速度 ( rad/s ) 
+- acc: 运动加速度 ( rad/s^2 ) 
+- dec: 运动减速度 ( rad/s^2 ) 
+
+### 25. 进入直接速度模式
+```python
+motor.velocity_mode()
+```
+`velocity_mode()`
+
+速度PID控制
+
+### 26. 进入匀加减速速度模式
+```python
+motor.velocity_ramp_mode(1.414)
+```
+`velocity_ramp_mode(ramp)`
+
+参数:
+- ramp: 加速度(rad/s^2)
+
+### 27. 进入力矩控制模式
+```python
+motor.torque_mode()
+```
+`torque_mode()`
+
+### 28. 读取电机PID参数
+```python
+motor.get_pid(1)
+```
+`get_pid(timeout = 0)`
+
+参数：
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 电机PID
+    - pos_kp : 位置环P
+    - vel_kp : 速度环P
+    - vel_ki : 速度环I
+
+### 29. 设置电机PID参数
+```python
+motor.set_pid(100,0.02,0.005)
+```
+`set_pid(pos_kp, vel_kp, vel_ki)`
+
+参数:
+- pos_kp: 位置环比例系数
+- vel_kp: 速度环比例系数
+- vel_ki: 速度环积分系数
+
+### 30. 读取电机速度限制
+```python
+motor.get_vel_limit()
+```
+`get_vel_limit(timeout = 0)`
+
+参数:
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 输出端最大速度(rad/s)，超时则不返回
+
+### 31. 读取电机电流限制
+```python
+motor.get_current_limit()
+```
+
+`get_current_limit(timeout = 0)`
+
+参数:
+- timeout : 请求超时时间(s)，0代表无超时时间
+
+返回值：
+- 最大电流(A)，超时则不返回
+
+### 32. 设置电机速度限制
+```python
+motor.set_vel_limit(3.14)
+```
+
+`set_vel_limit(vel_lim)`
+
+参数：
+- vel_lim: 输出端最大速度(rad/s)
+
+### 33. 设置电机电流限制
+```python
+motor.set_current_limit(10)
+```
+`set_current_limit(current_lim)`
+
+参数:
+- current_lim : 最大电流(A)
+
+### 34. 设置位置
+```python
+motor.set_pos(-1.57)
+```
+`set_pos(pos)`
+
+参数:
+- pos: 目标位置(rad)
+
+### 35. 设置绝对位置
+```python
+motor.set_abs_pos(-1.57)
+```
+`set_abs_pos(pos)`
+
+参数:
+- pos: 目标绝对位置(rad)
+
+### 36. 设置速度
+```python
+motor.set_vel(-0.5)
+```
+`set_vel(velocity)`
+
+参数：
+- velocity: 目标速度(rad/s)
+
+### 37. 设置力矩
+```python
+motor.set_torque(0.0)
+```
+`set_torque(torque)`
+
+参数：
+- torque: 目标力矩(Nm)
+
+### 38. 恢复出厂设置
+```python
+motor.reset()
+```
+`reset()`
+
+## 命令行工具
+
+1. robodyno
+- -c, --channel: CAN总线通道选项（可选，默认can0）
+- -b, --bitrate: CAN总线速率选项（可选，默认CAN_1M）
+- -h, --help: 显示帮助信息
+
+    `robodyno -h`
+
+- list: 列举总线上所有robodyno设备
+
+    -   例：当前CAN总线速率为1000K，通道为can0，列举所有robodyno设备
+
+        `robodyno list`
+
+- monitor: 监听总线上所有消息
+
+    - 例：当前CAN总线速率为500K，监听CAN总线上的实时消息
+
+        `robodyno monitor -b CAN_500K`
+
+2. robodyno-motor
+- -c, --channel: CAN总线通道选项（可选，默认can0）
+- -b, --bitrate: CAN总线速率选项（可选，默认CAN_1M）
+- --id: 需要操作的电机ID（可选，可传多个，默认0x10）
+- -h, --help: 显示帮助信息
+
+    `robodyno-motor -h`
+
+- enable: 电机使能
+
+    - 例：将ID为0x10的电机使能
+
+        `robodyno-motor enable`
+
+- disable: 电机失能
+
+    - 例：将ID为0x11的电机失能
+
+        `robodyno-motor disable --id 0x11`
+
+- info: 显示电机状态信息
+
+    - 例：显示ID为0x12、0x13及0x14的电机信息
+
+        `robodyno-motor info --id 0x12 0x13 0x14`
+
+- control: 控制电机运动
+
+    - -p, --pos: 指定电机运动位置(rad)
+
+    - 例：将电机转动到相对开机初始位置180°的位置
+
+        `robodyno-motor control -p 3.14`
+
+    - -ap, --abs-pos: 指定电机绝对位置（仅支持部分型号）(rad)
+
+    - 例：将ID为0x10的电机转动到相对复位位置180°的位置
+
+        `robodyno-motor control -ap 3.14`
+
+    - -v, --vel: 指定电机运动速度(rad/s)
+
+    - 例：操作ID为0x11的电机以15rpm的速度转动
+
+        `robodyno-motor control --id 0x11 -v 1.57`
+
+    - -t, --torque: 指定电机输出力矩(Nm)
+
+    - 例：操作ID为0x12, 0x13及0x14的电机输出0.1Nm的扭矩
+
+        `robodyno-motor control --id 0x12 0x13 0x14 -t 0.1`
+
+- config --new-id [-s, --save]: 修改电机ID，只能同时操作一个电机，-s 保存设置
+
+    - 例：将原ID为0x10的电机ID更改为0x11并保存
+
+        `robodyno-motor config --new-id 0x11 -s`
+    
+    - 例：将原ID为0x11的电机ID临时更改为0x10（断电后ID仍为0x11）
+
+        `robodyno-motor config --id 0x11 --new-id 0x10`
+
+- reset: 将电机恢复出厂设置（重新校准，ID复原为0x10）
+    
+    - 例：将ID为0x11的电机恢复出厂设置
+
+        `robodyno-motor reset --id 0x11`
```

### Comparing `robodyno-1.6.0/src/robodyno.egg-info/SOURCES.txt` & `robodyno-1.6.1b0/src/robodyno.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 src/robodyno.egg-info/PKG-INFO
 src/robodyno.egg-info/SOURCES.txt
 src/robodyno.egg-info/dependency_links.txt
 src/robodyno.egg-info/entry_points.txt
 src/robodyno.egg-info/requires.txt
 src/robodyno.egg-info/top_level.txt
 src/robodyno/components/__init__.py
-src/robodyno/components/brands/__init__.py
-src/robodyno/components/brands/robodyno.py
-src/robodyno/components/brands/uuid.py
 src/robodyno/components/can_bus/__init__.py
 src/robodyno/components/can_bus/adaptive_gripper.py
 src/robodyno/components/can_bus/can_bus_device.py
 src/robodyno/components/can_bus/gps_sensor.py
 src/robodyno/components/can_bus/imu_sensor.py
 src/robodyno/components/can_bus/led_driver.py
 src/robodyno/components/can_bus/motor.py
 src/robodyno/components/can_bus/pwm_driver.py
 src/robodyno/components/can_bus/slider_module.py
 src/robodyno/components/can_bus/stepper_driver.py
 src/robodyno/components/can_bus/vacuum_gripper.py
+src/robodyno/components/config/__init__.py
+src/robodyno/components/config/model.py
+src/robodyno/components/config/robottime_config.py
 src/robodyno/components/webots/__init__.py
 src/robodyno/components/webots/motor.py
 src/robodyno/components/webots/slider_module.py
 src/robodyno/components/webots/webots_device.py
 src/robodyno/interfaces/__init__.py
 src/robodyno/interfaces/can_bus.py
 src/robodyno/interfaces/webots.py
@@ -40,10 +40,11 @@
 src/robodyno/robots/three_dof_delta_robot/three_dof_delta_robot.py
 src/robodyno/robots/three_dof_palletizing_robot/__init__.py
 src/robodyno/robots/three_dof_palletizing_robot/three_dof_pallet_robot.py
 src/robodyno/robots/utils/__init__.py
 src/robodyno/robots/utils/interpolations.py
 src/robodyno/robots/utils/transformations.py
 src/robodyno/tools/__init__.py
-src/robodyno/tools/list_devices.py
-src/robodyno/tools/monitor.py
-src/robodyno/tools/utils.py
+src/robodyno/tools/can_bus_monitor.py
+src/robodyno/tools/cli.py
+src/robodyno/tools/cli_param_types.py
+src/robodyno/tools/motor_info_table.py
```

### Comparing `robodyno-1.6.0/src/robodyno.egg-info/entry_points.txt` & `robodyno-1.6.1b0/src/robodyno.egg-info/entry_points.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 [console_scripts]
-robodyno = robodyno:robodyno
-robodyno-motor = robodyno:robodyno_motor
+robodyno = robodyno.tools.cli:robodyno
 
 [robodyno.components.can_bus]
 ImuSensor = robodyno.components.can_bus.imu_sensor:ImuSensor
 Motor = robodyno.components.can_bus.motor:Motor
 PwmDriver = robodyno.components.can_bus.pwm_driver:PwmDriver
 SliderModule = robodyno.components.can_bus.slider_module:SliderModule
 StepperDriver = robodyno.components.can_bus.stepper_driver:StepperDriver
-VGripper = robodyno.components.can_bus.vacuum_gripper:VGripper
 
 [robodyno.components.webots]
 Motor = robodyno.components.webots.motor:Motor
 SliderModule = robodyno.components.webots.slider_module:SliderModule
 
 [robodyno.robots]
 FourDoFPallet = robodyno.robots.four_dof_palletizing_robot.four_dof_pallet_robot:FourDoFPallet
```

