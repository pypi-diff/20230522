# Comparing `tmp/esp-coredump-1.5.0.tar.gz` & `tmp/esp-coredump-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/esp-coredump-1.5.0.tar", last modified: Fri Mar 31 09:02:36 2023, max compression
+gzip compressed data, was "dist/esp-coredump-1.5.1.tar", last modified: Mon May 22 10:43:22 2023, max compression
```

## Comparing `esp-coredump-1.5.0.tar` & `esp-coredump-1.5.1.tar`

### file list

```diff
@@ -1,38 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:02:36.000000 esp-coredump-1.5.0/
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2471 2023-03-31 09:02:36.000000 esp-coredump-1.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:02:36.000000 esp-coredump-1.5.0/esp_coredump/
--rw-rw-rw-   0 root         (0) root         (0)      593 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3181 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/cli_ext.py
--rwxrwxrwx   0 root         (0) root         (0)    19008 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/coredump.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:02:36.000000 esp-coredump-1.5.0/esp_coredump/corefile/
--rw-rw-rw-   0 root         (0) root         (0)     3916 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/corefile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2014 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/corefile/_parse_soc_header.py
--rw-rw-rw-   0 root         (0) root         (0)    11656 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/corefile/elf.py
--rw-rw-rw-   0 root         (0) root         (0)     5234 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/corefile/gdb.py
--rw-rw-rw-   0 root         (0) root         (0)    25410 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/corefile/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1809 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/corefile/riscv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:02:36.000000 esp-coredump-1.5.0/esp_coredump/corefile/soc_headers/
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/corefile/soc_headers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/corefile/soc_headers/esp32.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/corefile/soc_headers/esp32c2.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/corefile/soc_headers/esp32c3.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/corefile/soc_headers/esp32c6.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/corefile/soc_headers/esp32h2.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/corefile/soc_headers/esp32s2.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/corefile/soc_headers/esp32s3.py
--rw-rw-rw-   0 root         (0) root         (0)    11172 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/corefile/xtensa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:02:36.000000 esp-coredump-1.5.0/esp_coredump/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1442 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/esp_coredump/scripts/espcoredump.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:02:36.000000 esp-coredump-1.5.0/esp_coredump.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2471 2023-03-31 09:02:36.000000 esp-coredump-1.5.0/esp_coredump.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      988 2023-03-31 09:02:36.000000 esp-coredump-1.5.0/esp_coredump.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 09:02:36.000000 esp-coredump-1.5.0/esp_coredump.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-03-31 09:02:36.000000 esp-coredump-1.5.0/esp_coredump.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-03-31 09:02:36.000000 esp-coredump-1.5.0/esp_coredump.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-31 09:02:36.000000 esp-coredump-1.5.0/esp_coredump.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 09:02:36.000000 esp-coredump-1.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2276 2023-03-31 09:02:26.000000 esp-coredump-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump/
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/cli_ext.py
+-rwxrwxrwx   0 root         (0) root         (0)    21962 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/coredump.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump/corefile/
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2019 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/_parse_soc_header.py
+-rw-rw-rw-   0 root         (0) root         (0)    12070 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/elf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5300 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/gdb.py
+-rw-rw-rw-   0 root         (0) root         (0)    28157 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/riscv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/esp32.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/esp32c2.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/esp32c3.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/esp32c6.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/esp32h2.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/esp32s2.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/esp32s3.py
+-rw-rw-rw-   0 root         (0) root         (0)    11177 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/xtensa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/scripts/espcoredump.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/scripts/run_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      290 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4334 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/tests/test_espcoredump.py
```

### Comparing `esp-coredump-1.5.0/LICENSE` & `esp-coredump-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.0/PKG-INFO` & `esp-coredump-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-coredump
-Version: 1.5.0
+Version: 1.5.1
 Summary: Generate core dumps on unrecoverable software errors
 Home-page: https://github.com/espressif/esp-idf
 Author: Espressif Systems
 Author-email: aleksei.apaseev@espressif.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `esp-coredump-1.5.0/README.md` & `esp-coredump-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.0/esp_coredump/__init__.py` & `esp-coredump-1.5.1/esp_coredump/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
 import os
 import sys
 
@@ -18,8 +18,8 @@
 
 from .coredump import CoreDump
 
 __all__ = [
     'CoreDump',
 ]
 
-__version__ = '1.5.0'
+__version__ = '1.5.1'
```

### Comparing `esp-coredump-1.5.0/esp_coredump/cli_ext.py` & `esp-coredump-1.5.1/esp_coredump/cli_ext.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
 import argparse
 import os
 
-from pygdbmi.gdbcontroller import DEFAULT_GDB_TIMEOUT_SEC
-
 from esp_coredump import __version__
 
 from .corefile import SUPPORTED_TARGETS
+from .corefile.gdb import DEFAULT_GDB_TIMEOUT_SEC
 
 try:
     # esptool>=4.0
     from esptool.loader import ESPLoader
 except (AttributeError, ModuleNotFoundError):
     # esptool<4.0
     from esptool import ESPLoader
 
 parser = argparse.ArgumentParser(description='espcoredump.py v%s - ESP32 Core Dump Utility' % __version__)
 parser.add_argument('--chip', default=os.environ.get('ESPTOOL_CHIP', 'auto'),
                     choices=['auto'] + SUPPORTED_TARGETS,
                     help='Target chip type')
+parser.add_argument('--chip-rev', type=int,
+                    help='Target chip revision')
 parser.add_argument('--port', '-p', default=os.environ.get('ESPTOOL_PORT', ESPLoader.DEFAULT_PORT),
                     help='Serial port device')
 parser.add_argument('--baud', '-b', type=int,
                     default=os.environ.get('ESPTOOL_BAUD', ESPLoader.ESP_ROM_BAUD),
                     help='Serial port baud rate used when flashing/reading')
 parser.add_argument('--gdb-timeout-sec', type=int, default=DEFAULT_GDB_TIMEOUT_SEC,
                     help='Overwrite the default internal delay for gdb responses')
