# Comparing `tmp/opr-8.tar.gz` & `tmp/opr-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opr-8.tar", last modified: Mon Dec 19 20:18:23 2022, max compression
+gzip compressed data, was "opr-9.tar", last modified: Fri Jan  6 01:44:04 2023, max compression
```

## Comparing `opr-8.tar` & `opr-9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 operbot   (1000) operbot   (1000)        0 2022-12-19 20:18:23.424740 opr-8/
--rw-r--r--   0 operbot   (1000) operbot   (1000)     3275 2022-12-19 20:18:23.424740 opr-8/PKG-INFO
--rw-r--r--   0 operbot   (1000) operbot   (1000)     1916 2022-12-19 20:17:09.000000 opr-8/README.rst
-drwxr-xr-x   0 operbot   (1000) operbot   (1000)        0 2022-12-19 20:18:23.416741 opr-8/opr/
--rw-r--r--   0 operbot   (1000) operbot   (1000)      258 2022-12-19 20:17:09.000000 opr-8/opr/__init__.py
--rw-r--r--   0 operbot   (1000) operbot   (1000)     3538 2022-12-19 20:17:09.000000 opr-8/opr/handler.py
--rw-r--r--   0 operbot   (1000) operbot   (1000)     2771 2022-12-19 20:17:09.000000 opr-8/opr/message.py
--rw-r--r--   0 operbot   (1000) operbot   (1000)    13127 2022-12-19 20:17:09.000000 opr-8/opr/objects.py
--rw-r--r--   0 operbot   (1000) operbot   (1000)     1993 2022-12-19 20:17:09.000000 opr-8/opr/running.py
--rw-r--r--   0 operbot   (1000) operbot   (1000)     3803 2022-12-19 20:17:09.000000 opr-8/opr/threads.py
-drwxr-xr-x   0 operbot   (1000) operbot   (1000)        0 2022-12-19 20:18:23.420740 opr-8/opr.egg-info/
--rw-r--r--   0 operbot   (1000) operbot   (1000)     3275 2022-12-19 20:18:23.000000 opr-8/opr.egg-info/PKG-INFO
--rw-r--r--   0 operbot   (1000) operbot   (1000)      337 2022-12-19 20:18:23.000000 opr-8/opr.egg-info/SOURCES.txt
--rw-r--r--   0 operbot   (1000) operbot   (1000)        1 2022-12-19 20:18:23.000000 opr-8/opr.egg-info/dependency_links.txt
--rw-r--r--   0 operbot   (1000) operbot   (1000)        4 2022-12-19 20:18:23.000000 opr-8/opr.egg-info/top_level.txt
--rw-r--r--   0 operbot   (1000) operbot   (1000)       38 2022-12-19 20:18:23.424740 opr-8/setup.cfg
--rw-r--r--   0 operbot   (1000) operbot   (1000)     1325 2022-12-19 20:17:09.000000 opr-8/setup.py
-drwxr-xr-x   0 operbot   (1000) operbot   (1000)        0 2022-12-19 20:18:23.424740 opr-8/test/
--rw-r--r--   0 operbot   (1000) operbot   (1000)      941 2022-12-19 20:17:09.000000 opr-8/test/test_bus.py
--rw-r--r--   0 operbot   (1000) operbot   (1000)      269 2022-12-19 20:17:09.000000 opr-8/test/test_evt.py
--rw-r--r--   0 operbot   (1000) operbot   (1000)      279 2022-12-19 20:17:09.000000 opr-8/test/test_hdl.py
--rw-r--r--   0 operbot   (1000) operbot   (1000)     5773 2022-12-19 20:17:09.000000 opr-8/test/test_obj.py
--rw-r--r--   0 operbot   (1000) operbot   (1000)      358 2022-12-19 20:17:09.000000 opr-8/test/test_pth.py
--rw-r--r--   0 operbot   (1000) operbot   (1000)      306 2022-12-19 20:17:09.000000 opr-8/test/test_thr.py
--rw-r--r--   0 operbot   (1000) operbot   (1000)      309 2022-12-19 20:17:09.000000 opr-8/test/test_tmr.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-06 01:44:04.344559 opr-9/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3275 2023-01-06 01:44:04.344559 opr-9/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1916 2023-01-04 14:37:17.000000 opr-9/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-06 01:44:04.344559 opr-9/opr/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1585 2023-01-06 01:04:39.000000 opr-9/opr/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3303 2023-01-05 14:01:09.000000 opr-9/opr/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2822 2023-01-05 15:24:19.000000 opr-9/opr/message.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    13127 2023-01-06 01:05:10.000000 opr-9/opr/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2487 2023-01-06 00:46:08.000000 opr-9/opr/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3840 2023-01-04 14:37:17.000000 opr-9/opr/threads.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-06 01:44:04.344559 opr-9/opr.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3275 2023-01-06 01:44:04.000000 opr-9/opr.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      337 2023-01-06 01:44:04.000000 opr-9/opr.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-01-06 01:44:04.000000 opr-9/opr.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        4 2023-01-06 01:44:04.000000 opr-9/opr.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-01-06 01:44:04.344559 opr-9/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)     1325 2023-01-05 23:31:27.000000 opr-9/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-06 01:44:04.344559 opr-9/test/
+-rw-r--r--   0 bart      (1000) bart      (1000)      941 2023-01-04 14:37:17.000000 opr-9/test/test_bus.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      269 2023-01-04 14:37:17.000000 opr-9/test/test_evt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      279 2023-01-04 14:37:17.000000 opr-9/test/test_hdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5773 2023-01-04 14:37:17.000000 opr-9/test/test_obj.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      358 2023-01-04 14:37:17.000000 opr-9/test/test_pth.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      306 2023-01-04 14:37:17.000000 opr-9/test/test_thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      309 2023-01-04 14:37:17.000000 opr-9/test/test_tmr.py
```

### Comparing `opr-8/PKG-INFO` & `opr-9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opr
-Version: 8
+Version: 9
 Summary: object programming runtime
 Home-page: http://github.com/operbot/opr
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
```

### Comparing `opr-8/README.rst` & `opr-9/README.rst`

 * *Files identical despite different names*

### Comparing `opr-8/opr/handler.py` & `opr-9/opr/handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # This file is placed in the Public Domain.
 # pylint: disable=C0115,C0116,W0703,W0201,R0902,R0903,W0613,R0201,E0402
 
 
 "handler"
 
 
