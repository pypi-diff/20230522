# Comparing `tmp/unicode-name-inquiry-1.9.1.tar.gz` & `tmp/unicode-name-inquiry-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicode-name-inquiry-1.9.1.tar", last modified: Fri May 12 21:30:46 2023, max compression
+gzip compressed data, was "unicode-name-inquiry-1.9.2.tar", last modified: Mon May 22 16:57:55 2023, max compression
```

## Comparing `unicode-name-inquiry-1.9.1.tar` & `unicode-name-inquiry-1.9.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-12 21:30:46.000000 unicode-name-inquiry-1.9.1/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1057 2023-05-10 23:37:19.000000 unicode-name-inquiry-1.9.1/LICENSE
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5215 2023-05-12 21:30:46.000000 unicode-name-inquiry-1.9.1/PKG-INFO
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4405 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.1/README.md
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2763 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.1/pyproject.toml
--rw-rw-r--   0 kevin     (1001) dialout     (20)       38 2023-05-12 21:30:46.000000 unicode-name-inquiry-1.9.1/setup.cfg
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-12 21:30:46.000000 unicode-name-inquiry-1.9.1/src/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2132 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.1/src/test_uni.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-12 21:30:46.000000 unicode-name-inquiry-1.9.1/src/uc/
--rw-rw-r--   0 kevin     (1001) dialout     (20)        0 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.1/src/uc/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1516 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.1/src/uc/block.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-12 21:30:46.000000 unicode-name-inquiry-1.9.1/src/uc/data/
--rw-rw-r--   0 kevin     (1001) dialout     (20)        0 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.1/src/uc/data/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    18514 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.1/src/uc/data/block.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1066 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.1/src/uc/data/ccc.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2498 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.1/src/uc/format.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2096 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.1/src/uc/search.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1341 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.1/src/uc/test_block.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3452 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.1/src/uc/test_format.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1351 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.1/src/uc/test_search.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3912 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.1/src/uc/test_uni.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3108 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.1/src/uc/uni.py
--rwxrwxr-x   0 kevin     (1001) dialout     (20)     6778 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.1/src/uni.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-12 21:30:46.000000 unicode-name-inquiry-1.9.1/src/unicode_name_inquiry.egg-info/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5215 2023-05-12 21:30:46.000000 unicode-name-inquiry-1.9.1/src/unicode_name_inquiry.egg-info/PKG-INFO
--rw-rw-r--   0 kevin     (1001) dialout     (20)      533 2023-05-12 21:30:46.000000 unicode-name-inquiry-1.9.1/src/unicode_name_inquiry.egg-info/SOURCES.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)        1 2023-05-12 21:30:46.000000 unicode-name-inquiry-1.9.1/src/unicode_name_inquiry.egg-info/dependency_links.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)       33 2023-05-12 21:30:46.000000 unicode-name-inquiry-1.9.1/src/unicode_name_inquiry.egg-info/entry_points.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)       16 2023-05-12 21:30:46.000000 unicode-name-inquiry-1.9.1/src/unicode_name_inquiry.egg-info/top_level.txt
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 16:57:55.000000 unicode-name-inquiry-1.9.2/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1057 2023-05-10 23:37:19.000000 unicode-name-inquiry-1.9.2/LICENSE
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5215 2023-05-22 16:57:55.000000 unicode-name-inquiry-1.9.2/PKG-INFO
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4405 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.2/README.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3817 2023-05-22 16:33:03.000000 unicode-name-inquiry-1.9.2/pyproject.toml
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       38 2023-05-22 16:57:55.000000 unicode-name-inquiry-1.9.2/setup.cfg
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 16:57:55.000000 unicode-name-inquiry-1.9.2/src/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2133 2023-05-21 14:51:20.000000 unicode-name-inquiry-1.9.2/src/test_uni.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 16:57:55.000000 unicode-name-inquiry-1.9.2/src/uc/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       35 2023-05-22 16:32:11.000000 unicode-name-inquiry-1.9.2/src/uc/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1639 2023-05-22 16:30:42.000000 unicode-name-inquiry-1.9.2/src/uc/block.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 16:57:55.000000 unicode-name-inquiry-1.9.2/src/uc/data/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       58 2023-05-22 16:32:46.000000 unicode-name-inquiry-1.9.2/src/uc/data/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    18613 2023-05-21 14:25:06.000000 unicode-name-inquiry-1.9.2/src/uc/data/block.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1066 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.2/src/uc/data/ccc.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1488 2023-05-22 16:31:01.000000 unicode-name-inquiry-1.9.2/src/uc/format.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2263 2023-05-21 17:34:53.000000 unicode-name-inquiry-1.9.2/src/uc/search.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1426 2023-05-21 17:53:23.000000 unicode-name-inquiry-1.9.2/src/uc/test_block.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3461 2023-05-21 17:50:43.000000 unicode-name-inquiry-1.9.2/src/uc/test_format.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1448 2023-05-21 17:51:19.000000 unicode-name-inquiry-1.9.2/src/uc/test_search.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5128 2023-05-22 15:28:23.000000 unicode-name-inquiry-1.9.2/src/uc/test_uni.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4864 2023-05-22 16:31:27.000000 unicode-name-inquiry-1.9.2/src/uc/uni.py
+-rwxrwxr-x   0 kevin     (1001) dialout     (20)     7043 2023-05-22 16:31:43.000000 unicode-name-inquiry-1.9.2/src/uni.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 16:57:55.000000 unicode-name-inquiry-1.9.2/src/unicode_name_inquiry.egg-info/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5215 2023-05-22 16:57:54.000000 unicode-name-inquiry-1.9.2/src/unicode_name_inquiry.egg-info/PKG-INFO
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      533 2023-05-22 16:57:54.000000 unicode-name-inquiry-1.9.2/src/unicode_name_inquiry.egg-info/SOURCES.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)        1 2023-05-22 16:57:54.000000 unicode-name-inquiry-1.9.2/src/unicode_name_inquiry.egg-info/dependency_links.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       33 2023-05-22 16:57:54.000000 unicode-name-inquiry-1.9.2/src/unicode_name_inquiry.egg-info/entry_points.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       16 2023-05-22 16:57:54.000000 unicode-name-inquiry-1.9.2/src/unicode_name_inquiry.egg-info/top_level.txt
```

### Comparing `unicode-name-inquiry-1.9.1/LICENSE` & `unicode-name-inquiry-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unicode-name-inquiry-1.9.1/PKG-INFO` & `unicode-name-inquiry-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicode-name-inquiry
-Version: 1.9.1
+Version: 1.9.2
 Summary: Command-line tool to display Unicode character information
 License: MIT License
 Project-URL: repository, https://codeberg.org/datatravelandexperiments/uni
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `unicode-name-inquiry-1.9.1/README.md` & `unicode-name-inquiry-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `unicode-name-inquiry-1.9.1/src/test_uni.py` & `unicode-name-inquiry-1.9.2/src/test_uni.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: MIT
-"""Test uni command"""
+"""Test uni command."""
 
 import uni
 
 def test_no_args(capsys):
     status = uni.main(['uni'])
     out = capsys.readouterr().out
     assert status != 0
