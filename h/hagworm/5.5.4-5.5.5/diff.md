# Comparing `tmp/hagworm-5.5.4.tar.gz` & `tmp/hagworm-5.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagworm-5.5.4.tar", last modified: Sat May 20 03:16:49 2023, max compression
+gzip compressed data, was "hagworm-5.5.5.tar", last modified: Mon May 22 03:51:14 2023, max compression
```

## Comparing `hagworm-5.5.4.tar` & `hagworm-5.5.5.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.729966 hagworm-5.5.4/
--rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.5.4/LICENSE
--rw-rw-rw-   0        0        0     7515 2023-05-20 03:16:49.728966 hagworm-5.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.5.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.623966 hagworm-5.5.4/c_extend/
--rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.5.4/c_extend/math.c
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.626965 hagworm-5.5.4/example/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.632966 hagworm-5.5.4/example/fastapi_demo/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/example/fastapi_demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.635966 hagworm-5.5.4/example/fastapi_demo/controller/
--rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.5.4/example/fastapi_demo/controller/__init__.py
--rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.5.4/example/fastapi_demo/controller/home.py
--rw-rw-rw-   0        0        0      888 2023-05-11 03:07:54.000000 hagworm-5.5.4/example/fastapi_demo/gunicorn.config.py
--rw-rw-rw-   0        0        0     1431 2023-05-17 08:11:13.000000 hagworm-5.5.4/example/fastapi_demo/main.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.637966 hagworm-5.5.4/example/fastapi_demo/model/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/example/fastapi_demo/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.638966 hagworm-5.5.4/example/fastapi_demo/service/
--rw-rw-rw-   0        0        0     3496 2023-03-01 02:07:14.000000 hagworm-5.5.4/example/fastapi_demo/service/__init__.py
--rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.5.4/example/fastapi_demo/setting.py
--rw-rw-rw-   0        0        0      800 2023-05-11 03:07:54.000000 hagworm-5.5.4/example/main_test.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.640966 hagworm-5.5.4/hagworm/
--rw-rw-rw-   0        0        0      495 2023-05-20 02:40:17.000000 hagworm-5.5.4/hagworm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.676965 hagworm-5.5.4/hagworm/extend/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.704965 hagworm-5.5.4/hagworm/extend/asyncio/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/asyncio/__init__.py
--rw-rw-rw-   0        0        0    16802 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/asyncio/base.py
--rw-rw-rw-   0        0        0     4988 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/asyncio/buffer.py
--rw-rw-rw-   0        0        0     2396 2023-05-11 03:07:54.000000 hagworm-5.5.4/hagworm/extend/asyncio/command.py
--rw-rw-rw-   0        0        0     2432 2023-05-18 10:57:40.000000 hagworm-5.5.4/hagworm/extend/asyncio/etcd.py
--rw-rw-rw-   0        0        0     3194 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/asyncio/event.py
--rw-rw-rw-   0        0        0     1370 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/asyncio/file.py
--rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/asyncio/future.py
--rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/asyncio/mail.py
--rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/asyncio/mongo.py
--rw-rw-rw-   0        0        0    15022 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/asyncio/mysql.py
--rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/asyncio/net.py
--rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/asyncio/ntp.py
--rw-rw-rw-   0        0        0     1570 2023-05-20 02:55:55.000000 hagworm-5.5.4/hagworm/extend/asyncio/pool.py
--rw-rw-rw-   0        0        0    12506 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/asyncio/redis.py
--rw-rw-rw-   0        0        0     7279 2023-05-11 03:07:54.000000 hagworm-5.5.4/hagworm/extend/asyncio/socket.py
--rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.5.4/hagworm/extend/asyncio/task.py
--rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/asyncio/transaction.py
--rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/asyncio/zmq.py
--rw-rw-rw-   0        0        0    22623 2023-05-11 03:07:54.000000 hagworm-5.5.4/hagworm/extend/base.py
--rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/cache.py
--rw-rw-rw-   0        0        0     1839 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/compile.py
--rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/config.py
--rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/crypto.py
--rw-rw-rw-   0        0        0     1792 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/error.py
--rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/event.py
--rw-rw-rw-   0        0        0     4558 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/igraph.py
--rw-rw-rw-   0        0        0     2326 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/interface.py
--rw-rw-rw-   0        0        0    14870 2023-05-13 05:06:56.000000 hagworm-5.5.4/hagworm/extend/logging.py
--rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/media.py
--rw-rw-rw-   0        0        0     1603 2023-05-10 07:58:09.000000 hagworm-5.5.4/hagworm/extend/metaclass.py
--rw-rw-rw-   0        0        0     4500 2023-05-11 03:07:54.000000 hagworm-5.5.4/hagworm/extend/process.py
--rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/qrcode.py
--rw-rw-rw-   0        0        0     7235 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/struct.py
--rw-rw-rw-   0        0        0     3758 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/text.py
--rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/trace.py
--rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/transaction.py
--rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/validator.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.707965 hagworm-5.5.4/hagworm/frame/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/frame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.715004 hagworm-5.5.4/hagworm/frame/fastapi/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/frame/fastapi/__init__.py
--rw-rw-rw-   0        0        0     8148 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/frame/fastapi/base.py
--rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/frame/fastapi/field.py
--rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/frame/fastapi/model.py
--rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/frame/fastapi/response.py
--rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/frame/gunicorn.py
--rw-rw-rw-   0        0        0     3846 2023-05-11 03:07:54.000000 hagworm-5.5.4/hagworm/frame/stress_tests.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.717995 hagworm-5.5.4/hagworm/static/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/static/__init__.py
--rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/static/cacert.pem
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.718965 hagworm-5.5.4/hagworm/third/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/third/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.721965 hagworm-5.5.4/hagworm/third/consul/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/third/consul/__init__.py
--rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/third/consul/config.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.727965 hagworm-5.5.4/hagworm/third/rabbitmq/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/third/rabbitmq/__init__.py
--rw-rw-rw-   0        0        0     3564 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/third/rabbitmq/consume.py
--rw-rw-rw-   0        0        0     5183 2023-05-20 03:08:12.000000 hagworm-5.5.4/hagworm/third/rabbitmq/publish.py
--rw-rw-rw-   0        0        0     5743 2023-05-20 02:53:42.000000 hagworm-5.5.4/hagworm/third/rabbitmq/rpc.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.647966 hagworm-5.5.4/hagworm.egg-info/
--rw-rw-rw-   0        0        0     7515 2023-05-20 03:16:49.000000 hagworm-5.5.4/hagworm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2195 2023-05-20 03:16:49.000000 hagworm-5.5.4/hagworm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 03:16:49.000000 hagworm-5.5.4/hagworm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      723 2023-05-20 03:16:49.000000 hagworm-5.5.4/hagworm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-20 03:16:49.000000 hagworm-5.5.4/hagworm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 03:16:49.729966 hagworm-5.5.4/setup.cfg
--rw-rw-rw-   0        0        0     2407 2023-05-20 02:38:55.000000 hagworm-5.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.854727 hagworm-5.5.5/
+-rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.5.5/LICENSE
+-rw-rw-rw-   0        0        0     7508 2023-05-22 03:51:14.853728 hagworm-5.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.5.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.749728 hagworm-5.5.5/c_extend/
+-rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.5.5/c_extend/math.c
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.751728 hagworm-5.5.5/example/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.757728 hagworm-5.5.5/example/fastapi_demo/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/example/fastapi_demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.760731 hagworm-5.5.5/example/fastapi_demo/controller/
+-rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.5.5/example/fastapi_demo/controller/__init__.py
+-rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.5.5/example/fastapi_demo/controller/home.py
+-rw-rw-rw-   0        0        0      888 2023-05-11 03:07:54.000000 hagworm-5.5.5/example/fastapi_demo/gunicorn.config.py
+-rw-rw-rw-   0        0        0     1431 2023-05-17 08:11:13.000000 hagworm-5.5.5/example/fastapi_demo/main.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.762730 hagworm-5.5.5/example/fastapi_demo/model/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/example/fastapi_demo/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.763731 hagworm-5.5.5/example/fastapi_demo/service/
+-rw-rw-rw-   0        0        0     3496 2023-05-22 00:30:47.000000 hagworm-5.5.5/example/fastapi_demo/service/__init__.py
+-rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.5.5/example/fastapi_demo/setting.py
+-rw-rw-rw-   0        0        0      800 2023-05-11 03:07:54.000000 hagworm-5.5.5/example/main_test.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.764730 hagworm-5.5.5/hagworm/
+-rw-rw-rw-   0        0        0      495 2023-05-22 03:46:07.000000 hagworm-5.5.5/hagworm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.799728 hagworm-5.5.5/hagworm/extend/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.827728 hagworm-5.5.5/hagworm/extend/asyncio/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/asyncio/__init__.py
+-rw-rw-rw-   0        0        0    16802 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/asyncio/base.py
+-rw-rw-rw-   0        0        0     4988 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/asyncio/buffer.py
+-rw-rw-rw-   0        0        0     2396 2023-05-11 03:07:54.000000 hagworm-5.5.5/hagworm/extend/asyncio/command.py
+-rw-rw-rw-   0        0        0     2432 2023-05-18 10:57:40.000000 hagworm-5.5.5/hagworm/extend/asyncio/etcd.py
+-rw-rw-rw-   0        0        0     3194 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/asyncio/event.py
+-rw-rw-rw-   0        0        0     1370 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/asyncio/file.py
+-rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/asyncio/future.py
+-rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/asyncio/mail.py
+-rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/asyncio/mongo.py
+-rw-rw-rw-   0        0        0    15022 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/asyncio/mysql.py
+-rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/asyncio/net.py
+-rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/asyncio/ntp.py
+-rw-rw-rw-   0        0        0     1570 2023-05-20 02:55:55.000000 hagworm-5.5.5/hagworm/extend/asyncio/pool.py
+-rw-rw-rw-   0        0        0    12507 2023-05-22 03:45:54.000000 hagworm-5.5.5/hagworm/extend/asyncio/redis.py
+-rw-rw-rw-   0        0        0     7279 2023-05-11 03:07:54.000000 hagworm-5.5.5/hagworm/extend/asyncio/socket.py
+-rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.5.5/hagworm/extend/asyncio/task.py
+-rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/asyncio/transaction.py
+-rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/asyncio/zmq.py
+-rw-rw-rw-   0        0        0    22623 2023-05-11 03:07:54.000000 hagworm-5.5.5/hagworm/extend/base.py
+-rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/cache.py
+-rw-rw-rw-   0        0        0     1839 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/compile.py
+-rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/config.py
+-rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/crypto.py
+-rw-rw-rw-   0        0        0     1792 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/error.py
+-rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/event.py
+-rw-rw-rw-   0        0        0     4558 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/igraph.py
+-rw-rw-rw-   0        0        0     2326 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/interface.py
+-rw-rw-rw-   0        0        0    14870 2023-05-13 05:06:56.000000 hagworm-5.5.5/hagworm/extend/logging.py
+-rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/media.py
+-rw-rw-rw-   0        0        0     1603 2023-05-10 07:58:09.000000 hagworm-5.5.5/hagworm/extend/metaclass.py
+-rw-rw-rw-   0        0        0     4500 2023-05-11 03:07:54.000000 hagworm-5.5.5/hagworm/extend/process.py
+-rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/qrcode.py
+-rw-rw-rw-   0        0        0     7235 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/struct.py
+-rw-rw-rw-   0        0        0     3758 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/text.py
+-rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/trace.py
+-rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/transaction.py
+-rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/validator.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.832728 hagworm-5.5.5/hagworm/frame/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/frame/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.839729 hagworm-5.5.5/hagworm/frame/fastapi/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/frame/fastapi/__init__.py
+-rw-rw-rw-   0        0        0     8148 2023-05-22 01:25:41.000000 hagworm-5.5.5/hagworm/frame/fastapi/base.py
+-rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/frame/fastapi/field.py
+-rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/frame/fastapi/model.py
+-rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/frame/fastapi/response.py
+-rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/frame/gunicorn.py
+-rw-rw-rw-   0        0        0     3846 2023-05-11 03:07:54.000000 hagworm-5.5.5/hagworm/frame/stress_tests.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.842729 hagworm-5.5.5/hagworm/static/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/static/__init__.py
+-rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/static/cacert.pem
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.843728 hagworm-5.5.5/hagworm/third/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/third/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.846728 hagworm-5.5.5/hagworm/third/consul/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/third/consul/__init__.py
+-rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/third/consul/config.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.852729 hagworm-5.5.5/hagworm/third/rabbitmq/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/third/rabbitmq/__init__.py
+-rw-rw-rw-   0        0        0     3564 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/third/rabbitmq/consume.py
+-rw-rw-rw-   0        0        0     5183 2023-05-20 03:08:12.000000 hagworm-5.5.5/hagworm/third/rabbitmq/publish.py
+-rw-rw-rw-   0        0        0     5743 2023-05-20 02:53:42.000000 hagworm-5.5.5/hagworm/third/rabbitmq/rpc.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.771730 hagworm-5.5.5/hagworm.egg-info/
+-rw-rw-rw-   0        0        0     7508 2023-05-22 03:51:14.000000 hagworm-5.5.5/hagworm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2195 2023-05-22 03:51:14.000000 hagworm-5.5.5/hagworm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 03:51:14.000000 hagworm-5.5.5/hagworm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      724 2023-05-22 03:51:14.000000 hagworm-5.5.5/hagworm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-22 03:51:14.000000 hagworm-5.5.5/hagworm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 03:51:14.854727 hagworm-5.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     2401 2023-05-22 03:46:54.000000 hagworm-5.5.5/setup.py
```

### Comparing `hagworm-5.5.4/LICENSE` & `hagworm-5.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/PKG-INFO` & `hagworm-5.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.5.4
+Version: 5.5.5
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
         
