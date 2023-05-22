# Comparing `tmp/soil-1.0.0rc5.post1.tar.gz` & `tmp/soil-1.0.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soil-1.0.0rc5.post1.tar", last modified: Thu May  4 11:13:21 2023, max compression
+gzip compressed data, was "soil-1.0.0rc7.tar", last modified: Mon May 22 07:15:47 2023, max compression
```

## Comparing `soil-1.0.0rc5.post1.tar` & `soil-1.0.0rc7.tar`

### file list

```diff
@@ -1,100 +1,104 @@
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.272182 soil-1.0.0rc5.post1/
--rw-r--r--   0 j         (1000) j         (1000)    11412 2018-12-07 19:26:39.000000 soil-1.0.0rc5.post1/LICENSE
--rw-r--r--   0 j         (1000) j         (1000)      163 2020-03-11 15:11:50.000000 soil-1.0.0rc5.post1/MANIFEST.in
--rw-rw-r--   0 j         (1000) j         (1000)     5751 2023-05-04 11:13:21.272182 soil-1.0.0rc5.post1/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)     4655 2023-04-24 16:43:50.000000 soil-1.0.0rc5.post1/README.md
--rw-rw-r--   0 j         (1000) j         (1000)      166 2023-04-24 16:44:33.000000 soil-1.0.0rc5.post1/requirements.txt
--rw-rw-r--   0 j         (1000) j         (1000)      191 2023-05-04 11:13:21.272182 soil-1.0.0rc5.post1/setup.cfg
--rw-rw-r--   0 j         (1000) j         (1000)     2211 2023-04-24 16:05:52.000000 soil-1.0.0rc5.post1/setup.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.264182 soil-1.0.0rc5.post1/soil/
--rw-rw-r--   0 j         (1000) j         (1000)      365 2023-03-23 13:48:55.000000 soil-1.0.0rc5.post1/soil/.VERSION.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-14 19:48:55.000000 soil-1.0.0rc5.post1/soil/.__init__.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    13297 2023-03-23 13:34:51.000000 soil-1.0.0rc5.post1/soil/.analysis.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     3720 2023-04-26 07:50:45.000000 soil-1.0.0rc5.post1/soil/.datacollection.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    37698 2023-04-29 12:20:51.000000 soil-1.0.0rc5.post1/soil/.environment.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    13143 2023-04-25 22:09:53.000000 soil-1.0.0rc5.post1/soil/.events.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     2588 2023-04-14 20:43:29.000000 soil-1.0.0rc5.post1/soil/.exporters.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     1110 2023-04-14 21:29:51.000000 soil-1.0.0rc5.post1/soil/.serialization.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    15937 2023-04-16 19:59:22.000000 soil-1.0.0rc5.post1/soil/.simulation.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     5011 2023-03-23 13:48:01.000000 soil-1.0.0rc5.post1/soil/.stats.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)   185860 2023-04-27 15:33:19.000000 soil-1.0.0rc5.post1/soil/.time.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    32688 2023-04-21 14:21:10.000000 soil-1.0.0rc5.post1/soil/.utils.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-04 13:46:42.000000 soil-1.0.0rc5.post1/soil/.visualization.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)       15 2023-05-04 11:13:12.000000 soil-1.0.0rc5.post1/soil/VERSION
--rw-rw-r--   0 j         (1000) j         (1000)     7899 2023-05-04 09:48:46.000000 soil-1.0.0rc5.post1/soil/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      107 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/__main__.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.268182 soil-1.0.0rc5.post1/soil/agents/
--rw-rw-r--   0 j         (1000) j         (1000)    82293 2023-04-27 07:13:41.000000 soil-1.0.0rc5.post1/soil/agents/.__init__.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    59903 2023-04-25 23:21:25.000000 soil-1.0.0rc5.post1/soil/agents/.evented.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    61000 2023-04-27 07:10:51.000000 soil-1.0.0rc5.post1/soil/agents/.fsm.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     5801 2023-04-25 03:00:06.000000 soil-1.0.0rc5.post1/soil/agents/.network_agents.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)      734 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/agents/BassModel.py
--rw-rw-r--   0 j         (1000) j         (1000)     1171 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/agents/CounterModel.py
--rw-rw-r--   0 j         (1000) j         (1000)      766 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/agents/IndependentCascadeModel.py
--rw-rw-r--   0 j         (1000) j         (1000)     3385 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/agents/SISaModel.py
--rw-rw-r--   0 j         (1000) j         (1000)    20467 2023-05-04 10:45:09.000000 soil-1.0.0rc5.post1/soil/agents/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)     1814 2023-05-02 17:48:59.000000 soil-1.0.0rc5.post1/soil/agents/evented.py
--rw-rw-r--   0 j         (1000) j         (1000)     5408 2023-05-04 11:04:55.000000 soil-1.0.0rc5.post1/soil/agents/fsm.py
--rw-rw-r--   0 j         (1000) j         (1000)      731 2023-04-29 09:53:33.000000 soil-1.0.0rc5.post1/soil/agents/geo.py
--rw-rw-r--   0 j         (1000) j         (1000)     3420 2023-04-25 03:00:06.000000 soil-1.0.0rc5.post1/soil/agents/network_agents.py
--rw-rw-r--   0 j         (1000) j         (1000)     2434 2023-05-02 17:39:42.000000 soil-1.0.0rc5.post1/soil/analysis.py
--rw-rw-r--   0 j         (1000) j         (1000)       36 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/config.py
--rw-rw-r--   0 j         (1000) j         (1000)      853 2023-04-26 07:50:45.000000 soil-1.0.0rc5.post1/soil/datacollection.py
--rw-rw-r--   0 j         (1000) j         (1000)     7217 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/debugging.py
--rw-rw-r--   0 j         (1000) j         (1000)      168 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/decorators.py
--rw-rw-r--   0 j         (1000) j         (1000)    15695 2023-05-04 10:22:08.000000 soil-1.0.0rc5.post1/soil/environment.py
--rw-rw-r--   0 j         (1000) j         (1000)      541 2023-04-25 22:09:53.000000 soil-1.0.0rc5.post1/soil/events.py
--rw-rw-r--   0 j         (1000) j         (1000)     9048 2023-05-02 17:55:40.000000 soil-1.0.0rc5.post1/soil/exporters.py
--rw-rw-r--   0 j         (1000) j         (1000)     2149 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/network.py
--rw-rw-r--   0 j         (1000) j         (1000)      739 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/parameters.py
--rw-rw-r--   0 j         (1000) j         (1000)     8070 2023-04-29 09:32:04.000000 soil-1.0.0rc5.post1/soil/serialization.py
--rw-r--r--   0 j         (1000) j         (1000)       24 2018-12-07 19:26:39.000000 soil-1.0.0rc5.post1/soil/settings.py
--rw-rw-r--   0 j         (1000) j         (1000)    13043 2023-05-02 20:14:49.000000 soil-1.0.0rc5.post1/soil/simulation.py
--rw-rw-r--   0 j         (1000) j         (1000)     5247 2023-05-04 11:12:52.000000 soil-1.0.0rc5.post1/soil/time.py
--rw-rw-r--   0 j         (1000) j         (1000)     4381 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/utils.py
--rw-rw-r--   0 j         (1000) j         (1000)      476 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/version.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.268182 soil-1.0.0rc5.post1/soil/web/
--rw-r--r--   0 j         (1000) j         (1000)       41 2018-12-08 17:08:24.000000 soil-1.0.0rc5.post1/soil/web/.gitignore
--rw-r--r--   0 j         (1000) j         (1000)     2984 2018-12-08 17:08:24.000000 soil-1.0.0rc5.post1/soil/web/README.md
--rw-rw-r--   0 j         (1000) j         (1000)    11272 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/web/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)       59 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/web/__main__.py
--rw-rw-r--   0 j         (1000) j         (1000)      575 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/web/config.yml
--rw-rw-r--   0 j         (1000) j         (1000)     1073 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/web/run.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.260182 soil-1.0.0rc5.post1/soil/web/static/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.268182 soil-1.0.0rc5.post1/soil/web/static/css/
--rw-r--r--   0 j         (1000) j         (1000)     7157 2018-12-08 17:08:24.000000 soil-1.0.0rc5.post1/soil/web/static/css/main.css
--rw-r--r--   0 j         (1000) j         (1000)     1107 2018-12-08 17:08:24.000000 soil-1.0.0rc5.post1/soil/web/static/css/timeline.css
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.268182 soil-1.0.0rc5.post1/soil/web/static/img/
--rw-r--r--   0 j         (1000) j         (1000)    18053 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/img/logo_gsi.svg
--rw-r--r--   0 j         (1000) j         (1000)   103744 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/img/logo_soil.png
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.268182 soil-1.0.0rc5.post1/soil/web/static/img/svg/
--rw-r--r--   0 j         (1000) j         (1000)      462 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/img/svg/home.svg
--rw-r--r--   0 j         (1000) j         (1000)      812 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/img/svg/person.svg
--rw-r--r--   0 j         (1000) j         (1000)      697 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/img/svg/plus.svg
--rw-r--r--   0 j         (1000) j         (1000)      992 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/img/svg/target.svg
--rw-r--r--   0 j         (1000) j         (1000)     1561 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/img/svg/time.svg
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.268182 soil-1.0.0rc5.post1/soil/web/static/js/
--rwxr-xr-x   0 j         (1000) j         (1000)    16528 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/js/socket.js
--rw-r--r--   0 j         (1000) j         (1000)     5040 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/js/template.js
--rw-r--r--   0 j         (1000) j         (1000)    12269 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/js/timeline.js
--rw-r--r--   0 j         (1000) j         (1000)    21818 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/js/visualization.js
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.268182 soil-1.0.0rc5.post1/soil/web/templates/
--rw-r--r--   0 j         (1000) j         (1000)    16450 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/templates/index.html
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.264182 soil-1.0.0rc5.post1/soil.egg-info/
--rw-r--r--   0 j         (1000) j         (1000)     5751 2023-05-04 11:13:21.000000 soil-1.0.0rc5.post1/soil.egg-info/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)     2123 2023-05-04 11:13:21.000000 soil-1.0.0rc5.post1/soil.egg-info/SOURCES.txt
--rw-r--r--   0 j         (1000) j         (1000)        1 2023-05-04 11:13:21.000000 soil-1.0.0rc5.post1/soil.egg-info/dependency_links.txt
--rw-r--r--   0 j         (1000) j         (1000)       78 2023-05-04 11:13:21.000000 soil-1.0.0rc5.post1/soil.egg-info/entry_points.txt
--rw-r--r--   0 j         (1000) j         (1000)      292 2023-05-04 11:13:21.000000 soil-1.0.0rc5.post1/soil.egg-info/requires.txt
--rw-r--r--   0 j         (1000) j         (1000)        5 2023-05-04 11:13:21.000000 soil-1.0.0rc5.post1/soil.egg-info/top_level.txt
--rw-rw-r--   0 j         (1000) j         (1000)       90 2023-04-24 17:04:44.000000 soil-1.0.0rc5.post1/test-requirements.txt
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.272182 soil-1.0.0rc5.post1/tests/
--rw-rw-r--   0 j         (1000) j         (1000)    11851 2023-05-02 19:21:49.000000 soil-1.0.0rc5.post1/tests/test_agents.py
--rw-rw-r--   0 j         (1000) j         (1000)     2231 2023-04-25 13:22:59.000000 soil-1.0.0rc5.post1/tests/test_config.py
--rw-rw-r--   0 j         (1000) j         (1000)     2450 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/tests/test_examples.py
--rw-rw-r--   0 j         (1000) j         (1000)     3761 2023-04-27 16:08:44.000000 soil-1.0.0rc5.post1/tests/test_exporters.py
--rw-rw-r--   0 j         (1000) j         (1000)      636 2023-04-24 16:55:59.000000 soil-1.0.0rc5.post1/tests/test_ipython.py
--rw-rw-r--   0 j         (1000) j         (1000)     8511 2023-05-04 11:04:12.000000 soil-1.0.0rc5.post1/tests/test_main.py
--rw-rw-r--   0 j         (1000) j         (1000)     1940 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/tests/test_mesa.py
--rw-rw-r--   0 j         (1000) j         (1000)     3133 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/tests/test_network.py
--rw-rw-r--   0 j         (1000) j         (1000)     1549 2023-05-02 15:39:46.000000 soil-1.0.0rc5.post1/tests/test_time.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 07:15:47.031227 soil-1.0.0rc7/
+-rw-r--r--   0 j         (1000) j         (1000)    11412 2018-12-07 19:26:39.000000 soil-1.0.0rc7/LICENSE
+-rw-r--r--   0 j         (1000) j         (1000)      163 2020-03-11 15:11:50.000000 soil-1.0.0rc7/MANIFEST.in
+-rw-rw-r--   0 j         (1000) j         (1000)     5739 2023-05-22 07:15:47.031227 soil-1.0.0rc7/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)     4655 2023-04-24 16:43:50.000000 soil-1.0.0rc7/README.md
+-rw-rw-r--   0 j         (1000) j         (1000)      152 2023-05-16 09:54:11.000000 soil-1.0.0rc7/requirements.txt
+-rw-rw-r--   0 j         (1000) j         (1000)      191 2023-05-22 07:15:47.031227 soil-1.0.0rc7/setup.cfg
+-rw-rw-r--   0 j         (1000) j         (1000)     2211 2023-04-24 16:05:52.000000 soil-1.0.0rc7/setup.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 07:15:47.023227 soil-1.0.0rc7/soil/
+-rw-rw-r--   0 j         (1000) j         (1000)      261 2023-05-22 07:15:09.000000 soil-1.0.0rc7/soil/.VERSION.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-14 19:48:55.000000 soil-1.0.0rc7/soil/.__init__.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    13297 2023-03-23 13:34:51.000000 soil-1.0.0rc7/soil/.analysis.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     3720 2023-04-26 07:50:45.000000 soil-1.0.0rc7/soil/.datacollection.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)   102403 2023-05-18 08:01:44.000000 soil-1.0.0rc7/soil/.decorators.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     2450 2023-05-17 21:10:06.000000 soil-1.0.0rc7/soil/.environment.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    13143 2023-04-25 22:09:53.000000 soil-1.0.0rc7/soil/.events.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     2588 2023-04-14 20:43:29.000000 soil-1.0.0rc7/soil/.exporters.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     1110 2023-04-14 21:29:51.000000 soil-1.0.0rc7/soil/.serialization.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    15937 2023-04-16 19:59:22.000000 soil-1.0.0rc7/soil/.simulation.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     5011 2023-03-23 13:48:01.000000 soil-1.0.0rc7/soil/.stats.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    11233 2023-05-18 11:05:12.000000 soil-1.0.0rc7/soil/.time.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    32688 2023-04-21 14:21:10.000000 soil-1.0.0rc7/soil/.utils.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-04 13:46:42.000000 soil-1.0.0rc7/soil/.visualization.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)        9 2023-05-22 07:15:09.000000 soil-1.0.0rc7/soil/VERSION
+-rw-rw-r--   0 j         (1000) j         (1000)     7865 2023-05-18 15:20:16.000000 soil-1.0.0rc7/soil/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      107 2023-04-21 12:27:50.000000 soil-1.0.0rc7/soil/__main__.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 07:15:47.027227 soil-1.0.0rc7/soil/agents/
+-rw-rw-r--   0 j         (1000) j         (1000)     2391 2023-05-17 21:17:56.000000 soil-1.0.0rc7/soil/agents/.__init__.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    59903 2023-04-25 23:21:25.000000 soil-1.0.0rc7/soil/agents/.evented.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     6689 2023-05-18 07:39:51.000000 soil-1.0.0rc7/soil/agents/.fsm.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    21543 2023-05-18 10:56:12.000000 soil-1.0.0rc7/soil/agents/.meta.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     5801 2023-04-25 03:00:06.000000 soil-1.0.0rc7/soil/agents/.network_agents.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      734 2023-04-21 12:27:50.000000 soil-1.0.0rc7/soil/agents/BassModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1171 2023-04-21 12:27:50.000000 soil-1.0.0rc7/soil/agents/CounterModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)      766 2023-04-21 12:27:50.000000 soil-1.0.0rc7/soil/agents/IndependentCascadeModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3385 2023-04-21 12:27:50.000000 soil-1.0.0rc7/soil/agents/SISaModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)     6319 2023-05-18 13:23:17.000000 soil-1.0.0rc7/soil/agents/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1051 2023-05-19 08:38:34.000000 soil-1.0.0rc7/soil/agents/evented.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5815 2023-05-19 08:36:48.000000 soil-1.0.0rc7/soil/agents/fsm.py
+-rw-rw-r--   0 j         (1000) j         (1000)      731 2023-04-29 09:53:33.000000 soil-1.0.0rc7/soil/agents/geo.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2121 2023-05-18 12:44:14.000000 soil-1.0.0rc7/soil/agents/meta.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3585 2023-05-10 16:19:55.000000 soil-1.0.0rc7/soil/agents/network_agents.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3751 2023-05-18 12:38:35.000000 soil-1.0.0rc7/soil/agents/view.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2205 2023-05-18 10:58:30.000000 soil-1.0.0rc7/soil/analysis.py
+-rw-rw-r--   0 j         (1000) j         (1000)       36 2023-04-21 12:27:50.000000 soil-1.0.0rc7/soil/config.py
+-rw-rw-r--   0 j         (1000) j         (1000)      853 2023-04-26 07:50:45.000000 soil-1.0.0rc7/soil/datacollection.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7217 2023-04-21 12:27:50.000000 soil-1.0.0rc7/soil/debugging.py
+-rw-rw-r--   0 j         (1000) j         (1000)      989 2023-05-18 12:42:23.000000 soil-1.0.0rc7/soil/decorators.py
+-rw-rw-r--   0 j         (1000) j         (1000)    19631 2023-05-19 14:04:51.000000 soil-1.0.0rc7/soil/environment.py
+-rw-rw-r--   0 j         (1000) j         (1000)      626 2023-05-10 15:48:22.000000 soil-1.0.0rc7/soil/events.py
+-rw-rw-r--   0 j         (1000) j         (1000)     9555 2023-05-18 14:06:19.000000 soil-1.0.0rc7/soil/exporters.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2149 2023-04-21 12:27:50.000000 soil-1.0.0rc7/soil/network.py
+-rw-rw-r--   0 j         (1000) j         (1000)      739 2023-04-21 12:27:50.000000 soil-1.0.0rc7/soil/parameters.py
+-rw-rw-r--   0 j         (1000) j         (1000)     8070 2023-04-29 09:32:04.000000 soil-1.0.0rc7/soil/serialization.py
+-rw-r--r--   0 j         (1000) j         (1000)       24 2018-12-07 19:26:39.000000 soil-1.0.0rc7/soil/settings.py
+-rw-rw-r--   0 j         (1000) j         (1000)    13135 2023-05-18 15:20:04.000000 soil-1.0.0rc7/soil/simulation.py
+-rw-rw-r--   0 j         (1000) j         (1000)     8089 2023-05-18 16:17:24.000000 soil-1.0.0rc7/soil/time.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4783 2023-05-18 10:58:56.000000 soil-1.0.0rc7/soil/utils.py
+-rw-rw-r--   0 j         (1000) j         (1000)      476 2023-04-21 12:27:50.000000 soil-1.0.0rc7/soil/version.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 07:15:47.027227 soil-1.0.0rc7/soil/web/
+-rw-r--r--   0 j         (1000) j         (1000)       41 2018-12-08 17:08:24.000000 soil-1.0.0rc7/soil/web/.gitignore
+-rw-r--r--   0 j         (1000) j         (1000)     2984 2018-12-08 17:08:24.000000 soil-1.0.0rc7/soil/web/README.md
+-rw-rw-r--   0 j         (1000) j         (1000)    11272 2023-04-21 12:27:50.000000 soil-1.0.0rc7/soil/web/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)       59 2023-04-21 12:27:50.000000 soil-1.0.0rc7/soil/web/__main__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      575 2023-04-21 12:27:50.000000 soil-1.0.0rc7/soil/web/config.yml
+-rw-rw-r--   0 j         (1000) j         (1000)     1073 2023-04-21 12:27:50.000000 soil-1.0.0rc7/soil/web/run.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 07:15:47.015227 soil-1.0.0rc7/soil/web/static/
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 07:15:47.027227 soil-1.0.0rc7/soil/web/static/css/
+-rw-r--r--   0 j         (1000) j         (1000)     7157 2018-12-08 17:08:24.000000 soil-1.0.0rc7/soil/web/static/css/main.css
+-rw-r--r--   0 j         (1000) j         (1000)     1107 2018-12-08 17:08:24.000000 soil-1.0.0rc7/soil/web/static/css/timeline.css
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 07:15:47.027227 soil-1.0.0rc7/soil/web/static/img/
+-rw-r--r--   0 j         (1000) j         (1000)    18053 2018-12-08 17:08:25.000000 soil-1.0.0rc7/soil/web/static/img/logo_gsi.svg
+-rw-r--r--   0 j         (1000) j         (1000)   103744 2018-12-08 17:08:25.000000 soil-1.0.0rc7/soil/web/static/img/logo_soil.png
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 07:15:47.027227 soil-1.0.0rc7/soil/web/static/img/svg/
+-rw-r--r--   0 j         (1000) j         (1000)      462 2018-12-08 17:08:25.000000 soil-1.0.0rc7/soil/web/static/img/svg/home.svg
+-rw-r--r--   0 j         (1000) j         (1000)      812 2018-12-08 17:08:25.000000 soil-1.0.0rc7/soil/web/static/img/svg/person.svg
+-rw-r--r--   0 j         (1000) j         (1000)      697 2018-12-08 17:08:25.000000 soil-1.0.0rc7/soil/web/static/img/svg/plus.svg
+-rw-r--r--   0 j         (1000) j         (1000)      992 2018-12-08 17:08:25.000000 soil-1.0.0rc7/soil/web/static/img/svg/target.svg
+-rw-r--r--   0 j         (1000) j         (1000)     1561 2018-12-08 17:08:25.000000 soil-1.0.0rc7/soil/web/static/img/svg/time.svg
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 07:15:47.027227 soil-1.0.0rc7/soil/web/static/js/
+-rwxr-xr-x   0 j         (1000) j         (1000)    16528 2018-12-08 17:08:25.000000 soil-1.0.0rc7/soil/web/static/js/socket.js
+-rw-r--r--   0 j         (1000) j         (1000)     5040 2018-12-08 17:08:25.000000 soil-1.0.0rc7/soil/web/static/js/template.js
+-rw-r--r--   0 j         (1000) j         (1000)    12269 2018-12-08 17:08:25.000000 soil-1.0.0rc7/soil/web/static/js/timeline.js
+-rw-r--r--   0 j         (1000) j         (1000)    21818 2018-12-08 17:08:25.000000 soil-1.0.0rc7/soil/web/static/js/visualization.js
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 07:15:47.027227 soil-1.0.0rc7/soil/web/templates/
+-rw-r--r--   0 j         (1000) j         (1000)    16450 2018-12-08 17:08:25.000000 soil-1.0.0rc7/soil/web/templates/index.html
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 07:15:47.023227 soil-1.0.0rc7/soil.egg-info/
+-rw-r--r--   0 j         (1000) j         (1000)     5739 2023-05-22 07:15:47.000000 soil-1.0.0rc7/soil.egg-info/PKG-INFO
+-rw-r--r--   0 j         (1000) j         (1000)     2228 2023-05-22 07:15:47.000000 soil-1.0.0rc7/soil.egg-info/SOURCES.txt
+-rw-r--r--   0 j         (1000) j         (1000)        1 2023-05-22 07:15:47.000000 soil-1.0.0rc7/soil.egg-info/dependency_links.txt
+-rw-r--r--   0 j         (1000) j         (1000)       78 2023-05-22 07:15:47.000000 soil-1.0.0rc7/soil.egg-info/entry_points.txt
+-rw-r--r--   0 j         (1000) j         (1000)      278 2023-05-22 07:15:47.000000 soil-1.0.0rc7/soil.egg-info/requires.txt
+-rw-r--r--   0 j         (1000) j         (1000)        5 2023-05-22 07:15:47.000000 soil-1.0.0rc7/soil.egg-info/top_level.txt
+-rw-rw-r--   0 j         (1000) j         (1000)       90 2023-04-24 17:04:44.000000 soil-1.0.0rc7/test-requirements.txt
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 07:15:47.027227 soil-1.0.0rc7/tests/
+-rw-rw-r--   0 j         (1000) j         (1000)    16405 2023-05-19 14:08:32.000000 soil-1.0.0rc7/tests/test_agents.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2231 2023-04-25 13:22:59.000000 soil-1.0.0rc7/tests/test_config.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2450 2023-04-21 12:27:50.000000 soil-1.0.0rc7/tests/test_examples.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3792 2023-05-04 14:58:41.000000 soil-1.0.0rc7/tests/test_exporters.py
+-rw-rw-r--   0 j         (1000) j         (1000)      636 2023-04-24 16:55:59.000000 soil-1.0.0rc7/tests/test_ipython.py
+-rw-rw-r--   0 j         (1000) j         (1000)     9540 2023-05-18 12:37:14.000000 soil-1.0.0rc7/tests/test_main.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1940 2023-04-21 12:27:50.000000 soil-1.0.0rc7/tests/test_mesa.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3133 2023-04-21 12:27:50.000000 soil-1.0.0rc7/tests/test_network.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1549 2023-05-02 15:39:46.000000 soil-1.0.0rc7/tests/test_time.py
```

### Comparing `soil-1.0.0rc5.post1/LICENSE` & `soil-1.0.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/PKG-INFO` & `soil-1.0.0rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: soil
-Version: 1.0.0rc5.post1
+Version: 1.0.0rc7
 Summary: An Agent-Based Social Simulator for Social Networks
 Home-page: https://github.com/gsi-upm/soil