```

### Comparing `unicode-name-inquiry-1.9.1/src/uc/block.py` & `unicode-name-inquiry-1.9.2/src/uc/block.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 # SPDX-License-Identifier: MIT
+"""Unicode blocks."""
 
 import uc.data.block
 
 class UniBlock:
     """Representation of a Unicode block (or any contiguous character range)."""
 
-    def __init__(self, which: int | str):
+    def __init__(self, which: int | str) -> None:
         self.range, self.name = block(which)
 
-    def __contains__(self, key: str | int):
+    def __contains__(self, key: str | int) -> bool:
         if isinstance(key, str):
             key = ord(key)
         return key in self.range
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return 'UniBlock({repr(self.rnge)},{repr(self.name)})'
 
-def __sq(s):
+def __sq(s: str) -> str:
     return ''.join([c.lower() for c in s if c.isalnum()])
 
 def by_name(name: str) -> tuple[range, str]:
     name = __sq(name)
     for r, names in uc.data.block.BLOCKS:
         for s in names:
             if name == __sq(s):
                 return (r, names[0])
-    raise ValueError(f'Unknown block "{name}"')
+    message = f'Unknown block "{name}"'
+    raise ValueError(message)
 
 def by_code_point(value: int) -> tuple[range, str]:
     for r, names in uc.data.block.BLOCKS:
         if value in r:
             return (r, names[0])
-    raise ValueError(f'No block contains 0x{value:06X}')
+    message = f'No block contains 0x{value:06X}'
+    raise ValueError(message)
 
 def block(which: int | str) -> tuple[range, str]:
     """Get a block by range, code point, character, or name."""
     if isinstance(which, int):
         # Block containing the given code point.
         return by_code_point(which)
 
     if isinstance(which, str):
         if len(which) == 1:
             # Block containing the given character.
             return by_code_point(ord(which))
         # Block looked up by name.
         return by_name(which)
 
-    raise TypeError(f'{which} does not identify a unicode block')
+    message = f'{which} does not identify a unicode block'
+    raise TypeError(message)
```

### Comparing `unicode-name-inquiry-1.9.1/src/uc/data/block.py` & `unicode-name-inquiry-1.9.2/src/uc/data/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,24 +41,26 @@
     (range(0x000F00, 0x001000), ['Tibetan']),
     (range(0x001000, 0x0010A0), ['Myanmar']),
     (range(0x0010A0, 0x001100), ['Georgian']),
     (range(0x001100, 0x001200), ['Hangul Jamo']),
     (range(0x001200, 0x001380), ['Ethiopic']),
     (range(0x001380, 0x0013A0), ['Ethiopic Supplement']),
     (range(0x0013A0, 0x001400), ['Cherokee']),
-    (range(0x001400, 0x001680), ['Unified Canadian Aboriginal Syllabics', 'UCAS']),
+    (range(0x001400,
+           0x001680), ['Unified Canadian Aboriginal Syllabics', 'UCAS']),
     (range(0x001680, 0x0016A0), ['Ogham']),
     (range(0x0016A0, 0x001700), ['Runic']),
     (range(0x001700, 0x001720), ['Tagalog']),
     (range(0x001720, 0x001740), ['Hanunoo']),
     (range(0x001740, 0x001760), ['Buhid']),
     (range(0x001760, 0x001780), ['Tagbanwa']),
     (range(0x001780, 0x001800), ['Khmer']),
     (range(0x001800, 0x0018B0), ['Mongolian']),
