# Comparing `tmp/pitop.pma-0.30.0.post1.tar.gz` & `tmp/pitop.pma-0.31.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.pma-0.30.0.post1.tar", last modified: Fri Dec 16 14:08:36 2022, max compression
+gzip compressed data, was "dist/pitop.pma-0.31.0.post2.tar", last modified: Mon May 22 19:13:13 2023, max compression
```

## Comparing `pitop.pma-0.30.0.post1.tar` & `pitop.pma-0.31.0.post2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:36.000000 pitop.pma-0.30.0.post1/
--rw-r--r--   0 runner    (1001) docker     (122)       31 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2022-12-16 14:08:36.000000 pitop.pma-0.30.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      175 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:36.000000 pitop.pma-0.30.0.post1/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:36.000000 pitop.pma-0.30.0.post1/pitop/pma/
--rw-r--r--   0 runner    (1001) docker     (122)      540 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2953 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/adc_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2551 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/button.py
--rw-r--r--   0 runner    (1001) docker     (122)     2458 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/buzzer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:36.000000 pitop.pma-0.30.0.post1/pitop/pma/common/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/common/encoder_motor_registers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/common/imu_registers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:36.000000 pitop.pma-0.30.0.post1/pitop/pma/common/math_functions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/common/math_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3746 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/common/math_functions/ellipsoid_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)      169 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/common/plate_registers.py
--rw-r--r--   0 runner    (1001) docker     (122)      926 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/common/servo_motor_registers.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/common/ultrasonic_registers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    17134 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/encoder_motor.py
--rw-r--r--   0 runner    (1001) docker     (122)     6086 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/encoder_motor_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     4934 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/imu.py
--rw-r--r--   0 runner    (1001) docker     (122)    10278 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/imu_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     2643 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/led.py
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/light_sensor.py
--rw-r--r--   0 runner    (1001) docker     (122)      301 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2589 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/plate_interface.py
--rw-r--r--   0 runner    (1001) docker     (122)     2028 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/potentiometer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4953 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/servo_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)    10704 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/servo_motor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1888 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/sound_sensor.py
--rw-r--r--   0 runner    (1001) docker     (122)     6079 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/ultrasonic_sensor.py
--rw-r--r--   0 runner    (1001) docker     (122)    12049 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/pitop/pma/ultrasonic_sensor_base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:36.000000 pitop.pma-0.30.0.post1/pitop.pma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2022-12-16 14:08:36.000000 pitop.pma-0.30.0.post1/pitop.pma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2022-12-16 14:08:36.000000 pitop.pma-0.30.0.post1/pitop.pma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-16 14:08:36.000000 pitop.pma-0.30.0.post1/pitop.pma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2022-12-16 14:08:36.000000 pitop.pma-0.30.0.post1/pitop.pma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-12-16 14:08:36.000000 pitop.pma-0.30.0.post1/pitop.pma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-16 14:08:36.000000 pitop.pma-0.30.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2054 2022-12-16 14:07:48.000000 pitop.pma-0.30.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.pma-0.31.0.post2/
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-05-22 19:13:13.000000 pitop.pma-0.31.0.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.pma-0.31.0.post2/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.pma-0.31.0.post2/pitop/pma/
+-rw-r--r--   0 runner    (1001) docker     (122)      540 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2953 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/adc_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/button.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2458 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/buzzer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.pma-0.31.0.post2/pitop/pma/common/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/common/encoder_motor_registers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/common/imu_registers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.pma-0.31.0.post2/pitop/pma/common/math_functions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/common/math_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3746 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/common/math_functions/ellipsoid_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/common/plate_registers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      926 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/common/servo_motor_registers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/common/ultrasonic_registers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17224 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/encoder_motor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6086 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/encoder_motor_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/imu.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10278 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/imu_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/led.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/light_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2586 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/plate_interface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/potentiometer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4953 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/servo_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10704 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/servo_motor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/sound_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6078 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/ultrasonic_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12048 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/pitop/pma/ultrasonic_sensor_base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.pma-0.31.0.post2/pitop.pma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-05-22 19:13:13.000000 pitop.pma-0.31.0.post2/pitop.pma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-05-22 19:13:13.000000 pitop.pma-0.31.0.post2/pitop.pma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 19:13:13.000000 pitop.pma-0.31.0.post2/pitop.pma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-22 19:13:13.000000 pitop.pma-0.31.0.post2/pitop.pma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 19:13:13.000000 pitop.pma-0.31.0.post2/pitop.pma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:13:13.000000 pitop.pma-0.31.0.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-05-22 19:12:55.000000 pitop.pma-0.31.0.post2/setup.py
```

### Comparing `pitop.pma-0.30.0.post1/PKG-INFO` & `pitop.pma-0.31.0.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.pma
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python PMA
```

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/__init__.py` & `pitop.pma-0.31.0.post2/pitop/pma/__init__.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/adc_base.py` & `pitop.pma-0.31.0.post2/pitop/pma/adc_base.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/button.py` & `pitop.pma-0.31.0.post2/pitop/pma/button.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/buzzer.py` & `pitop.pma-0.31.0.post2/pitop/pma/buzzer.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/common/encoder_motor_registers.py` & `pitop.pma-0.31.0.post2/pitop/pma/common/encoder_motor_registers.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/common/imu_registers.py` & `pitop.pma-0.31.0.post2/pitop/pma/common/imu_registers.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/common/math_functions/ellipsoid_functions.py` & `pitop.pma-0.31.0.post2/pitop/pma/common/math_functions/ellipsoid_functions.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/common/servo_motor_registers.py` & `pitop.pma-0.31.0.post2/pitop/pma/common/servo_motor_registers.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/common/utils.py` & `pitop.pma-0.31.0.post2/pitop/pma/common/utils.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/encoder_motor.py` & `pitop.pma-0.31.0.post2/pitop/pma/encoder_motor.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,18 @@
         braking_type=BrakingType.BRAKE,
         wheel_diameter=0.075,
         name="encoder_motor",
     ):
         self.name = name
         self._pma_port = port_name
 
-        self.__motor_core = EncoderMotorController(self._pma_port, braking_type.value)
+        if isinstance(braking_type, BrakingType):
+            braking_type = braking_type.value
+
+        self.__motor_core = EncoderMotorController(self._pma_port, braking_type)
         self.__forward_direction = forward_direction
         self.__wheel_diameter = wheel_diameter
 
         self.__prev_time_dist_cnt = time.time()
         self.__previous_reading_odometer = 0
 
         atexit.register(self.stop)
@@ -125,15 +128,14 @@
         :param braking_type:
             The braking type of the motor.
         """
         return BrakingType(self.__motor_core.braking_type())
 
     @braking_type.setter
     def braking_type(self, braking_type):
-
         self.__motor_core.set_braking_type(braking_type.value)
 
     def set_power(self, power, direction=Direction.FORWARD):
         """Turn the motor on at the power level provided, in the range -1.0 to.
 
         +1.0, where:
```

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/encoder_motor_controller.py` & `pitop.pma-0.31.0.post2/pitop/pma/encoder_motor_controller.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/imu.py` & `pitop.pma-0.31.0.post2/pitop/pma/imu.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/imu_controller.py` & `pitop.pma-0.31.0.post2/pitop/pma/imu_controller.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/led.py` & `pitop.pma-0.31.0.post2/pitop/pma/led.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/light_sensor.py` & `pitop.pma-0.31.0.post2/pitop/pma/light_sensor.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/plate_interface.py` & `pitop.pma-0.31.0.post2/pitop/pma/plate_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,25 +8,23 @@
 from .common.plate_registers import PlateRegisters
 
 logger = logging.getLogger(__name__)
 
 
 class PlateInterface(metaclass=Singleton):
     def __init__(self):