-import inspect
 import queue
-import sys
 import threading
 import time
 
 
 from .objects import Object
 from .threads import launch
 
 
 def __dir__():
     return (
             'Bus',
             'Callback',
             'Command',
             'Handler',
-            'scan',
            )
 
 
 __all__ = __dir__()
 
 
+
 class Bus(Object):
 
     objs = []
 
     @staticmethod
     def add(obj):
         if repr(obj) not in [repr(x) for x in Bus.objs]:
@@ -60,30 +58,34 @@
 
 
 class Callback(Object):
 
     cbs = Object()
     errors = []
 
-    def register(self, typ, cbs):
-        if typ not in self.cbs:
-            setattr(self.cbs, typ, cbs)
+    @staticmethod
+    def register(typ, cbs):
+        if typ not in Callback.cbs:
+            setattr(Callback.cbs, typ, cbs)
 
-    def callback(self, event):
-        func = getattr(self.cbs, event.type, None)
+    @staticmethod
+    def callback(event):
+        func = getattr(Callback.cbs, event.type, None)
         if not func:
             event.ready()
             return
         event.__thr__ = launch(func, event)
 
-    def dispatch(self, event):
-        self.callback(event)
+    @staticmethod
+    def dispatch(event):
+        Callback.callback(event)
 
-    def get(self, typ):
-        return getattr(self.cbs, typ)
+    @staticmethod
+    def get(typ):
+        return getattr(Callback.cbs, typ)
 
 
 class Command(Object):
 
     cmd = Object()
     errors = []
 
@@ -100,16 +102,15 @@
         if not evt.isparsed:
             evt.parse()
         func = Command.get(evt.cmd)
         if func:
             try:
                 func(evt)
             except Exception as ex:
-                tbk = sys.exc_info()[2]
-                evt.__exc__ = ex.with_traceback(tbk)
+                evt.__exc__ = ex.with_traceback(ex.__traceback__)
                 Command.errors.append(evt)
                 evt.ready()
                 return None
             evt.show()
         evt.ready()
         return None
 
@@ -132,15 +133,15 @@
     def add(cmd):
         Command.add(cmd)
 
     def announce(self, txt):
         self.raw(txt)
 
     def handle(self, event):
-        self.dispatch(event)
+        Callback.dispatch(event)
 
     def loop(self):
         while not self.stopped.set():
             self.handle(self.poll())
 
     def poll(self):
         return self.queue.get()
@@ -164,16 +165,7 @@
     def start(self):
         self.stopped.clear()
         self.loop()
 
     def wait(self):
         while 1:
             time.sleep(1.0)
-
-
-def scan(mod):
-    for key, cmd in inspect.getmembers(mod, inspect.isfunction):
-        if key.startswith("cb"):
-            continue
-        names = cmd.__code__.co_varnames
-        if "event" in names:
-            Command.add(cmd)
```

### Comparing `opr-8/opr/message.py` & `opr-9/opr/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # This file is placed in the Public Domain.
 # pylint: disable=C0115,C0116,W0703,W0201,R0902,R0903,W0613,R0201,C0103,E0402
 
 
-"event"
+"message"
 
 
 import threading
 import time
 
 
