# Comparing `tmp/ever_playground-0.5.0.tar.gz` & `tmp/ever_playground-0.6.1.tar.gz`

## Comparing `ever_playground-0.5.0.tar` & `ever_playground-0.6.1.tar`

### file list

```diff
@@ -1,17 +1,28 @@
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 ever_playground-0.5.0/Cargo.toml
--rw-rw-r--   0     1000     1000       78 2023-05-15 13:10:44.000000 ever_playground-0.5.0/.gitignore
--rw-rw-r--   0     1000     1000      181 2023-05-12 14:44:59.000000 ever_playground-0.5.0/.vscode/settings.json
--rw-rw-r--   0     1000     1000      566 2023-05-17 11:44:03.000000 ever_playground-0.5.0/README.md
--rw-rw-r--   0     1000     1000     4015 2023-05-19 19:14:08.000000 ever_playground-0.5.0/ever_playground/__init__.py
--rw-rw-r--   0     1000     1000     4917 2023-05-19 18:26:44.000000 ever_playground-0.5.0/ever_playground/ever_playground.pyi
--rw-rw-r--   0     1000     1000     2244 2023-05-19 14:55:11.000000 ever_playground-0.5.0/examples/basics.py
--rw-rw-r--   0     1000     1000     1874 2023-05-19 15:59:34.000000 ever_playground-0.5.0/examples/recover-stake.py
--rw-rw-r--   0     1000     1000     2331 2023-05-19 14:55:00.000000 ever_playground-0.5.0/examples/runvm.py
--rw-rw-r--   0     1000     1000     2919 2023-05-19 19:15:04.000000 ever_playground-0.5.0/examples/testgiver.py
--rw-rw-r--   0     1000     1000     3601 2023-05-19 15:12:42.000000 ever_playground-0.5.0/examples/validator-elect-req.py
--rw-rw-r--   0     1000     1000      946 2023-05-17 10:02:52.000000 ever_playground-0.5.0/pyproject.toml
--rw-rw-r--   0     1000     1000    15132 2023-05-19 18:27:17.000000 ever_playground-0.5.0/src/lib.rs
--rw-rw-r--   0     1000     1000     1064 2023-05-11 14:01:16.000000 ever_playground-0.5.0/src/tests.rs
--rw-rw-r--   0     1000     1000     3689 2023-05-15 14:26:56.000000 ever_playground-0.5.0/src/utils.rs
--rw-rw-r--   0     1000     1000    24701 2023-05-19 19:17:35.000000 ever_playground-0.5.0/Cargo.lock
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 ever_playground-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 ever_playground-0.6.1/Cargo.toml
+-rw-rw-r--   0     1000     1000       78 2023-05-15 13:10:44.000000 ever_playground-0.6.1/.gitignore
+-rw-rw-r--   0     1000     1000      181 2023-05-12 14:44:59.000000 ever_playground-0.6.1/.vscode/settings.json
+-rw-rw-r--   0     1000     1000      566 2023-05-17 11:44:03.000000 ever_playground-0.6.1/README.md
+-rw-rw-r--   0     1000     1000     4831 2023-05-22 11:02:08.000000 ever_playground-0.6.1/ever_playground/__init__.py
+-rw-rw-r--   0     1000     1000     5944 2023-05-22 15:35:59.000000 ever_playground-0.6.1/ever_playground/ever_playground.pyi
+-rw-rw-r--   0     1000     1000     2245 2023-05-22 13:02:10.000000 ever_playground-0.6.1/examples/basics.py
+-rw-rw-r--   0     1000     1000      836 2023-05-22 14:54:56.000000 ever_playground-0.6.1/examples/highload/generate.fif
+-rwxrwxr-x   0     1000     1000     3399 2023-05-22 16:05:31.000000 ever_playground-0.6.1/examples/highload/highload-wallet-v2.fif
+-rw-rw-r--   0     1000     1000     4689 2023-05-22 16:05:26.000000 ever_playground-0.6.1/examples/highload/highload-wallet-v2.py
+-rw-------   0     1000     1000      180 2023-05-22 14:37:50.000000 ever_playground-0.6.1/examples/highload/order-list-fift
+-rw-------   0     1000     1000      234 2023-05-22 14:54:59.000000 ever_playground-0.6.1/examples/highload/order-list-py
+-rw-------   0     1000     1000       32 2023-05-22 14:37:50.000000 ever_playground-0.6.1/examples/highload/sample.pk
+-rw-------   0     1000     1000       36 2023-05-22 14:37:50.000000 ever_playground-0.6.1/examples/highload/sample27172.addr
+-rwxrwxr-x   0     1000     1000      870 2023-05-22 16:19:06.000000 ever_playground-0.6.1/examples/recover-stake.fif
+-rw-rw-r--   0     1000     1000     1889 2023-05-22 16:19:27.000000 ever_playground-0.6.1/examples/recover-stake.py
+-rw-rw-r--   0     1000     1000     2327 2023-05-22 13:04:32.000000 ever_playground-0.6.1/examples/runvm.py
+-rwxrwxr-x   0     1000     1000     1187 2023-05-22 11:04:24.000000 ever_playground-0.6.1/examples/testgiver.fif
+-rw-rw-r--   0     1000     1000     2902 2023-05-22 11:25:27.000000 ever_playground-0.6.1/examples/testgiver.py
+-rwxrwxr-x   0     1000     1000     1645 2023-05-22 12:49:48.000000 ever_playground-0.6.1/examples/validator-elect-req.fif
+-rw-rw-r--   0     1000     1000     3607 2023-05-20 15:28:34.000000 ever_playground-0.6.1/examples/validator-elect-req.py
+-rw-rw-r--   0     1000     1000      946 2023-05-17 10:02:52.000000 ever_playground-0.6.1/pyproject.toml
+-rwxrwxr-x   0     1000     1000     2879 2023-05-22 16:19:13.000000 ever_playground-0.6.1/run-examples.py
+-rw-rw-r--   0     1000     1000    18118 2023-05-22 15:37:09.000000 ever_playground-0.6.1/src/lib.rs
+-rw-rw-r--   0     1000     1000     1064 2023-05-11 14:01:16.000000 ever_playground-0.6.1/src/tests.rs
+-rw-rw-r--   0     1000     1000     3689 2023-05-15 14:26:56.000000 ever_playground-0.6.1/src/utils.rs
+-rw-rw-r--   0     1000     1000    24730 2023-05-22 16:18:35.000000 ever_playground-0.6.1/Cargo.lock
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 ever_playground-0.6.1/PKG-INFO
```

