# Comparing `tmp/posttroll-1.9.0.tar.gz` & `tmp/posttroll-v1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posttroll-1.9.0.tar", last modified: Wed Oct 19 16:16:16 2022, max compression
+gzip compressed data, was "dist/posttroll-v1.1.0.tar", last modified: Thu Jan 28 09:55:51 2016, max compression
```

## Comparing `posttroll-1.9.0.tar` & `posttroll-v1.1.0.tar`

### file list

```diff
@@ -1,30 +1,27 @@
-drwxrwxr-x   0 pnuu      (1000) pnuu      (1000)        0 2022-10-19 16:16:16.101655 posttroll-1.9.0/
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)    35147 2021-12-23 09:11:06.000000 posttroll-1.9.0/LICENSE.txt
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)       51 2021-12-23 09:11:06.000000 posttroll-1.9.0/MANIFEST.in
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)      619 2022-10-19 16:16:16.101655 posttroll-1.9.0/PKG-INFO
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)      240 2021-12-23 09:11:06.000000 posttroll-1.9.0/README.md
-drwxrwxr-x   0 pnuu      (1000) pnuu      (1000)        0 2022-10-19 16:16:16.101655 posttroll-1.9.0/bin/
--rwxrwxr-x   0 pnuu      (1000) pnuu      (1000)     4666 2021-12-23 09:11:06.000000 posttroll-1.9.0/bin/nameserver
-drwxrwxr-x   0 pnuu      (1000) pnuu      (1000)        0 2022-10-19 16:16:16.101655 posttroll-1.9.0/posttroll/
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)     2766 2022-10-19 16:06:21.000000 posttroll-1.9.0/posttroll/__init__.py
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)     8534 2021-12-23 09:11:06.000000 posttroll-1.9.0/posttroll/address_receiver.py
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)     5937 2021-12-23 09:11:06.000000 posttroll-1.9.0/posttroll/bbmcast.py
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)     4715 2022-10-19 16:06:21.000000 posttroll-1.9.0/posttroll/listener.py
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)     6438 2021-12-23 09:11:06.000000 posttroll-1.9.0/posttroll/logger.py
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)     9981 2021-12-23 09:11:06.000000 posttroll-1.9.0/posttroll/message.py
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)     6113 2021-12-23 09:11:06.000000 posttroll-1.9.0/posttroll/message_broadcaster.py
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)     5408 2021-12-23 09:11:06.000000 posttroll-1.9.0/posttroll/ns.py
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)    12234 2022-10-19 16:06:21.000000 posttroll-1.9.0/posttroll/publisher.py
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)    17301 2022-10-19 16:06:21.000000 posttroll-1.9.0/posttroll/subscriber.py
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)      497 2022-10-19 16:16:16.101655 posttroll-1.9.0/posttroll/version.py
-drwxrwxr-x   0 pnuu      (1000) pnuu      (1000)        0 2022-10-19 16:16:16.101655 posttroll-1.9.0/posttroll.egg-info/
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)      619 2022-10-19 16:16:16.000000 posttroll-1.9.0/posttroll.egg-info/PKG-INFO
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)      566 2022-10-19 16:16:16.000000 posttroll-1.9.0/posttroll.egg-info/SOURCES.txt
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)        1 2022-10-19 16:16:16.000000 posttroll-1.9.0/posttroll.egg-info/dependency_links.txt
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)       56 2022-10-19 16:16:16.000000 posttroll-1.9.0/posttroll.egg-info/entry_points.txt
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)        1 2021-12-23 09:23:09.000000 posttroll-1.9.0/posttroll.egg-info/not-zip-safe
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)       23 2022-10-19 16:16:16.000000 posttroll-1.9.0/posttroll.egg-info/requires.txt
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)       10 2022-10-19 16:16:16.000000 posttroll-1.9.0/posttroll.egg-info/top_level.txt
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)      243 2022-10-19 16:16:16.101655 posttroll-1.9.0/setup.cfg
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)     1927 2022-10-19 16:06:21.000000 posttroll-1.9.0/setup.py
--rw-rw-r--   0 pnuu      (1000) pnuu      (1000)    81291 2022-10-19 16:06:21.000000 posttroll-1.9.0/versioneer.py
+drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2016-01-28 09:55:51.000000 posttroll-v1.1.0/
+drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2016-01-28 09:55:51.000000 posttroll-v1.1.0/bin/
+-rwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)     4264 2015-02-11 20:48:01.000000 posttroll-v1.1.0/bin/nameserver
+drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2016-01-28 09:55:51.000000 posttroll-v1.1.0/posttroll/
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     1819 2016-01-28 09:47:50.000000 posttroll-v1.1.0/posttroll/__init__.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     6275 2015-02-11 20:44:54.000000 posttroll-v1.1.0/posttroll/address_receiver.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     5390 2015-10-27 12:27:03.000000 posttroll-v1.1.0/posttroll/bbmcast.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     3821 2013-04-23 13:39:19.000000 posttroll-v1.1.0/posttroll/ingester.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     6523 2015-02-19 13:56:45.000000 posttroll-v1.1.0/posttroll/logger.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     9228 2016-01-28 09:47:50.000000 posttroll-v1.1.0/posttroll/message.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     4026 2015-03-25 15:41:43.000000 posttroll-v1.1.0/posttroll/message_broadcaster.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     4574 2016-01-28 09:47:50.000000 posttroll-v1.1.0/posttroll/ns.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     7790 2015-10-27 12:27:56.000000 posttroll-v1.1.0/posttroll/publisher.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    13390 2016-01-28 09:47:50.000000 posttroll-v1.1.0/posttroll/subscriber.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     3443 2013-04-23 07:31:15.000000 posttroll-v1.1.0/posttroll/test_multicast.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      827 2016-01-28 09:47:50.000000 posttroll-v1.1.0/posttroll/version.py
+drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2016-01-28 09:55:51.000000 posttroll-v1.1.0/posttroll.egg-info/
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      609 2016-01-28 09:55:51.000000 posttroll-v1.1.0/posttroll.egg-info/PKG-INFO
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      546 2016-01-28 09:55:51.000000 posttroll-v1.1.0/posttroll.egg-info/SOURCES.txt
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)        1 2016-01-28 09:55:51.000000 posttroll-v1.1.0/posttroll.egg-info/dependency_links.txt
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)       57 2016-01-28 09:55:51.000000 posttroll-v1.1.0/posttroll.egg-info/entry_points.txt
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)        1 2013-01-15 11:41:02.000000 posttroll-v1.1.0/posttroll.egg-info/not-zip-safe
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)        5 2016-01-28 09:55:51.000000 posttroll-v1.1.0/posttroll.egg-info/requires.txt
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)       10 2016-01-28 09:55:51.000000 posttroll-v1.1.0/posttroll.egg-info/top_level.txt
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     1963 2016-01-28 09:47:50.000000 posttroll-v1.1.0/setup.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      609 2016-01-28 09:55:51.000000 posttroll-v1.1.0/PKG-INFO
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      120 2016-01-28 09:55:51.000000 posttroll-v1.1.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `posttroll-1.9.0/bin/nameserver` & `posttroll-v1.1.0/bin/nameserver`

 * *Files 8% similar despite different names*

