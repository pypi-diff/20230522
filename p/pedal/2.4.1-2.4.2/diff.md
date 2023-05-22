# Comparing `tmp/pedal-2.4.1.tar.gz` & `tmp/pedal-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedal-2.4.1.tar", last modified: Mon May 22 16:09:08 2023, max compression
+gzip compressed data, was "pedal-2.4.2.tar", last modified: Mon May 22 16:55:56 2023, max compression
```

## Comparing `pedal-2.4.1.tar` & `pedal-2.4.2.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.968699 pedal-2.4.1/
--rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:21.000000 pedal-2.4.1/LICENSE
--rw-rw-rw-   0        0        0     2981 2023-05-22 16:09:08.968699 pedal-2.4.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.792698 pedal-2.4.1/Pedal.egg-info/
--rw-rw-rw-   0        0        0     2981 2023-05-22 16:09:08.000000 pedal-2.4.1/Pedal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3702 2023-05-22 16:09:08.000000 pedal-2.4.1/Pedal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:09:08.000000 pedal-2.4.1/Pedal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-22 16:09:08.000000 pedal-2.4.1/Pedal.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 16:09:08.000000 pedal-2.4.1/Pedal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-22 16:09:08.000000 pedal-2.4.1/Pedal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1958 2023-05-18 18:40:27.000000 pedal-2.4.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.789699 pedal-2.4.1/pedal/
--rw-rw-rw-   0        0        0      382 2023-05-18 18:14:23.000000 pedal-2.4.1/pedal/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.807700 pedal-2.4.1/pedal/assertions/
--rw-rw-rw-   0        0        0      549 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/assertions/__init__.py
--rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:31.000000 pedal-2.4.1/pedal/assertions/classes.py
--rw-rw-rw-   0        0        0    13288 2023-01-17 17:53:58.000000 pedal-2.4.1/pedal/assertions/commands.py
--rw-rw-rw-   0        0        0       73 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/assertions/constants.py
--rw-rw-rw-   0        0        0    20378 2022-09-17 21:23:34.000000 pedal-2.4.1/pedal/assertions/feedbacks.py
--rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:04.000000 pedal-2.4.1/pedal/assertions/functions.py
--rw-rw-rw-   0        0        0     5722 2021-01-26 15:12:38.000000 pedal-2.4.1/pedal/assertions/organizers.py
--rw-rw-rw-   0        0        0    33479 2023-01-17 17:50:34.000000 pedal-2.4.1/pedal/assertions/runtime.py
--rw-rw-rw-   0        0        0     3254 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/assertions/setup.py
--rw-rw-rw-   0        0        0    30229 2022-11-17 14:15:37.000000 pedal-2.4.1/pedal/assertions/static.py
--rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/assertions/unittest.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.817699 pedal-2.4.1/pedal/cait/
--rw-rw-rw-   0        0        0      445 2020-10-17 20:34:56.000000 pedal-2.4.1/pedal/cait/__init__.py
--rw-rw-rw-   0        0        0     2254 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/cait/ast_helpers.py
--rw-rw-rw-   0        0        0    11371 2021-03-12 21:12:46.000000 pedal-2.4.1/pedal/cait/ast_map.py
--rw-rw-rw-   0        0        0    10523 2021-01-08 04:00:46.000000 pedal-2.4.1/pedal/cait/cait_api.py
--rw-rw-rw-   0        0        0    22471 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/cait/cait_node.py
--rw-rw-rw-   0        0        0       59 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/cait/constants.py
--rw-rw-rw-   0        0        0     4693 2021-06-28 19:26:48.000000 pedal-2.4.1/pedal/cait/find_node.py
--rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:46.000000 pedal-2.4.1/pedal/cait/stretchy_tree_matching.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.827700 pedal-2.4.1/pedal/command_line/
--rw-rw-rw-   0        0        0       94 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/command_line/__init__.py
--rw-rw-rw-   0        0        0     7897 2022-04-30 18:25:37.000000 pedal-2.4.1/pedal/command_line/command_line.py
--rw-rw-rw-   0        0        0     7493 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/command_line/mocks.py
--rw-rw-rw-   0        0        0    25271 2022-11-11 18:14:58.000000 pedal-2.4.1/pedal/command_line/modes.py
--rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:52.000000 pedal-2.4.1/pedal/command_line/report.py
--rw-rw-rw-   0        0        0     3540 2020-11-08 16:28:36.000000 pedal-2.4.1/pedal/command_line/verify.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.852698 pedal-2.4.1/pedal/core/
--rw-rw-rw-   0        0        0      107 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/core/__init__.py
--rw-rw-rw-   0        0        0     8756 2022-11-11 16:40:07.000000 pedal-2.4.1/pedal/core/commands.py
--rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/core/environment.py
--rw-rw-rw-   0        0        0      707 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/core/errors.py
--rw-rw-rw-   0        0        0    20881 2023-01-17 17:46:13.000000 pedal-2.4.1/pedal/core/feedback.py
--rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/core/feedback_category.py
--rw-rw-rw-   0        0        0     6107 2022-11-17 14:35:13.000000 pedal-2.4.1/pedal/core/final_feedback.py
--rw-rw-rw-   0        0        0     7639 2023-01-17 17:14:11.000000 pedal-2.4.1/pedal/core/formatting.py
--rw-rw-rw-   0        0        0     1915 2022-06-12 19:44:51.000000 pedal-2.4.1/pedal/core/location.py
--rw-rw-rw-   0        0        0    13385 2022-11-28 05:44:51.000000 pedal-2.4.1/pedal/core/report.py
--rw-rw-rw-   0        0        0      822 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/core/resolver.py
--rw-rw-rw-   0        0        0     3985 2022-11-17 14:35:11.000000 pedal-2.4.1/pedal/core/scoring.py
--rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:08.000000 pedal-2.4.1/pedal/core/submission.py
--rw-rw-rw-   0        0        0      405 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/core/tag.py
--rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:35.000000 pedal-2.4.1/pedal/core/tool.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.865698 pedal-2.4.1/pedal/environments/
--rw-rw-rw-   0        0        0      657 2020-11-08 17:16:23.000000 pedal-2.4.1/pedal/environments/__init__.py
--rw-rw-rw-   0        0        0     3042 2021-02-26 19:18:08.000000 pedal-2.4.1/pedal/environments/blockpy.py
--rw-rw-rw-   0        0        0     9569 2022-11-23 18:26:45.000000 pedal-2.4.1/pedal/environments/gradescope.py
--rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:49.000000 pedal-2.4.1/pedal/environments/jupyter.py
--rw-rw-rw-   0        0        0    10351 2021-02-02 16:30:22.000000 pedal-2.4.1/pedal/environments/nbgrader.py
--rw-rw-rw-   0        0        0      368 2020-11-08 17:19:12.000000 pedal-2.4.1/pedal/environments/none.py
--rw-rw-rw-   0        0        0      766 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/environments/sandbox.py
--rw-rw-rw-   0        0        0     3651 2023-04-19 22:17:37.000000 pedal-2.4.1/pedal/environments/standard.py
--rw-rw-rw-   0        0        0     6259 2020-11-13 04:58:08.000000 pedal-2.4.1/pedal/environments/vpl.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.870699 pedal-2.4.1/pedal/extensions/
--rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/extensions/__init__.py
--rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:33.000000 pedal-2.4.1/pedal/extensions/microbit.py
--rw-rw-rw-   0        0        0    11604 2022-11-26 00:03:07.000000 pedal-2.4.1/pedal/extensions/plotting.py
--rw-rw-rw-   0        0        0       81 2022-07-17 15:14:06.000000 pedal-2.4.1/pedal/extensions/turtles.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.885698 pedal-2.4.1/pedal/questions/
--rw-rw-rw-   0        0        0      669 2021-12-05 16:49:53.000000 pedal-2.4.1/pedal/questions/__init__.py
--rw-rw-rw-   0        0        0       66 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/questions/constants.py
--rw-rw-rw-   0        0        0      624 2021-09-15 19:16:10.000000 pedal-2.4.1/pedal/questions/feedbacks.py
--rw-rw-rw-   0        0        0     6045 2022-11-16 17:32:45.000000 pedal-2.4.1/pedal/questions/graders.py
--rw-rw-rw-   0        0        0     3477 2021-12-05 16:42:01.000000 pedal-2.4.1/pedal/questions/loader.py
--rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:25.000000 pedal-2.4.1/pedal/questions/pool.py
--rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:15.000000 pedal-2.4.1/pedal/questions/questions.py
--rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:28.000000 pedal-2.4.1/pedal/questions/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.895699 pedal-2.4.1/pedal/resolvers/
--rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:56.000000 pedal-2.4.1/pedal/resolvers/__init__.py
--rw-rw-rw-   0        0        0      654 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/resolvers/core.py
--rw-rw-rw-   0        0        0     2099 2023-05-13 15:07:02.000000 pedal-2.4.1/pedal/resolvers/full.py
--rw-rw-rw-   0        0        0     1886 2022-11-23 18:27:16.000000 pedal-2.4.1/pedal/resolvers/sectional.py
--rw-rw-rw-   0        0        0      268 2021-01-26 15:52:26.000000 pedal-2.4.1/pedal/resolvers/silent.py
--rw-rw-rw-   0        0        0     5119 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/resolvers/simple.py
--rw-rw-rw-   0        0        0     1176 2020-11-03 17:24:20.000000 pedal-2.4.1/pedal/resolvers/statistics.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.908699 pedal-2.4.1/pedal/sandbox/
--rw-rw-rw-   0        0        0      662 2023-05-13 15:07:02.000000 pedal-2.4.1/pedal/sandbox/__init__.py
--rw-rw-rw-   0        0        0    17919 2023-05-18 18:30:27.000000 pedal-2.4.1/pedal/sandbox/commands.py
--rw-rw-rw-   0        0        0       72 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/sandbox/constants.py
--rw-rw-rw-   0        0        0     9652 2023-05-13 15:13:44.000000 pedal-2.4.1/pedal/sandbox/data.py
--rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:18.000000 pedal-2.4.1/pedal/sandbox/exceptions.py
--rw-rw-rw-   0        0        0    10750 2022-10-04 22:22:33.000000 pedal-2.4.1/pedal/sandbox/feedbacks.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.914699 pedal-2.4.1/pedal/sandbox/library/
--rw-rw-rw-   0        0        0      222 2022-07-17 15:26:46.000000 pedal-2.4.1/pedal/sandbox/library/__init__.py
--rw-rw-rw-   0        0        0     5028 2022-08-18 18:00:00.000000 pedal-2.4.1/pedal/sandbox/library/designer.py
--rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:41.000000 pedal-2.4.1/pedal/sandbox/library/matplotlib.py
--rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:51.000000 pedal-2.4.1/pedal/sandbox/library/microbit.py
--rw-rw-rw-   0        0        0     3400 2022-07-28 21:17:36.000000 pedal-2.4.1/pedal/sandbox/library/turtles.py
--rw-rw-rw-   0        0        0    10124 2023-05-22 15:55:11.000000 pedal-2.4.1/pedal/sandbox/mocked.py
--rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:23.000000 pedal-2.4.1/pedal/sandbox/result.py
--rw-rw-rw-   0        0        0    38840 2023-05-22 14:40:28.000000 pedal-2.4.1/pedal/sandbox/sandbox.py
--rw-rw-rw-   0        0        0     5048 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/sandbox/timeout.py
--rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:49.000000 pedal-2.4.1/pedal/sandbox/tracer.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.922698 pedal-2.4.1/pedal/source/
--rw-rw-rw-   0        0        0      912 2022-07-24 20:13:29.000000 pedal-2.4.1/pedal/source/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/source/constants.py
--rw-rw-rw-   0        0        0     5345 2022-10-04 00:04:29.000000 pedal-2.4.1/pedal/source/feedbacks.py
--rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/source/sections.py
--rw-rw-rw-   0        0        0     7441 2022-11-23 18:29:38.000000 pedal-2.4.1/pedal/source/source.py
--rw-rw-rw-   0        0        0      484 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/source/substitutions.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.936699 pedal-2.4.1/pedal/tifa/
--rw-rw-rw-   0        0        0     3049 2022-11-28 05:46:58.000000 pedal-2.4.1/pedal/tifa/__init__.py
--rw-rw-rw-   0        0        0     2143 2022-10-06 14:36:45.000000 pedal-2.4.1/pedal/tifa/commands.py
--rw-rw-rw-   0        0        0       91 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/tifa/constants.py
--rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:35.000000 pedal-2.4.1/pedal/tifa/contexts.py
--rw-rw-rw-   0        0        0    23536 2022-09-09 22:57:22.000000 pedal-2.4.1/pedal/tifa/feedbacks.py
--rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/tifa/identifier.py
--rw-rw-rw-   0        0        0      908 2022-06-07 19:06:45.000000 pedal-2.4.1/pedal/tifa/settings.py
--rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:15.000000 pedal-2.4.1/pedal/tifa/state.py
--rw-rw-rw-   0        0        0    24173 2022-10-07 14:11:04.000000 pedal-2.4.1/pedal/tifa/tifa_core.py
--rw-rw-rw-   0        0        0    42481 2022-09-22 03:35:00.000000 pedal-2.4.1/pedal/tifa/tifa_visitor.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.943699 pedal-2.4.1/pedal/types/
--rw-rw-rw-   0        0        0       86 2022-06-09 18:41:53.000000 pedal-2.4.1/pedal/types/__init__.py
--rw-rw-rw-   0        0        0     9115 2022-11-28 06:00:50.000000 pedal-2.4.1/pedal/types/builtin.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.951699 pedal-2.4.1/pedal/types/library/
--rw-rw-rw-   0        0        0      192 2022-07-26 18:00:27.000000 pedal-2.4.1/pedal/types/library/__init__.py
--rw-rw-rw-   0        0        0      792 2022-11-28 05:46:58.000000 pedal-2.4.1/pedal/types/library/cs1_curriculum.py
--rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:16.000000 pedal-2.4.1/pedal/types/library/designer.py
--rw-rw-rw-   0        0        0      792 2022-11-28 05:51:17.000000 pedal-2.4.1/pedal/types/library/matplotlib.py
--rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:25.000000 pedal-2.4.1/pedal/types/library/microbit.py
--rw-rw-rw-   0        0        0      441 2022-11-28 05:52:06.000000 pedal-2.4.1/pedal/types/library/turtles.py
--rw-rw-rw-   0        0        0    51752 2022-11-28 05:43:22.000000 pedal-2.4.1/pedal/types/new_types.py
--rw-rw-rw-   0        0        0    14813 2022-11-23 18:45:05.000000 pedal-2.4.1/pedal/types/normalize.py
--rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:52.000000 pedal-2.4.1/pedal/types/operations.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.967700 pedal-2.4.1/pedal/utilities/
--rw-rw-rw-   0        0        0      524 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/utilities/__init__.py
--rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:01.000000 pedal-2.4.1/pedal/utilities/ast_tools.py
--rw-rw-rw-   0        0        0     6580 2022-07-27 17:31:05.000000 pedal-2.4.1/pedal/utilities/comparisons.py
--rw-rw-rw-   0        0        0      679 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/utilities/dictionaries.py
--rw-rw-rw-   0        0        0     8300 2022-09-23 12:51:56.000000 pedal-2.4.1/pedal/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:41.000000 pedal-2.4.1/pedal/utilities/files.py
--rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/utilities/operators.py
--rw-rw-rw-   0        0        0     7037 2022-12-31 17:53:00.000000 pedal-2.4.1/pedal/utilities/progsnap.py
--rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/utilities/sorting.py
--rw-rw-rw-   0        0        0      326 2021-06-28 19:25:31.000000 pedal-2.4.1/pedal/utilities/system.py
--rw-rw-rw-   0        0        0     2313 2022-07-27 16:49:13.000000 pedal-2.4.1/pedal/utilities/text.py
--rw-rw-rw-   0        0        0      769 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/utilities/types.py
--rw-rw-rw-   0        0        0      121 2023-05-22 16:09:08.969699 pedal-2.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1196 2023-05-22 16:08:32.000000 pedal-2.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.905905 pedal-2.4.2/
+-rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:21.000000 pedal-2.4.2/LICENSE
+-rw-rw-rw-   0        0        0     2981 2023-05-22 16:55:56.905905 pedal-2.4.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.777901 pedal-2.4.2/Pedal.egg-info/
+-rw-rw-rw-   0        0        0     2981 2023-05-22 16:55:56.000000 pedal-2.4.2/Pedal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3702 2023-05-22 16:55:56.000000 pedal-2.4.2/Pedal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 16:55:56.000000 pedal-2.4.2/Pedal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-22 16:55:56.000000 pedal-2.4.2/Pedal.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 16:55:56.000000 pedal-2.4.2/Pedal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-22 16:55:56.000000 pedal-2.4.2/Pedal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1958 2023-05-18 18:40:27.000000 pedal-2.4.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.774889 pedal-2.4.2/pedal/
+-rw-rw-rw-   0        0        0      382 2023-05-18 18:14:23.000000 pedal-2.4.2/pedal/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.788890 pedal-2.4.2/pedal/assertions/
+-rw-rw-rw-   0        0        0      549 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/assertions/__init__.py
+-rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:31.000000 pedal-2.4.2/pedal/assertions/classes.py
+-rw-rw-rw-   0        0        0    13288 2023-01-17 17:53:58.000000 pedal-2.4.2/pedal/assertions/commands.py
+-rw-rw-rw-   0        0        0       73 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/assertions/constants.py
+-rw-rw-rw-   0        0        0    20378 2022-09-17 21:23:34.000000 pedal-2.4.2/pedal/assertions/feedbacks.py
+-rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:04.000000 pedal-2.4.2/pedal/assertions/functions.py
+-rw-rw-rw-   0        0        0     5722 2021-01-26 15:12:38.000000 pedal-2.4.2/pedal/assertions/organizers.py
+-rw-rw-rw-   0        0        0    33479 2023-01-17 17:50:34.000000 pedal-2.4.2/pedal/assertions/runtime.py
+-rw-rw-rw-   0        0        0     3254 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/assertions/setup.py
+-rw-rw-rw-   0        0        0    30229 2022-11-17 14:15:37.000000 pedal-2.4.2/pedal/assertions/static.py
+-rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/assertions/unittest.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.797891 pedal-2.4.2/pedal/cait/
+-rw-rw-rw-   0        0        0      445 2020-10-17 20:34:56.000000 pedal-2.4.2/pedal/cait/__init__.py
+-rw-rw-rw-   0        0        0     2254 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/cait/ast_helpers.py
+-rw-rw-rw-   0        0        0    11371 2021-03-12 21:12:46.000000 pedal-2.4.2/pedal/cait/ast_map.py
+-rw-rw-rw-   0        0        0    10523 2021-01-08 04:00:46.000000 pedal-2.4.2/pedal/cait/cait_api.py
+-rw-rw-rw-   0        0        0    22471 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/cait/cait_node.py
+-rw-rw-rw-   0        0        0       59 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/cait/constants.py
+-rw-rw-rw-   0        0        0     4693 2021-06-28 19:26:48.000000 pedal-2.4.2/pedal/cait/find_node.py
+-rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:46.000000 pedal-2.4.2/pedal/cait/stretchy_tree_matching.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.803891 pedal-2.4.2/pedal/command_line/
+-rw-rw-rw-   0        0        0       94 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/command_line/__init__.py
+-rw-rw-rw-   0        0        0     7897 2022-04-30 18:25:37.000000 pedal-2.4.2/pedal/command_line/command_line.py
+-rw-rw-rw-   0        0        0     7493 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/command_line/mocks.py
+-rw-rw-rw-   0        0        0    25271 2022-11-11 18:14:58.000000 pedal-2.4.2/pedal/command_line/modes.py
+-rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:52.000000 pedal-2.4.2/pedal/command_line/report.py
+-rw-rw-rw-   0        0        0     3540 2020-11-08 16:28:36.000000 pedal-2.4.2/pedal/command_line/verify.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.818888 pedal-2.4.2/pedal/core/
+-rw-rw-rw-   0        0        0      107 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/core/__init__.py
+-rw-rw-rw-   0        0        0     9298 2023-05-22 16:32:35.000000 pedal-2.4.2/pedal/core/commands.py
+-rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/core/environment.py
+-rw-rw-rw-   0        0        0      707 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/core/errors.py
+-rw-rw-rw-   0        0        0    20881 2023-01-17 17:46:13.000000 pedal-2.4.2/pedal/core/feedback.py
+-rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/core/feedback_category.py
+-rw-rw-rw-   0        0        0     6107 2022-11-17 14:35:13.000000 pedal-2.4.2/pedal/core/final_feedback.py
+-rw-rw-rw-   0        0        0     7639 2023-01-17 17:14:11.000000 pedal-2.4.2/pedal/core/formatting.py
+-rw-rw-rw-   0        0        0     1915 2022-06-12 19:44:51.000000 pedal-2.4.2/pedal/core/location.py
+-rw-rw-rw-   0        0        0    13385 2022-11-28 05:44:51.000000 pedal-2.4.2/pedal/core/report.py
+-rw-rw-rw-   0        0        0      822 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/core/resolver.py
+-rw-rw-rw-   0        0        0     3985 2022-11-17 14:35:11.000000 pedal-2.4.2/pedal/core/scoring.py
+-rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:08.000000 pedal-2.4.2/pedal/core/submission.py
+-rw-rw-rw-   0        0        0      405 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/core/tag.py
+-rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:35.000000 pedal-2.4.2/pedal/core/tool.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.827887 pedal-2.4.2/pedal/environments/
+-rw-rw-rw-   0        0        0      657 2020-11-08 17:16:23.000000 pedal-2.4.2/pedal/environments/__init__.py
+-rw-rw-rw-   0        0        0     3042 2021-02-26 19:18:08.000000 pedal-2.4.2/pedal/environments/blockpy.py
+-rw-rw-rw-   0        0        0     9569 2022-11-23 18:26:45.000000 pedal-2.4.2/pedal/environments/gradescope.py
+-rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:49.000000 pedal-2.4.2/pedal/environments/jupyter.py
+-rw-rw-rw-   0        0        0    10351 2021-02-02 16:30:22.000000 pedal-2.4.2/pedal/environments/nbgrader.py
+-rw-rw-rw-   0        0        0      368 2020-11-08 17:19:12.000000 pedal-2.4.2/pedal/environments/none.py
+-rw-rw-rw-   0        0        0      766 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/environments/sandbox.py
+-rw-rw-rw-   0        0        0     3651 2023-04-19 22:17:37.000000 pedal-2.4.2/pedal/environments/standard.py
+-rw-rw-rw-   0        0        0     6259 2020-11-13 04:58:08.000000 pedal-2.4.2/pedal/environments/vpl.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.831887 pedal-2.4.2/pedal/extensions/
+-rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/extensions/__init__.py
+-rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:33.000000 pedal-2.4.2/pedal/extensions/microbit.py
+-rw-rw-rw-   0        0        0    11604 2022-11-26 00:03:07.000000 pedal-2.4.2/pedal/extensions/plotting.py
+-rw-rw-rw-   0        0        0       81 2022-07-17 15:14:06.000000 pedal-2.4.2/pedal/extensions/turtles.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.841892 pedal-2.4.2/pedal/questions/
+-rw-rw-rw-   0        0        0      669 2021-12-05 16:49:53.000000 pedal-2.4.2/pedal/questions/__init__.py
+-rw-rw-rw-   0        0        0       66 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/questions/constants.py
+-rw-rw-rw-   0        0        0      624 2021-09-15 19:16:10.000000 pedal-2.4.2/pedal/questions/feedbacks.py
+-rw-rw-rw-   0        0        0     6045 2022-11-16 17:32:45.000000 pedal-2.4.2/pedal/questions/graders.py
+-rw-rw-rw-   0        0        0     3477 2021-12-05 16:42:01.000000 pedal-2.4.2/pedal/questions/loader.py
+-rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:25.000000 pedal-2.4.2/pedal/questions/pool.py
+-rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:15.000000 pedal-2.4.2/pedal/questions/questions.py
+-rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:28.000000 pedal-2.4.2/pedal/questions/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.849889 pedal-2.4.2/pedal/resolvers/
+-rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:56.000000 pedal-2.4.2/pedal/resolvers/__init__.py
+-rw-rw-rw-   0        0        0      654 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/resolvers/core.py
+-rw-rw-rw-   0        0        0     2099 2023-05-13 15:07:02.000000 pedal-2.4.2/pedal/resolvers/full.py
+-rw-rw-rw-   0        0        0     1886 2022-11-23 18:27:16.000000 pedal-2.4.2/pedal/resolvers/sectional.py
+-rw-rw-rw-   0        0        0      268 2021-01-26 15:52:26.000000 pedal-2.4.2/pedal/resolvers/silent.py
+-rw-rw-rw-   0        0        0     5119 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/resolvers/simple.py
+-rw-rw-rw-   0        0        0     1176 2020-11-03 17:24:20.000000 pedal-2.4.2/pedal/resolvers/statistics.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.859906 pedal-2.4.2/pedal/sandbox/
+-rw-rw-rw-   0        0        0      662 2023-05-13 15:07:02.000000 pedal-2.4.2/pedal/sandbox/__init__.py
+-rw-rw-rw-   0        0        0    17919 2023-05-18 18:30:27.000000 pedal-2.4.2/pedal/sandbox/commands.py
+-rw-rw-rw-   0        0        0       72 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/sandbox/constants.py
+-rw-rw-rw-   0        0        0     9652 2023-05-13 15:13:44.000000 pedal-2.4.2/pedal/sandbox/data.py
+-rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:18.000000 pedal-2.4.2/pedal/sandbox/exceptions.py
+-rw-rw-rw-   0        0        0    10750 2022-10-04 22:22:33.000000 pedal-2.4.2/pedal/sandbox/feedbacks.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.864905 pedal-2.4.2/pedal/sandbox/library/
+-rw-rw-rw-   0        0        0      222 2022-07-17 15:26:46.000000 pedal-2.4.2/pedal/sandbox/library/__init__.py
+-rw-rw-rw-   0        0        0     5028 2022-08-18 18:00:00.000000 pedal-2.4.2/pedal/sandbox/library/designer.py
+-rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:41.000000 pedal-2.4.2/pedal/sandbox/library/matplotlib.py
+-rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:51.000000 pedal-2.4.2/pedal/sandbox/library/microbit.py
+-rw-rw-rw-   0        0        0     3400 2022-07-28 21:17:36.000000 pedal-2.4.2/pedal/sandbox/library/turtles.py
+-rw-rw-rw-   0        0        0    10124 2023-05-22 15:55:11.000000 pedal-2.4.2/pedal/sandbox/mocked.py
+-rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:23.000000 pedal-2.4.2/pedal/sandbox/result.py
+-rw-rw-rw-   0        0        0    38840 2023-05-22 14:40:28.000000 pedal-2.4.2/pedal/sandbox/sandbox.py
+-rw-rw-rw-   0        0        0     5048 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/sandbox/timeout.py
+-rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:49.000000 pedal-2.4.2/pedal/sandbox/tracer.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.870905 pedal-2.4.2/pedal/source/
+-rw-rw-rw-   0        0        0      912 2022-07-24 20:13:29.000000 pedal-2.4.2/pedal/source/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/source/constants.py
+-rw-rw-rw-   0        0        0     5345 2022-10-04 00:04:29.000000 pedal-2.4.2/pedal/source/feedbacks.py
+-rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/source/sections.py
+-rw-rw-rw-   0        0        0     7441 2022-11-23 18:29:38.000000 pedal-2.4.2/pedal/source/source.py
+-rw-rw-rw-   0        0        0      484 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/source/substitutions.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.880906 pedal-2.4.2/pedal/tifa/
+-rw-rw-rw-   0        0        0     3049 2022-11-28 05:46:58.000000 pedal-2.4.2/pedal/tifa/__init__.py
+-rw-rw-rw-   0        0        0     2143 2022-10-06 14:36:45.000000 pedal-2.4.2/pedal/tifa/commands.py
+-rw-rw-rw-   0        0        0       91 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/tifa/constants.py
+-rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:35.000000 pedal-2.4.2/pedal/tifa/contexts.py
+-rw-rw-rw-   0        0        0    23656 2023-05-22 16:40:08.000000 pedal-2.4.2/pedal/tifa/feedbacks.py
+-rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/tifa/identifier.py
+-rw-rw-rw-   0        0        0      908 2022-06-07 19:06:45.000000 pedal-2.4.2/pedal/tifa/settings.py
+-rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:15.000000 pedal-2.4.2/pedal/tifa/state.py
+-rw-rw-rw-   0        0        0    24173 2022-10-07 14:11:04.000000 pedal-2.4.2/pedal/tifa/tifa_core.py
+-rw-rw-rw-   0        0        0    42489 2023-05-22 16:39:10.000000 pedal-2.4.2/pedal/tifa/tifa_visitor.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.885906 pedal-2.4.2/pedal/types/
+-rw-rw-rw-   0        0        0       86 2022-06-09 18:41:53.000000 pedal-2.4.2/pedal/types/__init__.py
+-rw-rw-rw-   0        0        0     9115 2022-11-28 06:00:50.000000 pedal-2.4.2/pedal/types/builtin.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.892906 pedal-2.4.2/pedal/types/library/
+-rw-rw-rw-   0        0        0      192 2022-07-26 18:00:27.000000 pedal-2.4.2/pedal/types/library/__init__.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:46:58.000000 pedal-2.4.2/pedal/types/library/cs1_curriculum.py
+-rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:16.000000 pedal-2.4.2/pedal/types/library/designer.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:51:17.000000 pedal-2.4.2/pedal/types/library/matplotlib.py
+-rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:25.000000 pedal-2.4.2/pedal/types/library/microbit.py
+-rw-rw-rw-   0        0        0      441 2022-11-28 05:52:06.000000 pedal-2.4.2/pedal/types/library/turtles.py
+-rw-rw-rw-   0        0        0    51752 2022-11-28 05:43:22.000000 pedal-2.4.2/pedal/types/new_types.py
+-rw-rw-rw-   0        0        0    14813 2022-11-23 18:45:05.000000 pedal-2.4.2/pedal/types/normalize.py
+-rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:52.000000 pedal-2.4.2/pedal/types/operations.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.904905 pedal-2.4.2/pedal/utilities/
+-rw-rw-rw-   0        0        0      524 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:01.000000 pedal-2.4.2/pedal/utilities/ast_tools.py
+-rw-rw-rw-   0        0        0     6580 2022-07-27 17:31:05.000000 pedal-2.4.2/pedal/utilities/comparisons.py
+-rw-rw-rw-   0        0        0      679 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/utilities/dictionaries.py
+-rw-rw-rw-   0        0        0     8300 2022-09-23 12:51:56.000000 pedal-2.4.2/pedal/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:41.000000 pedal-2.4.2/pedal/utilities/files.py
+-rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/utilities/operators.py
+-rw-rw-rw-   0        0        0     7037 2022-12-31 17:53:00.000000 pedal-2.4.2/pedal/utilities/progsnap.py
+-rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/utilities/sorting.py
+-rw-rw-rw-   0        0        0      326 2021-06-28 19:25:31.000000 pedal-2.4.2/pedal/utilities/system.py
+-rw-rw-rw-   0        0        0     2313 2022-07-27 16:49:13.000000 pedal-2.4.2/pedal/utilities/text.py
+-rw-rw-rw-   0        0        0      769 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/utilities/types.py
+-rw-rw-rw-   0        0        0      121 2023-05-22 16:55:56.906905 pedal-2.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1196 2023-05-22 16:26:30.000000 pedal-2.4.2/setup.py
```

### Comparing `pedal-2.4.1/LICENSE` & `pedal-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/PKG-INFO` & `pedal-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pedal
-Version: 2.4.1
+Version: 2.4.2
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Description: Pedal
         =====