-    (range(0x0018B0, 0x001900), ['Unified Canadian Aboriginal Syllabics Extended']),
+    (range(0x0018B0,
+           0x001900), ['Unified Canadian Aboriginal Syllabics Extended']),
     (range(0x001900, 0x001950), ['Limbu']),
     (range(0x001950, 0x001980), ['Tai Le']),
     (range(0x001980, 0x0019E0), ['New Tai Lue']),
     (range(0x0019E0, 0x001A00), ['Khmer Symbols']),
     (range(0x001A00, 0x001A20), ['Buginese']),
     (range(0x001A20, 0x001AB0), ['Tai Tham']),
     (range(0x001AB0, 0x001B00), ['Combining Diacritical Marks Extended']),
@@ -242,15 +244,16 @@
     (range(0x011700, 0x011750), ['Ahom']),
     (range(0x011800, 0x011850), ['Dogra']),
     (range(0x0118A0, 0x011900), ['Warang Citi']),
     (range(0x011900, 0x011960), ['Dives Akuru']),
     (range(0x0119A0, 0x011A00), ['Nandinagari']),
     (range(0x011A00, 0x011A50), ['Zanabazar Square']),
     (range(0x011A50, 0x011AB0), ['Soyombo']),
-    (range(0x011AB0, 0x011AC0), ['Unified Canadian Aboriginal Syllabics Extended-A']),
+    (range(0x011AB0,
+           0x011AC0), ['Unified Canadian Aboriginal Syllabics Extended-A']),
     (range(0x011AC0, 0x011B00), ['Pau Cin Hau']),
     (range(0x011B00, 0x011B60), ['Devanagari Extended-A']),
     (range(0x011C00, 0x011C70), ['Bhaiksuki']),
     (range(0x011C70, 0x011CC0), ['Marchen']),
     (range(0x011D00, 0x011D60), ['Masaram Gondi']),
     (range(0x011D60, 0x011DB0), ['Gunjala Gondi']),
     (range(0x011EE0, 0x011F00), ['Makasar']),
@@ -328,14 +331,16 @@
     (range(0x02B820, 0x02CEB0), ['CJK Unified Ideographs Extension E']),
     (range(0x02CEB0, 0x02EBF0), ['CJK Unified Ideographs Extension F']),
     (range(0x02F800, 0x02FA20), ['CJK Compatibility Ideographs Supplement']),
     (range(0x030000, 0x031350), ['CJK Unified Ideographs Extension G']),
     (range(0x031350, 0x0323B0), ['CJK Unified Ideographs Extension H']),
     (range(0x0E0000, 0x0E0080), ['Tags']),
     (range(0x0E0100, 0x0E01F0), ['Variation Selectors Supplement']),
-    (range(0x0F0000, 0x100000), ['Supplementary Private Use Area-A', 'S PUA A']),
-    (range(0x100000, 0x110000), ['Supplementary Private Use Area-B', 'S PUA B']),
+    (range(0x0F0000, 0x100000), ['Supplementary Private Use Area-A',
+                                 'S PUA A']),
+    (range(0x100000, 0x110000), ['Supplementary Private Use Area-B',
+                                 'S PUA B']),
     # Planes
     (range(0x000000, 0x010000), ['Basic Multilingual Plane', 'BMP']),
     (range(0x010000, 0x020000), ['Supplementary Multilingual Plane', 'SMP']),
     (range(0x020000, 0x030000), ['Supplementary Ideographic Plane', 'SIP']),
 ]
```

### Comparing `unicode-name-inquiry-1.9.1/src/uc/data/ccc.py` & `unicode-name-inquiry-1.9.2/src/uc/data/ccc.py`

 * *Files identical despite different names*

### Comparing `unicode-name-inquiry-1.9.1/src/uc/format.py` & `unicode-name-inquiry-1.9.2/src/uc/format.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,48 @@
 # SPDX-License-Identifier: MIT
+"""Formatting."""
 
-from collections.abc import Iterable, Sequence
+from collections.abc import Iterable
 
-import uc.block
 import uc.uni
 
 class UniFormat:
     """Allows a character to be passed to str.format_map()."""
 
-    def __init__(self, c: str, eol: str = '\n'):
+    alias = {
+        'id': 'identifier',
+        'utf-8': 'utf8',
+        'utf-16': 'utf16',
+        'v': 'ordinal',
+        'x': 'hexadecimal',
+    }
+
+    def __init__(self, c: str, eol: str = '\n') -> None:
         self.c = c
         self.v = ord(c)
         self.eol = eol
 
     def __getitem__(self, key: str) -> str:
         k = key.lower()
-        if k == 'char':
-            return self.c
-        if k == 'u':
-            return f'U+{self.v:04X}'
-        if k == 'v':
-            return str(self.v)
-        if k == 'x':
-            return f'{self.v:04X}'
+        if (a := self.alias.get(k)):
+            k = a
         if k.startswith('u') and k[1 :].isdigit():
-            width = int(k[1 :])
-            return f'U+{self.v:0{width}X}'
-        if key in set(('utf8', 'utf-8')):
-            return list_to_hex(utf32to8(self.v), 2)
-        if key in set(('UTF8', 'UTF-8')):
-            return repr(utf32to8(self.v))
-        if key in set(('utf16', 'utf-16')):
-            return list_to_hex(utf32to16(self.v), 4)
-        if key in set(('UTF16', 'UTF-16')):
-            return repr(utf32to16(self.v))
-        if key == 'block':
-            _, name = uc.block.block(self.v)
-            return name
-        if key == 'id':
-            return uc.uni.name(self.c).replace(' ', '_').replace('-', '_')
+            return uc.uni.u(self.c, digits=int(k[1 :]))
+        if k == 'utf8':
+            r = uc.uni.utf8(self.c)
+            return repr(r) if key.isupper() else list_to_hex(r, 2)
+        if k == 'utf16':
+            r = uc.uni.utf16(self.c)
+            return repr(r) if key.isupper() else list_to_hex(r, 4)
         if k in ('nfc', 'nfkc', 'nfd', 'nfkd'):
             v = uc.uni.normalize(self.c, k)