```diff
@@ -24,72 +24,64 @@
 """
 
 # TODO: make port configurable.
 
 from posttroll.ns import NameServer
 
 import logging
-import _strptime
 
 logger = logging.getLogger(__name__)
 
 if __name__ == '__main__':
-
+    
     import argparse
 
     parser = argparse.ArgumentParser()
     parser.add_argument("-d", "--daemon", help="Run as a daemon",
                         choices=["start", "stop", "status", "restart"])
     parser.add_argument("-l", "--log", help="File to log to (defaults to stdout)",
                         default=None)
     parser.add_argument("-v", "--verbose", help="print debug messages too",
                         action="store_true")
-    parser.add_argument("--no-multicast", help="disable multicasting",
-                        action="store_true")
-    parser.add_argument("-L", "--local-only", help="accept connections only from localhost",
-                        action="store_true")
     opts = parser.parse_args()
 
     if opts.log:
         import logging.handlers
         handler = logging.handlers.TimedRotatingFileHandler(opts.log,
                                                             "midnight",
                                                             backupCount=7)
     else:
         handler = logging.StreamHandler()
     handler.setFormatter(logging.Formatter("[%(levelname)s: %(asctime)s :"
-                                           " %(name)s] %(message)s",
-                                           '%Y-%m-%d %H:%M:%S'))
+                                                " %(name)s] %(message)s",
+                                                '%Y-%m-%d %H:%M:%S'))
     if opts.verbose:
         loglevel = logging.DEBUG
     else:
         loglevel = logging.INFO
     handler.setLevel(loglevel)
     logging.getLogger('').setLevel(loglevel)
     logging.getLogger('').addHandler(handler)
     logger = logging.getLogger("nameserver")
 
-    multicast_enabled = (opts.no_multicast == False)
-    local_only = (opts.local_only)
-
-    ns = NameServer(multicast_enabled=multicast_enabled, restrict_to_localhost=local_only)
+    ns = NameServer()
 
     if opts.daemon is None:
         try:
             ns.run()
         except KeyboardInterrupt:
             pass
         except:
             logger.exception("Something wrong happened...")
             raise
         finally:
-            print("Thanks for using pytroll/nameserver. "
-                  "See you soon on www.pytroll.org!")
+            print ("Thanks for using pytroll/nameserver. "
+                   "See you soon on www.pytroll.org!")
 
-    else:  # Running as a daemon
+    else: # Running as a daemon
         if opts.daemon == "status":
             import os
             import sys
             if os.path.exists("/tmp/nameserver.pid"):
                 with open("/tmp/nameserver.pid") as fd_:
                     pid = int(fd_.read())
                     try:
@@ -100,17 +92,16 @@
                         sys.exit(0)
             else:
                 sys.exit(1)
         try:
             import daemon.runner
             import signal
             import sys
-
+            
             class App(object):
-
                 """App object for running the nameserver as daemon.
                 """
                 stdin_path = "/dev/null"
                 stdout_path = "/dev/null"
                 stderr_path = "/dev/null"
                 run = ns.run
                 pidfile_path = "/tmp/nameserver.pid"
@@ -118,18 +109,20 @@
 
             def _terminate(*args):
                 """terminate the nameserver.
                 """
                 del args
                 ns.stop()
 
+
             signal.signal(signal.SIGTERM, _terminate)
 
+
             APP = App()
             sys.argv = [sys.argv[0], opts.daemon]
             angel = daemon.runner.DaemonRunner(APP)
             if opts.log:
                 angel.daemon_context.files_preserve = [handler.stream]
             angel.parse_args([sys.argv[0], opts.daemon])
             sys.exit(angel.do_action())
         except ImportError:
-            print("Cannot run as a daemon, you need python-daemon installed.")
+            print "Cannot run as a daemon, you need python-daemon installed."
```

### Comparing `posttroll-1.9.0/posttroll/__init__.py` & `posttroll-v1.1.0/posttroll/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,91 +1,57 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (c) 2010-2012, 2014.
-#
+
 # Author(s):
-#
+
 #   Lars Ø. Rasmussen <ras@dmi.dk>
 #   Martin Raspaud <martin.raspaud@smhi.se>
-#   Panu Lahtinen <panu.lahtinen@fmi.fi>
-#
+
 # This file is part of pytroll.
-#
+
 # Pytroll is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
-#
+
 # Pytroll is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-#
+
 # You should have received a copy of the GNU General Public License along with
 # pytroll.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Posttroll packages."""
-
-import logging
-import os
 import sys
+assert sys.version[0:3] >= '2.5', 'Python version 2.5 or above is required.'
 from datetime import datetime
 
 import zmq
-from donfig import Config
-
-from .version import get_versions
-
-config = Config('posttroll')
-context = {}
-logger = logging.getLogger(__name__)
+context = zmq.Context()
 
 
-def get_context():
-    """Provide the context to use.
-
-    This function takes care of creating new contexts in case of forks.
-    """
-    pid = os.getpid()
-    if pid not in context:
-        context[pid] = zmq.Context()
-        logger.debug('renewed context for PID %d', pid)
-    return context[pid]
+def renew_context():
+    global context
+    context = zmq.Context()
 
 
 def strp_isoformat(strg):
     """Decode an ISO formatted string to a datetime object.
-
     Allow a time-string without microseconds.
 
     We handle input like: 2011-11-14T12:51:25.123456
     """
     if isinstance(strg, datetime):
         return strg
     if len(strg) < 19 or len(strg) > 26:
         if len(strg) > 30:
             strg = strg[:30] + '...'
-        raise ValueError("Invalid ISO formatted time string '%s'" % strg)
+        raise ValueError("Invalid ISO formatted time string '%s'"%strg)
     if strg.find(".") == -1:
         strg += '.000000'
     if sys.version[0:3] >= '2.6':
         return datetime.strptime(strg, "%Y-%m-%dT%H:%M:%S.%f")
     else:
         dat, mis = strg.split(".")
         dat = datetime.strptime(dat, "%Y-%m-%dT%H:%M:%S")
         mis = int(float('.' + mis)*1000000)
         return dat.replace(microsecond=mis)
-
-
-def _set_tcp_keepalive(socket):
-    _set_int_sockopt(socket, zmq.TCP_KEEPALIVE, config.get("tcp_keepalive", None))
-    _set_int_sockopt(socket, zmq.TCP_KEEPALIVE_CNT, config.get("tcp_keepalive_cnt", None))
-    _set_int_sockopt(socket, zmq.TCP_KEEPALIVE_IDLE, config.get("tcp_keepalive_idle", None))
-    _set_int_sockopt(socket, zmq.TCP_KEEPALIVE_INTVL, config.get("tcp_keepalive_intvl", None))
-
-
-def _set_int_sockopt(socket, param, value):
-    if value is not None:
-        socket.setsockopt(param, int(value))
-
-
-__version__ = get_versions()['version']
-del get_versions
```

### Comparing `posttroll-1.9.0/posttroll/address_receiver.py` & `posttroll-v1.1.0/posttroll/address_receiver.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,230 +17,170 @@
 # Pytroll is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License along with
 # pytroll.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Receive broadcasted addresses in a standard pytroll Message.
-
-It will look like:
+"""
+Receive broadcasted addresses in a standard pytroll Message:
 /<server-name>/address info ... host:port
 """
 import copy
 import logging
 import os
+import thread
 import threading
-import errno
-import time
-
 from datetime import datetime, timedelta
 
-import netifaces
-from zmq import REP, LINGER
-
 from posttroll.bbmcast import MulticastReceiver, SocketTimeout
 from posttroll.message import Message
 from posttroll.publisher import Publish
-from posttroll import get_context
 
 
 __all__ = ('AddressReceiver', 'getaddress')
 
-LOGGER = logging.getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 debug = os.environ.get('DEBUG', False)
 broadcast_port = 21200
 
 default_publish_port = 16543
 
-ten_minutes = timedelta(minutes=10)
-zero_seconds = timedelta(seconds=0)
-
-
-def get_local_ips():
-    inet_addrs = [netifaces.ifaddresses(iface).get(netifaces.AF_INET)
-                  for iface in netifaces.interfaces()]
-    ips = []
-    for addr in inet_addrs:
-        if addr is not None:
-            for add in addr:
-                ips.append(add['addr'])
-    return ips
-
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 #
 # General thread to receive broadcast addresses.
 #
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 
 
 class AddressReceiver(object):
-    """General thread to receive broadcast addresses."""
 
-    def __init__(self, max_age=ten_minutes, port=None,
-                 do_heartbeat=True, multicast_enabled=True, restrict_to_localhost=False):
+    """General thread to receive broadcast addresses.
+    """
+
+    def __init__(self, max_age=timedelta(minutes=10), port=None,
+                 do_heartbeat=True):
         self._max_age = max_age
         self._port = port or default_publish_port
-        self._address_lock = threading.Lock()
+        self._address_lock = thread.allocate_lock()
         self._addresses = {}
         self._subject = '/address'
         self._do_heartbeat = do_heartbeat
-        self._multicast_enabled = multicast_enabled
         self._last_age_check = datetime(1900, 1, 1)
         self._do_run = False
         self._is_running = False
         self._thread = threading.Thread(target=self._run)
-        self._restrict_to_localhost = restrict_to_localhost
-        self._local_ips = get_local_ips()
 
     def start(self):
-        """Start the receiver."""
+        """Start the receiver.
+        """
         if not self._is_running:
             self._do_run = True
             self._thread.start()
         return self
 
     def stop(self):
-        """Stop the receiver."""
+        """Stop the receiver.
+        """
         self._do_run = False
         return self
 
     def is_running(self):
-        """Check if the receiver is alive."""
+        """Check if the receiver is alive.
+        """
         return self._is_running
 
     def get(self, name=""):
-        """Get the address(es)."""
+        """Get the address(es).
+        """
         addrs = []
 
-        with self._address_lock:
+        self._address_lock.acquire()
+        try:
             for metadata in self._addresses.values():
                 if (name == "" or
                         (name and name in metadata["service"])):
                     mda = copy.copy(metadata)
                     mda["receive_time"] = mda["receive_time"].isoformat()
                     addrs.append(mda)
