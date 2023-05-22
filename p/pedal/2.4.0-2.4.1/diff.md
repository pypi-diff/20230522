# Comparing `tmp/pedal-2.4.0.tar.gz` & `tmp/pedal-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedal-2.4.0.tar", last modified: Thu May 18 18:37:44 2023, max compression
+gzip compressed data, was "pedal-2.4.1.tar", last modified: Mon May 22 16:09:08 2023, max compression
```

## Comparing `pedal-2.4.0.tar` & `pedal-2.4.1.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:44.112724 pedal-2.4.0/
--rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:21.000000 pedal-2.4.0/LICENSE
--rw-rw-rw-   0        0        0     2924 2023-05-18 18:37:44.114730 pedal-2.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:42.795722 pedal-2.4.0/Pedal.egg-info/
--rw-rw-rw-   0        0        0     2924 2023-05-18 18:37:41.000000 pedal-2.4.0/Pedal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3702 2023-05-18 18:37:41.000000 pedal-2.4.0/Pedal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 18:37:41.000000 pedal-2.4.0/Pedal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-18 18:37:41.000000 pedal-2.4.0/Pedal.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 18:37:41.000000 pedal-2.4.0/Pedal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-18 18:37:41.000000 pedal-2.4.0/Pedal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1901 2020-10-17 19:58:17.000000 pedal-2.4.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:42.772724 pedal-2.4.0/pedal/
--rw-rw-rw-   0        0        0      382 2023-05-18 18:14:23.000000 pedal-2.4.0/pedal/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:42.912720 pedal-2.4.0/pedal/assertions/
--rw-rw-rw-   0        0        0      549 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/assertions/__init__.py
--rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:31.000000 pedal-2.4.0/pedal/assertions/classes.py
--rw-rw-rw-   0        0        0    13288 2023-01-17 17:53:58.000000 pedal-2.4.0/pedal/assertions/commands.py
--rw-rw-rw-   0        0        0       73 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/assertions/constants.py
--rw-rw-rw-   0        0        0    20378 2022-09-17 21:23:34.000000 pedal-2.4.0/pedal/assertions/feedbacks.py
--rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:04.000000 pedal-2.4.0/pedal/assertions/functions.py
--rw-rw-rw-   0        0        0     5722 2021-01-26 15:12:38.000000 pedal-2.4.0/pedal/assertions/organizers.py
--rw-rw-rw-   0        0        0    33479 2023-01-17 17:50:34.000000 pedal-2.4.0/pedal/assertions/runtime.py
--rw-rw-rw-   0        0        0     3254 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/assertions/setup.py
--rw-rw-rw-   0        0        0    30229 2022-11-17 14:15:37.000000 pedal-2.4.0/pedal/assertions/static.py
--rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/assertions/unittest.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.005721 pedal-2.4.0/pedal/cait/
--rw-rw-rw-   0        0        0      445 2020-10-17 20:34:56.000000 pedal-2.4.0/pedal/cait/__init__.py
--rw-rw-rw-   0        0        0     2254 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/cait/ast_helpers.py
--rw-rw-rw-   0        0        0    11371 2021-03-12 21:12:46.000000 pedal-2.4.0/pedal/cait/ast_map.py
--rw-rw-rw-   0        0        0    10523 2021-01-08 04:00:46.000000 pedal-2.4.0/pedal/cait/cait_api.py
--rw-rw-rw-   0        0        0    22471 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/cait/cait_node.py
--rw-rw-rw-   0        0        0       59 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/cait/constants.py
--rw-rw-rw-   0        0        0     4693 2021-06-28 19:26:48.000000 pedal-2.4.0/pedal/cait/find_node.py
--rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:46.000000 pedal-2.4.0/pedal/cait/stretchy_tree_matching.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.089720 pedal-2.4.0/pedal/command_line/
--rw-rw-rw-   0        0        0       94 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/command_line/__init__.py
--rw-rw-rw-   0        0        0     7897 2022-04-30 18:25:37.000000 pedal-2.4.0/pedal/command_line/command_line.py
--rw-rw-rw-   0        0        0     7493 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/command_line/mocks.py
--rw-rw-rw-   0        0        0    25271 2022-11-11 18:14:58.000000 pedal-2.4.0/pedal/command_line/modes.py
--rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:52.000000 pedal-2.4.0/pedal/command_line/report.py
--rw-rw-rw-   0        0        0     3540 2020-11-08 16:28:36.000000 pedal-2.4.0/pedal/command_line/verify.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.250713 pedal-2.4.0/pedal/core/
--rw-rw-rw-   0        0        0      107 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/core/__init__.py
--rw-rw-rw-   0        0        0     8756 2022-11-11 16:40:07.000000 pedal-2.4.0/pedal/core/commands.py
--rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/core/environment.py
--rw-rw-rw-   0        0        0      707 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/core/errors.py
--rw-rw-rw-   0        0        0    20881 2023-01-17 17:46:13.000000 pedal-2.4.0/pedal/core/feedback.py
--rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/core/feedback_category.py
--rw-rw-rw-   0        0        0     6107 2022-11-17 14:35:13.000000 pedal-2.4.0/pedal/core/final_feedback.py
--rw-rw-rw-   0        0        0     7639 2023-01-17 17:14:11.000000 pedal-2.4.0/pedal/core/formatting.py
--rw-rw-rw-   0        0        0     1915 2022-06-12 19:44:51.000000 pedal-2.4.0/pedal/core/location.py
--rw-rw-rw-   0        0        0    13385 2022-11-28 05:44:51.000000 pedal-2.4.0/pedal/core/report.py
--rw-rw-rw-   0        0        0      822 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/core/resolver.py
--rw-rw-rw-   0        0        0     3985 2022-11-17 14:35:11.000000 pedal-2.4.0/pedal/core/scoring.py
--rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:08.000000 pedal-2.4.0/pedal/core/submission.py
--rw-rw-rw-   0        0        0      405 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/core/tag.py
--rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:35.000000 pedal-2.4.0/pedal/core/tool.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.350729 pedal-2.4.0/pedal/environments/
--rw-rw-rw-   0        0        0      657 2020-11-08 17:16:23.000000 pedal-2.4.0/pedal/environments/__init__.py
--rw-rw-rw-   0        0        0     3042 2021-02-26 19:18:08.000000 pedal-2.4.0/pedal/environments/blockpy.py
--rw-rw-rw-   0        0        0     9569 2022-11-23 18:26:45.000000 pedal-2.4.0/pedal/environments/gradescope.py
--rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:49.000000 pedal-2.4.0/pedal/environments/jupyter.py
--rw-rw-rw-   0        0        0    10351 2021-02-02 16:30:22.000000 pedal-2.4.0/pedal/environments/nbgrader.py
--rw-rw-rw-   0        0        0      368 2020-11-08 17:19:12.000000 pedal-2.4.0/pedal/environments/none.py
--rw-rw-rw-   0        0        0      766 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/environments/sandbox.py
--rw-rw-rw-   0        0        0     3651 2023-04-19 22:17:37.000000 pedal-2.4.0/pedal/environments/standard.py
--rw-rw-rw-   0        0        0     6259 2020-11-13 04:58:08.000000 pedal-2.4.0/pedal/environments/vpl.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.398719 pedal-2.4.0/pedal/extensions/
--rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/extensions/__init__.py
--rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:33.000000 pedal-2.4.0/pedal/extensions/microbit.py
--rw-rw-rw-   0        0        0    11604 2022-11-26 00:03:07.000000 pedal-2.4.0/pedal/extensions/plotting.py
--rw-rw-rw-   0        0        0       81 2022-07-17 15:14:06.000000 pedal-2.4.0/pedal/extensions/turtles.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.502725 pedal-2.4.0/pedal/questions/
--rw-rw-rw-   0        0        0      669 2021-12-05 16:49:53.000000 pedal-2.4.0/pedal/questions/__init__.py
--rw-rw-rw-   0        0        0       66 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/questions/constants.py
--rw-rw-rw-   0        0        0      624 2021-09-15 19:16:10.000000 pedal-2.4.0/pedal/questions/feedbacks.py
--rw-rw-rw-   0        0        0     6045 2022-11-16 17:32:45.000000 pedal-2.4.0/pedal/questions/graders.py
--rw-rw-rw-   0        0        0     3477 2021-12-05 16:42:01.000000 pedal-2.4.0/pedal/questions/loader.py
--rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:25.000000 pedal-2.4.0/pedal/questions/pool.py
--rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:15.000000 pedal-2.4.0/pedal/questions/questions.py
--rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:28.000000 pedal-2.4.0/pedal/questions/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.578717 pedal-2.4.0/pedal/resolvers/
--rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:56.000000 pedal-2.4.0/pedal/resolvers/__init__.py
--rw-rw-rw-   0        0        0      654 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/resolvers/core.py
--rw-rw-rw-   0        0        0     2099 2023-05-13 15:07:02.000000 pedal-2.4.0/pedal/resolvers/full.py
--rw-rw-rw-   0        0        0     1886 2022-11-23 18:27:16.000000 pedal-2.4.0/pedal/resolvers/sectional.py
--rw-rw-rw-   0        0        0      268 2021-01-26 15:52:26.000000 pedal-2.4.0/pedal/resolvers/silent.py
--rw-rw-rw-   0        0        0     5119 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/resolvers/simple.py
--rw-rw-rw-   0        0        0     1176 2020-11-03 17:24:20.000000 pedal-2.4.0/pedal/resolvers/statistics.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.687740 pedal-2.4.0/pedal/sandbox/
--rw-rw-rw-   0        0        0      662 2023-05-13 15:07:02.000000 pedal-2.4.0/pedal/sandbox/__init__.py
--rw-rw-rw-   0        0        0    17919 2023-05-18 18:30:27.000000 pedal-2.4.0/pedal/sandbox/commands.py
--rw-rw-rw-   0        0        0       72 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/sandbox/constants.py
--rw-rw-rw-   0        0        0     9652 2023-05-13 15:13:44.000000 pedal-2.4.0/pedal/sandbox/data.py
--rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:18.000000 pedal-2.4.0/pedal/sandbox/exceptions.py
--rw-rw-rw-   0        0        0    10750 2022-10-04 22:22:33.000000 pedal-2.4.0/pedal/sandbox/feedbacks.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.738721 pedal-2.4.0/pedal/sandbox/library/
--rw-rw-rw-   0        0        0      222 2022-07-17 15:26:46.000000 pedal-2.4.0/pedal/sandbox/library/__init__.py
--rw-rw-rw-   0        0        0     5028 2022-08-18 18:00:00.000000 pedal-2.4.0/pedal/sandbox/library/designer.py
--rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:41.000000 pedal-2.4.0/pedal/sandbox/library/matplotlib.py
--rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:51.000000 pedal-2.4.0/pedal/sandbox/library/microbit.py
--rw-rw-rw-   0        0        0     3400 2022-07-28 21:17:36.000000 pedal-2.4.0/pedal/sandbox/library/turtles.py
--rw-rw-rw-   0        0        0     9976 2023-05-18 18:17:30.000000 pedal-2.4.0/pedal/sandbox/mocked.py
--rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:23.000000 pedal-2.4.0/pedal/sandbox/result.py
--rw-rw-rw-   0        0        0    38481 2023-05-18 18:30:27.000000 pedal-2.4.0/pedal/sandbox/sandbox.py
--rw-rw-rw-   0        0        0     5048 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/sandbox/timeout.py
--rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:49.000000 pedal-2.4.0/pedal/sandbox/tracer.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.796721 pedal-2.4.0/pedal/source/
--rw-rw-rw-   0        0        0      912 2022-07-24 20:13:29.000000 pedal-2.4.0/pedal/source/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/source/constants.py
--rw-rw-rw-   0        0        0     5345 2022-10-04 00:04:29.000000 pedal-2.4.0/pedal/source/feedbacks.py
--rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/source/sections.py
--rw-rw-rw-   0        0        0     7441 2022-11-23 18:29:38.000000 pedal-2.4.0/pedal/source/source.py
--rw-rw-rw-   0        0        0      484 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/source/substitutions.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.881719 pedal-2.4.0/pedal/tifa/
--rw-rw-rw-   0        0        0     3049 2022-11-28 05:46:58.000000 pedal-2.4.0/pedal/tifa/__init__.py
--rw-rw-rw-   0        0        0     2143 2022-10-06 14:36:45.000000 pedal-2.4.0/pedal/tifa/commands.py
--rw-rw-rw-   0        0        0       91 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/tifa/constants.py
--rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:35.000000 pedal-2.4.0/pedal/tifa/contexts.py
--rw-rw-rw-   0        0        0    23536 2022-09-09 22:57:22.000000 pedal-2.4.0/pedal/tifa/feedbacks.py
--rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/tifa/identifier.py
--rw-rw-rw-   0        0        0      908 2022-06-07 19:06:45.000000 pedal-2.4.0/pedal/tifa/settings.py
--rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:15.000000 pedal-2.4.0/pedal/tifa/state.py
--rw-rw-rw-   0        0        0    24173 2022-10-07 14:11:04.000000 pedal-2.4.0/pedal/tifa/tifa_core.py
--rw-rw-rw-   0        0        0    42481 2022-09-22 03:35:00.000000 pedal-2.4.0/pedal/tifa/tifa_visitor.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.930717 pedal-2.4.0/pedal/types/
--rw-rw-rw-   0        0        0       86 2022-06-09 18:41:53.000000 pedal-2.4.0/pedal/types/__init__.py
--rw-rw-rw-   0        0        0     9115 2022-11-28 06:00:50.000000 pedal-2.4.0/pedal/types/builtin.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.991722 pedal-2.4.0/pedal/types/library/
--rw-rw-rw-   0        0        0      192 2022-07-26 18:00:27.000000 pedal-2.4.0/pedal/types/library/__init__.py
--rw-rw-rw-   0        0        0      792 2022-11-28 05:46:58.000000 pedal-2.4.0/pedal/types/library/cs1_curriculum.py
--rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:16.000000 pedal-2.4.0/pedal/types/library/designer.py
--rw-rw-rw-   0        0        0      792 2022-11-28 05:51:17.000000 pedal-2.4.0/pedal/types/library/matplotlib.py
--rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:25.000000 pedal-2.4.0/pedal/types/library/microbit.py
--rw-rw-rw-   0        0        0      441 2022-11-28 05:52:06.000000 pedal-2.4.0/pedal/types/library/turtles.py
--rw-rw-rw-   0        0        0    51752 2022-11-28 05:43:22.000000 pedal-2.4.0/pedal/types/new_types.py
--rw-rw-rw-   0        0        0    14813 2022-11-23 18:45:05.000000 pedal-2.4.0/pedal/types/normalize.py
--rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:52.000000 pedal-2.4.0/pedal/types/operations.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:37:44.104718 pedal-2.4.0/pedal/utilities/
--rw-rw-rw-   0        0        0      524 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/utilities/__init__.py
--rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:01.000000 pedal-2.4.0/pedal/utilities/ast_tools.py
--rw-rw-rw-   0        0        0     6580 2022-07-27 17:31:05.000000 pedal-2.4.0/pedal/utilities/comparisons.py
--rw-rw-rw-   0        0        0      679 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/utilities/dictionaries.py
--rw-rw-rw-   0        0        0     8300 2022-09-23 12:51:56.000000 pedal-2.4.0/pedal/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:41.000000 pedal-2.4.0/pedal/utilities/files.py
--rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/utilities/operators.py
--rw-rw-rw-   0        0        0     7037 2022-12-31 17:53:00.000000 pedal-2.4.0/pedal/utilities/progsnap.py
--rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/utilities/sorting.py
--rw-rw-rw-   0        0        0      326 2021-06-28 19:25:31.000000 pedal-2.4.0/pedal/utilities/system.py
--rw-rw-rw-   0        0        0     2313 2022-07-27 16:49:13.000000 pedal-2.4.0/pedal/utilities/text.py
--rw-rw-rw-   0        0        0      769 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/utilities/types.py
--rw-rw-rw-   0        0        0      121 2023-05-18 18:37:44.120723 pedal-2.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1196 2023-05-18 18:33:43.000000 pedal-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.968699 pedal-2.4.1/
+-rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:21.000000 pedal-2.4.1/LICENSE
+-rw-rw-rw-   0        0        0     2981 2023-05-22 16:09:08.968699 pedal-2.4.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.792698 pedal-2.4.1/Pedal.egg-info/
+-rw-rw-rw-   0        0        0     2981 2023-05-22 16:09:08.000000 pedal-2.4.1/Pedal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3702 2023-05-22 16:09:08.000000 pedal-2.4.1/Pedal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 16:09:08.000000 pedal-2.4.1/Pedal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-22 16:09:08.000000 pedal-2.4.1/Pedal.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 16:09:08.000000 pedal-2.4.1/Pedal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-22 16:09:08.000000 pedal-2.4.1/Pedal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1958 2023-05-18 18:40:27.000000 pedal-2.4.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.789699 pedal-2.4.1/pedal/
+-rw-rw-rw-   0        0        0      382 2023-05-18 18:14:23.000000 pedal-2.4.1/pedal/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.807700 pedal-2.4.1/pedal/assertions/
+-rw-rw-rw-   0        0        0      549 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/assertions/__init__.py
+-rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:31.000000 pedal-2.4.1/pedal/assertions/classes.py
+-rw-rw-rw-   0        0        0    13288 2023-01-17 17:53:58.000000 pedal-2.4.1/pedal/assertions/commands.py
+-rw-rw-rw-   0        0        0       73 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/assertions/constants.py
+-rw-rw-rw-   0        0        0    20378 2022-09-17 21:23:34.000000 pedal-2.4.1/pedal/assertions/feedbacks.py
+-rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:04.000000 pedal-2.4.1/pedal/assertions/functions.py
+-rw-rw-rw-   0        0        0     5722 2021-01-26 15:12:38.000000 pedal-2.4.1/pedal/assertions/organizers.py
+-rw-rw-rw-   0        0        0    33479 2023-01-17 17:50:34.000000 pedal-2.4.1/pedal/assertions/runtime.py
+-rw-rw-rw-   0        0        0     3254 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/assertions/setup.py
+-rw-rw-rw-   0        0        0    30229 2022-11-17 14:15:37.000000 pedal-2.4.1/pedal/assertions/static.py
+-rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/assertions/unittest.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.817699 pedal-2.4.1/pedal/cait/
+-rw-rw-rw-   0        0        0      445 2020-10-17 20:34:56.000000 pedal-2.4.1/pedal/cait/__init__.py
+-rw-rw-rw-   0        0        0     2254 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/cait/ast_helpers.py
+-rw-rw-rw-   0        0        0    11371 2021-03-12 21:12:46.000000 pedal-2.4.1/pedal/cait/ast_map.py
+-rw-rw-rw-   0        0        0    10523 2021-01-08 04:00:46.000000 pedal-2.4.1/pedal/cait/cait_api.py
+-rw-rw-rw-   0        0        0    22471 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/cait/cait_node.py
+-rw-rw-rw-   0        0        0       59 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/cait/constants.py
+-rw-rw-rw-   0        0        0     4693 2021-06-28 19:26:48.000000 pedal-2.4.1/pedal/cait/find_node.py
+-rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:46.000000 pedal-2.4.1/pedal/cait/stretchy_tree_matching.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.827700 pedal-2.4.1/pedal/command_line/
+-rw-rw-rw-   0        0        0       94 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/command_line/__init__.py
+-rw-rw-rw-   0        0        0     7897 2022-04-30 18:25:37.000000 pedal-2.4.1/pedal/command_line/command_line.py
+-rw-rw-rw-   0        0        0     7493 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/command_line/mocks.py
+-rw-rw-rw-   0        0        0    25271 2022-11-11 18:14:58.000000 pedal-2.4.1/pedal/command_line/modes.py
+-rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:52.000000 pedal-2.4.1/pedal/command_line/report.py
+-rw-rw-rw-   0        0        0     3540 2020-11-08 16:28:36.000000 pedal-2.4.1/pedal/command_line/verify.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.852698 pedal-2.4.1/pedal/core/
+-rw-rw-rw-   0        0        0      107 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/core/__init__.py
+-rw-rw-rw-   0        0        0     8756 2022-11-11 16:40:07.000000 pedal-2.4.1/pedal/core/commands.py
+-rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/core/environment.py
+-rw-rw-rw-   0        0        0      707 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/core/errors.py
+-rw-rw-rw-   0        0        0    20881 2023-01-17 17:46:13.000000 pedal-2.4.1/pedal/core/feedback.py
+-rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/core/feedback_category.py
+-rw-rw-rw-   0        0        0     6107 2022-11-17 14:35:13.000000 pedal-2.4.1/pedal/core/final_feedback.py
+-rw-rw-rw-   0        0        0     7639 2023-01-17 17:14:11.000000 pedal-2.4.1/pedal/core/formatting.py
+-rw-rw-rw-   0        0        0     1915 2022-06-12 19:44:51.000000 pedal-2.4.1/pedal/core/location.py
+-rw-rw-rw-   0        0        0    13385 2022-11-28 05:44:51.000000 pedal-2.4.1/pedal/core/report.py
+-rw-rw-rw-   0        0        0      822 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/core/resolver.py
+-rw-rw-rw-   0        0        0     3985 2022-11-17 14:35:11.000000 pedal-2.4.1/pedal/core/scoring.py
+-rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:08.000000 pedal-2.4.1/pedal/core/submission.py
+-rw-rw-rw-   0        0        0      405 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/core/tag.py
+-rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:35.000000 pedal-2.4.1/pedal/core/tool.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.865698 pedal-2.4.1/pedal/environments/
+-rw-rw-rw-   0        0        0      657 2020-11-08 17:16:23.000000 pedal-2.4.1/pedal/environments/__init__.py
+-rw-rw-rw-   0        0        0     3042 2021-02-26 19:18:08.000000 pedal-2.4.1/pedal/environments/blockpy.py
+-rw-rw-rw-   0        0        0     9569 2022-11-23 18:26:45.000000 pedal-2.4.1/pedal/environments/gradescope.py
+-rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:49.000000 pedal-2.4.1/pedal/environments/jupyter.py
+-rw-rw-rw-   0        0        0    10351 2021-02-02 16:30:22.000000 pedal-2.4.1/pedal/environments/nbgrader.py
+-rw-rw-rw-   0        0        0      368 2020-11-08 17:19:12.000000 pedal-2.4.1/pedal/environments/none.py
+-rw-rw-rw-   0        0        0      766 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/environments/sandbox.py
+-rw-rw-rw-   0        0        0     3651 2023-04-19 22:17:37.000000 pedal-2.4.1/pedal/environments/standard.py
+-rw-rw-rw-   0        0        0     6259 2020-11-13 04:58:08.000000 pedal-2.4.1/pedal/environments/vpl.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.870699 pedal-2.4.1/pedal/extensions/
+-rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/extensions/__init__.py
+-rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:33.000000 pedal-2.4.1/pedal/extensions/microbit.py
+-rw-rw-rw-   0        0        0    11604 2022-11-26 00:03:07.000000 pedal-2.4.1/pedal/extensions/plotting.py
+-rw-rw-rw-   0        0        0       81 2022-07-17 15:14:06.000000 pedal-2.4.1/pedal/extensions/turtles.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.885698 pedal-2.4.1/pedal/questions/
+-rw-rw-rw-   0        0        0      669 2021-12-05 16:49:53.000000 pedal-2.4.1/pedal/questions/__init__.py
+-rw-rw-rw-   0        0        0       66 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/questions/constants.py
+-rw-rw-rw-   0        0        0      624 2021-09-15 19:16:10.000000 pedal-2.4.1/pedal/questions/feedbacks.py
+-rw-rw-rw-   0        0        0     6045 2022-11-16 17:32:45.000000 pedal-2.4.1/pedal/questions/graders.py
+-rw-rw-rw-   0        0        0     3477 2021-12-05 16:42:01.000000 pedal-2.4.1/pedal/questions/loader.py
+-rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:25.000000 pedal-2.4.1/pedal/questions/pool.py
+-rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:15.000000 pedal-2.4.1/pedal/questions/questions.py
+-rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:28.000000 pedal-2.4.1/pedal/questions/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.895699 pedal-2.4.1/pedal/resolvers/
+-rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:56.000000 pedal-2.4.1/pedal/resolvers/__init__.py
+-rw-rw-rw-   0        0        0      654 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/resolvers/core.py
+-rw-rw-rw-   0        0        0     2099 2023-05-13 15:07:02.000000 pedal-2.4.1/pedal/resolvers/full.py
+-rw-rw-rw-   0        0        0     1886 2022-11-23 18:27:16.000000 pedal-2.4.1/pedal/resolvers/sectional.py
+-rw-rw-rw-   0        0        0      268 2021-01-26 15:52:26.000000 pedal-2.4.1/pedal/resolvers/silent.py
+-rw-rw-rw-   0        0        0     5119 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/resolvers/simple.py
+-rw-rw-rw-   0        0        0     1176 2020-11-03 17:24:20.000000 pedal-2.4.1/pedal/resolvers/statistics.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.908699 pedal-2.4.1/pedal/sandbox/
+-rw-rw-rw-   0        0        0      662 2023-05-13 15:07:02.000000 pedal-2.4.1/pedal/sandbox/__init__.py
+-rw-rw-rw-   0        0        0    17919 2023-05-18 18:30:27.000000 pedal-2.4.1/pedal/sandbox/commands.py
+-rw-rw-rw-   0        0        0       72 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/sandbox/constants.py
+-rw-rw-rw-   0        0        0     9652 2023-05-13 15:13:44.000000 pedal-2.4.1/pedal/sandbox/data.py
+-rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:18.000000 pedal-2.4.1/pedal/sandbox/exceptions.py
+-rw-rw-rw-   0        0        0    10750 2022-10-04 22:22:33.000000 pedal-2.4.1/pedal/sandbox/feedbacks.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.914699 pedal-2.4.1/pedal/sandbox/library/
+-rw-rw-rw-   0        0        0      222 2022-07-17 15:26:46.000000 pedal-2.4.1/pedal/sandbox/library/__init__.py
+-rw-rw-rw-   0        0        0     5028 2022-08-18 18:00:00.000000 pedal-2.4.1/pedal/sandbox/library/designer.py
+-rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:41.000000 pedal-2.4.1/pedal/sandbox/library/matplotlib.py
+-rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:51.000000 pedal-2.4.1/pedal/sandbox/library/microbit.py
+-rw-rw-rw-   0        0        0     3400 2022-07-28 21:17:36.000000 pedal-2.4.1/pedal/sandbox/library/turtles.py
+-rw-rw-rw-   0        0        0    10124 2023-05-22 15:55:11.000000 pedal-2.4.1/pedal/sandbox/mocked.py
+-rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:23.000000 pedal-2.4.1/pedal/sandbox/result.py
+-rw-rw-rw-   0        0        0    38840 2023-05-22 14:40:28.000000 pedal-2.4.1/pedal/sandbox/sandbox.py
+-rw-rw-rw-   0        0        0     5048 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/sandbox/timeout.py
+-rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:49.000000 pedal-2.4.1/pedal/sandbox/tracer.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.922698 pedal-2.4.1/pedal/source/
+-rw-rw-rw-   0        0        0      912 2022-07-24 20:13:29.000000 pedal-2.4.1/pedal/source/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/source/constants.py
+-rw-rw-rw-   0        0        0     5345 2022-10-04 00:04:29.000000 pedal-2.4.1/pedal/source/feedbacks.py
+-rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/source/sections.py
+-rw-rw-rw-   0        0        0     7441 2022-11-23 18:29:38.000000 pedal-2.4.1/pedal/source/source.py
+-rw-rw-rw-   0        0        0      484 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/source/substitutions.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.936699 pedal-2.4.1/pedal/tifa/
+-rw-rw-rw-   0        0        0     3049 2022-11-28 05:46:58.000000 pedal-2.4.1/pedal/tifa/__init__.py
+-rw-rw-rw-   0        0        0     2143 2022-10-06 14:36:45.000000 pedal-2.4.1/pedal/tifa/commands.py
+-rw-rw-rw-   0        0        0       91 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/tifa/constants.py
+-rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:35.000000 pedal-2.4.1/pedal/tifa/contexts.py
+-rw-rw-rw-   0        0        0    23536 2022-09-09 22:57:22.000000 pedal-2.4.1/pedal/tifa/feedbacks.py
+-rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/tifa/identifier.py
+-rw-rw-rw-   0        0        0      908 2022-06-07 19:06:45.000000 pedal-2.4.1/pedal/tifa/settings.py
+-rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:15.000000 pedal-2.4.1/pedal/tifa/state.py
+-rw-rw-rw-   0        0        0    24173 2022-10-07 14:11:04.000000 pedal-2.4.1/pedal/tifa/tifa_core.py
+-rw-rw-rw-   0        0        0    42481 2022-09-22 03:35:00.000000 pedal-2.4.1/pedal/tifa/tifa_visitor.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.943699 pedal-2.4.1/pedal/types/
+-rw-rw-rw-   0        0        0       86 2022-06-09 18:41:53.000000 pedal-2.4.1/pedal/types/__init__.py
+-rw-rw-rw-   0        0        0     9115 2022-11-28 06:00:50.000000 pedal-2.4.1/pedal/types/builtin.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.951699 pedal-2.4.1/pedal/types/library/
+-rw-rw-rw-   0        0        0      192 2022-07-26 18:00:27.000000 pedal-2.4.1/pedal/types/library/__init__.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:46:58.000000 pedal-2.4.1/pedal/types/library/cs1_curriculum.py
+-rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:16.000000 pedal-2.4.1/pedal/types/library/designer.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:51:17.000000 pedal-2.4.1/pedal/types/library/matplotlib.py
+-rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:25.000000 pedal-2.4.1/pedal/types/library/microbit.py
+-rw-rw-rw-   0        0        0      441 2022-11-28 05:52:06.000000 pedal-2.4.1/pedal/types/library/turtles.py
+-rw-rw-rw-   0        0        0    51752 2022-11-28 05:43:22.000000 pedal-2.4.1/pedal/types/new_types.py
+-rw-rw-rw-   0        0        0    14813 2022-11-23 18:45:05.000000 pedal-2.4.1/pedal/types/normalize.py
+-rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:52.000000 pedal-2.4.1/pedal/types/operations.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:08.967700 pedal-2.4.1/pedal/utilities/
+-rw-rw-rw-   0        0        0      524 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:01.000000 pedal-2.4.1/pedal/utilities/ast_tools.py
+-rw-rw-rw-   0        0        0     6580 2022-07-27 17:31:05.000000 pedal-2.4.1/pedal/utilities/comparisons.py
+-rw-rw-rw-   0        0        0      679 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/utilities/dictionaries.py
+-rw-rw-rw-   0        0        0     8300 2022-09-23 12:51:56.000000 pedal-2.4.1/pedal/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:41.000000 pedal-2.4.1/pedal/utilities/files.py
+-rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/utilities/operators.py
+-rw-rw-rw-   0        0        0     7037 2022-12-31 17:53:00.000000 pedal-2.4.1/pedal/utilities/progsnap.py
+-rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/utilities/sorting.py
+-rw-rw-rw-   0        0        0      326 2021-06-28 19:25:31.000000 pedal-2.4.1/pedal/utilities/system.py
+-rw-rw-rw-   0        0        0     2313 2022-07-27 16:49:13.000000 pedal-2.4.1/pedal/utilities/text.py
+-rw-rw-rw-   0        0        0      769 2020-10-17 16:15:22.000000 pedal-2.4.1/pedal/utilities/types.py
+-rw-rw-rw-   0        0        0      121 2023-05-22 16:09:08.969699 pedal-2.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1196 2023-05-22 16:08:32.000000 pedal-2.4.1/setup.py
```

### Comparing `pedal-2.4.0/LICENSE` & `pedal-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/PKG-INFO` & `pedal-2.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pedal
-Version: 2.4.0
+Version: 2.4.1
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Description: Pedal
         =====
