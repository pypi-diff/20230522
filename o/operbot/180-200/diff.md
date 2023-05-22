# Comparing `tmp/operbot-180.tar.gz` & `tmp/operbot-200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operbot-180.tar", last modified: Sat May  6 14:52:38 2023, max compression
+gzip compressed data, was "operbot-200.tar", last modified: Mon May 22 21:29:29 2023, max compression
```

## Comparing `operbot-180.tar` & `operbot-200.tar`

### file list

```diff
@@ -1,55 +1,39 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-06 14:52:38.229128 operbot-180/
--rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-05-06 14:52:38.229128 operbot-180/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     4961 2023-05-06 13:50:40.000000 operbot-180/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-06 14:52:38.225128 operbot-180/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1001)     3306 2023-05-06 13:50:40.000000 operbot-180/bin/operbot
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1717 2023-05-06 14:51:56.000000 operbot-180/bin/operbotcmd
--rwxr-xr-x   0 bart      (1000) bart      (1001)      223 2023-05-06 13:50:40.000000 operbot-180/bin/operbotctl
--rwxr-xr-x   0 bart      (1000) bart      (1001)     2456 2023-05-06 13:50:40.000000 operbot-180/bin/operbotd
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-06 14:52:38.225128 operbot-180/files/
--rw-r--r--   0 bart      (1000) bart      (1001)      312 2023-05-06 13:50:40.000000 operbot-180/files/operbot.service
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-06 14:52:38.229128 operbot-180/operbot/
--rw-r--r--   0 bart      (1000) bart      (1001)      801 2023-05-06 13:50:40.000000 operbot-180/operbot/classes.py
--rw-r--r--   0 bart      (1000) bart      (1001)      621 2023-05-06 13:50:40.000000 operbot-180/operbot/clients.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1168 2023-05-06 13:50:40.000000 operbot-180/operbot/clocked.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1072 2023-05-06 13:50:40.000000 operbot-180/operbot/command.py
--rw-r--r--   0 bart      (1000) bart      (1001)      763 2023-05-06 13:50:40.000000 operbot-180/operbot/decoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      529 2023-05-06 13:50:40.000000 operbot-180/operbot/default.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1153 2023-05-06 13:50:40.000000 operbot-180/operbot/encoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      581 2023-05-06 13:50:40.000000 operbot-180/operbot/errored.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1843 2023-05-06 13:50:40.000000 operbot-180/operbot/handler.py
--rw-r--r--   0 bart      (1000) bart      (1001)      983 2023-05-06 13:50:40.000000 operbot-180/operbot/listens.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2010 2023-05-06 13:50:40.000000 operbot-180/operbot/loggers.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2304 2023-05-06 13:50:40.000000 operbot-180/operbot/message.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-06 14:52:38.229128 operbot-180/operbot/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)      309 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      456 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1001)      553 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1001)    20619 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      810 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1001)     7968 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)      392 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/sts.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1012 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1146 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)      371 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/upt.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3565 2023-05-06 13:50:40.000000 operbot-180/operbot/objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4364 2023-05-06 13:50:40.000000 operbot-180/operbot/persist.py
--rw-r--r--   0 bart      (1000) bart      (1001)      386 2023-05-06 13:50:40.000000 operbot-180/operbot/repeats.py
--rw-r--r--   0 bart      (1000) bart      (1001)      460 2023-05-06 13:50:40.000000 operbot-180/operbot/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2191 2023-05-06 13:50:40.000000 operbot-180/operbot/scanner.py
--rw-r--r--   0 bart      (1000) bart      (1001)      296 2023-05-06 13:50:40.000000 operbot-180/operbot/skipper.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1961 2023-05-06 13:50:40.000000 operbot-180/operbot/threads.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1251 2023-05-06 13:50:40.000000 operbot-180/operbot/utility.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-06 14:52:38.229128 operbot-180/operbot.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-05-06 14:52:38.000000 operbot-180/operbot.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      935 2023-05-06 14:52:38.000000 operbot-180/operbot.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-05-06 14:52:38.000000 operbot-180/operbot.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        8 2023-05-06 14:52:38.000000 operbot-180/operbot.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-05-06 14:52:38.229128 operbot-180/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)     1613 2023-05-06 13:50:40.000000 operbot-180/setup.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-06 14:52:38.229128 operbot-180/test/
--rw-r--r--   0 bart      (1000) bart      (1001)      715 2023-05-06 14:21:03.000000 operbot-180/test/test_decoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      382 2023-05-06 14:51:12.000000 operbot-180/test/test_encoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      903 2023-05-06 13:50:40.000000 operbot-180/test/test_inherit.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4588 2023-05-06 13:50:40.000000 operbot-180/test/test_objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1113 2023-05-06 13:50:40.000000 operbot-180/test/test_storage.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-22 21:29:29.986859 operbot-200/
+-rw-r--r--   0 bart      (1000) bart      (1000)     8213 2023-05-22 21:29:29.986859 operbot-200/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     5446 2023-05-22 18:06:45.000000 operbot-200/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-22 21:29:29.982859 operbot-200/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     2670 2023-05-22 18:06:45.000000 operbot-200/bin/operbot
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     1516 2023-05-22 18:06:45.000000 operbot-200/bin/operbotcmd
+-rwxr-xr-x   0 bart      (1000) bart      (1000)      223 2023-05-22 18:06:45.000000 operbot-200/bin/operbotctl
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     1759 2023-05-22 18:06:45.000000 operbot-200/bin/operbotd
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-22 21:29:29.982859 operbot-200/files/
+-rw-r--r--   0 bart      (1000) bart      (1000)      312 2023-05-22 19:56:20.000000 operbot-200/files/operbot.service
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-22 21:29:29.982859 operbot-200/operbot/
+-rw-r--r--   0 bart      (1000) bart      (1000)      966 2023-05-22 18:06:45.000000 operbot-200/operbot/__init__.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-22 21:29:29.986859 operbot-200/operbot/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      172 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      311 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      184 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/dbg.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      458 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      551 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1088 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    20538 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      798 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2964 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17914 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2410 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     7916 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      390 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/sts.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1000 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1142 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2563 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      371 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/upt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5768 2023-05-22 18:06:45.000000 operbot-200/operbot/modules/wsd.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-22 21:29:29.982859 operbot-200/operbot.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     8213 2023-05-22 21:29:29.000000 operbot-200/operbot.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      689 2023-05-22 21:29:29.000000 operbot-200/operbot.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-05-22 21:29:29.000000 operbot-200/operbot.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        4 2023-05-22 21:29:29.000000 operbot-200/operbot.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        8 2023-05-22 21:29:29.000000 operbot-200/operbot.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-05-22 21:29:29.986859 operbot-200/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)     1337 2023-05-22 21:29:28.000000 operbot-200/setup.py
```

### Comparing `operbot-180/PKG-INFO` & `operbot-200/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: operbot
-Version: 180
+Version: 200
 Summary: operator bot
 Home-page: http://github.com/operbot/operbot
 Author: Bart Thate
