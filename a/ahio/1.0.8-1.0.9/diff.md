# Comparing `tmp/ahio-1.0.8.tar.gz` & `tmp/ahio-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ahio-1.0.8.tar", last modified: Mon May 14 11:57:12 2018, max compression
+gzip compressed data, was "dist/ahio-1.0.9.tar", last modified: Fri May 25 11:19:11 2018, max compression
```

## Comparing `ahio-1.0.8.tar` & `ahio-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwx------   0 Alan       (501) staff       (20)        0 2018-05-14 11:57:12.000000 ahio-1.0.8/
--rw-------   0 Alan       (501) staff       (20)     3151 2018-05-14 11:57:12.000000 ahio-1.0.8/PKG-INFO
-drwx------   0 Alan       (501) staff       (20)        0 2018-05-14 11:57:12.000000 ahio-1.0.8/ahio/
-drwx------   0 Alan       (501) staff       (20)        0 2018-05-14 11:57:12.000000 ahio-1.0.8/ahio/drivers/
--rwx------   0 Alan       (501) staff       (20)     9733 2017-04-13 23:00:59.000000 ahio-1.0.8/ahio/drivers/generic_tcp_io.py
--rwx------   0 Alan       (501) staff       (20)     5148 2018-05-14 11:30:06.000000 ahio-1.0.8/ahio/drivers/__init__.py
--rwx------   0 Alan       (501) staff       (20)     7224 2016-12-02 12:19:38.000000 ahio-1.0.8/ahio/drivers/snap7.py
--rwx------   0 Alan       (501) staff       (20)     6944 2018-02-22 17:39:17.000000 ahio-1.0.8/ahio/drivers/raspberry.py
--rwx------   0 Alan       (501) staff       (20)     2753 2018-04-13 22:54:50.000000 ahio-1.0.8/ahio/drivers/dummy.py
--rwx------   0 Alan       (501) staff       (20)     7442 2017-11-10 21:54:22.000000 ahio-1.0.8/ahio/drivers/arduino.py
--rwx------   0 Alan       (501) staff       (20)     3717 2018-05-14 11:57:01.000000 ahio-1.0.8/ahio/__init__.py
--rwx------   0 Alan       (501) staff       (20)    18042 2016-12-02 12:19:25.000000 ahio-1.0.8/ahio/abstract_driver.py
-drwx------   0 Alan       (501) staff       (20)        0 2018-05-14 11:57:12.000000 ahio-1.0.8/ahio.egg-info/
--rw-------   0 Alan       (501) staff       (20)     3151 2018-05-14 11:57:12.000000 ahio-1.0.8/ahio.egg-info/PKG-INFO
--rw-------   0 Alan       (501) staff       (20)        1 2018-05-14 11:50:35.000000 ahio-1.0.8/ahio.egg-info/not-zip-safe
--rw-------   0 Alan       (501) staff       (20)      397 2018-05-14 11:57:12.000000 ahio-1.0.8/ahio.egg-info/SOURCES.txt
--rw-------   0 Alan       (501) staff       (20)       22 2018-05-14 11:57:12.000000 ahio-1.0.8/ahio.egg-info/requires.txt
--rw-------   0 Alan       (501) staff       (20)        5 2018-05-14 11:57:12.000000 ahio-1.0.8/ahio.egg-info/top_level.txt
--rw-------   0 Alan       (501) staff       (20)        1 2018-05-14 11:57:12.000000 ahio-1.0.8/ahio.egg-info/dependency_links.txt
--rw-------   0 Alan       (501) staff       (20)       34 2016-11-08 11:29:03.000000 ahio-1.0.8/MANIFEST.in
--rw-------   0 Alan       (501) staff       (20)     1879 2016-11-08 11:32:21.000000 ahio-1.0.8/README.md
--rwx------   0 Alan       (501) staff       (20)     2470 2017-04-13 23:03:43.000000 ahio-1.0.8/setup.py
--rw-------   0 Alan       (501) staff       (20)       79 2018-05-14 11:57:12.000000 ahio-1.0.8/setup.cfg
+drwx------   0 Alan       (501) staff       (20)        0 2018-05-25 11:19:11.000000 ahio-1.0.9/
+-rw-------   0 Alan       (501) staff       (20)      783 2018-05-25 11:19:11.000000 ahio-1.0.9/PKG-INFO
+drwx------   0 Alan       (501) staff       (20)        0 2018-05-25 11:19:11.000000 ahio-1.0.9/ahio/
+drwx------   0 Alan       (501) staff       (20)        0 2018-05-25 11:19:11.000000 ahio-1.0.9/ahio/drivers/
+-rwx------   0 Alan       (501) staff       (20)     9733 2017-04-13 23:00:59.000000 ahio-1.0.9/ahio/drivers/generic_tcp_io.py
+-rwx------   0 Alan       (501) staff       (20)     5109 2018-05-25 11:02:33.000000 ahio-1.0.9/ahio/drivers/__init__.py
+-rwx------   0 Alan       (501) staff       (20)     7224 2016-12-02 12:19:38.000000 ahio-1.0.9/ahio/drivers/snap7.py
+-rwx------   0 Alan       (501) staff       (20)     6944 2018-02-22 17:39:17.000000 ahio-1.0.9/ahio/drivers/raspberry.py
+-rwx------   0 Alan       (501) staff       (20)     2753 2018-04-13 22:54:50.000000 ahio-1.0.9/ahio/drivers/dummy.py
+-rwx------   0 Alan       (501) staff       (20)     7442 2017-11-10 21:54:22.000000 ahio-1.0.9/ahio/drivers/arduino.py
+-rwx------   0 Alan       (501) staff       (20)     3717 2018-05-25 11:03:02.000000 ahio-1.0.9/ahio/__init__.py
+-rwx------   0 Alan       (501) staff       (20)    18042 2016-12-02 12:19:25.000000 ahio-1.0.9/ahio/abstract_driver.py
+drwx------   0 Alan       (501) staff       (20)        0 2018-05-25 11:19:11.000000 ahio-1.0.9/ahio.egg-info/
+-rw-------   0 Alan       (501) staff       (20)      783 2018-05-25 11:19:11.000000 ahio-1.0.9/ahio.egg-info/PKG-INFO
+-rw-------   0 Alan       (501) staff       (20)        1 2018-05-25 11:04:01.000000 ahio-1.0.9/ahio.egg-info/not-zip-safe
+-rw-------   0 Alan       (501) staff       (20)      397 2018-05-25 11:19:11.000000 ahio-1.0.9/ahio.egg-info/SOURCES.txt
+-rw-------   0 Alan       (501) staff       (20)       22 2018-05-25 11:19:11.000000 ahio-1.0.9/ahio.egg-info/requires.txt
+-rw-------   0 Alan       (501) staff       (20)        5 2018-05-25 11:19:11.000000 ahio-1.0.9/ahio.egg-info/top_level.txt
+-rw-------   0 Alan       (501) staff       (20)        1 2018-05-25 11:19:11.000000 ahio-1.0.9/ahio.egg-info/dependency_links.txt
+-rw-------   0 Alan       (501) staff       (20)       34 2016-11-08 11:29:03.000000 ahio-1.0.9/MANIFEST.in
+-rw-------   0 Alan       (501) staff       (20)     1879 2016-11-08 11:32:21.000000 ahio-1.0.9/README.md
+-rwx------   0 Alan       (501) staff       (20)     2531 2018-05-25 11:19:07.000000 ahio-1.0.9/setup.py
+-rw-------   0 Alan       (501) staff       (20)       79 2018-05-25 11:19:11.000000 ahio-1.0.9/setup.cfg
```

### Comparing `ahio-1.0.8/ahio/drivers/generic_tcp_io.py` & `ahio-1.0.9/ahio/drivers/generic_tcp_io.py`

 * *Files identical despite different names*

### Comparing `ahio-1.0.8/ahio/drivers/__init__.py` & `ahio-1.0.9/ahio/drivers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,14 @@
     however implement all APIs described in `ahio.abstract_driver`, as they'll
     be needed to use the driver.
 
     @returns the driver package, or False if it failed.
     """
     global __count
     try:
-        print('Looking for %s' % name)
         dname = os.path.basename(name).replace('.py', '')
         mod_name = 'ahio.drivers.%s%d' % (dname, __count)
         loader = importlib.machinery.SourceFileLoader(mod_name, name)
         driver = loader.load_module()
         __count += 1
         return driver if hasattr(driver, 'ahioDriverInfo') else False
     except Exception:
```

### Comparing `ahio-1.0.8/ahio/drivers/snap7.py` & `ahio-1.0.9/ahio/drivers/snap7.py`

 * *Files identical despite different names*

### Comparing `ahio-1.0.8/ahio/drivers/raspberry.py` & `ahio-1.0.9/ahio/drivers/raspberry.py`

 * *Files identical despite different names*

### Comparing `ahio-1.0.8/ahio/drivers/dummy.py` & `ahio-1.0.9/ahio/drivers/dummy.py`

 * *Files identical despite different names*

### Comparing `ahio-1.0.8/ahio/drivers/arduino.py` & `ahio-1.0.9/ahio/drivers/arduino.py`

 * *Files identical despite different names*

### Comparing `ahio-1.0.8/ahio/__init__.py` & `ahio-1.0.9/ahio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 import ahio.drivers
 
 __author__ = 'Álan Crístoffer'
 __copyright__ = 'Copyright 2016, Álan Crístoffer'
 __credits__ = ['Álan Crístoffer']
 __license__ = 'MIT'
-__version__ = '1.0.8'
+__version__ = '1.0.9'
 __maintainer__ = 'Álan Crístoffer'
 __email__ = 'acristoffers@gmail.com'
 __status__ = 'Release'
 
 PortType = Enum('PortType', 'Analog Digital')
 Direction = Enum('Direction', 'Output Input')
 LogicValue = Enum('LogicValue', 'Low High')
```

### Comparing `ahio-1.0.8/ahio/abstract_driver.py` & `ahio-1.0.9/ahio/abstract_driver.py`

 * *Files identical despite different names*

### Comparing `ahio-1.0.8/README.md` & `ahio-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ahio-1.0.8/setup.py` & `ahio-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 with open(path.join(pwd, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(name='ahio',
       version=ahio.__version__,
       description='I/O Communication Library',
-      long_description=long_description,
+      #   long_description_content_type="text/markdown",
+      #   long_description=long_description,
       # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
       classifiers=[
           'Development Status :: 5 - Production/Stable',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: MIT License',
           'Natural Language :: English',
           'Operating System :: OS Independent',
```

