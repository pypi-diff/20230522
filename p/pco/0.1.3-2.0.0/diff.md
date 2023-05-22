# Comparing `tmp/pco-0.1.3.tar.gz` & `tmp/pco-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pco-0.1.3.tar", last modified: Mon Sep 21 13:57:44 2020, max compression
+gzip compressed data, was "pco-2.0.0.tar", last modified: Fri May 12 14:23:03 2023, max compression
```

## Comparing `pco-0.1.3.tar` & `pco-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxrwxrwx   0        0        0        0 2020-09-21 13:57:44.469009 pco-0.1.3/
--rw-rw-rw-   0        0        0    15666 2020-09-21 13:57:44.468012 pco-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    11578 2020-04-07 13:32:25.000000 pco-0.1.3/README.rst
-drwxrwxrwx   0        0        0        0 2020-09-21 13:57:44.448011 pco-0.1.3/pco/
--rw-rw-rw-   0        0        0  5619256 2020-06-19 08:00:28.000000 pco-0.1.3/pco/PCO_File.dll
--rw-rw-rw-   0        0        0   682296 2020-09-21 13:09:31.000000 pco-0.1.3/pco/PCO_Recorder.dll
--rw-rw-rw-   0        0        0   522296 2020-09-07 07:12:19.000000 pco-0.1.3/pco/SC2_Cam.dll
--rw-rw-rw-   0        0        0      119 2020-04-07 13:24:44.000000 pco-0.1.3/pco/__init__.py
--rw-rw-rw-   0        0        0    23051 2020-09-07 09:51:30.000000 pco-0.1.3/pco/camera.py
--rw-rw-rw-   0        0        0    37348 2020-04-07 06:21:03.000000 pco-0.1.3/pco/recorder.py
--rw-rw-rw-   0        0        0   356232 2019-10-23 10:52:23.000000 pco-0.1.3/pco/sc2_cl_me4.dll
--rw-rw-rw-   0        0        0   391560 2019-10-23 10:52:23.000000 pco-0.1.3/pco/sc2_clhs.dll
--rw-rw-rw-   0        0        0   200193 2020-09-07 11:34:09.000000 pco-0.1.3/pco/sdk.py
-drwxrwxrwx   0        0        0        0 2020-09-21 13:57:44.465012 pco-0.1.3/pco.egg-info/
--rw-rw-rw-   0        0        0    15666 2020-09-21 13:57:43.000000 pco-0.1.3/pco.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2020-09-21 13:57:43.000000 pco-0.1.3/pco.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-09-21 13:57:43.000000 pco-0.1.3/pco.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2020-09-21 13:57:43.000000 pco-0.1.3/pco.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2020-09-21 13:57:43.000000 pco-0.1.3/pco.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-09-21 13:57:44.469009 pco-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1909 2020-09-21 13:57:21.000000 pco-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:23:03.160584 pco-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2023-05-12 07:13:25.000000 pco-2.0.0/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-05-12 07:13:25.000000 pco-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12964 2023-05-12 14:23:03.160584 pco-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11547 2023-05-12 07:13:25.000000 pco-2.0.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)   104867 2023-05-12 07:13:26.000000 pco-2.0.0/license.pdf
+-rw-rw-rw-   0 root         (0) root         (0)   105021 2023-05-12 07:13:26.000000 pco-2.0.0/license_3rdParty.pdf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:23:03.152584 pco-2.0.0/pco/
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-05-12 14:23:02.000000 pco-2.0.0/pco/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-05-12 07:13:25.000000 pco-2.0.0/pco/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    59049 2023-05-12 07:13:25.000000 pco-2.0.0/pco/camera.py
+-rw-rw-rw-   0 root         (0) root         (0)    48437 2023-05-12 07:13:25.000000 pco-2.0.0/pco/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)    12517 2023-05-12 07:13:25.000000 pco-2.0.0/pco/flim.py
+-rw-r--r--   0 root         (0) root         (0)   104867 2023-05-12 14:23:02.000000 pco-2.0.0/pco/license.pdf
+-rw-r--r--   0 root         (0) root         (0)   105021 2023-05-12 14:23:02.000000 pco-2.0.0/pco/license_3rdParty.pdf
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-05-12 07:13:25.000000 pco-2.0.0/pco/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)    38376 2023-05-12 07:13:25.000000 pco-2.0.0/pco/recorder.py
+-rw-rw-rw-   0 root         (0) root         (0)   283652 2023-05-12 07:13:25.000000 pco-2.0.0/pco/sdk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:23:03.156584 pco-2.0.0/pco.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12964 2023-05-12 14:23:03.000000 pco-2.0.0/pco.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      376 2023-05-12 14:23:03.000000 pco-2.0.0/pco.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 14:23:03.000000 pco-2.0.0/pco.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-12 14:23:03.000000 pco-2.0.0/pco.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-12 14:23:03.000000 pco-2.0.0/pco.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-12 14:23:03.160584 pco-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     5215 2023-05-12 07:13:25.000000 pco-2.0.0/setup.py
```

### Comparing `pco-0.1.3/README.rst` & `pco-2.0.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,369 +1,401 @@
-
-.. image:: https://www.pco.de/fileadmin/user_upload/company/pco_logo.png
-   :width: 100pt
-
-|PyPI-Versions| |LICENCE| |Platform| |PyPI-Status|
-
-The Python package **pco** offers all functions for working with pco cameras that are based
-on the current SDK. All shared libraries for the communication with the
-camera and subsequent image processing are included.
-
-- Easy to use camera class
-- Powerful API to `pco.software development kit <https://www.pco.de/fileadmin/user_upload/pco-manuals/pco.sdk_manual.pdf>`_
-- Image recording and processing with `pco.recorder <https://www.pco.de/fileadmin/fileadmin/user_upload/pco-manuals/pco.recorder_manual.pdf>`_
-
-Installation
-============
-Install from pypi (recommended)::
-
-    $ pip install pco
-
-Basic Usage
-===========
-.. code-block:: python
-
-    import pco
-    import matplotlib.pyplot as plt
-
-    with pco.Camera() as cam:
-
-        cam.record()
-        image, meta = cam.image()
-
-        plt.imshow(image, cmap='gray')
-        plt.show()
-
-.. image:: https://www.pco.de/fileadmin/user_upload/company/screen.png
-
-Logging
-=======
-To activate the logging output create the ``Camera`` object with
-``debuglevel=`` parameter.
-
-The debug level can be set to one of the following values:
-
-- ``'off'`` Disables all output.
-- ``'error'`` Shows only error messages.
-- ``'verbose'`` Shows all messages.
-- ``'extra verbose'`` Shows all messages and values.
-
-The default debuglevel is ``'off'``.
-
-.. code-block:: python
-
-    pco.Camera(debuglevel='verbose')
-    ...
-    [][sdk] get_camera_type: OK.
-
-The optional ``timestamp=`` parameter activates a tag in the printed output.
-Possible values are: ``'on'`` and ``'off'``.
-
-The default value is ``'off'``.
-
-.. code-block:: python
-
-    pco.Camera(debuglevel='verbose', timestamp='on')
-    ...
-    [2019-11-25 15:54:15.317855 / 0.016 s] [][sdk] get_camera_type: OK.
-
-
-Documentation
-=============
-
-The pco.Camera class offers following methods:
-
-- `record()`_ generates, configures and starts a new recorder instance.
-- `stop()`_ stops the current recording.
-- `close()`_ closes the current active camera and releases the blocked ressources.
-- `image()`_ returns an image from the recorder as numpy array.
-- `images()`_ returns all recorded images from the recorder as list of numpy arrays.
-- `image_average()`_ returns the averaged image. This image is calculated from all recorded images in the buffer.
-- `set_exposure_time()`_ sets the exposure time of the camera.
-- `wait_for_first_image()`_ waits for the first available image in the recorder memory.
-
-The pco.Camera class has the following variables:
-
-- `configuration`_
-
-The pco.Camera class has the following objects:
-
-- `sdk`_ offers direct access to all underlying functions of the pco.sdk.
-- `recorder`_ offers direct access to all underlying functions of the pco.recorder.
-
-
-.. ---------------------------------------------------------------------------
-
-record()
---------
-
-Creates, configures and starts a new recorder instance.
-
-.. code-block:: python
-
-    def record(self, number_of_images=1, mode='sequence'):
-
-- ``number_of_images`` sets the number of images allocated in the driver. The RAM of the PC is limiting the maximum value.
-
-- ``mode`` sets the type of recorder:
-
-  - In ``'sequence'`` mode this function is blocking during record.
-    The recorder stops automatically when the ``number_of_images`` is reached.
-
-  - In ``'sequence non blocking'`` mode this function is non blocking.
-    Status must be checked before reading an image. This mode is used
-    to read images while recording, e.g. thumbnail.
-
-  - In ``'ring buffer'`` mode this function is non blocking.
-    Status must be checked before reading an image.
-    Recorder did not stop the recording when the ``number_of_images`` is reached.
-    The first image is overwritten from the next image.
-
-  - In ``'fifo'`` mode this function is non blocking.
-    Status must be checked before reading an image.
-    When the ``number_of_images`` in the fifo is reached, the following images are dropped
-    until images were read from the fifo.
-
-The entire camera configuration must be set before calling ``record()``.
-The ``set_exposure_time()`` command is the only exception. 
-This function has no effect on the recorder object and can be called up during 
-the recording.
-
-.. ---------------------------------------------------------------------------
-
-stop()
-------
-
-Stops the current recording.
-
-.. code-block:: python
-
-    def stop(self):
-
-In ``'ring buffer'`` and ``'fifo'`` mode this function must to be called by the user.
-In ``'sequence'`` and ``'sequence non blocking'`` mode, this function is automatically called up
-when the ``number_of_images`` is reached.
-
-
-.. ---------------------------------------------------------------------------
-
-close()
--------
-.. code-block:: python
-
-    def close(self):
-
-Closes the activated camera and releases the blocked ressources.
-This function must be called before the application is terminated.
-Otherwise the resources remain occupied.
-
-This function is called automatically, if the camera object is
-created by the ``with`` statement. An explicit call to ``close()`` is no
-longer necessary.
-
-.. code-block:: python
-
-    with pco.Camera() as cam:
-        # do some stuff
-
-
-.. ---------------------------------------------------------------------------
-
-image()
--------
-
-Returns an image from the recorder. The type of the image is a ``numpy.ndarray``.
-This array is shaped depending on the resolution and ROI of the image.
-
-.. code-block:: python
-
-    def image(self, image_number=0, roi=None):
-
-- ``image_number`` specifies the number of the image to read. In ``'sequence'`` or ``'sequence non blocking'`` mode the recorder
-  index matches the image number.
-  If ``image_number`` is set to ``0xFFFFFFFF`` the last recorded image is copied. This allows
-  e.g. thumbnail while recording.
-
-- ``roi`` sets the region fo interest. Only this region of the image is copied to the return value.
-
-  .. code-block:: python
-
-      >>> cam.record(number_of_images=1, mode='sequence')
-
-      >>> image, meta = cam.image()
-
-      >>> type(image)
-      numpy.ndarray
-
-      >>> image.shape
-      (2160, 2560)
-
-      >>> image, metadata = cam.image(roi=(1, 1, 300, 300))
-
-      >>> image.shape
-      (300, 300)
-
-.. ---------------------------------------------------------------------------
-
-images()
---------
-
-Returns all recorded images from the recorder as list of numpy arrays.
-
-.. code-block:: python
-
-    def images(self, roi=None, blocksize=None):
-
-- ``roi`` sets the region fo interest. Only this region of the image is copied to the return value.
-
-- ``blocksize`` defines the maximum number of images that are returned.
-  This parameter is only useful in ``'fifo'`` mode and under special conditions.
-
-  .. code-block:: python
-
-      >>> cam.record(number_of_images=20, mode='sequence')
-
-      >>> images, metadatas = cam.images()
-
-      >>> len(images)
-      20
-
-      >>> for image in images:
-      ...     print('Mean: {:7.2f} DN'.format(image.mean()))
-      ...
-      Mean: 2147.64 DN
-      Mean: 2144.61 DN
-      ...
-
-     >>> images = cam.images(roi=(1, 1, 300, 300))
-     
-     >>> images[0].shape
-    (300, 300)
-
-.. ---------------------------------------------------------------------------
-
-image_average()
-------------------------
-
-Returns the averaged image. This image is calculated from all recorded images in the buffer.
-
-.. code-block:: python
-
-    def image_average(self, roi=None):
-
-- ``roi`` defines the region fo interest. Only this region of the image is copied to the return value.
-
-  .. code-block:: python
-
-      >>> cam.record(number_of_images=100, mode='sequence')
-
-      >>> avg = cam.image_average()
-
-      >>> avg = cam.image_average(roi=(1, 1, 300, 300))
-
-.. ---------------------------------------------------------------------------
-
-set_exposure_time()
--------------------
-
-Sets the exposure time of the camera.
-
-.. code-block:: python
-
-    def set_exposure_time(self, exposure_time): 
-
-- ``exposure_time`` must be given as float or integer value in the unit 'second'.
-  The underlying values for the function ``sdk.set_delay_exposure_time(0, 'ms', time, timebase)``
-  will be calculated automatically. The delay time is set to 0.
-
-  .. code-block:: python
-
-      >>> set_exposure_time(0.001)
-
-      >>> set_exposure_time(1e-3)
-
-.. ---------------------------------------------------------------------------
-
-wait_for_first_image()
--------------------------
-Waits for the first available image in the recorder memory.
-
-.. code-block:: python
-
-    def wait_for_first_image(self):
-
-In recorder mode ``'sequence non blocking'``, ``'ring buffer'`` and ``'fifo'``,
-the function ``record()`` returns immediately.
-It is the responsibility of the user to wait for images from the 
-camera before calling ``image()``, ``images()`` or ``image_average``.
-
-.. ---------------------------------------------------------------------------
-
-configuration
--------------
-
-The camera parameters are updated by changing the ``configuration`` variable.
-
-.. code-block:: python
-
-    cam.configuration = {'exposure time': 10e-3,
-                         'roi': (1, 1, 512, 512),
-                         'timestamp': 'ascii',
-                         'pixel rate': 100_000_000,
-                         'trigger': 'auto sequence',
-                         'acquire': 'auto',
-                         'metadata': 'on',
-                         'binning': (1, 1)}
-
-The variable can only be changed before the ``record()`` function is called.
-It's a dictionary with a certain number of entries.
-Not all possible elements need to be specified. The following sample code only changes 
-the ``'pixel rate'`` and does not affect any other elements of the configuration.
-
-
-.. code-block:: python
-
-    with pco.Camera() as cam:
-
-        cam.configuration = {'pixel rate': 286_000_000}
-
-        cam.record()
-        ...
-
-.. ---------------------------------------------------------------------------
-
-
-sdk
----
-The object ``sdk`` allows direct access to all underlying functions of the pco.sdk.
-
-.. code-block:: python
-
-       >>> cam.sdk.get_temperature()
-       {'sensor temperature': 7.0, 'camera temperature': 38.2, 'power temperature': 36.7}
-
-All return values form ``sdk`` functions are dictionarys.
-Not all camera settings are currently covered by the ``camera`` class.
-Special settings have to be set directly  by calling the respective SDK function.
-
-.. ---------------------------------------------------------------------------
-
-recorder
---------
-
-The object ``rec`` offers direct access to all underlying functions of the pco.recorder.
-It is not necessary to call a recorder class method directly. 
-All functions are fully covered by the methods of the ``camera`` class.
-
-
-
-.. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/pco.svg
-   :target: https://pypi.python.org/pypi/pco
-
-.. |LICENCE| image:: https://img.shields.io/badge/License-MIT-green.svg
-   :target: https://opensource.org/licenses/MIT
-
-.. |Platform| image:: https://img.shields.io/badge/platform-win_x64-green.svg
-   :target: https://pypi.python.org/pypi/pco
-   
-.. |PyPI-Status| image:: https://img.shields.io/pypi/v/pco.svg
-  :target: https://pypi.python.org/pypi/pco
+
+.. image:: https://www.pco.de/fileadmin/user_upload/company/pco_logo.png
+   :width: 100pt
+
+|PyPI-Versions| |LICENCE| |Platform| |PyPI-Status|
+
+The Python package **pco** offers all functions for working with pco cameras that are based
+on the current SDK. All shared libraries for the communication with the
+camera and subsequent image processing are included.
+
+- Easy to use camera class
+- Powerful API to `pco.software development kit <https://www.pco.de/fileadmin/user_upload/pco-manuals/pco.sdk_manual.pdf>`_
+- Image recording and processing with `pco.recorder <https://www.pco.de/fileadmin/fileadmin/user_upload/pco-manuals/pco.recorder_manual.pdf>`_
+
+Installation
+============
+Install from pypi (recommended)::
+
+    $ pip install pco
+
+Basic Usage
+===========
+.. code-block:: python
+
+    import pco
+    import matplotlib.pyplot as plt
+
+    with pco.Camera() as cam:
+
+        cam.record()
+        image, meta = cam.image()
+
+        plt.imshow(image, cmap='gray')
+        plt.show()
+
+.. image:: https://www.pco.de/fileadmin/user_upload/company/screen.png
+
+Logging
+=======
+
+Logging is implemented according to the python logging package (https://docs.python.org/3/library/logging.html).
+Supported logging levels are:
+- `ERROR`
+- `WARNING`
+- `INFO`
+- `DEBUG`
+
+
+.. code-block:: python
+
+    logger = logging.getLogger("pco")
+    logger.setLevel(logging.INFO)
+    logger.addHandler(pco.stream_handler)
+
+
+
+.. code-block:: python
+
+    ...
+    [][sdk] get_camera_type: OK.
+    ...
+    [2019-11-25 15:54:15.317855 / 0.016 s] [][sdk] get_camera_type: OK.
+
+
+Documentation
+=============
+
+The pco.Camera class offers the following methods:
+
+- ``__init()__`` Opens and initializes a camera with its default configuration
+- ``__exit()__`` Closes the camera and cleans up everything (e.g. end of with-statement)
+- ``default_configuration()`` Set default configuration to the camera
+- `record()`_ Initialize and start the recording of images
+- `stop()`_ Stop the current recording
+- `close()`_ Closes the camera and cleans up everything
+- `wait_for_first_image()`_ Wait until the first image has been recorded
+- `wait_for_new_image()`_ Wait until a new image has been recorded
+- ``get_convert_control()`` Get current color convert settings
+- ``set_convert_control()`` Set new color convert settings
+- ``load_lut()`` Set the lut file for the convert control setting
+- ``adapt_white_balance()`` Do a white-balance according to a transferred image
+- `image()`_ Read a recorded image as numpy array
+- `images()`_ Read a series of recorded images as a list of numpy arrays.
+- `image_average()`_ Read an averaged image (averaged over all recorded images) as numpy array.
+
+The pco.Camera class has the following properties:
+
+- ``camera_name`` gets the camera name
+- ``camera_serial`` gets the serial number of the camera
+- ``is_recording`` gets a flag to indicate if the camera is currently recording
+- ``is_color`` gets a flag to indicate if the camera is a color camera
+- ``recorded_image_count`` gets the number of currently recorded images
+- ``configuration`` gets/sets the camera configuration
+- ``description`` gets the (static) camera description parameters
+- ``exposure_time`` gets/sets the exposure time (in seconds)
+- ``delay_time`` gets/sets the delay time (in seconds)
+
+The pco.Camera class holds the following objects:
+
+- `sdk`_ offers direct access to all underlying functions of the pco.sdk.
+- `rec`_ offers direct access to all underlying functions of the pco.recorder.
+- `conv`_ offers direct access to all underlying functions of the pco.convert according to the selected data_format.
+
+.. ---------------------------------------------------------------------------
+
+record()
+--------
+
+Creates, configures and starts a new recorder instance.
+
+.. code-block:: python
+
+    def record(self, number_of_images=1, mode='sequence', file_path=None):
+
+- ``number_of_images`` sets the number of images allocated in the driver. The RAM of the PC is limiting the maximum value.
+
+- ``mode`` sets the type of recorder.
+
+.. list-table:: record modes
+  :widths: 20 10 10 60
+  :header-rows: 1
+
+  * - Mode
+    - Storage
+    - Blocking
+    - Description
+  
+  * - ``sequence``
+    - Memory
+    - yes
+    - Record a sequence of images
+  
+  * - ``sequence non blocking``
+    - Memory
+    - no 
+    - Record a sequence of images, do not wait until record is finished
+  
+  * - ``ring buffer``
+    - Memory
+    - no 
+    - Continuously record images in a ringbuffer, once the buffer is full, old images are overwritten
+  
+  * - ``fifo``
+    - Memory
+    - no 
+    - Record images in fifo mode, i.e. you will always read images sequentially and once the buffer is full, recording will pause until older images have been read
+  
+  * - ``sequence dpcore``
+    - Memory
+    - yes
+    - Same as ``sequence``, but with DotPhoton preparation enabled
+  
+  * - ``sequence non blocking dpcore``
+    - Memory
+    - no 
+    - Same as ``sequence_non_blocking``, but with DotPhoton preparation enabled
+  
+  * - ``ring buffer dpcore``
+    - Memory
+    - no 
+    - Same as ``ring_buffer``, but with DotPhoton preparation enabled
+  
+  * - ``fifo dpcore``
+    - Memory
+    - no 
+    - Same as ``fifo``, but with DotPhoton preparation enabled
+  
+  * - ``tif``
+    - File  
+    - no 
+    - Record images directly as tif files  
+  
+  * - ``multitif``
+    - File  
+    - no 
+    - Record images directly as one or more multitiff file()s 
+  
+  * - ``pcoraw``
+    - File  
+    - no 
+    - Record images directly as one pcoraw file  
+  
+  * - ``dicom``
+    - File  
+    - no 
+    - Record images directly as dicom files
+  
+  * - ``multidicom``
+    - File  
+    - no 
+    - Record images directly as one or more multi-dicom file(s)
+
+- ``file_path`` Path where the image file(s) should be stored (only for modes who directly save to file)
+
+.. ---------------------------------------------------------------------------
+
+stop()
+------
+
+Stops the current recording.
+
+.. code-block:: python
+
+    def stop(self):
+
+In ``'ring buffer'`` and ``'fifo'`` mode this function must to be called by the user.
+In ``'sequence'`` and ``'sequence non blocking'`` mode, this function is automatically called up
+when the ``number_of_images`` is reached.
+
+
+.. ---------------------------------------------------------------------------
+
+close()
+-------
+.. code-block:: python
+
+    def close(self):
+
+Closes the activated camera and releases the blocked ressources.
+This function must be called before the application is terminated.
+Otherwise the resources remain occupied.
+
+This function is called automatically, if the camera object is
+created by the ``with`` statement. An explicit call to ``close()`` is no
+longer necessary.
+
+.. code-block:: python
+
+    with pco.Camera() as cam:
+        # do some stuff
+
+
+.. ---------------------------------------------------------------------------
+
+image()
+-------
+
+Returns an image from the recorder. The type of the image is a ``numpy.ndarray``.
+This array is shaped depending on the resolution and ROI of the image.
+
+.. code-block:: python
+
+    def image(self, image_number=0, roi=None):
+
+- ``image_number`` specifies the number of the image to read. In ``'sequence'`` or ``'sequence non blocking'`` mode the recorder
+  index matches the image number.
+  If ``image_number`` is set to ``0xFFFFFFFF`` the last recorded image is copied. This allows
+  e.g. thumbnail while recording.
+
+- ``roi`` sets the region fo interest. Only this region of the image is copied to the return value.
+
+  .. code-block:: python
+
+      >>> cam.record(number_of_images=1, mode='sequence')
+
+      >>> image, meta = cam.image()
+
+      >>> type(image)
+      numpy.ndarray
+
+      >>> image.shape
+      (2160, 2560)
+
+      >>> image, metadata = cam.image(roi=(1, 1, 300, 300))
+
+      >>> image.shape
+      (300, 300)
+
+.. ---------------------------------------------------------------------------
+
+images()
+--------
+
+Returns all recorded images from the recorder as list of numpy arrays.
+
+.. code-block:: python
+
+    def images(self, roi=None, blocksize=None):
+
+- ``roi`` sets the region fo interest. Only this region of the image is copied to the return value.
+
+- ``blocksize`` defines the maximum number of images that are returned.
+  This parameter is only useful in ``'fifo'`` mode and under special conditions.
+
+  .. code-block:: python
+
+      >>> cam.record(number_of_images=20, mode='sequence')
+
+      >>> images, metadatas = cam.images()
+
+      >>> len(images)
+      20
+
+      >>> for image in images:
+      ...     print('Mean: {:7.2f} DN'.format(image.mean()))
+      ...
+      Mean: 2147.64 DN
+      Mean: 2144.61 DN
+      ...
+
+     >>> images = cam.images(roi=(1, 1, 300, 300))
+     
+     >>> images[0].shape
+    (300, 300)
+
+.. ---------------------------------------------------------------------------
+
+image_average()
+------------------------
+
+Returns the averaged image. This image is calculated from all recorded images in the buffer.
+
+.. code-block:: python
+
+    def image_average(self, roi=None):
+
+- ``roi`` defines the region fo interest. Only this region of the image is copied to the return value.
+
+  .. code-block:: python
+
+      >>> cam.record(number_of_images=100, mode='sequence')
+
+      >>> avg = cam.image_average()
+
+      >>> avg = cam.image_average(roi=(1, 1, 300, 300))
+
+
+.. ---------------------------------------------------------------------------
+
+wait_for_first_image()
+-------------------------
+Waits for the first available image in the recorder memory.
+
+.. code-block:: python
+
+    def wait_for_first_image(self, delay=True, timeout=None):
+
+
+.. ---------------------------------------------------------------------------
+
+wait_for_new_image()
+-------------------------
+Wait until a new image has been recorded and is available (i.e. an image that has not been read
+yet).
+
+.. code-block:: python
+
+    def wait_for_new_image(self, delay=True, timeout=None):
+
+
+.. ---------------------------------------------------------------------------
+
+sdk
+---
+The object ``sdk`` allows direct access to all underlying functions of the pco.sdk.
+
+.. code-block:: python
+
+       >>> cam.sdk.get_temperature()
+       {'sensor temperature': 7.0, 'camera temperature': 38.2, 'power temperature': 36.7}
+
+All return values form ``sdk`` functions are dictionarys.
+Not all camera settings are currently covered by the ``camera`` class.
+Special settings have to be set directly  by calling the respective SDK function.
+
+.. ---------------------------------------------------------------------------
+
+rec
+--------
+
+The object ``rec`` offers direct access to all underlying functions of the pco.recorder.
+It is not necessary to call a recorder class method directly. 
+All functions are fully covered by the methods of the ``camera`` class.
+
+
+.. ---------------------------------------------------------------------------
+
+conv
+--------
+
+The object ``conv``  is a dictionary of convert objects to offer direct access to all
+underlying functions of the pco.convert.
+It is not necessary to call a ``conv`` class method directly. 
+All functions are fully covered by the methods of the ``camera`` class.
+
+
+
+
+
+.. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/pco.svg
+   :target: https://pypi.python.org/pypi/pco
+
+.. |LICENCE| image:: https://img.shields.io/badge/License-MIT-green.svg
+   :target: https://opensource.org/licenses/MIT
+
+.. |Platform| image:: https://img.shields.io/badge/platform-win_x64%20%7C%20linux_x64-green.svg
+   :target: https://pypi.python.org/pypi/pco
+   
+.. |PyPI-Status| image:: https://img.shields.io/pypi/v/pco.svg
+  :target: https://pypi.python.org/pypi/pco
+
```