-            if key.isupper():
-                return v
-            return ', '.join(uc.uni.name(c) for c in v)
+            return v if key.isupper() else ', '.join(
+                uc.uni.name(c, '?') for c in v)
         if key == 'eol':
             return self.eol
         if k in uc.uni.PROPERTIES:
             return str(uc.uni.PROPERTIES[k](self.c, ''))
         raise KeyError(key)
 
-def utf32to16(n: int) -> Sequence[int]:
-    """Converts a number to a list holding its UTF-16 encoding."""
-    if (n <= 0xD7FF) or (0xE000 <= n <= 0xFFFF):
-        return [n]
-    if n < 0x10000 or n > 0x10FFFF:
-        return []
-    n = n - 0x10000
-    return [0xD800 + (n >> 10), 0xDC00 + (n & 0x3FF)]
-
-def utf32to8(n: int) -> Sequence[int]:
-    """Converts a number to a list holding its UTF-8 encoding."""
-    if n < 0x80:
-        return [n]
-    r = []
-    m = 0x1F
-    while True:
-        r.append(0x80 | (n & 0x3F))
-        n = n >> 6
-        if n & m == n:
-            break
-        m = m >> 1
-    r.append((0xFE ^ (m << 1)) | n)
-    r.reverse()
-    return r
-
 def list_to_hex(i: Iterable[int], w: int = 2) -> str:
     """Return a string of hexadecimal numbers from a list of integers."""
-    return ' '.join(map(lambda x: f'{x:0{w}X}', i))
+    return ' '.join(f'{x:0{w}X}' for x in i)
```

### Comparing `unicode-name-inquiry-1.9.1/src/uc/search.py` & `unicode-name-inquiry-1.9.2/src/uc/search.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,70 +2,76 @@
 """Character name searches."""
 
 import fnmatch
 import re
 import unicodedata
 
 from collections.abc import Callable, Iterable
+from typing import Any
 
 import uc.uni
 
 # Name searches.
 
 NameSearch = Callable[
     [Iterable[str], Iterable[str], Callable[[Iterable], bool]], Iterable[str]]
 
+Fold = Callable[[Iterable[Any]], bool]
+
 def search_exact(select: Iterable[str],
                  source: Iterable[str],
-                 fold=all) -> Iterable[str]:
+                 _fold: Fold = all) -> Iterable[str]:
     r = []
     for s in select:
-        if len(s) > 1:
+        if len(s) == 1:
+            c = s
+        else:
             try:
-                s = uc.uni.unichr(s)
+                c = uc.uni.unichr(s)
             except ValueError:
                 continue
-        if s in source:
-            r.append(s)
+        if c in source:
+            r.append(c)
     return r
 
 def search_match(select: Iterable[str],
                  source: Iterable[str],
-                 fold=all) -> Iterable[str]:
+                 fold: Fold = all) -> Iterable[str]:
     search = [s.upper() for s in select]
     return (c for c in source if fold(
         x in unicodedata.name(c, '') for x in search))
 
 def search_word(select: Iterable[str],
                 source: Iterable[str],
-                fold=all) -> Iterable[str]:
+                fold: Fold = all) -> Iterable[str]:
     search = [s.upper() for s in select]
     return (c for c in source if fold(
         x in unicodedata.name(c, '').split() for x in search))
 
 def search_egrep(select: Iterable[str],
                  source: Iterable[str],
-                 fold=all) -> Iterable[str]:
+                 fold: Fold = all) -> Iterable[str]:
     search = [re.compile(x, re.IGNORECASE) for x in select]
     return (c for c in source if fold(
         x.search(unicodedata.name(c, '')) for x in search))
 
 def search_glob(select: Iterable[str],
                 source: Iterable[str],
-                fold=all) -> Iterable[str]:
+                fold: Fold = all) -> Iterable[str]:
     return search_egrep((fnmatch.translate(x) for x in select), source, fold)
 
 __NAME_SEARCH = {
     'exact': search_exact,
     'match': search_match,
     'word': search_word,
     'egrep': search_egrep,
     'glob': search_glob,
 }
 
 def search_name(mode: str,
                 select: Iterable[str],
                 source: Iterable[str],
-                fold=all) -> Iterable[str]:
+                fold: Fold = all) -> Iterable[str]:
     if mode in __NAME_SEARCH:
         return __NAME_SEARCH[mode](select, source, fold)
-    raise ValueError(f'Unknown mode ‘{mode}’')
+    message = f'Unknown mode ‘{mode}’'
+    raise ValueError(message)
```

### Comparing `unicode-name-inquiry-1.9.1/src/uc/test_block.py` & `unicode-name-inquiry-1.9.2/src/uc/test_block.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # SPDX-License-Identifier: MIT
-"""Test uc.block"""
+"""Test uc.block."""
 
 import pytest
 
 from uc.block import UniBlock
 
 def test_uniblock_init_code_point():
     b = UniBlock(0x0123)
     assert b.range == range(0x100, 0x180)
     assert b.name == 'Latin Extended-A'
 
 def test_uniblock_init_code_point_unassigned():
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='No block'):
         _ = UniBlock(0x43210)
 
 def test_uniblock_init_character():
     b = UniBlock('\u2192')
     assert b.range == range(0x2190, 0x2200)
     assert b.name == 'Arrows'
 
 def test_uniblock_init_character_unassigned():
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='No block'):
         _ = UniBlock('\U00042310')
 
 def test_uniblock_init_type_error():
     with pytest.raises(TypeError):