-Download-URL: https://github.com/gsi-upm/soil/archive/1.0.0rc5.post1.tar.gz
+Download-URL: https://github.com/gsi-upm/soil/archive/1.0.0rc7.tar.gz
 Author: J. Fernando Sanchez
 Author-email: jf.sanchez@upm.es
 Keywords: agent,social,simulator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `soil-1.0.0rc5.post1/README.md` & `soil-1.0.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/setup.py` & `soil-1.0.0rc7/setup.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/.analysis.py.~undo-tree~` & `soil-1.0.0rc7/soil/.analysis.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/.datacollection.py.~undo-tree~` & `soil-1.0.0rc7/soil/.datacollection.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/.events.py.~undo-tree~` & `soil-1.0.0rc7/soil/.events.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/.exporters.py.~undo-tree~` & `soil-1.0.0rc7/soil/.exporters.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/.serialization.py.~undo-tree~` & `soil-1.0.0rc7/soil/.serialization.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/.simulation.py.~undo-tree~` & `soil-1.0.0rc7/soil/.simulation.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/.stats.py.~undo-tree~` & `soil-1.0.0rc7/soil/.stats.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/.utils.py.~undo-tree~` & `soil-1.0.0rc7/soil/.utils.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/__init__.py` & `soil-1.0.0rc7/soil/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 except NameError:
     basestring = str
 
 from pathlib import Path
 from .agents import *
 from . import agents
 from .simulation import *
-from .environment import Environment, EventedEnvironment
+from .environment import Environment
 from .datacollection import SoilCollector
 from . import serialization
 from .utils import logger
 from .time import *
 from .decorators import *
 
 
@@ -113,21 +113,21 @@
         "--exporter",
         action="append",
         default=[],
         help="Export environment and/or simulations using this exporter",
     )
     parser.add_argument(
         "--max_time",
-        default="-1",
+        default="",
         help="Set maximum time for the simulation to run. ",
     )
 
     parser.add_argument(
         "--max_steps",
-        default="-1",
+        default="",
         help="Set maximum number of steps for the simulation to run.",
     )
 
     parser.add_argument(
         "--iterations",
         default="",
         help="Set maximum number of iterations (runs) for the simulation.",
@@ -245,22 +245,24 @@
                         setattr(target, tail, v)
                     except AttributeError:
                         target[tail] = v
 
             if args.only_convert:
                 print(sim.to_yaml())
                 continue
-            max_time = float(args.max_time) if args.max_time != "-1" else None
-            max_steps = float(args.max_steps) if args.max_steps != "-1" else None
-            res.append(sim.run(max_time=max_time, max_steps=max_steps))
+            d = {}
+            if args.max_time:
+                d["max_time"] = float(args.max_time) 
+            if args.max_steps:
+                d["max_steps"] = int(args.max_steps)
+            res.append(sim.run(**d))
 
     except Exception as ex:
         if args.pdb:
             from .debugging import post_mortem
-
             print(traceback.format_exc())
             post_mortem()
         else:
             raise
     if debug:
         from .debugging import set_trace
```

