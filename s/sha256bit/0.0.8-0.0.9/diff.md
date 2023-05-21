# Comparing `tmp/sha256bit-0.0.8.tar.gz` & `tmp/sha256bit-0.0.9.tar.gz`

## Comparing `sha256bit-0.0.8.tar` & `sha256bit-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 sha256bit-0.0.8/publish_to_pypi
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 sha256bit-0.0.8/requirements.txt
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sha256bit-0.0.8/.github/workflows/build.yml
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 sha256bit-0.0.8/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 sha256bit-0.0.8/.github/workflows/test.yml
--rw-r--r--   0        0        0     6929 2020-02-02 00:00:00.000000 sha256bit-0.0.8/sha256bit/__init__.py
--rwxr-xr-x   0        0        0  3364551 2020-02-02 00:00:00.000000 sha256bit-0.0.8/test/SHA256LongMsg.rsp
--rwxr-xr-x   0        0        0    80540 2020-02-02 00:00:00.000000 sha256bit-0.0.8/test/SHA256ShortMsg.rsp
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 sha256bit-0.0.8/test/__init__.py
--rw-r--r--   0        0        0     5486 2020-02-02 00:00:00.000000 sha256bit-0.0.8/test/test.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 sha256bit-0.0.8/test/test_api.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 sha256bit-0.0.8/test/test_cavp.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 sha256bit-0.0.8/test/test_hardcoded.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sha256bit-0.0.8/test/test_vs_hashlib.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sha256bit-0.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sha256bit-0.0.8/LICENSE
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 sha256bit-0.0.8/README.md
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 sha256bit-0.0.8/hatch.toml
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 sha256bit-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 sha256bit-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 sha256bit-0.0.9/build
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 sha256bit-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sha256bit-0.0.9/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 sha256bit-0.0.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 sha256bit-0.0.9/sha256bit/__init__.py
+-rwxr-xr-x   0        0        0  3364551 2020-02-02 00:00:00.000000 sha256bit-0.0.9/test/SHA256LongMsg.rsp
+-rwxr-xr-x   0        0        0    80540 2020-02-02 00:00:00.000000 sha256bit-0.0.9/test/SHA256ShortMsg.rsp
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 sha256bit-0.0.9/test/__init__.py
+-rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 sha256bit-0.0.9/test/test.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 sha256bit-0.0.9/test/test_api.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 sha256bit-0.0.9/test/test_cavp.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 sha256bit-0.0.9/test/test_hardcoded.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sha256bit-0.0.9/test/test_vs_hashlib.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sha256bit-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sha256bit-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 sha256bit-0.0.9/README.md
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 sha256bit-0.0.9/hatch.toml
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 sha256bit-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 sha256bit-0.0.9/PKG-INFO
```

### Comparing `sha256bit-0.0.8/.github/workflows/build.yml` & `sha256bit-0.0.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.8/.github/workflows/python-package.yml` & `sha256bit-0.0.9/.github/workflows/test.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,49 @@
-# This workflow will install Python dependencies, run tests and lint with a variety of Python versions
-# For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
-
-name: Python package
+name: test
 
 on:
-  #push:
-  #  branches: [ "main" ]
+  push:
+    branches:
+    - main
   pull_request:
-    branches: [ "main" ]
+    branches:
+    - main
 
-jobs:
-  build:
+concurrency:
+  group: test-${{ github.head_ref }}
+  cancel-in-progress: true
+
+env:
+  PYTHONUNBUFFERED: "1"
+  FORCE_COLOR: "1"
 
-    runs-on: ubuntu-latest
+jobs:
+  run:
+    name: Python ${{ matrix.python-version }} on ${{ startsWith(matrix.os, 'macos-') && 'macOS' || startsWith(matrix.os, 'windows-') && 'Windows' || 'Linux' }}
+    runs-on: ${{ matrix.os }}
     strategy:
-      fail-fast: true
+      fail-fast: false
       matrix:
-        python-version: ["3.10", "3.11"]
+      #  os: [ubuntu-latest, windows-latest, macos-latest]
+        os: [ubuntu-latest]
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
 
     steps:
     - uses: actions/checkout@v3
+
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
+
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install flake8 pytest hatch build
+        python -m pip install hatch build
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
-    - name: Lint with flake8
-      run: |
-        # stop the build if there are Python syntax errors or undefined names
-        flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
-        # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
-        flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
-    - name: Test with pytest
-      run: |
-        pytest
-    - name: Build
-      run: |
-        python -m build
+
+    - if: matrix.python-version == '3.11' && runner.os == 'Linux'
+      name: Lint
+      run: hatch run lint:all
+
+    - name: Run tests
+      run: hatch run cov
```

### Comparing `sha256bit-0.0.8/sha256bit/__init__.py` & `sha256bit-0.0.9/sha256bit/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import binascii
 import copy
 import struct
 
 
-class sha256bit:
+class Sha256bit:
     F32 = 0xFFFFFFFF
 
     _k = [
         0x428A2F98,
         0x71374491,
         0xB5C0FBCF,
         0xE9B5DBA5,
@@ -82,15 +82,15 @@
         0x9B05688C,
         0x1F83D9AB,
         0x5BE0CD19,
     ]
 
     @staticmethod
     def _rotr(x, y):
-        return ((x >> y) | (x << (32 - y))) & sha256bit.F32
+        return ((x >> y) | (x << (32 - y))) & Sha256bit.F32
 
     @staticmethod
     def _maj(x, y, z):
         return (x & y) ^ (x & z) ^ (y & z)
 
     @staticmethod
     def _ch(x, y, z):
@@ -103,15 +103,15 @@
 
     def __init__(self, m=None, *, bitlen=None):
         """SHA-256 implementation supporting bit granularity for message input length.
         API is the same as hashlib.
         """
         self._counter = 0
         self._cache = bytearray()
-        self._h = copy.deepcopy(sha256bit._h_init)
+        self._h = copy.deepcopy(Sha256bit._h_init)
         self._has_bitlen = False
         self._digest = None
         self.update(m, bitlen=bitlen)
 
     def export_state(self):
         if self._digest is None:
             h = self._h
@@ -119,15 +119,15 @@
         else:
             h = self._digest
             c = None
         return {'h': h, 'cnt': self._counter, 'cache': c}
 
     @staticmethod
     def import_state(state):
-        o = sha256bit()
+        o = Sha256bit()
         o._counter = state['cnt']
         if 0 != (o._counter % 8):
             o._has_bitlen = True
         if state['cache'] is None:
             o._digest = state['h']
             o._h = None
             o._cache = None
@@ -136,95 +136,100 @@
             o._cache = bytearray(state['cache'])
         return o
 
     def _compress(self, c):
         w = [0] * 64
         w[0:16] = struct.unpack('!16L', c)
         for i in range(16, 64):
-            s0 = sha256bit._rotr(w[i - 15], 7) ^ sha256bit._rotr(w[i - 15], 18) ^ (w[i - 15] >> 3)
-            s1 = sha256bit._rotr(w[i - 2], 17) ^ sha256bit._rotr(w[i - 2], 19) ^ (w[i - 2] >> 10)
-            w[i] = (w[i - 16] + s0 + w[i - 7] + s1) & sha256bit.F32
+            s0 = Sha256bit._rotr(w[i - 15], 7) ^ Sha256bit._rotr(w[i - 15], 18) ^ (w[i - 15] >> 3)
+            s1 = Sha256bit._rotr(w[i - 2], 17) ^ Sha256bit._rotr(w[i - 2], 19) ^ (w[i - 2] >> 10)
+            w[i] = (w[i - 16] + s0 + w[i - 7] + s1) & Sha256bit.F32
 
         a, b, c, d, e, f, g, h = self._h
 
         for i in range(64):