-
         self.__device_mcu = None
         self.__mcu_connected = False
         self.__mcu_thread_lock = Lock()
         self.__heartbeat_thread = None
 
     def __del__(self):
         self.__disconnect_mcu()
 
     def get_device_mcu(self):
-
         self.__connect_mcu()
 
         # Return the SMBusDevice instance
         return self.__device_mcu
 
     def __connect_mcu(self):
         if self.__mcu_connected:
@@ -74,15 +72,14 @@
             self.__mcu_connected = False
             raise IOError(
                 "Error communicating with Foundation/Expansion plate. Make sure it's connected to your pi-top."
             ) from None
 
     def __heartbeat_thread_loop(self):
         while self.__mcu_connected:
-
             with self.__mcu_thread_lock:
                 self.__send_heartbeat()
 
             for _ in range(10):
                 sleep(PlateRegisters.HEARTBEAT_SEND_INTERVAL_SECONDS / 10)
                 if self.__mcu_connected is False:
                     break
```

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/potentiometer.py` & `pitop.pma-0.31.0.post2/pitop/pma/potentiometer.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/servo_controller.py` & `pitop.pma-0.31.0.post2/pitop/pma/servo_controller.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/servo_motor.py` & `pitop.pma-0.31.0.post2/pitop/pma/servo_motor.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/sound_sensor.py` & `pitop.pma-0.31.0.post2/pitop/pma/sound_sensor.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/ultrasonic_sensor.py` & `pitop.pma-0.31.0.post2/pitop/pma/ultrasonic_sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
         port_name,
         queue_len=5,
         max_distance=3,
         threshold_distance=0.3,
         partial=False,
         name="ultrasonic",
     ):
-
         assert port_name in Port
         self._pma_port = port_name
         self.name = name
 
         if port_name in valid_analog_ports:
             self.__ultrasonic_device = UltrasonicSensorMCU(
                 port_name=port_name,
```

### Comparing `pitop.pma-0.30.0.post1/pitop/pma/ultrasonic_sensor_base.py` & `pitop.pma-0.31.0.post2/pitop/pma/ultrasonic_sensor_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,14 @@
         port_name,
         queue_len=3,
         max_distance=3,
         threshold_distance=0.3,
         partial=True,
         name="ultrasonic",
     ):
-
         self._pma_port = port_name
         self.name = name
 
         SmoothedInputDevice.__init__(
             self,
             get_pin_for_port(self._pma_port),
             pull_up=False,
```

### Comparing `pitop.pma-0.30.0.post1/pitop.pma.egg-info/PKG-INFO` & `pitop.pma-0.31.0.post2/pitop.pma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.pma
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python PMA
```

### Comparing `pitop.pma-0.30.0.post1/pitop.pma.egg-info/SOURCES.txt` & `pitop.pma-0.31.0.post2/pitop.pma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.30.0.post1/setup.py` & `pitop.pma-0.31.0.post2/setup.py`

 * *Files identical despite different names*

