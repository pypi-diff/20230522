# Comparing `tmp/rpqueue-0.33.4.tar.gz` & `tmp/rpqueue-0.33.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rpqueue-0.33.4.tar", last modified: Fri Oct 28 23:35:06 2022, max compression
+gzip compressed data, was "dist/rpqueue-0.33.5.tar", last modified: Mon May 22 19:09:25 2023, max compression
```

## Comparing `rpqueue-0.33.4.tar` & `rpqueue-0.33.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2022-10-28 23:35:06.000000 rpqueue-0.33.4/
-drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2022-10-28 23:35:06.000000 rpqueue-0.33.4/rpqueue/
--rw-rw-r--   0 josiah    (1000) josiah    (1000)     3193 2018-09-26 03:30:44.000000 rpqueue-0.33.4/rpqueue/run.py
--rw-r--r--   0 josiah    (1000) josiah    (1000)    76490 2022-10-28 21:01:55.000000 rpqueue-0.33.4/rpqueue/__init__.py
--rw-r--r--   0 josiah    (1000) josiah    (1000)        6 2022-10-28 23:29:37.000000 rpqueue-0.33.4/VERSION
--rwxrwxr-x   0 josiah    (1000) josiah    (1000)     1331 2022-10-28 20:56:59.000000 rpqueue-0.33.4/setup.py
--rw-rw-r--   0 josiah    (1000) josiah    (1000)    12517 2022-10-28 23:35:06.000000 rpqueue-0.33.4/PKG-INFO
+drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2023-05-22 19:09:25.000000 rpqueue-0.33.5/
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)        6 2023-05-22 19:09:08.000000 rpqueue-0.33.5/VERSION
+drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2023-05-22 19:09:25.000000 rpqueue-0.33.5/rpqueue/
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)    77897 2023-05-22 19:09:08.000000 rpqueue-0.33.5/rpqueue/__init__.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)     3193 2018-09-26 03:30:44.000000 rpqueue-0.33.5/rpqueue/run.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)    12517 2023-05-22 19:09:25.000000 rpqueue-0.33.5/PKG-INFO
+-rwxrwxr-x   0 josiah    (1000) josiah    (1000)     1331 2022-10-28 20:56:59.000000 rpqueue-0.33.5/setup.py
```

### Comparing `rpqueue-0.33.4/rpqueue/run.py` & `rpqueue-0.33.5/rpqueue/run.py`

 * *Files identical despite different names*

### Comparing `rpqueue-0.33.4/rpqueue/__init__.py` & `rpqueue-0.33.5/rpqueue/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     if MED_CLIENT or isinstance(conn, STRICT_CONNS):
         return conn.setex(key, time, value)
     return conn.setex(key, value, time)
 
 if list(map(int, redis.__version__.split('.'))) < [2, 4, 12]:
     raise Exception("Upgrade your Redis client to version 2.4.12 or later")
 