-        _ = UniBlock(UniBlock)
+        _ = UniBlock(UniBlock)  # type:ignore[arg-type]
 
 def test_uniblock_init_name():
     b = UniBlock('ASCII')
     assert b.range == range(0x00, 0x80)
     assert b.name == 'Basic Latin'
 
 def test_uniblock_init_name_unassigned():
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Unknown block'):
         _ = UniBlock('This is probably not the name of a Unicode block')
 
 def test_uniblock_contains():
     b = UniBlock('Arrows')
     assert 0x21FF in b
     assert '\u21FF' in b
     assert 0x2190 in b
```

### Comparing `unicode-name-inquiry-1.9.1/src/uc/test_format.py` & `unicode-name-inquiry-1.9.2/src/uc/test_format.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: MIT
-"""Test code.format"""
+"""Test code.format."""
 
 import pytest
 
 from uc.format import UniFormat
 
 # yapf: disable
 FORMAT_CASES: list[tuple[str, str, str]] = [
@@ -62,15 +62,15 @@
      'LATIN CAPITAL LETTER A, COMBINING GRAVE ACCENT'),
     ('\u01C4',      'NFKD',             'DZ\u030C'),
     ('\u01C4',      'nfkd',
      'LATIN CAPITAL LETTER D, LATIN CAPITAL LETTER Z, COMBINING CARON'),
 ]
 # yapf: enable
 
-@pytest.mark.parametrize('character,key,result', FORMAT_CASES)
+@pytest.mark.parametrize(('character', 'key', 'result'), FORMAT_CASES)
 def test_uni_format_init(character, key, result):
     u = UniFormat(character)
     assert u[key] == result
 
 def test_uni_format_key_error():
     u = UniFormat('X')
     with pytest.raises(KeyError):
```

### Comparing `unicode-name-inquiry-1.9.1/src/uc/test_search.py` & `unicode-name-inquiry-1.9.2/src/uc/test_search.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # SPDX-License-Identifier: MIT
-"""Test code.search"""
+"""Test code.search."""
 
 import sys
 
+from collections.abc import Generator
+
 import pytest
 
 from uc.search import search_name
 
 # NB. Some of these tests could fail in the future if Unicode adds
 # new characters with unfortunately conflicting names.
 
-def chars(lo: int = 0, hi: int = sys.maxunicode + 1):
+def chars(lo: int = 0,
+          hi: int = sys.maxunicode + 1) -> Generator[str, None, None]:
     return (chr(i) for i in range(lo, hi))
 
 def test_search_name_exact():
     r = search_name('exact', ['8', 'Digit nine', '\uABCD', 'fail'],
                     chars(0, 0x7F))
     assert list(r) == list('89')
 
@@ -35,9 +38,9 @@
     assert list(r) == list('%,:;@^`')
 
 def test_search_name_glob():
     r = search_name('glob', ['c[eo]*n'], chars(0, 0x7F))
     assert list(r) == list('%:;')
 
 def test_search_name_bad():
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Unknown'):
         _ = search_name('bad', ['c[eo]*n'], chars(0, 0x7F))
```

### Comparing `unicode-name-inquiry-1.9.1/src/uc/test_uni.py` & `unicode-name-inquiry-1.9.2/src/uc/test_uni.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 # SPDX-License-Identifier: MIT
-"""Test code.block"""
+"""Test code.block."""
 
 from typing import Any
 
 import pytest
 
-import uc.uni
 import uc.data.ccc
+import uc.uni
 
 UNICHR_CASES: list[tuple[str, Any]] = [
     ('C', 67),
     ('D', 'D'),
     ('E', 'Latin capital letter E'),
     ('F', 'u46'),
     ('G', 'U+000000047'),
 ]
 
-@pytest.mark.parametrize('c,i', UNICHR_CASES)
+@pytest.mark.parametrize(('c', 'i'), UNICHR_CASES)
 def test_unichr(c, i):
     u = uc.uni.unichr(i)
     assert u == c
 
 def test_unichr_type_error():
     with pytest.raises(TypeError):
-        _ = uc.uni.unichr(Any)
+        _ = uc.uni.unichr(TypeError)  # type: ignore[arg-type]
 
 def test_uni_bidirectional():
     assert uc.uni.bidirectional('B') == 'L'
     assert uc.uni.bidirectional('\u05D0') == 'R'  # HEBREW LETTER ALEF
 
+def test_uni_block():
+    assert uc.uni.block('\u00E5') == 'Latin-1 Supplement'
+
 def test_uni_category():
     assert uc.uni.category('B') == 'Lu'
     assert uc.uni.category('\u05D0') == 'Lo'  # HEBREW LETTER ALEF
 
 def test_uni_combining():
     assert uc.uni.combining('B') == 0
     # COMBINING DIAERESIS
@@ -42,26 +45,43 @@
     assert uc.uni.decimal('B') is None
     assert uc.uni.decimal('0') == 0
     # MATHEMATICAL DOUBLE-STRUCK DIGIT THREE
     assert uc.uni.decimal('\U0001D7DB') == 3
     assert uc.uni.decimal('\U00002464') is None  # CIRCLED DIGIT FIVE
 
 def test_uni_decomposition():