-Author-email: operbot100@gmail.com
+Author-email: thatebhj@gmail.com
 License: Public Domain
 Description: README
         ######
         
         
         **NAME**
         
@@ -145,14 +145,43 @@
         
         running the bot in the background is done with the -d option::
         
         
          $ operbot -d
         
         
+        **24/7**
+        
+        paste the following into /etc/systemd/system/operbot.service::
+        
+        
+         [Unit]
+         Description=operator bot
+         After=multi-user.target
+        
+         [Service]
+         Type=forking
+         KillMode=mixed
+         User=operbot
+         Group=operbot
+         DynamicUser=yes
+         StateDirectory=operbot
+         LogsDirectory=operbot
+         CacheDirectory=operbot
+         ExecStart=/usr/local/bin/operbotd
+         CapabilityBoundingSet=CAP_NET_RAW
+        
+         [Install]
+         WantedBy=multi-user.target
+        
+        and run the following with systemctl::
+        
+         > sudo systemctl enable operbot --now
+        
+        
         **COMMANDS**
         
         
         here is a short description of the commands::
         
         
          cfg - show the irc configuration, also edits the config
```

### Comparing `operbot-180/README.rst` & `operbot-200/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -137,14 +137,43 @@
 
 running the bot in the background is done with the -d option::
 
 
  $ operbot -d
 
 