@@ -34,15 +34,15 @@
         
         Pedal revolves around providing *Feedback Functions* that can be called in an
         Instructor Control Script to generate *Feedback* for a *Submission*, which are
         all attached to a *Report*. A *Resolver* can then transform that Feedback into
         something that an *Environment* can hand off to a learner (or other interested
         party). These Feedback Functions are organized into *Tools*.
         
-        .. image:: docsrc/_static/pedal-overview-v3.png
+        .. image:: https://raw.githubusercontent.com/pedal-edu/pedal/master/docsrc/_static/pedal-overview-v3.png
         
         One of our major goals is to attach metadata to feedback to enable easier
         analysis, versioning, and evaluation. Although Instructor Control Scripts can
         be written very imperatively to specify very complex (or simple) grading logic,
         we are trying to reach an elegant, declarative style. This will enable tooling
         to automatically generate reports on occurrences of feedback, connect to
         datasets like those in the ProgSnap format, and allow us to "unit test our
```

### Comparing `pedal-2.4.0/Pedal.egg-info/PKG-INFO` & `pedal-2.4.1/Pedal.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pedal
-Version: 2.4.0
+Version: 2.4.1
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Description: Pedal
         =====
@@ -34,15 +34,15 @@
         
         Pedal revolves around providing *Feedback Functions* that can be called in an
         Instructor Control Script to generate *Feedback* for a *Submission*, which are
         all attached to a *Report*. A *Resolver* can then transform that Feedback into
         something that an *Environment* can hand off to a learner (or other interested
         party). These Feedback Functions are organized into *Tools*.
         