```

### Comparing `pedal-2.4.1/Pedal.egg-info/PKG-INFO` & `pedal-2.4.2/Pedal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pedal
-Version: 2.4.1
+Version: 2.4.2
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Description: Pedal
         =====
```

### Comparing `pedal-2.4.1/Pedal.egg-info/SOURCES.txt` & `pedal-2.4.2/Pedal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/README.rst` & `pedal-2.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/assertions/__init__.py` & `pedal-2.4.2/pedal/assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/assertions/classes.py` & `pedal-2.4.2/pedal/assertions/classes.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/assertions/commands.py` & `pedal-2.4.2/pedal/assertions/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/assertions/feedbacks.py` & `pedal-2.4.2/pedal/assertions/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/assertions/functions.py` & `pedal-2.4.2/pedal/assertions/functions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/assertions/organizers.py` & `pedal-2.4.2/pedal/assertions/organizers.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/assertions/runtime.py` & `pedal-2.4.2/pedal/assertions/runtime.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/assertions/setup.py` & `pedal-2.4.2/pedal/assertions/setup.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/assertions/static.py` & `pedal-2.4.2/pedal/assertions/static.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/assertions/unittest.py` & `pedal-2.4.2/pedal/assertions/unittest.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/cait/ast_helpers.py` & `pedal-2.4.2/pedal/cait/ast_helpers.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/cait/ast_map.py` & `pedal-2.4.2/pedal/cait/ast_map.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/cait/cait_api.py` & `pedal-2.4.2/pedal/cait/cait_api.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/cait/cait_node.py` & `pedal-2.4.2/pedal/cait/cait_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/cait/find_node.py` & `pedal-2.4.2/pedal/cait/find_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/cait/stretchy_tree_matching.py` & `pedal-2.4.2/pedal/cait/stretchy_tree_matching.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/command_line/command_line.py` & `pedal-2.4.2/pedal/command_line/command_line.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/command_line/mocks.py` & `pedal-2.4.2/pedal/command_line/mocks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/command_line/modes.py` & `pedal-2.4.2/pedal/command_line/modes.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/command_line/report.py` & `pedal-2.4.2/pedal/command_line/report.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/command_line/verify.py` & `pedal-2.4.2/pedal/command_line/verify.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/core/commands.py` & `pedal-2.4.2/pedal/core/commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Imperative style commands for constructing feedback in a convenient way.
 Uses a global report object (MAIN_REPORT).
 """
 
 __all__ = ['feedback', 'set_success', 'compliment', 'give_partial', 'explain',
            'gently', 'hide_correctness', 'suppress', 'log', 'debug',
            'system_error', 'clear_report', 'get_all_feedback', 'guidance',
-           'contextualize_report', 'Feedback', 'get_submission']
+           'contextualize_report', 'Feedback', 'get_submission', 'set_formatter']
 
 from pedal.core.feedback import (Feedback, FeedbackKind, FeedbackCategory,
                                  FeedbackResponse)
 from pedal.core.report import MAIN_REPORT
 
 from pedal.core.submission import Submission
 
@@ -263,8 +263,21 @@
     title = "System Error"
     category = Feedback.CATEGORIES.SYSTEM
     kind = FeedbackKind.META
     valence = Feedback.NEUTRAL_VALENCE
     muted = True
 
 
-# TODO: set_line_offset(offset, filename='answer.py')
+# TODO: set_line_offset(offset, filename='answer.py')
+
+def set_formatter(formatter, report=MAIN_REPORT):
+    """
+    Set the formatter for the given report.
+
+    Args:
+        formatter (Formatter): The formatter class to use. If you wish to use an instance instead,
+            you'll need to call `set_formatter` on the report instance instead.
+        report (:py:class:`~pedal.core.report.Report`): The report to attach
+            this feedback to (defaults to the
+            :py:data:`~pedal.core.report.MAIN_REPORT`).
+    """
+    report.set_formatter(formatter(report))
```

### Comparing `pedal-2.4.1/pedal/core/environment.py` & `pedal-2.4.2/pedal/core/environment.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/core/errors.py` & `pedal-2.4.2/pedal/core/errors.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/core/feedback.py` & `pedal-2.4.2/pedal/core/feedback.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/core/feedback_category.py` & `pedal-2.4.2/pedal/core/feedback_category.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/core/final_feedback.py` & `pedal-2.4.2/pedal/core/final_feedback.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/core/formatting.py` & `pedal-2.4.2/pedal/core/formatting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/core/location.py` & `pedal-2.4.2/pedal/core/location.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/core/report.py` & `pedal-2.4.2/pedal/core/report.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/core/resolver.py` & `pedal-2.4.2/pedal/core/resolver.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/core/scoring.py` & `pedal-2.4.2/pedal/core/scoring.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/core/submission.py` & `pedal-2.4.2/pedal/core/submission.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/core/tool.py` & `pedal-2.4.2/pedal/core/tool.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/environments/__init__.py` & `pedal-2.4.2/pedal/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/environments/blockpy.py` & `pedal-2.4.2/pedal/environments/blockpy.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/environments/gradescope.py` & `pedal-2.4.2/pedal/environments/gradescope.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/environments/jupyter.py` & `pedal-2.4.2/pedal/environments/jupyter.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/environments/nbgrader.py` & `pedal-2.4.2/pedal/environments/nbgrader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/environments/sandbox.py` & `pedal-2.4.2/pedal/environments/sandbox.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/environments/standard.py` & `pedal-2.4.2/pedal/environments/standard.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/environments/vpl.py` & `pedal-2.4.2/pedal/environments/vpl.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/extensions/microbit.py` & `pedal-2.4.2/pedal/extensions/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/extensions/plotting.py` & `pedal-2.4.2/pedal/extensions/plotting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/questions/__init__.py` & `pedal-2.4.2/pedal/questions/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/questions/feedbacks.py` & `pedal-2.4.2/pedal/questions/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/questions/graders.py` & `pedal-2.4.2/pedal/questions/graders.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/questions/loader.py` & `pedal-2.4.2/pedal/questions/loader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/questions/pool.py` & `pedal-2.4.2/pedal/questions/pool.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/questions/questions.py` & `pedal-2.4.2/pedal/questions/questions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/questions/setup.py` & `pedal-2.4.2/pedal/questions/setup.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/resolvers/__init__.py` & `pedal-2.4.2/pedal/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/resolvers/core.py` & `pedal-2.4.2/pedal/resolvers/core.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/resolvers/full.py` & `pedal-2.4.2/pedal/resolvers/full.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/resolvers/sectional.py` & `pedal-2.4.2/pedal/resolvers/sectional.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/resolvers/simple.py` & `pedal-2.4.2/pedal/resolvers/simple.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/resolvers/statistics.py` & `pedal-2.4.2/pedal/resolvers/statistics.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/sandbox/__init__.py` & `pedal-2.4.2/pedal/sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/sandbox/commands.py` & `pedal-2.4.2/pedal/sandbox/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/sandbox/data.py` & `pedal-2.4.2/pedal/sandbox/data.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/sandbox/exceptions.py` & `pedal-2.4.2/pedal/sandbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/sandbox/feedbacks.py` & `pedal-2.4.2/pedal/sandbox/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/sandbox/library/designer.py` & `pedal-2.4.2/pedal/sandbox/library/designer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/sandbox/library/matplotlib.py` & `pedal-2.4.2/pedal/sandbox/library/matplotlib.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/sandbox/library/microbit.py` & `pedal-2.4.2/pedal/sandbox/library/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/sandbox/library/turtles.py` & `pedal-2.4.2/pedal/sandbox/library/turtles.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/sandbox/mocked.py` & `pedal-2.4.2/pedal/sandbox/mocked.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/sandbox/result.py` & `pedal-2.4.2/pedal/sandbox/result.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/sandbox/sandbox.py` & `pedal-2.4.2/pedal/sandbox/sandbox.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/sandbox/timeout.py` & `pedal-2.4.2/pedal/sandbox/timeout.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/sandbox/tracer.py` & `pedal-2.4.2/pedal/sandbox/tracer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/source/__init__.py` & `pedal-2.4.2/pedal/source/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/source/feedbacks.py` & `pedal-2.4.2/pedal/source/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/source/sections.py` & `pedal-2.4.2/pedal/source/sections.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/source/source.py` & `pedal-2.4.2/pedal/source/source.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/tifa/__init__.py` & `pedal-2.4.2/pedal/tifa/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/tifa/commands.py` & `pedal-2.4.2/pedal/tifa/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/tifa/contexts.py` & `pedal-2.4.2/pedal/tifa/contexts.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/tifa/feedbacks.py` & `pedal-2.4.2/pedal/tifa/feedbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,39 +14,39 @@
     kind = FeedbackResponse.KINDS.MISTAKE
 
 
 class action_after_return(TifaFeedback):
     """ Statement after return """
     title = "Action after Return"
     message_template = ("You performed an action after already returning from "
-                        "a function, on line {location.line}. You can "
+                        "a function, on line {location.line:line}. You can "
                         "only return on a path once.")
     justification = ("TIFA visited a node not in the top scope when its "
                      "*return variable was definitely set in this scope.")
 
     def __init__(self, location, **kwargs):
         super().__init__(location=location, **kwargs)
 
 
 class return_outside_function(TifaFeedback):
     """ Return statement outside of function """
     title = "Return outside Function"
     message_template = ("You attempted to return outside of a function on line "
-                        "{location.line}. But you can only return from within "
+                        "{location.line:line}. But you can only return from within "
                         "a function.")
     justification = "TIFA visited a return node at the top level."
 
     def __init__(self, location, **kwargs):
         super().__init__(location=location, **kwargs)
 
 
 class multiple_return_types(TifaFeedback):
     """ Multiple returned types in single function """
     title = "Multiple Return Types"
-    message_template = ("Your function returned {actual} on line {location.line}, "
+    message_template = ("Your function returned {actual} on line {location.line:line}, "
                         "even though you defined it to return {expected}. "
                         "Your function should return values consistently.")
     justification = ("TIFA visited a function definition with multiple returns "
                      "that unequal types.")
 
     def __init__(self, location, expected, actual, **kwargs):
         super().__init__(location=location, expected=expected,
@@ -54,42 +54,42 @@
 
 
 class write_out_of_scope(TifaFeedback):
     """ Write out of Scope """
     title = "Write Out of Scope"
     message_template = ("You attempted to write the variable {name_message} "
                         "from a higher scope (outside the function) on line "
-                        "{location.line}. You should only use variables inside "
+                        "{location.line:line}. You should only use variables inside "
                         "the function they were declared in.")
     justification = "TIFA stored to an existing variable not in this scope"
 
     def __init__(self, location, name, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
         super().__init__(location=location, name=name,
                          name_message=report.format.name(name), **kwargs)
 
 
 class unconnected_blocks(TifaFeedback):
     """ Unconnected Blocks """
     title = "Unconnected Blocks"
-    message_template = ("It looks like you have unconnected blocks on line {location.line}. "
+    message_template = ("It looks like you have unconnected blocks on line {location.line:line}. "
                         "Before you run your program, you must make sure that all "
                         "of your blocks are connected that there are no unfilled "
                         "holes.")
     justification = "TIFA found a name equal to ___"
 
     def __init__(self, location, **kwargs):
         super().__init__(location=location, **kwargs)
 
 
 class iteration_problem(TifaFeedback):
     """ Iteration Problem """
     title = "Iteration Problem"
     message_template = ("The variable {name_message} was iterated on line "
-                        "{location.line} but you used the same variable as the iteration "
+                        "{location.line:line} but you used the same variable as the iteration "
                         "variable. You should choose a different variable name "
                         "for the iteration variable. Usually, the iteration variable "
                         "is the singular form of the iteration list (e.g., "
                         "`for a_dog in dogs:`).")
     justification = "TIFA visited a loop where the iteration list and target were the same."
 
     def __init__(self, location, name, **kwargs):
@@ -97,30 +97,30 @@
         super().__init__(location=location, name=name,
                          name_message=report.format.name(name), **kwargs)
 
 
 class initialization_problem(TifaFeedback):
     """ Initialization Problem """
     title = "Initialization Problem"
-    message_template = ("The variable {name_message} was used on line {location.line}, "
+    message_template = ("The variable {name_message} was used on line {location.line:line}, "
                         "but it was not given a value on a previous line. "
                         "You cannot use a variable until it has been given a value."
                         )
     justification = "TIFA read a variable that did not exist or was not previously set in this branch."
 
     def __init__(self, location, name, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
         super().__init__(location=location, name=name,
                          name_message=report.format.name(name), **kwargs)
 
 
 class possible_initialization_problem(TifaFeedback):
     """ Possible Initialization Problem """
     title = "Possible Initialization Problem"
-    message_template = ("The variable {name_message} was used on line {location.line}, "
+    message_template = ("The variable {name_message} was used on line {location.line:line}, "
                         "but it was possibly not given a value on a previous "
                         "line. You cannot use a variable until it has been given "
                         "a value. Check to make sure that this variable was "
                         "declared in all of the branches of your decision."
                         )
     justification = "TIFA read a variable that was maybe set but not definitely set in this branch."
 
@@ -130,15 +130,15 @@
                          name_message=report.format.name(name), **kwargs)
 
 
 class unused_variable(TifaFeedback):
     """ Unused Variable """
     title = "Unused Variable"
     message_template = ("The {kind} {name_message} was {initialization} on line "
-                        "{location.line}, but was never used after that.")
+                        "{location.line:line}, but was never used after that.")
     justification = ("TIFA stored a variable but it was not read any other time "
                      "in the program.")
 
     def __init__(self, location, name, variable_type, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
         if isinstance(variable_type, ModuleType):
             kind, initialization = 'module', 'imported'
@@ -157,15 +157,15 @@
         super().__init__(location=location, fields=fields, **kwargs)
 
 
 class overwritten_variable(TifaFeedback):
     """ Overwritten Variable """
     title = "Overwritten Variable"
     message_template = ("The variable {name_message} was given a value, but "
-                        "{name_message} was changed on line {location.line} "
+                        "{name_message} was changed on line {location.line:line} "
                         "before it was used. One of the times that you gave "
                         "{name_message} a value was incorrect."
                         )
     justification = ("TIFA attempted to store to a variable that was previously "
                      "stored but not read.")
 
     def __init__(self, location, name, **kwargs):
@@ -174,15 +174,15 @@
                          name_message=report.format.name(name), **kwargs)
 
 
 class iterating_over_non_list(TifaFeedback):
     """ Iterating over non-list """
     title = "Iterating over Non-list"
     message_template = ("The {iter} is not a list, but you used it in the "
-                        "iteration on line {location.line}. You should only "
+                        "iteration on line {location.line:line}. You should only "
                         "iterate over sequences like lists.")
     justification = ("TIFA visited a loop's iteration list whose type was"
                      "not indexable.")
 
     def __init__(self, location, iter_name, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
         if iter_name is None:
@@ -197,15 +197,15 @@
 
 
 class iterating_over_empty_list(TifaFeedback):
     """ Iterating over empty list """
     title = "Iterating over empty list"
     message_template = ("The {iter} was set as an empty list, "
                         "and then you attempted to use it in an iteration on line "
-                        "{location.line}. You should only iterate over non-empty lists."
+                        "{location.line:line}. You should only iterate over non-empty lists."
                         )
     justification = "TIFA visited a loop's iteration list that was empty."
 
     def __init__(self, location, iter_name, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
         if iter_name is None:
             iter_list = "expression"
@@ -215,15 +215,15 @@
         super().__init__(location=location, fields=fields, **kwargs)
 
 
 class incompatible_types(TifaFeedback):
     """ Incompatible types """
     title = "Incompatible types"
     message_template = ("You used {op_name} operation with {left_name} and {right_name} on line "
-                        "{location.line}. But you can't do that with that operator. Make "
+                        "{location.line:line}. But you can't do that with that operator. Make "
                         "sure both sides of the operator are the right type."
                         )
     justification = "TIFA visited an operation with operands of the wrong type."
 
     def __init__(self, location, operation, left, right, **kwargs):
         op_name = OPERATION_DESCRIPTION.get(operation.__class__,
                                             str(operation))
@@ -236,15 +236,15 @@
         super().__init__(location=location, fields=fields, **kwargs)
 
 
 class invalid_indexing(TifaFeedback):
     """ Invalid Index """
     title = "Invalid Index"
     message_template = ("You indexed {left_name} with {right_name} on line "
-                        "{location.line}. But you can't index {left_name} with "
+                        "{location.line:line}. But you can't index {left_name} with "
                         "{right_name}."
                         )
     justification = ("TIFA attempted to call an .index() operation on a type"
                      " with a type that wasn't acceptable.")
     muted = True
 
     def __init__(self, location, left, right, **kwargs):
@@ -256,15 +256,15 @@
         super().__init__(location=location, fields=fields, **kwargs)
 
 
 class parameter_type_mismatch(TifaFeedback):
     """ Parameter type mismatch """
     title = "Parameter Type Mismatch"
     message_template = ("You defined the parameter {parameter_name_message} "
-                        "as {parameter_type_name}. However, the argument passed to that parameter on line {location.line} "
+                        "as {parameter_type_name}. However, the argument passed to that parameter on line {location.line:line} "
                         "was {argument_type_name}. The formal parameter type must match the argument's type."
                         )
     justification = "TIFA visited a function definition where a parameter type and argument type were not equal."
 
     def __init__(self, location, parameter_name, parameter, argument, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
         parameter_type_name = parameter.singular_name
@@ -282,15 +282,15 @@
 
 
 class field_type_mismatch(TifaFeedback):
     """ Field type mismatch """
     title = "Field Type Mismatch"
     message_template = ("You defined the field {field_name_message} "
                         "as {field_type_name}. However, the argument passed to that field's parameter in the"
-                        " constructor function on line {location.line} was {argument_type_name}. The formal field"
+                        " constructor function on line {location.line:line} was {argument_type_name}. The formal field"
                         " type must match the argument's type."
                         )
     justification = "TIFA visited a constructor function call where a parameter type and argument type were not subtypes."
 
     def __init__(self, location, field_name, field, argument, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
         field_type_name = field.singular_name
@@ -306,15 +306,15 @@
                   'argument_type_name': argument_type_name}
         super().__init__(location=location, fields=fields, **kwargs)
 
 class read_out_of_scope(TifaFeedback):
     """ Read out of scope """
     title = "Read out of Scope"
     message_template = ("You attempted to read the variable {name_message} "
-                        "from a different scope on line {location.line}. You "
+                        "from a different scope on line {location.line:line}. You "
                         "should only use variables inside the function they "
                         "were declared in."
                         )
     justification = "TIFA read a variable that did not exist in this scope but existed in another."
 
     def __init__(self, location, name, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
@@ -323,30 +323,30 @@
 
 
 # TODO: Complete these
 class type_changes(TifaFeedback):
     """ Type changes """
     title = "Type Changes"
     message_template = ("The variable {name_message} changed type from {old} to "
-                        "{new} on line {location.line}.")
+                        "{new} on line {location.line:line}.")
     justification = ""
     muted = True
 
     def __init__(self, location, name, old, new, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
         fields = {'location': location, 'name': name,
                   'name_message': report.format.name(name),
                   'old': old, 'new': new}
         super().__init__(location=location, fields=fields, **kwargs)
 
 
 class attribute_type_change(TifaFeedback):
     """ Type change on attribute """
     title = "Attribute Type Change"
-    message_template = ("On line {location.line}, you attempted to assign a {new} to "
+    message_template = ("On line {location.line:line}, you attempted to assign a {new} to "
                         "the attribute {attr_message}, which was supposed to be {old}.")
     justification = ""
     muted = False
 
     def __init__(self, location, attr, old, new, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
         fields = {'location': location, 'attr': attr,
@@ -354,28 +354,28 @@
                   'old': old, 'new': new}
         super().__init__(location=location, fields=fields, **kwargs)
 
 class type_change_append(TifaFeedback):
     """ Type Change in an append Method """
     title = "Type Change in Append"
     message_template = ("You attempted to append a {new} to a list that was "
-                        "supposed to have {old} on line {location.line}.")
+                        "supposed to have {old} on line {location.line:line}.")
     justification = ""
     muted = True
 
     def __init__(self, location, old, new, **kwargs):
         fields = {'location': location, 'old': old, 'new': new}
         super().__init__(location=location, fields=fields, **kwargs)
 
 
 class unnecessary_second_branch(TifaFeedback):
     """ Unnecessary second branch """
     title = "Unnecessary Second Branch"
     message_template = ("You have an `if` statement where one of the two branches"
-                       " only has `pass` in its body, on line {location.line}."
+                       " only has `pass` in its body, on line {location.line:line}."
                         " You shouldn't need an empty body.")
     justification = "There is an else or if statement who's body is just pass."
 
     def __init__(self, location, **kwargs):
         super().__init__(location=location, **kwargs)
 
 
@@ -400,15 +400,15 @@
         super().__init__(location=location, name=name, **kwargs)
 
 
 class not_a_function(TifaFeedback):
     """ Not a function """
     title = "Not a Function"
     message_template = ("You attempted to call {name} as if it"
-                        " was a function on line {location.line}. However,"
+                        " was a function on line {location.line:line}. However,"
                         " that expression was actually {singular_name}.")
     justification = ""
     # TODO: Unmute?
     #muted = True
 
     def __init__(self, location, name, called_type, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
@@ -462,15 +462,15 @@
                   "actual_type": actual_type}
         super().__init__(location=location, fields=fields, **kwargs)
 
 
 class nested_function_definition(TifaFeedback):
     """ Function defined not at top-level """
     message_template = ("The function {name_message} was defined inside of another"
-                        "block on line {location.line}. For instance, you may "
+                        "block on line {location.line:line}. For instance, you may "
                         "have placed it inside another function definition, or "
                         "inside of a loop. Do not nest your function "
                         "definition!")
     title = "Don't Nest Functions"
     justification = "Found a FunctionDef that was not at the top-level."
     muted = True
     unscored = True
@@ -481,15 +481,15 @@
                          name_message=report.format.name(name), **kwargs)
 
 
 class unused_returned_value(TifaFeedback):
     """ Expr node had a non-None value """
     title = "Did Not Use Function's Return Value"
     message_template = ("It looks like you called the {call_type} {name_message} on "
-                        "{location.line}, but failed to store the result in "
+                        "{location.line:line}, but failed to store the result in "
                         "a variable or use it in an expression. You should "
                         "remember to use the result!")
     justification = "Expression node calculated a non-None value."
     muted = True
     unscored = True
 
     def __init__(self, location, name, call_type, result_type, **kwargs):
```

### Comparing `pedal-2.4.1/pedal/tifa/identifier.py` & `pedal-2.4.2/pedal/tifa/identifier.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/tifa/settings.py` & `pedal-2.4.2/pedal/tifa/settings.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/tifa/state.py` & `pedal-2.4.2/pedal/tifa/state.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/tifa/tifa_core.py` & `pedal-2.4.2/pedal/tifa/tifa_core.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/tifa/tifa_visitor.py` & `pedal-2.4.2/pedal/tifa/tifa_visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                          report=self.report)
             return self.analysis
         # Attempt processing code - might fail!
         try:
             self.process_ast(ast_tree)
         except Exception as error:
             self.analysis.fail(error)
-            system_error(TOOL_NAME, "Successfully parsed but could not "
+            system_error(TOOL_NAME, message="Successfully parsed but could not "
                                     "process AST: " + str(error),
                          report=self.report)
         # Return whatever we got
         return self.analysis
 
     def process_ast(self, ast_tree):
         """
