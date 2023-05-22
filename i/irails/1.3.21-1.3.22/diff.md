# Comparing `tmp/irails-1.3.21.tar.gz` & `tmp/irails-1.3.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.21.tar", last modified: Sun May 21 14:43:30 2023, max compression
+gzip compressed data, was "irails-1.3.22.tar", last modified: Mon May 22 15:25:11 2023, max compression
```

## Comparing `irails-1.3.21.tar` & `irails-1.3.22.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.252108 irails-1.3.21/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.21/MANIFEST.in
--rw-rw-rw-   0        0        0     6224 2023-05-21 14:43:30.251109 irails-1.3.21/PKG-INFO
--rw-rw-rw-   0        0        0     5440 2023-05-21 08:50:53.000000 irails-1.3.21/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.159736 irails-1.3.21/irails/
--rw-rw-rw-   0        0        0      307 2023-05-21 14:43:14.000000 irails-1.3.21/irails/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.21/irails/_i18n.py
--rw-rw-rw-   0        0        0     2878 2023-05-21 08:27:23.000000 irails-1.3.21/irails/_loader.py
--rw-rw-rw-   0        0        0     5253 2023-05-20 14:13:50.000000 irails-1.3.21/irails/_utils.py
--rw-rw-rw-   0        0        0    12042 2023-05-20 06:44:17.000000 irails-1.3.21/irails/auth.py
--rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.21/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.168036 irails-1.3.21/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.169034 irails-1.3.21/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.21/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.21/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.21/irails/cbv.py
--rw-rw-rw-   0        0        0     6174 2023-05-19 07:06:13.000000 irails-1.3.21/irails/config.py
--rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.21/irails/controller_utils.py
--rw-rw-rw-   0        0        0    24918 2023-05-19 11:59:51.000000 irails-1.3.21/irails/core.py
--rw-rw-rw-   0        0        0    14606 2023-05-21 14:41:11.000000 irails-1.3.21/irails/database.py
--rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.21/irails/log.py
--rw-rw-rw-   0        0        0     8736 2023-05-21 14:38:31.000000 irails-1.3.21/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.21/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.21/irails/midware_session.py
--rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.21/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.185989 irails-1.3.21/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.21/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.21/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.21/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.21/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.21/irails/scripts/_migrate.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.21/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.21/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.21/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.21/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.21/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.21/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.125070 irails-1.3.21/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.199379 irails-1.3.21/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.21/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.21/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.21/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.21/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.21/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0     1300 2023-05-20 14:09:55.000000 irails-1.3.21/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.21/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      893 2023-05-14 14:08:50.000000 irails-1.3.21/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.21/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.201375 irails-1.3.21/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.21/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.203383 irails-1.3.21/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.21/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.215096 irails-1.3.21/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.21/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.21/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.21/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin-model.conf
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.229169 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/
--rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
--rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
--rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
--rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
--rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
--rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
--rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
--rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
--rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
--rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.21/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.21/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.21/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.21/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.128058 irails-1.3.21/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.233158 irails-1.3.21/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.21/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.21/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.21/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.21/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.237148 irails-1.3.21/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.21/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.21/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.239142 irails-1.3.21/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.131049 irails-1.3.21/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.244129 irails-1.3.21/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.21/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.247126 irails-1.3.21/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.21/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.21/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.21/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.132049 irails-1.3.21/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.249115 irails-1.3.21/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.21/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     1052 2023-05-21 13:45:32.000000 irails-1.3.21/irails/unit_test.py
--rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.21/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.166038 irails-1.3.21/irails.egg-info/
--rw-rw-rw-   0        0        0     6224 2023-05-21 14:43:29.000000 irails-1.3.21/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3115 2023-05-21 14:43:29.000000 irails-1.3.21/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 14:43:29.000000 irails-1.3.21/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-21 14:43:29.000000 irails-1.3.21/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      360 2023-05-21 14:43:29.000000 irails-1.3.21/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-21 14:43:29.000000 irails-1.3.21/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 14:43:30.253105 irails-1.3.21/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.052415 irails-1.3.22/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.22/MANIFEST.in
+-rw-rw-rw-   0        0        0     4878 2023-05-22 15:25:11.051417 irails-1.3.22/PKG-INFO
+-rw-rw-rw-   0        0        0     4096 2023-05-22 07:06:26.000000 irails-1.3.22/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.957289 irails-1.3.22/irails/
+-rw-rw-rw-   0        0        0      307 2023-05-22 15:24:45.000000 irails-1.3.22/irails/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.22/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2878 2023-05-21 08:27:23.000000 irails-1.3.22/irails/_loader.py
+-rw-rw-rw-   0        0        0     5253 2023-05-20 14:13:50.000000 irails-1.3.22/irails/_utils.py
+-rw-rw-rw-   0        0        0    12042 2023-05-20 06:44:17.000000 irails-1.3.22/irails/auth.py
+-rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.22/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.966666 irails-1.3.22/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.967664 irails-1.3.22/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.22/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.22/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.22/irails/cbv.py
+-rw-rw-rw-   0        0        0     6174 2023-05-19 07:06:13.000000 irails-1.3.22/irails/config.py
+-rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.22/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    24918 2023-05-19 11:59:51.000000 irails-1.3.22/irails/core.py
+-rw-rw-rw-   0        0        0    15980 2023-05-22 15:23:58.000000 irails-1.3.22/irails/database.py
+-rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.22/irails/log.py
+-rw-rw-rw-   0        0        0     8736 2023-05-21 14:38:31.000000 irails-1.3.22/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.22/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.22/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.22/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.980629 irails-1.3.22/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.22/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.22/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.22/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.22/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.22/irails/scripts/_migrate.py
+-rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.22/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.22/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.22/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.22/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.22/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.22/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.923380 irails-1.3.22/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.994143 irails-1.3.22/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.22/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.22/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.22/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.22/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.22/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0     1300 2023-05-20 14:09:55.000000 irails-1.3.22/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.22/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      893 2023-05-14 14:08:50.000000 irails-1.3.22/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.22/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.996140 irails-1.3.22/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.22/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.997137 irails-1.3.22/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.22/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.010010 irails-1.3.22/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.22/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.22/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.22/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.022980 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.22/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.22/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.22/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.22/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.928367 irails-1.3.22/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.026985 irails-1.3.22/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.22/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.22/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.22/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.22/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.029789 irails-1.3.22/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.22/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.22/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.032161 irails-1.3.22/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.931360 irails-1.3.22/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.039423 irails-1.3.22/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.22/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.044357 irails-1.3.22/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.22/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.22/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.22/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.932356 irails-1.3.22/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.046940 irails-1.3.22/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.22/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     1052 2023-05-21 13:45:32.000000 irails-1.3.22/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.22/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.964669 irails-1.3.22/irails.egg-info/
+-rw-rw-rw-   0        0        0     4878 2023-05-22 15:25:10.000000 irails-1.3.22/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3115 2023-05-22 15:25:10.000000 irails-1.3.22/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 15:25:10.000000 irails-1.3.22/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-22 15:25:10.000000 irails-1.3.22/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      360 2023-05-22 15:25:10.000000 irails-1.3.22/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-22 15:25:10.000000 irails-1.3.22/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 15:25:11.052415 irails-1.3.22/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.22/setup.py
```

### Comparing `irails-1.3.21/PKG-INFO` & `irails-1.3.22/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.21
+Version: 1.3.22
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 
 # irails
 A mvc framework used FastApi
 Simple and elegant use of FastApi in MVC mode
 
 [Online Docs](https://irails.2rails.cn/) 
-# Welcome to IRAILS(python on rails)
+# Welcome to IRAILS
 IRAILS is not just an ordinary imitation of Ruby on rails, but based on the characteristics of the Python language itself, combined with rich Python class libraries, it refuses to create wheels repeatedly, and can achieve web development with minimal code and configuration, making Python web development fast and powerful, and can be easily deployed on various platforms.
 The design concept of IRails refers to some RORs, but it has its own soul. It does not pursue the ultimate configuration and development, but rather appropriate configuration and development. Currently, it is in a preview version and will continue to improve in the future.
  
 
 ## Installation  
 
 * `pip install irails` - install irails
@@ -82,64 +82,7 @@
     +---uploads                             ## Others dir(if your need or not)
 ```
 ## Extras commands
 * `irails i18n gettext`  --generate i18n in irails app dir
 * `irails shell`         --run python interpreter with buildin support contexts 
 * `irails test`          --run project tests 
 * `irails migrate`       --run database migrations
-
-## Take a look configure file `general.yaml`
- 
-``` 
-    app:
-        appdir:
-        - apps
-        enabled: null
-    root: apps.root
-
-    cors:
-        allow_credentials: true
-        allow_headers:
-            - '*'
-        allow_methods:
-            - '*'
-        allow_origins:
-            - '*'
-    debug: true
-    errors:
-        error_404_page: '{ROOT.public_dir}/error_404.html'
-        error_500_page: '{ROOT.public_dir}/error_500.html'
-    log:
-        file: ''
-        level: DEBUG
-        name: iRails
-    public_dir: ./public
-
-    view:
-        jinja2:
-            block_end_string: '%}'
-            block_start_string: '{%'
-            comment_end_string: '#}'
-            comment_start_string: '{#'
-            variable_end_string: '}'
-            variable_start_string: ${
-        static_format:
-        - vue
-        - html
-    i18n:
-        lang: ['zh']
-        url_lang_key: 'lang'
-```
-## Take a look controller file 
- 
-```python
-    from irails import api_router,api,Request,Response,BaseController,application
- 
-    @api_router(path='/{controller}',auth='none')
-    class AdminController(BaseController): 
-        @api.get("/index")
-        def index(self):
-            """
-            :title Admin
-            """
-            return self.view()
-```
```

### Comparing `irails-1.3.21/README.md` & `irails-1.3.22/irails.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,33 @@
+Metadata-Version: 2.1
+Name: irails
+Version: 1.3.22
+Summary: Simple and elegant use of FastApi in MVC mode
+Home-page: https://github.com/smjkzsl/irails
+Author: Bruce chou
+Author-email: smjkzsl@gmail.com
+License: Apache License 2.0
+Keywords: web framework,mvc framework,fastapi framework
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # irails
 A mvc framework used FastApi
 Simple and elegant use of FastApi in MVC mode
 
 [Online Docs](https://irails.2rails.cn/) 
-# Welcome to IRAILS(python on rails)
+# Welcome to IRAILS
 IRAILS is not just an ordinary imitation of Ruby on rails, but based on the characteristics of the Python language itself, combined with rich Python class libraries, it refuses to create wheels repeatedly, and can achieve web development with minimal code and configuration, making Python web development fast and powerful, and can be easily deployed on various platforms.
 The design concept of IRails refers to some RORs, but it has its own soul. It does not pursue the ultimate configuration and development, but rather appropriate configuration and development. Currently, it is in a preview version and will continue to improve in the future.
  
 
 ## Installation  
 
 * `pip install irails` - install irails
@@ -62,64 +82,7 @@
     +---uploads                             ## Others dir(if your need or not)
 ```
 ## Extras commands
 * `irails i18n gettext`  --generate i18n in irails app dir
 * `irails shell`         --run python interpreter with buildin support contexts 
 * `irails test`          --run project tests 
 * `irails migrate`       --run database migrations
-
-## Take a look configure file `general.yaml`
- 
-``` 
-    app:
-        appdir:
-        - apps
-        enabled: null
-    root: apps.root
-
-    cors:
-        allow_credentials: true
-        allow_headers:
-            - '*'
-        allow_methods:
-            - '*'
-        allow_origins:
-            - '*'
-    debug: true
-    errors:
-        error_404_page: '{ROOT.public_dir}/error_404.html'
-        error_500_page: '{ROOT.public_dir}/error_500.html'
-    log:
-        file: ''
-        level: DEBUG
-        name: iRails
-    public_dir: ./public
-
-    view:
-        jinja2:
-            block_end_string: '%}'
-            block_start_string: '{%'
-            comment_end_string: '#}'
-            comment_start_string: '{#'
-            variable_end_string: '}'
-            variable_start_string: ${
-        static_format:
-        - vue
-        - html
-    i18n:
-        lang: ['zh']
-        url_lang_key: 'lang'
-```
-## Take a look controller file 
- 
-```python
-    from irails import api_router,api,Request,Response,BaseController,application
- 
-    @api_router(path='/{controller}',auth='none')
-    class AdminController(BaseController): 
-        @api.get("/index")
-        def index(self):
-            """
-            :title Admin
-            """
-            return self.view()
-```
```

### Comparing `irails-1.3.21/irails/_i18n.py` & `irails-1.3.22/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/_loader.py` & `irails-1.3.22/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/_utils.py` & `irails-1.3.22/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/auth.py` & `irails-1.3.22/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/base_controller.py` & `irails-1.3.22/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.22/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.22/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/cbv.py` & `irails-1.3.22/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/config.py` & `irails-1.3.22/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/controller_utils.py` & `irails-1.3.22/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/core.py` & `irails-1.3.22/irails/core.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/database.py` & `irails-1.3.22/irails/database.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import configparser
 import re,os,sys
-from typing import Any, Dict, List, Type, Union
+from typing import Any, Dict, List, Type, Union, overload
 from contextlib import contextmanager
 from sqlalchemy import (DateTime, Integer, 
                         String, Text, 
                         create_engine,
                         Engine,
                         MetaData, 
                         Table, 
                         Column, 
                         ForeignKey, 
                         func,
                         select,join,
                         TableClause,
-                        update,
+                        update,insert,delete,
                         event,text,TextClause,Table)
 from sqlalchemy.orm import DeclarativeBase,Session,sessionmaker,relationship,Query 
 from sqlalchemy.ext.automap import automap_base 
-from ._utils import camelize_classname,pluralize_collection 
+from sqlalchemy.sql._typing import _ColumnsClauseArgument
 from alembic import command
 from alembic.config import Config 
+from ._utils import camelize_classname,pluralize_collection 
 from .log import _log
 from ._i18n import _,set_module_i18n
 from .config import config,ROOT_PATH
 from ._utils import get_plural_name,get_singularize_name
  
-events={
+EVENTS={
 'before_insert', 
 'after_insert', 
 'before_update', 
 'after_update',
 'before_delete',
 'after_delete', 
 'before_attach',
@@ -55,17 +56,29 @@
     table_prefix = cfg.get("table_prefix","")
 
  
 class Base( DeclarativeBase ):
     __abstract__ = True
     update_at = Column(DateTime(timezone=True), server_default=func.now(), onupdate=func.now())
     create_at = Column(DateTime(timezone=True), server_default=func.now())
+    #i18n_json_data={
+    #       'col1':{
+    #           'en':'bruce',
+    #           'zh':'布鲁斯'
+    #       },
+    #       'col2':{
+    #           'en':'hellow',
+    #           'zh':'你好'
+    #       },
+    #       ....
+    # 
+    # }
     i18n_json_data = Column(Text,server_default='{}',info={'json':True})
     def __init_subclass__(cls,*args,**kwargs) -> None: 
-        for e in events:
+        for e in EVENTS:
             if hasattr(cls,e):
                 event.listen(cls, e, getattr(cls,e)) 
         set_module_i18n(cls,cls.__module__)
         super().__init_subclass__(*args,**kwargs)
 class Relations():
     __all = {}
     @classmethod
@@ -120,96 +133,137 @@
 
  
 class _serviceMeta(type):
     def __new__(cls, name, bases, attrs):
         obj = super().__new__(cls, name, bases, attrs)
         if obj.__name__!="Service":
             set_module_i18n(obj=obj,module_name=attrs['__module__'])
+         
         return obj
 
 class Service(metaclass=_serviceMeta):
     __all_generated = {}
-    engine:Engine = engine
+     
     _ = _ #the i18n traslation object ,it's will auto redirect the `app_name/locales` dir i18n configure
     
     @classmethod
     def session(self)->Session:
         if hasattr(self,"_session"):
             return self._session
         if hasattr(self,'_session_local'):
             session_local = getattr(self,'_session_local')
         else:
             session_local =  sessionmaker(bind=engine)
             setattr(self,"_session_local", session_local) #cache sessionmaker object
         session = session_local()
         setattr(self,"_session",session)
         return session
- 
+     
+    # @classmethod
+    # def query(self, *entities: _ColumnsClauseArgument[Any], **kwargs: Any)->Query:
+    #     """get query object"""
+    #     session = self.session()   
+    #     return  session.query(*entities,**kwargs)  
+     
+    @classmethod
+    def query(self,model:Base,*args,**kwargs)->Query:
+        session = self.session()
+        query = session.query(model).filter(*args).filter_by(**kwargs)
+        return query
+    @classmethod
+    def insert(self,model:Base,**values)->int:
+        '''
+            execute insert :model with :values 
+            :return rowcount
+        '''
+        stmt = insert(model).values(**values)
+        with engine.begin() as conn:
+            ret = conn.execute(stmt)
+            conn.commit()
+            return ret.rowcount
+    @classmethod
+    def update(self,model:Base,*where,**values)->int:
+        '''
+            execute update :model with :values on :model by :where
+            :return rowcount
+        '''
+        stmt = update(model).where(*where).values(**values)
+        with  engine.begin() as conn:
+            return conn.execute(stmt).rowcount
+    @classmethod
+    def select(self,model:Base,*where)->List[Base]:
+        '''
+            execute select statement with :where condition on :model
+            :return rows of result
+        '''
+        stmt = select(model).where(*where)
+        with engine.begin() as conn:
+            ret = conn.execute(stmt)
+            return ret.fetchall()     
+    
+    @classmethod
+    def count(self,model:Base,*args)->int:
+        '''
+            :return count by givened :args on :model
+        '''
+        if hasattr(model,'id'):
+            return self.session().query(func.count(model.id)).filter(*args).scalar()
+        else:
+            return len(self.list( model,*args))
     @classmethod
     def get(self,model:Base,id:int)->Base:
         return self.session().get(model,id)
     @classmethod
     def add(self,model:Union[Type,Base],**kwargs)->Base:
         if isinstance(model,Base):
             m=model
         else:
             if  kwargs  :
                 m=model(**kwargs)
         if m:
             session = self.session()
             session.add(m)
             session.commit()
-            session.merge(m)
+            session.merge(m,load=False)
             return m
         return None
     @classmethod
-    def list(self,model:Base,**kwargs)->List[Base]:
+    def list(self,model:Base,*args, **kwargs)->List[Base]:
         session = self.session()  
         query = session.query(model) 
+        if args:
+            query = query.filter(*args)
         if kwargs:
             query = query.filter_by(**kwargs) 
         return query.all()
-    @classmethod
-    def query(self,model:Base)->Query:
-        session = self.session()  
-        query = session.query(model) 
-         
-        return query
+    
     
     @classmethod
-    def delete(self,model:Base,**kwargs)->int:
-        session = self.session()  
-        if kwargs:
-            cnt = session.query(model).filter_by(**kwargs).delete()
-        else:
-            cnt = session.query(model).delete()
-        session.commit()
-        return cnt
-    @classmethod
-    def update(self,model:Base,filters:Dict=None, values:Dict=None)->Base:
-        cnt = 0
-        if values:
-            session = self.session() 
-            cnt = session.query(model).filter_by(**filters).update(values)
-            session.commit() 
+    def delete(self,model:Base,*args,**kwargs)->int:
+        query = self.query(model,*args,**kwargs)
+         
+        cnt = query.delete()
+        
+        self.session().commit()
         return cnt
+    
     @classmethod
     def flush(self,model:Base=None):
         session = self.session()
         if not model:
             return session.commit()
         if not model in session:
             session.merge(model)
         session.commit()
          
     @classmethod
     @contextmanager 
     def get_session(cls):
         """Provide a transactional scope around a series of operations."""
-        if not cls.engine:
+        if not  engine:
             yield None
             return
         if hasattr(cls,'_session_local'):
             session_local = getattr(cls,'_session_local')
         else:
             session_local =  sessionmaker(bind=engine)
             setattr(cls,"_session_local", session_local) #cache sessionmaker object
@@ -263,24 +317,15 @@
             tbItem = tblClass()
             setattr(tbItem,"_tableItem",tbl) 
             cls.__all_generated[table_name] = tbItem
             return tbItem
         else:
             raise NameError()
 
-
-            
-# def ismongo_cloud(uri):
-#     import re 
-#     # uri = 'mongodb+srv://dbbruce:smjk123@atlascluster.siz4vrp.mongodb.net/?retryWrites=true&w=majority' 
-#     # 匹配 MongoDB Cloud 连接字符串的正则表达式
-#     regex = re.compile("mongodb\+srv:\/\/.*@.*\.mongodb\.net\/.*\?.*") 
-#     return regex.match(uri)
-      
-
+ 
 def sanitize_path(path):
     # 匹配非法字符
     illegal_chars = r'[\\/:\*\?"<>\|]'
     # 将非法字符替换为下划线
     sanitized_path = re.sub(illegal_chars, '_', path)
     return sanitized_path
```

### Comparing `irails-1.3.21/irails/log.py` & `irails-1.3.22/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/midware.py` & `irails-1.3.22/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/midware_casbin.py` & `irails-1.3.22/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/midware_session.py` & `irails-1.3.22/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/mvc_router.py` & `irails-1.3.22/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/_app.py` & `irails-1.3.22/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/_controller.py` & `irails-1.3.22/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/_i18n.py` & `irails-1.3.22/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/_migrate.py` & `irails-1.3.22/irails/scripts/_migrate.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/_model.py` & `irails-1.3.22/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/_project.py` & `irails-1.3.22/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/_run.py` & `irails-1.3.22/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/_shell.py` & `irails-1.3.22/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/_test.py` & `irails-1.3.22/irails/scripts/_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/main.py` & `irails-1.3.22/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.22/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/tpls/app/home.tpl` & `irails-1.3.22/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/tpls/app/model.jinja` & `irails-1.3.22/irails/scripts/tpls/app/model.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/tpls/app/service.jinja` & `irails-1.3.22/irails/scripts/tpls/app/service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.22/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.22/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.22/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.22/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.22/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.22/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.22/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.22/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.22/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.22/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.22/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.22/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/unit_test.py` & `irails-1.3.22/irails/unit_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails/view.py` & `irails-1.3.22/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/irails.egg-info/SOURCES.txt` & `irails-1.3.22/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.21/setup.py` & `irails-1.3.22/setup.py`

 * *Files identical despite different names*

