# Comparing `tmp/cheap_pie-0.9.20.tar.gz` & `tmp/cheap_pie-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheap_pie-0.9.20.tar", last modified: Fri May 12 09:57:39 2023, max compression
+gzip compressed data, was "cheap_pie-1.0.0.tar", last modified: Mon May 22 21:34:10 2023, max compression
```

## Comparing `cheap_pie-0.9.20.tar` & `cheap_pie-1.0.0.tar`

### file list

```diff
@@ -1,49 +1,46 @@
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-12 09:57:39.901868 cheap_pie-0.9.20/
--rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 cheap_pie-0.9.20/LICENSE
--rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2023-05-12 09:57:39.902188 cheap_pie-0.9.20/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     8013 2023-05-11 21:25:50.000000 cheap_pie-0.9.20/README.md
--rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2023-05-12 09:57:39.902963 cheap_pie-0.9.20/setup.cfg
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1071 2023-05-12 09:20:29.000000 cheap_pie-0.9.20/setup.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-12 09:57:39.821803 cheap_pie-0.9.20/src/
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-12 09:57:39.832108 cheap_pie-0.9.20/src/cheap_pie/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/__init__.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-12 09:57:39.862509 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     7394 2023-05-06 21:35:32.000000 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cbitfield.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2205 2023-05-11 21:49:21.000000 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cheap_pie.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2873 2023-05-05 19:42:59.000000 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cp_banner.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2092 2023-05-05 19:46:51.000000 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cp_cli.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     6501 2023-05-11 21:50:54.000000 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cp_hal.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     9037 2023-05-11 21:40:13.000000 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cp_register.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2534 2023-05-11 05:47:26.000000 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/test.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-12 09:57:39.876745 cheap_pie-0.9.20/src/cheap_pie/parsers/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2088 2023-05-07 09:34:36.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/cp_parsers_wrapper.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3989 2023-05-07 09:06:44.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/ipxact_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3294 2023-05-07 08:41:29.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/ipyxact_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      430 2023-05-07 09:09:07.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/name_subs.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1026 2023-05-07 09:10:56.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/rdl_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4091 2023-05-07 09:33:12.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/svd_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4134 2023-05-07 09:35:26.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/svd_parse_repo.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1968 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/xml_xslt.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-12 09:57:39.888286 cheap_pie-0.9.20/src/cheap_pie/tools/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      156 2023-05-12 09:20:29.000000 cheap_pie-0.9.20/src/cheap_pie/tools/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     5727 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/tools/hal2doc.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1553 2022-12-12 21:51:02.000000 cheap_pie-0.9.20/src/cheap_pie/tools/rdl2any.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      890 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/tools/rdl2verilog.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      944 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/tools/reload_module.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2200 2023-05-11 21:44:55.000000 cheap_pie-0.9.20/src/cheap_pie/tools/search.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      563 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/tools/test_rdl.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-12 09:57:39.900249 cheap_pie-0.9.20/src/cheap_pie/transport/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/transport/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1775 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/transport/cp_dummy_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2289 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/transport/cp_esptool_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2027 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/transport/cp_jlink_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1985 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/transport/cp_pyocd_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     5284 2023-05-06 21:31:25.000000 cheap_pie-0.9.20/src/cheap_pie/transport/cp_pyverilator_transport.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-12 09:57:39.842349 cheap_pie-0.9.20/src/cheap_pie.egg-info/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2023-05-12 09:57:39.000000 cheap_pie-0.9.20/src/cheap_pie.egg-info/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1408 2023-05-12 09:57:39.000000 cheap_pie-0.9.20/src/cheap_pie.egg-info/SOURCES.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-05-12 09:57:39.000000 cheap_pie-0.9.20/src/cheap_pie.egg-info/dependency_links.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)      101 2023-05-12 09:57:39.000000 cheap_pie-0.9.20/src/cheap_pie.egg-info/requires.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       10 2023-05-12 09:57:39.000000 cheap_pie-0.9.20/src/cheap_pie.egg-info/top_level.txt
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-22 21:34:10.598870 cheap_pie-1.0.0/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 cheap_pie-1.0.0/LICENSE
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     8432 2023-05-22 21:34:10.599369 cheap_pie-1.0.0/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     8091 2023-05-18 10:44:55.000000 cheap_pie-1.0.0/README.md
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2023-05-22 21:34:10.600896 cheap_pie-1.0.0/setup.cfg
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1260 2023-05-22 21:32:25.000000 cheap_pie-1.0.0/setup.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-22 21:34:10.517321 cheap_pie-1.0.0/src/
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-22 21:34:10.528772 cheap_pie-1.0.0/src/cheap_pie/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      207 2023-05-22 21:21:25.000000 cheap_pie-1.0.0/src/cheap_pie/__init__.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-22 21:34:10.553938 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      211 2023-05-22 20:58:17.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     7623 2023-05-21 17:00:23.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cbitfield.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2800 2023-05-21 16:18:51.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cheap_pie_main.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3232 2023-05-18 12:45:16.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_banner.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3388 2023-05-22 19:16:36.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_builder.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2691 2023-05-21 13:23:16.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_cli.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     8613 2023-05-22 21:20:38.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_hal.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    15666 2023-05-22 20:39:24.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_register.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3669 2023-05-22 21:00:42.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/test.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-22 21:34:10.573128 cheap_pie-1.0.0/src/cheap_pie/parsers/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      163 2023-05-22 20:56:30.000000 cheap_pie-1.0.0/src/cheap_pie/parsers/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2427 2023-05-21 15:47:51.000000 cheap_pie-1.0.0/src/cheap_pie/parsers/cp_parsers_wrapper.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3161 2023-05-21 16:42:25.000000 cheap_pie-1.0.0/src/cheap_pie/parsers/ipxact_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2643 2023-05-21 16:43:35.000000 cheap_pie-1.0.0/src/cheap_pie/parsers/ipyxact_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1166 2023-05-21 13:58:09.000000 cheap_pie-1.0.0/src/cheap_pie/parsers/rdl_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3133 2023-05-21 16:44:23.000000 cheap_pie-1.0.0/src/cheap_pie/parsers/svd_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3209 2023-05-21 16:45:01.000000 cheap_pie-1.0.0/src/cheap_pie/parsers/svd_parse_repo.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2506 2023-05-21 13:40:46.000000 cheap_pie-1.0.0/src/cheap_pie/parsers/xml_xslt.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-22 21:34:10.584553 cheap_pie-1.0.0/src/cheap_pie/tools/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       92 2023-05-21 15:55:01.000000 cheap_pie-1.0.0/src/cheap_pie/tools/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4418 2023-05-22 21:15:24.000000 cheap_pie-1.0.0/src/cheap_pie/tools/hal2doc.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2712 2023-05-22 19:30:55.000000 cheap_pie-1.0.0/src/cheap_pie/tools/rdl2any.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2651 2023-05-22 21:20:52.000000 cheap_pie-1.0.0/src/cheap_pie/tools/search.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-22 21:34:10.597032 cheap_pie-1.0.0/src/cheap_pie/transport/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      219 2023-05-22 21:18:16.000000 cheap_pie-1.0.0/src/cheap_pie/transport/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2367 2023-05-21 15:28:36.000000 cheap_pie-1.0.0/src/cheap_pie/transport/cp_dummy_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2298 2023-05-21 15:27:18.000000 cheap_pie-1.0.0/src/cheap_pie/transport/cp_esptool_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1776 2023-05-21 16:01:42.000000 cheap_pie-1.0.0/src/cheap_pie/transport/cp_jlink_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1777 2023-05-21 16:11:06.000000 cheap_pie-1.0.0/src/cheap_pie/transport/cp_pyocd_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     5206 2023-05-22 20:54:15.000000 cheap_pie-1.0.0/src/cheap_pie/transport/cp_pyverilator_transport.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-22 21:34:10.542069 cheap_pie-1.0.0/src/cheap_pie.egg-info/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     8432 2023-05-22 21:34:10.000000 cheap_pie-1.0.0/src/cheap_pie.egg-info/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1317 2023-05-22 21:34:10.000000 cheap_pie-1.0.0/src/cheap_pie.egg-info/SOURCES.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-05-22 21:34:10.000000 cheap_pie-1.0.0/src/cheap_pie.egg-info/dependency_links.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      125 2023-05-22 21:34:10.000000 cheap_pie-1.0.0/src/cheap_pie.egg-info/requires.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       10 2023-05-22 21:34:10.000000 cheap_pie-1.0.0/src/cheap_pie.egg-info/top_level.txt
```

### Comparing `cheap_pie-0.9.20/LICENSE` & `cheap_pie-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.20/README.md` & `cheap_pie-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,17 @@
 https://github.com/oddball/ipxact2systemverilog
 
 # Others	
 In conjunction with pyVISA (https://pyvisa.readthedocs.io/en/master/), used for 
 instument control, it provides a simple and fully python-contained environment
 for silicon validation.
 
+Graphical Render of bitfield structures
+https://github.com/wavedrom/bitfield
+
 C++ register/bitfields access (including generation from svd)
 https://github.com/thanks4opensource/regbits
 
 STM C++ regbits implementation
 https://github.com/thanks4opensource/regbits_stm
 
 a barebone embedded library generator
```

### Comparing `cheap_pie-0.9.20/setup.py` & `cheap_pie-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,34 +2,39 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setup(
     name='cheap_pie',
-    version='0.9.20',
+    version='1.0.0',
     license='Apache 2.0',
     author="Marco Merlin",
     author_email='marcomerli@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description="A python tool for silicon validation.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     url='https://github.com/bat52/cheap_pie',
     keywords='python silicon validation',
     install_requires=[
           'untangle',
           'hickle',
           # parsers
           'cmsis-svd',
           'ipyxact',
           'python-docx',
+          'wavedrom',
+          'wavedrom-ascii',
           'pyverilator',
           'peakrdl-ipxact',
           'peakrdl-uvm',
           'peakrdl-verilog',
+          # 'lxml', # for xlst ipxact conversions
           # transport layers
           #'pylink-square',
           #'pyocd',
           #'esptool',
           #'packaging' # for verilator version check
       ],
 )
```

### Comparing `cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cbitfield.py` & `cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cbitfield.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Autogenerated with SMOP
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
 from ast import literal_eval
 
-class cp_bitfield():
+class CpBitfield():  # pylint: disable=R0902
     """A bitfield register class """
     # field width
     width = 1
 
     # LSB
     lsb = 1
 
@@ -33,21 +33,21 @@
     # field name
     fieldname = ""
 
     # host interface handler
     hif = None
 
     # read/write
-    rw  = "rw"
+    read_write = "rw"
 
     # reset value
     reset = 0
 
-    def __init__(self, regfield="",regaddr=0, regname="", width="1",
-                 bit_offset="0", comments="",hif=None, rw = "rw", reset=0):
+    def __init__(self, regfield="",regaddr=0, regname="", width="1", # pylint: disable=R0913
+                 bit_offset="0", comments="", hif=None, read_write = "rw", reset=0):
 
         if isinstance(width,str):
             width= literal_eval(width)
         # field width
         self.width = int( width )
 
         if isinstance(bit_offset,str):
@@ -67,88 +67,87 @@
         bstr = "0b" + ("1" * self.width) + ("0" * self.lsb)
         self.mask=literal_eval( bstr )
         self.comments = comments
         self.addr = int( regaddr )
         self.regname = regname
         self.fieldname = regfield
         self.hif = hif
-        self.rw = rw
+
+        assert isinstance(read_write,str)
+        assert read_write.lower() in ['r','w','rw']
+        self.read_write = read_write
+
         self.reset = reset
 
-    def _strval(self,fieldval,width=25):
+    def __str__(self,fieldval=None,width=25):
+        """ returns value string of a bitfield from a register value
+        input : regval value of the full register either in decimal or
+        hexadecimal """
         #
-        bitstr = self.fieldname  + ' [' + str(self.width) + '] = ' + hex(fieldval)
+        bitstr = self.fieldname  + ' [' + str(self.width) + ']'
+        if not fieldval is None:
+            bitstr += ' = ' + hex(fieldval)
 
         if self.width > 1:
             msb = str( self.lsb + self.width - 1)
             regstr = self.regname + '[' + msb + ':' + str(self.lsb) + ']'
         else:
             regstr = self.regname + '[' + str(self.lsb) + ']'
 
-        fmtstr = '%%%ds @ %%%ds' % (width,width)
+        fmtstr = '%%%ds @ %%%ds' % (width,width) # pylint: disable=C0209
         return fmtstr % (regstr,bitstr)
 
-    def __repr__(self,regval=None):
-        """ displays value of a bitfield from a register value
-        input : regval value of the full register either in decimal or
-        hexadecimal """
+    def __repr__(self, regval = None):
+        """
+        displays position of a bitfield in a register
+        """
         #
         if regval is None:
-            if self.hif is None:
-                regval=0
-            else:
-                regval=self.hif.hifread(self.addr)
-        #
-        # compute field value from register value
-        if isinstance(regval, str):
-            regval=literal_eval(regval)
-        fieldval = (regval & self.mask ) >> (self.lsb)
-
-        outstr= self._strval(fieldval)
-        # print(outstr)
-        return outstr
+            fieldval = None
+        else:
+            fieldval = self.getbit(regval=regval)
+        return self.__str__(fieldval=fieldval)
 
     def display(self,regval=None):
         """
         Display the bitfield
         """
-        print(self)
-        return self
+        fieldval = self.getbit(regval=regval)
+        fieldstr = self.__str__(fieldval=fieldval) # pylint: disable=C2801
+        print(fieldstr)
 
-    def getbit(self,regval=None,echo=False,as_signed=False,*args,**kwargs):
+    def getbit(self,regval=None,echo=False,as_signed=False): # ,*args,**kwargs):
         """ function display(self,regval=None,echo=False,as_signed=False)
         # displays value of a bitfield from a register value
         # input : regval value of the full register either in decimal or
         # hexadecimal"""
         #
         if regval is None:
             if self.hif is None:
                 regval=0
             else:
-                regval=self.hif.hifread(self.addr)
+                regval=self.hif.hifread(self.addr) # ,*args,**kwargs)
 
         # compute field value from register value
         if isinstance(regval, str):
             regval=literal_eval(regval)
         fieldval = (regval & self.mask ) >> (self.lsb)
 
         # get bitfield as signed value
         if as_signed:
             fieldsign = -(fieldval & (1 << (self.width - 1)))
             fieldmod = (fieldval & (self.mask>>(self.lsb+1)))
             fieldval = fieldsign + fieldmod
 
-        # fieldval=self.value(regval)
         if echo:
-            outstr= self._strval(fieldval)
-            print(outstr)
+            self.display(regval)
         #
         return fieldval
 
-    def setbit(self,fieldval=0,echo=False, writeback=True, regval=None,*args,**kwargs):
+    def setbit(self,fieldval=0,echo=False, writeback=True, regval=None,*args,**kwargs): # pylint: disable=W1113
         """ function display(self,regval)
         # displays value of a bitfield from a register value
         # input : regval value of the full register either in decimal or
         # hexadecimal """
 
         ## read input register value ###################################################
         if not (self.hif is None) and regval is None:
@@ -178,84 +177,89 @@
             raise ValueError(f'Bitifield value f{fieldval} out of range!')
         #
         ## write back new register value ###############################################
         if writeback:
             self.hif.hifwrite(self.addr,outregval,*args,**kwargs)
         #
         if echo:
-            outstr=self._strval(fieldval)
-            print(outstr)
+            self.display(regval=regval)
         #
         return outregval
 
     #@function
     def help(self):
         """ function ret = help(self)
         # displays register comments """
         print(self.comments)
 
-    #@function
-    def value(self,regval=0):
-        """ function ret = value(self,regval)
-        # Returns value of a bitfield from a register value
-        # input : regval value of the full register either in decimal or
-        # hexadecimal """
-        #
-        if isinstance(regval, str):
-            regval=literal_eval(regval)
-        #
-        ret = (regval & self.mask ) >> (self.lsb)
-        return ret
-
     def __index__(self):
         return int(self.getbit())
 
 def test_cp_bitfield():
     """
     Test function for cp_bitfield class
     """
-    import sys
-    import os.path
+    import sys # pylint: disable=C0415
+    import os.path # pylint: disable=C0415
     sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
-    from transport.cp_dummy_transport import cp_dummy
+    from transport.cp_dummy_transport import CpDummyTransport # pylint: disable=C0415, disable=E0401
 
-    field = cp_bitfield(
+    field = CpBitfield(
         regfield = 'fname',
         regaddr = 10,
         regname = 'rname',
         width = '2',
         bit_offset = '2',
         comments = 'comment',
-        hif = cp_dummy()
+        hif = CpDummyTransport()
     )
 
+    print('# setbit, getbit')
     val = 3
     field.setbit(val)
     assert field.getbit() == val
-    field.value()
-    field.display()
-    field.display(2)
+
+    print('# display')
+    field.display(4)
+
+    print('# str')
+    print(str(field))
+
+    print('# print')
+    print(field)
+
+    print('# help')
     field.help()
 
-    # signed assignement
+    print('# signed assignement')
     negval = -1
     field.setbit(negval)
     retval = field.getbit(as_signed=True)
     assert negval==retval
 
-    # decimal representation
+    print('# decimal representation')
     print(hex(field))
 
-    # options
+    print('# setbit with echo')
     field.setbit(val,echo=True)
-    field.setbit(val,writeback=False)
-    rv = field.setbit(1,regval=1)
-    assert rv==5
 
-    # test assertion
+    print('# setbit without writeback')
+    val=1
+    field.setbit(val)
+    assert field.getbit() == val
+    newval = 3
+    field.setbit(newval,writeback=False)
+    assert field.getbit() == val
+
+    print('# setbit with regval')
+    val=3
+    regretval = field.setbit(val)
+    assert field.setbit(val,regval=regretval) == regretval
+
+    print('# test assertion')
     try:
         field.setbit(7)
         assert False, 'Assertion was not raised!!!'
     except ValueError as error:
         print(f'Assertion raised correctly: <{error}>')
 
 if __name__ == '__main__':
```

### Comparing `cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cheap_pie.py` & `cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cheap_pie_main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 #!/usr/bin/python3
 """
 This file is part of cheap_pie, a python tool for chip validation
  author: Marco Merlin
  email: marcomerli@gmail.com
 """
 
+if __name__ == '__main__':
+    # needed if cheap_pie not installeds
+    import os
+    import sys
+    sys.path.append( os.path.join(os.path.dirname(__file__), '../..') )
+
+from cheap_pie.parsers.cp_parsers_wrapper import cp_parsers_wrapper # pylint: disable=C0413,E0401
+from cheap_pie.cheap_pie_core.cp_banner import cp_banner            # pylint: disable=C0413,E0401
+from cheap_pie.cheap_pie_core.cp_cli import cp_cli                  # pylint: disable=C0413,E0401
+from cheap_pie.transport.cp_dummy_transport import CpDummyTransport # pylint: disable=C0413,E0401
+
 # Ipython autoreload
 # %load_ext autoreload
 # %autoreload 2
 # %reset
 # %run cheap_pie
 
-import os
-import sys
-sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
-
-from parsers.cp_parsers_wrapper import cp_parsers_wrapper
-from cheap_pie_core.cp_banner import cp_banner
-from cheap_pie_core.cp_cli import cp_cli
-from cheap_pie_core.cp_hal import cp_hal
-
-def main(argv=[]):
+def cp_main(argv=[]): # pylint: disable=W0102
     """
     Main cheap_pie function
     """
     ## banner #######################################################################
     cp_banner()
     #
     ## input parameters ###########################################################
     print('Parsing input arguments...')
-    p = cp_cli(argv)
+    prms = cp_cli(argv)
 
     ## transport hif interface %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     print('Initialising Host Interface...')
 
-    # init jlink transport
-    if p.transport == 'jlink': # disable jlink for testing
-        from transport.cp_jlink_transport import cp_jlink
-        hif = cp_jlink(device = p.device )
-    elif p.transport == 'dummy':
-        from transport.cp_dummy_transport import cp_dummy
-        hif = cp_dummy()
-    elif p.transport == 'ocd':
-        from transport.cp_pyocd_transport import cp_pyocd
-        hif = cp_pyocd(device = p.device )
-    elif p.transport == 'esptool':
-        from transport.cp_esptool_transport import cp_esptool
-        hif = cp_esptool(port = p.port )
-    elif p.transport == 'verilator':
-        from transport.cp_pyverilator_transport import cp_pyverilator_transport
-        hif = cp_pyverilator_transport( p.top_verilog )
+    # init jlink transport: importing under if case allows not installing all transport libraries
+    if prms.transport == 'dummy':
+        hif = CpDummyTransport()
+    elif prms.transport == 'jlink': # disable jlink for testing
+        from cheap_pie.transport.cp_jlink_transport import CpJlinkTransport # pylint: disable=C0413,C0415,E0401
+        hif = CpJlinkTransport(device = prms.device )
+    elif prms.transport == 'ocd':
+        from cheap_pie.transport.cp_pyocd_transport import CpPyocdTransport # pylint: disable=C0413,C0415,E0401
+        hif = CpPyocdTransport(device = prms.device )
+    elif prms.transport == 'esptool':
+        from cheap_pie.transport.cp_esptool_transport import CpEsptoolTransport # pylint: disable=C0413,C0415,E0401
+        hif = CpEsptoolTransport(port = prms.port )
+    elif prms.transport == 'verilator':
+        from cheap_pie.transport.cp_pyverilator_transport import CpPyverilatorTransport # pylint: disable=C0413,C0415,E0401
+        hif = CpPyverilatorTransport( prms.top_verilog )
     else:
         hif=None
-        assert False, f'Invalid transport: {p.transport}'
+        assert False, f'Invalid transport: {prms.transport}'
 
     ## init chip ##################################################################
     print('Initialising Hardware Abstraction Layer...')
-    hal = cp_hal( cp_parsers_wrapper( p, hif=hif ) )
+    lhal = cp_parsers_wrapper( prms, hif=hif )
 
     ## welcome ####################################################################
     print('Cheap Pie is ready! Type hal.<TAB> to start browsing...')
 
-    return hal
+    return lhal
 
 if __name__ == '__main__':
-    hal = main(sys.argv[1:])
+    hal = cp_main(sys.argv[1:])
```

### Comparing `cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cp_banner.py` & `cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_banner.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,37 +9,37 @@
 def cp_banner():
     """
     Just a nice looking banner for cheap_pie
     """
     logo = (
     "        _..._                                                                     ",
     "    .-'_..._''.                                                                   ",
-    "  .' .'      '.\  .              __.....__               _________   _...._       ",
-    " / .'           .'|          .-''         '.             \        |.'      '-.    ",
-    ". '            <  |         /     .-''`'-.  `.            \        .'```'.    '.  ",
-    "| |             | |        /     /________\   \    __      \      |       \     \ ",
+    "  .' .'      '.\  .              __.....__               _________   _...._       ", # pylint: disable=W1401
+    " / .'           .'|          .-''         '.             \        |.'      '-.    ", # pylint: disable=W1401
+    ". '            <  |         /     .-''`'-.  `.            \        .'```'.    '.  ", # pylint: disable=W1401
+    "| |             | |        /     /________\   \    __      \      |       \     \ ", # pylint: disable=W1401
     "| |             | | .'''-. |                  | .:--.'.     |     |        |    | ",
-    ". '             | |/.'''. \|    .-------------'/ |   \ |    |      \      /    .  ",
-    " \ '.          .|  /    | | \    '-.____...---.`` __ | |    |     |\`'-.-'   .'   ",
+    ". '             | |/.'''. \|    .-------------'/ |   \ |    |      \      /    .  ", # pylint: disable=W1401
+    " \ '.          .|  /    | | \    '-.____...---.`` __ | |    |     |\`'-.-'   .'   ", # pylint: disable=W1401
     "  '. `._____.-'/| |     | |  `.             .'  .'.''| |    |     | '-....-'`     ",
     "    `-.______ / | |     | |    `''-...... -'   / /   | |_  .'     '.              ",
-    "             `  | '.    | '.                   \ \._,\ '/'-----------'            ",
+    "             `  | '.    | '.                   \ \._,\ '/'-----------'            ", # pylint: disable=W1401
     "                '---'   '---'                   `--'  ``                          ",
     "                            ___                                                   ",
-    "                         .'/   \                                                  ",
-    "_________   _...._      / /     \      __.....__                                  ",
-    "\        |.'      '-.   | |     |  .-''         '.                                ",
-    " \        .'```'.    '. | |     | /     .-''`'-.  `.                              ",
-    "  \      |       \     \|/`.   .'/     /________\   \                             ",
+    "                         .'/   \                                                  ", # pylint: disable=W1401
+    "_________   _...._      / /     \      __.....__                                  ", # pylint: disable=W1401
+    "\        |.'      '-.   | |     |  .-''         '.                                ", # pylint: disable=W1401
+    " \        .'```'.    '. | |     | /     .-''`'-.  `.                              ", # pylint: disable=W1401
+    "  \      |       \     \|/`.   .'/     /________\   \                             ", # pylint: disable=W1401
     "   |     |        |    | `.|   | |                  |                             ",
-    "   |      \      /    .   ||___| \    .-------------'                             ",
-    "   |     |\`'-.-'   .'    |/___/  \    '-.____...---.                             ",
+    "   |      \      /    .   ||___| \    .-------------'                             ", # pylint: disable=W1401
+    "   |     |\`'-.-'   .'    |/___/  \    '-.____...---.                             ", # pylint: disable=W1401
     "   |     | '-....-'`      .'.--.   `.             .'                              ",
     "  .'     '.              | |    |    `''-...... -'                                ",
-    "'-----------'            \_\    /                                                 ", 
+    "'-----------'            \_\    /                                                 ", # pylint: disable=W1401
     "                          `''--'                                                  ",
     "A python tool for chip validation by Marco Merlin\n"
     )
     for line in logo:
         print(line)
 
 def test_banner():
```

### Comparing `cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cp_cli.py` & `cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,27 +2,47 @@
 """
 Cheap Pie Command Line Interface
 """
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
-import argparse
+import os
 import sys
+import pathlib
+import argparse
+
+def cp_root_dir():
+    """ Returns the full path of Cheap Pie root directory """
+    return pathlib.Path(__file__).parent.parent.absolute()
+
+def cp_devices_dir():
+    """ Returns the full path of ad filename in Cheap Pie devices directory """
+    return os.path.join(
+        cp_root_dir(),
+        'devices')
+
+def cp_devices_fname(fname):
+    """ Returns the full path of ad filename in Cheap Pie devices directory """
+    return os.path.join(
+            cp_devices_dir(), fname
+            )
 
-def cp_cli(args=[]):
+def cp_cli(args=[]): # pylint: disable=W0102
     """
     Cheap Pie Command Line Interface
     """
     parser = argparse.ArgumentParser(description='Cheap Pie Configuration')
     # register format options
     parser.add_argument("-rf", "--regfname", help="register description file name",
                         action='store', type = str, default="QN908XC.svd")
     parser.add_argument("-dd", "--devicedir", help="register description files folder",
-                        action='store', type = str, default="./devices")
+                        action='store', type = str,
+                        default=cp_devices_dir()
+                        )
     parser.add_argument("-fmt","--format", help="device description format",
                         action='store', type = str, default="cmsis-svd",
                         choices=["svd","cmsis-svd","ipxact","ipyxact","rdl"])
     parser.add_argument("-ve", "--vendor",
                         help="device vendor. if specified parses svd file from github repository.",
                         action='store', type = str, default=None)
     # transport options
```

### Comparing `cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cp_hal.py` & `cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_hal.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,29 +6,18 @@
 # -*- coding: utf-8 -*-
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
 import hickle as hkl
 
-try:
-    # cheap_pie installed with pip 
-    from cheap_pie.transport.cp_dummy_transport import cp_dummy
-    import cheap_pie.tools.search
-    from cheap_pie.tools.hal2doc import hal2doc
-
-except:
-    import sys
-    import os.path
-    sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
-    from transport.cp_dummy_transport import cp_dummy
-    import tools.search
-    from tools.hal2doc import hal2doc
+import cheap_pie.tools.search # pylint: disable=W0611
+from   cheap_pie.tools.hal2doc import hal2doc
 
-class cp_hal:
+class CpHal():
     """
     Cheap Pie Hardware Abstraction Layer
     """
     regs = []
     hif = None
 
     def __init__(self,regs):
@@ -46,44 +35,47 @@
 
     def __next__(self):
         return self.regs.next()
 
     def __getitem__(self, idx):
         if isinstance(idx,int):
             return self.regs[idx]
-        elif isinstance(idx,str):
+        if isinstance(idx,str):
             return self.regs._asdict()[idx]
         assert False,'Unsupported indexing!'
 
     def __setitem__(self, idx, value):
         if isinstance(idx,int):
             return self.regs[idx].setreg(value)
-        elif isinstance(idx,str):
+        if isinstance(idx,str):
             return self.regs._asdict()[idx].setreg(value)
         assert False, 'Unsupported indexing!'
 
+    def __repr__(self):
+        return 'CP_HAL: %d registers' % len(self.regs) # pylint: disable=C0209
+
 ## search methods ###########################################################
 
     def search_bitfield(self,field,case_sensitive=False):
         """
         Search bitfields which name contains a specified string
         """
-        return tools.search.bitfield(self.regs,field,case_sensitive=case_sensitive)
+        return cheap_pie.tools.search.bitfield(self.regs,field,case_sensitive=case_sensitive) # pylint: disable=E0601
 
     def search_register(self,reg,case_sensitive=False):
         """
         Search registers which name contains a specified string
         """
-        return tools.search.register(self.regs,reg,case_sensitive=case_sensitive)
+        return cheap_pie.tools.search.register(self.regs,reg,case_sensitive=case_sensitive)
 
     def search_address(self,address,mask='0xFFFFFFFF'):
         """
         Search register matching a specified address
         """
-        return tools.search.address(self.regs,address,mask=mask)
+        return cheap_pie.tools.search.address(self.regs,address,mask=mask)
 
     def to_docx(self,*args):
         """
         Generate a .docx document describing an Hardware Abstraction Layer
         """
         hal2doc(self.regs,*args)
 
@@ -108,116 +100,174 @@
         regs_dict = self.regs2dict()
         hkl.dump(regs_dict, fname, compression='gzip')
 
     def dump_diff(self,f1name='dump.hkl',f2name='dump2.hkl',width = 60):
         """
         Perform a diff on two dumped .hkl files.
         """
-        fmtstr = '%%%ds |%%%ds' % (width,width)
+        fmtstr = '%%%ds |%%%ds' % (width,width) # pylint: disable=C0209
 
         field1 = hkl.load(f1name)
         field2 = hkl.load(f2name)
 
         # create a header with filenames
         outstrlist = []
         for reg,val in field1.items():
             if not field2[reg] == val:
-                f1regstr = self[reg].__repr__(val).split('\n')
-                f2regstr = self[reg].__repr__(field2[reg]).split('\n')
+                f1regstr = self[reg].__repr__(val        ).split('\n') # pylint: disable=C2801
+                f2regstr = self[reg].__repr__(field2[reg]).split('\n') # pylint: disable=C2801
 
-                for idx in range(len(f1regstr)):
+                for idx in range(len(f1regstr)): # pylint: disable=C0200
                     if not f1regstr[idx]==f2regstr[idx]:
-                        linestr = fmtstr % (f1regstr[idx],f2regstr[idx])
-                        outstrlist.append(linestr)
+                        outstrlist.append(fmtstr % (f1regstr[idx],f2regstr[idx]))
 
         # print output
         if len(outstrlist) > 0:
             headerstr = fmtstr % (f1name,f2name)
             outstrlist.insert(0,headerstr)
             for line in outstrlist:
                 print(line)
         else:
             print('No differences found!!!')
 
-def test_to_docx():
+        return outstrlist
+
+def test_cp_hal_to_docx():
     """
     Test Function for Cheap Pie HAL to .docx
     """
-    from parsers.cp_parsers_wrapper import cp_parsers_wrapper
-    from cheap_pie_core.cp_cli import cp_cli
+    from parsers.cp_parsers_wrapper import cp_parsers_wrapper  # pylint: disable=C0415,C0413,E0401
+    from cheap_pie_core.cp_cli import cp_cli                   # pylint: disable=C0415,C0413,E0401
 
     prms = cp_cli(['-t','dummy','-rf','my_subblock.xml','-fmt','ipxact'])
-    hal = cp_hal(cp_parsers_wrapper(prms))
-
+    hal = cp_parsers_wrapper(prms)
     hal.to_docx()
 
-def test_cp_hal():
+def test_cp_hal(): # pylint: disable=R0914,R0915
     """
     Test Function for Cheap Pie Hardware Abstraction Layer
     """
-    from parsers.cp_parsers_wrapper import cp_parsers_wrapper
-    from cheap_pie_core.cp_cli import cp_cli
-    from ast import literal_eval
+    from ast import literal_eval                                        # pylint: disable=C0415
+    from parsers.cp_parsers_wrapper import cp_parsers_wrapper # pylint: disable=C0415,E0401
+    from transport.cp_dummy_transport import CpDummyTransport # pylint: disable=C0415,E0401
+    from cheap_pie_core.cp_cli import cp_cli                  # pylint: disable=C0415,E0401
 
+    print('# hal initialize')
     prms = cp_cli(['-t','dummy'])
-    hal = cp_hal(cp_parsers_wrapper(prms,cp_dummy()))
+    hal = cp_parsers_wrapper(prms,hif=CpDummyTransport())
 
-    print('Test register methods...')
-    # hex assignement
+    print('# hal test register methods...')
+    print('# hal hex assignement')
     inval = "0xFFFFFFFF"
     hal.regs.ADC_ANA_CTRL.setreg(inval)
     retval = hex(hal.regs.ADC_ANA_CTRL.getreg())
-    # print('%s' % retval.encode('hex'))
     print(retval)
     assert literal_eval(inval) == literal_eval(retval)
 
-    # decimal assignement
+    print('# hal decimal assignement')
     inval = 2
     hal.regs.ADC_ANA_CTRL.setreg(inval)
     retval = hal.regs.ADC_ANA_CTRL.getreg()
     assert inval == retval
 
+    print('# hal reg representation')
+    hal.regs.ADC_ANA_CTRL # pylint: disable=W0104
+
+    print('# hal reg display')
     hal.regs.ADC_ANA_CTRL.display()
-    print('Test bitfield methods...')
 
+    print('# hal reg print')
+    print(hal.regs.ADC_ANA_CTRL)
+
+    print('# hal reg str')
+    print(str(hal.regs.ADC_ANA_CTRL))
+
+    print('# hal test bitfield methods...')
+    print('# hal bitfield display')
     hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.display()
+    print('# hal bitfield display with value')
     hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.display(2)
+    print('# hal bitfield setbit')
     hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.setbit(inval)
     retval = hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.getbit()
     assert inval == retval
 
-    # subscriptable interface
-    hal[0]
-    hal[0][0]
-    hal['ADC_ANA_CTRL']
-
-    # test assignement
-    hal['ADC_ANA_CTRL'] = 1
-    hal['ADC_ANA_CTRL']['ADC_BM'] = 2
-    # dict-based assignement in single register write
-    hal['ADC_ANA_CTRL'] = {'DITHER_EN': 1, 'CHOP_EN': 1, 'INV_CLK': 1}
-
-    # test search
-    reg = hal.search_register('ADC_ANA_CTRL')
-    assert len(reg)>0
-    field = hal.search_bitfield('ADC_BM')
-    assert len(field)>0
-    reg = hal.search_address('0x4000702c')
-    assert len(reg)>0
-    reg = hal.search_address('0xF000702c',mask='0x0FFFFFFF')
-    assert len(reg)>0
-    reg = hal.search_address('0xF000702c')
-    assert reg is None
-
-    # test conversion to doc
-    test_to_docx()
+    print('# hal subscriptable interface...')
+    print('# hal[0]')
+    print(hal[0])
+
+    print('# hal[0][0]')
+    print(hal[0][0])
+
+    print("# hal['ADC_ANA_CTRL']")
+    print(hal['ADC_ANA_CTRL'])
+
+    print('# hal dict-based reg assignement')
+    regval = 1
+    hal['ADC_ANA_CTRL'] = regval
+    assert hal.regs.ADC_ANA_CTRL.getreg() == regval
+
+    print('# hal dict-based bitfield assignement')
+    fieldval = 2
+    hal['ADC_ANA_CTRL']['ADC_BM'] = fieldval
+    assert hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.getbit() == fieldval
+
+    print('# hal dict-based assignement in single register write')
+    dither = 1
+    chop = 1
+    inv = 1
+    hal['ADC_ANA_CTRL'] = {'DITHER_EN': dither, 'CHOP_EN': chop, 'INV_CLK': inv}
+    assert hal.regs.ADC_ANA_CTRL.bitfields.DITHER_EN.getbit() == dither
+    assert hal.regs.ADC_ANA_CTRL.bitfields.CHOP_EN.getbit() == chop
+    assert hal.regs.ADC_ANA_CTRL.bitfields.INV_CLK.getbit() == inv
+
+    print('# hal search_register')
+    searchreg = 'ADC_ANA_CTRL'
+    reglist = hal.search_register(searchreg)
+    reg = reglist[0]
+    print(reg)
+    assert str(reg) == searchreg
+
+    print('# hal search_bitfield')
+    searchfield = 'ADC_BM'
+    fieldlist = hal.search_bitfield(searchfield)
+    print(fieldlist)
+    field = fieldlist[0]
+    print(field)
+    assert searchfield in field
+
+    print('# hal search_address')
+    searchaddr = '0x4000702c'
+    reg = hal.search_address(searchaddr)
+    print(f'# Register {reg}')
+    addr = hex(hal[reg].addr)
+    print(f'# Address: {addr}')
+    assert addr == searchaddr
+
+    print('# hal search_address with mask')
+    searchaddr = '0xF000702c'
+    searchmask = '0x0FFFFFFF'
+    reg = hal.search_address(searchaddr,mask=searchmask)
+    print(f'# Register {reg}')
+    addr = hex(hal[reg].addr)
+    print(f'# Address: {addr}')
+    assert (literal_eval(addr)       & literal_eval(searchmask) ==
+            literal_eval(searchaddr) & literal_eval(searchmask) )
+    reg = hal.search_address(searchaddr)
+    assert reg==''
 
-    # test dump
+    print('# hal dump')
     dump1 = 'dump1.hkl'
     dump2 = 'dump2.hkl'
     hal.dump(dump1)
     hal['ADC_ANA_CTRL']['ADC_BM'] = 3
     hal.dump(dump2)
-    hal.dump_diff(dump1,dump2)
+    diff = hal.dump_diff(dump1,dump2)
+    print(diff)
+    assert len(diff) == 2
+
+    print('# hal regs2dict')
+    mydict = hal.regs2dict()
+    assert isinstance(mydict,dict)
 
 if __name__ == '__main__':
     test_cp_hal()
```

### Comparing `cheap_pie-0.9.20/src/cheap_pie/parsers/svd_parse_repo.py` & `cheap_pie-1.0.0/src/cheap_pie/parsers/svd_parse.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python3
-""" Cheap Pie parser module for .svd files using SVDParser module """
+""" Cheap Pie module for native .svd files parser """
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
 # parser build for CMSIS-SVD xml file format
 # https://www.keil.com/pack/doc/CMSIS/SVD/html/index.html
 #
@@ -11,96 +11,76 @@
 #
 # import untangle
 # hal = untangle.parse('QN908XC.xml')
 # from cbitfield import cp_bitfield
 # from cp_register import cp_register
 # ADC_ANA_CTRL = cp_register("ADC_ANA_CTRL","0x4000702C",
 #                            "ADC core and reference setting regsiter" , hif )
-# ADC_BM = cp_bitfield("ADC_BM","0x4000702C",
-#                      "ADC_ANA_CTRL",3,0, "ADC bias current selection." ,hif)
+# ADC_BM = cp_bitfield("ADC_BM","0x4000702C","ADC_ANA_CTRL",3,0, "ADC bias current selection." ,hif)
 
 from ast import literal_eval
-from collections import namedtuple
-from cmsis_svd.parser import SVDParser
+import untangle # for parsing xml
 
-import sys
-import os.path
-sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
-
-from cheap_pie_core.cbitfield   import cp_bitfield
-from cheap_pie_core.cp_register import cp_register
-from parsers.name_subs import name_subs
+from cheap_pie.cheap_pie_core.cp_builder import CpHalBuilder # pylint: disable=C0413,E0401
+from cheap_pie.cheap_pie_core.cp_cli import cp_devices_fname
 
-def svd_parse(fname,vendor=None,hif=None, base_address_offset = "0x00000000"):
-    """ Cheap Pie parser function for .svd files using SVDParser module """    
+def svd_parse(fname,vendor=None,hif=None, base_address_offset = "0x00000000"): # pylint: disable=W0613
+    """ Cheap Pie native parser for .svd files """
     ## read input file ########################################################
-    if vendor is None:
-        svd = SVDParser.for_xml_file(fname)
-    else:
-        svd = SVDParser.for_packaged_svd(vendor,fname)
+    svd = untangle.parse(fname)
 
     ## loop over lines ########################################################
-    outdict = {}
+    cpb = CpHalBuilder(hif)
 
-    for periph in svd.get_device().peripherals:
+    for periph in svd.device.peripherals.peripheral: # pylint: disable=R1702
         # print(periph.name.cdata)
 
-        base_address=periph.base_address
+        base_addr_str=periph.baseAddress.cdata
+        base_address=literal_eval(base_addr_str)
 
         if hasattr(periph,'registers'):
-            for reg in periph.registers:
-                if hasattr( reg, 'name'):
-                    # close old register, before opening a new one
-                    if 'regname' in locals():
-                        struct_register.dictfield2struct()
-                        outdict[regname]=struct_register
-
+            for reg in periph.registers.register:
+                if hasattr( reg.name, 'cdata'):
                     # new register
-                    periph_name=periph.name
-                    rname=reg.name
-                    regname = name_subs(f'{periph_name}_{rname}')
-
-                    regaddr=reg.address_offset + base_address + literal_eval(base_address_offset)
-                    comments=reg.description
-                    # print(comments)
-                    struct_register=cp_register(regname,regaddr,comments,hif)
+                    addr_str=reg.addressOffset.cdata
+                    regaddr=(
+                        literal_eval(addr_str) +
+                        base_address +
+                        literal_eval(base_address_offset)
+                    )
+
+                    cpb.reg_open(
+                        regname=f'{periph.name.cdata}_{reg.name.cdata}',
+                        regaddr=regaddr,
+                        comments=reg.description.cdata,
+                        )
 
-                    # for field_idx in range(nfields):
                     if hasattr(reg,'fields'):
-                        for field in reg.fields :
-                            regfield=field.name
-
+                        for field in reg.fields.field:
                             if not field is None:
-                                # print regfield
-                                regfield=name_subs(regfield)
-
-                                width=field.bit_width
-                                bitoffset=field.bit_offset
-                                comments=field.description
-                                # print(comments)
-
                                 # Create new field class
-                                class_regfield=cp_bitfield(regfield,regaddr,regname,
-                                                           width,bitoffset,comments,hif)
-                                struct_register.addfield(class_regfield)
-
-            # create last register, if existing
-            if 'regname' in locals():
-                # outstruct=addreg2struct(outstruct,regname,struct_register)
-                struct_register.dictfield2struct()
-                outdict[regname]=struct_register
+                                cpb.newfield(
+                                    regfield=field.name.cdata,
+                                    width=field.bitWidth.cdata,
+                                    offset=field.bitOffset.cdata,
+                                    comments=field.description.cdata,
+                                    )
 
     # convert output dictionary into structure
-    return namedtuple("HAL", outdict.keys())(*outdict.values())
+    return cpb.out()
+
+def test_svd_parse(argv=[]): # pylint: disable=W0102
+    """ test function for .svd parser """
 
-def test_svd_parse_repo():
-    """ Test Function for .svd parser based of SVDParser module """
-    print('Testing QN9080 with repo parser...')
+    if len(argv) > 1:
+        fname=argv[1]
+    else:
+        fname = cp_devices_fname("QN908XC.svd")
 
-    from parsers.svd_parse_repo import svd_parse
-    svd_parse(fname="./devices/QN908XC.svd")
+    hal = svd_parse(fname)
+    assert len(hal) > 0
 
-    print('Testing K20 with repo parser...')
-    svd_parse(fname='MK20D7.svd',vendor='Freescale')
+    return hal
 
 if __name__ == '__main__':
-    test_svd_parse_repo()
+    import sys
+    print(svd_parse(sys.argv))
```

### Comparing `cheap_pie-0.9.20/src/cheap_pie/parsers/xml_xslt.py` & `cheap_pie-1.0.0/src/cheap_pie/parsers/xml_xslt.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,67 @@
 #!/usr/bin/python3
 
+""" Convert between different .xml formats using .xslt rules
+Examples of conversion between different IP-XACT versions
+"""
+
 import sys
-import lxml.etree as ET
 import argparse
 import os
+import difflib
 
-def xml_xslt_parse(args=[]):
+import lxml.etree as ET
+from cheap_pie.cheap_pie_core.cp_cli import cp_devices_fname, cp_root_dir
+
+def xml_xslt_parse(args=[]): # pylint: disable=W0102
+    """ Parsing function for xml converter """
     parser = argparse.ArgumentParser(description='Apply XSLT to .xml file')
-    # parser.add_argument("-in", "--input", help=".xml input", action='store', type = str, default="./devices/my_subblock.xml")
-    parser.add_argument("-in", "--input", help=".xml input", action='store', type = str, default="./devices/generic_example.xml")
-    # parser.add_argument("-xslt", "--xslt", help=".xslt file", action='store', type = str, default="ipxact2svd.xslt")
-    # parser.add_argument("-xslt", "--xslt", help=".xslt file", action='store', type = str, default="./parsers/rules/from1.0_to_1.1.xsl")
-    parser.add_argument("-xslt", "--xslt", help=".xslt file", action='store', type = str, default="./parsers/rules/from1685_2009_to_1685_2014.xsl")
-    parser.add_argument("-out", "--output", help=".xml output", action='store', type = str, default="output.xml")
+    parser.add_argument("-in", "--input", help=".xml input",
+                        action='store', type = str, default=cp_devices_fname("generic_example.xml"))
+    parser.add_argument("-xslt", "--xslt", help=".xslt file",
+                        action='store', type = str,
+                        default=os.path.join(
+                            cp_root_dir(),
+                            "parsers/ipxact_rules/from1685_2009_to_1685_2014.xsl"
+                            )
+                        )
+    parser.add_argument("-out", "--output", help=".xml output",
+                        action='store', type = str, default="output.xml")
     return parser.parse_args(args)
 
 def xml_xslt(xmlin, xslt, xmlout):
-    dom = ET.parse(xmlin)
-    xslt = ET.parse(xslt)
-    transform = ET.XSLT(xslt)
-    newdom = transform(dom)
-    infile = ET.tostring(newdom, pretty_print=True).decode('utf-8')
+    """ Convert between different .xml formats using .xslt rules """
+    dom       = ET.parse(xmlin) # pylint: disable=I1101
+    xslt      = ET.parse(xslt)  # pylint: disable=I1101
+    transform = ET.XSLT(xslt)   # pylint: disable=I1101
+    newdom    = transform(dom)
+    infile    = ET.tostring(newdom, pretty_print=True).decode('utf-8') # pylint: disable=I1101
     # print(infile)
     if os.path.isfile(xmlout):
         os.remove(xmlout)
-    outfile = open(xmlout, 'a')
-    outfile.write(infile)
+    with open(xmlout, 'a', encoding='utf-8') as outfile:
+        outfile.write(infile)
 
 def compare(fromfile,tofile):
-    with open(fromfile) as ff:
-        fromlines = ff.readlines()
-    with open(tofile) as tf:
-        tolines = tf.readlines()
-
-    import difflib
-    # diff = difflib.context_diff(fromlines,tolines,fromfile=fromfile,tofile=tofile)
+    """ Compare two text files """
+    with open(fromfile, encoding='utf-8') as ffh:
+        fromlines = ffh.readlines()
+    with open(tofile, encoding='utf-8') as tfh:
+        tolines = tfh.readlines()
     diff = difflib.unified_diff(fromlines,tolines,fromfile=fromfile,tofile=tofile)
-    sys.stdout.writelines(diff)
 
-def test_xml_xslt(args):
-    p = xml_xslt_parse(args)
-    xml_xslt(xmlin = p.input, xslt = p.xslt, xmlout = p.output)
+    difflines = []
+    for line in diff:
+        difflines.append(line)
+        # print(line)
+
+    assert len(difflines) > 0
+
+def test_xml_xslt(args=[]): # pylint: disable=W0102
+    """ Test convert between different .xml formats using .xslt rules """
+    prms = xml_xslt_parse(args)
+    xml_xslt(xmlin = prms.input, xslt = prms.xslt, xmlout = prms.output)
     # diff input output
-    compare(p.input,p.output)
+    compare(prms.input,prms.output)
 
 if __name__ == '__main__':
     test_xml_xslt(sys.argv[1:])
-    pass
```

### Comparing `cheap_pie-0.9.20/src/cheap_pie/tools/hal2doc.py` & `cheap_pie-1.0.0/src/cheap_pie/tools/hal2doc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,182 +1,132 @@
 #!/usr/bin/python3
 
+""" Cheap Pie Module to export register descriptio into .docx file """
+
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
 from docx import Document
 # from docx.enum.table import WD_TABLE_ALIGNMENT
-from operator import attrgetter
-# from cbitfield import cp_bitfield
-
-import sys
-import os.path
-sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
-
-from cheap_pie_core.cbitfield import cp_bitfield
-
-def reg_add_reserved_bitfields(fields,regwidth=32):
-    next_lsb = 0
-    outfields = []
-
-    if isinstance(fields,list):
-        if len(fields) > 0:
-            for idx in reversed(range(len(fields))):
-            # for idx in range(len(fields)):
-                field = fields[idx]
-                outfields.insert(0,field)
-                #outfields.append(field)
-
-                if next_lsb < field.lsb:
-                    # print("Add Reserved field!")
-                    newfield=cp_bitfield("Reserved",0,field.regname,field.lsb-next_lsb,next_lsb,"Reserved")
-                    outfields.insert(1,newfield)
-                    # outfields.append(newfield)
-
-                # print("LSB: %d, WIDTH: %d" % ( field.lsb, field.width ) )
-                next_lsb = field.lsb + field.width
-
-            # check if register is filled up to full width    
-            if next_lsb < regwidth:
-                newfield=cp_bitfield("Reserved",0,fields[0].regname,regwidth-next_lsb,next_lsb,"Reserved")
-                outfields.insert(0,newfield)
-                # outfields.append(newfield)
-
-    return outfields  
-
-def int2hexstr(n,width):
-    fmt = "%%0%dx" % width
-    # print fmt 
-    # string = "%0256x" % n
-    # return string
-    # string = "\"%0256x\" % n"
-    string = "\"%s\" %% n " % fmt
-    # print string    
-    return eval(string)
+INCH2EMU = 914400
 
-def inch2emu():
-    return 914400
+def int2hexstr(num,width): # pylint: disable=W0613
+    """ Convert integer into hex string """
+    fmt = "%%0%dx" % width          # pylint: disable=C0209
+    # print fmt
+    string = "\"%s\" %% num " % fmt # pylint: disable=C0209
+    # print string
+    return eval(string) # pylint: disable=W0123
 
 def doc_create_header(template=None):
+    """ Create document header """
     if template is None:
         document = Document()
     else :
         document = Document(template)
 
     # document.add_heading('Document Title', 0)
     document.add_heading('Register Description', level=1)
     document.add_paragraph("")
 
     return document
 
-def doc_add_regtable(doc,reg,tablestyle=None,nbits_addr=32):
+def doc_add_regtable(doc,reg,tablestyle=None,nbits_addr=32): # pylint: disable=R0912
+    """ Add table description of a register to a document """
+    # header
     doc.add_heading(reg.regname, level=3)
-    
+
     # address
-    # doc.add_paragraph('Offset Address: 0x%d' % reg.addr)
-    doc.add_paragraph('Offset Address: 0x%s' % int2hexstr(reg.addr,nbits_addr/4))
-    # description
+    doc.add_paragraph('Offset Address: 0x%s' % int2hexstr(reg.addr,nbits_addr/4)) # pylint: disable=C0209
 
-    if isinstance(reg.comments,str):             
+    # description
+    if isinstance(reg.comments,str):
         doc.add_paragraph(reg.comments)
-    else:        
-        Warning("Non-string comments for reg: " + reg.regname)
+    else:
+        print("Warning: Non-string comments for reg: " + reg.regname)
 
     # bitfields table
     table = doc.add_table(rows=1, cols=5)
 
     if tablestyle is not None:
         table.style = tablestyle
-
     # table.alignment = WD_TABLE_ALIGNMENT.CENTER
-   
+
     # configure column width
     # https://stackoverflow.com/questions/43749177/python-docx-table-column-width
     # inch2emu = 914400
     cwidths = [         1.5,  0.5,    0.5,      1,            3]
 
     # create table header
     headers = ['Field name','rwu','Bit #','Reset','Description']
     hdr_cells = table.rows[0].cells
 
-    for idx in range(len(headers)):
+    for idx in range(len(headers)): # pylint: disable=C0200
         hdr_cells[idx].text  = headers[idx]
-        hdr_cells[idx].width = cwidths[idx]*inch2emu()
+        hdr_cells[idx].width = cwidths[idx]*INCH2EMU
         hdr_cells[idx].bold  = True
         # hdr_cells[idx].alignment=WD_ALIGN_PARAGRAPH.CENTER
 
     # add bitfields
-    for field in reversed(reg.bitfields):
+    for field in reversed(reg.get_ordered_bitfields()):
         row_cells = table.add_row().cells
         row_cells[0].text = field.fieldname
-        row_cells[0].width = cwidths[0]*inch2emu()
+        row_cells[0].width = cwidths[0]*INCH2EMU
 
-        if len(field.rw)/field.width > 1:
-            row_cells[1].text = str.lower(field.rw[0:2])
+        if len(field.read_write)/field.width > 1:
+            row_cells[1].text = str.lower(field.read_write[0:2])
         else:
-            row_cells[1].text = str.lower(field.rw)
-        row_cells[1].width = cwidths[1]*inch2emu()
+            row_cells[1].text = str.lower(field.read_write)
+        row_cells[1].width = cwidths[1]*INCH2EMU
 
         if field.width == 1:
-            row_cells[2].text = "%d" % ( field.lsb )
+            row_cells[2].text = "%d" % ( field.lsb ) # pylint: disable=C0209
         else:
-            row_cells[2].text = "%d:%d" % ( field.lsb + field.width -1, field.lsb)
-        row_cells[2].width = cwidths[2]*inch2emu()
+            row_cells[2].text = "%d:%d" % ( field.lsb + field.width -1, field.lsb) # pylint: disable=C0209
+        row_cells[2].width = cwidths[2]*INCH2EMU
 
         if isinstance(field.reset,str):
             row_cells[3].text = field.reset
         else:
-            resetstr = "%d\'%s" % (field.width, bin(field.reset)[1:])
+            resetstr = "%d\'%s" % (field.width, bin(field.reset)[1:]) # pylint: disable=C0209
             row_cells[3].text = resetstr
-        row_cells[3].width = cwidths[3]*inch2emu()
+        row_cells[3].width = cwidths[3]*INCH2EMU
 
-        if isinstance(reg.comments,str):             
+        if isinstance(reg.comments,str):
             row_cells[4].text = field.comments
-            row_cells[4].width = cwidths[4]*inch2emu()
+            row_cells[4].width = cwidths[4]*INCH2EMU
             # print(field.comments)
-        else:        
-            Warning("Non-string comments for field: %s in reg: %s" % (field.fieldname, reg.regname))
+        else:
+            print(f"Warning: Non-string comments for field: \
+                  {field.fieldname} in reg: {reg.regname}")
 
     doc.add_paragraph("")
 
 def hal2doc(hal,fname='hal.docx',template=None,tablestyle=None,nbits_addr=32):
-    
+    """  export register description to .docx file """
     # initialize doc
     doc = doc_create_header(template)
 
     # loop over registers
-    for reg in hal:                
-        # print(reg.regname)
-
-        # convert bitfields namedtuple into list
-        bitfields = list(reg.bitfields)
-
-        # sort by lsb
-        bitfields=sorted(bitfields,key=attrgetter('lsb'))
-        bitfields.reverse()
-
-        # add reserved bitfields
-        reg.bitfields = reg_add_reserved_bitfields(bitfields)
-
+    for reg in hal:
         # create register table
         doc_add_regtable(doc,reg,tablestyle,nbits_addr)
 
     # save document
     doc.save(fname)
 
 def test_hal2doc():
+    """ Test function for export tool from register description to .docx """
     print('Testing hal2doc...')
-    if False:
-        from parsers.svd_parse import svd_parse
-        # from parsers.svd_parse_repo import svd_parse
-        hal = svd_parse(fname="./devices/QN908XC.svd")
-    else:
-        from parsers.ipxact_parse import ipxact_parse
-        # from parsers.svd_parse_repo import svd_parse
-        hal = ipxact_parse(fname="./devices/my_subblock.xml")
+
+    from parsers.ipxact_parse import ipxact_parse      # pylint: disable=C0413,E0401,C0415
+    from cheap_pie_core.cp_cli import cp_devices_fname # pylint: disable=C0413,E0401,C0415
+
+    fname = cp_devices_fname("my_subblock.xml")
+    hal = ipxact_parse(fname=fname)
+
     # convert to .docx
     hal2doc(hal)
 
 if __name__ == '__main__':
     test_hal2doc()
-    pass
```

### Comparing `cheap_pie-0.9.20/src/cheap_pie/tools/search.py` & `cheap_pie-1.0.0/src/cheap_pie/tools/search.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,70 @@
 #!/usr/bin/python3
 
+""" Module including functions to search registers and bitifield in a
+Cheap Pie register description
+"""
+
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
 from ast import literal_eval
 
 def str_in_str(str1,str2,case_sensitive=True):
+    """ Check if a string is present into another string """
     if case_sensitive:
-        return (str1 in str2)
-    return (str1.upper() in str2.upper())
+        return str1 in str2
+    return str1.upper() in str2.upper()
 
 def register(hal,regname,case_sensitive=True):
-    retval = []    
+    """ Search a register by name """
+    retval = []
     for reg in hal: # loop over all registers
         if str_in_str(regname,reg.regname,case_sensitive):
             print( reg.regname )
             retval.append(reg.regname)
     return retval
 
-def bitfield(hal,bitfield,case_sensitive=True):
+def bitfield(hal,bitfield_name,case_sensitive=True):
+    """ Search a bitfield by name """
     retval = []
     for reg in hal: # loop over all registers
-        # print reg.regname        
+        # print reg.regname
         for field in reg.bitfields:
-            if str_in_str(bitfield,field.fieldname,case_sensitive):
-                print( reg.regname + " @ " + field.fieldname )
-                retval.append(field)
+            if str_in_str(bitfield_name,field.fieldname,case_sensitive):
+                fieldstr = str(field)
+                print(fieldstr)
+                retval.append(fieldstr)
     return retval
 
-def address(hal, address, mask='0xFFFFFFFF'):
+def address(hal, addr, mask='0xFFFFFFFF'):
+    """ Search a register by address """
     # convert address into integer, if needed
     if isinstance(mask,str):
         mask    = int( literal_eval(mask) )
-    if isinstance(address,str):
-        address = int( literal_eval(address) )
+    if isinstance(addr,str):
+        addr    = int( literal_eval(addr) )
 
-    retval = []    
     for reg in hal: # loop over all registers
         # print reg.regname
-        if (reg.addr & mask) == (address & mask):
+        if (reg.addr & mask) == (addr & mask):
             print( reg.regname + " : " + hex(reg.addr) )
             return reg.regname
 
+    return ''
+
 def test_search():
+    """ Test Search Module """
+    from parsers.svd_parse_repo import svd_parse_repo  # pylint: disable=E0401,C0415
+    from cheap_pie_core.cp_cli import cp_devices_fname # pylint: disable=E0401,C0415
     print('Testing search...')
-    from parsers.svd_parse_repo import svd_parse
-    hal = svd_parse(fname="./devices/QN908XC.svd", hif=None)
+
+    fname = cp_devices_fname("QN908XC.svd")
+    hal = svd_parse_repo(fname=fname, hif=None)
 
     print('## ADC registers:')
     ret = register(hal,'ADC')
     assert len(ret) > 0
 
     print('##  ADC_BM bitfields:')
     ret = bitfield(hal,'ADC_BM')
@@ -61,14 +75,14 @@
     assert len(ret) > 0
 
     print('## 0xF000702c register name:')
     ret = address(hal,'0xF000702c',mask='0x0FFFFFFF')
     assert len(ret) > 0
 
     ret = address(hal,'0xF000702c')
-    assert ret is None
+    assert ret==''
 
 if __name__ == '__main__':
     import sys
     import os.path
     sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
     test_search()
```

### Comparing `cheap_pie-0.9.20/src/cheap_pie/transport/cp_dummy_transport.py` & `cheap_pie-1.0.0/src/cheap_pie/transport/cp_dummy_transport.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,82 @@
 #!/usr/bin/python3
-#
+""" A dummy mockup transport module for Cheap Pie """
+
 # -*- coding: utf-8 -*-
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
 from ast import literal_eval
 
 def hex_bw(val,hex_digits_width = 8 ):
-    """ converts integer value into an hex string of fixed width """  
-    
-    assert( isinstance(val,int) )
+    """ converts integer value into an hex string of fixed width """
+    assert isinstance(val,int)
 
-    retstr = "{0:#0{1}x}".format(val,hex_digits_width+2)
+    retstr = "{0:#0{1}x}".format(val,hex_digits_width+2) # pylint: disable=C0209
 
     #  Explanation:
     # {   # Format identifier
     # 0:  # first parameter
     # #   # use "0x" prefix
     # 0   # fill with zeroes
     # {1} # to a length of n characters (including 0x), defined by the second parameter
     # x   # hexadecimal number, using lowercase letters for a-f
     # }   # End of format identifier
 
     # print(retstr)
 
-    return(retstr)
+    return retstr
+
+def numeric_input(val):
+    """ Numeric input that supports string evaluation with literal_eval """
+    if isinstance(val, int):
+        return val
+    if isinstance(val, str):
+        return int ( literal_eval(val) )
+    assert False, f'Unsupported input type: {type(val)}'
+
+def hifread_preproc(addr):
+    """ convert input of hifread into numeric """
+    return numeric_input(addr)
+
+def hifwrite_preproc(addr,val,mask='0xFFFFFFFF'):
+    """ convert input of hifwrite into numeric """
+    return numeric_input(addr),numeric_input(val),numeric_input(mask)
 
-class cp_dummy(object):
+class CpDummyTransport():
     """ A transport mockup """
-    mem = dict()
-           
+    mem = {}
+
     def hifread(self, addr = "0x40000888"):
+        """ Mockup for read a register """
 
         # make sure string format is always the same
-        if isinstance(addr,str):
-            addr = int(literal_eval(addr))
+        addr = hifread_preproc(addr)
 
         addrstr = hex_bw(addr)
-        
+
         # check address exists, or create it
-        if addrstr not in self.mem.keys():
+        if addrstr not in self.mem.keys(): # pylint: disable=C0201
             self.mem[addrstr] = 0
 
-        ret = self.mem[addrstr]
-        return(ret)
+        return self.mem[addrstr]
 
     def hifwrite(self,addr = "0x40000888",val = "0x00000352"):
+        """ Mockup for write a register """
+
+        addr,val,_ = hifwrite_preproc(addr,val)
 
-        if isinstance(addr,str):
-            addr = int( literal_eval(addr) )
-            
-        if isinstance(val, str):
-            val  = int ( literal_eval(val) )
-        
         self.mem[hex_bw(addr)] = val
-            
+
         return int( val )
 
-def test_cp_dummy():
-    t = cp_dummy()
+def test_cp_dummy( transport = CpDummyTransport() ):
+    """ Test transport mockup """
+    print("# Test dummy transport")
     addr = 4
     val = 5
-    t.hifwrite(addr=addr,val=val)
-    assert( val==t.hifread(addr = addr) )
-    pass
+    transport.hifwrite(addr=addr,val=val)
+    assert val==transport.hifread(addr = addr)
 
 if __name__ == '__main__':
     test_cp_dummy()
-    pass
```

### Comparing `cheap_pie-0.9.20/src/cheap_pie/transport/cp_esptool_transport.py` & `cheap_pie-1.0.0/src/cheap_pie/transport/cp_esptool_transport.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,77 @@
 #!/usr/bin/python3
-#
+
+""" Esptool Cheap Pie transport module """
+
 # -*- coding: utf-8 -*-
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
+import os
 from ast import literal_eval
 import esptool
-import os
 
-class cp_esptool(object):
-    """ A wrapper around pyocd transport """
+from cheap_pie.transport.cp_dummy_transport import CpDummyTransport, test_cp_dummy # pylint: disable=E0401
+
+class CpEsptoolTransport(CpDummyTransport):
+    """ A wrapper around esptool transport """
     port = None
-    mem = dict()
-    
+
     def __init__(self, port='/dev/ttyUSB0' ):
-        if port is None:
-            self.port = None
-        else:
-            print('Connecting to pyocd probe... ') 
-            self.port = port
-        
+        self.port = port
+
     def hifread(self, addr = '0x3ff00014'):
-        # print self
-        # print addr    
+        """ read register through esptool """
 
         if isinstance(addr,int):
             # convert to string
             addr = hex(addr)
-            
-        if not self.port is None:
+
+        if self.port is None:
+            # fallback to dummy transport
+            ret = CpDummyTransport.hifread(self,addr)
+        else:
             #  ret = esptool.main( ['--port' , self.port , '--after no_reset', 'read_mem', addr]  )
             # dump value on file... horrible hack because no output available
             tmpfile = 'tmpdump'
-            ret = esptool.main( ['--port' , self.port , '--after', 'no_reset', 'dump_mem', addr, '4', tmpfile]  )
+            ret = esptool.main( # pylint: disable=E1101
+                ['--port' , self.port , '--after',
+                'no_reset', 'dump_mem', addr, '4', tmpfile]
+                               )
 
             if os.path.isfile(tmpfile):
-                f = open(tmpfile, "rb")
-                ret = '0x' + f.read().hex()
-                os.remove(tmpfile)                
+                with open(tmpfile, "rb") as tmpfh:
+                    ret = '0x' + tmpfh.read().hex()
+                os.remove(tmpfile)
             else:
                 ret = 0
 
-            pass
-        else:
-            ret = self.mem[addr]
-            
-        return(ret)
+        return ret
 
-    def hifwrite(self,addr = '0x3ff00014',val = "0x00000352"):
+    def hifwrite(self, addr = '0x3ff00014', val = "0x00000352"):
+        """ write register through esptool """
 
         if isinstance(addr,int):
             addr = hex(addr)
-            
+
         if isinstance(val, int):
             val = hex(val)
-        
-        if not self.port is None:            
-            # ret = esptool.main( ['--port' , self.port , 'write_mem', addr, val ,'0xFFFFFFFF'] )
-            ret = esptool.main( ['--port' , self.port , '--after', 'no_reset' ,'write_mem', addr, val ,'0x0'] )
-            pass
+
+        if self.port is None:
+            # fallback to dummy transport
+            CpDummyTransport.hifwrite(self,addr,val)
         else:
-            # print hex(addr)
-            self.mem[addr] = val
-            
+            esptool.main( # pylint: disable=E1101
+                ['--port' , self.port , '--after', 'no_reset' ,'write_mem', addr, val ,'0x0']
+                )
+
         return literal_eval( val )
-       
 
 def test_cp_esptool():
-    t = cp_esptool(port= None)
-    # t = cp_esptool()
-    addr = '0x3ff00014'
-    val = '2'
-    t.hifwrite(addr=addr,val=val)
-    val=t.hifread(addr = addr)
-    print(val)
-    pass
+    """ Test esptool transport """
+    test_cp_dummy(
+        transport = CpEsptoolTransport(port = None)
+        )
 
 if __name__ == '__main__':
     test_cp_esptool()
-    pass
```

### Comparing `cheap_pie-0.9.20/src/cheap_pie/transport/cp_jlink_transport.py` & `cheap_pie-1.0.0/src/cheap_pie/transport/cp_jlink_transport.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,63 @@
 #!/usr/bin/python3
-#
+
+""" JLink Cheap Pie transport module """
+
 # -*- coding: utf-8 -*-
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
 import pylink
-from ast import literal_eval
-
-class cp_jlink(object):
+from cheap_pie.transport.cp_dummy_transport import CpDummyTransport, test_cp_dummy, \
+    hifread_preproc,hifwrite_preproc # pylint: disable=E0401
+class CpJlinkTransport(CpDummyTransport):
     """ A wrapper around jlink transport """
     jl = None
-    mem = dict()
-    
-    def __init__(self,device = 'QN9080C'):
-        if device is None:
-            self.jl = None
-        else: 
-            self.jl = pylink.JLink()
+
+    def __init__(self, device = None ):
+        if not device is None:
+            self.jl = pylink.JLink() # pylint: disable=C0103
             self.jl.exec_command('ProjectFile = JLinkSettings.ini')
             self.jl.open()
             self.jl.set_speed(10)
             self.jl.set_tif(pylink.enums.JLinkInterfaces.SWD)
             self.jl.connect(device)
-            assert(self.jl.connected()==True)
+            assert self.jl.connected()
 
     def __del__(self):
-        if not (self.jl is None):
+        if not self.jl is None:
             self.jl.close()
-        
+
     def hifread(self, addr = "0x40000888"):
-        # print self
-        # print addr    
+        """ read register through JLink """
 
-        if isinstance(addr,str):
-            addr = int(literal_eval(addr))
-            
-        if not self.jl is None:
-            r = self.jl.memory_read32(addr,1)
-            ret = r[0]
+        addr = hifread_preproc(addr)
+
+        if self.jl is None:
+            ret = CpDummyTransport.hifread(self,addr)
         else:
-            ret = self.mem[hex(addr)]
-            
-        # print hex(r[0])
-        return(ret)
+            read = self.jl.memory_read32(addr,1)
+            ret = read[0]
+
+        return ret
 
     def hifwrite(self,addr = "0x40000888",val = "0x00000352"):
+        """ write register through JLink """
 
-        if isinstance(addr,str):
-            addr = int( literal_eval(addr) )
-            
-        if isinstance(val, str):
-            val = int ( literal_eval(val) )
-        
-        if not self.jl is None:
-            self.jl.memory_write32( addr, [val] )
+        addr,val,_ = hifwrite_preproc(addr,val)
+
+        if self.jl is None:
+            CpDummyTransport.hifwrite(self, addr, val)
         else:
-            # print hex(addr)
-            self.mem[hex(addr)] = val
-            
+            self.jl.memory_write32( addr, [val] )
+
         return int( val )
-        
-    """ def halt(self):
-        self.jl.halt()
-        return(0)
-        
-    def go(self):
-        self.jl.go()
-        return(0) """
 
 def test_cp_jlink():
-    t = cp_jlink(device = None)
-    addr = 4
-    val = 5
-    t.hifwrite(addr=addr,val=val)
-    val=t.hifread(addr = addr)
-    pass
+    """ test JLink transport """
+    test_cp_dummy(
+        CpJlinkTransport(device = None)
+    )
 
 if __name__ == '__main__':
     test_cp_jlink()
-    pass
```

### Comparing `cheap_pie-0.9.20/src/cheap_pie/transport/cp_pyverilator_transport.py` & `cheap_pie-1.0.0/src/cheap_pie/transport/cp_pyverilator_transport.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 Cheap Pie module for pyverilator transport
 """
 import os
 import argparse
 import sys
 from ast import literal_eval
 from shutil import copyfile
+import subprocess
+from packaging import version
 
 import pyverilator
 
-def cli(args=[]):
+from cheap_pie.transport.cp_dummy_transport import hifread_preproc, hifwrite_preproc # pylint: disable=E0401
+
+def cli(args):
     """ Command Line Interface for pyverilator transport class """
     parser = argparse.ArgumentParser(description='rdl2verilog pyverilator ')
     # register format options
     parser.add_argument("-f", "--fname",
                         help="register file description .v", action='store',
                         type = str, default="./devices/verilog/basic_rf.v")
     return parser.parse_args(args)
 
-class cp_pyverilator_transport():
+class CpPyverilatorTransport():
     """
     Cheap Pie class for pyverilator transport
     """
     sim = None
 
     def __init__(self,fname):
 
@@ -82,22 +86,16 @@
         # check out when en = 1
         # sim.io.en = 1
         # curr_out = sim.io.out
         # print('sim.io.out = ' + str(curr_out))
 
     def hifwrite(self, addr='0x00', val='0xB16B00B5', mask='0xFFFFFFFF'):
         """ Write register """
-        if isinstance(addr,str):
-            addr = literal_eval(addr)
-
-        if isinstance(val,str):
-            val = literal_eval(val)
 
-        if isinstance(mask,str):
-            mask = literal_eval(mask)
+        addr,val,mask = hifwrite_preproc(addr,val,mask)
 
         # write value
         self.sim.io.addr = addr
         self.sim.io.wdata = val
         self.sim.io.wmask = mask
         self.sim.io.read = 0
         self.sim.io.valid = 0
@@ -117,16 +115,15 @@
         # sim.io.basicreg_basicfield_we = 0
         # sim.clock.tick()
         # sim.io.basicreg_basicfield_we = 1
         # sim.clock.tick()
 
     def hifread(self,addr = '0x00'):
         """ Read register """
-        if isinstance(addr,str):
-            addr = literal_eval(addr)
+        addr = hifread_preproc(addr)
 
         # SW read
         self.sim.io.addr = addr
         self.sim.io.read = 1
 
         self.sim.io.valid = 0
         self.sim.clock.tick()
@@ -140,37 +137,35 @@
         self.sim.clock.tick()
 
         # print(hex(outval))
         return outval
 
 def verilator_version():
     """ Return verilator version """
-    import subprocess
-    result = subprocess.run(['verilator', '--version'], stdout=subprocess.PIPE)
+    result = subprocess.run(['verilator', '--version'], stdout=subprocess.PIPE, check=False)
     ver = result.stdout.split()[1]
     return ver.decode("utf-8")
 
 def verilator_version_ok():
     """ True if the installed verilator version works as transport for cheap_pie """
     # check Verilated::flushCall() exist
     # https://github.com/chipsalliance/chisel3/issues/1565
-    from packaging import version
     ver = verilator_version()
     # print(ver)
-    if ( version.parse(ver) < version.parse("4.036") or
-         version.parse(ver) > version.parse("4.102")):
-        return True
-    else:
-        return False
 
-def test_cp_pyverilator(args = []):
+    return (
+            version.parse(ver) < version.parse("4.036") or
+            version.parse(ver) > version.parse("4.102")
+            )
+
+def test_cp_pyverilator(args=[]): # pylint: disable=W0102
     """ Test pyverilator transport """
     if verilator_version_ok():
         prms = cli(args)
-        hif = cp_pyverilator_transport(prms.fname)
+        hif = CpPyverilatorTransport(prms.fname)
         val = literal_eval('0x5A5A5A5A')
         hif.hifwrite(val = val)
         print( hex(hif.hifread()) )
         assert hif.hifread() == val
     else:
         print('Warning: pyverilator not working anymore \
               with verilator versions between 4.036 and 4.102.')
```

### Comparing `cheap_pie-0.9.20/src/cheap_pie.egg-info/SOURCES.txt` & `cheap_pie-1.0.0/src/cheap_pie.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,35 +6,32 @@
 src/cheap_pie.egg-info/PKG-INFO
 src/cheap_pie.egg-info/SOURCES.txt
 src/cheap_pie.egg-info/dependency_links.txt
 src/cheap_pie.egg-info/requires.txt
 src/cheap_pie.egg-info/top_level.txt
 src/cheap_pie/cheap_pie_core/__init__.py
 src/cheap_pie/cheap_pie_core/cbitfield.py
-src/cheap_pie/cheap_pie_core/cheap_pie.py
+src/cheap_pie/cheap_pie_core/cheap_pie_main.py
 src/cheap_pie/cheap_pie_core/cp_banner.py
+src/cheap_pie/cheap_pie_core/cp_builder.py
 src/cheap_pie/cheap_pie_core/cp_cli.py
 src/cheap_pie/cheap_pie_core/cp_hal.py
 src/cheap_pie/cheap_pie_core/cp_register.py
 src/cheap_pie/cheap_pie_core/test.py
 src/cheap_pie/parsers/__init__.py
 src/cheap_pie/parsers/cp_parsers_wrapper.py
 src/cheap_pie/parsers/ipxact_parse.py
 src/cheap_pie/parsers/ipyxact_parse.py
-src/cheap_pie/parsers/name_subs.py
 src/cheap_pie/parsers/rdl_parse.py
 src/cheap_pie/parsers/svd_parse.py
 src/cheap_pie/parsers/svd_parse_repo.py
 src/cheap_pie/parsers/xml_xslt.py
 src/cheap_pie/tools/__init__.py
 src/cheap_pie/tools/hal2doc.py
 src/cheap_pie/tools/rdl2any.py
-src/cheap_pie/tools/rdl2verilog.py
-src/cheap_pie/tools/reload_module.py
 src/cheap_pie/tools/search.py
-src/cheap_pie/tools/test_rdl.py
 src/cheap_pie/transport/__init__.py
 src/cheap_pie/transport/cp_dummy_transport.py
 src/cheap_pie/transport/cp_esptool_transport.py
 src/cheap_pie/transport/cp_jlink_transport.py
 src/cheap_pie/transport/cp_pyocd_transport.py
 src/cheap_pie/transport/cp_pyverilator_transport.py
```