-    assert uc.uni.decomposition('B') == ''
+    assert not uc.uni.decomposition('B')
     # LATIN SMALL LETTER E WITH ACUTE
     # → LATIN SMALL LETTER E, COMBINING ACUTE ACCENT
     assert uc.uni.decomposition('\u00E9') == '0065 0301'
 
 def test_uni_digit():
     assert uc.uni.digit('B') is None
     assert uc.uni.digit('0') == 0
     # MATHEMATICAL DOUBLE-STRUCK DIGIT THREE
     assert uc.uni.digit('\U0001D7DB') == 3
     assert uc.uni.digit('\U00002464') == 5  # CIRCLED DIGIT FIVE
 
+def test_uni_hexadecimal():
+    assert uc.uni.hexadecimal('\u00E2') == '00E2'
+    assert uc.uni.hexadecimal('\U0001D53B') == '1D53B'
+
+def test_uni_identifier():
+    assert (uc.uni.identifier('\U0001D53C') ==
+            'MATHEMATICAL_DOUBLE_STRUCK_CAPITAL_E')
+    assert uc.uni.identifier('\U00101234', 'Default') == 'Default'
+
+def test_uni_east_asian_width():
+    assert uc.uni.east_asian_width('B') == 'Na'
+    assert uc.uni.east_asian_width('\u05D0') == 'N'  # HEBREW LETTER ALEF
+    assert uc.uni.east_asian_width('\u0308') == 'A'  # COMBINING DIAERESIS
+    assert uc.uni.east_asian_width('\u30A6') == 'W'  # KATAKANA LETTER U
+    assert uc.uni.east_asian_width('\uFF21') == 'F'  # FULLWIDTH LATIN CAPITAL A
+    assert uc.uni.east_asian_width('\uFF73') == 'H'  # HALFWIDTH KATAKANA U
+
 def test_uni_mirrored():
     assert uc.uni.mirrored('B') == 0
     assert uc.uni.mirrored('(') == 1
 
 def test_uni_name():
     assert uc.uni.name('B') == 'LATIN CAPITAL LETTER B'
     assert uc.uni.name('\U00101234') == 'U+101234'
@@ -81,36 +101,46 @@
     # LATIN CAPITAL LETTER DZ WITH CARON → D, LATIN CAPITAL LETTER Z WITH CARON
     assert uc.uni.nfkc('\u01C4') == 'D\u017D'
     assert uc.uni.normalize('\u01C4', 'nfkc') == 'D\u017D'
 
 def test_uni_nfd():
     assert uc.uni.nfd('B') == 'B'
     assert uc.uni.normalize('B', 'nfd') == 'B'
-    # LATIN CAPITAL LETTER A WITH GRAVE → A, COMBINING GRAVE ACCENT
+    # LATIN CAPITAL LETTER A WITH GRAVE → A, COMBINING GRAVE ACCENT
     assert uc.uni.nfd('\u00C0') == 'A\u0300'
     assert uc.uni.normalize('\u00C0', 'nfd') == 'A\u0300'
 
 def test_uni_nfkd():
     assert uc.uni.nfkd('B') == 'B'
     assert uc.uni.normalize('B', 'nfkd') == 'B'
-    # LATIN CAPITAL LETTER DZ WITH CARON → D, Z, COMBINING CARON
+    # LATIN CAPITAL LETTER DZ WITH CARON → D, Z, COMBINING CARON
     assert uc.uni.nfkd('\u01C4') == 'DZ\u030C'
     assert uc.uni.normalize('\u01C4', 'nfkd') == 'DZ\u030C'
 
 def test_uni_numeric():
     assert uc.uni.numeric('B') is None
     assert uc.uni.numeric('0') == 0
     # MATHEMATICAL DOUBLE-STRUCK DIGIT THREE
     assert uc.uni.numeric('\U0001D7DB') == 3
     assert uc.uni.numeric('\U00002464') == 5  # CIRCLED DIGIT FIVE
     assert uc.uni.numeric('\u00BC') == 0.25  # VULGAR FRACTION ONE QUARTER
 
 def test_uni_ordinal():
     assert uc.uni.ordinal('B') == 66
 
+def test_uni_utf8():
+    assert uc.uni.utf8('B') == [66]
+    assert uc.uni.utf8('\u00E0') == [195, 160]
+    assert uc.uni.utf8('\u30A6') == [0xE3, 0x82, 0xA6]
+
+def test_uni_utf16():
+    assert uc.uni.utf16('B') == [66]
+    assert uc.uni.utf16('\U0001D538') == [55349, 56632]
+    assert not uc.uni.utf16('\uD838')
+
 def test_uni_width():
     assert uc.uni.width('B') == 'Na'
     assert uc.uni.width('\u05D0') == 'N'  # HEBREW LETTER ALEF
     assert uc.uni.width('\u0308') == 'A'  # COMBINING DIAERESIS
     assert uc.uni.width('\u30A6') == 'W'  # KATAKANA LETTER U
     assert uc.uni.width('\uFF21') == 'F'  # FULLWIDTH LATIN CAPITAL LETTER A
     assert uc.uni.width('\uFF73') == 'H'  # HALFWIDTH KATAKANA LETTER U