-        LOGGER.debug('return address %s', str(addrs))
+        finally:
+            self._address_lock.release()
+        logger.debug('return address ' + str(addrs))
         return addrs
 
-    def _check_age(self, pub, min_interval=zero_seconds):
-        """Check the age of the receiver."""
+    def _check_age(self, pub, min_interval=timedelta(seconds=0)):
+        """Check the age of the receiver.
+        """
         now = datetime.utcnow()
         if (now - self._last_age_check) <= min_interval:
             return
 
-        LOGGER.debug("%s - checking addresses", str(datetime.utcnow()))
+        logger.debug(str(datetime.utcnow()) + " checking addresses")
         self._last_age_check = now
-        to_del = []
-        with self._address_lock:
+        self._address_lock.acquire()
+        try:
             for addr, metadata in self._addresses.items():
                 atime = metadata["receive_time"]
                 if now - atime > self._max_age:
                     mda = {'status': False,
                            'URI': addr,
                            'service': metadata['service']}
                     msg = Message('/address/' + metadata['name'], 'info', mda)
-                    to_del.append(addr)
-                    LOGGER.info("publish remove '%s'", str(msg))
+                    del self._addresses[addr]
+                    logger.info("publish remove '%s'", str(msg))
                     pub.send(msg.encode())
-            for addr in to_del:
-                del self._addresses[addr]
+        finally:
+            self._address_lock.release()
 
     def _run(self):
-        """Run the receiver."""
+        """Run the receiver.
+        """
         port = broadcast_port
-        nameservers = []
-        if self._multicast_enabled:
-            while True:
-                try:
-                    recv = MulticastReceiver(port)
-                except IOError as err:
-                    if err.errno == errno.ENODEV:
-                        LOGGER.error("Receiver initialization failed "
-                                     "(no such device). "
-                                     "Trying again in %d s",
-                                     10)
-                        time.sleep(10)
-                    else:
-                        raise
-                else:
-                    recv.settimeout(tout=2.0)
-                    LOGGER.info("Receiver initialized.")
-                    break
-
-        else:
-            recv = _SimpleReceiver(port)
-            nameservers = ["localhost"]
-
+        recv = MulticastReceiver(port).settimeout(2.)
         self._is_running = True
-        with Publish("address_receiver", self._port, ["addresses"],
-                     nameservers=nameservers) as pub:
+        with Publish("address_receiver", self._port, ["addresses"]) as pub:
             try:
                 while self._do_run:
                     try:
                         data, fromaddr = recv()
-                        if self._multicast_enabled:
-                            ip_, port = fromaddr
-                            if self._restrict_to_localhost and ip_ not in self._local_ips:
-                                # discard external message
-                                LOGGER.debug('Discard external message')
-                                continue
-                        LOGGER.debug("data %s", data)
+                        del fromaddr
                     except SocketTimeout:
-                        if self._multicast_enabled:
-                            LOGGER.debug("Multicast socket timed out on recv!")
-                            continue
+                        logger.debug("Multicast socket timed out on recv!")
+                        continue
                     finally:
                         self._check_age(pub, min_interval=self._max_age / 20)
                         if self._do_heartbeat:
                             pub.heartbeat(min_interval=29)
                     msg = Message.decode(data)
                     name = msg.subject.split("/")[1]
                     if(msg.type == 'info' and
                        msg.subject.lower().startswith(self._subject)):
                         addr = msg.data["URI"]
                         msg.data['status'] = True
                         metadata = copy.copy(msg.data)
                         metadata["name"] = name
 
-                        LOGGER.debug('receiving address %s %s %s', str(addr),
-                                     str(name), str(metadata))
+                        logger.debug('receiving address ' + str(addr)
+                                     + " " + str(name) + " " + str(metadata))
                         if addr not in self._addresses:
-                            LOGGER.info("nameserver: publish add '%s'",
+                            logger.info("nameserver: publish add '%s'",
                                         str(msg))
                             pub.send(msg.encode())
                         self._add(addr, metadata)
             finally:
                 self._is_running = False
                 recv.close()
 
     def _add(self, adr, metadata):
-        """Add an address."""
-        with self._address_lock:
+        """Add an address.
+        """
+        self._address_lock.acquire()
+        try:
             metadata["receive_time"] = datetime.utcnow()
             self._addresses[adr] = metadata
+        finally:
+            self._address_lock.release()
 
-
-class _SimpleReceiver(object):
-
-    """ Simple listing on port for address messages."""
-
-    def __init__(self, port=None):
-        self._port = port or default_publish_port
-        self._socket = get_context().socket(REP)
-        self._socket.bind("tcp://*:" + str(port))
-
-    def __call__(self):
-        message = self._socket.recv_string()
-        self._socket.send_string("ok")
-        return message, None
-
-    def close(self):
-        """Close the receiver."""
-        self._socket.setsockopt(LINGER, 1)
-        self._socket.close()
-
-
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 # default
 getaddress = AddressReceiver
```

### Comparing `posttroll-1.9.0/posttroll/bbmcast.py` & `posttroll-v1.1.0/posttroll/bbmcast.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,97 +18,92 @@
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License along with
 # posttroll.  If not, see <http://www.gnu.org/licenses/>.
 
 """Send/receive UDP multicast packets.
-
 Requires that your OS kernel supports IP multicast.
 
 This is based on python-examples Demo/sockets/mcast.py
 """
 
-import logging
-import os
-import struct
-from socket import (AF_INET, INADDR_ANY, IP_ADD_MEMBERSHIP, IP_MULTICAST_LOOP,
-                    IP_MULTICAST_TTL, IPPROTO_IP, SO_BROADCAST, SO_REUSEADDR,
-                    SOCK_DGRAM, SOL_IP, SOL_SOCKET, gethostbyname, socket,
-                    timeout, SO_LINGER)
-
 __all__ = ('MulticastSender', 'MulticastReceiver', 'mcast_sender',
            'mcast_receiver', 'SocketTimeout')
 
 # 224.0.0.0 through 224.0.0.255 is reserved administrative tasks
-MC_GROUP = os.environ.get('PYTROLL_MC_GROUP', '225.0.0.212')
+MC_GROUP = '225.0.0.212'
 
 # local network multicast (<32)
-TTL_LOCALNET = int(os.environ.get('PYTROLL_MC_TTL', 31))
+TTL_LOCALNET = 31
 
-logger = logging.getLogger(__name__)
+import struct
+from socket import (socket, AF_INET, SOCK_DGRAM, SOL_SOCKET, SO_REUSEADDR,
+                    SO_BROADCAST, IPPROTO_IP, IP_ADD_MEMBERSHIP, INADDR_ANY,
+                    IP_MULTICAST_TTL, IP_MULTICAST_LOOP, SOL_IP, timeout,
+                    gethostbyname)
 
 SocketTimeout = timeout  # for easy access to socket.timeout
 
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 #
 # Sender.
 #
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 
 
 class MulticastSender(object):
-    """Multicast sender on *port* and *mcgroup*."""
+
+    """Multicast sender on *port* and *mcgroup*.
+    """
 
     def __init__(self, port, mcgroup=MC_GROUP):
         self.port = port
         self.group = mcgroup
         self.socket, self.group = mcast_sender(mcgroup)
-        logger.debug('Started multicast group %s', mcgroup)
 
     def __call__(self, data):
-        self.socket.sendto(data.encode(), (self.group, self.port))
+        self.socket.sendto(data, (self.group, self.port))
 
     def close(self):
-        """Close the sender."""
+        """Close the sender.
+        """
         self.socket.close()
 
 # Allow non-object interface
 
 
 def mcast_sender(mcgroup=MC_GROUP):
     """Non-object interface for sending multicast messages.
     """
     sock = socket(AF_INET, SOCK_DGRAM)
-    try:
-        sock.setsockopt(SOL_SOCKET, SO_REUSEADDR, 1)
-        if _is_broadcast_group(mcgroup):
-            group = '<broadcast>'
-            sock.setsockopt(SOL_SOCKET, SO_BROADCAST, 1)
-        elif((int(mcgroup.split(".")[0]) > 239) or
-             (int(mcgroup.split(".")[0]) < 224)):
-            raise IOError("Invalid multicast address.")
-        else:
-            group = mcgroup
-            ttl = struct.pack('b', TTL_LOCALNET)  # Time-to-live
-            sock.setsockopt(IPPROTO_IP, IP_MULTICAST_TTL, ttl)
-    except Exception:
-        sock.close()
-        raise
+    sock.setsockopt(SOL_SOCKET, SO_REUSEADDR, 1)
+    if _is_broadcast_group(mcgroup):
+        group = '<broadcast>'
+        sock.setsockopt(SOL_SOCKET, SO_BROADCAST, 1)
+    elif((int(mcgroup.split(".")[0]) > 239) or
+         (int(mcgroup.split(".")[0]) < 224)):
+        raise IOError("Invalid multicast address.")
+    else:
+        group = mcgroup
+        ttl = struct.pack('b', TTL_LOCALNET)  # Time-to-live
+        sock.setsockopt(IPPROTO_IP, IP_MULTICAST_TTL, ttl)
     return sock, group
 
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 #
 # Receiver.
 #
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 
 
 class MulticastReceiver(object):
-    """Multicast receiver on *port* for an *mcgroup*."""
+
+    """Multicast receiver on *port* for an *mcgroup*.
+    """
     BUFSIZE = 1024
 
     def __init__(self, port, mcgroup=MC_GROUP):
         # Note: a multicast receiver will also receive broadcast on same port.
         self.port = port
         self.socket, self.group = mcast_receiver(port, mcgroup)
 
@@ -116,19 +111,19 @@
         """A timeout will throw a 'socket.timeout'.
         """
         self.socket.settimeout(tout)
         return self
 
     def __call__(self):
         data, sender = self.socket.recvfrom(self.BUFSIZE)
-        return data.decode(), sender
+        return data, sender
 
     def close(self):
-        """Close the receiver."""
-        self.socket.setsockopt(SOL_SOCKET, SO_LINGER, struct.pack('ii', 1, 1))
+        """Close the receiver.
+        """
         self.socket.close()
 
 # Allow non-object interface
 
 
 def mcast_receiver(port, mcgroup=MC_GROUP):
     """Open a UDP socket, bind it to a port and select a multicast group.
@@ -138,53 +133,49 @@
         group = None
     else:
         group = mcgroup
 
     # Create a socket
     sock = socket(AF_INET, SOCK_DGRAM)
 
-    try:
-        # Allow multiple copies of this program on one machine
-        # (not strictly needed)
-        sock.setsockopt(SOL_SOCKET, SO_REUSEADDR, 1)
-        if group:
-            sock.setsockopt(SOL_IP, IP_MULTICAST_TTL, TTL_LOCALNET)  # default
-            sock.setsockopt(SOL_IP, IP_MULTICAST_LOOP, 1)  # default
-
-        # Bind it to the port
-        sock.bind(('', port))
-
-        # Look up multicast group address in name server
-        # (doesn't hurt if it is already in ddd.ddd.ddd.ddd format)
-        if group:
-            group = gethostbyname(group)
-
-            # Construct binary group address
-            bytes_ = [int(b) for b in group.split(".")]
-            grpaddr = 0
-            for byte in bytes_:
-                grpaddr = (grpaddr << 8) | byte
-
-            # Construct struct mreq from grpaddr and ifaddr
-            ifaddr = INADDR_ANY
-            mreq = struct.pack('!LL', grpaddr, ifaddr)
-
-            # Add group membership
-            sock.setsockopt(IPPROTO_IP, IP_ADD_MEMBERSHIP, mreq)
-    except Exception:
-        sock.close()
-        raise
+    # Allow multiple copies of this program on one machine
+    # (not strictly needed)
+    sock.setsockopt(SOL_SOCKET, SO_REUSEADDR, 1)
+    if group:
+        sock.setsockopt(SOL_IP, IP_MULTICAST_TTL, TTL_LOCALNET)  # default
+        sock.setsockopt(SOL_IP, IP_MULTICAST_LOOP, 1)  # default
+
+    # Bind it to the port
+    sock.bind(('', port))
+
+    # Look up multicast group address in name server
+    # (doesn't hurt if it is already in ddd.ddd.ddd.ddd format)
+    if group:
+        group = gethostbyname(group)
+
+        # Construct binary group address
+        bytes_ = [int(b) for b in group.split(".")]
+        grpaddr = 0
+        for byte in bytes_:
+            grpaddr = (grpaddr << 8) | byte
+
+        # Construct struct mreq from grpaddr and ifaddr
+        ifaddr = INADDR_ANY
+        mreq = struct.pack('!LL', grpaddr, ifaddr)
+
+        # Add group membership
+        sock.setsockopt(IPPROTO_IP, IP_ADD_MEMBERSHIP, mreq)
 
     return sock, group or '<broadcast>'
 
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 #
 # Small helpers.
 #
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 
 
 def _is_broadcast_group(group):
     """Check if *group* is a valid multicasting group.
     """
     if not group or gethostbyname(group) in ('0.0.0.0', '255.255.255.255'):
         return True
```

### Comparing `posttroll-1.9.0/posttroll/logger.py` & `posttroll-v1.1.0/posttroll/logger.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from posttroll.message import Message
 from threading import Thread
 
 import copy
 import logging
 import logging.handlers
 
-LOGGER = logging.getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 
 class PytrollFormatter(logging.Formatter):
 
     """Formats a pytroll message inside a log record.
     """
 
@@ -112,15 +112,16 @@
 class Logger(object):
 
     """The logging machine.
 
     Contains a thread listening to incomming messages, and a thread logging.
     """
 
-    def __init__(self, nameserver_address="localhost", nameserver_port=16543):
+    def __init__(self,
+                 (nameserver_address, nameserver_port)=("localhost", 16543)):
         del nameserver_address, nameserver_port
         self.log_thread = Thread(target=self.log)
         self.loop = True
 
     def start(self):
         """Starts the logging.
         """
@@ -131,46 +132,47 @@
         """
         with Subscribe(services=[""], addr_listener=True) as sub:
             for msg in sub.recv(1):
                 if msg:
                     if msg.type in ["log.debug", "log.info",
                                     "log.warning", "log.error",
                                     "log.critical"]:
-                        getattr(LOGGER, msg.type[4:])(msg.subject + " " +
+                        getattr(logger, msg.type[4:])(msg.subject + " " +
                                                       msg.sender + " " +
                                                       str(msg.data) + " " +
                                                       str(msg.time))
 
                     elif msg.binary:
-                        LOGGER.debug("%s %s %s [binary] %s", msg.subject,
-                                     msg.sender,
-                                     msg.type,
+                        logger.debug(msg.subject + " " +
+                                     msg.sender + " " +
+                                     msg.type + " " +
+                                     "[binary] " +
                                      str(msg.time))
                     else:
-                        LOGGER.debug("%s %s %s %s %s", msg.subject,
-                                     msg.sender,
-                                     msg.type,
-                                     str(msg.data),
+                        logger.debug(msg.subject + " " +
+                                     msg.sender + " " +
+                                     msg.type + " " +
+                                     str(msg.data) + " " +
                                      str(msg.time))
                 if not self.loop:
-                    LOGGER.info("Stop logging")
+                    logger.info("Stop logging")
                     break
 
     def stop(self):
         """Stop the machine.
         """
         self.loop = False
 
 
 def run():
     """Main function
     """
     import argparse
 
-    global LOGGER
+    global logger
 
     parser = argparse.ArgumentParser()
     parser.add_argument("-r", "--rotated", help="Time rotated log file")
     parser.add_argument("-v", "--verbose", help="print debug messages too",
                         action="store_true")
     parser.add_argument("-s", "--server", help="server to listen to",
                         default="localhost")
@@ -187,30 +189,30 @@
     if opts.rotated:
         handler = logging.handlers.TimedRotatingFileHandler(opts.rotated,
                                                             when="midnight",
                                                             backupCount=7)
     else:
         handler = logging.StreamHandler()
 
-    LOGGER = logging.getLogger("pytroll")
-    LOGGER.setLevel(loglevel)
+    logger = logging.getLogger("pytroll")
+    logger.setLevel(loglevel)
 
     handler.setLevel(loglevel)
 
     formatter = ColoredFormatter("[%(asctime)s %(levelname)-19s] %(message)s")
     handler.setFormatter(formatter)
-    LOGGER.addHandler(handler)
+    logger.addHandler(handler)
 
     import time
     try:
-        tlogger = Logger(opts.server, opts.port)
-        # logger = Logger("safe", 16543)
+        tlogger = Logger((opts.server, opts.port))
+        #logger = Logger(("safe", 16543))
         tlogger.start()
         while True:
             time.sleep(1)
     except KeyboardInterrupt:
         tlogger.stop()
-        print("Thanks for using pytroll/logger. "
-              "See you soon on www.pytroll.org!")
+        print ("Thanks for using pytroll/logger. "
+               "See you soon on www.pytroll.org!")
 
 if __name__ == '__main__':
     run()
```

### Comparing `posttroll-1.9.0/posttroll/message.py` & `posttroll-v1.1.0/posttroll/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2010 - 2018, 2021 PyTroll Community
-#
+# Copyright (c) 2010-2012, 2014, 2015.
+
 # Author(s):
-#
+
 #   Lars Ø. Rasmussen <ras@dmi.dk>
 #   Martin Raspaud    <martin.raspaud@smhi.se>
-#   Panu Lahtinen <panu.lahtinen@fmi.fi>
-#
-# This file is part of PyTroll.
-#
+
+# This file is part of pytroll.
+
 # Pytroll is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
-#
+
 # Pytroll is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-#
+
 # You should have received a copy of the GNU General Public License along with
 # pytroll.  If not, see <http://www.gnu.org/licenses/>.
 
 """A Message goes like:
 <subject> <type> <sender> <timestamp> <version> [mime-type data]
 
 ::
@@ -35,15 +34,14 @@
   pytroll://DC/juhu info henry@prodsat 2010-12-01T12:21:11.123456 v1.01 application/json "jhuuuu !!!"
 
 Note: It's not optimized for BIG messages.
 """
 
 import re
 from datetime import datetime
-import _strptime
 try:
     import json
 except ImportError:
     import simplejson as json
 
 from posttroll import strp_isoformat
 
@@ -53,84 +51,77 @@
 
 class MessageError(Exception):
 
     """This modules exceptions.
     """
     pass
 
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 #
 # Utillities.
 #
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 
 
 def is_valid_subject(obj):
     """Currently we only check for empty strings.
     """
-    return isinstance(obj, str) and bool(obj)
+    return isinstance(obj, (str, unicode)) and bool(obj)
 
 
 def is_valid_type(obj):
     """Currently we only check for empty strings.
     """
-    return isinstance(obj, str) and bool(obj)
+    return isinstance(obj, (str, unicode)) and bool(obj)
 
 
 def is_valid_sender(obj):
     """Currently we only check for empty strings.
     """
-    return isinstance(obj, str) and bool(obj)
+    return isinstance(obj, (str, unicode)) and bool(obj)
 
 
 def is_valid_data(obj):
     """Check if data is JSON serializable.
     """
     if obj:
         try:
             tmp = json.dumps(obj, default=datetime_encoder)
             del tmp
         except (TypeError, UnicodeDecodeError):
             return False
     return True
 
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 #
 # Message class.
 #
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 
 
 class Message(object):
 
     """A Message.
 
     - Has to be initialized with a *rawstr* (encoded message to decode) OR
     - Has to be initialized with a *subject*, *type* and optionally *data*, in
       which case:
 
-      - It will add a few extra attributes.
+      - It will add add few extra attributes.
       - It will make a Message pickleable.
     """
 
     def __init__(self, subject='', atype='', data='', binary=False, rawstr=None):
         """Initialize a Message from a subject, type and data...
         or from a raw string.
         """
         if rawstr:
             self.__dict__ = _decode(rawstr)
         else:
-            try:
-                self.subject = subject.decode('utf-8')
-            except AttributeError:
-                self.subject = subject
-            try:
-                self.type = atype.decode('utf-8')
-            except AttributeError:
-                self.type = atype
+            self.subject = subject
             self.type = atype
             self.sender = _getsender()
             self.time = datetime.utcnow()
             self.data = data
             self.binary = binary
         self.version = _VERSION
         self._validate()
@@ -171,23 +162,16 @@
         """
         self._validate()
         return _encode(self, binary=self.binary)
 
     def __repr__(self):
         return self.encode()
 
-    def __unicode__(self):
-        return self.encode()
-
     def __str__(self):
-        try:
-            return unicode(self).encode('utf-8')
-        except NameError:
-            return self.encode()
-
+        return self.encode()
 
     def _validate(self):
         """Validate a messages attributes.
         """
         if not is_valid_subject(self.subject):
             raise MessageError("Invalid subject: '%s'" % self.subject)
         if not is_valid_type(self.type):
@@ -204,19 +188,19 @@
     def __getstate__(self):
         return self.encode()
 
     def __setstate__(self, state):
         self.__dict__.clear()
         self.__dict__ = _decode(state)
 
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 #
 # Decode / encode
 #
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 
 
 def _is_valid_version(version):
     """Check version.
     """
     return version == _VERSION
 
@@ -226,15 +210,15 @@
     """
     if isinstance(dct, list):
         pairs = enumerate(dct)
     elif isinstance(dct, dict):
         pairs = dct.items()
     result = []
     for key, val in pairs:
-        if isinstance(val, str):
+        if isinstance(val, basestring):
             try:
                 val = strp_isoformat(val)
             except ValueError:
                 pass
         elif isinstance(val, (dict, list)):
             val = datetime_decoder(val)
         result.append((key, val))
@@ -244,23 +228,14 @@
         return dict(result)
 
 
 def _decode(rawstr):
     """Convert a raw string to a Message.
     """
     # Check for the magick word.
-    try:
-        rawstr = rawstr.decode('utf-8')
-    except (AttributeError, UnicodeEncodeError):
-        pass
-    except (UnicodeDecodeError):
-        try:
-            rawstr = rawstr.decode('iso-8859-1')
-        except (UnicodeDecodeError):
-            rawstr = rawstr.decode('utf-8', 'ignore')
     if not rawstr.startswith(_MAGICK):
         raise MessageError("This is not a '%s' message (wrong magick word)"
                            % _MAGICK)
     rawstr = rawstr[len(_MAGICK):]
 
     # Check for element count and version
     raw = re.split(r"\s+", rawstr, maxsplit=6)
@@ -314,35 +289,35 @@
     except AttributeError:
         raise TypeError(repr(obj) + " is not JSON serializable")
 
 
 def _encode(msg, head=False, binary=False):
     """Convert a Message to a raw string.
     """
-    rawstr = str(_MAGICK) + u"{0:s} {1:s} {2:s} {3:s} {4:s}".format(
-        msg.subject, msg.type, msg.sender, msg.time.isoformat(), msg.version)
-
+    rawstr = _MAGICK + "%s %s %s %s %s" % \
+        (msg.subject, msg.type, msg.sender,
+         msg.time.isoformat(), msg.version)
     if not head and msg.data:
         if not binary and isinstance(msg.data, str):
             return (rawstr + ' ' +
                     'text/ascii' + ' ' + msg.data)
         elif not binary:
             return (rawstr + ' ' +
                     'application/json' + ' ' +
                     json.dumps(msg.data, default=datetime_encoder))
         else:
             return (rawstr + ' ' +
                     'binary/octet-stream' + ' ' + msg.data)
     return rawstr
 
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 #
 # Small internal helpers.
 #
-# -----------------------------------------------------------------------------
+#-----------------------------------------------------------------------------
 
 
 def _getsender():
     """Return local sender.
     Don't use the getpass module, it looks at various environment variables
     and is unreliable.
     """
```

### Comparing `posttroll-1.9.0/posttroll/ns.py` & `posttroll-v1.1.0/posttroll/ns.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-#
-# Copyright (c) 2011, 2012, 2014, 2015, 2021 Pytroll Community
-#
+
+# Copyright (c) 2011, 2012, 2014, 2015 SMHI
+
 # Author(s):
-#
+
 #   Martin Raspaud <martin.raspaud@smhi.se>
-#   Panu Lahtinen <panu.lahtinen@fmi.fi"
-#
+
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-#
+
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-#
+
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Manage other's subscriptions.
 
 Default port is 5557, if $NAMESERVER_PORT is not defined.
 """
 import logging
-import os
-import time
 from datetime import datetime, timedelta
 
-from threading import Lock
+import time
 # pylint: disable=E0611
-from zmq import LINGER, NOBLOCK, POLLIN, REP, REQ, Poller
+from zmq import REQ, REP, LINGER, POLLIN, NOBLOCK, Poller
+# pylint: enable=E0611
 
-from posttroll import get_context
+from posttroll import context
 from posttroll.address_receiver import AddressReceiver
 from posttroll.message import Message
-
-# pylint: enable=E0611
-
+import os
 
 PORT = int(os.environ.get("NAMESERVER_PORT", 5557))
 
 logger = logging.getLogger(__name__)
 
-nslock = Lock()
 
 class TimeoutError(BaseException):
 
-    """A timeout."""
+    """A timeout.
+    """
     pass
 
 # Client functions.
 
 
 def get_pub_addresses(names=None, timeout=10, nameserver="localhost"):
     """Get the address of the publisher for a given list of publisher *names*
@@ -61,42 +57,43 @@
     """
     addrs = []
     if names is None:
         names = ["", ]
     for name in names:
         then = datetime.now() + timedelta(seconds=timeout)
         while datetime.now() < then:
-            addrs += get_pub_address(name, nameserver=nameserver, timeout=timeout)
+            addrs += get_pub_address(name, nameserver=nameserver)
             if addrs:
                 break
-            time.sleep(timeout / 20.0)
+            time.sleep(.5)
     return addrs
 
 
 def get_pub_address(name, timeout=10, nameserver="localhost"):
     """Get the address of the publisher for a given publisher *name* from the
-    nameserver on *nameserver* (localhost by default)."""
+    nameserver on *nameserver* (localhost by default).
+    """
+
     # Socket to talk to server
-    socket = get_context().socket(REQ)
+    socket = context.socket(REQ)
     try:
-        socket.setsockopt(LINGER, int(timeout * 1000))
+        socket.setsockopt(LINGER, timeout * 1000)
         socket.connect("tcp://" + nameserver + ":" + str(PORT))
-        logger.debug('Connecting to %s',
-                     "tcp://" + nameserver + ":" + str(PORT))
+
         poller = Poller()
         poller.register(socket, POLLIN)
 
         message = Message("/oper/ns", "request", {"service": name})
-        socket.send_string(str(message))
+        socket.send(str(message))
 
         # Get the reply.
         sock = poller.poll(timeout=timeout * 1000)
         if sock:
             if sock[0][0] == socket:
-                message = Message.decode(socket.recv_string(NOBLOCK))
+                message = Message.decode(socket.recv(NOBLOCK))
                 return message.data
         else:
             raise TimeoutError("Didn't get an address after %d seconds."
                                % timeout)
     finally:
         socket.close()
 
@@ -110,60 +107,53 @@
     if addrs:
         return Message("/oper/ns", "info", addrs)
     else:
         return Message("/oper/ns", "info", "")
 
 
 class NameServer(object):
-    """The name server."""
 
-    def __init__(self, max_age=timedelta(minutes=10), multicast_enabled=True, restrict_to_localhost=False):
+    """The name server.
+    """
+
+    def __init__(self, max_age=timedelta(minutes=10)):
         self.loop = True
         self.listener = None
         self._max_age = max_age
-        self._multicast_enabled = multicast_enabled
-        self._restrict_to_localhost = restrict_to_localhost
 
     def run(self, *args):
         """Run the listener and answer to requests.
         """
         del args
 
-        arec = AddressReceiver(max_age=self._max_age,
-                               multicast_enabled=self._multicast_enabled,
-                               restrict_to_localhost=self._restrict_to_localhost)
+        arec = AddressReceiver(max_age=self._max_age)
         arec.start()
         port = PORT
 
         try:
-            with nslock:
-                self.listener = get_context().socket(REP)
-                self.listener.bind("tcp://*:" + str(port))
-                logger.debug('Listening on port %s', str(port))
-                poller = Poller()
-                poller.register(self.listener, POLLIN)
+            self.listener = context.socket(REP)
+            self.listener.bind("tcp://*:" + str(port))
+            poller = Poller()
+            poller.register(self.listener, POLLIN)
             while self.loop:
-                with nslock:
-                    socks = dict(poller.poll(1000))
-                    if socks:
-                        if socks.get(self.listener) == POLLIN:
-                            msg = self.listener.recv_string()
-                    else:
-                        continue
-                    logger.debug("Replying to request: " + str(msg))
-                    msg = Message.decode(msg)
-                    active_address = get_active_address(msg.data["service"], arec)
-                    self.listener.send_unicode(str(active_address))
+                socks = dict(poller.poll(1000))
+                if socks:
+                    if socks.get(self.listener) == POLLIN:
+                        msg = self.listener.recv()
+                else:
+                    continue
+                logger.debug("Replying to request: " + str(msg))
+                msg = Message.decode(msg)
+                self.listener.send_unicode(str(get_active_address(
+                    msg.data["service"], arec)))
         except KeyboardInterrupt:
             # Needed to stop the nameserver.
             pass
         finally:
             arec.stop()
-            self.stop()
+            self.listener.close()
 
     def stop(self):
         """Stop the name server.
         """
-        self.listener.setsockopt(LINGER, 1)
+        self.listener.setsockopt(LINGER, 0)
         self.loop = False
-        with nslock:
-            self.listener.close()
```

### Comparing `posttroll-1.9.0/posttroll/subscriber.py` & `posttroll-v1.1.0/posttroll/subscriber.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,480 +1,400 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-#
-# Copyright (c) 2011, 2012, 2013, 2014, 2015, 2021 Pytroll community
-#
+
+# Copyright (c) 2011, 2012, 2013, 2014, 2015.
+
 # Author(s):
-#
+
 #   Martin Raspaud    <martin.raspaud@smhi.se>
 #   Lars Ø. Rasmussen <ras@dmi.dk>
-#   Panu Lahtinen <panu.lahtinen@fmi.fi>
-#
+
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-#
+
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-#
+
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Simple library to subscribe to messages."""
-
-from time import sleep
+"""Simple library to subscribe to messages.
+"""
 import logging
-import time
 from datetime import datetime, timedelta
-from threading import Lock
-from urllib.parse import urlsplit
+from urlparse import urlsplit
 
+import time
 # pylint: disable=E0611
-from zmq import LINGER, NOBLOCK, POLLIN, PULL, SUB, SUBSCRIBE, Poller, ZMQError
-
+from zmq import (SUB, Poller, LINGER,
+                 POLLIN, SUBSCRIBE, PULL, NOBLOCK, ZMQError)
 # pylint: enable=E0611
-from posttroll import get_context
-from posttroll import _set_tcp_keepalive
-from posttroll.message import _MAGICK, Message
+from posttroll import context
+from posttroll.message import Message, _MAGICK
 from posttroll.ns import get_pub_address
 
-LOGGER = logging.getLogger(__name__)
 
+logger = logging.getLogger(__name__)
+
+
+class Subscriber(object):
 
-class Subscriber:
-    """Class for subscribing to message streams.
+    """Subscriber
 
     Subscribes to *addresses* for *topics*, and perform address translation of
     *translate* is true. The function *message_filter* can be used to
     discriminate some messages on the subscriber side. *topics* on the other
     hand performs filtering on the publishing side (from zeromq 3).
 
     Example::
 
         from posttroll.subscriber import Subscriber, get_pub_address
 
         addr = get_pub_address(service, timeout=2)
         sub = Subscriber([addr], 'my_topic')
         try:
             for msg in sub(timeout=2):
-                print("Consumer got", msg)
+                print "Consumer got", msg
 
         except KeyboardInterrupt:
-            print("terminating consumer...")
+            print "terminating consumer..."
             sub.close()
 
     """
 
-    def __init__(self, addresses, topics='', message_filter=None, translate=False):
-        """Initialize the subscriber."""
+    def __init__(self, addresses, topics='', message_filter=None,
+                 translate=False):
         self._topics = self._magickfy_topics(topics)
         self._filter = message_filter
         self._translate = translate
 
         self.sub_addr = {}
         self.addr_sub = {}
         self.poller = None
 
         self._hooks = []
         self._hooks_cb = {}
 
-        self.poller = Poller()
-        self._lock = Lock()
-
         self.update(addresses)
 
+        self.poller = Poller()
         self._loop = True
 
     def add(self, address, topics=None):
         """Add *address* to the subscribing list for *topics*.
 
         It topics is None we will subscibe to already specified topics.
         """
-        with self._lock:
-            if address in self.addresses:
-                return False
-
-            topics = self._magickfy_topics(topics) or self._topics
-            LOGGER.info("Subscriber adding address %s with topics %s",
-                        str(address), str(topics))
-            subscriber = get_context().socket(SUB)
-            _set_tcp_keepalive(subscriber)
-            for t__ in topics:
-                subscriber.setsockopt_string(SUBSCRIBE, str(t__))
-            subscriber.connect(address)
-            self.sub_addr[subscriber] = address
-            self.addr_sub[address] = subscriber
-            if self.poller:
-                self.poller.register(subscriber, POLLIN)
-            return True
+        if address in self.addresses:
+            return False
+
+        topics = self._magickfy_topics(topics) or self._topics
+        logger.info("Subscriber adding address " + str(address)
+                    + " with topics " + str(topics))
+        subscriber = context.socket(SUB)
+        for t__ in topics:
+            subscriber.setsockopt(SUBSCRIBE, t__)
+        subscriber.connect(address)
+        self.sub_addr[subscriber] = address
+        self.addr_sub[address] = subscriber
+        if self.poller:
+            self.poller.register(subscriber, POLLIN)
+        return True
 
     def remove(self, address):
-        """Remove *address* from the subscribing list for *topics*."""
-        with self._lock:
-            try:
-                subscriber = self.addr_sub[address]
-            except KeyError:
-                return False
-            LOGGER.info("Subscriber removing address %s", str(address))
-            if self.poller:
-                self.poller.unregister(subscriber)
-            del self.addr_sub[address]
-            del self.sub_addr[subscriber]
-            subscriber.close()
-            return True
+        """Remove *address* from the subscribing list for *topics*.
+        """
+        try:
+            subscriber = self.addr_sub[address]
+        except KeyError:
+            return False
+        logger.info("Subscriber removing address " + str(address))
+        if self.poller:
+            self.poller.unregister(subscriber)
+        del self.addr_sub[address]
+        del self.sub_addr[subscriber]
+        subscriber.close()
+        return True
 
     def update(self, addresses):
-        """Update with a set of addresses."""
-        if isinstance(addresses, str):
+        """Updating with a set of addresses.
+        """
+        if isinstance(addresses, (str, unicode)):
             addresses = [addresses, ]
         s0_, s1_ = set(self.addresses), set(addresses)
         sr_, sa_ = s0_.difference(s1_), s1_.difference(s0_)
         for a__ in sr_:
             self.remove(a__)
         for a__ in sa_:
             self.add(a__)
         return bool(sr_ or sa_)
 
     def add_hook_sub(self, address, topics, callback):
-        """Specify a SUB *callback* in the same stream (thread) as the main receive loop.
-
-        The callback will be called with the received messages from the
+        """Specify a *callback* in the same stream (thread) as the main receive
+        loop. The callback will be called with the received messages from the
         specified subscription.
 
         Good for operations, which is required to be done in the same thread as
         the main recieve loop (e.q operations on the underlying sockets).
         """
-        LOGGER.info("Subscriber adding SUB hook %s for topics %s",
-                    str(address), str(topics))
-        socket = get_context().socket(SUB)
+        logger.info("Subscriber adding SUB hook " + str(address)
+                    + " for topics " + str(topics))
+        socket = context.socket(SUB)
         for t__ in self._magickfy_topics(topics):
-            socket.setsockopt_string(SUBSCRIBE, str(t__))
+            socket.setsockopt(SUBSCRIBE, t__)
         socket.connect(address)
         self._add_hook(socket, callback)
 
     def add_hook_pull(self, address, callback):
-        """Specify a PULL *callback* in the same stream (thread) as the main receive loop.
-
-        The callback will be called with the received messages from the
-        specified subscription. Good for pushed 'inproc' messages from another thread.
+        """Same as above, but with a PULL socket.
+        (e.g good for pushed 'inproc' messages from another thread).
         """
-        LOGGER.info("Subscriber adding PULL hook %s", str(address))
-        socket = get_context().socket(PULL)
+        logger("Subscriber adding PULL hook " + str(address))
+        socket = context.socket(PULL)
         socket.connect(address)
         self._add_hook(socket, callback)
 
     def _add_hook(self, socket, callback):
-        """Add a generic hook. The passed socket has to be "receive only"."""
+        """Generic hook. The passed socket has to be "receive only".
+        """
         self._hooks.append(socket)
         self._hooks_cb[socket] = callback
         if self.poller:
             self.poller.register(socket, POLLIN)
 
     @property
     def addresses(self):
-        """Get the addresses."""
+        """Get the addresses
+        """
         return self.sub_addr.values()
 
     @property
     def subscribers(self):
-        """Get the subscribers."""
+        """Get the subscribers
+        """
         return self.sub_addr.keys()
 
     def recv(self, timeout=None):
-        """Receive, optionally with *timeout* in seconds."""
+        """Receive, optionally with *timeout* in seconds.
+        """
         if timeout:
             timeout *= 1000.
 
-        for sub in list(self.subscribers) + self._hooks:
+        for sub in self.subscribers + self._hooks:
             self.poller.register(sub, POLLIN)
         self._loop = True
         try:
             while self._loop:
-                sleep(0)
                 try:
                     socks = dict(self.poller.poll(timeout=timeout))
                     if socks:
                         for sub in self.subscribers:
                             if sub in socks and socks[sub] == POLLIN:
-                                m__ = Message.decode(sub.recv_string(NOBLOCK))
+                                m__ = Message.decode(sub.recv(NOBLOCK))
                                 if not self._filter or self._filter(m__):
                                     if self._translate:
                                         url = urlsplit(self.sub_addr[sub])
                                         host = url[1].split(":")[0]
                                         m__.sender = (m__.sender.split("@")[0]
                                                       + "@" + host)
                                     yield m__
 
                         for sub in self._hooks:
                             if sub in socks and socks[sub] == POLLIN:
-                                m__ = Message.decode(sub.recv_string(NOBLOCK))
+                                m__ = Message.decode(sub.recv(NOBLOCK))
                                 self._hooks_cb[sub](m__)
                     else:
                         # timeout
                         yield None
-                except ZMQError as err:
-                    if self._loop:
-                        LOGGER.exception("Receive failed: %s", str(err))
+                except ZMQError, err:
+                    logger.exception("Receive failed " + str(err))
         finally:
-            for sub in list(self.subscribers) + self._hooks:
+            for sub in self.subscribers + self._hooks:
                 self.poller.unregister(sub)
 
     def __call__(self, **kwargs):
-        """Handle calls with class instance."""
         return self.recv(**kwargs)
 
     def stop(self):
-        """Stop the subscriber."""
+        """Stop the subscriber.
+        """
         self._loop = False
 
     def close(self):
-        """Close the subscriber: stop it and close the local subscribers."""
+        """Close the subscriber: stop it and close the local subscribers.
+        """
         self.stop()
-        for sub in list(self.subscribers) + self._hooks:
-            try:
-                sub.setsockopt(LINGER, 1)
-                sub.close()
-            except ZMQError:
-                pass
+        for sub in self.subscribers + self._hooks:
+            sub.setsockopt(LINGER, 0)
+            sub.close()
 
     @staticmethod
     def _magickfy_topics(topics):
-        """Add the magick to the topics if missing."""
+        """Add the magick to the topics if missing.
+        """
         # If topic does not start with messages._MAGICK (pytroll:/), it will be
         # prepended.
         if topics is None:
             return None
-        if isinstance(topics, str):
+        if isinstance(topics, (str, unicode)):
             topics = [topics, ]
         ts_ = []
         for t__ in topics:
             if not t__.startswith(_MAGICK):
                 if t__ and t__[0] == '/':
                     t__ = _MAGICK + t__
                 else:
                     t__ = _MAGICK + '/' + t__
             ts_.append(t__)
         return ts_
 
     def __del__(self):
-        """Clean up after the instance is deleted."""
-        for sub in list(self.subscribers) + self._hooks:
+        for sub in self.subscribers + self._hooks:
             try:
                 sub.close()
-            except Exception:  # noqa: E722
+            except:
                 pass
 
 
-class NSSubscriber:
-    """Automatically subscribe to *services*.
+class NSSubscriber(object):
 
-    Automatic subscriptions are done by requesting addresses from the
+    """Automatically subscribe to *services* (requesting addresses from the
     nameserver. If *topics* are specified, filter the messages through the
     beginning of the subject. *addr_listener* allows to add new services on the
     fly as they appear on the network. Additional *addresses* to subscribe to
     can be specified, and address translation can be performed if *translate*
     is set to True (False by default). The *timeout* here is specified in
     seconds. The *nameserver* tells which host should be used for nameserver
     requests, defaulting to "localhost".
 
     Note: 'services = None', means no services, and 'services =""' means all
-    services. Default is to listen to all services.
+    services.
     """
 
-    def __init__(self, services="", topics=_MAGICK, addr_listener=False,
+    def __init__(self, services=None, topics=_MAGICK, addr_listener=False,
                  addresses=None, timeout=10, translate=False, nameserver="localhost"):
-        """Initialize the subscriber.
-
-        Note: services = None, means no services
-              services = "", means all services
-
-        Default is to listen to all available services.
+        """ Note: services = None, means no services
+                  services = "", means all services
         """
+
         self._services = _to_array(services)
         self._topics = _to_array(topics)
         self._addresses = _to_array(addresses)
 
         self._timeout = timeout
         self._translate = translate
 
         self._subscriber = None
         self._addr_listener = addr_listener
         self._nameserver = nameserver
 
     def start(self):
-        """Start the subscriber."""
+        """Start the subscriber.
+        """
         def _get_addr_loop(service, timeout):
-            """Try to get the address of *service* until for *timeout* seconds."""
+            """Try to get the address of *service* until for *timeout* seconds.
+            """
             then = datetime.now() + timedelta(seconds=timeout)
             while datetime.now() < then:
                 addrs = get_pub_address(service, nameserver=self._nameserver)
                 if addrs:
                     return [addr["URI"] for addr in addrs]
                 time.sleep(1)
             return []
 
+        # Search for addresses corresponding to service.
+        for service in self._services:
+            addr = _get_addr_loop(service, self._timeout)
+            if not addr:
+                logger.warning("Can't get any address for " + service)
+            else:
+                logger.debug("Got address for " + str(service)
+                             + ": " + str(addr))
+            self._addresses.extend(addr)
+
         # Subscribe to those services and topics.
-        LOGGER.debug("Subscribing to topics %s", str(self._topics))
+        logger.debug("Subscribing to topics " + str(self._topics))
         self._subscriber = Subscriber(self._addresses,
                                       self._topics,
                                       translate=self._translate)
 
         if self._addr_listener:
             self._addr_listener = _AddressListener(self._subscriber,
                                                    self._services,
                                                    nameserver=self._nameserver)
 
-        # Search for addresses corresponding to service.
-        for service in self._services:
-            addresses = _get_addr_loop(service, self._timeout)
-            if not addresses:
-                LOGGER.warning("Can't get any address for %s", service)
-                continue
-            else:
-                LOGGER.debug("Got address for %s: %s",
-                             str(service), str(addresses))
-            for addr in addresses:
-                self._subscriber.add(addr)
-
         return self._subscriber
 
     def stop(self):
-        """Stop the subscriber."""
+        """Stop the subscriber.
+        """
         if self._subscriber is not None:
             self._subscriber.close()
             self._subscriber = None
 
 
-class Subscribe:
-    """Subscriber context.
-
-    See :class:`NSSubscriber` and :class:`Subscriber` for initialization parameters.
+class Subscribe(NSSubscriber):
 
-    The subscriber is selected based on the arguments, see :function:`create_subscriber_from_dict_config` for
-    information how the selection is done.
+    """Subscriber context. See :class:`NSSubscriber` for initialization
+    parameters.
 
     Example::
 
         from posttroll.subscriber import Subscribe
 
         with Subscribe("a_service", "my_topic",) as sub:
             for msg in sub.recv():
-                print(msg)
+                print msg
 
     """
 
-    def __init__(self, services="", topics=_MAGICK, addr_listener=False,
-                 addresses=None, timeout=10, translate=False, nameserver="localhost",
-                 message_filter=None):
-        """Initialize the class."""
-        settings = {
-            'services': services,
-            'topics': topics,
-            'message_filter': message_filter,
-            'translate': translate,
-            'addr_listener': addr_listener,
-            'addresses': addresses,
-            'timeout': timeout,
-            'nameserver': nameserver,
-        }
-        self.subscriber = create_subscriber_from_dict_config(settings)
-
     def __enter__(self):
-        """Start the subscriber when used as a context manager."""
-        return self.subscriber
+        return self.start()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        """Stop the subscriber when used as a context manager."""
-        return self.subscriber.stop()
+        return self.stop()
 
 
 def _to_array(obj):
-    """Convert *obj* to list if not already one."""
-    if isinstance(obj, str):
+    """Convert *obj* to list if not already one.
+    """
+    if isinstance(obj, (str, unicode)):
         return [obj, ]
     if obj is None:
         return []
     return obj
 
 
-class _AddressListener:
-    """Listener for new addresses of interest."""
+class _AddressListener(object):
+
+    """Listener for new addresses of interest.
+    """
 
     def __init__(self, subscriber, services="", nameserver="localhost"):
-        """Initialize address listener."""
-        if isinstance(services, str):
+        if isinstance(services, (str, unicode)):
             services = [services, ]
         self.services = services
         self.subscriber = subscriber
         self.subscriber.add_hook_sub("tcp://" + nameserver + ":16543",
                                      ["pytroll://address", ],
                                      self.handle_msg)
 
     def handle_msg(self, msg):
-        """Handle the message *msg*."""
+        """handle the message *msg*.
+        """
         addr_ = msg.data["URI"]
         status = msg.data.get('status', True)
         if status:
-            msg_services = msg.data.get('service')
+            service = msg.data.get('service')
             for service in self.services:
-                if not service or service in msg_services:
-                    LOGGER.debug("Adding address %s %s", str(addr_),
-                                 str(service))
+                if not service or service in service:
+                    logger.debug("Adding address " + str(addr_)
+                                 + str(service))
                     self.subscriber.add(addr_)
                     break
         else:
-            LOGGER.debug("Removing address %s", str(addr_))
+            logger.debug("Removing address " + str(addr_))
             self.subscriber.remove(addr_)
-
-
-def create_subscriber_from_dict_config(settings):
-    """Get a subscriber class instance defined by a dictionary of configuration options.
-
-    The subscriber is created based on the given options in the following way:
-
-    - setting *settings['addresses']* to a non-empty list AND *settings['nameserver']* to *False*
-      will disable nameserver connections and connect only the listed addresses
-
-    - setting *settings['nameserver']* to a string will connect to nameserver
-      running on the indicated server
-
-    - if *settings['nameserver']* is missing or *None*, the nameserver on localhost is assumed.
-
-    Additional options are described in the docstrings of the respective classes, namely
-    :class:`~posttroll.subscriber.Subscriber` and :class:`~posttroll.subscriber.NSSubscriber`.
-
-    """
-    if settings.get('addresses') and settings.get('nameserver') is False:
-        return _get_subscriber_instance(settings)
-    return _get_nssubscriber_instance(settings).start()
-
-
-def _get_subscriber_instance(settings):
-    addresses = settings['addresses']
-    topics = settings.get('topics', '')
-    message_filter = settings.get('message_filter', None)
-    translate = settings.get('translate', False)
-
-    return Subscriber(addresses, topics=topics, message_filter=message_filter, translate=translate)
-
-
-def _get_nssubscriber_instance(settings):
-    services = settings.get('services', '')
-    topics = settings.get('topics', _MAGICK)
-    addr_listener = settings.get('addr_listener', False)
-    addresses = settings.get('addresses', None)
-    timeout = settings.get('timeout', 10)
-    translate = settings.get('translate', False)
-    nameserver = settings.get('nameserver', 'localhost') or 'localhost'
-
-    return NSSubscriber(
-        services=services,
-        topics=topics,
-        addr_listener=addr_listener,
-        addresses=addresses,
-        timeout=timeout,
-        translate=translate,
-        nameserver=nameserver
-    )
```

### Comparing `posttroll-1.9.0/posttroll.egg-info/SOURCES.txt` & `posttroll-v1.1.0/posttroll.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-LICENSE.txt
-MANIFEST.in
-README.md
 setup.cfg
 setup.py
-versioneer.py
 bin/nameserver
 posttroll/__init__.py
 posttroll/address_receiver.py
 posttroll/bbmcast.py
-posttroll/listener.py
+posttroll/ingester.py
 posttroll/logger.py
 posttroll/message.py
 posttroll/message_broadcaster.py
 posttroll/ns.py
 posttroll/publisher.py
 posttroll/subscriber.py
+posttroll/test_multicast.py
 posttroll/version.py
 posttroll.egg-info/PKG-INFO
 posttroll.egg-info/SOURCES.txt
 posttroll.egg-info/dependency_links.txt
 posttroll.egg-info/entry_points.txt
 posttroll.egg-info/not-zip-safe
 posttroll.egg-info/requires.txt
```

### Comparing `posttroll-1.9.0/setup.py` & `posttroll-v1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# Copyright (c) 2011, 2012, 2014, 2015, 2020.
+# Copyright (c) 2011, 2012, 2014, 2015.
 
 # Author(s):
 
 #   The pytroll team:
 #   Martin Raspaud <martin.raspaud@smhi.se>
 
 # This file is part of pytroll.
@@ -19,27 +19,31 @@
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 
 # You should have received a copy of the GNU General Public License along with
 # this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import setup
-import versioneer
+import sys
+import imp
 
+version = imp.load_source('posttroll.version', 'posttroll/version.py')
 
-requirements = ['pyzmq', 'netifaces', "donfig"]
+
+requirements = ['pyzmq']
+if sys.version_info < (2, 6):
+    requirements.append('simplejson')
 
 
 setup(name="posttroll",
-      version=versioneer.get_version(),
-      cmdclass=versioneer.get_cmdclass(),
+      version=version.__version__,
       description='Messaging system for pytroll',
       author='The pytroll team',
-      author_email='pytroll@googlegroups.com',
-      url="http://github.com/pytroll/posttroll",
+      author_email='martin.raspaud@smhi.se',
+      url="http://github.com/mraspaud/posttroll",
       packages=['posttroll'],
       entry_points={
           'console_scripts': ['pytroll-logger = posttroll.logger:run', ]},
       scripts=['bin/nameserver'],
       zip_safe=False,
       license="GPLv3",
       install_requires=requirements,
@@ -48,10 +52,9 @@
           'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
           'Programming Language :: Python',
           'Operating System :: OS Independent',
           'Intended Audience :: Science/Research',
           'Topic :: Scientific/Engineering',
           'Topic :: Communications'
       ],
-      python_requires='>=3.7',
       test_suite='posttroll.tests.suite',
       )
```