### Comparing `soil-1.0.0rc5.post1/soil/agents/.evented.py.~undo-tree~` & `soil-1.0.0rc7/soil/agents/.evented.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/agents/.network_agents.py.~undo-tree~` & `soil-1.0.0rc7/soil/agents/.network_agents.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/agents/BassModel.py` & `soil-1.0.0rc7/soil/agents/BassModel.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/agents/CounterModel.py` & `soil-1.0.0rc7/soil/agents/CounterModel.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/agents/IndependentCascadeModel.py` & `soil-1.0.0rc7/soil/agents/IndependentCascadeModel.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/agents/SISaModel.py` & `soil-1.0.0rc7/soil/agents/SISaModel.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/agents/__init__.py` & `soil-1.0.0rc7/soil/environment.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,705 +1,542 @@
 from __future__ import annotations
 
-import logging
-from collections import OrderedDict, defaultdict
-from collections.abc import MutableMapping, Mapping, Set
-from abc import ABCMeta
-from copy import deepcopy, copy
-from functools import partial, wraps
-from itertools import islice, chain
-import inspect
-import types
-import textwrap
-import networkx as nx
-import warnings
+import os
 import sys
+import logging
 
-from typing import Any
-
-from mesa import Agent as MesaAgent, Model
-from typing import Dict, List
-
-from .. import serialization, network, utils, time, config
-
+from typing import Any, Callable, Dict, Optional, Union, List, Type
+from types import coroutine
 
-IGNORED_FIELDS = ("model", "logger")
+import networkx as nx
 
 
-def decorate_generator_step(func, name):
-    @wraps(func)
-    def decorated(self):
-        while True:
-            if self._coroutine is None:
-                self._coroutine = func(self)
-            try:
-                if self._last_except:
-                    val = self._coroutine.throw(self._last_except)
-                else:
-                    val = self._coroutine.send(self._last_return)
-            except StopIteration as ex:
-                self._coroutine = None
-                val = ex.value
-            finally:
-                self._last_return = None
-                self._last_except = None
-            return float(val) if val is not None else val
-    return decorated
-
-
-def decorate_normal_func(func, name):
-    @wraps(func)
-    def decorated(self):
-        val = func(self)
-        return float(val) if val is not None else val
-    return decorated
-
-
-class MetaAgent(ABCMeta):
-    def __new__(mcls, name, bases, namespace):
-        defaults = {}
-
-        # Re-use defaults from inherited classes
-        for i in bases:
-            if isinstance(i, MetaAgent):
-                defaults.update(i._defaults)
-
-        new_nmspc = {
-            "_defaults": defaults,
-        }
-
-        for attr, func in namespace.items():
-            if attr == "step":
-                if inspect.isgeneratorfunction(func) or inspect.iscoroutinefunction(func):
-                    func = decorate_generator_step(func, attr)
-                    new_nmspc.update({
-                        "_last_return": None,
-                        "_last_except": None,
-                        "_coroutine": None,
-                    })
-                elif inspect.isasyncgenfunction(func):
-                    raise ValueError("Illegal step function: {}. It probably mixes both async/await and yield".format(func))
-                elif inspect.isfunction(func):
-                    func = decorate_normal_func(func, attr)
-                else:
-                    raise ValueError("Illegal step function: {}".format(func))
-                new_nmspc[attr] = func
-            elif (
-                isinstance(func, types.FunctionType)
-                or isinstance(func, property)
-                or isinstance(func, classmethod)
-                or attr[0] == "_"
-            ):
-                new_nmspc[attr] = func
-            elif attr == "defaults":
-                defaults.update(func)
-            elif inspect.isfunction(func):
-                new_nmspc[attr] = func
-            else:
-                defaults[attr] = copy(func)
+from mesa import Model
+from time import time as current_time
 
+from . import agents as agentmod, datacollection, utils, time, network, events
 
-        # Add attributes for their use in the decorated functions
-        return super().__new__(mcls, name, bases, new_nmspc)
 
+# TODO: maybe add metaclass to read attributes of a model
 
-class BaseAgent(MesaAgent, MutableMapping, metaclass=MetaAgent):
+class BaseEnvironment(Model):
     """
-    A special type of Mesa Agent that:
+    The environment is key in a simulation. It controls how agents interact,
+    and what information is available to them.
 
-    * Can be used as a dictionary to access its state.
-    * Has logging built-in
-    * Can be given default arguments through a defaults class attribute,
-    which will be used on construction to initialize each agent's state
+    This is an opinionated version of `mesa.Model` class, which adds many
+    convenience methods and abstractions.
 
-    Any attribute that is not preceded by an underscore (`_`) will also be added to its state.
+    The environment parameters and the state of every agent can be accessed
+    both by using the environment as a dictionary and with the environment's
+    :meth:`soil.environment.Environment.get` method.
     """
 
-    def __init__(self, unique_id, model, name=None, init=True, **kwargs):
-        assert isinstance(unique_id, int)
-        super().__init__(unique_id=unique_id, model=model)
+    collector_class = datacollection.SoilCollector
+    schedule_class = time.TimedActivation
 
-        self.name = (
-            str(name) if name else "{}[{}]".format(type(self).__name__, self.unique_id)
+    def __new__(cls,
+                *args: Any,
+                seed="default",
+                dir_path=None,
+                collector_class: type = None,
+                agent_reporters: Optional[Any] = None,
+                model_reporters: Optional[Any] = None,
+                tables: Optional[Any] = None,
+                **kwargs: Any) -> Any:
+        """Create a new model with a default seed value"""
+        seed = seed or str(current_time())
+        self = super().__new__(cls, *args, seed=seed, **kwargs)
+        self.dir_path = dir_path or os.getcwd()
+        collector_class = collector_class or cls.collector_class
+        self.datacollector = collector_class(
+            model_reporters=model_reporters,
+            agent_reporters=agent_reporters,
+            tables=tables,
         )
+        for k in dir(cls):
+            v = getattr(cls, k)
+            if isinstance(v, property):
+                v = v.fget
+            if getattr(v, "add_to_report", False):
+                self.add_model_reporter(k, k)
+
+        return self
+
+    def __init__(
+        self,
+        *,
+        id="unnamed_env",
+        seed="default",
+        dir_path=None,
+        schedule=None,
+        schedule_class=None,
+        logger = None,
+        agents: Optional[Dict] = None,
+        collector_class: type = datacollection.SoilCollector,
+        agent_reporters: Optional[Any] = None,
+        model_reporters: Optional[Any] = None,
+        tables: Optional[Any] = None,
+        init: bool = True,
+        **env_params,
+    ):
+
+        super().__init__()
 
-        self.alive = True
 
-        logger = utils.logger.getChild(getattr(self.model, "id", self.model)).getChild(
-            self.name
-        )
-        self.logger = logging.LoggerAdapter(logger, {"agent_name": self.name})
+        self.current_id = -1
+
+        self.id = id
 
-        if hasattr(self, "level"):
-            self.logger.setLevel(self.level)
+        if logger:
+            self.logger = logger
+        else:
+            self.logger = utils.logger.getChild(self.id)
 
-        for k in self._defaults:
-            v = getattr(model, k, None)
-            if v is not None:
-                setattr(self, k, v)
-
-        for (k, v) in self._defaults.items():
-            if not hasattr(self, k) or getattr(self, k) is None:
-                setattr(self, k, deepcopy(v))
+        self.schedule = schedule
+        if schedule is None:
+            if schedule_class is None:
+                schedule_class = self.schedule_class
+            self.schedule = schedule_class(self)
 
-        for (k, v) in kwargs.items():
-            setattr(self, k, v)
+        for (k, v) in env_params.items():
+            self[k] = v
 
+        if agents:
+            self.add_agents(**agents)
         if init:
             self.init()
+            self.datacollector.collect(self)
 
     def init(self):
         pass
 
-    def __hash__(self):
-        return hash(self.unique_id)
-
-    def prob(self, probability):
-        return prob(probability, self.model.random)
-
-    @classmethod
-    def w(cls, **kwargs):
-        return custom(cls, **kwargs)
-
-    # TODO: refactor to clean up mesa compatibility
     @property
-    def id(self):
-        msg = "This attribute is deprecated. Use `unique_id` instead"
-        warnings.warn(msg, DeprecationWarning)
-        print(msg, file=sys.stderr)
-        return self.unique_id
+    def agents(self):
+        return agentmod.AgentView(self.schedule._agents, getattr(self.schedule, "agents_by_type", None))
 
-    @classmethod
-    def from_dict(cls, model, attrs, warn_extra=True):
-        ignored = {}
-        args = {}
-        for k, v in attrs.items():
-            if k in inspect.signature(cls).parameters:
-                args[k] = v
-            else:
-                ignored[k] = v
-        if ignored and warn_extra:
-            utils.logger.info(
-                f"Ignoring the following arguments for agent class { agent_class.__name__ }: { ignored }"
-            )
-        return cls(model=model, **args)
+    def agent(self, *args, **kwargs):
+        return agentmod.AgentView(self.schedule._agents, self.schedule.agents_by_type).one(*args, **kwargs)
 
-    def __getitem__(self, key):
-        try:
-            return getattr(self, key)
-        except AttributeError:
-            raise KeyError(f"key {key}  not found in agent")
+    def count_agents(self, *args, **kwargs):
+        return sum(1 for i in self.agents(*args, **kwargs))
 
-    def __delitem__(self, key):
-        return delattr(self, key)
+    def agent_df(self, steps=False):
+        df = self.datacollector.get_agent_vars_dataframe()
+        if steps:
+            df.index.rename(["step", "agent_id"], inplace=True)
+            return df
+        model_df = self.datacollector.get_model_vars_dataframe()
+        df.index = df.index.set_levels(model_df.time, level=0).rename(["time", "agent_id"])
+        return df
+
+    def model_df(self, steps=False):
+        df = self.datacollector.get_model_vars_dataframe()
+        if steps:
+            return df
+        df.index.rename("step", inplace=True)
+        return df.reset_index().set_index("time")
 
-    def __contains__(self, key):
-        return hasattr(self, key)
-
-    def __setitem__(self, key, value):
-        setattr(self, key, value)
-
-    def __len__(self):
-        return sum(1 for n in self.keys())
+    @property
+    def now(self):
+        if self.schedule is not None:
+            return self.schedule.time
+        raise Exception(
+            "The environment has not been scheduled, so it has no sense of time"
+        )
+    def init_agents(self):
+        pass
 
-    def __iter__(self):
-        return self.items()
+    def add_agent(self, agent_class, unique_id=None, **agent):
+        if unique_id is None:
+            unique_id = self.next_id()
 
-    def keys(self):
-        return (k for k in self.__dict__ if k[0] != "_" and k not in IGNORED_FIELDS)
+        agent["unique_id"] = unique_id
 
-    def items(self, keys=None, skip=None):
-        keys = keys if keys is not None else self.keys()
-        it = ((k, self.get(k, None)) for k in keys)
-        if skip:
-            return filter(lambda x: x[0] not in skip, it)
-        return it
+        agent = dict(**agent)
+        unique_id = agent.pop("unique_id", None)
+        if unique_id is None:
+            unique_id = self.next_id()
 
-    def get(self, key, default=None):
-        try:
-            return getattr(self, key)
-        except AttributeError:
-            try:
-                return getattr(self.model, key)
-            except AttributeError:
-                return default
+        a = agent_class(unique_id=unique_id, model=self, **agent)
 
-    @property
-    def now(self):
-        try:
-            return self.model.now
-        except AttributeError:
-            # No environment
-            return None
+        self.schedule.add(a)
+        return a
 
-    def die(self, msg=None):
-        if msg:
-            self.info("Agent dying:", msg)
-        else:
-            self.debug(f"agent dying")
-        self.alive = False
-        try:
-            self.model.schedule.remove(self)
-        except KeyError:
-            pass
-        return time.Delay(time.INFINITY)
+    def remove_agent(self, agent):
+        agent.alive = False
+        self.schedule.remove(agent)
 
-    def step(self):
-        raise NotImplementedError("Agent must implement step method")
+    def add_agents(self, agent_classes: List[type], k, weights: Optional[List[float]] = None, **kwargs):
+        if isinstance(agent_classes, type):
+            agent_classes = [agent_classes]
+        if weights is None:
+            weights = [1] * len(agent_classes)
 
-    def _check_alive(self):
-        if not self.alive:
-            raise time.DeadAgent(self.unique_id)
+        for cls in self.random.choices(agent_classes, weights=weights, k=k):
+            self.add_agent(agent_class=cls, **kwargs)
 
-    def log(self, *message, level=logging.INFO, **kwargs):
+    def log(self, message, *args, level=logging.INFO, **kwargs):
         if not self.logger.isEnabledFor(level):
             return
-        message = " ".join(str(i) for i in message)
-        message = "[@{:>4}]\t{:>10}: {}".format(self.now, repr(self), message)
+        message = message + " ".join(str(i) for i in args)
+        message = " @{:>3}: {}".format(self.now, message)
         for k, v in kwargs:
             message += " {k}={v} ".format(k, v)
         extra = {}
         extra["now"] = self.now
-        extra["unique_id"] = self.unique_id
-        extra["agent_name"] = self.name
+        extra["id"] = self.id
         return self.logger.log(level, message, extra=extra)
 
-    def debug(self, *args, **kwargs):
-        return self.log(*args, level=logging.DEBUG, **kwargs)
-
-    def info(self, *args, **kwargs):
-        return self.log(*args, level=logging.INFO, **kwargs)
-
-    def count_agents(self, **kwargs):
-        return len(list(self.get_agents(**kwargs)))
-
-    def get_agents(self, *args, **kwargs):
-        it = self.iter_agents(*args, **kwargs)
-        return list(it)
-
-    def iter_agents(self, *args, **kwargs):
-        yield from filter_agents(self.model.schedule._agents, *args, **kwargs)
-
-    def __str__(self):
-        return self.to_str()
-
-    def to_str(self, keys=None, skip=None, pretty=False):
-        content = dict(self.items(keys=keys))
-        if pretty and content:
-            d = content
-            content = "\n"
-            for k, v in d.items():
-                content += f"- {k}: {v}\n"
-            content = textwrap.indent(content, "    ")
-        return f"{repr(self)}{content}"
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}({self.unique_id})"
-    
-    def at(self, at):
-        return time.Delay(float(at) - self.now)
-    
-    def delay(self, delay=1):
-        return time.Delay(delay)
-
-
-def prob(prob, random):
-    """
-    A true/False uniform distribution with a given probability.
-    To be used like this:
-
-    .. code-block:: python
-
-          if prob(0.3):
-              do_something()
-
-    """
-    r = random.random()
-    return r < prob
-
+    def step(self):
+        """
+        Advance one step in the simulation, and update the data collection and scheduler appropriately
+        """
+        super().step()
+        self.schedule.step()
+        self.datacollector.collect(self)
+        if self.now == time.INFINITY:
+            self.running = False
+
+        if self.logger.isEnabledFor(logging.DEBUG):
+            msg = "Model data:\n"
+            max_width = max(len(k) for k in self.datacollector.model_vars.keys())
+            for (k, v) in self.datacollector.model_vars.items():
+                # msg += f"\t{k:<{max_width}}"
+                msg += f"\t{k:<{max_width}}: {v[-1]}\n"
+            self.logger.debug(f"--- Steps: {self.schedule.steps:^5} - Time: {self.now:^5} --- " + msg)
+
+    def add_model_reporter(self, name, func=None):
+        if not func:
+            func = name
+        self.datacollector._new_model_reporter(name, func)
+
+    def add_agent_reporter(self, name, reporter=None, agent_class=None, *, agent_type=None):
+        if agent_type:
+            print("agent_type is deprecated, use agent_class instead", file=sys.stderr)
+        agent_class = agent_type or agent_class
+        if not reporter and not agent_class:
+            reporter = name
+        if agent_class:
+            if reporter:
+                _orig = reporter
+            else:
+                _orig = lambda a: getattr(a, name)
+            reporter = lambda a: (_orig(a) if isinstance(a, agent_class) else None)
+        self.datacollector._new_agent_reporter(name, reporter)
 