-from .objects import Default, register
+from .objects import Class, Default, register
 from .handler import Bus
 from .threads import elapsed
 
 
 def __dir__():
     return  (
              "Parsed",
@@ -69,14 +69,17 @@
             self.args = args
             self.rest = " ".join(args)
             self.txt = self.cmd + " " + self.rest
         else:
             self.txt = self.cmd
 
 
+Class.add(Parsed)
+
+
 class Event(Parsed):
 
 
     def __init__(self):
         Parsed.__init__(self)
         self.__ready__ = threading.Event()
         self.__thr__ = None
@@ -92,17 +95,17 @@
         pass
 
     def done(self):
         diff = elapsed(time.time()-self.createtime)
         Bus.say(self.orig, self.channel, f'ok {diff}')
 
     def ok(self, txt=None):
-        text = "ok " + txt or ""
+        text = "ok " + (txt or "")
         text = text.rstrip()
-        Bus.say(self.orig, self.channel, txt)
+        Bus.say(self.orig, self.channel, text)
 
     def ready(self):
         self.__ready__.set()
 
     def reply(self, txt):
         self.result.append(txt)
 
@@ -110,7 +113,10 @@
         for txt in self.result:
             Bus.say(self.orig, self.channel, txt)
 
     def wait(self):
         if self.__thr__:
             self.__thr__.join()
         self.__ready__.wait()
+
+
+Class.add(Event)
```

### Comparing `opr-8/opr/objects.py` & `opr-9/opr/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,55 @@
 # This file is placed in the Public Domain.
 # pylint: disable=C0112,C0115,C0116,W0613,W0108,R0903
 
 
-"""big Object
+"""objects
 
 
 this module contains a big Object class that provides a clean, no methods,
 namespace for json data to be read into. this is necessary so that methods
 don't get overwritten by __dict__ updating and, without methods defined on
 the object, is easily being updated from a on disk stored json (dict).
 
 basic usage is this:
 
->>> import cmdz
->>> o = cmdz.Object()
+>>> import opr
+>>> o = opr.Object()
 >>> o.key = "value"
 >>> o.key
 'value'
 
 Some hidden methods are provided, methods are factored out into functions
 like get, items, keys, register, set, update and values.
 
 load/save from/to disk:
 
->>> from cmdz import Object, load, save
+>>> from opr import Object, load, save
 >>> o = Object()
 >>> o.key = "value"
 >>> p = save(o)
 >>> oo = Object()
 >>> load(oo, p)
 >>> oo.key
 'value'
 
 big Objects can be searched with database functions and uses read-only files
 to improve persistence and a type in filename for reconstruction:
 
-'cmdz.object.Object/11ee5f11bd874f1eaa9005980f9d7a94/2021-08-31/15:31:05.717063'
-
->>> from cmdz import Object, save
+>>> from opr import Object, save
 >>> o = Object()
 >>> save(o)  # doctest: +ELLIPSIS
-'cmdz.object.Object/...'
+'opr.objects.Object/...'
 
 great for giving objects peristence by having their state stored in files.
 
 """
 
 
 import datetime
-import inspect
 import json
 import os
 import pathlib
 import time
 import uuid
 import _thread
 
@@ -81,15 +78,14 @@
             'load',
             'loads',
             'locked',
             'match',
             'printable',
             'register',
             'save',
-            'scan',
             'spl',
             'update',
             'values',
             'write'
            )
 
 
@@ -367,23 +363,23 @@
     @staticmethod
     def last(otp, selector=None, index=None, timed=None):
         res =  sorted(Db.find(otp, selector, index, timed), key=lambda x: fntime(x.__fnm__))
         if res:
             return res[-1]
         return None
 
+
 def fnclass(path):
-    pth = []
     try:
         _rest, *pth = path.split("store")
+        splitted = pth[0].split(os.sep)
+        return splitted[1]
     except ValueError:
         pass
-    if not pth:
-        pth = path.split(os.sep)
-    return pth[0]
+    return None
 
 
 def fns(otp, timed=None):
     if not otp:
         return []
     assert Wd.workdir
     path = os.path.join(Wd.workdir, "store", otp) + os.sep
@@ -405,14 +401,15 @@
                     ):
                         continue
                     if timed and timed.to and fntime(path2) > timed.to:
                         continue
                     res.append(path2)
     return sorted(res, key=lambda x: fntime(x))
 
+
 def fntime(daystr):
     daystr = daystr.replace("_", ":")
     datestr = " ".join(daystr.split(os.sep)[-2:])
     if "." in datestr:
         datestr, rest = datestr.rsplit(".", 1)
     else:
         rest = ""
@@ -520,15 +517,23 @@
 
     @staticmethod
     def getpath(path):
         return os.path.join(Wd.get(), "store", path)
 
     @staticmethod
     def moddir():
-        return os.path.join(Wd.get(), "mod")
+        mdr = os.path.join(Wd.get(), "mod")
+        cdir(mdr)
+        return mdr
+
+    @staticmethod
+    def nmdir():
+        mdr = os.path.join(Wd.get(), "notmod")
+        cdir(mdr)
+        return mdr
 
     @staticmethod
     def set(path):
         Wd.workdir = path
 
     @staticmethod
     def storedir():
@@ -545,25 +550,22 @@
                 continue
             if fnm not in res:
                 res.append(fnm)
         return res
 
 
 def cdir(path):
-    if not os.path.isdir(path):
+    path = os.path.abspath(path)
+    fname = path.split(os.sep)[-1]
+    if fname.count(":") == 2:
         path = os.path.dirname(path)
     ppp = pathlib.Path(path)
     ppp.mkdir(parents=True, exist_ok=True)
 
 
-def scan(mod):
-    for _key, clz in inspect.getmembers(mod, inspect.isclass):
-        Class.add(clz)
-
-
 def spl(txt):
     try:
         res = txt.split(",")
     except (TypeError, ValueError):
         res = txt
     return [x for x in res if x]
```

### Comparing `opr-8/opr/running.py` & `opr-9/opr/runtime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 # This file is placed in the Public Domain.
 # pylint: disable=C0115,C0116,C0411,C0413,W0212,R0903,W0201,E0402,W0613
 
 
 "runtime"
 
 
+import inspect
 import os
-import sys
 import time
 
 
-from .handler import scan
 from .message import Event, Parsed
-from .objects import Default, spl, update
+from .handler import Command
+from .objects import Class, Default, spl, update
 
 
 def __dir__():
     return (
             "Cfg",
             "Console",
             "boot",
             "command",
             "parse",
-            'scanner',
+            'scanpkg',
             'scandir',
             "wait"
            )
 
 
 class Config(Default):
 
     pass
 
 
-def boot():
-    prs = parse()
+Class.add(Config)
+
+
+def boot(txt):
+    prs = parse(txt)
     if "c" in prs.opts:
         Cfg.console = True
     if "d" in prs.opts:
         Cfg.daemon= True
     if "v" in prs.opts:
         Cfg.verbose = True
     if "w" in prs.opts:
         Cfg.wait = True
+    if "x" in prs.opts:
+        Cfg.exec = True
     update(Cfg.prs, prs)
     update(Cfg, prs.sets)
 
 
 def command(cli, txt, event=None):
     evt = (event() if event else Event())
     evt.parse(txt)
@@ -70,41 +75,54 @@
     for fnm in os.listdir(path):
         if fnm.endswith("~") or fnm.startswith("__"):
             continue
         res.append(fnm.split(os.sep)[-1][:-3])
     return res
 
 
-def parse(txt=None):
-    if txt is None:
-        txt = " ".join(sys.argv[1:])
+def parse(txt):
     prs = Parsed()
     prs.parse(txt)
     update(Cfg.prs, prs)
     return prs
 
 
-def scanner(pkg, importer, mods=None):
+def scan(mod):
+    for key, cmd in inspect.getmembers(mod, inspect.isfunction):
+        if key.startswith("cb"):
+            continue
+        names = cmd.__code__.co_varnames
+        if "event" in names:
+            Command.add(cmd)
+
+
+def scanpkg(pkg, importer, mods=None):
     path = pkg.__path__[0]
     name = pkg.__name__
-    scandir(path, importer, name, mods)
+    return scandir(path, importer, name)
 
 
-def scandir(path, importer, pname, mods=None):
+def scandir(path, importer, pname=None, mods=None):
+    res = []
+    if pname is None:
+        pname = path.split(os.sep)[-1]
     for modname in listmod(path):
+        if not modname:
+            continue
         if mods and not include(modname, spl(mods)):
             continue
         mname = "%s.%s" % (pname, modname)
-        mod = importer(mname, path)
-        scan(mod)
+        ppath = os.path.join(path, "%s.py" % modname)
+        mod = importer(mname, ppath)
+        res.append(mod)
+    return res
 
 
-def wait():
+def wait(func=None):
     while 1:
         time.sleep(1.0)
-
-
-## runtime
+        if func:
+            func()
 
 
 Cfg = Config()
 Cfg.prs = Parsed()
```

### Comparing `opr-8/opr/threads.py` & `opr-9/opr/threads.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is placed in the Public Domain.
 # pylint: disable=C0112,C0115,C0116,R0902
 
 
-"thread"
+"threads"
 
 
 import queue
 import threading
 import time
 import types
 
@@ -160,9 +160,9 @@
     if "__self__" in dir(obj):
         return "%s.%s" % (obj.__self__.__class__.__name__, obj.__name__)
     if "__class__" in dir(obj) and "__name__" in dir(obj):
         return "%s.%s" % (obj.__class__.__name__, obj.__name__)
     if "__class__" in dir(obj):
         return obj.__class__.__name__
     if "__name__" in dir(obj):
-        return obj.__name__
+        return "%s.%s" % (obj.__class__.__name__, obj.__name__)
     return None
```

### Comparing `opr-8/opr.egg-info/PKG-INFO` & `opr-9/opr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opr
-Version: 8
+Version: 9
 Summary: object programming runtime
 Home-page: http://github.com/operbot/opr
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
```

### Comparing `opr-8/setup.py` & `opr-9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 continue
             upl.append(d)
     return upl
 
 
 setup(
     name="opr",
-    version="8",
+    version="9",
     author="Bart Thate",
     author_email="operbot100@gmail.com",
     url="http://github.com/operbot/opr",
     description="object programming runtime",
     long_description=read(),
     long_description_content_type="text/x-rst",
     license="Public Domain",
```

### Comparing `opr-8/test/test_bus.py` & `opr-9/test/test_bus.py`

 * *Files identical despite different names*

### Comparing `opr-8/test/test_obj.py` & `opr-9/test/test_obj.py`

 * *Files identical despite different names*

