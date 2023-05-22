# Comparing `tmp/salesea-1.0.7.tar.gz` & `tmp/salesea-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesea-1.0.7.tar", last modified: Thu May 18 10:34:19 2023, max compression
+gzip compressed data, was "salesea-1.0.8.tar", last modified: Mon May 22 05:45:23 2023, max compression
```

## Comparing `salesea-1.0.7.tar` & `salesea-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 10:34:19.784366 salesea-1.0.7/
--rw-rw-rw-   0        0        0     2047 2023-05-18 10:34:19.784366 salesea-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1431 2023-05-18 09:19:56.000000 salesea-1.0.7/README.md
--rw-rw-rw-   0        0        0      111 2023-05-18 10:34:19.785366 salesea-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1844 2023-05-18 10:33:56.000000 salesea-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 10:34:19.766764 salesea-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-18 10:34:19.778366 salesea-1.0.7/src/salesea/
--rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.7/src/salesea/__init__.py
--rw-rw-rw-   0        0        0     1916 2023-05-18 08:27:21.000000 salesea-1.0.7/src/salesea/__main__.py
--rw-rw-rw-   0        0        0     7607 2023-05-18 09:43:08.000000 salesea-1.0.7/src/salesea/app.py
--rw-rw-rw-   0        0        0     3509 2023-05-18 08:19:26.000000 salesea-1.0.7/src/salesea/config.py
--rw-rw-rw-   0        0        0      715 2023-05-18 08:26:30.000000 salesea-1.0.7/src/salesea/log.py
--rw-rw-rw-   0        0        0     7300 2023-05-18 10:33:46.000000 salesea-1.0.7/src/salesea/nginx.py
--rw-rw-rw-   0        0        0      936 2023-05-18 09:22:59.000000 salesea-1.0.7/src/salesea/solution.py
--rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.7/src/salesea/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-18 10:34:19.783366 salesea-1.0.7/src/salesea.egg-info/
--rw-rw-rw-   0        0        0     2047 2023-05-18 10:34:19.000000 salesea-1.0.7/src/salesea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-05-18 10:34:19.000000 salesea-1.0.7/src/salesea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 10:34:19.000000 salesea-1.0.7/src/salesea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-18 10:34:19.000000 salesea-1.0.7/src/salesea.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      150 2023-05-18 10:34:19.000000 salesea-1.0.7/src/salesea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 10:34:19.000000 salesea-1.0.7/src/salesea.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 05:45:23.385628 salesea-1.0.8/
+-rw-rw-rw-   0        0        0     2319 2023-05-22 05:45:23.385628 salesea-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1345 2023-05-22 05:39:22.000000 salesea-1.0.8/README.md
+-rw-rw-rw-   0        0        0      111 2023-05-22 05:45:23.386628 salesea-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2298 2023-05-22 03:40:12.000000 salesea-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 05:45:23.368629 salesea-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 05:45:23.378628 salesea-1.0.8/src/salesea/
+-rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.8/src/salesea/__init__.py
+-rw-rw-rw-   0        0        0     1916 2023-05-18 08:27:21.000000 salesea-1.0.8/src/salesea/__main__.py
+-rw-rw-rw-   0        0        0     7110 2023-05-22 05:38:19.000000 salesea-1.0.8/src/salesea/app.py
+-rw-rw-rw-   0        0        0     3509 2023-05-18 08:19:26.000000 salesea-1.0.8/src/salesea/config.py
+-rw-rw-rw-   0        0        0     1214 2023-05-22 05:27:18.000000 salesea-1.0.8/src/salesea/log.py
+-rw-rw-rw-   0        0        0     7716 2023-05-22 03:01:08.000000 salesea-1.0.8/src/salesea/nginx.py
+-rw-rw-rw-   0        0        0      936 2023-05-18 09:22:59.000000 salesea-1.0.8/src/salesea/solution.py
+-rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.8/src/salesea/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 05:45:23.384628 salesea-1.0.8/src/salesea.egg-info/
+-rw-rw-rw-   0        0        0     2319 2023-05-22 05:45:23.000000 salesea-1.0.8/src/salesea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-05-22 05:45:23.000000 salesea-1.0.8/src/salesea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 05:45:23.000000 salesea-1.0.8/src/salesea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-22 05:45:23.000000 salesea-1.0.8/src/salesea.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-05-22 05:45:23.000000 salesea-1.0.8/src/salesea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 05:45:23.000000 salesea-1.0.8/src/salesea.egg-info/top_level.txt
```

### Comparing `salesea-1.0.7/README.md` & `salesea-1.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -21,30 +21,24 @@
     access_log /to/path/access.log salesea;
   ```
 
 ### Python要求
 
 - Python版本：3.6+
 
-- Python依赖包：
-
-  ```shell
-  pip3 install -r requirements.txt
-  ```
-
 - [conf.ini](conf.ini)配置文件
 
   ```ini
   [nginx]
   server_name = 需要采集的nginx server_name，可以使用*通配符
   nginx_path = 如果你配置了环境变量，可以为空
   [request]
   concurrency = 上传日志并发数
   [salesea]