```

### Comparing `esp-coredump-1.5.0/esp_coredump/coredump.py` & `esp-coredump-1.5.1/esp_coredump/coredump.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 #!/usr/bin/env python
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # ESP-IDF Core Dump Utility
 #
 import os
 import subprocess
 import sys
 import textwrap
 from contextlib import contextmanager
 from distutils.spawn import find_executable
 from shutil import copyfile
-from typing import List, Optional, Tuple, Union
+from typing import Optional, Tuple, Union
 
 import serial
 
+from .tools import load_json_from_file
+
 try:
     # esptool>=4.0
     from esptool.cmds import detect_chip
     from esptool.loader import ESPLoader
 except (AttributeError, ModuleNotFoundError):
     # esptool<4.0
     from esptool import ESPLoader
     detect_chip = ESPLoader.detect_chip
 
 from construct import Container, GreedyRange, Int32ul, ListContainer, Struct
-from pygdbmi.gdbcontroller import DEFAULT_GDB_TIMEOUT_SEC
 
 from .corefile import RISCV_TARGETS, SUPPORTED_TARGETS, XTENSA_TARGETS, xtensa
 from .corefile.elf import (TASK_STATUS_CORRECT, ElfFile, ElfSegment,
                            ESPCoreDumpElfFile, EspTaskStatus)
-from .corefile.gdb import EspGDB
+from .corefile.gdb import DEFAULT_GDB_TIMEOUT_SEC, EspGDB
 from .corefile.loader import (ESPCoreDumpFileLoader, ESPCoreDumpFlashLoader,
                               ESPCoreDumpLoaderError, EspCoreDumpVersion)
 
-IDF_PATH = os.getenv('IDF_PATH')
+IDF_PATH = os.getenv('IDF_PATH', '')
+ESP_ROM_ELF_DIR = os.getenv('ESP_ROM_ELF_DIR')
+ROMS_JSON = os.path.join(IDF_PATH, 'tools', 'idf_py_actions', 'roms.json')  # type: ignore
 
 MORE_INFO_MSG = 'Read more: https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html'
 GDB_NOT_FOUND_ERROR = (
     f'GDB executable not found. Please install GDB or set up ESP-IDF to complete the action. '
     f'{MORE_INFO_MSG}'
 )
 IDF_SETUP_ERROR = f'Please set up ESP-IDF to complete the action. {MORE_INFO_MSG}'
@@ -56,28 +59,30 @@
     def __init__(self,
                  baud: Optional[int] = int(os.environ.get('ESPTOOL_BAUD', ESPLoader.ESP_ROM_BAUD)),
                  chip: str = os.environ.get('ESPTOOL_CHIP', 'auto'),
                  core_format: str = 'elf',
                  port: str = os.environ.get('ESPTOOL_PORT', ESPLoader.DEFAULT_PORT),
                  gdb_timeout_sec: int = DEFAULT_GDB_TIMEOUT_SEC,
                  core: Optional[str] = None,
+                 chip_rev: Optional[int] = None,
                  gdb: Optional[str] = None,
                  extra_gdbinit_file: Optional[str] = None,
                  off: Optional[int] = None,
                  prog: Optional[str] = None,
                  print_mem: Optional[str] = None,
                  rom_elf: Optional[str] = None,
                  save_core: Optional[str] = None,
                  ):
         if prog is None:
             raise ValueError("Path to program\'s ELF binary is not provided")
 
         self.baud = baud
         self.chip = chip
         self.core = core
+        self.chip_rev = chip_rev
         self.core_format = core_format
         self.gdb = gdb
         self.gdb_timeout_sec = gdb_timeout_sec
         self.extra_gdbinit_file = extra_gdbinit_file
         self.off = off
         self.prog = prog
         self.port = port
@@ -94,56 +99,79 @@
         if os.path.exists(elf_path):
             elf = ElfFile(elf_path)
             for s in elf.sections:
                 if s.name == '.text':
                     sym_cmd = 'add-symbol-file %s 0x%x' % (elf_path, s.addr)
         return sym_cmd
 
-    def get_core_dump_elf(self, e_machine=ESPCoreDumpFileLoader.ESP32):
-        # type: (Optional[int]) -> Tuple[str, Optional[str], Optional[list[str]]]
+    def extract_chip_rev_from_elf(self):
+        if not os.path.exists(self.core):
+            raise FileNotFoundError(f"Provided ELF file {self.core} is not found or doesn't exist")
+        elf = ElfFile(elf_path=self.core)
+        chip_rev = None
+        for s in elf.note_segments:
+            for n in s.note_secs:
+                if b'ESP_CHIP_REV' in n.name:
+                    chip_rev = int.from_bytes(n.desc, 'little')
+                    break
+
+        return chip_rev
+
+    def get_core_header_info_dict(self, e_machine=ESPCoreDumpElfFile.EM_XTENSA):
         loader = None  # type: Union[ESPCoreDumpFlashLoader, ESPCoreDumpFileLoader, None]
-        core_filename = None
-        target = None
-        temp_files = None
+        core_dump_info_map = {
+            'core_elf_path': None,
+            'target': None,
+            'temp_files': None,
+            'chip_rev': None,
+        }
 
         if not self.core:
             # Core file not specified, try to read core dump from flash.
             if not IDF_PATH:
                 print(IDF_SETUP_ERROR)
                 sys.exit(1)
             loader = ESPCoreDumpFlashLoader(self.off, self.chip, port=self.port, baud=self.baud)
         elif self.core_format != 'elf':
             # Core file specified, but not yet in ELF format. Convert it from raw or base64 into ELF.
             loader = ESPCoreDumpFileLoader(self.core, self.core_format == 'b64')
         else:
             # Core file is already in the ELF format