-        .. image:: docsrc/_static/pedal-overview-v3.png
+        .. image:: https://raw.githubusercontent.com/pedal-edu/pedal/master/docsrc/_static/pedal-overview-v3.png
         
         One of our major goals is to attach metadata to feedback to enable easier
         analysis, versioning, and evaluation. Although Instructor Control Scripts can
         be written very imperatively to specify very complex (or simple) grading logic,
         we are trying to reach an elegant, declarative style. This will enable tooling
         to automatically generate reports on occurrences of feedback, connect to
         datasets like those in the ProgSnap format, and allow us to "unit test our
```

### Comparing `pedal-2.4.0/Pedal.egg-info/SOURCES.txt` & `pedal-2.4.1/Pedal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/README.rst` & `pedal-2.4.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 Pedal revolves around providing *Feedback Functions* that can be called in an
 Instructor Control Script to generate *Feedback* for a *Submission*, which are
 all attached to a *Report*. A *Resolver* can then transform that Feedback into
 something that an *Environment* can hand off to a learner (or other interested
 party). These Feedback Functions are organized into *Tools*.
 
-.. image:: docsrc/_static/pedal-overview-v3.png
+.. image:: https://raw.githubusercontent.com/pedal-edu/pedal/master/docsrc/_static/pedal-overview-v3.png
 
 One of our major goals is to attach metadata to feedback to enable easier
 analysis, versioning, and evaluation. Although Instructor Control Scripts can
 be written very imperatively to specify very complex (or simple) grading logic,
 we are trying to reach an elegant, declarative style. This will enable tooling
 to automatically generate reports on occurrences of feedback, connect to
 datasets like those in the ProgSnap format, and allow us to "unit test our