+**24/7**
+
+paste the following into /etc/systemd/system/operbot.service::
+
+
+ [Unit]
+ Description=operator bot
+ After=multi-user.target
+
+ [Service]
+ Type=forking
+ KillMode=mixed
+ User=operbot
+ Group=operbot
+ DynamicUser=yes
+ StateDirectory=operbot
+ LogsDirectory=operbot
+ CacheDirectory=operbot
+ ExecStart=/usr/local/bin/operbotd
+ CapabilityBoundingSet=CAP_NET_RAW
+
+ [Install]
+ WantedBy=multi-user.target
+
+and run the following with systemctl::
+
+ > sudo systemctl enable operbot --now
+
+
 **COMMANDS**
 
 
 here is a short description of the commands::
 
 
  cfg - show the irc configuration, also edits the config
```

### Comparing `operbot-180/bin/operbot` & `operbot-200/bin/operbot`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,60 @@
 #!/usr/bin/env python3
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,W,E0611,E0402
+# pylint: disable=C,I,R,E0611,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
-import getpass
-import pwd
 import os
 import sys
 import termios
 import time
 import traceback
 
 
-from operbot.clients import Client
-from operbot.command import command
-from operbot.errored import Errors
-from operbot.loggers import Logging
-from operbot.message import parse
-from operbot.objects import update
-from operbot.scanner import scandir, scanpkg, importer, starter, threader
-from operbot.runtime import Cfg, date
-from operbot.threads import launch
+sys.path.insert(0, os.getcwd())
 
 
-import operbot.modules
+from opr.clients import Client
+from opr.command import command, scan
+from opr.errored import Errors
+from opr.loggers import Logging
+from opr.message import parse
+from opr.objects import update
+from opr.persist import Persist
+from opr.threads import launch
+
+
+from operbot.modules import cmd, err, flt, irc, log, rss, sts, tdo, thr
+
+
+Persist.workdir = os.path.expanduser("~/.operbot")
+
+
+DATE = time.ctime(time.time()).replace("  ", " ")
+NAME = "operbot"
+
+
+scan(cmd)
+scan(err)
+scan(flt)
+scan(irc)
+scan(log)
+scan(rss)
+scan(sts)
+scan(thr)
+scan(tdo)
 
 
 def cprint(txt):
-    if "v" in Cfg.opts:
-        print(txt)
-        sys.stdout.flush()
+    print(txt)
+    sys.stdout.flush()
 
 
 class CLI(Client):
 
     def announce(self, txt):
         pass
 
@@ -53,15 +70,15 @@
         evt.wait()
 
     def poll(self):
         return self.event(input("> "))
 
 
 def banner():
-    cprint(f"{Cfg.name.upper()} started at {date}")
+    cprint(f"{NAME.upper()} started at {DATE}")
     
 
 def daemon():
     pid = os.fork()
     if pid != 0:
         os._exit(0)
     os.setsid()
@@ -72,66 +89,40 @@
     ses = open('/dev/null', 'a+')
     os.dup2(sos.fileno(), sys.stdout.fileno())
     os.dup2(ses.fileno(), sys.stderr.fileno())
 
 
 def main():
     cfg = parse(' '.join(sys.argv[1:]))
-    update(Cfg, cfg)
-    scanpkg(operbot.modules, importer, doall=True)
-    scandir("mod", importer, doall=True)
-    Logging.raw = cprint
+    if "v" in cfg.opts:
+        Logging.raw = cprint
     dowait = False
     if cfg.txt:
         cli = CLI()
-        command(cli, Cfg.otxt)
-    elif 'd' in Cfg.opts:
+        command(cli, cfg.otxt)
+    elif 'd' in cfg.opts:
         daemon()
         dowait = True
-    elif 'c' in Cfg.opts:
+    elif 'c' in cfg.opts:
         banner()
         csl = Console()
         csl.start()
         dowait = True
     if dowait:
-        for mod in scanpkg(operbot.modules, threader, Cfg.mod):
-            thr = getattr(mod, "_thr", None)
-            if thr:
-                thr.join()
-        for mod in scandir("mod", threader, Cfg.mod):
-            thr = getattr(mod, "_thr", None)
-            if thr:
-                thr.join()
+        irc.start()
+        rss.start()
         while 1:
             time.sleep(1.0)
             waiter()
 
 
-def privileges(username):
-    try:
-        pwnam = pwd.getpwnam(username)
-    except KeyError:
-        username = getpass.getuser()
-        try:
-            pwnam = pwd.getpwnam(username)
-        except KeyError:
-            return username
-    if os.getuid() != 0:
-        return username
-    os.setgroups([])
-    os.setgid(pwnam.pw_gid)
-    os.setuid(pwnam.pw_uid)
-    return username
-
-
 def waiter():
     got = []
     for ex in Errors.errors:
-        if not Cfg.silent:
-            traceback.print_exception(type(ex), ex, ex.__traceback__)
+        traceback.print_exception(type(ex), ex, ex.__traceback__)
         got.append(ex)
     for exc in got:
         Errors.errors.remove(exc)
 
 
 def wrap(func):
     fds = sys.stdin.fileno()
```