-def calculate_distribution(network_agents=None, agent_class=None):
-    """
-    Calculate the threshold values (thresholds for a uniform distribution)
-    of an agent distribution given the weights of each agent type.
+    @classmethod
+    def run(cls, *,
+            name=None,
+            iterations=1,
+            num_processes=1, **kwargs):
+        from .simulation import Simulation
+        return Simulation(name=name or cls.__name__,
+                          model=cls, iterations=iterations,
+                          num_processes=num_processes, **kwargs).run()
 
-    The input has this form: ::
+    def __getitem__(self, key):
+        try:
+            return getattr(self, key)
+        except AttributeError:
+            raise KeyError(f"key {key}  not found in environment")
 
-            [
-            {'agent_class': 'agent_class_1',
-                'weight': 0.2,
-                'state': {
-                    'id': 0
-                }
-            },
-            {'agent_class': 'agent_class_2',
-                'weight': 0.8,
-                'state': {
-                    'id': 1
-                }
-            }
-            ]
+    def __delitem__(self, key):
+        return delattr(self, key)
 
-    In this example, 20% of the nodes will be marked as type
-    'agent_class_1'.
-    """
-    if network_agents:
-        network_agents = [
-            deepcopy(agent) for agent in network_agents if not hasattr(agent, "id")
-        ]
-    elif agent_class:
-        network_agents = [{"agent_class": agent_class}]
-    else:
-        raise ValueError("Specify a distribution or a default agent type")
-
-    # Fix missing weights and incompatible types
-    for x in network_agents:
-        x["weight"] = float(x.get("weight", 1))
-
-    # Calculate the thresholds
-    total = sum(x["weight"] for x in network_agents)
-    acc = 0
-    for v in network_agents:
-        if "ids" in v:
-            continue
-        upper = acc + (v["weight"] / total)
-        v["threshold"] = [acc, upper]
-        acc = upper
-    return network_agents
-
-
-def _serialize_type(agent_class, known_modules=[], **kwargs):
-    if isinstance(agent_class, str):
-        return agent_class
-    known_modules += ["soil.agents"]
-    return serialization.serialize(agent_class, known_modules=known_modules, **kwargs)[
-        1
-    ]  # Get the name of the class
-
-
-def _deserialize_type(agent_class, known_modules=[]):
-    if not isinstance(agent_class, str):
-        return agent_class
-    known = known_modules + ["soil.agents", "soil.agents.custom"]
-    agent_class = serialization.deserializer(agent_class, known_modules=known)
-    return agent_class
-
-
-class AgentView(Mapping, Set):
-    """A lazy-loaded list of agents."""
-
-    __slots__ = ("_agents",)
-
-    def __init__(self, agents):
-        self._agents = agents
+    def __contains__(self, key):
+        return hasattr(self, key)
 
-    def __getstate__(self):
-        return {"_agents": self._agents}
+    def __setitem__(self, key, value):
+        setattr(self, key, value)
 
-    def __setstate__(self, state):
-        self._agents = state["_agents"]
+    def __str__(self):
+        return str(dict(self))
 
-    # Mapping methods
     def __len__(self):
-        return len(self._agents)
+        return sum(1 for n in self.keys())
 
     def __iter__(self):
-        yield from self._agents.values()
-
-    def __getitem__(self, agent_id):
-        if isinstance(agent_id, slice):
-            raise ValueError(f"Slicing is not supported")
-        if agent_id in self._agents:
-            return self._agents[agent_id]
-        raise ValueError(f"Agent {agent_id} not found")
-
-    def filter(self, *args, **kwargs):
-        yield from filter_agents(self._agents, *args, **kwargs)
-
-    def one(self, *args, **kwargs):
-        return next(filter_agents(self._agents, *args, **kwargs))
-
-    def __call__(self, *args, **kwargs):
-        return list(self.filter(*args, **kwargs))
+        return iter(self.agents())
 
-    def __contains__(self, agent_id):
-        return agent_id in self._agents
-
-    def __str__(self):
-        return str(list(unique_id for unique_id in self.keys()))
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}({self})"
+    def get(self, key, default=None):
+        return self[key] if key in self else default
 
+    def keys(self):
+        return (k for k in self.__dict__ if k[0] != "_")
 
-def filter_agents(
-    agents: dict,
-    *id_args,
-    unique_id=None,
-    state_id=None,
-    agent_class=None,
-    ignore=None,
-    state=None,
-    limit=None,
-    **kwargs,
-):
+class NetworkEnvironment(BaseEnvironment):
     """
-    Filter agents given as a dict, by the criteria given as arguments (e.g., certain type or state id).
+    The NetworkEnvironment is an environment that includes one or more networkx.Graph intances
+    and methods to associate agents to nodes and vice versa.
     """
-    assert isinstance(agents, dict)
 
-    ids = []
-
-    if unique_id is not None:
-        if isinstance(unique_id, list):
-            ids += unique_id
+    def __init__(self,
+                 *args,
+                 topology: Optional[Union[nx.Graph, str]] = None,
+                 agent_class: Optional[Type[agentmod.Agent]] = None,
+                 network_generator: Optional[Callable] = None,
+                 network_params: Optional[Dict] = {},
+                 init=True,
+                 **kwargs):
+        self.topology = topology
+        self.network_generator = network_generator
+        self.network_params = network_params
+        if topology or network_params or network_generator:
+            self.create_network(topology, generator=network_generator, **network_params)
         else:
-            ids.append(unique_id)
-
-    if id_args:
-        ids += id_args
+            self.G = nx.Graph()
+        super().__init__(*args, **kwargs, init=False)
 
-    if ids:
-        f = (agents[aid] for aid in ids if aid in agents)
-    else:
-        f = agents.values()
-
-    if state_id is not None and not isinstance(state_id, (tuple, list)):
-        state_id = tuple([state_id])
+        self.agent_class = agent_class
+        if self.agent_class:
+            self.populate_network(self.agent_class)
+        self._check_agent_nodes()
+        if init:
+            self.init()
+            self.datacollector.collect(self)
 
-    if agent_class is not None:
-        agent_class = _deserialize_type(agent_class)
+    def add_agent(self, agent_class, *args, node_id=None, topology=None, **kwargs):
+        if node_id is None and topology is None:
+            return super().add_agent(agent_class, *args, **kwargs)
         try:
-            agent_class = tuple(agent_class)
+            a = super().add_agent(agent_class, *args, node_id=node_id, **kwargs)
         except TypeError:
-            agent_class = tuple([agent_class])
-
-    if ignore:
-        f = filter(lambda x: x not in ignore, f)
-
-    if state_id is not None:
-        f = filter(lambda agent: agent.get("state_id", None) in state_id, f)
-
-    if agent_class is not None:
-        f = filter(lambda agent: isinstance(agent, agent_class), f)
-
-    state = state or dict()
-    state.update(kwargs)
-
-    for k, vs in state.items():
-        if not isinstance(vs, list):
-            vs = [vs]
-        f = filter(lambda agent: any(getattr(agent, k, None) == v for v in vs), f)
-
-    if limit is not None:
-        f = islice(f, limit)
-
-    yield from f
+            self.logger.warning(f"Agent constructor for {agent_class} does not have a node_id attribute. Might be a bug.")
+            a = super().add_agent(agent_class, *args, **kwargs)
+        self.G.nodes[node_id]["agent"] = a
+        return a
+
+    def remove_agent(self, agent, remove_node=True):
+        super().remove_agent(agent)
+        if remove_node and hasattr(agent, "remove_node"):
+            agent.remove_node()
+
+    def add_agents(self, *args, k=None, **kwargs):
+        if not k and not self.G:
+            raise ValueError("Cannot add agents to an empty network")
+        super().add_agents(*args, k=k or len(self.G), **kwargs)
+
+    def create_network(self, topology=None, generator=None, path=None, **network_params):
+        if topology is not None:
+            topology = network.from_topology(topology, dir_path=self.dir_path)
+        elif path is not None:
+            topology = network.from_topology(path, dir_path=self.dir_path)
+        elif generator is not None:
+            params = dict(generator=generator,
+                                           dir_path=self.dir_path,
+                                           seed=self.random,
+                                           **network_params)
+            try:
+                topology = network.from_params(**params)
+            except TypeError:
+                del params["seed"]
+                topology = network.from_params(**params)
+        else:
+            raise ValueError("topology must be a networkx.Graph or a string, or network_generator must be provided")
+        self.G = topology
 
+    def init_agents(self, *args, **kwargs):
+        """Initialize the agents from a"""
+        super().init_agents(*args, **kwargs)
 