### Comparing `ever_playground-0.5.0/Cargo.toml` & `ever_playground-0.6.1/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [package]
 name = "ever-playground"
-version = "0.5.0"
+version = "0.6.1"
 edition = "2021"
 
 [lib]
 name = "ever_playground"
 crate-type = ["cdylib"]
 
 [dependencies]
+ed25519-dalek = "1"
 num-bigint = "0.4"
 pyo3 = { version = "0.18.3", features = ["extension-module", "num-bigint"] }
+rand = "0.7"
 
-ton_block = { git = "https://github.com/tonlabs/ever-block.git", tag = "1.9.48" }
-ton_types = { git = "https://github.com/tonlabs/ever-types.git", tag = "2.0.4" }
-ton_labs_assembler = { git = "https://github.com/tonlabs/ever-assembler", tag = "1.2.98" }
-ton_vm = { git = "https://github.com/tonlabs/ever-vm.git", tag = "1.8.136" }
+ton_block = { git = "https://github.com/tonlabs/ever-block.git", tag = "1.9.61" }
+ton_types = { git = "https://github.com/tonlabs/ever-types.git", tag = "2.0.7" }
+ton_labs_assembler = { git = "https://github.com/tonlabs/ever-assembler", tag = "1.2.111" }
+ton_vm = { git = "https://github.com/tonlabs/ever-vm.git", tag = "1.8.149" }
```

### Comparing `ever_playground-0.5.0/README.md` & `ever_playground-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ever_playground-0.5.0/ever_playground/__init__.py` & `ever_playground-0.6.1/ever_playground/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from enum import Enum
 from typing import Tuple
+from fractions import Fraction
 
 from .ever_playground import Cell, Builder, Slice, Dictionary, assemble, runvm
+from .ever_playground import ed25519_new_keypair, ed25519_secret_to_public, ed25519_sign, ed25519_check_signature
 
 __all__ = [
     "Cell",
     "Builder",
     "Slice",
     "Dictionary",
     "ExceptionCode",
     "StateInit",
     "assemble",
     "runvm",
     "parse_smc_addr",
     "load_address",
     "parse_load_address",
     "parse_adnl_address",
+    "ed25519_new_keypair",
+    "ed25519_secret_to_public",
+    "ed25519_sign",
+    "ed25519_check_signature",
 ]
 
 class ExceptionCode(Enum):
     NormalTermination = 0
     AlternativeTermination = 1
     StackUnderflow = 2
     StackOverflow = 3
@@ -62,14 +68,22 @@
 
 def parse_adnl_address(addr: str) -> int:
     """Parses ADNL address"""
     if len(addr) != 64:
         raise Exception("ADNL address must consist of exactly 64 hexadecimal characters")
     return int(addr, 16)
 