```

### Comparing `pedal-2.4.0/pedal/assertions/__init__.py` & `pedal-2.4.1/pedal/assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/assertions/classes.py` & `pedal-2.4.1/pedal/assertions/classes.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/assertions/commands.py` & `pedal-2.4.1/pedal/assertions/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/assertions/feedbacks.py` & `pedal-2.4.1/pedal/assertions/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/assertions/functions.py` & `pedal-2.4.1/pedal/assertions/functions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/assertions/organizers.py` & `pedal-2.4.1/pedal/assertions/organizers.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/assertions/runtime.py` & `pedal-2.4.1/pedal/assertions/runtime.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/assertions/setup.py` & `pedal-2.4.1/pedal/assertions/setup.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/assertions/static.py` & `pedal-2.4.1/pedal/assertions/static.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/assertions/unittest.py` & `pedal-2.4.1/pedal/assertions/unittest.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/cait/ast_helpers.py` & `pedal-2.4.1/pedal/cait/ast_helpers.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/cait/ast_map.py` & `pedal-2.4.1/pedal/cait/ast_map.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/cait/cait_api.py` & `pedal-2.4.1/pedal/cait/cait_api.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/cait/cait_node.py` & `pedal-2.4.1/pedal/cait/cait_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/cait/find_node.py` & `pedal-2.4.1/pedal/cait/find_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/cait/stretchy_tree_matching.py` & `pedal-2.4.1/pedal/cait/stretchy_tree_matching.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/command_line/command_line.py` & `pedal-2.4.1/pedal/command_line/command_line.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/command_line/mocks.py` & `pedal-2.4.1/pedal/command_line/mocks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/command_line/modes.py` & `pedal-2.4.1/pedal/command_line/modes.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/command_line/report.py` & `pedal-2.4.1/pedal/command_line/report.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/command_line/verify.py` & `pedal-2.4.1/pedal/command_line/verify.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/core/commands.py` & `pedal-2.4.1/pedal/core/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/core/environment.py` & `pedal-2.4.1/pedal/core/environment.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/core/errors.py` & `pedal-2.4.1/pedal/core/errors.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/core/feedback.py` & `pedal-2.4.1/pedal/core/feedback.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/core/feedback_category.py` & `pedal-2.4.1/pedal/core/feedback_category.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/core/final_feedback.py` & `pedal-2.4.1/pedal/core/final_feedback.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/core/formatting.py` & `pedal-2.4.1/pedal/core/formatting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/core/location.py` & `pedal-2.4.1/pedal/core/location.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/core/report.py` & `pedal-2.4.1/pedal/core/report.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/core/resolver.py` & `pedal-2.4.1/pedal/core/resolver.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/core/scoring.py` & `pedal-2.4.1/pedal/core/scoring.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/core/submission.py` & `pedal-2.4.1/pedal/core/submission.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/core/tool.py` & `pedal-2.4.1/pedal/core/tool.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/environments/__init__.py` & `pedal-2.4.1/pedal/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/environments/blockpy.py` & `pedal-2.4.1/pedal/environments/blockpy.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/environments/gradescope.py` & `pedal-2.4.1/pedal/environments/gradescope.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/environments/jupyter.py` & `pedal-2.4.1/pedal/environments/jupyter.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/environments/nbgrader.py` & `pedal-2.4.1/pedal/environments/nbgrader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/environments/sandbox.py` & `pedal-2.4.1/pedal/environments/sandbox.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/environments/standard.py` & `pedal-2.4.1/pedal/environments/standard.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/environments/vpl.py` & `pedal-2.4.1/pedal/environments/vpl.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/extensions/microbit.py` & `pedal-2.4.1/pedal/extensions/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/extensions/plotting.py` & `pedal-2.4.1/pedal/extensions/plotting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/questions/__init__.py` & `pedal-2.4.1/pedal/questions/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/questions/feedbacks.py` & `pedal-2.4.1/pedal/questions/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/questions/graders.py` & `pedal-2.4.1/pedal/questions/graders.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/questions/loader.py` & `pedal-2.4.1/pedal/questions/loader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/questions/pool.py` & `pedal-2.4.1/pedal/questions/pool.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/questions/questions.py` & `pedal-2.4.1/pedal/questions/questions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/questions/setup.py` & `pedal-2.4.1/pedal/questions/setup.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/resolvers/__init__.py` & `pedal-2.4.1/pedal/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/resolvers/core.py` & `pedal-2.4.1/pedal/resolvers/core.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/resolvers/full.py` & `pedal-2.4.1/pedal/resolvers/full.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/resolvers/sectional.py` & `pedal-2.4.1/pedal/resolvers/sectional.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/resolvers/simple.py` & `pedal-2.4.1/pedal/resolvers/simple.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/resolvers/statistics.py` & `pedal-2.4.1/pedal/resolvers/statistics.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/sandbox/__init__.py` & `pedal-2.4.1/pedal/sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/sandbox/commands.py` & `pedal-2.4.1/pedal/sandbox/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/sandbox/data.py` & `pedal-2.4.1/pedal/sandbox/data.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/sandbox/exceptions.py` & `pedal-2.4.1/pedal/sandbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/sandbox/feedbacks.py` & `pedal-2.4.1/pedal/sandbox/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/sandbox/library/designer.py` & `pedal-2.4.1/pedal/sandbox/library/designer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/sandbox/library/matplotlib.py` & `pedal-2.4.1/pedal/sandbox/library/matplotlib.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/sandbox/library/microbit.py` & `pedal-2.4.1/pedal/sandbox/library/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/sandbox/library/turtles.py` & `pedal-2.4.1/pedal/sandbox/library/turtles.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/sandbox/mocked.py` & `pedal-2.4.1/pedal/sandbox/mocked.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,24 +194,24 @@
     _ORIGINAL_STDOUT = sys.stdout
 
     def __init__(self, stdout=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._original_stdout = self._ORIGINAL_STDOUT if stdout is None else stdout
 
     def write(self, s):
-        """
-
-        Args:
-            s:
-
-        Returns:
-
-        """
-        super().write(s)
         self._original_stdout.write(s)
+        return super().write(s)
+
+    def flush(self):
+        self._original_stdout.flush()
+        return super().flush()
+
+    def writelines(self, lines):
+        self._original_stdout.writelines(lines)
+        return super().writelines(lines)
 
 
 def make_fake_output(also_print=False) -> StringIO:
     """
     Creates a fake output stream that can be used to capture the output
     of a function. This is useful for testing functions that print things.
```

### Comparing `pedal-2.4.0/pedal/sandbox/result.py` & `pedal-2.4.1/pedal/sandbox/result.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/sandbox/sandbox.py` & `pedal-2.4.1/pedal/sandbox/sandbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,38 +192,42 @@
         else:
             self._stop_mocking(context)
 
         self._next_context_id += 1
         return self
 
     def run(self, code=None, filename=None, inputs=None, threaded=None,
-            after=None, before=None):
+            after=None, before=None, real_io=False):
         """
         If both ``code`` and ``filename`` are None, then the submission's
         main file will be executed. If ``code`` is given but ``filename`` is
         not, then it is assumed to be instructor code.
 
         TODO: This should actually return the ExecutionContext that was generated, right?
             But the user should be able to treat that as if it were the Sandbox...
 
         Args:
+            real_io: If True, makes print and input actually write to stdout.
             code (str or :py:class:`~pedal.cait.cait_node.CaitNode` or None):
                 The code to execute.
             filename (str or None): The filename to use for this code.
             inputs (list[str]): Optional inputs to be passed to
                 :py:func:`~pedal.sandbox.Sandbox.set_input`.
             threaded (bool): Whether or not to run this code in a threaded
                 environment, which allows for timeouts.
             after (str): Code to run after this code (without a filename).
             before (str): Code to run before this code (without a filename).
 
 
         Returns:
             Sandbox: This sandbox instance.
         """
+        if real_io:
+            self.allow_function('print')
+            self.set_input(input)
         if threaded is None:
             threaded = self.threaded
         if code is None:
             if filename is None:
                 filename = self.report.submission.main_file
             code = self.report.submission.files[filename]
         elif filename is None:
@@ -232,14 +236,17 @@
             self.set_input(inputs)
         if before is not None:
             self._execute(before, filename, SandboxContextKind.RUN, threaded)
         self.target = None
         self._execute(code, filename, SandboxContextKind.RUN, threaded)
         if after is not None:
             self._execute(after, filename, SandboxContextKind.RUN, threaded)
+        if real_io:
+            self.clear_mocked_function('print')
+            self.clear_input()
         return self
 
     def call(self, function, *args, target="_", threaded=None,
              inputs=None, function_kwargs=None,
              args_locals=None, kwargs_locals=None, **kwargs):
         """
         Execute the given function from the student's namespace.
@@ -600,15 +607,16 @@
     def clear_mocked_function(self, function_name):
         """
         Removes the mocking associated with the given function name.
 
         Args:
             function_name (str): The name of the function to be mocked.
         """
-        del self._module_overrides['__builtins__'][function_name]
+        if function_name in self._module_overrides['__builtins__']:
+            del self._module_overrides['__builtins__'][function_name]
 
     def allow_module(self, module_name):
         """
 
         Args:
             module_name (str):
```

### Comparing `pedal-2.4.0/pedal/sandbox/timeout.py` & `pedal-2.4.1/pedal/sandbox/timeout.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/sandbox/tracer.py` & `pedal-2.4.1/pedal/sandbox/tracer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/source/__init__.py` & `pedal-2.4.1/pedal/source/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/source/feedbacks.py` & `pedal-2.4.1/pedal/source/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/source/sections.py` & `pedal-2.4.1/pedal/source/sections.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/source/source.py` & `pedal-2.4.1/pedal/source/source.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/tifa/__init__.py` & `pedal-2.4.1/pedal/tifa/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/tifa/commands.py` & `pedal-2.4.1/pedal/tifa/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/tifa/contexts.py` & `pedal-2.4.1/pedal/tifa/contexts.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/tifa/feedbacks.py` & `pedal-2.4.1/pedal/tifa/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/tifa/identifier.py` & `pedal-2.4.1/pedal/tifa/identifier.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/tifa/settings.py` & `pedal-2.4.1/pedal/tifa/settings.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/tifa/state.py` & `pedal-2.4.1/pedal/tifa/state.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/tifa/tifa_core.py` & `pedal-2.4.1/pedal/tifa/tifa_core.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/tifa/tifa_visitor.py` & `pedal-2.4.1/pedal/tifa/tifa_visitor.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/types/builtin.py` & `pedal-2.4.1/pedal/types/builtin.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/types/library/cs1_curriculum.py` & `pedal-2.4.1/pedal/types/library/cs1_curriculum.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/types/library/designer.py` & `pedal-2.4.1/pedal/types/library/designer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/types/library/matplotlib.py` & `pedal-2.4.1/pedal/types/library/matplotlib.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/types/library/microbit.py` & `pedal-2.4.1/pedal/types/library/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/types/new_types.py` & `pedal-2.4.1/pedal/types/new_types.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/types/normalize.py` & `pedal-2.4.1/pedal/types/normalize.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/types/operations.py` & `pedal-2.4.1/pedal/types/operations.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/utilities/__init__.py` & `pedal-2.4.1/pedal/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/utilities/ast_tools.py` & `pedal-2.4.1/pedal/utilities/ast_tools.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/utilities/comparisons.py` & `pedal-2.4.1/pedal/utilities/comparisons.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/utilities/dictionaries.py` & `pedal-2.4.1/pedal/utilities/dictionaries.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/utilities/exceptions.py` & `pedal-2.4.1/pedal/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/utilities/files.py` & `pedal-2.4.1/pedal/utilities/files.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/utilities/operators.py` & `pedal-2.4.1/pedal/utilities/operators.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/utilities/progsnap.py` & `pedal-2.4.1/pedal/utilities/progsnap.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/utilities/sorting.py` & `pedal-2.4.1/pedal/utilities/sorting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/utilities/text.py` & `pedal-2.4.1/pedal/utilities/text.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/pedal/utilities/types.py` & `pedal-2.4.1/pedal/utilities/types.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.0/setup.py` & `pedal-2.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='pedal',
-    version='2.4.0',
+    version='2.4.1',
     python_requires='>=3.6',
     author='acbart,lukesg08',
     author_email='acbart@udel.edu',
     description='Tools to provide feedback on student code.',
     keywords='feedback education teaching program analysis tifa cait sandbox pedal grading grader grade',
     packages=['pedal', 'pedal.core', 'pedal.utilities', 'pedal.environments',
               'pedal.resolvers', 'pedal.command_line',
```