-            core_filename = self.core
+            core_dump_info_map['core_elf_path'] = self.core
+            chip_rev = self.extract_chip_rev_from_elf()
+
+            if self.chip_rev is not None and chip_rev != self.chip_rev:
+                print('Provided chip revision does not match the one extracted from the provided coredump elf file.',
+                      file=sys.stderr)
+                exit(1)
+
+            core_dump_info_map['chip_rev'] = chip_rev
 
         # Load/convert the core file
         if loader:
             loader.create_corefile(exe_name=self.prog, e_machine=e_machine)
-            core_filename = loader.core_elf_file
+            core_dump_info_map['core_elf_path'] = loader.core_elf_file
             if self.save_core:
                 # We got asked to save the core file, make a copy
                 copyfile(loader.core_elf_file, self.save_core)
-            target = loader.target
-            temp_files = loader.temp_files
+            core_dump_info_map['target'] = loader.target
+            core_dump_info_map['chip_rev'] = loader.chip_rev
+            core_dump_info_map['temp_files'] = loader.temp_files
 
-        return core_filename, target, temp_files  # type: ignore
+        return core_dump_info_map
 
     def get_chip_version(self):  # type: () -> Optional[int]
         for segment in self.core_elf.note_segments:
             for sec in segment.note_secs:
                 if sec.type == ESPCoreDumpElfFile.PT_INFO:
                     ver_bytes = sec.desc[:4]
                     return int((ver_bytes[3] << 8) | ver_bytes[2])
         return None
 
     def get_target(self):  # type: () -> str
-        target = None
 
         if self.chip != 'auto':
             return self.chip  # type: ignore
 
         chip_version = self.get_chip_version()
         if chip_version is not None:
             if chip_version == EspCoreDumpVersion.ESP32:
@@ -154,20 +182,23 @@
 
             if chip_version == EspCoreDumpVersion.ESP32S3:
                 return 'esp32s3'
 
             if chip_version == EspCoreDumpVersion.ESP32C3:
                 return 'esp32c3'
 
+        target = None
         try:
             inst = detect_chip(self.port, self.baud)
         except serial.serialutil.SerialException:
-            print('Unable to identify the chip type. Please use the --chip option to specify the chip type or '
-                  'connect the board and provide the --port option to have the chip type determined automatically.')
-            exit(0)
+            print('Unable to identify the chip type. '
+                  'Please use the --chip option to specify the chip type or '
+                  'connect the board and provide the --port option to have the chip type determined automatically.',
+                  file=sys.stderr)
+            exit(1)
         else:
             target = inst.CHIP_NAME.lower().replace('-', '')
 
         return target  # type: ignore
 
     def get_gdb_path(self, target):  # type: (str) -> Optional[str]
         if self.gdb:
@@ -176,28 +207,27 @@
         if target in XTENSA_TARGETS:
             # For some reason, xtensa-esp32s2-elf-gdb will report some issue.
             # Use xtensa-esp32-elf-gdb instead.
             gdb_path = 'xtensa-esp32-elf-gdb'
         elif target in RISCV_TARGETS:
             gdb_path = 'riscv32-esp-elf-gdb'
         else:
-            raise ValueError('Invalid value: {}. For now we only support {}'.format(target, SUPPORTED_TARGETS))
+            raise ValueError(f'Invalid value: {target}. For now we only support {SUPPORTED_TARGETS}')
         if not find_executable(gdb_path):
             return None
 
         return gdb_path
 
-    def get_gdb_args(self, target, core_elf_path, is_dbg_mode=False):
-        # type: (str, Optional[str], bool) -> List[str]
+    def get_gdb_args(self, target, core_elf_path, chip_rev, is_dbg_mode=False):
         gdb_tool = self.get_gdb_path(target)
         if not gdb_tool:
             print(GDB_NOT_FOUND_ERROR)
             sys.exit(1)
 
-        rom_elf_path = self.get_rom_elf_path(target)
+        rom_elf_path = self.get_rom_elf_path(target=target, chip_rev=chip_rev)
         rom_sym_cmd = self.load_aux_elf(rom_elf_path)
 
         gdb_args = [gdb_tool]
 
         if self.extra_gdbinit_file:
             if not os.path.isfile(self.extra_gdbinit_file):
                 raise ValueError(f'{self.extra_gdbinit_file} does not exist')
@@ -213,19 +243,47 @@
         gdb_args.append('--core={}'.format(core_elf_path))  # core file
         if rom_sym_cmd:
             gdb_args += ['-ex', rom_sym_cmd]
         gdb_args.append(self.prog)
 
         return gdb_args
 
-    def get_rom_elf_path(self, target):  # type: (str) -> str
+    def get_rom_elf_path(self, chip_rev, target):  # type: (Optional[int], str) -> str
         if self.rom_elf:
-            return self.rom_elf  # type: ignore
+            return self.rom_elf
+
+        if chip_rev is None:
+            return ''
+
+        rom_file_path = ''
 