+def load_keypair(filename: str) -> Tuple[bytes, bytes]:
+    """Loads private key from a file"""
+    print(f"Loading private key from file {filename}")
+    with open(filename, "rb") as file:
+        secret = file.read()
+        public = ed25519_secret_to_public(secret)
+        return public, secret
+
 class StateInit:
     split_depth: int
     tick: bool
     tock: bool
     code: Cell
     data: Cell
     library: Dictionary
@@ -126,27 +140,36 @@
         if self.library is None:
             b.i(1, 0)
         else:
             b.i(1, 1).s(Slice(self.library.serialize()))
         return b
 
 class Currency:
-    FACTOR = 1000000000 # TODO make this read-only
+    FACTOR = 1000000000
     value: int
 
     def __init__(self, value: int = None):
         if value < 0 or value.bit_length() > 128:
             raise Exception("Currency value must be non-negative and fit into 128 bits")
         self.value = value
 
+    @classmethod
+    def from_str(cls, value: str):
+        value = int(Fraction(value) * Currency.FACTOR)
+        return Currency(value)
+
     def deserialize(self, s: Slice):
-        # TODO
-        pass
+        len = s.u(4)
+        if len == 0:
+            self.value = 0
+        else:
+            self.value = s.u(len * 8)
 
     def serialize(self) -> Builder:
         if self.value == 0:
             return Builder().i(4, 0)
-        len = 1
-        while self.value.bit_length() > len * 8:
-            len += 1
+        len = (self.value.bit_length() + 7) >> 3
         assert(len <= 16)
         return Builder().i(4, len).i(len * 8, self.value)
+
+    def __str__(self) -> str:
+        return str(float(Fraction(self.value) / self.FACTOR))
```

### Comparing `ever_playground-0.5.0/ever_playground/ever_playground.pyi` & `ever_playground-0.6.1/ever_playground/ever_playground.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,21 @@
     """
     A TVM cell consists of at most 1023 bits of data, and of at
     most four references to other cells. All persistent data (including TVM
     code) in the TON Blockchain is represented as a collection of TVM
     cells.
     """
 
-    def write(self) -> bytes:
+    def write(self, flags: int) -> bytes:
         """
         Writes the Cell to a boc bytestream.
+
+        Bits of the flags parameter have the following effect:
+        - +1 enables bag-of-cells index creation (useful for lazy deserialization of large bags of cells).
+        - +2 includes the CRC32-C of all data into the serialization (useful for checking data integrity).
         """
 
     @staticmethod
     def read(bytes: bytes) -> Cell:
         """
         Reads a Cell from a boc bytestream.
         """
@@ -90,19 +94,29 @@
     def x(self, bitstring: str) -> Builder:
         """
         Appends a Builder with a bitstring.
 
         TODO describe what TVM bitstring is
         """
 
+    def y(self, data: bytes) -> Builder:
+        """
+        Appends a Builder with bytes.
+        """
+
     def r(self, cell: Cell) -> Builder:
         """
         Appends a Builder with a Cell.
         """
 
+    def fits(self, slice: Slice, extra_bits: int, extra_refs: int) -> bool:
+        """
+        TODO
+        """
+
     def finalize(self) -> Cell:
         """
         Converts a Builder into an ordinary Cell.
         """
 
     def slice(self) -> Slice:
         """
@@ -122,20 +136,30 @@
     def __init__(self, bit_len: int) -> None: ...
 
     def get(self, key: Slice) -> Slice:
         """
         Searches for a given key and returns corresponding value. None is returned when key is not found.
         """
 
+    def add(self, key: Slice, value: Slice) -> Dictionary:
+        """
+        TODO
+        """
+
     def add_kv_slice(self, key_len: int, slice: Slice) -> Dictionary:
         """
         Adds a new key-value pair from the slice. The first key_len data bits are used as a key,
         and all the rest as a value.
         """
 
+    def cell(self) -> Cell:
+        """
+        Returns underlying cell.
+        """
+
     def serialize(self) -> Builder:
         """
         Serializes a Dictionary into a Builder as defined in the TL-B scheme of HashmapE.
         """
 
     def deserialize(self, slice: Slice) -> Dictionary:
         """
@@ -173,7 +197,25 @@
     steps: int
     gas_used: int
 
 def assemble(code: str) -> Cell:
     """
     Translates a code string in assembler language to a Cell of TVM bytecode.
     """