-def from_config(
-    cfg: config.AgentConfig, random, topology: nx.Graph = None
-) -> List[Dict[str, Any]]:
-    """
-    This function turns an agentconfig into a list of individual "agent specifications", which are just a dictionary
-    with the parameters that the environment will use to construct each agent.
-
-    This function does NOT return a list of agents, mostly because some attributes to the agent are not known at the
-    time of calling this function, such as `unique_id`.
-    """
-    default = cfg or config.AgentConfig()
-    if not isinstance(cfg, config.AgentConfig):
-        cfg = config.AgentConfig(**cfg)
-
-    agents = []
-
-    assigned_total = 0
-    assigned_network = 0
-
-    if cfg.fixed is not None:
-        agents, assigned_total, assigned_network = _from_fixed(
-            cfg.fixed, topology=cfg.topology, default=cfg
+    @property
+    def network_agents(self):
+        """Return agents still alive and assigned to a node in the network."""
+        for (id, data) in self.G.nodes(data=True):
+            if "agent" in data:
+                agent = data["agent"]
+                if getattr(agent, "alive", True):
+                    yield agent
+
+    def add_node(self, agent_class, unique_id=None, node_id=None, find_unassigned=False, **kwargs):
+        if unique_id is None:
+            unique_id = self.next_id()
+        if node_id is None:
+            if find_unassigned:
+                node_id = network.find_unassigned(
+                    G=self.G, shuffle=True, random=self.random
+                )
+            if node_id is None:
+                node_id = f"Node_for_agent_{unique_id}"
+            assert node_id not in self.G.nodes
+
+        if node_id not in self.G.nodes:
+            self.G.add_node(node_id)
+
+        assert "agent" not in self.G.nodes[node_id]
+
+        a = self.add_agent(
+            unique_id=unique_id,
+            agent_class=agent_class,
+            topology=self.G,
+            node_id=node_id,
+            **kwargs,
         )
+        a["visible"] = True
+        return a
 
-    n = cfg.n
-
-    if cfg.distribution:
-        topo_size = len(topology) if topology else 0
-
-        networked = []
-        total = []
-
-        for d in cfg.distribution:
-            if d.strategy == config.Strategy.topology:
-                topo = d.topology if ("topology" in d.__fields_set__) else cfg.topology
-                if not topo:
-                    raise ValueError(
-                        'The "topology" strategy only works if the topology parameter is set to True'
-                    )
-                if not topo_size:
-                    raise ValueError(
-                        f"Topology does not have enough free nodes to assign one to the agent"
-                    )
-
-                networked.append(d)
-
-            if d.strategy == config.Strategy.total:
-                if not cfg.n:
-                    raise ValueError(
-                        'Cannot use the "total" strategy without providing the total number of agents'
-                    )
-                total.append(d)
-
-        if networked:
-            new_agents = _from_distro(
-                networked,
-                n=topo_size - assigned_network,
-                topology=topo,
-                default=cfg,
-                random=random,
-            )
-            assigned_total += len(new_agents)
-            assigned_network += len(new_agents)
-            agents += new_agents
-
-        if total:
-            remaining = n - assigned_total
-            agents += _from_distro(total, n=remaining, default=cfg, random=random)
-
-        if assigned_network < topo_size:
-            utils.logger.warn(
-                f"The total number of agents does not match the total number of nodes in "
-                "every topology. This may be due to a definition error: assigned: "
-                f"{ assigned } total size: { topo_size }"
-            )
-
-    return agents
+    def _check_agent_nodes(self):
+        """
+        Detect nodes that have agents assigned to them.
+        """
+        for (id, data) in self.G.nodes(data=True):
+            if "agent_id" in data:
+                agent = self.agents(data["agent_id"])
+                self.G.nodes[id]["agent"] = agent
+                assert not getattr(agent, "node_id", None) or agent.node_id == id
+                agent.node_id = id
+        for agent in self.agents():
+            if hasattr(agent, "node_id"):
+                node_id = agent["node_id"]
+                if node_id not in self.G.nodes:
+                    raise ValueError(f"Agent {agent} is assigned to node {agent.node_id} which is not in the network")
+                node = self.G.nodes[node_id]
+                if node.get("agent") is not None and node["agent"] != agent:
+                    raise ValueError(f"Node {node_id} already has a different agent assigned to it")
+                self.G.nodes[node_id]["agent"] = agent
+
+    def add_agents(self, agent_classes: List[type], k=None, weights: Optional[List[float]] = None, **kwargs):
+        if k is None:
+            k = len(self.G)
+            if not k:
+                raise ValueError("Cannot add agents to an empty network")
+        super().add_agents(agent_classes, k=k, weights=weights, **kwargs)
+
+    def agent_for_node_id(self, node_id):
+        return self.G.nodes[node_id].get("agent")
+
+    def populate_network(self, agent_class: List[Model], weights: List[float] = None, **agent_params):
+        if isinstance(agent_class, type):
+            agent_class = [agent_class]
+        else:
+            agent_class = list(agent_class)
+        if not weights:
+            weights = [1] * len(agent_class)
+        assert len(self.G)
+        classes = self.random.choices(agent_class, weights, k=len(self.G))
+        toadd = []
+        for (cls, (node_id, node)) in zip(classes, self.G.nodes(data=True)):
+            if "agent" in node:
+                continue
+            node["agent"] = None # Reserve
+            toadd.append(dict(node_id=node_id, topology=self.G,  agent_class=cls, **agent_params))
+        for d in toadd:
+            a = self.add_agent(**d)
+            self.G.nodes[d["node_id"]]["agent"] = a
+        assert all("agent" in node for (_, node) in self.G.nodes(data=True))
+        assert len(list(self.network_agents))
+
+
+class EventedEnvironment(BaseEnvironment):
+
+    def __init__(self, *args, **kwargs):
+        self._inbox = dict()
+        super().__init__(*args, **kwargs)
+        self._can_reschedule = hasattr(self.schedule, "add_callback") and hasattr(self.schedule, "remove_callback")
+        self._can_reschedule = True
+        self._callbacks = {}
 
+    def register(self, agent):
+        self._inbox[agent.unique_id] = []
 
-def _from_fixed(
-    lst: List[config.FixedAgentConfig],
-    topology: bool,
-    default: config.SingleAgentConfig,
-) -> List[Dict[str, Any]]:
-    agents = []
-
-    counts_total = 0
-    counts_network = 0
-
-    for fixed in lst:
-        agent = {}
-        if default:
-            agent = default.state.copy()
-        agent.update(fixed.state)
-        cls = serialization.deserialize(
-            fixed.agent_class or (default and default.agent_class)
-        )
-        agent["agent_class"] = cls
-        topo = (
-            fixed.topology
-            if ("topology" in fixed.__fields_set__)
-            else topology or default.topology
-        )
+    def inbox_for(self, agent):
+        try:
+            return self._inbox[agent.unique_id]
+        except KeyError:
+            raise ValueError(f"Trying to access inbox for unregistered agent: {agent} (class: {type(agent)}). "
+                            "Make sure your agent is of type EventedAgent and it is registered with the environment.")
 
-        if topo:
-            agent["topology"] = True
-            counts_network += 1
-        if not fixed.hidden:
-            counts_total += 1
-        agents.append(agent)
-
-    return agents, counts_total, counts_network
-
-
-def _from_distro(
-    distro: List[config.AgentDistro],
-    n: int,
-    default: config.SingleAgentConfig,
-    random,
-    topology: str = None
-) -> List[Dict[str, Any]]:
-
-    agents = []
-
-    if n is None:
-        if any(lambda dist: dist.n is None, distro):
-            raise ValueError(
-                "You must provide a total number of agents, or the number of each type"
+    @coroutine
+    def _polling_callback(self, agent, expiration, delay):
+        # this wakes the agent up at every step. It is better to wait until timeout (or inf)
+        # and if a message is received before that, reschedule the agent
+        # (That is implemented in the `received` method)
+        inbox = self.inbox_for(agent)
+        while self.now < expiration:
+            if inbox:
+                return self.process_messages(inbox)
+            yield time.Delay(delay)
+        raise events.TimedOut("No message received")
+
+    @coroutine
+    def received(self, agent, expiration=None, timeout=None, delay=1):
+        if not expiration:
+            if timeout:
+                expiration = self.now + timeout
+            else:
+                expiration = float("inf")
+        inbox = self.inbox_for(agent)
+        if inbox:
+            return self.process_messages(inbox)
+
+        if self._can_reschedule:
+            checked = False
+            def cb():
+                nonlocal checked
+                if checked:
+                    return time.INFINITY
+                checked = True
+                self.schedule.add_callback(self.now, agent.step)
+            self.schedule.add_callback(expiration, cb)
+            self._callbacks[agent.unique_id] = cb
+            yield time.INFINITY
+        res = yield from self._polling_callback(agent, expiration, delay)
+        return res
+
+
+    def tell(self, msg, recipient, sender=None, expiration=None, timeout=None, **kwargs):
+        if expiration is None:
+            expiration = float("inf") if timeout is None else self.now + timeout
+        self._add_to_inbox(recipient.unique_id,
+            events.Tell(timestamp=self.now,
+                        payload=msg,
+                        sender=sender,
+                        expiration=expiration,
+                        **kwargs))
+
+    def broadcast(self, msg, sender, ttl=None, expiration=None, agent_class=None):
+        expiration = expiration if ttl is None else self.now + ttl
+        # This only works for Soil environments. Mesa agents do not have an `agents` method
+        sender_id = sender.unique_id
+        for (agent_id, inbox) in self._inbox.items():
+            if agent_id == sender_id:
+                continue
+            if agent_class and not isinstance(self.agents(unique_id=agent_id), agent_class):
+                continue
+            self.logger.debug(f"Telling {agent_id}: {msg} ttl={ttl}")
+            self._add_to_inbox(agent_id,
+                events.Tell(
+                    payload=msg,
+                    sender=sender,
+                    expiration=expiration,
+                )
             )
-        n = sum(dist.n for dist in distro)
-
-    weights = list(dist.weight if dist.weight is not None else 1 for dist in distro)
-    minw = min(weights)
-    norm = list(weight / minw for weight in weights)
-    total = sum(norm)
-    chunk = n // total
-
-    # random.choices would be enough to get a weighted distribution. But it can vary a lot for smaller k
-    # So instead we calculate our own distribution to make sure the actual ratios are close to what we would expect
-
-    # Calculate how many times each has to appear
-    indices = list(
-        chain.from_iterable([idx] * int(n * chunk) for (idx, n) in enumerate(norm))
-    )
-
-    # Complete with random agents following the original weight distribution
-    if len(indices) < n:
-        indices += random.choices(
-            list(range(len(distro))),
-            weights=[d.weight for d in distro],
-            k=n - len(indices),
-        )
-
-    # Deserialize classes for efficiency
-    classes = list(
-        serialization.deserialize(i.agent_class or default.agent_class) for i in distro
-    )
-
-    # Add them in random order
-    random.shuffle(indices)
-
-    for idx in indices:
-        d = distro[idx]
-        agent = d.state.copy()
-        cls = classes[idx]
-        agent["agent_class"] = cls
-        if default:
-            agent.update(default.state)
-        topology = (
-            d.topology
-            if ("topology" in d.__fields_set__)
-            else topology or default.topology
-        )
-        if topology:
-            agent["topology"] = topology
-        agents.append(agent)
-
-    return agents
-
-
-from .network_agents import *
-from .fsm import *
-from .evented import *
-from typing import Optional
-
-
-class Agent(FSM, EventedAgent, NetworkAgent):
-    """Default agent class, has both network and event capabilities"""
-
-
-class Noop(Agent):
-    def step(self):
-        return
-
-
-from ..environment import NetworkEnvironment
-
-
-from .BassModel import *
-from .IndependentCascadeModel import *
-from .SISaModel import *
-from .CounterModel import *
+    def _add_to_inbox(self, inbox_id, msg):
+        self._inbox[inbox_id].append(msg)
+        if inbox_id in self._callbacks:
+            cb = self._callbacks.pop(inbox_id)
+            cb()
+
+    @coroutine
+    def ask(self, msg, recipient, sender=None, expiration=None, timeout=None, delay=1):
+        ask = events.Ask(timestamp=self.now, payload=msg, sender=sender)
+        self._add_to_inbox(recipient.unique_id, ask)
+        expiration = float("inf") if timeout is None else self.now + timeout
+        while self.now < expiration:
+            if ask.reply:
+                return ask.reply
+            yield time.Delay(delay)
+        raise events.TimedOut("No reply received")
+
+    def process_messages(self, inbox):
+        valid = list()
+        for msg in inbox:
+            if msg.expired(self.now):
+                continue
+            valid.append(msg)
+        inbox.clear()
+        return valid
 
 
-def custom(cls, **kwargs):
-    """Create a new class from a template class and keyword arguments"""
-    return type(cls.__name__, (cls,), kwargs)
+class Environment(EventedEnvironment, NetworkEnvironment):
+    pass
```

### Comparing `soil-1.0.0rc5.post1/soil/agents/fsm.py` & `soil-1.0.0rc7/soil/agents/fsm.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,72 +2,82 @@
 from .. import time
 from types import coroutine
 from functools import partial, wraps
 import inspect
 
 
 class State:
-    __slots__ = ("awaitable", "f", "generator", "name", "default")
+    __slots__ = ("awaitable", "f", "attribute", "generator", "name", "default")
 
     def __init__(self, f, name, default, generator, awaitable):
         self.f = f
         self.name = name
+        self.attribute = "_{}".format(name)
         self.generator = generator
         self.awaitable = awaitable
         self.default = default
 
-    @coroutine
-    def step(self, obj):
-        if self.generator or self.awaitable:
-            f = self.f
-            next_state = yield from f(obj)
-            return next_state
-
-        else:
-            return self.f(obj)
-
     @property
     def id(self):
         return self.name
-
-    def __call__(self, *args, **kwargs):
-        raise Exception("States should not be called directly")
-
-class UnboundState(State):
+    
+    def __get__(self, obj, owner=None):
+        if obj is None:
+            return self
+        try:
+            return getattr(obj, self.attribute)
+        except AttributeError:
+            b = self.bind(obj)
+            setattr(obj, self.attribute, b)
+            return b
 
     def bind(self, obj):
         bs = BoundState(self.f, self.name, self.default, self.generator, self.awaitable, obj=obj)
         setattr(obj, self.name, bs)
         return bs
 
+    def __call__(self, *args, **kwargs):
+        raise Exception("States should not be called directly")
+
 
 class BoundState(State):
     __slots__ = ("obj", )
 
     def __init__(self, *args, obj):
         super().__init__(*args)
         self.obj = obj
-    
+
+    @coroutine
+    def __call__(self):
+        if self.generator or self.awaitable:
+            f = self.f
+            next_state = yield from f(self.obj)
+            return next_state
+
+        else:
+            return self.f(self.obj)
+
+
     def delay(self, delta=0):
         return self, self.obj.delay(delta)
-    
+
     def at(self, when):
         return self, self.obj.at(when)
 
 
 def state(name=None, default=False):
     def decorator(func, name=None):
         """
         A state function should return either a state id, or a tuple (state_id, when)
         The default value for state_id is the current state id.
         """
         name = name or func.__name__
         generator = inspect.isgeneratorfunction(func)
         awaitable = inspect.iscoroutinefunction(func) or inspect.isasyncgen(func)
-        return UnboundState(func, name, default, generator, awaitable)
+        return State(func, name, default, generator, awaitable)
 
     if callable(name):
         return decorator(name)
     else:
         return partial(decorator, name=name)
 
 
@@ -109,77 +119,83 @@
             setattr(cls, k, v)
         return cls
 
 
 class FSM(BaseAgent, metaclass=MetaFSM):
     def __init__(self, init=True, state_id=None, **kwargs):
         super().__init__(**kwargs, init=False)
+        bound_states = {}
+        for (k, v) in list(self._states.items()):
+            if isinstance(v, State):
+                v = v.bind(self)
+            bound_states[k] = v
+            setattr(self, k, v)
+
+        self._states = bound_states
+
         if state_id is not None:
             self._set_state(state_id)
+        else:
+            self._set_state(self._state)
         # If more than "dead" state is defined, but no default state
         if len(self._states) > 1 and not self._state:
             raise ValueError(
                 f"No default state specified for {type(self)}({self.unique_id})"
             )
-        for (k, v) in self._states.items():
-            setattr(self, k, v.bind(self))
 
         if init:
             self.init()
-        if not self._state and (self.step == FSM.step):
-            raise ValueError(
-                f"No default state specified for {type(self)}({self.unique_id})"
-            )
 
     @classmethod
     def states(cls):
         return list(cls._states.keys())
 
     @property
     def state_id(self):
         return self._state.name
     
     def set_state(self, value):
         if self.now > 0:
             raise ValueError("Cannot change state after init")
         self._set_state(value)
 
+    @coroutine
     def step(self):
         if self._state is None:
             if len(self._states) == 1:
                 raise Exception("Agent class has no valid states: {}. Make sure to define states or define a custom step function".format(self.__class__.__name__))
             else:
                 raise Exception("Invalid state (None) for agent {}".format(self))
 
-        self._check_alive()
-        next_state = yield from self._state.step(self)
+        next_state = yield from self._state()
 
         try:
             next_state, when = next_state
+            self._set_state(next_state)
+            return when
         except (TypeError, ValueError) as ex:
             try:
                 self._set_state(next_state)
                 return None
             except ValueError:
                 return next_state
 
-        self._set_state(next_state)
-        return when
-
     def _set_state(self, state):
         if state is None:
             return
         if isinstance(state, str):
             if state not in self._states:
                 raise ValueError("{} is not a valid state".format(state))
             state = self._states[state]
-        if not isinstance(state, State):
+        if isinstance(state, State):
+            state = state.bind(self)
+        elif not isinstance(state, BoundState):
             raise ValueError("{} is not a valid state".format(state))
         self._state = state
 
     def die(self, *args, **kwargs):
         super().die(*args, **kwargs)
         return self.dead.at(time.INFINITY)
 
     @state
     def dead(self):
-        return time.INFINITY
+        return time.INFINITY
```

### Comparing `soil-1.0.0rc5.post1/soil/agents/geo.py` & `soil-1.0.0rc7/soil/agents/geo.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/agents/network_agents.py` & `soil-1.0.0rc7/soil/agents/network_agents.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from . import BaseAgent
+from .. import environment
 
 
 class NetworkAgent(BaseAgent):
     def __init__(self, *args, topology=None, init=True, node_id=None, **kwargs):
         super().__init__(*args, init=False, **kwargs)
+        assert isinstance(self.model, environment.NetworkEnvironment), "NetworkAgent requires a NetworkEnvironment"
 
         self.G = topology or self.model.G
         assert self.G is not None, "Network agents should have a network"
         if node_id is None:
             nodes = self.random.choices(list(self.G.nodes), k=len(self.G))
             for n_id in nodes:
                 if "agent" not in self.G.nodes[n_id] or self.G.nodes[n_id]["agent"] is None:
                     node_id = n_id
                     break
             else:
                 node_id = len(self.G)
                 self.info(f"All nodes ({len(self.G)}) have an agent assigned, adding a new node to the graph for agent {self.unique_id}")
-                self.G.add_node(node_id)
+                self.G.add_node(node_id, find_unassigned=True)
         assert node_id is not None
         self.G.nodes[node_id]["agent"] = self
         self.node_id = node_id
         if init:
             self.init()
 
     def count_neighbors(self, state_id=None, **kwargs):
```

### Comparing `soil-1.0.0rc5.post1/soil/analysis.py` & `soil-1.0.0rc7/soil/analysis.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,16 @@
         ignore.append("time")
 
     ax = model_df.drop(ignore, axis='columns').plot();
     if agent_df is None:
         try:
             agent_df = env.agent_df()
         except UserWarning:
-            print("No agent dataframe provided and no agent reporters found. Skipping agent plot.", file=sys.stderr)
+            print("No agent dataframe provided and no agent reporters found. "
+                  "Skipping agent plot.", file=sys.stderr)
             return
     if not agent_df.empty:
         agent_df.unstack().apply(lambda x: x.value_counts(),
                                  axis=1).fillna(0).plot(ax=ax,
                                                         secondary_y=True)
 
 
@@ -39,19 +40,14 @@
     # TODO: improve url parsing. This is a hacky way to check we weren't given a URL
     if "://" not in fpath:
         fpath = f"sqlite:///{fpath}"
     engine = sqlalchemy.create_engine(fpath)
     with engine.connect() as conn:
         env = pd.read_sql_table("env", con=conn,
                                 index_col="step").reset_index().set_index([
-                                    "simulation_id", "params_id",
-                                    "iteration_id", "step"
+                                    "params_id", "iteration_id", "step"
                                 ])
-        agents = pd.read_sql_table("agents", con=conn, index_col=["simulation_id", "params_id", "iteration_id", "step", "agent_id"])
+        agents = pd.read_sql_table("agents", con=conn, index_col=["params_id", "iteration_id", "step", "agent_id"])
         config = pd.read_sql_table("configuration", con=conn, index_col="simulation_id")
-        parameters = pd.read_sql_table("parameters", con=conn, index_col=["iteration_id", "params_id", "simulation_id"])
-        try:
-            parameters = parameters.pivot(columns="key", values="value")
-        except Exception as e:
-            print(f"warning: coult not pivot parameters: {e}")
+        parameters = pd.read_sql_table("parameters", con=conn, index_col=["simulation_id", "params_id", "iteration_id"])
 
         return Results(config, parameters, env, agents)
```

### Comparing `soil-1.0.0rc5.post1/soil/datacollection.py` & `soil-1.0.0rc7/soil/datacollection.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/debugging.py` & `soil-1.0.0rc7/soil/debugging.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/events.py` & `soil-1.0.0rc7/soil/events.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,22 +14,23 @@
     expiration: float = None
     timestamp: float = None
     id: int = field(default_factory=uuid4)
 
     def expired(self, when):
         return self.expiration is not None and self.expiration < when
 
-
 class Reply(Message):
     source: Message
 
 
 class Ask(Message):
     reply: Message = None
 
 
 class Tell(Message):
-    pass
+    def __post_init__(self):
+        assert self.sender is not None, "Tell requires a sender"
+
 
 
 class TimedOut(Exception):
     pass
```

### Comparing `soil-1.0.0rc5.post1/soil/exporters.py` & `soil-1.0.0rc7/soil/exporters.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import sys
 from time import time as current_time
+from datetime import datetime
 from io import BytesIO
 from textwrap import dedent, indent
 
 
 import networkx as nx
 import pandas as pd
 
@@ -70,51 +71,63 @@
     def iteration_start(self, env):
         """Method to call when a iteration start"""
         pass
 
     def iteration_end(self, env, params, params_id):
         """Method to call when a iteration ends"""
         pass
+    
+    def env_id(self, env):
+        try:
+            return env.id
+        except AttributeError:
+            return f"{env.__class__.__name__}_{current_time()}"
+
 
     def output(self, f, mode="w", **kwargs):
         if not self.dump:
             f = DryRunner(f, copy_to=self.copy_to)
         else:
             try:
                 if not os.path.isabs(f):
                     f = os.path.join(self.outdir, f)
             except TypeError:
                 pass
         return open_or_reuse(f, mode=mode, backup=self.simulation.backup, **kwargs)
 
-    def get_dfs(self, env, **kwargs):
+    def get_dfs(self, env, params_id, **kwargs):
         yield from get_dc_dfs(env.datacollector,
-                              simulation_id=self.simulation.id,
-                              iteration_id=env.id,
+                              params_id,
+                              iteration_id=self.env_id(env),
                               **kwargs)
 
 
-def get_dc_dfs(dc, **kwargs):
+def get_dc_dfs(dc, params_id, **kwargs):
     dfs = {}
     dfe = dc.get_model_vars_dataframe()
     dfe.index.rename("step", inplace=True)
     dfs["env"] = dfe
+    kwargs["params_id"] = params_id
     try:
-        dfa = dc.get_agent_vars_dataframe() 
+        dfa = dc.get_agent_vars_dataframe()
         dfa.index.rename(["step", "agent_id"], inplace=True)
         dfs["agents"] = dfa
     except UserWarning:
         pass
     for table_name in dc.tables:
         dfs[table_name] = dc.get_table_dataframe(table_name)
     for (name, df) in dfs.items():
         for (k, v) in kwargs.items():
-            df[k] = v
-        df.set_index(["simulation_id", "iteration_id"], append=True, inplace=True)
-    
+            if v:
+                df[k] = v
+            else:
+                df[k] = pd.Series(dtype="object")
+        df.reset_index(inplace=True)
+        df.set_index(["params_id", "iteration_id"], inplace=True)
+
     yield from dfs.items()
 
 
 class SQLite(Exporter):
     """Writes sqlite results"""
     sim_started = False
 
@@ -125,71 +138,88 @@
 
         from sqlalchemy import create_engine
 
         self.dbpath = os.path.join(self.outdir, f"{self.simulation.name}.sqlite")
         logger.info("Dumping results to %s", self.dbpath)
         if self.simulation.backup:
             try_backup(self.dbpath, remove=True)
-        
+
         if self.simulation.overwrite:
             if os.path.exists(self.dbpath):
                 os.remove(self.dbpath)
-        
+
+        outdir = os.path.dirname(self.dbpath)
+        if outdir and not os.path.exists(outdir):
+            os.makedirs(outdir)
+
         self.engine = create_engine(f"sqlite:///{self.dbpath}", echo=False)
 
         sim_dict = {k: serialize(v)[0] for (k,v) in self.simulation.to_dict().items()}
         sim_dict["simulation_id"] = self.simulation.id
         df = pd.DataFrame([sim_dict])
-        df.to_sql("configuration", con=self.engine, if_exists="append")
+        df.reset_index().to_sql("configuration", con=self.engine, if_exists="append", index=False)
 
     def iteration_end(self, env, params, params_id, *args, **kwargs):
         if not self.dump:
             logger.info("Running in NO DUMP mode. Results will NOT be saved to a DB.")
             return
 
         with timer(
-            "Dumping simulation {} iteration {}".format(self.simulation.name, env.id)
+            "Dumping simulation {} iteration {}".format(self.simulation.name, self.env_id(env))
         ):
-
-            pd.DataFrame([{"simulation_id": self.simulation.id,
+            d = {"simulation_id": self.simulation.id,
                            "params_id": params_id,
-                           "iteration_id": env.id,
-                           "key": k,
-                           "value": serialize(v)[0]} for (k,v) in params.items()]).to_sql("parameters", con=self.engine, if_exists="append")
+                           "iteration_id": self.env_id(env),
+            }
+            for (k,v) in params.items():
+                d[k] = serialize(v)[0]
+
+            pd.DataFrame([d]).reset_index().to_sql("parameters",
+                                                   con=self.engine,
+                                                   if_exists="append",
+                                                   index=False)
+            pd.DataFrame([{
+                "simulation_id": self.simulation.id,
+                "params_id": params_id,
+                "iteration_id": self.env_id(env),
+            }]).reset_index().to_sql("iterations",
+                                     con=self.engine,
+                                     if_exists="append",
+                                     index=False)
 
             for (t, df) in self.get_dfs(env, params_id=params_id):
-                df.to_sql(t, con=self.engine, if_exists="append")
+                df.reset_index().to_sql(t, con=self.engine, if_exists="append", index=False)
 
 class csv(Exporter):
     """Export the state of each environment (and its agents) a CSV file for the simulation"""
 
     def sim_start(self):
         super().sim_start()
 
     def iteration_end(self, env, params, params_id, *args, **kwargs):
         with timer(
             "[CSV] Dumping simulation {} iteration {} @ dir {}".format(
-                self.simulation.name, env.id, self.outdir
+                self.simulation.name, self.env_id(env), self.outdir
             )
         ):
             for (df_name, df) in self.get_dfs(env, params_id=params_id):
-                with self.output("{}.{}.csv".format(env.id, df_name), mode="a") as f:
+                with self.output("{}.{}.csv".format(self.env_id(env), df_name), mode="a") as f:
                     df.to_csv(f)
 
 
 class gexf(Exporter):
     def iteration_end(self, env, *args, **kwargs):
         if not self.dump:
             logger.info("Not dumping GEXF (NO_DUMP mode)")
             return
 
         with timer(
-            "[GEXF] Dumping simulation {} iteration {}".format(self.simulation.name, env.id)
+            "[GEXF] Dumping simulation {} iteration {}".format(self.simulation.name, self.env_id(env))
         ):
-            with self.output("{}.gexf".format(env.id), mode="wb") as f:
+            with self.output("{}.gexf".format(self.env_id(env)), mode="wb") as f:
                 nx.write_gexf(env.G, f)
 
 
 class dummy(Exporter):
     def sim_start(self):
         with self.output("dummy", "w") as f:
             f.write("simulation started @ {}\n".format(current_time()))
@@ -215,24 +245,24 @@
         nx.draw(
             env.G,
             node_size=10,
             width=0.2,
             pos=nx.spring_layout(env.G, scale=100),
             ax=f.add_subplot(111),
         )
-        with open("graph-{}.png".format(env.id)) as f:
+        with open("graph-{}.png".format(self.env_id(env))) as f:
             f.savefig(f)
 
 
 class summary(Exporter):
     """Print a summary of each iteration to sys.stdout"""
 
-    def iteration_end(self, env, *args, **kwargs):
+    def iteration_end(self, env, params_id, *args, **kwargs):
         msg = ""
-        for (t, df) in self.get_dfs(env):
+        for (t, df) in self.get_dfs(env, params_id):
             if not len(df):
                 continue
             tabs = "\t" * 2
             description = indent(str(df.describe()), tabs)
             last_line = indent(str(df.iloc[-1:]), tabs)
             # value_counts = indent(str(df.value_counts()), tabs)
             value_counts = indent(str(df.apply(lambda x: x.value_counts()).T.stack()), tabs)
@@ -258,25 +288,9 @@
         if not self.dump:
             logger.debug("NOT dumping results")
             return
         with self.output(self.simulation.id + ".dumped.yml") as f:
             logger.info(f"Dumping simulation configuration to {self.outdir}")
             f.write(self.simulation.to_yaml())
 
-class default(Exporter):
-    """Default exporter. Writes sqlite results, as well as the simulation YAML"""
 
-    def __init__(self, *args, exporter_cls=[], **kwargs):
-        exporter_cls = exporter_cls or [YAML, SQLite]
-        self.inner = [cls(*args, **kwargs) for cls in exporter_cls]
-
-    def sim_start(self, *args, **kwargs):
-        for exporter in self.inner:
-            exporter.sim_start(*args, **kwargs)
-
-    def sim_end(self, *args, **kwargs):
-        for exporter in self.inner:
-            exporter.sim_end(*args, **kwargs)
-
-    def iteration_end(self, *args, **kwargs):
-        for exporter in self.inner:
-            exporter.iteration_end(*args, **kwargs)
+default = SQLite
```

### Comparing `soil-1.0.0rc5.post1/soil/network.py` & `soil-1.0.0rc7/soil/network.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/parameters.py` & `soil-1.0.0rc7/soil/parameters.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/serialization.py` & `soil-1.0.0rc7/soil/serialization.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/simulation.py` & `soil-1.0.0rc7/soil/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,16 @@
     finally:
         logger.debug("RUNNING AGAIN")
         _AVOID_RUNNING = False
 
 
 def _iter_queued():
     while _QUEUED:
-        (cls, params) = _QUEUED.pop(0)
-        yield replace(cls, parameters=params)
+        slf = _QUEUED.pop(0)
+        yield slf
 
 
 # TODO: change documentation for simulation
 @dataclass
 class Simulation:
     """
     A simulation is a collection of agents and a model. It is responsible for running the model and agents, and collecting data from them.
@@ -126,19 +126,19 @@
             self.model_reporters = self.model_reporters
             self.tables = self.tables
             self.id = f"{self.name}_{current_time()}"
 
     def run(self, **kwargs):
         """Run the simulation and return the list of resulting environments"""
         if kwargs:
-            return replace(self, **kwargs).run()
+            res = replace(self, **kwargs)
+            return res.run()
 
-        param_combinations = self._collect_params(**kwargs)
         if _AVOID_RUNNING:
-            _QUEUED.extend((self, param) for param in param_combinations)
+            _QUEUED.append(self)
             return []
 
         self.logger.debug("Using exporters: %s", self.exporters or [])
 
         exporters = serialization.deserialize_all(
             self.exporters,
             simulation=self,
@@ -150,14 +150,16 @@
             **self.exporter_params,
         )
 
         results = []
         for exporter in exporters:
             exporter.sim_start()
 
+        param_combinations = self._collect_params(**kwargs)
+
         for params in tqdm(param_combinations, desc=self.name, unit="configuration"):
             for (k, v) in params.items():
                 tqdm.write(f"{k} = {v}")
             sha = hashlib.sha256()
             sha.update(repr(sorted(params.items())).encode())
             params_id = sha.hexdigest()[:7]
             for env in self._run_iters_for_params(params):
@@ -200,14 +202,15 @@
                         return None
                 else:
                     func = self._run_model
 
                 for env in tqdm(utils.run_parallel(
                     func=func,
                     iterable=range(self.iterations),
+                    num_processes=self.num_processes,
                     **params,
                 ), total=self.iterations, leave=False):
                     if env is None and self.dry_run:
                         continue
 
                     yield env
 
@@ -334,20 +337,21 @@
         module = importlib.util.module_from_spec(spec)
         sys.modules[module_name] = module
         spec.loader.exec_module(module)
         for (_name, sim) in inspect.getmembers(module, lambda x: isinstance(x, Simulation)):
             sims.append(sim)
         for sim in _iter_queued():
             sims.append(sim)
+        # Try to find environments to run, because we did not import a script that ran simulations
         if not sims:
             for (_name, env) in inspect.getmembers(module,
-                                                   lambda x: inspect.isclass(x) and
-                                                   issubclass(x, environment.Environment) and
-                                                   (getattr(x, "__module__", None) != environment.__name__)):
-                sims.append(Simulation(model=env, **kwargs))
+                                                lambda x: inspect.isclass(x) and
+                                                issubclass(x, environment.Environment) and
+                                                (getattr(x, "__module__", None) != environment.__name__)):
+                    sims.append(Simulation(model=env, **kwargs))
         del sys.modules[module_name]
     assert not _AVOID_RUNNING
     if not sims:
         raise AttributeError(f"No valid configurations found in {pyfile}")
     if added:
         sys.path.remove(folder)
     for sim in sims:
```

### Comparing `soil-1.0.0rc5.post1/soil/time.py` & `soil-1.0.0rc7/soil/time.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from mesa.time import BaseScheduler
 from queue import Empty
 from heapq import heappush, heappop, heapreplace
-from collections import deque
+from collections import deque, defaultdict
 import math
 import logging
 
 from inspect import getsource
 from numbers import Number
 from textwrap import dedent
+import random as random_std
 
 from .utils import logger
 from mesa import Agent as MesaAgent
 
 
 INFINITY = float("inf")
 
@@ -19,174 +20,285 @@
     """A delay object which can be used both as a return value and as an awaitable (in async code)."""
     __slots__ = ("delta", )
     def __init__(self, delta):
         self.delta = float(delta)
 
     def __float__(self):
         return self.delta
-    
+
+    def __eq__(self, other):
+        return float(self) == float(other)
+
     def __await__(self):
         return (yield self.delta)
 
 class When:
     def __init__(self, when):
         raise Exception("The use of When is deprecated. Use the `Agent.at` and `Agent.delay` methods instead")
+
 class Delta:
     def __init__(self, delta):
         raise Exception("The use of Delay is deprecated. Use the `Agent.at` and `Agent.delay` methods instead")
 
 class DeadAgent(Exception):
     pass
 
 
-class PQueueActivation(BaseScheduler):
+class Event(object):
+    def __init__(self, when: float, func, order=1):
+        self.when = when
+        self.func = func
+        self.order = order
+
+    def __repr__(self):
+        return f'Event @ {self.when} - Func: {self.func}'
+
+    def __lt__(self, other):
+        return (self.when < other.when) or (self.when == other.when and self.order < other.order)
+
+
+class PQueueSchedule:
     """
-    A scheduler which activates each agent with a delay returned by the agent's step method.
+    A scheduler which activates each function with a delay returned by the function at each step.
     If no delay is returned, a default of 1 is used.
-    
-    In each activation, each agent will update its 'next_time'.
     """
 
-    def __init__(self, *args, shuffle=True, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self, shuffle=True, seed=None, **kwargs):
         self._queue = []
         self._shuffle = shuffle
-        self.logger = getattr(self.model, "logger", logger).getChild(f"time_{ self.model }")
+        self.time = 0
+        self.steps = 0
+        self.random = random_std.Random(seed)
         self.next_time = self.time
 
-    def add(self, agent: MesaAgent, when=None):
+    def insert(self, when, callback, replace=False):
         if when is None:
             when = self.time
         else:
             when = float(when)
-
-        self._schedule(agent, None, when)
-        super().add(agent)
-
-    def _schedule(self, agent, when=None, replace=False):
-        if when is None:
-            when = self.time
+        order = 1
         if self._shuffle:
-            key = (when, self.model.random.random())
-        else:
-            key = (when, agent.unique_id)
+            order = self.random.random()
+        event = Event(when, callback, order=order)
         if replace:
-            heapreplace(self._queue, (key, agent))
+            heapreplace(self._queue, event)
         else:
-            heappush(self._queue, (key, agent))
+            heappush(self._queue, event)
+
+    def remove(self, callback):
+        for i, event in enumerate(self._queue):
+            if callback == event.func:
+                del self._queue[i]
+                break
+
+    def __len__(self):
+        return len(self._queue)
 
     def step(self) -> None:
         """
-        Executes agents in order, one at a time. After each step,
-        an agent will signal when it wants to be scheduled next.
+        Executes events in order, one at a time. After each step,
+        an event will signal when it wants to be scheduled next.
         """
 
         if self.time == INFINITY:
             return
 
         next_time = INFINITY
 
         now = self.time
 
         while self._queue:
-            ((when, _id), agent) = self._queue[0]
+            event = self._queue[0]
+            when = event.when
             if when > now:
                 next_time = when
                 break
 
-            try:
-                when = agent.step() or 1
-                when += now
-            except DeadAgent:
-                heappop(self._queue)
-                continue
+            when = event.func() 
+            when = float(when) if when is not None else 1.0
 
             if when == INFINITY:
                 heappop(self._queue)
                 continue
 
-            self._schedule(agent, when, replace=True)
+            when += now
+
+            self.insert(when, event.func, replace=True)
 
         self.steps += 1
 
         self.time = next_time
 
         if next_time == INFINITY:
-            self.model.running = False
             self.time = INFINITY
             return
 
 
-class TimedActivation(BaseScheduler):
-    def __init__(self, *args, shuffle=True, **kwargs):
-        super().__init__(*args, **kwargs)
+class Schedule:
+    def __init__(self, shuffle=True, seed=None, **kwargs):
         self._queue = deque()
         self._shuffle = shuffle
-        self.logger = getattr(self.model, "logger", logger).getChild(f"time_{ self.model }")
+        self.time = 0
+        self.steps = 0
+        self.random = random_std.Random(seed)
         self.next_time = self.time
 
-    def add(self, agent: MesaAgent, when=None):
+    def _find_loc(self, when=None):
         if when is None:
             when = self.time
         else:
             when = float(when)
-        self._schedule(agent, None, when)
-        super().add(agent)
-
-    def _schedule(self, agent, when=None, replace=False):
         when = when or self.time
         pos = len(self._queue)
         for (ix, l) in enumerate(self._queue):
             if l[0] == when:
-                l[1].append(agent)
-                return
+                return l[1]
             if l[0] > when:
                 pos = ix
                 break
-        self._queue.insert(pos, (when, [agent]))
+        lst = []
+        self._queue.insert(pos, (when, lst))
+        return lst
+
+    def insert(self, when, func, replace=False):
+        if when == INFINITY:
+            return
+        lst = self._find_loc(when)
+        lst.append(func)
+    
+    def add_bulk(self, funcs, when=None):
+        lst = self._find_loc(when)
+        n = len(funcs)
+        #TODO: remove for performance
+        before = len(self)
+        lst.extend(funcs)
+        assert len(self) == before + n
+
+    def remove(self, func):
+        for bucket in self._queue:
+            for (ix, e) in enumerate(bucket):
+                if e == func:
+                    bucket.remove(ix)
+                    return
+
+    def __len__(self):
+        return sum(len(bucket[1]) for bucket in self._queue)
 
     def step(self) -> None:
         """
-        Executes agents in order, one at a time. After each step,
-        an agent will signal when it wants to be scheduled next.
+        Executes events in order, one at a time. After each step,
+        an event will signal when it wants to be scheduled next.
         """
         if not self._queue:
             return
 
         now = self.time
 
         next_time = self._queue[0][0]
 
         if next_time > now:
             self.time = next_time
             return
 
         bucket = self._queue.popleft()[1]
         if self._shuffle:
-            self.model.random.shuffle(bucket)
-        for agent in bucket:
-            try:
-                when = agent.step() or 1
-                when += now
-            except DeadAgent:
+            self.random.shuffle(bucket)
+        next_batch = defaultdict(list)
+        for func in bucket:
+            when = func()
+            when = float(when) if when is not None else 1
+
+            if when == INFINITY:
                 continue
 
-            if when != INFINITY:
-                self._schedule(agent, when, replace=True)
+            when += now
+            next_batch[when].append(func) 
+        
+        for (when, bucket) in next_batch.items():
+            self.add_bulk(bucket, when)
 
         self.steps += 1
         if self._queue:
             self.time = self._queue[0][0]
         else:
             self.time = INFINITY
 
 
+class InnerActivation(BaseScheduler):
+    inner_class = Schedule
+
+    def __init__(self, model, shuffle=True, **kwargs):
+        self.model = model
+        self.logger = getattr(self.model, "logger", logger).getChild(f"time_{ self.model }")
+        self._agents = {}
+        self.agents_by_type = defaultdict(dict)
+        self.inner = self.inner_class(shuffle=shuffle, seed=self.model._seed)
+
+    @property
+    def steps(self):
+        return self.inner.steps
+
+    @property
+    def time(self):
+        return self.inner.time
+
+    def add(self, agent: MesaAgent, when=None):
+        when = when or self.inner.time
+        self.inner.insert(when, agent.step)
+        agent_class = type(agent)
+        self.agents_by_type[agent_class][agent.unique_id] = agent
+        super().add(agent)
+    
+    def add_callback(self, when, cb):
+        self.inner.insert(when, cb)
+
+    def remove_callback(self, when, cb):
+        self.inner.remove(cb)
+    
+    def remove(self, agent):
+        del self._agents[agent.unique_id]
+        del self.agents_by_type[type(agent)][agent.unique_id]
+        self.inner.remove(agent.step)
+
+    def step(self) -> None:
+        """
+        Executes agents in order, one at a time. After each step,
+        an agent will signal when it wants to be scheduled next.
+        """
+        self.inner.step()
+
+    def __len__(self):
+        return len(self.inner)
+
+
+class BucketTimedActivation(InnerActivation):
+    inner_class = Schedule
+
+
+class PQueueActivation(InnerActivation):
+    inner_class = PQueueSchedule
+
+
+#Set the bucket implementation as default
+TimedActivation = BucketTimedActivation
+
+try:
+    from soilent.soilent import BucketScheduler, PQueueScheduler
+
+    class SoilentActivation(InnerActivation):
+        inner_class = BucketScheduler
+    class SoilentPQueueActivation(InnerActivation):
+        inner_class = PQueueScheduler
+
+    # TimedActivation = SoilentBucketActivation
+except ImportError:
+    pass
+
+
 class ShuffledTimedActivation(TimedActivation):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, shuffle=True, **kwargs)
 
 
 class OrderedTimedActivation(TimedActivation):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, shuffle=False, **kwargs)
-
-
```

### Comparing `soil-1.0.0rc5.post1/soil/utils.py` & `soil-1.0.0rc7/soil/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,23 +89,20 @@
     if not isinstance(d, dict):
         return d
     return dict(_flatten_dict(d))
 
 
 def _flatten_dict(d, prefix=""):
     if not isinstance(d, dict):
-        # print('END:', prefix, d)
         yield prefix, d
         return
     if prefix:
         prefix = prefix + "."
     for k, v in d.items():
-        # print(k, v)
         res = list(_flatten_dict(v, prefix="{}{}".format(prefix, k)))
-        # print('RES:', res)
         yield from res
 
 
 def unflatten_dict(d):
     out = {}
     for k, v in d.items():
         target = out
@@ -138,14 +135,15 @@
             traceback.format_exception(type(ex), ex, ex.__traceback__)[:]
         )
         return ex
 
 
 def run_parallel(func, iterable, num_processes=1, **kwargs):
     if num_processes > 1 and not os.environ.get("SOIL_DEBUG", None):
+        logger.info("Running simulations in {} processes".format(num_processes))
         if num_processes < 1:
             num_processes = cpu_count() - num_processes
         p = Pool(processes=num_processes)
         wrapped_func = partial(run_and_return_exceptions, func, **kwargs)
         for i in p.imap_unordered(wrapped_func, iterable):
             if isinstance(i, Exception):
                 logger.error("Trial failed:\n\t%s", i.message)
@@ -153,8 +151,28 @@
             yield i
     else:
         for i in iterable:
             yield func(i, **kwargs)
 
 
 def int_seed(seed: str):
-    return int.from_bytes(seed.encode(), "little")
+    return int.from_bytes(seed.encode(), "little")
+
+
+def prob(prob, random):
+    """
+    A true/False uniform distribution with a given probability.
+    To be used like this:
+
+    .. code-block:: python
+
+          if prob(0.3):
+              do_something()
+
+    """
+    r = random.random()
+    return r < prob
+
+
+def custom(cls, **kwargs):
+    """Create a new class from a template class and keyword arguments"""
+    return type(cls.__name__, (cls,), kwargs)
```

### Comparing `soil-1.0.0rc5.post1/soil/web/README.md` & `soil-1.0.0rc7/soil/web/README.md`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/web/__init__.py` & `soil-1.0.0rc7/soil/web/__init__.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/web/config.yml` & `soil-1.0.0rc7/soil/web/config.yml`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/web/run.py` & `soil-1.0.0rc7/soil/web/run.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/web/static/css/main.css` & `soil-1.0.0rc7/soil/web/static/css/main.css`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/web/static/css/timeline.css` & `soil-1.0.0rc7/soil/web/static/css/timeline.css`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/web/static/img/logo_gsi.svg` & `soil-1.0.0rc7/soil/web/static/img/logo_gsi.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/web/static/img/logo_soil.png` & `soil-1.0.0rc7/soil/web/static/img/logo_soil.png`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/web/static/img/svg/person.svg` & `soil-1.0.0rc7/soil/web/static/img/svg/person.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/web/static/img/svg/plus.svg` & `soil-1.0.0rc7/soil/web/static/img/svg/plus.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/web/static/img/svg/target.svg` & `soil-1.0.0rc7/soil/web/static/img/svg/target.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/web/static/img/svg/time.svg` & `soil-1.0.0rc7/soil/web/static/img/svg/time.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/web/static/js/socket.js` & `soil-1.0.0rc7/soil/web/static/js/socket.js`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/web/static/js/template.js` & `soil-1.0.0rc7/soil/web/static/js/template.js`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/web/static/js/timeline.js` & `soil-1.0.0rc7/soil/web/static/js/timeline.js`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/web/static/js/visualization.js` & `soil-1.0.0rc7/soil/web/static/js/visualization.js`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil/web/templates/index.html` & `soil-1.0.0rc7/soil/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/soil.egg-info/PKG-INFO` & `soil-1.0.0rc7/soil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: soil
-Version: 1.0.0rc5.post1
+Version: 1.0.0rc7
 Summary: An Agent-Based Social Simulator for Social Networks
 Home-page: https://github.com/gsi-upm/soil
-Download-URL: https://github.com/gsi-upm/soil/archive/1.0.0rc5.post1.tar.gz
+Download-URL: https://github.com/gsi-upm/soil/archive/1.0.0rc7.tar.gz
 Author: J. Fernando Sanchez
 Author-email: jf.sanchez@upm.es
 Keywords: agent,social,simulator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `soil-1.0.0rc5.post1/soil.egg-info/SOURCES.txt` & `soil-1.0.0rc7/soil.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.cfg
 setup.py
 test-requirements.txt
 soil/.VERSION.~undo-tree~
 soil/.__init__.py.~undo-tree~
 soil/.analysis.py.~undo-tree~
 soil/.datacollection.py.~undo-tree~
+soil/.decorators.py.~undo-tree~
 soil/.environment.py.~undo-tree~
 soil/.events.py.~undo-tree~
 soil/.exporters.py.~undo-tree~
 soil/.serialization.py.~undo-tree~
 soil/.simulation.py.~undo-tree~
 soil/.stats.py.~undo-tree~
 soil/.time.py.~undo-tree~
@@ -42,24 +43,27 @@
 soil.egg-info/dependency_links.txt
 soil.egg-info/entry_points.txt
 soil.egg-info/requires.txt
 soil.egg-info/top_level.txt
 soil/agents/.__init__.py.~undo-tree~
 soil/agents/.evented.py.~undo-tree~
 soil/agents/.fsm.py.~undo-tree~
+soil/agents/.meta.py.~undo-tree~
 soil/agents/.network_agents.py.~undo-tree~
 soil/agents/BassModel.py
 soil/agents/CounterModel.py
 soil/agents/IndependentCascadeModel.py
 soil/agents/SISaModel.py
 soil/agents/__init__.py
 soil/agents/evented.py
 soil/agents/fsm.py
 soil/agents/geo.py
+soil/agents/meta.py
 soil/agents/network_agents.py
+soil/agents/view.py
 soil/web/.gitignore
 soil/web/README.md
 soil/web/__init__.py
 soil/web/__main__.py
 soil/web/config.yml
 soil/web/run.py
 soil/web/static/css/main.css
```

### Comparing `soil-1.0.0rc5.post1/tests/test_agents.py` & `soil-1.0.0rc7/tests/test_agents.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from unittest import TestCase
 import pytest
 
-from soil import agents, environment
+from soil import agents, events, environment
 from soil import time as stime
 
 
 class Dead(agents.FSM):
     @agents.default_state
     @agents.state
     def only(self):
@@ -16,21 +16,22 @@
     def test_die_returns_infinity(self):
         """The last step of a dead agent should return time.INFINITY"""
         d = Dead(unique_id=0, model=environment.Environment())
         ret = d.step()
         assert ret == stime.INFINITY
 
     def test_die_raises_exception(self):
-        """A dead agent should raise an exception if it is stepped after death"""
+        """A dead agent should continue returning INFINITY after death"""
         d = Dead(unique_id=0, model=environment.Environment())
         assert d.alive
         d.step()
         assert not d.alive
-        with pytest.raises(stime.DeadAgent):
-            d.step()
+        when = float(d.step())
+        assert not d.alive
+        assert when == stime.INFINITY
 
     def test_agent_generator(self):
         """
         The step function of an agent could be a generator. In that case, the state of the
         agent will be resumed after every call to step.
         """
         a = 0
@@ -58,55 +59,101 @@
             def root(self):
                 return self.other
 
             @agents.state
             def other(self):
                 self.times_run += 1
 
+        assert MyAgent.other.id == "other"
         e = environment.Environment()
         a = e.add_agent(MyAgent)
         e.step()
         assert a.times_run == 0
         a.step()
         assert a.times_run == 1
         assert a.state_id == MyAgent.other.id
         a.step()
         assert a.times_run == 2
 
+    def test_state_decorator_multiple(self):
+        class MyAgent(agents.FSM):
+            times_run = 0
+
+            @agents.state(default=True)
+            def one(self):
+                return self.two
+
+            @agents.state
+            def two(self):
+                return self.one
+
+        e = environment.Environment()
+        first = e.add_agent(MyAgent, state_id=MyAgent.one)
+        second = e.add_agent(MyAgent, state_id=MyAgent.two)
+        assert first.state_id == MyAgent.one.id
+        assert second.state_id == MyAgent.two.id
+        e.step()
+        assert first.state_id == MyAgent.two.id
+        assert second.state_id == MyAgent.one.id
+
+    def test_state_decorator_multiple_async(self):
+        class MyAgent(agents.FSM):
+            times_run = 0
+
+            @agents.state(default=True)
+            def one(self):
+                yield self.delay(1)
+                return self.two
+
+            @agents.state
+            def two(self):
+                yield self.delay(1)
+                return self.one
+
+        e = environment.Environment()
+        first = e.add_agent(MyAgent, state_id=MyAgent.one)
+        second = e.add_agent(MyAgent, state_id=MyAgent.two)
+        for i in range(2):
+            assert first.state_id == MyAgent.one.id
+            assert second.state_id == MyAgent.two.id
+            e.step()
+        for i in range(2):
+            assert first.state_id == MyAgent.two.id
+            assert second.state_id == MyAgent.one.id
+            e.step()
+
     def test_broadcast(self):
         """
         An agent should be able to broadcast messages to every other agent, AND each receiver should be able
         to process it
         """
 
         class BCast(agents.Evented):
-            pings_received = 0
+            pings_received = []
 
-            def step(self):
-                print(self.model.broadcast)
-                try:
-                    self.model.broadcast("PING")
-                except Exception as ex:
-                    print(ex)
+            async def step(self):
+                self.broadcast("PING")
+                print("PING sent")
                 while True:
-                    self.process_messages()
-                    yield
-
-            def on_receive(self, msg, sender=None):
-                self.pings_received += 1
+                    msgs = await self.received()
+                    self.pings_received += msgs
 
-        e = environment.EventedEnvironment()
+        e = environment.Environment()
 
-        for i in range(10):
+        num_agents = 10
+        for i in range(num_agents):
             e.add_agent(agent_class=BCast)
         e.step()
-        pings_received = lambda: [a.pings_received for a in e.agents]
-        assert sorted(pings_received()) == list(range(1, 11))
+        # Agents are executed in order, so the first agent should have not received any messages
+        pings_received = lambda: [len(a.pings_received) for a in e.agents]
+        assert sorted(pings_received()) == list(range(0, num_agents))
         e.step()
-        assert all(x == 10 for x in pings_received())
+        # After the second step, every agent should have received a broadcast from every other agent
+        received = pings_received()
+        assert all(x == (num_agents - 1) for x in received)
 
     def test_ask_messages(self):
         """
         An agent should be able to ask another agent, and wait for a response.
         """
 
         # There are two agents, they try to send pings
@@ -136,25 +183,24 @@
                         pings.append(self.now)
                         response = yield from target.ask("PING")
                         responses.append(response)
                     else:
                         print("NOT sending ping")
                     print("Checking msgs")
                     # Do not block if we have already received a PING
-                    if not self.process_messages():
-                        yield from self.received()
-                print("done")
-
-            def on_receive(self, msg, sender=None):
-                if msg == "PING":
-                    pongs.append(self.now)
-                    return "PONG"
-                raise Exception("This should never happen")
+                    msgs = yield from self.received()
+                    for ping in msgs:
+                        if ping.payload == "PING":
+                            ping.reply = "PONG"
+                            pongs.append(self.now)
+                        else:
+                            raise Exception("This should never happen")
+
 
-        e = environment.EventedEnvironment(schedule_class=stime.OrderedTimedActivation)
+        e = environment.Environment(schedule_class=stime.OrderedTimedActivation)
         for i in range(2):
             e.add_agent(agent_class=Ping)
         assert e.now == 0
 
         for i in range(5):
             e.step()
             time = i + 1
@@ -368,8 +414,111 @@
         assert a.now == 13
         assert a.my_state == 4
         model.step()
         assert a.now == 16
         assert a.my_state == 5
         model.step()
         assert a.now == 17
-        assert a.my_state == 5
+        assert a.my_state == 5
+    
+    def test_receive(self):
+        '''
+        An agent should be able to receive a message after waiting
+        '''
+        model = environment.Environment()
+        class TestAgent(agents.Agent):
+            sent = False
+            woken = 0
+            def step(self):
+                self.woken += 1
+                return super().step()
+
+            @agents.state(default=True)
+            async def one(self):
+                try:
+                    self.sent = await self.received(timeout=15)
+                    return self.two.at(20)
+                except events.TimedOut:
+                    pass
+            @agents.state
+            def two(self):
+                return self.die()
+
+        a = model.add_agent(TestAgent)
+
+        class Sender(agents.Agent):
+            async def step(self):
+                await self.delay(10)
+                a.tell(1)
+                return stime.INFINITY
+
+        b = model.add_agent(Sender)
+
+        # Start and wait
+        model.step()
+        assert model.now == 10
+        assert a.woken == 1
+        assert not a.sent
+
+        # Sending the message
+        model.step()
+        assert model.now == 10
+        assert a.woken == 1
+        assert not a.sent
+
+        # The receiver callback
+        model.step()
+        assert model.now == 15
+        assert a.woken == 2
+        assert a.sent[0].payload == 1
+
+        # The timeout
+        model.step()
+        assert model.now == 20
+        assert a.woken == 2
+
+        # The last state of the agent
+        model.step()
+        assert a.woken == 3
+        assert model.now == float('inf')
+
+    def test_receive_timeout(self):
+        '''
+        A timeout should be raised if no messages are received after an expiration time
+        '''
+        model = environment.Environment()
+        timedout = False
+        class TestAgent(agents.Agent):
+            @agents.state(default=True)
+            def one(self):
+                try:
+                    yield from self.received(timeout=10)
+                    raise AssertionError('Should have raised an error.')
+                except events.TimedOut:
+                    nonlocal timedout
+                    timedout = True
+
+        a = model.add_agent(TestAgent)
+
+        model.step()
+        assert model.now == 10
+        model.step()
+        # Wake up the callback
+        assert model.now == 10
+        assert not timedout
+        # The actual timeout
+        model.step()
+        assert model.now == 11
+        assert timedout
+
+    def test_attributes(self):
+        """Attributes should be individual per agent"""
+
+        class MyAgent(agents.Agent):
+            my_attribute = 0
+        
+        model = environment.Environment()
+        a = MyAgent(model=model)
+        assert a.my_attribute == 0
+        b = MyAgent(model=model, my_attribute=1)
+        assert b.my_attribute == 1
+        assert a.my_attribute == 0
```

### Comparing `soil-1.0.0rc5.post1/tests/test_config.py` & `soil-1.0.0rc7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/tests/test_examples.py` & `soil-1.0.0rc7/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/tests/test_exporters.py` & `soil-1.0.0rc7/tests/test_exporters.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,16 @@
             def constant(self):
                 return 1
 
         s = simulation.Simulation(
             model=ConstantEnv,
             name="exporter_sim",
             exporters=[
-                exporters.default,
+                exporters.YAML,
+                exporters.SQLite,
                 exporters.csv,
             ],
             exporter_params={"copy_to": output},
             parameters=dict(
                 network_generator="complete_graph",
                 network_params={"n": n_nodes},
                 agent_class=agents.CounterModel,
```

### Comparing `soil-1.0.0rc5.post1/tests/test_ipython.py` & `soil-1.0.0rc7/tests/test_ipython.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/tests/test_main.py` & `soil-1.0.0rc7/tests/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 import pickle
 import networkx as nx
 from functools import partial
 
 from os.path import join
-from soil import simulation, Environment, agents, network, serialization, utils, config, from_file
+from soil import simulation, Environment, agents, serialization, from_file, time
 from mesa import Agent as MesaAgent
 
 ROOT = os.path.abspath(os.path.dirname(__file__))
 EXAMPLES = join(ROOT, "..", "examples")
 
 
 class CustomAgent(agents.FSM, agents.NetworkAgent):
@@ -131,17 +131,17 @@
             ser, name = serialization.serialize(i)
             assert type(ser) == str
             des = serialization.deserialize(name, ser)
             assert i == des
 
     def test_serialize_agent_class(self):
         """A class from soil.agents should be serialized without the module part"""
-        ser = agents._serialize_type(CustomAgent)
+        ser = serialization.serialize(CustomAgent, known_modules=["soil.agents"])[1]
         assert ser == "test_main.CustomAgent"
-        ser = agents._serialize_type(agents.BaseAgent)
+        ser = serialization.serialize(agents.BaseAgent, known_modules=["soil.agents"])[1]
         assert ser == "BaseAgent"
         pickle.dumps(ser)
 
     def test_until(self):
         n_runs = 0
 
         class CheckRun(agents.BaseAgent):
@@ -190,15 +190,15 @@
                 return self.pong.delay(2)
 
             @agents.state
             def pong(self):
                 return self.ping
 
         a = ToggleAgent(unique_id=1, model=Environment())
-        when = a.step()
+        when = float(a.step())
         assert when == 2
         when = a.step()
         assert when == None
 
     def test_load_sim(self):
         """Make sure at least one of the examples can be loaded"""
         sims = from_file(os.path.join(EXAMPLES, "newsspread", "newsspread_sim.py"))
@@ -248,8 +248,38 @@
         assert "base" in df.columns
         assert "subclass" in df.columns
         assert df["now"][(0,0)] == 1
         assert df["now"][(0,1)] == 1
         assert df["base"][(0,0)] == "base"
         assert df["base"][(0,1)] == "base"
         assert df["subclass"][(0,0)] is None
-        assert df["subclass"][(0,1)] == "subclass"
+        assert df["subclass"][(0,1)] == "subclass"
+    
+    def test_remove_agent(self):
+        """An agent that is scheduled should be removed from the schedule"""
+        model = Environment()
+        model.add_agent(agents.Noop)
+        model.step()
+        model.remove_agent(model.agents[0])
+        assert not model.agents
+        when = model.step()
+        assert when == None
+        assert not model.running
+
+    def test_remove_agent(self):
+        """An agent that is scheduled should be removed from the schedule"""
+
+        allagents = []
+        class Removed(agents.BaseAgent):
+            def step(self):
+                nonlocal allagents
+                assert self.alive
+                assert self in self.model.agents
+                for agent in allagents:
+                    self.model.remove_agent(agent)
+
+        model = Environment()
+        a1 = model.add_agent(Removed)
+        a2 = model.add_agent(Removed)
+        allagents = [a1, a2]
+        model.step()
+        assert not model.agents
```

### Comparing `soil-1.0.0rc5.post1/tests/test_mesa.py` & `soil-1.0.0rc7/tests/test_mesa.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/tests/test_network.py` & `soil-1.0.0rc7/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5.post1/tests/test_time.py` & `soil-1.0.0rc7/tests/test_time.py`

 * *Files identical despite different names*