-        return '{}_rom.elf'.format(target)
+        if not IDF_PATH:
+            print("The ROM ELF file won't be loaded automatically since you are running the utility out of IDF.")
+            return rom_file_path
+
+        roms_json = load_json_from_file(ROMS_JSON)
+        target_roms = roms_json.get(target, [])
+
+        if not target_roms:
+            print("The ROM ELF file won't load automatically since it was not found for the provided chip type.")
+            return rom_file_path
+
+        index = len(target_roms)
+        for idx in range(len(target_roms)):
+            if target_roms[idx].get('rev') == chip_rev:
+                index = idx
+                break
+        if index < len(target_roms):
+            chip_rev_from_json = target_roms[index]['rev']
+            rom_elf_file_name = f'{target}_rev{chip_rev_from_json}_rom.elf'
+            rom_file_path = os.path.join(ESP_ROM_ELF_DIR, rom_elf_file_name)  # type: ignore
+        else:
+            print("The ROM ELF file won't load automatically since it was not found for the provided chip type.")
+
+        return rom_file_path
 
     def get_task_info_extra_note_tuple(self):  # type: () -> Tuple[Optional[list[str]], Optional[Container]]
         extra_note = None
         task_info = []
         for note_seg in self.core_elf.note_segments:
             for note_sec in note_seg.note_secs:
                 if note_sec.type == ESPCoreDumpElfFile.PT_EXTRA_INFO and 'EXTRA_INFO' in note_sec.name.decode('ascii'):
@@ -246,15 +304,17 @@
     def print_threads_info(self, task_info):  # type: (Optional[list[Container]]) -> None
         print(self.gdb_esp.run_cmd('info threads'))
         # THREADS STACKS
         threads, _ = self.gdb_esp.get_thread_info()
 
         if not threads:
             print('\nThe threads information for the current task could not be retrieved. '
-                  'Please try running this command again.')
+                  'Please try running this command again with --gdb-timeout-sec option to increase '
+                  f'the default value of internal delay for gdb responses (Default: {DEFAULT_GDB_TIMEOUT_SEC})')
+            return
 
         for thr in threads:
             thr_id = int(thr['id'])
             tcb_addr = self.gdb_esp.gdb2freertos_thread_id(thr['target-id'])
             task_index = int(thr_id) - 1
             task_name = self.gdb_esp.get_freertos_task_name(tcb_addr)
             self.gdb_esp.switch_thread(thr_id)