+
+from typing import Tuple
+
+def ed25519_new_keypair() -> Tuple[bytes, bytes]:
+    """
+    """
+
+def ed25519_secret_to_public(secret: bytes) -> bytes:
+    """
+    """
+
+def ed25519_sign(data: bytes, secret: bytes) -> bytes:
+    """
+    """
+
+def ed25519_check_signature(data: bytes, signature: bytes, public: bytes) -> bool:
+    """
+    """
```

### Comparing `ever_playground-0.5.0/examples/basics.py` & `ever_playground-0.6.1/examples/basics.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     C("c20",
         C("bfc000b4d82161bcb1013f2c6f06dd505c2fae81979bec199f1e6fee63c8c570054_"),
         C("2_",
             C("bfbc43df2056abee4c1a443fbfcfede0ba90d214c77322167fc08ce48920c17c1b"),
             C("bf94a50c1a849a4742214e751977af268269e6eeae064ce800634acea241d430d3"))))
 expect(c, dict_cell1)
 
-dict_bytes = dict_cell1.write()
+dict_bytes = dict_cell1.write(0)
 dict_bytes = bytes(dict_cell1)
 dict_cell2 = C.read(dict_bytes)
 #print(dict_cell2)
 
 expect(dict_cell1, dict_cell2)
 
 #open("test.boc", "wb").write(dict_cell.write())
```

### Comparing `ever_playground-0.5.0/examples/recover-stake.py` & `ever_playground-0.6.1/examples/recover-stake.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 
 # def? $1 { @' $1 } { "recover-query.boc" } cond constant output_fname
 output_filename = "recover-query.boc"
 if argc > 0:
     output_filename = sys.argv[1]
 
 # now constant query_id
-query_id = int(time.time())
+query_id = 1684770872 # int(time.time())
 
 # ."query_id for stake recovery message is set to " query_id . cr
 print(f"query_id for stake recovery message is set to {query_id}")
 
 # <b x{47657424} s, query_id 64 u, b>
 # cr ."Message body is " dup <s csr. cr
 body = B().x("47657424").i(64, query_id).finalize()
 print(f"Message body is {body}")
 
 # 2 boc+>B output_fname tuck B>file ."Saved to file " type cr
-open(output_filename, "wb").write(bytes(body))
+open(output_filename, "wb").write(body.write(2))
 print(f"Saved to file {output_filename}")