-            s0 = sha256bit._rotr(a, 2) ^ sha256bit._rotr(a, 13) ^ sha256bit._rotr(a, 22)
-            t2 = s0 + sha256bit._maj(a, b, c)
-            s1 = sha256bit._rotr(e, 6) ^ sha256bit._rotr(e, 11) ^ sha256bit._rotr(e, 25)
-            t1 = h + s1 + sha256bit._ch(e, f, g) + sha256bit._k[i] + w[i]
+            s0 = Sha256bit._rotr(a, 2) ^ Sha256bit._rotr(a, 13) ^ Sha256bit._rotr(a, 22)
+            t2 = s0 + Sha256bit._maj(a, b, c)
+            s1 = Sha256bit._rotr(e, 6) ^ Sha256bit._rotr(e, 11) ^ Sha256bit._rotr(e, 25)
+            t1 = h + s1 + Sha256bit._ch(e, f, g) + Sha256bit._k[i] + w[i]
 
             h = g
             g = f
             f = e
-            e = (d + t1) & sha256bit.F32
+            e = (d + t1) & Sha256bit.F32
             d = c
             c = b
             b = a
-            a = (t1 + t2) & sha256bit.F32
+            a = (t1 + t2) & Sha256bit.F32
 
         for i, (x, y) in enumerate(zip(self._h, [a, b, c, d, e, f, g, h])):
-            self._h[i] = (x + y) & sha256bit.F32
+            self._h[i] = (x + y) & Sha256bit.F32
 
     def update(self, m, *, bitlen=None):
         """Update the hash object with the bytes in data. Repeated calls
         are equivalent to a single call with the concatenation of all
         the arguments.
         """
         if not m:
             return
-        assert not self._has_bitlen, 'we support bitlen only for last call'
+        if self._has_bitlen:
+            raise AssertionError('we support bitlen only for last call')
+        bytes_bitlen = len(m) * 8
         if bitlen is not None:
             if 0 != (bitlen % 8):
                 self._has_bitlen = True
+                if bytes_bitlen - bitlen >= 8 or bitlen >= bytes_bitlen:
+                    raise AssertionError(
+                        'bitlen=%d, bytes_bitlen=%d'
+                        % (
+                            bitlen,
+                            bytes_bitlen,
+                        )
+                    )
             else:
-                assert bitlen == len(m) * 8, 'bitLen=%d, len(m)*8=%d' % (
-                    bitlen,
-                    len(m) * 8,
-                )
+                if bitlen != bytes_bitlen:
+                    raise AssertionError(
+                        'bitlen=%d, bytes_bitlen=%d'
+                        % (
+                            bitlen,
+                            bytes_bitlen,
+                        )
+                    )
             self._counter += bitlen
         else:
-            self._counter += len(m) * 8
+            self._counter += bytes_bitlen
 
         self._cache += m
 
         while len(self._cache) > 64:
             self._compress(self._cache[:64])
             self._cache = self._cache[64:]
 
-        if len(self._cache) == 64:
-            if 0 != (self._counter % 8):
-                assert self._has_bitlen
-                # at least one bit is issing to form a full block, nothing to do
-            else:
-                self._compress(self._cache[:64])
-                self._cache = self._cache[64:]
+        if len(self._cache) == 64 and 0 == (self._counter % 8):
+            self._compress(self._cache[:64])
+            self._cache = self._cache[64:]
 
     def _pad(self):
-        lastBlockBitLen = self._counter % 512
-        lastBlockFullBytesCnt = lastBlockBitLen // 8
-        if lastBlockBitLen < 448:
-            padlen = 55 - lastBlockFullBytesCnt
+        last_block_bitlen = self._counter % 512
+        last_block_full_bytes_cnt = last_block_bitlen // 8
+        if last_block_bitlen < 448:
+            padlen = 55 - last_block_full_bytes_cnt
         else:
-            padlen = 119 - lastBlockFullBytesCnt
-        if False:
-            print(lastBlockBitLen, lastBlockFullBytesCnt, padlen, len(self._cache))
+            padlen = 119 - last_block_full_bytes_cnt
 
         shift = self._counter % 8
         if shift > 0 and (len(self._cache) > 0):
             mask = 0xFF << (8 - shift)
             self._cache[-1] = (self._cache[-1] & mask) | (0x80 >> shift)
         else:
             self._cache += b'\x80'
         self._cache += (b'\x00' * padlen) + self._counter.to_bytes(8, byteorder='big')
-        if False:
-            from pysatl import Utils
 
-            print('counter=%d (0x%x)' % (self._counter, self._counter))
-            print(Utils.hexstr(self._cache))
-        assert len(self._cache) in [64, 128], 'len(self._cache)=%d' % len(self._cache)
+        if len(self._cache) not in [64, 128]:
+            raise AssertionError('len(self._cache)=%d' % len(self._cache))
 
     def digest(self):
         """Return the digest of the bytes passed to the update() method
         so far as a bytes object.
         """
         if self._digest is not None:
             return self._digest
```

### Comparing `sha256bit-0.0.8/test/SHA256LongMsg.rsp` & `sha256bit-0.0.9/test/SHA256LongMsg.rsp`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.8/test/SHA256ShortMsg.rsp` & `sha256bit-0.0.9/test/SHA256ShortMsg.rsp`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.8/test/test.py` & `sha256bit-0.0.9/test/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import hashlib
 import re
 
 from pysatl import Utils
 
-from sha256bit import sha256bit
+from sha256bit import Sha256bit
 
 
 def block_generator(seed, msg_bitlen):
     l2block = hashlib.sha256(seed).digest()
     l2block += hashlib.sha256(l2block).digest()
-    blockBitLen = len(l2block) * 8
-    assert blockBitLen == 64 * 8
+    block_bitlen = len(l2block) * 8
+    assert block_bitlen == 64 * 8
     bitlen = 0
-    while bitlen + blockBitLen < msg_bitlen:
+    while bitlen + block_bitlen < msg_bitlen:
         yield l2block
-        bitlen += blockBitLen
+        bitlen += block_bitlen
         l2block = hashlib.sha256(l2block).digest()
         l2block += hashlib.sha256(l2block).digest()
     # last block
-    lastBlockBitLen = msg_bitlen % 512
-    if 0 != lastBlockBitLen:
-        lastBlockFullByteLen = (lastBlockBitLen + 7) // 8
-        l2block = bytearray(l2block[0:lastBlockFullByteLen])
-        assert len(l2block) == lastBlockFullByteLen
+    last_block_bitlen = msg_bitlen % 512
+    if 0 != last_block_bitlen:
+        last_block_full_bytelen = (last_block_bitlen + 7) // 8
+        l2block = bytearray(l2block[0:last_block_full_bytelen])
+        assert len(l2block) == last_block_full_bytelen
         mask = 0xFF & (0xFF << (8 - (msg_bitlen % 8)))
         if 0 != mask:
             l2block[-1] &= mask
     yield l2block
 
 
 def msg_generator(seed, msg_bitlen):
@@ -35,48 +35,48 @@
         o += b
     return o
 
 
 def check_against_hashlib(n_seeds=3, max_length=1024 * 4):
     print('check against hashlib')
 
-    assert hashlib.sha256(b'abc').digest() == sha256bit(b'abc').digest()
+    assert hashlib.sha256(b'abc').digest() == Sha256bit(b'abc').digest()
 
     def check_against_hashlib(seed, msg_bitlen):
         expected = hashlib.sha256()
-        dut = sha256bit()
+        dut = Sha256bit()
         for block in block_generator(seed, msg_bitlen):
             # print(Utils.hexstr(block))
             expected.update(block)
             dut.update(block)
         assert expected.digest() == dut.digest()
 