```

### Comparing `pedal-2.4.1/pedal/types/builtin.py` & `pedal-2.4.2/pedal/types/builtin.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/types/library/cs1_curriculum.py` & `pedal-2.4.2/pedal/types/library/cs1_curriculum.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/types/library/designer.py` & `pedal-2.4.2/pedal/types/library/designer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/types/library/matplotlib.py` & `pedal-2.4.2/pedal/types/library/matplotlib.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/types/library/microbit.py` & `pedal-2.4.2/pedal/types/library/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/types/new_types.py` & `pedal-2.4.2/pedal/types/new_types.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/types/normalize.py` & `pedal-2.4.2/pedal/types/normalize.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/types/operations.py` & `pedal-2.4.2/pedal/types/operations.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/utilities/__init__.py` & `pedal-2.4.2/pedal/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/utilities/ast_tools.py` & `pedal-2.4.2/pedal/utilities/ast_tools.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/utilities/comparisons.py` & `pedal-2.4.2/pedal/utilities/comparisons.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/utilities/dictionaries.py` & `pedal-2.4.2/pedal/utilities/dictionaries.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/utilities/exceptions.py` & `pedal-2.4.2/pedal/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/utilities/files.py` & `pedal-2.4.2/pedal/utilities/files.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/utilities/operators.py` & `pedal-2.4.2/pedal/utilities/operators.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/utilities/progsnap.py` & `pedal-2.4.2/pedal/utilities/progsnap.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/utilities/sorting.py` & `pedal-2.4.2/pedal/utilities/sorting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/utilities/text.py` & `pedal-2.4.2/pedal/utilities/text.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/pedal/utilities/types.py` & `pedal-2.4.2/pedal/utilities/types.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.1/setup.py` & `pedal-2.4.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='pedal',
-    version='2.4.1',
+    version='2.4.2',
     python_requires='>=3.6',
     author='acbart,lukesg08',
     author_email='acbart@udel.edu',
     description='Tools to provide feedback on student code.',
     keywords='feedback education teaching program analysis tifa cait sandbox pedal grading grader grade',
     packages=['pedal', 'pedal.core', 'pedal.utilities', 'pedal.environments',
               'pedal.resolvers', 'pedal.command_line',
```

