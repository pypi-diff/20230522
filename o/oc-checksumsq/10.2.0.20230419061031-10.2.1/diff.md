# Comparing `tmp/oc_checksumsq-10.2.0.20230419061031-py3-none-any.whl.zip` & `tmp/oc_checksumsq-10.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,10 @@
-Zip file size: 8689 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 06:10 cdt_checksumsq/__init__.py
--rw-r--r--  2.0 unx     2496 b- defN 23-Apr-19 06:10 cdt_checksumsq/checksums_interface.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 06:10 cdt_checksumsq/test/__init__.py
--rw-r--r--  2.0 unx     1029 b- defN 23-Apr-19 06:10 cdt_checksumsq/test/test_doublequeue.py
--rwxr-xr-x  2.0 unx     2400 b- defN 23-Apr-19 06:10 oc_checksumsq-10.2.0.20230419061031.data/scripts/chkreg.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-19 06:10 oc_checksumsq-10.2.0.20230419061031.dist-info/LICENSE
--rw-r--r--  2.0 unx      236 b- defN 23-Apr-19 06:10 oc_checksumsq-10.2.0.20230419061031.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 06:10 oc_checksumsq-10.2.0.20230419061031.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-19 06:10 oc_checksumsq-10.2.0.20230419061031.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      966 b- defN 23-Apr-19 06:10 oc_checksumsq-10.2.0.20230419061031.dist-info/RECORD
-10 files, 18591 bytes uncompressed, 6987 bytes compressed:  62.4%
+Zip file size: 7605 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        0 b- defN 23-May-22 09:43 oc_checksumsq/__init__.py
+-rw-r--r--  2.0 unx     2464 b- defN 23-May-22 09:43 oc_checksumsq/checksums_interface.py
+-rwxr-xr-x  2.0 unx     2378 b- defN 23-May-22 09:43 oc_checksumsq-10.2.1.data/scripts/chkreg.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-22 09:43 oc_checksumsq-10.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      221 b- defN 23-May-22 09:43 oc_checksumsq-10.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-22 09:43 oc_checksumsq-10.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-May-22 09:43 oc_checksumsq-10.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      693 b- defN 23-May-22 09:43 oc_checksumsq-10.2.1.dist-info/RECORD
+8 files, 17219 bytes uncompressed, 6379 bytes compressed:  63.0%
```

## zipnote {}

```diff
@@ -1,31 +1,25 @@
-Filename: cdt_checksumsq/__init__.py
+Filename: oc_checksumsq/__init__.py
 Comment: 
 
-Filename: cdt_checksumsq/checksums_interface.py
+Filename: oc_checksumsq/checksums_interface.py
 Comment: 
 
-Filename: cdt_checksumsq/test/__init__.py
+Filename: oc_checksumsq-10.2.1.data/scripts/chkreg.py
 Comment: 
 
-Filename: cdt_checksumsq/test/test_doublequeue.py
+Filename: oc_checksumsq-10.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: oc_checksumsq-10.2.0.20230419061031.data/scripts/chkreg.py
+Filename: oc_checksumsq-10.2.1.dist-info/METADATA
 Comment: 
 
-Filename: oc_checksumsq-10.2.0.20230419061031.dist-info/LICENSE
+Filename: oc_checksumsq-10.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: oc_checksumsq-10.2.0.20230419061031.dist-info/METADATA
+Filename: oc_checksumsq-10.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: oc_checksumsq-10.2.0.20230419061031.dist-info/WHEEL
-Comment: 
-
-Filename: oc_checksumsq-10.2.0.20230419061031.dist-info/top_level.txt
-Comment: 
-
-Filename: oc_checksumsq-10.2.0.20230419061031.dist-info/RECORD
+Filename: oc_checksumsq-10.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cdt_checksumsq/checksums_interface.py` & `oc_checksumsq/checksums_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def __init__(self, *args, **argv):
         super(ChecksumsQueueClient, self).__init__(*args, **argv)
         self.queue_cnt = None
 
     def basic_args(self, parser = None):
         parser = super(ChecksumsQueueClient, self).basic_args(parser)
         parser.add_argument('--queue-cnt', help = 'cdtcontents queue name', default = getenv('AMQP_CNT_QUEUE', queue_cnt_name))
-        # SII-13216 Overriding default exchange value for message duplication support
+        # Overriding default exchange value for message duplication support
         parser.set_defaults(exchange='cdt.dlartifacts.input')
         return parser
 
     def setup_from_args(self, args = None):
         args = super(ChecksumsQueueClient, self).setup_from_args(args)  # this sets up all parent classes
         self.setup(queue_cnt = args.queue_cnt) # this relates to current class
         return args
@@ -40,15 +40,15 @@
         self.routing_key = self.queue_cnt
         super(ChecksumsQueueClient, self).send(*args, **argv)
         self.routing_key = usual_routing_key
 
         return usual
 
 
-# A.Knyazev, SII-10060: 'artifact_deliverable' default value has been changed to 'None' 
+# 'artifact_deliverable' default value has been changed to 'None' 
 #   otherwise we may occasionly enable forbidden distributive
 
 class ChecksumsQueueServer(QueueApplication):
     default_queue_name = queue_name
     published = queue_published
 
     def register_file(self, location, citype, depth=0, remove=False, version=None, client=None, parent=None, artifact_deliverable=None):
```

## Comparing `oc_checksumsq-10.2.0.20230419061031.data/scripts/chkreg.py` & `oc_checksumsq-10.2.1.data/scripts/chkreg.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 parser.add_argument('--ping', help='Send ping message', default=False, action='store_true')
 parser.add_argument('--register', help='Send file registration request', metavar='PATH', default=None)
 parser.add_argument('--citype', help='CIType code', default=None)
 parser.add_argument('--loctype', help='Location type, default: NXS', default='NXS')
 parser.add_argument('--revision', help='SVN revision', default=None)
 parser.add_argument('--depth', type=int, help='File registration depth, default: 0', default=0)
 
-#A.Knyazev, SII-10060: these two parameters added for possibility to register in Mongo correctly with 
+#these two parameters added for possibility to register in Mongo correctly with 
 # deploying deny/allow mechanism
 parser.add_argument('--parent', help='Parent list: JSON-parsable string', default=None)
 parser.add_argument('--artifact-deliverable', help="Delivery enabled", default=None)
 parser.add_argument('--version', help='Version', default=None)
 parser.add_argument('--client', help="CDT client code", default=None)
 
 client.basic_args(parser)     # add AMQP-specific arguments
```

## Comparing `oc_checksumsq-10.2.0.20230419061031.dist-info/LICENSE` & `oc_checksumsq-10.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