-VERSION = '0.33.4'
+VERSION = '0.33.5'
 
 RPQUEUE_CONFIGS = {}
 
 __all__ = ['VERSION', 'new_rpqueue', 'set_key_prefix',
     'set_redis_connection_settings', 'set_redis_connection',
     'task', 'periodic_task', 'cron_task', 'Task', 'EnqueuedTask', 'Data',
     'get_task', 'result', 'results',
@@ -161,20 +161,48 @@
     '''
     if PY3 and isinstance(pfix, str):
         pfix = pfix.encode('latin-1')
     globals().update((k, pfix+v) for k, v in _NAME_KEYS.items())
     global KEY_PREFIX
     KEY_PREFIX = pfix
 
+class SharedMemoryQuit:
+    """
+    This is a deferred object simply to make sure that this is usable from
+    sources without /dev/shm
+    """
+    def __init__(self):
+        self._v = None
+
+    def _init(self):
+        if not self._v:
+            try:
+                self._v = multiprocessing.Array('i', (0,), lock=False)
+            except:
+                # No /dev/shm? Probably AWS lambda. That's fine.
+                # Just run directly via execute task / use to trigger tasks
+                # running elsewhere / use for data queues
+                log_handler.warning("/dev/shm not available, multiple process may not work properly")
+                raise SystemExit("broken")
+                self._v = [0]
+
+    def __getitem__(self, entry):
+        self._init()
+        return self._v[entry]
+
+    def __setitem__(self, entry, value):
+        self._init()
+        self._v[entry] = value
+
 PY3 = sys.version_info >= (3, 0)
 _SB = (str, bytes) if PY3 else (str, unicode)
 REGISTRY_CHANGED = 0
 REGISTRY = {}
 NEVER_SKIP = set()
-SHOULD_QUIT = multiprocessing.Array('i', (0,), lock=False)
+SHOULD_QUIT = SharedMemoryQuit()
 REENTRY_RETRY = 5
 DEFAULT_QUEUE = b'default'
 DEADLETTER_QUEUE = b'DEADLETTER_QUEUE'
 MINIMUM_DELAY = 1
 EXECUTE_TASKS = False
 QUEUE_ITEMS_PER_PASS = 100
 KEEP_REDIS_TASK_REGISTRY = False
@@ -580,15 +608,14 @@
     last = last or {}
     if not KEEP_REDIS_TASK_REGISTRY or not REGISTRY_CHANGED:
         return last
 
     new = {}
     REGISTRY_CHANGED = 0
     for name, task in REGISTRY.items():
-        queue, name, delay, attempts, retry_delay, save_results, vis_timeout, use_dead, delay
         delay = task.delay
         if isinstance(task.delay, CronTab):
             delay = ' '.join(m.input for m in delay.matchers)
         new[name] = json.dumps([_to_str(task.queue), name, delay, task.never_skip,
             task.attempts, task.retry_delay, task.save_results,
             task.vis_timeout, task.use_dead])
 
@@ -1704,14 +1731,22 @@
 def execute_tasks(queues=None, threads_per_process=1, processes=1, wait_per_thread=1, module=None):
     '''
     Will execute tasks from the (optionally) provided queues until the first
     value in the global SHOULD_QUIT is considered false.
     '''
     global EXECUTE_TASKS
     EXECUTE_TASKS = True
+    # make sure to initialize prior to fork
+    SHOULD_QUIT[0] = 0
+    no_dev_shm = False
+    if type(SHOULD_QUIT._v) is list and processes > 1:
+        log_handler.warning("/dev/shm is not available, reducing processes to 1")
+        processes = 1
+        no_dev_shm = True
+
     signal.signal(signal.SIGUSR1, quit_on_signal)
     signal.signal(signal.SIGTERM, quit_on_signal)
     log_handler.setLevel(LOG_LEVELS[LOG_LEVEL.upper()])
     sp = []
     def _signal_subprocesses(signum, frame):
         for pp in sp:
             if pp.is_alive():
@@ -1720,19 +1755,29 @@
         _print_stackframes_on_signal(signum, frame)
     signal.signal(signal.SIGUSR2, _signal_subprocesses)
 
     threads_per_process = max(threads_per_process, 1)
     processes = max(processes, 1)
     __import__(module) # for any connection modification side-effects
     log_handler.info("Starting %i subprocesses", processes)
-    for p in range(processes):
+    # don't start subprocesses if we can't
+    run_local = processes == 1 and no_dev_shm
+
+    for p in range(processes - run_local):
         pp = multiprocessing.Process(target=execute_task_threads, args=(queues, threads_per_process, 1, module))
         pp.daemon = True
         pp.start()
         sp.append(pp)
+
+    if run_local:
+        # can't run multiprocessing, because we have no /dev/shm :(
+        sp.append(threading.Thread(target=execute_task_threads, args=(queues, threads_per_process, 1, module)))
+        sp[-1].daemon = 1
+        sp[-1].start()
+
     last = {}
     while not SHOULD_QUIT[0]:
         _handle_delayed(get_connection(), queues, 1)
         last = _update_redis_task_registry(last, get_connection())
 
     log_handler.info("Waiting for %i subprocesses to shutdown", len(sp))
     # wait some time for processes to die...
```

### Comparing `rpqueue-0.33.4/setup.py` & `rpqueue-0.33.5/setup.py`

 * *Files identical despite different names*

### Comparing `rpqueue-0.33.4/PKG-INFO` & `rpqueue-0.33.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rpqueue
-Version: 0.33.4
+Version: 0.33.5
 Summary: Use Redis as a priority-enabled and time-based task queue.
 Home-page: https://github.com/josiahcarlson/rpqueue
 Author: Josiah Carlson
 Author-email: josiah.carlson@gmail.com
 License: GNU LGPL v2.1
 Description: 
         Description
```