```

### Comparing `unicode-name-inquiry-1.9.1/src/uc/uni.py` & `unicode-name-inquiry-1.9.2/src/uc/uni.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # SPDX-License-Identifier: MIT
-
-from collections.abc import Callable
-from typing import Any
+"""Character conversions and properties."""
 
 import unicodedata
 
+from collections.abc import Callable, Sequence
+from typing import Any, TypeVar
+
+import uc.block
+
+T = TypeVar('T')
+
 # Conversion
 
 def unichr(value: int | str) -> str:
-    """Converts an integer, character, or Unicode name to character."""
+    """Convert an integer, character, or Unicode name to character."""
     if isinstance(value, int):
         return chr(value)
 
     if not isinstance(value, str):
-        raise TypeError(f'{value} is not str or int')
+        message = f'{value} is not str or int'
+        raise TypeError(message)
 
     # Now we have a str.
     if len(value) == 1:
         return value
 
     # Check for a string that represents an integer.
     try:
@@ -35,71 +41,116 @@
     if value.lower()[0] == 'u':
         i = value[1 :]
         if i[0] == '+':
             i = i[1 :]
         # Let this raise ValueError.
         return chr(int(i, 16))
 
-    raise ValueError(f'No character {repr(value)}')
+    message = f'No character {value!r}'
+    raise ValueError(message)
+
+def utf32to16(n: int) -> Sequence[int]:
+    """Convert a number to a list holding its UTF-16 encoding."""
+    if (n <= 0xD7FF) or (0xE000 <= n <= 0xFFFF):
+        return [n]
+    if n < 0x10000 or n > 0x10FFFF:
+        return []
+    n = n - 0x10000
+    return [0xD800 + (n >> 10), 0xDC00 + (n & 0x3FF)]
+
+def utf32to8(n: int) -> Sequence[int]:
+    """Convert a number to a list holding its UTF-8 encoding."""
+    if n < 0x80:
+        return [n]
+    r = []
+    m = 0x1F
+    while True:
+        r.append(0x80 | (n & 0x3F))
+        n = n >> 6
+        if n & m == n:
+            break
+        m = m >> 1
+    r.append((0xFE ^ (m << 1)) | n)
+    r.reverse()
+    return r
 
 # Normalization
 
-def normalize(c: str, form) -> str:
+def normalize(c: str, form: str) -> str:
     # NB: character first.
     return unicodedata.normalize(form.upper(), c)
 
 # Uniform property access functions. These all accept a ‘default’ argument,
 # even though in many cases it is not used.
 
 PropertyAccessFunction = Callable[[str, Any | None], Any]
 
 PROPERTIES: dict[str, PropertyAccessFunction] = {}
 
-def register(v: dict):
+def register(v: dict) -> Callable:
 
-    def decorator(fn):
+    def decorator(fn: Callable) -> Callable:
         v[fn.__name__] = fn
         return fn
 
     return decorator
 
 @register(PROPERTIES)
 def bidirectional(c: str, _=None) -> str:
     return unicodedata.bidirectional(c)
 
 @register(PROPERTIES)
+def block(c: str, _=None) -> str:
+    return uc.block.block(ord(c))[1]
+
+@register(PROPERTIES)
 def category(c: str, _=None) -> str:
     return unicodedata.category(c)
 
 @register(PROPERTIES)
+def char(c: str, _=None) -> str:
+    return c
+
+@register(PROPERTIES)
 def combining(c: str, _=None) -> int:
     return unicodedata.combining(c)
 
 @register(PROPERTIES)
-def decimal(c: str, default=None):
+def decimal(c: str, default: T | None = None) -> int | T | None:
     return unicodedata.decimal(c, default)
 
 @register(PROPERTIES)
 def decomposition(c: str, _=None) -> str:
     return unicodedata.decomposition(c)
 
 @register(PROPERTIES)
-def digit(c: str, default=None):
+def digit(c: str, default: T | None = None) -> int | T | None:
     return unicodedata.digit(c, default)
 
 @register(PROPERTIES)
-def east_asian_width(c: str, _=None):
+def east_asian_width(c: str, _=None) -> str:
     return width(c)
 
 @register(PROPERTIES)
+def hexadecimal(c: str, _=None, digits: int = 4) -> str:
+    return f'{ord(c):0{digits}X}'
+
+@register(PROPERTIES)
+def identifier(c: str, default: T | None = None) -> str | T | None:
+    try:
+        return unicodedata.name(c).replace(' ', '_').replace('-', '_')
+    except ValueError:
+        return default
+
+@register(PROPERTIES)
 def mirrored(c: str, _=None) -> int:
     return unicodedata.mirrored(c)
 
 @register(PROPERTIES)
-def name(c: str, default=None) -> str:
+def name(c: str, default: T | None = None) -> str | T:
     try:
         return unicodedata.name(c)
     except ValueError:
         if default is not None:
             return default
         return f'U+{ord(c):04X}'
 
@@ -116,17 +167,29 @@
     return unicodedata.normalize('NFD', c)
 
 @register(PROPERTIES)
 def nfkd(c: str, _=None) -> str:
     return unicodedata.normalize('NFKD', c)
 
 @register(PROPERTIES)
-def numeric(c: str, default=None):
+def numeric(c: str, default: T | None = None) -> float | T | None:
     return unicodedata.numeric(c, default)
 
 @register(PROPERTIES)
 def ordinal(c: str, _=None) -> int:
     return ord(c)
 
 @register(PROPERTIES)