-    for seedByte in range(0, n_seeds):
-        for msgBitLen in range(0, max_length, 8):
-            seed = bytearray([seedByte])
-            check_against_hashlib(seed, msgBitLen)
+    for seed_byte in range(0, n_seeds):
+        for msg_bitlen in range(0, max_length, 8):
+            seed = bytearray([seed_byte])
+            check_against_hashlib(seed, msg_bitlen)
 
 
 def check(msg, bitlen, sig):
-    m = sha256bit()
+    m = Sha256bit()
     if isinstance(msg, str):
         msg = msg.encode('ascii')
     descr = 'msg      = ' + Utils.hexstr(msg) + '\n'
     descr += 'bitlen   = %d\n' % bitlen
     descr += 'expected = ' + sig + '\n'
     try:
         m.update(msg, bitlen=bitlen)
         digest = m.hexdigest()
     except Exception as e:
         print(descr)
         raise e
-    errMsg = '\n'
-    errMsg += descr
-    errMsg += 'digest   = ' + digest + '\n'
-    assert digest == sig, errMsg
+    err_msg = '\n'
+    err_msg += descr
+    err_msg += 'digest   = ' + digest + '\n'
+    assert digest == sig, err_msg
 
 
 def check_hardcoded_test_vectors():
     print('check few minimal hardcoded test vectors')
 
     tests = [
         {
@@ -101,70 +101,70 @@
         },
     ]
 
     for test in tests:
         check(test['msg'], test['bitlen'], test['digest'])
 
     assert (
-        sha256bit(b'\x00', bitlen=1).hexdigest() == 'bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375'
+        Sha256bit(b'\x00', bitlen=1).hexdigest() == 'bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375'
     )
 
 
 def check_against_nist_cavp():
     print("check against 'short' and 'long' bit oriented test vectors from NIST CAVP")
     # (https://csrc.nist.gov/CSRC/media/Projects/Cryptographic-Algorithm-Validation-Program/documents/shs/shabittestvectors.zip)
 
     from pathlib import Path
 
     resource_path = Path(__file__).parent
-    for tvFile in ['SHA256ShortMsg.rsp', 'SHA256LongMsg.rsp']:
-        tvPath = resource_path.joinpath(tvFile)
-        with open(tvPath) as f:
+    for tv_file in ['SHA256ShortMsg.rsp', 'SHA256LongMsg.rsp']:
+        tv_path = resource_path.joinpath(tv_file)
+        with open(tv_path) as f:
             for line in f:
                 if line.startswith('Len'):
                     bitlen = int(re.search(r'Len = (.+)', line).group(1))
                 if line.startswith('Msg'):
                     msg = Utils.ba(re.search(r'Msg = (.+)', line).group(1))
                     if bitlen == 0:
                         msg = bytes(0)
                 if line.startswith('MD'):
-                    MD = re.search(r'MD = (.+)', line).group(1)
-                    check(msg, bitlen, MD)
+                    md = re.search(r'MD = (.+)', line).group(1)
+                    check(msg, bitlen, md)
 
 
 def check_api():
     print('check API')
     msg = msg_generator(bytes(0), 300 * 8)
     expected = hashlib.sha256(msg).digest()
     # print(Utils.hexstr(msg))
     # print(Utils.hexstr(expected))
-    assert expected == sha256bit(msg).digest()
+    assert expected == Sha256bit(msg).digest()
     for len1 in range(0, len(msg) * 8):
-        dut1 = sha256bit()
+        dut1 = Sha256bit()
         dut1.update(msg[:len1])
         state = dut1.export_state()
-        dut2 = sha256bit.import_state(state)
+        dut2 = Sha256bit.import_state(state)
         dut2.update(msg[len1:])
         assert expected == dut2.digest()
     for len1 in range(1, len(msg) * 8):