-  visit_apikey = 上传日志的apikey
+  visit_apikey = salesea的apikey
   interval = 采集间隔，单位秒
   ```
 
 ### 安装
     
 ```shell
 python3 -m pip install salesea -i https://pypi.org/simple
```

### Comparing `salesea-1.0.7/src/salesea/__main__.py` & `salesea-1.0.8/src/salesea/__main__.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.7/src/salesea/app.py` & `salesea-1.0.8/src/salesea/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+# -*- coding: utf-8 -*-
 # 解析Nginx日志, 根据开始时间进行筛选
-import asyncio
+from time import sleep
+
+import requests
 import itertools
 import json
 import os
 import re
-import aiohttp as aiohttp
 from pathlib import Path
 
 from .nginx import Nginx, NginxException
 from .log import logger
 from .solution import print_solution
 
+
 def launch():
     # 将PID写入文件
     pid = os.getpid()
     with open("salesea.pid", "w") as f:
         f.write(str(pid))
     #############################################################################
     #####Global Variable#########################################################
@@ -22,20 +25,19 @@
     nginx = None
 
     #############################################################################
     #####Get Access Servers######################################################
 
     def get_access_servers(server_name=None):
         nginx_path = nginx.nginx_path
-        pattern = server_name.replace(".", "\.").replace("*", ".*?") if server_name is not None else None
         servers = []
         logger.debug(f"nginx_path: {nginx_path}")
         for server in nginx.servers:
             if server.logfile is not None:
-                match = server_name is None or re.match(pattern, server.name)
+                match = server.eq_name(server_name)
                 logger.debug(f"server_name: {server.name} {'匹配' if match else '不匹配'}")
                 if match:
                     servers.append(server)
         return servers
 
     #############################################################################
     #####Parse Nginx Log########################################################
@@ -62,90 +64,85 @@
                         fobj.seek(offset)
                         # 清除0到偏移量之间的内容
                         fobj.truncate(0)
                         break
 
     #############################################################################
     #####Scheduler##############################################################
-    # 使用asyncio实现定时任务
     def scheduler(interval):
         def decorator(func):
-            async def wrapper(*args, **kwargs):
+            def wrapper(*args, **kwargs):
                 while True:
-                    await func(*args, **kwargs)
-                    await asyncio.sleep(interval)
+                    func(*args, **kwargs)
+                    sleep(interval)
 
             return wrapper
 
         return decorator
 
     #############################################################################
     #####Utils###################################################################
     # 迭代器切割
     def chunked(iterable, n):
         for i in range(0, len(iterable), n):
             yield iterable[i:i + n]
 
     #############################################################################
     #####Main###################################################################
-    async def main():
+    def main():
         logfile = "./access.log"
         # 替换所有的$符号为(.*?)，并且将$符号后面的字符串作为分组名
         log_pattern = re.sub(r"\$[a-zA-Z_]\w*", r"(?P<\g<0>>.*?)", LOG_FORMAT)
         log_pattern = log_pattern.replace('$', '').replace('[', '\[').replace(']', '\]')
         servers = get_access_servers(SERVER_NAME)
 
         if servers:
             [logger.info(f'解析到配置：{server.name}:{server.port} >> {server.logfile}') for server in servers]
         else:
             logger.error('未解析到指定的Nginx服务器\n')
             print_solution()
             exit(1)
 
         @scheduler(CHECK_INTERVAL)
-        async def task():
-            # logger.debug(f"开始扫描日志文件：{[str(server.logfile) for p in servers]}")
+        def task():
             count = 0
-            async with aiohttp.ClientSession(headers={
-                'Content-Type': 'application/json'
-            }) as session:
+            with requests.session() as sess:
                 for server in servers:
+                    # logger.debug(f"开始扫描日志文件：{[str(server.logfile) for p in servers]}")
                     nginx_log_iter = parse_nginx_log(server.logfile, log_pattern)
-                    tasks = []
-                    while True:
-                        datas = itertools.islice(nginx_log_iter, REQUEST_CONCURRENCY)
+
+                    for data in nginx_log_iter:
                         try:
-                            for data in datas:
-                                # 使用并发请求
-                                d = re.match(r"[a-zA-Z]+\s(?P<path>/.*?)(?P<query>\?.*?)?\s",
-                                             data['request']).groupdict()
-                                tasks.append(session.post('https://salesea.cn/api/visit', data=json.dumps({
-                                    'visitApiKey': VISIT_APIKEY,
-                                    'domain': server.name or SERVER_NAME or 'localhost',
-                                    'path': d.get('path'),
-                                    'query': d.get('query'),
-                                    'referrer': data['http_referer'],
-                                    'user_agent': data['http_user_agent'],
-                                    'ip': data['remote_addr'],
-                                })))
-                                count += 1
-                            if not tasks:
-                                break
-                            results = await asyncio.gather(*tasks)
-                            for result in results:
-                                text = await result.text()
-                                logger.debug(f"请求结果: {text}")
-                            tasks.clear()
+                            # 使用并发请求
+                            d = re.match(r"[a-zA-Z]+\s(?P<path>/.*?)(?P<query>\?.*?)?\s",
+                                         data['request']).groupdict()
+                            data = {
+                                'visitApiKey': VISIT_APIKEY,
+                                'domain': server.name[0] or SERVER_NAME or 'localhost',
+                                'path': d.get('path'),
+                                'query': d.get('query'),
+                                'referrer': data['http_referer'],
+                                'user_agent': data['http_user_agent'],
+                                'ip': data['remote_addr'],
+                            }
+                            result:requests.Response = sess.post('https://salesea.cn/api/visit', data=json.dumps(data), headers={
+                                'Content-Type': 'application/json'
+                            })
+                            count += 1
+                            obj = result.json()
+                            if obj['code'] == 'error':
+                                logger.error(f"响应错误: {obj} - {data}")
+                            else:
+                                logger.debug(f"响应结果: {obj}")
                         except Exception as e:
-                            logger.error(f"请求错误: {e}")
-                            logger.info(f"请求错误: {data}")
+                            logger.error(f"请求错误: {e} - {data}")
 
             logger.__getattribute__('info' if count else 'debug')(f"解析到[{count}]条日志")
 
-        await task()
+        task()
 
     try:
         from .config import NGINX_PATH, SERVER_NAME, CHECK_INTERVAL, REQUEST_CONCURRENCY, VISIT_APIKEY, LOG_FORMAT
 
         try:
             nginx = Nginx(Path(NGINX_PATH) if NGINX_PATH else None)
         except NginxException as e:
@@ -158,10 +155,10 @@
         logger.debug(f"# nginx_path: {nginx.nginx_path}")
         logger.debug(f"# server_name: {SERVER_NAME}")
         logger.debug(f"# check_interval: {CHECK_INTERVAL}")
         logger.debug(f"# request_concurrency: {REQUEST_CONCURRENCY}")
         logger.debug(f"# visit_apikey: {'*' * 8} ({len(VISIT_APIKEY or '')})")
         logger.debug(f"#" * 65)
 
-        asyncio.get_event_loop().run_until_complete(main())
+        main()
     except KeyboardInterrupt:
         logger.info("用户终止程序")
```

### Comparing `salesea-1.0.7/src/salesea/config.py` & `salesea-1.0.8/src/salesea/config.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.7/src/salesea/nginx.py` & `salesea-1.0.8/src/salesea/nginx.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 # coding: utf-8
 import re
 import os
 import platform
+from http import server
 from pathlib import Path
 
 
 class Server:
     def __init__(self, server_name, server_port, logfile, configs):
-        self.name = server_name
+        self.name: tuple = server_name
         self.port = server_port
         self.logfile = logfile
         self.configs = configs
 
+    def eq_name(self, server_name):
+        pattern = server_name.replace(".", "\.").replace("*", ".*?") if server_name is not None else None
+        if server_name is None:
+            return True
+        for _ in self.name:
+            if re.match(pattern, _) is not None:
+                return True
+
+        return False
+
     @classmethod
     def create(cls, server, nginx_path):
         _server_name = server['server_name']
         _logfile = server['logfile']
         _configs = server['configs']
         _server_port = server['port']
         logfile = Path(_logfile)
@@ -142,14 +153,16 @@
             else:
                 continue
 
             # 判断servername是否有ip，有ip就不存。比如servername 127.0.0.1这样的配置
             if len(re.findall('\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}', servername)) > 0:
                 continue
 
+            servername = tuple(r[0].split())
+
             include = ' '.join(re.findall('include\s+([^;]*);', singleServer))  # include不止一个
             # location可能不止一个
             locations = re.findall('location\s*[\^~\*=]{0,3}\s*([^{ ]*)\s*\{[^}]*proxy_pass\s+https?://([^;/]*)[^;]*;',
                                    singleServer)
 
             backend_list = list()
             backend_ip = ''
```

### Comparing `salesea-1.0.7/src/salesea/solution.py` & `salesea-1.0.8/src/salesea/solution.py`

 * *Files identical despite different names*