@@ -127,9 +127,9 @@
         * 本项目任何版本不保证没有BUG，商业使用请自行承担风险
         * 如果有任何问题，欢迎与我联系，邮箱wsb310@gmail.com，微信号wsb310
         
 Platform: all
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.9, <3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `hagworm-5.5.4/README.md` & `hagworm-5.5.5/README.md`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/c_extend/math.c` & `hagworm-5.5.5/c_extend/math.c`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/example/fastapi_demo/gunicorn.config.py` & `hagworm-5.5.5/example/fastapi_demo/gunicorn.config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/example/fastapi_demo/main.py` & `hagworm-5.5.5/example/fastapi_demo/main.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/example/fastapi_demo/service/__init__.py` & `hagworm-5.5.5/example/fastapi_demo/service/__init__.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/example/fastapi_demo/setting.py` & `hagworm-5.5.5/example/fastapi_demo/setting.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/example/main_test.py` & `hagworm-5.5.5/example/main_test.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/base.py` & `hagworm-5.5.5/hagworm/extend/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/buffer.py` & `hagworm-5.5.5/hagworm/extend/asyncio/buffer.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/command.py` & `hagworm-5.5.5/hagworm/extend/asyncio/command.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/etcd.py` & `hagworm-5.5.5/hagworm/extend/asyncio/etcd.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/event.py` & `hagworm-5.5.5/hagworm/extend/asyncio/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/file.py` & `hagworm-5.5.5/hagworm/extend/asyncio/file.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/future.py` & `hagworm-5.5.5/hagworm/extend/asyncio/future.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/mail.py` & `hagworm-5.5.5/hagworm/extend/asyncio/mail.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/mongo.py` & `hagworm-5.5.5/hagworm/extend/asyncio/mongo.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/mysql.py` & `hagworm-5.5.5/hagworm/extend/asyncio/mysql.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/net.py` & `hagworm-5.5.5/hagworm/extend/asyncio/net.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/ntp.py` & `hagworm-5.5.5/hagworm/extend/asyncio/ntp.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/pool.py` & `hagworm-5.5.5/hagworm/extend/asyncio/pool.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/redis.py` & `hagworm-5.5.5/hagworm/extend/asyncio/redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 __author__ = r'wsb310@gmail.com'
 
-from aredis import lock, StrictRedis, StrictRedisCluster
+from coredis import lock, StrictRedis, StrictRedisCluster
 
 from .base import Utils
 
 from ..error import catch_error, catch_warning
 from ..interface import AsyncContextManager
 from .ntp import AsyncNTPClient
 from .transaction import Transaction
```

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/socket.py` & `hagworm-5.5.5/hagworm/extend/asyncio/socket.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/task.py` & `hagworm-5.5.5/hagworm/extend/asyncio/task.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/transaction.py` & `hagworm-5.5.5/hagworm/extend/asyncio/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/asyncio/zmq.py` & `hagworm-5.5.5/hagworm/extend/asyncio/zmq.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/base.py` & `hagworm-5.5.5/hagworm/extend/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/cache.py` & `hagworm-5.5.5/hagworm/extend/cache.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/compile.py` & `hagworm-5.5.5/hagworm/extend/compile.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/config.py` & `hagworm-5.5.5/hagworm/extend/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/crypto.py` & `hagworm-5.5.5/hagworm/extend/crypto.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/error.py` & `hagworm-5.5.5/hagworm/extend/error.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/event.py` & `hagworm-5.5.5/hagworm/extend/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/igraph.py` & `hagworm-5.5.5/hagworm/extend/igraph.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/interface.py` & `hagworm-5.5.5/hagworm/extend/interface.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/logging.py` & `hagworm-5.5.5/hagworm/extend/logging.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/media.py` & `hagworm-5.5.5/hagworm/extend/media.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/metaclass.py` & `hagworm-5.5.5/hagworm/extend/metaclass.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/process.py` & `hagworm-5.5.5/hagworm/extend/process.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/qrcode.py` & `hagworm-5.5.5/hagworm/extend/qrcode.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/struct.py` & `hagworm-5.5.5/hagworm/extend/struct.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/text.py` & `hagworm-5.5.5/hagworm/extend/text.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/trace.py` & `hagworm-5.5.5/hagworm/extend/trace.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/transaction.py` & `hagworm-5.5.5/hagworm/extend/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/extend/validator.py` & `hagworm-5.5.5/hagworm/extend/validator.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/frame/fastapi/base.py` & `hagworm-5.5.5/hagworm/frame/fastapi/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/frame/fastapi/field.py` & `hagworm-5.5.5/hagworm/frame/fastapi/field.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/frame/fastapi/model.py` & `hagworm-5.5.5/hagworm/frame/fastapi/model.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/frame/fastapi/response.py` & `hagworm-5.5.5/hagworm/frame/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/frame/gunicorn.py` & `hagworm-5.5.5/hagworm/frame/gunicorn.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/frame/stress_tests.py` & `hagworm-5.5.5/hagworm/frame/stress_tests.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/static/cacert.pem` & `hagworm-5.5.5/hagworm/static/cacert.pem`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/third/consul/config.py` & `hagworm-5.5.5/hagworm/third/consul/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/third/rabbitmq/consume.py` & `hagworm-5.5.5/hagworm/third/rabbitmq/consume.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/third/rabbitmq/publish.py` & `hagworm-5.5.5/hagworm/third/rabbitmq/publish.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm/third/rabbitmq/rpc.py` & `hagworm-5.5.5/hagworm/third/rabbitmq/rpc.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm.egg-info/PKG-INFO` & `hagworm-5.5.5/hagworm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.5.4
+Version: 5.5.5
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
         
@@ -127,9 +127,9 @@
         * 本项目任何版本不保证没有BUG，商业使用请自行承担风险
         * 如果有任何问题，欢迎与我联系，邮箱wsb310@gmail.com，微信号wsb310
         
 Platform: all
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.9, <3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `hagworm-5.5.4/hagworm.egg-info/SOURCES.txt` & `hagworm-5.5.5/hagworm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.4/hagworm.egg-info/requires.txt` & `hagworm-5.5.5/hagworm.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 APScheduler==3.10.1
 Pillow==9.5.0
 PyJWT==2.7.0
 PyYAML==6.0
 SQLAlchemy==2.0.14