```

### Comparing `ever_playground-0.5.0/examples/runvm.py` & `ever_playground-0.6.1/examples/runvm.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,16 +53,16 @@
         BLKPUSH 3, 2
         {}
         DROP
     }}
     REPEAT
 """
 
-chksignu_loop = assemble(loop.format(50000, "CHKSIGNU"))
-blkdrop2_loop = assemble(loop.format(5000000, "BLKDROP 2"))
+chksignu_loop = assemble(loop.format(10000, "CHKSIGNU"))
+blkdrop2_loop = assemble(loop.format(1000000, "BLKDROP 2"))
 
 res = runvm(S(chksignu_loop), [], gas_limit = 100000)
 expect(ExceptionCode.OutOfGas.value, res.exit_code) # out of gas
 
 def benchmark(name, code_cell, iters, steps = None, gas_used = None):
     print("running {}".format(name))
     t = time.time()
@@ -74,9 +74,9 @@
         expect(steps, res.steps)
     if gas_used:
         expect(gas_used, res.gas_used)
 
     print("total time {:.2f}s".format(elapsed))
     print("one iteration takes {:.2f}us".format(elapsed * 1000000 / iters))
 
-benchmark("chksignu loop", chksignu_loop, 50000, 200008, 3750248)
-benchmark("blkdrop2 loop", blkdrop2_loop, 5000000, 20000008, 375000248)
+benchmark("chksignu loop", chksignu_loop, 10000, 40008, 750259)
+benchmark("blkdrop2 loop", blkdrop2_loop, 1000000, 4000008, 75000248)
```

### Comparing `ever_playground-0.5.0/examples/testgiver.py` & `ever_playground-0.6.1/examples/testgiver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # #!/usr/bin/fift -s
 # "TonUtil.fif" include
 
 import sys
 from fractions import Fraction
 
 from ever_playground import Builder as B, Slice as S, Currency, parse_smc_addr, parse_load_address
-#TODO, slice_from_binary_int
 
 # { ."usage: " @' $0 type ." <dest-addr> <seqno> <amount> [<savefile>]" cr
 #   ."Creates a request to TestGiver and saves it into <savefile>.boc" cr
 #   ."('testgiver-query.boc' by default)" cr 1 halt
 # } : usage
 def usage():
     print(f"usage: {sys.argv[0]} <dest-addr> <seqno> <amount> [<savefile>]")
@@ -32,47 +31,46 @@
 
 # $1 true parse-load-address =: bounce 2=: dest_addr
 # $2 parse-int =: seqno
 # $3 $>GR =: amount
 # def? $4 { @' $4 } { "testgiver-query" } cond constant savefile
 dest_address = sys.argv[1]
 dest_wc, dest_addr = parse_load_address(dest_address)
-bounce = 1 # TODO?
+bounce = True # TODO?
 seqno = int(sys.argv[2])
-amount = int(Fraction(sys.argv[3]) * Currency.FACTOR)
+amount = Currency.from_str(sys.argv[3])
 savefile = "testgiver-query"
 if argc > 3:
     savefile = sys.argv[4]
 
 # ."Requesting " amount .GR ."to account "
 # dest_addr 2dup bounce 7 + .Addr ." = " .addr
 # ."seqno=0x" seqno x. ."bounce=" bounce . cr
-print(f"Requesting {amount} to account {dest_address} seqno {hex(seqno)}")
+print(f"Requesting {amount} to account {dest_address} seqno {hex(seqno)} bounce {bounce}")
 
 # // create a message (NB: 01b00.., b = bounce)
 # <b b{01} s, bounce 1 i, b{000100} s, dest_addr addr, 
 #    amount Gram, 0 9 64 32 + + 1+ 1+ u, 0 32 u, "GIFT" $, b>
 # <b seqno 32 u, 1 8 u, swap ref, b>
 # dup ."enveloping message: " <s csr. cr
-
-gift = bytes("GIFT", "utf8").hex()
+hint = bytes("GIFT", "utf8").hex()
 c1 = B().ib("01").i(1, bounce).ib("000100").i(8, dest_wc).i(256, dest_addr) \
-    .b(Currency(amount).serialize()).i(9 + 64 + 32 + 1 + 1, 0).i(32, 0).x(gift) \
+    .b(amount.serialize()).i(9 + 64 + 32 + 1 + 1, 0).i(32, 0).x(hint) \
     .finalize()
 message = B().i(32, seqno).i(8, 1).r(c1).finalize()
 print(f"enveloping message: {message}")
 
 # <b b{1000100} s, giver_addr addr, 0 Gram, b{00} s,
 #    swap <s s, b>
 # dup ."resulting external message: " <s csr. cr
 # 2 boc+>B dup Bx. cr
 # savefile +".boc" tuck B>file
 # ."(Saved to file " type .")" cr
 ext_message = B().ib("1000100").i(8, giver_wc).i(256, giver_addr) \
     .b(Currency(0).serialize()).ib("00").s(S(message)).finalize()
 print(f"resulting external message: {ext_message}")
-ext_message_bytes = bytes(ext_message)
+ext_message_bytes = ext_message.write(2) # include crc32
 print(ext_message_bytes.hex())
 
 output_filename = savefile + ".boc"
 open(output_filename, "wb").write(ext_message_bytes)
 print(f"(Saved to file {output_filename})")
```

### Comparing `ever_playground-0.5.0/examples/validator-elect-req.py` & `ever_playground-0.6.1/examples/validator-elect-req.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,18 +54,18 @@
 if argc > 4:
     output_filename = sys.argv[5]
 
 # ."Creating a request to participate in validator elections at time " elect_time .
 # ."from smart contract " -1 src_addr 2dup 1 .Addr ." = " .addr
 # ." with maximal stake factor with respect to the minimal stake " max_factor ._
 # ."/65536 and validator ADNL address " adnl_addr 64x. cr
-print(f"Creating a request to participate in validator elections at time {elect_time}"
-    f" from smart contract -1:{src_addr:x}"
-    f" with maximal stake factor with respect to the minimal stake {max_factor}"
-    f"/65536 and validator ADNL address {adnl_addr:x}")
+print(f"Creating a request to participate in validator elections at time {elect_time} "
+    f"from smart contract -1:{src_addr:064x} "
+    f"with maximal stake factor with respect to the minimal stake {max_factor}"
+    f"/65536 and validator ADNL address {adnl_addr:064x}")
 
 # B{654c5074} elect_time 32 u>B B+ max_factor 32 u>B B+ src_addr 256 u>B B+ adnl_addr 256 u>B B+
 def bb(len: int, v: int):
     return v.to_bytes(len, "big")
 
 b = bb(4, 0x654c5074) + bb(4, elect_time) + bb(4, max_factor) + bb(32, src_addr) + bb(32, adnl_addr)
```

### Comparing `ever_playground-0.5.0/pyproject.toml` & `ever_playground-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ever_playground-0.5.0/src/lib.rs` & `ever_playground-0.6.1/src/lib.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 mod tests;
 mod utils;
 
 use std::sync::Arc;
 
+use ed25519_dalek::Signer;
 use utils::*;
 
 use num_bigint::{BigInt, BigUint, Sign};
 use pyo3::{
     prelude::*,
     basic::CompareOp,
     exceptions::PyRuntimeError,
@@ -22,15 +23,15 @@
         integer::{IntegerData, utils::process_value},
         savelist::SaveList,
     },
 };
 
 #[pyclass]
 #[derive(Clone)]
-pub struct Cell {
+struct Cell {
     cell: InternalCell,
 }
 
 #[pymethods]
 impl Cell {
     #[new]
     #[pyo3(signature = (bitstring, *args))]
@@ -49,18 +50,24 @@
         Ok(Self { cell })
     }
     fn reference(&self, index: usize) -> PyResult<Cell> {
         self.cell.reference(index)
             .map(|cell| Self { cell })
             .map_err(runtime_err)
     }
-    fn write<'a>(&'a self, py: Python<'a>) -> PyResult<&PyBytes> {
-        ton_types::write_boc(&self.cell)
-            .map(|bytes| PyBytes::new(py, &bytes))
-            .map_err(runtime_err)
+    fn write<'a>(&'a self, py: Python<'a>, flags: usize) -> PyResult<&PyBytes> {
+        if flags > 3 {
+            return err!("flags {} is not supported", flags)
+        }
+        let include_index = flags & 1 == 1;
+        let include_crc = flags & 2 == 2;
+        let writer = ton_types::BocWriter::with_root(&self.cell).map_err(runtime_err)?;
+        let mut bytes = Vec::new();
+        writer.write_ex(&mut bytes, include_index, include_crc, None, None).map_err(runtime_err)?;
+        Ok(PyBytes::new(py, &bytes))
     }
     #[staticmethod]
     fn read(bytes: Vec<u8>) -> PyResult<Self> {
         ton_types::read_single_root_boc(bytes)
             .map(|cell| Self { cell })
             .map_err(runtime_err)
     }
@@ -71,28 +78,28 @@
     fn __len__(&self) -> PyResult<usize> {
         self.cell.count_cells(usize::MAX).map_err(runtime_err)
     }
     fn __str__(&self) -> PyResult<String> {
         PyResult::Ok(dump_cell(self.cell.clone()))
     }
     fn __bytes__<'a>(&'a self, py: Python<'a>) -> PyResult<&PyBytes> {
-        self.write(py)
+        self.write(py, 0)
     }
     fn __richcmp__(&self, other: Self, op: CompareOp, py: Python<'_>) -> PyObject {
         match op {
             CompareOp::Eq => self.cell.eq(&other.cell).into_py(py),
             CompareOp::Ne => self.cell.ne(&other.cell).into_py(py),
             _ => py.NotImplemented(),
         }
     }
 }
 
 #[pyclass]
 #[derive(Clone)]
-pub struct Slice {
+struct Slice {
     slice: SliceData,
 }
 
 #[pymethods]
 impl Slice {
     #[new]
     fn new(cell: Cell) -> PyResult<Self> {
@@ -139,15 +146,15 @@
     fn __str__(&self) -> PyResult<String> {
         Ok(dump_cell(self.slice.cell().clone()))
     }
 }
 
 #[pyclass]
 #[derive(Clone, Default)]
-pub struct Builder {
+struct Builder {
     builder: BuilderData,
 }
 
 #[pymethods]
 impl Builder {
     #[new]
     fn new() -> Self {
@@ -188,19 +195,31 @@
     fn x(mut slf: PyRefMut<Self>, bitstring: String) -> PyResult<PyRefMut<Self>> {
         let slice = SliceData::from_string(&bitstring)
             .map_err(runtime_err)?;
         slf.builder.checked_append_references_and_data(&slice)
             .map_err(runtime_err)?;
         Ok(slf)
     }
+    fn y(mut slf: PyRefMut<Self>, bytes: Vec<u8>) -> PyResult<PyRefMut<Self>> {
+        let length = bytes.len() * 8;
+        let bytes = BuilderData::with_raw(bytes, length)
+            .map_err(runtime_err)?;
+        slf.builder.append_builder(&bytes)
+            .map_err(runtime_err)?;
+        Ok(slf)
+    }
     fn r(mut slf: PyRefMut<Self>, cell: Cell) -> PyResult<PyRefMut<Self>> {
         slf.builder.checked_append_reference(cell.cell)
             .map_err(runtime_err)?;
         Ok(slf)
     }
+    fn fits(&self, slice: Slice, extra_bits: usize, extra_refs: usize) -> bool {
+        self.builder.check_enough_space(slice.slice.remaining_bits() + extra_bits) &&
+            self.builder.check_enough_refs(slice.slice.remaining_references() + extra_refs)
+    }
     fn slice(&self) -> PyResult<Slice> {
         SliceData::load_builder(self.builder.clone())
             .map(|slice| Slice { slice })
             .map_err(runtime_err)
     }
     fn finalize(&self) -> PyResult<Cell> {
         self.builder.clone().into_cell()
@@ -212,15 +231,15 @@
             .map_err(runtime_err)?;
         Ok(dump_cell(cell))
     }
 }
 
 #[pyclass]
 #[derive(Clone)]
-pub struct Dictionary {
+struct Dictionary {
     map: HashmapE,
 }
 
 #[pymethods]
 impl Dictionary {
     #[new]
     fn new(bits: usize) -> Self {
@@ -231,22 +250,27 @@
     }
     fn get(&self, key: Slice, py: Python<'_>) -> PyResult<PyObject> {
         match self.map.get(key.slice).map_err(runtime_err)? {
             Some(slice) => Ok(Slice { slice }.into_py(py)),
             None => Ok(py.None())
         }
     }
-    fn add(&mut self, key: Slice, value: Slice) -> PyResult<Self> {
-        self.map.set(key.slice, &value.slice).map_err(runtime_err)?;
-        Ok(self.clone())
+    fn add(mut slf: PyRefMut<Self>, key: Slice, value: Slice) -> PyResult<PyRefMut<Self>> {
+        slf.map.set(key.slice, &value.slice).map_err(runtime_err)?;
+        Ok(slf)
     }
-    fn add_kv_slice(&mut self, key_bits: usize, mut slice: Slice) -> PyResult<Self> {
+    fn add_kv_slice(mut slf: PyRefMut<Self>, key_bits: usize, mut slice: Slice) -> PyResult<PyRefMut<Self>> {
         let key = slice.slice.get_next_slice(key_bits).map_err(runtime_err)?;
-        self.map.set(key, &slice.slice).map_err(runtime_err)?;
-        Ok(self.clone())
+        slf.map.set(key, &slice.slice).map_err(runtime_err)?;
+        Ok(slf)
+    }
+    fn cell(&self) -> PyResult<Cell> {
+        self.map.data()
+            .map(|cell| Cell { cell: cell.clone() })
+            .ok_or(PyRuntimeError::new_err("empty dictionary"))
     }
     fn serialize(&self) -> PyResult<Builder> {
         let mut builder = BuilderData::new();
         self.map.write_hashmap_data(&mut builder).map_err(runtime_err)?;
         Ok(Builder { builder })
     }
     #[staticmethod]
@@ -468,20 +492,63 @@
                 list.push(convert_from_vm(py, item)?)
             }
             Ok(PyList::new(py, list).into_py(py))
         }
     }
 }
 
+#[pyfunction]
+fn ed25519_new_keypair<'a>(py: Python<'a>) -> PyResult<&PyTuple> {
+    let mut csprng = rand::thread_rng();
+    let keypair = ed25519_dalek::Keypair::generate(&mut csprng);
+    Ok(PyTuple::new(py, vec!(
+        PyBytes::new(py, keypair.secret.as_bytes()),
+        PyBytes::new(py, keypair.public.as_bytes()),
+    )))
+}
+
+fn load_secret(secret: &PyBytes) -> PyResult<ed25519_dalek::SecretKey> {
+    let secret = ed25519_dalek::SecretKey::from_bytes(secret.as_bytes())
+        .map_err(|err| PyRuntimeError::new_err(format!("invalid secret bytes: {}", err)))?;
+    Ok(secret)
+}
+
+#[pyfunction]
+fn ed25519_secret_to_public<'a>(secret: &'a PyBytes, py: Python<'a>) -> PyResult<&'a PyBytes> {
+    let secret = load_secret(secret)?;
+    let public = ed25519_dalek::PublicKey::from(&secret);
+    Ok(PyBytes::new(py, public.as_bytes()))
+}
+
+#[pyfunction]
+fn ed25519_sign<'a>(data: &'a PyBytes, secret: &'a PyBytes, py: Python<'a>) -> PyResult<&'a PyBytes> {
+    let secret = load_secret(secret)?;
+    let public = ed25519_dalek::PublicKey::from(&secret);
+    let keypair = ed25519_dalek::Keypair { secret, public };
+    let signature = &keypair.sign(data.as_bytes()).to_bytes()[0..];
+    Ok(PyBytes::new(py, signature))
+}
+
+#[pyfunction]
+fn ed25519_check_signature<'a>(data: &'a PyBytes, signature: &'a PyBytes, public: &'a PyBytes) -> bool {
+    let Ok(public) = ed25519_dalek::PublicKey::from_bytes(public.as_bytes()) else { return false };
+    let Ok(signature) = ed25519_dalek::Signature::from_bytes(signature.as_bytes()) else { return false };
+    public.verify_strict(data.as_bytes(), &signature).is_ok()
+}
+
 #[pymodule]
 fn ever_playground(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<NaN>()?;
     m.add_class::<Cell>()?;
     m.add_class::<Builder>()?;
     m.add_class::<Slice>()?;
     m.add_class::<Dictionary>()?;
     m.add_class::<Continuation>()?;
     m.add_class::<VmResult>()?;
     m.add_wrapped(wrap_pyfunction!(assemble))?;
     m.add_wrapped(wrap_pyfunction!(runvm))?;
+    m.add_wrapped(wrap_pyfunction!(ed25519_new_keypair))?;
+    m.add_wrapped(wrap_pyfunction!(ed25519_secret_to_public))?;
+    m.add_wrapped(wrap_pyfunction!(ed25519_sign))?;
+    m.add_wrapped(wrap_pyfunction!(ed25519_check_signature))?;
     Ok(())
 }
```

### Comparing `ever_playground-0.5.0/src/tests.rs` & `ever_playground-0.6.1/src/tests.rs`

 * *Files identical despite different names*

### Comparing `ever_playground-0.5.0/src/utils.rs` & `ever_playground-0.6.1/src/utils.rs`

 * *Files identical despite different names*

### Comparing `ever_playground-0.5.0/Cargo.lock` & `ever_playground-0.6.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -223,18 +223,20 @@
  "serde",
  "sha2 0.9.9",
  "zeroize",
 ]
 
 [[package]]
 name = "ever-playground"
-version = "0.5.0"
+version = "0.6.1"
 dependencies = [
+ "ed25519-dalek",
  "num-bigint",
  "pyo3",
+ "rand",
  "ton_block",
  "ton_labs_assembler",
  "ton_types",
  "ton_vm",
 ]
 
 [[package]]
@@ -768,16 +770,16 @@
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "ton_block"
-version = "1.9.48"
-source = "git+https://github.com/tonlabs/ever-block.git?tag=1.9.48#6060d0e12b211989cac766d2f2d74221878e3a5d"
+version = "1.9.61"
+source = "git+https://github.com/tonlabs/ever-block.git?tag=1.9.61#3870fa91ec28902eaf10795a9cc08ca08465578e"
 dependencies = [
  "base64",
  "crc",
  "ed25519",
  "ed25519-dalek",
  "failure",
  "hex",
@@ -786,31 +788,31 @@
  "num-traits",
  "sha2 0.10.6",
  "ton_types",
 ]
 
 [[package]]
 name = "ton_labs_assembler"
-version = "1.2.98"
-source = "git+https://github.com/tonlabs/ever-assembler?tag=1.2.98#0b1d964b57d249148fa3bd914ff6d2cf1250dccf"
+version = "1.2.111"
+source = "git+https://github.com/tonlabs/ever-assembler?tag=1.2.111#c7febf00f6e77a2e77984ee6f9ebaac40cefeaef"
 dependencies = [
  "failure",
  "hex",
  "log",
  "num",
  "num-traits",
  "serde",
  "serde_json",
  "ton_types",
 ]
 
 [[package]]
 name = "ton_types"
-version = "2.0.4"
-source = "git+https://github.com/tonlabs/ever-types.git?tag=2.0.4#83d376d4079c9761b54cc58d30b975f406ea527f"
+version = "2.0.7"
+source = "git+https://github.com/tonlabs/ever-types.git?tag=2.0.7#5815cc3cb53f7dc3cf91a32616159c595f81d0ff"
 dependencies = [
  "aes-ctr",
  "base64",
  "crc",
  "curve25519-dalek",
  "ed25519",
  "ed25519-dalek",
@@ -828,16 +830,16 @@
  "sha2 0.10.6",
  "smallvec",
  "x25519-dalek",
 ]
 
 [[package]]
 name = "ton_vm"
-version = "1.8.136"
-source = "git+https://github.com/tonlabs/ever-vm.git?tag=1.8.136#e6f66084cc51640322303d41c2915392a46098c6"
+version = "1.8.149"
+source = "git+https://github.com/tonlabs/ever-vm.git?tag=1.8.149#e867fffddd6aecd2d7f846cdf6e19dcb09f80778"
 dependencies = [
  "ed25519",
  "ed25519-dalek",
  "failure",
  "hex",
  "lazy_static",
  "log",
```

### Comparing `ever_playground-0.5.0/PKG-INFO` & `ever_playground-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ever-playground
-Version: 0.5.0
+Version: 0.6.1
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # ever-playground
 
 A tool alternative to Fift: play with Cells, Slices, Builders, and Dictionaries — native types of TVM; assemble and run TVM code.
```