@@ -348,14 +408,21 @@
             if cs.flags & ElfSegment.PF_X:
                 seg_name = 'rom.text'
             else:
                 seg_name = 'tasks.data'
             print('.coredump.%s 0x%x 0x%x %s' % (seg_name, cs.addr, len(cs.data), cs.attr_str()))
             print(self.gdb_esp.run_cmd('x/%dx 0x%x' % (len(cs.data) // 4, cs.addr)))
 
+    def verify_target(self, core_header_info_dict):
+        target = core_header_info_dict.get('target')
+        if target is None:
+            target = self.get_target()
+            core_header_info_dict['target'] = target
+        return target
+
     @contextmanager
     def _handle_coredump_loader_error(self):
         try:
             yield
         except ESPCoreDumpLoaderError as e:
             print(f'Failed to load core dump: {e}', file=sys.stderr)
             if e.extra_output:
@@ -369,50 +436,51 @@
 
     def dbg_corefile(self):  # type: () -> Optional[list[str]]
         """
         Command to load core dump from file or flash and run GDB debug session with it
         """
         exe_elf = ESPCoreDumpElfFile(self.prog)
         with self._handle_coredump_loader_error():
-            core_elf_path, target, temp_files = self.get_core_dump_elf(e_machine=exe_elf.e_machine)
-            self.core_elf = ESPCoreDumpElfFile(core_elf_path)
+            core_header_info_dict = self.get_core_header_info_dict(e_machine=exe_elf.e_machine)
+            self.core_elf = ESPCoreDumpElfFile(core_header_info_dict['core_elf_path'])
 
-        if target is None:
-            target = self.get_target()
+        temp_files = core_header_info_dict.pop('temp_files')
+        self.chip = self.verify_target(core_header_info_dict)
+
+        gdb_args = self.get_gdb_args(is_dbg_mode=True, **core_header_info_dict)
 
-        gdb_args = self.get_gdb_args(target, core_elf_path, is_dbg_mode=True)
         p = subprocess.Popen(bufsize=0,
                              args=gdb_args,
                              stdin=None, stdout=None, stderr=None,
                              close_fds=CLOSE_FDS)
         p.wait()
         print('Done!')
-        return temp_files
+        return temp_files  # type: ignore
 
     def info_corefile(self):  # type: () -> Optional[list[str]]
         """
         Command to load core dump from file or flash and print it's data in user friendly form
         """
-        self.exe_elf = ESPCoreDumpElfFile(self.prog)
         with self._handle_coredump_loader_error():
-            core_elf_path, target, temp_files = self.get_core_dump_elf(e_machine=self.exe_elf.e_machine)
-            self.core_elf = ESPCoreDumpElfFile(core_elf_path)
+            self.exe_elf = ESPCoreDumpElfFile(self.prog)
+            core_header_info_dict = self.get_core_header_info_dict(e_machine=self.exe_elf.e_machine)
+            self.core_elf = ESPCoreDumpElfFile(core_header_info_dict['core_elf_path'])
 
-        if target is None:
-            target = self.get_target()
+        temp_files = core_header_info_dict.pop('temp_files')
+        self.chip = self.verify_target(core_header_info_dict)
 
         if self.exe_elf.e_machine != self.core_elf.e_machine:
             raise ValueError('The arch should be the same between core elf and exe elf')
 
         task_info, extra_note = self.get_task_info_extra_note_tuple()
 
         print('===============================================================')
         print('==================== ESP32 CORE DUMP START ====================')
 
-        gdb_args = self.get_gdb_args(target, core_elf_path, is_dbg_mode=False)
+        gdb_args = self.get_gdb_args(is_dbg_mode=False, **core_header_info_dict)
 
         self.gdb_esp = EspGDB(gdb_args, timeout_sec=self.gdb_timeout_sec)
 
         extra_info = None
         if extra_note:
             extra_info = Struct('regs' / GreedyRange(Int32ul)).parse(extra_note.desc).regs
             marker = extra_info[0]
@@ -434,8 +502,8 @@
             self.print_core_dump_memory_contents()
 
         print('\n===================== ESP32 CORE DUMP END =====================')
         print('===============================================================')
 
         del self.gdb_esp
         print('Done!')
-        return temp_files
+        return temp_files  # type: ignore
```

### Comparing `esp-coredump-1.5.0/esp_coredump/corefile/__init__.py` & `esp-coredump-1.5.1/esp_coredump/corefile/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
 
 from abc import ABC, abstractmethod
 from importlib import import_module
```

### Comparing `esp-coredump-1.5.0/esp_coredump/corefile/_parse_soc_header.py` & `esp-coredump-1.5.1/esp_coredump/corefile/_parse_soc_header.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # This script will parse soc.h and generate .py file containing all of the target constants.
 # Once one manually adds a new target, the constants file can be regenerated.
 # The script is ESP-IDF dependent and is not intended for use by end users.
 #
```

### Comparing `esp-coredump-1.5.0/esp_coredump/corefile/elf.py` & `esp-coredump-1.5.1/esp_coredump/corefile/elf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
 import hashlib
 import os
 from typing import Optional
@@ -109,14 +109,16 @@
         self._struct = None  # type: Optional[Struct]
         self._model = None  # type: Optional[Container]
 
         self.sections = []  # type: list[ElfSection]
         self.load_segments = []  # type: list[ElfSegment]
         self.note_segments = []  # type: list[ElfNoteSegment]
 
+        self.sha256 = b''  # type: bytes
+
         if elf_path and os.path.isfile(elf_path):
             self.read_elf(elf_path)
 
     def read_elf(self, elf_path):  # type: (str) -> None
         """
         Read elf file, also write to ``self.model``, ``self.program_headers``,
         ``self.section_headers``
@@ -139,14 +141,21 @@
                                              seg.data,
                                              seg.ph.p_flags) for seg in self._model.note_segments]
         self.sections = [ElfSection(self._parse_string_table(self._model.string_table, sec.sh.sh_name),
                                     sec.sh.sh_addr,
                                     sec.data,
                                     sec.sh.sh_flags) for sec in self._model.sections]
 
+        # calculate sha256 of the input bytes (note: this may not be the same as the sha256 of any generated
+        # output struct, as the ELF parser may change some details.)
+        sha256 = hashlib.sha256()
+        sha256.update(elf_bytes)
+        self.sha256 = sha256.digest()
+
+
     @staticmethod
     def _parse_string_table(byte_str, offset):  # type: (bytes, int) -> str
         section_name_str = byte_str[offset:]
         string_end = section_name_str.find(0x00)
 
         if (string_end == -1):
             raise ValueError('Unable to get section name from section header string table')
@@ -198,23 +207,14 @@
             'sections' / Sequence(*section_subcons),
         ]
         if string_table_sh is not None:
             args.append('string_table' / Pointer(string_table_sh.sh_offset, Bytes(string_table_sh.sh_size)))
 
         return Struct(*args)
 
-    @property
-    def sha256(self):  # type: () -> bytes
-        """
-        :return: SHA256 hash of the input ELF file
-        """
-        sha256 = hashlib.sha256()
-        sha256.update(self._struct.build(self._model))  # type: ignore
-        return sha256.digest()
-
 
 class ElfSection(object):
     SHF_WRITE = 0x01
     SHF_ALLOC = 0x02
     SHF_EXECINSTR = 0x04
     SHF_MASKPROC = 0xf0000000
 
@@ -267,14 +267,21 @@
 
 
 class ElfNoteSegment(ElfSegment):
     def __init__(self, addr, data, flags):  # type: (int, bytes, int) -> None
         super(ElfNoteSegment, self).__init__(addr, data, flags)
         self.type = ElfFile.PT_NOTE
         self.note_secs = NoteSections.parse(self.data)
+        for note in self.note_secs:
+            # note.name should include a terminating NUL byte, plus possible
+            # padding
+            #
+            # (note: construct.PaddingString can't parse this if there
+            # are non-zero padding bytes after the NUL, it also parses those.)
+            note.name = note.name.split(b'\x00')[0]
 
     @staticmethod
     def _type_str():  # type: () -> str
         return 'NOTE'
 
 
 TASK_STATUS_CORRECT = 0x00
```

### Comparing `esp-coredump-1.5.0/esp_coredump/corefile/gdb.py` & `esp-coredump-1.5.1/esp_coredump/corefile/gdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
 import logging
 import re
 import time
 
-from pygdbmi.gdbcontroller import DEFAULT_GDB_TIMEOUT_SEC, GdbController
+from pygdbmi.gdbcontroller import GdbController
 
 from . import ESPCoreDumpError
 
+DEFAULT_GDB_TIMEOUT_SEC = 3
+
 
 class EspGDB(object):
     def __init__(self, gdb_args, timeout_sec=DEFAULT_GDB_TIMEOUT_SEC):
 
         """
         Start GDB and initialize a GdbController instance
         """
@@ -89,19 +91,20 @@
         """
         filtered_responses = self._gdbmi_run_cmd_get_responses(cmd="-interpreter-exec console \"%s\"" % gdb_cmd,
                                                                resp_message=None, resp_type='console', multiple=True,
                                                                done_message='done', done_type='result')
         return ''.join([x['payload'] for x in filtered_responses]) \
             .replace('\\n', '\n') \
             .replace('\\t', '\t') \
-            .rstrip('\n')
+            .rstrip('\n') \
+            .replace('\\"', '"')
 
     def get_thread_info(self):
         """ Get information about all threads known to GDB, and the current thread ID """
-        result = self._gdbmi_run_cmd_get_one_response('-thread-info', 'done', 'result', response_delay_sec=2)['payload']
+        result = self._gdbmi_run_cmd_get_one_response('-thread-info', 'done', 'result', response_delay_sec=DEFAULT_GDB_TIMEOUT_SEC)['payload']
         if not result:
             return None, None
 
         current_thread_id = result['current-thread-id']
         threads = result['threads']
         return threads, current_thread_id
```

### Comparing `esp-coredump-1.5.0/esp_coredump/corefile/loader.py` & `esp-coredump-1.5.1/esp_coredump/corefile/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
 import base64
 import binascii
 import hashlib
@@ -41,14 +41,23 @@
     'tot_len' / Int32ul,
     'ver' / Int32ul,
     'task_num' / Int32ul,
     'tcbsz' / Int32ul,
     'segs_num' / Int32ul,
 )
 
+EspCoreDumpV2_1_Header = Struct(
+    'tot_len' / Int32ul,
+    'ver' / Int32ul,
+    'task_num' / Int32ul,
+    'tcbsz' / Int32ul,
+    'segs_num' / Int32ul,
+    'chip_rev' / Int32ul,
+)
+
 CRC = Int32ul
 SHA256 = Bytes(32)
 
 TaskHeader = Struct(
     'tcb_addr' / Int32ul,
     'stack_top' / Int32ul,
     'stack_end' / Int32ul,
@@ -111,16 +120,19 @@
         return self.version & 0x000000FF
 
 
 class EspCoreDumpLoader(EspCoreDumpVersion):
     # "legacy" stands for core dumps v0.1 (before IDF v4.1)
     BIN_V1 = EspCoreDumpVersion.make_dump_ver(0, 1)
     BIN_V2 = EspCoreDumpVersion.make_dump_ver(0, 2)
-    ELF_CRC32 = EspCoreDumpVersion.make_dump_ver(1, 0)
-    ELF_SHA256 = EspCoreDumpVersion.make_dump_ver(1, 1)
+    BIN_V2_1 = EspCoreDumpVersion.make_dump_ver(0, 3)
+    ELF_CRC32_V2 = EspCoreDumpVersion.make_dump_ver(1, 0)
+    ELF_CRC32_V2_1 = EspCoreDumpVersion.make_dump_ver(1, 2)
+    ELF_SHA256_V2 = EspCoreDumpVersion.make_dump_ver(1, 1)
+    ELF_SHA256_V2_1 = EspCoreDumpVersion.make_dump_ver(1, 3)
 
     def __init__(self):  # type: () -> None
         super(EspCoreDumpLoader, self).__init__()
         self.core_src_file = None  # type: Optional[str]
         self.core_src_struct = None
         self.core_src = None
 
@@ -149,39 +161,51 @@
         Return the target str by reading core elf
         """
         with open(self.core_src_file, 'rb') as fr:  # type: ignore
             coredump_bytes = fr.read()
 
         _header = EspCoreDumpV1Header.parse(coredump_bytes)  # first we use V1 format to get version
         self.set_version(_header.ver)
-        if self.dump_ver == self.ELF_CRC32:
+        if self.dump_ver == self.ELF_CRC32_V2:
             self.checksum_struct = CRC
             self.header_struct = EspCoreDumpV2Header
-        elif self.dump_ver == self.ELF_SHA256:
+        elif self.dump_ver == self.ELF_CRC32_V2_1:
+            self.checksum_struct = CRC
+            self.header_struct = EspCoreDumpV2_1_Header
+        elif self.dump_ver == self.ELF_SHA256_V2:
             self.checksum_struct = SHA256
             self.header_struct = EspCoreDumpV2Header
+        elif self.dump_ver == self.ELF_SHA256_V2_1:
+            self.checksum_struct = SHA256
+            self.header_struct = EspCoreDumpV2_1_Header
         elif self.dump_ver == self.BIN_V1:
             self.checksum_struct = CRC
             self.header_struct = EspCoreDumpV1Header
         elif self.dump_ver == self.BIN_V2:
             self.checksum_struct = CRC
             self.header_struct = EspCoreDumpV2Header
+        elif self.dump_ver == self.BIN_V2_1:
+            self.checksum_struct = CRC
+            self.header_struct = EspCoreDumpV2_1_Header
         else:
             raise ESPCoreDumpLoaderError('Core dump version "0x%x" is not supported!' % self.dump_ver)
 
+        self.header = self.header_struct.parse(coredump_bytes)
+
         self.core_src_struct = Struct(
             'header' / self.header_struct,
             'data' / Bytes(this.header.tot_len - self.header_struct.sizeof() - self.checksum_struct.sizeof()),
             'checksum' / self.checksum_struct,
         )
         self.core_src = self.core_src_struct.parse(coredump_bytes)  # type: ignore
 
-        # Reload header if header struct changes after parsing
-        if self.header_struct != EspCoreDumpV1Header:
-            self.header = EspCoreDumpV2Header.parse(coredump_bytes)
+        if self.header and self.header.get('chip_rev') is not None:
+            self.chip_rev = self.header.chip_rev  # type: ignore
+        else:
+            self.chip_rev = None  # type: ignore
 
         if self.chip_ver in self.COREDUMP_SUPPORTED_TARGETS:
             if self.chip_ver == self.ESP32:
                 self.target_methods = Esp32Methods()  # type: ignore
             elif self.chip_ver == self.ESP32S2:
                 self.target_methods = Esp32S2Methods()  # type: ignore
             elif self.chip_ver == self.ESP32C3:
@@ -208,74 +232,109 @@
 
         if self.checksum_struct == CRC:
             self._crc_validate()
         elif self.checksum_struct == SHA256:
             self._sha256_validate()
 
     def _crc_validate(self):  # type: () -> None
-        data_crc = binascii.crc32(
-            EspCoreDumpV2Header.build(self.core_src.header) + self.core_src.data) & 0xffffffff  # type: ignore
+        if self.dump_ver in [self.BIN_V2_1,
+                             self.ELF_CRC32_V2_1]:
+            data_crc = binascii.crc32(
+                EspCoreDumpV2_1_Header.build(self.core_src.header) + self.core_src.data) & 0xffffffff  # type: ignore
+        else:
+            data_crc = binascii.crc32(
+                EspCoreDumpV2Header.build(self.core_src.header) + self.core_src.data) & 0xffffffff  # type: ignore
         if data_crc != self.core_src.checksum:  # type: ignore
             raise ESPCoreDumpLoaderError(
                 'Invalid core dump CRC %x, should be %x' % (data_crc, self.core_src.crc))  # type: ignore
 
     def _sha256_validate(self):  # type: () -> None
-        data_sha256 = hashlib.sha256(
-            EspCoreDumpV2Header.build(self.core_src.header) + self.core_src.data)  # type: ignore
+        if self.dump_ver in [self.ELF_SHA256_V2_1]:
+            data_sha256 = hashlib.sha256(
+                EspCoreDumpV2_1_Header.build(self.core_src.header) + self.core_src.data)  # type: ignore
+        else:
+            data_sha256 = hashlib.sha256(
+                EspCoreDumpV2Header.build(self.core_src.header) + self.core_src.data)  # type: ignore
+
         data_sha256_str = data_sha256.hexdigest()
         sha256_str = binascii.hexlify(self.core_src.checksum).decode('ascii')  # type: ignore
         if data_sha256_str != sha256_str:
             raise ESPCoreDumpLoaderError('Invalid core dump SHA256 "{}", should be "{}"'
                                          .format(data_sha256_str, sha256_str))
 
     def create_corefile(self, exe_name=None, e_machine=ESPCoreDumpElfFile.EM_XTENSA):
         # type: (Optional[str], Optional[int]) -> None
         """
         Creates core dump ELF file
         """
         self._validate_dump_file()
         self.core_elf_file = self._create_temp_file()
 
-        if self.dump_ver in [self.ELF_CRC32,
-                             self.ELF_SHA256]:
+        if self.dump_ver in [self.ELF_CRC32_V2,
+                             self.ELF_CRC32_V2_1,
+                             self.ELF_SHA256_V2,
+                             self.ELF_SHA256_V2_1]:
             self._extract_elf_corefile(exe_name, e_machine)
         elif self.dump_ver in [self.BIN_V1,
-                               self.BIN_V2]:
+                               self.BIN_V2,
+                               self.BIN_V2_1]:
             self._extract_bin_corefile(e_machine)
         else:
             raise NotImplementedError
 
     def _extract_elf_corefile(self, exe_name=None, e_machine=ESPCoreDumpElfFile.EM_XTENSA):
         # type: (str, Optional[int]) -> None
         """
         Reads the ELF formatted core dump image and parse it
         """
         with open(self.core_elf_file, 'wb') as fw:  # type: ignore
             fw.write(self.core_src.data)  # type: ignore
 
         core_elf = ESPCoreDumpElfFile(self.core_elf_file, e_machine=e_machine)  # type: ignore
 
+        if self.chip_rev is not None:  # type: ignore
+            chip_rev_note = b''
+            chip_rev_note += self._build_note_section('ESP_CHIP_REV',
+                                                      ESPCoreDumpElfFile.PT_INFO,
+                                                      Int32ul.build(self.chip_rev))  # type: ignore
+            try:
+                core_elf.add_segment(0, chip_rev_note, ElfFile.PT_NOTE, 0)
+            except ESPCoreDumpLoaderError as e:
+                logging.warning('Skip core dump info NOTES segment {:d} bytes @ 0x{:x}. (Reason: {})'
+                                .format(len(chip_rev_note), 0, e))
+            core_elf.dump(self.core_elf_file)
+
         # Read note segments from core file which are belong to tasks (TCB or stack)
         for seg in core_elf.note_segments:
             for note_sec in seg.note_secs:
                 # Check for version info note
-                if note_sec.name == 'ESP_CORE_DUMP_INFO' \
+                if note_sec.name == b'ESP_CORE_DUMP_INFO' \
                         and note_sec.type == ESPCoreDumpElfFile.PT_INFO \
                         and exe_name:
                     exe_elf = ElfFile(exe_name)
                     app_sha256 = binascii.hexlify(exe_elf.sha256)
                     coredump_sha256_struct = Struct(
                         'ver' / Int32ul,
                         'sha256' / Bytes(64)  # SHA256 as hex string
                     )
                     coredump_sha256 = coredump_sha256_struct.parse(note_sec.desc[:coredump_sha256_struct.sizeof()])
-                    if coredump_sha256.sha256 != app_sha256:
+
+                    logging.debug('App SHA256: {!r}'.format(app_sha256))
+                    logging.debug('Core dump SHA256: {!r}'.format(coredump_sha256))
+
+                    # Actual coredump SHA may be shorter than a full SHA256 hash
+                    # with NUL byte padding, according to the app's APP_RETRIEVE_LEN_ELF_SHA
+                    # length
+                    core_sha_trimmed = coredump_sha256.sha256.rstrip(b'\x00').decode()
+                    app_sha_trimmed = app_sha256[:len(core_sha_trimmed)].decode()
+
+                    if core_sha_trimmed != app_sha_trimmed:
                         raise ESPCoreDumpLoaderError(
-                            'Invalid application image for coredump: coredump SHA256({!r}) != app SHA256({!r}).'
-                            .format(coredump_sha256, app_sha256))
+                            'Invalid application image for coredump: coredump SHA256({}) != app SHA256({}).'
+                            .format(core_sha_trimmed, app_sha_trimmed))
                     if coredump_sha256.ver != self.version:
                         raise ESPCoreDumpLoaderError(
                             'Invalid application image for coredump: coredump SHA256 version({}) != app SHA256 version({}).'
                             .format(coredump_sha256.ver, self.version))
 
     @staticmethod
     def _get_aligned_size(size, align_with=4):  # type: (int, int) -> int
@@ -508,15 +567,15 @@
             tool_args.append(self.core_src_file)  # type: ignore
             # read core dump partition
             et_out = subprocess.check_output(tool_args, stderr=subprocess.STDOUT)
             if et_out:
                 logging.info(et_out.decode('utf-8'))
         except subprocess.CalledProcessError as e:
             raise ESPCoreDumpLoaderError(f'parttool script execution failed with error {e.returncode}, '
-                                         "failed command was: '{}'".format(' '.join(e.cmd)),
+                                         f"failed command was: '{' '.join(e.cmd)}'",
                                          extra_output=e.output.decode('utf-8', 'ignore'))
 
     def _get_core_dump_partition_info(self, part_off=None):  # type: (Optional[int]) -> Tuple[int, int]
         """
         Get core dump partition info using parttool
         """
         logging.info('Retrieving core dump partition offset and size...')
@@ -532,15 +591,15 @@
             res = subprocess.check_output(invoke_args).strip()
             (offset_str, size_str) = res.rsplit(b'\n')[-1].split(b' ')
             size = int(size_str, 16)
             offset = int(offset_str, 16)
             logging.info('Core dump partition offset=%d, size=%d', offset, size)
         except subprocess.CalledProcessError as e:
             raise ESPCoreDumpLoaderError(f'parttool script execution failed with error {e.returncode}, '
-                                         "failed command was: '{}'".format(' '.join(e.cmd)),
+                                         f"failed command was: '{' '.join(e.cmd)}'",
                                          extra_output=e.output.decode('utf-8', 'ignore'))
         return offset, size
 
 
 class ESPCoreDumpFileLoader(EspCoreDumpLoader):
     def __init__(self, path, is_b64=False):  # type: (str, bool) -> None
         super(ESPCoreDumpFileLoader, self).__init__()
```

### Comparing `esp-coredump-1.5.0/esp_coredump/corefile/riscv.py` & `esp-coredump-1.5.1/esp_coredump/corefile/riscv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
 from typing import Any, Optional, Tuple
 
 from construct import Int16ul, Int32ul, Padding, Struct
```

### Comparing `esp-coredump-1.5.0/esp_coredump/corefile/xtensa.py` & `esp-coredump-1.5.1/esp_coredump/corefile/xtensa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
 from typing import Any, Optional, Tuple
 
 from construct import Int16ul, Int32ul, Int64ul, Struct
```

### Comparing `esp-coredump-1.5.0/esp_coredump/scripts/espcoredump.py` & `esp-coredump-1.5.1/esp_coredump/scripts/espcoredump.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
 import logging
 import os.path
 
@@ -25,16 +25,16 @@
         log_level = logging.INFO
     else:
         log_level = logging.DEBUG
     logging.basicConfig(format='%(levelname)s: %(message)s', level=log_level)
 
     kwargs = {k: v for k, v in vars(args).items() if v is not None}
 
-    del(kwargs['debug'])
-    del(kwargs['operation'])
+    del kwargs['debug']
+    del kwargs['operation']
 
     espcoredump = CoreDump(**kwargs)
     temp_core_files = None
 
     try:
         if args.operation == 'info_corefile':
             temp_core_files = espcoredump.info_corefile()
```

### Comparing `esp-coredump-1.5.0/esp_coredump.egg-info/PKG-INFO` & `esp-coredump-1.5.1/esp_coredump.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-coredump
-Version: 1.5.0
+Version: 1.5.1
 Summary: Generate core dumps on unrecoverable software errors
 Home-page: https://github.com/espressif/esp-idf
 Author: Espressif Systems
 Author-email: aleksei.apaseev@espressif.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `esp-coredump-1.5.0/esp_coredump.egg-info/SOURCES.txt` & `esp-coredump-1.5.1/esp_coredump.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 esp_coredump/__init__.py
 esp_coredump/cli_ext.py
 esp_coredump/coredump.py
+esp_coredump/tools.py
 esp_coredump.egg-info/PKG-INFO
 esp_coredump.egg-info/SOURCES.txt
 esp_coredump.egg-info/dependency_links.txt
 esp_coredump.egg-info/entry_points.txt
 esp_coredump.egg-info/requires.txt
 esp_coredump.egg-info/top_level.txt
 esp_coredump/corefile/__init__.py
@@ -23,8 +24,11 @@
 esp_coredump/corefile/soc_headers/esp32c2.py
 esp_coredump/corefile/soc_headers/esp32c3.py
 esp_coredump/corefile/soc_headers/esp32c6.py
 esp_coredump/corefile/soc_headers/esp32h2.py
 esp_coredump/corefile/soc_headers/esp32s2.py
 esp_coredump/corefile/soc_headers/esp32s3.py
 esp_coredump/scripts/__init__.py
-esp_coredump/scripts/espcoredump.py
+esp_coredump/scripts/espcoredump.py
+esp_coredump/scripts/run_tests.py
+tests/__init__.py
+tests/test_espcoredump.py
```

### Comparing `esp-coredump-1.5.0/setup.py` & `esp-coredump-1.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
 import io
 import os
 import re
@@ -45,24 +45,25 @@
     raise RuntimeError('Unable to find version string.')
 
 
 setup(
     name=NAME,
     version=find_version(init_file_path),
     description=DESCRIPTION,
+    include_package_data=True,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'esp-coredump = esp_coredump.scripts.espcoredump:main'
+            'esp-coredump = esp_coredump.scripts.espcoredump:main',
         ],
     },
     install_requires=REQUIRED,
     license='Apache 2.0',
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
```