### Comparing `operbot-180/bin/operbotcmd` & `operbot-200/bin/operbotd`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 #!/usr/bin/env python3
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0611,E0402,W0212
+# pylint: disable=C,I,R,W,E0611,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
+import getpass
+import pwd
 import os
 import sys
 import termios
+import time
 import traceback
 
 
-from operbot.clients import Client
-from operbot.command import command
-from operbot.errored import Errors
-from operbot.message import parse
-from operbot.objects import update
-from operbot.persist import Persist
-from operbot.scanner import scandir, scanpkg, importer
-from operbot.runtime import Cfg
+from opr.clients import Client
+from opr.command import command, scan
+from opr.errored import Errors
+from opr.loggers import Logging
+from opr.message import parse
+from opr.objects import update
+from opr.persist import Persist
+from opr.threads import launch
 
 
-import operbot.modules
+from operbot.modules import cmd, irc, log, rss, tdo
 
 
 Persist.workdir = "/var/lib/operbot/"
 
 
-def cprint(txt):
-    print(txt)
-    sys.stdout.flush()
+scan(cmd)
+scan(irc)
+scan(log)
+scan(rss)
+scan(tdo)
 
 
-class CLI(Client):
-
-    def announce(self, txt):
-        pass
-
-    def raw(self, txt):
-        cprint(txt)
-
-
-def main():
-    if "INVOCATION_ID" not in os.environ:
-        print("not a systemd")
+def daemon():
+    pid = os.fork()
+    if pid != 0:
         os._exit(0)
-    cfg = parse(' '.join(sys.argv[1:]))
-    update(Cfg, cfg)
-    scanpkg(operbot.modules, importer, doall=True)
-    scandir("mod", importer, doall=True)
-    cli = CLI()
-    evt = command(cli, Cfg.otxt)
-    evt.wait()
+    os.setsid()
+    os.umask(0)
+    sis = open('/dev/null', 'r')
+    os.dup2(sis.fileno(), sys.stdin.fileno())
+    sos = open('/dev/null', 'a+')
+    ses = open('/dev/null', 'a+')
+    os.dup2(sos.fileno(), sys.stdout.fileno())
+    os.dup2(ses.fileno(), sys.stderr.fileno())
 
 
 def waiter():
     got = []
     for ex in Errors.errors:
         if not Cfg.silent:
             traceback.print_exception(type(ex), ex, ex.__traceback__)
