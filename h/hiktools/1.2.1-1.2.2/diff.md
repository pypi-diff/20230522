# Comparing `tmp/hiktools-1.2.1.tar.gz` & `tmp/hiktools-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiktools-1.2.1.tar", last modified: Sun Mar  5 20:32:49 2023, max compression
+gzip compressed data, was "hiktools-1.2.2.tar", last modified: Mon May 22 07:03:34 2023, max compression
```

## Comparing `hiktools-1.2.1.tar` & `hiktools-1.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-05 20:32:49.891592 hiktools-1.2.1/
--rw-rw-rw-   0        0        0     1088 2023-01-16 21:48:12.000000 hiktools-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     4942 2023-03-05 20:32:49.887593 hiktools-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4093 2023-03-05 20:31:54.000000 hiktools-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-05 20:32:49.521430 hiktools-1.2.1/hiktools/
--rw-rw-rw-   0        0        0     1183 2023-03-05 20:30:09.000000 hiktools-1.2.1/hiktools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-05 20:32:49.702232 hiktools-1.2.1/hiktools/csadp/
--rw-rw-rw-   0        0        0     2176 2023-03-05 08:32:29.000000 hiktools-1.2.1/hiktools/csadp/CService.py
--rw-rw-rw-   0        0        0     1351 2023-03-05 08:33:10.000000 hiktools-1.2.1/hiktools/csadp/__init__.py
--rw-rw-rw-   0        0        0     2577 2023-03-05 08:25:01.000000 hiktools-1.2.1/hiktools/csadp/checksum.py
--rw-rw-rw-   0        0        0     8762 2023-03-05 08:35:45.000000 hiktools-1.2.1/hiktools/csadp/model.py
--rw-rw-rw-   0        0        0     2454 2023-03-05 08:34:49.000000 hiktools-1.2.1/hiktools/csadp/payloads.py
--rw-rw-rw-   0        0        0     2625 2023-03-05 08:22:34.000000 hiktools-1.2.1/hiktools/csadp/uarray.py
-drwxrwxrwx   0        0        0        0 2023-03-05 20:32:49.781490 hiktools-1.2.1/hiktools/fmod/
--rw-rw-rw-   0        0        0     1208 2023-03-05 07:33:46.000000 hiktools-1.2.1/hiktools/fmod/__init__.py
--rw-rw-rw-   0        0        0     1733 2023-03-05 07:35:16.000000 hiktools-1.2.1/hiktools/fmod/__main__.py
--rw-rw-rw-   0        0        0    14387 2023-03-05 14:02:52.000000 hiktools-1.2.1/hiktools/fmod/decrypter.py
--rw-rw-rw-   0        0        0     1895 2023-03-05 08:17:58.000000 hiktools-1.2.1/hiktools/fmod/extractor.py
-drwxrwxrwx   0        0        0        0 2023-03-05 20:32:49.848279 hiktools-1.2.1/hiktools/sadp/
--rw-rw-rw-   0        0        0     1330 2023-03-05 07:26:44.000000 hiktools-1.2.1/hiktools/sadp/__init__.py
--rw-rw-rw-   0        0        0     3970 2023-03-05 07:32:47.000000 hiktools-1.2.1/hiktools/sadp/client.py
--rw-rw-rw-   0        0        0    10030 2023-03-05 07:25:17.000000 hiktools-1.2.1/hiktools/sadp/message.py
-drwxrwxrwx   0        0        0        0 2023-03-05 20:32:49.576235 hiktools-1.2.1/hiktools.egg-info/
--rw-rw-rw-   0        0        0     4942 2023-03-05 20:32:49.000000 hiktools-1.2.1/hiktools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2023-03-05 20:32:49.000000 hiktools-1.2.1/hiktools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-05 20:32:49.000000 hiktools-1.2.1/hiktools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-05 20:32:49.000000 hiktools-1.2.1/hiktools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      878 2023-03-05 20:30:09.000000 hiktools-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-05 20:32:49.896592 hiktools-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 07:03:34.207636 hiktools-1.2.2/
+-rw-rw-rw-   0        0        0     1088 2023-01-16 21:48:12.000000 hiktools-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     5980 2023-05-22 07:03:34.208637 hiktools-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5131 2023-05-22 06:58:35.000000 hiktools-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 07:03:33.715300 hiktools-1.2.2/hiktools/
+-rw-rw-rw-   0        0        0     1183 2023-05-22 06:58:35.000000 hiktools-1.2.2/hiktools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:03:33.950839 hiktools-1.2.2/hiktools/csadp/
+-rw-rw-rw-   0        0        0     2174 2023-05-22 06:58:35.000000 hiktools-1.2.2/hiktools/csadp/CService.py
+-rw-rw-rw-   0        0        0     1351 2023-03-05 08:33:10.000000 hiktools-1.2.2/hiktools/csadp/__init__.py
+-rw-rw-rw-   0        0        0     2567 2023-05-22 06:58:35.000000 hiktools-1.2.2/hiktools/csadp/checksum.py
+-rw-rw-rw-   0        0        0     8961 2023-05-22 06:58:35.000000 hiktools-1.2.2/hiktools/csadp/model.py
+-rw-rw-rw-   0        0        0     2450 2023-05-22 06:58:35.000000 hiktools-1.2.2/hiktools/csadp/payloads.py
+-rw-rw-rw-   0        0        0     2669 2023-05-22 06:58:35.000000 hiktools-1.2.2/hiktools/csadp/uarray.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:03:34.076141 hiktools-1.2.2/hiktools/fmod/
+-rw-rw-rw-   0        0        0     1203 2023-05-22 06:58:35.000000 hiktools-1.2.2/hiktools/fmod/__init__.py
+-rw-rw-rw-   0        0        0     1725 2023-05-22 06:58:35.000000 hiktools-1.2.2/hiktools/fmod/__main__.py
+-rw-rw-rw-   0        0        0    14944 2023-05-22 06:58:35.000000 hiktools-1.2.2/hiktools/fmod/digicap.py
+-rw-rw-rw-   0        0        0     1902 2023-05-22 06:58:35.000000 hiktools-1.2.2/hiktools/fmod/export.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:03:34.178641 hiktools-1.2.2/hiktools/sadp/
+-rw-rw-rw-   0        0        0     1330 2023-03-05 07:26:44.000000 hiktools-1.2.2/hiktools/sadp/__init__.py
+-rw-rw-rw-   0        0        0     4033 2023-05-22 06:58:35.000000 hiktools-1.2.2/hiktools/sadp/client.py
+-rw-rw-rw-   0        0        0    10206 2023-05-22 06:58:35.000000 hiktools-1.2.2/hiktools/sadp/message.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:03:33.773299 hiktools-1.2.2/hiktools.egg-info/
+-rw-rw-rw-   0        0        0     5980 2023-05-22 07:03:33.000000 hiktools-1.2.2/hiktools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2023-05-22 07:03:33.000000 hiktools-1.2.2/hiktools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 07:03:33.000000 hiktools-1.2.2/hiktools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 07:03:33.000000 hiktools-1.2.2/hiktools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      876 2023-05-22 06:58:35.000000 hiktools-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-22 07:03:34.216886 hiktools-1.2.2/setup.cfg
```

### Comparing `hiktools-1.2.1/LICENSE` & `hiktools-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hiktools-1.2.1/PKG-INFO` & `hiktools-1.2.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,60 @@
-Metadata-Version: 2.1
-Name: hiktools
-Version: 1.2.1
-Summary: Hikvision utility tools
-Author-email: MatrixEditor <not@supported.com>
-Project-URL: Homepage, https://github.com/MatrixEditor/hiktools
-Project-URL: API-Docs, https://hiktools.readthedocs.io
-Project-URL: Native-API-Docs, https://matrixeditor.github.io/hiktools/docs/html/d3/dcc/md__r_e_a_d_m_e.html
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Hiktools
 
 ![Module](https://img.shields.io:/static/v1?label=Module&message=hiktools&color=9cf)
 ![Build](https://img.shields.io:/static/v1?label=Python&message=>=3.5&color=green)
 ![Platform](https://img.shields.io:/static/v1?label=Platforms&message=Linux|Windows&color=yellowgreen)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.2.1&color=green)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.2.2&color=green)
 
-This is now a small project with four main functionalities: 
 
+This respository was former known as `hikvision-sdk-cam`, but has changed since the old content of this repository was deleted. This is now a small project with four main functionalities:
 * A Wireshark dissector for the Search Active Devices Protocol,
-* Decrypt and extract hikvision firmware, 
-* Send raw SADP packets (only Linux) and 
-* Send commands via UDP Broadcast. 
+* Decrypt and extract hikvision firmware,
+* Send raw SADP packets (only Linux) and
+* Send commands via UDP Broadcast.
 
-To get familiar with the API provided in this repository, take a quick look at the python documentation available **[here »](https://hiktools.readthedocs.io/)** or the 
+To get familiar with the API provided in this repository, take a quick look at the python documentation available **[here »](https://hiktools.readthedocs.io/)** or the
 C++ documentation available at Github-Pages **[here »](https://matrixeditor.github.io/hiktools/docs/html/d3/dcc/md__r_e_a_d_m_e.html)**.
 
+### Installation
+
+You can now install the `hiktools` module with pip:
+
+```bash
+$ python3 -m pip install hiktools
+```
+
 ### Overview
 ---
 **Update:** Since feature version `1.1.0` the native packet creation and communication works! It is still only usable on UNIX systems that support sending raw ethernet frames. The checksum algorithm was disassebled and decompiled correctly, just the input parameters were interpreted wrong. The algorithm is implemented in [C/C++](/cpp/checksum.h) and [python3](/hiktools/csadp/checksum.py).
 
-Communication on UDP works fine at the moment - this API is just a small wrapper which can be used for a more general API. 
+Communication on UDP works fine at the moment - this API is just a small wrapper which can be used for a more general API.
+
+Firmware decryption and extraction will only work on newer `digicap.dav` files with at least  `1` file entry (otherwise there will be no files to inspect) in the header. All firmware files and updates can be downloaded from the following endpoint (EU):
+
+* https://www.hikvisioneurope.com/uk/portal
 
-Firmware decryption and extraction will only work on newer `digicap.dav` files with at least one file entry (otherwise there will be no files to inspect) in the header. All firmware files and updates can be downloaded from the following endpoint (EU):
+There is also a full list of files available at this enpoint stored in a JSON file named [firmwarelist.json](/gists/firmwarelist.json).
+
+> Info: There is an interesting file located in the extracted files of a firmware image: /hroot.img/initrd/etc/passwd. A password is set to the root user:
+
+    Name: passwd
+    Folder: -
+    Size: 44
+    Packed Size: 1 024
+    Mode: -rwxrwxr-x
+    Last change: 2016-12-23 08:27:46
+    Last modification: 2016-12-23 08:27:46
+    -------------------------------------------
+
+    root:ToCOv8qxP13qs:0:0:root:/root/:/bin/psh
+
+The plain password is `hiklinux`, kudos to [Don Bowman](https://blog.donbowman.ca/2018/01/18/hacking-the-hikvision-part-1/).
+
+> Old exploit with authkey := YWRtaW46MTEK
 
 ### Basic Usage
 ---
 
 - Firmware inspection and extraction
 
 ```python
@@ -69,15 +79,15 @@
 python3 -m hiktools.fmod input.dav outputDir
 ```
 
 - Native interface on sending raw packets (only LINUX)
 ```python
 from hiktools import csadp
 
-# Because the following module requires root priviledges it 
+# Because the following module requires root priviledges it
 # has to be imported directly.
 from hiktools.csadp import CService
 
 sock = CService.l2socket('wlan0')
 counter = 0x115e
 
 # To build an Inquiry packet, we need the following information:
@@ -115,12 +125,12 @@
   for response in client:
     if response is None: break
     # initiate the response
     message = sadp.unmarshal(response.toxml())
 
     # message objects contain a dict-like implementation
     for property_name in message:
-      print(message[property_name]) 
-    
+      print(message[property_name])
+
     # e.g.
     print('Device at', message['IPv4Address'])
 ```
```

### Comparing `hiktools-1.2.1/hiktools/__init__.py` & `hiktools-1.2.2/hiktools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = '1.2.1'
+__version__ = '1.2.2'
 __author__  = 'MatrixEditor'
```

### Comparing `hiktools-1.2.1/hiktools/csadp/CService.py` & `hiktools-1.2.2/hiktools/csadp/CService.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,38 +22,37 @@
 """
 `WARNING`: This module is usable only on linux systems.
 
 A small module which ensures the right permissions are used to execute the
 script base. It covers the creation of a layer 2 socket.
 """
 
-__all__ = ['l2socket']
+__all__ = ["l2socket"]
 
 import socket
 
 from sys import platform
 
 # Check if the program is running with root priviledges
-if platform != 'linux':
-    raise OSError('Unsupported platform for layer II network operations!')
+if platform != "linux":
+    raise OSError("Unsupported platform for layer II network operations!")
 else:
     try:
         import os
 
         if os.getuid():
-            raise PermissionError('This library requires super-user priviledges.')
+            raise PermissionError("This library requires super-user priviledges.")
 
     except AttributeError as exc:
-        raise PermissionError('This library requires super-user priviledges.') from exc
+        raise PermissionError("This library requires super-user priviledges.") from exc
 
 
 def l2socket(interface: str) -> socket.socket:
     """Creates a layer II socket and binds it to the given interface."""
     if not interface:
-        raise ValueError('Interface not specified')
+        raise ValueError("Interface not specified")
 
     sock = socket.socket(socket.PF_PACKET, socket.SOCK_RAW)
     sock.settimeout(2)
     sock.bind((interface, 0))
 
     return sock
-
```

### Comparing `hiktools-1.2.1/hiktools/csadp/__init__.py` & `hiktools-1.2.2/hiktools/csadp/__init__.py`

 * *Files identical despite different names*

### Comparing `hiktools-1.2.1/hiktools/csadp/checksum.py` & `hiktools-1.2.2/hiktools/csadp/checksum.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,36 +15,35 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-__all__ = [
-  'get_checksum'
-]
+__all__ = ["get_checksum"]
 
 from hiktools.csadp.uarray import UIntArray
 
+
 def get_checksum(buf: UIntArray, prefix: int) -> int:
-    '''The SADP checksum algorithm implemented in python3.
+    """The SADP checksum algorithm implemented in python3.
 
     For a more accurate view on the algorithm, see the C++ source code on the
     `hiktools`_ repository on github.
 
     :param buf: an unsinged int16 array (can be created via a call to
                   ``to_uint16_buf()``)
     :param prefix: the sender's type specification. As defined in the C++
                   header file, ``0x42`` specifies a client and ``0xf6``
                   an server.
-    '''
-    csum : int  = 0
-    lower: int  = 0
-    high : int  = 0
-    index: int  = 0
+    """
+    csum: int = 0
+    lower: int = 0
+    high: int = 0
+    index: int = 0
 
     if 3 < (prefix & 0xFFFFFFFE):
         index = (prefix - 4 >> 2) + 1
         while index != 0:
             prefix -= 4
             lower += buf[0]
             high += buf[1]
```

### Comparing `hiktools-1.2.1/hiktools/csadp/model.py` & `hiktools-1.2.2/hiktools/csadp/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,90 +15,94 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-__doc__ = '''
+__doc__ = """
 CSADP packets are wrapped into objects that support the ``__bytes__`` method to
 dynamically create the byte buffer.
 
 This module covers the conversion between binary data to MAC- and IP addressees
 and defines base classes for SADPPackets.
-'''
+"""
 
 import struct
 import binascii
 
-from socket import (
-  AF_INET6,
-  inet_aton,
-  inet_ntoa,
-  inet_ntop,
-  inet_pton
-)
+from socket import AF_INET6, inet_aton, inet_ntoa, inet_ntop, inet_pton
 
 from hiktools.csadp.checksum import get_checksum
 from hiktools.csadp.uarray import LITTLE_ENDIAN, to_uint16_buf
 
 __all__ = [
-  'inet_stomac', 'inet_mactos', 'inet_stoip', 'inet_iptos',
-  'EthernetHeader', 'SADPHeader', 'SADPPacket', 'SERVER_PREFIX',
-  'CLIENT_PREFIX', 'PACKET_TYPE', 'inet6_stoip', 'inet6_iptos',
-  'SADPPayload', 'payload'
+    "inet_stomac",
+    "inet_mactos",
+    "inet_stoip",
+    "inet_iptos",
+    "EthernetHeader",
+    "SADPHeader",
+    "SADPPacket",
+    "SERVER_PREFIX",
+    "CLIENT_PREFIX",
+    "PACKET_TYPE",
+    "inet6_stoip",
+    "inet6_iptos",
+    "SADPPayload",
+    "payload",
 ]
 
 CLIENT_PREFIX = 0x42
-SERVER_PREFIX = 0xf6
+SERVER_PREFIX = 0xF6
 
 PACKET_TYPE = {
     "DeviceOnlineRequest": 0x02,
     "Inquiry": 0x03,
     "InquiryResponse": 0x04,
     "UpdateIP": 0x06,
     "UpdateIPResponse": 0x07,
-    "ResetPassword": 0x0a,
-    "ResetPasswordResponse": 0x0b,
-    "CMSInfo": 0x0c,
-    "CMSInfoResponse": 0x0d,
+    "ResetPassword": 0x0A,
+    "ResetPasswordResponse": 0x0B,
+    "CMSInfo": 0x0C,
+    "CMSInfoResponse": 0x0D,
     "ModifyNetParam": 0x10,
-    "ModifyNetParamResponse": 0x11
+    "ModifyNetParamResponse": 0x11,
 }
 
 PAYLOAD_TYPE = {
-  # structure of this dict
-  # int: class<? extends SADPPayload>, ...
+    # structure of this dict
+    # int: class<? extends SADPPayload>, ...
 }
 
 
 def inet_stomac(mac: str) -> bytes:
     """Converts the string mac address into a byte buffer."""
-    mac = mac.replace(':', '').replace('-', '')
+    mac = mac.replace(":", "").replace("-", "")
     return binascii.unhexlify(mac)
 
 
-def inet_mactos(buffer: bytes, index: int, sep: str =':') -> str:
+def inet_mactos(buffer: bytes, index: int, sep: str = ":") -> str:
     """Converts bytes to a MAC address."""
-    return binascii.b2a_hex(buffer[index:index+6], sep=sep).decode('utf-8')
+    return binascii.b2a_hex(buffer[index : index + 6], sep=sep).decode("utf-8")
 
 
 def inet_stoip(ip_address: str) -> bytes:
     """Converts the string ip address into a byte buffer."""
     return inet_aton(ip_address)
 
 
 def inet_iptos(buffer: bytes, offset: int) -> str:
     """Converts bytes to an IP address."""
-    return inet_ntoa(buffer[offset:offset+4])
+    return inet_ntoa(buffer[offset : offset + 4])
 
 
 def inet6_iptos(buffer: bytes, offset: int) -> str:
     """Converts bytes to an IP address."""
-    return inet_ntop(AF_INET6, buffer[offset:offset+16])
+    return inet_ntop(AF_INET6, buffer[offset : offset + 16])
 
 
 def inet6_stoip(ip6: str) -> bytes:
     """Converts the string ip address into a byte buffer."""
     return inet_pton(AF_INET6, ip6)
 
 
@@ -122,79 +126,92 @@
 
     :param eth_type: The specified ethernet type for this packet. This value can
                     be used for validation, because it has to be ``0x8033``.
     :type eth_type: uint16 (int)
     """
 
     def __init__(self, buf: bytes = None) -> None:
-        self.dest: str = 'FF:FF:FF:FF:FF:FF'
+        self.dest: str = "FF:FF:FF:FF:FF:FF"
         self.src: str = ""
         self.eth_type: int = 0x8033
         if buf is not None and len(buf) >= 14:
             self.dest = inet_mactos(buf, 0)
             self.src = inet_mactos(buf, 6)
-            self.eth_type = struct.unpack('!H', buf[12:14])[0]
+            self.eth_type = struct.unpack("!H", buf[12:14])[0]
 
     def __bytes__(self) -> bytes:
         """Packs this header object into a byte buffer.
 
         The returned structure is defined in the documentation of this class.
 
         :returns: all values stored by this header object packed into a byte buffer.
         """
         buf = bytearray()
         buf += inet_stomac(self.dest)
         buf += inet_stomac(self.src)
-        buf += struct.pack('!H', self.eth_type)
+        buf += struct.pack("!H", self.eth_type)
         return bytes(buf)
 
 
 class SADPHeader:
     """A simple class wrapper to store header variables of SADPPackets."""
+
     def __init__(self, buf: bytes = None) -> None:
-        self.prefix: int = 0 #  uint8
-        self.counter: int = 0 # uint32
-        self.packet_type: int = 0 # uint8
-        self.params: int = 0 # uint8
-        self.checksum: int = 0 # uint16
+        self.prefix: int = 0  #  uint8
+        self.counter: int = 0  # uint32
+        self.packet_type: int = 0  # uint8
+        self.params: int = 0  # uint8
+        self.checksum: int = 0  # uint16
         if buf is not None and len(buf) >= 14:
-            values = struct.unpack('!HBBIHBBH', buf)
+            values = struct.unpack("!HBBIHBBH", buf)
             self.prefix = values[2]
             self.counter = values[3]
             self.packet_type = values[5]
             self.params = values[6]
             self.checksum = values[7]
 
     def __bytes__(self) -> bytes:
         buf = bytearray(14)
-        struct.pack_into('!HBBIHBBH', buf, 0,
-            0x2102, 0x01, self.prefix, self.counter, 0x0604,
-            self.packet_type, self.params, self.checksum
+        struct.pack_into(
+            "!HBBIHBBH",
+            buf,
+            0,
+            0x2102,
+            0x01,
+            self.prefix,
+            self.counter,
+            0x0604,
+            self.packet_type,
+            self.params,
+            self.checksum,
         )
         return bytes(buf)
 
 
 class SADPPayload:
     """The base class for all payload types."""
+
     def __init__(self, buf: bytes = None) -> None:
         self.buf = buf
 
     def __bytes__(self) -> bytes:
         raise NotImplementedError(
-            'Abstract class SADPPayload does not implement __bytes__()')
+            "Abstract class SADPPayload does not implement __bytes__()"
+        )
+
 
 class SADPPacket:
     """A dynamic class for creating SADPPackets for sending and resceiving data."""
 
     def __init__(self, buf: bytes = None) -> None:
         self.eth_header: EthernetHeader = EthernetHeader(buf[:14] if buf else None)
         self.header: SADPHeader = SADPHeader(buf[14:] if buf else None)
-        self.src_ip: str = ''
-        self.dest_ip: str = '0.0.0.0'
-        self.subnet: str = '0.0.0.0'
+        self.src_ip: str = ""
+        self.dest_ip: str = "0.0.0.0"
+        self.subnet: str = "0.0.0.0"
         self.payload: SADPPayload = SADPPayload()
         if buf is not None and len(buf) >= 52:
             self.src_ip = inet_iptos(buf, 34)
             self.dest_ip = inet_iptos(buf, 44)
             self.subnet = inet_iptos(buf, 48)
             self.payload = SADPPayload()
             if self.header.packet_type in PAYLOAD_TYPE:
@@ -232,14 +249,15 @@
 
     >>> @payload(PACKET_TYPE['UpdateIP'])
     >>> class MySADPPayload(SADPPayload):
     ...    pass
 
     :param ptype: the packet type the payload class should be mapped to
     """
+
     def do_register(payload_type):
         if ptype in PAYLOAD_TYPE:
-            raise NameError(f'Payload of type {ptype} already exists')
+            raise NameError(f"Payload of type {ptype} already exists")
         PAYLOAD_TYPE[ptype] = payload_type
         return payload_type
 
     return do_register
```

### Comparing `hiktools-1.2.1/hiktools/csadp/payloads.py` & `hiktools-1.2.2/hiktools/csadp/payloads.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,34 +15,32 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-__doc__ = '''
+__doc__ = """
 Known payload implementations.
-'''
+"""
 
-__all__ = [
-    'InquiryPayload', 'inquiry', 'InquiryResponsePayload'
-]
+__all__ = ["InquiryPayload", "inquiry", "InquiryResponsePayload"]
 
 from hiktools.csadp.model import (
-    SADPPayload, SADPPacket,
-
+    SADPPayload,
+    SADPPacket,
     payload,
     inet6_iptos,
     inet6_stoip,
-
     CLIENT_PREFIX,
-    PACKET_TYPE
+    PACKET_TYPE,
 )
 
-@payload(PACKET_TYPE['Inquiry'])
+
+@payload(PACKET_TYPE["Inquiry"])
 class InquiryPayload(SADPPayload):
     def __init__(self, ipv6: str = None, buf: bytes = None) -> None:
         super().__init__(buf)
         self.ipaddress = ipv6
         if self.buf is not None:
             self.ipaddress = inet6_iptos(self.buf, 0)
 
@@ -51,21 +49,21 @@
             self.buf = bytearray()
             self.buf += inet6_stoip(self.ipaddress)
             self.buf += bytes([0 for _ in range(12)])
             self.buf = bytes(self.buf)
         return self.buf
 
 
-@payload(PACKET_TYPE['InquiryResponse'])
+@payload(PACKET_TYPE["InquiryResponse"])
 class InquiryResponsePayload(SADPPayload):
     pass
 
 
 def inquiry(mac: str, ipv4: str, ipv6: str, counter: int) -> SADPPacket:
     packet = SADPPacket()
     packet.eth_header.src = mac
-    packet.header.packet_type = PACKET_TYPE['Inquiry']
+    packet.header.packet_type = PACKET_TYPE["Inquiry"]
     packet.header.counter = counter
     packet.header.prefix = CLIENT_PREFIX
     packet.src_ip = ipv4
     packet.payload = InquiryPayload(ipv6=ipv6)
     return packet
```

### Comparing `hiktools-1.2.1/hiktools/csadp/uarray.py` & `hiktools-1.2.2/hiktools/csadp/uarray.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,30 +18,32 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import struct
 
-__all__ = [
-  'LITTLE_ENDIAN', 'BIG_ENDIAN', 'UIntArray', 'to_uint16_buf'
-]
+__all__ = ["LITTLE_ENDIAN", "BIG_ENDIAN", "UIntArray", "to_uint16_buf"]
+
+LITTLE_ENDIAN = "<"
+BIG_ENDIAN = ">"
 
-LITTLE_ENDIAN = '<'
-BIG_ENDIAN = '>'
 
 class UIntArray(list):
     """Simple wrapper class for byte buffers."""
+
     def __init__(self, bytes_size: int) -> None:
-        self.max = 1 << bytes_size*8
+        self.max = 1 << bytes_size * 8
 
-    def __iadd__(self, __x: list) -> 'UIntArray':
+    def __iadd__(self, __x: list) -> "UIntArray":
         for i, val in enumerate(__x):
             if self.max <= val:
-                raise TypeError('Unsupported value (0 - %#x) at index %d' % (self.max - 1, i))
+                raise TypeError(
+                    "Unsupported value (0 - %#x) at index %d" % (self.max - 1, i)
+                )
         return super().__iadd__(__x)
 
 
 def to_uint16_buf(buffer: bytes, encoding: str = BIG_ENDIAN) -> UIntArray:
     """Converts the given byte buffer into an unsigned 16-bit integer array.
 
     :param buffer: the raw bytes buffer
@@ -50,19 +52,19 @@
     :type encoding: str, optional
     :raises ValueError: if an invalid encoding is provided
     :raises ValueError: if an invalid input length is provided
     :return: the converted buffer
     :rtype: UIntArray
     """
     if 62 < ord(encoding) or 60 > ord(encoding):
-        raise ValueError('Invalid encoding value')
+        raise ValueError("Invalid encoding value")
 
     length = len(buffer)
     if length == 0:
         return buffer
     if length % 2 != 0:
-        raise ValueError(f'Invalid input array length ({length})')
+        raise ValueError(f"Invalid input array length ({length})")
 
     seq = UIntArray(2)
     for i in range(0, len(buffer), 2):
-        seq += struct.unpack(encoding + 'H', bytes(buffer[i:i+2]))
+        seq += struct.unpack(encoding + "H", bytes(buffer[i : i + 2]))
     return seq
```

### Comparing `hiktools-1.2.1/hiktools/fmod/__init__.py` & `hiktools-1.2.2/hiktools/fmod/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from hiktools.fmod.decrypter import *
-from hiktools.fmod.extractor import *
+from hiktools.fmod.digicap import *
+from hiktools.fmod.export import *
```

### Comparing `hiktools-1.2.1/hiktools/fmod/__main__.py` & `hiktools-1.2.2/hiktools/fmod/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 
 from hiktools.fmod import DigiCap, export
 
 if __name__ == '__main__':
     args = len(sys.argv)
 
     if args == 2 and sys.argv[1] == '-h':
-        print(f'Usage: {__file__} <Input File> <Output DIR>\n')
+        print(f'Usage: {__name__} <Input File> <Output DIR>')
         sys.exit(1)
 
     if args != 3:
         print('[-] Expected only 2 arguments (type -h for help).')
         sys.exit(1)
 
     with DigiCap(sys.argv[1]) as dcap:
-        print("Got", dcap.head.files.value, "files to save!")
+        print("Got", dcap.head.files, "files to save!")
         export(dcap, sys.argv[2])
         for resource in dcap:
             print('> File name="%s", size=%d, pos=%d, checksum=%d' % resource)
```

### Comparing `hiktools-1.2.1/hiktools/fmod/decrypter.py` & `hiktools-1.2.2/hiktools/fmod/digicap.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,57 +26,79 @@
 The basic process of decrpytion os the following:
     - Read the raw header (first 108 bytes)
     - Decode the header XOR with the decryption key
     - Parse the header
     - Decode the rest of the firmware file XOR with the decryption key
     - Parse the embedded files
 """
+from __future__ import annotations
 
 __all__ = [
-  'InvalidFileFormatException', 'FileAccessException', 'DigiCapHeader',
-  'read_raw_header', 'decode_xor16', 'split_header', 'split_files',
-  'fopen_dav', 'DigiCap'
+    "InvalidFileFormatException",
+    "FileAccessException",
+    "DigiCapHeader",
+    "read_raw_header",
+    "decode_xor16",
+    "split_header",
+    "split_files",
+    "fopen_dav",
+    "DigiCap",
 ]
 
+import logging
+
 from io import IOBase
-from typing import Generator, Iterator, overload
+from typing import Generator, Iterator
 from struct import unpack
 
+from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
+
+logger = logging.getLogger("hiktools-logger")
+
+
 ###############################################################################
 # Exception Classes
 ###############################################################################
 class InvalidFileFormatException(Exception):
     """Base class for DAV file exceptions."""
 
 
 class FileAccessException(Exception):
     """Base class for permission related issues."""
 
+
 ###############################################################################
 # Data Types
 ###############################################################################
-BIG_ENDIAN = '>'
-LITTLE_ENDIAN = '<'
+BIG_ENDIAN = ">"
+LITTLE_ENDIAN = "<"
+
 
 def uint32(value: bytes, encoding: str = LITTLE_ENDIAN) -> int:
     """Unpacks an unsigned 32-bit integer from the given buffer.
 
     :param value: the input buffer
     :type value: bytes
     :param encoding: the encoding to use, defaults to LITTLE_ENDIAN
     :type encoding: int, optional
     :raises TypeError: if the buffer is not a bytes object
     :return: the unpacked unsigned 32-bit integer
     :rtype: int
     """
     if isinstance(value, (bytes, bytearray, tuple, list)):
-        result, = unpack(f"{encoding}I", value)
+        if len(value) < 4:
+            raise ValueError(
+                "Could not verify buffer length - expected at least 4 "
+                f"bytes, got {len(value)}"
+            )
+
+        (result,) = unpack(f"{encoding}I", bytearray(list(value)[:4]))
         return result
 
-    raise TypeError(f'Unexpected input type: {type(value)}')
+    raise TypeError(f"Unexpected input type: {type(value)}")
 
 
 def uint24(value: bytes, encoding: int = LITTLE_ENDIAN) -> int:
     """Unpacks an unsigned 24-bit integer from the given buffer.
 
     :param value: the input buffer
     :type value: bytes
@@ -85,41 +107,45 @@
     :raises ValueError: if an invalid encoding value is provided
     :raises TypeError: if the buffer is not a bytes object
     :return: the unpacked unsigned 24-bit integer
     :rtype: int
     """
     if isinstance(value, (bytes, bytearray, tuple, list)):
         if len(value) < 3:
-            raise ValueError(f'Invalid buffer length ({len(value)}), expected at least 4')
+            raise ValueError(
+                f"Invalid buffer length ({len(value)}), expected at least 4 "
+                "bytes to handle."
+            )
 
         if encoding == BIG_ENDIAN:
             return value[0] << 16 | value[1] << 8 | value[2]
         if encoding == LITTLE_ENDIAN:
             return value[0] | value[1] << 8 | value[2] << 16
 
-        raise ValueError('Unexpected Encoding!')
-    raise TypeError(f'unexpected input type: {type(value)}')
+        raise ValueError(
+            f"Unexpected Encoding, got {str(encoding)} ('<' or '>' accepted)"
+        )
+    raise TypeError(f"unexpected input type: {type(value)}")
 
 
-@overload
-def uint8(value: int) -> int: ...
-def uint8(value: bytes) -> int:
+def uint8(value: bytes | int) -> int:
     """Converts the input to an unsigned 8-bit integer
 
     :param value: the input buffer or int
     :type value: bytes
     :raises TypeError: if an invalid input is provided
     :return: the unsigned 8-bit integer
     :rtype: int
     """
     if isinstance(value, bytes):
         return int(value[0])
     if isinstance(value, int):
         return int(value & 0xFF)
-    raise TypeError(f'unexpected input type: {type(value)}')
+    raise TypeError(f"unexpected input type: {type(value)}")
+
 
 class DigiCapHeader:
     """A class covering important configuration information.
 
     :param magic: magic header bytes indicating the used firmware
     :type magic: int
 
@@ -144,78 +170,85 @@
     :param signature: unidentified
     :type signature: int
 
     :param features: unidentified
     :type features: int
 
     """
-    def __init__(self, magic: int = 0x00, header_checksum: int = 0x00,
-                 header_length: int = 0x00, files: int = 0x00,
-                 language: int = 0x00, device_class: int = 0x00,
-                 oem_code: int = 0x00, signature: int = 0x00,
-                 features: int = 0x00) -> None:
+
+    def __init__(
+        self,
+        magic: int = 0x00,
+        header_checksum: int = 0x00,
+        header_length: int = 0x00,
+        files: int = 0x00,
+        language: int = 0x00,
+        device_class: int = 0x00,
+        oem_code: int = 0x00,
+        signature: int = 0x00,
+        features: int = 0x00,
+    ) -> None:
         self.magic = magic
         self.header_checksum = header_checksum
         self.header_length = header_length
         self.files = files
         self.language = language
         self.device_class = device_class
         self.oem_code = oem_code
         self.signature = signature
         self.features = features
 
     def __repr__(self) -> str:
-        return f'<DigiCapHeader length={self.header_length}, files={self.files}>'
+        return f"<DigiCapHeader length={self.header_length}, files={self.files}>"
+
 
 ###############################################################################
 # Funtions
 ###############################################################################
-def fopen_dav(file_name: str, mode: str = 'rb') -> IOBase:
+def fopen_dav(file_name: str, mode: str = "rb") -> IOBase:
     """Opens a file with te 'dav' extension.
 
     :param file_name:  The absolute or relative path to the file
     :type file_name: str
     :param mode: The mode this file shoul be opened with (either 'r' or 'rb'), defaults to 'rb'
     :type mode: str, optional
 
     :raises InvalidFileFormatException: on invalid file extension
     :raises ValueError: on invalid argument values
     :raises FileAccessException:  if there are issues with open the file
 
     :return: A file reader instance.
     :rtype: IOBase
     """
-    if not file_name or not file_name.endswith('dav'):
-        raise InvalidFileFormatException('Expected a *.dav file on input.')
+    if not file_name or not file_name.endswith("dav"):
+        raise InvalidFileFormatException("Expected a *.dav file on input.")
 
-    if not mode or mode not in ['r', 'rb']:
-        raise ValueError('Expected a reading mode.')
+    if not mode or mode not in ["r", "rb"]:
+        raise ValueError("Expected a reading mode.")
 
     try:
-        res = open(file_name, mode)
+        res = open(file_name, mode)  # noqa
     except OSError as open_error:
         raise FileAccessException(open_error) from open_error
 
     if not res:
-        raise FileAccessException('Unable to open *.dav file')
+        raise FileAccessException("Unable to open *.dav file")
 
     return res
 
 
-@overload
-def read_raw_header(resource: str) -> bytes: ...
-def read_raw_header(resource: IOBase) -> bytes:
+def read_raw_header(resource: IOBase | str) -> bytes:
     """Reads the first 108 bytes from the resource stream."""
     if isinstance(resource, str):
-        resource = fopen_dav(resource, 'rb')
+        resource = fopen_dav(resource, "rb")
 
-    if not resource or resource.mode != 'rb':
-        raise ValueError('Expected a reading bytes mode resource.')
+    if not resource or resource.mode != "rb":
+        raise ValueError("Expected a reading bytes mode resource.")
 
-    buf_len = 0x6c # 108 bytes
+    buf_len = 0x6C  # 108 bytes
     try:
         buf = resource.read(buf_len)
     except OSError as error:
         raise FileAccessException(error) from error
 
     return buf
 
@@ -231,105 +264,110 @@
 
     return bytes(result)
 
 
 def split_header(buf: bytes) -> DigiCapHeader:
     """Extracts information from the decoded firmware header."""
     if not buf or len(buf) == 0:
-        raise ValueError('Invalid buf object len() == 0 or object is None.')
+        raise ValueError("Invalid buf object len() == 0 or object is None.")
 
     # REVISION: maybe add magic value check to validate the right firmware
     # file is going to be inspected.
-    magic = uint32(buf)
+    magic = uint32(buf[:4])  # 9 the buffer should have only four bytes
     header_checksum = uint32(buf[4:8])
     header_length = uint32(buf[8:12])
     files = uint32(buf[12:16])
     language = uint32(buf[16:20])
     device_class = uint32(buf[20:24])
     oem_code = uint32(buf[24:28])
     signature = uint32(buf[28:32])
     features = uint32(buf[32:36])
 
     checksum = uint8(buf[8]) + (uint24(buf[9:12]) * 0x100)
     if checksum != header_length:
         raise InvalidFileFormatException(
-            f'Invalid header size: expected {checksum}, got {header_length}')
+            f"Invalid header size: expected {checksum}, got {header_length}"
+        )
 
     return DigiCapHeader(
-        magic, header_checksum, header_length, files, language,
-        device_class, oem_code, signature, features
+        magic,
+        header_checksum,
+        header_length,
+        files,
+        language,
+        device_class,
+        oem_code,
+        signature,
+        features,
     )
 
 
-@overload
-def split_files(buf: IOBase, length: int = 0x0) -> Generator[tuple, None, None]: ...
-def split_files(buf: bytes, length: int = 0x40) -> Generator[tuple, None, None]:
+def split_files(
+    buf: bytes | IOBase, length: int = 0x40
+) -> Generator[tuple, None, None]:
     """Iterates over all files located in the given filesystem index
 
     :param buf: the input buffer or file pointer
     :type buf: bytes
     :param length: the amount of bytes to read, defaults to 0x40
     :type length: int, optional
     :raises ValueError: if the reading mode is not 'rb'
     :raises ValueError: if the amount of bytes to read is <= 0
     :yield: a tuple storing the file name, file position, and file checksum
     :rtype: Generator[tuple, None, None]
     """
     if isinstance(buf, IOBase):
-        if not buf or buf.mode != 'rb':
-            raise ValueError('Expected a reading bytes mode resource.')
+        if not buf or buf.mode != "rb":
+            raise ValueError("Expected a reading bytes mode resource.")
 
         if length <= 0:
-            raise ValueError('Expected a length > 0.')
+            raise ValueError("Expected a length > 0.")
 
         buf.seek(0, 0)
         buf = buf.read(length)
 
     index = 0x40
     amount = uint32(buf[12:16])
     for _ in range(amount):
-        file_name = buf[index:index+32].replace(b'\x00', b'')
+        file_name = buf[index : index + 32].replace(b"\x00", b"")
         index += 32
 
-        file_length = uint32(buf[index:index+4])
-        file_pos = uint32(buf[index+4:index+8])
-        file_checksum = uint32(buf[index+8:index+12])
+        file_length = uint32(buf[index : index + 4])
+        file_pos = uint32(buf[index + 4 : index + 8])
+        file_checksum = uint32(buf[index + 8 : index + 12])
         index += 12
-        yield file_name.decode('utf-8'), file_length, file_pos, file_checksum
+        yield file_name.decode("utf-8"), file_length, file_pos, file_checksum
 
 
 ###############################################################################
 # Classes
 ###############################################################################
 class DigiCap:
     """The base class for operating with digicap.dav files."""
 
-
-    KEY_XOR = b'\xBA\xCD\xBC\xFE\xD6\xCA\xDD\xD3\xBA\xB9\xA3\xAB\xBF\xCB\xB5\xBE'
+    KEY_XOR = b"\xBA\xCD\xBC\xFE\xD6\xCA\xDD\xD3\xBA\xB9\xA3\xAB\xBF\xCB\xB5\xBE"
     """The key used to encrypt/decrypt the firmware files."""
 
-    @overload
-    def __init__(self, resource: IOBase = None) -> None: ...
-    def __init__(self, resource: str = None) -> None:
+    def __init__(self, resource: str | IOBase = None) -> None:
         self._file = None
         self._name = None
         self._filelist = []
         self._len = 0
         self._head = None
 
         if resource is not None:
             if isinstance(resource, str):
                 if not self.fopen(resource):
-                    raise InvalidFileFormatException(f'Invalid input file: {resource}')
+                    raise InvalidFileFormatException(f"Invalid input file: {resource}")
 
             elif isinstance(resource, IOBase):
                 self._file = resource
                 self._name = resource.name
             else:
-                raise ValueError(f'Invalid argument type: {type(resource)}')
+                raise ValueError(f"Invalid argument type: {type(resource)}")
 
     def fopen(self, resource: str) -> bool:
         """Opens the given resource.
 
         Will be called automatically when this class is used in a with statement.
         """
         if resource is not None:
@@ -348,61 +386,60 @@
         """Sets the reader's position to the start of the stream."""
         self._file.seek(0, 0)
         return self._file.seekable()
 
     def fread(self, length: int, offset: int = -1) -> bytes:
         """Reads the given amount of bytes from the underlying stream."""
         if self._file.closed:
-            raise ValueError('FileInoutStream is closed!')
+            raise ValueError("FileInoutStream is closed!")
 
         if offset >= 0:
             self._file.seek(offset)
         return self._file.read(length)
 
     def fparse(self):
         """Parses the firmware file."""
         if self._file is not None:
             raw_head = read_raw_header(self._file)
-            decoded_head = decode_xor16(raw_head, self.KEY_XOR, 0x6c)
+            decoded_head = decode_xor16(raw_head, self.KEY_XOR, 0x6C)
 
             self._head = split_header(decoded_head)
             self.reset()
             raw_data = decode_xor16(
                 self._file.read(self.head.header_length),
                 self.KEY_XOR,
-                self.head.header_length
+                self.head.header_length,
             )
             self._filelist = list(split_files(raw_data))
+            if len(self) == 0:
+                logger.warning("Could not decode firmware - detected 0 files!")
         else:
-            raise ValueError('Input source is None.')
+            raise ValueError("Input source is None.")
 
     @property
     def name(self) -> str:
         """The file name (absolute or relative)"""
         return self._name
 
     @property
     def head(self) -> DigiCapHeader:
         """The header object storing important configuration data."""
         return self._head
 
-    def __enter__(self) -> 'DigiCap':
+    def __enter__(self) -> "DigiCap":
         self.fparse()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.fclose()
-        if exc_value is not None:
-            return False
 
     def __len__(self) -> int:
         return len(self._filelist) if not self._len else self._len
 
     def __iter__(self) -> Iterator[tuple]:
         return iter(self._filelist)
 
     def __getitem__(self, index: int) -> tuple:
         return self._filelist[index]
 
     def __repr__(self) -> str:
         return f'<DigiCap file="{self._name}">'
-
```

### Comparing `hiktools-1.2.1/hiktools/fmod/extractor.py` & `hiktools-1.2.2/hiktools/fmod/export.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,34 +15,33 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-__all__ = [
-  'export'
-]
+__all__ = ["export"]
 
-from os import mkdir
-from hiktools.fmod.decrypter import DigiCap, FileAccessException
+from pathlib import Path
+from hiktools.fmod.digicap import DigiCap, FileAccessException
 
 
 def export(dfile: DigiCap, location: str) -> bool:
     """Extracts all files stored in the given digicap file."""
     if location is None or dfile is None:
-        raise ValueError('Input file or location is null')
+        raise ValueError("Input file or location is null")
 
+    path = Path(location)
     try:
-        mkdir(location)
+        path.mkdir(exist_ok=True)
     except OSError as error:
         raise FileAccessException(error) from error
 
-    location = location.strip('/')
     for fname, flen, fpos, _ in dfile:
         try:
-            with open('/'.join([location, fname]), 'wb') as exp_file:
+            with open(str(path / fname), "wb") as exp_file:
                 exp_file.write(dfile.fread(flen, fpos))
-            return True
-        except OSError:
-            pass
-    return False
+        except OSError as err:
+            print(str(err))
+            return False
+
+    return True
```

### Comparing `hiktools-1.2.1/hiktools/sadp/__init__.py` & `hiktools-1.2.2/hiktools/sadp/__init__.py`

 * *Files identical despite different names*

### Comparing `hiktools-1.2.1/hiktools/sadp/client.py` & `hiktools-1.2.2/hiktools/sadp/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,39 +19,38 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """
 UDP-Client implementation to communicate with Hikvision cameras.
 """
 
-__all__ = [
-  'SADPClient', 'hik_code'
-]
+__all__ = ["SADPClient", "hik_code"]
 
 import socket
 
 from hiktools.sadp.message import SADPMessage
 
 
 class SADPClient:
     """A simple UDP wrapper client.
 
     This clas implements basic funtionalities of an UDP socket sending data
     from UDP broadcast. The with directive can be used and __iter__ is also
     implemented in order to iterate over reveiced SADPMessages.
     """
+
     def __init__(self, port: int = 37020, timeout: int = 2) -> None:
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
         self._sock.settimeout(timeout)
-        self._address = ('239.255.255.250', port)
+        self._address = ("239.255.255.250", port)
         self.buf_size = 2048
 
-    def __enter__(self) -> 'SADPClient':
+    def __enter__(self) -> "SADPClient":
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
     def close(self):
         """Closes the underlying socket."""
@@ -73,14 +72,15 @@
         try:
             while True:
                 data = self.recv_next(self.buf_size)
                 yield SADPMessage(response=data)
         except socket.timeout:
             pass
 
+
 def hik_code(serial: str, timestamp: tuple) -> str:
     """Generates the old Hikvision reset code.
 
     Arguments:
     :param serial: The device's serial number.
     :type serial: str
     :param timestamp: A timestamp of the following format: (day, month, year)
@@ -95,16 +95,21 @@
     month = int(timestamp[1])
     year = int(timestamp[2])
 
     composed = serial + year + month + day
     for i, val in enumerate(composed):
         magic += (ord(val) * (i + 1)) ^ (i + 1)
 
-    magic = str((magic * 0x686b7773) & 0xFFFFFFFF)
+    magic = str((magic * 0x686B7773) & 0xFFFFFFFF)
     for i, c0 in enumerate(magic):
-        if c0 < 51: result += chr(c0 + 33)
-        elif c0 < 53: result += chr(c0 + 62)
-        elif c0 < 55: result += chr(c0 + 47)
-        elif c0 < 57: result += chr(c0 + 66)
-        else: result += chr(c0)
+        if c0 < 51:
+            result += chr(c0 + 33)
+        elif c0 < 53:
+            result += chr(c0 + 62)
+        elif c0 < 55:
+            result += chr(c0 + 47)
+        elif c0 < 57:
+            result += chr(c0 + 66)
+        else:
+            result += chr(c0)
 
     return result
```

### Comparing `hiktools-1.2.1/hiktools/sadp/message.py` & `hiktools-1.2.2/hiktools/sadp/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,64 +20,74 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """
 Small module that contains message declarations for UDP communication.
 """
 
 __all__ = [
-  'SADPMessage', 'fromdict', 'BasicDictObject',
-  'DiscoveryPacket', 'SafeCode', 'DeviceSafeCodePacket',
-  'unmarshal', 'ActionResponse'
+    "SADPMessage",
+    "fromdict",
+    "BasicDictObject",
+    "DiscoveryPacket",
+    "SafeCode",
+    "DeviceSafeCodePacket",
+    "unmarshal",
+    "ActionResponse",
 ]
 
 import xml.etree.ElementTree as xmltree
 import ctypes
 import base64
 
 from typing import Iterator, overload
 
 __types__ = {}
 """A dict object storing all defined message types.
 """
 
+
 def message_type(name: str):
     """Registers a new message type.
 
     :param name: the name of the type to register
     :type name: str
     """
+
     def wrapper(clazz):
         if name not in __types__:
             __types__[name] = clazz
         return clazz
+
     return wrapper
 
 
 class SADPMessage:
     """A simple exchange class.
 
     For exchanging data between the client and the device this object wrapper
     is used. It stores the message string which is sent over broadcast to the
     device and the response as bytes.
 
     :param response: A response buffer storing the received bytes.
     :type response: bytes
     """
-    def __init__(self, message: str = None, response=None,
-                sender: tuple = None) -> None:
+
+    def __init__(
+        self, message: str = None, response=None, sender: tuple = None
+    ) -> None:
         self._message = message
         self._response = response
         self._sender = (None, 0) if not sender else sender
 
     def toxml(self) -> xmltree.Element:
         """Transforms the received bytes into an XML element."""
         if self._response is not None:
             return xmltree.fromstring(self._response)
         else:
-            raise ValueError('Response value is null')
+            raise ValueError("Response value is null")
 
     def set_response(self, response: bytes):
         """The message's response setter.
 
         :param response: the raw response onbject
         :type response: bytes
         """
@@ -96,15 +106,15 @@
 
     @property
     def sender(self) -> tuple:
         """The sender ip address and port. (DO NOT USE)"""
         return self._sender
 
     def __bytes__(self) -> bytes:
-        return self.message.encode('utf-8')
+        return self.message.encode("utf-8")
 
     def __repr__(self) -> str:
         return self.message
 
     def __str__(self) -> str:
         return self.message
 
@@ -115,20 +125,22 @@
     :param value: The input dict containing the XML nodes.
     :type value: dict
 
     :returns: An message object containing all nodes of the given
                 dict object converted into an XML string.
     :rtype: SADPMessage
     """
-    root = xmltree.Element('Probe')
+    root = xmltree.Element("Probe")
     for key in value:
         elem = xmltree.Element(key)
         elem.text = value[key]
         root.append(elem)
-    return SADPMessage(message=xmltree.tostring(root, xml_declaration=True).decode('utf-8'))
+    return SADPMessage(
+        message=xmltree.tostring(root, xml_declaration=True).decode("utf-8")
+    )
 
 
 def pack(buffer: bytes, fmt: type, index=0) -> int:
     """Puts the bytes in the given buffer into one integer.
 
     :param buffer: the input buffer
     :type buffer: bytes
@@ -136,19 +148,25 @@
     :type fmt: type
     :param index: the current buffer position, defaults to 0
     :type index: int, optional
     :return: the packed integer variable
     :rtype: int
     """
     if fmt == ctypes.c_uint32:
-        return pack(buffer, ctypes.c_uint16, index) | pack(buffer, ctypes.c_uint16, index+2) << 16
+        return (
+            pack(buffer, ctypes.c_uint16, index)
+            | pack(buffer, ctypes.c_uint16, index + 2) << 16
+        )
     if fmt == ctypes.c_uint8:
         return fmt(buffer[index])
     if fmt == ctypes.c_uint16:
-        return pack(buffer, ctypes.c_uint8, index) | pack(buffer, ctypes.c_uint8, index+1) << 8
+        return (
+            pack(buffer, ctypes.c_uint8, index)
+            | pack(buffer, ctypes.c_uint8, index + 1) << 8
+        )
     raise TypeError(f'Invalid type "{str(fmt)}" - not implemented!')
 
 
 class BasicDictObject:
     """The base class for response objects.
 
     A small wrapper class implementing basic dict behaviour.
@@ -178,25 +196,25 @@
     def __contains__(self, item):
         return str(item) in self._capabilities
 
     def __iter__(self) -> Iterator[str]:
         return iter(self._capabilities)
 
     def __str__(self) -> str:
-        text = [f'<{self.__class__.__name__}>']
+        text = [f"<{self.__class__.__name__}>"]
         for cap_name in self:
-            text.append(f'\t<{cap_name}>{self[cap_name]}</{cap_name}>')
-            text.append(f'</{self.__class__.__name__}>')
-        return '\n'.join(text)
+            text.append(f"\t<{cap_name}>{self[cap_name]}</{cap_name}>")
+            text.append(f"</{self.__class__.__name__}>")
+        return "\n".join(text)
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__} object>'
+        return f"<{self.__class__.__name__} object>"
 
 
-@message_type('inquiry')
+@message_type("inquiry")
 class DiscoveryPacket(BasicDictObject):
     """A simple discovery packet response wrapper.
 
     Contains all information related to the inquiry response packet. Possible
     nodes are:
 
     `DeviceType`, `DeviceDescription`, `CommandPort`, `HttpPort`, `MAC`, `Ipv4Address`,
@@ -209,30 +227,34 @@
 class SafeCode:
     """The device's safe code wrapper class.
 
     A safe code is requested by the SADP Tool to export it and send it to the
     customer service. An unlock code should be returned which can reset the device.
     """
 
-    SAFECODE_FLAG = '03000000'
+    SAFECODE_FLAG = "03000000"
     """Safe code header value"""
 
     @overload
-    def __init__(self, code: bytes) -> None: ...
+    def __init__(self, code: bytes) -> None:
+        ...
+
     def __init__(self, code: str) -> None:
         if not code:
-            raise ValueError('Code argument has to be non null!')
+            raise ValueError("Code argument has to be non null!")
 
-        self._b64_encoded = code.encode('utf-8') if isinstance(code, str) else code
+        self._b64_encoded = code.encode("utf-8") if isinstance(code, str) else code
         self._b64_decoded = base64.decodebytes(self._b64_encoded)
 
         if self._b64_decoded[:4].hex() != self.SAFECODE_FLAG:
-            raise ValueError('Invalid SafeCode: expected %#x as flag' % self.SAFECODE_FLAG)
+            raise ValueError(
+                "Invalid SafeCode: expected %#x as flag" % self.SAFECODE_FLAG
+            )
 
-        self._code = str(self._b64_decoded[4:-4], 'utf-8')
+        self._code = str(self._b64_decoded[4:-4], "utf-8")
         self._cksum = pack(self._b64_decoded[:-4], ctypes.c_uint32)
 
     @property
     def checksum(self) -> ctypes.c_uint32:
         """The checksum stored in the safe code."""
         return self._cksum
 
@@ -241,66 +263,66 @@
         """The full safe code as a string"""
         return self._code
 
     def __repr__(self) -> str:
         return self.code
 
 
-@message_type('getcode')
+@message_type("getcode")
 class DeviceSafeCodePacket(BasicDictObject):
     """A response packet for the 'getcode' message.
 
     This class can contain the following nodes:
 
     `MAC`, `Uuid`, `Code`, `Types`
     """
 
     @property
     def code(self) -> str:
         """The base64 safecode string."""
-        return self['Code']
+        return self["Code"]
 
     def get_safecode(self) -> SafeCode:
         """Returns the converted safecode as a SafeCode object."""
         return SafeCode(self.code)
 
 
-@message_type('reset')
+@message_type("reset")
 class ActionResponse(BasicDictObject):
     """A 'reset' message response packet.
 
     The response packet just contains one field of interest named 'Result'. It
     applies to the following values: failure, success, denied
     """
 
     def __init__(self, root: xmltree.Element = None) -> None:
         super().__init__(root)
 
     @property
     def success(self) -> bool:
         """Returns whether the action invocation was successful."""
-        return self['Result'] == 'success'
+        return self["Result"] == "success"
 
 
 def unmarshal(root: xmltree.Element):
     """Tries to de-serialize an XML-String.
-    
+
     Possible object types are: DiscoveryPacket, DeviceSafeCodePacket, ActionResponse,
     and BasicDictObject for messages that are not implemented yet.
 
     :param root:  The XML root element (non null).
     :type root: xmltree.Element
     :return: A qualified object instance or None if the given argument was None or
              the input could not be converted.
     :rtype: ? extends BasicDictObject, None
     """
     if root is None:
-        raise ValueError('Input argument is null')
+        raise ValueError("Input argument is null")
 
-    req_type = root.find('Types')
+    req_type = root.find("Types")
     if req_type is None:
         return None
 
     for type_name, cls in __types__.items():
         if type_name == req_type.text.lower():
             return cls(root=root)
     return BasicDictObject(root=root)
```

### Comparing `hiktools-1.2.1/hiktools.egg-info/PKG-INFO` & `hiktools-1.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiktools
-Version: 1.2.1
+Version: 1.2.2
 Summary: Hikvision utility tools
 Author-email: MatrixEditor <not@supported.com>
 Project-URL: Homepage, https://github.com/MatrixEditor/hiktools
 Project-URL: API-Docs, https://hiktools.readthedocs.io
 Project-URL: Native-API-Docs, https://matrixeditor.github.io/hiktools/docs/html/d3/dcc/md__r_e_a_d_m_e.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -18,33 +18,62 @@
 License-File: LICENSE
 
 # Hiktools
 
 ![Module](https://img.shields.io:/static/v1?label=Module&message=hiktools&color=9cf)
 ![Build](https://img.shields.io:/static/v1?label=Python&message=>=3.5&color=green)
 ![Platform](https://img.shields.io:/static/v1?label=Platforms&message=Linux|Windows&color=yellowgreen)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.2.1&color=green)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.2.2&color=green)
 
-This is now a small project with four main functionalities: 
 
+This respository was former known as `hikvision-sdk-cam`, but has changed since the old content of this repository was deleted. This is now a small project with four main functionalities:
 * A Wireshark dissector for the Search Active Devices Protocol,
-* Decrypt and extract hikvision firmware, 
-* Send raw SADP packets (only Linux) and 
-* Send commands via UDP Broadcast. 
+* Decrypt and extract hikvision firmware,
+* Send raw SADP packets (only Linux) and
+* Send commands via UDP Broadcast.
 
-To get familiar with the API provided in this repository, take a quick look at the python documentation available **[here »](https://hiktools.readthedocs.io/)** or the 
+To get familiar with the API provided in this repository, take a quick look at the python documentation available **[here »](https://hiktools.readthedocs.io/)** or the
 C++ documentation available at Github-Pages **[here »](https://matrixeditor.github.io/hiktools/docs/html/d3/dcc/md__r_e_a_d_m_e.html)**.
 
+### Installation
+
+You can now install the `hiktools` module with pip:
+
+```bash
+$ python3 -m pip install hiktools
+```
+
 ### Overview
 ---
 **Update:** Since feature version `1.1.0` the native packet creation and communication works! It is still only usable on UNIX systems that support sending raw ethernet frames. The checksum algorithm was disassebled and decompiled correctly, just the input parameters were interpreted wrong. The algorithm is implemented in [C/C++](/cpp/checksum.h) and [python3](/hiktools/csadp/checksum.py).
 
-Communication on UDP works fine at the moment - this API is just a small wrapper which can be used for a more general API. 
+Communication on UDP works fine at the moment - this API is just a small wrapper which can be used for a more general API.
+
+Firmware decryption and extraction will only work on newer `digicap.dav` files with at least  `1` file entry (otherwise there will be no files to inspect) in the header. All firmware files and updates can be downloaded from the following endpoint (EU):
+
+* https://www.hikvisioneurope.com/uk/portal
 
-Firmware decryption and extraction will only work on newer `digicap.dav` files with at least one file entry (otherwise there will be no files to inspect) in the header. All firmware files and updates can be downloaded from the following endpoint (EU):
+There is also a full list of files available at this enpoint stored in a JSON file named [firmwarelist.json](/gists/firmwarelist.json).
+
+> Info: There is an interesting file located in the extracted files of a firmware image: /hroot.img/initrd/etc/passwd. A password is set to the root user:
+
+    Name: passwd
+    Folder: -
+    Size: 44
+    Packed Size: 1 024
+    Mode: -rwxrwxr-x
+    Last change: 2016-12-23 08:27:46
+    Last modification: 2016-12-23 08:27:46
+    -------------------------------------------
+
+    root:ToCOv8qxP13qs:0:0:root:/root/:/bin/psh
+
+The plain password is `hiklinux`, kudos to [Don Bowman](https://blog.donbowman.ca/2018/01/18/hacking-the-hikvision-part-1/).
+
+> Old exploit with authkey := YWRtaW46MTEK
 
 ### Basic Usage
 ---
 
 - Firmware inspection and extraction
 
 ```python
@@ -69,15 +98,15 @@
 python3 -m hiktools.fmod input.dav outputDir
 ```
 
 - Native interface on sending raw packets (only LINUX)
 ```python
 from hiktools import csadp
 
-# Because the following module requires root priviledges it 
+# Because the following module requires root priviledges it
 # has to be imported directly.
 from hiktools.csadp import CService
 
 sock = CService.l2socket('wlan0')
 counter = 0x115e
 
 # To build an Inquiry packet, we need the following information:
@@ -115,12 +144,12 @@
   for response in client:
     if response is None: break
     # initiate the response
     message = sadp.unmarshal(response.toxml())
 
     # message objects contain a dict-like implementation
     for property_name in message:
-      print(message[property_name]) 
-    
+      print(message[property_name])
+
     # e.g.
     print('Device at', message['IPv4Address'])
 ```
```

### Comparing `hiktools-1.2.1/hiktools.egg-info/SOURCES.txt` & `hiktools-1.2.2/hiktools.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 hiktools/csadp/__init__.py
 hiktools/csadp/checksum.py
 hiktools/csadp/model.py
 hiktools/csadp/payloads.py
 hiktools/csadp/uarray.py
 hiktools/fmod/__init__.py
 hiktools/fmod/__main__.py
-hiktools/fmod/decrypter.py
-hiktools/fmod/extractor.py
+hiktools/fmod/digicap.py
+hiktools/fmod/export.py
 hiktools/sadp/__init__.py
 hiktools/sadp/client.py
 hiktools/sadp/message.py
```

### Comparing `hiktools-1.2.1/pyproject.toml` & `hiktools-1.2.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2268 696b 746f 6f6c 7322 0d0a 7665  = "hiktools"..ve
-00000020: 7273 696f 6e20 3d20 2231 2e32 2e31 220d  rsion = "1.2.1".
+00000020: 7273 696f 6e20 3d20 2231 2e32 2e32 220d  rsion = "1.2.2".
 00000030: 0a64 6573 6372 6970 7469 6f6e 3d22 4869  .description="Hi
 00000040: 6b76 6973 696f 6e20 7574 696c 6974 7920  kvision utility 
 00000050: 746f 6f6c 7322 0d0a 6175 7468 6f72 7320  tools"..authors 
 00000060: 3d20 5b0d 0a20 207b 206e 616d 653d 224d  = [..  { name="M
 00000070: 6174 7269 7845 6469 746f 7222 2c20 656d  atrixEditor", em
 00000080: 6169 6c3d 226e 6f74 4073 7570 706f 7274  ail="not@support
 00000090: 6564 2e63 6f6d 2220 7d2c 0d0a 5d0d 0a72  ed.com" },..]..r
@@ -15,41 +15,41 @@
 000000e0: 2035 202d 2050 726f 6475 6374 696f 6e2f   5 - Production/
 000000f0: 5374 6162 6c65 272c 0d0a 2020 2020 2749  Stable',..    'I
 00000100: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
 00000110: 203a 3a20 5363 6965 6e63 652f 5265 7365   :: Science/Rese
 00000120: 6172 6368 272c 0d0a 2020 2020 274c 6963  arch',..    'Lic
 00000130: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
 00000140: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-00000150: 6e73 6527 2c20 200d 0a20 2020 2027 5072  nse',  ..    'Pr
-00000160: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000170: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000180: 332e 3627 2c0d 0a20 2020 2027 5072 6f67  3.6',..    'Prog
-00000190: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000001a0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000001b0: 3727 2c0d 0a20 2020 2027 5072 6f67 7261  7',..    'Progra
-000001c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001d0: 3a20 5079 7468 6f6e 203a 3a20 332e 3827  : Python :: 3.8'
-000001e0: 2c0d 0a20 2020 2027 5072 6f67 7261 6d6d  ,..    'Programm
-000001f0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000200: 5079 7468 6f6e 203a 3a20 332e 3927 2c0d  Python :: 3.9',.
-00000210: 0a20 2020 2027 5072 6f67 7261 6d6d 696e  .    'Programmin
-00000220: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000230: 7468 6f6e 203a 3a20 332e 3130 272c 0d0a  thon :: 3.10',..
-00000240: 2020 5d0d 0a0d 0a5b 7072 6f6a 6563 742e    ]....[project.
-00000250: 7572 6c73 5d0d 0a22 486f 6d65 7061 6765  urls].."Homepage
-00000260: 2220 3d20 2268 7474 7073 3a2f 2f67 6974  " = "https://git
-00000270: 6875 622e 636f 6d2f 4d61 7472 6978 4564  hub.com/MatrixEd
-00000280: 6974 6f72 2f68 696b 746f 6f6c 7322 0d0a  itor/hiktools"..
-00000290: 2241 5049 2d44 6f63 7322 203d 2022 6874  "API-Docs" = "ht
-000002a0: 7470 733a 2f2f 6869 6b74 6f6f 6c73 2e72  tps://hiktools.r
-000002b0: 6561 6474 6865 646f 6373 2e69 6f22 0d0a  eadthedocs.io"..
-000002c0: 224e 6174 6976 652d 4150 492d 446f 6373  "Native-API-Docs
-000002d0: 2220 3d20 2268 7474 7073 3a2f 2f6d 6174  " = "https://mat
-000002e0: 7269 7865 6469 746f 722e 6769 7468 7562  rixeditor.github
-000002f0: 2e69 6f2f 6869 6b74 6f6f 6c73 2f64 6f63  .io/hiktools/doc
-00000300: 732f 6874 6d6c 2f64 332f 6463 632f 6d64  s/html/d3/dcc/md
-00000310: 5f5f 725f 655f 615f 645f 6d5f 652e 6874  __r_e_a_d_m_e.ht
-00000320: 6d6c 220d 0a0d 0a5b 746f 6f6c 2e73 6574  ml"....[tool.set
-00000330: 7570 746f 6f6c 732e 7061 636b 6167 6573  uptools.packages
-00000340: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-00000350: 5b22 2e22 5d0d 0a69 6e63 6c75 6465 203d  ["."]..include =
-00000360: 205b 2268 696b 746f 6f6c 732a 225d        ["hiktools*"]
+00000150: 6e73 6527 2c0d 0a20 2020 2027 5072 6f67  nse',..    'Prog
+00000160: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000170: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000180: 3627 2c0d 0a20 2020 2027 5072 6f67 7261  6',..    'Progra
+00000190: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000001a0: 3a20 5079 7468 6f6e 203a 3a20 332e 3727  : Python :: 3.7'
+000001b0: 2c0d 0a20 2020 2027 5072 6f67 7261 6d6d  ,..    'Programm
+000001c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000001d0: 5079 7468 6f6e 203a 3a20 332e 3827 2c0d  Python :: 3.8',.
+000001e0: 0a20 2020 2027 5072 6f67 7261 6d6d 696e  .    'Programmin
+000001f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000200: 7468 6f6e 203a 3a20 332e 3927 2c0d 0a20  thon :: 3.9',.. 
+00000210: 2020 2027 5072 6f67 7261 6d6d 696e 6720     'Programming 
+00000220: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000230: 6f6e 203a 3a20 332e 3130 272c 0d0a 2020  on :: 3.10',..  
+00000240: 5d0d 0a0d 0a5b 7072 6f6a 6563 742e 7572  ]....[project.ur
+00000250: 6c73 5d0d 0a22 486f 6d65 7061 6765 2220  ls].."Homepage" 
+00000260: 3d20 2268 7474 7073 3a2f 2f67 6974 6875  = "https://githu
+00000270: 622e 636f 6d2f 4d61 7472 6978 4564 6974  b.com/MatrixEdit
+00000280: 6f72 2f68 696b 746f 6f6c 7322 0d0a 2241  or/hiktools".."A
+00000290: 5049 2d44 6f63 7322 203d 2022 6874 7470  PI-Docs" = "http
+000002a0: 733a 2f2f 6869 6b74 6f6f 6c73 2e72 6561  s://hiktools.rea
+000002b0: 6474 6865 646f 6373 2e69 6f22 0d0a 224e  dthedocs.io".."N
+000002c0: 6174 6976 652d 4150 492d 446f 6373 2220  ative-API-Docs" 
+000002d0: 3d20 2268 7474 7073 3a2f 2f6d 6174 7269  = "https://matri
+000002e0: 7865 6469 746f 722e 6769 7468 7562 2e69  xeditor.github.i
+000002f0: 6f2f 6869 6b74 6f6f 6c73 2f64 6f63 732f  o/hiktools/docs/
+00000300: 6874 6d6c 2f64 332f 6463 632f 6d64 5f5f  html/d3/dcc/md__
+00000310: 725f 655f 615f 645f 6d5f 652e 6874 6d6c  r_e_a_d_m_e.html
+00000320: 220d 0a0d 0a5b 746f 6f6c 2e73 6574 7570  "....[tool.setup
+00000330: 746f 6f6c 732e 7061 636b 6167 6573 2e66  tools.packages.f
+00000340: 696e 645d 0d0a 7768 6572 6520 3d20 5b22  ind]..where = ["
+00000350: 2e22 5d0d 0a69 6e63 6c75 6465 203d 205b  ."]..include = [
+00000360: 2268 696b 746f 6f6c 732a 225d            "hiktools*"]
```