-        dut = sha256bit()
+        dut = Sha256bit()
         remaining = len(msg)
         p = 0
         while remaining > 0:
             chunk = msg[p : p + len1]
             dut.update(chunk, bitlen=len(chunk) * 8)
             p += len1
             remaining -= len1
         assert expected == dut.digest()
         state = dut.export_state()
-        dut2 = sha256bit.import_state(state)
+        dut2 = Sha256bit.import_state(state)
         assert expected == dut2.digest()
-    dut = sha256bit(b'\x00', bitlen=1)
+    dut = Sha256bit(b'\x00', bitlen=1)
     state = dut.export_state()
-    dut2 = sha256bit.import_state(state)
+    dut2 = Sha256bit.import_state(state)
     assert dut2.hexdigest() == 'bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375'
 
 
 if __name__ == '__main__':
     check_api()
     check_hardcoded_test_vectors()
     check_against_nist_cavp()
```

### Comparing `sha256bit-0.0.8/.gitignore` & `sha256bit-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.8/LICENSE` & `sha256bit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.8/README.md` & `sha256bit-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # sha256bit
 
 
 | | |
 | --- | --- |
 | CI/CD | [![CI - Test](https://github.com/sebastien-riou/sha256bit/actions/workflows/test.yml/badge.svg)](https://github.com/sebastien-riou/sha256bit/actions/workflows/test.yml) [![CD - Build](https://github.com/sebastien-riou/sha256bit/actions/workflows/build.yml/badge.svg)](https://github.com/sebastien-riou/sha256bit/actions/workflows/build.yml) |
-| Package | [![PyPI - Version](https://img.shields.io/pypi/v/sha256bit.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/sha256bits/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hsha256bit.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/sha256bit/) |
-| Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) |
+| Package | [![PyPI - Version](https://img.shields.io/pypi/v/sha256bit.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/sha256bits/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sha256bit.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/sha256bit/) |
+| Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)  [![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/ambv/black) [![License - apache-2.0](https://img.shields.io/badge/license-apache--2.0-blue)](https://spdx.org/licenses/) |
 
 
 Pure python implementation of SHA256 with features which are often lacking:
 - bit granularity for message input length
 - import/export API to "persist" the state in the middle of a hash computation
 
 ## Installation
 
     python3 -m pip install sha256bit
 
 ## Usage
 
 ### One liner 
 
-    >>> from sha256bit import sha256bit
-    >>> sha256bit("abc".encode()).hexdigest()
+    >>> from sha256bit import Sha256bit
+    >>> Sha256bit("abc".encode()).hexdigest()
     'ba7816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015ad'
 
 ### Bit length capability
 
-    >>> from sha256bit import sha256bit
-    >>> sha256bit(b'\x00',bitlen=1).hexdigest()
+    >>> from sha256bit import Sha256bit
+    >>> Sha256bit(b'\x00',bitlen=1).hexdigest()
     'bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375'
 
 ### Import/export
 
-    >>> from sha256bit import sha256bit
-    >>> h1 = sha256bit("a".encode())
+    >>> from sha256bit import Sha256bit
+    >>> h1 = Sha256bit("a".encode())
     >>> state = h1.export_state()
-    >>> h2 = sha256bit.import_state(state)
+    >>> h2 = Sha256bit.import_state(state)
     >>> h2.update("bc".encode())
     >>> h2.hexdigest()
     'ba7816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015ad'
 
 ## Test with `pytest`
 
     pytest-3
@@ -54,14 +54,14 @@
 
     python3 -m test.test_api
     python3 -m test.test_cavp
     python3 -m test.test_hardcoded
     python3 -m test.test_vs_hashlib
 
 ## Build the package
-Build is done using `hatchling`
+Build is done using `hatchling`. The script `build` allows to build for different version of python3:
 
-    python3 -m build
+    ./build python3.9
 
 
 ## Create a new version
 Version is managed by `hatch-vcs`, you just need to create a tag in github.
```

### Comparing `sha256bit-0.0.8/hatch.toml` & `sha256bit-0.0.9/hatch.toml`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.8/pyproject.toml` & `sha256bit-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,16 @@
 [tool.ruff.flake8-quotes]
 inline-quotes = "single"
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
-# Tests can use relative imports and assertions
-"test/**/*" = ["TID252", "S101"]
+# Tests can use relative imports and assertions and print
+"test/**/*" = ["TID252", "S101", "T201"]
 
 [tool.mypy]
 disallow_untyped_defs = false
 follow_imports = "normal"
 ignore_missing_imports = true
 pretty = true
 show_column_numbers = true
```

### Comparing `sha256bit-0.0.8/PKG-INFO` & `sha256bit-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sha256bit
-Version: 0.0.8
+Version: 0.0.9
 Summary: SHA256 with bit granularity for message input length
 Project-URL: Homepage, https://github.com/sebastien-riou/sha256bit
 Project-URL: Bug Tracker, https://github.com/sebastien-riou/sha256bit/issues
 Author: Sebastien Riou
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -23,46 +23,46 @@
 
 # sha256bit
 
 
 | | |
 | --- | --- |
 | CI/CD | [![CI - Test](https://github.com/sebastien-riou/sha256bit/actions/workflows/test.yml/badge.svg)](https://github.com/sebastien-riou/sha256bit/actions/workflows/test.yml) [![CD - Build](https://github.com/sebastien-riou/sha256bit/actions/workflows/build.yml/badge.svg)](https://github.com/sebastien-riou/sha256bit/actions/workflows/build.yml) |
-| Package | [![PyPI - Version](https://img.shields.io/pypi/v/sha256bit.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/sha256bits/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hsha256bit.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/sha256bit/) |
-| Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) |
+| Package | [![PyPI - Version](https://img.shields.io/pypi/v/sha256bit.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/sha256bits/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sha256bit.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/sha256bit/) |
+| Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)  [![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/ambv/black) [![License - apache-2.0](https://img.shields.io/badge/license-apache--2.0-blue)](https://spdx.org/licenses/) |
 
 
 Pure python implementation of SHA256 with features which are often lacking:
 - bit granularity for message input length
 - import/export API to "persist" the state in the middle of a hash computation
 
 ## Installation
 
     python3 -m pip install sha256bit
 
 ## Usage
 
 ### One liner 
 
-    >>> from sha256bit import sha256bit
-    >>> sha256bit("abc".encode()).hexdigest()
+    >>> from sha256bit import Sha256bit
+    >>> Sha256bit("abc".encode()).hexdigest()
     'ba7816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015ad'
 
 ### Bit length capability
 
-    >>> from sha256bit import sha256bit
-    >>> sha256bit(b'\x00',bitlen=1).hexdigest()
+    >>> from sha256bit import Sha256bit
+    >>> Sha256bit(b'\x00',bitlen=1).hexdigest()
     'bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375'
 
 ### Import/export
 
-    >>> from sha256bit import sha256bit
-    >>> h1 = sha256bit("a".encode())
+    >>> from sha256bit import Sha256bit
+    >>> h1 = Sha256bit("a".encode())
     >>> state = h1.export_state()
-    >>> h2 = sha256bit.import_state(state)
+    >>> h2 = Sha256bit.import_state(state)
     >>> h2.update("bc".encode())
     >>> h2.hexdigest()
     'ba7816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015ad'
 
 ## Test with `pytest`
 
     pytest-3
@@ -77,14 +77,14 @@
 
     python3 -m test.test_api
     python3 -m test.test_cavp
     python3 -m test.test_hardcoded
     python3 -m test.test_vs_hashlib
 
 ## Build the package
-Build is done using `hatchling`
+Build is done using `hatchling`. The script `build` allows to build for different version of python3:
 
-    python3 -m build
+    ./build python3.9
 
 
 ## Create a new version
 Version is managed by `hatch-vcs`, you just need to create a tag in github.
```