@@ -79,9 +76,18 @@
         print('')
     finally:
         if gotterm:
             termios.tcsetattr(fds, termios.TCSADRAIN, old)
         waiter()
 
 
+def main():
+    daemon()
+    irc.start()
+    rss.start()
+    while 1:
+        time.sleep(1.0)
+        waiter()
+
+
 if __name__ == "__main__":
     wrap(main)
```

### Comparing `operbot-180/operbot/encoder.py` & `operbot-200/operbot/modules/fnd.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,49 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,W,E0402
+# pylint: disable=C,I,R,E0401
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
-import json
+import time
 
 
-from .objects import Object
+from opr.objects import keys, prt
+from opr.persist import files, find, fntime
+from opr.utility import elapsed
 
 
 def __dir__():
     return (
-            'ObjectEncoder',
-            'dumps'
+            'fnd',
            )
 
 
 __all__ = __dir__()
 
 
-class ObjectEncoder(json.JSONEncoder):
-
-
-    def default(self, o) -> str:
-        if isinstance(o, dict):
-            return o.items()
-        if isinstance(o, Object):
-            return vars(o)
-        if isinstance(o, list):
-            return iter(o)
-        if isinstance(o,
-                      (type(str), type(True), type(False),
-                       type(int), type(float))
-                     ):
-            return str(o)
-        try:
-            return json.JSONEncoder.default(self, o)
-        except TypeError:
-            return str(o)
-
-    def encode(self, o) -> str:
-        return json.JSONEncoder.encode(self, o)
-
-    def iterencode(self, o, _one_shot=False) -> str:
-        return json.JSONEncoder.iterencode(self, o, _one_shot)
-
-
-def dumps(*args, **kw) -> str:
-    kw["cls"] = ObjectEncoder
-    return json.dumps(*args, **kw)
+def fnd(event):
+    if not event.args:
+        res = ','.join(sorted([x.split('.')[-1].lower() for x in files()]))
+        if res:
+            event.reply(res)
+        else:
+            event.reply('no types yet.')
+        return
+    otype = event.args[0]
+    nmr = 0
+    keyz = None
+    if event.gets:
+        keyz = ','.join(keys(event.gets))
+    if len(event.args) > 1:
+        keyz += ',' + ','.join(event.args[1:])
+    for obj in find(otype, event.gets):
+        if not keyz:
+            keyz = ',' + ','.join(keys(obj))
+        prnt = prt(obj, keyz)
+        lap = elapsed(time.time()-fntime(obj.__oid__))
+        event.reply(f'{nmr} {prnt} {lap}')
+        nmr += 1
+    if not nmr:
+        event.reply(f'no result ({event.txt})')
```

### Comparing `operbot-180/operbot/modules/flt.py` & `operbot-200/operbot/modules/flt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,W,E0402
+# pylint: disable=C,I,R,W,E0401,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 
-from operbot.listens import Listens
-from operbot.objects import kind
+from opr.listens import Listens
+from opr.objects import kind
 
 
 def __dir__():
     return (
             'flt',
            )
