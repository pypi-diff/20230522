# Comparing `tmp/pymcp2221-1.0.6.tar.gz` & `tmp/pymcp2221-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymcp2221-1.0.6.tar", last modified: Wed Mar  1 09:00:18 2023, max compression
+gzip compressed data, was "pymcp2221-1.0.7.tar", last modified: Mon May 22 18:50:32 2023, max compression
```

## Comparing `pymcp2221-1.0.6.tar` & `pymcp2221-1.0.7.tar`

### file list

```diff
@@ -1,36 +1,27 @@
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-03-01 09:00:18.342898 pymcp2221-1.0.6/
--rw-r--r--   0 vpaeder    (501) staff       (20)       21 2022-03-07 11:14:44.000000 pymcp2221-1.0.6/.gitignore
--rw-r--r--   0 vpaeder    (501) staff       (20)     2960 2023-03-01 09:00:18.342316 pymcp2221-1.0.6/PKG-INFO
--rw-r--r--   0 vpaeder    (501) staff       (20)     2021 2022-03-07 12:05:07.000000 pymcp2221-1.0.6/README.md
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-03-01 09:00:18.320602 pymcp2221-1.0.6/docs/
--rw-r--r--   0 vpaeder    (501) staff       (20)    67530 2022-03-07 11:59:50.000000 pymcp2221-1.0.6/docs/index.html
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-03-01 09:00:18.326488 pymcp2221-1.0.6/examples/
--rw-r--r--   0 vpaeder    (501) staff       (20)      737 2022-03-07 11:57:05.000000 pymcp2221-1.0.6/examples/README.md
--rw-r--r--   0 vpaeder    (501) staff       (20)     1753 2022-03-07 11:14:44.000000 pymcp2221-1.0.6/examples/adc.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     1785 2022-03-07 11:14:44.000000 pymcp2221-1.0.6/examples/dac.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     1192 2022-03-07 11:14:44.000000 pymcp2221-1.0.6/examples/find_device.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     1592 2022-03-07 11:14:44.000000 pymcp2221-1.0.6/examples/gpio.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     2248 2022-03-07 11:14:44.000000 pymcp2221-1.0.6/examples/gpio_powerup.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-03-01 09:00:18.329219 pymcp2221-1.0.6/mcp2221/
--rw-r--r--   0 vpaeder    (501) staff       (20)    63198 2023-03-01 08:48:33.000000 pymcp2221-1.0.6/mcp2221/__init__.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     5145 2022-03-07 11:14:44.000000 pymcp2221-1.0.6/mcp2221/enums.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      814 2022-03-07 11:14:44.000000 pymcp2221-1.0.6/mcp2221/exceptions.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-03-01 09:00:18.332451 pymcp2221-1.0.6/pymcp2221.egg-info/
--rw-r--r--   0 vpaeder    (501) staff       (20)     2960 2023-03-01 09:00:18.000000 pymcp2221-1.0.6/pymcp2221.egg-info/PKG-INFO
--rw-r--r--   0 vpaeder    (501) staff       (20)      553 2023-03-01 09:00:18.000000 pymcp2221-1.0.6/pymcp2221.egg-info/SOURCES.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)        1 2023-03-01 09:00:18.000000 pymcp2221-1.0.6/pymcp2221.egg-info/dependency_links.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)        7 2023-03-01 09:00:18.000000 pymcp2221-1.0.6/pymcp2221.egg-info/requires.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)       14 2023-03-01 09:00:18.000000 pymcp2221-1.0.6/pymcp2221.egg-info/top_level.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)       38 2023-03-01 09:00:18.343034 pymcp2221-1.0.6/setup.cfg
--rw-r--r--   0 vpaeder    (501) staff       (20)     1261 2023-03-01 08:59:17.000000 pymcp2221-1.0.6/setup.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-03-01 09:00:18.341506 pymcp2221-1.0.6/tests/
--rw-r--r--   0 vpaeder    (501) staff       (20)      262 2022-03-07 11:14:44.000000 pymcp2221-1.0.6/tests/__init__.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     2109 2022-03-07 11:14:44.000000 pymcp2221-1.0.6/tests/comm.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     5394 2022-03-07 11:14:44.000000 pymcp2221-1.0.6/tests/common.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     2306 2022-03-07 11:14:44.000000 pymcp2221-1.0.6/tests/gpio.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     3773 2023-02-28 07:15:06.000000 pymcp2221-1.0.6/tests/i2c.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     2317 2022-03-07 11:14:44.000000 pymcp2221-1.0.6/tests/memory.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     1051 2022-03-07 11:14:44.000000 pymcp2221-1.0.6/tests/misc.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    17603 2023-03-01 07:42:52.000000 pymcp2221-1.0.6/tests/settings_flash.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     7067 2022-03-07 11:14:44.000000 pymcp2221-1.0.6/tests/settings_sram.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     1960 2022-03-07 11:14:44.000000 pymcp2221-1.0.6/tests/status.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-22 18:50:32.302593 pymcp2221-1.0.7/
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1071 2023-05-22 18:22:30.000000 pymcp2221-1.0.7/LICENSE
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3182 2023-05-22 18:50:32.302276 pymcp2221-1.0.7/PKG-INFO
+-rw-r--r--   0 vpaeder    (501) staff       (20)     2221 2023-05-22 18:22:30.000000 pymcp2221-1.0.7/README.md
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-22 18:50:32.296620 pymcp2221-1.0.7/mcp2221/
+-rw-r--r--   0 vpaeder    (501) staff       (20)    63516 2023-05-22 18:39:33.000000 pymcp2221-1.0.7/mcp2221/__init__.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     5145 2023-05-22 18:22:30.000000 pymcp2221-1.0.7/mcp2221/enums.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      814 2023-05-22 18:22:30.000000 pymcp2221-1.0.7/mcp2221/exceptions.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-22 18:50:32.298450 pymcp2221-1.0.7/pymcp2221.egg-info/
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3182 2023-05-22 18:50:32.000000 pymcp2221-1.0.7/pymcp2221.egg-info/PKG-INFO
+-rw-r--r--   0 vpaeder    (501) staff       (20)      417 2023-05-22 18:50:32.000000 pymcp2221-1.0.7/pymcp2221.egg-info/SOURCES.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)        1 2023-05-22 18:50:32.000000 pymcp2221-1.0.7/pymcp2221.egg-info/dependency_links.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)        7 2023-05-22 18:50:32.000000 pymcp2221-1.0.7/pymcp2221.egg-info/requires.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)       14 2023-05-22 18:50:32.000000 pymcp2221-1.0.7/pymcp2221.egg-info/top_level.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)       38 2023-05-22 18:50:32.302680 pymcp2221-1.0.7/setup.cfg
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1261 2023-05-22 18:35:22.000000 pymcp2221-1.0.7/setup.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-22 18:50:32.301898 pymcp2221-1.0.7/tests/
+-rw-r--r--   0 vpaeder    (501) staff       (20)      262 2023-05-22 18:22:30.000000 pymcp2221-1.0.7/tests/__init__.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     2158 2023-05-22 18:34:39.000000 pymcp2221-1.0.7/tests/comm.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     5394 2023-05-22 18:22:30.000000 pymcp2221-1.0.7/tests/common.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     2306 2023-05-22 18:22:30.000000 pymcp2221-1.0.7/tests/gpio.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3773 2023-05-22 18:22:30.000000 pymcp2221-1.0.7/tests/i2c.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     2317 2023-05-22 18:22:30.000000 pymcp2221-1.0.7/tests/memory.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1051 2023-05-22 18:22:30.000000 pymcp2221-1.0.7/tests/misc.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    17603 2023-05-22 18:22:30.000000 pymcp2221-1.0.7/tests/settings_flash.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     7067 2023-05-22 18:22:30.000000 pymcp2221-1.0.7/tests/settings_sram.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1960 2023-05-22 18:22:30.000000 pymcp2221-1.0.7/tests/status.py
```

### Comparing `pymcp2221-1.0.6/PKG-INFO` & `pymcp2221-1.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcp2221
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python driver for the Microchip MCP2221/MCP2221A USB 2.0 to I2C/UART protocol converters.
 Home-page: https://github.com/vpaeder/pymcp2221
 Author: Vincent Paeder
 Author-email: python@paeder.fi
 Project-URL: Bug Tracker, https://github.com/vpaeder/pymcp2221/issues
 Keywords: MCP2221,MCP2221A,Microchip
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,22 +14,25 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Communications
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB)
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB) :: Human Interface Device (HID)
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # pymcp2221
+
 This is a python driver for the Microchip MCP2221/MCP2221A USB 2.0 to I2C/UART protocol converters
 ([manufacturer's page](https://www.microchip.com/en-us/product/MCP2221A)).
 
 First and foremost, there are python packages for the same chip available [here](https://github.com/nonNoise/PyMCP2221A) and [here](https://github.com/pilotak/python-mcp2221). If you use them and are satisfied, you probably won't find improvements in my package. If you're missing some features however, my code is meant to expose every chip feature described in the datasheet in a systematic manner, for python 3.2+.
 
-##### Implemented features
+## Implemented features
+
 - Status/Set Parameters (0x10) - ok
 - Read Flash Data (0xB0) - ok
 - Write Flash Data (0xB1) - ok
 - Send Flash Access Password (0xB2) - ok
 - I2C Write Data (0x90) - ok
 - I2C Write Data Repeated Start (0x92) - ok
 - I2C Write Data No Stop (0x94) - ok
@@ -39,38 +42,54 @@
 - Get GPIO Values (0x51) - ok
 - Set SRAM Settings (0x60) - ok, except GPIO directions/values through SRAM (duplicate with 0x50)
 - Get SRAM Settings (0x61) - ok, except GPIO directions/values through SRAM (duplicate with 0x51)
 - Reset Chip (0x70) - ok
 
 Every feature marked *ok* is implemented, but some of them, like I2C, haven't been tested in real conditions.
 
-# Requirements
+## Requirements
+
 - [hidapi](https://pypi.org/project/hidapi)
 
-# Setup
+## Setup
+
 From command line, use:
 
-    python setup.py install
+```bash
+python setup.py install
+```
 
 or for Linux/OSX:
 
-    sudo python setup.py install
+```bash
+sudo python setup.py install
+```
+
+On Linux, to access your devices without root privileges, you need to set specific udev rules, as explained in [hidapi documentation](https://github.com/trezor/cython-hidapi#udev-rules).
+
+## Examples
 
-# Examples
 See [examples](examples) folder.
 
-# Tests
+## Tests
+
 The [tests](tests) folder contains unit tests for most of the aspects of this package. To run them, use:
 
-    python -m unittest
+```bash
+python -m unittest
+```
+
+## API
 
-# API
 You can find docs in the [docs](docs) folder (generated from python docstrings). Alternatively, you can rely on python docstrings
 
 1) either from the command line, use pydoc:
-    ```bash
-    pydoc mcp2221
-    ```
+
+```bash
+pydoc mcp2221
+```
+
 2) or from within python:
-    ```python
-    import mcp2221; help(mcp2221)
-    ```
+
+```python
+import mcp2221; help(mcp2221)
+```
```

### Comparing `pymcp2221-1.0.6/README.md` & `pymcp2221-1.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # pymcp2221
+
 This is a python driver for the Microchip MCP2221/MCP2221A USB 2.0 to I2C/UART protocol converters
 ([manufacturer's page](https://www.microchip.com/en-us/product/MCP2221A)).
 
 First and foremost, there are python packages for the same chip available [here](https://github.com/nonNoise/PyMCP2221A) and [here](https://github.com/pilotak/python-mcp2221). If you use them and are satisfied, you probably won't find improvements in my package. If you're missing some features however, my code is meant to expose every chip feature described in the datasheet in a systematic manner, for python 3.2+.
 
-##### Implemented features
+## Implemented features
+
 - Status/Set Parameters (0x10) - ok
 - Read Flash Data (0xB0) - ok
 - Write Flash Data (0xB1) - ok
 - Send Flash Access Password (0xB2) - ok
 - I2C Write Data (0x90) - ok
 - I2C Write Data Repeated Start (0x92) - ok
 - I2C Write Data No Stop (0x94) - ok
@@ -18,38 +20,54 @@
 - Get GPIO Values (0x51) - ok
 - Set SRAM Settings (0x60) - ok, except GPIO directions/values through SRAM (duplicate with 0x50)
 - Get SRAM Settings (0x61) - ok, except GPIO directions/values through SRAM (duplicate with 0x51)
 - Reset Chip (0x70) - ok
 
 Every feature marked *ok* is implemented, but some of them, like I2C, haven't been tested in real conditions.
 
-# Requirements
+## Requirements
+
 - [hidapi](https://pypi.org/project/hidapi)
 
-# Setup
+## Setup
+
 From command line, use:
 
-    python setup.py install
+```bash
+python setup.py install
+```
 
 or for Linux/OSX:
 
-    sudo python setup.py install
+```bash
+sudo python setup.py install
+```
+
+On Linux, to access your devices without root privileges, you need to set specific udev rules, as explained in [hidapi documentation](https://github.com/trezor/cython-hidapi#udev-rules).
+
+## Examples
 
-# Examples
 See [examples](examples) folder.
 
-# Tests
+## Tests
+
 The [tests](tests) folder contains unit tests for most of the aspects of this package. To run them, use:
 
-    python -m unittest
+```bash
+python -m unittest
+```
+
+## API
 
-# API
 You can find docs in the [docs](docs) folder (generated from python docstrings). Alternatively, you can rely on python docstrings
 
 1) either from the command line, use pydoc:
-    ```bash
-    pydoc mcp2221
-    ```
+
+```bash
+pydoc mcp2221
+```
+
 2) or from within python:
-    ```python
-    import mcp2221; help(mcp2221)
-    ```
+
+```python
+import mcp2221; help(mcp2221)
+```
```

### Comparing `pymcp2221-1.0.6/mcp2221/__init__.py` & `pymcp2221-1.0.7/mcp2221/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,17 @@
         """Class constructor.
 
         Parameters:
             dev_descriptor(dict): the device descriptor to open device from.
                                   Use find_devices to obtain one. (default None)
             password(str): 8 byte password to modify flash content (default "")
 
+        Raises:
+            IOException: if device was provided and device couldn't be opened.
+
         Note:
             If dev_descriptor is provided, device is opened automatically. If you
             don't want this to happen, provide no descriptor and use open() method
             at a later time.
         """
         self._opened = False
         self._password = password
@@ -128,24 +131,29 @@
 
         Parameters:
             dev_descriptor(dict): the device descriptor to open device from.
                                   Use find_devices to obtain one.
         
         Returns:
             bool: True if device could be opened, False otherwise.
+        
+        Raises:
+            IOException: if device couldn't be opened.
         """
         if self._opened == True: return False
         # create hidapi device instance
         self.dev = hid.device()
         try:
             self.dev.open_path(dev_descriptor["path"])
             self.dev.set_nonblocking(True)
             self._opened = True
-        except OSError:
+        except (OSError, IOError):
             self._opened = False
+            raise IOException("Can't open device. Check that the device descriptor exists and that you have access permissions.")
+
         return self._opened
     
     @property
     def opened(self) -> bool:
         """Tells if a device associated with this instance
         is currently opened.
```

### Comparing `pymcp2221-1.0.6/mcp2221/enums.py` & `pymcp2221-1.0.7/mcp2221/enums.py`

 * *Files identical despite different names*

### Comparing `pymcp2221-1.0.6/mcp2221/exceptions.py` & `pymcp2221-1.0.7/mcp2221/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymcp2221-1.0.6/pymcp2221.egg-info/PKG-INFO` & `pymcp2221-1.0.7/pymcp2221.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcp2221
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python driver for the Microchip MCP2221/MCP2221A USB 2.0 to I2C/UART protocol converters.
 Home-page: https://github.com/vpaeder/pymcp2221
 Author: Vincent Paeder
 Author-email: python@paeder.fi
 Project-URL: Bug Tracker, https://github.com/vpaeder/pymcp2221/issues
 Keywords: MCP2221,MCP2221A,Microchip
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,22 +14,25 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Communications
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB)
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB) :: Human Interface Device (HID)
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # pymcp2221
+
 This is a python driver for the Microchip MCP2221/MCP2221A USB 2.0 to I2C/UART protocol converters
 ([manufacturer's page](https://www.microchip.com/en-us/product/MCP2221A)).
 
 First and foremost, there are python packages for the same chip available [here](https://github.com/nonNoise/PyMCP2221A) and [here](https://github.com/pilotak/python-mcp2221). If you use them and are satisfied, you probably won't find improvements in my package. If you're missing some features however, my code is meant to expose every chip feature described in the datasheet in a systematic manner, for python 3.2+.
 
-##### Implemented features
+## Implemented features
+
 - Status/Set Parameters (0x10) - ok
 - Read Flash Data (0xB0) - ok
 - Write Flash Data (0xB1) - ok
 - Send Flash Access Password (0xB2) - ok
 - I2C Write Data (0x90) - ok
 - I2C Write Data Repeated Start (0x92) - ok
 - I2C Write Data No Stop (0x94) - ok
@@ -39,38 +42,54 @@
 - Get GPIO Values (0x51) - ok
 - Set SRAM Settings (0x60) - ok, except GPIO directions/values through SRAM (duplicate with 0x50)
 - Get SRAM Settings (0x61) - ok, except GPIO directions/values through SRAM (duplicate with 0x51)
 - Reset Chip (0x70) - ok
 
 Every feature marked *ok* is implemented, but some of them, like I2C, haven't been tested in real conditions.
 
-# Requirements
+## Requirements
+
 - [hidapi](https://pypi.org/project/hidapi)
 
-# Setup
+## Setup
+
 From command line, use:
 
-    python setup.py install
+```bash
+python setup.py install
+```
 
 or for Linux/OSX:
 
-    sudo python setup.py install
+```bash
+sudo python setup.py install
+```
+
+On Linux, to access your devices without root privileges, you need to set specific udev rules, as explained in [hidapi documentation](https://github.com/trezor/cython-hidapi#udev-rules).
+
+## Examples
 
-# Examples
 See [examples](examples) folder.
 
-# Tests
+## Tests
+
 The [tests](tests) folder contains unit tests for most of the aspects of this package. To run them, use:
 
-    python -m unittest
+```bash
+python -m unittest
+```
+
+## API
 
-# API
 You can find docs in the [docs](docs) folder (generated from python docstrings). Alternatively, you can rely on python docstrings
 
 1) either from the command line, use pydoc:
-    ```bash
-    pydoc mcp2221
-    ```
+
+```bash
+pydoc mcp2221
+```
+
 2) or from within python:
-    ```python
-    import mcp2221; help(mcp2221)
-    ```
+
+```python
+import mcp2221; help(mcp2221)
+```
```

### Comparing `pymcp2221-1.0.6/setup.py` & `pymcp2221-1.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymcp2221",
-    version="1.0.6",
+    version="1.0.7",
     author="Vincent Paeder",
     author_email="python@paeder.fi",
     description="Python driver for the Microchip MCP2221/MCP2221A USB 2.0 to I2C/UART protocol converters.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=['MCP2221', 'MCP2221A', 'Microchip'],
     url="https://github.com/vpaeder/pymcp2221",
```

### Comparing `pymcp2221-1.0.6/tests/comm.py` & `pymcp2221-1.0.7/tests/comm.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
     def test_open_ok(self):
         with patch("hid.device"):
             self.mcp.open({"path":b""})
             self.assertTrue(self.mcp._opened)
 
     def test_open_fail(self):
-        self.mcp.open({"path":b""})
+        with self.assertRaises(IOException):
+            self.mcp.open({"path":b""})
         self.assertFalse(self.mcp._opened)
     
     def test_open_no_path(self):
         with self.assertRaises(KeyError):
             self.mcp.open({"nopath":""})
     
     def test_close(self):
```

### Comparing `pymcp2221-1.0.6/tests/common.py` & `pymcp2221-1.0.7/tests/common.py`

 * *Files identical despite different names*

### Comparing `pymcp2221-1.0.6/tests/gpio.py` & `pymcp2221-1.0.7/tests/gpio.py`

 * *Files identical despite different names*

### Comparing `pymcp2221-1.0.6/tests/i2c.py` & `pymcp2221-1.0.7/tests/i2c.py`

 * *Files identical despite different names*

### Comparing `pymcp2221-1.0.6/tests/memory.py` & `pymcp2221-1.0.7/tests/memory.py`

 * *Files identical despite different names*

### Comparing `pymcp2221-1.0.6/tests/misc.py` & `pymcp2221-1.0.7/tests/misc.py`

 * *Files identical despite different names*

### Comparing `pymcp2221-1.0.6/tests/settings_flash.py` & `pymcp2221-1.0.7/tests/settings_flash.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 __all__ = ["TestReadFlashChipSettings", "TestWriteFlashChipSettings",
            "TestReadFlashUSBDescriptors", "TestWriteFlashUSBDescriptors",
            "TestReadFlashGPSettings", "TestWriteFlashGPSettings"]
 
 class TestReadFlashChipSettings(MCPTestWithReadMock):
     def setUp(self):
         super().setUp()
-        self.xb0_00[4:] = bytearray(64)
+        self.xb0_00[4:] = bytearray(60)
         self.mcp._read_response.return_value = self.xb0_00
         self.mcp.set_default_memory_target(MemoryType.Flash)
 
     def test_read_cdc_sn_enumeration_enable(self):
         self.do_test_read_func_bit(self.mcp.read_cdc_sn_enumeration_enable, 4, 7)
         self.do_test_read_prop_bit("cdc_sn_enumeration_enable_flag", 4, 7)
```

### Comparing `pymcp2221-1.0.6/tests/settings_sram.py` & `pymcp2221-1.0.7/tests/settings_sram.py`

 * *Files identical despite different names*

### Comparing `pymcp2221-1.0.6/tests/status.py` & `pymcp2221-1.0.7/tests/status.py`

 * *Files identical despite different names*