-def width(c: str, _=None):
+def u(c: str, _=None, digits: int = 4) -> str:
+    return f'U+{ord(c):0{digits}X}'
+
+@register(PROPERTIES)
+def utf8(c: str, _=None) -> Sequence[int]:
+    return utf32to8(ord(c))
+
+@register(PROPERTIES)
+def utf16(c: str, _=None) -> Sequence[int]:
+    return utf32to16(ord(c))
+
+@register(PROPERTIES)
+def width(c: str, _=None) -> str:
     return unicodedata.east_asian_width(c)
```

### Comparing `unicode-name-inquiry-1.9.1/src/uni.py` & `unicode-name-inquiry-1.9.2/src/uni.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 #!/usr/bin/env python
 # SPDX-License-Identifier: MIT
+"""`uni` command."""
 
 import argparse
 import itertools
 import pathlib
 import sys
 
 from collections.abc import Iterable
 
-import uc.uni
 import uc.block
 import uc.format
 import uc.search
+import uc.uni
 
 SELF = 'uni'
 error_count = 0
 
-def error(s):
-    global error_count
+def error(s: str) -> None:
+    global error_count  # noqa: PLW0603
     error_count += 1
     print(f'{SELF}: {s}', file=sys.stderr)
 
-def unichr_e(value) -> str | None:
+def unichr_e(value: int | str) -> str | None:
     try:
         return uc.uni.unichr(value)
     except ValueError:
-        error(f'No character {repr(value)}')
+        error(f'No character {value!r}')
         return None
 
 def unicode_points(
         blocks: Iterable[uc.block.UniBlock] | None = None) -> Iterable[int]:
-    """Returns a sequence of all Unicode points in the blocks."""
+    """Return a sequence of all Unicode points in the blocks."""
     if blocks:
-        source: Iterable[int] = itertools.chain.from_iterable(
-            (b.range for b in blocks))
-    else:
-        source = range(sys.maxunicode + 1)
-    return source
+        return itertools.chain.from_iterable(b.range for b in blocks)
+    return range(sys.maxunicode + 1)
 
 def unicode_chars(
         blocks: Iterable[uc.block.UniBlock] | None = None) -> Iterable[str]:
-    """Returns a map of all Unicode character names in the blocks."""
+    """Return a map of all Unicode character names in the blocks."""
     return (chr(i) for i in unicode_points(blocks))
 
 CANNED_FORMATS = {
     'char': ('print the character', '{char}'),
     'name': ('print the character name', '{name}'),
     'short': ('print the character, code, and name', '{char} {u} {name}'),
     'long': ('print full details about the character',
@@ -77,20 +75,21 @@
     'decomposition',
     'digit',
     'mirrored',
     'numeric',
     'width',
 )
 
-def main(argv: list[str] | None = None):
+def main(argv: list[str] | None = None) -> int:  # noqa: C901, PLR0912, PLR0915
     if argv is None:
         argv = sys.argv  # pragma: no cover
-    global SELF
+
+    global SELF  # noqa: PLW0603
     SELF = pathlib.Path(argv[0]).stem
-    global error_count
+    global error_count  # noqa: PLW0603
     error_count = 0
 
     parser = argparse.ArgumentParser(prog=SELF)
     search_group = parser.add_argument_group('search options')
     anyall = search_group.add_mutually_exclusive_group()
     anyall.add_argument(
         '--all',
@@ -175,52 +174,57 @@
 
     parser.add_argument(
         'character',
         nargs=argparse.REMAINDER,
         help='character, name, or search pattern')
     args = parser.parse_args(argv[1 :])
 
+    # Collect character property selections.
     props = []
     for p in PROPS:
         if (pp := getattr(args, p, [])):
             for v in pp:
                 props.append((p, v))
 
+    # Collect unicode block selections.
     blocks = []
     if args.block is not None:
         for b in args.block:
             try:
                 blocks.append(uc.block.UniBlock(b))
             except ValueError as e:
                 error(e)
                 return error_count
 
+    # Find matching characters.
     chrs: Iterable[str]
     if args.character:
         if args.search:
             chrs = uc.search.search_name(args.search, args.character,
                                          unicode_chars(blocks), args.fold)
         else:
             cc = (unichr_e(name) for name in args.character)
             chrs = (
                 c for c in cc
-                if c and ((any((c in b for b in blocks)) if blocks else True)))
+                if c and (any(c in b for b in blocks) if blocks else True))
     elif blocks:
         chrs = unicode_chars(blocks)
     elif props:
         chrs = unicode_chars()
     else:
         parser.print_help()
         return 1
 
+    # Limit matching characters by character property selections.
     if props:
         chrs = (
             c for c in chrs if args.fold(
                 str(uc.uni.PROPERTIES[p](c, '')) == v for p, v in props))
 
+    # Report results.
     if not args.format:
         args.format = [CANNED_FORMATS['short'][1]]
     sep = False
     for c in chrs:
         if sep:
             print(end=args.eol)
         sep = True
```

### Comparing `unicode-name-inquiry-1.9.1/src/unicode_name_inquiry.egg-info/PKG-INFO` & `unicode-name-inquiry-1.9.2/src/unicode_name_inquiry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicode-name-inquiry
-Version: 1.9.1
+Version: 1.9.2
 Summary: Command-line tool to display Unicode character information
 License: MIT License
 Project-URL: repository, https://codeberg.org/datatravelandexperiments/uni
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `unicode-name-inquiry-1.9.1/src/unicode_name_inquiry.egg-info/SOURCES.txt` & `unicode-name-inquiry-1.9.2/src/unicode_name_inquiry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