```

### Comparing `operbot-180/operbot/modules/irc.py` & `operbot-200/operbot/modules/irc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,W,E0402,E1101
+# pylint: disable=C,I,R,W,E0401,E0402,E1101
 
 
 """internet relay chat
 
 IRC
 
 ::
@@ -52,27 +52,26 @@
 import ssl
 import time
 import textwrap
 import threading
 import _thread
 
 
-from operbot.classes import Classes
-from operbot.clients import Client
-from operbot.command import Command
-from operbot.default import Default
-from operbot.errored import Errors
-from operbot.message import Message
-from operbot.listens import Listens
-from operbot.loggers import Logging
-from operbot.objects import Object, copy, edit, keys, prt, update
-from operbot.persist import find, fntime, last, write
-from operbot.runtime import Cfg
-from operbot.threads import launch
-from operbot.utility import elapsed
+from opr.classes import Classes
+from opr.clients import Client
+from opr.command import Command
+from opr.default import Default
+from opr.errored import Errors
+from opr.message import Message
+from opr.listens import Listens
+from opr.loggers import Logging
+from opr.objects import Object, copy, edit, keys, prt, update
+from opr.persist import find, fntime, last, write
+from opr.threads import launch
+from opr.utility import elapsed
 
 
 def __dir__():
     return (
             'Config',
             'IRC',
             'NoUser',
@@ -83,43 +82,44 @@
             'met'
             'mre',
             'pwd',
             'start'
            )
 
 
+NAME = "operbot"
 saylock = _thread.allocate_lock()
 
 
 def start():
     irc = IRC()
     irc.start()
-    if "v" in Cfg.opts:
+    if "v" in irc.cfg.opts:
         Logging.debug(prt(
                           irc.cfg,
                           ",".join(keys(irc.cfg)),
                           skip='control,password,realname,sleep,username')
                          )
         irc.joined.wait()
     return irc
 
 
 class Config(Default):
 
-    channel = '#%s' % Cfg.name
+    channel = '#%s' % NAME
     control = '!'
-    nick = Cfg.name
+    nick = NAME
     password = ''
     port = 6667
-    realname = Cfg.name
+    realname = NAME
     sasl = False
     server = 'localhost'
     servermodes = ''
     sleep = 60
-    username = Cfg.name
+    username = NAME
     users = False
 
     def __init__(self):
         Default.__init__(self)
         self.control = Config.control
         self.channel = Config.channel
         self.nick = Config.nick
@@ -416,18 +416,18 @@
                 break
 
     def logon(self, server, nck):
         self.connected.wait()
         self.authed.wait()
         self.direct('NICK %s' % nck)
         self.direct(
-                 'USER %s %s %s :%s' % (self.cfg.username or Cfg.name,
+                 'USER %s %s %s :%s' % (self.cfg.username or NAME,
                  server,
                  server,
-                 self.cfg.realname or Cfg.name)
+                 self.cfg.realname or NAME)
                 )
 
     def kill(self, event):
         pass
 
     def log(self, event):
         pass
@@ -595,15 +595,15 @@
         self.connected.clear()
         self.joined.clear()
         launch(Client.start, self)
         launch(Output.start, self)
         launch(
                self.doconnect,
                self.cfg.server or "localhost",
-               self.cfg.nick or Cfg.name,
+               self.cfg.nick or NAME,
                int(self.cfg.port or '6667')
               )
         if not self.keeprunning:
             launch(self.keep)
 
     def stop(self):
         Logging.debug("stopping")
```

### Comparing `operbot-180/operbot/modules/log.py` & `operbot-200/operbot/modules/log.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,W,E0402
+# pylint: disable=C,I,R,E0401,E0402
 
 
 import time
 
 
-from operbot.classes import Classes
-from operbot.persist import find, fntime, write
-from operbot.objects import Object
-from operbot.utility import elapsed
+from opr.classes import Classes
+from opr.persist import find, fntime, write
+from opr.objects import Object
+from opr.utility import elapsed
 
 
 def __dir__():
     return (
             'Log',
             'log',
            )
```

### Comparing `operbot-180/operbot/modules/rss.py` & `operbot-200/operbot/modules/rss.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,W,E0402,E1101
+# pylint: disable=C,I,R,E0401,E0402,E1101
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 import html.parser
@@ -15,22 +15,22 @@
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 from urllib.request import Request, urlopen
 
 
-from operbot.classes import Classes
-from operbot.listens import Listens
-from operbot.objects import Object, prt, update
-from operbot.persist import find, fntime, last, write
-from operbot.repeats import Repeater
-from operbot.runtime import Cfg
-from operbot.threads import launch, threaded
-from operbot.utility import elapsed, spl
+from opr.classes import Classes
+from opr.listens import Listens
+from opr.objects import Object, prt, update
+from opr.persist import find, fntime, last, write
+from opr.repeats import Repeater
+from opr.threads import launch, threaded
+from opr.utility import elapsed, spl
+
 
 def __dir__():
     return (
         'Feed',
         'Fetcher',
         'Repeater',
         'Rss',
@@ -48,14 +48,17 @@
 def start():
     fetcher = Fetcher()
     fetcher.start()
     return fetcher
 
 
 DEBUG = False
+NAME = "operbot"
+
+
 fetchlock = _thread.allocate_lock()
 
 
 class Feed(Object):
 
     pass
 
@@ -191,15 +194,15 @@
             for itm in spl(item):
                 setattr(obj, itm, Parser.getitem(line, itm))
             res.append(obj)
         return res
 
 
 def getfeed(url, item):
-    if Cfg.debug:
+    if DEBUG:
         return [Object(), Object()]
     try:
         result = geturl(url)
     except (ValueError, HTTPError, URLError):
         return [Object(), Object()]
     if not result:
         return [Object(), Object()]
@@ -223,15 +226,15 @@
                 return i.groups()
     return []
 
 
 def geturl(url):
     url = urllib.parse.urlunparse(urllib.parse.urlparse(url))
     req = urllib.request.Request(url)
-    req.add_header('User-agent', useragent(Cfg.name.upper()))
+    req.add_header('User-agent', useragent(NAME))
     with urllib.request.urlopen(req) as response:
         response.data = response.read()
         return response
 
 
 def striphtml(text):
     clean = re.compile('<.*?>')
```

### Comparing `operbot-180/operbot/modules/tdo.py` & `operbot-200/operbot/modules/tdo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,W,E0402
+# pylint: disable=C,I,R,E0401,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 import time
 
 
-from operbot.classes import Classes
-from operbot.objects import Object
-from operbot.persist import find, fntime, write
-from operbot.utility import elapsed
+from opr.classes import Classes
+from opr.objects import Object
+from opr.persist import find, fntime, write
+from opr.utility import elapsed
 
 
 class Todo(Object):
 
     def __init__(self):
         super().__init__()
         self.txt = ''
```

### Comparing `operbot-180/operbot/modules/thr.py` & `operbot-200/operbot/modules/thr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,W,E0402,E1101
+# pylint: disable=C,I,R,E0401,E0402,E1101
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 import threading
 import time
 
 
-from operbot.objects import Object, update
-from operbot.utility import elapsed
+from opr.objects import Object, update
+from opr.utility import elapsed
 
 
 def __dir__():
     return (
             'thr',
            )
```

### Comparing `operbot-180/operbot.egg-info/PKG-INFO` & `operbot-200/operbot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: operbot
-Version: 180
+Version: 200
 Summary: operator bot
 Home-page: http://github.com/operbot/operbot
 Author: Bart Thate
-Author-email: operbot100@gmail.com
+Author-email: thatebhj@gmail.com
 License: Public Domain
 Description: README
         ######
         
         
         **NAME**
         
@@ -145,14 +145,43 @@
         
         running the bot in the background is done with the -d option::
         
         
          $ operbot -d
         
         
+        **24/7**
+        
+        paste the following into /etc/systemd/system/operbot.service::
+        
+        
+         [Unit]
+         Description=operator bot
+         After=multi-user.target
+        
+         [Service]
+         Type=forking
+         KillMode=mixed
+         User=operbot
+         Group=operbot
+         DynamicUser=yes
+         StateDirectory=operbot
+         LogsDirectory=operbot
+         CacheDirectory=operbot
+         ExecStart=/usr/local/bin/operbotd
+         CapabilityBoundingSet=CAP_NET_RAW
+        
+         [Install]
+         WantedBy=multi-user.target
+        
+        and run the following with systemctl::
+        
+         > sudo systemctl enable operbot --now
+        
+        
         **COMMANDS**
         
         
         here is a short description of the commands::
         
         
          cfg - show the irc configuration, also edits the config
```

### Comparing `operbot-180/operbot.egg-info/SOURCES.txt` & `operbot-200/operbot.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,31 @@
 README.rst
 setup.py
 bin/operbot
 bin/operbotcmd
 bin/operbotctl
 bin/operbotd
 files/operbot.service
-operbot/classes.py
-operbot/clients.py
-operbot/clocked.py
-operbot/command.py
-operbot/decoder.py
-operbot/default.py
-operbot/encoder.py
-operbot/errored.py
-operbot/handler.py
-operbot/listens.py
-operbot/loggers.py
-operbot/message.py
-operbot/objects.py
-operbot/persist.py
-operbot/repeats.py
-operbot/runtime.py
-operbot/scanner.py
-operbot/skipper.py
-operbot/threads.py
-operbot/utility.py
+operbot/__init__.py
 operbot.egg-info/PKG-INFO
 operbot.egg-info/SOURCES.txt
 operbot.egg-info/dependency_links.txt
+operbot.egg-info/requires.txt
 operbot.egg-info/top_level.txt
+operbot/modules/__init__.py
 operbot/modules/cmd.py
+operbot/modules/dbg.py
 operbot/modules/err.py
 operbot/modules/flt.py
+operbot/modules/fnd.py
 operbot/modules/irc.py
 operbot/modules/log.py
+operbot/modules/mbx.py
+operbot/modules/mdl.py
+operbot/modules/req.py
 operbot/modules/rss.py
 operbot/modules/sts.py
 operbot/modules/tdo.py
 operbot/modules/thr.py
+operbot/modules/udp.py
 operbot/modules/upt.py
-test/test_decoder.py
-test/test_encoder.py
-test/test_inherit.py
-test/test_objects.py
-test/test_storage.py
+operbot/modules/wsd.py
```

### Comparing `operbot-180/setup.py` & `operbot-200/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,51 @@
-# This file is placed in the Public Domain.
+# This file is placed in the Public Domain
 
 
-"operator bot"
+_author__ = "B.H.J. Thate <thatebhj@gmail.com>"
+__version__ = 1
 
 
 import os
 
 
 from setuptools import setup
 
 
 def read():
     return open("README.rst", "r").read()
 
 
-def uploadlist(dir):
-    upl = []
-    for file in os.listdir(dir):
-        if not file or file.startswith('.'):
-            continue
-        d = dir + os.sep + file
-        if os.path.isdir(d):   
-            upl.extend(uploadlist(d))
-        else:
-            if file.endswith(".pyc") or file.startswith("__pycache"):
-                continue
-            upl.append(d)
-    return upl
-
-
 setup(
     name="operbot",
-    version="180",
+    version="200",
     author="Bart Thate",
-    author_email="operbot100@gmail.com",
+    author_email="thatebhj@gmail.com",
     url="http://github.com/operbot/operbot",
     description="operator bot",
     long_description=read(),
     long_description_content_type="text/x-rst",
     license="Public Domain",
-    packages=["operbot", "operbot.modules"],
-    include_package_data=True,
-    data_files=[
-                ("operbot", ["files/operbot.service",]),
-                ("share/doc/operbot", ["README.rst"])
-               ],
+    install_requires=[
+                      "opr",
+                     ],
+    packages=[
+              "operbot",
+              "operbot.modules"
+             ],
     scripts=[
              "bin/operbot",
              "bin/operbotd",
              "bin/operbotcmd",
              "bin/operbotctl"
             ],
+    include_package_data=True,
+    data_files=[
+                ("operbot", ["files/operbot.service",]),
+               ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: Public Domain",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3 :: Only",
         "Intended Audience :: System Administrators",
         "Topic :: Communications :: Chat :: Internet Relay Chat",
```