-aredis==1.1.8
+coredis==2.3.2
 aiohttp==3.8.4
 aiomysql==0.1.1
 aiosmtplib==2.0.1
 aio-pika==9.0.7
 async-etcd3gw==0.8
 cachetools==5.3.0
 confluent-kafka==2.1.1
```

### Comparing `hagworm-5.5.4/setup.py` & `hagworm-5.5.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,22 +22,22 @@
     author_email=r'wsb310@gmail.com',
     description=r'Network Development Suite',
     long_description=long_description,
     long_description_content_type=r'text/markdown',
     url=r'https://gitee.com/wsb310/hagworm',
     packages=setuptools.find_packages(),
     package_data={r'hagworm': [r'static/*.*']},
-    python_requires=r'>=3.9, <3.10',
+    python_requires=r'>=3.9',
     install_requires=[
         r'APScheduler==3.10.1',
         r'Pillow==9.5.0',
         r'PyJWT==2.7.0',
         r'PyYAML==6.0',
         r'SQLAlchemy==2.0.14',
-        r'aredis==1.1.8',
+        r'coredis==2.3.2',
         r'aiohttp==3.8.4',
         r'aiomysql==0.1.1',
         r'aiosmtplib==2.0.1',
         r'aio-pika==9.0.7',
         r'async-etcd3gw==0.8',
         r'cachetools==5.3.0',
         r'confluent-kafka==2.1.1',
```

